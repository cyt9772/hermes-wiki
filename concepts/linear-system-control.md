---
title: Linear System, Control, and State-Space (선형 시스템·제어·상태공간)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [concept, state-space-control, signal-processing, linear-algebra]
sources: [raw/books/linear-system-theory-design.md, raw/books/signals-and-systems-oppenheim.md]
confidence: high
---
# Linear System, Control & State-Space

**1개의 선형 다변수 동역학 시스템의 "내부 구조(상태공간) → 외부 입력-출력 관계"를 행렬로 서술하고, 안정을 판별하고, 피드백으로 원하는 동역학을 설계하는** 개념. 클러스터 2권이 이 축을 다름:

- **[[linear-system-theory-design]] (Chen, Stony Brook)** — 이 개념의 **전체**: 제2장(선형대수: 행렬·Jordan·행렬함수)→제3장(2묘사: 입력-출력/상태변수)→장5(제어가능·관측가능)→장6(불가전 실현·식별)→장7(상태피드백·추정기·**분기 원리**)→장8(안정)→장9(합성시스템·해제·점근추적) `[raw/books/linear-system-theory-design.md]`
- **[[signals-and-systems-oppenheim]] (Oppenheim·Willsky, MIT)** — 이 개념의 **학부 진입점**: 제11장 선형피드백시스템(궤적 p.700, **Nyquist 안정성 p.713**, 증폭도/위상 마진) `[raw/books/signals-and-systems-oppenheim.md]`]`

## 2권 비교

| 항목 | Chen (대학원) | Oppenheim·Willsky (학부) |
|---|---|---|
| **관점** | **내부 구조**: 상태공간 ẋ=Ax+Bu, y=Cx+Du + 제어로 **구조 설계** | **외부 관계**: 컨벌루션·전달함수·주파수응답 + 제어로 **안정성** |
| **선급** | 선형대수(행렬·공간 기하) + ODE | 미적분·푸리에 + ODE(1~2계) |
| **제어 가능성** | 제5장 **필수**: 제어가능성(p.175)·관측가능성(p.192)·**분기 분해** | 서론 수준 — 전달함수 + 주파수응답 중심 |
| **안정 판별** | Routh-Hurwitz(장8-3)·**Lyapunov**(장8-5)·Lyapunov 방법론 | **Nyquist**(장11)·궤적·증폭도/위상 마진 |
| **합성시스템** | 장9: 병렬·직렬·피드백 합성의 완전 특성(제어/관측/안정) | 장3·장11: 블록다이어그램 + 단일루프 |
| **제어기 설계** | **장7**: 상태피드백(고유치 할당 p.351) + **분기 원리** + 추정기(전차원/감소차) → **장9**: 단일피드백 보상기(고분모행렬 할당 p.468) | 장11: 궤적/Nyquist으로 **안정 + 마진 확보** |
| **최적추정** | 옵티멀 추정(장26 Kalman-Bucy)·EKF가 [[estimation-and-filtering]]로 넘어감 | 없음 — **랜덤 세계에 비** (확률 축은 이 클러스터 외부) |

## "2권 사이에 놓인 다리"
학부(Oppenheim)의 "주파수응답 + 안정 마진"과 대학원(Chen)의 "상태공간 + 고유치 할당"은 **같은 시스템의 두 묘사**(Chen 장3-6 비교: 두 묘사의 관계). Nyquist가 **주파수 영역** 안정판별이라면, Routh-Hurwitz·Lyapunov가 **극점·시간 영역으로**, 궤적이 **개폐루프 극점 이동**으로 — 3 판정의 **동일성**이 이 개념의 핵심 통합점.

**분기 원리(Chen 장7-5, p.355~361 전후)**는 제어·추정의 분리를 법칙화:
> "제어기가 (A, B)의 제어로 관측가능성을 보존한다면, 추정기가 (A, C)의 관측가능성을 보존하는 한, 두 가지를 **독립 설계**해도 합쳐서 안정이 성립" — 이 원리가 [[estimation-and-filtering]]의 Kalman(Bu)가 Chen 세계로 **상태 공간 내 추정기**로 재진입하는 통로.

## 상태공간 6장 구조 (Chen 기준)
```
장2 선형대수(Jordan/행렬함수)  →  장3 2묘사(I/O vs state)
        ↓
장4 동역학방정식·해   →  장5 제어·관측가능(필수)·분기 분해
        ↓
장6 불가전 실현·식별  →  장7 상태피드백·추정기·분기 원리
        ↓
장8 안정(R-H/Lyapunov)  →  장9 합성시스템·해제·점근추적
```
Oppenheim 장11(궤적/Nyquist)은 **장8(안정)의 주파수판도**로, Chen **장7(추정기)**은 **랜덤 세계**([[estimation-and-filtering]])로부터 오는 입력.

## 인접
- [[estimation-and-filtering]] — 옵티멀 추정·Kalman · **분기 원리**가 이 개념과 이어지는 접점
- [[stochastic-processes-cluster]] — 란덤 입력의 선형시스템 통과(장장)
- **미분방정식(다른 클러스터)** — ODE 선급(Chen 서문 "Elementary ODE"+행렬 조작)·Lyapunov. 텍스트로만 언급, 위키링크는 하지 않음(다른 클러스터 소유)
- [[linear-algebra-and-its-applications]] (Strang) — 선급 선형대수의 **학부** 버전; Chen 장2는 그 **이론/응용** 축
- [[signals-and-systems-korea]] (한국어 교재) — 학부 신호-시스템(제11장 피드백까지)의 한국어 대응
