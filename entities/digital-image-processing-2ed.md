---
title: Digital Image Processing (Gonzalez & Wintz 1987)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-theory, image-processing, dft-fft]
sources: [raw/books/digital-image-processing-2ed.md]
confidence: high
---
# Digital Image Processing (Gonzalez & Wintz 1987)

> 표지/원저: **Rafael C. Gonzalez** (Electrical Engineering Department, University of Tennessee, Knoxville & Perceptics Corporation) · **Paul Wintz** (Consultant)
> 출판: Addison-Wesley, Second Edition 1987 (Reprinted with corrections November 1987), 522p, ISBN 0-201-11026-1

## 개요
디지털 영상 처리(DIP) 분야의 고전 이론 교과서. 1920년대 Bartlane 케이블 화상 전송에서 출발한 기술사(제1장)를 거쳐, 시각 인지와 **이미지 모델·샘플링·양자화**(제2장)로 기초를 세운 뒤, **2D DFT·FFT·Hadamard·Hough 변환**(제3장)으로 주파수 영역 도구상을 갖춰, **histogram enhancement·spatial smoothing/sharpening**(제4장), **degradation model과 Wiener·inverse filtering·제약 최소제곱 restoration**(제5장), **differential/contour/run-length encoding과 DPCM·transform encoding**(제6장), **segmentation — edge detection·thresholding·region growing·motion**(제7장), **representation & description — chain code·shape number·Fourier descriptor·texture·문법**(제8장)까지 이론-수학-구현을 한 권에 담은 제2판 `[raw/books/digital-image-processing-2ed.md]`.

## 장 구조 (TOC 기반, 522p)
1. **Introduction** — 배경, Digital Image Representation, DIP 시스템 요소(processor/digitizer/computer/storage/display)
2. **Digital Image Fundamentals** — 시각 인지, 이미지 모델, Sampling & Quantization, pixel 관계(연결성·거리·산술/논리), Imaging Geometry(변환·카메라 모델·stereo), Photographic Film
3. **Image Transforms** — Fourier/2D DFT 특성, FFT, Walsh/Hadamard/DCT, Hotelling, Hough transform
4. **Image Enhancement** — histogram modification(equalization·specification·local), smoothing(averaging·median·lowpass), sharpening(미분·highpass), image model 기반, 주파수역에서 공간 마스크 생성, pseudo-color
5. **Image Restoration** — degradation model, circulant/block-circulant 행렬 대각화, 무제약/제약 복원, inverse filtering, Wiener filter, 대화형 복원, 공간영역, warping·보간
6. **Image Encoding** — fidelity criteria, mapping/quantizer/coder, error-free(differential·contour·run-length), DPCM, transform encoding, hybrid(RPV TV)
7. **Image Segmentation** — discontinuity detection, edge linking(Hough·graph), thresholding(6종 기법), region-oriented(growing, split & merge), motion 활용
8. **Representation and Description** — chain code·polygon·signature·skeleton, boundary descriptors(shape number·Fourier·moments), regional(descriptors·topology·texture), similarity·relational descriptions(string grammar)
9. **Appendix** — A: Image Display Subroutines · B: Coded Images

## 핵심 내용
- 제2판은 제1판에 비해 49개 신장, 86개 신도, 100+ 신규 참고문헌으로 확대; 수학적 수준은 수학 분석·행렬·확률·프로그래밍 기초를 갖춘 4학년 수준의 기술계 학생 범위 `[raw/books/digital-image-processing-2ed.md]`
- 주파수 영역의 핵심 도구는 **2D DFT의 분리가능성·병진·주기·켤레대칭·회전·convolution-correlation** 특성과 **FFT 구현**(제3장) — 영상 향상·복원·인코딩이 모두 이 위에 서 있다 `[raw/books/digital-image-processing-2ed.md]`
- **Restoration**은 열화 모델 h*x = y를 행렬로 표현하고 circulant/block-circulant를 대각화하는 체계: 무제약 대수복원 → **inverse filtering** → **Wiener(최소평균제곱)** → 제약 최소제곱 순으로 전개 `[raw/books/digital-image-processing-2ed.md]`
- **Encoding**은 "fidelity 기준에 대한 부호화"로 구성 — error-free(차등/컨투어/run-length) → DPCM → transform → hybrid(RPV TV)의 3단계 사례 `[raw/books/digital-image-processing-2ed.md]`
- **Segmentation**은 discontinuity detection → edge linking(boundary) → thresholding → region → motion의 위계, **Description**은 chain code~문법(string grammar)까지의 기하-통계-언어 3축으로 정리 `[raw/books/digital-image-processing-2ed.md]`
- 제8장의 **Fourier descriptors·texture·shape numbers**는 영상 인식·영상 압축의 선행 단계로, MPEG 계열 부호화 문헌과 연결

## 관련
- 개념: [[image-processing-fundamentals]] — 이론(Gonzalez·Wintz) + Java 실무(Efford) + C 실무(NHK) 3책 비교
- 실무 계열: [[image-processing-java]] (Java 중심) · [[image-processing-practice-nhk]] (C 중심)
- 저자: [[rafael-gonzalez]] · [[paul-wintz]]
- 인접 분야(기존): [[ofdm-orthogonal-frequency-division]] · [[mimo-multiple-input-multiple-output]] — 주파수 영역/신호 처리 배경
