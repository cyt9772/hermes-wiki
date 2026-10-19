---
title: 검색증강생성 (RAG, Retrieval-Augmented Generation)
created: 2026-10-19
updated: 2026-10-19
type: concept
tags: [ai, ai-agent, llm, rag]
sources: [raw/books/ai-agent-dev-ollama.md, raw/books/ai-agent-engineering.md, raw/books/llm-ai-agent-7projects.md]
confidence: high
---
# 검색증강생성 (RAG)

> "검색증강생성" — 3권 모두 LLM 에이전트 기억/지식 계층의 핵심 구성요소로 다룸

## 개념
RAG = 외부 문서/지식베이스에서 **검색**한 관련 내용을 LLM 프롬프트에 **증강**해 환각 감소·최신 지식 접목을 해결하는 기술. 에이전트 '기억' 계층의 기본.

## 서별 전개
- **[[ai-agent-dev-ollama]] 5장 (p123)**: 로컬 환경 RAG 실습 — 올라마 임베딩 + 벡터 저장소 + 랭체인 RAG 체인 → PDF 텍스트 RAG까지. "LLM 학습에 없는 정보(최신 문서)를 런타임에 주입"하는 입문 경로.
- **[[ai-agent-engineering]] 6장 Knowledge & Memory (p158)**: RAG를 에이전트 메모리 설계의 한 축으로 위치 — 벡터 스토어, 시맨틱 경험 메모리(semantic episodic memory), 그래프 RAG(Graph RAG)까지 메모리 스펙트럼으로 확장.
- **[[llm-ai-agent-7projects]] 에이전트 5 (p311)**: LlamaIndex 기반 RAG 실전 — "검색증강생성이란 무엇인가(313) / 프롬프트 엔지니어링·RAG·파인튜닝의 위치 비교(314) / 사용자 관점의 RAG 과정(317) / RAG 기반 에이전트(319)" — 재무보고서 검색 예제.

## RAG vs 파인튜닝 (7projects서 314p 비교)
- RAG: 지식 업데이트가 빠르고 출처 추적 가능, 런타임 비용↑
- 파인튜닝: 모델에 내장돼 응답 스타일/도메인 어휘에 강점, 업데이트 비용↑

## 관련
- [[ai-agent]] — RAG가 매달리는 시스템
- [[ai-agent-engineering]] — Ch.6 메모리
- [[llm-ai-agent-7projects]] — Ch.9 (에이전트 5)
