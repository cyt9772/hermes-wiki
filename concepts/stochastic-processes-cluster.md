---
title: 확률·랜덤 프로세스 클러스터 (_probability cluster_)
created: 2026-10-25
updated: 2026-10-25
type: concept
tags: [concept, stochastic-processes, signal-processing]
sources: [raw/books/probability-random-variables.md, raw/books/probability-random-process.md, raw/books/discrete-random-signals.md]
confidence: high
---
# 확률·랜덤 프로세스 클러스터 (2026-10-25, 3권)

같은 "공학 확률" 주제를 서로 다른 위치에서 파는 3권의 축을 정리: **고전 이론 축(Papoulis)** vs **통신 응용 축(Leon-Garcia)** vs **이산시간·최적화 축(Therrien)**. 공통 토대는 확률행렬·마르코프·가우시안 프로세스·파워 스펙트럼 4개다.

## 3권 비교

| 항목 | [[probability-random-variables]] (Papoulis, McGraw-Hill 1991, 682p) | [[probability-random-process]] (Leon-Garcia, 613p) | [[discrete-random-signals]] (Therrien, Prentice Hall, 751p) |
|---|---|---|---|
| 목표 독자 | EE·통신 대학원, 수학 기반 중 | EE/CS 학부~대학원, 설계 도구 중 | 대학원, 확률론·선형대수 선급 |
| 수준 | 공리→특성함수→극한정리, **이론 체제** | 모델→예제→성능, **통신 해석** | 랜덤 벡터→최적필터, **최적화 이론** |
| TOC 구조 | 2부 16장: 부I 확률론(장1~9) / 부II 확률과정(장10~16) | 9장: 확률모델(1)→확률/변수(2~5)→**랜덤 프로세스(6)·랜덤 신호(7)·마르코프(8)·큐잉(9)** | 10장+부록: 랜덤벡터(2)→프로세스(3)→2모먼트(4)→**변환(5)·추정(6)·최적필터(7)·선형예측(8)·선형모델(9)·스펙트럼추정(10)** |
| 중심 도구 | **특성함수**(장5 p.115, 장7 결합) | CDF·벡터분포 + PSD(장7) + 마르코프·큐잉 | 2모먼트 행렬 **스펙트럼 인자화·Wold 분해**(장이해 p.249·p.390) |
| 스펙트럼 다룸? | 장10 파워 스펙트럼 + 장13 스펙트럼 추정(이론) | 장7 PSD + LTI 통관(통신 관점) | 장10 스펙트럼 추정(최대우도·서브스페이스, **알고리즘**으로 다름) |
| 추정·필터링 포함? | 장14 평균제곱 추정(개요) | 장4.9★ 개요 수준 | 장6~7 **전체**(베이스·LSMSE·FIR/IIR 최적) |

## 공통 축 (3권에 전부 등장)
1. **가우시안 프로세스** — Papoulis 장10-8(가우시안 과정), Leon-Garcia 장4.8·4.9, Therrien 장3.8(gaussian process)·장5.7(LS 변환과 가우시안). Therrien은 "가우시안이라면 모든 고저 모먼트는 2모먼트로 정화된다"를 반복 강조.
2. **마르코프 프로세스** — Leon-Garcia 장8(체인), Therrien 장3.5(이산 + 연속 시간). Papoulis는 부II에 짧게.
3. **스펙트럼(PSD)** — 3권 모두 랜덤 신호의 주파수적 표현으로 등장. 차이는 **다루는 깊이**: Leon-Garcia는 "잡음 통과(장7)"까지, Papoulis는 스펙트럼 추정 이론(장13), Therrien은 스펙트럼 인자화→Wold→ALC로 최적필터·최종적으로 **스펙트럼 추정 알고리즘**(장8.9, 장10)로 닫는다.
4. **랜덤 벡터·다변수 분포** — Therrien 장2가 전부(고스 밀도 p.43, 역전, 유니터리 대각화), Leon-Garcia 장4, Papoulis 장6~7.

## 클러스터 내부 논리
- **순차 독학 경로**: Leon-Garcia(모델+예제, 1학기) → Papoulis(특성함수·극한정리, 확실히 이론) → Therrien(이산시간·최적화, 확률을 **최적화 도구**로 쓰는 관점).
- Therrien 장1 서문 "정규화 랜덤 프로세스를 이산시간 관점에서 새로 시작한다" — Leon-Garcia·Papoulis가 연속시간 기본에서 이산으로 확장한다면, Therrien은 **이산이 기본**이라 이 클러스터는 "이산 기본"과 "연속 기본"의 두 관점을 대조하는 축.
- 이 세 권의 하류는 [[estimation-and-filtering]] — 추정은 확률+선형대수의 합이므로, 3권 모두가 그 전제.
- 인접: [[information-coding-theory]](장15 엔트로피·추정↔코딩 대칭), [[cdma-dss-spread-spectrum]](랜덤 신호·스펙트럼 실용), [[digital-signal-processing]](랜덤 신호 처리의 연속·이산 대조).
