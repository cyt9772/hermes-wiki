# Wiki Schema

## Domain
AI books & stock investing (AI 관련 책/도서 소스 + 주식·투자 분석).
- **AI 쪽**: AI/ML/LLM 관련 책의 핵심 개념, 저자, 주요 주장, 책 간 연결
- **Investing 쪽**: 종목/섹터/거시 분석, 회사 리서치, 밸류에이션, 투자 논지(thesis), watchlist

## Conventions
- File names: lowercase, hyphens, no spaces (e.g., `attention-mechanism.md`)
- Every wiki page starts with YAML frontmatter (see below)
- Use `[[wikilinks]]` to link between pages (minimum 2 outbound links per page)
- When updating a page, always bump the `updated` date
- Every new page must be added to `index.md` under the correct section
- Every action must be appended to `log.md`
- **Content language:** 페이지 본문은 한국어 또는 영어 혼용 가능 (소스 성격에 맞춰서).
  다만 파일명·태그·frontmatter 키는 항상 English.
- **Provenance markers:** 3+ 소스를 종합한 페이지에서 특정 소스에서 온 claim은
  문단 끝에 `^[raw/books/xxx.md]` 마킹으로 출처 연결.

## Frontmatter
```yaml
---
title: Page Title
created: YYYY-MM-DD
updated: YYYY-MM-DD
type: entity | concept | comparison | query | summary
tags: [from taxonomy below]
sources: [raw/books/source-name.md]
# Optional quality signals:
confidence: high | medium | low
contested: true
contradictions: [other-page-slug]
---
```

### raw/ Frontmatter
```yaml
---
source_url: https://example.com           # or book metadata (author, isbn, chapter)
ingested: YYYY-MM-DD
sha256: <hex digest of the raw content below the frontmatter>
---
```

## Tag Taxonomy
**AI:** book, chapter, author, concept, llm, ml-basics, deep-learning, agents, architecture, inference, training, alignment
**Investing:** stock, company, sector, macro, strategy, valuation, earnings, risk, korea-kospi, watchlist
**Meta:** comparison, summary, thesis, source

Rule: 모든 페이지 태그는 이 분류에 있어야 함. 새 태그 필요 시 먼저 여기 추가.

## Page Thresholds
- **생성**: 엔티티/개념이 2+ 소스 등장 OR 1 소스의 핵심이면 페이지 생성
- **합치기**: 기존 페이지가 있는 언급은 기존 페이지에 추가
- **생성 금지**: 단발성 언급, 도메인 밖 사안
- **분할**: 200줄 초과 시 서브토픽으로 분할 + 상호 링크
- **아카이브**: 내용 전부가 대체되면 `_archive/` 이동, index 제거

## Entity Pages (회사, 저자, 책)
- Overview, 핵심 사실/날짜, 관련 엔티티 ([[wikilinks]]), 근거 출처
- 책 엔티티 페이지: 저자, 핵심 тезис, 각 장 요약, 교훈, 관련 개념 링크
- 회사 엔티티 페이지: 비즈니스 모델, 핵심 지표, AI 관련성, 경쟁사, 밸류에이션 맥락

## Concept Pages
- 정의/설명, 현재 지식 상태, 미해결 논쟁, 관련 개념 링크
- 예: attention, moat, compound-interest, rpgm(RAG-Prompt-Grounding-Memory)...

## Comparison Pages
- 비교 대상과 이유, 비교 차원 (표 형식 권장), 종합 결론, 출처

## Update Policy
1. 날짜 우선 — 새로운 소스가 일반적으로 기존 내용을 대체
2. 진지한 모순이면 양쪽 입장을 날짜·출처 병기
3. frontmatter에 `contradictions:` 기록, lint 시 사용자에게 리뷰 요청
