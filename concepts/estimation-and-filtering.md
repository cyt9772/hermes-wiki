---
title: Estimation and Filtering (추정·필터링)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [concept, estimation-filtering, signal-processing]
sources: [raw/books/estimation-theory.md, raw/books/discrete-random-signals.md, raw/books/linear-system-theory-design.md]
confidence: high
---
# Estimation & Filtering — 추정과 필터링

**모수가 숨어 있고, 그 모수를 관측에서 "최적"으로 추측하는 수학**을 4개 프레임(최소제곱·최대우도·가우스·Kalman)으로 묶은 개념. 클러스터 6권 가운데 **핵심 실체**: 3권이 다른 위치에서 이 주제를 다룸 — Mendel은 체계, Therrien은 알고리즘, Chen은 구조(제어가능성·관측가능성·분리 원리)이다.

## 4 프레임 비교

| 프레임 | 목적함수/원리 | 선급 | 대표 |
|---|---|---|---|
| **최소제곱 LS** | $\sum \lVert y_i - Hx \rVert^2$ 최소 | 선형 공간·행렬 (SVD) | Mendel 레슨 3~5, BLUE(9) / Therrien 장6 장9 / Chen 장7 |
| **최대우도 ML** | $\arg\max L(\theta\vert y)$ — 노이즈 밀도에서 유도 | 미적분·적분 | Mendel 레슨 10~11 / Therrien 장6.2 / Papoulis 장3 |
| **가우시안 + 베이스 MAP** | $p(x\vert y) \propto p(y\vert x)p(x)$ — 로그우도 = 이차형 + 선형형 | 가우시안 분포·조건밀도 | Mendel 레슨 12~14 / Therrien 장6.3 |
| **Kalman 필터** | **시간순** 상태 추정 — 예측(레슨16)·필터(17-18)·스무딩(20-21) | 상태공간·가우시안·시간순추론 | Mendel 레슨 15~21(26) / Therrien 장7 / Chen 장7 추정기 |

핵심 등가: **"가우시안 세계에서는 LS = ML = MAP"** — Mendel 26레슨의 줄거리가 바로 이 등가를 세 축(레슨3~5→레슨11→레슨14→레슨17)으로 증명하는 흐름 `[raw/books/estimation-theory.md]`. Therrien은 같은 내용을 **알고리즘**으로 전환: 직교원리→FIR→Levinson(LPC)→IIR/최소위상→Wold→Schur→AR/ARMA(Yule-Walker) `[raw/books/discrete-random-signals.md]`.

## 3권의 각도
- **[[estimation-theory]] (Mendel)** — 레슨2(모델)→LS→성질(소표본·대표본)→ML→베이스→**상태 추정 3단계**→비선형. "왜 LS·ML·Kalman이 같은 답을 주는가"가 전체. 소표본(무편향·효율)과 대표본(asymptotic) 성질을 레슨 6~8에서 분리 `[raw/books/estimation-theory.md]`
- **[[discrete-random-signals]] (Therrien)** — 장6~7(베이즈·LSMSE·최적 FIR/IIR)과 장8(Levinson·Schur·격자)·장9(AR/ARMA·Yule-Walker)·장10(최대우도·**서브스페이스법** 스펙트럼 추정)을 **알고리즘 군**으로 배열. "추정 = 예측 = 필터링 = 스펙트럼 추정"이 같은 직교원리에서 도출 `[raw/books/discrete-random-signals.md]`
- **[[linear-system-theory-design]] (Chen)** — 장7 "상태피트백과 상태 추정기". **분리 원리(7-5)**가 "제어기·추정기를 독립 설계해도 합쳐서 안정"의 근거 — 추정기가 **시스템 내부 컴포넌트**로 진입하는 접점. 옵티멀 추정은 부록/별표로 남고, **제어가능성·관측가능성(장5)이 추정기 존재성의 선진 조건** `[raw/books/linear-system-theory-design.md]`

## 개념 지도
```
관측 y = Hx + v
        │
   ┌────┴────┬─────────────┬─────────────┐
   │LS(이차형)│  ML(우도)   │  MAP(베이스) │ Kalman(시간순)
   │  BLUE   │  MLE       │  가우시안    │  예측·필터·스무딩
   └────┬────┴─────┬───────┴──────┬───────┘
        └──────────┴──────┬───────┘
                          │ 가우시안·선형
                     "동일 해"
        │
        ├─→ 제어 영역: 분리 원리(Chen 장7) → 옵티멀 LQR/LQE
        └─→ 비선형: EKF(Mendel 24)·Iterated LS
```

## 인접
- [[stochastic-processes-cluster]] — 확률적 선급(가우시안 프로세스·특성함수·PSD)
- [[linear-system-control]] — 상태공간·분기 원리·제어가능성
- [[information-coding-theory]] — 추정↔코딩 대칭 (추정정보 vs 코딩정리)
- [[cdma-dss-spread-spectrum]] — **매칭 필터**(Therrien 장5.8, p.239)가 최적 수신기 = LS/MAP 추정관점에서의 첫 실용
