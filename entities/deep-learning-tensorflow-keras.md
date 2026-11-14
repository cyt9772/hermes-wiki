---
title: 텐서플로와 케라스로 구현하는 딥러닝
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, deep-learning, tensorflow, keras, neural-networks]
sources: [raw/books/deep-learning-tensorflow-keras.md]
confidence: medium
---

# 텐서플로와 케라스로 구현하는 딥러닝

> "간단히 말해, 머신러닝 모델은 어떤 입력을 해당 출력으로 매핑하는 함수를 계산하는 방법이다." (p51)

## 개요
- **Author:** 아미타 카푸어 (Amita Kapoor) · 안토니오 굴리 (Antonio Gulli) · 수짓 팔 (Sujit Pal) 지음, 이병욱 옮김
- **Publisher:** 에이콘출판 (2023, 원서 *Deep Learning with TensorFlow and Keras* 1st ed., Packt 2022) | **Pages:** 856
- **Positioning:** Keras 창시자 프랑소와 숄레(François Chollet)가 "이론과 실제 사이에서의 균형이 잘 잡혀 훌륭하다"고 추천 (p6). TensorFlow/Keras 코드로 딥러닝을 구현하는 실무 입문서.

## 내용
- 1장 TF와 신경망 기초: 시그모이드·Tanh·ELU·LeakyReLU·ReLU 등 활성화 함수를 다루고, 비선형 활성화와 다층 구성으로 "거의 모든 것을 학습"할 수 있음을 설명 (p50).
- 지도학습 예제: MNIST(60,000장 훈련·10,000장 테스트, 28×28 grayscale)로 필기체 숫자 인식망을 만들고 원-핫 인코딩으로 라벨을 표현한다 — 숫자 3은 [0,0,0,1,0,0,0,0,0,0] (p51~52).
- 2장 회귀와 분류: 다변량 회귀를 행렬로 표현하고, 손실함수(최소 제곱오차의 합)와 그래디언트 하강·TensorFlow 최적기로 계수를 구한다 (p100).
- 선형 회귀를 위한 신경망: 선형 활성(activation=None)의 단일 Dense 계층이 일반화된 회귀자임을 보여주고, K.Sequential로 구축·훈련한다 (p101~102).
- 실무 습관: 신경망 입력은 정규화해야 하며(data.min()/max()), 가중치 곱셈이 발산하는 것을 막기 위해 순서화한다 (p102).

## 관련 페이지
- [[deep-learning-nvidia-guide]] — NVIDIA·역전파 중심으로 기초를 다지는 딥러닝 입문서
- [[tensorflow-explained]] — 텐서플로우 API/계산 그래프 기초를 먼저 다루는 서
- [[ai-ml-dl-intro]] — AI/ML/DL 역사와 개념 개요 입문서
- [[llm-ai-agent-7projects]] — AI/LLM 프로젝트 실무 계열
