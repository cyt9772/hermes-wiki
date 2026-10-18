---
title: Streaming Media Architecture (Windows Media era)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [media-frameworks, network-programming]
sources: [raw/books/inside-windows-media.md]
confidence: high
---
# 스트리밍 미디어 아키텍처

## ASF/ASX/WMV 계층 (2000년 초)
```
[ASF Container]  ←  멀티미디어 컨텐트 (오디오+비디오+메타)
   ↑ ASX(ASF Play List)를 참조하는 경우
[WMP / WM Encoder / WMS]
   ↑ TCF or HTTP
[Client (WMP) ←(LAN/WAN)→ Proxy ← WMS]
```

## 전송 방식
- **유니캐스트** (client-to-client 1:1, WMS) — TCP 기반, TCF/HTTP rollover, FEC으로 packet loss 보상
- **멀티캐스트** (1:many, 1 WMS → N client) — 수신측 bandwidth·loss에 민감, FEC 필수
- **인텔리전트 스트리밍** — TCF → UDP → HTTP 순으로 자동 전환
- **Proxy** — 클로버·대역폭·auth 등 정책 적용, 프록시 자동 탐지

## Related
- [[inside-windows-media]] (book)
- [[tcpip-complete]] (network base)
