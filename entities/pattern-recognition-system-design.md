---
title: 패턴 인식 시스템 설계 (MATLAB/Simulink, LMI)
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, pattern-recognition]
sources: [raw/books/pattern-recognition-system-design.md]
confidence: medium
---

# 패턴 인식 시스템 설계 (MATLAB/Simulink, LMI)

> 소개 (p7): '선형 행렬 부등식(LMI: Linear Matrix Inequality)을 이용하여 (시스템) 해석 및 설계를 하는 것이 실질적인 가치를 지니는 이유는 신뢰성 있고 효율적인 콘벡스(Convex) 최적화 기법에 의해 (시)스템 (해)석 및 설계 문제가 풀릴 수 있기 때문이다.'

## 개요
- **저자:** 박연묵 (Ph.D., 삼성전자 책임연구원 · 메커트로닉스, 미국 MIT 기전공학부, 한국과학기술원(KAIST) 박사)
- **출판:** 도서출판 아진(A-JIN), 2013 ©. MATLAB/Simulink 학생용 버전 포함
- **성격:** 선형 행렬 부등식(LMI)을 도구로 삼아 패턴 인식 시스템을 설계하는 공학 서적, PDF 148쪽. 최적화·로버스트 제어 툴박스 실습과 결합.

## 내용
- LMI 개념 입문: J.C. Willems에 의해 창안된 LMI의 용어와 의미를 쉽게 설명 (p7).
- 핵심 도구: `LMI Control Toolbox`와 `Robust Control Toolbox`(MATLAB)를 이용해 LMI로 표현된 문제를 푸는 절차 (p1).
- 적용 분야: 패턴 인식 시스템(Pattern Recognition System) 설계에서 LMI가 어떻게 쓰이는지 구체적 예로 다룸 — 국내에 관련 기법서·기술서가 드문 실정을 메우기 위한 목적 (p7).
- 부록/동봉: MATLAB & Simulink Student Version 및 Control/DSP/Image/Optimization/Signal/Statistics Toolbox 설치 안내, 학생용 버전 구매·학교/대학원 용도 제한 사항 (p3).
- 수학 기반: 선형 대수(행렬 부등식, 콘벡스 최적화)를 전제로 하는 패턴 인식 모델링 접근.

## 관련 페이지
- [[pattern-recognition-intro]] — 통계적 패턴인성 기초(밀도추정·분류기)와 LMI 설계 관점의 연계
- [[linear-system-theory-design]] — LMI와 로버스트 제어/시스템 설계를 다루는 선형 제어 이론서
- [[ai-introduction]] — 패턴인성 기법의 상위 영역인 인공지능 입문
