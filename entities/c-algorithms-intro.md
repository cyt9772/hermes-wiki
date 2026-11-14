---
title: C로 배우는 알고리즘 입문
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, algorithms, c-language, beginner]
sources: [raw/books/c-algorithms-intro.md]
confidence: medium
---

# C로 배우는 알고리즘 입문

> 프로그래머의 창조적인 생각과 지속적인 흥미를 불러일으키는 원동력은 알고리즘이다 (p5)

## 개요
- **저자/역자/출판:** 카사이 아사오 (Asao Kasai) 저, 진명조 역, 한빛미디어 | 2004 | 486쪽
- **포지셔닝:** 일본 원서(Gijutsu-Hyoron) 한국어판. '명쾌한 개념 + 실습 예제 + 응용 연습 예제'의 계단식 학습법과 사전식 구성, 윈도우·리눅스 컴파일러에서 테스트한 완전 소스를 강점으로 제시 (p1).
- **대상:** 언어의 기본 문법을 익히고 본격 개발을 앞두고 있는 입문자 ~ 현업 숙련 개발자까지 (p5).

## 내용
- 워밍업 실습: 호너법(Horner)으로 다항식 f(x)=5x⁴+4x³+3x²+2x+1 값을 n번 곱셈·n번 덧셈으로 계산 — 점화식 f₀=a₄, f₁=f₀·x+a₃ … 로 표현 (p20).
- 학습 방법: 개념 설명 → C 소스 실습 → 응용 예제로 단계적으로 확장하는 계단식 구조. 각 예제에 주석과 완전 소스가 따라붙음 (p1, 5).
- 알고리즘의 역할: '어떻게 하면 이런 기능을 구현할 수 있을까', '더 효율적인 프로그램을 만들 수는 없지' 하는 질문을 해결하는 도구로 알고리즘을 포지셔닝 (p5).

## 관련 페이지
- [[first-algorithms-datastructures]] — 같은 주제의 입문서(파이썬). 같은 알고리즘을 다른 언어로 비교
- [[algorithm-problem-solving-theory]] — C 언어로 BOJ 문제를 풀 실전 단계로 확장
- [[good-programming-principles-25]] — C 소스 작성 시 코드 가독성·구조화 원칙 적용
