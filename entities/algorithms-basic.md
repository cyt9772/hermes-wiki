---
title: 알고리즘 기초 (Foundations of Algorithms, 5th ed.)
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, algorithms, data-structures, complexity-analysis]
sources: [raw/books/algorithms-basic.md]
confidence: medium
---

# 알고리즘 기초 (Foundations of Algorithms, 5th ed.)

> 이 책은 알고리즘의 설계, 알고리즘의 복잡도 분석, 계산복잡도 (문제의 분석)에 대하여 다룬다. (p4)

## 개요
- **저자/원서:** Foundations of Algorithms, Fifth Edition (Jones and Bartlett) — 홍릉과학출판사 한국어 번역
- **분량:** 636쪽 | **방법:** OCR (영문·숫자 아티팩트 존재)
- **포지셔닝:** 학부 고학년·대학원 수준. 미적분 대신 이산구조+대수학 기초만 있으면 이해 가능하도록, 수학적 개념을 자연어로 설명하는 방향 (p4-5). 의사코드 기반 (특정 언어에 종속되지 않음, p4).

## 내용
- 구성: '응용분야별보다는 문제를 해결하는데 사용한 기술별로' 조직 — 분할정복(2장)·동적계획(3장)·탐욕(4장)·되추적·분기한정(5·6장) (p5-6).
- 계산복잡도: 7장 정렬문제(합병/퀵/힙정렬, 결정트리 하한), 8장 검색(보간검색, B-트리, 선택문제)을 분석으로 다룬다 (p6, 12).
- 9장 NP 이론: 다항시간 알고리즘을 찾은 문제·다루기 힘들다고 증명된 문제·아직 증명되지 않은 3분류, NP-완전/NP-Hard 집합 (p6, 13).
- 10장 유전 알고리즘과 유전 프로그래밍을 부록 수준이 아닌 본문 장으로 포함 (p5, 13).
- 의사코드 표기: 지역배열 길이를 'SS[2..n]'처럼 0++ 스타일보다 유연하게 표현, 'exchange x and y;' 같은 수학적 단축 표현도 사용 (p20-21).

## 관련 페이지
- [[intro-algorithms-korean]] — CLRS 3판 국역; 동종 대학원 교과서와 비교하여 읽기 좋은 교차 교재
- [[good-programming-principles-25]] — 알고리즘 설계와 프로그래밍 원칙을 서로 연결
- [[computer-algorithms]] — Horowitz/Sahni; 비슷한 수준(대학원)의 영어 원서
