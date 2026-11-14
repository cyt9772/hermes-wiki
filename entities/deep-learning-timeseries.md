---
title: 딥러닝으로 걷는 시계열 예측
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, deep-learning, time-series, rnn, python]
sources: [raw/books/deep-learning-timeseries.md]
confidence: medium
---

# 딥러닝으로 걷는 시계열 예측

> 가장 기본적인 RNN이니까 코딩을 하면서 이해해보도록 하겠습니다 (p175)

## 개요
- **저자:** 본문에서 미확인 (스캔 OCR 텍스트, 표지·목차 영역 아티팩트 심함)
- **쪽수:** 350쪽 | **성격:** 파이썬 기반 시계열 예측 딥러닝 실습서 — RNN·LSTM 중심, 금융(KOSPI) 데이터 예제
- **방법:** tesseract 5.5.3 (kor+eng, 300dpi) OCR

## 내용
- 시계열 예측의 기본 흐름: 과거 N개 값에 기반해 다음값을 예측하며, 노드 간 가중치 전달·연산으로 다음 값(예: 5→6)을 도출 (p175).
- SimpleRNN 구현: `numpy`로 (3,5) 입력 / (3,) 출력 데이터 구성 — 입력 1~5 → 6, 2~6 → 7, 3~7 → 8 대응 (p175).
- `x_train`과 `y_train`의 크기를 맞추기 위한 시퀀스 슬라이싱 기법 (p175).
- 실전 예제: KOSPI 200 지수(`kospi200`)에 `split_xy(..., 5, 1)`로 입력·출력 분할, `sklearn.model_selection.train_test_split(random_state=2, test_size=0.3)`로 학습/테셋 분리 (p340).

## 관련 페이지
- [[ai-ml-dl-intro]] — 딥러닝 개념 입문 계열
- [[tensorflow-explained]] — 파이썬 딥러닝 도구서 계열
- [[business-statistics-python]] — 파이썬 데이터 분석 계열
