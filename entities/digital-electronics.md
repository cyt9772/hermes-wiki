---
title: Digital Electronics, 3rd ed. (McGraw-Hill Basic Skills, 1990)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, electrical-engineering, digital-electronics, electronic-circuits]
sources: [raw/books/digital-electronics.md]
confidence: high
---
# Digital Electronics, 3rd ed. (Tokheim, 1990)

> 저자: Roger L. Tokheim (표지 OCR 'TFIID T이/어티M' — copyright 페이지 CIP 데이터 'Tokheim, Roger L.'로 확정)
> McGraw-Hill, 『Basic Skills in Electricity and Electronics』 시리즈, 3rd ed. 1990 (International Edition, Singapore 인). ISBN 0-07-100352-5, 352p

## 개요
**직업학교(Basic Skills) 과정용 디지털 전자공학 입문서**. DC/전기 기초에서 2진 코드(BCD·Excess-3·Gray·ASCII), 논리 게이트·부울대수, 결합/순차 논리(인코더·디코더·7-segment 디스플레이, 플립플롭·카운터·시프트 레지스터), 산술 회로(Half/Full Adder, 2의 보수), 메모리(RAM·ROM·PROM), 디지털 시스템(계산기·디지털 시계·주파수 카운터)까지 전 범위를 다룹고, 마지막 13장에서 연산증폭기를 매개로 D/A·A/D 변환(가다이어형·비교기·디지털 멀티미터·광량계)으로 아날로그 세계와 연결한다. 매 장마다 짧은 Self-Test 문제(해답 포함)가 반복 배치되는 실습 중심 구조. `^[raw/books/digital-electronics.md]`

## 장 구조 (13장 + Index, 352p)
1. **Digital Electronics** — 디지털/아날로그 구분, 2가치 로직, 계산기·시계·PC 응용
2. **Numbers We Use in Digital Electronics** — 2진·8진·16진, BCD, 보수
3. **Binary Logic Gates** — AND/OR/NOT/NAND/NOR/XOR·XNOR, 게이트 IC (74xx TTL/40xx CMOS), 부울대수
4. **Using Binary Logic Gates** — 조합 논리: MUX·DEMUX·인코더/디코더, 74151/74154, 7-segment LCD·VF 디스플레이 구동, 트러블슈팅
5. **Encoding, Decoding, and Seven-Segment Displays** — 8421/Excess-3/Gray/ASCII 코드, 7447 데코더/드라이버, LCD 구동
6. (5·6장 통합 영역) 플립플롭 전단계 타이밍 회로 + **7. Flip-Flops** — R-S·클럭 R-S·D·J-K, IC 래치, 트리거 동작, 슈머트 트리거
7. **Counters** — 리플/동기/다운/자가동정 카운터, 주파수 분배기, TTL/CMOS 카운터 IC, 게임기 응용, 트러블슈팅
8. **Shift Registers** — 직렬/병렬 로드, 74194 범용 시프트 레지스터, 디지털 룰렛, 시프트 등록기 고장 진단
9. **Arithmetic Circuits** — 2진 덧셈/감산, Half/Full Adder, 병렬 감산기, 4비트 Adder/Subtractor, 2의 보수, 곱셈기, Full Adder 트러블슈팅
10. **Memories** — RAM(SRAM IC), ROM, PROM, 자기 코어 메모리, 대용량 저장장치, 마이크로컴퓨터 메모리
11. **Digital Systems** — 계수기·컴퓨터·마이크로컴퓨터 구조, 주소 디코딩, 데이터 전송 에러 검출, 디지털 시계(LSI), 주파수 카운터, LCD 타이머, 게임기
12. **Connecting with Analog Devices** — D/A 변환(가다이어형), 연산증폭기 개요, A/D 변환(비교기·기초·양자화), A/D IC, 디지털 광량계, 디지털 멀티미터

## 핵심 기여 / 학습 포인트
- **직업학교 과정 설계**: 매 주제마다 "설명 → Self-Test → 실제 IC(74194·74151·7447 등) 적용 → Troubleshooting" 루프 — 수학과 이론서가 아니라 "부품 레벨에서 만지는" 디지털 전자학
- **TTL(74xx)과 CMOS(40xx) 양 시리즈 실용 비교** — 같은 기능을 양쪽 IC로 구현하는 장들(디스플레이·카운터)은 제품군 차이를 체득하게 함
- **디지털 ↔ 아날로그 접점(13장)** — 연산증폭기를 매개로 한 D/A·A/D 변환 원리가 디지털 교재 안에서 자립적으로 설명됨
- **LSI 시대의 디지털 시계·주파수 카운터 설계** — 1990년대 기준 실제 제품(디지털 시계 IC)을 분해해 설계

## OCR 신뢰도
- PDF 내장 텍스트 레이어 사용(pdftotext -layout, OCR 불필요). 일부 대문자 표지·TOC 라틴자 깨짐('T이/어티M', 'E미ㄲON') — 본문은 양호
- 수식·부호(논리 기호, IC 핀 번호)는 레이아웃 추출 특성상 열 정렬 깨짐 가능 — IC 번호와 수치 해석 시 원본 PDF 대조 권장

## Related
- 저자: (단발성 — Roger L. Tokheim, 직업교육 시리즈 저자 → 엔티티 미생성)
- 개념: [[digital-logic-basics]], [[semiconductor-devices]], [[amplifiers-analog-circuits]], [[fpga-hdl]] (디지털 논리 확장)
- 관계서: [[digital-theory-experimentation]] (같은 주제 실험서), [[intro-electronics]] (동 시대 기술직 수험서)
