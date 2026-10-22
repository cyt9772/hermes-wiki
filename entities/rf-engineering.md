---
title: RF and Microwave Wireless Systems (Chang 2000 / 한빛미디어 2009)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, engineering, rf, microwave, antenna]
sources: [raw/books/rf-engineering.md]
confidence: high
---
# RF and Microwave Wireless Systems / RF 및 초고주파 공학 (Chang 2000, 한빛미디어 2009)

> 원저: **Kai Chang** (UCLA) — RF and Microwave Wireless Systems, 2000 John Wiley & Sons
> 번역: 홍익표
> 출판: **한빛미디어**, 1판 2009-08-24 / 2쇄 2011-07-06, ISBN 978-89-7914-685-1, 390p

## 개요
**무선(RF/마이크로파) 시스템**의 전 주파수 대역(300kHz~300GHz)을 다루는 교재. **개요(제0장: RF/마이크로파 무선 시스템의 역사 — Maxwell·Hertz·Marconi —, 주파수 스펙트럼)** → **전파와 전송선로(제1장: 전송선로 방정식, 임피던스/반사/전달, 정재파비, 데시벨, 스미스차트, 산란계수, 동축/Microstrip, 도파관)** → **안테나 시스템(제2장: 등방성 방사체, 원거리장, 모노폴/다이폴, 혼, 파라볼라, Microstrip 패치, 배열/위상배열)** → **무선통신 부품과 시스템 파라미터(제3장: 결합기/하이브리드/전력분배기, 공진기/필터, 아이솔레이터/서큘레이터, 검파기/믹서)** → **수신기(제4장: 잡음, NF, P1dB, IM3, SFDR)** → **송신기·발진기(제5장)** → **변조/복조(제6장)** → **다중접속(제7장: FDMA/TDMA/CDMA/OFDMA)** `[raw/books/rf-engineering.md]`.

## 장 구조 (TOC 기반, 390p)
- **제0장 개요** — RF/마이크로파 무선 시스템의 역사(Maxwell·Hertz·Marconi), 주파수 스펙트럼, 무선 응용
- **제1장 전파와 전송선로** — 파의 전파, 임피던스/반사/전달, **VSWR**, 스미스차트, 산란계수, 동축/Microstrip, 도파관, 임피던스 정합
- **제2장 안테나 시스템** — 등방성 방사체, 원거리장, 모노폴/다이폴, 혼, 파라볼라, Microstrip 패치, **위상배열**, 측정
- **제3장 무선통신 부품** — 결합기/하이브리드/전력분배기, 공진기/필터/멀티플렉서, 아이솔레이터/서큘레이터, 검파기/믹서, 발진기/증폭기
- **제4장 수신기** — **잡음지수(NF)**, **압축점(P1dB)**, **IM3(3차 혼성)**, 스퓨리어스, **SFDR**
- **제5장 송신기와 발진기**
- **제6장 변조와 복조**
- **제7장 다중접속 기술** — **FDMA/TDMA/CDMA/OFDMA** 비교

## OCR 신뢰도
- text-layer 원서(한빛미디어 2009). VSWR/NF/P1dB/IM3/SFDR 표기 안정
- **활용법**: **유선/무선 공통**(전송선로) + **무선 시스템**(안테나·부품)이 한 권. [[microwave-engineering]](Pozar)이 이론+부품이면, Chang은 **실무 시스템 파라미터** 관점
- **주의**: 2000 원서 기준 — 4G/5G 시대의 OFDMA MIMO는 별도 서적

## Related
- 저자: [[kai-chang]] (UCLA)
- 개념: [[transmission-lines-microwave]] · [[antenna-design]]
- 인접: [[microwave-engineering]] (Pozar) · [[antenna-theory]] (Stutzman)
- 인접: [[spread-spectrum-cdma]] — 다중접속(제7장)
