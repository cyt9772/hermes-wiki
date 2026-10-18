---
title: USB 대용량 저장장치 (USB Mass Storage, 2nd Ed.)
created: 2026-10-18
updated: 2026-10-18
type: entity
tags: [book, usb-bus]
sources: [raw/books/usb-mass-storage.md]
confidence: high
---
# USB 대용량 저장장치 (USB Mass Storage)

Jan Axelson 저, 성원호·최강민 옮김, 에이콘출판. 원서 "USB Mass Storage" 2nd Ed. (2002, Newnes/Elsevier)의 한국어 번역. **USB Mass Storage Class (MSC) 프로토콜·드라이버·하드웨어 설계 실무서.**

**인용 원문 (p.15):** "USB 2.0은 데이터 전송 속도를 480 Mbps로 향상시켰다. 이는 USB 대용량 저장장치 규격에서 정의한 최대 전송률이다."

## 이 책의 위치
[[usb-complete]](총론)의 7장 "Mass Storage"를 **전체 책 한 권**으로 확장한 전문서. USB MSC = 플래시 드라이브/하드디스크가 호스트 OS에서 "디스크"로 인식되는 표준 계층.

## 내용 구조 (원서 2판, 주된 장)
1. **USB 대용량 저장장치 개요** — MSC 클래스 소개, SCSI 명령어 매핑
2. **Bulk-Only Transport (BOT)** — MS를 전달하는 전송 계층: CBW(Command Block Wrapper) → 데이터 → CSW(Status)
3. **SCSI 명령어** — INQUIRY·READ CAPACITY·READ(10)·WRITE(10)·TEST UNIT READY·MODE SENSE
4. **플래시 메모리 USB** — flash controller, SPI/NAND 인터페이스
5. **하드 디스크 USB** — SATA/IDE↔USB 브리지
6. **드라이버** — Windows/Linux의 MSC 클래스 드라이버, WDM
7. **보안** — USB lock, read-only 플래시

## 핵심 개념 (SCSI 명령어)
| 명령 | 코드 | 역할 |
|------|------|------|
| INQUIRY | 12 | 디바이스 ID·제조사·프로토콜 질의 |
| READ CAPACITY | 25 | logical block 수·크기 |
| TEST UNIT READY | 00 | 준비 상태 확인 |
| READ(10) | 28 | LBA 기준 읽기 |
| WRITE(10) | 2A | LBA 기준 쓰기 |
| MODE SENSE | 1A | 모드 페이지 파라미터 조회 |

## BOT의 3단계 파이프라인
```
CBW (Command Block Wrapper)   ← 호스트 → 디바이스
  ├ Tag, dCBWLength, CBWFlags, LUN, CBWDataTransferLength(32-bit),
  │ CBWDataBufferOffset, LUN, Command Length, DBE(16-byte SCSI CDB)
데이터 패킷 (Bulk IN/OUT)
CSW (Command Status Wrapper)  ← 디바이스 → 호스트
  ├ Data Residue, Status, Tag
```

## Related
- [[usb-bus-architecture]] — 기본 구조 (usb-complete)
- [[usb-mass-storage-class]] — MSC 전문 개념 (아래)
- [[usb-complete]] — 총론
- [[jan-axelson]] — 저자
