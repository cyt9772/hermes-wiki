---
title: Introduction to Communication Systems (3rd ed., Stremler 1993)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, telecom-systems, signal-processing, wireless-communications, information-theory, coding-theory, stochastic-processes, fourier-analysis, dsp]
sources: [raw/books/stremler-introduction-communication-systems-3ed.md]
confidence: high
---
# Introduction to Communication Systems (Ferrel C. Stremler, 3rd ed. 1993)

> 저자: **Ferrel C. Stremler** — "This textbook presents to undergraduates an introductory explanation of communication systems, with the emphasis on signal design and modulation." (Preface, p.vii)
> 출판: Addison-Wesley, 3rd ed. 1993 (Copyright 1990, 1982, 1977 — 초판 1977, 2판 1982, 3판 1990/1993). 777p. 예제문제 117 + 훈련문제 133 + 장말 문제 520개 (60% 신규, Preface p.viii).
> 3판 신증: "Material added in this third edition is, primarily, about digital methods and reflects the continually increasing importance of digital signal transmission and modulation" — 파이버 옵틱·ISDN(제7장), Nyquist 펄스형성(ISI), FSK 확장(병렬/직렬 MSK), 확산스펙트럼 2절(제10장) 추가 (Preface, p.vii).

## 개요
통신공학의 분석·신호설계 입문 교과서로, "By 'communication' we mean the conveying or transmission of information from one place and/or time to another." (Chapter 1, p.1)으로 출발해 직교함수 표현 → 푸리에 변환 → 스펙트럼 밀도 → 아날로그 변조(AM·각변조) → 펄스 변조·PCM → 확률·랜덤 프로세스 → 정보이론·채널용량 → 디지털 변조(ASK/FSK/PSK·확산스펙트럼)로 이어지는 단일 서술 구조다. 아날로그·디지털 양쪽을 하나의 수학적 틀(정현파 전개, 정합필터, 최적검출)로 연결하는 전형적인 미국 교재.

가장 실용적인 장치는 장별 example/drill problem 체계(117+133문항, 답 포함)와 520개 장말 문제 — "These range from commercial broadcasting and telephone systems to satellite telemetry and radar" (Preface, p.vii)로 실제 방송·통신망을 예시로 삼는다. 정합필터는 7.11 "The Matched Filter" (p.431)·7.12 Matched-Filter Codeword Detection (p.437)에서 이론화되고, PN 열(7.13, p.439)·확산스펙트럼(10.5 Direct-Sequencing Spread Spectrum, p.627; 10.9 Frequency-Hopping, p.655)으로 이어져 이 책 내에서도 아날로그 검출 → 디지털 확산 변조로 하나의 선을 그린다.

제9장 "Information and Digital Transmission" (p.531~)에서 엔트로피·채널용량(9.2, p.536)·양자화 노이즈(9.4, p.541)·착오확률(9.5, p.547)을 다루어, [[coding-information-theory]](Hamming)의 코딩 관점과 교차한다.

## 장 구조 (10장 + 부록, 777p)
| # | 제목 | pp. |
|---|------|-----|
| 1 | Introduction | 1–7 |
| 2 | Orthogonality and Signal Representations (직교함수, 지수 푸리에 급수, 임펄스 응답) | 8–81 |
| 3 | The Fourier Transform and Applications (스펙트럼 밀도, DFT 3.17 p.135, FFT 3.18 p.141, 표본화 정리 p.126) | 82–162 |
| 4 | Spectral Density and Correlation (에너지/전력 스펙트럼 밀도, 상관, 대역제한 화이트 노이즈 4.7 p.188) | 163–218 |
| 5 | Amplitude Modulation (DSB-SC, AM, FDM, SSB p.255, VSB p.266, 감쇠·전파효과 p.277) | 219–297 |
| 6 | Angle Modulation (FM/PM, 임계치효과 6.9 p.351, 디이스프레싱 p.355) | 298–370 |
| 7 | Pulse Modulation (PAM, TDM, Nyquist 펄스형성(ISI), PWM/PPM, PCM, 파이버 옵틱·ISDN 7.10 p.429, **정합필터 7.11 p.431**, PN열 7.13 p.439) | 371–456 |
| 8 | Probability and Random Variables (확률밀도, 결합분포, 랜덤 프로세스 8.12 p.498, 자기상관·전력스펙트럼 p.504) | 457–530 |
| 9 | Information and Digital Transmission (엔트로피 9.1 p.531, 채널용량 p.536, 양자화 노이즈 p.541, PCM S/N p.558, DPCM p.560, 편차응답 p.572, 등화기 p.577, M-ary p.584, 오류정정 부호 p.589) | 531–607 |
| 10 | Digital Modulation (ASK p.608, FSK p.610, PSK p.618, **DS-SS 10.5 p.627**, QAM/QPSK p.634, MSK p.641, M-ary FSK p.651, **FH-SS 10.9 p.655**, M-ary PSK p.659, APK p.663, 최적 검출 10.14 p.673) | 608–748 |
| App A–I | 수식표·Decibels·방송주파수대역·전기전화채널·Bessel·스테레오AM·가우시안확률률표 | 693–746 |

## 핵심 주제
- **정합필터의 단일 서술선**: 7.11–7.12 (p.431–437)에서 두 신호의 격차를 검출하는 필터로 정의하고, 10.5·10.14에서 확산스펙트럼·최적검출 알고리즘으로 확장.
- **확산스펙트럼**: 3판 신증 두 절 — DS-SS(직렬확산, p.627)와 FH-SS(주파수 도약, p.655). "spread spectrum, in which the bandwidth is purely spread before transmission and then restored to its original in reception, is introduced" (제10장 서론, p.608) — CDMA 이동통신의 이론적 출발.
- **채널용량과 착오확률의 통합** (9.2 p.536, 9.5 p.547) — 아날로그 S/N 성능(AM/FM)와 디지털 비트오율 사이에 놓는 공통 척도.
- **DFT·FFT** (3.17–3.18) — 통신 맥락에서 DSP 기초(DFT)를 다루어 [[computer-based-exercises-signal-matlab]]류와 교차.
- 520문제 + 117 example + 133 drill 구조 — "lends itself to self-paced or individualized tutorial instruction" (Preface, p.vii).

## 관련
- 해답집: [[stremler-comm-systems-solutions]] (동 저자 3판 교재의 문제풀이, 성진출판)
- 동시대 교재: [[taub-schilling-principles-communication-systems-2ed-trans]] (Taub & Schilling 2판 한국역) · [[analog-digital-communication-theory-matlab]] (MATLAB 실습 교재)
- 확률·랜덤 프로세스: [[a-papoulis]] · [[probability-random-variables]] (제8장의 이론적 배경)
- 코딩·정보이론: [[coding-information-theory]] · [[richard-hamming]] (9.13 오류정정 부호)
- 신호·시스템: [[signals-and-systems-oppenheim]] · [[alan-v-oppenheim]] (제2·3장의 수학적 도구)
- 확산스펙트럼 응용: [[cdma-all]] (DS-SS/FH-SS의 이동통신 확장)

## 추출/OCR 신뢰도
pdftotext 양호. 일부 문자 깨짐(예: OCR에서 `Pulse …odulation` 중간 자 일부 누락 = Pulse Modulation, "ISI가미" = ISDN) — 식 번호·목차·문맥으로 cross-check. 원문 PDF: `/work/wiki/raw/books/stremler-introduction-communication-systems-3ed.pdf`.
