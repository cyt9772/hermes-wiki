---
title: OFDM — 직교 주파수 분할 다중화
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, ofdm, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md]
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

## Related
- [[wireless-channel-modeling]] — flat vs frequency-selective, CP 설계
- [[array-antenna-beamforming]] — MIMO × OFDM (space-time coding)
- 책: [[mimo-ofdm-wireless-matlab]] (전강), [[latest-mobile-comm-systems]]
