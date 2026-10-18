---
title: TCP/IP 완전정복 (Inside TCP/IP)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, tcp-ip]
sources: [raw/books/inside-tcpip.md]
confidence: high
---
# TCP/IP 완전정복 (Inside TCP/IP)

Karanjit S. Siyan 저, 이도희 옮김, 성안당(Seoandang) 2001-06 1쇄. 원서 **Inside TCP/IP**, New Riders (Macmillan Computer Publishing) 1997. **TCP/IP 프로토콜 계층 구조·주소지정·라우팅·응용프로그래밍 표준서.** 15장 + 4부.

## 인용 (pg6, Part I)
> "TCP/IP 네트워크의 개요 — TCP/IP란? TCP/IP: 과거와 현재, DARPA의 역할, 초기의 DARPA 실험, ARPAnet의 진화, 독자적 네트워크에서 개방형 TCP/IP 네트워크로 변천, 멀티 벤더 네트워크, TCP/IP의 숨은 추진력"

## 구성 (4 Part / 15 Chapter)
| Part | Chapter |
|------|---------|
| Part I TCP/IP 계층화 모델과 물리적 기반 (p.1) | 1 TCP/IP 소개 (p.9) · 2 프로토콜 계층화 (p.43) · 3 네트워크 지원 (p.81) — LAN(이더넷·토큰링·FDDI), 리피터/브리지/라우터 |
| Part II TCP/IP 인터네트워킹 기반 (p.171) | 4 IP 주소 지정 (p.173) · 5 주소 결정 프로토콜 (ARP, p.213) · 6 인터넷 프로토콜 (IP, p.259) — 헤더·단편화·옵션·바이트 순서 · 7 IP 경로 설정 (p.311) · 8 ICMP (p.342) · 9 서브넷화/슈퍼넷화 (p.391) · 10 경로 설정 프로토콜 (p.437) · 11 전송 프로토콜 (p.475) |
| Part III TCP/IP 응용프로그램 서비스 (p.541) | 12 자동 구성 (p.543) — DHCP·SLP · 13 응용프로그램 APIs (p.577) — WinSock·BSD Sockets 비교 · 14 네트워크 관리 (p.655) — SNMP, MIB, Managed Nodes |
| Part IV 미래의 방향 (p.675) | 15 IP의 차세대와 ATM (p.677), 표준 프로토콜 (p.705) |

## 핵심 개념
- **DoD 모델** vs **OSI 모델** (Chapter 2) — 프로토콜 다중화/개별화, TCP/IP 구현과 호스트 OS
- **주소**: NSAP → IP, 클래스 A/B/C/D/E, 점십진, 특수 주소 (This Network·Broadcast·Loopback), 개별/동보/다중 전송 (Chapter 4)
- **IP 헤더** — Version·IHL·Type of Service·Total Length·Flags/Fragment Offset·TTL·Protocol·Header Checksum, 옵션 (Chapter 6)
- **ICMP** — Echo Request/Reply, Destination Unreachable, Time Exceeded, Redirect (Chapter 8)
- **DHCP** — DORA (Discover/Offer/Request/Ack), Dynamic DNS (Chapter 12)
- **SNMP** — MIB, Get/GetNext/Set/Trap, Managed Agent (Chapter 14)

## Related
- [[tcp-ip]] (concept)
- [[osi-7-layer-model]] (기존)
- [[karanjit-siyan]] (author)
- [[windows-sockets-network-programming]] (API)
- [[tcpip-network-programming]] (실험)
