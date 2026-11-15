---
title: 금융 전문가를 위한 머신러닝 알고리즘
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, machine-learning, nlp]
sources: [raw/books/ml-algorithms-for-finance-pros.md]
confidence: medium
---

# 금융 전문가를 위한 머신러닝 알고리즘

> 표지: '금융 전문가를 위한 파이썬으로 배우는 금융 머신러닝 알고리즘의 원리와 활용' (p1)

## 개요
- **저자:** 얀네스 클라스 지음, 박진수 옮김 (p3)
- **출판:** 위키북스, 초판 2021-02-07, 510쪽 (p3)
- **성격:** 파이썬 기반 머신러닝(선형/로지스틱 회귀, SVM, 랜덤 포레스트, 신경망, LSTM, NLP·텍스트 분석, 자기부호기) 원리부터 금융(주가 예측, 신용 평가, 리스크 관리) 적용까지 다루는 실전서 (p1, p3).

## 내용
- Attention 3D 블록 구현: 텐서 입력 `(batch_size, time_steps, input_dim)`에서 Permute→Reshape→Dense(softmax)→[평균 or 개별]→RepeatVector→Permute→Multiply 9단계로 주의 벡터를 생성·적용, '단어 벡터의 경우 각각 50개의 서로 다른 가중치를 계산한다. 입력 차원이 실제로 다른 것을 나타내는 시계열 모델로 작업하는 경우에 유용할 수 있다' (p261–262).
- 신경망 구조: 은닉 계층, 임베딩 계층, 자기부호기(AutoEncoder), 잠재 디리클레 할당(LDA) 등 금융 텍스트 분석에 활용되는 주요 아키텍처 (p223, p258, p295 색인).
- 시계열 모델: 자기회귀(AR), 자기회귀적 통합 이동평균(ARIMA), 이동평균(MA), 고차 이동평균(LMA), 이동분산(FGARCH) 등 금융 시계열 핵심 모델 다룸 (p157, p130 색인).
- 색인 확인: '은닉층', '정칙 드롭아웃', '정형/비정형', '이미지 증강', '자동 머신러닝', '모의탐색' 등 ML 개념 510쪽 전역에 걸쳐 정리 (p504–506).

## 관련 페이지
- [[python-finance-ai]] — 파이썬·케라스 금융 딥러닝
- [[deep-learning-tensorflow-keras]] — 케라스 신경망 실전
- [[finance-risk-ml-python]] — 파이썬 머신러닝 리스크
