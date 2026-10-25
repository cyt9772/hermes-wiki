---
title: MATLAB 실습과 함께 배우는 아날로그 및 디지털 통신이론 (김명진, 2007)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, telecom-systems, signal-processing, stochastic-processes, dsp, matlab-simulation]
sources: [raw/books/analog-digital-communication-theory-matlab.md]
confidence: high
---
# MATLAB 실습과 함께 배우는 아날로그 및 디지털 통신이론 (김명진, 2007)

> 저자: **김명진** — "대학에서 3학년을 대상으로 통신공학 강의를 해오면서 학부생도 쉽게 접근할 수 있는 적절한 교재가 아쉬워하던 중 생능출판사의 권유로 이 책을 집필하기로 한 이래 벌써 3년의 세월이 흘렀다" (서문, 2007년 1월 서명).
> 발행: **생능출판사** — "초판 발행 : 2007. 2. 15 / 제11판 4쇄 : 2010. 2. 10 / 발행인: 김승기 / 발행처: 생능출판사 / ISBN: 978-89-7050-573-2" (권말, p.943). 943p.
> 성격: "이 교재는 학부 과정에서 두 학기에 걸쳐 강의되면 적당할 것으로 본다. 만일 이 교재가 디지털 통신 과정에 대한 교재로 사용된다면 6장부터 다루면 될 것이다" (서문) — 아날로그(2–5장) → 확률(6장) → 디지털(7–13장) 단일 서술선.

## 개요
아날로그·디지털을 **한 책에 통합**한 한국어 통신공학 교재. 디지털 편에서는 "반송파의 진폭, 주파수, 위상을 M 개로 확장한 MASK, MFSK, MPSK 변조와 반송파 진폭과 위상을 모두 변화시키는 QAM 변조 등에 대해 스펙트럼 특성과 비트오율 성능 등에 대해 설명하였다" (서문) — 이어 **"12장에서 다루는 대역확산 통신은 CDMA 이동전화 시스템의 기본을 이루는 전송방식이다. 그러나 앞에서 다룬 전송 방식과 개념이 다르기 때문에 11장에 포함시키지 않고 별도의 장으로 다루었다"** (서문) — 대역확산(확산스펙트럼) 전송방식을 다른 디지털 변조 장에서 분리해 독립 장(12장)으로 전거한 것이 이 책의 특징.

**MATLAB 실습 결합**이 서술의 축이다: "이 책에서는 MATLAB 실습을 통하여 통신 과정의 이해도를 높이고자 하였으며, MATLAB 프로그램에 익숙하지 않은 학생들을 위하여 예제 프로그램을 같이 수록하였다. 예제 프로그램을 포함하여 실습 과정에서 많이 호출하는 함수들을 CD에 같이 제공하였다" (서문) — 13장 중 7개 장에 "Matlab을 이용한 실습" 절이 정례화(3.8 p.189, 4.8 p.275, 5.8 p.367, 8.4 p.571, 9.5 p.636, 10.5 p.707, 11.8 p.792). [[practical-digital-communications-korea]](문호, C/Matlab)·[[computer-based-exercises-signal-matlab]](Proakis)·[[a-course-in-dsp]](Mitra, Matlab Companion)와 같은 실습형 계열.

## 장 구조 (13장, 943p)
| # | 제목(목차) | pp. |
|----|------|-----|
| 1 | 서론 (통신의 원리, 아날로그/디지털 시스템, SNR·채널 대역폭) | 17–38 |
| 2 | 신호의 시간 영역 분석 (신호 성질·분류, 선형시스템·convolution, 상관함수) | 39–85 |
| 3 | 신호의 주파수 영역 분석 (직교표현, 푸리에 급수·변환, 스펙트럼 밀도, **Matlab 실습 3.8 p.189**) | 86–206 |
| 4 | 진폭 변조 (DSB-SC/DSB-TC/SSB/VSB, PLL·Costas 루프, FDM·수퍼헤테로다인, Matlab 4.8 p.275) | 207–303 |
| 5 | 각 변조 (FM/PM, 잡음효과, FM 스테레오, Matlab 5.8 p.367) | ~310–379 |
| 6 | 확률변수와 랜덤 프로세스 (확률, 통계적 평균, 주요 분포, 랜덤 프로세스 PSD, 백색잡음) | 380–455 |
| 7 | 펄스 변조와 펄스부호 변조 (표본화, PAM/PWM/PPM, TDM, PCM·양자화, DPCM, DM/ADM) | 456–528 |
| 8 | 디지털 데이터의 기저대역 전송 (NRZ/RZ/맨체스터 라인코딩, **눈 다이어그램 8.2.2 p.558**, ISI·펄스정형, **Raised-cosine 8.3.2 p.566**, Matlab 8.4 p.571) | ~529–587 |
| 9 | 기저대역 신호 검출 (NRZ 검출, **정합필터 9.2.1 p.605**, 상관수신기 9.2.3 p.615, **최적 수신기 9.3 p.618**, 비트오율 9.4 p.625) | ~588–647 |
| 10 | 디지털 대역통과 변조 (ASK/FSK/PSK/DPSK, 반송파 복구, Matlab 10.5 p.707) | ~648–724 |
| 11 | M-진 변조 (대역통과 신호 표현, QPSK, **MSK 11.3 p.749**, MASK 11.4 p.762, MPSK 11.6 p.780) | ~725–809 |
| 12 | 대역확산 통신 (개념, **직접수열(DS) DS-SS 12.2 p.822**, **주파수도약(FH) 12.3 p.843**, PN 코드 12.4 p.848, PN 동기화 12.5 p.859) | ~810–865 |
| 13 | 채널 코딩 (개념, 선형 블록코드 13.2 p.890, 인터리빙 13.3 p.906, **컨볼루션 코드 13.5**) | ~866–934 |

## 핵심 주제
- **정합 필터·최적 수신기** (9.2.1 p.605, 9.3 p.618) — "정합 필터를 이용한 신호의 검출"(9.2.2 p.610)·상관 수신기(9.2.3 p.615)를 9장에서 집중 서술, 9.4 비트오율(SNR) 성능으로 수렴. [[stremler-introduction-communication-systems-3ed]] 7.11·[[taub-schilling-principles-communication-systems-2ed-trans]] 11.4·[[practical-digital-communications-korea]] 2.5의 같은 내용과 병렬.
- **대역확산 DS-SS/FH + PN 코드** (12장) — "대역확산 통신은 원래 군사용으로 보안성이 높은 통신의 목적으로 개발" (12.1) → 다중접속(CDMA)으로 확장(서문: "CDMA 이동전화 시스템의 기본을 이루는 전송방식"). [[cdma-all]]·[[mobile-communication-engineering-korea]] 10장(디지털 CDMA 셀룰라)과 직결.
- **M-진 변조(MSK/MASK/MPSK/QAM)** (11장) — 서문에서 명시; [[stremler-introduction-communication-systems-3ed]] 10.6 QAM과 동시대 변조 이론.
- **MATLAB 실습 정례화** — 각 장에 Matlab 실습 절 + 예제 프로그램 CD 동봉. [[computer-based-exercises-signal-matlab]](Proakis)·[[a-course-in-dsp]](Mitra)와 같은 계열.
- 연습문제 풀이는 "이 교재에 동반되어 제공되는 CD에 수록" (서문).

## 관련
- 저자: 김명진 (대학 통신공학 강사)
- 아날로그·디지털 통신 교재군: [[stremler-introduction-communication-systems-3ed]] · [[taub-schilling-principles-communication-systems-2ed-trans]] · [[practical-digital-communications-korea]]
- 확산/이동통신: [[cdma-all]] · [[mobile-communication-engineering-korea]] · [[latest-mobile-comm-systems]]
- 확률·부호화 배경: [[a-papoulis]] (6장 랜덤 프로세스) · [[probability-random-variables]] · [[coding-information-theory]] (13장 컨볼루션/블록 코드) · [[signals-and-systems-oppenheim]] (2·3장 신호분석 도구)

## 추출/OCR 신뢰도
text-layer 전반 양호(목차·서문·본문 가독), 목차 OCR 노이즈("Matlab" → 깨진 토큰, "Pulse Shaping" → 깨진 토큰)만 존재. 11.2·13.1 소절 페이지는 목차 OCR으로 누락. 원문 PDF: `/work/wiki/raw/books/analog-digital-communication-theory-matlab.pdf`.
