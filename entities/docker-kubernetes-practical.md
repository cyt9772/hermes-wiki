---
title: 실전 도커와 쿠버네티스
created: 2026-11-07
updated: 2026-11-07
type: entity
tags: [book, docker, kubernetes, container, devops, immutable-infrastructure, vagrant]
sources: [raw/books/docker-kubernetes-practical.md]
confidence: medium
---
# 실전 도커와 쿠버네티스

> 원서(일본어) | 한국어판 | (출판사 확인 필요)
> 478p `raw/books/docker-kubernetes-practical.md`

## 개요
"현장에서 바로 활용할 수 있는 컨테이너 개발 기법과 실전 기술"이라는 부제로, **도커(이해·설치·명령어·Dockerfile) - 불변 인프라 - Vagrant - 쿠버네티스로 이어지는 컨테이너 실무**를 다룸. 가상화 대비 컨테이너의 장·단점, 레지스트리(이미지 저장소), 불변 인프라(멱등성) 개념을 실무 관점으로 정리 `raw/books/docker-kubernetes-practical.md`.

## 장 구조 (CHAPTER 체제)
| 장 | 핵심 |
|----|------|
| 1 | 도커 이해 및 설치 (컨테이너 가상화 개념·레지스트리·Vagrant) |
| 2 | 도커 명령어 (Dockerfile 작성·이미지/컨테이너 조작) |
| 5-6 | 쿠버네티스 (Pod·ReplicaSet 등 오케스트레이션) |
| 9 | Vagrant (VM 기반 개발 환경과 컨테이너 비교) |

`raw/books/docker-kubernetes-practical.md`

## 특징
- **불변 인프라(Immutable Infra) 개념을 반복 강조** — 멱등성·복제성 관점
- 컨테이너 vs 서버 가상화 비교를 1장 전반에 배치
- 도커·쿠버네티스·Vagrant 3종 실습을 현장 관점으로 연결

## 핵심 컨셉 연결
- [[docker-kubernetes-essentials]] — Docker·K8s·오케스트레이션·마이크로서비스 클러스터
- [[start-docker-kubernetes]] — 시작하는 Docker/K8s (개념 입문)과의 대비
- [[cloud-computing]] — 불변 인프라·클라우드 배포 맥락

## Related
- 개념: [[docker-kubernetes-essentials]], [[cloud-computing]]
- 관련: [[start-docker-kubernetes]]
