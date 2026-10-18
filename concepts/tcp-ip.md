---
title: TCP/IP Protocol Stack
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [tcp-ip, networking]
sources: [raw/books/inside-tcpip.md, raw/books/tcpip-network-programming.md]
confidence: high
---
# TCP/IP 프로토콜 스택

## 계층 (Siyan, Inside TCP/IP)
- **DoD 4계층**: 호스트-호스트 (전송) / 인터네트워크 / 네트워크 접근 / 물리 — OSI 7계층과 비교. ^[raw/books/inside-tcpip.md]
- Part I: 계층화 모델 + 물리적 기반(이더넷·토큰링·FDDI, 리피터/브리지/라우터)
- Part II: IP 주소지정(클래스 A-E) · ARP · IP 헤더(Version/IHL/TOS/Length/Flags/TTL/Checksum) · 경로 설정(ICMP) · 서브넷/슈퍼넷 · 라우팅 프로토콜(RIPv2/BGP4) · 전송 프로토콜(TCP/UDP) ^[raw/books/inside-tcpip.md]
- Part III: DHCP 자동 구성, 응용 API (WinSock vs BSD), SNMP 관리 (MIB, Get/Trap)
- Part IV: 차세대 IP + ATM

## 구현 레벨 실험 (Murayama)
- Ethernet 프레임 → ARP(주소결정) → IP(라우팅·단편화) → TCP(3-way handshake, window) — raw 소켓으로 직접 패킷 생성/수신. ^[raw/books/tcpip-network-programming.md]
- 실험 프로그램: scanhost(호스트 스캔), scanport_tcp(포트 스캔), arpupdate(ARP 테이블 조작), redirect(ICMP redirect) ^[raw/books/tcpip-network-programming.md]

## Related
- [[osi-7-layer-model]]
- [[tcpip-complete]]
- [[raw-sockets]]
- [[karanjit-siyan]] · [[yukio-murayama]]