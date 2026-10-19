---
title: MCP (Model Context Protocol)
created: 2026-10-19
updated: 2026-10-19
type: concept
tags: [ai, ai-agent, llm, mcp, protocol]
sources: [raw/books/ai-agent-dev-ollama.md, raw/books/ai-agent-engineering.md]
confidence: high
---
# MCP (Model Context Protocol)

> "에이전트가 도우미를 활용하는 표준 인터페이스" — 도구 연결의 USB-C 규격비유

## 개념
MCP = LLM/에이전트와 외부 도구·데이터소스 사이를 표준화한 프로토콜. 한 도구가 한 LLM 앱에 수작업 통합되던 것을 **규격 하나로 다수 연결**로 바꿔주는 개방 표준.

## 서별 전개
- **[[ai-agent-dev-ollama]] 9장 MCP 활용법 (p261)**: Smithery(마켓플레이스)·클로드 데스크톱 연결·MCP 서버를 쓰는 에이전트 작성 — 실습 프로젝트 2개로 마무리:
  - **Ch10**: 노션 MCP + 긱뉴스 MCP 조합으로 AI 뉴스 블로그 작성 자동화
  - **Ch11**: 위스퍼(목소리) + 로컬 LLM 멀티모달 자동 회의록
- **[[ai-agent-engineering]] Ch.4 Tools (p104)**: LangChain 도구 → **MCP** → 상태 유지 도구 → 도구 개발 자동화로 도구 계층을 확장. MCP를 "도구 생태계의 표준 커넥터"로 위치짓고, Ch.8 A2A(에이전트 간) 프로토콜과 대비.

## 관련
- [[ai-agent]] — MCP가 확장하는 것
- [[orchestration]] — 도구 호출을 조율하는 구조
- [[agent-harness]] — 하네스가 관리하는 도구 레이어
