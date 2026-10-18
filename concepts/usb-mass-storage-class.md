---
title: USB Mass Storage Class (MSC)
created: 2026-10-18
updated: 2026-10-18
type: concept
tags: [usb-bus]
sources: [raw/books/usb-mass-storage.md, raw/books/usb-complete.md]
confidence: high
---
# USB Mass Storage Class (MSC)

USB Mass Storage Class: SCSI 계열 저장장치(HDD/SSD/플래시)를 USB로 접근할 때 OS가 표준 드라이버로 인식하는 **클래스 프로토콜**. 2000년대 플래시 드라이브 폭발의 원동력.

## 3계층 구조
```
┌──────────────────┐
│  OS (Windows·Linux) │  디스크(\\.\PHYSICALDRIVE0)로 보는 계층
├──────────────────┤
│  SCSI 명령 (CDB)  │  INQUIRY / READ(10) / WRITE(10)
├──────────────────┤
│  Bulk-Only Transport (BOT) │  CBW → data → CSW
├──────────────────┤
│  USB Bulk (Bulk-Only)  │
└──────────────────┘
```

## CBW — SCSI 명령 패킷 (32바이트 기본)
| Field | Size | 의미 |
|-------|------|------|
| Signature | 4 | 0x43425355 ('USBC') |
| Tag | 4 | 요청 식별자 |
| Data Transfer Length | 4 | byte 단위 |
| Flags | 1 | 0x00 (IN) / 0x80 (OUT) |
| LUN | 1 | Logical Unit Number |
| Command Length | 1 | CDB byte 수 (1~16) |
| CBW Data Buffer Offset | 4 | (PIM 사용 시) |
| Command Data Block | 16 | SCSI CDB 원본 |

## CSW — 응답 (13바이트)
- Data Residue (4b), CSW Status (1b: 0=Pass, 1=Fail, 2=Phase Error), Tag (4b)

## Related
- [[usb-bus-architecture]] — USB 구조
- [[usb-mass-storage-book]] — 전문서
