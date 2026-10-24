---
title: Visual C++를 이용한 디지털 영상처리의 구현 (장동혁 1999)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-processing, image-filtering, image-segmentation]
sources: [raw/books/digital-image-processing-implementation.md]
confidence: high
---
# Visual C++를 이용한 디지털 영상처리의 구현 (장동혁 1999)

> 표지/원저: **장동혁** (권내 저자 소개·소속 기재 없음)
> 출판: PC 어드밴스 (PC ADVANCE Publisher, 발행인 김성은), 1999, 309p (ISBN 89-7785-061-4)

## 개요
1999년, 한글 Visual C++ 영상 처리 구현서. 영상 처리 분야의 **보편화**를 목표로, 전공이 아니어도 "알고리즘은 어떤 언어로도 변환 가능하도록 독립적으로 프로그래밍"된 코드 위주로 구성했다 `[raw/books/digital-image-processing-implementation.md]`. 1부에서 디지털 영상처리의 개념·활용분야(생물학·인공위성·문서 처리·공장 자동화·의료 진단 영상·영화 효과·인터넷 방송)와 MFC 기초(MFC 프로젝트 생성, 직렬화 Serialize, 문서/뷰/메인프레임 객체)·RAW 파일 포맷·CTestDoc/CTestView/CChildFrame 클래스로 준비를 마치고, 2부에서 픽셀 연산(사칙연산, Saturation/Wrapper)→히스토그램 분석·개선(균등화·스트레칭·로그 생성자)→기하학적 변환(크기 확대/축소·회전·보간·반사)→윤곽선 검출(Sobel·Prewitt·Roberts·Laplacian·Canny)→모폴로지(침식/팽창/열기/닫기, 이진+그레이)→주파수 공간 변환(FFT 정/역방향, 저주파/고주파 통과 필터)→이진화(블록/동적)·세선화→마스크 필터링(블러링/샤프닝)→**OpenGL** 기초(AUX 라이브러리, 애니메이션, 원근/안개 효과)까지 각 장마다 소스 코드와 실행 파일을 구현으로 끝낸다.

## 장 구조 (권내 목차)
1. 디지털 영상처리(DIP)의 개념과 활용분야
2. Visual C++ 프로그래밍의 이해 I (MFC/리소스 편집기/직렬화)
3. 디지털 영상처리를 위한 준비와 Visual C++ 프로그래밍 기법 (RAW 포맷, CTestDoc 등)
4. 픽셀 단위 이미지 연산 + 실제 구현
5. 히스토그램 분석과 개선 (평활화·스트레칭·로그)
6. 기하학적 변환 (크기·회전·반사·보간법)
7. 그레이 평면 윤곽선 검출 (Sobel/Prewitt/Roberts/Laplacian/Canny)
8. 모폴로지 기법 (이진·그레이)
9. 주파수 공간에서의 변환 (FFT, 저/고주파 필터)
10. 디지털 영상의 개선 기법 (블록·동적 이진화, 세선화)
11. 마스킹(행렬 조작)을 이용한 픽셀 필터링 (블러링/샤프닝)
12. 그래픽(그래픽스) 구현을 위한 OpenGL (AUX, 애니메이션, 안개 효과)

## 핵심 내용
- **실무 1세대**: 1999년 시점의 Windows MFC + 펜티엄 PC 환경에서 영상 처리를 "직접 구현"하는 흐름을 정립 — CD에 장별 소스·실행 파일과 RAW 영상 데이터를 함께 제공 `[raw/books/digital-image-processing-implementation.md]`
- **알고리즘 독립성**: "주된 알고리즘은 어떤 언어로도 변환이 가능하도록 독립적으로 프로그래밍되어 있다" — Visual C++를 쓰지 않아도 알고리즘 중심 독서가 가능(저자서문)
- **윤곽선 검출 체계**: Sobel·Prewitt·Roberts·Laplacian·Canny 마스크를 차례로 구현 — 경계선 검출의 교과서적 진행 순서
- **OpenGL까지 확장**: 영상 처리 코드를 넘어 AUX 라이브러리로 3D 애니메이션·안개(원근) 효과를 구현, 미디어 프로그래밍으로의 확장 예
- **활용법**: 역사적 위치(90년대 말 실무서)로, [[image-processing-programming-visualc]](2007)와 함께 MFC 영상 처리 구현의 계보를 보는 자료. 현대적 재구현은 MFC 대신 OpenCV를 쓰는 것이 유효

## 관련
- 저자: [[jang-dong-yeop]]
- 개념: [[image-processing-programming]] — 영상 처리 프로그래밍 (C/C++/Java 구현)
- 인접: [[image-processing-programming-visualc]] (2007, 이후 세대 MFC DIP) · [[image-processing-java]] (Java 기반 DIP)
