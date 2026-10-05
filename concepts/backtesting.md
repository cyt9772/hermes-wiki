---
title: 백테스팅 (Backtesting)
created: 2026-10-05
updated: 2026-10-05
type: concept
tags: [backtesting, backtest, quant, metrics, sharpe, mdd]
sources: [raw/books/wise-quant-investing.md]
---

# 백테스팅 (Backtesting)

**한 줄 정의:** 과거 주가에 매매 전략을 적용해 성과(CAGR·Sharpe·HitRatio·MDD)를 측정하고 벤치마크와 비교하는 전략 검증 절차. 이 책의 실습 핵심 도구.

## 구조/메커니즘
1. **전략 코드화** — 신호(매수/매도)를 파이썬으로 정의. 예: `signal(df, signal_type='band')`, `fs.position(df)`, `fs.evaluate(df, cost=.001)`, `fs.performance(df, rf_rate=0.01)`.
2. **성과 측정** — 백테스트 결과 지표: CAGR(연평균수익률), Accumulated return(누적수익률), Average return(평균수익률), Benchmark return, Number of trades, Hit ratio, Investment period, Sharpe ratio, MDD, Benchmark MDD. (p.050–052)
3. **벤치마크 대비 판단** — "벤치마크는 내가 비교할 대상이다. 내가 투자한 종목이 아니라 같은 기간에 상승한 종목이 비교의 대상이다. … 벤치마크보다 높게 상승한 [종목을 골라야 한다]." (p.060)

## 투자 관점
- **수익률만으로는 부족** — p.057 "백테스팅에서 가장 신경을 쓸 부분은 수익률이다. 하지만 수익률만 높다고 좋은 전략이 … [아니다]" (일부 깨짐). 승률·MDD·벤치마크를 함께 본다.
- **실패도 학습** — 보잉·Bale] 예: "CAGRO -22.119%가 나왔다. 벤치마크수익률보다는 나았다고 위로할 수 있겠지만 처참히 깨진 투자다. 수익률이 하찮으니 나머지는 볼 필요도 없다." (p.089, 일부 깨짐) → "다른 기간도 많이 테스트해보고 전략을 선택할 필요가 있다."
- **기간/튜닝에 민감** — "엔벨로프 전략은 … 튜닝의 가능성도 무한하다. 이동평균을 지수이동평균으로 바꿔보기도 되고, w를 [변경]하며 테스트 해볼 수도 있다." (p.092)
- **복리 환산** — CAGR은 누적수익률을 연평균으로 환산, "1년보다 짧으면 단리 … 1년보다 길면 복리로" (p.051) → [[compound-interest]]

## 원문 근거 (OCR verbatim, page-anchored)
> "앞에서 백테스팅 결과물로 수억률을 비롯한 여러 투자성과 측정지표가 나왔다. 각 숫자는 어떤 의미인지 하나씩 알아보자." — p.050

> "CAGR: … 연평균으로 따졌을 때 수익률이 얼마나 되는지 측정한 [지표], 누적수익률을 연평균수익률로 환산해서 구한다. 테스트 기간이 1년보다 짧으면 단리로 계산해 확장하고, 1년보다 길면 복리로 계산해 …한다." — p.051 (일부 깨짐)

> "백테스트를 통해 [전략]의 [성과]를 볼 [수] 있다. [ROCE]를 이용한 … [전략]의 수익률은 … [확인]했다." — p.301 (수식·지표 토큰 다수 깨짐, 원서 대조 필요)

> "100% 승률은 아니더라도 90% 또는 80%의 [승률]을 노리며, 확률적인 우위를 가진 상태로 매수한다." — p.097 (일부 깨짐)

## See also
- [[quant-investing]] — 백테스트가 검증하는 퀀트 전략
- [[compound-interest]] — CAGR·복리 환산
- [[value-investing]] · [[trend-following]] — 백테스트되는 두 가지 전략 가족
- [[relative-strength]] · [[momentum-investing]] — 단기 전략 지표
- [[us-equity-market]] — 벤치마크(미국 지수) 기준
- 실서: [[wise-quant-investing]] (백테스트 실습 전 과정)
