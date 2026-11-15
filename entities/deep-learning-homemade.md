---
title: 혼자 만들면서 공부하는 딥러닝
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, deep-learning, keras, transformer]
sources: [raw/books/deep-learning-homemade.md]
confidence: medium
---

# 혼자 만들면서 공부하는 딥러닝

> 표지: '혼자서도 제대로 학습하고 싶을 때 / 다양한 딥러닝 모델을 구현해 보고 싶을 때' (p1)

## 개요
- **저자:** 박해선 지음 (p1)
- **출판:** 한빛미디어, 초판 2025년 5월 (p3) | **양:** PDF 446쪽
- **성격:** '혼자 만들면서 공부하는' 시리즈의 딥러닝 편. 이론만 읽고 끝내지 않고 실전 프로젝트를 직접 완성하는 데 초점을 두고, 이미지/텍스트 분류·요약, 전이학습, 트랜스포머까지 20개 딥러닝 모델을 구현한다 (p1, p3). '혼자 만들면서' 시리즈의 목표는 '배운 지식을 실전에 적용'하는 프로젝트 완성이며, 동영상 강의와 저자 Q&A를 지원하는 학습 사이트를 함께 운영한다 (p4).

## 내용
- 학습 경로가 LeNet-5 같은 역사적 합성곱 신경망(CNN) 모델에서 시작해, 곧바로 최신 모델로 넘어가지 않고 단계별로 확장된다 — '1장에서 살펴봤던 LeNet-5는 처음 합성곱 신경망을 소개한 역사적 모델이지만, 곧바로 이미…' (p81).
- 텍스트 처리 실습은 BERT 토크나이저 중심: 부분단어(wordpiece) 분해, `##` 접두사, `[CLS]` 특수 토큰을 다룬다 — 'pandemonium이 세 개의 부분단어로 나뉘어 있습니다. ##는 해당 토큰이 단어의 중간이나 끝에 들어가는 부분단어임을 나타냅니다. [CLS]는 텍스트 분류용 특수 토큰입니다' (p245).
- BERT 백본 모델에서는 `transformer_encoder()` 출력 중 첫 번째 토큰만 Dense() 클래스 층으로 전달하는 구성을 사용한다 (p245).
- 토큰↔ID 변환 API(`token_to_id()`, `id_to_token()`, `tokenize()`, `detokenize()`)를 실전 코드로 학습한다 (p245).

## 관련 페이지
- [[deep-learning-tensorflow-keras]] — Keras로 신경망을 구현하는 실습 기반 입문서
- [[deep-learning-timeseries]] — 딥러닝과 시계열을 접목하는 계열
- [[transformer-llm-advanced]] — 트랜스포머·어텐션 심화
- [[ml-dl-self-study]] — 같은 저자(박해선)의 1:1 과외식 ML/DL 자습서
