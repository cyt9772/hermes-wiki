---
title: 소프트웨어 정의 무선 (Software Defined Radio, SDR)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [wireless-communications, software-defined-radio, telecom-systems]
sources: [raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 소프트웨어 정의 무선 (SDR)

하드웨어(반도체/IC)로 고정한 기능을 **소프트웨어 알고리즘**으로 재구성하는 무선 통신 패러다임.

## 핵심 정의
"소프트웨어 무선기술은 이들 서비스가 **하나의 작은 단말기로 [제공] 수 있는 가능성을 가지고 있다**" `[raw/books/latest-mobile-comm-systems.md]` p.500

## 3분류 (8장, p.500)
| 유형 | 예 |
|------|----|
| **통신기반** | PDC / PHS / CDMA 디지털 셀룰러 |
| **제어-기반** | GPS / VICS / 레이다 (AHS, ETC) |
| **방송기반** | 라디오 / 아날로그 TV / 위성 TV / 디지털 TV |

## SDR 구현 원칙
1. **모듈화** — RF / 기저대역 / 프로토콜을 분리
2. **모듈간의 연결 규칙** — 디지털 인터페이스(예: IQ 샘플 스트림)
3. **실시간성** — 고속 DAC/ADC + DSP/FPGA
4. **업그레이더빌리티** — 펌웨어(소프트웨어) 업그레이드로 표준 전환 가능

## 이 책의 SDR 관점 (8장)
"소프트웨어 무선기술을 실현하는 PHS 응용 (1)(3)에서와 같다. … 한 대의 차량에서 사용될 수 있는 서비스의 수는 10가지가 넘는다. 그래서 소프트웨어 무선기술의 구현이 가능한 빨리 이루어져야 한다." `[raw/books/latest-mobile-comm-systems.md]` p.500

## Related
- [[mimo-ofdm-wireless-matlab]] — OFDM/MIMO를 SDR로 구현하는 현대적 예
- [[spread-spectrum-cdma]] — CDMA는 SDR로 가장 자연스러운 재구성(소프트웨어 디스프래터)
- [[channel-access-protocols]] — 프로토콜 부프로그램 교체(`feval(char(protocol(pno)))`)는 SDR 철학의 실체
- 책: [[latest-mobile-comm-systems]] (8장 전강)
