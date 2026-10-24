---
title: Linear Algebra and Its Applications (Strang 1988)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, linear-algebra, engineering-mathematics]
sources: [raw/books/linear-algebra-and-its-applications.md]
confidence: high
---
# Linear Algebra and Its Applications (Strang 1988)

> 표지/원저: **Gilbert Strang** (Massachusetts Institute of Technology)
> 출판: Saunders College Publishing, Harcourt Brace Jovanovich, 3rd ed. 1988, 517p (ISBN 0-15-551005-3)

## 개요
Gilbert Strang(MIT)의 선형대수 교과서 3판. "Fantastic subject" (preface)이라는 표현 그대로 **수학적 구조와 응용을 동시에** 다룸 — 가우스 소거·행렬 곱(제1장) → vector space·**4 basic subspaces**(행/열/핵/좌핵)·network·incidence matrix·linear transformation(제2장) → orthogonality·projection·least squares·Gram-Schmidt·**Fast Fourier Transform**(제3장, 선형대수 내재) → determinant(제4장) → eigenvalue/eigenvector·diagonal·difference/differential equation·Hermitian/Unitary·similarity(제5장) → positive definite(제6장) → 행렬 연산(제7장) → **linear programming·game theory·minimax** (제8장). 부록에 **SVD·pseudoinverse**(부록 A), **Jordan form**(부록 B), **computer code**(부록 C) — DCT, DSP, 신호·시스템 같은 "engineering-math" 기초 서적 `[raw/books/linear-algebra-and-its-applications.md]`.

## 장 구조 (8장 + Appendix A-C, 517p)
1. **MATRICES AND GAUSSIAN ELIMINATION** — 기하, elimination, matrix multiplication, triangular factors, inverses/transposes, special matrices and applications
2. **VECTOR SPACES AND LINEAR EQUATIONS** — subspace, m 방정식 n 미지수, linear independence/basis/dimension, **the four fundamental subspaces**, **networks and incidence matrices**, **linear transformations**
3. **ORTHOGONALITY** — orthogonal subspace, inner product/projection, **least squares approximation**, orthogonal bases/Gram-Schmidt, **The Fast Fourier Transform(3.5)**, review and preview
4. **DETERMINANTS** — 성질, 공식, applications
5. **EIGENVALUES AND EIGENVECTORS** — diagonal form, **difference equations and Aⁿ**, **differential equations and e^{At}**, **complex matrices(symmetric vs Hermitian, orthogonal vs unitary)**, **similarity transformations**
6. **POSITIVE DEFINITE MATRICES** — min/max/saddle, 판별, semi-definite/indefinite
7. **COMPUTATIONS WITH MATRICES**
8. **LINEAR PROGRAMMING AND GAME THEORY** — linear inequalities, **simplex/Karmarkar**, duality, network models, minimax theorem
+ APPENDIX A **SVD and the Pseudoinverse** (p.442)
+ APPENDIX B **The Jordan Form** (p.453)
+ APPENDIX C **Computer Codes for Linear Algebra** (p.461), References, Index

## 핵심 내용
- **4 basic subspaces**(row space, column space, null space, left null space)를 명시적으로 다룸(제2.4절) — 선형대수의 핵심 구조 `[raw/books/linear-algebra-and-its-applications.md]`
- **FFT를 선형대수 내재**(제3.5절)로 다룸 — orthogonality·unitary matrix 관점 — DSP 교과서([[a-course-in-dsp]] 제5장)의 FFT와 수학 구조에서 연결 `[raw/books/linear-algebra-and-its-applications.md]`
- **eigenvalue·e^{At}·difference/differential equation** 연결(제5장) — 제어·신호·시스템 동역학 기반 `[raw/books/linear-algebra-and-its-applications.md]`
- **SVD·pseudoinverse(부록 A)·Jordan(부록 B)** — DCT, DPCM, image compression 같은 "engineering-math" 응용의 기초 `[raw/books/linear-algebra-and-its-applications.md]`
- **Linear programming·game theory(제8장)** — 선형대수가 optimization·economics로 확장되는 시점 `[raw/books/linear-algebra-and-its-applications.md]`

## Related
- 저자: [[gilbert-strang]]
- 개념: [[linear-algebra-applications]] — 선형대수 응용 클러스터 개념
- 인접: [[a-course-in-dsp]] (FFT), [[signals-and-systems-korea]] (동역학 기반), [[dct-algorithms-applications]] (변환·구조), [[advanced-engineering-mathematics]] (공학 수학)
