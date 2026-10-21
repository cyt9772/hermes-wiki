---
title: Numerical Recipes in C, 2nd ed. (Press et al.)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, engineering-mathematics, numerical-methods]
sources: [raw/books/numerical-recipes-in-c.md]
confidence: high
---
# Numerical Recipes in C, 2nd ed. (Press·Teukolsky·Vetterling·Flannery)

> "Our aim in writing the original edition of Numerical Recipes was to provide a book that combined general discussion, analytical mathematics, algorithmics, and actual working programs." (Preface to the Second Edition, raw p. 10)
> 저자: William H. Press (Harvard-Smithsonian CfA), Saul A. Teukolsky (Cornell), William T. Vetterling (Polaroid), Brian P. Flannery (EXXON), Cambridge University Press, 2nd ed. 1992 (ISBN 0-521-43108-5), 1022p

## 개요
**"The Art of Scientific Computing"** — 수치해석 알고리즘을 C 언어로 구현하는 실무 교과서. "일반적 논의 + 해석 수학 + 알고리즘 + 실제 동작 프로그램" 4요소를 결합하는 것을 명시적 목표로 내세우며, 각 소절마다 알고리즘 설명 뒤 C 함수(소스 코드)를 붙이는 구조. Fortran·Pascal·BASIC 번역판도 동시 발행. `^[raw/books/numerical-recipes-in-c.md]`

## 장 구조 (20장 + 부록 A-C, 1022p)
1. **서론** — 프로그램 구조, C 관습, 오차·정확도·안정성 (roundoff vs truncation error)
2. **선형대수방정식해** — Gauss-Jordan, LU 분해, 삼대각, SVD, 희소행렬, Cholesky·QR 분해
3. **보간·외삽 (Interpolation/Extrapolation)** — 다항·라시온(rational function) 보간, **3차 스플라인**, 2차원 이상 보간
4. **함수적분 (Integration)** — 등간격 공식, **Romberg 적분**, 부적분(수렴적분), **가우스 적분**·직교 다항식, 다차원
5. **함수평가** — 급수·연결성, 연속분수, 클렌쇼우(Clenshaw) 반복, 2·3차방정식, 수치미분, **체비셰프(Chebyshev) 근사**, Padé
6. **특수함수** — 가마·베타, 오차함수, 베셀(정수/수정/분수), 구면하모니크, 프레셀·타원적분·야코비 타원
7. **난수** — 균등/지수/정규 변환, 거절법, 암호 기반, Monte Carlo·준난수
8. **정렬** — 삽입·Shell, Quicksort, Heapsort, 선택·순위
9. **루트탐색·비선형연립방정식** — 브래킷팅·이분법, 세칸트·위앙가르덴-데커-브렌트(Dekker-Brent), Newton-Raphson(연립), 전역수렴법
10. **함수의 최소·최대화** — 1차원 골든섹션, Brent법, 단순법(Simplex), Powell 방향집합법, 쌍직각법(Conjugate Gradient), 가변메트릭법, 선형프로그래밍·단순법(LP), 시뮬레이티드 어닐링(모의열화)
11. **고유값 문제 (Eigensystems)** — Jacobi, Householder·기번스(삼대각화), QR 알고리즘(헤센버그), 역반복(Inverse Iteration)
12. **푸리에·FFT** — 이산샘플 푸리에, **고속푸리에변환(FFT)**, 2차원 FFT, 메모리-로컬 FFT
13. **푸리에·스펙트럼 응용** — 컨볼루션/디컨볼루션(FFT), 상관, **Wiener 필터**, 전력스펙트럼, 선형예측, **웨이브릿(Wavelet)**
14. **데이터의 통계적 서술** — 모멘트·분산·왜도(skewness), 분포동일성 검정, 선형상관·비모수 랭크 상관, Savitzky-Golay
15. **최소제곱** — 직선·2좌표오차, 일반 최소제곱, 비선형 모형, 신뢰한계
16. **상미분방정식 수치해** — **Runge-Kutta**·적응스텝, Bulirsch-Stoer(Richardson), 경계층, 다단계·예측-보간
17. **2점경계값** — Shooting, 이완법
18. **적분방정식·역문제** — Fredholm·Volterra, Backus-Gilbert, 최대엔트로피
19. **편미분 수치해** — Flux-Conservative, 확산형, 다차원, Fourier·Cyclic Reduction, 멀티그리드
20. **비수치 해법** — Gray 코드, CRC, **Huffman 압축**, 부동소수점
+ 부록 A(타입선언), B(PUBLIC DOMAIN 서브루틴), C(복소산술)

## 핵심 기여
- **알고리즘 + C 코드 병기** — "알고리즘 설명 뒤 실제 C 함수" 패턴이 이 분야의 표준 교재 형식을 확립
- **오차 분류의 정립적 설명** — roundoff error(하드웨어) vs truncation error(algorithm) 분리와 안정성 논리 (1.3, "clever minimization of truncation error is practically the entire content of the field of numerical analysis!") `^[raw/books/numerical-recipes-in-c.md]`
- **스펙트럼 분석(13장)의 실무 통합** — FFT를 통한 보편적·상관·Wiener 필터·전력스펙트럼·선형예측을 한 장에 묶어 과학 컴퓨팅의 주류 도구로

## C 코드 snippet (2.1 gaussj)
```c
void gaussj(float **a, int n, float **b, int m)
{
    int *jndxc, *indxr, *ipiv;
    int i, icol, irow, j, k, l, ll;
    float big, dum, pivinv, temp;
    indxc = ivector(1, n);
    indxr = ivector(1, n);
    ipiv  = ivector(1, n);
    for (j = 1; j <= n; j++) ipiv[j] = 0;
```
> 주의: 원문에 깨진 토큰이 있다 — `mnt`→`int`, `mllt`→`int`, `big` 비교식 일부, 주석 한글화 없음(영문). 실제 코드는 원본 PDF(raw p. 55~56) 대조 필요.

## OCR 신뢰도
- 텍스트 레이어 내장본 (pdftotext -layout, OCR 없음) — 본문은 양호
- **주의**: C 코드의 일부 토큰이 깨짐 (`mnt`, `mllt`, `a[j][k]` 등) — code fence로 복원 시 원본 PDF 대조 필수
- 수식 번호·식 본문은 양호

## Related
- 개념: [[numerical-methods-science-computing]], [[differential-equations-engineering]]
- 관련 책: [[advanced-engineering-mathematics]] — 같은 수치해법 영역을 Kreyszig식 이론 체계로 다룸
