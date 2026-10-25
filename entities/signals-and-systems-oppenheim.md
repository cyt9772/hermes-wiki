---
title: Signals and Systems (2nd ed)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, fourier-analysis, engineering-mathematics]
sources: [raw/books/signals-and-systems-oppenheim.md]
confidence: high
---
# Signals and Systems (2nd ed)

> A. V. Oppenheim · A. Willsky, Prentice Hall, 810p — SIGNAL PROCESSING SERIES(Oppenheim 편집) 계열. MIT EECS학과 첫 신호-시스템 교과 강연 노트를 기반으로 한 학부 표준 교과서 `[raw/books/signals-and-systems-oppenheim.md]`.

## 개요
연속시간(CT)·이산시간(DT)을 **나란히(parallel) 발전**시키는 것이 조직 원리. 서문은 "최근 기술 발전으로 CT/DT 양쪽 기술에 대한 동등한 숙달이 급증했다"며, 분석 도구(컨벌루션→푸리에→Laplace/z)마다 CT·DT 쌍장을 두고 유사성으로 직관을 공유하고 차이로 개별 성질을 선명하게 한다. 미적분 + 복소수 다루기 + 미분방정식 경력이 있으면 자립적(노컨베션·푸리에·변환 사전 지식 불요). 장말 문제 350여 개를 "숙달은 연습 없이는 불가"라는 신념으로 수록 `[raw/books/signals-and-systems-oppenheim.md]`.

## 장 구조 (원문 TOC 기준, 11장 + 부록)
1. **Introduction** (p.1) — 동기와 관점
2. **Signals and Systems** (p.7) — 독립변수 변형(시프트·확대), 기본 CT/DT 신호(복소지수·스텝·임펄스), 시스템 성질(인과성·선형성·시불변성), 블록다이어그램
3. **LTI Systems** (p.69) — 신호의 임펄스 분해, DT 컨벌루션 합(p.75) → CT 컨벌루션 적분(p.88), 미분/차분방정식 LTI, 블록다이어그램, 특이함수
4. **CT Fourier 분석** (p.161) — 복소지수 입력 응답, CT 푸리에급수, 수렴, CTFT, 주기신호와 CTFT, 성질표, 컨벌루션·변조 성질, 1/2계 시스템 주파수응답(p.240)
5. **DT Fourier 분석** (p.291) — DT 푸리에급수·DTFT, 듀얼리티(p.336), 차분방정식 주파수응답, 1/2계 시스템
6. **Filtering** (p.397) — 이상/비이상 주파수선형, BT/DT 미분·차분방정식 필터, **Butterworth** 부류(p.422)
7. **Modulation** (p.447) — AM·SSB·PAM/TDM, DT 변조, FM
8. **Sampling** (p.513) — 샘플링 정리(p.514), 내삽 재생, 별리어싱, DT 처리, 주파수역 샘플링, 디시메이션/인터포레이션
9. **Laplace Transform** (p.573) — ROC, 역변환, 극-제로 기하평가, ROC 포함 단사/양변 ROC
10. **z-Transform** (p.629) — ROC, CT↔DT 시스템 변환(p.658), 양변 z
11. **Linear Feedback Systems** (p.685) — 궤적(root locus, p.700), **Nyquist 안정성**(p.713), 이득/상 여준
+ 부록 A: 부분 분수 전개(CT/DT), 참고문헌, 주제색인. 문제집 350+ `[raw/books/signals-and-systems-oppenheim.md]`

## 핵심
- **DT에서 CT로 유도**하는 순서 — 컨벌루션 합(이산)을 직관으로 먼저 세우고 적분으로 확장. 서문이 명시한 교수법 `[raw/books/signals-and-systems-oppenheim.md]`
- 필터·변조·샘플링·피드백은 "기본 기법의 중요 용도"로 **입문 수준 소개**로 편성 — 심화 응용(DSP·통신)은 계열서로. 제8장 샘플링(별리어싱 p.527)이 CT↔DT 다리의 실용 지점 `[raw/books/signals-and-systems-oppenheim.md]`
- 제11장 피드백(궤적·Nyquist)이 신호-시스템 교과에서 [[linear-system-control]] 쪽으로 넘어드는 접점 — Nyquist 판정(p.713)까지 포함 `[raw/books/signals-and-systems-oppenheim.md]`
- CT/DT 쌍장 구조(4/5, 9/10)가 [[digital-signal-processing]]의 "연속 이론 → 이산 구현" 흐름의 학부 버전. 한국 교재 [[signals-and-systems-korea]]도 같은 이원 배치이나 이 장(11장)까지 넓힘

## Related
- 저자: [[alan-v-oppenheim]] · [[alan-willsky]] (MIT 듀오)
- 개념: [[digital-signal-processing]] · [[linear-system-control]]
- 인접: [[signals-and-systems-korea]] (한국어 신호-시스템 교재) · [[a-course-in-dsp]] (DSP 후속) · [[analog-filter-design]] (Butterworth 장 접점)
- **해답집**: [[oppenheim-signals-systems-solutions]] — Solution Book (Prentice Hall, 1st ed. 1982, 177p), 장말 문제 풀이(CT/DT 컨벌루션·FT·Laplace·z·피드백)
