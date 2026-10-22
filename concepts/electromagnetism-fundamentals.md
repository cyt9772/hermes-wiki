---
title: 전자기학 기초 (Electromagnetism Fundamentals)
created: 2026-10-22
updated: 2026-10-22
type: concept
tags: [engineering]
sources: [raw/books/em-engineering.md, raw/books/basic-em.md, raw/books/time-harmonic-em.md, raw/books/electromagnetism.md, raw/books/em-exam.md]
confidence: high
---
# 전자기학 기초 (Electromagnetism Fundamentals)

Maxwell 4방정식을 축으로, 정전기·정자기·시간진행 전자기장을 다루는 공학/물리 교과서 **5권(USB)** 공통.

## 5권 비교 (관점별)

| 관점 | 페이지 | 소스 |
|---|---|---|
| **공학** (Hayt) | Vector → Gauss → Coulomb → Biot-Savart → Ampere → Maxwell → plane wave → transmission line | [[em-engineering]] 492p |
| **물리** (Griffiths) | Vector → Electrostatics → Matter → Magnetostatics → Electrodynamics → EM waves → **relativistic** | [[basic-em]] 513p |
| **수학** (Harrington) | **time-harmonic**, **파공간**(plane/cylindrical/spherical), **completeness** decomposition | [[time-harmonic-em]] 495p |
| **만화** (Endo) | **개념 직관** 6장: Coulomb → Gauss → Current → Ampere → Relativity | [[electromagnetism]] 262p |
| **수험** (Yong) | **기출문제+모범답안** — Coulomb·Gauss·dipole·Maxwell·**Poynting** | [[em-exam]] 285p |

## 학습 경로 (권장)
1. **입문**: [[electromagnetism]] (만화) — "왜 Maxwell인가" 질문 해소
2. **개념**: [[em-engineering]] (Hayt, 공학) 또는 [[basic-em]] (Griffiths, 물리)
3. **수학**: [[time-harmonic-em]] (Harrington) — time-harmonic/wave-space
4. **실전**: [[em-exam]] (수험서) — 문제 풀이
5. **마이크로파**: [[microwave-engineering]] (Pozar) — 제2-4장으로 이어짐
6. **RF 시스템**: [[rf-engineering]] (Chang) — 실무 시스템 파라미터

## 주의
- **서로 포집 관계**: Hayt ⊂ Griffiths ⊂ Harrington — 중복 학습 불필요
- **Harrington**은 "time-harmonic" 관점이라 Pozar/Hayt와 **이론 구조** 다름
- **OCR**: 수식(Maxwell, ∇, Larmor)은 원본 PDF 대조
