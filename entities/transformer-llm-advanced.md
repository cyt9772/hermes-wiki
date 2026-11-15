---
title: Transformer와 LLM 심화
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, deep-learning, transformer]
sources: [raw/books/transformer-llm-advanced.md]
confidence: medium
---

# Transformer와 LLM 심화

> 표지: '실무역량 (제1.2판) / (주)한국에이아이연구소 대표이사 홍근선 저' (p2, p3)

## 개요
- **저자:** 홍근선 ((주)한국에이아이연구소 대표이사, 전자공학 박사수료, 남서울대학교 전산과 교수) (p3)
- **성격:** 실무역량 교육 교재. Transformer와 LLM의 원리를 Keras와 PyTorch 두 프레임워크로 Model 설계하는 심화 과정 (p4). PDF 248쪽.

## 내용
- 구조(차례, p4): 1부 Deep Learning 기본 정리(1.1 DL 개요 p9, 1.2 Keras Model 설계 workflow p30, 1.3 PyTorch Model 설계 workflow p55) → 2부 Attention Mechanism(2.1 Word Embedding p77, 2.2 Attention Mechanism, 2.3 Self-Attention) → 이후 LLM 심화.
- 어텐션 메커니즘을 직접 코드로 전개: '2부. Attention Mechanism — 2.1 Word Embedding / 2.2 Attention Mechanism / 2.3 Self-Attention' 순서로 심화 (p72~73).
- LLM 시대가 온 배경으로서 Gated(게이트) 구조 모델까지 다루며, 'Gated 모델 저자는 encoder expert가 특정 토큰이나 얕은 개념에 특화됨을 관찰'한 사례를 제시 (p162 부근).
- Keras와 PyTorch의 Model 설계 workflow를 병행 비교하는 실습 구성 (p4).

## 관련 페이지
- [[deep-learning-homemade]] — 트랜스포머·BERT 관련 모델을 직접 구현하는 실전서
- [[deep-learning-tensorflow-keras]] — Keras 기반 딥러닝 기초
- [[keras-dl-understanding-impl]] — Keras 모델 설계·RNN/CNN 실습 계열
- [[deep-learning-timeseries]] — 시계열 예측 딥러닝 계열
