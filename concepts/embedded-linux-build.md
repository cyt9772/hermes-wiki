---
title: 임베디드 리눅스 빌드 체인 (toolchain → bootrom → kernel → rootfs)
created: 2026-11-01
updated: 2026-11-01
type: concept
tags: [embedded-linux, build-system, arm, kernel, linux, concept, book]
sources:
  [raw/books/embedded-linux-systems-arm-an.md,
   raw/books/embedded-linux-yocto-project.md,
   raw/books/embedded-linux-cross-dev-hae.md,
   raw/books/mastering-embedded-linux-programming.md]
confidence: high
---
# 임베디드 리눅스 빌드 체인 (toolchain → bootrom → kernel → rootfs)

임베디드 리눅스 시스템은 호스트(개발자 PC)에서 **타겟 보드용** 코드와 이미지를 만들어 탑재하는 과정이다. 모든 4권 교재가 동일한 파이프라인을 공유한다: **크로스 툴체인(GNU toolchain) → 부트로더(bootrom) → 리눅스 커널 → 루트 파일시스템(rootfs)**. 각 장이 이 4단계를 다른 순서·다른 깊이로 서술하지만, 그 "단계"와 "방향"은 일치한다.

## 4단계 파이프라인

1. **크로스 툴체인(toolchain)** — 호스트에서 타겟 아키텍처(ARM/MIPS 등)로 컴파일·링크하는 GNU 컴파일러·리더·assembler 세트. `raw/books/mastering-embedded-linux-programming.md` 제2장
2. **부트로더(bootrom)** — 커널을 RAM에 로드하고 커널에게 실행 흐름을 인계하는 첫 코드. `raw/books/embedded-linux-systems-arm-an.md` 제15장, `raw/books/mastering-embedded-linux-programming.md` 제3장, `raw/books/embedded-linux-cross-dev-hae.md` 제14장
3. **리눅스 커널(kernel)** — CPU·메모리·I/O를 관리하는 OS 코어; 보드 디바이스 트리(BoD) 기반 커널 구성과 컴파일. `raw/books/mastering-embedded-linux-programming.md` 제4장, `raw/books/embedded-linux-cross-dev-hae.md` 제15장
4. **루트 파일시스템(rootfs)** — 커널 상에서 실행되는 초기 사용자 공간; busybox·응용프로그램·라이브러리. `raw/books/mastering-embedded-linux-programming.md` 제5장, `raw/books/embedded-linux-cross-dev-hae.md` 제16장

## 자동화 레이어
위 4단계를 **레시피(recipe)로 서술**하고 BitBake 엔진으로 조립하는 것이 **Yocto/OpenEmbedded**다. 이 레이어는 파이프라인 자체를 "데이터(레시피)로 표현"하는 것이다 `raw/books/embedded-linux-yocto-project.md` 제8장.

## 서별 전개
| 서적 | toolchain | bootrom | kernel | rootfs |
|------|-----------|---------|--------|--------|
| [[embedded-linux-systems-arm-an]] | 제15장 | 제15장 | 제16장 | 제18장 |
| [[embedded-linux-yocto-project]] | 제3장 | 제7장 | 제9장 | 제7장 |
| [[embedded-linux-cross-dev-hae]] | 제12장 | 제14장 | 제15장 | 제16장 |
| [[mastering-embedded-linux-programming]] | 제2장 | 제3장 | 제4장 | 제5장 |

- ARM 중심, 하드웨어 명령어부터: [[embedded-linux-systems-arm-an]]
- 레시피/BitBake 자동화 중심: [[embedded-linux-yocto-project]]
- 설계→구현→상용화 수동 파이프라인: [[embedded-linux-cross-dev-hae]]
- 툴체인→부트로더→커널→rootfs 순서 실무서: [[mastering-embedded-linux-programming]]

## Related
- 저자: [[park-jaeho]] (임베디드 리눅스 교재)
- 커널 심화: [[linux-kernel-development-love]], [[linux-kernel-programming-itepert]]
- 리눅스 활용: [[linux-essential-utilities]]
- 유닉스 시스템 프로그래밍: [[unix-advanced-programming]], [[unix-ipc-signals]]
