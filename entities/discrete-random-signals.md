---
title: Discrete Random Signals and Statistical Signal Processing
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, stochastic-processes, estimation-filtering]
sources: [raw/books/discrete-random-signals.md]
confidence: high
---
# Discrete Random Signals and Statistical Signal Processing

> **Charles W. Therrien**, Naval Postgraduate School, Monterey, CA — Prentice Hall Signal Processing Series, 751p. 이산시간 랜덤 프로세스·통계적 신호처리 대학원 교과서 `[raw/books/discrete-random-signals.md]`.

## 저자 확인(wrapper "원저" 해소)
원문 txt 서지 표제("Tharles W. Therrien — aval Postgraduate School, onterey, CA")는 텍스트레이어 OCR 왜곡이며, 책 내부 참고문헌에서 동일 저자가 **"Charles W. Therrien, *Decision, Estimation, and Classification*"**으로 여러 번 실린다. 원저 = **Charles W. Therrien (Naval Postgraduate School, Monterey, CA)**, 출판사 **Prentice Hall** — 확인됨. 서문은 1987년 NPS "이산시간 랜덤 프로세스" 개설강의를 기반으로 하되, 책 출간 연도는 원문에 명시되어 있지 않아 기재하지 않음.

## 개요
"신호처리가 변했다. 더 이상 아날로그기기의 시대는 아니다. 우리는 확고하고, 장래 회복 불가능하게, 디지털(샘플링, 이산시간) 신호처리 영역에 있다" — 서문. 1987년 NPS에서 개설된 "이산시간 랜덤 프로세스" 강의에서 출발, 연속시간 랜덤 프로세스 과목의 **이산시간 대안**으로서 랜덤 프로세스를 순도 있는 이산 관점에서 소개 `[raw/books/discrete-random-signals.md]`.

## 장 구조 (원문 TOC 기준, 10장 + 부록)
1. **Introduction** (p.1) — 이산 랜덤 신호, 통계적 신호처리, 응용
2. **Random Vectors** (p.17) — 벡터 정의·특징, 기대·모멘트, **다변수 고스 밀도**(p.43), 선형변환, 역전, 상관행렬 대각화(유니터리, p.50), 삼각분해
3. **Random Processes** (p.85) — 랜덤 신호·시퀀스, 단순 디스크 프로세스, **마르코프 프로세스**(p.99), **마팅게일·절대적 공정 프로세스**(p.118), 주기·거의주기, **고스 프로세스**: CT/DT(p.124)
4. **Second-Moment Analysis** (p.140) — 상관·공분산 함수/행렬(p.141), 주파수역·변환역 표현(p.152), **이산 Karhunen-Loève 변환**(p.173), 샘플링 CT, **화이트 노이즈**(p.198), 고계 모먼트
5. **Linear Transformations** (p.223) — LSI 변환(p.224), 차분방정식 표현(p.232), 스펙트럼 표현(p.236), **매칭 필터**(p.239), **스펙트럼 인자화·혁신 표현**(p.249), 고계 모먼트 변환(p.261)
6. **Estimation** (p.279) — 모수 추정(p.280), 1·2모먼트 추정(p.301), **베이스(Bayes) 추정**(p.311), **선형 평균제곱 추정**(p.319)
7. **Optimal Filtering** (p.337) — 직교 원리(p.338), 선형 예측 필터링(p.341), **FIR**(p.347)·**IIR**(p.356) 최적 필터, 순환(p.379), **Wold 분해**(p.390)
8. **Linear Prediction** (p.409) — AR 모델(p.411), AR 프로세스 선형예측·역예측/비인과 AR, **Levinson 순환**(p.422), 격자 표현·반사 계수, **최소위상 성질**(p.441), **Schur 알고리즘**(p.444), 스플릿(p.458), 삼각분해, FIR Wien 필터 격자(p.491)
9. **Linear Models** (p.503) — 랜덤 프로세스 선형 모델링(p.504), 데이터로부터 모수 추정(p.514), 최소제곱 원리(p.518), AR/ARMA 모델링(p.535·p.550), 최소제곱·**Yule-Walker 방정식**(p.564), 예제·비교
10. **Spectrum Estimation** (p.585) — 고전 스펙트럼 추정(p.586), 선형모델 기반(p.596), **최대우도 스펙트럼 추정**(p.607), **서브스페이스법**(p.614), 고급 주제 참조(p.656)
+ 부록 A: 벡터 방향 최적화(p.685), 부록 B: 대역통과 신호·시스템의 복소 표현(p.696), 용어집(p.712) `[raw/books/discrete-random-signals.md]`

## 핵심
- **이산시간 중심** — CT 랜덤 프로세스를 샘플링으로 취급하지 않고, 처음부터 이산 시간·유열·변환으로 랜덤 프로세스를 전개. 서문 "순수한 이산 관점"이 책 전체 편성을 결정 `[raw/books/discrete-random-signals.md]`
- 장 5 **스펙트럼 인자화·혁신 표현**(p.249)과 장 7 **Wold 분해**(p.390)가 선형 예측·최적필터의 이론적 뿌리 — AR 모델(장 8.2) → Levinson → 격자 → Schur로 이어지는 "선형예측 알고리즘 군"이 이 책의 최대 특징
- 장 10 **최대우도 스펙트럼 추정** + **서브스페이스법(p.614)**이 [[estimation-theory]](Mendel)의 추정-스펙트럼 접점과 [[information-coding-theory]]의 스펙트럼-코딩 대칭을 잇는 실용 지점
- 매칭 필터(p.239)가 확률론과 신호처리를 결합한 "최적 수신기"의 첫 등장 — CDMA/확산 스펙트럼([[cdma-dss-spread-spectrum]])의 수신 이론 기반

## Related
- 고전 확률론: [[probability-random-variables]] (Papoulis, 특성함수 중심) · [[probability-random-process]] (Leon-Garcia, 통신 응용)
- 추정·스펙트럼: [[estimation-theory]] (Mendel, 26 레슨) · [[estimation-and-filtering]] (추정-필터링 개념)
- 클러스터: [[stochastic-processes-cluster]]
- 인접: [[cdma-dss-spread-spectrum]] · [[information-coding-theory]]
