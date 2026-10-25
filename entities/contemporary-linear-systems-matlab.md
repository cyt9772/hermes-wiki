---
title: Contemporary Linear Systems Using MATLAB 4.0
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, state-space-control, signal-processing, matlab-simulation]
sources: [raw/books/contemporary-linear-systems-matlab.md]
confidence: high
---
# Contemporary Linear Systems Using MATLAB 4.0

> Robert D. Strum · Donald E. Kirk — PWS Publishing, 1996, 699p. **MATLAB 4.0 기반 선형시스템 "컴퓨터-바이어스(computer-biased)" 교과서** — "we have used a 'computer-biased' approach in which computer solutions and theory are viewed as mutually reinforcing rather than as an either-or proposition. We adhere to the axiom that one learns by doing rather than by listening, and, consequently, more than 200 problems are provided for the reader to solve" (Preface) [raw/books/contemporary-linear-systems-matlab.md].

## 개요
"이론과 MATLAB 구현을 독립 항목으로 분리하지 않고 한 흐름에 통합"하는 선형시스템서. 전제 조건: 미적분·미분방정식·복소수·행렬 연산 + "첫 번째 전기공학 과정의 배경" (Preface). 1–9장 + Appendix A(MATLAB: An Overview, p.659) + B(Useful Formulae, p.665) + Index(p.667). 장 1 서두: "Reasons for studying linear systems theory; Mathematical description and MATLAB generation of important signals and sequences; A road map of domains, models, and operations; Use of displot and plot for graphing" (p.1) [raw/books/contemporary-linear-systems-matlab.md].

## 장 구조 (TOC 기준, 9장 + Appendix A·B)
1. **Signals and Sequences** (p.1) — 학습동기, 신호·시퀀스 MATLAB 생성, 도메인·모델 로드맵, displot/plot
2. **Continuous Systems** (p.37) — 특성, 컨볼루션, 임펄스응답, 시수스 주파수응답, 상태공간, conv 시뮬레이션
3. **Systems** (p.491) — 라플라스·전달함수·모델 계열
4–6. *(중간 장: Fourier Series, State-Space Topics, 등 — TOC 일부 가독 불가)*
7. **Discrete Systems** (p.363) — 컨볼루션, unit sample response, 시수스 주파수응답, 상태공간
8. **Discrete-Time Systems** (p.615) — 이산시간 상태공간, 디지털 제어, MATLAB 4.0 구현
9. **Digital Control** (p.615~) — P8.x 문제들, 상태공간 디지털 제어
+ Appendix A MATLAB: An Overview (p.659) · B Useful Formulae (p.665) · Index (p.667)

## 핵심
- **"Computer-biased" 접근법** — MATLAB을 "부록이 아닌 본문"으로, 이론과 코드를 **각 장 안에서 교차 제시**. 이 관점은 [[contemporary-linear-systems-matlab]]이 1990년대 "MATLAB 교과서"류(선형시스템·신호처리)의 원형 중 하나인 이유
- **200+ 문제 + 250+ MATLAB 예제** — 전제 조건(미분방정식·행렬)을 갖춘 독자를 위한 "실습 중심" 설계. [[computer-based-exercises-signal-matlab]](신호처리 실습)과 대비: 이 책은 **선형시스템·제어** 쪽
- **Continuous → Discrete → Digital Control 3단 구조**(장 2→7→8)는 [[signals-and-systems-oppenheim]](이론)의 "연속시간→이산시간" 흐름을 MATLAB으로 **구현 가능하게 재구성**
- 라플라스·상태공간·컨볼루션 3개 도구를 **각 시스템 유형(연속/이산)에 매핑**하는 표(road map, 장 1)가 이 책의 핵심 도면

## 저자·관련
- 저자: Robert D. Strum, Donald E. Kirk (별도 페이지 없음)
- 개념: [[linear-system-control]] · [[digital-signal-processing]] (이산시간·디지털 제어 접점)
- 인접: [[linear-system-theory-design]] (Chen, 이론심화) · [[linear-system-theory-design-3ed]] (Chen 3rd ed) · [[computer-based-exercises-signal-matlab]] (신호처리 실습서) · [[signals-and-systems-oppenheim]] (이론서) · [[mimo-ofdm-wireless-matlab]] (MATLAB 시뮬레이션 같은 클러스터)
