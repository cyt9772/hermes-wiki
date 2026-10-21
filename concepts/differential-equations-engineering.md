---
title: 공학 수학과 미분방정식 (Differential Equations in Engineering)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering-mathematics]
sources: [raw/books/advanced-engineering-mathematics.md]
confidence: high
---
# 공학 수학과 미분방정식 (Differential Equations in Engineering)

## 정의
**물리 현상을 미분으로 모델링하고, 그 방정식의 해를 해석적·수치적으로 구하는 공학 수학의 핵심 축**. 상미분(1변수) → 편미분(2변수 이상) → 라플라스 변환 → 특수함수(베셀·레전드르)의 4단계를 포함.

## Part A — 상미분 (Kreyszig Chaps. 1-5, 1285p 중 p.1-302)
> "An ordinary differential equation is an equation that contains one or several derivatives of an unknown function, which we call y(x) or y(t)." (Chap. 1.1, raw p. 13)

**Chap. 1 — 1계 상미분**
- 분리 가능한 (1.3), 적분인자(1.5), Euler(1.6), Picard 반복·존재-고유(1.9)
- **모델링**: 전기회로(1.7), 직교궤적(1.8)

**Chap. 2 — 2계 이상 선형**
- 상수계수 2계(2.2), 복소경(2.3), 매개변수변수법(2.10)
- **모델링**: 질량-스프링 자유진동(2.5), **외력진동·공진(2.11)**, 전기회로(2.12)

**Chap. 3 — 연립·위상평면**
- 상수계수 연립(3.3), 임계점·안정성(3.4), 비선형(3.5)
- **Lotka-Volterra 포식자-피식자 모델** (Preface, raw p. 9)

**Chap. 4 — 급수해법·특수함수**
- **레전드르 다항식**(4.3), **Frobenius 법**(4.4), **베셀 함수 J·Y**(4.5-4.6), **Sturm-Liouville** 직교함수(4.7-4.8)

**Chap. 5 — 라플라스 변환**
- 정·역변환(5.1), 미분·적분 변환(5.2), 단원계단(5.3), **보완 적분**(5.5), 부분분수(5.6), 미분방정식(5.7)

## Part C — 푸리에·편미분 (Kreyszig Chaps. 10-11, p. 525-648)
> "Modeling: Vibrating String, Wave Equation" (11.2, raw p. 15)

- **푸리에 급수** (10.1-10.4), 푸리에 적분·변환(10.8-10.10)
- **변수분리법** + 푸리에 급수로 파동방정식(11.3-11.4), 열방정식(11.5-11.6)
- 포물·이퍼볼·타원형 편미분, 라플라스 연산자(11.9-11.11)

## Part D — 복소함수 (Kreyszig Chaps. 12-16, p. 651-827)
- **코시-리만 방정식** (12.4, 라플라스 방정식과 연결)
- 코시 적분 정리·정리공식(13.2-13.3), 테일러·로랑 급수(14.4, 15.1)
- **잔수법(Residues)** + 실적분(15.3-15.4), 형상사영·전위이론(16.1-16.4)

## Related
- 책: [[advanced-engineering-mathematics]], [[numerical-recipes-in-c]]
- 개념: [[numerical-methods-science-computing]] — 수치해법은 이 미분방정식을 컴퓨터로 푸는 단계, [[laplace-transform-circuits]] — 라플라스 변환을 회로 해석에 적용 (S-평면·극-영점)
