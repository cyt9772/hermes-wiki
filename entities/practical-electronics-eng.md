---
title: 모듈을 위한 실용 전자공학 (Practical Electronics for Inventors, 4th ed.)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/practical-electronics-eng.md]
confidence: high
---
# 모듈을 위한 실용 전자공학 (Practical Electronics for Inventors, 4ed)

> "모듈을 위한 실용 전자공학 — 기초부터 실무까지" (표지)
> 원저: Paul Scherz, Simon Monk — *Practical Electronics for Inventors*, 4th Edition (McGraw-Hill, 2016)
> 번역: 박진수 옮김, McGraw-Hill Education Korea + J Pub, 2018-11-30 (ISBN 979-11-88621-32-3), 1068p

## 개요
**발명가・실무자를 위한 전자공학 교과서 전체 스펙트럼 교재**. 회로이론(옴의 법칙·키르히호프·RLC)에서 반도체(다이오드·트랜지스터·사이리스터), 광전자, 센서, 측정 장비(오실로스코프), 필터, 발진기/TIMER(555), 전원장치(SMPS), 디지털 논리, 마이크로컨트롤러(아두이노·PIC), FPGA(Verilog·VHDL), 모터 구동, 오디오 전자학에 이르기까지 — 기초→실무 전 과정을 다루고 모듈/오픈소스 하드웨어(17장)로 마무리. `[raw/books/practical-electronics-eng.md]`

## 장 구조 (17장 + Appendix A, 1068p)
1. **전자공학 소개**
2. **전자공학 이론** — 전류·전압·저항·접지, 옴의 법칙, 키르히호프, 중첩·테브난/노턴 정리, 커패시터·인덕터
3. **기본 전기 회로 부품** — 전선·케이블·커넥터, 전지(1차/2차), 스위치, 계전기, 저항기, 커패시터, 인덕터
4. **반도체** — 다이오드(PN·제너·버랙터·LED·마이크로파), 트랜지스터(BJT·JFET·MOSFET·IGBT), 사이리스터(SCR·트라이액), 과도전압 억제, IC 패키지
5. **광전자공학** — LED·레이저·광저항기·광 다이오드·광전지·광 트랜지스터·광 사이리스터·광섬유
6. **센서** — 정밀도/정확도, 온도(서미스터·열전대), 근접성, 운동·힘·압력
7. **오실로스코프** — 작동 원리·빔·측정·응용·임피던스
8. **전자공학 실험실** — 작업장·멀티미터·직류 전원·시험 장비
9. **필터** — 수동/능동 저역·고역·대역통과·노치, 통합 필터 IC
10. **발진과 타이머** — RC 발진기, **555 타이머 IC**(비안정/단안정), VCO, 빈 브리지, LC·결정 발진기
11. **전압 조정기와 전력 장치** — 고정/가변 조정기, 변압기·정류기, **스위칭 조정기(SMPS)**
12. **디지털 전자공학** — 논리 상태·게이트·조합 논리·제품군(TTL/CMOS), 순차 논리(플립플롭·계수기·시프트 레지스터), A/D·D/A, ROM·RAM, 디스플레이
13. **마이크로컨트롤러** — ATtiny85·PIC·32비트 MCU·DSP, **아두이노**, 인터페이스
14. **프로그램 가능 논리(FPGA)** — Icarus, Elbert v2 보드, **Verilog/VHDL**, 시뮬레이션
15. **모터** — 직류 모터 속도/방향 제어, 서보, 스테퍼
16. **오디오 전자공학** — 마이크·증폭기·믹서·임피던스 정합·스피커
17. **모듈** — 브레이크아웃 보드, RF/오디오 모듈, 플러그앤플레이, 오픈소스 하드웨어
+ **Appendix A** — 배전과 가정 배선(3상)

## 핵심 기여 / 학습 포인트
- **이론→부품→회로→시스템→실습**의 완결된 전자공학 교육 경로 (17장 연속)
- **반도체 3대 계통**(4장 다이오드·4장 트랜지스터·4장 사이리스터)의 동작 원리 물리 기반
- **실습 도구** 7장(오실로스코프) + 8장(실험실)이 별도 장 — 이론 교재와 차별점
- **555 타이머(10장)** — 가장 범용적인 타이머 IC의 완전 분석
- **FPGA + Verilog/VHDL(14장)** — 하드웨어 기술(HDL)까지 다루는 이례적 범위

## OCR 신뢰도
- **주의**: scan-only → tesseract 300dpi 재-OCR. 수치/단위/식 심하게 깨짐 (예 "66009"=6.6.6.9 식)
- **활용법**: 구조·개념 학습용으론 충분. 수치 해석·회로 설계 재사용 시 원본 대조 필수

## Related
- 저자: [[paul-scherz]], [[simon-monk]] — 원저 2인, 박진수 번역
- 개념: [[semiconductor-devices]], [[sensors-electronics]], [[analog-filter-design]], [[timer-oscillator-circuits]], [[power-supply-regulation]], [[digital-logic-basics]], [[microcontroller-arduino]], [[fpga-hdl]]
- 관련 책(전자공학 분야): 없음 (이 1권이 전자공학 기초의 축)
