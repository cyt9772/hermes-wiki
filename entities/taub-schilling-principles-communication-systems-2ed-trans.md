---
title: 통신시스템의 이론과 원리 (Taub & Schilling 2판, 진용옥 역)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, telecom-systems, signal-processing, stochastic-processes, wireless-communications, information-theory, coding-theory, cdma-dsss]
sources: [raw/books/taub-schilling-principles-communication-systems-2ed-trans.md]
confidence: high
---
# 통신시스템의 이론과 원리 (Principles of Communication Systems, Taub & Schilling 2nd ed. 한국역)

> 원저: **Herbert Taub / Donald L. Schilling** (저자서문 서명 "Herbert Taub, Donald L. Schilling") — CUNY(뉴욕시립대학) 전자공학.
> 역자: **공학박사 진용옥 역** (표지 상단. 본문에 "역자로서는 다시 없는 영광이 될 것이다. … 이에 대한 책임은 전적으로 역자에게 있으며" — 역자서문).
> 원서 1판 1971 McGraw-Hill, 2판 1986 — "1971년에 미국의 Mcgraw-Hill출판사에 의해 초판이 출간된 이래 … 1986년에는 제 2판이 출간되었다" (역자서문, p. ii). 한국역 776p (성안당 계열 판본).

## 개요
1980년대 한국에서 쓰이던 통신공학 표준 교재. 역자서문에 따르면 "아날로그 통신 시스템에 대해서는 전부분에 걸쳐 완벽하리만큼 다루었지만, 주안점은 디지탈 시스템에 두었으며, 여러 장에 걸쳐 교환기와 컴퓨터 통신, 그리고 대역 확산 스펙트럼 등을 논의하였다" (저자서문, p. i). 2판은 "두 학기 동안 강의할 내용으로 보강"된 판으로, 약 600여 개 연습문제를 수록한다 (저자서문, p. i).

특이한 서술 전략: "이상 4개의 장에서(3장에서 6장까지)는 잡음을 배제한 상태에서 스펙트럼을 비교하고 상대적 구조적 복잡성에 대해 집중 기술한다" — 즉 AM(3장)·FM(4장)·A/D변환(5장)·디지털 변조(6장)를 먼저 잡음 없는 스펙트럼/복잡성 관점에서 비교하고, 잡음을 2장에서 수학적으로 정립한 뒤 7장(잡음의 수학적 표현)·8·9장(AM·FM의 잡음)·10~12장(착오확률·정합필터·SNR)에서 성능분석으로 이어가는 이원적 구조. 이 서술선은 [[stremler-introduction-communication-systems-3ed]](아날로그→확률→디지털의 연속 서술)와 형식 대비된다.

확률 부분도 교과서적: "통신 시스템에서의 확률적 개념의 중요성은 아무리 강조해도 지나침이 없으며, 특히 통신에 관한 논의에서 잡음의 출현과 특성은 기본적이고 필수적인 것이다" (저자서문, p. i), 2장에서 "체비세프 부등식(2.13), 가우스성 확률밀도(2.14), 레일라이 확률밀도(2.16), 중심극한정리(2.20)"까지 서술 — [[a-papoulis]]·[[probability-random-variables]]가 다룰 분포론과 겹친다.

## 장 구조 (17장, 776p)
| # | 제목 | pp. |
|---|------|-----|
| 1 | 스펙트럼 분석 (전력스펙트럼밀도, 푸리에 변환, Parseval, 상관, 직교함수·Gram-Schmitt, 신호와 벡터) | 1 |
| 2 | 확률변수와 랜덤 프로세스 (체비세프·가우스·레일라이, 랜덤 펄스열 스펙트럼) | 56 |
| 3 | 진폭변조 시스템 (주파수천이, DSB/SSB/VSB, 변조기) | 115 |
| 4 | 주파수 변조 시스템 (FM/PM, 스펙트럼, PLL, 스테레오 FM) | 146 |
| 5 | 아날로그 디지털 변환 (표본화·양자화·PCM, 적응 델타변조·선형예측 부호화, AD 변환) | 186 |
| 6 | 디지탈 변조 (M-ary PSK/QAM, M-ary FSK, MSK, Trellis-decoded modulation) | 308 |
| 7 | 잡음의 수학적 표현 (백색잡음, 필터 출력잡음) | 328 |
| 8 | 진폭변조 시스템에서의 잡음 | 344 |
| 9 | 주파수변조 시스템에서의 잡음 | ~370 |
| 10 | FM 임계치 효과 (임계치 스파이크, PLL/반송파·비트 동기) | ~390 |
| 11 | 데이터 전송 (기저대역, **정합필터 11.4 p.446**, 착오확률 11.5 p.447) | 414 |
| 12 | PCM/DM의 잡음 (SNR 비교) | ~470 |
| 13 | 정보이론과 부호화 (블록코드·반복·바이터비 알고리즘·격자복조변조/Trellis-decoded modulation) | ~520 |
| 14 | 통신시스템과 잡음 계산 (잡음온도·손실) | ~560 |
| 15 | 전화교환 (Strowger p.640·크로스바 p.648·디지털 교환기) | ~630 |
| 16 | 컴퓨터통신 (ARPANET, ALOHA·CSMA 무선패킷) | ~680 |
| 17 | 대역 확산 스펙트럼 (acquisition·direct sequence·FH·PN열) | ~720 |

(페이지는 본문 헤더/찾아보기 기반 — 5장=186p, 7장=328p, 8장=344p, 11.4 정합필터=446p, 17장=720-744p)

## 핵심 주제
- **정합필터와 착오확률** — 11.4 "백색잡음·정합필터" (p.446), 11.5 "정합필터의 착오활률" (p.447). "정합 필터의 개념이 거론되고, 착오의 확률이 시스템을 비교하는 척도로서 소개된다" (저자서문, p. ii). CDMA 이동통신 수신기 이론의 토대 → [[cdma-all]]·[[cdma-wcma-radio-analysis]](이상근, [[lee-sang-geun]])와 연결.
- **대역 확산 스펙트럼** (17장) — " Spread Spectrum: direct sequence, frequency hopping, PN sequences 730–735, acquisition 734–741" (찾아보기, p.740대). DS-SS의 이론 원전급 서술.
- **Trellis-decoded modulation** (13장, p.590–599) — TCM의 조기 서술, [[stremler-introduction-communication-systems-3ed]] 10.6 TCM/QAM과 동시대.
- **정보이론×부호화 통합** (13장) — [[coding-information-theory]](Hamming)의 Shannon 정리와 병행 독학 용.
- 약 600 연습문제 — [[stremler-comm-systems-solutions]](Stremler 풀이집)과 대비되는 "문제 중심" 교재.

## 관련
- 공식 해답집: [[taub-schilling-comm-theory-solutions]] (Taub·Schilling 원저, 김윤호 역, 17장 풀이)
- 동시대 교재: [[stremler-introduction-communication-systems-3ed]] (Stremler 3판) · [[analog-digital-communication-theory-matlab]] (MATLAB 실습) · [[practical-digital-communications-korea]] (한국어 디지털통신)
- 이론 배경: [[a-papoulis]] (확률·랜덤 프로세스) · [[probability-random-variables]] · [[signals-and-systems-oppenheim]] (스펙트럼 분석 도구)
- 확산스펙트럼 응용: [[cdma-all]] · [[cdma-wcma-radio-analysis]] · [[mobile-communication-engineering-korea]]

## 추출/OCR 신뢰도
text-layer 추출 전반 양호하나 OCR 잔존 오류 다수(예: "프로서쓰/프로세서"=프로세스, "저11/저12판"=제1/2판, "스펭트룀"=스펙트럼). 장별 페이지는 본문 헤더 숫자 기준. 원문 PDF: `/work/wiki/raw/books/taub-schilling-principles-communication-systems-2ed-trans.pdf`.
