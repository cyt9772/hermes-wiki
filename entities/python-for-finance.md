---
title: 파이썬을 활용한 금융분석 (Python for Finance, 2nd Edition)
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, quant, derivatives]
sources: [raw/books/python-for-finance.md]
confidence: medium
---

# 파이썬을 활용한 금융분석 (Python for Finance, 2nd Edition)

> 표지: '파이썬의 기초부터 금융공학적·머신러닝, 퀀트분석, 매매 시스템 구현까지' (p1)

## 개요
- **저자:** 이브 힐피시 (Yves Hilpisch), 옮긴이 김도형 (p2, p4)
- **출판:** 한빛미디어 (주), 초판 2016·2판 2022-03-30, 788쪽 (p3)
- **성격:** 파이썬 기반 금융공학·퀀트분석 종합 실전서. 금융 기초·통계·데이터 분석에서 옵션 가격 계산, 알고리즘 트레이딩, 머신러닝까지 파이썬 생태계(Numpy, Pandas, Scipy, Matplotlib, CVXPY 등)를 다룸 (p1, p2).

## 내용
- 2판에서는 금융 데이터 과학, 알고리즘 트레이딩, 금융공학 장을 대폭 추가·개편했으며, '초판의 몇몇 장은 완전히 삭제'하고 '특히 초판에서 가장 중요하다고 생각했던 주제에 집중' (p4–p5 서문).
- spline(스플라인) 보간법 적용 시 '데이터가 정렬되어 있어야 하고 잡음이 없어야 하며 다차원 문제에는 적용할 수 없다. 또한 계산량이 더 많기 때문에 어떤 경우에는 회귀법보다 훨씬 계산 시간이 오래 걸릴 수 있다' (p399).
- 11.2 최적화: '금융이나 경제 분야에서는 최적화가 중요한 역할을 한다. 예를 들면 옵션 가격 계산을 위해 시장 데이터를 기반으로 인수 교정(calibration)을 하거나 대리인의 효용 함수를 최적화하는 경우 등이다' (p400).
- 부록 B 유러피안 콜 옵션: 가격 곡면과 베가(Vega) 곡면을 3D 표면 플롯으로 시각화하며, strike/maturity 축에 대한 민감도 변화를 보여주어 옵션 그릭 계산·시각화 기법을 정리 (p781–782).

## 관련 페이지
- [[finance-recipes]] — 파이썬 금융공학 레시피(동일 주제 계열)
- [[deep-learning-tensorflow-keras]] — 머신러닝/딥러닝 기반 금융 모델링
- [[business-statistics-python]] — 파이썬 기반 통계·비즈니스 분석
