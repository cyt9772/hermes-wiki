---
title: 전송선로·마이크로파 정합 (Transmission Lines & Microwave Matching)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering]
sources: [raw/books/microwave-engineering.md, raw/books/rf-engineering.md]
confidence: high
---
# 전송선로·마이크로파 정합 (Transmission Lines & Microwave Matching)

RF/마이크로파(300kHz~300GHz)에서 신호를 전달·정합·분배하는 부품·기법.

## 두 관점 (Pozar vs Chang)

| 항목 | **Pozar** (이론+부품) | **Chang** (실무 시스템) |
|---|---|---|
| 전송선로 | lumped-element, Smith chart, quarter-wave (제3장) | 파의 전파, 임피던스/반사/전달, **VSWR**, Smith chart, 산란계수 (제1장) |
| 도체선/도파관 | microstrip, stripline, waveguide modes (제4장) | 동축/Microstrip, 도파관, 집중소자 (제1장) |
| **정합** | stub, quarter-wave, multi-section (제6장) | 임피던스 정합 네트워크 (제1장) |
| **부품** | power divider, **rat-race**, **Wilkinson**, 90/180 hybrid, **isolator**, **circulator**, **filter** (제7-11장) | 결합기, 하이브리드, 전력분배기, 공진기, 필터, 멀티플렉서 (제3장) |
| **수신기** | active circuit, amplifer, oscillator, noise figure (제9장) | 수신기, **잡음지수(NF)**, **압축점(P1dB)**, **IM3(3차 혼성)**, 스퓨리어스, **SFDR** (제4장) |
| **송신기** | amplifier, oscillator, noise (제9장) | 송신기 파라미터, 잡음, 변조 (제5장) |

## 실무 포인트
- **VSWR / 산란계수** — 두 책 모두. **Chang** 실무 측정, **Pozar** 이론
- **Smith chart** — 두 책 모두. **Pozar** 폭넓게(정합·부품 설계), **Chang** 실무
- **부품 설계** — **Pozar** 제7-11장 상세, **Chang** 제3장 실무 개요
- **수신기 NF/P1dB/IM3/SFDR** — **Chang** 제4장만 상세 (수신기 품질 지표)

## 관련
- [[array-antenna-beamforming]] (기존) · [[wireless-channel-modeling]] (기존) · [[ofdm-orthogonal-frequency-division]] (기존)
