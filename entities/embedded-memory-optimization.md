---
title: 임베디드 메모리 최적화기법 (Code Optimization: Effective Memory Usage)
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, embedded, memory, c]
sources: [raw/books/embedded-memory-optimization.md]
confidence: medium
---

# 임베디드 메모리 최적화기법 (Code Optimization: Effective Memory Usage)

> 최적화의 개요: "코드의 최적화를 시작하기 전에, 같은 코드에 대해 신뢰성이 높되 최적화되지 않은 버전을 작성하라" — 최적화 7규칙 제1규칙 (p3)

## 개요
- **Author:** Kris Kaspersky 저, 여인춘 역
- **Publisher:** 에이콘출판 (Acorn) — 임베디드 시스템 프로그래밍 시리즈 No.10
- **Pages:** 399
- **Positioning:** "CODE OPTIMIZATION: EFFECTIVE MEMORY USAGE" (p4). 기계 코드·자료 구조 수준에서 프로파일링(VTune)과 x86(Pentium) 기계코드 최적화에 초점을 둔 실무서.

## 내용
- 최적화 7규칙 제1규칙: "코드의 최적화를 시작하기 전에, 같은 코드에 대해 신뢰성이 높되 최적화되지 않은 버전을 작성하라 / 이것은 여러분이 코드의 최적화를 시작하기 전에 프로그램이 올바로 작동하는지 확인하기 위함이다" (p3).
- 제2규칙(알고리즘이 우선): "퀵 정렬과 이진 검색을 구현할 경우 비록 소스 코드를 서툴게 구현했다 하더라도 속도가 최소 10배 이상 증가할 것이다" (p3).
- 잘못된 통념: "컴파일러의 전지전능한 힘에 대한 믿음은 아무런 근거도 없다 / 훌륭한 최적화 컴파일러 조차도 아주 잘 설계된 코드만을 효율적으로 해석할 수 있다" (p6).
- 프로파일링·기계코드 최적화: "arithmetic command가 골고루 분산되었고 레지스터 read/write command가 중간중간 끼어들어 나간다 / Pentium 프로세서들은 단 하나의 ALU만을 갖기 때문에 이러한 구성은 성능을 거의 2배로 증가시킨다" (p70).

## 관련 페이지
- [[embedded-linux-primer]] — 임베디드 Linux 프로그래밍 기초 계열
- [[embedded-systems-firmware]] — 임베디드 시스템 펌웨어·하드웨어 계층 최적화
- [[gnu-linux-rapid-embedded]] — 임베디드 Linux 실시간 개발 계열
