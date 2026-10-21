---
title: 라플라스 변환 기반 회로 해석 (Laplace Transform Circuits)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/circuits-and-systems.md, raw/books/nilson-riedel-electric-circuits.md]
confidence: medium
---
# 라플라스 변환 기반 회로 해석

## 정의
**미분방정식으로 기술되는 회로를 복소 주파수(s) 영역에서 대수방정식으로 변환해 해석**하는 방법. 라플라스 변환 → s 영역에서 부분분수 전개로 역변환 → 시간 영역 응답. 회로의 동적 특성(과도응답, 진동, 안정성)을 특성근(극)의 위치로 파악할 수 있다는 것이 핵심가치.

## 핵심 구조 (회로 및 시스템 중심)

### 1. 라플라스 변환과 기본정리
- 라플라스 변환: f(t) → F(s)=∫₀^∞ f(t)e^(-st)dt — 미분 ↔ s·F(s) − 초기값. `[raw/books/circuits-and-systems.md]`
- **기본정리(8.3)**: 평탄성·스케일링·시간이동·s역 이동. `[raw/books/circuits-and-systems.md]`
- **초깃값·최종값 정리(9.4)**: F(s)에서 t=0⁺와 t→∞ 값을 역변환 없이 직접. `[raw/books/circuits-and-systems.md]`
- **부분분수 전개(8.5)**: 역변환을 위한 주 실무 기법. `[raw/books/circuits-and-systems.md]`
- **Heaviside 전개정리(8.6)**: 극이 중근일 때의 전개 확장. `[raw/books/circuits-and-systems.md]`

### 2. S-평면과 특성근
- 회로방정식(미분방정식)의 **특성방정식 Q(s)=0의 근 = 극**. `[raw/books/circuits-and-systems.md]`
- **근의 위치 → 시간 응답 대응**(7.4):
  - 좌반면(real<0) → 수렴(감쇠) 응답
  - 우반면(real>0) → 발산(발진 증폭)
  - 실축( Imag=0) → 비감쇠 정현파
  - conjugate pair → 잔상 응답
- **1계(시간상수)**: 단일 실근 → 지수감쇠. `[raw/books/circuits-and-systems.md]`
- **2계**: 판별식 D=b²−4ac — D>0(비잔상), D=0(임계잔상), D<0(잔상). `[raw/books/theory-of-circuits.md]`

### 3. 상태방정식 (상대방정식)
- **상태공간 표현**: n계 회로를 1계 연립 방정식 ẋ=Ax+Bu, y=Cx+Du로. `[raw/books/circuits-and-systems.md]`
- **Cayley-Hamilton 정리(10.6)**: 특성방정식을 행렬 자체에 대입 → 고차 역전렬식 불필요. `[raw/books/circuits-and-systems.md]`
- **특성방정식·특성벡터(10.5)**: 극과 영점의 행렬 대수적 해석.
- **해석법**: 시간영역 해석(10.7) + 라플라스 해석(10.9) 병행. `[raw/books/circuits-and-systems.md]`

### 4. 극과 영점
- **극(pole)**: F(s)의 분모가 0이 되는 s 값 — 시스템 동역학. `[raw/books/circuits-and-systems.md]`
- **영점(zero)**: F(s)의 분자가 0이 되는 s 값 — 입력 전달 억제.
- **극-영점 분포 → 시간영역 응답**(12.7): 극만으로는 결정 불가, 영점 위치에 따라 잔상 진폭이 달라짐. `[raw/books/circuits-and-systems.md]`
- **안정성(12.8)**: 모두 극이 좌반면에 있으면 안정. 능동회로는 우반면 극 가능(이득>1 발진). `[raw/books/circuits-and-systems.md]`
- **Routh-Hurwitz 판정법**(12장 인용): 극 위치를 직접 구하지 않고 안정성 판별.

### 5. 신호변환
- **단위계단·램프·임펄스**(9.1–9.2): 기본 파형의 라플라스 변환. `[raw/books/circuits-and-systems.md]`
- **중첩적분(9.5–9.7)**: 임의 입력을 임펄스 응답 적분으로 — LTI 회로의 완전 기술. `[raw/books/circuits-and-systems.md]`

### 6. 전이함수
- **정의**: 출력 라플라스 / 입력 라플라스 (초깃값 0 가정). `^[raw/books/theory-of-circuits.md]`
- **용도**: 파형 무관한 회로 특성 — 주파수응답·안정성·극-영점의 출발점. `^[raw/books/theory-of-circuits.md]` `^[raw/books/circuits-and-systems.md]`
- **2단자 파라미터(13장)**: 전이함수의 확장 — Z/Y/H/ABCD 파라미터. `^[raw/books/circuits-and-systems.md]`

## 관련 개념
- [[dc-ac-circuit-analysis]] — 라플라스는 DC·AC 시간영역 해석의 수학적 일반화
- [[digital-logic-basics]] — 디지털 회로 해석으로의 확장(20장 z-변환)
- [[analog-filter-design]] — 주파수응답 기반 필터 설계
- [[semiconductor-devices]] — 라플라스 적용 범위(수동 소자 vs 비선형 소자)

## 출처
- `raw/books/circuits-and-systems.md` — 7~12장(라플라스, 상태방정식, 극-영점)
- `raw/books/theory-of-circuits.md` — 16장(라플라스 변환), 17장(전달함수)
