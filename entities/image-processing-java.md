---
title: Digital Image Processing: A Practical Introduction Using Java (Efford 2000)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-theory, image-processing, image-filtering]
sources: [raw/books/image-processing-java.md]
confidence: high
---
# Digital Image Processing: Java로 하는 디지털 영상 처리 (Efford 2000)

> 표지/원저: **Nick Efford** (School of Computer Studies, University of Leeds)
> 출판: Addison-Wesley (an imprint of Pearson Education), First published 2000, 368p

## 개요
Java 언어로 디지털 영상 처리를 **구현부터 이론까지** 다루는 실무 교과서. 이미지의 물리적 획득(카메라·CCD·인간 시각, 제2장)과 디지털 표현(sampling·quantisation·RGB, 제3장)을 출발점으로, **Java 2D API(BufferedImage·Raster·BufferedImageOp)**를 이용한 영상 처리 프로그래밍(제4장)과 PGM/PPM·PNG 파일 입출력(제5장)을 실습 기반으로 잡는다 `[raw/books/image-processing-java.md]`. 후반부는 grey level·histogram equalisation(제6장), convolution·Canny edge·rank filter(제7장), **DFT·FFT·Wiener/역확산(filtering·deconvolution)**(제8장), affine 변환·warping·interpolation(제9장), thresholding·region growing·split & merge(제10장), **eroding/dilation/opening/closing·greyscale morphology**(제11장), 무손실 압축(delta/Run Length, 제12장)으로 이어지며, 모든 기법이 Java 코드로 구현되어 있다 `[raw/books/image-processing-java.md]`.

## 장 구조 (TOC 기반, 368p)
1. **Introduction** — images, image processing(concept examples: contrast, motion blur, warping)
2. **Imaging** — passive/active imaging, camera optics, CCD sensors, human eye, 3D imaging(stereoscopy, CT)
3. **Digital images** — sampling·spatial resolution·sampling pattern, quantisation, colour(RGB·other models), representation(8-bit greyscale, colour), volumetric data, OOP with images
4. **Images in Java** — Java 1.0/1.1 image API, producer/consumer, pixel data, **Java2D API**(BufferedImage, Raster/WritableRaster, DataBuffer, RasterOp/BufferedImageOp/BufferedImageFilter), Java Advanced Imaging
5. **Basic image manipulation** — storage media·file formats(**PBM/PGM/PPM, PNG**), Java reading/writing, display, printing, pixel data manipulation(ROI, geometric, 산술·논리)
6. **Grey level and colour enhancement** — grey level mapping(linear/non-linear), histograms, histogram equalisation, colour processing
7. **Neighbourhood operations** — convolution & correlation(Java 성능), linear filtering(low/high pass, high freq emphasis), edge detection(simple, Laplacian, **Canny**), rank filtering(median, min/max, range), hybrid & adaptive filters
8. **The frequency domain** — spatial frequency, Fourier theory(2D), DFT(스펙트럼, FFT, Java 구현), 스펙트럼 해석, filtering(low/high/band, 주기적 노이즈), **deconvolution**(PSF, inverse filter, **Wiener filter**)
9. **Geometric operations** — affine transformations(Java), transformation algorithms, interpolation(zero/first/higher order), affine image transformation, warping & morphing
10. **Segmentation** — thresholding(grey level/colour, Java tools), contextual(pixel connectivity, region similarity, **region growing**, split & merge)
11. **Morphological image processing** — structuring elements, **erosion·dilation**, **opening·closing**, hit & miss, morphological filtering, **greyscale morphology** (Java 구현)
12. **Image compression** — redundancy, performance, **lossless(delta compression, run length encoding)**

## 핵심 내용
- **Java 2D API**를 영상 처리의 표준 인터페이스로 가정: BufferedImage → Raster(WritableRaster) → DataBuffer 계층 구조를 먼저 정립하고 모든 알고리즘을 이 위에 구현 `[raw/books/image-processing-java.md]`
- **Canny edge detector**를 171절에서, **Wiener filter**와 **역확산(deconvolution)**를 제8장에서 PSF 개념과 함께 설명 — Gonzalez·Wintz의 이론적 복원과 실무 구현의 연결고리 `[raw/books/image-processing-java.md]`
- **Morphology**(제11장)는 structuring element·fitting·hitting으로 기본 개념을 잡은 뒤 erosion/dilation → opening/closing → hit & miss → greyscale morphology 순으로 전개, Java 클래스로 structuring element를 표현 `[raw/books/image-processing-java.md]`
- 전체 장이 **Exercises(프로그래밍 과제)**로 끝나고, CD-ROM에 도구 제공 — "읽고 코드를 바꾸어 실행한다"의 수업 구조 `[raw/books/image-processing-java.md]`
- 제12장 무손실 압축: **delta compression**과 **run length encoding**을 핵심 기법으로, Gonzalez·Wintz 제6장(image encoding)의 실무 버전 `[raw/books/image-processing-java.md]`

## 관련
- 개념: [[image-processing-fundamentals]] — 이론(Gonzalez·Wintz) + Java 실무(Efford) + C 실무(NHK) 3책 비교
- 이론 기초: [[digital-image-processing-2ed]] — Gonzalez·Wintz
- C 언어 실무: [[image-processing-practice-nhk]]
- 저자: [[nick-efford]]
