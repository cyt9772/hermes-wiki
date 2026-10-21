---
title: 수치해법 — 과학 컴퓨팅 (Numerical Methods for Science and Computing)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering-mathematics, numerical-methods]
sources: [raw/books/numerical-recipes-in-c.md, raw/books/advanced-engineering-mathematics.md]
confidence: high
---
# 수치해법 — 과학 컴퓨팅 (Numerical Methods for Science and Computing)

## 정의
**수치(이산, discrete) 근사로 연속 수학적 문제를 풀 때의 방법론**. 보간·적분·미분·루트탐색·고유값·푸리에·최소제곱·상미분·편미분으로 구성되며, 알고리즘의 **오차(stability, truncation, roundoff)** 분석이 핵심.

## 두 소스의 관점
### Numerical Recipes in C (Press et al., 1992) — C 구현 관점
> "The discrepancy between the true answer and the answer obtained in a practical calculation is called the truncation error. ... It is only a slight exaggeration to say that clever minimization of truncation error is practically the entire content of the field of numerical analysis!" (§1.3, raw p. 55~56)

> "Our aim in writing the original edition of Numerical Recipes was to provide a book that combined general discussion, analytical mathematics, algorithmics, and actual working programs." (Preface, raw p. 10)

**핵심 기여**: 각 소절마다 **C 함수 코드 + 알고리즘 설명**을 병기하는 표준 형식을 확립. Romberg 적분(4.3), 가우스 적분(4.5), FFT(12.2), QR 알고리즘(11.6), 가변메트릭법(10.7) 등 실무 도구.

### Kreyszig 8th ed. (1999) — 이론 체계 관점
> "The idea of error estimation by halving. Changes in Sec. 17.4 on splines, in Sec. 17.5 on error estimates in integration. Adaptive integration and Romberg integration included (Sec. 17.5)." (Preface, raw p. 9)

> "Runge-Kutta-Fehlberg method (Sec. 19.1), extension of Euler and Runge-Kuua methods to systems and higher order equations (Sec. 19.3) included." (Preface, raw p. 10)

**핵심 기여**: 수치해법을 독립 파트(Part E, Chaps. 17-19)로 설정 — 오차 전파(17.1), 반복·보간(17.2-17.4), 적분·미분(17.5), LU 분해·최소제곱·고유값(18.1-18.9), Euler/RK-F/다단계·편미분(19.1-19.7).

## 공통 주제
| 주제 | NR (C) | Kreyszig |
|---|---|---|
| 보간·스플라인 | 3.1-3.5 | 17.3-17.4 |
| 적분 | 4.1-4.6 (Romberg, 가우스) | 17.5 (Romberg, 적응적분) |
| 상미분 수치해 | 16.0-16.7 (RK, bulirsch-stoer, stiff) | 19.1-19.3 (RK-F, Euler 확장) |
| 편미분 수치해 | 19.0-19.6 (flux-conservative, multigrid) | 19.4-19.7 (elliptic, parabolic, hyperbolic) |
| 고유값 | 11.0-11.7 (Jacobi, QR, inverse iteration) | 18.6-18.9 (power method, QR) |
| 푸리에·FFT | 12.0-12.6, 13장(스펙트럼) | 10.8-10.10 (푸리에 적분·변환) |

## Related
- 책: [[numerical-recipes-in-c]], [[advanced-engineering-mathematics]]
- 개념: [[differential-equations-engineering]]
