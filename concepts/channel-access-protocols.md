---
title: 채널 액세스 프로토콜 (Channel Access Protocols)
created: 2026-10-15
updated: 2026-10-18
type: concept
tags: [networking, data-communication]
sources: [raw/books/lan-van-isdn.md, raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 채널 액세스 프로토콜

공유 매체를 여러 단말이 어떻게 사용할 것인가를 정한 규칙. 이 책 4장에서 **고정/임의/요구 할당** 세 분류로 체계화하고, LAN(7장)의 체제에 적용한다.

> "제4장 채널 액세스 프로토콜의 분류 … 4.2 고정 할당 프로토콜 / 4.3 임의 할당 프로토콜 / 4.4 요구 할당 프로토콜 / 4.5 채널 액세스 프로토콜의 성능 비교" `[raw/books/lan-van-isdn.md]` TOC p.5

## 세 가지 분류
| 분류 | 원리 | 예 |
|------|------|-----|
| **고정 할당 (Fixed Assignment)** | 시간/주파수 슬롯을 고정 배정 | TDM, FDM, 고정 슬롯 |
| **임의 할당 (Random Assignment)** | 충돌 허용하되 재전송으로 복구 | ALOHA, CSMA, CSMA/CD |
| **요구 할당 (Demand Assignment)** | 필요 시 접근권 요청 | Token Ring(토큰 회수/발급) |

## 대표 예
- **CSMA/CD** (경쟁 탐지-충돌 탐지) — 이더넷 계열. 임의 접근. `Carrier Sense Multiple Access / Collision Detection`
- **Token Ring** — 토큰(접근권)을 순환시키며, 토큰을 소유한 단말만 전송. 요구 접근. 충돌 회피, 대칭성

## 성능 비교 (4.5)
- 충돌 허용형(임의) — 부하가 낮을 때 효율, 높아지면 충돌 증가로 급감
- 토큰 기반(요구) — 부하 높을 때 안정, 지연이 고정적

## 이동통신 다중접속 시뮬레이션 (추가)
[[latest-mobile-comm-systems]] 제6장: 무선 이동통신에서의 임의 할당 접근 —
- **순수 ALOHA** (6.5): 전 구간 전송, 충돌 시 재전송 (원리 6.5.1, 시뮬레이션 6.5.2, 결과 6.5.3)
- **슬롯화된 ALOHA** (6.6): 슬롯 정렬로 효율 37%/18.3% → ~54%
- **비경합 CSMA** (6.7): carrier sense로 충돌 사전 감소
- **슬롯화된 CSMA** (6.8): 슬롯 정렬 + carrier sense
- MATLAB: `feval(char(protocol(pno)))` 부프로그램 교체로 프로토콜 시뮬레이션 공용 프레임워크 (p.334)
- 캡쳐(capture) 효과 고려 (p.334) → `capture == TRUE/FALSE` 옵션


## 관련 개념
- [[local-area-network]] — 채널 액세스를 물리/데이타링크 계층에서 구현
- [[osi-7-layer-model]] — 1~2계층(물리/데이타링크)의 핵심 문제
- [[lan-van-isdn]] (책) — 4장 분류 체계 + 7장 LAN 적용
