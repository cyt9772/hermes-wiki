---
title: XSLT — Extensible Stylesheet Language Transformation
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [xml]
sources: [raw/books/xml-for-www.md, raw/books/xml-10days.md]
confidence: high
---
# XSLT — Extensible Stylesheet Language Transformation

XML 문서를 HTML/SVG/오직서로 변환하는 XML 기반 스타일 시트. `xml-for-www` (개념)와 `xml-10days` (제2-4일)가 함께 다룸.

## 기본 구조
```xml
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
  <xsl:template match="/">
    <html><body>
      <xsl:apply-templates/>
    </body></html>
  </xsl:template>
  <xsl:template match="title">
    <h1><xsl:value-of select="."/></h1>
  </xsl:template>
</xsl:stylesheet>
```

## 핵심 기능 (xml-10days L3-L9)
- `xsl:apply-templates` — 트리기 순회
- `xsl:for-each` / `xsl:sort` — 순차 처리·정렬
- `xsl:value-of` / `xsl:attribute` — 값·속성 출력
- `xsl:if` / `xsl:choose` — 조건 분기
- `xsl:variable` — 지역변수
- **xPath** — 위치 경로·함수 (L8), `concat()`, `number()`, `date()` 등

## xPath (위치 경로)
- `//book[price>50]` — 조건 필터
- `book/title[1]` — n번째 자식
- `preceding-sibling::author` — 이전 형제
- `normalize-space()` — 공백 정규화

## Related
- [[xml-fundamentals]]
- [[xml-10days]] — XSLT 실습
- [[yoshihiro-yamada]] (author)
