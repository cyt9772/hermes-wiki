---
title: WinSock API
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [sockets, networking, windows-api]
sources: [raw/books/winsock-network-programming.md, raw/books/computer-network-programming.md]
confidence: high
---
# WinSock API

Windows에서 BSD Socket API를 구현한 표준. WinSock 1 (16-bit) → **WinSock 2 (32-bit)** — winsock2.h, WSAStartup/WSACleanup 명시 필요. ^[raw/books/winsock-network-programming.md]

## 핵심 호출 (기본 흐름)
- `socket()` — 소켓 번호; `AF_INET`, `SOCK_STREAM`(TCP)/`SOCK_DGRAM`(UDP)
- `bind()`/`listen()`/`accept()` — 서버; `connect()` — 클라이언트
- `send()`/`recv()` (스트림) · `sendto()`/`recvfrom()` (데이터그램)
- 지원 루틴: 바이트 순서 변환 `htons/htonl/ntohs/ntohl`, 에러 보고 `WSAGetLastError()` ^[raw/books/winsock-network-programming.md]

## 동작 3모드 (Ch.5)
- **Blocking** (기본, "Blocking is Real"), **Nonblocking**, **Asynchronous (WSAAsyncSelect)** — 이벤트 기반 ^[raw/books/winsock-network-programming.md]

## BSD와의 포팅 차이 (Ch.12)
- 16-bit Windows 고려사항, 함수명 차이 — `htons` 등 지원 함수, `ioctlsocket` ↔ `ioctl` ^[raw/books/winsock-network-programming.md]
- Unix/Win 환경 비교: [[computer-network-programming-book]] (3.8 윈속)

## Related
- [[socket-programming-patterns]]
- [[windows-sockets-network-programming]] (main source)
- [[winsock-bsd-compare]]
- [[bob-quinn]] · [[dave-shute]] (authors)