---
title: 어레이 안테나 / 빔포밍 (Array Antenna / Beamforming)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 어레이 안테나 / 빔포밍

여러 안테나 요소를 배열·가중으로 배열해 **공간 방향성(beam)**을 형성·추적하는 기법. 셀룰러·5G MIMO의 핵심.

## 기본 원리
- N개 안테나 + N개 가중 → 공간 응답(steering vector)
- DOA(Direction Of Arrival) 추정: MVDR / MUSIC
- beamforming gain: `N·directivity`

## 셀룰러 적용 (제7장)
"7.5 셀룰러 시스템을 위한 어레이 안테나를 사용한 beamforming 기술" `[raw/books/latest-mobile-comm-systems.md]` TOC p.10

- 셀 엣지 간섭 감소
- 공간 다이버시티 + beamforming
- 고속 데이터 (10.7 MHz, 5.8 GHz 3G) — 주파수 효율·공간 효율 동시 확보

## 관련
- [[mimo-ofdm-wireless-matlab]] — MIMO 안테나 시스템과 시공간 부호(STBC)의 상세 이론·MATLAB
- [[wireless-channel-modeling]] — MIMO H matrix 모델링
- [[spread-spectrum-cdma]] — CDMA + beamforming 결합 (3G CDMA)
- [[software-defined-radio]] — 빔포밍 가중을 SDR로 재구성
