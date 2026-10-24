---
title: Bluetooth: Connect Without Cables (Bray & Sturman 2001)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, bluetooth-wpan, telecom-systems, wireless-communications]
sources: [raw/books/bluetooth-connect-without-cables.md]
confidence: high
---
# Bluetooth: Connect Without Cables (Bray & Sturman 2001, Pearson)

> 표지/원저: **Jennifer Bray** · **Charles F. Sturman** (원저)
> 번역: 이문수, 강치운, 오종택, 이정재, 변건식
> 출판: 원저 — Prentice Hall PTR (Pearson), 2001; 한국어판 — Pearson Education Korea + 홍릉과학출판사, 2001, 535p

## 개요
블루투스 1.0B 규격 기반의 실무 교재. "안테나로부터 시작하여 프로토콜 스택과 그것과의 인터페이스, 각종 응용과 호스트 사용자 인터페이스에 이르기까지" 블루투스 기술을 완전하게 다루며 `[raw/books/bluetooth-connect-without-cables.md]`, 타이밍 조건·규격 권고안과 실제 구현 간 차이·workaround·옵션 선택까지 포함. 저자들이 고객연수(first-day) 후 브뤼셀에서 "블루투스에 관한 책을 써야 한다"고 합의하여 기획된 것으로 서문(머리말 II)에서 밝히고 있다.

## 장 구조 (TOC 기반, 535p)
1. **개요** — 기원·SIG·목적·프로토콜 스택·보안·프로파일·시험승인
2. **안테나** — 방사 패턴, 이득/손실, 종류, 칩 안테나, 장착
3. **무선 인터페이스 RF** — 주파수 호핑, 변조, 심볼 타이밍, 출력 제한, RF 구조
4. **베이스밴드** — 장치 주소, 마스터/슬레이브/피코넷, SCO/ACL, 패킷 구조·부호화, 시간 동기
5. **링크 제어기** — LMP, 링크 상태, 피코넷/스코터넷, 저전력
6. **오디오** — SCO 링크, 오디오 코덱, 서브시스템
7. **링크 관리자** — LMP PDU, 링크 설정, 보안, QoS
8. **HCI** — 패킷, 트랜스포트, 흐름제어, 모듈 구성
9. **L2CAP** — 다중화, 신호화, 접속 설정/구성/단절
10. **RFCOMM** — 직렬 포트 에뮬레이션
11. **SDP** — 서비스 발견 (클라이언트/서버, 데이터베이스, UUID)
12. **WAP** — 무선 접속 프로토콜
13. **OBEX/IrDA** — 객체 교환
14. **TCS** — 전화 제어
15. **블루투스 프로파일** — GAP/SPP/FAX/HS/LAN/OPP/FTP/sync/intercom/cordless telephony
16. **암호화·보안** — 키 생성, 페어링, 본딩, 보안 모드
17. **저전력** — hold/sniff/park 모드
18. **QoS** — 요청/위반, flush, link supervision
19. **시험과 승인** — 적합성/형식승인
20. **시험 모드** — test mode

## 핵심 내용
- 프로토콜 스택을 세 부(블루투스 모듈 / 블루투스 호스트 / cross-layer) + 시험과 시장 맥락 4부분으로 구성 `[raw/books/bluetooth-connect-without-cables.md]`
- 주파수 호핑·GFSK 변조·SCO/ACL 물리링크 등 RF 및 베이스밴드 핵심 메커니즘 상세 설명 `[raw/books/bluetooth-connect-without-cables.md]`
- L2CAP → RFCOMM → SDP → WAP/OBEX/TCS 계층 구조와 상호작용 실용 가이드 `[raw/books/bluetooth-connect-without-cables.md]`
- 페어링·본딩·보안 모드·키 교환 실무 워크플로우 `[raw/books/bluetooth-connect-without-cables.md]`
- 저전력 모드(hold/sniff/park)와 QoS 관리 구현 팁 `[raw/books/bluetooth-connect-without-cables.md]`
- 시험·승인(qualification) 프로세스 — 프로덕트 인증 준비 `[raw/books/bluetooth-connect-without-cables.md]`

## 관련
- 저자: [[jennifer-bray]] · [[charles-sturman]]
- 개념: [[lte-radio-interface]] — LTE 무선 접속 (차세대 이동통신; 블루투스는 WPAN 단)
- 인접: [[bluetooth-explained]] (MCPC, 신구문화사 2001) — 블루투스 해설서
- 인접: [[cdma-dss-spread-spectrum]] — 확산 스펙트럼 (블루투스 FHSS와 대비)
- 인접: [[rf-engineering]] · [[microwave-engineering]] — RF 회로
