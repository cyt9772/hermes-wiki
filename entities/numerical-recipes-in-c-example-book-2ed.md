---
title: Numerical Recipes Example Book in C — 2nd ed. (Press et al., Cambridge UP 1988)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, engineering-mathematics, numerical-methods, scientific-computing]
sources: [raw/books/numerical-recipes-in-c-example-book-2ed.md]
confidence: high
---
# Numerical Recipes Example Book (C) — 2nd ed. (1988)

> 저자: **William T. Vetterling** (Polaroid), **Saul A. Teukolsky** (Cornell), **William H. Press** (Harvard-Smithsonian CfA), **Brian P. Flannery** (EXXON) — Press·Teukolsky·Vetterling·Flannery 4인
> 출판: **Cambridge University Press** (First Edition 1988; **Second Edition originally published 1992** — 이 PDF = 2nd ed. 예제집), 336p (ISBN 0-521-43720-2)
> 원서 인용: "The routines in Numerical Recipes in C: The Art of Scientific Computing, numbering more than 300, are meant to be incorporated into user applications; they are procedures (or functions), not stand-alone (main) programs." (Preface, p. v)
> 원서 인용: "The programming conventions used in this book are discussed fully in Chapter 1 of Numerical Recipes in C... You should have a copy of that book — without it, this one will not be very meaningful." (A Note on Numerical Recipes Utility Functions, p. vii)

## 개요
**Press·Teukolsky·Vetterling·Flannery**의 원서 *Numerical Recipes in C*의 **데모·검증 예제집**. 원서의 300여 C routine을 "단순 예제 프로그램으로 어떻게 호출하고, 어떤 입력을 넣어서 어떤 출력이 나오는지"를 chapter별로 보여주는 companion volume. 각 chapter는 원서와 **정확히 동일한 구성**(20장)이며, 각 routine에 1-3개 demo program + (필요시) sample input/output. `^[raw/books/numerical-recipes-in-c-example-book-2ed.md]`

## 장 구조 (원서 chapter 동일 구성, 336p)
| # | Topic | Book p. |
|---|-------|---------|
| 1 | Preliminaries | 1 |
| 2 | Solution of Linear Algebraic Equations | 6 |
| 3 | Interpolation and Extrapolation | 40 |
| 4 | Integration of Functions | 54 |
| 5 | Evaluation of Functions | 68 |
| 6 | Special Functions | 81 |
| 7 | Random Numbers | 125 |
| 8 | Sorting | 139 |
| 9 | Root Finding and Nonlinear Sets of Equations | 153 |
| 10 | Minimization and Maximization of Functions | 168 |
| 11 | Eigensystems | 185 |
| 12 | Fast Fourier Transform | 195 |
| 13 | Fourier and Spectral Applications | 209 |
| 14 | Statistical Description of Data | 222 |
| 15 | Modeling of Data | 247 |
| 16 | Integration of Ordinary Differential Equations | 264 |
| 17 | Two-Point Boundary Value Problems | 277 |
| 18 | Integral Equations and Inverse Theory | 280 |
| 19 | Partial Differential Equations | 284 |
| 20 | Less-Numerical Algorithms | 290 |
| A | Header Files | 300 |
| B | Utility Functions | 313 |
| C | Complex Arithmetic | 319 |
| — | Index of Demonstrated Routines | 322 |

## 핵심
- **원서 routine의 C demo** — `main()`으로 둘러싼 호출 예제 + sample I/O (각 장)
- **Validation discipline** — "these programs were used during the later stages of the production of Numerical Recipes in C to maintain integrity of the source code" (Preface, p. v)
- **utility function (`nrtype.h`, `mem.h`, `nrutil`) 규약** — A Note on Numerical Recipes Utility Functions (p. vii)
- **2nd ed = 1992 2nd ed 원서 기준** — 예제는 1988 원서(1st ed) 기준 + 2nd ed(1992) 반영

## Related
- 원서: [[numerical-recipes-in-c]] — 이 예제집이 accompaniment하는 **2nd ed 원서**
- 개념: [[numerical-methods-science-computing]]
- 저자: William H. Press (Harvard-Smithsonian), Saul A. Teukolsky (Cornell), William T. Vetterling (Polaroid), Brian P. Flannery (EXXON)
