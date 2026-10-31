---
title: HID — Human Interface Device (USB HID)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [usb-bus]
sources: [raw/books/usb-complete.md]
confidence: high
---
# HID (Human Interface Device)

USB 디바이스 클래스 중 **키보드·마우스·게임패드·조이스틱·스캐너·오디오 마이크** 등 **사람이 직접 조작하는 디바이스**를 위한 표준.

## 구조 (book 1, 11-13장)
- 제11장: **HID 제어와 인터럽트 전송** — HID는 인터럽트 전송으로 동작 (지연 민감, 소량)
- 제12장: **HID 리포트** (Report) — 리포트 타입(Input/Output/Feature), 리포트 디스크립터 (Report Descriptor), 컬렉션(Collections: Physical/Usage/Application)
- 제13장: **HID 애플리케이션** — OS 드라이버 스택

## 리포트 디스크립터 (Report Descriptor)
"릴레이 리포트 형식" — 바이너리 디코딩 표.
- **Usage Page**: 키보드(0x01), 마우스(0x02), 게임패드(0x0C) 등
- **Logical Min/Max**: 값 범위
- **Report Count / Size**: 바이트 수
- **Collection**: 논리 그룹
- **Input/Output/Feature**: 데이터 방향

## 특징
- **OS 독립** — Windows/Linux/macOS 모두 동일 HID 드라이버 제공
- **드라이버 불필요** — OS 내장
- **플러그 앤 플레이** — 즉석 인식

## Related
- [[usb-bus-architecture]] — 디바이스 클래스 중 하나
- [[usb-power-management]] — HID의 Sleep/Suspend
- [[computer-network-programming-book]] (저서) — HID는 OS의 입력 계층으로 동작
