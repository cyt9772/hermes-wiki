---
title: 임베디드 리눅스 스택 — 4단계 파이프라인과 3권 교재
created: 2026-11-07
updated: 2026-11-07
type: concept
tags: [embedded-linux, yocto, linux-kernel, bootloader, rootfs, concept]
sources: [raw/books/bbb-yocto-project.md, raw/books/gnu-linux-rapid-embedded.md, raw/books/embedded-linux-primer.md]
confidence: high
---
# 임베디드 리눅스 스택 — 4단계 파이프라인과 3권 교재

임베디드 리눅스는 호스트에서 타겟 보드용 **크로스 툴체인 → 부트로더 → 커널 → 루트 파일시스템**의 4단계를 만들어 탑재하는 구조다([[embedded-linux-build]] 참고). 이번 3권 모두 이 4단계를 다루지만 각축이 다르다: Yocto/BitBake 자동화(비글본), 하드웨어 주변장치 통합(BBB·SAMA5D3·Wandboard), 기초 이론+구조+부팅(다양한 아키텍처). 한 권은 "자동화/레시피", 한 권은 "주변장치 실습", 한 권은 "개념+디버깅".

## 4단계 파이프라인

1. **크로스 툴체인(toolchain)** — 호스트에서 타겟(ARM 등)으로 컴파일하는 GCC/LD/assembler. `raw/books/bbb-yocto-project.md` 제1장(호스트 환경 설정·필수 패키지), `raw/books/gnu-linux-rapid-embedded.md` 제3장(C 컴파일러·크로스 컴파일), `raw/books/embedded-linux-primer.md` 제2.3.8절·제12장(교차개발 환경)
2. **부트로더(bootrom/bootloader)** — 커널을 RAM에 로드하고 인계하는 첫 코드(MLO/U-Boot/SPL). `raw/books/bbb-yocto-project.md` 제1장(생성된 이미지: MLO, U-Boot, Image, dtb, 루트FS, 모듈), `raw/books/gnu-linux-rapid-embedded.md` 제1장·제2장(부트로더 둘러보기·uBoot 명령), `raw/books/embedded-linux-primer.md` 제7장(uBoot 구조·포팅)
3. **리눅스 커널(kernel)** — CPU/메모리/I/O 관리 OS 코어; 아키텍처·구성·초기화. `raw/books/bbb-yocto-project.md` 제8장(커널 무선 지원 활성화), `raw/books/gnu-linux-rapid-embedded.md` 제3장(커널 모듈·DTS 디바이스 트리), `raw/books/embedded-linux-primer.md` 제4장·제5장·제16장(구조·빌드·구동)
4. **루트 파일시스템(rootfs)** — 커널 위 사용자 공간; busybox·응용·라이브러리. `raw/books/bbb-yocto-project.md` 제6장(패키지 추가·패키지그룹·이미지 bbappend), `raw/books/gnu-linux-rapid-embedded.md` 제5장(JFFS2·UBIFS·Yocto), `raw/books/embedded-linux-primer.md` 제6장(루트FS·init·initrd·initramfs)·제11장(BusyBox)

## 책별 관점

- **bbb-yocto-project**(Irfan Sadiq; Packt 원본, 에이콘 한국어판) — 입문+실습. 제1장 비글본 부팅부터 제2장 BitBake, 제3장 helloworld 레시피, 제4장 멀티미디어, 제5장 레이어, 제6장 콘솔게임, 제7장 감시(V4L2·gstreamer), 제8장 무선AP. Yocto 레시피·레이어·패키지에 집중.
- **gnu-linux-rapid-embedded**(Rodolfo Giometti; Packt 원본) — 하드웨어 중심 실습. 제1장 개발 시스템(BBB·SAMA5D3·Wandboard), 제2장 콘솔 관리, 제3장 커널·드라이버, 제4장 데몬·스크립트, 제5장 임베디드 OS·Yocto, 제6~19장 GPIO·TTY·USB·I2C·SPI·1-Wire·이더넷·WLAN·CAN·SND·V4L·ADC·PWM·기타.
- **embedded-linux-primer**(Christopher Hallinan, 정보문화사 한국어판) — 개념+구조+부팅+디버깅의 종합 입문. 제2장 시스템 해부, 제4장 커널 구조, 제5장 커널 초기화, 제6장 루트FS·init, 제7장 부트로더, 제8장 드라이버, 제9장 파일시스템, 제11장 BusyBox, 제12~15장 개발환경·디버깅, 제17장 리얼타임.

## Related
- [[embedded-linux-build]]
- [[embedded-linux-yocto-project]]
- [[embedded-linux-systems-arm-an]]
- [[embedded-firmware-basics]]
- [[linux-kernel-structure]]
- [[raspberry-pi-iot]]
- [[embedded-linux-cross-dev-hae]]
- [[mastering-embedded-linux-programming]]
