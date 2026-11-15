---
title: 파이썬과 케라스를 이용한 딥러닝/강화학습 주식투자
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, deep-learning, LRL]
sources: [raw/books/dl-rl-stock-investing.md]
confidence: medium
---

# 파이썬과 케라스를 이용한 딥러닝/강화학습 주식투자

> 표지: '알고리즘 트레이딩을 위한 케라스를 이용한 최첨단 해법 입문 / 파이썬과 케라스를 이용한 딥러닝/강화학습 주식투자' (p1, p4)

## 개요
- **저자:** 박찬규 / 이대엽 / 전이주 (p3)
- **출판:** 위키북스, 초판 2020년 4월 27일, ISBN 979-11-5839-203-1 (p3) | **양:** PDF 323쪽
- **성격:** 알고리즘 트레이딩을 위해 파이썬 + 케라스로 딥러닝과 강화학습을 실전(주식 시장)에 적용하는 실전서. 예제 코드는 `wikibook.co.kr/dltrading-rev/`와 `github.com/quantylab`에서 다운로드 가능 (p3, p323).

## 내용
- 구성: RLTrader(강화학습 주식투자 시뮬레이션 프로그램) 모듈 개발 — 5.1 RLTrader 개발 환경 setup(Anaconda, PlaidML) p98~101, 5.2 RLTrader2 설계·커스터마이징 p117~ 등을 다룬다 (p11, p16).
- 학습 대상: 'RLTrader: 실제 주식 데이터에서 수많은 반복적 투자를 통해 더 좋은 투자 정책'을 학습하는 강화학습 시뮬레이션 도구 (p115).
- 주식 시세·주문 등 증권사 API(키움, 대신증권 등)를 연결해 실무 트레이딩 시스템 구축을 다루며, 저자는 대신증권 API를 '가장 직관적이고 구현하기 쉬웠다'고 평가 — '거듭 말하지만 저자는 위 증권사들과 어떤 이해관계가 없음을' 밝힌다는 공정성 고지를 함께 수록 (p233~242).
- 학습 단위 개념 정립: '대상 데이터 전부를 대상으로 한 차례 반복하는 과정을 에포크(epoch)라고 합니다. 100번' — 에포크(run) 개념을 반복 학습과 함께 설명한다 (p109).

## 관련 페이지
- [[python-keras-reinforcement-learning]] — 케라스로 강화학습을 배우는 게임 AI 실전서
- [[rnn-time-series-advanced]] — 시계열·주식 예측 딥러NING 계열
- [[python-financial-analysis]] — 파이썬 금융 데이터 분석
- [[pakhomxi-investing]] — 투자 전략·포트폴리오 계열
- [[naver-securities]] — 증권 데이터 API·주식 시세 계열
- [[stock-university-real-strategy-3]] — 실전 주식 트레이딩 전략 계열
- [[dl-rl-stock-investing]] 제외: [[dividend-king]] — 배당·장기 투자 전략 계열
