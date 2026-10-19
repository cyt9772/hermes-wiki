---
title: 하네스 엔지니어링 with 클로드 코드
created: 2026-10-19
updated: 2026-10-19
type: entity
tags: [book, ai, ai-agent, agent-harness, claude-code, multi-agent]
sources: [raw/books/harness-engineering.md]
confidence: high
---
# 하네스 엔지니어링 with 클로드 코드

**황민호** 지음, **한빛미디어** 2026-06-11 초판 / 3쇄 2026-07-15, ISBN 979-11-7579-059-9, 307p.
깃허브: <https://github.com/revfactory> (하네스 스킬·에이전트 템플릿 공유)

> "병목은 능력이 아니라 **구조**다." — Ch.1
> "챗봇과 싸우지 말고, **하네스를 설계하라.**" — 미셸 하시모토 (권말 epigraph)

## 구성 (Part 4부 / 14장)
- **Part 1 하네스란 무엇인가** — 01 왜 하네스인가 (49→79pt 실험, 5가지 오해) · 02 3분 Quick Start (2인 팀: commit-author/reviewer)
- **Part 2 하네스 구성하기** — 03 책임 분리(에이전트=Who, 스킬=How, 오케스트레이터=When/Whom) · 04 에이전트 정의(역할 계약서) · 05 스킬 설계(Progressive Disclosure) · 06 오케스트레이터
- **Part 3 하네스 스킬로 구성하기** — 07 메타스킬 6단계 파이프라인 · 08 6가지 아키텍처 패턴 · 09 팀/서브에이전트/하이브리드 · 10 하네스 등록과 진화(CLAUDE.md 포인터, Phase 0 감사)
- **Part 4 하네스 실전편** — 11 리뷰팀 · 12 풀스택 기능 구현(로그인) · 13 레거시 마이그레이션(3,500 테스트) · 14 디버깅/RCA

## 위치 (4권 내 차별점)
- **단일 주제 집중** — "에이전트 팀을 둘러싼 구조(하네스) 설계"만 전담.
- **클로드 코드(Claude Code) 특화** — CLAUDE.md, Subagent, Slash Command 등 CLI 에이전트 운영 실무.
- 4권 중 **팀/조직 단위 에이전트 운영** 관점 (개인 실습 → 팀 → 리드 개발자).

## Related
- [[agent-harness]] [[orchestration]] [[ai-agent]]
- [[hwang-minho]] (저자)
- [[ai-agent-engineering]] (멀티에이전트 이론) [[ai-agent-dev-ollama]] (도구 실습) [[llm-ai-agent-7projects]] (프레임워크)
