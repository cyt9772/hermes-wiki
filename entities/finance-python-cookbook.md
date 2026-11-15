---
title: 금융 파이썬 쿡북 (Python for Finance Cookbook)
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, python, finance, monte-carlo, risk]
sources: [raw/books/finance-python-cookbook.md]
confidence: medium
---

# 금융 파이썬 쿡북 (Python for Finance Cookbook)

> 표지: '금융 데이터 처리와 기술 분석부터 딥러닝 적용까지' (p1)

## 개요
- **저자:** 에릭 르오션(?), 옮긴이 크라스랩 (p1, p4)
- **출판:** Packt Publishing 2020 원서, 에이콘출판(주) 2021 한국어판, 494쪽 (p3)
- **성격:** 파이썬으로 금융 데이터 처리·기술 분석·리스크(VaR/ES)·자산 배분·딥러닝(LSTM/GRU)까지 레시피(문제→코드)로 풀이하는 실전 쿡북 (p1, p4).

## 내용
- 포트폴리오 VaR: '1일 포트폴리오 값과 그로 인한 차이을 계산하고 오름차순으로 정렬했다. X% VaR은 단순히 정렬된 포트폴리오 차이의 (1-X)% 번째 백분위 수다' (p255).
- 은행 VaR 관행: '은행은 종종 1일 및 10일 VaR을 계산한다. 후자의 경우 1일 VaR을 계산하고 10의 제곱근을 곱할 수도 있다. 이 계산을 자본 요구 사항을 낮추는 방향으로 활용하면 은행에 도움이 될 수 있다' (p256).
- VaR 단점: '모수 분포를 가정한다(분산·공분산 방식). 꼬리 위험을 충분히 포착하지 못한다. 이른바 블랙 스완(Black Swan) 이벤트를 고려하지 못한다(과거 샘플에 없는 경우가 아니라면). 과거 VaR은 새로운 시장 상황에 적응에 느릴 수 있다' (p256).
- Expected Shortfall(ES): '임계값을 초과할 때 잠재적 손실의 크기에 대한 정보를 포함하지 않는다는 것. 이는 예상 부족(Expected Shortfall, 조건부 VaR 또는 꼬리 손실이라고도 한다)이 작동하는 시점이다. 이는 시나리오의 최악의 x%에서 예상되는 손실이 무엇인지 간단히 설명한다' (p256).
- 딥러닝: '포겟 게이트: 시그모이드 함수를 사용해 유지할 정보(1에 가까운 시그모이드 값) 또는 망각(0에 가까운 값) 정보를 결정한다. 이 함수는 현재의 입력과 이전 은닉 상태에 적용된다' — LSTM 게이트 구조를 RNN·GRU와 비교 (p486–487).

## 관련 페이지
- [[finance-recipes]] — 파이썬 금융공학 레시피
- [[deep-learning-tensorflow-keras]] — 신경망 아키텍처 실전
- [[wise-quant-investing]] — 퀀트 투자·포트폴리오
