---
title: Enterprise Programming with Java
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, programming, java, jdbc, rmi]
sources: [raw/books/enterprise-programming-java.md]
confidence: medium
---
# Enterprise Programming with Java

> 동일한 JDBC API 프로그램이 각 DBMS에 알맞게 접근하도록 이어주는 인터페이스 역할을 하는 프로그램이 바로 JDBC 드라이버이다 (p28)
## 개요
- **발행:** 삼성SDS·멀티캠퍼스 (교육용)
- **쪽수:** 290p (텍스트 레이어 추출, 로컬 PDF `/run/media/yutae/Data/Enterprise Programming with Java.pdf`)
- **위치화:** JDK 1.1→1.2 업그레이드, Enterprise Application 모델, JDBC, 네트워크·RMI 프로그래밍, 객체 직렬화 등 자바 엔터프라이즈 개발의 핵심 축을 다루는 실무서 (목차 p4).
## 내용
- 장 구성: I장 JDK 1.1→1.2 Upgrade, II장 JDBC 프로그래밍(java.sql 패키지, 데이터베이스 접근 모델), III장 Network 프로그래밍(소켓, URL, 한글/다국어, RMI, 객체 직렬화, CallBack) (p4).
- JDBC 아키텍처: 'JDBC 프로그램은 JDBC 드라이버 매니저를 통해서 특정 데이터베이스를 직접 접근하고 처리하는 JDBC 드라이버를 먼저 선택한다' (p28).
- 4종 드라이버: 'JDBC 드라이버는 역할에 따라 크게 네가지 종류로 구분된다' — 첫 번째는 'JDBC-ODBC 브리지… 전자 서명이 안 된 Java 애플릿은 보안상 문제를 위해 이 드라이버를 사용할 수 없다' (p30).
## 관련 페이지
- [[unix-network-programming-ste]] — 네트워크 프로그래밍 계열
- [[windows-sockets-network-programming]] — Windows 소켓·멀티스레드 계열
- [[beginning-linux-programming]] — 리눅스 C/시스템 프로그래밍 계열
