---
title: 디지털 신호 처리 (Digital Signal Processing)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, signal-processing, dsp, dft-fft, fourier-analysis]
sources: [raw/books/a-course-in-dsp.md, raw/books/signals-and-systems-korea.md]
confidence: high
---
# 디지털 신호 처리 (Digital Signal Processing)

연속/이산 신호를 **이산 시간·유한 정밀도**(샘플링 + 양자화)로 변환하고, LTI 모델·푸리에/z-변환·DFT/FFT·디지탈 필터 설계로 분석·합성하는 공학 분야. 이 클러스터에서는 한국 신호-시스템 교재(이론 편성)와 Porat DSP 교과서(설계·응용 편성) 두 관점이 만난다.

## Porat — A Course in Digital Signal Processing (1997)
- DSP 교육은 "signals and systems" 과목이 끝나는 지점(컨벌루션, 변환, 주파수응답, 안정성)에서 시작 — 제2장이 그 복습 `[raw/books/a-course-in-dsp.md]`
- 샘플링/재생(제3장) → **DFT** (제4장, DCT/DST 포함) → **FFT**(Cooley-Tukey, 제5장) → 스펙트럼 분석(제6장) → z-변환(제7장) → **IIR/FIR 필터** 설계(제8-11장) → **멀티레이트**(제12장) → 랜덤 신호·응용(제13-14장) `[raw/books/a-course-in-dsp.md]`
- FIR 설계: IRT·창법·least-squares·**equiripple(Remez)** — 위상선형성(GLP Type I-IV) 제약과 함께 `[raw/books/a-course-in-dsp.md]`
- 응용 범위: 음성(노이즈 필터링·부호화·인식·합성), 레이다/소나(도파도 추정·이미징), 전화(모뎀·셀룰러) `[raw/books/a-course-in-dsp.md]`

## 신호 및 시스템 (1992, 한국 교재)
- 연속/이산 신호와 LTI를 **같은 맥락**에서 해석하는 통일된 시각을 목표로 하되, **DSP 설계까지 확장하지 않는 이론서** — 기본신호·LTI(제1장) → 연속 푸리에급수/변환(제2장) → DtFT·DFT·**FFT**(제3장) → z-변환(제4장) → 샘플링·재생(제5장) → 연속↔이산 등가시스템·스타변환(제6장) → LTI 상태공간(제7장) `[raw/books/signals-and-systems-korea.md]`
- 선진 요구: 회로, Fourier 급수, **Laplace 변환** 기본개념 `[raw/books/signals-and-systems-korea.md]`
- 부록에 "컴퓨터 프로그램" 수록 — 시뮬레이션 기반 학습 `[raw/books/signals-and-systems-korea.md]`

## 두 소스 비교

| 차원 | 신호 및 시스템 (1992) | Porat (1997) |
|---|---|---|
| 범위 | 신호-시스템 이론 (7장, 264p) | DSP 전역 (14장, 630p) |
| FFT | 이산시간 장(제3장)에서 산출 | 독립 장(제5장) + 스펙트럼 분석 |
| 필터 | — (상태까지만) | FIR/IIR 설계·구현 (제8-11장) |
| 추가 | 상태공간·스타변환 | 멀티레이트·랜덤 신호·응용 |

## 관련
- [[a-course-in-dsp]] · [[signals-and-systems-korea]]
- [[dct-algorithms-applications]] (DCT/변환 부호화 → [[transform-coding]])
- [[linear-algebra-applications]] (FFT·SVD의 선형대수 기초)
- 인접: [[analog-filter-design]], [[ofdm-orthogonal-frequency-division]], [[spread-spectrum-cdma]]
