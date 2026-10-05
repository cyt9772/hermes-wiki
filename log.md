# Wiki Log

> Chronological record of all wiki actions. Append-only.
> Format: `## [YYYY-MM-DD] action | subject`
> Actions: ingest, update, query, lint, create, archive, delete
> When this file exceeds 500 entries, rotate: rename to log-YYYY.md, start fresh.

## [2026-10-05] create | Wiki initialized
- Domain: AI books & stock investing (AI 관련 책 소스 + 주식·투자 분석)
- Structure created: SCHEMA.md, index.md, log.md, raw/, entities/, concepts/, comparisons/, queries/

## [2026-10-05] ingest | 세븐테크 (The Seven Technologies, 2022)
- Source: /Down/전자책/세븐테크.pdf → raw/books/seventech.pdf (SHA-256 30e9...aed9)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 219/219 pages → raw/books/seventech.md 내장
- Created: entities/seventech.md, entities/kim-mi-kyung.md
- Created: concepts/artificial-intelligence.md, concepts/blockchain.md, concepts/robotics.md, concepts/iot.md, concepts/cloud-computing.md, concepts/metaverse.md
- index.md updated (7 pages), 5G 장 저자 OCR상 불분명 → 원서 대조 flag

## [2026-10-05] ingest | 금리의 역습 (rate-counterattack)
- Source: /Down/전자책/금리의 역습.pdf → raw/books/rate-counterattack.pdf (13M)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 204/204 pages → raw/books/rate-counterattack.md
- Created: entities/rate-counterattack.md
- Created: concepts/interest-rates.md, concepts/interest-rates-inflation.md, concepts/credit-cycle.md, concepts/fx-and-interest-rates.md
- Fixed pre-existing drift: blockchain.md 販売→판매, robotics.md 前→전직
- Author name not reliably OCR'd → flagged for cover/title-page cross-check

