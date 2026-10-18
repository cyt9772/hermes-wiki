---
title: MIMO — 다중입력다중출력 (Multiple-Input Multiple-Output)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, mimo, ofdm, channel-modeling, signal-processing]
sources: [raw/books/mimo-ofdm-wireless-matlab.md]
confidence: medium
---
# MIMO (Multiple-Input Multiple-Output)

## 정의
**수신·송신 양쪽 모두에서 다수 안테나**를 사용해, 동일 주파수 대역에서 **병렬 공간(경로) 스트림**을 만들어 용량·링크 신뢰도를 높이는 무선 전송 기술. 단일 안테나(SISO) 대비 **공간 다이버시티·공간 분리(빔포밍)·공간 다중화** 3 효과를 조합.

## 핵심 원리
- **공간 다중화(Spatial Multiplexing)**: M×N 배열에서 min(M,N)개의 독립 스트림을 동시에 전달 → 용량 선형 증가. `용량 = min(M,N) × log2(1+SNR)` (근사)
- **공간 다이버시티(Spatial Diversity)**: 동일 정보를 다수 경로로 중복 전달 → 페이딩에 강함
- **빔포밍(Beamforming)**: 위상·진폭 가중으로 공간 방향성 집중

## MIMO 채널 모델 (제3장, 4 표준 비교)
- **I-METRA** — 3GPP 실외 셀룰러 MIMO 채널
- **SCM** — Spatial Channel Model (3GPP)
- **SCM-E** — 확장형 (Enriched)
- **IEEE 802.11 TGn** — 무선 LAN(와이파이) N MIMO 채널

> `raw/books/mimo-ofdm-wireless-matlab.md` p.~120-155

## MIMO-OFDM 결합
MIMO 스트림 × OFDM 서브캐리어 → **MIMO-OFDM** (3G UPA·LTE·5G NR의 기본 구성). OFDM은 다중경로 ISI를 제거, MIMO는 용량을 확장.

## Related
- [[ofdm-orthogonal-frequency-division]] — OFDM과 결합
- [[wireless-channel-modeling]] — SISO·MIMO 채널 모델
- [[space-time-coding]] — 시공간 부호
- [[array-antenna-beamforming]] — 안테나 어레이·빔포밍
