---
title: Probability, Random Variables, and Stochastic Processes (2nd ed)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, stochastic-processes, engineering-mathematics]
sources: [raw/books/probability-random-variables.md]
confidence: high
---
# Probability, Random Variables, and Stochastic Processes (2nd ed, International)

> A. Papoulis, McGraw-Hill (1991), 682p. 공학(특히 EE·통신) 대학원 수준의 확률론·확률과정 고전 교과서 — 확률론(부1)과 확률과정(부2)을 하나의 수학 체계로 잇는 2부 구성 `[raw/books/probability-random-variables.md]`.

## 개요
부 I(장 1~9)는 공리에서 출발해 확률 공간, 조건부 확률, 랜덤 변수와 그 함수, 다변수 분포, 모멘트·특성함수, 랜덤 변수 계열과 통계(모수 추정·가설검정)까지 확률론 자체를 다룸. 부 II(장 10~16)는 이 확률론을 과정(시간 인덱스 랜덤 변수)에 올려, LTI 시스템 통과 · 스펙트럼 표현/추정 · 평균제곱 추정 · 엔트로피까지 이어가는 "공학 확률"의 전범 `[raw/books/probability-random-variables.md]`.

## 장 구조 (원문 TOC 기준, 2부 16장)
**부 I — 확률과 랜덤 변수**
1. The Meaning of Probability (p.4) — 확률의 정의, 확률과 귀납, 인과 vs 무작위
2. The Axioms of Probability (p.15) — 집합론, 확률공간, 조건부 확률
3. Repeated Trials — 결합 사건, 이항, 극한 정리, 푸아송 정리·랜덤 포인트
4. The Concept of a Random Variable (p.63) — 분산·밀도, 조건부 분포
5. Functions of One Random Variable (p.86) — 분포의 g(x), 평균·분산, 모멘트, **특성함수**(p.115)
6. Two Random Variables (p.124) — 이변수 분포, 두 랜덤 변수의 함수
7. Moments and Conditional Statistics (p.151) — 결합 모멘트·**결합 특성함수**, 조건기대, **평균제곱 추정**(p.173)
8. Sequences of Random Variables (p.182) — 조건부 특성함수·정규성, 확률 수렴·극한 정리, 랜덤 수 생성
9. Statistics (p.241) — **모수 추정**(p.244), **가설 검정**(p.265)

**부 II — 확률과정**
10. General Concepts (p.285) — 정의, **확률적 입력을 가진 시스템**(p.303), **파워 스펙트럼**(p.319), 디지털 과정(p.332)
11. Basic Applications (p.345) — 랜덤 워크·브라운 운동·열잡음, 푸아송 포인트·샷 노이즈, 변조, 순환정상, 대역제한·샘플링 정리, 노이즈 속 결정신호, **바이스펙트럼**
12. Spectral Representation — 확률과정의 스펙트럼 분해
13. Spectral Estimation (p.427)
14. Mean Square Estimation (p.480)
15. Entropy (p.533)
16. Selected Topics (p.603) `[raw/books/probability-random-variables.md]`

## 핵심
- **특성함수**가 확률계산의 중심 도구 — 장 5(단변수, p.115)와 장 7(결합, p.157)에서 극한 정리·정규 분포를 유도하는 통로 `[raw/books/probability-random-variables.md]`
- "확률적 입력을 가진 LTI 시스템"(p.303) + 파워 스펙트럼(p.319)이 신호-시스템 축과 확률 축을 잇는 hinge — 이 한 장이 [[signals-and-systems-oppenheim]]의 확률 없는 세계에 확률이 들어오는 지점
- 장 13 스펙트럼 추정 + 장 14 평균제곱 추정이 [[estimation-and-filtering]]의 고전 근간. Therrien [[discrete-random-signals]] 장 6~10이 정확히 이 흐름의 이산시간·최적화 버전
- 장 15 엔트로피가 확률론과 정보이론([[information-coding-theory]])을 직접 연결 — 확률-정보이론-추정 삼각 구조의 정점

## Related
- 저자: [[a-papoulis]]
- 클러스터: [[stochastic-processes-cluster]] — [[probability-random-process]](공학 응용 편성)와 [[discrete-random-signals]](이산시간 전문)와의 비교
- 개념: [[information-coding-theory]] · [[estimation-and-filtering]]
- **해답집**: [[papoulis-probability-random-variables-2ed-solutions]] — Solutions Manual (182p), 2nd ed. 16장(부 I 확률론 Ch.2–9 + 부 II 확률과정 Ch.10–16) 전수 문제 해법
