---
title: 디지털 변조 (Digital Modulation)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 디지털 변조 (Digital Modulation)

디지털 기저대역(bit stream)을 무선 주파수 대역으로 올리는 3축(진폭/위상/주파수) 변조 방법론.

## 이 책의 변조 분류 (제3장)
| 변조 | 축 | 주 특징 |
|------|----|---------|
| **BPSK** | 위상 (0/180°) | 2상 위상; 가장 단순한 위상 변조 |
| **QPSK** | 위상 (4상) | 2비트/심볼; 주파수 효율 2×BPSK |
| **QAM / 직교 변조** | 위상 + 진폭 | M-QAM, 주파수 효율 3×QPSK (16/64/256) |
| **OQPSK** | 위상 (4상, 직교) | 위상 점프 180° 금지 — 비코헤런트 수신 적합 |
| **MSK** | 위상 + 주파수 (FM 계열) | 연속 위상, 제한 스펙트럼, 직교 위상 |

## BPSK 기본 구조 (3.2)
- I(동상)/Q(직교) 채널 분리
- 심볼 매핑: `0 → +1, 1 → -1`
- 코헤런트 수신은 180° 위상 역전 문제(180° ambiguity) 존재 — OQPSK/MSK가 해법

## MSK 특징 (3.5)
- Gaussian-pulsed FSK, h=0.5
- 제한 대역(제한 스펙트럼) + 연속 위상

## MATLAB 시뮬레이션 패턴 (이 책 공통)
1. 랜덤 bit stream 생성
2. 심볼 mapper (`0/1` → `I/Q`)
3. upsample (칩률) + channel filter (root-Nyquist)
4. AWGN / Rayleigh channel
5. 채널 추정 + 복원 → BER plot

## Related
- [[spread-spectrum-cdma]] — 변조 위에 확산 칩 곱하기
- [[wireless-channel-modeling]] — 페이딩 환경에서의 BER
- 책: [[latest-mobile-comm-systems]] (3장), [[mimo-ofdm-wireless-matlab]] (OFDM 변조와 대조)
