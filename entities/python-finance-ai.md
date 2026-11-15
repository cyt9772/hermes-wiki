---
title: 파이썬 기반 금융 인공지능 (Artificial Intelligence in Finance)
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, deep-learning, trading]
sources: [raw/books/python-finance-ai.md]
confidence: medium
---

# 파이썬 기반 금융 인공지능 (Artificial Intelligence in Finance)

> 표지: '파이썬과 케라스를 활용한 금융 시계열 데이터 기반 알고리즘 트레이딩 전략' (p1)

## 개요
- **저자:** 이브 힐피시 (Yves Hilpisch), 옮긴이 김도형 (p1, p3)
- **출판:** 한빛미디어(주), 초판 2022-09-30, 513쪽 (p3)
- **성격:** 파이썬·케라스(TensorFlow)로 금융 시계열 데이터에 밀집 신경망, LSTM, 합성곱 신경망(CNN)을 적용해 알고리즘 트레이딩 전략을 구성하는 실전서 (p1, p3).

## 내용
- 신경망 도입 목적: '이 장과 3부 전체의 주목표는 금융 시장에 신경망을 적용함으로써 통계적 비효율성을 발견하는 것이다. 이 장에서 제시된 수치적인 결과는 예측 정확도의 경우, 특정 사례에서 60% 예측 정확도를 보여줌으로써 어느 정도 희망이 있다는 것을 보장한다' (p255).
- 데이터: 'EUR/USD 환율의 일중 가격 시계열에 대한 통계적 비효율성의 힌트를 발견했다. 이 장과 다음 장에서는 환율 자산 클래스, 특히 EUR/USD 환율에 초점을 맞춘다. 여러 가지 이유로 환율의 통계적 비효율성을 경제적으로 이용하는 것은 VIX 변동성 지수와 같은 변동성 상품 등의 다른 자산 클래스를 이용하는 것보다 복잡하지 않다' — Refinitiv Eikon 데이터 API에서 시가·고가·저가·종가 활용 (p255–256).
- 합성곱 신경망 구현: '시계열 데이터에 맞는 1차원 합성곱층'을 핵심으로 `Conv1D(filters=96, kernel_size=5, activation='relu')` → `Flatten` → `Dense(10)` → `Dense(1, sigmoid)` 구조로 35,157 파라미터 모델 훈련 예시 (p506).
- 학습 결과: 'val_loss 0.69~0.72, val_accuracy 약 0.50, loss 0.63, accuracy 0.59-0.60' — 60epochs, batch_size=48, validation_split=0.15 (p507).

## 관련 페이지
- [[python-for-finance]] — 파이썬 금융 기초·퀀트분석
- [[deep-learning-tensorflow-keras]] — 케라스/TensorFlow 신경망 실전
- [[finance-python-cookbook]] — 파이썬 금융·딥러닝 레시피
