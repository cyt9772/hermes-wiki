---
title: PSpice 회로 시뮬레이션 (Circuit Simulation with PSpice)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [circuit-simulation, electronic-circuits, engineering]
sources: [raw/books/introduction-to-pspice.md]
confidence: high
---
# PSpice 회로 시뮬레이션 (Circuit Simulation with PSpice)

## 정의
**SPICE(Simulation Program with Integrated Circuit Emphasis) 계열 소프트웨어로 디지털/아날로그 회로를 컴퓨터에서 해석하는 실무 기법**. PSpice는 UC Berkeley Electronics Research Laboratory가 개발한 SPICE를 MicroSim Corporation이 상용화한 버전(PSpice·Probe 포함, 등록 상표). 이 클러스터의 중심서 [[introduction-to-pspice]](Nilsson·Riedel, 1993)는 PSpice를 **회로 해석 교과서**(*Electric Circuits* 4판)에 통합하는 실무서로, "PSpice 프로그램 작성 → 기본 소스 모델 구성 → 컴퓨터 출력 검증" 3단계를 가르친다.

## 핵심 절차 (introduction-to-pspice 기준)
1. **Source file 구성** — 3종 문장: Data statements(소스·소자 정의), Control statements(.OP·.DC·.TF·.SENS·.TRAN·.AC), Output statements(응답 변수).
2. **DC 해석** — .OP(정지점), .DC(소스 스윕), .TF(이득·입출력 임피던스), .SENS(민감도).
3. **과도 해석** — .TRAN, 지수 펄스 소스, natural response, step response, piecewise linear 소스, V/C 제어 스위치.
4. **AC·주파수 해석** — 정현파 소스, AC steady-state, AC power with Probe, frequency response + Bode plot, Fourier series.
5. **특수 소자** — **op amp 모델링 3단계**(저항+종속소스 → subcircuit → library model), mutual inductance, 이상적 변압기.
6. **검증** — "PSpice 출력 데이터를 검증하여 컴퓨터 해가 알려진 회로 동작의 관점에서 합당한지 확인" — 67문제의 2대 목적 (Preface).

## SPICE ↔ PSpice
- SPICE: UC Berkeley 원본, 리서치용.
- PSpice: MicroSim 상용화 — PSpice Control Shell, Probe 메뉴, library model 제공. Appendix C에서 "Differences between SPICE and PSpice" 명시.

## 학습 포인트
- **출력 검증 습관** — 시뮬레이터 출력은 항상 물리 직관(주어진 회로 동작)으로 검증해야 한다.
- **op amp 모델링** — 서브회로로 이상 op amp를 구성, library model로 실용 op amp를 시뮬레이션.
- **부록 활용** — Control Shell & Probe 메뉴 가이드(A), 시뮬레이션 파라미터(B), SPICE↔PSpice 차이(C), Quick Reference(D).
- **교과서 마진 마크** — *Electric Circuits* 4판 마진의 색 마크 ↔ 이 실무서의 대응 섹션.

## 관련 개념 (이 wiki)
- **기존 이론서와의 결합**: [[dc-ac-circuit-analysis]] (DC/AC 회로이론) · [[laplace-transform-circuits]] (S-평면·전달함수) · [[amplifiers-analog-circuits]] (증폭기) · [[circuits-diagnosis-practice]] (회로 진단 실무) · [[timer-oscillator-circuits]] (타이머·발진 회로)
- **모 교과서**: [[nilson-riedel-electric-circuits]] (PSpice 서의 모 교과서)
- **회로 인접**: [[intro-electronic-circuits]] · [[theory-of-circuits]] · [[circuits-and-systems]]
- **실무**: [[practical-electronics-eng]] (실무 전자공학)
- **인접 클러스터**: [[dct-algorithms-applications]] (전환 부호) · [[ofdm-orthogonal-frequency-division]] (무선 적용)

## 미해결 논쟁 / 현재 지식
- **SPICE 계열의 현재 지위** — LTspice·ngspice·PSpice(Ansys)가 대등한 위치. 1993년 PSpice/Probe 환경은 현재와 메뉴·명령이 다름.
- **검증 습관**은 여전히 유효 — 시뮬레이션 오류(수렴 실패, 이상 소자)는 물리 직관으로 검증해야 한다.

## Related
- 책: [[introduction-to-pspice]] · [[nilson-riedel-electric-circuits]]
- 저자: [[james-w-nilsson]]
- 태그: `circuit-simulation` · `electronic-circuits` · `electrical-engineering`
