---
title: WinSock vs BSD Sockets
created: 2026-10-18
updated: 2026-10-18
type: comparison
tags: [sockets, windows-api]
sources: [raw/books/winsock-network-programming.md, raw/books/computer-network-programming.md]
confidence: high
---
# WinSock vs BSD Sockets

BSD Socket API의 Windows 구현 — 포팅 시 차이 (winsock-network-programming Ch.12).

| 항목 | BSD (Unix) | WinSock |
|------|-----------|---------|
| 헤더/라이브러리 | `<sys/socket.h>` | `winsock.h` (WS1) / `winsock2.h` (WS2) |
| 초기화 | 불필요 | `WSAStartup`/`WSACleanup` 명시 |
| 에러 | `errno` · `perror` | `WSAGetLastError()` · `WSASetLastError` |
| 파일 디스크립터 | int / fd_set | SOCKET (`unsigned int`) · `FD_SETSIZE` |
| ioctl | `ioctl` | `ioctlsocket` |
| 비동기 | select, signals, async/IO | select(), WSAAsyncSelect(), blocking hooks |
| 16/32-bit | - | 16-bit Windows (WS1) ↔ 32-bit (WS2) 고려 |
| 플랫폼 | Unix 계열 | Win32 (WOSA 모델, 다른 플랫폼 지원) |

- 공통: socket/connect/bind/listen/accept/send/recv, 바이트 순서 htons/htonl/ntohs/ntohl — 양측 동일. ^[raw/books/winsock-network-programming.md]
- Unix/Win 프로그래밍 환경 비교: [[computer-network-programming-book]] 1.4 (p.32-37)
- "Incidentals" + Functions List (Ch.12.3-12.4) — 포팅 체크리스트.

## Related
- [[winsock-api]]
- [[socket-programming-patterns]]
- [[windows-sockets-network-programming]]