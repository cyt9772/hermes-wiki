---
title: Linear System Theory and Design
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, state-space-control, linear-algebra, differential-equations, signal-processing]
sources: [raw/books/linear-system-theory-design.md]
confidence: high
---
# Linear System Theory and Design

> Chi-Tsong Chen, State University of New York at Stony Brook — Prentice Hall, 682p. **다변수 선형 시스템·제어 설계** 대학원 교과서. 1970년 같은 저자 *Introduction to Linear System Theory*의 "major revision"으로 서문에 명시 `[raw/books/linear-system-theory-design.md]`.

## 개요
"상·대학원급 선형 시스템·다변수 설계 과정"용(서문). 선진 수학 = 행렬 조작 + Elementary ODE. 별표(★) 없는 절은 Stony Brook 1차 선형시스템 강의에서 10여 년간 사용, 별표 절은 2차 과정(다변수 시스템)에서 개발 — 즉 **1차 코어 과정과 2차 다변수 과정를 한 책으로 통합**. 선형대수(장 2) → 시스템 표현(장 3) → 상태공간 해석(장 4~6) → 피드백·계측기(장 7) → 안정(장 8) → 합성 시스템 설계(장 9)로 흐르는 9장+부록 구성 `[raw/books/linear-system-theory-design.md]`.

## 장 구조 (원문 TOC 기준, 9장 + 부록 A~G)
1. **Introduction** (p.1) — 시스템 연구, 책의 범위
2. **Linear Spaces and Linear Operators** (p.6) — 선형 공간·기저·표현, 선형연산자·행렬 표현, **대수·고차 대수·Jordan형**(p.33), 행렬 함수(p.45), 노름·내적
3. **Mathematical Descriptions of Systems** (p.70) — 입력-출력 묘사(선형/인과/relaxed/시불변, 전달함수행렬), **상태변수 묘사**(상태개념 p.83, 동역학방정식), 두 묘사 비교, 합성시스템, ★이산시간(p.121)
4. **Linear Dynamical Equations and Impulse-Response Matrices** (p.133) — 방정식 해(시변/불변), 동치 동역학방정식, 임펄스응답행렬, ★주기 A(t)·Floquet
5. **Controllability and Observability** (p.168) — 시간함수 선형독립, 시변/불변 **제어가능성**(p.175)·**관측가능성**(p.192), 정준분해(canonical decomposition, 장 5-5), Jordan형 시스템, ★출력 제어가능성, ★계산 문제
6. **Irreducible Realizations, Strict System Equivalence, and Identification** (p.232) — 적정 가역행렬 특성다항식·도수, 불가환 실현(관측/제어 정준형, Hankel, Jordan), 벡터 전달함수 실현, ★Hankel법(SVD·행검색)·공약분해법·다항식행렬 표현, ★엄밀(한) 시스템 등가, ★오염없는 데이터로부터 이산시스템 **식별**(p.300)
7. **State Feedback and State Estimators** (p.324) — 정준형 방정식, **상태피드백**(단변수 p.334/다변수, 고유치·고유벡터 할당 p.351), **상태 추정기**(전차원 p.355/감소차원 p.361), 분리 원리, ★해제(decoupling)
8. **Stability of Linear Systems** (p.384) — 입력-출구 안정, **Routh-Hurwitz**(p.395), 동역학방정식 안정, ★Lyapunov 정리(p.412), ★이산시간
9. **Linear Time-Invariant Composite Systems** (p.432) — 완전 특성, 합성시스템 제어/관측(병렬·직렬·피드백), 피드백 안정, **단일피드백 보상기 설계**(단변수 p.458/단입단출/다변수 고유치·분모행렬 할당 p.468~478, **해제 p.486**), **점근 추적·장애 거부**(p.488), 입력-출구 피드백 보상기, ★minimum-energy 제어
+ 부록: A 초등행렬 연산, B 실변수 해석함수, C 최소에너지 제어, D 샘플링 후 제어가능성, E 헤르미트 형식·SVD, F 행렬방정식 AM+MB=N, G 다항식·다항식행렬, H(선형대수 보충) `[raw/books/linear-system-theory-design.md]`

## 핵심
- **상태공간+행렬이론 선진** — 장 2가 선형 공간·Jordan형·행렬 함수를 "시스템"이 아닌 **연산자 기학**으로 다룸. 이건 [[linear-algebra-and-its-applications]](Strang)의 응용 쪽이 아니라 이론 쪽의 선형대수. 행렬 지수(e^At 계산 p.~)·Cayley-Hamilton·Jordan 표준형이 제어가능성/관측가능성(장 5·6)의 토대
- **제어가능성·관측가능성 → 불가환 실현 → 상태피드백·계측기 → 합성 시스템 설계**이라는 5단 구조가 이 책의 골격. 분리 원리(장 7-5)가 "피드백+계측기"를 독립 설계하는 근거 — [[estimation-theory]](Mendel)의 Kalman/BLUE가 "최적"이라면, 이 책은 **대수·기하 구조** 기반
- 장 6 ★식별(오염없는 데이터, 지속적 자극 입력, p.300)과 장 7 ★해제가 선형시스템↔시스템식별/통계적 추정([[discrete-random-signals]] 장 9 AR/ARMA 모델링)의 접점. 두 클러스터 사이 다리가 이 장에 있음
- Routh-Hurwitz(장 8-3)·Lyapunov(장 8-5)이 미분방정식 축(원문 differential-equations 클러스터)과 연결 — 이 페이지에서는 텍스트로만 언급, 위키링크는 금지(다른 클러스터 소유)

## Related
- 저자: [[chi-tsong-chen]]
- 개념: [[linear-system-control]] (상태공간·제어·시스템 클러스터) · [[estimation-and-filtering]] (옵티멀 추정 접점)
- 인접: [[linear-algebra-and-its-applications]] (선형대수 이론) · [[signals-and-systems-oppenheim]] (제11장 피드백과의 연계)
