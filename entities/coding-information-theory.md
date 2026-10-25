---
title: Coding and Information Theory (Richard W. Hamming, 2nd ed.)
created: 2026-10-25
updated: 2026-10-25
type: entity
tags: [book, coding-theory, information-theory]
sources: [raw/books/coding-information-theory.md]
confidence: high
---
# Coding and Information Theory (Richard W. Hamming, 2nd ed. 1986)

> 저자: **Richard W. Hamming** (Richard Wesley Hamming, 1915–) — Stanford University Graduate School
> 출판: Prentice-Hall (Englewood Cliffs, NJ 07632), 2nd ed. 1986 (1st ed. 1980). ISBN 0-13-139072-4. Library of Congress: 85-17034, 519.4, OA268.H35 1986.
> Editorial: Nicholas C. Romanelli. Cover: Frederick Charles Ltd.
> 저자 소개: Bell Laboratories, Murray Hill, NJ → Stanford University. Shannon·Kolmogorov의 부호화 이론과 함께 20세기 코딩이론을 정립.

## 개요
코딩이론과 정보이론을 단일 저술로 통합한 학부·초급 대학원 교과서. "A Very Abstract Summary"로 개론을 열고 (1) 오류 검출 코드 → (2) 오류 수정 코드 → (3) 가변부호(Huffman) → (4) 혼성 코드 → (5) **Shannon의 엔트로피와 코딩 제1·2정리**까지 체계적으로 전개. 저자가 자명명한 "Hamming code"가 3장, **Huffman code**와 Hamming-Huffman 부호화(4.14)가 4장, **Shannon 제1정리**(6장, 엔트로피), **채널과 상호 정보량**(7장), **채널 용량**(8장), **Shannon 주 정리**(부호화 정리, 10장), **알파비트 코딩 이론**(11장)으로 이어지는 단일 서술 구조.

## 장 구조 (11장, 280p 기반)
| # | topic | pp |
|---|-------|----|
| **1** | **Introduction** — A Very Abstract Summary, History, **Model of the Signaling System**, **Information Source**, Encoding a Source Alphabet, Some Particular Codes, **ASCII Code**, Other Codes, Radix r Codes, Escape Characters, Outline of the Course | 1–19 |
| **2** | **Error-Detecting Codes** — Why, Simple Parity, White Noise, Retransmission, **Burst Error**, Weighted Codes, **Modular Arithmetic**, **ISBN** Book Numbers | 20–33 |
| **3** | **Error-Correcting Codes** — Rectangular, Triangular·Cubic·n-Dim, **Hamming Error-Correcting Codes**, Equivalent Codes, Geometric Approach, Single-Error-Correction Plus Double-Error-Detection, **Hamming Codes Using Words**, Applications | 34–50 |
| **4** | **Variable-Length Codes: Huffman Codes** — Unique Decoding, **Instantaneous Codes**, Construction, **Kraft Inequality**, Shortened Block Codes, **McMillan Inequality**, **Huffman Codes**, Special Cases, Extensions, Radix r, **Noise in Huffman Coding Probabilities**, Use of Huffman Codes, **Hamming-Huffman Coding** | 51–78 |
| 5 | Miscellaneous Codes — **Markov Process**, Ergodic Markov Processes, ... | 79–102 |
| **6** | **Entropy and Shannon's First Theorem** | 103–137 |
| **7** | **The Channel and Mutual Information** | 138–152 |
| **8** | **Channel Capacity** | 153–163 |
| 9 | Some Mathematical Preliminaries | 164–190 |
| **10** | **Shannon's Main Theorem** (채널 부호화 정리) | 191–208 |
| **11** | **Alphabet (Coding) Theory** | 209–280 |

## 핵심 기여
- **코딩×정보이론 단일 서술** — 2세기 코딩이론의 두 축(부호화 + 부호 이론)을 한 책을 통해 "정보 소스에서 채널 용량까지" 통합.
- **Hamming code** (서명)와 **Huffman code** (4.8)의 **Hamming-Huffman 부호화** (4.14) — 저자의 대표적 부호화 기법.
- **Kraft·McMillan 불등식** (4.5·4.7)이 가변부호의 경계조건.
- **Shannon 제1정리** (6장)와 **Shannon 주정리(부호화 정리)** (10장) — 코딩이론의 양 끝단.
- **Modular arithmetic · ISBN** (2.8·2.9)으로 실용 오류 검출 코드.

## Related
- 저자: [[richard-hamming]]
- 개념: [[spread-spectrum-cdma]] · [[cdma-dss-spread-spectrum]] (채널 부호의 적용) · [[information-coding-theory]] (정보공학 개요)
- 인접: [[video-compression-mpeg]] (정보부호 이론의 영상 적용) · [[digital-signal-processing]] (DSP 이론) · [[signals-and-systems-korea]]

## OCR/추출 신뢰도
- pdftotext 양호. 저자 이름 일부 깨짐(`Richard W. Hamming`은 1·7·22행서 명확) — 식 번호·문맥 cross-check.
