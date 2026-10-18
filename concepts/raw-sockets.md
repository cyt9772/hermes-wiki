---
title: Raw Sockets
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [sockets, tcp-ip]
sources: [raw/books/tcpip-network-programming.md, raw/books/winsock-network-programming.md]
confidence: high
---
# Raw Sockets

OS 프로토콜 스택을 우회(또는 부분 우회)해 **IP/TCP/UDP/ICMP 헤더를 프로그램이 직접 작성·분석**하는 소켓.

## 용도 (실험·교육)
- 프로토콜 동작 검증: Ethernet 헤더·ARP·IP·ICMP 직접 송수신. ^[raw/books/tcpip-network-programming.md]
- 실험 프로그램: scanhost, scanport_tcp, arpupdate, redirect (ICMP) ^[raw/books/tcpip-network-programming.md]
- IPv6 헤더·소켓 (FreeBSD 기준) ^[raw/books/tcpip-network-programming.md]

## WinSock 옵션 (Ch.16)
Raw Sockets, Multicast, Loopback, Sockets as File Handles — "Optional Standard Is an Oxymoron" 원칙: 표준에 없는 기능은 구현별 차이 확인. ^[raw/books/winsock-network-programming.md]

## Related
- [[tcp-ip]]
- [[tcpip-network-programming]]
- [[winsock-api]]