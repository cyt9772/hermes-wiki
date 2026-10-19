---
title: AI 에이전트 엔지니어링
created: 2026-10-19
updated: 2026-10-19
type: entity
tags: [book, ai, ai-agent, llm, multi-agent, orchestration, security]
sources: [raw/books/ai-agent-engineering.md]
confidence: high
---
# AI 에이전트 엔지니어링 (AI Agent Engineering)

**원서:** *Building Applications with AI Agents* — Michael Albada
**한국어판:** 강민혁 옮김, **한빛미디어** 2026-01-23 초판 / 3쇄 2026-07-03, ISBN 979-11-7579-013-1, 400p

> "단일 에이전트와 멀티 에이전트 중 **어떤 방식으로 선택해야 하는가**, 그리고 그 전환의 시점과 기준을 실무자가 판단하는 사고방식을 제시한다." — 서문

## 구성 (Part 3부 / 13장)
- **Part 1 개념과 UX** — 1.에이전트(정의·유형·모델선택·동기→비동기·워크플로 vs 에이전트) · 2.시스템 설계(도구·메모리·오케스트레이션·설계 트레이드오프) · 3.UX 디자인(모달리티·컨텍스트 연속성·신뢰 커뮤니케이션)
- **Part 2 구축과 확장** — 4.도구(LangChain 도구·MCP·상태유지) · 5.오케스트레이션(ReAct·Plan-Execute·쿼리분해·성찰형) · 6.지식과 메모리(벡터스토어·RAG·시맨틱경험·그래프RAG) · 7.학습(비모수·SFT/DPO/RLVR) · 8.멀티에이전트(스웜·A2A·메시지브로커·액터)
- **Part 3 신뢰·운영·거버넌스** — 9.검증 및 측정(테스트·할루시네이션) · 10.모니터링(Grafana·ELK·Phoenix·Langfuse·OTel·섀도·카나리) · 11.개설퐁(피드백·A/B·베이지안 밴딧) · 12.보안(MAESTRO 위협모델링·LLM보안·거버넌스) · 13.인간-에이전트 협업(감독·투명성·공정성)

## 위치 (4권 내 차별점)
- 4권 중 **가장 이론·설계 중심** + **보안/거버넌스/운영(Ch9-13)을 단독으로 다룸** (MAESTRO, 섀도 모드, 카나리, A2A 프로토콜).
- "단일→멀티 전환 시점" 판단 프레임이 독보적.
- 실습 코드보다 **아키텍처 설계·트레이드오프** 위주.

## Related
- [[ai-agent]] [[orchestration]] [[rag]] [[mcp]] [[agent-harness]]
- [[michael-albada]] (저자)
- [[ai-agent-dev-ollama]] (실습) [[llm-ai-agent-7projects]] (프로젝트) [[harness-engineering]] (구조)
