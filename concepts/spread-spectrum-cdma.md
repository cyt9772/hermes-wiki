---
title: 확산 스펙트럼 / CDMA (Spread Spectrum / Code Division Multiple Access)
created: 2026-10-18
updated: 2026-10-31
type: concept
tags: [wireless-communications, cdma, signal-processing, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md, raw/books/3g4g-mobility-systems.md, raw/books/comm-theory-matlab.md, raw/books/digital-communication-matlab.md, raw/books/proakis-communications-systems.md]
confidence: high
---
# 확산 스펙트럼 / CDMA

다중접속과 반간섭·보호를 **부호화**로 달성하는 무선통신 계열. 각 사용자에게 고유의 확산 코드(spreading code)를 부여해 정보신호를 넓은 대역으로 "확산"시켜 전송·수신한다.

## 정의
"CDMA 프로토콜은 다중접속 능력이 주로 코딩에 의해 달성되는 프로토콜로 구성된다. [각 사용자에게 자신의 정보신호를 부호화하는데 사용되는 고유의 코드 [가] 부여한다] … 코드신호의 대역폭이 정보신호의 대역폭보다 훨씬 크게 선택되기 때문에 부호화 과정은 [SS] 스펙트럼을 확산하고 이로 인해 확산 스펙트럼(SS) 변조라고 알려져 있다." `[raw/books/latest-mobile-comm-systems.md]` p.267

## SS 변조 두 조건
1. 대역폭이 정보 대역폭보다 **훨씬** 커야 한다.
2. 무선주파수 대역폭은 보내진 정보가 아닌 **다른 함수**에 의해 결정되어야 한다.
`[raw/books/latest-mobile-comm-systems.md]` p.268

## 분류 (5.2)
| 유형 | 원리 |
|------|------|
| **직접 확산 (DS)** | 칩(칩률 > 정보률)으로 직접 곱해 주파수 확산 |
| **주파수 합핑 (FFH)** | 캐리어를 hopping pattern으로 변경 |
| **시간 합핑 (TH)** | 시간 슬롯을 hopping pattern으로 변경 |
| **Chirp 확산** | 주파수 swept 칩 (linear chirp) |
| **합성(혼합)** | DS+FFH 또는 DS+TH 결합 |

## 확산 코드 생성 (5.3)
- **LFSR (Linear Feedback Shift Register)** — m-시퀀스
- **Gold 코드** — 두 개의 m-시퀀스 조합
- **직교 Gold 코드** — 상호 직교성이 보장된 Gold
- 직교 확산 시 **정합 필터** → 상관검출로 다중 사용자 분리

## 기원
"SS 변조방식은 원래 **재밍회피와 낮은 검출확률**로 인해 군사용 레이더와 통신에서 사용되기 위해 개발되었다. 최근에서야 … 민간부분에의 응용에 관심을 가지기 시작했다." `[raw/books/latest-mobile-comm-systems.md]` p.267

## BER 성능
- 5.5 AWGN 환경 / 5.5.2 레일리(Rayleigh) 환경에서 BER 시뮬레이션.
- 확산 이득 = 확산 코드 칩률/정보률비 (processing gain)

## 3G/4G 이동통신에서의 확산 (2009 배치 추가)
- **3G/4G 시스템 (이상근·조봉열·여운영 2009)** — 동기식 CDMA 배경 독자를 위한 비동기 WCDMA 비교; UMB 무선망 구조, 채널 코딩·채널 모델링·**Rake 수신** 개념, HSDPA/HSUPA/WiMAX(3.5세대)와 초기 4G 기술 흐름 `[raw/books/3g4g-mobility-systems.md]`
- **MATLAB 통신이론 (신윤기 2011)** — 각 장마다 MATLAB 프로그램 수록; 아날로그(AM/FM) + 디지털 변조(PSK/QAM) + 정합 필터·오판확률, SNR 중심 통신 성능 분석 + **확산 스펙트럼 11장** `[raw/books/comm-theory-matlab.md]`
- **디지털통신 MATLAB/SIMULINK (양원영 외 2005)** — 변조(QPSK/QAM)·채널 코딩·FEC·등화·OFDM의 MATLAB/SIMULINK 시뮬레이션; 이론/실습 축 `[raw/books/digital-communication-matlab.md]`
- **Proakis·Salehi *Communication Systems* (1994)** — 아날로그/디지털 변조 이론 축으로 SNR·BER 성능 분석 중심; 변조·확산 부호화·OFDM 개념 `[raw/books/proakis-communications-systems.md]`

## Related
- [[channel-access-protocols]] — 다중접속 접근 방식 비교 (ALOHA/CSMA는 임의, CDMA는 부호 기반 임의·동시)
- [[digital-modulation]] — 변조 방식과 결합
- [[wireless-channel-modeling]] — 레일리/로레이 페이딩 환경에서의 성능
- [[software-defined-radio]] — CDMA 수신/부호화도 SDR로 구현
- 책: [[latest-mobile-comm-systems]] (5장 전강), [[mimo-ofdm-wireless-matlab]]
- 3G/4G: [[3g4g-mobility-systems]] (WCDMA·Rake·UMB) · [[comm-theory-matlab]] (MATLAB 확산 11장) · [[digital-communication-matlab]] (MATLAB/SIMULINK)
- 이론: [[proakis-communications-systems]] (변조·확산·BER)
