---
title: Windows Sockets Network Programming
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, sockets, network-programming]
sources: [raw/books/winsock-network-programming.md]
confidence: high
---
# Windows Sockets Network Programming

Bob Quinn·Dave Shute 저, Addison-Wesley (Advanced Windows Series) 1996, ISBN 0-201-63372-8. **WinSock API의 개념·동작 모드·스택·실전 예제(FTP 클라이언트) 실무서.**

## 인용 (pg10, 제1장)
> "Many vendors to work together, this laid the foundation for the creation and success of the Windows Sockets API, or 'WinSock' as it has become known."

## 구성 (17장, pg6-9 차례 확인)
| # | 내용 |
|---|------|
| 1 | Introduction to Windows Sockets — WinSock란/역사/이점/미래 (p.1) |
| 2 | Windows Sockets Concepts — OSI 네트워크 모델 → WinSock 모델, Modular Boxes, Services·Protocols·APIs (p.11) |
| 3 | TCP/IP Protocol Services — Transport·Network Services, Support Protocols, Future (p.31) |
| 4 | Network Application Mechanics — Client-Server Model, Open→Name→Associate→Send/Receive→Close (p.47) |
| 5 | Operation Modes — **Blocking/Nonblocking/Asynchronous**, 성능·플랫폼 차이 (p.75) |
| 6 | Socket States — **WSAAsyncSelect() · select()**, Peeking, Out-of-Band, Listening (p.121) |
| 7 | Sample Application & Library — **Sample FTP Client** (p.178), Sample Library (p.234), WinSockx.h (p.251) |
| 8 | Host Names and Addresses — Resolution, Host Table·DNS·NIS, Local Host, Addresses·Formatting (p.257) |
| 9 | Socket Information and Control — Control, Options, **Blocking Hooks** (p.285) |
| 10 | Support Routines — Startup/Cleanup, **Byte Ordering**, Ports, Protocol Names, Error Reporting (p.319) |
| 11 | DLLs over WinSock — New API, DLL Issues, Sample DLL (p.353) |
| 12 | Porting from **BSD Sockets** — Differences, 16-bit Considerations, Functions List (p.385) |
| 13 | Debugging — Problem Types·Qualification, Installation/Network/Application, Tools (p.405) |
| 14 | Dos and Don'ts — Data Flow, Stream/Datagram Algorithms, Good-News Code, Common Traps (p.427) |
| 15 | Platforms — WOSA Network Model, 32-bit WinSock, Other Platforms (p.459) |
| 16 | Optional Features — **Raw Sockets, Multicast, Loopback, Sockets as File Handles** (p.471) |
| 17 | **WinSock 2** — Is it Needed?, Overview of Features (p.495) |

## 핵심 개념
- **동작 3모드**: Blocking (기본) / Nonblocking (SOCK_NONBLOCK? WinSock는 WSASocket flag) / **Asynchronous (WSAAsyncSelect)** — 이벤트 기반, select()는 포스크립트 스타일
- **select()**: read/write/except fd_set 체크
- **Byte ordering**: htons/htonl/ntohs/ntohl (Network Byte Order = Big-Endian)
- **BSD Sockets porting**: WinSock1는 16-bit, WinSock2는 32-bit

## Related
- [[winsock-api]] (concept)
- [[socket-programming-patterns]]
- [[bob-quinn]] · [[dave-shute]] (authors)
- [[tcpip-complete]] (이론)
- [[tcpip-network-programming]] (BSD raw 소켓 실험)
