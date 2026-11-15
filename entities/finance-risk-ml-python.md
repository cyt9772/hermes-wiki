---
title: 파이썬 머신러닝을 이용한 금융 리스크 관리
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, risk, machine-learning]
sources: [raw/books/finance-risk-ml-python.md]
confidence: medium
---

# 파이썬 머신러닝을 이용한 금융 리스크 관리

> 표지: 'Machine Learning for Financial Risk Management with Python' (p1)

## 개요
- **저자:** 압둘라 카라산 지음, 이병욱 옮김 (p1, p4)
- **출판:** O'Reilly Media 원서, 에이콘출판(주) 2023 한국어판, 387쪽 (p4)
- **성격:** 파이썬(Numpy, Scipy, hmmlearn)으로 신용 리스크(신용등급·PD·LGD), 시장 리스크(Sharpe, Fama-Factor), 시계열 리스크(GARCH, HMM)에 머신러닝(K-평균 군집, 은닉 마르코프 모델)을 적용하는 실무서 (p1, p4).

## 내용
- K-평균 군집 알고리듬: '1. 중심이 될 k개의 임의의 점을 선택한다. 2. 선택한 거리 측정법을 기준으로 쿤태치와 k개의 중심 사이의 거리를 계산한다. 이러한 거리에 기반하여 각 관측치를 가장 가까운 클러스터에 할당한다. 3. 할당을 기반으로 클러스터 센터를 갱신한다. 4. 중심이 변경되지 않을 때까지 2단계부터 절차를 반복한다' (p208).
- 클러스터 수 결정: '관성은 가장 가까운 중심까지의 거리 제곱의 합으로 계산된다' — 엘보우법, 실루엣 점수('값 1은 관측치가 정확한 중심에 가깝고 올바르게 분류됐음을 나타낸다. 그러나 -1은 관측치가 올바르게 군집화되지 않았음을 나타난다'), 칼린스키-하라바츠(CH) 지표, 갭 분석 등 4가지 방법 (p208–209).
- 시장 리스크 OLS: Fama-French 3인자(Mkt-RF, SMB, HML) 회귀 결과 'R², Jarque-Bera(IB)=80241.345, Skew=0.433, Kurtosis=22.955, Durbin-Watson=2.717' — 다인자 모델 수익률 예측 (p378).
- HMM 은닉 마르코프 모델: '가우스 HMM이 더 나은 위험 조정 수익률을 제공해 다른 분석 중에서 포트폴리오 할당에 유용함을 시사한다' — S&P 지수 수익률 3컴포넌트 분류(고변동성·중간·저변동성) (p379).

## 관련 페이지
- [[python-for-finance]] — 파이썬 금융분석 기초
- [[finance-python-cookbook]] — 파이썬 금융·리스크
- [[wise-quant-investing]] — 퀀트 투자·포트폴리오 리스크
