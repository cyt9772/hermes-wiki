---
title: Probability and Random Processes for EE (2nd ed.) — Instructor Manual (Leon-Garcia)
created: 2026-10-25
updated: 2026-10-25
type: book
tags: [book, stochastic-processes, probability, instructor-manual]
sources: [raw/books/leon-garcia-probability-random-processes-2ed-instructor.md]
confidence: high
---
# Probability and Random Processes for EE (2nd ed.) Instructor Manual

> Alberto Leon-Garcia, McGraw-Hill — [[probability-random-process]](2nd ed., McGraw-Hill 613p)의 Ch.2–5(기본 확률론·랜덤변수·다변수·합) 장별 문제 풀이, 246p `[raw/books/leon-garcia-probability-random-processes-2ed-instructor.md]`(표지 p.1, "Instructor Manual Probability and Random Processes for Electrical Engineering Second Edition").

## 개요
원서 부 기본 확률론(Ch.2~5) 문제집 풀이. 각 장 서두 표제만 나열하고 곧바로 문제 풀이(`2.1 a) S={1,2,3,4,5,6}` p.2)가 시작되는 해법집 형식 — "2.2 The outcome of this experiment consists of a pair of numbers (x, y) where x = number of dots in first toss and y = number of dots in second toss. Therefore, S = set of ordered pairs (x, y)..."(p.2)처럼 표본 공간 구성부터 단계 전개. Ch.5 후반(5.8 Problems Requiring Cumulative Knowledge)에서는 "The long term bit rate S ... will approach the entropy of the source with probability 1."(5.8(c), p.245)처럼 확률론→정보이론(엔트로피)으로 넘어가는 종합 문제가 실려 있음.

## 구성 (246p)
- **Ch.2 Basic Concepts** (p.2~): 표본 공간·사건·공리(2.x 순)
- **Ch.3 Random Variables** (p.46~): CDF·PDF, 3종류 RV, 분포 함수
- **Ch.4 Multiple Random Variables** (p.129~): 벡터 RV, 결합 분포, 특성함수, 가우시안
- **Ch.5 Sums & Long-Term Averages** (p.208~): 합과 공분산 — "VAR(X+Y+Z) = VAR(X)+VAR(Y)+VAR(Z) + 2COV(X,Y)+2COV(X,Z)+2COV(Y,Z)"(p.208), CLT·대수의 법칙, 5.8 종합 문제까지(p.246)
- 원서 Ch.6~9(Random Processes·PSD·Markov·Queueing)는 본 매뉴얼에 **없음** — 이 4장에 해당하는 해법은 원서 companion 자료로 별도 취급 필요

## 활용
- [[probability-random-process]] Ch.2–5 문제 대조 1차 자료. 수식 추출 깨짐은 중간 수준 — 정답 대조 시 로컬 원본 PDF(`/work/wiki/raw/books/leon-garcia-probability-random-processes-2ed-instructor.pdf`) 확인
- CLT·에르미트 공분산(Ch.5)은 [[stochastic-processes-cluster]]의 공통 축, Ch.4 특성함수는 [[probability-random-variables]](Papoulis)와 비교
- [[discrete-random-signals]](Therrien)의 확률 배경과 같은 주제인데 Papoulis보다 예제 중심으로 편성 — 이 매뉴얼의 풀이도 실용적

## Related
- 원서: [[probability-random-process]] (Leon-Garcia 2nd ed.)
- 저자: [[alberto-leon-garcia]]
- 개념/클러스터: [[stochastic-processes-cluster]] · [[probability-random-variables]](해법집 버전 별도)
