---
title: 컴퓨터 네트워크 프로그래밍 (컴퓨터 네트워크 프로그래밍, 김화종)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, sockets, network-programming]
sources: [raw/books/computer-network-programming.md]
confidence: high
---
# 컴퓨터 네트워크 프로그래밍

김화종 저 (강원대학교 정보통신연구소). **SOCKET 기반 C/Unix 네트워크 프로그래밍 + Java 소켓 실전.** "이 책에서는 TCP/IP 계층의 응용 프로그램 개발에 필수적인 소켓(socket)을 중심으로 한 클라이언트–서버 통신 기술을 다룬다" — 머리말 (pg3). 예제 소스: telecom.kangwon.ac.kr/net_prog

## 인용 (pg3, 머리말)
> "최근 인터넷 서비스를 중심으로 정보통신 서비스가 급격히 증가하고 있으며 이것의 앞으로 어떤 형태로 발전될지는 예측하기가 어려울 정도이다."

## 구성 (7장 + 부록, pg5-10 차례 확인)
| # | 내용 |
|---|------|
| 1 | **네트워크 프로그래밍의 이해** (p.1) — 분류(디바이스드라이버/트랜스포트/응용) (p.4-5), TCP/IP(액세스/인터넷/트랜스포트/네임서비스) (p.6-28), 클라이언트-서버 모델 (p.28), 프로그래밍 환경(Unix/Win/Java) (p.32) |
| 2 | **유닉스 소켓 시스템 콜** (p.41) — 소켓 정의·번호·개설·구조체 (p.43-52), 바이트 순서·IP 주소변환 (p.54-57), **연결형/비연결형 클라이언트** daytime·echo (p.63-76), **연결형 서버** echo (p.78-84), signal()·fork() (p.86-90), 토크 프로그램 (p.90+) |
| 3 | **소켓 응용 프로그래밍** (p.101) — 동작 모드 (p.103), **채팅 서버 (select())** (p.105), 채팅 클라이언트 (p.116), SO_REUSEADDR (p.120-122), **멀티캐스트** (p.123-127), 데몬/inetd 서버 (p.131-135), WinSock (p.141) |
| 4 | **자바의 이해** (p.145) — 기초 문법·타입 (p.147), class/interface/overloading (p.154-161), 예외 (p.163), 스레드 (p.167), AWT (p.172), 스트림 (p.176) |
| 5 | **자바 네트워크 프로그래밍** (p.185) — InetAddress/Socket/ServerSocket (p.189-197), **자바 채팅 서버** (p.200), **채팅 클라이언트** (p.209), **DatagramPacket·DatagramSocket** 에코 (p.217-219), **자바 멀티캐스트 채팅** (p.223-225), URL/URLConnection (p.227-230) |
| 6 | **네트워크 데이터베이스 프로그래밍** (p.235) — 테이블·SQL (p.237), **JDBC** 절차·응용 (p.240-254), **3-tier C/S 모델** (p.261) |
| 7 | **분산 네트워크 프로그래밍** (p.265) — 분산 객체 모델 (p.267), **RMI** (스텁·스켈톤, p.271-275) + daytime·채팅 예제 (p.277-280), **코바 (CORBA)** (p.294) |
| 부록 | A. UNIX 소켓 시스템 콜 요약 (p.305) · B. 문법 (p.307) · C. 에러 코드 (p.309) |

## Related
- [[socket-programming-patterns]] (concept)
- [[java-sockets]] (concept)
- [[kim-hwa-jong]] (author)
- [[tcpip-complete]] (이론)
- [[winsock-bsd-compare]]
- [[jdbc]]
