---
title: 블랙-숄즈 모형 (Black-Scholes Model) — 옵션 가격
created: 2026-10-15
updated: 2026-10-31
type: concept
tags: [investing, options, finance, valuation]
sources: [raw/books/finance-recipes.md]
confidence: high
---

# 블랙-숄즈 모형 (Black-Scholes-Model) — 옵션 가격

**"옵션 세계에서 바이블 같은 공식"** — 콜옵션/풋옵션의 공정가격을 기초자산 가격·행사가격·만기·이자율·변동성 5변수로 결정. 옵션 가격 C = S·N(d₁) − K·e^(−rT)·N(d₂)의 구조로 "기초자산 기댓값 − 행사가격의 현재가치"를 환율로 나타내며, 옵션 그릭스(Δ·Γ·θ·ν·ρ)의 계산 근거.

> "옵션에 관심이 있는 사람이라면 블랙-숄즈 방정식이라는 이름을 한 번쯤 들어본 적... 블랙-숄즈 방정식은 옵션 세계에서 바이블 같은 공식입니다." (Ch.12, p.245)
>
> "복잡해 보이는 공식이지만 한번 프로그래밍을 해놓으면 컴퓨터가 하기 때문에 사용은 간단합니다." (p.245)

## 공식 (이론가)

**콜옵션** C(S,K,r,σ,T) = S·N(d₁) − K·e^(−rT)·N(d₂)
**풋옵션** P(S,K,r,σ,T) = K·e^(−rT)·N(−d₂) − S·N(−d₁)

$$d_1 = \frac{\ln(S/K) + (r + \sigma^2/2)T}{\sigma\sqrt{T}}, \qquad d_2 = d_1 - \sigma\sqrt{T}$$

- S: 기초자산 가격 (stock price at time 0)
- K: 행사가격 (strike price)
- T: 잔존만기 (연율로, time to maturity)
- r: 이자율 (연속복리, risk-free)
- σ: 변동성 (volatility)
- N(x): 표준정규분포 누적분포함수

## 직관적 의미 (p.245)

> "블랙-숄즈 모형에서 콜옵션의 가격인 C = S·N(d₁) − K·e^(−rT)·N(d₂) 중 N(d₁), N(d₂)는 옵션이 행사될 기댓값을 나타냅니다. 블랙-숄즈 모형에서 앞부분 S·N(d₁)은 '기초자산의 기댓값'이고, 뒷부분 K·e^(−rT)N(d₂)는 ... '행사가격의 기댓값의 현재가치'입니다."

즉 **콜옵션 = (행사 시 받을 기초자산 기댓값) − (행사 시 지급할 행사가격의 현재가치 기댓값)**. 이는 옵션을 "현금흐름 할인"의 문제로 환원한다는 의미로, 옵션 가격 평가의 가장 핵심적인 통찰.

## 실전 적용 (이 책)

1. **변동성(σ)의 역할**: "옵션가격 = 내재가치 + 시간가치" (p.242~243). 시간가치는 "시간이 지나면 가능성은 사라진다" (p.241)로, **시간가치 소멸 = 시간가치 decay (θ, 세타)** 로 설명.
2. **그릭스**: Δ(델타)·Γ(감마)·θ(세타)·ν(바르)·ρ(라우) — "어려워 보이는 옵션 용어" (p.246), 블랙-숄즈 공식의 편미분으로 계산
3. **Python 구현**: Ch.15 "파이썬으로 구현하는 블랙-숄즈 모형" (p.301~314) — 옵션가격 그래프·그릭스 시각화

## 실전 도구 (금융 MATLAB·금융 자격 축, 2005~2018 배치)
- **Neural Networks in Finance (McNelis 2005, MATLAB 한국어판)** — 신경망(MLP·RBF·KNN)을 포트폴리오 최적화·옵션/리스크 관리에 적용; MATLAB `fmincon`·`fzero` 최적화 도구 — 블랙-숄즈의 "프로그래밍으로 계산" 관행을 수치최적화 도구와 연결 `[raw/books/matlab-financial-analysis.md]`
- **매경TEST (매일경제신문·금융연수원, 2016)** — 경제·경영·재무·금융 국가공인 자격 교재; 이자율·통량·옵션 등 금융 기본개념 시험 범위 — 이론서(finance-recipes)의 개념을 자격시험으로 검증할 실용 축 `[raw/books/mg-test-exam.md]`
- **펀드투자권유대행인(FSA) 자격 (금융투자협회 2018)** — 펀드 판매·권유 실무 규제; 금융시장 이해를 영업 관점에서 보완 `[raw/books/fund-solicitation-agent.md]`
- **MATLAB 통계분석 (한정호·최승호, 2013)** — 확률분포·가설검정·선형회귀·Monte-Carlo 시뮬레이션 — 옵션 가격의 확률적 해석(무위험측정, 동적헷지 모의) 기초 도구 `[raw/books/matlab-statistical-analysis.md]`

## 출처

- raw: raw/books/finance-recipes.md, pages 245~247, 301~314
- 참고: 예제 코드 https://github.com/finterstellar/download
- 추가 도구: raw/books/matlab-financial-analysis.md, raw/books/mg-test-exam.md, raw/books/fund-solicitation-agent.md, raw/books/matlab-statistical-analysis.md

## 관련

- 옵션 그릭스: [[option-greeks]] (Δ·Γ·θ·ν·ρ — 블랙-숄즈의 편미분)
- 가격 구성: [[time-value-of-money]] (현금흐름 할인 구조)
- 선물: [[futures-theory-price]] (같은 할인 구조 위에 설계)
- 도구: [[matlab-financial-analysis]] · [[matlab-statistical-analysis]] — MATLAB 금융/통계 실습
- 자격/실무: [[mg-test-exam]] (매경TEST) · [[fund-solicitation-agent]] (FSA)
