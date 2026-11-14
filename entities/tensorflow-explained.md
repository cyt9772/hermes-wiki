---
title: 엣지있게 설명한 텐서플로우
created: 2026-11-14
updated: 2026-11-14
type: entity
tags: [book, deep-learning, tensorflow, computation-graph, tensorboard]
sources: [raw/books/tensorflow-explained.md]
confidence: medium
---

# 엣지있게 설명한 텐서플로우

> "2015년 11월에 오픈 소스로 공개된 이후에, 현재 사용할 수 있는 가장 흥미로운 머신 러닝 라이브러리 중의 하나로써" (p4)

## 개요
- **Author:** Sam Abrahams · Danijar Hafner · Erik Erwitt · Ariel Scarpinelli 공저, 정기철 역
- **Publisher:** 홍릉과학출판 (2017, 원서 *TensorFlow for Machine Intelligence*, Bleeding Edge/Backstop 2016) | **Pages:** 300
- **Positioning:** TensorFlow 기초(설치·API)와 머신러닝을 분리해 다루는 초기 TensorFlow(1.x) 입문서 — "텐서플로우 공부"와 "텐서플로우를 이용한 머신 러닝 수행 방법"을 분리하는 것을 섹션 1의 목표로 삼는다 (p4).

## 내용
- 섹션 1(텐서플로우 API·기초·실습): 선형 회귀·로지스틱 회귀·클러스터링 등 간단한 ML 모델을 만들고, 그래프 표현 → 텐서플로우 코드 변환 → TensorBoard로 모델링 검증하는 흐름을 배운다 (p4).
- 섹션 2: 텐서플로로 고급 딥 모델(deep models)을 구현하는 법 (p5).
- 계산 그래프 기초: 모든 TensorFlow 프로그램의 핵심에는 계산 그래프가 있으며, 노드/에지(종속 관계) 개념과 'addition' 예(1+2=3)로 방향성 그래프 구조를 설명한다 (p52).
- 이름 영역(name scope): tf.name_scope로 그래프를 구성하면 A/B/C/D 네임 스코프가 Transformation 아래 2레이어 4스 코프로 배치되고, 같은 설정의 오퍼레이션(tf.sub/tf.mul, tf.add/tf.div)은 TensorBoard에서 동일 색으로 표시된다 (p100~101).
- 한계 논의: Kubernetes 지원 당시에는 여전히 개발 중, 커스텀 연산 개발 오버헤드가 크고 일부 기능이 아직 없다는 점을 짚는다 (p50).

## 관련 페이지
- [[deep-learning-tensorflow-keras]] — TensorFlow/Keras로 딥러닝 구현을 넘어가는 입문서
- [[deep-learning-nvidia-guide]] — 역전파·신경망 이론 기초를 함께 다루는 딥러닝 입문서
- [[ai-ml-dl-intro]] — ML/DL 개념과 역사 개요 입문서
- [[ai-agent-engineering]] — AI/LLM 실무 엔지니어링 계열
