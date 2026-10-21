---
title: DC/AC 회로 해석 공통 코어 (DC/AC Circuit Analysis)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [electrical-engineering, electronic-circuits]
sources: [raw/books/electronics-basics.md, raw/books/theory-of-circuits.md, raw/books/circuits-and-systems.md]
confidence: high
---
# DC/AC 회로 해석 공통 코어

## 정의
**DC와 AC 회로 해석을 관통하는 기본 정리와 도구의 체계**. 3권 공통: (1) 직렬·병렬 소자 합성, (2) 키르히호프 법칙, (3) 중첩의 원리, (4) Thévenin/Norton 등가, (5) RLC 소자의 임피던스, (6) 공진·주파수 응답. AC 해석은 DC 법칙에 +리액턴스/복소수를 얹은 일반화.

## 공통 코어 구조

### 1. 직렬·병렬 합성 (DC·AC 공통)
- **저항**: 직렬 합성 R=R₁+R₂+…; 병렬 합성 1/R=1/R₁+1/R₂+… `^[raw/books/electronics-basics.md]`
- **인덕턴스**: 직렬 합성 L=L₁+L₂+…; 병렬 합성 1/L=1/L₁+1/L₂+… `^[raw/books/electronics-basics.md]`
- **캐파시턴스**: 직렬 합성 1/C=1/C₁+1/C₂+…; 병렬 합성 C=C₁+C₂+… `^[raw/books/electronics-basics.md]`
- **임피던스 (AC)**: 직렬 Z=Z₁+Z₂+…; 병렬 1/Z=1/Z₁+1/Z₂+… — DC의 R에 +jX를 얹은 것. `^[raw/books/electronics-basics.md]`

### 2. 키르히호프 법칙
- **전류법칙 (KCL)**: 분기점에서 유입 전류의 합 = 유출 전류의 합. `^[raw/books/electronics-basics.md]` `^[raw/books/circuits-and-systems.md]`
- **전압법칙 (KVL)**: 폐루프에서 전압강하의 합 = 전압원의 합. `^[raw/books/electronics-basics.md]` `^[raw/books/circuits-and-systems.md]`
- **용도**: 루프전류법·마디전압법·망전류법의 기본 전제. `^[raw/books/electronics-basics.md]`
- **회로망 이론(10장)**: 중첩·테브난·노턴·밀만 법칙까지 KCL/KVL의 체계적 전개. `^[raw/books/electronics-basics.md]`

### 3. 중첩의 원리
- **DC**: 각 전원이 독립적으로 기여하는 전압/전류의 합. `^[raw/books/electronics-basics.md]`
- **AC**: 복소수(phasor) 영역에서 같은 원리 적용. `^[raw/books/electronics-basics.md]` `^[raw/books/circuits-and-systems.md]`
- **한계**: 비선형 소자(다이오드·트랜지스터)에는 적용 불가. `^[raw/books/electronics-basics.md]`

### 4. Thévenin·Norton 등가
- **Thévenin**: 비정전 회로 → 전압원 V_th + 직렬 저항 R_th. `^[raw/books/electronics-basics.md]` `^[raw/books/circuits-and-systems.md]`
- **Norton**: 동일 회로 → 전류원 I_n + 병렬 저항 R_n. V_th=I_n·R_th. `^[raw/books/electronics-basics.md]`
- **밀만 법칙**: 멀티분지 분기점에서 특정 분지 전류/전압을 한 번에. `^[raw/books/electronics-basics.md]`
- **AC 확장**: 임피던스 Z_th로 교체. `^[raw/books/electronics-basics.md]` `^[raw/books/circuits-and-systems.md]`

### 5. RLC 소자 + 임피던스
- **저항 R**: 전압·전류 동위상. P=VI. `^[raw/books/electronics-basics.md]`
- **인덕턴스 L**: 전류가 전압보다 90° 지체. X_L=2πfL. `^[raw/books/electronics-basics.md]`
- **캐파시턴스 C**: 전압이 전류보다 90° 지체. X_C=1/(2πfC). `^[raw/books/electronics-basics.md]`
- **임피던스 Z**: Z=R+j(X_L−X_C), |Z|=√(R²+(X_L−X_C)²). `^[raw/books/electronics-basics.md]` `^[raw/books/theory-of-circuits.md]`
- **회로이론(자격)**: 같은 RLC를 기사 시험 범위에서 임피던스·전력인자·공진으로 다루어 `^[raw/books/theory-of-circuits.md]`

### 6. 공진·주파수 응답
- **직렬 공진**: X_L=X_C, f₀=1/(2π√LC), 임피던스 최소화. `^[raw/books/electronics-basics.md]` `^[raw/books/theory-of-circuits.md]`
- **병렬 공진**: 임피던스 극대화. `^[raw/books/electronics-basics.md]`
- **Q(선택비)**: Q=ω₀L/R (직렬), 대역폭 BW=f₀/Q. `^[raw/books/electronics-basics.md]`
- **주파수응답**: 주파수 f에 따른 |Z(f)|·∠Z(f) 곡선 → 보트 그림으로 표현. `^[raw/books/circuits-and-systems.md]`

## 관련 개념
- [[laplace-transform-circuits]] — 라플라스 변형으로 위 시간영역 분석을 수학적 체계화
- [[analog-filter-design]] — 공진(RLC)을 필터 설계로 확장
- [[semiconductor-devices]] — 비선형 소자 트랜지스터 회로 (중첩 원리의 한계)
- [[digital-logic-basics]] — 디지털 논리 (회로 해석 적용 범위)

## 출처
- `raw/books/electronics-basics.md` — 1~26장 (DC·AC 회로 해석 전 과정)
- `raw/books/theory-of-circuits.md` — 1~4장 (직류·정현파·RLC), 16–17장 (라플라스·전달함수)
- `raw/books/circuits-and-systems.md` — 3장(회로방정식), 11장(임피던스함수), 14장(정상상태), 15장(주파수응답)
