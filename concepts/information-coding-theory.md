---
title: 코딩이론 × 정보이론
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, information-theory, coding-theory]
sources: [raw/books/information-engineering-korea.md]
confidence: medium
---
# 코딩이론 × 정보이론

코딩이론(채널코딩·소스코딩)과 정보이론(엔트로피·채널용량)은 **상호보완적**이다 — 코딩이론이 "무엇을 어떻게 코딩할지"를, 정보이론이 "한계가 어디까지인지"를 정량적으로 제시함으로써 정보공학의 양대 핵심 이론을 이룬다. 이 클러스터의 한국 정보공학 교재(1996)가 이 접목을 체계화한다.

## 정보공학 — 코딩이론과 정보이론의 접목 (진영사, 1996)
- **전제(머리말)**: "정보이론은 코딩이론으로부터 유도될 수 있으며, 코딩이론에 의해 성취될 수 있는 시스템의 한계는 정보이론에 의해 제시된다" — 두 이론의 **상호보완적** 관계 `[raw/books/information-engineering-korea.md]`
- **수학적 기반: 확률론**(제1장) — 상대빈도·공리, Bayes 규칙, 이산/연속 랜덤변수, 결합분포, 통계적 평균 `[raw/books/information-engineering-korea.md]`
- **코딩이론 3단계**: 채널코딩(패리티·재전송·가중치·**Hamming**·기하학적 접근, 제3장) → **가변길이 코드**·**Kraft 부등식**·**Huffman**(제4장) → **상관관계/자압축**·Markov + Huffman·**DPCM/ADPCM/DM/ADM**·Arith code(제5장) `[raw/books/information-engineering-korea.md]`
- **정보이론 3단계**: **엔트로피** 정의·성질(제6장) → 소스코딩의 한계(Entropy↔평균코드길이, 제7장) → **채널 특성·상호정보**(제8장) → **채널용량**(균일채널·BSC, 제9장) → **Shannon 정리**(소스/채널 코딩 정리, 제10장) `[raw/books/information-engineering-korea.md]`

## 두 축 (코딩 ↔ 정보)

| 축 | 소스 (1996) | 핵심 |
|---|---|---|
| 채널코딩 | 제3장 | 오류 검출/정정 (패리티·Hamming) |
| 소스코딩 | 제4-5장 | 효율 (Huffman·DPCM·자압축) |
| 정보 한계 | 제6-7장 | 엔트로피-코드길이의 상한 |
| 채널 한계 | 제8-10장 | 상호정보·채널용량·Shannon 정리 |

## 관련
- [[information-engineering-korea]]
- [[information-coding-theory]] (본인 개념)
- 인접: [[a-course-in-dsp]] (통신/신호 배경), [[spread-spectrum-cdma]] (채널 용량 활용), [[ofdm-orthogonal-frequency-division]], [[dct-algorithms-applications]] (소스 부호화 접점 → [[transform-coding]])
