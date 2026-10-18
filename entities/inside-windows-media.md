---
title: Inside Windows Media
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, media-frameworks]
sources: [raw/books/inside-windows-media.md]
confidence: high
---
# Inside Windows Media

**Microsoft Corporation** 지음 (New Riders, Macmillan USA, 1999-11 원서), Think.Tec 번역, 도서출판 Com&Books 1판 발행 2000-06, 351p. 펴낸이: 박수경. WMT 1.x 시대: ASF·ASX·WMV 중심의 스트리밍 미디어 개발 실무서.

## 구성 (Part 1-4 + 부록 A/B/C)
| Part | 장 |
|------|----|
| Part 1 시작하기 | 1. WMT 소개 · 2. 컨텐트 제작(비디오포맷·오디오·스튜디오 녹음) |
| Part 2 구성 요소 | 3. WMS 사용 · 4. WMP 사용 · 5. WMT 총정리 |
| Part 3 고급 사용 | 6. WMT 디자인/개발 · 7. WRM으로 미디어 파일 패키징 · 8. PPT 스트리밍 · 9. WMT 고급 활용 |
| Part 4 기본 개념 | 10. 디지털 압축·인코딩 원리 · 11. 네트워킹·프로토콜 (LAN/WAN·IP·WMS 클라이언트/서버 프로토콜·UDP·FEC·멀티캐스트·인텔리전트 스트리밍·TCF 한계) |
| 부록 | A. 오디오·비디오 캡처 카드 · B. 컨텐트 합법 사용 요령 · C. WMT 용어집 |

## 핵심 포인트
- ASF/ASX/WMV: ASF container, ASF Play List, WMP automation, Encoder→WMS→Client chain
- TCF (Transport Control Protocol) vs HTTP rollover, 인텔리전트 스트리밍 (TCP/UDP 프로토콜 자동 선택)
- Proxy auto-detection, receiver quality evaluation
- 멀티캐스트 vs 유니캐스트 · FEC (Forward Error Correction)

## Related
- [[streaming-media-architecture]] (concept)
- [[local-area-network]] (LAN 기초)
