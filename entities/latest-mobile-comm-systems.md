---
title: 최신 이동통신 시스템 (Latest Mobile Communication Systems)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, telecom-systems, wireless-communications, matlab-simulation, ofdm, mimo, cdma, channel-modeling, software-defined-radio]
sources: [raw/books/latest-mobile-comm-systems.md]
confidence: high
---
# 최신 이동통신 시스템 (최신 이동통신 시스템)

> "MATLAB 실습예제가 풍부한 — 유비쿼터스 모바일 시대의 가이드북" (표지)
> 원서: Harada & Prasad, *Simulation and software radio for mobile communications* (Artech House, 2002, ISBN 1-58053-044-3)
> 국내 번역: 차종상 · 이종헌 · 강창목 · 왕진철 편역, 도서출판 그린 (ISBN 89-5727-063-9, 509p)

## 개요
이동통신 시스템의 **이론 + MATLAB 시뮬레이션**을 병행하는 실무 교재. "이동통신시스템에 대한 이해도를 극대화하기 위한 방편으로서 … 컴퓨터 시뮬레이션을 활용한 핵심적인 내용 및 시스템을 구현 및 평가하는 기법을 병행" `[raw/books/latest-mobile-comm-systems.md]` p.13

핵심 원칙: 이동통신 역사를 통해 최근 표준의 개념을 배운다(개척기→셀룰러 이전→셀룰러 3시대) `[raw/books/latest-mobile-comm-systems.md]` p.14.

## 장 (chapter) 구조
| 장 | 주제 | 핵심 |
|----|------|------|
| 1 | 이동통신 역사 | 개척기(1860s Maxwell 전자기파 공리) / 셀룰러 이전 / 셀룰러 시대로 3분류 (표 1.1) |
| 2 | MATLAB 기초 | 벡터·행렬·인덱싱·행렬연산, 데이터 생성과 BER, 이동통신용 I/O |
| 3 | 디지털 변조 | BPSK / QPSK / 직교변조 / OQPSK / MSK — 이론 + 시뮬레이션 코드 (pp.65-131) |
| 4 | 채널 모델링 | AWGN / 레이리 / 로레이 — BER 성능 시뮬레이션 |
| 5 | 확산·CDMA | 직접 확산(직접/주파수/시간/Chirp/합성) / 확산 코드(LFSR, Gold, 직교 Gold) / BER (pp.266-295) |
| 6 | 다중접속 프로토콜 | 비경합·경합, 순수/슬롯 ALOHA, 비경합/슬롯 CSMA — MATLAB 코드 (pp.295-362) |
| 7 | 어레이 안테나·빔포밍 | 셀룰러용 어레이 안테나 (beamforming) 기술 (10.7 MHz 고속 데이터, 5.8 GHz 3G) |
| 8 | 소프트웨어 무선 (SDR) | 소프트웨어로 만드는 통신기 — 모듈/연결 규칙, 통신기·제어기·방송기 3종 분류 (p.500) |

## 핵심 인용
- **이론+시뮬레이션 병행**: "이동통신시스템에 대한 이해도를 극대화하기 위한 방편으로서 … 컴퓨터 시뮬레이션을 활용한 …시스템을 구현 및 평가하는 기법을 병행" `[raw/books/latest-mobile-comm-systems.md]` p.13
- **역사 = 최근 표준의 개념**: "이동통신의 역사는 세 시기로 범주화 될 수 있다. (1) 개척기 (2) 셀룰러 이전시기 (3) 셀룰러 시기" `[raw/books/latest-mobile-comm-systems.md]` p.14
- **CDMA = 부호화 다중접속**: "CDMA 프로토콜은 다중접속 능력이 주로 코딩에 의해 달성되는 프로토콜로 구성된다 … 각 사용자에게 자신의 정보신호를 부호화하는데 사용되는 고유의 코드 [가] 부여한다" `[raw/books/latest-mobile-comm-systems.md]` p.267
- **SS 변조 군에서 민간으로**: "SS 변조방식은 원래 재밍회피와 낮은 검출확률로 인해 군사용 레이더와 통신에서 사용되기 위해 개발되었다" `[raw/books/latest-mobile-comm-systems.md]` p.267
- **ALOHA/CSMA 시뮬레이션**: `while` 루프 + `feval(char(protocol(pno)))` — 프로토콜 부프로그램 교체로 다양한 접근 프로토콜 시뮬레이션 `[raw/books/latest-mobile-comm-systems.md]` p.334
- **SDR 목적**: "소프트웨어 무선기술은 이들 서비스가 하나의 작은 단말기로 [제공] 수 있는 가능성을 가지고 있다" `[raw/books/latest-mobile-comm-systems.md]` p.500

## 주의 (OCR quality)
- 수식·식 번호 깨짐 많음 (e.g. `02844&`=`[CDMA에서]`, `SEAALS`=`[코드로]`, `PSs ASE SS`=`[SS]`, `np-CSMA`=`[비경합 CSMA]`)
- MATLAB variable name 깨짐 (`Splen`=Send_len, `Wtime`=wait_time, `Mstatedl`=`Mstate(1)`)
- **MATLAB 코드를 재사용할 경우 원본 PDF 대조 필수**

## Related
- 저자: [[hiroshi-harada]], [[ramjee-prasad]]
- 개념: [[spread-spectrum-cdma]], [[digital-modulation]], [[wireless-channel-modeling]], [[channel-access-protocols]], [[array-antenna-beamforming]], [[software-defined-radio]]
- 관련 책 (동일 원서): [[mimo-ofdm-wireless-matlab]] — Harada·Prasad의 후속작
