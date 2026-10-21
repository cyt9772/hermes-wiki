---
title: 증폭기·아날로그 회로 (Amplifiers & Analog Circuits)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [electrical-engineering, electronic-circuits, signal-processing]
sources: [raw/books/new-electronics.md, raw/books/intro-electronics.md]
confidence: medium
---
# 증폭기·아날로그 회로 (Amplifiers & Analog Circuits)

## 정의
**전력(진폭)을 키워주는 전기 회로 + 그 부속 기능(바이어스·되먹임·발진·연산)**. 비선형 소자(트랜지스터·FET·연산증폭기)를 선형 동작점에 놓아 증폭 특성을 얻는 회로 설계의 총칭. 두 기술평가 수험서(신전자공학·전자공학입문)의 핵심 영역이며, 현대 표준서(practical-electronics ch.16 오디오)와의 공통 토대.

## 트랜지스터(BJT) 증폭회로 (new-electronics 제4장, intro-electronics 제4~5장)
- **동특성과 등가회로** — 정특성 곡선군에서 동작점(Q-point) 설정; **T형 등가회로**·**h-상수(hybrid) 등가회로** 두 모형으로 게인·입력/출력 임피던스 분석 `^[raw/books/intro-electronics.md]`
- **주요 특성** — 온도·주파수에 따른 h-상수 변화, **잡음 특성**, **일그러짐률(왜곡)**
- **바이어스 회로** (new-electronics 4-3) — 고정 바이어스 → 자체 바이어스 → **전류 되먹임형** → **전압 되먹임형** + 안정지수. Q점의 온도 안정화는 바이어스 설계의 핵심
- **저주파 증폭**(so신호/대신호)·**고주파 증폭**(하이브리드 π형 등가, **중화 회로**로 자기발진 방지, 고주파 한계)·**직류 증폭**(직접결합, 변조형, **차동 증폭회로**)·**광대역 중폭**(저역/고역 보상, 비디오 증폭, 중간 주파 증폭)
- **되먹임 증폭** (intro-electronics 제5장) — 전압 되먹임(출력 임피던스 ↓) / 전류 되먹임(출력 임피던스 ↑)으로 선형화·안정화
- **전력 증폭** — **A급**(정량)·**B급 푸시풀**(추-인, 양방향 증폭), 푸시풀 연결로 효율·왜곡 타협
- **이미터 접지** 및 **이미터 follower**(에미터 팔로어, 전압 팔로어)

## FET·MOSFET 증폭회로 (new-electronics 제5장, intro-electronics 제5장)
- **JFET** — 구조(채널·게이트 편압), **전달 특성**·**드레인 특성** 곡선, 고정/자체 바이어스
- **MOSFET** — **공핍형(depletion)**/**증가형(enhancement)** 구조·특성 차이, 각형별 바이어스 회로
- **FET 증폭회로** (intro-electronics 5-3) — 전압 제어 소자라 입력 임피던스가 BJT보다 높음
- MOSFET은 "이미터(소스) 전극이 많을수록 집적도 높음" — 디지털 MOS 논리로의 다리 `^[raw/books/intro-electronics.md]`

## 연산증폭기(Op-amp) 회로 (new-electronics 제6장, intro-electronics 제6장)
- **차동 증폭기** — 1단자 접속·차동 동작·**동상(동극성) 동작**, 입력/출력 저항, **동상 성분 제거**
- **가상 접지(virtual ground)** 개념 → **일정 이득 회로**(비전달/전달 증폭), **가산기 회로** `^[raw/books/new-electronics.md]`
- **응용**(intro-electronics 6-4) — **부호 변환(인버터)**, **덧셈기**, **고입력 저항 차동 증폭기**, **미분·적분 회로**, **가변 표준(정전압) 전원**
- **소자 계통별 op-amp** (new-electronics 6-3) — 바이폴라 / **BiFET** / **BiMOS** 연산증폭기 비교
- digital-electronics 13장·Levine Exp 15·16에서도 op-amp가 D/A·A/D 변환의 구성 단위로 등장 — 아날로그-디지털 경계의 공통 소자

## 발진회로 (new-electronics 제7장, intro-electronics 제7장)
- **발진의 원리와 조건**(반데르크 발진 조건 계열) — 양성 되먹임 루프
- **사인파** — **LC 발진**(하아틀리/Hartley·콜피츠/Colpitts), **수정발진**(수정 진동자), **CR(RC) 발진**(이상형·브리지형/빈 브리지)
- **비사인파** — **톱날파 발진**, **블로킹(Blocking) 발진**, **멀티바이브레이터**(무안정/단안정/양안정)
- **초고주파 발진기**(intro-electronics 7-5) — **마그네트론**, **클라이스트론** 등 UHF 발진관

## Related
- [[semiconductor-devices]] — 증폭기의 소자 기반(트랜지스터·FET)
- [[digital-logic-basics]] — MOS 증폭 → MOS 논리로(디지털 경계)
- [[timer-oscillator-circuits]] — 발진기·555 타이머(Levine Exp 12에서 IC 타이머)
- [[analog-filter-design]] — 주파수 응답·보상 회로
- [[power-supply-regulation]] — 정전압·정류·평활(두 수험서 3장/9장)
- 관련 책: [[new-electronics]], [[intro-electronics]] (주 소스), [[digital-theory-experimentation]] (Exp 15 op-amp), [[practical-electronics-eng]] (오디오 증폭)
