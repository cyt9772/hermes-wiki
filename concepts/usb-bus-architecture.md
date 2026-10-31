---
title: USB 버스 아키텍처 (USB Bus Architecture)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [usb-bus, electrical-engineering]
sources: [raw/books/usb-complete.md, raw/books/usb-mass-storage.md]
confidence: high
---
# USB 아키텍처

## USB 4대 전송 방식 (book 1, 3장)
| 방식 | 용도 | 특징 |
|------|------|------|
| **제어 전송 (Control)** | 설정·열거·상태 질의 | 항상 소량의 데이터, 양방향 |
| **벌크 (Bulk)** | 대용량 데이터 (마사저지) | 오류 회피, 최대 대역폭 |
| **인터럽트 (Interrupt)** | 지연 민감 (키보드·마우스·게임패드) | 주기적 폴링, 소량 데이터 |
| **동기 (Isochronous)** | 실시간 (오디오) | 고정 시간 슬롯, 오류 허용 |

## 엔드포인트 (Endpoint)
"엔드포인트" — 디바이스 안의 **논리적 채널**. 각 디바이스는 1개 이상, 각 엔드포인트는 고유한 **BID (Bus ID) + Endpoint ID** 로 식별.

## 디바이스 클래스 (book 1, 7장)
USB는 "디바이스 클래스"로 동작을 표준화. 같은 클래스의 디바이스는 **동일한 드라이버**로 동작:
- **Communications** (모뎀·네트워크)
- **Human Interface Device (HID)** — 키보드/마우스/게임패드/조이스틱
- **Mass Storage** — USB 메모리·외장 HDD
- **Printer / Image / Audio / Video**
- **Wireless (Wireless USB)**
- **Vendor-Specific**

## 호스트 컨트롤러 (HCD — Host Controller Driver)
- USB 1.1: UHCI (USB Host Controller Interface)
- USB 2.0: EHCI (Enhanced USB Host Controller)
- USB 3.0: xHCI (eXtensible Host Controller Interface)
- **HCD**: 하드웨어를 직접 조작하는 드라이버 (book 1, 6장 "칩 선택")

## 버스 토폴로지
"허브" (Hub)로 스타 구조를 재귀적으로 확장. USB 2.0 기준 최대 5개 허브, 127개 디바이스.

## USB 3.0 (SuperSpeed) — book 1 4판의 핵심
- 대역폭 480Mbps (USB 2.0) → **5Gbps** (USB 3.0)
- Full-rate (12Mbps) / High-speed (480Mbps) / SuperSpeed (5Gbps) 3속도
- **호환성** — USB 2.0 디바이스는 USB 3.0 포트에서 480Mbps로 동작
- **케이블** — USB 3.0은 별도 초록색 커넥터 (SS 9핀)
- **전원** — 5V 900mA (USB 2.0) 유지, 데이터는 슈퍼스피드로

## Related
- [[usb-hid]] — HID 클래스 특화
- [[usb-mass-storage-book]] — Mass Storage 클래스 + SCSI 매핑
- [[usb-power-management]] — Sleep/Suspend
- [[osi-7-layer-model]] — USB는 물리(1)+데이타링크(2)+응용(7) 단순 구조
