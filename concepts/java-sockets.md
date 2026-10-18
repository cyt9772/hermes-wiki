---
title: Java Sockets
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [sockets, network-programming]
sources: [raw/books/computer-network-programming.md]
confidence: high
---
# Java 네트워크 소켓

## 핵심 클래스 (Ch.5)
- `InetAddress` — IP 주소 표현 (p.190)
- `Socket` / `ServerSocket` — TCP (연결형). 서버: accept → 입출력 스트림; 클라이언트: 연결 (p.193-197) ^[raw/books/computer-network-programming.md]
- `DatagramPacket` / `DatagramSocket` — UDP 데이터그램 (p.217-219)
- `MulticastSocket` — 멀티캐스트 (p.223-225)
- `URL` / `URLConnection` — HTTP (p.227-230)

## 주요 예제
- 자바 채팅 서버·클라이언트 (Ch.5.2-5.3)
- 데이터그램 에코 (Ch.5.4)
- 자바 멀티캐스트 채팅 (Ch.5.5)

## 관련
- Java 기초: class/객체/인터페이스/스레드 (Ch.4, p.145-176) ^[raw/books/computer-network-programming.md]
- 분산: RMI (스텁·스켈톤), 코바 [CORBA] (Ch.7)
- 3-tier C/S 모델 + JDBC (Ch.6)

## Related
- [[socket-programming-patterns]]
- [[computer-network-programming-book]]
- [[jdbc]]