---
title: 가치투자 (Value Investing)
created: 2026-10-05
updated: 2026-10-05
type: concept
tags: [value investing, valuation, PER, PBR, factor, us-stocks]
sources: [raw/books/wise-quant-investing.md]
---

# 가치투자 (Value Investing)

**한 줄 정의:** PER·PBR·재무비율 같은 밸류에이션 지표로 '저평가' 주식과 '우량(고수익)' 주식을 선별해 장기적으로 매수하는 투자 철학. 이 책 4~6장이 다룬다.

## 구조/메커니즘
1. **재무제표 이해** — 손익계산서·재무상태표·현금흐름표·재무비율 (4장, p.117–130)
2. **저평가 선별** (5장) — PER·PBR·PSR·PCR·시가총액 하위·EV/EBITDA·EV/Sales·**NCAV**(그레이엄)·**PEG**(피터린치)
3. **우량 선별** (6장) — ROA·ROE·**RIM**(잔여이익)·**GP/A**(노비막스)·안정성·성장률·회전율·해자(이익률)
4. **전략 합성** (7장) — 여러 지표를 종합 등으로 병합 (그린블라트 마법공식, 피오트로스키 F-score)

지표 정의 (OCR, p.135–137):
- "PER = 시가총액 / 순이익" — "PER이 낮을수록 이익에 비해 주가가 싸다는 것을 의미한다." (p.135)
- "PBR = 시가총액 / 순자산" — "PBR이 낮을수록 이익에 비해 주가가 싸다는 것을 의미한다." (p.137)

## 투자 관점
- **장기 시선** — "PER, PBR 같은 지표를 활용하는 투자 모델은 장기적인 시각에서 주가를 예측한다." (p.033)
- **밸류 팩터** — 저평가(PER·PBR·NCAV)와 우량(ROE·GP/A·RIM) 두 축을 함께 봐 [[trend-following]](단기·기술)과 대비된다.
- **합성 전략** — 여러 팩터 종합 등수로 상위 종목 선별 (그린블라트 마법공식: ROCE+PER, p.303) → [[valuation-multiples]]
- **미국 시장** — PER·NCAV 같은 전략은 미국 종목 데이터로 백테스트됨 (p.134–260) → [[us-equity-market]]

## 원문 근거 (OCR verbatim, page-anchored)
> "PER는 주가의 이익 대비 비율을 나타내는 지표이다. PER이 낮을수록, 이익에 비해 주가가 싸다는 것을 의미한다. 주가가 낮아지는 [원인 중] 이익이 감소하는 경우 … PER는 [높아진다]." — p.135 (일부 깨짐)

> "PBR은 주가가 순자산(자기자본) 대비 얼마나 높은지를 나타내는 지표이다. PBR이 낮을수록, 이익에 비해 주가가 싸다는 것을 의미한다." — p.137

> "NCAV는 순유동자산(Net Current Asset Value)으로, 자산의 순자산 … 순유동자산은 … 부채를 제거한 순유동자산이다." — p.169 (일부 깨짐)

> "PEG는 PER을 EPS Growth Rate(이익 성장률)으로 나눈 것이다. … PER가 낮을수록 이익(이익)에 대비해 주가가 싸다고 해석할 수 있다." — p.205 (일부 깨짐)

> "RIM은 이자비용 … 주주가 요구하는 수익률(요구수익률) 초과이익이 잔여이익이다." — p.223 (수식 일부 깨짐)

## See also
- [[quant-investing]] — 가치 지표를 퀀트로 전환하는 맥락
- [[valuation-multiples]] — PER·PBR·PSR 등 밸류에이션 지표
- [[backtesting]] — 전략 검증 (재무지표 기반)
- [[trend-following]] — 대비되는 단기·기술 가족
- [[us-equity-market]] — 데이터가 있는 미국 시장
- 실서: [[wise-quant-investing]] (5~7장 가치/우량/합성)
