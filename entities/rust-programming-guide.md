---
title: 러스트 프로그래밍 공식 가이드 (The Rust Programming Language)
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, rust, programming-language, systems, safety]
sources: [raw/books/rust-programming-guide.md]
confidence: medium
---

# 러스트 프로그래밍 공식 가이드 (The Rust Programming Language)

> 전반적으로 러스트의 가장 큰 목표는 안전성과 생산성, 속도와 적합성을 제공함으로써 지난 수십 년간 개발자가 어쩔 수 없이 받아들였던 트레이드오프를 제거하는 것에 있다. (p18)

## 개요
- **저자/역자/출판:** 스티브 클라브닉(Steve Klabnik), 캐롤 니콜스(Carol Nichols) 지음, 장현희 옮김, 제이펍 | 2019 | 643쪽
- **원서:** The Rust Programming Language (No Starch Press, 2018). 오픈소스(https://github.com/rust-lang/book).
- **포지셔닝:** 러스트 커뮤니티에서 'the book'으로 불리는 공식 입문서. C 언어 기본 지식을 가정을 특정 언어 경험은 가정하지 않음.

## 내용
- 러스트의 목표: 안전성 · 생산성 · 속도 · 적합성을 모두 제공하여 개발자의 트레이드오프를 제거 (p18).
- 읽는 방법: 2·12·20장은 프로젝트 수행 장(코딩), 나머지는 개념 학습. '러스트를 학습하는 과정에서 가장 중요한 부분은 컴파일러가 표시하는 에러 메시지를 읽는 방법을 터득하는 것' (p18-20).
- 소유권(Ownership): 제4장에서 오너십 시스템을 본격적으로 학습. 베타리더는 '러스트는 다른 언어에서 찾기 어려운 소유권 개념 때문에 진입장벽이 높은데, 이 책은 그 부분 이해를 돕는다'고 언급 (p19, 21).
- 베타리더 평가: 'C는 빠르고 훌륭하지만 구현해야 할 부분이 너무 많으며, 최근 C++은 기능이 너무 많아져서 복잡. 러스트는 그 중간 어디쯤'이라는 평가 (p22, 네이버 이봉준).

## 관련 페이지
- [[good-programming-principles-25]] — 러스트의 소유권·타입시스템이 '안전하고 깔끔한 코드' 원칙을 언어 수준에서 보장하는 방식과 대응
- [[beginning-linux-programming]] — 시스템 프로그래밍 맥락에서 C 대신 러스트를 선택할 때 비교
- [[algorithm-problem-solving-theory]] — 알고리즘 문제를 C로 푸는 것과 대비: 소유권·형식시스템으로 메모리 오류를 컴파일 단계에서 제거
