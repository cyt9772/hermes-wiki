---
title: 실용 디지털 통신 (문호, 2000)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, telecom-systems, signal-processing, wireless-communications, coding-theory, information-theory, matlab-simulation, cdma-dsss]
sources: [raw/books/practical-digital-communications-korea.md]
confidence: high
---
# 실용 디지털 통신 (문호, 2000)

> 저자: **문호** — "방송국 엔지니어로서 10년간 산업체에서 근무한 후 대학에 [와서] 20년간 디지털통신에 대한 강의를 해온 경험과 미국 · 일본 · 독일 대학에서 연구하면서 나온 결과를 토대로" (머리말, p. iii).
> 출판: 두선 (도서출판 영일 — "도서출판 영일의 김윤수 사장님과 관계자에게 감사". 머리말). 570p. C · Matlab 부록 동반.
> 성격: "본서의 특징은 한마디로 B.Sklar와 Proakis가 지은 '디지털 통신'을 참고로 했는데, 이 책에서 다뤄지지 않은 설명이나 수식을 전부 풀어서 보완했을 뿐만 아니라 C언어나 Matlab 프로그램으로 중요한 결과를 프로그램으로 보임으로써 그 결과가 눈에 들어오도록 했다" (머리말, p. iii) — Sklar·Proakis의 디지털통신을 한국어로 해설·보완한 교재.

## 개요
"0과 1이 디지털통신에서 어떤 의미가 있는가를 풀려고 애썼다"는 포부의 디지털통신 전과정 교재. 한국 컨텍스트가 두드러진다: "기존의 아날로그 셀룰러 이동 통신에서 디지털 CDMA 이동통신시스템을 우리가 세계최초로 상용화 했고, 무선 멀티미디어 이동 통신인 IMT-2000 개발을 눈앞에 두고 있는데 그 '백본'이 되고 있는 것이 '디지털 통신' 기술이다" (머리말, p. iii).

기저대역·변조·채널 부호화·확산·암호를 한 서술로 꿰뚫는다. 특히 **정합 필터**를 2.5절(p.96)에 배치해 "정합 필터의 사용 목적은 펄스의 존재 유무를 판별하는 시점에서 신호 성분을 증가시키고 잡음 성분을 감소시키는 것이다" (2.5 정합 필터, p.96~104)로 명제화 — [[stremler-introduction-communication-systems-3ed]] 7.11·[[taub-schilling-principles-communication-systems-2ed-trans]] 11.4에서 같은 내용을 영어로 다루는 대목과 대응.

부호화 편에서는 차세대 무선통신 맥락을 앞세운다: "기존의 convolutional code / Reed-Solomon 연접 부호와 1993 년에 발표된 터보 부호（Turbo Code）를 채택하려는 것을 알 수 있다" (제5장 도입, [표 5-5] 차세대 무선 멀티미디어 통신을 위한 채널 코딩 기법) — 5.6절 "IMT-2000의 Turbo Codes의 반복 복호기" (p.327)에서 Interleaver/Deinterleaver 구조와 반복 복호까지 서술. 2000년 시점의 IMT-2000(3G) 채널 코딩 전망서적 성격.

## 장 구조 (9장 + 부록, 570p)
| # | 제목 | pp. |
|---|------|-----|
| 1 | 디지털 통신의 개요 (신호 종류, 스펙트럼 밀도, 자기상관, 랜덤 신호, 선형시스템 전송, 디지털 데이터 대역폭) | 9–59 |
| 2 | 신호 포맷팅과 기저대역전송 (PCM·양자화, AWGN 검파, **정합 필터 2.5**, 기저대역 비트 에러확률, ISI, 등화기, 부분응답) | 59–138 |
| 3 | 변복조 이론 (통과대역 변조, 동기/비동기 검파, 이진·M-ary 오차확률) | 141–232 |
| 4 | 채널 부호화 Ⅰ — 파형 코딩, 선형 블록 부호, 부호화 능력, 순환 부호, 블록 부호 (Hadamard 등) (4.1~269, 5장 297~) | 233–296 |
| 5 | 길쌈 부호화 (convolutional code, Viterbi 복호, 성능 한계, 인터리빙, **IMT-2000 Turbo 복호기 5.6 p.327**, 결론 p.342) | 297–350 |
| 6 | 변조와 부호화의 교환 (오차확률평면, 나이키스트 최소대역폭, **샤논 채널용량 6.4**, 대역폭효율평면, QAM, **TCM 6.8 p.379**) | 351–406 |
| 7 | 동기화 및 다중화 (동기 p.407, 다중화 p.433) | 407–452 |
| 8 | 대역확산 기법 (DS-SS, 가상잡음열, 주파수도약, 동기화, 전파방해) | 453–492 |
| 9 | 암호화와 복호화 (블록/스트림/공개키 암호) | 493–564 |
| 부록 | Fourier Transform · 통계적 신호판단이론의 기초 · 디지털통신/컴퓨터스위칭/퍼지논리 세계 최초 정낭(?) | 565–576 |

## 핵심 주제
- **정합 필터 + 비트오차확률** (2.5·2.6, p.96–109) — "에러 확률을 가장 적게 하는" 최적 수신기, AWGN 검파(2.4 p.93)와 직결.
- **터보 부호·반복 복호** (5.6, p.327) — 1993년 발표된 터보 부호의 IMT-2000 적용 논의(원문: "1993 년에 발표된 터보 부호（Turbo Code）를 채택하려는 것을 알 수 있다" — 제5장 도입부·[표 5-5] 차세대 무선 멀티미디어 통신 채널 코딩 기법, p.297~300대); 부록 III에 Viterbi 알고리즘 프로그램 제공(머리말, p. iv).
- **TCM(격자 부호 변조)** (6.8, p.379) — 변조와 부호화의 결합, [[stremler-introduction-communication-systems-3ed]] 10.6 QAM/QPSK와 동제목.
- **대역확산(DS/FH)** (8장) — CDMA 원리, [[cdma-all]]·[[mobile-communication-engineering-korea]] 10장(디지털 CDMA 셀룰라)과 이어짐.
- MATLAB/C 실습 — "C언어나 Matlab 프로그램으로 중요한 결과를 프로그램으로 보임" — [[analog-digital-communication-theory-matlab]]·[[computer-based-exercises-signal-matlab]]과 같은 실습형 계열.

## 관련
- 저자: [[moon-ho]] (〈C 언어 영상통신의 신호처리〉(대영사 1999) 저자; 본서 머리말의 자매편 "C언어를 이용한 영상신호처리(1994)" "C언어·Matlab을 이용한 디지털 필터설계(1997)" "실용 정보이론(1998)"과 동일한 필자)
- 디지털통신 교재군: [[stremler-introduction-communication-systems-3ed]] · [[taub-schilling-principles-communication-systems-2ed-trans]] · [[analog-digital-communication-theory-matlab]]
- 확산/이동통신: [[cdma-all]] · [[mobile-communication-engineering-korea]] · [[latest-mobile-comm-systems]]
- 코딩이론: [[coding-information-theory]] (길쌈·블록 부호의 이론 배경)

## 추출/OCR 신뢰도
text-layer 양호, 목차·머리말 가독성 높음. 일부 토큰 깨짐(예: "디 작,1 확산 기법"=대역확산 기법, `…Coi…nal Code` = convolutional Code). 원문 PDF: `/work/wiki/raw/books/practical-digital-communications-korea.pdf`.
