---
title: Docker·Kubernetes 컨테이너 개발 실무
created: 2026-11-07
updated: 2026-11-07
type: concept
tags: [docker, kubernetes, container, devops, image, pod, service, concept]
sources:
  [raw/books/docker-kubernetes-practical.md,
   raw/books/start-docker-kubernetes.md]
confidence: high
---
# Docker·Kubernetes 컨테이너 개발 실무

Linux 컨테이너 기술 **Docker**와 오케스트레이터 **Kubernetes**를 활용한 DevOps 실무서 2권의 묶음. 둘 다 "Docker 이미지/컨테이너 → 스택(컴포넌트) → K8s 클러스터 → Pod/Service/Deployment"의 4단계를 공유하지만, 관점이 다르다.

## 4단계 커브
1. **Docker 개념·설치** — 컨테이너 vs VM, 이미지/레이어/레지스트리. `raw/books/docker-kubernetes-practical.md` 전 6장, `raw/books/start-docker-kubernetes.md` 제1-2장
2. **Dockerfile·Compose** — 이미지 빌드·레이어 최적화·Multi-stage·Compose 스탭. `raw/books/docker-kubernetes-practical.md` 제5-8장, `raw/books/start-docker-kubernetes.md` 제3-5장
3. **K8s 기초·클러스터** — Node/Pod/Service/Ingress/API. `raw/books/docker-kubernetes-practical.md` 제9-14장, `raw/books/start-docker-kubernetes.md` 제6-9장
4. **운영·확장** — Deployment·HPA·RBAC·Secret·Monitoring. `raw/books/docker-kubernetes-practical.md` 제15-20장, `raw/books/start-docker-kubernetes.md` 제10-15장

## 두 서적의 관점
| 서적 | 분량 | 관점 |
|------|------|------|
| docker-kubernetes-practical (야마다 아키노리/심효섭 역, 위키북스 2019) | 478p | 실무 중심 — Dockerfile→K8s 리소스 매핑 |
| start-docker-kubernetes (용찬호, 위키북스 2020) | 629p | 입문→중급 학습 곡선 — 개념 이해 → 스택 운영 |

## Related
- 상위 개념: [[orchestration]] (K8s 오케스트레이션), [[cloud-computing]]
- 인접: [[linux-kernel-structure]] (namespaces/cgroups = 컨테이너의 핵심 커널 기능)
- 실무: [[embedded-linux-build]] (이미지 빌드 → 컨테이너 배포)
