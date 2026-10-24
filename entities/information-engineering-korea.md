---
title: 정보공학 (1996)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, information-theory, coding-theory]
sources: [raw/books/information-engineering-korea.md]
confidence: medium
---
# 정보공학 — 코딩이론과 정보이론의 접목 (1996)

> 표지/원저: (원문 미확인) — 표기 "강오캉, 창용민, 언선규" 3자, 인명 OCR 왜곡(확인 필요).
> 출판: 진영사, 1996(발문 종료 "1996 년 겨울"), 461p

## 개요
정보의 표시·전송·저장을 정량적으로 다루는 "협의의" 정보공학 교재 — 정보통신공학·전파공학·전자공학·컴퓨터공학 학부 3·4학년 대상(머리말) `[raw/books/information-engineering-korea.md]`. "코딩이론(채널코딩 + 소스코딩)과 정보이론(엔트로피 + 채널용량 + Shannon 정리)은 **상호보완적** (코딩에 의한 한계는 정보이론이 제시, 정보이론은 코딩에서 유도) 관계"라는 전제(머리말) 아래 (1) **확률론**(제1장) → (2) 정보공학-통신시스템 모델(제2장) → (3-5) **코딩이론**(채널코딩·Hamming, 가변길이·**Huffman**, 상관·DPCM/ADPCM/DM/ADM, Arith code) → (6-8) **정보이론**(엔트로피·소스 한계, 채널 특성·상호정보, 채널용량) → (10) **Shannon 정리**(소스/채널 코딩 정리)로 이어지는 10장 체제 `[raw/books/information-engineering-korea.md]`.

## 장 구조 (10장 + 부록 I-II, 461p)
1. **확률과 랜덤변수** — 상대빈도·공리, Bayes 규칙, 이산/연속 랜덤변수, 결합분포, 통계적 평균
2. **정보공학과 통신시스템** — 구조, 신호시스템 모델, 소스알파벳/코드알파벳
3. **채널코딩** — 패리티검사, 재전송, 다발오류, 가중치 코드, 오류정정, **Hamming 코드**, 기하학적 접근
4. **가변길이 코드** — 소스코딩, 유일/동시 디코딩, **Kraft 부등식**, **Huffman 코드**와 응용, 확률추정오류
5. **상관관계와 자료압축** — Markov 과정 + Huffman, 예측형 부호, **DPCM/ADPCM/DM/ADM**, Arith code
6. **정보의 특성과 ENTROPY** — 정보이론-코딩 관계(6.1), **엔트로피** 정의성질
7. **소스코딩의 한계** — Entropy↔평균 코드길이, 동시코드, 코드 확장, Markov 과정
8. **채널의 특성과 상호정보** — BSC, 신호시스템 Entropy, **상호정보**
9. **채널용량** — 균일채널/균일입력, **BSC 용량**, 연속 소스
10. **SHANNON의 정리** — 소스/채널코딩 정리, 결정규칙/오류확률, **랜덤코드와 그 평균**, 일반적 채널
+ 부록 I 적분표·급수표, 부록 II 오차함수표

## 핵심 내용
- **코딩이론 × 정보이론의 접목**이라는 명시적 제목 — 두 이론이 상호보완(코딩이론은 "한도를 설정", 정보이론은 "한도 제시") `[raw/books/information-engineering-korea.md]`
- **DPCM·ADPCM·DM·ADM** 예측 부호화를 5장 5.4절에서 다룸 — 음성/영상 신호의 자료압축에 핵심 `[raw/books/information-engineering-korea.md]`
- **Huffman 코드**와 **Kraft 부등식**을 4장에서 다룸, **Arith code**를 5장에서 다룸 `[raw/books/information-engineering-korea.md]`
- **채널코딩(3장) + 가변길이 코드(4장) + 상관/자압축(5장)**의 3단계 체계 + **엔트로피(6-7장) + 채널용량(8-9장) + Shannon 정리(10장)** `[raw/books/information-engineering-korea.md]`
- 저자·일부 OCR 왜곡(인명, 표기 일부 깨짐) → 원본 대조 필요, confidence: medium

## Related
- 개념: [[information-coding-theory]] — 코딩이론 × 정보이론 클러스터 개념
- 인접: [[a-course-in-dsp]] (DSP 쪽), [[dct-algorithms-applications]] (변환 부호화), [[signals-and-systems-korea]] (신호시스템 모델)
