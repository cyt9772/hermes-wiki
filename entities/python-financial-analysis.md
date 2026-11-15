---
title: 파이썬으로 배우는 금융분석
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, time-series, statistics]
sources: [raw/books/python-financial-analysis.md]
confidence: medium
---

# 파이썬으로 배우는 금융분석

> 표지: '금융의 기초 개념부터 해석까지, 문제를 통한 계산 활용까지' (p1)

## 개요
- **저자:** 본문 확인 불가 (OCR 아티팩트. 저작권 페이지에 Packt Publishing 2017 원서 'Python for Finance - Second Edition (9781787125698)' 한국어판으로 명시, p3)
- **출판:** 에이콘출판(주), 2018 ©, 735쪽 (p3)
- **성격:** 파이썬 기반 금융 기초 개념·통계·시계열 분석·옵션·GARCH 등 금융 데이터 분석을 문제 중심 예제로 풀어가는 Packt 한국어 번역서 (p1, p3).

## 내용
- S&P500 일 수익률 통계량(평균·표준편차·왜도·첨도) 계산 결과 'S&P500 skewness = -0.64035588, kurtosis = 20.81432822'로 '음의 왜도, 두터운 꼬리'를 확인하며, Cook Pine Capital의 '두터운 꼬리 리스크(2008)' 논문과 비교 (p367).
- t-검정: '금융에 있어 t-검정은 가장 많이 사용되는 통계적 가설 검정 방법 중 하나인데, 귀무가설이 맞을 경우 검정 통계치가 스튜던트 t 분포를 따른다' — 2013년 IBM 일별 수익률 평균이 0인지 검증 예제 (p368).
- 바틀렛(Bartlett) 등분산 검정: 'sp.stats.bartlett() 함수가 "모든 입력 샘플은 동일 분산을 가진 모집단들로 부터 추출됐다"라는 귀무가설을 통해 등분산에 대한 바틀렛 검증을 수행한다' (p368).
- 색인 확인: GARCH 모델, Monte Carlo 시뮬레이션, KMV 모델, Loss Given Default, Jarque-Bera normality test, Kolmogorov-Smirnov test 등 옵션·리스크·시계열 핵심 개념이 전체 735쪽에서 반복 다룸 (p727–728).

## 관련 페이지
- [[finance-recipes]] — 파이썬 금융공학 레시피(동일 Packt 계열)
- [[python-for-finance]] — 파이썬을 활용한 금융분석(동일 원서 계열)
- [[business-statistics-python]] — 파이썬 통계 분석 기초
