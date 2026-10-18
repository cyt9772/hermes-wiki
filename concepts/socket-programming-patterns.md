---
title: Socket Programming Patterns
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [sockets, network-programming]
sources: [raw/books/winsock-network-programming.md, raw/books/computer-network-programming.md, raw/books/tcpip-network-programming.md]
confidence: high
---
# 소켓 프로그래밍 패턴

TCP(연결형 스트림) vs UDP(비연결형 데이터그램) 서버-클라이언트 호출 순서.

## TCP 서버 (연결형)
socket → bind → listen → accept(반복) → send/recv close. ^[raw/books/computer-network-programming.md]
## TCP 클라이언트
socket → connect → send/recv → close.

## UDP (비연결형)
socket → (bind) → sendto / recvfrom — 연결 상태 없음, 각 datagram 독립. ^[raw/books/tcpip-network-programming.md]

## 핵심 관행
- **연결형 클라이언트·서버 작성 절차** vs **비연결형** ([[computer-network-programming-book]] Ch.2.3-2.4) ^[raw/books/computer-network-programming.md]
- **select()** — 다중 소켓 이벤트 대기; [[computer-network-programming-book]] Ch.3.2 (채팅 서버), [[windows-sockets-network-programming]] Ch.6 ^[raw/books/computer-network-programming.md]
- SO_REUSEADDR, 데몬/inetd 서버 구축, 멀티캐스트 — [[computer-network-programming-book]] Ch.3.4-3.6
- **동작 3모드**: Blocking/Nonblocking/Asynchronous — [[winsock-api]]

## Related
- [[winsock-api]]
- [[computer-network-programming-book]]
- [[windows-sockets-network-programming]]