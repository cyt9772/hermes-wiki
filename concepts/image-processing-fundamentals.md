---
title: 디지털 영상 처리 기초 (Digital Image Processing)
created: 2026-10-24
updated: 2026-10-31
type: concept
tags: [engineering, image-theory, image-processing]
sources: [raw/books/digital-image-processing-2ed.md, raw/books/image-processing-java.md, raw/books/image-processing-practice-nhk.md, raw/books/digital-image-processing-2kor.md, raw/books/digital-image-processing-c-ki.md, raw/books/image-processing-matlab.md, raw/books/practical-image-processing-matlab.md, raw/books/dsp-image-matlab-charbit.md]
confidence: medium
---
# 디지털 영상 처리 기초 (Digital Image Processing)

**디지털 영상 처리**는 analog 영상(빛, 전기 신호)을 **이산 화소(pixels)의 2차원 배열**로 표본화·양자화하여 디지털 데이터로 변환한 뒤, **향상(enhancement) → 복원(restoration) → 분할(segmentation) → 압축(encoding)**의 파이프라인으로 정보를 추출·변형·축소하는 기술이다 `[raw/books/digital-image-processing-2ed.md]` `[raw/books/image-processing-java.md]` `[raw/books/image-processing-practice-nhk.md]`

## Digital Image Processing (Gonzalez·Wintz 1987) — 이론 체계
- **이미지 모델**: 2D 신호 s(x,y) — 표본화(spatial)·양자화(tonal)로 디지털화; 인접 화소의 연결성(4/8), 거리(Euclidean/Chessboard/City), 산술·논리 연산까지 기본 관계로 정의 `[raw/books/digital-image-processing-2ed.md]`
- **변환 도구**: 2D DFT의 분리가능성·병진·주기·켤레대칭·회전·convolution-correlation 특성 + FFT + Walsh/Hadamard/DCT + Hotelling + **Hough transform**(feature extraction) `[raw/books/digital-image-processing-2ed.md]`
- **향상/복원**: histogram equalization/specification/local → smoothing(average·median·lowpass) → sharpening(미분·highpass) → **Wiener(최소평균제곱)·inverse filtering·제약 최소제곱**; degradation model = h*x = y + n `[raw/books/digital-image-processing-2ed.md]`
- **압축/분할/기술**: differential·contour·run-length encoding → DPCM → transform → hybrid(RPV TV); segmentation(edge·threshold·region·motion); description(chain code·shape number·Fourier descriptor·texture·string grammar) `[raw/books/digital-image-processing-2ed.md]`

## Digital Image Processing: Java (Efford 2000) — Java 실무
- **표본화·양자화·RGB 모델**을 개념으로 잡은 뒤 **Java 2D API(BufferedImage → Raster/WritableRaster → DataBuffer)** 계층 구조를 영상 처리의 표준 인터페이스로 활용 `[raw/books/image-processing-java.md]`
- **Canny edge detector·rank filtering(median·range)·hybrid/adaptive filter** — Gonzalez·Wintz 제4장의 Java 구현 버전 `[raw/books/image-processing-java.md]`
- **DFT·FFT·spectral interpretation** + **Wiener/역확산(deconvolution by PSF)** — 주파수 영역 이론과 Java 구현 통합 `[raw/books/image-processing-java.md]`
- **Morphology(erosion/dilation/opening/closing/hit-and-miss)** + **greyscale morphology** — Gonzalez·Wintz 제2판(1987)에는 없는 기법, Java 클래스로 structuring element 표현 `[raw/books/image-processing-java.md]`
- **무손실 압축**: delta compression + run length encoding — 실질 코드 중심 `[raw/books/image-processing-java.md]`

## C 언어에 의한 화상처리 실무 (NHK, 한국어 1999) — C 실무
- **목적별 독립장**: 임계값 추출(물체) → 미분/그라디언트/라플라시안/Prewitt(윤곽) → 평활화/메디안(잡음 제거) → 콘트라스트/히스토그램 평탄화(보기 쉽게) → 특징 파라미터/라벨링 `[raw/books/image-processing-practice-nhk.md]`
- **컬러**: RGB↔YUV 변환·휘도·채도·색상 조작·2차원 히스토그램·RGB 임계값·화면 합성 `[raw/books/image-processing-practice-nhk.md]`
- **기하학 변환**: 확대·축소·이동·회전·투시 변환 — 선형 보간법 + **동차 좌표** `[raw/books/image-processing-practice-nhk.md]`
- **주파수 영역**: DFT 이론(오일러 공식·진폭·위상) + **2차원 FFT·2차원 컨볼루션 C 구현** `[raw/books/image-processing-practice-nhk.md]`
- **압축**: run-length + **DPCM** + **하프만(가변길이)** 부호화 C 구현 + DCT 압축 칼럼 `[raw/books/image-processing-practice-nhk.md]`

## 3책 비교
| 주제 | Gonzalez·Wintz (이론, 1987) | Efford (Java, 2000) | NHK (C, 1999) |
|---|---|---|---|
| 표본화·양자화 | 이미지 모델 + nonuniform 방식 | spatial resolution + sampling pattern | 표본화·양자화 기초 |
| 향상(enhancement) | histogram + spatial smoothing/sharpening | grey level mapping + histogram equalisation + colour | 콘트라스트 강조 + 히스토그램 평탄화 + 컬러 부가 |
| 복원(restoration) | Wiener + inverse + 제약 최소제곱 (수학적 체계) | Wiener + deconvolution (PSF, Java) | (부각 없음) |
| 분할(segmentation) | edge·threshold·region·motion (8가지 기법) | thresholding + region growing + split&merge | 임계값 추출 + 특징 파라미터 + 라벨링 |
| 압축(encoding) | differential/contour/run-length/DPCM/transform/hybrid | delta + run length (lossless) | run-length + DPCM + 하프만 + DCT |
| 형태론(morphology) | (2판에 없음) | **제11장 전편**(erosion/dilation/opening/closing/greyscale) | (부각 없음) |
| 언어/구현 | (MATLAB 등, 언어 독립) | **Java 2D API** | **표준 C** |
| 교육 목표 | 이론·수학 4년 차 수준 | 프로그래밍 실무 + 실험 | 엔지니어 실무 + C 소스 |

## 2000s~2015 배치 추가 — 한국어판·MATLAB·C 실무
### Gonzalez·Woods·Rice 한국어판 (1996, 866p)
- **Digital Image Processing** (Gonzalez·Woods·Rice, U. Tennessee·U. Michigan)의 한국어 번역 — 공간 영역/변분/부호화/복원/합성/분할까지 한 권 `[raw/books/digital-image-processing-2kor.md]`
- 기존 [[digital-image-processing-2ed]](Gonzalez·**Wintz**, 2nd Ed 1987)와 **구분**: 원저 제목은 같지만 저자(Woods·Rice)·판차 다름 `[raw/books/digital-image-processing-2kor.md]`

### 디지털 영상처리 (C 언어) — Ohmsha 원저, 성안당 1998
- NTSC / Pseudo-NTSC 색신호 분산·동기·색상 처리 (C 구현) `[raw/books/digital-image-processing-c-ki.md]`
- FIR/IIR 필터, FF Filter, Edge/Noise/Geometric 보정 — VTR·전자줌 실용 알고리즘 `[raw/books/digital-image-processing-c-ki.md]`
- FFT/DCT 기반 부호화, MPEG 연계 — C 코드 실습 중심 `[raw/books/digital-image-processing-c-ki.md]`

### MATLAB 영상처리 2권 (2005/2012)
- **MATLAB을 이용한 디지털영상처리** (Gonzalez·Woods·Eddins 2nd Ed, McGraw-Hill Korea 2012, 746p) — 1D/2D 신호·공간 색공간(RGB/YCbCr/HSV)·공역/주파수 필터(`imfilter`)·복원·분할·형태학·JPEG 계열 압축 `[raw/books/image-processing-matlab.md]`
- **MATLAB 실용 영상처리** (정성환·이문호, 홍릉 2005, 441p) — 컬러 공간·히스토그램·명암 변환, 공간 필터/마스크/모폴로지/보간, DCT·Hough·MPEG 연계 `[raw/books/practical-image-processing-matlab.md]`

### DSP × Image 통합
- **신호처리·이미지처리 MATLAB** (Blanchet·Charbit 2008, 794p) — DSP(DFT·IIR·FIR) + 영상(2D DCT·에지·모폴로지) 동시 실습 — [[digital-signal-processing]] 축과 본 개념의 접점 `[raw/books/dsp-image-matlab-charbit.md]`

## 관련
- 책: [[digital-image-processing-2ed]] · [[image-processing-java]] · [[image-processing-practice-nhk]]
- 추가: [[digital-image-processing-2kor]] (Gonzalez·Woods·Rice 한국어) · [[digital-image-processing-c-ki]] (C 언어 Ohmsha) · [[image-processing-matlab]] (MATLAB 2nd) · [[practical-image-processing-matlab]] (MATLAB 실무) · [[dsp-image-matlab-charbit]] (DSP+Image 통합)
- 저자: [[rafael-gonzalez]] · [[paul-wintz]] · [[nick-efford]]
- 인접 개념(기존): [[ofdm-orthogonal-frequency-division]] — DFT/FFT 공용 배경
- 인접 분야(기존): [[rf-engineering]] · [[microwave-engineering]]
