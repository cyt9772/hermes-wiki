---
title: USB 완전정복 (USB Complete, 4th Ed.)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, usb-bus, electrical-engineering]
sources: [raw/books/usb-complete.md]
confidence: high
---
# USB 완전정복 (USB Complete, 4th Ed.)

> "USB는 누구의 도움 없이 책으로 쓰기에는 너무나도 큰 주제다" — 저자 서문 p.5
> "USB는 역사상 가장 성공한 범용 인터페이스" — 번역 서문 p.8
> 원서: Jan Axelson, *USB Complete: The Developer's Guide, 4th Ed.* (2010), Lakeview Research
> 국내 번역: 신진철, 디오이즈 감수, **에이콘출판 2011** (ISBN 89-5727-152-7), 628p

## 개요
USB(Universal Serial Bus) **3.0(SuperSpeed)까지**를 개발자 관점에서 다룬 실무서. 20장 구조.
"USB 관련 개발 업무는 예전에 비해 쉽다. 칩 제조사에서 거의 모든 것을 제공하기 때문이다. 그러나 모든 개발이 그렇듯 **한 번에 잘 되는 일은 없다**" `[raw/books/usb-complete.md]` p.6-7

## 장 (chapter) 구조
| # | topic | 핵심 |
|---|-------|------|
| 1 | USB 기초 | 사용상 제약·이점·한계·USB vs 이더넷 (p.33-60) |
| 2 | USB 전송 | 전송 기초·패킷 형식·링크 관리 (p.69+) |
| 3 | 용도별 전송 방식 | 제어/벌크/인터럽트/동기 (p.105+) |
| 4 | 열거 | Descriptor 열거 절차 (p.139+) |
| 5 | 제어 전송 | 설정·확인 (p.175+) |
| 6 | 칩 선택 | 컨트롤러·HCD (p.199+) |
| 7 | 디바이스 클래스 | Mass Storage/HID/Communication (p.229+) |
| 8 | 호스트와 통신 | 드라이버 모델 (p.285+) |
| 9 | 디바이스와 드라이버 결합 | (p.301+) |
| 10 | 디바이스 감지 | 하드웨어 변경 (p.325+) |
| 11-13 | **HID (Human Interface Device)** | 제어와 인터럽트 전송 · 리포트 · HID 애플리케이션 (p.365-444) |
| 14 | WinUSB | (p.445+) |
| 15 | 허브의 모든 것 | (p.477+) |
| 16 | **전원 관리** | 섌프·섌프/섌프 (p.497+) |
| 17 | 테스트와 디버깅 | (p.521+) |
| 18 | 버스상의 패킷 | (p.539+) |
| 19 | 전기적·물리적 인터페이스 | (p.557+) |
| 20 | 임베디드 시스템용 호스트 | (p.593+) |

## 핵심 인용
- **범용성**: "USB는 역사상 가장 성공한 **범용 인터페이스**다. 첫 이니셜 U의 Universal이라는 단어에서 알 수 있듯이 USB는 그야말로 만능 인터페이스" `[raw/books/usb-complete.md]` p.8
- **USB 3.0 (SuperSpeed) FAQ** (p.64-68): 기능·호환성·케이블·전원 4가지로 정리
- **디버깅 어려움**: "특히 장착/제거, 원인 불명의 인식 오류, 호스트 리부팅, 저전력 문제 등에 직면하면 디버깅이 어렵고 힘들다. USB는 고속인 데다가 스펙 자체가 복잡하기 때문이다" `[raw/books/usb-complete.md]` p.8
- **개발자 관점**: "USB-IF가 정의한 분야를 골고루 다룬다. 개발자의 입장에서 USB를 설명하고 어떻게 접근해야 할지를 알려주는 책은 세계적으로 이 [책]" `[raw/books/usb-complete.md]` p.7

## 주의 (추출 품질)
- 본 PDF는 **내장 텍스트 레이어가 있어 OCR 없이 pdftotext로 추출**
- 일부 OCR/텍스트 깨짐: `nlicrocnginecrrng`(미크로엔지니어링 랩스), `rIJSB`('USB' 깨짐) — 토큰 교차 확인
- **WinUSB**는 2000년대 후반 등장한 API — 4판(2010)부터 포함

## Related
- 저자: [[jan-axelson]] — USB·Serial Port·임베디드 네트워킹 전문
- 개념: [[usb-bus-architecture]], [[usb-hid]], [[usb-power-management]]
- 관련 책: [[usb-mass-storage-book]] — 같은 저자, USB Mass Storage Class 특화
- 관련: [[osi-7-layer-model]] (USB는 물리/데이타링크/응용 3계층 단순 구조)
