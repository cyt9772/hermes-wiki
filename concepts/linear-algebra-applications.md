---
title: 선형대수 응용 (Linear Algebra & Applications)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, linear-algebra, engineering-mathematics]
sources: [raw/books/linear-algebra-and-its-applications.md]
confidence: high
---
# 선형대수 응용 (Linear Algebra & Applications)

행렬·벡터 공간·고유값·행렬 분해를 **구조적**으로 다뤘을 때 회로(네트워크), 동역학(차분/미분방정식), 신호(FFT), 최적화(LP·게임이론)로 확장되는 공학 수학의 기초. Strang 교재(3rd ed., 1988) 한 권이 이 응용 지도를 통째로 담고 있다.

## Linear Algebra and Its Applications (Strang 1988)
- **4 기본 공간**(row/column space, two nullspaces) — 선형방정식해의 구조를 정리(제2.4절) `[raw/books/linear-algebra-and-its-applications.md]`
- **네트워크와 incidence matrix**(제2.5절) — 회로 분석을 선형대수로 정식화 `[raw/books/linear-algebra-and-its-applications.md]`
- **정방행렬 분해 계보**: LU(gauss elimination, 제1-2장) → QR·**Gram-Schmidt**·least squares(제3장) → **고유값/diagonal form**(제5장) → **SVD·pseudoinverse(부록 A)·Jordan form(부록 B)** `[raw/books/linear-algebra-and-its-applications.md]`
- **동역학 연결**: difference equation + Aⁿ, differential equation + e^{At}(제5장) — 상태공간·지수응답의 수학 `[raw/books/linear-algebra-and-its-applications.md]`
- **FFT를 정방행렬(orthogonal/unitary)로 다룸**(제3.5절) — DSP의 FFT(Porat 제5장)와 같은 수학 `[raw/books/linear-algebra-and-its-applications.md]`
- **최적화 접점**: simplex·Karmarkar, duality, network models, **minimax theorem**(제8장) `[raw/books/linear-algebra-and-its-applications.md]`

## 응용 맵 (Strang 구조 기준)

| 선형대수 테마 | Strang 위치 | 공학 응용 |
|---|---|---|
| 가우스 소거·LU | 제1장 | 방정식 해법, 수치 계산 |
| 4 기본 공간 | 제2.4절 | 해의 존재/유일성, 구조 |
| incidence matrix | 제2.5절 | 회로/네트워크 |
| least squares·QR | 제3장 | 회귀·추정 |
| FFT(unitary) | 제3.5절 | DFT/FFT, 스펙트럼 |
| 고유값·e^{At} | 제5장 | 동역학·안정성 |
| SVD·pseudoinverse | 부록 A | 압축·근사·DCT 계열 변환 |
| LP·minimax | 제8장 | 최적화·게임 |

## 관련
- [[linear-algebra-and-its-applications]]
- [[a-course-in-dsp]] (FFT·DFT의 선형대수적 해석), [[signals-and-systems-korea]] (상태공간·동적특성)
- MATLAB 실습 축: [[linear-algebra-matlab]] (LU·QR·SVD 수치 실험) · [[signals-systems-matlab]] (DFT·라플라스·Z MATLAB) · [[matlab-statistical-analysis]] (통계 수치)
- 인접: [[advanced-engineering-mathematics]], [[numerical-methods-science-computing]]
