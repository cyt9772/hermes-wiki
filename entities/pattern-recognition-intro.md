---
title: 패턴인식 개론 (개정판)
created: 2026-11-15
updated: 2026-11-15
type: entity
tags: [book, pattern-recognition]
sources: [raw/books/pattern-recognition-intro.md]
confidence: medium
---

# 패턴인식 개론 (개정판)

> 저자 머리말 (p6): '이 책은 패턴인성을 공부하려는 입문자뿐만 아니라 인공지능, 데이터 마이닝에 관심이 많은 전기／전자／컴퓨터 관련학과의 대학원생이나 연구원을 대상으로, 각 주제의 핵심을 비교적 자세히 정리할 수 있도록 구성했습니다.'

## 개요
- **저자:** 한학용 (동아대학교 전자공학부, 음성·영상 신호처리 및 패턴인식 응용 전문)
- **출판:** 한빛아카데미, IT CookBook, 개정판 (초판 2014, ISBN 979-1156641-03)
- **성격:** MATLAB 실습을 통한 입체적 학습을 지향하는 패턴인식 입문 교재, PDF 562쪽. 선형대수·확률통계 기초부터 SVM·AdaBoost까지 19장.

## 내용
- 학습 로드맵: 대상패턴 → 특징 추출/선택 → 특징 변환(축소: PCA·LDA·ICA·MDS) → 분류기/패턴인식 (p10).
- 1장 패턴인성의 개요 — AI 철학적 논쟁, 분류기, 성능평가, 영문자·어류분류 사례 (p22-39).
- 2~4장 수학 기초 — 벡터/행렬, 행렬식·역행렬·고유값·SVD, 기초통계, 확률분포·가우시안 (p46-100).
- 5~6장 통계적 결정 이론, 최우추정(MLE), 선형·이차 분류기 (p101~).
- 7~9장 클러스터링(k-means, LBG 비균일 이진 분할), GMM, 비모수 밀도추정(커널, k-NN) (p152-~).
- 10~12장 PCA/KL 변환(얼굴인식 사례), LDA, ID3 결정 트리.
- 13~15장 인공신경망, 자기조직화 특징지도(SOM, 코호넨), 유전 알고리즘(순회판매원 문제).
- 16~19장 시계열(DTW 동적 시간 와arping), 음성인식의 HMM, SVM, AdaBoost — 각 장마다 MATLAB 실습 (p339~).
- 추천사(CAPTIG 대표 이동윤, p4-5)의 연구 준칙 3가지: 결합추구의 원리, 가능한 모든 패턴을 찾아내려는 노력, 축소의 원리.
- 참고문헌: Duda/Hart/Stork「Pattern Classification」、Webb「Statistical Pattern Recognition」、Franc/Hlavac「Statistical Pattern Recognition Toolbox」 등 (p12).

## 관련 페이지
- [[pattern-recognition-system-design]] — 패턴인식 모델링을 LMI(선형 행렬 부등식) 최적화로 설계하는 상보적 관점
- [[ai-introduction]] — 인공신경망·유전 알고리즘 장에서 겹치는 AI 입문서
- [[ai-ml-dl-intro]] — 분류·클러스터링·SVM 등 패턴인성 기법의 ML 이론적 배경
