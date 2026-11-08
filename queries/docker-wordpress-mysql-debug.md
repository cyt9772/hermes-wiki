---
title: Docker Desktop (Linux VM) + WordPress/MySQL 스택 구축 5단계 실패와 해결
created: 2026-11-08
updated: 2026-11-08
type: query
tags: [docker, container, database, debugging, tutorial, web-server]
sources: [raw/books/start-docker-kubernetes.md]
confidence: high
---

# Docker Desktop (Linux VM) + WordPress/MySQL 스택 구축 5단계 실패와 해결

> 2026-11-08 실습 기록. 『시작하는 도커와 쿠버네티스』 p.42 WordPress 예제를
> RTX5090 (Ubuntu 26.04, Docker Desktop 4.98.0 / LinuxKit VM)에서 그대로 수행하던 중
> 연쇄 실패 5건을 각각 진단 → 정상 구동(설치 페이지 도달)까지의 전 과정.

## 질문 (원점)

p.42 예제 — MySQL + WordPress 2컨테이너 스택을 호스트 볼륨에 올려 `ls`로
DB 파일 생성을 확인하는 연습. 4차례 실행이 모두 교재의 산출물과 달랐다:

1. `docker run ... -v /home/wordpress_db:workspace mysql:8.4`
   → `error while creating mount source path '/host_mnt/home/wordpress_db': mkdir ... permission denied`
2. 경로 교정 후 실행 → 컨테이너는 실행되나 `~/work/docker/`가 계속 비어 있음
3. Docker File Sharing에 `/work` 추가 후에도 여전히 비어 있음
4. 그 후엔 `--initialize ... data directory has files in it. Aborting`
5. DB 정상인데 WordPress 화면이 `Database Error`

## 배경: Docker Desktop (Linux) + VM 구조의 핵심

- Docker Desktop (Linux)은 엔진을 LinuxKit **VM 안에서** 실행. 컨테이너에 건
  `-v host:container`는 VM 내부로 `/host_mnt/...`로 바인드된다.
- **VM과 공유되지 않는 경로를 `-v`하면 에러가 뜨지 않는다.** 컨테이너 overlay FS
  (VM 로컬 디스크)가 조용히 마운트되고, 쓰이는 파일은 전부 VM에 갇힌다. (실패 3)
- `docker inspect .Mounts`의 `Source`/`RW:true`는 **마운트 의도이지 실체 증거가
  아니다.** 실체는 컨테이너 내 `df -T` 또는 양방향 파일 교환 테스트로 확인한다.

## 실패 1: `mkdir /host_mnt/home/wordpress_db: permission denied`

- 원인: (a) 대상 디렉터리가 호스트에 없으며 (b) 상위 `/home`이 `root:root 755`로
  yutae 계정에 쓰기 불가. 데몬(VM)이 자동 생성하려도 같은 거부.
- 재현: yutae로 `/home` 아래 `mkdir` → `Permission denied` 확인.
- 해결: `-v`에 **이미 존재하는 writable 경로**를 쓸 것. 꼭 원할 땐
  `sudo mkdir -p /home/wordpress_db && sudo chown 1000:1000 ...` 후 실행.

## 실패 2: DB 파일이 하나도 안 생김 (Exited 1)

- `-e MYSQL_ROOT_PASSWORD`에 **값이 없음** → 빈 문자열로 전달 →
  MySQL 8.4 엔트리포인트가 `Database is uninitialized and password option is not specified`
  로 초기화 전 종료. 파일을 남기지 않고 죽는 것이라 디렉터리가 비어 보임.
- 교훈: `-e KEY=VALUE` — 값 없는 `-e KEY`은 "빈 값"일 뿐 "무시"가 아니다.

## 실패 3: File Sharing 추가 후에도 디렉터리가 비어 있음 (가장 깊은 함정)

- 구조: `~/work` → **`/work` 심볼릭링크**이고, `/work`는 별도 디스크
  (`/dev/nvme0n1p1`). VM에서 심볼릭링크를 해석해 `File Sharing` 목록이
  실제 디바이스 `/work`를 포함하지 않음.
- 증거 체인 (전부 실측):
  - 컨테이너 내 `df -T /var/lib/mysql` → `overlay ... upperdir=/run/rootfs.upper`
    (호스트 디스크 아님)
  - 양방향 테스트: 컨테이너에서 쓴 파일이 호스트에 미소재, 호스트에서 쓴 파일이
    컨테이너에 미소재
  - `/work/docker_probe`에 `-v` 실행 → 명시 거부
    `The path /work/docker_probe is not shared from the host and is not known to Docker.`
  - 심볼릭링크 없이 홈 바로 아래 경로(`~/docker_direct`)는 양방향 정상 동작
- 해결: Docker Desktop Settings → Resources → **File Sharing**에 `/work` 추가 후
  컨테이너 재생성 (이후 마운트는 실질 동작 확인).

## 실패 4: `--initialize specified but the data directory has files in it. Aborting`

- 실패 3 진단 중 생성했던 프로브 텍스트 파일이 데이터 디렉터리(=`-v` 소스)에
  잔존 → MySQL `--initialize`가 "비어 있어야 한다"는 전제 아래 거부.
- 해결: 잔존 파일 제거 후 재실행. (즉 "파일 정리 + 재실행"이 정답이라는
  마지막 단계의 정답.)

## 실패 5: WordPress `Database Error` — 교재의 오타

- 사용 명령: `-e WORDPRESS_DB__PASSWORD=password` — **밑줄이 두 개**.
- 공식 `wordpress` 이미지의 `wp-config.php`는
  `getenv_docker('WORDPRESS_DB_PASSWORD', 'example password')`처럼 **PHP 실행 시**에
  밑줄 한 개의 변수명을 읽으므로, 밑줄 두 개 변수는 무시되고 기본값
  (`example username` / `example password`)으로 설정이 고착.
- 결과: `Access denied for user 'example username'@'...' (using password: YES)`
  → HTTP 500 `Error establishing a database connection`.
- 해결: `-e WORDPRESS_DB_USER=root -e WORDPRESS_DB_PASSWORD=***
  (`--link wordpressdb_hostvolume:mysql`가 `mysql` 호스트네임으로 DB를 해석하게
  해주므로 `DB_HOST` 기본값 `'mysql'`이 그대로 통함).
- 교훈: env 변수명 오타는 컨테이너 시작 시점이 아니라 **HTTP 요청 시점**에
  "Database Error"로만 표면화됨.

## 최종 검증 (정상 상태 도달)

- `~/work/docker`에 `ibdata1`, `mysql.ibd`, `#innodb_redo`, `undo_001/002`,
  `binlog.*` 등 InnoDB 데이터 정상 생성 — **교재 p.42 산출물과 일치**
- `docker ps`: `wordpressdb_hostvolume` / `wordpress_hostvolume` 모두 `Up`
- `curl -I http://localhost:40147/` → **HTTP 302 → `WordPress › Installation`**
  (설치 페이지 도달 = DB 연결 정상, 초기화 완료)
- 포트 40147은 Docker가 랜덤 할당한 값. 고정 원하면 `-p 8080:80` 명시.

## 재사용 체크리스트 (Docker on Linux VM + host volume)

1. `-v` 경로: 존재하는 writable 디렉터리 사용, 새로 만들면 `sudo` + `chown`
2. env 값: `-e KEY=VALUE` (값 없음 = 빈 값 = 의미 있는 차이)
3. 심볼릭링크/별도 장치: **realpath 기준**이므로 File Sharing에 실제 디바이스 경로 포함
4. 마운트 실체 검증: 컨테이너 내 `df -T` + 양방향 파일 교환. `inspect`로는 부족
5. 재생성 전 데이터 디렉터리 잔존 파일 정리 (MySQL `--initialize` 거부 방지)
6. `wordpress` 이미지 env: `WORDPRESS_DB_PASSWORD` / `WORDPRESS_DB_USER` —
   밑줄 개수 한 글자 단위 정사. DB 접속 오류가 HTTP 단계에서야 보임

## Related

- 교재: [[start-docker-kubernetes]] — p.42 WordPress 스택 예제 + p.45 볼륨 오버라이드 예제의 원문. [[docker-kubernetes-essentials]], [[docker-kubernetes-practical]] — Docker·K8s 개념·실무 클러스터

## 부록: p.45 볼륨 오버라이드 예제 "결과가 다른" 질문 (2026-11-08)

- 현상: `docker run -v ~/wordpress_db:/home/testdir_2 alicek106/volume_test` → 컨테이너에서 `ls /home/testdir_2` 빈 출력. 교재 회색 박스는 `auto.cnf ib_buffer_pool wordpress` 등이 보임.
- 원인(논리적): `-v` 오버라이드의 정의상 이미지의 `testdir_2`(안 `test` 파일)는 **호스트 디렉터리 내용으로 대체**됨. 호스트 디렉터리가 비어 있으면 컨테이너에도 비어 보이는 것이 **정상 결과**이며, 교재 저자의 `/home/wordpress_db`는 앞 실습으로 MySQL 데이터로 이미 채워진 상태였음.
- 검증: `hostfile.txt` 호스트 작성 → 컨테이너 `ls` 즉시 확인 (양방향 정상). `~/wordpress_db`는 방금 만든 빈 디렉터리 확인.
- 교재와 동일 산출물: `volume_dummy`(무마운트 → `test` 파일 확인) 후 `~/work/docker`(실제 InnoDB 데이터) 마운트 → 교재 회색 박스와 동일한 파일 목록. `~/wordpress_db`에 파일을 채우면 동일.
- 교훈: 실습 결과 불일치는 (1) 마운트 실체 (2) 호스트 소스 디렉터리의 **기존 내용** (3) 이미지 내부 기본값 — 이 3축으로 분리 진단할 것. 마운트가 살아 있어도 소스가 비면 컨테이너도 비어 보임 (교재 예제는 "전단계 산출물 재사용"을 전제로 함).
