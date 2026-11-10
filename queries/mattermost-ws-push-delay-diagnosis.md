---
title: Mattermost 채팅 "답변이 늦게 보임" WebSocket 수신 지연 진단
created: 2026-11-10
updated: 2026-11-10
type: query
tags: [networking, web-server, debugging, linux, system-admin, docker]
sources: [raw/books/inside-tcpip.txt]
confidence: high
---

# Mattermost 채팅 "답변이 늦게 보임" WebSocket 수신 지연 진단

> 2026-11-10 실습 기록. 자체호스트 Mattermost(브라우저 접속)에서 보트(에이전트)의
> 답변이 즉시 표시되지 않고, **다른 채널로 이동했다가 다시 오면(또는 강제 새로고침하면)
> 보인다는** 보고를 받아, 서버↔브라우저 경로를 구간별로 증거로 분리한 진단 전 과정.
> 결론: 서버·네트워크 모두 정상, **브라우저 측 WebSocket 수신이 유휴 시점에 중단**되는 것이 원인.

## 증상 (원점)

- 채널에 보트의 답변이 **즉시 안 보임**.
- 다른 채널로 갔다 와서(=채널 재진입, WS 재구독) 메시지가 나타남.
- "나머지" 메시지는 **나가는 쪽(사용자→서버)은 즉시**, 들어오는 쪽만 지연.

## 진단 방법론: 경로를 3구간으로 분리

1구간 **에이전트 게이트웨이 → Mattermost API** (HTTP POST)
2구간 **Mattermost 앱 → WebSocket 허브 → 클라이언트** (WS push)
3구간 **브라우저 WS 수신 → 화면 렌더링**

각 구간을 독립 증거로 판정하되, 어느 구간이든 단정짓지 않고 **증거 우선**:

### 1구간 — 게이트웨이: 즉시 전송 확인 (정상)
게이트웨이 로그(`logs/agent.log`)에서 수신 시각과 전송 시각이 붙어 있음:
```
23:40:31,898 inbound message: platform=mattermost ... msg='두개의 명령어를 입력했습니다.'
23:40:34,900 response ready: ... time=3.0s ... response=354 chars
23:40:34,919 [Mattermost] Sending response (354 chars) to uh6axx...
```
→ 게이트웨이는 수신 후 3초 만에 HTTP POST로 보냄. 1구간 무결.

### 2구간 — 서버: WS 드롭/에러 0건, DB에 저장 확인 (정상)
- `docker logs mattermost-app --since 4h | grep -iE "drop|slow|queue"` → **0건**
- 앱 컨테이너 `Up ... (healthy)`; 클라이언트 WS close만 서버 재시작(본인 작업) 시점의 hub stop/start뿐.
- 결정적 증거 — **posts 테이블 직접 조회**(DB에 저장 = 전송 완료):
  ```
  docker exec mattermost-postgres psql -U mmuser -d mattermost -t -c \
   "select to_timestamp(createat/1000+9*3600) as kst, left(message,80)
    from posts where channelid='<채널id>' and deleteat=0 order by createat desc limit 5;"
  ```
  → "보이지 않는다"는 메시지가 DB에 전부 존재. 2구간 무결.
- 채널 멤버십도 정상: `channels` 타입 `D`/`O` 각각 `deleteat=0`, `channelmembers` 2명 정상.

### 3구간 — 브라우저: 수신 중단이 원인 (판정)
- 대조 테스트: **다른 채널(hermes-test)에서는 즉시 표시**, 해당 DM 채널에서만 지연.
  → 채널 멤버십/서버측 문제 아님(서버측은 위 1·2구간에서 모두 정상 확인).
- 재현 패턴: `Ctrl+Shift+R`(강제 새로고침 = WS 세션 재확립) 하면 즉시 표시,
  유휴 방치하면 다시 지연 → **WS 세션이 살아 있음에도 브라우저가 이벤트를 드롭**하는 패턴.
- 접속 환경: LAN 케이블, 웹 브라우저(Chrome/Linux), 프록시·터널 없음 → 중간장비 원인은 배제.

## 원인 (판정)

브라우저가 유휴/백그라운드 탭의 **WebSocket 수신(이벤트 pump)을 중단**시키는 상태.
채널 전환·페이지 리로드는 WS 재연결을 일으키므로 밀린 메시지가 한 번에 복귀 —
"다른 채널로 갔다와야 보인다"의 정확 메커니즘. (WebSocket·TCP/IP 구조 배경: [[tcp-ip]],
[[socket-programming-patterns]] 참고.)

## 해결 (검증순서대로)

1. **`chrome://settings/performance` → 메모리 절약(Memory Saver) 끄기**,
   또는 설정의 "제외 사이트"에 접속하는 사이트만 추가(사이트 보존).
2. 재발 시 **시크릿 창**에서 접속하여 시험 → 정상이면 **확장 프로그램**(광고 차단기 우선)
   중 하나가 WebSocket을 가로챈 것; 확장을 하나씩 끄며 특정.
3. 검증: 수리 후 해당 채널 **10~15분 방치**, 이후 메시지가 즉시 표시되면 완결.

## 재사용 체크리스트 (채팅앱 "들어오는 메시지 지연" 공통)

- [ ] 게이트웨이/앱 로그: 수신→전송 시각차 (구간A)
- [ ] 서버 로그 WS drop/slow/queue 0건 여부 (구간B)
- [ ] DB `posts`에 메시지 저장 여부 = 전송 완료 판정 (구간B)
- [ ] 채널 멤버십·`deleteat` 정상 여부
- [ ] **다른 채널(또는 다른 기기) 대조** — 채널 특화 vs 클라이언트 공통 구분
- [ ] 강제 새로고침/채널 재진입 시 복귀하면 → 클라이언트 WS 수신(구간C)
- [ ] 프록시·터널·VPN 경유 여부 확인 (중간장비 WS 타임아웃의 흔한 원인)
- [ ] 브라우저 에너지 절약/탭 수면/확장(광고 차단) 점검

## 교훈

- "서버가 느린가, 클라이언트가 보이는가"를 **구간 분리 + DB 직접 조회**로 판정할 것 —
  전송 완료(DB 저장)를 기준으로 서버 무결을 먼저 증명하는 것이 핵심.
- WebSocket 기반 채팅의 "지연"은 **대부분 수신측(브라우저) 이벤트 드롭**이며,
  채널 전환·리로드가 수복하는 패턴 수신측 증상.

## Related

- [[tcp-ip]] — TCP/UDP·계층 구조 (수신측 패킷/이벤트 처리 배경)
- [[socket-programming-patterns]] — 소켓 통신 패턴
- [[docker-wordpress-mysql-debug]] — 같은 queries/ 형식의 실측 진단 기록
- [[local-area-network]] — LAN/브리지(접속 경로 배경)
