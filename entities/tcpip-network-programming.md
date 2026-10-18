---
title: 기초부터 배우는 TCP/IP 네트워크 실험 프로그래밍 (Kiso kara Wakaru TCP/IP Network Jikken Programming)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, tcp-ip, sockets]
sources: [raw/books/tcpip-network-programming.md]
confidence: high
---
# 기초부터 배우는 TCP/IP 네트워크 실험 프로그래밍

Murayama Yukio (무라야마 유키오) 저, 송봉길 역, 원서 Ohmsha (오옴사·日本) 2001 "Kiso kara Wakaru TCP/IP Network Jikken Programming", 한국어판 오옴사·성안당 공동출간 2005 (C언어). **C 소켓으로 TCP/IP 패킷을 직접 만들어 실험하는 프로그래밍서.**

## 인용 (pg10, 제1장 서두)
> "네트워크 프로그래밍을 하기 위해서 필요한 TCP/IP의 기초에 대해 배우겠습니다. … 패킷 교환의 기초 (1.1.2), 프로토콜 스택과 패킷의 처리 (1.1.6)"

## 구성 (pg10-15 차례, 확인됨)
| # | 내용 |
|---|------|
| 1 | **TCP/IP 프로토콜 스택 입문** (p.2) — 네트워크·패킷 교환·SW/HW·OS, 프로토콜 스택 구조, 클라이언트-서버 모델, IPv6 |
| 2 | **프로토콜 스택의 실질적 구현** — Ethernet (p.47) · **ARP** (p.53) · **IP** (p.60, 헤더/라우팅/fragment) · **TCP** (p.89, 커넥션/신뢰성/버퍼/윈도) · **Checksum** (p.99) |
| 3 | **소켓** — 구조체·시스템콜 (UDP vs TCP) (p.109-119) |
| 4 | *(차례 pg13 확인: UDP 통신 p.135)* — UDP 예제: 서버/클라이언트 소스+해설 |
| 5 | **TCP 통신 (p.151)** — 예제 프로그램, 처리 흐름, 서버/클라이언트 소스+해설 |
| 6 | *(차례 pg14 확인: 통신의 식별 p.212)* — 호스트 스캔 (scanhost) + TCP 포트 스캔 (scanport_tcp) |
| 7 | *(차례 pg15 확인: ARP 실험 p.252)* — **arpupdate** 프로그램: 같은 IP의 이중 호스트, ARP 태블 조작 실험 |
| 8 | *(차례 pg15 확인: IP/ICMP 실험 p.286)* — 라우팅 테이블, **redirect** 프로그램 |
| 9 | **IPv6** (pg7 언급) — IPv6 헤더·소켓 (FreeBSD 확인) |
| 10+ | 이후장: ICMP·raw socket·실전 네트워크 데몬 (차례 뒷부분) |

## 실험 환경 (pg1, pg2)
- C 언어, **Linux LASER 5.6 / FreeBSD 4.2 / macOS 10.0 / PS2 Linux** (IPv6은 FreeBSD)
- "사적 IP를 사용해서 실험 네트워크를 구축하고, 그 위에서 실험하도록" (pg9)
- 패킷 모니터링으로 Ethernet 헤더 구조 학습 권장

## Related
- [[raw-sockets]] (concept)
- [[socket-programming-patterns]]
- [[tcpip-complete]] (Siyan, 이론 중심)
- [[windows-sockets-network-programming]] (WinSock API)
- [[yukio-murayama]] (author)
