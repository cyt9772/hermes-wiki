---
title: 슬기로운 퀀트투자
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, quant, trading, us-stocks, valuation]
sources: [raw/books/smart-quant-investing.md]
confidence: medium
---

# 슬기로운 퀀트투자

> 주린이+코알못도 파이썬으로 쉽게 따라 하는 퀀트 레시피 (p3)

## 개요
- **저자:** 김용환 (Finterstellar) — 한국거래소 구조화상품 부문 출신 서학개미, 전 저서 「파이썬을 활용한 금융공학 레시피」(한빛미디어, 2018); Yubin Kim — 퀀트머신 개발자 (p5)
- **출판:** 한빛미디어(주), 초판 1쇄 2021-09-30, Copyright © 2021, ISBN 979-11-6224-475-3 (p3)
- **성격:** "서학개미를 위한 퀀트투자 입문서이자 실습서" — 퀀트머신(Finterstellar)과 구글 콜랩에서 유명 전략을 구현·백테스트 (p7, p8).

## 내용
- 지은이의 말: 2020년 유동성 호황 이후 "시장의 룰이 바뀌었다"며 지속 가능한 전략을 만들어 꾸준히 실행하자는 문제의식 (p7).
- 서학개미는 월스트리트 펀드매니저·로빈후드 군단과 경쟁해야 하고 언어·시차 장애물로 퀀트 전략이 좋은 무기가 된다는 논리 (p7).
- 구성: 1·2장 퀀트머신 개념과 설치, 3장 단기투자 전략(RSI, 엔벨로프, 볼린저밴드, 스토캐스틱 등), 4·5장 가치투자 밸류에이션(PER, PBR, EV/EBITDA 등), 7장 그린블라트 마법공식·피오트로스키 스코어 합성 (p9).
- 퀀트머신 실습 예제: `fs.set_terms(trade_start='2011Q1', trade_end='2021Q1')` 등으로 4대장+대형주 조건을 설정 (p188).
- 동명·동저자 책의 별도 인덱스: [[wise-quant-investing]] (raw/books/wise-quant-investing.md 기반).

## 관련 페이지
- [[finance-recipes]] — 같은 저자의 파이썬 금융공학 레시피
- [[quant-investing-python]] — 퀀트 전략 검증 실습서
- [[python-algorithm-trading]] — 알고리즘 트레이딩 입문서
