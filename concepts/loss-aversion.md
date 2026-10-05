---
title: 손실회피성 (Loss Aversion)
created: 2026-10-05
updated: 2026-10-05
type: concept
tags: [behavioral-economics, prospect-theory, psychology, investing, risk]
sources: [raw/books/behavioral-economics.md]
confidence: high
---

# 손실회피성 (Loss Aversion)

동일 금액의 손실이 이익보다 **2~2.5배 강하게** 느껴지는 심리적 비대칭 — 프로스펙트 이론 가치함수의 굴절점.

## 메커니즘

- 가치함수 v(x)은 준거점(reference point)을 기점으로 이익 구간에선 concave(민감도 감소), 손실 구간에선 convex이며, 손실 쪽 기울기가 더 가팔라 **-v(-x) > v(x)** (p102, p110).
- 카너먼·트버스키 측정: "1,000원의 이익과 1,000원의 손실에서 각각의 절대치는 후자가 약 2배에서 2.5배나 큰 걸로 나타났다" (p110).
- 결과로 (1000원, 0.5 : -1000원, 0.5) 같은 50:50 복권을 대부분이 거부 — "이 금액의 손익에서는 손실 쪽을 크게 평가한다는 의미" (p109).
- 손실회피성의 파생 현상들 (제5장, p132-156): [[concepts/endowment-effect]] (보유효과), 현상유지 바이어스 (status quo bias), 재판매 목적이면 보유효과가 사라짐 (리스트, p143).
- 손실 여부가 반복되면 "1회의 이익이나 손실을 얻으면 그 결과 값이 새로운 준거점이 되고" 다음 평가의 기준이 이동 (p113) — 손절 후 재진입, 평가 손실 장기화.

## 투자 관점

1. **손절 지연**: 매도가 손실을 확정시키는 "실현 손실"이라 손실회피 작용에 막혀 평가손실이 장기화된다. 손절 기준을 매수 전 수리로 고정하는 것이 대안.
2. **과조기 이익 확정**: 이익은 손실만큼 감각적이지 않으므로 작은กำไร을 빨리 챙기는 비대칭 트레이딩이 생김.
3. **리스크 태도 비대칭**: 이익에서는 리스크 회피, 손실에서는 리스크 추구 (p109) — 바닥에서 "반등 한 방"에 베팅하는 저가매집 심리의 원인.
4. [[concepts/asset-allocation]] 관점: 손실 구간에서의 과민한 손절/방치가 리밸런싱의 실제 마찰비용으로 작동.

## 원문 근거 (p. = `raw/books/behavioral-economics.md` 기준)

> "손실은 똑같은 금액의 이익보다도 훨씬 더 강하게 평가된다." (p109)
> "카너먼과 트버스키의 측정에서는… 1,000원의 이익과 1,000원의 손실에서 각각의 절대치는 후자가 약 2배에서 2.5배나 큰 걸로 나타났다." (p110)
> "가치함수의 세 번째 특성은 '손실회피성(loss aversion)'이다." (p109, 영문 token garbled)
> "보유효과란 사람들이 어떤 [물건을] 실제로 소유하고 있을 때 [그]를… 높게 평가하는 것을 말한다." (p136)

## See also

- [[concepts/endowment-effect]]
- [[concepts/framing-effect]]
- [[concepts/asset-allocation]]
- [[entities/behavioral-economics]]
