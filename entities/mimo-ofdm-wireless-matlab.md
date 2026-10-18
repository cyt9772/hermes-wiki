---
title: MIMO-OFDM 무선통신과 MATLAB (MIMO-OFDM Wireless Communications with MATLAB)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, wireless-communications, ofdm, mimo, channel-modeling, space-time-coding, matlab-simulation]
sources: [raw/books/mimo-ofdm-wireless-matlab.md]
confidence: high
---
# MIMO-OFDM 무선통신과 MATLAB

> "MIMO-OFDM Wireless Communications with MATLAB" (표지)
> 저자: 조융수 · 김재권 · 양원영 공저
> 출판: 홍릉과학출판사, 2008 (Copyright © 2008), 728p 한국 집필 원서 (번역이 아님)

## 개요
3G 이후(IMT-2000 / IMT-Advanced) **무선 광대역 멀티미디어 통신**에서 핵심 기술인 **MIMO·OFDM**을 MATLAB 기반으로 다루는 실무 교재. "3 세대 이후(IMT-2000) … 1Gbps(nomadic)·100Mbps(고속 이동)" 목표를 달성하기 위해, 다중경로 영향으로 인한 에러율을 잡는 **무선접속방식**으로서 OFDM을 택하고, 이를 MIMO와 결합하는 전체 파이프라인(채널모델→OFDM→동기화→채널추정→PAPR→간섭제거→용량)을 이론+MATLAB 실행으로 다룬다 `[raw/books/mimo-ofdm-wireless-matlab.md]` p.3.

## 장 구조 (TOC 기반, 728p)
1. **서론** — 3G/초3G/4G 시대, IMT-2000·IMT-Advanced 용량 목표, OFDM 기본 원리 (pp. ~1-65)
2. **SISO 채널 모델링** — Rayleigh·Rician 페이딩, 옥내/옥외 채널 모델링 (p.66~)
3. **MIMO 채널 모델링** — I-METRA, SCM, SCM-E, IEEE 802.11 TGn (pp. ~120-155)
4. **OFDM** — 단일/다중 반송파, 기본 원리, 보호 대역, Coded OFDM, **OFDMA**(다중접속), 자원 할당, Duplexing (pp. ~157-210)
5. **OFDM 동기화** — 심볼 타이밍·반송파 주파수·샘플링 클럭 옵셋의 영향과 추정 기법, 셀룰러 동기화 (pp. ~214-248)
6. **채널 추정** — 구조(Comb/Pi), 훈련 신호 기반, 보간, Decision-directed, DFT, Blind, EM, 고속 이동 시 추정 (pp. ~249-290)
7. **PAPR** — 개요, PAPR 감쇄 기법 (pp. ~289-340)
8. **셀간 간섭** — 조정/공존/제거/랜덤화 (pp. ~341-360)
9. **MIMO 채널 용량** — 행렬 이론, Deterministic MIMO 채널 용량 (pp. ~362-?)
10. **MATLAB** — 시뮬레이션 통합 (pp. ~?-728)

## 핵심 기여 / 학습 포인트
- **MIMO 채널 모델링의 표준 4종**을 한 장(제3장)에 비교: I-METRA(실외 셀룰러), SCM(3GPP), SCM-E(확장), IEEE 802.11 TGn(무선 LAN)
- **OFDM 전체 파이프라인**을 파고드는 깊이: 동기화(제5장)와 채널추정(제6장)가 별도 장으로 분리 — 실무에서 가장 어려운 2 영역
- **PAPR 감쇄(제7장) + 셀간 간섭(제8장)** — 광대역 셀룰러 OFDM 실전 문제 2종
- 각 장에 MATLAB 시뮬레이션 코드 동봉 (MATLAB/Simulink, The MathWorks)

## OCR 신뢰도
- **주요 주의**: scan-only PDF → tesseract 300dpi re-OCR. OFDM 심볼 간섭/채널 추정/용량 공식의 수식이 심하게 깨짐 (예: "10054668" = 100 Mbps)
- **MATLAB 코드** — 변수명/함수명은 대개 잘 OCR됨, 그러나 `fft`/`ifft` 식과 인덱싱은 원본 PDF 대조 필요
- **활용법**: 개념 구조 이해용으론 충분. 수식·코드 재사용 시 원본 PDF 대조 필수

## Related
- 저자: [[jo-yong-soo]], [[kim-jae-gwon]], [[yang-won-yeong]]
- 개념: [[ofdm-orthogonal-frequency-division]], [[mimo-multiple-input-multiple-output]], [[wireless-channel-modeling]], [[space-time-coding]]
- 관련 책(같은 분야, 다른 저자): [[latest-mobile-comm-systems]] — Harada·Prasad 원저(2002, 이동통신 전반). 이 책은 **MIMO·OFDM에 특화**된 한국 집필서.
