---
title: 실전 알고리즘 트레이딩 레벨업
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, quant, trading, backtesting, zipline]
sources: [raw/books/algorithm-trading-levelup.md]
confidence: medium
---

# 실전 알고리즘 트레이딩 레벨업

> 파이썬 백테스트 활용 — Andreas F. Clenow 저, 이기홍 역 (p5)

## 개요
- **저자:** Andreas F. Clenow (안드레아스 F. 클레노우) — 스위스 취리히 기반 자산운용 매니저, 기업가, 헤지 펀드 매니저; 저서 《Following the Trend》(Wiley, 2013), 《Stocks on theMove》(2015) (p8)
- **옮긴이:** 이기홍 — 카네기멜론대 석사, 피츠버그대 Finance Ph.D., CFA·FRM, 삼성생명·HSBC·새마을금고중앙회·한국투자공사 등에서 포트폴리오 매니저 (p10)
- **출판:** 에이콘출판, Korean Edition © 2022 (원서 2019, ISBN 9781091983786), 509쪽 (p4, p2)
- **성격:** 아이디어를 백테스트·구현하는 방법을 Zipline·PyFolio·Empyrical로 처리하는 실전 책 (p11).

## 내용
- 옮긴이의 말: "갖고 있는 아이디어를 어떻게 백테스트하고 구현하는가를 설명하는 책"이며, Zipline·PyFolio·Empyrical을 "최고의 백테스트 및 성과 분석 소프트웨어"로 사용 (p11).
- 에이콘의 알고리듬 트레이딩 생태계에서 《실전 알고리즘 트레이딩 배우기》(세바스티앙, 2020)와 스테판 젠슨 머신러닝/딥러닝 책의 갭을 메우는 위치 (p11).
- 2장 "시스템 트레이딩" — 트레이딩 방법 검증, 과학적 접근법, 일관성 있는 방법론, 시간 관리 (p15 목차).
- SMA50/SMA100 롤링 평균 비교로 포지션 결정하는 백테스트 코드 예 — "SMA50이 SMA100 위에 있으면 1로 설정" (p86).
- 코드 공개: 저자의 followingthetrend.com/trading-evolved/ 에서 다운로드 (p12).

## 관련 페이지
- [[python-algorithm-trading]] — 파이썬 알고리즘 트레이딩 입문서
- [[quant-investing-python]] — 퀀트 전략 검증 실습
- [[finance-risk-ml-python]] — 금융 머신러닝 리스크 관리
