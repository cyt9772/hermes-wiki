---
title: 시작하는 도커와 쿠버네티스
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, docker, kubernetes, container-swarm, orchestration, cloud]
sources: [raw/books/start-docker-kubernetes.md]
confidence: high
---
# 시작하는 도커와 쿠버네티스

> 원서 | 한국어판 | (출판사 확인 필요)
> 629p `raw/books/start-docker-kubernetes.md`

## 개요
"도커와 쿠버네티스가 가져온 변화"를 입문 관점에서 다루는 교과서. 1부에서 **도커 기본(1-2장) - 컨테이너 오케스트레이션 개념 - 도커 스웜(3장) - 서버 클러스터링 기본**을 학습하고, 2부에서 **쿠버네티스(4장 이후) - 네임스페이스 - 스커커 확장 - x509 인증**으로 넘어가며, 2부 말미에는 종합 실습을 배치 `raw/books/start-docker-kubernetes.md`.

## 장 구조 (2부 / 13장+)
| 부/장 | 핵심 |
|----|------|
| 1부 1장 | 도커 기본 사용법 (도커 엔진·컨테이너 조작) |
| 1부 2장 | 컨테이너의 기본 개념 (독립성·확장성) |
| 1부 3장 | 도커 스웜 (클러스터링·오케스트레이션) |
| 2부 4장 | 쿠버네티스 기본 |
| 2부 5-8장 | 네임스페이스·스케줄러·확장 |
| 2부 10장 | x509 인증서 기반 사용자 인증 |
| 2부 11-13장 | 커스텀 스케줄러·스케줄러 확장 |

`raw/books/start-docker-kubernetes.md`

## 특징
- **도커 스웜(3장)을 오케스트레이션 입문**으로 배치
- 2부에서 쿠버네티스의 네임스페이스·스케줄러·인증(10장)까지 다룸
- 컨테이너 오케스트레이션의 "왜"를 먼저 설명하는 입문 구조

## 핵심 컨셉 연결
- [[docker-kubernetes-essentials]] — Docker·K8s·오케스트레이션·마이크로서비스 클러스터
- [[docker-kubernetes-practical]] — 같은 도메인의 "현장 실무" 관점
- [[cloud-computing]] — 컨테이너 오케스트레이션이 지향하는 클라우드 인프라 맥락

## Related
- 개념: [[docker-kubernetes-essentials]], [[cloud-computing]]
- 관련: [[docker-kubernetes-practical]]
