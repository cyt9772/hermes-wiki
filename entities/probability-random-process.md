---
title: Probability and Random Processes for Electrical Engineering (2nd ed)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, signal-processing, stochastic-processes, engineering-mathematics]
sources: [raw/books/probability-random-process.md]
confidence: high
---
# Probability and Random Processes for Electrical Engineering (2nd ed)

> Alberto Leon-Garcia, McGraw-Hill, 613p. EE/CS 학부~대학원 대상 확률·랜덤 프로세스 교과서 — **통신 시스템 예제**를 각 장에 심어 이론을 실용으로 붙이는 편성 `[raw/books/probability-random-process.md]`.

## 개요
장 1은 "통신·컴퓨터공학에서 수학 모델이 왜 도구인지를" 묻기 시작(패킷 음성 전달 상세 예제, 1.4) — 확률 모델을 **설계 도구**로 쓰는 관점이 책 전체를 지배. 이후 기본 확률론(장 2~5) → 랜덤 프로세스(장 6) → 랜덤 신호 처리(장 7) → 마르코프(장 8) → 큐잉(장 9)으로 "통신 시스템 해석"을 위한 최소 확률론을 조립 `[raw/books/probability-random-process.md]`.

## 장 구조 (원문 TOC 기준, 9장)
1. **Probability Models in ECE** (p.1) — 결정 모델 vs 확률 모델, 통계적 정규성, 확률의 공리적(axiomatic) 접근. 예제: 패킷 음성 전달(1.4), 불안정 채널 통신, 랜덤 신호 처리, 자원공유, 신뢰성
2. **기본 확률론** (p.~23) — 표본 공간(sample space), 사건, 공리, 계산용 센팅법(counting), 조건부 확률·베이츠, 독립, 순차 실험(이항·다항·기하), 랜덤 수 생성(★)
3. **Random Variables** (p.84) — CDF, 3종류의 RV, PDF, 조건분포, 주요 RV(불연속·연속)
4. **Multiple Random Variables** — 벡터 RV, 조건부, 이변수/다변수, 결합 CDF, PDF, 특성함수, **고스 RV**(4.8), 고스 벡터 선형변환, 평균제곱 추정(★4.9), 상관 벡터 생성(★4.10)
5. **Sums of Random Variables and Long-Term Averages** (p.269) — 합, 평균·분산, 독립합의 PDF, **샘플평균과 대수의 법칙**(5.2), **중심 극한 정리**(5.3), 신뢰구간(★5.4), 수렴, 장시간 도착률
6. **Random Processes** (p.329) — 정의, 1·2모먼트 특성
7. **Analysis and Processing of Random Signals** (p.403) — **파워 스펙트럼 밀도(PSD)**, LTI 통과, 잡음 통과
8. **Markov Chains** (p.459) — 마르코프 프로세스, 체인
9. **Introduction to Queueing Theory** (p.499) — 큐의 구조, 도착·서비스 분포, 성능 지표 `[raw/books/probability-random-process.md]`

## 핵심
- 매 장 **통신 예제**가 선두 — 장 1은 "패킷 음성 전달 시스템" 전체를 확률 모델로 씀. 이론-설계를 나란히 두지 않고 예제에서 이론으로 `[raw/books/probability-random-process.md]`
- **고스(가우시안) RV·벡터**(장 4.8~4.10)와 **PSD**(장 7)가 이 책의 핵심 축 — Papoulis [[probability-random-variables]]가 특성함수 중심이라면, 이 책은 **벡터 분포 + 스펙트럼** 중심(통신 관점). [[stochastic-processes-cluster]] 비교표에서 "수준" 열의 대표
- **마르코프 체인(장 8) + 큐잉(장 9)**을 확률론 교과서에 포함 — Papoulis·Therrien에는 없는 성능 모델링 축. 통신/네트워크로 확장되는 지점
- 장 5 CLT·대수법칙 + 장 7 PSD는 신호-시스템 축([[signals-and-systems-oppenheim]] 장 11 피드백 → 랜덤 세계)에 이은 "무작위 신호 해석"의 교과서적 관문

## Related
- 저자: [[alberto-leon-garcia]]
- 클러스터: [[stochastic-processes-cluster]] — [[probability-random-variables]](고전/특성함수)와 [[discrete-random-signals]](이산·최적화) 대비
- 개념: [[digital-signal-processing]] · [[cdma-dss-spread-spectrum]] (랜덤 신호 + 스펙트럼 관점)
- **해답집**: [[leon-garcia-probability-random-processes-2ed-instructor]] — Instructor Manual (246p), 2nd ed. Ch.2–5(기본 확률론·랜덤변수·다변수·합) 장별 문제 풀이
