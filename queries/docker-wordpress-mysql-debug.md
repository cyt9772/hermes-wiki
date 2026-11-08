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

## 부록2: Docker Desktop → 네이티브 엔진 전환 후 "Error establishing a database connection" 재발 체인 (2026-11-08)

Docker Desktop 3개의 구조적 함정(VM 파일 공유, 심볼릭링크 해석, `/host_mnt` 권한)을 제거하기 위해
Docker Desktop을 제거하고 네이티브 `docker-ce` 엔진으로 전환한 뒤 같은 스택을 재부팅하던 중
새로운 실패 체인이 발생했다. 체인 전체 + 교훈 정리:

### 체인 1: `docker-credential-desktop` 실행 파일 없음 (이미지 pull 차단)

- 현상: `docker run --rm hello-world` → `error getting credentials - err: exec: "docker-credential-desktop": executable file not found in $PATH`
- 원인: Docker Desktop이 `~/.docker/config.json`에 `"credsStore": "desktop"`을 남김. CLI는
  이 스토어의 실행 파일을 호출해 인증을 받으려 하고, Desktop 제거 후엔 실행 파일이 사라져
  **모든 registry 접근**(pull/login)이 실패. 컨테이너 실행과는 무관한 CLI 단계의 차단.
- 해결: `~/.docker/config.json`에서 `credsStore`, `plugins`, `features` 키 제거.
  보호 파일이라 직접 patch 불가 → Python 스크립트로 수정, `config.json.bak-*` 백업.
- 검증: `hello-world` 정상 pull·실행.

### 체인 2: `invalid reference format` + `-e: command not found`

- 현상: 백슬래시 줄 연속(`\`)이 담긴 `docker run` 명령이 `invalid reference format` →
  `-e: command not found`, `-v: command not found`으로 조각나 shell이 분리 해석.
- 추측된 원인: 줄 끝에 `\` 뒤 공백/CR(붙여넣기 유래)이 섞여 shell이 줄을 거기서 끊음.
- 검증 안 함: 재시도(한 줄로 입력) 후 정상 실행되어 확인하지 못함.
- 교훈: 붙여넣기 시 `\` 줄 연속은 공백 없이 확인, 또는 한 줄 명령으로 실행.

### 체인 3: WordPress 500 — DB 접속 거부 (핵심, 재발의 진짜 원인)

Docker Desktop 시절 08:28에 **이미 초기화된** 데이터 디렉터리 `/home/yutae/work/docker`를
재마운트했는데, MySQL은 **`/var/lib/mysql`에 이미 데이터가 있으면 `MYSQL_ROOT_PASSWORD`를 무시**한다.
초기화 시점에 root 비밀번호가 고착되어, 그 뒤 컨테이너에 `MYSQL_ROOT_PASSWORD`로 **새 값을 줘도
그 값이 무시**되고, `WORDPRESS_DB_PASSWORD`가 그 고착 값과 맞지 않으면
`Access denied for user 'root'@'172.18.0.x' (using password: YES)` → HTTP 500.

진단 기법 (값을 화면에 드러뜨리지 않는 실측 순서):

1. `docker exec <wp> sh -c 'printf "%s" "$WORDPRESS_DB_PASSWORD" | wc -c'` — env 값 **길이**만 확인
   (실측: WP와 DB 양쪽 모두 길이 **3**. 즉 초기화 당시의 3자 값이 그대로 사용됨)
2. WP 컨테이너에서 `wp-config.php`의 실제 `DB_USER`/`DB_HOST`/`DB_PASSWORD`와 env 대조 —
   `wp-config.php`는 이미지 입장에서 **PHP 실행 시점에** env를 읽으므로, run 시점 env와
   컨테이너 재시작 사이에 값이 바뀌면 고착값이 남는다.
3. 호스트·컨테이너 어느 쪽에서든 `php -r 'new mysqli("mysql","root","<값>","wordpress")'`로
   연결 성공/실패를 분리 확인 — 비밀번호 자체 문제는 여기서 판정.

결론: 실패의 본질은 **밀어 넣은 새 비밀번호 ≠ 초기화 시점에 고착된 비밀번호**이며,
**"데이터 디렉터리가 비어 있지 않으면 초기화 비밀번호는 절대 바뀐다"**는 MySQL 동작이 함정이다.

### 재발 방지 3원칙

1. **초기화 비밀번호를 바꾸려면 데이터 디렉터리를 빈 것으로 만들어야 한다.**
   (MySQL은 `/var/lib/mysql`이 비어 있어야 `MYSQL_ROOT_PASSWORD`로 다시 초기화.)
   기존 파일이 있으면 `--initialize`가 아예 거부(=실패 4)되거나, 기존 비밀번호가 승자.
2. **`WORDPRESS_DB_PASSWORD`는 밑줄 한 개**. 밑줄 두 개(`WORDPRESS_DB__PASSWORD`)를 주면
   무시되고 `wp-config.php`가 `example username`/`example password`로 고착 → 1045 (실패 5 재발).
3. **양쪽 env를 같은 값으로 통일**. `MYSQL_ROOT_PASSWORD`(DB 측)와
   `WORDPRESS_DB_PASSWORD`(WP 측)가 달라야 1045. 같은 값 + 빈 디렉터리 = 안정.

### 최종 성공 루트 (실측, 2026-11-08 19:53)

데이터 디렉터리 `~/work/docker`(103MB, 이미 고착된 비밀번호)를 자동 검증이 `rm -rf`를
차단한 덕분에 **`docker.bak-20261108-195350`으로 rename**하고, 빈 `/home/yutae/work/docker`
를 새로 만든 뒤, `MYSQL_ROOT_PASSWORD`와 `WORDPRESS_DB_PASSWORD`를 **같은 3자 값**으로
통일한 두 컨테이너를 재생성.

- `docker exec wordpressdb_hostvolume sh -c 'printf "%s" "$MYSQL_ROOT_PASSWORD" | wc -c'` → **3**
- `docker exec wordpress_hostvolume sh -c 'printf "%s" "$WORDPRESS_DB_PASSWORD" | wc -c'` → **3**
- WP 컨테이너에서 `mysqli_select_db(<host>=wordpressdb_hostvolume, "wordpress")` → 연결 **OK**,
  `wordpress` 테이블 수 = 0 (초기화 상태, 정상)
- `docker port wordpress_hostvolume` → `80/tcp -> 0.0.0.0:8080` (고정 포트 8080으로 변경)
- `http://localhost:8080/` → `HTTP 302 → /wp-admin/install.php`, install.php HTTP 200
  (제목 `WordPress › Installation`) — **DB 연결 정상, 설치 페이지 도달**

### 남은 조치 (사용자)

- **DB root 비밀번호가 3자 짧은 값으로 고정되어 있다.** WordPress 설치 전이라면 이 상태가
  가장 안전할 때다. WordPress 설치 전에 **더 강력한 비밀번호로 통일 재초기화**를 권장
  (방법은 체인3 재발 방지 3원칙 1, 2, 3).
- `docker.bak-20261108-195350`(103MB)는 고착된 3자 비밀번호 DB로 **복원 가치가 낮음**.
  `sudo rm -rf /home/yutae/work/docker.bak-20261108-195350`으로 정리 권장.

### 교훈 (부록2 종합)

- Docker Desktop → 네이티브 전환은 File Sharing/심볼릭링크/VM 구조 3개 함정을 동시에 제거하지만,
  **`~/.docker/config.json`의 `credsStore`/`plugins`/`features` 잔여는 CLI 인증 단계에서
  pull을 여전히 막음** — 전환 직후 반드시 정리.
- `--link name:host`는 **호스트네임 해석**만 도와줄 뿐 실제 TCP는 bridge IP(172.18.0.x)
  경유. 실패 체인에서 "비밀번호가 서로 다르다"고 착각하기 쉬운데, 3자료를 나눠 확인해야
  원인 분리가 됨: (1) `env` 값 길이, (2) `php -r` mysqli 직접 실행, (3) `wp-config.php`
  고착값과 run 시점 env 대조.
- 데이터 디렉터리가 이미 고착된 비밀번호라면 `docker run -e`로 새 값을 줘도 **무시됨**.
  "비어 있어야 초기화"는 MySQL의 동작이므로, 비밀번호를 바꾸려면 반드시 **빈 디렉터리** + 재실행.
- `WORDPRESS_DB_PASSWORD`는 **밑줄 한 개** 정사. 둘은 `wp-config.php` 기본값으로
  고착 → `example username`/`example password` 오타 재발.

