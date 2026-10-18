---
title: 무선 채널 모델링 (Wireless Channel Modeling)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, channel-modeling, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 무선 채널 모델링

무선 전파의 **추적 불가능한 산란·다경로·도플러**를 통계 분포로 모델링하는 프레임워크.

## 모델 분류 (4장 계열)
| 모델 | 가정 | 사용처 |
|------|------|--------|
| **AWGN** | 가산 백색 가우스 잡음만 | BER 기저 성능 |
| **Rayleigh** | LOS 부재, 단경로 다중경로 (fading) | 셀룰러 indoor/urban |
| **Rician** | LOS + scattered | line-of-sight 존재 |
| **Log-Normal** | 장기 shadowing (건물·지형 블록) | 셀 커버리지 마르코프 |
| **MIMO 채널** (H matrix) | 다안테나 상호 채널 | 공간 다이버시티 |

## 다중경로 통계 양상
- **도플러 천이 (Doppler shift)** `f_d = f_c·v/c·cosθ` — 이동속도와 주파수에 비례
- **코히어런트 시간** (coherence time) `T_c ~ 1/f_d`
- **코히어런트 대역폭** (coherence bandwidth) `B_c ~ 1/τ` (지연 전이 분산)
  - `B_c` 커짐 → flat fading (narrowband)
  - `B_c` 작음 → frequency-selective (OFDM 필요)

## BER 시뮬레이션 흐름 (제4장)
1. 변조 심볼 생성 ([`[[digital-modulation]]`])
2. 채널: AWGN / Rayleigh / Rician / MIMO H
3. 잡음/산란 인접 (rayleigh fading: `h ~ CN(0,1)`)
4. 복조 → BER 계산
5. 주파수 sweep (SNR range)

## Related
- [[digital-modulation]] — BER을 측정하는 변조 기법
- [[spread-spectrum-cdma]] — 레일리 페이딩에서의 확산 이득
- 책: [[latest-mobile-comm-systems]] (4장), [[mimo-ofdm-wireless-matlab]] (MIMO 채널 모델링 전강 — 제2·3장)
