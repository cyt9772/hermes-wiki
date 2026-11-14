---
title: QT5 프로그래밍 가이드
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, programming, qt, c++]
sources: [raw/books/qt5-programming-guide.md]
confidence: medium
---
# QT5 프로그래밍 가이드

> Qt는 Embedded Linux, Mac OS X, Windows, Linux, Android, QNX, MeeGo, WebOS, Symbian 등 다양한 플랫폼을 지원하는 크로스 플랫폼 프레임워크입니다 (p4)
## 개요
- **저자:** 김대진
- **쪽수:** 623p (텍스트 레이어 추출, 로컬 PDF `/run/media/yutae/Data/QT5 프로그래밍 가이드.pdf`)
- **위치화:** '예제 중심의 애플리케이션 개발을 위한 프로그래밍 가이드'. C++ 외 파이썬·루비 지원, 전 세계 약 50만 명 이상 사용 (p1, p4).
## 내용
- 크로스 플랫폼: 'Embedded Linux에서 개발한 애플리케이션 소스 코드를 Windows, Android, QNX와 같은 다양한 플랫폼에서… 소스 코드 변경 없이 그대로 사용할 수 있다' (p4).
- 시그널·슬롯: 'slider 인스턴스의 값이 변경될 때 valueChanged() 시그널 함수 이벤트가 발생한다. 시그널을 발생하면 이미지의 확대 축소 기능을 처리하는 setZoom() 슬롯함수가 이벤트를 처리한다' (p100).
- QPainter: 'QPainter 클래스의 재정의 함수인 paintEvent() 함수가 실행된다' — `scale()`로 비율을, `drawPixmap()`로 이미지를 렌더링 (p101).
## 관련 페이지
- [[embedded-linux-primer]] — 임베디드 리눅스 개발 계열
- [[gnu-linux-rapid-embedded]] — 임베디드 리눅스 개발 계열
- [[embedded-systems-firmware]] — 임베디드 시스템·펌웨어 계열
