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

## [2026-10-05] ingest | 박곰희 투자법 (pakhomxi-investing)
- Source: /Down/전자책/박곰희 투자법.pdf → raw/books/pakhomxi-investing.pdf (23.5M, SHA-256 cf6bd6bf…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 299/299 pages → raw/books/pakhomxi-investing.md
- Created: entities/pakhomxi-investing.md (박곰희·박동호, 인플루언셜 2020-12, ISBN 979-11-91056-36-5)
- Created: concepts/asset-allocation.md, concepts/rebalancing.md, concepts/etf-investing.md, concepts/investment-asset-class.md
- chapter divider(p20/40/85/114/234) OCR garbled → 본문에서 주제 재구성, flag

## [2026-10-05] ingest | 미국 주식으로 은퇴하기 (retire-with-us-stocks)
- Source: /Down/전자책/미국 주식으로 은퇴하기.pdf → raw/books/retire-with-us-stocks.pdf (26.7M, SHA-256 bf0a4c6c…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 244/244 pages → raw/books/retire-with-us-stocks.md
- Created: entities/retire-with-us-stocks.md (황금부엉이·CIP 최철, (주)첨단, 2020~21 추정 — CIP 연도 OCR garble)
- Created: concepts/compound-interest.md, concepts/us-equity-market.md, concepts/index-investing.md, concepts/retirement-planning.md
- Parallel ingest race: dividend·etf·asset-allocation 페이지는 동시대 타 책 소스 → dividend 페이지는 생략(충돌 회피), 링크 purged

## [2026-10-05] ingest | 시대의 1등주를 찾아라 (find-the-top-stock)
- Source: /Down/전자책/시대의 1등주를 찾아라.pdf → raw/books/find-the-top-stock.pdf (SHA-256 6920bd5e…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 296/296 pages → raw/books/find-the-top-stock.md
- Created: entities/find-the-top-stock.md (이한영, 페이지2룩스 2021-09-08, ISBN 979-11-90977-38-8)
- Created: concepts/top-picking.md, concepts/momentum-investing.md, concepts/relative-strength.md, concepts/sector-rotation.md
- 증거 종목: 삼성전자·LG전자·포스코·SK하이닉스 등 + Package substrate 밸류체인(부록 p291-294)

## [2026-10-05] ingest | 배당왕 (dividend-king)
- Source: /Down/전자책/배당왕.pdf → raw/books/dividend-king.pdf (SHA-256 2734bd70…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 254/254 pages → raw/books/dividend-king.md
- Created: entities/dividend-king.md (삼성증권 리서치센터, 출판사 OCR상 미확인, 2019~20)
- Created: concepts/dividend-investing.md, concepts/dividend-growth.md, concepts/dividend-yield.md, concepts/payout-ratio.md
- 수치 토크(p034 회복률, p129 배당성향 28%) OCR 가독성 낮음 → "(OCR)" 표기로 flag

## [2026-10-05] ingest | 행동 경제학 (behavioral-economics)
- Source: /Down/전자책/행동 경제학.pdf → raw/books/behavioral-economics.pdf (SHA-256 ee14e779…)
- OCR: tesseract 5.5.3 (kor+eng, 300dpi), 343/343 pages → raw/books/behavioral-economics.md (18,522줄)
- Created: entities/behavioral-economics.md (도모노 노리오 著, 이명희 譯, 지형 2007-01, ISBN 89-957370-5-0)
- Created: concepts/loss-aversion.md, concepts/endowment-effect.md, concepts/anchoring-effect.md, concepts/mental-accounting.md, concepts/framing-effect.md, concepts/time-preference.md
- chapter-5(p132) 제목 garble → TOC p020에서 재구성 flag; 영문 저자명 OCR garble(Knetsch→60100 등) flag

