---
title: 한글 코드 시스템 프로그래밍 가이드 (Hangul Code System Programming Guide)
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, hangul, coding, unicode]
sources: [raw/books/hangul-code-system.md]
confidence: medium
---

# 한글 코드 시스템 프로그래밍 가이드 (Hangul Code System Programming Guide)

> 표지·머리말: "유닉스와 PC 환경에서 동시에 사용할 수 있도록 범용 프로그램(General Program) 방법을 제시하여 다양한 환경에서 효율적으로 프로그램을 개발할 수 있도록 설명" (p4)

## 개요
- **Author:** 한국어정보처리연구소
- **Pages:** 517
- **Positioning:** "c로 구현한 한글 코드 시스템 프로그래밍" (p1). 완성형·조합형·유니코드의 원리와 한글 코드 변환 프로그램(Full Source Code 제공) 개발, 유닉스·PC 양쪽 환경의 범용 개발까지 다룬다.

## 내용
- 1바이트 체계의 한계: "현대 한글은 11,172 자이므로 256 자까지만 표현할 수 있는 1바이트 체계로는 현대 한글을 전혀 표현할 수 없었다" 그래서 각양 한글 코드가 생겨났다는 서술 (p14).
- 분류 기준: "가장 중요한 기준은 한글 1음절을 표현하는데 조합 원리를 사용하는가, 필요한 바이트 수는 얼마인가, 8번째 비트를 사용하는가 등이다" (p14).
- N바이트 코드: "한글 한 음절을 표현하기 위해 글자별로 2 바이트부터 5 바이트까지를 사용한다 / 이런 이유로 멀티바이트(multi-byte) 코드라고도 부른다" (p15).
- 코드 체계 개요: 완성형·조합형·유니코드(2.x)의 기본 원리, 코드 변환 프로그램 개발, 부록의 코드표를 함께 제공한다 (p4).

## 관련 페이지
- [[c-hardware]] — C로 직접 하드웨어/시스템을 다루는 저수준 프로그래밍 계열
- [[embedded-c-optimization]] — C 기반 저수준/임베디드 개발 맥락
- [[coding-test]] — 알고리즘·자료구조 풀이 등 프로그래밍 실전 기술서
