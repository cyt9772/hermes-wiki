---
title: Elementary Differential Equations with Linear Algebra (Ross L. Finney & Donald R. Ostberg)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, differential-equations, linear-algebra, engineering-mathematics]
sources: [raw/books/elementary-differential-equations.md]
confidence: high
---
# Elementary Differential Equations with Linear Algebra (Ross L. Finney & Donald R. Ostberg)

> 저자: **Ross L. Finney** (University of Illinois — Urbana) · **Donald R. Ostberg** (Northern Illinois University) · with the assistance of **Robert G. Kuller** (Northern Illinois University)
> 출판: Addison-Wesley, 1976 (1st ed. 1968, Kreider·Kuller·Ostberg). ©1976, 1968 Addison-Wesley Publishing Company. Addison-Wesley Series in Mathematics (Consulting Editor: Lynn H. Loomis). Library of Congress Card No. 75-12096, ISBN 0-201-05515-X.
> 1st edition: *Elementary Differential Equations* — Donald L. Kreider, Robert G. Kuller, Donald R. Ostberg (1968)

## 개요
학부 공학·과학을 위한 상미분 + 선형대수 통합 교과서. "미분방정식은 인간이 세계를 묘사하는 기본 도구"라는 목표로 전 장에 물리·생물·경제 **적용 예**를 배치. 1계 상미분(Ch.1) 직후 2장이 선형대수, 3장에 미분 연산자, 4-5장에 연산자 기반 상수계수 선형방정식, 6장에서 Laplace로 이어지는 **통합적 전개**가 특징.

## 장 구조 (11장, 526p 기반)
| # | topic | pp |
|---|-------|----|
| 1 | First-Order Differential Equations (분리가능, homogeneous coefficients, exact, integrating factor, reduction of order, geometric & physical applications) | 1–44 |
| **2** | **The Elements of Linear Algebra** (real vector spaces, subspaces, linear independence, bases, coordinate systems, dimension, determinants) | **45–83** |
| 3 | Linear Transformations and Linear Differential Operators (product, polynomials, null space & image, operator equations, 1계 선형 차분방정식) | 84–112 |
| 4 | Linear Differential Equations (1계 선형, 존재·고유, solution space, **Wronskian**, **Abel formula**) | 113–151 |
| 5 | Equations with Constant Coefficients (2계·n계 homogeneous, variation of parameters & Green's functions, reduction of order, undetermined coefficients, Euler equation, **capacitor circuits**, **Kepler/뉴턴 중력**) | 152–207 |
| 6 | The Laplace Transform (piecewise, exponential order, convolution, Green's functions, 조화 spring, 에너지·tautogram, 변환 표) | 208–264 |
| 7 | Series Solutions (power series, ordinary/singular point, **Legendre**, Bessel, Bessel properties) | 265–308 |
| 8 | Oscillation Theory (separation theorem, standard·self-adjoint, comparison, Sonin-Polya, Bessel zeros) | 309–319 |
| **9** | **Matrices and Systems of Linear Equations** (linear transformations and bases, matrix of a linear transformation, addition, multiplication, change of basis, systems of linear equations, **eigenvalues & eigenvectors**) | **320–354** |
| 10 | Systems of Linear Differential Equations (1계 계통, complex/repeated eigenvalues, biol.·econ.·phys. applications) | 355–391 |
| 11 | Direction Fields and Numerical Methods (existence theorem, uniqueness, **Euler**, **modified Euler**) | 392–435+ |

## 핵심 기여
- **선형대수 → 미분방정식 통합** — 2장의 벡터 공간·기저·좌표계·행렬은 3장의 선형 미분 연산자(차등 연산자)와 4장의 Abel·Wronskian, 9장의 eigenvalue 기반 연립방정식 해법에서 "수학적 뼈대"로 작용.
- **연산자 관점** — 3장에서 `L[y] = y'' + p(t)y' + q(t)y` 형태의 선형 연산자를 정교하게 정의하여, 상수계수·매개변수변수법·Laplace·급수해법을 단일 연산자 체계로 통합.
- **Wronskian · Abel formula** (Ch. 4)가 2계 해의 구조를 다룸.
- **Euler·modified Euler 수치해법** (Ch. 11)은 존재·고유 정리와 병행 — 해석법과 수치법의 병치.
- **Kepler·뉴턴 중력** (Ch. 5.10), **물리 회로** (Ch. 5.9), **생물·경제 적용** (Ch. 10) — 이공학 적용.

## Related
- 저자: [[ross-finney]] · [[donald-ostberg]]
- 개념: [[differential-equations-linear-system]] (이 책의 중심) · [[differential-equations-engineering]] (Kreyszig 편미분·복소함수 — 상호 보완) · [[linear-algebra-and-its-applications]] (Strang 대수 관점)
- 인접: [[numerical-methods-science-computing]]

## OCR/추출 신뢰도
- pdftotext 양호. 서명·책명 일부 토큰 깨짐(한자형 변형) — 식 번호·문맥으로 cross-check. 장 구조는 TOC 영역서 재확인.
