---
title: 영상 처리 프로그래밍 (Image Processing Programming)
created: 2026-10-24
updated: 2026-10-24
type: concept
tags: [engineering, image-processing, image-filtering]
sources: [raw/books/image-processing-programming-visualc.md, raw/books/digital-image-processing-implementation.md, raw/books/practical-digital-video-c.md]
confidence: medium
---
# 영상 처리 프로그래밍 (Image Processing Programming)

영상 처리 이론을 프로그래밍 언어(C/C++, Windows MFC/Win32, Java)로 **직접 구현**하는 실전 분야. 픽셀 단위 연산·공간/주파수 필터·기하 변환·분할·모폴로지를 알고리즘이 아니라 동작하는 윈도우 프로그램(또는 Java 애플리케이션)으로 만들어 검증하는 접근. 이론은 Gonzalez·Wintz류 교과서가 담당하고, 이 개념 페이지는 "구현" 축의 책들을 묶는다.

## Visual C++ 기반 구현 (한국, 1999→2007)
MFC/Win32 위주의 두 세대 한국어 실무서.

### Visual C++를 이용한 디지털 영상처리의 구현 (장동혁 1999)
- MFC 기초(문서/뷰/메인프레임, 직렬화) + **RAW 파일 포맷**으로 입출력을 정립하고, 픽셀 연산·히스토그램·기하 변환·윤곽선 검출(Sobel/Prewitt/Roberts/Laplacian/Canny)·모폴로지·FFT·이진화·세선화·마스크 필터링까지 장마다 소스·실행 파일을 실음 `[raw/books/digital-image-processing-implementation.md]`
- "주된 알고리즘은 어떤 언어로도 변환 가능하도록 독립적 프로그래밍" — 언어에서 추상화된 알고리즘 중심 구현 `[raw/books/digital-image-processing-implementation.md]`
- 마지막 장에서 **OpenGL**(AUX 라이브러리, 애니메이션, 원근/안개 효과)로 이어감 — 정지 영상 처리 → 3D 그래픽스의 확장 `[raw/books/digital-image-processing-implementation.md]`

### 영상처리 프로그래밍 by Visual C++ (황선규 2007)
- **CDib + RGBBYTE 클래스 설계**로 BMP/DIB 입출력·화면 출력·클립보드·픽셀 참조를 자체 구현하고, 전 장의 알고리즘을 ImageTool 하나의 프로그램에 기능을 쌓는 통합 구조 `[raw/books/image-processing-programming-visualc.md]`
- 화질 향상(감마·히스토그램 균등화)→산술/논리 연산→공간적 필터→기하 변환(보간법 3종)→**DFT·FFT·주파수 필터**→허프 변환·Harris 코너→컬러→분할(이진화·레이블링·외곽선 추적)→모폴로지→모양 기술자→AVI 동영상·움직임 추출의 완결된 커리큘럼 `[raw/books/image-processing-programming-visualc.md]`
- **객체 추적 프로젝트**: 부록에서 OpenCV 웹 카메라 입력 + 본문의 영상 처리 기법으로 침입자 감시 시스템을 만들어 JPG로 저장 — 이론→구현→프로젝트로 이어지는 구조 `[raw/books/image-processing-programming-visualc.md]`
- OpenCV 라이브러리(CDib 연동) 사용법을 부록으로 포함 — 순수 MFC 구현과 오픈소스 라이브러리 활용의 절충 `[raw/books/image-processing-programming-visualc.md]`

## C 언어 기반 비디오 프로그래밍 (영문, 1994)
### Practical Digital Video with Programming: Examples in C (Mattison 1994)
- 정지 영상 처리보다 **모션 비디오**에 초점: NTSC/PAL/SECAM·양자화·해상도, 디스플레이, CIE/RGB/YUV 색 표현, CCIR 601/656, 캡처 하드웨어, VFW/AVI(RIFF)·QuickTime 소프트웨어 환경 `[raw/books/practical-digital-video-c.md]`
- 각 알고리즘(스페이스 필터, 스케일링, 콘트라스트, 화상, Huffman, VQ, DPCM, 8×8 DCT 인코딩/디코딩)마다 **C 데모 소스**를 붙여 동작시키는 방식 — "Programming, Examples in C"의 취지 `[raw/books/practical-digital-video-c.md]`
- 1994년 디지털 비디오 산업 스냅샷: Video Spigot·Pro Movie Studio·Intel Smart Video Recorder, D1/D2 테이프, CD CCIR-656 직렬 영상 코드 `[raw/books/practical-digital-video-c.md]`

## 비교 (구현 축)
| 차원 | 장동혁 1999 | 황선규 2007 | Mattison 1994 |
|---|---|---|---|
| 언어/환경 | Visual C++ (MFC, 1999) | Visual C++ 2005 (MFC) | C/C++ (DOS/Win32, VFW) |
| 입출력 | RAW 포맷 | BMP/DIB (CDib 자체 구현) | AVI/RIFF, CCIR-656, 파일 포맷 부록 |
| 커버리지 | 정지 영상 12종 기법 | 정지 영상 + 동영상(AVI) + OpenCV + 프로젝트 | 정지 + 모션 비디오 + 압축 + 캡처 HW/SW |
| 특징 | OpenGL까지 확장 | 통합 프로그램 구조, 객체 추적 프로젝트 | C 데모 코드 중심, 당시 표준·산업 |

## 관련
- 책: [[image-processing-programming-visualc]] · [[digital-image-processing-implementation]] · [[practical-digital-video-c]] · [[image-processing-java]]
- 저자: [[hwang-sun-kyu]] · [[jang-dong-yeop]] · [[phillip-mattison]]
- 인접: [[image-processing-fundamentals]] (이론 교과서 축) · [[image-processing-practice-nhk]] · [[video-compression-mpeg]] · [[streaming-media-architecture]]
