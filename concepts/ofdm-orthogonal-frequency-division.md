---
title: OFDM — 직교 주파수 분할 다중화
created: 2026-10-18
updated: 2026-10-31
type: concept
tags: [wireless-communications, ofdm, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md, raw/books/digital-communication-matlab.md, raw/books/proakis-communications-systems.md, raw/books/h264-avc-video-compression.md, raw/books/hdtv-theory-technology.md]
confidence: high
---
# OFDM (Orthogonal Frequency Division Multiplexing)

**직교 주파수 분할 다중화**(OFDM): 하나의 고속 기저대역 데이터를 N개의 저속 서브캐리어로 나눠 송신. 직교성을 이용해 간섭 없이 동시에 전송하고, 다중경로·주파수 선택적 페이딩에 강하다.

## 원리
- 각 서브캐리어는 주기적 직교(orthogonal) → 간섭 없이 동시에 전송
- IFFT/FFT로 기저대역↔주파수 영 변환
- **Cyclic Prefix (CP)**: 다중경로 지연 전이 분산(T_s) → CP 길이 → ISI(심볼 간 간섭) 제거
- 채널 평탄화 (flat fading per subcarrier) → 단일-계수 등화(1-tap per subcarrier)

## 이 책의 OFDM 관련
- [[mimo-ofdm-wireless-matlab]] — OFDM + MIMO (제1~17장, UWB MB-OFDM 포함)
- [[latest-mobile-comm-systems]] — "10.7 MHz 고속 데이터", 3G 5.8GHz, 빔포밍 결합 (TOC p.10)

## OFDM·채널 코딩 실습 축 (2005~2009 배치 추가)
- **디지털통신과 MATLAB/SIMULINK (양원영 외 2005, 홍릉, 430p)** — 변조(QPSK/QAM)·채널 코딩·FEC·등화·OFDM MATLAB/SIMULINK 시뮬레이션; 이론서(Taub·Stremler) 대비 실용 축 `[raw/books/digital-communication-matlab.md]`
- **Proakis·Salehi *Communication Systems* (1994, 907p)** — 아날로그/디지털 변조 이론 축, SNR·BER 성능 분석; OFDM·확산 부호화 개념의 이론적 배경 `[raw/books/proakis-communications-systems.md]`
- **3G/4G 이동통신 (이상근 외 2009)** — 채널 코딩·채널 모델링·Rake 수신 — OFDM 전신인 확산·코딩 계열 `[raw/books/3g4g-mobility-systems.md]`

## Related
- [[wireless-channel-modeling]] — flat vs frequency-selective, CP 설계
- [[array-antenna-beamforming]] — MIMO × OFDM (space-time coding)
- LTE: [[lte-radio-interface]] — OFDM downlink / SC-FDMA uplink
- 책: [[mimo-ofdm-wireless-matlab]] (전강), [[latest-mobile-comm-systems]]
- 디지털통신 실습: [[digital-communication-matlab]] (OFDM 시뮬레이션) · [[proakis-communications-systems]] (이론)
- 방송 접목: [[h264-avc-video-compression]] (모바일 TV 5개 방식) · [[hdtv-theory-technology]] (DVB/ATSC/ISDB-T)
