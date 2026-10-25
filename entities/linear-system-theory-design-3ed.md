---
title: Linear System Theory and Design (3rd ed.)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, state-space-control, linear-algebra, differential-equations, signal-processing]
sources: [raw/books/linear-system-theory-design-3ed.md]
confidence: high
---
# Linear System Theory and Design (3rd ed.)

> Chi-Tsong Chen, SUNY Stony Brook — Oxford University Press, 1999, 343p. **1970년 *Introduction to Linear System Theory*의 "complete rewriting"** — 서문: "This edition is a complete rewriting of the book Linear System Theory and Design, which was the expanded edition of Introduction to Linear System Theory published in 1970" [raw/books/linear-system-theory-design-3ed.md].

## 개요
"상·대학원급 선형 시스템·다변수 설계 과정"용. 수학적 토대: 선형대수(Laplace + 행렬) + "elementary differential equations". 1970년 1판 대비 **두 가지 큰 변화**: (1) "the geometric approach, the abstract algebraic approach, rational fractions, and optimization are not discussed" (범위 축소), (2) "the polynomial fraction design in the input/output feedback (controller/estimator) configuration is deleted. Instead we discuss design in the two-parameter configuration" (2-param model matching 도입). 9장 + References(p.319) + Answers(p.321) + Index(p.331). 장 6 서두: "If we use a minimal realization to implement a transfer function, then the number of integrators used in an op-amp circuit will be minimum. Thus minimal realizations are of practical importance" (p.184) [raw/books/linear-system-theory-design-3ed.md].

## 장 구조 (TOC 기준, 9장)
1. **Introduction** (p.1)
2. **Mathematical Descriptions of Systems** (p.5) — 인과성·집중성, LTI, Op-Amp 구현, 선형화, RLC, 이산시간
3. **Linear Algebra** (p.44) — 기저·표현·직교화, 유사변환, 대각·Jordan형, 행렬함수, **Lyapunov, SVD, 행렬노름**
4. **State-Space Solutions and Realizations** (p.86) — LTI 상태방정식 해, 이산화, 정준형, 실현, LTV
5. **Stability** (p.127) — BIBO, internal/absolute, **Lyapunov 정리**, LTV
6. **Controllability and Observability** (p.143) — 제어·관측가능성 지수, 정준분해, Jordan 조건, 샘플링 후 제어가능성
7. **Minimal Realizations and Coprime Fractions** (p.184) — 공약분열, **QR 분해, balanced realization, Markov 매개변수**, 행렬 공약분열
8. **State Feedback and State Estimators** (p.231) — Lyapunov 방정식, regulation·tracking, 강인 추적, 다변수 상태피드백·추정기, **분리 원리**
9. **Pole Placement and Model Matching** (p.269) — single-loop pole placement, **two-parameter model matching**, multivariable, decoupling, internal model
+ References (p.319) · Answers to Selected Problems (p.321) · Index (p.331)

## 핵심
- **3rd ed. = "완전 rewrite"가 아니라 "범위 재정의"** — 1판의 "정규형·식별·decoupling"을 삭제하고, **two-parameter model matching(장 9)**을 "주된 설계 방식"으로 승격. "this configuration seems to be more suitable for practical application" (서문) [raw/books/linear-system-theory-design-3ed.md]
- **LTI 상태공간 → 제어·관측 → 최소 실현 → 상태피드백·추정기 → 폴할당·모델매칭**의 5단 구조가 2nd ed.와 동일하되, **장 7(Minimal Realizations + Coprime Fractions)의 위치가 강화**됨 — "QR Decomposition"(7.3.1, p.195)·"balanced realization"(7.4, p.197)이 2nd ed.에 없던 **수치해석 도구**
- **Lyapunov 정리(장 5.4, p.132)**를 "안정성 = 기본 시스템 개념"으로 제시: "Every system must be designed to be stable; otherwise, it may burn out or disintegrate. Therefore stability is a basic system concept" (장 5 서두, p.127) [raw/books/linear-system-theory-design-3ed.md]
- **SVD·QR·Lyapunov 방정식 3종**을 "MATLAB으로 계상 가능한 선형대수 도구"로 통합 — [[linear-algebra-and-its-applications]](Strang)의 응용 쪽이 아닌 **제어·시스템 이론 쪽의 선형대수**
- 1판과 3rd ed.의 차이: 1판의 "geometric/abstract algebraic approach" → 3rd ed.의 "polynomial fraction + state-space" 2축. 이 변경은 **[[signals-and-systems-oppenheim]]**(LTI 이론)과 **[[estimation-and-filtering]]**(장 8 추정기)의 접점

## 저자·관련
- 저자: [[chi-tsong-chen]]
- 개념: [[linear-system-control]] · [[linear-algebra-applications]] (장 3) · [[differential-equations-engineering]] (장 2 서두)
- 인접: [[linear-system-theory-design]] (2nd ed, 같은 저자 — **이 페이지의 전판**) · [[signals-and-systems-oppenheim]] (LTI 기반) · [[estimation-and-filtering]] (장 8 상태 추정기) · [[contemporary-linear-systems-matlab]] (MATLAB 실습서)
