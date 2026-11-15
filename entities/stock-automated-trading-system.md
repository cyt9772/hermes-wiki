---
title: 주식 자동 거래 시스템 구축
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, trading, automation, python, react]
sources: [raw/books/stock-automated-trading-system.md]
confidence: medium
---

# 주식 자동 거래 시스템 구축

> 파이썬과 리액트를 활용한 — 데이터 수집부터 거래 자동화, API 서버, 웹 개발, 데이터 분석까지 아우르는 (p1)

## 개요
- **저자:** 박재현 (p3)
- **출판:** 위키북스, 1쇄 2020-02-12 / 2쇄 2020-08-24, 348p, ISBN 979-11-5839-188-1 (p3)
- **성격:** 데이터 수집 → 저장 → 분석 → 거래 자동화 → API 서버·웹(리액트)까지 주식 자동 거래 시스템 전체를 개발하는 실무서. 예제 코드 https://github.com/wikibook/stock-trading/ (p3).

## 내용
- 집필 의도: "하나의 주제를 깊이 다루는 것보다 아무것도 없는 상태에서 전체 시스템을 개발하는 내용을 다뤄보고 싶었습니다" — 1~2년 차 개발자 수준에 맞춰 전체 구성·흐름·개발 방법을 안내 (p5).
- 데이터 수집: 이베스트투자증권 Open API(XA 세션·쿼리 객체 구현), 공공데이터, 웹 크롤링, 데이터 마켓(Quandl) (목차 p6).
- 저장·가공: MongoDB 문서/컬렉션 구조와 CRUD 명령어, 배열 관련 명령어 (목차 p7).
- 거래 자동화 코어: pythoncom.PumpWaitingMessages 로 XA 메시지 처리, "결과 블록" 카운트/필드 변환 로직 (p60).
- 10년 차 개발자의 두 번째 책 — 첫 책은 암호화폐 시스템 개발 (p5).

## 관련 페이지
- [[stock-trading-system-hands-off]] — 파이썬 데이터 수집·차트 분석·매매 자동화
- [[koreainvestment-openapi]] — 한국투자증권 Open API 자동매매
- [[python-algorithm-trading]] — 알고리즘 트레이딩 입문서
