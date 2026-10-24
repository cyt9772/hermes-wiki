---
title: Practical Digital Video with Programming: Examples in C (Mattison 1994)
created: 2026-10-24
updated: 2026-10-24
type: entity
tags: [book, engineering, image-processing, video-compression]
sources: [raw/books/practical-digital-video-c.md]
confidence: high
---
# Practical Digital Video with Programming: Examples in C (Mattison 1994)

> 표지/원저: **Phillip E. Mattison** (권내 소속/이력 기재 없음)
> 출판: John Wiley & Sons (Wiley Professional Computing), 1994, 540p (ISBN 0-471-31016-6 paper/disk)

## 개요
1994년, PC 위 **모션 비디오(motion video) 실전**서. "PC 모션 비디오는 TV를 대신할 재미가 아니라, 다른 수단으로 전달하기 어려운 정보를 point-to-point로 주고받는 수단"이라는 전제 아래, 카메라·디스플레이·색 표현·데이터 포맷·저장 기술·프로그래밍 환경·상업적 캡처 하드웨어·압축 표준까지를 **직관적 설명 → 구체적 상세** 순으로 다루고, 각 주제에 C/C++ 데모 소스(예: LPF_DEMO, HPF_DEMO, DDA_DEMO, CON_DEMO, NEG_DEMO, HUFFDEMO, VQ_DEMO, DCT encode/decode, AVI2VID)를 붙인다 `[raw/books/practical-digital-video-c.md]`. 압축 장에서는 컬러 서브샘플링(CCIR 601)·런 길이 인코딩·허프만 인코딩·벡터 양자화(FST)·DPCM·DCT(2D, 8×8 블록)·움직임 추정을 C로 구현하고, 저장 장에서는 CD(CCIR-656 직렬 영상 코드)·고정 디스크·나선 스캔 테이프·D1/D2 포맷을, 소프트웨어 장에서는 DOS/Windows DLL 환경, Windows용 비디오, AVI(RIFF), QuickTime를, 하드웨어 장에서는 Creative Video Spigot·Media Vision Pro Movie Studio·Intel Smart Video Recorder을 다룬다.

## 장 구조 (권내 Contents)
1. The Evolution of Information
2. Video Fundamentals (카메라, NTSC, PAL/SECAM, 양자화, 해상도)
3. Computer Display Systems (CRT/LCD, 프레임 버퍼, 2D 필터링, 변환 디바이스)
4. Color Representation (CIE, RGB, YUV, 변환)
5. Data Compression Techniques (서브샘플링, RLE, Huffman, VQ, FST, DPCM, DCT, motion estimation)
6. Video Data Storage (CD/CCIR-656, disk, helical tape, D1/D2)
7. Motion Video Capture Hardware (Video Spigot, Pro Movie Studio, Smart Video Recorder)
8. Motion Video Software Environment (DOS/Windows, DLL, VFW, AVI/RIFF, QuickTime)
9. Video Image Processing Techniques (spatial filtering, scaling, contrast, negative — C listings)
- Appendix A: Motion video and still image file formats
- Appendix B: DOS-based C++ source files
- Appendix C: About the software

## 핵심 내용
- **C 언어 중심의 비디오 구현**: 영상 처리 알고리즘(공간 필터, 스케일링, 콘트라스트, 화상)를 전부 C 데모로 제공 — "Practical Digital Video with Programming"이 서명에 들어간 이유 `[raw/books/practical-digital-video-c.md]`
- **1994년 시점의 표준·제품**: NTSC/PAL/SECAM, CCIR 601/656, VFW/AVI, QuickTime, MPEG/H.261을 언급하는 등 90년대 초 디지털 비디오 산업의 스냅샷 — MPEG 표준 상세는 "전문 교과서로 가라"며 배제(서문)
- **압축 기술 비교**: DPCM·DCT·VQ를 모두 실제로 계산해 비교할 수 있는 수준으로 제시 — 이후 MPEG 계열 부호화서와 함께 읽으면 부호화 배경이 명확해진다
- **활용법**: 시대적 위치로, 현대는 H.264/HEVC·FFmpeg로 대체되지만 AVI/RIFF 구조와 VFW 개념은 여전히 유효. [[video-compression-mpeg]] 등 MPEG 계열서와 함께 읽기

## 관련
- 저자: [[phillip-mattison]]
- 개념: [[image-processing-programming]] — 영상 처리 프로그래밍 (C/C++/Java 구현)
- 인접: [[mpeg-2-watkinson]] (MPEG 부호화), [[video-compression-mpeg]] (MPEG 표준 개요)
