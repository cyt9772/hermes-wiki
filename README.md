# Hermes LLM Wiki — AI Books & Investing

Hermes Agent가 읽고/쓰고/유지보수하는 markdown 지식기반 (Karpathy LLM Wiki 패턴).
주제: **AI 관련 책/도서 소스** + **주식·투자 분석**.

## 구조
- `SCHEMA.md` — 구조 규칙, frontmatter, 태그 분류 (에이전트 행동 기준)
- `index.md` — 전체 페이지 카탈로그 (섹션별)
- `log.md` — 액션 로그 (append-only)
- `raw/` — Layer 1: 변경 불가 원본 소스 (books / articles / reports)
- `entities/` — Layer 2: 회사, 저자, 책 등 엔티티 페이지
- `concepts/` — Layer 2: 개념/주제 페이지 (attention, moat, RAG…)
- `comparisons/` — Layer 2: 비교 분석
- `queries/` — Layer 2: 저장할 가치가 있는 질답

## 동기화
이 디렉토리는 GitHub private 저장소와 git으로 연동됩니다.
(Hermes 에이전트가 session 시작 시 `git pull`, 작업 후 `git commit && git push`를 수행)
