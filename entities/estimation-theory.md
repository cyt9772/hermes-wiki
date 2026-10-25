---
title: Lessons in Estimation Theory for Signal Processing, Communications, and Control (3rd ed)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, estimation-filtering, stochastic-processes]
sources: [raw/books/estimation-theory.md]
confidence: high
---
# Lessons in Estimation Theory for Signal Processing, Communications, and Control (3rd ed)

> Jerry M. Mendel, Prentice Hall, 580p. 신호처리·통신·제어 3개 응용 공통의 **추정 이론**을 26개 레슨 체제로 묶은 대학원 교과서. "Lessons"라는 제목의 뜻: 각 레슨은 요약→전개→질문·문제로 자립 `[raw/books/estimation-theory.md]`.

## 개요
레슨 2(선형 모델)에서 출발, 최소제곱(배치·SVD·순환) → 추정량 성질(소표본/대표본) → 최대우도 → 가우시안·베이스 → **상태 추정(예측→필터링→스무딩)** → 비선형(Kalman-Bucy·EKF)까지 이어지는 단 하나의 추론 사슬을 그린다 `[raw/books/estimation-theory.md]`.

## 레슨 구조 (원문 TOC 기준, 26 레슨)
1. Introduction, Coverage, Philosophy, Computation (p.1)
2. **The Linear Model** (p.9) — 선형 모델, 컨볼루셔널 모델(반사 지진학) 부록
3. **Least-squares: Batch** (p.27) — 목적함수, 고정/확장 기억, 정규화 부록
4. **Least-squares: SVD** (p.44) — SVD로 eLS 계산, 의사역행 부록
5. **Least-squares: Recursive** (p.58) — RLS, inversion lemma
6. Small-sample Properties (p.74) — 무편향성·효율성
7. **Large-sample Properties** (p.91) — 확률 수렴, 비대차 무편향성·일관성, **비대차 정규성**, 비대차 효율성
8. Properties of LS Estimators (p.108)
9. **Best Linear Unbiased Estimation (BLUE)** (p.121) — BLUE vs WLS, 순환 BLUE, 랑그르 부록
10. **Likelihood** (p.137) — 우도비, 우도기대값
11. **Maximum-likelihood Estimation** (p.147) — MLE 성질, 선형 모델 MLE, 로그우도
12. **Multivariate Gaussian RV** (p.164) — 가우시안 밀도·성질, 조건밀도
13. **Mean-squared Estimation of Random Parameters** (p.173)
14. **Maximum a Posteriori (MAP) Estimation**
15. **Discrete-time Gauss-Markov Random Sequences** (p.211) — 성질, 상태변수 모델, SNR
16. **State Estimation: Prediction** (p.227) — 단단계/일반 상태 예측기, **혁신 프로세스**(p.233)
17. **State Estimation: Filtering (the Kalman Filter)** (p.242) — 유도(p.246), **MAP 기원 Kalman** 부록(p.253)
18. **State Estimation: Filtering Examples** (p.259) — 예제, Kalman 응용 부록
19. **Steady-state Kalman Filter** (p.279) — 단채널, **Wiener FIR 필터와의 관계**(p.286), Kalman vs Wiener, Levinson 부록
20. **State Estimation: Smoothing** (p.304) — 3종류 스무더, 단/이단계
21. **Smoothing (General Results)** (p.317) — 고정간격/고정점/고정lags, **최소분산 디콘볼류션(MVD)**, ML 디콘볼류션
22. State Estimation for the **Random-Variable Model** (p.345) — 편향, 상관 노이즈, 완전측정 low-order 추정기
23. **Linearization and Discretization of Nonlinear Systems** (p.364)
24. **Iterated LS and Extended Kalman Filtering** (p.384)
25. **Maximum Likelihood and Parameter Estimation** (p.397)
26. **Kalman-Bucy Filtering** (p.413) `[raw/books/estimation-theory.md]`

## 핵심
- **세 추정 축의 수학적 등가성**: 최소제곱(레슨 3~5) — BLUE(레슨 9) — MLE(레슨 11) — MAP(레슨 14) — Kalman(레슨 15~18, 26). "왜 이 셋이 같은 답을 주는가"가 책의 뼈대 — [[estimation-and-filtering]] 비교표의 이론 축 `[raw/books/estimation-theory.md]`
- **소표본(레슨 6·8) vs 대표본(레슨 7) 성질** 분리 — 무편향성·일관성·비대차정규성·비대차효율성 4성질을 MLE와 LS 각각에 매칭
- **상태 추정 3단계(예측→필터→스무딩)**가 독립 레슨(16/17-18/20). 레슨 19가 **Wiener FIR 필터와 Kalman의 관계**를 명시(비교 p.293) — Therrien [[discrete-random-signals]] 장 7과 같은 주제를 가우시안·상태공간에서 다름. Kalman-Bucy(레슨 26)·EKF(레슨 24)까지 연결
- 레슨 9 **BLUE**와 레슨 11 **선형모델 MLE**의 비교가 "공분산 미지(WSLS) vs 기지(ML)"의 공학 판단 기준 — [[linear-system-theory-design]] 옵티멀 추정·디콘볼류션 접점(레슨 21 **MVD**, p.329)

## Related
- 클러스터: [[stochastic-processes-cluster]] · [[estimation-and-filtering]]
- 인접: [[discrete-random-signals]] (Therrien, 이산 랜덤 프로세스 + 최적필터) · [[linear-system-theory-design]] (Chen, 상태공간 + 상태피드백/추정기)
- 개념: [[information-coding-theory]] (추정↔코딩 대칭) · [[cdma-dss-spread-spectrum]] (최적 수신기)
