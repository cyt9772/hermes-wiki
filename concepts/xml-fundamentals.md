---
title: XML Fundamentals
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [xml]
sources: [raw/books/xml-for-www.md, raw/books/xml-10days.md]
confidence: high
---
# XML Fundamentals

## 5가지 원칙 (xml-for-www 1장)
1. **루트 요소** (root element) — 유일한 최상위
2. **중첩** (nesting) — 올바른 개/닫기
3. **속성** (attribute) — key="value" 쌍
4. **빈 요소** (empty/self-closing tag) — `<a/>`
5. **특수 5기호** — `&lt; &gt; &amp; &quot; &apos;` 또는 CDATA

## DTD vs XML Schema
| | DTD | XML Schema (XSD) |
|---|-----|-------------------|
| 타입 시스템 | × (명시적) | ✓ (xs:string, xs:int, ...) |
| 네임스페이스 | 제한적 | ✓ |
| 언어 | DTD 자체 (XML 아닌) | XML (XSD) 기반 |

## 관련 개념
- XML = SGML + HTML의 문제 의식 (xml-10days 제0일)
- XML ≠ 마크업 언어, **데이터 표현 언어** (메타 기술 언어)
- DTD: `<!DOCTYPE>`, XML Schema: `<xs:schema>`
- JSP + XML: 서버 측 동적 문서 (xml-10days 8-9일)

## Related
- [[xslt-styling]]
- [[xml-for-www]] / [[xml-10days]] (books)
- [[elizabeth-castro]] / [[yoshihiro-yamada]] (authors)
