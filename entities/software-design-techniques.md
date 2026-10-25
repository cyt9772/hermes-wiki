---
title: 소프트웨어 설계 테크닉 — 객체지향 아무도 가르쳐 주지 않았던 프로그래밍
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, uml-oo-modeling, object-oriented, software-quality, programming]
sources: [raw/books/software-design-techniques.md]
confidence: high
---

# 소프트웨어 설계 테크닉 — 객체지향 아무도 가르쳐 주지 않았던 프로그래밍 (한국어판)

Watanabe Kouzo(와타나베 코우조) 외 9명의 공동 저서, `Zero Kara Manabu · Software Sekkei / software design techniques`(Nikkei Business Publications, 2002)의 **한국어판**(`김성훈` 역, 성안당, 2004). 이 책은 구조화 분석(DFD)·ER 모델링을 시작으로 UML 다이어그램과 디자인 패턴(GoF)까지를 하나의 실용 실습서로 엮은, **현장 실무 중심**의 객체지향 설계 입문서다.

## 저자·서지
- 저자: Watanabe Kouzo 외 9명(와타나베 코우조 외 9인, Nikkei Business Publications 원저).
- 한국 번역: 김성훈 역, 성안당(cyber.co.kr), 2004. 원저 2002.
- UML의 "표준 3인"이 아니라, 실무 개발자(엔지니어)가 쓴 **현장 실무서**라는 점에서 이 클러스터의 다른 4권과 대비된다.

## 장별 개요 (원문 차 례 기준, 12장)
원문 목차 기준 총 12장(Intro + Part 1..7 + 장 1..12):
- **Intro**: `왜 분석/설계가 필요한가`, `소프트웨어 개발에 실패하다`, `라이프사이클`, `구조화 분석과 ER 모델링`.
- **Part 1~3 (구조화·ER 모델링)**: `1 구조화 분석의 기초`, `2 ER 모델링으로 설계하자`, `3 개발에 성공한 분석/설계의 실제`.
- **Part 1~3 (UML 맛보기)**: `UML 맛보기`, `다이어그램을 알면 UML이 보인다`, `시스템 개발 과정 속의 UML`.
- **장 3~6 (프로그램 설계)**: `알기 쉬운 프로그램 설계하기(로봇)`, `리팩토링으로 프로그램을 생생하게`, `꼼꼼한 설계의 지름길: 디자인 패턴`, `대화형 웹 애플리케이션에 Observer/Command`.
- **장 7~12 (객체지향 주무르기)**: `객체지향에 관한 다섯 가지 의문`, `객체지향 기술의 기본 틀(캡슐화/상속/폴리모피즘)`, `OOP 함정(자식-부모, 상속 혼동)`, `UML 정적/동적 분석`, `유지보수하고 재이용하기 쉬운 객체지향 설계 요령`.
- **부록**: `IBM Rational Rose XDE` 활용.

## 핵심 컨셉
- **Watanabe의 객체지향 설계 원칙 5가지(5 요령)**:
  1. 역할분담을 확실히 한다 (`책임 = 1개, 분할`).
  2. 이름은 본질을 나타내도록.
  3. 작은 것이 좋은 것이다 (방법 20-30행 상한).
  4. 숨기는 것이 많을수록 좋다 (정보 은폐, `private/protected`).
  5. 타인과 관계되는 일을 줄인다 (인수·반환값 최소, 의존도 최소). — `유지보수·재이용성 높은 설계`라는 주제 아래 정리 (p. 361-366).
- **GoF 디자인 패턴 (5형제/칠형제)**: `Factory Method / Abstract Factory / Singleton / Composite / Adapter / Observer / Command` 7개를 "꼭 알아 둘 디자인 패턴 칠형제"로 다룸 (장 4, p. 184-214).
- **UML 다이어그램 8종**: 클래스, 객체, 유스케이스, 시퀀스, 협업, 상태차트, 활동, 배포 — UML을 **커뮤니케이션 수단**으로 제시.
- **현장주의(현장에서의 분석/설계)**: "책상(Desk)에서만 하는 분석/설계"를 `탁상주의`의 폐해로 비판하고, 사용자·설계자가 함께 현장(현장/전자칠판)에서 설계하는 `현장주의`를 권함.

## Related
- 저자: [[watanabe-kouzo]]
- 클러스터: [[uml-oo-design-cluster]] / [[object-oriented-design-patterns]]
- 기존 관련: [[software-configuration-management]] (개발 프로세스와 접점)
