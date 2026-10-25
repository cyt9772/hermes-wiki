---
title: Advanced Engineering Mathematics, 8th ed. (Kreyszig)
created: 2026-10-22
updated: 2026-10-22
type: entity
tags: [book, engineering-mathematics, numerical-methods]
sources: [raw/books/advanced-engineering-mathematics.md]
confidence: high
---
# Advanced Engineering Mathematics, 8th ed. (Kreyszig)

> "Differential equations are of fundamental importance in engineering mathematics because many physical laws and relations appear mathematically in the form of such equations." (Part A 서두, raw p. 1)
> 저자: Erwin Kreyszig (Ohio State University), John Wiley & Sons, 8th ed. 1999 (ISBN 0-471-33328-X), 1285p

## 개요
**공학계 표준 공학 수학 교재**. 상미분·편미분·라플라스·특수함수(레전드르·베셀)·선형대수·벡터해석(그라스호프·스톡스 정리)·복소함수·푸리에 분석·수치해법(보간·적분·Euler/Runge-Kutta)·최적화·그래프·확률통계를 하나의 체계로 묶은 7부 23장 구조. 물리 문제에서 수식 모델링 → 해법 → 해석의 3단계를 반복 교육하는 것이 이 책의 교육 철학이다. `^[raw/books/advanced-engineering-mathematics.md]`

## 장 구조 (Part A–G, 23장, 1285p)
- **Part A — 상미분 (Chaps. 1-5)**: 1장 1계(방향장·분리 가능·적분인자), 2장 2계 이상 선형(고유진법·매개변수변수법·공진), 3장 연립·위상평면·안정성, 4장 급수해법·레전드르·베셀·Sturm-Liouville, 5장 **라플라스 변환**(단위계단·Dirac Δ·보완 적분)
- **Part B — 선형대수·벡터해석 (Chaps. 6-9)**: 행렬·연립해, **고유값 문제**(대각화·단일/헤르미트), 기울기·발산·베어링, 그린·가우스 발산·**스톡스 정리**
- **Part C — 푸리에 분석·편미분 (Chaps. 10-11)**: 푸리에 급수/적분/변환, 파동방정식·열방정식(변수분리·d'Alembert), 포물·이퍼볼·타원형 분류
- **Part D — 복소해석 (Chaps. 12-16)**: 코시-리만, 코시 적분 정리·정리공식, 테일러·로랑 급수·**잔수법**, 형상사영·전위이론
- **Part E — 수치해법 (Chaps. 17-19)**: 고정소수점·오차, 반복방정식해, **보간·스플라인**(17.3-17.4), 수치적분·미분(Romberg·적응적분, 17.5), LU 분해·최소제곱·QR 분해·Power 법, Euler/Runge-Kutta(19.1)-다단계법·편미분 수치해(19.4-19.7)
- **Part F — 최적화·그래프 (Chaps. 20-21)**: 단순법(선형프로그래밍), 최단경로·최대유량·대칭분배
- **Part G — 확률·통계 (Chaps. 22-23)**: 확률분포(이항·포아송·정규), 추정·가설검증·피츠성분석
- **Appendix 1-5**: 참고문헌, 홀수문제 해답, 특수함수 공식, 추가 증명, 함수표

## 핵심 기여
- **모델링→해법→해석 3단계 교육 구조** — 해를 얻는 것보다 물리적 의미를 읽는 것을 강조 ("The computer can sometimes give us nonsense", Part A 서두)
- **수치해법을 독립 파트로 배치** (Part E): 이론 파트(상미분/편미분/복소)와 해법 파트(수치해법)가 장 단위에서 서로 참조(1장 직후 19.1-19.3으로 바로 수치해 접목 가능)
- **4개 학기 연속 과정** 구성 제안 — 상미분 → 선형대수/벡터해석 → 복소 → 수치해법의 표준 공학 수학 시퀀스

## OCR 신뢰도
- 텍스트 레이어 내장본 (pdftotext -layout 추출, OCR 없음) — 본문 추출은 양호
- **주의**: 수식·도식은 추출에서 깨짐 심함 (예: "sh1-", "cu", "0rdinary" 같은 변형 토큰). 식 번호·문맥으로 cross-check하고 수치 해석 재사용 시 원본 PDF(로컬) 대조 필요
- 부록/수식표 (Appendix 3, 5)는 신뢰도 낮음 — 인용 시 원본 확인

## Related
- 저자: [[erwin-kreyszig]]
- 개념: [[numerical-methods-science-computing]], [[differential-equations-engineering]]
- 관련 책: [[numerical-recipes-in-c]] — 수치해법의 C 구현 관점 (Kreyszig Part E의 알고리즘을 Press 등 4인이 C로 구현), [[practical-electronics-eng]] — 이교재가 다루는 전자공학 모듈의 수학적 기초
- **해답집**: [[kreyszig-advanced-engineering-math-8ed-instructor]] — 8th ed. Instructor's Manual (Wiley 1999, 317p), Ch.1~23 전수 문제 해답 + 장별 "Major Changes"·절별 Purpose 코멘트
