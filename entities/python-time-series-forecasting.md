---
title: 파이썬 시계열 예측 분석
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, time-series, forecasting, python, deep-learning]
sources: [raw/books/python-time-series-forecasting.md]
confidence: medium
---

# 파이썬 시계열 예측 분석

> 통계 모델, 딥러닝, 파이썬 라이브러리를 활용한 대규모 시계열 데이터 분석 (p1)

## 개요
- **저자:** 마르쿠 페이셰이루 (Marcos Falcão) 지음, 동동구 옮김 (p1)
- **출판:** 제이펍 (J-Pub Co. Ltd.), 1판 1쇄 2024-07-25; 원서 Time Series Forecasting in Python (Manning, 2022), ISBN 979-11-93926-31-4 (p3)
- **성격:** 통계 모델(ARIMA계)에서 딥러닝(LSTM 등)까지 대규모 시계열 예측을 파이썬으로 다루는 실무서.

## 내용
- 책의 구성은 3부: Part 1·2 통계 모델기반 예측 — "시간은 그 누구도 기다려주지 않는다" (p8), Part 3 "딥러닝을 활용하여 대규모 예측하기" (p11).
- Part 2 통계 모델: ARIMA(p,d,q), SARIMA(p,d,q)(P,D,Q)m로 월간 항공 승객 수 예측, 외생 변수를 넣은 SARIMAX로 실질 GDP 예측, VAR·VARMA·그레인저 인과관계 테스트로 다중시계열 예측, 캡스톤 프로젝트(호주의 항당뇨제 처방 건수 예측) (p8~p11).
- Part 3 딥러닝: 시계열 예측에 딥러닝이 필요한 경우, 데이터 윈도우(DataWindow 클래스)·베이스라인 모델, 선형/심층 신경망, "LSTM으로 과거 기억하기" (RNN·LSTM 아키텍처) (p10~p11).
- 출판사 면책: "이 책에 기재된 내용을 기반으로 한 운용 결과에 대해 지은이/옮긴이·제이펍 출판사는 일체의 책임을 지지 않음" (p5).

## 관련 페이지
- [[deep-learning-timeseries]] — 시계열 딥러닝(인간 학습 기반) 책
- [[finance-python-cookbook]] — 파이썬 금융 모델링
- [[quant-investing-python]] — 금융 데이터 분석과 퀀트 전략 검증
