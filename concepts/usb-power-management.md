---
title: USB 전원 관리 (USB Power Management)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [usb-bus]
sources: [raw/books/usb-complete.md]
confidence: high
---
# USB 전원 관리

USB 16장 "전원 관리"의 주제. USB는 전원 공급(5V VBUS)을 버스 자체로 하므로, 전원 상태 관리는 데이터 상태와 분리된 독립 계층이다.

## 3단계 전력 상태
| 상태 | 설명 |
|------|------|
| **Working** (정상) | 5V VBUS 공급. 디바이스별 한도: USB 1.1 100mA / 2.0 500mA / 3.0 900mA |
| **Suspend** (선택적 절전) | 호스트가 3초 이상 버스 활동 없는 디바이스를 절전 상태로 전환. 디바이스는 **3ms 이내에 Suspend에 진입**하고, Resume 시 10ms 이내 정상 동작해야 함 |
| **Remote Wakeup** | Suspend 중에도 디바이스(키보드·마우스 등)가 호스트를 깨울 수 있는 특권 |

## Selective Suspend
"USB 2.0의 Selective Suspend는 디바이스별로 Suspend 여부를 선택할 수 있다" — OS가 개별 엔드포인트 수준에서 절전을 제어.
- 디바이스가 **Selective Suspend capable**이라면 OS가 개별 제어
- 그렇지 않다면 디바이스 전체가 Suspend

## Power Policy (OS 수준)
- Windows: `Power Policy`에서 디바이스별 Suspend 허용 (device property)
- Linux/Unix: `pm_runtime_put()` / `usbsuspend` 계열 API
- **Self-powered vs Bus-powered** — 디바이스가 자체 전원을 가졌을 때 전원 요청량과 OS의 정책이 달라진다

## Related
- [[usb-bus-architecture]] — USB 기본 구조
- [[usb-hid]] — HID의 Suspend/Remote Wakeup
- [[usb-complete]] (책) — 16장 전원 관리
