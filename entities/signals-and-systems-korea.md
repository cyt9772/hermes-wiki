---
title: 신호 및 시스템
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, signal-processing, fourier-analysis, dsp]
sources: [raw/books/signals-and-systems-korea.md]
confidence: medium
---
# 신호 및 시스템 (1992)

> 표지/원저: 저자 미상 — 원문 표지 "공저" 표기, 개별 인물명 OCR 왜곡(확인 필요). 중앙대 전기공학·제어계측공학과 관련.
> 출판: (출판사 원문 미확인 — 발문에 "희중당 관계자" 감사 인사 있음), 1992. 5. 발문, 264p

## 개요
전기·전자계 3·4학년 대상 "신호 및 시스템" 교과서. 연속/이산시간을 **반대(나란히) 배치**해서 동일 맥락에서 다루는 것(서문 기본목표 2)이 최대 특징 — 기본 신호·LTI 시스템(제1장) → 연속시간 푸리에급수/변환(제2장) → 이산시간 푸리에해석·DFT·**FFT** (제3장) → z-변환(제4장) → 샘플링·재생·A/D·D/A(제5장) → 연속↔이산 등가시스템·스타변환(제6장) → **LTI 상태공간** (제7장)으로 7장 구성 `[raw/books/signals-and-systems-korea.md]`. "희로이론" 수준의 회로·Fourier급수·Laplace 기본이 선진으로 요구된다.

## 장 구조 (7장 + 부록 A-D, 264p)
1. **신호 및 시스템** — 연속/이산 기본신호, LTI(선형성·시불변성·인과성·안정성·임펄스응답), 미분/차분방정식, 디콘벌루션·상관
2. **연속시간 푸리에급수 및 푸리에변환** — 주기/비주기함수, CtFT 여와 특성, 극좌표 표현
3. **이산시간 신호 및 시스템의 푸리에해석** — DtFT·성질, DFT(정의·특성·선형컨벌루션 활용), **FFT**, DtFT-DFT 관계
4. **z-변환** (원문 TOC에서 4장 장제목 1글자 깨짐 — z-변환으로 판독) — 정의· 특성· 역변환· LTI 해석· 기하학적 평가· 극점/제로
5. **샘플링과 재생** — D/A·A/D 변환, sampling·reconstruction·내삽, sample-and-hold
6. **연속시간시스템과 이산시간시스템** — 이산등가시스템, 입력불변 등가변환, 스타변환/펄스전달함수, s↔z 극점 대응
7. **LTI 시스템의 상태공간표현** — 상태방정식/출력식, 해, 전달함수/특성방정식, 연속→이산, 유사변환
+ 부록 A-D: 인과 LTI 극점 안정도기준, 변환 표, 유용한 공식, **컴퓨터 프로그램**

## 핵심 내용
- 신호·시스템 **이론 교과서** — DSP 응용(디지털 필터 설계·멀티레이트·랜덤 신호 등)은 다루지 않고 수학적 해석 중심으로 편성 `[raw/books/signals-and-systems-korea.md]`
- 연속↔이산 이중 구조가 제2장(연속 FT) / 제3장(DtFT·DFT·FFT) / 제6장(등가시스템)까지 일관되며 "FFT는 이산시간 장(제3장)에서 다루는" 한국식 편성 `[raw/books/signals-and-systems-korea.md]`
- 상태공간(제7장)까지 포함해 제어이론 접점을 포함 — DSP 교과서(Porat)보다 범위가 좁고 수학적
- 부록에 "컴퓨터 프로그램" 수록(원문 OCR: "컴퓨터 프로그램 256")
- 저자·출판사 원문 확인 필요 → 엔티티 confidence: medium

## Related
- 개념: [[digital-signal-processing]] — 신호·시스템 → DSP 이론 클러스터
- 인접: [[a-course-in-dsp]] (Porat 1997, 동일한 신호-시스템 → DSP 흐름을 영어로 다룸)
- 인접: [[linear-algebra-applications]] (선형대수 기반), [[analog-filter-design]] (analog 쪽 접점)
