---
title: 파이썬을 활용한 금융공학 레시피
created: 2026-10-15
updated: 2026-10-15
type: entity
tags: [book, finance-engineering, python, derivatives, data-analysis]
sources: [raw/books/finance-recipes.md]
source_book: "파이썬을 활용한 금융공학 레시피"
confidence: high
---

# 파이썬을 활용한 금융공학 레시피 (Financial Engineering with Python)

**"문과생의 코딩 울렁증과 이과생의 금융 울렁증을 한 방에 해결하는 금융공학 사이다"** — 금융상품 밸류에이션의 수학적 개념(선물·옵션·펀드)을 파이썬(엑셀 → 넘파이 → 팬더스 → matplotlib)으로 하나씩 구현하는 입문 실무서. 저자 김용환(finterstellar), 한빛미디어 2018.

> "금융상품을 운용할 때 비교 대상보다 높은 수익을 추구하는 것을 알파(α), 비교 대상의 수익률과 유사한 패턴의 수익을 추구하는 것을 베타(β)라고 합니다." (Ch.16, p.326)

## 개요

파이썬으로 금융공학을 배운다는 것은 두 가지 울렁증을 동시에 치유하는 것 — (1) 문과생은 코드를, (2) 이과생은 금융상품의 밸류에이션. 이 책은 그 교차점에서 **"필요한 것만"** (minimal-just-enough)을 다루는 컨셉.

## 구성 (4부, 19장)

1. **부, 1부 준비하기** (Ch.1~3) — 금융상품의 진화(은행·보험·주식·파생상품·구조화), 금융공학 = 금융 + 모델링, 돈의 시간가치(PV/FV), 파이썬 설치(Anaconda · Jupyter).
2. **Part II, 주식과 지수** (Ch.4~7) — KOSPI100/200/500/1000 지수, 주가 그래프, 엑셀 실습, 파이썬 기초(함수·모듈·뷰티플 수프), **네이버 HTML 크롤링으로 KOSPI 10대 기업/지수 데이터 수집**.
3. **Part III, 파생상품** (Ch.8~15) — **선물 개념(레버리지, 이론가, 베이시스, 콘탱고/백워데이션, 롤오버)** (Ch.8-9), 옵션의 구조·특성·가격(내재가치+시간가치, 변동성) (Ch.12), **블랙-숄즈 모형과 옵션 그릭스(Δ, Γ, θ, ν, ρ)** (Ch.12-13), 엑셀/파이썬으로 모형 구현.
4. **Part IV, 펀드와 구조화 상품** (Ch.16~19) — 액티브 vs. 패시브, **알파(α) vs. 베타(β)**, ETF/ETN/ELW/ELS 구조화 상품, K10 펀드 설계.

## 핵심 개념 링크

- 돈의 시간가치: **[[time-value-of-money]]** (PV/FV · 이자율 · 할인)
- 선물: **[[futures-theory-price]]** (이론가, 레버리지의 안전장치) / **[[basis-contango]]** (베이시스·콘탱고·백워데이션·롤오버)
- 옵션: **[[black-scholes]]** (C = S·N(d₁) − K·e^(−rT)·N(d₂)) / **[[option-greeks]]** (Δ·Γ·θ·ν·ρ)
- 펀드: **[[alpha-vs-beta]]** (알파·베타·벤치마크) / **[[structured-products]]**
- 데이터: 크롤링(뷰티플 수프) → 팬더스(시리즈·데이터프레임) → 시각화(matplotlib) 파이프라인
- 코딩 기술: 반복 데이터(넘파이 배열) → 데이터베이스(팬더스) — 금융 데이터 처리

## 관련 서적

- 투자/매매: [[trading-technique]] (돈을 부르는 매매의 기술 — 실시간 매매), [[futures-options-pricing]] (선물옵션 가격 이론 기법서)
- 밸류에이션: [[essentialism]] (집중), [[accounting-genius-hong]] (재무제표), [[retire-with-us-stocks]] (미국주식)
- 데이터 분석: [[wise-quant-investing]] (슬기로운 퀀트투자 — 통계·승률)

## 참고

- 저자가 직접 배포하는 예제 코드: https://github.com/finterstellar/download
- 이 책은 **수학·프로그래밍의 "기본기"**에 치중 — 투자 전략·비전 서적이 아님. 매매·투자 철학은 다른 서적과 조합해야 함
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 400/400p (errors=0)
