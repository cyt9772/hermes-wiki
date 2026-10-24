---
title: 영상처리 프로그래밍 by Visual C++ (황선규 2007)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-processing, image-filtering, image-segmentation]
sources: [raw/books/image-processing-programming-visualc.md]
confidence: high
---
# 영상처리 프로그래밍 by Visual C++ (황선규 2007)

> 표지/원저: **황선규** (한양대학교 영상 처리 전공 박사, 실시간 특징점 정합·3D 객체 추적 연구)
> 출판: 한빛미디어 (주) IT EXPERT 시리즈, 2007 (초판 2007-05-25, 4쇄 2009-10), 848p

## 개요
Visual C++ 2005(MFC)로 영상 처리 알고리즘을 직접 구현하는 실무서. 이론서도 코드집도 아니라, 각 장마다 알고리즘의 이론적 배경을 먼저 풀어 놓고 바로 ImageTool이라는 통합 프로그램에 기능을 추가하는 구성이다 `[raw/books/image-processing-programming-visualc.md]`. 1부에서 BMP 포맷 분석과 DIB 처리용 **CDib 클래스**를 만들고 영상 입출력·화면 출력·복사/붙여넣기·확대 보기까지 되는 프로그램 틀을 세운 뒤, 2부에서 화질 향상(반전·명암비·감마·히스토그램 균등화)→산술/논리 연산→공간적 필터링→기하학적 변환(보간법)→주파수 공간 처리(DFT·FFT·저역/고역 필터)→특징값 추출(허프 변환·Harris 코너)→컬러 처리→분할(이진화·레이블링·외곽선 추적)→모폴로지→모양 기술자(푸리에 기술자·불변 모멘트)→동영상(AVI·움직임)까지 영상 처리 핵심 영역을 순서대로 다룬다. 부록에서 **OpenCV** 라이브러리 사용법과 웹 카메라 기반 침입자 감시 시스템 프로젝트를 실습으로 완성한다 `[raw/books/image-processing-programming-visualc.md]`.

## 장 구조 (권내 목차)
1. 영상 처리의 개요
2. Visual C++ 2005 시작하기
3. BMP 파일의 이해
4. CDib 클래스 만들기
5. 영상 처리 프로그램 틀 만들기 (ImageTool)
6. 화질 향상 기법 (반전/명암비/감마/히스토그램 균등화)
7. 영상의 산술 및 논리 연산
8. 다양한 공간적 필터링 기법
9. 영상의 기하학적 변환 (이동·크기·회전·반사, 보간법)
10. 주파수 공간에서의 영상 처리 (DFT/FFT/저역·고역 필터)
11. 영상의 특징값 추출 방법 (경계선·허프 변환·Harris 코너)
12. 컬러 영상 처리 (색 모델 변환·컬러 외곽선·히스토그램 균등화)
13. 영상 분할 (이진화·레이블링·외곽선 추적)
14. 모폴로지 연산 (침식·팽창·열기·닫기)
15. 모양 기술자 (외곽선 푸리에 기술자·불변 모멘트)
16. 동영상 처리 (AVI 재생·움직임 추출)
- 부록 A: OpenCV 이용하기 / 부록 B: 침입자 감시 시스템 만들기

## 핵심 내용
- **통합 프로그램 구조**: CDib(DIB 입출력·화면 출력·클립보드·픽셀 참조) + RGBBYTE(트루컬러 픽셀) 클래스를 직접 설계하고, 전 장의 알고리즘을 ImageTool에 기능을 쌓는 방식으로 구현 — 모든 예제가 하나의 프로그램으로 모인 점이 이 책의 특징 `[raw/books/image-processing-programming-visualc.md]`
- **BMP/DIB 포맷 실무**: 구조체(BITMAPFILEHEADER 등) 단위 BMP 파일 분석부터 화면 출력까지, 윈도우즈 기본 비트맵 포맷을 직접 파싱하는 과정을 상세히 다룬다
- **공간↔주파수 균형**: 공간적 필터링(평탄화/샤프닝/잡음 제거)과 이산 푸리에 변환·FFT·주파수 도메인 저역/고역 통과의 구현을 병행 — 영상 처리의 두 축을 모두 코드까지 연결
- **대상 독자**: 고등학교 수학 + C/C++ 문법 이상, Visual C++ 윈도우즈 프로그래밍 미숙자에게 적합 (저자서문)
- **활용법**: 이론은 Gonzalez·Wintz급 교과서([[digital-image-processing-2ed]])에서, 구현은 이 책과 함께 — 특히 MFC 기반 픽셀 단위 구현의 참고서로 쓸 만함

## 관련
- 저자: [[hwang-sun-kyu]]
- 개념: [[image-processing-programming]] — 영상 처리 프로그래밍 (C/C++/Java 구현)
- 인접: [[image-processing-java]] (Java 기반 DIP), [[image-processing-fundamentals]] (Gonzalez·Wintz 이론기초)
