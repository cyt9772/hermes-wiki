---
source_url: /run/media/yutae/UBUNTU 26_0/리눅스프로그래밍_필수유틸리티.pdf
title: 리눅스 프로그래밍 필수 유틸리티
author: 백창우
publisher: 한빛미디어
year: 2010
isbn: 978-89-7914-759-9
extract: pdftotext (poppler, 2026-10-17)
text_layer: true
---

> Text-layer full-text wrapper. Original PDF: 리눅스프로그래밍_필수유틸리티.pdf (sha256 388ba6f70b2230e8160e9fbc6d2d2122cbc67deb0c314ac6cdeb9dc88cdfe82d). Page markers: `===== PAGE N =====` = PDF page N.

===== PAGE 1 =====
www.hanb.co.kr

유닉스 리눅스
프로그래밍
r
그
/사以

필수유틸리티 개정판
vim, make, gcc, gdb, svn, binutils
개발 생산성을 높이는 유틸리티 사용법
vim, make, gcc, gdb, svn 등의 유틸리티로
프로그래밍 생산성을 높이는 방법을 보여준다
백창우 지음

句.

U>
II*

히빈미디01
Hanblt Media, Inc.

===== PAGE 2 =====
유닉스 리눅스
프로그래밍
필수 유틸리티 ［ 개정판］
vim, make, gcc, gdb, svn, binutils

백창우 지음

===== PAGE 3 =====
백창우 bckddn@hanmail.net
삼성전자, 삼성SDS, （주）누스코에서 여러 종류의 RTOS를 주도적으로 개발하였다. 해당 RTOS들
은 각종 삼성전자 제품 및 많은 제품군에 탑재되어 전세계에 수출되고 있다. 삼성종합기술원에
서 컴파일러를 개발하였다. （주）누스코에서 디버거와 Hypervisor 및 각종 시스템 S/W를 개발하
였다. 오프라인 시스템 S/W 스터디 그룹 http://www.iamroot.org를 9년째 운영 중이다. 현재는
（주）누스코의 대표이사로 근무하고 있다.

유닉스 리눅스 프로그래밍 필수 유틸리티

EB

지은이I백창우
펴낸이।김태헌
펴낸곳 । 한빛미디어（주）
주 소 I 서울시 마포구 서교동 480-26 한빛빌딩 2층 IT출판부
전 화 I IT전문서팀 02） 325-0984, 영업 1팀 02） 336-7114
팩 스 | 02） 336—7124
등 록 I 1999년 6월 24일 제 10-1779호
초판 발행 | 2이0년 9월 6일
3쇄 발행 | 2012년 11월 12일

정 가134,000원
ISBN | 978-89-7914-759-9 93560

기 획I한동훈
편 집I한동훈
Published by HANBIT Media, Inc. Printed in Korea
Copyright ©2010 by 백창우 & HANBIT Media, Inc.

이 책의 저작권은 백창우와 한빛미디어（주）에 있습니다.
저작권법에 의해 보호를 받는 저작물이므로 무단 복제 및 무단 전재률 금합니다.
이 책에 대한 의견을 주시거나 오탈자 및 잘못된 내용의 수정 정보는 한빛미디어（주）의 홈페이지나 아래 이메일로
연락주십시오. 잘못된 책은 구입하신 서점을 통해 교환해 드립니다.
http://www.hanb.co.krask@hanb.co.kr

===== PAGE 4 =====
I 저자 서문 I

개정판이 나오기까지

해묵은 원고를 지금에서야 출판한다. 2007년 9월부터 쓰기 시작했으니 햇수로 총 3년
이 걸린 것이다. 쓰는 데 2년, 출판사 일정으로 1년이 더 걸렸다.
쓰는 데 이렇게 오랜 시간이 걸린 것은 필자의 사정 때문이다. 초판과 개정판 사이 필
자는 생애 처음으로 회사란 곳에 들어가 봤고, 회사를 설립도 해 봤다. 본 서적을 쓰는
동안 필자의 삶은 참으로 굵직굵직하게 흘러갔었다.
원고를 쓰는 내내 저작 활동은 필자의 즐거운 주말을 방해하는 훼방꾼이었다. 매주 필
자는 항상 무거운 마음으로 주말을 보냈었다. 그래서 이렇게 마지막 서평을 쓰는 지금
기분이 무척 홀가분하다.
다만, 아쉬운 점은 저작 기간이 너무 오래 걸렸다는 점이다. 현재 페도라 13이 나와 있
는 시점에 이 책은 페도라 7로 설명하고 있고, gcc-4.5.1 이 나와 있는 시점에 2007년도
에 작성하여 gcc-4.1.2를 설명하고 있다. 그렇지만 내용에는 큰 변화가 없기에 독자는
걱정하지는 않아도 된다. 다만, 필자가 독자에게 좀 더 잘해 주지 못한 것 같아 이 점이
무척 아쉬울 뿐이다.

2004년도에 이 책의 초판을 쓰고 서평을 적을 때 개인적으로 초판에 대해 평가한 점수
는 60점이었다. 그래서 많이 부끄러웠다. 이번 개정판은 70점이다. 독자에게 100점짜리
를 대접하지 못해 송구스럽다.
언젠가 100점짜리를 써서 드리고 싶긴 하지만, 실제로 그럴지는 모르겠다. 책을 쓸 때
필자는 항상 “내가 다시 책을 쓰면 사람이 아니다”라고 다짐하곤 한다. 저작 활동은 그
만큼 고되고 고독한 작업이기 때문이다. 그래서 지금은 영원히 다시 쓰고 싶지가 않다.
하지만 모든 산고가 그렇듯 출산의 순간은 고통스럽지만, 시간이 지나면 빨리 잊히는
것도 산고이 기에 다짐이 지켜질지, 다시 100점짜리에 도전할지는 “잘 모르겠다”고 하는
것이 맞을 것 같다.

서문 3

===== PAGE 5 =====
어쨌든 이 책을 쓰는 내내 독자에게 조금이라도 도움이 될 수 있기를 바랐다. 서평을
쓰는 마지막 이 순간까지도 그러고 있다. 부디 필자의 소망이 이루어지기를 간절히 바
란다.
독자 중에 이 책의 내용이 아주 재미있었거나가슴 두근거리게 하는 사람이 있다면 필
자에게 연락이라도 한번 주었으면 하고 바란다. 필자는 비록 작지만 기술적으로는 한국
최고인 System S/W 전문 회사를 경 영하고 있다. 필자는 그러한 사람들과 함께 회사를
키워가고 싶고, 비록 그렇게 인연이 되지 않을지라도 그러한 사람이 존재한다는 것이라
도 알고 지내고 싶다.
그러니 그러한 사람이 있다면 꼭 필자에게 메일이라도 한 통 보내 주길 간곡히 부탁
드린다.
마지막으로 이 책이 나올 수 있게 도와주신 분들에게 감사드리고 싶다. 먼저 나의 영원
한 멘토이자 형님이신 건국대학교 박정근 교수님께 감사드린다. 이 책의 많은 부분은
박정근 교수님의 영향을 받았다. 그리고 박정근 교수님이 없었다면 어쩌면 필자가 이
자리에 존재하지도 못했을 거라는 생각을 가지고 있다. 그분께 “좋아하고, 존경하고, 세
상에 존재해 주셔서 감사하다”는 말을 전하고 싶다.
곧 있으면 더 큰 세계적인 무대로 떠나시는 김홍석 박사님께도 감사드린다. 이 책의 내
용 중 gcc 컴파일러 부분은 그분께 많은 영향을 받았다. 감사와 함께 더 큰 무대에서 그
분께 “항상 행복이 함께하기를 기원한다”는 말을 전하고 싶다.
필자에게 영원한 스승이신 삼성전자 김정한 상무님께도 감사드린다. 이 책의 많은 내용
중 그분에 게서 배운 것들이 많이 있다. 그리고 삶을 살아가는 자세 역시 그분에게서 배
웠기에 그분께 “존경하고, 감사드린다”는 말을 꼭 전하고 싶다.
슈퍼 엔지니어이자 필자의 영원한 친구인 경민이에게 감사드린다. 경민이는 잘 모르겠
지만 알게 모르게 필자에게 많은 영향을 끼쳤다. 경민이에게 “항상 고맙고, 다음 주 소
주 한잔하자”는 말을 전하고 싶다.

KIST 김수현 박사님께도 감사드린다. 비록 뒤늦게 뵙게 되어 이 책에 직접적인 영향을
주지는 않았지만, 항상 도움만 받고 있기에 이 자리를 빌어 “더 잘해드리지 못해 미안
하고, 감사드린다”는 말을 꼭 전하고 싶다.

4

서문

===== PAGE 6 =====
필자의 회사 동료들에게도 감사드린다. 평생의 친구이자 동반자이고, 필자에게 “삶의
이유”라는 사실을 꼭 전하고 싶다.
마지막으로 사랑하는 가족에게 감사드린다. 먼저 필자를 있게 하였고, 삶으로써 필자에
게 항상 감동과 지혜를 가르쳐 주시는 부모님께 “영원히 사랑하고, 존경하고, 감사드린
다”는 말을 전하고 싶다. 그리고 항상 필자에게 응원을 아끼지 않는 동생 승권이에게도
“사랑하고, 고맙다”는 말을 함께 전하고 싶다.
그리고 이 책을 읽어 주신 모든 독자분들께 감사드린다.
미천한 필자의 능력이 부디 0.001%라도 세상에 도움이 될 수 있기를 간절히 기원한다.

2010년 8월 4일 불면의 밤에
백창우

서문 5

===== PAGE 7 =====
I 목차 I

저자 서문

3

11부I 튜토리얼

_

___________

©튜토리얼
01. 간단한 소스 프로그램 작성

19

02. gcc 컴파일러로 실행 파일 생성

21

03. make를 사용해 컴파일

25

04. 문제 발생, 벌레를 잡아라

'

29

05. svn을 사용한 프로젝트 버전 관리

36

06. doxygen을 이용한 문서화

40

07. autotools를 사용한 이식성 높은 빌드

44

08. RPM 패키징

51

|2부| 에디팅

가와 vim 에 디 터
01.vi 개괄

59

이의 역사

59

이의 장점

59

서른 살이 넘은

에디터,그 매력

02. 기본적인 vim 사용법트레이닝

60

61

vim의 모드 이해

62

파일 열기, 저장, 종료

63

===== PAGE 8 =====
입력

66

이동

67
70

편집

문자열 탐색

74
74

문자열 치환

75

되돌리기와 되살리기

03. vim을 강력하게 하는 고급 테크닉

78

정규 표현식을 사용한 문자열 탐색과 치환
여러 파일을 편집하는 방법

78
88

반복되는 문자열을 저장해서 쓰기

92

매크로의 사용

94

다중창 사용하기
마킹으로 이동하기

95
99

셸명령사용

102

04. vim의 조력자 ctags, cscope, 기타 플러그인

104

소스 태그를 찾기 위한 만능 해결사 ctags

104

ctags 설정 및 기본 사용법

105

vim 내장 스크립트 작성

110

cscope* 사용해 나머지 2%를 채워라

114

완벽한 조합 vim 十 screen + ctags + cscope

119

모르는 함수를 알고 싶을 때 man page의 활용

122

플러그인을 사용해 vim의 기능 확장

124

05. 개발자를 위한 vim의 유용한 팁

130

빠른 괄호 이동 및 빠른 탐색

130
130

폴딩기능이용

131

함수의 원형과 지역변수의 선언 부분으로 바로 이동
여러 행 탭 끼워 넣기

132
133

탭사이즈조정

133

흐트러진소스정렬
행번호보여주기

134
135

”M 문자제거

136

파일에서 달라진 부분 비교하기
헤더 파일 바로 읽어오기

137
138

자동 완성기능 사용하기

139

정규 표현식에서의 매칭 문자 사용

139

파일 탐색 기능 활용

06. 개발자들의 vim 설정

139

===== PAGE 9 =====
0

기타 편집기 소개

01. emacs

145

02. 이클립스

147

이클립스소개

147

이클립스의 특징

148

이클립스의장단점

148

03. gedit

149

04. KDevelop

150

05. anjuta

151

13부I 컴파일과 링킹

gcc compiler
01.컴파일의의미

155

인스트럭션과어셈블리

155

0과1밖에모르는 CPU

159

02. 알아 두면 정말 유용한 C 소스 컴파일 과정

163

C 소스의전체컴파일 과정

163

cc1-E 에의한전처리과정

171

cc1 에 의한 어셈블리 소스 파일로 컴파일

177

as에 의한 기계어 코드 생성

202

collect》에 의한 링킹 과정

208

03. gcc를 사용해 원하는 컴파일하기

218

gcc 옵션 분류

218

gcc 옵션 적용 규칙

226

가장 단순한 컴파일 명령

229
230

반드시 알아야 할 gcc 필수 옵션 및 중요 옵션

04. gcc를 이용한 최적화 컴파일

260

프로파일 결과를 이용한 최적화

260
265

함수 프레임 포인터 제거

276

머신 종속적인 옵션을 이용한 최적화

===== PAGE 10 =====
프리패치 (prefetch)를 이용한 최적화

279

레지스터 활용을 통한 최적화

gcc 컴파일 속도 최적화

281
281

05. 기타 알아 두면 좋을 만한 것

282

환경 변수를 사용한 gcc 설정
specs 파일을 이용한 gcc 설정

282
283

Id linker
01. 링킹의기본 이해

289

링킹 과정 절차

289

02. ELF 바이너리 포맷 구조

295

ELF 바이너리포맷이란?

295

ELF 바이너리 포맷의 구조

296

ELF 바이너리를 해석하는 두 가지 관점

298

ELF 헤더

299

프로그램 헤더 테이블
각종 섹션의 종류

301
304
307

03. Id를 사용한 링킹

315

섹션 헤더 테이블

Id를사용한 기본적인링킹

315

알아 두면 유용한 Id 옵션

325

04. 링커 스크립트

335

링커 스크립트의 이해

335

링커 스크립트 기본 문법

342

05. Id를 사용한 고급 링킹 테크닉

357

OS 개발을 위한 링커 스크립트

357

XIP 기법을 사용한 메모리 절약

358

오버레이 (overlay)

361
363

필요한 데이터 바이너리 이미지에 포함

06. 라이브러리를 만들기

365

정적 라이브러리 만들기

365

공유 라이브러리 만들기

369

===== PAGE 11 =====
gas assembler
01. gas를 사용해 어셈블하기

377

gas의 이 SH

378

as를 사용한 어셈블 실습

381

02. 어셈블리 파일의 작성

388

assembly 기본 사용법

389

C 소스에서 컴파일된 어셈블리 파일 분석

391

전처리기 사용

gas assembler 필수 지시자

396
397

03. 인라인 어셈블리의 사용

403

@ 삶을윤택하게 하는 바이너리 유틸리티
01. 바이너리 유틸리티 사용하기

415

addr2line 명령으로 특정 주소가 어떤 파일의 어떤 라인인지 알아보기 416
c++filt 명령으로 맹글링되기 전의 C + + 또는 JAVA 심볼명 보기 416
gpmf로 프로파일 정보 알아보기

418

nm으로 ELF 포맷의 심볼 테이블 보기

420

objcopy 사■용하!'기

422

objdump 사용하기

423

readelf 명령으로 ELF 파일의 각종 정보 보기

426

size 명령으로 오브젝트 파일의 사이즈 보기

427

strings 명령으로 바이너리 내부 문자열 보기
오브젝트 파일의 사이즈 줄이기

427
427

gcov로 커버리지 정보 알아보기

428

|4부| 디버깅___________________________________________________

혀 gdb 디버거
01. 단순하지만 매우 강력한 디버거 gdb

435

gdb에 대한 소개

435

gdb로 간단한 디버깅 따라 하기

436

gdb의 시작과 종료

438

소스 보기

440

===== PAGE 12 =====
브레이크포인트

441

프로그램 실행
변수와 레지스터 값 검사

446
449
451

스택의 상태 검사

462

와치 포인트 설정

메모리 상태 검사

473

기타 유용한 명령

475

02. gdb를 이용한 디버깅 테크닉

479

코어 파일을 이용한 디버깅
실행 중인 프로세스 디버깅

479
482

멀티프로세스 프로그램 디버깅

484

멀티스레드프로그램디버깅

488

라이브러리 디버깅

493

GUI 디버거 DDD의 사용
01.DDD 란무엇인가?

501

02. DDD를 人요한 디버깅

501

ddd 시작과 종료

502

ddd의 각부분설명

502

ddd에서 브레이크포인트 설정

503

ddd에서 브레이크포인트 해제

506

프로그램에 걸려 있는 브레이크포인트 확인

507

프로그램 수행

507
509

와치 포인터 설정

레지스터, 메모리, 스레드, 스택 등의 상태 확인

510
513

프로세스 attach와 detach

513

기타알아 두면좋을사항

514

변수값검사

기타 디버깅 툴
01. trace 유틸리티를 사용한 프루그램문제점 분석

517

strace를 사용해 프로세스의 문제 진단

517

Itrace를 사용해 프로세스가 호출하는 공유 라이브러리 함수 알아보기

523

02. 문제 진단 유틸리티

524

splint로 소스 코드의 문제점 진단

524

메모리 디버거의 사용

526

===== PAGE 13 =====
15부 I 프로젝트 빌드

make
01. make의 이해
make의 기본 동작

533

기술 파일의 작성

534
538

02. 매크로의 사용

542

매크로 작성 기본 규칙
매크로 사용 시 주의 사항
내부적으로 정의되어 있는 매크로의 사용

542
545
547

03. 확장자 규칙의 사용

551

04. 더미 타겟의 人용

558

05. 명령 사용 규칙

558

06. 재귀적 make°| 사용

562

서브 Makefileoil 대한 매크로 전달

567

07. 조건부 수행

569

08. 함수의 사용

570

셸 명령 함수

571

문자열 처리 함수

572
577

파일 이름 관련 함수
기타 유용한 함수

579

함수 사용할 때 주의 사항

582

09. 특수 타겟

584

10. make 최종 정리

585

autoconf
01. autoconf 란 무엇인가

592

02. 따라 해 보기

593

03. autoconf의 구조와 원리

597

===== PAGE 14 =====
04. configure.ac 파일 작성 규칙

601

05. 사용 가능한 매크로

603

프로그램 결정 매크로

603

라이브러리체크 매크로

610

헤더파일체크 매크로

613

06. 함수 체크 매크로

616

파일 체크 매크로

619
620

기타 유용한 매크로

620

구조체 및 타입 체크 매크로

07. 세밀한 제어를 위한 configure.ac 작성

623

08. 설정 헤더를 사용해 소스 파일에 설정 적용

627

automake
01. automake의 구조와 원리

635

02. 따라 해 보기

636

03. Makefile.am 파일 작성 규칙

639

04. 재귀적 Makefile.am 파일 작성

644

| 6부| 프로젝트 버전 관리

Subversion, CVS
01.버전관리의이해

653

버전 관리 정의

653

프로젝트 파일 버전 관리의 필요성

654

02. Subversion을 이용한 버전 관리

656

Subversion 소개

657

03. Subversion 서버 설정

659

저장소 생성 및 초기화

659

===== PAGE 15 =====
ssh를 이용한 서버 설정

660
661

http를 이용한 서버설정

664

svnserve를 이용한 서버 설정

668

저장소 접근 방식 종류 이해

04. Subversion을 사용해 프로젝트 진행
에디트 환경 변수 설정
프로젝트 디렉토리 정리

671
671
671

import 명령으로 프로젝트 서버에 등록

674

checkout 명령으로 프로젝트 파일 가져오기
commit 명령으로 변경된 내용 저장소에 반영

676
677

update 명령으로 저장소의 최신 내용 작업 디렉토리에 반영

679

log 명령으로 리비전별 로그 확인

681

diff 명령으로 변경된 내용 비교

682

blame 명령으로 라인 단위의 작성자 확인

684

status 명령으로 작업 디렉토리 상태 확인

685

add 명령으로 파일이나 디렉토리를 버전 관리 대상에 추가

686

delete 명령으로 파일이나 디렉토리를 버전 관리 대상에서 제거

686

rename 명령으로 파일명이나 디렉토리명 변경

687

lock/unlock 명령으로 파일 잠금 및 해제

687

revert 명령으로 파일 이전 상태로 되돌리기

688

export 명령으로 버전 정보 제외한 프로젝트 파일만 가져오기

689

copy 명령으로 브랜치하기

690

merge 명령으로 머지하기

692

copy 명령으로 태깅하기

694

cleanup 명령으로 작업 사본 정리하기

695

dump/load 명령으로 백업 및 복구하기

695

충돌에 관한 해결법

696
701

기타 간단한 팁

05. CVS를 이용한 버전 관리

704

CVS 소개

705

06. CVS 서버 설정

706

저장소 디렉토리 생성 및 초기화

706

cvs 사용자 생성 및 권한 설정

707

CVS 사용자 등록

707

CVS 서버실행

709

07. CVS를 사용해 프로젝트 진행

710

CVS 서버에로그인

711

import 명령으로 CVS 서버에 프로젝트 파일 등록

714

===== PAGE 16 =====
checkout 명령으로 프로젝트 파일 받아오기
commit 명령으로 수정한 내용을 저장소 디렉토리에 반영

716
717

update 명령을 사용해 현재 작업 디렉토리에 최신 소스 반영

719

소스 충돌 해결

720
721
726

add와 remove를 이용한 파일과 디렉토리 추가 및 삭제
파일 이전 버전으로 돌리기
파일 버전대별 차이점 확인

728
729

현재 시점의 소스 태깅하기

731

브랜치하기

732
733

파일 로그 및 특정 부분을 수정한 사람 확인하기

브랜치한 소스 머지하기

해 프로그래밍 유형별 가용 유틸리티
01. GUI 프로그래밍

737

QT 디자이너를 사용한 간단한 GUI 애플리케이션 만들기

738

glade를 사용해 간단한 GUI 애플리케이션 만들기

746

02.네트워크 프로그래밍

효 vim 명령 정리
부록 C

735

755

759

gcc 옵션 정 리

767

autoconf 매크로 정 리

771

찾아보기

781

===== PAGE 17 =====
11 부 I 튜토리 얼

===== PAGE 18 =====
1
튜토리얼

01 간단한 소스 프로그램 작성
02 gcc 컴파일러로 실행 파일 생성
03 make를 사용해 컴파일
04 문제 발생, 벌레를 잡아라
05 svn을 사용한 프로젝트 버전 관리
06 doxygen을이용한 문서화
07 autotools를 사용한 이식성 높은 빌드
08 RPM 패키징

===== PAGE 19 =====
L-c+S S-tudy
시작하기 전에 먼저 필자의 테스팅 환경을 설명하고자 한다. 필자가 예제들을 테스팅한
환경은 페도라 (Fedora) 7 과 우분투 (Ubuntu) 7.04 배포판 환경이다. 반드시 필자와 환경
을 맞줄 필요는 없다. 하지만 리눅스/유닉스에 익숙하지 않은 독자라면 필자의 환경과
맞출 것을 권하고 싶다. 이 책에서 설명하는 몇몇 툴들은 버전의 영향을 제법 타기 때문
이다.
그리고 리눅스를 설치한다면 전체 설치를 권장한다. 표준 설치를 하면 개발에 필요한 여
러 요소가 누락된다. 때문에 예제를 따라 하다 필요한 툴이 없어 툴을 설치하는 데 시간
을 낭비할 수 있다. 되도록이면 목적에 집중하길 바란다.

1 장은 이 책의 시작임과 동시에 책의 내용을 전반적으로 보여주는 장이다. 그냥 한번 따
라 해 보길 바란다.

===== PAGE 20 =====
01 L 간단한 소스 프로그램 작성
리눅스(유닉스를 포함해)에서 개발하는 일은 무척 즐거운 일이다. 하지만 그런 즐거움
은 리눅스 철학과 개발 환경을 잘 이해하고 있을 때 비로소 얻을 수 있다. 그렇지 않다
면 단지 시련의 연속일 뿐이다.
리눅스에서 개발을 잘하고 싶은가? 그렇다면 이해하려고 노력하기 바란다. 필자의 주
위를 둘러보면 윈도우 환경에서만 개발하다 어떤 이유로 리눅스 개발 환경에 발을 들
인 사람들이 있다. 비교적 적응을 잘하는 사람이 있는가 하면, 계속 윈도우와 비교하며
툴툴거리다 결국 모든 것을 부정하고 윈도우 환경으로 되돌아가는 사람도 있다.
안타까운 일이다. 운영체제가 무슨 잘못이 있겠는가? 적어도 유닉스는 윈도우보다 30년
전에 세상을 지배했었고, 오늘날에도 리눅스와 함께 건재함을 과시하고 있다. 이런 역
사적 사실은 외면하고 윈도우만 겨우 배워 윈도우만 옳다고 이야기하는 것은 무지의
소치라고밖에 볼 수 없다. 필자는 이 책을 읽는 사람들이 리눅스 개발 환경을 잘 이해
해서 필자가 느끼는 리눅스 개발 환경의 즐거움을 함께 공유하기를 바란다.
이 책은 개발 방법론 책도 아니고, 그렇다고 소프트웨어 엔지니어링 책도 아니다. 이 책
은 리눅스/유닉스 개발 환경에서 어떤 유틸리티를 어떻게 활용하면 좀 더 효율적인 개
발 환경을 조성할 수 있는지 알려주는 데 목적이 있다. 때문에 프로젝트의 각 단계에서
개발자가 사용할 수 있는 유틸리티를 주제로 해 필요성과 원리, 사용법에 대해 많은 것
을 알아볼 것이다.
이제 앞으로 프로젝트에서 사용할 간단한 소스 프로그램을 작성해 보자. 그런데 전통
적인 hello world 프로젝트는 이제 너무 식상한(?) 느낌이다. 그래서 like 프로그램을
작성하고 프로젝트명을 likeU 프로젝트라 지칭하기로 하자. 먼저 소스 프로그램을 작
성하려면 편집기의 사용이 필수적이다. 리눅스/유닉스에는 여러 종류의 편집기가 있지
만, 이 절에서는 너무도 유명한 vim을 사용해 like.c 소스 프로그램을 작성한다.
$ vim like.c

$ 기호는 셸 프롬프트를 의미하고, $ 기호 이후부터가 입력할 명령이다. 셸에서 위와 같
이 명령을 내리면 ［그림 1-1］ 과 같은 vim 화면이 뜰 것이다.

1장-튜토리얼 19

===== PAGE 21 =====
[그림 1-1] vi like.c 실행 화면

우분투 사용자라면 우분투가 최초 설치된 환경에서는 vim이 제대로 설치되지 않고 vim-tiny가 설치되
어 있을 것이다. vim-tiny를 사용해도 무방하지만 어차피 2부 “에디팅” 과정에 가면 vim을 설치해야
되기 때문에 다음 명령으로 vim-tiny를 지우고 vim을 설치하기 바란다.

sudo apt-get remove vim-tiny
sudo apt-get install vim

i 키를 누르고 다음과 같이 소스 프로그램을 작성한다.
〔예제 1-1〕 like.c 소스 파일 내용

#include <stdio.h>
int main()
{
printf("I like you.\n");
return 0;
}

[그림 1-2] like.c 소스 작성 화면

20 1 부—튜토리얼

===== PAGE 22 =====
Esc] 키를 누르고 :wq!를 차례로 입력하면 like.c 파일이 저장된다. 저장된 파일은 셸
프롬프트에서 cat like.c 명령으로 확인할 수 있다.

【그림 1-3] like.c 저장 화면

페도라 7이나 우분투 7.04 feisty의 경우 기본 인코딩(encoding)이 UTF-8이므로 필자와 같이 네트
워크로 접속해 작업을 할 경우 UTF-8을 지원하지 않는 터미널을 사용하면 한글이 제대로 출력되지 않
을 수 있다. 그럴 때는 셸에서 다음 명령을 입력해 ?』코딩을 EUC-KR로 바꿔 보기 바란다. 보통 윈도우
터미널이(JTF-8을 지원하지 않는 경우는 있지만, EUC-KR은 대부분 지원하므로 인코딩을 EUC-KR
로 바꾸면 제대로 한글이 출력될 것이다.
,-

$ export LANG=ko_KR.EUC-KR

2 | gCC 컴파일러로 실행 파일생성 <
이제 작성된 소스 파일을 컴파일할 차례다. GNU에서 만든 gcc 컴파일러를 사용해 소
스를 컴파일해 보자.
$ gcc —W -Wa丄1 -02 -o like like.c

우분투 사용자는 관련 헤더 파일이 시스템에 없어 정상적으로 컴파일되지 않을 것이다. 우분투 사용자
는 다음 명령으로 컴파일 관련 헤더 파일과 라이브러리를 설치한 후 컴파일 명령을 내리기 바란다.

sudo apt-get install build-essential

1 장_ 튜토리얼 21

===== PAGE 23 =====
앞의 명 령에서 사용된 옵션은 다음과 같다.
才예...，.. 丄

• （스7ag옵션은 모든 경고 메시지를 출력하는 옵션이고, -W는 -Wall에서 제외된

1유지 종류의 경고 메시지까지 출력하라는 의미다. 결국 -W -Wall 옵션은 모든
경고 메시지를 출력하라는 의미이고, gcc는 like.c 소스에서 아주 사소한 문제라
도 발견하면 경고 메시지를 출력한다.

• -02 옵션은 최적화에 관계된 옵션으로, like.c를 컴파일하는 과정에서 최적화 과
정을 수행해 속도를 향상시키고 사이즈를 줄일 때 사용하는 옵션이다.

• -o 옵션은 output의 의미로, like.c를 컴파일해 결과로 나오는 실행 파일명이 like
가 되게 지정하는 옵션이다.

gcc에 관계된 옵션, 원리, 구조 등의 좀 더 자세한 내용은 3부 “컴파일과 링킹” 과정에
서 설명한다.
서 B ro（jt@os：/temp/test/temp
[root（흐os temp]tt gcc -W -Wall -02 -o like like.c
[root（흐os temp]tt |

［그림 1-4］ like.c 컴파일 화면

［그림 1-4］ 와 같이 아무런 출력 메시지 없이 끝났다면 정상적으로 컴파일된 것이다.

./like 명령으로 실행시키면 “I like you.”라는 메시지가 기분 좋게 출력되는 것을 확인
할수있다.
B roQt@os：/temp/test/temp
|[root@os temp]tt gcc -W -Wall -02 -o like like.c
[rootdos temp]tt
[root@os temp]tt Is
like like.c
[rootdos temp]tt
|[root@os tegpltt -/like
pITke ^ou ]
[rootOos temp]# |

［그림 1-5］ ./like 실행 화면

이제 모두에게 보여주기 좋은 like 프로그램이 만들어졌다. 그런데 여기에 연인에게 보
여주는 기능이 필요해졌다. 이를 위해 like.c 소스를 다음과 같이 수정하고 love.c 소스
를 새로 주가하자.

22

1부—튜토리얼

===== PAGE 24 =====
〔예제 1-2〕 like.c 소스 파일 내용

#include <stdio.h>
void lovecall();
int main()
{
printf ("I like you.\n");
lovecall();
return 0;

〔예제 1-3］

love.c 소스 파일 내용

#include <stdio.h>
void lovecall()
{

：

printf("I love you.\n");

}

|

위 두 소스의 작성법은 그전과 동일하다. i 키를 누른 후 소스를 타이핑하고 % 키를
누른 다음 :wq!를 입력해 저장하면 된다.
$ gcc -W -Wall -02 -o like like.c love.c

위 명령으로 컴파일하고 ./like 명령으로 실행시키면 ［그림 1-6］ 과 같이 실행됨을 확인
할수있다.
Q) root@os：/temp/test/temp

三

[root(흐os temp]tt Is
like like.c loue.c
[rootQos temp]#
[rootSos temp]tt gcc -W -Wall -02 -o like like.c loue.c
[root(흐os temp]#
[root@os temp]# ./like
I like you.
I loue you.
[rootQos temp]tt |

［그림 1-6］ ./like 실행 화면

이제 연인에게도 보여주기 좋은(?) 아주 훌륭한 프로그램이 만들어졌다. 그리고 이제는
좀 더 고차원적인 의미를 소스에 추가해 보자'.

23

===== PAGE 25 =====
like.c 소스 파일 내용

〔예제 1-4)

#include <stdio.h>
void lovecall();
int

main()

{
printf
("I
lovecall ();

like

you.\n");

return 0;
}

〔예제 1-5] 누 love.c 소스 파일 내용

#include <stdio.h>
#include <unistd.h>
#include <math.h>
void lovecall()
{
double love;
for

(love=0;
sin(love)+2;
printf("I love you.\n");
sleep (1) ;

love++)

{

}
}

love 변수는 계속 증가하는데, sin(love) 는 love 의 사인 값을 반환한다. sin() 함수는
-1 과 1 사이의 값을 리턴하는데, +2가 되었음으로 위 루프는 무한히 반복되면서 love
변수의 값이 증가한다. 그러므로 C 소스를 읽을 수 있는 사람이라면 소스의 숨은 의미
인 무한히 더욱더 “I love you.”한다는 것을 알 수 있다.
위 소스는 다음과 같은 명령으로 컴파일해야 한다. sin() 함수는 링커인 Id가 C 소스를
위해 기본적으로 링크하는 libc.a 라이브러리 안에.들어있지 않고 libm.a 라이브러리
안에 들어있다. 그렇기 때문에 링크 옵션 -1 呈 Ubm.a 라이브러리를 포함시킨다는 점을
명시해야만 컴파일이 가능하다. 그렇지 않으면'；'s’in() 함수가 정의되지 않았다는 오류
메시지가 출력될 것이다.
$ gcc -W -Wall -02 -o like like.c love.c -Im

24 1 부_튜토리얼

===== PAGE 26 =====
3
[그림 1-7] ./like 실행 화면

위 프로그램의 실행을 멈추려면 %+c 키를 누르면 된다. 이제 소스 자체에도 의미가
들어있는 아주 훌륭한(?) 프로그램이 만들어졌다. 그런데 과연 이 소스를 누군가에게
보내 준다면 위와 같은 복잡한 명령으로 컴파일할 수 있을까? 물론 리눅스/유닉스를
잘 아는 C 프로그래머라면 쉽게 컴파일할 수 있을 것이다. 그렇지만 다른 대부분의 사
람은 프로그래머가 아니다. 그리고 개발하는 필자 역시 매번 위와 같이 긴 명령으로 컴
파일하기 힘들어지기 시작했다. 이럴 때 컴파일 명령을 각 파일에 맞게 자동화시켜주는
도구가 있다면 좋을 것이다. 바로 프로젝트 파일 관리 유틸리티 즉, make의 사용이 필
요한 시점이다.

3| make를 사용해 컴파일
〔예제 1-6〕 Makefile 내용

CC
CFLAGS
LDFLAGS

= gcc
= -W -Wall
= -Im

-02

$(LDFLAGS)

사이 간격이 TAB임을 주의

1 장— 튜토리얼

25

===== PAGE 27 =====
［그림 1-8］ M가＜ efile의 작성

위와 같이 소스 파일과 같은 디 렉토리 내에 Makefile이 란 이름으로 make 기술 파일을
작성하고 make 명령을 내리면 ［그림 1-9］ 와 같이 수행된다.
巾[)/흐63@0巾________________

B r001@03：/<6

[root@os temp]tt Is
Makefile like.c loue.c
[root@os tenp]tt
[rootBos temp]#[make]
gcc -W -Wall -02 -o like like.c loue.c -Im
[root@os tenp]tt
[root@os temp]# is
Makefile like like.c loue.c
[root@os temp]# |

［그림 1-9］ make 명령 수행 화면

경우에 따라서는 ［그림 1-9］와 같이 출력되지 않고 ”make： 'like’는 이미 갱신되었습니다.’’와 같은 메
시지만 출력될 수도 있다. 이런 상황은 like 파일의 생성 시간이 소스 파일의 최종 수정 시간보다 이후라
서 make가 다시 컴파일할 필요가 없다고 판단해 컴파일 과정을 건너뛴 경우다.
이럴 경우 make clean 명령으로 like 파일을 지운 후 다시 make 명령을 내리면 ［그림 1-9］와 같이 컴
파일되는 화면을 볼 수 있을 것이다.

［그림 1-9］ 와 같은 결과는 /usr/bin/make가 방금 작성한 기술 파일(Makefile)을 읽고
해석해 개발자 대신 컴파일 명령을 내린 것이다. make는 파일 관리 유틸리티로서, 각
파일의 종속 관계를 파악해 명령을 자동화시킬 때 유용한 유틸리티다.
이제 이 소스의 컴파일을 원하는 사람은 컴파일 명 령과 파일 구조를 몰라도 단지 make
명령만 내리면 컴파일할 수 있다. 그리고 개발자 역시 그동안 테스트를 위해 매번 “gcc

-W -Wall -02 -o like like.c love.c -kn” 과 같이 긴 명령으로 컴파일하던 것에서 해
방돼 좀 더 간단한 명령으로 컴파일할 수 있게 되었다.

26 1부—튜토리얼

===== PAGE 28 =====
그 외에 make를 사용함으로써 생기는 이점이 훨씬 많이 있다. 그 부분은 5부 “프로젝
트 빌드”에서 다룬다.
이제 좀 더 새로운 기능을 추가해 보자. 사용자에게서 이름을 입력받아 “I like you.”
메시지 다음으로 입력받은 이름을 출력해 보자.
〔예제 1-7〕, like, c 소스 파일 내용

#include <stdio.h>
void lovecall();
char *getname()
{
char name[128];
printf("Input name : ”);
scanf("%s", name);
r은turn name;
}
int main()
{
char *str;
str = getname();
printf ("I like you.\n");
printf("%s\n", str);
return 0;
}

［예제 1-기과 같이 소스를 수정한 후 make 명령으로 컴파일한다.
'斜 rocitiS’os：/temp/test/te「np
[rootQos €emp]tt make clean
[root(흐os temp]tt make
gcc -W -Wall -02 -o like like.c loue.c -Im
like.c: In function 'getname':
like.c:12: warning: Function returns address of local variable |
[root(흐os temp]* |

［그림 1-10］ make 명령 수행 화면

，:,

1장- 튜토리얼 27

===== PAGE 29 =====
똑똑한 gcc 는 필자의 속도 모르고 친절하게 위 소스에 문제가 있다고 경고 메시지를
출력해 주었다. 소스만 보고도 소스에 문제가 있음을 파악한 독자가 많이 있을 것이다.
그렇지만 지금은 디버깅을 위해 일부러 이런 문제가 있는 소스를 만들었으니 잠시 눈
감아 주길 바란다.
이제 ./like 명령을 수행하면 “Input name : ”이라는 메시지가 출력된다. 그리고 이름을
입력하면 수정된 소스에 의해 “I like you.” 메시지 다음으로 입력한 이름이 출력될 것
이다. 다음은 실제로 실행시킨 결과 화면이다.

[그림 1-11] ./like 실행 화면

&S 지금 출력되는 결과와 앞으로 gdb를 사용하면서 출력되는 결과는 시스템에 따라 다를 수 있다. 그러니
출력 결과가 다르더라도 고민하지 말기 바란다.

앗! 어찌된 일일까? 예상과 달리 “kara”라는 이름을 입력했는데 이상한 글자가 출력되
었다. 문제 원인을 찾는 가장 손쉬운 방법은 printf문을 사용해 실행 중간 중간 변수의
값을 찍어 확인해 보는 방법과, 소스를 다시 한 번 더 잘 확인해 보는 방법 이 있다. 하지
만 여기서는 GNU에서 만든 매우 강력한 디버거인 gdb를 사용해 어떤 부분에서 문제
가 발생했는지 알아보자.

28 1부_ 튜토리얼

===== PAGE 30 =====
4 문제 발생, 벌레를 잡아라
gdb를 사용하려면 먼저 다음과 같은 명령으로 다시 컴파일해야 한다.
$ gcc -W -Wall -02 -g -o like like.c love.c -Im

그동안의 과정에서 사용한 기본적인 컴파일 옵션 외에 -g 옵션이 추가된 것을 확인할
수 있다. -g 옵션은 컴파일 후 생성되는 바이너리에 디버거 섹션을 추가하는 역할을 한
다. 디버거 섹션은 나중에 자세히 설명하겠지만 디버깅을 위한 여러 정보를 담고 있는
섹션이다. 이런 정보에는 전역 심볼 주소, 소스에서 사용된 타입 정보 등이 있고, 컴파
일되는 바이너리에 포함되어 gdb 같은 디버거에게 디버깅을 위한 정보를 제공한다.

-g 옵션을 붙여주지 않으면 디버거 섹션이 추가되지 않아 gdb로 디버깅 시에 바이너
리를 역어셈블해 어셈블리 코드로 디버깅할 수밖에 없다. 그러나 -g 옵션을 추가하면
디버거 섹션에 있는 정보를 이용해 소스 레벨에서 디버깅이 가능하다.
$ gdb like

위와 같은 명령을 실행하면 gdb가 실행되면서 ［그림 1-12］ 와 같은 화면이 출력되고

gdb 프롬프트가 나타난다.
꼬 씌
스
一

|[root@os temp]tt gdb like
GNU gdb Red Hat Linux (6.5-8.Fc6rh)
Icopyright (C) 2006 Free Software Foundation, Inc.
IGDB is Free software, couered by the GNU General Public License,
| and you are
|welcoine to change it and/or distribute copies of it under certai
In conditions.
Ilype "show copying" to see the conditions.
Ilhere is absolutely no warranty For GDB. Type “show warranty" I
lor details.
IThis GDB was configured as ___________ _______________________________________ host
llibthreaddb library "/lib/libthread_db.so.1".

긔

(gdb) |

［그림 1-12］ gdb 실행 화면

gdb 내에서 list라고 명령을 내리면 ［그림 1-13］ 과 같이 main() 함수 부분의 소스가 출
력 된다.

1장_ 튜토리얼 29

===== PAGE 31 =====
[그림 1너3] list 명령 수행 후의 모습

b main 명령 (=break main)으로 main() 함수의 진입점에 브레이크를 건다. 일단 브레
이크를 걸어야만 오류 추적이 가능하다. 브레이크를 걸지 않으면 정지하는 지점 없이
끝까지 수행하기 때문에 원하는 지점에서의 정보를 확인할 수 없다.

[그림 1—14] b main 명령 수행 화면

브레이크를 건 후에는 r(run) 명령으로 프로그램을 실행한다. 그러면 프로그램이 실행
하다가 브레이크가 걸린 부분에서 정지한다.

30 1부—튜토리얼

===== PAGE 32 =====
우리가 확인하려는 변수는 main() 함수의 str 변수와 getnameO 함수의 name 변
수다. display str 명령으로 str 변수의 내용을 화면에 표시하고, s(step) 명령으로

getnameO 함수가 호출될 때 getnameO 함수 내부로 추적해 들어간다.
그리고 getnameO 함수 내에서 display name 명령으로 name 변수의 값을 확인한다.
Brootgos：/temp/tesVtemp____________
(gdb){display str|
2： str = 0x42130a14 " tft»023B 다#001@：갸"
(gdb)
(9이시흐]
getname () at like.c:9
9

printf("Input name : ");
(gdb)「Blspla^ '’'세이
3：
name
=
"W204?
OOOB
c바0O1=O0WOOW00W00WOOW00WO0WO0OWWn

»023BeW003tf000tt080
[W090B?
»080Btf024tfnW023B流jj요7
풼?
오‘?
00«호*1
77W003»000W000W001W000W00Otf000P?
aBWI77tf200tf0OM흐,Xtf6ei@]tt00OW0fl
뷰0008Z바001@좄드? 083? OOO흐? 바881=020fy001Q바001 바0OW00W0OW00W0
00W000W000W022?
00mW222tf203tt004ttb?
016tt023BW02Wntt023BW210?
?
Q
01 바 20WWWb"
(gdb) |

［그림 1-16］ getnameO 함수로 들어간 후 display name 명령을 수행한 화면

［그림 1-16］ 에서 보이는 바와 같이 아직 main() 함수의 str 변수에는 값이 저장되지 않
아 쓰레기 값이 들어있는 것을 확인할 수 있고, getnameO 함수의 name 변수 역시 쓰
레기 값이 들어있는 것을 확인할 수 있다. s 2 명령(=step 2)으로 두 단계 더 진행시켜
보면 “Input name : ” 문자열이 출력되고 사용자 입 력을 기다린다.
IB root@os：/temp/test/temp
(gdb) s 2—
Input name : |

［그림 1-17］ s 2 명령 수행 직후의 모습

이때 원하는 이름(kara)을 입력하고 Enterj 키를 누르면 다음 명령이 수행되면서 화면
에 name 변수의 값을 출력한다.

1장_튜토리얼 31

===== PAGE 33 =====
H root@os ：/temp/test/temp
(gdb) s 2
Input name :|kara [
13

>,

3: name =
0010tt900tf00WO00W0O0W000tf000tf000tf0O8WWntf92j
3Betf003tt000OW7W000B? W000BW82Wntt023B而요? 풼? 오? 9000ttl 77價
WW0OW0OW0OW0OWWWO00P? aB바 177tf2OWOO0@,Xt『OO1(흐]y00W00WO遺
08Z肝001@졿jj? 003? 000@? 바001(그바020F싸001mo01바OOWO9W00W0OMO0O^|
000tf000tt022? 00110tt222W203tt00Wb? 016WO23BW024WnW023BW210? ? 001'
2 03tf 00Wb"
(gdb) |

a

［그림 1-18］ 이름(kara)을 입력한 후의 모습

［그림 1-18］ 에서 보듯이 name 변수에 정확하게 “kara”라는 문자열이 입력되었다. 그
런데도 최종적으로 출력된 결과는 “kara”가 아닌 이상한 문자열이 출력되 었다. 그 문제
를 분석하기 위해 name 변수의 주소 값을 알아보자.

name 변수의 주소 값을 알아보는 명 령은 p(print) &name이다. 그리고 p &name 명
령으로 알아낸 name 변수의 주소에 저장된 값을 알아보는 명령은 x/s “알아낸 주소”
또는 p name 이다.

［그림 1-19］ name 변수의 주소에 들어있는 값을 확인한 모습

필자의 시스템에서 p &name 명령으로 알아본 name 변수 주소는 Oxbfffe6OO번지이
고, Oxbfffe6OO번지에 저장된 값은 “kara”임을 알 수 있다. 단, name 변수의 주소는 테
스트하는 환경에 따라 다를 수 있다. 앞으로 필자가 Oxbfffe6OO번지를 사용한 부분은
각자 시스템에 설정된 name 변수의 주소로 바꿔 이해하기 바란다.
지금까지의 과정은 정상적으로 수행 중임을 알 수 있다. 그러면 다시 s 명령으로 getnameO
함수를 빠져나간다. 그리고 s 명령으로 계속 한 단계씩 진행해 str = getnameO； 이후
의 상황-0-.루- 간 후 main() 함수에서 str 변수에 name 변수의 주소인 0xbfffe600 값
이 저장되는지 확인한다.

32 1부_ 튜토리얼

===== PAGE 34 =====
M root@os：/temp/tes1/temp___________________ H 同 E3'
0000222W203W00Wb¥ll1^023Ktt02Wntf023Btf276?“T O61 凍3
203tf 80Wr
(gdb) s
main () at like.c:20
28
printF("I like you.Wn");
1： str = 0x42130al4 " I#나fO23B ctf001@^p'
(gdb) s
19
str = getnane();
1: str = 0x4213Oa14 ” tftW023B c»081@：샤,,
(gdb) s
20
printffl 즈ike you.Wn");
1: str =| OxbFFFe；5B8 “kira：7]
(gdb)

P

［그림 1-2이 getnameO 함수 호출 이후의 모습

getnameO 함수의 호출 후 str 변수에는 name 변수의 주소 값인 0xbfffe600번지가
들어가 있고, 0xbfffe600번지에는 “kara”라는 문자열이 들어 있음을 확인할 수 있다.
그러므로 아직까지는 아무 문제가 발생하지 않았음을 알 수 있다. 문제를 발견하기 위
해 다시 s 명 령으로 한 단계 더 진행시킨다.
떠 root@os：/temp/tesytemp

0同£1

28
瓦:고1tf("I like you.tfn");—
1： Str = 0x42130a14 " WtW023B 다#001@：갸"
(gdb) s
19
str = getnameO ；
1： Str = 0x42130a14 " ttttt023B ctt001@?|："
(gdb) s
26
printf("I like you.tfn");
1: str = 0xbFFfe680 "kara"
(gdb) s
I like you.
21
printf(^,%stfn,,, str);
1:|str = OxbFFFeZofl ” i B22B"~1
*b)

B

［그림 1-21］ name 변수 값이 변경되어 버린 모습

그런데 printf(“l like you.\n”)； 함수가 호출되고 화면에 “I like you.” 문자열이 출력된
순간 name 변수의 값이 변경돼 버렸다. main() 함수의 str 변수 값은 이전 name 변수
의 주소인 0xbfffe600을 그대로 가지고 있지만, Oxbfffe6OO번지의 값이 “kara"에서 이
상한 문자열로 변경된 것을 확인할 수 있다.
지금까지의 정보들을 바탕으로 유추할 수 있는 결론은 getnameO 함수의 name 변수가 함수
스택에 생성되는 지역변수이므로 getnameO 함수가 호출될 때만 유효하고 getnameO
함수가 끝나는 순간 유효하지 않기 때문에 발생하는 문제라는 점을 알 수 있다.
결국 getnameO 함수의 호출이 끝난 직전까지는 이전 name 변수로 잡혔던 주소에

“kara” 문자열이 있었지만 printf() 함수가 호출되는 순간 getnameO 함수의 name 변
수 위치에는 printfO 함수의 지역변수들이 할당되므로 name 변수의 위치에 있던 값들
이 printfO 변수의 값들로 변경된 것을 확인할 수 있다.

1장_ 튜토리얼 33

===== PAGE 35 =====
이런 문제를 해결하려면 ［예제 1-8］ 과 같이 소스에 static 키워드를 추가한다. 그러면
변수가 사라지는 현상은 해결된다. 그렇지만 아직까지는 scanf 함수에서 입력되는 문
자열의 범위를 검사하지 않기 때문에 오버플로우가 발생할 수 있는 문제의 소지가 남
아있다. 하지만 당장 쓰는 데는 문제가 없을 것이다.
: 컴파일러는 static 키워드를 붙인 변수에 한해 해당 변수를 프로그램의 데이터 영역에 할당한다. 지역변
수의 경우 스택에 할당되어 함수 내에서만 변수의 공간이 유효하지만, 데이터 영역에 할당되면 메모리
의 일정 공간을 실제로 할당받으므로 프로그램이 종료할 때까지 변수는 자신만의 공간을 갖는다.

〔예제 1-8］

like.c 소스 파일 내용

#include <stdio.h>
void lovecall();
char *getname()
{
static char name[128];
printf("Input name : ");
scanf("응s", name);
return name;
}
int main()
{
char *str;
str = getname();
printf("I like you.\n”);
printf("%s\n"z str);
return 0;
}

34 1 부_튜토리얼

===== PAGE 36 =====
B root@os：/temp/test/temp
[rootQos temp]# make
gee -W -Wall -02 -g -o like like.c loue.c -1m
[root（흐os temp]tt
[root（흐os temp]tt ./like
Input name : kara
I like you.
kara |
[root（흐os tenp]tt |

［그림 1-22］ static 키워드를 추가한 후의 결과

사실 ［예제 1-8］ 은 번거롭게 디버거를 사용하지 않고 소스만 보고도 잘못되 었다는 것
을 누구라도 금방 알 수 있다. gdb 를 이용한 좀 더 그럴듯한 디버깅은 4부 “디버깅”과
정에서 다룬다. 그리고 4부에서는 gdb뿐만 아니라 GUI 디버거인 DDD를 포함해 각종
디버깅 유틸리티를 자세히 다룰 예정이다.
이제 버그도 잡았고 프로그램도 어느 정도 안정화를 이뤘다. 지금까지 작성한 likeU 프
로젝트를 인터넷에 공개한다고 해 보자. 그래서 세계 각국의 수많은 개발자가 개발에
동참하길 원한다. 또는 이제 팀을 만들어 혼자가 아닌 팀 단위 프로젝트로 진행한다고
해 보자. 이렇게 다수가 프로젝트에 참여한다고 할 때에는 여러 가지 문제가 발생한다.
첫째, 소스의 동기화 문제가 있을 수 있다. 각기 다른 소스로 작업을 하면 소스가 동기
화되지 않는다. 동기화되더라도 한 소스로 작업을 하면 동시에 수정하지 못하거나 동시
에 수정할 경우 덮어 쓰기 문제가 발생한다.
예를 들면 A라는 개발자와 B라는 개발자가 있을 때, A 개발자가 like.c 파일을 수정하
는 도중에 B 개발자가 like.c 파일을 열어 수정 작업을 했다. A 개발자가 수정이 끝나
저장하고 이후 B 개발자가 like.c 파일을 저장했다면 A 개발자의 작업 내용은 사라져
버리고 만다.
또 다른 문제는 어떤 사람이 어떤 작업을 했는지 알기가 힘들어 작업 관리가 용이하지
않고, 새로운 기능의 추가 또는 빈번한 테스트 과정 중에 소스의 관리가 용이하지 않다
는 점이다. 다수가 참여하는 프로젝트에서는 이런 문제가 중요하며, 또한 반드시 해결
해야 하는 문제다. 이때 사용 가능한 유틸리티가 바로 cvs 와 subversion 같은 버전 관
리 유틸리티다.

1장_튜토리얼 35

===== PAGE 37 =====
05 svn을 사용한 프로젝트 버전 관리 )
svn의 원리를 간단하게 알아보자. 먼저 저장소(repository)라는 공간을 만들고 그곳에
프로젝트 파일들을 미리 넣어놓는다. 각 개발자는 저장소에서 프로젝트 파일을 받아와
수정한 후 다시 저장소에 있는 프로젝트 파일들을 갱신한다. 이때 svn이 각 개발자가
수정한 부분에 대해 동기화를 자동으로 수행한다.

［그림 1-23］ svn을 사용한 프로젝트 버전 관리

svn을 사용하려면 먼저 저장소를 만들어 야 한다. 다음 명 령으로 svn 저장소를 만들 수
있다.
$ svnadmin create --fs-type fsfs /tmp/repository

/tmp/repository는 임의의 저장소 경로로, 원하는 위치에 원하는 이름을 사용하면 된
다. ［그림 1-24］ 와 같이 어떤 메시지도 출력되지 않으면 정상적으로 저장소가 만들어
진 것이다.
우분투 사용자들은 다음 명령으로 subversion을 먼저 설치하기 바란다. 우분투는 데스크톱용 OS를
지향하는데, 그래서 그런지 우분투 배포판을 개발용으로 사용하려면 설치하고 손봐야 할 것들이 많이
있다.

sudo apt-get install subversion

'디 root@os：/temp/test/temp
[root（흐os tenp]tt sunadmin create —— FsFs /tnp/repository
[root@os temp]tt |

［그림 1-24］ 저장소 생성

36 1 부_튜토리얼

-IQI 시

===== PAGE 38 =====
다음으로 작성한 소스를 저장소에 넣는다. 소스 파일이 있는 디렉토리（필자의 경우는

temp이다）의 상위 디렉토리로 가서 다음 명령을 내린다.
$ svn import ./temp file:///tmp/repository/likeU -m "likeU project”
-1 root@os：/temp/test
[rootllos temp]tt Is
소스 파일
Makefile like.c loue.c ：
위치
[rootl흐os tenp]ttj)wd
》ten»p/te；st/t；；ip']............
[root(흐os temp]tt cd ..
[root@os test]#
[root!흐os test]tt sun import ./temp File:///tnp/repository/likeU -I
ID "likeU project"
temp/like.c
Adding
Adding
temp/loue.c
Adding
temp/MakeFile
Committed reuision 1.
[root@os test]tt |

山
［그림 1-25］ 프로젝트 파일 저장소에 등록

temp 는 지금까지 우리가 작성한 프로젝트 파일이 들어 있는 디렉토리이고, /tmp/
repository는 이전에 생성한 저장소를 의미한다. -m 옵션 뒤에는 적고 싶은 말을 적는
다. 예를 들면 “likeU project start”와 같은 말을 적으면 된다.
［그림 1-25］ 는 svn import 명령을 실행한 결과를 보여준다. test 디렉토리에는 temp
디렉토리가 있고, temp 디렉토리에는 프로젝트 소스 파일들이 있다. 프로젝트 상위 디
렉토리인 test 디렉토리에서 svn import 명령을 실행하면 Adding 메시지와 함께 소
스 파일들이 저장소에 저장된다. 이제 svn 을 사용해 프로젝트를 관리하기 위한 모든
준비는 끝났다. 앞으로 각 개발자들은 저장소에서 소스 파일을 받아와 수정하고, 수정
한 파일을 저장소에 갱신하면서 프로젝트를 진행하면 된다. 저장소에 있는 프로젝트
파일을 받아오는 일을 checkout 이라 하고, 임의의 디렉토리에서 아래 명령을 사용해

checkout할 수 있다.
$ svn co fi丄e:///tmp/repository/likeU

위 명령을 실행하면 ［그림 1-2이과 같이 저장소에서 likeU 프로젝트 파일들을 받아온다.

1장—튜토리얼 37

===== PAGE 39 =====
g] root@os：/temp/test
[root@os test]tt is
______________________________________________
[rootQos test]# |sun
://7Fiiip'7F"e'pository/likeir
A likeU/like .c
A likeU/loue.c
A likeU/Makefile
Checked out reuision 1.
[root@os test]#
[rootl흐os test]# Is
iiiceii tMip
[root@os test]# is likeU/
Makefile like.c loue.c
[root（흐os test]# |

[그림 1-26] svn checko내 화면

<EE 저장소에서 likeU 프로젝트 파일을 받아왔으면 이제 더 이상 원본인 temp 디렉토리는 사용하지 않을
것이다. temp 디렉토리와 likeU 디렉토리의 차이점은, likeU 디렉토리에는 프로젝트 소스 파일들과 함
께 svn 제어 정보가 들어있다는 점이다. likeU 디 렉토리에서 Is -al 명령으로 살펴보면 .svn이라는 svn
제어 정보를 담고 있는 디렉토리를 확인할 수 있을 것이다.

이제 프로젝트 수행에 필요한 소스 파일이 확보되 었다. 확보된 소스를 가지고 수정 및
추가 작업을 하면 된다. 그리고 작업 이 끝났으면 다시 저장소로 프로젝트 파일을 갱신
한다.

like.c 파일에 새롭게 ［그림 1-2刀과 같이 주석을 추가했다.

［그림 1-27］ like.c에 주석 추가

수정된 내용을 저장소에 반영하는 작업을 commit이라 부르고 likeU 디렉토리 내에서
다음 명령을 내리면 저장소에 있는 like.c 파일 버전이 증가하면서 추가된 내용이 반영
된다.
$ svn ci -m "like.c 주석추가" like.c

38 1 부— 튜토리얼

===== PAGE 40 =====
［그림 1-281 svn 저장소의 like.c 파일 갱신

-m 옵션 뒤에 오는 문자열은 로그에 남기기 위한 메시지다. like.c 파일을 수정했다면
어떤 내용을 수정 했는지에 대한 로그를 남기면 된다. 남겨진 로그는 svn log like.c 명
령으로 그동안 어떤 로그가' 남겨졌는지 확인할 수도 있다. 이렇게 갱신된 내용은 다른
개발자가 svn co 명 령으로 새롭게 체크아웃할 때 반영된다.
어떤 개발자가 주석이 추가되기 전에 이미 likeU 프로젝트를 저장소에서 받았다면 그 프
로젝트 소스에는 주석이 반영되지 않았을 것이다. 이럴 때는 likeU 디렉토리에서 svn up
명령만 내리면 갱신된 내용이 저장소에서 해당 개발자의 프로젝트 파일들에 반영된다.

A, B 두 명의 개발자가 동시에 like.c 파일을 받아와서 수정하고 갱신하는 상황이 발생
하는 경우 수정한 부분이 서로 다르다면 svn 은 수정된 부분을 서로 조합해 소스를 동
기화한다. 그리고 서로 같은 부분을 수정해 소스의 충돌이 발생한다면 충돌 발생 여부
를 개발자에 게 통보하고 개발자가 결정을 내릴 수 있게 한다.
이렇게 소스를 수정하고 저장소에 반영하고, 다른 개발자가 갱신한 내용을 저장소에서
받아오는 과정을 통해 여러 개발자가 좀 더 효율적으로 개발할 수 있다. svn의 기능에
는 이것 외에도 할 이야기가 많지만 7부 “프로젝트 관리”에서 다룬다.
이제 svn을 사용함으로써 작업 내용의 동기화 문제와 충돌 문제가 해결되었다. 하지만
이 프로젝트를 공개하거나 여러 사람과 함께 팀 단위로 수행하기에는 아직 한 가지 문
제가 남아있다. 그것은 바로 문서화가 되지 않았다는 점이다. 문서화가 되지 않은 프로
젝트는 다른 사람이 이해하기 어렵고, 작성한 본인도 시간이 지나면 망각의 늪에 빠져
버리기 십상이다.
보통 문서화는 기본적으로 설계하면서 작성하고, 구현이 완료된 후 작성하는데 여간
번거로운 작업이 아니다. 하나의 소스 파일에 여러 사람이 기능을 추가하는 경우 더
더욱 문서화가 어 렵다. 이 렇게 귀 찮고 하기 싫은 문서화를 해 줄 수 있는 무언가가 있
다면 우리의 삶이 한결 윤택해질 것이다. 이럴 때 쓰라고 나온 것이 doxygen 이다.

doxygen을 사용하면 주석을 통해 자동으로 문서를 생성할 수 있다.

1장_ 튜토리얼 39

===== PAGE 41 =====
06 doxygen을 이용한 문서화
doxygen은 소스 파일 내에 사용된 주석을 바탕으로 문서를 생성하는 유틸리티다.
doxygen이 생성하는 문서 포맷에는 html, doc, pdf, dvi 등 여러 가지 포맷이 있다.
doxygen을 사용하려면 like.c 파일 내에 ［예제 1-이와 같이 doxygen이 이해할 수 있
는 주석을 추가해야 한다.
〔예제 1-9〕 like.c 파일에 doxygen 주석 추가
/★★

* @file
* @brief
* @author
* @date

like.c
main source file
WOOS

2009.04.27

* likeU 프로젝트소스파일

*/
#include <stdio.h>

/★★
* @brief
* ©return

getname 함수입니다.
입력받은 이름

*/
char *getname()
{
static char name[128];
printf ("Input name : ");
scanf("%s", name);
return name;

* @brief main 함수입니다.
* @return 0 = OK, 1 = error

*/
int main()
{
char *str;

40 1 부— 튜토리얼

===== PAGE 42 =====
str = getname();
printf ("I like you.\n");
printf("%s\n", str);
return 0;
}

그런 다음 likeU 디렉토리 내에서 다음 명령으로 doxygen 설정 파일을 생성한다.
$ doxygen -g

: 우분투 사용자는 위 명령을 내리기 전에 다음 명령으로 doxygen을 먼저 설치하기 바란다.

sudo apt-get install doxygen

[그림 1-29] Doxyfile 생성 모습

doxygen -g 명령을 내리면 Doxyfile 파일이 생성되는데, 이 파일은 doxygen 의 설정
파일로 doxygen의 여러 기능을 제어하는 데 사용된다. doxyfile을 열어보면 제공하는
많은 기능만큼 여러 옵션이 있는데, 이런 기능들은 나중에 자세히 살펴보기로 하고 우
선은 다음 옵션들만 설정한다.
〔예제 1-10〕 Doxyfile 수정 내용

PROJECT NAME

likeU

EXTRACT_ALL

YES

1 장—튜토리얼 41

===== PAGE 43 =====
마지막으로 다음과 같이 doxygen 명령을 내리면 likeU 디렉토리에 html 디렉토리와

latex 디렉토리가 생기면서 각 디렉토리에 문서화한 각 포맷의 문서가 생성된다.
$ doxygen
HI root@os：/temp/test/likeU
Generating
group documentation_________
Generating
directory documentation____________
Generating
namespace index________
Generating
group index_______
Generating
directory index-..
Generating
example index________
Generating
File ne fiber index__________
Generating
namespace member index_________
Generating
page index_______
Generating
graph info page...
[root（흐os likeU]tt
[root（흐os likeU]tt Is
DoxyFile Makefile |
^
• | like.c
[root（흐os likeU]tt
[root@os likeU]1t |

[그림 1-30] doxygen 명령 모습

［그림 1-31］ 은 html 디렉토리에 있는 index.html 파일을 웹 브라우저로 열어본 모습
이다.

［그림 1-31］ index.html 파일을 웹 브라우저로 연 모습

42 1부_튜토리얼

===== PAGE 44 =====
주석으로 doxygen에 제공한 정보가 많지 않아 다소 부족하긴 하지만 어 쨌든 html 문
서가 만들어졌다. doxygen 에서 생성하는 문서의 질은 얼마나 많은 정보를 doxygen
에 제공하느냐에 달려있다. 우리가 제공한 정보는 턱없이 부족하기 때문에 이쯤에서 만
족하자.

doxygen을 사용해 훌륭한 문서를 만드는 방법은 7부 ‘프로젝트 관리 ’에서 알아본다.
이제 다소 민망(?)하긴 하지만 문서화도 했고 svn을 사용해 세계 각지의 개발자와 협
력해 아주 훌륭한 likeU 프로젝트를 완성 했다. 많은 사람이 likeU 프로그램을 사용하기
를 원하고 있다.
그러나 likeU 프로젝트 소스를 배포하는 데는 아직 문제가 남아있다. likeU 프로젝트가
개발된 컴퓨팅 환경과, 컴파일되어 사용할 환경이 다르기 때문이다.
사용자의 운영체제 환경은 Solaris나 BSD, 혹은 리눅스일 수도 있다. 그리고 또한 리눅
스 내에서도 배포판마다 다른 점들이 있다.
컴파일러의 종류, 특정 라이브러리의 유무, C 소스 내에서 사용된 데이터 타입의 크기
등과 같은 서로 다른 점들로 인해 정상적으로 컴파일되지 않거나 컴파일되더라도 정상
적으로 작동하지 않을 수 있다.
개발자는 어떤 환경에서든 컴파일되고 동작할 수 있는 이식성을 제공해야 한다. 물론
모든 환경에 다 이식되는 프로젝트를 만들기는 매우 힘들지만 최소한 컴파일이 안 된
다면 그 이유는 알려 줄 수 있어야 한다.
지 금 의 프로젝트에서는 make 가 컴파일 과정을 담당하는데, make 는 기술 파일

(Makefile)에 기술된 대로 컴파일 명령을 수행한다. 결국 이식성 높은 프로젝트를 만들
려면 컴파일 환경을 체크해 각 환경에 맞는 기술 파일을 동적으로 만들어야 한다. 물론
소스의 내용도 각기 다른 환경을 포용할 수 있도록 작성되어야 한다.
기술 파일을 동적으로 만드는 일은 configure 셸 스크립트가 하는데, 이런 configure
스크립트는 autoconf 유틸리티가 생성한다. 그럼 likeU 프로젝트에 autoconf 를 사용
해 좀 더 이식성 높은 프로젝트를 만드는 방법을 알아보자.

1장_ 튜토리얼 43

===== PAGE 45 =====
07 L autotools를 사용한 이식성 높은빌드서
a니totools란 autoconf 패키지나 automake 패키지에 들어 있는 일련의 유틸리티들을
통틀어 지칭하는 말이다. autoconf는 configure.ac 파일을 입력으로 받아 config니re
스크립트를 생성하고, config니re 스크립트는 시스템 정보를 수집하고 config.status 스
크립트를 생성한다.

config.status 스크립트는 config니re 스크립트가 수집한 시스템 정보를 바탕으로
Makefile .in 파일을 입력으로 받아 Makefile 을 생성한다. Makefile .in 파일은 Makefile
의 템플릿 파일로, configure가 수집한 시스템 정보를 바탕으로 Makefile을 만드는 데
사용된다.

autoconf를 사용해 config니re 스크립트를 생성하고 configure 스크립트를 실행해
Makefile을 동적으로 생성하는 대략적인 구조는 ［그림 1-32］ 와 같다.

［그림 1-32］ autoconf의 실행 과정

automake는 Makefile.in 파일을 자동 생성시키는 유틸리티다. 개발자가 직접
Makefilejn 파일을 작성하는 것보다 많은 시스템 정보를 이용하므로 이식성 높은
Makefile을 생성할 수 있는 템플릿 파일을 만든다.

44 1부—튜토리얼

===== PAGE 46 =====
configure.ac

Makefile

[그림 1-33] automake 실행 과정

먼저 autoconf의 입력으로사용되는 configure.ac 파일을 ［예제 1-11］ 과 같이 작성한다.
〔예제 1-11］

configure.ac 파일의 내용

AC_INIT(likeU, 0.0.1, woos@hanbit.co.kr)
# C 컴파일러와 CFLAGS 옵션을체크
AC_PROG_CC
# libm.a 라이브러리유무를체크
AC_CHECK_LIB ( [m] , [sin] )
# libintl.h 헤더파일의유무를체크
AC_CHECK_HEADERS ( [libintl.h] )
# setlocale 함수의 사용 유무를 체크
AC_CHECK_FUNCS([setlocale])
# • / configure 스크립트 수행 후 생성할 파일을 지정
AC_CONFIG_FILES ( [Makefile] )
AC_OUTPUT

［예제 1-11］ 과 같은 configure.ac 파일을 작성하고 autoconf 명령을 내리면 autoconf
가 configure 스크립트를 만든다.

1장—튜토리얼

45

===== PAGE 47 =====
'히 root@os ：/temp/test/likell
[rootdos likeU]tt Is
DoxyFile Makefile configure.ac
[rootQos likeU]tt __________ _______
[root(흐os likeU]ttfautoconT]
[root(흐os likeU]tt Is
DoxyFile _________________ configure.ac
Makefile |configure |
[rooteos likeU]tt |

[그림 1—34] autoconf 명령 수행

우분투 사용자는 autoconf 명령을 내리기 전에 다음 명령으로 autoconf를 먼저 설치하기 바란다.

sudo apt-get install autoconf

기존의 Makefile을 지우고 다음과 같은 Makefile.in 파일을 만든다.
〔예제 1-12〕 Makefile.in 파일의 내용

CC
CFLAGS
LDFLAGS

= @cc@
= @CFLAGS@
= @LIBS@

all : like
like : like.c love.c
(CC) $ (CFLAGS) -o $@ $A $ (LDFLAGS)
사이 간격이 TAB임을 주의

clean :
< > @rm -rf *.o like
사이 간격이 TAB임을 주의

@CC@와 @CFLAGS@, @LIBS@는 configure 스크립트를 수행한 후 configure 스크립
트가 수집한 시스템 정보로 각각 치환된다. 예를 들어 시스템에 있는 C 컴파일러가 gcc
라면 @CC@는 gcc로 치환되고, cc라면 @CC@는 으로 치환된다.

./config니re 명령을 실행해 보면 configure.ac 파일에 적어준 대로 시스템 정보를 수집
하고 있음을 확인할 수 있다.

46 1부—튜토리얼

===== PAGE 48 =====
| B root@os：/temp/test/likell

-lOl x|

[rootdos
likeU]tt ./configure
checking
for gcc— gcc
checking
For C compiler default output File name____________________ a.out
checking
whether the C compiler works______________ yes
checking
whether
we are cross compiling___________ no
checking
For
suffix oF executables—
checking
For suffix
of object Files__________ o
checking
whether we are using the GNU C compiler yes—<
［컴파일러 정보
checking
whether
gcc accepts -g— yes
checking
For gee option to accept ANSI C____________ none needed
checking
For sin
in
-Im...
yes_________________________________
libm.a
checking
how to run the C preprocessor______________ gcc -E
for
checking
egrep_______ grep -E
checking
For ANSI C header files____________yes
checking
For sys/types.h...
yes
checking
For sys/stat.h...
yes
checking
For stdlib.h________ yes
checking
For string.h________ yes
checking
for
memory.h—
yes
checking
For strings.h—
yes
checking
For inttypes.h________ yes
checking
For stdint.h________ yes
checking
For unistd.h— yes
checking
libintl.h usability______________으es
checking
libintl.h presence yes
checking
For libintl.h__________ yes----------------； libintl.h
checking
for setlocale— yes-----------------------------configure: creating ./config.status
k setlocaleO:
config.status: creating Makefile
[root（흐 os likeU]tt
likeU]tt is Makefile
[root@os
Makefile
[root（흐 os likeU]tt |

[그림 1-35] ./configure 명령 수행

./configure 스크립트를 수행한 후 최종적으로 만들어진 Makefile을 열어보면 다음과
같이 @CC@, @CFLAGS@, @LIBS@가 시스템에서 수집한 정보로 치환됐음을 확인할
수 있다.

[그림 1—36] ./configure 명령 수행 후에 생성된 Makefile

1장—튜토리얼 47

===== PAGE 49 =====
이제 make 명령을 내리면 컴파일된다.

［그림 1—37］ make 명령을 수행한 화면

지금까지 autoconf* 사용해 좀 더 이식성 높은 프로젝트 빌드 방법을 알아보았다. 현
재의 소스는 그렇게 복잡하지 않으므로 굳이 a니tomake를 사용해 Makefile의 템플릿
파일인 Makefilejn 파일을 만들 필요가 없다. 그렇지만 프로젝트의 규모가 커진다면

a니 tomake 를 사용해 Makefile .in 파일을 생성하는 것이 좀 더 높은 이식성을 가진 프로
젝트를 만드는 데 도움이 된다.
이제부터 automake를 사용해 좀 더 이식성이 높은 Makefile.in 파일을 생성하는 방법
을 알아보자. automake를 사용하려면 먼저 configure.ac 파일을 ［예제 1-13］ 과 같이
수정해 automake를 사용할 것이라고 명시해야 한다.
〔예제 1-13)

configure.ac 파일의 내용

AC_INIT(likeU, 0.0.1, woos@hanbit.co.kr)
AM_INIT_AUTOMAKE( [likeU] , [0.0.1] )
# C 컴파일러와 CFLAGS 옵션을체크
AC_PROG_CC
# libm.a 라이브러리 유무를 체크
AC_CHECK_LIB([m], [sin])
# libintl.h 헤더 파일의 유무를 체크
AC_CHECK_HEADERS([libintl.h])
# setlocale 함수의 사용 유무를 체크
AC_CHECK_FUNCS([setlocale])
# . /configure 스크립트 수행 후 생성할 파일을 지정
AC_CONFIG_FILES ([Makefile] )
AC_OUTPUT

48 1부_튜토리얼

# 추가부분

===== PAGE 50 =====
그리고 Makefile.in 파일을 지우고 Makefile.am 파일을 ［예제 1-14］ 와 같이 작성
한다.
〔예제 1-14)

Makefile.am 파일의 내용

bin_PROGRAMS
like_SOURCES

like
like.c love.c

다음 명령을 차례로 내린다.
aclocal
autoconf
automake --add-missing foreign --copy

우분투 사용자는 위 명령을 내리기 전에 아래 명령을 통해 automake를 먼저 설치하기 바란다.

sudo apt-get install automake

R root@os：/temp/test/likeU
[rootQos 1ikeUftt aclocal >& /deu/null
[root@os
likeU]tti
autoconf
likeU]tt|automake add-missing --------------------------------------------------------[rootQos
[root（흐 os likeU --------------------------------------------------------------------------------------------- likeU]tt Is
[rootOos
aclocal
DoxyFile
configure.ac install-sh
like.c
[Make File, am
depconp
loue.c
jilakefile.in | configure
like
missing
[root@os likeU]tt |

[그림 1-38] automake 명령 수행

Is 명령을 수행하면 automake가 아래와 같은 Makefilejn 파일을 만든 것을 확인할 수
있다. automake 가 만든 Makefile .in 파일은 직접 손으로 작성한 Makeffle.in 파일보다

configure 스크립트｝ 수집한 정보를 더 많이 이용하므로 좀 더 이식성 높은 빌드를
할수있다.

1장_ 튜토리얼 49

===== PAGE 51 =====
'이 rgo|@으은:/temp/t흐st/likeU
It Makefile.in generated by automake 1.9.5 from Makefile.am.
tt Oconfigure_input@
tt Copyright (C) 1994, 1995, 1996, 1997, 1998, 1999, 2000, 2881, 2902,
# 2803, 2004, 2005 Free Software Foundation, Inc.
# This Makefile.in is free software; the Free Software Foundation
it giues unlimited permission to cop^ and/or distribute it,
# with or without modifications, as long as this notice is preserved.

I

# This program is distributed in the hope that it will be useful,
tt but WITHOUT ANY WARRANT?, to the extent permitted by law; without
« euen the implied warranty of MERCHANTABILITV or FITNESS FOR A
tt PARTICULAR PURPOSE.

iasoj4AMia
SOURCES = $(like_SOURCES)
srcdir = • /'■r.ir3
top_srcdir =
UPATH =
pkgdatadir = $(datadir)/
pkglibdir = $(libdir)/
pkgincludedir = $(includedir)/
top_builddir = .
an三cd = CDPATH= $$<ZSH_UERSIOH*.}$(PfiTH_SEPARATOR) && cd
INSTALL =
install_sh_DATft = $(install_sh) -c -n 644
instal〔하^PROGRAM = $(install_sh) -c
install_sh_SCRIPT = $(install_sh) -c
INSTfiLL_HESDER = $(INSTfiLLDfiTfi)
~
~

9,8-1 꼭대기

[그림 1—39] Makefile.in 파일 내용

이제 ./configure 명령을 다시 실행하면 configure 스크립트가 수집한 정보를 바탕으
로 Makefile.in 파일을 Makefile 파일로 바꾼다. 그런 다음 다시 make 명령을 내리면

like 실행 파일이 컴파일된다.
OH root@os：/temp/test/likeU
configure: creating ./config.status
config.status: creating Makefile
config.status: executing depfiles commands
[rooteos likeU]tt make
if gcc -DPACKAGE_NfiME=tf"likeUW" -DPfiCKAGE_TARNfiME=tf"likeutf" -DPA
C K A G E _ U E R S I 0 N = t f " 0 . 0 . 1 W " - D P A C K A G E _ S T R I N G = t f " l i k e U W 0 . 0 .키 # " - D P A C K
AGE_BUGREPORT=W”woos@hanbit.co.krtf" -DPACKAGEWlikeUtt" -DUERSIO
N가iFfl.O.ltf" -DHfiUE_LIBM=1 -DSTDC_HEADERS=1 -DHAUE_SVS_TVPES_H=1
- D H A U E _ S V S _ S T A T _ H = 1 -애 A U E _ S T D L l i _ H= 1 -D HAUE _ STR IN G_ H= 1 - D H 6 U E_M
EMORV H = I - DHAU E_ STRINGS _ H ： I - DHAUE _ IHTTVPES Z H = I - DHAUE _ STDIN < H
=1 -DiiAUEjJNisTDlH너 -애6UE_LIBINTI_ZH=I -애AUE_SETLOCALE=I -I?
-g -02 -MT like.o -HD -MP -MF ".deps/like.Tpo" -c -o lik
e.o like.c; W
then mu -F ".deps/like.Tpo" deps/like.Po"; else rm -f ".deps/l
ike.Tpo"; exit 1; Fi
if gcc -DPACKAGE_NAME=W"likeUW" -DPACKAGE_TfiRNAME=tf"likeutf" -DPA
CKAGE_UERSI0N=W"0.0.Itt" -DPACKfiGE_STRING=tf"likeUtf 0.0.Itf" -DPACK
AGE_BUGREPORT=tt"woos@hanbit.co.krtt" -DPACKAGE=W"likeUtf" -DUERSIO
N=W"0.0.1tt" -애AUE_LIBM=1 -DSTDC_HEADERS=1 -DHfiUE_SVS_TVPES_H=1
-D HAUE _S V S _STAT_H=1 -애 ftUE_STDI_l6_H=1 -DHfiUE_STRING_H=1 - D H 6 U E_N
EMORV _ H = I - DHAU E_ STRINGS _ H = I - DHA U E _ INTTYPES _ H = I -DHAUE_STDINT_H
= 1 -DHfiUE_UNISTD2H=1 -DHAUE LIBINTL”H=1 -DHAUE_SETL0CAI_E=1 -I?
-g -02 -MT loue.o -MD —MP -MF ’’.deps/loue.Tpo” -c -o loul
e.o loue.c; tf
then mu -F ”.deps/loue.Tpo" ".deps/loue.Po"; else rm -f ".deps/1
oue.Tpo"; exit 1; Fi
gcc -g -02 -o like like.o loue.o -In
[rootgos likeU]tt Is like
iike |
[rootBos likeUJtt |
j

[그림 1—40] ./configure 명령 후 make 명령으로 컴파일

50

1 부—튜토리얼

===== PAGE 52 =====
이제 어디서든 쉽게 이식될 수 있고 컴파일될 수 있는 likeU 프로젝트가 완성되었다.
지금까지의 작업만0-루도 매우 훌륭한 프로젝트가 만들어졌다. 그렇지만 아직까지는
소스 파일을 받아 컴파일 과정을 거쳐야만 사용할 수 있다.
소스를 배포하지 않고 이미 컴파일된 바이너리 파일을 배포한다면 사용자들은 분명 좀
더 쉽게 like 프로그램을 사용할 수 있을 것이다.
컴파일된 실행 파일을 배포할 때 tarball(*.tar.gz) 형태로 묶어 제공하는 것도 한 가지
방법이 될 수 있지만, 그렇게 배포한다면 설치, 제거, 유지 관리가 용이하지 않을 것이
다. 이런 경우 레드햇에서 사용하는 설치와 관리가 쉬운 RPM 파일로 만들어 배포하는
것이 좋은 대안이 될 수 있다.

C8LRPM 패키징
RPM 패키지를 빌드하려면 먼저 빌드 트리를 구축해야 한다. 빌드 트리는 일련의 디렉
토리 구조로, 레드햇 계열 사용자라면 /usr/src/redhat 디렉토리 아래에서 미리 구축
된 빌드 디 렉토리를 확인할 수 있다.
자신의 시스템에 빌드 트리가 구축되어 있지 않다면 다음과 같은 구조의 디렉토리를

mkdir 명 령으로 생성하기 바란다.
redhat
|— BUILD
|— RPMS
I |-- athlon
I I— i386
I |— i486
I |— i586
I |— i686
I '—— noarch
I— SOURCES
I— SPECS
SRPMS

1 장—튜토리얼 51

===== PAGE 53 =====
, 우분투 사용자들은 이번 절을 진행하기 전에 다음 명령을 내려 rpm 시스템을 설치하기 바란다. 그러면

/usr/src/rpm 아래에 빌드 트리도 같이 만들어질 것이다.
sudo apt-get install rpm
앞으로 우분투 사용자는 /usr/src/redhat이라고 말한 부분을 모두 /usr/src/rpm으로 이해하고 읽어
가기 바란다.

레드햇 사용자라면 이미 존재하는 /usr/src/redhat 디렉토리를 그냥 이용하면 된다.
그러면 먼저 프로젝트 소스 파일이 들어 있는 디렉토리명을 ［패키지명］-［버전］ 형태로
바꾼다. 예를 들면 likeU 디 렉토리를 likeU-0.0.1 로 바꾼다.
$ mv 丄ikeU likeU-0.0.1

그리고 다음의 명령으로 likeU-0.0.1 디렉토리를 통째로 likeU-O.O.l.tar.gz 파일로
압축한다.
$ tar -czf likeU-0.0.1.tar.gz likeU-0.0.1

압축된 likeU-O.O.l.tar.gz 파일을 빌드 트리인 /usr/src/redhat/SOURCES 디렉토리
로 복사한다. 이 압축된 소스는 차후에 압축 해제 과정을 거치고 컴파일 과정을 거쳐

RPM 패키지 빌드에 이용된다.

［그림 1-41］ 명령 순서

/usr/src/redhat 또는 /usr/src/rpm 디렉토리에 파일을 복사하려면 root 권한으로 복사해야 한다. 페
도라 사용자라면 su 명령을 이용해 root 유저로 전환한 후 복사하면 되고, 우분투 사용자라면 다음 명
령과 같이 sudo 명령을 앞에 붙여 파일을 복사하기 바란다.
sudo cp -f likeU-0.0.1.tar.gz /usr/src/rpm/SOURCES
또한 rpm을 빌드하거나 설치할 때도 root의 권한이 필요하기 때문에 이후에 나오는 명령들의 경우, 우
분투 사용자라면 모두 sudo 명령을 앞에 붙여 사용하기 바란다.

52 1부—튜토리얼

===== PAGE 54 =====
이제 /usr/src/redhat/SPECS 디렉토리에 likeU-O.O.l-l.spec 파일을 ［예제 1-15］ 와
같은 내용으로 생성한다. specs 파일은 RPM 패키지를 빌드하기 위한 명령과 패키지
정보를 적어놓은 파일이다.

%define version 0.0.1
%define name likeU
Summary:
Name:
Version:
Release:
Prefix:
Group:
Source:
BuildRoot:
License:
Uri:

I like you program
응{name}
%{version}
1
/usr
Utilities/Text
%{name}-%{version}.tar.gz
/usr/tmp/%{name}-%{version}
GPL
http://woos.wowdns.com/likeU/

%description
설명: I like you 프로그램입니다. 소중한사람에게 선물하세요. :)

%prep
%setup q
%build
. / configure---------------------------------make
%install
mkdir -p $RPM_BUILD_ROOT/usr/bin
make prefix=$RPM_BUILD_ROOT/usr install
%clean
rm -rf $RPM_BUILD_ROOT
%files
응defattr(—,root,root)
% {_p refix} /bin/like
%changelog
* Wed Dec 15 1999 chang-woo baek <bckddn@daum.net>
- updated to 991203
- build proces changed

1 장—튜토리얼 53

===== PAGE 55 =====
마지막으로 /usr/src/redhat/SPECS 디렉토리에서 다음 명령을 내리면 RPM 패키지를
빌드한다.
$ rpmbuild -ba likeU-0.0.1-1.spec

주의할 점은 레드햇 9.0 이하 버전에서는 rpmbuild 명령 대신 rpm 명령을 사용해야
한다는 점이다. -ba 옵션은 동일하다. 빌드된 RPM 패키지는 /usr/src/redhat/RPMS/

i386/likeU-0.0.1-l.i386.rpm 형태로 생성된다.
M mot@os：/usr/src/redhat/SPECS

........

Requires: libc.so.6 libc.so.6(GLIBC_2.0) libm.so.6 libm.so.6(GLI
BC_2.0)
퐈일 처리 중: likeU-debuginFo-0.8.1-1
Requires(rpmlib): rpmlib(CompressedFileHames) <= 3.0.4-1 rpmlib(
PayloadFilesHauePreFix) <= 4.0-1
Checking for unpackaged file(s): /usr/lib/rpn/check-Files /usr/t
mp/likeU-8.0.1

경 고: 호스트명을 정 규화(canonicalize) 할 수 없음: os
작성 : /usr/src/redhat/SRPMS/likeU—0.0.1-1 .src.rpm
작성 : /ust-/src/redhat/RPMS/i386/likeU-0.0.1-1 .i386 .rpm
작성 : Zusr/src/redhat/RPMS/i386/likeU-debuginFo-0.0.1-1 .i386.rpn
실행 중(玄clean): /bin/아 -e /uar/tmp/rpm-tmp.31897
+ umask 822
+ cd /usr/src/redhat/BUILD
+ cd likeU-8.0.1
+ rm -rF /usr/tmp/likeU-0.0.1
+ exit 8
rroot@os SPECS]tt Is /usr/src/redhat/RPMS/i386/
iikell-B.'s.l••••1 3M，nm] likeU-debuginFo-0.0.1-1 .i386.rpm
[rootSos SPECS]# “
[흐으으쁘또 SPECSjtt |______________________________________________________________

[그림 1-42] rpmbuild -ba likeU-0.0.1-1.spec 명령 후의 모습

빌드된 RPM 패키지를 rpm -Uvh likeU-0.0.1-l.i386.rpm 명령으로 설치하고, rpm

-qi likeU 명령으로 제대로 설치되었는지 검증한다.
-'■I root@os：/usr/src/redhat/RPMS/i^ffi
froo^s SPECSp cd .77RPbis/i386/ —
[root@os i386]tt Is
likeU 8.0.1- 1.1386.rpm likeU-debuginFo-0.0.1-1.i386.rpn
[rootQos i386] 1tl[root@os i386]#|rpra -Uuh likeU-8.8.1-1.i386
준비 증... I----------------------------------- --- ----------------- -1:likeU
rroot@os i3861»
[root@os i386]# like
Input nane : kara

=ial

I싀

[100%]

kara
[rootBos i386]lt|rpm -qi likeU
Name
likeU
Relocations:
/usr
Uersion
Uendor: (none)
0.0.1
Release
Build Date: 2807년 09월 29일 (토) 오
후 12시 36 분 28 초
Install Date: 2087년 09월 29일 (토) 오후 12시 39분 53초
Build Host: os
Group
: Utilities/Text
Source RPM: likeU-0.8.1-1.src.rpm
Size
: 3128
License: GPL
Signature
: (none)
URL
: http://woos.wowdns.coii/likelJ/
Summary
: I like you program
Description :
설명 : I like you 프로그램입니다. 소중한 사람에게 선물하세요. ：）
[rootSos i386]«
[root@os i386]#
[rootQos i386]tt
[rootBos

쓰!의흐!____________________________________ —

[그림 1—43] RPM 검증 화면

54 1 부—튜토리얼

시

===== PAGE 56 =====
정상적으로 설치되었다면 ［그림 1-43］ 과 같이 설치된 RPM 패키지의 정보를 볼 수 있다.

2장부터는 이제까지 사용한 각 개발 유틸리티의 기능과 구조, 원리를 심도 있게 파악하고
어떻게 활용하는지 알아보자.

1장_ 튜토리얼 55

===== PAGE 57 =====
I 2부 I 에디 팅

===== PAGE 58 =====
가와 vim 에디 터

01 vi 개괄
02 기본적인 vim 사용법 트레이닝
03 vim을 강력하게 하는 고급 테크닉
04 vim의 조력자 ctags, cscope, 기타 플러그인
05 개발자를 위한 vim의 유용한 팁
06 개발자들의 vim 설정

===== PAGE 59 =====
— Le+'s S+cidy 丄—

-------- ——

---------- —

유닉스 시스템에서 널리 시용되는 에디터로는 vi 와 emacs 를 들 수 있다. 어와 emacs 는
유닉스 시스템에서 에디터계의 양대 산맥으로 군림하고 있으며, 예전엔 두 에디터 사용
자 간에 마치 종교 전쟁이라도 하듯이 각 에디터의 장단점을 놓고 밤새 논쟁을 불러일으
키기도 했었다.
그만큼 두 에디터는 유닉스 시스템에서 독보적이고 많은 사용자 층을 보유하며, 또한
개성이 강하다. 2장에서는 유를 알아본다.
그럼 먼저 고리타분한 어의 역사를 알아보자. vi 는 역사를 가진 몇 안 되는 소프트웨어이
므로 규의 역사를 아는 것은 으 이해하는 데 도움이 된다.

===== PAGE 60 =====
01 Lvi 개괄
। 이의 역사
허는 BSD 의 씨셸 (C shell) 을 개발한 빌 조이가 1976 년에 ed 의 기능을 확장시킨

ex(EXtended editor) 편집기를 개발하고, 확장시켜 만들었다.
vi 이전에 사용되던 에디터로 ed와 ex라는 라인 에디터가 있는데, sed를 사용해 본 독
자라면 라인 에디터가 얼마나 불편한지 알 수 있을 것이다. ed나 ex 같은 라인 에디터
는 근대의 에디터와는 인터페이스가 많이 다르다. 라인 에디터는 마치 명령을 내리듯이
문서를 편집하므로 사용법이 복잡하고 다루기 힘든 편집기였다.
행 단위로 문서를 편집하던 시기에 마치 종이에 글을 쓰듯이 문서를 작성한다는 일은
매우 고무적이었을 것이다. 믿겨지지 않겠지만 그래서 vi가 Visual edit의 준말이다.
어는 기존의 에디터에 대한 새로운 인터페이스뿐만 아니라 에디터의 통합을 가지고 왔
다. vi 이전에는 각 벤더의 터미널마다 제어 코드가 각기 '달라 독립적인 에디터가 존재
할 수 없었다. 그러나 서로 다른 터미널의 특성을 제어하기 위한 termcap 데이터베이
스를 이용해 동일한 인터페이스로 제어를 할 수 있게 되었다. 세상의 많은 유닉스 시스
템에서 어를 표준으로 선택한 것은 당연한 일이었다. 물론 이 이야기는 1970년대의 호
랑이 담배 피던 시절 이야기다.

| 나의 장점
필자가 생각하는 아의 최대 장점은 바로 키보드로 모든 것이 가능하다는 점이다. 어를
사용하면 마우스를 만질 필요가 없다. 키보드로 모든 기능을 사용할 수 있기 때문에 일
에 집중할 수도 있고, 또한 매우 빠르게 일을 처리할 수도 있다.
어는 마우스가 없는 시대에 만들어졌기 때문에 현대에 나오는 어떤 에디터보다 독특한
인터페이스를 가지고 있다. 이런 독특한 인터페이스로 인해 하를 처음 접하는 사용자는
많은 불편함을 느끼곤 한다.
그러나 익숙해지면 어가 정말 강력한 에디터라는 것을 알 수 있다. 그래서 만들어진 지

30년이 넘은 에디터가 지금까지도 사랑받고 있는 것이다.

2장-vi와 vim 에디터

59

===== PAGE 61 =====
vi의 다른 장점으로는 가벼우면서도 매우 많은 기능을 내장한다는 데 있다. 아는 에디터
의 기본 기능에도 충실하면서 작업 효율을 높일 수 있는 매우 강력한 기능들을 많이 제
공한다. vi의 기능들은 너무 많아 한 번에 다 익히기 힘들다. 처음엔 기본 기능만 사용하
다가 나중에 아의 파워 유저가 되었을 때 마치 보물찾기 하듯이 숨어있는 기능들을 하
나씩 찾는 것은 작은 즐거움 중 하나다. 이런 즐거움으로 인해 어는 싫증나지 않는 에디
터다.

I 서른 살이 넘은 에디터, 그매력
파의 나이는 서른 살을 훌쩍 넘어간다. 다른 학문들과 비교하면 상대적으로 짧은 컴퓨
터 역사에서 볼 때 어는 분명 쥬라기 공원 시대의 공룡 소프트웨어임에 틀림이 없다. 모
든 소프트웨어는 생성과 소멸의 과정을 거치는데, 대부분의 소프트웨어들은 라이프 사
이클이 매우 짧다. 그러나 어는 유닉스보다 조금 늦게 나와서 유닉스의 발전과 함께 아
직까지 사용되고 있는 아주 진기 한 소프트웨 어 다.
인도네시아 동쪽 코모도 섬에 코모도 도마뱀이 서식하고 있는데, 코모도 도마뱀은 약 1억
년 전에 출현한 후 아직까지 별다른 진화의 과정을 거치지 않고 지금까지 살고 있다. 이
그모.두. 도마뱀의 주 무기는 바로 침인데, 침 속에는 치명적인 박테리아가 기생하고 있어
한 번 물리면 패혈증이 걸려 살아날 수 없다.
필자는 어를 볼 때 코모도 도마뱀을 연상하곤 한다. 1억년 전에 출연했지만 큰 진화의
과정을 거치지도 않았으면서 아직도 치명적인 무기를 가진 위력적인 존재로, vi와 코모
도 도마뱀이 여러모로 닮은 것 같다.

[그림 2-1] 구1쿠두 도마뱀

필자는 독자에게 어의 사용법을 알려줄 수 있지만 필자가 느끼는 어의 매력은 독자에게
강요할 수 없다고 생각한다.
어의 매력을 발견하는 것은 독자의 몫으로 돌리겠다. 부디 이번 장이 끝날 때쯤어의 매
력을 발견하기 바란다.
60 2부_ 에디팅

===== PAGE 62 =====
다음 절은 어를 아예 모르는 독자들을 위한 페이지다. 기본적인 입력, 편집, 이동, 저장
과 관련된 내용으로 구성되어 있다. 이미 기본적인 vi 사용법을 아는 독자라면 바로 고
급 테크닉으로 넘어가는 것이 좋을 것이다.
이 책에서 필자가 의도하는 바는 어를 이미 알고 있는 사용자에게 좀 더 고급 테크닉을
알려주는 것이다. 그래서 허의 기본 사용법은 다소 이 책의 의도와는 맞지 않다. 그러나
필자는 퍼를 처음 접하는 독자라도 이 책을 따라와 주었으면 하는 바람으로 기본 사용
법을 먼저 설명하고자 한다.

2 L 기본적인 vim 사용법 트레이닝
퍼를 자유자재로 다룰 수 있기를 원하는가? 그렇다면 반드시 각인해 둬야 될 말이 있다.
아래의 말을 반드시 기억해 두자.
“어는 배우는 것이 아니라 몸으로 익히는 것이다.”
어는 습관이다. 어의 많은 명령은 매우 단순하며 일관성이 있다. 먼저 그런 일관성을 파
악해야 되고, 일관성을 파악한 후에는 문서의 어떤 부분을 편집하려고 마음먹 었다면 머
릿속의 생각보다 빠르게 번개와 같은 손놀림으로 이미 편집하고 있을 때까지 부단히
사용해야 한다.
인터넷 게시판에서 글을 다 쓰고 습관적으로 어의 저장 명령인 瓦하（■:wq!를 눌러서 그
동안 작성한 내용이 전자 먼지로 사라져가는 것을 경험할 때쯤 되면 어가 얼마나 괜찮
은 에디터인지 알 수 있다. 그때까지 하는 단지 독특하지만 불편한 에디터일 뿐이다.
이번 장 역시 눈으로 보고 이해하는 장이 아니라 손으로 따라 하는 장이라는 점을 기억
하고 예제가 나오면 무조건 따라 해 보기 바란다. 다시 한 번 말하지만 너는 배우는 것
이 아니라 몸에 익히는 것이다.
어는 서른 살이 넘은 공룡시대 에디터인 만큼 오랜 진화의 과정을 거치면서 많은 클론
을 낳았는데, 앞으로 실습에서 사용할 vim이 바로 그것 이다. vim은 Vi Improved의 준
말로, vi의 기본 기능에 충실하면서 어에는 없는 여러 편리한 기능이 추가되 었다. 유닉
스 시스템은 벤더에 따라 어 또는 vim을 탑재한 시스템이 있는데, 리눅스에는 거의 vim
이 탑재되어 있다. 필자는 어보다 vim을 사용하라고 권하고 싶다. 전통적인 아보다는

2장_vi와 vim 에디터

61

===== PAGE 63 =====
vim이 인터페이스나 기능면에서 훨씬 월등하기 때문이다. 그러므로 앞으로 vim을 기
준으로 설명한다.

| vim의 모드 이해
vim을 이해하려면 먼저 vim의 여러 가지 모드를 이해해야 한다. vim에는 여섯 가지 기
본 모드와 다섯 가지 추가 모드가 있다. 이중 기본 모드에 포함되는 표준 모드, 입력 모
드, 명 령라인 모드만 이해하면 vim을 사용하는 데 전혀 지장이 없다.

n 표준 모드
표준 모드는 키 입력을 통해 vim에게 명령을 내리는 모드다. 표준 모드에서 커서를 이
동하거나, 삭제, 복사, 붙이기 등의 작업을 수행할 수 있다. 이 표준 모드 때문에 처음

vim을 접하는 대부분의 사람들은 생소함을 느낀다. vim을 실행하면 표준 모드부터 시
작하는데, 표준 모드에서는 아무리 타이핑해도 글자가 입력되지 않기 때문이다. 표준
모드는 vim에게 명령을 내리기 위한 모드지 편집을 위한 모드가 아니라는 점을 기억하
기 바란다.
@ 입력 모드
입력 모드는 실제로 문서를 편집하기 위한 모드다. 입력 모드에서 글자를 타이핑하면
실제로 화면에 출력되면서 글자의 입력이 가능하게 된다. 다시 한 번 강조한다. vim은
표준 모드와 입력 모드가 있는데, 표준 모드는 키 입력으로 삭제, 복사, 붙이기 등의
작업을 수행하는 모드고, 입력 모드가 실제로 문서를 타이핑해 편집하는 모드라는 점
을 기억하기 바란다. vim은 일반 에디터와 다르게 표준 모드와 입력 모드가 분리되어
있다. 이런 특징을 이해하지 못하고 접근하면 vim은 낯설고 이해하기 힘든 에디터가
된다.
@ 명령라인 모드
명령라인 모드는 명령 입력으로 여러 가지 일을 수행할 수 있는 모드다. 명령라인 모드
에서 수행할 수 있는 일에는 vim의 설정을 바꾸거나, 파일을 저장하고 읽거나, 특정 패
턴을 찾고 바꾸거나. 외부 명 령을 실행하거나, vim을 종료 하는 등과 같은 매우 다양한
일들이 있다.

62 2부_에디팅

===== PAGE 64 =====
［그림 2-2］ 모드 전환 관계

각 모드의 전환은 ［그림 2-2］ 와 같다. vim을 처음 실행시키면 표준 모드에서부터 시작
한다. 표준 모드에서 I, i, A, a, O, o, s 중 한 키를 누르면 편집이 가능한 입 력 모드로 전
환된다（나중에 다시 설명하겠지만 입력 모드 전환 키를 다 기억할 필요는 없다）.
입력 모드에서 복사, 붙이기 등과 같은 작업을 수행하려면 표준 모드로 다시 전환해야
한다. 입 력 모드에서 표준 모드로의 전환은 ［ Esc］ 키를 누르면 된다. ［그림 2-2］ 에서 보
는 바와 같이 입력 모드에서 명 령라인 모드로 바로 전환은 불가능하다. 일단 표준 모드
로 전환한 후 명령라인 모드로 전환해야 한다. 표준 모드에서 명령라인 모드로 전환하
려면 :, /, ? 키 중 한 키를 눌러 전환한다.
: 키는 vim 설정 명령이나 파일 관련 명령, ex 편집기 명령 등을 입력할 때 사용하고,
/ 키와 ? 키는 특정 패턴을 찾을 때 사용한다. / 키를 누른 후 찾으려는 패턴을 입력하
면 패턴이 나오는 곳으로 커서가 이동한다. / 키는 정방향 탐색을 할 때 이용하고, ?
키는 역방향 탐색을 할 때 이용한다.
어의 기본 모드에 대해 알았다면 이제는 에디터의 기본 기능을 알아보자. 에디터로서의
기본 기능에는 입력, 이동, 삭제, 복사, 붙이기, 찾기, 치환, 저장, 종료 등이 있다. 먼저
실행 방법과 저장, 종료를 알아보자.

I 파일 열기, 저장, 종료
$ vi hello.c

리눅스 셸 프롬프트상에서 위 명령을 내리면 vim이 실행된다. ‘$’는 셸 프롬프트를 의
미한다. 실행 시 hello.c 파일이 이미 존재한다면 hello.c 파일이 열리고, hello.c 파일
이 존재하지 않는다면 새로 생성한다.

2장_ 아와 vim 에디터

63

===== PAGE 65 =====
’ root@os：~

[그림 2-3] vi hello.c 명령 후 모습

명령을 내리면 ［그림 2-3］ 과 같이 다소 썰렁한 화면이 나타날 것이다. 하단에 “hello.c”
［새 파일］이라는 메시지도 보일 것이다.
파일명을 지정하지 않고 단순히 vim 명령만 입력했다면 ［그림 2-4］ 와 같은 화면이 나
타날 것이다.

빔 - 항상된 Ui
판 7.0.237
by Bram Moolenaar et al.
Modified by
빔은 소스가 얼려 있고 공짜로 배포됩니다
우간다에 사는 가난한 아이를 도와주세요?
이에 대한 정보를 보려면 :help iccF

입력

끝내려면
:q
온라인 도움말을 보려면 :help 또는 입력
type :help version?

입력
for uersion info

8.8-

1 모두 P|

［그림 2-41 vim 명령 후 모습

“우간다에 사는 가난한 아이를 도와주세요!”라고 표시되는 것은 vim이 charityware0］
기 때문이다. charityware란 무료로 사용할 수 있게 하는 대신 자선 단체 기부를 부탁
하는 소프트웨 어다.
지금부터 ［그림 2-3］ 을 예로 들어 설명한다. ［그림 2-3］ 과 같은 상태가 표준 모드 상태
다. 표준 모드에서는 I, i. A, a, O, o, s 키 중 하나를 눌러 입력 모드로 전환하지 않는 한
타이핑을 해도 아무런 글자도 써지지 않는다. i 키를 눌러 표준 모드에서 입력 모드로
전환해 보자.

64 2부_에디팅

===== PAGE 66 =====
입력 모드로 전환하면 비로소 문서를 작성할 수 있다. 필자는 ［그림 2-5］ 와 같이 “I like

you.”를 타이핑 했다.

［그림 2-5］ 입력 모드에서 텍스트 입력 후 저장

텍스트 입력이 끝나면 Esc］ 키를 눌러 입력 모드에서 표준 모드로 전환한다. 현재까지

hello.c 파일이 저장된 것은 아니다. heUo.c 파일에 저장하려면 % 키를 누르고 : 키
를 눌러 명령라인 모드로 전환해 ［그림 2-5］ 와 같이 w 명령을 입력하고 Enter］ 키를 누
른다.

vim 종료는 표준 모드에서 : 키를 눌러 일단 명령라인 모드로 전환하고 q 명령을 내리
면 종료한다（뜨 : q EnteH를 순차적으로 누르면 종료한다）. 일반적으로 자주 사용하
는 저장 후 종료는 명령라인 모드에서 다음과 같은 형식으로 사용한다.
: wq!

wq 명령은 저장 후 종료하라는 의미고, !는 강제 저장, 종료를 의미한다. 사용자가 자
신의 hello.c 파일을 수정 중이었는데, hello.c 파일의 퍼미션이 읽기 전용이었다면 저
장하려고 할 때 읽기 전용 파일이라는 경고 메시지가 뜨면서 저장할 수 없다. 그때는 !
를 붙여 강제 저장해야 한다.
마찬가지로 문서에 수정을 가했는데, 저장하지 않고 종료하려면 :q 명령 뒤에 !를 붙여
줘 야 저장하지 않고 종료할 수 있다.

2장_vi와 vim 에디터 65

===== PAGE 67 =====
［표 2-1］ 저장 및 종료

명령

설명

：w

저장

：w file.txt

file.txt 파일로 저장

：w〉〉file.txt

file.txt 파일에 덧붙여 저장

:q

vi 종료

ZZ

저장 후종료

:wq!

강제 저장 후 종료

：e file.txt

file.txt 파일을 불러옴

：e

현재 파일을 불러옴

［표 2-1］ 의 명령은 표준 모드에서 입력해야 되는 키 순서를 의미한다. 처음에 :을 입력
하면 표준 모드에서 명령라인 모드로 저절로 전환되므로 앞에 :이 붙은 명령은 모두 명
령라인 모드의 명령이다. 반면 ZZ와 같이 앞에 :이 붙지 않은 명령은 표준 모드 자체의
명령이다.
다 기억할 필요 없이 일단 처음 vim을 처음 시작하는 사람은 다음 명령만 반드시 기억
하기로 흐｝자.
• 저장: 上sc］ + ：w
• 저장 후 종료: .Esc| + ：wq!
• 저장하지 않고 종료: Esc］ + :⑴

• file .txt 를 불러옴: 'Esc］ + ：e file .txt

I 입력
입력은 입력 모드에서 가능하다. 표준 모드에서 입력 모드로 전환하려면 a, A, i, I, o, O,

S, cc 등의 키를 누른다. 독자들은 입력 모드 키가 너무 많은 것이 의아할 것이다. 각 키
에 대한 설명은 ［표 2-2］ 와 같다.
［표 2-2］ 입력 모드 전환 키

66

a

커서 위치 다음 칸부터 입력

A

커서 행의 맨 마지막부터 입력

i

커서의 위치에 입력

I

커서 행의 맨 앞에서부터 입력

0

커서의 다음 행에 입력

0

커서의 이전 행에 입력

s

커서 위치의 한 글자를 지우고 입력

cc

커서 위치의 한 행을 지우고 입력

2부— 에디팅

===== PAGE 68 =====
［표 2-2］ 는 대표적인 키를 나열한 것이고, 표에서 나열한 키 외에도 몇 가지 키가 더 있
다. 키 중 특히 많이 사용하는 키의 경우에는 음영으로 처리했다.
키들을 모두 외우고 쓸 필요는 없다. 물론 많이 알면 그만큼 더 편하겠지만 vim을 처음
시작하는 지금은 i(insert) 키만 기억하자. 안 그러면 앞으로 나올 수많은 키로 인해 꿈
속에서 키보드 괴물과 싸우게 될지도 모른다.
그■리고 믿기지 않겠지만 나중에 익숙해지면 저 많은 키를 모두 골고루 사용하게 될 것
이다.

I 이동
vim은 커서 이동과 관련해 매우 재미 있는 방식을 사용한다. 입 력 모드에서 이동은 일
반 편집기처럼 화살표 키를 사용한다. 표준 모드에서는 화살표 키로 이동할 수도 있고

h, j, k, 1 키를 이용할 수도 있다. h, j, k, 1 키는 표 2-31 과 같이 대응된다.
［표 2-3］ 표준 모드 이동 키

h
—

j

1

k

1

1

—*

처음엔 h, j, k, 1 키를 이용한 커서 이동이 어딘지 모르게 어색할 것이다. 그러나 h, j, k,

1 키에 익숙해지면 정말 괜찮은 키 매핑이라는 것을 알 수 있다. h, j, k, 1 키를 이용함으
로써 손이 키보드의 중심에서 벗어나지 않고 이동이 가능하기 때문이다.
표준 모드에서 단어 단위의 이동은 w 키와 b 키로 가능하다. w 키를 누르면 다음 단어
의 첫 글자로 이동하고, b 키를 누르면 이전 단어의 첫 글자로 이동한다.
같은 행 내에서 제일 처음 글자와 마지막 글자로 이동은 A 키와 $ 키를 사용한다. A 키
를 누르면 행의 제일 첫 글자로 이동하고, $ 키를 누르면 행의 제일 마지막 글자로 커서
가 이동한다.
+ 키와 - 키는 행을 변경할 때 사용한다. + 키는 다음 행의 첫 글자로 이동하고, - 키는
이전 행의 첫 글자로 이동한다. ( 키와 ) 키는 문장의 이동에 사용한다. vi에서 문장의
끝이란 마침표(.)가 나오는 지점을 의미한다. { 키와 } 키는 문단 단위의 이동에 사용한
다. 문단은 공백인 행을 기준으로 나눠진다.

2장_vi와 vim 에디터 67

===== PAGE 69 =====
우선 앞으로 실습에서 사용할 예제를 정하자. 예제는 리눅스 커널 소스로 하면 좋을 것
같다. 다음 주소에서 리눅스 커널 소스를 아무거나 받아오기 바란다.

• http://www.kernel.org
리눅스상에서 커널 소스를 받는 명령:

wget ［커널 소스 주소］
예) wget ftp://ftp.kern이.org/p니b/linux/kern이/v2.6/lirmx-2.6.29.tar.gz

다음 문서는 리눅스 커널 디렉토리에서 COPYING 파일을 연 것이다. 여러분도 다음
문서를 vim으로 열어 앞에서 설명한 이동 방법을 따라 해 보기 바란다.
헤 root@os：/te「np/test/너 m

|푸回

of this license document, but changing it is not allowed.
Preamble

： 문장 범우
.................

―The licenses for most"software are designed to take away your］
freedom to share and change it.| By contrast,'+66'—dHU' Gen；r；l Public
License is intended to guarantee your Freedom to share and change Free ■
software--to make sure the software is free for all its users. This
General Public License applies to most oF the Free Software
Foundation's software and to any other program whose authors commit to ■
using it. (Some other Free Software Foundation software is covered by H
the GNU Library General Public License instead.) Vou can apply it to |
your prograns, too.
： b.,

'''세

When we speak of Free soFtware, we are referring to Freedom, not
price. Our General Public Licenses are designed to make sure that you ■
have the Freedom to distribute copies oF free software (and charge For I
this seruice if you wish), that you receive source code or can get it
H
if you want it, that you can change the software or use pieces of it
M
in new Free programs; and that you know you can do these things. H
| To protect your rights, we need to nake restrictions that Forbid
44,1

6

어 P|

［그림 2-6］ vim에서 문장과 문단 범위

gg 키는 문서의 맨 처음으로 이동할 때 사용하고, G 키는 문서의 마지막 위치로 이동할
때 사용한다.
지금까지 자주 사용하는 커서 이동 키를 설명했다. 모든 커서 이동과 화면 이동에 관련
된 키는 ［표 2-4］ 와 같다.

68 2부_에디팅

===== PAGE 70 =====
［표 2-4］ 표준 모드 이동 키 종합 （ ［ n］ 은 임의의 번호를 의미）
h

왼쪽으로 이동

1

오른쪽으로 이동

j

아래 행으로 이동

k

위 행으로 이동

w or W

다음 단어의 첫 글자로 이동

b or B

이전 단어의 첫 글자로 이동

e or E

단어의 마지막 글자로 이동

Enter

다음 행의 첫 글자로 이동

현재 행의 첫 글자로 이동

$

현재 행의 마지막 글자로 이동

+

다음 행의 첫 글자로 이동

-

위 행의 첫 글자로 이동

(

이전 문장의 첫 글자로 이동

)

다음 문장의 첫 글자로 이동

{

이전 문단으로 이동

}

다음 문단으로 이동

H

커서를 화면의 맨 위로 이동

zEnter]

현재 행을 화면의 맨 위로 이동

M

커서를 화면의 중앙으로 이동

z.

현재 행을 화면의 중앙으로 이동

L

커서를 화면 최하단으로 이동

z-

현재 행을 화면의 최하단으로 이동

[n]H

커서를 위에서 n번째 행으로 이동

[n]L

커서를 아래에서 n번째 행으로 이동

라-니

반 화면 위로 스크롤

C레—d

반 화면 아래로 스크롤

jCtrl]-b

한 화면 위로 스크롤

Ctrl]-f

한 화면 위로 스크롤

gg, IG

문서의 맨 첫 행으로 이동

G

문서의 맨 마지막 행으로 이동

[n]G

n번째 행으로 이동

：[n]

n번째 행으로 이동

A

굉장히 많은 키로 인해 기가 질릴지도 모로겠다. 하지만 역시 다 익힐 필요는 없다. 사
실 위에 나오는 키를 하나도 사용하지 않고 단지 화살표 키만 사용할 수도 있다. 물론
그렇게 사용한다면 vim이 정말로 싫어질 것이다. 지금은 h, j, k, 1 키와 단어 단위의 이
동 키인 짜와 b, 문단 단위의 이동 키인 {와 }, 라인의 시작과 끝으로 이동하는 A와 $, 특
정한 행으로 이동하는 ：［ n］ , 문서의 시작과 끝으로 이동하는 gg와 G 정도만 기억하자.
그리고 나머지는 이 책의 부록 부분에 있는 vim 명령 요약을 컴퓨터 옆에 붙여놓고 필
요할 때 하나씩 익히면 된다.
• 한 글자씩 이동: h, j, k, 1
• 단어 단위 이동: w, b
• 문단 단위 이동: I}
• 라인의 시작과 끝: A, $

• n번째 행으로 이동: ：［ n］

（ ［ n］ 은 임의의 번호）

• 문서의 시작과 끝: gg,G

2장_vi와 vim 에디터 69

===== PAGE 71 =====
I 편집
n 삭제
표준 모드에서 X를 누르면 현재 커서 위치의 한 글자를 삭제한다. dw는 커서 위치의
한 단어를 삭제하고, dd는 한 행을 삭제한다.
어의 명 령에는 규칙이 하나 있는데, 명령 앞에 숫자를 넣으면 그 명 령 앞에 누른 숫자만
큼 반복한다는 의미가 있다. 그래서 10x를 누르면 현재의 커서부터 10개의 글자가 삭
제된다. 마찬가지로 10dw를 누르면 10개의 단어가, 10dd를 누르면 10행이 삭제된다.
懇 •:scieen I： bash】 n>ci@《J3：/i€'S丁W 우 HOW히
The Road Not Taken

JR [screen I： bash] r0ct@as：/Ter
The Hoad Not Taken

jjwo = diverged in o yellow wood, I
And surry I could not travel both
And be one traveller, lang I stood H
And looked down one as F.)r as I could ■
To INwre it bent in the undergrouth; B

Bo Where it bent tn the ijnriergrouth;

■

모두 |리

"tPSt .txt" 91, a,i

h 보다 식은 술

［그림 2-7］ 4dd 명령 화면

주로 많이 사용하는 삭제 명령은 위에서 설명한 X, dw, dd 정도가 있고, 기타 삭제와
관련된 다른 방법은 ［표 2-5］ 와 같다.
［표 2-5］ 삭제와 관련된 키
X,

에

커서 위치의 글자 삭제

X, dh

커서 바로 앞의 글자 삭제

dw

한단어를 삭제

d0

커서 위치부터 행의 처음까지 삭제

D. d$

커서 위치부터 행의 끝까지 삭제

dd

커서가 있는 행을 삭제

dj

커서가 있는 행과 그 다음 행을 삭제

dk

커서가 있는 행과 그 앞 행을 삭제

@ 복사와 붙이기
『는 현재 커서 위치의 한 단어를 복사한다. yy는 현재 커서 위치의 한 행을 복사한다.
이렇게 복사한 문자들은 P로 붙여넣을 수 있다. 위의 삭제에서 설명한 아의 명령 규칙
대로 10yw는 현재 커서 위치에서 10개의 단어를 복사하고, 10yy는 10개의 행을 복사
한다. 마찬가지로 2P는 복사한 내용을 2번 붙여넣는다.

70 2부—에디팅

===== PAGE 72 =====
빼 [screen I: bash] root®os：/t?mp/tes?

| 【?cieen ?： bashi rnotsgo^./temp/test
石;nS?FT&i«‘'n...

|ihe Road Not raiten
[Juo roads di verged in a yellaw Mind,
And sorry I could not travel both
And h? one travel l?i-, long I stood
Andi looked doim one as far as I could
To Where it bent in the undergrouth;

Two roads diverged in a yelloir wood,
And sorry I could not travel both
I be one traveller, long I stood
looked down one as Fair as I con)
Where it bent in the undergrouth:
roads diuerged in a yellow uood.
sarru I could not travel both

고구

I"test.txt" 9L., 2H3C ：l,1

［그림 2-8］ 2yy로 두 행을 복사한 후 p로 붙여넣은 화면

@ 잘라내기
잘라내기를 이해하려면 먼저 아의 레지스터에 대해 알아야 한다. vi는 총 17개의 레지스
터를 가지고 있는데, 일단 dd 명령으로 한 행을 지웠다면 화면에서 지워짐과 동시에 그
내용은 “1 레지스터에 들어간다. 그리고 다시 dd 명령으로 한 행을 지우면 “1 레지스터
에 들어 있던 내용은 “2 레지스터로 옮겨가고 “1 레지스터에 새로 지운 내용이 들어간다.
aaa를 지웠을 때
“2

“1

“3

“4

“5

“3

“4

“5

“2

“3

“4

“5

bbb

aaa

. “6

“7

“8

“9

“6

“7

“8

“9

“6

“7

“8

“9

aaa
bbb를 지웠을 때
“1

“2

bbb

aaa

ccc를 지웠을 때
“1
CCC

［그림 2-9］ 레지스터에 들어가는 형식

이런 레지스터는 명 령라인 모드에서 :reg 명령으로 볼 수 있다. ［그림 2-9］ 는 레지스터
의 이름을 나타낸 것이고, ［그림 2-1 이은 ：reg 명령으로 레지스터의 내용을 본 것이다.
«■’

“0

“1

“2

“3

“4

“5

“6

“7

“8

“9

“

“%

“#

‘7

［그림 2-10］ 레지스터 버퍼

“” 레지스터는 바로 이전에 지워진 내용이 항상 들어간다. “1부터 “9까지 레지스터는 지
워지는 내용이 큐 형식으로 들어간다.

“1부터 “9 외에 나머지 레지스터는 특수한 목적이 있다. 레지스터에는 최근까지 타이
핑한 내용이 들어간다. 그래서 ［그림 2-11］ 에서 알 수 있는 것은 필자가 최근에 “ABC”
를 타이핑했다는 것이다. “% 레지스터 버퍼에는 현재 편집하는 파일명이 들어간다. 그
리고 마지 막으로 7 레지스터에는 가장 최근에 검색한 문자열이 들어간다.
2장_vi와 vim 에디터 71

===== PAGE 73 =====
R (screen 1： bash] root^as:/temp/test
using il. (Sorw other Free SoFtuare Futmddlimi software is tuuered by
the RMI Library general. Public License instead.) Vmi can apply it to

- [헌호/꾸서

reg

__，체히.人妄- ■…■' •
'•

59 Tenple Place, Suite 338, Boston, Mfi »?111-1387

o create_process<(unsigned long)task2)：
1
59 Tenple Place, Suite 33B. Boston, IM 02111-1307
2 Copyright (R) 19H9, 1991 Free Software Foundation, Inc.
Uersion 2, June 1991
fttW GFHCRftl PlIBI IC LICENSF

Linus Torvalds

［그림 2-11］ ：reg 명령으로 살펴본 레지스터의 내용

바로 이전에 지워서 레지스터에 들어가 있는 내용은 p 명령으로 붙여넣을 수 있다. 복
사 역시 마찬가지다. yy를 눌러 한 행을 복사했다면 그 내용은 일단 레지스터에 들어간
다. 그리고 p 명령으로 레지스터에 있는 내용을 다시 출력할 수 있다. 그래서 너에서 잘
라내기란 일단 dw나 dd로 지우고 p 명 령으로 붙여넣으면 된다.

P 명령으로 붙여넣을 때 특정 레지스터를 선택할 수 있다. “2p하면 2번 레지스터에 있
는 내용이 붙여넣어진다. 이전에 지우긴 했는데 그 내용이 어떤 레지스터에 있는지 모
르겠다면 명령라인 모드에서 :reg 명령을 입력해 확인할 수 있고, 또 다른 방법으로는

“Ipu.u.u. 명령으로 각 레지스터에 있는 내용을 하나씩 되돌리면서 붙여넣을 것을 선택
할 수 있다. “Ip는 1번 레지스터의 내용을 붙여넣는 명령이고, u는 되돌리기 명령이다.
그리고 .은 바로 이전에 했던 작업을 반복하는 명령이다.

Q 블록 지정
지금까지 여러 단어 혹은 여러 행을 지우거나 복사하기 위해 명령 앞에 숫자를 붙여주
었다. 예를 들면 5개의 단어를 지우려면 5dw를 사용했고, 5행을 복사하려면 5yy를 사
용했다. 그러나 여러 단어나 행을 지우거나 복사하려고 일일이 단어의 개수나 행 개수
를 세기는 매우 귀찮은 일이다. 그럴 때는 블록을 지정해 직접 개수를 세지 않고도 쉽
게 원하는 작업을 수행할 수 있다.
［그림 2-12］ 와 같이 원하는 위치에서 v 키를 누르고 j 키로 커서를 아래로 이동시키면
역상으로 블록이 형성되는 것을 볼 수 있다. 일단 원하는 범위만큼 블록을 지정했다면
지우고 싶을 경우에는 d를 누른다. 또한 지정된 블록을 복사하고 싶을 경우 y를 누르면
지정된 블록에 대한 복사가 일어난다.

72 2부_에디팅

===== PAGE 74 =====
Frr

H root@os：/temp/test
First Loue
Though nurtured like the sailing noon
in beauty's murderous brood,
She walked awhile and blushed awhile
And on my pathway stood
]ntil I thought her body bore
I heart of Flesh and blood.

모두

7,1

-- 비주얼 --

너

[그림 2-12] 블록 지정 모습 1

다음과 같은 문자열이 있어 Uid 부분만 지우고자 한다면 일반 블록 지정으로는 지우기
가 힘들다. 이때는 %J+v 키를 사용한다. £trl] 키를 누른 상태에서 v 키를 누르면 커서
의 위치를 기점으로 사각형의 블록을 형성할 수 있다. 원하는 만큼 지정한 후 삭제(d),
복사(y)를 하면 된다.
® ro ot@ o s ：/te mp/test
priuoxy
pum
desktop
radud
choijm
sepj20
zsjung x

uid
73
24
80
75
502
5 03

pass
x
x
x
x
x
x

504

8,13—24

" 비주얼 구역 -

모두

[그림 2-13] 블록 지정 모습 2

[표 2-6] 블록 지정 후 사용 가능한 키

대소문자 전환

d

삭제

y

복사

C

치환

)

라인 앞에 탭 삽입

<

라인 앞에 탭 제거

선택된 영역에 대해 ex 명령

J

행을 합침

대문자로 만듦

U

소문자로 만듦

U

2장_vi와 vim 에디터

===== PAGE 75 =====
I 되돌리기와 되살리기
되돌리기와 되살리기 기능이 vim에 없었다면 vim은 정말 정신 건강에 해로운 에디터
였을 것이다. 혹은 있더라도 기능을 사용할 줄 모른다면 정신 건강을 해치기는 마찬가
지다. vim에서 되돌리기 기능은 u 명령을 사용한다. 그리고 되살리기는 Ctrt］ +r 키를 이
용한다. 원래 u 명령의 의미는 되돌리기가 아니라 명령 취소의 의미다. 그러나 결국 되
돌리기가 되는 것은 사실이기 때문에 되돌리기 기능이라고 말하곤 한다.

I 문자열 탐색
vim에서 특정한 문자열을 찾는 방법은 매우 쉽다. 그냥 단순히 한 문자열만 찾으려면
다음과 같이 표준 모드에서 / 키（역방향 탐색은 ? 키）를 누른 후 찾기 원하는 문자열을
입 력하기만 하면 된다.
/［찾고자하는문자열］ 또는 ?［찾고자하는문자열］

다음 예는 커 널 소스 디 렉토리의 COPYING 파일을 열어 “to”라는 문자열을 탐색한 예다.
B root@os：/temp/tesVvim

즈

司픠

EH

price. Our General Public Licenses are designed t聽 make sure'that you
haue the Freedom 호 distribute copies oF free software (and charge for
this service if you wish), that you receiue source code or can get it
if you want it, that you can change the software or use pieces of it
in new Free programs; and that 으ou know i^ou can do these things.
To protect your rights, we need (E_nake restrictions that Forbid
anyone |히 deny you these rights or 기hl ask you QQ surrender the rights.
These restrictions translate |히 certain responsibilities for you if you
distribute copies of the software, or iF you modify it.
For example, if you distribute copies oF such a program, whether
gratis or For a fee, you must giue the recipients all the rights that
you haue. Vou must make sure that they, Q0o, receiue or can get the
source code. And you must show them these terms so they know their
rights.
We protect your rights with two steps: (1) copyright the software, and
(2) oFFer 90U this license which giues you legal permission ［物 copy,
distribute and/or modify the software.

/to

38,50

11X

희

【그림 2-14］ 문자열 탐색 모습

위 화면에서 n 키를 누르면 커서가 다음에 매칭되는 “to” 문자열로 이동하고, 대문자

N 키를 누르면 이전에 매칭한 “to” 문자열로 이동한다.
간단한 문자열의 경우 위와 같은 /, ?를 사용한 명령 형식으로 찾을 수 있다. 그러나 좀
더 복잡한 문자열의 경우 고급 테크닉에서 배울 정규 표현식을 사용해야 한다.

74 2부_에디팅

===== PAGE 76 =====
I 문자열 치환
문자열 치환 역시 매우 쉽다. 명령라인 모드에서 다음 명령을 내리면 문서에 있는 모든

old 문자열을 new로 바꾼다.
:%s/old/new/g

띤

g)foot@os：/temp/i0t ME

old Friends and old wine are best.
old friends and old wine are best. ■
old friends and old wine are best.

Friends and nfFTI wine are best.
friends
and new wine are best,
friends
and new wine are bpst.

old friends and old wine are best.

friends

and

new wine are best.

old friends and old wine are best.

friends

and

new wine are best.

모干

:%5/old/new/g|

［그림 2-15］ 치환 전과 치환 후

위 명령은 슬래시 (/)를 구분자로 총 4개의 부분으로 나눠져 있는데, 다음과 같다.
: ［범위］ / 매칭 문자열］ / ［치환 문자열］ / ［행 범위］

먼저 범위는 매칭 문자를 치환할 문서상의 범위를 의미한다. 96s는 문서 전체를 의미한
다. 그래서 :%s/old/new/g 를 하면 문서 전체에 있는 old 문자열이 new 문자열로 치
환된다. 아래 예제들은 범위 지정의 예다.
문서 전체에서 제일 처음 매칭되는 라인의 문자열만 치환한다.
:s/old/new/g
M raGt@05：/ternp/test
UJld
friends
old
Friends
old
Friends
old
friends
old Friends

and old
and old
and old
and old
and old

wine
vine
wine
uine
wine

are
are
are
are
are

nest.
best.

<175C 저장 했급니디

［그림 2-16］ 치환 전과 치환 후

2행에서 4행 사이에 매칭되는 문자열을 치환한다.
:2Z 4s/old/new/g

2장_vi와 vim 에디터 75

===== PAGE 77 =====
SJid friends and old
iltl friends
and
ild Frientls
ami
ild friends
and
ild friends
and

old
old
old
old

wine
wine
wine
wine
wine

<175C 7규장 했습

[그림 2-17] 치환 전과 치환 후

현재 커서의 위치에서 위로 1 행, 아래로 3행의 범위에 매칭되는 문자열을 치환한다.
:-1,+3s/old/new/g
H '0=?〕: '-0 T -0 ：.•
old friends anil old wine are h?st.
old Friends and old wine are best.
허.d friends and old wine are best.
old Friends and old wine are best.
old Friends and old wine are bestoJd Friends and old wine are bestold Friends and olrt wine are bpst.

3,1

W司 I 호

쁘gocWas■:.4’：‘--|?..丄：’：1

Ftie nils and W3 uinp are best.
_±」 old| TFT?

醫W x|

nds and new wine ar휴 best Frie nds and new wine are best,
Frie nds and new wine are best,
frie nds and new wine are best,
Frie nds and BPM wine are be5t.
15g『TFT；

모두

r

른

[그림 2너8] 치환 전과 치환 후

치환 문자열은 매칭 문자열을 만났을 때 치환할 문자열을 의미하고, 행 범위는 치환될
행의 범위를 의미한다. g는 행 전체에 걸쳐 치환하라는 의미고, 행 범위에 g를 쓰지 않고
명령을 내리면 한 행에서 여러 개의 매칭 문자열이 있더라도 한 번만 치환이 일어난다.
:%s/old/new/

해 rogt@0S：,Aemp/test
tjld friends and old wine
old friends and
old
old Friends
and old
old friends
and old
old Friends
and old
old friends
and old
and old
old friends

wine
wine
wine
wine
wine
wine

[그림 2-19] 치환 전과 치환 후

행 범위에 다음과 같이 e를 지정하면 매칭되는 문자열에 대해 치환할 것인지 사용자에
게 물어본다.
:응s/old/new/gc

76 2부—에디팅

===== PAGE 78 =====
® root@os：/temp/test
old friends
and
and
Old friends
and
old friends
and
old friends
and
old friends
and
old friends
and
old Friends

wine are best,
wine are best,
wine are best,
wine are best,
wine are best.
wine are best,
wine are best.

버［ 꿈 (y/n/a/q/：LrE/『?) 1,1

모두

［그림 2-20］ 치환 명령 질의

특정한 패턴이 있는 행만 치환하게 하려면 다음과 같은 형식으로 사용한다.
: ［범위］ /［패턴］ /［매칭 문자열］ /［치환 문자열］ /［행 범위］

위 명령은 매칭 문자에 대한 치환을 조절할 수 있으므로 유용하다. 예를 들어 아래
와 같은 셸 스크립트가 있을 때 주석 부분은 손대지 않고 실제 스크립트 명령 부분
만 TEST 변수를 STR 변수로 전부 바꾸려 할 경우 이전에 배운 내용에 따르면 주석의

TEST도 치환된다.
〔예제 2너〕 테스트용 셸 스크립트 내용

#!/bin/sh
#######################
# TEST SHELL SCRIPT
#######################
TEST="foobar"
echo $TEST

그러나 다음처럼 명령을 내리면 주석 부분은 건드리지 않고 변수명을 바꿀 수 있다.
:g/\(A［얘］.*TEST\|ATEST\)/s/TEST/STR/g

［그림 2-21］ 치환 전과 치환 후

\(T#］ .*TEST\|ATEST\)의 의미는 나중에 배우게 될 정규 표현식에서 나오는데, 지금
당장은 #으로 시작하지 않는 TEST 문자열과 TEST로 시작하는 문자열이라는 의미만
알아 두기 바란다.

2장_vi와 vim 에디터 77

===== PAGE 79 =====
그래서 명령을 내리면 #으로 시작하는 주석에 있는 TEST는 문자열 치환이 되지 않고
실제 셸 스크립트의 소스 부분만 치환이 일어난 것을 확인할 수 있다.
이런 치환 명 령을 요약 정리해 보면 ［표 2-刀과 같다.
［표 2-7］ 치환 명령 요약
：s/old/new

현재 행의 처음 이d를 new로 교체

:s/old/new/g

현재 행의 모든 old를 new로 교체

：10,20s/old/new/g

10번째 행부터 20번째 행까지 모든 old를 new로 교체

：-3,+4s/old/new/g

현재 커서 위치에서 3행 위부터 4행 아래까지 old를 new로 교체

：%s/이 d/new/g

문서 전체에서 이d를 new로 교체

：%s/이 d/new/gc

문서 전체에서 이d를 new로 확인하며 교체

:g/pattern/s/이 d/new/g

patternOl 있는 모든 행의 old를 new로 교체

：g/pattern/s//new/g

：%s/old/new/g 와 동일

3 vim을 강력하게 하는 고급 테크닉
지금까지는 정말 편집기로서의 기본적인 기능만을 설명했다. 지금까지의 내용만으로는

vim이 다른 편집기에 비해 많이 다르다는 것은 알 수 있었지만, 어째서 vim이 다른 편
집기와 비교해 강력한지는 알 수 없었을 것이다. 사실 앞으로 설명하는 내용이 여러분
에게 알려주려는 것이고, 이 책의 목적이다.

I 정규 표현식을 사용한 문자열 탐색과 치환
vim에서 특정한 패턴의 문자열을 찾고 치환하는 작업은 매우 설레고 즐거운 일이다. vi
는 정규 표현식을 지원하기 때문이다. vi뿐만 아니라 grep과 같은 패턴 매칭을 이용하
는 대부분의 유닉스 프로그램은 정규 표현식을 지원한다.
정규 표현식의 정의를 내리자면 정규 표현식은 기호나 문자를 사용해 문자열을 표현하
는 방식이다. 먼저 표 2-8］ 을 기준으로 예를 들어 알아보자.

78 2부_ 에디팅

===== PAGE 80 =====
[표 2-8] vim 정규 표현식

A

행의 첫 문자（□ 안에서는 not의 의미）

$

행의 끝

아무 문자나 한 문자 의미

\1

or의 의미

[]

[] 사이의 문자 중 하나

\{min,max\}

min 이상 max 이하 반복됨

*

앞의 내용이 0번 이상 반복됨

\+

앞의 내용이 1번 이상 반복됨

\<

단어의 시작

\>

단어의 끝

\n

new line 문자

\t

tab 문자

[표 2-8] 의 내용은 vim에서 지원하는 정규 표현식이다. “like”나 “korea” 같은 소문자
로 이뤄진 모든 문자열을 표현하고 싶다고 하자. 그냥 말로 풀어 표현하면 “소문자로
이루어진 문자열”일 것이다. 그러나 이렇게 자연어로 표현하는 방법은 컴퓨터가 인식하
는 데 있어 별로 유용하지 못하다.
컴퓨터는 인간의 언어를 모르고, 또한 각 나라마다 자연어가 서로 다르기 때문이다. 그
리고 자연어는 정형화되어 있지 않고 여러 말로 표현 가능하다. 예를 들면 “알파벳 소
문자로 이루어져 있는 문자열” 또는 “소문자로만 구성되어 있는 문자열”과 같이 여러
가지 다른 말로 표현이 가능하다.
이런 모호성 때문에 0과 1밖에 모르는 컴퓨터에 있어 자연어는 활용하기 어렵다. 그래
서 문자열을 표현하는 새로운 방식이 필요하게 되었는데, 정규 표현식이 그 해답을 제
시한다.
“소문자로 이루어진 문자열”을 위에 있는 하에서 사용하는 정규 표현식대로 표현해 보
면 다음과 같다.
[a-z]\+

이런 정규 표현식은 탐색이나 치환에서 그대로 이용할 수 있다. 다음은 탐색의 예다.

2장_vi와 vim 에디터

79

===== PAGE 81 =====
[그림 2-22] /[a-z]\+ 명령으로 탐색한 예

대괄호([])는 대괄호 내에 있는 한 글자를 의미한다. 그래서 [a-z]의 의미는 a부터 z까
지 한 글자를 의미하고, 뒤에 \+가 붙어서 a부터 그까지의 한 글자가 한 번 이상 반복되
는 것을 의미한다. 뒤에 \+ 대신 * 기호가 붙으면 0번 이상 반복을 의미한다. 그러므로
위 정규 표현식에 해당되는 문자열은 “like”, “korea”와 같이 소문자로만 이뤄진 문자열
이다.
소문자 문자열이 앞에 오고 뒤에 숫자가 있는 “likeOlOl”, “korealll7”과 같은 문자열
을 정규 표현식으로 표현한다면 다음과 같이 할 수 있다.
[a-z]\+[0-9]\+ 또는 [a-z]\+[0123456789]\+

[그림 2-23] /[a—z]\+[0-9]\+ 명령으로 탐색한 예

80 2부—에디팅

===== PAGE 82 =====
a부터 그까지의 글자가 한 번 이상 반복되고 0부터 9까지의 문자가 한 번 이상 반복되는
문자열이 바로 “likeOlOl”, “korealll7”과 같은 문자열를 의미 한다.

“OK like”, “OK korealll?”과 같이 앞부분에 “OK”, 뒤에 소문자 단어, 그리고 그 뒤에
숫자가 올 수도 있고 오지 않을 수도 있는 비교적 복잡한 문자열도 다음과 같이 간단하
게 표현할 수 있다.
0K\ [a-z]\+[0-9]*

“OK” 문자 뒤에 오는 공백은 앞에 \를 붙여줘야 정상적인 공백으로 인식한다. 공백 문
자가 구분의 의미를 지닌 메타 캐릭터이기 때문에 역슬래시를 붙이지 않으면 메타 캐
릭터로 인식한다. 다른 예로 ‘.’과 같이 정규 표현식 내에서 의미를 지니는 문자도 자
체를 표현하려면 ‘V과 같이 역슬래시를 붙여 ‘.’의 의미를 없애줘야 한다.

[그림 2-24] /0K\ [a-z]\+[0-9]* 명령으로 탐색한 예

어의 정규 표현식으로 위 정규 표현식을 풀어보면 “OK” 문자열이 앞에 오고 a부터 z 중
한 글자가 한 번 이상 반복되고 0부터 9 사이 문자가 0번 이상 반복된다는 의미다.
정규 표현식에서 A 기호의 의미는 행의 시작을 의미한다. 행의 처음이 숫자로 시작되는
문자열을 표현하려면 정규 표현식으로 다음과 같이 표현할 수 있다.
A[0-9]\+.*

‘.’의 의미는 개행 문자 ‘\n’을 제외한 모든 문자를 의미한다. 그래서 위의 정규 표현식
에 해당하는 문자열은 다음과 같은 것들이다.

2장_vi와 vim 에디터 81

===== PAGE 83 =====
[그림 2-25] /A[0-9]\+* 명령으로 탐색한 예

기호가 대괄호([]) 내에서 사용된다면 not의 의미를 지닌다.
A[A0-9]\+.*

[그림 2-26] /午。9]\+.* 명령으로 탐색한 예

앞에서 나온 정규 표현식과 반대로 위 정규 표현식은 대괄호 내에 A 기호가 있어 숫자
로 시작하지 않는 문자열을 표현한다.
A

기호가 행의 시작을 의미한다면 $ 기호는 행의 끝을 의미한다. 그래서 다음 정규 표현

식은 숫자로 끝나는 문자열을 의미한다.
.*[0-9]$

82 2부_에디팅

===== PAGE 84 =====
[그림 2-27] /.*[0-9]$ 명령으로 탐색한 예

\< 기호와 \〉기호는 단어의 시작과 끝을 의미한다. 가령 “ko”로 시작되는 단어를 표현
하고자 할 때 다음과 같이 표현할 수 있다.
\<ko
B root@os:/temp/test
What Though Life Conspire To Cheat Vou
What thought life conspire to cheat you.
Do not sorrow or complain.
Lie still on the day of pain,
And the day of joy will greet 少ou.
Hearts liue in the coming day.
There's an end to passing sorrow.
Suddenly all Files away,
And delight returns tomorrow.
JErea 扇real117 扇komo Korea
like likeOIOI
012korea
11 abc

OK like
OK U)rea1117
/!#<ko

22,4

모두 p|

[그림 2-28] /\<ko 명령으로 탐색한 예

위 정규 표현식은 “korea”, “kokomo”와 같은 단어의 “ko” 부분을 의미한다. 마찬가지
로 ea\〉는 “korea” 같은 문자열의 ea 부분을 표현한다.

\{min1max\} 기호의 의미는 min번 이상 max번 이하로 반복된다는 의미다. 영문자로 시작
하고 3자리에서 4자리 숫자로 끝나는 문자열을 표현하려면 다음과 같이 나타낼 수 있다.

2장_vi와 vim 에디터 83

===== PAGE 85 =====
[A-z]\+[0-9]\{3,4\}

[그림 2-29] /[A—z]\+[0-9]\{3,4\} 명령으로 탐색한 예

위의 정규 표현식으로는 koreal2와 같이 두 자리 숫자로 끝나는 문자열은 포함되지
않는다. 반드시 koreal23과 같이 3자리 에서 4자리로 끝나는 숫자가 있어 야 하기 때문
이다.

\1 기호는 or의 의미를 지니고 있다. Korea나 korea와 같이 앞부분에 대소문자 구분을
하지 않고 korea를 표현하려 면 다음과 같이 할 수 있다.
\(K\|k\)orea
H root@os:/temp/test
What Though Life Conspire To Cheat Vou
What thought life conspire to cheat 브ou.
Do not sorrow or complain.
Lie still on the day oF pain,
And the day of joy will greet 90U.
Hearts liue in the coming day.
There's an end to passing sorrow.
Suddenly all Files away.
And delight returns tomorrow.
MKB 1333히1117 "komo msr
like like0181
B12 므WB
11 abc
3
OK like
OK H3JEE1117
/tfCKtf|ktt)orea

[그림 2-30] A(K\|k\)orea 명령으로 탐색한 예

84 2부—에디팅

13,24

모두 리

===== PAGE 86 =====
그럼 개행 문자(\n) 나 탭 문자(\t) 를 표현하고 싶을 때는 어떻게 하면 될까? 개행 문자
는 ‘\n’으로 표현하고, 탭은 ‘\f 로 표현 가능하다. ‘\n’과 ‘\f 같은 표현법은 vim에만 있
는 확장 정규 표현식이다. 확장 정규 표현식은 뒤에 다룬다.
정규 표현식 내에 vim은 POSIX 문자 클래스를 지원하는데, 이런 문자 클래스를 이용
하면 정규 표현식에서 사용하기 힘든 제어 문자들을 쉽게 사용할 수 있다. 다음 표는

POSIX 문자 클래스를 보여준다.
[표 2-9] POSIX 문자 클래스
문자 클래스

내용

[:alnum：]

알파벳과 숫자 [A-Za-zO-9]

[:alpha：]

알파벳 [A-Za-z]

[:cntrl:]

제어 문자

[:blank：]

탭과 공백 문자

[:digit:]

숫자 [0-9]

[：graph：]

제어 문자와 공백 문자를 제외한 문자

[:lower：]

소문자 [a-z]

[：upper：]

대문자 [A-Z]

[:print：]

제어 문자를 제외한 문자. 즉, 프린트할 수 있는 문자

[:punct：]

[:graph:] 문자 중 [:alnum：｝ 을 제외한 문자. ex)!,@,#,$,%,A-

[:space：]

화이트 스페이스 예: 공백, 탭, 캐리지 리턴, 개행 문자, 수직 탭, 폼 피드

[：xdigit:]

16 진수

이런 문자 클래스를 이용해 “소문자로 이루어져 있는 문자열”을 정규 표현식으로 표현
하면 다음과 같다.
[[:lower:]]\+

[그림 2-31] /[[：lower：]]\+ 명령으로 탐색한 예
2장_vi와 vim 에디터 85

===== PAGE 87 =====
vim 내에서 POSK 문자 클래스를 사용할 때는 위와 같이 대괄호를 두 개 사용해야 한
다. 이런 문자 클래스는 모든 화이트스페이스를 한 번에 표현하는 것이 가능하기 때문
에 자주 사용되곤 한다. 예를 들면 “int var；”와 같은 변수의 선언 부분을 POSK 문자
클래스를 사용하지 않고 정규 표현식으로 표현하려면 다음과 같이 해야 한다.
int\(\ \|\t\|\n)\+var;

그러나 문자 클래스를 사용하면 다음과 같이 간단하게 표현할 수 있다.
int[[:space:]]\+var;

이상이 정규 표현식에 관한 설명이었다. 이런 정규 표현식은 문자열 탐색에 그대로 이
용할 수 있다. 그리고 다소 복잡한 문자열을 표현하려면 정규 표현식을 사용해야 한다.
가령 다음과 같이 함수의 구현 부분을 찾으려면 정규 표현식을 사용하지 않고서는 표
현하기 힘들다.
/int [ [: space: ] ] \4-myfunc [ [: space :]]*(.*) [ [: space: ] ] * {

int nytuncfuoid) {
Return >J；

11,2-9

[그림 2-32] /int[[：space：]]\+myfunc[[：space：]]*(.*)[[：space：]]*{ 명령으로 탐색한 예

이런 정규 표현식은 앞서 말한 바와 같이 셸 명령인 grep에서도 사용할 수 있다.
현재 디 렉토리 이하의 모든 파일 중 int myfunc(void) 함수가 구현된 파일을 찾으려면
셸에서 다음 명령을 내린다.
$ egrep "int[[:space:]]+myfunc[[:space:]]*\(.*\)[[:space:]]*\{" ./ -Rlz
Mm-4?>os：.=mp/>est
(rootRos test]a pgrep [ :spacer ]]«nyfanc[[
./like.c
[i-oolRos test]# |

....................

:弓]]저*(：해)f('：spacp：] ]해주"
테

[그림 2-33] egrep "int[[：space：]]+myfunc[[：space：]]*\(.*\)[[：space：]]*\{"./ -Rlz 명령 수행 예

86

2부— 에디팅

===== PAGE 88 =====
명령이 다소 길지만 C 소스의 함수 구현 부분과 같이 복잡도가 높은 문자열은 위와 같
은 방식으로 정밀하게 검색해야만 어떤 파일에 있는지 한 번에 찾을 수 있다.
그리고 정규 표현식의 규칙만 확실하게 이해한다면 위와 같이 긴 정규 표현식의 의미
를 해석하는 일도 어렵지 않을 것이다.

vim는 확장 정규 표현식 또한 지원한다. 확장 정규 표현식은 [표 2-10]과 같다.
[표 2-1 이 vim 확장 정규 표현식
\i

변수 지정에 사용되는 문자[_0-9A-Za—z]

\l

누와 같지만 숫자는 제외

\k

키워드로 사용하는 문자[_\.\—0—9A—Za—z〉]

\K

\k 와 같지만 숫자는 제외

\f

파일명으로 사용하는 문자

\F

\f 와 같지만 숫자는 제외

\p

프린트 가능한 문자

\p

\p 와 같지만 숫자는 제외

\s

화이트 스페이스 문자（공백과 탭）

\s

화이트 스페이스가 아닌 문자

\d

숫자｛ 0—9]

\D

숫자가 아닌 문자P0—9]

\x

16진수 숫재 0-9A-Fa-f]

\x

16진수 숫자가 아닌 문자fO-9A—Fa-f]

\o

8진수 숫재 0-7]

\o

8진수 숫자가 아닌 문재。刀

\w

영문 단어에서 사용되는 문재0-9A-Za-z-]

\w

영문 단어에서 사용되지 않는 문재A0-9A—Za-z—]

\h

영문 단어의 시작에 사용되는 문자[A-Za-z—]

\H

영문 단어의 시작에 사용되지 않는 문재AA-Za-z-]

\a

모든 알파벳 [A-Za-z]

\A

알파벳이 아닌 문재AA-Za-z]

\I

소문재 a-z]

\L

소문자가 아닌 문자Ta-z]

\니

대문자｛ A-Z]

\u

대문자가 아닌 문재AA-Z]

\e

esc

\t

tab

\r

캐리지 리턴

\b

백스페이스

\n

개행 문자

2장_vi와 vim 에디터 87

===== PAGE 89 =====
확장 정규 표현식을 사용하면 정규 표현식을 훨씬 짧고 간결하게 작성할 수 있다. 가령
대문자로 이루어진 단어를 찾고자 할 때 일반적인 정규 표현식이나 POSIX 문자 클래
스를 사용한다면 다음과 같이 해야 될 것이다.
/\<[[:upper:]]\+\> 또는 /\<[A-Z]\+\>

하지만 vim 확장 정규 표현식을 사용하면 다음과 같이 간단하게 줄일 수 있다.
/\<\u\+\>

뭐 그렇게 확 줄어든 느낌이 들지 않는다. 그렇다면 앞에서 myfuncO 함수의 구현 부분
을 찾을 때 사용한 다음 정규 표현식을 줄여보자.
/int[[:space:]]\+myfunc[[:space:]]*(.*)[[:space:]]*{

위 정규 표현식을 vim 확장 정규 표현식으로 줄여보면 다음과 같다.
/int\s\+myfunc\s*(.*)\s*{

문자열 탐색뿐만 아니라 치환에서도 정규 표현식을 그대로 적용할 수 있다. 예를 들면
알파벳으로 이뤄져 있는 모든 단어를 “alpha”라는 문자열로 치환하려면 다음과 같은
명령을 내린다.
:%s/[A-z]\+/alpha/g

지금까지 vim의 정규 표현식을 알아봤다. 정규 표현식을 알면 쓸데없는 반복 작업을 최
소화할 수 있다. 그래서 필자는 반드시 정규 표현식을 익혀두라고 말하고 싶다. 정규 표
현식은 vim 에서 뿐만 아니라 grep, sed, awk, lex 등 많은 부분에서 사용하고 있으므
로 유닉스 계열 시스템에서 무언가를 해 보고자 하는 사람이라면 반드시 익혀두는 것
이 좋다.

I 여러 파일을 편집하는 방법
보통 한 프로젝트의 소스 파일은 하나의 파일로 이뤄져 있지 않다. 코딩을 하다 보면
이 파일에서 저 파일로 옮겨가면서 수정해야 되는 일이 대부분이다. 보통 GUI 편집기
는 여러 파일의 편집을 지원하기 위해 여러 탭으로 구분해 파일을 편집하는 형식으로
이뤄져 있다. 지금 수정하는 파일에서 다른 파일을 수정하려면 마우스나 단축키를 사용
해 다른 파일의 탭을 열고 수정하면 된다.

88 2부_에디팅

===== PAGE 90 =====
vim도 여러 파일을 편집하는 모드를 지원하는데, 필자가 생각하기에 여러 파일을 편집하
는 데 있어 vim만큼 편리한 편집기도 드물다. 그렇지만 vim의 기본 설정 상태에서는 편집
하기가 다소 불편하다. 여러 파일을 편리하게 편집하려면 몇 가지 설정을 해 줘야 한다.
먼저 여러 파일을 여는 방법을 알아보자. ［그림 2-34］ 처럼 현재 작업 디렉토리에는

filel.c, file2.c, file3.c 세 개의 파일이 있다. 각 파일이 프로젝트에서 각 부분을 담당한
다고 생각하면 된다.

［그림 2-34］ 현재 디렉토리의 파일

이렇게 여러 파일이 있을 때 한꺼번에 여러 파일을 여는 방법은 다음과 같은 명령으로
가능하다.
$ vi filel. c file2 . c file3 . c

위 명령과 같이 여러 파일명을 일일이 지원해도 되고, 다음과 같이 셸 메타 기호를 사
용해 한꺼번에 지정해도 된다.
$ vi * 또는 vi *. c

위 명령을 내리면 다음과 같이 filel.c 파일이 열린 것을 확인할 수 있다.

[그림 2-35] fflelc의 내용

보기에는 filel.c 파일밖에 열리지 않은 것으로 보인다. 그렇지만 vim 내부적으로는 세
개의 파일이 다 열려 있는 상태다. 열려있는 각 파일은 vim의 파일 버퍼에 들어있다. 각
파일 버퍼에 들어있는 내용은 ：ls 명령으로 확인할 수 있다. 사실 ［그림 2-35］ 처럼 filel.c
가 열려 있는 화면을 파일 버퍼라고 부르기도 한다.

2장_vi와 vim 에디터 89

===== PAGE 91 =====
그럼 파일 버퍼 간 전환을 해 보자.
:b2

명령라인 모드에서 위 명령을 내리면 열려있는 2번 파일로 전환한다. :b2라는 명령은
“파일 버퍼 2번”의 의미다.

[그림 2-36] fileZc의 내용

마찬가지로 3번 파일 버퍼로 전환하려면 :b3이라고 명령을 내린다. 열려있는 파일을 닫는
명령은 :bw다. :bw하면 현재의 버퍼를 닫는다. 버퍼에 관련된 명령은 다음 표와 같다.
[표 2-11] 파일 버퍼 관련 명령 요약
： buffers

버퍼의 내용을 나열

：files 또는 ：ls

버퍼의 내용을 나열

：b[N]

N번 버퍼로 이동

：bd[N]

N번 버퍼를 삭제（ N이 없으면 현재의 버퍼를 완전 삭제）

：bw[N]

N번 버퍼를 완전 삭제（ N이 없으면 현재의 버퍼를 완전 삭제）

:bp[N]

이전 버퍼로 이동. N을 붙이면 이번만큼 이전 버퍼로 이동

:bn[N]

이후 버퍼로 이동. N을 붙이면 이번만큼 이후 버퍼로 이동

：sb[N]

창을 수평 분할해 N번 버퍼를 로드

：bf

첫 번째 버퍼로 이동

：bl

마지막 버퍼로 이동

：al

현재 열려있는 모든 버퍼를 수평 분할 창에 로드

위에서 사용한 방법으로 파일을 전환하는 것은 코딩 과정 내내 빈번하게 발생하는 파
일 전환을 고려해 볼 때 다소 불편한 면이 있다. 이제 vim의 설정을 변경해 좀 더 편리
하게 단축키를 지정해 놓자.
:map ,1 :b!1<CR>
:map ,2 :b!2<CR>
:map t 3 :b!3<CR>

90 2부—에디팅

===== PAGE 92 =====
map 명령은 단축키를 매핑 (mapping) 할 때 사용한다. 위 명령을 명령라인 모드에서
차례로 내린 후 표준 모드에서 ,1 키를 누르면 1번 버퍼로 전환하고 ,2를 누르면 2번 버
퍼로 전환한다. 이때 타이밍이 중요하다. , 키를 누르고 뗀 후 숫자 키를 눌러야 하는데,
, 키를 누른 후 한참 있다가 1 키를 누르면 정상적인 명령으로 인식하지 않는다.

bl 이라고 하지 않고 b!l 이라고 한 이유는 2 번 버퍼에서 편집 작업을 수행한 후 파일
을 저장하지 않고 1번 버퍼로 이동하려고 할 때 vim이 파일이 편집되었지만 저장되지
는 않았다고 경고를 띄울 경우, 강제로 버퍼를 전환하기 위해서다.〈CR〉은 vim 내에서

Enter］ 키의 의미다.
현재 vim에 매핑되어 있는 모든 매핑 리스트는 단순히 명령라인 모드에서 :map이라고
입력해 주면 알 수 있다.
이제 파일 버퍼를 전환할 때는，［숫자］를 누르면 된다. 그런데 매번 위와 같이 ：map 명
령으로 키를 매핑해야 한다면 정말 불편한 일이 아닐 수 없다. 좀 더 편리하게 하려면

vim 설정 파일에 map 명령을 등록해야 한다.
vim 설정 파일에 키 매핑 추가
사용자의 홈 디렉토리에 .vimrc 파일을 생성하면 vim은 실행할 때 ~/.vimrc 파일을 읽
어 실행한다. .vimrc 파일은 vim 설정 파일로, vim 이 실행될 때 ~/.vimrc 파일에 적힌
명 령을 차례로 수행한다.

~/.vimrc 파일을 열어 다음 내용을 추가하자.
〔예제 2-2〕 ~/. vimrc 파일 내용

map
map
map
map
map
map
map
map
map
map
map
map
map

zl
,2
,3
,4
,5
/6
,7
,8
,9
zO
rX

zZ
,W

b!KCR>
b!2<CR>
b!3<CR>
b!4<CR>
b!5<CR>
b!6<CR>
b!7<CR>
b!8<CR>
b!9<CR>
b!10<CR>
bn!<CR>
bp!<CR>
bw<CR>

" 1 번파일버퍼로이동
" 2번파일버퍼로이동
" 3번 파일 버퍼로 이동
" 4번파일버퍼로이동
" 5번파일버퍼로이동
" 6번파일버퍼로이동
" 7번파일버퍼로이동
" 8번파일버퍼로이동
" 9번파일버퍼로이동
" 10번파일버퍼로이동
" 다음 파일 버퍼로 이동
" 이전파일버퍼로이동
" 현재 파일 버퍼 닫음

2장_vi와 vim 에디터

91

===== PAGE 93 =====
lot 제
lap
tap
tap
tap
tap
tap
lap
lap
tap
tap
lap
lap

,9
,0

:흐 P

sr：~
b?1<CR>
b*2<CR>
b?3<CR>
b?』»<CR>
b?5<CR>
b?6<CR>
b?7<CR>
b*8<CR>
b?9<CR>
b?18〈CR：
bn?<CR>
bp?<CR>
bw<CR>

번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
번 파일 버퍼로 이동
0번
버퍼로 이드
버퍼로 이
I음
버퍼로 이
I전
।재
버퍼 닫음

[그림 2-37] 〜/.vimrc 파일의 내용

그리고 다시 여러 파일을 열었다면 표준 모드에서 ,1 또는 ,2와 같은 단축키로 파일 버
퍼를 전환할 수 있다. 지금 설정에서는 10개의 파일 버퍼를 단축키로 지정했다. 그러나

vim에서 사용 가능한 파일 버퍼는 이보다 훨씬 많다（ 1000단위가 넘어갈 정도다）. 10개
이상의 파일 버퍼를 지정하고 싶다면 추가로 지정한다.

map 명령으로 단축키를 매핑할 때 주의할 점이 있다. map 명령으로 매핑할 때는 표준
모드에서 사용하지 않는 단축키를 사용해야 한다. 나중에 다시 map 명령을 설명하겠
지만 호기심에 먼저 시작하는 독자가 있다면 반드시 이점을 기억하고 map 명령을 사
용하기 바란다. 그리고 참고로 위 .vimrc 파일에서 "（큰따옴표）는 주석을 의미한다.

I 반복되는 문자열을 저장해서 쓰기
이전에 잘라내기에서 레지스터에 대해 잠깐 언급했다. 이전에 설명한 17개의 레지스터
외에 vim은 a부터 그까지 26개의 레지스터를 더 지원한다. 이런 레지스터를 네임 레지
스터라고 하는데, 이 레지스터는 반복되는 문자열을 저장해 쓰기에 편리하다.
가령 C 코딩을 하다 보면 다음과 같이 printf로 디버깅 메시지를 찍어보는 경우가 빈번
히 발생한다.
〔예제 2-3〕 printf로 디버깅 메시지를 찍어보는 예제 소스

int main () {
int i;
i = 2;
#ifdef DEBUG
printf("DEBUG : i = %d\n", i);
#endif
return 0;
}

92 2부—에디팅

===== PAGE 94 =====
이런 디버깅 메시지를 네임 레지스터에 저장하고 사용하면 된다. 저장하는 명령은 표준
모드에서 다음과 같이 하면 된다.
"a3yy

Ha는 a 레지스터에 저장하라는 의미고, 3yy는 현재 커서 위치에서 세 행을 복사해 저장
하라는 의미다.
이렇게 명령을 내리면 현재의 커서 위치에서 아래로 3행을 복사해 a 레지스터에 저장
한다. 저장된 내용을 붙여넣는 방법은 원하는 위치에서 다음 명령을 내리면 된다.
"ap

"a로 a 레지스터를 지정하고 p로 붙여넣었다.

[그림 2-38] "a3yy 명령을 내린 화면

[그림 2—39] "ap 명령을 내린 화면

a부터 z까지 총 26개의 네임 레지스터를 지원함으로써 넉넉하게 원하는 문자열을 저장
해 사용할 수 있다.

2장_vi와 vim 에디터 93

===== PAGE 95 =====
I 매크로의 사용
vim에서 매크로란 키 입력을 네임 레지스터에 저장해 사용하는 방법을 말한다. 이해하
기 쉽게 예제를 보면서 알아보자.

[그림 2-40] 매크로 사용 설명을 위한 예제 소스

위와 같은 소스 파일이 있다고 가정했을 때 현재 커서가 있는 행에 주석을 넣으려면 키
입 력으로 A i // Space Bar] EsclEnterH 키를 순차적으로 눌러준다. A 기호는 커서를 현재
행의 처음으로 이동하는 명령이다. i 키를 사용해 입력 모드로 전환한 후 //와 공백을
입력한다. 그리고 % 키를 사용해 표준 모드로 전환한 후 Enter! 키를 눌러 다음 행의
처음으로 커서를 이동하는 것이다.
이런 키 입력을 저장해 필요할 때 사용하는 기능이 있다면 반복적으로 키를 눌러줘야
하는 작업에서는 편리할 것이다. 이런 경우 사용하는 기능이 바로 매크로 기능이다. 매
크로를 사용하는 방법은 다음과 같다.
먼저 q [네임 레지스터명]을 눌러 매크로를 등록할 레지스터를 지정한다. 가령 b 레지
스터를 사용하려면 qb라고 입 력한다.
qb

qb 라고 입력하면 화면 하단에 “기록 중”이란 글자가 나온다. 이후에 누르는 키들은
b 레지스터에 저장된다.
A i // Space Bar] Escl Enter] 키를 차례로 누른다. 그리고 q를 누르면 화면 하단의 “기록

중”이란 메시지가 사라지면서 b 레지스터에 이제까지 누른 키들이 등록된다.

94 2부_ 에디팅

===== PAGE 96 =====
이제 b 레지스터에 등록된 매크로는 @b를 누름으로써 사용할 수 있다. @b를 누르면
A i // Space Bar| Esc『Enter| 키를 순차적으로 누르는 것과 같은 결과를 가져온다. 5@b를

누르면 @b를 다섯 번 사용한 결과가 나타난다.

[그림 2-41] 은 b 레지스터에 A i // SpaceBar]|Esc]£nterj 키를 등록해 5@b 명령으로
다섯 번 반복했을 때의 결과다.

[그림 2-41] 5@b 명령 후

마찬가지로 행 주석을 없애는 매크로를 c 레지스터에 저장하려면 qc를 입력해 매크로
를 저장할 레지스터를 지정한 후 A3x Ente「|를 입력한 후 q를 누른다.
A

기호는 행의 처음을 의미하고, 3x를 사용해 현재 커서의 위치에서 세 글자를 지운 후

Enter]를 눌러 다음 행의 처음= 이동한다는 의미다.

I 다중 창 사용하기
프로그래밍을 하거나 소스를 분석하다 보면 다른 파일에 작성된 구조체의 타입이나 소
스를 참조해야 될 때가 많이 발생한다. 이런 경우 다중 창 기능을 사용하면 유용하다.
다중 창 기능이란 vim의 화면을 여러 개로 분할해 사용하는 방법을 말한다.
표준 모드에서 Ctrl]-w n（ Ctrl] 키를 누른 상태에서 w 키를 누르고, Ctrt] 키를 떼고 n 키
를 누른다. n은 new의 의미） 키를 누르면 vim 창이 [그림 2-42]처럼 가로로 분할되는
것을 볼 수 있다.
2장_vi와 vim 에디터 95

===== PAGE 97 =====
［그림 2-42］ £gBv n 입력 후 모습

이렇게 창이 분할되면 ：e ［파일명］ 명령으로 파일을 불러올 수 있다. ［그림 2-43］ 은
파일을 불러오는 모습을 보여준다.

［그림 2-43］ ：e file2.c 명령으로 새로 열린 창에 file2.c 파일을 불러온 모습

창 간 커서 전환은 Ctrl］ -ww(.Ctrt］ 키를 누른 상태에서 w 키를 두 번 누름) 키로 할 수
있다.
반복해서 Ctrl|-wn 키를 누르면 창을 계속 분할할 수 있다. 그리고 이렇게 분할한 창은
食리-wq(quit) 키를 누르거나 명령라인 모드에서 :q!를 입력함으로써 닫을 수 있다.

CtrtJ-ws 키는 현재의 파일을 분할한다. 무슨 말이냐 하면 현재 filel.c 파일이 열려 있
는 창에서 Ctrt|-ws(split) 키를 누르면 창이 수평 분할되면서 filel.c의 내용이 분할된
창에 나타난다.

Ctii］ -wv(vertical split) 키를 누르면 창이 수직 분할된다. ［그림 2-44］ 는 Ctrl］ -wv 키
로 창을 수직 분할한 예다.

96

2부_에디팅

===== PAGE 98 =====
[그림 2-44] CtrlHw 키로 수직 분할한 모습

수직 분할 역시 창 간 전환은 Ctrl]-ww 키로 하며, 주로 두 파일을 비교할 때 사용한다.
분할한 창의 사이즈를 조절하고 싶을 때가 있다. 가령 헤더 파일에 구조체를 참고하다
가 당장은 필요가 없어졌지만 빈번하게 참고해야 될 때가 있을 것이다. 이런 경우 창의
크기를 조정하면 된다. 수정 중인 소스 파일의 창은 최대로 하고, 헤더 파일의 창은 최
소로 만들면 되는 것이다.
현재 작업 중인 창을 최대로 하는 명 령은 수평 분할일 경우 Ctrl]-w 키이고, 수직 분할
일 경우 Ctrt]-w| 키다.

[그림 2-45] 최대화하기 전의 모습

2장_vi와 vim 에디터 97

===== PAGE 99 =====
[그림 2-46] Ctrl]—w 키로 최대화한 모습

위와 같이 최대화한 창을 원래대로 균등하게 분할된 상태로 만들고 싶을 때가 있을 것
이다. 그럴 때는 %-w= 키를 사용하면 최대화되었던 창이 원래의 균등 분할된 상태
로 돌아온다.
다음은 이런 창 분할과 관련된 명령들을 요약해 놓은 표다.
[표 2너2] 다중 창 명령 요약

표준 모드

명령라인 모드

결과
창생성

:Ctrl]—WS

:sp[plit]

현재 파일을 두 개의 수평 창으로 나눔

逆가—WV

：[N]vs[plit]

새로운 수직 창 생성, N이 붙으면 N칸 크기의 창 분할

Ctrl]—wn

：new

새로운 수평 창 생성

Ctrll-v/

수평 창으로 나누고 이전 파일의 오픈

Ctrt]-wf

창을 수평으로 나누고 커서 위치의 파일을 오픈

食라—wi

커서 위치의 단어가 정의된 파일을 오픈
창 삭제

jCtrll-wg

:q[니 0

현재 커서의 창을 삭제

jCtrl]-wc

:clo[se]

현재 커서의 창을 삭제

wo

：on[ly]

현재 커서의 창만 남기고 모든 창 삭제
창이동

W]—wh

왼쪽 창으로 커서 이동

lCtrl]-wi

아래쪽 창으로 커서 이동

：Ctrl]-wk

위쪽 창으로 커서 이동

: Cti니—wl

오른쪽 창으로 커서 이동

Ctrl]—ww

창을 순차적으로 이동

食리—WP

가장 최근에 이동한 방향으로 이동

心러]—wt

최상위 창으로 이동

Ctrl]—Wb

최하위 창으로 이동

98 2부—에디팅

===== PAGE 100 =====
창 위치 바꾸기

[C레—wr

순차적으로 창의 위치를 순환

:Ctrl]—WX

이전 창과 위치를 바꿈
창크기 조정

食파%=

창의 크기를 모두 균등하게 함

SJ—w_

수평 분할에서 창의 크기를 최대화
수직 분할에서 창의 크기를 최대화

%—w[N]+

：res[ize] +N

창의 크기를 N행만큼 증가(%-w+는 1행만큼 증가)

心tr〔j—w「N]—

：res[ize] -N

창의 크기를 N행만큼 감소(째-w-는 1행만큼 감소)

；CtrtHw「N]>

창의 크기를 오른쪽으로 N칸만큼 증가(수직 창에 한함)

£"w[N]〈

창의 크기를 왼쪽으로 N칸만큼 증가(수직 창에 한함)
* 명령라인 모드에서 [] 내의 문자는 생략 가능함을 의미

위 명령들을 자세히 살펴보면 규칙성이 있음을 발견할 수 있다. 일단 幼！]-w를 누르게
되어 있다. 그리고 창 생성의 경우 분할(split), 새 창(new), 수직 분할(vertical split)의
영문자 첫 글자로 이뤄져 있다.
창 삭제의 경우도 마찬가지다. 일단 Ctrlpw를 누른다. 그리고 종료(quit), 닫기(close),
단일(only)의 영문자 첫 글자를 누르면 된다.
창 이동의 경우 기본 이동 키인 h, j, k, 1 키와 연관이 있는 것을 알 수 있고, 최상위 (top),
최하위(bottom) 등의 첫 글자로 이뤄진 것을 알 수 있다.
이런 일관성만 파악한다면 아무리 많은 창 관련 명령도 외우기 쉬울 것이다. 그리고 항
상 말하듯이 어는 배우는 것이 아니라 익히는 것이기 때문에 이해되었다고 해서 따라
해 보지 않으면 안 된다. 몸이 기억할 수 있게 여러 번 반복해서 사용해야 한다.

I 마킹으로 이동하기
지금까지 vim의 기본적인 커서 이동에 관해 알아봤다. 이제는 좀 더 고차워적인 마킹
으로 이동하는 방법을 알아보자.
마킹은 의미대로 커서의 특정 위치를 임의의 문자로 마킹해 나중에 표시한 위치로 한
번에 돌아가기 위한 방법이다. 이런 마킹 기법은 소스가 매우 긴 파일이거나 여러 곳을
동시에 수정할 때 많이 사용된다. 그리고 특히 커널과 같이 거대한 프로젝트 소스를 분
석할 때 사용하면 유용하다.

2장_vi와 vim 에디터 99

===== PAGE 101 =====
마킹은 다음 명령으로 가능하다.
m ［임의의알파벳］

: 마킹할 때

’ ［마킹한 알파벳］ : 마킹된 위치로 돌아갈 때

마킹에는 세 가지 종류가 있다. A-Z까지 대문자로 마킹한 전역 마킹과 a-z까지 소문자
로 마킹한 지역 마킹, 그리고 ~/.viminfo 파일에서 자동으로 지정한 0-9 로 이뤄진 파
일 마킹이 그것이다.
알파벳으로 마킹하는 전역, 지역 마킹은 언제든지 사용 가능하지만 숫자로 이뤄진 파일
마킹은 vim이 실행될 때나 종료될 때 자동으로 지정되기 때문에 사용할 수 없다. 파일
마킹은 이전에 vim으로 편집한 파일의 경로와 파일 내에서의 위치를 vim이 알아서 마
킹 한다.
전역 마킹과 지역 마킹의 차이점은 다음과 같다.
• 전역 마킹 (A-Z)： 현재 파일을 포함한 다른 파일 간의 마킹 이 가능하다.
• 지역 마킹(a-z)： 현재 파일 내에서만 마킹이 가능하다.
즉, 대문자로 마킹하면 파일이 다르더라도 마킹한 위치로 이동할 수 있지만 소문자로
마킹하면 현재 파일 내에서만 마킹이 유효하다.

ma를 눌러 현재 커서 위치를 a로 마킹한다.

［그림 2-47］ 마킹 사용법 예제 1

위와 같은 소스가 있을 때 main() 함수에 dojDrintO 함수가 사용되었는데, 이전에

do_print() 함수의 원형이 선언되지 않았다. 그래서 위 소스는 컴파일되긴 하지만 컴파
일할 때 경고 메시지가 발생한다.

100 2부.에디팅

===== PAGE 102 =====
경고 메시지는 결코 달가운 것이 아니므로 main() 함수 앞에 do_print() 함수의 원형
을 선언해 경고 메시지를 없애주기로 했다. do_print() 함수는 물론 현재 파일의 아래
부분에 있고, 필자는 do_print 함수를 모르는 상태라고 가정하자.
표준 모드에서 탐색 명령 /do_print 를 사용하면 do_print() 함수를 찾을 수 있을 것
이고, yy 명령으로 do_print() 함수의 정의 부분에서 원형을 복사할 수 있다. 하지만
돌아오는 것이 문제다. 파일이 매우 길 경우 원하는 위치로 돌아오는 것이 만만치 않
을 것이다. 물론 위 소스는 매우 짧고 돌아오려는 위치가 파일의 최상단에 있기 때문에

gg (파일의 처음으로 이동) 명령으로 돌아오면 될 것이다. 그러나 돌아오려는 위치가
파일에서 임의의 위치일 경우 마킹을 사용하면 한결 수월하다.
먼저 현재 위치를 마킹해야 한다. 현재 위치에서 ma(marking a) 라고 입력하면 현재
위치가 a 로 마킹된다. 그런 다음 /do_print 명령으로 do_print() 함수가 정의되어 있
는 곳을 찾는다. 찾았으면 yy로 복사한다.

[그림 2-48] 마킹 사용법 예제 2

그리고 다시 a 로 마킹된 곳으로 돌아가면 된다. "a(' 기호는 backtick을 의미)를 입력
하면 a 로 마킹된 지점으로 돌아간다. 그리고 p 명령으로 do_print() 함수의 원형을 붙
여넣고 편집하면 된다.

2장_vi와 vim 에디터 101

===== PAGE 103 =====
［그림 2-49］ 마킹 사용법 예제 3

vim에서 마킹된 모든 정보는 ：marks 명령으로 확인할 수 있고 마킹과 관련된 명령은
［표 2-13］ 과 같다.
［표 2-13］ 마킹 관련 명령 요약

명령 I 내용
ma

a로 마킹, mb는 b로 마킹

'a

a로 마킹된 위치로 돌아감

직전에 커서가 위치하던 행의 처음
이전에 vim으로 현재 파일을 닫았을 때
커서가 있던 행의 처음으로 이동

명령

내용

‘a

a로 마킹된 행의 처음으로 돌아감

w

직전의 커서 위치로 이동

\«

이전에 vim으로 현재 파일을 닫았을 때
커서가 있던 위치로 이동

I 셸명령사용
vim에서 작업을 하다가 잠깐 셸로 돌아가 어떤 명령을 실행해야 할 때가 있다. 예를 들
면 ifconfig 명령을 입력해 작업 PC의 IP를 알아내거나, 현재의 프로그램을 컴파일하고
실행시켜 결과를 알아보고 싶은 경우가 있을 것이다. 그럴 때마다 매번 vim을 종료하
고 셸로 돌아가서 명령을 내린 후 다시 vim을 실행한다면 작업이 비효율적일 것이다.
이렇게 셸 명령을 입력하거나 셸로 잠깐 빠져나가기 위한 방법이 있다.
명령라인 모드에서 :!［명령］을 입력하면 잠시 vim을 빠져나갔다가 명령이 수행된 후
다시 vim으로 돌아온다. 예를 들면 :!1s를 입력하면 1s 명령이 수행되고 다시 vim으로
돌아올 수 있다.

102 2부_에디팅

===== PAGE 104 =====
［그림 2-50］ 명령 수행의 예

마찬가지로 셸을 수행할 수도 있다. :!bash라고 입력하면 새로운 셸이 열리면서 vim을
빠져 나간다. 셸에서 원하는 명령을 수행하고 다시 vim으로 돌아오려면 셸에서 exit 명
령을 내려 셸을 종료한다. 그러면 다시 vim으로 돌아온다.
명령을 내린 후 화면에 출력되는 결과가 필요할 수 있다. 그때는 ：r !［명령］과 같은 형식
으로 명령을 내리면 명령이 수행된 결과가 현재 커서의 위치에 끼워 넣어진다.
가령 1s 명령을 내렸을 때 화면에 출력되는 결과를 현재 커서 위치에 끼워 넣고 싶다면
：r !ls라고 명령을 내린다.

［그림 2-51］ ：r !ls 명령 수행의 예

원래 ：r ［파일명］ 명령은 현재 커서의 위치에 파일의 내용을 끼워 넣으려고 사용한다.
그래서 filel.c 파일을 수정하고 있었는데. ：r file2.c 명령을 내리면 현재 커서의 위치에

file2.c의 내용이 끼워 넣어진다.

2장_vi와 vim 에디터 103

===== PAGE 105 =====
04 vim의 조력 ajctags, cscope,
기타 플러그인
지금부터 배울 내용은 정말 흥미롭고 재미있는 내용들이다. vim은 여러 프로그램 또는
내장 스크립트와 연동이 가능하다. 이런 연동 가능한 대표적인 프로그램으로는 ctags,

cscope, man°l 있고, 내장 스크립트에는 bufexplorer, taglist, calendar, vimspell 등
수없이 많다.
연동 프로그램은 바이너리 형식의 실행 파일들로, vim과 독자적으로 동작할 수 있는 프
로그램을 의미한다. 내장 스크립트는 vim의 내장 스크립트로, 프로그래밍된 스크립트
파일을 말한다.
원래 vim은 기능 확장을 위한 자체적인 내장 스크립트를 가지고 있다. 이 내장 스크립
트는 의외로 많은 문법과 기능이 있어 내장 스크립트로 프로그래밍해 vim에 새로운 기
능을 추가하는 것이 가능하다.
내장 스크립트는 보통 vim 플러그인이라 부르고 확장자가 *.vim으로 끝난다. vim은 실
행될 때 전역 플러그인 디렉토리（페도라인 경우 /usr/share/vim/vim［버전］/plugin） 에
있는 내장 스크립트를 읽어 들이고, 사용자 홈 디렉토리의 ~/.\dm/plugin 디렉토리에
있는 내장 스크•립트를 읽어 새로운 기능을 추가한다.
이런 프로그램과 연동해 vim은 강력한 편집기가 되는 것이다. 때로는 연동 프로그램을
사용하려고 vim을 사용할 정도로 연동 프로그램의 기능은 매우 비중 있고 가치 있다.

I 소스 태그를 찾기 위한 만능 해결사 ctags
필자가 vim을 사용하면서 진정으로 vim이 강력하고 멋진 편집기라고 느꼈을 때는 바
로 ctags의 사용법을 익히고 난 후였다.
유닉스 프로그래밍하는 사람치고 ctags를 모른다면 간첩에 가깝다. 아니면 정말 강인
한 인내의 소유자거나 거짓말을 보태 프로그래밍을 수행의 목적으로 하는 사람일지도
모른다. 그 정도로 ctags는 매우 잘 알려졌고 유용하다.

104 2부—에디팅

===== PAGE 106 =====
ctags의 정의
ctags는 프로그래밍 소스 코드에서 태그（전역변수 선언, 함수 정의, 매크로 선언）들의
데이터베이스（ tags 파일）를 생성하는 유닉스 명령이다. 이후 생성된 태그 데이터베이
스는 vim이나 emacs 같은 편집기에서 특정 심볼을 찾고자 할 때 이용할 수 있다.

ctags에서 인식하는 파일 종류는 다음 표와 같다.
[표 2-14] ctags에서 인식하는 파일 종류

Assembler, ASP, Awk, C, C++,
BETA, Cobol, Eiffel, Fortran,
Java, Lisp, Lua, Make, Pascal,
Perl, PHP, PL/SQL, Python,
REXX, Ruby, Scheme, Shell scripts （ Bourne/Korn/Z） ,
S-Lang, Tel, Vera, Verilog, Vim,
YACC/Bison

ctags를 사용하면 커널과 같은 거대 프로젝트를 분석하거나 다른 사람이 프로그래밍
소스로 프로그래밍할 때 유용하게 사용할 수 있다. ctags와 같은 툴을 사용하지 않고
리눅스 커널 같은 거대 프로젝트를 분석한다면 그건 흔히 말하는 삽으로 땅을 파는 일
이라고 생각한다.
커 널 스스는 수많은 디 렉토리 트리가 있으며 , 또한 수많은 파일로 이뤄졌다. 많은 디 렉
토리와 파일 속에서 원하는 태그를 grep의 정규 표현식으로 찾는 일은 웬만한 인내로
는 하기 힘들다. grep 명령으로 검색하는 시간도 시간이지만, 무엇보다 일의 흐름이 끊
어져 생기는 피해도 만만치 않다.
그렇지만 ctags를 사용하면 단 몇 초 안에 태그가 있는 파일을 열어 커서를 원하는 태
그 바로 앞에 가져다 놓는다. 그럼 실습으로 ctags를 사용해 어떻게 커널을 분석하는지
알아보자.

I ctags 설정 및 기본 사용법
ctags 를 사용하려면 ctags 패키지가 설치돼 있어야 한다. 셸에서 ctags --help 명
령으로 ctags 가 설치돼 있는지 확인하자. ctags 가 설치돼 있지 않다면 http ： //ctags.

sourceforge .net 이나 http://rpm.pbone.net 에서 받을 수 있다. ctags 가 설치됐다면
vim에서 사용할 수 있는 태그 데이터베이스를 ctags 명령으로 생성해야 한다.

2장_vi와 vim 에디터 105

===== PAGE 107 =====
앞으로

분석할

커널

소스

디

렉토리（필자의

경우/work/book/utils_new/vim/

linux-2.6.29） 로 이동해 다음의 명령을 내리면 태그 데이터베이스인 tags 파일이 만들
어진다. 이전에 받아 놓은 커널 소스가 없다면 /usr/include 디렉토리를 사용해도 되지
만 앞으로 실습에서 많이 이용되기 때문에 커널 소스를 kernel.org에서 받아 압축을 풀
어두기 바란다.
$ ctags -R

위 명령을 내리면 ［그림 2-52］ 와 같이 tags 파일이 만들어진다.
1* root@server：/work/book/utils_new/vim/linux-2.6.2§
[root@seruer linux-2.6.29]휴'11ct주히'三히—"
[root@seruer linux-2.6.29]tt
[rootSseruer linux-2.6.29]# Is -al tags ___________________________________
-rw-r--r-- 1 root root 105644065 4월 26 23:49[tags|
[rootBswver linux-2.6.29]# |

［그림 2-52］ ctags 명령을 통해 태그 데이터베이스（ tags 파일） 생성

tags 파일을 열어 내용을 보면 ［그림 2-53］ 과 같다.

［그림 2-53］ 태그 데이터베이스 파일의 내용

tags 파일은 세 개의 필드로 이뤄졌는데, 첫째 필드는 태그명을 나타내고, 둘째 필드는
파일명, 셋째 필드는 파일 내에 태그가 정의된 형식을 나타낸다.

vim 에서 커널의 printkO 함수의 원형을 알고 싶어 태그를 찾는 명령을 내리면 먼저
tags 파일의 태그명 필드를 비교해 printk와 일치하는 태그를 찾고 일치하는 태그들의
리스트를 보여준다.

106 2부_에디팅

===== PAGE 108 =====
리스트 중 하나를 사용자가 선택하면 vim은 태그가 위치한 파일을 열고 커서를 태그에
위치시 킨다.
태그 데이터베이스를 만들었다면 vim에서 set 명령으로 tags 변수에 생성한 태그 데이
터베이스（ tags 파일） 파일을 설정해 준다. 태그 파일이 복수 개일 때는 ‘,’를 구분자로
여러 개의 태그 파일을 지정할 수 있다.
- 단일 지정

: set tags=./tags
-복수 지정

: set tags=./tags,/work/book/utils_new/vim/linux-2.6.29/tags,/usr/
include/tags

:set tag5=/work/book/utils_new/uin/linux-2.6.29/1ags|

[그림 2-54] tags 변수의 설정

매번 위와 같이 태그 변수를 지정해 준다면 굉장히 번거로울 것이다. 홈 디렉토리의

.vimrc 파일을 열어 다음 내용을 추가하면 매번 태그 변수를 지정하지 않아도 vim이
실행될 때 변수를 자동으로 지정한다.
root@server7woiVbook/utils_new/vim/linux

.그 P
lap
lap
lap
tap
)ap
lap
tap
lap
tap
lap
tap

히)

,7
,8
,9
,0

b?1<CR>
b?2<CR>
b?3<CR>
b?4<CR>
b?5<CR>
b?6〈CR>
b?7<CR>
b?8 CR>
b?9<CR>
b?10CCR>
bn?<CR>
bp?<CR>
bw<CR>

” 1번 파일 버퍼로 이동
"2번
파일 버퍼로 이동
» 3 번 파일 버퍼로 이동
"4번
파일 버퍼로 이동
" 5번
파일 버 퍼 로 이동
“ 6번
파일 버 퍼 로 이동
" 7번
파일 버 퍼 로 이동
•• 8번
파일 버 퍼 로 이동

•• 9번

파일

버퍼로

이동

" 18번 파일 버퍼로 이응

" 다음 퐈일 버퍼로 이응
" 이전 파일 버퍼로 이드
“ 현재 파일 버퍼 닫음 ‘

[그림 2-55] 〜/.vimrc 파일에 tags 변수의 설정

2장_vi와 vim 에디터

107

===== PAGE 109 =====
이제 ctags를 사용하기 위한 모든 준비가 끝났다. 커널 디 렉토리 (kernel 소스가 없는
사람은 /usr/include 디렉토리)에서 vim 을 실행시킨다. 그리고 명령라인 모드에서 다
음 명령을 내려본다.
: t j start_kernel (kernel 스J스가■ 없는 사•람은 : tj printf)

tj 명령은 tag jump의 약자다. tj start_kernel을 실행하면 태그 데이터베이스 파일
(tags)에서 start_kern이 태그를 찾아 ［그림 2-5이처럼 리스트로 나열한다.

파일
arch/alpha/boot/bootp .c
start_kernel
start_kernel(uoid)
2F
start kernel
arch/alpha/boot/bootpz.c
start_kernel(void)
start_kernel
arch/alpha/boot/main.c
uoid .start_kernel(uoid)
startjkernel” init/main.c
asmlinkage uoid _]nit start_kernel(uoid)
Choice number (<Enter> cancels): |
1F

[그림 2-56] ：tj start kernel 명령 수행 결과 1

지금 4개의 start_kernel 태그를 tags 파일에서 찾았다. 우리가 보기 원하는 start_

kernel은 i386 PC의 커널 메인 시작 코드이므로 init/main.c 파일의 start_kernel 4번
에 해당한다. 여기서 4번을 입력하면 ［그림 2-5기과 같이 init/main.c 파일이 열리고 커
서가 start_kernel 태그의 시작 위치로 이동한다.
/ m()t6’’<;prvt>r：/w(ifk/bm)k/utils iww/virn/linux -2.6.29

하smlinkage uoid _init start_k아'nel(uoid)
char * command_line;
extern struct kernel_param _start_____________________________ _stop
a찌];
sinp_setup_processor_id();
/*
* Need to run as early as possible, to initialize the
* lockdep hash:
*/
lockdep_init();
"init/main.c" 884L, 21649C

530,1

[그림 2-57] ：tj start_kernel 명령 수행 결과 2

명령라인 모드에서 ：sts start_kern이이라고 입력하면 ［그림 2-58］ 과 같이 vim 창이 수
평 분할되면서 init/main.c 파일의 start_kernel에 커서가 이동한다.

108 2부—에디팅

===== PAGE 110 =====
［그림 2-58］ ：sts start_kernel 명령 수행 결과

태그를 찾고 점프하는 명령은 ［표 2-15］ 와 같다.
［표 2너5］ ctags 명령 요약
:ta 旧I그1 또는 Ctrl 뉘

［ tag］ 가 정의된 위치를 나열하고 선택한 위치로 점프.

：ts ［태그］ 또는 ：tj ［ tag］

현재 위치는 스택에 pus된다.

：po 또는 ctriH-t

스택 top에 저장된 위치를 pop하고 그 위치로 점프

：sts ［태그］

［ tag］ 7^ 정의된 위치를 나열하고 선택한 위치로 창을 수평 분할해

：stj ［태그］

새로 생성된 창에 표시

：tn

느나 ts로 점프했을 때 다음 태= 점프

:tp

느나 ts로 점프했을 때 이전 태그로 점프

：tr

느나 ts로 점프했을 때 처음 태그로 점프
나나 ts로 점프했을 때 마지막 태그로 점프

：pts ［태그］

［태그］가 정의된 위치를 나열하고 선택한 위치로 창을 수평 분할해
새로 생성된 창에 표시하지만 커서는 현재 위치에 유지

:ptj ［태그］

미리보기 윈도우에 태그가 정의된 형식을 보여줌

：ptn

ptj 나 pts로 점프했을 때 다음 태그로 점프

:ptp

ptj 나 pts로 점프했을 때 이전 태그로 점프

：ptr

ptj 나 pts로 점프했을 때 처음 태그로 점프

：ptl

ptj나 pts로 점프했을 때 마지막 태그로 점프

［표 2-15］ 에서 :ta와 :ts는 스택을 사용한다고 되어 있다. 그 말은 현재 위치를 vim 스
택에 push하고 점프를 한다는 의미다. 나중에 다시 점프했던 곳으로 돌아올 때는 ：po
나 %+t 키를 눌러 스택에 저장되어 있는 위치를 pop해서 돌아온다.
물론 위의 모든 명령을 다 외울 필요는 없다. 필자의 경험상 :sts와 ：tj, Ctii|+L Ctrl|+t
정도만 알아도 ctags 를 사용하는 데 별문제 없다. 일단 ctags 를 이용해 소스 파일의
특정 태그를 쉽게 찾는 방법은 익혔다. 그런데 아직은 조금 불편하다.

2장_vi와 vim 에디터

109

===== PAGE 111 =====
아직까지는 명령라인 모드에서 ：sts start_kernel이라고 일일이 타이핑해야 하기 때문
이다. start_kernel이 아니라 usb_get_current_Jrame_number 태그라면 느낌이 어떨
까? 태그 명령을 좀 더 쉽게 사용하기 위해 vim의 내장 스크립트를 작성해 보자.

I vim 내장 스크립트 작성
홈 디 렉토리의 .vimrc 파일을 열어 다음과 같은 행을 추가한다.
〔예제 2-4〕 〜/.vimrc

파일에 추가한 내용

if version >= 500
func! Sts()
let st = expand(”<cword>")
exe "sts ’’. st
endfunc
nmap ,st :call Sts()<cr>
func! Tj ()
let st = expand("<cword>")
exe "tj ".st
endfunc
nmap ,tj :call Tj ()<cr>
endif

[그림 2-59] 〜/.vimrc 파일에 추가한 모습

먼저 if version >= 500 ~ endif로 묶어 vim의 버 전이 5.0 이상일 때만 적용되 게 했다.
이렇게 하는 이유는 하위 버전의 vim 스크립트에서는 함수 형식을 지원하지 않아 오류
가 발생하기 때문이다.

110 2부_에디팅

===== PAGE 112 =====
func! Sts() ~ endfunc로 Sts() 함수를 정의하고 let st로 st 변수를 생성했다. 그리고
expand("<cword>") 명령으로 현재의 커서가 위치하는 단어를 읽어 st 변수에 집어넣
었다. exe 명령으로 뒤에 오는 명령을 수행하는데, "sts ’’.st하게 되어 "sts " 문자열에

st 변수의 문자열을 붙여넣었다. 따라서 현재 커서가 위치한 태그가 start_kernel이라
면 exe "sts start_kernel" 형식으로 수행된다.
이렇게 정의한 함수를 nmap ,st ：call Sts()<cr> 명령으로 ,st 키에 매핑했다. 그래서 표
준 모드에서 ,st라고 명령을 내리면 명령라인 모드에서 ：call Sts()<cr> 명령이 수행되어

Sts() 함수가 호출된다(내장 스크립트 작성에 대해 더 궁금한 독자는 vim 매뉴얼을 참
고하기 바란다. ：help usr_41).
이제는 커서를 찾으려는 태그의 위치에 놓고 표준 모드에서 ,st 명령만 내리면 ：sts ［태
그］ 명령을 수행할 수 있다. 마찬가지로 ,tj 명령을 내리면 ：tj ［태그］ 명령이 수행된다.
제대로 동작하는지 한번 테스트해 보자.
$ vi -t start_kernel

어떤 위치에서든지 셸에서 위 명령을 내리면 vim 은 현재 설정 파일에 설정된 tags 변
수의 패스를 기준으로 tags 파일을 찾아 tags 파일에서 제일 처음 만나는 태그로 점프
한다. 대부분 원하는 위치로 점프하지만 kernel과 같이 중복되는 태그가 많을 경우 원
하는 위치로 한 번에 점프될 때가 드물다. 원하는 곳으로 점프하지 않았다면 ：tn 명령으
로 우리가 보기 원하는 커널 디렉토리의 init/main.c 파일을 찾아 이동해야 한다.
이동을 하였다면 찾기 원하는 태그의 위치에 커서를 위치시킨다. ［그림 2-6이은 2.4 버
전 커널에서 lock_kernel() 함수에 커서를 위치시켰다. 그리고 ,st 명령을 내리면 lock_

kerneK) 함수가 정의된 파일 리스트가 나타난다.
'g] r0ot@os：/usr/src/Hnux-2.4

세|||圓히

三 Activate the First processor."—
asmlinkage uoid _init start_kernel(uoid)
<
char » comnahdlifie;
extern char sayed_coininand_line[ ];
/*
* Interrupts are still disabled. Do necessary wtsps, then
* enable then
*/
locg_kernel();
printk(linuxbanner);
setup_arch(ftcoFinand_li.ne);
printkC Kpf-nel conmmtf line: %.<：?.'m“, saued connand line);
parse_options(coniRand_line);
trap_init();
initZlRQO;
_____________________ 359,5-12

62홍 P|

［그림 2-60］ ,st 명령을 수행하는 모습

2장_vi와 vim 에디터 111

===== PAGE 113 =====
3 rooibos：/usr/$rc/linux-2.4
it pri Kind tag
IF
F
2 F

f

3 F

f

F

cl

5

F

F

6

F

F

__ HHC

표일

P
/usr/src/linuxalpha/smplock .hO
static _inline
void lock_kernel(uoid)
loci<> kernel
/usr/src/linuxm-arm/smplock.h山
static inline uoid lock_kernel(uoid)
lock_kernel
/usr/src/linux-.
cris/snp_lock.hH
extern _inline uoid lock_kernel(uoid)
lock kernel
/usr/src/linux-cris/snplock.hH
lock kerru1!

甘

lock kernel
extern _inline
lock kerne 1

/usr/src/linuxuoid lockkernel(void)
/usr/src/linux-

neric/smplock.h昌
~i386/smplock .hH

.......................................... cJrjjJt-.ix'......... Axxl.i.na---------- iinirt 1 nrlz Uo»-ni>1 f iini ri t

빠 키를 누르면
다음 리스트가 나오고
q 키를 누르면 선택을 위해 정지

sr/src/linux- -ia6*»/smplock .hl
sr/src/linux- -n68k/smplock.h
uoid lo마<_kernel(uoid)
sr/src/linux- ~nips/smplock.

•- 더 --I

三|

[그림 2-61] ,st 명령 수행 결과 1

원하는 파일을 선택하면 선택된 파일이 열린다. 우리는 i386 커널 코드를 분석할 것이
기 때문에 q 키를 눌러 리스트의 출력을 정지시키고 6번을 눌러 /usr/src/linux-2.4/

incl니de/asm-i386/smplock.h 파일을 연다.

[그림 2-62] ,st 명령 수행 결과 2

/usr/src/linux—2.4/incl니de/asm—i386/smplock.h 파일의 lock_kernel() 함수 내부에
current가 사용되었는데, current?} 무엇인지 알고 싶어졌다. 그러면 다시 current에
커서를 가져다놓고 ,st를 입력한다.

112 2부—에디팅

===== PAGE 114 =====
［그림 2-63］ current에 ,st 명령을 수행

current는 매크로라는 것을 알 수 있고, 실제로는 get_current() 함수 호출이라는 것을
알 수 있다. 지금 창이 세 개로 나누어졌는데, 좀 더 넓게 보고 싶을 경우 Ctrl］ +w _ 키
를 누르면 ［그림 2-64］ 와 같이 현재 커서의 창이 최대로 되는 것을 확인할 수 있다.

［그림 2-64］ 자세히 보기 원하는 창을 최대화

이제 ctags의 설정까지 마쳐서 ctags를 쉽게 사용할 수 있게 되었다. 무척이나 쉽고 편
리하지 않은가? 당장이라도 코딩하면서 테스트해 보고 싶어졌을 것이다. 부단히 사용
해 몸에 익히길 바란다.

2장_vi와 vim 에디터 113

===== PAGE 115 =====
I cscope> 사용해 나머지 2%를 채워라
ctags만으로도 커널 소스와 같은 대규모 프로젝트를 분석하는 데 부족한 점은 없을 것
이다. 그렇지만 ctags가 완전히 우리의 욕구를 충족시켜주는 것은 아니다. ctags로 찾
을 수 있는 C, C++ 소스의 태그 종류는 [표 2-16]과 같다.
[표 2-16] ctags로 찾을 수 있는 C. C++ 태그 종류

classes
macro definitions (and #undef names)
enumerators
function definitions
enumeration names
class, struct, or union members
namespaces
function prototypes and declarations [off]
structure names
typedefs
union names
variable definitions
extern and forward variable declarations [off]

즉, ctags만으로는 지역변수나 전역변수가 사용된 곳이나 함수가 사용된 곳을 찾기 힘
들다. 이때는 cscope를 사용한다.

cscope는 대화식 C 소스 분석 프로그램이다. cscope는 심볼을 찾기 위한 데이터베이
스 파일로 cscope.out 파일을 사용하고, ctags가 찾지 못하는 것들을 찾아낼 수 있다.

ctags가 단지 vim이 사용하는 태그 데이터베이스만 만드는 프로그램임에 비해 cscope
는 원래부터 C 소스를 분석하기 위해 만들어졌다. 그래서 cscope는 vim 없이 자체적
으로 동작 가능하며, C 소스를 분석할 때 유용하게 사용할 수 있다.

cscope로 분석 가능한 소스 파일에는 Assembly, C, C++, Lex, Yacc 등이 있다.
cscope가 설치되어 있지 않다면 http://cscope.sourceforge.net이나 http：//rpm.
pbone.net 사이트에서 다운로드할 수 있다. cscope를 설치 했으면 다음 명령을 사용
해 분석하려는 커널 디렉토리에 cscope.out 파일을 생성한다.
$ find . \ (-name ’ * . c ’ -o -name ’ * . cpp ’ -o -name ’ * . cc ’ -o -name
’ * .h’ -o -name ’ * . s ’ -o -name ’ * . S ’ \) -print > cscope .files
$ cscope -i cscope.files

114 2부—에디팅

===== PAGE 116 =====
굉장히 복잡한 명령으로 보일 거라고 예상한다. 제일 처음 find 명령으로 현재 디렉
토리 이하 모든 디렉토리에 있는 파일 중 어셈블리 소스 파일(*.s, *.S)과 C 스스 파일,

C++ 소스 파일을 찾아 cscope.files 파일에 파일 리스트로 만든다.
그리고 cscope -i cscope.files 명 령으로 파일 리스트에 있는 파일을 cscope 가 한 줄
씩 읽어들여 cscope.out 심볼 데이터베이스 파일을 생성한다. 매번 cscope 심볼 데이
터베이스 파일을 만들기 위해 위와 같이 긴 명령을 내린다면 너무나도 가혹한 일이다.
위 명령을 셸 스크립트로 만들어 보자.
〔예제 2-5)

mkcscope.sh 파일 작성

#!/bin/sh
rm -rf cscope.files cscope.files
find . \ (-name ’ *.c’ -o -name ’ *.cpp' -o -name ’ * .cc’ -o -name :
’ * .h’ -o -name ’ * . s1 -o -name ’ * . S ’ \) -print > cscope .files
cscope -i cscope.files

위와 같이 mkcscope.sh 파일을 만들고 다음 명령을 차례로 수행해 mkcscope.sh 명
령을 사용할 수 있게 한다.
$ chmod 755 mkcscope.sh
$ mv mkcscope.sh /usr/local/bin

그리고 커널 디렉토리로 가서 mkcscope.sh 명령을 수행하면 ［그림 2-65］ 와 같은 화
면이 나오면서 심볼 데이터베이스가 만들어지는 것을 확인할 수 있다.
경우에 따라 상태 바가 멈춰서 한동안 움직이지 않을 때가 있을 것이다. cscope 하위
버전을 사용하면 간혹 cscope가 데이터베이스를 빌드하면서 무한 루프에 빠져버리는
경우가 있다. 그런 현상이 일어난다면 cscope를 최신 버전으로 바꾸면 된다.
/ root④server：/work/book/utils_new/너m/1inux-2.60
riUWUiLMILhMgtTtabase 6720

22678

Find this C symbol:
Find this global definition:
Find functions called by this Function:
Find Functions calling this Function:
Find this text string:
Change this text string:
Find this egrep pattern:
Find this File:
Find Files ttincluding this File:
Find all Function definitions:
Find all symbol assignments:

［그림 2-65］ 커널 디렉토리에서 mkcscope.sh 명령 수행
2장_vi와 vim 에디터

115

===== PAGE 117 =====
데이터베이스 파일(cscope.out)의 빌드가 끝났으면 Ctrl]+d 키를 눌러 빠져나온다.
이제는 앞으로 cscope를 사용할 것이라고 vim에 알려야 한다. ~/.vimrc 파일에 다음
내용을 추가하면 vim에서 cscope를 사용할 수 있다.
〔예제 2-6〕 〜/.vimrc 파일에 추가한 내용

set csprg=/usr/bin/cscope
set nocsverb
cs add /work/book/utils_new/vim/linux-2.6.29/cscope.out
set csverb
set csto=0
set cst

[그림 2-66] 〜/.vimrc 파일에 cscope 설정을 추가한 모습

이제 기분 좋게 cscope® 사용하기 위한 설정이 끝났다. cscope를 vim에서 사용하려
면 먼저 cscope의 명령 형식을 알아야 한다.
：cs find { 질의종류} { 심볼}

ex) : cs find s start_kernel

cscope의 명령 형식은 위와 같다. 먼저 명령라인 모드에 ：cs find 명령이 오고 다음에
질의의 종류가 온다. 질의의 종류는 찾으려는 심볼의 범위를 말한다. 마지막으로 심볼
이 오는 형식으로, cscope 명령은 항상 위와 같이 구성된다.

116 2부—에디팅

===== PAGE 118 =====
질의의 종류는 ［표 2-1기을 참고한다.
[표 2-17] cscope 질의 종류
0 or s

Find this C symbol

1 or g

Find this definition

2 or d

Find functions called by this function

3 or c

Find functions calling this function

4 or t

Find assignments to

6 or e

Find this egrep pattern

7orf

Find this file

8 or i

Find files including this file

그러면 이제 cscope를 본격적으로 사용해 보자. 명령라인 모드에서 다음 명령을 입력
하면 start_kernel과 관련된 모든 심볼을 찾을 수 있다. start_kernel 함수가 사용된 곳
혹은 내부에서 변수의 지역변수 이름으로 사용되었던 모든 start_kernel 심볼을 찾을
수 있다.
: cs find s start_kernel
오 root@server：~
:scope

=_싀

: start kernel

厂1'
1
2
3

6

8

9

arch/alpha/boot/head.S «GLOBAL»
jsr $26,start_kernel
60 I arch/arm/kernel/head—common.S <<GL0BAL»
b start_kernel
arch/aur32/kernel/head.S <<GLOBAL»
.long start_kernel
508
arch/fru/kernel/head.S «GLOBAL>>
call start_kernel
449
arch/ia64/kernel/head.S «GLOBfiL»
br.call.sptk.many rp=start_kernel
27
arch/m32r/kernel/head.S <<GLOBAL>>
.global start_kernel
120 1 arch/m68knommu/platForm/68328/head-de2.S
«GLOBfiL»
jrap start_kernel
213
arch/m68knonmiJ/platForm/68328사wad-pilot .S
.....«JULDBjftL».......................................

閉삐삐!※a 키를 누르면 다음 리스트가 i
출력되고 q 키를 누르면 출력 중지 ^68328/head-ram.S

■- 더 -

[그림 2-67] ：cs find s start kernel 명령을 수행한 모습

나머지는 질의 종류 표를 보면서 직접 해 보기 바란다. 그럼 이제 cscope를 좀 더 편하
게 사용할 수 있게 ~/.vimrc 파일에 스크립트를 작성하자.

2장_vi와 vim 에디터 117

===== PAGE 119 =====
〔예제 2-기

〜/.vimrc 파일에 추가한 cscope 함수와 단축키 설정

func! Css ()
let
css
=
expand(”<cword>")
new
exe "cs find s ". css
if getline (1) == ’’ ’’
exe "q!
endif
endfunc
nmap ,css :call Css()<cr>
func! Csc ()
let
csc
=
expand("<cword>")
new
exe "cs find c ’’. csc
if getline (1) == ”’’
exe "q!
endif
endfunc
nmap ,csc :call Csc()<cr>
func! Csd()
let
csd
=
expand("<cword>”)
new
exe "cs find d ”. csd
if getline(1) == ""
exe "q!
endif
endfunc
nmap ,csd :call Csd()<cr>
func! Csg()
let
csg
=
expand("<cword>")
new
exe "cs find g ”. csg
if getline (1) == ’’’’
exe q!
endif
endfunc
nmap ,csg :call Csg ()<cr>

이제 스크립트만 보고도 대충은 감을 잡을 거라고 생각한다. 위 스크립트는 각각의

cscope 질의 종류를 함수로 만들고 각 함수를 키에 매핑해 놓았다. 가령 심볼이 정의
된 곳과 사용된 곳을 보려면 커서를 심볼에 위치시키고 ,css라고 명령을 내린다. 심볼
이 정의된 곳을 찾으려면 ,csg 명령을 내린다. 나머지는 여러분이 한 번씩 직접 해 보기
바란다.

118 2부_에디팅

===== PAGE 120 =====
사실 ctags 와 같이 cscope 를 사용한다면 위에서 매핑한 키 명령을 다 사용할 필요는
없다. cscope 는 ctags보다 훨씬 느리기 때문에 ctags를 사용하다가 ctags가 찾지 못하
는 것만 cscope 로 사용하면 된다. 예를 들면 함수나 변수가 사용된 곳을 찾을 때와 같
은경우다.

| 완벽한 조합 vim + screen + ctags + cscope
지금까지 vim + ctags + cscope를 사용한 프로그래밍과 소스 분석 기법을 알아보았다.
이 조합에 screen을 추가하면 아주 환상적 인 개발 환경 이 구현된다.

screen은 여러 가상 터미널을 생성해 나눠주는 역할을 한다. 로그인한 후 셸을 할당받
으면 하나의 가상 터미널과 연결된 셸을 받는다. 키보드로 입력하면 터미널을 통해 셸
에 전달되고, 셸에서 출력되는 내용은 터미널을 통해 화면에 출력된다.

telnet이나 ssh로 접속을 해 두 개의 셸을 사용하고 싶었다면 단순히 bash 명령을 입력
해 셸을 두 개 띄우는 것으로는 해결되지 않는다. 셸이 같은 터미널 (/dev/pts/[N]) 을
공유하게 돼 입력과 출력 모두 두 개에서 동시에 이뤄지기 때문이다.
그렇지만 실제로는 bash 명령으로 두 개의 셸을 띄우고 1s 명령을 실행해 보면 화면에

1s의 결과가 두 번 출력되는 것은 아니다. 자식 셸을 띄운 부모 셸은 자식 셸이 끝날 때
까지 대기하고 있기 때문이다.

[그림 2-68] 원격으로 접속해 bash 명령을 내렸을 때 모습

위 예에서 두 개의 셸을 독립적으로 사용하려면 두 개의 셸 각각에 가상 터미널을 새로
할당해야 한다. 그런 일을 하는 것이 바로 screen 이다. screen으로 세 개의 셸을 띄웠
을 때는 [그림 2-69]와 같은 구조를 가진다.

2장_vi와 vim 에디터

119

===== PAGE 121 =====
[그림 2-69] screen 명령을 수행한 후 셸을 3개 띄운 모습

결국 screen을 사용하면 하나의 화면에서 두 개의 셸을 번갈아 가면서 사용할 수 있다.
셸에서 다음 명령을 내리면 screen이 실행된다.
$ screen

[그림 2-70] screen 명령을 수행

싱겁게도 화면만 지워지고 어떤 변화도 일어나지 않을 것이다. 이렇게 screen을 실행
시켰다면 1s 명령을 내린 후에 Ctrl]+ac 키를 눌러보자. 1s 명령 후의 결과가 사라지고
새로운 셸이 뜨는 것을 알 수 있다. 새로운 셸은 새로운 가상 터미널을 할당받은 상태
다. 가상 터미널 간 전환은 Ctrl|+aa 키로 하고, Ctrl|+ac 키는 새로운 터미널을 생성할
때 사용한다.
[Ctrl] +ac

120 2부—에디팅

===== PAGE 122 =====
[그림 2-71] 새로운 가상 터미널 생성

그 외 screen의 단축키는 다음 표와 같다.
[표 2너8] screen 단축키 요약
Ctrl] +a’

화면 하단에 새로운 가상 터미널을 선택할 수 있는 입력 프롬프트가 나옴

Ctrt]+a”

현재 생성되어 있는 모든 가상 터미널이 나열되며 커서로 선택할 수 있음

Ctrl. +a[N]

N번째 가상 터미널로 이동

Ctrl. +aa

바로 이전 가상 터미널로 이동

CfiU+ac

새로운 가상 터미널 생성

jCtri] +ad

현재의 가상 터미널을 닫음

헤 +ag

visual bell을 on/off

IM

다음 가상 터미널로 이동

心레 +ap

이전 가상 터미널로 이동

Shiftl +[Page up]

화면 위로 이동

WH +[Page Down]

화면 아래로 이동

screen은 여러 파일을 수정할 때 유리하다. 파일 버퍼 간 전환은 vim 내에서 :b[N] 명
령으로 하면 되지만 때로는 여러 개의 창을 사용하고 싶을 때가 있을 것이다. 가령 한
창에서는 파일을 수정하고, 다른 창에서는 컴파일하고 디버깅하는 용도로 말이다.
이럴 때 screen 을 사용하면 좋을 것이다. 그리고 screen 의 또 다른 좋은 점은 세션을
유지한다는 점 이다. 필자가 telnet이나 ssh를 사용해 원격으로 소스를 수정하고 있었는
데 갑자기 네트워크 불량으로 접속이 종료되면 대책이 없을 것이다.
물론 vim은 “.파일명.swp” 파일에 주기적으로 백업을 하지만 .swp 파일의 내용이 항상
화면과 동기화되는 것은 아니다. 이럴 때 screen을 사용하는 중이었다면 걱정할 필요
가 없다. 사용자가 갑자기 접속을 잃었더라도 screen의 세션은 그대로 유지되므로 고
뇌에 찬 비명이나 한숨 대신 다시 접속해 단지 다음 명령만 내려주면 접속을 잃었을 때
의 화면이 그대로 복구된다.

2장_vi와 vim 에디터 121

===== PAGE 123 =====
$ screen -r 또는 screen -r ［세션명］

궁금한 독자가 있다면 지금 당장 실행해 보기 바란다. 먼저 ssh 로 접속해 screen 을
작동시키고 vim 으로 파일을 수정하고 창을 과감하게 닫는다. 그런 후 다시 접속해

screen -r 또는 screen -r ［세션명］ 명령을 내리면 편집 중이던 정겨운 화면을 볼 수
있을 것이다.

screen 의 특정 세션을 분리하는 것은 screen -D ［세션명］ 명령이다. 여러 개의
screen 세션이 살아있어 그 중 하나를 분리해 다시 연결하고 싶다면 screen -D ［세션
명］, screen -r ［세션명］ 명령을 차례로 내려준다.

vim 을 사용한다면 vim + screen + ctags + cscope는 환상의 조합으로 통한다. 이 프
로그램 네 개를 활용하면 프로그래밍을 아주 효율적이고 편리하게 할 수 있다.

| 모르는 함수를 알고 싶을 때 man page의 활용
c 프로그래밍을 하다 보면 자주 사용하지 않는 함수의 경우 사용법을 모를 경우가 있
다. 혹은 다른 사람이 작성한 소스를 분석하다가 표준 c 라이브러 리에는 포함되어 있
지만 직접 사용해 보지 않아 무슨 일을 하는지 모르는 경우가 있다.

Windows 계열 IDE에서는 이런 경우를 대비해 온라인 매뉴얼과 MSDN이라는 아주 방대
한 매뉴얼을 제공한다. 유닉스 계열도 매뉴얼을 제공하는데, man page가 바로 그것이다.

man page를 활용하면 모르는 함수의 원형이나 사용법을 아주 쉽게 참고할 수 있다.
먼저 ~/.vimrc 파일에 다음 내용을 추가한다.
〔예제 2-8〕 〜/.vimrc 파일에 추가한 man page 사용 함수와 단축키 설정

func! Man()
let sm = expand (”<cword>’’)
exe ’’! man -S 2:3:4:5:6:7:8:9: tel: n: 1: p: o " . sm
endfunc
nmap ,ma :call Man()<cr><cr>

위 설정이 제대로 되지 않으면 exe 명령을 아래와 같이 바꿔보기 바란다.
exe ’’! man -S ko:2:3:4:5:6:7:8 ’’. sm

122 2부—에디팅

===== PAGE 124 =====
[그림 2-72] ~/.vimrc 파일에 추가한 내용

위 설정을 보면 sm 변수에 현재 커서가 위치한 단어를 읽어 와 "!man -S 2：3：4：5：6：7：

8：9：tcl：n：l：p：o ".sm 명령으로 man을 실행시키는 것을 알 수 있다.
이때 -S 2：3：4：5：6：7：8：9：tcl：n：l：p：o 옵션을 붙여준 이유는 man page에는 C 프로그래밍
함수의 매뉴얼뿐만 아니라 여러 셸 명령도 함께 있는데, 셸 명령이 man 프로그래밍을
참조하는 디렉토리의 1번 디렉토리에 있어 C 함수와 셸 명령이 중복되면 셸 명령을 우
선시하기 때문이다.
예를 들면 printf 는 C 함수로도 존재하고 /usr/bin/printf 와 같이 셸 명령.0 .루-두 존재
한다. -S 2：3：4：5：6：7：8：9：tcl：n：l：p：o 옵션을 붙이지 않고 man printf 명령을 내리면 C
함수의 매뉴얼을 보여주는 것이 아니라 /usr/bin/printf 명령의 매뉴얼을 보여준다.
이와 같이 셸 명령과 C 함수의 이름이 중복됐을 때 C 함수의 매뉴얼을 우선 실행하기
위해 위 옵션을 붙여준 것이다.
원래 vim에서 대문자 K를 누르면 매뉴얼이 보인다. 그러나 대문자 K로 출력되는 man

page는 셸 명 령을 우선 실행하므로 C 프로그래머의 매뉴얼로 적합하지 않다.
이렇게 설정하고 소스 내에서 매뉴얼을 보기 원하는 함수에 커서를 가져다 놓고 표준
모드에서 ,ma를 입력하면 커서 위치의 함수를 찾아 화면에 매뉴얼을 보여준다. 다음은

printf 함수의 매뉴얼을 보여주는 예다.

2장_vi와 vim 에디터 123

===== PAGE 125 =====
WiTI히

M [screen 4： bash] root@cs：/'terr®/lest
P«INIF(3)

Linux Programmer *s Manual

PRINTF(3)

NAME
printf,
fprintF,
sprintF,
snprintf,
vsprinlf, 115nprintf - Foriwtted output conversion

uprintF,

vFprintF,

SYNOPSIS
Itincludp <stdio.h>
int printF(const char “format, ...)；
int Fprintf(FILE "stream, const char «f
...)；
int sprintf(char «str. const char «Format, —);
int snprintF(char *str. size_t size, const char *format.

이□끄흐

filnclude <stdarg.h>

[그림 2-73] printf 함수 위에 커서를 두고 ,ma 명령을 수행한 모습

이 렇게 man page를 vim과 같이 활용하면 매우 편리하다. 언제든지 매뉴얼을 볼 수 있
기 때문에 vim이 좀 더 강력해진다.

ctags, cscope, man은 vim과 연동 가능한 대표적인 바이너리다. 다음은 vim의 플러그
인에 대해 알아본다.

I 플러그인을 사용해 vim의 기능 확장
앞서 ~/.vimrc 파일에 vim 스크립트를 사용해 기능을 확장하는 작업을 간단하게 해 보
았다. 이 렇게 .vimrc 파일에 스크립트를 직접 넣어도 기능 확장이 가능하지만 vim은 좀
더 유연한 기능 확장을 제공한다. 그리고 기능 확장을 위한 미리 만들어진 스크립트가
많이 있다.
이런 스크립트를 vim 플러그인이라 하고, http://www.vim.org/scripts 에서 수많은

vim 플러그인을 볼 수 있다. http://www.vim.org/scripts 에 있는 플러그인 중에는 글
자의 색깔을 바꾸거나 달력을 보여주는 간단한 것에서부터 게임이나 파일 버퍼를 보여
주고 영문 스펠링을 검사하는 복잡한 것까지 다양하다.
그럼 플러그인을 어떻게 vim에 붙여 사용하는지 알아보자. 먼저 http：//www.vim.org/

scripts 사이트에서 calendar.vim 스크립트를 받아온다. calendar.vim 스크립트는 vim
에서 달력을 보여주는 스크립트다. calendar.vim 스크립트의 내용을 보면 다음과 같이

vim 스크립트로 작성 됐음을 알 수 있다.

124 2부—에디팅

===== PAGE 126 =====
劉 rcoWCi：：' / '，'•「『/?>U2h
0Mp
nnwp

Calemi<ir-0 :cal Calen(lar( J
j CalendarH :cal C<»lentUr(1)<£R>

”* GetTokea : get token from source with count
•*
'«
‘*

src : source
din : deliniter
ent : skip count

^unctiont :GetTok&n(s>*c,dlm,cnt)
let tokn hit=8
” flaq oF Found
let tokn Fnd" fround path
let tokn_5P!=■'
•' token
let tokn_all-a:src “
all source
“• safe for end
let tokn._all - tokfi_all.a:dln
»4»ile a
let tokn_spl - strpart(tokn_all,e,natch(tokn_all,a:dlin))
let tokn_hit “ tokn_hit ♦ i
if tokn_hit — a:cnt
return tokn_spl
“calendar.vim" 1l5fil, 355
C

脚

286,1

［그림 2-74］ calendar.vim 스크립트의 내용

스크립트를 받아왔으면 vim이 실행되면서 스크립트를 읽을 수 있게 특정 위치에 옮겨
야 한다. 그리고 이때 전역으로 모든 사용자가 스크립트를 공유하는 위치가 있고, 현재
의 사용자만이 스크립트를 사용하는 위치가 따로 있다.
전역으로 사용 가능하게 하려면 페도라 배포판의 경우 /usr/share/vim/vim70/plugin
디 렉토리에 calendar.vim 파일을 복사하고, 자신만 사용하려면 mkdir ~/.vim/plugin
명령으로 자신의 홈 디렉토리에 ~/.vim/plugin 디렉토리를 만든 후 calendar.vim 파
일을 ~/.vim/plugin 디 렉토리에 복사한다.
다음은 root 유저를 사용하는 필자의 플러그인 설치 예다.
HI root@os：~/.vim/plugin
[rooteos plugin]ft pwd
/root/ .uiin/plugin
[root80s pluginpt is calendar.vim
calendar.vim
[rootQos plugin]tt |

［그림 2-75］ calendar 플러그인을 설치한 모습

이렇게 calendar.vim 플러그인을 설치했으면 vim을 실행하고 명령라인 모드에서

:Calendar라고 명령을 내린다. ［그림 2-76］ 과 같이 달력이 나타난다.

2장_vi와 vim 에디터 125

===== PAGE 127 =====
［그림 2-76］ :Calendar 명령을 수행한 후의 모습

이렇게 달력을 나타내는 기능이 프로그래밍에서 그렇게 유용한 기능은 아닐 것이다. 좀
더 유용한 기능인 파일 버퍼를 보여주고 커서를 선택해 파일 버퍼를 이동하는 플러그
인을 사용해 보자. http://www.vim.org/scripts 사이트에서 bufexplorer.zip 파일을 받
아와 압축을 푼다. 그러면 bufexplorer.vim 스크립트가 있을 것이다. b니fexplorer.vim
스크립트를 이전과 같이 ~/.vim/plugin 디렉토리에 복사하고 여러 텍스트 파일이 있
는 디렉토리에서 다음 명 령을 실행해 여러 파일을 vim으로 연다.
$ vim *

그러고 나서 명령라인 모드에서 :Buffixplorer를 입력하면 ［그림 2-7기처럼 파일 버퍼
의 리스트가 나열되고 커서를 이용해 파일을 선택할 수 있는 화면이 나온다.
H [screen 4： bash] root@os：/temp/test
" Press ? For Help
” Sorted by mru
|

1

玄

Filel.c
/temp/test
file2.c
/temp/test
file3.c /temp/test
4 mark.c /tenp/test

［그림 2-77］ BufExplorer 명령을 수행한 후의 모습

126 2부—에디팅

===== PAGE 128 =====
열려는 파일 위치로 가서 Ented 키를 누르면 선택한 파일이 열린다.
째 [screen 4: bash] root@os：/temp/test
허truct nptine <
unsigned int hour;
unsigned int minute;
unsigned int second;

>

"file2.c" 5L, 82C

[그림 2-78] file2.c* 선택한 예

필자는 개인적으로 bufexplorer보다는 ,1 또는 ,2, •••를 사용한 파일 버퍼 간 이동을 좋
아 하지만, 눈으로 확인하면서 파일 버퍼를 선택하고 싶은 독자라면 bufexplorer를 사
용하는 것도 좋을 것이다.
다음으로 설명할 플러그인은 현재 파일의 태그 리스트를 보여주고 이동이 가능하게 하
는 taglist다. taglist를 활용하면 현재 파일에 어떤 전역변수와 함수가 있는지 일목요연
하게 알 수 있고, 태그 간 이동도 쉽게 할 수 있다. 매우 큰 파일을 수정할 때 taglist를
이용하면 좀 더 편리하게 작업을 할 수 있다.
마찬가지로 http://www.vim.org/scripts 사이트에서 taglist.vim 스크립트를 받아
와 ~/.vim/plugin 디렉토리에 설치한다. 그리고 이전에 ctags 를 실습할 때 사용했던

kernel 디렉토리로 이동해 다음 명령을 내린다.
$ vim -t start_kernel

위 명령을 내리면 start_kernel과 일치되는 태그들이 나열될 것인데, init/main.c를 번호
로 선택해 init/main.c 파일을 연다.
명령라인 모드에서 ：Tlist라고 입력하면 ［그림 2-7이와 같이 현재 파일에 있는 변수 함수
명이 나열된다.

2장_vi와 vim 에디터 127

===== PAGE 129 =====
［그림 2-79］ ：Tlist 명령을 수행한 화면

Ctrt|+ww 키를 눌러 태그 리스트 창으로 이동한 후 이동하려는 태그에서 Enter］ 키를
누르면 커서가 선택한 태그 위치로 이동한다. ［그림 2-80］ 은 debug_kernel 태그를 선
택해 이동한 예다.

[그림 2-80] debug_kern이 선택 화면

다음으로 소개할 플러그인은 영문 단어 스펠링을 검사하는 vimspeU 플러그인이다. 역
시 마찬가지로 http://www.vim.org/scripts 사이트에서 vimspell.vim 스크립트를 받
아 설치하면 된다.
스펠링 체크 기능은 텍스트 파일이나 C 소스에서 주석에만 적용된다. 좀 더 명확한 결
과를 보여주기 위해 커널 디렉토리에 있는 COPYING 파일을 열어 결과를 보여준 예는
다음과 같다.

128

2부_ 에디팅

===== PAGE 130 =====
명령라인 모드에서 :SpellCheck라고 입력하면 vimspell이 동작하면서 스펠링이 틀린
단어를 찾아낸다.
［그림 2-81］ 은 결과 화면인데 필자가 일부러 틀리게 입력한 글자들이 붉은색 밑줄 글
자로 표시되는 것을 알 수 있다.
HIFJE3||

(screen 4： bash) root®os：/u$r/src/linux-2.4

으

NOIET This copyright does »not* cover user programs that use kernel네
services by nornal system calls - this is merely considered nornal usH

g

Also note that thd Ibelou is copyrighted tyy the Free Software

kernel) is copyrighted | no and others who actually wrote it.
Eueryone is pernitted to copy and distribute uerbdtin copies
oF this license document, but changing it is not allowed.
Preamble
The licenses for most software are designed to take duay your
8.29 꼭대기

［그림 2-81］ vimspell 플러그인을 설치해 :SpellCheck 명령을 수행한 화면

vimspell 플러그인을 설치한 후 ：help vimspell이라고 입력하면 vimspell에서 지원하
는 명령라인 모드 명령을 알 수 있다. 매번 ：SpellCheck 명령을 내리지 않고 자동으로
스펠링을 체크하려면 ：SpellAutoEnable 명령을 내리고, 자동 체크 기능을 해제하려면

:SpellAutoDisable 명령을 내린다.
단, vimspell은 vim의 실행 속도를 느리게 할 수 있으므로 주의해서 사용해야 한다. 플
러그인을 실행시키는 명령은 보통 스크립트 소스의 주석 부분에 있다. 주석 부분에 없
다면 명 령라인 모드에서 :command 명 령으로 확인할 수도 있다. 그렇지만 모든 플러
그인을 :command 명령으로 확인할 수 있는 것은 아니다. 기타 유용한 플러그인으로
여러 라인의 주석을 처리하는 EnhCommentify과, html, xml, sgml 문서 작성을 도와
주는 xmledit, cvs 명령이 정리된 cvscommand, 그림을 그리는 Drawlt 등이 있다.
그리고 지금까지 소개한 플러그인 외에 http://www.vim.org/scripts 사이트에 가보면
수많은 플러그인이 있다. 나머지 플러그인의 설치와 사용은 독자에게 맡긴다. 유용한
플러그인을 찾으려면 http://www.vim.org/scripts 사이트에서 많이 내려 받은 플러그
인순으로 찾으면 된다.
그 중에서는 오류가 발생하는 플러그인도 있고, 또한 어떤 플러그인은 vim의 속도를 떨
어뜨린다는 것을 숙지하고, 자신의 상황에 맞는, 자신이 필요로 하는 플러그인을 찾아
설치하는 것이 좋을 것이다.

2장_vi와 vim 에디터

===== PAGE 131 =====
5 개발자를 위한 vim의 유용한 팁
다음으로 소개할 내용은 인터넷에 떠도는 vim의 유용한 팁이다. 가끔은 팁이 정말 유용하
게 사용될 때가 많다. 그러나 팁은 팁일 뿐이다. 정공법을 모르고 팁만 안다는 것은 아무
의미가 없다. 지금까지 잘 따라왔던 독자라면 팁을 이해하는 데도 별 무리가 없을 것이다.

I 파일 탐색 기능 활용
간혹 편집을 하다보면 어떤 디렉토리의 파일을 편집해야 하는데 파일명이 기억나지 않
을 때가 있다. 이때는 vim 의 파일 탐색 기능을 이용하면 된다. 파일 탐색 기능은 vim
에 explorer 플러그인이 설치되어 있어야 된다. 페도라 배포판이라면 기본적으로

explorer 플러그인이 설치되어 있으므로 바로 사용할 수 있다.
:20vs ./

위 명령으로 창을 나눌 때 뒤에 디렉토리명을 지정해 주면 해당 디렉토리에 있는 파일
들이 브라우징된다. 열어보려는 파일을 선택하면 파일이 열린다.
iU root@os：/temp/test
•’ Press ? for keyboa
” Sorted hy name (Jb

UincUirte <stdio.h>

"= /temp/test/

int main() {

B./
File2.c
file3.c
like.c
mark
mark .c
rnyfunc .c
old.txt
tags
.myfunc.c.swp
filel.h

<emp/test 4,1 모둬
|"/teinp/test"는 자료방입니다

s同리
ng
■

mpfunc();
return 8;
}

int mpfunc(uoid) {
return 0;
>

m9f「unc.c

■■EK■■■■■■風느
너

[그림 2-82] ：20vs ./ 명령으로 현재 디렉토리의 파일 리스트를 보여준 화면

I 빠른괄호 이동 및 빠른 탐색
긴 함수의 경우 if문과 while문이 중첩 사용되면 함수의 범위나 if문과 while문의 범위
가 어디까지인지 잊어버리는 수가 있다. 이때는 범위를 알고 싶은 ‘{’ 또는 ‘}’ 기호에서
% 기호를 누르면 쌍을 이루는 ‘{’ 또는 ‘}’로 커서가 이동한다.

130 2부-에디팅

===== PAGE 132 =====
［그림 2-83］

{ 기호에 커서를 위치

"] I M ： I i j 'O’! I <--■• J ： / r '•■'■：

/

1h PH

~

int Ipn = *>t rlPti(sl r);

For (i=«, sp=str; i < HfiX_ARGU && j <= len; j++) {
if (?*(str*j) *(str：j-i))
arqufi**] - sp;
if (isspace(«(str*j))) <
»(str+j)= -mr；
if (j o ftft *(str*j-i))
argufi’*] ’ sp;
sp = str ♦ j * ?;

drgu[i] = Q;
■•nshell.C,' =L , 1113C 저장 헸습니다

29,2-9

m

27% Q

［그림 2-84］ % 기호를 눌렀을 때 쌍이 되는 } 기호로 커서가 이동한 모습

찾으려는 문자열에 커서를 두고 * 기호나 # 기호를 누르면 /［찾으려는 문자열］ 또는
?［찾으려는 문자열］ 명령을 내렸을 때와 같은 결과가 된다.

［그림 2-85］ str 문자열에서 * 기호를 입력한 모습

I 폴딩기능이용
폴딩 기능은 한 파일 내에 함수가 많을 경우 함수를 접어 보기 편하게 해 주는 기능이다.
다음은 폴딩 기능을 사용해 두 개의 함수를 접은 예다.

2장_vi와 vim 에디터

131

===== PAGE 133 =====
■:<：<«：•： b사나 •：•«»« -.•=.=•=江아Tuha
'.t 1t u- I h..l 가.'|
-；

RH기H|

int *mW) |
ch*r •스p;
int s, j：
iftt l 흐# ■ $trlw《오 tr)：

히: <▼, 4 bw< 유"BOE히|
:
t；m ：»b«.i
:
ri «■.'••"ef>¥MO뉴 1V
M心』:; W：

日
M
■'
■
:m

히

hit gtta_his(char *s>;
For (s*s» j"'.> 아i < Wtx MtSS ?«)<- les; j»*> {
if
s* «i으
ar§>F(i**] ” sp;
if (Is5Pau(*(：$tr*j)}} <
•(S-tF*j) - •='；
if tj ?- < M. "사<••!■?»
argufi+’J ■‘ sp：
師 « Str • J • i;

mt$c eMr >*gv[9HXJ)kl하}:
static char sti■{斗！?»]j

•— ZB 童': Slt M'H'-qUi I (---------------------------------- - ----------------ZXMtftne 11Km..DEB¥C
>-- j% 호: 2st MhHU} <------------------------------ =------------ -------—........... . ........

휴r'yvfi] • ■■；
rt*tvr* i;
r/M유 hip M쎄jsfaiiG
ini WlwllQ (
:iftt 호※:
struct «쪄.. struct. »«s：
uhll^ (1B&사 《
prill?»< 'W 3 ’•};
«?R5et<str. h. !；l"(iF《str)：);
조누헤

[그림 2-86] 폴딩 기능을 수행한 후의 모습

폴딩 기능으로 접으려는 함수의 시작 부분에 있는 ‘{’ 위에 커서를 두고 표준 모드에서

v]}zf 명령을 내리면 함수가 접힌다.
V]} 명령을 내리면 ‘{’ 기호를 기준으로 블록을 형성한다. 블록이 형성된 상태에서 zf 명
령을 내리면 함수가 폴딩된다. 위 명령이 어렵다면 그냥 V로 블록을 잡고 zf 명령을 내
린다.
접힌 함수를 펴는 방법은 접힌 부분에서 ??를 눌러주거나 ZO 명령을 내리면 된다.
이런 폴딩 명령은 다소 복잡하므로 ~/.vimrc 파일에 다음과 같은 내용을 추가해 단축
키를 지정하는 것이 좋다.
map <F1> v]}zf

위 내용을 추가하면 앞으로 £1] 키를 사용해 폴딩 기능을 이용할 수 있다.

I 함수의 원형과 지역변수의 선언 부분으로 바로 이동
ctags를 사용해 함수의 원형을 알면 되지만, ctags를 사용하지 않고 간단하게 함수의
원형을 알 수 있는 방법이 있다. 함수가 사용된 부분에 커서를 위치시키고 표준 모드에
서 [i를 누르면 화면 하단에 해당 함수의 원형이 출력된다.
그리고 지역변수가 선언된 부분으로 이동하고 싶을 때는 지역 함수 위에 커서를 두고
표준 모드에서 gd를 입력하면 지역변수가 선언된 위치로 이동한다.

132 2부_에디팅

===== PAGE 134 =====
I 여러 행 탭 끼워 넣기
여러 행의 앞부분에 탭을 일괄적으로 끼우거나 제거해야 될 때가 의외로 자주 발생한
다. 그럴 때는 다음 명령으로 해결할 수 있다.
[N]» 또는 [N]«

[N]은 현재 행 이하로 적용할 행의 범위를 말한다.〉〉는 행의 앞에 탭을 하나 더 둔다.
〈〈는 행의 앞에 있는 탭 하나를 제거한다.
아래 그림은 커서의 위치에서 7» 했을 때의 결과다.
三m
gtruct File_operdtions irrenote_.fop5 “ {
redd:
irre»Bte_reid.
write:
ope ii:
irrewte_epen.
release: irren(»te_reie«5e,
Inctl:
irreB®te_ioctl,

static iat irrenote init(uoid) {
H51,5

%희

[그림 2-87] 여러 행 탭 끼워 넣기의 예

탭을 끼워 넣을 파일의 범위가 넓어 도저히 셀 수 없다면 V를 이용해 블록을 지정하고
〉키나〈 키를 이용해 탭을 끼워 넣을 수 있다.

I 탭 사이즈 조정
리눅스 커널 소스는 기본적으로 탭 사이즈가 8 칸이다. 그리고 vim 의 기본 탭 사
이즈도 8 칸이다. 소스의 가독성을 위해 탭 사이즈 8 칸도 괜찮은 선택이다. 그러나

X-Windows 프로그래밍을 한다면 탭 사이즈 8 칸으로는 어림도 없다. XLib에서 사용
하는 함수명들이 모두 길뿐만 아니라 함수에 포함되는 인자의 개수도 만만치 않다. 그
때는 탭 사이즈를 알맞게 조절해야 한다.
탭 사이즈와 관련된 vim 변수에는 ts(tabstop), sw(shiftwidth), sts(softtabstop) 등
이 있다. ts 는 문서에 있는 ‘\f 문자를 몇 칸으로 보여줄지 결정하는 변수이고, sw 는
〉〉키 또는 « 키로 탭 사이즈를 조절할 때나 인덴트에서 자동 줄 맞추기를 할 때 사용
되는 화면 표시 크기다. 그리고 마지막으로 sts는 Tab 키를 눌렀을 때 표시되는 간격을
지정해 주는 변수다.

2장_vi와 vim 에디터 133

===== PAGE 135 =====
sw와 sts는 마음대로 바꿔도 상관은 없는데, ts만큼은 8로 되어 있지 않으면 인덴트 문제
가 발생하므로 가급적 8로 유지하는 것이 좋다. 탭 사이즈는 set 명 령으로 변수의 값을 바
꿔서 조정한다. 명령라인 모드에서 다음 명령을 차례로 내리면 탭 사이즈가 조정된다.
:set ts=8
:set sw=4
:set sts=4

실행 시마다 적용하게 하려면 ~/.vimrc 파일에 다음 내용을 추가하면 된다.
〔예제 2-9〕

set ts=8
set sw=4
set sts=4

파일의 종류마다 탭 사이즈를 별도로 지정하고 싶을 때가 있을 것이다. 예를 들면 html
소스, C 소스 파일, python 스크립트 파일이 있을 때 html 소스의 탭 사이즈는 ts=8,

sw=2, sts=2로 하고 싶고, C 스스는 ts=8, sw=8, sts=8로, 마지막으로 python 스크립
트는 ts=8, sw=4, sts=4와 같이 각각 다르게 지정하고 싶다고 하자.
그러면 각 파일마다 최상단이나 최하단에 각 소스 파일의 주석 형식으로 다음과 같이
넣어주면 vim이 파일을 열 때 알아서 설정한다.
html
C
python

<!—- vi: set ts=8 sts=2 sw=2: ——>
/* vi: set ts=8 sts=8 sw=8: */
# vi: set ts=4 sts=4 sw=4:

I 흐트러진 소스 정렬
간혹 소스를 마우스로 드래그해서 복사한 후 붙여넣었다면 ［그림 2-88］ 과 같이 소스가
흐트러지는 현상이 발생한다.

134 2부-에디팅

===== PAGE 136 =====
[그림 2-88] 마우스 드래그로 붙여넣기 해 소스가 흐트러진 예

위와 같은 현상이 나타나면 V로 블록을 지정하고 = 키를 누르면 소스가 깔끔하게 정 렬
된다.

[그림 2-89] 블록 지정 후 = 키를 눌러 정렬한 예

블록을 지정하지 않고 소스 전체를 정렬하는 방법은 표준 모드에서 다음과 같이 입력
하면 된다.
gg=G

| 행 번호 보여주기
vim에서 행 번호는 다음 명 령으로 간단하게 붙여줄 수 있다.
:set nu

2장_vi와 vim 에디터 135

===== PAGE 137 =====
[그림 2-90] 행 번호를 붙여준 예

I AM 문자 제거
MS 윈도우 시스템에서 작성된 파일을 유닉스 시스템의 vim에서 열면 다음과 같이 특수
한 문자가 찍혀서 나올 때가 있다.

[그림 2-91] AM 문자가 포함되어 있는 텍스트 파일

이런 현상이 일어나는 이유는 개행 문자가 MS 윈도우는 \r\n인데 반해, 유닉스 계열 운
영체제는 \n이기 때문이다.
위와 같은 현상이 발생하면 치환 명령으로 지워주거나 :set fileformat=dos로 설정해
준다.
치환 명령을 사용할 때는 AM 문자를 표현할 수 있어야 하는데, 히+v :Enter! 키를 누르
면 AM이 표시된다.
:%s/AM//g

위와 같이 명령을 내리면 깔끔하게 지워지는 것을 확인할 수 있다.
A

[ 문자는 CtrtJ+v Esc] 키고, A[[H~ 문자는 Ctrl]+v 日] 키, A[[12~ 문자는 으川+v F2]

키, ... 이런 식으로 각각의 특수 문자들을 지정할 수 있다.

136

2부_ 에디팅

===== PAGE 138 =====
I 파일에서 달라진 부분 비교하기
6부 “프로젝트 파일 버전 관리”에서 배우겠지만 CVS나 svn을 사용해 다수의 개발자가
프로젝트를 수행하다 보면 누가 어떤 부분을 수정 했는지 알지 못할 때가 발생한다. 그
럴 경우에는 diff 명령으로 원본 파일과 비교할 수 있지만 diff 명령은 결과가 텍스트 형
식으로 나오기 때문에 현명한 선택이 아니다. 이때는 vimdiff 명령을 이용하면 아주 멋
지게 비교할 수 있다.
먼저 실습을 위해 커널 디렉토리에 있는 COPYING 파일을 COPYING.ORG 파일로 복
사한다. 그리고 COPYING 파일을 열어 행을 지우고 추가하면서 원본 파일과 다르게
변경한다.
저장 후에 다음 명령을 내리면 달라진 부분이 일목요연하게 나타난다.
vimdiff COPYING COPYING.ORG

[그림 2-92] vimdiff 명령 수행 결과

파일의 달라진 점을 찾는 명령은 vimdiff도 있지만 m이d, xxdiff도 있다. 각자의 취향에
맞게 선택해 사용하면 된다.

2장_vi와 vim 에디터 137

===== PAGE 139 =====
I 헤더 파일 바로 읽어오기
소스 내에 사용된 헤더 파일을 키 한 번으로 읽어 들일 수 있다.

[그림 2-93] 헤더 파일 읽어 들이기 1

위와 같은 소스 파일이 있을 때 읽어 들일 헤더 파일명에 커서를 위치시킨다. 필자는

command.h 파일을 읽고자 한다. Ctrl|+wf 키를 누르면 창이 수평 분할되면서 헤더 파
일이 열린다.

[그림 2-94] 헤더 파일 읽어들이기 2

이때 path 변수에 경로를 지정하면 지정한 경로를 기준으로 헤더 파일을 찾는다. 그래
서 ~/.vimrc 파일에 다음과 같은 명령을 추가하면 vim 은 헤더 파일을 /usr/include 부
터 /work/book/utils_new/vim/linux-2.6.29/include까지 찾는다.
set path=/usr/include:/work/book/utils_new/vim/linux-2.6.29/include

Ctrl]+wf 명령은 헤더 파일에만 해당되는 것은 아니다. 커서 위치에 있는 문자열을 파
일로 인식하므로 헤더 파일뿐만 아니라 어떤 종류의 파일이던지 상관없이 열린다.

138 2부_에디팅

===== PAGE 140 =====
I 자동완성 기능 사용하기
함수나 변수의 일부만을 타이핑하고 *+p 나 Ctri]+n 키를 누르면 자동 완성 기능을
사용할 수 있다. 매우 긴 함수나 변수를 일일이 타이핑하지 않아도 되므로 자동 완성
기능은 유용할 때가 많다. EirD+p 키는 커서 위치에서부터 위로 자동 완성이 가능한
단어가 있는지 찾고, ctrli+n 키는 아래로 내려가면서 찾는다. 주로 %+n 키보다는

Ctrl|+p 키가 많이 사용된다.

I 정규 표현식에서의 매칭 문자 사용
간혹 정규 표현식으로 매칭한 문자를 치환 시 다시 사용하고 싶을 때가 있을 것이다.
예를 들면 다음과 같은 경우다.
aaa=YES
aas=NO

위와 같은 문자열들이 있을 때 다음과 같이 치환하려면 aaa= 뒤에 YES가 오는지 NO
가 오는지 알아야 한다.
ccc=YESz
ddd=YES
ccc=NO, ddd=NO

이 럴 때는 다음과 같이 치환 명 령을 사용한다.
:%s/aaa=\(YES\|NO\)/ccc=\l, ddd=\l/gc

6 [ 개발자들의 vim 설정
vim 을 처음 설치했을 때는 ~/.vimrc 파일 자체가 없기 때문에 vim 의 기본 설정만을
사용해야 된다. 물론 vim 의 기본 설정은 개발자가 사용하기에 다소 불편한 면이 있
다. 그래서 개발자들은 자신만의 ~/.vimrc 파일을 만들어 사용하는데, 다음은 필자의

~/.vimrc 파일 내용이다. 필자처 럼 사용해도 되고 독자가 직접 만들어 사용해도 된다.
독자가 직접 만들려면 vim 스크립트 작성법을 알아야 하는데, vim에서 ：help usr_41 이
라고 입 력하면 스크립트 작성법에 관한 매뉴얼을 볼 수 있다.

2장_vi와 vim 에디터 139

===== PAGE 141 =====
매뉴얼에는 if문, while문의 사용법이나 함수의 사용법, 변수의 선언법 등에 관한 내용
이 있고, 간단한 예제도 있으므로 vim 스크립트를 작성하는 데 도움이 된다.
〔예제 2-10)

~/.vimrc 예제

”============= 기본 변수 설정 =========

set cindent
set smartindent
set autoindent
set nowrap
set ff=unix
set bg=dark
set ruler
set path=/root/work/include,/usr/include,/usr/local/include,/
usr/src/include

============= key 매핑 ===========
map <F1> v] }zf
map <F2> zo
map <F3> : Tlist<crXC-WXC-W>
map <F4> :BufExplorer<cr>
map <PageUp> <C-UXC-U>
map <PageDown> <C-D><C-D>

’’=========== 인덴트 설정 및 제거 ===========

map ,noi :set noai<CR>:set nocindent<CR>:set nosmartindent<CR>
map ,sei :set ai<CR>:set cindent<CR>:set smartindent<CR>

=========== 파일 버퍼 간 이동 ==============

map
map
map
map
map
map
map
map
map
map
map
map
map

:b!KCR>
:b!2<CR>
:b!3<CR>
:b!4<CR>
,5 :b!5<CR>
,6 :b!6<CR>
,7 :b!7<CR>
,8 :b!8<CR>
z9 :b!9<CR>
,0 :b!10<CR>
:bn!<CR>
f Z :bp!<CR>
, w :bw<CR>

,1
,2
,3

" 1 번 파일 버퍼로 이동
" 2번 파일 버퍼로 이동
" 3번 파일 버퍼로 이동
" 4번파일버퍼로이동
" 5번 파일 버퍼로 이동
" 6번 파일 버퍼로 이동
" 7번파일버퍼로이동
" 8번 파일 버퍼로 이동
" 9번 파일 버퍼로 이동
" 10번파일버퍼로이동
" 다음 파일 버퍼로 이동
" 이전파일버퍼로이동
" 현재파일버퍼를닫음

========== ctags 설정 =============

140

2부— 에디팅

" 폴딩
" 폴딩 해제

’’ taglist
’’ BufExplorer

===== PAGE 142 =====
set tags=./tags,../tags,.•/•./tags,/usr/include/tags,/usr/local/
include/tags
if version >= 500
func! Sts()
let st = expand (’’<cword>’’)
exe "sts ’’. st
endfunc
nmap ,st :call Sts ()<cr>
func! Tj()
let st = expand("<cword>")
exe "tj ”.st
endfunc
nmap ,tj :call Tj ()<cr>
endif

••========== cscope 설정 ============
set csprg=/usr/bin/cscope
set nocsverb
cs add /work/book/utils_new/vim/linux—2.6.29/cscope.out
set csverb
set csto=0
set cst

func! Css()
let css = expand (’’<cword>")
new
exe ”cs find s ". css
if getline (1) == ’’ ’’
exe ”q! ’’
endif
endfunc
nmap ,css :call Css ()<cr>

func! Csc()
let csc = expand("<cword>")
new
exe "cs find c ". csc
if getline (1) == ’’’’
exe "q! ’’
endif
endfunc
nmap ,csc :call Csc()<cr>

2장_vi와 vim 에디터

===== PAGE 143 =====
"========== man page 설정 ===========
func! Man()
let sm = expand(”<cword>")
exe
”Iman
-S
2:3:4:5:6:7:8:9:tel:n:1:p:o
endfunc
nmap ,ma :call Man()<cr><cr>

"========== 인터넷 사전 설정 ==============

func! EEdic()
let sed = expand (’’<cword>")
new
exec ”r! eedic.sh ".sed
set nomod wrap
endfunc
nmap ,ed :call EEdic()<cr>gg

〔예제 2-11〕 /ijsr/local/bin/eedic.sh의 내용

#!/bin/sh
w3m -dump \
"http://kr.dictionary.search.yahoo.com/search/dictionaryp?p
=$l&subtype=eng" \
2> /dev/null \
I awk ’BEGIN { fig = 0 } \
/단어 더 보기/ | | /숙어/ | | /예문/ { fig = 0 } \
{\
if (fig) print $0 \
}/단어 \ (영한\)/ { fig = 1 } ' \

I sed ’ s/\[. *\]//g’ I sed 's/?//g’ I sed ’ s/단어장에 추가7/g ’ | sed
's/단어장에//g’ \
I sed -e *s/A추가'//g* | sed -e ’ s/A [ [: space :]]*([[: space: ] ] *$//g’
I sed ’s/D//g’ \
I sed ’s/()//g' | sed -e ’s/A[[:space:]]*)//g’ I sed ’s/<L//g’ |
sed -e ’ s/ [〔〕] //g’ \
I sed -e ’s/[[:space:]]*$//g’ I sed ’/A$/d’
echo "”

142 2부—에디팅

".sm

===== PAGE 144 =====
3
기타 편집기 소개

01 emacs
02 이클립스
03 gedit
04 KDev이op
05 anjuta

===== PAGE 145 =====
이번 장에서는 vim 외에 사용할 수 있는 편집기를 다룬다. 이번 장을 시작하면서 필자가
하고 싶은 말은 다음과 같다. 유닉스/리눅스 시스템에서 뭔가를 하기 원하는 독자라면 다
른 편집기에 앞서 vim 또는 emacs 중 하나를 선택해 먼저 익숙해지기 바란다.
유닉스/리눅스 시스템에서는 터미널에서 벗어날 수가 없다. 아주 오랜 세월 동안 터미널
이 있어왔고 그 세월 동안 터미널에 최적화되어 왔다. 터미널에서 마우스를 사용하지 않
고 개발에 최적화된 편집기를 사용해 빠른 속도로 개발하는 것은 유닉스/리눅스 시스템
개발자만이 가질 수 있는 특권이기도 하다.
어찌되었던 터미널 환경은 핵전쟁이 나서 세상의 모든 컴퓨터가 다 파괴되어도 지속
될 것이다. 첫 번째 컴퓨터가 만들어짐과 동시에 유닉스/리눅스 개발자들은 터미널부
터 만들 것이기 때문이다. 때문에 터미널의 CU 모드에서 사용 가능한 편집기 하나 정도
는 반드시 제대로 사용할 수 있어야 한다. 터미널에서 사용 가능한 편집기라면 vim 또는

emacs가 단연 최고라 말할 수 있다.

===== PAGE 146 =====
emacs
emacs는 vi만큼이나 역사가 깊고 훌륭한 편집기다. emacs는 Editing MACroS의 약자
로, 1976년에 GNU의 창시자인 리차드 스톨만과 가이 스틸, 데이브 문이 TMACS를 발
전시켜 만들었다.

emacs는 emacs만을 위한 책이 나와 있을 정도로 방대한 에디터이기 때문에 짧은 지
면으로 emacs의 진면목을 설명할 수는 없다. 이번 절에서는 emacs가 무엇이라는 것
정도로만 짚고 넘어가자.

File Edit OwLiuns Bufftms Tuuls C Help

O 醉 )c . 펴 •

.'

7

_______________
1r

_ 느 리 AW!
쳐《include (scheduler, h)

繼*

» Bmlude \process..h)
B #iiK；lude <uSYS» h〉

[그림 3-1] emacs 실행 화면

fil emacs의 특징
emacs 역시 마우스가 없는 시대에 만들어진 편집기이므로 키보드만으로 모든 일을 다
처리할 수 있다. 그런 면에 있어서 emacs와 어는 닮았다.
어가 키 조합을 통해 많은 명령을 처리하듯이 emacs 역시 많은 키 조합을 통해 명령을
처리한다. 그렇지만 emacs의 키 명 령은 정말 질리도록 많다. 앞서 필자가 설명한 vim
의 키 명령들은 많이 사용하는 키를 중점적으로 설명하였다. 설명한 키 외에도 수많은
키 명령이 vim에는 있다. 그러나 그런 모든 vim의 키 명령을 통틀어도 emacs의 5분의
3장_기타편집기소개 145

===== PAGE 147 =====
1 정도밖에 되지 않는다면 독자들은 emacs가 얼마나 많은 키 명령으로 이뤄졌는지 알
수 있을 것이다.

emacs는 수많은 키 명령만큼이나 많은 기능이 있다. vim이 편집기의 기본에 충실한 편집
기라면 emacs는 편집기의 기능 외에도 파일 관리, 디버거, 웹 브라우저, mail, ftp, news
리더 이외의 수많은 기능을 통합한 편집기를 가장한 프로그램이라고 말할 수 있다.
과거 이런 emacs를 두고 emacs는 편집기가 아니라 편집기를 가장한 운영체제라는 말
이 있었다. 그 말의 의미는 첫째로 emacs가 수많은 환경을 제공해 주었고, 둘째로 당시
에는 너무 많은 메모리와 디스크 공간을 사용할 정도로 emacs가 거대했기 때문이다.
실제로 emacs를 사용하는 사람 중에는 부팅 시 셸을 띄우는 대신 emacs를 띄우게 설
정해 놓은 사람들도 있다.

emacs의 다른 특징 .0.루.는 lisp 언어를 통해 기능을 추가할 수 있다는 점이다（ emacs에
서 사용하는 lisp을 elisp라 한다）. 그런 면에서 vim의 내장 스크립트와 비슷하다고 느
낄 수 있을지 모르지 만, elisp은 vim 스크립트보다 훨씬 많은 확장성을 제공한다.

@ emacs의 장단점
emacs의 장점은 앞에서 언급한 많은 기능과 elisp을 통한 뛰어난 확장성에 있다. 편집
기의 기능만을 놓고 볼 때 vim 에 있는 거의 대부분의 기능들은 emacs에 구현되어 있
다. 그리고 vim 에서 사용 가능한 플러그인들과 ctags 와 같은 프로그램들도 emacs에
모두구현되 어 있다.

emacs 의 단점은 많은 용량과 느린 속도에 있다. 수많은 기능이 내장되어 있는 만큼
emacs의 크기는 10메가 단위를 훌쩍 넘어간다. 대신 vim은 기껏해야 2메가 정도다. 이
런 많은 용량은 emacs를 임베디드 시스템 같이 작은 시스템에서 사용하기 어렵게 한다.
그리고 emacs 의 많은 기능은 elisp 로 구현되어 있는데, emacs 기동 시에 이런 elisp
스크립트들을 읽어 들이기 때문에 실행할 때 시간을 많이 소비해 실행 속도가 vim보다
는 훨씬 느리다.
유닉스, 리눅스 개발자 간에 있어 emacs가 좋은가 어가 좋은가에 대한 논쟁은 앞에서
설명 했듯이 치 열하게 벌어지곤 한다. 필자 역시 좋아하는 편집기가 있으나 종교 전쟁에
말려들고 싶은 생각이 없기에 중립의 자세를 고수하고자 한다. 다만 필자는 vim도 훌륭
한 편집기고 emacs도 훌륭한 편집기임에 분명한 사실이기 때문에 둘 중 어느 것을 선택하
든지 배워 볼 만한 가치는 있을 거라 생각한다.

146 2부_ 에디팅

===== PAGE 148 =====
2 L 이클립스
CLI 편집기로 vim 과 emacs 가 있다면 GUI 편집기에는 이클립스(eclipse)가 있다. 이
클립스 역시 어나 emacs 정도의 비중이 있고 책도 여러 권 나와 있다. 조그만 지면에서
이클립스를 소개하는 것은 이클립스에 대한 모독이다. 이클립스는 소개하는 책도 여러
권 나와 있을 정도로 비중 있는 편집기다. 때문에 이 절에서는 이클립스에 대한 간단한
소개 정도로 그치겠다. 이클립스에 대해 더 궁금한 독자는 이클립스만을 설명한 책을
보기 바란다.

I 이클립스 소개
이클립스는 IBM에서 개발해 오픈 소스로 공개한 IDE(통합 개발 환경)이다. 기본적으
로는 자바 프로그래밍을 위한 IDE로서 자바 기반으로 만들어졌으며, 따로 플러그인을
추가해 확장하면 C, C++, COBOL, Eiffel과 같은 언어도 지원한다.

[그림 3-2] 이클립스 실행 화면

3장_ 기타 편집기 소개

===== PAGE 149 =====
I 이클립스의 특징
이클립스는 UML 모델링, 디버깅, 단위 테스팅, 리팩토링, 그래픽 개발, CVS 연동 등 많
은 기능을 제공하며, 리눅스, 솔라리스, AK, HP-UX 둥의 유닉스 계열 플랫폼과, MAC

OSX, MS 윈도우즈 플랫폼에서 사용 가능하다.
vim, emacs와 같이 고대에 만들어진 프로그램이 아니기 때문에 기본적으로 GUI 기반
으로 만들어졌다.
이클립스의 많은 기능과 오픈 소스라는 장점 때문에 이클립스는 많은 부분에서 사용되
고 있다. 리눅스나 유닉스에서는 기본적으로 이클립스가 설치되어 있지 않다. http：//

www.eclipse.org에 가면 이클립스를 무료로 내려 받아 사용할 수 있다.

| 이클립스의 장단점
이클립스의 가장 큰 장점은 통합 개발 환경을 지원한다는 점이다. 이클립스를 사용하면
설계에서부터 코딩, 컴파일과 디버깅, 리팩토링까지 모두 이클립스 안에서 해결할 수
있다. 그리고 이클립스는 어나 emacs와는 다르게 근대에 만들어진 소프트웨어기 때문
에 인터페이스가 익숙해서 배우기 쉽다. 무엇이던 익숙한 것은 배우기가 쉬울 것이다.
그렇다고 어나 emacs가 배우기 까다로운 편집기라고 생각하지는 않는다.
단지 독자들이 근대에 나온 편집기에 너무 익숙해 어나 emacs를 사용할 때 생소함을
많이 느낄 뿐이라고 생각한다. 그런 면에서 볼 때 이클립스의 인터페이스는 따로 배우
지 않아도 될 만큼 쉽다.
다른 장점으로 이클립스는 오픈 소스로 공개됨으로써 개발 속도가 매우 빠르고 많은
기능을 플러그인 형식으로 지원한다는 점이다. 누구나 원한다면 이클립스의 개발에 참
여할 수 있으며, 또한 이클립스의 훌륭한 기능들을 무료로 사용할 수 있다.
이클립스가 편집기라고 해서 이클립스를 단순히 편집기로만 보면 안 된다. 이클립스는
하나의 잘 짜여진 프레임워크라 보는 것이 옳다. 세상에는 수많은 이클립스 기반 툴이
있다. 이런 툴들은 반드시 편집기 또는 IDE와 같은 형태일 필요는 없다. 빌드 또는 설정
유틸리티, 디버거, 모니터링 툴 등 수많은 툴을 이클립스 기반으로 제작한다.
이런 것들이 가능한 이유는 이클립스가 많은 확장성을 제공하기 때문이다. 이클립스 프
레임 워크를 이해하고 JAVA 프로그래밍에 능숙하다면 이클립스 프레임워크를 이용해
손쉽게 원하는 프로그램들을 만들 수 있다.
148 2부_에디팅

===== PAGE 150 =====
훌륭한 IDE 임에 의심의 여지가 없는 이클립스의 가장 큰 약점은 속도에 있다. 이클
립스는 자바 기반으로 만들어졌기 때문에 실행 속도가 느리다. 특히 리눅스 시스템은

X-Windows 시스템이 클라이언트'서버（ CS 구조） 구조를 가지고 있어 원래 윈도우즈 시
스템이 느린데다가 자바 가상 머신의 느린 실행 속도까지 더해져 더욱 느리게 느껴진다.
불과 5~6년 전만 해도 리눅스 시스템에서 이클립스를 돌리는 일은 웬만한 시스템에서
는 인내심 없이 하기 힘들었다. 현재는 컴퓨팅 파워도 매우 막강해졌고, JVM의 성능도
많이 개선되 었기 때문에 쓸 만하다고 본다.

3 gedit
gedit는 gnome 데스크탑 환경에서 기본적으로 제공하는 에디터다. gedit는 GUI 에디
터이면서 윈도우즈 환경에서 사용되는 에디터들과 인터페이스가 거의 동일하다. 때문
에 리눅스 시스템을 처음 사용하는 사람일지라도 편하게 사용할 수 있다.

[그림 3-3] gedit 실행 화면

사실 필자는 gedit를 거의 사용해 본 적이 없다. 이클립스는 플러그인을 개발하면서 사
용해 봤고, 앞으로 설명할 KDevelop는 오래전부터 유명하기 때문에 상당히 예전에 사
용한 적이 있지만 gedit는 어쩌다 gedit로 파일이 열리지 않은 이상 사용해 보지 않았다.

3장_기타편집기소개 149

===== PAGE 151 =====
그런데 필자가 gedit를 설명하는 이유는 도저히 유닉스/리눅스 편집기 환경에 적응하
기 힘든 독자라면 gedit도 있음을 알려주기 위해서다. gedit는 윈도우즈 환경에서 사용
하는 에디트 플러스와 인터페이스가 거의 동일하다.

04 【KDevelop
KDE에서 동작하는 GUI 애플리케이션을 개발할 때는 KDevelop 사용도 고려해 볼
만하다. KDevelop는 리눅스에서 사용 가능한 IDE다. C, C++, python, java, pascal,

fortran, ada, perl, php, ruby, sql, bash 셸 스크립트 등을 지원하고 인터페이스가 윈
도우즈의 VC 와 비슷하다.
현재까지 3.5.4 버전까지 나왔으며, 내부적으로 QT designer 같은 GUI 인터페이스를
생성하기 쉬운 툴들과 같이 사용하기 때문에 GUI 프로그램을 눈으로 보면서 쉽게 만들
수 있고, 프로그래밍, 디버깅, 배포를 위한 설치 스크립트를 모두 한 번에 만들 수 있어
매우 강력하다.

KDevelop는 GNU GPL을 따르기 때문에 무료로 사용할 수 있으며 , 페도라 배포판에
서는 기본적으로 KDevelop가 설치되기 때문에 손쉽게 사용할 수 있다.

[그림 3-4] KDevelop 실행 화면

150 2부_에디팅

===== PAGE 152 =====
05 【anjuta
KDE/QT 진영에서 사용 가능한 IDE에 KDevelop가 있다면 GNOME/GTK 진영에서
는 anjuta가 있다. anjuta는 페도라 기본 패키지로 설치되지 않기 때문에 http：//anjuta.

org/에서 내려 받아 설치 해야 한다.
glade와 같이 사용하면 GUI 애플리케이션용 IDE로 손색이 없으며, 소스 프로그램의
작성, 컴파일, 디버깅, CVS와의 연동 등을 지원한다.
Anjuta： /rootZanjuts~-'L2.2/sclntlila/Eator.cxy (Saved).

a «D
細 오 硏 펴 (고 허 >} Taos：«o
____
Swb의____________________
t> A Caret
t> ft CellBuffer
t> A Characterindexer
> tt CoiourAllocat»d
t ft ColourDesIred
t> ft Contractionstate
t> H DocMo혀flcatlon
0 Hl DocW하cher
b 倒 Document
|> H DocumentAcceasor
b 10 Documentindexer
0 A OynamicLIbrary
으 ■( OynamlcLlDrarylmpi
흐 Editor
0 AbandonPalntO
Q AddChar(char ch
Q A(»CharUTF(chai
□ BraceMatch<lnt t
S 0uttonOown(Poin
Q ButtonMoveCPoln
Q ButtonUtKPoInt p
O CancelMooesO
0 ChangeCaseOfSe
Q ChanoeSIzeO

으criewwppcri
[root@>s root]# |

3

AutoLlneLayout [554]

Etftor.cxx » 11 |EtftorJ)» [getilne.t:'

pdoc->Insertchar(pdoc-> Length(),
// Fad tha end of lines with spacoa if required

currentPos = PositionFromLineXd1ne? xlnsert)j
if (CXFromPosItlonCcurrentPos) < xlnsert) && (1 + i < Ten)) £
for (int 1=8； 1 < xlnsert - XFromPosltlon(currentPos)； 1++) £
pdoc->Insertchar(currentPos, ■〉；
currentPos++；
prevCr - ptr[1] -= •■.：：-•；
3 else £
pdoc->InsertStr1ng(currentPos, ptr +1, i)；
currentPos++；
prevCr - false；
3
}
pdoc-> EndUndoAct1on();
SetEmptySeiectlontposj；
^"rbool Editor：：CanPaste() {
return Ipdoc->IsReadOnly() a& ISelectlonContalnsProtectedf)；
Iwol d Editor： : Cl ear O £
if (currentPos -- anchor) €
if (1RangeContainsProtected(currentPosJ currentPos + i)) £
DelCharC)；

anjuta-4.2.2.
tar.
tar
cal I backs.c
cmic I -18e—1.1386. rpm

eci I pse-p I at form-3.0RC3-I Inux-tJtk.zIp kdevelop-3.0.4. tar
hanterm-xf-2.0.5-6.1386, rom
kdevelop-3.0.4.tar.bz2
i!i ksycu
k develop-3.OaS-l. 1386.rpin te@
Instaii.log

prlml 11 ves. c
src.tar

Jl

tacK [허 'watcheg—f
Project： anjuta

Zoom’ -2

Col： 025

■jobrBuiid'fi-oject Mode：'i5nlx7L?y

[그림 3-5] anjuta 실행 화면

MS 윈도우 환경의 IDE 를 이용한 개발에 익숙한 독자라면 KDevelop 와 anjuta 같
은 IDE 가 프로그래밍하는 데 익숙하고, 그래서 편하게 느껴질 것이다. 그렇지만

KDevelop 나 anjuta 같은 IDE 는 어나 emacs 를 완전히 익힌 후에 사용하는 것이 바람
직하다. 어나 emacs는 유닉스 개발자에 있어 이미 편집기 이상의 의미를 지니고 있는
유닉스의 철학을 담고 있는 편집기이기 때문이다. vi나 emacs를 이해하는 것은 유닉스
를 이해하는 데 도움이 된다.

3장—기타 편집기 소개

151

===== PAGE 153 =====
1 3부 I 컴파일과 링킹

===== PAGE 154 =====
4
gcc compiler

01 컴파일의 의미
02 알아 두면 정말 유용한 C 소스 컴파일 과정
03 gcc를 사용해 원하는 컴파일하기
04 gcc를 이용한 최적화 컴파일
05 기타알아 두면좋을만한것

===== PAGE 155 =====
Le/t's S*t•느dy
앞서 코딩을 위한 vim과 emacs 편집기 사용법을 알아봤다. 지금 당장은 번개 같은 손놀림
으로 멋지게 코딩하지는 못하겠지만 생각하는 바를 표현하는 데는 문제가 없을 것이다.
프로젝트를 위해 코딩을 했다면 컴파일해 실행 결과를 확인해야 한다. 이번 장에서는 컴
파일 과정의 의미는 무엇이고, 리눅스 시스템에서 컴파일 과정은 어떠하며, 어떻게 하면
잘 컴파일할 수 있는지 알아본다.
또한 컴파일과 직접 관련은 없지만 리눅스/유닉스 시스템 프로그래밍을 하면서 반드시
알아둬야 할 컴파일과 관련된 여러 유틸리티의 사용법과 원리도 알아본다.
이번 장에서 필자가 독자에게 알려주고자 하는 핵심은 컴파일하는 전체 과정을 이해해
컴파일 과정에서 문제가 발생했을 때 문제를 해결할 수 있는 능력과 컴파일러를 잘 다뤄
원하는 바이너리를 만들 수 있는 능력이다.
컴파일을 설명하기에 앞서 먼저 짚고 넘어가야 할 것이 하나 있다. 컴파일이라는 것은 결
국 컴파일러를 이용해 인간이 만든 코드를 CPU 가 이해할 수 있는 코드로 변경하는 과정
이다. 그렇기 때문에 당연히 아키텍처 종속적일 수밖에 없고 컴파일러마다 과정과 결과
가 다를 수 있다. 그래서 이번 장에서 설명할 컴파일러는 페도라 7 배포판과 우분투 7.04
배포판에 기본적으로 설치되는 gcc-4 丄 x 버전의 컴파일러로 설명한다. 또한 설명할 아
키텍처는 범용으로 자주 사용하는 인텔 i368 아키텍처와 임베디드 시스템에서 많이 사용
하는 ARM 아키텍처로 한정한다.

===== PAGE 156 =====
01 【컴파일의 의미
컴파일 과정 설명에 들어가기 전에 컴파일의 의미를 짚어보자. 흔히 말하기를 컴파일은
인간이 이해할 수 있는 형식 언어(C, C++ 등)로 작성된 소스 코드를 CPU가 이해할 수
있는 기계어로 번역하는 과정이라고 말한다. 그럼 기계어는 무엇이고 왜 기계어로 번역
해야만 하는 것일까? 이 문제에 대한 해답을 아는 것은 컴파일 과정의 의미를 이해하는
데 큰 도움이 된다.

I 인스트럭션과 어셈블리
기계어를 다른 말로 머신 인스트럭션(machine instruction) 즉, 기계 명령이라고 말하
기도 하고, 그냥 줄여 명령이라고 부르기도 한다. 명령이란 단어는 셸(shell) 명령과 다
소 혼동될 소지가 있으므로 앞으로 그냥 인스트럭션이라 부르기로 하자.
이런 인스트럭션은 01010101 같은 이진수로 이뤄진 숫자로 CPU의 종류마다 고유하며,

CPU가 특정 행동을 취하게 하기 위한 코드를 말한다. 가령 위에서 예를 든 01010101
은 i386 계열 CPU에게 “ebp 레지스터를 현재의 스택에 push하게 하는 인스트럭션”이
다. 각각의 인스트럭션은 어셈블리 코드와 1대 1로 대응하므로 숫자로 이뤄진 인스트
럭션을 역어셈블해 어셈블리 언어로 표현할 수 있고, 어셈블리 언어를 어셈블해 인스트
럭션으로 표현할 수 있다.
〔예제 4-1〕 like.c 소스 파일 내용

#include <stdio.h>
int main()
{
printf ("I like you!\n");
return 0;
}

［예제 4-1］ 과 같이 우리에게 이젠 너무나 친숙한 like.c 소스 파일이 있을 때 like.c
파일을 다음 명령으로 컴파일하면 like 실행 파일을 얻을 수 있다.
gcc

-g

-o

like

like.c

4장_ gcc compiler

155

===== PAGE 157 =====
우분투 사용자들은 다음 명령을 내려 컴파일 과정에 필요한 헤더 파일과 라이브러리를 먼저 설치하기
바란다.

sudo apt-get install build-essential

이런 like 실행 파일은 내부적으로 CPU에 명령을 내리기 위한 인스트럭션（명령）과 데
이터로 이뤄졌고 실제로 ［예제 4-2］ 와 같은 형식을 가진다.

IKES1 like 실행 파일의 내용
... 상략

080483a4 <main>
#include <stdio

.h>

int main ()
80483a4:
80483a8:
80483ab:
80483ae:
80483af:
80483bl:
80483b2:

80483cl:

8d 4c 24 04
83 e4 fO
ff 71 fc
55
89 e5
51
83 ec 04
"I like you!\n");
c7 04 24 aO 84 04 08
e8 f3 fe ff ff
0;
b8 00 00 00 00

80483c6:
80483c9:
80483ca:
80483cb:
80483ce:
80483cf:

83 c4 04
59
5d
8d 61 fc
c3
90

printf(
80483b5:
80483bc:
return

lea
and
pushl
push
mov
push
sub

0x4 (%esp),%ecx
$0xfffffff0,%esp
Oxfffffffc(%ecx)
% ebp
응esp,%ebp
%ecx
$0x4,%esp

movl
call

$0x80484a0,(%esp)
80482b4 <puts@plt>

mov

$0x0,%eax

add
pop
pop
lea
ret
nop

$0x4,%esp
%ecx
% ebp
Oxfffffffc(%ecx),%esp

}

... 하략

［예제 4-2］ 는 -g 옵션을 지정하고 컴파일한 like 실행 파일에 대해 objdump 명령을
다음과 같이 수행하면 볼 수 있다.
objdump -S like

156

3부— 컴파일과 링킹

===== PAGE 158 =====
［예제 4-2］의 결과는 페도라 7 배포판에서 gcc-4.1,2 버전으로 컴파일했을 때의 결과다. 컴파일에 사용
된 gcc 버전에 따라 결과가 약간씩 차이가 있을 수 있다.
예를 들면 다음 코드들은 gcc-4.1.x대 이상에서만 별도의 옵션을 주지 않아도 볼 수 있는데,

SSECStreaming SIMD Extension) 데이터 타입 지원을 위한 스택 재정렬(stack realign) 코드로,
gcc-4.1.x 이상 버전에서 gcc가 기본적으로 생성하는 코드다.
lea
and
pushl

0x4(%esp),%ecx
$0xfffffff0,%esp
Oxfffffffc(%ecx)

pop
pop
lea

응ecx
%ebp
Oxfffffffc(%ecx),%esp

이렇게 gcc 버전에 따라 컴파일한 결과가 약간씩 차이가 나는 것은 gcc 내부에 구현된 C 소스 파일을
분석하는 방법 및 최적화하는 방법, 그리고 컴파일러 정책이 버전별로 약간씩 차이가 나기 때문이다.

그러니 위 = 부분이 있건 없건 크게 문제가 있는 게 아니므로 자신의 코드가 필자와
다르다고 연연하지 말기를 바란다.

objdump 명령은 바이너리 파일의 정보를 보기 위한 명령인데, -S 옵션을 주면 like 파
일의 디버깅 정보와 함께 인스트럭션과 인스트럭션에 대응하는 어셈블리 코드를 함께
보여준다. ［예제 4-2］ 에서 디버깅 정보는 C 소스로 표현된 부분이고, 컴파일 시 -g 옵
션을 추가해야 볼 수 있는 부분이다.
여기서 맨 앞에 있는 16진수는 메모리의 주소이고, 중간에 있는 16진수 숫자 부분이 인
스트럭션이다. 그리고 인스트럭션 옆에 있는 코드가 인스트럭션과 대응하는 어셈블리
코드다. 어셈블리 코드는 실제로 들어있는 것이 아니라 objdump가 인스트럭션을 역
어셈해 어셈블리 언어로 알기 쉽게 보여준 것이다.

objdump -S like 명령으로 출력되는 실제 코드는 ［예제 4-2］ 보다 훨씬 긴데, 프로그
램의 = 위아래로 gcc 가 컴파일 과정에서 붙인 초기화 코드와 종료 코드가 들어가기
때문이다. 우리는 실제 C 코드 부분만 있으면 된다.

main() 함수의 80483ae번지를 보면 인스트럭션 0x55가 보일 것이다. 0x55 옆에는 어
셈블리 코드로 “push %ebp”라고 되어 있다. 즉, CPU는 0x55를 만나면 “현재의 스택에

ebp 레지스터를 저장”한다(0x55는 2 진수로 01010101이다). 마찬가지로 CPU가 다음
행의 인스트럭션인 0x89e5를 만나면 esp 레지스터의 값을 ebp 레지스터로 옮긴다.

4장_ gcc compiler

157

===== PAGE 159 =====
［예제 4-2］ 에서는 인스트럭션만 나타나 있고 데이터 부분은 표현되지 않았지만, 위 프
로그램에서 데이터 부분은 “I like you!\n”와 같은 문자열이다.

"I like you!\n” 문자열은 읽기 전용 데이터 공간Crodata 섹션)에 들어가는데, objdump -S like 명령
으로는 확인할 수 없고 objdump -s like 명령으로 확인 가능하다. objdump -s like 명령을 내렸을 때
출력되는 화면에서 “Contents of section .rodata” 부분에 “I like you!\n” 문자열이 들어있는 것을
확인할 수 있을 것이다. 섹션은 이후 더욱 자세히 설명한다.

전역변수를 사용했다면 전역변수의 공간이 잡히면서 데이터로 사용된다. like.c 파일을
컴파일해 얻은 실행 파일 like는 위와 같이 인스트럭션과 데이터로 이뤄져 있으며, 파일
의 내용을 16진수로 보여주는 xxd like 명령으로 like 파일을 읽어보면 실제로 인스트
럭션이 들어 있으을 확연히 알 수 있다.
기 root@os：/temp/like
0000310：
05e8
5589
0W0320:
0000330： b82c
0000340： allc
0000350:
83c0
WW36 0：
1c96
OW0370： C404
0000380： 5589
00W39O：
0000
0000380： d0c9
e551
00003b0:
00003c0： h R)8
00003d0:
5589
5589
O00O3e8:
00803FO： 0083
0000408:
45fo
0000410： 55F8
0000420：
8b45
0000430:
048b
0000440： dF83
0OW45 0： 5589
0000460：
0883
0000470： 75FU

7eff
FffF
e553 83ec
9504
082d
9604 0839
01a3 1c96
0408 39c3
5b5d c38d
e583 ec08
0000 85c0
c390 ［而
83EC 04c 7
0000 0000
e55d c38d
e557 5653
edc
e873
8d83 20FF
85d2 742b
1083 c781
4508 8904
c41c 5bse
e553 bb20
F8Ff
740c
83c4 045 b

585b
0480
2895
C376
0408
77e8
7426
a130
7409
2404
0424
83c4
7426
e85e
feFf
ffff
31FF
8944
24FF
5F5d
9504
83eb
5dc3

c9c3
3d20
8488
1F8d
FF14
c605
008d
9584
c784
83e4
a 884
0459
808d
ff8d
2945
89c6
2408
1683
c38b
0883
04ff
5589

9090
9604
Clf8
b426
8528
2096
bc27
0885
2430
F0fF
0408
5d8d
bc27
0081
8320
F0c1
8db6
8b45
C604
1c24
ec04
dO8b
e553

9090 9890
U..S....= .
-U?
0800 753F
.X.
028d BSFf
........... "( --------..............9.U___ &.
0000 0000
...........
9504 08a1
(0408 0183
____ 9.W —
0000 0000
U.................0. . .
t..
C074 12b8
9584 88FF
........................ 0.
71Fc '5589 셔
； ……L$.... •q .U.
.0................. $...
Fef f
e8f3
61Fc c390 |
......................V] .a
U..]..t&..
0000 0000
C315 1200
u..wus.*..
............ s____
FfFF fF89
E................. )E
7dF0 028b
•>
U...t+1...
0000 0000
0c89 4424
.E.....D$ .
E. -0$
.9 >.u
397d F075
..E.
C390 9090
$■
U..S..................
a120 9584
....t...................
0383 F8FF
u....[].U.
S.
83ec 84e8

-I

:|

［그림 4-1］ like 실행 파일에서 실제 인스트럭션의 위치

［그림 4-1］ 과 같이 like 실행 파일에 objdump 로 본 main() 함수의 인스트럭션이

0x8d4c2404 0x83e4fo 0xff71fc… 형식으로 들어있음을 확인할 수 있고, 그 중에는
“push %ebp”, “mov %esp,%ebp”에 해당하는 0x55, 0x89e5도 들어 있음을 확인할 수
있다. 그런데 인스트럭션이 objdump 와 xxd 로 보이는 것처럼 16 진수로 표기된 것은
아니다. like 실행 파일은 하드디스크에 들어 있고 하드디스크는 자화 물질의 방향에 따
라서 0과 1로 데이터를 저장하기 때문에 실제로는 2진수가 들어있는 것이다. 단지 사람
이 보기 쉽게 objdump와 xxd가 16진수로 보여준 것일 뿐이다. 그러므로 우리는 0x55
의 경우 실제로 0101 0101 형태로 하드디스크에 저장되어 있음을 알 수 있다.

158 3부- 컴파일과링킹

===== PAGE 160 =====
Direction of current

[그림 4-2] 하드디스크에 저장된 모습

이렇게 자화 물질의 방향에 따라 저장된 인스트럭션은 나중에 코일로 이뤄진 하드디스
크의 헤더에 의해 읽혀질 때 유도 전기를 발생시킨다. 그래서 전압의 유무에 따라 1과

0이 표현되어 RAM에 정보가 저장된다. *
이제 CPU가 해석할 수 있는 인스트럭션（기계어）이 2진수란 것을 알았고, 실행 파일은
이런 인스트럭션과 데이터로 이뤄졌음을 알았다. 그럼 왜 하필 인스트럭션은 2진수여
야 할까? 그리고 왜 CPU는 0과 1만 있는 2진수만을 이해할 수 있을까?

I 0과 1밖에 모르는 CPU
앞서 실행 파일을 아주 무자비하게 해부해 실행 파일이 어떻게 구성됐는지 알았다. 물
론 실행 파일의 구조에 대한 이야기는 이것이 전부는 아니다. 나머지 내용은 ELF 바이
너 리 포맷을 설명할 때 하겠다.
실행 파일을 해부하면서 느낀 근본적인 의문은 “왜 CPU는 0과 1밖에 모르는가?”이다.
이에 대해 알려면 먼저 0과 1의 의미를 확실히 알아야 한다. 그러려면 기존의 논리적인

0과 1의 의미에서 벗어나 물리적인 0과 1의 의미를 알아야 한다. 그러면 기존의 뜬구름
잡는 것 같은 0과 1은 지워버리고, 물리적인 0과 1의 의미를 알아보자.

4장_ gcc compiler 159

===== PAGE 161 =====
CPU는 다음과 같은 요소로 구성되어 있다.

OR 게이트

AND 게이트

NOR 게이트

NOT 게이트

［그림 4-3］ 논리회로

［그림 4-3］ 의 요소들을 논리회로라 하고, 소위 말하는 반도체를 의미한다. 물론 논리
회로가 위 그림과 같이 생긴 것은 아니다. 이해하기 쉽게 위와 같은 기호로 논리회로를
표현했을 뿐이다. 위와 같은 논리회로는 주로 실리콘（규소 Si） 에 불순물（갈륨이나 인
듐）을 섞어 만든 반도체를 기본 소자로 해서 만든다.
［그림 4-3］ 에는 설명을 간단히 하기 위해 OR, AND, NOR, NOT 게이트밖에 보이지
않았는데, 실제로는 위와 비슷한 종류의 논리회로로 NAND, XOR, XNOR 등 여러 가
지 타입이 더 있다. 여기서 “반도체”라는 단어의 의미를 짚어보는 것은 정말 중요하다.
도체가 전기를 잘 통과시키는 물질이고, 부도체가 전기를 잘 통과시키지 않는 물질이라
면 반도체는 특정 상황에서 전기를 잘 통과시키지만, 그렇지 않은 상황에서는 전기를
통과시키지 않는 물질을 말한다.

AND, OR, NOR 등의 게이트도 이런 반도체들을 조합해 만드는데, AND 게이트를 예
로 들면 AND 게이트는 A, B 양극에 전압이 동시에 인가되어야만 C 쪽으로 전압이 인
가되고 A, B 양극 중 어느 한쪽이라도 전압이 인가되지 않으면 C 쪽으로 전압이 인가
되지 않는 특성을 가지고 있다.
이에 비해 OR 게이트는 A, B 양극 중 어느 한 극이라도 전압이 인가되면 C 쪽으로 전
압이 인가되고 A, B 둘 다 전압이 인가되지 않으면 C 쪽으로 전압이 인가되지 않는 특
성을 가진다.

NOR 게이트는 OR 게이트와 반대로 A, B 둘 다 전압이 인가되지 않을 경우 C 쪽으로
전압이 인가되고 A, B 양극 중 어느 한쪽이라도 전압이 인가되면 C 쪽으로 전압이 인
가되지 않는다. 그런 의미에서 반도체란 전기적으로 제어가 가능한 “스위치”라고도 말
할수있다.

160

3부_ 컴파일과 링킹

===== PAGE 162 =====
여기서 전압이 있다는 말은 논리 T을 의미하고, 전압이 없다는 말은 논리 ‘0’을 의미한
다. CPU 내부는 위와 같은 반도체로 이뤄진 논리회로들이 복잡하게 엮어져 연산을 위
한 연산장치와 제어를 위한 제어장치 등으로 이뤄진다. 결국 다른 시각으로 보면 CPU
는 전기적으로 제어가 가능한 여러 특성을 갖는 전기적 스위치가 복잡하게 연결되어
연산을 위한 연산회로를 이루고, 제어를 위한 제어회로를 이뤄 이런 회로들이 유기적으
로 연결된 장치라고 볼 수 있다.

[그림 4-4] 8Bit CPU 연산장치 회로 일부분

CPU는 위와 같이 논리회로들로 구성된 장치이므로 ‘0’과 T밖에 모르는 장치고, 우리
는 이런 CPU에게 명령을 내리기 위해 C 소스를 컴파일해 0과 1로 이루어진 바이너리
파일로 변환하는 것이다.
이전에 보았던 스택에 “ebp 레지스터를 push”하는 인스트럭션은 16진수로 0x55였고,
하드디스크에서 자화 물질의 자기장 방향에 따라 2진수 0101 0101로 되어 있다는 것
을 배웠다. 이런 0101 0101은 like 프로그램을 실행시킬 때 하드디스크의 헤더가 읽어
메모리에 올리는데, 메모리에서는 ‘0’이 전압이 없는 상태, T이 전압이 있는 상태로 저
장된다.
4장_ gcc compiler 161

===== PAGE 163 =====
이후 CPU 가 인스트럭션을 실행하기 위해 메모리에서 인스트럭션을 가져오면 결국

0101 0101O] CPU에게 전달되는데, 그 말은 데이터 버스 선들을 따라 전압이 없고, 있
고, 없고, 있고, 없고, 있고, 없고, 있고 한 신호가 CPU에 입력됨을 의미한다. 전기적 스
위치로 이뤄진 CPU는 이런 신호를 받으면 현재의 스택에 ebp 레지스터를 push한다.
컴파일 과정은 이렇게 인간이 이해하는 언어를 CPU가 이해하는 인스트럭션으로 변환
하는 과정이고, 그 과정에는 다소 복잡한 절차를 거친다. 컴파일러를 잘 사용하려면 이
런 컴파일 과정을 반드시 이해해야 한다. 그러면 리눅스 시스템에서 컴파일 과정은 어
떤 절차로 어떻게 이뤄지는지 알아보자.
Tip 여
가끔 CPU를 보면서 어떻게 만드는지 궁금했을 독자들이 있을 것이다. CPU를 만드는 과정을 간단하게
설명하면 다음과 같다.

1. 기본 원료가 되는 실리콘 단결정 기둥（잉곳이라 부르기도 한다）을 잘라 얇은 원판의 웨이퍼로 만든다.
2. 웨이퍼를 연마해 매끈하게 만든다.
3. 웨이퍼 판을 고온의 산소와 반응시켜 얇은 실리콘 산화막（산화막은 부도체임）을 생성한다.
4. 빛에 반응하는 물질인 감광액（PR）을 웨이퍼에 바른다. 이런 감광액은 필름에 사용되는 감광액과 유
사해 나중에 현상하면 빛을 쪼여준 부분은 없어지고 쪼이지 않은 부분은 감광액이 그대로 남는다.

5. 감광액을 바른 웨이퍼에 회로 모양을 그린 유리판을 대고 자외선을 쪼여준다.
6. 웨이퍼를 현상하면 빛을 받은 부분의 감광액은 사라지고 받지 않은 부분은 감광액이 남아 웨이퍼에
회로 모양（패턴）이 생긴다.

7. 회로가 찍힌 웨이퍼에 산화막을 녹이는 가스를 분사하면 감광액이 묻어 있지 않은 부분만 산화막이
사라지고 감광액이 묻어 있는 부분은 산화막이 남는다.

8. 감광액을 모두 없애고 산화막이 사라진 부분에 불순물을 주입한다（이 부분이 반도체가 된다）.
9. 불순물을 주입한 부분에 알루미늄 이온을 분사하거나 구리 기둥을 세워 배선한다.
10. 3에서 9의 과정을 반복하면서 여러 층의 회로를 형성한다.
11. 회로가 다 만들어진 원판의 웨이퍼를 칩 단위로 자른다.
12. 마지막으로 잘라진 조각들을 칩의 다리에 해당하는 부분에 배선하고, 칩의 껍질에 해당하는 부분으
로 패키징해 시중에서 볼 수 있는 CPU와 같은 형태로 만든다.
CPU는 위와 같은 과정으로 만들어진다. 복잡하게 생각할 필요 없이 웨이퍼에 사진을 찍는 것과 같은
원리로 아주 미세하게 제어장치, 연산장치와 같은 회로를 웨이퍼에 찍어 넣는다고 생각하면 될 것이다.
좀 더 자세한 내용을 알고 싶은 독자는 인터넷에 검색해 보기 바란다. 실제 사진과 함께 그림으로 자세
히 설명해 놓은 자료를 많이 찾을 수 있을 것이다. 분명하게 말할 수 있는데, 흥미롭고 재미있을 것이다.
『반도체가 꼭 져기적으로만제0?가능한스위치일까?
반도체가 반드시 전기적으로만 제어 가능한 스위치를 의미하는 것은 아니다. 기본 소자와 첨가되는 불
순물의 종류에 따라 빛이나 열에너지에 의해 제어 가능하기도 한다. 이렇게 빛이나 열에너지에 의해 도
체 성질을 가지는 것도 반도체라 부른다.

162 3부—컴파일과링킹

===== PAGE 164 =====
02 J갈아두면정말 유용한 C 소스
컴파일과정
컴파일은 단순히 컴파일러 옵션 몇 개를 더 안다고 잘하게 되는 것은 아니다. 컴파일을
잘하려면 컴파일 과정이 어떻게 이루어지는지 반드시 이해해야 한다. 필자가 이 절에서
컴파일 과정을 알려주려는 이유는 컴파일 과정을 이해하면 C 소스가 제대로 컴파일되
지 않을 때 문제를 해결할 수 있는 능력을 키울 수 있고, 원하는 바이너리를 쉽게 만들
수가 있기 때문이다.
필자는 이번 과정이 이 장 전체에서 가장 중요한 부분이라고 생각한다. 다소 지루할지
도 모르지만 컴파일 과정을 이해하고 나면 프로그래밍 실력이 한 단계 성숙된 것을 느
낄 수 있을 거라고 확신한다. 먼저 앞으로 사용할 gcc 컴파일러를 설명한다.

I C 소스의 전체 컴파일 과정
gcc는 GNU에서 만든 C 컴파일러다. 수많은 옵션만큼이나 기능이 풍부해 원하는 바이
너리를 쉽게 만들 수 있으므로 애플리케이션뿐만 아니라 운영체제, 부트로더 등도 다른
컴파일러에 비해 쉽게 만들 수 있다.
또한 gcc는 현존하는 어떤 컴파일러보다 많은 CPU 아키텍처를 지원한다. ARM, DEC,

AVR, i386, PPC, SPARC, M68XX 등 수없이 많은 아키텍처를 지원하기 때문에 원하는
어떤 CPU의 크로스 컴파일러도 쉽게 찾아 사용할 수 있다.
: 소문자 gcc와 대문자 GCC는 의미가 다르다. 소문자 gcc는 GNU C Compiler의 약자로 말 그대로

GNU C 컴파일러를 의미하고, 대문자 GCC는 GNU Compiler Collection의 약자로 C 컴파일러인
gcc와 C+ + , 자바, ada, Fortran, Objective-C 컴파일러들을 포함하는 컴파일러의 묶음을 의미한다.
※ 필자가 앞으로 이 책에서 gcc라 표기한 것은 모두 다음에 설명할 /니sr/bin/gcc인 C 컴파일러 드라
이버를 의미하고, GCC라 표기한 것은 gcc를 포함하는 GNU Compiler Collection의 각 언어 컴파
일러 드라이버를 통칭하는 것임을 유념하기 바란다.

4장_ gcc com메er

163

===== PAGE 165 =====
/usr/bin/gcc가 C 컴파일러라고 해서 C 소스만을 컴파일할 수 있는 것은 아니다. C++
소스도 컴파일할 수 있고, 심지어 Fortran, ada, Objective-C, JAVA도 컴파일할 수 있
다. 그것은 gcc의 구조적 특성 때문에 가능한 일이다. 그럼 gcc는 어떤 구조적 특성이
있기에 이렇게 여러 언어를 컴파일할 수 있는 것일까?
흔히들 /usr/bin/gcc가 C 컴파일러라고 알고 있겠지만 정답을 이야기하자면 엄밀한
의미에서 /usr/bin/gcc는 C 컴파일러가 아니다. 방금 앞에서 GNU에서 만든 C 컴파일
러라고 말해 놓고 다시 C 컴파일러가 아니라고 말하니 필자가 가증스럽겠지만 엄연한
사실이다.

/usr/bin/gcc는 내부적으로 전처리기인 cppO 또는 ccl -E 명령을 호출해 전처리 과
정을 수행하고, 진짜 C 컴파일러인 호풔' 호출해 컴파일한 후 어셈블러안^’ 호출해
목적 코드로 만들고, 마지막으로 링커를 호출하는（헤그夢 호출하여 collect》가 내
부적으로 링커인 Id를 호출해 라이브러리와 링크해 실행 파일로 만들어낸다.
즉, gcc는 실제 컴파일 과정을 담당하지 않고 전처리기와 C 컴파일러, 어셈블러, 링
커를 각각 호출해 주는 역할만 담당한다. 이렇게 각각의 컴파일 과정에 필요한 명
령을 순차적으로 호출해 주는 것을 컴파일러 드라이버 （ compiler driver） 라 부르고,

/usr/bin/gcc는 C 컴파일러 드라이버에 해당한다. gcc가 C 컴파일러 드라이버라
면 그럼 진짜 C 컴파일러는 무엇일까? 진짜 C 컴파일러는 /usr/libexec/gcc/i386-

redhat-linux/4.1.2/cc!을 들 수 있다（우분투 7.04의 경우 /usr/lib/gcc/i486-linux.gnu/4.1.2/ccl 이다）.
/usr/libexec/gcc/i386-redhat-linux/4.1.2 디렉토리에는 여러 실행 파일이 있는데,
각 실행 파일의 역할은 다음과 같다.

• ccl： C 컴파일러, -E 옵션을 붙이면 C 전처리기로 동작
• cclplus： C++ 컴파일러, -E 옵션을 붙이면 C++ 전처리기로 동작
• collect2: 링커（내부에서 링커인 Id를 호출해 링크함）
、/、Z、Z、Z丁/W으〜/〜'~
f951： 포트란 컴파일러
〜XZ

•

164 =_컴파일과링킹

===== PAGE 166 =====
우 페도라 7의 경우 cc1 은 /usr/libexec/gcc/i386-re하W-linux/4.1.2 디렉토리에 들어있고, 우분투

7.04의 경우에는 /usr/lib/gcc/i486-linux-gnu/4.1.2 디렉토리에 들어있다. 배포판 종류마다 cc1 이 있
는 위치가 다르고, 들어있는 파일의 종류도 다를 수 있다. 이는 gcc를 빌드할 때 지정한 설정에 의해 바이
너리가 설치될 위치라든지 지원할 언어의 종류가 달라 설치되는 바이너리 종류가 달라지기 때문이다.
아래에는 페도라 배포판에서 컴파일러가 있는 디렉토리에 포함될 수 있는 바이너리 종류를 기술한 것이다.

. • cppO： 전처리기（예전에 사용됨. 현재는 컴파일러에 전처리 과정이 통합됨）
/ • cd ： C 컴파일러, -E 옵션을 붙이면 전처리기로 동작
• cdobj： Objective-C 컴파일러, -E 옵션을 붙이면 전처리기로 동작
• cdplus： C++ 컴파일러, -E 옵션을 붙이면 전처리기로 동작
•

f771： 포트란 77 컴파일러

• f951: 포트란 95 컴파일러
• jd: 자바 네이티브（native） 컴파일러
• collects 링커（내부적으로 진짜 링커인 Id를 호출함）
乂 • Id： 링커（실제로는 포함되지 않지만 Id가 실제 링커이기에 설명）

그리고 /usr/bin 디렉토리에 가보면 다음과 같은 파일들이 있는데, 이는 컴파일러 드라
이버들이다.

• cc： C 컴파일러 드라이버, gcc와 동일
•

gcc： C 컴파일러 드라이버

• C++： C++ 컴파일러 드라이버, g++와 동일
• g++： C++ 컴파일러 드라이버
• gcj： 자바 컴파일러 드라이버（페도라 7의 기본 설치에서는 포함되지 않음）
각각의 컴파일러 드라이버 간에는 다소 경계가 모호한 편이다. 무슨 말인고 하니 컴파
일러 드라이버는 전처리기, 컴파일러, 어셈블러, 링커를 각각 호출해 주는 역할만 담당
하기 때문에 컴파일 과정에서의 비중은 그렇게 크지 않다. 그리고 컴파일러 드라이버는
어떤 언어로 작성된 소스 파일이 있을 때 소스 파일의 확장자를 해석해서 비록 자신이
지원하는 언어의 소스가 아닐지라도 해당 소스에 맞는 전처리기와 컴파일러를 호출해
주기도 한다.
때문에 gcj 자바 컴파일러 드라이버로 C++ 소스를 컴파일할 수 있고, gcc C 컴파일러
드라이버로 C++ 소스를 컴파일할 수도 있다. 물론 이때는 gcc와 gcj가 C++ 전용 컴파
일러 드라이버가 아니므로 C++ 소스를 컴파일하기 위해 기본적으로 요구되는 라이브
러리를 알지 못해 -lstdc++ 옵션을 컴파일 명령 시 추가해 주지 않으면 오류를 출력하
겠지만 말이다.

4장_ gcc compiler

165

===== PAGE 167 =====
［그림 4-5］ 는 like.c 소스 파일이 있을 때 gcc C 컴파일러 드라이버가 like.c 파일을
어떤 과정을 통해 컴파일하는지 그림으로 나타낸 것이다.

［그림 4-5］

gcc 컴파일 과정

［그림 4-5］ 에서 gcc는 cppO 또는 ccl -E를 호출해 전처리 과정을 거쳐 like.c 파일을

like.i 파일로 만든다. like.i 파일은 C 컴파일러인 ccl에 의해 어셈블리 코드인 like.s로
컴파일되고, 이후 like.s는 as 어셈블러에 의해 어셈블 과정을 거쳐 like.o 오브젝트 파
일로 만들어진다.

like.o 파일은 다시 collect》가 링커인 Id를 호출한 후 libc.a 같은 표준 C 라이브러리와
링크해 최종적으로 실행 파일인 like 파일을 만든다. gcc에 의한 C 소스 컴파일 과정
은 크게 이런 방식으로 이뤄진다. like.c가 C 소스가 아니라 like.cpp 같이 C++ 소스였
다면 전처리 과정에 생성되는 파일이 likej가 아니라 likeji이고, ccl C 컴파일러 대신

cclplus C++ 컴파일러가 사용된다.
독자의 이해를 돕기 위해 실제로 이런 컴파일 과정이 일어나는지 직접 확인해 보자.
먼저 기존에 사용하던 like.c 파일이 ［예제 4-3］ 과 같이 있다.
(예제 4-3〕

like.c 소스 파일 내용

★include <stdio.h>

；

int main()

:

{

i
printf("I like you!\n");
return 0;

}

166 3부—컴파일과링킹

;
；
：

===== PAGE 168 =====
그리고 다음 명령으로 컴파일한다.
gcc -V -save-temps -o like like.c

위 명령에서 -v 옵션은 컴파일되는 과정을 화면으로 출력하라는 옵션이고丁temgp
옵션은 컴파일 과정에서 발생되는 중간 파일을 지우지 않고 저장하라는 옵션이司厂

gcc는 컴파일 과정 시 생성되는 전처리 파일(hke.i)과 어셈블리 파일(like.s), 오브젝트
파일(like.o)을 /tmp 디렉토리에 생성하고 지워 버리는데, -save-temps 옵션을 지정
하면 중간에 생성한 파일을 지우지 않고 현재 디렉토리에 저장한다. 위 명령을 내리면
［그림 4-6］ 과 같은 메시지가 출력됨을 확인할 수 있다.
廢] root@os ：/temp/like

=Idl ..시서

[root@os like]tt gcc -u -saue-temps -o like like.c
Reading specs From /usr/lib/gcc/i386-redhat-linux/4.1.2/specs
Target: i386—redhat-linux
Configured with: . ./configure ——preFix=/usr --mandir=/usr/share/man --info
dir=/usr/share/info ------------------------------------------------ ——一一enable-checki
ng=release —— --enable-____________________________________________ ——
ceptions --enable-languages=c,c++,objc,obj-C++,jaua,Fortran,ada --enable-j
aua—awt=gtk --disable-dssi -------------------------------------------------- --------------------------------------------------------------------aua-1.5.0-gcj-1.5.8.8/jre --------------------------------------------------------------------------------- enable-jaua-maintain
er—node----------------------------------------------------------------------------------------------- .jar--------------------------------------------—
Thread model: posix
gcc uersion 4.1.2 28870925 (Red Hat 4.1.2—27)
______________ ___________________
/usr/libexec/gcc/i386-redhat—linux/4.1.2/cc1
-E
-quiet
-u
like.c
-mtune=g
eneric -fpch—preprocess -o like .i____________________________ _______________________________________
ignoring nonexistent directory "/us»-/lib/gcc/i386-redhat-linux/U.1.2/../..
/../. ./i386-redhat-linux/include"
ttinclude "_______ " search starts here:
ttinclude <_______ > search starts here:
/usr/local/include
/usr/lib/gcc/i386-redhat—linux/4.1.2/include
/usr/include
End of search list.
•
________________________ ____________
/usr/libexec/gcc/i386—redhat-linux/4.1.2/cc1 -fpreprocessed like.i -quiet
—dumpbase like.c -iitune=generic —auxbase like —uersion -o like.s________________________________ _
GNU C uersion 4.1.2 20070925 (Red Hat 4.1.2-27) (i386-redhat-linux)
compiled by GNU C uersion 4.1.2 20876925 (Red Hat 4.1.2-27).
GGC heuristics: param ggc—min-expand=64 ----------------------------------------- ---Compiler executable checksum: 53c9f9515bF7a4d930482540205071F7
as -U -Qy -o like.o_like.g
GNU
assembler
uersion
2.17.50.0.12-4
(i386-redhat-linux)
using
BFD
uersion
2.17.58.0.12-4 20B78128__三丄.… ...................... ___ _
__________ __________________
/usr/libexec/gcc/i386-redhat-linux/4.1.2/collect2 ——eh-frame—hdr -m elF_i
386 ------------------------------------- -dynamic-linker /lib/ld-linux.so.2 -o like /usr/lib/g
cc/i386-redhat-linux/4.1.2/../crtl.o /usr/lib/gcc/i386—redhat-linux/
4.1.2/../ct-ti.o /usr/lib/gcc/i386-redhat-linux/4.1.2/crtbegin.o -L/u
sr/lib/gcc/i386-redhat-linux/4.1.2 -L/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2/.like.o -Igcc ——as-needed l g c c _ s - - n o - a s - n e e d e d - 1 c - I g c c a s - n e e d e d - l g c c _ s — — / u s r / l i
b/gcc/i386-redhat-linux/4.1.2/crtend.o /usr/lib/gcc/i386-redhat-linux/4.1.
2/...1../crtn.으
_____________________________________
[root@os like]#-]

［그림 4-61 like.c 컴파일 메시지

［그림 4-6］ 에서 확인할 수 있듯이 gcc는 내부적으로 ccl -E와 ccl, as, collect』를 각
각 호출함을 알 수 있다. 그리고 -save-temps 옵션에 의해 1s 명령을 내리면 컴파일
중간 과정에서 생성된 Uke.i 파일과 like.s 파일이 보존되었음을 확인할 수 있다.

4 장_ gcc compiler 167

===== PAGE 169 =====
[그림 4-7] 컴파일 과정에서 생성된 like.i 파일과 like.s

like.i 파일과 like.s 파일을 각각 열어보면 like.i
파일은 전처리 과정이 끝난 C 소스 파
- ------------------- —------- ---------- ---------일이라는 것을 알 수 있고, Jike.s 파일은 컴파일 과정을 거친 후의 어셈블리 파일이라
는 것을 확인할 수 있다.

extern int ftrylockFile (FILE *_stream) _attribute_ ((_nothr
ow_)) ；

extern uoid Funlockfile (FILE *_stream) _attribute_ ((_nothrH
ow__))；
tt 858 ”/ysr/include/stdio.h" 3 却
tt 2 "like.c” 2
int main()
printFC I li" you?to”);
return
g
"like-i" 933L, 18fl46c

[그림 4-8] 전처리 과정이 끝난 like.i 파일의 내용

[그림 4-9] 컴파일 과정이 끝난 like.s 파일의 내용

168 3부_컴파일과링킹

I
933,1

바닥JB|

===== PAGE 170 =====
이런 like.i 파일과 like.s 파일은 컴파일 중간 과정의 산물로서 컴파일러 오류로 인한
문제나 전처리 과정에서의 오류로 인한 문제가 발생했을 때 유용하게 사용할 수 있다.
예를 들면 다음과 같은 상황이다.
〔예제 4-4〕 like.h 소스 파일 내용

struct

my_struct
int a;

{

} my;
#define my MY

〔예제 4-5〕 like.c 소스 파일 내용

#include <stdio.h>
#include "like.h"
int

main()

{
my.a = 0;
printf("I like you! my.a = 응d\n", my.a);
return 0;
}

여러분은 위와 같은 코드가 왜 문제인치 단번에 알 수 있을 것이다. like.h 에서 my_

struct 타입의 구조체 my를 정의했는데, 바로 밑에서 define으로 인해 앞으로 my로 쓰
는 모든 문자는 MY로 대체된다. 그래서 like.c에서 my를 사용하면 전처리 과정 내에서

MY로 치환되어 버리므로 "가 정의되지 않아 컴파일 오류가 발생한다.
그럼 위 예제들을 컴파일하면 어떤 오류 메시지가 출력될까? 똑똑한 gcc가 알아서 위
예제의 어떤 부분에 문제가 있다고 알려줄 수 있을까? 다음은 컴파일 메시지다.

[그림 4-10] gcc 오류 메시지

4장_ gcc compiler

169

===== PAGE 171 =====
당연하게도 gcc 는 MY가 정의되지 않았다는 오류 메시지를 출력한다. c 소스만 놓고
볼 때 위 소스에서 대문자 "가 나올 일은 없다. 물론 우리는 위 소스의 어떤 부분이
문제가 있는지 알고 있는 상태이고, 헤더 파일로 like.h밖에 include하지 않았기 때문
에 문제를 모르더라도 단번에 찾을 수 있을 것이다. 그렇지만 이런 상황을 가정해 보자.
자신이 직접 작성하지 않은 소스를 수정해 컴파일하고자 하는데, 그 소스 파일은 여러
헤더 파일을 include 하고 있고, 또 include 한 헤더 파일 내에서 다른 헤더 파일을 더
많이 include하고 있다.
컴파일 과정에 소스에서는 분명히 사용하지 않은 심볼이 정의되지 않았다는 오류 메시
지가 출력된다. 가령 위와 같이 MY가 정의되지 않았다고 출력되는 것처럼 말이다.
어떻게 보면 정말 찾기 어려운 오류가 될 수 있다. -save-temps 옵션을 모를 경우에는
말이다.

-save-temps 옵션을 사용해 전처리 과정을 거치고 난 중간 파일을 확인해 보면 어떤
부분에서 문제가 발생했는지 단번에 알 수 있다. ［그림 4-11］ 은 Hke.c 파일의 전처리
과정 산물인 like.i 파일의 내용이다.

［그림 4-11］ like.i 파일의 내용

이런 현상은 드물지만 가끔씩 발생하는 현상으로 한 번 발생하면 문제를 찾기가 정말
힘들 수도 있다. 실제로 필자도 남이 작성한 코드를 수정하던 과정에서 이와 유사한 일
이 발생해 황당했던 적이 있다.
그러나 이제 독자들은 컴파일 과정이 어떤 절차로 진행되는지 알았고 그 부산물이 무
엇인지도 알았기 때문에 이런 문제가 발생해도 해결하는 데 어려움은 없을 거라고 본
다. Hke.s 파일은 ccl C 컴파일러로 컴파일한 결과 파일이다. 이런 like.s 어셈블리 파
일은 as 어셈블러에 의해 어셈블되면 like.s에 있는 어셈블리 명령대로 인스트럭션으로
변환되면서 like.o 바이너리가 생성된다.

170 3부_ 컴파일과링킹

===== PAGE 172 =====
Hke.s 와 같은 어셈블리 파일은 독자들이 어떤 프로그램을 작성하느냐에 따라서 매우
유용할 수 있고, 한 번도 쳐다보지 않을 수도 있다. 여러분이 애플리케이션을 제작한다
면 중간 과정에서 생성되는 어셈블리 파일은 C 소스 중간에 인라인 어셈블리를 사용
하지 않는 한 거의 볼 필요가 없을 것이다. 그러나 독자들이 운영체제나 부트로더 같이
시스템 아키텍처의 특성을 많이 타는 프로그램을 제작하고자 한다면 거의 매번 컴파일
할 때마다 어셈블리 파일을 확인해야 할 것이다.
운영체제나 부트로더의 제작에 있어 컴파일러는 더 이상 우리의 든든한 친구가 아니라
변덕쟁이 여자 친구가 되고 만다. 컴파일러가 만드는 코드에 항상 관심을 가지고 주의
를 기울여야 컴파일러가 만드는 예기치 못한 오류를 잡아낼 수 있다.
전체적으로 어떻게 컴파일 과정이 진행되는지 알아봤고, 이제는 단계별로 컴파일 과정
내에 어떤 일이 일어나는지 좀 더 자세히 알아보자.

| CC1 —B에 의한 전처리 과정

ccl -E에 의한 전처리 과정을 설명하기 전에 gcc -v -save-temps -o like like.c라는
명령을 내렸을 때 맨 처음 나오는 메시지의 의미를 알아보는 것이 좋을 것 같다.
〔예제 4-6〕 gcc -V —save-temps -o like like.c 명령 수행 시 첫 메시지

Using built-in specs.
Target: i386-redhat-linux
Configured
with:
.
.
/configure
--prefix=/usr
--mandir=/usr/
share/man
--infodir=/usr/share/info
--enable-shared
--enablethreads=posix
--enable-checking=release
--with-system-zlib
--enable-____________ cxa_atexit
--disable-libunwind-exceptions
--enablelanguages=c,
C++,
objc,
obj-c+
+
java,
fortran,
acia
--enable-javaz
awt=gtk
--disable-dssi
--enable-plugin
--with-java-home=/usr/
lib/j
vm/j
ava-1.5.0-gcj-1.5.0.0/jre
--enable-libgcj-multifile
--enable-j
ava-maintainer-mode
--with-ecj-j
ar=/usr/share/j
ava/
eclipse-ecj.jar with-cpu=generic ---------------------------------------------------------------------Thread model: posix
gcc version 4.1.2 20070502 (Red Hat 4.1.2-12)

：

:
；
；
：

:
：
；

. • • 전처리 과정 명령

여러분도 실제로 확인해 보면 ［예제 4-6］ 과 같은 메시지가 출력됨을 알 수 있을 것이다.

4장_ gcc compiler 171

===== PAGE 173 =====
Using built-in specs 부분에 대한 설명은 specs 파일을 사용한 gcc 설정에서 하기
로 한다. 다음에 오는 Target은 생성할 바이너리의 종류를 나타내는 부분이다. 그래서

i386 아키텍처의 리눅스에서 동작하는 바이너리가 생성됨을 알 수 있다.
Configured with는 gcc 를 빌드할 때 어 떤 옵션으로 빌드했는지 보여 준다. --enablelanguages 옵션 부분을 보면 지원할 언어로 c, c++, objc, obj-c++, java, fortran, ada
를 선택한 것을 확인할 수 있다. Thread model 로는 posix thread 모델을 사용함을 알
수 있고, 마지막으로 gcc 버전이 따라온다.
다음으로 ccl -E 에 의한 전처리 과정이 따라오는데, 전처리 과정은 크게 두 부분으로
나눌 수 있다. 첫 번째 과정은 헤더 파일의 삽입이고, 두 번째 과정은 매크로 치환 및 적
용이다. 헤더 파일의 삽입 설명에 앞서 먼저 C 소스 내에서 헤더 파일을 include하는
이유를 알아보자. C 소스 내에 헤더 파일을 include하는 것은 C 언어의 문법적 특성과
관련된 것으로, C 언어는 함수를 사용하기 전에 함수의 원형이 어떤지 먼저 선언을 해
야 한다는 것을 배웠을 것이다.
〔예제 4-7〕

#include <stdio.h>
void myfunc(void);
int main() {
myfunc();
return 0;
}

void myfunc(void) {
printf ("I like you!\n");

［예제 4 -刀처럼 main() 함수 내에서 myfunc() 함수를 사용하려면 myfunc() 함수 사
용 이전에 함수의 원형을 void myfunc(void)；과 같은 형식으로 선언해야 한다. 이렇게
선언한 정보는 함수가 실제로 사용될 때 컴파일러가 인자 값이나 리턴 값을 체크해 함
수가 제대로 사용되었는지 확인할 때 이용한다.
［예제 4-기에서 myfunc() 함수는 main() 함수 위에서 선언하고 사용하였기 때문에 상
관없지만 myfuncO 함수 내에서 사용된 printfO 함수는 어떨까? 함수를 사용하는 데
있어 먼저 선언해야 한다는 조항은 printfO 함수라고 예외일 수 없다. 원형을 먼저 선
언하지 않은 함수를 사용하면 컴 파일러의 종류에 따라 경고 또는 오류를 출력 한다.

172 3부_ 컴파일과링킹

===== PAGE 174 =====
그런데 printfO 함수는 그냥 사용해도 무방하다. 그 이유는 바로 include한 stdio.h 파
일에 printfO 함수의 원형이 선언되어 있기 때문이다. ［그림 4-12］ 는 /usr/include/

stdio.h 파일의 내용인데, 보는 바와 같이 printfO 함수의 원형이 선언되어 있음을 확인
할 수 있다. 헤더 파일을 C 소스 내에 include하면 전처리기가 include한 자리에 헤더
파일의 내용을 붙인다.
繼] root@os：/temp/like
This function is a possible cancelfdliuii point and therefore
not
_ marked with THROW. */

3xrern-TnF~prTntF~(72consEThaF~*^^
7* Write ——
extern int sprintF (char *_________________________ ____s,
_const char *_restrict _________________________ ...) _THROW;
"/usr/include/stdiQ.h" 854L, 28548C____________________________ 339,1

39하

[그림 4-12] /usr/include/stdio.h 파일의 내용

그럼 다시 본론으로 돌아가서 ccl -E가 수행되면 제일 먼저 입력으로 지정한 소스
파일을 읽어 들인다. 소스 파일 내에 #include〈stdio.h〉를 만나면 시스템 헤더 파일
디렉토리로

등록된

/usr/local/include,

/usr/lib/gcc-lib/i386—redhatlinux/3.2.2/

include, /usr/include 디 렉토리순으로 stdio.h 파일이 있는지 찾는다（유닉스 계열 시
스템은 /usr/include 디렉토리에 헤더 파일들이 모여 있다）.
이런 기본 탐색 include 디렉토리를 추가하기 위해 gcc 옵션으로 -［ ［ include 디렉토
리］ 형식으로 붙이면 -I 뒤에 오는 in시ude 디렉토리를 먼저 탐색하게 할 수 있다. 예
를 들면 gcc -I/root/incl니de -o like like.c를 실행하면 /root/include, /usr/local/

include,

/usr/lib/gcclib/i386—redhat—linux/3.2.2/include,

/usr/include순으로

헤더

파일을 찾는다.

stdio.h 파일은 /usr/include 디렉토리에 있기 때문에 ccl -E는 stdio.h 파일을 찾을
수 있다. 찾을 수 없다면 ccl -E는 ［그림 4-13］ 과 같은 오류 메시지를 출력할 것이다.
隊1 root@os :/temp/like2

—

[root@os like2]tt gcc -o like like.c
like.c:1:19: error: stdio.h: 그런 파일이나 디렉토리가 없음
like.c: In Function 'main':
like.c:5: warning: incompatible implicit declaration of built-ii
Function 'printf'
[root(흐os like2]tt |

킈
［그림 4너3］ stdio.h 파일을 찾지 못한 오류 메시지

stdioh 파일을 찾았다면 현재 소스 파일의 #include〈stdio.h〉라고 적힌 부분에 stdioh
파일의 내용을 읽어 붙여 넣는다.

4장_ gcc compiler

173

===== PAGE 175 =====
stdio.h 파일을 붙여 넣는 중간에 stdio.h 파일 내에 기술된 #include <features.h>
를 만나면 ccl -e 는 stdio.h 를 붙이는 것을 잠시 중단하고 다시 /usr/local/include,

/usr/lib/gcclib/i386—redhat—linux/3.2.2/incl니 de, /usr/include순으로 features.h 파
일을 찾는다.

features.h 파일 역시 /usr/include 디렉토리에 있기 때문에 ccl -E 는 features.h 파
일을 찾을 수 있다. ccl -E 는 소스에서 stdio.h 의 #include 〈 features.h 〉부분에

features.h 파일의 내용을 붙여 넣는다.
features.h 파일 내에 다시 #include 〈 test.h 〉가 있었다면 역시 stdiojh 에서 #include
〈features.h〉를 만났을 때와 마찬가지로 일단 features.h를 붙이는 것을 중단하고 test.h
를 찾아 소스에 붙인다.

test.h 를 다 붙였으면 중단되었던 feat 니 res.h 의 나머지 부분을 붙여 넣고 features.!^
다 붙였으면 마지막으로 stdio.h의 나머지 부분을 붙여 넣는다. ccl -E는 결국 이런 식
으로 소스 파일 내에 사용된 헤더 파일과 헤더 파일 내에 사용된 헤더 파일의 내용을
모두 소스 파일에 붙여 넣는다.
헤더 파일을 모두 붙였으면 이제 치환이 일어난다. #define 된 부분은 ccl -E 의 심볼
테이블에 저장되고 심볼 테이블에 들어있는 문자열과 같은 문자열을 만나면 #define된
내용으로 치환이 일어난다. 물론 이때 #ifdef와 같이 소스를 선택적으로 추가, 제거하는
매크로들도 처리된다. gcc -v -save-temps -o like like.c 명령을 내렸을 때 ccl -E
는 다음과 같은 형 태로 수행된다.
〔예제 4-8〕, 전처리기 수행 모습

— 전처리 명령

/usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl -E -quiet -v like.
c —mtune=generic -fpch-preprocess -o like.i
----- 수행 결과

ignoring nonexistent directory "/usr/lib/gcc/i386—redhat—
linux/4.1.2/../../../../i386-redhat-linux/include”
#include
search starts here:
#include <...> search starts here:
/usr/local/include
/usr/lib/gcc/i386-redhat-linux/4.1.2/include
/usr/include
End of search list.

174 3부—컴파일과링킹

===== PAGE 176 =====
gcc-4.1.x는 ccl -E에 의해 ［예제 4-8］ 과 같은 형태로 수행되지만 예전 버전 g유에서
는 cppO에 의해 전처리 과정이 수행되었다. cppO에 의해 전처리 과정이 수행될 때는
［예제 4-9］ 와 같은 형태로 처리된다. 이렇게 굳이 예전 버전 gcc의 전처리 과정을 보여
주는 것은 필자가 독자에게 알려 주고 싶은 것이 있어서다.
〔예제 4-9〕 gcc-3.2.2 버전에서의 전처리기 수행 모습

/usr/lib/gcc-lib/i386-recihat—linux/3.2.2/cppO -lang-c -v -D__
GNUC =3 -D GNUC MINOR =2 -D GNUC PATCHLEVEL =2 -D GXX ：
ABI_VERSION=102 -D_____ ELF__ -Dunix -D_______ gnu_linux______-Dlinux -D_
ELF
-D unix
-D gnu linux -D linux -D unix -D
linux -Asystem=posix ____________ ____________________ -D_____ STDC_HOSTED____ =1 ：
-Acpu=i386 -Amachine=i386 -Di386 -D______________ i386 -D______i386____ -D_____tune_ :
i386 like.c like.i

gcc-3.2.2의 전처리 과정을 보면 전처리기가 ccl -E가 아니라 cppO가 사용되는 것을
확인할 수 있다. -D 옵션은 C 소스 파일의 제일 첫 부분에 #deflne한 것과 의미가 같
다. 예를 들어 -D_ELF_와 같은 경우 각 소스 파일과 헤더 파일 내부의 제일 첫 행에

#define __ELF__한 것과 동일한 의미를 지닌다.
위와 같은 -D 옵션 인자들은 주로 운영체제별로 코드를 달리해야 될 때 이용한다. 다음
은 운영체제별로 코드를 달리 사용하는 예제 소스다.
〔예제 4-10)

운영체제별 선택 코드

#include <stdio.h>
#include <stdlib.h>
#ifdef __WINDOWS__
#include <conio.h>
#endif
int main() {
#ifdef______ linux_
system("cl은ar");
#elif __WINDOWS__
system ("cis") ;
#endif

;

return 0;
}

위에서 사용한 코드 중 #ifdef __linux__ 같은 매크로는 소스 내에 정의하지 않았더라
도 cppO가 실행될 때 -D__linux__ 같은 옵션으로 define 하기 때문에 사용 가능하다.
위 소스를 리눅스에서 컴파일하면 당연히 전처 리 과정 이 끝난 후 다음과 같이 된다.

4장_ gcc compiler 175

===== PAGE 177 =====
〔예제 4-11］ I 전처리 과정 후의 소스 코드

#include <stdio.h>
#include <stdlib.h>
int main() {
system(’’clear") ;
return 0;
}

이렇게 -D__linux__ 같이 소스싱에 define되지 않았지만 전처리기가 임의로 define
하는 것을 predefine 매크로라 한다. predefine 매크로에는 이렇게 전처리기가 임의로

define해 주는 것 외에도 ANSI 으에서 정의한__FILE______ yNE__ 등과 같이 소스 파
일 내에서 이미 정의된 매크로도 predefine 매크로에 속한다.
이런 predefine된 매크로는 주로 디버깅 출력 메시지에 사용되거나, 시스템 종류마다
혹은 컴파일러 종류마다 소스 코드를 구분해 컴파일하고자 할 때 사용된다.
예전에 cppO를 전처리기로 사용할 때까지는 이렇게 -D 옵션을 사용해 명시적으로

predefine 처리를 했었는데, ccl -E에서는 명시적으로 하지 않고 내부적으로 알아서
predefine 처리된다.
ccl -E에 의해 전처리 과정이 끝난 후의 like.i 파일 내용은 다음과 같다.

［그림 4-14］ 전처리 과정이 끝난 like.i 파일의 내용

［그림 4-14］ 에서 보면 #include〈stdio.h〉한 부분이 /usr/include/stdio.h 파일의 내용
으로 치환되어 있는 것을 확인할 수 있다.

176 3부_ 컴파일과링킹

===== PAGE 178 =====
I cc1 에 의한 어셈블리 소스 파일로 컴파일
전처리 과정이 끝났으면 이제 진짜 C 컴파일러인 CC1 이 나설 차례다. CC1 으로 컴파일
하는 과정은 다른 일반적인 컴파일러와 동일하다. ccl의 컴파일 과정은 크게 세 부분으
로 나뉠 수 있는데, 전단부 (front-end) 와 중단부 (middle-end), 후단부 (back-end) 가
바로 그것이다. 그리고 이런 컴파일 과정은 C 컴파일러인 ccl뿐만 아니라 C++ 컴파일
러인 cclplusJAVA 컴파일러인 jcl 역시 동일하다.

[그림 4-15] GCC 컴파일러(ccl, cclplus, jd 등)의 컴파일 과정

에서 하는 일은 언어 종속적인 부분을 처리하는 일이다. 전체적으로 하는 일은
소스 코드가 올바르게 작성되었는지 분석하고, 중단부에 넘겨주기 위한 GIMPI£ 트리
(소스 코드를 트리 형태로 표현한 자료 구조)를 생성하는 일이다.
트^에서 하는 일은 전단부에서 넘겨받은 GIMPLE 트리를 이용해 아키텍처 비종속
적인 최적화를 수행한 후 최종적으로 후단부에서 사'용■하는 RTL(Register Transfer

Language： 고급 언어와 어셈블리 언어의 중간 형태)을 생성하는 일이다. ccl에서 수행
하는 최적화 중 많은 최적화가 중단부에서 이뤄진다. 기억해야 될 것은 아키텍처 비종
속적인 최적화가 중단부에서 하는 중요한 일 중 하나라는 점이다.
에서는 아키텍처 비종속적인 최적화와 함께 아키텍처 종속적인 최적화가 수행
된다. 그리고 최적화가 완료되었으면 비로소 목적 코드를 생성한다. 여기서 목적 코드
는 어셈블리 코드를 의미한다. 후단부에서 수행하는 최적화의 종류도 중단부 못지않게
많다. 인스트럭션 스케줄링이나 레지스터 할당 등과 같은 일이 후단부에서 하는 중요한
일 중 하나다.

4장_ gcc compiler

177

===== PAGE 179 =====
gcc-3.x 버전까지는 cc1 의 컴파일 과정이 크게 전단부/후단부 두 개의 단계만으로 이뤄졌었다.
전단부에서 어휘/구문/의미 분석을 수행하고 바로 중간 표현인 RTKRegister Transfer Lang니age)
을 생성하면, 후단부에서 RLT로 최적화를 수행하고 목적 코드를 생성하는 구조로 되어 있었다.
이랬던 것이 gcc-4.x대로 오면서 새로운 중단부 개념이 생기고, 후단부에서 하던 아키텍처 비종속적인
최적화가 모두 중단부로 옮겨와 컴파일 단계가 전단부/중단부/후단부를 가지는 현재의 구조가 되었다.
그리고 현재 gcc는 후단부의 최적화를 중단부로 옮겨오는 중이다. 후단부가 없어지지는 않겠지만, 앞으
로 더욱 후단부의 부분이 중단부로 옮겨올 것으로 보인다.

이 런 전단부와 중단부, 후단부의 관계를 좀 더 상세히 나타내면 ［그림 4-16］ 과 같다.

［그림 4-16］ GCC 컴파일러의 컴파일 과정

그러면 각 단계에서 하는 일은 무엇인지 좀 더 자세하게 알아보자. 갈 길이 급하고 gcc
의 내부 구조보다는 단순히 사용하기만 원하는 독자가 있다면 이 단계에서 바로 “목적
코드 생성” 과정으로 건너뛰기 바란다. 지금 설명할 내용이 gCC를 이해하고 잘 사용하
는 데 있어 매우 중요하긴 하지만, 그냥 적당히 사용하는 데는 몰라도 상관없다.

178 3부_ 컴파일과링킹

===== PAGE 180 =====
지금부터 설명할 내용은 어쩌면 여러분의 머리를 혼란스럽게 할 수 있다. 단순히 gcc 를 사용
하고자 하는 독자라면 제발 부탁이니 지금 설명할 과정을 건너뛰고 “목적 코드 생성” 과정으로
넘어가길 바란다.
지금부터 설명할 내용을 알아‘ 두면 앞으로 독자에게 두고두고 도움이 될 수 있다. 프로그래밍
을 그냥 잘하는 것이 아니라 매우 잘하려면 반드시 컴파일러와 프로세서 아키 텍처는 매우 깊
게 이해해야 된다.
때문에 필자는 혼신의 힘을 다해 되도록 이해하기 쉽게 어려운 부분을 다 빼고 꼭 필요한 것만
설명하였다. 하지만 컴파일러 자체가 크게 어렵지는 않지만 처음 시작할 때는 많은 배경 지식
을 요구하므로 아무것도 모르는 상태에서 접근하는 것은 쉽지 않다.
필자가 확실하게 전달하고자 하는 것은 전체 컴파일 과정의 이해인데, 자칫 다음에 설명할 내
용을 준비가 안 된 사람이 본다면 숲을 보지 못하고 나무만 보는 상황이 될 수가 있다. 그러니
정말 꼭 보고 싶은 독자가 아니라면 일단 넘어가고 나중에 보고 싶을 때 보기 바란다.
그리고 컴파일러 이론은 매우 방대하고 알아야 될 개념도 많기 때문에 이 책에서 설명하는 데
한계가 있다. 필자는 이 책에서 독자가 컴파일러를 전체적으로 이해하는 데 꼭 필요한 것들만
설명하겠다. 문제는 이렇게 꼭 필요한 것조차도 준비가 안 된 사람에게는 어려울 수가 있으므
로 주의를 준 것이다.
더 많이 알고 싶고, 더 잘하고 싶은 독자가 있다면 개인적으로 컴파일러 책을 읽어 볼 것을
권한다.

O CC1 전단부에서 하는 일
CC1 의 전단부（ front-end） 에서 하는 일은 C 소스 코드를 입력받아 소스 코드의 문법
상, 의미상의 오류를 파악하고, 최종적으로 트리 형태의 중간 표현（ IR： Intermediate

Representation） 인 GIMPLE 트리를 생성하는 일이다. 중간 표현（ GIMPLE 트리）에 대
해서는 바로 다음에 설명한다.

Front-end
（어휘/구문/의미 분석）

중간 표현

（ GIMPLE
트리）

［그림 4-17］ CC1 전단부 처리 과정

CC1 을 포함한 대부분의 컴파일러가 전단부에서 하는 일은 ［그림 4-18］ 과 같이 어휘
분석, 구문 분석, 의미 분석, 중간 표현 생성이라는 4단계로 크게 나눠진다.

4장_ gcc compiler

179

===== PAGE 181 =====
그리고 각 단계에서 하는 일은 다음과 같다.
► 어휘 분석
어휘 분석에서 하는 일은 c 소스 코드를 의미가 있는 가장 최소 단위로 나누는 일이다.
이런 일을 수행하는 것을 어휘 분석기라 부르고 다른 말로 스캐너라고도 한다. 전처리
된 like.i 소스 코드는 스캐너에 의해 읽혀지면서 소스 코드를 문법적으로 의미 있는 가
장 최소 단위로 나눈다. 이런 문법적으로 의미 있는 가장 최소 단위의 문자열을 토큰이
라 부르고, 그 종류와 예는 [표 4-1] 과 같다.
[표 4-1] 토큰 종류

종류

예

지정어

if, while, for, do, switch, case 등

연산기호

, *./,%,＜〉, = 등

구분자

(, [.： 등

명칭

main, printf, var 등

상수

1203,120.3, “I like you!\n” 둥

어휘 분석 단계에서 likej는 위와 같은 토큰으로 나눠지고, 나눠진 토큰을 하나씩 다음
단계인 구문 분석을 담당하는 파서에 넘긴다.
► 구문분석
구문 분석에서 하는 일은 프로그램의 문법상 오류를 찾아내는 일이다. 그래서 like.c 파
일에 문법적인 오류가 있었다면 이 단계에서 걸러진다. 이런 구문 분석을 수행하는 것
을 구문 분석기라 부르고, 다른 말로 파서(parser)라 부른다.

180 3부_ 컴파일과링킹

===== PAGE 182 =====
스캐너에게서 토큰을 넘겨받은 파서는 파스 트리를 만들면서 문법적 오류가 있는지 체
크한다. 그래서 사소한 문법적 오류들, 예를 들면 세미콜론을 빼먹었다거나 괄호 닫
기를 안 한 것 같은 문법적 오류들은 모두 이 단계에서 걸러진다.

［그림 4-19］ 파스 트리 예

［그림 4-19］ 는 독자의 이해를 돕기 위해 “(5 * X) + 3”이라는 소스 코드가 있을 때 생성
되는 파스 트리의 모양이 어떤지 그림으로 보여준 것이다.
입력 받은 소스상에 문법적 오류가 없었다면 소스 파일 전체 내용을 표현하는 파스 트
리가 정상적으로 만들어진다. 하지만 문법적 오류가 있다면 파스 트리가 정상적으로
만들어지지 않는다. 파스 트리가 정상적으로 만들어지는지 만들어지지 않는지 여부는

C 언어 문법에 의해 결정된다. 이렇게 C 언어 문법에 맞게 정상적으로 파스 트리가 만
들어지는지 여부에 따라 문법적 오류를 체크하는 것이다.

like.c 파일에 문법적 오류가 있었다면 이 단계에서 오류를 출력할 것이다.
► 의미 분석
의미 분석 단계에서는 문법상 오류는 없지만 의미상 오류가 있는 것을 체크한다. 예를
들면 선언되지 않은 변수를 사용했다거나, 함수를 사용하는 데 있어 인자 개수나 인자
형 이 불일치 했다거나, 그리고 변수 사용에 있어 자료형 이 불일치한 것 등이 의미 분석
단계에서 체크하는 것들이다. 이때는 ［그림 4-18］ 에서 보이는 어휘 분석과 구문 분석
단계에서 구축된 심볼 테이블을 이용해 이런 일들을 수행한다.

4장_ gcc compiler 181

===== PAGE 183 =====
이상의 단계를 거치면 C 소스 파일 내에서 잘못 사용된 문법이나 오타, 잘못 사용된 함
수, 정의되지 않은 변수의 사용 같은 오류들이 모두 걸러진다. 그리고 이렇게 소스상의
오류를 찾아내는 일이 CC1 전단부에서 하는 매우 중요한 일 중 하나다. CC1 전단부에서
하는 두 번째 중요한 일은 C 소스 코드를 ccl 내부에서 사용하는 중간 표현 코드로 변
경하는 일이다.
► 중간 표현 생성
거의 모든 컴파일러는 언어 종속적인 부분과 기계 종속적인 부분을 분리해 컴파일러를
모듈화하고 최적화를 쉽게 하기 위해 중간 표현을 사용한다. CC1 은 내부적으로 두 가지
종류의 중간 표현을 사용하는데, 하나는 중단부에서 사용하는 GIMPLE 트리 이고, 다른
하나는 후단부에서 人卜용'흐｝느추 RTL(Register Transfer Language)이다.

GIMPLE 트리는 언어 독립적인 특성을 제공하기 위해 사용하는 트리 형태의 중간 표현
이고, RTL은 기계 독립적인 특성을 제공하기 위해 사용하는 거의 어셈블리 수준의 중
간 표현이다.

GIMPLE 트리는 여러 프로그래밍 언어 소스를 공통된 언어 표현으로 바꾼 후 소스 코
드를 트리 형태로 표현한 것으로, GIMPLE 트리가 생성되는 과정은 다음과 같다.

［그림 4-20］ 중간 표현 생성 과정

의미 분석 단계까지 거쳤다면 likej 소스 파일은 문법적, 의미적으로 오류가 없다고
볼 수 있다. 이런 like.i 소스 파일의 구문 분석에서 만들어진 파스 트리를 각 언어의

AST (Abstract Syntax Tree) 로 변경한다. 그리고 AST(Abstract Syntax Tree) 를 다시
언어 종속적이지 않은 GENERIC 트리로 바꾸고, 마지막으로 GENERIC 트리를 좀 더
간소화시켜 GIMPLE 트리를 생성한다. AST는 바로 다음에 설명한다.
［그림 4-20］ 에서 보면 각 언어의 AST(Abstract Syntax Tree)는 각 언어의 genericize
에 의해 GENERIC 트리로 바뀌고, GENERIC 트리는 다시 GIMPLE 트리로 바뀌는

182 3부- 컴파일과링킹

===== PAGE 184 =====
것을 볼 수 있다. 그리고 이렇게 GENERIC 트리를 GIMPLE 트리로 바꾸는 과정을

Gimplify라 부른다.
여기서 AST란 토큰만으로 이뤄진 트리를 말한다.

(5*X + 3)

파스 트리는 구문 분석을 위해 실제 코드에는 없는 넌터미널(non-terminal)(예: ［그림

4-21］ 에서 number, part, expression과 같은 것들)들이 들어있는데, 이는 구문 분석에
서만 필요하고 이후 과정에서는 필요하지 않다. 때문에 불필요한 정보를 제거해 앞으로
과정을 단순화시키기 위해 파스 트리를 더 간단한 형태인 AST로 변경하는 것이다.
［그림 4-21］ 에서는 간단한 AST (Abstract Syntax Tree) 의 예를 보여준다. 확인해 보면
소스에서 사용된 토큰만으로 이뤄진 것을 볼 수 있을 것이다. AST는 파스 트리에서 좀
더 추상화했다고 해서 Abstract Syntax Tree라 부른다. 결국 파스 트리를 간소화시킨
것이 AST라고 보면 된다.
넌터미널(non-terminal)이란?
컴파일러 용어 중 하나로서 ［그림 4-20］의 파스 트리에서 number, name, part, expression 등과 같
이 토큰에 해당되지 않는 것들을 의미한다. 컴파일러를 배울 때는 중요하지만 이 책에서는 몰라도 상관
없다.
— 당부 사항

그

으

우

AST, GENERIC 트리, GIMPLE 트리, 넌터미널(non-terminal) 등 생소한 단어가 나왔다. 이런 것들
을 반드시 이해할 필요는 없다. 컴파일 과정의 전체적인 흐름만 알면 된다. 그렇기 때문에 이해가 안 되
는 부분이 있더라도 전혀 부담갖지 말고 가볍게 신나게 무소뿔처럼 거침없이 읽어나가기 바란다.
4장_ gcc compiler 183

===== PAGE 185 =====
GIMPLE 트리 이 전에 있는 GENERIC 트리는 소스를 트리 구조로 표현하는 데 있어 언
어 독립적인 특징을 제공하기 위해 만들어졌다. 그래서 GCC에서 지원하는 많은 언어
의 소스 코드는 GENERIC 트리로 표현 가능하다. GENERIC 트리와 같은 공통된 표현
으로 소스 코드의 AST를 바꾸지 않고, 각 언어의 AST를 가지고 컴파일 과정을 진행하
는 컴파일러를 구현하면 문제가 있을 수 있다.
예를 들면 GENERIC 트리로 변경하지 않고 각 언어의 AST를 가지고 최적화하는 부분
을 컴파일러에 구현할 수도 있다. 그렇지만 이렇게 하면 최적화 코드는 모든 언어에서
필요로 한다고 할지라도 해당 언어만을 최적화할 수 있는 코드로 한정되어 버린다. 또
한 새로운 언어를 추가하는 데 있어서도 매번 해당 언어의 최적화 코드를 새로 작성해
야한다.
이렇게 컴파일러가 언어 종속적이게 되는 문제를 해결하기 위해 (오으에서는 각 언어

(C, C++, JAVA, ADA, Objective-C, Fortran 등)의 AST를 GENERIC 트리 같은 공통
된 중간 표현으로 바꾼다. 이후 GENERIC 트리를 시작으로 하는 최적화 코드를 컴파일
러에 작성한다면 동일한 최적화 코드를 여러 언어에 공통적으로 사용할 수 있게 된다.

GENERIC 트리는 모든 언어의 AST에서 제공하는 표현을 지원할 수 있어야 하기 때문
에 GCC가 지 원하는 언어 의 AST 표현들의 슈퍼 셋으로 구성된다. 쉽 게 말하면 GCC가
지원하는 모든 언어의 소스 코드를 표현할 수도 있는 언어라는 의미다.

GCC가 여러 언어를 지원할 수 있는 것은 다 이런 GENERIC 트리 같은 중간 표현이 있
었기 때문이다. 다음은 전단부에서 생성하는 like.i의 GENERIC 트리 표현을 예로 든
것이다.
〔예제 4-12)

like.i의 GENERIC 트리

main ()

;

{

|
int D.1620;
printf
D.1620
return

}

(&"Ilike you!\n"[0]);
= 0;
D.1620;

:
;
；

!

[예제 4-12]는 그다지 트리 구조처럼 보이지 않을 것이다. 그렇지만 사실 [예제 4-12]
코드는 전단부에서 트리 자료 구조로 표현된 것이 맞다. 컴파일러 내부에서 트리 자료
구조로 표현된 like.i< 텍스트 형식으로 표현하면 이렇게 소스 코드처럼 보이게 되는

184 3부—컴파일과링킹

===== PAGE 186 =====
것이다. 소스 코드에서 만들어진 자료 구조라서 이를 텍스트로 표현하면 소스처 럼 보이
는 것은 어쩌면 당연한 것이다.

GENERIC 트리는 GCC에서 언어 독립적인 측면을 제공하기 위해 만들어진 중간 표현
이라고 했었다. 이런 중간 표현들은 언어 독립적인 측면 외에도 아키텍처 독립적인 측
면을 제공하기도 하는데, 이에 대해서는 후단부에서 RTL 중간 표현을 이야기할 때 설
명하겠다.
이렇게 생성된 like.i의 GENERIC 트리는 Gimplify 과정을 거치면서 GIMPLE 트리로
변경된다. GIMPLE 트리는 GENERIC 트리와 유사한데, GENERIC 트리의 서브셋으로
서 좀 더 최적화하기 수월한 형태로 GENERIC 트리를 변경한 것이다. GIMPLE 트리에
는 GENERIC 트리와는 다르게 몇 가지 제약이 존재하는데, 대략 다음과 같다.
• 한 명령은 3개 이상의 오퍼 랜드를 가질 수 없다.

• if문에서는 하나의 비교문만 와야 한다.
• 함수를 호출할 때 함수의 인자는 변수만 허용한다.
이런 제약들로 인해 표현의 복잡도가 줄어들어 최적화하기 수월한 형태가 된다. 다음은

hke.i의 GIMPLE 트리 표현을 보여준다.
〔예제 4너3〕 like.i의 GIMPLE 트리

main ()
{
int D.1620;
printf (&"I like you!\n"[0]);
D.1620 = 0;
return D.1620;

like.i의 GENERIC 트리와 GIMPLE 트리를 비교해 보면 like.i 소스가 너무 단순해서 그
다지 다른 점을 확인하기 힘들 것이다. ［표 4-2］ 를 보면 GENERIC 트리와 GIMPLE 트
리가 어떻게 다른지 확인할 수 있을 것이다.

4장_ gcc compiler 185

===== PAGE 187 =====
[표 4-2] GENERIC 트리와 GIMPLE 트리 비교

C 소스

GENERIC 트리

if (add(a - 3, 4)) {

if (add (a — 3, 4) != 0)

b = a++ % 2；

D.1142 = a-3；
D.1143 = add (D.1142, 4)；

{
b = a++ % 2；

}

GIMPLE 트리

if (D.1143 != 0)

}

{

이%

b = a % 2；

{

a = a +1；

}

}
이 se
{
}

위 표에서 보면 소스의 길이는 GIMPLE 트리가 가장 길지만, if문에서의 복잡한 표현들
이 잘게 쪼개져 GENERIC 트리보다 훨씬 간결하게 표현된 것을 확인할 수 있다.
이런 GIMPLE 트리는 전단부에서 최종적으로 생성하는 중간 표현이고, 이후 중단부에
입력으로 들어가 최적화 과정을 거친다.
전단부에서 GIMPLE 트리와 같이 소스와 유사한 트리 형태의 중간 표현을 생성하는 데
는 언어 독립적인 측면을 제공하는 것 외에도 한 가지 이유가 더 있다. gcc-3.x 버전까
지만 해도 gcc는 전단부에서 AST로 함수 인라인만 수행하고 AST를 바로 RTL로 변환
하였다. 이후 이런 RTL은 후단부에서 모든 최적화 과정에 사용되었다.
나중에 보겠지만 RTL은 거의 어셈블리 수준의 중간 표현이라서 구조체라든지, 배열 등
과 같은 구조를 이해할 수 없어 상위 레벨 최적화에 적합하지 않다. GIMPLE 트리는 이
런 상위 레벨 최적화 문제도 해결하기 위해 만들어졌다.
자, 지금까지 gcc의 전단부에 대해 알아보았다. “하하하. 사실 지금까지 필자가 한 말은
모두 거짓말이다.”라고 말하면 어떨까? 지금까지 배운 내용의 신뢰가 와르르 무너지지
않는가? 좀 더 확실히 마음에 와 닿게 하기 위해 사실인지 아닌지 직접 눈으로 확인해
보자. gcc의 좋은 점은 지금까지 설명한 GIMPLE 트리를 직접 눈으로 확인할 수 있다
는 것이다. 그리고 시간이 많고 하드한 일을 원하는 하드코어적 성향의 훌륭한 독자라
면 직접 공개된 gcc 소스 코드를 분석해 확인할 수도 있다.

186

3부_ 컴파일과 링킹

===== PAGE 188 =====
► GIMPLE 트리 확인
지금까지 컴파일 과정에서 사용한 like.c 파일은 너무도 간단해 like.c 파일의 GIMPLE
트리를 살펴봤자 그다지 마음에 와 닿는 것이 없을 것이다. 사실은 필자가 독자에게
뭔가를 알려주고 싶은 것이 있는데, 이전에 사용한 like.c 소스로는 확인이 불가능하다.
그러므로 아래와 같은 CTest.c 소스 파일을 작성하고 테스트해 보자.
〔예제 4너4〕 CTest.c 파일 내용

#include <stdio.h>
int main()
{
int i, j, k;
j = 0;
k = 0;
for (i=0; i < 10; i++) {
if ((i % 2) != 0) {
j += 1；
} else {
k += 1;
}
printf (’’j = %d, k = %d\n", j, k) ;
}
return 0;

[예제 4-14] 소스를 보면 알겠지만 하는 일은 간단하다. 루프를 10번 돌면서 홀수이면

j에 1을 더하고, 짝수이면 k에 1을 더한다. 위 소스 코드를 다음 명령으로 컴파일해 보
면 CTest.c의 GIMPLE 트리를 확인할 수 있다.
$ gcc -o CTest CTest.c -fdump-tr은은一all

-fdump-tree-all 옵션은 ccl 컴파일러 자체를 디버깅할 때 사용하는 옵션 중 하나로,
ccl이 소스 파일의 컴파일 과정을 진행하면서 모든 과정에서 중간에 생성되는 트리들
을 덤프하는 옵션이다. 그래서 -fdump-tree-all 옵션을 사용하면 전단부에서 생성하
는 GIMPLE 트리를 눈으로 직 접 확인할 수 있다.
하지만 아쉽게도 GENERIC 트리는 확인할 수 없다. gcc-4.0.x 버전에서 -fdump-

tree-generic라는 옵션이 잠시 추가되어 GENERIC 트리의 덤프가 가능했지만, 이후

4장_ gcc compiler

187

===== PAGE 189 =====
버전에서 해당 옵션이 빠져버렸다. 안타깝지만 GIMPLE 트리를 확인하는 것만으로 만
족하자. 다음은 -fd니mp-tree-all 옵션을 주고 CTest.c 파일을 컴파일한 결과다.
싀믜싀

<"woos@os： ~/gcc
woos@os:~/gcc$ is
CTest.c
woos@os:~/gcc$
woos@os:~/gcc$ |gcc -0 CTest CTest.c —Fdunp-tree—all|
wooseos:~/gcc$
woos@os:~/gcc$ is
CTest
CTest.c.t06.ucg
CTest.c
CTest .c.t16.useless
CTest.c.toe.tu
CTest.c.t18.lower
CTest.c.tIQ.eh
CTest.c.t82.original
CTest.c.t03.gimmie |
CTest.c.t20.cFg
woos@os:~/gcc$ 1

CTest.c.t21.cplxlowerO
CTest.c.t22.ueclower
CTest.c.t24.fixupcfg

［그림 4-22］ 실제 컴파일 결과

gcc-4.x대 버전 이하의 gcc를 사용하는 독자는 -fdump-tree-all 옵션이 지원되지 않을 것이다. gcc는
3.x대 버전에서 4.x대 버전으로 변경되면서 많은 부분이 바뀌었다. 자신이 사용하는 gcc 버전이 낮아
-fdump-tree-all 옵션이 지원되지 않는다면 개념적으로만 이해하고 넘어가자. 여기서는 굳이 GIMPLE
트리를 확인하는 것이 중요한 게 아니라 컴파일 과정이 어떤지 아는 것이 더 중요하기 때문이다.

［그림 4-22］ 는 실제 컴파일한 결과 화면이다. 파일명이 ［소스 파일명］.［컴파일 과정
번히.［컴파일 과정명］으로 하는 파일들이 여럿 생긴 것을 확인할 수 있을 것이다. 중
간에 t［숫자］ 형식으로 표현된 부분은 컴파일 과정 번호를 의미하고, 맨 마지막에 오는

tu, gimple, veg 등과 같은 것들은 컴파일 과정명을 의미한다.
우리는 컴파일 명령 시 최적화를 전혀 하지 않았기 때문에 최적화 과정을 건너뛰어 과
정 번호가 순차적이지 못하고 드문드문 빠져 있는 것을 확인할 수 있다. 다음과 같이

-O［최적화 레벨］ 옵션을 주면 최적화 과정을 수행하기 때문에 훨씬 많은 트리 덤프 파
일이 생성됨을 확인할 수 있을 것이다.
$
gcc
-o
CTest
CTest.c
-fdump-tree-all
$
gcc
-o
CTest
CTest.c
-fdump-tree-all
$ gcc -o CTest CTest.c -fdump-tree-all -03

-01
-02

# 최적화 레벨 1
# 최적화 레벨 2
# 최적화 레벨 3

이렇게 생성되는 파일들은 전단부와 중단부에서 생성하는 트리들을 덤프한 파일로서
중간 표현 변환 단계, 최적화를 위한 분석 단계, 그리고 각각의 최적화 단계에서 과정
번호순으로 트리들을 덤프해 보여주는 것이다. 각 덤프 파일의 의미를 제대로 이해하
려면 컴파일러 지식이 필요하기 때문에 따로 설명하지 않는다. 굳이 알고 싶은 독자는

man gcc 명 령으로 확인해 보기 바란다.

188 3부_ 컴파일과링킹

===== PAGE 190 =====
이렇게 생성되는 파일 중에서 CTest.c.tO3.gimple 파일이 CTest.c의 GIMPLE 트리를
담고 있는 파일이다. tO3 번호는 컴파일 과정 번호라서 gcc 버전에 따라 컴파일 과정이
다를 수 있다. 때문에 마지막에 있는 컴파일 과정명인 gimple로 해당 파일을 확인하면
된다. CTest.c.tO3.gimple 파일을 열어보면 다음과 같은 내용을 볼 수 있을 것이다.
〔예제 4-15〕 CTest.c.tO3.gimple 파일 내용

main ()
{
int D.1782;
_Bool D.1783;
int D.1784;
int i;
int j;
int k;
j = 0;
k = 0;
i = 0;
goto <D1780>;
<D1779>:;
D.1782 = i & 1;
D.1783 = (_Bool) D.1782;
if (D.1783)
{

-j = j + 1；

}
else
{
k = k + 1;
}
printf (&’’j = 응d, k = %d\n" [0] , j, k) ;
i = i + 1;
<D1780>:;
if (i <= 9)
{
goto <D1779>;
}
else
{
goto <D1781>;
)
<D1781>:;
D.1784 = 0;
return D.1784;

4장_ gcc compiler 189

===== PAGE 191 =====
GIMPLE 트리 코드를 보면 이전에 설명한 GIMPLE 트리의 제약 조건이 적용된 것이
보이고, 모든 코드가 좀 더 복잡도가 낮은 형태로 변경된 것이 보일 것이다. 그리고 한
번 자세히 보면 재미있는 결과를 확인할 수 있을 것이다. for문이 풀어지면서 if { goto

<D1779>； } else { goto <D1781>； }문으로 변경된 것을 확인할 수 있다. 이렇게 for문
같은 것은 좀 더 하위 수준의 중간 표현인 RTL로 변경하기 위해, 그리고 여러 언어를
지원하기 위해 if { goto <D1779>； } else { goto <D1781>； 문과 같은 단순한 형태로

ccl 내부에서 변경된다. 이렇게 while, for, switch 등과 같은 문들이 모두 goto로 바
뀐 GIMPLE 트리를 저수준 GIMPLE 트리라 하고, 아직 바뀌지 않은 GIMPLE 트리를 고
수준 GIMPLE 트리라 한다. 고수준 GIMPLE 트리는 이렇게 모두 저수준 GIMPLE 트리
로 변경된다.
시간이 충분한 독자라면 while문과 do while문, switch문이 GIMPLE 트리싱에서 어떻
게 변경되는지 확인해 보기 바란다. 재미있는 결과들을 확인할 수 있을 것이다.
Tip 에
간혹 개발자 사이트에서 GOTO문의 사용에 대해 논쟁이 오갈 때가 있다. GOTO문 자체를 극도로 혐
오해서 사용하면 안 된다는 사람과, 적당히 사용하면 아무 문제없다는 사람들로 나눠져서 논쟁이 격해
질 때가 있다.
물론 필자는 한 페이지를 넘어가지 않는 범위에서 딱 필요한 시점에 알맞게 적당히 사용한 GOTO문은
나쁘지 않다는 주의다. 어차피 컴파일러 내부에서는 for, while, switch문 모두 GOTO로 변경된다.
컴파일러 내부에서 어차피 GOTO문이 사용되니 그렇다고 GOTO문을 자주 사용하자는 것도 아니다.
GOTO문은 코드의 블록(Basic Block)을 나눠버리므로 최적화에 좋지 않은 영향을 미칠 수 있다. 가독
성, 최적화 모두를 고려해도 GOTO가 옳다면 사용하지 않는 것이 조금은 우습다고 본다.

GOTO문을 반대하는 사람 중에는 자신의 프로그래밍 철학과 자신의 기준에 의해 반대하는 사람들이
있다. 그런 사람들은 충분히 납득 가능하고 합리적인 이유들을 이야기한다.
문제는 자신의 이야기를 하지 않고 대학교 수업 시간에 교수님께 들은 이야기나 덱스트라 같은 유명인
의 이야기를 아무 생각 없이 앵무새처럼 따라 하는 사람들이 있다. 그런 사람들을 보면 마치 카세트테이
프 같다는 느낌이 든다. 독자가 GOTO를 사용하던 사용하지 않던 관계 없다. 단지 자신의 생각과 철학
으로 사용 여부를 결정하기 바란다.

자바 소스의 GIMPLE 트리를 확인해 보고 싶은 독자도 있을 것이다. 지면 관계상 결과
는 생략하고 어떻게 확인하는지 과정만 알아보자. 먼저 다음과 같은 자바 예제 코드를
생성한다.

190 3부_ 컴파일과링킹

===== PAGE 192 =====
〔예제 4너 6]

JavaTest.java 파일 내용

public class JavaTest {
public static
int i, j.

void main(String args[]) {
k;

j = 0;
k = 0;
for (i=0; i < 10; i++) {
if ((i % 2) != 0) {
j += 1；
} else {
k += 1;
}
System, out .print 丄n ("j = " + j + ”, k = ’’ + k) ;
}

그리고 다음 명령으로 컴파일한다.
$ gcj -o JavaTest JavaTest.java --main=JavaTest -fdump-tree-all

gcj 명령은 GCC의 자바 컴파일러 드라이버다. gcj는 GCC 빌드 시 지원 언어 중에 자
바를 포함시켰을 때 생성된다. 그렇지만 어찌된 영문인지 페도라 7 배포판이나 우분투

7.04 배포판에서 GCC는 자바를 지원하게 빌드되었지만 gcj는 포함하고 있지 않다. 때
문에 gcj 명 령을 사용하려면 다음 명 령을 사용해 먼저 gcj를 설치한 후 자바 소스를 컴
파일할 수 있을 것이다.
- 페도라 7 배포판의 경우
# yum install java-1.5.0-gcj*
- 우분투 7.04 배포판의 경우

$ sudo apt-get install gcj

gcj는 SUN 자바 컴파일러인 javac와는 다르게 바이트 코드를 생성하지 않고 네이티브(native) 바이너
리를 생성하는 GNU의 자바 컴파일러다.

4장_ gcc compiler 191

===== PAGE 193 =====
지금까지 gcc 컴파일러의 전단부에 대해 알아보았고, 최종적으로 생성되는 GIMPLE
트리도 직접 눈으로 확인해 보았다. 그러면 잠시 쉬어 가자. 느긋하게 기지개도 한번 켜
고, 주방으로 가서 맛있는 커피도 한잔 타오기 바란다. 여기 맛있는 커피를 타는 비법을
공개한다.
커피의 황금 비율
커피에도 황금 비율이 있다. 커피의 황금 비율은 커피:프림:설탕의 비율을 각각 1：2：3으로 하는 것이
다. 그러면 아주 맛있는 커피를 먹을 수 있다.

좋류벽항금비을및게법丁

三 三 _—

—으

三3

1. 다방커피 0.8 ： 1 ： 1 (비법 : 커피 잔을 뜨겁게 한 후 탄다.)
2. 자판기 1 ： 2.8 ： 2.7 (초정밀 비율 = 15 ： 44 ： 41)
3. 인스턴트 1.5 ： 2 ： 2 (비법: 물 85ml 용량에 온도를 85~90幻로 데운다.)
4. 프리마 표지에 써있는 비율 1 ： 2 ： 1.4

이렇게 생성된 GIMPLE 트리는 컴파일러 중단부에서 읽혀져 아키텍처 비종속적인 최
적화 과정을 진행하게 된다. 그럼 중단부에서는 어떤 일이 일어나는지 알아보자.

@ CC1 중단부에서 하는 일
CC1 중단부(middle-end)에서 하는 일은 GIMPLE 트리를 입력으로 받아 SSA(Static
Single Assignment) 형태로 변환한 후 SSA에 기초한 아키텍처 비종속적인 최적화를
수행하고, 최종적으로 ccl 후단부(back-end)에서 사용할 RTL을 생성하는 일이다. 여
기서 아키텍처 비종속적이라는 말의 의미는 아키텍처에 구애받지 않고 할 수 있는 최
적화를 말한다.

192 3부_ 컴파일과링킹

===== PAGE 194 =====
► SSA 변환
SSA(Static Single Assignment)는 중간 표현의 한 가지 형 태로서 변수에 값을 한 번만
할당하는 표현 형태를 의미한다. 예를 들어 다음과 같은 표현이 있다고 가정하자.
i = 10
j = i + 10
k = j + 20
j=i+k
m=j+5

이를 SSA로 변경하면 다음과 같이 된다.
i_l
10
j_2 = i_l + 10
k 3 = :i_2 + 20
+ k_3
j：4 = i 1
m_5 = :i_4
+5

보면 알겠지만 각각의 변수에는 단 한 번만 값이 할당된다는 것을 확인할 수 있다. 이
렇게 중간 표현을 SSA 형태로 변경하는 이유는 SSA 형태의 중간 표현이 사이드 이펙
트(side effect)가 없고, 데이터 흐름을 명시적으로 분명하게 표혀할 수 있어 최적화를
구현하는 데 용이하기 때문이다. 특히 몇몇 최적화는 반드시 SSA상에서 구현해야 하는
것도 있다.
때문에 gcc는 중단부 시작 부분에서 GIMPLE 트리를 SSA로 변경하고 이후 SSA 기반
최적화를 수행한다.
이전에 CTest.c 파일을 -fdump-tree-all -03 옵션을 지정하고 컴파일하면 CTest.

c.t28.ssa라는 파일이 생성되었는데, 이것이 GIMPLE 트리가 SSA 형식으로 변경된 파
일이다. SSA 표현을 보고 싶다면 해당 파일을 열어 확인해 보기 바란다(t28은 컴파일
과정 번호라서 gcc 버전에 따라 다를 수 있다).

-03 옵션으로 컴파일하면 거의 모든 컴파일 과정을 거치는데, 무려 100단계나 된다.
다음은 -03 -fdump-tree-all 옵션을 사용해 CTest.c 파일을 컴파일했을 때 생성되는
덤프 파일들이다.

4장_ gcc compiler

193

===== PAGE 195 =====
〔예제 4너7〕 -fdump-tree-all -03 옵션으로 컴파일 시 생성되는 파일 리스트

CTest.c.tOO.tu
CTest.c.t02.original
CTest.c.t03.gimple
CTest.c.t06.veg
CTest.c.tlO.cleanup_cfg
CTest.c.tl6.useless
CTest.c.tl9.lower
CTest.c.t20.eh
CTest.c.t21.cfg
CTest.c.t22.cplxlowerO
CTest.c.t23.veclower
CTest. c. t25 .fixupefg
CTest.c.t27.salias
CTest.c.t28.ssa
CTest.c.t2 9.aliasl
CTest.c.t30.retslot
CTest.c.t31.copyrenamel
CTest.c.t32.eustores
CTest.c.t33.ccp
CTest.c•t34.fre
CTest.c.t35.deel
CTest.c.t36.forwpropl
CTest•c.t37.copypropl
CTest.c.t38.vrp
CTest.c.t39.dce2
CTest.c.t40.mergephi
CTest.c.t41.doml
CTest.c.t42.phionlycopypropl
CTest.c.t43.phioptl
CTest.c.t44.alias2
CTest.c.t45.tailr
CTest. c. t4 6 .profile
CTest.c.t47.ch
CTest.c.t49.cplxlower
CTest.c.t50.sra
CTest.c.t51.alias3
CTest.c.t52.copyrename2
CTest.c.t53.dom2
CTest.c.t54.phionlycopyprop2

CTest.c.t55.reassocl
CTest.c.t56.dce3
CTest.c.t57.dsel
CTest.c.t58.alias4
CTest.c.t59.forwprop2
CTest.c.t60.phiopt2
CTest.c.t61.objsz
CTest.c.t62.store_ccp
CTest.c.t63.store_copyprop
CTest.c•t64.fab
CTest.c.t65.alias5
CTest.c.t66.crited
CTest.c.t67.pre
CTest.c.t68.sink
CTest.c.t69.loop
CTest.c.t70.loopinit
CTest.c.t71.copyprop2
CTest.c.t72.lim
CTest.c.t73.unswitch
CTest.c.t74.seep
CTest.c.t75.empty
CTest.c.t77.iveanon
CTest.c.t82.cunroll
CTest.c.t83.ivopts
CTest.c.t84.loopdone
CTest.c.t86.reassoc2
CTest.c.t87.dom3
CTest.c.t88.phionlycopyprop3
CTest.c•t8 9.eddee
CTest.c.t90.dse2
CTest.c.t91.forwprop3
CTest.c.t92.phiopt3
CTest.c.t93.tai1c
CTest.c.t94.copyrename3
CTest•c.t95.uneprop
CTest.c.t96.optimized
CTest.c.t97.nrv
CTest.c.t98.vars
CTest.c.t99.blocks
CTest. c. tlOO .final_cleanup

이 중에서 CTest.c.t28.ssa 이후부터가 gcc 중단부에서 SSA 기반 최적화를 수행하면서 생
성한 파일들이다. SSA를 만들었다면 이제 아키텍처 비종속적인 최적화를 수행할 차례다.

194

컴파일과링킹

===== PAGE 196 =====
► SSA 기반 아키텍처 비종속적인 최적화
최적화는 프로그램의 기능은 같지만 크기가 작고, 빠르며, 메모리를 작게 사용하도록
코드를 변경하는 것을 말한다. cel은 컴파일 시간의 대부분을 최적화 과정에 사용한다.
또한 ccl 소스의 대부분은 최적화를 위한 코드다.
최적화가 중요한 이유는 프로그램이 한 번 컴파일되면 변경이 불가능하고, 그 프로그램
이 언제까지고 계속 사용될 수 있기 때문이다. 그래서 최적화를 수행함으로써 컴파일
시간이 오래 걸릴지라도 프로그램 수행 속도가 증가해 전체 시스템 성능에 지속적으
로 좋은 영향을 미칠 수 있기 때문이다. 세상의 모든 PC가 1Mbyte 작아지고 1초만 빨
라졌을 때 하드디스크와 메모리가 얼마나 절약되고, 전력이 얼마나 절약될지 생각해 보
자. 그래서 최적화는 크게 보면 인류 평화에 이바지하는 일이다. ccl의 최적화 과정은
크게 2단계로 나눠지는데, 중단부에서 하는 SSA 기 반의 아키 텍처 비종속적 인 최 적화와
후단부에서 하는 RTL 기반 아키텍처 종속적인 최적화가 있다.
여기서는 SSA 기반의 아키텍처 비종속적인 최적화에 대해 이야기하고자 한다. SSA 기반
아키텍처 비종속적인 최적화는 다시 지역 최적화, 전역 최적화, 루프 최적화라는 3가지로
나눌 수 있다.
지역 최적화에서는 공통 부분식의 제거, 연산 강도 경감, 상수 계산 등을 통해 최적화
를 실현한다. 예를 들면 곱하기 연산 중 쉬프트 연산으로 바꿀 수 있는 것은 바꾸고,

var=5+3；을 var=8；과 같이 미 리 상수로 바꿀 수 있는 것은 바꾼다.
저역 최적화에서는 공통 부분식을 제거하고 사용되지 않는 코드를 제거한다. 루프 최적
화에서는 루프 내에서 불변하는 코드를 루프 밖으로 빼버리거나, 합칠 수 있는 루프는
하나로 합치는 등의 일을 통해 최적화를 가능하게 한다.
이런 최적화들에 대해 자세하게 독자에게 알려주면 분명 도움이 될 것이다. 하지만 이
런 최적화를 설명하기에는 양이 너무 많고 복잡하기 때문에 이 책의 범위를 벗어난다.
그래서 필자는 중단부에서 어떤 종류의 최적화를 수행하는지 대표적인 최적화만 정리
하고, 꼭 설명이 필요한 최적화에 대해서는 “gcc 를 이용한 최적화” 절에서 각각 따로
설명하겠다.
다음은 중단부에서 수행하는 아키텍처 비종속적인 최적화의 리스트다.
• 각종 반환 값 최적화(return value optimizations)
• 전체 중복성 제거 (full redundancy elimination)

4장_ gcc compiler 195

===== PAGE 197 =====
• 조건부 상수 전파(conditional constant propagation)
• 데드 코드 제거 (dead code elimination)
• 복’사 전파(copy propagation)

• value range propagation
• branch prediction and profiling
• dead store elimination
• 기타
이런 최적화 과정을 통해 CTest.c 파일이 어떤 형태로 변경되는지 궁금한 독자가 있다
면 CTest.c .t28.ssa 이후로 하나씩 열어보면서 확인해 보기 바란다. 최종 단계에서 재미
있는 변화를 발견할 수 있을 것이다.
그리고 지면 관계상 생략했지만 SSA 기반 최적화 이전에 인터프로시저 분석 (IPA ：

inter-procedural analysis) 이라는 단계가 더 있다. 인터프로시저 분석에서는 함수
inline을 수행하기도 하고, 동적 프로파일링 코드를 삽입하기도 하고, 포인터 분석을 위
한 프로파일링 코드 등을 삽입하기도 한다. 이런 프로파일링 코드들은 나중에 배우게
될 gcov나 gprof 같은 프로파일링 분석 툴에서 사용된다.
이런 인터프로시저 분석에서 생성하는 중간 파일들은 -fdump-ipa-all 이라는 옵션을
주면 확인할 수 있다.
이제 앞에서 열거한 중단부의 최적화 과정이 끝났으며, 마지막으로 후단부에서 사용할

RTL을 생성한다.
►

RTL 생성

RTL(Register Transfer Language)은 GCC에서 기계 독립적인 특성을 제공하기 위해
사용하는 중간 표현의 한 형태다. RTL은 여러 중간 표현 형태 종류 중 3-address 코드
형태이고 lisp 언어를 기반으로 하고 있어 lisp 언어와 형태적으로 유사하다. 하지만 형
태적으로 유사할 뿐이지 문법적으로는 많이 다르다.

RTL 은 후단부의 최적화 과정에서 사용되는 중간 표현인데, 레지스터 전송 언어
(Register Transfer Language) 라는 이름에서 알 수 있듯이 레지스터 레벨의 연산과
오퍼랜드로 표현된다. 때문에 형식이 거의 어셈블리 언어와 유사하다. 하지만 특정 아
키텍처에 종속적이지 않고 많은 아키텍처를 포용할 수 있게 설계되었다.
간단한 예로 a=b+c；처럼 사용된 코드는 다음과 같은 RTL 표현으로 바뀐다.

196 3부_ 컴파일과링킹

===== PAGE 198 =====
〔예제 4-18)

a=b+c；의 RTL 표현

(insn 12 11 13 1 (set (reg:SI 62)
(mem/c/i:SI (plus:SI (reg/f:SI 54 virtual-stack-vars)
(const_int -4 [Oxfffffffc])) [0 c+0 S4 A32])) -1 (nil)
(nil) )
(insn 13 12 14 1 (parallel [
(set (reg:SI 61)
(plus:SI
virtual-stack-vars)

(mem/c/i:SI

(plus:SI

(reg/f:SI

54

(const_int -8 [0xfffffff8])) [0 b+0 S4 A32])
(reg:SI 62)))
(clobber (reg:CC 17 flags) )
]) -1 (nil)
(nil))
(insn 14 13 15 1 (set (mem/c/i:SI (plus:SI (reg/f:SI 54 virtualstack-vars)
(const_int
-12
[Oxfffffff4]))
[0
a+0
(reg:SI 61)) -1 (nil)
(expr_list:REG_EQUAL (plus:SI (mem/c/i:SI (plus:SI (reg/f:SI 54
virtual-stack-vars)
(const_int -8 [0xfffffff8])) [0 b+0 S4 A32])
(mem/c/i:SI (plus:SI (reg/f:SI 54 virtual-stack-vars)
(const_int -4 [Oxfffffffc])) [0 c+0 S4 A32]))
(nil)))

S4

A32])

like.c 소스의 RTL 표현을 보고 싶은 독자는 다음 명 령으로 RTL 표현을 볼 수 있다.
$ gcc “O like like.c -da

위 명령을 내리면 like.c.OO.expand 파일이 생성되는데, like.c.OO.expand에 like.c의

RTL 표현을 볼 수 있다. 낮은 버전의 gcc를 사용한다면 like.c.OO.expand 파일이 생기
지 않을 수도 있다. 그렇다면 like.c.xx.rtl 파일을 열어보기 바란다.

RTL 파일을 열어보면 그렇게 보이진 않겠지만 어셈블리 파일이라고 볼 수도 있다. 사실
이 파일은 RTL에서 정의하는 아키텍처의 머신 코드다. 이 아키텍처는 가상의 아키텍처
로서 레지스터 개수가 무한대이고, 여러 연산자와 여러 메모리 액세스 방법을 지원한다.
우선 이 기본 RTL 코드를 사용해 최적화 과정을 수행하면서 실제 아키텍처에 맞게 연
산자와 메모리 액세스 방식을 변경해 나간다. 그리고 마지막에는 가상의 레지스터들을
실제 물리 레지스터에 맵핑하고 실제 타겟 머신의 어셈블리 파일로 변환해 컴파일 과
정을 마무리한다.

4장_ gcc compiler

197

===== PAGE 199 =====
이런 RTL 표현은 gcc를 포팅하거나 디버깅할 때는 반드시 이해해야 하지만 그렇지 않
을 때는 굳이 알 필요는 없다. 혹시라도 궁금한 사'람이 있다면 http://gcc.gnu.org/

onlinedocs/gccint에서 gcc 문서를 읽어보기 바란다.
-fdump-tree-aU 옵션과 마찬가지로 -da 옵션 역시 아무런 최적화 옵션을 주지 않으
면 중간의 최적화 과정을 생략해 컴파일 과정 번호가 중간 중간 비는 것을 확인할 수
있을 것이다. 모든 과정의 RTL 표현을 덤프하려면 -03 옵션을 지정한다.

gcc는 애초 설계에서부터 많은 아키텍처를 지원하기 위해 설계된 컴파일러다. 그래서
포팅이 비교적 쉽게 되어 있고 현존하는 아키텍처에 대해 많은 부분을 포용할 수 있게
되어 있다.

gcc가 이렇게 많은 아키 텍처를 지원할 수 있게 된 이유는 전/중단부와 후단부가 잘 나눠져
있고, RT1 표현에서 많은 아키텍처의 특징을 표현할 수 있는 확장을 제공하기 때문이다.
: gcc가 이렇게 많은 아키텍처를 지원하기 위해 설계되다 보니 성능 면에서는 아무래도 해당 아키텍처에
특화된 컴파일러보다는 떨어질 수밖에 없다. 예를 들면 gcc는 인텔이 만든 x86 아키텍처 전용 컴파일러
인 icc보다는 x86 아키텍처에서 최적화 성능이 떨어지고, ARM용 크로스 컴파일러인 arm-linux-gcc
는 ARM 아키텍처 전용 컴파일러인 armcc보다 ARM 아키텍처에서 최적화 성능이 떨어진다.
그렇지만 하나의 컴파일러가 이렇게 많은 아키텍처를 지원하고, 또한 비교적 성능을 잘 내고, 무료인 것
은 gcc가유일하다.
앞으로 나올 새로운 아키텍처 등도 gcc가 지원 가능함과 동시에 성능을 잘 낼지는 두고 볼일이지만(현
재로는 많이 모자란 감이 있다), 현재 지원하는 아키텍처만으로도 gcc는 매우 매력적인 컴파일러임에는
분명하다.

RTL을 생성하는 것으로써 중단부에서 하는 일이 모두 끝났다. 정리해 보면 전단부에서
넘겨받은 GIMPLE 트리를 SSA로 변환하고 SSA 기반 아키텍처 비종속적인 최적화를
수행한 후 최종적으로 RTL로 변환하는 것이 중단부에서 하는 일이다.

@ CC1 후단부에서 하는 일
중단부에서 RTL이 전달되면 후단부(back-end)에서는 RTL로 다음과 같은 일을 수행
한다.

[그림 4-24] 후단부에서 하는 일

198 3부—컴파일과링킹

===== PAGE 200 =====
후단부에서 하는 가장 중요한 일은 RTL을 이용해 최적화를 수행하는 일과 실제 목적
코드(타겟 아키텍처 어셈블리)를 생성하는 일이다. RTL 최적화에는 아키텍처 비종속적
인 최적화와 아키텍처 종속적인 최적화가 같이 이뤄진다. 그리고 인스트럭션 스케줄링
과 레지스터 할당, 함수의 프롤로그와 에필로그를 붙여 넣는 일도 후단부에서 하는 중
요한 일 중 하나다.

►

RTL 최적화

이전까지는 아키텍처 비종속적인 최적화만 수행하였다 . 후단부에서는 아키텍처 비종속
적인 최적화도 하지만 아키텍처 종속적인 최적화도 함께 수행한다.
대표적인 아키텍처 종속적인 최적화가 핍홀 (peephole) 최적화의 일종인 기계 숙어

(Machine idioms) 변환인데, 여러 인스트럭션을 아키텍처에서 지원하는 하나의 인스
트럭션으로 바꾸는 기법이다.
예를 들면 DSP 계열 프로그래밍에서는 알고리즘 특성상 곱한 값을 다시 더하는 경우
가 빈번하게 발생하는데, 이 럴 경우 mul 인스트럭션 다음에 add 인스트럭션이 오는 패
턴이 자주 반복된다. 목적 코드를 생성할 타겟 아키텍처에서 곱하고 더하는 것을 한 번
에 할수 있는 mac (Multiply and Accumulate： 곱하고 더하는 인스트럭션) 인스트럭
션을 지원한다면 이런 두 개의 연산에 대해 모두 mac 인스트럭션 하나로 바꿀 수 있다.
하지만 이런 일은 해당 아키텍처에서 mac 연산을 지원해야만 가능하다. 이렇게 아키 텍
처의 특성을 타는 최적화를 아키텍처 종속적인 최적화라 한다.
이런 아키텍처 종속적인 최적화의 방법에는 효율적인 레지스터 할당과 효율적인 인스
트럭션 선택, 메모리 접근의 최적화 및 연산 순서 조절 등 여러 가지 방법이 있다. cel
의 후단부에서 수행하는 RTL 최적화에는 다음과 같은 종류가 있다.
• 각종 고전 최적화
• 공통 부분식 제거 (Common Subexpression Elimination)

• GCSE/PRE
• 상수 전파(Constant Propagation)
• 복사 전파(Copy Propagation)
• 각종 제어 흐름 그래프 최적화(cross-jumping, block merging)
• 베이직 블록 재정렬(Basic Block Reordering)

• if 변환(IF-Conversion)

4장_ gcc compiler

199

===== PAGE 201 =====
• 각종 loop 최적화

• loop 풀기 (Loop Unrolling)
• 연산 강도 경감

• loop 내의 불변 코드 옮김 (Invariant Code Motion)
• 각 명령의 실행 사이클을 고려한 인스트럭션 스케줄링(Instruction Scheduling)
• 레지스터 할당(Register Allocation)

• Satisfying operand constraints
위에 나오는 최적화 중에서 주의 깊게 보아야 할 것은 바로 레지스터 할당이다. 레지스
터 할당은 RTL(Register Transfer Language)을 실제 목적 크= 루 변환하기 위해서 꼭
필요한, 중요한 일 중 하나다.

RTL은 최초 타겟 아키 텍처가 무한 개의 가상 레지스터를 가진 것으로 전제하고 생성되
는데, 코드 내에 사용된 지역변수라든지 SSA나 여러 최적화 기법을 통해 생성되는 임
시 변수들이 모두 가상 레지스터에 할당된다.
이후 이런 가상 레지스터들은 레지스터 할당을 통해 실제 물리 레지스터 또는 메모리
로 바뀐다. 이렇게 최초의 모든 지역변수와 임시 변수를 가상 레지스터에 할당하는 이
유는 최적화에 용이하기 때문이다.
레지스터 할당이란 이런 무한한 가상 레지스터를 사용하게 작성된 코드를 실제 아키텍
처에 있는 제한된 개수의 물리 레지스터를 사용하게 바꾸는 일이다. 제한된 물리 레지
스터를 효율적으로 할당하는 일은 쉬운 일이 아니다. 물리 레지스터에 할당할 수 있는
것은 할당하고, 그렇지 못한 것들은 메모리에 할당한다. 이렇게 메모리에 할당하는 것
을 스필 (spill) 이라 한다. 그리고 가장 효율적인 레지스터 할당 방법을 찾는 것은 NP-

complete한 문제라서 딱히 그 해법이 나와 있지 않다. 때문에 휴리스틱 알고리즘을 사
용하는데, 그래프 컬러링과 같은 기법을 사용한다.
레지스터 할당에 대해서는 설명하였고, 그 외 나머지 최적화 기법에 대해서는 “gcc를
이용한 최적화” 과정에서 꼭 필요한 것만 설명하겠다. 좀 더 많이 알고 싶고 관심 있는
독자들은 되도록 개인적으로 찾아보기 바란다. 이런 최적화 기법들을 잘 알게 되면 프
로그래밍하는 습관이 달라지고 시스템을 이해하는 폭이 넓어진다.

200 3부- 컴파일과링킹

===== PAGE 202 =====
► 목적 코드 생성

RTL 최적화를 통해 아키텍처 종속적인 최적화까지 수행했다면 이제 실제 목적 코드를
생성할 차례다. 목적 코드는 타겟 아키텍처의 어셈블리 코드로서 이후 어셈블러(as)에
의해 인스트럭션으로 변환된다. 목적 코드의 생성은 ［그림 4-24］ 에 보이는 코드 생성
기(Code Generator)가 담당한다. 최적화와 레지스터 할당까지 끝난 RTL은 문법만 다
르게 보일 뿐이지 실제로는 목적 코드와 거의 유사하다. 때문에 코드 생성기는 어렵지
않게 RTL을 목적 코드인 어셈블리 코드로 변환할 수 있다.

［그림 4-25］ 컴파일 과정이 끝난 like.s 파일의 내용

이제 ccl C 컴파일러에 의한 컴파일 과정이 모두 끝났다. gcc에 의한 컴파일 과정에서
거의 모든 부분은 CC1 에서 일어난다. 때문에 다소 설명이 길어질 수밖에 없었다.
하지만 여기서 우리가 주목해야 될 것은 CC1 의 컴파일 과정에서 문법 체크와 최적화
과정, 목적 코드 생성이 일어난다는 것이다. 그래서 CC1 의 옵션 조정으로 문법 체크
수위라든지, 최적화 수위, 불필요한 문법적 경고 메시지를 제거하는 등의 일이 가능
하다.

4장_ gcc compiler 201

===== PAGE 203 =====
I as에 의한 기계어 코드 생성
이제 컴파일이 끝난 어셈블리 코드는 as에 의해 기계어로 어셈블된다. gcc -o like

like.c -v -save-temps 명령으로 gcc가 내리는 어셈블 명령은 다음과 같다.
as -V -Qy -o like.o like.s

as에 의해 생성되는 like.o 파일은 어셈블된 like.s의 인스트럭션과 데이터가 들어있는
ELF 바이너리 포맷 구조를 가진다. 바이너리 포맷이란 바이너리 파일의 구조를 결정짓
는 규약을 말한다. 바이너 리 포맷이 필요한 이유는 다음과 같다.
우리가 링커가 되었다고 가정하고 링커의 입장에서 여러 오브젝트 파일을 링킹한다고
생각해 보자. 여러 바이너리가 일정한 규칙을 가지고 있지 않고 제멋대로 되어 있다면
링킹하기가 쉽지 않을 것이다.
바이너리 파일의 구조를 알아야만 어디서 어디까지가 인스트럭션이고, 어디서 어디까
지가 데이터인지 알 수 있을 것이다. 그리고 어떻게든 링킹을 해서 실행 파일을 만들어
냈다고 치고 커널 로더（ execveO 시스템 콜）에 의해 실행한다고 가정해 보자. 커널 로
더 역시 아무런 정보가 없다면 실행 파일을 메모리에 어떻게 올려야 할지 어디서부터
실행시켜야 할지 알 수 없을 것이다.
이렇게 오브젝트 파일이나 실행 파일은 그 자체로서 링커나 로더에게 정보를 제공해야
만 링킹하고, 로드하고, 실행할 수 있는 것이다. 물론 그러려면 바이너리 파일이 일정한
규칙을 가지는 구조로 되어 있어야 하고 바이너리 스스로 정보를 제공할 수 있어야 가
능하다. 그렇기 때문에 바이너리 포맷이 필요한 것이다. 이런 바이너리 포맷에는 유닉스
시스템의 경우 a.out, ELF, COFF 정도가 있고, 윈도우즈 시스템에서는 COFF, PE 포맷
이 사용된다.

a.out은 과거 유닉스 시스템에서 사용하던 포맷인데, 확장성의 한계와 동적 링킹이 어
렵다는 이유로 지금은 거의 사용되지 않고 있다. 그리고 COFF 포맷은 한동안 사용되
다가 좀 더 나은 ELF 포맷이 등장함으로써 거의 사용되지 않고 있다. 대부분 현재 나오
는 유닉스 계열 시스템은 대부분 ELF 포맷을 사용한다. ELF 포맷은 나중에 자세히 다
룬다.

as에 의해 생성되는 재배치 가능한 ELF 포맷으로 되어 있는 like.o 파일은 다음과 같은
구조를 가지고 있다.

202 3부- 컴파일과 링킹

===== PAGE 204 =====
뭔가 복잡하다. 다 볼 필요 없고 지금은 .text, .data, .rodata, .bss 부분만 이해하면 된
다. .text 영역은 텍스트 섹션으로, like.c의 인스트럭션이 들어있는 부분이다. .data 영
역은 데이터 섹션으로, like.c의 데이터가 들어있는 부분이다. 현재 like.c 소스 코드에
서는 데이터 섹션에 잡힐만한 초기 값이 0이 아닌 전역변수가 없기 때문에 데이터 섹션
에는 아무것도 들어 있지 않다.
그리고 BSS 섹션은 초기 값이 0인 전역변수에 할당되는 공간인데, 역시 like.c 소스에
는 그런 변수가 없기 때문에 BSS 섹션에 아무것도 들어있지 않다.
마지막으로 “I like you.\n”처럼 변하지 않는 데이터들은 모두 .rodata라고 표시된 읽기
전용 데이터 (read only) 섹션에 들어간다. like.o 파일은 이런 구조를 가지고 있고, 나
머지 섹션들에 대해서는 ELF 포맷을 설명하면서 자세히 다룬다.

as 는 오브젝트 파일의 제일 처음에 ELF (Executable and Linking Format) 헤더를 붙
인다. ELF 헤더에는 바이너리의 특징을 결정짓는 엔디안, 운영체제, CPU의 정보와 함
께 바이너리 내부에 있는 각 구역의 시작 위치와 크기 정보가 들어 있다. 다음은 readelf

-a like.o 명 령으로 살펴본 like.o 파일의 ELF 헤더 정보다.

4장_ gcc compiler

203

===== PAGE 205 =====
[그림 4-27] like.o 파일의 ELF 헤더 정보

readelf 명령은 ELF 포맷 바이너리의 정보를 보기 위한 명령인데, 바로 사용할 수 없을
것이다. like.o 파일이 없기 때문이다. gcc -c like.c 명령으로 like.o 파일을 만들고 나
서 readelf -a like.o하면 이런 정보를 볼 수 있다.

ELF 헤더 다음에는 프로그램 헤더 테이블을 붙이는데. like.o처럼 재배치 가능한 오브
젝트에는 보통 프로그램 헤더 테이블이 없고 like 실행 바이너리 같은 것들에는 있다.
프로그램 헤더 테이블은 커널 로더에 필요한 정보를 제공하는 테이블로, 프로그램을 섹
션 단위가 아닌 세그먼트 단위로 보여준다.
프로그램 헤더 테이블 다음에는 텍스트 섹션이 오는데, 여기에는 like.s를 어셈블해 만
들어진 인스트럭션을 붙인다. “lea 0x4（ %esp） , %ecx”와 같은 어셈블리 명령들이 숫
자（인스트럭션）로 표현되어 붙는다.
다음으로 오는 데이터 섹션에는 like.s의 데이터들이 들어간다. 물론 like.c 파일에는 전
역변수를 사용하지 않아 이 부분은 비어있다. 그리고 BSS 섹션 역시 전역변수가 사용
되지 않았기 때문에 비어있다. 다음에 읽기 전용 데이터 섹션에 내부에서 사용된 문자
열 “I like you!\n”가 들어간다.
그리고 나머지 기타 섹션（심볼 테이블, 스트링 테이블, 각종 재배치 섹션 등）들이 오
게 된다. 이런 나머지 섹션들은 링커, 로더, 디버거에게 정보를 제공하기 위한 섹션들
로 구성된다. like.o의 기타 섹션으로는 심볼 테이블과 재배치 섹션 등이 있다. 심볼 테
이블은 like.c 파일 내부에 사용된 심볼들의 정보가 들어있는 테이블이다. 여기서 심볼
은 메모리상의 주소를 가지는 모든 것을 의미한다. 전역변수나 함수, 전역 구조체, 정적
변수 모두 메모리상에 공간이 할당되면 주소를 가진다. 심볼 테이블에는 이런 전역변

204

3부_ 컴파일과 링킹

===== PAGE 206 =====
수나 함수, 전역 구조체, 정적 변수들의 이름, 크기와 종류, 전역인가 지역인가를 의미
하는 스코프 등의 정보가 들어 있다. like.c 같은 경우에 전역변수가 사용되지 않았기 때
문에 like.o 파일의 심볼 테이블을 readelf -s like.o 명령.. 0 -루 읽어보면 puts() 함수와

mainO 같은 함수 심볼의 정보만 들어 있음을 확인할 수 있다.
root@os：/temp/like
[root（흐os
Symbol table '.symtab*
jm:
Ualue
0: 00000000
1: 08000000
2： 00000000
3: 00000800
1*: 00080000
00000000
00000080
80008000
00000000
00000000
[rootSos like]tt |

readelF -s like.o

Size
0
0
0
0
0
0
0
0
43
0

contains 10 entries:
Bind
Type
NOTVPE
LOCAL
LOCAL
FILE
SECTION LOCAL
SECTION LOCAL
SECTION LOCAL
SECTION LOCAL
SECTION LOCAL
SECTION LOCAL
FUNC
GLOBAL
NOTVPE
GLOBAL

Uis
DEFAULT
DEFAULT
DEFfiULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT

Ndx
UHD
ABS
1
3
4
5
7
6
1
UND

Name
like .1

main |
P니ts 1

［그림 4-28］ like.o 파일의 심볼 테이블

어라! 그런데 like.c 파일에는 분명히 printfO 함수를 사용했는데, 왜 printfO 함수는
안 보이고 사용하지도 않은 puts() 함수가 보이는 걸까?
이것은 printfO 함수를 puts() 함수로 gcc가 내부적으로 변경하였기 때문이다. gcc는
내부적으로 빌트인 함수(builtin function)라고 하는 gcc 자체적.0-루- 제공하는 내장 함
수가 있다. 이런 빌트인 함수들은 __builtin_［ 함수명］() 형식의 이름을 가지는데, gcc의
여러 향상된 확장 기능을 제공하기 위해 사용된다.
대표적인 경우로 __builtin_expect() 함수와 __builtin_prefetch() 함수가 있는데, 둘
다 최적화를 위해 사용된다. __■builtirvexpect(［조건식］) 함수는 조건식에서 자주 발
생할 예상 결과를 컴파일러에게 알려줘 좀 더 최적화된 코드를 생성할 수 있게 하고,

_builtin_prefetch() 함수는 조만간 사용될 것으로 예상되는 데이터를 캐시(cache)에
미리 가져오게 명시적으로 지정할 때 사용한다.

__builtin_expect() 함수와 __builtin_j>refetch() 함수는 프로그래머가 명시적으로 지
정해 줘야 하지만, 문자열만 인자로 사용한 printf(［문자열］)문에 대해서는 gcc가 임의
로 _］ ?uiltin_puts(［문자열］) 함수 또는 _builtin_putchar(［문자열］)로 변경해 준다.

printf("test\n")와 같이 문자열이 여러 문자로 이루어졌고 \n이 있는 경우에는
__builtin_puts("test\n") 함수로 변경되고, printf("c”)와 같이 하나의 문자로만 이루어
진 경우에는 __builtin_putchar(99) 함수로 바뀐다. 이렇게 변경된 __builtin_puts()
함수와 __builtin_putchar() 함수는 나중에 puts() 함수와 putchar() 함수로 변경된다.
4장_ gcc compiler 205

===== PAGE 207 =====
이런 빌트인 확장이 일어나는 것은 이미 잘 알려진 몇몇 함수 ( p ri ntf, fprintf, sprintf,

fputs 등)에 대해 해당 함수가 내부적으로 어떤 함수와 같은 기능을 제공한다는 것을
gcc가 이미 알고 있다고 전제하고 gcc의 코드가 작성되 었기 때문이다.
빌트인 확장이 일어나는 시점과 해당하는 함수의 종류는 gcc 버전에 따라 다 다르고,
우리가 사용하는 gcc-4.1.x는 GIMPLE 트리를 만드는 시점에서 일어나고, gcc-4.0.x에
서는 RTL을 만드는 시점에서 일어난다.
〔예제 4-19)

test.c 파일 내용

#include <stdio.h>
int main()
{
char buffer[10];
printf("test\n");
printf("c");
sprintf(buffer, ”%s", "test”);
return 0;

[예제 4-19]의 test.c 파일을 작성하고 다음 명령을 내리면 지금까지 설명한 내용을 직
접 눈으로 확인할 수 있다.
$ gcc -o test test.c -fdump-tree-all -da

gcc-4.1.x 버전인 경우에는 test.c.t03.gimple 파일을 열어보고, gcc-4.0.x 버전인 경우
에는 test.c.00,expand 파일을 열어보면 다음과 같은 결과를 확인할 수 있다. 변환되지
않으면 -o2 최적화 옵션을 추가해 보기 바란다.
〔예제 4-20〕 gcc-4丄x 버전으로 컴파일했을 때 test.c.t03.gimple 파일의 내용

main ()

：

{

；
int D.1780;
char buffer[10];
__ builtin_puts (&"test"[0]);
__builtin_putchar (99);
__builtin_memcpy (&buffer, &"test"[0], 5);
571780 = O’;
return D.1780;

}

이런 빌트인 확장이 일어나는 게 싫다면 컴파일 시 -fno-builtin 옵션을 추가하자.

206 3부_ 컴파일과 링킹

：
：

===== PAGE 208 =====
다시 컴파일 과정으로 돌아와 심볼 테이블 다음으로 Relocation 섹션 즉, 재배치 섹션
이 들어간다. 현재 l&e.c에서 printfO 함수가 사용되고 최종적으로 puts() 함수로 변경
되었지만 아직 puts() 함수가 링크되지는 않았다. 그래서 아직까지는 puts 심볼의 주소
가 어떻게 될지 모르는 상황이므로 ［그림 4-29］ 와 같이 readelf -r like.o 명령으로 살
펴본 결과에서 심볼 값이 0으로 설정되어 있는 것을 확인할 수 있다. 이후 링커에 의해

puts 의 주소는 재배치되어야 한다. 이렇게 재배치해야 되는 심볼의 정보가 들어있는
위치가 바로 재배치 섹션이다. 다음은 like.o 파일의 재배치 섹션의 정보다. 재배치해야
될 심볼이 puts() 함수밖에 없어 재배치 텍스트(.rel.text) 섹션만 존재한다.

[그림 4-29] like.o 파일의 Relocation 섹션 정보

지금까지 컴파일 과정에서 알아야 되는 섹션에 대한 설명은 다 한 것 같다. 나머지 섹션
들은 ELF 바이너리 포맷을 설명하면서 설명한다. 다음은 xxd like.o 명령. 0 -루 like.o
파일의 전체 내용을 본 모습이다. 지금까지 설명 한 구조가 한눈에 보일 것이다.
———

® root@os：7temp/like
7F45 4c46 0101 0100 0000 0000 0000
0100 0300 0100 0000 8000 0000 0000
ec00 0000 0880 0888 348B 8B0B B80B 28B0
쁘으흐 08B이8d4c 2404 83e4 F0FF 71Fc 5589
e551
83ec
04c7
0424
0000
0000
e8fc
Ffb8 0008 0000 83c4 0459 5d8d 61Fc c300
4920 6c69 6b65 2079 6f75 218fl 00^7 4343
3a28 2847 4e55 2920 342e 312e 3220
3037 3039 3235 2028 5265 6420 4861
342e 312e 322d 3237 2900 002e 7379
6162 0O2e 7374 7274 6162 002e 7368
7274 6162 002e 7265 6c2e 7465 7874
6461 7461
002e 6273 7300 2e72 6f64
6100 2e63 6F6d 6d65 6e74 002e 6e6f
2e47 4e55 2d73 7461 636b 0000 0000
0000 0000 0000 0000 0000 0000 0000
0000 0000 0000 0000 0000 0000 0000 0000

1EF 저폐
텍

더
0006888：
0009090：
8088030：
88808b0：
00008c0:
00O0Od8：
0000060：
88000f0：

|타 섹션 1
(심:콜 테이블, 1 0000 0000 0100 0000 0200 0000 0000
재배?디 섹션들, 0000 0000 3402 0000 3000 0000 0a00
1타 섹션, j 0800 0000 0400 0000 1W0 0000 09 00
섹;녀 테이블) ］0300 8000 0000 0000 0000 0000 4403 0000
0000230：
80002b8：
08002c8：
8300200：
88302&0：
8O802F8：
0088308：
0000310：
0000320：
8000330：
8889340：
000035B：
0080368：

1200 0000 0000 0000 0000 0000 0100 0000
0000 0000 0000 0000 0000 0000
000s 0000 0100 0000 0000 0008
0400 f1FF 0900 0000 0000 0000
0300 0100 0000 0000 0000 0080
0300 0300 0000 0000 0000 0000
0300 0400 0000 0000 0000 0000
0300 0500 0000 0800 0000 0000
0300 0700 0000 0008 0000 0000
0300 0600 0800 0000 WOO 0000
1200 0100 OdOO 0000 0000 0000
1000 0000 006c 696b 652e 6300
0070 7574 7300 0000 1400 0000
1900 0000 0209 8000

0000
0000
0000
0000
0000
0000
0000
0000
2b00
0000
6d61
0105

0000
0000

싀믜씌
ELF

U
FffF

3230
7420
6d74
7374
002e
6174
7465
0000
0000

................ V]
like 少ou!
.GCC
: (GNU) 4.1 2 20
070925
(Red Hat
4.1.2-27)..
symt
ab. .strtab.
1shst
rtab.
.rel.text..
data.
.bss..rodat
a..comment..note
.GNU-stack....................

0000
0000
0000

0000
0000
0000
0000
0000
0000
0000
0000
WW
0000
696e
0000

........... like.c.main
.puts................................
1,1

모두 티

［그림 4-30］ xxd like.o 명령으로 본 like.o 파일의 구조
4장_ gcc compiler

207

===== PAGE 209 =====
그리고 비교를 위해 like.o의 인스트럭션을 첨부한다.
IMEW1 objdump -S like.o 명령으로 본 like.o의 인스트럭션

...상략

int main()
{
0:
4:
7:
a:
b:
d:
e:

8d 4c 24 04
83 e4 fO
ff 71 fc
55
89 e5
51
83 ec 04
printf("I like you!\n");
11:
c7 04 24 00 00 00 00
18:
e8 fc ff ff ff
return 0;
Id: b8 00 00 00 00

lea
and
pushl
push
mov
push
sub

0x4 (%esp),%ecx
$0xfffffff0,%esp
Oxfffffffc(%ecx)
% ebp
%esp,%ebp
%ecx
$0x4,%esp

movl
call

$0x0,(%esp)
19 <main+0xl9>

mov

$0x0z %eax

22:
25:
26:
27:
2a:

add
pop
pop
lea
ret

$0x4,%esp
%ecx
% ebp
Oxfffffffc(%ecx),%esp

j
83 c4 04
59
5d
8d 61 fc
c3

텍스트 섹션의 인스트럭션이 들어 있는 것을 확인할 수 있다.

I collect에 의한 링킹 과정
as에 의해 ELF 포맷의 오브젝트 파일이 만들어졌으면 링커에 의해 표준 C 라이브러리
와 링크된다.
구 버전 gcc 는 내부적으로 Id 를 직접 호출해 링크했지만, 최신 버전 gcc는 collect2에
서 내부적으로 진짜 링커인 Id를 호출해 링크한다. 링크를 왜 하는지 모르는 독자는 없
을 거라 생각한다. like.o 파일에서는 puts() 함수를 사용하고 있다. puts() 함수는 분명
소스 파일 내에 구현하지 않았기 때문에 그냥은 사용할 수 없다.

puts() 함수는 표준 C 라이브러리 내에 공유 라이브러리 혹은 정적 라이브러리 안에
오브젝트 파일 형태로 들어있다. 여기서 잠깐 공유 라이브러리가 무엇이고 정적 라이브
러리가무엇인지 알아보자.

208 3부_ 컴파일과 링킹

===== PAGE 210 =====
01

정적 라이브러리

먼저 라이브러리란, 프로그래밍에 사용할 수 있게 미리 만들어져 있는 함수나 변수들의
묶음을 의미한다. 이런 함수나 변수들은 미리 컴파일되어 있어 소스 파일의 컴파일 과
정에서 링크만 하면 바로 사용할 수 있다.
기본적으로 C에서 바로 사용할 수 있는 puts(), printfO, scanf(), read(), write(),

memcpyO, strcpyO 등의 함수가 모여 있는 라이브러리를 표준 C 라이브러리라 하고,
별도로 컴파일 과정에서 링크하지 않아도 자동으로 링크된다.
그래서 C 소스를 작성할 때 puts(), printfO 함수와 같은 것들을 마음껏 사용할 수 있
는 것이다.
먼저 정적 라이브러리는 이런 puts(), printfO, scanf(), read(), write() 등의 함수들이
오브젝트 파일로 컴파일되어 하나의 파일로 묶여 있는 형태를 말한다. 이런 정적 라이
브러리는 “lib［라이브러리 이름］.a” 형식의 이름(확장자가 .a)을 가지는데, 표준 C 라이
브러리의 경우 libc.a란 이름으로 /usr/lib 디렉토리에 위치한다. 다른 예로 수학 함수
를 지원하는 math 정적 라이브러리는 /usr/lib/libm.a 형태로 존재한다. 그럼 이런 정
적 라이브러리 안에 실제로 puts() 함수나 printfO 함수, scanfO 함수의 오브젝트 파
일이 존재하는지 알아보자.
mkdir libc
cd libc
cp /usr/lib/libc.a ./
ar -x libc.a

# 임시 디렉토리 생성

# ar -x 명령으로 libc.a 파일을푼다.

위 명령을 차례로 내리면 /usr/lib/Ubc.a 라이브러리를 풀어 Ubc.a 파일이 어떤 파일들
로 묶여 있는지 알 수 있다. ［그림 4-23］ 에서 보는 바와 같이 Ubc.a 파일은 수많은 오브
젝트 파일들로 묶여 있는 것을 확인할 수 있고, 그 속에는 우리에게 친숙한 printfO라
든지 strcmpO, strcpyO, memcpyO 등과 같은 함수들의 오브젝트(printf.o, strcmp.o
등) 파일도 찾을 수 있을 것이다.
그 중에서 ioputs.o 파일이 있는데, ioputs.o에 puts() 함수가 들어 있다. 궁금한 독자는

nm ioputs.o 명 령으로 ioputs.o의 심볼 테이블을 읽어보기 바란다(nm 명령은 심볼 테
이블을 읽는 명령이다).

4장_ gcc compiler 209

===== PAGE 211 =====
® root@os：/temp/like/libc
nemcpp_chk.o
xmknod.o
memfrob.o
xmknodat.0
memmem.o
xpg-strerror.0
memmoue.o
xpg_basename.o
memmouechk.o
xstat.o
mempcpy.o
xstat64.o
mempcpychk .o
xstatconu.o
[root@os libc]tt Is ioputs.o printF.o strcmp.o
loputsTo memcpyTo printf.o ' stremp.o strepp.o I
[root@o：5''lLibc]1f

strc

py.o

me

me

p이

-

o

[그림 4-31] libc.a 파일에 묶여 있는 오브젝트 파일들

이렇게 묶여 있는 오브젝트들은 컴파일 과정에서 （ gcc 옵션으로 -static 옵션을 주면

libc.a와 링크한다） Uke.o와 링크되어 삽입된다. 다음은 like 바이너리 파일이 like.o,
printf.o, scanf.o 세 개의 오브젝트 파일로만 구성된다고 가정하고, collect』의 명령라
인에서 like.o printf.o scanf.o순으로 입력했을 때 생성되는 like 바이너리의 모습을 예
로 든 것이다. collect』는 내부적으로 링커인 Id를 호출해 링킹 과정을 수행하므로 실제
로는 다음 그림과 같이 Id에 의해 링킹 과정이 일어난다.
Id -o like like.o printf.o
like.o
like.o Text
like.o Data
like.o BSS

like 바이너리
like.o Text
*Text

printf.o
printf.o Text

printf.o Text
scanf.o Text

J

like.o Data
printf.o Data
printf.o Data
printf.o BSS
scanf.o
scanf.o Text

scanf.o Data

-Data

J

like.o BSS
>BSS
printf.o BSS

scanf.o Data

[그림 4-32] 정적 라이브러리를 이용한 링킹

Id는 입력되는 순서대로 각 오브젝트의 text 섹션과, data 섹션, bss 섹션을 순차적으로
붙이면서 like 바이너리를 구성한다. libc.a에는 여러 수많은 오브젝트가 있으므로 실제
로는 더 많은 오브젝트의 text, data, bss 섹션이 추가되고, 또한 위 그림에 표현되진 않
았지만 프로그램 수행 전에 초기화하고 종료할 때 사용하는 startup 코드가 실행 바이
너리 제일 앞과 뒤에 들어간다.

210 3부—컴파일과링킹

===== PAGE 212 =====
［그림 4-32］ 는 독자에게 어떤 식으로 오브젝트가 링크되는지 예를 보인 것이지 실제

like 바이너리의 모양이 그림과 같은 것은 아니다. 실제 모양은 어떤 파일이 링킹되고
그 순서가 어떤지를 알면 알 수 있기 때문에 이 컴파일러 과정 설명이 끝나면 누구나
쉽게 유추할 수 있을 것이다.
이렇게 정적 라이브러리를 이용해 컴파일하는 방식에는 단점이 있을 수 있다. 그것은
바로 각각의 실행 파일에 같은 오브젝트 파일이 중복되어 링크가 되기 때문에 실행 파
일의 크기가 커져 하드디스크의 공간을 낭비하고, 실행할 때 메모리의 공간도 낭비한다
는 점이다. 이런 정적 라이브러리의 결점을 보완하기 위해 나온 것이 바로 공유 라이브
러리라는 개념이다.

@ 공유 라이브러리

공유 라이브러리 역시 내부적으로 puts() 함수와 printfO, scanf() 함수들의 인스트럭
션을 가지고 있다. 공유 라이브러리는 정적 라이브러리와는 다르게 여러 함수의 ELF
오브젝트들이 묶여 있는 형 태가 아니라 여러 함수를 포함하는 하나의 큰 ELF 바이너리
형태다.
공유 라이브러리를 사용해 like.o 오브젝트와 링킹할 때는 like.o 오브젝트 내에

puts() 함수를 호출하는 부분에서 puts() 함수를 직접 호출하지는 않는다. 대신
PLT(Procedure Linkage Table) 섹션이라는 바이너리에 포함된 특정 영역을 호출하
게 링크한다.
이후 컴파일된 like 프로그램을 실행하면 execveO 시스템 콜은 like 프로그램의 ELF
헤더를 읽어 동적 링커를 사용한다는 정보를 얻고 like 프로그램 수행에 필요한 섹션들
과 함께 동적 링커 (/lib/ld-linux.so.2)도 같이 like 프로세스의 주소 공간에 로드한다.
동적 링커가 이미 메모리에 올라와 있다면 동적 링커의 메모리상 주소 공간만 like 프
로세스의 주소 공간에 맵핑한다.
그리고 제어권을 동적 링커에게 넘긴다. 이후 동적 링커는 like 바이너리에서 어떤 공유
라이브러리를 필요로 하는지 알아내고, 해당 공유 라이브러리들이 아직 메모리에 로딩
되어 있지 않다면 메모리에 로딩한다. 그리고 해당 공유 라이브러리들이 로딩된 메모리
상 주소 공간을 like 프로세스의 메모리 영역으로 맵핑한다.
그런 후 제어권이 다시 like 프로그램의 startup 코드로 넘어가면 비로소 like 프로그램
의 main() 함수가 수행된다. like 프로그램의 main() 함수 내에서는 puts() 함수를 호

4장_ gcc compiler 211

===== PAGE 213 =====
출하는 부분이 있고, 공유 라이브러리와 링킹 시 putsO 함수를 직접 호출하는 것이 아
니라 like 바이너리의 PLT(Procedure Linkage Table) 섹션에 있는 특정 엔트리를 호
출하게 되어 있어 PLT 섹션의 특정 엔트리가 호출된다.

PLT 섹션의 코드에는 like 바이너리에 포함된 GOT (Global Offset Table) 섹션(정
확하게 이야기하면 GOT.PLT 섹션임)이라는 특수한 영역의 puts() 함수 엔트리에 있
는 값을 인다이렉트(in-direct)로 해서 점프하게 작성되어 있는데, 초기 GOT(Global

Offset Table) 섹션의 puts() 함수 엔트리에는 최종적으로 동적 링커를 호출하는 주소
를 가지고 있다. 때문에 결국 like 바이너리의 main() 함수에서 공유 라이브러리에 있
는 putsO 함수가 처음 호출되면 동적 링커가 수행된다.
이후 동적 링커는 putsO 함수의 주소를 공유 라이브러리의 심볼 테이블에서 찾고, 찾
은 putsO 함수의 주소 값을 GOT(Global Offset Table) 섹션의 putsO 함수 엔트리에
저장하고, like 프로그램으로 가서 다시 putsO 함수를 호출한다. 이렇게 처음 공유 라
이브러리에 있는 함수가 호출될 때는 동적 링커가 실행되어 동적으로 링킹 과정이 일
어 난다.
이후에 putsO 함수가 다시 호출될 때는 GOT (Global Offset Table) 섹션의 putsO 함
수 엔트리에는 이미 공유 라이브러리의 putsO 함수의 실제 주소가 들어있기 때문에 동
적 링커를 거치지 않고 putsO 함수가 바로 호출된다.
지금까지 설명한 것이 공유 라이브러리 메커니즘이다. PLT나 GOT 같은 생소한 단어
가 나와 조금은 어색했을 거라 생각한다. PLT 섹션과 GOT 섹션은 ELF 바이너리 포맷
에 있는 섹션들로, 테이블 형태로 되어 있고 동적 링킹을 위해 반드시 필요한 섹션들이
다. PLT 섹션과 GOT 섹션은 ELF 바이너리 포맷을 설명할 때 따로 설명하겠다.

like 바이너리의 PLT(Procedure Linkage Table) 섹션의 내용과 GOT(Global Offset
Table) 섹션의 내용은 objdump -D like 명령 혹은 objdump -j .pit -D like와
objdump -j .got -s like 명 령으로 확인 가능하다. 궁금한 독자들은 한 번씩 확인해 보
기 바란다.
공유 라이브러리는 공유 라이브러리를 사용하는 프로세스가 하나라도 있다면 메모리
에 로딩되고, 공유 라이브러리를 사용하는 프로세스가 하나도 없기 전까지는 계속 메모
리에 상주한다. 그리고 공유 라이브러리를 사용하는 모든 프로세스는 이미 메모리에 로
드되어 있는 하나의 공유 라이브러리를 공유해 사용한다. 이렇게 하면 메모리를 절약하
고 하드디스크 공간을 절약할 수 있다는 장점이 있으므로 공유 라이브러리를 사용하는

212 3부_ 컴파일과링킹

===== PAGE 214 =====
일 역시 세계 평화에 기여하는 일이다. 이런 장점에도 불구하고 공유 라이브러리의 사
용에는 다음과 같은 단점이 있을 수 있다.
먼저 약간의 실행 속도 감소(아주 약간)가 있을 수 있다. 그리고 컴파일할 당시에 사용
한 공유 라이브러리가 없는 시스템이거나, 있더라도 라이브러리 메이저 버전이 다르
다면 실행되지 않을 수 있다. 표준 c 공유 라이브러리 파일은 시스템마다 틀린데, 페도
라 7 의 경우 /lib/libc.so.6 파일이고, 우분투 7.04 의 경우에는 /lib/tls/i686/cmov/libc.

so.6 파일이 표준 C 공유 라이브러리 파일이다. 공유 라이브러리는 “lib［라이브러리 이
름］.so.［메이저 버전］.［마이너 버전］.［패치 버전］”과 같은 형식의 이름(확장자가 .so)을
갖는다.
자신의 시스템에서 사용하는 표준 C 공유 라이브러리와 동적 링커는 컴파일된 like 바
이너리에서 Idd like 명령을 사용해 확인할 수 있다. 공유 라이브러리에 대한 좀 더 자
세한 내용은 라이브러리 제작 과정에서 설명한다.
다음 그림은 nm 명령으로 /lib/libc.so.6 파일에서 puts 심볼을 찾아본 예다. nm 명령
은 ELF 포맷 바이너리의 심볼 테이블을 보이는 명령으로, 바이너리 파일 내부에 어떤
함수와 전역변수, 구조체 등이 정의되었고, 메모리에 로딩되었을 때 어떤 주소 번지에
위치하는지를 확인할 때 사용하는 명령이다.
1 root@os：/temp/like
[rootdos like]tt nm /lib/libc.so.6 | grep puts
T _I0_fputs
423e45ao
423e5ab0
T _I0_puts
t 三GT_IO_fputs
423e45ao
423ed890
t __________________________
424642b0
t _argpfmtstreamputs
W Fputs
423e45ao
T Fputs unlocked
423ed890
423e5ab0 » puts |
42462480 T putspent
[root（흐os like]tt |

［그림 4-33］ nm 명령으로 살펴본 공유 라이브러리 내의 printf 함수

［그림 4-33］ 에서 볼 수 있듯이 /lib/libc.so.6 표준 C 공유 라이브러리에는 puts() 함
수가 있는 것을 확인할 수 있다. 다시 본론으로 돌아와 collect》에서 내부적으로 호출
되는 링커 Id는 like.o 내부에 사용된 puts() 함수를 사용하기 위해 표준 C 라이브러리

(libc) 와 링크를 해야 하는데, 라이브러리 탐색 패스에서 링크하려는 공유 라이브러리
가 있다면 공유 라이브러리를 사용해 링크하고, 없다면 정적 라이브러리와 링크한다.
［예제 4-22］ 는 페도라 7 배포판에서 like.c 파일을 -v -save-temps 옵션으로 컴파일
할 때 collect27} 수행되는 모습인데, 앞으로 이 예제로 설명하겠다.

4장_ gcc compiler

213

===== PAGE 215 =====
〔예제 4-22］

collect』의 수행 모습

/usr/libexec/gcc/i386-redhat-linux/4.1.2/collect2 --eh-framehdr -m elf_i386
----------------------------- -dynamic-linker /lib/ld-linux.so.2 -o like
/usr/lib/gcc/i386—redhat—linux/4.1•2/../•./../crtl.o
/usr/lib/gcc/i386—redhat—linux/4.1.2/../../../crti.o
/usr/lib/gcc/i386—redhat-丄inux/4.1.2/crtbegin.o
-L/usr/lib/gcc/i386-redhat-linux/4.1.2
—L/usr/lib/gcc/i386—redhat-linux/4.1.2
—L/usr/lib/gcc/i386—redhat-linux/4.1.2/
like.o
-Igcc --as-needed ---------------------------------------------------- ---Igcc --as-needed -lgcc_s ------------------------------------------/usr/lib/gcc/i386-redhat-linux/4.1.2/crtend.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/../crtn.o

［예제 4-22］ 의 옵션들은 Id에 대부분 그대로 전달되며, 각 옵션의 의미는 다음과 같다.
먼저 -m elfJ386에 의해 바이너리 포맷과 CPU 타입을 지정했다. 그리고 -dynamic­

linker /lib/ld-linux.so.2에 의해 동적 링커로 /lib/ld-linux.so.2를 지정했다. 원래 동
적 링커는 두 가지 종류가 있는데, a.out 바이너리 포맷의 공유 라이브러리를 링크하기
위한 /lib/ld-2.6.so（페도라 7 배포판 경우）와 ELF 포맷의 공유 라이브러리를 링크하기
위한 /lib/ld-linux.so.2가 바로 그것이다. like.o와 링크한 /lib/libc.so.6는 ELF 포맷의
공유 라이브러리이기 때문에 /lib/ld-linux.so.2를 동적 링커로 사용한다.

-o like 옵션에 의해 링크 과정이 끝나고 생성되는 실행 파일명은 like가 된다. 그리고
독자들은 like.o에 crtl.o와 ctri.o, crtbegin.o, crtend.o, crtn.o가 같이 링크되는 것이
의아할 것이다. like.o에서 필요한 심볼은 puts이고 puts는 표준 C 라이브러리를 링크
하면 있으므로 지금까지 배운 내용만으로는 위와 같은 파일들을 링크할 아무런 이유가
없기 때문이다.

like.o 외에 나머지 오브젝트들은 startup 코드라고 하며, 초기화 루틴과 종료 루틴들이
들어 있는 오브젝트들이다.
흔히 프로그램을 실행시키면 main 함수부터 실행되는 것으로 알고 있겠지만 실제로는
그렇지 않다. 실제로는 crtl.o에 있는 _start부터 시작한다. 먼저 커널의 execveO 시
스템 콜이 프로그램을 메모리에 적재한 후 main（ int argc, char **argv, char **envp）
함수에서 사용하는 인자 값들（실행 인자 개수, 인자, 환경 변수）을 프로세스의 스택에

push 한다.

214 3부_ 컴파일과링킹

===== PAGE 216 =====
그리고 동적 링커를 필요로 하지 않는다면 crtl.o에 있는 _start를 바로 수행하고, 동적
링커를 필요로 한다면 동적 링커를 수행한 후 _start^ 수행한다. _start는 커널이 저장
한 정보를 꺼내고 /lib/libc.so.6에 있는 __libc_start_main() 함수를 호출한다. _libc_

start_main() 함수는 프로그램 수행에 필요한 많은 초기화를 수행하고, 비로소 진짜
main() 함수를 호출한다. 이렇게 실제 프로그램의 main() 함수가 수행되기까지는 많은
과정을 거친다.
다음으로

-L/usr/lib/gcc/i386-redhat-linux/4.1.2,

linux/4.1.2,

-L/usr/lib/g<x/i386-redhat-linux/4.1.2/../../..

-L/usr/lib/gcc/i386-redhat옵션으로

라이브러리

파

일을 찾을 디 렉토리를 지정한다.

/usr/lib/gcc/i386-redhat-linux/4.1.2/../../..

디렉토리는

실제로

/usr/lib

디렉토리

를 의미한다. 그렇기 때문에 collect2에서 호출되는 Id는 라이브러리를 링크하기 위
해 라이브러리들을 -L 옵션으로 지정된 /usr/lib/gcc/i386-redhat-linux/4.1.2, /usr/

lib 디렉토리와, 기본적으로 라이브러리를 찾기 위해 Id가 탐색하는 /usr/i386-redhatlinux/lib, /usr/local/lib, /lib, /usr/lib 디 렉토리순으로 찾는다.
링크하는 라이브러리가 위에서 지정한 디렉토리에 있지 않고 다른 디렉토리에 있어
찾을 수 없다면 링크 오류가 발생한다. 그럴 때는 -L/root/lib 같이 -L 옵션으로 라이
브러리를 찾을 디렉토리를 추가해야 한다. 다음으로 링크할 like.o 오브젝트를 지정한
다. 그리고 -Igcc --as-needed ------- ----------------------------------- -Igcc --as-needed

-lgcc_s --no-as-needed 옵션으로 같이 링크할 라이브러리를 지정한다.
-1 옵션 뒤에 오는 것이 라이브러리명인데 앞에 붙는 lib를 떼어버리고 확장자 이전까
지가 라이브러리명이다. 즉, libc.*의 경우 c가 라이브러리명이고, libm.*의 경우 m이
라이브러리명이다. ［예제 4-22］ 의 -Igcc에서 라이브러리명이 gcc이기 때문에 실제 파
일명은 libgcc.*라는 것을 알 수 있고, -lgcc_s의 경우 실제 파일명은 libgcc_s.*라는 것
을 알 수 있다.
이 중에서 libgcc.*는, 공유 라이브러리는 없고 /usr/lib/gcc/i386-redhat-linux/4.1.2
디렉토리에 libgcc.a 형태로 있는 정적 라이브러리만 있다. libc.*는 /usr/lib/libc.a 형
태의 정적 라이브러리와 /lib/libc.so.6 형태로 있는 공유 라이브러리가 같이 존재한다.
정적 라이브러리와 공유 라이브러리가 같이 존재할 경우 공유 라이브러리를 우선시하
므로 collect』에서 호출되는 Id는 libgcc.a와 libgcc_s.so, /lib/tls/libc.so.6를 링크해
최종적으로 실행 파일 Bke를 만들어낸다.

4장_ gcc compiler 215

===== PAGE 217 =====
libgcc.a, libgcc_s.so 같은 라이브러리는 gcc에서 사용하는 아키텍처와 관련된 함수들
을 담고 있는 라이브러리다. 이런 아키텍처와 관련된 대표적인 함수로는 ARM 아키텍
처의 __udivsi3() 함수 같은 것들이 있다. ARM 아키텍처에는 나누기 인스트럭션이 없
기 때문에 arm-linux-gcc 컴파일러는 unsigned int 타입으로 이뤄진 c = a / b ； 같은

C 소스를 c = __udivsi3(a, b)； 같은 나누기 함수 호출로 바꾼 후 컴파일 과정을 수행한
다. 나누기 연산뿐만 아니라 부동소수점 더하기 연산 같은 것도 ARM 아키텍처에서 지
원하지 않기 때문에 내부적으로 __floatadd() 같은 함수 호출로 바꾼 후 컴파일 과정을
수행한다.
결국 인스트럭션으로 지원하지 않는 연산자들은 함수 호출로 변경되어 소프트웨어적
으로 처리된다. 이때 이런 __ udivsi3(), __floatadd() 같은 아키텍처와 관계된 함수들
이 들어 있는 라이브러 리가 바로 libgcc.a와 libgcc_s.so 라이브러 리 다.
그러면 최종적으로 생성되는 like 바이너리 파일은 정말 이렇게 만들어졌을까? 최종적
으로 생성되는 like 바이너리 구조는 -Wl,-M 옵션을 추가해 컴파일하면 확인할 수 있다.
$ gcc -0 like like.c -save-temps -Wl,-M >& like.Ids

위와 같은 명령을 내리고 likejds 파일을 열어보면 다음과 같이 like 바이너리의 실제
구조를 확인할 수 있다.
〔예제 4-23]

like.Ids 파일의 내용

... 상략

.text 0x080482d0

0x24

0x080482d0
.text 0x080482f4
0x0804831a

/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crtl.o
__start

0x26

/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crti.o

0x6 90909090

.text 0x08048320

0x83 /usr/lib/gcc/i386-redhat-linux/4.1.2/crtbegin.o

0x080483a3
.text 0x080483a4

0x2b like.o

0x1 90909090

0x080483a4

main

0x080483cf

0x1 90909090

.text 0x080483d0

0x79 /usr/lib/libq_ponshared.a(elf-init.oS)

• • • 중략

.rodata 0x080484a0

Oxc like.o

• • • 중략

.data 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crti.o

.data 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/crtbegin.o

.data 0x0804961c

0x0 like.o

.data 0x0804961c

0x0 /usr/lib/libc_nonshared.a (elf-init.oS)

216 =_ 컴파일과링킹

===== PAGE 218 =====
.data 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/crtend. o

.data 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/./crtn.o

• • • 중략

.bss 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crtl.o

.bss 0x0804961c

0x0 /usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crti.o

.bss 0x0804961c

0x5 /usr/lib/gcc/i386-redhat-linux/4.1.2/crtbegin.o
0x3 00

0x08049621
.bss 0x08049624

0x0 like.o

.bss 0x08049624

0x0 /usr/lib/libcjnonshared. a (elf-init. oS)

.bss 0x08049624

0x0 /usr/lib/gcc/i386—redhat—linux/4.1.2/crtend.o

.bss 0x08049624

0x0 /usr/lib/gcc/i386—redhat—linux/4.1.2/../../../crtn.o

• ••하략

보면 알겠지만 이전에 설명한 대로 각각의 ELF 오브젝트에 text, data, bss 섹션 등이

collect2 명령을 내릴 때 지정한 순서대로 배치되어 있음을 확인할 수 있다. 그리고 호
기심 많은 독자라면 -static 옵션으로 표준 C 라이브러리를 정적 링킹했을 때 생성되는

like 바이너리의 모양은 어떤지 -Wl,-M 옵션으로 확인해 보는 것도 재미있을 것이다.
이것으로 컴파일 과정이 완전히 끝났다. 이제 만들어진 like 실행 파일을 셸에서 ./like
명령으로 내려주면 실행된다. 프로그램이 실행되는 과정에서도 독자에게 도움이 될 만
한 것들이 많은데, 내용이 방대하므로 따로 설명하지 않는다. 실행 과정이 궁금한 독
자가 있다면『리눅스 커널의 이해, 개정판 (Understanding the Linux Kernel, 3nd

Edition)』(한빛미디어, 2006)을 보기 바란다.
축하한다. 이제 독자들은 믿겨지지 않겠지만 gcc 컴파일 과정에 있어서는 전문가가 되
었다. 지금까지 필자가 설명한 gcc 컴파일 과정은 앞으로 배울 것들에 대한 이해의 폭
을 한 차원 높일 수 있고, 유닉스/리눅스 프로그래밍을 하는 데 있어 두고두고 도움이
되는 지식이다. 반드시 알아야 되는 지식 중 하나인데, 유닉스/리눅스 분야에 오랫동안
종사했던 사람이라 할지라도 관심을 가지고 탐구하지 않았다면 이런 gcc 컴파일 과정
에 대해 잘 알지 못한다. 그러니 자부심을 가지기 바란다. 필자가 장담하건대 누가 뭐래
도 독자는 gcc 컴파일 과정 분야에 있어서 전문가가 되었다.

4장_ gcc compiler 217

===== PAGE 219 =====
3L gcc를 사용해 원하는 컴파일하기

I

이제 우리는 이번 장을 통틀어 가장 쓸 만한 걸 배워보자. “지금 할 것이 가장 쓸 만한
것이라면 이전에 배운 컴파일 과정은 뭐였나?”라고 반문하는 독자가 있을 것이다. 이전
컴파일 과정은 이번 장을 통틀어 가장 의미 있는 장이었다.
“컴파일 과정” 절은 이번 절을 이해하기 위한 선행 지식임과 동시에 리눅스 환경에서

c 프로그래밍을 하기 위해 필수적으로 알아야 되는 지식이다. 이전 컴파일 과정을 이
해하지 않았다면 지금 배울 내용들을 이해하기 힘들 것이다. 결국 독자가 원하는 것은

gcc 컴파일러로 잘 컴파일하는 것이라고 본다. 그러려면 gcc의 수많은 옵션을 알아야
한다.

gcc 는 정말 끔찍할 정도로 많은 옵션이 있다. man gcc 명령으로 gcc의 수많은 옵션을
쳐다보는 것만으로도 정신적 충격을 받을 수 있을 정도다. 그런 옵션들을 다 설명하는
것은 필자도 무리고 독자도 힘들 것이다.
필자는 이 책이 gcc 를 설명한 책이 되기를 바랄 뿐이지 gcc 매뉴얼이 되길 바라지는
않는다. 원리와 의미도 건너뛰고 수많은 gcc 옵션을 주루룩 나열하면서 설명하면 필자
도 따분할 뿐만 아니라 정말 중요한 것들을 놓칠 수 있다.
정말 중요한 것은 독자가 gcc의 수많은 옵션들을 하나씩 다 아는 것이 아니라 gcc 옵션들
의 구성과 구조를 파악하고 필요한 옵션을 어떻게 하면 적재적소에 사용할 수 있는가를 익
히는 것이라 하겠다. 결국 모든 것은 원리와 규칙이다. 매뉴얼보다 자세하진 않겠지만 필자
는 독자에게 gcc를 전문가 수준으로 사용할 수 있는 구조와 원리를 알려줄 것이다.

I gcc 옵션 분류
gcc의 옵션은 크게 C 컴파일러 드라이버 옵션, 전처리기 옵션, 컴파일러 옵션, 어셈블러
옵션, 링커 옵션으로 나눠진다. 다음과 같은 gcc 명령이 있을 때 이런 명령은 gcc C 컴
파일러 드라이버에 의해 해석되고, 각 옵션이 종류별로 분류되고 해당 과정（전처리, 컴
파일, 어셈블, 링킹）을 수행하는 바이너리를 실행할 때 기본 옵션에 추가되어 수행된다.
gcc
-v
-I/usr/local/include
-o like like.c -lm

218 3부—컴파일과링킹

-DDEBUG

-Wall

-W

-02

-L/usr/local/lib

===== PAGE 220 =====
그래서 위와 같은 명령은 각각 다음과 같이 해석되어 각 과정을 수행하는 바이너리를
호출할 때 사용된다.

gcc C 컴파일러 드라이버 자체의 옵션으로, gcc가 컴파일 과정을 어떻게 수행
하는지 화면에 출력한다. -I/usr/local/include -DDEBUG는 전처리기（ ccl -E） 의 옵
션으로, gcc가 전처리기를 수행할 때 기본 옵션에 추가해 수행한다. -Wall -W -02
는 ccl의 옵션으로, gcc가 ccl을 수행할 때 기본 옵션에 추가해 수행한다. -L/usr/

local/lib -o like -im은 collect2의 옵션.0.루, 마찬가지로 gcc가 기본 옵션에 추가해
collect》를 수행한다. 이후 collect』는 내부적으로 링커인 Id를 호출할 때 이렇게 전달
된 옵션을 Id로 넘겨 링킹 과정을 수행한다.
이 중 가장 많은 옵션을 가지고 있는 것은 ccl으로, C 언어 옵션, 경고 옵션, 디버깅 옵
션, 최적화 옵션 등으로 나눠진다. gcc에서는 각 과정 옵션 외에 ccl의 기능을 좀 더 세
분화해 기능별로 분류한다.

man gcc 명령을 내려 보면 gcc 에서 기능별로 분류해놓은 옵션 리스트를 볼 수 있다.
“Option Summary" 부분을 보면 어떻게 분류되어 있는지 확인할 수 있고, 옵션 종류별
특징을 정리하면 다음과 같다（설명할 때 기준은 C 컴파일러를 기준으로 한다）.

►

Overall Options （ gcc 컴파일러 드라이버 옵션）

gcc 컴파일러 드라이버의 옵션으로 주로 “컴파일 과정을 어디까지 진행할 것인지?”,
“컴파일 진행 과정을 출력할 것인지?” 등을 조절할 때 사용한다. 또한 버전 출력, 도움
말 출력 등에 대해 지정할 때도 사용한다. 대표적으로 우리가 지금껏 컴파일 과정을 보
기 위해 사용한 -v 옵션이 overall options에 해당한다.

Overall 옵션에는 다음과 같은 것들이 있다. 그리고 지금부터는 옵션이 무척 많으므로
개개의 옵션은 보지 말고 한글만 읽기 바란다.
-c
-S
-E
-o
file
-combine
-### ------------- ----- target-help --version

►

-pipe

-pass-exit-codes

-x

language

-v

C Language Options （ ccl 의 front-end 옵션）

C 언어 종류나 표준과 관련된 옵션으로, 특정 C 언어 종류를 지정하거나 ANSI 표준
을 지원할 것인지, 빌트인 함수 （ builtin function） 사용 여부, 특정 타입의 signed/
니nsigned 지정 여부, 표준 C 라이브러리 사용 여부 등을 정할 때 사용한다.

4 장_gcc compiler 219

===== PAGE 221 =====
각 C 언어 종류와 표준에 부합하는 C 소스를 작성하고자 할 때 주로 사용하고, 대표적
인 옵션으로는 ANSI 표준 C 문법에 대한 적합성을 검사할 때 사용하는 -ansi 옵션 등
이 있다. C 옵션에는 다음과 같은 것들이 있다.
-ansi
-std=standard
asm
-fno-builtin
-fms-extensions
-traditional-cpp
-fsigned-bitfields
char

►

-fgnu8
9-inline
-aux-info
filename
-f
no-fno-builtin-function
-fhosted
-ffreestanding
-trigraphs
-no-integrated-cpp
-traditional
-fallow-single-precision
-fcond-mismatch
-fsigned-char
-funsigned-bitfields
-funsigned-

C-H- Language Options （ cdplus의 front-end 옵션）

C Lang니age Options와 의미는 거의 동일하고, C++ 언어에 특화된 속성들을 정할 때
사용하는 옵션들이다.
—fabi-version=n
-fno-access-control
-fcheck-new
-fconserve-space
-ffriend-inj
ection
-fno-const-strings
-fno-elide-constructors
-fno-enforce-eh-specs
-ffor-scope
-fno-for-scope
-fno-gnu-keywords
-fno-implicit-templates
-fno-implicit-inline-templates
-fno­
implementinlines
-fms-extensions
-fno-nonansi-builtins
-fno­
operator-names
-fno-optional-diags
-fpermissive
-frepo
-fnortti
-fstats
-ftemplate-depth-n
-fno-threadsafe-statics
-fuse-cxaatexit
-fno-weak
-nostdinc++
-fno-default-inline
-fvisibilityinlines-hidden
-Wabi
-Wetor-dtor-privacy
-Wnon-virtual-dtor
-Wreorder
-Weffc++
-Wno-deprecated
-Wstrict-null-sentinel
-Wnonon-template-friend
-Wold-style-cast
-Woverloaded-virtual
-Wnopmf-conversions -Wsign-promo

►

Objective-C and Objective—C++ Language Options （ cdobj front-end 옵션）

Objective-C 컴파일러인 cclobj의 옵션으로, 의미는 C Language Options와 거의
동일하다.
-fconstant-string-class=class-name
-fgnu-runtime
-fnext-runtime
-fno-nil-receivers
-fobjc-call-cxx-cdtors
-fobjc-direct-dispatch
-fobjc-exceptions
-fobjc-gc
-freplace-objc-classes
-fzero-link
-gen-decls
-Wassign-intercept
-Wno-protocol
-Wselector
-Wstrictselector-match -Wundeclared-selector

►

Language Independent Options （ cd 옵션）

오류 메시지의 출력 포맷 조절 등에 사용되는 옵션들로 거의 사용할 일이 없다.
-fmessage-length=n -fdiagnostics-show-location=[once|every-line]
-fdiagnostics-show-options

220 =_ 컴파일과 링킹

===== PAGE 222 =====
►

Warning Options （ cc1 의 front-end 옵션）

각종 경고 메시지를 출력할지 말지를 결정할 때 사용한다. 주로 모든 경고 메시지를 출
력하는 -Wall -W 옵션을 사용해 컴파일하고, 불필요한 경고가 발생할 때 Warning

options에 있는 해당 경고를 끄는 옵션을 이용해 불필요한 경고 메시지만 제거하는 형
식으로 사용한다.
-fsyntax-only
-pedantic
-pedantic-errors
-w
-Wextra
-Wall
-Waggregate-return
-Wno-attributes
-Wc++-compat
-Wcast-align
-Wcast-qual
-Wchar-subscripts
-Wcomment
-Wconversion
-Wnodeprecated-declarations
-Wdisabled-optimization
-Wno-div-by-zero
-Wno-endif-labels
-Werror
-Werror-implicit-function-declaration
-Wfatal-errors
-Wfloat-equal
-Wformat
-Wformat=2
-Wno-formatextra-args
-Wformat-nonliteral
-Wformat-security
-Wformat-y2k
-Wimplicit
-Wimplicit-function-declaration
—Wimp丄icit-int
-Wimport
-Wno-import
-Winit-self
-Winline
-Wno-int-to-pointer-cast
-Wnoinvalid-offsetof
-Winvalid-pch
-Wlarger-than-len
-Wunsafe-loop­
optimizations
-Wlong-long
-Wmain
-Wmissing-braces
-Wmissingfield-initializers
-Wmissing-format-attribute
-Wmissing-includedir
s
-Wmissing-noreturn
-Wno-multichar
-Wnonnull
-Wpacked
-Wpadded
-Wparentheses
-Wpointer-arith
—Wno—pointer-to-int-cast
-Wredundant-decls
-Wreturn-type
-Wsequence-point
-Wshadow
-Wsigncompare
-Wstack-protector
-Wstrict-aliasing
-Wstrict-aliasing=2
-Wswitch
-Wswitch-default
-Wswitch-enum
-Wsystem-headers
-Wtrigraphs
-Wundef
-Wuninitialized
-Wunknown-pragmas
-Wnopragmas
-Wunreachable-code
-Wunused
-Wunused-function
-Wunused丄
abel
-Wunused-parameter
-Wunused-value
-Wunused-variable
-Wvariadic-macros -Wvolatile-register-var -Wwrite-strings

►

C-only Warning Options （ cc1 의 front-end 옵션）

C 언어에서만 해당하는 몇 가지 경고 메시지를 끄거나 켤 때 사용한다.
-Wbad—function-cast
-Wmissing-declarations
-Wnested-externs
-WoId-style-definition
-Wtraditional -Wdeclaration—after-statement -Wpointer-sign

►

-Wmissing-prototypes
-Wstrict-prototypes

Debugging Options （ cd 옵션）

cel과 같은 컴파일러 자체 디버깅을 위해 사용하는 옵션이다. 우리가 지금껏 gcc 컴파
일 과정을 알아보기 위해 사용한 —fd니mp-tree-all, -save-temps, —da 옵션이 모두

debugging 옵션에 해당한다.
-dletters
-dumpspecs
-dumpmachine
-dumpversion
-fdump-unnumbered
-fdump-translation-unit[-n]
-fdump-class-hierarchy[-n]
-fdump-ipaall
-fdump—ipa-cgraph
-fdump-tree-all
-fchimp—tree-original[-n]
—fdump—tree-optimized[-n]
-fdump-tree-inlined[-n]
-fdump-tree-

4장_ gcc compiler 221

===== PAGE 223 =====
cfg
-fdump-tree-vcg
-fdump-tree-alias
-fdump-tree-ch
-fdump-treessa[-n]
-fdump—tree—pre[—n]
-fdump-tree—ccp[-n]
-fdump-treedee
[-n]
-fdump-tree-gimple[-raw]
—fdump-tree—mudf丄ap[-n]
-fdumptree-dom[-n]
-fdump-tree-dse[-n]
-fdump-tree-phiopt[-n]
-fdumptree-forwprop[-n]
-fdump-tree—copyrename[-n]
-fdump-tree-nrv
-fdump-tree-vect
-fdump-tree-sink
-fdump-tree—sra[—n]
-fdumptree-salias
-fdump-tree-fre[-n]
-fdump-tree-vrp[-n]
-ftree­
vector
izer-verbose=n
-fdump-tree—storecep[-n]
-feliminate—dwarf2dups
-fmem-report
-feliminate-unused-debug-types
-feliminateunused—debug-symbols
-fprofile-arcs
-frandom-seed=string
-fschedverbose=n
-ftest-coverage
-ftime-report
-fvar-tracking
-g
-gleve丄
-gcoff
-gdwarf-2
-ggdb
-gstabs
-gstabs+
-gvms
-gxcoff
-gxcoff+
-p
-pg
—print-file-name=library
-print-1
ibgcc-file-name
-print-multidirectory
-print-multi-lib
-print-prog—name=program
-print-searchdirs -Q -save-temps -time

►

Optimization Options (cd middle-end / back-end 옵션)

ccl 의 옵션으로, 각종 최적화와 관련된 옵션이다. 가장 대표적인 것이 이전에 사용한
-O [최적화 레벨] 옵션이다. 보통은 -O [최적화 레벨] 옵션을 사용해 최적화 옵션들의
묶음을 결정하고, -f [각종 최적화 옵션] 옵션을 사용해 특정 최적화를 추가/제거하는
형식으로 많이 사용한다.
-falign-functions=n
-falign-jumps=n
-falign-labels=n
-falignloops=n
-fbounds-check
-fmudflap
-fmudflapth
-fmudflapir
-fbranchprobabilities
-fprofile-values
-fvpt
-fbranch-target-load-optimize
-fbranch-target-load-optimi
ze2
-fbtr-bb-exclusive
-fcaller­
saves
-fcprop-registers
-fese-follow-jumps
-fese-skip-blocks
-fex-limited-range
-fdata-sections
-fdelayed-branch
-fdelete­
null
-point
erchecks
-fearly-inlining
-fexpensive-optimizations
-ffast-math
-f
float-store
-fforce-addr
-ffunction-sections
-fgese
-fgcse-lm
-fgese-sm
-fgcse-las
-fgcse-after-reload
-floopoptimize
-fcrossjumping
-fif-conversion
-fif-conversion2
-finline­
functions
-finline-functions-called-once
-finline-limit=n
-fkeep­
inline-functions
-fkeep-static-consts
-fmerge-constants
-fmergeall-constants
-fmodulo-sched
-fno-branch-count-reg
-fno-defaultinline
-fno-defer-pop
-floop-optimize2
-fmove-loop-invariants
-fnofunction-cse
-fno-guess-branch-probability
-fno-inline
-fno-matherrno
-fno-peephole
-fno-peephole2
-funsafe-math-optimizations
-funsafe-loop-optimizations
-ffinite-math-only
-fno-trapping-math
-fno-zero-initialized-in-bss
-fomit-frame-pointer
-foptimizeregister-move
-foptimi
ze-sibling-calls
-fprefetch-loop-arrays
-fprofile-generate
-fprofile-use
-fregmove
-frename-registers
-freorder-blocks
-freorder-blocks-and-partition
-freorderfunctions
-frerun-cse-after-loop
-frerun-loop-opt
-frounding­
math
-fschedule-insns
-fschedule-insns2
-fno-sched-interblock
-fno-sched-spec
-fsched-spec-load
-fsched-spec-load-dangerous
-fsched-stalled-insns=n
—fsched-stalled—insns—dep=n
-fsched2-use-

222 3부—컴파일과링킹

===== PAGE 224 =====
superblocks
-fsched2-use-traces
-freschedu丄e—modu丄o-scheduledloops
-fsignaling-nans
-fsingle-precision-constant
-fstack­
protector
-fstack-protector-all
-fstrength-reduce
-fstrictaliasing
-ftracer
-fthread-jumps
-funroll-all-loops
-funroll­
loops
-fpeel-loops
-fsplit-ivs-in-unroller
-funswitch-loops
-fvariable-expansion-in-unroller
-ftree-pre
-ftree-ccp
-ftreedee
-ftree-loop-optimize
-ftree-loop-1inear
-ftree-loop-im
-ftreeloop-ivcanon
-fivopts
-ftree-dominator-opts
-ftree-dse
-ftree­
copyrename
-ftree-sink
-ftree-ch
-ftree-sra
-ftree-ter
-ftree-lrs
-ftree-fre
-ftree-vectorize
-ftree-vect—loop-version
-ftree-salias
-fweb
-ftree-copy-prop
-ftree-store-ccp
-ftree-store-copy-prop
------------------------------------------ --- -0 -00 -01 -02
-03 -0s

►

Preprocessor Options （ cd -E 또는 cppO 옵션）

전처리기 옵션으로, 매크로 정의 및 비정의 등 여러 전처리기 옵션이 여기에 해당한다.
-Aquestion=answer
—A-question[=answer]
-Dmacro[=defn]
-E
-H
-idirafter
file
-iprefix
file
-iwithprefix
dir
dir
-isysroot
dir
-M
-MM
-MF
-MG
-fworking-directory
-remap
-trigraphs
-Xpreprocessor option

►

-C
-dD
-di
-dM
-dN
dir
-include
file
-imacros
-iwithprefixbefore
dir
-isystem
—MP
—MQ
-MT
-nostdinc
-P
-undef
-Umacro
-Wp,option

Assembler Option （ as 옵션）

as의 옵션이다. as는 아키텍처마다 각기 다른 어셈블러가 사용되기 때문에 gcc에서 지
원하는 옵션은 거의 없고 해당 어셈블러에게 옵션을 바로 넘겨주기 위한 옵션들이 주
로 있다.
-Wa,option -Xassembler option

►

Linker Options （ collect2 또는 Id 옵션）

각종 링커 관련 옵션으로, OS, 부트로더 등과 같은 시스템 프로그래밍을 할 때 자주 사
용되는 옵션들이 들어 있다.
object-file-name
-llibrary
-nostartfiles
-pie
-rdynamic
-s
-static
-static-libgcc
-symbolic -Wl,option -Xlinker option -u symbol

►

-nodefaultlibs
-shared

-nostdlib
-shared-libgcc

Directory Options （ cd -E, collect2 등 옵션）

헤더 파일을 찾을 위치 지정（ -Hpath]） , 라이브러리를 찾을 위치 지정（ -L[path]） 등 각
종 디렉토리 지정에 사용되는 옵션들이다.
-Bprefix -Idir -iquotedir -Ldir —specs=fi丄e -I- --sysroot=dir

4장_ gcc compiler 223

===== PAGE 225 =====
► Target Options （ cd 옵션）
컴파일하려는 타겟 아키텍처를 지정하거나 여러 버전의 컴파일러가 설치되었을 때 특
정 컴파일러를 지정하기 위해 사용하는 옵션이다. 타겟 아키텍처의 지정은 GCC를 컴
파일할 당시에 지정한 아키텍처여야만 한다. 그다지 쓸 일이 없다.
-V version -b machine

►

Machine Dependent Options （ cd, as, collect2 옵션）

각종 아키텍처에 종속적인 옵션들이다. 아키텍처마다 독특한 구조를 가지고 있고, 같은
아키텍처라 할지라도 프로세서의 종류（예: 386과 펜티엄 등）에 따라 지원하는 인스트
럭션 셋과 특징이 다르다. 머신 종속적인 옵션은 이런 각 프로세서의 구조와 특징을 컴
파일러에 반영할 때 사용하는 옵션들이다.
예를 들면 머신 종속적인 옵션 종류 중 i386 and x86-64 Options 종류에 -march 옵
션이 있는데, g 으로 컴파일 시 -march=athlon-xp 옵션을 주면 AMD 애슬론 까에 최
적화된 코드를 생성할 수 있고, -march=core2 옵션을 주면 인텔 코어2에 최적화된 코
드를 생성할 수 있다. 이렇게 생성된 코드들은 각 프로세서에서 지원하는 인스트럭션
셋으로 구성되기 때문에 오래된 구형 i386 머신에서는 동작하지 않을 수 있다.
이런 머신 종속적인 옵션들은 아키텍처 종류에 따라 서로 다른 옵션을 가지고 있다. 그
래서 x86을 타겟.0-로 하는 머신 종속 옵션들은 ARM 타겟으로 하는 arm-linux-gcc 컴
파일러 에서는 지원하지 않는다.
머신 종속적인 옵션들은 이런 특성을 갖는 옵션들의 집합이고, 모두 -m으로 시작한다.
ARC Options ...
ARM Options . . .
AVR Options . . .
Blackfin Options . . .
CRIS Options ...
CRX Options . . .
Darwin Options ...
DEC Alpha Options . . .
DEC Alpha/VMS Options ...
FRV Options ...
H8/300 Options ...
ELPPA Options . . .
i386 and x86-64 Options .. .
IA—64 Options . . .
M32R/D Options ...
M32C Options ...

224 3부— 컴파일과 링킹

===== PAGE 226 =====
M680x0 Options ...
M68hclx Options ...
MCore Options ...
MIPS Options ...
MMIX Options ...
MN10300 Options ...
MT Options ...
PowerPC Options ...
RS/6000 and PowerPC Options ...
S/390 and zSeries Options ...
SH Options ...
SPARC Options ...
System V Options ...
TMS320C3x/C4x Options ...
V850 Options ...
VAX Options ...
x86-64 Options ...
Xstormyl6 Options ...
Xtensa Options ...
zSeries Options ...
※너무 많아 아키텍처 종류만 표시하였다.

►

Code Generation Options （ cd 옵션）

인스트럭션을 생성할 규칙을 재정의할 때 사용하는 옵션들이다. 특정 레지스터를

caller saved 레지스터로 사용할지, callee saved 레지스터로 사용할지 등을 지정하
거나 스택을 체크하는 인스트럭션을 삽입하는 둥과 같은 각종 인스트럭션 생성 규
칙을 지정할 때 사용하는 옵션들이다. 대표적으로 위치 비종속 코드（ PIC： Position-

Independent CodeX 생성할 때 사용하는 -fPIC 옵션 등이 있다.
-fcall-saved-reg
-fcall-used-reg
-ffixed-reg
-fexceptions
-fnonca11-exceptions
-funwind-tables
-fasynchronous-unwind-tables
-finhibit-size-directive
-finstrument-functions
-fno-common
-fnoident
-fpcc-struct-return
-fpic
-fPIC
-fpie
-fPIE
-fno-jump­
tables
-freg-struct-return
-fshared-data
-fshort-enums
-fshort­
double
-fshort-wchar
-fverbose-asm
-fpack-struct[=n]
-fstack-check
-fstack-limit-register=reg
-fstack-limit“symbol=sym
-fargumentalias
-fargument-noalias
-fargument-noalias-global
-fleading­
underscore
-ftls-model=model
-ftrapv
-fwrapv
-fbounds-check
-fvisibility -fopenmp

정말 많다. 많긴 하지만 어떤 옵션 종류로 나눠지는지 조금은 알았을 것이다. gcc 옵션
적용에는 일정한 규칙을 가지고 있는데, 지금부터는 그런 규칙에는 무엇이 있는지 알아
본다.

4장_ gcc compiler 225

===== PAGE 227 =====
I gcc 옵션 적용 규칙
gcc의 옵션 적용 규칙은 매우 단순하다. 이런 규칙을 알고 나면 원하는 대로 gcc 옵션
을 사용해 컴파일할 수 있다.

O 첫 번째: 각각의 옵션에는 대부분 그에 상응하는 gcc 내부 변수가 있다.
gcc를 컴파일하면 gcc/options.c 파일과 gcc/options.h 파일이 생성되고, 그 내부에
는 gcc 옵션에 대응하는 다음와 같은 변수들이 정의된 것을 볼 수 있다.
〔예제 4-24)

gcc/options.h 파일 내용

. • • 상략

extern int
extern int
extern int
extern int
extern int
extern int
extern int

warn_unsafe_loop_optimizations;
warn_unused_function;
warn_unused_label;
warn_unused_parameter;
warn__unused_value;
warn_unused_variable;
warn_register_var;

• • • 중략

extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int
extern int

flag_bounds_check;
flag_br anch_on_count_reg;
flag_branch_probabilities;
flag_branch_target_load_optimize;
flag_branch_target_load_optimize2;
flag_btr_bb_exclusive;
flag_caller_saves;
flag_check_ref erences;
flag_no_common;
flag_cprop_registers;
flag_cross jumping;
flag_cse_follow_j umps;
flag_cse_skip_blocks;
flag_cx_limited_range;
flag_data_sections;

• •• 하략

예를 들어 int warnjjnused_variable 변수는 gcc로 컴파일 시 -W니nused_variable
옵션을 주면 값이 설정되는 변수이고, 아무런 옵션도 주지 않으면 기본 값이 0으로 설
정되는 변수다. -Wunused_yariable 옵션은 소스 파일 내에 정의는 되 었지만 사용되지
않는 변수가 있을 때 컴파일 과정에서 경고를 출력하게 하는 옵션이다. gcc는 자체 소
스 코드 내 warn_unused_yariable 변수의 값을 사용해 사용되지 않은 변수에 대해 경

226 3부— 컴파일과 링킹

===== PAGE 228 =====
고를 출력할지 말지 결정하게 구현되어 있고, -Wunused_yariable 옵션을 사용해 이 런

warn_unused_variable 변수의 값을 설정할 수 있다.
-Wunused_variable 옵션뿐만 아니라 각각의 옵션은 대부분 그에 대응하는 변수를 가
지고 있고, gcc 컴파일러는 내부적으로 해당 변수의 값으로 특정 기능을 수행할지 말지
를 결정하게 구현되어 있다.
@ 두 번째: -[f|W|m][옵션]은 설정이고 -[f|W|m]no-[옵션]은 해제다.

예를 들면 int flag_cse.followjumps 변수는 -fcse—skip-blocks 옵션으로 값을 설정
하고, 0으로 초기화할 때는 -fno-cse-skip-blocks 옵션을 사용한다.
마찬가지로 int warn_unused_function 변수는 -Wun니sed-function 옵션으로 값을
설정하고, 해제할 때는 -Wno-unused-function 옵션을 사용한다. 이렇게 f, W, m으
로 시작하는 많은 옵션은 해당 옵션 사이에 no-를 붙이면 해당 기능을 해제하는 의미
로 사용된다.

@ 세 번째: 동일 종류의 옵션은 최종 옵션만 옵션 변수에 값이 설정된다.

int warn_unused_f니nction 변수는 소스 파일 내에 사용되지 않은 함수가 있을 때 경
고를 출력하는 기능을 수행한다. int warn_unused_f니nction 변수는 -Wunused-

function 옵션으^ 값을 설정하고, -Wno-unused-function 옵션으^. 값을 해제한다.
다음과 같이 명령을 내리면 최종 옵션의 값만 warn_un니sedjimction 변수에 설정된다.
$ gcc -o like like.c -Wunused-function -Wno-unused-function
-Wunused-function -Wno-unused-function

-Wunused-function,

-Wno-unused-function

옵션이

아•무리

많이

붙어도

항상

최종 옵션만 유효하다. 때문에 int warn_unused_f니nction 변수에는 마지막에 오는

-Wno-unused-function 옵션에 의해 0이 설정된다.

Q 네 번째: 그룹 옵션이 존재한다.
-fdump-tree-all 옵션은 아래 옵션들을 동시에 준 것과 동일하다.
-fdump-tree-original[-n]
-fdump-tree-optimized[-n]
-fdumptree-inlined[—n]
-fdump-tree-cfg
-fdump-tree-veg
-fdump-treealias
-fdump-tree-ch
-fdump-tree-ssa[-n]
-fdump-tree-pre[-n]
-fdump-tree-ccp[-n]
-fdump-tree-dee[-n]
-fdump-tree-gimple[—raw]

4장_ gcc compiler 227

===== PAGE 229 =====
-fdump-tree-mudflap[-n]
—fdump-tree-dom[-n]
-fdump-tree—dse[-n]
-fdump-tree-phiopt[-n]
-fdump-tree-forwprop[-n]
-fdump-treecopyrename[-n]
-fdump-tree-nrv
-fdump-tree-vect
-fdump-tree-sink
-fdump—tree-sra[-n]
-fdump-tree-salias
-fdump-tree-fre[-n]
-fdumptree-vrp[-n] -ftree-vectorizer-verbose=n -fdump-tree-storeccp[-n]

마찬가지로 -O1 옵션을 주면 다음 옵션들을 동시에 준 것과 동일하다.
-fdefer-pop
-fdelayed-branch
-fguess-branch-probability
registers
-floop-optimize
-fif-conversion
-fif-conversion2
-ftree-dce
-ftree-dominator-opts
-ftree-dse
-ftree-ter
-ftree-sra
-ftree-copyrename
-ftree-fre
-ftree-ch
-fmerge-constants

-fcprop-ftree-ccp
-ftree-lrs
-funit-at-a-time

이렇게 gcc에서는 한꺼번에 여러 옵션을 지정한 것과 같은 효과를 낼 수 있는 그룹 옵
션들이 있다. 대표적인 그룹 옵션으로 최적화 관련 옵션인 -O 옵션과 모든 경고를 출
력하는 -Wall 옵션 등이 있다.
몇몇 옵션을 제외한 대부분의 그룹 옵션들은 그룹 내 포함된 서브 옵션을 지정할 때
순서에 영향을 받는다. 예를 들면 -O1 옵션을 주면 위에 적어놓은 -fdefer-pop,

-fdelayed-branch, -fguess-branch-probability, ••• 등의 옵션 변수 값이 모두 1로
설정된다. gcc -o like like.c -O1 -fno-defer-pop 명령을 내리면 -O1 옵션에 포함
되는 모든 옵션 변수의 값은 1로 설정되고 int flag_defer_pop 변수의 값만 0으로 설정
된다.
그리고 gcc -o like like.c -fno-defer-pop -O1 명령을 주면 마지막 -이의 영향을
받기 때문에 모든 그룹 옵션 변수의 값이 1로 설정된다.
同 다섯 번째: -f는 플래그이고, -W는 경고, -m은 아키텍처 종속, 기타 나머지들이다.

옵션들을 가만히 보면 -f로 시작하는 것과 -W로 시작하는 것, -m으로 시작하는 것, 나
머지 기타 옵션들이 있다. -f로 시작하는 것은 컴파일러의 특정 기능을 켜거나 끌 때 사
용하는 것으로, 주로 최적화, 문법 체크, 컴파일러 자체 디버깅과 관계가 있다.

-W로 시작하는 것은 주로 경고와 관련이 있고, -m으로 시작하는 것은 아키텍처 종속
적인 옵션들이다.

228 3부- 컴파일과 링킹

===== PAGE 230 =====
@ 마지막: 하나의 옵션이 반드시 하나의 변수만 바꾸는 것은 아니다.

대부분 하나의 옵션은 하나의 기능만을 의미하기 때문에 하나의 변수 값만 바꾼다. 하
지만 어떤 옵션들은 어떤 기능을 켜고 끌 때 그 기능에 종속적인 다른 변수의 값을 켜
고 끄기도 한다. 그룹 옵션이 대표적인 경우다.
이것으로 끝이다. gcc 옵션 규칙은 이것밖에 없다. 그러면 이제 본격적으로 어떤 옵션
들이 있는지 알아보자.

I 가장 단순한 컴파일 명령
성급한 독자를 위해 먼저 가장 단순한 컴파일 명령을 설명한다. 가장 단순한 컴파일 명
령은 다음과 같다.
$ gcc like.c

위와 같이 명령을 내리면 like.c가 a.out이라는 이름으로 컴파일된다. a.out이란 이름은
전통적으로 유닉스 시스템 이 a.out 바이너 리 포맷을 사용한 데서 유래한다.

[그림 4-34] gcc like.c로 컴파일한 모습

정말 단순하다. 출력 파일의 이름조차 지정하지 않은 컴파일 방법이다. 위와 같은 컴파일
방법은 간단한 소스 테스트에서 자주 사용하고, 보통은 다음과 같은 형식으로 사용한다.
gcc -W -Wall -02 -o like like.c

-Wall 옵션은 모든 모호한 코딩에 대해 경고를 보내는 옵션이고, -W 옵션은 합법적이
지만 모호한 코딩에 대해 경고를 보내는 옵션이다. 그래서 -W -Wall 옵션을 붙이면 아
주 사소한 모호성에 대해서도 경고가 발생한다.

-02 는 최적화 레벨을 2 로 설정한다. 최적화 레벨 2 는 사이즈와 성능에 트레이드오프
(trade-off)가 없는 많은 최적화를 수행한다. -o like는 컴파일된 파일명을 like로 하라
는 의미다. 위와 같은 기본 컴파일 명령에 다음부터 설명하는 옵션들을 바탕으로 추가
할 옵션을 추가하면 된다.

4장_ gcc compiler 229

===== PAGE 231 =====
I 반드시 알아야 할 gcc 필수 옵션 및 중요 옵션
지금부터 설명할 옵션들은 너무도 자주 사용해 웬만하면 외워 두는 것이 좋을 만한 옵
션들이다. 그러니 잘 보아두기 바란다. 옵션은 gcc C 드라이버, 전처리기, C 컴파일러,
어 셈블러, 링커 옵션순으로 설명하겠다.

KI gcc C 컴파일러 드라이버 옵션
gcc C 컴파일러 드라이버 옵션에는 컴파일 과정을 어디까지 진행할지, 또는 컴파일 과
정을 출력할지 여부 등을 지정하는 옵션들이 있다.

►
-

-E
E 옵션은 전처리 과정의 결과를 화면에 보이는 옵션이다. gcc -E like.c하면 like.c

를 전처리한 후의 결과가 화면에 출력된다. 그래서 전처리 과정 중에 발생한 오류를
검증할 때 사용하면 좋다. 그렇지만 그것은 -save-temps 옵션을 모를 때의 경우고,

-save-temps 옵션을 사용해 likej 파일을 읽어보는 것이 더 좋은 방법이다.
►

-S

어셈블리 파일만 생성하고 컴파일 과정을 멈춘다. 그래서 -S 옵션을 주고 컴파일하면
［그림 4-35］ 와 같이 like.s 어셈블리 파일을 얻을 수 있다.

［그림 4-35］ gcc -S like.c 명령 수행 후 만들어진 어셈블리 파일

►

-C

오브젝트 파일까지만 생성하고 컴파일 과정을 멈춘다. 그래서 링킹 과정은 수행되지 않
는다. gcc -c like.c하면 like.c의 오브젝트 파일인 like.o 파일을 얻을 수 있다.

［그림 4-36］ gcc -c like.c 명령 수행 후 만들어진 오브젝트 파일

230 3부— 컴파일과 링킹

===== PAGE 232 =====
►

-v

이전에 많이 사용하던 -V 옵션이다. -V 옵션을 붙이면 gcc가 컴파일 과정을 어떤 식으
로 수행하는지를 화면에 자세하게 출력한다.

2

그러흐

그〉

역시 이전에 많이 사용하던 옵션이다. 컴파일 과정에서 생성되는 중간 파일인 전처리
파일(*.i)과 어셈블리 파일(*.s), 오브젝트 파일(*.o)을 지우지 않고 현재 디렉토리에 저
장한다. 컴파일 과정에서 발견되는 오류를 분석할 때 많이 사용한다.

@ cd -E 또는 cppO 전처리기 옵션
ccl -E 전처리기의 옵션은 주로 소스 내에서 사용된 헤더 파일과 define 매크로와 관
련된 옵션들이다. 전처리 과정에서 오류가 발생한다면 ccl -E의 옵션들을 점검해야 될
필요가 있다.
►니

전처리 과정에서 헤더 파일을 탐색하는 기본 디렉토리를 추가할 때 사용하는 옵션이다.
［예제 4-25］ 와 같은 예제 소스가 있을 때 소스 파일 내에서 include〈헤더 파일〉과 같
은 형식으로 include된 헤더 파일은 페도라 7 배포판에서 기본적으로 시스템 헤더 디
렉토리로

설정된

/usr/local/incl니de,

/usr/lib/gcc/i386-redhat-lin니x/4.1.2/include,

/usr/include 디 렉토리순으로 헤더 파일을 찾고, #include "헤더 파일', 형 태로 incl니de
된 헤더 파일은 현재 디렉토리에서 먼저 찾고 /니sr/local/include, /니sr/lib/gcc/i386-

redhat-lin 니 x/4.1.2/include, /니 sr/include 디렉토리순으로 찾는다.
〔예제 4-25〕 헤더 파일을 탐색하는 기본 디렉토리 추가 예제

#incliide <stdio.h>
#include "like.h"

,

：

int main()
：：

{
printf("I
return 0;

like

you!\n”);

/usr/local/include, /usr/lib/gcc/i386-redhat-linux/4.1.2/include, /usr/include
디렉토리에 stdio.h 파일이 없다면 다음과 같은 오류 메시지를 출력한다.

4장_ gcc compiler 231

===== PAGE 233 =====
혜 root@os：/temp/like2
[root(흐os like2]tt gcc -o like like.c
like.c:1:19: error: stdio.h: 그런 파일이나 디렉토리가 없음
like.c: In Function 'main':
like.c:5: warning: incompatible implicit declaration of built-in
Function 'printf'
[rooteos like2]tt |

［그림 4-37］ 헤더 파일을 못 찾아서 출력된 오류 메시지

［그림 4-3刀과 같은 오류가 발생하면 -Hinclude 디렉토리］ 옵션으로 stdio.h가 있는
디렉토리를 따로 지정해야 한다. /root/include 디렉토리에 stdio.h 파일이 있다면 -1/

root/include라고 하면 된다. -I 옵션으로 헤더 파일을 찾을 디렉토리를 추가하면 시
스템 헤더 디렉토리보다 추가한 디렉토리에서 우선적으로 찾는다. 그래서 -I/root/

include하면 제일 먼저 /root/include 디렉토리에서 헤더 파일을 찾고 /usr/local/
include,

/usr/lib/gcc/i386-redhat-linux/4.1.2/include,

/usr/include

디렉토리순으

로 헤더 파일을 찾는다.

►

-include ［헤더 파일 경로］

헤더 파일을 소스 내에 추가할 때 사용한다. 소스의 제일 처음에 #include “헤더 파일
경로”로 한 것과 동일하다. 그다지 많이 사용되지는 않지만 가끔씩 GNU 프로젝트 소스
들에서 사용한다.
► -이매크로］
매크로를 외부에서 define할 때 사용한다. ［예제 4-26］ 을 gcc -DDEBUG -o like

like.c 명 령으로 컴파일하면 소스의 제일 앞에 #define DEBUG문을 추가한 것과 동일
하다. 주로 ［예제 4-26］ 에서와 같이 디버깅 메시지 활성 또는 비활성화 등과 같이 컴파
일 과정에서 특정 코드를 추가/제거하는 용도로 많이 사용한다.
〔예제 4-26〕 디버깅 메시지 활성 또는 비활성화 예제

#include <stdio.h>
int main()
#ifdef DEBUG
printf("Debug message : I like you!\n");
#endif
return 0;
}

232 3부— 컴파일과 링킹

===== PAGE 234 =====
［그림 4-38］ 은 gcc로 컴파일 시 -DDEBUG 옵션을 사용해 외부에서 define해 컴파일
한 후 실행한 모습이다.
터 root@os：/temp/like2
like2]it gcc -o like like.c
[rootdos
[rooteos
like2]# ./like
[rooteos
like2]#
[root@os
like2]tt gcc |-DDEBUG |-o like like.c
[root@os
like2]#
[root(흐 os like2]# ./like
Debug message : I like you?
[rooteos like2]tt |

［그림 4-38］ 컴파일 후 실행 모습

► -이매크로］늬매크로 값］
소스 파일 시작 부분에 #define ［매크로］ ［매크로 값］문을 추가한 것과 동일하다. ［예제

4-2刀을 gcc -DPACKAGE=\"likeU\"-o like like.c 명령으로 컴파일하면 “package :
likeU” 문자가 출력되고 소스 파일의 제일 처음에 #define PACKAGE HlikeUH문을 추
가한 것과 동일하다.
〔예제 4-27〕 매크로 정의와 매크로 값 지정 예제

#include <stdio.h>
int main()
{
printf("package : %s\n", PACKAGE);
return 0;
}

® root@os:/temp/like2
fiGteos like2]¥ gcc |—DPfiCKftGE나#,•likelike.c
[root(흐os like2]tt
[root(흐os like2]# ./like
package : likeU
[root(흐os like2]tt |

［그림 4-39］ —DPACKAGE=\"likell\” 옵션으로 컴파일 후 실행

►

-u ［매크로］

-U는 -D와 반대로 소스 파일 첫 부분에 Wndef ［매크로］ 옵션을 추가한 것과 동일하
다. 거의 사용하지 않는다.

4장_ gcc compiler

233

===== PAGE 235 =====
►

—M 과 —MM

나중에 배울 make의 기술 파일인 Makefile을 작성할 때 유용한 종속 항목 리스트를 출
력한다. 여기서 종속 항목이란 타겟이 컴파일되기 위해 필요한 항목을 의미한다. 예를
들면 ［예제 4-2刀의 소스 코드에서 like 실행 파일은 like.c 소스 파일이 필요하고, 또한

like.c는 stdio.h 파일을 include하고 있기 때문에 stdioh 파일도 필요하다.
또한 like 는 stdioh 가 include 하고 있는 여러 헤더 파일도 필요로 한다. 이런 종속 관
계를 make의 기술 파일에서 사용하는 형식으로 정리해 출력한다. -M 옵션은 make를
위한 소스 파일의 모든 종속 항목을 출력하고, -MM 옵션은 기본 include 디 렉토리에
있는 헤더 파일은 빼고 종속 항목을 출력한다. -M 과 -MM 옵션은 나중에 배울 make
유틸리티에서 매우 유용하게 사용할 수 있기 때문에 make를 설명할 때 따로 설명한다.
■ root@os：/temp/like2
[rootQos like2]tt gcc -M like.c
like.o: like.c /usr/include/stdio.h /usr/include/features.h tt
/usr/include/sys/cdefs.h /usr/include/bits/wordsize.h tf
/usr/lnclude/gnu/stubs.h /usr/include/gnu/stubs-32.h tf
/usr/lib/gcc/i386-redhat-linux/4.1.2/include/stddeF.h tf
/usr/include/bits/t^pes.h /usr/include/bits/typesizes.h tf
/usr/include/libio.h /usr/include/ G config.h /usr/include/wch
ar.h tt
/usr/include/bits/wchar.h /usr/include/gconu.h tf
/usr/lib/gcc/i386-redhat-linux/4.1.2/include/stdarg.h tt
/usr/include/bits/stdio_liin.h /usr/include/bits/sys_errlist.h
[rootQos like2]tt |

［그림 4-40］ -M 옵션으로 like.c 파일의 종속 항목을 본 예

►

-nostdinc

디폴트 include 디렉토리 (즉, /usr/include 디렉토리)에서 헤더 파일을 탐색하지 않고

-I 옵션으로 추가한 디렉토리에서만 헤더 파일을 찾는다. 운영체제 커널처럼 표준 C 함
수를 사용하지 않는 프로그램을 컴파일할 때 잘못된 include로 인해 오류가 발생하는
것을 방지하려 할 때 사용한다.

►

-C

- E 옵션과 함께 사용하며 전처리 과정에서 주석을 제거하지 않는다. 그리 많이 사용하
지는 않지만 전처리 과정 오류 파악에 사용하면 유용하다.

►

-Wp,［옵션들］

전처리기 (ccl -E) 와 C 컴파일러 드라이버 (gcc) 의 옵션이 서로 동일하다면 해당 옵션
은 C 컴파일러 드라이버의 옵션으로 처리된다. gcc 가 옵션을 해석해 ccl -E, ccl, as,

collect2에 옵션을 전달하기 때문이다. 한마디로 주종 관계로서 gcc가 모든 컴파일 도
구의 주인이기 때문에 그렇다.

234 3부_ 컴파일과 링킹

===== PAGE 236 =====
gcc 의 해석을 거치지 않고 바로 전처리기의 옵션으로 전달하고 싶을 때 -Wp 옵션
을 사용한다. -Wp,-DDEBUG,-I/usr/include,-M 으로 사용하면 전처리기 (ccl -E) 로

-DDEBUG -I/usr/include -M 옵션이 바로 전달된다.
이상으로 전처리기 옵션 설명이 끝났다. 다음으로 가장 많은 옵션을 가지고 있는 C 컴
파일러(ccl)의 옵션에 대해 알아본다.

@ cd C 컴파일러의 옵션
gcc의 수많은 옵션 중 거의 대부분의 옵션은 바로 CC1 의 옵션이다. CC1 의 옵션은 크게
4가지 종류로 나눌 수 있는데, C 언어 옵션, 경고 옵션, 최적화 옵션, 디버깅 옵션이다.
ccl 의 옵션을 잘 활용해 경고의 수위를 조절하거나 최적화 수위를 조절할 수 있다. 각
각의 옵션을 종류별로 설명하면 다음과 같다.
►

C 언어 옵션

주로 C 언어 종류와 표준과 관련된 옵션으로, 각 C 언어 종류와 표준에 부합하는 C 소
스를 작성하려 할 때 사용한다. C 언어는 여러 종류가 있는데, gcc에서 지원하는 C 언
어는 3가지가 있다. 흔히 K&R C라고 이야기하는 오래된 Traditional C와 ANSI C, 그
리고 GNU에서 확장한 GNU C가 그것이다. 기본적으로 gcc는 GNU C89 문법으로 문
법을 체크한다.
—ansi

ANSI C 표준에 부합하는 소스를 작성하려 할 때 사용하는 옵션이다. -ansi 옵션을 붙
이면 ANSI C 표준(ISO C89)으로 문법 체크를 하고 GNU C의 확장 문법은 사용 불가
능하다. 이식성 높은 소스를 작성하려면 -ansi 옵션을 사용해 ANSI C 표준 문법으로
소스 코드를 체크하기 바란다. -ansi 옵션을 사용하기로 마음먹 었다면 -pedantic 옵션
도 함께 사용하기 바란다. -pedantic 옵션을 사용하지 않으면 gcc 버 전에 따라 ANSI

C 표준에 맞지 않은 문법일지라도 컴파일할 수 있다. 또한 ANSI C 표준 문법에서는
C++ 단일 라인 주석 (//) 및 asm, typeof 같은 키워드 등을 사용할 수 없다.
-std=[C 표준들]

기타 다른 표준들을 지정하려 할 때 사용한다. 지정 가능한 C 표준들은 다음과 같다.

4장_ gcc compiler 235

===== PAGE 237 =====
• c89 또는 iso9899：1990
ANSI C89 표준이다. 1989년에 제정되어 C89이고 위에서 -ansi 옵션을 준 것과 동
일하다.
예) -std=c89
다음 예는 ANSI C89 표준에 정의되어 있는 3중자를 사용한 소스 코드인데, 이런 것
도 표준에 있다는 것을 알려주기 위해 넣었다.
〔예제 4-28)

3중자를 사용한 C 소스 코드

??=include <stdio.h>
int main ()
??<
printf("I like you.\n");
??>

c 표준들에서는 종교 혹은 문화적인 문제로 인해 e에서 사용하는 문자 셋을 사용할
수 없는 국가들을 위해 3중자 혹은 2중자를 정의해 뒀는데, 위 소스가 3중자를 사용
한 C 소스 코드다. 무척 생소하겠지만 C89 표준으로 작성된 소스다. 위 소스는 -ansi
혹은 -std=c89 옵션을 지정해야만 컴파일할 수 있다. 3중자 혹은 2중자는 전처리 과
정 이 전에 C에서 사용하는 문자들로 치환된다.

• c99 또는 iso9899：1999
1999년에 새로 제정된 ANSI C 표준이다. gcc 3.x 버전부터 사용 가능하며, 그 이전
버전은 사용 불가능하다. 기존의 C89에 비해 많은 새로운 문법이 추가되었고 새로운
기술들이 접목되었다. C99의 문법대로 작성하면 다음과 같은 코드도 작성 가능하다
〔예제 4-29)

ANSI C99 표준 소스 코드

#include <stdio.h>

；

int main()
{

：

printf("Hello, C99\n");
int
for

a = 9;
(int i=0;
i<10; i++)
{
printf ("i =
%d\n", i);

；
：

:

}

i

int array[3] = { a*2, a-1, a/2 };
for
(int i=0;
i<3;
i++) {

：

236 3부— 컴파일과 링킹

===== PAGE 238 =====
printf("array[i] = %d\n", array[i]);
}
return

0;

}

C 소스이지만 마치 C++ 소스 문법처럼 작성됐다. 위 소스 코드를 컴파일하려면 반드
시 -std=c99 옵션을 지정해야 한다.

［그림 4-41］ C99 예제 소스 컴파일 및 실행

• gnu89
GNU에서 제정한 GNU C89 표준으로 문법을 체크한다. 전체적으로 C99와 유사하
지만 C99와 완전 동일하지는 않다. 가령 위 C99 문법의 소스에서 for문 안에 변수를
정의한 것과 같은 것은 GNU C89의 문법에서 사용할 수 없다.

• gnu99
GNU C99 표준으로 문법을 체크한다.
위에서 설명한 표준들이 대표적인 표준들이고, 위에서 설명한 것 외에도 몇 가지 표
준이 더 있다. 나머지 표준들에 대해서는 gcc 매뉴얼을 참고하기 바란다.
-traditional

오래된 Traditional C（다른 말로 K&R C） 문법으로 문법을 검사한다. ［예제 4-30］ 과
같은 문법의 C 소스를 한 번쯤 보았을 것이다. 이 게 바로 Traditional C 문법으로 작성
된 C 소스다. -traditional 옵션은 하위 호환을 위해 존재할 뿐이고 gcc 3.x 버전부터
지원하지 않는다.

4장_ gcc compiler 237

===== PAGE 239 =====
〔예제 4-30)

Traditional C 스스

void func(a, b)
int a;
int b;
{
int c;
c = a + b;
}
int main()
{
func (1, 2);
return 0;
}

-fno-asm

gn니89 문법에서 지원하는 asm, inline, typeof 키워드를 사용하지 않는다. gcc는 기본
적으로 gnu89 문법으로 문법을 체크하는데, asm은 C 소스 내에 어셈블리 코드를 삽입
할 때 사용하고, inline은 인라인 함수를 지정할 때, typeof 키워드는 변수의 타입을 알
아볼 때 사용한다. 이런 asm, inline, typeof 키워드는 ANSI C89 표준에서는 지원하지
않기

때문에

ANSI

C89에서

지원하는

asm

inline

typeof

키워드를

사

용해야 한다. gnu89 문법을 바탕으로 asm, inline, typeof 키워드를 사용하지 않으려
할 때 -fno-asm 옵션을 사용한다.
〔예제 4-31J

_asm_ 키워드를 사용한 예제 소스

#include <stdio.h>
int main()
{
// asm( "nopXn");
__asm___ ( "nop\n" ) ;
printf(”I like you!\n");
return 0;
}

238 =_ 컴파일과 링킹

===== PAGE 240 =====
〔예제 4-32〕

_typeof__ 키워드를 사용한 예제 소스

#include <stdio.h>
#define xchg(x,y) do {___________ typeof____ (x) tmp = x; \
x = y; \
y = tmp; \
} while(0)
int main()
{
int a = 1, b = 2;
char c = 'a', d = 'b';
xchg(a,b);
xchg(c,d);
printf ("a = %d, b = 응d\n", a, b);
printf("c = %c, d = %c\n", c, d);
return 0;
}

► 경고옵션

ccl 의 옵션을 조정해 경고 수위를 조절할 수 있다. gcc 는 경고 수위 조절에 있어서 많
은 융통성을 제공하기 때문에 문법 체크의 엄격성을 제공하면서도 원하지 않는 경고를
없앨 수 있다. 보통의 경우 모든 경고를 활성화시키는 -Wall -W 옵션을 사용해 컴파일
한다. 그렇지만 -Wall -W 옵션을 사용하면 정말 지나칠 정도로 사소한 것까지 경고를
출력하기 때문에 보기 안 좋은 컴파일이 되곤 한다. 경고 옵션에서 중요하게 보아야 될
것은 -Wall -W 옵션을 사용해 모든 경고 메시지를 활성화시켰을 때 어떻게 수위를 조
절할지 아는 것이다.
— W고F -Wall

-Wall 옵션은 모든 모호한 문법에 대한 경고 메시지를 출력한다. 그리고 -W는 합법적
이지만 모호한 코딩에 대해 부가적인 정보를 제공한다. 소스 코드의 엄격성을 보장하려
면 두 옵션은 반드시 사용하는 것이 좋다.
예） gcc -W -Wall -o test test.c

- W -Wall 옵션을 주어 모든 경고 메시지를 활성화시키면 무시하고 싶은 아주 사소한
문법적 오류도 경고 메시지로 출력한다.

4장_ gcc com에er 239

===== PAGE 241 =====
〔예제 4-33)

like.c 파일의 내용

#include <stdio.h>
void unused_func()

{

；
printf("unused function!\n");

}

：

int main()

；

{
int a;
printf ("I like you.\n");
return 0;

}

；

|

가령 [예제 4-33] 과 같은 like.c 파일이 있을 때 -W -Wall 옵션으로 컴파일하면 다음
과 같은 경고 메시지가 출력되는 것을 볼 수 있다.
[H root@os:/temp/like2
[rootBos like2]ft gcc -W -Wall -o like like
like.c: In function 'main1:
like.c:19: warning: unused uariable 'a'
[rooteos like2]tt |

［그림 4-42］ 사소한 경고 메시지

main() 함수에서 int a； 변수가 정의되었는데 사용되지 않았다고 나타나는 경고 메시지
다. 그리고 어떤 버전의 gcc 같은 경우 unused_func() 함수와 같이 정의되었는데 사용
되지 않은 함수에 대해서도 경고 메시지를 출력한다.
이런 아주 사소한 경고 메시지를 없애려면 -Wno-［제거할 경고］ 옵션을 붙이면 된다.
여기서 제거할 경고 옵션은 man gcc 명령으로 gcc 옵션들의 리스트를 보았을 때 -W
문자로 시작하는 아래와 같은 옵션들이다.
-Wunused, -Wunused-function, -Wunused-label, -Wunused-parameter,
-Wunused-value, -Wunused-variable, -Wwrite-strings, •••

가령 정의는 되었지만 사용되지 않은 변수에 대한 경고 메시지는 -Wno-unused-

variable 옵션을 사용해 없앨 수 있고, 사용되지 않은 함수에 대한 경고 메시지는
-Wno-unused-function 옵션을 사용해 없앨 수 있다. 그리고 둘 다를 포함한 모든 사
용하지 않은 경고 메시지를 없애려면 -Wno-unused 옵션을 사용한다. ［그림 4-43］ 은

240 3부_ 컴파일과 링킹

===== PAGE 242 =====
이전의

like.c 소스에서

-Wno-니nused-function 옵션과

-Wno-unused-variable을

사용해 un니sed_func() 함수와 a 변수가 사용되지 않은 데 대한 경고 메시지를 없애는
예를 보여준다.
|테 mot@os：/temp/like2
[rootSos like2]tt gcc -W-Wall[
[root（흐os like2]tt |

-I QI x|
-Wno—unused-Function -Wno-unused-uariable[-0 like like.c Q

［그림 4-43］ 사소한 경고 메시지 제거

물론 이런 사용되지 않은 변수가 크게 문제를 일으키지는 않을 것이다. 그리고 개발이
끝나면 프로젝트 정리 차워에서 사용되지 않은 변수들은 모두 제거될 것이다. 하지만
개발 중간에 소스의 변동이 심할 때 이런 변수들이 나타나 컴파일 과정에서 오류 메시
지를 뿌리면 여간 성가신 게 아니다. 물론 다소 너그러운 사람들도 있겠지만 필자와 같
이 경고 메시지 자체를 혐오하는 성향을 가진 많은(?) 사람은 충분히 공감할거라 생각
한다.
아래와 같은 test.c 파일을 -W -Wall 옵션으로 컴파일하면 “division by zero” 경고가 출력된다.
test.c 파일 내용

： int main()
：{
；

int b;

：

b = 1/0;

；

return 0;

-‘
i

；}

；

|

이런 test.c를 -W -Wall 옵션으로 컴파일하면서 소스 수정 없이 경고 메시지를 제거해 보자. 제거할 경
고 옵션은 man gcc 명령을 내렸을 때 “Warning Options” 부분에서 찾을 수 있다.

-w

모든 경고 메시지를 제거한다. 그래서 -W 옵션을 사용하면 모든 경고 메시지가 출력
되지 않는다. -W 옵션은 -Wall, -W［옵션명］ 등의 경고 옵션들보다 우선시되므로 다른
경고 옵션을 붙이더라도 경고가 출력되지 않는다.
경고는 일종의 잠재적 오류다. 언제든 특정한 상황에서 경고는 오류가 될 수 있다. 그렇
기 때문에 -w 옵션을 사용해 모든 경고를 제거하는 것은 좋지 않은 방법이다. 경고에

4장_ gcc compiler 241

===== PAGE 243 =====
는 이유와 원인이 있기 마련이고, 눈에 보이는 경고를 보이지 않게 하는 것보다는 이유
와 원인을 파악해 경고를 제거하는 것이 현명한 방법이다. 이런 것에 반드시 습관을 들
이기 바란다.
-Werror

모든 경고는 컴파일을 중단하는 오류로 취급한다. 그래서 경고가 하나만 발생해도 컴파
일 과정은 중단된다.
—pedantic

ANSI C89 표준에서 요구하는 모든 경고 메시지를 표시한다. ANSI 표준 문법으로 소스
코드를 작성하려 할 때는 -ansi 옵션과 함께 반드시 -pedantic 옵션도 같이 사용하기
바란다.
—pedantic—errors

ANSI C89 표준에서 요구하는 모든 경고를 오류로 취급한다.
-Wtraditional

소스가 ANSI C와 K&R C 간에 서로 다른 결과를 가져올 수 있는 부분이 있다면 경고
한다. 거의 쓸 일이 없다. 그러니 잊어버려라.
►최적화 옵션
이전에 최적화가 세계 평화에 이바지할 수 있다고 하였다. 최적화가 중요한 이유는 한
번 컴파일된 실행 파일은 언제까지고 계속 사용할 수 있다는 점 때문이다.

1s 같은 프로그램을 상상해 보자. 1s는 유닉스 시스템에서 필수 명령이고, 한 번 설치되
면 바꿀 일이 거의 없다. 독자가 유닉스 시스템을 사용하면서 얼마나 많은 1s 명 령을 사
용하는지 생각해 보면 최적화를 통한 속도 향상이 시스템 전체 사용 시간으로 봤을 때
얼마나 중요한지 알 수 있다.

gcc 컴파일러는 이런 최적화를 위해 수많은 기법을 제공한다. 앞서도 설명했듯이 gcc
의 컴파일 시간 대부분은 최적화를 위한 코드 분석과 최적화를 수행하면서 소비한다.
그리고 gcc의 소스 코드 상당 부분은 최적화를 위한 코드들로 이뤄졌다. 최적화 기법은
여러 가지가 있을 수 있는데, 보통 다음과 같은 최적화 기법들이 있다.
• 과도한 함수 호출 제거
• 상수의 전달과 변수 복제 전달의 최적화

242 3부_ 컴파일과 링킹

===== PAGE 244 =====
• 불필요한 loop 제거
• 상수의 곱셈 최적화
• 함수 호출 인수의 지 연된 pop 동작 방지 (스택 최소화)
• 재귀 호출이 함수의 최종부에서 일어나지 않도록 최적화
• 효율적인 레지스터 할당
• 유추에 의한 변수 최적화

• inline 함수의 최적화와 스택 프레임 포인터의 제거
• 각 명령의 실행 사이클을 고려한 스케줄링
• 반복되는 코드의 제거
• 루프에서의 동작 불변 코드 옮김
• 각 하드웨어에서 지원하는 단축 명령 기능에 의한 지역 최적화

gcc는 최적화에 대해서도 굉장한 유연성을 제공한다. 최적화 기법을 일일이 선택해 최
적화할 수도 있고, -()［최적화 레벨］ 옵션으로 미리 여러 최적화 기법을 묶어 놓은 최
적화 방법을 사용할 수도 있다. man gcc 명 령으로 gcc의 옵션들을 보았을 때 가장 많
은 옵션을 가지고 있는 것이 Optimization Options 종류다. 각 옵션은 각각의 최적화
기법을 사용함을 의미하며, 각 옵션의 최적화 기법은 man gcc 명령으로 자세히 알 수
있다.

-O 옵션은 이런 개개의 최적화 옵션 중 어떤 아키텍처에서든 사용할 수 있는 옵션들을
묶어 최적화 레벨을 설정할 때 이용한다. 보통의 경우 -O［최적화 레벨］ 옵션으로 최적
화 레벨을 선택하고 몇몇 최적화 옵션에 대해서만 -f 옵션을 사용해 세부 설정하는 방
법을 사용한다
때문에 gcc 최적화에서는 가장 먼저 -O 옵션부터 이야기되어야 한다. 그러면 -O［최
적화 레벨］ 옵션에 대해 알아보자.

-00
어떤 최적화도 수행하지 않는다. 소스 내에 함수 선언 시 inline 키워드를 사용해 인라인
함수를 명시했더라도 인라인 함수가사용된 데 대해 인라인 확장이 일어나지 않는다. 컴
파일 시 아무런 최적화 옵션도 붙이지 않으면 -O0 옵션을 준 것과 동일하다.

4 장_ gcc compiler 243

===== PAGE 245 =====
최적화 테스트를 위해 다음과 같은 코드를 작성하고 -00 옵션으로 컴파일해 보자.
〔예제 4-34〕 test.c 최적화 테스트 코드

#include <stdio.h>
int a, b, c;
int fund (int argl, int arg2)
int i, j, k;
for (i=0; i<0xfffff; i++) {
j = argl 十 arg2;
k=j*2*4*8*16;
if (1%2) a = argl + arg2 + i * 8 + k;
}
return a;

inline int func2(int al,
{
int i, j, t = 4;
for (i=0; i<0xfffff;
j = 3 * t;
b = 3 * t / (i +
}
return b += j；

int main()
{
int i, h, y;
h = y = 0;
for (i=0; i<0xf; i++) {
for (h=0; h<0xf; h++) {
y = fund (h, i) ;
func2 (i, y);

for (h=0; h<0xf; h += 2) {
c = fund (y, 2) ;
b = func2 (h, i);
}
}
printf("END : %d %d\n", a, b);
return 0;

244 W_ 컴파일과 링킹

int a2)

i += 2) {
1) ；

===== PAGE 246 =====
［예제 4-34］ 의 소스는 -O 옵션의 레벨별 최적화 기법들을 모두 테스트하기에 좋은 예제
는 아니다. -O 옵션의 레벨별 모든 최적화 기법을 다 적용할 수 있는 예제 코드를 짧게
작성하기란 의외로 쉽지 않다. 위 예제는 필자가 임의로 적당히 작성한 예제 코드다.

gcc -OO -save-temps -o test test.c 명령으로 컴파일한 후 사이즈와 실행 속도를 알
아보면 다음과 같다.
H root@os ：/temp/like2^
[root@os like2]tt gcc -08 -saue—temps -o test test.c
[rootdos like2]tt Is -al test
—rwxr-xr-x 1 root root| 5270 |2O07-11 —86 05:18 test
[root（흐os like2]tt
[root（흐os like2]tt time ./test
END : 46180350 12
real
BnS.209s.
user'
0n2747'!5&]
sys
OmO.002s
[root（흐os like2]tt |

H
［그림 4-44］

-00 옵션으로 컴파일한 후 사이즈와 실행 시간을 테스트

time 명령은 정확한 수행 속도 및 성능 측정에는 알맞지 않다. 그렇지만 프로그램 수행
시간 측정을 위해 간단하게 사용할 만은 하다. 결과 화면을 보면 사이즈는 5270바이트
고 실행 시간은 총 5.209초가 걸렸는데, 이 중 유저 모드에서는 2.475초가 걸렸다. ［예
제 4-34］ 의 코드는 커널 모드에서 동작하는 코드가 마지막 printfO 함수 빼고는 없기
때문에 유저 모드에서 동작한 시간만 보면 된다. 그리고 컴파일된 어셈블리 파일을 보
면 다음과 같은 부분이 보일 것이다.
. . . main 함수 부분
... 상략

call
fund
movl
응eax,
-8(%ebp)
movl
-8(%ebp), %eax
movl
%eax,
4(%esp)
movl -16(%ebp), %eax
movl
%eax,
(%esp)
call
func2
... 하략

func2는 분명히 인라인 함수인데, 인라인 확장되지 않고 그냥 함수로 취급되어 call 인
스트럭션으로 호출되는 것이 보일 것이다. 이 렇게 인라인 함수가 확장되지 않는다면 인
라인 함수를 많이 사용하는 리눅스 커널에서 문제가 생길 수 있다.

4장_ gcc compiler 245

===== PAGE 247 =====
커널에서 사용된 인라인 함수 중에는 인라인으로 확장된다는 전제하에 어셈블리로 코
팅되어 있는 인라인 함수가 많기 때문이다. 컴파일 시 최적화 옵션을 주지 않거나 -00
로 최적화를 수행하지 않으면 인라인 함수가 확장되지 않는다는 데 주의하고, 인라인
확장만 원한다면 -finline 옵션을 추가하자.

-01
-O1 옵션은 -O 옵션과 동일하다. -O1 옵션은 gcc 에서 수행하는 효과가 큰 몇 가지
기본 최적화를 수행한다. -O1 옵션에 의해 활성화되는 최적화 옵션은 다음과 같다.
[표 4-3] -01 옵션에 포함된 최적화 옵션
최적화옵션

설명

-fdefer-pop

스택에 여러 함수의 리턴 값을 쌓아두고 한꺼번에 pop한다. -fdefer-pop
옵션을 주지 않으면 함수가 리턴될 때마다 매번 함수의 리턴 값을 스택에서
pop한다. 굳이 바로 사용해야 될 리턴 값이 아니라면 바로 pop하는 것보다

는 한꺼번에 pop하는 게 훨씬 효율적이다.
-fdelayed-branch

타겟 아키텍처가 지연 분기(delayed branch)# 지원한다면 분기 명령 이후
에 유효한 다른 인스트럭션을 스케줄링해 넣는다. 예를 들면 add a, b； jump
L1；이라는 명령이 있을 때 jump 명령에 의해 파이프라인이 깨어져 지연이 발
생하는데, 지연 분기를 지원하는 아키텍처에서는 브랜치 명령 바로 뒤에 오
는 인스트럭션은 브랜치 명령과 함께 수행할 수 있다. 그래서 지연 분기를
지원하는 아키텍처에서는 인스트럭션을 jump L1； add a, b；로 바꿈으로써
jump 명령과 함께 add 명령이 수행될 수 있게 하는 기법을 사용할 수 있다.

-fguess-branch-probability

분기 예측의 정확도를 높이기 위해 제어 흐름 그래프(Control—Flow Graph)
기반의 휴리스틱 분기 예측 알고리즘을 사용한다. 쉽게 이야기하면 if(a) {A}
이se {B}문이 있을 때 a 값에 의해 A 문장이 수행될지 B 문장이 수행될지 결
정된다. gcc는 어떤 문장이 더 자주 수행될지를 제어 흐름 그래프 기반의 휴
리스틱 알고리즘을 통해 예측할 수 있다.

-fguess-branch-probability

옵션이 분기 예측 기능을 켠다. 그래서 분기문이 좀 더 효율적으로 구성되게
코드를 생성할 수 있다. 분기 예측은 이런 휴리스틱 알고리즘으로도 가능하
고_______________ 함수를 사용해 프로그래머가 명시적으로 gcc에게 알
려줄 수도 있으며, 나중에 설명할 프로파일 결과를 통해서도 gcc에 알려줄
수 있다.

-fcprop-registers

레지스터 할당과 post 레지스터 할당 이후에 레지스터 복사(예: mov rO, r1)
를 제거하고, 스케줄링 종속성을 줄이기 위해 복사 전파(copy propagation)
과정을 수행한다.

-floop-optimize

각종 루프 최적화를 수행한다. 루프 내에 변하지 않는 코드들을 루프 밖으로
옮기고 루프 종료 테스트 상태를 좀 더 단순하게 만든다.

-fif-conversion

조건 분기 인스트럭션(예: ble, bit)을 분기하지 않는 형태의 코드로 변경할 수
있다면 변경한다.

-fif—conversion2

조건 수행 인스트럭션(예: addlt, suble)을 사용해 조건 분기 인스트럭션을
분기하지 않는 형태의 코드로 변경한다.

246 3부_ 컴파일과 링킹

===== PAGE 248 =====
최적화 옵션
-ftree-ccp

설명

트리에서 sparse 조건부 상수 전파(conditional constant propagation) 과정
을수행한다.

-ftree-dce

트리에서 사용되지 않은 코드를 제거(dead code 이imination)한다.

-ftree-dominator-opts

도미네이터 트리 traversal에 기초한 다양한 스칼라 크린업을 수행한다.

-ftree-ter

SSA 트리 표현에서 일반적인 트리 표현으로 변환하는 단계에서 한 번만 정

의하고 한 번만 사용하는 임시 변수를 해당 변수가 사용되는 위치에 정의하
게 바꾼다. 이렇게 하면 해당 변수의 라이브 구간(live range)이 감소해 레지
스터 할당이 수월해진다.
-ftree-lrs

SSA 트리 표현에서 일반적인 트리 표현으로 변환하는 단계에서 변수들의

라이브 구간(live range)을 잘게 자른다. 이는 레지스터 할당 과정에서 각 변
수를 스택에 할당하지 않고 좀 더 많이 레지스터에 할당하기 위해 필요한 과
정이다.
-ftree-sra

집합의 스칼라 변환을 수행한다. 이 과정은 구조체를 너무 일찍 메모리로 바
꾸는 것을 막기 위해 구조체 참조들을 스칼라로 바꾸는 것을 말한다.

-ftree-copyrename

트리에서 copy renaming을 수행한다.

-ftree-fre

트리에서 전체 중복성 제거(Full Redundancy 티mination) 과정을 수행한다.

-ftree-ch

트리에서 루프 헤더 복사를 수행한다. 이렇게 하면 코드 모션 최적화의 효과
를 증대시킬 수 있다.

—funit—at—a—time

코드를 만들기 전에 모든 compilation 유닛을 구성 요소로 분석한다.

-fmerge-constants

com 에 ation 유닛들을 통틀어 동일한 상수 (string constants and floating
point constants)# 합친다.

최대한 이해하기 쉽게 풀어 쓰려고 노력을 했는데 실패했다는 생각이 든다. 대부분 컴
파일러 관련 용어이므로 컴파일러와 아키텍처에 대한 배경 지식이 없으면 무슨 말을
하는지 다소 이해하기 어려울 것이다. 사실 모두 영어로 된 컴파일러 알고리즘들을 억
지로 한글로 번역해 놓고 보니 영어 알고리즘 이름에만 익숙한 필자도 이해하기 힘들
정도다.
굳이 이해하지 않아도 된다. 그냥 -O1 옵션에서는 이런 것들을 수행하는구나, 혹은 그
렇겠거니 하고 넘어가도 앞으로 독자들이 유닉스/리눅스 시스템에서 프로그래밍하는
데 아무런 지장이 없다. 그러니 이해가 안 된다고 전혀 걱정하지 말기 바란다.
위 내용 중_________________________재미난 빌트인 함수가 있는데, 이에 대해서
는 “binutils 를 사용한 최적화” 과정에서 설명한다. 모든 최적화를 다 설명하긴 힘들
고 -Hoop-optimize 옵션에서 포함하는 루프 최적화 중 루프 불변 코드 이동 (loop

invariant code motion)이라는 최적화 알고리즘만 간단히 알아보자.

4장_ gcc compiler 247

===== PAGE 249 =====
컴파일러 최적화에 있어 루프를 최적화하는 것은 매우 중요하다. 프로그램에서 80% 이
상 수행 시간을 좌우하는 것이 바로 루프 부분이기 때문이다. 때문에 컴파일러는 되도
록 루프 부분을 최적화하기 위해 노력한다. 이런 루프 최적화 알고리즘 중 루프 불변
코드 이동이라는 최적화 알고리즘이 있는데, 이 알고리즘은 루프 내에서 변하지 않는
코드를 밖으로 빼는 알고리즘이다.
〔예제 4-35] 수 루프 불변 코드 이동(loop invariant code motion) 알고리즘 예

y = 1 + 2；
for (i=0; i<n; i++) {
j = j + 2;
k = y + 3;
z = k + 1;

y = 1 + 2；
k = y + 3;
z = k + 1;
for (i=0; i<n; i++) {
j = j + 2;
}

}

루프 불변 코드란 루프가 돌 때 값이 변하지 않는 코드를 말한다. 위 예제에서 좌측이
원본 코드인데, 원본 코드의 k = y + 3；와 z = k + 1；과 같은 코드가 루프 불변 코드에
해당한다. 아무리 루프를 많이 돌아도 k 값과 z 값은 변하지 않는다.
“누가 이런 바보 같은 코드를 생성할까?”라고 말하겠지만 프로그래머가 명시적으로 생
성하지 않더라도 최적화 과정에서 저절로 생긴다. 이런 루프 불변 코드를 루프 바깥으
로 옮기는 것이 루프 불변 코드 이동 알고리즘이 하는 일이다.
루프 불변 = 이동 알고리즘을 수행하고 나면 우측에 보는 것과 같이 루프 몸체가 줄
어든다. 눈으로 보기에는 이렇게 간단하지만 사실 이 알고리즘은 그렇게 단순하지만은
않다. 루프 불변 코드를 찾기 위해 수행하는 알고리즘과 실제 이동에는 많은 분석이 필
요하다. 하지만 뭐 어쩌겠는가? 알고리즘이 복잡하던 복잡하지 않던 우리는 루프 불변
코드 이동 알고리즘이 결국 루프 내에 있는 불변 코드를 밖으로 옮기는 거라고만 이해
하면 된다.
나머지 다른 옵션 설명들이 표에서 설명한 것만으로도 이해가 되었으면 좋겠지만 이해
가 되지 않더라도 문제될 건 없으리라 생각한다. 때문에 다른 옵션들에 대해서는 따로
설명하지 않겠다.
그러면 -O1 옵션을 주고 컴파일하면 어떤 결과가 나오는지 알아보자. 다음은 -O1 옵
션을 주고 [예제 4-34] 파일을 컴파일한 후 사이즈와 실행 시간을 비교한 것이다.

248 3부_ 컴파일과 링킹

===== PAGE 250 =====
'지 root@os：/temp/like2
[root@os like2]tt gee -01 -saue-tenps -o test test.c
[rootdos like2]# Is -al test
-rwxr-xr-x 1 root root| 5174~]2007-11-86 12:09 test
[rootSos like2]tt
[root（흐os like2]# time ./test
END : 46180350 12
real
0|113.1555느
user
6RT77A7：' |
sys~" 0m0.802s
[root（흐os Iike2]tt |

[그림 4-45] -01 옵션으로 컴파일한 후 사이즈와 실행 시간을 테스트

실행 속도는 최적화하지 않았을 때인 2.475초보다 확실히 향상되었고, 사이즈도 최적
화하지 않은 5270바이트에서 조금 줄어든 것을 확인할 수 있다. 그리고 test.s 파일을
열어보면 인라인 함수인 func2() 함수가 확장된 것도 확인할 수 있다.
• . • main 함수 부분
• • • 상략

call fund
movl
%eax, 응edi
movl
$1, %ecx
movl
$12, %ebx
.L12:
movl
옹ebx, %edx
movl
%ebx, %eax
sari
$31, %edx
idivl
%ecx
addl
$2, %ecx
cmpl
$1048577, %ecx
jne .L12
addl
$12, %eax
movl
옹eax, b
addl
$1, %esi
cmpl
$15, %esi
jne .Lil
movw
$0, %si
movl
$12, %ebx
. L15 :
movl $2, 4 (%esp)
movl
응edi, (%esp)
call
fund
... 하략

굵은 글씨로 되어 있는 부분이 바로 func2() 함수가 인라인 확장된 부분이다. funclO
함수는 call 인스트럭션으로 호출한 반면 func2() 함수는 call func2 대신 func2() 함수
의 인스트럭션이 자리하고 있음을 확인할 수 있다.

4장_ gcc compiler 249

===== PAGE 251 =====
-02
가장 많이 사용하는 최적화 옵션이고 일반 애플리케이션이나 커널을 컴파일할 때 주로
사용한다. -02 옵션은 수행 속도와 사이즈 간에 트레이드오프가 존재하지 않는 거의
모든 최적화를 수행한다. -02 옵션은 -O1 옵션에 포함된 모든 최적화를 기본적으로
수행하고 다음과 같은 최적화를 더 수행한다.
[표 4-4] -02 옵션에서 추가되는 최적화 옵션들
옵션

| 설명

-fthread-jumps

중복된 비교 점프문을 최적화한다.

—fcrossjumping

= 사이즈를 줄이기 위해 크로스 점핑 변환을 수행한다.

-foptimize-sibling-calls

시블링 함수와 테일 재귀 함수의 호출을 최적화한다.

-fcse-follow-jumps

공통 부분식 제거(common subexpression 이imination： 약자로 CSE) 시 점프
의 타겟이 다른 패스로는 닿을 수 없는 경우 공통 부분식 제거는 점프를 따
라 간다.

—fcse—skip—blocks

-fcse-follow-jumps와 비슷하지만 공통 부분식 제거(CSE)가 블록을 뛰어넘

는 점프 인스트럭션을 따라 간다.
-fgcse

전역 공통 부분식 제거(global common subexpression 이imination) 과정을
수행한다.

-fgcse-lm

전역 공통 부분식 제거 시 load 인스트럭션을 루프 밖으로 옮긴다.

-fexpensive-optimizations

비교적 비용이 비싼 몇 개의 최적화를 수행한다.

-fstrength-reduce

루프 내 연산 강도 경감과 반복 변수를 제거한다.

-frerun—cse—after—loop

루프 최적화를 수행한 후 공통 부분식 제거를 다시 수행한다.

-frerun-loop-opt

루프 최적화를 두 번 수행한다.

-fcaller-saves

함수 호출 시 변경되는 caller saved 레지스터의 값을 유지하는 것이 더 이득
일 때 함수 호출 인스트럭션 주위에 해당 레지스터의 값을 저장하고 복구하
는 인스트럭션을 삽입한다.

-fpeephole2

아키텍처 종속적인 핍홀(peephole) 최적화를 수행한다.

-fschedule-insns

인스트럭션 스케줄링을 수행한다. 인스트럭션 스케줄링은 인스트럭션의 수
행 순서를 바꿔서 지연(d이ay)을 최소화하기 위한 방법이다.

-fschedule-insns2

레지스터 할당이 끝난 후인스트럭션스케줄링을한 번 더 한다.

-fsched-interblock

베이직 블록들을 가로질러 인스트럭션 스케줄링을 수행한다. 일반적으로 인
스트럭션 스케줄링은 베이직 블록 내에서만 수행한다.

-fsched-spec

load가 아닌 인스트럭션들에 대해 speculative 이동을 수행한다.

-fregmove

레지스터를 최대한 사용하기 위해 레지스터 번호를 다시 매긴다.

—fstrict—게 iasing

엘리어싱 규칙을 최대한 엄격하게 한다.

-fdelete-null-pointer-checks

불필요한 null 포인터 체크를 제거한다.

-freorder-blocks

코드 지역성(locality)을 향상시키기 위해 베이직 블록들을 재정렬한다.

250 3부_ 컴파일과 링킹

===== PAGE 252 =====
옵션

설명

-freorder-functions

코드 지역성(locality)을 향상시키기 위해 함수들을 재정렬한다.

-falign-functions

함수의 시작 주소를 2의 거듭제곱으로 정렬한다.

-falign-jumps

분기 타겟의 주소를 2의 거듭제곱으로 정렬한다.

너 align 니 oops

루프의 시작 주소를 2의 거듭제곱으로 정렬한다.

—f게ign—labels

레이블 주소를 2의 거듭제곱으로 정렬한다.

-ftree-vrp

트리에서 값 범위 전파(Value Range Propagation) 과정을 수행한다.

-ftree-pre

트리에서 부분 중복성 제거(Partial Redundancy 티mination) 과정을 수행한다.

-02 옵션은 -이의 옵션에 위 옵션들이 더해진다. 때문에 -이보다 훨씬 많은 최적화
를 수행한다.
위 최적화 중에서 공통 부분식 제거 (Common Subexpression Elimination： 보통 줄
여서 CSE라 부름)라는 매우 유명한 최적화 알고리즘이 있는데, 공통 부분식 제거 알고
리즘은 다음과 같다.
〔예제 4-36) [ 공통 부분식 제거 예

1: x = a - b;
2: w = c + a - b;
3: y = c * d;
4: x = d +c

1:
2:
3:
4:
5:

tO = a
- b;
x = tO;
w = c + to;
y=c*
d;
x=d+
c;

좌측이 원본 코드일 때 a - b라는 식이 첫 번째 라인에서 사용되고 두 번째 라인에서도
사용되었다. 이렇게 공통된 부분식은 우측과 같은 형식으로 변경할 수 있다. 이렇게 되
면 원래 코드에서는 a-b 연산을 두 번 수행할 것을 한 번만 수행하면 된다. 이런 일을
수행하는 것을 공통 부분식 제거라 부른다.
우측의 공통 부분식 제거 과정이 끝난 코드에서 두 번째 라인의 x = tO 명 령은 다섯 번
째 라인에서 x 의 값이 다시 재정의되기 때문에 데드 코드 (dead code) 이므로 제거될
수 있다. 때문에 x = tO； 라인은 데드 코드 제거 (Dead Code Elimination) 과정에서 제
거될 것이다. 결국 공통 부분식 제거를 통해 a - b 연산이 하나 줄어든다.

-02 옵션을 주고 컴파일한 [예제 4-34] 코드의 결과는 다음 그림과 같다.

4장_ gcc compiler

251

===== PAGE 253 =====
［그림 4-46］ -02 옵션으로 컴파일한 후 사이즈와 실행 시간을 테스트

［그림 4-46］ 을 보면 -O1 옵션에서 실행 시간이 1.767초였던 것이 약간 단축된 것을
알 수 있을 것이다. 이건 필자의 경우에 그렇고 반드시 -02 옵션이 -O1 옵션보다 빠
르다고 이야기할 수 없다. 컴파일러의 최적화 과정은 매우 오묘해 같은 최적화 기법을
사용할지라도 어떤 순서로 적용하는지 또는 어떤 최적화와 어떤 최적화를 조합할지에
따라 결과가 상당히 차이가 날 수 있다.
때문에 -O1 옵션으로 컴파일한 결과가 -02 옵션으로 컴파일한 결과보다 더 빠를 수
있고, 마찬가지로 -02 옵션으로 컴파일한 결과가 -03 옵션으로 컴파일한 결과보다
더 빠를 수 있다. 이런 문제는 gcc에만 국한된 문제가 아니라 모든 컴파일러에서 공통
적으로 발생하는 문제다. 때문에 최적화를 많이 한다고 무조건 좋은 것이 아니라 어떤
특징을 갖는 프로그램에서 어떤 최적화를 어떻게 적절히 조합하는가가 최적화에 있어
중요하다. 이점에 유념하기 바란다.

-03
가장 높은 레벨의 최적화로 모든 최적화를 수행한다. -03 옵션을 사용하면 모든 함수
에 대해 인라인 함수가 아닐 경우에도 함수 자체의 크기가 그리 크지 않고 단순하다면
인라인 함수와 같이 취급해 인라인 확장을 한다. -03 옵션을 사용하면 -02 옵션의 최
적화를 모두 하면서 동시 에 다음과 같은 최 적화를 더 수행한다.
［표 4-5］ -03 옵션에서 추가되는 최적화 옵션
옵션

설명

-finline-functions

단순한 함수들을 그 함수를 호출한 함수에 인스트럭션으로 포함시킨다. 때문에 단순
한 함수를 호출하는 call 인스트럭션 자리에 해당 함수 자체의 인스트럭션이 붙는다.
이렇게 하면 바이너리 자체의 사이즈는 커지지만 함수를 호출하는 오버헤드가 줄기
때문에 프로그램 종류에 따라 많은 성능 향상을 기대할 수 있다.

-funswitch-loops

루프 내에 루프 불변의 조건들과 분기 명령들을 이동한다.

-fgcse-after-reload

reload 과정 후에 불필요한 로드 제거(redundant load 이imination) 과정을 수행한다.

252 3부— 컴파일과 링킹

===== PAGE 254 =====
다음은 -03 최적화 과정을 통해 생성된 결과다.
H root@os ：/temp/like2 ................

....................

[rootQos like2]tt gcc -03 -saue-temps -o test test.c
[root@os like2]tt is -al test
-rwxr-xr-x 1 root root[히히]2007-11-06 14:23 test
[root（흐os like2]tt
[root（흐os like2-]tt time ./test
END : 46180350 12
real 8nl.177s
user 0no.696s
pys
OmO.003s
[rootdos like2]tt |

[그림 4-47] -03 옵션으로 컴파일한 후 사이즈와 실행 시간을 테스트

보통 -03 옵션을 지정하면 단순한 함수들의 인라인 과정이 일어나 바이너리 사이즈가
커진다. 하지만 우리가 결과를 보기 위해 사용한 예제 소스의 경우 함수 호출이 많지
않기 때문에 오히려 사이즈가 줄어버렸다. 사이즈는 그렇지만 속도를 보면 가장 빠른
것을 확인할 수 있을 것이다.
하지만 반드시 -03가 -02보다 빨라진다는 보장은 없다. 대부분의 경우 -03 옵션에
서 성능이 향상되지만 경우에 따라 오히려 성능이 -02 옵션보다 감소할 수도 있다. 이
는 캐시와 관계된 문제로 바이너리 사이즈가 커져 캐시 미스가 많이 발생할 수도 있기
때문이다. 이런 점도 컴파일러 최적화의 오묘한 점이다.

사이즈 최적화를 수행한다. -02 옵션 중에서 사이즈를 늘리는 최적화만 제거하고 나
머지 최적화는 다 수행한다. -Os 옵션을 사용하면 -02 옵션에서 다음과 같은 옵션들
이 비활성화된다.
-falign-functions
-falign-jumps
-falign-loops
-falign-labels
-freorder-blocks
—freorder-blocks-and—partition
-fprefetch-loop-arrays
-ftree-vect-loop-version

다음은 -Os 옵션을 사용했을 때 결과 화면이다. -O를 사용한 최적화 중 가장 사이즈
가 줄어든 것을 확인할 수 있을 것이다. 임베디드 시스템 같이 공간이 협소한 곳에서
사용하는 프로그램을 작성할 때 자주 사용된다.

4장_ gcc compiler 253

===== PAGE 255 =====
【그림 4-48］ -Os 옵션= 컴파일한 후 사이즈와 실행 시간을 테스트

그런데 특이하게도 -02 옵션보다 최적화 종류가 줄었는데도 오히려 속도는 -02 옵션
보다 잘 나오는 것을 확인할 수 있다. 이것 또한 컴파일러 최적화의 오묘함 중 하나다.
이렇게 된 원인에는 최적화 옵션의 조합 때문일 수 있고, 사이즈가 작아짐으로 인해 캐
시 히트(hit)가 더 자주 발생했을 수 있기 때문이다.
실제 시뮬레이션을 돌려보면 바이너리 사이즈와 수행 속도 간에는 상당한 연관 관계가
있음을 알 수 있다. 이는 캐시 때문인데 바이너리 사이즈가 작으면 작을수록 캐시에 들
어가는 인스트럭션의 비율이 증가해 수행 속도가 향상될 수 있다.
어떤 아키텍처에서는 캐시의 영향으로 코드 사이즈가 30% 감소하면 성능이 30% 향상
되기도 한다. 그리고 ARM 아키텍처에서는 캐시를 끄고 프로그램을 돌렸을 때와 캐시를
켜고 프로그램을 돌렸을 때를 비교해 보면 캐시를 켰을 때 수행 성능이 10배 정도 향상
되기도 한다. 이렇게 최적화를 원하는 독자는 캐시의 영향도 어느 정도 알아야 한다.
지금까지 -O［최적화 레벨］ 옵션들이 어떤 옵션들의 묶음이고 해당 옵션들이 무슨 일
을 하는지 대략적으로 알아보았다. -O［최적화 레벨］ 옵션에 포함되는 최적화 옵션들
은 비교적 아키텍처와 소스 프로그램의 특성을 타지 않고 최적화하는 옵션들이다. 아직
실험적이거나, 아키텍처 종속적이거나, 소스 프로그램에 특성을 타는 최적화 옵션들은

-O［최적화 레벨］ 옵션에 포함되어 있지 않다. 그런 옵션들은 “gcc를 사용한 최적화 컴
파일” 절에서 알아본다.
► 디버깅 옵션
디버깅 옵션은 애플리케이션을 디버깅하기 위한 옵션과 GCC 컴파일러 자체를 디버깅
하기 위한 옵션으로 나눠진다.

254 3부_ 컴파일과링킹

===== PAGE 256 =====
-g
디버거에 제공하는 디버깅 정보를 바이너리에 삽입한다. 이런 디버깅 정보에는 대
표적으로 변수의 타입, 전역 심볼명과 주소, 소스 라인 정보 등이 있고 리눅스에서는

DWARF2라 부르는 디버깅 정보 포맷으로 되어 있다.
-g 옵션으로 바이너리를 컴파일하면 DWARF2 디버깅 포맷이 ELF 바이너리에 섹션
형태로 삽입된다. -g 옵션을 주고 컴파일한 like 바이너리를 readelf -a like 명령으
로 읽어 보았을 때 .debug_* 로 시작하는 섹션들이 DWW2 를 구성하는 섹션들이다.

DWARF2 포맷에 대한 좀 더 자세한 사항은 이후 과정에서 따로 설명한다.
이렇게 삽입된 디버깅 정보는 gdb 같은 디버거로 디버깅 시에 소스를 보면서 디버깅하
는 것이 가능하게 한다. -g 옵션을 주지 않고 컴파일한 바이너리를 gdb로 디버깅한다
면 역어셈해 어셈블리 코드로 디버깅할 수밖에 없다.
소스 정보가 삽입된다고 해서 실제 소스의 내용이 삽입되는 것은 아니다. 단지 어떤 인
스트럭션이 어떤 소스 파일의 몇 번째 라인에 해당한다는 정보만 삽입된다.

-g 옵션도 -O 옵션처럼 레벨이 있는데, -gO는 디버깅 정보를 삽입하지 않고 -g3는 디
버깅 정보를 가장 많이 삽입한다. -g는 기본적으로 -g2와 동일하다. ［그림 4-49］ 는 -g
옵션을 주어 컴파일한 바이너리를 objdump -S test 명령으로 디버깅 정보 중에서 라
인 정보를 이용해 인스트럭션을 소스와 함께 보여준 예다.

［그림 4-49］ -g 옵션으로 컴파일해 objdump -S test 명령으로 본 디버깅 심볼

4장_ gcc compiler 255

===== PAGE 257 =====
이런 -g 옵션으로 디버깅 심볼을 삽입한 바이너리는 용량이 매우 크기 때문에 개발 초
기에만 사용하고 개발이 끝나면 제거해야 한다.
그리고 디버깅을 위해 -g 옵션을 주고 컴파일할 때는 어떤 최적화도 하지 않는 것이 좋
다. 최적화한 바이너리로 디버깅하면 인스트럭션이 제거되거나 인스트럭션 스케줄링에
의해 인스트럭션의 순서가 바뀌어 버려 디버깅이 어려워지기 때문이다.

-pg
프로파일을 위한 코드를 삽입한다. 이런 프로파일 코드는 컴파일 과정에서 설명했듯이
중단부의 SSA 최적화 이전에 인터프로시저 분석(IPA) 과정에서 삽입된다. -pg 옵션을
사용해 컴파일한 프로그램이 종료하면 프로파일 정보가' gmon.out 파일에 저장된다.
이후 gprof로 gmon.out 파일의 내용을 분석해 어떤 함수가 얼마나 호출되 었고 시간은
얼마나 걸렸는지 확인할 수 있다. 그래서 병목 현상이 일어나는 부분과 어떤 부분을 코
드 최적화를 해야 될지 알 수 있다. 다음은 -pg 옵션을 주어 컴파일한 후 test 프로그램
을 수행하고 나서 gprof ./test 명 령으로 살펴본 프로파일 정보 내용 중 일부다.
64x14 -1 O| .시

I ® root@os：/temp/like2
index

아 time

self

[1]

100.0

O.OO
1.73
0.83

2.56
0.00
0.00

345/345
345/345

<spontaneous>
main [1]
func2 [2]
funci [3]

children

called

name

[2]

67.5

1.73
1.73

0.00
8.00

345/345
345

nain [1]
Func2 [2]

[3]

32.5

0.83
0.83

0.00
0.00

345/345
345

nain [1]
Funci [3]

11

스」

거

［그림 4-501 test 프로그램의 프로파일 정보

B as 의 옵션
gcc 는 as 의 옵션에 대해서는 그다지 잘 알지 못한다. 몇몇 as 옵션들이 Machine
Dependent Options에 포함되어 사용 가능하지만 다양하지는 않다. 그래서 as에 옵션
을 지정하려면 이전에 -Wp,［전처리 옵션들］ 형식으로 전처리기인 ccl -E에 gcc를 거
치지 않고 바로 전달했듯이 -Wa,［ as 옵션들］ 형식으로 gcc를 거치지 않고 바로 전달하
는 형식을 많이 사용한다.

►

-Wa,［ as 옵션들］

［ as 옵션들］에 들어가는 것은 진짜 as의 옵션들이다. 때문에 각 아키텍처의 어셈블러마
다 옵션들이 다를 수 있다. x86에서 유용한 as 옵션으로는 다음과 같은 것들이 있다.

256 3부_ 컴파일과 링킹

===== PAGE 258 =====
• -al： 어셈블된 인스트럭션을 보여준다.
• -as： 정의된 심볼을 보여준다.
• -I［패스］: include 디렉토리를 지정한다. 어셈블리 소스 내에서 사용된 .include
지정자가 지정하는 헤더 파일을 찾고자 할 때 사용한다.

• -W 또는 一no-warn： 경고 메시지를 출력하지 않는다.
• -march=［아키텍처 문자열］: 해당 어셈블리로 번역한다.
이러한 as 옵션들은 -Wa,-al,-as 와 같은 형식으로 사용하면 as 에 -al -as 옵션과 같이
전해진다.
同 collect2 또는 Id의 옵션

링커 옵션은 매우 중요하다. 자신이 작성한 프로그램은 링킹 오류가 잘 나지 않지만 다
른 사람이 작성한 프로그램을 컴파일하려 하면 링킹 오류가 의외로 자주 발생하기 때
문이다. 그리고 원하는 바이너리를 만들기 위해선 링커의 개념과 사용되는 옵션을 반드
시 명확하게 알아야만 시행착오를 겪지 않는다.

►

—1』라이브러리 디렉토리］

라이브러리를 찾을 디렉토리를 지정한다 . 기본적으로 라이브러리는 /usr/i386-redhat-

linux/lib, /usr/local/lib, /lib, /usr/lib 디렉토리에서 찾는데, 라이브러리의 위치가 다른
곳에 있다면 -L 옵션으로 따로 지정해야 한다. 예를 들면 like.c 파일 내부에서 /opt/lib/

libl&e.a 파일에 있는 루틴을 사용했다면 컴파일 시 다음과 같이 해야 한다.
gcc -o like like. c -L/opt/lib -Hike

► 니［라이브러리 이름］
같이 링크할 라이브러리를 지정한다. 이전에도 설명했듯이 라이브러리의 이름은 앞에
오는 lib를 떼어버리고 확장자 이전까지가 라이브러리명이다. 그래서 libc.*의 경우 c가
라이브러리명이고, liblike.*의 경우 like가 라이브러리명이다. 다른 옵션들은 컴파일 명
령에서 소스 파일의 앞에 오나 뒤에 오나 상관이 없지만 꼭 -1 옵션만은 소스 파일의 뒤
에 와야 한다. 특히 main() 함수가 있는 파일보다는 무조건 뒤에 와야 한다.
라이브러리를 main() 함수보다 앞에 링크하면 undefined 참조 오류가 발생한다. 이는
링커가 아카이브를 찾는 데 있어 항상 main() 함수 뒤에서 탐색하기 때문에 이런 문제
가 발생한다.

4장_ gcc compiler

257

===== PAGE 259 =====
그리고 lex(fl 예)의 라이브러리 (libfLa) 같이 main() 함수가 라이브러리 내에 포함되
어 있는 라이브러리에서 예기치 못한 결과가 나올 수 있기도 하다. libfl.a 라이브러리를
사용해 컴파일하는 경우 아래와 같이 -1 옵션을 소스 파일보다 앞에 두면 실행 시 소스
의 main() 함수가 실행되는 것이 아니라 Hbfl.a 라이브러리에 있는 main() 함수가 실
행되어 버린다.
gcc -lfl -o like like. c

반드시 -1 옵션은 소스 뒤에 붙이도록 하자.

►

-shared

공유 라이브러리와 정적 라이브러리가 같이 있을 경우 공유 라이브러리를 우선 링크한
다. 기본적으로 아무 옵션을 주지 않아도 공유 라이브러리를 우선 링크한다.

►

-static

정적 라이브러리와 공유 라이브러리가 같이 있다면 정적 라이브러리를 우선 링크한다. 정
적 라이브러리와 공유 라이브러리의 사용은 각기 장단점이 있다. 먼저 정적 라이브러리를
사용해 링크하면 파일의 사이#} 매우 커진다. ［그림 4-51］ 은 같은 소스 파일을 하나는
정적 라이브러리를 사용해 링크하고, 하나는 공유 라이브러리를 사용해 링크한 예다.
[혀 mot@os：/temp/like2
[root@os like2]S gcc -static -o like.static like.c
[rooteos like2]tt gcc -shared -o like.shared like.c
[rooteos like2]S
[rootQos like2]tt Is -al like.static like.shared
—rwxr-xr-x 1 root root
-rwxr-xr-x 1 root root
[root@os like2]# |

64x9 -!□! x|
■■■■싀

411612007-11-06 16:03 like.shared
537682|2087-11—86 16:03 like.static

□
［그림 4-51］ 파일 사이즈 비교

［그림 4-51］ 에서 보듯이 정적 라이브러리로 링크한 파일이 크기가 확연히 큰 것을 알
수 있다. 사이즈는 크지만 정적 라이브러리로 컴파일한 바이너리는 수행 속도가 약간
빠르고, 같은 아키텍처라면 어디에서나 대부분 실행될 수 있다.
반면 공유 라이브러리는, 사이즈는 작지만 속도가 약간(매우 약간) 느리고, 컴파일한
바이너리를 다른 컴퓨터에서 실행하려 할 때 컴파일할 당시의 공유 라이브러리와 메이
저 버전이 같은 공유 라이브러리가 시스템에 있어야만 실행할 수 있다. 그래서 공유 라
이브러리로 컴파일한 바이너리를 배포할 때는 컴파일할 때 사용한 공유 라이브러리도
함께 배포하는 것이 좋다. 이런 장단점을 알고 공유 라이브러리와 링크할 것인지 정적
라이브러리와 링크할 것인지 결정해야 한다.

258 3부_ 컴파일과링킹

===== PAGE 260 =====
►

-nostdlib

링크 시에 표준 C 라이브러리를 사용하지 않는다. 운영체제나 부트로더, 디바이스 드라
이버 같이 표준 c 라이브러 리를 사용하지 않는 프로그램을 컴파일할 때 사용한다.

►

-nostartfiles

crtl.o, crti.o, ctrbegin.o, crtend.o, crtn.o 등과 같은 crt 오브젝트 파일들을 링크하지
않는다. 역시 운영체제, 부트로더 같은 프로그램을 컴파일할 때 사용한다.

►
-

-WI, ［링커 옵션들］, -Xlinker ［ f링커 옵션］
W1 옵션은 gcc를 거치지 않고 바로 링커에 옵션을 전하려 할 때 사용한다.
$ gcc -o like like.c —Wl,—M,-s

위와 같이 명령을 내리면 collect》에 -M -s 옵션이 전달된다. 이후 collect』는 링커인

Id를 -M -s 옵션으로 호출한다. -Xlinker 옵션은 gcc가 인식하지 못하는 특정 링커에
대해 옵션을 지정할 때 사용한다.
$ gcc -o like like.c -Xlinker -M -Xlinker -s

위와 같이 명령을 내리면 역시 collect》에 -M -s 옵션이 전달되고 진짜 링커인 Id 호출
시 -M -s 옵션으로 Id가 호출된다.
다음은 -W1 옵션과 -Xlinker 옵션에서 사용 가능한 유용한 링커 옵션들이다.

• -s： 실행 파일에서 심볼 테이블 제거
• -x： 출력 파일에 로컬 심볼 제거
• -e［ name］ ： 시작 심볼을 name 심볼로 사용한다. gcc -Wl,-emain -o like like,
c 명령을 내리면 시작 심볼로 main 심볼을 사용한다. 기본적으로 시작 심볼은
_start 심볼이다.
• -M： 링커 스크립트와 메모리 맵을 자세하게 출력한다. 때문에 프로그램의 메모리
구조를 자세하게 알 수 있다. 링커 스크립트는 시스템 프로그래밍에 있어 중요한
부분이므로 링커 장에서 따로 자세히 설명 한다.
이제 gcc에 대한 모든 설명이 끝났다. 정말 수고 많았다. 지금까지 gcc 컴파일러를 사
용할 때 필요한 모든 중요 옵션을 거의 다 알아보았다. 이것들만 알아도 당장 프로그래
밍하는 데 아무런 문제가 없고, 앞으로도 문제가 없을 것이다. 그리고 이것들을 다 알고
있는 사람도 흔치 않다.

4장_ gcc compiler 259

===== PAGE 261 =====
지금부터 설명하는 것은 필자가 덤으로 남기는 것이다. 덤이니깐 가벼운 마음으로 읽
고, 갈 길이 급한 독자는 바로 다음 장인 “linker” 장으로 넘어가면 된다. 앞으로 설명하
는 것들은 유닉스 리눅스 프로그래밍에 익숙해졌을 때 gcc에 대해 좀 더 잘 알고 싶다
면 그때 보아도 늦지 않다.

04L gcc를 이용한 최적화 컴파일
이번 절에서는 -O［최적화 레벨］에 포함되지 않은 최적화 기법들을 설명한다. -O［최적
화 레벨］ 옵션으로 설정되는 최적화 옵션들은 아키텍처의 특성을 타지 않고 비교적 소
스 프로그램의 특성도 타지 않는 최적화들이다. 사용자가 아키텍처의 특성과 소스 프로
그램의 특성을 잘 이해하고 있다면 gcc에서 지원하는 -O［최적화 레벨］ 옵션에 포함되
지 않은 최적화 옵션들을 사용해 좀 더 성능을 향상시킬 수 있다.
하지만 이번 절을 시작하는 시점에서 필자는 하고 싶은 말이 있다. 그것은 바로 어설
픈 최적화는 안 하느니만 못하다는 점이다. 아키텍처의 특성, 소스 프로그램의 특성, 최
적화의 영향에 대해 정확하게 이해하지 못한다면 -O［최적화 레벨］ 옵션으로 만족하기
바란다. -03 옵션만 사용해도 정말 많은 최적화를 수행하기 때문에 충분히 최적화된
코드로 컴파일할 수 있다.
지금부터 설명하는 최적화 옵션들은 필자가 비교적 안전한 최적화 옵션들만 골라 설명
하겠지만 경우에 따라서는 최적화되고 안 되고의 문제를 떠나 프로그램 수행에 중대한
문제를 일으킬 수도 있다.
프로그램에서 가장 중요한 것은 프로그램이 얼마나 빨리 수행되는지가 아니라 프로그
램이 얼마나 정확하게 수행되느냐다. 조금 빠르게 한다고 해서 프로그램이 오작동을 일
으키게 하는 것만큼 우매한 일도 없다. 그러니 이점을 분명히 명심하기 바란다.

| 머신 종속적인 옵션을 이용한 최적화
이전에 gcc 옵션 분류에서 머신 종속적인 옵션을 간단히 설명하였다. 머신 종속적인
옵션이란 아키텍처 특성에 따라, 그리고 프로세서 종류에 따라 코드 생성을 달리 할 때
사용하는 옵션이라고 설명했다. 이런 머신 종속적인 옵션을 사용하면 프로세서에 좀 더
최적화된 인스트럭션을 사용해 바이너리를 생성할 수 있다.
260 3부- 컴파일과링킹

===== PAGE 262 =====
O -march=cpu—type —mtune=cpu—type —mcpu=cpu—type
-march 옵션은 cpu-type 으로 지정하는 프로세서의 인스트럭션 셋으로 구성된 코드
를 생성한다. 그리고 약간 의미가 다르게 -mtune 과 - mcpu 는 cpu-type 에 좀 더 최적
화된 코드를 생성한다. 그 말이 그 말 같다는 생각이 들 것이다. 간단히 예를 들면 다음
과 같다.

x86 바이너리를 컴파일할 때 -march=pentium4 옵션을 주면 펜티 엄 4 에서 지원하는
인스트럭션 셋으로 구성된 코드를 생성한다. 그래서 MMX, SSE, SSE2의 인스트럭션들
을 사용할 수 있다. 때문에 MMX, SSE, SSE2 인스트럭션을 지원하지 않는 오래된 펜티
엄에서는 -march=pentium4 옵션을 주고 컴파일한 코드가 동작하지 않을 수 있다.

-mtune 옵션은 인스트럭션을 스케줄링하거나 정렬할 때 -mtune 옵션으로 지정해 준
CPU에 최적화되게 스케줄링하고 정렬한다. 이때 고려되는 것에는 각 CPU의 파이프라
인 단계와 각 인스트럭션을 수행하는 데 걸리는 사이클, 버스와 캐시의 크기 등이 있다.
쉽게 예를 들면 펜티엄 3는 파이프라인 단계가 10단계이고 펜티엄 4는 파이프라인 단
계가 20단계인데, CPU 내부의 멈춤(stall)을 줄이기 위해 인스트럭션의 순서를 섞을 때

-mtune 옵션으로 지정한 CPU에 최적화되게 인스트럭션을 섞는다.
인스트럭션 스케줄링 이 란 CPU 내부의 특정 자원이 사용 가능하지 않아 CPU가 멈추는

(stall) 것을 줄이기 위해 인스트럭션 수행 순서를 바꾸는 것을 말한다.
그리고 인스트럭션 정렬이란 함수나 레이블이 시작하는 주소를 해당 CPU의 버스 너비
와 캐시의 크기에 최적화되게 맞추는 것을 말한다.

-mtune 옵션은 이런 CPU 의 특성을 반영해 최적화된 코드를 생성하는 역할만 담
당한다. 따라서 -mtune 옵션이 인스트럭션 셋에 영향을 주는 것은 아니기 때문에

-mtune=pentium4 옵션으로 컴파일했더라도 i386 인스트럭션 셋을 사용했다면 오래
된 펜티 엄에서도 동작하는 코드를 생성할 수 있다. 마찬가지로 -mtune=athlon-xp 옵
션으로 컴파일했다고 해서 펜티엄에서 동작하지 않는 것도 아니다. 단지 펜티엄에서 좀
비효율적 이 게 될 뿐이다. -mcpu는 -mtune과 거의 동일하다.

-march 옵션은 -mtune 옵션을 내부적으로 포함한다. 때문에 -march=pentium4 옵
션을 줬다면 굳이 -mtune=pentium4 를 명시하지 않아도 -mtune=pentium4< 같이
준 것과 동일한 결과를 얻을 수 있다. 물론 -march 와 -mtune 의 cpu-type 을 다르게
지정할 수도 있다. 그렇게 되면 생성되는 코드의 인스트럭션 셋은 -march에서 지정된

4장_ gcc compiler

261

===== PAGE 263 =====
cpu-type 이 사용되고, 스케줄링과 코드 정렬은 -mtune 에 지정된 cpu-type 으로 최적
화된다. 그리고 -march 옵션은 주지 않고 -mtune 옵션만 주어 인스트럭션 셋은 모든

x86 아키텍처에 공통된 것을 사용하게 하고, 스케줄링과 코드 정렬만 특정 프로세서에
최적화할 수도 있다.
결론적으로 -march 옵션과 -mtune 옵션을 사용하면 특정 프로세서에 최 적화된 코드
를 생성할 수 있다. 물론 이때는 그 프로그램이 다른 프로세서에서 사용될지 여부는 심
각하게 고민해야 한다.
다음은 like.c 파일을 -mtune 옵션만 달리하고 컴파일한 모습이다.
84x8 J디 시

H root@os：/temp/like2
like2]tt
[rootSos
like2]tt
[root@os
like2]tt
[rootOos
like2]tt
[rootQos
like2]tt
[rootQos
like2]tt
[root@os
[root（흐 os like2]tt
[root（흐 os like2]tt

gcc ~o like like.c ~Q2

j삐;;";

mu like.s like.s.pentiunU
gcc -o like like.c -02 -saue-tenps -march=pentimi4|-ntune=athlon-헤
mu like.s like.s.athlon-xp

[그림 4-52] —mtune=penth」m4와 —mtune=athlon—xp 컴파일 모습

이때 ［그림 4-52］ 에서 생성되는 like.s 파일을 vimdiff like.s.pentium4 like.s.athlon-

xp 명령으로 비교하면 결과는 다음과 같다.

[그림 4-53] —mt니ne=pentium4와 -mtune=athlon-xp 컴파일 결과

262 3부— 컴파일과 링킹

===== PAGE 264 =====
인스트럭션의 위치와 코드 정렬 부분이 서로 다른 것을 확인할 수 있을 것이다. popl과

leave 인스트럭션 같은 경우 얼핏 보기에는 인스트럭션 종류도 다른 것 같은데, 둘 다
펜티엄 4에서 지원하는 인스트럭션이기 때문에 인스트럭션 셋이 다르지는 않다.
［표 4-6］ 은 -march 와 -mtune 옵션에 지정할 수 있는 CPU 종류에 따라 사용할 수
있는 cpu-type 문자열들이다.
[표 4-6] x86 아키텍처 一march, -mtune, —mcpu의 cpu-type 종류
cpu-type

CPU 종류

generic

IA32/AMD64/EM64T

| 설명

현재는 i686 프로세서를 의미, -mtune, —mcp니
에서만 사용가능

i386

i386 DX/SX/CX/EX/SL

오래된 i386 프로세서

i486

i486 DX/SX/DX2/SL/SX2/DX4

오래된 i486 프로세서

i586, Pentium

pentium

MMX를 지원하지 않는 오래된 펜티엄

pentium-mmx

PentiumMMX

MMX 지원 펜티엄

pentiumpro

PentiumPro

펜티엄 프로

i686

모든 i686 familly

모든 i686 familly

pentium2

Pentium II, Celeron

MMX 지원 펜티엄프로

pentium3, pentium3m

Pentium III, Pentium HIM

MMX, SSE 지원 펜티엄프로

pentium-m

Pentium M

펜티엄 3 CPU의 저전력 버전

pentium4, pentium4m

Pentium 4, Pemtium 4M

MMX, SSE, SSE2 지원 펜티엄 4

prescott

Pentium 4 Prescott

MMX, SSE, SSE2, SSE3 지원 펜티엄 4

nocona

Penti니m 4 Xeon, Nocona

MMX, SSE, SSE2, SSE3, 64Bit 지원 펜티엄 4

core2

Core2 Duo

MMX, SSE, SSE2, SSE3, 64Bit,

코어2 지원 펜티엄 4
k6

AMDK6

MMX 지원 K6

k6—2, k6-3

AMD K6 11, AMD K6 III

MMX, 3dN0W! 지원 K6

athlon, athlon-tbird

AMD Athlon, AMD Tbird

MMX, 3clMOWL enhanced 3dMOW!,
SSE prefetch 인스트럭션 지원 Athlon

athlon-4

AMD Athlon 4

MMX, 3dNOW!, enhanced 3dNOW!,

athlon-xp

AMD Athlon XP

모든 SSE 인스트럭션 지원 Athlon

athlon-mp

AMD Athlon MP

k8, opteron,

AMD K8, AMD Opteron,

MMX, SSE, SSE2, 3dN0W!,

athlon64, athlon-fx

AMD Athlon 64, AMD Athlon FX

enhanced 3dNOW!, 64-bit x|원 K8

amdfamlO

AMD Family 10 core CPUs

MMX, SSE, SSE2, SSE3, SSE4A,
3dN0W!, enhanced 3dNOW!,
ABM, 64-bit 지원 AMD Family 10

winchip-c6

IDT Winchip C6

MMX 지원 C6

winchip2

IDT Winchip2

MMX, 3dNOW! 지원

c3

ViaC3

MMX. 3dN0W! 지원 C3

c3-2

Via C3-2

MMX, SSE 지원 C3-2

4장_ gcc compiler 263

===== PAGE 265 =====
x86 아•키텍처에서 一march와 -mtune, -mcpu에서 지정할 수 있는 cpu-type은
generic만 제외하고 동일하다. generic은 -march에서 사용할 수 없다. -march는 인
스트럭션 셋을 지정하는데 각각의 CPU 종류마다 지원하는 인스트럭션이 다르기 때문
이다. generic은 현재 가장 보편적인 프로세서를 의미하고 현재 우리가 사용하는 gcc-

4.1.2는 i686으로지정되어 있다.
다음은 ARM 프로세서에서 -march에 지정 가능한 ARM 아키텍처 타입명들이다.
armv2,
armv2a,
armv3,
armv3m,
armv5tez armv6, armv6j, iwmmxt, ep9312

armv4,

armv4t,

armv5,

armv5tz

ARM에서는 인스트럭션 셋을 버전별로 정의해 놓았기 때문에 위 인스트럭션 셋 이름을
사용해 지정하면 된다.
다음은 ARM에서 -mtune, -mcpu 옵션에 지정할 수 있는 프로세서 타입명들이다.
arm2,
arm250z
arm3,
arm6z
arm60z
arm600,
arm610,
arm620,
arm7,
arm7m,
arm7d,
arm7clm,
arm7cii,
arm7dmi,
arm70,
arm700,
arm700i,
arm710,
arm710c,
arm7100,
arm7500,
arm7500fe,
arm7tdini,
arm7tdini-s,
arm8,
strongarm,
strongarmllO,
strongarmllOO,
arm8,
arm810,
arm9,
arm9e,
arm920,
arm920t,
arm922t,
arm946e-s,
arm966e-s,
arm968e-sz
arm926ej-sz
arm940tz
arm9tdmi,
armlOtdmi,
arml020t,
arml026ej-s,
armlOe,
arml020e,
arml022e,
armll36j-sz
armll36jf-s,
mpcore,
mpcorenovfp, armll76jz-s, armll76jzf-s, xscale, iwmmxt, ep9312

위 리스트에서 자신이 사용하는 ARM 프로세서에 맞는 아키텍처 타입과 프로세서 타입
을 각각 -march 옵션과 -mtune, -mcpu 옵션에 지정하면 해당 프로세서에 최적화된
코드를 생성할 수 있다.

-m으로 시작하는 머신 종속적인 옵션에는 최적화에 도움이 될 만한 옵션들이 아직도
많은데, 그 중에서 기본 중에 기본이라 할 수 있는 -march, -mtune, -mcpu 옵션만
설명하고 마치도록 한다. 다른 ARM과 x86 아키텍처의 다른 머신 종속적인 옵션들이
궁금한 독자는 부록을 보기 바란다. 머신 종속적인 옵션들에는 3D, 코덱 프로그램 같은

DSP 프로그램의 연산에 사용하면 극도의 성능 향상을 경험할 수 있는 최적화 옵션이
많이 있기 때문에 DSP 프로그래밍을 하는 독자라면 한 번쯤 꼭 봐두길 권장한다.
마지막으로 알아야 될 점은 이런 머신 종속적인 옵션들은 다른 타겟 아키텍처의 인스
트럭션을 생성하는 gcc 에서는 지원이 안 된다는 점이다. 예를 들면 -mthumb 옵션은

ARM을 타겟으로 하는 gcc에서만 유효하고 다른 타겟 아키텍처의 gcc에는 없는 옵션

264 3부- 컴파일과링킹

===== PAGE 266 =====
이다. 때문에 여러 아키텍처에서 컴파일 가능한 프로젝트를 만들고자 할 때는 이런 머
신 종속적인 옵션들도 고민해야 한다.

I 프로파일 결과를 이용한 최적화
프로파일 결과를 이용한 최적화는 간단하게 말해 컴파일한 프로그램을 한 번 수행해
프로그램의 동작 특성을 파악하고, 그 정보를 바탕으로 다시 컴파일하면서 좀 더 최적
화하는 기법을 말한다. like.c 파일을 예로 들어 프로파일 결과를 이용한 컴파일 절차는
다음과 같다.

1. like.c 파일을 -fprofile-generate 옵션을 주어 컴파일한다. 그러면 생성되는 like
바이너리 에 프로파일 정보를 출력하는 코드가 추가되어 컴 파일된다.
예） gcc -02 -o like like.c -fprofile-generate

2. like 프로그램을 그냥 한 번 수행한다. 이렇게 수행하면 추가된 프로파일 코드에
의해 프로파일 결과가 들어 있는 파일들（ like.gcda, like.gcno） 이 현재 디 렉토리에
생성된다.
예） ./like

3. 1번에서 사용한 컴파일 옵션 그대로에서 -fprofile-generate 옵션을 빼고
-fprofile-use 옵션을 추가해 like.c를 다시 컴파일한다. 이렇게 하면 gcc는 like
프로그램이 수행될 때 수집한 정보를 바탕으로 좀 더 최적화해 like 바이너리를 생
성한다.
예） gcc -02 -o like like.c -fprofile-use
프로파일 정보를 이용한 최적화 방법은 일반 애플리케이션을 작성하는 사람에게는 생
소하겠지만 3D 그래픽, 코덱, RF 통신과 같이 극도의 성능을 요구하는 프로그래밍을
하는 사람들에게는 매우 친숙한 방법이다. 이런 프로그래밍에서는 프로그래밍의 편의
보다는 모자란 CPU 자원을 좀 더 효율적으로 사용하기 위해 두 번 컴파일하는 수고도
마다하지 않는다.

-fprofile-use 옵션은 프로파일 정보를 이용해 할 수 있는 모든 최적화를 수행하는데,
-fprofile-use 옵션에 의해 선택되는 최적화 옵션은 다음과 같다.

4장_ gcc compiler 265

===== PAGE 267 =====
-fbranch-probabilities
-funroll-loops
-fpee丄一loops
-ftracer
-fvpt

그러면 각각의 옵션이 어떤 의미를 지니는지 알아보자.

Q -fbranch-probabilities 옵션을 이용한 분기 최적화
분기 최적화란 상태에 따른 분기문이 있을 때 프로그램이 주로 어떤 쪽으로 분기하는
지를 파악하고 이를 바탕으로 파이프라인이 최대한 깨지지 않게 코드를 생성하는 것을
말한다.
이를 설명하려면 파이프라인의 개념을 알아야 된다. 혹시 모르는 사람을 위해 먼저 파
이프라인의 개념을 간단히 알아보■자.
단계
시간

L1：
MOV r1, r2
ADD r1, #1
CMP r1, #2
B
JLE L1
Dr1,
r3,
Dr5,
r3.
.
B

브랜치가 일어나지
丄 않는경우 으

브랜치가
)
丄 일어나는 경우_』

［그림 4-54］ 파이프라인 과정

현대의 거의 모든 프로세서는 클록 주파수를 높임과 동시에 프로세서 사용률을 높이기
위한 파이프라인 구조를 가지고 있는데, ［그림 4-54］ 와 같다. 그림은 5단계 파이프라인
을 가지고 있는 ARM9 같은 프로세서에서 인스트럭션이 파이프라인을 통해 처리되는
과정을 나타낸다. IF, ID 단계는 전처리 과정이고, EX 단계에서 인스트럭션이 실제로
수행된다.

266 =_ 컴파일과 링킹

===== PAGE 268 =====
시간 단위는 ARM 같은 RISC CPU에서는 1 클록을 의미한다. 그래서 위 그림과 같은
인스트럭션들이 있을 때 최초 1번째 클록에서는 MOV rl, r2가 IF 단계로 가고, 2번째
클록에서는 ADD rl, #1 이 IF 단계로 가고, MOV rl, r2가 ID 단계로 간다.
이렇게 파이프라인이 채워지면서 인스트럭션이 수행된다. 그런데 JLE와 같은 브랜치
인스트럭션이 EX 단계에 오면 상태에 따라 브랜치가 일어날 수도 있고 일어나지 않을
수도 있다. JLE는 Jump Less Equal의 약자이므로 위 인스트럭션에서는 rl이 2보다 작
으면 브랜치가 일어난다.
실제로 브랜치가 안 일어난다면 1번과 같이 그냥 계속 순차적으로 진행하면 된다. 그러
나 브랜치가 되면 JLE 인스트럭션 뒤에 파이프라인을 채우고 있는 인스트럭션들은 의
미가 없어져 버린다. 그래서 파이프라인을 비우고 새로운 브랜치 타겟의 인스트럭션을
받아와야 한다. 위 그림에서는 L1 레이블에 있는 인스트럭션이 브랜치 타겟 인스트럭
션이다. 결국 브랜치가 되면 2번과 같은 상황이 되어 2 사이클이 낭비된다.
이런 파이프라인과 브랜치와의 관계를 실제 소스로 살펴보면 다음과 같다.

〔예제 4-37)test.c 코드 내용
#include <stdio.h>
void big () {
printf("big!\n");
}

|

void small() {
printf("small!\n");

}

；

int main(int argc, char **argv)
{
int i, j;

|

for (i=0; i < 3; i++) {
printf ("input : ’’) ;
scanf("%d”, &j);
if (j > 5) {
big() ;
} els은 {
small();
}
}
return
}

：

0;

;
!

4장_ gcc compiler 267

===== PAGE 269 =====
[예제 4-37] 코드는 루프를 3번 돌면서 매번 j 값을 사용자에게서 입 력받아 그 값이 5보
다 크면 big() 함수를 호출하고, 그렇지 않으면 smalK) 함수를 호출한다. 이럴 경우 두
가지 모양의 어셈블리 코드가 생성될 수 있는데, 그 형태는 다음 그림과 같다.

(a) j 값이 5보다 클 때 브랜치

(b) j 값이 5보다 작거나 같을 때 브랜치

[그림 4-55] 생성되는 어셈블리 코드 모양

하나는 j 값이 5보다 클 때 브랜치하고, 다른 하나는 j 값이 5보다 작거나 같을 때 브랜
치한다. 위 소스 코드에서 j 값은 사용자 입력으로 받기 때문에 제어 흐름 그래프 분석
만으로는 gcc가 어떤 모양이 좋을지 결정할 수 있는 정보가 아무것도 없다. 보통 이런
경우 gcc 는 비교문의 값이 참인 경우에 브랜치하지 않게 (b)와 같은 모양으로 코드를
생성한다.
입력 값이 주로 5보다 작거나 같은 값이 계속 들어온다면 (a)와 같은 모양의 구조가 브
랜치 횟수가 적어 (b) 모양보다 훨씬 이득일 것이다. 반대로 5보다 큰 값이 계속 입력
된다면 (b)와 같은 모양이 (a)보다 훨씬 이득일 것이다.

-fbranch-probabilities 옵션은 프로파일링 정보 중에서 브랜치되는 정보를 이용해
(a)와 같은 모양으로 코드를 생성하는 것이 이득인지 (b)와 같은 모양으로 코드를 생성
하는 것이 이득인지를 결정할 수 있게 해준다.

test.c 코드를 -fbranch-probabilities 옵션을 사용해 최적화하려면 다음과 같이 한다.
먼저 test.c 를 -fprofile-arcs 옵션 또는 -fprofile-generate (내부적으로 -fprofile-

arcs 옵션이 포함되어 있다) 옵션을 사용해 컴파일한다.
$ gcc -o test test.c -02 -save-temps -fprofile-generate

268 3부— 컴파일과 링킹

===== PAGE 270 =====
-이최적화 레벨］ 옵션은 반드시 붙이기 바란다. -fbranch-probabilities 옵션은

-fprofile-arcs 옵션으로 추가한 프로파일 정보를 이용한다. -fprofile-generate 옵션
에는 -fprofile-arcs, -fprofile-val니es, -fvpt 옵션들이 포함된다.
그러면 test 바이너리가 생성될 것이다. test 바이너리를 실행해 아무 값이나 입력한다.
$ ./test
input : <==== 아무값이나입력

like 바이너리 수행이 끝나면 프로파일 정보가‘ 담긴 test.gcda, test.gcno 두 개의 파일
이 생성된다. 구 버전 gcc에서는 test.da, test.no 파일이 생성될 것이다.
프로파일 정보가 담긴 파일이 생성되었으면 이전 옵션에서 -fprofile-generate 옵
션을 빼고 -fbranch-probabilities 옵션 또는 一fprofile—니seC내부적>으^ -fbranch-

probabilities 옵션이 포함되어 있다） 옵션을 사용해 재컴파일한다.
$ gcc -o test test.c -02 -save-temps -fbranch-probabiliti은s

이렇게 하면 gcc는 test 바이너리가 수행되면서 수집한 프로파일 정보를 이용해 제어
흐름을 최적화해 새로운 test 바이너리를 생성한다. 다음은 실제 수행 결과다.
W root@os ：/temp/test3

---------------------------------------------—=—三...—으三—======%=^^^쫴뗴1^나파■메네^^루

■■■KB

[rootQos test3]tt gcc -o test test.c -02 -save-tenps|-fpFbfile-generate]
[root@os \est3]tt ./test
input : 1
small!
input : 1
small?
input : 1
small?------------------------------------------------------------------------------------------------------ ________ _____________
[root(흐os test3]tt gcc -o test teyt.c -02 -saue.-temps |-fbrancK三'probAETiTEn?]
[root(흐os test3]M 'cp' -F test.s [Fest.s.small |
[rootQos test3]tt
[rootQos test3]#
[root@os test3]U gcc -o test test.c -02 -saue-tenps|-Fprofile-generate[
[rootQos test3]# ./test
input : 9
big?
input : 9
big?
input : 9
big?
[root(흐os test3]tt gcc -o [est test.c ~02 -saye—tenps |-，Ft；ranch：：pj'6t)a611ities |
[root@os test3]tt 'cp' -F|test'.s test.s.61'프"]
[rootQos test3]tt
[rootQos test3]tt |

［그림 4-56］ 프로파일 정보를 이용해 분기 최적화

필자는 처음에는 1만 입력해 프로파일을 생성하고, 재컴파일 시 중간 어셈블리 파일을

test.s.small로 만들었고, 다른 하나는 9만 입 력하고 재컴파일 시 중간 파일을 test.s.big
로 만들었다. 아래는 두 파일의 결과를 나타낸다.

4 장_ gcc compiler 269

===== PAGE 271 =====
〔예제 4-38)

1만 입력했을 때와 9만 입력했을 때 재컴파일 결과

test.s.small

test.s.big

.••상략

... 상략

.L6:

.L6:
movl
call
movl
movl
call scanf
cmpl
jg .L15
call

$.LC2, (%esp)
printf
%esi, 4 (%esp)
$.LC3, (%esp)

movl
call
movl
movl
call
cmpl
jle .L7
call

$5, -16(%ebp)
small

.L9:
addl
$1, %ebx
cmpl
$3, %ebx
,p2align 4,z 2
jne .L6
movl
-12 (%ebp), %ecx
xorl
%eax, %eax
movl
-8(%ebp), %ebx
movl
-4(%ebp), %esi
movl
%ebp, %esp
popl
응ebp
lea丄
一4(%ecx), 응esp
ret
.L15:
call
big
jmp .L9
... 하략

$.LC2, (%esp)
printf
%esi, 4 (%esp)
$.LC3, (%esp)
scanf
$5, -16(%ebp)
big

.L9:
addl
$1, %ebx
cmpl
$3, 응ebx
.p2align 4,,2
jne .L6
addl
$28, %esp
xorl
%eax, %eax
popl
%ecx
popl
%ebx
popl
%esi
popl
%ebp
leal
-4 (%ecx),
응esp
ret
.L7:
call
jmp .L9

small

... 하략

각각이 필자가 말한 대로 최적화된 것을 확인할 수 있을 것이다.
이런 브랜치 정보는__builtin_expect() 빌트인 함수를 사용해 프로그래머가 명시적으
로 gcc에 알려줄 수도 있다. if (__builtin_expect(a〈O, 1)) { AAA } else { BBB }와 같
은 문장이 있을 때 __builtin_expect() 함수의 첫 번째 인자로 사용된 a<0 비교문은 두
번째 인자로 사용된 1의 값을 가질 가능성이 크다고 gcc에 명시적으로 힌트를 준다. 이
렇게 힌트를 주면 gcc는 true에 해당하는 AAA 코드를 수행할 때 파이프라인이 안 깨
지 게 코드를 배치 한다.
이제 프로파일 정보를 이용한 최적화가 대충 어떤 것인지 알았을 테니 -fprofile-use
옵션을 사용했을 때 켜지는 나머지 최적화는 다소 간단하게 넘어가자.

270 3부- 컴파일과링킹

===== PAGE 272 =====
ARM과 같은 크로스 컴파일 환경쓰는 프로파일 정보를 어떻게 수집할까?
두 가지 방법이 있다. 시뮬레이터를 사용하거나, ARM 보드상에서 직접 수행하는 방법이 있을 수 있다.
여기서는 테스트 목적으로 시뮬레이터를 사용하는 방법만 간단히 설명한다. ARM 시뮬레이터에는 여러
종류가 있지만 간단하게 사용할 수 있는 Simit-ARM 시뮬레이터를 사용해 프로파일 정보를 수집하는
절차만 알아보자.

1. http://simit-arm.so니rceforge.net/에서 simit-arm release 3.0 버전을 받아 설치한다.
2. http://www.falinux.com/zdownload/toolchain.php에서 arm—toolchain—3.3.4.tar.gz 파■일
을 받아 ARM 크로스 컴파일러를 설치한다(버전이 3.3.4임에 주의).
3. 소스 파일을 arm-linux-gcc 컴파일러로 컴파일할 때 -02 -static -fprofile-generate 옵션을 주고
컴파일한다.

4. simit ［바이너리명］ 명령으로 실행하면 프로파일 정보가 들어있는 파일들이 생성된다.
5. -02 -static -fbranch-probabilities 옵션으로 재컴파일한다.
※저자주 QEMU라는 시뮬레이터가 Simit-ARM보다는 좋다.

@ -funr에니oops 옵션을 이용한 루프 최적화
프로파일 정보를 이용해 컴파일 타임에 루프 횟수가 정해진 루프를 펼친다. 다음 코드
와 같이 소스상에서 몇 번 루프를 도는지 알 수 있는 루프가 있다면 이를 언롤한다.
for

(i=l;

i<50;

i++)

{

func(i);
}

위와 같은 루프를 언롤하면 다음과 같이 된다.
for (i=l; i<50; i+=5) {
func(i);
func (i+1);
func (i+2);
func(i+3);
func(i+4);
}

루프 언롤을 해서 생기는 이점은 브랜치를 좀 더 적게 해서 파이프라인이 깨지는 횟수
를 감소시킨다는 점이다. 하지만 코드 사이즈가 커짐으로써 캐시 미스가 더 많이 발생
할 수 있기 때문에 루프를 무작정 언롤해서는 안 된다.

@ -fpeel-loops 옵션을 이용한 루프 최적화
프로파일 정보로부터 루프가 그다지 많이 돌지 않는다면 루프 필링 (loop peeling 또는

loop splitting이라고도 한다)을 실시한다. 루프 필링이란 루프 내에 인덱스와 인접하

4장_ gcc compiler

271

===== PAGE 273 =====
지만 다른 값을 가지면서 인덱스 범위 내에서 인덱스의 증감과 같이 변하는 연산을 루
프 밖으로 빼는 것을 말한다. 예를 들면 다음과 같다.
k = 10;
for (i=0; i<10; i十+) {
dst [i] = src[i] +src[k];
k = i;
}

너는 0, 1, 2, 3,

10으로 변하고, k는 10, 0, 1, 2,

9로 변한다. 이런 코드를 루프 필링

하면 다음과 같이 된다.
dst[0] = src[0] + src[10];
for (i=l; i<10; i++) {
dst[i] = src[i] +src[i-1];

동일한 기능을 수행하지만 루프 몸체 내에 k=i；가 빠져 루프가 훨씬 가벼워졌다.

H -ftracer
프로파일 결과를 토대로 베이직 블록을 슈퍼 블록으로 만든다. 베이직 블록의 개념은
다음과 같다.
〔예제 4-39] CTest.c 파일 내용

#include <stdio.h>
int main ()
{
int i, j, k;
j = 0;
k = 0;
for (i=0; i < 10; i++) {
if ((i % 2) != 0) {
j += 1；
} else {
k += 1;
}
printf("j = %d, k = %d\n", j r k);

return 0;

272 3부— 컴파일과 링킹

===== PAGE 274 =====
위와 같은 CTest.c 예제 코드가 있을 때 위 코드를 gcc -o CTest CTest.c -fdump-

tree-all 명령으로 컴파일하면 CTest.c.t21.cfg 파일이 생성된다. CFG는 제어 흐름 그
래프(Control Flow Graph)의 약자로, 제어 흐름 분석 (Control Flow Analysis)을 통
해 생성된 결과 파일이다. 모든 컴파일러는 최적화를 위해 제어 흐름 분석과 데이터 흐
름 분석 (Data Flow AnalysisX 기본적으로 하는데, 그 중 제어 흐름 분석은 소스 프로
그램을 제어 흐름 단위로 나누고 그 관계를 분석한 것이다.
〔예제 4-40)

CTest.c.t2I.cfg 파일의 내용

;; Function main (main)
Merging b丄ocks 6 and 7
main ()
{
int k;
int j;
int i;
int D.1909;
_Bool D.1908;
int D.1907;
# BLOCK 0
# PRED: ENTRY (fallthru)
j = 0;
k = 0;
i = 0;
goto <bb 5> (<L4>);
# SUCC: 5 (fallthru)
# BLOCK 1
# PRED: 5 (true)
<L0>:;
D.1907 = i & 1;
D.1908 = (_Bool)
if (D.1908) goto
# SUCC: 2 (true)

D.1907;
<L1>; else goto <L2>;
3 (false)

# BLOCK 2
# PRED: 1 (true)
<L1>:;
j = j + 1；
goto <bb 4> (<L3>);
# SUCC: 4 (fallthru)

4장_ gcc com메er 273

===== PAGE 275 =====
# BLOCK 3
# PRED: 1 (false)
<L2>:;
k=k+
1;
# succ： 4 (fallthru)
# BLOCK 4
# PRED: 2 (fallthru) 3 (fallthru)
<L3>:;
printf (&’’j = %d, k = %d\n" [0] , j, k) ;
i = i + 1;
# SUCC: 5 (fallthru)
# BLOCK 5
(fallthru)
# PRED: 0 (fallthru) 4
<L4>:;
9) goto
<L0>; else goto <L5>;
if (i <=
# SUCC: 1 (true)
6 (false)
# BLOCK 6
# PRED: 5 (false)
<L5>:;
D.1909 = 0;
return D.1909;
# SUCC: EXIT

이렇게 제어 흐름 단위로 나눠진 블록을 베이직 블록이라 부른다. 베이직 블록이란 블
록 내에서는 제어 흐름이 변하지 않고 순차적으로 진행되며 제어 흐름이 바뀌는 단위
로 나눈 소스 코드의 블록을 말한다. 그래서 베이직 블록 내에는 베이직 블록이 끝나는
시점이나 시작되는 시점이 아니고서는 브랜치문과 같이 제어 흐름을 바꿀 수 있는 인
스트럭션은 존재하지 않는다.
위 예제에서 보듯이 CTest.c.t21.cfg는 7개의 베이직 블록으로 이뤄져 있는 것을 확인
할 수 있다. 그리고 각각의 베이직 블록들은 goto문에 의해 제어 흐름이 바뀌거나 레이
블（〈LO〉：, <L1>： 등）에 의해 제어 흐름이 들어오는 단위로 나눠지는 것을 확인할 수 있
다. 위 예제를 제어 흐름 그래프로 그려보면 다음과 같다.

274 3부_ 컴파일과 링킹

===== PAGE 276 =====
［그림 4-57］ CTeslc.t21.cfg의 제어 흐름 그래프

독자가 이해하기 쉽게 C 소스에서 베이직 블록을 나눠 보면 다음과 같다.
〔예제 4-41〕 C 소스에서의 베이직 블럭

#include <stdio,h>
int main()
{
int i, j, k;
j = 0;
k = 0;

이런 베이직 블록 간의 제어 흐름 관계를 나타낸 것이 ［그림 4-5기에 보이는 제어 흐름
그래프다.
간단히 말해 슈퍼 블록이란 제어 흐름 그래프에서 인접한 베이직 블록들을 합쳐 좀
더 크게 만든 블록을 말한다. 베이직 블록을 슈퍼 블록으로 만들 때는 꼬리 복제(tail

duplication)라는 기법을 사용한다.

4장_ gcc compiler 275

===== PAGE 277 =====
이렇게 베이직 블록을 슈퍼 블록으로 만들었을 때의 이점은 인스트럭션 스케줄링 효율
이 향상된다는 점이다. 인스트럭션 스케줄링은 기본적으로 베이직 블록 단위로 수행하
는데, 스케줄링할 인스트럭션 개수가 작으면 스케줄링 효율이 감소한다. 지연이 발생되
는 구간에 끼워 넣을 인스터럭션의 개수가 적기 때문이다.
베이직 블록을 슈퍼 블록으로 만들면 블록의 크기가 훨씬 커져 스케줄링할 대상이 되
는 인스트럭션 개수가 많아져 스케줄링 효율이 향상될 수 있다.
슈퍼 블록을 만들 때 프로파일 정보는 어떤 블록을 슈퍼 블록으로 만들면 더 효율이 좋
을지 결정하는 데 사용된다. 이런 슈퍼 블록은 IA-64와 같은 VLIW 아키텍처에서는 큰
의미가 있지만 그 외 아키텍처에서는 그다지 큰 의미를 지니는 것은 아니다.
同 -fvpt

컴파일러가 조건식의 값에 대한 정보를 수집하는 코드를 추가하게 한다. 그 정보를 바
탕으로 최적화를 수행한다.
지금까지 프로파일 정보를 이용한 최적화 옵션들을 알아보았다. 프로파일 정보에 의한
최적화는 입력 값이 일정한 패턴을 가지는 프로그램에서 많은 성능 향상을 기대할 수
있다. 그러니 두 번 컴파일해야 되는 귀찮음보다 성능 향상이 중요한 프로그램을 작성
하는 독자라면 한 번쯤 사용해 볼 만하다.

I 함수 프레임 포인터 제거
많이 사용되는 최적화 기법으로 함수의 프레임 포인터를 제거하는 방법이 있다. 프레임
포인터를 제거하는 방법은 비교적 안전하고, 손쉽게 할 수 있어 자주 사용되는 최적화
옵션이다. 프레임 포인터를 간단하게 설명하면 다음과 같다.
〔예제 4-42]

test.c 파일 내용

int add(int a, int b) {
return a + b;
}
int sub(int a, int b) {
return a - b;

276 3부— 컴파일과 링킹

===== PAGE 278 =====
［예제 4-42］ 와 같은 코드가 있을 때 이를 gcc -S test.c 명령으로 컴파일하면 다음과
같은 어 셈블리 코드를 얻을 수 있다.
WIEIEffikll test.s 파일 내용

.file
"test. c”
. text
.globl add
.type add, @function
add:
pushl
%ebp
movl
옹esp, %ebp
movl
12(%ebp), %eax
addl
8 (%ebp), %eax
popl
옹ebp
ret
. size
add, .-add
.globl sub
.type
sub, ^function
sub:
pushl
%ebp
movl
%esp, %ebp
movl
12(%ebp), %edx
movl
8 (%ebp), %eax
subl
%edx, %eax
popl
%ebp
ret
.size sub, .-sub
.ident ”GCC: (GNU) 4.1.2 20070925 (Red Hat 4.1.2-27)”
.section
.note.GNU-stack,”",@progbits

add() 함수와 sub() 함수의 최상위를 보면 이전 ebp 레지스터의 값을 스택에 push 하
고, 현재 esp 레지스터의 값을 ebp 레지스터에 설정하는 것이 보일 것이다. ebp 레지
스터가 x86 아키텍처에서 프레임 포인터로 사용되는 레지스터다. 이렇게 함수의 시작
부분에서 ebp 레지스터의 값을 현재 esp 레지스터의 값으로 변경하는 것을 함수의 프
레 임 포인터를 설정 한다고 한다.
이런 프레임 포인터 설정 과정은 함수의 프롤로그(function prologue) 과정 중 하나이
고, 이렇게 설정된 프레임 포인터 레지스터(x86의 경우 ebp)는 함수 내 지역변수를 액
세스한다든지 할 때 기준이 되는 레지스터로 사용된다.
그리고 각 함수의 마지막 부분을 보면 저장했던 ebp 레지스터를 다시 popl 명령으로
복구하는 것이 보일 것이다. 이것은 이전 함수의 프레임 포인터로 복구하는 과정이고

4장_ gcc compiler 277

===== PAGE 279 =====
함수의 에필로그 (function epilogue) 과정 중 하나다. 좀 더 자세히 알고 싶으면 이 책
의 “디버깅” 과정에 있는 “함수 호출 과정과 스택 프레임”이라는 부분을 보기 바란다.
이런 프레임 포인터 설정과 해제 과정은 함수 내에 다른 함수를 호출할 때는 반드시 필
요한 과정이지만 그렇지 않을 때는 그다지 필요하지 않다. 때문에 최적화를 위해서라면
콜 그래프 내의 리프 노드에 있는 즉, 내부에서 어떤 함수도 호출하지 않는 함수에 대
해서는 프레임 포인터 설정과 해제 코드를 제거하는 것이 좋다.

O -fomit-frame-pointer
-fomit-frame-pointer 옵션은 프레임 포인터 설정이 필요 없는 함수에 대해 프레임
포인터 설정을 제거한다. 그래서 ［예제 4-42］ 의 test.c 소스 코드를 -fomit-frame-

pointer 옵션을 주고 gcc -S test.c -fomit-frame-pointer 명 령으로 컴파일하면 다음
과 같은 어셈블리 코드가 만들어진다.
EEBEEflt 프레임 포인터가 제거된 test.s

.file "test. c"
. text
.globl add
.type add, @function
add:
mov丄
8 (%esp), %eax
addl
4 (%esp), %eax
ret
. size add, .-add
.globl sub
.type sub, ^function
sub:
movl
8 (%esp), %edx
movl
4 (%esp), %eax
subl
응edxz %eax
ret
.size sub, .-sub
.ident
"GCC:
(GNU)
4.1.2
20070925
(Red
. section
. note. GNU-stack, ’’", @progbits

Hat 4.1.2-27)"

위 예제를 보면 프레임 포인터가 제거된 것을 확인할 수 있을 것이다. 이런 프레임 포
인터 제거 옵션은 아주 많이 사용하는 최적화 옵션 중의 하나이기 때문에 기억해 두면
좋다.

278 3부_ 컴파일과링킹

===== PAGE 280 =====
I 프리패치(prefetch)를 이용한 최적화
현대에 나오는 거의 모든 아키 텍처는, 프로세서는 매우 빠른 데 반해 메모리는 아주 느
리다. 때문에 load 명령을 처리하는 데 많은 클록 사이클을 소모한다. 큰 배열이 있을
때 루프를 돌면서 배열을 순차적으로 액세스하면서 어떤 명령을 수행한다면 배열의 값
이 캐시에 있지 않는 한 매번 메모리로부터 load가 발생해 프로그램 수행 성능이 나빠
진다. 프리패치를 이용한 최적화는 나중에 프로그램 수행에 필요한 메모리 값을 캐시에
미리 가져다 놓게 프로세서에 지시하는 것을 말한다.

QI —fprefetch—loop—arrays
-fprefetch -loop - arrays 옵션을 사용하면 루프에 진입하기 전에 컴파일러는 루프 내
에서 사용할 메모리 영역을 캐시에 미리 가져다 놓는 프리패치 인스트럭션을 삽입한다.
〔예제 4-45)

test.c 파일 내용

int arrayl[100];
int array2[100];
int

main()
int i, n;
for

：

{

(i=0; i < 100; i++)
array2[i] += arrayl[i] + i;

{

}

：

return 0;
}

：

[예제 4-45]와 같은 test.c 파일이 있을 때 이를 gcc -S test.c -02 -fprefetch-loop-

arrays -march=pentium4 명령으로 컴파일하면 다음과 같이 프리패치 인스트럭션이
삽입된 것을 확인할 수 있다.
〔예제 4-46)

—fprefetch—loop—arrays —march=pentium4 옵션으로 컴파일한 결과

.file "test. c"
. text
.globl main
.type
main, ^function
main:
leal
4(%esp), %ecx
andl $—16, %esp
pushl -4(%ecx)

4장_ gcc compiler 279

===== PAGE 281 =====
pushl
응ebp
movl
%esp, %ebp
pushl %ecx
xorl
응edx, %edx
prefetchtO array2
prefetchtO array2+64
prefetchtO array2+128
prefetchtO array2+192
prefetchtO array2+256
prefetchtO array2+320
prefetchtO arrayl
prefetchtO arrayl+64
prefetchtO arrayl+128
prefetchtO arrayl+192
prefetchtO arrayl+256
prefetchtO arrayl+320
.L2
movl
array2(,%edxz 4), 응eax
addl
arrayl(,%edx,4), %eax
addl
응edx, %eax
movl
%eax, array2(,%edx,4)
addl
$1, %edx
cmpl
$100, %edx
jne .L2
xorl
%eax, %eax
popl
%ecx
popl
%ebp
leal
-4(%ecx), %esp
ret
.size main, .-main
.comm arrayl,400,32
.comm array2,400,32
.ident "GCC: (GNU) 4.1.2 20070925 (Red Hat 4.1.2-27)”
.section
.note.GNU-stack,”",Qprogbits

잘 보면 루프의 시작 부분에 prefetchtO 인스트럭션이 삽입된 것이 보일 것이다. 이 렇게
되면 루프의 시작 부분에서 arrayl과 array2에 있는 값들을 캐시에 가져오기 시작한다.
이 런 프리패치 옵션을 사용할 때는 -02 -march=cpu-type 옵션을 반드시 붙여야 함
을 명심하기 바란다.

280

3부— 컴파일과 링킹

===== PAGE 282 =====
I 레지스터 활용을 통한 최적화
x86과 같은 아키텍처에서는 메모리의 값에 대해 직접 연산할 수 있고, 그런 코드에 대
해 어셈블리 코드가 생성될 때도 직접 연산하는 코드가 생성된다. 자주 사용되는 값이
라면 메모리에 직접 연산하는 코드보다는 메모리 값을 레지스터에 로드하고 레지스터
값을 사용해 연산하는 것이 훨씬 효율적이다.

H -fforce—mem
메모리에 있는 값을 레지스터에 로드해 연산을 수행한다. GCC 4.2에서 제거된 옵션이
지만 이전 버전에서 사용할 수 있다.

@ -fforce-addr
메모리 주소 값을 레지스터에 로드 후 연산을 수행한다.

I gcc 컴파일 속도 최적화
O -pipe
gcc 는 컴파일 시 /tmp 디렉토리에 임시 파일을 생성하고, 각 과정의 바이너리는 이런
임시 파일을 입력으로 받아 다음 과정을 수행한다. -pipe 옵션을 사용하면 컴파일 과
정에서 임시 파일을 생성해 전달하지 않고 파이프로 전달해 컴파일 속도를 좀 더 빠르
게 할 수 있다.

gcc -o test test.c -pipe -v 명령을 내려 보면 다음과 같이 파이프를 통해 히에서 as
로 전달하는 것을 확인할 수 있을 것이다.
/usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl
-quiet
-dumpbase test.c -mtune=generic -auxbase test -version -o - |
as -V -Qy -o /tmp/ccBNINBE.o -

-v

test.c

-quiet

이상으로 gcc 최적화 옵션을 사용한 최적화를 알아보았다. 더 많은 최적화 옵션이 있
지만 이제는 필자도 지친다. 자주 사용하거나 잘 알려지지 않았지만 효과가 큰 최적화
는 거의 대부분 설명한 것 같다. 나머지 옵션들이 궁금한 독자들은 man gcc 명령으로

gcc 매뉴얼을 보면서 찾아보기 바라고, 더 상세한 내용은 info gcc 명령으로 gcc 온라
인 매뉴얼을 보기 바란다.

4장_ gcc com에er 281

===== PAGE 283 =====
5 1기타알아두면좋을만한것
드디어 gcc 그 대단원의 막에 도착했다. 중요한 것들은 훨씬 이전에 설명이 다 끝났다.
지금 할 것들은 그냥 상식선에서 알아 두기 바란다.

I 환경 변수를 사용한 gcc 설정
gcc에서 수행될 때 사용하는 기본 환경 변수들이 있는데, 이런 환경 변수의 값을 설정
해 gcc 수행을 원하는 대로 바꿀 수 있다. 이 런 환경 변수들은 다음과 같다.

O COMPILER_PATH
gcc는 내부적으로 전처리기(ccl -E), 컴파일러(ccl), 어셈블러(as), 링커(collect』또
는 Id)를 호출할 때 COMPILER_PATH에 등록된 디렉토리에서 먼저 전처리기, 컴파일
러, 어셈블러, 링커 등을 찾는다. 그래서 COMPILER_PATH 값을 설정해 우리가 원하는
전처리기, 컴파일러, 어셈블러, 링커 등을 사용해 컴파일하게 하는 것이 가능하다.
# 페도라 7 배포판에 있는 ccl 컴파일러를 /tmp 디렉토리로 복사

$ cp /usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl /tmp
# COMPILER_PATH 환경 변수에 ccl을 찾을 디렉토리로 /tmp와 /root를 설정
$ export COMPILER_PATH=/tmp:/root
# 컴파일명령수행

$ gcc -S test.c -v

이전에 사용한 test.c에 대해 위와 같은 명령을 순차적으로 내리면 /tmp/ccl이 컴파일
러로 사용되는 것을 확인할 수 있다.

@ CJNCLUDE_PATH / CPLUS_INCLUDE_PATH / OBJCJNCLUDE_PATH
소스 파일을 전처리할 때 헤더 파일을 찾을 디렉토리를 지정하는 환경 변수다. C_

INCLUDE_PATH는 C 소스에 대해 지정하고, CPLUS_INCLUDE_PATH는 C++ 소스에
대해 지정하고, OBJC_INCLUDE_PATH는 Objective C 소스에 대해 헤더 파일을 찾을
디렉토리를 지정한다.
예) export C_INCLUDE_PATH=/tmp：/root

282 3부_ 컴파일과 링킹

===== PAGE 284 =====
@ LIBRARY_PATH
라이브러리를 찾을 디 렉토리를 지정하는 환경 변수다. collect2 또는 Id에 게 LIBRARY_

PATH에 등록된 디 렉토리들을 -L 옵션으로 넘긴다.
예） export LIBRARY_PATH=/tmp ：/root

I specs 파일을 이용한 gcc 설정
specs 파일이라고 있는데, -v 옵션을 주고 컴파일하면 제일 처음에 다음과 같은 메시
지가 출력될 것이다.
[root@os
test4]#
Using built-in specs.

gcc

-o

test

test.c

-v

... 하략

이런 specs 파일이 예전에는 파일 시스템상에 존재했었는데, 이제는 gcc에 내장됐다.
내장된 specs 파일을 보는 옵션은 -dumpspecs이다. gcc -dumpspecs〉specs 명
령을 사용해 gcc에 내장된 specs 파일을 덤프해 보면 다음과 같은 specs 파일을 볼 수
있을것이다.
〔예제 4-47]

spesc 파일 내용

*asm:
%{v:-V} %{Qy:} %{!Qn:-Qy} 응{n} %{T} 응{Ym,*} 응{Yd,*} %{Wa,*:%*}
• • • 중략

*cpp:
%{posix:-D_POSIX_SOURCE} %{pthread:-D_REENTRANT}
• • • 중략

ccl -E %{traditional|ftraditional|traditional-cpp:-traditional-cpp}
*ccl:
% (ccl_cpu) % {profile: -p}
..•히륨

이런 specs 파일은 컴파일러 드라이버（ gcc, g++, gcj 등）가 수행될 때 읽어 들이고

specs 파일에 적힌 대로 각각 바이너리（전처리기, 컴파일러, 어셈블러, 링커）들을 호출
하게 되어 있다. 그렇기 때문에 specs 파일을 수정해 원하는 형태로 각각의 바이너리
들을 호출하게 하는 것이 가능하다.

4장_ gcc compiler 283

===== PAGE 285 =====
다음과 같이 명령을 내려 보자.
# 페도라 7 배포판

$ gcc -dumpspecs > /usr/lib/gcc/i386-redhat-linux/4.1.2/specs
# 우분투 7.04 배포판

$ gcc -dumpspecs > /usr/lib/gcc/i486-linux-gnu/4.1.2/specs

그러면 페도라 7 배포판일 경우 /니sr/lib/gcc/i386-redhat-lin니x/4.1.2/specs 파일이
생길 것이다. /usr/lib/gcc/i386-redhat-lin니x/4.1.2/specs 파일을 열어보면 다음과
같은 내용이 있을 것이다.
〔예제 4-48)

• • • O삿랴
—I
*ccl_options:
응（P9 ： % { f
亡己①合“日으코흐七은1‘ : *and -f om코t-f ram은一point은r
are incompatib고e}} % 1 % { !Q:-quiet} -dumpbase %B % { d*}
%
{m*
}
%{a*}
%{c|S:%{o*:-auxbase-strip
%
*
}
%{!o*:-auxbase
%b}}%{!c:%{!S:-auxbase
%b}
}
%{g*}
%{0*}
%{W*&pedantic*}
%
{w}
응{std*&ansi&trigraphs}
%{v:-version}
%{pg:-p}
%{p}
%{f*}
응{undef}
%{Qn:-fno-ident} ------------------------ -------------%{--target-help:--target-help}
%{!fsyntax-only:%{S:%W{o*}%{!o*:-o
%b.s}}}
%{fsyntax-only:-o
%j}
% {-param*} % {fmudflap | f mudflap th: -fno-builtin -f no-merge-constants}
%{coverage:-fprofile-arcs
-ftest-coverage}
• •• 하략

맨 마지막 부분을 보면 %{coverage：-fprofile-arcs -ftest-coverage} 부분이 보이는
데, 의미는 다음과 같다. gcc 명령으로 컴파일 시 -coverage 옵션을 주면 ccl을 수행
할 때 -fprofile-arcs -ftest-coverage 옵션을 추가하라는 의미다.
바로 앞에 있는 %{fmudflap|fmudflapth：-fno-b니iltin -fnoemerge—constants} 구절
의 의미는 gcc 명령으로 컴파일 시 -fmudflap 옵션 또는 -fmudflapth 옵션이 있다면

ccl을 수행할 때 -fno-builtin 옵션과 -fno-merge-constants 옵션을 추가하라는 의
미다.
다른 예를 들면 %{pg：%{fomit—frame-pointer：%e-pg and -fomit-frame-pointer

are incompatible}} 구절의 의미는 -pg 옵션이 있고 동시에 -fomit- frame-pointer
옵션이 있다면 오류(%e)로 “pg and -fomit-frame-pointer are incompatible” 문자
열을 출력하라는 의미이고, %{!Q：-quiet} 구절의 의미는 -Q 옵션이 없다면 -q니iet 옵
션을 추가하라는 의미다.

284 3부—컴파일과링킹

===== PAGE 286 =====
이렇게 specs 파일을 조절하면 컴파일러 드라이버의 동작을 아주 세부적으로 조절할
수 있다. /usr/lib/gcc/i386-redhat-linux/4.1.2/specs 파일에서 *ccl_options： 부분
의 맨 끝에 다음과 같이 -aaa를 추가하면 gcc C 컴파일러 드라이버는 ccl 을 수행할 때

-aaa 옵션을 매번 추가해 오류가 출력된다.
(예제 4-49)

/usr/Iib/gcc/i386-redhat“linux/4.1.2/specs 파일에 一aaa 옵션 추가

• •• 상략

*ccl_options:
%
{pg
:
%
{
fomit-frame-pointer:%e-pg
and
-fomit-frame-pointer
are incompatible } } %1 % { ! Q : -quiet} -dumpbase %B % { d* }
%
{m*
}
%{a*}
%{c|S:%{o*:-auxbase-strip
%
*
}
%{!o*:-auxbase
%b}}%{!c:%{!S:-auxbase
%b}
}
%{g*}
%{0*}
%{W*&pedantic*}
%
{w}
%{std*&ansi&trigraphs}
%{v:-version}
%{pg:-p}
%{p}
%{f*}
%{undef}
%{Qn:-fno-ident} % ---------------------------------- %{--target-help:—-target-help}
%{!fsyntax-only:%{S:%W{o*}%{!o*:-o
%b.s}}}
%{fsyntax-only:-o
%j
}
% {-param* } % {fmudflap | fmudflapth: -fno—bui丄tin -fno-merge-constants}
%{coverage:-fprofile-arcs -ftest-coverage} -aaa
... 하략

다음은 실제 수행 예다.
즈지 root@os：/temp/test4
[root(흐os test4]tt|gccj-o test^t’^E：?'
Reading specs from /usr/lib/gcc/i386-redhat-linux/4.1.2/specs I
Target: 1386-redhat-linux
Configured with: . ./configure--------------------------------------------------- ---- fnandir=/usr/share/nan --info
dir=/usr/share/inFo ——enable-shared —-enable-threads=posix --enable-checki
ng=release --with-system—zlib ——enable-_cxaatexit --disable-libunwind-ex
ceptions --enable-languages=c,c++,objc,obj-c++,jaua,Fortran,ada --enable-j
aua-awt=gtk --disable-dssi --enable-plugin --with-jaua—hone=/usr/lib/jun/j
흐ua-1.5.0—gcj-1.5.0.0/jre ——enable-libgcj-multifile --enable—jaua—maintain
er—node----------------------------------------------------------------------------------------------- .jar* ——

스!

—

Thread model: posix
gcc uersion 4.1.2 2B878925 (Red Hat 4.1.2-27)_______________________________________________
/usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl —quiet —u test.c -quiet -dun
pbase test.c -mtune=qeneric -auxbase test —uersion —aaa —o Ztmp/ccoQ6Txf.s
ccl: error: unrecognized connand line option "—aaa"]
ignoring nonexistent directory '7usr/lib/gcc/i386-redhat-linux/4.1.2/..
/.. ./i386-redhat—linux/include"
ttinclude search starts here:
ttinclude <—> search starts here:
/usr/local/include
/usr/lib/gcc/i386-redhat-linux/4.1.2/include
/usr/include
End of search list.
GNU C version 4.1.2 20070925 (Red Hat 4.1.2—27) (i386—redhat-linux)
compiled by GNU C version 4.1.2 20070925 (Red Hat 4.1.2-27).
GGC heuristics: --------------------------ggc-min—expand=64 ——ggc-min-heapsize=64411
[root@os test』*]# |

[그림 4-58] specs 파일에 -aaa를 추가한 예

4장_ gcc compiler 285

===== PAGE 287 =====
이런 specs 파일을 사용한 설정은 정말 특별한 경우가 아니고는 그다지 사용할 일이
없을 것이다. 하지만 오랫동안 사용된 gcc 설정 방법이기 때문에 개념적으로 알아 두기
바란다.
비로소 gcc 에 대한 모든 설명이 끝났다. 독자들에게 물고기도 잡아주면서 물고기 잡
는 법도 알려주려고 많은 노력을 했는데, 결과가 어떨지는 모르겠다. 부디 이번 장을 통
해 gcc뿐만 아니라 프로그래밍의 원리, 컴파일러, 프로세서에 대해서도 어느 정도 이해
의 폭이 넓어졌기를 바란다. 원리를 이해하면 겁날 것이 아무것도 없다. 무식하게 옵션
이 많은 gcc일지라도 하나씩 벗겨보면 체계와 원리가 보일 것이고, 그런 체계와 원리를
이해하면 앞으로 gcc를 사용하는 데 있어 모르는 부분이 나올지라도 쉽게 난관을 헤쳐
나갈 수 있을 거라 생각한다.
지금까지 gcc 라는 엄청난컴파일러를 헤쳐나온 각자에게 박수를 보내자. 축하한다.
필자가 장담하건대, 이제 독자는 gcc 컴파일러에 있어 어느 누구 못지않은 전문가가
되었다.

286

3부_컴파일과 링킹

===== PAGE 288 =====
5
Id linker

01 링킹의기본 이해
02 ELF 바이너리 포맷 구조
03 Id를사용한링킹
04. 링커 스크립트
05 Id를 사용한 고급 링킹 테크닉
06 라이브러리를만들기

===== PAGE 289 =====
“화룡점정”이란 말이 있다. 필자는 컴파일과 링킹 과정에서 화룡점정이라 할 수 있는 링
킹 과정을 설명하고자 한다. 링킹 없는 컴파일 과정은 감자 없는 감자탕과 같다. 그저
그런 뼈다귀 해장국이 되느냐 훌륭한 감자탕이 되느냐는 감자가 들어가느냐 아니냐가
좌우한다.
마찬가지로 그저 그런 아무 일도 못하는 바이너리 조각이 되느냐 동작 가능한 훌륭한 바
이너리가 되느냐는 최종 링킹 과정이 좌우한다. 원하는 대로 링킹되어 제대로 수행될 때까
지 우리는 여기서 멈출 수 없다.
지금부터 설명할 이야기는 ld(/usr/bin/ld)에 관한 이야기다. Id 는 리눅스 시스템에서 사용
되는 링커다. gcc는 collect2를 호줄해 링킹 과정을 수행하는데, collect》는 내부적으로 진
짜 링커인 W를 호출해 링킹 과정을 수행한다.

===== PAGE 290 =====
1L링킹의 기본이해
링킹 과정은 컴파일과 링킹에서 마지막 과정으로 조각난 오브젝트 파일들을 하나의 바
이너리 이미지로 합치는 과정이다. 그동안 벌려놓았던 모든 일을 정리하고, 컴파일 과
정을 마무리 짓는 과정이라 할 수 있다.
링킹 과정은 매우 단순하다. 링킹 과정은 딱 두 마디로 요약할 수 있는데, 결합과 재배
시 (relocation) 다.

I 링킹 과정 절차
결합 과정은 간단하게 말해 ELF 포맷으로 되어 있는 각 오브젝트를 섹션 종류별로 하나
의 오브젝트로 합치는 과정 이다.
(좌) main.c (우) funcs.c

#include <stdio.h>

#include <stdio.h>

void fund () ;
void func2 ();

extern int varl, var2;
int var8 = 0x33333333;
const int var9 = 0x12345678;
int varlO;

int varl = Oxllllllll;
int var2;
int var3 = 0;
int main() {
static int va r 4 =
0x22222222;
static int var5;
int var6;
printf("This is main()
function!\n") ;
fund () ;
func2 ();

void fund () {
printf ( "This is fund ()
function!\n");
printf ( "varl = 0x%X,
var2=0x%X\n",
varl, var2);
}
void func2() {
printf("This is func2 ()
function!\n");
)

return 0;
}

5장_ Id linker

289

===== PAGE 291 =====
위와 같은 소스 파일들이 있을 때 다음 명령을 내리면 test 실행 파일이 만들어진다.
$ gcc -o test main.c funcs.c -v -save-temps

이때 컴파일 과정에서 호출되는 collect》는 다음과 같은 명령으로 호출된다.
〔예제 5-2〕 링킹 과정 호줄 명령

/usr/libexec/gcc/i386-redhat-linux/4.1.2/collect2
--eh-frame-hdr -m elf_i386 --hash-style=gnu -dynamic-linker /
lib/ld-linux.so.2
-o test
/usr/lib/gcc/i386-redhat-linux/4.1.2/••/../•./crtl.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crti.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/crtbegin.o
-L/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2/../../..
main.o funcs.o
-Igcc --as-needed ---------------------------------------------------- ---Igcc —-as-needed -lgcc_s --no-as-needed
/usr/lib/gcc/i386-redhat-linux/4.1.2/crtend.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/../crtn.o

이후 이렇게 호출된 collect》는 실제 링커인 Id를 호출하는데, collect》가 받은 옵션들
을 Id에 그대로 넘겨 링킹한다. 위 명령에서 collect》만 Id로 변경하면 그대로 링킹됨을
확인할 수 있다.

main.c 와 funcs.c 를 컴파일해 test 실행 파일을 만드는데, 다음 그림과 같이 실제로는
많은 라이브러리와 오브젝트들이 함께 링킹됨을 확인할 수 있다.

[그림 5-1] gcc -o test main.c funcs.c 명령 링킹 과정

290 W_ 컴파일과 링킹

===== PAGE 292 =====
각각의 라이브러리와 오브젝트가 어떤 일을 수행하는지는 이전 컴파일 과정에서 모두
설명 했으므로 따로 설명하지 않는다.
그런데 위 그림과 같이 실제 링킹 과정을 예로 들어 설명을 하자니 링킹 과정에 포함되
는 파일들이 너무 많아 이해하는 데 복잡하다. main.o와 funcs.o 파일만으로 test 실행
파일을 생성할 수 있다고 가정하자. 실제로는 ［그림 5-1］ 과 같겠지만 말이다.

main.c 와 funcs.c 소스 파일만. 0 .루. test 실행 파일이 생성된다고 가정할 때 main.c와
funcs.c 는 컴파일 과정과 어셈블 과정을 통해 main.o와 funcs.o라는 ELF 오브젝트로
만들어지고, 다음과 같은 결합 과정을 거쳐 test 바이너리를 생성한다.
만약 main.o와 funcs.o만을 링킹하여
test를 생성할 수 있다고 가정하면

Symbol Table

[그림 5-2] main.o와 tested 결합 과정

우리는 이전 gcc 컴파일 과정에서 어셈블된 *.o의 오브젝트 파일은 ELF 바이너리 포
맷으로 되어 있다는 것을 배웠고, 또한 ELF 바이너리 포맷은 위 그림과 같이 각 섹션

（ .text 섹션, .data 섹션, .bss 섹션 등）들로 이뤄진다는 것을 배웠다.
각 섹션에 대해서는 나중에 설명하기로 하고, 여기서는 링커인 Id에 의해 각 오브젝트
가 어떤 형태로 결합되어 실행 파일로 만들어지는지 설명한다.
［그림 5-2］ 를 보면 알겠지만 최종적으로 생성되는 test 실행 파일은 main.o와 funcs.o
의 각 섹션이 종류별로 합쳐져 하나의 ELF 실행 파일을 구성한다. 이렇게 합쳐지는 순
서는 별도의 링커 스크립트를 사용하지 않았다면 Id 명령을 내렸을 때 인자로 넣은 오
브젝트 파일의 순서를 따른다. 그래서 Id -o test main.o funcs.o와 같은 명령에 의해

main.o에 있는 .text 섹션이 먼저 오고, 다음으로 funcs.o의 .text 섹션이 온다.

5장_ Id linker 291

===== PAGE 293 =====
다른 섹션 역시 마찬가지다. main.o가 Id의 input 파일 중에 인자로 먼저 왔기 때문에

main.o의 각 섹션이 먼저 오고, 이후에 funcs.o의 섹션들이 종류별로 뒤에 따라온다.
이런 순서로 각 섹션이 배치되는 것은 Id 내부에 있는 기본 링커 스크립트 때문이다. 기
본 링커 스크립트는 나중에 자세히 알아본다.
［그림 5-2］ 에서는 ELF 오브젝트의 섹션 중 매우 중요한 섹션인 .text, .rodata, .data,

.bss 섹션만을 표현하였다. 나중에 설명하겠지만 ELF 오브젝트에는 아주 다양한 종류
의 섹션들이 있다. 그 중 ［그림 5-2］ 와 같이 링킹 과정에서 합쳐지는 섹션들이 있는 반
면에 정보가 통합되거나 없어지는 섹션도 있다.
중요한 점은 Id가 링킹 과정에서 첫 번째 하는 일은 각 오브젝트를 같은 종류의 섹션별
로 묶어 하나의 ELF 바이너리로 만든다는 점이다.
결합 과정이 끝나면 재배치(relocation) 과정이 일어난다. 재배치 과정은 그냥 단순히
결합 과정에서 합쳐진 각 섹션을 실제 코드에 맞게 조정하는 과정이라 말할 수 있다.
재배치 과정은 메모리에 바이너리 이미지가 로드될 위치(x86 리눅스라면 기본 링커 스
크립트에 의해 기본적으로 0x8048000 번지)를 시작으로 결합 과정이 끝난 바이너리에
각 심볼이 가지게 될 실제 주소를 구하고, 해당 심볼을 참조하는 부분에 대해 구한 주
소를 설정하는 과정을 말한다.
여기서 심볼이란 주소를 가지는 모든 것을 말한다. 심볼에는 함수도 있을 수 있고, 변수
도 있을 수 있다. C 소스에서 함수와 전역변수 둥은 컴파일 과정이 끝난 어셈블리 코드
에서 함수와 변수를 참조하기 위한 레이블(label)이란 것을 가진다.
이런 레이블은 함수명 또는 변수명 뒤에 콜론(：)이 붙은 형태다. 어셈블리 코드에서 해당
함수를 호출하거나 해당 변수를 load/store할 때는 이런 레이블을 참조한다. 이후 레이
블은 모두 주소로 변경되고 레이블을 참조하는 부분 역시 레이블의 주소로 변경된다.
［예제 5-1］ 의 main.c 파일을 gcc -S main.c 명령으로 컴파일하면 다음과 같은 어셈블
리 파일이 나오는데, 이중 varl：, var3：, var4.1782：, main： 등과 같이 콜론(:)으로 끝나
는 것들이 레이블이다.

3부_ 컴파일과 링킹

===== PAGE 294 =====
〔예제 5-3)

main.s 파일 내용

.file

"main. c"

• • • 중략

varl:
• • • 중략

.long 286331153
• • • 중략

var3:
. zero 4
• • • 중략

var4.1782:
• • • 중략

.LCO:
.string
. text

"This

is

main()

function!

• • • 중략

main:
leal 4 (%esp), %ecx
• •• 하략

이렇게 레이블처럼 c 소스상에 주소를 표현하는 모든 것을 심볼이라 한다. 사실 레이
블은 심볼을 이루는 대부분이다. 하지만 심볼에 포함되는 것에는 레이블만 있는 것이
아니다. 레이블은 어셈블리상의 주소 표현이고, 나중에 배우겠지만 링커 스크립트에 의
해 생성되는 심볼도 있다.

test
.text

0x8048000

main

0x8048100

fund

0x8048150

func2

call 0x8048100
call 0x8048150
load r1. 0x8048320
load r2. 0x8048390

0x8048200

fund
func2

.rodata

0x8048250

0x8048320

var1

0x8048340
0x8048390

var2

0x8048420

0x8048480

[그림 5-3] 재배치(relocation) 과정

5장_ Id linker

293

===== PAGE 295 =====
결합 과정이 끝나면 재배치 과정이 일어난다고 했다. 먼저 아예 결합 과정도 일어나지
않은 main.o와 funcs.o는 ［그림 5-3］ 과 같이 시작 주소가 0번지로 설정돼 있으며, 각
심볼(main, varl, var2, fund, func2 등)은 시작 주소 0을 기준으로 정렬된다.
［그림 5-3］ 에서 보면 main.o의 .text 섹션에서 funcl()과 func2()를 호출하는 call 인
스트럭션이 있는데, 결합 및 재배치 과정이 이뤄지지 않은 상태에서는 funcs.o에 있는

funcl0 과 func2() 의 주소를 모르기 때문에 각 call 인스트럭션 뒤에 오는 주소 필드는
비어 있다.
마찬가지로 funcs.o 의 .text 섹션에 있는 funcl() 함수에서 varl 과 var2 를 로드하는 인
스트럭션 역시 main.o 에 있는 varl 과 var2 의 주소를 모르기 때문에 초기 값으로 0x0
번지를 load하는 코드로 구성됨을 확인할 수 있다.
결합 과정이 끝나고 나서도 심볼을 참조하는 각 인스트럭션들은 실제 주소를 가지지
않는다. 결합 과정이 끝나면 실제 메모리로 로드될 주소(x86 리눅스라면 0x8048000)
를 기준으로 각 레이블 (main, funcl, func2, varl, var2 등)이 메모리에 위치할 실제 주
소를 알 수 있다. 이렇게 알게 된 주소를 기준으로 해당 레이블을 참조하는 인스트럭션
들에 대해 실제 레이블 주소를 설정하는 과정이 바로 재배치 과정이다.
［그림 5-3］ 에서 보면 funcl은 0x8048100에 위치하고, func2는 0x8048150에 위치한
다. 그러면 재배치 과정을 통해 main 함수에서 funcl 과 func2 를 호출하는 call 인스
트럭션에 실제 funcl 과 func22］ 주소를 넣는다. 마찬가지로 fund 함수에서는 varl
과 var2 를 load 하는 인스트럭션이 있는데, 재배치 과정을 통해 실제 varl 의 주소인

0x8048320과 var2의 주소인 0x8048390을 로드하는 인스트럭션으로 변경된다.
血E ［그림 5-3］은 실제 main.o와 funcs.o의 오브젝트 구조는 아니다. 독자가 이해하기 쉽게 각종 수치를
좀 더 단순화시켰기 때문에 실제 오브젝트와는 약간 차이가 있을 수 있다. 가령 main.o의 .data 섹션에
는 varl 과 wr4만 들어가기 때문에 .data 섹션의 사이즈는 0x20이 아니라 0x8이 되어야 한다.
마찬가지로 main 레이블이 0x8048000번지에 올 수는 없다. 실제 0x8048000번지에는 test 바이너
리의 ELF 헤더가 오고, 이후 프로그램 헤더 테이블이 오고, 이후 각종 섹션들이 온 이후에 main 레이블
이 온다.
위 그림은 독자의 이해를 돕기 위해 각 주소를 단순화시켰음을 기억해 두기 바란다.

재배치 과정까지 끝나면 이제 프로그램을 수행할 모든 준비가 끝났다. ./test 명령을
내리면 bash 셸에서 exec() 시스템 콜을 사용해 test 실행 파일을 메모리에 로드하고

test 프로그램은 위 그림과 같이 Id에 의해 정해진 주소에 로드되어 수행된다.

294 3부_ 컴파일과 링킹

===== PAGE 296 =====
지금까지 링킹 과정에서 일어나는 일들을 알아보았다. 무척 단순하지 않은가? 그렇다.
링킹 과정은 매우 단순한 과정이다. 사시 링킹 과정에서는 링킹 과정 자체를 이해해야
하지만, 링킹에서 사용되는 ELF 바이너리 포맷에 대해 더 자세히 알아 둘 필요가 있다.
이는 마치 불고기보다는 냉면을 맛있게 하는 불고기집과 같다고 생각하면 된다. 이 집
에서는 고기만 먹으면 손해다. 정작 중요한 것은 마지막 냉면을 먹는 것이 더 중요한
그런 형국이라 보면 될 것이다.

02I ELF 바이너 리 포맷 구조
링킹 과정에서 냉면에 해당하는 것은 ELF 바이너리 포맷과 링커 스크립트다. 리눅스/
유닉스 분야에서 뭔가를 이뤄보고 싶은 사람들은 반드시 ELF 바이너 리 포맷을 알아 두
어야 한다.

ELF 바이 너 리 포맷을 아는 것은 바로 도움이 될 수도 있고 바로 도움이 되지 않을 수도
있다. 하지만 리눅스/유닉스 분야의 다른 지식들을 받아들일 때 이해의 폭을 한 차원
높일 수 있으므로 ELF 바이 너 리 포맷은 기초 중의 기초라 말할 수 있다. 그리고 언젠가
는 ELF 바이너리 포맷과 만나야 할 일이 생기게 될 것이다.

I ELF 바이너리 포맷이란?
ELF (Executable and Linkable Format) 바이너리 포맷은 유닉스/리눅스 시스템에서
가장 널리 사용되는 바이너리 포맷이다. ELF 바이너리 포맷 이전에는 COFF(Common

Object File Format) 바이너리 포맷이 사용되었고, 그 이전에는 a.out 이라는 매우 단
순한 바이너리 포맷이 사용되었다.
이전에 gcc를 설명하면서 gcc에 아무런 옵션도 주지 않고 단순히 C 소스 파일만 인자
로 해서 컴파일하면 a.out이라는 실행 바이너리 파일이 생성된다는 점을 기억하고 있
을 것이다. 이 a.out이라는 파일명은 과거에 사용했었던 a.out이라는 바이너리 포맷에
서 유래한다. 그렇다고 해서 a.out 실행 파일이 a.out 포맷이란 것은 아니다. a.out 실행
파일 역시 ELF 바이너리 포맷으로 이뤄졌고 파일명만 전통적으로 그렇다는 이야기다.

5장_ Id linker

295

===== PAGE 297 =====
a.out
（초창기 unix 시스템）

［그림 5-4］ 바이너리 포맷의 변화

a.out 바이너리 포맷은 매우 단순한 포맷으로 초창기 유닉스 시스템에서 사용되다 확
장성과 기능의 한계로 인해 System V（시스템 파이브라 읽는다. 브이가 아님） 초기에

COFF 포맷으로 변경되었다. 한동안 COFF가 사용되다 C++ 프로그램의 지원 등이 미
미한 한계로 인해 혜성같이 등장한 ELF에게 바이너리 포맷의 자리를 내주었다.
오늘날 거의 모든 유닉스 시스템에서는 표준 바이너리 포맷으로 ELF를 사용한다. 때문
에 독자 중 유닉스 시스템 분야에 있어 전문가가 되기를 희망하는 사람이 있다면 이제

ELF는 링커를 알기 위해 알아야 되는 부가적인 지식이 아니라 하나의 과정과 같이 반
드시 알아 둬야하는 내용이다.

ELF 바이너리 포맷은 매우 단순한 구조를 가지고 있어 기본 규칙만 알면 매우 쉽게 이
해할 수 있다.

| ELF 바이너리 포맷의 구조
본격적으로 ELF 바이너리 포맷의 구조를 설명하기 전에 예제로 사용할 바이너리 파일
을 먼저 생성해 놓자. ［예제 5-1］ 에 나온 main.c와 funcs.c를 작성해 다음과 같은 명 령
으로 컴파일해 보자.
$ gcc -o test main.c funcs.c -save-temps
■ bckddn@lksas：~/book
[bckddnhlksas
book]$
gcc
-o
[bckddnQlksas book]후
[ bckddn@lksas book ] $ Is
Funcs.c |funcs.o] main.c |main.o||test|
Funcs.i funcs.s main.i nain.s
[bckddnQlksas book]$ |

test

main.c

Funcs.c

-save-temps

［그림 5-5］ 예제 소스 컴파일

앞으로 위 명령으로 생성되는 test, main.o, f니ncs.o를 기준으로 설명한다. 이렇게 생성
되는 test, main.o, funcs.o 같은 ELF 바이너리 파일은 다음과 같은 구조를 가진다.

296 =_ 컴파일과 링킹

===== PAGE 298 =====
[그림 5-6] ELF 바이너리 포맷의 기본 구조

먼저 ELF 헤더가 온다. 그리고 test와 같은 실행 바이너리에는 프로그램 헤더 테이블이
온다. 실행 바이너리는 필수적으로 존재해야 되는 영역이다. 다음으로 오는 것이 섹션
과 세그먼트들의 영역이다. 이 부분은 바로 다음에 설명한다. 마지막으로 섹션 헤더 테
이블이 온다. 섹션 헤더 테이블은 main.o, funcs.o 같은 재배치 가능한 오브젝트에는
필수적으로 있어야 하는 영역이다.
이것으로 끝, 이것이 ELF 바이너리 포맷의 기본 구조다. 무척 단순한 구조라는 느낌이
들 것이다.
덧붙여서 test 같은 실행 바이너리들을 ELF에서는 재배치 불가능한 ELF 오브젝트라 말
한다. 이는 심볼들의 재배치가 이미 이뤄지고 재배치를 위한 정보를 바이너리에서 제거
해 버렸으므로 재배치를 위한 정보가 없어 링커는 더 이상 재배치 과정을 수행할 수 없
기 때문이다.
그리고 main.o, funcs.o 같은 오브젝트들을 재배치 가능한 ELF 오브젝트라 부른다. 재
배치 가능한 ELF 오브젝트에는 재배치 섹션이라는 것이 존재하는데, 재배치 섹션에는
해당 오브젝트 파일의 어떤 부분에 어떤 심볼로 값을 바꿔야 하는지에 대한 정보가 들
어 있다.

5장_ Id linker

297

===== PAGE 299 =====
I ELF 바이너리를 해석하는 두 가지 관점
ELF에서는 섹션 & 세그먼트 영역을 다음 그림처럼 두 가지 관점으로 볼 수 있다.

Section View

『

(Linkable sections)

■

Segment View

、

(Executable segments)

Describes segments

Describes sections

[그림 5-7] ELF 바이너리 포맷의 두 가지 뷰

먼저 프로그램 헤더 테이블에 의해 해석해 보는 세그먼트 뷰가 있고, 섹션 헤더 테이블
에 의해 해석해 보는 섹션 뷰가 있다.
똑같은 영역을 어떤 테이블로 해석하느냐에 따라 세그먼트 뷰가 될 수도 있고, 섹션 뷰
가 될 수도 있다. 세그먼트 뷰에서는 섹션 & 세그먼트 영역을 세그먼트란 단위로 해석
한다. 세그먼트는 하나 또는 여러 개의 섹션이 모인 단위로, 시스템 로더（ execv 시스템
콜）에 의해 해석되는 단위다.
그래서 시스템 로더는 프로그램 헤더 테이블을 읽어 프로그램을 수행할 때 어디서부터
어디까지를 메모리로 로드해야 되는지 알 수 있다.
섹션 뷰는 섹션 헤더 테이블에 의해 해석되는 뷰다. 섹션 뷰에서는 섹션 & 세그먼트 영역
을 섹션이란 단위로 보는데. 섹션은 링커나 디버거가 ELF 바이너리 포맷을 해석하는 단
위다.

298

3부_ 컴파일과 링킹

===== PAGE 300 =====
I ELF 헤더
이런 프로그램 헤더 테이블과 섹션 헤더 테이블을 나타내는 것은 바로 ELF 헤더다.

ELF 헤더에는 어디서부터 어디까지가 프로그램 헤더 테이블이고, 어디서부터 어디까
지가 섹션 헤더 테이블인지에 대한 정보가 들어있다.
그래서 링커는 바이너리 파일 제일 앞에 오는 ELF 헤더를 읽어 섹션 헤더 테이블의 위
치를 알아내고, 이후 섹션 헤더 테이블에 있는 정보를 이용해 섹션 & 세그먼트 영역을
섹션 뷰로 해석해 링킹 과정을 진행한다. 반면 로더는 ELF 헤더를 읽어 프로그램 헤더
테이블의 위치를 알아 내고, 이후 프로그램 헤더 테이블에 있는 정보를 이용해 섹션 &
세그먼트 영역을 세그먼트 뷰로 해석해 어떤 세그먼트를 메모리로 로드해야 되는지 정
보를 얻어 낸다.
〔예제 5-4〕 /usr/include/elf.h에 있는 ELF 헤더 구조

typedef struct
/* Magic number and other info */

unsigned char

e_ident[EI_NIDENT];

Elf32_Half

e_type

/* Object file type */

Elf32_Ha丄f

ejnachine

/* Architecture */

Elf32_Word

e_version

/* Object file version */

Elf32_Addr

e_entry

/* Entry point virtual address */

Elf32_Off

e__phoff

/* Program header table file offset */

Elf32_Off

e_shoff

/* Section header table file offset */

Elf32_Word

e_Jlags

/* Processor-specific flags */

Elf32_Half

e_ehsize

/* ELF header size in bytes */

Elf32_Half

e_phentsize

/* Program header table entry size */

Elf32_Half

e_phnum

/* Program header table entry count */

Elf32_Half

e_shentsize

/* Section header table entry size */

Elf32_Ha丄f

e__shnum

/* Section header table entry count */

Elf32_Half

e_shstrndx

/* Section header string table index */

} Elf32_Ehdr;

ELF 헤더 구조는 ［예제 5-4］ 와 같다. 복잡하게 보이겠지만 알고 보면 매우 단순한 구
조다. 제일 처음 매직 넘버가 오는데 0x7f, ‘E’, ‘L’, ‘F’가 들어간다. 그리고 오브젝트 타
입 및 각종 아키텍처 정보들이 온다.
여기서 주위 깊게 보아야 될 것은 ELF 헤더에 프로그램 헤더 테이블의 파일상 오프셋

(ejjhoff)과 섹션 헤더 테이블의 파일상 오프셋(e_shoff)이 들어 있다는 점이다.

5장_ Id linker

299

===== PAGE 301 =====
그리고 각 헤더의 크기 (e_phentsize, e_shentsize)와 개수 정보(e_phnum, e_shnum)
도 함께 있어 링커와 로더는 ELF 헤더만 읽어보면 프로그램 헤더 테이블 또는 섹션 헤
더 테이블을 쉽게 찾을 수 있고, 해당 테이블의 엔트리 사이즈와 개수도 쉽게 파악할
수 있다.

ELF 헤더에는 프로그램 시작 위치를 결정하는 엔트리 정보(e_entry)도 있는데, 엔트리
는 로더가 프로그램을 메모리에 로더하고 제일 처음 시작할 주소를 의미한다. 이런 엔
트리 주소는 _start 레이블로 설정된다. 왜 처음 시작할 주소가 main이 아닌 _start인지
는 이전 컴파일 과정을 본 독자라면 쉽게 이해할 수 있을 것이다.
그러면 ELF 헤더가 실제로 ［예제 5-4］ 와 같은 정보로 이뤄졌는지 확인해 보자.

readelf -h ［ ELF 오브젝트］ 명령을 내리면 ELF 오브젝트의 ELF 헤더 정보를 읽을 수
있다. 다음은 test 바이너리와 main.o의 ELF 헤더 내용을 읽어본 화면이다.

［그림 5-8］ readelf -h test 명령으로 본 test 바이너리의 ELF 헤더

300

3부— 컴파일과 링킹

===== PAGE 302 =====
［그림 5-9］ readelf -h main.o 명령으로 본 main.o 바이너리의 ELF 헤더

그러면 실제 ELF 헤더에는 프로그램 헤더 테이블과 섹션 헤더 테이블의 파일상 시작
주소가 들어 있음을 확인할 수 있다. 그리고 main.o와 같이 재배치 가능한 ELF 오브젝
트에는 프로그램 헤더의 개수가 0이라는 것을 확인할 수도 있다.

| 프로그램 헤더 테이블
프로그램 헤더 테이블은 다음과 같은 형태를 가진다.

typedef struct
{
Elf32_Word
Elf323)ff
Elf32jlddr
Elf322Addr
Elf322word
Elf32Jiord
Elf322word
Elf322word
} Elf322：Phdr;

p_type;
p_offset;
p__vaddr;
p_paddr;
p_filesz;
pjnemsz;
p^flags;
p_align;

［그림 5너이 프로그램 헤더 테이블의 구조

5장_ Id linker

301

===== PAGE 303 =====
프로그램 헤더 테이블은 프로그램 헤더 구조체로 이루어진 배열이다. 그래서 프로그램
헤더 테이블이라고 이야기한다. 하나의 엔트리는 하나의 세그먼트를 지칭한다. 프로그
램 헤더 테이블의 각 엔트리는 다음과 같은 형태다.
I〔예제 5-5〕»usr/include/elf.h에 있는 프로그램 헤더 구조

typedef

struct

Elf32_ _Word
Elf32_ _Off
Elf32_ _Addr
Elf32_ _Addr
Elf32_ _Word
Elf32_ _Word
Elf32_ _Word
Elf32_ _Word
} Elf32_ _Phdr;

p_type;
p_offset;
p_vaddr;
p_paddr;
p_filesz;
p_memsz;
p_flags;
p_align;

/*
/*
/*
/*
/*
/*
/*
/*

Segment
Segment
Segment
Segment
Segment
Segment
Segment
Segment

type */
file offset */
virtual address */
physical address */
size in file */
size in memory */
flags */
alignment */

프로그램 헤더 구조체를 보면 해당 세그먼트의 세그먼트 타입은 무엇이며, 파일상 위치
는 어떠하며, 크기는 어떤지, 그리고 메모리로 로드될 가상 주소와 물리 주소는 어떤지
등에 대한 정보를 담고 있다.

test와 같은 최종 실행 바이너리에는 프로그램 헤더 테이블이 반드시 있어야 한다. 그
러나 main.o와 fimcs.o와 같이 재배치 가능한 ELF 오브젝트는 프로그램 헤더 테이블
이 없어도 된다.
프로그램 헤더 테이블은 시스템 로더（ exec 시스템 콜）에 제공할 정보를 담고 있다. 셸
에서 test 바이너리를 실행하면 시스템 로더는 test 바이너리의 프로그램 헤더 테이블
을 읽어 test 바이너리에서 어떤 부분을 메모리로 로드해 프로세스를 만들 것인지 알
수 있다.

302 3부_ 컴파일과 링킹

===== PAGE 304 =====
; bckddn@lksas：~/book ______ _______________
[bcl《dcln@ll<sas bool<l$|rea(lel.F '-1
E1F File type is EXEC (Executable file)
Entry point 0x8O482e0
There are 7 program headers, starting at offset 52
Program Headers:
Type
OFFset
UirtAddr
PhysAddr
FileSiz MemSiz
Fig
PHDR
0x00003스
8x08048034
0x08048034
0X000?0 0X00Oe0 R E
INTERP
0X080114
0x08848114
0X08048114
0x00013 0X00013 R
[Requestinq proqran interpreter: /lib/ld-linux.so.2]
LOAD
0X000000 0X08048000
0x08848080 0x00578 0x00578 R E
LOAD
0x000578 0x08049578
0x08 049578 0x0010c 0X08124 RW
DVNfiMIC
0x00058c 0x0804958c
0x08 04958c 8X00OC8 0xWOc8 RW
NOTE
0x600128 0x88048128
0X08048128 0X00020 0x80820 R
GNU_STRCK
0X600000 0X00000000
6x00000000 0X00000 0x08000 RW
Section to Segment mapping:
Segment
Sections________
08
01 .interp
02 .interp .note.ABI-tag .gnu.hash .dynsym .dynstr .gnu.uersion
ersion_r .rel.dyn .rel.plt .init .pit -text .fini .rodata .eh_Frane
83 .ctors .dtors .jcr .dynamic .got .got.pit .data .bss

W

Align
0x4
0x1
0x1080
0x1600
0X4
0x4
0x4

.gnu

■丁西펴而W

05
.note.ABI-tag
06
[bckddnmksas book]$ |

［그림 5-11］ readelf -I test 명령으로 본 test 파일의 프로그램 헤더 테이블 정보

［그림 5-11］ 은 readelf -1 test 명령으로 본 test 실행 바이너리 파일의 프로그램 헤더
테이블 정보다. 그림에서 보면 타입 부분에 LOAD라고 적혀 있는 부분이 메모리로 로
드해야 될 세그먼트다.
이전에도 설명했지만 세그먼트는 시스템 로더가 프로그램을 보는 단위로, 하나의 세그
먼트에는 여러 개의 섹션이 포함될 수 있다. 그림에서 “Program Headers” 부분에 있
는 각 라인이 각 세그먼트를 의미하고 프로그램 헤더의 정보를 나타낸다.
Type
Offset
LOAD 0x000000

VirtAddr
0x08048000

PhysAddr
0x08048000

FileSiz
0x00578

MemSiz
0x00578

Fig
RE

Align
0x1000

LOAD라고 표시된 것 중 첫 번째 라인만 해석해 보면 다음과 같다.
먼저 타입은 메모리에 로드해야 되는 세그먼트다. 그리고 파일상의 시작 오프셋은 0x0
이고, 로드할 가상 주소는 0x8048000이고, 물리 주소 역시 0x8048000이다. 특별한 경
우가 아니라면 가상 주소와 물리 주소는 동일하다.
로드할 크기는 0x578이기 때문에 결국 파일상 오프셋 0x0에서 0x578 바이트만큼 메모
리에 로드함을 알 수 있다. 메모리에 잡히는 사이즈는 0x578로 파일상 사이즈와 동일
하다.

5장_ Id linker 303

===== PAGE 305 =====
이렇게 메모리상 사이즈와 파일상 사이즈는 동일할 수도 있지만 .bss 섹션과 같이 파일
사이즈에는 잡히지 않고 메모리 사이즈에만 잡히는 섹션을 포함하는 세그먼트는 파일
사이즈와 메모리 사이즈가 다를 수 있다.
마지막으로 플래그 부분에 우라고 된 것은 읽기 (R) 가능하고 실행®) 가능한 세그먼
트란 의미다. RE 외에도 W가 올 수 있는데, 쓰기 가능한 세그먼트란 의미다. 정렬 부분

(Align)에 0x1000으로 된 것은 이 세그먼트가 0x1000 단위로 정렬되어야 함을 의미한다.
OxlWO은 하나의 페이지 단위(4K)이므로 결국 페이지 단위로 정렬되어야 함을 의미한다.
프로그램 헤더의 타입에는 LOAD 외에도 다음과 같은 것들이 올 수 있는데, 각각의 의
미는 다음과 같다.
[표 5-1] 프로그램 헤더 타입 리스트

타입명

의미

LOAD

메모리에 로드해야 되는 세그먼트

NULL

사용되지 않는 프로그램 헤더

DYNAMIC

동적 링크를 해야 되는 자료를 포함하는 세그먼트

INTERP

인터프리터 이름을 포함하는 세그먼트

PHDR

프로그램 헤더를 포함하는 세그먼트

NOTE

노트 정보를 포함하는 세그먼트

SHLIB

예약된 n루그램 헤더

나머지 세그먼트들에 대해서는 위에 필자가 해석한 대로 해석해 보면 금방 어떤 세그
먼트를 의미하는지 알 수 있을 것이다.
하단에 “Segment Sections...”라고 표현된 부분은 “Program Headers”의 각 세그먼트
가 어떤 섹션들로 이뤄졌는지 나타낸다. 그래서 메모리로 로드되는 섹션에는 .text 섹
션과 .rodata 섹션, .data 섹션, .bss 섹션 등이 포함됨을 알 수 있다. 이런 섹션들은 섹
션 헤더 테이블에 의해 해석된다.

I 섹션 헤더 테이블
섹션 헤더 테이블은 섹션 & 세그먼트 영역에서 어디서부터 어디까지가 무슨 섹션이고,
해당 섹션의 특징은 어떤지에 대한 정보를 담고 있다. 섹션 헤더 테이블이 없다면 링커
나 디버거는 ELF 오브젝트를 해석할 수 없었을 것이다. 섹션 헤더 테이블은 main.o나

funcs.o 같이 재배치 가능한 ELF 오브젝트에는 반드시 있어야 한다.

304 3부_ 컴파일과 링킹

===== PAGE 306 =====
섹션 헤더 테이블은 다음과 같은 구조를 가지고 있다.
ELF Header
Program Header
Table
.text
.data

.rodata
typedef struct
{
Elf32_Word
Elf32_Word
Elf322word
Elf322Addr
Elf323)ff
ElfaOord
Elf322word
Elf322word
Elf32~Word
Elf32Jtord
} Elf32：Shdr;

.symtab
.strtab
.r 이.text
.r 이.data
Section header 0

.rel.rodata

Section header 1
Section header 2
Section header 3

Section Header Table

Section header 4

sh_name;
sh_type;
sh_flags;
sh_addr;
sh_of.fset;
sh_size;
sh_link;
sh_info;
sh_addralign;
sh_entsize;

[그림 5-12] 섹션 헤더 테이블의 구조

프로그램 헤더 테이블과 마찬가지로 섹션 헤더 테이블 역시 섹션 헤더 구조체의 배열
로 되어 있다. 섹션 헤더 구조체는 다음과 같다.
〔예제 5-6)

/usr/include/elf.h에 있는 섹션 헤더 구조

typedef struct
Elf32 Word

Section

name (string

tbl index)

sh_name;

/*

sh_type;
sh_flags;
sh_addr;
sh_offset;
sh_size;
sh_link;
sh_info;
sh_addralign;
sh entsize; /

/ Section
type */
/ Section
flags */
/ Section virtual addr at
execution 大/
/ Section
file offset */
.*
/ Section size in bytes
/ 大 Link to
another section */
/ Additional section information */
/ Section alignment 大/
Entry size if section holds table */

*/
Elf32_Word
Elf32_Word
Elf32_Addr
Elf32_Off
Elf32_Word
Elf32_Word
Elf32_Word
Elf32_Word
Elf32_Word
} Elf32 Shdr;

섹션 헤더 구조를 살펴보면 해당 섹션의 이름(sh_name), 타입 (shjype), 파일상의 위
치 (sh_offset) 및 크기 (sh_size) 등의 정보를 담고 있다.

5장_ Id linker

305

===== PAGE 307 =====
bckddn@lksas：~/book

스!

스!

[bckddnSlksas bookreadelf -S main.o|
There are 11 section headers, starting at oFFset 8x10c:
Section Headers:
[Nr] Name
Type
Addr
OFF Size ES Fig Lk InF Al
[ 0]
NULL
00000000 000800 000000 00
[ 1] .text
PROGBITS
00000000 000034 000035 08 AX 0
[ 2] .rel.text
REL
00000000 000418 000020 08
[ 3] .data
PROGBITS
00000000 00006c 000008 08 WA 004
[ 4] .bss
NOBITS
08000000 000074 008008 00 WA 804
[ 5] .rodata
PROGBITS
00800000 000074 000019 00 A 8
[ 6] .comment
PROGBITS
08000000 00008d WO02e W
[ 7] .note.GNU-stack PROGBITS
00000000 0808bb 008000 00
[ 8] .shstl'tab
STRTAB
08000000 0000bb 000051 00
[ 9] .symtab
SYI4TAB
00090000 0002c4 000110 10
[10] .strtab
STRTAB
00009000 0883d4 000041 00
Key to Flags:
W (write), A (alloc), X (execute), M (merge), S (strings)
I (inFo), L (link order), G (group), x (unknown)
0 (extra OS processing required) o (OS specific), p (processor specific)
[bckddnQlksas book]$ |

000
04
914

01
001
0
01
0
01
10 10 4
0
91

비
[그림 5-13】 readelf -S main.o 명령으로 읽어본 main.o의 섹션 헤더 테이블 정보

[그림 5-131 은 readelf -S main.o 명령으로 읽어본 main.o 파일의 섹션 헤더 테이블
정보다. 보면 알겠지만 main.o 파일은 .text, .rel.text, .data, .bss, ,rodata, .comment
등의 섹션으로 이뤄졌다.
이 중에서 .text 섹션 라인만 따로 떼어 설명한다.
[Nr] Name
[ 1] .text

Type
PROGBITS

Addr
00000000

Off Size
000034 000035

ES Fig
00 AX

Lk Inf Al
0
04

[Nr]은 섹션 테이블에서 인덱스를 의미한다. Name은 당연히 섹션의 이름을 의미하고,
타입에 있는 PROGBITS는 프로그램에서 정의된 섹션임을 의미한다.
프로그램에서 정의된 섹션이 란 소스 프로그램에서 프로그래머가 명시적으로 컴파일러
디렉티브나 어셈블리 디렉티브를 사용해 어떤 함수 또는 변수를 특정 섹션에 생성한
경우일 수도 있고, 컴파일러에 의해 기본적으로 생성된 섹션일 수도 있다.
다음 예는 프로그래머가 컴파일러 디렉티브 또는 어셈블리 디렉티브를 사용해 특정한
함수를 특정한 섹션에 명시적으로 생성한 예다.
〔예제 5-7) r myfunc 함수를 .mysection에 생성한 C 소스 예

int

attribut은
return 0;

}

306 3부— 컴파일과 링킹

((

section

("

.mysection”)))

myfunc

()

{

===== PAGE 308 =====
〔예제 5-8〕 myfunc 함수를 .mysection에 생성한 어셈블리 소스 예

.section .mysection,”ax”,@progbits
.globl myfunc
•type
myfunc,
@function
myfunc:
pushl
%ebp
mov丄
%esp, %ebp
movl
$0, %eax
popl
%ebp
ret

［예제 5-刀은 컴파일러 디 렉티브를 사용해 myfunc 함수를 .mysection에 생성한 예이
고, ［예제 5-8］ 은 어셈블리 디렉티브를 사용해 myfunc 함수를 .mysection에 생성한
예다. C 소스에서 함수나 변수 앞에 __attribute__ ((__section__ (”섹션명")))이라는
키워드를 적어주면 gcc가 알아서 해당 함수나 변수를 “섹션명”이라고 적어준 섹션에
생성한다.
컴파일러가 기본적으로 생성하는 섹션이란 , 컴파일러는 기본적으로 프로그래머가 명시
적으로 어떤 섹션에 생성하지 않은 변수와 함수들에 대해 인스트럭션은 .text 섹션에,
초기화된 변수는 .data 섹션에, 초기화되지 않은 변수는 .bss 섹션에, 문자열과 같은 것
은 .rodata 섹션 등에 생성하는 것을 의미한다.
이렇게 프로그래머가 명시적으로 생성한 섹션이나 컴파일러가 기본적으로 생성한 섹
션들은 타입 값으로 PROGBITS를 가진다.

I 각종 섹션의 종류
.text 섹션은 컴파일러가 기본적으로 생성한 섹션이고 프로그램의 인스트럭션을 담고
있는 섹션이다. 때문에 당연히 타입으로 PROGBITS7} 오게 된다. 타입으로 올 수 있는
것은 PROGBITS 외에도 다음과 같은 것들이 있다.
［표 5-2］ 섹션 헤더 타입 리스트

타입명

의미

NULL

비활성 섹션으로, 관련된 섹션이 없음을 의미한다.

PROGBITS

프로그램에서 정의된 섹션이다. 프로그래머에 의해 명시적으로 정의되었을 수도 있고,
컴파일러에 의해 기본적으로 정의되었을 수도 있다.

SYMTAB

심볼 테이블을 가지고 있는 섹션이다.

5장_ Id linker 307

===== PAGE 309 =====
타입명

의미

STRTAB

스트링 테이블을 가지고 있는 섹션이다. 여기서 스트링이란 ELF 바이너리를 해석하기
위한 여러 가지 문자열을 말한다. 예를 들면 여러 심볼의 스트링, 섹션 이름 스트링 등
을 의미한다（ C 소스상의 스트링을 의미하지 않음을 유념하기 바란다）.

REUX

명시적인 가수가 있는 재배치 엔트리들을 가지고 있는 섹션이다. 여기서 명시적인 가
수란 A=BK에서 B가 심볼이라 가정할 때 C처럼 더하는 수를 의미한다. REUX 섹션은
재배치 엔트리들로 구성되는데, 각 엔트리에는 재배치해야 될 위치와 심볼명들이 들
어 있다.
그리고 하나의 오브젝트는 여러 개의 재배치 섹션을 가질 수 있다.

HASH

심볼의 해시 테이블을 가지고 있는 섹션이다. 동적 링킹하는 오브젝트는 심볼 해시 테
이블을 가지는데, 이런 해시 테이블이 들어있는 섹션을 의미한다.

DYNAMIC

동적 링킹을 위한 정보가 들어있는 섹션이다.

NOTE

파일 정보가 들어있는 섹션이다.

NOBITS

아무런 공간을 차지하지 않는 섹션이다. ,bss 섹션이 이에 해당한다.

REL

명시적인 가수가 없는 재배치 엔트리를 가지는 섹션을 의미한다. 가수 부분을 제외하고
REL人 섹션과 많은 부분이 같다.

SHLIB

예약된 섹션이지만 특별한 의미를 가지는 섹션은 아니다.

DYNSYM

동적 링킹 심볼들이 아주 작게 들어가는 섹션이다.

LOPROC

프로세서 의존적인 정보를 포함하는 섹션이다.

HIPROC

프로세서 의존적인 정보를 포함하는 섹션이다.

LOUSER

애플리케이션을 위해 예약된 인덱스의 하위 한도를 포함하는 섹션이다.

HIUSER

애플리케이션을 위해 예약된 인덱스의 상위 한도를 포함하는 섹션이다.

다시 본론으로 돌아가 .text 섹션에서 타입 다음에 있는 Addr 필드는 .text 섹션이 메모
리로 로드될 때의 주소를 의미한다. 현재 main.o는 아직 메모리에 로드될 정확한 주소
가 정해지지 않아서 시작 주소가 0x0으로 설정되어 있다. 최종 바이너리 단계로 가야
메모리에 로드될 주소가 정해진다.

Off 필드는 오프셋을 의미하는 필드로, .text 섹션이 파일상 어떤 위치에 있는지 나타
낸다. 그래서 위 예에서 .text 섹션은 main.o 파일의 시작에서부터 0x34 바이트 떨어
진 위치에서 시작됨을 알 수 있다. Size는 당연히 .text 섹션의 사이즈를 말한다. 그래서
위 예에서 .text 섹션은 main.o 파일의 시작 부분인 0x34 바이트에서 시작하고 크기가

0x35바이트임을 의미한다.

308

3부_컴파일과 링킹

===== PAGE 310 =====
ES 는 엔트리 사이즈라는 의미로, 심볼 테이블 섹션 (.symtab) 또는 재배치 섹션 (.rel.
text, .rel.data 등) 등과 같이 고정된 사이즈를 가지는 엔트리들로 이뤄진 섹션들의 경우
에 한 엔트리의 크기를 바이트 단위로 나타내는 필드다. .text 섹션은 고정된 크기의 엔
트리로 이뤄진 섹션이 아니므로 0x0으로 표현된다. Fig 필드는 섹션의 속성을 나타내는
플래그로 W(데이터를 가지고 있음), A(프로세스 실행 동안 메모리를 차지함), X(인스트
럭션을 가지고 있음), M(프로세서 고유의 특징을 위해 예약해 놓음) 등이 있다.

Lk(link) 필드는 다른 섹션에 의존해 해석해야 되는 섹션에 의존하는 섹션 인덱스를 포
함하는 필드이고, Inf(info) 필드는 의존하는 섹션에 대해 그 외 정보를 포함하는 섹션
이다.
마지막으로 Al(align) 필드는 .text 섹션이 메모리 주소에서 어떤 단위로 정렬되어야 함
을 나타낸다. .text 섹션의 정렬 필드는 4이기 때문에 4바이트 단위로 메모리 주소상에
서 정렬되어야 함을 알 수 있다.
지금까지 .text 섹션에 대한 설명이 다 끝났다. 나머지 섹션들에 대해서도 필자가 설명
한 대로 해석해 보면 금방 어떤 의미라는 것을 알 수 있을 것이다. 그러면 ELF 바이너
리 포맷에는 어떤 섹션들이 있는지 알아보자.

ELF 바이너리 포맷의 각 섹션은 각각의 정보들을 담고 있다. 예를 들면 .text 섹션은 인
스트럭션을 담고 있고, .symtab 섹션은 심볼 테이블을 담고 있으며, ,debug_info 섹션
은 디버깅 심볼 정보를 담고 있다.
각각의 정보들은 구조도 제각각이다. .text 섹션은 인스트럭션이 연속해서 들어 있는 형
태이고, .symtab 섹션은 테이블 형태이고, .debugjnfo 섹션은 트리 구조이다. 이렇게
정보도 다르고 구조도 다른 각 섹션에 대해 링커 또는 디버거, 시스템 로더 등은 자신
에게 필요한 정보가 든 섹션만 골라서 정보를 해석하고, 하고자 하는 일을 수행한다.

ELF 섹션에는 유저가 명시적으로 정의한 섹션도 있고 컴파일러가 정의한 섹션도 있다.
이 중 알아야 될 것은 컴파일러가 정의한 섹션이다. ELF 바이너리 포맷에는 다음과 같
은 컴파일러가 정의한 섹션이 있고, 의미는 다음과 같다.

5장_ Id linker

309

===== PAGE 311 =====
[표 5-3] ELF 바이너리 포맷에 포함되는 섹션 리스트

섹션명

설명

.text

프로그램 수행에 필요한 인스트럭션이 들어가는 섹션이다.

.rodata

프루그램 메모리 이미지에 포함되는 읽기 전용（ read-only） 데이터가 들어가는 섹션이다.

.rodatal
.data
.datal

초기화된 전역 데이터 혹은 static 데이터를 포함하는 섹션이다. 여기서 초기화되었다는 말
의 의미는 001 아닌 초기 값을 가지는 실제 메모리상에 잡히는 전역변수 혹은 static 변수와
같은 데이터를 의미한다.

,bss

초기화되지 않은 전역 데이터 혹은 static 데이터를 포함하는 섹션이다. 여기서 초기화되지
않았다는 말의 의미는 0인 초기 값을 가지는 실제 메모리상에 잡히는 전역변수 혹은 static
변수와 같은 데이터를 의미한다.
.bss 섹션은 실제 파일 이미지상에는 포함되지 않고, 프로세스를 생성할 때 메모리상에 공

간이 할당된다.
.comment

버전 제어 정보가 들어가는 섹션이다. 컴파일한 gcc 버전 정보가 들어간다.

.ctors

C++ 생성자 함수들에 대한 초기화된 포인터들이 들어간다.

.dtors

C++ 소멸자 함수들에 대한 초기화된 포인터들이 들어간다.

.debug

“디버깅을 위한 심볼 정보 또는 라인 정보가 들어가는 섹션이다”라고 ELF 매뉴얼（ man 이f라

Jine

고 명령을 치면 볼 수 있다）에서 이야기하고 있지만 매뉴얼대로 특별히 그렇지는 않다.
리눅스 시스템에서는 디버거를 위해 DWARF라는 디버깅 정보 섹션들을 제공한다. gcc -g
옵션으로 컴파일하면 ELF 바이너리에 디버깅 정보를 위한 섹션들이 추가되는데, 현재 가장
많이 사용되는 DWARF2（ 버전 2라는 의미）에서는 다음과 같은 섹션들이 ELF 바이너리의 섹
션으로 추가된다.
.debugjnfo : 디버깅 심볼 정보（변수명, 함수명, 타입 등）가 들어있는 섹션
.debug_abbrev : .debugjnfo를 해석하기 위한 정보가 들어있는 섹션
.debugjine : 인스트럭션의 소스상 라인 정보가 들어있는 섹션
.debug_pubnames : 이름으로 심볼 정보를 찾을 수 있는 정보가 든 섹션
.debug_aranges : 주소로 심볼 정보를 찾을 수 있는 정보가 든 섹션
.deb니g_str: .deb니g_* 섹션들에서 참조하는 스트링이 들어있는 섹션
.debugjoc : 로케이션 정보가 든 섹션
.debugjrame : 함수 프레임 정보가 든 섹션
.debug 섹션과 Jine 섹션은 DWARF2 섹션 중 .debugjnfo 섹션과 .debugjine 섹션에 해당

한다.
.dynamic

동적 링킹 정보가 들어가는 섹션이다.

.dynstr

동적 링킹을 위해 필요한 심볼 테이블이 들어가는 섹션이다.

jnit

프로세스 초기화를 위한 인스트럭션이 들어있는 섹션이다. 프로그램이 실행될 때 main 엔트
리 포인터를 부르기 이전에 이 섹션에 있는 인스트럭션들이 먼저 수행될 수 있다.

.fini

프로세스 종료를 위한 인스트럭션이 들어있는 섹션이다. 프로그램이 종료될 때 이 섹션에
있는 인스트럭션이 수행될 수 있다.

.got

전역 오프셋 테이블이 들어가는 섹션이다. 전역 오프셋 테이블은 공유 라이브러리 같은
PIC（ Position-Independent Code） 코드를 생성하기 위해 필요한 테이블이다. 자세한 내용은

공유 라이브러리를 설명할 때 다룬다.

310 3부—컴파일과링킹

===== PAGE 312 =====
섹션명

설명

.pit

프로시저(procedure) 링킹을 위한 테이블을 가지는 섹션이다. 공유 라이브러리에 포함된 함
수를 사용할 때 동적 링커 또는 해당 공유 라이브러리 함수를 호출하기 위한 인스트럭션을
초기에 포함한다. 자세한 내용은 공유 라이브러리를 설명할 때 다룬다.

.hash

심볼 해시 테이블을 포함하는 섹션이다.

Jnterp

프로그램 인터프리터의 패스가 들어가는 섹션이다. 공유 라이브러리를 사용할 경우 /lib/ldlin니x.so와 같이 동적 링커의 패스가 들어간다.

.note

특정 유닉스 시스템. ABI 등을 위한 정보를 포함하는 섹션이다.

.r이 NAME

재배치 정보를 가지는 섹션이다. 어떤 섹션의 특정 부분을 재배치해야 한다면 해당 섹션의

.relaNAME

재배치 섹션이 포함된다. NAME은 재배치를 해야 될 섹션을 의미한다. 예를 들면 .text 섹션
의 특정 부분을 재배치해야 한다면 .rel.text 섹션이 추가되고, .rel.text 섹션에는 .text 섹션에
서 재배치해야 될 심볼 정보와 섹션상의 위치가 들어간다. 마찬가지로 .debugjnfo 섹션의
특정 부분을 재배치해야 한다면 .rekdebugjnfo 섹션이 추가되고, 재배치해야 될 심볼 정보
와 섹션상 위치가 들어간다.
링커는 이런 재배치 섹션(.r이*, .rela*)을 보고 재배치해야 될 심볼들의 위치와 정보를 파악
한다.

.shstrtab

섹션들의 이름(스트링) 테이블을 포함하는 섹션이다.

.strtab

각종 심볼들의 스트링 테이블이 들어가는 섹션이다.

.symtab

심볼 테이블이 들어가는 섹션이다.

위 섹션 리스트는 리눅스 시스템에서 man elf 명 령으로 ELF 메뉴얼을 봤을 때 나오는
내용을 바탕= 작성되었다. 이 매뉴얼은 1999 년에 작성되어 현실과는 약간 차이가
있을 수 있다. 위에서 설명한 섹션 외에도 현재는 .gnuhash, .dynsym, .dynstr 등과 같
은 섹션들이 gcc로 컴파일하면 기본적으로 추가될 수 있다.
무척 많은 섹션이 있다. 전부 다 이해할 필요는 없고 필자가 굵게 표시한 .text, .rodata,

.data, .bss 섹션만 확실하게 이해하면 된다. 나머지 섹션들에 대해서는 어떤 섹션들이
있을 수 있는지만 확인하고, 나중에 ELF 바이너리 포맷으로 무언가를 하고자 할 때 보
아도 늦지 않다.

.text 섹션은 ［표 5-3］ 에서 설명한 대로 프로그램의 인스트럭션이 들어가는 섹션이다.
이해하기 쉽게 ［예제 5-9］ 의 소스를 다음 명령으로 컴파일한 후 예를 들어 설명하도록
하겠다.
$ gcc -o test main.c funcs.c -save-temps -g

5장_ Id linker 311

===== PAGE 313 =====
〔예제 5-9〕 (좌) main.c (우) funcs.c

#include <stdio.h>

#include <stdio.h>

void fund () ;
void func2 ();

extern int varl, var2;
int var8 = 0x33333333;
const int var9 = 0x12345678;
int varlO;

int varl = Oxllllllll;
int var2;
int var3 = 0;
int main() {
static int va r 4 =
0x22222222;
static int var5;
int var6;
printf("This is main()
function!\n");
fund () ;
func2 () ;

void fund () {
printf ( "This is fund ()
function!\n”);
printf ("varl = 0x%X,
var2=0x%X\n"z
varlz var2);
}
void func2() {
printf("This is func2 ()
function!\n");
}

return 0;
}

［그림 5-14］ 컴파일 명령 예

그러면 test와 main.o, funcs.o 같은 ELF 오브젝트 파일이 생성되는데, objdump -s

［ ELF 오브젝트명］과 같은 명령을 내리면 각 섹션의 내용을 볼 수 있다. ［그림 5-15］ 는
objdump -s test 명령으로 본 test ELF 바이너리의 .text 섹션에 들어있는 인스트럭션
이다.
［그림 5-15］ 에서 사각형으로 표시된 부분이 test ELF 바이너리의 .text 섹션 내용이다.
좌측에 8048xxx로 표현된 것은 해당 인스트럭션이 메모리상에 위치하는 주소를 의미
한다.

312 3부_ 컴파일과링킹

===== PAGE 314 =====
' root@os：/temp/ld

=1므12d

Contents 10f section .text:
801*8300 31ed5e89 e183e4F8 50545268 608^0408
8048310 68708404 98515668 d』*830408 e8a7ffff
804832 0 FfF49090 5589e!553 83ec04e8 00000006
8048330 5b81c3b8 1300008b 93FCFFFF FF85d274
80483U0 05e872FF FFFf585b c9c39890 90909090
8048350 5589e553 83ec8480 3dls9704 8800753F
804836 0 b81』l9604 082dl 096 0408C1F8 028d58FF
8048370 81149704 0839c376 1F8db426 00008000
8048380 83c001a3 14970488 FF148510 9604O8a1
8048390 14970408 39c377e8 C6051897 84080183
8048330 C4045b5d c38d7426 W8dbc27 00000880
80483bo S589e583 ec08ali8 96040885 C07412b8
80483c0 00800000 85co7489 C7042418 96O408FF
80483d0 d8c9c390 8d4c21»84 83e4F0FF 71Fc5589
88483e0 e55183ec 14c70424 30850408 e8F7Feff
80483f0 ffe81600 OOO0e844 000000b8 O0»
8048耳00 83c41459 5d8d61Fc C3909090 5589e583
8048418 ec18c784 24588504 08e8caFe Ffffa124
8048420 9704088b 15089704 08894424 08895424
8048430 04c70』<24 67850408 e89bfeFf fFc9c355
8048440 89e583ec 08c70424 7d850408 e897feff
8048450 FFc9c390 90909090 90909090 90909090
8048460 5589e55d c38d7426 008dbe27 00000080
8048470 5589e557 5653e85e 00000081 c36dl200
8048480 0883ec1c e807feff FF8d8320 FFFFFF89
8048498 45f08d83 28Ffffff 2945F0C1 7dF0028b
80484aO 55F085d2 742b31FF 89c68db6 80000000
80484b0 8b451083 C7B18944 24088b45 0c894424
80484C0 048t)4508 890424FF 1683c604 397df075
80484(18 dF83c41c 디b5e5F5d c38ble24 C39O9090
80484e0 5589e553 bb089604 0883ec04 al089604
80484F0 0883F8FF 740c83eb 04ffd98b 0383f8FF
8048508 75F>183c4 045b5dc3

I. ............ PTRh'____
hp...QUh
................ ..
....U..S
[................... ................ t
........
U..S....
=............u?
________ ..............X.
............ 9.U
A

H

....9.w.
u.................. ........... t..
................... • •$……
............ L$. ....q.U.
Q............$ 0..................
............... D
…V].a.
... .U...
.… $P..
..D$..T$
.. .$g...
............... U
.................$}....................

.........$

U..WUS.*

.....
■
----■• ■
..... ■
..... ■
■
.....
I
..... I
............ ID. . 리

Eaa■ «■■

-E........... D $..E..D$ ■
«aE«n
....9}.u ■
U..S....
....t...

El

：!

［그림 5-15］ objdump -s test 명령으로 본 test ELF 바이너리의 .text 섹션의 내용

.rodata 섹션은 C 소스 내에 포함된 문자열이나 const 변수와 같은 읽기 전용 데이터
가 위치하는 섹션이다. 그래서 objdump -s test 명령으로 .rodata 섹션 부분을 보면
［예제 5-9］ 의 소스 파일에 포함된 문자열들과 const int var9 같은 const 변수의 값이
위치한 것을 확인할 수 있다.
• bckddn@lksas：~/book/ld1
Contents oF section .rodata:
8048504
03000000
01800200
8048514
20697328
6d61696e
8048524
696f6e21
00008000
8048534
20697320
66756e63
8048544
74696f6e
21B07661
8948554
20766172
323d3078
8048564
20697320
66756e63
80485711 74696f6e 2100

80000898
p8292066
7856341기
31282920
72313d30
25580a00
32282920

___
5프瓦꺄
756e637|i|
54686973
66756e63
7825582c
54686973
66756e63

............................. This
is inainO Func 11
ion!
xU4.This
is Fund () Func
tion?.uar1=0x허X,
var2=0x허X..This
is
Func2()
Func
tion!.

［그림 5너6］ objdump -s test 명령으로 본 test ELF 바이너리의 .rodata 섹션의 내용

［그림 5-16］ 에서 사각형으로 표시된 부분이 var9 변수의 값이다. x86 아키텍처는 리틀
엔디안을 사용하기 때문에 Ox 12345678 과 같은 값이 0x78563412 와 같은 형식으로
보임에 유의하기 바란다.

5장_ Id linker 313

===== PAGE 315 =====
.data과 .datal 섹션은 초기화된 데이터가 잡히는 섹션이다. ［표 5-3］ 에서도 설명했듯
이 여기서 초기화되었다는 말의 의미는 C 소스에서 명시적으로 초기화되었다는 의미
보다는 0이 아닌 값으로 초기화되었다는 의미다.
이런 초기화된 데이터는 시스템 로더(exec 시스템 콜)가 프로세스를 생성할 때 메모리
로 그대로 읽어 들인다. 그래서 ［예제 5-9］ 의 main.c에 varl과 var4 같이 어떤 전역변
수 혹은 static 변수의 값을 C 소스에서 명시하면 해당 변수의 초기 값이 우리가 명시한
값을 가지고 있다는 걸 보장할 수 있다.
root@os：/temp/ld
Contents of section .data:
8 049704 OB00fl8flfl[ 11111111 22222222 33333335] ............................................................ 3333

［그림 5-17］ objdump -s test 명령으로 본 test ELF 바이너리의 .data 섹션의 내용

［그림 5-1 刀에서 보면 .data 섹션에 초기화된 전역변수 (varl, var8) 혹은 초기화된

static 변수(var5)의 값이 들어 있음을 확인할 수 있다.
.bss 섹션에는 초기화되지 않은 전역변수 혹은 static 변수의 값이 잡히는 섹션이다. 역
시 여기서도 초기화되지 않았다는 말의 의미는 0인 값으로 설정된 전역변수 혹은 static
변수를 의미한다.
그래서 ［예제 5-9］ 의 소스에서는 var2, var3, var5, varlO01 모두 .bss 섹션에 포함된다.

var3를 보면 지금껏 설명한 초기화된 변수 혹은 초기화되지 않은 변수의 의미를 명확
하게 알 수 있다.
［예제 5-9］ 의 main.c 소스에서 보면 var3가 0으로 명시적으로 초기화되었지만 0의 값
으로 설정된 전역변수 혹은 static 변수는 초기화되었다고 이야기하지 않는다. 0이 아
닌 초기 값으로 설정된 전역변수 혹은 static 변수만이 초기화되었다고 이야기한다. 때
문에 var3는 .bss 섹션에 위치한다.

.bss 섹션은 특이하게도 실제 ELF 바이너리에서는 공간이 할당된 섹션이 아니다. 섹션
헤더 테이블에서만 .bss 섹션의 헤더만 존재하고, 실제 ELF 바이너리 이미지에는 .bss
섹션의 공간이 할당되어 있지 않다.
대신 시스템 로더가 프로세스 이미지를 메모리에 만들 때 .bss 섹션에 해당하는 부분을
메모리에 할당하고, 모두 0으로 초기화한다. 이렇기 때문에 C 소스에 명시적으로 초기
값을 설정하지 않은 전역변수 혹은 static 변수의 값이 0의 값을 가진다는 것을 보장할

314 3부_ 컴파일과링킹

===== PAGE 316 =====
수 있는 것이다. 또한 이렇게 .bss 섹션의 영역을 ELF 바이너리 이미지에 할당하지 않
음으로써 ELF 바이너리의 사이즈를 줄일 수 있다.
이상으로 ELF 바이너리 포맷에 대한 거의 대부분의 중요한 내용은 설명이 끝났다. 무
척 단순한 포맷이라는 느낌이 들었다면 다행이다. 사실 ELF는 무척 단순한 구조를 가
지고 있다. 우리가 알아야 될 내용은 여기까지다. 나머지 각 섹션의 구조가 궁금하거나,
링커나 로더, 디버거를 만들어야 하는 독자가 있다면 pdf 파일 형태인 ELF 매뉴얼을
읽어보기 바란다. ELF 매뉴얼도 내용이 많지만 지금까지 배운 내용을 바탕으로 하나씩
따져보면 무척 간단하다는 것을 알 수 있을 것이다.

3Lid 를 사용한 링킹
이제 링킹 과정이 어떻게 되는지도 알았고 링킹을 이해하기 위한 기본 지식인 ELF 바
이너리 포맷도 알아보았다. 그러면 지금부터 실제 Id로 어떻게 링킹하는지 알아보자.
지금부터 다루는 내용은 Id를 사용한 기본 링킹 및 기본 옵션에 대한 설명이다.

I Id를 사용한 기본적인 링킹
다소 의아스러울 수도 있겠지만 실제 Id로 직접 링킹할 일은 그다지 많지 않다. 특히 애
플리케이션 프로그래밍을 할 때는 모듈 간 분리를 위해 부분 링킹하는 것 외에는 거의
없다고 보아도 무방하다.
그러면 왜 Id의 사용법을 알아야 되는 걸까? 그것은 애플리케이션 프로그래밍 외에 임
베디드 프로그래밍, 운영체제, 부트로더 같은 특수한 프로그램들은 Id로 직접 링킹해야
하기 때문이다. 그리고 메모리 최적화 등을 위해 XIP, 오버레이 등과 같은 특수한 기법
을 사용할 경우 반드시 Id로 직접 링킹해야 한다.
반드시 알 필요는 없지만 알아 두면 언젠가는 요긴하게 쓰이는 것이 Id를 사용한 링킹
방법이다. 고수는 컴파일 과정이나 시스템 성능 또는 메모리 사용량 최적화 과정에서
어떤 문제에 직면하면 Id를 사용한 링킹까지 고려할 수 있지만, 중수는 아는 데까지만
고려할 수밖에 없다. 비약이 좀 있지만 Id를 사용한 링킹 기법은 고수와 중수를 나누는
기준이라 볼 수도 있을 것 같다.

5장_ Id linker

315

===== PAGE 317 =====
그러면 본격적으로 Id를 사용한 각종 링킹 기법을 알아보자.

B Id를 사용한 애플리케이션 최종 링킹
최종 링킹은 재배치 가능한 오브젝트(예: main.o, funcs.o 등)들의 결합과 재배치 과정
을 통해 재배치 불가능한 오브젝트(예: test 실행 바이너리) 즉, 최종 실행 바이너리를
만들어 내는 과정이다.
이전 “gcc” 장에서 컴파일 과정을 설명할 때 최종 링킹되는 과정은 다음과 같았다.
〔예제 5-10)

/usr/libexec/gcc/i386-redhat-linux/4.1.2/collect2
-eh-frame-hdr -m elf_i386 -------------------------------------dynamic-linker /lib/ld-linux.so.2
o test
/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crtl.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crti.o
/usr/lib/gcc/i386—redhat-linux/4.1.2/crtbegin.o
-L/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2/../../ . .
main. o
funcs.o
-Igcc as-needed -丄gcc_s -------------------------------------------------- -Igcc --as-needed
丄gcc_s -------------------/usr/lib/gcc/i386-redhat-linux/4.1.2/crtend.o
/usr/lib/gcc/i386-redhat-linux/4.1.2/../../../crtn.o

collect』에 의한 애플리케이션 최종 링킹 과정은 다소 복잡하게 보일 것이다. 복잡하게
보이는 이유는 링킹 과정에서 사용되는 오브젝트 또는 라이브러리가 많이 있기 때문이
다. 각각의 오브젝트나 라이브러리의 용도는 “gcc” 장에서 컴파일 과정을 설명하면서
모두 설명하였다. 궁금한 독자가 있다면 “gcc” 장의 컴파일 과정을 읽어보기 바란다.

Id로 위 명령들을 일일이 지정해 최종 링킹할 수도 있다. 물론 그렇게 하면 gcc로 컴파
일하면서 링킹이 이뤄진 것과 동일한 결과물을 얻을 수 있다. 하지만 위와 같은 명령으
로 매번 애플리 케 이션을 최종 링 킹 한다면 다소 가혹하다는 느낌 이 든다.
［예제 5-1 이과 같이 번잡하게 최종 링킹할 필요 없이 다음과 같은 명령을 내리면 깔끔
하게 최종 링킹된다. 그전에 먼저 다음 명령을 사용하려면 main.o와 funcs.o가 만들어
져 있어야 한다. gcc -c *.c 명령 또는 gcc -o test main.c funcs.c -save-temps 명령
으로 먼저 main.o와 funcs.o를 만든 후 다음 명령을 내리기 바란다.

316 3부_ 컴파일과링킹

===== PAGE 318 =====
$ Id -dynamic-linker /lib/ld-linux.so.2 -o test /usr/lib/crtl.o
/usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c
j쩌 root@server：,work/book/utlls_new/ld
[rootBseruer Idjtt Is main.o funcs.o
Euncs.o main .o']
[root(흐seruer ld]tt______________________________________________________________
[rootBseruer Id]# Id -dynamic-linker /lib/ld-linux.so.2 —o t
est /usr/lib/crtl.o /usr/lib/crti.0 Zusr/lib/crtn.0 nain.o f
lines.o —1c____________________________________________________________________
[root@seruer Id]#
[rootBserver Id]# Is test
곤est I
[rootBseruer ld]tt
[root@seruer Id]# ./test
This is main() Function?
This is Fund() function?
uar1=0x11111111, uar2=0x0
This is Func2() function?
[rootBseruer Id]# |

[그림 5너8] Id 명령을 사용해 최종 링킹한 예

각 옵션을 살펴보면 다음과 같다. -dynamic-linker /lib/ld-linux.so.2 옵션은 동적 링
커로 /lib/ld-linux.so.2를 사용한다고 명시한 것이다. 이렇게 하면 .interp 섹션에 /lib/

ld-linux.so.2 동적 링커의 패스가 들어가 test 명령 수행 시 /lib/ld-lin니x.so.2를 test
애플리케이션의 메모리 주소 공간에 같이 로드해 먼저 수행한다.
이후 /lib/ld-linux.so.2 동적 링커가 test 실행 바이너리 실행에 필요한 공유 라이브러
리를 알아내고 해당 라이브러리들이 이미 메모리에 로드되어 있다면 로드된 공유 라
이브러리를 test 프로세스의 주소 공간에 맵핑하고, 아직 로드되어 있지 않다면 로드한
후 test 프로세스의 주소 공간에 맵핑 한다.

-dynamic-linker /lib/ld-lin니x.so.2 옵션으로 동적 링커를 /lib/ld-linux.so.2로 정해
주지 않았다면 Id는 -1c에 의해 /usr/lib/libc.so.l을 동적 링커로 인식하기 때문에 다음
과 같은 오류가 발생한다.
으 root@server：/work/book/utils_new,ld

[root@seruer ld]tt Id -0 test /usr/lib/crtl.0 /usr/lib/crti.0
/usr/lib/crtn.0 main.o Funcs.0 -1c
[root@seruer Id]#
[rootBseruer ld]tt ./test
-bash: ./test: /usr/lib/libc.so.1: bad ELF interpreter: 그런

파일이나 디렉토리가 없음
[root@seruer |

[그림 5-19] 동적 링커를 지정하지 않았을 때 오류 메시지

다음으로 -o test 옵션으로 최종 실행 바이너리명이 test임을 Id에 알리고, /usr/lib/

crtl.o /usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c를 링킹해 test 실행 바이너
리를 만든다.

5장_ Id linker

317

===== PAGE 319 =====
이전에 컴파일 과정에서 설명했지만 crtl.o, crti.o 는 crt function이라고 하며 main 함
수가 수행되기 전에 제일 처음 수행되는 초기화 코드들이 있는 오브젝트들이다. 이런
초기화 코드들은 main 함수보다 먼저 수행되어 애플리케이션이 수행될 환경을 조성한
다. 그리고 crtn.o 오브젝트에는 애플리케이션이 끝난 후에 종료를 처리하는 코드들이
들어 있다. crt*.o 파일들을 링킹해 주지 않았다면 test 애플리케이션은 제대로 동작하지
않았을 것이다.
이것으로 완벽하게 애플리케이션의 최종 링킹이 끝난 듯하지만 사실은 그렇지 않다. 그
것은 ［예제 5-10］ 에서 -Igcc와 -lgcc_s에 의해 링킹되는 libgcc.a와 libgcc_s.so에 관
련이 있다. 이전 “gcc” 장의 컴파일 과정 설명에서 아키텍처에서 지원하지 않는 연산
등이 C 소스 내에서 사용된 경우（예: ARM 아키텍처에서 c = a / b； 같은 나누기 연산
등）에 gcc는 이런 연산 등을 내부적으로 함수（예: c = __udivsi3（ a, b） ；） 호출로 바꾸고
컴파일 과정을 수행한다고 했었다. 그리고 최종 링킹 단계에서 이런 함수들이 들어있는

libgcc.a, libgcc_s.so 같은 라이브러리와 링킹함으로써 링킹 과정을 마무리 짓는다.
현재 test 애플리케이션에서는 이런 아키텍처에서 지원하지 않는 연산 등이 사용되지
않아 libgcc.a, libgcc_s.so 같은 라이브러리와 링킹할 필요가 없다. 하지만 아키텍처에
서 지원하지 않는 연산 등이 사용되어 gcc 내부 함수로 바뀌 었다면 libgcc.a와 libgcc_

s.so를 다음과 같이 반드시 최종 링킹 과정에서 추가해야 한다. 그리고 다음 명령에서
/usr/lib/gcc/i386-redhat-linux/4.1.2 는 필자가 사용하는 컴파일러의 라이브러리 디
렉토리다.
$ Id -L/usr/lib/gcc/i386-redhat-linux/4.1.2 -dynamic-linker /
lib/ld-linux.so.2 -o test /usr/lib/crtl.o /usr/lib/crti.o /usr/
lib/crtn.o main.o funcs.o -1c -Igcc -lgcc_s

지금까지 Id를 사용한 최종 링킹 방법을 알아보았다. 독자에게 미안한 말이지만 애플리
케이션을 최종 링킹할 때는 보통 이렇게 Id로 최종 링킹하지는 않는다. 본 예는 독자의
이해를 위해 Id로 최종 링킹한 예였다. 실제로는 다음과 같이 gcc 명령으로 최종 링킹
한다.
$ gcc -0 test main.o funcs.o

이렇게 gcc로 최종 링킹하는 이유는 main.o와 funcs.o를 컴파일한 컴파일러의 버전
에 따라 libgcc.a와 libgcc_s.so에 포함된 함수명 등이 다를 수 있기 때문이다. 예를 들
면 arm-lin니X-gcc에서 일반적으로 unsigned int형에 대한 나누기 연산자에 대응되는

318 3부—컴파일과링킹

===== PAGE 320 =====
함수는 __udivsi3() 함수지 만, GNU EABI (Embedded Application Binary Interface)
.모드루 컴파일된 arm-linux-gcc는 __aeabi_uidiv() 함수가 니nsigned "형 나누기 연
산자에 대응되는 함수다.

c = a / b;

그래서 위와 같은 나누기 연산에 대해 일반적인 arm-linux-gcc 는 위 연산을 c =

__udivsi3(a, b)；로 치환해 컴파일하지만 EABI 모드로 컴파일된 arm-linux-gcc는 위
연산을 c = __aeabi_uidiv(a, b)；로 치환해 컴파일한다.
때문에 어떤 컴파일러로 컴파일했는가의 문제는 어떤 libgcc.a와 libgcc_s.so에 링킹하
느냐의 문제로 결부된다. 반드시 libgcc.a와 libgcc_s.so는 컴파일할 당시의 컴파일러
에 포함된 libgcc.a와 libgcc_s.so에 링킹되어야 한다.
그래서 libgcc.a 와 libgcc_s.so 가 어떤 디렉토리에 있는지 알아야 하고, 해당 디렉토
리를 알고 있는 것은 Id 가 아니라 컴파일 명령에서 사용한 gcc 이기 때문에 Id 보다는

gcc 가 최종 링킹에서 사용되는 것이다. 그리고 컴파일러의 버전에 따라 crtl.o, crti.o,
crtn.o 같은 링킹해야 될 CRT 오브젝트의 종류도 다르다. 때문에 애플리케이션을 최종
링킹할 때에는 Id를 직접 사용해 최종 링킹하는 것보다 gcc를 사용해 최종 링킹하는 것
이 효율적이다.

tKff ABI (Application Binary Interface) 란?
ABI는 애플리케이션의 바이너리에 적용되는 일종의 규약이다. ABI의 종류에 따라 함수 호출 방식(프롤
로그 절차, 스택 사용 방식 등)이 다를 수 있고, 함수 호출 시 사용되는 레지스터(caller/callee saved
register)의 종류도 다를 수 있다.
함수 호출뿐만 아니라 데이터 타입의 사이즈, align 및 C++에서 함수 이름을 맹글링(mangling)하는 방
식, 기타 오브젝트 파일의 포맷 등과 같이 코드를 생성하는 전반적인 방식을 다루는 규약이 바로 ABI다.

지금까지 Id를 사용한 최종 링킹을 설명하였다. 다음으로 설명할 것들은 Id를 사용하기
위해 반드시 알아둬야 할 옵션들이다.
하지만 공교롭게도 Id의 옵션들은 많은 부분 gcc의 링커 옵션과 동일하다. gcc에서 링
킹을 위해 collect》를 호출하고 collect》에서 Id를 호출하기 때문에 어쩌면 그것은 당
연한 일일지도 모른다. 다른 문제는 없다.

5장_ Id linker

319

===== PAGE 321 =====
필자가 이전에 gcc 를 설명하면서 링커 옵션으로 설명했던 몇 가지 옵션을 다시 설명
해야 하는지 고민이 될 뿐이지만 말이다. 어쨌든 gcc 는 gcc 이고, Id 는 Id 이니 중복이
되더라도 gcc 과정을 건너뛰고 링킹 과정만 보고자 하는 독자를 위해 이전에 설명했
던 Id의 몇 가지 옵션을 다시 설명한다.

@ 니 옵션으로 링킹될 라이브러리 지정

링킹할 때 특정 라이브러리를 포함하려면 -1［라이브러리명］ 옵션을 사용한다. 이때 라
이브러리명은 libfl.so가 있을 때 앞에 있는 lib와 확장자인 .so를 떼어낸 fl만이 라이브
러리명이 된다. 참고로 fl 라이브러리는 GNU FLEX（스캐너）의 라이브러리다.
그래서 다음과 같은 명령으로 링킹하면 test 바이너리에 fl 라이브러리가 포함된다.
$ Id -dynamic-1inker /lib/ld-linux.so.2 -o test /usr/lib/crtl.o
/usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c -Ifl.

fl 라이브러리가 공유 라이브러리였다면 -Ifl 옵션에 의해 libfl.so가 링킹되지만, 정적
라이브러리였다면 libfl.a가 링킹된다. 정적 라이브러리이든 공유 라이브러리이든 GNU

FLEX 라이브러리를 링킹할 때는 -Ifl 옵션을 추가하면 된다. 그리고 정적 라이브러리와
공유 라이브러리가 동시에 존재한다면 Id 는 -static 옵션이 있지 않는 한 공유 라이브
러리를 링킹한다.

-1 옵션을 사용해 라이브러리를 링킹할 때 주의할 점은 -1 옵션은 반드시 소스보다 뒤
에 와야 한다는 점이다. 이렇게 해야 되는 이유는 Id가 C 소스에서 호출한 라이브러리
함수들을 라이브러리에서 찾을 때는 명령라인에서 입력을 기준으로 라이브러리를 한
번만 스캔해서 찾아, C 소스에서 참조하는 라이브러리 오브젝트를 링킹하기 때문이다.
때문에 -1［라이브러리명］ 옵션보다 뒤에 오는 오브젝트들에 대해서는 Id가 해당 라이
브러리의 심볼들을 리졸브하지 못하는 문제가 발생할 수도 있다.
무슨 말인지 이해가 안 되면 -1 옵션은 반드시 소스보다 뒤에 와야 한다는 것만 기억하
고 우선 넘어가자. 뒤에서 자세히 설명한다.

-1［라이브러리명］ 옵션과 동일한 옵션으로는 --library=［라이브러리명］ 옵션이 있다.

320 3부— 컴파일과 링킹

===== PAGE 322 =====
@ -L 옵션으로 라이브러리 검색 디렉토리 지정
-1［라이브러리명］ 옵션을 주면 Id는 기본적으로 /usr/i386-redhat-linux/lib, /usr/
local/lib, /lib, /usr/lib 디렉토리 순서로 라이브러리명에 해당하는 라이브러리가 있는
지 찾는다. -Itest 옵션을 주었는데 libtest.a 라이브러리가 /opt/lib 디 렉토리에 있어 라
이브러리를 찾지 못하면 Id는 오류를 출력할 것이다. 이때는 다음과 같이 -L［라이브러
리 디 렉토리 패스］ 옵션을 추가하면 된다.
$
Id
-L/opt/lib
-dynamic-linker
/lib/ld-linux.so.2
crtl.o /usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c -Itest

-o

test

/usr/lib/

-L ［라이브러리 디렉토리 패스］ 옵션은 여러 번 중복 사용할 수 있고, --librarypath=［라이브러리 디렉토리 패스］ 옵션과 동일하다.

E -static 옵션으로 정적 링킹
공유 라이브러리와 정적 라이브러리가 동시에 있는 경우 -static 옵션을 주면 정적 라
이브러리와 링킹한다. 그래서 다음과 같이 명령을 내리면 모든 라이브러리를 정적 링킹
한다.
$ Id -static -L/usr/lib/gcc/i386-redhat-linux/4.1.2 -o test
/usr/lib/crtl.o
/usr/lib/crti.o
/usr/lib/crtn.o
-\( -Igcc -lgcc_eh -1c -\)

main.o

funcs.o

정적 링킹을 할 때는 물론 포함되는 모든 라이브러리의 정적 라이브러리가 있어야 한
다. 위 명령에서 주의 깊게 보아야 할 것은 -\( -Igcc -lgcc_eh -lc -\) 부분이다.
이전에는 -static 옵션을 주지 않고 최종 링킹할 때는 -\( 옵션과 -\) 옵션이 포함되지
않았었다. -\( 옵션과 -\) 옵션은 두 옵션 사이에 오는 라이브러리들에 대해 참조하는
심볼을 완전히 찾을 때까지 라이브러리들을 계속 스캔하면서 찾는 옵션이다.
이렇게 하는 이유는 Id가 기본적으로 정적 라이브러리에 있는 오브젝트를 링킹하고자
할 때는 명령라인에서 주어지는 순서대로 한 번만 스캔하면서 심볼의 참조를 찾고, 해
당 심볼을 정의하는 정적 라이브러리 내의 해당 오브젝트만 링킹하기 때문이다.
그런데 문제는 뒤에 오는 다른 라이브러리에서 이전에 링킹한 정적 라이브러리 내 링
킹되지 않은 오브젝트를 참조하고자 한다면 해당 오브젝트는 링킹되지 않았기 때문에
심볼을 찾지 못하는 문제가 발생할 수 있다.

5장_ Id linker 321

===== PAGE 323 =====
다음 그림은 -\（ 옵션과 -\） 옵션을 제거했을 때 발생하는 오류 메시지다.
퍼 root@server：/work/book/utils_new/ld
to __ ___________________________
/usr/lib/libc.a(fileops.o): In function '_IO_File_underflow':
(.text+0x14가)): undefined reference to '_Unwind_Resime'
/usr/Mb/libc.a(Fileops.0): In Function '_IO_File_Fopen‘:
(.text+8x1cd7): undefined reference to '_Unwind_Resuine'
/usr/lib/libc.a(Fileops.o):(.eh_Frane+0xde): undefined reference
to __ ___________________________
/usr/lib/libc.a(iogetdelim.o): In function 'getdelim':
(.text+0x26c): undefined reference to 'UnwindResume'
/usr/lib/libc.a(iogetdelim.o):(.eh_frame+0xde): undefined reFeren
ce to ___ ___________________________
[rootSseruer ld]tt |

j

[그림 5-20] -\（ 옵션과 -\） 옵션을 사용하지 않았을 때 오류 메시지

이런 문제를 해결하려면 -\（ 옵션과 A） 옵션을 사용해 여러 번 스캔하면서 심볼의 참
조를 찾고 해당 심볼을 정의하는 정적 라이브러리 내의 오브젝트를 링킹하는 일을 해
주어야 한다.

-\（ 옵션과 -\） 옵션 대신 一start-group 옵션과 --end-group 옵션을 사용해도 무
방하다. 다음은 -static 옵션으로 정적 링킹한 예다.
주 root@server：7work/book/utils_new/ld
[rootBseruer ld]tt Id[-static]-C/usi^iib/gcc/i386-redhat-linux/4.l|
.2 -o test /usr/lib/crtl.o /usr/lib/crti.o /usr/lib/crtn.o main.o
Funes.0 start-group -Igcc -lgcc_eh -1c --------------------------------------------------------[rootSseruer ld]tt
[rootSseruer ld]tt ./test
This is main() Function*
This is func1() Function?
uar1=8x11111111, uar2=0xO
This is func2() function?
[root@seruer ld]tt |

[그림 5-21] -static 옵션으로 정적 링킹한 예

@ -shared 옵션으로 공유 라이브러리와 링킹
-shared 옵션을 사용하면 정적 라이브러리와 공유 라이브러리가 동시에 있을 때 공
유 라이브러리와 링킹한다. 이 옵션은 -static 옵션이 있지 않으면 기본적으로 활성화
되어 있는 옵션이기 때문에 이전까지 -static 옵션을 주지 않고 링킹한 것들은 모두

-shared 옵션이 켜져 있었다고 생각하면 된다.

322 3부_ 컴파일과 링킹

===== PAGE 324 =====
0-r 옵션으로 부분 링킹하기
대부분의 경우 Id를 사용해 직접 링킹하는 경우는 운영체제, 부트로더 같은 프로그램을
링킹할 때 링커 스크립트로 바이너리 맵을 직접 설정할 경우와 애플리케이션의 모듈화
를 위해 부분 링킹하는 경우다.
부분 링킹은 재배치 가능한 오브젝트들을 링킹해 하나의 큰 재배치 가능한 오브젝트로
만드는 과정이다. 이렇게 링킹된 재배치 가능한 오브젝트는 나중에 다시 링킹될 수 있
다. 예를 들면 다음과 같은 경우다.

［그림 5-22］ Id를 사용한 부분 링킹 예

［그림 5-22］ 에서 음영 처리된 부분이 부분 링킹에 해당한다. Id 명령은 다음과 같다.
$ Id -r -o sub.o memo.o calendar.o

-O 옵션 뒤에 오는 sub.o 가 부분 링킹 후 출력할 오브젝트 파일이고, 뒤에 오는
memo.o 와 calendared} 입력 오브젝트 파일이다. 부분 링킹을 할 때는 이렇게 -r 옵
션을 붙여주면 된다. 그러면 입력으로 넣어주는 재배치 가능한 오브젝트 파일들을 하나
의 큰 재배치 가능한 오브젝트 파일로 만들어준다. 이렇게 만들어진 큰 재배치 가능한
오브젝트 파일은 나중에 다시 링킹될 수 있다.
그러면 이게 어떻게 프로그램의 모듈화에 이용될 수 있을까? ［그림 5-22］ 의 예제만 봐
서는 그다지 마음에 와 닿지 않을 것이다. 간단한 운영체제 소스를 예로 들어보겠다.

5장_ Id linker 323

===== PAGE 325 =====
위 그림은 MyOS라는 프로젝트의 디렉토리 구조를 보여준다. 음영으로 표시된 부분은
디렉토리를 의미하고 그렇지 않은 부분은 파일을 의미한다. 그래서 MyOS 프로젝트 디
렉토리에는 common과 fs, net 디 렉토리가 있고, common 디 렉토리는 arch 디 렉토리
와 schedulers라는 파일로 이뤄진 것을 확인할 수 있다. 위와 같은 프로젝트가 있다면
링킹 과정에서 다음과 같이 모듈화할 수 있다.

1. 먼저 i386.S 파일과 arm.S 파일 중 하나를 gcc ［기타 필요 옵션］ -c ［소스 파일명］
-o arch.o 명 령으로 컴파일해 arch.o 파일을 만든다.
2. 그리고 scheduler.c 파일을 gcc ［기타 필요 옵션］ -c ［소스 파일명］ -o
s사led니ler.o 명령으로 컴파일해 scheduler.o 파일을 만든다.
3. arch.o와 scheduler.o를 Id ［기타 필요 옵션］ -r arch.o scheduler.o -o
common.o 명령으로 컴파일해 common.o를 만든다.
4. 이후 같은 식으로 file.c를 gcc ［기타 필요 옵션］ -c file.c -o file.o 명령으로 컴파
일해 file.o로 만들고 ext3.c를 gcc ［기타 필요 옵션］ -c ext3.c -o ext3.o 명령으
로 컴파일해 ext3.o로 만든다.

5. 마찬가지로 이렇게 만들어진 file.o와 ext3.o를 Id ［기타 필요 옵션］ -r file.o
ext3.o -o ext3.o 명령으로 컴파일해 ext3.o를 만든다.
6. 계속 이런 식으로 범위를 넓혀 가면서 부분 링킹해 나가면 최종적으로 common,
o와 fs.o, net.o가 생성되는데, 마지막으로 -r 옵션을 제거한 Id ［기타 필요 옵션］
common.o fs.o net.o -o MyOS 명령을 내리면 최종 링킹할수 있다.

324 3부— 컴파일과 링킹

===== PAGE 326 =====
다소 복잡하게 느껴지겠지만 실제로 해 보면 그다지 복잡하지도 어렵지도 않은 과정이
다. -r 옵션을 사용하면 각각의 오브젝트를 좀 더 큰 덩어리로 부분 링킹하면서 오브젝
트를 모듈별로 분리하는 것이 가능해진다.
이상 지금까지 설명한 것들이 Id를 사용할 때 반드시 알아 두어야 할 옵션들이다. 다음
부터 설명할 것은 알아 두면 유용한 Id의 옵션들이다.

I 알아 두면 유용한 Id 옵션
Id의 옵션들은 무척이나 많다. 지금부터 설명할 옵션들은 그 중에서 제법 많이 사용되
는 Id의 옵션들이다.

D -M, —-print-map, -Map 옵션으로 링크 맵 출력
링킹된 바이너리의 링크 맵이 궁금한 사람들이 있을 것이다. -M 옵션을 추가해 링킹하
면 링킹된 바이너리가 어떻게 링킹되었는지 자세한 정보를 출력한다.
$
Id
-M
-dynamic-linker
/lib/ld-linux.so.2
/usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c

-o

test

/usr/lib/crtl.o

다음 예는 위 명령을 내렸을 때 출력되는 링크 맵 정보에서 .data 섹션 부분만 보여준
다. 다음 예에서 확인할 수 있듯이 링킹 시 사용된 오브젝트들의 .data 섹션이 어떤 주
소에 위치하며, 포함되는 심볼들은 무엇인지에 대한 정보가' 자세히 출력됨을 확인할 수
있을것이다.
I〔예제 5-11) ® M 옵션으로 출력되는 .data 섹션 예
... 상략

. data
*(.data
. data

. data
.data
.data
.data
. data

0x080495a4
.data.* .gnu.
0x080495a4
0x080495a4
0x080495a4
0x080495a8
0x080495a8
0x080495a8
0x080495a8
0x080495b0
0x080495b0
0x080495b4

0x10
linkonce.d.*)
0x4 /usr/lib/crtl.o
data_start
__data_start
0x0 /usr/lib/crti.o
0x0 /usr/lib/crtn.o
0x8 main.o
varl
0x4 funcs.o
var8
0x0 /usr/lib/libc nonshared.a(elf-init.oS)

... 하략

5장_ Id linker

325

===== PAGE 327 =====
-M 옵션은 —print-map 옵션과 동일하고 -Map ［맵 파일명］ 옵션을 주면 링크 맵을
표준 출력 대신 인자로 주는 맵 파일명에 출력한다.
@ -s 또는 -S 옵션으로 심볼 정보 제거

-s 또는 一 strip-all 옵션을 사용하면 링킹된 오브젝트에서 심볼 정보를 제거할 수 있
다. 이렇게 하면 파일의 사이즈를 많이 줄일 수 있다. 심볼 정보를 제거하더라도 프로그
램 수행에는 지장이 없다. 단지 나중에 설명할 바이너리 유틸리티를 사용한 각종 정보
를 확인하는 것이 어려울 뿐이다. -S 또는 一 strip-debug 옵션을 사용하면 디버거 심
볼 정보만 제거할 수 있다.
쌔 root@s 이 wr：/work/bool으 utils_new/ld

싀믜씌

[root@seruer Id]# Id -dynamic-linker /lib/ld-linux.so.2 -o test
usr/lib/crtl.0 /usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c
[root@seruer Id]#
[root@seruer ld]tt Is -al test
-rwxr-xr-x 1 root root |4263| 6월 1 04:02 test
[root@seruer Id]#
[root@seruer
usr/lib/crtl.o

ld]tt
Id
/usr/lib/crti.o

三丁

-dynamic-linker
/usr/lib/crtn.o

/lib/ld-linux.so.2
main.o

-o
test
funcs.o

/
-1c

[root@seruer ld]tt
[root@seruer Id]# Is -al test
-rwxr-xr-x 1 root root |2740| 6월 1 04:02 test
[root@seruer ld]tt |

버
［그림 5-24］ -s 옵션을 추가했을 때 파일 사이즈의 변화

@ -X 또는 -X 옵션으로 지역 심볼 제거

지역 심볼은 외부로 export 되지 않는 심볼들을 말한다. 이런 심볼들은 다른 오브젝트
에서 참조하지 않기 때문에 제거해도 관계없다. -x 옵션은 모든 지역 심볼을 제거하
고, -X 옵션은 모든 임시 지역 심볼을 제거한다. 임시 지역 심볼이란, 컴파일러가 컴파
일 과정에서 문자열 등의 참조를 위해 임시로 생성한 심볼이다. 임시 지역 심볼은 보통

.LC［숫자］:와 같은 형식이고, -save-temps 옵션을 주고 컴파일한 후 main.s 파일을 열
어보면 다음과 같은 임시 지 역 심볼을 확인할 수 있다.
〔예제 5-12〕 main.s 파일의 임시 지역 심볼

... 상략
.LCO:

.string "This is main() function!
... 하략

［예제 5-12］ 에서 .LCO：와 같은 것이 바로 임시 지역 심볼이다.

326 3부- 컴파일과링킹

===== PAGE 328 =====
B --oformat 옵션으로 출력 바이너리 포맷 지정
—oformat ［바이너리 포맷］ 옵션으로 출력되는 바이너리 포맷을 지정할 수 있다. 지정
가능한 바이너리 포맷은 objdump -i 옵션으로 확인할 수 있는데, 필자의 경우 다음과
같다.
〔예제 5-13］

objdump -i 명령으로 알아본 지정 가능한 바이너리 포맷

... 상략

elf32—i386 a.out—i386—linux efi-app-ia32 elf32-little elf32-big
i386 elf32-i386 a.out-i386-linux efi-app-ia32 elf32-little elf32-big

i386

srec symbolsrec tekhex binary
srec
symbolsrec
tekhex

ihex trad-core
binary
ihex -----------

...하략

자세히 보면 인텔 헥사 포맷 (ihex) 도 있고, 모토로라의 S-record(srec) 포맷도 보일
것이다. 이 중 자주 사용되는 것은 순수한 바이너리를 나타내는 binary 포맷이다. Id 옵
션으로 —oformat binary 옵션을 주면 ELF 바이너리 포맷에서 프로그램 수행에 필요
한 섹션만 뽑아 순수한 바이너리를 출력한다. 이때 출력되는 바이너리는 ELF 바이너리
가 아니다. 인스트럭션과 데이터로만 이루어진 순수한 플랫 바이너리(flat binary)다.

—oformat 옵션으로 바이너리 포맷을 지정하는 것은 주로 임베디드 시스템 프로그램
에서 사용되고 일반 애플리케이션에서는 거의 사용되지 않는다. 그리고 애플리케이션
에서 사용하더라도 거의 대부분 심볼 관련 오류가 발생할 것이다.

同 -rpath 옵션과 -rpath-link 옵션으로 공유 라이브러리 검색 패스 추가

-rpath ［디렉토리 패스］ 옵션은 -L［디렉토리 패스］ 옵션과 비슷하게 라이브러리 검색
패스를 추가한다. 다른 점이 있다면 -L 옵션은 공유 라이브러리와 정적 라이브러리 모
두를 찾는 기본 패스를 추가하지만 -rpath는 공유 라이브러리 검 색 패스만 추가한다는
것이다. 그리고 -rpath와 -L 옵션이 동시에 사용되면 -L 옵션은 무시된다.

-rpath-link ［디렉토리 패스 또는 패스들］ 옵션 역시 공유 라이브러리 검색 패스를 추
가한다. -rpath-link의 인자는 하나의 디 렉토리 패스 또는 ‘:’으로 구분된 디 렉토리 패
스 리스트를 줄 수 있다. -rpath-link 는 여러 번 사용될 수 있고 -rpath-link /root ： /

tmp：/opt/lib 같이 리스트로 한꺼번에 여러 검색 디렉토리를 추가할 수도 있다.

5장_ Id linker 327

===== PAGE 329 =====
@ -e 또는 ——entry 옵션으로 엔트리 포인터 설정
엔트리 포인터는 프로그램이 로드되고 제일 처음 수행할 주소를 의미한다. 일반적으로
애플리케이션의 엔트리 포인터는_start 심볼로 설정되어 있다. 이후 _start에서 main()
함수를 호출한다.
애플리케이션의 엔트리 포인터가 _start로 설정되어 있는 것은 나중에 배울 Id가 ELF
바이너리의 모양을 잡을 때 참조하는 기본 링커 스크립트에서 엔트리 포인터를 _start
로 설정하고 있기 때문이다.
엔트리 포인터를 변경하면 제일 처음 수행할 주소를 바꿀 수 있다. 예를 들면 다음과
같이 링킹하면 엔트리 포인터를 _start 대신 func2로 바꾼다. 그래서 프로그램을 수행
하면 func2() 함수부터 수행된다.
$
Id
-dynamic-linker
/lib/ld-linux.so.2
usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c -e func2

-o

test

/usr/lib/crtl.o

/

$
Id
-dynamic-1inker
/lib/ld-linux.so.2
-o
usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c --entry=func2

test

/usr/lib/crtl.o

/

또는

다음 그림은 엔트리 포인터를 f니nc2로 했을 때 실제 수행되는 모습이다.
-[□I 시
IrrootBserver ld]tt Id -dunamic-linker /lib/ld-linux.so.2 —o test /Bl
[usr/lib/crtl.o yusr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -lcH|

|[root@seruer ld]tt ./test
[This is func2() function?)

세그멘테이션 ◎쥬
[root@seruer Id]# |

[그림 5-25] 엔트리 포인터를 func2로 변경

위 그림에서 알 수 있듯이 main() 함수가 먼저 호출되지 않고 func2() 함수가 먼저 호
출된 것을 확인할 수 있다. 그리고 func2() 함수 수행 후 리턴되는 과정에서 리턴 주소
가 올바르지 않아 세그먼테이션 오류가 발생한 것도 확인할 수 있다.
엔트리 포인터를 변경하는 일은 애플리케이션에서는 거의 일어나지 않지만 운영체제,
부트로더 등과 같은 프로그램들을 빌드할 때 가끔 사용되곤 한다.

328 3부- 컴파일과 링킹

===== PAGE 330 =====
8 ——section-start 또는 -T［ text|data|bss］

옵션으로 섹션 위치 지정

섹션의 위치를 지정할 때는 一section-start ［섹션명］ = ［주소］ 옵션을 사용한다. 이때
주소는 16진수를 사용한다.
이와 비슷한 옵션으로 -Ttext ［주소］, -Tdata ［주소］, -Tbss ［주소］ 옵션이 있는데, 각
각은 .text 섹션과 .data 섹션, .bss 섹션의 주소를 결정한다.
이렇게 섹션의 위치를 옵션으로 지정하는 경우는 운영체제나 부트로더 같은 시스템 소
프트웨어 빌드 시 간혹 사용되는 방식이다. 다음은 -Ttext 0x0 옵션으로 .text 섹션의
위치를 o번지로설정한예다.
$
Id
-Ttext
boot.o net.o

0x0

-s

--oformat

binary

-e

startup

-o

bootld

startup.o

@ -T ［링커 스크립트 패스］ 옵션으로 기본 링커 스크립트 변경
-T ［링커 스크립트 패스］ 옵션을 사용하면 Id가 출력 파일 생성 시 사용하는 기본 링커
스크립트를 변경할 수 있다. 이에 대해서는 바로 다음에 올 “링커 스크립트” 절에서 제
대로 알아본다. 사용 예는 다음과 같다.
$
Id
-T
test.Ids
-dynamic-linker
lib/crtl.o /usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c

/lib/ld-linux.so.2

-o

test

/usr/

0 —wrap 옵션을 사용한 래퍼 함수의 사용
간혹 소스에서 사용된 함수를 래퍼 함수로 호출해야 할 일이 발생할 수 있다. 이때는

-wrap ［함수 심볼명 ］ 옵션을 사용해 간단히 그 일을 수행할 수 있다.
〔예제 5너4〕 main.c 소스 파일 내용

#include <stdio.h>
int main() {
char *p;
p = (char *)malloc(10);
return 0;
}

예를 들면 위와 같은 main.c 소스 파일이 있을 때 main.c에서는 mallocO 함수를 내부
에서 호출한다. 이때 mallocO 함수를 래퍼 함수로 호출하고 싶다면 다음과 같이 한다.

5장_ Id linker 329

===== PAGE 331 =====
〔예제 5-15)

main.c 소스 파일 내용

#include <stdio.h>
^include <stdlib.h>
int

main() {
char *p;
p = (char *)malloc(10);
return

0;

}

void *______ wrap__malloc (int c) {
void *q = 0;
printf("wrapper malloc start! p = 0x%X\n”, q);
q = (void *)________real_malloc (c) ;
printf("wrapper malloc end! p = 0x%X\n”, q);
return q;
}

먼저 래퍼 함수를 추가한다. 래퍼 함수의 이름은 __wrap_［ 함수명］이 된다. 그리고 래
퍼 함수 내에서는 실제 함수를 호출하는데, 이때는 __real_［ 함수명］이 실제 함수를 호
출하는 부분이 된다.
그 래 서 m al loc ( ) 함 수 의 래 퍼 함 수 는 __wr a p_malloc() 함수가 되고, _wrap_

malloc() 함수 내에서 malloc() 함수를 호출하는 부분은 __real_malloc() 부분이 된다.
위 소스를 컴파일하는 방법은 다음과 같다.
$ gcc -c main.c
$
Id
-dynamic-1inker
/lib/ld-linux.so.2
usr/lib/crti.o /usr/lib/crtn.o main.o -1c --wrap malloc

-o

test

/usr/lib/crtl.o

/

또는

$ gcc -o test main.c -W1z--wrap,malloc

위와 같이 명령을 내려 컴파일 후 실행해 보면 다음 그림과 같이 malloc() 함수 호출이
래퍼 함수인 _Yrap_malloc() 함수 호출로 바뀐 것을 확인할 수 있을 것이다.

330 3부_ 컴파일과 링킹

===== PAGE 332 =====
주 root@server：/work/book/utils_new/ld
[rooteseruer ld]tt gee -c main.c
[root@server ld]tt Id -dynamic-linker /lib/ld-linux.so.2 —o test /
usr/lib/crtl .o /usr/lib/crti .0 /usr/lib/crtn .0 main .0 — 1c [三히히
malloc'l
[root@seruer Id]#
[root@seruer ld]tt
[root@seruer Id]# ./test
wrapper malloc start? p = 0x0
wrapper malloc end! p = 0X855AOO8
[rooteseruer Id]# |

［그림 5-26］ 래퍼 함수의 호출

｛回 - -trace-symbol 옵션으로 심볼 정의 및 참조 찾기

--trace-symbol= ［심볼명］ 옵션은 심볼의 정의 및 참조를 찾는 데 유용하다. 예를 들
면 puts 심볼을 어떤 라이브러리 혹은 오브젝트에서 정의하거나 참조하는지 알고자 할
때는 다음과 같이 사용한다.
$
Id
-static
—L/usr/lib/gcc/i386—redhat-linux/4.1.2
lib/crtl.o
/usr/lib/crti.0
/usr/lib/crtn.o
main.o
funcs.o
-lgcc_eh -1c -\) --trace-symbol=puts

-o
-\

test
(

/usr/
-Igcc

1* root@server：/work/book/utils_new/fd
[rootaseruer ld]tt Id -static -L/usr/lib/gcc/i386-redhat-linux/H.1
.2 -o test /usr/lib/crtl.0 /usr/libgcrti.0 /usr/lib/crtq.o main.o
funcs.0 —乂( -Igcc -lgcc_eh -1c -1*、) |-—trace—syr>bol=puts |
main.o: reference to puts
Funcs.0: reference to puts
/usr/lib/libc.a(ioputs.o): definition of puts
[root@seruer Id]#|

I커
[그림 5-27] --trace-symbol 옵션의 사용

그러면 위 그림과 같이 puts 심볼을 main.o와 funcs.o에서 참조하며, /usr/lib/libc.a에
있는 ioputs.o에서 정의한다는 것을 확인할 수 있다. --trace-symbcJ은 여러 번 사용
할 수 있으며, -y ［심볼명］ 옵션을 사용해도 동일한 결과를 얻을 수 있다.
하지만 이 명령을 너무 철석같이 믿지는 마라. 라이브러리와 관련해서는 라이브러리가
해당 심볼을 정의하고 있어도 해당 심볼을 못 찾을 수도 있다. 그 이유는 바로 다음에
오는 --start-group 옵션을 설명하면서 이야기하도록 하겠다.
마지막으로 --trace-symbol 옵션은 --trace 옵션과 함께 사용하면 좀 더 많은 정보
를 알아낼 수 있다. —trace 옵션은 현재 작업 중인 오브젝트가 무엇인지 출력한다.

5장_ Id linker

331

===== PAGE 333 =====
Q) ——start-group, ——end-group 옵션을 통한 심볼 참조 오류 해결
이전에 -static 옵션을 설명할 때 --start-group 옵션과 --end-group 옵션을 잠깐
언급했는데, 다소 모자란 감이 있어 다시 설명한다.
이런 경험이 있는 독자가 있는지 모르겠다. 예를 들면 정적 라이브러리(*.a)들을 링킹
하려고 했는데, 해당 정적 라이브러리들에는 분명히 어떤 심볼이 정의되어 있음에도

undefined reference to '심볼명’ 오류가 뜨는 경우 말이다. 그런 일이 없으리라 생각
하겠지만 의외로 자주 발생한다.
이 문제가 발생하는 이유는 Id가 정적 라이브러리를 링킹하는 방식과 관련이 있다. 이
해가 쉽도록 다음 명 령을 예로 들어 설명한다.
$
Id
lib/crtl.o
-lgcc_^h -1c

-static
—L/usr/lib/gcc/i386-redhat-linux/4.1.2
/usr/lib/crti.o
/usr/lib/crtn.o
main.o

-o

test
funcs.o

/usr/
-Igcc

나중에 라이브러리를 만들 때 자세히 설명하겠지만 정적 라이브러리(*.a)는 여러 오브
젝트 (*.o) 파일을 하나로 묶어 놓은 형태다. 여기서 정적 라이브러리는 -Igcc, -lgcc_

eh, -1c 에 해당하는 libgcc.a, libgcc_eh.a, libc.a이다. 이 모두는 각각 여러 개의 오브
젝트가 묶여진 형 태다.

Id는 라이브러리를 링킹할 때 명령라인에서 입력되는 오브젝트와 라이브러리 순서대
로 딱 한 번만 스캔하면서 참조되는 심볼을 찾고, 해당 심볼을 정의하고 있는 정적 라
이브러리 내에 해당 오브젝트만 링킹을 수행한다. 위 명령에서는 crtl.o, crti.o, main.o,

funcs.o, libgcc.a, libgcc_eh.a, libc.a순으로 스캔하면서 참조하는 각종 심볼들을 찾고,
정적 라이브러리에서 해당하는 심볼을 정의하는 오브젝트가 있는지 찾고, 있다면 해당
오브젝트만 링킹한다. hmcs.o까지 스캔했는데 libgcc.a에서 정의한 심볼을 이전에 한
번도 참조하지 않았다면 libgcc.a에 들어있는 어떤 오브젝트도 링킹되지 않는다.
문제는 뒤에 오는 libc.a에 있는 어떤 오브젝트가 이전에 main.o에서 참조된 심볼을 정
의하고 있어 링킹되는 오브젝트가 libgcc.a에 있는 오브젝트에서 정의하는 심볼을 참
조한다면 libgcc.a에 있는 어떤 오브젝트도 링킹되지 않았기 때문에 심볼을 찾을 수 없
는 오류가 발생한다는 점이다. 실제로 해당 심볼은 libgcc.a에 있는데도 말이다.
이런 경우 임시방편으로 -1c 옵션과 -Igcc 옵션의 순서를 바꾸면 해결되기도 한다. 하지
만 순서를 바꾸었는데, 이제는 libgcc.a에서 링킹되는 오브젝트가 libc.a에 존재는 하지만
이전 참조가 없어 링킹되지 않은 오브젝트의 심볼을 참조한다면 순서를 바꾸어도 아무

332 3부— 컴파일과 링킹

===== PAGE 334 =====
소용이 없다. 이런 경우를 교차 참조라 하는데, 딱 앞의 예제가 교차 참조의 좋은 예다.

libgcc_eh.a에 들어있는 unwind-c.o에는 __gcc_personality_vO 심볼을 정의하고
있다（의심스러우면 nm [libgcc_eh.a 패스] 명령으로 확인해 보기 바란다）. 하지만

unwind-c.o에 있는 어떤 심볼도 이전에 참조하지 않았기 때문에 unwind-c.o는 링킹
되지 않는다. 문제는 libc.a에서 링킹되는 각종 함수들의 오브젝트에서 unwind-c.o에
있는 __gcc_personality_vO를 참조하는데, unwind-c.o가 링킹되지 않았기 때문에 다
음 그림과 같은 오류 메시지가 발생한다.
旗 root@server：/work/book/utils_new/ld
/usr/lib/libc.a(wFileops.o): In Function 'lOwfileunderFlow':
(.text+0x1224): undefined reference to '_Unwind_Resime1
/usf/lib/libc.3(»£1180目5.인):(.eh frame+8xde): undefined reference
to I’‘ qcc_per5onality_u0,]
/usr/lib/libc.흐(Fileops.o): In Function '_IO_file_underflow':
(.text+0x14ab): undefined reference to '_Unwind_Resime*
/usr/lib/libc .a(fileops.o): In function ' lO File fopen':
(.text+8x1cd7): undefined reference to '_Unwind_Resmne1
/u완71ib/libc ,a나::ileops.o} :( .eh Frane*8xde): undefined reference
to |'_ .gcC—personalitj/Jja1 j
/usr/lib/libc.a(iogetdelim.o): In function 'getdelim1:
(.text+0x26c): undefined reference to '_Unwind_Resune‘
/usr/^ib/libc.a(ioqetdelim이):(.eh frame*flxde): undefined reFeren
ce to p_ gcc personality uB’l
[roothseruer Id]# |

[그림 5-28] 심볼 참조 오류 발생

다른 심볼 참조 오류 메시지도 발생하는데, 모두 비슷한 상황에서 발생하는 오류 메시
지다. 그러면 -1c 옵션과 -lgcc_eh 옵션의 순서를 바꾸면 괜찮을까?
i/3 mot@serwr:/work/book/utils_new/ld

J □! 시

n Function '.L413':
(.text+0x1896): undefined reference to |'_stack_chk_Fail_local'|
/usr/lib/gcc/i386-redhat-linux/4.1.2/libgcc_eh.a(unwind-dw2.o): I
n Function '_Unwind_Backtrace':
______ _________________________
(.text+OxIcel): undefined reference to |* stack_chk_Fail_local,'|
/usr/lib/gcc/i386-redhat-linux/4.1.2/lAjgcc_eh.a(unwind-dw2.o)I
n Function '_Unwind_RaiseException*:
(.text+0x1F43): undefined reference to r_stack_chk_fail_local*|
/usr/lib/gcc/i386-redhat-linux/4.1.2/li'bqc(三.eh.a(unGind-dw2.o).
text+8x2155): nore undefined references to |T_stack_chk_Fa:il_loca
1' Follow
/usr/lib/gcc/i386-redhat-linux/n.1.2/libgcc_eh.a(unwind-dw2-fde-g
libc-o): In function '_Unwind_Find_FDE':
(.text+9x1508): undefined reference to 'dl_iterate_phdr‘
[root@seruer ld]tt |

거

[그림 5-29] -lgcc_eh 옵션과 -Ic 옵션의 순서를 바꾸었을 때 오류 메시지

위 그림에서 알 수 있듯이 이제는 __stack_chk_faiLlocal 심볼을 찾을 수 없다는 오류
가 발생한다. __stack_chk_fail_local 심볼은 nm /usr/lib/libc,a 명령으로 확인해 보면

libc.a에 들어 있는 stack_chk_fail_local.o 오브젝트에 정의되었음을 알 수 있다. 문제는
libc.a에 있는 오브젝트들이 링크될 때 이전에 stack_chk_fail_local.o에서 정의하는 심
볼을 참조하지 않아 stack_chk_fail_local.o가 링킹에 포함되지 않았다.

5장_ Id linker

333

===== PAGE 335 =====
그런데 Iibgcc_eh.a에서 링킹되는 오브젝트가 참조하고 있으니 당연히 심볼을 찾지 못
하는 오류가 발생한다.
이 렇게 오도 가도 못하는 상황일 때 一 start-group 옵션과 一 end-group 옵션을 사
용하면 된다. 一 start-group 옵션과 -- end-group 옵션은 두 옵션 사이에 있는 정적
라이브러리에 대해서는 한 번이 아니라 여러 번 스캔하면서 심볼 참조를 찾아내고, 해
당 심볼을 정의하고 있는 오브젝트들을 링킹에 포함시킨다.
그래서 이전에 오류가 발생했던 링킹 명령과 달리 다음과 같이 링킹 명령을 내려주면
오류가 발생하지 않음을 확인할 수 있을 것이다.
$
Id
-static
—L/usr/lib/gcc/i386-redhat-linux/4•1.2
lib/crtl.o
/usr/lib/crti.o
/usr/lib/crtn.o
main.o
group -Igcc -lgcc_eh -1c --end-group

-o
test
funcs.o

/usr/
--start-

수 root@server：/work/book/utils_.new/ld
[root@seruer Id]# Id -static -L/u와'/].：ib/gcc/i386-redhat-linux/4.1
.2 -o test /usr/lib/crti.o /usr/lib/crti.g /usr/lib/c^tn.o main.o
Funcs.o |--start-gFoii’p| -Igcc -lgcc_eh -1c[__end—group |
[root@se；uer Id]#[root@seruer Id]# Is test
test
[root@seruer Id]# |

[그림 5-30] - -start-group 옵션과 - -end-group 옵션을 추가해 링 킹

--start-group 옵션은 -\（ 옵션과 동일하고 一 end-group 옵션은 -\） 옵션과 동일하
기 때문에 一 start-group 옵션과 -- end-group 옵션 대신 -\（ 옵션과 -\） 옵션을 사
용해도 무방하다.
교차 참조되어 심볼을 못 찾는 문제는 의외로 자주 발생하므로 --start-group 옵션과

--end-group 옵션은 반드시 기억해 두기 바란다.
이상으로 Id에서 자주 사용되는 옵션들을 모두 알아보았다. 이런 옵션 외에도 Id는 더
많은 옵션이 있다. 가장 많이 사용되는 옵션들은 필자가 지금까지 설명한 옵션들이다.
사실 이 정도까지 사용하는 사람도 그렇게 많지는 않다.
나머지 필자가 설명하지 않은 옵션들 중에도 유용한 옵션이 많이 있다. 그렇지만 이 글
을 읽는 절대 다수의 독자들은 나머지 옵션들을 사용할 이유가 거의 없을 거라 본다.
나머지 옵션들은 정말 특수한 경우가 아니고서는 사용할 필요가' 없다. 필자가 하필 그
런 특수한 경우에 해당해 몇 가지 정도 사용하긴 하는데, 필자가 하는 일은 정말 특수
한 일이기 때문에 나머지 사람들은 전혀 걱정하지 않아도 된다.
334 3부_ 컴파일과 링킹

===== PAGE 336 =====
04 링커 스크립트
링커 스크립트는 Id가 링킹 과정을 수행하는 데 있어 모든 링킹 과정을 조절하는 스크
립트다. Id는 링커 스크립트에 기술된 대로 링킹 과정을 수행한다. 링커 스크립트가 없
다면 Id는 제대로 링킹 과정을 수행할 수 없다. 링커 스크립트는 Id가 링킹 과정을 수행
하는 데 있어 반드시 필요한 존재다.
이런 링커 스크립트를 직접 작성하면 일반적으로 하기 힘든 여러 가지 유용한 일들을
가능하게 할 수 있다. 그리고 운영체제, 부트로더 또는 일부 임베디드 시스템 소프트웨
어와 같은 프로그램들은 반드시 링커 스크립트를 직접 작성해야 한다.

I 링커 스크립트의 이해
링커 스크립트가 없다면 Id 는 링킹 과정을 수행할 수 없다고 했었다. 그런데 우리는
애플리케이션을 빌드할 때 별도의 링커 스크립트를 지정해 주지 않았다.
이렇게 별도의 링커 스크립트를 지정해 주지 않으면 Id는 자신이 내장하고 있는 기본
링커 스크립트를 사용해 링킹 과정을 수행한다.

[그림 5-31] Id에 내장된 기본 링커 스크립트를 이용한 링킹 과정

5장_ Id linker

335

===== PAGE 337 =====
기본 링커 스크립트는 Id —verbose 명령으로 다음 그림과 같이 확인 가능한데,
“==..==”부터가 내장된 기본 링커 스크립트의 시작 부분이고, 거의 마지막에 있는
까지가 링커 스크립트의 끝 부분이다.
艾 root@server：/work/book/utils_new/ld
[rootGseruer Id]# Id --uerbose
GNU Id uersion 2.17.50.0.6-6.el5 20061020
Supported emulations:
elf_i386
i3861inux
using internal linker script:
/»
Script
For
-z
conbreloc:
combine
and
sort
,,elF32-i386",
OUTPUT_FORriAT("elf32-i386",
■'elf32-i386")
0UTPUT_ARCH(i386)
ENTRvCstart)
SEARCHZDIR("/usr/i386-redhat-linux/lib"); SEfiRCH_DIR("/usr/local/i

reloc

sections

*/

lib"); SEAR애_DIR("/lib"); SEARCH_DIR(*7usr/lib")；
SECTIONS
/* Read-only sections, merged into text segment: */
PROVIDE (
executable_start = 0x08048000); . = 0x08048000 + SIZ
EOF_HEADERS;
.interp
{ *(.interp) }
{ «(.hash) >
-hash
{ «(.gnu.hash) >
.gnu .hash
< *(.dynsyro) >
.dynsym
{ *(.dynstr) }
.dynstr
< *(.gnu.uersion) }
.gnu .version
< *(.gnu.uersiond) >
.gnu .uersion_d
{ *(.gnu.uersionr) }
.gnu.uersion_r
.rel.dyn
*
*
*
*
*

( .rel.init)
(.rel.text .rel.text.* .rel.gnu.linkonce.t.*)
(.rel.fini)
( .rel.rodata .rel.rodata.* .rel.gnu.linkonce.r.»)
(.rel.data.rel.ro* .rel.gnu.linkonce.d.rel.ro.*)

［그림 5-321 Id —verbose 명령으로 본 기본 링커 스크립트 내용

이전에 필자는 x86 리눅스 시스템에서 애플리케이션의 시작 주소가 0x8048000 이후
라고 몇 번씩 이야기했었다. 왜 그렇게 되는지는 위의 기본 링커 스크립트를 보면 알
수 있다.

. = 0x8048000 + SIZEOF_HEADERS 문장에 의해 0x8048000 + ELF 헤더 사이즈 + 프
로그램 헤더 테이블 사이즈 이후에 .interp 섹션부터 시작해 프로그램의 각종 섹션들이
위치한다. 물론 인스트럭션이 들어있는 .text 섹션도 이후에 위치한다. 그래서 x86 리눅
스 시스템의 애플리케이션 시작 주소는 0x8048000 이후 헤더 위치만큼 떨어진 위치가
된다. 확인을 원하는 독자는 이전에 링킹한 test 프로그램을 nm test I sort 명령으로
확인해 보기 바란다. main 함수의 시작 주소가 0x8048000번지에서 약간 떨어진 주소
에 위치하고 있을 것이다.

336 기부_ 컴파일과 링킹

===== PAGE 338 =====
이렇게 링커 스크립트와 관련된 아무런 옵션도 주지 않고 링킹하면 Id에 내장되어 있는
기본 링커 스크립트를 사용해 링킹한다. 이때 링커 스크립트가 Id에게 알려주는 것은
다음과 같다.
• 입력 오브젝트의 어떤 섹션들을 합쳐 출력 오브젝트의 어떤 섹션을 만들어라.
• 어떤 섹션의 시작 주소는 몇 번지부터다
• 어떤 주소를 가지는（예: .text 섹션의 시작 위치 등） 어떤 심볼을 정의하라.
• 어떤 섹션의 시작 주소는 몇 바이트로 정 렬하라.
• 어떤 섹션은 버려라.
위의 것들 외에도 링커 스크립트로 Id에서 지시내릴 수 있는 것들은 참으로 다양하다.
애플리케이션을 개발할 때 링커 스크립트를 직접 다룰 일은 거의 발생하지 않는다. 하
지만 운영체제, 부트로더, 펌웨어, 임베디드 시스템에서 동작하는 프로그램 등을 개발
할 때는 반드시 링커 스크립트를 직접 작성해야 하는 경우가 많이 발생한다.
이런 프로그램들을 개발할 때 링커 스크립트를 직접 작성해야 되는 이유는 다음과 같
다. 우선 프로그램이 로드되고 실행되는 메모리 주소가 애플리케이션과는 다르다. 일반
적으로 애플리케이션들은 가상 주소를 사용하는 데 반해 운영체제와 같은 시스템 소프
트웨어들은 가상 주소를 사용하기 이전에 물리 주소를 직접 사용하는 경우가 많이 있
다. 예를 들면 부팅할 때와 같은 경우 말이다.
가상 주소를 사용한다면 특정 가상 주소에 DRAM을 맵핑해 프로그램을 동작시킬 수
있다. 때문에 프로그램을 항상 같은 주소로 로딩하고 수행시키는 일이 가능해진다. 하
지만 물리 주소를 사용한다면 실제 DRAM이 위치하는 물리 주소에 프로그램을 로딩하
고 수행시켜야 한다. 때문에 프로그램의 시작 주소는 프로그램을 수행시킬 시스템의 물
리 메모리 주소에 맞춰 주어야 한다. 그러므로 프로그램의 시작 주소 변경을 위해 링커
스크립트를 직접 수정해야 한다.
다른 이유도 여러 가지가 있을 수 있는데 “고급 링킹 테크닉”에서 따로 설명한다.
링커 스크립트를 이해하는 것은 매우 쉽다. ELF, Id만 제대로 알고 있으면 링커 스크립
트의 문법이 간단하기 때문에 금방 이해할 수 있다. 그러면 링커 스크립트 작성법을 본
격적으로 알아보자.

5장_ Id linker

337

===== PAGE 339 =====
O 간단한 링커 스크립트 테스트
먼저 기본 링커 스크립트를 가지고 간단한 테스트를 해 보겠다. 다음 명령으로 Id에
내장되어 있는 기본 링커 스크립트를 default.lds로 만들기 바란다.
$ Id ——verbose > default.Ids

【그림 5-33] defaultjds 파일 생성

defaultjds 파일을 생성했으면 다음과 같이 맨 처음 나오는 “==••• ===” 줄 이전 부분
과 맨 끝에 나오는 “===•..===” 부분을 제거하기 바란다.
〔예제 5-16)

default.lds 파일 내용

GNU Id version 2.17.50.0.6-6.e!5 20061020
Supported emulations:
elf_i386
i3861inux
using internal linker script:
/* Script for -z combreloc: combine and sort reloc sections */
OUTPUT—FORMAT("elf32-i386", "elf32-i386",
"elf32-i386")
OUTPUT_ARCH(i386)
ENTRY(_start)
SEARCH_DIR (’’ /usr/i38 6-redhat-linux/lib” ) ; SEARCH_DIR ( "/usr/
local/lib”); SEARCH_DIR("/lib"); SEARCH_DIR("/usr/lib");
SECTIONS
{
/* Read-only sections, merged into text segment: */
PROVIDE (__executable_start = 0x08048000); . = 0x08048000 +
SIZEOF_HEADERS;
.interp
: { * (.interp) }
.hash
: { *(.hash) }
• • • 중략

/* DWARF 3 */
.debug_pubtypes 0 : { *(.debug_pubtypes) }
.debug_ranges 0 : { *(.debug_ranges) }
/DISCARD/ : { *(.note.GNU-stack) }

338 =_ 컴파일과 링킹

===== PAGE 340 =====
그리고 ［예제 5-16］ 에서 “PROVIDE ••• ”에 해당하는 라인에서 다음과 같이 프로그램
시작 주소를 0x8050000으로 변경하기 바란다.
PROVIDE (_ e x e c u t a b l e _ s t a r t = 0 x 0 8 0 5 0 0 0 0 ) ; . = 0 x 0 8 0 5 0 0 0 0 +
SIZEOF_HEADERS;

그런 후 ［예제 5-1］ 의 main.c와 funcs.c 소스를 다음 명령으로 컴파일하면 정상적인

test 실행 파일이 만들어질 것이다.
$ gcc -c main.c
$ gcc -c funcs.c
$
Id
-T
default.Ids
-dynamic-linker
/lib/ld-linux.so.2
usr/丄ib/crtl.o /usr/lib/crti.o /usr/lib/crtn.o main.o funcs.o -1c

-o

test

/

또는

$ gcc -W1,-T,default.Ids -o test main.c funcs.c

［그림 5-34］ 생성된 test 실행 파일

Id 옵션 중 -T ［링커 스크립트 패스］ 옵션을 주면 Id는 기본 링커 스크립트 대신 -T 옵
션으로 주는 링커 스크립트로 링킹 과정을 수행한다. 우리는 이전에 기본 링커 스크립
트에서 시작 주소를 0x8048000에서 0x8050000으로 변경하였다. 그래서 nm 명령으로

test 실행 파일의 심볼 주소를 읽어 보면 모두 0x8050000 이후에 각각의 심볼들이 위
치한다.

5장_ Id linker

339

===== PAGE 341 =====
기본 링커 스크립트로 장난치는 것은 이쯤에서 끝내기로 하고 매우 간단한 링커 스크
립트를 가지고 가장 많이 사용하는 링커 스크립트의 문법을 알아보자. 먼저 편집기로
다음과 같은 test.lds 파일을 작성하기 바란다.
〔예제 5-17)

test.lds 파일 내용

SECTIONS
{
/* 주석 */

. = 0x8050000;
.text : { * (.text) }
. = 0x9000000;
.data : { *(.data) }
. = OxAOOOOOO;
rodata_start = .;
.rodata

:

{

*(.rodata)

}

rodata_end = .;
.bss : { * (.bss) }

［예제 5-1 기의 test.lds가 의미하는 바는 다음과 같다. 먼저 = 0x8050000；”와

“rodata_start = .；" 문장에 있는 ‘.’과 같은 것을 위치 카운터라 한다. = ［주소］”와 같
은 대입문이 오면 현재 위치를 ［주소］에 맞춘다는 의미이고, “［심볼명］ = .”과 같은 문장
이 오면 현재 위치를 심볼 값으로 심볼명에 해당하는 심볼을 정의한다는 의미다.
그래서 = 0x8050000；” 문장에 의해 현재 위치는 0x8050000으로 된다. 다음으로

“.text : {*(.text) }” 문장이 오는데, “.text : { ••• }” 문장에 의해 출력 섹션 즉, test 바이
너리에 출력되는 섹션이 .text 섹션임을 의미하고, 중괄호(‘{}’) 내부에 있는 “*(.text)”
문장에 의해 모든 입력 오브젝트(‘*’에 의해, 여기서는 main.o, funcs.o, 라이브러리
오브젝트 등)의 .text 섹션들이 합쳐져 .text 출력 섹션을 만든다는 의미다.
다음으로 = 0x9000000：” 문장에 의해 위치 카운터는 0x9000000으로 변경되고 해당
위치에 출력 섹션 .data 섹션이 위치하는데, 모든 입력 오브젝트의 .data 섹션들을 합쳐

.data 출력 섹션을 만들어냄을 의미한다. .rodata, .bss 섹션 역시 위에 설명한 방식으
로 모두 해석할 수 있다.

340 3부_ 컴파일과 링킹

===== PAGE 342 =====
“rodata_start = .；” 문장과 “rodata_end = .；” 문장은 rodata_start 심볼과 rodata_end
심볼을 정의하는데, 심볼의 값은 현재 위치 카운터로 정의된다. 그래서 rodata_start 심
볼은 .rodata 섹션 시작 주소를 심볼 값으로 갖고, rodata_end 심볼은 .rodata 섹션이
끝난 주소를 심볼 값으로 갖는다.
［예제 5-1 刀과 같은 testjds는 다음 명 령으로 링킹하는 데 이용할 수 있다.
$ Id -T test.Ids -o test main.o funcs.o -L/usr/lib -1c

［그림 5-35］ testjds를 이용해 링킹

Id -T testjds -o test main.o funcs.o -L/usr/lib -lc 명령을 내리면 위 그림과 같이
test 실행 파일이 생성된다. 생성된 test 실행 파일에 nm test I sort -kl 명령을 내리
면 위 그림과 같이 각각의 심볼들이 testjds 파일에서 정한 위치에 위치함을 확인할
수 있다.
물론 이렇게 만들어진 test 실행 파일은 실제로 실행할 수 없다. 동적 링커를 지정하지
도 않았고, 초기화와 종료를 수행하는 crt 오브젝트를 링킹하지도 않았기 때문이다.
지금까지 간단한 링커 스크립트를 맛보았고, 이제 본격적으로 링커 스크립트의 문법을
알아보자.

5장_ Id linker 341

===== PAGE 343 =====
I 링커 스크립트 기본 문법
링커 스크립트의 문법은 ELF 바이너리 포맷의 구조를 이미 알고 있다면 매우 간단하게
이해할 수 있다. 먼저 기본이 되는 SECTIONS 명령을 알아보자.

O SECTIONS 명령
완전한 링커 스크립트는 반드시 SECTIONS 명령이 들어있어야 한다. SECTIONS 명령
은 다음과 같은 구조로 되어 있다.
〔예제 5-18)

SECTIONS 명령 기본 형식

SECTIONS
{

sections-명령
sections-명령
}

SECTIONS 명령은 SECTIONS 키워드가 있고 중괄호({, )) 사이에 “sections-명령”들
이 들어가는 구조로 되어 있다. sections-명령은 SECTIONS 명령 내부에 기술될 수 있
는 명령들이다. 이런 명령에는 4가지 타입이 있는데, 각각은 다음과 같다.
• 출력 섹션 기술

• ENTRY 명 령
•

심볼대입

•

오버레이 기술

각각의 기술들에 대해 차차 설명하기로 하고, 이 중 가장 중요한 출력 섹션 기술을 먼
저 알아보자.
@ 출력 섹션 기술

출력 섹션 기술은 출력 오브젝트에 출력될 섹션들을 기술하는 명령이다. 여기서 출력
오브젝트는 Id -T test.lds -o test main.o funcs.o -L/usr/lib -1c와 같은 명령이 있을
때 test처럼 링킹되어 출력될 오브젝트를 말한다. 반대로 main.o, funcs.o, -1c(정적 링
킹 시 Ubc.a에 있는 오브젝트)와 같은 오브젝트를 입 력 오브젝트라 한다.
출력 섹션 기술은 출력 오브젝트에 포함되는 섹션들을 기술하는 명령이다. 그래서 ［예제

5-19］ 에 있는 testjds는 출력 오브젝트에 .text, .data, .bss 섹션이 들어있음을 의미한다.

342 3부— 컴파일과 링킹

===== PAGE 344 =====
〔예제 5-19〕 test. Ids 출력 섹션 기술 예

SECTIONS
{
.text : { * (.text) }
.data : { *(.data) }
.bss : { * (.bss) }
}

위 예제와 같은 출력 섹션 기술은 매우 간단한 형태의 출력 섹션 기술이다. 출력 섹션
기술 형태를 매우 단순하게 보면 다음과 같다.
출력 섹션명: { 입력 섹션 명령들)

그래서 ［예제 5-19］ 에서 .text 출력 섹션의 입력 섹션은 *(.text)가 되고, 모든 입력 오
브젝트에 포함되어 있는 .text 섹션을 의미한다. 따라서 이를 해석해 보면 모든 입력 오
브젝트에 있는 .text 섹션들을 합쳐 .text 출력 섹션을 만들라는 의미다.
보통은 이렇게 단순한 형태의 출력 섹션 기술이 많이 사용된다. 그래서 이 정도만 알아
도 링커 스크립트를 작성하는 데 크게 무리가 없지만 좀 더 복잡하고 다양한 기능을 사
용하려면 제대로 된 출력 섹션 기술법을 알아야 된다. 지금부터 출력 섹션의 기술법을
설명한다.
먼저 기본적인 출력 섹션 기술 형식은 다음과 같다.
〔예제 5-20)

출력

섹션명

[address] [ (type) ] : [AT (Ima)]

{
입력 섹션一명령
입력 섹션一명령

} [>region] [AT>lma_region] [:phdr :phdr ...] [=fillexp]

이 중 반드시 필요한 것은 출력 섹션명과 콜론(：), 그리고 중괄호(I })다. 나머지는 있어
도 되고 없어도 되는 부분이다. 각각을 해석해 보면 다음과 같다.
먼저 출력 섹션명이 온다. .text, .data, .bss와 같은 것들이 출력 섹션명에 해당한
다. 그리고 주소가 올 수 있는데, 해당 출력 섹션이 위치하는 VMA(Virtual Memory

Address)를 의미한다.

5장_ Id linker

343

===== PAGE 345 =====
링커 스크립트에서는 두 가지 종류의 주소 개념이 사용되는데, VMA 와 LMA(Load

Memory Address)가 바로 그것이다. VMA는 해당 프로그램이 수행될 때 사용되는 가
상 메모리 주소를 의미한다. LMA는 해당 프로그램이 로드될 메모리 주소를 의미한다.
일반적으로 VMA와 LMA는 동일하지만 다음과 같은 특수한 상황에서 VMA와 LMA는
달라질 수 있다.
0x0

0x0
0x10

0x10000

0x20

(A) 출력 오브젝트

(B) 시스템 메모리 구조

(D) .data, .bss만
RAM에서 수행

［그림 5-36］ VMA와 LMA가 다른 예

［그림 5-36］ 에서 (A) 와 같은 출력 오브젝트가 있을 때 (A) 출력 오브젝트에서 0x0,

0x10, 0x20과 같은 것은 파일상의 섹션 오프셋을 의미한다. (A) 오브젝트가 로딩될 시
스템의 메모리 맵은 (B)와 같은 형태라고 가정을 하자. (B)와 같은 메모리 맵은 임베디
드 시스템에서 흔히 볼 수 있는 메모리 맵이다.
먼저 (A) 출력 오브젝트는 (C) 또는 (D)와 같이 ROM에 위치하고 전원이 인가되면 부
팅하면서 자신의 이미지를 RAM에 복사한다. (C)는 전체 출력 오브젝트 이미지를 RAM
에 복사한 후 RAM에서 .text 섹션이 실행되는 경우이고, (D)는 RAM 공간을 절약하기
위해 .data와 .bss 섹션만 RAM에 복사한 경우이다. (D)와 같은 경우 .text 섹션은 ROM
의 영역에서 실행된다(물론 .bss 섹션은 실제 파일 이미지에 공간이 잡히는 섹션이 아
니므로 복사하고 말 것도 없지만 예를 들어 설명하면 그렇다).
이때 (C)의 경우 LMA와 VMA는 RAM의 영역인 0x10000번지로 동일하다. 하지만 (D)
의 경우에 .text 섹션은 LMA와 VMA가 0x0번지로 동일하지만, .data 섹션은 LAM가

0x10번지인 반면 VMA는 0x10000을 가진다. .bss 섹션 역시 LMA는 0x20번지인 반면
VMA는 0x10010번지를 가진다.

344 3부- 컴파일과링킹

===== PAGE 346 =====
(D)와 같이 RAM 공간을 절약하기 위해 .text 섹션은 ROM에서 바로 실행시키고, .data
와 .bss 섹션과 같이 쓰기 가능해야 되는 섹션만 RAM에 복사해 실행하는 기법을 XIP
라 부른다. "는 나중에 자세히 설명한다. 지금 여기서는 이런 특수한 경우에 LMA 와

VMA가 달라질 수도 있음을 감각적으로 확인하면 된다.
출력 섹션명 뒤에 오는 [address] 필드는 해당 섹션이 위치할 VMA를 의미한다. 그래
서 다음 예와 같이 기술하면 .mysection 섹션은 VMA OxAOOOOOO번지 에 위 치 한다.
〔예제 5-21〕 출력 섹션 기술 예

SECTIONS {
.mysection OxAOOOOOO :
{
입력 섹션一명령
입력 섹션一명령

다음에 오는 [(type)]은 섹션의 종류를 나타내며, 다음과 같은 것들이 올 수 있다.

• NOLOAD: 해당 섹션을 로드하지 않음
• DSECT： 호환을 위해 존재하며 거의 사용되지 않음
• COPY： 호환을 위해 존재하며 거의 사용되지 않음
• INFO： 호환을 위해 존재하며 거의 사용되지 않음
• OVERLAY： 호환을 위해 존재하며 거의 사용되지 않음
type 지정은 거의 사용되지 않기 때문에 신경 쓰지 않아도 된다. 다음에 오는 [AT(lma)]
키워드는 VMA와 LMA가 다를 경우 LMA를 명시해 주는 필드다.
〔예제 5-22〕 줄력 섹션 기술 예: AT 키워드

SECTIONS {
. = 0x1000;
my_lma = ALIGN(4);
.mysection OxAOOOOOO : AT(my_lma)
{
입력 섹션一명령
입력 섹션一명령

}

5장_ Id linker

345

===== PAGE 347 =====
그래서 위와 같이 기술하면 .mysection 섹션의 VMA는 OxAOOOOOO번지로 설정되고,

LMA는 0x1000번지로 설정된다. AT 키워드는 myjma와 같은 심볼 없이 AT(OxlOOO)
과 같이 사용할 수도 있다.
일반적으로 AT 키워드를 사용해 LMA를 VMA와 달리해야 될 경우는 그리 많지 않다.
하지만 반드시 그렇게 해야 될 경우가 있는데, 나중에 설명할 XIP 기법이나 오버레이
기법을 사용할 경우에는 LMA와 VMA를 달리해 주어야 한다.
다음으로 중괄호({, }) 안에 각종 입력 섹션 명령들이 올 수 있다. 입력 섹션 명령에는
다음과 같은 종류가 있다.
• 입력 섹션 기술
• 심볼 할당
• 직접 포함할 자료 값
• 특별한출력 섹션 키워드
이 중 입력 섹션 기술이 가장 중요하다. 입력 섹션 기술은 나중에 설명하기로 하고 줄
력 섹션 기술에 있는 Dregion］ 을 먼저 설명한다.
［〉region］ 은 출력 섹션의 메모리 영역을 정하는 필드다. 간단하게 예를 들면 다음과 같다.
〔예제 5-23)

출력 섹션 기술 예: 메모리 영역 지정(VMA)

MEMORY { SRAM : ORIGIN = 0x8000000, LENGTH = 0x100000 }
SECTIONS {
.mysection

:

{

입력 섹션一명령
입력 섹션一명령

}

} >SRAM

먼저 MEMORY 명령으로 시스템의 특정 메모리 영역을 정의한다. MEMORY 명령은
다음과 같은 형태면 된다.
MEMORY {
메모리명 ［ (attr) ］ : ORIGIN = 시작주소, LENGTH = 사이즈

}

346 3부- 컴파일과링킹

===== PAGE 348 =====
attr로 올 수 있는 것은 다음과 같다.
•

R： 읽기 전용 영역

• W： 읽기/쓰기 영역
•

X： 실행 가능 영역

•

A： 할당가능 영역

• I： 초기화된 영역
•

L： 초기화된 영 역(I와 동일)

• I; 위 속성의 의미를 역으로 함
다음은 MEMORY 명령의 예다.
MEMORY {
ROM (rx) : ORIGIN = 0x0, LENGTH = IM
RAM : ORIGIN = 0x400000, LENGTH = 32M
}

결국 ［예제 5-23］ 에서는 MEMORY ( SRAM : ORIGIN = 0x8000000, LENGTH =

0x100000 } 명령으로 시작 주소가 0x8000000이고, 사이즈가 0x100000인 SRAM 영역
이 정의되었다. 그리고 .mysection : {...} >SRAM 명령으로 .mysection 섹션을 SRAM
영역에 할당했다.

[>region] 키워드 다음에는 [AT>lma_region] 키워드가 올 수 있다. [AT〉lma_region]
키워드는 [>region] 키워드와 사용법 면에서 거의 동일하며, LMA의 메모리 영역을 지
정하는 점에서 차이가 있을 뿐이다. 다음은 [AT>lma_region] 키워드의 사용 예다.
〔예제 5-24〕 줄력 섹션 기술 예: 메모리 영역 지정(LMA)

MEMORY {
ROM (rx) : ORIGIN = 0x0, LENGTH = 0x10000
SRAM : ORIGIN = 0x8000000, LENGTH = 0x100000
}
SECTIONS {
.mysection : {
입력 섹션一명령
입력 섹션一명령

}
} >SRAM AT>ROM

5장_ Id linker 347

===== PAGE 349 =====
다음으로 올 수 있는 키워드는 [：phdr ：phdr …] 키워드다. 해당 키워드는 해당 섹션을
포함시킬 세그먼트를 지정하는 키워드다. 예를 들면 다음과 같다.
〔예제 5-25〕 출력 섹션 기술 예: 세그먼트 지정

PHDRS { mydata PT_LOAD; }
SECTIONS {
.mysection : {
입력 섹션一명령
입력 섹션一명령
}

} :mydata

위 예제는 mydata 세그먼트를 정의하고 .mysection 섹션을 mdata 세그먼트에 포함시
킨 예다. PHDRS 명령은 프로그램 헤더를 정의하는 명령인데, 다음과 같은 구조를 가지
고 있다.
PHDRS {
세그먼트명 타입 [FILEHDR] [PHDRS] [AT （주소） ] [FLAGS （플래그） ] ;

타입에는 다음과 같은 것들이 올 수 있다.
[표 5-4] 프로그램 헤더 타입 리스트

348

타입명

의미

PT_LOAD

메모리에 로드해야 되는 세그먼트

PT_NULL

사용되지 않는 프로그램 헤더

PT_DYNAMIC

동적 링크를 해야 되는 자료를 포함하는 세그먼트

PTJNTERP

인터프리터 이름을 포함하는 세그먼트

PT_PHDR

프로그램 헤더를 포함하는 세그먼트

PT_NOTE

노트 정보를 포함하는 세그먼트

PT_SH 니 B

예약된 프로그램 헤더

expression

expressionOl 프로그램 헤더 타입임. 위에 해당하지 않는 타입의 경우 사용

3부— 컴파일과 링킹

===== PAGE 350 =====
출력 섹션 기술에서 마지막으로 오는 것은 [=fillexp] 키워드다. [=fillexp] 키워드는 출
력 섹션에서 입력 섹션이 위치하는 영역 외에 나머지 영역들에 대해, 예를 들면 정렬을
위해 필요한 빈 공간 등을 fillexp로 채우는 것을 의미한다. 그래서 다음과 같은 예제에
서 .mysection 섹션의 빈 공간은 0x5A5A가 반복해서 채워진다.
〔예제 5-26〕 출력 섹션 기술 예: 빈 영역 채우기 지정

SECTIONS { *
.mysection : {
입력 섹션-명령
입력 섹션一명령

}

：

i
:

i

} =0x5A5A

지금까지 출력 섹션 기술을 설명하였다. 지금까지 설명한 모든 내용을 종합해 보면 출력
섹션 기술은 다음과 같이 복잡하게 기술할 수도 있다.
〔예제 5-27〕

■ PHDRS { mydata PT_LOAD; }
： MEMORY {

ROM (rx) : ORIGIN = 0x1000, LENGTH = 0x10000
SRAM : ORIGIN = 0x8000000, LENGTH = 0x100000
!

}

： SECTIONS {

. = 0x1000;
my_lma = ALIGN(4);
.mysection 0x8000000 (NOLOAD) : AT(my_lma)
i{
입력 섹션一명령
입력 섹션一명령

} >SRAM AT>ROM :mydata =0x5A5A
|}

물론 출력 섹션 기술은 LMA와 VMA가 두 번 설정되는 오류가 있다. 위 예에서는 이 렇
게 복잡하게 사용할 수도 있다는 점 만 확인하면 된다.
지금까지 출력 섹션 기술을 알아보았다. 이제는 입력 섹션 기술을 알아보자.

5장_ Id linker

349

===== PAGE 351 =====
0 입력 섹션 기술
입력 섹션 기술은 출력 섹션 기술에 비하면 매우 단순하다. 다음은 입력 섹션 기술의 예다.
[표 5-5] 입력 섹션 기술 예

기술예
*(.text)

| 의미
모든 파일의 .text 섹션

*(EXCLUDE_FILE (a.o b.o) .text)

a.o와 b.o를 제외한 모든 파일의 .text 섹션

♦(.text .rodata)

모든 파일의 .text 섹션과 .rodata 섹션

*(.text) *(. rodata)

모든 파일의 .text 섹션과 .rodata 섹션

a.o(.text)

a.o의 .text 섹션

a.o

a.o의 모든 섹션

사;?.o(.text)

kk로 시작하고 아무 글자나 하나 오고 .0로 끝나는 파일의 .text 섹션

출력 섹션 기술에서 “입력 섹션-명령”에 해당하는 부분에 입력 섹션 기술을 적으면 된
다. 그러면 Id가 해당 입력 섹션들을 합쳐 출력 섹션으로 만들어준다. 입력 섹션 기술에
서 입력 오브젝트의 지정은 유닉스 셸에서 사용하는 정규 표현식을 지원하므로 다음과
같은 예도 가능하다.
.test : { aa?.o(.data .rodata) bb[0-9].o(,userdef_section) }

풀어 보면 aa로 시작하고 아무 문자나 한 문자가 오는 오브젝트들에서 .data 섹션,

.rodata 섹션과, bb로 시작하고 아무 숫자 하나가 오는 오브젝트들에서 .userdef_
section을 합쳐 .test 섹션으로 만들라는 의미다.
[표 5-5]에서 *(.text .rodata)와 *(.text) *(.rodata)의 차이점은 다음과 같다.

.text : { *(.text .rodata) } 기술을 예로 들면 먼저 *(.text .rodata)는 모든 입력 오브젝
트의 .text 섹션과 .rodata 섹션을 합쳐 .text 출력 섹션을 만들라는 의미다. 가령 main,

o와 funcs.o가 입력 섹션이라면 test 실행 파일의 .text 섹션에는 main.o의 .text 섹션
이 먼저 오고 다음으로 main.o의 .rodata 섹션이 온다. 그리고 f니ncs.o의 .text 섹션이
위치하고 다음으로 f니ncs.o의 .rodata 섹션이 위치한다.
반면 .text : { *(.text) *(.rodata) } 기술을 하면 test 실행 파일의 .text 섹션에는 main,

o의 .text 섹션이 먼저 오고 다음으로 funcs.o의 .text 섹션이 오며 , 다음으로 main.o의
.rodata 섹션이 오고 마지막으로 funcs.o의 .rodata 섹션이 온다.
*(.text .rodata)냐 *(.text) *(.rodata)냐에 따라 .text 출력 섹션에 포함되는 입력 섹션
의 순서가 달라진다.
350 3부— 컴파일과 링킹

===== PAGE 352 =====
Q 심볼 대입 명령
심볼 대입 명령은 심볼에 값을 대입하는 명령이다. 보통 주소를 값으로 대입하는데, 반
드시 주소가 아니라도 상관은 없다. 심볼 대입 명령은 대입 연산자 외에 다양한 연산자
를 사용할 수 있는데, 사용할 수 있는 연산자는 다음과 같다.
symbol
symbol
symbol
symbol
symbol
symbol
symbol
symbol
symbol

expression ;
expression ;
expression ;
expression ;
expression ;
«= : expression ;
»= : expression ;
&= ।expression ;
expression ;

［예제 5-28］ 은 실제 심볼 대입 명령의 예다.
〔예제 5-28〕

SECTIONS
. = 0x8050000;
.text : { *(.text) }
. = 0x80B0000;
.data : { *(.data) }
. = 0x80E0000;
. += 0x1000;
rodata_start = .;
.rodata : { *(.rodata) }
PROVIDE(rodata_end = (. + 3) & ~ 4);
.bss : {
__ bss_start = ALIGN(4);
*(.bss)
__bss_end = . ;

［예제 5-28］ 에서 rodata_start 심볼과 rodata_end 심볼을 정의한다. 이렇게 정의한 심
볼은 링커 정의 심볼(linker defined symbol)이라 부르기도 하고, C 소스 또는 어셈블
리 소스 코드에서 다음과 같은 형식으로 참조할 수 있다.
〔예제 5-29〕

extern unsigned char *rodata_start
extern unsigned char *rodata_end
main () {

5장_ Id linker

===== PAGE 353 =====
int i;
for (i=(int)rodata_start; i < rodata_end; i++)
{
}
return 0;
}

rodata_end에서 (. + 3) & ~ 4)； 값은 현재 주소: 위치 카운터)를 4바이트 정렬한
값이다. 이것은 _bss_start 심볼을 정의할 때 ALIGN(4) 함수를 사용한 것과 의미적으
로 같다. 그리 고 PROVIDE (symbol = expression) 에 의 해 symb이에 해 당하는 심 볼이

C 소스 또는 어셈블리 소스에 정의되어 있지 않다면 symb이을 새로 정의하지만, 이미
symbol 심볼이 C 소스 또는 어셈블리 소스에 정의되어 있다면 새롭게 정의하지 말라
는의미다.
이렇게 하면 C 소스 또는 어셈블리에서 정의한 심볼과 링커에서 정의한 심볼의 충돌을
막을 수 있다.

S 사용가능한함수
링커 스크립트에서는 다음과 같은 기본 함수들이 있다. 이런 기본 함수들은 링커 스크
립트 내에서 자유롭게 사용 가능하다.
[표 5-6] 기본 함수 예

352

함수명

의미

ABSOLUTEfexp)

표현식 exp의 (재배치 가능하지 않은) 절댓값을 반환

ADDR(section)

section의 절대 주소를 (VMA) 반환

ALIGN(exp)

다음 exp 경계에 정렬한 위치 카운터를 (.) 반환

BLOCK(exp)

오래된 링커 스크립트와 호환을 위한 것으로 AUGN과 동일

DEFINED(symbol)

symbolOl 전역 심볼표에 있고 정의돼 있다면 1을 반환하고, 아니면 0을 반환

MAX(exp1, exp2)

exp1 와 exp2 중 큰 값을 반환

MIN(exp1, exp2)

exp1 와 exp2 중 작은 값을 반환

NEXT(exp)

exp의 배수인 할당되지 않은 다음 주소를 반환

SIZEOF(section)

sectionOl 정의되었다면 그 크기를 바이트 단위로 반환

SIZEOF_HEADERS

출력 파일 헤더의 크기를 바이트 단위로 반환

sizeof_headers

SIZEOF_HEADERS와 동일

3부_ 컴파일과 링킹

===== PAGE 354 =====
함수 사용 예를 직접 확인하고 싶다면 Id —verbose 명령으로 기본 링커 스크립트를
보기 바란다. 표에서 설명한 함수들의 실제 사용 모습을 확인할 수 있을 것이다.

自기타명령

지금까지 출력 섹션 기술과 입력 섹션 기술을 알아보았다. 이제부터는 아직 설명하지
못한 나머지 명령들을 알아본다.

► ENTRY(symbol)
symbol을 엔트리 포인터로 설정한다. 이전에 Id 옵션을 설명하면서 -e ［엔트리 포인
테 옵션에 대해 설명한 것이 기억날 것이다. 엔트리 포인터는 프로그램을 로딩하고 제
일 처음 수행시킬 주소를 의미한다. 일반적으로 별다른 옵션을 주지 않으면 엔트리 포
인터는 _start 레이블로 설정되어 있다. 그것은 기본 링커 스크립트에서 ENTRY(_start)
명령에 의해 _start 레이블이 엔트리 포인터로 지정되기 때문이다. 궁금한 사람은 Id

—verbose 명령으로 기본 링커 스크립트를 확인해 보기 바란다.
_start 레이블은 gcc 기본 옵션으로 컴파일할 경우 링킹되는 /usr/lib/crtl.o 에 들어있
다. 그런데 애플리케이션을 컴파일하는 경우가 아니라서 /usr/lib/crtl.o 을 링킹하지
않는 경우라면 어떻게 할까?
이런 경우라면 링커 스크립트가 엔트리 포인터를 _start에서 프로그램 내에 존재하는
다른 레이블로 바꿔 주어야 링킹 시 경고가 발생하지 않는다.
〔예제 5-30)

ENTRY (main)
SECTIONS
{
.text : { * (.text) }
.rodata : { * (.rodata) }
.data : { *(.data) }
.bss : { *(.bss) }

［예제 5-3이은 ENTRY 명령으로 엔트리 포인터를 main으로 변경한 예다. 이렇게 경고
를 없애기 위해 엔트리 포인터를 바꿀 수도 있고, 애플리케이션이라면 처음 시작하는
주소를 바꾸기 위해 엔트리 포인터를 바꿀 수도 있다.
INCLUDE filename

5장_ Id linker

353

===== PAGE 355 =====
filename에 해당하는 링커 스크립트를 현재 링크 스크립트의 현재 위치에 include
한다.
INPUT (filel, file2, • • •) 또는 INPUT (filel file2 , • ■ •)

인자로 오는 오브젝트 파일 filel과 file2를 입력 오브젝트로 포함한다. 이것은 명령라
인에서 Id -o ［출력 오브젝트］ filel file2 •••를 한 것과 동일하다.
GROUP (filel, file2 , • ■ •) 또는 GROUP (filel file2 , • • •)

filel과 file2는 아카이브 파일(*.a)이다. 이 명 령은 인자로 오는 아카이브 파일에서 정의
되지 않은 참조가 새로 만들어지지 않을 때까지 반복 검색한다. 이 명령은 명령라인에
서 --start-group filel file2 --end-group 옵션을 준 것과 동일하다.
OUTPUT(filename)

출력 파일을 filename으로 설정한다. 이 명령은 명 령라인에서 -o filename 옵션을 준
것과 동일하다.
SEARCH_DIR(path)

라이브러리 검색 패스에 path를 포함시킨다. 이 옵션은 명령라인에서 -Lpath 옵션
을 준 것과 동일하다. 이전에 필자가 Id는 애플리케이션을 컴파일할 때 /usr/i386-

redhat-linux/lib, /usr/local/lib, /lib, /usr/lib순으로 라이브러리를 찾는다고 이야기
했었다. 이런 순서로 찾는 것은 기본 링커 스크립트에 다음과 같이 SEARCH_DIR 명령
이 지정되어 있기 때문이다.
〔예제 5-31)

기본 링커 스크립트의 내용

OUTPUT_FORMAT("elf32-i386", "elf32-i386", "elf32-i386")
OUTPUT_ARCH(i386)
ENTRY(_start)
SEARCH_DIR("/usr/i386-redhat-linux/lib");
SEARCH_DIR("/usr/
local/lib"); SEARCH_DIR("/lib"); SEARCH_DIR("/usr/lib");
SECTIONS

STARTUP (filename)

354 3부— 컴파일과 링킹

：
：

:
：

===== PAGE 356 =====
filename에 해당하는 오브젝트를 가장 먼저 링킹한다는 점을 제외하면 INPUT 명령과
동일하다. 엔트리 포인터가 실허 이미지의 제일 처음인 경우에 유용하다. 운영체제, 부
트로더, 펌웨어 같은 프로그램들이 이 경우에 해당하는데, 이런 프로그램들은 ELF 헤더
에 있는 엔트리 포인트를 참조하지 않는다.
아예 ELF 헤더조차 제거되고 프로그램 수행에 필요한 순수 바이너리 이미지만 존재하
는 프로그램에서 프로그램의 시작 주소는 거의 대부분 프로그램의 제일 첫 부분이 된
다. 때문에 보통의 경우 Id -o kernel startup.o •••와 같이 입력 오브젝트의 순서로 제
일 처음 위치하는 코드를 정하는데, STARTUP 명령을 사용해도 이와 같은 역할을 수행
할수있다.
OUTPUT_FORMAT(bfdname)

출력 오브젝트 포맷으로 bfdname에 해당하는 포맷으로 설정한다. 여기서 BFD는

Binary File Descriptor의 약자다. objdump -i 명령으로 사용 가능한 BFD 이름
을 확인할 수 있다. OUTPUT_FORMAT(bfdname) 명령은 명령라인에서 -oformat

bfdname 옵션을 준 것과 동일하다.
OUTPUT_FORMAT(default-bfd, big-bfd, little-bfd)

아무 옵션을 주지 않으면 출력 오브젝트 포맷을 default-bfd 포맷으로 설정하고, -EB
옵션을 주면 big-bfd 포맷으로, -EL 옵션을 주면 little-bfd 포맷으로 설정한다. 여기서

big과 little은 빅 엔디안과 리틀 엔디안을 의미한다. 기본 링커 스크립트에는 다음과 같
이 지정한다.
〔예제 5-32)

기본 링커 스크립트의 내용

OUTPUT_FORMAT("elf32-i386", "elf32-i386" , "elf32-i386")
SECTIONS

：

TARGET(bfdname)

입력 오브젝트의 BFD 형식을 bfdname으로 설정한다.
ASSERT(exp,

message)

5장_ Id linker

355

===== PAGE 357 =====
exp가 0이면 message를 출력하고 링킹 과정을 종료한다. 링킹 과정에서 오류를 찾을
때 사용한다.
EXTERN(symbol symbol ...)

symbol을 출력 파일에 정의되지 않은 심볼로 포함시킨다.
OUTPUT_ARCH(bfdarch)

출력 아키텍처를 지정한다. objdump -i 명령으로 지정 가능한 아키텍처를 확인할 수
있다.
BYTE(value) / SHORT(value) / LONG(value) / QUAD(value)

현재 위치에 지정된 사이즈(BYTE： 1, SHORT： 2, LONG： 4, QUAD： 8)의 공간을 할당
하고 value 값으로 설정한다. 사용 예는 다음과 같다.
〔예제 5-33)

공간 할당 예

SECTIONS
{
.text : {
text_start = .;
*(.text)
text_end =
.;
text_size = .;
LONG (text_end - text___start) ;
}
.data : { *(.data) }
.bss : { * (.bss) }

：

：
：
；

i
;

이런 BYTE, SHORT, LONG, QUAD 명 령은 반드시 출력 섹션 명 령 내에서만 사용되
어야 한다.
이상 링커 스크립트를 사용하는 방법 및 링커 스크립트의 각종 문법에 대한 설명이 끝났
다. 이쯤에서 재미난 사실을 하나 알려주겠다. 표준 C 공유 라이브러리인 /usr/Hb/Hbc.

so 파일을 열어보기 바란다. 해당 파일을 열어보면 해당 파일이 사실은 링커 스크립트임
을 확인할 수 있을 것이다. 원래 Id의 입력 파일에는 라이브러리뿐만 아니라 링크 스크
립트도 포함된다. 그리고 더욱 재미난 사실은 /usr/lib/libc.so 파일의 실제 라이브러리
중 하나인 Aib/libc.so.6 파일을 한번 수행시켜 보라. 그러면 라이브러리 중에 /lib/libc.

so.6와 같이 실제 수행될 수 있는 공유 라이브러리도 있다는 것을 확인할 수 있을 것이
다. 다음으로는 지금까지 배운 내용을 토대로 좀 더 고급 링킹 테크닉을 알아본다.

356 3부_ 컴파일과 링킹

===== PAGE 358 =====
05 Id를 사용한 고급 링킹 테크닉
지금까지 배운 내용을 정리하자. 많은 것을 알아보았는데, 어떨 때 사용하는지 이해하
지 못하면 제대로 알았다고 이야기할 수 없을 것이다.

I os 개발을 위한 링커 스크립트
OS 를 개발하는 독자가 있는가? 필자는 지금까지 1 개의 GPOS 와 서로 다른 4 종류의
RTOS를 개발하였다. 그 중에는 대기업의 표준 플랫폼 OS가 되어 수많은 종류의 제품
으로 전 세계에 수출되는 OS도 있다.

OS를 개발할 때는 링커 스크립트를 직접 작성해야 한다고 설명했는데, 어떻게 작성하
면 되는지 필자가 사용하는 OS의 링커 스크립트로 알아보자.
〔예제 5-34)

OS 개발을 위한 testos.lds 링커 스크립트

OUTPUT_FORMAT("elf32-littlearm", "elf32-littlearm"z "elf32-littlearm")
OUTPUT_ARCH(arm)
ENTRY(startup)
SECTIONS
{
. = 0xA0008000;
kernel_start = .;
_text_start = .;
text : { *(.text) }
_text_end = .;
rodata : { *(.rodata) }
_rodata_end = .;
_data_start = .;
data : { *(.data) }
_data_end = .;
_bss_start = .;
bss : { * (.bss) }
_bss_end = .;
_kernel_end = .;

5장_ Id linker 357

===== PAGE 359 =====
위 예제는 필자가 QEMU라는 에뮬레이터에서 OS 테스트를 위해 사용하는 링커 스크
립트를 매우 단순하게 만들어 놓은 것이다. QEMU는 여러 시스템을 지원하는데, 필자
가 사용하는 시스템은 PXA-255 프로세서를 탑재한 시스템이다. 필자가 사용하는 시스
템에서 0xA0008000 영역은 DRAM 영역으로, 부트로드가 kernel을 로딩하는 번지다. 그
래서 .text 섹션의 시작 번지가 0xA0008000번지로 된 것이다.
이런 링커 스크립》｝ 있을 때 다음과 같은 명령을 사용해 DRAM(0xA0008000)에 로
드할 OS 이미지를 만든다.
arm-linux-ld
-EL
-static
-X
-L/usr/local/arm-linux—4.1.1/
bin/
.
./lib/gcc/arm-iwmmxt—linux-gnueabi/4.1.1
-L/usr/local/armlinux-4.1.1/bin/../lib/gcc
-L/usr/local/arm-linux-4.1.1/bin/
.
.
/
lib/gcc/arm-iwmmxt-linux-gnueabi/4.1.1/../../../../arm-iwmmxtlinux-gnueabi/lib
-T
testos.Ids
-N
arch/arm/built-in.o
kernel/
built-in.o task/built-in.o -o xnous.elf -Igcc
arm-linux-objcopy
xnous.img

-0

binary

-R

.note

-R

.comment

-S

xnous.elf

나머지 부분들은 지금까지 배운 내용을 바탕으로 하나씩 해석해 보면 그리 어렵지 않
을 것이다.

IXIP 기법을 사용한 메모리 절약
XIP(eXecute In Place)는, .text 섹션 및 .rodata 섹션처럼 읽기 전용 섹션은 ROM에
두고, .data 섹션, .bss 섹션처럼 쓰기 가능한 섹션들은 RAM에 두고 수행시키는 기법이
다. 일반적으로 XIP를 사용하지 않으면 읽기 전용 섹션도 RAM에 두고 수행시켜야 하
기 때문에 메모리 낭비를 가져올 수 있다.
0x0

0x0
0x10

0x10000

0x20
(A) 출력 오브젝트

(B) 시스템 메모리 구조

[그림 5-37] 일반적인 방식(C)과 XIKD) 방식 비교

358 3부—컴파일과링킹

===== PAGE 360 =====
［그림 5-3刀이 일반적인 방식과 XIP 방식을 비교한 그림이다. (A)와 같은 OS 커널 이
미지가 있고, (B) 와 같은 메모리 맵을 가지는 시스템이 있을 때 (C) 와 같이 부팅 시

ROM에 있는 모든 이미지를 RAM에 복사한 후 수행하는 방식이 일반적인 방식이고,
(D)와 같이 .data, .bss 섹션처럼 쓰기 가능 섹션만 RAM에 복사한 후 수행하는 방식이
XIP 방식이다.
XIP 방식을 사용하려면 OS 커널의 링크 스크립트는 다음과 같아야 한다.
〔예제 5-35)

XIP를 사용하는 링커 스크립트

OUTPUT_FORMAT("elf32-littlearm",
OUTPUT_ARCH(arm)
ENTRY(startup)
SECTIONS

"elf32-littlearm",

"elf32-littlearm")

{
• = ［제일 처음 수행되는 ROM 영역 시작 주소］ ;

________________ __ .;
__text_start = .;
.text : { * (.text) }
__text_end = .;
.rodata
:
{
__rodata_end = .;

*(.rodata)

}

__ data_loc_start = ALIGN(4) ;
. = ［ RAM상의 .data 섹션주소］ ;
__data_start = .;
. data : AT (_______ data_loc_start) { * (. data) }
__data_end = .;
data loc end = data loc start + SIZEOF(.data);
__bss_start = .;
.bss : { * (.bss) }
__________ __ .;
_________ __ .;
}

우선 다음 문장에 의해 .rodata 섹션 바로 뒤에 오는 .data 섹션의 바이너리 이미지상
의 위치를 구한다.
__data_loc_start = ALIGN(4) ;

5장_ Id linker

359

===== PAGE 361 =====
그리고 다음 문장에 의해 .data 섹션의 VMA를 [RAM상의 .data 섹션 주소]로 맞춘다.
. = [RAM상의 .data 섹션 주소] ;

그리고 다음과 같이 .data 섹션의 LMA를 .rodata 섹션 바로 뒤로 설정한다. 이렇게 하면

OS 바이너리 이미지상에서 .data 섹션은 .rodata 섹션 바로 뒤에 위치한다. 하지만 .data
섹션 내 정의된 모든 심볼은 [RAM상의 .data 섹션 주소]를 기준으로 정의되어 있다.
마찬가지로 .data 섹션에 있는 전역변수 등을 액세스하는 .text 섹션의 인스트럭션 역
시 .data 섹션의 심볼을 참조할 때는 [RAM상의 .data 섹션 주소]로 설정된 VMA를 기
준으로 참조하게 컴파일된다.
.data : AT (_______ data_loc_start) { * (.data) }

.bss 섹션은 어차피 바이너리 이미지에 포함되지 않는 영역이므로 신경 쓸 필요 없다.
부팅 시 .bss 섹션은 0으로 초기화시키기만 하면 된다.
이렇게 했으면 Id로 기존과 동일한 명령으로 링킹 과정을 수행하고 부팅 시 다음과 같
은 코드가 먼저 호출되 게 해 .data 섹션을 [RAM상의 .data 섹션 주소]로 복사한다.
〔예제 5-36)

extern
extern
extern
extern
extern

.data 섹션의 RAM으로 이동과 .bss 섹션 초기화 코드

unsigned char
unsigned char
unsigned char
unsigned char
unsigned char

__data_loc_start;
__data_start;
__data_end;
______________
___________

void Xiplnit() {
unsigned char *src, *dst;
src = &_____ data_loc_start;
dst = &_____ data_start;
/* . data 섹션 복사 */
while (dst < &________ data_end) {
*dst++ = *src++;
}
/* .bss 섹션초기화 */
for (dst = &___________________ dst < _____ ____________ __
*dst = 0;

이후에 .text 섹션에서 전역변수의 참조는 모두 복사한 RAM에서 이루어진다. 그러면
프로그램은 정상적으로 동작한다.
360 3부- 컴파일과 링킹

===== PAGE 362 =====
I 오버레이(overlay)
오버레이 (overlay)는 과거 메모리가 부족한 시절에 적은 양의 메모리로 큰 프로그램을
동작시키기 위해 사용하던 기법이다. 현재의 시스템들은 메모리가 넉넉하기 때문에 메
모리를 줄이기 위해 오버레이를 사용하지는 않고 느린 메모리(예: NOR flash)와 빠른
메모리(예: SRAM)가 있을 때 느린 메모리의 코드를 빠른 메모리로 이동시켜 수행하고
자 할 때 사용한다.
쉽게 설명하면 프로그램을 수행할 때 파일 또는 플래시에 있는 특정 함수를 SRAM에
있는 오버레이 영역에 복사한 후 수행한다. 이후 다른 함수를 수행해야 한다면 역시 수
행할 다른 함수를 SRAM에 있는 오버레이 영역에 복사한 후 수행한다.
이렇게 하면 중간 중간 코드를 복사해야 되는 오버헤드는 증가하지만 메모리를 아낄
수 있다. 또 시스템에 따라서는 매우 빠른 메모리를 잘 활용함으로써 수행 성능을 증가
시킬 수도 있다.
오버레이를 테스트할 수 있게 보여주면 좋겠지만 불행히도 오버레이는 XIP와 마찬가
지로 애플리케이션으로 쉽게 보여주기 힘들다. 여기서 필자는 그냥 오버레이를 어떻게
하면 되는지 간략하게 예를 들어 살펴보겠다.
〔예제 5-37)

main.c 파일 내용

extern char load_start_funcl, load_stop_funcl;
extern
char
load_start_func2z
void fund () ;
void func2();

load_stop_func2;

int main() {
int i;

：

for (i=0; i < 2; i++) {
memcpy((char *) 0x80000000, &__ load_start_funcl, &____________ load_ ；
stop_funcl - &________ load_start_funci) ;
fund () ;
:
memcpy ((char
*) 0x80000000, &_____ load_start_func2, &__________ load_ ：
stop_func2 - &_______ load_start_func2);
；
func2();
：
}

：

return 0;

；

5장_ Id linker 361

===== PAGE 363 =====
〔예제 5-38)

(A) funcl.c 파일 내용

void fund () {

(i=0; i < 3; i++) {
/* fund loop body */

(B) func2.c 파일 내용

void func2()

(i=0; i < 2; i++) {
/* func2 loop body */

SECTIONS
{
. = [RAM 시작주소]
.text : { *(.text) }
.rodata : { *(.rodata) }
.data : { *(.data) }
.bss : { *(.bss) }
OVERLAY 0x80000000 : AT(0x90000000) {
. fund { fund. o (. text) }
.func2 { func2.o(.text) }

위와 같은 소스 코드와 링커 스크립트가 있을 때 오버레이를 위한 컴파일과 링킹은 다
음과 같다.
$ gcc -c main. c fund. c func2 . c
$ Id -T overlay.Ids -o test main.o fund.o func2.o

일반적인 컴파일 방법과 동일함을 알 수 있을 것이다. overlay.lds에 OVERLAY 명령으
로 오버 레이 섹션들을 기술한다.
오버레이 명령에서 0x80000000번지는 오버레이 영역으로 코드들을 복사해 수행할 영
역이다. 뒤에 오는 0x90000000번지는 해당 코드들이 위치하는 영역이다. 이런 코드들
은 _Joad_start_［섹션명］, __Joad_stop_［섹션명］과 같이 참조할 수 있다.
오버레이 코드를 수행할 때는 다음과 같이 먼저 복사를 하고 수행한다.
memcpy((char *)0x80000000, ___________ load_start_funcl, ___________l o a d _ s t o p _ f u n c l __load_start_funcl);
fund () ;

memcpy((char *)0x80000000, ___________ load_start_func2, __________ l o a d _ s t o p _ f u n c 2 __load_start_func2);
func2();

362 3부— 컴파일과 링킹

===== PAGE 364 =====
이상 오버레이 설명을 마친다. 필자가 지금껏 오버레이를 사용해야 되는 경우를 본 적
은 단 한 번밖에 없다. 사실 오버레이는 거의 사용되지 않는다. 하지만 이런 기법도 있
다는 걸 알아 두면 언젠가는 요긴하게 사용될 것이라 생각한다.

I 필요한 데이터 바이너리 이미지에 포함
이런 일을 경험한 적이 있는가? 코덱이나JPEG 이미지 파일을 임베디드 시스템에서 디
코딩해야 하는데, 해당 임베디드 시스템에 아직 파일 시스템이 없다. 그렇다면 어떻게
테스트할 수 있을까?
이런 경우 해당 파일을 .data 섹션에 포함시키면 메모리에서 파일을 읽어 작업을 진행
할수있다.
〔예제 5-40)

data.img 파일 내용

test!! 1
test!! 2
test!! 3
test!! 4
test!! 5
test!! 6

먼저 ［예제 5-4이과 같은 데이터 파일이 있다. 현재 필자는 간단하게 텍스트 형식의 파
일을 만들었는데, 동영상 파일이든지 음악 파일이든지 뭐든 상관없다.
〔예제 5-41)

Ids.S 파일 내용

.section .data
. globl file_start
. globl file_end
file_start:
. incbin ’’data. img"
file_end:

해당 파일을 실행 바이너리 이미지에 포함시키려면 위와 같은 어셈블리 파일을 작
성한다. 살펴보면 .incbin "data.img" 문장에 의해 data.img 파일을 바이너리 형태로

incl니de하는 것을 알 수 있다.

5장_ Id linker

363

===== PAGE 365 =====
(예제 5-42]

main.c 파일 내용

#include <stdio.h>
extern char file_start;
은xt은rn char file_end;

int main() {
char *i;
for (i=&file_start; i<&file_end; i++) {
putchar(*i);
fflush (stdout) ;
}
return 0;

main.c 파일을 위와 같이 작성하고 다음 명령으로 컴파일하면 정상적으로 컴파일된다.
$ gcc -o test main.c Ids.S

실행시켜 보면 다음 그림과 같이 datajmg 파일이 바이너리 이미지 속에 포함되어 있
음을 확인할 수 있다.

[그림 5-38] 실행 바이너리에 데이터 파일 포함

이런 예는 파일 시스템이 존재하지 않는 시스템에서 무언가를 테스트하고자 할 때 요
긴하게 사용할 수 있다.
지금까지 Id를 사용한 고급 링킹 테크닉을 알아보았다. 지금 설명한 것들 외에도 상당
히 많은 링킹 테크닉이 있지만 지면 관계상 이만 생략한다. 그런 링킹 테크닉은 독자가
직접 찾아보기 바란다. 지금까지 배운 내용을 토대로 충분히 고급 링킹 테크닉들을 이
해할 수 있을 것이다.

364 3부- 컴파일과링킹

===== PAGE 366 =====
06 L 라이브러리를 만들기
이제 라이브러리를 한번 만들어 보자. 이전에 C 컴파일 과정을 이해한 독자라면 라이
브러리를 만드는 일은 너무나 쉬울 것이다. 그냥 간단한 명령 몇 줄로 라이브러리를 만
들수 있다.
정작 중요한 것은 라이브러리의 개념과 라이브러리의 의미, 그리고 라이브러리가 어떤
식으로 사용되는지 이해하는 것이다.
라이브러리는 미리 컴파일된 오브젝트들의 집합이다. 이런 오브젝트들은 자주 사용하
는 함수의 소스를 컴파일해 만든다. 라이브러리를 사용하는 이유는 자주 사용하는 함수
들을 쉽게 사용하려는 것이 주목적이고, 미리 컴파일되어 있어 링킹만 하면 바로 사용
가능하므로 컴파일 시간을 단축시킬 수 있기 때문이다. 그 외에도 라이브러리를 사용하
는 다른 장점이 있는데, 그에 대해서는 공유 라이브러리를 설명할 때 하기로 한다.
이런 라이브•러리는 세 가지 종류가 있다. 하나는 정적 라이브러리이고, 다른 하나는 공
유 라이브러리이며, 마지막 하나는 동적 라이브러리다. 정적 라이브러리와 공유 라이브
러리, 동적 라이브러리가 근본적으로 다른 것은 아니다. 무슨 말인가 하면 각각의 소스
는 하나의 소스로 동일하다. 단지 컴파일 과정에서 컴파일하는 옵션이 다르고 사용하는
방식이 약간의 차이가 있을 뿐이다.
정적 라이브러리는 컴파일 시 링커에 의해 라이브러리의 오브젝트 코드가 만들려는 바
이너리에 추가되는 형태로 사용된다. 반면 공유 라이브러리는 컴파일 시에 라이브러리
함수가 사용된 곳에 공유 라이브러리를 사용한다는 표시만 해놓고 바이너리가 실행되
는 순간에 동적 링커(ld-linux.so.2)에 의해 링킹된다.
이미 이전 과정을 잘 따라온 독자라면 다 이해되었을 거라 생각된다. 그럼 본격적으로
라이브리를 만들어 보자.

I 정적 라이브러리 만들기
정적 라이브러리는 컴파일되어 있는 오브젝트 파일들이 하나의 파일로 묶여 있는 형태
다. 반면 공유 라이브러리는 컴파일되어 있는 오브젝트 파일 자체다. 백문이 불여일견
백견이 불여일타라고 실제로 한번 만들어보자.

5장_ Id linker

365

===== PAGE 367 =====
먼저 라이브러리를 만들기 위한 소스 코드를 작성해야 한다.
〔예제 5-43〕 filel.c 소스 코드

#include <stdio.h>
void fund ()
{
printf("hello funcl\n");
}
void func2()
{
printf("hello func2\n");
}

〔예제 5-44)

file2.c 소스 코드

#include <stdio.h>
void func3()
{
printf("hello func3\n");
}

〔예제 5-45)

mylib.h 소스 코드

void fund (void) ;
void func2(void);
void func3(void);

filel.c 와 file2.c 가 라이브러리로 만들 소스 파일이다. mylibh 파일은 filel.c와 file2.c
에서 작성한 함수의 원형이 들어있는 헤더 파일이다. 이런 헤더 파일이 라이브러리를
만들 때 반드시 필요한 것은 아니다.
헤더 파일은 라이브러리를 사용할 때 함수의 원형을 추가하기 쉽게 하려고 만든 것이
다. 라이브러리를 만들 때는 보통 이렇게 라이브러리에 들어가는 함수들의 원형이 적힌
헤더 파일을 같이 만들어 준다. 그래야만 나중에 라이브러리를 사용할 때 소스 내에 헤
더 파일을 include해 쉽게 사용할 수 있고, 또한 라이브러리 안에 어떤 함수가 들어있
다는 것을 쉽게 알 수 있기 때문이다.

366

3부_ 컴파일과 링킹

===== PAGE 368 =====
소스가 작성되었으면 컴파일한다. 정적 라이브러리를 만드는 컴파일 옵션은 일반 오브
젝트를 컴파일하는 것과 동일하다.
gcc -c filel.c file2 . c

위 명령으로 컴파일하면 다음과 같이 filel.o, file2.o 두개의 오브젝트 파일이 만들어진다.

［그림 5-39］ 라이브러리로 만들 소스 파일 컴파일

이제 두 오브젝트를 다음 명령으로 묶어주면 정적 라이브러리가 만들어진다.
ar rscv libmy. a filel. o file2 . o

［그림 5-4이 libmy.a 라이브러리 제작

ar 명령은 여러 개의 파일을 하나의 파일로 묶을 때 사용한다. ar 명령으로 반드시 라이
브러리만 묶으라는 법은 없다. 묶고 싶은 파일이 있요면 ar 명령으로 묶으면 된다. 물론

ar보다 더 좋은 tar가 있긴 하지만 말이다. tar와 ar 이름이 비슷하지 않은가? 둘 다 ar
이 archive의 의미이기 때문이다. 이렇게 여러 파일이 하나의 파일로 묶인 파일을 아카
이브 파일이라 한다.

ar 명령에서 s 옵션은 아카이브 파일 내부에 오브젝트 파일의 인덱스를 생성할 때 사용
한다. s 옵션을 주지 않아 인덱스가 생성되지 않았다면 ranlib libmy.a 명 령으로 인덱스
를 생성해 주어야 한다.

5장_ Id linker

367

===== PAGE 369 =====
그럼 이렇게 만든 라이브러리를 사용해 보자.
〔예제 5-46)

like.c 소스 코드

#include <stdio.h>
#include "mylib.h"
int main()
{
fund () ;
func2();
func3 () ;
return 0;
}

like.c를 작성하고 다음 명령으로 컴파일한다.
gcc -o like like.c -L./ -Imy

libmy.a 파일은 기본 라이브러리 디렉토리에 없기 때문에 위와 같이 -L 옵션을 사용해
gcc에 라이브러리를 찾을 디렉토리를 지정해 주어야 한다.
컴파일해서 실행해 보면 다음과 같이 정상적으로 실행되는 것을 확인할 수 있다.

[그림 5-41] like.c 컴파일

정적 라이브러리 제작은 이것으로 끝났다. 무척이나 쉽지 않은가? ar 명령의 옵션 몇
가지 만 소개하면 다음과 같다.
ar rus ［라이브러리 이름］ ［오브젝트 파일들］
ar ds ［라이브러리 이름］ ［오브젝트 파일들］
ar x ［라이브러리 이름］
ar t ［라이브러리 이름］

368

3부_ 컴파일과 링킹

: 기존 아카이브 파일에 오브젝트 추가
: 기존 아카이브 파일에서 오브젝트 제거
: 아카이브에서 오브젝트 파일 추출
: 아카이브에 있는 파일 리스트 출력

===== PAGE 370 =====
I 공유 라이브러리 만들기
이전에도 설명했듯이 정적 라이브러리를 사용해 컴파일하는 방법과 공유 라이브러리
를 사용해 컴파일하는 방법 둘 다 장단점이 있다. 정적 라이브러리를 사용하면 속도가
빠르고 바이너리를 배포할 때 제한이 없다. 그러나 사이즈가 크다는 단점이 있다.
반면 공유 라이브러리를 사용하면 사이즈는 작지만 속도가 약간 느리고 바이너리를 배
포할 때 컴파일할 당시에 사용한 공유 라이브러리와 같은 메이저 버전을 가지는 공유
라이브러리가 있는 시스템에서 만 동작하는 단점이 있다.
둘 다 장단점을 가지고 있지만 다음 이유 때문에 공유 라이브러리를 사용해 컴파일하
는 것이 좋다.

abc 정적 라이브러리를 사용해 컴파일한 파일이 있었는데, abc 라이브러리에 보안 결
함이 발견되었다. 그러면 abc 라이브러리를 사용해 컴파일한 모든 파일을 바꿔야 한다.
그렇지만 공유 라이브러리를 사용해 컴파일하였다면 abc 공유 라이브러리만 바꾸면
된다.
공유 라이브■러리를 이용해 컴파일한 파일들은 모두 실행 시 공유 라이브러리와 링크되
기 때문에 하나의 공유 라이브러리만 바꾸면 된다. 이렇게 라이브러리에 문제가 생겨
바꿔야 될 파일이 몇 개밖에 없다면 상관이 없지만 전 세계적이라면 어떨까?
라이브러리에 의한 보안 버그는 가끔 있는 일이다. 실제로 2002년 3월에 z 라이브러리
에 의한 유명한 보안 버그가 있었다. z 라이브러리는 압축을 위한 루틴이 들어있는 라
이브러리였는데, z 라이브러리의 코드 내에 동적으로 할당한 메모리를 두 번 free하는
코드가 들어있었다. 이미 free한 메모리를 다시 free하면 시스템이 어떤 상황에 빠지게
될지 예측할 수 없다 z 라이브러리는 압축 기능을 사용하는 많은 애플리케이션（대표적
으로 gzip） 에 아주 광범위하게 사용되었는데, 문제는 많은 애플리케이션이 정적 라이
브러 리를 사용해 컴파일되 었다는 점 이다.
그 많은 파일을 다 바꾸려면 정말 끔찍할 것이다. 그리고 표면상 z 라이브러리를 사용
하였는지 사용하지 않았는지 알 수 없다. 특히 배포판에 들어 있는 실행 파일들은 사이
즈를 줄이기 위해 바이너리 내부의 심볼 테이블을 지워버리는데, 그러면 nm 명령으로
도 알 수 없다.
이럴 때 공유 라이브러리를 사용해 컴파일하였다면 /usr/lib/libz.so 파일만 바꾸면 쉽
게 해결할 수 있었을 것이다.

5장_ Id linker 369

===== PAGE 371 =====
여담이지만 Z 라이브러리 문제는 그보다 휠씬 더 심각했었다. 리눅스 커널 역시 압축
기능을 위해 Z 라이브러리를 사용하는데, 커널의 lib 디렉토리에 소스 형태로 들어있다.
애플리케이션이 예측 불가능한 상황에 빠지는 것도 문제지만 커널이 예측하지 못하는
상황에 빠지는 것에 비할 바는 아니다. 커널이 잘못되면 시스템을 망가뜨릴 수도 있다.
그렇기 때문에 정적 라이브러리보다는 공유 라이브러리를 사용하는 것을 장려하는 추
세다.
공유 라이브러리를 제작하려면 컴파일 옵션을 달리해야 한다. 다음과 같은 옵션으로 먼
저 소스 파일을 컴파일한다.
gcc -fPIC -c filel. c file2 . c

-fPIC 옵션은 위치에 관계없이 수행되는 코드（ PIC： Position Independent Code） 로
컴파일하라고 cel 컴파일러에 알려주는 옵션이다. 이렇게 컴파일하였으면 filel.c와

file2.c에 대한 오브젝트 파일인 fllel.o와 file2.o가 만들어지고, 이제 다음 명령으로 공
유 라이브러리를 제작하면 된다.
gcc -shared -Wlz -soname, libmy. so. 0 -o libmy. so. 0.0.0 filel .o file2 .o

-shared 옵션은 fllel.o와 file2.o를 링크할 때 정적 라이브러리와 동적 라이브러리가
같이 있다면 동적 라이브러리를 사용해 링크하라는 옵션이고, -W1 옵션은 -W1 옵션
뒤에 오는 옵션들을 gcc를 거치지 않고 링크（ collects에 바로 전달하라는 의미다. 그
래서 -Wl,-soname,libmy.so하면 링크인 collect》에 -soname libmy.so와 같은 형식
으로 바로 전달된다.

-soname 옵션은 만들어질 공유 라이브러리의 soname을 정하는 것이다. 이것은 파
일명과는 틀린 개념으로 지금과 같이 soname을 libmy.so.0라고 지어주고 파일명을

libmy.so.0.0.0인 공유 라이브러리를 만들었다면 이후 libmy.so（나중에 만드는 libmy.
so.0.0.0의 심볼릭 링크 파일）를 링크해 컴파일되는 모든 실행 파일은 실행될 때 동적
링크（ /lib/ld-linux.so.2） 가 공유 라이브러리를 찾을 때 libmy.so.0.0.0을 찾는 것이 아
니라 soname인 libmy.so.O（역시 libmy.so.0.0.0의 심볼릭 링크） 파일을 찾아 링크한다.
이런 식으로 soname을 붙여 사용하는 이유는 파일명과 상관없이 서로 다른 버전의 공
유 라이브러리를 융통성 있게 사용하기 위해서다. -o libmy.so.0.0.0은 만들어질 공유
라이브러리의 실제 파일명이다.

370 3부— 컴파일과 링킹

===== PAGE 372 =====
0.0.0 에서 제일 앞에 0은 메이저 버전으로, 라이브러리에 중대한 변화가 발생했을 때
바뀌는 번호다. 메이저 버전이 바뀌었다는 이야기는 이전 메이저 버전의 라이브러리와
새로 만든 라이브러리가 너무 바뀌어 도저히 호환이 안 된다는 의미와 같다. 그래서 메
이저 버전이 틀린 라이브러리로 컴파일된 실행 파일은 같은 이름(my)의 라이브러리가
있더라도 실행될 수 없다.
두 번째 0은 마이너 버전으로, 약간의 변화가 발생했을 때 변화되는 번호다. 마이너 버
전이 바뀜으로써 미치는 영향은 애플리케이션에 크지가 않다. 마이너 버전이 달라도 메
이저 버전만 같으면 실행될 때 링크될 수 있다.
마지막 0은 패치 버전을 의미하고 소스의 변경 없이 라이브러리를 새로 만들거나 아니
면 아주 사소한 변화가 생겼을 때 변하는 버전이다.
위 명령을 내리면 다음과 같이 libmy.so.0.0.0 공유 라이브러리가 만들어진다.
터 root@os：/temp/book/compiler/lib
— --------- ---------- -------------------------------------- ---------- - ---------- --- --- -- ——

[rootQos lib]# gcc -shared -W1soname,libmy.so.0 -o libn으.so.0.0.0 filel
2.0
[rootBos lib]tt Is libmy.so.0.0.0
libmy so.8.6.0 |
[root（흐os lib]#

처
[그림 5-42] libmy.so.0.0.0 공유 라이브러리 링크

이렇게 만들어진 libmy.so.0.0.0은 ELF 포맷으로 된 하나의 바이너리 파일이다. readelf

-a libmy.so.0.0.0 명령으로 ELF 포맷의 정보를 읽어보면 이 바이너리의 속성과 이 라
이브러 리가 필요한 동적 라이브러 리와 soname을 볼 수 있다.
라이브러리를 만들었으면 libmy.so.0.0.0 라이브러리를 이용해 컴파일되는 실행 파일
들을 링크할 때 링크(collect》)가 찾을 수 있게 Hbmy.so.0.0.0 파일의 심볼릭 링크 파
일인 libmy.so 파일을 만들어야 한다.
그리고 이후 이렇게 컴파일된 실행 파일이 실행될 때 동적 링크(/lib/ld-linux.so.2)가

soname으로 찾을 수 있게 soname을 파일명으로 하는 libmy.so.0.0.0 파일의 심볼링
링크를 만들어야 한다.
In -s libmy.so.0.0.0 libmy. so # gcc 링크를 위한 파일
In -s libmy. so. 0.0.0 libmy.so. 0 # 동적 링크를 위한 파일

5장_ Id linker

371

===== PAGE 373 =====
Is -al 명령을 내려 보면 다음과 같은 모습으로 되어 있어야 한다.
87x14 -|Dlx|

O root@os：/temp/book/compiler/lib
[rootl흐 os 1:

I싀

합계 40
drwxr-xr-x
drwxr-xr-x

-t*w-r--r
- ----------------irwxrwxrwx
irwxrwxrwx
-rwxr-xr-x

2 root
7 root
1 root
root
root
root
root
1 root
1 root
root
root

root
root
root
root
root
root
root
root
root
root
root

04：21 .
00:03 ..
08:05 Filel.c
02:17 filel.o
00:07 File2.c
02:17 File2.o
04:20
libmy.so -> libny.so.0.0.8
04:20
libPiy.so.O ~> libmp.so.0.8.8
04:06 |libay.so.0.8.8
00:58
00:88 mulib.h

버

[root@os libltt

[그림 5-43] libmy.so.0.0.0 파일을 심볼릭 링크 건 모습

자, 여기까지 다 되었다면 이제 동적 링크(/lib/Id-linux.so.2)가 찾을 수 있게 libmy.

so.0.0.0 파일이 있는 디렉토리를 설정해야 한다. /etc/ld.so.conf 파일을 열어 libmy.
so.0.0.0 파일이 있는 디 렉토리를 다음과 같은 모습으로 추가한다.

[그림 5-44] /etc/ld.so.conf 파일에 libmy.so.O 파일이 있는 디렉토리를 추가한 모습

필자의 경우 /temp/book/compiler/lib 디렉토리에 libmy.so.0.0.0 파일의 심볼릭 링
크인 libmy.so.O 파일이 들어있다.
이제 다음 명령으로 실제 동적 로더가 읽어들이는 /etc/ld.so.cache 파일을 새로 만든다.
丄 dconfig

.

libmy.so 파일을 링크해 컴파일된 실행 파일의 동적 로더는 수행될 때 /etc/ld.so.
preload, /etc/ld.so.cache 파일순으로 파일을 읽어 어떤 디렉토리에 공유 라이브러리
가 있는지 알아낸다. 기본적으로 /usr/lib 디 렉토리를 찾지만 /usr/lib 디렉토리가 아닌
다른 디렉토리에 공유 라이브러리가 있다면 /etc/ld.so.conf 파일에 디렉토리를 추가
하고 Idconfig 명령으로 /etc/ld.so.cache 파일을 갱신해야 한다(/usr/lib 디렉토리에
복사하면 귀찮게 위 절차를 하지 않아도 된다).

372 3부_ 컴파일과 링킹

===== PAGE 374 =====
이제 공유 라이브러리를 사용하기 위한 준비가 다 되었다. 그러면 공유 라이브러리를
사용하게 이전의 like.c를 다음 명령으로 컴파일한다.
gcc -o like like.c -L./ -Imy

위 명령으로 컴파일한 후 Idd like 명령으로 like 파일이 사용하는 공유 라이브러리 목
록을 읽어보면 다음과 같이 libmy.so.O를 사용한다는 것을 알 수 있다. Idd 명령은 바이
너리 파일이 요구하는 공유 라이브러리 목록을 볼 때 사용한다.

[그림 5-45] like 파일 컴파일 후 Idd 명령으로 사용하는 공유 라이브러리 목록을 출력

위와 같이 사용하는 공유 라이브러리 목록이 나오고 그 중 libmy.so.0이 필요하다는 것
을 알 수 있다. 그리고 다음 동적 링크로 /lib/ld-linux.so.2를 사용하는 것을 알 수 있다.
컴파일된 like 실행 파일을 실행해 보면 다음과 같이 정상적으로 수행되는 것을 알 수
있다.

[그림 5-46] ./like 명령 실행 결과

이제 라이브러 리 제작도 할 수 있게 되 었다.

5장_ Id linker 373

===== PAGE 375 =====


===== PAGE 376 =====
6
gas assembler

01 gas를사용해 어셈블하기
02 어셈블리파일의작성
03 인라인 어셈블리의 사용

===== PAGE 377 =====
Let s S*t■느dy
지금부터 다룰 내용은 9as에 관한 내용이다. gas는 리눅스 시스템에서 사용되는 어셈
블러다. 6장에서는 gas 어셈블러를 사용한 어셈블링 기법과 간단한 어셈블리 파일 작성
법, 인라인 어셈블리 사용법을 알아본다.
필자는 x86과 ARM 아키텍처를 골고루 설명하고자 노력하겠지만 테스트하기 쉬운 x86
쪽으로 설명이 치우치는 것은 어쩔 수 없을 것 같으니 그 점은 양해 바란다.

===== PAGE 378 =====
01 L
gas를 사용해 어셈블하기
프

''•느—*'

gas 는 프로판 가스, 도시 가스와 같은 가스가 아니 다. gas (GNU Assembler)는 GNU
에서 만든 어셈블러를 말한다.

gas 는 GCC 패키지에 들어있지 않고 Binutils 패키지에 들어있다. gas 의 리눅스 명령
은 통상 /usr/bin/as 로 사용된다. 그래서 GNU 어셈블러라는 의미로 말할 때는 gas 라
는 단어를 사용하고, 어셈블러 명령을 이야기할 때는 as를 사용하기로 한다. 둘 다 같은
것이니 의아해 하지 않았으면 한다.

gas의 특징은 상당히 많은 아키 텍처를 지원한다는 점이다. 물론 그렇더라도 x86용으로
컴파일된 gas가 갑자기 ARM 어셈블리 파일을 어셈블할 수는 있는 것은 아니다. 여기
서 gas가 많은 아키텍처를 지원한다는 의미는 여러 아키텍처의 gas를 하나의 소스에서
빌드할 수 있다는 의미다. 현재 gas 최신 버전에서 지원하는 아키텍처는 다음과 같다.
Alpha,
ARC,
ARM,
CRIS,
D10V,
D30V,
i386,
i960,
IA-64,
IP2K,
M32C, M32R, M680X0, M68HC11, MCORE, MIPS, MMIX, PDP11, picoJava,
PowerPC, SPARC, TIC54X, Z80, Xtensa

이런 특징으로 말미암아 여러 아키텍처에 이식해야 되는 소스를 작성할 때 동일한 어
셈블리 지시자를 사용하는 것이 가능하다. 또 gcc가 여러 아키텍처를 지원하는 데 gas
가 일조를 한다.
이렇게 많은 아키텍처를 지원한다고 해서 gas가 최고로 훌륭한 어셈블러라 보기는 어
렵다. gas는 구닥다리 1 패스 방식의 어셈블러다. 여기서 1 패스라는 말의 의미는 어셈
블리 파일을 한 번에 읽어 들이면서 바로 어셈블링한다는 의미다. 이렇게 하면 어셈블
속도가 향상될 수 있다. 그렇지만 융통성이 떨어질 수 있다. 실제로 gas는 몇 가지 측면
에서 융통성이 다소 떨어진다.
그렇다고 할지라도 gas가 훌륭한 어셈블러 축에 속하는 것은 사실이다. 상용 어셈블러
라 할지라도 gas만한 활용성과 확장성을 지닌 어셈블러는 많지 않기 때문이다.
그러면 본격적으로 gas에 대해 알아보자.

6장_ gas assembler 377

===== PAGE 379 =====
I gas의 이해
여기서 짚고 넘어가야 할 것이 있다. 필자는 gas를 많이 사용해 보지 않았다.
“시작하기도 전에 이건 뭔 소리인가? 그럼 gas 사기꾼이란 말인가?”
이렇게 생각하는 독자가 있을지 모르겠다. 하지만 안심하라! 그것은 그럴만한 이유가
있기 때문이다. 사실 필자는 다른 사람들에 비해 어셈블리 언어를 많이 사용한 사람 축
에 들어간다. 그간 필자는 운영체제, 컴파일러, 디버거 같은 시스템 소프트웨어를 주로
개발해 왔기 때문이다.
때문에 어셈블리 언어는 필자에게 매우 친숙한 언어이고, 한창때는 C 소스를 실시간에
머리만으로 컴파일해 어셈블리로 볼 정도로 익숙한 언어였다. 그리고 실제로 많은 어셈
블리 파일을 작성하였다.
하지만 한창 어 셈블리를 사용할 때도 gas로 어셈블해 본 일은 거의 없다. 몇 번 있긴 한
데 그건 정말 손에 꼽을 정도다. 그러면 무엇으로 어셈블했는가? 바로 gcc를 사용해 어
셈블했었다.
나중에 알게 되겠지만 gas 를 사용해 어셈블하는 것보다 gcc를 사용해 어셈블하는 것
이 훨씬 편리한 경우가 많이 있다. gcc 를 사용해 어셈블하는 것이 편한 대표적인 경
우는 C 전처리기를 사용할 수 있다는 점이다. 때문에 어셈블리 파일 내에서 #include

Khardware.h"와 같은 문장을 사용할 수 있다. 그리고 각 아키텍처의 어셈블리 파일마
다 아키텍처에서 지원하는 인스트럭션을 체크하기 위해 별도의 옵션을 gas에 주어야
하는데, gcc를 사용하면 gcc가 알아서 gas를 호출할 때 이런 옵션들을 추가한다. 그렇
기 때문에 gas 를 호출해 직접 어셈블하는 것보다는 gcc 를 사용해 어셈블하는 경우가
많은 것이다.
그래서 필자는 잘 사용하지도 않는 gas를 열심히 알려주기보다는 gas가 뭐라는 것 정
도로만 이해할 수 있도록 알려주려 한다. 한마디로 말해 그냥 대충대충(?) 알려주려 하
니 독자들도 가벼운 마음으로 그냥 대충대충 건성으로 듣기 바란다.

378 3부_ 컴파일과 링킹

===== PAGE 380 =====
이전 컴파일 과정을 본 독자라면 Id로 링킹 이전에 as가 호출되어 어셈블 과정을 수행
한다는 점을 기억하고 있을 것이다.

cppO 또는 cc1 -E
전처리기

c&S1

일러

[그림 6-1] gcc 컴파일 과정

위 그림에서 볼 수 있듯 CC1 으로 컴파일된 like.s는 as로 어셈블되어 like.o 오브젝트로
만들어지고, 이후 collect』로 like 실행 바이너리가 된다. 여기서 as가 바로 gas다.
컴파일 순서로만 본다면 Id 설명 이전에 gas 를 먼저 설명했어야 한다. 하지만 이렇게
순서를 바꾼 이유는 ELF 바이너리 포맷을 이해하고 있어야 gas를 제대로 이해할 수 있
기 때문이다. 때문에 독자가 쉽게 이해할 수 있게 설명 순서를 바꾼 것이다.
그러면 이전에 컴파일 과정에서 as가 호출되는 부분을 되짚어 보자.
$ gcc -o like like.c -v -save-temps

like 실행 파일을 만들 때 위와 같이 명령을 내리면 다음과 같이 컴파일되었다.

6장_ gas assembler 379

===== PAGE 381 =====
root@os：/temp/like

-------------------------------------------------------------- : ■ .............................. •.스...;—그===玄쓰^^^^^또

[root(흐os like]tt gcc -u -saue-tenps -o like like.c
Reading specs From /usr/lib/gcc/i386-redhat-linux/4.1.2/specs
Target: i386-redhat-linux
Configured with: ../configure ——preFix=/usr ——一-info
dir=/usr/share/info ------------------------------------------------ ------------------------------------------------------ enable-checki
- -----------------------------------------------------------------enable-----------------------------------------------------------------------------------ceptions --------------------------------------------------------------------------------------------------------------------------- ---- enable-j
- ------------------------------------------------------ ---------------------------------- --------------------------------------------------------------------aua-1.5.0—gcj-1.5.0.0/jre -------------------------------------------------------------------------- —-enable-jaua-maintain
- ---------------------------------------------------------------------------------------------------------- .jar---------------------------------------------——host=i386—redhat-iinux
Thread model: posix
qcc uersion 4.1.2 28B7Q925 (Red Hat 四.1.2-27)________________________________________________________
/usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl -E -quiet -u like.c -intune=g
eneric -Fpch-preprocess -o like.i
ignoring nonexistent directory 'Vusr/lib/gcc/iSSS^Tedhat-rinux/ii.l .2/”T77Z
/.. ./i386—redhat—linux/include"
ttinclude "—" search starts here:
Itinclude <—> search starts here:
/usr/local/include
/usr/lib/gcc/i386-redhat-linux/4.1.2/include
/usr/include
End of search list._______________________________________ _________________________
/usr/libexec/gcc/i386-redhat-linux/4.1.2/ccl -fpreprocessed like.i -quiet
—dumpbase like.c -mtune=generic -auxbase like -uersion -o like.s
CHUCuersion 4.1.2(Red Hat 4.1.2-27) (i3S6-redhat-linux)
compiled by GNU C uersion 4.1.2 28078925 (Red Hat 4.1.2-27).
GGC heuristics: --------------------------ggc—min-expand=64 ——ggc-nin-heapsize=64411
Compiler executable 드hecksum 53c9F9515bF7a』»d930482540205071F7
as -U —Qy —o like.o_like.g]
GNU
assembler
uersion
2.17.50.0.12-4
(i386—redhat-iinux)
using
BFD
uersion
2.17.50.0.12—4 20870128______________________________ ________________________________________
/usr/libexec/gcc/i386-redhat—linux/4.1.2/collect2 —-eh-Frame-hdr -m elfi
386 --------------------------------------dynamic-linker Zlib/ld-linux.so.2 -o like Zusr/lib/g
cc/i386-redhat-linux/4.1.2/../crtl.o /usr/lib/gcc/i386-redhat-linux/
4.1.2/../.../crti.o /usr/lib/gcc/i386—redhat-linux/4.1.2/crtbegin.o -L/u
sr/lib/gcc/i386-redhat-linux/4.1.2 -l_/usr/lib/gcc/i386-redhat-linux/4.1.2
-L/usr/lib/gcc/i386-redhat-linux/4.1.2/.like.oj—Igcc --as-needed Igccs ------------------------------------ ---- -Igcc --as-needed -Igccs ——/usr/li
b/gcc/i386-redhat-linux/4.1.2/crtend.o /usr/lib/gcc/i386—redhat-linux/4.1.
2/../../../crtn.£_____________________________________________________________________________________
[root@os like]tt |

[그림 6-2] like 실행 파일 컴파일 과정

여기서 as가 호출되는 부분을 보면 다음과 같은 명령으로 호출됨을 알 수 있다.
$ as -V -Qy -o like.o like.s

여기서 -V 옵션은 단순히 gas의 버전을 화면에 출력하라는 옵션이다. 그래서 as 명령
밑에 as 버전이 출력된 것이다. -Qy 옵션은 as가 지원하는 옵션이 아니므로 as 내부적
으로 그냥 무시된다.
때문에 쓸모없는 옵션들을 제외하고 실제 유효한 옵션들만 모아 as 명령을 재구성해
보면 다음과 같다.
$ as -o like.o like.s

자, 이 명령이 바로 as를 사용해 어셈블하는 명령이다. x86 as 명령 사용법은 이것으로
끝이다. 이제 x86 as를 알고자 하는 독자는 as 사용에 대해 배울 것을 다 배웠다. 나머
지는 알아도 그만, 몰라도 그만이다.

380

3부_ 컴파일과 링킹

===== PAGE 382 =====
하지만 ARM 환경에서 작업하는 독자라면 이것 외에도 몇 가지 옵션을 기억해 둘 필요
가 있다. 때문에 이제부터는 알아 두면 좋은 몇 가지 옵션을 알아본다.

I as를 사용한 어셈블 실습
먼저 실습을 위해 다음과 같은 어셈블리 파일을 작성하자.
〔예제 6-1〕 like.S 파일 내용

. text
.globl main
main:
subl
movl
call
addl
ret

$4, %esp
$likestr, (%esp)
puts
$4, %esp

likestr:
.string "I like you!

위 소스는 like.c와 같은 기능을 수행하는 어셈블리 파일을 작성한 것이다. 위 파일에
다음과 같은 명령을 내리면 어셈블하고 링킹한다. Id 링커 사용은 이전에 열심히 설명
했으니 따로 설명하지 않겠다. Id 명령이 잘 이해가 안 되는 독자는 5 장 “Id linker’
과정을 다시 한 번 보기 바란다.
$ as -o like.o like.S
$
Id
—L/usr/lib/gcc/i386—redhat-linux/4.1.2
Id-linux.so.2
-o
like
/usr/lib/crtl.o
crtn.o like.o -1c -Igcc -lgcc_s

-dynamic-1inker
/usr/lib/crti.o

/lib/
/usr/lib/

gcc를 사용해 그냥 컴파일하려면 다음 명 령을 사용한다.
$ gcc -o like like.S
root@seryer7work/book/utils new/as
[ro(rt'6Aeruer |；'5]井|‘；|"；,‘‘“7：*"히丄丁휴으:；^
[root@seruer as]# Id -L/iisr/lib/gcc/i386-redhat-linux/4.1.2 -dyna
mic-linker /lib/ld-linux.so.2 -o like /usr/lib/crti.o /usr/lib/cr
ti.o /usr/lib/crtn.o like.o -1c -Igcc -lgcc_s
[root@seruer
as]tt
Jroot@seruer
as]# Is like
b』怨,.」
[root@seruer
JrootBserue흐
|i ""iike you?]
[rootBseruer

as]tt
as]# ./like
as]# |

[그림 6-3] like.S 파일 어셈블 및 링킹

6장_ gas assembler 381

===== PAGE 383 =====
이렇게 만들어진 like 바이너리를 수행시키면 ［그림 6-3］ 과 같이 정상적으로 수행되는
것을 확인할 수 있다. 이때 알아 두면 좋을 옵션들을 정리해 보면 다음과 같다.

n -al 옵션（아키텍처 공통）
-al 옵션은 아키텍처 공통 옵션으로 어떤 아키텍처에서든지 사용 가능하다. -al 옵션은
각 어셈블리 라인이 어떤 인스트럭션으로 컴파일되는지 알 수 있는 리스트를 출력한다.
그래서 as -o like.o like.S -al 명령을 내리면 다음과 같은 결과가 출력된다.

［그림 6-4］ -al 옵션으로 컴파일한 모습

알고 있으면 정말 어쩌다 한 번쯤은 사용할 일이 있겠지만 거의 사용되지 않을 것이니
그냥 넘어가자.

@ -defsym ［심볼명］듸심볼 값］ 옵션（아키텍처 공통）
입력 파일을 어셈블하기 전에 ［심볼명］ 심볼을 ［심볼 값］의 값으로 정의한다. 그래서
다음과 같이 명령을 내리면 aaa란 심볼이 0x12345678의 값을 가지고 like.o의 심볼 테
이블에 추가되는 것을 확인할 수 있다.
$ as -o like.o like.S -defsym aaa=0xl2345678

382 3부— 컴파일과 링킹

===== PAGE 384 =====
j/1 root@server：/work/book/utils new/as
[root@server
[rooteseruer
[root@seruer

35]씨35三0 like.o :Lik'e.S'-deFsym aaa=8x12345678
as]tt
as]# readelf -s like.o

Symbol table
'.syntab' contains 8 entries:
Ualue Size Type
Num:
Bind Uis Ndx Name
B: 0808OBB8
으 NOTYPE LOCAL DEFAULT UND
0 NOTVPE LOCAL DEFAULT ABS aaa
| 1： 12345678
2： 00080000
DEFAULT
0 SECTION LOCAL
3: 08000000
SECTION LOCAL
DEFAULT
4： 00000000
SECTION LOCAL
DEFAULT
5： 00000013
NOTVPE
LOCAL
DEFAULT
1 likestr
6： 00000800
NOTVPE
GLOBAL DEFAULT
1 main
7： 00000800
NOTVPE
GLOBAL DEFAULT
UND puts
[rootSseruer as]tt |

I거
[그림 6-5] -defsym 옵션을 사용해 심볼 추가

이 옵션은 존재하지 않는 심볼에 대해 코드에서는 심볼 참조가 있지만 실제로는 참조
되지 않는 심볼이 있을 경우 이를 컴파일 과정에서 무시할 때 사용 가능하다. 예를 들
면 다음과 같은 경우다.
〔예제 6-2〕 like.c 파일 내용

#include <stdio.h>
extern int aaa;
int main() {
printf ("I like you!
return 0;
}
void func() {
printf(”aaa = %d\n", aaa);
}

[예제 6-2] like.c 파일에서 호출되지 않는 함수 func()에서 aaa 변수를 참조한다. 하지
만 aaa는 실제로 존재하지 않는 변수다. 그러면 컴파일 과정에서 다음과 같은 심볼 오
류가 발생한다.

[그림 6-6] 컴파일 과정 오류 메시지

6장_ gas assembler

383

===== PAGE 385 =====
aaa 심볼을 찾을 수 없으니 당연히 링킹 과정에서 오류가 발생한다. 이렇게 해당 심볼
을 코드상에서 참조는 하지만 실제 코드가 호출되지 않아 심볼 오류를 무시해도 되는
명확한 경우에는 다음과 같이 컴파일하면 정상적으로 컴파일 가능하다.
$ gcc -o like like.c -War-defsym,aaa=0xl2345678
L* root@server：/work/book/utils_new/as
[rootSseruer as]# gcc -o like like.c -Wa,-defsym,aaa=0x12345678
[rootSseruer as]#
[root@seruer as]# is like
like
[rooteseruer as]# ./like
I like you?
[root@seruer as]# |

[그림 6-7] -defsym 옵션을 사용해 오류 메시지 제거

gcc 옵션 중에서 -Wa,[as옵션]… 옵션은 gcc가 as를 호출할 때 -Wa에 추가한 옵션
들을 as 옵션으로 추가해 as를 호출하라는 의미다. 그래서 as는 호출될 때 -defsym

aaa=0xl2345678 옵션이 추가되어 호출된다. 이렇게 하면 실제 aaa 심볼은 코드나 라
이브러리에 존재하지 않지만 as가 -defsym aaa=0xl2345678 옵션에 의해 직접 정의
하기 때문에 정상적으로 컴파일할 수 있다.
물론 이렇게 처리해야 되는 경우는 매우 드물게 발생한다. 간혹 오래된 오픈 소스 프로
젝트를 컴파일할 때 컴파일러 버전이 달라 심볼을 찾지 못해 컴파일이 안 되지만 그 심
볼이 사용될 이유가 없다는 것을 잘 아는 상황이라면 근본적인 해결책은 아니더라도
이렇게 해서 컴파일할 수 있다.
@ 니 dir 옵션（아키텍처 공통）

어셈블리 파일 내 .include ”파일명" 지시어가 사용되었으면 해당 파일명을 찾는 디
렉토리를 추가하는 옵션이다. .include ''파일명"은 어셈블러 지시자로, 어셈블러에
게 “파일명”에 해당하는 파일의 내용을 현재 위치에 삽입하라는 의미다. 이는 C 소스
에서 #icnlude ’’파일명" 문장과 동일하고, as 의 -I 옵션은 gcc 의 -I 옵션과 동일하게

include 파일을 찾을 디 렉토리를 추가하는 옵션이다.

H -R 옵션（아키텍처 공통）
.data 섹션을 .text 섹션에 포함시킨다. 이렇게 하면 .data 섹션의 사이즈가 0이 되어 버
리고 모든 .data 섹션의 내용이 .text 섹션에 들어간다. 이렇게 해서 생길 수 있는 이점
은 인스트럭션과 데이터가 하나의 섹션 내에 있으니 더 짧은 오프셋으로 참조 가능하
다는 것이다. 아키텍처에 따라서는 이런 일이 성능 향상에 도움을 주기도 한다.
384 3부- 컴파일과 링킹

===== PAGE 386 =====
同 —32 | —-64(x86)

워드 사이즈를 32비트로 할 것인지 64비트로 할 것인지 결정한다. 이 옵션은 x86 아키
텍처에서만 유효하다. --64 옵션은 x86_64 플랫폼이나 -enable-64-bit-bfd 옵션으
로 컴파일한 32비트 as에서만 사용 가능하다.
자신이 x86_64 플랫폼에서 32 비트 어셈블리 파일을 어셈블한다면 一32 옵션을 지정
해야 한다.
同 一march=CPU[+EXTENSION...](x86)

어셈블리 파일을 컴파일하는 데 있어 인자로 준 CPU 타입에서 지원하는 인스트럭션만
사용되었는지 체크하고, 지원하지 않는 인스트럭션이 사용되었으면 오류를 출력한다.

CPU 타입에 사용할 수 있는 타입 문자열들은 다음과 같다.
i8086,
il86,
i286z
i386,
i486,
i586,
i686,
pentium,
pentiumpro,
pentiumii,
pentiumiii,
pentium4,
prescott,
nocona,
core,
core2,
k6, k6_2, athlon, opteron, k8, amdfamlO, generic32, generic64.

이 타입들은 최신 버전 as 에서 지원 CPU 타입이고, as 버전에 따라 지원하는 타입이
다를 수 있으니 기억해 두기 바란다.
뒤에 오는 +EXTENSION은 해당 CPU의 확장 인스트럭션 셋을 지정한다. 예를 들면

i686 아키텍처 기본 인스트럭션에 vmx 확장 인스트럭션과 sse4 확장 인스트럭션을 체
크하고자 한다면 -march=i686+vmx+sse4 옵션을 사용한다. 이때 사용 가능한 확장
인스트럭션 타입 문자열은 다음과 같다.
mmx,
ssez
sse2,
sse3,
ssse3,
sse4.1,
sse4.2,
sse4,
avx,
xsave,
aes,
pclmul,
fmaz
movbe,
ept,
3dnow,
3dnowa,
svme, abm, padlock

vmx,
sse4a,

smx,
sse5,

이 옵션은 자신이 작성한 어셈블리 언어가 해당하는 아키텍처에서 지원하는지 확인하
는 데 유용하게 사용할 수 있다.

Q -mtune=CPU(x86)
이 옵션은 -march 옵션과 연계해 최적화할 프로세서 타입을 지정한다. gcc 의 -mtune
옵션과 거의 동일하다. 사용 가능한 CPU 타입은 x86의 -march 옵션에서 지정 가능한

CPU 타입 문자열들이다.

6장_ gas assembler 385

===== PAGE 387 =====
—mcpu=PROCESSOR[+EXTENSION...](ARM)
인자로 오는 PROCESSOR 타입과 +EXTENSION 타입에서 지원하는 인스트럭션으로
어셈블리 코드가 작성됐는지 체크한다. 지원되지 않는 인스트럭션이 사용되었다면 오
류를 출력 한다.
최신 버전 as에서 지원하는 프로세서 타입 문자열은 다음과 같다.
arml,
arm2,
arm250,
arm3,
arm6,
arm60z
arm600,
arm610,
arm620,
arm7,
arm7nlz
arm7d,
arm7dmz
arm7di,
arm7dmi,
arm70,
arm7
0
0,
arm700i,
arm710,
arm710t,
arm720,
arm720t,
arm740t,
arm710c,
arm7100,
arm7500,
arm7500fe,
arm7t,
arm7tdlni,
arm7tdmi-s,
arm8,
arm810,
strongarm,
strongarml,
strongarmllO,
strongarmllOO,
strongarmlllO,
arm9,
arm920,
arm920t,
arm922t,
arm940t,
arm9tdmi,
fa526 (Faraday FA52 6 processor) , fa626 (Faraday FA62 6 processor) ,
arm9ez
arm926e,
arm926ej—s,
arm94
6e-rO,
arm946e,
arm946e-s,
arm966e-rO,
arm966e,
arm966e-s,
arm968e-s,
armlOt,
armlOtdmi,
armlOe,
arml020,
arml020t,
arml020e,
armlO22e,
armlO26ej—s,
fa626te
(Faraday
FA626TE
processor),
fa726te
(Faraday
FA726TE
processor)
,
armll36j—s,
armll36jf-s,
armll56t2
—s,
armll56t2f—s,
armll76jz-s,
armll76jzf-s,
mpcore,
mpcorenovfp,
cortex-a8,
cortex
—a9,
cortex
—r4,
cortex—m3,
ep9312
(ARM92
0
with
Cirrus
Maverick
coprocessor),
180200
(Intel
XScale
processor)
iwmmxt
(Intel
(r)
XScale
processor
with
Wireless
MMX(tm)
technology
coprocessor), xscale

그리고 지원하는 EXTENSION 타입 문자열은 다음과 같다.
+maverick, +iwmmxt, +xscale

®-march=ARCHITECTURE[+EXTENSION...](ARM)
x86 -march 옵션과 동일하게 어셈블리 코드에서 ARCHITECTURE와 EXTENSION에
서 지원하는 인스트럭션으로만 작성됐는지 체크하는 옵션이다. 지원하지 않는 인스트
럭션이 포함되었다면 오류를 출력한다. 사용 가능한 아키텍처 타입은 다음과 같다.
armvl,
armv2,
armv2a,
armv2s,
armv3,
armv3m,
armv4,
armv4t,
armv4txm,
armv5,
armv5t,
armv5txm,
armv5tez
armv6,
armv6j,
armv6k,
armv6z,
armv6zk,
armv7z
armv7-a,
armv7—m, iwmmxt, xsca丄e

armv4xm,
armv5texp,
armv7-r,

I® —mfpu=［부동소수점 포맷］(ARM)
이 옵션은 인자로 오는 ［부동소수점 포맷］이 어셈블리 파일 내에 제대로 사용되었는지
체크하는 옵션이다. 부동소수점 연산이 지원하지 않는 타입으로 어셈블리 코드가 작성

386

3부— 컴파일과 링킹

===== PAGE 388 =====
됐다면 오류를 출력할 것이다. 이때 사용 가능한 [부동소수점 포맷] 문자열은 다음과
같다.
softfpa,
fpe,
fpe2z
fpe3,
fpa,
fpalO,
fpall,
arm7500fe,
softvfp+vfp,
vfpA
vfplO,
vfplO-r0,
vfp9,
vfpxd,
vfpv2
vfpv3-dl6 arml020t, arml020e, armll36jf-sz maverick, neon

softvfp,
vfpv3

(D —mthumb과 -mthumb-interwork(ARM)
-mthumb 옵션은 어셈블리 파일을 16비트 thumb 인스트럭션으로 어셈블한다.
-mthumb -interwork 옵션은 thumb 모드와 ARM 모드 간의 상호 호출을 지원 가능하
게 어셈블한다.

E -mapcs [26|32](ARM)
-mapcs는 ARM 프로시저 호출 표준(Arm Procedure Calling Standard)의 버전을 지
정하는 옵션으로, 지정 가능한 버전에는 26과 32가 있다. ARM 프로시저 호출 표준이란
어떤 함수를 호출할 때 어떤 레지스터를 인자를 넘기는 데 사용하고, 어떤 레지스터를
함수 내 변수를 사용할 것인지 (caller/callee saved register 선택), 호출 순서는 어떻
게 할 것인지 등을 정의한 규약이다.
이 옵션을 사용해 ARM 프로시저 호출 표준을 선택할 수 있다. 이는 프로그램 수행 성
능에 영향을 줄 수 있다.

E@ —mfloat—abi 三 abi 와 一meabi三ver(ARM)
-mfloat-abi 옵션은 인자로 오는 abi를 부동소수점 ABI (Application Binary
Interface)로 사용한다. ABI가 궁금한 독자는 이 전에 “gcc” 장에서 설명 한 ABI 부분을
찾아 보기 바란다. abi로 사용 가능한 타입에는 다음과 같은 것들이 있다.
soft, softfp, hard

-meabi 옵션은 생성할 오브젝트 파일의 EABI 버전을 결정한다. 사용 가능한 EABI 버
전 문자열은 다음과 같다.
gnu, 4, 5

ABI 또는 EABI에 의해 함수 호출 방식 및 아키 텍처에서 지원하지 않는 연산 등을 위한
함수 호출명 등이 많이 달라질 수 있다.

6장_ gas assembler

===== PAGE 389 =====
0힌 —EB와 -EL(ARM)
인스트럭션을 빅 엔디안(-EB)으로 인코딩할지 리틀 엔디안(-EL)으로 인코딩할지 결
정한다.
이상 as 공통, x86, ARM 아키텍처에서 자주 사용하는 옵션 설명이 끝났다. 이런 옵션
들을 직접 사용할 일은 거의 없으리라 본다. 이전에도 말했듯이 as를 직접 호출할 일은
상당히 드물기 때문이다. as를 사용해 어셈블하기보다는 gcc를 사용해 어셈블하는 편
이 더 낫다. 때문에 굳이 위 옵션들을 기억할 필요는 없다.

a

어셈블리 파일의 작성

지금부터 간단한 어셈블리 파일의 작성법을 알아본다. 어셈블리 파일을 작성하려 한다
면 당연히 어셈블리 언어를 잘 알아야 한다. 어셈블리 언어를 필자가 알려 줄 수 있으
면 좋겠지만 어셈블리 언어를 알려면 해당 아키텍처의 특징, 인스트럭션, 문법 같은 것
들을 알아야 한다. 그것은 이 책의 범위를 벋어난다.
때문에 필자는 독자가 이미 어셈블리 언어를 알고 있다는 전제하에 설명하고, 되도록
간단히 맛보기 정도로만 설명하겠다.
여기서 필자가 독자에게 꼭하고 싶은 이야기는 다음과 같다. 어셈블리가 어렵다고 생각
하는 독자가 있을 것이다. 필자가 단언하건데 어셈블리는 c보다 3배는 쉽다. 실제로 필
자의 경험을 이야기하는 것이다. 그리고 이는 필자뿐만 아니라 필자 주위에 있는 어셈블
리 전문가들, 필자에게 어셈블리를 배웠던 사람들이 하나같이 공통적으로 하는 말이다.
어셈블리가 어렵다고 느끼는 것은 어셈블리가 진짜 어려워서가 아니라 자신의 마음이
어렵다고 느껴서 어려운 것이다. 단지 접해 보지 않아서 그렇다. 실제로 해 보면 어셈블
리는 정말 아무것도 아님을 알 수 있을 것이다.

388 3부- 컴파일과 링킹

===== PAGE 390 =====
I assembly 기본 사용법
먼저 이전에 사용하던 like.S 파일로 하나씩 알아보자.
like.S 파일 내용

. text
.globl main
main:
subl
movl
call
addl
ret

$4, %esp
$likestr, (%esp)
puts
$4, %esp

.string

"I like you!

likestr:

변수를 어떻게 사용하는지 알아보자. 위 소스 파일을 다음과 같이 고치기 바란다.
〔예제 6-4)

. text
.globl main
main:
pushl
aaa
aaa 값을 스택에 push함 大/
pushl
$likestr
丄ikestr 주소를 스택에 push함 */
call
printf
printf 함수 호출 */
addl $8, %esp /* 스택에 8을 더해 스택 주소를 이전 상태로복귀 */
ret
likestr: .string "I like you! aaa = %d\n"
aaa: .long 1234

그다지 크게 달라진 것은 없다. 단지 aaa：라는 레이블을 만들고 거기에 .long이라는 어
셈블러 지시자를 사용해 4바이트짜리 공간을 할당했다. 그리고 초기 값을 1234으로 설
정했다.
그리고 likestr의 원래 문자열에 “aaa = %d”라는 문자열을 추가하고 puts 함수 호출을

printf 함수 호출로 바꾸었다.
위 어셈블리 코드는 다음 명령으로 컴파일할 수 있다.
$ gcc -o like like.S

6장_ gas assembler

389

===== PAGE 391 =====
그리고 수행하면 다음과 같이 aaa 공간의 내용이 출력됨을 확인할 수 있을 것이다. 어
떻게 변수를 정의하고 참조하는지 대략 감이 잡힐 것이다. 실제로 C 컴파일러에서 컴
파일된 변수들이 aaa와 같은 형식으로 공간이 잡히고 참조되어 사용된다.

[그림 6-8] like 파일 실행 결과

자, 이제는 다른 파일에 있는 함수를 어떻게 호출하는지 한번 알아보자. 먼저 다음과
같은 func.c 파일을 작성한다.
〔예제 6-5〕 func.c 파일 내용

#include <stdio.h>
void func () {
printf("This is func () !!\n");
}

그리고 Hke.S 파일은 다음과 같이 고친다.
-i like.S 파일의 내용

. text
.extern func
.globl main
main:
pushl
push 丄
call
addl
call
ret

aaa
$likestr
printf
$8Z %esp
func

likestr:
.string "I 丄ike you! aaa = %d\n"
aaa:
.long 1234

390 3부- 컴파일과링킹

===== PAGE 392 =====
역시나 그다지 변화는 없다. .extern 지시자가 추가되었고 func 함수를 호출하는 인스
트럭션이 추가되었다. func 심볼은 like.S 파일에는 없기 때문에 .extern 지시자를 사용
해 외부에서 참조하는 심볼이라고 어셈블러에게 알려준다. 위 파일들은 다음 명령으로
컴파일할수있다.
$ gcc -o .like like.S func.c

그러 면 다음과 같이 func() 함수가 정상적으로 잘 호출되는 것을 확인할 수 있다.

[그림 6-9] like 파일 실행 모습

I C 소스에서 컴파일된 어셈블리 파일 분석
이제 좀 더 큰 어셈블리 파일에 대해 알아보자. 그리고 gcc가 C 소스를 어떻게 컴파일
하는지도 알아보자. 먼저 다음과 같은 main.c 파일을 작성 한다.
〔예제 6-7〕 main.c 파일 내용

tinclude <stdio.h>
int aaa = 1111;
int bbb = 2222;
int ccc;
int main() {
ccc = aaa + bbb;
printf("ccc = %d\n", ccc);
return 0;

[예제 6-7] 파일을 gcc -o main main.c -save-temp 옵션으로 컴파일한다. 그러면
다음과 같은 main.s 파일이 생성된다.

6장_ gas assembler

391

===== PAGE 393 =====
BKIEIKg：il| main.s 파일 내용

.file "main. c"
.globl aaa
. data
.align 4
.type aaa, @object
.size aaa, 4
aaa:
.long 1111
.globl bbb
.align 4
.type bbb, @object
.size bbb, 4
bbb:
.long 2222
.section

.rodata

.LCO:
.string "ccc = %d\n"
. text
.globl main
.type main, ^function
main:
leal
4 (%esp), %ecx
andl
$-16, %esp
pushl -4(%ecx)
pushl %ebp
movl
%esp, %ebp
pushl %ecx
subl
$20, %esp
movl
aaa, %edx
movl
bbb, 응eax
leal
(%edx,%eax), %eax
movl
응eax, ccc
movl
ccc, %eax
movl
%eax, 4(%esp)
movl
$.LCO, (%esp)
call
printf
movl
$0, %eax
addl
$20, %esp
popl
%ecx
popl
%ebp
leal
-4(%ecx), %esp
ret
.size main, .-main
.comm ccc,4, 4
.ident ”GCC: (GNU) 4.1.2 20071124 (Red Hat 4.1.2-42)"
. section
. note. GNU-stack, ’’", @progbits

392 3부— 컴파일과 링킹

===== PAGE 394 =====
다른 것은 다 볼 필요 없고 aaa와 bbb, ccc 변수가 어떻게 잡혔는지 먼저 확인해 보자.

aaa 부분을 보면 다음과 같다.
...상략

.globl aaa
. data
.align
. type
• size

/* aaa 레이블을 외부로 익스포트함 */
/* . data 섹션이라는 의미 */
4

/* 현재 위치 카운트를 2”4만큼 정렬 즉, 16바이트만큼 정렬 *
/* aaa의 타입은 오브젝트 */

aaa, @object
aaa, 4

aaa:
. long

1111

/* aaa의 사이즈는 4바이트 */
/* 여기가 진짜 aaa 레이블임 */
/* 4바이트 공간을 잡고 초기 값을 1111로 함 */

...하략

먼저 aaa 가 전역변수이므로 다른 파일에서 심볼을 찾을 수 있게 aaa 심볼을 .globl 지
시자를 통해 외부로 익스포트한다. 그러면 ELF 바이너리 포맷의 심볼 테이블에 aaa가
들어가서 링킹 시 aaa의 존재를 링커가 알 수 있다.
그리고 .data 지시자를 통해 이후 어셈블되는 것들은 .data 섹션에 공간을 잡게 지시한
다. 뒤에는 aaa： 레이블이 오고 .long 1111에 의해 실질적인 aaa의 4바이트 공간이 잡
힘으로써 이 때 잡히는 aaa의 공간이 .data 지시자에 의 해 .data 섹션에 위 치 한다.

.align 4 는 정렬을 위한 지시자다. 2 의 4 승 단위로 현재 주소를 정렬하라는 의미로,
16바이트 단위로 정렬된다. type과 size는 디버깅 정보인 타입과 사이즈를 심볼 테이블
에 추가하라는 의미다. 그래서 이 렇게 컴파일 과정에서 생성된 main.o 파일을 readelf

-s main.o 명령으로 보면 aaa의 타입이 오브젝트로, 사이즈가 4로 설정되어 있는 것을
확인할 수 있다.
여1 root@server：/work/book/utils_new/as2
[root@seruer as2]tt readelF -s main.o
Symbol table '.symtab' contains 13 entries:
Num
Ualue
Size Type
Bind
0
08008000
0 NOTVPE
LOCAL
1
00000000
0 FILE
LOCAL
2
08000000
0 SECTION LOCAL
00808000
3
0 SECTION LOCAL
4
00800000
0 SECTION LOCAL
5
00000000
SECTION LOCAL
6
00080000
SECTION LOCAL
00000000
7
SECTI（써 LOCAL
8
00000000
OBJECT | GLOBAL
9
00000004
GLOBAL
OBJECT
10
0O0OW00
71 FUNC
GLOBAL
GLOBAL
11
00000004
4 OBJECT
12
00000800
0 NOTVPE
GLOBAL
[root@server as2]tt |

Uis
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT
DEFAULT

Hdx
UHD
ABS
1
3
4
5
7
6
3
3
1

Name
main.c

aaa
bbb
main
ccc
UND printf

con

[그림 6-10] readelf -s main.o 명령 결과

6장_ gas assembler 393

===== PAGE 395 =====
실질적으로 aaa 레이블을 정의하는 것은 aaa： 문장이다. 레이블명 + 콜론(：)을 붙이면
레이블을 정의할 수 있다. 그러면 해당 레이블을 어셈블리 코드 내에서 참조하는 것이
가능하다. 다음은 실제 어셈블리 코드에서 참조하는 부분이다.
... 상략

movl
movl
leal
movl

aaa, %edx
bbb, %eax
(응edx, %eax) , %eax /*
%eax, ccc

/*
/*
/*

aaa의 값을 edx 레지스터에 넣음 */
bbb의 값을 eax 레지스터에 넣음 */
edx 값과 eax 값을 더해 eax에 넣음 */
eax 값을 ccc에 넣음 */

.••하략

aaa： 레이블 다음으로 “.long 1111” 문장이 온다. Jong은 이전에도 말했듯이 현재 위
치에 4바이트 공간을 잡는다는 의미다. 그리고 1111에 의해 초기 값으로 1111을 설정
한다. 또한 이전에 나온 .data 지시자에 의해 aaa 레이블의 4바이트 공간은 .data 섹션
에 할당된다.
위 예는 컴파일러에서 나온 결과라 다소 복잡한데, aaa 변수를 사용하기 위해 반드시
필요한 문장은 다음과 같다.
/* 여기가 진짜 aaa 레이블임 */
/* 4바이트 공간을 잡고 초기 값을 1111로 함 */

aaa:
.long 1111

나머지는 디버깅을 위한 정보(.type, .size)를 주거나 성능 향상을 위해 정렬(.align)한
것이다. ARM 아키텍처와 같은 아키텍처는 4바이트 크기의 변수에 4바이트 단위의 주
소 정렬이 반드시 필요하지만 x86은 정렬해 주지 않아도 관계없다. 그리고 “.globl aaa”
는 aaa를 굳이 외부로 익스포트할 이유가 없다면 제거해도 된다.
위 예에서는 .data 지시자를 제거했음으로 aaa의 공간은 .text 섹션에 잡힌다. aaa의 공
간이 .text 섹션에 공간이 잡혀도 수행하는 데는 아무런 문제가 없다.
이제 bbb를 한번 보자. bbb도 aaa와 동일하다.
• • • 삿략
0—1
.globl bbb
.align 4
.type
.size
bbb:
.long 2222
... 하략

394

W_ 컴파일과 링킹

bbb, @object
bbb, 4

===== PAGE 396 =====
bbb에는 .data 지시자가 보이지 않는데, aaa에서 이미 .data 지시자가 사용되었기 때문
에 bbb도 .data 지시자가 유효하다. 때문에 bbb도 당연히 .data 섹션에 잡힌다.
그리고 다음 문장이 온다.
...상략

.section

.rodata

.LCO:
.string ”ccc = %d\n"
. text
.globl main
.type

main,

@function

leal
andl

4 (%esp), %ecx
$-16, 응esp

main:

... 하략

먼저 “.section

.rodata” 지시자에 의해 이제부터 .rodata 섹션에 어셈블됨을 의미

한다. .LC0： 라는 레이블이 오는데, 이렇게 .LC［숫자］:와 같은 형식의 레이블을 지역 레
이블이라 부르고, 컴파일러가 코드를 생성하면서 임의로 만드는 레이블이다. 이런 지역
레이블은 특별한 지시자 또는 as 옵션을 주지 않는 한 외부로 익스포트되지 않는다.

“.string "ccc = %d\n"” 지시자에 의해 현재 위치에 “ccc = %d\n”이라는 문자열이 위
치한다. 물론 이 문자열은 이전 “.section .rodata” 지시자에 의해 읽기 전용 섹션인

.rodata 섹션이 위치한다.
그리고 .text 지시자에 의해 이후부터 .text 섹션임을 의미한다. .globl main 지시자에
의해 main 심볼이 외부로 익스포트된다. 그리고 “.type main, ©function” 지시자에
의해 main.o 파일의 심볼 테이블에 main의 타입이 함수라는 정보가 들어간다. 이후

main 함수의 인스트럭션이 어셈블되는데, 모두 .text 지시자에 의해 .text 섹션에 어셈
블된다.
그럼 CCC는 도대체 어디에 잡히는 것일까? CCC는 초기화되지 않은 전역 데이터이니 당
연히 .bss 섹션에 잡혀야 한다. 그런데 ccc가 있는 곳을 한번 보자. “.comm ccc,4,4”
라는 지시자가 있다. 이 문장의 의미는 .bss 섹션 내 공통 영역을 잡고 여기에 ccc를

4바이트만큼 할당하라는 의미다. 때문에 e으는 .bss 섹션에 들어간다.
자, 여기까지 설명하면서 필자가 알려주고 싶은 것이 있다. 이전에 우리는 컴파일 과정
혹은 링킹 과정에서 인스트럭션은 .text 섹션에 잡히고, 초기화된 전역 데이터는 .data

6장_ gas assembler

===== PAGE 397 =====
섹션에, 그리고 초기화되지 않은 전역 데이터는 .bss 섹션에 잡힌다고 했다. 그런데 도
대체 누가 각각의 데이터나 인스트럭션을 해당하는 섹션에 잡아주는가?
바로 ccl 컴파일러가 어셈블리 파일을 생성하면서 .text, .data, .rodata, .comm 같은
지시자를 사용해 각각의 인스트럭션과 변수들을 해당 섹션들에 잡아준다. 어셈블러는
이렇게 컴파일러가 지시한 대로 각 데이터 또는 인스트럭션을 원하는 섹션에 위치시키
는일만수행한다.
나머지 인스트럭션 부분은 문법적인 측면과 아키텍처적인 측면이 강하므로 해석은 독
자에게 맞기겠다. 시간이 되거나 어셈블리를 배워 보고픈 독자라면 한번 해석해 보기
바란다. 해석할 때는 3가지를 알 필요가 있는데, 먼저 해당 아키텍처 구조를 알아야 하
고, 해당 아키텍처에는 어떤 인스트럭션이 있는지 알아야 하며, 마지막으로 gas에서 사
용하는 어 셈블리 문법 (AT&T)을 알아야 한다.
각각의 내용들이 인터넷에 흔하게 널려 있으니 이 3가지 내용을 담고 있는 문서를 찾아
한번 해석해 보기 바란다.

I 전처리기 사용
어셈블리 파일을 작성할 때는 확장자를 *.S로 작성할 수도 있고 *.s로 작성할 수도 있
다. 확장자를 대문자 s로 하느냐 소문자 S로 하느냐에 따라 약간의 차이가 있다.
먼저 확장자가 대문자 S인 어셈블리 파일을 gcc로 컴파일하면 ccl -E C 전처리기가 호
출된다. 그래서 어셈블리 파일 내에 #include ”hardware.h"와 같은 C 전처리기 문장을
사용할 수 있다. 마찬가지로 #ifdef ~ #endif와 같은 전처 리기 문장도 사용 가능하다.
반면 확장자가 소문자 s 인 파일은 전처리 과정 없이 바로 as 가 불리어진다. 그래서

C 전처 리 문장은 사용 불가능하다.
이 때문에 많은 사람이 확장자를 소문자 대신 대문자로 주로 사용한다. C 전처리기를
사용하면 어셈블리 프로그래밍에 효율성이 증가하고, 헤더 파일을 C 소스와 어셈블리
소스가 동시에 사용할 수 있어 하나의 헤더 파일로 전처리기에 의한 설정이 가능하기
때문이다.

396 3부—컴파일과링킹

===== PAGE 398 =====
I gas assembler 필수 지시자
이전에 사용했던 .long, .string과 같이 점(.)으로 시작하는 것들이 어셈블러 지시자들
이다. 즉, 어셈블러에게 어떤 지시를 내리는 문장이란 의미다. as는 수많은 어셈블러 지
시자를 제공한다. 이번 과정에서는 그 중에 자주 사용하는 것 위주로만 설명한다.

O 정렬 지시자
► .align abs-expr, abs-expr
.align 지시자는 현재 주소를 처음 오는 2 A abs-expr 단위로 정렬한다. 뒤에 오는 absexpr 는 정렬할 때 빈 영역을 채우는 값으로 abs-expr 값을 사용하라는 의미다. 뒤에
abs-expr은 생략 가능하고 .align 지시자는 통상 다음과 같이 사용한다.

.align
main:

4
pushl
call printf

$likestr

위와 같이 하면 main 함수는 2의 4승 주소 단위로 정 렬된 주소에 위 치 한다.
정렬 지시자는 x86과 같은 아키텍처에서 최적화를 위해 의미가 있지만 ARM 같은 아키
텍처에서는 반드시 사용할 필요가 있다.

ARM 아키텍처에서는 4바이트 단위의 데이터나 인스트럭션에 접근하려면 반드시 4바
이트 단위로 정렬된 주소로 접근해야 한다. 즉, 4바이트짜리 변수의 시작 주소는 항상

4바이트 단위로 정렬되어 있어야 한다. 그렇지 않으면 해당 변수 접근 시 혹은 해당 인
스트럭션 접근 시 data abort이나 prefetch abort가 발생할 것이다.
그러면 어떨 때 정렬이 흐트러지는가? ARM은 인스트럭션이 4바이트이므로 웬만하면
흐트러지지 않는다. 하지만 인스트럭션 중간에 문자열이 위치하면 정렬이 어긋날 수 있
다. 때문에 ARM 어셈블리 파일을 작성할 때 문자열이 중간 중간 포함된다면 함수와 변
수 사이 사이에 .align 지시자를 적절히 넣어주는 것이 중요하다.

6장_ gas assembler

397

===== PAGE 399 =====
@ 할당 지시자

► .byte expressions
1

바이트 공간을 할당하고 expressions 값으로 채운다.
예） .byte OxFF

►

.word expressions 또는 .short expressions 또는 .hword expressions

2바이트 공간을 할당하고 expressions 값으로 채운다.
예） .word 1234

►

Jong expressions 또는 Jnt expressions

4바이트 공간을 할당하고 expressions 값으로 채운다.
예） Jong 0x12345678

►

.ascii "string"

현재 위치에 string 문자열을 할당한다. 하지만 끝에 0을 채우지는 않는다.
예） .ascii ”1 like you!\n"

►

.asciz "string"과 .string "string"

현재 위치에 string 문자열을 할당한다. 끝에 0을 채운다.
예） .asciz ”1 like you!\n”

►

.fill repeat, size, value

.fill 지시자는 repeat만큼 반복하면서 size 단위로 value 값을 채운다. size와 value는
생략 가능하다. .fill 지시자 사용 예를 들면 다음과 같다.
.long OxCCCCCCCC
.fill 2, 4, 0x12345678
.long 0xAAAAAAAA
.long 0xAAAAAAAA
.long 0xAAAAAAAA

위 지시자는 4바이트 단위로 2번 반복하면서 0x12345678을 채운다. 그래서 다음과 같
은 형태로 채워진다.

398 3부_ 컴파일과 링킹

===== PAGE 400 =====
艾 root@server：/work/book/utils_new/as
Contents of section. ..text:
0Q00 cccccccc
aaaaaaaa
0010 aaaaaaaa
O0OOOOe8
0020 00886841
OO8d7600
0030 6c6c6c6c
696b6528
0040 2249206c
640300
0050 203d2025
[root@seruer as]# |

aaaaaaaa
FcFFfffF
d204OOO8
796F7521

|aaaaaaaa
FF353880
83c408c3
00222222
20616161

［그림 6-11］ .fill 지시자 사용 예

위 그림에서 4(size)바이트 단위로 2(repeat)번 Ox12345678(value)°1 채워진 것을
확인할 수 있다.
.long OxCCCCCCCC
.fill 3, 8Z 0x12345678
.long OxAAAAAAAA
.long 0xAAAAAAAA
.long 0xAAAAAAAA

위와 같이 했다면 8바이트 단위로 3번 0x12345678이 채워진다.
逐 root@server：/work/book/utils_new7as
[rootBseruer as]# objdump -s like.o
like.o:

File format elf32-i386

Contents of section .text:
8B00 cccccccc[7856341280000000!78563412
0O10I00080000178563412 880600801aaaaaaaa
aaaaaaaa
aaaaaaaa
0020 aaaaaaaa
FcFFffff
8W00e8
0030 00806851
d204O0O0
808d7680
0840 6c6c6c6c
796F7521
696b6528
W50 2249206c
648a00
0060 203(12025
[root@seruer as]# |

FF354800
83c408c3
00222222
20616161

［그림 6-12］ .fill 지시자 사용 예

［그림 6-12］ 에서 볼 수 있듯이 0x12345678이 8바이트 단위로 3번 채워진 것을 확인할
수 있다. 큰 공간을 할당하거나 배열을 할당하고자 할 때 자주 사용한다.

► .space size, fill
size 바이트만큼 fill 값으로 채운다. fill이 생략되면 0으로 채워진다. 큰 공간을 할당하
려 할 때 자주 사용한다.

@ 심볼 관련 지시자

► .global symbol 또는 .globl symbol
링커가 해당 심볼을 알 수 있게 심볼을 외부로 익스포트한다. 이렇게 하면 symbol이 해당

ELF 오브젝트의 심볼 테이블에 익스포트되어 링커가 해당 심볼의 존재를 확인할 수 있다.

6장_ gas assembler 399

===== PAGE 401 =====
► .extern symbol
symbol을 외부 심볼로 선언한다. 이렇게 하면 외부 심볼을 어셈블리 파일 내에서 참조
할수있다.

►

.equ symbol, expression 또는 .set symbol, expression

심볼의 값을 expression 으로 설정한다. 이렇게 설정된 심볼은 어셈블리 코드 내에서
사용될 수 있다.

B 섹션 관련 지시자
►

.text

.text 섹션에 포함됨을 나타낸다. 정확하게 이야기하면 0번 보조 .text 섹션(subsection)
에 포함됨을 의미하고 우리가 일반적으로 생각하는 .text 섹션을 의미한다.

►

.text subsection

subsection 번호에 해당하는 보조 .text 섹션에 포함됨을 의미한다. subsection은 0 에
서 8192까지인 숫자이다. 이 지시자는 .text 섹션 내부를 그룹으로 나눠 다음에 오는 것
들을 특정 그룹에 할당하고자 할 때 사용한다. 하지만 거의 사용할 필요가 없으니 이해
가 안 되면 그냥 넘어가도 된다.
예) .text 1

►

.data

.data 섹션에 포함됨을 나타낸다. 정확하게 이야기하면 0번 보조 .data 섹션(subsection)
에 포함됨을 의미하고, 우리가 일반적으로 생각하는 .data 섹션을 의미한다.

►

.data subsection

subsection 번호에 해당하는 보조 .data 섹션에 포함됨을 의미한다. subsection은 0 에
서 8192 까지인 숫자다. 이 지시자 역시 .data 섹션 내부를 그룹으로 나누어 다음에 오
는 것들을 특정 그룹에 할당하고자 할 때 사용한다. 하지 만 거의 사용할 필요가 없으니
이해가 안 되면 그냥 넘어가도 된다.
예) .data 1

►

comm symbol, length

.bss 섹션에 length 사이즈를 가지면서 symbc)l명을 가지는 공통 영역을 설정한다. 즉,
.bss 섹션에 length 사이즈의 symbol을 설정한 것과 같다.

400 s부—컴파일과링킹

===== PAGE 402 =====
►

.section name, subsection

name 섹션에 다음에 올 어셈블리 코드를 어셈블해 넣는다. subsection 번호가 생략되
면 name 보조 섹션 0이 사용되고, 아니면 subsection 번호의 name 보조 섹션에 어셈
블된다.
쉽게 이야기하면 다음에 오는 것들을 name이란 섹션에 할당하라는 의미다.
예） .section mysection

同 기타 중요한 지시자

►

.if expression 〜 .else 〜 .endif

expression 이 참이면 참인 문장을 어셈블하고, 거짓이면 거짓인 문장을 어셈블한다.
예를 들면 다음과 같이 사용한다.
.endif 사용 예

. text
.globl main
main:
.if 3 > 4
pushl

aaa

pushl

bbb

pushl
call
add 丄
ret

$likestr
printf
$8, %esp

. string

"1111”

. else
.endif

.align 4
aaa: .long 1234
bbb: .long 5678
likestr:
.string "I like you! aaa = %d\n"

C와 마찬가지로 .else 지시자는 생략할 수 있다. 그리고 .if 지시자 외에 다음과 같은 지
시자들도 사용할 수 있다.

6장_ gas assembler 401

===== PAGE 403 =====
►

Jfdef symbol 〜 .else 〜 .endif

심볼이 정의되었으면 참인 문장을 어셈블하고, 정의되지 않았으면 거짓인 문장을 어셈
블한다. .else 지시자는 생략할 수 있다.

►

.ifndef symbol 〜 .else 〜 .endif 또는 .ifnotdef symbol 〜 .else 〜 .endif

심볼이 정의되지 않았으면 참의 문장을 어셈블하고, 정의되었으면 거짓인 문장을 어셈
블한다. .else 지시자는 생략할 수 있다.

►

.include "file"

현 위치에 해당 file을 include한다.

► .macro name, arg,... 〜 endm
매크로를 지정한다. 사용법은 다음과 같다.
〔예제 6-10)

my_uart_init:
.macro init_uart SBA, gp2
/* Disable UART and disable
mov \gp2, #0x0
str \gp2, [\SBA, #0x0c]
str \gp2, [\SBA, #0x04]
/* Enab丄e UART */
Idr \gp2, [\SBA, #0x04]
orr \gp2, \gp2, #0x40
str \gp2, [\SBA, #0x04]
.endm
/* initialize UART */
Idr
rO, =0x40100000
init_uart rO, rl
Idr
rO, =0x40700000
init__uart rO, rl
mov

interrupts */
@ (DLAB OFF)
@ IER_DLH = 0x0

@ \gp2 = IER_DLH
@ Set the enable uart bit

@ FFUART:0x40100000
@ init FFUART
@ STUART:0x40700000
@ init STUART

pc, ir

［예제 6-1 이은 init_uart라는 매크로를 정의한 예다. .macro ~ .endm까지는 init_uart
라는 매크로의 선언 부분이다. 선언이기 때문에 정의되기 전까지는 실제 존재하는 것이
아니다.

402 3부— 컴파일과 링킹

===== PAGE 404 =====
어셈블리 소스 내에 “init_uart rO, rl”와 같이 매크로가 정의되면 정의된 위치에 선언한

init_uart 매크로의 내용이 채워진다. 이렇게 채워질 때 init_uart 매크로의 선언 부분에
SBA와 gp2 같은 것들이 매크로 인자인데, “init_uart rO, rl”와 같이 사용하면 매크로
선언에서 \SBA라 표기된 부분이 rO로 치환돼 채워지고, \gp2라 표기된 부분이 rl으로
치환돼 채워진다.

►

.org ［주소］, ［채울 값］

현재 위치를 인자로 오는 주소 위치로 설정한다. 이때 빈 영역에 대해서 채울 값으로
채운다. 채울 값은 생략 가능하고 주소는 현재 위치 카운트 값과 같거나 혹은 증가시키
는 주소에 한해서만 유효하다. 즉, 거꾸로 거슬러 주소를 설정할 수는 없다는 말이다.
위치 카운트에 대해서는 Id 링킹 과정 중 링커 스크립트를 설명할 때 했기 때문에 따로
설명하지 않는다.

C3 인라인 어셈블리의 사용
인라인 어셈블리는 c 소스 내에 어셈블리 코드를 사용하는 방법을 말한다. 이런 인라
인 어셈블리는 부트 로더를 작성하거나, OS 또는 디바이스 드라이버를 작성하지 않는
한 거의 사용되지 않는다. 그러나 애플리케이션을 작성하더라도 알아 두면 한 번은 정
말 요긴하게 쓰일 수 있는 것이 바로 인라인 어셈블리다.
그렇지만 아무리 요긴하게 쓰일지라도 되도록이면 인라인 어셈블리 사용을 자제하는
것이 좋다. c 소스 안에 어셈블리 코드가 들어가면 이미 그 소스는 해당 어셈블리를 사
용하는 CPU만으로 아키텍처가 제한되기 때문이다.
인라인 어셈블리는 c 로는 하기 힘든 작업에 사용된다. 예를 들면 현재 프로세스의 스
택 주소를 읽어 오는 것과 같이 레지스터를 직접 건드린다든지 특정 포트에 값을 쓴다
든지 하는 일에 이용된다.
어셈블리 언어는 모든 CPU의 근본적인 언어이고, CPU가 이해하는 인스트럭션을 단지
글자로 표현한 언어이기 때문에 매우 강력하다. 그래서 C로 하기 힘든 작업도 아주 쉽
게 해낼수 있다.

6장_ gas assembler 403

===== PAGE 405 =====
또 다른 경우로 최적화를 시킬 때 어셈블리를 사용하는 경우도 있는데, 그건 예전에 컴
파일러가 제대로 발전하지 않았을 때 이야기고 지금은 아무리 최적화하려고 노력을 해
도 gcc -02 나 -03 만큼 최적화하기는 힘들다. 물론 gcc -02 정도의 레벨에서 나온
어셈블리 코드를 보면 최적화할 만한 것도 많이 눈에 띄기는 하지만 어셈블리 코드로
작성하는 데 들이는 시간에 비 할 바는 아니 라고 생각한다.
필자는 어셈블리 언어는 반드시 배워두는 것이 좋다고 생각하는 사람 중 하나다. 어셈
블리를 이해하는 것은 단지 하나의 저급 언어를 이해한다는 의미가 아니라 시스템 아
키텍처를 이해하는 수단이 된다. 아키텍처를 이해한다는 것은 프로그래머에게 정말 큰
힘이 아닐 수 없다.
우리가 프루.-？■래밍을 하는 데 있어 적어도 1+1이 왜 2가 되는지는 알고 프로그래밍해
야 되지 않겠는가?
사실 어떻게 보면 C 언어도 어셈블리의 확장이라고 볼 수 있다. 과거에 고급 언어가 나
오지 않은 시절에는 어셈블리를 매크로 단위로 묶어 마치 고급 언어처럼 프로그래밍하
던 시절도 있었다.

C 언어의 모든 문법은 몇 줄의 어셈블리 언어와 동일하다. 물론 컴파일러는 C 언어를
중간 언어로 변환하고 최적화를 수행해 단순히 C 언어의 문법을 어셈블리 언어로 표현
한 것과 많이 달라진 모습의 어셈블리 코드를 만들어내지만, 최적화를 수행하지 않고
단순히 c 언어를 중간 언어로 바꾼 초기 형태는 바로 어셈블리로 거의 똑같이 표현할
수 있다.
그리고 어셈블리를 알면 디버깅을 할 때 도움이 된다. 어셈블리를 아는 상태에서 디버
거를 사용하는 것과 모르는 상태에서 디버거를 사용하는 것은 디버거가 제공하는 정
보를 이해하는 데 큰 차이를 보인다. 그래서 어셈블리는 반드시 알아 두는 것이 좋다고
필자는 생각한다.
서론이 길었다. 그럼 본격적으로 인라인 어셈블리 설명으로 들어가도록 하겠다. 먼저
예제를 보면서 설명한다.

404 3부_ 컴파일과 링킹

===== PAGE 406 =====
〔예제 6-11)

like.c 소스 코드

#include <stdio.h>
int main()
{
__asm_______ volatile ("nop") ;
return 0;
}

가장 간단한 형태의 인라인 어셈블리다. 인라인 어셈블리의 시작은 __asm__ 지정
어로부터 시작한다. 그리고 __volatile__ 키워드가 오는데, 변수 앞에 volatile# 지
정하면 해당 변수는 컴파일러가 최적화를 수행하지 않듯이 인라인 어셈블리에서의

__volatile__ 키워드는 인라인 어셈블리에 포함된 인스트럭션에 최적화를 수행하지
않겠다는 의미다. __asm__ 지정어는 인라인 어셈블리의 사용에 있어 필수 요소지만

__volatile__ 키워드는 사용하지 않아도 상관은 없다.
그 다음 여는 괄호(‘(’)가 나오고 "nop" 이라는 CPU 인스트럭션이 나왔다. nop는 CPU
인스트럭션 중 no operation이라고도 하며 아무 일도 하지 않는 인스트럭션이다. 마지
막으로 닫는 괄호(‘)’)가 나오고 세미콜론이 나왔다. 위 소스는 gcc -save-temps -o

like hke.c처럼 일반적인 C 소스 컴파일하듯이 하면 된다. 실행시켜 보면 실망스럽겠지
만 아무 일도 하지 않을 것이다.
이렇게 인라인 어셈블리로 작성된 부분은 다음 그림과 같이 컴파일러가 컴파일한 like.s
어셈블리 파일에 그대로 복사된다.

[그림 6-13] 컴파일된 like.s 파일

6장_ gas assembler 405

===== PAGE 407 =====
이제 다른 예제를 살펴보자.
〔예제 6-12〕 like.c 소스 코드

#include <stdio.h>
int main()
__asm______ volatile (
"movl $3, %eax\n"
)；
return 0;

이전과 별반 달라진 것이 없다. 위 코드는 단지 eax 레지스터에 상수 3을 집어넣는 일
밖에 하지 않는다. 상수는 여기서 보면 $ 기호를 앞에 붙었는데, 이것은 리눅스에서 사
용하는 AT&T 문법의 어셈블리 언어에서 상수를 표현할 때 쓰는 방법이다. 그리고 이
전에 한 줄로 썼던 것과는 다르게 세 줄로 늘렸다. 이렇게 줄을 늘려도 관계없다. 보통
의 경우 표현해야 될 인스트럭션이 적으면 한 줄에 몰아서 쓰고, 표현해야 될 인스트럭
션이 많으면 이 렇게 줄을 나누어 쓴다.
위 소스를 컴파일해도 싱겁게 아무 일도 일어나지 않고 끝나 버린다. 이제 다른 예제를
살펴보자.
〔예제 6-13) 느 like.c 소스 코드

#include <stdio.h>
int main()
{
int a = 0;
int b = 100;
__asm______ volatile (
"movl %1, %%eax\n\t"
"movl 옹%eax, %0\n"
: "=m" (a)
: "m" (b)
: "eax”

printf("a = %d, b = %d\n”, a, b);
return 0;
}

406

3부— 컴파일과 링킹

===== PAGE 408 =====
드디어 무언가 하는 듯한 소스가 나왔다. 다소 복잡해 보이지만 알고 보면 아주 간단한
인라인 어셈블리 문법이다.

"movl %1, %%eax\n\t"에서 %1의 의미는 콜론(‘：’)이 시작하는 데서부터 두 번째 인
자를 의미한다. 위 예에서는 "m" (b)라고 된 부분이 %1에 해당하고, 그 다음 줄에 %0
이라고 나온 부분은 "=mH (a)를 의미한다. 그리고 a와 b는 위에서 선언된 변수 a와 b를
의미한다.

a와 b 앞에 오는 "m"은 a와 b가 메모리 타입의 저장 공간이라는 의미다.
즉, "movl %1, %%eax\n\t" 는 변수 b 의 값을 eax 레지스터에 넣는다는 의미다. b 변
수에는 현재 100이 들어가 있기 때문에 eax 레지스터에는 100이 들어간다.
이전에 eax 레지스터를 지칭할 때는 %eax처럼 % 기호를 한 번만 써주었는데, 이번에
는 %% 기호를 두 번 써줬다. 그 이유는 인텔 AT&T 어셈블리 언어의 문법과 관련된 문
제로, 인텔 AT&T 어셈블리 언어는 레지스터를 표현할 때 % 기호를 붙인다. 그런데 인
라인 어셈블리에서 인수를 표현하는 것 역시 %를 붙이기 때문에 레지스터와 인수의 구
분이 모호해져 버린다.
그래서 결국 인수를 사용하지 않을 때는 레지스터에 % 기호를 하나 붙이고 인수를 사
용할 때는 인수와의 구분을 위해 레지스터에 % 기호를 두 번 붙여주는 편법을 사용한
것이다.
이것은 gcc 에서 사용하는 gas 어셈블러의 어셈블리 문법 중 레지스터 앞에 % 기호를
붙이는 특징 때문에 벌어지는 일이므로 인텔 아키텍처만 그렇고 나머지 아키텍처는 그
렇지 않다. 나머지 아키텍처는 레지스트 앞에 % 기호를 붙이지 않는다(필자가 알고 있
는 한도 내에서는…).
그리고 \n\t를 붙여주었다. __asm__으로 시작되는 부분은 모두 컴파일러에 의해 최적
화 과정이 끝나고 그대로 붙여넣기가 되는데, 그때 \n\t 를 붙여주지 않으면 어셈블리
소스가 흐트러져 버린다. 예를 들면 \n\t를 제거하면 다음과 같은 어셈블리 파일로 컴
파일된다.

6장_ gas assembler

===== PAGE 409 =====
[그림 6-14] 컴파일된 like.s 파일

그림에서 보이는 바와 같이 \n\t 를 제거하니 인스트럭션이 붙어버린 것을 알 수 있다.
이렇게 되면 어셈블 과정에서 오류가 발생한다. 어셈블러는 한 줄에 한 인스트럭션만
있는 것으로 가정하고 어셈블 과정을 수행하기 때문이다. \t는 인스트럭션의 앞에 탭을
두어 어셈블리 소스를 예쁘게 하기 위한 옵션이지만 \n은 필수다. 반드시 \n은 붙여주
고, 되도록이면 그냥 \n\t 이렇게 붙여주기 바란다.
자, 다시 위 소.스루 돌아가 Hmovl %%eax, %0\n" 분을 해석해 보면 eax 레지스터에
있는 값（현재 100） 을 첫 번째 인자 즉, a 변수에 넣는 일을 한다. 그래서 결국 a 변수의
값이 100이 된다. 그리고 이전에 없던 콜론 부분이 추가되었는데, 의미는 다음과 같다.

(a)
"m" (b)
"eax"

408 3부— 컴파일과 링킹

===== PAGE 410 =====
a 변수가 들어 있는 첫 번째 : "=m" (a) 필드는 출력을 의미한다. 함수에서 보면 리턴되
는 변수 또는 레지스터와 유사한 개념이다. 그리고 b 변수가 있는 두 번째 필드는 입력
을 의미한다. 마지막으로 오는 "eax"는 위 인라인 어셈블리를 수행한 후 변화되는 레지
스터를 적어 넣는 부분이다.
이 런 필드 부분은 반드시 위와 같이 한 필드에 하나만 쓸 수 있는 것은 아니다. 다음과
같이 콤마(,)로 구분해 여 러 개를 사용할 수 있다.

: "* (a) , "* (c) , "=m" (d)
: "m" (b), "m" (e)
: "eax", "ebx"

위와 같이 사용하면 a 변수는 인라인 어셈블리 내에서 첫 번째 인자이기 때문에 %0으
로 표현되고, c 변수는 두 번째 인자이기 때문에 %1로 표현된다.
마찬가지로 d 변수는 %2, b 변수는 %3 이런 식으로 표현된다. ‘=’이라고 붙은 것은 인
라인 어셈블리 수행 후 값이 바뀐다는 의미다. 이후 이 정보는 컴파일러가 읽어 들여
값이 바뀐 것들에 대해서는 최적화할 때 혹은 레지스터를 할당할 때 주의하게 된다.
출력 필드 부분에는 위의 예제에서 보는 바와 같이 모두 ‘=’ 기호를 붙여주어야 한다.

"m”이라고 붙은 것은 괄호 안에 오는 것의 메모리 타입이 저장 공간이라는 의미다. 이
런 지정자는 m만이 있는 것이 아니다. 이런 지정자에는 다음과 같은 것들을 사용할 수
있다.

• m： 메모리
• r： 범용 레지스터(eax, ebx, ecx, edx)
• i： 정수 상수나 문자열
• n： 정수 상수
• E： 부동소수점 상수
• F： 부동소수점 상수
• g： 범용 레지스터 또는 메모리 또는 상수
• X： 어떤 오퍼랜드도 허용
• p： 메모리 주소
• q： 범용 레지스터 (eax, ebx, ecx, edx)

6장_ gas assembler 409

===== PAGE 411 =====
• a： eax
• b：ebx
• c’ ecx
• d： edx
• D： edi
• S： esi
•

K： Oxff

• L： Oxffff
다소 난잡하게 보일지도 모르겠다. 다 각각의 의미가 있는 것들이고, 위 예는 i386 머
신에 종속된 것들도 있고 아닌 것들도 있다. 그리고 위에서 보이는 것 말고도 지정자는
많이 있다. 나머지는 매뉴얼을 보기 바라고 알맞게 골라서 쓰면 된다.
그리고 되도록 입력과 출력을 구분할 것을 당부한다. 입출력을 구분하지 않으면 평상시
에는 문제가 없다가 최적화 레벨에 따라 미묘한 문제가 발생하곤 한다.
이제 위 예제 소스를 비로소 컴파일해 실행해 보면 우리가 예상했던 것과 같이 a 변수
에 b 변수의 값인 100이 출력되는 것을 확인할 수 있다.

[그림 6-15] 컴파일 후 실행한 모습

이제 좀 더 색다른 예제를 다뤄보자.
〔예제 6너4〕 like.c 소스 코드

#include <stdio.h>
int main()
{
int a = 1;
char *str = "a = %dz number = %d\n";
__asm______ volatile (
"pushl %0\n\t"
"pushl %l\n\t"
"pushl %2\n\t"

410

컴파일과 링킹

===== PAGE 412 =====
"call printf\n\t”
"addl $12, %%esp\n\t”
: "g” (4*2) , ’’ g" (a) , "g" (str)
)；
__asm______ volatile ("movl $4, 옹eax\n\tmovl $5, %ebx\n") ;
return 0;

이번에 함수 호출의 경우를 예로 들었다. 위와 같이 사용하지 않는 출력 필드는 비워두어
야 한다. 그리고 4*2와 같이 상수를 직접 넣어주었다. 그리고 다음 한 줄의 코드는 인스트
럭션이 짧을 경우 이렇게 한 줄로 코딩해도 된다는 것을 보여주기 위해 넣은 코드다.
위 코드를 컴파일해 나오는 어셈블리 코드는 다음과 같다.

[그림 6-16] 컴파일 후 나오는 어셈블리 코드의 모습

6장_ gas assembler 411

===== PAGE 413 =====
_^흐므으^server：,work/book/utils_new/as2

丄旦 스］

[rootSseruer as2]tt gcc -saue-tenps -o like like.c
[rootBseruer as2]tt
[root@s하'uer as2j# ./like
a = 1, number = 8
[root@seruer* as2]tt |

［그림 6-17］ 실행 결과

이상이 인라인 어셈블리에 대한 기본적인 문법 설명이었다. 다소 부족한 점이 있지만
지금까지 이 책을 잘 따라온 독자라면 이미 많은 원리를 이해하고 있어 어셈블리 언어
만 알면 얼마든지 자신이 원하는 대로 응용해 볼 수 있을 것이다.
어셈블리 문법은 매우 간단하다. 데이터를 넣고, 빼고, 더하고, 곱하고, 나누고 그런 일
밖에 없다. 거부감 때문에 그렇지 막상 시작해 보면 C보다도 훨씬 쉽다. 어셈블리 문법
은 쉬운 반면에 어셈블리는 CPU에 대한 많은 백그라운드 지식을 요구한다. 하나씩 시
행착오를 겪으면서 도전해 본다면 결코 어렵지만은 않을 거라고 생각한다. 이제는 독자
에게 바톤을 넘기겠다. 힘껏 달리기 위해 독자가 갖춰야 될 것들은 모두 갖췄다. 원 없
이 힘껏 달려보기 바란다.

412 3부_ 컴파일과링킹

===== PAGE 414 =====
7

장

윤택하게 하는
바이너리
유틸리티

01 바이너리유틸리티사용하기

===== PAGE 415 =====
s S+c*dy
바이너 리 유틸리 티는 바이너 리를 조작하거나 바이너 리 정보를 보기 위한 프로그램들의
모임을 말한다. 이런 바이너리 유틸리티를 잘 활용하면 바이너리 파일에서 각종 유용한
정보를 얻을 수 있고, 또한 바이너리 파일의 사이즈를 줄인다든가 하는 여러 가지 일을
수행할 수 있다.

===== PAGE 416 =====
페 바•이너리 유틸리티 사용하기
바이너리 유틸리티는 binutils라는 패키지에 포함되어 있다. 때문에 다음 명령을 사용
하면 자신의 시스템에 어떤 바이너리 유틸리티가 설치됐는지 확인할 수 있다.
rpm -ql binutils | grep A/usr/bin
root④server：/work/book/utils_new/binutils
[rootSseruer binutils]tt rpm -ql binutils | grep A/usr/bin
/usr/bin/addr21ine
/usr/bin/ar
/usr/bin/as
/usr/bin/c++Filt
/usr/bin/gproF
/usr/bin/ld
/usr/bin/nn
/usr/bin/objcopy
/usr/bin/objdunp
/usr/bin/ranlib
/usr/bin/readelF
/usr/bin/size
/usr/bin/strings
/usr/bin/strip
[root@s하'ver binutils]tt |

[그림 7-1] 바이너리 유틸리티 목록

각각의 바이너리 유틸리티가 하는 일은 다음과 같다.

• addr21ine： 바이너리 파일에서 특정 주소가 어떤 파일의 어떤 라인인지 보여줌
• ar： 정적 라이브러리를 만들고 수정
•

as： GNU 어셈블러

• c++filt： C++ 또는 JAVA 심볼 문자열을 맹글링되기 전의 문자열로 보여줌
• gprof： 프로파일 정보 출력
• Id： GNU 링커
• nm： ELF 포맷 오브젝트 파일의 심볼을 보여줌
• objcopy： 오브젝트 파일의 복사 및 변환
• objdump： 오브젝트 파일을 덤프하거나 역어셈할 때 사용
• ranlib： 정적 라이브러리 내에 인덱스를 생성할 때 사용
• readelf： ELF 포맷의 오브젝트 파일 정보를 보여줌
• size： 오브젝트 파일의 사이즈 정보 출력
• strings： 바이너리에서 출력 가능한 문자열들을 출력
• strip： 오브젝트 파일의 사이즈를 줄임
7장—삶을 윤택하게 하는 바이너리 유틸리티 三415

===== PAGE 417 =====
이 중 Id와 ar, as는 이전에 하나의 장으로 설명을 했다. 그리고 이들 모두가 다 자주 사
용되는 것은 아니다. 그래서 이전에 설명했던 것들을 제외하고 자주 사용되는 것들 위
주로 하나씩 사용법을 설명하겠다.

I addr기ine 명령으로 특정 주소가 어떤 파일의 어떤 라인인지 알아보기
addr21ine 명령은 그렇게 많이 사용되지 않는다. addr21ine 명령은 다음과 같이 사용한다.
addr21ine -fe like 0x8048384

위 명령은 like 파일이 실제로 메모리로 로딩되었을 때 0x8048384번지가 어떤 소스 파
일의 어떤 라인 부분인지를 알아보고자 할 때 사용한다. 위 실행 명령에서 0x8048384
번지는 필자가 예를 들기 위해 미리 nm like 명령으로 main 함수의 번지를 알아낸 주
소 값이다. 그리고 위 명령을 사용하려면 like가 -g 옵션으로 디버깅 정보가 추가되게
컴파일되어 있어 야한다.
위 명령을 수행시키면 다음과 같은 결과가 나온다.

[root@seruer binutils]# gcc -o like like.c -g
[root@seruer binutils]tt
[root@seruer binutils]tt addr21ine -fe like 0x8048384
main
/work/book/utilsnew/binutils/like.c:3
[root@seruer binutils]# |

버
[그림 7-2] addr2line 실행 모습

즉, like 명령이 수행되어 메모리로 로딩되었을 때 0x8048384번지는 like.c 파일의 3번
째 줄 위치이고 main 함수 부분임을 알 수 있다.

I c++filt 명령으로 맹글링되기 전의 C-H- 또는 JAVA 심볼명 보기
맹글링 (mangling)은 C++나 JAVA 같은 객체지향 언어에서 함수명을 클래스명과 인자
타입으로 변경하는 것을 말한다. 예를 들면 다음과 같다.
class Config {
pub丄ic :
int OptionCheck (char 大flag) ;
int LineParse(char *line);
}；

416 3부_ 컴파일과링킹

===== PAGE 418 =====
위와 같은 클래스가 있을 때 멤버 함수인 OptionCheckO 함수와 LineParseO 함수는
컴파일러 내부적으로 다음과 같이 변경된다.
Config: :OptionCheck (char*)
Config: : LineParse (char*)

==> _ZN6ConfigllOptionCheckEPc
==> _ZN6Config9LineParseEPc

즉, 클래스명과 함수명, 인자 타입을 기준으로 OptionCheck와 같은 경
우에는 _ZN6Configl lOptionCheckEPc로, LineParse와 같은 경우에는

_ZN6Config9LineParseEPc로 심볼명이 변경된다. 이렇게 '클래스명과 함수명, 인자 타
입을 기준으로 함수의 심볼명을 변경하는 작업을 맹글링이라 한다.
객체지향 언어에서 멤버 함수의 심볼을 맹글링하는 이유는 함수 오버로드나 가상 함수
를 사용하기 위함이다. C와 같은 언어 에서는 함수명으로 해당 함수를 다른 함수와 유
일하게 구분해 줄 수 있지만, 객체지향 언어에서는 함수 오버로드나 가상 함수를 지원
하기 때문에 함수명으로 해당 함수를 유일하게 구분해 줄 수 없다. 때문에 함수명과 클
래스명, 인자 타입을 사용해 함수명을 맹글링해 바꿔주는 것이다.

c++filt 명령은 이렇게 맹글링된 함수명을 맹글링되기 전의 함수명으로 바꿔준다.
c++filt의 사용법은 다음과 같다.
$ c++filt ［디맹글링할심볼명］

그래서 필자가 간단하게 작성한 sarpd라는 C++ 프로그램에서 사용되는 맹글링된 심
볼들을 c++filt 명령을 사용해 디 맹글링해 보면 다음과 같다.
^root@server：/work/book/utils new/binutils/sarpd-1J
[root@seruer sarpd-1.1 ]1t Is -al sarpd
—rwxr-xr—x 1 root root 9108 7월 8 23:44 sarpd
[rootBseruer sarpd-1.1 ]ii
[root@seruer sarpd-1.1 ]#। grep

|

080485&Q T _ZN6Config11OptioriCheckEPc
88048630 T 2zN6ConFig9LineParseEPc
88048aa0 T _ZH6ConFigC1EiPPc
88848CF0 T _ZN6ConFigC2EiPPc
[root@seruer sarpd-1.1]tt____________________________________________________
[root@seruer sarpd-1.1]# c++Filt _ZN6Config110ptionCheckEPc
ConFig::OptionCheck(char*)
[ rootBserver sarpd—TTTjT"—""""""—
[root@seruer sarpd-1.1]# c*+filt _ZN6Config9LineParseEPc

으의뜨으三느띄흐흐으£의흐하_______________________________
ji’Footi하』,Fuer '’'SG’Fpd-’i .ijT™
"
——
——
[root@seruer sarpd 1.1]# |

［그림 7-3］ c++filt 명령으로 맹글링된 심볼을 디맹글링한 모습

7장_ 삶을 윤택하게 하는 바이너리 유틸리티 417

===== PAGE 419 =====
I gprof로 프로파일 정보 알아보기
이전에 컴파일러 옵션을 설명할 때 -pg 옵션에서 gprof를 사용하는 법을 알아보았다.
프로파일 정보는 바이너리가 수행될 때 생성되는 정보로, 어떤 함수가 몇 번 호출되었
고 어떤 함수에서 수행 시간은 얼마나 걸렸나와 같은 정보들이다.
이런 정보들은 주로 프로그램 병목 현상들을 찾을 때 이용되고, 특별히 많이 호출되거
나 시간을 많이 소비한 함수들을 최적화하기 위해 찾을 때 사용된다.
프로파일 정보를 보려면 먼저 -pg 옵션으로 실행 파일을 재컴파일해야 한다.

-pg 옵션으로 재컴파일하는 이유는 실행 파일에 프로파일 정보를 출력하는 코드를
집어 넣기 위해서다. 이렇게 -pg 옵션으로 컴파일하면 실행 파일이 수행 종료될 때

gmon.out 파일이 생성되는데, gprof 가 바로 이 gmon.out 의 정보를 이용해 프로파일
정보를 출력한다.
〔예제 7너〕 like.c 소스 코드

★include <stdio.h>

void fund (int delay)
{
printf("1”);
while (delay;
}
void func2 (int delay)
{
printf ("2");
whi丄e (delay--);
}
int main()
{
int i, j;
for (i=0; i < 16; i++) {
fund (80000000) ;
for (j=0; j < 4; j++) {
func2 (6000000);
}
}

3부— 컴파일과 링킹

===== PAGE 420 =====
printf(”\n");
return 0;

위와 같은 소스를 작성하고 다음 명령으로 컴파일한다.
$ gcc —pg -g -o like like.c

그리고 like 명령을 몇 번 수행한 후 gprof -b ./like〉like .profile 명령을 수행하고

like.profile 파일을 열어보면 다음과 같이 like 파일이 실행되던 동안의 프로파일 정보
를 확인할 수 있다.
j^roo^t@servef：/work/book/utils_new/binutils
31at profile:
Each sample counts
% cumulatiue
time seconds
78.88
4.37
21.74
5.58
저i
휴.

as 9.01
self
seconds
4.37
1.21

seconds.
calls
16
64

self
ms/call
273.34
18.85

total
ms/call
273.34
18.85

name
Fund
Func2

Call graph

granularity: each sample hit couers 2 byte(s) for 0.18후 of 5.58 s
econds
index % tine
[1]

100.8

"like.profile"

self

children

0.00
5.58
4.37
0.00
29L,
1110C

called

name

16/16

<spontaneous>
main [1]
Funci [2]
1,1

꼭대기

[그림 7-4] gprof -b ./like〉like.profile 명령 수행 후 like.profile 파일 내용

각 필드가 무엇을 의미하는지 아는 독자들이 있을 것이다. -b 옵션을 제거하고 gprof

./like〉like.profile 명령을 내리면 각 필드가 무엇을 의미하는지 자세한 설명도 함께
출력된다.
그리고 -pg 옵션과 함께 -g 옵션을 추가해 컴파일한 후 like 명령을 한 번 수행하고,

gprof -A ./like I less 명령을 내리면 다음 그림과 같이 소스 파일의 내용도 함께 출력
된다.

7장— 삶을 윤택하게 하는 바이너리 유틸리티 419

===== PAGE 421 =====
[그림 7-5] gprof -A ./like I less 명령 수행 모습

프로파일링 정보를 추출하는 데는 어떤 면에서 gprof보다 gcov가 더 유용할 때가 많다.

gcov는 binutils 패키지에 포함되는 패키지가 아니니 이번 장의 마지막에 잠깐 설명한다.

| nm으로 ELF 포맷의 심볼 테이블 보기
앞에서는 주로 바이너리의 심볼을 볼 때 nm 명령을 많이 사용했다.

[그림 7-6] nm like한 결과

위와 같이 nm like 명령을 내렸을 때 첫 번째 필드는 메모리에 로드되었을 때 함수나
변수의 주소임을 알 수 있고, 세 번째 필드는 심볼임을 알 수 있다. 그렇다면 두 번째 필
드의 알파벳은 무엇을 의미하는 것일까? 두 번째 필드의 의미는 다음과 같다.

420 3부_ 컴파일과 링킹

===== PAGE 422 =====
• A： 주소가 절대적이어서 변경되지 않는 심볼
• B： 심볼이 BSS 섹션（예: 초기화되지 않은 전역변수 등）에 있음
• C： 공통 심볼（초기화되지 않은 자료）
• D: 심볼이 data 섹션에 위치（예: 초기화된 전역변수 등）
• G： 작은 공간의 전역 객체, data 섹션（초기화된 자료）에 위치
• I： 심볼이 다른 심볼의 인다이렉트（간접 참조）임
•

N： 디버그 심볼

• R： 읽기 전용 섹션에 위치하는 심볼
• S： 작은 객체를 위한 BSS 섹션의 심볼
• T： text 섹션에 있는 심볼（코드）
• U： 정의되지 않은 심볼
• V： 확정적이지 않은 심볼, 링크 시에 확정적인 심볼을 만나면 변경됨
• W： 확정적이지 않은 심볼, 링크 시에 확정적인 심볼을 만나지 못하면 0으로 됨
• -： a.out 오브젝트 파일의 stabs 심볼
• ?： 알 수 없는 심볼
이런 심볼들을 원하는 종류만 뽑아 보여주려면 다음 옵션을 사용한다.

• -a： 디버깅 심볼까지 포함해 모든 심볼 출력
• -D： 동적 심볼만 출력 （공유 라이브러리의 심볼 등）
• -g： 외부 심볼만 출력
• -v： 주소로 출력 정렬
• -s： 정적 라이브러리의 심볼을 출력할 때 어떤 오브젝트 파일에 어떤 심볼이 있는
지출력

• -u： 정의되지 않은 심볼만출력
그리고 바이너리에서 유용한 심볼만 뽑아 심볼 맵 파일을 만들 때는 다음과 같은 명령
을 사용한다.
$ nm [바이너리명] I grep -v ' \ （ compiledX） \ |\ （ \.o$$\） \|\（ [aUw]
\） \I\（ \•\.ng$$\） \|\（ LASH[RL]DI\） ' | sort > Symbols.map

위 명령을 내리면 Symbols .map 파일이 만들어지는데, Symbols .map 파일에는 실제
유효한 심볼들만 정렬되어 들어 있다.

7장_ 삶을 윤택하게 하는 바이너리 유틸리티 421

===== PAGE 423 =====
I objcopy 사용하기
objcopy는 오브젝트 파일을 다른 오브젝트 파일로 복사할 때 사용한다. objcopy는 선
택적으로 필요한 부분만 복사할 수 있기 때문에 파일의 사이즈를 줄이는 데 주로 사용
하고 바이너리 포맷을 바꾸는 데도 사용한다. 가장 간단한 사용법은 다음과 같다.
$ objcopy like like.new

like 파일을 line.new로 복사하였다. 복사된 like.new는 기존의 like와 동일하다.
$ objcopy -0 binary like like.new

like 파일에서 인스트럭션과 데이터만을 뽑아 like.new 로 만든다. 이렇게 만들어진
like.new는 ELF 헤더도 붙지 않은 순수한 바이너리 자체다. 주로 부트로더를 만들 때
이 런 식으로 사용하는데, 이유는 다음과 같다.
모든 CPU마다 전원이 인가되었을 때 CPU가 인스트럭션을 처음 읽어 실행할 번지가
정해져 있다. 예를 들면 i386 계열 CPU는 OxFFFFO번지이고, ARM 계열 CPU는 0x0번
지이며, MPC860 CPU 같은 경우 OxFFFOOlOO번지다.

i386 계열 CPU는 전원이 켜지는 순간 OxFFFFO번지의 인스트럭션을 제일 처음 읽어
수행한다. OxFFFFO 번지에는 BIOS 의 POST (Power On Self Test) 프로그램으로 점프
하는 인스트럭션이 들어 있다.

ARM 계열 CPU는 전원이 인가되는 순간 0x0번지에 있는 인스트럭션부터 읽어 수행
한다.
이렇게 모든 CPU는 전원이 들어오는 순간 처음 명령을 읽어서 수행할 번지가 정해져
있다.

1386 PC 이외에는 대부분 처음 수행하는 프로그램은 부트로더인데, 이런 부트로더는 인
스트럭션이 제일 앞에 있는 바이너리여야 한다. 즉, ELF 헤더가 붙어서는 안 된다는 이
야기다. ELF 헤더는 운영체제에서 필요한 정보이지 CPU 명령인 인스트럭션이 아니다.

CPU는 정 말 단순하게 eip 레지스터가 가리키는 번지의 인스트럭션을 순차적으로 수행
하는 역할밖에 하지 못한다. ELF 헤더가 앞에 붙은 부트로더가 ARM 계열 CPU에서 메
모리 0x0번지에 있었다면 어떻게 되겠는가?

422

3부_ 컴파일과 링킹

===== PAGE 424 =====
당연히 ELF 헤더는 정상적인 인스트럭션이 아니므로 전원을 넣자마자 시스템이 정지
해 버린다. 이렇게 부트로더와 같은 특징을 가지는 프로그램들을 빌드할 때 objcopy

-O binary bootloader bootloader.bin 같은 명령을 사•용해 ELF 헤더를 완전히 제거
하고 프로그램 수행에 불필요한 나머지 섹션들을 완전히 제거해 준다.
$ objcopy -R .note -R .comment 丄ike like.new

위 명령을 수행하면 .note 섹션과 .comment 섹션을 제거하고 like .new 에 like 를 복사
한다. 원래 -R 옵션이 섹션을 제거할 때 사용되고, .note 섹션과 .comment 섹션은 실
행에 반드시 필요한 섹션이 아니므로 바이너리 사이즈를 줄일 때 위와 같이 사용한다.
$ obj copy -S like like.new

위와 같이 명령을 내리면 모든 심볼과 재배치 정보를 제거해 like.new 파일을 만든다.
그래서 바이너리 파일의 사이즈가 확실히 줄어든다. -R .note -R .comment 옵션과
같이 바이너리 파일의 사이즈를 줄일 때 자주 사용하는 옵션이다.
위의 예제들은 자주 사용하는 예제들이고, 나머지는 man objcopy 명령.0.루- 사용법을
알아보는 것도 좋을 것 이다.

I objdump 사용하기
objdump는 바이너리의 정보를 보여주는 명령이다. 오브젝트 파일의 어셈블리 코드를
볼 때 매우 유용한 명 령으로 자주 사용된다. objdump는 주로 바이너리 파일의 인스트
럭션 어 셈블리 코드를 볼 때 사용한다.
$ objdump —d like

위 명령은 filel.o 파일의 인스트럭션을 역어셈블해 보여준다. 그래서 다음 그림과 같이
어 셈블리 코드를 볼 수 있다.

7장_삶을 윤택하게 하는 바이너리 유틸리티

조

===== PAGE 425 =====
■■■■ -I 미 시

효1 root@server：/work/book/utils_new/binutils
8048639:
83 ec 04—
804863c:
a1 84 96 04 08
8048641：
83 F8 FF
8048644：
740c
al_ctors_aux+ 0x22>
80486467
83 eb 04
8048649：
FF d0
804864b:
8b 03
804864d：
83 F8 FF
8048650：
75 F4
al_ctors_aux+0x16>
8048652?
83 cU 04
8048655：
5b
8048656：
5d
8048657：
C3
Disassembly of section .Fini:
08048658 <_Fini>:
8048658：
8848659：
804865b：
804865c：
804865F：

55
89 e5
53
83 ec0스
e8 00

00 0000

8048664：
5b
8048665：
81 c3 04 11 00 00
804866b：
e8 cO Fd FF FF
al_dtors_aux>
8048670：
59
8048671：
5b
8048672：
C9
80n8673：
c3
[root(흐server binutils]tt |

sub
mou
cmp
je

$0x4,%esp
0x8 02(9684,%eax
$0xFFFFffFF,%eax
8048652 <_do_glob

sub
call
mou
crip
jne

$0x4,허ebx
*%eax
(%ebx)，헝eax
$OxFFFFFFFF,%eax
8048646 <_doglob

add
pop
pop
ret

$0x4,헝esp
%ebx
玄ebp

push
nou
push
sub
call

%esp,玄ebp
엉 ebx
수0x4,%esp

pop
add
call

%ebx
$Ox1104f%ebx
8048430 <_doglob

POP
POP
leaue
ret

엉ecx
헝ebx

싀

%ebp

8048664 <_

_Fini+0xc

기

[그림 7-7] objdump -d like 명령 결과

objdump -d like I less 명령으로 천천히 보면 main 함수의 인스트럭션과 fund,
func2 함수의 인스트럭션을 확인할 수도 있을 것이다.
위 명령의 결과는 순수한 어셈블리만 나와 있어 다소 보기가 힘들다. C 소스 코드와 같
이 보면 정말 한눈에 볼 수 있을 것이다. 다음 명령은 C 소스 코드와 함께 출력한다. 다
음 명령을 사용하려면 먼저 바이너리를 컴파일할 때 -g 옵션으로 디버깅 정보를 삽입
해야 한다.
$ objdump -S like

424 3부— 컴파일과 링킹

===== PAGE 426 =====
li/’ root@server：/work/book/utils_new/binutils

리m

■■K

JDI X|

uoid Func2(int delay)
{
80484d7：
80484d8：
80484da：
80484dd:
t>

55
89 e5
83 ec
e8 9a

08
Fe ff ff

| g브쁘트:으스 |
24 32 00 00 W
80484e2：
C7 04
Fe FF FF
80484e9:
e8 5e
lt>
[while (dela^-53
80484ee:
836d 08 01
80484F2：
837d 08 FF
bp)
80484F6：
75F6
7>
L」
80484F8：
80484F9：

push
IIOU
sub
call

호 ebp
헝esp,%ebp
$0x8,허esp

noul
call

$0x32,(허esp)
804834c <putchar@p

subl
cmpl

$0x1,8x8(%ebp)
$0xfFFfFFFF,0x8(%e

jne

80484ee <Func2+0x1

804837c <mcount@pl

leaue
ret

c9
C3

08O484Fa <nain>:
int main() |
<____________ 1
80484Fa:
80484Fe：
8048501：
8048504:
8048505：
8048507：
8048508:

8d4c
83 e4
FF71
55
89 e5
51
83 ec

214 04
F0
fc

14

lea
and
pushl
push
mou
push
sub

0x4(허esp)，혀ecx
$0xFFFFFFF0,%esp
QxFfFffffc(어ecx)
&ebp
후 esp,%ebp
Zecx
$0x14,%esp

：!

커

[그림 7-8] objdump -S like I less 명령 결과

objdump는 주로 이렇게 바이너리의 어셈블리 코드를 볼 때 사용하고, 나머지 유용한
옵션들은 다음과 같다.

• -a： 아카이브 헤더를 보여줌(예: objdump -a libmy.a)
• -x： 바이너리의 모든 헤더를 볼 때 사용
• -t: 심볼 테이블을 볼 때 사용

• -T： 동적 심볼을 볼 때 사용
• -r： 재배치 엔트리를 볼 때 사용
• -R： 동적 재배치 엔트리를 볼 때 사용
• -s： 모든 섹션들의 값을 볼 때 사용
나머지 옵션들은 readelf 명령의 기능과 중복되는 경향이 있다. 주로 ELF 포맷의 정보
를 읽는 기능들인데, 그런 것들은 readelf 명령을 사용하면 된다.

7장_ 삶을 윤택하게 하는 바이너리 유틸리티 425

===== PAGE 427 =====
I readelf 명령으로 ELF 파일의 각종 정보 보기
readelf 명령은 ELF 파일의 각종 정보를 보기 위한 명령이다. 앞에서 gcc와 Id, as에 대
해 알아볼 때 수없이 readelf 명령을 사용하였다. 때문에 여기서 따로 readelf 명령을
설명하지 않는다. 그냥 주로 사용하는 옵션들만 설명한다.

• -a： 모든 정보를 보여줌
• -h： ELF 헤더 정보를 보여줌
• -1： 프로그램 헤더들을 보여줌
• -s： 섹션 헤더들을 보여줌
• -e： 모든 헤더를 보여줌
• -s： 심볼 테이블을 보여줌
• -n： note 섹션의 정보를 보여줌
• -r： 재배치 섹션의 정보를 보여줌
• -d： 동적 섹션의 정보를 보여줌
다음은 ELF 바이너리 포맷에서 디버깅 정보를 포함하는 DWARF2라는 디버깅 정보 포
맷의 정보를 보는 옵션들이다. DWARF2는 다음과 같은 섹션들로 이뤄졌고. gcc로 컴
파일 시 -g 옵션을 주면 ELF 바이너 리 내에 포함된다.

• ,debug_info： 디버깅 심볼 정보（변수명, 함수명. 타입 등）가 들어 있는 섹션
• .debug_abbrev： .debugjnfo를 해석하기 위한 정보가 들어 있는 섹션
• .debugjine： 인스트럭션의 소스상 라인 정보가 들어 있는 섹션
• .debug_pubnames： 이름으로 심볼 정보를 찾을 수 있는 정보가 든 섹션
• ,debug_aranges： 주소로 심볼 정보를 찾을 수 있는 정보가 든 섹션
• .debug_str： .debug_* 섹션들에서 참조하는 문자열이 들어 있는 섹션
• .debug_loc： 로케이션 정보가 든 섹션
• .debug_frame： 함수 프레임 정보가' 든 섹션
--debug-dump=[=line,=infoz
=strz =loc]

위 옵션은

debug-d니mp=line 또는

=abbrev,=pubnamesz

debug—dump=info 같은 형식으^ 시~응•하

고, 인자에 따라 DWARF2의 각종 섹션의 내용을 보여준다.

426 =_ 컴파일과 링킹

=ranges,=macro,=frames,

===== PAGE 428 =====
I size 명령으로 오브젝트 파일의 사이즈 보기
size 명령은 오브젝트 파일의 text, data, bss 섹션에 대한 사이즈를 보여준다.
$ size like
주 root@server：/work/book/utils....new/binutils
[root@server
binutils]#
text
data
bss dec
1384
268
12
[rootSseruer binutils]# |

size

like
1664

hex Filename
680 like

[그림 7-9] size 명령으로 본 like 파일의 각 섹션 크기

I strings 명령으로 바이너리 내부 문자열 보기
strings 명령은 바이너리 내부에서 출력 가능한 문자열을 출력한다. 그래서 strings like
명령을 내리면 다음과 같이 like 바이너리에 포함된 출력 가능한 문자열들이 출력된다.
| 페' root@server：/work/book/utils_new/binutils
[rootBseruer binutils]# strings like
/lib/ld—linux.so.2
_______________ __
libc.so.6
lOstdinused
putchar
_______________
mcount
_mcleanup
_libc_start_main
_______________
GLIBO-1.3
GLIBC_2.0
PTRhp
[rooteseruer binutils]# |

[그림 7-10] strings 명령으로 본 like 파일 내부의 문자열

strings 명령은 바이너리를 간단하게 분석하려 할 때 유용하다.

| 오브젝트 파일의 사이즈 줄이기
strip 명령은 바이너리 파일의 사이즈를 줄일 때 사용하는 옵션인데, 매우 자주 사용하
고 유용한 명령이다. objcopy도 바이너리 파일의 사이즈를 줄일 때 사용하기 때문에
다소 기능이 중복되는 경향이 있다. 그러나 strip 을 사용하던 objcopy 를 사용하던 하
는 일은 똑같기 때문에 마음에 드는 것을 사용하면 된다. 보통의 경우 objcopy보다는

strip으로 파일 사이즈를 줄이는 것이 더 일반적이다.

7장— 삶을 윤택하게 하는 바이너리 유틸리티 427

===== PAGE 429 =====
바이너리 파일의 사이즈를 줄이는 작업은 컴파일 막바지에 한다. 주로 배포하려는 프로
그램이나 임베디드 시스템 같이 최대한 공간을 아껴 써야 하는 시스템을 위해 실행에
필요 없는 부분을 제거해 바이너리 사이즈를 줄인다.
$ strip -R .note -R .comment -s like

위 명령은 -R 옵션으로 .note 섹션과 .comment 섹션을 제거하고, -s 옵션으로 모든
실행에 필요 없는 심볼을 제거한다. 위 명령을 내리면 다음과 같이 like 파일의 사이즈
가 줄어든 것을 확인할 수 있다.
/ root④server：/work/book/utils_new/binutiis
[rootSseruer binutils]#ls-al like
—rwxr-xr—x 1 root root| 7865~| 7월 9 88:52 like
[root@seruer binutils]tt
[root@seruer binutils]# strip -R .note -R .comment -s like
[root@seruer binutils]tt
[root@server binutils]#ls_-al like
—rwxr-xr—x 1 root root| 3132~| 7월 9 81:18 like
[root@seruer binutils]tt |

[그림 7-11] strip 명령으로 파일 사이즈 줄이기

| gcov로 커버리지 정보 알아보기
gcov는 binutils에 포함된 패키지가 아니다. gcov는 gcc 패키지에 포함된 유틸리티다.
그런데 “binutils" 장에서 gcov를 설명하는 이유는, gcov가 하는 일이 컴파일과 직접적
인 관련이 없으며, 기능이 gprof와 유사해 비교 설명하기 좋기 때문이다.

gcov는 코드 커버리지를 파악하는 유틸리티다. 코드 커버리지는 코드에서 어떤 부분이
얼마만큼 수행되는지 찾는 일이다. 때문에 코드 커버리지를 수행하면 어떤 부분의 코드
가 한 번도 수행되지 않는지 확인할 수 있다. 이후 이런 정보로 해당 코드를 제거할지
여부를 결정할 수 있다.
그리고 프로그램을 테스트하기 위한 테스트 코드를 작성할 경우 소스 코드의 모든 부
분을 다 테스트할 수 있는 테스트 케이스를 작성했는지 확인하는 것도 가능하다.

gcov가 코드 커버리지 툴이라고 해서 반드시 코드 커버리지에만 사용하라는 법은 없
다. 어떤 점에서 gcov는 gprof보다 더 최적화를 위해 유용하게 사용될 수 있다.

gprof 가 프로파일링을 위해 좋은 툴이기는 하지만 부족한 점이 있다. 그것은 gprof 가
기본적으로 함수 단위의 프로파일링 정보만 제공한다는 점이다.

428 3부— 컴파일과 링킹

===== PAGE 430 =====
최적화를 위해서라면 어떤 함수가 얼마만큼 시간을 소비했는지 아는 것도 중요하다. 하
지만 이미 어떤 함수가 시간을 많이 소비한다는 것을 알았다면 해당 함수의 어떤 부분
에서 시간을 많이 소비하는지 아는 것도 중요하다.

gprof를 사용하면 함수의 수행 시간을 알 수 있지만 함수 내에 어떤 부분이 많이 수행
되어 시간을 많이 소비하는지 아는 것은 불가능하다. gcov는 베이직 블록 단위의 프로
파일링을 수행해 함수 내에 어떤 루프가 많이 수행되었는지, 어떤 if 문장에서 참인 문
장이 많이 수행되는지, 거짓인 문장이 많이 수행되었는지까지 확인할 수 있다.

gcov를 사용하는 법은 매우 간단하다. 먼저 다음과 같은 test.c 예제 프로그램을 작성
하자.
〔예제 7-2〕 test.c 소스 코드

#include <stdio.h>
int a, b, c;
int fund (int argl, int arg2)
{
int i, j, k;
for (i=0; i<0xfffff; i++) {
j = argl + arg2;
k=j*2*4*8*16;
if (1%2) a = argl + arg2 + i * 8 + k;
}
return a;
}
inline int func2(int al, int a2)
{
int i, j, t = 4;
for (i=0; i<0xfffff; i += 2) {
j = 3 * t;
b = 3 * t / (i + 1) ;
}
return b += j;
}
int main()
{
int i, h, y;
h = y = 0;

7장_삶을 윤택하게 하는 바이너리 유틸리티 429

===== PAGE 431 =====
for (i=0; i<0xf; i++) {
for (h=0; h<0xf; h+十) {
y = fund (h, i) ;
func2 (i, y);
}
for (h=0; h<0xf; h += 2) {
c = fund (y, 2) ;
b = func2 (h, i);
}
}
printf("END : %d 응d\n", a, b);
return 0;

［예제 7-2］ 의 소스 코드를 다음과 같은 컴파일 옵션으로 컴파일한다.
$ gcc -o test test.c -fprofile-arcs -ftest-coverage -g

-fprofile-arcs -ftest-coverage 옵션은 예제 소스 내 각 베이직 블록에 프로파일링
코드를 삽입하라는 옵션이다. 베이직 블록이 이해되지 않는 독자는 “gcc” 장에서 베이
직 블록에 대해 간략히 설명했으니 참고하기 바란다.
컴파일 후 프로그램을 수행시키면 test.gcda, test.gcno 파일이 생성된다. 이 두 개의
파일에 test.c 소스 파일에 포함된 각 베이직 블록의 프로파일링 정보가 들어있다.
수 root@server：/work/book/utils_new/gcov
[roog흐server gcou]tt gcc —o test'test.c[-FproFile—arcs -ftest-cou7
Page] -g
[root@seruer qcov]tt
[root@seruer gcov]tt|./test|
END : 46180350 12
_____________
[root@server gcov]tt[gcoui test.c |
File 'test.c'
Lines executed:100.OS허 oF 23
test.c:creating 'test.c.gcou'
[rootSseruer gcou]tt Is
test test.c jtes€.c^gcou| test.gcda test.gcno
[root@seruer gcou]1t H

커
［그림 7너2］ gcov를 이용한 프로파일링 정보 생성

430

3부_ 컴파일과 링킹

===== PAGE 432 =====
그리고 위 그림과 같이 gcov test.c 명령을 내리면 다음과 같은 test.c.gcov 파일이
생성된다.

[그림 7-13] 생성된 testc.gcov 파일 내용

test.c.gcov 파일을 보면 각 라인의 제일 앞에 있는 숫자가 해당 라인이 몇 번 호출되었
는지를 나타내는 숫자다. 이렇게 gcov를 사용하면 베이직 블록 단위의 수행 정보를 확
인할 수 있다. 이런 정보를 이용해 우리는 정확하게 어떤 부분을 최적화하는 데 좀 더
신경을 써야 하는지 알 수 있다.
이상 gcov를 포함한 바이너리 유틸리티 사용법에 대한 모든 설명이 끝났다. 이전 gcc,

Id를 잘 따라왔던 독자라면 바이너 리 유틸리티의 단순 사용법뿐만 아니라 원리와 출력
하는 각종 정보들의 의미도 쉽게 이해할 수 있었을 거라 본다.
바이너리 유틸리티는 익혀 놓으면 나중에 두고두고 유용하게 사용될 수 있기 때문에
꼭 익혀두자.

7장- 삶을 윤택하게 하는 바이너리 유틸리티

431

===== PAGE 433 =====
I 4부 I 디버깅
소프트웨어 개발 프로젝트에서 개발자들은 디버깅에 상당한 시간을
소모하곤 한다. 뛰어난 개발자는 훌륭한 산출물을 얼마나 빨리 산출
해 내는지에 따라 결정된다. 아무리 훌륭한 결과물을 내놓을지라도
남들이 평균 10일 만에 끝낼 일을 20일 동안 하고 있다면 뛰어난 개
발자라 할 수 없다. 그렇기 때문에 뛰어난 개발자는 탁월한 개발 능
력과 함께 탁월한 디버깅 능력도 반드시 갖추고 있어야 한다.
이번 과정에서는 개발 기간을 단축시키기 위한 여러 디버깅 기법과
디버깅 툴의 사용법을 알아본다.

===== PAGE 434 =====
8a
gdb 디버거

01 단순하지만 매우 강력한 디버거 gdb
02 gdb를 이용한 디버깅 테크닉

===== PAGE 435 =====
gdb 는 GNU 에서 만든 매우 강력한 디버거다. 리눅스 시스템에서 gdb 는 디버거의 표준
에 가깝다. 그렇기 때문에 리눅스 시스템 개발자가 gdb 를 사용하지 못하는 일은 있을
수도 없고 있어서도 안 된다. 이번 과정에서는 이런 gdb 의 사용법과 gdb 를 사용한 디버
깅 기법을 알아본다.

===== PAGE 436 =====
01 단순하지만 매우 강력한 디버거 gdb ]
본격적으로 gdb 설명에 들어가기 전에 필자가 독자들에게 반드시 해 주고 싶은 이야기
가 있다. 그것은 디버깅을 아무리 잘 하더라도 애초에 버그를 생성하지 않는 것만 못하
다는 점이다. 가장 뛰어난 디버깅 능력은 애초에 버그를 생성하지 않는 것이다.
이는 코딩 습관과 관련이 있고 인간적인 문제로 해석될 수 있다. 애초에 코딩하는 습관
이 잘못되 어 있으면 버그를 많이 양산할 수밖에 없다. 때문에 처음부터 코딩 습관을 잘
길들일 필요가 있다.
버그를 적게 생성하는 코딩 기법에는 테스트 주도 개발（ Test-Driven Development） 0]
나 방어적 프로그래밍 같은 여러 기법이 있다. 필자가 해당 프로그래밍 기법에 대해 대
략적으로라도 설명해 주면 좋겠지만 관련 책도 많이 나와 있으므로 생략한다. 그렇지만
자신의 코딩 습관이 의심스러운 독자가 있다면 관련 서적을 반드시 참고해 보기 바란다.
그래서 자신만의 코딩 습관을 적 립하기 바란다. 그러면 프로그래머 생활 내내 두고두고
도움이 될 것이라 확신한다.
하지만 아무리 코딩 습관을 좋게 바꾼다고 할지라도 디버깅에서 자유로운 것은 아니다.
인간은 완전하지 않기 때문에 실수를 할 수밖에 없기 때문이다. 때문에 gdb를 잘 사용할
줄 알아야 한다. 그럼 먼저 gdb를 간단히 소개한 후 바로 gdb 사용법을 알아보기로 한다.

I gdb에 대한 소개
이전에도 이야기했듯이 gdb 는 GNU에서 만든 매우 강력한 디버거다. 감히 강력하다
는 수식어를 붙일 수 있는 이유는 gdb가 원하는 만큼의 다양하고 많은 정보를 제공하
기 때문이다. gdb는 CLI（명령라인 인터페이스）를 통해 각종 정보를 제공하는데, 메모
리 정보, 스택 정보, 레지스터 정보 등 매우 다양한 정보를 제공한다. 그리고 gdb는 제
한적으로나마 멀티프로세스, 멀티스레드 디버깅이 가능하며, 원격으로 커널을 디버깅
할 수도 있다.

gdb는 굉장히 단순하고 직관적인 디버거다. 그래서 사용하기 쉽고 빨리 배울 수 있다.
물론 gdb가 기본적으로 텍스트 모드에서 동작하기 때문에 사용하는 데 다소 불편한 감
은 있다. 많이 불편하다면 GUI 모드를 지원하는 ddd（ gdb를 포함하는 GUI 디버거）와

8장_ gdb 디버거 | 435

===== PAGE 437 =====
kdbg도 있으니 취향에 따라 골라 사용하면 된다. 이중 ddd의 사용법은 뒤에서 따로 설
명한다.

gdb 는 C, C++, Objective-C, Fortran, Java, Pascal, assembly, Modula-2, Ada 등의 수
많은 언어를 지원하며, i386, arm, ppc, spare, mips, alpha 등의 수많은 아키텍처도 지원
한다. 또한 Linux, SunOS, BSD, Irix, lynxos 등 수많은 운영체제에서도 동작 가능하다.

GUK 지원하는 디버거인 ddd 도 있는데 굳이 gdb 를 알아야 되는 이유는 다음과 같
다. GUI 디버거가 자동카메라라면 텍스트 모드 디버거인 gdb는 수동카메라에 비유할
수 있다. 자동카메라는 쉽게 조작할 수 있고 카메라의 구조나 사용법을 잘 모르는 사용
자라 할지라도 사진의 품질을 어느 정도 보장받을 수 있다. 그러나 입맛에 맞는 원하는
사진을 찍을 수는 없다. 반면 수동카메라는 배우기 어렵고, 구조나 원리를 잘 알아야 사
진의 품질을 보장받을 수 있는 단점은 있지만 원하는 사진을 찍을 수 있다. 수동카메라
로 사진을 잘 찍고 못 찍고는 전적으로 카메라를 조작하는 사람에게 달린 문제다.
처음엔 다소 불편할지도 모르겠지만 gdb는 매우 단순하기 때문에 익숙해지면 누구나
원하는 사진을 찍을 수 있다. gdb가 어렵다는 선입견을 가지고 있는 사람들에게 필자
가 공언하건대 gdb는 매우 단순하고 쉽다.

I gdb로 간단한 디버깅 따라 하기
gdb 역시 vim 과 마찬가지로 눈으로 익히는 디버거는 아니다. gdb를 잘 다루려면 gdb
명령들을 많이 알아야 되는데, 따라 하다 보면 저절로 알게 된다. 설령 명령을 모르더라
도 걱정할 필요는 없다. gdb 는 강력한 자동 완성 기능과 history 기능, 그리고 help 명
령으로 원하는 명령을 쉽게 확인할 수 있기 때문이다. 그럼 먼저 앞으로 실습에서 사용
할 소스 코드를 작성하자.
〔예제 8너〕 bugprg.c 파일의 내용

#include <stdio.h>
struct time {
int hour;
int min;
int sec;
} gtime = {1,2,3}, gtimes[4];
char *array[4] = {"one", "two", "three"};

436 4부—디버깅

===== PAGE 438 =====
int func (short sw, char *str)
{
printf ("first char = %c\n", *str) ;
if (sw)
return 2;
return 3;
}
int main()
{
int Ival = 2331, i;
char *lstr = "I like you. ’’;
struct time *pt = &gtime;
for (i=0; i < 4; i++) {
printf("loop 응d : ", i);
gtime.hour += func(i % 2, array[i]);
}
return 0;
}

［예제 8-1］ 을 보면 알겠지만 문제가 있다. 문제를 발견했다고 해서 스스로 문제를 고치
지 말지 바란다. 그랬다가는 프로그램은 잘 돌아가겠지만 다음부터 해야 될 일이 없어
질 것이다. 일단은 자신을 세뇌시키면서 애써 모른 척하고 ［예제 8-1］ 을 컴파일한다.
gcc -g -o bugprg bugprg.c

gdb를 사용해 디버깅하려면 위 명령처럼 -g 옵션을 붙여야 한다. -g 옵션을 붙이면 컴
파일되는 실행 파일에 여러 디버깅 정보가 삽입된다. 여기서 디버깅 정보란 내부에 사
용된 심볼 문자열과 심볼의 주소, 컴파일에 사용된 소스 파일 등이 해당되고, 가장 중요
한 컴파일된 각각의 인스트럭션들이 어떤 소스 파일의 어떤 행에 해당되는지 등의 정
보도 포함된다.
: 이런 디버깅 정보들은 ELF 바이너리 포맷 내에 .debug?■라는 이름을 가지는 섹션에 들어있다. 그리고
각각의 디버거 섹션에 들어가는 정보의 종류와 자료 구조는 DWARF라는 디버깅 정보 포맷이라는 규약
을 따른다. 현재까지 DWARF는 버전 3까지 개발되었으며, 주로 사용되는 것은 DWARF2다.
디버거를 개발하기 원하는 독자나 디버거의 작동 원리가 궁금한 독자들은 DWARF 디버깅 정보 포맷의
매뉴얼을 찾아 읽어보기 바란다.

8장_ gdb 디버거 437

===== PAGE 439 =====
“컴파일러” 장에서 언급했듯이 c 소스 각각의 한 행은 한 묶음의 어셈블리 코드와 대
응된다. 컴파일이 끝난 후 생성되는 각 어셈블리 코드 묶음을 c 소스의 각 행과 비교할
수 있게 소스 파일과 해당 인스트럭션이 어떤 C 소스 행에 해당되는지 등의 정보가 추
가된다. 이런 정보를 이용하면 gdb 에서 C 소스를 보면서 디버깅하는 것이 가능하다.

-g 옵션을 붙이지 않으면 C 소스의 행 정보7} 포함되지 않아 어셈블리 코드만 보면서
디버깅하는수밖에 없다.

-g 옵션을 주고 컴파일할 때는 최적화 옵션（ -O 옵션 등）을 사용하지 않는 것이 좋다.
최적화 옵션을 사용해 최적화 과정을 수행하면 어셈블리 코드 자체에 많은 변경이 가
해져 C 소스의 한 행과 대응되는 어셈블리 묶음이 흐트러진다. 그래서 디버깅할 때 코
드의 흐름 자체가 C 소스의 흐름을 따르지 않고 들쑥날쑥할 수 있다.

gcc -g -o bugprg bugprg.c 명령으로 컴파일한 bugprg 프로그램을 실행시키면
［그림 8-1］ 과 같이 오류가 출력되는 것을 확인할 수 있다.

［그림 8-1］ b니gprg 실행 화면

그럼 gdb 의 사용법도 익힐 겸 gdb 를 사용해 어디에서 문제가 발생했는지 한번 알아
보자.

I gdb의 시작과 종료
gdb를 시작하는 방법에는 여러 가지가 있을 수 있다. 가장 단순한 방법은 다음과 같이
하는것이다.
gdb bugprg

위와 같이 명령을 내리면 ［그림 8-2］ 와 같은 검은 바탕에 횐색 글씨가 가득한 썰렁한
화면이 나타난다.

438 4부— 디버깅

===== PAGE 440 =====
root@os：/temp/gdb

_싀믜씌

[rootdos gdb]tt gdb bugprg
GNU gdb Red Hat Linux (6.6-8.Fc7rh)
Copyright (C) 2006 Free Software Foundation, Inc.
GDB is free software, covered by the GNU General Public License, and pou are ■
welcome to change it and/or distribute copies oF it under certain conditions.H
Type "show copying" to see the conditions.
There is absolutely no warrant少 For GDB. Type "show warranty" for details. I
This GDB was configured as ''i386-redhat-linux-gnu"_______________________
Using host libthread db library "/lib/libthread db.so.1".
(gdb) |

［그림 8-2］ gdb 실행 화면

［그림 8-2］ 에서 사용한 명령 외에도 프로그램이 죽을 때 코어(core) 파일이 생성되었
다면 코어 파일을 이용해 디버깅할 수도 있다. 코어 파일은 프로세스가 수행 중에 치명
적인 예외가 발생해 더 이상 수행이 불가능할 때 생성된다. 이런 치명적인 예외 상황이
란 0으로 나눈다던지 잘못된 메모리 참조 등과 같은 상황들이 있고, 운영체제 내에서
어떤 경우에 코어 파일을 생성할지 미리 정의되어 있다.
예외 상황에 처하면 운영체제는 시그널을 해당 프로세스에 보내고, 시그널을 받은 프로
세스는 커널에 있는 기본 시그널 핸들러를 수행하는데, 기본 시그널 핸들러에서 코어
파일로 저장하는 부분이 있다면 현재 수행 중인 프로세스의 이미지를 코어 파일로 저
장한다. 즉, 코어 파일이 란 문제가 발생해 프로세스가 종료되는 순간의 프로세스 이미
지 파일로, 여기에는 종료 순간의 CPU context와 프로세스의 코드 및 데이터, 스택 등
의 정보가 들어 있어 디버깅할 때 유용하게 사용할 수 있다.
또한 gdb는 현재 수행 중인 프로세스를 디버깅하는 것도 가능한데, 그때는 gdb ［프로
그램명］ ［현재 수행 중인 프로세스의 PID］ 같은 형식으로 실행한다. 지금은 gdb의 기
본적인 사용법을 익히는 것이 급하기 때문에 코어 파일을 이용한 디버깅 방법과 수행
중인 프로세스의 디버깅은 나중에 따로 설명한다. gdb를 종료하는 방법은 프롬프트 창
에서 q(quit) 명령을 내리거나 OH］ +d 키를 누르면 된다.
► 실행 방법

• gdb ［포루77■램명 ］ 예) gdb bugprg
• gdb ［프로그램명］ ［ core 파일명］ 예) gdb bugprg core. 14998
• gdb ［프로그램명］ ［실행 중인 프로세스 PID］ 예) gdb bugprg 14998
► 종료 방법

•q
• ［ Ctrlj+d

8장_ gdb 디버거 서 439

===== PAGE 441 =====
I 소스 보기
l(list) 명령을 입력하면 ［그림 8-3］ 과 같이 소스의 내용을 출력한다.

［그림 8-3］ I 명령을 입력해 소스의 내용을 본 화면

다시 1을 누르거나 아무 입력 없이 lEnter］ 키를 누르면 소스의 나머지 부분을 보여준다.

gdb에서 아무런 입력 없이 gnier］ 키를 누르는 것은 바로 전 명령의 반복을 의미한다.
특정한 행을 보려면 1 ［행 번히 명령을 내린다. 가령 10행 주위의 소스 파일 내용을 보
려고 한다면 다음과 같이 입 력한다.
1 10

마찬가지로 특정한 함수 부분을 보고 싶다면 1 ［함수명］과 같이 입력한다. 그리고 소스
가 여러 파일로 분산되어 있어 다른 파일에 있는 함수를 보고자 한다면 1 ［파일명］:［함
수명］ 명령을 사용한다. ［그림 8-4］ 는 1 func를 입력해 func 함수의 소스 부분을 출력
한 모습이다.

［그림 8-4］ I func 명령을 이용해 func 함수의 소스를 출력한 모습

그 외에도 여러 가지 소스를 출력하는 명령이 있는데, 많이 쓰는 것들은 위에서 설명한
것과 1 -를 들 수 있다. 1 -는 출력된 첫 행 이전의 행들을 출력하는 명령이다. 즉, 출력
된 첫 행이 23행일 경우 1 -하면 13~22행을 출력해 보여준다.

44(f 4부- 디버깅

===== PAGE 442 =====
［표 8-1］ list 명령 사용법 예
I

main 함수를 기점으로 소스 출력

110

10행을 기준으로 출력

I func

func 함수의 소스를 출력

I-

출력된 행의 이전 행을 출력

I file.c：func

file.c 파일의 func 함수 부분을 출력

I file.c：10

file.c 파일의 10행을 기준으로 출력

1 명령은 기본적으로 10행의 소스 코드를 출력하는데, 10행의 소스 코드를 보고 있으면
다소 답답한 느낌이 들것이다. 출력되는 행의 수를 변경하는 명령은 다음과 같다.
set listsize 20

위 명령을 내리면 출력 행이 10행에서 20행으로 늘어난다.

| 브레이크포인트
bugprg 프로그램을 실행시켜 보면 알겠지만 bugprg 프로그램과 같이 이상 종료하는
프로그램을 gdb 로 디버깅할 때 제일 먼저 하는 일은 gdb 에서 그냥 한번 실행시켜 보
는 일이다. 프로그램을 실행하는 명령은 r(mn)인데, i• 명령을 내려 프로그램을 수행했
을 때 프로그램이 이상 종료했다면 gdb 는 어떤 파일, 어떤 함수, 어떤 라인에서 어떤
문제가 발생했다는 것을 화면에 출력한다. 우리는 이렇게 출력되는 메시지를 보고 그
부분에 가서 확인만 하면 된다.
［그림 8-5］ 는 r 명령을사용해 프로그램을 실행시켰을 때 gdb가 결과를 출력한 모습이다.

［그림 8-5］ r 명령을 입력해 프로그램을 수행한 모습

［그림 8-5］ 에서 보면 bugprg 프로그램은 세그먼트 폴트가 발생해서 이상 종료했는데,

bugprog.c 파일의 14 행에 해당하는 func 함수 내에서 세그먼트 폴트가 발생했음을

8장_ gdb 디버거

441

===== PAGE 443 =====
알 수 있다. 그리고 func 함수는 두 개의 인자로 호출되는데, 각 인자 값이 1과 0x0이라
는 것도 확인할 수 있다.
［그림 8-5］ 의 정보만으로도 func 함수의 str 인자에 널 포인터(0x0)가 입력되어 해당
널 포인터 값을 printf 함수로 출력하려고 하니 세그먼트 폴트가 발생했다는 것을 누구
나 유추할 수 있다. 그러면 어떤 함수의 호출을 통해 func 함수가 호출되었는지 확인하
기 위해 bt 명령을 입력해 ［그림 8-6］ 과 같이 스택을 백트레이스해 보자.

［그림 8-6］ bt 명령으로 스택 프레임을 본 모습

백트레이스는 프로그램의 스택 프레임을 순차적으로 따라가면서 해석해 현재 수행 코
드까지 어떤 함수들의 호출이 있었으며 , 각 함수를 호출할 때 인자는 무엇인지 확인 가
능하게 한다. bugprg 프로그램은 너무도 단순해 굳이 백트레이스해 보지 않더라도 어
떤 함수가 func 함수를 호출하였는지 금방 알 수 있고 어떤 부분이 잘못되었는지도 금
방 알 수 있다. 하지만 실전에서는 bugprg 프로그램 같은 단순한 프로그램은 보기 힘
들다. 백트레이스는 실전에서와 같이 복잡한 호출 관계를 가지고 있는 프로그램에 문제
가 발생했을 때 문제 발생 지점의 호출 경로를 찾을 때 유용하게 사용한다.
［그림 8-6］ 을 보면 func 함수는 main 함수에서 호출하였고, 인자 sw는 1, 인자 str은

0x0의 값을 가지고 호출되었음을 확인할 수 있다. 이렇게 세그먼트 폴트와 같은 예외
로 인해 이상 종료하는 프로그램이라면 그냥 한번 수행시켜 gdb에서 출력되는 정보만
으로도 디버깅하는 데 많은 도움이 된다.
백트레이스한 후에 보통의 경우 문제가 발생한 스택 프레임을 선택해 디버깅하기 시작
한다. 아니면 지금까지 얻은 정보를 바탕으로 func 함수가 호출되는 부분에 브레이크
포인트를 설정해 어떨 때 func 함수의 str 인자로 0x0 값이 넘어가는지 확인한다. 하지
만 지금 우리는 gdb를 처음 배우고 있는 단계이기 때문에 기본 사용법을 익히기 위해

main 함수의 시작 부분에 브레이크포인트를 설정하자.
b main

위 명 령을 내리면 ［그림 8-刀과 같이 main 함수의 시작 부분에 브레이크포인트가 설정
된다. 그래서 r 명령으로 프로그램을 다시 수행시키면 브레이크포인트를 설정한 부분

442 4부—디버깅

===== PAGE 444 =====
에서 프로그램 수행이 멈추는 것을 확인할 수 있다.
x mot@os：/temp/9db
(gdb) b main
Breakpoint 1 at 0x80483F9: File bugprg.c, line 24.
(gdb) |

[그림 8-7] b main 명령으로 main 함수의 시작 부분에 브레이크포인트 설정

브레이크포인트를 설정하는 방법에는 여러 가지가 있을 수 있는데, 다음 표와 같다.
[표 8-2] 브레이크포인트 명령
b func

func 심볼의 시작 부분에 브레이크포인트 설정

b10

10행에 브레이크포인트 설정

b file.c：func

file.c 파일의 func 심볼에 브레이크포인트 설정

b file.c：10

file.c 파일의 10행에 브레이크포인트 설정

b+2

현재 행에서 2개 행 이후 지점에 브레이크포인트 설정

b-2

현재 행에서 2개 행 이전 지점에 브레이크포인트 설정

b*0x8049000

0x8049000 주소에 브레이크포인트 설정(어셈블리로 디버깅 시 사용)

b 10 if var = 0

10행에 브레이크포인트를 설정하는데, var 변수의 값이 0일 때 작동

rb fun*

*fun*에 해당하는 모든 심볼에 브레이크포인트 설정

rb ^un

fun으로 시작하는 모든 심볼에 브레이크포인트 설정

rb TestClass"

TestClassOII 해당하는 모든 심볼에 브레이크포인트 설정

b 10 if var == 0과 같은 형식으로 브레이크포인트를 설정하는 것은 gdb의 아주 멋진
기능 중 하나다. b 10 if var == 0 명령의 의미는 10 행을 수행할 때 var 변수 값이 0 이
라면 브레이크를 건다는 의미다. 그리고 b 20 if var〉0 명령의 의미는 20행을 수행할
때 var 변수 값이 0보다 크다면 브레이크를 건다는 의미다.
이와 같이 어떤 상황에 맞게 브레이크를 걸게 할 수도 있고 그냥 통과시킬 수도 있는
기능은 매우 편리하기 때문에 자주 사용된다. 10행에 이미 브레이크포인트가 설정되어
있다면 condition 명령으로 브레이크가 걸릴 조건을 설정하거나 변경할 수 있다.
condition [N] var ==
condition [N] func(i) > 5

0

condition [N] var == 0 명령은 N번 브레이크포인트에서 var 변수가 0 일 때 동작하라
고 설정한다. 여기서 N번이란 브레이크포인트의 고유 번호를 의미한다. 모든 브레이크
포인트는 1부터 시작하는 고유 번호를 가지는데, 고유 번호는 바로 뒤에서 설명한다.

8장_ gdb 디버거 443

===== PAGE 445 =====
10행에 설정된 브레이크포인트의 고유 번호가 2라면 condition 명령으로 condition 2
var == 0과 같이 명령을 내려 브레이크가 걸릴 조건을 설정할 수 있다.
condition [N] func(i)〉5 명령은 ftmc(i)의 값이 5보다 클 때 N번 브레이크가 동작하
라는 명령이다. condition 명령은 이와 같이 함수 호출과 함께 좀 더 복잡하게 사용 가
능하다.
ignore [N] 100

위 명령은 N번 브레이크포인트가 100번 지날 때까지 무시하라는 의미다. ignore 명령
은 루프 내에서 특정 횟수의 루프를 돌린 후 브레이크포인트가 걸리게 할 때 유용하다.

rb 명령은 rbreak 명령으로 사용될 수도 있다. rb 명령은 정규 표현식을 사용해 브레이
크포인트를 설정하는 명령이다. 그래서 정규 표현식을 사용해 여러 심볼에 손쉽게 브레
이크포인트를 설정하는 것이 가능하다.

b 명령으로 브레이크를 설정하면 gdb가 종료할 때까지 유효하다. 그러나 때로는 한 번
만 브레이크를 걸고 싶을 때도 있을 것이다. 그때는 b 명령 대신 tb 명령(한 번만 사용
되는 브레이크포인트 설정, 사용법은 b 명령과 동일하다)을 사용하면 된다.
설정된 브레이크포인트를 지우는 명령은 clear (줄여서 cl 로 쓰기도 한다) 명령이다.

cl main하면 main 함수에 설정되어 있는 브레이크포인트가 지워진다. 브레이크포인트
를 지우거나 상태를 변경하는 명령은 [표 8-3]과 같다.
[표 8-3] 브레이크포인트 지우기 및 상태 변경 명령
cl func

func 함수의 시작 부분에 브레이크포인트 지움

이 10

10행의 브레이크포인트 지움

cl file.c：func

file.c 파일의 func 함수에 브레이크포인트 지움

cl file.c：10

file.c 파일의 10행에 있는 브레이크포인트 지움

d

모든 브레이크포인트를 지움

disable br

모든 브레이크포인트 비활성화

disable br 1

1번 브레이크포인트 비활성화

disable br 1 3

1번, 3번 브레이크포인트 비활성화

enable br

모든 브레이크포인트 활성화

enable br 1

1번 브레이크포인트 활성화

enable br once 1

1번 브레이크포인트를 활성화하고, 한 번만 걸리고 비활성화되게 설정

enable br d이ete 1

1번 브레이크포인트를 활성화하고, 한 번만 걸리고 제거되게 설정

444 4부_ 디버깅

===== PAGE 446 =====
현재 설정되어 있는 브레이크포인트를 보여주는 명령은 info breakpoints 명령 또는

info b 명령이다. info breakpoints 와 같이 긴 명령을 위해서 gdb 는 세 가지 기능을
제공하는데, 하나는 info b 와 같이 축약형이고, 다른 하나는 히스토리 기능이 있어서

T 키를 누르면 이전에 타이핑한 내용이 출력되는 것이다. 그리고 가장 쓸모 있는 나머
지 하나는 바로 자동 완성 기능이다. info 바만 입력하고 Tab］ 키를 누르면 나머지 글자
를 적지 않아도 gdb 가 알아서 info breakpoints로 명령을 만들어준다. 또한 info 만 입
력하고 Tab］ 키를 두 번 이상 누르면 info 뒤에 올 수 있는 인자들의 리스트가 나열된다.
사용 가능한 명령이 생각나지 않을 경우 아무것도 입력하지 않은 상태에서 ¥ 키를
두 번 누르면 사용 가능한 모든 명령의 리스트가 나열된다. 때문에 명령이 기억나지 않
을 때 유용하게 사용할 수 있다. ［그림 8-8］ 은 info breakpoints 명 령으로 본 브레 이크
포인트 리스트다.

［그림 8-8］ 브레이크포인트 설정 상태

필자는 지금 b main 명령과 b func 명령을 이용해 브레이크포인트를 두 개 설정해 놓
은 것을 알 수 있다. 이렇게 main 함수와 func 함수에 브레이크포인트를 설정하면 당
연히 main 함수의 시작 부분에서 멈추고 func 함수의 시작 부분에서 멈춘다.
나중에 func 함수의 시작 부분에 있는 브레이크포인트가 필요 없어졌다면 cl func 명
령으로 브레이크포인트를 지워도 되지만, disable 2 명령을 사용해 func 함수에 설정
되어 있는 브레이크포인트를 비활성화시킬 수 있다. 이렇게 비활성화되어 있는 브레이
크포인트는 enable 2 명 령으로 다시 활성화시 킬 수 있다.
여기서 숫자 2는 ［그림 8-8］ 에서와 같이 브레이크포인트의 고유한 번호를 의미한다.
［그림 8-8］ 에서 func 함수에 설정된 브레이크포인트의 번호는 2번이다.

8장_ gdb 디버거 ! 445

===== PAGE 447 =====
I 프로그램 실행
b main 명령으로 main 함수의 시작 부분에 브레이크포인트를 설정했다면 r(run) 명령
으로 프로그램을 실행한다. 이미 프로그램이 실행 중일 때 r 명령을 내리면 재시작하고,

k 명령을 내리면 프로그램이 종료한다.
지금 디버깅에서 사용하는 bugprg 프로그램은 프로그램 실행 시 별도의 인자를 필요
로 하지 않는다. 그래서 그냥 r 명령만 내려주면 프로그램이 실행된다. 그러나 find 같
은 프로그램은 인자를 요구한다. 인자를 붙여주어야 실행되는 프로그램이라면 r 명령
뒤에 r ./ -name *.c -print와 같이 인자를 적어준다.
［표 8-4］ 프로그램 실행 명령

r

프로그램 실행

r arg1 arg2

arg1 과 arg2를 인자로 프로그램 실행

k

프로그램 실행 종료

r 명령으로 bugprg 프로그램을 실행하면 이전에 브레이크포인트를 설정한 main 함수
의 시작 부분에 멈추면서 ［그림 8-9］ 와 같은 문자열이 출력된다.

［그림 8-9］ r 명령으로 bugprg 프로그램 수행

여기서 S(Step)를 입력하면 현재 행을 수행하고 멈춘다. 현재 행이 함수를 호출하는 부
분이라면 함수를 수행하는데, 함수의 내부로 들어가서 수행된다. n(next)을 입력하면
마찬가지로 현재의 행을 수행하고 멈추는데, 함수 호출하는 부분이라면 함수의 내부로
들어가지 않고 그냥 함수를 수행한다. 그리고 c(continiie)를 입력하면 다음 브레이크
포인트를 만날 때까지 멈추지 않고 계속 수행한다.
다음 그림들은 s 명령과 n 명령의 차이점을 보여주는데, S 를 계속 입력했을 때 func
함수를 호출하는 라인을 만나면 func 함수의 내부로 들어간 모습과 n 명령을 사용해

func 함수를 호출하는 라인에서 함수만 수행하고 내부로는 들어가지 않는 모습을 보여
준다.

446 4부- 디버깅

===== PAGE 448 =====
［그림 8-10］ s 명령을 사용해 한 행씩 수행하면서 함수 내부로 들어간 모습

［그림 8-11］ n 명령을 사용해 한 행씩 수행한 모습（함수 내부로 들어가지 않음）

gdb를 이용해 디버깅할 때는 s, n, c 명령을 잘 조합해서 사용해야 불필요한 키 입력에
에너지를 낭비하지 않을 수 있다. 일단 s, n, c의 의미를 명확하게 숙지하고 계속 사용
하다 보면 어떻게 하는 것이 좀 더 효율적인지 저절로 알게 될 것이다.
［그림 8-1 이과 ［그림 8-11］ 에서 필자는 여러분에게 보이기 위해 s와 n을 계속 입력했
지만 s를 반복 입력할 경우 한 번만 s를 입력하고 나머지는 Enter） 키를 눌러 대신할 수
있다. 또한 s 6을 입력하면 S를 6번 입력한 것과 동일하고, n 6하면 n을 6번 입력한 것
과 동일하다는 점도 기 억하기 바란다.
［표 8-5］ 진행 명령 요약 1
S

현재 행 수행 후 멈춤, 함수 호출 시 함수 내부로 들어감

s6

s를 6번 입력한 것과 동일

n

현재 행 수행 후 멈춤, 함수 호출 시 함수 수행 후 다음 행으로 감

n6

n을 6번 입력한 것과 동일

c

다음 브레이크포인트를 만날 때까지 계속 진행

8장_ gdb 디버거 447

===== PAGE 449 =====
자, ［예제 8-2］ 와 같은 코드가 있다. 그런데 for문 부분에서 실수로 s를 입력해 for문
내부로 들어가 버렸다고 가정해 보자.
〔예제 8-2〕 for문을 빠져 나오는 경우를 설명하기 위한 예제

• •.상략

for

(i=0; I < 1000000;
num += i;
printf(”%d\n", num);

i+十)

{

}
... 하략

여기서 백만 번 동안 Enterl 키를 누르고 있을 독자는 없을 거라고 생각한다. 이때는

u(until)를 입력해 for문에서 빠져나올 수 있다. 그리고 현재 수행하고 있는 함수가 매
우 길어 함수가 끝난 시점으로 가고 싶으면 finish 명령을 사용한다. 함수의 나머지 부
분을 수행하지 않고 바로 빠져 나오고 싶다면 return 명령을 사용한다. return 1234와
같이 return 명령 뒤에 인자를 붙이면 함수의 리턴 값이 된다. u 명령과 finish, return
명령은 s. n, c 명령과 함께 자주 사용되는 명령이기 때문에 반드시 숙지하자.
이제까지 소개한 명령 외에 다른 진행 관련 명령에는 si, ni가 있다. si나 ni 모두 현재의
인스트럭션 하나를 수행한다. 두 명령의 차이점은 s, n과 같이 si는 함수를 호출하는 인
스트럭션에서 함수 내부로 들어가고, ni는 함수를 호출하는 인스트럭션에서 함수 내부
로 들어가지 않는다는 점 이다.
다음의 문장을 예로 들어보자.
printf("丄oop %d : ", i);

s 또는 n 명령의 입장에서 본다면 하나의 행이지만, 어셈블리 인스트럭션 수준에서 보
면 4개의 인스트럭션들로 구성된 문장이다. 즉, 위 문장은 s 또는 n 명령 한 번에 진행
이 되지만, si 또는 ni 명령을 사용한다면 4번 실행해야 한 문장이 진행된다.
요약하면 s 또는 n 명령은 진행 단위가 소스 프로그램 언어 수준에서의 한 문장을 대상
으로 하며, si 또는 ni 명 령은 소스 프로그램 언어 수준에서의 한 문장에 대응하는 어셈
블리 인스트럭션을 대상으로 한다는 차이점 이 있다.

448

4부—디버깅

===== PAGE 450 =====
［표 8-6］ 진행 명령 요약 2
U

현재 loop를 빠져 나감

finish

현재 함수를 수행하고 빠져 나감

return

현재 함수를 수행하지 않고 빠져 나감

r아 urn 123

현재 함수를 수행하지 않고 빠져 나감. 리턴 값은 123

si

현재의 인스트럭션을 수행, 함수 호출 시 함수 내부로 들어감

ni

현재의 인스트럭션을 수행. 함수 호출 시 함수 내부로 들어가지 않음

advance 20

현재 파일의 20라인을 만날 때까지 진행

advance file.c：20

file.c 파일의 20라인을 만날 때까지 진행

자주 사용하는 프로그램 수행 관련 명령은 이것이 전부다. 정말 간단하지 않은가?

s(step), n(next), c(continue), u(until), finish, return, si, ni 명령만 알고 있으면 얼
마든지 원하는 위치로 이동할 수 있다.

| 와치 포인트 설정
어떤 변수 값이 바뀔 때마다 브레이크를 걸려면 와치 포인트를 사용한다. 와치 포인트
는 변수 값이 어떻게 바뀌는지, 그리고 어떤 코드가 바뀌는지 확인할 때 편리하다. 와치
포인트는 다음과 같이 사용한다.
watch ［변수명］
rwatch ［변수명］
awatch ［변수명］

각각의 와치 포인터의 차이점은 그냥 watch는 변수의 값이 써질 때 브레이크가 걸리
고, rwatch 는 변수의 값이 읽혀질 때 브레이크가 걸리며, awatch는 읽거나 쓰거나 모
든 경우에 브레이크가' 걸린다는 점이다.
［그림 8-12］ 는 watch i 명 령으로 i 변수에 와치 포인트를 설정하고 i 변수의 값이 써질
때마다 브레이크가 걸리면서 i 변수의 이전 값과 현재 값을 출력하는 모습을 보여준다.

8장_gdb 디버거 ； 449

===== PAGE 451 =====
［그림 8-12］ i 변수에 와치 포인트 설정

［그림 8-12］ 에서 볼 수 있듯이 ［예제 8-1］ bugprg 프로그램의 i 변수에 와치 포인트를
설정하고 c(continue) 명령을 입력하니 i 변수의 값이 써질 때마다 브레이크가 걸리면
서 i 변수의 이전 값과 현재 값이 출력됨을 확인할 수 있다.
그리고 i 변수와 같은 지역변수에 와치 포인트를 설정하려면 프로그램 수행 context
가 해당 지역변수가 정의된 함수 내에 있을 때 와치 포인트를 설정해야 한다. 지역변수
는 해당 함수 내에서만 존재하므로 프로그램 수행 context?} 해당 함수 내에 있지 않
다면 i 변수의 위치를 찾을 수 없기 때문이다. 그래서 필자는 ［그림 8-12］ 의 실습에서

b main 으로 브레이크를 걸고 r 명 령으로 main 함수에 들어간 이후에 watch i 명령을
사용해 i 변수에 와치 포인트를 설정하였다.
이런 와치 포인트는 매우 자주 사용되는 명령 중 하나다. 그러므로 반드시 숙지하기 바
란다.

450 4부_ 디버깅

===== PAGE 452 =====
I 변수와 레지스터 값 검사
디버거를 사용하는 목적은 특정 시점에서의 메모리 값과 레지스터 값을 확인하기 위함
이다. 앞서 배운 내용으로 이제 특정한 시점으로 이동할 수 있게 되었을 거라고 생각한
다. 이제는 특정한 시점에서 변수 값과 레지스터 값을 어떻게 확인하는지 알아보자.
먼저 for문이 처음 시작되는 부분으로 이동하기 바란다. k 명령으로 이전에 수행하던

bugprg 프로그램을 종료한다. 필자의 경우 for 문이 28 행에 있기 때문에 b 28 명령으
로 브레이크포인트를 걸고 r 명령으로 프로그램을 실행한 후 main 함수에 이전 설정해
놓은 브레이크에서 브레이크가 걸려 다시 c 명령을 입력해 for문의 시작 부분으로 이
동했다. 각자 상황이 다를 수 있으니 이전에 배운 내용을 바탕으로 for문의 시작 부분
으로 잘 이동하기 바란다.
정상적으로 for문의 시작 부분으로 이동했다면 화면에 “for （ i=0； i〈 4； i++） {”와 같은

for문의 소스 라인이 출력될 것이다.

O 전체 변수의 값 출력
먼저 지역변수들에는 어떤 것이 있으며, 각각의 값은 무엇인지 알아보자. for문 위치에
서 info locals 명령을 입력하면 현재 상태에서의 지역변수와 각각의 값이 출력된다.

[그림 8-13] info locals 명령으로 지역변수의 종류와 값 출력

i 변수는 아직 값이 할당되지 않아 쓰레기 값이 들어 있고 Istr 변수는 “I like you.” 문자
열을 가리키고 있는 것을 확인할 수 있다. 그리고 pt 변수는 struct time 타입의 포인터
변수고, 또한 gtime 구조체를 가리키고 있기 때문에 gtime 구조체의 주소인 0x804858f
의 값을 가지고 있음을 확인할 수 있다.
이제 info variables 명령으로 전역변수에는 어떤 것들이 있는지 확인해 보자. info

variables을 내리면 전역변수 리스트들과 Non~debugging 심볼들이 출력된다.

8장_gdb 디버거 451

===== PAGE 453 =====
［그림 8-14］ info variables 명령어로 본 전역변수 리스트

Non-debugging 심볼들은 표준 C 라이브러리의 심볼들이기 때문에 신경 쓰지 말기
바란다.

@ 개별 변수의 값 출력

각각의 변수 값을 확인하려면 p(print) 명령을 사용한다. p ［변수명］ 명령을 내리면 해
당 변수 값이 출력된다. 그리고 P ［함수명］ 명령을 내리면 함수의 주소 값이 출력된다.

［그림 8-15］ p 명령으로 변수의 값 출력

@ 포인트 변수의 값 출력

포인트 변수인 pt 의 값 확인을 위해 p pt 명령을 내리면 어쩌면 당연하게도 pt가 가리
키고 있는 gtime 구조체의 주소 값만 출력된다. 실제 구조체의 내용을 보려면 p *pt와
같은 형식으로 명령을 내려야 한다.
이런 문법은 C 언어에서 포인트 타입 변수가 가리키는 실제 값을 의미하는 문법과 동
일하다. C 언어에서 어떤 포인트 타입 변수가 가리키는 실제 값을 보려면 * 기호를 붙
이듯이 P 명령에서도 변수명 앞에 * 기호를 붙인다. 이중 포인트라면 ** 기호를 붙인다.

452 4부-디버깅

===== PAGE 454 =====
... 상략

struct time *pt = &gtime;
struct time **ppt = &pt;
... 하략

[ 關 [screen 2： bash] root@os：/temp/book/debug
(gdb) p pt
$1 = (struct time *) 0x89494eq_________________
(gdb) p *pt
$2 = {hour = 1, min = 2, sec = 3}
|(gdb) p ppt
|$3 = (struct time **) 0xbFffd728
(gdb) p *ppt
1$4 = (struct time *) 0x80494e4
(gdb) p **ppt
$5 = {hour = 1, min = 2, sec = 3}
(gdb) |

［그림 8-16］ p 명령으로 포인트 변수의 값을 본 모습

［그림 8-16］ 에서 보듯이 포인트 변수가 가리키는 실체를 보려면 * 기호를 적절히 넣어
야 한다. pt 변수 값인 0x80494e4 의 값을 보려면 인다이렉트를 의미하는 *를 하나 붙
이고, ppt와 같이 더블 인다이렉트 변수 값을 보고자 한다면 * 기호를 두 번 붙인다.

S 레지스터의 값 출력
P 명령은 또한 레지스터의 값을 보는 데도 이용된다. ［그림 8-1 기에서 p $［레지스터명］
명령을 사용해 지정한 레지스터 값을 확인한 예를 볼 수 있을 것이다.

［그림 8-17］ p 명령으로 본 각 레지스터 값

이런 레지스터 값 전체를 한 번에 확인하는 명령은 info registers 명령이고, MMX 레
지스터를 포함해 거의 모든 레지스터 값을 확인하는 명령은 info all-registers 명령이
다. info registers 명령을 내리면 ［그림 8-18］ 과 같이 각 레지스터 값이 출력된다.

8장_gdb 디버거

453

===== PAGE 455 =====
［그림 8-18］ info registers 명령으로 각 레지스터의 값 출력

@ 포인트가 가리키는 구조체 배열을 출력

다음과 같이 포인트 변수가 힙에 생성된 구조체 배열을 가리키는 소스가 추가되었을
때 구조체 배열의 전체 내용을 확인하기 위해 *pt하면 당연하게도 하나의 구조체밖에
출력되지 않는다. gdb는 pt가 struct time 타입의 포인트 변수라는 것밖에 모르기 때문
이다.
...상략

pt = (struct time *)malloc(sizeof(struct time) 大 4);
• •• 하략

［그림 8-19］ 는 위 예제 코드가 있을 때 p *pt 명령으로 pt 변수가 가리키는 구조체 배
열을 출력한 예다. 보면 알겠지만 크기 4의 구조체 배열인데, 실제로는 하나의 구조체
밖에 출력되지 않는다.

［그림 8-19］ p *pt 명령으로 본 힙의 구조체 배열

이 럴 때는 별도로 gdb 에게 pt 변수가 가리키는 값이 배열임을 알려야 한다. gdb에게
배열의 크기를 알리고자 할 때는 @ 기호를 사용한다. p *pt@4 명령을 내리면 gdb 가

4 크기의 배열임을 알 수 있기 때문에 ［그림 8-2이과 같이 원하는 모습으로 출력된다.

454 4부_ 디버깅

===== PAGE 456 =====
HFH
=허 히

® [screen 2： bash] root@os：/temp./book/debug
(gdb) p *pt@4
$5 = {{hour = 0, min = 0, sec = 0}, {hour = 0, min
sec = 0}, {hour = 8, min
min = 0, sec = 0}}
(gdb) |

0}, {hour = 0,

［그림 8-20］ p *pt@4 명령으로 본 동적 할당된 구조체 배열

同 중복된 변수명이 있을 때 특정 변수를 지정해서 출력

p 명령으로 var 변수의 값을 확인하고자 하는데 전역변수 var과 지역변수 var이 동시
에 존재한다면 지 역변수가 사용된 함수 내에 있을 경우 지역변수 var의 값이 화면에 출
력된다. P 명령은 C 언어에서와 같이 변수의 이름이 중복될 경우 변수의 범위를 고려해
가장 적합한 변수를 선택해 출력한다. 가령 다음과 같이 두 개의 소스로 이뤄진 프로그
램이 있을 때 main 함수의 heUo 함수를 호출하는 부분에서 p var 명 령으로 var 변수
의 내용을 출력하면 main.c 파일에 있는 var 변수 값인 5000이 출력된다.
〔예제 8-3〕 변수명이 중복될 때 특정 변수를 지정해 줄력하는 예제

[[[ main.c ]]]

[[[ hello.c ]]]

int var = 2000;

#include <stdio.h>

void hello() ;
int main-()

void hello()
{
static int var = 6000;
printf ("hello, world!\n");

{
int var = 5000;
hello () ;
return 0;

<=== 현재 위치

H [screen 3： bash] root@os：/temp/book/debug/hello

(하?—
Starting program: /temp/book/debug/hello/hello
Breakpoint 1, main () at main.c:10
10
hello();
(gdb) p uar
$1 = 5000
(gdb) B

[그림 8-21] p var한 결과

이 상태에서 main.c 파일의 전역변수로 정의된 var 변수 값이나 hello 함수에 static으
로 정의된 var 변수 값을 확인하기 원한다면 ：： 기호를 사용해 ［그림 8-22］ 와 같이 p 명
령을 내려야 한다.

8장_ gdb 디버거 | 455

===== PAGE 457 =====
삐 [screen 3： bash] root@os：/temp/booK/debug/hello
(gdb) p 'main.c'::uar
$3 = 2000
(gdb) p hello::uar
$4 = 6000
(gdb) I

［그림 8-22］ p ‘main.c’：：var 명령과 p hello：：var 명령의 결과

특정 파일의 전역변수를 지정하고자 할 때는 P‘［파일명］’::［변수명］과 같이 따옴표를 파
일명에 붙이고, 특정 함수의 static 변수 값을 확인하고자 할 때는 p ［함수명］::［변수명］
과 같이 사용한다. 파일명인 경우 따옴표(‘)를 붙여야 한다는 것에 주의하기 바란다.

B 출력 형식의 지정
P 명령으로 변수 값이나 레지스터 값을 출력하면 기본적으로 10진수로 출력된다. 출력
형식을 10진수 외에 다른 형식으로 바꾸고자 할 때는 p/［출력 형식］ ［변수］ 형태로 명령
을 내린다. 가령 p Ival 명령을 내리면 Ival 변수 값을 10진수 형태로 출력한다. Ival 변수의
값을 16진수로 출력하고 싶다면 p/x Ival 명령을 사용한다. 여기서 x는 출력 형식을 16진
수로 하라는 의미다. 이 렇게 지정할 수 있는 출력 형식에는 다음과 같은 것들이 있다.

• t： 2진수로 출력
• o： 8진수로 출력
• d： 부호가 있는 10진수로 출력 (int)
• u： 부호가 없는 10진수로 출력 (unsigned int)
• x： 16진수로 출력
• c： 최초 1바이트 값을 문자형으로 출력
• f： 부동소수점 값 형식으로 출력
• a： 가장 가까운 심볼의 오프셋을 출력
위의 출력 형식 중 가장 자주 사용하는 것은 16진수로 출력하는 X다.

a의 의미가 모호할 거라는 생각이 든다. a의 의미는 다음과 같다. p/a 0x8048000 명령
을 내리면 0x8048000 위치에서 가장 가까운 심볼과의 오프셋을 출력한다.
［그림 8-23］ 에 보면 p/a 0x804842d 명령을 내렸을 때 출력되는 값이〈main+40〉인데,
이 말은 0x804842d 위치에서 가장 가까운 심볼은 main 함수이고, 0x804842d의 위치
는 main 함수에서 40바이트만큼 떨어져 있다는 의미다.

456 4부_ 디버깅

===== PAGE 458 =====
［그림 8-23］ 여러 출력 형식으로 출력

同 타입이 다를 경우 타입을 변환해 출력

가령 다음과 같은 소스 코드가 있을 때 p vstr 명령을 내리면 gdb 는 vstr 변수의 타입
을 void *로 인식하기 때문에 vstr 변수에 있는 주소 값만을 출력한다.
• • • 상략

void Wstr = (void *)"I like you. ";
... 하략

이전에 p Istr 명 령을 내려 Istr 변수의 내용을 보았을 때는 주소 값과 해당 주소가 가리
키는 문자열도 같이 출력되었는데, void *vsti•은 그렇지 않다. 이유는 -g 옵션을 주어
컴파일할 때 추가된 디버깅 정보에 vstr 변수의 타입이 void * 타입으로 지정되어 있기
때문이다 이렇게 타입이 다른 포인트 변수의 내용을 보고자 한다면 타입에 대한 정보
를 gdb에 임의로지정한다.

gdb 에게 변수의 타입이 무엇이라고 알리는 방법은 바로 C 언어에서 사용하는 타입
변환 문법과 동일하다. 타입 변환 문법을 사용해 p (char *)vstr 명령을 내리면 ［그림

8-24］ 와 같이 vstr 변수의 값이 우리가 원하는 문자열 형식으로 출력된다.
® [screen 2： bash] root@os ：/temp/book/debug
(gdb) p Istr

立 = 흐으쁘씌브 "I 끄쓰 you."
(gdb) p ustr
$8 = (uoid *) 0x80484ba
(gdb) p (char *)ustr
$9 = 0x80484ba "I like you."
(gdb) |

［그림 8-241 타입을 변환해 출력

s 특정 위치 지정
C 언어에서 타입 변환이 되듯이 gdb 는 C 언어의 문법대로 특정 위치를 지정할 수도
있다. 가령 p Istr + 4를 하면 “I like you.”문자열에서 4바이트 떨어진 위치의 문자열부
터 출력한다. 그래서 “ke you.”가 출력된다. 역시 p (array［ l］ + 1) 명령과 같이 배열에
대한 특정 문자열 지정도 가능하다.

8장_ gdb 디버거 457

===== PAGE 459 =====
［그림 8-25］ C 언어 문법을 사용해 특정한 위치 지정

E 변수 값 설정
이상이 P 명령을 사용해 변수 값을 확인하는 방법이다. P 명령은 변수 값을 확인하는
일 외에도 변수 값을 설정하는 마법과 같은 기능도 가지고 있다. 가령 다음과 같은 명
령을 내리면 Ival 변수 값이 1000으로 설정된다.
p Ival = 1000

［그림 8-26］ p 명령으로 변수 값 설정

이런 형식의 명령은 특정 변수의 값을 다르게 설정해 테스트할 때 유용하다. 지금까지
변수 값을 출력하는 방법을 알아보았는데, 여러 특수 상황을 일일이 설명하다 보니 갑
자기 gdb가 어렵게 느껴졌을지도 모르겠다. 여러 설명이 있었지만 결론은 하나다.
변수 값을 출력하려면 P 명령을 사용한다.
이것만 기억하면 된다.
［표 8-7］ 출력 명령 요약
P ［변수명］

변수 값을 출력

P ［함수명］

함수의 주소를 출력

P/［출력 형식］ ［변수명］

변수 값을 출력 형식으로 출력

P ‘［파일명］’::［변수명］

파일명에 있는 전역변수의 값을 출력

P ［함수명］::［변수명］

함수에 있는 변수 값을 출력

P ［변수명］@［배열 크기］ 변수의 내용을 변수 배열의 크기 형태로 출력

458 4부_ 디버깅

===== PAGE 460 =====
이제 변수 값도 확인할 수 있게 되었다. 지금까지의 내용만으로도 gdb 로 디버깅하는
데 아무런 문제가 없다. 프로그램을 실행시키는 방법, 브레이크포인트를 설정하는 방
법, 변수와 레지스터의 값을 확인하는 방법만 확실하게 알면 사용하는 데 조금은 불편
하겠지만 디버깅하는 데는 아무런 지장이 없다. 지금부터 설명할 내용은 알아 두면 좋
은 내용들인데, gdb 가 정말 강력하다는 것을 알려면 기본적인 것 외에 나머지 기능도
잘 알아야 한다.

W 화면에 변수의 값을 자동으로 디스플레이하기

s 명령으로 한 행씩 진행하면서 p 명령으로 매번 변수 값이 변경되었는지를 확인하면
서 디버깅한다면 무척이나 피곤할 것이다. 요즘 같이 모든 사물에 인체 공학이 적용되
고 있는 시대에 gdb 가 인간을 위한 최소한의 배려를 하지 않았다면 gdb 는 아마도 몇
몇 특이한 성격의 소유자만의 전유물이 되었을 것이다. 계속 변수 값이 변하는 것을 확
인하고자 할 경우 display 명령을 사용하면 s 명령으로 진행하면서 변하는 변수 값을
확인할 수 있다.

[그림 8-27] display gtime.hour 명령을 사용한 예

［그림 8-2刀과 같이 display gtime.hour 명령을 내리면 s 명령으로 한 행씩 진행할 때
마다 gtime.hour 변수 값을 화면에 디스플레이한다. 이런 display 명령은 지역변수를
디스플레이하는데, 함수가 바뀌어 변수의 범위를 벗어나면 해당 변수를 디스플레이하
지 않는다. 가령 Ival 변수 같이 main 함수의 지역변수인 경우 main 함수를 벗어나면

gdb는 Ival 변수를 디스플레이하지 않는다.
디스플레이를 해제하려면 undisplay 명령을 사용한다. 가령 gtime.hour 변수는 1번 디
스플레이인데, 그것은 gtime.hour 변수가 출력되는 앞부분의 숫자를 보면 된다. gtime.

hour 변수가 더 이상 디스플레이되지 않기 원한다면 다음 명령으로 디스플레이를 해
제한다.

8장_ gdb 디버거 | 459

===== PAGE 461 =====
undisplay 1

여기서 1 은 gtime.hour 변수의 디스플레이 번호다. display 명령 역시 p 명령과 마찬
가지로 출력 형식을지정할수 있다. display/x g time .hour 명령을 내리면 gtimehour
변수 값을 16진수 형식으로 매번 디스플레이한다. 이런 출력 형식은 p 명령에서 사용
하는 x, o, t, •••와 동일하다.

• t： 2진수로 출력
• o： 8진수로 출력
• d： 부호가 있는 10진수로 출력 (int)
• u： 부호가 없는 10진수로 출력 (unsigned int)
• x： 16진수로 출력
• c： 최초 1바이트 값을 문자형으로 출력
• f： 부동소수점 값 형식으로 출력
• a： 가장 가까운 심볼의 오프셋을 출력
또한 disable display ［디스플레이 번히 명령으로 디스플레이되는 것을 일시적으로
비활성화시킬 수도 있다. 이렇게 일시적으로 비활성화된 디스플레이는 enable display
［디스플레이 번히 명령으로 다시 활성화시킬 수 있다.
［표 8-8］ 디스플레이 관련 명령 요약
display ［변수명］

변수 값을 매번 화면에 디스플레이한다.

display/［출력 형식］ ［변수명］

변수 값을 출력 형식으로 디스플레이한다.

undisplay ［디스플레이 번히

디스플레이 설정을 없앤다，

disable display ［디스플레이 번히

디스플레이를 비활성화시킨다 .

enable display ［디스플레이 번히

디스플레이를 활성화시 킨다.

자, 이제 변수 값을 보는 법도 익혔고 디스플레이하는 법도 익혔으니 그럼 다시 디버깅
하던 bugprg 프로그램으로 돌아가 디버깅하던 것을 마저 해 보자. 먼저 main 함수의

for문 부분에 브레이크포인트를 걸고 r 명 령으로 실행시킨다.
b 28

460 4부_ 디버깅

# 필자의 경우 28행에서 for문이 시작된다.

===== PAGE 462 =====
그리고 i 변수, func 함수의 인자로 넘어가는 arrayti] 값, for 문이 한 번 수행될 때마
다 변경되는 gtimehour 변수 값을 알아보기 위해 다음 명령으로 각각을 디스플레이
시킨다.
display i
display array[i]
display gtime.hour

[그림 8-28] 디버깅 시 값의 변화를 확인할 변수 지정

display array[i] 명령을 내렸을 때 [그림 8-28] 에 표시된 것처럼 오류 메시지가 나타
날지도 모른다. 현재 i 의 값이 초기화되어 있지 않아 의 값에 쓰레기 값이 들어 있어

array 범위를 벗어났기 때문이다. 이럴 때는 [그림 8-28] 에서와 같이 p i = 0 명령으로
i 값을 0으로 초기화시킨 후 display array[i] 명 령을 다시 내리기 바란다.
이제 s 명령으로 한 행씩 수행하면서 프로그램의 수행 과정을 추적해 보자. s 명령으로
한 행씩 진행하다 보면 그림과 같이 func 함수 내부로 들어간다. func 함수 내부에 들
어왔으면 이제 스택 관련 명령을 한번 테스트해 보자.

【그림 8-29] func 함수 내부에 들어온 모습

8장_gdb 디버거 : 461

===== PAGE 463 =====
I 스택의 상태 검사
［그림 8-29］ 와 같은 상황에서 info f 또는 info frame 명령을 내리면 다음과 같은 결과
가 출력될 것이다.
，:" root@os：/temp/gdb
(gdb) inFo Frane
Stack leuel 8, Frame at 8xbFe64250:
eip = 0x80483b1 in Func (bugprg.c:14); saved eip 0x894845c
called by Frane at OxbFe64280
source language c.
Arglist at 0xbfe64248, args: sw=0, str=8x8048550 "one"
Locals at OxbFe64248, Preuious frame's sp is 0xbFe64250
Saved registers:
ebp at OxbFe64248, eip at 0xbfe6424c
(gdb) |

■-1(꿔，시

. Hid

버
［그림 8-30］ info frame 명령으로 func 함수의 스택 프레임 정보를 출력

info frame 명령은 현재 함수의 스택 프레임에 있는 내용을 확인하는 명령이다. 아직은
위 메시지가 암호(?) 같겠지만 조금만 알고 나면 위 메시지가 디버깅을 위해 얼마나 중
요한지 알 수 있다.

n 스택은 어떻게 잡히나
스택 프레임을 설명하기 전에 먼저 스택이 무엇인가 알아보자. 스택이 무엇인지 모르는
독자는 없을 것이다. 스택을 간단하게 설명하면 함수의 호출 시 함수의 지역변수나 함
수 호출 정보가 저장되는 메모리 공간을 말한다.
〔예제 8-4)

스택을 위한 예제

int add(int nz int m)
int r;
r = n + m;
return r;
}

［예제 8-4］ 에서 인자로 넘어가는 n과 m, 그리고 지 역변수인 r이 할당되는 공간이 바로
스택이다. 스택은 이런 지역변수 외에도 함수가 호출될 때 함수 호출이 끝나고 다시 복
귀할 주소인 리턴 어드레스도 저장하고, 함수 호출과 관련된 레지스터(ebp)도 저장한
다. 리눅스에서 동작하는 모든 프로세스는 실행될 때 다음과 같은 가상 주소 공간을 할
당받는데, 이 중에 스택의 공간이 잡혀있다.

462 4부_ 디버깅

===== PAGE 464 =====
모든 프로세스는 실행될 때 위와 같은 4기가바이트의 가상 주소 공간을 가진다. 4기가
바이트란 말에 의아해 하는 독자가 있을 거라고 생각한다. 보통의 PC는 그보다 작은

1기가바이트나 2기가바이트의 메모리를 가지고 있기 때문이다. 실제로 거의 대부분의
PC는 4기가바이트 이하의 메모리를 가지고 있다. 그러나 페이징 기법에 의해 마치 4기
가바이트의 메모리가 있는 것처럼 동작할 수 있다.

4기가바이트의 주소 공간에서 사용되는 주소를 실제 물리 메모리인 페이지 프레임과
맵핑시키는 것은 전적으로 운영체제의 몫이다. 애플리케이션은 그에 대해 아무런 신경
을 쓰지 않고 그냥 4기가바이트가 있다고 생각하고 사용한다. ［그림 8-31］ 에서 보듯이

0x00 ~ Oxbfffffff까지 하위 3기가바이트 주소 공간이 바로 프로세스가 사용하는 주소
공간이고, OxCOOOOOOO ~ Oxffffffff까지 상위 1기가바이트 주소 공간이 바로 커널이 사
용하는 주소 공간이다.

8장_gdb 디버거 463

===== PAGE 465 =====
그리고 ［그림 8-31］ 에서 보듯이 공유 라이브러리의 시작 주소는 하위 1기가바이트
이후인 0x40000000 부터 시작되는 것을 알 수 있고, 사용자 스택은 동그라미가 쳐진

Oxbfffffff부터 하향 성장하는 것을 알 수 있다.
여기서 하향 성장한다는 말은 i386 계열 CPU에서 스택에 데이터를 저장하면 스택 top
을 가리키는 레지스터(esp)의 주소가 줄어들면서 스택 공간이 늘어난다는 의미다. 즉,
［그림 8-31］ 에서 스택은 화살표 방향으로 성장하는데, 화살표가 0x00번지를 향해 아
래로 성장하는 것을 알 수 있다. ［그림 8-31］ 을 애써 이해할 필요는 없다. 단지 프로세
스의 스택이 Oxbfffffff 주소부터 아래로 늘어난다는 점만 알면 된다.

@ 함수 호출 과정과 스택 프레임

이런 스택은 push, pop 혹은 mov 인스트럭션이 사용되거나 아니면 함수가 호출될 때
사용된다. ［예제 8-5］ 와 같은 소스 프로그램이 있을 때 main 함수에서 add 함수를 호
출하면 다음과 같은 일이 일어난다.
〔예제 8-5〕 add.c 예제 소스

int add(int n, int m)
{
int r;
r = n + m;
return r;
}
int main()
{
int k;
k = add(1, 3);
return 0;
}

이해를 돕기 위해 위 소스를 gcc -o add add.c -save-temps 명령으로 컴파일해 생
성되는 어셈블리 코드로 설명하겠다. ［예제 8-5］ 를 컴파일하면 ［예제 8-6］ 과 같은 어
셈블리 파일이 생성된다. 주의할 것은 컴파일러 버전에 따라 출력되는 어셈블리 파일의
내용이 다르다는 점이다. ［예제 8-6］ 은 gcc-3.2.2 버전으로 컴파일했을 때 결과다. 어
셈블리 파일의 결과가 다르게 나왔더라도 당황하지 말기 바란다. 여기서는 결과 확인이

464 4부— 디버깅

===== PAGE 466 =====
중요한 것이 아니라 어떤 식으로 함수가 호출되는지 이해하는 것이 더 중요하기 때문
이다. 그리고 내용이 조금 다를지라도 하는 일은 거의 동일하다.
〔예제 8-6〕 컴파일된 어셈블리 파일

.file "add. c’’
. text
.globl add
.type add,^function
add:
pushl
movl
subl
movl
addl
movl
movl
leave
ret

% ebp ......................................................................................................... 4
%esp, %ebp ............................................................................................... 5
$4, %esp .................................................................................................... 6
12 (%ebp), %eax
8 (%ebp), %eax
응eax, -4(%ebp)
-4(%ebp), %eax

.Lfel:
. size add,.Lfel-add
.globl main
.type

main,@function

main:
pushl
movl
subl
andl
movl
subl
subl
pushl
pushl

%ebp
%esp, %ebp
$8, %esp
$-16, %esp
$0, %eax
응eax, 응esp
$8, %esp
$3 ............................................................................................................... 1
$1 ............................................................................................................... 2

call
addl
movl
movl
leave
ret

add ............................................................................................................. 3
$16z %esp
%eax, -4 (%ebp)
$0, %eax

.Lfe2:
. size
main, .I」fe2-main
.ident "GCC: (GNU) 3.2.2 20030222 (Red Hat Linux 3.2.2-5)"

먼저 add 함수가 호출되기 전 스택의 상태는 ［그림 8-32］ 와 같다.

8장—gdb 디버거

465

===== PAGE 467 =====
［그림 8-32］ add 함수가 호출되기 전 스택의 상태

esp 레지스터가 현재 스택의 top을 가리키고 main 함수의 지역 변수 k가 스택에 할당된
모습이다. ［예제 8-6］ 에서 pushl $3 인스트럭션을 수행하면 C 소스의 k = add(l, 3)；에
서 add 함수의 m 인자로 넘어갈 3이 스택에 push된다. 그러면 ［그림 8-33］ 과 같은 형
태가 된다.

그리고 pushl $1을 수행하면 add 함수의 n 인자로 넘어갈 1 이 스택에 push된다.

466 4부_ 디버깅

===== PAGE 468 =====
그리고 call add 인스트럭션에 의해 현재의 스택에 리턴 어드레스인 eip 레지스터의 값
이 저장된다.
다음으로 add 함수가 수행되기 시작한다. eip 레지스터에는 다음에 수행할 인스트럭션
주소가 들어 있는데, call add 인스트럭션 바로 밑에 있는 addl $16, %esp 인스트럭션
의 메모리 주소가 들어 있다.
이렇게 스택에 저장된 eip 레지스터의 값은 add 함수가 끝날 때 add 함수의 제일 아래
에 있는 ret 인스트럭션에 의해 main 함수로 다시 돌아올 때 이용된다.

이제 add 함수가 수행되는데, add 함수의 시작 부분（ 4로 표시된 부분）에 있는 pushl

%ebp 인스트럭션에 의해 현재 ebp 레지스터의 값이 스택에 저장된다.

8장_gdb 디버거 467

===== PAGE 469 =====
ebp 레지스터를 현재의 스택에 저장했다면 esp 레지스터의 값을 ebp 레지스터에 넣
는다. 결국 ebp 레지스터와 esp 레지스터의 값은 같은 주소를 가진다.

ebp 레지스터는 베이스 레지스터라 부르고 함수 내에서 변하지 않기 때문에 지역변수
와 인자에 접근할 때 기준으로 사용된다. 예를 들면 add 함수 내에서 인자인 n 변수로
접근하고자 할 때는 8(%ebp)와 같은 형식으로 접근하고, m 변수는 12(%ebp), 그리고
지역변수인 r 변수는 -4(%ebp) 와 같은 형식으로 접근한다. esp 레지스터는 스택에 값
을 push 하거나 pop 할 때 기준이 되는 레지스터로서 스택 top 이 라 하고 push, pop 할
때마다 변한다.

ebp 레지스터를 스택에 저장하고 esp 레지스터의 값을 ebp 레지스터에 넣는 과정을 프
롤로그 과정이라 하고, 함수가 호출될 때 항상 함수의 시작 부분에서 일어나는 일이다.

468 4부_ 디버깅

===== PAGE 470 =====
프롤로그 과정이 끝났으면 이제 esp 레지스터에 4를 빼서 add 함수에서 사용할 지역
변수인 r의 공간을 할당한다. 그러면 최종적으로 스택은 다음과 같은 모양이 된다.

여기가 중요하다. ［그림 8-38］ 에 보이는 main 함수의 스택과 add 함수의 스택을 main
함수의 스택 프레임, add 함수의 스택 프레임 이라고 부른다.

@ 스택 프레임에 있는 정보를 이용해 디버깅

앞에서 info frame 명 령으로 func 함수의 스택 프레임을 보았다.
• root@os：/temp/gdb
(gdb) inFo Frane
Stack leuel 0, Frame at 0xbfe64250:
_______
eip = 0x80483b1 in Func (bugprg.c:14)
saued
called by Frame at 0xbfe64280
source language c. _________________________________________
Arglist at 8xbfe64248, | args:
Locals at 0xbFe64248, PreuiousFrame's sp is 0xbFe6425O
Saved registers:
ebp at 0xbFe64248, eip at 0xbFe6424c
(gdb) |

;「

"one"!

［그림 8-39］ info frame 명령으로 func 함수의 스택 프레임 정보를 출력

이런 스택 프레임이 디버깅에서 중요한 이유는 바로 해당 함수를 호출할 때 사용한 함
수의 인자와 함께 리턴 어드레스가 들어 있기 때문이다. 그래서 함수의 인자 값을 읽어
봄으로써 함수가 제대로 호출되었는지 확인할 수 있고, 리턴 어드레스를 읽어봄으로써
어떤 함수의 어떤 부분에서 해당 함수를 호출했는지 알 수 있다.
［그림 8-39］ 에서 표시되어 있는 부분은 어떤 부분에서 func 함수를 호출했는지, func
함수가 호출될 때 인자로 넘어간 값들이 어떤 것들이었는지 보여준다.

8장_ gdb 디버거

469

===== PAGE 471 =====
특정 함수가 이유 없이 종료됐을 때 info frame 명령으로 스택 프레임을 읽어보면 함
수가 호출될 때 어떤 인자 값으로 호출되었으며 어떤 함수의 어떤 부분에서 호출했는
지 바로 알 수 있기 때문에 이상 유무를 쉽게 찾을 수 있다. func 함수에서 bt 명 령으로
백트레이스해 보면 전체 스택 프레임을 볼 수 있는데, 다음과 같다.

［그림 8-40］ bt 명령으로 본 전체 스택 프레임

［그림 8-40］ 은 두 개의 스택 프레임을 보이는데, 호출된 순서대로 main 함수의 스택
프레임과 func 함수의 스택 프레임을 각각 확인할 수 있다. 내용을 자세히 살펴보면 함
수가 호출될 때 인자와 caller 함수의 어떤 라인에서 callee 함수를 호출했는지 라인 정
보도 확인 가능할 것이다.

func 함수의 경우 main 함수 내 bugprg.c 파일의 30 행에서 호출되었고, 인자로 0 과
문자열 “one”의 주소인 0x8048550을 사용해 호출되었음을 확인할 수 있다.

frame 명령을 사용하면 스택 프레임 간에 전환도 가능하다. 기본적으로 info frame 명
령을 내리면 현재 함수（ func 함수）의 스택 프레임 정보를 보이는데, frame 1 명령을 내
린 후 info frame 명령을 내리면 ［그림 8-4이에서 1로 표시되어 있는 main 함수의 스
택 프레임 내용을 출력한다.
root@os:/temp/gdb
(gdb)|frame 1 ]
#1
0x8804845c in main () at bugprg.c:30
30
gtime.hour += func(i % 2, array[i]);
(gdb) |'i"n司히
Stack leuel 1, frame at 0xbfe64288:
eip = 8x804845c infmain |(bugprg.c:30); saued eip 0x423a2F78
caller of Frame at 8xbFe64250
source language c.
Arglist at 8xbFe64278, args:
Locals at 0xbfe64278, Preuious frame's sp at 0xbFe6426c
Saued registers:
ebx at 0xbFe64270, ebp at 0xbFe64278, esi at 0xbFe64274,
eip at 8xbFe6427c
(gdb) |

［그림 8-41］ frame 명령으로 스택 프레임 전환

스택 프레임 정보에는 위와 같이 함수가 어디에서 호출되었고 호출될 때 인자가 무엇
이며 지역변수는 어떤 것이 할당되었는지에 대한 정보가 나와 있어 디버깅할 때 유용

470 4부—디버깅

===== PAGE 472 =====
하게 사용할 수 있다. 스택 프레임에 관련된 명령은 다음과 같은 것들이 있다. 스택 프레
임 명령들은 거의 모두 자주 사용되는 명령들이니 잘 기억해 두기 바란다.
［표 8-9］ 스택 프레임 관련 명령 요약
frame [N]

n번 스택 프레임으로 변경

up

상위 스택 프레임으로 이동

up [N]

n번 상위 스택 프레임으로 이동

down

하위 스택 프레임으로 이동

down [N]

n번 하위 스택 프레임으로 이동

info frame

스택 프레임 정보를 출력

info args

함수가 호출될 때 인자를 출력

info locals

함수의 지역변수를 출력

info catch

함수의 예외 핸들러를 출력

보통 프로그램이 이상 종료하면 스택이 깨지지 않은 이상 스택 프레임은 종료될 당시
상태를 유지한다. 그래서 bt 명령으로 스택을 백트레이스해 어떤 함수 호출에서 종료했
는지 확인하고 info frame 명령으로 인자 값을 확인한 후 디버깅한다.
그럼 한번 실습해 보자. 지금까지 잘 따라왔으면 bugprg 프로그램의 func 함수에서
수행이 멈춰 있을 것이다. c(continue) 명령을 내려 계속 수행시키면 세그먼트 폴트
가 발생해 프로세스가 SIGSEGV 시그널을 받고 다음과 같이 중지할 것이다.

［그림 8-42］ SIGSEGV 시그널을 받아 중지된 모습

위와 같은 상황에서 bt 명령으로 전체 스택 프레임을 보면 ［그림 8-43］ 과 같다.

［그림 8-43］

bt 명령으로 전체 스택 프레임을 본 모습
8장_gdb 디버거 471

===== PAGE 473 =====
main 함수의 30행에서 func 함수를 호출하였는데, 인자로 1과 0x0을 가지고 호출한
것을 확인할 수 있다. 그러면 도대체 어떤 이유로 func 함수에 str 인자로 0x0이 들어
갔는지 알아보기 위해 frame 1 명령으로 스택 프레임을 main 함수의 스택 프레임으로
변경해 보자.

[그림 8-44] main 함수의 스택 프레임으로 변경

main 함수의 스택 프레임으로 변경되면 func 함수가 호출될 당시의 소스를 출력한다.
func 함수는 i % 2라는 인자와 array[i]라는 인자로 호출되었다. 그러면 p 명령으로 각
각의 인자가 어떤 값을 가지는지 알아보자.

[그림 8-45] 변수 값 확인

p 명령으로 i 변수의 값을 확인해 보니 3이라는 값이 나왔다. 그리고 array[i]의 값은
0x0 값이 나왔다. array 배열의 값을 p array 명 령-0-루 확인해 보면 array는 4개의 엔
트리만 가지는 문자열 배열임을 확인할 수 있다. 그런데 배열의 마지막 값이 0x0으로
되어 있는 것을확인할 수 있다.

1 array 명령을 내리면 C 소스 내에서 array[] 배열이 정의되어 있는 부분이 출력된다.

[그림 8-46] I array 명령으로 array[] 배열의 정의 부분 출력

472 4부-디버깅

===== PAGE 474 =====
어랏, 그런데 array 배열의 정의되어 있는 부분을 보니 배열의 크기는 4로 잡혀 있지만
초기 값은 최초 3개만 잡혀 있고 나머지 하나는 초기 화되지 않았다.
이제야 모든 의문이 밝혀졌다. func 함수에서 세그먼트 폴트가 발생한 이유는 array 배
열이 완전히 초기화되지 않았기 때문이다. 때문에 array 배열 정의 부분을 다음과 같이
바꾸면 bugprg 프로그램은 이상 없이 잘 동작할 것이다.
char *array［ 4］ = {"one", "two", "three", "four"};

어떤가 gdb 로 디버깅하는 일이 무척 재미있고 쉽지 않은가? 지금까지 간단한 버그가
발생하는 프로그램을 gdb로 어떻게 디버깅하는지 알아보았다. 다음으로 메모리 상태
를 보는 방법을 알아보자.

I 메모리 상태 검사
디버깅을 하다 보면 변수 값을 확인하는 일 외에 메모리의 특정 범위에 있는 값들을 확
인하고 싶을 때도 있다. 혹은 특정 범위의 인스트럭션들이 어떻게 이뤄졌는지 확인하고
싶을 때도 있다. 그런 경우 x 명 령으로 확인할 수 있다.

x main 명령을 내리면 main 함수의 .주소에서 4바이트를 읽어 화면에 출력한다. 그리
고 x 0x8048200 명령을 내리면 0x8048200번지에 있는 4바이트를 읽어 화면에 출력한
다. x 명 령은 이 렇게 단독으로 사용할 수도 있지만 일반적으로 x 명령을 사용하는 규칙
에 따라 사용한다. x 명령의 규칙은 다음과 같다.
x/ ［범위］ ［출력 형식］ ［범위의 단위］

범위는 출력할 개수를 의미한다. 가령 x/10 main 명령을 내리면 main 함수 시작부터

40바이트를 출력한다. 출력 형식 부분은 기본적으로 p 명령을 사용할 때 사용되는 출
력 형식에 s(문자열 형식)와 i(인스트럭션 형식) 형식이 추가됐다. 그래서 x 명령을 사
용할 때 지정할 수 있는 형식에는 다음과 같은 것들이 있다.

• t： 2진수로 출력
• o： 8진수로 출력
• d： 부호가 있는 10진수로 출력 (int)
• u： 부호가 없는 10진수로 출력 (unsigned int)
• x： 16진수로 출력

8장_ gdb 디버거

===== PAGE 475 =====
• C： 최초 1 바이트 값을 문자형으로 출력
• f: 부동소수점 형식으로 출력
• a： 가장 가까운 심볼의 오프셋을 출력
• s： 문자열로 출력
•

i： 어셈블리 형식으로 출력

x/10i main 명령을 내리면 ［그림 8-4刀과 같이 main 함수의 시작부터 인스트럭션을
어셈블리로 변환해 보여준다.
-I미 시

root@os :/temp/gdb
(gdb) x/18i main
<nain>:
0x80483e6
<inain+U>:
0x86483ea
<nain+7>:
0x80483ed
0X8O483FO < m a i n + 1 0 >
<main+11>
0X80483F1
<main+13>
0X80483F3
<main+14>
0X8O483F4
<main+15>
0X80483F5
<main+16>
0x80483f6
<main+19>
8x80483f9
(gdb) |

lea
0x4(헝esp),허ecx
and
$0xFfffffF0,^esp
pushl OxFFFFfFFc(허ecx)
push %ebp
mou
혀esp,%ebp
push
黑esi
push
허ebx
push %ecx
sub
$0x1c,허esp
moul $0x91b,0xFFFFFfe4(%ebp)

［그림 8—47］ x/10i main 명령을 내린 모습

범위 단위는 범위를 지정할 때 사용될 단위를 의미한다. 기본적으로 word(4바이트)
단위이고, 다음과 같은 것들이 있다.

•

b： 1바이트단위 (byte)

• h： 2바이트 단위 (halfword)
• w： 4바이트 단위 (word)
• g： 8바이트 단위 (giant word)
x/10b 0x8048200 명령을 내리면 ［그림 4-48］ 과 같이 0x8048200번지를 시작으로 10바
이트를 출력한다.

[그림 4-48] x/10b 0x8048200 명령을 내린 모습

474 디버깅

===== PAGE 476 =====
이렇게 메모리를 직접 읽어보는 일은 -g 옵션을 가지고 컴파일되지 않은 실행 파일을
디버깅하고자 할 때 많이 사용된다. 소스는 없고 실행 파일만 있는데, 실행 파일이 어떻
게 동작하는지 알고 싶거나 실행에 문제가 발생했을 경우 X 명령을 사용한다.
소스가 없기 때문에 -g 옵션을 주고 다시 컴파일하는 것은 불가능하고, 어쩔 수 없이
역어셈블해 어셈블리 코드로 디버깅할 수밖에 없다. 어셈블리 코드로 디버깅하는 데 어
셈블리 코드의 모든 심볼은 이미 주소로 변경되어 버렸다. 물론 그 주소가 어떤 타입을
의미하는지도 모른다. 결국 각각의 주소를 확인하려면 X 명령을 사용해 메모리를 직접
읽어보는 수밖에 없다.

I 기타 유용한명령
다음은 gdb에서 사용할 수 있는 기타 유용한 명령들을 소개한다.

o 어셈블리 코드 보기
어셈블리 코드를 보려면 x/i 명령보다는 disas 명령이 더 일반적이다. 함수의 어셈블리
코드를 보고자 할 때 x 명령은 함수의 범위를 정확하게 지정해야 하는 반면에 disas 명
령은 함수의 이름만 주면 되기 때문이다. disas 명령은 어셈블리 코드로 디버깅할 때
많이 사용한다.
disas func

disas func 명령은 func 함수의 어셈블리 코드를 보여준다.
disas 0x8048300 0x8048400

위 명령은 주소 범위 사이의 어셈블리 코드를 보여준다.
root@os：/temp/gdb
(gdb)|disas main |
Dump of assembler code For Function main:
lea
0x4(%esp)，후ecx
0x080483e6
<nain+0>:
$8xFFfffff8,%esp
and
0x080483ea
<main+4>:
pushl
0xFFFFFFFc(%ecx)
0x080483ed
<nain+7>:
%ebp
Ox080483FO
<nain+10>:
push
%esp,%ebp
mou
0X08O483F1
<main+11>:
push
허 esi
0xO8O483f3
<main+13>:
허 ebx
0XO8O483F4
<nain+14>:
push
%ecx
0x080483F5
<nain+15>：
push
흐0x1c,훟esp
sub
0X080483F6
<main+16>：
$0x91b,0xfFFfFFe4(%ebp)
noul
0x080483f9
<nain+19>:
moul
$0X8048574,0xFfFFFFec(%ebp)
0x08048400
<main+26>:
추0X88496Fc,0xfFFFFFF0(%ebp)
0x08048407
<nain+33>:
moul
《0x0,0xfFFfFFe8(%ebp)
9x0804840e <nain+40>：
moul
|——Type <return> to continue.
or q <return> to quit-------------------------

[그림 8-49] disas main 명령 사용

8장_ gdb 디버거 475

===== PAGE 477 =====
@ call 명령을 사용한 함수별 모듈 테스트
caU 명령을 사용하면 함수를 임의대로 호출할 수 있다. 물론 이때 매개변수도 마음대로
줄 수 있다. 그래서 call 명령을 함수별 모듈 테스트에 사용한다. 매개변수를 달리한 후
함수에서 리턴되는 값이나 변수 값들의 변화를 판단해 함수가 제대로 동작하는지 알아
볼 때 매우 유용하다. ［예제 8-기로 알아보자.
〔예제 8-7〕 func.c 예제 코드

int
var;
int func(int n)

；

{
}

i

var += n;
return 99;

；

|

int main()

；

{

::
int i = 100; <====== 현재 위치
while (i--)

}
}

return

{
func (i);
0;

；
：

i
；
i

［예제 8-기과 같은 소스가 있을 때 main 함수에 브레이크를 걸어 call func(lOO) 명령
을 내리면 func 함수가 수행되면서 var 값에 100 씩 더해지고 func 함수에서 리턴되는
값인 99를 출력한다.

［그림 8-50］ call 명령으로 특정 함수를 임의로 호출

476 4부—디버깅

===== PAGE 478 =====
call과 비슷한 명령으로 jump 명령이 있는데, jump 명령은 임의의 행, 주소 또는 함수
로 무조건 분기하는 명령이다. jump *0x08048321 명령은 0x08048321 주소로 무조건
분기해 인스트럭션을 계속 수행한다. 그리고 jump 10 명령은 10행으로 무조건 분기해
수행한다. 마지막-0-루 jump func 명령은 func 함수로 무조건 분기해 수행한다.

@ 디버깅하는 프로세스에 시그널 보내기

signal 명령을 사용하면 디버깅 대상의 프로세스에 시그널을 보낼 수 있다. 보낼 수 있
는 시그널의 종류는 info signals 명 령으로 확인할 수 있다.
signal SIGKILL

위 명령을 내리면 실행 중이던 프로세스가 kill signal을 받아 종료한다. 그래서 ［그림

8-51］ 과 같이 c 명령이 동작하지 않게 된다. 이미 종료되었기 때문이다.

［그림 8-51］ signal 명령으로 signal을 보낸 모습

Q 메모리 특정 영역에 값을 설정
P 명령을 사용해 메모리 특정 주소에 값을 저장할 수도 있지만 set 명령을 사용해 메모
리 특정 주소에 저장하는 것이 더 일반적이다. p 명령을 사용해 0x8048000 주소에 99
를 저장하고자 할 때는 p *0x8048000=99와 같은 형식으로 사용하고, set 명 령을 사용
하고자 할 때는 다음과 같은 형식으로 사용한다.
set {타입 }［주소］ = ［값］

0x8048300번지에 int 타입으로 100을 넣고자 한다면 다음과 같은 set 명 령을 내린다.
set {int}0x8048300 = 100

8장_gdb 디버거 477

===== PAGE 479 =====
이렇게 명령을 내리면 0x8048300번지에 int 공간인 4바이트 크기의 공간에 100이 들어
간다.

[그림 8-52] set 명령의 사용

타입 문자열로 올 수 있는 것들은 C 언어에서 타입을 정의할 때 사용되는 int, double,

char, ••• 등을 사용할 수 있다.

Q gdb 환경 설정 관련 명령 및 정보 출력 명령
set 명령의 또 다른 기능 중 하나는 gdb 의 환경을 설정할 수 있다는 것이다. 가령 set
prompt woos ： 명령을 내리면 (gdb) 라고 표기하던 프롬프트가 woos :로 바뀐다. 그
리고 set print array on 명령은 배열을 출력할 때 한 행에 출력하는 것이 아니라 다음
과 같이 여러 행에 출력한다.
$2 =
{0x80484a8 "one",
0x80484ac "two",
0x80484b0 "three",
0x0}

이렇게 변경 가능한 환경 설정은 매우 다양한데, info set 명령으로 확인할 수 있다.

info 명령은 정보를 출력할 때 사용한다. info functions 명령은 함수들의 리스트를 출
력하고, info types 명령은 선언된 타입을 보여준다.

info 명령으로 확인 가능한 정보들은 info 를 입력하고 = 키를 두 번 누르면 알 수
있다.

478

4부—디버깅

===== PAGE 480 =====
2 L gdb를 이용한 디버깅 테크닉
기본적인 gdb 사용법을 익혔으니 이번 절에서는 gdb를 이용해 상황별 디버깅 기법과
프로그램 종류별 디버깅 기법을 알아본다. 이전 절에서 배운 내용만0.루.두 디버깅하는
데 부족하지 않지만 몇몇 특수한 상황의 경우 디버깅 기법을 알고 있어야 디버깅이 가
능하기 때문이다. 이전에 배운 내용을 어떻게 응용하는지 확인해 보기 바란다.

I 코어 파일을 이용한 디버깅
앞서 설명했지만 코어 파일이란 프로세스에 예외가 발생해 중지되는 순간의 프로세스
수행 이미지를 의미한다. 이런 프로세스의 이미지에는 중지되는 순간의 CPU context
와 변수 값, 스택의 내용이 들어 있어 디버깅 시 매우 유용하게 사용할 수 있다. 코어 파
일이 생길 수 있는 예외 상황으로는 다음과 같은 것들이 있을 수 있다.

1. 키보드 종료 신호를 받음
2. 잘못된 인스트럭션 수행
3. 디버깅을 위한 브레이크포인트
4. 비정상 종료
5. 버스 오류
6. 부동소수점 예외
7. 잘못된 메모리 참조
8. CPU 시간 제한 초과
9. 파일 크기 제한 초과
10. 잘못된 시스템 콜
이전까지 디버깅에 사용한 bugprg 프로그램의 경우 내부에 잘못된 메모리 참조를 하
기 때문에 코어 파일이 생긴다. 생기지 않는다면 셸에서 코어 파일의 크기가 0으로 설
정되어 있는 경우이므로 다음 명령으로 코어 파일의 제한 크기를 늘리면 된다.
ulimit -S -c 100000000

8장_ gdb 디버거 479

===== PAGE 481 =====
이제 bugprg 프로그램을 수행시키면 코어 파일이 생성됨을 확인할 수 있다.

［그림 8-53］ 코어 파일이 생성된 모습

이렇게 코어 파일이 생성되었다. gdb ［프로그램명］ ［코어 파일명］으로 gdb를 수행하
면 프로그램에 예외가 발생된 그때의 상황으로 환경이 설정된다.
gdb bugprg core.9730

코어 파일 뒤에 오는 숫자는 코어 파일을 남긴 프로세스의 PID로, 필자와 같지 않을 것
이다. 코어 파일만 디버깅에 이용하지 않고 bugprg 프로그램을 함께 디버깅에 사용하
는 이유는 다음과 같다.

./bugprg 명령을 셸에서 내리면 셸이 fork 해 자식 프로세스를 생성한다. 자식 프로
세스는 evecve 시스템 콜을 호출하는데, 인자를 bugprg 프로그램의 패스로 호출한
다. 그러면 커널은 bugprg 프로그램을 자식 프로세스의 메모리 공간에 읽어 들인다.

bugprg는 ELF 바이너리 포맷의 실행 이미지로서 여러 가지 정보가 들어있는데, 그 중
에 프로그램 수행에 꼭 필요한 세그먼트 메모리에 로드한다（디버깅 정보는 로드되지
않는다）. 커널은 환경 변수를 bugprg 프로그램의 태스크에 push하는 등과 같은 여 러
자잘한 초기화 작업을 수행한 후 메모리 에 로드한 bugprg를 실행한다.
코어 파일은 프로그램에 문제가 발생했을 때 커널이 수행 중인 프로그램의 이미지를
파일로 만든 것으로, 메모리와 레지스터, 스택의 정보들로 구성된다. 또한 코어 파일은
커널이 메모리에 로드해 수행 중인 프로그램 이미지이기 때문에 애초부터 디버깅 정보

（ DWARF 섹션들）를 메모리에 로드하지 않았으므로 코어 파일에는 디버깅을 위한 정보
가 전혀 들어있지 않다. 때문에 코어 파일 디버깅을 위해서는 코어 파일과 함께 디버깅
정보가 들어 있는 bugprg 실행 파일도 함께 사용된다.

480 4부_ 디버깅

===== PAGE 482 =====
才 root@os：/temp/gdb
[root(흐os gdb]tt gdb bugprg core.9730
GNU gdb Red Hat Linux (6.6—8.fc7rh)
Copyright (C) 2006 Free Software Foundationy Inc.
GDB is free software, couered bp the GNU General Public License,
and 90U are
welcome to change it and/or distribute copies of it under certai
n conditions.
Type "show copying" to see the conditions.
There is absolutely no warranty For GDB. Type "show warranty" F
or details.
This GDB was configured as ''i386-redhat-linux-gnu"_______________________
Using host libthreaddb library "/lib/libthreaddb.so.1".
warning: Can't read pathname For load map: input/output error.
Reading symbols From /lib/libc.so.6__________________ done.
Loaded symbols For /lib/libc.so.6
Reading symbols From /lib/ld-linux.so.2____________________ done.
Loaded symbols For /lib/ld-linux.so.2
Core was generated by './tjugprg1.
Program terminated with signal 11, Segmentation fault.
tt0 Ox080483b4 in Func (sw=1, str=0x0) at bugprg.c:14
14
printF(“First char = 하cWn", *str);
(gdb) I

[그림 8-54] 코어 파일을 이용해 gdb 실행

gdb를 실행하면 코어 파일에 있는 정보로 무엇 때문에 프로그램이 이상 종료했는지 출
력하고, 심볼을 로드하고 어떤 함수에 문제가 있었는지 출력한다. 그러면 bt 명령으로
스택 프레임을 읽어보고 이전과 같이 디버깅하면 된다.

[그림 8-55] 디버깅 모습

이전에 디버깅하던 것과 동일하다는 생각이 들 것이다. 한 번씩 순차적으로 따라 해 보면

core 파일을 이용해 어떻게 디버깅하는지 금방 알 수 있을 것이다.

8장_ gdb 디버거 481

===== PAGE 483 =====
I 실행 중인 프로세스 디버깅
다음으로 실행 중인 프로세스의 디버깅 기법이다. 이런 경우를 한번 생각해 보자. 서버
프로그램을 작성해 실행시켰는데 서버 프로그램이 죽지는 않지만 제대로 동작하지는
않는다. 그리고 매번 오동작하는 것이 아니라 아주 가끔씩 오동작한다고 가정하면 어떻
게 디버깅해야 할까?
이때는 두 가지 방법이 있는데, 하나는 gdb로 프로그램을 수행한 후 문제가 발생될 때
까지 s 명령으로 수행시키는 고난의 방법과 문제가 발생하길 기다리고 있다가 문제가
발생하면 attach 명령으로 해당 프로세스를 디버깅하는 방법이 바로 그것이다.

attach ［수행 프로세스 PID］ 명령을 내리면 gdb가 현재 수행 중인 프로세스에 일단 브
레이크를 걸고 디버깅할 수 있게 해 준다. 그래서 비동기적으로 문제가 발생하는 경우
에 attach 명령을 사용하면 매우 편리하다. ［예제 8-8］ 로 직접 테스트해 보자.
loop.c 예제 프로그램

〔예제 8-8)

#include <unistd.h>
void
{

fund

(int

i)

static int j;
j += i；

void
{

func2(int

i)

static int k;
k -= i;

int main()
{
int i = 0;
while (1) {
i++；
fund (i) ;
func2 (i);
s丄eep (1);
}
return 0;

482 4부— 디버깅

===== PAGE 484 =====
[예제 8-8]은 무한 루프를 계속 돌면서 fund 함수와 func2 함수를 호출하는 프로그램
이다. 예제 소스를 컴파일해 loop 실행 파일을 만들고 먼저 실행시킨다.

[그림 8-56] loop 프로그램 수행

loop 프로그램을 수행시켰다면 다른 터미널에서 다음 명령을 이용해 loop 프로세스의
PID를 알아낸다.
ps ax | grep loop

[그림 8-57] loop 프로세스의 PID를 알아냄

필자의 경우 PID가 2391인 것을 확인할 수 있다. PID를 알아냈다면 gdb loop 명령으
로 gdb를 실행한다. 그리고 다음과 같은 attach [PID] 명령을 내리면 현재 수행 중인

loop 프로세스에 브레이크가 걸리고 디버깅 가능한 상태로 전환된다.
attach 2391

[그림 8-58] attach 명령으로 디버깅 가능 상태 전환

8장_ gdb 디버거 483

===== PAGE 485 =====
이제 일반적인 디버깅하듯이 디버깅하면 된다. 문제의 원인을 찾았으면 detach 명령을
내려 프로세스를 놓으면 프로세스는 디버거의 손아귀에서 벗어나 혼자 동작한다.

| 멀티프로세스 프로그램 디버깅
gdb로 멀티프로세스를 디버깅하는 일은 다소 편법을 사용해야 하는 번거로운 작업이
다. 특히 버전이 낮은 gdb를 사용한다면 fork() 함수가 호출되면서 자식 프로세스가 죽
어버리기 때문에 멀티프로세스 프로그램의 디버깅이 불가능하다. 다행히 페도라 7 배
포판에 기본적으로 탑재된 6.6-8 버전 gdb는 멀티프로세스 디버깅이 가능하다.
그럼 어떻게 멀티프로세스 프로그램을 디버깅하는지 알아보자. 보통 멀티프로세스 프
로그램들은 다음과 같은 소스로 이뤄진다.
〔예제 8-9)

기본적인 멀 티프로세스 프로그램 소스 예

• ••상략

pid = fork () ;
if (!pid) {

................................................................................................ 1

자식 프로세스가 할 일

}
부모 프로세스가 할 일

... 하략

fork 함수를 호출하면 호출한 프로세스와 같은 새로운 자식 프로세스가 하나 생성된
다. 여기서 fork 함수를 호출한 프로세스를 부모 프로세스라 하고, 새로 생성된 프로세
스를 자식 프로세스라 한다. 부모 프로세스의 pid 변수에는 fork 함수의 리턴 값에 의
해 새로 생성된 자식 프로세스의 PID 값이 들어가고, 자식 프로세스의 pid 변수에는 역
시 fork 함수의 리턴 값에 의해 0이 들어간다. 이렇게 fork 함수에서 리턴되는 값이 다
른 점을 이용해 부모 프로세스와 자식 프로세스가 수행할 일을 달리할 수 있는데, ［예
제 8-9］ 와 같이 if문을 이용해 pid 변수 값이 0인지 아닌지 판단해 부모와 자식 간 프로
그램 수행 흐름이 다르게 할 수 있다.

gdb 는 fork 함수가 호출되어 자식 프로세스가 생성되더라도 부모 프로세스만 디버깅
이 가능하다. 자식 프로세스는 gdb 의 통제를 받지 않을 뿐만 아니라 gdb 버전이 낮을
경우 코어 파일만 남기고 바로 죽어버린다.

484 4부— 디버깅

===== PAGE 486 =====
부모 프로세스를 디버깅하고자 한다면 별 설정 없이 그냥 디버깅하면 되지만, 자식 프
로세스를 디버깅하고자 한다면 다음과 같이 할 수 있다. 부모 프로세스와 자식 프로세
스 간에 데이터를 주고받거나 동기화하는 부분이 전혀 없는 프로그램이라면 부모 프로
세스의 제어 흐름을 자식 프로세스의 제어 흐름으로 바꿀 수 있다.
［예제 8-9］ 의 1번 부분에 브레이크포인트를 설정하고 r 명령으로 프로그램을 수행시킨
다. 1 번 부분에 멈췄다면 다음과 같은 p 명령으로 부모 프로세스의 pid 변수 값을 0으
로 변경해 부모 프로세스가 자식 프로세스의 제어 흐름을 따라가게 할 수 있다.
p pid = 0

부모 프로세스와 자식 프로세스의 동기화가 중요하다면 그때부터 문제가 생기기 시작
한다. 두 가지 정도의 방법이 있는데, 하나는 자식 프로세스를 attach하는 방법으로 다
음과 같다. 먼저 ［예제 8-10］ 과 같이 프로그램을 수정한 후 자식 프로세스가 fork되면
일정 시간을 지연시키는 코드를 삽입한다. 이때 sleep 함수를 사용해 지연시키면 안 된
다. 반드시 루프를 돌게 해 지연시키기 바란다（지연 시간은 변수 값을 적절히 조정해서
정해야 한다）.
〔예제 8-10）

unsigned int d = 0x3fffffff;
pid = fork();
if
(pid)
while(d--);

printf("%d\n”,

pid);

if (!pid) {
자식 프로세스가 할 일

}
부모 프로세스가 할 일

［예제 8-10］ 과 같이 사용하면 프로세스가 지연되기 전에 새롭게 생성된 자식 프로세스
의 PID를 출력하는데, 재빨리 다른 터미널을 열어 gdb ［프로그램명］ ［자식 PID］ 명령
으로 자식 프로세스를 attach하기 바란다. 그 다음부터는 일반적인 gdb 디버깅 방법과
동일하게 디버깅하면 된다. 그러면 실제 소스 코드로 멀티프로세스 프로그램을 디버깅
하는 방법을 알아보자.
8장_ gdb 디버거 485

===== PAGE 487 =====
〔예제 8-11)

fork.c 예제 소스

#include <stdio.h>
#include <unistd.h>
int main ()
{
int pid, var, i = 0x3fffffff;
pid = fork();
if (pid) printf("%d\n”, pid);
while (i--);
if (!pid) {
for (i=0; i<10000; i++) {
var += i;
sleep (1);
}
}
for (i=0; K10000; i++) {
var -= i;
sleep(1);
}
return 0;
}

［예제 8-11］ 을 컴파일하고 디버깅하기 전에 먼저 6.2 버전 이상의 gdb가 설치되어 있
는지 확인한다. gdb -v 명 령을 사용하면 현재 사용 중인 gdb 버전을 확인할 수 있다.

fork.c를 컴파일했으면 gdb fork 명령으로 실행하고, ［그림 8-59］ 와 같이 while 루프
가 끝나는 “if (!pid) {”(필자의 경우 13번째 라인) 부분에 브레이크포인트를 설정하고
실행한다.

［그림 8-59］ fork 프로그램 부모 프로세스 디버깅

486 4부_ 디버깅

===== PAGE 488 =====
r 명령으로 fork 프로그램을 실행하면 fork된 자식 프로세스의 PID를 출력한다. 그러
면 자식 프로세스의 PID(그림에서는 5927)를 재빨리 읽어 새로운 터미널에서 다음과
같이 gdb 를 실행한다.
...■ root@os：/temp/gdb

히

[rootSos g6b ]
gdQ Fork 07]
GNU gdb Red Hat Linux (6.6-8.Fc7rh)
Copyright (C) 2006 Free Software Foundation, Inc.
GDB
is
free
software,
covered
by
the
GNU
General
Public
License,
and you are
welcome
to
change
it
and/or
distribute
copies
oF
it
under
certai
n conditions.
Type "show copying" to see the conditions.
There
is
absolutely
no
warranty
for
GDB.
Type
"show
warranty"
F
or details.
This GDB was configured as "iSSd-redhat-linux—gnu"—
Using host libthreaddb library "/lib/libthread_db.so.1".
Attaching to program: /tenp/gdb/fork, process 5927
Reading symbols from /lib/libc.so.6__________________ done.
Loaded symbols for /lib/libc.so.6
Reading symbols from /lib/ld-linux.so.2—done.
Loaded symbols for /lib/ld-linux.so.2
0x08048445 in main () at fogk.c:11
11
_
while(i—);|
(gdb) |

티
［그림 8-60］ gdb 6.2 버전으로 자식 프로세스 디버깅

gdb ［프로그램명］ ［ PID 번히와 같은 형식으로 명령을 내리면 fork된 자식 프로세스
를 attach해 디버깅할 수 있다. 필자의 경우 자식 프로세스의 PID로 5927이 출력되었
다. 그래서 ［그림 8-6이과 같이 gdb fork 5927 명령을 내리면 자식 프로세스를 디버깅
할수있다.
［그림 8-60］ 의 하단에 있는 while(i-)；가 출력되지 않고 다른 엉뚱한 메시지가 출력
된다면 지연 시간이 초과된 상태에서 gdb 를 수행한 것이므로 그때는 지연 루프의 카
운트를 좀 더 길게 조정하던가 아니면 fork 프로세스를 수행한 후 좀 더 빠르게 gdb로

fork 프로세스를 attach해야 한다.
［그림 8-60］ 과 같이 시간 지연 루프인 while(i-)；가 보인다면 정상 수행된 것이다. 정
상적으로 자식 프로세스가 attach되었다면 이후부터는 일반적인 프로세스 디버깅하듯
이 디버깅하면 된다. 부모 프로세스 역시 마찬가지로 일반적인 디버깅하듯이 디버깅하
면 된다.
멀티프로세스 프로그램을 디버깅하는 나머지 한 방법은 부모와 자식 간에 파이프와 같
은 공유 자원을 이용해 데이터 교환을 하지 않을 때 사용할 수 있는 방법인데, 바로 두
개의 터미널에서 각각의 gdb를 띄우는 것이다. 예를 들면 다음과 같은 형태를 의미한다.

8장_ gdb 디버거 487

===== PAGE 489 =====
# 1 번터미널
gdb test
# 2번터미널
gdb test

그리고 p 명령으로 각각의 gdb에서 생성한 프로세스 pid 변수 값을 1번 터미널은 0(자
식이 된다)으로 만들고, 2 번 터미널은 1 번 터미널 gdb 에서 생성한 부모 프로세스의

PID 값으로 설정한다. gdb에서 생성한 프로세스의 PID 값을 알고 싶으면 ps ax I grep
［프로그램명］ 명령을 사용하면 확인할 수 있다. 이렇게 되면 실제 부모 자식은 아니지
만 pid 변수 값은 부모 자식인 상태에서 가질 수 있는 값들로 설정된다. PID를 사용해
동기화한다면 이런 식으로 하고, 파이프가 아닌 다른 IPC 자원을 이용해 동기화를 수행
한다면 각각의 프로세스에 p 명령으로 IPC ID 값을 서로 하나로 일치시켜 동기화시킬
수 있다.
결국 이렇게 하나 저렇게 하나 멀티프로세스 프로그램의 디버깅은 편법일 수밖에 없다.
멀티프로세스를 디버깅하는 데 있어 굳이 디버거를 사용하겠다면 위에서 설명한 방법
대로 사용한다.

| 멀티스레드 프로그램 디버깅
gdb 를 이용해 멀티스레드 프로그램을 디버깅하는 일은 매우 쉬운 일이다. 단일 스레
드 프로그램과 멀티스레드 프로그램의 디버깅에 있어서 다른 점은 처음 브레이크포인
트를 거는 방법이 다르다는 것 외에는 별반 차이가 없다. ［예제 8-12］ 를 가지고 실제로
어떻게 디버깅하는지 알아보자.
〔예제 8-12］

thread.c 예제 소스

#include <stdio.h>

；

#include <pthread.h>

；

int var;

；

void *add(void *n) {

;

int a;

：

whiled) {
a = var++;
printf("add thread!\n");

}
488 4부— 디버깅

i

===== PAGE 490 =====
}
void *sub(void *n) {
int b;
while (1) {
b = var--;
printf("sub thread!\n");
}
}
int main() {
pthread_t p_thread[2];
pthread_create(&p_thread[0], NULL, add, NULL);
pthread_create(&p_thread[1], NULL, sub, NULL);
pthread_join(p_thread[0], NULL);
pthread_join(p_thread[1], NULL);
return 0;
}

［예제 8-12］ 는 다음 명령으로 컴파일한다.
gcc -o thread thread.c -Ipthread -g

gdb thread 명령으로 gdb 를 실행한 후 1 명령으로 브레이크포인트를 설정할 위치를
찾는다. 브레이크포인트를 설정할 적당한 위치는 pthread_create 함수에 의해 스레드
들이 생성되고 난 직후가 적당하다.

pthreadjoin 함수가 사용되었다면 제일 첫 브레이크포인트를 pthreadjoin 함수 이
후에 설정해서는 안 된다. pthreadjoin 함수가 호출되면 gdb 의 현재 스레드인 main
스레드가 잠들어 버리기 때문에 더 이상 진행하는 것이 불가능하다.
더 이상 진행하는 것이 불가능하다면 Ct「l|+Z 키를 눌러 main 스레드를 중지시킨 후

thread 명령으로 다른 스레드를 선택해 디버깅하거나, Ctffl+C 키를 눌러 중지시킨 후
r 명령으로 다시 시작할 수 있다.

8장_ gdb 디버거 ； 489

===== PAGE 491 =====
［그림 8-61］ 브레이크포인트를 설정한 모습

보통 멀티스레드 디버깅을 할 때는 pthread_create 함수가 호출되어 스레드가 생성
된 후 브레이크포인트를 잡는다. ［예제 8-12］ 는 pthread_create 함수 호출 후 바로

pthreadjoin 함수가 호출되므로 ［그림 8-61］ 과 같이 pthreadjoin 함수가 호출되기
전 위치에 브레이크포인트를 설정하고 r 명령으로 실행한다. 그러면 pthread_create
함수에 의해 add 스레드와 sub 스레드가 생성되면서 새로운 스레드가 생성되었다는
메시지가 출력되고 프로그램 수행이 중지된다. info threads 명령을 내리면 현재 어떤
스레드가 동작하고 있는지 ［그림 8-62］ 와 같이 출력된다.
上

root@os ：/temp/gdb

add
thread?
add
thread?
add
thread?
add thread?
[New Thread -1218667632 (LWP 6277)]
[Switching to Thread -1208174912 (LWP 6273)]
Breakpoint 1, main () at thread.c:28
28
ptpread join(p thread[8], NULL);
(gdb) | info threails|
3
Thread
-1218667632
(LWP
6277)
0x4245d928
in
from /lib/libc.so.6
2
Thread
-1288177776
(LWP
6276)
0X0076F402
* 1 Thread —1288174912 (LWP 6273) main () at thread.c:28

clone
in

()

_kernel_usyscall

(gdb) |

()

I
DI

[그림 8-62] info threads 명령 수행

［그림 8-62］ 을 보면 생성된 순서대로 1번 스레드는 현재 스레드로 main 스레드를 의
미하고, 2번은 add 스레드, 3번은 sub 스레드를 의미한다. 그러면 다음과 같은 명령 형
식으로 add 스레드에 브레이크포인트를 설정한다.
b ［라인번히 thread ［브레이크될스레드번히

490 4부_ 디버깅

===== PAGE 492 =====
b 명령 뒤에 thread를 넣고 스레드 번호를 붙이면 해당 스레드만이 설정한 브레이크포
인트에서 정지한다. add 스레드는 스레드 번호가 2로 할당되었고, 또한 add 스레드가
수행하는 add 함수의 루프 부분은 9행이기 때문에 필자의 경우 b 9 thread 2라고 브레
이크포인트를 설정했다. 그러면 2번 스레드만 9행에 오면 브레이크가 걸리고, 나머지
스레드는 브레이크가 걸리지 않는다.

[그림 8-63] add 스레드에 브레이크포인트 설정

add 스레드에 브레이크포인트를 설정했으면 이제 sub 스레드에 브레이크포인트를 설
정해야 한다. 현재 sub 스레드의 스레드 번호는 3번이고 sub 함수의 루프 부분은 17행
이기 때문에 b 17 thread 3 명령을 내리면 된다. 이후 sub 스레드가 17행을 만나면 브
레이크가 걸릴 것이다.

[그림 8-64] sub 스레드에 브레이크포인트 설정

이제 C 명 령을 내려 프로그램을 수행시키면 브레이크포인트를 걸어준 부분에서 각각의
스레드가 멈춘다. 다음부터는 일반적인 단일 스레드 디버깅 방법과 동일하다.

8장_gdb 디버거

===== PAGE 493 =====
［그림 8-65］ c 명령으로 수행 후 디버깅

［예제 8-12］ 에서 add, sub 함수 내에서 지역변수 a, b가 각각 사용되었는데, 각 스레드
는 자신의 지 역 변수 외에 다른 스레드의 지 역 변수로는 접근할 수 없다. 그래서 add 스
레드가 수행 중일 때 p b 명령을 수행할 수는 없다. 역시 sub 스레드가 수행 중일 때

p a 명령을 수행할 수도 없다. add 스레드가 수행 중일 때 sub 스레드의 지역변수인
b의 값을 보고 싶다면 현재 스레드를 임시로 전환해야 한다.
위의 예제를 컴파일한 후 gdb로 디버깅하는 상황에서 어떤 스레드들이 돌아가는 중이
고 현재의 스레드가 무엇인지 알고자 할 때는 info threads 명령을 사용한다.
/ mot@os：/temp/gdb
(gdb) info threads
3 Thread -1218667632 (LWP 6277) sub (n=0xB) at thread.c:19
Thread -1208177776
LWP 6276； add
n=BxBj at' thread.c:'il"|
1 Thread -1208174912 (LWP 6273) 0XOO76F4O2 in ____________________________________

*》—

〔

〔

11 ()
(gdb) |

버
[그림 8-66] info threads 명령 화면

［그림 8-66］ 에서 스레드 숫자 앞에 *가 붙어 있는 스레드는 현재 수행 중인 스레드임을
의미한다. 그래서 현재 수행 중인 스레드는 add 스레드임을 알 수 있다. 앞에서 이야기
했지만 add 스레드에서는 sub 스레드의 지역변수 b에 접근할 수 없다. b 변수의 내용
을 보고자 한다면 ［그림 8-6기과 같이 thread 3 명령으로 현재 스레드를 sub 스레드로
변경한다.
thread ［ N］

492

4부—디버깅

===== PAGE 494 =====
여기서 [N]은 현재 스레드를 N번 스레드로 변경하라는 의미다.

[그림 8-67] thread 3 명령으로 현재 스레드를 sub 스레드로 변경

그 다음부터는 멀티스레드일지라도 디버깅하는 방식에는 별다른 차이가 없다. 이상이
멀티스레드 프로그램을 디버깅 하는 예였고 다음으로는 라이브러리를 디버깅 하는 예를
알아보자.

I 라이브러리 디버깅
라이브러리를 디버깅하는 것도 무척이나 간단하다. 라이브러리 소스가 있다면 전부

-g 옵션을 주어서 재컴파일해 라이브러리를 만들어 링크하면 된다. 라이브러리 소스가
없다면 어쩔 수 없이 라이브러리 부분은•역어셈블해 디버깅할 수밖에 없다.
라이브러리를 디버깅할 때는 라이브러리 소스의 패스가 매우 중요하다. 즉, bugprg 프
로그램을 예로 들어보면 -g 옵션을 주고 bugprg 프로그램을 컴파일했더라도 소스 파
일인 bugprg.c 파일이 같은 디렉토리에 있지 않다면 gdb에 1 명령을 내렸을 때 소스를
출력할 수 없다. 또는 소스 파일의 이름이 변경되어도 소스를 출력할 수 없다. 그럴 때
는 소스의 이름과 위치를 맞추거나 아니면 역어셈블해 디버깅하는 방법밖에는 없다.
이전에 수없이 이야기했지만 다시 확인하기 위해 물어보면, 왜 이런 일이 벌어질까?

gdb는 -g 옵션으로 컴파일된 실행 파일을 가지고 수행될 때 실행 파일에 들어 있는 디
버깅 정보 중에 실행 파일이 어떤 소스 파일로 이뤄졌는지 알아내고, 1 명령을 내렸을
때 각 인스트럭션에 대응하는 소스를 소스 파일에서 읽어 출력한다. 소스 파일과 실행
파일의 위치가 다르다면 dir 명령으로 소스 파일의 디 렉토리를 지정하거나 gdb를 실행
할 때 -d 옵션으로 지정해야 소스를 보면서 디버깅할 수 있다. dir 명령을 어떻게 사용
하는지 알아보기 위해 표준 C 라이브러리를 디버깅해 보자.

8장_ gdb 디버거 493

===== PAGE 495 =====
먼저 현재 시스템에 설치되어 있는 표준 C 라이브러리(glibc)는 디버깅 정보가 포함되
어 있지 않으므로 디버깅 정보가 포함되게 재컴파일해야 한다. 소스를 받아 재컴파일하
는 일은 번거로운 작업이므로 그냥 현재 시스템에 설치되어 있는 glibc의 SRPM 패키
지를 사용해 재컴파일한다.
http://ftp.kaist.ac.kr/pub/fedora/linux/releases/7/Fedora/source/SRPMS

위 주소에서 glibc-［버전］.src.rpm SRPM 패키지를 다운로드한다. 나중에 패키징 과정
에서 배우겠지만 SRPM 패키지는 소스가 들어 있는 RPM 패키지다. 이런 SRPM 패키지
를 이용하면 손쉽게 디버깅 정보가 들어 있는 RPM 패키지를 빌드할 수 있다.
페도라 배포판 버전이 7이 아닌 경우에는 위 주소에서 7을 8이나 9 등 본인이 사용하는
페도라 배포판 버전으로 변경하기 바란다. 필자는 페도라 배포판 7을 사용하기 때문에
위 주소에서 glibc-2.6-3.src.rpm 파일을 다운로드했다. glibc SRPM 패키지를 받았으
면 다음 명령으로 디버깅 정보가 포함된 이ibc 패키지를 빌드하기 바란다.
rpmbuild ——rebuild ---------------------- glibc-2.6-3.src.rpm

이 작업은 상당히 오랜 시간을 요구하는 작업이므로 느긋한 마음으로 팔굽혀 펴기와 같
은 운동을 해도 괜찮을 것 같다. 건강한 신체에 건강한 정신이 깃드는 법, 나약한 육체에
큰 정신은 아무짝에도 쓸모없고 강한 육체에 나약한 정신 역시 아무짝에도 쓸모없다.
팔굽혀 펴기 대략 2000개쯤 했으면 다음과 같이 정상적으로 빌드된 것을 확인할 수 있
을 것이다.

［그림 8-68］ 디버깅 정보가 포함된 glibc 빌드 모습

494 4부— 디버깅

===== PAGE 496 =====
이

glibc-debuginfo-2.6~3.i386.rpm

중

파일과

glibc-debuginfo-common-2.6-3.

i386.rpm 파일이 디버깅 정보가 포함된 glibc 패키지다. 그러면 다음 명령으로 디버깅
정보가 포함된 glibc RPM 패키지를 설치하기 바란다.
rpm -Uvh /usr/src/redhat/RPMS/i386/glibc-debuginfo-common-2.6—3.
i386•rpm
rpm -Uvh /usr/src/redhat/RPMS/i386/glibc-debuginfo—2.6-3.i386.rpm

순서가

중요하니

glibc-debuginfo-common

패키지를

먼저

설치한

후

glibc-

debuginfo 패키지를 설치하기 바란다. 디버깅 정보가 포함된 glibc 패키지 설치가 끝
났으면 이 전에 사용하던 bugprg를 다음 옵션으로 컴 파일한다.
gcc -o bugprg bugprg.c -g -L/usr/lib/debug/usr/lib -1c -static

라이브러리 탐색 디렉토리로 /usr/lib/debug/usr/lib 디렉토리를 지정하고 정적 표준

C 라이브러리를 이용해 링크했다. /usr/lib/debug/usr/Bb 디렉토리에는 다음과 같은
파일들이 있을 것이다.
gconv

libcrypt.a

libpcprofile. so. debug

libBrokenLocale.a

libdl.a

libpthread.a

libanl.a
libbsd-compat.a

libg.a

libpthread_nonshared.a

libieee.a

libresolv.a

libbsd.a

libm.a

librpcsvc.a

libc.a

libmcheck.a

librt.a

libc_nonshared.a

libmemusage.so.debug

librtkaio.a

libc_stubs.a

libnsl.a

libutil.a

/usr/lib/debug/usr/lib 디렉토리에 있는 파일들이 방금 설치한 디버거 정보가 포함된
이ibc 패키지 파일이고, 컴파일될 당시 -g 옵션을 주어 디버깅 정보를 삽입해 컴파일한
라이브러리 파일들이다. 그래서 위 파일들이 있으면 표준 C 함수들을 소스 레벨에서
디버깅하는 것이 가능하다.
하지만 디버깅 정보가 삽입된 표준 C 라이브러리와 링크했더라도 표준 C 라이브러리
함수를 소스 레벨에서 디버깅할 수 있는 것은 아니다. 표준 C 라이브러리를 컴파일할
때 사용한 실제 소스가 있어야 소스 레벨에서의 디버깅이 가능하다.
그러면 다시 소스를 받아야 하는 것인가? 전혀 고민할 필요는 없다. 이전에 설치한

glibc-debuginfo-common-2.6-3.i386.rpm 패키지에 소스가 포함되어 있었기 때문
에 소스는 이미 시스템에 설치됐다. /usr/src/debug/glibc-20070515T2025 디렉토리

8장_gdb 디버거 495

===== PAGE 497 =====
에서 glibc 소스 파일들을 확인할 수 있을 것이다. 이렇게 소스 파일까지 갖췄다면 이제
모든 준비는 끝났다. 그러면 gdb bugprg 명령으로 gdb를 실행시킨다.

bugprg 프로그램에서 표준 C 함수가 사용된 부분은 printf 함수를 호출하는 부분이다.
때문에 printf 함수를 호출하는 부분에 브레이크포인트를 설정한다.

[그림 8-69] 표준 C 라이브러리 함수인 printf 함수에 브레이크를 건 모습

r 명령으로 bugprg 프로그램을 수행시키고 printf 함수에서 브레이크가 걸리면 s 명령
으로 printf 함수 내부로 들어가 본다.

[그림 8-70] printf 함수 내부로 들어간 모습

printf 함수 내부로 들어가니 printf.c 파일을 gdb가 찾지 못해 “printf.c： No such file
or directory.” 메시지를 출력한 것을 확인할 수 있다. 소스 파일을 찾지 못했기 때문에
당연히 1 명령을 내려도 소스가 출력되지 않는다.

printf 함수의 소스를 보려면 dir 명령으로 printf.c 파일이 있는 디렉토리를 먼저 지정
해야 한다. 앞에서 glibc-debuginfo-common-2.6-3.i386.rpm 파일을 설치해 /usr/

src/debug/glibc-20070515T2025 디렉토리 내에 표준 C 라이브러리 함수들의 소스
를 미리 풀어 놓았었다.

496 4부_ 디버깅

===== PAGE 498 =====
printf.c

파일은

/usr/src/debug/glibc-20070515T2025/stdio-common

디렉토리에

들어있다. gdb에 printf.c 파일이 있는 위치를 알리기 위해 다음 명령을 내린다. 그러면

gdb가 printf 함수의 소스를 찾을 수 있어 소스 레벨에서의 디버깅이 가능하다.
dir /usr/src/debug/glibc-20070515T2025/stdio-common

[그림 8-71] dir 명령으로 printf.c?있는 디렉토리 지정

dir 명령으로 printf.c 소스 파일이 있는 위치를 지정하고 나니 1 명령을 내렸을 때 정상
적으로 소스가 출력됨을 확인할 수 있을 것이다. 이렇게 dir 명령은 소스 파일이 들어
있는 위치를 지정해 gdb가 소스 파일을 읽을 수 있게 해준다.
이렇게 표준 C 라이브러리도 dir 명령을 이용해 소스의 디렉토리를 지정하면 소스를
보면서 디버깅하는 것이 가능하다.
이상이 gdb를 이용한 디버깅 방법이었다. 필자가 지면이 모자라 소개하지 못한 부분도
있다. 그런 부분은 독자가 한번 직접 찾아 알아보기 바란다. 그 과정에서 gdb를 좀 더
많이 알게 될 것이다.
: 마지막으로 중요한 데 필자가 빠트린 팁을 설명하겠다. gdb 프롬프트에서 명령을 내리면 TUI 모드
로 디버깅하는 것이 가능하다. 그러면 훨씬 gdb를 사용하기 쉽다. TUI 모드로 디버깅하다 화면이 지저
분해지면 Ctrt]+L 키를 누르기 바란다.

8장_ gdb 디버거 497

===== PAGE 499 =====


===== PAGE 500 =====
\

a
GUI 디버거
DDD 의 사용

01 DDD 란무엇인가?
02 DDD를사용한디버깅

===== PAGE 501 =====
Le+'s S+udy 서
개인 취향에 따라 다르겠지만 gdb 를 설명할 때 gdb 의 검은 배경 화면만큼이나 암담한 심
정을 느낀 독자가 있었을 것이다. 아마도 GUI 에 너무 익숙해져 gdb의 인터페이스가 어렵
게만 느껴졌을 것이다.
사실 따지고 보면 gdb 가 절대 어려운 것은 아니다. 디버거가 하는 일 자체가 “특정 위치
지정”, “프로그램 수행”, “메모리와 레지스터 값 출력”이라는 매우 단순한 일을 수행하기
때문에 복잡할 필요가 전혀 없다. 그리고 gdb 의 명령들도 일정한 규칙이 있어 복잡하지
않다. 그렇지만 CU（명령라인 인터페이스）를 많이 격어보지 않은 독자라면 CU를 보는 것
자체가 어렵게 느껴졌을 것이다. gdb 가 어렵게 느껴진 사람들을 위해 지금부터는 GUI 디
버거인 ddd를 알아보자.

===== PAGE 502 =====
BLDDD란두헛이가?

표 三，j

ddd 는 지역번호가 아니다. ddd 는 Data Display Debugger 의 약자다. ddd 는 여러 디
버거의 프론트엔드로 CLI 디버거들에게 GUI 환경을 제공한다. 때문에 ddd를 사용하려
면 gdb 같은 실제 디버거가 있어야 한다. 리눅스에서 ddd는 디버거로 gdb를 기본적으
로 사용하지만 ddd에 포함될 수 있는 디버거로는 dbx, xdb, jdb 등이 있다.
이름이 의미하듯이 ddd의 가장 큰 장점은 바로 자료 구조를 비주얼하게 보여준다는 점
이다. 필자는 소싯적에 gdb를 더 선호했었는데, 이제는 ddd를 더 선호한다. 가장 큰 이
유는 ddd가 gdb보다 더 편하기 때문이다. 한창 어린 시절에는 gdb를 사용해 화려하게

CLI로 디버깅하던 것이 나름대로 개발자의 로망이라 생각했었다. 이제는 로망이고 뭐고
그냥 편한 것이 좋다고 생각한다. 인생 뭐 있겠는가? 좋은 것이 좋은 거란 생각이 든다.
그리고 복잡한 자료 구조나 구조체를 가진 프로그램을 디버깅할 때는 gdb 가 적합하
지 않을 수도 있다. 복잡한 자료 구조나 구조체의 값들이 변하는 것을 보려고 gdb에서

display 명령으로 출력하면 자료 구조나 구조체가 크면 클수록 정말 정신 사납게 된다.
화면이 온통 자료 구조 값들로 뒤덮여 어떤 것이 소스이고 어떤 것이 자료 구조인지 분
간이 안 갈 정도가 되어버린다. ddd는 이런 자료 구조들을 아주 비주얼하게 보여주므
로 아무리 복잡한 자료 구조라도 한눈에 확인하는 것이 가능하다.

ddd는 처음 접하는 사람도 디버깅할 수 있을 만큼 사용하기 편하므로 쉽게 접근할 수
있는 디버거다.

02 DDD 를 사용한 디버깅
ddd 사용법을 설명하기 전에 앞에서 gdb 에 대한 내용을 보지 않은 독자는 gdb 부터
보기를 바란다. ddd 는 gdb 를 이용하는 GUI 디버거이므로 많은 부분이 gdb 사용법과
내용이 겹친다. 때문에 gdb 에서 이미 설명한 부분은 독자들이 gdb 를 알고 있다는 가
정하에 따로 설명하지 않겠다.

9장_ GUI 디버거 DDD°| 사용 501

===== PAGE 503 =====
I ddd 시작과 종료
ddd는 gdb처럼 아래와 같은 방법으로 시작 가능하다. 각 실행 방법의 의미는 gdb와
동일하다.
ddd
ddd ［프로그램명］
ddd ［프로그램명］ ［ core 파일명］
ddd ［프로그램명］ ［실행 중인 프로세스 PID］

종료 방법은 일반 윈도우 종료와 마찬가지로 우측 상단에 있는 종료 버튼을 누르거나
툴바에서 File — Exit 메뉴를 누르거나 % + q 키를 누르면 된다. 너무 당연한 것을
설명하였나?

I ddd의 각부분 설명
이전에 사용하던 bugprg 명령을 디버깅하려면 ddd bugprg 라고 입력한다. 그러면 다
음과 같은 ddd 창이 뜬다.
DDD： /temp/gdb/bugprg.s:

［그림 9-1］ ddd 실행 화면

502 4¥_ 디버깅

===== PAGE 504 =====
ddd는 여러 부분으로 나눠졌는데, ① 부분을 디버거 콘솔이라 부른다. 디버거 콘솔은
CLI 디버거（예: gdb） 에 직접 명령을 내릴 때 사용되는 창이다. 그리고 ddd에서 마우스
로 어떤 명령을 내릴 때 명령이 실질적으로 내려지는 창이기도 하다.
② 부분은 소스 창이라 부른다. 소스 창은 소스가 출력되는 것 외에 브레이크포인트를

설정한다거나 마우스로 자료 구조를 선택한다거나 할 때 사용되는 창이다. 처음 ddd를
실행시킨 독자들은 필자처럼 라인 번호가 출력되지 않을 것이다. 라인 번호는 메뉴바

—» Edit — Preferences —* Source —* Display Source Line Numbers 체크 버튼을
클릭하면 볼 수 있다.
③ 부분은 데이터 창이라 부른다. ddd를 처음 실행시켰을 때는 데이터 창이 나타나지
않는다. 데이터 창은 특정 자료 구조에 대해 display 명령을 내려야 생성되는 창이다.

display 명령은 조금 후에 알아본다.
마지막 ④ 부분은 명령 툴이라 부른다. 명령 툴은 ddd에 명령을 내리기 위해 존재한다.
명령 툴 부분을 보면 우리가 gdb에서 사용하던 익숙한 명령들이 버튼 형태로 있는 것
을 확인할 수 있다.
그리고 ［그림 9-1］ 에서는 표현되지 않았지만①과@부분사이에 기계 명령 창이란 부
분이 더 있다. 기계 명령 창은 프로그램의 인스트럭션을 출력하는 창이다. 인스트럭션
레벨에서 브레이크포인트를 설정하거나 디버깅하고자 할 때 기계 명령 창에서 하면 된
다. 기계 명 령 창은 메뉴바 一* View 메뉴에서 Machine Code Window 메뉴를 체크하
면 나타난다.

I ddd에서 브레이크포인트 설정
ddd에서 브레이크포인트를 설정하는 방법은 크게 세 가지가 있다. 이 중 가장 보편적
인 방식은 소스 창의 소스 코드 중 브레이크포인트를 설정하려는 라인에서 마우스 오
른쪽 버튼을 클릭해 브레이크포인트를 설정하는 방식이다.

9장_ GUI 디버거 DDD°| 사용 503

===== PAGE 505 =====
［그림 9-2］ 소스 창에서 브레이크포인트를 설정하는 모습

［그림 9-2］ 가 소스 창에서 마우스 클릭으로 브레이크포인트를 설정하는 모습이다. 이
때 주의할 점은 라인 번호 가까이에서 클릭해야 한다는 것이다. 라인 번호와 떨어진 소
스에서 클릭하면 변수 등을 display하기 위한 메뉴가 나타난다.
브레이크포인트 설정 메뉴 창에는 여러 가지 메뉴가 나오는데, Set Breakpoint가 브
레이크포인트를 설정하는 메뉴다. 한 번만 걸리는 임시 브레이크포인트를 설정하려면

Set Temporary Breakpoint를 선택한다.
Continue Until Here는 선택한 지점까지 진행(continue)하고 브레이크를 걸고자 할
때 사용한다. 예를 들면 프로그램 수행 context가 23번째 라인에 있는데, 30번째 라인
에서 Continue Until Here 메뉴를 선택하면 30번째 라인까지 수행하고 브레이크를 건
다. 그래서 프로그램 수행 context는 30번째 라인으로 온다. Continue Until Here 메
뉴를 사용하려면 프로그램이 동작(run)하고 있어야만 한다.

Set Execution Position 메뉴는 Continue Until Here 메뉴오｝는 다르게 중간에 수행해
야 할 코드를 건너뛰고 해당 지점으로 바로 분기하려 할 때 사용한다. 각각의 메뉴 내
용을 정리해 보면 다음과 같다.

504 4¥_ 디버깅

===== PAGE 506 =====
［표 9-1］ 브레이크포인트 설정 메뉴
Set Breakpoint

해당 지점에 브레이크포인트 설정

Set Temporary Breakpoint

해당 지점에 임시 브레이크포인트 설정

Continue Until Here

해당 지점까지 수행 후 멈춤

Set Execution Position

해당 지점으로 건너뛴 후 멈춤

브레이크포인트가 설정되었으면 ［그림 9-3］ 과 같이 설정된 자리에 붉은색 stop 마크
가 표시되면서 브레이크포인트가 설정된 것이 표현된다.

［그림 9-3］ 브레이크포인트가 설정된 모습

브레이크포인트를 설정하는 두 번째 방식은 디버거 콘솔에서 gdb 명령을 타이핑해 설
정하는 방식이다. ［그림 9-3］ 에서 보면 필자가 디버거 콘솔에서 b 28 명령을 사용해

28번째 라인에 브레이크포인트를 설정했음을 확인할 수 있다.
브레이크포인트를 설정하는 마지막 방식은 툴바의 메뉴를 이용하는 방식이다. 원하는
라인을 소스 창에서 클릭하고 툴바의 Break 버튼을 클릭하면 브레이크포인트가 설정
되는데, 그다지 많이 사용되진 않는다.

9장_ GUI 디버거 DDD의 사용 505

===== PAGE 507 =====
I ddd에서 브레이크포인트 해제
브레이크포인트를 해제하는 방식에도 크게 3가지 방식이 있다. 먼저 소스 창의 브레이
크포인트에서 마우스 오른쪽 버튼을 클릭해 해제하는 방식이 있다.

［그림 9-4］ 브레이크포인트 해제 메뉴

설정된 브레이크포인트에서 마우스 오른쪽 버튼을 누르면 ［그림 9-4］ 와 같은 메뉴 창
이 출력된다. 이 중 Delete Breakpoint 메뉴가 브레이크포인트를 해제하는 메뉴다.

Disable Breakpoint 메뉴는 브레이크포인트를 지우지는 않고 비활성화시키는 메뉴이
고, Properties... 메뉴는 브레이크포인트가 걸리기 위한 조건을 설정하는 메뉴인데.

gdb 명령으로 b 30 if i >= 2 같은 조건 브레이크문과 같다고 보면 이해하기 쉬울 것
이다.
브레이크포인트를 해제하기 위한 두 번째 방식은 디버거 콘솔에서 cl ［해제할 라인 번
히와 같은 명령을 사용하는 방식이 있고, 마지막으로 브레이크포인트를 클릭한 후 툴
바에서 Clear 버튼을 눌러 해제하는 방식이 있다.

506 디버깅

===== PAGE 508 =====
I 프로그램에 걸려 있는 브레이크포인트 확인
현재 프로그램에 걸려 있는 브레이크포인트들을 확인하고 조건을 변경하려면 두 가지
방식이 있다. 첫 번째는 디버거 콘솔에서 info breakpoints 명령을 내린 후 브레이크포
인트들을 확인한 후 수작업으로 condition 명령을 사용해 브레이크가 걸릴 조건을 변
경하는 방식이다.
두 번째 방식은 메뉴바 — Source —■ Breakpoints 메뉴를 선택하면 ［그림 9-5］ 와 같
은 Breadpoints and Watchpoints 창이 뜨는데, 해당 창에서 프로그램에 설정되어 있
는 브레 이크포인트들을 확인하고 조건도 변경할 수 있다.

[그림 9-5] Breakpoints and Watchpoints 창

I 프로그램 수행
자, 이제 브레이크포인트 설정과 해제하는 방법도 알았으니 본격적으로 프로그램을
수행하면서 디버깅해 보자. 먼저 main 함수의 시작 부분에 브레이크포인트를 설정하기
바란다. 그리고 프로그램을 수행한다. 프로그램을 수행하려면 디버거 콘솔에서 r(run)
명령을 입력하거나 ［그림 9-6］ 과 같이 명령 툴에서 Run 버튼을 클릭하면 프로그램이
수행된다.

9장_ G니 디버거 DDD의 사용 507

===== PAGE 509 =====
［그림 9-6］ 프로그램 수행 모습

프로그램을 수행하면 ［그림 9-6］ 과 같이 녹색 화살표로 현재 어디를 수행할 차례인지
라인 번호 옆에 표시된다. 디버거 콘솔에서 진행 명령은 gdb의 명령과 동일하므로 따
로 설명하지 않겠다. 명령 툴의 각 버튼은 ［표 9-2］ 와 같다.
［표 9-2］ 명령 툴 버튼 설명
Run

프로그램을 수행

Interrupt

프로그램에 SIGINT 시그널을 보냄（브레이크포인트를 설정하지 않은 프로그램의 수행을 멈출
때 사용）

Step

현재의 라인을 수행, 함수 호출 시 함수 내부로 들어감

Stepi

현재의 인스트럭션을 수행, 함수 호출 시 함수 내부로 들어감

Next

현재의 라인을 수행, 함수 호출 시 함수 내부로 들어가지 않음

Nexti

현재의 인스트럭션을 수행. 함수 호출 시 함수 내부로 들어가지 않음

Until

현재 bop를 빠져 나감

Finish

현재 함수를 수행하고 빠져 나감

Cont

다음 브레이크포인트를 만날 때까지 진행

Kill

프로그램 수행 종료

Up

현재 보고 있는 함수를 호출한 함수로 소스 창 이동

508 4부— 디버깅

===== PAGE 510 =====
Down

현재 보고 있는 함수가 호출한 함수로 소스 창 이동

Undo

변수 값 등이 이전 명령 수행 전 상태로 돌아감（실제 수행 흐름은 이전으로 돌아가지 않음）

Redo

변수 값 등이 다음 명령 수행 후 상태로 돌아감（실제 수행 흐름은 이전으로 돌아가지 않음）

Edit

에디터가 수행되면서 소스를 수정할 수 있음

Make

재컴파일을 위해 Make 명령을 내림

대부분의 명령들은 이미 gdb에서 설명했음으로 따로 설명하지 않고 설명하지 않은 명
령만 알아보자. Interrupt 명령은 이미 프로그램이 수행 중인데 브레이크포인트를 설정
하지 않았을 경우 등 프로그램을 멈출 방법이 없을 때 사용한다. 예를 들면 루프를 한
참 돌린 후 임의로 멈추고자 할 때 브레이크포인트 설정 없이 r 명령으로 그냥 수행시
킨 후 Interrupt 버튼을 눌러 멈추면 된다.

Up/Down 명령은 소스 창의 포커스를 옮길 때 사용하는 명령이다. 가령 현재 프로그
램 수행 커서가 main 함수에서 호출한 func 함수 수행 중일 때 Up 버튼을 누르면 func
함수를 호출한 main 함수로 소스 창 포커스가 이동한다. Down 버튼은 반대로 이동한
포커스를 다시 돌릴 때 사용한다고 생각하면 된다.

Undo 버튼은 변수 값 등의 이전 명령 수행 전 상태를 확인할 때 사용한다. Redo 버튼
은 그 반대라 생각하면 된다. Undo/Redo는 실제 명령을 취소하지는 못한다. 단지 이
전 상태 확인만 가능하다.

Edit/Make 명령은 디버깅 중 잘못된 부분을 확인해 소스 수정 후 다시 결과를 확인하
려 할 때 사용한다. Edit/Make 명령은 굉장히 자주 사용하므로 한 번씩 테스트해 보기
바란다.

I 와치 포인터 설정
와치 포인터를 설정하는 방법에는 주로 두 가지가 사용된다. 디버거 콘솔에서 watch
명령으로 설정할 수도 있고 툴바의 Watch 메뉴에서 설정할 수도 있다. 와치 포인터 설
정은 전혀 어려운 것이 아니므로 따로 설명하지 않는다.

9장_GUI 디버거 DDD의 사용 509

===== PAGE 511 =====
I 변수 값 검사
ddd를 사용하면서 gdb보다 편하다고 느끼는 부분이 바로 각종 변수와 레지스터 값을
확인할 때다. 우선 디버거 콘솔에 명령을 직접 입력하지 않고 변수의 값을 확인해 보는
방식에는 크게 세 가지 정도가 있다.

GI 마우스 커서로 해당 변수 값 확인
마우스 커서를 해당 변수에 위치시키면 ［그림 9-刀과 같이 해당 변수의 값이 출력된다.

［그림 &-7］ 마우스 커서를 사용해 변수 값 확인

@ print 메뉴로 해당 변수 값 확인
다음으로 ［그림 9-8］ 과 같이 값을 확인하려는 변수에서 마우스 오른쪽 버튼을 클릭하
면 Print ［변수명］ 메뉴가 나타나는데, 해당 메뉴를 선택하면 디버거 콘솔로 변수의 값
이 출력된다.

510 4부_디버깅

===== PAGE 512 =====
［그림 9-8］ print 메뉴에서 변수 값 확인

［그림 9-8］ 에서 Print *［변수명］ 메뉴도 보일 것이다. 해당 메뉴는 값을 알려는 변수가
포인터 변수일 때 해당 포인터가 가리키는 값을 확인하려 할 때 사용한다.

@ display 메뉴로 해당 변수 값 확인
［그림 9-8］ 에서 보면 Display ［변수명］ 메뉴가 보일 것이다. 해당 메뉴를 클릭해 보면
［그림 9-9］ 와 같이 된다.

[그림 9-9] Display gtime와 Display pt를 수행한 예
9장_ GUI 디버거 DDD의 사용 ； 511

===== PAGE 513 =====
필자는 Display gtime과 Display pt를 수행했다. pt의 경우 포인터 변수이기 때문에
실제 값을 보려면 포인터 변수가 가리키는 값을 알아야 한다. 이렇게 포인터 변수의 값
을 따라가려면 ［그림 9-9］ 에서와 같이 해당 포인터 값에서 마우스 오른쪽 버튼을 클릭
했을 때 나오는 Display *() 메뉴를 클릭한다. 그러면 ［그림 9-10］ 과 같이 포인터 변수
가 가리키는 값이 표시된다.

［그림 9-10］ pt의 값에서 Display *() 메뉴를 선택한 예

［그림 9-10］ 에서는 포인터 변수 간의 관계가 그다지 복잡하지 않아 모양이 단순하게
나오는데, 복잡한 자료 구조의 경우 ［그림 9-11］ 처럼 화려하게 출력된다.

512 4부—디버깅

===== PAGE 514 =====
［그림 9-11］ 복잡한 자료 구조의 Display 예

| 레지스터, 메모리, 스레드, 스택 등의 상태 확인
레지스터, 메모리, 스레드, 스택 등의 상태를 확인하는 방법은 너무 쉽다. 메뉴바 —

Status 메뉴를 클릭해 보면 스택, 레지스터, 스레드, 시그널 등의 상태를 확인할 수 있
다. 그리고 메뉴바 — Data 메뉴를 열어보면 메모리 값을 확인해 볼 수 있는 메뉴가 있
다. 너무 쉬우니 그냥 한 번씩 테스트해 보기 바란다.

| 프로세스 attach와 detach
프로세스를 attach 하고 detach 하는 것도 무척 간단하다. attach 하려면 메뉴바 — File

—’Attach to Process... 메뉴를 클릭해 ［그림 9-12］ 와 같은 창이 나타날 때 attach할
프로세스를 선택해 Attach 버튼만 누르면 attach된다.

9장_ GUI 디 버거 DDD의 사용 513

===== PAGE 515 =====
[그림 9-12] 프로세스 attach 모습

그리고 detach하고자 할 때는 메뉴바 — File — Detach Process 메뉴를 선택하면 된다.

I 기타 알아두면 좋을 사항
다음은 그냥 알아 두면 좋을 정도의 내용이다.

O 창을 분리해 사용하는 법
지금까지 필자가 ddd 사용법을 설명하면서 디버거 콘솔, 소스 창, 데이터 창이 하나로
합쳐진 형태로 사용하면서 설명하였다. 사실 이렇게 창이 하나로 붙은 상태에서 사용하
면 실전에서 많이 불편하다. 예를 들면 자료 구조가 클 경우 데이터 창을 크게 늘리면
상대적으로 소스 창과 디버거 콘솔의 사이*} 줄어들 수밖에 없기 때문이다.
그래서 보통은 이렇게 창을 하나로 합쳐 사용하지 않고 각각의 창들을 따로 분리해
사용한다. 창을 분리하고자 할 경우 메뉴바 —■ Preferences —■ Startup — Window

Layout —* Separate Windows를 선택하면 ddd 실행 시 창이 분리된 상태로 시작된다.
@ 지역변수와 인자 값은 Display해 놓으면 보기 편하다

지역변수와 인자 값은 자주 확인하는 경향이 있다. 지역변수의 값이 바뀌는 것을 쉽게
알 수 있고 함수가 호출되었을 때 인자 값을 한눈에 알아보려면 해당 값들을 display해
놓으면 디버깅하기가 훨씬 편하다. 메뉴바 — Data ■— Display Local Variables 메뉴와
메뉴바 ~> Data —• Display Arguments 메뉴를 선택해 놓으면 함수가 호출될 때마다
해당 함수의 지역변수들과 인자들이 데이터 창에 display된다.
이상으로 ddd를 사용해 어떻게 디버깅하는지 알아보았다. 사용해 보면 알겠지만 ddd는
정말 쉬운 디버거다. gdb가 불편한 독자가 있다면 ddd를 사용해 보라고 권하고 싶다.

514 4부_디버깅

===== PAGE 516 =====
10
기타 디버깅 툴

01 trace 유틸리티를사용한 프로그램문제점 분석
02 문제 진단 유틸리티

===== PAGE 517 =====
LG+'S S+mdy
일반적으로 스위스 만능 칼과 일반 톱 둘 다 있을 때 나무를 자르는 데 스위스 만능 칼을
사용하지는 않는다. 나무만 자르고자 할 때는 톱이 더 성능도 좋고 사용하기도 편하기 때
문이다. 스위스 만능 칼에 온갖 도구가 달려있어 못하는 일이 없을 지라도 말이다.
디버거와 기타 디버깅 툴과의 관계는 스위스 만능 칼과 일반 톱의 관계와 같다. 디버거로
못하는 디버깅이란 거의 없다. 하지만 디버거가 모든 디버깅에 가장 적합한 것은 아니다.
어떤 문제들에 대해서는 디버거보다 더 적합한 툴들이 있다. 지금부터 그런 툴에는 어떤
것이 있는지 알아보자.

===== PAGE 518 =====
01 trace 유틸리티를 사용한 프로그램
문제점 분석
trace 유틸리티는 프로그램이 수행하면서 생성하는 각종 트레이스를 출력한다. 이런
트레이스에는 시스템 콜 트레이스와 라이브러리 함수 호출 트레이스 등이 있다.

I strace를 사용해 프로세스의 문제 진단
strace, Itrace로 대표되는 trace 유틸리티는 프로그램의 문제를 진단하는 데 사용한
다. 여기서 strace는 System-call tracer를 의미하는 말로 프로세스가 호출하는 시스템
콜을 화면에 출력한다. 시스템 콜이란 프로세스가 커널에 요청하는 서비스 루틴으로,

open, read, write 등이 대표적이고 그 외 다음과 같은 것들이 있다.
exit
fork
read
write
open
close
waitpid
creat
link
unlink
execve
chdir
time
mknod
chmod
lchownl6
alarm
fstat
pause
utime
access
nice
sync
kill
rename
mkdir
rmdir
dup
pipe
times
signal
geteuidl6
getegidl6

acct
umount
ioctl
fcntl
setpgid
umask
chroot
ustat
dup 2
getppid
getpgrp
setsid
sigaction
sgetmask
getrusage
gettimeofday
settimeofday
getgroupsl6
setgroupsl6
old_select
symlink
Istat
readlink
uselib
swapon
reboot
munmap
truncate
ftruncate
fchmod
fchownl6
getpriority
setpriority

sysinfo
ipc
fsync
sigreturn
clone
setdomainname
newuname
modify_ldt
adjtimex
mprotect
scall
setfsuidl6
setfsgidl6
llseek
getdents
select
flock
msync
readv
writev
getsid
fdatasync
sysctl
m 丄 ock
munlock
mlockall
munlockall
cwd
vfork
getrlimit
mmap2
truncate64
ftruncate64

stat64
lstat64
fstat64
Ichown
getuid
getgid
geteuid
getegid
setreuid

10장_ 기타디버깅툴 517

===== PAGE 519 =====
위 표는 리눅스 커널 2.4에 있는 시스템 콜을 나열한 것인데, 실제로 이보다 훨씬 많이
있지만 지면상 생략했다. 이런 시스템 콜은 많은 부분 표준 C 라이브러리 내에 함수 형
태로 들어 있다.
예를 들면 open(), read(), write() 등이 바로 시스템 콜이다. 시스템 콜이 필요한 이
유는 다음과 같다. 유닉스 시스템은 커널 모드와 유저 모드라는 두 가지 모드를 가지고
있고, 각각의 모드는 다음과 같은 특징 이 있다.
커널 모드에서는 모든 메모리 영역에 접근 가능하며, 모든 인스트럭션이 사용 가능하
다. 반면 유저 모드에서는 자신에게 할당된 메모리 영역에만 접근 가능하며, 잘못되면
시스템에 치명적인 몇몇 인스트럭션(Igdt, lidt 둥)은 사용 불가능하다.
이렇게 유저 모드와 커널 모드로 나누어 놓은 이유는 시스템을 보호하기 위해서다. 일
반적인 애플리케이션들은 유저 모드에서 동작한다. 그런데 애플리케이션이 수행 중에
커널 메모리 영역에 있는 자료 구조를 변경해야 될 일이 생겼다고 하자. 예를 들면 nice
함수를 사용해 자신의 우선순위를 변경하려고 하였다면 커널에 있는 자신의 프로세스
구조체(task_struct)에 있는 nice 필드 값을 변경시켜야 한다.
애플리케이션은 유저 모드에서 동작하기 때문에 커널 메모리에 접근이 불가능하다. 이
럴 경우 시스템 콜을 사용해 커널에게 변경시켜달라고 요청을 한다. 표준 C 라이브러
리 함수 nice() 의 어셈블리 코드를 보면 커널에 요청하는 코드가 들어 있음을 확인할
수 있다. nice뿐만 아니라 커널에 있는 모든 자료 구조에 접근하려면 시스템 콜을 사용
해야 한다. 또한 자료 구조뿐만 아니라 모든 장치에 접근하기 위해서도 시스템 콜을 사
용해 커널에 요청해야 한다.
표준 C 라이브러리에 보면 많은 함수가 시스템 콜로 되어 있다. strace 유틸리티는

ptrace라는 시스템 콜을 사용해 자식 프로세스가 어떤 시스템 콜을 호출하는지 감시한
다. 그리고 호출하는 내용을 화면에 출력한다. 이 런 시스템 콜 정보는 프로그램이 이유
없이 수행이 안 될 때 유용하게 사용할 수 있다. 가령 다음과 같은 상황이 발생했다고
가정해 보자.
프로그램이 그동안 잘 수행되다가 갑자기 수행이 안 되는데 아무런 메시지도 출력하
지 않는다. 물론 gdb를 사용해 무엇이 문제인지 알아봐도 되지만 프로그램이 -g 옵션
으로 컴파일되지 않았거나 소스 파일이 없다면 역어셈블해 디버깅해야 한다. 이럴 경우

strace 명령으로 프로그램을 수행해 어떤 시스템 콜을 호출하고 리턴 값은 무엇인지 체
크하면 정말 쉽게 문제를 분석할 수 있다.

518 4부_디버깅

===== PAGE 520 =====
간단히 예를 들어 설명한다.
〔예제 10-1) ; syscall.c 테스트 예제

#include <stdio.h>
#include <sys/types.h>
#inclucie <sys/stat.h>
#include <fcntl.h>
int main() {
int fd;
fd = open (’’/bin/cat", O_WRONLY) ;
if

(fd >= 0) {
printf (’’0K\n") ;

}
return 0;
}

［예제 10-1］ 과 같은 syscall.c 테스트 예제 코드가 있다고 가정하다. 코드를 읽어보면
알겠지만 별다른 것 없다. /bin/cat 파일을 쓰기 전용으로 열고 정상적으로 열린다면

“OK”를 출력하는 소스 코드다. 위 코드를 gcc -o syscall syscall.c 명 령으로 컴파일한
후실행한다.

［그림 10-1］ 정상적인 수행 모습

당연히 ［그림 10-1］ 에서 보듯이 “OK”가 정상적으로 출력될 것이다. 이제 이 프로그램
이 비정상적으로 동작하는 상황을 임의로 한번 만들어본다.

［그림 10-2］ 비정상적인 수행 모습

10장_ 기타디버깅 툴 519

===== PAGE 521 =====
［그림 10-2］ 에서 보면 syscall 프로그램을 실행시켰을 때 “OK”가 출력되지 않음을 확
인할 수 있다. ［그림 10-2］ 와 같은 비정상적인 수행 상황을 만들려면 먼저 cat〉aaa 명
령을 입력하고 Ctrl］ + z 키를 눌러 cat 명령을 멈춘 후 빠져 나온다. 그리고 syscall 프
로그램을 실행 시켜 보면 “OK” 문자열이 출력되지 않는 것을 확인할 수 있을 것이다.
자, cat〉aaa 명령은 우리가 모른다고 가정하고 어느 날 갑자기 잘 동작하던 syscall 프
로그램이 ［그림 10-2］ 와 같이 동작하지 않게 되 었다고 가정하자. 물론 소스도 없다. 이
럴 때 strace를 사용하면 운이 좋으면 한 번에 문제를 찾을 수도 있고 운이 나쁘더라도

syscall 프로그램에서 무슨 일을 하는지 대충 짐작할 수 있다.
strace -fF ./syscall

위 명령을 내리고 나면 다음과 같은 메시지가 출력된다.
’ root@os：/temp/gdb

『[rootBos gdb]tt|strace -FF ./syscall
execue("./syscall", ["./syscall"], [/« 27 uars »/]) = 0
0x839d000
brk(0)
access("/etc/ld.so.preload", R_0K)
-1 ENOENT (No such file or dil
rectory)
open("/etc/ld.so.cache", O RDONLV)
Fstat64(3, <st_mode=S_IFREG|0644, st_size=61603,
...» = 0
mmap2(NULL, 61603, PR0T_READ, MAP_PRTUATE, 3, 0)
= 0xb7F9e000
close(3)
0
3
open("/lib/libc.so.6", 0_RD0NLV)
read(3, "»177ELFtf1W1W1WOW0tf OWflWOWOtf0W0tf0tf3tf0»3W0W1W0W0W0W3200:B"..
2) = 512
fstat64(3, {st_node=S_IFREG|0755, st_size=1673760, ...}) = 0
mnap2(NULL, 4096, PROT_READ|PROT_WRITE, MAP_PRIUATE|MAP_AN0NVM0US,
0) = 0xb7F9d000
mmap2(Ox4238d0O0, 1390032, PROT_READ|PROT_EXEC, MAP_PRIUATE|MAP_DENYWRI
TE, 3, 0) = Ox4238dOO0
mmap2(0x424db000, 12288, PROT_READ|PROT_WRITE, MAP_PRIUATE|MAP_FIXED|MA
PDENVWRITE, 3, 0x14e) = 0x424dbOO0
mmap2(Ox424de0O0, 9680, PROT_READ|PROTWRITE, MAP PRIUATE|MAP_FIXED|MAP
AHONVMOUS, -1, 0) = 0x424de000
close(3)
=0
nnap2(NULL, 4096, PROT_READ|PROT_WRITE, MAP_PRIUfiTE|MAP_fiNONVMOUS, -1,
0) = 0xb7F9c000
set_thread_area({entry_number:-1 -> 6, base_addr:0xb7F9c6c0, limit:1048
575, seg_32bit:1, contents:0, read_exec_only:8, limit_in_pages:1, seg_n
ot_present:0, useable:1}) = 0
nprotect(0x424db000, 8192, PROT_READ)
nprotect(0x419d70O0, 4096, PROT_READ)
=0
munfnap(8xb7fge088, 61603)
=8
openC'/bin/cat", O_WRONLV)
= -1 ETXTBSV (Text File busy)
exit_group(8)
Process 12999 detached
[root
os gdb]tt |

(흐

[그림 10-3] strace —fF ./syscall 명령을 내린 모습

520 4부—디버깅

프로그램 실행
준비 과정

===== PAGE 522 =====
strace -fF ./syscaU 명령을 내리니 뭔지는 모르겠지만 암호와 같은 수많은 메시지가
출력됨을 확인할 수 있을 것이다. 이 메시지 중 ［그림 10-3］ 에서 “프로그램 실행 준비
과정”이라 적혀 있는 앞부분은 프로그램이 수행하기 위해 공유 라이브러리 등과 링크
하려고 동적 링크가 커널에게 요청한 시스템 콜이기 때문에 신경 쓸 필요가 없다.

syscall 프로그램이 호출한 시스템 콜은 그 밑에 사각형 부분인데 open 시스템 콜을 보
면 리턴 값이 -1 인 것을 알 수 있다. open 에서 -1 이 리턴되었다는 의미는 open 시스
템 콜이 정상적으로 수행되지 않았다는 의미다. 그리고 -1 뒤에는 “ETXTBSY” 문자열
이 보일 것이다. ETXTBSY는 open 함수가 왜 실패했는지 이유를 나타내는 값이다. 이
값은 errno 변수에 들어가는 값이기도 하다.
혹시 ETXTBSY와 같은 오류 번호가 무엇을 의미하는지 알고 싶은 독자는 man open 명령으로 open
함수의 매뉴얼을 보면 ETXTBSY를 포함한 다른 여러 오류 번호를 확인할 수 있다.

“ETXTBSY” 문자열 뒤에는 설명이 있는데 “Text file busy”라 표시되어 있다. “Text
file busy” 의 의미는 실행 파일을 쓰기 권한으로 open 하는데, 이때 실행 파일이 이미
실행되고 있다는 의미다. 윈도우= 그렇고 리눅스도 그렇지만 대부분의 운영체제에
서 현재 실행되고 있는 바이너리 파일은 쓰기 권한으로 open할 수 없다.
즉, /bin/cat 을 쓰기 권한으로 open 하고자 했는데 /bin/cat 이 이미 실행되고 있다
는 말이다. 하하하. 드디어 문제의 원인을 찾았다. 그럼 cat 명령을 종료한 후에 다시

syscall 프로그램을 실행시켜 보자.

［그림 10-4］ cat 명령 종료 후 syscall 수행

fg 명령을 내리고 리 + C 키를 눌러 cat 명령을 종료시킬 수 있다. 그리고 syscall 프
로그램을 다시 수행시켜 보면 정상적으로 “OK”가 출력되는 것을 확인할 수 있을 것이
다. 우리는 방금 strace 명령을 사용해 손쉽게 syscall 프로그램의 문제가 무엇인지 확
인해 보았다. strace를 몰랐다면 어 땠을까?

10장_ 기타 디버깅 툴 521

===== PAGE 523 =====
물론 gdb 를 사용하면 쉽게 확인할 수 있다. 하지만 gdb 를 사용해 확인했다면 일일이
인스트럭션을 따라가면서 무엇이 문제인지 확인하는 데 시간도 걸리고 상당히 번거로
웠을 것이다.
이렇게 strace 명령으로 프로그램이 요청하는 시스템 콜 정보는 프로그램의 문제를 알
아보는 것뿐만 아니라 프로그램이 어떻게 수행되는지 또는 어떤 파일에 접근하는지 알
아보는 데도 유용하게 이용할 수 있다.
〔예제 10-2)

system call 요청 모습

• ..상략

open("./ispace.conf", O_RDONLY)
=3
fstat64(3, {st_mode=S_IFREG|0644, st_size=764, ...})
=0
mmap2(NULL, 4096, PROT_READ|PROT_WRITEZ MAP_PRIVATE|MAP_
ANONYMOUS, -1, 0)
= 0x40017000
read(3, "################################" • … 4096) = 764
read(3, 4096)
=0
close (3)
=0
munmap(0x40017000, 4096)
=0
open("./ispace.log", O_RDONLY)
=3
fstat64(3, {st_mode=S_IFREG|0644, st_size=1397, . . . })
=0
mmap2(NULL, 4096, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS,
-1, 0)
= 0x40017000
read(3, "Aug 11 08:00:23 Proactive Manage"..., 4096)
= 1397
read(3,
4096)
=0
• •• 하략

［예제 10-2］ 는 strace 명령으로 어떤 프로그램의 시스템 콜을 본 것인데, 이 프로그램
은 먼저 ./ispace.conf 파일을 열어 읽어 들이는 것을 알 수 있다. ./ispace.conf 파일의
모든 내용은 모르지만 처음엔 ####으로 시작하는 것으로 보아서 설정 파일일 가능성 이
높을 것이다.
그리고 ./ispace.log 파일을 열어 읽어들이는데, 내용은 “Aug 11 08：00：23 Proactive

Manage” 형태의 날짜로 되어 있는 것을 알 수 있다. 이렇게 시스템 콜 정보로 프로그
램이 어떻게 동작하는지 전체적인 윤곽도 잡을 수 있다. 때로는 현재 수행 중인 서버
프로세스가 어떤 시스템 콜을 요청하고 있는지 알고 싶을 때가 있을 것이다. 정상적으
로 동작하는지 어떤지를 파악하려고 알고 싶을 때가 있다. 그럴 때는 다음 명령을 사용
한다.

522 디버깅

===== PAGE 524 =====
strace -fFp [수행 중인 서버 PID]

f 옵션은 자식 프로세스가 fork되면 자식 프로세스의 시스템 콜까지 출력하라는 의미
고, F는 vfork에 의해 생성된 자식 프로세스의 시스템 콜도 출력하라는 의미다. 그리고

P 옵션은 뒤에 오는 PID를 가지는 프로세스를 트레이스하라는 의미다.
위 명령을 각자 테스트해 보기 바란다. 먼저 터미널 두 개를 띄워 놓고 한 터미널에서
다른 터미널의 PID를 사용해 위 명령을 내려보자. 예를 들면 A, B 터미널 두 개를 띄워
놓고 B 터미널에서 strace -fFp [A 터미널의 PID] 명령을 내린다. 그리고 A 터미널에
타이핑을 해 보면 재미난 현상을 확인할 수 있을 것이다. 관심 있는 사람들은 한번 해
보기 바란다.

I Itracel 사용해 프로세스가 호출하는 공유 라이브러리 함수 알아보기
Itrace는 library call tracer의 줄임말로 프로세스가 호출하는 공유 라이브러리 함수를
보여준다. 표준 C 공유 라이브러리를 링크해 컴파일했다면 모든 표준 C 함수가 여기에
해당한다. Itrace는 반드시 공유 라이브러리의 함수 호출만을 보여주기 때문에 컴파일
시 -static 옵션을 주어 정적 라이브러리와 링크하게 컴파일한 실행 파일의 경우에는
아무런 정보도 표시하지 못한다. 다음은 어떤 프로그램을 Itrace 명령으로 수행시켜 나
타난 결과인데, 그 프로그램이 호출하는 함수는 무엇이며, 인자는 무엇이며, 리턴되는
값은 무엇인지 자세한 정보가 출력되는 것을 확인할 수 있다.
V] [screen 1： baqg]_root@o으ytemp/book/debug/hns

：' 리터 가 지

strtok("2003.08.11 Thu 14:00:27", •'.•')
‘- "
atoi(8xbFFFee30, 0x888497be, 511, 18, 1)
strtok(NULL,
atoi(0xbFFFee35, 0x880497be, 511, 10, 1)
strtok(NULL, " ")
atoi(0xbFfFee38, 0x888497c0, 511, 10, 1)
strtok(NULL, " ")
strncpy(0xbfFFee20, "Thu", 15)
strcmpCThu'', "Sun")
strcmpC'Thu", "Mon")
strcnp("Thu“, "Tue")
strcmp("Thu", "Wed")
strcmp("Thu", "Thu")
strtok(NULL,
atoi(0xbFFFee3f, 8x080497de, 15, 10, 4)
strtok(NULL,
atoi(0xbFFFee42, 0x080497de, 15, 10, 4)
strtok(NULL,
atoi(0xbFFFee45, 0x088497e0, 15, IB, 4)
strcnpflight", "light")
calloc(1, 56)
meincpy(0x0804ae50, "H033", 44)
Fgets("Aug 11 08:00:23 Proactive Manage"__________________ , 512, 0x08i
++♦ exited (status 0) +++
[root
os hns]tt 1

= ••2003"
= 2003
= "08"
=8
= "11"
= 11
= "Thu"
= 0xbfFFee20
=1
=1
= -1
= —1
=0
= "14”
= 14
= "00"
=0
= "27"
= 27
=0
= 0x0804ae50
= Ox 08O4ae50
»4a998) = NULL

(흐

[그림 10-5] Itrace 명령으로 본 공유 라이브러리 함수 호출 정보

10장_ 기타디버깅툴 523

===== PAGE 525 =====
fork된 자식 프로세스가 요청하는 공유 라이브러리 함수까지 보려면 -f 옵션을 사용하
고, 현재 수행 중인 프로세스의 함수 요청을 보려면 -p [PID] 옵션을 사용한다. 그리고
시스템 콜과 함수 호출을 같이 보려면 -S 옵션을 사용한다.
이렇게 trace 유틸리티들은 사용하기 간편하면서도 양질의 정보를 제공하므로 디버깅
이나 프로그램을 분석하는 데 자주 이용되곤 한다.

꼬2문제 진단 유틸리티

tW•.艾!:※
丁 ■.
'스.'.:
*•’ 느

I splint로 소스 코드의 문제점 진단
[예제 10-3]과 같은 문제의 소스가 있다고 할 때 과연 이 소스의 문제는 컴파일러가 알
아서 찾아줄 수 있을까?
〔예제 10-3〕 bug.c 예제 소스

#include <stdio.h>
#include <stdlib.h>
int add(int a, int b)
{
return a + b;

int main()
{
int arr[3] = {1, 2, 3};
int i, no_init;
int *p;
for (i=0; i<5; i++)
no_init += add(i, arr[i]);
p = (int *)malloc(sizeof(int) * 2);
fr은은 (p);
free(p);
return 0;
}

524 4부— 디버깅

===== PAGE 526 =====
［예제 10-3］ 은 no_init 지역변수를 사용하면서 초기화시키지 않았다. 그래서 의도와 다
른 결과가 나올 수 있다. 또한 arr 배열을 사용함에 있어서 배열의 범위를 넘어간다. 이
런 경우 보통 세그먼트 폴트가 발생한다.
마지막으로 free를 두 번 하였다. 이런 경우 항상 그런 것은 아니지만 프로그램이 중단될
수 있다. 문제의 소스를 gcc의 -W -Wall 옵션으로 모든 오류 메시지를 활성화시켜 컴파일
해도 gcc는 문제에 대해 알지 못한다. ［예제 10-3］ 은 문법적으로 이상이 없기 때문이다.

［그림 10-6］ gcc로 버그 프로그램 컴파일

gcc 는 알지 못했지만 splint 로 점검해 보면 알 수 있다. splint (Secure Programming
Lint)는 미국 버지니아 대학에서 만든 C 소스 검사 유틸리티다. splint는 C 소스를 검
사해 문제가 발생할 수 있는 아주 사소한 오류도 출력한다. 페도라 7 배포판의 경우

splint가 기본적으로 설치되어 있지 않으므로 yum install splint 명령으로 먼저 설치하
기 바란다.
• root@os：/temp/gdb

(흐

[root
os gdb]tt splint bug.c
Splint 3.1.1
11 Sep 2006
bug.c: (in function main)
bug.c:16:3: Uariable no_init used before definition
An rualue is used that map not be initialized to a ualue on sone execution
path. (Use -usedef to inhibit warning)
bug7c:20:^: bead storage p passed as out parameter to freg. p ""

-—■

Memory is used aFter it has been released (either by passing as an only param
or assigning to an only global). (Use —usereleased to inhibit warning)
bug.c:19:7: Storage p released
bug.c:4:5: Function exported but not used outside bug: add
A declaration is exported, but not used outside this module. Declaration can
use static qualifier. (Use —exportlocal to inhibit warning)
bug.c:7:1: Definition oF add
Finished checking ------------------ 3 code warnings
[root@os gdb]tt |

［그림 10—7］ splint bug.c 명령으로 C 소스 검사

10장—기타디버깅툴 525

===== PAGE 527 =====
I 메모리 디버거의 사용
프로그래머들이 굉장히 많이 저지르는 실수 중 다음과 같은 것이 있을 수 있다.
〔예제 10-4〕 메모리 디버거의 사용을 보이기 위한 예제

int func()
{
int *p = NULL;
*p = 1212;
p
=
(int

*)malloc(sizeof(int))

;

p

*)malloc(sizeof(int))

;

=

(int

free (p);
free(p);
return 0;

［예제 10-4］ 의 문제는 할당되지 않은 포인트 변수에 값을 집어넣은 것과 malloc을 두
번하면서 같은 포인트 변수에 받음으로써 하나의 int 타입 공간에 대한 참조를 잃어버
린 것, 그리고 free를 두 번 한 것을 들 수 있다.
할당되지 않은 공간에 값을 집어넣은 것은 당연히 세그먼트 폴트가 발생할 것이고, int
타입 참조를 하나 잃어버린 것 때문에 위 함수가 계속 호출된다면 메모리 누수가 발생
한다.
메모리 누수 문제는 ［예제 10-4］ 와 같이 할당된 메모리에 free를 해 주지 않아 발생하
는데, 짧게 끝나는 프로그램은 문제가 되지 않는다. 프로그램이 종료됨과 동시에 커널
이 프로그램에 할당된 메모리 자원을 모두 반환하기 때문이다. 하지만 서버 데몬이나

GUI 애플리케이션과 같이 항상 수행되는 프로그램의 경우 메모리 누수가 발생하면 시
스템의 메모리를 고갈시킨다. 시스템의 메모리가 고갈되더라도 스왑 파일 시스템을 이
용해 시스템이 죽지는 않겠지만 속도는 매우 느려질 것이다.

526 4부_ 디버깅

===== PAGE 528 =====
이런 메모리 누수나 잘못된 메모리 참조를 디버깅하는 데 valgrind, mpatrol 등의
메모리 디버거가 이용될 수 있다. 메모리 관련 디버거는 valgrind, mpatrol 외에도

dmalloc, LeakTracer, mcheck 등 매우 많은 종류가 있고 dmalloc과 같이 라이브러
리 형식이거나 valgrind와 같이 실행 바이너리 형식인 것도 있다. 이 중 valgrind가 단
연 최고라 말할 수 있다.

El valgrind
valgrind는 대부분의 메모리 문제를 찾을 수 있는 매우 똑똑한 메모리 디버거다.
valgrind는 가상으로 프로그램을 실행시켜 프로그램에서 요청하는 malloc, free를 잡
아채 문제가 있는지 없는지 동적으로 분석한다. 동적으로 분석하기 때문에 valgrind가
정확하게 문제를 찾아낼 수 있다. 대신 약간 느린 단점이 있긴 하다.
얼마 전 필자는 누군가의 부탁으로 T-DMB 음성, 영상 코덱을 ARM 아키텍처에 최적
화하는 일을 맡았었다. 문제는 해당 코덱이 아직 개발 과정에 있는 코덱이라 제대로 되
는 것이 하나도 없었다는 점이다. 현재 성능이 어떻게 나오는지 체크하기 위해 코덱을
정상 동작시키는 일만도 수많은 버그를 고치고 나서야 가능했다.
가뿐한 기분으로 버그들을 해결하고 테스트 보드에서 돌리니 중간쯤 돌다가 메모리 오
류가 발생해 멈춰버리는 것이었다. 처음엔 단순한 메모리 참조 오류인줄 알고 gdb로
확인해 보니 단순한 메모리 참조 오류가 아니었다. 할당받은 메모리를 2중 free하는 문
제도 있었고, 메모리 leak도 발생해 시스템의 메모리를 완전히 고갈시키는 문제가 소스
전반에 걸쳐 나타나고 있었다.
보통 상황이 이쯤되면 웬만한 개발자는 소위 말해 절어 버린다. 버그 중에 잡기 힘든
버그가 메모리 버그이기 때문이다. 소스라도 간단하면 문제가 없겠는데, 코덱 소스이다
보니 얼마나 정신없게 코딩되어 있겠는가. 더구나 처음부터 끝까지 필자의 개입 없이
다른 사람이 짠 소스 코드다.
하지만 필자는 전혀 절지 않았다. 필자에 게는 든든한 valgrind가 있었기 때문이다. 그
러니 valgrind를 꼭 기억하기 바란다.

10장_ 기타 디버깅 툴 527

===== PAGE 529 =====
그럼 valgrind를 사용해 실제 디버깅을 해 보자. 이전에 사용하던 bug.c 파일을 -g 옵
션으로 재컴파일하고 다음과 같은 명령으로 실행하면 b니g.c에 있는 메모리 관련 오류
를 자세하게 출력한다.
valgrind
-v ./bug

--tool=memcheck

——leak-check=yes

--leak-resolution=high

valgrind가 bug 프로그램이 호출하는 malloc나 free를 추적하면서 문제가 있는 부분
에 대해 ［그림 10-8］ 과 같은 오류 메시지를 출력한다.
root@os：/temp/gdb
==13243==
by Ox804844A: main (bug.c:19)
—13243— REDIR: Ox423FC810 (menset) redirected to 0x4006600 (memset)
==13243==
==13243== ERROR SUMMARY: 13 errors from 9 contexts (suppressed: 0 from 0)
==13243==
==13243==
1 errors in context 1 of 9:
==13243==
Inuaiid"
/ deiete / delete[ ] |
==13243==
at 8X4B058FF: free (vq replace _njalloc.c:233)
==13243==[
bjj 8x8848455: main (bug.c：20)
==13243==
Address 0x401A028 is 0 bytes inside a block of size 8 free'd
==13243==
at 0X4B050FF: free (vq_replace_malloc.c:233)
==13243==[
'6
520&@44
main <b；f.c':19) — |
==13243==
1 errors in context 2 of 9:
==13243==
==13243==
Conditional jump or moue depends on uninitialised ualue(s)
==13243==
0X419C6D25: _dl_relocate_object (in /lib/ld-2.6.so)
==13243==
by 0X419BFA84: dl_main (in /lib/ld-2.6.so)
==13243==
by 0x419CFF6A: _dl_sysdep_start (in /lib/ld-2.6.so)
==13243==
0X419BD2B7: 2dlzstart ?in /lib/ld-2.6.so)
==13243==
by Ox419BC816: (within /lib/ld-2.6.so)
==13243==
==13243==
errors in context 3 of 9:
==13243==
Conditional jump or moue depends on uninitialised ualue(s)
==13243==
at 0x419C6BE3: _dl_relocate_object (in /lib/ld-2.6.so)
==13243==
by 8x419BFM4: @l_i；ain (in 71ib/ld-2.6.so)

싀믜씌
I싀

니
「

히

呼

阿

L리

［그림 10-8］ valgrind에서 출력한 오류 메시지

［그림 10-8］ 에서 valgrind 테스트 중 혹시 세그먼트 폴트가 발생해 valgrind가 제대로
동작하지 않는 독자도 있을 것이다. bug.c 소스 내용을 보면 for （ i=0； i<5； i++） 부분에

arr 배열의 크기가 3인데 배열의 사이즈를 넘어간 참조를 해서 그런 것이니 for （ i=0； I
〈 3； i++） 로 바꾸고 컴파일하면 될 것이다.
［그림 10-8］ 을 보면 알겠지만 valgrind는 정확하게 bug.c의 19행과 20행에서 2중 free
를 한다고 알려준다. bug.c에서는 메모리 leak을 발생시키는 부분이 없어 valgrind 출
력 결과가 그다지 재미없는데, 메모리 leak이 발생하면 어디에서 leak이 발생했고 얼마
만큼 leak이 발생 했는지 결과까지 출력 한다.

528

4부_ 디버깅

===== PAGE 530 =====
지금은 valgrind가 그다지 마음에 와닿지 않는 독자도 있을 거라 생각한다. 와닿던 와
닿지 않던 메모리 디버거라 하면 valgrind를 기억해 두기 바란다. 언젠가는 valgrind의
위대함을 눈물로 칭송할 날이 반드시 올 것이다.
이것으로 메모리 디버거에 대한 설명은 마치고자 한다. valgrind 외에 수많은 메모리
디버거가 있지만 valgrind만 알고 있으면 될 것이다. 이상으로 기타 디버깅 툴에 대한
설명을 마친다.

10장_ 기타 디버깅 툴 529

===== PAGE 531 =====


===== PAGE 532 =====
11.
make

01 make°| 이해
02 매크로의사용
03 확장자 규칙의사용
04 더미 타겟의 사용
05 명령사용규칙
06 재귀적 make의 사용
07 조건부수행
08 함수의사용
09 특수 타겟
10 make 최종 정리

===== PAGE 533 =====
Le+ s S+uidy
를 수정하고 컴파일해 결과를 확인하는 일은 프로젝트 수행 과정 내내 무수히 많이
발생한다. 소스 파일이 적으면 상관이 없다. 그러나 소스 파일이 많다면 그 과정을 일일
이 손으로 작업한다는 것은 정말 크나큰 고역이 아닐 수 없다.
또한 개발 과정이 끝난 후 프로젝트 파일을 소스로 배포하는 데도 문제가 있다. 개발한
컴퓨터의 환경과 컴파일될 컴퓨터의 환경이 같을 것이라는 보장은 없다. 세상에는 수많
은 종류의 유닉스와 리눅스가 있고, 겉모습은 비슷하지만 서로 다른 점이 많이 있다. 개
발자가 개발한 소스가 많은 컴퓨터에서 제대로 동작하려면 몇 가지 기술과 유틸리티의
도움이 필요하다.
여러분은 make, autoconf, automake, libtool 과정에서 이런 문제를 해결하기 우 I 해 프
로젝트를 손쉽게 빌드하는 방법과 여러 시스템에 쉽게 이식될 수 있는 이식성 높은 프
로젝트 빌드 방법을 배울 것이다.

===== PAGE 534 =====
01 make 의 이해
make 는 매우 유용한 유틸리티임과 동시에 굉장히 매력적이고 똑똑한 유틸리티다.
make가 없었다면 유닉스, 리눅스 개발자들은 프로젝트가 끝남과 동시에 손가락에 지
문이 남아 있지 않았을 것이다.
개발 과정에서 소스 파일을 수정하고 컴파일한 후에 수행 결과를 확인하는 일은 프로
젝트 수행 전반에 걸쳐 일어나는 매우 반복적인 일이다. 소스 파일 개수가 많지 않으면

gcc 명령으로 일일이 타이핑해 컴파일하는 것도 나름의 멋이 있다. 그러나 소스 파일
이 많아지고, 각 파일에 대해 서로 다른 컴파일러와 어셈블러를 사용하고, 각기 다른 옵
션으로 컴파일해야 된다면 컴파일하는 데 시간도 많이 걸리고 일일이 타이핑해야 하기
때문에 개발자에게는 정말 고통이다. 또한 커널과 같은 대규모 프로젝트를 컴파일할 때
는 컴파일 시간도 많이 걸린다. 개발하는 시간도 모자란데 컴파일해 결과를 확인하는
일에 많은 시간을 낭비할 수는 없는 노릇이다. 이런 문제점들을 해결하기 위해 나온 것
이 바로 make 다.

make 에 대한 정의를 내린다면 make 는 파일 관리 유틸리티다. make 는 각 파일 간의
종속 관계를 파악해 기술 파일(Makefile)에 기술된 대로 컴파일 명령이나 셸(shell) 명
령을 순차적으로 내린다. make는 각 파일에 대한 반복적 명령을 자동화시켜 개발자의
수고를 덜고, 시간을 절약할 수 있다.
프로젝트에 make를 도입한다면 컴파일 시간을 절약할 수 있고 프로그램의 종속 구조
를 빠르게 파악할 수 있으며 관리가 용이해진다. 또한 단순 반복 작업을 최소화시킬 수
있다. 그리고 make는 소스를 컴파일하는 것뿐만 아니라 닥북(DocBook) 문서를 컴파
일하고 기타 순차적이고 반복적인 어떤 작업에든지 이용할 수 있다.

11장_ make 533

===== PAGE 535 =====
기술 파일 (Makefile)
의미 해석

d.c, c2.c, c3.c, c4.c
중에 컴파일하지 않아도
지장이 없는 것은?

a. c 파일을 디버깅 옵션으로 컴파일해라.
b.c는 모듈을 컴파일해라.
d. cc는 c++ 컴파일러로 컴파일해라.
/temp/c 디렉토리에 들어가서 확장자가
c인 모든 파일 을 컴파일해 라.

/usr/bin/make

d .c, c2.c, c3.c, c4.c 파일을 각각 컴파일해서
실행 파일 mybin을 만들어라.
만든 mybin을 /user/local/bin에 복사해 라.
모든 object 파일과 실행 파일을 지워라.
/user/local/bin의 mybin을 지워 라.

［그림 11-1］ make와 기술 파일의 관계

make의 동작 방식은 매우 단순하다. ［그림 11-1］ 과 같은 Makefile 기술 파일을 작성
하면 make가 기술 파일에 적힌 대로 명령을 수행한다. 결국 기술 파일을 작성하는 법
과 make 에 대한 몇 가지 특징만 이해하면 make 를 프로젝트에 도입할 수 있다. 기술
파일을 작성하는 일은 매우 쉽고 간단하기 때문에 빠르게 익힐 수 있다. 먼저 독자의
이해를 돕기 위해 간단한 예제 기술 파일을 바탕으로 설명한다.

| make의 기본 동작

nmnsil 소스 파일의 내용
diary.h :
#include <stdio.h>
int memo();
int calendar ();

memo. c :
#include "diary.h"
int memo() {
printf("function memo.\n”);
return 0;
}

main.c :
#include "diary.h”
int main() {
memo();
calendar();
return 0;

calendar.c :
#include "diary.h”
int calendar() {
printf("function calendar.\n");
return 0;

}

}

5부_ 프로젝트 빌드

===== PAGE 536 =====
［예제 11-1］ 은 예를 들기 위해 작성한 것이다. 소스를 컴파일해 실행 파일 diary를 만
든다고 할 때 각 소스 파일의 종속 구조는 다음과 같다.

실행파일

［그림 11-2］ 소스 파일 구조도

〔예제 11-2)

Makefile의 내용

-E可

all : diary
diary : memo.o calendar.o main.o
<j+gcc -W -Wall -o diary memo.o calendar.o main.o

—W
—-［③

사이 간격이 TAB임을 주의

memo.o : memo.c
gcc -W -Wall -c -o memo.o memo.c

—~@1
—41瓦］

calendar.o : calendar.c
gcc -W -Wall -c -o calendar.o calendar.c

—PZ
<-4⑦］

main.o : main.c
gcc -W -Wall -c -o main.o main.c

—폐

—4⑨

clean :
rm -rf *.o diary

소스 구조에서 볼 수 있듯이 diary라는 프로그램은 memo.c와 calendar.c, main.c 파
일로 이뤄졌고, 각 C 소스 파일은 diary,h 파일을 include한다. ［예제 11-2］ 와 같은

Makefile을 작성하고 make 명령을 내리면 각 오브젝트에 대한 컴파일 명령을 수행한
후 최종적으로 diary 파일을 생성하는 것을 알 수 있다.

11 장_ make 535

===== PAGE 537 =====
if' root@serwr：/work/book/utils_new/make
[root@seruer make]ttjmake' clean |~~~
,.
........
rn -rF *.o
diarp
[root@seruer
make]tt[make |
gee -W
-Wall - c -o memo.0 nemo.c
-Wall - c -o calendar.0 calendar.c
gee -W
gcc -W
-Wall - c -o main.o main.c
gcc -W -Wall
- o diary meino.o calendar.o nain.o
[root@seruer
make]tt
[root@seruer
make]tt Is diary
diary|
[root@seruer
make]tt |

[그림 11-3] 컴파일 화면

이런 일이 어떻게 발생하는지 먼저 알아보자.

1. make 명령을 내리면 make는 먼저 현재 디렉토리 내에서 기술 파일을 찾는다. 기
술 파일은 Makefile, makefile 또는 GNU make인 경우에는 GNUmakefile일 수
있다. 지금 상황에서는 Makefile이 기술 파일에 해당한다.

2. Makefile 내에서 제일 처음 오는 타겟을 찾는다. 현재로서는 all 타겟이 해당한다.
3. aU 타겟을 만들기 위한 종속 항목 diary를 보고 diary라는 파일이 현재 디렉토리
내에 없다는 것을 확인한다.

4. diary를 생성하기 위한 룰을 찾기 위해 (2) 항목을 접하고 diary를 생성하기 위한
첫 번째 종속 항목 memo.o가 아직 만들어져 있지 않았음을 확인한다.

5. memo.o를 생성하기 위한 룰을 찾기 위해 (4) 항목을 읽고 memo.o의 종속 항목
memo.c가 현재 디 렉토리에 있는 것을 확인하면 make는 memo.o를 만들기 위한
명령인 (5) 명령으로 memo.o를 컴파일해 만들어낸다.

memo.o가 미리 만들어져 있다면 make는 다시 만들 필요가 있는지 검토한다. 만
들어져 있는 memo.o 보다 memo.c 의 수정 시간이 최근이라면 memo.o 가 만들
어진 후 memo.c가 수정되었기 때문에 다시 만들 필요가 있다. 다시 만들 필요가
있다면 make는 (5) 명령을 수행하고 그렇지 않다면 (5) 명령을 건너뛰고 다음 과
정으로 넘어간다. 다른 파일도 마찬가지로 만들어졌다면 다시 만들 필요가 있는지
판단해 만들 필요가 있다면 만든다.

6. 다시 (2) 항목으로 가서 diary의 종속 항목 memo.o는 생성되었지만 calendar.o
는 아직 생성되지 않았음을 확인한다.

7. calendar.o를 생성하기 위한 룰인 (6) 항목으로 가서 calendar.o는 calendar.으에
종속되어 있고 calendar.c는 현재 디렉토리에 있다는 것을 확인하고 calendar.o
를 생성하기 위한 명령인 (7) 명령을 수행해 calendar.o를 생성한다.

536

5부—프로젝트빌드

===== PAGE 538 =====
8. 다시 (2) 항목으로 가서 diary를 생성하기 위한 종속 항목인 main.o가 아직 만들
어지지 않았음을 확인하고 main.o를 생성하기 위한 룰인 (8) 항목으로 가서 main.
으의 존재 유무를 확인하고 (9) 명령을 수행해 main.o를 생성한다.

9. 다시 (2) 항목으로 가서 이제는 diary 를 생성하기 위한 종속 항목인 memo.o,
calendar.o, main.o가 다 만들어진 것을 확인하고 diary를 생성하기 위한 명령인
(3) 명 령을 수행해 diary를 생성한다.
10. (1) 항목으로 가서 aU 타겟을 생성하기 위한 diary가 만들어진 것을 확인한 후 현
재 all 타겟을 생성하기 위한 특별한 명령이 없으므로 make는 all 타겟이 생성되
었다고 간주하고 정상적으로 종료한다.
위에서 설명한 내용을 토대로 make의 기본 동작을 정리하면 다음과 같다. make 명령
수행 시 make memo.o 명령과 같이 특별한 타겟 (make memo.o 명령에서는 memo.o
가 타겟임)을 지정하지 않으면 제일 처음 만나는 타겟을 생성하려고 한다. 그래서 처음
에 ［예제 11-2］ 의 경우 ⑴ 항목의 aU 타겟을 생성하려고 하기 때문에 전체 오브젝트 파
일이 컴파일되고 최종적으로 diary 실행 파일을 링크한다. make memo.o와 같이 특별
한 타겟을 지정하면 make는 memo.o 타겟을 생성하기 때문에 다음과 같이 수행한다.

[그림 11-4] make memo.o 명령 수행

make clean 은 나중에 다룰 예정이니 지금은 그냥 make clean 명령을 내리면 ［예제
11-2］ 에서 clean 타겟에 해당하는 rm -rf *.o diary 명령을 수행한다고 생각하자.
make memo.o 명령을 수행하기 전에 make clean 명령을 내린 이유는 이미 만들어
진 memo.o를 지우기 위해서다. 현재 이전 make 명 령으로 인해 memo.o가 이미 만들
어져 있는데, make 는 memo.o 파일의 생성 시간과 memo.c 파일의 최근 수정 시간을
비교해 다시 만들 필요가 있는지 판단한다. memo.o는 memo.c의 최근 수정 시간보다
이후에 만들어졌기 때문에 make는 다시 만들 필요가 없다고 판단하고 컴파일 명령을
수행하지 않는다.

11장_ make 537

===== PAGE 539 =====
make 는 모든 타겟에 대해 타겟과 종속 항목들의 수정 시간을 비교해 재컴파일할 필
요가 있는지 판단한다. 타겟이 모든 종속 항목의 수정 시간보다 이후에 만들어졌다면

make는 새로 컴파일할 필요가 없는 것으로 간주하고 그 타겟에 대해서는 컴파일 명령
을 수행하지 않는다.
이런 기능은 kernel 처럼 거대한 프로젝트를 다룰 때 유리하다. 제일 처음 kernel 소스
를 컴파일하면 이미 컴파일되어 있는 오브젝트 파일이 없기 때문에 전체를 컴파일하는
데 많은 시간이 걸린다. 그러나 두 번째 이후부터는 수정된 파일만 컴파일하고 전체 링
킹하기 때문에 컴파일 시간이 매우 적게 든다.

kernel에 어떤 기능을 추가하기 위해 kernel을 수정하고 매번 전체 소스를 컴파일해야
한다면 정말 kernel 프로그래밍하기가 힘들었을 것이다. 현재와 같이 make를 사용하
지 않고 셸 스크립트 같은 것으로 kernel 컴파일을 했다면 책을 옆에다 두고 컴파일하
는 데 걸리는 무료한 시간을 달래야 했을지도 모르는 일이다.
지금까지 make가 기술 파일(Makefile)을 어떻게 해석해 명령을 내리는지 알아보았다.
결국 프로젝트에 make를 사용하기 위해 기술 파일만 작성하면 되는 것이다.
기술 파일을 작성하는 일은 매우 간단하고 단순한 작업이다. 몇 가지 규칙만 따른다
면 자신의 프로젝트에 맞는 기술 파일을 쉽게 생성할 수 있다. 위에 예로 든 기술 파일

(Makefile)은 독자의 이해를 돕기 위해 작성한 것이라서 make의 놀라운 기능을 거의
사용하지 않아 기술 파일이 일일이 컴파일 명령을 쳐서 컴파일하는 것만큼 길다.
실제 make의 숨은 기능을 사용한다면 단 몇 행으로 위.기술 파일이 하는 모든 작업을
그대로 할 수 있는 기술 파일을 만들어낼 수 있다. 이제 기술 파일을 작성하는 데 지켜
야 할 규칙과 make의 다른 숨은 기능들을 사용해 좀 더 효율적인 기술 파일을 작성하
는 방법을 알아보자.

I 기술 파일의 작성
기술 파일의 파일명은 GNU make 인 경우 GNUmakeflle, makefile, Makefile 중 어
떤 것도 사용할 수 있지만 관습적으로 Makefile을 사용한다. Makefile을 사용하는 이
유는 대문자로 시작하기 때문에 주로 소문자로 시작하는 소스 파일과 쉽게 구분되기
때문이다.

538

5부_ 프로젝트빌드

===== PAGE 540 =====
한 디렉토리 내에 GNUmakefile과 makefile, Makefile0］

함께 들어있다면 GNU

make인 경우 GNUmakefile, makefile, Makefile순으로 기술 파일을 찾기 때문에
GNUmakefile이 프로젝트 빌드에 사용된다.

O 기술 파일의 기본 구조
〔예제 11-3）

기술 파일 기본 구조

CC = gcc
targetl : dependencyl dependency2
commandl
command2
target2
:
dependency3
commands
command4

dependency4

dependency,

［예제 11-3］ 은 기술 파일의 기본 구조를 보여준다. 기술 파일의 제일 첫 부분은 내부에
서 사용할 매크로의 정의 부분이다. 매크로를 기술 파일에서 사용하면 정의된 스트링으
로 치환된다. 다음에 오는 것은 규칙 정의 부분인데, 타겟이 오고 콜론（：） 뒤에 그 타겟
을 생성하기 위해 필요한 종속 항목들의 리스트가 온다.
종속 항목과 타겟은 통상 파일명이 되지만 반드시 그럴 필요는 없다. 그 부분에 대해서
는 나중에 좀 더 심도 있는 기술 파일 작성 기법에서 알아보기로 하고 일단 파일이라고
생각하면 이해하기 편할 것이다. 그래서 ［예제 11-3］ 의 룰 1을 예로 들면 targetl 파일
을 빌드하려면 dependencyl 파일과 dependency2 파일이 필요하다. 보통 종속 항목
에 속하는 파일들은 타겟을 빌드할 소스 파일이나 오브젝트 파일들이다. 다음 행으로
종속 항목들이 충족되었을 때 타겟을 생성하기 위한 명령 리스트가 온다. 종속 항목이
충족된 상태에서 타겟을 생성하기 위해 make는 나열된 명령을 위에서 아래로 순차적
으로 수행해 타겟을 생성한다. 기술 파일의 기본 구조를 알고 기술 파일 구문 기본 규
칙을 지키면서 기술 파일을 작성하면 독자는 아주 쉽게 기술 파일을 만들 수 있다.
기술 파일 구문 기본 규칙이란 것도 매우 간단하기 때문에 겁내지 말기 바란다.

11장_ make 539

===== PAGE 541 =====
@ 기술 파일 구문 작성 기본 규칙

1. 명령의 시작은 반드시 TAB으로 시작되어야 한다.
targetl : dependencyl dependency2 ...
commandl
<----- ► command2
오

Tab으로 시작한다.

명령이 탭으로 시작되어야 하는 규칙은 make 의 오래된 관습이다. 탭으로 시작되
지 않은 명령절을 만나면 make는 명령절을 타겟절로 해석하기 때문에 “*** missing

separator." 혹은 “… 분리 기호 ...”라는 오류 메시지를 출력하고 수행을 중단할 것
이다. vim 설정에 따라 어떤 vim에서는 Makefile을 해석해 탭과 같은 크기의 공백을
만나면 붉은색 블록으로 잘못된 명령라인임을 알리기도 하고 다음 그림처럼 명령라
인 색깔을 붉은색이 아닌 흰색으로 보여주기도 한다.

[그림 11-5] TAB 시작 오류 화면

2. 비어있는행은 무시된다.
targetl : dependencyl dependency2 . . . 타겟절
이 행은 무시된다.

commandl

며령절

타겟절 이하에 오는 명령절에 있어 비어있는 명령라인은 무시된다.

3. ‘#’을 만나면 개행 문자를 만날 때까지 무시한다.
targetl : dependencyl dependency2 ...
commandl
# 주석

540

5부_ 프로젝트 빌드

# 주석
# 주스j

===== PAGE 542 =====
기술 파일 내에서 ‘#’은 셸 스크립트와 마찬가지로 주석의 시작을 의미한다. 그래서
이후 개행 문자까지 make에 의해 무시된다.

4. 기술 행이 길어지면 V를 사용해 이을 수 있다.
diary : memo.o calendar.o\ ,........................n
갍은의마 . diary : memo. o calendar. o main. o
ma. 丄 ri • o

셸 스크립트와 마찬가지로 행 끝에 ‘\’를 만나면 ‘\’는 공백으로 치환되고 다음 행의
‘\’가 있던 바로 뒤에 붙는다.

5. ‘;’는 명령라인을 나눌 때 사용한다.
targetl : dependencyl dependency2; commandl

위와 같이 타겟절에 ‘;’를 붙이면 정의절의 끝을 의미하고 바로 뒤에 명령절이 올 수
있다. 그렇지만 위와 같이 잘 사용하지는 않는다. 기술 파일의 가독성이 떨어지기 때
문이다. 이후 독자들도 5번 규칙은 알아만 두고 무시하기 바란다.

6. 종속 항목이 없는 타겟도 사용 가능하다.
clean :
rm -rf*.o targetl target2

6번 규칙은 자주 사용된다. 종속 항목이 없기 때문에 명 령절은 바로 수행된다. 명령
절이 정상적으로 수행된 후에 make는 타겟이 실제 파일로 존재하지 않더라도 룰을
해석하는 그 순간만큼은 타겟이 만들어진 것으로 간주한다.

7. 명령부분에는어떤 명령이 와도 상관없다.
targetl : dependencyl dependency2 ...
‘ cp -f filel file2
gcc -o targetl dependencyl dependency2
gdb targetl

명령절에는 반드시 컴파일 명령이나 종속 항목과 관계된 명령만사용하라는 법은 없
다. 개발자가 필요한 어떤 명령이라도 알맞게 사용하면 된다.

지금까지 기술 파일 구문 작성 기본 규칙을 알아보았다. 매우 쉽지 않은가?
지금까지 배운 내용만으로도 독자의 프로젝트에 맞는 기술 파일을 만들 수 있다. 그렇
지만 아직까지는 무언가 부족하다. 이제부터 어떻게 하면 좀 더 효율적으로 기술 파일
을 작성할 수 있는지 알아보자.

11장_ make 541

===== PAGE 543 =====
2 L 매크로의 사용
기술 파일 내에 매크로는 C와 마찬가지로 사용자 정의 변수에 특정한 문자열을 정의하
고 표현하는 것을 의미한다. 이후 매크로는 기술 파일 내에 정의된 문자열로 치환되어
사용될 수 있다. 매크로를 사용하는 일은 좀 더 일관되고 좀 더 이식성이 높고 융통성
있는 기술 파일을 만들기 위해 필요하다.
CC = gcc

가령 위와 같은 CC 매크로를 정의했다면 호는 기술 파일 내부에서 $(CC)로 표기함으
로써 gcc로 치환될 수 있다. 같은 소스를 ARM 아키텍처에 맞게 크로스 컴파일러로 컴
파일해 ARM CPU에서 동작하는 실행 파일을 만들려고 한다면 다음과 같이 CC 매크로
의 정의 부분만 간단하게 고치면 된다.
CC = arm-丄inux-gcc

매크로를 사용하지 않았다면 위와 같이 간단하게 끝나지는 않았을 것이다. 기술 파일
내에 gcc 가 사용된 모든 부분을 일일이 찾아내 arm-linux-gcc로 바꿔야 했을 것이다.
매크로를 정의해 사용하는 일은 융통성 있는 기술 파일을 만들기 위해 필요한 일이며,
독자는 적재적소에 매크로를 사용해 융통성 있는 기술 파일을 만들 수 있다.
어디에든 “반드시”라는 단어는 존재하지 않으며, 독자가 판단하기에 매크로를 사용하기
적절한 곳이라면 매크로를 사용하면 된다. 매크로를 사용하는 데 있어 매우 간단한 규
칙이 있다. 이 규칙만 알면 여러분은 얼마든지 매크로를 사용할 수 있다.

I 매크로 작성 기본 규칙
1. 매크로의 정의는 를 포함하는 하나의 문장이다.
NAME 노 = s~tring
매크로 이름

‘=’의 좌측에는 매크로 이름이 오고 우측에는 정의 문자열이 온다. 관습적으로 매크
로 이름은 대문자를 사용한다.

2. ‘#’은 주석문의시작이다.
NAME = string # 주석

542

5부_ 프로젝트 빌드

===== PAGE 544 =====
3. 여러 행을 사용할 때는 ‘\’를 사용한다.
NAME = _____ ___________ ____ -DMODULE -W -Wall \
—DNO_DEBUG

위 문장은 다음 문장과 동일하다.
NAME = _____ ___________ ____ -DMODULE -W -Wall -DNO_DEBUG

4. 매크로를 참조할 때는 괄호나 중괄호를 둘러싸고 앞에 ‘$’를 붙인다.
NAME = string
${NAME}
$(NAME)
${NAME}.c
macro_${NAME}

#
#
#
#

string
string
string.c
macro_string

중괄호나 괄호 둘에는 미묘한 차이가 있지만 둘 다 사용해도 무방하다. 단지 중괄호
는 셸에서 환경 변수 치환에도 사용되기 때문에 셸 환경 변수와의 구분을 위해 괄호
의 사용을 권장하는 편이다.

5. 정의되지 않은 매크로를 참조할 때는 n네 문자열로 치환된다.
NAME = string
my $ (NAME)
my $ (NO_DEFINE)

# my string으로 치환된다.
# my로 치환된다 (NO_DEFINE은 정의되지 않음) .

6. 중복된 정의는 최후에 정의된 값을 사용한다.
NAME
= stringA
NAME
= stringB
$ (NAME) # stringB로 ：치환된다.

7. 매크로 정의 시 이전에 정의된 매크로를 참조해 정의할 수 있다.
NAME
NAME2

= string
= my $ (NAME) # NAME2는 my string으로 정의됨

8. 여러 대입 기법을 사용할 수 있다.
NAME1 =
string
NAME2 :=string # (2)
NAME2 +=
string
NAME3 ?=
string

# (1)
# (3)
# (4)

(1)번과같은 경우를 재귀적 확장 매크로라 하고, (2)번과 같은 경우를 단순 확장 매
크로라 한다. 둘 다 위와 같이 정의할 때는 나중에 string으로 치환된다. 그러나 다음
과 같이 여러 번 참조하는 형태로 할 때는 이야기가 달라진다.

11장_ m 자〈e543

===== PAGE 545 =====
〔예제 11-4〕 매크로 대입 표기의 차이 1

A
B
C

= $ (B) BB
= $(C) CC
=D

a
b
c

:= $(b) bb
:= $(c) cc
:= d

all :
@echo $ (A)
@echo $(a)

# 명령 앞의 @는 명령을 출력하지 않고
# 결과만 출력하고자 할 때 사용한다.

위와 같이 작성하고 make 명 령을 내리면 다음과 같은 출력 결과가 나온다.

[그림 11-6] make 명령 결과

‘=’를 사용한 A 매크로는 먼저 $(B) BB로 치환된다. 다시 $(B) BB에서 $(B)가 $(C)

CC로 치환되어 $(C) CC BB로 치환된다. 마지막으로 $(C)가 D로 치환되어 최종적
으로 D CC BB로 치환된 것을 확인할 수 있다.
반면 를 사용한 a 매크로는 bb 만 치환되고 나머지는 치환되지 않았다. 그 이유는
‘=’를 사용한 재귀적 확장 매크로는 여러 번 스캔되면서 재귀적으로 확장이 일어나
는 반면 는 단 한 번 위에서 아래로 스캔되면서 확장이 일어난다. 그러므로 당연
히 b 매크로는 a 매크로를 정의하기 이전에 정의되지 않았기 때문에 null 문자로 치
환된 것이다. 다음과 같이 작성하면 두 매크로 대입법은 같은 결과를 가져온다.
〔예제 11-5〕 매크로 대입 표기의 차이 2

C
B
A

=D
= $(C) CC
= $(B) BB

c
b
a

:= d
:= $(c) cc
:= $(b) bb

all :
@echo $(A)
@echo $ (a)

544

5부—프로젝트빌드

# 명령 앞의 @는 명령을 출력하지 않고
# 결과만 출력하고자 할 때 사용한다.

===== PAGE 546 =====
if* root@server：/work/book/utils_new/nwke4
[rootOseruer make4]# make
D CC BB
d cc bb
[root@server make4]tt |

[그림 11-7] make 명령 결과

위의 경우라면 a 매크로도 한 번의 스캔으로 모두 확장 가능하기 때문에 A 매크로와
같은 결과를 가져오는 것을 알 수 있다. ‘=’를 사용하던지 를 사용하던지 독자의
마음이다. 단, 알고서 사용하면 된다.

(3)번과 같은 ‘+=’는 기존의 매크로에 공백을 두고 현재의 문자열을 덧붙인다. 그래
서 다음과 같은 결과가 나온다.
NAME2 := stringl
NAME2 += string2 # stringl string2로 치환된다.

(4)번의 ‘?=’는 현재 정의하는 매크로가 정의되어 있지 않았을 때 정의한다.
NAME1 = my
NAME1 ?= stringl # NAME1 이 앞에 정의되어 있기 때문에
# 이 절은무시된다.

NAME2 ?= string2 # string2로 정의된다.

지금까지 매크로 작성에 있어서 알아야 할 규칙을 알아보았다. 이제 독자는 매크로를
사용해 좀 더 직관적이면서 융통성 있는 기술 파일을 작성할 수 있을 것이다. 단, 다음
부터 설명할 매우 간단한 주의 사항만 습득하면 매크로를 사용하는 데 있어서 막힘이
없을 것이다.

I 매크로 사용 시 주의 사항
1. 구분을 위해 문자열에 따옴표를 넣으면 따옴표 또한 문자열의 일부로 인식한다.
NAME = "string"
$ (NAME)

# string이 아니라 "string"으로 치환된다.

프로그래머가 매크로를 사용함에 있어서 실수할 수 있는 요소 중 하나가 C 프로그래
밍에서 문자열은 따옴표로 표기하기 때문에 매크로를 사용할 때도 습관적으로 따옴
표로 표기하는 것이다. C의 매크로와 마찬가지로 make 매크로 역시 파상해 그 의미
를 해석하지 않고 단순히 치환됨에 주의해야 한다.

11장_ make 545

===== PAGE 547 =====
2. 매크로의 이름에는
NAME
NAME:2
NAME#2

=
=
=

‘#’이 들어가서는 안 되고 TAB으로 시작해서도 안 된다.

string
string
string

乂
乂
乂

당연한 이야기겠지만 ‘:’은 타겟을 정의할 때 사용되고, ‘#’은 주석의 시작을 의미하
기 때문에 사용할 수 없다. 또한 TAB으로 시작하는 라인은 기술 파일 내에서 명령라
인으로 인식되기 때문에 사용해서는 안 된다.

3. 매크로는 반드시 치환될 위치보다 먼저 정의되어야 한다.
$ (NAME)
NAME = string

4. ‘\’나

# 위에 정의되지 않았으므로 null 문자로 치환된다.

‘〉’과 같은 셸 메타 문자는 사용을 자제해야 한다.

지금까지 매크로를 사용하는 데 있어서 필요한 몇 가지 규칙과 또 주의해야 될 사항을
알아보았다. 지금까지의 내용을 바탕으로 처음 make를 시작할 때 사용한 기술 파일을
좀 더 융통성 있고 직관적이게 고쳐보면 다음과 같다.
〔예제 11-6〕 Makefile

CC
CFLAGS
TARGET

= gcc
= -W -Wall
= diary

al丄 : $(TARGET)
$(TARGET) : memo.o calendar.o main.o
$(CC)
$(CFLAGS)
-o
$(TARGET)

memo.o

calendar.o

main.o

memo.o : memo.c
$(CC) $(CFLAGS) -c -o memo.o memo.c
ca丄endar.o : calendar.c
$(CC) $(CFLAGS) -c -o calendar.o calendar.c
main.o : main.c
$(CC) $(CFLAGS)

-c

-o

main.o

main.c

clean :
rm -rf *.o diary

위와 같이 작성하고 make 명령을 수행해 보면 처음과 같은 결과가 나옴을 확인할 수
있다.
546

5부_ 프로젝트빌드

===== PAGE 548 =====
珍 root@server：,work/book/utils_new/make
[root@seruer make]tt make clean
rn —rF *.o diar
makejtt make
[rootBseruer
gcc
-W
-Wall -c -o nemo.o meno.c
gee
-W
-Wall -c -o calendar.o calendar.c
gcc —W -Wall -c -o main.o main.c
gcc
-W
-Wall -o diary inemo.o calendar.o nain.o
[rootBseruer
make]tt |

少

［그림 11-81 컴파일 화면

I 내부적으로 정의되어 있는 매크로의 사용
지금까지 기술 파일 내에 매크로를 정의하고 정의한 매크로를 사용해 기술 파일을 작
성 했다. 매크로 사용에 있어 좀 더 간결하고 자주 사용되는 방법이 있는데, make 내부
적으로 미리 정의되어 있는 매크로를 사용하는 방법이다.

make -p 명령을 셸에서 내리면 make 내부에 정의된 매크로 리스트들이 나열된다.

［그림 11-9］ make -p 명령 입력 화면

make -p 명령을 통해 나열되는 매크로는 make 내부에 미리 정의되어 있기 때문에 정
의할 필요 없이 바로 사용할 수 있다. 가령 $（ LD） 라고 사용하면 기술 파일 내에 정의되
지 않았더라도 make 내부에 LD 매크로가 Id로 정의되어 있기 때문에 Id로 치환된다.
$（ LD）

# Id로치환

그 밖에도 CC, CXX（ C++ 컴파일러）, FC（포트란 컴파일러）와 같은 각종 컴파일러와

CFLAGS（ C 컴파일 옵션）, CXXFLAGS（ C++ 컴파일 옵션）와 같은 각종 컴파일 옵션,
11장_ make 547

===== PAGE 549 =====
MAKE, SHELL과 같이 자주 사용하는 매크로들은 make 내부적으로 미리 정의되었고,
다음과 같은 명 령으로 확인 가능하다.
make -p | grep A[[:alpha:]]*[[:space:]]*=[[:space:]]
[표 11-1] 내부적으로 정의된 매크로 리스트

548

매크로 이름

설명

기본값

AR

아카이브 관리 프로그램

ar

AS

어셈블러

as

CC

C 컴파일러

cc

CXX

C++ 컴파일러

g++

CO

RCS check out 프루그램

co

CPP

C 전처리기

cc -E

FC

포트란 컴파일러

f77

GET

sees 관련 프로그램

get

LD

링크

Id

LEX

스캐너 코드 생성기

lex

PC

파스칼 컴파일러

pc

YACC

파서 코드 생성기

yacc

MAKEINFO

Texinfo 파일을 Info 파일로 변환

mak이 nfo

TEX

TeX 문서로부터 TeX DVI 생성

tex

TEXI2DVI

Texinfo 파일을 dvi 파일로 변환 프로그램

texi2dvi

WEAVE

Web을 TeX로 변환

weave

CWEAVE

C Web을 TeX로 변환

eweave

TANGLE

Web을 파스칼로 변환

tangle

CTANGLE

C Web을 C로 변환

ctan 이 e

RM

파일을 지우는 명령

rm —f

ARFLAGS

ar 플래그

rv

ASFUXGS

어셈블러 플래그

CFUXGS

C 컴파일러 플래그

CXXFLAGS

C++ 컴파일러 플래그

COFL7XGS

RCS co 플래그

CPPFL入GS

C 전처리기 플래그

FFLAGS

포트란 컴파일러 플래그

GFLAGS

sees get 플래그

LDFLAGS

링크 플래그

LFLAGS

Lex 플래그

PFLAGS

파스칼 컴파일러 플래그

YFLAGS

Yacc 플래그

5부_ 프로젝트빌드

===== PAGE 550 =====
그리고 make 내부적으로 정의되어 있지만 make -p 명령으로 확인할 수 없는 매크로
들이 있는데, 이를 자동 매크로라 부르고 ［표 11-2］ 와 같다.
［표 11-2］ 자동 매크로 리스트

현재의 타겟보다 최근에 변경된 종속 항목 리스트

$?

（확장자 규칙에서 사용 불가）
현재 타겟의 종속 항목 리스트

$A

（확장자 규칙에서 사용 불가）
$@

현재 타겟의 이름

$<

현재 타겟보다 최근에 변경된 종속 항목 리스트
（확장자 규칙에서만 사용 가능）

$*

현재 타겟보다 최근에 변경된 현재 종속 항목의 이름（확장자 제외）
（확장자 규칙에서만 사용 가능）
현재의 타깃이 라이브러리 모듈일 때 .0 파일에 대응되는 이름

$%

(예) /temp/target: /usr/local/c/test.c
$ {@F }： 현재 target의 파일 부분(target)
$ {<F }： 현재 필요 항목의 파일 부분(teste)
$ {@D }: 현재 target의 디렉토리 부분(/temp)
$ {<D }： 현재 필요 항목의 디렉토리 부분 (/usr/local/c)

［표 11-2］ 와 같은 자동 매크로들을 이용하면 기술 파일을 좀 더 적은 양으로 표현 가능
하므로 기술 파일 내에서 자주 사용되곤 한다.
target : dependencyl.c dependency2.c
gcc -o target dependencyl.c dependency2.c

위와 같은 target의 정의절이 있을 때 명령절 내에서 아는 종속 항목 리스트로 치환된
다. 그리고 $@는 target으로 치환된다. 그러므로 위와 같은 룰 정의는 자동 매크로에 의
해 다음과 같이 기술될 수 있다.
target

:
dependencyl.c
gcc -o $@ $A

dependency2.c

자동 매크로에 의한 표기법은 매우 많이 사용되기 때문에 외워둘 필요가 있다. ©와 '의
의미가 서로 혼동될 수도 있다. ©가 과녁과 같이 생겼기 때문에 타겟이라고 외우면 한
결수월할 것이다.
$〈와 $*는 다음에 배울 확장자 규칙에서 다루기로 하고 $%는 타겟을 생성하는 데 라
이브러리가 사용될 때 라이브러리 내의 특정 함수 하나를 지정할 경우 사용하는 매크
로이지만 GNU make에서는 지원하지 않는 기능이다.

11장_ make 549

===== PAGE 551 =====
$(@F)와 $(〈F)는 타겟 정의 부분에 있어서 현재 타겟의 파일 부분과 현재 종속 항목의
파일 부분을 의미한다.
/tamp/target.o : /usr/local/c/target.c

예를 들면 위와 같은 패스를 가지는 타겟 정의 항목이 있다면 명령절 부분에서 $(@F)를
사용하면 target.o로 치환되고 $(〈F)는 targeted 치환된다. 또한 마찬가지로 $(@D)는

/temp로 치환되고 $(〈D)는 /usr/local/c로 치환된다.
내부 정의 매크로와 자동 매크로를 사용해 처음 make를 설명할 때 사용한 기술 파일
을 고쳐보면 다음과 같이 간결하게 고칠 수 있다.
(예제 11-7]

CC
CFLAGS
TARGET

Makefile

= gcc
= -W -Wall
= diary

all : $(TARGET)
$(TARGET)
:
memo.o
calendar.o
$ (CC) $ (CFLAGS) -o $@ $A
memo.o : memo.c
$(CC) $(CFLAGS)

-c

-o

$@

main.o

$A

calendar.o : calendar.c
$(CC) $(CFLAGS) -c -o $@ $A
main.o : main.c
$(CC) $(CFLAGS) -c -o $@ $A
clean :
rm -rf *.o diary

기술 파일의 모습이 다소 암호화되기는 했지만 지금까지 배운 내용으로 쉽게 이해할
수 있을 것이다. 위 기술 파일을 작성하고 나서 make 명령을 내리면 처음 설명할 때 작
성한 기술 파일과 동일한 결과가 나옴을 알 수 있다.

550 5부_ 프로젝트 빌드

===== PAGE 552 =====
艾 root@server：/work/book/utils_new/make
[rootQseruer make]tt make clean
rm —rf *.o diarj1P
[root
seruer make]tt make
gee -W -Wall -c -o neno.o meno.c
gcc -W -Wall -c -o calendar.0 calendar.c
gcc -W -Wall -c -0 main.0 nain.c
gcc -W -Wall -o diary memo.0 calendar.0 main.0
[rootSseruer make]tt |

=1므! 시

Md

(흐

Izl

[그림 11-10] 컴파일 화면

지금까지 매크로를 정의하고 매크로를 사용해 좀 더 융통성 있는 기술 파일 작성법을
알아보았다. 그리고 내부적으로 정의된 매크로와 자동 매크로를 사용해 좀 더 간결하게
기술 파일을 작성하는 요령을 익혔다. 그러나 뭔가 허전하다.
지금까지 make 의 기능으로서는 make 가 그렇게 유용한지 알 수 없을 것이다. 아직까
지는 여전히 각 오브젝트 타겟을 명시하고 각 오브젝트를 생성하기 위한 컴파일 명령
을 일일이 기술해야 했다.
이제부터 배울 내용은 확장자 규칙이다. 이 확장자 규칙을 배움으로써 독자들은 비로소

make의 강력함을 알게 되고, make가 정말 우리들의 든든한 친구임을 인식할 수 있을
것이다. 그럼 흥미진진한 확장자 규칙을 알아보자.

3 L 확장자 규칙의 사용

'：

make -p 명령으로 출력되는 내용 중 다음과 같은 내용을 볼 수 있을 것이다.
〔예제 11-8)내부적으로 정의되어 있는 확장자 규칙

%.O：%.C
#

실행할명령(내장) :

$(COMPILE.c) $(OUTPUT_OPTION) $<
%
#

.0: %.cc
실행할 명령 (내장) :

$(COMPILE.cc) $(OUTPUT_OPTION) $<
%

.0: 응.cpp

#

실행할명령 (내장) :

$(COMPILE.cpp) $(OUTPUT_OPTION) $<
%

.0: % .p

11장_ make 551

===== PAGE 553 =====
#

실행할명령(내장) :

$(COMPILE.p) $(OUTPUT_OPTION) $<
%

. o: % . f

#

실행할명령 (내장) :

$(COMPILE.f) $(OUTPUT_OPTION) $<
응.o: 응•S
#

실행할 명령 (내장):

$(COMPILE.S) -o $@ $<
# make -p로 출력되는 내용을 보면 COMPILE .xx는 각 소스들의 컴파일러 및 컴파일 옵션이 지정
되어 있는 것을 확인할 수 있고, OUTPUT_OfTION은 -o $@로 지정되어 있는 것을 확인할 수 있다.

일반적으로 *.C 파일을 오브젝트(컴파일러 -C 옵션)로 컴파일하면 그에 대응하는 *.O
파일이 만들어진다. 그리고 파일명에서 확장자 으는 컴파일러의 필수 요구 사항이다.
즉, gcc 컴파일러는 *.c 파일이 있을 때 확장자 .c를 보고 그 파일이 C 프로그래밍 소스
파일인 것을 인식한다.
그것은 컴파일러의 필수 요구 사항으로 다른 확장자를 가지는 파일을 컴파일러가 C 소
스 파일로 인식하는 것은 아니다. 가령 *.abc 파일을 gcc로 컴파일하는 것은 불가능하
다. *.abc 파일이 정상적인 C 문법으로 작성된 C 소스 파일일지라도 gcc는 *.abc를 소
스 파일로 인식하지 않는다.

C 컴파일러 외에도 이런 확장자 규칙은 C++(.cc), 포트란Cf), 어셈블러(.s), 자바(java)
컴파일러에도 각각 적용된다.
물론 gcc 같이 아예 컴파일이 안 될 정도로 엄격하게 확장자 규칙을 지키는 것도 있고
그보다 덜 한 것도 있지만 관습적, 암묵적으로 각 언어 소스에 적용되는 확장자가 정해
져 있다.

test.f 파일은 포트란 소스 파일이고 f77 과 같은 포트란 컴파일러로 f77 -c -o test.o
test.f처럼 명령을 내리면 test.o라는 오브젝트를 생성할 수 있다.
*.f 파일은 포트란 컴파일러를 이용해 *.o 파일로 만들 수 있고, *.c는 C 컴파일러를 이
용해 *.o로 만들 수 있으며, *.cc는 C++ 컴파일를 이용해 *.o로 만들 수 있다. 이런 확장
자가 가지는 규칙에 기초해 make는 사용자가 내리는 명령을 알아서 해석해 컴파일 과
정을 자동화할 수 있다.

552 5부- 프로젝트 빌드

===== PAGE 554 =====
확장자 규칙을 사용하면 독자는 매우 적은 내용의 기술 파일로 많은 일을 make에 게 맡
길 수 있다. 다음 예는 이 런 확장자 규칙을 이용해 컴파일하는 방식을 보여준다.
〔예제 11-9〕 Makefile

OBJECTS = memo.o calendar.o main.o
all : diary
diary : $(OBJECTS)
$(CC) -o $@ $A
clean :
rm -rf *.o diary

위와 같이 기술 파일을 작성하고 make 명령을 내리면 ［그림 11-11］ 과 같은 컴파일 과
정이 수행된다（ make 명령을 내리기 전에 먼저 make clean 명령으로 이전에 컴파일된
파일들을 지워야 한다）.

［그림 11-11］ 컴파일 화면

앞서 내장된 매크로의 사용 부분을 본 독자라면 CC가 정의되지 않았는데 왜《로 치환
됐는지 알 수 있을 것이다.
마치 마법과 같은 일이 일어났다. 매우 짧은 기술 파일이었는데, 컴파일 과정에서 필요
한 모든 명령이 내려진 것을 알 수 있다. 위와 같은 기술 파일을 make 는 다음과 같이
해석해 명령을수행한다.

1. 기술 파일에서 diary 를 생성하기 위해 make 는 종속 항목을 살펴보고 종속 항목
을 각각 타겟으로 설정한다.

2. diary 는 memo.o 에 의존하고 memo.o 는 만들어지지 않았으며 memo.o 를 생성
하기 위한 룰도 기술 파일에는 정의되어 있지 않다.

3. make는 확장자가 .o인 내부 확장자 규칙을 이용해 다음과 같은 기준으로 현재 디
렉토리에서 memo.o를 생성할 파일을 찾는다.

11장_ make 553

===== PAGE 555 =====
- 확장자를 제외하고 memo.o와 같은 이름이 있어야 한다. memo.c가 해당된다.
- 중요 확장자를 가지고 있어야 한다. 예) ,c .cc .cpp .c .s .S •••
- 내부 확장자 규칙에 따라 memo.o를 만드는 데 사용할 수 있어야 한다. ［예제

11-8］ 를 보면 %.o： %.c에 대응하는 확장자 규칙이 있다.
4.내부 정의 확장자 규칙의 명령 (［표 11-2］ 에서는 $ (COMPILE .c) $(OUTPUT_
OPTION) $〈)을 이용해 memo.o를 생성한다. 예) cc -c -o memo.o memo.c
내부에 정의된 확장자 규칙을 사용하면 분명 좀 더 적은 기술 파일의 내용으로 많은 일
을 할 수 있다. 그렇지만 이것만으로는 원하는 대로 컴파일할 수는 없다. 즉, 독자가 원
하는 컴파일 옵션을 사용하고 싶을 때가 있을 것이다. 그럴 때는 내부적으로 정의된 확
장자 규칙을 재정의해 사용할 수 있다.
예를 들면 디버깅 메시지를 활성화시키기 위해 컴파일러 옵션에서 -DDEBUG 옵션을
사용하고 싶을 때는 다음과 같이 확장자 규칙을 재정의한다. 물론 CFLAGS 매크로를
재정의해도 되지만 여기서는 확장자 규칙의 재정의를 설명하기 위해 예로 든 것이다.
〔예제 11-10〕 Makefile

OBJECTS = memo.o calendar.o main.o
.SUFFIXES : .o .c
%.o : %.c
# .o와 대응되는 .c를발견하면 다음 명령을 수행한다.
$(CC) -DDEBUG -c -O $@ $<
all : diary
diary : $(OBJECTS)
$ (CC) -o $@ $A
clean :
rm -rf *.o diary

기존의 Makefile에서 추가된 부분이 바로 확장자 규칙을 재정의하기 위해 추가한 부분
이다. .SUFFIXES는 특수 타겟으로 .SUFFIXES의 종속 항목은 확장자 규칙을 검사하는
데 사용되는 확장자들의 리스트다. 그러므로 확장자 규칙을 사용하려는 확장자는 먼저

.SUFFIXES 타겟의 종속 항목으로 설정해야 한다.
이전에 .SUFFIXES를 사용하지 않아도 확장자 규칙이 통용된 이유는 make 내부적으로
중요 확장자에 대해 .SUFFIXES 타겟의 종속 항목으로 이미 등록되어 있기 때문이다.

554 5부_ 프로젝트 빌드

===== PAGE 556 =====
%는 일치하는 확장자를 제외한 파일명을 의미한다. make에서 %는 일치하는 모든 문자
열을 의미하는데, 예제에서는 파일명이 일치하는 문자열이다.
확장자 규칙 정의에서 기존의 타겟을 생성하기 위한 룰과 다른 점은 $A 대신 $〈가 사용
되었다는 점이다.
자동 매크로에서 $〈와 $*는 확장자 규칙에서 사용된다고 설명하였다. t는 일반적인 타
겟을 생성하기 위한 룰에서는 사용할 수 있지만 확장자 규칙에서는 사용할 수 없다. 반
대로 $〈는 일반적인 타겟 생성 룰에서는 사용할 수 없고 확장자 규칙에서만 사용할 수
있다.
확장자 규칙을 재정의하기 위한 약간 오래된 방식은 ［예제 11-11］ 과 같다.
〔예제 11-11〕 Makefile

OBJECTS = memo.o calendar.o main.o
.SUFFIXES : .o .c

# make가중요하게 여길 확장자 리스트

.c.o :

# .o와 대응되는 .c를발견하면 다음 명령을 수행한다.
$ (CC) -DDEBUG -c -O $@ $<

all : diary
diary : $ (OBJECTS)
$(CC) -o $@ $A
clean :
rm -rf *.o diary

위 확장자 규칙을 재정의한 방법 중 하나를 사용해 make 명령을 내리면 ［그림 11-12］
와 같이 원하는 대로 컴파일됨을 알 수 있다.

硏 mot@server：/work/book/utils_new/make
[root@seruer make]tt make clean
m —rF *.o diary
[root
seruer nake]tt make
cc -DDEBUG -c -o memo.o memo.c
cc -DDEBUG -c -o calendar.o calendar.c
cc -DDEBUG -c -o main.o main.c
cc -o diary metno.o calendar.o nain.o
[root@seruer make]tt |

(흐

［그림 11 너2］ 컴파일 화면

11장_ make 555

===== PAGE 557 =====
지금까지 놀라운 확장자 규칙을 사용한 컴파일 방법을 배웠다. 그렇지만 놀라기엔 아
직 이르다. 위의 기술 파일에서는 OBJECTS 매크로에 필요한 오브젝트 파일을 명시했
다. 필요한 오브젝트 파일이 예제 소스와 같이 얼마되지 않는다면 OBJECTS 매크로에
일일이 명시해도 된다. 그렇지만 소스 파일이 100개 정도 된다면 어떻게 하겠는가? 일
일이 100개의 오브젝트 파일명을 명시하는 것도 힘들지만 개발 과정 동안 파일이 계속
들어가고 나간다면 기술 파일을 수정하는 빈도도 늘어날 것이다. 이런 경우에는 와일드
카드 매칭 기법과 대입 참조 기법을 사용하면 간단히 해결할 수 있다.
〔예제 11-12〕 Makefile

SRCS

= $(wildcard *.c) # memo.c calendar.c main.c

OBJECTS = $(SRCS:.c=.o)

# memo.o calendar.o main.o

all : diary
diary : $(OBJECTS)
$(CC) -o $@ $A
clean
:
rm -rf *.o diary

위와 같이 작성하고 make 명령을 내리면 그전에 작성한 Makefile과 동일하게 동작함
을 알 수 있다.

SRCS 매크로에서 $ (wildcard *.c) 는 현재 디렉토리에서 오와 파일명이 일치하는 파일
을 찾아 공백을 구분 문자로 SRCS 매크로에 정의한다. 결국 SRCS에는 현재 디 렉토리
에 있는 memo.c calendar.c main.c로 정의된다.
정의된 SRCS는 다시 OBJECTS 매크로에 정의되는데, $(SRCS：.c=.o)와 같은 대입 참조
기법을 통해 확장자 .c가 .o로 바뀐다. 그래서 OBJECTS는 memo.o calendar.o main.o
로 정의된다.
위와 같은 기법을 사용하면 아무리 많은 소스 파일이라도 겁날 게 없다. 위 기술 파일
에서 SRCS = *.c 라고 사용하지 않고 SRCS = $(wildcard *.c) 와 같이 사용한 이유는

SRCS = 유라고 사용하면 매크로를 정의할 때는 와일드카드 확장이 되지 않기 때문이
다(*.c 식의 와일드카드 확장은 타겟 정의절과 명령절에서만 일어난다).
그래서 SRCS 매크로는 memo.c calendar.c main.c가 정의되는 게 아니라 *.c 가 정의
되기 때문에 OBJECTS 역시 *.o 로 정의된다. $(wildcard *.c) 와 같이 사용하는 것을

556 5부_ 프로젝트 빌드

===== PAGE 558 =====
make 함수의 사용이라고 한다. GNU make 에서는 사용 가능한 함수가 여럿 있다. 그
에 대해서는 후에 따로 정리한다. 위와 같은 기술 파일은 또 다음과 같이 한 줄로 표현
할수있다.
〔예제 11-13］

Makefile

OBJECTS
$ (patsubst % . c, % . o, $(wildcard * . c) )
calendar.o main.o

memo.o

all : diary
diary : $(OBJECTS)
$ (CC) -o $@ $A
clean :
rm -rf *.o diary

위 기술 파일에서 patsubst 함수는 문자열 처리에 사용되는데, 세 번째 인자로 오는

$ (wildcard *.c) 의 결과인 memo.c calendar.c main.c 에서 공백으로 구분된 문자열들
각각에 대해 첫 번째 인자인 %.c와 매칭되는 것을 %.o로 바꾼다.
여기서 %는 확장자를 제외한 파일명을 의미한다. 그러므로 memo.c calendar.c main.c
는 memo.o calendar.o main.o로 치환된다. 함수에 대한 부분은 뒤에 따로 정리하겠다.
위 기술 파일을 가지고 make 명령을 내리면 ［그림 11-13］ 과 같이 제대로 컴파일되는
것을 확인할 수 있다.

［그림 11-13］ 컴파일 화면

지금까지 어떻게 하면 기술 파일을 좀 더 효율적으로 작성할 수 있는지 알아보았다. 지
금까지의 내용만으로도 독자들은 make의 매력에 흠뻑 취했을 거라고 생각한다. 그렇
지만 아직은 갈 길이 멀다. 좀 더 make의 매력에 취해 보기 바란다.

11장_ make 557

===== PAGE 559 =====
04 더미 타겟의 사용
앞서 make 명령을 내리기 전에 make clean 명령을 사용해 이전에 컴파일된 ,o 파일
과 최종 타겟 파일인 diary 파일을 지워주었다. 여기서 clean과 같은 타겟을 더미 타겟

(Dummy target) 또는 Phony target이라고 한다. 일반적으로 타겟으로 지정되는 것들
은 생성될 파일임에 비해 더미 타겟은 파일이 생성되지 않는 개념적인 타겟을 의미한다.
〔예제 11-14〕i

OBJECTS = $(patsubst %. c, % . o, $(wildcard *.c))
calendar.o main.o

# memo.o

all : diary
diary : $(OBJECTS)
$(CC) -o $@ $A
clean :
rm -rf *.o diary

더미 타겟은 생성되지 않기 때문에 clean 타겟의 rm -rf *.o diary 명령은 make clean
명령 시 매번 수행된다. 더미 타겟은 재귀적으로 make 를 사용할 때 사용하기도 하고
또 매번 수행해야 될 룰을 정의할 때 사용하기도 한다.

5 L 명령 사용 규칙
지금껏 명령을 사용하는 데 아무런 제약 없이 사용하였다. 그렇지만 명령 사용에 있어
서도 몇 가지 간단한 규칙이 있다. 이런 규칙을 모른다면 정말 낭패를 볼 수도 있다.
echo :
@echo "test! ’’

위와 같은 룰이 있을 때 make echo 명령을 내리면 make 는 내부적으로 새로운 셸을
띄우고 다음과 같이 명령을 내린다.
/bin/sh -c echo "test!”

558

5부_ 프로젝트 빌드

===== PAGE 560 =====
여기서 새로운 셸을 띄운다는 것이 중요한데, 다음과 같은 룰이 있을 때 make del 명령
을 내리면 땅을 치고 통곡할 일이 벌어질지도 모른다.
d은1 :
cd ./backup
rm -rf*

원래 의도는 ./backup 디렉토리의 모든 파일을 지우려고 하였으나 실제로는 현재 디
렉토리의 모든 파일을 지운다. 이유는 두 명령이 서로 다른 셸에서 수행되기 때문이다.
그래서 원래 의도대로 실행시키려면 다음과 같이 세미콜론（；）을 이용해 한 줄에 작성해
야한다.
del :
cd ./backup; rm —rf*

셸에서 세미콜론（;）은 명령의 끝을 의미한다. 그래서 한 라인으로 두 명령을 표현할 수
있는 것이다. 그렇지만 위 명령절도 문제가 있다. backup 디렉토리가 현재 디렉토리에
없다면 어떻게 되겠는가? cd ./backup 명령은 실패할 것이고 결국 현재 디렉토리의 모
든 파일을 지울 것이다. 이런 경우에는 세미콜론（；） 대신 &&를 사용한다.
del :
cd ./backup && rm -rf*

&&는 앞의 명령이 성공했을 때 뒤에 오는 명령을 수행하라는 의미다.
위의 echo 룰에서 echo 명령 앞에 ‘@’를 붙인 이유는 명령 에코 기능을 끄기 위해서
다. 명령 에코 기능이란 명령을 수행할 때 수행되는 명령을 보여주는 기능인데 ‘®’를
붙이지 않으면 echo 명령도 출력되고 명령의 결과도 출력되어 다음과 같이 되기 때문
에 를 붙여 준 것이다. 다음 그림은 를 붙여주지 않은 예로, 명령 수행 결과 이전
에 명령이 출력된 것을 확인할 수 있다.

[그림 11-14] make echo 명령 수행 결과

모든 명령에 대한 명령 에코 기능을 끌려면 다음과 같은 특수 내장 타겟을 사용한다.
.SILENT :

11장_ make 559

===== PAGE 561 =====
.SILENT 타겟은 특수 내장 타겟으로, .SILENT 타겟에 등록된 종속 항목에 수행되는
명령들은 에코 기능을 끄기 때문에 수행되는 명령이 화면에 출력되지 않는다.
전체 수행 명령에 대한 에코 기능을 끄려면 위와 같이 타겟만 명시한다. 특수 내장 타
겟은 뒤에 따로 설명한다.
리눅스에서 C 프로그래밍을 해 본 독자라면 main() 함수의 리턴 값이 integer 값이 아
니라면 즉, void main() {}이라면 컴파일 시 경고가 뜨는 것을 경험했을 것이다.
그럼 main() 함수에서 리턴되는 값은 어디에서 쓰이는 것일까? main() 함수에서 리턴
되는 값은 그 함수를 fork() 해 수행시킨 부모 프로세스가 wait() 시스템 콜을 호출할
때 부모 프로세스에 전달된다.
쉽게 이야기하면 cat file.txt 명령을 수행했을 때 명령을 받은 셸은 forkO 시스템 콜
로 자식 프로세스를 생성하고 그 자식 프로세스가 execv() 시스템 콜로 cat 명령을
수행한다.

file.txt 파일이 있고 읽기 권한이 있다면 cat 명령은 정상적으로 수행될 것이다. 통상
C 프로그램에서 정상적으로 수행되었을 경우 return 0；을 한다. 그러나 file.txt 파일이
없어 정상적으로 수행되지 못했다면 0이 아닌 다른 값을 리턴할 것이다.
이것은 유닉스 프로그래밍의 오랜 관례로 자식 프로세스가 정상적으로 수행되었는지
부모 프로세스가 확인하는 데 이용된다. 셸에서 바로 직전 명령 수행 후 리턴 값을 보
려면 다음과 같이 echo $? 명 령으로 확인할 수 있다.
root@server：/work/book/utils_new/make
[root@seruer
inake]tt
this is file.txt?
[root@server make]tt
[root@seruer make]tt echo $?
0______________________ _
[root@seruer make]tt |

cat

File.txt

[그림 11-15] cat 명령이 정상적으로 수행된 후에 001 리턴된 상황

왜 root@server：/work/book/utils_new/make
[rootBseruer make]tt cat File.txt
cat: File.txt: 그런 파일이나 디렉토리가 없음
[root@server make]tt_________________
[rootSseruer make]tt echo $? I
[rooteseruer make]tt

[그림 11 너6] cat 명령이 정상적으로 수행된 후에 1이 리턴된 상황

560

5부_ 프로젝트 빌드

_싀마쓰

===== PAGE 562 =====
make는 명령 한 행을 수행 후 매번 리턴 값을 체크해 0이 아닌 값이 리턴된 경우 수행
을 종료한다. 명령이 비정상적으로 수행되어 0이 아닌 값이 리턴되더라도 make 수행을
계속하려면 명령 앞에 다음과 같이 ‘-’를 붙여야 한다. 때문에 다음 예제 기술 파일을 이
용해 make cat 명령을 내리면 file.txt 파일이 있건 없건 echo done 명령이 수행된다.
‘-’를 붙이지 않았더라면 file.txt 파일이 없었을 때 make 는 cat file.txt 명령의 리턴 값
이 0이 아니므로 echo done 명 령을 수행하지 않고 중단했을 것이다.
cat :
-cat
file.
@echo done

txt

기술 파일 전체에 대해 명령 오류를 무시하고 싶다면 다음 행을 추가한다.
.IGNORE :

.IGNORE 역시 특수 내장 타겟으로 .IGNORE의 종속 항목에 등록된 파일에 수행하는
명령은 오류가 발생해도 무시한다. 모든 명령 오류를 무시하고 싶으면 위와 같이 종속
항목 없이 타겟만 지정한다.
마지막으로 명령 사용에 있어 주의할 점은 셸 변수의 사용이다. 기술 파일 내에서 셸
변수를 참조하려면 $$｛변수명｝과 같이 ‘$’ 기호를 두 개 붙여주고 중괄호로 묶거나 “$$
변수명 ”과 같이 괄호를 붙이지 않는다.
〔예제 11-15〕 Makefile

OBJECTS = $(patsubst % . c, %.o, $(wildcard *.c))

# memo.o

calendar.o main.o
all : diary
diary : $(OBJECTS)
$(CC) -o $@ $A
cp -f diary $${HOME} # 사용자의 홈 디렉토리로 diary를 복사한다.
clean :
rm -rf *.o diary

셸 변수를 사용할 때는 기술 파일 내부에 셸 스크립트를 사용하는 데도 유의해야 한다.

11장_ make 561

===== PAGE 563 =====
다음과 같이 셸 스크립트를 사용하려면 $$ 기호를 두 개 붙여야 한다.
echo_name :
for NAME in woos test; do echo $${NAME}; done
# , $ ’ 를 하나만 붙인다면 macro로 인식하기 때문에

# NAME이 매크로로 정의되어 있지 않으면 null 문자로 처리된다.

C6 재귀적 make의 사용
지금까지 배운 것을 토대로 프로젝트를 수행하는 데 문제는 없을 것이다. 그러나 프로
젝트 규모가 커진다면 소스를 여러 디렉토리에 나누어 관리하는 것이 한결 수월하다.
여러 디렉토리로 나누어진 소스를 make로 관리하는 기법에는 기술 파일 내부에서 일
일이 경로를 지정하는 방법과 VPATH를 사용하는 방법, 마지막으로 재귀적인 make 사
용법이 있다.
경로를 지정하는 방법보다는 VPATH나 재귀적 make의 사용이 훨씬 효율적이고 유연
하다. 그러나 WATH는 파일명에 종속되는 경향이 있어 보통은 재귀적으로 make를 많
이 사용한다.

[그림 11-17] 디렉토리. 파일 트리 구조

위와 같은 구조로 소스 파일이 있을 때 최상위 디렉토리에는 Makefile 만 있고 나머
지 소스들은 각자 자신만의 소스 디렉토리에 흩어져 있는 것을 확인할 수 있다. 가령

562

5부—프로젝트빌드

===== PAGE 564 =====
memo.c 파일은 memo 디 렉토리에 있고, main.c 파일은 main 디 렉토리에 있다. 또한
각 디렉토리는 include 디렉토리만 제외하고 모두 자신들의 Makefile을 가지고 있다.
각 디 렉토리에 있는 Makefile은 다음과 같이 모두 동일하다.
〔예제 11-16〕 main/Makeflle, memo/Makefile, calendar/Makefile

OBJECTS = $(patsubst %.c, %.o, $(wildcard *.c))
CFLAGS = -I../include
all : $ (OBJECTS)
cp -f $A ../
clean :
rm -rf *.o

최상위 디렉토리의 Makefile은 다음과 같다.
〔예제 11-17〕 최상위 Makefile

all : calendar.o main.o memo.o
$ (CC) -o diary $A
calendar.o :
cd calendar && make
main.o :
cd main && make
memo.o :
cd memo && make
clean :
cd memo && make clean
cd calendar && make clean
cd main && make clean
-rm -rf *.o diary

위와 같을 때 최상위 디렉토리에서 make 명령을 내리면 ［그림 11-18］ 과 같이 컴파일
된다.

11장_ make 563

===== PAGE 565 =====
푸 root@server：/work/book/utils_new/make
[root@seruer make]tt make
cd calendar && make
make[1]: Entering directory '/work/book/utils_new/nake/calendar
cc -I../include -c -o calendar.o calendar.c
cp -F calendar.o ../
make[1]: Leaving directory '/work/book/utils_new/make/calendar’
cd main && make
make[1]: Entering directory '/work/book/utils_new/make/nain1
cc -I../include -c -o nain.o main.c
cp -F main.0 ../
make[1]: Leauing directory '/work/book/utils_new/make/main'
cd memo && make
make[1 ]: Entering directory '/work/book/utils_new/niake/memo1
cc -I../include -c -o memo.o memo.c
cp -f mono.o ../
make[1]: Leauing directory '/work/book/utils_new/nake/memo1
cc -o diar^ calendar.o main.o memo.o
[rootBseruer make]It
[root@seruer make]!* Is diary
diary
[rootdseruer make]tt |

[그림 11 너8] make 명령 수행 결과

위 Makefile을 해석해 보면 다음과 같다. 먼저 make는 all 타겟을 만나는데, all 타겟을
생성하려면 종속 항목으로 calendar.o main.o memo.o와 같은 타겟들이 있다.
먼저 calendar.o를 생성하기 위한 룰로 가면 calendar.o는 종속 항목이 없기 때문
에 바로 cd calendar && make 명령이 수행된다(cd calendar && make 명령 대신

make -C calendar 명 령을 人｝용해도 된다).
&& 기호는 이전에 설명했듯이 cd calendar 명령이 정상적으로 수행되었을 때 뒤에
오는 make 명령을 수행한다는 의미다. 결국 calendar 디렉토리 내에서 make 명령이
수행되는데, calendar 디 렉토리에 있는 Makefile을 읽어 수행하면 cc -I../include -c

-o calendar.o calendar.c 명령이 수행된 후 cp -f calendar.o ../ 명령에 의해 상위 디
렉토리로 복사된다.
마찬가지로 main.o memo.o 타겟 역시 calendar.o와 같이 각각의 디렉토리 내에서

make 명령을 수행한다. 종속 항목의 컴파일이 끝났으면 마지막으로 all 타겟의 명령라
인인 $(CC) -o diary $A가 수행되면서 최종적으로 diary 파일을 생성한다.
위에서 사용한 기술 파일은 독자의 이해를 돕기 위해 작성한 파일이고, 보통 다음과 같
은 기술 파일을 사용해 재귀적 make를 구현한다.

564 5부— 프로젝트 빌드

===== PAGE 566 =====
(예제 11-18)

TARGET
SUBDIRS
OBJS

최상위 Makefile

= diary
= calendar main memo
= calendar/built-in.o main/built-in.o memo/built-in.o

all : compile $(OBJS)
$(CC) $(OBJS) -o $(TARGET)
compile :
@for dir in $(SUBDIRS); do \
make -C $$dir || exit $?; \
done
clean:
@for dir in $(SUBDIRS); do \
make -C $$dir clean; \
done
rm -rf *.o *.i *.s $(TARGET)

〔예제 11-19〕I，calendar main memo 디렉토리 Makefile

TARGET
OBJS
CFLAGS

:= built-in.o
:= $(patsubst %.c, 응.o, $(wildcard *.c))
:= -I../include

all : $ (OBJS)
$(LD) -r $(OBJS) -o $(TARGET)
clean :
rm -rf *.o $(TARGET)

위 기술 파일에서 유심히 보아야 할 것은 최상위 Makefile에서 각각의 서브디렉토리에

make 명령을 내리는 부분이다.
이전에는 오브젝트마다 타겟을 두어 따로 명령을 내렸지만 지금은 SUBDIRS 매크로에
서브디렉토리를 등록한 후 하나의 타겟에서 셸 스크립트에 의해 일괄적으로 make 명
령을 내리는 것을 확인할 수 있다. 이렇게 사용하면 기술 파일의 길이가 짧아지고 새로
운 서브디렉토리를 추가할 때 용이하다.
그리고 서브디렉토리의 Makefile 을 보면 각각의 오브젝트들을 컴파일하고 $(LD)

-r $(OBJS) -o $(TARGET) 명 령을 사용해 최종적으로 built-in.o라는 재배치 가능한
오브젝트를 생성함을 알 수 있다. 이렇게 하면 서브디렉토리마다 타겟 파일명이 통일
되어 Makefile을 기술하는 데 한결 수월하다.

11장_ make 565

===== PAGE 567 =====
기술 파일들을 위와 같이 바꾸고 make 명령을 내리면 ［그림 11-19］ 와 같이 각 서브디
렉토리에 make 명령을 내리면서 정상적으로 컴파일되는 것을 확인할 수 있다.

望 root@server：/work/book/utils_new/make2
[root(흐seruer make2]tt make
make[1]: Entering directory '/work/book/utils_new/nake2/calendar'
cc -I../include -c -o calendar.0 calendar.c
Id -r calendar.0 -o built-in.o
make[1]: Leaving directory '/work/book/utils_new/u»ake2/calendar'
make[1]: Entering directory '/work/book/utils_new/make2/ii»ain'
cc -I../include -c -o main.o main.c
Id -r main.o -0 built-in.0
nake[1]: Leaving directory '/work/book/utils_new/u»ake2/main’
make[1]: Entering directory '/work/book/utils_new/nake2/ii»emo ’
cc -I../include -c -o memo.0 memo.c
Id —r memo.0 -o built-in.0
make[1]: Leaving directory '/work/book/utils_new/nake2/neno1
cc calendar/built-in.0 main/built-in.0 memo/built-in.o -o diar
[rootQseruer make2]tt
[root@server make2]tt Is diary
diary
[rootQseruer make2]tt |

으

［그림 11-19］ make 명령 수행

기존의 재귀적 Makefile에 비해 한결 깔끔해진 것을 알 수 있다. 하지만 아직까지 정말
사용하기 편하게 완전히 정리된 것은 아니다. 모자란 부분들은 차차 하나씩 채워가자.
이렇게 재귀적 make를 사용하지 않고 WATH를 사용해 여러 디렉토리를 컴파일하는
예를 간단하게 짚고 넘어가자. 최상위 디렉토리의 Makefile을 다음과 같이 수정하면

VPATH를 이용해 여 러 디 렉토리의 소스 파일을 컴파일할 수 있다.
〔예제 11-20)

죄상위 Makefile

VPATH = calendar main memo
OBJECTS = calendar.o main.o memo.o
CFLAGS = -I./include
diary : $(OBJECTS)
$(CC) -o $@ $A
clean :
-rm -rf *.o calendar/*.o main/*.o memo/*.o diary

VPATH 매크로를 지정하면 make가 소스 파일들을 찾을 때 현재 디렉토리뿐만 아니
라 VPATH에 등록된 디렉토리에서까지 소스 파일을 찾는다. 그래서 현재 디렉토리에
는 memo.c 가 없지만 memo 디렉토리에 memo.c 파일이 있기 때문에 컴파일할 때

memo/memo.c를 이용해 아무 이상 없이 컴파일된다.

566 5부—프로젝트빌드

===== PAGE 568 =====
VPATH를 이용해 여러 디렉토리에 있는 소스 파일을 컴파일할 때는 각 서브디렉토리
에 Makefileol 없어도 된다. 위 기술 파일로 컴파일하면 ［그림 11-20］ 과 같은 결과 화
면을 볼 수 있다.

[rooteseruer make2]tt make
cc -I./include -c -o calendar.o calendar/calendar.c
cc -I./include
-c -o main.o nain/main.c
cc -I./include
-c -o memo.o nemo/memo.c
cc -o diary calendar.o main.o memo.o
[root@seruer make2]tt
[rootl
server make2]tt is diary
diary
[root@seruer make2]tt |

그

［그림 11-201 make 명령 수행 결과

재귀적 make를 사용할지 VPATH를 사용할지 여부는 독자의 자유다. 그렇지만 대부분
의 경우 파일명에 종속적이지 않는 재귀적 make를 많이 사용한다. VPATH는 파일명에
종속적이기 때문에 다른 디렉토리라도 파일명이 같아서는 안 된다.

| 서브 Makefileoil 대한 매크로 전달
현재의 Makefile은 최상위 Makefile과 서브디렉토리의 Makefile이 아무런 연관이 없
다. 그렇지만 최상위 Makefile에서 지정한 매크로를 서브디렉토리의 Makefile로 전달
하고 싶을 때가 있을 것이다. 지금의 상황으로는 컴파일러로 으가 사용된다.
유를 gcc（사실 리눅스에서（오나 gcc나 같은 것이다）로 바꾸고 싶다고 해서 최상위

Makefile에 CC = gcc라는 매크로를 추가하면 diary 타겟에 대한 룰만 gcc로 변경되고
나머지 서브디 렉토리에서는 cc가 사용된다.
그럴 때는 export 키워드를 사용한다. ［예제 11-21］ 의 Makefile과 같이 어느 한 매크
로만 서브 Makefile에 전달하고 싶으면 매크로 앞에 export 키워드를 붙여준다.
모든 매크로에 대해 전달하고 싶으면 export 키워드를 단독으로 써준다.
〔예제 11-21〕

TARGET
SUBDIRS
OBJS
)export CC

:= diary
:= calendar
main memo
:= calendar/built-in.o main/built-in.o memo/built-in.o
:= gcc|

all : compile
$(OBJS)
$ (CC) $(OBJS) -o $(TARGET)

11 장— make 567

===== PAGE 569 =====
compile :
@for dir in $(SUBDIRS); do \
make -C $$dir || exit $?; \
done
clean:
@for dir in $(SUBDIRS); do \
make -C $$dir clean; \
done
rm -rf *.o *.i *.s $(TARGET)

［예제 11-21］ 과 같이 export 키워드로 정의된 매크로는 서브 Makefile에도 전달된다.
그래서 컴파일해 보면 다음과 같이 cc가 모두 gcc로 바뀐 결과 화면을 볼 수 있다.
모으 root@server：/work/book/utils_new/make2
[root@seruer make2]tt make
make[1]: Entering directory '/work/book/utils_new/make2/calendar'
[-1../include -c -o calendar.o calendar.c
r calendar.o -o built-in.o
nake[1]: Leauing directory '/work/book/utils_new/nake2/calendar'
[1]: Entering directory '/vjork/book/utils_new/nake2/main1
gcc |-I../include -c -o main.o main.c
id -r main.o -o built-in.o
make[1]: Leauing directory '/work/book/utils_new/n)ake2/main'
make[1]: Entering directory '/work/book/utils_new/make2/meno’
-I../include -c -o memo.o nemo.c
r memo.o -o built-in.o
nake[1]: Leauing directory '/work/book/utils_new/nake2/nemo1
gcc calendar/built-in.o main/built-in.o neno/built—in.o -o diary
[root
server make2]tt |

쁘쓰

(흐

［그림 11-21］ make 명령 수행 결과

지금까지 배운 내용만 알아도 프로젝트를 하는 데 크게 어려움은 없을 것이다. 이제부
터는 조건부 수행과 함수 사용법 등을 배워보자.
조건부 수행과 함수 사용법은 GNU 프로젝트 또는 kernel Makefile 등에서 많이 사용
되고 있기 때문에 그런 프로그램들의 소스 구조와 컴파일 환경을 알려면 알아 둘 필요
가 있다. 또한 조건부 수행 방법과 함수 사용법은 좀 더 효율적인 기술 파일을 작성하
는 데 도움을 준다. 그렇지 만 갈 길이 급한 독자라면 이 부분을 건너뛰 고 autoconf부터
보아도 무방하다. 결국 나중에 다시 보겠지만 지금까지 배운 것만으로도 당장 프로젝트
를 수행하는 데는 아무런 지장이 없을 것이다.

568 5부_ 프로젝트빌드

===== PAGE 570 =====
07 L 조건부 수행
C에서 if ~ else문이 있다면 make에는 ifeq ~ else ~endif문이 있다.
all :
ifeq ($(CC),gcc)
# 내부 정의매크로 CC 는 cc 로 되어있다.
Qecho "C 컴파일러는 GNU gcc입니다. "
else
@echo HC 컴파일러는 $ (CC) 입니다" # 이 부분이 수행된다.
endif

위와 같은 기술 파일을 작성하고 make 명령을 수행하면 else 부분의 명령이 수행
된다. 그 이유는 내부에 정의된 매크로 CC가 으로 정의되어 있기 때문이다. ifeq

($(CC),gcc)는 $(CC)가 gcc인가를 판단한다. 그렇다면 @echo “C 컴파일러는 GNU
gcc입니다.”가 수행되고 그렇지 않다면 @echo “C 컴파일러는 $(CC)입니다”가 수행된
다. 반드시 끝은 endif로 끝나야 한다. null 문자를 비교하려면 ifeq ($(CC),)처럼 사용
한다. 또한 다음과 같이 else 문장은 없어도 된다.
all :
ifeq ($(CC),)
@echo "C 컴파일러는 GNU gcc입니다."
endif
@echo "end”

같지 않은지 비교하고 싶다면 ifneq ~ else ~ endif문을 사용한다. ifeq와는 반대로
명령이 수행되는 것 외에는 ifeq와 다르지 않다.
al丄 :
ifneq ($(CC),gcc)
@echo HC 컴파일러는 GNU gcc입니다. "
else
@echo "C 컴파일러는 $(CC) 입니다."
endif

# $ (CC) 가• gcc 와 같지않다면?
# 이 부분이 수행된다.

ifeq문과 ifneq문은 다음 예와 같이 리눅스 커널 Makefile 내에서 사용자가 make
menuconfig 시 지정한 커널 옵션으로 파일이나 디렉토리를 선택적으로 매크로에 추
가할 때 많이 사용한다.

11장_ make 569

===== PAGE 571 =====
ifeq ($(CONFIG_ARCH_CLPS7500),y)
SUBDIRS
十= drivers/acorn/char
CLPS_ADDR
= 0xc0000800
endif

ifdef ~ else ~ endif문은 매크로가 정의되었는지 되지 않았는지에 따라 Makefile을
다르게 구성할 때 사용한다.
all :
ifdef CC
@echo "CC 매크로는 정의되어 있습니다. "
else
@echo "CC 매크로는 정의되지 않았습니다. "
endif

# CC가정의되어 있다면?
# 이 부분이 수행된다.

반대로 ifndef ~ else ~ endif 문은 매크로가 정의되지 않을 때 수행되는 문장을 정의
하고, 기본 사용법은 ifdef문과 같다.
all :
ifndef NO_DEFINE
# $ (NO_DEFINE) 이 정의되어 있다면?
@echo "NO_DEFINE 매크로는 정의되지 않았습포다. ”
else
@echo "NO_DEFINE 매크로는 정의되었습니다."
endif

8 함수의 사용
make는 기술 파일에서 사용할 수 있는 많은 함수를 제공한다. make 함수에는 문자열
을 처 리하기 위한 함수부터 파일 관련 함수, 반복을 위 한 함수 등이 있고 매우 유용하
기 때문에 자주 사용되곤 한다.
대표적인 경우가 리눅스 커널 소스에 있는 Makefile이다. make 함수를 모르면 함수가
사용된 기술 파일을 이해하기 힘들기 때문에 사용하지는 않더라도 최소한 어떤 것이
함수라는 정도만이라도 알아야 한다.
기억할지 모르겠지만 앞에서 기술 파일을 작성할 때도 함수를 사용했었다. [예제 11-22]
의 기술 파일 내에서 $ (wildcard *.c) 부분이 make 함수의 사용 예다.

570

5부—프로젝트빌드

===== PAGE 572 =====
〔예제 11-22]

make 함수를 사용한 기술 파일

SRCS
= $(wildcard *.c) # memo.c calendar.c main.c
OBJECTS = $(SRCS:.c=.o)
# memo.o calendar.o main.o
all : diary
diary : $(OBJECTS)
$(CC) -o $@ $A

make 에서 함수는 다음과 같은 형식으로 사용된다.
$ （함수명 함수인자들）

$0 기호 내에 함수명이 오고 공백이나 탭 이후에 함수의 인자들이 오는 형태다. 함수
의 인자가 여러 개라면 콤마（,）로 구분된다. 그러면 어떤 함수가 있고 어떻게 사용하는
지 알아보자.

I 셸 명령 함수
$ （ shell 셸 명령）

shell 함수는 굉장히 자주 사용되는 함수다. shell 함수는 뒤에 오는 셸 명령을 수행하
고 결과를 리턴한다.
SRCS = $ (shell Is *.c)
echo :
@echo $(SRCS)

가령 위와 같은 기술 파일을 작성하고 현재 디렉토리에 kkk.c 파일과 기술 파일만 있는
상태에서 make echo 명령을 내리면 다음과 같이 현재 디렉토리에 있는 C 소스 파일
들의 리스트를 출력한다.
i/ root⑤server:/work/book/utils_new/make2
[rootSseruer make2]tt make echo
kkk.c
[root@seruer make2]tt |

[그림 11—22] shell 함수의 사용

11장_巾가危 571

===== PAGE 573 =====
이런 결과가 나오는 이유는 shell 함수에 의해 Is *.c 명령을 셸에 내린 결과가 SRCS
매크로에 정의되었기 때문이다.

shell 함수는 명령 수행 결과를 매크로로 정의할 때 사용할 수 있는 유일한 방법이다.
굉장히 자주 사용하는 함수니 기억하기 바란다.

| 문자열 처리 함수
► 문자열 치환 함수
$ (subst 찾을문자, 변경할문자, 목표 문자)

subst 함수는 목표 문자에서 찾을 문자를 발견하면 변경할 문자로 치환한다. 가령 다음
과 같이 사용하면 STR 매크로는 “I LIKE you.”라는 문자열로 정의된다.
STR = $(subst like, LIKE, I like you.)
echo :
@echo $(STR)

그래서 make echo 명령을 내리면 ［그림 11-23］ 과 같이 “like” 문자열이 “LIKE” 문자열
로 바뀌어 출력되는 것을 확인할 수 있다.

廢]
（ 으
（흐

raot@os：/’temp/book/make
[root
os nidkeJU make echo
I LIKE you.
[root
os make]tt |

同£3

H

［그림 11-23］ make echo 명령 결과

$ (patsubst 패턴, 변경 문자열 , 목표 문자열)

patsubst 함수는 목표 문자열에서 패턴을 발견하면 변경 문자열로 변경한다. 패턴에는
% 기호를 사용할 수 있는데, % 기호는 공백과 탭을 제외한 모든 문자열을 의미한다.
가령 “I like yo니.” 문자열이 있을 때 %ke는 “like” 문자와 일치한다.
STR = $(patsubst %.c, %.o, memo.c main.c ABCD)
echo :
@echo $(STR)

patsubst 함수는 위와 같이 많이 사용한다. 위와 같은 기술 파일을 작성하고 make
echo 명령을 내리면 ［그림 11-24］ 와 같이 출력된다.

572 5부- 프로젝트 빌드

===== PAGE 574 =====
PI root@os：/temp./book/make
[root@os makejtt make echo
meno.o nain.o ABCD
[root
os make]tt |

(흐

[그림 11—24] make echo 명령 결과

memo.c main.c ABCD 문자열에서 memo.c오｝ main.c는 패턴인 %.c와 일치하기 때문
에 %.o로 치환되고, ABCD는 패턴과 일치되지 않기 때문에 치환되지 않는다.
매크로에서 특정 패턴을 치환하려면 patsubst 함수 대신 다음과 같이 사용할 수도 있다.
$(매크로 명 : 패턴=치환할 문자열)

그래서 다음과 같은 기술 파일은 patsubst 함수를 사용해 작성한 기술 파일과 동일한
결과를 가져온다.
MACRO
STR
echo :

= memo.c main.c ABCD
= $(MACRO:%.c=%.o)
@echo $ (STR)

► 문자를 정렬하는 함수
$ (sort 문자열)

sort 함수는 인자로 오는 문자열에 대한 정렬을 수행한다. 중복되는 문자열이 있다면
하나의 문자열만 인식한다.
다음과 같은 예제 기술 파일이 있을 경우 make echo 명령을 내리면 정렬되고 중복
문자열은 하나로 통합되어 출력되는 것을 확인할 수 있다.
MACRO = bbb aaa ccc aaa ddd
STR
= $(sort $(MACRO))
echo :
@echo $(STR)

'흐] root@as ：/temp/book/make
[rooiBos make]tt make echo
aaa bbb ccc ddd
[rootl
os nake]tt |

흐

[그림 11-25] 정렬되어 출력된 결과

11장_ make 573

===== PAGE 575 =====
► 공백 문자의 제거
$ (strip 문자열)

strip 함수는 인자로 오는 문자열의 제일 앞에 사용된 공백 문자를 제거하고 각 문자 간
에 공백 문자열이 하나 이상 사용되었다면 하나로 만든다.

strip 함수에 의해 “ Ilike you. ”와 같은 문자열은 “I like you. ”로 바뀐다.
strip 함수는 ifeq 명 령으로 두 문자열을 비교할 때 많이 사용한다. 가령 다음과 같은 기
술 파일이 있을 때 strip 함수를 사용하면 유용하다.
CC = gcc[Space Bar][Space Bar][Space Bar][Space Bar][Enter]
all :
ifeq ($ (CC), gcc)
@echo UC 컴파일러는 GNU gcc입니다. "
endif

CC 매크로가 “gcc ”와 같은 공백이 포함된 gcc 문자열로 정의되어 있다면 “C 컴파일
러는 GNU gcc입니다.”라는 문자열이 출력되지 않는다.
공백의 영향을 제거하려면 다음과 같이 strip 함수를 사용한다.
CC = gcc[Space Bar][Space Bar][Space Bar][Space Bar][Enter]
all :
ifeq ($(strip $ (CC)), gcc)
@echo "C 컴파일러는 GNU gcc입니다. "
endif

► 문자필터링함수
$ (filter 패턴 , 문자열)

filter 함수는 패턴과 일치하는 문자열만을 걸러준다. 가령 다음과 같은 예가 있을 때 각
파일들은 비교 패턴에 따라 소스 파일과 헤더 파일로 분리된다.
FILES = memo.c head.h main.c asm.S diary.h
SRCS
= $ (filter %.c %.S, $ (FILES))
HEADS
= $ (filter %.h, $ (FILES))
echo :
@echo "source files : $ (SRCS) ’’
@echo "head files : $ (HEADS) ”

574

5부—프로젝트빌드

===== PAGE 576 =====
위 기술 파일 내에서 문자열은 “memo.c head.h main.c asm.S diary.h”이고, SRCS 매
크로 정의 부분에서 filter 함수에 의해 걸러질 패턴은 확장자가 .c 또는 .S 파일이다. 그
래서 SRCS 매크로에는 소스 파일인 memo.c main.c asm.S가 걸러져 정의된다.
마찬가지로 HEADS 매크로에서 필터링될 패턴은 확장자가 .h인 문자열이다. 결국

HEADS 매크로는 “head.h diary.h” 문자열로 정의된다.
0® root@os ：/temp/book./make
[rootBos nMkejlt make echo
source Files : neino.c main.c asn.S
head Files : head.h diary.h
[rootBos make]It |

[그림 11—26] filter 함수에 의한 필터링 결과

$ (filter-out 패턴 , 문자열)

fflter-out 함수는 filter 함수와 반대로 패턴과 일치하지 않는 문자열만 걸러준다. 그래
서 위 기술 파일에서 filter 함수를 filter-out 함수로 변경해 make echo 명령을 내리면
다음과 같이 소스 파일과 헤더 파일이 바뀌어 출력되는 것을 확인할 수 있다.
H root@os ：/temp/book/make
[rootBos
make echo
source files : head.h diary.h
head files : neno.c main.c asn.S
[roomos make]it |

[그림 11-27] filter-out 함수에 의한 필터링 결과

► 특정 문자열을 찾는 함수
$ （ findstring 찾을 문자열, 대상 문자열）

findstring 함수는 대상 문자열에서 찾을 문자열을 찾는다. 그래서 찾으면 찾을 문자열
을 리 턴하고, 못 찾으면 null 문자를 리턴한다.
STR = aaa bbb ccc
echo :
@echo bbb : $ (findstring bbb, $ (STR))
@echo kkk : $ (findstring kkk, $ (STR))

그래서 위와 같은 기술 파일을 작성하고 make echo 명령을 내리면 다음과 같은 결과
를 확인할 수 있다.

11장_ make 575

===== PAGE 577 =====
W root@os：/temp/book/make
[roottdos make]tt make echo
bbb : bbb
kkk :
[root드os make]tt |

러|可피

M

[그림 11-28] findstring 함수의 사용

위 상황은 bbb 문자열의 경우 aaa bbb ccc 문자열 내에서 발견할 수 있기 때문에

bbb를 리턴했지만 kkk 문자열은 찾을 수 없기 때문에 mill 문자를 리턴한 상황이다.
$ (words 문자열)

words 함수는 문자열에서 사용된 단어의 개수를 리턴한다. 그래서 $ (words aa bb
cc)와 같이 사용되면 3을 리턴한다.
$ (word n, 문자열)

word 함수는 문자열에서 n번째 단어를 리턴한다. $(word 2, I like yo니.)하면 “I like
you； 문자열에서 두 번째 단어인 “like”를 리턴한다.
$ (wordlist 시작 번호, 끝 번호, 문자열)

wordlist 함수는 시작 번호부터 끝 번호까지의 단어들을 리턴한다. 예를 들면
$ (wordlist 2, 4, aa bb cc dd ee) 라고 사용하면 두 번째 단어 인 bb부터 4번째 단어 인
dd까지 bb cc dd가 리턴된다.
$ (firstword 문자열 )

firstword 함수는 문자열에서 첫 번째 단어를 리턴한다. 그래서 $(firstword I like
you.)와 같이 사용하면 첫 번째 단어 인 I를 리턴한다.
$ (join 문자열, 문자열)

join 함수는 앞의 문자열과 뒤에 오는 문자열을 합쳐 하나의 문자열로 만들어낸다. 가
령 $(join src asm, .c .S) 와 같이 사용하면 src.c asm.S를 리턴한다. 앞에 오는 문자열
의 단어 개수와 뒤에 오는 문자열의 개수가 맞지 않다면 뒤에 남는 단어는 합치지 않고
따로 출력한다.

576 W_ 프로젝트 빌드

===== PAGE 578 =====
I 파일 이름 관련 함수
$ （ dir 문자열）

dir 함수는 문자열에서 디렉토리 부분만 추출한다. 다음과 같은 기술 파일이 있을 때 make
echo 명령을 내리면 문자열의 디렉토리들만추출되어 나오는 것을 확인할수 있다.
PATHS = /bin/ls /sbin/ifconfig memo/memo. c Makefile
echo :
@echo $（ dir $（ PATHS） ）

［그림 11—29］ dir 함수의 사용

$ （ notdir 문자열）

notdir 함수는 dir 함수와 반대로 디 렉토리가 아닌 부분만 추출한다. 그래서 위 기술 파
일에서 dir 함수를 notdir 함수로 바꾸고 make echo 명령을 내리면 ［그림 11-30］ 과
같은 결과를 확인할 수 있다.
혜 root@os：/temp/book/make
[rootWos makeJtt make echu
Is ifconfig memo.c Makefile
[rootdos make]It |

［그림 11—30］ notdir 함수의 사용

$ （ suffix 문자열）

suffix 함수는 문자열에서 확장자만 추출한다. 그래서 다음과 같은 기술 파일이 있다면
make echo 명령으로 확장자만 출력되는 것을 확인할 수 있다.
FILES = src/memo.c asm/asm.S for.f Is /etc/resolv.conf
echo :
@echo $ (suffix $ (FILES))

폐 root@os：/temp/book/make
[rut)ll<>os make JII ma kt* echo
.c .S .F .conf
[rootQos make]

휴|

［그림 11—31］ suffix 함수의 사용

11 장 _ make 577

===== PAGE 579 =====
$ （ basename 문자열）

basename 함수는 문자열에서 점 (.)과 확장자를 제외한 순수한 파일명만 추출한다. 그
래서 위 기술 파일에서 suffix 함수를 basename 함수로 변경하고 make echo 명령을
내리면 ［그림 11-32］ 와 같이 출력되는 것을 확인할 수 있다.

廢] root@os ：/temp/book,/make
[rootWos nuikeJtt make echo
src/nemo asm/asm For Is /etc/resolu
[rootl
os make]9 |

흐

［그림 11—32］ basename 함수의 사용

$ （ addsuffix 접미사‘, 문자열）

addsuffix 함수는 문자열의 각 단어 뒤에 접미사를 붙여준다. addsuffix 함수를
$(addsuffix .c, memo main)과 같이 사용하면 문자열인 memo main에 접미사인 .c
를 각각 붙여 memo.c main.c 문자열을 리턴한다.
echo :
@echo $ （ addsuffix .c, memo main）

B root@os：/temp/bo아〈/mgke
[rootBos make]It make echo
meno.c main.c
[root@os nake]tt |

［그림 11-33］ addsufix 함수의 사용

$ （ addprefix 접두어 , 문자열）

addprefix 함수는 각 문자열에 접두어를 붙여준다. 그래서 $(addprefix src/, memo,
c main.c)하면 문자열인 memo.c main.c 각각에 접두어인 src/를 붙여 src/memo.c
src/main.c가 리턴된다.
echo :
@echo $ （ addprefix src/, memo main）

廢）ro ot@ o s:/te rnp/b o a k/m:a b e
[l ootWos make JII make et ho
src/memo src/nain
[rooteos make]tt |

[그림 11-34] addprefix 함수의 사용

578

5부_ 프로젝트빌드

===== PAGE 580 =====
I 기타유용한함수
$ (wildcard 패턴)

현재 디렉토리에서 패턴과 일치하는 파일 리스트를 뽑는다. 가령 $(wildcard *.c)라고
사용하면 현재 디렉토리에 있는 모든 .c 파일의 리스트를 리턴한다. 그리고 $ (wildcard

test.*)라고 사용하면 파일명이 test인 모든 파일을 리턴한다.
wildcard 함수는 자주 사용되기 때문에 반드시 기억할 필요가 있다.
$ (foreach 변수명 , 대 입 문자열, 확장 문자열 )

foreach 함수는 조금 특별하다. foreach 함수는 변수명에 대입 문자열을 단어별로 대
입해 넣고 그 변수를 확장 문자열에서 사용한다. 일단 예제로 알아보자.
SRCS = $(foreach str, a b c, $(str).c)
echo :
@echo $(SRCS)

위 예를 보면 변수명으로 str 이 설정되었다. 그리고 대입 문자열에 a b c 가 사용되었
다. 그러면 foreach 함수는 먼저 str 변수에 대입 문자열의 첫 번째 단어인 a 를 넣어
서 str 변수를 확장 문자열 부분에서 이용한다. 현재 str 변수에는 a 가 들어 있기 때문
에 $(str).c는 a.c를 의미한다. 그래서 먼저 a.c가 리턴된다. 그리고 b를 str 변수에 넣고

$(str).c에서 확장한다. 결국 b.c가 리턴된다. 마지막으로 c.c7} 리턴되어 최종적으로 a.c
b.c c.c가 출력된다.
圖 [screen 2： bash] root@os:/temp/book/make
저
(흐

[root
os make J It make echo
a.c b.c c.c
[root
os nake]tt |

[그림 11—35] foreach 함수에 의한 확장

현재로서는 문자열 부분에 $(str).c와 str 변수가 사용되었다. 그러나 str 변수를 반드시
사용하라는 법은 없다. foreach 함수에서 중요한 것은 단어의 개수만큼 반복한다는 것
이다. 다음 예는 세 번째 인자인 확장 문자열에서 str 변수를 사용하지 않은 예다.
SRCS = $(foreach str, a b c, TEXT)
echo :
@echo $(SRCS)

11 장_ make 579

===== PAGE 581 =====
關 [screen 2： bash] root@os ：/temp/book/make

아
（흐

[rootWos m
cejll make echo
TEXT TEXT TEXT
[root
os make]9 |

［그림 11-36］ foreach 함수에 의한 확장

확장 문자열에서 str 변수를 사용하지 않고 TEXT 문자열만 사용했기 때문에 TEXT 문
자열이 a b c 단어 개수만큼 출력된 예다.
다음은 make 매뉴얼에 있는 예제인데, foreach 함수는 주로 다음과 같이 사용되어 반
복 확장할 때 유용하다.
SRCS = $(foreach dir, . memo main calendar, $(wildcard $(dir)/*.c))
echo :
@echo $(SRCS)

위와 같은 기술 파일을 작성하면 dir 변수에 먼저 점(.)이 들어간다. 그리고 $(wildcard

./*.c)에서 현재 디렉토리에 있는 모든 C 소스 파일의 이름으로 확장된다. 그리고 두 번
째로 dir 변수에는 memo가 들어간다. dir 변수는 다시 확장 문자열에서 $(wildcard

memo/*.c)와 같이 사용되어 memo 디렉토리에 있는 모든 C 소스 파일의 이름으로
확장된다.
마찬가지로 main, calendar 디렉토리 각각에 있는 C 소스 파일의 이름으로 확장되어

make echo 명령을 내리면 ［그림 11-3刀과 같이 출력된다.
關 [screen 2： bash] root@os：/temp/book/make

V

[rootWus mdkejtt make echo
./kkk.c memo/memo.c main/main.c calendar/calendar.c
[root
os make]tt |

（흐

[그림 11-37] make echo 명령 수행

foreach 함수를 쓰는 데 특별한 주의 사항은 없다. 단지 foreach 함수 내에서 선언된
변수는 foreach 함수 내에서만 유효하다는 점을 기억하기 바란다.
$ (origin 매크로명)

origin 함수는 매크로가 어떻게 정의된 매크로인지에 관한 문자열을 리턴한다. 다음과
같은 기술 파일이 있을 때 make echo 명령을 내리면 다음과 같은 결과를 출력한다.

580

5부—프로젝트빌드

===== PAGE 582 =====
DEFINE = str
echo :
@echo
@echo
@echo
@echo

$(origin
$(origin
$(origin
$(origin

UNDEFINE)
DEFINE)
PATH)
CMDDEF)

아⑥os:/temp/boak/make

OB [screen 2： bash] ro

[rootdos make]Itjmake CMDDEF=kkk I
1,11,1............. .
undefined 1
File
enuironment
conmand line
[rooWos make]# |

[그림 11-38] make CMDDEF=kkk 명령을 내린 결과

origin 함수에 의해 UNDEFINE 매크로는 정의되지 않았기 때문에 “undefined” 문자열
이 출력되었고, 기술 파일 내에 정의된 DEFINE 매크로는 “file” 문자열이 출력되었다.
그리고 PATH 환경 변수에 대해서는 “environment” 문자열이 출력되었고 마지막으
로 make 명령을 내릴 때 정의한 CMDDEF 매크로의 경우에는 “command line” 문자
열이 출력되었다. 이렇게 origin 함수는 매크로가 어떻게 정의된 매크로인지 알고자 할
때 사용한다.

origin 함수가 리턴하는 문자열들은 ［표 11-3］ 과 같다.
［표 11-3］ origin 함수에서 리턴하는 문자열의 의미
undefined

정의되지 않음

file

기술 파일 내에서 정의된 매크로

environment

환경 변수 예） HOME. PWD

command line

make 명령 시 정의된 매크로

default

make 내부에 정의된 매크로 예） AS. CC

environment override

환경 변수

automatic

자동 매크로 예） $@, $?, …

override

override 매크로

11장_ make 581

===== PAGE 583 =====
I 함수 사용할 때 주의 사항
이상이 make에서 사용할 수 있는 함수 대부분의 설명이었다. 일단 어떤 함수들이 있는
지 알고 자신에 게 필요한 함수를 찾아 사용하면 된다. 그렇지만 함수를 사용할 때 다음
과 같은 주의 사항이 있다.
첫째. 함수는 함수를 지원하는 make에서 사용해야 된다. GNU make는 함수를 지원하
기 때문에 바로 사용할 수 있다. 그러나 지원하지 않는 make도 많이 있다.
함수를 기술 파일에서 사용하면 이미 그 기술 파일은 함수를 지원하는 make로만 종속
된다. 그래서 이식성을 해칠 수 있다. 이런 부분은 나중에 배울 automake에서 문제가
된다. automake 는 여러 기계에서 동작할 수 있는 Makefile 을 생성하는 소스 패키징
유틸리티인데 함수를 지원하지 않는다.
둘째, 함수의 인자로 콤마(,)와 공백( )을 사용할 때 주의해야 한다.
TEXT= id, pass, name
STR = $(subst $(TEXT))
echo :
@echo $(STR)

위 기술 파일의 의도는 TEXT 매크로에 정의된 id, pass, name 문자열에서 사용된 콤
마(,)를 언더바(_)로 바꾸는 것이 목적 이었다. 그렇지만 위와 같이 기술 파일을 작성하
고 make echo 명령을 내리면 의도와 다른 결과가 나옴을 확인할 수 있다.
W [screen 2： bash] root@os：/temp/book/make
[rootQos make]tt make echo
id, pass, name
[rootQos nake]tt |

［그림 11-39］ make echo 명령 결과

［그림 11-39］ 에서 볼 수 있듯이 의도와는 다르게 스 id, pass, name이 출력되었다. 그
이유는 바로 subst 함수 내에서 처음 오는 콤마(,)에 대해 찾을 문자열 콤마(,)로 인식
하지 않고 인자 구분을 위한 콤마(,)로 인식 했기 때문이다.
결국 subst 함수는 첫 번째 인자와 두 번째 인자가 없는 상태에서 세 번째 인자로 id,

pass, name 문자열이 사용되었다.
콤마(,)를 인자로 사용하려면 다음과 같이 comma 매크로를 따로 정의해 사용한다.

582

&부_ 프로젝트 빌드

===== PAGE 584 =====
comma
TEXT= id, pass, name
STR = $ (subst $(comma),$ (TEXT))
echo :
@echo $(STR)

위와 같이 기술 파일을 작성하고 다시 make echo 명령을 내리면 이제는 의도했던 대로
출력이 될 것이다.

觸 [screen 2： bash] root@os：/temp/book/make
（ 흐

[root
os iDdkeJII make echo
id_ pass_ name
[root@os make]tt |

［그림 11-40］ 콤마를 함수 인자로 사용

공백 역시 마찬가지다. 공백을 함수 인자로 사용하려면 다음과 같이 공백을 매크로로
정의하고 나서 사용해야 한다.
space
= $ (null) $(null)
TEXT
= id, pass, name
STR = $ (subst $(space),$(TEXT))
echo :
@echo $(STR)

nuU 매크로는 당연히 이전에 정의되지 않은 매크로다. 이렇게 정의되지 않은 매크로는
매크로 치환 시 null 문자열로 치환된다. 결국 nuU 문자 사이의 공백 문자만이 space
매크로로 정의된다.
이때 주의할 점은 마지막 $〔null) 뒤에는 공백을 넣어서는 안 된다는 것이다. 공백이 추
가되면 뒤에 추가된 공백만큼 space 매크로의 문자열로 정의된다. 이 렇게 space 매크
로를 정의하고 subst 함수의 인자로 넣으면 ［그림 11-41］ 과 같이 id, pass, name 문자
열 내에서 공백이 _로 치환되어 출력된다.

解 [screen 2： bash] root@os ：/temp/booK/make
（흐

[root
os makeJtt make echo
_id,_pass,_name
[root@os make]# |

［그림 11-41］ 공백 문자를 함수의 인자로 사용

11장_ make

583

===== PAGE 585 =====
9 【특수 타겟
앞에서 확장자 규칙을 새로 정의할 때 .SUFFIXES 타겟을 사용한 것이 기억날 것이다.

.SUFFKES와 같은 타겟을 특수 타겟이라 하고, 기술 파일 전체에 영향을 미칠 수 있는
make 기능을 정의할 때 사용한다. 특수 타겟의 종류와 의미는 ［표 11-4］ 와 같다.
［표 11-4］ 특수 타겟의 종류
타겟 종류

설명

.DEFAULT

m가紀가 요청된 타겟을 빌드할 룰을 기술 파일 또는 확장자 규칙에서 찾지

못하면 .DEFAULT 타겟에 기술된 명령을 수행한다.
.IGNORE

명령 수행 시 반환되는 오류 코드를 무시한다. make 명령 시 i 옵션을 준 것
과 동일하고, .기술 파일 내에서 모든 명령 앞에 ’ 기호를 붙여준 것과 동일
하다. 예） -rm -rf *.o
PRECIOUS 타겟에 기술된 파일들은 빌드 중단 신호 또는 명령라인에서 오

PRECIOUS

류가 반환되더라도 지우지 않는다.
.SILENT

명령은 실행하지만 실행되는 명령을 화면에 출력하지 않는다. -s 옵션과 동
일하고 모든 명령 앞에 를 붙인 것과 동일하다.

.SUFFIXES

.SUFFIXES 타겟에 정의된 확장자들은 중요 확장자들로, 확장자 규칙과 연관

될 수 있다.
재귀적 make 사용법에 있어 export 키워드를 단독으로 기술 파일에서 사용

.EXPORT_ALL_VARIABLES

한 것과 마찬가지로 기술 파일 내의 모든 매크로들을 하위 기술 파일에 전달
한다.

다른 타겟은 이전에 설명한 것도 있고 위 표를 읽어보면 바로 알 수 있으므로 따로 설
명하지 않고 .DEFAULT 타겟의 의미를 알아본다.
다음과 같은 기술 파일이 있을 때 기술 파일에 정의되어 있지 않은 타겟 빌드 명령인

make notarget 명령을 내리면 다음과 같은 오류 메시지를 출력하면서 make가 멈춘다.
echo :
@echo "Hei丄o, world!

醫] [screen 2： bash] rpot@os：./temp/boQk/maye

라|드I 히

[coot(Jos nidkc JU Imake notdrget
1

make: … 목표 Aiuidrgyt■'를 민들 규칙이 없음. 멈춤. ■
[root
os
|

(흐

거
[그림 11-42] make notarget 명령 수행

584

5부_ 프로젝트 빌드

===== PAGE 586 =====
그러나 다음과 같이 기술 파일 내에 .DEFAULT 특수 내장 타겟을 설정하고 타겟으로
빌드 실패 시 수행할 명령을 등록하면 make가 타겟을 빌드할 룰을 기술 파일 또는 확
장자 규칙에서 찾지 못했을 때 .DEFAULT 타겟에 등록한 명령을 수행한다.
.DEFAULT :
@echo ’’. DEFAULT target test! ’’
hello :
@echo "Hello, world!

關 [screen 4: bash] root@os：/temp/book/make
（ 흐

[root
os make JU make iwtarget
.DEFAULT target test?
[root@os make]tt |

[그림 11-43] .DEFAULT 타겟을 정의한 경우

지금까지 make에 대한 거의 대부분을 설명했다. 내용이 많아서 그렇지 그렇게 어려운
부분은 없었을 거라고 생각한다.

make 최종 정리
마지막으로 지금까지의 내용을 총정리한다는 의미에서 필자가 자주 사용하는 make
파일 구조를 알려주고자 한다. 먼저 디렉토리 구조는 다음과 같다.

才 root@server：,work/book/utils_new/make3
[root@seruer make3]tt tree
-- Config.ink
-- Makefile
-- Rules.mk
-- calendar
|-- Makefile
'-- calendar .c
-- include
'-- diary.h
-- main
|-- Makefile
'main.c
-- memo
|-- Makefile
'-- nemo.c

耳 directories, 10 files
[root@seruer makes]t |

[그림 11-44] build tree 구조

11 장 _ make 585

===== PAGE 587 =====
그리고 각각의 파일들은 다음과 같다.
〔예제 11-23]

최상위 Makefile

.EXPORT_ALL_VARIABLES:
TARGET
TOPDIR
SUBDIRS '

:= diary
:= $(shell /bin/pwd)
:= main memo calendar

###################################
include $ (TOPDIR) /Config.mk
all : compile $(OBJS)
$ (CC) $ (OBJS) $ (addsuffix /built-in.o, $ (SUBDIRS)) -o $ (TARGET)
include $(TOPDIR)/Rules.mk

최상위 Makefile에서는 타겟과 서브디렉토리를 정의한다.
〔예제 11-24)

최상위 Config.mk 파일

CC
LD
INCLUDES
DEFINES
CFLAGS

:= gcc
:= Id
:= -I. -1$(TOPDIR)/include
：= -DDEBUG
：= -02
-W -Wall $(INCLUDES) $(DEFINES)

######################################
.SUFFIXES : .o .c .S
% . o: % . c
$(CC) $(CFLAGS) -c $< -o $@
% . o: % . S
$(CC) $(CFLAGS) -c $< -o $@
######################################

Config.mk 파일에는 각종 매크로를 선언한다.

586

5부—프로젝트빌드

===== PAGE 588 =====
〔예제 11-25〕 최상위 Rules.mk 파일

compile:
@for dir in $(SUBDIRS); do \
make -C $$dir || exit $?; \
done
clean:
@for dir in $(SUBDIRS); do \
make -C $$dir clean; \
done
rm -rf *.o *.i *.s $(TARGET)

모든 Makefile에서 공통으로 사용할 룰은 Rules.mk 파일에 정의한다.
〔예제 11-26]

각 서브디렉토리(main, memo, calendar)의 Makefile

ifndef TOPDIR
TOPDIR :=
endif
include $ (TOPDIR) /Config.mk
TARGET
SUBDIRS

:= built-in.o
:=

OBJS
OBJS

:= $ (patsubst
+= $(patsubst

%.S,

응.o,

응.c,

%.o,

$(wildcard *.S))
$(wildcard *.c))

all : compile $(OBJS)
$(LD) -r $ (addsuffix /$ (TARGET) z $ (SUBDIRS)) $ (OBJS) -o $ (TARGET)
include $(TOPDIR)/Rules.mk

각각의 서브디렉토리에서는 위와 같은 Makefile을 공통으로 사용한다.
이상과 같다. 이해를 쉽게 하기 위해 많은 부분을 축약했는데, 들어갈 내용은 다 들어갔
다고 본다. 위 build 구조는 상당히 쉽고 편하게 작성된 build 구조다. 새로운 서브디렉
토리를 추가하려면 기존의 서브디렉토리에서 Makefile을 복사한 후 SUBDIRS 매크로
에 등록만 해 주면 된다. 그러면 해당 디렉토리에 있는 *.S, *.c 파일을 찾아 자동으로 컴
파일한다. 위 구조에서 make 명령을 내리면 다음과 같이 컴파일한다.

11장_ make 587

===== PAGE 589 =====
命 mot@server：/work/book/utils_new/make3 ZZZ쫴■■■■BR
[root@server makes]#[make|
make[1]: Entering directory '/work/book/utils_new/make3/main'
gcc -02 -W -Wall -I. -I/work/book/utils_new/make3/include -DDEBUG
c main.c -o main.0
Id -r main.o -o built-in.0
make[1]: Leaving directory '/work/book/utils_new/nake3/nain'
make[1]: Entering directory '/work/book/utils_new/make3/nemo*
gcc -02 -W -Wall -I. -I/work/book/utils_new/make3/include -DDEBUG
c memo.c -0 memo.o
Id -r memo.o -o built-in.0
make[1] : Leaving directory '/work/book/utils_new/nake3/meno'
make[1]: Entering directory '/work/bool</utils_new/nake3/calendar ’
gcc -02 -W -Wall -I. -1 /v;ork/book/utils_new/make3/include -DDEBUG
c calendar.c -0 calendar.0
Id —r calendar.0 -0 built-in .0
nake[1]: Leaving directory '/work/book/utils_new/make3/calendar'
gcc main/built—in.o nemo/built-in.0 calendar/built—in.0 -o diary
[rootBseruer make3]tt
[root@seruer make3]tt Is diary
diarpl
[root

（흐seruer make3]tt |

니
[그림 11-45] make 명령 결과

지금까지 배운 내용을 토대로 본 기술 파일을 해석해 보면 그리 어렵지 않게 해석할 수
있을 것이다. 그리고 본 기술 파일은 독자가 이해하기 쉽게 필자가 사용하는 기술 파
일에서 많은 부분을 축약한 파일이다. 본 기술 파일을 토대로 독자의 상황에 맞게 기술
파일을 추가 변경한다면 독자에게 많은 도움이 될 것이라고 필자는 생각한다.
이상 make 과정이 완전히 끝났다. make를 끝내면서 필자가 하고 싶은 말은 유닉스 계
열에서 무언가를 이루고 싶은 사람이 있다면 make는 반드시 확실하게 익혀두라고 말
하고 싶다. make는 유닉스 시스템에서 필수 중의 필수인 유틸리티다.

588

5부_ 프로젝트빌드

===== PAGE 590 =====
12
autoconf

01 autoconf 란무엇인가
02 따라 해보기
03 autoconf의 구조와 원리
04 configure.ac 파일 작성 규칙
05 사용 가능한 매크로
06 함수 체크 매크로
07 세밀한 제어를 위한 configure.ac 작성
08 설정 헤더를 사용해 소스 파일에 설정 적용

===== PAGE 591 =====
I■•으+'s S-fr느dy
앞서 makef- 배우면서 어떻게 하면 쉽게 컴파일할 수 있는지 알아보았다. make 를 사
용하면 프로젝트 파일들을 쉽게 컴파일할 수 있고, 또한 프로젝트 파일들을 구조적으로
나누어 관리할 수 있다. 그렇지만 프로젝트 빌드에 있어 make 만으로는 해결하기 힘든
문제가 하나 남아있다. 그것은 바로 동일한 프로젝트 파일들로 서로 다른 플랫폼과 서
로 다른 머신에서도 별다른 변경 없이 컴파일할 수 있는 이식성이다. 여러 가지 플랫폼
을 지원하려면 개발자는 그런 이식성을 제공해야 한다.

===== PAGE 592 =====
개발한 컴퓨터 환경과 컴파일할 컴퓨터의 환경이 항상 같다면 이식성 문제로 고민할
필요는 없다. 개발 시 사용한 설정 그대로 컴파일하면 되기 때문이다. 그러나 일반적으
로 개발한 환경과 컴파일하는 환경은 서로 같지 않다. 사용자들은 어떤 환경에서든지
소스 프로그램을 컴파일해 사용하고 싶어 한다.
어떤 유닉스에서 혹은 어떤 리눅스에서, 때론 말도 되지 않는 직접 만든 유닉스 계열 운
영체제 환경에서도 마찬가지다. 하지만 필자가 이 글을 쓰면서 사용한 페도라 리눅스 9
환경에서 개발한 소스 프로그램은 선 솔라리스에서 컴파일되지 않을 수 있다. 그리고
같은 리눅스일지라도 데비안 배포판이나 젠투 배포판에서 컴파일되지 않을 수 있고, 같
은 레드햇 계열일지라도 버전이 다른 페도라 리눅스 10 버전에서는 컴파일되지 않을
수 있다.
컴파일이 되고 안 되고를 결정하는 요소는 무수히 많다. 컴파일러의 종류, 헤더 파일의
유무, 헤더 파일 위치, 라이브러리의 유무, 라이브러리 위치, 컴파일 시 사용하는 유틸
리티의 유무 등이 있다. 그리고 컴파일이 되더라도 내부에서 사용한 데이터 타입이 달
라 정상적으로 동작하지 않을 수 있다. 컴파일러나 헤더 파일, 라이브러리가 없는 등의
극단적인 경우라면 컴파일되지 않는 것이 어쩌면 당연하다（컴파일러를 만들어 컴파일
할 수 있는 것도 아니니깐）.
그렇지만 컴파일러의 종류가 다르다든지（예를 들면 gcc나 cc 또는 bcc） , 헤더 파일, 라
이브러리 파일의 위치가 다른 경우와 같이 조금만 설정을 변경하면 컴파일 가능한 경
우가 많이 있게 마련이다. 또한 컴파일은 되지만 데이터 타입이 틀려 정상 작동하지 않
는 경우에도 제대로 동작하게 할 수 있다. 미리 소스 코드에서 다른 데이터 타입에 대
한 처리를 해놓았다면 컴파일 당시에 데이터 타입을 체크해 전처리 과정을 통해 제대
로 동작하는 코드로 컴파일하는 것이 가능하기 때문이다. 이런 요소들은 대개 컴파일
타임에 결정되는 요소들이다. 아무리 개발자가 이식성 높은 코드를 작성했더라도 컴파
일 타임에 이런 요소를 적용시키지 않으면 컴파일이 되지 않거나 되더라도 정상 작동
하지 않을 수 있다. 그렇다고 개발자가 일일이 찾아다니면서 각 시스템에 맞게 적용시
키기는 어려운 노릇이지 않은가?
이때 사용할 수 있는 것이 바로 autotools 다. autotools 를 사용하면 컴파일 타임에 발
생할 수 있는 이런 예외적인 사항을 체크해 융통성 있게 빌드할 수 있다. autotools는
크게 autoconf와 automake로 구성 되는데, 먼저 autoconf를 알아보자.

12장_ autoconf 591

===== PAGE 593 =====
01 【autoconf란 무엇인가
autoconf 는 무엇일까? 간단하게 말해 autoconf 는 configure 셸 스크립트를 생성하는
유틸리티다. 한 번이라도 유닉스, 리눅스 시스템에서 소스 프로그램으로 프로그램을 설
치해 본 독자라면 다음과 같은 순서로 설치한다는 것을 알고 있을 것이다.
. /configure
make
make install

아주 친숙한 명령들이지 않은가? configure 명령은 셸 스크립트로 작성됐다. 그래서
정말 특이한 셸만을 사용하는 독특한 유닉스 시스템이 아닌 이상은 어떤 유닉스 시스
템에서든 동작할 수 있다.

configure 스크립트가 하는 일은 시스템 컴파일 환경을 체크하고 체크한 결과에 따라
make 기술 파일 (Makefile) 을 동적으로 생성하는 일이다. configure 스크립트가 체크
하는 항목에는 현재 시스템에서 어떤 컴파일러를 사용하는지, 그리고 특정 라이브러리
가 있는지 없는지, 특정 헤더 파일이 있는지, 특정 데이터 타입의 크기는 얼마인지 등
컴파일 과정 전반에 필요한 정보들이다.
이 렇게 수집된 정보를 바탕으로 configure 스크립트는 시스템 상황에 맞는 Makefile을
최종적으로 생성한다. 예를 들면 현재 시스템의 컴파일러가 cc 라면 configure/} 만든

Makefile의 CC 매크로는 으로 정의되고, gcc라면 gcc로 정의된다. 컴파일러뿐만 아니
라 다른 유틸리티 역시 마찬가지이고, 함수나 데이터 타입의 사용 유무에 따라 define
옵션이 적절히 설정된다. 마지막으로 make 명령을 내리면 make 는 현재 시스템에 맞
게 정의된 빌드 방법으로 빌드한다.

autoconf 로 configure 스크립트를 생성하는 일은 매우 쉬운 일이다. 단지 configure,
ac 파일에 만들어질 configure 스크립트가 어떤 정보를 수집해야 되는지 알려주기만
하면 된다.
알려주는 방법은 미리 정의되어 있는 autoconf 매크로를 configure.ac 파일에 적절
하게 적으면 된다. 가령 시스템에 있는 C 컴파일러를 체크하려면 C 컴파일러를 찾는

AC_PROG_CC 매크로를 적고, C 전처리기를 체크하려면 C 전처리기를 찾는 매크로인
AC_PROG_CPP 매크로를 적는다.

592

5부_ 프로젝트 빌드

===== PAGE 594 =====
2L따라해보기
그럼 일단 감을 잡기 위해 한번 간단하게 a니toconf로 configure 스크립트를 생성해 보자.
〔예제 12-1〕 like.c 소스 파일

#include <stdio.h>
int main()
{
printf("I like you.\n");
return 0;
}

위와 같이 아주 간단한 like.c 소스 파일을 작성하고 다음과 같은 configure.ac 파일을
작성한다. 이전에도 말했듯이 configure.ac 파일은 어떤 검사를 수행하는 configure
스크립트를 생성하라고 autoconf에 알려주는 파일이다.
〔예제 12-2)

configure.ac 파일

dnl 시작 매크로
AC_INIT(like, 0.0.1, woos@mymail.com)
dnl 체크할 프로그램
AC_PROG_CC
AC_PROG_CPP

# C 컴파일러를 결정
# c전처리기를결정

dnl 체크할 라이브러리
AC_CHECK_LIB ( [c] , [memcpy])
AC^CHECK^LIB ( [m] , [sin] )

# libc를 체크
# libm을 체크

dnl 체크할 헤더 파일
# 괄호에 있는 헤더 파일들을 체크
AC_CHECK_HEADERS([fcntl.h stdlib.h string.h sys/ioctl.h termios.
h unistd.h])
AC_HEADER_DIRENT
# dirent.h 체크
dnl 체크할 데이터 타입 및 구조체
AC_TYPE_SIZE_T
AC2STRUCT_TM

# size_t 타입 체크
# struct tm을 체크

dnl 체크할 라이브러리 함수
AC_CHECK_FUNCS ([strchr strdup strstr] ) # 괄호 안의 함수들을 체크
AC^FUNcJiALLOC
# malloc 함수 체크
dnl 최종적으로 생성할 파일명
AC_CONFIG_FILES ( [Makefile] )
AC"OUTPUT

# 최종적으로 Makefile 생성

12 장 _ autoconf 593

===== PAGE 595 =====
［예제 12-2］ 의 내용 중에 dnl로 시작된 것은 모두 주석을 의미한다. 그래서 굳이 dnl로
시작되는 것들을 적을 필요는 없다. # 역시 주석을 의미하고 dnl과 #이 다른 점은, dnl
은 m4 내부에서 사용되는 주석 함수이므로 autoconf 명령으로 생성될 configure 스
크 립 트 내에 포함되지 않지만 주석 처리한 것은 configure 스크립트 내에 포함
된다는 점이다.

configure.ac 에 사용된 각각의 행은 모두 autoconf 에서 미리 정의되어 있는 autoconf
매크로들이다. 이후 이런 autoconf 매크로는 a니toconf 명령에 의해 각 기능을 수행하
는 셸 스크립트로 확장되어 configure 스크립트의 내용이 된다.
하위 버전 autoconf 에서는 파일명 config 니 re.ac 대신 config 니 re.in 을 사용한다.

autoconf -V 명령으로 확인한 autoconf 버전이 2.57 이하라면 config 니 re.ac 파일을
configurejn으로 변경하기 바란다. 그리고 변경해야 될 것이 몇 가지 더 있는데, 다음
과 같이 각 매크로를 변경하기 바란다.
AC_INIT (like, 0.0.1, woos@mymail. com)
AC_FUNC_MALLOC
AC_CONFIG_FILES ( [Makefile] )
AC_OUTPUT

=>

AC_INIT(like.c)

=>
=>

제차
제거

=>

AC_OUTPUT (Makefile)

autoconf는 버전 특성을 많이 타는 유틸리티다. 상위 호환은 그런대로 되지만 하위 호
환이 잘 되지 않는 편이다. 앞으로 autoconf 는 페도라 9 에 기본적으로 설치되어 있는

autoconf 버 전으로 설명하겠다.
물론 하위 버전 autoconf를 위해 버전에 따라 다르게 적용해야 될 부분을 설명하겠지
만 원활한 실습을 위해 가능하면 환경을 페도라 9 이상 버전으로 바꿀 것을 권장한다.
위와 같이 configure.ac 파일을 작성했으면 이제 Makefile.in 파일을 작성할 차례다.

Makefile.in 파일은 configure 스크립트가 시스템 정보를 수집하고 Makefile을 생성할
때 구조를 잡아주는 탬플릿 파일이다.

Makefile .in 파일의 기본적인 내용은 Makefile 과 거의 유사하지만 configure 스크립트
가 수집한 정보로 변경될 부분이 있는 것이 특징이다.
〔예제 12-3〕 Makefile.in 파일의 내용

CC
CPP
CFLAGS
DEFS

594

&부— 프로젝트 빌드

= @cc@
= @CPP@
= @CFLAGS@
= @DEFS@

===== PAGE 596 =====
LIBS

= @LIBS@

all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS) $(LIBS) -o $@ $?
clean :
-rm -rf like

Makefile.in 파일 내에서 @ 기호로 둘러싸인 @CC@와 같은 것들이 configure 스크
립트에 의해 수집된 시스템 정보로 치환될 부분이다. 나중에 @CC@는 현재 시스템에
있는 C 컴파일러로 치환되고, @CPP@는 현재 시스템에 있는 C 전처리기로 치환되어

Makefileo] 생성된다. 이렇게 @로 둘러싸인 것들을 autoconf 변수라 부르고, 다른 말
로 설정 매개변수라 부르기도 한다.

autoconf 변수는 그냥 아무렇게나 적는 것이 아니라 configure.ac 파일을 작성할 때
추가한 매크로 각각에 자신이 사용하는 변수가 미리 정의되어 있다. 예를 들면 CC 변
수는 AC_PROG_CC 매크로에서 정의된 변수고, CPP 변수는 AC_PROG_CPP 매크로에
정의된 변수다. 좀 더 자세한 설명은 좀 있다 하기로 하고 일단 이렇게 작성했으면 현
재 디렉토리에는 like.c, configure.ac, Makefile .in 이렇게 세 개의 파일이 있을 것이다.
그렇다면 autoconf 명령을 내려 configure 셸 스크립트를 생성한다.
autoconf
于 root@server：/work/book/utils_new/autoconf
[root@seruer
Makefile.in
[rootQseruer
[rootSseruer
[root@seruer
[r*oot@seruer
Makefile.in

autoconf]tt Is
configure.ac like.c
autoconf

autoconf]tt| autoconF j
autoconf]tt
autoconf]!* Is
|confi5ure|
IUtonite.cache configure.ac
[rootSseruer autoconF]tt |

like.c

[그림 12네 autoconf 명령으로 configure 셸 스크립트 생성

아무 메시지 없이 autoconf 명령이 수행되면 정상적으로 수행된 것이다. 오류 메시지가
출력된다면 configure.ac 파일이 잘못 작성된 경우이므로 철자를 한번 확인하기 바란다.
생성된 configure 스크립트는 약 4000행 가까운 셸 스크립트 파일이다. 몇 줄 되지 않
은 매크로를 4000행 가까이 늘린 것은 autoconf에서 사용하는 m4 매크로 처리기다.

12장_ autoconf 595

===== PAGE 597 =====
다음과 같이 ./configure 명령을 내리면 configure 셸 스크립트가 수행되면서

configure.ac 파일에서 체크 항목으로 지정한 것들이 체크되는 것을 확인할 수 있다.
gP root@server：/work/book/utils_new/autoconf
[root(흐seruer autoconf]tt ./configure
checking
For gcc_____ gee
checking
For C compiler default output file name —
whether the C compiler works______________yes
checking
whether we are cross compiling— no
checking
checking
for suffix oF executables______________
checking
for suFfix oF object Files_______________ o
checking
whether we are using the GNU C compiler... yes
whether gcc accepts -g— yes
checking
checking
For gcc option to accept ANSI C________________ none needeq
[checking how to run the' C preprocessor— gcd~~
E
checking for memcpy in -1c— yes
checking for sin in -Im______________ yes
egrep_____grep -E
for
checking
ANSI C header files... yes
for
checking
sys/types.h— yes
for
checking
For sys/stat.h________ yes
checking
stdlib.h_______ yes
for
checking
For string.h— yes
checking
memory.h— yes
for
checking
For strings.h— yes
checking
For inttypes.h_______ yes
checking
For stdint.h— yes
checking

三

[그림 12—2] ./configure 명령 수행

configure 스크립트는 수행이 끝날 때쯤에 수집된 시스템 정보를 바탕으로 config,
status 셸 스크립트를 생성하고 수행한다.
config.status 스크립트는 Makefile.in 파일을 입력으로 Makefile .in 파일 내에 사용된
©로 시작하는 autoconf 변수들을 수집 한 정보로 치환해 Makefile을 생성 한다.
생성된 Makefile을 열면 각각의 autoconf 변수들이 수집한 시스템 정보로 치환되어 있
는 것을 확인할 수 있다.
艾 root@server：/work/book/utils new/autoconf
CC
= gcc
CPP
= gcc -E
CFLAGS
|= _g -02
,, -DPACKAGE_TARNfi
“like
DEFS
= —DPACKAGE_NAME=
,,
(AGE_UERSI0N-V'8.0.1^" -DPACKAGE_S?RING=
ME=
"like
DPAC
)PACicAGE_BUGREP0RT=V'woos@mynail7conV "like'
e.0.1
JE_LIBM=1 -DSTDC_HEADERS=1 -DHAUE_SVS_TY
DHfiUE LIBC=1 DHfi
PES H=1 -DHAUE_SVE_STfiT_H=1 -DHAUE_STDLIB_H=1 -DHAUE_STRI
NG_H=1
-DHfiUE_MEM
-DHfiUE_STRINGS_H=1
-DHAUE_INTTVP
NI
=1 -DHAUE2UNISTD_H=I
AUE_PCNTL_H
ES
=1 -DHAUE
STD
=i AUE_STDEIB_
I=I -DHAUE_STRTNG_H=I—-DHAUE_SVSZIOCTCH
-DHAUE_UNISTD_H=1
-DHAUE_DIREHT_H=1
=1
-DHAUE_TERMIOS H=1
DHAUE_STRDUP=1 DHAUE STRSTR=1 -DHftUE S
-DHAUE_STRCHR=1
1fiLL0C=1
TDLIB H=1 -DHAUE
= -In -lc
LIBS

느

느

느 一
、 느" 一

허
애

드 【 대

으

느

-애

lall : like
like : like.c
lakefile [ + ]

[그림 12-3] config.status 스크립트에 의해 치환된 Makefile

596

5부_ 프로젝트빌드

===== PAGE 598 =====
이제 make 명령을 내리면 make는 현재 시스템에 맞게 작성된 Makefile로 like.c 소스
파일을 컴파일한다.

[root@seruer autoconF]tt make
,,
gcc -g -02 —DPfiCKfiGE_NAME=
"like
DPACKAGE_TARNftME=
"li
keV —DPACKAGE_UERSI5N=
8.0.1
-DPACKAGE_STRING=V'ii|<e^H
0.0.1^" -DPACKAGE_BUGREP0RT=V'Woos@mynail7comV -DHAUE_LH
IBC=1 -DHAUE_LIBMM -DSTDC_HEADERS=1 DHAUE_SVS_TVPES_H=lH
fiUE_SVS_&TfiT_H=1
fiuE_STDLIB_H=1 DHAUE_STRING_H=1 ■.
-DHAUE_MEM0RV_H=1 -DHfiUE_STElNGS_H=1 -DHAUE_liiTTVPEsZH
-DHAUE_STDINT_H=1 -DHAUE2UNISTD_H=1 -DHfiUE_FCNTL_H=1--DHAB
UE_STD
IB_H=1 -DHAUE_STRTNG_H=1--DHfiUE_Sys2lOCTLZH=1
A
UE_TERMI0S_H=1 -DHAUE_UNISTD_H=1 -DHfiUE_DIRENT_H=1 -DHAUEH
_STRCHR=I
AUE_STRDUP=I -DHAUE_STRSTR=I
HAUE_STDLIB_H^
=1 -DHAUE_MALL0C=1 -Im -lc -o like like.c
[root@seruer
autoconF]tt
[rootSseruer
autoconF]tt ./like
I like you.
[rooteserver
autoconf]tt
|[root@server
autoconf]tt |

느 느 一
느'' 으"

애

으 너

애

너■
-애 昌

『

-애

니）

［그림 12-4］ make 명령 수행

그러면 지금까지의 과정이 어떻게 해서 일어났는지 알아보자.

KI autoconf의 구조와 원리

[그림 12-5] autoconf의 구조

［그림 12-5］ 는 a니toconf의 구조를 잘 보여준다. autoconf를 사용하려면 먼저

configure.ac 파일을 작성해야 한다. configure.ac 파일은 직접 작성해도 되고
autoscan의 도움을 받아도 된다.

12장_ autoconf

597

===== PAGE 599 =====
autoscan 명령은 현재 디렉토리를 기준으로 소스 파일과 Makefile .in, Makefile.am 파
일의 내용을 기초해 configure.scan 파일을 생성한다. 소스 파일 내 사용된 함수 및 구
조체 종류, include된 헤더 파일 종류, 사용된 라이브러리 종류, Makefile에서 사용하는
빌드 유틸리티의 종류 등이 configure.scan 파일을 생성하는 기초 자료다.

configure.scan 파일은

파일명만

config니re.ac로

변경하면

바로

사용

가능한

configure.ac 파일이 될 수 있다.
autoscan 명령으로 만든 configure.ac 파일은 원하는 체크 항목이 과할 수도 있고 부
족할 수도 있다. 그래서 주로 autoscan 명령을 통해 생성된 config니re.scan 파일을 바
탕으로 수정해 configure.ac 파일을 만드는 편이다.
autoscan

autoscan 명령은 위와 같이 아무런 인자 없이 입력한다. autoscan 명령을 내리면 현재
디렉토리에 configure.scan 파일이 생성된다.

configure.ac 파일은 autoconf 매크로로 구성되어 있는데, autoconf 매크로는 m4 매
크로 처리기 형식의 매크로다. m4는 Retinal 포트란에서 사용하는 전처리기다. C에서

cppO 또는 ccl -E가 전처리기로 사용되듯이 Retinal 포트란에서는 m4가 전처리기로
사용된다. m4가 cppO처럼 전처리기라고 해서 cppO와 같이 단순 치환하는 간단한 매
크로 처리기는 아니다.

m4는 내장 함수를 가지고 있어 cppO로는 도저히 상상도 할 수 없는 일들을 처리할 수
있다. 예를 들면 문자열 처리와 관련한 여러 가지 작업을 수행할 수 있고, 산술 연산뿐
만 아니라 유닉스 명령도 사용할 수 있다. 물론 m4는 근본적으로 매크로 처리기이므로
매크로를 선언된 문자열로 치환하는 것이 m4의 기본 임무다.

autoconf는 m4의 이런 기능을 이용해 configure.ac 파일에 사용된 autoconf 매크로
들을 각각의 기능을 수행하는 셸 스크립트로 확장한다. 예를 들면 이전에 사용한 AC_

CHECK_LIB([c], [main]) 매크로는 libc를 체크하는 [예제 12-4]와 같은 셸 스크립트
로 확장되어 configure 스크립트에 추가된다.
〔예제 12-4)

libc를 제크하는 셸 스크립트

...상략
ac_cv_lib_c_main=no
fi

598

5부—프로젝트빌드

i
：
；

===== PAGE 600 =====
rm -f conftest.$ac_objext conftest$ac_exeext conftest.$ac_ext
LIBS=$ac_check_lib_save_LIBS
fi
echo "$as_me:$LINENO: result: $ac_cv_lib_c_main" >&5
echo "${ECHO_T}$ac_cv_lib_c_main" >&6
if test $ac_cv_lib_c_main = yes; then
cat »confdefs.h «_ACEOF
#define HAVE_LIBC 1
_ACEOF
LIBS="-lc $LIBS"
fi

configure.ac 파일에 정의한 모든 매크로는 이와 같은 각각의 셸 스크립트로 m4에 의
해 확장된다. 그래서 생성된 configure 스크립트를 수행시키면 configure.ac 파일에서
정의한 체크 항목을 각각 체크할 수 있는 것이다.

configure.ac 파일에 사용할 수 있는 매크로는 이미 정의되어 있는 a니toconf 매크로라
고 했으니 어디엔가 정의되어 있어야 할 것이다. autoconf 매크로는 모두 /usr/share/

autoconf 디렉토리에 정의되어 있다.
grep 명령으로 configure.ac 파일에서 사용된 AC_PROG_CC 매크로를 /usr/share/
autoconf 디렉토리에서 확인하면 ./autoconf/c.m4 파일에 정의되어 있는 것을 알 수
있을 것이다.

autoconf 명령으로 생성된 configure 스크립트를 수행하면 각각의 항목을 체크하고
수집된 정보를 바탕으로 config.status 셸 스크립트를 생성한다.

config.status 스크립트는 파일명.in 파일의 내용을 치환해 파일명 파일을 생성하는
스크립트다. 예를 들면 Makefile .in 파일이 있으면 Make file.in 파일 내부에 사용된

autoconf 변수를 수집한 시스템 정보로 바꾸고 Makefile을 만든다. config.h.in 파일이
있으면 내부에서 사용된 C define을 수집한 시스템 정보를 적용해 config.h 파일로 변
경하는 것이 config.status 스크립트의 임무다.

config.stat니s 스크립트에서 생성할 파일을 지정하는 매크로는 AC_CONFIG_FILES 매
크로다. AC_CONFIG_FILES 매크로에 인자로 사용된 파일들은 config.status 스크립트
가 수행될 때 인자로 사용된 파일명.in 파일을 찾아 내부의 a니toconf 변수에 수집된 시
스템 정보를 적용해 “.in”을 제거하고 파일명으로 만든다.

12장_ autoconf 599

===== PAGE 601 =====
지금은 AC_CONFIG_FILES([Makefile])만 지정했기 때문에 Makefile만을 생성했지만
나중에 다른 파일도 생성한다는 것을 확인할 수 있을 것이다.

config.status 스크립트가 *.in 파일에서 치환하는 내용은 @변수명®으로 되어 있
는 부분인데, 이전에 말했듯이 이런 변수명은 configure.ac 파일을 작성할 때 사용한

autoconf 매크로에서 이미 정해져 있다.
config.status 스크립트나 config.log 파일을 열면 [그림 12-6]에서 네모로 체크한 부
분을 확인할 수 있는데, 이것은 바로치환될 변수들의 리스트와 그에 해당하는 시스템
정보다.

[그림 12-6] config.status 스크립트에 들어 있는 변수와 수집된 시스템 정보

위 변수 중 해당하는 파일이나 유틸리티를 찾지 못한 변수가 있으면 그 변수의 값은 null
문자로 설정된다. 그래서 나중에 해당 변수가 치환될 때도 nuU 문자(‘’)로 치환된다.

configure 스크립트 수행이 끝나면 config.status 스크립트 외에 configjog 파일도 생
성되어 있다.

config.log 파일은 configure 스크립트가 수행되면서 수집한 시스템 정보 리스트가 들
어 있기 때문에 Makefile .in 파일을 작성하는 데 있어 configure 스크립트가 수집하는
정보와 변수명을 모른다면 configjog 파일에서 확인할 수 있다. 또한 config.log 파일
은 configure 스크립트 오류 발생 시 오류에 대한 정보도 들어있기 때문에 configure
스크립트 수행 과정에서 문제가 발생했다면 제일 먼저 확인해야 되는 파일이기도 하다.

Makefile.in 파일은 직접 작성해도 되고 좀 더 이식성 있는 Makefilejn 파일을 생성하
기 위해서는 automake 명령으로 자동 생성해도 된다. automake를 사용해 Makefile,

in 파일을 생성하는 방법은 automake를 설명할 때 따로 설명한다.

600

5부_ 프로젝트 빌드

===== PAGE 602 =====
04 【configure, ac 파일 작성 규칙
지금까지 배운 내용으로 볼 때 autoconf는 원리가 매우 단순함을 깨달았을 것이다. 원
리가 단순한 만큼 사용법 또한 매우 단순하다.

autoconf 를 사용하려면 configure.ac 파일에 자신이 체크하고 싶은 항목의 매크로를
찾아서 주르륵 적거나 그것도 귀찮으면 autoscan 명령으로 자동 생성한다. 그리고 해
당 매크로가 어떤 변수를 넘겨주는지 확인하고 Makefile.in 파일을 작성할 때 해당 변
수를 알맞게 사용하면 된다.

configure.ac 파일을 작성하는 데 특별히 대단한 규칙이 있는 것은 아니지만 반드시
알고 있어야 낭패를 당하지 않는 규칙들이 있다. 지금부터는 그런 규칙을 설명한다.
먼저 configure.ac 파일의 기본적인 형태는 다음과 같다.
AC_INIT(FULL-PACKAGE-NAME, VERSION, BUG-REPORT-ADDRESS, TARNAME)
# programs 결정에 관한 매크로
# librarie에 관한 체크 매크로
# header file에 관한 체크 매크로
# typedef z structure, 컴파일러 특성에 관한 체크 매크로
# library function들에 관한 체크 매크로
AC_CONFIG_FILES ( [file...] ) # configure 를 수행한 후 생성될 파일을 지정
AC^OUTPUT-

ACJNIT 매크로는 반드시 시작 부분에 있어야 한다. ACJNIT 매크로에는 네 개의 인
자가 들어가는데, 이 중 세 번째 인자와 네 번째 인자는 생략할 수 있다.
인자가 있는 autoconf 매크로들은 매크로명과 괄호(‘(’) 사이를 반드시 공백 없이 붙여
야 한다(예: AC_INIT(like, 0.0.1,...)). 그렇지 않으면 오류가 발생할 것이다.

ACJNIT 매크로의 첫 번째 인자에는 패키지명을 적고, 두 번째 인자에는 버전을 적는
다. 그리고 세 번째 인자에는 버그를 보고할 메일 주소를 적고, 네 번째 인자에는 tar 파
일명을 적는다. 모든 인자를 다 적은 AC_INIT 매크로의 예는 다음과 같다.
AC_INIT(like,

0.0.1,

woos@mymai丄.com,

like.tar.gz)

12장_ autoconf

601

===== PAGE 603 =====
하위 버전의 autoconf 에서는 AC_INIT 매크로에 인자가 단 하나만 들어가는데, 다음
예와 같이 configure 스크립트와 같은 디렉토리에 있는 소스 파일명을 아무거나 하나
적으면 된다.
AC_INIT(like.c)

configure 스크립트와 같은 디렉토리에 있는 소스 파일이 없으면 configure 스크립
트가 있는 디렉토리를 기준으로 소스 파일의 상대 경로를 적는다. 이렇게 소스 파일
을 적는 이유는 configure 스크립트가 정확한 위치에 있는지 확인하기 위한 목적이다.

ACJNIT 매크로 다음에 오는 항목들은 각각의 체크 항목과 관련된 매크로다. 일반적으
로 위와 같은 순서를 따르며 반드시 위와 같은 순서를 지킬 필요는 없지만 통일성을 위
해 지키는 것이 좋다.

AC_CONFIG_FILES 매크로는 반드시 있을 필요는 없지만 AC_CONFIG_FILES 매크로
가 없으면 configure 스크립트가 아무짝에 쓸모 없게 될 것이다. AC_CONFIG_FILES
매크로를 사용하지 않고 생성된 configure 스크립트는 시스템 체크만 수행하고 어떤
파일도 생성하지 않기 때문이다.

AC_CONFIG_FILES 매크로에는 출력될 파일들을 적으면 된다. 일반적으로 Makefile이
출력될 파일이기 때문에 AC_CONFIG_FILES([Makefile])라고 사용한다. 그리고 다음
과 같이 여러 개의 파일을 지정할 수도 있다.
AC_CONFIG_FILES ([Makefile conf .h db/Makefile])

위와 같이 사용되었다면 현재 디렉토리에는 Makefilejn, conf.h.in 파일이 있어야 하고

db 디 렉토리 에 는 Makefile .in 파일 이 있어 야 한다. 각각의 파일들은 config.status 스
크립트에 의해 내부에서 사용된 autoconf 변수가 치환되어 .in 확장자가 없는 파일로
생성된다.
인자에서 쓰인 대괄호([])는 m4에서 사용하는 문자열을 의미하고, C 소스에서 쌍 따옴
표(“”)를 문자열에 붙이는 것과 같은 의미다.
하위 버전의 autoconf는 AC_CONFIG_FILES 매크로 대신 AC_OUTPUT 매크로에서
출력 파일을 지정했다. 물론 상위 버전의 autoconf 역시 AC_OUTPUT 매크로에서 출
력 파일로 지정해도 되지만 현재는 AC_CONFIG_FILES 매크로에 출력 파일을 지정하
는 것이 더 일반적이기 때문에 AC_CONFIG_FILES 매크로에 지정하기 바란다.

602 &부_ 프로젝트 빌드

===== PAGE 604 =====
AC_OUTPUT 매크로는 반드시 마지막에 와야 되는 매크로다. AC_OUTPUT 매크로를
넣지 않으면 config.status 스크립트가 생성되지 않는다. 그러면 역시 configure 스크
립트가 아무짝에도 쓸모없게 될 것이다.

AC_CONFIG_FILES 매크로에 출력 파일을 지정하지 않고 AC_OUTPUT 매크로에 출
력 파일을 지정하는 방법은 다음과 같다.
AC_OUTPUT ([Makefile conf .h db/Makefile])

물론 이렇게 AC_OUTPUT 매크로에 출력 파일을 지정했다면 AC_CONFIG_FILES
매크로는 사용하지 말아야 한다. 구 버전 autoconf 와 호환을 위해서라면 이렇게

AC_OUTPUT 매크로에 출력 파일을 지 정하기 바란다.
이상이 configure.ac 파일 작성의 기본적인 규칙이다. autoconf를 사용하는 일은 이런
기본 규칙을 지키면서 자신이 체크하고자 하는 항목의 매크로를 추가하기만 하면 된다.

autoconf에서 사용 가능한 매크로의 종류는 프로그램 체크 매크로, 라이브러리 체크,
헤더 파일 체크, 함수 체크, 파일 체크 매크로 등 그 수가 매우 광범위하다. 이 많은 매
크로를 모두 설명하는 것은 독자들이 지루해 할 것이므로 자주 사용하는 매크로와 사
용법이 독특한 매크로를 위주로 설명한다. 나머지 매크로는 모두 부록에서 설명 했으니
나중에 configure.ac 파일을 직접 작성할 때 참고하기 바란다. 그럼 어떤 매크로가 사
용 가능한지 알아보자.

5 L 사용가능한매크로
I 프로그램 결정 매크로
프로그램 결정 매크로의 특징은 프로그램이 존재하는지 체크하고, 존재한다면 실행 가
능한지 확인한다. 실행까지 가능하다면 해당 변수에 프로그램명을 넣어 Makefile.in 파
일로 넘긴다. 프로그램 결정 매크로와 각 매크로가 넘기는 변수에는 다음과 같은 것들
이 있다.

12장_ autoconf 603

===== PAGE 605 =====
[표 12-1] 프로그램 결정 매=
매크로

넘기는 변수

설명

AC_PROG_CC

CC

C 컴파일러 결정（환경 변수 CC 값이 우선이고, 없으면
gcc, cc순으로 찾음）

AC_PROG_CPP

CPP

C전처리기 결정

AC_PROG_CXX

cxx

C++ 컴파일러 결정

AC_PROG_CXXCPP

CXXCPP

C++전처리기 결정

AC_PROG_F77

F77

포트란 컴파일러 결정

AC_PROG_AWK

AWK

awk 프로그램 결정（ mawk, gawk, nawk, awk순으로 찾음）

AC_PROG_YACC

YACC, BISON

YACO 결정（ bison, byacc, yacc순으로 찾음）

AC_PROGJNSTALL

INSTALL

install 프로그램이나 install 스크립트 결정

AC_PROG丄EX

LEX

lex 결정（ flex, lex순으로 찾음）

AC_PROG_LN_S

LN

link 결정

AC_PROG_MAKE_SET

MAKE

make 결정

AC_PROG_RAN 니 B

RANLIB

ranlib 결정

AC_PROG_EGREP

EGREP

grep 명령의 一E 옵션（ egrep순으로 결정）

AC_PROG_FGREP

FGREP

grep 명령의 一F 옵션（ fgrep순으로 결정）

사용법은 다음과 같다. 소스 프로그램에서 yacc를 사용해 파서를 구현했을 경우 프로
그램 결정 매크로를 사용해 이식성을 높이는 방법은 다음과 같다.
먼저 yacc에 대해 간단하게 설명하면 yacc는 파서를 만들 때 사용하고 *.y 파일을 입력
으로 파서 인 y.tab.c 파일을 생성한다. yacc는 플렛폼에 따라 여 러 종류가 있을 수 있는
데, bison, byacc, yacc가 모두 yacc의 일종이다. 각각은 서로 약간씩은 다르지만 기본
적으로 *.y 파일을 읽어 파서를 생성하는 일은 같다.
이때 어떤 시스템에 yacc로 bison이 있는데, 프로젝트 파일의 Makefile에서 byacc
를 사용해 컴파일하게 되어 있으면 정상적으로 컴파일이 완료되지 못할 것이다. yacc
으로 bison이 있지만 실행 명령이 달라 실행되지 못하는 경우다. 이런 상황이라면

configure.ac 파일과 Makefilejn 파일을 다음과 같이 작성하면 현재 시스템에 bison
이 있던 byacc가 있던 혹은 yacc가 있던지 간에 configure 스크립트가 현재 시스템에
있는 yacc를 찾아 사용 가능하게 한다.

604

5부_ 프로젝트빌드

===== PAGE 606 =====
〔예제 12-5)

configure.ac 파일의 내용

AC_INIT(parser, 0.0.1, woos@mymail.com)
AC_PR0G_CC
AC_PR0G_YACC
AC_CONFIG_FILES ( [Makefile] )
AC_0UTPUT

먼저 configure.ac 파일에서 AC_PROG_YACC 매크로를 사용해 yacc를 결정하는 매
크로를 추가한다. 그리고 Makefile.in 파일을 다음과 같이 작성한다.
〔예제 12-6)

Makefile.in 파일의 내용

CC
CFLAGS
YACC
all :

= @CC@
= @CFLAGS@
= @YACC@ # AC_PROG_YACC 매크로에서 넘겨 주는 변수

parser

parser : parser.y
$(YACC) $A
$ (CC) $ (CFLAGS) -o parser y.tab.c

그러면 config니re 스크립트가 수행하면서 현재 시스템에 있는 yacc을 bison, byacc,

yacc순으로 찾아 결과를 YACC 변수에 넣고 config.status 스크립트를 생성한다.
config.status 스크립트가 수행되면서 Makefile.in 파일에서 사용된 @YACC@ 기호를
찾는 결과 명령으로 치환해 Makefile을 생성한다.
필자의 시스템에서 위 파일들을 작성하고 autoconf 명령으로 configure 스크립트를
생성한 후 수행했을 때 생성되는 Makefile의 내용은 다음과 같다.

[그림 12-7] Makefile 내용

12장_ autoconf

605

===== PAGE 607 =====
［그림 12-’기에서 알 수 있듯이 필자의 시스템에는 yacc로 bison이 있다. 이상이 yacc
를 사용하는 예였고, C 컴파일러를 결정하는 매크로 사용법은 다음과 같다.
〔예제 12-7〕 configure.ac 파일의 내용

AC_INIT(like, 0.0.1, woos@mymail.com)
AC_PR0G_CC
AC_CONFIG_FILES ( [Makefile] )
AC_0UTPUT

configure,ac 파일에 위와 같이 AC_PROG_CC 매크로를 추가한다. 이후 AC_PROG_
CC 매크로는 autoconf 명령에 의해 C 컴파일러를 찾는 셸 스크립트로 확장될 것이다.
〔예제 12-8)

Makefile.in 파일의 내용

CC
CFLAGS
DEFS

= @cc@
= @CFLAGS@
= @DEFS@

all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS) -o $@ $A

［예제 12-8］ 와 같이 작성하고 autoconf 명령으로 configure 스크립트를 생성한다.
생성한 configure 스크립트를 수행하면 다음과 같은 Makfile이 생성된다.

=J므L스J
I스!

므? root@server：/work/book/utils_new/autoconf1

§c—
1 gw |
CFLAGS
= -g -02
= -DPACKAGE NAME=V'likeV -DPACKAGE_TARNA
DEFS
ME=V'likeV' —DPACKAGE_UERSI6N=
0.0.1'
-DPACKAGE_STRING=
V'like^ 0.0.1
-DPfiCKAGE_BUGREPORT=Vwoos@mymailTcoii»V'

乂"

으"

、”

all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS)

「＜ $@ $*

［그림 12—8］ 생성된 Makefile 내용

AC_PROG_CC 매크로는 먼저 시스템 환경 변수에 CC7} 있는지 확인한다. 있으면 환경
변수 (으의 내용을 CC 변수에 넣어 config.status 스크립트를 생성한다.

CC 환경 변수가 없으면 gcc, 유순으로 컴파일러를 찾는다. 필자의 시스템에서는 CC 환

606 5부— 프로젝트 빌드

===== PAGE 608 =====
경 변수가 정의되어 있지 않고 gcc가 있기 때문에 Makefile.in 파일에서 사용된 @CC@
가 gcc로 치환되어 Makefile이 생성된 것을 확인할 수 있다.

@CFLAGS©와 @DEFS@는 AQJNIT 매크로에 정의된 변수다. 이렇게 ACJNIT 매크
로에 정의되어 있어 항상 전달되는 변수를 기본 변수라 하고, ./configure —prefix=/

usr/local----------------------------- configure 스크립트를 수행하면서 옵션을 지정해 내
용을 바꿀 수 있다.
위 기본 변수 중 유심히 보아야 될 것은 바로 DEFS 변수다. DEFS 변수에는 시스템 환
경을 체크하고 체크한 결과를 define 옵션으로 넘겨주는 매크로가 있을 때 define 옵
션이 추가되는 변수다. 이 렇게 DEFS 변수에 추가된 매크로는 위 Makefile처 럼 gcc 컴
파일 옵션으로 사용된다. 그러면 각 파일에 define 설정을 하는 것이 가능하다. 물론 이
렇게 각 소스 파일에 적용되는 define은 전처리 과정에서 각 시스템에 맞는 소스 파일
을 선택할 때 사용한다.

DEFS 변수 외 에 반드시 알아야 할 기본 변수에는 LIBS 변수가 있다. LIBS 변수에는 링
크에 전달할 라이브러리 옵션이 들어 있다. 가령 configure.ac 파일에서 라이브러리 체
크 매크로를 사용했다면 해당되는 라이브러리에 대해 “-1라이브러명” 형식으로 LIBS
변수에 추가된다.
이제 생성된 Makefile로 make 명령을 내리면 다음과 같이 기분 좋게 컴파일되는 것을
확인할 수 있다.
'I [screen 4： bash] root@os：~/os/autoscan/test

FT*

[rooithos test]tt make_________________ __________ __ _________________ _
gcc -g -02 -DPACKAGE_NfiME=tt"li@7, —DPACKAGE_TARNfiME=tf,,likeW" I
PACKAGE_UERSION=tt"0.0.1tf" -DPfiCKfiGE_STRING=tf"liketf 0.0.W" -DPAI
KfiGE_BUGREPORT=tf”woos@mymail.comtf" -o like like.c
[rootQos
|

[그림 12-9] make 명령 수행 화면

이상이 프로그램 결정 매크로의 사용에 관한 설명이다. 나머지 매크로 역시 사용법은
동일하다. configure.ac 파일에 매크로를 추가하고 Makefilejn 파일에서 넘겨주는 변
수를 사용해 작성하면 된다.

C 컴파일러와 관련해 위에서 정의한 매크로 외에 몇 가지 부수적인 매크로가 더 있다.
빅 엔디안 지원 여부, volatile 지원 여부, long double 타입의 지원 여부 등을 체크하
는 매크로가' 더 있다. 필요한 독자는 이 책 뒤에 있는 부록을 참고하기 바란다.

12장_ autoconf 607

===== PAGE 609 =====
그런데 [표 12-1]에 나와 있지 않은 프로그램을 찾고 싶을 때는 어떻게 하면 될까? 가령

cat 명령이 시스템에 있는지를 찾고 싶다면 말이다.
그럴 때는 다음과 같은 매크로를 사용하면 된다.

AC_CHECK_PROG(variable, prog, value-if-found, [vah e-if-not-found], [path], [reject])
』

AC_CHECK_PROG 매크로는 셸의 PATH 환경 변수 디 렉토리들에서 prog 프로그램을 찾
는다. 찾으면 variable 변수에 value-if-found 값을 넣고 못 찾으면 value -if-not-found
값을 넣는다.
대괄호([])가 있는 인자들은 모두 생략 가능함을 의미하고 path 인자가 사용되었다면 path
인자가 지정한 위치에서도 찾는다. 찾았더라도 reject 인자가 지정하는 파일은 제외한다.

AC_CHECK_PROG 매크로를 사용하는 예는 다음과 같다. 먼저 configure.ac 파일에
다음과 같은 라인을 추가한다.
AC_CHECK_PROG([CAT], [cat], [YES], [NO], [$PATH:/root/bin:/root/sbin],
[/usr/bin/cat])

위 매크로의 의미는 cat 프로그램을 PATH 환경 변수가 지정하는 디렉토리와 /root/

bin, /root/sbin 디렉토리에서 찾는다. 찾았으면 CAT 변수에 YES 문자열을 넣고, 못
찾았으면 NO 문자열을 넣는다. 찾았더라도 /usr/bin/cat은 제외한다.
현재 필자의 시스템에는 cat 명령이 /bin/cat으로 존재하기 때문에 CAT 변수에는 YES
문자열이 들어간다.

autoconf 명령으로 configure 스크립트를 새로 생성한 후 수행시키면 config.status
스크립트 내 CAT 변수의 값이 YES로 지정된 것을 확인할 수 있다.
B [screen 1： bash] root@os：/temp/book/autoconf
厂厄
0gg헤示三리히一

（흐,
츠:
수
（ 흐

s,@ftWK
qawk, ;t
s：@CftT@：；ES,
t t|
s,
LIB0BJS@,,;t t
s,@LTLIBOBJS@,,；t t

HisIB

量
BT

[그림 12너0] config.status 스크립트 내용

물론 이렇게 정의된 CAT 변수는 Makefile.in 파일에서 @CAT@과 같이 사용하면 YES
문자열로 치환될 것이다.
앞으로 설명할 모든 매크로의 포루투. 타입에서 대괄호로 묶여 있는 인자는 생략이 가
능하다. 가령 AC_CHECK_PROG (variable, prog, value-if-found, [value-if-not-

found], [path], [reject])에서 variable, prog, value-if-found 인자는 반드시 있어야
608

5부- 프로젝트빌드

===== PAGE 610 =====
하지만 [value-if-not-found], [path], [reject] 인자는 생략해도 무방하다. 그래서 AC_

CHECK_PROG 매크로의 생략 가능한 인자를 생략하고 사용하는 방법은 다음과 같다.
AC_CHECK_PROG([CAT], [cat] , [YES] )

찾아야 하는 프로그램이 많아 AC_CHECK_PROG 매크로를 여러 번 써야 한다면 다음
과 같이 AC_CHECK_PROGS 매크로를 사용할 수 있다.

AC_CHECK_PROGS(variable, progs, [value-if-not-fo nd], [path])
니

AC_CHECK_PROGS 매크로는 공백으로 구분되는 progs 리스트에 있는 프로그램들을 차
례로 찾는다. 찾았으면 variable 변수에 찾은 값을 넣고 리스트의 프로그램을 하나도 못 찾
으면 value-if-not-found 값을 넣는다.
기본적으로 PATH 셸 환경 변수에 등록된 디렉토리에서 찾지만 path가 지정되어 있으면

path 위치도 찾는다.

AC_CHECK_PROG 매크로가 단 하나의 프로그램만을 체크하는 데 비해 AC_CHECK_
PROGS 매크로는 여러 개의 프로그램을 체크할 수 있다. AC_CHECK_PROGS 매크로
를 사용해 여러 개의 프로그램을 체크하는 예는 다음과 같다.
AC_CHECK_PROGS([MYCC], [acc vcc cc gcc])

위 예를 configure.ac 파일에 추가하고 autoconf 명령으로 configure 스크립트를
새로 생성한 후 수행한다. 생성되는 config.status 파일의 내용을 보면 다음과 같이

MYCC 변수가 할당되고 MYCC 변수 값으로 으가 설정되어 있는 것을 확인할 수 있다.
QI [screen 1: bash] root@os:/temp/book/autoconf
^@fuJk@7gawk7it”t
s,@CfiT@,VES,;t t
s,@MVCC@,cc, ；t t|
iJse,,；t t
___________________________________________________ 473,1

前

[그림 12-11] config.status 파일 내용

MYCC 변수에 cc 가 설정되어 있는 이유는 acc 와 vcc 는 현재 시스템에 없고 cc 가 제
일 먼저 찾아지는 프로그램이기 때문이다. gcc 도 있지만 gcc 보다 먼저 찾아진 cc 가

MYCC 변수 값으로 설정된다.
위 예에서는 모든 명령을 찾지 못했을 때 MYCC 변수 값으로 설정되는 value-if-

not-found 인자를 사용하지 않았다. 이렇게 되면 모든 명 령 리스트를 찾지 못했을 때
MYCC 변수 값은 null 문자열로 설정된다.

12장_ autoconf 609

===== PAGE 611 =====
프로그램 체크 매크로에는 조금 특이한 매크로로 AC_CHECK_TOOL 매크로가 있다.

AC_CHECK_TOOL 매크로는 자주 사용되진 않지만 특이성 때문에 살펴보자.
AC_CHECK_TOOL(var/ab/e, prog, [value-if-not-found], [path])
AC_CHECK_PROG
를

붙인

매크로와

유사하지만

prog에

AC_CANONICAL_HOST와

대시(-)

prog를 먼저 찾고 없으면 그냥 prog를 찾는다. AC_CANONICAL_HOST는

configure 스크립트를 수행할 때 ./configure-------------------------------------------------- 같은 형식으
로 지정 가능하다.

위 설명만으로 이해가 되지 않으므로 직접 예를 들면서 설명한다.
AC_CHECK_TOOL([MYCC]f [gcc])

위와 같은 라인을 configure.ac 파일에 추가하고 configure 스크립트를 새로 생성한
후 configure 스크립트를--------------------------------------- 옵션을 주고 수행해 본다.

config.status 파일을 열었을 때 레드햇 리눅스라면 기본적으로 i386-redhat-linuxgcc 명령이 있기 때문에 [그림 12-12]와 같이 MYCC 변수에 i386-redhat-linux-gcc
가 설정되어 있는 것을 확인할 수 있다.
H [screen 1： bash] root@os：/temp/book/autoconf
丁하졔히;흐
흐
s,（ 흐CAT@,VES, ；t t_________
sp5fi7U^,i386-redhat—linux~gcc, ;t t |
s,@ac_ct_MVCC@,,;t t
473,1

[그림 12너2] config.status 파일 내용

이상으로 프로그램 결정 매크로의 설명을 마칠까 한다. 그 외 프로그램 결정에 사용 가
능한 매크로로 AC_CHECK_TOOLS, AC_PATH_PROG, AC_CHECK_PORGS 등 여러
매크로가 있다. 나머지 매크로에 대한 설명을 부록에 넣어 두었으니 configure.ac 파일
을 작성할 때 참고하기 바란다.

| 라이브러리 체크 매크로
라이브러리 체크 매크로는 자주 사용되는 매크로로, 특정 라이브러리를 링크해 사용 가
능한지를 체크한다. 또한 특정 라이브러리와 링크해 특정 함수를 사용 가능한지도 체크
한다.

610

5부_ 프로젝트빌드

===== PAGE 612 =====
AC_C H ECK_LIB(//'brazy, function, [action-if-found], [action-if-not-found], [other-libraries])
인자인 라이브러리(library)와 링크해 주어진 함수(function)가 사용 가능한지 테스트한다.
사용 가능하다면 action-if-found에 지정된 셸 스크립트 또는 autoconf 매크로를 수행하
고, 사용 가능하지 않다면 action-if-not-found에 지정된 셸 스크립트 또는 autoconf 매
크로를수행한다.
사용 가능하지만 action-if-found가 생략되었다면 LIBS 변수에 -llibrary가 추가되고,

DEFS 변수에 모두 대문자인 -DHAVE_LIBlibrary=l 이 추가된다.
예를 들어 m 라이브러리가 링크 가능하다면 LIBS 변수에 -1m이 추가되고, DEFS 변수에

-DHAVE_LIBM=1 이 추가된다.
other-libraries 에는 다른 라이브러리와 같이 링크하지 않으면 링크 오류가 나는 라이브러
리인 경우처 럼 링크할 라이브러리를 공백 문자로 분리해 적는다.
가령 gtk 라이브러리와 같이 반드시 XII 라이브러리나 gdk 라이브러리와 링크해야만 링
크 오류가 나지 않는 라이브러리 같은 경우에는 [-1X11 -Igdk]와 같은 형식으로 적어준다.

AC_CHECK_LIB 매크로를 사용해 특정 라이브러리의 사용 유무를 체크하는 방법은 다
음과 같다.
AC_CHECK_LIB([m], [sin], [echo libm found!], [echo libm not found!])

위와 같이 configure.ac 파일에 추가하고 autoconf 명령-0-루 configure 스크립트를
새로 생성한다. 이후 configure 스크립트를 수행시키면 configure 스크립트는 sin 함
수를 호출하는 더미 C 소스 프로그램을 하나 만든다.
그리고 gcc 옵션으로 -1m 옵션을 주어 컴파일한다. 링크 오류 없이 정상적으로 컴파일
된다면 m 라이브러리와 링크해 sin 함수가 사용 가능하다는 의미다. m 라이브러리와
링크해 sin 함수가 사용 가능하다면 echo libm found! 명 령을 수행한다.
링크 오류가 발생한다면 m 라이브러리 안에 sin 함수가 없거나 해서 사용 불가능하다
는 의미다. 그럴 때는 echo libm not found! 명령을 수행한다.
새로 생성한 configure 스크립트를 수행해 보면 m 라이브러리와 링크해 sin 함수가 사
용 가능하기 때문에 다음과 같은 화면이 출력됨을 알 수 있다(m 라이브러리에 sin 함
수의 텍스트 코드가 들어 있다).

톲히 [screen 1 ： bash] rootG?'os：/temp/book/autoco「if
checking For gcc option to accept ANSI C... none needed
checking For sin in —im.yes |
libm found?
|
configure: creating ./config.status
config.status: creating Makefile
[root@os autoconf]tt

느______

[그림 12너3] configure 스크립트 수행

12장_ autoconf 611

===== PAGE 613 =====
위 예에서는 action-if-found 부분에 echo 명령을 넣었기 때문에 LIBS 변수와 DEFS
변수에는 아무 내용도 추가되지 않는다. action-if-found 부분 인자가 생략되었다면
기본 변수인 LIBS 변수와 DEFS 변수는 각각 “4m”, “-DHAVE_LIBM=1” 값이 추가된
다. 그리고 수행해야 될 명령이 여러 개라면 echo libm found； Is； ps처럼 세미콜론(；)
을 사용해 여러 명령을 한꺼번에 수행할 수 있다.
현재의 예제에서는 라이브러리를 링크하는 데 실패하더라도 “libm not found!” 메시지
만 출력하고 계속 수행한다. 실패 했을 때 중단하려 면 다음과 같이 사용한다.
AC_CHECK_LIB ( [m] , [kkkk] , AC_MSG_RESULT ( [libm found! ] ) , AC_MSG_
ERROR([libm not found!]))

위와 같은 행을 추가하고 다시 configure 스크립트를 수행시키면 kkkk 함수가 사용할
수 없기 때문에 다음과 같이 오류 메시지와 함께 configure 스크립트 수행이 중단되는
것을 확인할 수 있다.

조] [screen 1： bash] root@os:/temp/book;/autuconf
checking
whether
we
are
using
the
GNU
checking whether gee accepts -g— yes
checking for.gee.option to accept.ANSI C— none needed
checking for kkkk in —Im_____________ no
configure: error: libm not Found?
fjF‘6"6tQ6
autoconF]tt |

C

compiler...

yes

흐

[그림 12너4] configure 스크립트 수행 결과

위 예제에서 사용된 AC_MSG_* 매크로는 화면에 메시지를 출력하는 매크로인데, AC_

MSG_ERROR 매크로는 메시지를 출력하고 오류를 발생시켜 configure 스크립트 수행
을 중단시킨다. 메시지 출력과 관련된 매크로들은 다음과 같다. 그리고 메시지 관련 매
크로는 자주 사용하고 중요하기 때문에 자세히 보기 바란다.

AC_MSG__CHECKING(feafure-(yesc/7pf/'or7)
checking 메시지를 발생시킨다. 바로 위 그림에서 checking for •••에 해당하는 메시지다.

AC_M S G_RESULT (result-description)
결과 메시지를 줄력한다.

AC_M SG_NOTICE (message)
notice 메시지를 출력한다. configure : message 형식으로 출력한다.

AC_M SG_E R R0 R(error-description, [exit-status])
오류 메시지를 출력하고 configure 스크립트 수행을 중단한다.

612

5부—프로젝트빌드

===== PAGE 614 =====
AC_MSG_FAILURE(em)r-descr/pf/or7, [exit-status])
오류 메시지를 출력하고 configure 스크립트 수행을 중단한다. 그리고 “See 'conflgjog’

for more details.” 메시지를 출력한다.

AC_MSG_WARN (pro 이em-c/escr/pf/on)
경고 메시지를 출력한다. configure 스크립트 수행은 중단되지 않는다.

특정한 함수가 들어있는 라이브러리를 찾으려면 AC_SEARCH_LIBS 매크로를 사용한다.

AC_SEARCH_LIBS(/l/ncf/on, search-libs, [action-if-found], [action-if-not-found], [other-libraries])
주어진 함수(function)가 사용 가능한 라이브러리를 라이브러리 리스트인 search-libs에
서 찾는다.

사용 예는 다음과 같다. sin 함수가 c 라이브러리에 있는지, pthread 라이브러리에 있
는지, m 라이브러리에 있는지 확실히 알지 못할 때는 configure.ac 파일에 다음 행을
추가한다.
AC_SEARCH_LIBS([sin], [c pthread m])

위와 같이 사용하면 configure 스크립트가 sin 함수를 호출하는 더미 소스 프로그램을
작성하고 c, pthread, m 라이브러 리순으로 링크해 링크 오류가 발생하는지 발생하지 않
는지 체크한다. 링크 오류가 발생하지 않는다면 해당 라이브러리에 해당 함수가 있다는
의미이므로 LIBS 변수와 DEFS 변수에 링크가 가능한 라이브러리 값을 각각 추가한다.
결국 위 예제에서는 sin 함수가 사용 가능한 m 라이브러리를 찾아 LIBS 변수에 -1m을
추가하고 DEFS 변수에 -DHAVE_LIBM=1 을 추가한다.

| 헤더 파일 체크 매크로
특정 헤더 파일이 있는지 체크하려면 헤더 파일 체크 매크로를 사용한다. 헤더 파일 체
크 매크로는 컴파일될 수 있는 환경인지 결정하는 데 사용하고, 헤더 파일의 유무에 따
라 define과 include를 달리해야 할 때 많이 사용한다.

AC_CHECK_HEADER(/?eader-f/7e, [action-if-found], [action-if-not-found], [includes =
default-includes 7)
주어진

헤더

파일(header-file)을

찾으면

action-if-found를

수행하고,

찾지

못하면

action-if-not-found# 수행한다.

12장_ autoconf 613

===== PAGE 615 =====
AC_CHECK_HEADER 매크로는 다음과 같이 사용한다.
AC_CHECK_HEADER([linux/socket.h] , AC_MSG_RESULT([linux/socket.h
found!]), AC_MSG_WARN([Missing linux/socket.h header!]))

물론 위 예는 연결된 한 행이다. 이 행을 configure.ac 파일에 추가하고 autoconf 명
령으로 configure 스크립트를 생성한다. 생성된 configure 스크립트를 수행하면 C 전
처리기 cppO가 헤더 파일을 찾기 위해 탐색하는 경로인 /usr/local/include, /usr/lib/

gcc/i386-redhat-linux/[버전]/include,

/usr/include순으로

linux/socket.h

파일이

있는지 찾는다.
찾으면 action-if-found에 있는 명령을 수행하고, 못 찾았으면 action-if-not-found
에 있는 명령을 수행한다.
네 번째 인자인 includes 필드는 헤더 파일을 체크하는 데는 필요 없다. 나중에 구조체
와 타입을 체크할 때 따로 설명하겠다.

AC_CHECK_HEADERS(/7ea(yer-f/7es, [action-if-found], [action-if-not-found], [includes =
'default-includes 7)
주어진 헤더 파일 리스트인 header-files에서 각각의 헤더 파일을 찾는다. 각각의 헤더 파
일이

찾아지면 action-if-found 부분을 수행하고, 찾지

못하면 action-if-not-found 부분

을수행한다.

AC_CHECK_HEADERS 매크^는 다음•과 같巾] 사^한다.
AC_CHECK_HEADERS([dirent.h stdlib.h errno.h],
WARN([Missing header!]))

, AC_MSG_

위와 같은 행을 configure.ac 파일에 추가하고 configure 스크립트를 생성하면 dirent,

h와 stdlib.h, errno.h 파일을 각각 찾는다. 각각의 파일들을 찾으면 action-if-found
를 수행하고, 못 찾으면 action-if-not-found를 수행한다.
찾은 파일은 DEFS 변수에 -DHAW_파일명_확장자=1 형식으로 추가된다. 위 예에
서 모든 파일을 다 찾으면 DEFS 변수에 “-DHAVE_DIRENT_H=1 -DHAVE_STDLIB_

H=1 -DHAVE_ERRNO_H=1” 문자열이 추가된다. 이렇게 추가된 문자열은 gcc 컴파일
옵션으로 사용되어 헤더 파일의 유무에 따라 include* 달리할 때 사용된다.
헤더 파일을 찾는 미는 AC_CHECK_HEADER 매^■와 AC_CHECK_HEADERS
매크로 외에 특수한 헤더 파일을 찾는 매크로가 더 있다. 주로 이런 매크로는 같은 기

614

5부- 프로젝트빌드

===== PAGE 616 =====
능을 수행하는 헤더 파일이지만 플랫폼에 따라 이름이 틀린 헤더 파일을 찾을 때 사용
한다.
예를 들면 AC_HEADER_DIRENT 매크로는 dirent.h, sys/ndir.h, sys/dir.h, ndir.h를
순차적으로 찾아 어떤 헤더 파일이 먼저 선택되느냐에 따라 DEFS 변수에 추가되는

define 옵션이 틀려진다.
AC_HEADER_DIRENT 매크로가 먼저 선택되는 파일에 따라 DEFS 변수에 추가하는
define 은 다음과 같다.
dirent.h
sys/ndir.h
sys/dir.h
ndi r. h

HAVE_DIRENT_H
HAVE_SYS_NDIR_H
HAVE_SYS_DIR_H
HAVE_NDI,R_H

Makefile .in 에서 DEFS 변수를 gcc 옵션으로 사용해 컴파일하고 C 소스에서 define 에
따라 다르게 include할 코드를 다음과 같이 추가하면 플랫폼이 틀려도 각 플랫폼에 맞
는 디 렉토리 엔트리 헤더 파일을 include할 수 있다.
〔예제 12-9)

C 소스 예제

# if HAVE_DIRENT_H
# include <dirent.h>
# define NAMLEN(dirent) strlen((dirent)->d_name)
#else
# define dirent direct
# define NAMLEN (dirent) (dirent) ->d_namlen
# if HAVE_SYS_NDIR_H
# include <sys/ndir.h>
# endif
# if HAVE_SYS_DIR_H
# include <sys/dir.h>
# endif
# if HAVE_NDIR_H
# include <ndir.h>
# endif
#endif

특수 헤더 파일을 찾는 매크로는 주로 이럴 때 사용하므로 찾으려는 헤더 파일이 특
수 헤더 파일 매크로로 존재한다면 AC_CHECK_HEADER 매크로나 AC_CHECK_

HEADERS 매크로 대신 특수 헤더 파일 매크로를 사용하는 것이 좋다.

12장_ autoconf | 615

===== PAGE 617 =====
특수 헤더 파일 매크로와 해당하는 헤더 파일에는 다음과 같은 것들이 있다.
[표 12-2] 특수 헤더 파일 매크로

매크로

헤더 파일

AC_HEADER_【기RENT

dirent.h, sys/ndir.h, sys/dir.h, ndir.h

AC_HEADER_MAJOR

sys/types.h, sys/mkdev.h, sys/sysmacros.h

AC_HEADER_STAT

sys/stat.h

AC_HEADER_STDBOOL

stdbool.h

AC_HEADER_STDC

stdlib.h, stdarg.h, string.h, float.h

AC_HEADER_SYS_WAIT

sys/wait.h

AC_HEADER_TIME

time.h, sys/time.h

AC_HEADER_TIOCGWINSZ

sys/ioctl.h, termios.h

특수 헤더 파일에 해당하는 헤더 파일을 찾으려면 위 매크로를 사용해야 한다. 각 특수
헤더 파일 매크로에 대한 세부적인 변경 사항이나 내용은 부록에 자세하게 설명했으니
필요할 때 참고하기 바란다.

C6| 함수 체크 매크로
특정 함수가 사용 가능한지 가능하지 않은지, 그리고 사용 가능하다면 어떻게 사용해야
되는지 알려면 함수 체크 매크로를 사용한다.
함수 체크 매크로는 주로 같은 기능의 함수지만 함수명이 다르거나 함수의 인자가 다
른 경우 체크되는 함수의 형식에 따라 다른 소스로 컴파일하고자 할 때 사용한다. 예를
들면 이제는 더 이상 리눅스에서 사용하지 않는 getpgrp 함수는 프로세스의 그룹 ID
를 리턴하는 함수인데, 어떤 플랫폼에서는 getpgrp 함수가 인자를 사용하지 않고 어
떤 플랫폼에서는 인자로 0 을 사용했다. 이런 경우 configure.ac 파일에 AC_FUNC_

GETPGRP라는 함수 체크 매크로를 넣어주면 인자의 종류에 따라 DEFS 변수의 값이
설정된다. getpgrp 함수의 인자 값이 void라면 -DGETPGRP_yOID=l이 추가되고, 그
렇지 않다면 아무것도 추가되지 않는다.
이렇게 DEFS 변수에 추가된 값을 이용해 소스 코드 내에서 인자 값을 다르게 호출할
때 함수 체크 매크로가 사용된다.

616

5부_ 프로젝트 빌드

===== PAGE 618 =====
#if

GETPGRP_VOID
pid = getpgrp ();
#else
pid = getpgrp (0);
#endif

함수 체크 매크로에도 단순히 함수의 사용 가능 여부만 체크하는 일반 함수 체크 매크
로와 함수 사용 가능 여부에 따라 플랫폼에 따른 소스를 적용해 줘야 되는 특수 함수
체크 매크로가 있다.
일반 함수 체크 매크로에는 다음과 같은 것들이 있다.

AC_CHECK_FUNC(funcf/'on, [action-if-found], [action-if-not-foundf)
주어진 함수(function)가 사용 가능한지 체크한다. 사용 가능하면 action-if-found를 수행
하고, 그렇지 않다면 action-if-not-found를 수행한다.

사용 예는 다음과 같다.
AC_CHECK_FUNC([printf], , AC_MSG_ERROR([Invalid printf function!]))

configure.ac 파일에 위와 같은 행을 추가하고 configure 스크립트를 생성하면 스
크립트 수행 시에 printf 함수가 사용 가능한지 체크한다. 사용 가능하다면 아무 일도
수행하지 않고, 사용 가능하지 않다면 “Invalid printf function!” 메시지를 출력하고

configure 스크립트 수행을 중지한다.
AC_CHECK_FUNCS(functions, [action-if-fo nd], [action-if-not-found])
니

주어진 함수들의 리스트에서 각각의 함수가 사용 가능한지 체크한다. 사용 가능하면

action -if-found# 수행하고, 가능하지 않다면 action-if-not-found> 수행한다.
DEFS 변수에는 -DHAVE_함수명 = 1과 같은 형식으로 적절히 설정된다.

AC_CHECK_FUNCS 매크로를 사용하는 예는 다음과 같다.
AC_CHECK_FUNCS([printf

strdupb

,

AC_MSG_ERROR([Invalid

function!]))

configure.ac 파일에 위와 같은 행을 추가하고 configure 스크립트를 생성하면
configure 스크립트 수행 시 printf 함수와 strdup 함수가 사용 가능한지 체크한다.
사용 가능하다면 아무 일도 수행하지 않고 DEFS 변수에 “-DHAVE_PRINTF = 1

-DHAVE_STRDUP=1” 문자열이 추가된다. 사용 가능하지 않다면 “Invalid function!”
문자열을 출력한 후 configure 스크립트 수행을 종료한다.

12장_ autoconf 617

===== PAGE 619 =====
이상이 일반적인 함수 체크 매크로 사용의 예였다. 특수 함수 체크 매크로는 [표 12-3]
과 같다. 체크하려는 함수가 특수 함수에 포함된다면 특수 함수 매크로를 사용해 체크
해야 한다. 특수 함수 매크로 사용에 관한 구체적인 설명은 부록을 참고하기 바란다.
[표 12-3] 특수 함수 매크로

618

매크로

함수

AC_FUNC_ALLOCA

allocaO

AC_FUNC_CHOWN

chown()

AC_FUNC_CLOSEDIR_WID

closedir()

AC_FUNC_ERROR_ATJ」NE

error_at_line()

AC_RJNC_FNMATCH, AC_FUNC_FNMATCH_GNU

fnmatchO

AC_FUNC_FORK

fork(), vfork()

AC_FUNC_FSEEKO

fseekoO

AC_FUNC_GETGROUPS

getgroupsO

AC_FUNC_GETLOADAVG

getlodavgO

AC_FUNC_GETMNTENT

getmntent()

AC_FUNC_GETPGRP

getpgrpO

AC_FUNC 丄STAT_FOLLOWS_SUXSHED_SYMUNK

IstatO

AC_FUNC_MALLOC

wllocO

AC_FUNC_MEMCMP

memcmpO

AC_FUNC_MBRTOWC

mbrtowc()

AC_FUNC_MKTIME

mktimeO

AC_FUNC_MMAP

mmap()

AC_FUNC_OBSTACK

obstackO

AC_RJNC_REALLOC

reallocO

AC_FUNC_SELECT_ARGTYPES

selectO

AC_FUNC_SETPGRP

setpgrpO

AC_FUNC_STAT, AC_FUNC_LSTAT

stat(), IstatO

AC_FUNC_SEWBUF_REVERSED

setvbufO

AC_FUNC_STRCOLL

strcoll()

AC_RJNC_STRTOD

strtodO

AC_FUNC_STRERROR_R

strerror_r()

AC_FUNC_STRFWE

strftimeO

AC_FUNC_STRNLEN

strnlen()

AC_FUNC_UTIME_NULL

utime()

AC_FUNC_VPRINTF

vprintf()

AC_REPLACE_FNMATCH

fnmatch

5부_ 프로젝트빌드

===== PAGE 620 =====
I 구조체 및 타입 체크 매크로
AC_CHECK_MEMBER(aggregate.member, [action-if-found], [action-if-not-found], [includes

= 'default-includes'])
aggregate.member가 있는지 찾는다. 있으면 action-if-found를 수행하고, 없으면
action-if-not—found를 수행한다.

AC_CHECK_MEMBER 매크로는 주로 구조체를 찾을 때와 구조체에서 특정 멤버가 있
는지 확인할 때 사용하는 매크로다.
AC_CHECK_MEMBER(struct tm.tm_sec, AC_MSG_RESULT([tm struct found!]),
AC_MSG_ERROR([tm struct not found!]), [#include <time.h>])

configure.ac 파일에 위와 같이 행을 추가하면 configure 스크립트가 time.h를
include해 struct tm.tm_sec가 사용 가능한지 찾는다. 사용 가능하다면 “tm struct
found!” 문자열을 화면에 출력하고, 사용 가능하지 않다면 “tm struct not found!” 문
자열을 화면에 출력한 후 멈춘다.
AC_CHECK_MEMBERS(meznders, [action-if-found], [action-if-not-found], [includes =

'default-includes 7)
구조체 멤버 리스트인 members 각각을 구조체 멤버가 있는지 확인한다. 있으면 action-

if-fo니nd를 수행하고, 없으면 action-if-not-fo니nd를 수행한다.

AC_CHECK_TYPE(type, [action-if-found], [action-if-not-found], [includes = 'default-includes'])
type이 있는지 확인한다. 있으면 action-if-fo니nd를 수행하고, 없으면 action-if-notfound를 수행한다. includes가 있으면 includes를 incl니de해 체크한다.

타입 체크 매크로의 사용 예는 다음과 같다.
AC_CHECK_TYPE(time_t, AC_MSG_RESULT([time_t type found!]), AC_MSG_
ERROR([time_t type not found!]), [#include <time.h>])

위 예는 time.h를 include해 타입이 있는지 확인한다. time_t 타입이 있으면

type found!” 문자열을 출력하고, 없으면 type not found!” 문자열을
출력한다.
AC_CHECK_TYPES((ypes, [action-if-found], [action-if-not-found], [includes = 'default-includes'])
타입 리스트인 types가 각각 있는지 찾는다. 있으면 action-if-found 부분을 수행하고, 없
으면 action-if-not-found 부분을 수행한다.

12장_ autoconf 619

===== PAGE 621 =====
이상이 구조체와 타입 체크에 관련된 매크로였다. 구조체와 타입 체크 매크로 역시 특
수 구조체와 특수 타입 체크 매크로가 있다. 특수 구조체 매크로에 대해서는 부록을 참
고하기 바란다.

I 파일 체크 매크로
AC_CHECK_FILE(#7e, [action-if-found], [action-if-not-found])
AC_CHECK_FILE 매크로는 file이 있으면 action-if-found< 수행하고, 없으면 action-ifnot-found 를 수행한다.

AC_CHECK_FILES(files, [action-if-found], [action-if-not-found])
files

리스트에

있는

파일이

있으면

action-if-found<

수행하고,

없으면

action-if-not-

found를 수행한다. 한 번만 액션을 수행하는 게 아니라 해당하는 파일 각각의 유무에 따른
액션을 수행한다.

I 기타 유용한 매크로
AC_SUBST( variable)
configure.ac 파일에서 정의한 variable 변수를 Makefile .in 으로 넘겨줄 때 사용한다.

AC_SUBST 매크로는 굉장히 자주 사용하는 매크로이므로 기억할 필요가 있다.
AC_SUBST 매크로를 사용해 configure.ac 파일에서 정의한 변수를 넘겨주는 예는 다
음과 같다.
〔예제 12-10〕 configure.ac 파일 내용

AC_INIT(diary, 0.0.1, woos@mymail.com)

；

AC_PROG_CC

：

INCPATH=/root/include
AC__SUBST ([ INCPATH ] )
AC_CONFIG_FILES ( [Makefile] )
AC_0UTPUT

620

5부_ 프로젝트 빌드

：

===== PAGE 622 =====
〔예제 12-11〕 Makefile.in 파일 내용

CC = @CC@
CFLAGS = @CFLAGS@
INCPATH = @INCPATH@
all : Like
like : like.c

$(CC) $(CFLAGS) -1$(INCPATH) -o $@ $

위와 같이 각각의 파일을 작성하고 생성한 configure 스크립트를 수행하면 [그림

12-15]와 같이 Makefile의 configure.ac 파일 내에서 AC_SUBST 매크로로 넘겨준
INCPATH 변수 값이 치환되어 있는 것을 확인할 수 있다.

[그림 12-15] INCPATH 변수가 치환된 예

configure.ac 파일에서 사용된 INCPATH 변수는 configure 스크립트에서 셸 변수로
설정되고, INCPATH 변수를 Makefile .in（정확히 이야기하면 config.status 스크립트）
파일에 넘겨주는 스크립트가 추가된다.

AC_DEFINE（ ctef/'ne, [value], [description]）
Makefile.in

파일로

-Ddefine=value

넘어가는

형식으로

DEFS

추가된다.

변수에

-Ddefine을

description은

추가한다.

value이

AC_CONFIG_HEAD

사용되면

매크로가

사용

되었을 때 AC_CONFIG_HEAD가 지정하는 파일에 define 설명으로 들어갈 내용이다（뒤
에 있는 설정 헤드 부분을 참고하기 바람）.

AC_DEFINE 매크로 역시 매우 자주 사용되는 매크로다. AC_DEFINE 매크로를 사용하
는 예는 다음과 같다.

12장_ autoconf 621

===== PAGE 623 =====
〔예제 12너2〕

configure.ac 파일 내용

AC_INIT(diary, 0.0.1, woos@mymail.com)
AC_PR0G_CC
AC_DEFINE([HELLO] , [1] )
AC^DEFINE([WORLD], [0])
AC_CONFIG_FILES ( [Makefile] )

AC^OUTPUT"
（예제 12-13〕 Makefile.in 파일 내용

cc = @cc@
CFLAGS = @CFLAGS@
DEFS = @DEFS@
all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS) -o $@ $

위와 같은 파일을 각각 작성하고 autoconf 명령으로 configure 스크립트를 생성한 후
수행하면 다음과 같은 Makefile이 생성된다.

배 [screen
CC
CFLAGS
DEFS

1 ： bash]root@os：/temp/book/autoconfj
= gcc
= -g -02
= -DPfiCKAGE_NfiME=tf"diaryW"
-DPACKAGE_TfiRNAME=tt"diaryW,'
DPfiCKfiGE uERS10N=tt”0.0.1tt" —DPACKficE SJRINGW'diaryW O.fl.W"
DPACKAGE2BUGREP0RT=tf"woos@mymail.con@"j-DHELL0=1 BwORLD
5]

三

all : like
like : like .c
$(CC) $(CFLAGS) $(DEFS) -O $@ $"

I— 끼워봏기 --

모두 Pl

11,1

[그림 12-16] Makefile의 내용

make 명령을 내리면 컴파일 옵션으로 AC_DEFINE 매크로로 넘겨준 define 옵션이
추가되어 컴파일되는 모습을 ［그림 12-1 刀과 같이 확인할 수 있다.
• ■] [screen 1:
[root@os autoconFI]# rm -rf like
[rootSos autoconFI]tt make
gcc -g -02 -DPACKfiGE_NAME
#"diarytt" -DPACKAGE_TARNAME=tf"diarytf"
,, -D
-DPfiCKAGE_UERSION=W"0.0.1W" -DPfiCKfiGE STRING^^’diarytt
1
PfiCKfiGE—BilGREPORTMirvjoost
iwiail.coiW~[-DHELL0=1 -bwGRLD=B | -o li
ke like.c
[root@os autoconFI]# |

나

흐

흐쓰 바

긔
［그림 12너 7］ make 명령 수행

622 5부— 프로젝트 빌드

===== PAGE 624 =====
AC_CANONICAL_SYSTEM
시스템의 정보를 수집한다. host, host_cpu, host_vendor, host_os, target, target_cpu,

target_vendor, target_os, build, b니ild_cpu, b니ild_yendor, b니ild_os 둥의 변수에 각각
의 정보가 저장된다.

AC_CANONICAL_HOST
시스템의 정보를 수집한다. host, host_cpu, host_yendor, host_os 둥의 변수에 각각의
정보가 저장된다.

AC_OUTPUT_COMMAN DS(exfra-cn7ds, [init-cmds])
config.status 스크립트 수행이 끝나면 extra-cmds를 수행한다. init-cmds가 있으면
config.status 스크립트 수행 전에 init-cmds를 먼저 수행한다.

이상이 자주 사용하는 autoconf 매크로이고, 설명한 것 외에도 수많은 autoconf 매크
로가 있다. 부록에 있는 autoconf 매크로 리스트를 참고하고 부록의 내용이 부족하다
면 http://www.gnu.org/software에 있는 매뉴얼을 참고하기 바란다.

7 L 세밀한 제어를 위한 configure.ac 작성 |
autoconf를 사용하다 보면 autoconf에서 정의되어 있는 매크로만으로는 도저히 하기
힘든 일들이 있다. 예를 들면 configure 스크립트가 수행하면서 사용자의 입력을 받는
다든지 하는 경우가 대표적이다. 이렇게 configure 스크립트를 좀 더 세밀하게 설정하
려면configure.ac 파일에 셸 스크립트를 직접 넣어야 한다.

configure.ac 파일에 작성된 각각의 매크로들은 m4에 의해 셸 스크립트로 치환된
다. configure.ac 파일 내에 autoconf 매크로로 정의되지 않은 문자열을 만나면 바로

configure 스크립트로 복사된다. 이런 특징을 이용하면 configure 스크립트에 우리가
원하는 기능을 수행하는 셸 스크립트를 넣을 수 있다. 단, 몇 가지 주의 사항을 알고 나
서 말이다.

12장_ a 니 toconf 623

===== PAGE 625 =====
〔예제 12-14〕! configure.ac 파일의 내용

AC_INIT (like, 0.0.1, woos@mymail.com)
if test -f "kerneldir.h"; then
KERNEL__DIR=' cat kerneldir .h 2> /dev/null ’
else
KERNEL_DIR="/usr/src/linux"
fi
clear
echo
echo -ne "ARM Linux source directory [[ $KERNEL_DIR ]]
read KERNEL_DIR_TMP
if test "$KERNEL_DIR_TMP” != then
KERNEL_DIR=$KERNEL_DIR_TMP
fi
echo $KERNEL_DIR > kerneldir.h
CFLAGS="$CFLAGS -I$KERNEL_DIR/include"
AC_PROG_CC
AC_CONFIG_FILES ( [Makefile] )
AC OUTPUT

(예제 12-15]

? Makefile.in 파일의 내용

cc

= @cc@

CFLAGS

= @CFLAGS@

a丄1 : like
like : like.c
$(CC) $(CFLAGS) -o $@ $?
clean :
-rm -rf like

configure.ac 파일을 보면 셸 스크립트가 추가됐다. 이렇게 추가된 셸 스크립트는
configure 스크립트에 그대로 복사된다.
셸 스크립트를 잘 모르는 독자라면 다소 복잡하게 느껴질지 모르겠다. 그러나 셸 스크
립트에 현혹되지 말자. 이 예제를 통해 알고자 하는 것은 셸 스크립트가 아니라 셸 스
크립트를 configure.ac 파일에 추가하는 방법 이다.

624 부— 프로젝트 빌드

===== PAGE 626 =====
if test -f "kerneldir.h”; then
KERNEL_DIR=’cat kerneldir.h 2> /dev/nul丄’
else
KERNEL_DIR=H/usr/src/linux"
fi

위 스크립트는 test 명령으로 현재 디렉토리에 kerneldir.h 파일이 있는지 찾는다. 있으
면 KERNEL_DIR 셸 변수에 kerneldir.h 파일의 내용으로 값을 설정하고, 파일이 없으
면 7usr/src/linux” 문자열을 KERNEL_DIR 변수 값으로 설정한다.
주의 깊게 볼 점은 if문을 사용할 때 대괄호([])를 사용하지 않고 test 명령을 사용했다
는 점이다. 보통 셸 스크립트를 작성할 때 위와 똑같은 의미로 다음과 같이 test 명령
대신 대괄호를 사용해 작성하곤 한다.
if [ -f "kerneldir.h" ]; then
KERNEL_DIR=’cat kerneldir.h 2> /dev/null’
else
KERNEL_DIR="/usr/src/lirmx"
fi

[ 명령이나 test 명령이나 어차피 같은 명령이다. 유닉스 시스템에서 test 명령의 심볼
릭 링크로 [ 명령이 있기 때문이다. 의심스러운 독자는 Is -al /usr/bin/[ 명령을 내려
보기 바란다.

configure.ac 스크립트에 셸 스크립트를 추가할 때는 [ 명령 사용에 '주의해야 한다.
m4에서 대괄호는 문자열을 의미하므로 configure 스크립트에 적용될 때 대괄호가 없어
지기 때문이다. 그래서 [ 명령을 사용한 셸 스크립트는 다음과 같은 형식으로 configure
스크립트에 추가된다.
if -f "kerneldir.h" ; then
KERNEL_DIR=’cat kerneldir.h 2> /dev/null’
else
KERNEL_DIR="/usr/src/linux"
fi

저렇게 되면 당연히 오류가 발생한다. test 명령을 사용하면 대괄호가 없어지는 문제를
걱정하지 않아도 되지만 굳이 test 명령 대신 [ 명령을 사용하고자 한다면 다음과 같이
대괄호를 두 개 붙여야 한다.
if [ [ -f ’’kerneldir.h" ] ] ; then
KERNEL_DIR=’cat kerneldir.h 2> /dev/null'
else
KERNEL_DIR=’’/usr/src/linux"
fi

12 장 _ autoconf

625

===== PAGE 627 =====
while문을 사용하는 데도 마찬가지다. while test -f "/etc/passwd’’； 처럼 사용하던지
아니면 while [[ -f "/etc/passwd" ]]；처럼 사용해야 한다.

configure.ac 예제를 보면 echo 명령으로 출력하는 부분도 [[ $KERNEL_DIR ]]과 같
이 대괄호를 두 개 사용한 것을 확인할 수 있을 것이다.
또 다른 주의 사항은 셸 변수의 사용에 있다. 셸 변수명으로 “AC_”나 “AM_”로 시작하는
변수명을 사용해서는 안 된다.

m4 가 AC_ 로 시작하는 셸 변수를 만나면 autoconf 매크로로 인식하기 때문에 매크
로가 정의되지 않았다는 오류 메시지를 출력한다. 그리고 AM% 시작하는 변수명은

automake의 매크로로 인식해 오류가 발생한다.
clear
echo
echo -ne "ARM Linux
read KERNEL_DIR_TMP

source

directory

[

[

$KERNEL_DIR

]

]

:

’’

if test "$KERNEL_DIR_TMP" != then
KERNE L_DIR= $ KERNEL_DIR_TMP
fi
echo $KERNEL_DIR > kerneldir.h
CFLAGS="$CFLAGS -I$KERNEL_DIR/include"

셸 스크립트의 다음 내용은 화면을 지우고 “ARM Linux source directory [ $KERNEL_

DIR ] ： ” 문자열을 출력한 후 사용자 입력을 KERNEL_DER_TMP 변수에 받아 입력이
있었는지 체크한다. 입력이 있었으면 KERNEL_DIR 변수 값을 갱신하고 새로운 값으로

kerneldir.h 파일에 적용한다.
“CFLAGS="$CFLAGS -I$KERNEL_DIR/include"” 부분에서 CFLAGS 셸 변수 값을 새
로 설정하는데, CFLAGS 변수는 ACJNIT 매크로가 확장되어 추가되는 셸 스크립트에
이미 정의되어 있다. 이렇게 설정된 CFLAGS 변수는 Makefile.in 파일로 전달되어

@CFLAGS©에서 변수의 내용으로 치환된다.
감이 빠른 독자는 여기서 Makefile.in 파일로 전달되는 autoconf 변수가 configure 스
크립트의 셸 변수라는 것을 알 수 있을 것이다. 이전에 AC_PROG_YACC 매크로를 사
용하면 Makefllejn 파일로 YACC 변수가 전달된다는 것을 확인했다. YACC 변수 역시

AC_PROG_YACC 매크로가 셸 스크립트로 확장되면 그 속에 셸 변수인 YACC 변수로
존재한다.

626

5부_ 프로젝트 빌드

===== PAGE 628 =====
위 예제로 생성된 configure 스크립트를 수행시키면 다음과 같이 추가한 셸 스크립트
가 제대로 수행됨을 확인할 수 있다.

[그림 12너8] ./configure 명령 수행

여기서 새로운 커널 디렉토리를 입력하면 Makefile에 적용된다.
M [screen 1：

브as비 joat@os:/temp/book/autoconf

[root@os agtoconF]tt make
gcc -g -0
-I/roo£/include'] -o like like.c
[rootQos aiitoconF]tt |

기

[그림 12너9] make 명령 수행

08 설정 헤더를 사용해 소스 파일에
설정적용
지금까지 배운 내용대로 소스 파일에 설정을 적용한다면 컴파일 옵션에서 DEFS 변수
를 추가해 -D 옵션으로 define을 적용하는 방법밖에는 없다.
이렇게 적용하는 방법에는 두 가지 문제가 있는데, 컴파일 명령이 너무 길어져 컴파일
오류 메시지가 발생했을 때 메시지를 확인하는 것이 용이하지 않다는 점과 명령 길이
제한에 걸릴 수 있다는 점 이다.

autoconf는 설정을 소스 파일에 적용하기 위한 좀 더 유연한 방법을 제공하는데, 바로
설정 헤더를 사용하는 것이다. 설정 헤더를 사용하려면 AC_CONFIG_HEADER 매크로
를 사용하는데, 다음 예제를 보면 어떻게 사용하는지 알 수 있다.
〔예제 12-16)

like.c 파일의 내용

#include <stdio.h>
#ifdef HAVE_CONFIG_H
#include ”config.h"
#endif

12 장 _ autoconf 627

===== PAGE 629 =====
int main()
{
#if INSERT_CODE == 1
printf("insert code!\n");
#endif
printf ("I like you.\n");
#if REMOVE_CODE == 1
printf("remove code?\n”);
#endif
return 0;
}

〔예제 12-17〕 Makefile.in 파일의 내용

CC = @CC@
CFLAGS
DEFS

= @CFLAGS@
= @DEFS@

all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS) -o $@ $A
clean :
rm -rf *.o like

like.c 소스 코드를 자세히 보면 define되는 매크로에 따라 서로 다른 문장이 출력됨을
알 수 있다. 소스 코드를 작성 했으면 config니re.ac 파일을 다음과 같이 직성 한다.
（예제 12-18〕 configure.ac 파일 내용

AC_INIT(like, 0.0.1, woos@mymail.com)
AC_CONFIG_HEADER ([config.h])
AC_PROG_CC
AC_DEFINE([INSERT_CODE], [1], [Description : INSERT__CODE define])
AC_DEFINE([REMOVE_CODE], [0], [Description : REMOVE_CODE define])
AC_CONFIG_FILES ( [Makefile] )
AC_OUTPUT

628

5부—프로젝트빌드

===== PAGE 630 =====
AC_CONFIG_HEADER([config.h]) 매크로가 추가된 것을 확인할 수 있다. 그리고
AC_DEFINE 매크로가 추가되 었는데, 하나는 INSERT_CODE를 define하고 값을 1로
주었고 다른 하나는 REMOVE_CODE를 define하고 값으로 0을 주었다.

AC_CONFIG_HEADER 매크로를 사용하지 않았다면 이 렇게 define한 매크로는 DEFS
변수에 “-DINSERT_CODE = 1 -DREMOVE_CODE=0”과 같은 형식으로 추가될 것
이다. 그러나 AC_CONFIG_HEADER를 사용했기 때문에 DEFS 변수에는 -DHAW_

CONFIG_H만 들어가고, define된 내용■은 모두 config.h 파일에 “#define INSERT_
CODE 1”과 같은 형식으로 적용된다.
configure.ac 파일을 위와 같이 작성했으면 이제 configh 파일의 템플릿 파일이 될
config.h.in 파일을 작성해야 한다. config,h.in 파일은 다음과 같은 내용이 포함되어야
한다.
〔예제 12-19)

config.h.in 파일의 내용

#undef INSERT_CODE
#undef REMOVE_CODE

config.h.in 파일의 내용을 기초로 config.status 스크립트는 config.h 파일을 생성하는
데, DEFS 변수에 적용된 define에 대해서 설정해 configh 파일을 생성한다.

config.h.in 파일은 직접 작성해도 되고 autoheader를 사용해 자동.0.루 생성해도 된다.
autoheader 명령은 configure.ac 파일에서 사용된 AC_CONFIG_HEADER 매크로에
인자로 사용된 파일에 .in이 붙은 파일을 생성한다.

autoheader 명령은 .in 파일을 생성할 때 config니re.ac에 사용된 매크로에서 생성될
수 있는 define을 일일이 찾아내 #undef [C 매크로명] 형식으로 .in 파일의 내용을 채
운다.
필자는 autoheader 명령으로 config.h.in 파일을 생성했다.
IB [screen 3： bash] root@os :/temp/book/autoconf
[root@os autoconf ] tt] auioKeGtiG'i：’[~
[root
os autoconf]#
[root
os autoconf]tt Is config.h.in
config.h.in"]
[root
os autoconf]tt |

（흐
（흐
（ 흐

[그림 12—20] a니toheader 명령으로 config.h.in 파일을 생성한 예

12 장 _ autoconf 629

===== PAGE 631 =====
생성된 config.h.in 파일을 열어보면 다음과 같은 내용으로 되어있다.
〔예제 12-20〕 config.h.in 파일의 내용

/* config.h.in. Generated from configure.ac by autoheader. */
/* Description : INSERT__CODE define */
#undef INSERT_CODE
/* Define to the address where bug reports for this package should
be sent. */
#undef PACKAGE_BUGREPORT
/* Define to the full name of this package. */
#undef PACKAGE_NAME
/* Define to the full name and version of this package. */
#undef PACKAGE_STRING
/* Define to the one symbol short name of this package. */
#undef PACKAGE_TARNAME
/* Define to the version of this package. */
#imdef PACKAGE_VERSION
/* Description : REMOVE__CODE define */
#undef REMOVE_CODE

AC_DEFINE 매크로를 사용해 넘겨준 INSERT_CODE 매크로와 REMOVE_CODE가
각각 undefine되어 있음을 확인할 수 있다. 그리고 AC_DEFINE 매크로의 세 번째 인
자로 사용된 “Description : …” 문자열이 각 C 매크로 위에 주석으로 들어가 있음도
확인할 수 있다.
이제 autoconf 명령으로 configure 스크립트를 생성하고 configure 스크립트를 수행
하면 Makefile과 함께 config.h 파일도 생성됨을 확인할 수 있다.
g) [screen 3： bash] root@os：/temp/book/autoconf
checking For gcc option to accept ANSI C___________________ none needed
configure: creating ./config.status
config.status: creating Makefile
config.status: creating config.h
[rootBos autoconF]tt
[root
os autoconf]tt is config.h
configTh"]
troofio
autoconf]tt |

(흐
厂

[그림 12—21] configure 명령으로 생성된 config.h

630

5부_ 프로젝트 빌드

===== PAGE 632 =====
config.h 파일을 열어보면 [예제 12-21]과 같이 undefine되어 있던 부분들이
configure 스크립트가 수행되면서 수집한 정보에 의해 변경되었음을 확인할 수 있다.
〔예제 12-21)

생성된 config.h 파일의 내용

/* config.h. Generated by configure .
*/
/* config.h. in. Generated from configure.ac by autoheader.

*/

/* Description : INSERT_CODE define */
#define INSERT_CODE 1
/* Define to the address where bug reports for this package should
be sent. */
#define PACKAGE_BUGREPORT ”woos@mymail.com"
/* Define to the ful丄 name of this package. */
#define PACKAGE_NAME "like"
/* Define to the ful丄 name and version of this package. */
#define PACKAGE_STRING "like 0.0.1”
/* Define to the one symbol short name of this package. */
#define PACKAGE_TARNAME "like"
/* Define to the version of this package. */
#define PACKAGE_VERSION ”0.0.1"
/* Description : REMOVE_CODE define */
#define REMOVE_CODE 0

생성된 Makefile을 열어보면 ［그림 12-22］ 와 같이 DEFS 변수의 내용에 -DHAVE_

CONFIG_H만 들어 있는 것을 확인할 수 있다.
V] [screen 3： bash] root@os：/temp/book/autoconf

所

= 으—

CFLfiGS
DEFS

=|-6HAUE CONFIG H

厂厂一厂

= -g -02

|

all : like
like : like.c
$(CC) $(CFLAGS) $(DEFS) -o $@ $?
clean :
rm -rF like
____________________________________________________________ 1,1 꼭대기

Bl

[그림 12—22] Makefile의 내용

12 장 _ autoconf

631

===== PAGE 633 =====
AC_CONFIG_HEADER 매크로를 사용하면 DEFS 변수에 들어가는 define 설정은 모
두 AC_CONFIG_HEADER에서 지정한 파일로 들어가고 단지 -DHAVE_파일명(예:

-DHAVE_CONFIG_H) 만이 저장된다.
like.c 소스 파일을 보면 “HAVE_CONFIG_H 매크로가 정의 되 었다면 config.h 파일을
include하라”는 부분을 확인할 수 있는데, HAVE_CONFIG_H는 Makefile에서 컴파일
옵션으로 지정하여야 한다.
이제 make 명령으로 컴파일한 후 ./like 명령을 내리면 define된 설정에 따라 소스가
전처리 과정에서 변경된 것을 확인할 수 있다.
g

[screen

3：

bash]

root@os：/temp/book/autoconf

[root@os autoconf jtt liiake]
gcc -g -02 -DHfiUE_CONFIG_H -o like like.c
[rooteos autoconf]#
[rootBos autgconf]tt ./like
insert code?
I like you.
[root@iDs’HitoconF]ft |

[그림 12-231 ./like 명령 수행

이상이 컴파일 옵션을 사용하지 않고 설정 헤더를 사용해 설정을 적용한 예였다. 이전
에도 말했지만 컴파일 옵션에서 DEFS 변수에 넘어오는 define을 적용하는 것은 명령
길이 제한도 문제지만 무엇보다 너무 많은 컴파일 옵션으로 인해 컴파일 과정 파악이
힘들어 주로 설정 헤더를 사용하곤 한다.
지금까지가 autoconf의 내용이었다. 필자가 전반적인 내용은 다 설명했지만 autoconf
에 대해서 아직도 이야기할 것이 많이 남아 있다.
나머지는 독자가 직접 알아보기 바란다. 지금까지의 내용만으로도 autoconf를 사용하
는 데 부족함이 없고, 또한 새로운 autoconf 기술을 익히는 데 힘들지 않을 것이다.

GNU 온라인 매뉴얼과 여러 프로젝트 파일에서 사용된 configure.ac 또는 configure,
in 파일의 내용을 참고삼아 하나씩 익혀가기 바란다.

632

&부- 프로젝트 빌드

===== PAGE 634 =====
13
automake

01 automake의 구조와 원리
02 따라 해보기
03 Makefile.am 파일 작성 규칙
04 재귀적 M기＜efile.am 파일 작성

===== PAGE 635 =====
앞서 Makefile 의 템플릿 파일인 Makefile.in 파일을 직접 작성해 만들었다. 이렇게 직접
작성하는 방법의 문제점은 configure 스크립트가 수집하는 시스템 정보의 양은 많은 데
비해 Makefile.in 에서 사용하는 정보는 적다는 점이다. 그래서 좀 더 높은 이식성을 제
공할 수 없다.
그리고 이전에 테스트하면서 작성한 Makefile.in 파일은 기능이 아주 단순해 작성하는
데 시간이 얼마 걸리지 않았지만 많은 기능을 Makefile.in 파일에 넣으려면 작성하는 데
많은 시간이 걸린다. automake는 이런 문제를 해결하기 위해 만들어졌다.

===== PAGE 636 =====
01 | automake의 구조와 원리
automake는 Makfile.in 파일을 생성하는 유틸리티다. 이렇게 생성된 Makefile.in 파일
은 GNU 표준을 따르는 Makefile이며 많은 기능이 추가되었고, 또한 많은 시스템 정보
를 이용하기 때문에 직접 작성하는 것보다 이식성이 높다.

[그림 13-1] automake 구조도

［그림 13-1］ 은 automake를 잘 설명하고 있다. automake는 Makefile.am 파일을 입
력으로 받아 Makefile.in 파일을 생성한다. 이렇게 생성된 Makefile .in 파일은 config,

status 스크립트에 의해 Makefile로 변경된다.
Makefile.am 파일은 automake가 이해하는 변수로 구성되어 있고, 이런 변수를 사용
해 Makeflie.in 파일의 빌드 방법을 설정할 수 있다.

a니toconf와 automake를 사용해 전체 프로젝트를 빌드하는 과정을 그림으로 나타내
면 다음과 같다.

13장_ automake 635

===== PAGE 637 =====
Makefile.am

automake

[그림 13-2] autoconf와 automake의 구조도

2 L 따라 해 보기
automake를 사용해 어떻게 Makefilejn 파일을 생성할 수 있는지 알아보자.
소스 파일인 like.c 파일은 그대로 이용하기로 하고 configure.ac 파일에서 AC_INIT
매크로 바로 뒤에 AMJNIT_AUTOMAKE 매크로를 추가해 autoconf에게 automake
를 사용한다는 것을 알려준다.

AMJNIT_AUTOMAKE 매크로에는 두 개의 인자가 들어가는데, 하나는 프로젝트명이
고 나머지 하나는 프로젝트 버 전이다.
〔예제 13-1)

configure.ac 파일 내용

AC_INIT(like, 0.0.1, woos@mymail.com)
AM_INIT_AUTOMAKE(like, 0.0.1)
AC_PROG_CC
AC_CONFIG_FILES ( [Makefile] )
AC_OUTPUT

636 5부— 프로젝트 빌드

===== PAGE 638 =====
configure,ac 파일을 작성 했다면 이제는 Makefile.am 파일을 작성한다. Makefile.am
파일은 어떤 일을 하는 Makefllejn 파일을 생성할지 automake에 알려주는 파일이다.
어떤 일이란 컴파일해 생성할 바이너리 파일명은 무엇이며, 소스 파일에는 어떤 것들이
있고, make instaU 명령을 내렸을 때 어떤 디렉토리에 설치되는지 등의 일을 의미한다.
〔예제 13-2)

Makefile.am 파일의 내용

bin_PROGRAMS
like_SOURECS

= like
= like.c

Makefile.am 파일 작성 규칙에서 각 변수가 의미하는 바를 따로 설명하겠지만 간단
하게 설명하면 bin_PROGRAMS 변수는 make install 명령 수행 시 autoconf 변수인

bindir 변수에 설정되어 있는 디렉토리에 설치될 프로그램 파일명이 like라는 의미다.
또한 프로그램이기 때문에 컴파일해야 된다는 의미도 있다. 그리고 like_SOURCES 변
수의 의미는 like 프로그램의 소스 파일에는 like.c가 있다는 의미다.
이렇게 작성했으면 aclocal 명령을 수행해 aclocal.m4 파일을 생성한다. aclocal.m4는

m4 매크로로 구성되고, automake를 사용하기 위 한 여러 체크 항목을 정의 한다.

[그림 13-3] aclocal 명령으로 aclocal.m4 파일 생성

이제 autoconf 명 령으로 config니re 스크립트를 생성 한다.
autoconf

마지막으로 automake 명령으로 Makefile .in 파일을 생성한다.
automake —-foreign --add-missing ——copy

關 [screen 3： bash] root®os:/temp/book/autoconf
히
으 厂一for ei'흐;데 add

[root@o^~airtoconf ]
ayton
ke
configure .ac: installing tT7instai1-sh'
configure.ac: installing ' ./inkinstalldirs'
configure.ac: installing './missing'
Makefile.am: installing './depcomp'
[root@os autoconF]tt
[rootBos au(oconf]1t Is Makefile.in
Makefiie.ini
[root00s autoconF]tt
[rootBos autoconFjtt |

厂.

[그림 13-4] automake 명령으로 Makefile.in 파일 생성

13 장 _ automake

===== PAGE 639 =====
------------- 옵션은 엄격성을 foreign으로 맞추라고 automake에 주문하는 옵션이다.
원래 automake는 GNU 패키지 관리자가 사용하는 유틸리티로, 패키지에 반드시 들어
가야 하는 파일들과 Makffle 타겟이 GNU 표준으로 엄격하게 규정되어 있다.
예를 들면 INSTALL, COPYING, AUTHORS, ChangeLog, NEWS, README 같은 파
일이 대표적인데, 엄격성을 foreign으로 주지 않으면 이런 파일들이 없어 Makefile.in
파일이 만들어지지 않는다. foreign은 가장 낮은 엄격성으로 automake가 동작하는 데
꼭 필요한 검사만 수행하므로 이런 파일들이 없어도 Makefilejn 파일이 만들어진다.

automake에서 정의되어 있는 엄격성은 다음과 같다.
［표 13-1］ automake의 엄격성 종류
어겨서
□ —1 O

옵션

설명
BSD cygnus 규칙을 따른다.

cygnus

cygnus

foreign

——foreign

가장 낮은 엄격성

gn 니

—-gnu

GNU 표준으로 중간 정도의 엄격성

gnits

——gnits

가장 높은 gnits 엄격성을 따른다.

--add-missing 옵션은 automake로 작성된 Makefile.in 내부에서 사용하는 명령들을
추가하라는 옵션이다. install-sh, mkinstaildirs, missing, depcomp가 대표적인 명령
들이고, /usr/share/a니tomake-버전 디렉토리에 이런 파일들이 들어있다.

--copy 옵션이 붙지 않으면 /usr/share/automake-버전 디렉토리에 있는 파일들을
심볼릭 링크해 추가하고, —copy 옵션이 붙으면 복사해 추가한다.

automake로 생성된 Makefile.in 파일을 열어보면 ［그림 13-5］ 와 같이 여러 시스템 정
보를 모두 활용하는 이식성 있는 Makefiles이 만들어졌음을 확인할 수 있다.
OH [screen 3： bash] root@os：/temp/book/autoconf
AMTAR =~@AMTAR@
AUK = @AWK@
CC = @CC@
DEPDIR = @DEPDIR@
INSTfiLL_STRIP_PROGRfiM = @INSTALL_STRIP_PROGRAM@
PACKAGE = @PACKAGE8
STRIP = @STRIP@
UERSION = @UERSI0N@
an_include = dam_included
an_quote = ______ _____________
installsh = @install_sh@
bin_PROGRfiMS = like
]ike_SOURECS = like.c
"Makefile.in” 39BL, 11822C

［그림 13-5］ 생성된 Makefile.in 파일의 내용

638

5부— 프로젝트 빌드

===== PAGE 640 =====
./configure 명령을 수행한 후 make 명령을 내리면 ［그림 13-6］ 과 같이 like 파일을
컴파일한다.
■•'I [screen 3： bash] root@os：/temp/book/autoconf

I

리—

[root@os autoconF jit' nal
source='like.c' object='like.o’ libtool=no W
depFile=,.deps/like.Po' tnpdepFile=*.deps/like.TPo' tf
depmode=gcc3 /bin/sh ./depconp tf
,, -DPACKAGE_TARNAME=W"likeW" -DPACKAGE
gcc -DPACKAGE_NfiME=W"lil
_UERSION=W"0.0.1tf" -DPACKftGE_STRING=W"likeW 0.0.W" -DPACKAGEBU
EREPORT
TwoosSinymail.comW" -DPACKAGE=W'likeW" -DUERSION
"0.6.1
-I. -I. -g -02 -c 'test -F 'like.c' 11 echo './''like.c
gcc -g -02 -o like like.o
[root
os autoconf]9
[root
os autoconf]tt Is like
iike |
[root@os autoconf]tt ./like
I like you.
[root@os autoconf]tt j________________________________________________________________

《마#

나！

나#

（흐
여

［그림 13-6］ make 명령 수행

지금까지 automake< 사용해 Makefile .in 파일을 생성하는 예를 살펴봤다. 결국 우
리가 원하는 Makefile .in 파일을 생성하려면 Makefile.am 파일을 잘 작성해야 한
다. Makefile.am 파일을 작성하는 일 역시 간단한 규칙만 알면 의외로 쉽다. 그럼

Makefile.am 파일을 작성하는 규칙을 알아보자.

C3| Makefile.am 파일 작성 규칙
Makefile.am 파일을 작성할 때 가장 먼저 알아야 될 것은 Makefile.am 파일에서 사용
하는 변수의 명명법이다. automake 변수는 프로그램의 빌드, 설치, 테스트 등에 관한
골격을 잡아주는 역할을 수행한다.
접두어_주요변수명 예） bin_PROGRAMS

automake 변수는 위와 같은 형식으로 되어 있다. 앞부분에 주요 접두어가 오고 언더
바（ J 다음에 주요 변수명이 나온다.
접두어는 파일을 설치할 방법과 설치될 디렉토리를 automake에게 알리는 역할을 한
다. 가령 접두어로 sbin이 붙으면 configure 스크립트에서 Makefilejn으로 넘기는 변
수 중 sbindir 변수가 지정하는 디렉토리에 설치한다는 의미다. 그래서 이렇게 생성된

Makefile로 make install 명령을 내리면 해당 파일을 sbindir 변수가 지정하는 디렉토
리에 설치한다.

13장_ automake 639

===== PAGE 641 =====
configure 스크립트에서 Makefile.in 파일로 항상 넘기는 변수들이 있는데, 이런 변수
를 기본 변수라 한다. 기본 변수에는 다음과 같은 것들이 있으며 AC_INIT 매크로에서
정의된 변수들이기 때문에 항상 넘긴다.
［표 13-2］ configure 스크립트에서 M개＜ efile.in으로 항상 넘어오는 기본 변수

변수

설명

bindir

실행 파일을 설치할 디렉토리

sbindir

시스템 관리자가 실행할 용도의 실행 파일을 설치할 디렉토리

datadir

읽기 전용 아키텍처 중립적인 자료를 설치할 디렉토리

includedir

C header file을 설치할 디렉토리

infodir

info 형식의 문서를 설치할 디렉토리

mandir

man 형식의 문서를 설치할 최상위 디렉토리

libdir

object code 라이브러리를 설치할 디렉토리

libexecdir

다른 프로그램에 의해 간접적으로 실행되는 파일을 설치할 디렉토리

srcdir

Makefile에 대한 소스 코드가 있는 디렉토리

top_srcdir

패키지에 대한 최상위 소스 코드 디렉토리

sysconfdir

읽기 전용 단일 머신 자료를 설치할 디렉토리

prefix

아키텍처 의존적이지 않은 파일에 대한 설치 접두어

exec_prefilx

아키텍처 의존적인 파일에 대한 설치 접두어

CFL人GS

C 컴파일러에 대한 디버깅, 최적화 옵션

CPPFLAGS

C 전처리기와 컴파일러에 대한 옵션

CXXFL7XGS

C-H- 컴파일러에 대한 디버깅, 최적화 옵션

FFUXGS

포트란 77 컴파일러에 대한 디버깅, 최적화 옵션

DEFS

C 컴파일러에게 전달할 D 옵션

LDFUXGS

링커에 대한옵션

LIBS

링커에 전달할 라이브러리 옵션

［표 13-2］ 에서 굵은 글씨로 되어 있는 것들이 automake 변수의 접두어로 사용될 수
있는 것들이다. 잘 보면 모두 dir로 끝남을 알 수 있다.

automake의 접두어는 이렇게 dir로 끝나는 변수에서 dir을 뺀 나머지 부분이 될 수 있
다. 가령 libdir 같은 경우 dir을 뺀 lib가 접두어로 사용된다.
이런 접두어는 Makefile.am 파일 내에서 지정한 변수를 사용해도 된다.

640

5부_ 프로젝트 빌드

===== PAGE 642 =====
〔예제 13-3]

Makefile, am 파일 내용

i •••상략

：

： mydir=/usr/local/my

; my_PROGRAMS = test
：

••.하략

l 예제 13-3] 은 Makefile.am 파일 내에 변수 mydir 을 지정하고 값으로 /usr/local/my
를 정의하였다. 이렇게 직접 변수를 지정할 때 주의해야 될 점은 변수명과 = 기호와 변
수 값을 띄우지 말고 붙여 써야 한다는 점이다.

my_PROGRAMS = test에 의해 make install 명 령을 수행하면 test 프로그램이 컴파일
된 후 mydir 변수 값인 /usr/local/my 디 렉토리에 설치된다.
주요 변수명은 이미 존재하는 파일이나 생성될 파일의 종류를 나타내고 파일을 빌드할
규칙을 automake에게 알리는 역할을 한다. 예를 들면 주요 변수명 PROGRAMS는 컴파
일되고 링크될 파일을 의미하고, LIBRARIES는 라이브러리로 빌드될 파일을 의미한다. 이
런 주요 변수명과 주요 변수명의 접두어가 될 수 있는 것에는 다음과 같은 것들이 있다.

O SUBDIRS
재귀적 make 사용 시 Makefile.am 파일이 있는 하위 디렉토리를 지정한다. SUBDIRS
가 지정되면 configure.ac 파일에 AC_PROG_MAKE_SET 매크로를 지정해야 한다.
예) SUBDIRS = po lib src tests

@ PROGRAMS
컴파일되고 링크될 파일 리스트로 다음과 같은 것들이 있다.

• bin： bindir 변수의 디렉토리에 설치 예) bin_PROGRAMS = heUo
• sbin： sbindir 변수의 디 렉토리에 설치 예) sbin_PROGRAMS = hello
• libexec： libexecdir 변수의 디렉토리에 설치
•

pkglib： $ (prefix) /lib/$ (PACKAGE) 디 렉토리 에 설치

• noinst： 설치되지는 않음
• check： make check 명령이 내려지기 전까지는 만들어지지 않아야 된다는 의미
• EXTRA : 컴파일될 수도 있고 안 될 수도 있음
예) EXTRA_PROGRAMS = hello 1 hello2

13장_ automake 641

===== PAGE 643 =====
@SOURCES
어떤 소스의 파일들이 어떤 파일로 빌드되는지를 알린다.
• 접두어: 빌드될 파일의 이름이 온다. 예를 들면 다음과 같다
예) bin_PROGRAMS = hello

hello_SOURCES = hello.c hello.h
• EXTRA： 빌드될 때 필요할 수도 있고 필요하지 않을 수도 있는 파일들
예) EXTRA_hello_SOURCES = version.h

Q LIBRARIES
빌드될 라이브러리의 리스트로 다음과 같다.

• lib： libdir 변수의 디 렉토리에 설치 예) lib_LIBWIES = libtest.a
• pkglib： $(prefix)/lib/$(PACKAGE)의 디렉토리에 설치
• noinst： 설치되지는 않음
• check： make check 명령이 내려지기 전까지는 만들어지지 말아야 된다는 의미
• EXTRA： 컴파일될 수도 있고 안 될 수도 있음
예) EXTRA_PROGRAMS = hello 1

hello2

同 LTLIBRARIES

동적 라이브러리 리스트로 다음과 같다.

• lib： libdir 변수의 디렉토리에 설치 예) lib_ LTLIBRARIES = libtestja
• EXTRA： build될 때 필요할 수도 있고 필요하지 않을 수도 있는 파일들
0 HEADERS
헤더 파일 리스트로 다음과 같다.

• include： includerdir 변수의 디렉토리에 설치
예) include_HEADERS = hello ,h

• oldinclude： oldincluderdir 변수의 디렉토리에 설치
• pkginclude： $ (prefix) /include/$ (PACKAGE) 변수의 디렉토리에 설치
• noinst： 설치되지는 않음

642

5부_ 프로젝트빌드

===== PAGE 644 =====
a SCRIPTS
스크립트 파일의 리스트로 다음과 같다.

• bin： bindir 변수의 디렉토리에 설치 예) bin_SCRIPTS = hello.sh
• sbin： sbindir 변수의 디렉토리에 설치 예) sbin_SCRIPTS = hello.sh
• libexec： libexecdir 변수의 디렉토리에 설치
• pkgdata： $ (prefix)/data/$ (PACKAGE) 의 디렉토리에 설치
• noinst： 설치되지는 않음
• EXTRA： build될 때 필요할 수도 있고 필요하지 않을 수도 있는 파일들
@ DATA
데이터 파일로 다음과 같다.

• data： datadir 변수의 디렉토리에 설치 예) doc_DATA = hello.txt
• sysconf： sysconfdir 변수의 디렉토리에 설치
• sharedstate： sharedstatedir 변수의 디렉토리에 설치
• localstate： localstatedir 변수의 디렉토리에 설치
• pkgdata： $ (prefix) /data/$ (PACKAGE) 변수의 디 렉토리 에 설치
• noinst： 설치되지는 않음
흐］ 니SP： Emacs Lisp

E TEXINFOS
Texinfo 파일 리스트로 다음과 같다.
• info： infodir 변수의 디 렉토리에 설치
ID MANS
man 파일 리스트로 다음과 같다.
• man： mandir 디렉토리에 설치
Makefile.am 파일에서 위에 정의한 주요 변수명과 접두어를 사용해 빌드될 규칙을 적으
면 automake 명령에 의해 Makefile.in 파일이 생성된다. 이렇게 생성된 Makefile.in 파일
에는 기본적으로 all, tags, check, install, uninstall 등의 타겟이 생성되는데, tags는 tags
파일을 생성하는 타겟이며, check는 컴파일될 수 있는지 없는지 체크하는 타겟이다.

13장_ automake 64： ；

===== PAGE 645 =====
이렇게 기본적으로 생성되는 타겟에 자신이 정의한 타겟을 같이 수행하고 싶다면

Makefile.am 파일에 일반적인 Makefile 작성하듯이 타겟을 정의하면 된다.
직접 정의한 타겟은 Makefile.in 파일의 끝 부분에 바로 복사된다. 타겟의 정의뿐만 아니
라 Makefile.am 파일에 어떤 내용을 추가하면 automake가 인식하는 변수가 아닌 이상
바로 Makefilejn으로 복사된다. 직접 작성한 타겟과 automake가 생성하는 타겟의 이름
이 중복되면 automake가 생성한 타겟을 먼저 수행한 후 직접 적은 타겟이 수행된다.

Makefile.am 파일에 타겟을 직접 작성하거나 매크로를 정의할 때 주의해야 될 점은
GNU make만이 사용하는 make 함수나 ifdef ~ endif와 같은 조건부 수행을 사용해서
는 안 된다. automake가 지향하는 것은 여 러 컴퓨터에서 빌드될 수 있는 기술 파일을
만드는 것인데, GNU make만이 지원하는 기능을 사용하면 GNU make가 있는 컴퓨터
로 이식성이 제한되어 버리기 때문이다.
그럼 지금까지의 내용을 토대로 재귀적 make를 수행하는 Makefile.am 파일을 작성해
보자.

표 재귀적 Makefile.am 파일 작성
automake 를 사용해 재귀적 make 를 구현하기 위해 먼저 include, memo, main,
calendar 디렉토리를 생성하고 각 디렉토리에 다음과 같은 소스 파일을 작성한다.
〔예제 13-4〕 재귀적 make를 구현을 위한 예제 소스

include/diary.h :
#include <stdio.h>
int memo();
int calendar();

memo/memo. c :
#include "diary.h"
int memo() {
printf("function
return 0;

memo.\n");

}
main/main.c :
#include "diary.h"
int main() {
memo () ;
calendar();
return 0;

calendar/calendar.c
#include "diary.h”
int calendar() {
. printf("function
return 0;

}

}

644 5부_ 프로젝트빌드

calendar.\n");

===== PAGE 646 =====
소스 파일들을 작성했으면 최상위 소스 디렉토리에 다음과 같은 configure.ac 파일을
작성한다.
〔예제 13-5)

configure.ac 파일 내용

AC_INIT(diary, 0.0.1, woos@mymail.com)
AM_INIT_AUTOMAKE(diary, 0.0.1)
AC_PROG_CC
AC_PROG_MAKE_SET
AC_PROG_RANLIB
AC_CONFIG_FILES ([Makefile
calendar/Makefile
db/Makefile
memo/Makefile] )
AC__OUTPUT

configure.ac 파일에 보면 ACJNIT 매크로 다음에 AM_INIT_AUTOMAKE 매크로를
사용해 autoconf에게 automake를 사용함을 알렸다. 그리고 AC_PROG_MAKE_SET
매크로를 추가하였는데, AC_PROG_MAKE_SET 매크로는 재귀적 make를 사용하기 위
해 반드시 추가해야 되는 매크로다. AC_PROG_RANLIB 매크로는 라이브러리를 만들
기 위해 사용하는 매크로인데, 내친김에 라이브러리도 만들어 보자.

configure.ac 파일을 작성했으면 프로젝트가 있는 최상위 디렉토리에 다음과 같은
Makefile.am 파일을 작성한다.
〔예제 13-6)

CFLAGS

최상위 디렉토리 Makefile.am

= @CFLAGS@ -I../include -I./include

SUBDIRS
= main memo calendar
bin_PROGRAMS
=' diary
diary_SOURCES = diary.h main/main.c memo/memo.c calendar/calendar.c
lib_LIBRARIES
= libmydiary.a
libmydiary_a_SOURCES = diary.h memo/memo.c calendar/calendar.c

clean
rm -rf *.o *.a diary
@echo 모든 파일을 지웠습니다.

13 장 _ automake 645

===== PAGE 647 =====
CFLAGS 매크로에서 @CFLAGS@는 config.status 스크립트에 의해 시스템 정보로 변
경될 부분이다. 그래서 CFLAGS는 config.status 스크립트에서 넘어오는 CFLAGS 변
수 값에 -I../include -I./incl니de를 추가한 것이다.

SUBDIRS 매크로에는 Makefile.am 파일이 있는 디렉토리를 지정한다. 그러면
automake가 SUBDIRS 매크로에 등록된 서브디렉토리로 들어가 Makefile.am 파일을
읽 어 Makefile .in 파일을 생성 한다.

bin_PROGRAMS = diary의 의미는 기본 변수 bindir의 값으로 등록된 디렉토리에 설
치할 실행 파일 diary라는 의미다. 통상 bindir 변수에는 기본 값으로 /usr/local/bin이
들어 있기 때문에 diary는 make install 명 령으로 /usr/local/bin 디 렉토리에 설치된
다. sbin_PROGRAMS - diary할 경우 make install 명령을 내리면 sbindir 변수 값인

/usr/local/sbin 디 렉토리에 diary 실행 파일을 설치한다.
bindir 값은 configure 명령 시 ./config니re-------------------------------- 같은 옵션으로 변경
가능하다. 그리고 주요 변수명 PROGRAMS가 의미하는 바는 diary 파일은 컴파일해 생
성하는 파일이라는 의미도 있다.

diary_SOURCES는 diary 실행 파일의 소스를 지정하는 변수다. 즉, diary 실행 파일은
diary.h main/main.c memo/memo.c calendar/calendar.c 파일들'을 이용해 컴파일
하고 링크해 만든다는 의미다.

lib_LIBRARIES = libmydiary.a 변수는 기본 변수 libdir이 지정하는 디렉토리에 설치할
라이브러리 libmydiary.a라는 의미다.

libdir은 기본으로 /usr/local/lib의 값을 가지고 있기 때문에 make install 명령으로
libmydiary.a 라이브러리는 /usr/local/lib 디렉토리에 설치된다. 역시 libdir 변수도
./configure --libdir=/usr/lib와 같은 옵션으로 변경 가능하다.
주요 변수명 LIBRARIES는 컴파일해 아카이브 파일로 묶어 라이브러리로 만든다는 의
미다. automake를 사용하면 이 렇게 손쉽게 라이브러 리를 만들 수 있다.

libmydiary_a_SOURCES 변수는 libmydiary.a 라이브러리에 필요한 소스 파일을 지
정하는 변수다. 여기서 주의 깊게 보아야 할 것은 libmydiary.a_SOURCES가 아니
라 libmydiary_a_SOURCES라는 점이다. 이렇게 autoconf 매크로나 automake의
변수에는 점(.)을 사용하지 않고 언더 바(_)를 사용하는 경우가 많으니 주의하기 바
란다. 그리고 clean 타겟을 넣어주었다. 이렇게 clean 타겟을 직접 넣어주면 생성될

646 W_ 프로젝트 빌드

===== PAGE 648 =====
Makefile.in 파일에 그대로 복사되기 때문에 바로 사용 가능하다. 물론 automake가 생
성하는 clean 타겟도 Makefile .in 파일에 생성된다. 이렇게 이중으로 타겟이 정의되면

make clean 명령을 내릴 경우 먼저 automake가 정의한 clean 타겟이 수행되고 그 다
음에 직접 작성한 dean 타겟이 수행된다.
최상위 디렉토리의 Makefile.am 파일을 작성하였다면 이제는 각 서브디렉토리의

Makefile .am 파일을 작성 할 차례 다.
원칙대로라면 각 서브디렉토리는 각각의 실행 파일 또는 라이브러리들을 빌드하기 위
한 Makefile.am 파일이 있어야 된다. 그렇지만 지금 사용하는 소스 파일은 각 서브디렉
토리가 단지 소스 파일을 나누기 위해 있으므로 그럴 필요가 없다. 그래서 각 서브디렉
토리 (main, memo, calendar)의 Makefile.am 파일을 다음과 같이 작성하면 된다.
〔예제 13-7)

clean :
rm -i?f * . o
@echo ’pwd’ 디렉토리의 파일을 지웠습니다.

이제 모든 준비가 끝났다. 각 디 렉토리 와 디 렉토리 에 있는 파일들을 tree 명 령으로 보았
을 때 다음과 같이 되어 있으면 모든 준비가 끝난 것이다.

[그림 13-7] 디렉토리 tree 구조

최상위 디렉토리에는 Makefile.am, config니re.ac 파일과 calendar, include, main,

memo 디렉토리가 있다. 그리고 각 서브디렉토리에는 소스 파일과 MakefUe.am 파일
이 있으면 된다.

13장_ automake | 647

===== PAGE 649 =====
먼저 aclocal 명령을 내려 a니tomake가 참조하는 aclocal.m4 파일을 생성한다. 그리고

autoconf 명령을 내려 configure 스크립트를 생성한다.

［그림 13—8］ a이ocal 명령과 autoconf 명령 수행

마지막으로 automake-------------------- -- add-missing --copy 명령을 내리면 Makefile,

in 파일과 각 서브디렉토리에 Makefile.in 파일이 생성된다. automake --foreign
--add-missing ——copy 명령은 automake----------------- -a -c 명령으^로. 줄일 수 있다.
H root@server：/temp/hanbit

(거

[root
seruer hanbitjtt_autoconf
[root@seruer hanbit]#
configure.ac: installing ./install-sh'
configure .ac: installing ' ./inkinstalldirs1
configure.ac: installing './missing*
Makefile.am: installing './depcomp*
[root
seruer hanbit]tt 1

프흐흐흐三후延흐호三"’’리

(흐

[그림 13-9] automake 명령 수행

자, 이제 ./configure 명령을 내리면 시스템 정보를 수집해 최상위 디렉토리에 있는

Makefllejn 파일과 각 서브디렉토리의 Makefile .in 파일에 시스템에서 수집한 정보를
더해 Makefile로 만든다.
H root@server：/temp/hanbit
checking whether build environment is sane... yes
checking for gawk... gauk
checking whether make sets $(MAKE)_______________ yes
checking For gee_________ gee
checking for C compiler deFault output___________________ a.out
checking whether the C compiler works_________________ yes
checking whether we are cross compiling__________________ no
checking For suFFix oF executables________________
checking For sufFix of object files___________________ o
checking whether we are using the GNU C compiler... yes
checking whether gee accepts -g— yes
checking For gcc option to accept ANSI C___________________ none needed
checking For style of include used by make____________________ GNU
checking dependency style oF gcc_______________ gcc3
chpcking whether make sets $(MfiKE)... (cachpd) yps
checking For ranlib___________ ranlib
configure: creating ./conFig.status
conFig
.status: creating Makefile
conFig.status:
creating
calendar/MakeFile
conFig.status:
creating
main/Makefile
conFig.status:
creating meno/Makefile
conFig.status: executing depfiles commands
[root@seruer hanbit]tt j

［그림 13너이 ./confgure 명령 수행

648

&부— 프로젝트 빌드

===== PAGE 650 =====
이제 멋지게, 그리고 기운차게 make 명령을 타이핑해 입력하면 화면에 수많은 문자를
뿌리면서 diary 실행 파일과 libmydiary.a 라이브러 리를 빌드한다.
『~厂

'1 root@server：/temp/hanbit
source=,main/nain.c, object='main.0' libtool=no tt
depfile='.deps/iwin.Po' tnpdepFile=1.deps/main.TPo' tt
depfiode=gcc3 /bin/sh ./depcomp tf
gcc -DPfiCKAGE_NAME=tt"diarytt" -DPACKfiGE_TARNfiME=tt"diarytt” -DPA
CKfiGE_UERSION=W',0.0.W,, -DPACKAGE_STRING=W"diarytf 0.0.키#" -DP
fiCKAGE_BUGREPORT=W''woos@mymail.coiiiw'' -DPfiCKAGE=tf"diaryW" -DUE
RSI0N=@"0.8.1W" -I. -I. -g -02 -I../include -I./include
-c -o main.0 'test —F 'main/main.c' || echo '''nain/main.c
gcc -g —02 -I../include -I./include -o diar브- main.o memo.
o calendar .0
nake[1]: 나감 '/temp/hanbit' 디 렉토리
[root@seruer hanbit]tt Is diary libmydiary.a
diary libmydiarp.a
[root@server hanbit]tt |

[그림 13-11] m가＜ e 명령 수행

make install 명령을 내리면 Makefile.am 파일을 작성하면서 지정한 각 디렉토리로
diary 파일과 libmydiary.a 파일이 설치된다.
'히 root@server：/temp/hanbit
nake[2]: 나감 '/tenp/hanbit/calendar' L| -1 f
make[1]: 나감 '/temp/hanbit/calendar'〔디 렉토리
make[1]: 들어감 '/tenp/hanbit' 디 렉토리
make[2]: 들어감 "/tenp/hanbit' cj 렉토리
/bin/sh ./mkinstalldirs /usr/local/bin
/usr/bin/install -c diary /usr/local/bin/diary
/bin/sh ./mkinstalldirs /usr/local/lib
/usr/bin/install -c -m 644 libmydiary.a /usr/local/lib/libmy
diary .a
ranlib /usr/local/lib/libnydiary.a

―.——■——

make[2]: 나감 '/temp/hanbit' 디렉토리
make[1]: 니■감 '/temp/hanbit1 [j 렉토리
[root@seruer hanbit]tt |

[그림 13너2] make install 명령 수행

이상이 automake와 autoconf를 이용해 프로젝트를 이식성있게 빌드하는 방법이
다. 역시 automake에 대해서는 아직 설명할 게 많이 남아 있지만 나머지는 독자의 몫
으로 남긴다. 물고기 잡는 법을 알려주었으니 충분히 스스로 알아갈 수 있을 거라 본
다. 좀 더 쉽게 빨리 익히기를 바란다면 GNU 프로젝트 파일의 configure,ac 파일과

Makefile.am 파일을 보고 어떻게 되어 있는지 확인하면서 하나씩 익혀나가면 많은 도
움이 될 것이다.

13장_ automake

===== PAGE 651 =====
| 6부 | 프로젝트 버전 관리

===== PAGE 652 =====
Subversion,
CVS

이 버전관리의이해

02 S니bversion을 이용한 버전 관리
03 Subversion 서버 설정
04 Subversion-g- 사용해 프로젝트 진행
05 CVS를 이용한버전 관리
06 CVS 서버 설정
07 CVS> 사용해 프로젝트 진행

===== PAGE 653 =====
Let's S+udy K-------------------

------------

이번 과정에서는 Subversion(서브버전) 또는 CVS를 사용한 프로젝트 형상 관리

(Software Configuration Management) 기법을 알아본다. 형상 관리는 공동 개발 프
로젝트에서 매우 중요한 개념이다. 때문에 “형상 관리”라는 말을 지금 처음들은 독자가
있다면 처음 듣는다고 무시하지 말고 이번 장을 좀 더 자세히 읽어보기 바란다. 형상 관
리는 프로젝트를 성공시키기 위해 반드시 필요하다.

===== PAGE 654 =====
血배전과라의0］ 해
먼저 형상 관리가 무엇인지에 대해 알아보자. 형상 관리란 소스 코드 버전 관리에서부
터 소스 코드 변경 관리, 그리고 빌드와 릴리즈 관리를 포함하는 프로젝트 전반의 관리
방법을 체계적으로 정의하는 관리 방법 이다. 형상 관리를 잘하면 다수가 함께 참여하는
프로젝트에서 많은 문제를 줄일 수 있다. 그리고 프로젝트를 주먹구구식 이 아닌 좀 더
체계적으로 수행할 수 있다.
형상 관리는 원래 소프트웨어 공학에서 나온 말이다. 소프트웨어 공학에서 소프트웨어
소스 버전 관리를 좀 더 포괄적으로 확장시켜 만든 개념이 형상 관리다. 때문에 형상
관리하면 제일 처음 떠오르는 것은 버전 관리다.
이번 장에서는 버 전 관리 툴인 Subversion과 CVS을 알아본다.

I 버전 관리 정의
버전 관리란 프로젝트에서 생성되는 각종 소스, 문서, 실행 바이너리 등과 같은 파일들
을 생성부터 소멸까지 체계적인 버전으로 관리한다는 의미다. 여기서 말하는 버전이란
흔히 말하는 소프트웨어의 버전과는 약간 차이가 있다.
여기서 말하는 버전이란 Subversion, CVS 같은 버전 관리 툴이 관리하는 버전으로, 파
일의 생성, 수정, 소멸에 따라 변화하는 버전이다. 예를 들면 main.c라는 파일이 있을
경우 main.c가 생성될 때 최초 버전이 할당되고, 이후 main.c가 수정되면서 main.c의
버전이 버전 관리 툴에 의해 저절로 변화한다.
main.c (V1)

main.c (V2)

main.c (V3)

lain.c (V4)

| int main() {
printf(“aa”)；
printf(“bb”)；
sleep(1)；

int main() {
sleep(1)；
printf(“cc")；
return 0；

return 0；

}

}

길동

삿갓

우동

삿갓

［그림 14-1］ 버전 관리 예

14장—Subversion, CVS 653

===== PAGE 655 =====
이렇게 변화하는 버전이 버전 관리 툴에서 관리하는 버전이고, 버전 관리 툴을 사용해
언제든지 이전 버전의 파일을 받아볼 수 있고, 변경 내역을 추적/확인할 수도 있다.

I 프로젝트 파일 버전 관리의 필요성
프로젝트 파일들을 버 전 관리하면 다음과 같은 장점 이 있다.

1. 잘못 수정한 내용을 이전 버전으로 되돌릴 수 있다.
2. 개발자 개개인이 따로 백업하지 않아도 된다.
3. 변경 내역을 추적/확인하는 것이 가능해 파일의 변화를 쉽게 파악할 수 있다.
4. 공동 개발 시 발생하는 파일 동기화 문제와 덮어쓰기 문제를 쉽게 해결할 수 있다.
5. 릴리즈 파일 관리 및 릴리즈 파일의 패치 관리가 뒤섞이지 않고 체계적이게 된다.
개발하다 보면 이전 버전으로 되돌아가야 될 때가 많이 있다. 보통 버전 관리 시스템을
사용하지 않는 개발자들은 이전 버전으로 돌아가야 될 경우를 대비해 현재 작업본의
복사본을 만들어 놓고 작업하다가 이전 버전으로 되돌아가야 한다면 복사본을 작업본
으로 바꾸곤 한다. 하지만 버전 관리 툴을 사용하면 이런 번거로운 과정을 거치지 않아
도 된다. 모든 파일들의 변화는 버전으로 관리되므로 필요하다면 언제든 이전 버전으로
돌아갈 수 있고, 이전 버전과의 변화를 비교할 수도 있다.
그래서 개발자 개개인이 롤백이나 만일의 사태에 대비해 따로 백업하지 않아도 된다.
개발자는 그냥 마음 편히 변화된 내용을 버전 관리 툴에 맞기기만 하면 된다. 그러면
버전 관리 툴이 알아서 그런 문제들이 발생했을 때 해결할 수 있게끔 해준다.
버전 관리 툴을 사용하면 파일의 변경 내역을 추적/확인하는 것도 가능하다. 때문에 문
제가 생겼다면 해당 문제를 언제 누가 만들었는지 확인할 수 있다. 이 런 기능은 단독
개발에도 자신의 기억을 살리는 데 유용하지만 공동 개발에서 커뮤니케이션 오버헤드
를 줄이는 데 더 유용하다. 공동으로 프로젝트를 개발하다 보면 누가 어떤 함수를 왜
추가했고, 어 떤 파일을 왜 만들었는지 확인해야 될 필요가 많이 발생한다. 버전 관리 시
스템이 없다면 해당 담당자에게 물어봐야 하지만 있다면 해당 파일의 로그를 확인하는
것만으로도 충분하다.

654

6부_ 프로젝트 버전 관리

===== PAGE 656 =====
길동 루-1
파일 생성

- main.c

삿갓 루—1
- bb 출력문 추가

우동 로그
삿갓 로그
- 출력 홬인율 위해 - aa 출력문 제거
잠깐 대기 기능 추가
— cc 추력문 추가
main.c (V3)

main.c (V4)

[그림 14—2] 파일 버전별 로그 추가 예

버전 관리는 이렇게 단독 프로젝트보다 공동 프로젝트에서 더욱 빛을 발한다. 프로젝트
를 공동으로 진행하면 여러 가지 문제가 많이 발생하는데, 대표적인 문제가 덮어쓰기와
동기화 문제다.
덮어쓰기는 하나의 파일에 여러 사람이 작업을 할 경우 이전 사람의 작업 내용이 이후
사람의 작업 내용 반영으로 인해 덮어써지는 문제를 말한다.

[그림 14-3] 덮어쓰기 문제 예

예를 들면 main.c라는 하나의 파일을 공유 디렉토리에 넣고 김삿갓과 장우동이 같은
시점에 main.c 파일을 동시에 수정한다고 가정하자. 먼저 김삿갓이 main.c에 내용을
추가하고 저장했다. 이후 장우동이 main.c에 새로운 내용을 추가하고 저장했다면 김삿
갓의 작업 내용은 장우동의 작업 내용이 덮어써버려 사라지고 만다.
덮어쓰기 문제는 프로젝트의 성격상 모듈화가 힘들어 하나의 소스를 공유해 개발할 때
발생한다. 열심히 작업한 후 파일을 다시 열었을 때 자신이 작업한 내용이 사라진 것만
큼 허탈한 일도 없을 것이다.

14장_ Subversion, CVS 655

===== PAGE 657 =====
동기화 문제는 다음과 같은 문제다. main.c 파일로 두 사람이 main.c의 서로 다른 부분
을 동시에 작업 했다면 결국 두 내용은 하나의 main.c 파일에 합쳐져야 한다. 버전 관리
툴을 사용하지 않는다면 누군가 한 사람이 일일이 소스를 비교하면서 하나로 합칠 수
밖에 없다. 하지만 버전 관리 툴을 사용하면 버 전 관리 툴이 알아서 두 내용을 하나로
합쳐준다.
이렇게 버전 관리 툴을 사용하면 사람이 직접 해야 되는 수고를 덜고 프로젝트 파일들
을 체계적으로 관리할 수 있다. 때문에 버전 관리 툴이 필요하다. 이런 버전 관리 툴의
장점은 단순히 사용해 보는 정도로는 부족하다. 버전 관리 툴의 장점을 제대로 파악하
려면 버전 관리 툴을 사용해 프로젝트를 체계적으로 진행해 보아야만 한다. 그렇지 않
다면 남들이 하니깐 따라하는 정도밖에 되지 못한다. 그래서 아직도 버전 관리 툴을 사
용하지 않고 매일 날짜별로 *.tar.gz로 묶어 백업하는 회사가 있는 것이다.
필자는 이번 과정을 통해 독자가 버전 관리 툴을 이해할 수 있기를 바란다. 그러려면
책에 있는 명령 몇 번 쳐보는 것만으로는 절대 부족하다. 버전 관리 툴을 이해하려면
실제 프로젝트로 직접 체험해 봐야 한다. 때문에 필자는 단순히 이해하는 것으로 끝내
지 말고 간단한 프로젝트에라도 꼭 도-입해 사용해 보라고 권하고 싶다. 그것만이 버전
관리 툴을 제대로 이해할 수 있는 길이다.

Subversion을 이용한 버전 관리
버전 관리 툴에는 오픈 소스부터 상용까지 여러 가지 종류가 있다. 이번 장에서는 그 중

Subversion과 CVS를 알아본다. 모두 버 전 관리 툴이다. 우리는 특수한 상황이 아닌 한
이 중에서 하나만 프로젝트에 도입하면 된다. 그러면 가장 좋은 것 하나만 설명하지 왜
두 가지를 다 설명하는지 의문이 들겠지만 두 가지 모두 여러 곳에서 많이 사용되기 때
문이다.
자신의 프로젝트만 생각한다면 자신에 게 맞는 한 가지 버전 관리 툴만 사용해도 된다.
하지만 리눅스/유닉스 프로그래밍 분야의 전문가가 되기 위해서는 적어도 이 두 가지
버 전 관리 툴의 기본 사용법은 알고 있어 야 한다. 앞으로 개발에 필요할지 모르는 많은
라이브러 리와 툴들이 이 두 가지 버 전 관리 툴에 의해 관리되기 때문이다. 따라서 적어
도 기본은 알고 있어야 필요한 라이브러리와 툴들의 소스를 다운 받을 수 있다.

656 6부- 프로젝트버전 관리

===== PAGE 658 =====
이번 절에서는 먼저 Subversion에 의한 버전 관리 기법을 알아본다. Subversion은 현
재 오픈 소스 진영에서 가장 많이 사용되는 버전 관리 툴이다. 때문에 Subversion의 사
용법에 대해서는 자세히 알아 두는 것이 좋다.

I Subversion 소개
Subversion은 2000년도에 CVS를 대체할 목적..0-루 개발되었다. Subversion 이전에는
CVS가 버전 관리 툴로 많이 사용되 었다. CVS는 티라노사우루스 렉스가 돌아다니던 백
악기 시대의 버전 관리 툴로, 오픈 소스를 활성화시키는 데 많은 기여를 한 툴이다

CVS가 처음 나온 1980년대 후반만 하더라도 CVS는 훌륭한 버전 관리 툴이었다. 하지
만 CVS는 시대와 환경의 변화에 제대로 적응하지 못했고, 시간이 지날수록 버전 관리
툴의 한계를 드러냈다. 결국 2000년대 초 CollabNet 사에서 새로운 버전 관리 툴을 개
발하기 위한 개발자를 모집하였고, 그때 개발된 툴이 바로 Subversion이다.

CVS도 중요하기 때문에 CVS에서 Subversion으로 넘어오면서 달라진 점들을 나열해
보면 다음과 같다.
먼저 원자적 커밋을 지원한다. 커밋은 나중에 자세히 설명하겠지만 쉽게 설명하면 변경
된 프로젝트 파일들을 버전 관리 툴에게 넘기는 작업이다. 이렇게 변경된 파일을 버전
관리 툴에 넘기면 해당 파일의 버전 또는 프로젝트 파일 저장소 버전이 바뀐다.
원자적 커밋이란 변경된 파일 묶음 단위로 버전 관리 툴에 반영한다는 의미다. CVS는
파일 단위로 변경된 내용을 반영했기 때문에 동시에 여러 사람이 개발 시 소스 코드가
꼬이는 문제가 발생했었다.
다음으로 디렉토리도 버전 관리 대상에 포함되었다. CVS는 파일만 버전 관리 대상이었
다. 때문에 디렉토리의 생성/삭제가 어려웠고, 파일의 생성/삭제, 파일명 수정, 파일 복
사와 같은 디렉토리 변경을 추적하지도 못했다. 이 문제는 대단히 심각해서 CVS를 사
용해 프로젝트를 진행하기 힘들게 만드는 첫 번째 요인이었다.
마지막으로 CVS는 바이너리 파일과 텍스트 파일을 비교할 때 서로 다른 알고리즘을
사용해서 파일을 등록할 때 바이너리 파일인지 텍스트 파일인지 알려줄 필요가' 있었다.

CVS가 자동으로 어느 정도 구분해 주긴 했지만 제대로 구분해 줬는지 일일이 확인해
야 되었으므로 이 또한 상당히 번거로운 일이었다.

14장_ Subversion, CVS 657

===== PAGE 659 =====
이것 외에도 http 프로토콜 지원, 빠른 브랜치와 태깅 같은 기능적 변화가 제법 있었지
만 앞에서 설명한 내용들이 CVS에서 Subversion으로 오면서 바뀐 가장 주요 변화였다.
때문에 Subversion은 나오자마자 선풍적인 인기를 끌면서 빠르게 CVS를 대체했다.

Subversion 은 CVS 를 대체하기 위해 개발되었기 때문에 기능적으로 CVS 의 거의 모
든 기능을 포함한다. 명령 또한 CVS 명령을 그대로 따왔기 때문에 CVS 사용자는 쉽게

Subversion을 사용할 수 있고, Subversion 사용자는 쉽 게 CVS를 사용할 수 있다.

［그림 14-4］ Subversion을 사용한 개발 구조

Subversion을 이용해 프로젝트를 진행하는 구조는 매우 단순하다. ［그림 14-4］ 와 같
이 중앙에 Subversion 서버가 있고 Subversion 서버에 버전 관리할 프로젝트 파일을
넣어 둔다. 개발자들은 Subversion 서버에 접속해 프로젝트 파일을 자신의 PC로 가져
온다.
개발자는 가져온 프로젝트 파일에 새로운 내용을 추가하고 추가한 내용을 Subversion
서버에 있는 프로젝트 파일에 반영한다. 이후 다른 개발자가 Subversion 서버에서 프
로젝트 파일을 받으면 새롭게 변경된 프로젝트 파일을 받아볼 수 있다.
공동 개발로 인해 발생할 수 있는 덮어쓰기 문제나 동기화 문제는 모두 Subversion이
알아서 처리한다. 개발자는 자신의 디렉토리에 있는 소스로 마치 혼자서 작업하듯이 프
로젝트를 진행하면 된다. 물론 개발자는 완전히 혼자서 하는 작업이 아니기 때문에 중
간 중간에 서버에 있는 최신 프로젝트 파일과 자신의 작업 디렉토리에 있는 프로젝트
파일을 동기화시켜야 한다. 이것이 Subversion을 사용한 프로젝트의 기본 개념이다.
그러면 지금부터 실제로 Subversion을 사용해 프로젝트를 진행해 보자.

658 6부_ 프로젝트버전 관리

===== PAGE 660 =====
3 Subversion 서버 설정
Subversion을 프로젝트에 도입하려면 먼저 Subversion 서버를 설정해야 한다.
Subversion 서버를 설정하려면 root 권한이 필요하다.
Subversion 서버 설정을 위해서는 시스템에 S니bversion이 설치되어 있어야 한다. svn
--version 명령으로 Subversion이 설치되어 있는지 확인할 수 있다. 설치되어 있지
않다면 다음 명령으로 설치하기 바란다.
$ yum install subversion
$ sudo apt-get insta丄1 subversion # 으■분투 사용자

# 페도라사-용자'

I 저장소 생성 및 초기화
S니bversion을 설치했으면 앞으로 프로젝트 파일들을 저장해 둘 디렉토리를 하나 생성
하자. 필자는 /home/svnroot를 사용하고자 한다. /home/svnroot에 앞으로 사용할
저장소들을 만들 것이다.
$ mkdir /home/svnroot
/ root@server：~

_____

[root@seruer ~]tt|mkdir /home/sunroot|
[root@seruer |

［그림 14-5］ 저장소 디렉토리 생성

디렉토리를 생성했으면 이제 저장소를 만들자. 저장소는 프로젝트 파일들이 들어갈 장
소를 의미한다. 보통의 경우 하나의 프로젝트는 하나의 저장소를 가지고, 해당 저장소
에 각종 프로젝트 파일이 들어가 버전 관리된다.
저장소는 svnadmin 명령으로 생성한다. /home/svnroot 디렉토리에서 다음 명령을
내리면 myproject라는 저장소가 생성된다.
$ svnadmin create --f s-type f sf s ［생성할저장소패스］
예:

$ svnadmin create --fs-type fsfs /hom은/svnroot/myproj®c:t

14장_ Subversion, CVS 659

===== PAGE 661 =====
産 root@server：/home/svnroot

하'

[root@seru
' svm'oot ]tt|'&；；；；'；aininrc?em --Fs-type fsFs /honie/sunroot/wyproject
[root@server sunroot]
[rootSserver sunroot]ttfiT'^home/svnr-oiot/'Ryproject |
README.txt conf db format hooks locks
[root
seruer sunroot]# |

허

（흐

[그림 14-6] myproject 저장소 디렉토리 생성

필자는 /home/svmoot/myproject 를 저장소 디렉토리로 설정했다. 저장소 디렉토리
명은 프로젝트 성격에 맞게 각자 알아서 결정하면 된다. 옵션으로 준 --fs-type fsfs는
저장소 타입을 파일 타입으로 만들라고 지정한 것이다. 파일 타입 외에 BSD DB 타입
의 저장소가 있을 수 있다. BSD DB는 오류가 발생 했을 때 복구하는 데 문제가 많기 때
문에 보통은 파일 타입으로 저장소를 만든다.

I 저장소 접근 방식 종류 이해
저장소를 생성했으면 이제 개발자들이 저장소에 접근할 수 있도록 저장소 권한을 설정
해야 한다. 개발자들이 저장소에 접근할 수 있는 방식에는 크게 4가지 방식이 있는데,
각각은 다음과 같다.

O 서버에서 직접 작업하는 경우
Subversion 서버에 시스템 계정이 있어야 하고 시스템 계정으로 로그인해서 작업하는
경우에 사용하는 방식이다. 저장소는 로컬 머신의 파일 시스템에 있다. 때문에 다음과
같은 URL로 접근한다.
$ svn [svn 명령] file:///home/svnroot/mypr°jec七

이 방식은 중요하게 다뤄야 할 Subversion 서버에 보안상 문제가 많이 있고 안정성 면
에서도 문제점을 내포하고 있다. 때문에 개인적으로 자신의 파일들을 관리하는 데는 사
용하지만 공동 프로젝트에서는 잘 사용하지 않는 방식이다.

@ ssh를 이용해 원격으로 작업하는 경우
Subversion 서버에 시스템 계정이 있을 때 사용하는 방식이다. ssh 프로토콜을 사용해
서버에 있는 프로젝트 파일을 자신의 PC로 가져와 작업하고 다음과 같은 형식의 URL
로 접근한다.

660 6부_ 프로젝트버전 관리

===== PAGE 662 =====
$ svn [svn 명령] svn+ssh://[ID] @ [주소] /110111은/3’7111‘00七/1117P亡0드은0七

보안성이 좋고 별도의 서버 설정이 필요 없어 많이 사용되는 방식 중 하나다.

@ http를 이용해 원격으로 작업하는 경우
Subversion 서버에 Subversion 계정이 있어야 한다. Subversion 계정은 일반적인
시스템 계정과 다르게 Subversion에서만 사용하는 계정이다. 설정에 따라 http 또는

https 프로토콜을 사용해 서버에 있는 프로젝트 파일을 자신의 PC로 가져와 작업하고
다음과 같은 형식의 URL로 접근한다.
$

svn

［ svn

명령］

svn+http://［주소］/svn/myproject

또는

$ svn ［ svn 명령］ svn+https://［주소］/svn/mypr°ject

속도가 비교적 빠르고 접근성이 높아 가장 많이 사용하는 방식 중 하나다.

B svnserve를 이용해 원격으로 작업하는 경우
Subversion 패키지에 포함된 svnserve라는 서버 프로그램을 사용해 접근하는 방식이
다. Subversion 서버에 Subversion 계정이 있어야 하고 SVN 프로토콜을 사용해 서버
에 있는 프로젝트 파일을 자신의 PC로 가져 와 작업한다.
무거운 웹서버를 띄우지 않아도 되므로 비교적 가볍고 다음과 같은 형식의 URL로 접근
할수있다.
$ svn ［ svn 명령］ svn: // ［ ^41］ /myproject

위 4 가지 방식 중 가장 많이 사용되는 방식은 http 방식과 ssh 방식이다. 어떤 방식이
든 보통은 자신의 프로젝트 성격에 맞게 한두 가지 방식만 사용한다. 때문에 모든 방
식을 다 설정할 필요는 없다. 그렇지만 우리는 Subversion을 배우고 있는 중이니 ssh,

http, svnserve 방식의 서버를 모두 설정해 보자.

I ssh를 이용한 서버 설정
먼저 ssh를 사용한 방식으로 설정해 보자. ssh를 사용한 방식으로 설정하려면 해당 저
장소에 접근할 그룹을 시스템에 하나 생성해야 한다. 다음 명령을 사용하면 새로운 그
룹을 생성할 수 있다.

14장_ Subversion, CVS

661

===== PAGE 663 =====
$ groupadd [그룹명]

# ［그룹명 ］ 그룹생성

예:

$ groupadd svn

［그림 14-7］ 시스템 계정 생성

필자는 ［그림 14-刀과 같이 svn 그룹을 하나 생성했다. 이후 생성할 개발자 계정들은
모두 svn 그룹에 포함될 것이고, 저장소는 svn 그룹이 읽고 쓸 수 있게끔 접근 권한을
설정할 것이다.

svn 그룹을 생성하였으면 다음 명령으로 개발자 계정을 생성한다. 우분투 사용자는
useradd 명령 대신 adduser 명령을 동일한 옵션으로 사용하기 바란다.
$ useradd ［개발자계정명 ］ -g ［개발자 그룹명 ］
$ passwd ［개발자계정명］
예:

$ useradd satgat -g svn
$ passwd satgat
$ useradd udong -g svn
$ passwd udong

# satgat 계정을 svn 그룹으로 생성
# satgat 계정 암호 등록
# udong 계정을 svn 그룹으로 생성
# udong 계정 암호 등록

/ root(®server：/home/svnroot
[root@server sunroot]It useradd satgat -g sun
[root
server sunroot]# passwd satgat
Changing password for user satgat.
New UNIX password:
Retype new UNIX password:
passwd: all authentication tokens updated successfully.
[rootSseruer sunroot]#
[ root@seruer sunroot ] tt pjseradrarijdo^^
[root@seruer sunroot]# passwd udong
Changing password for udong. ~
New UNIX password:
Retype new UNIX password:
passwd: all authentication tokens updated successfully.
[root@seruer sunroot]# |

(흐

―"워

［그림 14-8］ 시스템 계정 생성

필자는 김삿갓〔satgat) 계정과 장우동(udong) 계정을 생성하였다. 그리고 -g svn 옵션
을 사용해 계정 생성 시 satgat 계정과 udong 계정의 그룹을 svn으로 설정하였다. 이렇
게 -g 옵션을 사용해 해당 계정의 그룹을 svn 그룹에 등록해도 되고, 일단 계정을 생성
한 후 다음 그림과 같이 /etc/group 파일에서 svn 그룹에 해당 계정을 등록시켜도 된다.

662 6부_ 프로젝트 버전 관리

===== PAGE 664 =====
［그림 14-9］ /etc/group 파일을 수정해 그룹을 등록한 모습

그룹 등록이 끝났으면 svn 그룹이 저장소를 읽고, 쓸 수 있도록 저장소 권한을 설정한다.
$ chown root. svn [저장소 패스] -R
$ chmod g+w [ 저장소패스] -R
예:

$ chown root.svn /home/svnroot/myproject -R
$ chmod g+w /home/svnroot/myproject -R

醫' root@server：/home/svnroot
[ r o o t Q s e r u e r sunroot]# chown root .sun /home/sunroot/myproject -R
[root
seruersunroot]# chmod g+w /home/sunroot/myproject -R
[ r o o t @ s e r u e r sunrootjtt
sunroot]tt |
[root@seruer

（흐

［그림 14너0］ myproject 저장소 접근 권한 설정

이제 ssh 방식으로 저장소에 접근하기 위한 모든 설정이 끝났다. 제대로 설정되었는지
다음 명령으로 확인해 보자.
$ svn info svn+ssh://satgat@localhost ［저장소 패스］
예:

$ svn info svn+ssh://satgat@localhost/home/svnroot/myproject

=1QJ 스!
[[root
seruer sunroot]tt[sun info 'svn*ssh://satgat@localhost/home/sunroot/iiijjpt'oject|
satgat@localhost’s password:
경호: myproject
URL: sun+ssh://satgat
localhost/home/sunroot/m.yproject
저장소 루트: sun+ssh://satgat@iocalhost/home/svnroot/iiiyproject
저장소 UUID: C877893F-357F-4373-aa14-94951Fb5H
65
root@server：/home/svnroot

（ 흐

（흐

느

리비전: 0
노드 종류: 디렉토리
마지막 수정 리비전: 0
마지막 수정 일자: 2009-09-21 05:26:18 +0900 （ 20B9-09-21, 월）
[rooteseruer sunroot]# |

［그림 14네］ 저장소 접근 확인 모습

14장_ Subversion, CVS 663

===== PAGE 665 =====
그림과 같이 저장소 정보가 출력된다면 정상적으로 설정된 것이다.

I http를 이용한 서버 설정
다음으로 http를 이용한 방식의 저장소 설정을 해 보자. 먼저 아파치 웹서버와 웹서버

svn 모듈을 설치해야 한다. 다음 명 령으로 설치할 수 있다.
$ yum install httpd mod_dav_svn
$ sudo apt-get install apache2 libapache2-svn # 우분투사용자

# 페도라시^g•자‘

설치가 되었으면 웹서버가 저장소 디렉토리를 읽고 쓸 수 있게 권한 설정을 해 줘야 한
다. 다음과 같은 명령을 사용하면 권한 설정이 가능하다.
# 페도라사용자

$ chown apache /home/svnroot/myproject -R
$ chmod u+w /home/svnroot/myproject -R
# 우분투사용자

$ sudo chown www-data /home/svnroot/myproject -R
$ sudo chmod u+w /home/svnroot/myproject -R
if root@sierver：/home/svnroot
[root@seruer sunroot]# chown apache /home/sunroot/myproject -R
[root@seruer sunroot]# chmod u+w /home/sunroot/nyproject -R
[rootSseruer sunroot]# |

[그림 14-12] myproject 저장소 접근 권한 설정

페도라 사용자와 우분투 사용자의 저장소 사용자명 이 다른 것은 각 배포판에 따라 웹
서버 프로세스의 사용자가 다르기 때문이다. 중요한 것은 웹서버 프로세스의 사용자가
무엇이냐에 따라 저장소 사용자가 설정되어야 한다는 점이다. 그래야 웹서버가 저장소
에 읽고 쓸 수 있다. 웹서버 프로세스 사용자는 웹서버를 동작시킨 후 ps -aux 명령으
로 확인하거나 웹서버 설정 파일의 User 필드 부분에서 확인 가능하다.
저장소 권한을 설정했으면 이제 웹서버 설정 파일에 Subversion 저장소 관련 설정을
해야 한다. 페도라 배포판이라면 /etc/httpd/conf.d/subversion.conf 파일을 열어 다
음 내용을 추가한다. /etc/httpd/conf.d/subversion.conf 파일이 없으면 그냥 /etc/

httpd/conf/httpd.conf 파일에 추가■한다.

664 6부_ 프로젝트버전 관리

===== PAGE 666 =====
우분투

/etc/apache2/mods-enabled/dav_svn.conf

사용자는

apache2/mods-enabled/dav_svn.load에

설정하거나

해당

파일과

파일들이

없으면

/etc/
/etc/

apache2/apache2.conf 파일에 설정한다.
〔예제 14-1)

웹서버 설정 파일에 svn 설정 추가

# svn 모듈 로드 설정. 우분투 사용자는 dav_svn. load 파일에
# 모듈 로드 부분이 이미 설정되어 있는지 먼저 확인해 보기 바란다.

LoadModule dav_svn_module
LoadModule authz_svn_module

modules/mod_dav_svn.so
modules/mod_authz_svn.so

# location /svn의 설정. 이후 http:// [서버 IP]/svn/[저장소명] URL로
# 접속하면 /home/svnroot/[ 저장소명 ] 으로 접속하게 됨
<Location /svn>
DAV svn
# 저장소의 부모 패스 설정. 저장소가 모인 위치이고

# http:// [서버 IP]/svn으로 접속 시 위치할장소임
SVNParentPath /home/svnroot
AuthType Basic
# 프로젝트명을설정

AuthName "MyProject"
# /svn에 해당하는 Subversion 계정 파일 위치
# 임의의 장소에 생성하고 설정하면 됨

AuthUserFile /etc/svn-passwd
Require valid-user
</Location>

위 내용을 웹서버 설정 파일에 추가했으면 나머지 설정은 일반적인 웹서버 설정하듯이
하면 된다. 일반적인 웹서버 설정을 모른다면 그냥 두어도 무방하다.
여기까지

했으면

이제

/etc/svn-passwd를

만들어야

한다.

/etc/svn-passwd는

Subversion 사용자 계정들이 정의되어 있는 파일이다. 이전에도 설명했듯이 Subversion
사용자 계정은 시스템 계정과는 다르게 Subversion에서만 사용하는 계정이다.

Subversion 계정 파일을 만들려면 우선 /etc/svn-passwd라는 빈 파일을 하나 만들
고 다음 명령을 사용해 하나씩 내용을 추가한다.

14장_ Subversion. CVS 665

===== PAGE 667 =====
[Subversion 사용자 계정 ID]

$ htpasswd —nd
예:

$ htpasswd
$ htpasswd

-nd satg.at
-nd udong

[그림 14-13] 암호화된 암호 생성

htpasswd -nd satgat 명령 또는 htpasswd -nd udong 명령을 내리면 암호를 입력하
라는 메시지가 나오는데, 그때 앞으로 해당 正가 사용할 암호를 입력하면 된다. 그러면

satgat：,zG0qCf6u 1 ATM 또는 udong：0UiaK9zAM6ORL와 같이 “[Subversion ID]：[암호
화된 암히” 형식으로 출력되는데, 이 내용으로 /etc/svn-passwd 파일을 채우면 된다.

發- root@server：/home/svnroot

키 x|

_Jt

satgat:.zG0qCF6u1fiTM
dong:0UiaK9zAM60RI

파

••/etc/svn-passwd" 2L, 41c

모두

o

[그림 14너4] /etc/svn-passwd 파일 내용

이후 새로운 Subversion 계정을 등록하고자 할 때도 /etc/svn-passwd 파일에

htpasswd -nd [ID] 명령을 사용해 등록하면 된다.
Subversion 사용자 계정 등록을 완료했으면 다음 명령으로 웹서버를 재시작하기 바란다.
$ service httpd restart
$ sudo /etc/init.d/apache2 restart

[그림 14-15] 웹서버 재시작

666 &부— 프로젝트 버전 관리

# 페도라사용자
# 우분투사용자

===== PAGE 668 =====
웹서버가 정상적으로 동작한다면 http 방식으로 Subversion을 사용하기 위한 모든 설
정이 끝났다. 다음 명령을 수행해 http 방식으로 프로젝트 저장소에 제대로 접근하는지
확인한다.
$ svn info http://localhost/svn/myproject
if root@server：/home/svnroot
[rootBseruer svnroot']'히 s<m~://localhostjsun/띄yproject
인증 영역 (realm): <http://localhost: 8 0> My Project
'satgat•의 암호:
겅로: my|가-oject
URL: http://localhost/sun/myproject

저장소 루트: http://localhost/sun/myproject
저장소 UUID： c877893F-357f-4373-aa14-94951Fb5ff65
리비전: 0
노드 종류: 디렉토리
마지막 수정 리비전: 0
마지막 수정 일자: 2009-09-21 05:26:18 +0900 (2009-09-21, 월)
[rootSserver sunroot]# |

[그림 14-16] http 방식으로 svn 동작 확인

ID와 암호를 입력했을 때 위 그림과 같이 정상적으로 저장소 정보가 출력되면 설정이
완료된 것이다. 외부에서 접속이 잘 안 된다면 방화벽 설정과 SELinux 설정을 확인해
보기 바란다. 간혹 상위 버전 svn을 사용한다면 svn info 명령 시 다음과 같은 오류 메
시지가 출력될 수 있다.

[그림 14너7] svn info 시 오류 메시지

그럴 경우에는 ~/.s 니 bversion/servers 파일을 열어 다음 그림과 같이 [global] 필드에
있는 store-plaintext-passwords = no 필드를 주석 해제한다.

14장_ Subversion, CVS 667

===== PAGE 669 =====
改 root@serwr：/home/svnroot

-!□! x|

tttttt SSL certificate. See details aboue For ouerriding security |
ttlttt due to SSL.
[global]
tt http-proxy-exceptions = *.exception.con, www.internal-site.org
tt http-proxy-host = deFaultprox
whatever.com
# http-proxy-port = 7008
# http-proxy-username = defaultusernane
ft http-proxy-password = deFaultpassword
# http-compression = no
# No http-tineout, so just use the builtin default.
# No neon-debug-nask, so neon debugging is disabled.
# ssl-authority-files = /path/to/CAcert.pen;/path/to/Cftcert2.pem
tt
tt Password / passphrase caching parameters:
g store-passwords = no
tore—plaintext—passwords = no|
tt store-ssl-client-cert-pp = no
# store-ssl-client-cert-pp-plaintext = no

으.

덥

153,1

바닥 Pl

[그림 14-18] 〜/.subversion/serwrs 파일 수정 내용

이제 http를 사용한 Subversion 서버 설정이 모두 끝났다. 페도라 사용자라면 https
프로토콜도 별도의 설정 없이 바로 사용 가능할 수 있으니 svn info https：//localhost/

svn/myproject 명 령으로도 한번 테스트해 보기 바란다.

I svnserve를 이용한 서버 설정
마지막으로 svnserve를 사용한 서버 설정을 해 보자. svnserve를 이용한 방식은 웹서
버를 돌리기 어려운 경우에 사용될 수 있다. 리눅스 개발 환경에서 웹서버를 돌리기 어
려운 상황은 많이 없으므로 svnserve보다는 http를 사용한 서버 설정 방식이 훨씬 많
이 사용된다. 하지만 간혹 svnserve도 사용되므로 설정법을 알아보자.

svnserve을 사용한 서버를 설정하려면 먼저 다음과 같은 /etc/xinetd.d/svn 파일을
생성한다.

J /etc/xinetd.d/svn 파일 내용

|〔예제 14-2〕

service

svn

{
disable
port
socket_type
protocol
wait
user
server
server args
}

668

6부—프로젝트버전 관리

= no
= 3690
= stream
= tcp
= no
= root
= /usr/bin/svnserve
= -i -r /home/svnroot

===== PAGE 670 =====
우분투 사용자 중 /etc/xinetd.d 디렉토리가 없는 사람은 xinetd 데몬이 설치되지 않은
경우이니

sudo

atp-get install xinetd 명령으로 설치한 후 /etc/xinetd.d/svn 파일을

생성하기 바란다.
파일을 생성했으면 다음 명 령으로 xinetd 데몬을 재실행한다.
$ service xinetd restart
$ sudo /etc/init. d/xinetd start

# 페도라 人누용자
# 우^'투■人b용■자‘

［그림 14-19］ xinetd 데몬 재시작

제대로 svnserve가 동작하는지 확인하려면 다음과 같은 명령을 내린다.
$ svn info svn://localhost/myproject
우 root@server：~
[rootBseruer ~]tt[svn info svn ://localhost/iiHJproject |
경로: myproject
URL: sun://localhost/myproject
저장소 루트: sun://localhost/myproject
저장소 UUID： c877893F-357f-4373-aa14-94951Fb5Ff65

리비전: 0
노드 종류: 디렉토리
마지막 수정 리비전: 0
마지막 수정 일자: 2009-09-21 05:26:18 +0900 (2009-09-21, 월)
[root@seruer ~]# |

［그림 14-20］ svnserve 동작 확인

제대로 설정되었다면 위 그림과 같이 정상적으로 저장소 정보를 받아와 출력할 것이다.
그런데 아직 끝난 것이 아니다. 위 명령을 내렸을 때 ID와 암호로 인증 과정 없이 바로
저장소 정보를 받아왔다. 그것은 모든 사용자가 저장소에 접근할 수 있다는 의 미 다. 때
문에 보안을 위 해 인증 과정 에 관련된 설정을 추가해야 한다.
인증 과정을 추가하려면 ［저장소 디렉토리 패스］/conf/svnserve.conf 파일에 다음과
같은 내용을 추가한다. 필자는 /home/svnroot/myproject/conf/svnserve.conf 파일
에 다음과 같은 내용을 추가하였다.

14장_ Subversion, CVS 669

===== PAGE 671 =====
〔예제 14-3]

/home/svnroot/myproject/conf/svnserve.conf 파일 내용

[general]
anon-access = none
auth-access = write
password-db = passwd

# 등록안 된사용자는접근 권한 없음
# 등록된 사용자는 쓰기 권한 있음
# 암호 파일은 passwd

그리고 /home/svnroot/myproject/conf/passwd 파일을 열어 다음과 같이 사용자들
을 등록한다.
〔예제 14-4〕 /home/svnroot/myproject/conf/passwd 파일 내용

[users]
satgat = 1234
udong = abcdef

위 예제는 satgat 사용자와 udong 사용자를 등록한 예다. 각 라인은 [ID] = [암히와
같은 형식으로 되어 있고, 암호는 암호화되지 않고 그냥 일반 문자열로 되어 있다. 그래
서 satgat 사용자의 암호는 1234가 되고 udong 사용자의 암호는 abcdef가 된다.
자, 여기까지 했으면 다시 svn info 명령을 내려 보자. 그러면 다음 그림과 같이 인증
과정을 수행함을 확인할 수 있다.

[그림 14-21] 인증 과정 수행 모습

이제 모든 서버 설정이 끝났다. 그럼 본격적으로 Subversion을 사용해 프로젝트를 진
행해 보자.

670 6부_ 프로젝트 버전 관리

===== PAGE 672 =====
Subversion/을 사용해 프로젝트 진행
Subversion을 사용해 프로젝트를 진행하는 일은 매우 단순하다. 우선 제일 처음 누군
가가 프로젝트 디렉토리를 정리해 import 명령으로 Subversion 서버에 프로젝트 파일
을 등록한다. 그런 후 checkout 명령을 통해 등록한 파일을 내 PC로 받아온다. 이후 내

PC에서 작업한 내용을 commit 명령으로 서버에 반영한다. 마지막으로 중간 중간 다른
사람이 작업한 내용을 update 명령으로 내 PC에 반영하면서 프로젝트를 진행한다.
이것이 기본이다. 이 정도만 알면 Subversion을 사용해 프로젝트를 진행하는 일이 가
능하다. 그럼 각각의 과정과 명령들을 알아보자.

I 에디트 환경 변수 설정
Subversion을 사용하려면 먼저 SVN_EDITOR 환경 변수를 설정해야 한다. SVN_
EDITOR는 Subversion의 로그를 작성할 때 사용할 에디터 명령이 정의되어야 하는
환경 변수다.
환경 변수 설정은 ~/.bash_profile 파일에 다음과 같은 라인을 한 줄 추가하면 된다.
• • • 중략

export SVN_EDITOR=vim
... 하략

그리고 다음 명 령을 내린다.
$ source ~/.bash_profile

source 명령은 최초 한 번만 내리면 된다. 이후부터는 셸이 시작될 때 저절로 SVN_
EDITOR 환경 변수가 설정된다.

| 프로젝트 디렉토리 정리
먼저 프로젝트 디렉토리를 정리해야 한다. 각 팀의 개발 프로세스 혹은 개발 방식에 맞
게 프로젝트 디렉토리를 정리하면 된다. 어떤 방식으로 정리하는지에 대한 정답은 없
다. 필자의 회사에서는 다음과 같은 구조로 하나의 프로젝트 디렉토리를 구성한다.

14장_ Subversion, CVS

671

===== PAGE 673 =====
〔예제 14-5］

프로젝트 디렉토리 구조 예

-- 01_General
I01_Proposal
I-- 02_Project_Management
I—- 03_Status_Report
'—- 04_Weekly_Report
- - 02_Requirement
- - 03_Feasibility_Study
—
— 04_System_Analysis
—
- 05_High_Level_Design
—
— 06_Detailed_Design
- - 07_Implementation
- - 08_Test
- - 09_Completion
- - 10_Transfer
55_Source
I-- branches
I —- tags
'—- trunk
- - 99_Reference

# 일반적인것들
# 과제 제안서
# 프로젝트 관리 관련 툴 파일 또는 계획서
# 월간 또는 분기 보고서
# 팀원들의주간보고서
# 요구 사항 분석서 및 분석 자료

# research 문서또는 지•료
# 시스템 분석서 및 분석 자료
# 상위 디자인 문서
# 상세 디자인 문서
# 실제 구현내용 문서
# 테스팅 계획서 및 테스팅 보고서
# 완료보고서
# 인수인계 보고서 및 관련 내용
# 실제구현소스
# 소스브랜치
# 소스태그
# 소스메인트리
# 각종참조

필자의 회사는 Subversion 으로 프로젝트 문서와 소스를 통합 관리한다. 그리고 개발
프로세스가 있어 개발을 진행하는 순서와 절차가 있다. 물론 아직 개발 프로세스가 완
전히 정립되지 않았지만 언젠가는 기필코 반드시 정립시키고자 한다. 어떻든 그렇기 때
문에 필자 회사의 프로젝트 디렉토리 구조는 ［예제 14-5］ 와 같이 구성된 것이다.
소스만 Subversion으로 관리하는 팀이라면 위 구조와 같이 할 필요는 없다. 소스만 관
리하는 팀이라면 다음과 같이 3개의 디렉토리만 생성하면 된다.
I-- branches
I-- tags
'-- trunk

# 소스브랜치
# 소스태그
# 소스메인트리

위 구조는 Subversion에서 추천하는 구조다. 먼저 trunk 디 렉토리에 소스가 들어간다.

trunk 는 줄기라는 뜻으로, 소스의 메인 트리다. branches는 가지라는 뜻으로 trunk의
브랜치들이 들어가는 곳이다. 브랜치는 메인 트리(trunk)의 소스들을 테스트하거나 새
로운 기능을 추가해 테스트하고자 할 때 메인 트리를 건드리지 않기 위해 만든 소스의
가지다.

672 6부_ 프로젝트버전 관리

===== PAGE 674 =====
위 그림에서 동그란 것은 Subversion에서 관리하는 파일 또는 디렉토리의 버전이라고
보면 된다. 맨 위에 일렬로 버전이 진행해 나가는 것이 trunk다. 브랜치는 그림과 같이

trunk에서 파일 버전의 가지를 친 것이다. 때문에 브랜치에는 가지를 친 trunk의 파일
또는 디렉토리들이 모두 들어있다. branches 디렉토리는 이런 브랜치 파일 또는 디렉
토리가 위치하는 곳이다.

tags에는 태깅한 프로젝트 파일들이 들어간다. 태깅은 특정한 시점에서의 프로젝트 파
일들의 스냅샵이라고 보면 된다. 태깅은 특정 버전을 릴리즈하거나 특정 시점의 파일들
을 저장해야 될 필요가 있을 때 한다. 태그 디렉토리에 이런 특정 시점의 프로젝트 파
일들이 들어간다. 그렇지만 이것은 Subversion에서 태깅을 하는 방식이고, 다른 버전
관리 툴들은 다른 방식으로 태깅을 한다. 하지만 다른 버전 관리 툴 역시 태깅의 의미는

Subversion과 같다.
각 디렉토리의 의미를 알았으면 본격적으로 프로젝트 디렉토리를 한번 만들어보자. 다
음 명령을 순차적으로 내리면 project라는 프로젝트 디렉토리가 만들어진다.
$ mkdir project
$ mkdir project/trunk
$ mkdir project/branches
$ mkdir project/tags

[그림 14-23] 프로젝트 디렉토리 생성

14장_ Subversion, CVS

673

===== PAGE 675 =====
프로젝트 디 렉토리를 생성 했으면 이제 프로젝트 파일들을 생성하거나 복사해야 한다.
당장 생성할 파일과 복사할 파일이 없다면 그냥 이대로 저장소에 등록(import)해도 된
다. 필자는 12 장에서 make 를 설명할 때 사용한 예제 소스를 trunk 에 넣도록 하겠다.

12장의 ［그림 12-44］ 에서 설명한 소스 트리 구조가 그것이다. 예제 소스가 없는 사람
은 실습을 위해 그냥 아무 소스 또는 디 렉토리를 넣기 바란다.
root@server：/work/book/utils_new/svn
[rootSseruer 5un]tt tree
'— project
|-- branches
|tags
'-- trunk
|-- ConFig.mk
|—- Makefile
|-- Rules.mk
|-- calendar
|
|—— Makefile
|
'-- calendar .c
j-- include
|
diary.h
|-- main
|
|— Makefile
|
'-- main.c
'-•- memo
|-- Makefile
'-- memo.c
8 directories, 18 files
[root@seruer sun]tt |

［그림 14-24］ 프로젝트 파일 구조

최종적으로 만들어진 프로젝트 디렉토리 구조는 위 그림과 같다. 프로젝트 디렉토리
에 최초 파일들을 넣었으면 쓸데없는 컴파일 중간 파일(예: *.O ) 같은 것들은 들어있
지 않은지 확인한다. 프로젝트 디 렉토리를 깔끔하게 정리했으면 이제 해당 디렉토리를

Subversion 서버에 등록(import)한다.

I import 명령으로 프로젝트 서버에 등록
생성한 project 디렉토리가 있는 위치에서 다음 명령을 내리면 project 디렉토리의 내
용이 Subversion 서버에 있는 myproject 저장소에 등록된다.
$ svn import project http://localhost/svn/myproject

674 6부—프로젝트버전 관리

===== PAGE 676 =====
[그림 14-25] svn import 명령으로 프로젝트 파일 저장소 등록

위 명령에서 import는 svn의 서브 명령이고 project는 등록할 파일 디렉토리 패스

http：//localhost/svn/myproject 저장소의 URL이다. 저장소 URL은 각각의 방식에 따
라 다음과 같이 다르게 적어주면 된다.
-

로컬

file: ///home/svnroot/mypro ject
- ssh
svn+ssh://satgat@localhost/home/svnroot/inyproject
- http 또는 https
http://localhost/svn/myprojecthttps://localhost/svn/myproject
— svnserve
svn://localhost/myproject

현재는 저장소가 로컬 머신에 있어 주소를 localhost를 사용했는데, 원격지에 저장소
서버가 있다면 해당 서버의 IP 또는 도메인을 주소로 사용하면 된다.

svn import 명령을 내리면 다음 그림과 같이 SVN_EDITOR 환경 변수로 등록한 vim
이 실행된다. 그러면 vim을 이용해 로그를 남기 면 된다.

[그림 14-26] 로그 작성

14장_ Subversion, CVS 675

===== PAGE 677 =====
필자는 “프로젝트 시작”이라는 로그를 남겼다. 저장하고 종료하면 Subversion ID와 암
호를 물어보고, 인증 과정을 성공하면 다음 그림과 같이 project 디렉토리에 있는 내용
들이 저장소에 등록된다.
旗 root@seryer：/work/book/utils_new/svn
[rootBseruer sun]tt Is
project
[root@seruer sun]# sun import project http://localhost/sun/myproj
ect

인증 엉 역 (realm): <http://localhost :8B> My Project
•耳atgat •으j 암호:
추가
project/trunk
추가
project/trunk/Rules.mk
추가
project/trunk/include
추가
pro ject/trunk/include/diary .h
추가
project/trunk/nain
추가
project/trunk/nain/main .c
추가
project/trunk/main/Makefile
추가
project/trunk/calendar
추가
pro ject/trunk/calendar/calendar .c
추가
project/trunk/calendar/Makefile
추가
project/trunk/ConFig.nk
추가
project/trunk/MakeFile
추가
project/trunk/memo
추가
project/trunk/meno/MakeFile
추가
project/trunk/meno/meno .c
추가
project/branches
추가
project/tags
커밋된 리비전 1[root@seruer sun]tt |

[그림 14-27] 저장소에 프로젝트 파일 등록

3

이렇게 하면 저장소에 프로젝트 파일이 등록 완료된다.

| checkout 명령으로 프로젝트 파일 가져오기
import 명령으로 프로젝트 파일들을 저장소에 등록했으면 이제는 각 개발자가 저장소
에 등록된 파일들을 자신의 PC로 가져와 작업해야 한다. 저장소에 있는 파일들을 자신
의 PC로 가져오는 명령은 checkout 명령이다.
앞으로 작업에 사용할 작업 디렉토리에서 다음 명령을 내리면 저장소에 있는 프로젝트
파일들을 자신의 PC로 받아온다.
$ svn checkout http://localhost/svn/myproject
또는

$ svn co http://localhost/svn/myproject

676 6부_ 프로젝트버전 관리

===== PAGE 678 =====
/ root@server：/work/book/utils_new/svn
[root@server sun]tt|ls]
[root@seruer sun]母
[ root@seruer sun ] #| 하『 checkout l"i；ttp://loca：Lhost/sun/mj)iproject |
인증 영역 (realm): <http://localhost: 8 0> MyProject
-satgat'으j 암호:
A
myproject/trunk
A
myproject/trunk/Rules. 까《
A
myproject/trunk/include
A
myproject/trunk/include/diary.h
A
myproject/trunk/main
fi
nyproject/trunk/main/nain.c
A
inyproject/trunk/nain/MakeFile
A
myproject/trunk/calendar
A
niyproject/trunk/calendar/calendar .c
A
myproject/trunk/calendar/MakeFile
A
myproject/trunk/ConFig.ink
A
myproject/trunk/MakeFile
A
myproject/trunk/nemo
A
rnyproject/trunk/memo/Makefile
A
rnyproject/trunk/memo/memo.c
ft
myproject/branches
fi
muproject/tags

체크아훗된‘aui천
7丁!
[rootBseruer sun]It Is .

；1ype°je<표"I
[rootSseruer sun]# |

[그림 14-28] 저장소에서 프로젝트 파일 받아오기

맨 마지막에 나오는 메시지인 “체크아웃된 리비전 1.”의 의미는 현재 프로젝트 파일이
버전 1이라는 의미다. 리비전(revision)은 프로젝트를 진행하면서 저장소에 새로운 내
용을 반영할 때마다 증가하는 버전이다.
프로젝트 파일들의 사이즈가 커서 특정 폐스에 있는 파일들만 가져오고자 한다면 해당
패스를 다음과 같이 적어준다.
$ svn checkout http://localhost/svn/myproject/trunk/main

위 명령은 프로젝트 저장소 전체를 받아온 것이 아니라 저장소 내에 trunk 디렉토리 내
의 main 디 렉토리만 받아오는 명령이다.
프로젝트 파일을 저장소에서 받아왔으면 이제 개발을 진행한다.

| commit 명령으로 변경된 내용 저장소에 반영
개발을 진행하면서 myproject/trunk/main/main.c 파일을 다음과 같이 수정했다고
가정하자.

14장_ Subversion. CVS 677

===== PAGE 679 =====
〔예제 14-6〕 수정 전후의 main.c 파일 (좌: 수정 전, 우: 수정 후)

#include "diary.h"
int main() {
memo();
calendar();
return 0;

#include "diary.h”
int main() {
printf("I like you!\n");
memo();
calendar();
return 0;

}

}

［예제 14-6］ 에 보면 main.c 파일에 printf("I like you!\n")； 라인을 다음 그림과 같이
추가했다.

수 root@server：/work/book/utils_new/svn/myproject/tmnk
ftiHclude "diary .h”
int main() {
Eemo();
calendar();
return 8;

"main/main.c" 7L, 77c 저장 했습니다'

3,5

모두

［그림 14-29］ main.c 파일 수정 전

［그림 14-30］ main.c 파일 수정 후

이렇게 파일을 수정했으면 저장소에 반영해 주어야 한다. 그래야만 다른 개발자들도 자
신의 PC 에 수정된 내용을 반영할 수 있다. 변경된 내용을 저장소에 반영하는 명령은

commit 명령이다. 다음과 같이 명령을 내리면 로그를 작성하기 위한 vim이 실행되면
서 로그 작성 후 변경된 내용이 저장소에 반영된다.
$

svn

commit

또는

$ svn ci

678

6부_ 프로젝트 버전 관리

===== PAGE 680 =====
［그림 14—31］ 로그 작성

艾 root@server：/work/book/utiIs_new/svn/myproject/trunk
[rootBserver trunk]tt|sdn conHitiF]

인 층 엉 억(realm)： <http://localhost:80> MyProject
•satgat•의 암호:
전솢중
trunk/nain/ni 그:in.c
파일 데이터 저송종 .

허티된# 5i 전그
[root@seruer trunk]# |

［그림 14-32］ 저장소에 변경된 내용 반영

［그림 14-32］ 를 보면 마지막 메시지로 “커밋된 리비전 2.”라고 출력이 되었다. 이 말은
현재 저장소의 리비전이 2로 바뀌었다는 의미다.

I update 명령으로 저장소의 최신 내용 작업 디렉토리에 반영
다른 사람과 함께 진행하는 프로젝트라면 중간 중간 저장소에서 다른 사람이 작업한
내용을 자신의 작업 사본 디렉토리에 반영해 주어야 한다. 이렇게 저장소의 최신 내용
을 자신의 작업 사본 디렉토리에 반영하는 명령이 update 명령이다. 자신의 작업 사본
디렉토리 내에서 다음 명령을 내리면 저장소의 최신 내용이 작업 사본에 반영된다.
$ svn update
또는

$ svn up

그럼 update 명령을 테스트해 보자. 먼저 update 명령은 저장소의 내용을 자신의 작업
사본에 반영하는 것이니 테스트를 위해 다른 사용자의 작업 내용이 저장소에 반영되어
있어야 할 것이다. 그래서 필자는 udong 사용자로 프로젝트 파일을 먼저 checkout했다.

14장_ Subversion, CVS 679

===== PAGE 681 =====
Z1 root@server：/work/book/utils_new/svn/udong
[root@seruer sun]H is
myproject
____________________________________________________________
[rootSseruer sun]#Inkdir udong
[rootGseruer sun]tt cd udong/
[root@seruer udongsun checkout http://localhost/svn/ii少project
인증 영역 {r$al븨) 드 <http://local.host: 8 0> My Project
그託g託 ■ 희 암호 : |
인증 엉 억 (realm) | <http://localhost :80> My Project

사용자명:ud0n9
'udong1'의 앙호: |
A
A
A
A
A
A
A
fi
A
A
A
A
A
fi
A
A
A

myproject/trunk
myproject/trunk/Rules.nk
nyproject/trunk/include
nyproject/trunk/include/diary.h
nyproject/trunk/main
nyproject/trunk/nain/nain.c
nyproject/trunk/main/Makefile
myproject/trunk/calendar
myproject/trunk/calendar/calendar .c
inyproject/trunk/calendar/Makefile
inyproject/trunk/Config.nk
myproject/trunk/Makefile
myproject/trunk/neno
myproject/trunk/nemo/Makefile
myproject/trunk/memo/meno.c
nyproject/branches
myproject/tags

체크아웃된 리비전 2.
[rooteseruer udong]tt |

[그림 14-33] udong 사용자 체크아웃

그리고 udong 사용자의 작업 사본에서 main.c 파일을 다음과 같이 변경하였다.

[그림 14—34] udong 사용자 main.c 파일 수정

그런 후 다음 명령으로 commit해 니dong 사용자가 수정한 main.c 파일 내용을 저장소
에 반영하였다.
$ svn commit -m Hend 메시지 추가"
Z7 root@server：7work/book/utils_new/svn/udong/myproject/trunk
[root@seruer trunk]tt sun commit -n "end 메시지 추가,,
|인 증 영 역(realm) : <http://localhost:80> MyProject
‘udong•으j 암호:
전송중
trunk/nain/nain.c

파잏 데이 터 저송,중 -

퀴밋된# 5i 전立
[rooteseruer trunk]*! |

[그림 14-35] 니dong 사용자 변경 내용 저장소에 반영

680 6부—프로젝트버전 관리

===== PAGE 682 =====
위 그림에서 svn commit 명령 시 -m "end 메시지 추가" 옵션은 vim을 사용하지 않
고 로그를 간단하게 남길 때 사용한다. svn 명령 시 -m ［로그 메시지］ 옵션을 주면

Subversion은 vim을 띄우지 않고 옵션으로 준 로그 메시지를 로그로 사용한다.
이제 저장소에는 udong 사용자의 main.c 수정 내용이 반영되었다. 그러면 다시 satgat
사용자의 작업 디렉토리로 돌아가 svn update 명령을 내린다. 그러면 다음과 같이 저
장소의 최신 내용이 satgat 사용자의 작업 디 렉토리로 반영된다.

三

司

그'石/s vn/m y p ro j e ct/tru n k

| 노F ro 01@ s
iWE/
o r k/b o o k/util s3
|[root1흐seruer ' trunkjttl's'un up |
이증 영 억 (realm): <http://localhost: 8 0> My Project
|‘udong•의 암호:
|인증 엉 억 (realm): <http ://localhost :80> My Project
사용자멍 :satgat
•satgat•의 암호:
U raain/nain.c

|업데이트 된 리비전 3.
[rootSseruer trunk]#

［그림 14-36］ 저장소의 최신 내용 작업 디렉토리에 반영

update후 main.c 파일을 열어보면 udong 사용자의 작업 내용이 반영된 것을 확인할
수 있다.
업데이트 명령은 특정 버전으로 Update하는 것도 가능하다. 가령 리비전 3인 상황에서

svn update -r 2 명령을 내리면 리비전 스로 파일들을 변경한다.
$ svn update -r 2
$ svn update -r 1 trunk/main/main.c trunk/memo

I log 명령으로 리비전별 로그 확인
저장소에 변경된 로그를 확인하고 싶을 때가 있다. 어떤 사용자가 무슨 일을 했는지 해
당 사용자가 작성한 로그를 log 명 령으로 확인할 수 있다. 로그를 확인할 때는 다음과
같은 명령을 내린다.
$
$
$
$
$
$

svn
svn
svn
svn
svn
svn

log
log
log
log
log
log

# 전체로그확인

trunk/main/main.c
trunk/memo
-r 2
-r 1:3
-r 3:1

# trunk/main/main. c 로그 확인
# trunk/memo 로그 확인
# 리비전2 로그확인
# 리비전 1에서 3까지 로그 확인
# 리비전 3에서 1까지 로그 확인

14장_ Subversion, CVS

681

===== PAGE 683 =====
【그림 14-37] svn log 명령 결과

로그를 확인할 때 -V 옵션을 주면 좀 더 자세한 정보를 출력한다. 반대로 -q 옵션을 주
면 좀 더 간략하게 출력한다.

I diff 명령으로 변경된 내용 비교
리비전별로 어떤 내용이 바뀌었는지 비교하고 싶을 때가 있다. 그럴 때는 diif 명령을
사용한다. diff 명령을 이해하려면 먼저 특수한 리비전인 HEAD 리비전과 BASE 리비
전의 개념을 이해해야 한다.
[표 14-1] HEAD와 BASE 리비전 키워드
리비전 키워드

설명

HEAD

현재 저장소의 최신 리비전

BASE

현재 작업하고 있는 작업 사본을 꺼내온 리비전

HEAD 리비전은 저장소에 있는 최신 리비전을 의미한다. 그래서 현재는 리비전 3이다.
BASE 리비전은 현재 작업 중인 작업 사본을 꺼낸 리비전을 의미한다. 이럴 때 diff 명
령으로 변경된 내용을 비교하는 방법은 다음과 같다.
$
$
$
$

svn diff
svn diff
svn diff
svn diff

682 6부—프로젝트버전 관리

# 현재 작업 중인 모든 파일과 BASE 비교

-r HEAD
-r 2
-r 2:3

# 현재 작업 중인 모든 파일과 HEAD 비교
# 현재 작업 중인 모든 파일과 리비전 2 비교
# 리비전 2와 3의 모든 파일 비교

===== PAGE 684 =====
$
$
$

svn
svn
svn

diff
diff
diff

-r 2 : BASE
-r 2 : HEAD
-r 2 : HEAD main. c

# 리비전 2와 BASE의 모든 파일 비교
# 리비전 2와 HEAD의 모든 파일 비교
# 리비전 2와 HEAD의 main. c 파일 비교

l11
11
[root(흐server trunk]ft|；un 네：丁
1r 에
인증 영역(realm): <http://localhost:80>
MyProject
■satgat ■으j 암호:
Index: main/main.c
==================================================

(리비전 2)
(리비전 3)

—— main/main.c
+++ main/main.c
ee -3,6 +3,8 ee
printf("I like yout^n");
memo();
calendar();
+ printF("end.^n"); // end
+

추가

return 0;
>
[root@seruer trunk]# |

[그림 14-38] svn diff 명령으로 리비전 2와 3를 비교한 모습

하지만 svn diff 명령으로 출력되는 결과는 변경된 부분만 표시되기 때문에 이해하기
힘든 문제가 있다. 다음과 같이 하면 diff 결과를 쉽게 확인할 수 있다.

O vimdiff를 사용해 비교하는 방법
1. 다음명령을수행한다.
echo -e ’#!/bin/sh\n’ > /usr/local/bin/svndiff-vim.sh
echo -e ’vimdiff "$6" ”$7” ’ » /usr/local/bin/svndiff-vim.sh
chmod 755 /usr/local/bin/svndiff-vim.sh

2. 〜/.subversion/config 파일에 [helpers] 필드에 다음 라인을 추가한다.
diff-cmd = svndiff-vim.sh

3. 그리고 svn diff 명령을 내리면 다음과 같이 vimdiff로 바뀐 부분을 보여준다.

[예 1] svn diff 명령 결과

14장_ Subv이'sion, CVS

683

===== PAGE 685 =====
@ meldS 사용해 비교하는 방법
1. yum이나 apt-get으로 m이d 패키지를 설치한다.
yum install meld

2. 다음명령을수행한다.
echo -e ’#!/bin/sh\n’ > /usr/local/bin/svndiff-meld.sh
echo -e ’meld "$6" ’’$7" ' » /usr/local/bin/svndiff-meld.sh
chmod 755 /usr/local/bin/svndiff-meld.sh

3. 〜/.subwrsion/config 파일의 [helpers] 필드에서 diff—cmd를 다음과 같이 변경한다.
diff-cmd = svndiff-meld.sh

4. svn diff 명령을 수행하면 다음과 같이 m이d로 바뀐 부분을 보여준다.

[예 2] svn diff 명령 결과

I blame 명령으로 라인 단위의 작성자 확인
프로젝트를 하다 보면 어떤 파일의 어떤 라인을 누가 추가했는지 확인하고 싶을 때가
있다. 이런 일은 자주 발생한다. 버그가 생겼거나 해당 라인이 이해가 안 될 경우 누가
해당 라인을 작성했는지 알아야 되기 때문이다. 이럴 때 blame 명령을 사용하면 라인
단위로 누가 작성했는지 확인할 수 있다.
$ svn blame main.c
$ svn blame -r 3 main.c

684

6부_ 프로젝트 버전 관리

# main. c 파일 라인 단위 작성자 확인
# 리비전 3의 라인 단위 작성자 확인

===== PAGE 686 =====
[그림 14-39] svn blame 명령으로 라인 단위 작성자를 확인하는 모습

| status 명령으로 작업 디렉토리 상태 확인
현재 작업 디 렉토리 상태를 알고 싶을 때가 있다. 예를 들면 commit을 하기 전에 어떤 파
일들을 변경했는지 확인하고 싶은 경우 말이다. 이럴 때는 svn status 명령을 사용한다.
$ svn status
또는

$ svn stat

改 root@server：/work/book/utils_new/svn/myproject/truoic
言]

|[root@seruer trunk]tt[sun stati
?
main/test.c
|ri
nemo/memo .c
M
Makefile
[root@seruer trunk]# |

[그림 14-40] svn status 명령으로 작업 디렉토리 확인

svn status 명령은 BASE 리비전에서 바뀌지 않은 파일은 표시하지 않는다. 우리는 맨
앞에 붙은

‘M’과 같은 키워드로 각 파일의 상황을 알 수 있는데, 각각이 의미하는

바는 다음과 같다.
• ‘ ’ 수정되지 않음

• ‘A’ 파일 또는 디렉토리가 현재 작업 디렉토리의 버전 관리 대상에 더해짐
• ‘C’ 충돌 났음
• ‘D’ 파일 또는 디렉토리가 현재 작업 디렉토리의 버전 관리 대상에서 제거됨
• ‘I’ 무시됨
• ‘M’ 수정되었음
• ‘?’ 버전 관리 대상이 아님
•‘!’지워짐
14장_ Subversion, CVS 685

===== PAGE 687 =====
위 내용대로 해석해 보면 memo.c 파일과 Makefile 파일이 수정되었고, test.c 파일
이 있지만 버전 관리 대상이 아닌 것을 알 수 있다. 이렇게 svn status 명령을 사용하면

commit 전에 누락된 파일 등을 확인하는 것이 가능하다.

I add 명령으로 파일이나 디렉토리를 버전 관리 대상에 추가
작업 디렉토리에 아무리 새로운 파일이나 디렉토리를 만든다고 해서 버전 관리 대상에
포함되는 것은 아니다. 새로운 파일 또는 디렉토리를 버전 관리 대상에 포함시키려면
다음과 같이 svn add 명령을 사용해야 한다.
$ svn add testl.c test2.c

# testl. c와 test2 . c를 버전 관리 대상에 포함

广 root@server：/work/book/utils_new/svn/myproject/trunk
[rootBseruer trunk]!! [touch testl.c test2.c|
[root@seruer 타*unk]tt
[root@server trunk]tt Is
Config.mk Rules.mk include memo test2.c
Makefile calendar main testl.c
[root@seruer trunk
[rootBseruer trunk]!* svn status
?
testl .c'|
?
test2.c
?
fiain/test .c
M
memo/memo.c
M
Makefile
[root@server trunk]U|sun add testl.c test2.즈"]
fi
testl.c
fi
test2.c
[root@server trunk]tt |

［그림 14-411 svn add 명령을 사용해 버전 관리 대상에 포함

svn add 명령을 사용해 버전 관리 대상에 파일이나 디렉토리를 포함시켰다면 svn
commit을 해야 저장소에 반영된다.

I d이ete 명령으로 파일이나 디렉토리를 버전 관리 대상에서 제거
프로젝트를 하다 보면 어떤 파일이나 디렉토리를 제거하고 싶을 때가 있다. 그럴 때는

svn delete 명령을 사용해 해당 디렉토리나 파일을 버전 관리 대상에서 제거해야 한다.
$ svn delete Config.mk
또는

$ svn del Config.mk

686 6부—프로젝트버전 관리

# Config.mk 파일을 버전 관리 대상에서 제거

===== PAGE 688 =====
푸 root@server：/work/book/utils_new/svn/myproject/truni:
히',

[rootBserver Erunk]
s'un delete ConFig.mk]
D
ConFig.mk
[root@seruer trunk])) sun status
A
testl.c
A
test2.c
?
main/test.c
D
ConFig.mk
M
memo/memo.c
M
Makefile
[rooteseruer trunk]tt |

[그림 14—42] svn delete 명령을 사용해 버전 관리 대상에서 제거

svn delete 명 령 역시 commit을 해야만 저장소에 반영된다.

I rename 명령으로 파일명이나 디렉토리명 변경
rename 명령을 사용하면 파일명이나 디렉토리명을 변경할 수 있다.
$ svn rename Rules .mk aaa.mk # Rules .mk 파일을 aaa.mk로 변경
또는

$ svn ren Rules.mk aaa.mk

[그림 14—43] svn rename 명령으로 파일명 변경

svn rename 명령 역시 commit을 해야 저장소에 반영된다.

I lock/unlock 명령으로 파일 잠금 및 해제
공동으로 프로젝트를 진행하다 보면 어떤 파일들을 자신만 수정하고 싶을 때가 있다.
이 럴 때는 svn lock 명령을 사용한다.
$ svn lock include/diary .h # include/diary .h 파일을 잠금

14장_ Subversion, CVS 687

===== PAGE 689 =====
于 root@server：/work/book/utils_new/svn/myproject/trunk
[root@server trunk]하「5<»|/lock inciude/diary.h |
인증 영 억 （ realm） : <http://localhost: 8 0> My Project
*satgat* 희 암호:
•diary.h‘ （은）는 'satgat•（이）가 잠궜습니다.
[root@seruer trunk]tt
[root@seruer trunk]1t sun status
D
Rules. 까<
A
testl .c
R
,test2.c
K i‘n‘』i；』de7diary.h |
?
nain/test.c
A + aaa.mk
D
Config.mk
H
nemo/meno.c
M
Makefile
[rootSseruer trunk]!! |

［그림 14-44］ svn lock 명령으로 파일을 잠금

svn lock 명령 역시 저장소에 반영하려면 commit을 해야 한다. 어떤 파일에 lock을 하
면 잠근 사람 외에는 수정할 수 없다. lock을 풀려면 svn unlock 명령으로 잠긴 파일을
풀 수 있다.

lock 을 걸면 잠근 사람 외에는 수정할 수 없다고 했다. 그렇다면 어떤 사람이 프로젝
트 파일에 lock을 걸고 아프리카 오지 탐험을 가버렸다면 어떻게 할까? 그럴 때는 svn

unlock 명령 시 一force 옵션을 주면 강제로 lock을 해제할 수 있다.

I revert 명령으로 파일 이전 상태로 되돌리기
파일을 한참 수정했는데 잘못 꼬여 버리거나 하는 경우에는 어떻게 해야 할까? 해당 파
일을 지워버리고 svn update 명령으로 다시 받아오는 방법도 있지만 아름답지 못한
방법이다. 그 방법보다는 revert 명령을 사용하면 파일을 원래대로 되돌릴 수 있다.
$ svn revert Makefile # Makefile을 원래대로 되돌림

［그림 14-45］ 는 수정된 Makefile을 svn revert 명령으로 원래대로 되돌린 모습이다.
처음 svn status 명령을 내렸을 때는 Makefile이 수정되었다는 표시로 ‘M’이 표시되어
있었지만 다음번 svn status 명령 시에는 Makefile이 원래대로 되돌려져 사라진 것을
확인할 수 있다.

svn revert 명령은 수정된 파일뿐만 아니라 ［그림 14-45］ 에서 보이는 testl.c와 같은
버 전 관리 대상에 추가되 었지만 commit되지 않은 파일, 버 전 관리 Rules.mk 같은 버
전 관리 대상에서 제거된 파일 역시 원래대로 되돌릴 수 있다.

688 6부_ 프로젝트버전 관리

===== PAGE 690 =====
[그림 14-45] svn revert 명령으로 파일을 원래대로 되돌림

I export 명령으로 버전 정보 제외한 프로젝트 파일만 가져오기
저장소에서 checkout 으로 프로젝트 파일을 받아오면 디렉토리마다 .svn 디렉토리가
들어간다. .svn 디렉토리는 Subversion이 버전을 관리하기 위한 메타 정보가 들어 있
는 디렉토리로, 프로젝트 파일 트리를 외부에 릴리즈할 때 필요 없는 파일들이다.
이렇게 Subversion의 관리 정보를 제외한 순수한 프로젝트 파일만 가져오려 할 때는

svn export 명령을 사용한다.
# 저장소에 있는 최신 버전 프로젝트 파일들을 release-0.1로 익스포트

$ svn export http://localhost/svn/myproject release-0.1
# 저장소에 히는 리비전 2 프로젝트 파일들을 release-0.1로 익스포트

$ svn export -r 2 http://localhost/svn/myproject release-0.1
# checkout?}-myproject 프로젝트를 release—0.1 로 익스포트
$ svn export myproject release-0.1.

svn export 명령을 사용하지 않고 Subversion 관리 정보를 모두 지우는 방법에는 한
가지가 더 있는데, 다음과 같은 명 령을 수행하면 된다.
$ find myproject -name . svn -exec rm -rf {} \;

.svn 디렉토리만 지워주면 관리 정보가 모두 없어지기 때문에 위 명령으로 .svn 디렉토
리를 찾아 모두 지워주면 된다.

14장_ Subversion, CVS 689

===== PAGE 691 =====
I copy 명령으로 브랜치하기
이전에도 설명했듯이 새로운 기능을 추가하거나 테스트할 때 브랜치를 한다.

이렇게 브랜치한 것은 머지(merge) 과정을 통해 메인 트리와 다시 합칠 수도 있다. 물
론 테스트만 해 보고 필요 없으면 버릴 수도 있다. 그리고 위 그림과 같이 브랜치에서
다시 브랜치할 수도 있다.
브랜치는 작업 디렉토리를 cp 명령으로 로컬에서 단순히 다른 디렉토리로 복사하는 것
과는 다르다. cp 명령으로 작업 디렉토리를 로컬에서 복사하면 버전 관리 정보는 여전
히 메인 트리의 관리 정보를 가진다. 때문에 Subversion 관점에서는 복사본 역시 작업
디렉토리와 똑같다. 그래서 cp 명령으로 단순히 복사한 디렉토리에 내용을 수정하고

commit하면 메인 트리에 반영된다.
반면 브랜치는 svn copy 명령으로 브랜치하고 해당 브랜치를 checkout하면 이후부터
의 작업은 해당 브랜치에만 반영된다. 브랜치는 이래서 단순히 cp 명령으로 복사해서
는 안 되고 svn copy 명 령으로 브랜치해야 된다.
이전에 브랜치는 테스트하거나 새로운 기능을 추가하면서 테스트할 때 많이 사용한다
고 했었다. 그럼 브랜치하지 않고 단순히 복사하고 테스트한 후 복사한 디렉토리를 지
워 버리는 것은 어떨까? 물론 단순한 기능 구현이나 테스트라면 그렇게 해도 된다. 하
지만 기능 구현 및 테스트가 시간이 오래 걸리는 작업이므로 버전 관리가 되어야 한다
면 그때는 브랜치를 사용해야 한다.
브랜치는 다음과 같은 명 령으로 한다.
$ svn copy trunk branches/test-branch
$ svn commit

690 6부—프로젝트버전 관리

===== PAGE 692 =====
위 명령을 내리면 trunk를 복사해 branches/test-branch를 만들고 commit해 저장소
에 해당브랜치를 반영한다.
/ root@server：/work/book/utils_new/svn/myproject

「

[rootOseruer nyproject]# Is
branches tags trunk
[root@seruer myproject]#|sun copy trunk branches/test-branch|
A
branches/test-branch
[ rooteseruer nyproject ] #
[root@seruer myproject ]»| sun'commit -m "test—branch 생'.서" |
인 중 영역 (realm): <http://localhost: 8 0> My Project
•satgat •희 암호:

추가

branches/test-branch

커밋된 리비전 耳.
[rooteseruer nyproject]# |

[그림 14-47] svn branch 명령으로 브랜치

브랜치를 했으면 브랜치한 트리를 받아와야 해당 브랜치 트리를 가지고 수정하고

commit할 수 있다. 브랜치한 트리를 받아 오려면 새로운 작업 디렉토리에서 다음과 같
은 checkout 명령..0-루 받아올 수 있다.

[그림 14-48] 브랜치 checkout

이후 test-branch에서 작업한 내용들은 test-branch에 반영된다. 그러면 메인 트리

（ tr니nk） 가 아닌 test-branch 트리에서 마음껏 테스트할 수 있다.

14장_ Subversion, CVS

===== PAGE 693 =====
이때 브랜치 트리의 리비전 번호와 trunk 트리의 리비전 번호는 별개가 아니다.

Subversion은 리비전 번호를 저장소 단위로 관리하기 때문에 브랜치 트리가 변경되면
저장소의 리비전 번호가 바뀐다. 그러면 trunk의 HEAD 리비전도 바뀐다. 저장소에 포
함된 모든 것은 저장소 리비전 버전으로 사용하기 때문이다.

I merge 명령으로 머지하기
머지는 파일들을 비교해 달라진 부분을 하나로 합치는 과정이다. 머지라는 이름 때문에
파일을 합친다는 느낌이 들겠지만 사실은 서로 지금까지 달라진 부분들을 찾아 달라진
부분을 적용시키는 과정이다. 일종의 리비전별 달라진 내용을 패치한다고 생각하면 이
해하기 쉬울 것이다.
머지는 브랜치에서 작업을 하다 브랜치 내용을 trunk 에 반영하고 싶을 때 하곤 한다.
브랜치의 작업 내용을 trunk에 반영할 때 수작업으로 일일이 반영한다면 노력이 많이
든다. svn merge 명령은 이렇게 일일이 수작업으로 해야 할 일들을 기계적으로 자동
화시켜주는 명령이다.
물론 기계적으로 머지를 수행하기 때문에 충돌이 나거나 하는 문제가 발생할 수 있다.

Subversion의 머지는 완벽한 머지를 추구한다기보다는 기계적으로 할 수 있는 것들만
머지하고 나머지는 사람에 게 맡기는 구조다. 이 정도만 해 줘도 삶이 한결 윤택해질 수
있다.
머지를 테스트하기 위해 먼저 checkout 한 test-branch 의 main.c 파일을 다음과 같이
수정한다.

[그림 14—49] test—branch의 m기n.c 파일 수정 내용

그리고 commit한다.

692

6부—프로젝트버전 관리

===== PAGE 694 =====
우 root@server：/work/book/utils_new/svn/test-branch
[rootQseruer test-branch]# sun ci -m "머지 테스트‘
인증 영역 (realm): <http://localhost: 8 0> My Project
王atgat•의 암호:
전송중
main/main .c

파임 데이터 저송종 커밋된己jui 전호丁
[root@server test-branch]#
[rooteseruer test-branch]# |

[그림 14-50] 수정 내용 commit

그러면 test-branch의 리비전 번호는 5가 된다. 최초 test-branch를 브랜치했을 때 리비
전 번호는 4였는데 5가 된 것이다. 머지를 하려면 리비전 번호를 알아 두는 것이 중요하다.
자, 그러면 다시 trunk로 간다.
머지하기 전에 먼저 trunk의 파일들을 정리한다. 수정했는데 아직 commit 안 된 것이
있다면 commit하고, 저장소의 최신 버전으로 update도 한다. 그러면 trunk 쪽에서는
머지를 위한 준비가 다 된 것이다.
일반적으로 머지를 할 때는 trunk의 최신 버전과 test-branch의 최신 버전을 머지한
다. 이때 test-branch가 처음 시작되었을 때부터 현재까지 변경된 내용을 trunk에 적
용시 킨다.
그러면 test-branch는 리비전 얼마에서부터 시작됐는가? test-branch는 리비전 4에
서부터 시작되었고 현재는 5다.
그렇다면 trunk에서 다음 명 령을 사용해 머지 한다.
$ svn merge -r 4:HEAD http://localhost/svn/myproj ect/branches/test-branch
또는

$ svn merge -r 4:5 http://localhost/svn/myproject/branches/test-branch

(흐 server trunk ]tt| svn update]

| [root

|인 증 영 역 (re31m): <http://localhost :80> MyProject
satgat •의 암호:
리비전 5.

(흐
레스바

[ root
seruer trunk ] It________________________________________________
JrootQseruer trunk]tt
n merge —r 4:HERD http://localhost/svn/i
j
|ro’j
~anch
s^te
bran
인승 앵 으] (realm): <http ://16calhost :80> MyProject
•satgat•으j 암호:

['司
브 하广

엣[

진

— 병합중: r5 리비전을 ’.•에 병함:
U main/main.c
[root@seruer

바'unk]tt |

[그림 14-51] svn merge 명령으로 머지

14장_ Subversion, CVS

693

===== PAGE 695 =====
머지를 할 때 -r 4：HEAD의 의미는 “리비전 4에서 저장소에 있는 최신 리비전까지”라는
의미다. 저장소에 있는 최신 리비전은 5이기 때문에 리비전 4에서 5까지 test-branch
에서 있었던 변경을 trunk에 적용시킨다.
머지를 할 때 브랜치의 리비전을 반드시 최신으로 해 줄 필요는 없다. 특정 브랜치 리
비전까지 머지를 하려고 한다면 -r 4：［특정 리비전］과 같은 형식으로 해 주면 된다.
위와 같은 svn merge 명령을 내렸으면 머지가 모두 끝났다. 그러면 머지가 잘 되었는
지 main.c 파일을 열어 한번 확인해 보자.

［그림 14—52］ 머지된 main.c 파일 내용

머지가 잘된 것을 확인할 수 있다. 머지가 제대로 되었으면 commit해야 저장소에 반영
된다. 머지가 잘못되어 머지한 내용을 버려야 한다면 다음과 같이 한다.
$ svn revert main.c

I copy 명령으로 태깅하기
태깅은 특정 시점의 프로젝트 파일들을 표시하는 것이다. 태깅은 보통 릴리즈를 했거나
버그 픽스를 해서 특정 시점을 표시해야 될 때 하곤 한다. 이렇게 특정 시점의 프로젝
트 파일들에 태깅을 하면 나중에 해당 시점의 프로젝트 파일들을 다시 보고자 할 때 쉽
게 찾을 수 있다.
태깅하는 방법은 svn copy 명령으로 브랜치하는 것과 같다. 다음 명령은 trunk 를

tags/release-0.1 로 태깅하는 명령이다.
$ svn copy trunk tags/release-0.1
$ svn commit

694 6부—프로젝트버전 관리

===== PAGE 696 =====
if root@server：/work/book/utils_new/svn/myproject
[root@seruer myfroject]히"g〔^"rr造'허후,하;丁'짜쁘y

f

fi
tags/release-Q.1
[t*oot@seruer myproject]# sun commit -m "release-0.1 태그 생성
인 증 영 역 （ rea]믜） : <http ://localhost :88> MyProject
‘satgat•의 암호:
추가
tags/release-0.1

커밋된 리비전 6.
[root@seruer myproject]# |

[그림 14-53] release-0.1 태그 생성

Subversion에서는 브랜치든 태깅이든 동일하게 취급된다. 때문에 되도록 태깅한 것들
은 태깅의 본래 의도에 맞게 건드리지 말아야 한다.

| 이eanup 명령으로 작업 사본 정리하기
간혹 다른 사용자와 svn 명령이 충돌해 현재 처리 중인 svn 명령을 강제로 종료할 때가
있다. 예를 들면 다른 사용자가 commit를 하고 있을 때 공교롭게도 update 명 령을 수
행해 update 시간이 너무 길어 참지 못하고 食리 + c 키를 눌러 중단하는 일과 같은 경
우가 이 에 해당한다.
이럴 때 잘못되면 작업 사본 디렉토리에 잠금 파일들이 생성될 수 있다. 잠금 파일이
생성되면 svn 명령을 제대로 처리하지 못하는 일이 발생한다. 이럴 때는 다음과 같이

svn cleanup 명 령을 수행하며 잠금 파일들을 정리한다.
$ svn cleanup

I dump/load 명령으로 백업 및 복구하기
저장소가 오류가 나 그동안 작업한 내용이 다 사라져버리는 것만큼 끔찍한 재앙도 없
을 것이다. 때문에 저장소를 백업하는 일은 매우 중요하다. 그러면 어떻게 백업하면 될
까? 저장소 디렉토리를 압축해 보관하면 되지 않을까? 물론 그렇게 해도 된다. 그런데
그렇게 할 경우 다시 복구할 때 OS 나 Subversion 버전을 원래의 환경으로 맞춰 주어
야 한다. 하지만 dump와 load를 이용해 백업 및 복구를 하면 Subversion이 있는 어디
에서든 복구하는 것이 가능하다.
먼저 저장소에서 다음과 같은 명령을 내리면 백업된다.
$ svnadmin dump myproject > myproj ect.backup

14장_ Subversion, CVS

695

===== PAGE 697 =====
그리고 복구는 다음과 같이 하면 된다.
$ svnadmin load myproj ect < myproj ect.backup

I 충돌에 관한 해결법
충돌이란 Subversion 0 ] 저장소 내용과 새로운 내용을 합치고자 할 때 발생한다. 일반
적으로 두 내용의 상이한 부분이 다른 부분이라면 충돌은 발생하지 않는다. 하지만 두
내용의 같은 부분이 서로 상이하다면 Subversion이 해당 내용들을 합치지 못해 충돌
이 발생한다.
여러 사람이 동시에 작업하다 보면 충돌과 같은 문제가 반드시 발생한다. 충돌 문제는

merge 시나 update 시에 발생하고, 충돌이 발생하는 상황은 대개 같은 부분을 수정했
을 경우 자주 발생한다.
충돌 상황을 쉽 게 예를 들면 다음과 같다. 먼저 udong 사용자와 satgat 사용자는 동일
한 리비전으로 update해 동일한 프로젝트 파일들을 가지고 있다. 이 상황에서 그림과
같이 udong 사용자가 memo.c 파일에 sleep(l)；이라는 내용을 추가하고 commit했다.
그러 면 저장소는 udong 사용자가 commit한 내용으로 되 어 있을 것이 다.

[그림 14—54] udong 사용자 memo.c 수정 내용

그리고 공교롭게도 satgat 사용자 역시 다음 그림과 같이 udong 사용자가 수정한 부분
과 같은 부분을 수정하고 commit을 시도한다.

[그림 14—55] satgat 사용자 memo.c 수정 내용

696

6부_ 프로젝트 버전 관리

===== PAGE 698 =====
그러면 다음과 같이 commit이 실패했다는 메시지가 출력되고 memo.。｝ 만료되었기
때문에 업데이트하라는 메시지가 출력된다. 아직까지 충돌 상황은 아니다. 단지 satgat
사용자가 commit 하려고 하는데 누군가가 먼저 commit해 satgat 사용자가 최신 버전
으로 니pdate해야 commit할 수 있는 상황일 뿐이다.
/ root@server：/work/book/utils_new/svn/myproject/trunk
[rootBseruer triml《]lUsun ci -m "wa&: 함주 호촐 주하리广
인증 영역 (realm): <http: //localhost :88> MyProject
’udong’으j 암호:
인증 영역,(realm): <http://localhost: 8 0> My Project

사용자명 ：satgat
■satgat’의 암호:
전송중
trunk/memo/memo. c
sun: 커밌이 실패하었습니다:
느 느 __ _ _ .
아m:| 파힐 호든 티 헤序치 'memo.c• 는 만료된 것입 니 다; 업 데0| 트 하세

111Tlit

sun: resource out of date; try updating
[root@seruer trunk]# |

[그림 14-56] commit 실패 메시지

이 상황에서 svn update 명령을 내리면 두 내용의 같은 부분이 충돌해 충돌 메시지가
발생한다.
/ mot@server：/work/book/utils_new/svn/myproject/trunk
[root@seruer trunk]1t| sun update 厂
인 증 영 역 (realn)： <http ://localhost :80> MyProject
•주atgat•의 암호:

충돝 발견됨 : 'PI리w/meno.c'.
선택:’다음에 시도, (dF) diH-Full, (e) edit,
(nc) mine-conflict, (tc) theirs-conflict,
(S) 모든 옵션:I

[그림 14-57] memo.o 충돌 메시지

최신 버전 svn은 충돌 상황이 발견되면 친절하게 다음 키워드들을 눌러 충돌을 해결하
라고 알려주는데, 각 키워드가 의미하는 바는 다음과 같다.

n P：

다음에 시도

P를 누르면 충돌 상황을 해결하지 않고 그냥 넘어간다. 그냥 넘어가면 memo.c가 있는
디렉토리에 memo.c, memo.c.r5, memo.c.r6, memo.c.mine 파일이 각각 생성되는데,
각 파일이 의미하는 바는 다음과 같다.

14장_ Subversion, CVS 697

===== PAGE 699 =====
[표 14-2] 충돌 파일 설명

파일명

설명

memo.c

충돌이 난 파일로. 내부에 충돌 정보가 들어 있다.

memo.c.r5

현재 작업 파일의 저장소 BASE 파일이다.

memo.c.r6

저장소에 있는 최신 버전 HEAD 파일이다.

memo.c.mine

현재 작업자가 작업하고 있는 파일이다.

p를 눌러 그냥 넘어갔다면 충돌을 해결하기 전까지는 commit을 하지 못한다. 충돌을
해결하려면 다음과 같은 방법을 선택해 충돌을 해결해야 한다.

1. 자신이 작성한 내용을 버리고 저장소에 있는 최신 버전 HEAD 파일 내용으로 충돌을 해결하고자
한다면 다음 명령을 수행한다.
- cp -f memo.c.r6 memo.c # 저장소 내용으로memo• c 파일을 덮음
- rm -rf memo.c.r5 memo.c.r6 memo.c.mine

2. 자신이 작성한 내용으로 충돌을 해결하고자 한다면 다음 명령을 수행한다.
- cp -f memo. c .mine memo. c # 자신이 작성한 내용으로 memo. c 파일을 덮음
- rm -rf memo.c.r5 memo.c.r6 memo.c.mine

3. 문제가 복잡해 충돌을 수작업으로 직접 해결해야 한다면 다음 명령을 수행한다.
— vi memo. c
# 직접 수정
- rm -rf memo.c.r5 memo.c.r6 memo.c.mine

층들을 해결하려면 위 명령들과 같이 충돌 시 발생하는 memo.c.r5, memo.c.r6, memo,
c.mine 파일을 지워 주어야만 충돌이 해결된다. memo.c.r5, memo.c.r6, memo.c.mine
파일이 지워지지 않았다면 계속 충돌 상황임으로 commit을 할 수 없다.

3번 방식으로 충돌 문제를 해결해야 하는 되는 경우는 충돌한 두 내용이 다 필요한 경
우다. 예를 들면 공교롭게 satgat 사용자와 udong 사용자가 같은 부분을 수정해 충돌
이 발생했지만 두 사용자의 수정 내용이 모두 필요해 일일이 수작업으로 소스 코드를
바로 맞춰야 하는 경우 3번과 같은 방식으로 해결할 수 있다.

698 6부_ 프로젝트버전 관리

===== PAGE 700 =====
이때 충돌이 발생한 memo.c 파일을 열어보면 ［그림 14-58］ 과 같이 충돌 정보가 들어
있다. 충돌 정보에서 .mine 부분은 본인이 작성한 내용이고, .r6 부분은 저장소 최신 버
전의 내용이다.
개발자는 충돌 내용을 참고해 올바른 소스 코드로 충돌 내용을 제대로 수정한다. 그리
고 충돌을 해결한 후에 memo.c.r5 memo.c.r6 memo.c.mine 파일을 지워주면 충돌
이 해결된다.

@ df： diff-full
df 키워드를 누르면 다음 그림과 같이 머지된 부분을 출력해 보여준다. 일단 df 키워드
로 머지된 부분에서 충돌이 발생한 부분을 확인하고 p 를 입력해 그냥 넘어갈 것인지
아니면 이 자리에서 바로 해결할 것인지 결정할 수 있다.
/ root@server：/work/book/utils_new/svn/myprojecVtrunk

선택:
전환,

(p)

다음에

시도,

(df)

diFF-Full,

(e)

edit,

(r)

해결상태로

(me) mine—conflict, (tc) theirs-conFlict,
(s)
모든 옵션:dF
----- memo/.sun/text-base/memo.c.sun-base 화 9뭘 22 88:40:56 2009
+++ memo/.sun/tmp/inemo. c. tmp
화 9 월 22 88:44:16 2009
@@ -1,6 *1,12 0흐
ttinclude "diary.h"
int memo() {
printF("fupction me no. ''n");
♦««<« .mine I
+ wait (10);

+ sleep(l);
♦>>>>>>> .r6
return 8;
}

선택: (p) 다음에 시도, (df) diFF-full, (e) edit, (r) 해걸상태로
전환,
(me) nine-conFlict, (tc) theirs-conFlict,
(s)

모든 옵션:!

［그림 14-59］ df 키워드로 충돌이 난 부분을 확인

14장_ Subversion, CVS 699

===== PAGE 701 =====
@ e： edit
e 키워드를 입력하면 다음 그림과 같이 충돌된 소스 파일을 수정할 수 있게 에디터를 띄워
준다. 개발자는 에디터에서 파일의 내용을 올바르게 고쳐 충돌 상황을 해결할 수 있다.

[그림 14-60] e 키워드로 에디터를 동작시킨 모습

B me： mine-conflict
자기 자신이 작성한 내용으로 충돌 상황을 해결한다. 다음 명 령을 수행한 것과 동일하다.
$ cp -f memo.c.mine memo.c
$ rm -rf memo.c.r5 memo.c.r6 memo.c.mine
同 tc： theirs-conflict

저장소의 내용으로 충돌 상황을 해결한다. 다음 명령을 수행한 것과 같다.
$ cp -f memo.c.r6 memo.c
$ rm -rf memo.c.r5 memo.c.r6 memo.c.mine

0 s： 모든 옵션
선택 가능한 모든 충돌 처리 옵션을 다음과 같이 출력해 보여준다.
애 root@server：/work/book/utils_new/svn/myproject/trunk
선택: (P) 다음에 시도, (df) diFF-Full, (e) edit.
(me) mine-conflict, (tc) theirs-conFlict,
(5)모든 옵션흐］
(e) edit
(df) diFF-Full
(r) resolued

- change merged File in an
- show all changes made to
- accept merged version oF

editor
merged file
File

(de) display-conflict - show all conflicts (ignoring merged version)
(me) mine-conFlict
- accept ray uersion for all conflicts (same)
(tc) theirs-conflict - accept their uersion for all conflicts (same)
(mF) mine-Full
(tf) theirs-Full

- accept my uersion of
- accept their uersion

entire File (euen non-con
of entire File (same)

(p) postpone
(1) launch
(s) show all

- nark the conflict to
- launch external tool
- show this list

be resolued later
to resolve conflict

선택: (p) 다음에 시도, (df) difF-Full, (e) edit,
(me) nine-conflict, (tc) theirs-conflict,
(5)모든 옵션:|

[그림 14-61] s 키워드로 모든 옵션을 본 모습

700 6부—프로젝트버전 관리

===== PAGE 702 =====
svn에서 키워드를 입력해 충돌을 해결했건 수작업으로 충돌을 해결했건 충돌을 해결
했다면 그때부터는 기존의 방식대로 프로젝트를 진행한다.
오랫동안 서로 다르게 개발되던 브랜치를 머지하거나 오랫동안 update* 하지 않은
상태에서 계속 개발하다 commit하고자 할 때는 충돌이 많이 발생한다. 때문에 되도록
이면 자주 자주 update 해야 한다. 충돌이 많이 발생할 것 같은 상황이 된다면 meld와
같은 머지 툴을 이용해 수동으로 내용을 머지해 주는 것도 한 방법이다.
수동으로 머지한다는 말의 의미는 다른 디렉토리에 현재 저장소의 HEAD를 받은 후

meld 등과 같은 수동 머지 툴을 이용해 현재 작업 디렉토리와 HEAD의 다른 점을 비
교하면서 직접 추가할 건 추가하고 뺄 건 빼는 것이다.
이렇게 수동 머지를 하려면 meld와 같은 툴을 알아야 하는데, meld는 다음에 간단히
소개하기로 한다.

I 기타 간단한 팁
지금까지는 Subversion을 사용해 프로젝트를 진행하는 방법을 알아보았다. 지금까지
배운 내용만0-루두 프로젝트를 진행하는 데는 아무런 문제가 없다. 앞으로는 어떻게 하
면 좀 더 효율적으로 svn을 사용해 프로젝트를 진행할 수 있을지 그에 대한 팁들을 알
아보자.
해 meld를 이용한 똑똑한 머지

공동 프로젝트를 수행할 때 파일을 비교하거나 수작업으로 머지하는 일은 상당히 자주
발생한다. 예를 들면 자신의 작업 디렉토리에서 수정 내역을 비교 확인하거나, 다른 사
람이 작업한 내용을 자신의 작업 디렉토리에 반영하거나, 브랜치와 머지하거나, 저장소
내용을 update 할 때 변화가 심해 충돌이 많이 예상되는 경우에 meld 같은 툴을 사용
해 수동으로 머지한다.

meld 를 알 기 전에 필자는 파일을 비교하거나 머지할 때 vimdiff 를 사용하거나
kompare를 사용했었다. 그러다 어떤 친구에게 meld란 프로그램을 추천받고 감동받은
적이 있다. meld는 상용 머지 프로그램에 비해 뒤지지 않을 정도로 매우 훌륭한 머지
프로그램이다. 이제 필자는 meld 없이 큰 프로젝트를 머지하는 일은 상상도 하기 싫을
정도다.

14장_ Subv이'sion, CVS 701

===== PAGE 703 =====
meld를 사용하려면 먼저 설치를 해야 한다. 다음과 같은 명령으로 meld를 설치할 수
있다.
$ yum install meld
$ sudo apt-get intall meld

# 페도라사용자
# 우분투사용자

위 명령으로 설치가 되지 않는다면 http://meld.sourceforge.net에서 다운로드해 설
치하기 바란다.

meld는 굉장히 직관적인 머지 프로그램이기 때문에 따로 배울 필요 없다. meld를 사
용해 파일을 비교하거나 머지하는 명령은 다음과 같다.
$ meld
$ meld <dir>
$ meld <file>
$ meld <file> <file> [file]
$ meld <dir> <dir> [dir]

# 단순히 me Id를 동작

# <dir>을 버전 관리 브라우징
# <file>을 버전 관리 브라우징
# 둘또는 세파일간 비교
# 둘또는 세 디렉토리 간 비교

다음은 meld를 테스트하기 위해 필자가 test-branch를 임의로 수정하고 m이d trunk

test-branch 명령을 수행한 모습이다.

[그림 14-62] m이d trunk test-branch 명령 수행 모습

702 6부—프로젝트버전 관리

===== PAGE 704 =====
meld trunk test-branch 명령을 내리면 위와 같이 meld 가 수행된다. 이때 빨간색으
로 표시된 파일은 내용이 서로 다른 파일이다. 필자가 위 화면에서 Conflg.mk 파일을
더블 클릭하면 meld가 다음과 같이 서로 다른 부분을 깔끔하게 비교해 보여준다.

[그림 14-63] 내용이 다른 파일 비교

머지를 할 때는 위 그림에서 보이는 화살표를 클릭해 파일의 내용을 머지하는 것이 가
능하다. 그리고 파일 내용을 meld에서 바로 수정하는 것도 가능하다.

meld는 알아 두면 무척 편한 툴이기 때문에 Subversion을 배우는 사람들은 꼭 기억해
두기 바란다.

@ 암호 입력 없이 사용하는 법

지금까지는 Subversion 을 사용하면서 서버와 접속해 저장소에 뭔가를 해야 될 때는
항상 암호를 입력해야 했었다. svn 명령 시마다 매번 암호를 입력하려면 여간 귀찮은
일이 아니다.

http 방식과 svnserve 방식에서 암호 입력 없이 Subversion 명령을 사용하려면
-/.subversion/servers 파일에 다음 라인을 추가한다. 그러면 최초 한 번만 암호를 입
력하고 이후부터는 저장된 암호를 사용해 인증 과정을 수행한다.

14?|_ Subversion, CVS 703

===== PAGE 705 =====
〔예제 14-7)

〜/.subversion/servers 파일 내용

.•.상략

s tore-pas swords = yes
store-plaintext-passwords = yes
• •• 하략

저장된 인증 정보를 없애려면 ~/.subversion/auth 디렉토리를 지운다.

ssh 를 이용한 방식에서 암호 없이 svn 명령을 사용하려면 암호 없이 ssh 를 로그인할
수 있게끔 설정한다. 해당 설정 방법은 인터넷에 많은 참고 자료가 있으니 ssh 암호 없
이 로그인하는 법을 찾아 설정하기 바란다. 하지만 이렇게 되면 보안에 문제가 있을 수
있으므로 필자는 그다지 추천하지 않는다.
이상으로 Subversion에 대한 설명이 모두 끝났다. 지금까지 배운 내용만으로

Subversion을 프로젝트에 도입하는 데 아무런 어려움이 없을 것이다. 하지만 독자 중
에서는 아직 뭔가 모자람을 느끼는 사람들이 있을지 모르겠다.
필자가 유추하건대 그것은 아마 개발 방법론에 대한 설명이 없어서 그럴 수 있을 것이
라 본다. 예를 들면 Subversion을 사용해 개발하는 데 있어 commit은 얼마나 자주 할
것이며, 브랜치는 언제 할 것이며, 소스를 관리하고 프로젝트를 진행하는 방식은 어떠
해야 되는지 하는 것들 말이다.
불행히도 이 책에서 그런 내용을 주제로 다룰 수 없다. 범위를 벗어나는 것도 문제지만
개발 프로세스는 회사마다 다르고, 프로젝트 성격에 따라서도 다르기 때문이다. 때문에
개발 프로세스에는 정답이 없다. 나머지 부분들은 독자들에게 맡긴다. 어떻게 하면 좀
더 효율적으로 프로젝트를 운영할 수 있을지 직접 해 보면서 고민하기 바란다.

Levs 를이용한 버전관리
이번 절에서는 CVS를 설명한다. CVS는 과거에 많이 사용되던 버전 관리 툴이었다. 현
재는 Subversion의 등장으로 말미 암아 과거처 럼 많이 사용되지는 않는다. 하지만 그렇
다고 해서 CVS를 몰라서는 안 된다. 아직까지 CVS를 사용하는 곳이 제법 많이 있으며,

CVS는 버전 관리 툴에 있어 중요한 의미를 지니고 있기 때문이다.

704 6부_ 프로젝트 버전 관리

===== PAGE 706 =====
그리고 Subversion이 항상 CVS보다 좋다고 말할 수는 없다. 프로젝트 단위가 커지면

Subversion은 버전 정보를 관리하기 위한 메타 데이터를 위해 너무 많은 하드 디스크
공간을 사용한다. 거의 원본 소스와 맞먹을 정도로 차지할 때도 있다. 이런 문제로 말미
암아 실제로 필자가 관리하고 있는 서버의 버전 관리 툴을 Subversion에서 CVS로 교
체한 바 있다.
때문에 CVS가 Subversion에 비해 많은 부분이 구식이기는 하지만 CVS도 존재 이유가
있기 마련이다. Subversiono］ CVS를 모태로 만들어졌기 때문에 CVS와 Subversion은
기능적으로 매우 유사하다. 그래서 Subversion을 알면 CVS도 저절로 알 수 있다.
때문에 필자는 이번 과정을 되도록 간단히 설명하고자 한다. CVS의 위상 등으로 볼 때
독자가 사용할 수 있을 정도로만 설명하는 것이 맞을 거라 본다.

I CVS 소개
CVS 는 Concurrent Versions System의 약자로, Subversion 과 마찬가지로 여러 사람
이 공동으로 프로젝트를 수행할 때 발생할 수 있는 소스 충돌이나 소스 동기화 문제들
을 해결하기 위해 개발됐다.
원래 CVS 이전에 RCS가 있었다. RCS는 개개의 파일 버전을 관리하는 유틸리티인데,
이런 RCS의 관리 기능을 프로젝트 단위 또는 모듈 단위로 확장해 만든 것이 바로 CVS
다. 그래서 CVS와 RCS는 많은 부분에서 닮았다. 가끔 vi ［파일명］을 입력한다는 것이
잘못 입력해 ci ［파일명］ 형식으로 명령이 내려져 파일명이 ［파일명］,v 형식으로 바뀌
어 버리는 황당한 경험을 해 본 독자들이 있을 것이다. ci 명령이 바로 RCS에서 사용하
는 체크인 명령이다.

昌
CVS 서버

.••거서-'..

［그림 14-64］ CVS 개발 구조

14?|_ Subversion, CVS 705

===== PAGE 707 =====
Subversion과 마찬가지로 CVS 역시 중앙 집중식 버전 관리 툴이다. 개발자들은 CVS
서버에서 프로젝트 파일을 받아와 서버와 동기화시키면서 개발을 진행한다. 이때 각 프
로젝트 파일의 버 전 관리와 각종 동기화 문제는 CVS가 담당한다.

6 CVS 서버 설정
Subversion과 마찬가지로 CVS를 프로젝트에 도입하려면 먼저 CVS 서버를 설정해야
한다. CVS 서버를 설정하려면 시스템에 CVS가 설치되어 있어야 한다. cvs -v 명령을
내리면 CVS가 설치되어 있는지 설치되지 않았는지 확인할 수 있다. 설치되지 않았다면

yum이나 apt-get으로 설치하기 바란다.

| 저장소 디렉토리 생성 및 초기화
CVS를 설치했거나 설치되어 있는 것을 확인했으면 프로젝트에서 사용할 프로젝트 파
일들을 보관하는 저장소(Repository) 디렉토리를 생성한다.
$ mkdir /home/cvs

觸 root@embedded：~
[root@embedded rootjttjgkdir /home/cus
[root
embedded root]#

（ 흐

［그림 14-65］ 저장소 디렉토리 생성

필자는 /home/cvs 디렉토리를 저장소 디렉토리로 사용하고자 한다. 이후 프로젝트에
사용될 파일들은 /home/cvs 디렉토리 아래에 두고, 개발자들은 저장소 디렉토리에 등
록된 프로젝트 파일을 받아 사용할 것이다.
저장소 디렉토리를 생성했으면 이제 초기화한다. 초기화하는 일은 저장소 디렉토리에

CVS에서 사용하는 제어 파일들이 들어 있는 디렉토리를 생성하는 일이다.
$ cvs -d /home/cvs init

위 명령을 내리면 ［그림 14-66］ 과 같이 /home/cvs 디렉토리에 CVSROOT 디렉토리
가 생성되면서 저장소가 초기화된다.

706

6부_ 프로젝트 버전 관리

===== PAGE 708 =====
B root@embedded ： ~

昌® E31

[rootSenbedded root]ttjcus -d /home/cvs inif]”~
[root
embedded root]tt
[rootBe^edded root]# is /home/cus/

（흐

（흐embedded root]tt |

[root

[그림 14-66] 저장소 초기화

| CVS 사용자 생성 및 권한 설정

저장소 디렉토리까지 초기화했으면 시스템에 CVS 유저를 등록하고 저장소 디렉토리에
대한 cvs 유저의 접근 권한을 설정한다. 이후 CVS 서버에 접속해 저장소 디렉토리에
접근할 사용자들은 모두 시스템의 cvs 유저 권한으로 접근할 것이다.
$ adduser cvs
$ chown root.cvs /home/cvs -R
$ chmod 770 /home/cvs -R

위 명령을 순차적으로 내리면 시스템에 CVS 유저와 그룹이 생성되고 저장소 디렉토리
의 권한이 CVS 유저와 CVS 그룹에 맞게 설정된다.

[그림 14-67] CVS 유저 생성 및 권한 설정

CVS 유저를 추가만 하고 이대로 그냥 둔다면 CVS 유저에 대한 암호가 없어 보안상 위험
할 수 있다. passwd cvs 명령으로 cvs 사용자의 암호를 아무거나 입력시켜 놓으면 된다.
이후 cvs 사용자로 로그인할 일이 거의 없기 때문에 굳이 암호를 기억할 필요는 없다.

I CVS 사용자 등록
이제 CVS 사용자를 등록한다. CVS 사용자는 CVS 서버에 인증을 거쳐 프로젝트 파일
을 받아올 때 인증에 유효한 사용자를 의미 한다. CVS 사용자는 시스템 사용자와 같이
실제 시스템 사용 권한을 가지고 있는 대상은 아니며, 단지 CVS 서버만이 인지하는 사
용자다.

14장_ S니bversion, CVS

707

===== PAGE 709 =====
CVS 사용자를 등록하는 방법은 ［저장소 디렉토리］/CVSROOT/passwd 파일을 ［예제
14-8］ 과 같이 생성하면 된다.
〔예제 14-8〕 /home/cvs/CVSROOT/passwd 파일의 내용

satgat:Gj 4MN6BEZsJb6:cvs
udong:EBry7 DMv/HWKg:cvs
anonymous::cvs

passwd 파일을 보면 각각의 사용자 정보가 콜론(:)을 기준으로 세 개의 필드로 구분되
어 있다. 첫 행의 satgat은 CVS 사용자 ID고, Gj4MN6BEZsJb6는 crypt 알고리즘으로
암호화된 satgat 사용자의 암호이고, 마지막 cvs는 저장소에 접근할 때 시스템에 등록
된 cvs 유저의 권한으로 접근한다는 의미다.

crypt 알고리즘으로 암호화된 암호를 생성하는 방법은 Subversion과 같이 다음 명령
을 사용한다.
htpasswd -n ［ ID］

［그림 14-68］ 은 htpasswd 명령으로 satgat 사용자와 니dong 사용자의 암호화된 암호
를 생성하는 예다.
fl [screen 1： bash] root@os：~
|[root@os' root]tt htpasswd -nb satgat 1234

Fa€jaTFfiAD93§aX司司피
[rootBos root]tt htpasswd -nb udong abed
udong': gl .H2VK；nxMm； |
|[root@os root]tt |

［그림 14-68］ 암호화된 암호를 생성한 예

［그림 14-68］ 에서 사각형으로 표시된 부분을 복사해 CVSROOT 디렉토리에 있는

passwd 파일의 암호 필드에 붙여 넣으면 된다.
현재 passwd 파일에는 anonymous 사용자가 등록되어 있는데, 암호 필드 부분이 비
어 있음을 확인할 수 있다. 오픈 소스를 개발하고 있어 익명 사용자에게 소스를 공개하
고자 한다면 이렇게 anonymous 사용자를 등록하고 암호를 비워둔다. 그리고 익명 사
용자를 위해 몇 가지 설정을 더해야 한다. 그냥 이렇게 익명 사용자를 등록시켜 놓으면
익명 사용자에게 쓰기 권한이 있어 위험하기 때문이다.

708 6부_ 프로젝트 버전 관리

===== PAGE 710 =====
익명 사용자에 게 읽기 권한만 부여하려면 /home/cvs/CVSROOT 디 렉토리에 readers
파일을 생성하고 ［예제 14-9］ 와 같이 읽기 권한만 부여할 사용자 ID를 추가한다.
〔예제 14-9］

/home/cvs/CVSROOT/readers 파일의 내용

anonymous

readers 파일을 생성해 접근 권한을 설정하는 방법 외에 writers 파일을 이용해 접근
권한을 설정할 수도 있다. /home/cvs/CVSROOT/writers 파일을 생성하면 writers
파일에 등록된 ID만 쓰기 권한이 주어지고 나머지 ID에는 읽기 권한만 주어진다. 최종
적으로 생성한 /home/cvs/CVSROOT/passwd 파일을 열어보면 ［그림 14-69］ 와 같
은 형 태가 된다.

圈 root@embedded：/
^atgat:ETND93SaXW5yw:cus
udong:gl.H2YK1mxMm2:cus
anonymous::cus

1,1

모두 B

[그림 14—69] /home/cvs/CVSROOT/passwd 파일의 내용

I CVS 서버 실행
cvs 사용자까지 설정하였으면 마지막으로 cvs 서버를 실행한다. 슈퍼 데몬으로
xinedt 를 사용하는 레드햇 계열 리눅스에서 CVS 서버를 실행하려면 /etc/xinetd.d 디
렉토리에 다음과 같은 내용의 cvspserver 파일을 생성한다.
〔예제 14-10)

service

/etc/xinetd.d/cvspserver 파일의 내용

dvspserver

{
disable
flags
socket_type
wait
user
server
qerver_args

= no
= REUSE
= stream
= no
= CVS
= /usr/bin/cvs
= ——al丄ow-root=/home/cvs pserver

}

위 파일에서 server 필드에는 cvs 명령의 패스를 적는다. 레드햇 계열 리눅스라면 /usr/

bin 디렉토리에 cvs 명령이 있으므로 /usr/bin/cvs라고 적는다.

14장_ Subversion, CVS

709

===== PAGE 711 =====
server_args에는 CVS 서버를 실행시킬 때 넘겨줄 인자를 적는다. 원래 /usr/bin/cvs 명
령은 CVS 서버의 기능과 CVS 클라이언트의 기능을 동시에 가지고 있는데, cvs 명령을
수행할 때 뒤에 따라오는 인자에 따라 서버가 될 때가 있고 클라이언트가 될 때가 있다.

cvs 명령의 인자로 -- allow-root=/home/cvs pserver 를 주면 서버의 기능을 수행하
는데, 저장소 디렉토리로 /home/cvs를 이용한다.

/etc/xinetd.d/cvspserver 파일을 작성 했으면 다음 명 령으로 xinetd 슈퍼 데몬을 재시
작해야 한다.
$ service xinetd restart

[그림 14—70] xinetd 슈퍼 데몬 재시작

슈퍼 데몬을 재시작했을 때 cvspserver가 정상적으로 설정되었다면 netstat -an 명령
에 의해 cvspserver의 포트인 2401 포트가 열려 있음을 확인할 수 있다.
netstat -an | grep 2401

[그림 14—71] netstat -an I grep 2401 명령으로 확인한 서버 작동 여부

위와 같이 2401 포트가 열려 있는 것을 확인했다면 CVS 서버 설정이 모두 끝난 것이다.

07 CVS를 사용해 프로젝트 진행
서버 설정 이 끝났으면 다음 할 일은 앞으로 사용할 프로젝트 파일을 CVS 저장소 디 렉
토리에 등록시키는 일이다. CVS 저장소 디렉토리에 프로젝트 파일을 등록시키려면 먼
저 CVS 서버로 로그인해야 한다.

710 6부_ 프로젝트버전 관리

===== PAGE 712 =====
I CVS 서버에 로그인
로그인 과정은 최초 한 번만 수행하면 된다. 로그인이 성공하면 사용자 홈 디렉토리의

.cvspass 파일에 로그인 정보가 유지되기 때문에 다음부터는 로그인 과정을 수행하지
않아도 원하는 작업을 수행할 수 있다.
로그인 명령을 설명하기 전에 먼저 CVS 명령 구조를 알아보자. CVS 서버로 로그인하
거나 서버에서 파일을 받아오고, 수정한 파일을 서버에 반영하는 등 모든 작업은 CVS
명 령으로 이루어진다. cvs 명령은 모두 다음과 같은 형식이다.
$ CVS ［전역 옵션］ 명령 ［명령 옵션］

먼저 CVS 명령이 오고 그 다음으로 전역 옵션이 온다. 전역 옵션은 CVS 명령을 사용할
경우 전역 사항들을 지정할 때 사용하고, 대표적인 전역 옵션으로 저장소 디렉토리를
지정하는 -d 옵션과 결과 메시지를 출력하지 않는 -q 옵션 등이 있다.
전역 옵션 뒤에는 명령이 오는데, 이런 명령에는 CVS 서버로 로그인하고 파일을 받아
오고, 파일을 동기화시키는 둥의 일을 수행하는 명령이 온다. ［표 14-3］ 에는 대표적인
명령을 나열했는데, 읽어보면 대략 명령의 성격이 어떤지 알 수 있을 것이다.
［표 14-3］ CVS 명령의 종류
전체 명령

동의어

| 명령 설명

login

CVS 서버로 로그인

logout

.cvspass 파일에서 저장소 제거

import

프로젝트 파일 등록

checkout

co, get

프로젝트 파일 가져오기

commit

ci

프로젝트 파일 수정 후 CVS 서버에 반영

update

up

CVS 서버의 최신 버전을 작업 디렉토리에 반영

add

new

파일 또는 디렉토리 추가

remove

rm, d이ete

파일 삭제
파일 버전에 따른 차이점 비교

diff
log

rlog

파일 로그 보기

annotate

ann

라인별 정보 출력（작성 날짜, 작성자 등）

status

파일 상태 보기

history

각종 히스토리 보기

tag

freeze

프로젝트 파일들 태깅하기

rtag

저장소 디렉토리에 태깅하기

release

모듈 release

14장_ Subversion, CVS 711

===== PAGE 713 =====
명령 다음으로 각 명령에 대한 옵션이 온다. 가령 cvs -q commit -m "새로운 내용 추
가”와 같은 명령이 있을 때 -m "새로운 내용 추가’, 같은 것이 commit 명령의 옵션이다.

cvs 명령 구조에서 역시 대괄호로 묶여 있는 것들은 있을 수도 있고 없을 수도 있는 부
분을 의미한다. 즉, 전역 옵션이나 명령 옵션은 설정 상태나 사용하는 명령의 종류에 따
라 있을 수도 있고 없을 수도 있다.

ws 명령 구조를 알았으니 이제 login 명령을 내려 CVS 서버에 로그인한다. 먼저 로그
인할 현재의 상황을 그림으로 나타내면 다음과 같다.
203.237.229.121

CVS 계정

CVS 서버
［그림 14-72］ 로그인 상황

지금 로그인하려는 상황은 김삿갓이 자신의 PC에서 자신의 CVS 사용자 ID인 satgat으
로 로그인하려는 상황이다. 김삿갓이 CVS 서버에 로그인하려면 자신의 PC에서 다음
명령을 입력한다.
$ cvs -d :pserver:satgat@203.237.229.121:2401/home/cvs login

-d 옵션 뒤에 오는 :pserver：satgat@203.237.229.121：2401/home/cvs의 각 필드가
의미하는 바는 다음과 같다.
: ［접속 방법］ : ［ CVS 사용자 ID］ @ ［원격지 CVS 저장소 디렉토리 주소］

pserver는 CVS 서버에 접속하는 방법을 의미한다. pserver 대신 ext를 사용하면 시스
템 계정을 이용해 rsh나 ssh로 접속하는 방법을 의미한다. 시스템 계정을 이용해 rsh나

ssh를 이용해 CVS 서버에 접근하는 방법은 나중에 다룬다.
satgat은 CVS 사용자 ID를 의미하고, 203.237.229.121 ：2401/home/cvs는 CVS 서버
저장소 디렉토리 주소를 의미한다. 즉, 저장소 디렉토리는 203.237.229.121 컴퓨터의

/home/cvs 디 렉토리를 의미하고, 중간에 있는 2401은 포트 번호를 의미 한다.
203.237.229.121은 필자가 설정한 CVS 서버의 IP 주소다. 독자는 자신이 CVS 서버로
설정한 컴퓨터의 주소를 적어주면 된다. 한 대의 PC에 CVS 서버를 설정하고 CVS 클라
이언트도 같이 사용하고자 한다면 위 명령에서 IP를 127.0.0.1 또는 localhost로 적어주
기 바란다.
712 6부_ 프로젝트버전 관리

===== PAGE 714 =====
위 명령을 내리면 ［그림 14-73］ 과 같이 Login... 메시지가 뜨고 CVS password： 프롬
프트가 출력된다. 여기에 satgat 사용자의 암호를 입력하면 로그인된다.
H [screen 1： bash] root@os ：/temp/book/diary

（흐

BIE

[root
os diary]tt cus -d :pser*uer:satgat@2O3.237.229.121:2401/home/cus login
Logging in to :pseruer:satgat@203.237.229.121:2401/home/cus
CUS password:
[rootSos diary|

［그림 14-73］ CVS 서버 로그인

위 그림과 같이 암호를 입력했을 때 아무런 메시지 없이 셸 프롬프트가 떨어지면 정상
적으로 로그인된 것이다.

CVS 서버에 명령을 내리려면 매번 -d :pserver：satgat@203.237.229.121：2401/home/
cvs 옵션으로 저장소 디렉토리를 지정해야 하는데, 옵션 인자가 길어 여간 불편한 것
이 아니다. 이럴 때는 전역 환경 변수 CVSROOT# 생성하고 그 값으로 ：pserver：satg

at@203.237.229.121：2401/home/cvs를 할당하면 -d 옵션을 붙이지 않고 cvs login과
같은 형식으로 명령을 사용할 수 있다. ［예제 14-11］ 과 같이 ~/.bash_profile 파일을
열어 다음 행을 추가한다.
〔예제 14-11)

...상략

export CVSROOT=:pserver:satgat@203.237.229.121:/home/cvs
... 하략

위와 같은 행을 ~/.bash_profile 파일에 추가했다면 다음 명령을 내려 설정한 내용을
현재 셸의 환경 변수에 적용시킨다.
$ source 〜/.bash_profile

이제는 -d 옵션으로 일일이 저장소 디렉토리를 지정하지 않아도 명령을 사용할 수 있
다. 로그인이 성공적으로 끝났으면 CVS 서버에 앞으로 프로젝트에서 사용할 프로젝트
파일들을 등록한다.

14장_ Subversion, CVS 713

===== PAGE 715 =====
I import 명령으로 CVS 서버에 프로젝트 파일 등록
등록할 프로젝트 파일은 이전에 “make” 장에서 사용한 diary 프로그램이다. 먼저 등록
할 파일들을 정리한다. 미리 컴파일되어 있는 오브젝트 파일들이 있다면 깨끗이 지우고
필요 없는 파일들도 다 제거한다.
ESElEBEi cvs 서버에 등록할 파일 리스트

diary.h :
#inc丄ude <stdio.h>
int memo();
int calendar();

m은mo.c :
#include "diary.h"
int memo() {
printf("function memo.\n");
return 0;
}

main.c :
#include "diary.h"
int main() {
memo();
calendar();
return 0;

calendar.c :
#include "diary.h"
int calendar() {
printf("function calendar.\n");
return 0;

}

}

[그림 14-74] CVS 서버에 등록할 파일 리스트

CVS 서버에 프로젝트 파일을 등록시키려면 CVS import 명령을 사용한다.
$ cvs import -m "diary 프로젝트 시작" diary project start

위와 같이 CVS import 명령을 내리면 저장소 디렉토리에 diary 디렉토리가 생기면서

diary 디 렉토리의 내부에 프로젝트 파일이 들어간다.
-m 옵션 뒤에는 자신이 적고 싶은 말을 적는다. 다음으로 CVS 서버의 저장소 디렉토
리에 생성될 디렉토리명을 적는다. CVS 서버의 저장소 디렉토리에 생성되는 디렉토리
를 모듈이라고 부르고, 위 예에서는 모듈명으로 diary를 사용한다.

714 6부_ 프로젝트버전 관리

===== PAGE 716 =====
그 다음에 오는 project와 start는 벤드 태그와 릴리즈 태그를 의미하는데, 크게 중요한
부분이 아니므로 아무 말이나 적으면 된다.
현재는 CVSROOT 환경 변수에 :pserver：satgat@203.237.229.121：/home/cvs 문
자열을 등록시켰기 때문에 -d 옵션을 사용하지 않고 바로 import 명령을 사용했다.

CVSROOT 환경 변수를 등록시키지 않았다면 다음과 같이 -d 옵션을 사용해야 한다.
$
cvs
-d
:
pserver:satgat@2
"diary 프로젝트 시작" diary project start

03.237.229.121:/home/cvs

import

-m

프로젝트 소스 파일이 있는 디렉토리에서 위 명령을 내리면 ［그림 14-75］ 와 같은 메시
지가 출력된다.

［그림 14-75］ 프로젝트 파일 등록

위 명령을 내린 후 저장소 디렉토리에 가보면 다음과 같이 diary 디렉토리가 생기고 내
용으로 diary 프로젝트의 파일들이 ［파일명］ ,v와 같은 이름으로 들어 있는 것을 확인할
수 있다.
■ ] root@embedded：/
[root@enbedded /]tt Is /hone^cus/
CUSROOT diary
[rootQeinbedded /]#
[root
embedded /]#
[rooteembedded /]# Is /home/cus/di
y/
Makefile, u calendar .c ,u diarji.h,u main.c,v memo .c ,u
[root
embedded /]# |

（ 흐

하'

（흐

［그림 14-76］ 저장소 디렉토리에 등록된 diary 모듈

［파일명］,V 파일을 열어보면 파일의 내용과 함께 CVS만이 이해하는 제어 문자열이 들
어 있는 것을 볼 수 있다. 저장소 디렉토리에 있는 파일들은 웬만해서는 직접 손대지
않는 것이 좋다. 실수로 저장소 디렉토리에 있는 파일들을 수정하면 CVS가 정상적으로

14장_ Subversion, CVS 715

===== PAGE 717 =====
작동하지 않을 수 있기 때문이다.
저장소 디 렉토리에 등록할 다른 프로젝트가 있다면 역시 같은 방법으로 등록시킨다. 물
론 등록시킬 때 모듈 이름은 다른 것으로 해야 한다. 나중에 저장소 디렉토리에 있는
파일들을 받아올 때 모듈 이름을 지정해 원하는 프로젝트 파일을 받아 올 수 있다.
저장소 디 렉토리에 앞으로 사용할 프로젝트 파일을 등록시켰으면 이제 본격적으로 프
로젝트를 진행한다. 저장소 디 렉토리에 있는 프로젝트 파일을 받아서 수정하고 수정한
내용을 다시 저장소 디 렉토리에 반영하고, 다른 사람이 저장소 디 렉토리에 반영한 내용
을 자신의 작업 디 렉토리에 동기화시키는 등의 일을 수행한다.

| checkout 명령으로 프로젝트 파일 받아오기
다음 명령을 내리면 저장소 디렉토리에 있는 diary 모듈의 프로젝트 파일들을 받아온다.
$ cvs checkout diary
또는

$ cvs co diary

당연히 위 명령을 내리기 전에 CVS 서버에 로그인이 되어 있어야 한다. 필자는 현재

CVS 서버에 프로젝트 파일을 등록할 때 satgat 계정으로 로그인했기 때문에 바로 위
명령을 사용할 수 있다. 로그인하지 않았다면 위 명령을 내리기 전에 cvs login 명령으
로 로그인부터 하기 바란다.

checkout 명령의 옵션으로는 저장소 디렉토리에서 받아올 모듈을 지정한다. 위와 같
이 받아올 모듈로 diary를 지정하면 ［그림 14-7刀과 같은메시지가 출력되면서 diary
모듈을 받아온다.
=1 root@os：/temp/book/projecl
[rootBos project]y| cvs.checkoiii：—di
cus seruer: Updating diary
U diary/Makefile
U diary/calendar.c
U diary/diary.h
U diar
main.c
U diary/neno.c
[rootQos project]#
[root
os project]# is

58

헤]‘'

시4 _|미 x|

으/

연
[root（흐os project]!*

£root@os project]# Is diarp/
CVS | Makefile calendar.c diary.h main.c
[rootBos project]tt |

［그림 14-77］ checkout 명령으로 파일을 받아옴

716 6부—프로젝트버전 관리

memo -c

三

===== PAGE 718 =====
위 그림에서 볼 수 있듯이 diary 디렉토리가 checkout 명 령을 내린 디 렉토리에 생성되
고 diary 디렉토리에는 프로젝트 파일들이 들어 있는 것을 확인할 수 있다. CVS 서버
에서 받아온 프로젝트 디렉토리에는 프로젝트 파일과 함께 CVS 디렉토리도 힘께 들어
있는 것을 확인할 수 있는데, CVS 디 렉토리에 들어 있는 파일들은 CVS 서버 정보와 파
일 정보가 들어 있기 때문에 웬만해서는 손대지 않는 것이 좋다.

| commit 명령으로 수정한 내용을 저장소 디렉토리에 반영
받아온 파일을 마음껏 수정했다면 commit 명령을 사용해 저장소 디렉토리에 반영해
야 한다. 그래야 다른 개발자들의 소스에도 자신이 수정한 내용을 적용시킬 수 있다.
필자는 ［그림 14-78］ 과 같이 main.c 파일을 열어 추가했다.

［그림 14-78］ main.c 파일에 주석 추가

main.c 파일을 변경할 경우 다음과 같이 commit 명령을 내리면 저장소 디렉토리에 있는
main.c,v 파일에 새로운 내용이 반영된다.
$ cvs commit -m "main. c 파일 주석 추기main. c
또는

$ cvs ci -m "main. c 파일 주석 추가" main. c

위 명령을 내리면 ［그림 14-79］ 와 같이 출력되면서 저장소 디렉토리에 있는 main.c
파일에 반영된다.
mot@os：/temp/book/projec^'diary
|[root@os diary]tt|cu； connit -m

..1111a~페三…'뿌적"추가" main.c

Checking in main.c;
|/home/cus/diaru/nain.c,u <-- main.c
new revision: ll2; previous revision: 1 Jl~]
done
[rootQos diary]tt |

［그림 14-79］ main.c 파일 CVS 서버에 반영

14장_ Subversion, CVS 717

===== PAGE 719 =====
출력 메시지를 유심히 보면 main.c 파일의 이전 버전이 1.1 이었는데 1.2로 변경되었다
는 메시지가 보일 것이다. 이렇게 모든 파일들은 최초 1.1 버전에서 시작해 파일이 수
정되고 변경되면서 commit 명령을 내릴 때마다 버전이 증가한다. CVS는 이렇게 파일
별로 따로 버전을 가지고 있는 반면 Subversion은 전체 저장소 버전만 가지고 있다.
이 렇 게 CVS 서버에 반영을 하였으면 이제 다른 사람이 CVS 서버에 로그인해

checkout할 경우 주석이 추가된 main.c 파일을 받을 수 있다. ［그림 14-8이은 CVS 사
용자 udong ID로 로그인한 후 checkout해 파일을 받아 실제로 main.c 파일에 주석 이
추가된 것을 확인한 예다.
廢) root@os：/temp_______________ ___

(흐

[root
os temp]# cus -d :pseruer:udong@203.237.229.121:24fl1
/home/cus login
Logging in to :pseruer:udong@203.237'
5T4
i:2401/hone/cus

.友 ‘⑦
》

CUS password:______________________________________________________________
[root@os temp]tt cus -d :pseruer:udong@2"d5'.'
5'7r.229.121:2401
/hone/cus co diary
cus seruer: Updating diary
U diary/Makefile
U diary/calendar.c
U diary/diary.h
U diarji/main .c
U diar
memo.c
[root@os tenp]#
[root@os temp]tt cat diar^/main.c
^include ‘‘digry.h"

으/

어:丄주석추가 I
lint main() {
nemo();
calendar();
return 0;

root@os temp]tt

［그림 14—80］ udong 계정으로 로그인 후 checkout한 예

수정된 여러 파일에 대해 한꺼번에 반영하고 싶다면 디렉토리에서 cvs commit 또는

cvs ci라고만 명 령을 내린다. 그러면 cvs commit 명령을 내린 디 렉토리 이하로 변경된
파일을 cvs 명령이 찾아 ［그림 14-81］ 과 같은 화면을 띄워준다.

［그림 14—81］ cvs ci 명령 후 결과 화면

718 6부—프로젝트버전 관리

===== PAGE 720 =====
위 그림은 diary.h 파일과 memo.c 파일을 수정한 후 cvs ci 명령을 내린 결과 화면이
다. vi 편집기가 실행된 모습인데, 여기에 수정된 내용에 대한 설명을 적어주고 ：wq! 명
령으로 저장한다. 그러면 ［그림 14-82］ 와 같이 diaryh 파일과 memo.c 파일의 변경된
부분이 CVS 서버에 각각 반영된다.

［그림 14-82］ 설명 추가 후 저장 결과

공동으로 작업을 진행할 경우 자신이 수정한 내용을 저장소 디렉토리에 반영하는 것도
알아야 되겠지만 다른 사람이 반영한 내용을 자신의 작업 디렉토리에 적용하는 법도
알아야 된다. 다른 사람이 수정한 내용을 현재 작업 디렉토리에 적용하려면 update 명
령을 사용한다

I update 명령을 사용해 현재 작업 디렉토리에 최신 소스 반영
지금 상황에서 장우동이 main.c 파일에 다음과 같이 주석을 추가하고 commit 명령을
내려 저장소 디렉토리의 main.c,v 파일에 반영했다.
〔예제 14너3〕 main.c 파일의 내용

#include
/*

"diary.h”

* 주석추가

*/
int main() {

:
；

memo () ;
calendar();

// 장우동 주석 추가

return 0;
}

14장_ Subversion, CVS 719

===== PAGE 721 =====
장우동이 반영한 최신 버전의 소스를 현재 작업 디렉토리에 있는 소스에 적용하려면
다음과 같은 명령을 내린다.
$ cvs update
또는

$ CVS up

［그림 14-83］ CVS up 명령으로 최신 버전 소스 적용

CVS up 명령을 내리면 위와 같이 변경된 파일이 표시되고 다음과 같이 장우동이 추가

한 내용이 들어있다.
/' root@server：/work/book/utils_new/svn/myproject/trunl(
int main() |
*mo();
calendar();

// 장우동 주석 추가

return 0;

B

_______________________________________________________ 10,1

바닥

［그림 14-84］ cvs up 명령 후 main.c 파일의 변화된 내용

Subversion 과 마찬가지로 CVS 역시 cvs up 명령을 자주 내려 항상 저장소 디렉토리
에 적용된 최신의 소스 파일을 자신의 작업 디렉토리에 적용시켜야 한다.

| 소스 충돌 해결
여러 사람이 작업을 하다 보니 소스 충돌이 생길 수 있는 가능성은 항상 있다.

Subversion 과 마찬가지로 두 사람이 같은 파일을 수정하고 commit했는데 수정한 부
분이 다르다면 CVS가 알아서 수정한 부분을 조합한다. 그렇지만 공교롭게도 같은 파일
의 같은 부분을 수정했다면 소스 충돌이 발생한다. 소스 충돌이 발생하면 CVS는 소스
충돌이 어떤 파일에서 발생했는지 개발자에게 알리고 개발자가 결정하게 한다.
［그림 14-85］ 는 CVS에서 소스 충돌이 났을 때 발생하는 메시지다.

720 6부_ 프로젝트 버전 관리

===== PAGE 722 =====
i [screen 1 ： bash] root@os：/temp/book/project/diary
[ rootSos diarjj ] ft | 헤〒페
cus seruer: UpdatTrig™™
RCS file: /home/cus/diary/nain.c,u
retrieving reuision 1.6
retrieuing revision 1.8_________________________________
Mergljig~~diTFereliices~^eTw^ME^^
rcsmerge: warning: conflicts during merge
cus seruqr:
conflicts Found in main.c
구.;■■히
[root@os diary]tt |

［그림 14-85］ 충돌이 발생했다는 메시지

출력되는 문자열 중 제일 하단의 main.c 문자 앞에 C는 main.c 파일이 충돌했다는 의
미다. 그래서 main.c 파일을 열어보면 ［그림 14-86］ 과 같이 충돌이 발생한 부분을 CVS
가 표시해 놓은 부분을 발견할 수 있다.

위 그림에서 표시된 부분이 바로 충돌이 발생한 부분이다. 이제 김삿갓이 할 일은 어떤
코드를 사용할지 선택하는 일이다. 자신의 코드를 포기할 것인지 아니면 장우동과 상의
해 자신의 코드로 밀고 나갈 것인지 결정을 하면 된다. 어떤 코드를 선택하든지 김삿갓
은 선택한 코드는 남기고, 선택하지 않은 코드는 지우고 main.c 파일을 저장한다. 그리
고 새롭게 적용된 내용을 CVS 서버에 반영하기 위해 cvs ci 명령을 내리면 소스 충돌
상황은 종료된다.

I add와 remove를 이용한 파일과 디렉토리 추가 및 삭제
파일이나 디렉토리를 추가할 때는 add 명령을 사용하고, 제거할 때는 remove 명령을
사용한다.
$ cvs add newfile. c

14장_ Subversion, CVS

===== PAGE 723 =====
위 명령을 내리고 CVS ci 명령을 내리면 CVS 서버에 newfile.c 파일이 추가된다. CVS
역시 add 명령 후 저장소에 반영하려면 반드시 commit을 해 주어야 한다.
關 [screen 1: bash] root@os：/temp/book/'project/diary
_스!마씌
=_________
- --=.-.-丄=====—--；"'1『---------

[root@os diary]tt|cus add newfile.c |
cus seruer: scheduling File’'newfile.c‘ For addition
cus seruer: use 'cus commit' to add this file permanently
[rootBos diary]tt
[rootSos diary]tt|'c
f'—n'"newfile.c
cus conmit: Examining .
RCS file: /hone/cus/diary/newfile.c,u
done
Checking in newFile.c;
/home/cus/diary/newFile.c,u <-- newfile.c
initial revision: 1.1
done
[root@Q5 diary]it |

（正 허

퐈일 추가'“I

버

［그림 14—87］ newfile.c 파일을 추가시킨 예

디렉토리를 추가시키는 예도 파일을 추가시키는 방법과 동일하다. CVS add ［디렉토리
명］ 명령을 내리고 cvs ci 명령을 내리면 저장소 디렉토리에 디렉토리가 생성된다. 이
렇게 생성한 파일과 디렉토리는 다른 개발자가 cvs update 명령을 내리면 해당 개발자
의 작업 디렉토리에도 생긴다.

CVS를 사용함에 있어서 디렉토리 트리를 추가시켜는 일은 매우 번거로울 수도 있다.
CVS는 디렉토리를 버전 관리 대상에 포함하지 않아 디렉토리 트리를 추가시키기 위한
별도의 명령을 지원하지 않기 때문이다.
예를 들면 ［그림 14-88］ 과 같이 newdir 디렉토리를 현재의 작업 디렉토리에 추가하고

newdir 디렉토리 이하에 있는 모든 파일들을 추가시키고자 한다면 일일이 cvs add 명
령과 cvs ci 명령을 각 파일과 디렉토리에 내려야 한다.

［그림 14-88］ 새롭게 추가한 newdir 디렉토리 트리 구조

722 6부_ 프로젝트 버전 관리

===== PAGE 724 =====
위 그림에서 볼 수 있듯이 새롭게 추가하려는 디렉토리 newdir 디렉토리는 내부에

filel.c, file2.c, file3.c 파일과 newdir2, newdir3 디 렉토리를 가지고 있고, 각 디 렉토리
에는 또 자신의 파일들을 가지고 있다.

CVS는 이렇게 디렉토리 트리를 추가하는 명령을 지원하지 않는다. 그래서 개발자들은
각자 디 렉토리 트리를 추가하는 스크립트를 직접 만들어 사용한다. 다음은 필자가 사용
하는 스크립트 파일이다.
〔예제 14-14]

#!/usr/bin/python
# vi: set ts=4 sts=4 sw=4: #
import os
import sys
import getopt
import glob
def read_dir (args, dirname, filenames) :
if not dirname.endswith("CVS") :
if dirname. endswith (’’/”) :
dirname = dirname[0:dirname.rindex("/")]
os.system("cvs add ’’ + dirname)
for f in filenames:
if os .path. isfile (dirname+’,/"+f) :
os.system("cvs add " + dirname + ”/” + f)
########### main start 파##########
if len(sys.argv) > 1:
options, args = getopt.getopt(sys.argv[1:], "t:”)
for op, var in options:
if op == ”-t":
os.path.walk(var, read_dirz [])
os. system (”cvs ci -m \"디렉토리 추가\"")

위 스크립트를 /usr/local/cvsadd.py 이름으로 작성하고 chmod 755 /usr/local/

cvsadd.py 명령으로 실행 권한을 준다. 그리고 newdir 디렉토리의 상위 디렉토리에서
다음과 같이 명령을 내리면 newdir 디렉토리 이하 모든 파일과 디렉토리가 CVS 서버
에 추가된다.
$ cvsadd.py -t newdir

14장_ Subversion, CVS 723

===== PAGE 725 =====
'I [screen 1： bash] root@os：/temp/book/project/diary

_싀믜싀

RCS file: /home/cus/diary/newdir/newdir2/file6.c,u
done
Checking in newdir/newdir2/File6.c;
/home/cus/diary/newdir/newdir2/f:ile6 .c ,u <-- file6.c
initial reuision: 1.1
done
RCS File: /hone/cvs/diary/newdir/newdir2/file7.c,u
done
Checking in newdir/newdir2/File7.c;
/home/cus/diary/newdir/newdir2/File7.c,u <-- File7.c
initial revision: 1.1
done
RCS file: /tiouie/cus/diary/newdir/newdir3/Fi.le8.c,u
done
Checking in newdir/newdir3/file8.-c;
/hone/ws/diar*y/newdir/newdir3/file8.c,u <-- FileS.c
initial revision: 1.1
done
RCS file: /hone/cus/diary/newdir/newdirS/File?.c,u
done
Checking in newdir/newdir3/File9.c;
/home/cus/diary/newd:ir/nevjdir3/file9.c,u <-- File9.c
initial revision: 1.1
done
[rootfios diar
y|

아]

［그림 14-89］ cvsadd.py 명령으로 디렉토리 트리 추가

파일이나 디렉토리를 추가하는 방법을 알았으면 필요 없는 파일이나 디렉토리를 제거
하는 방법도 알아야 할 것이다. 디렉토리 제거는 조금 애매한 문제가 있으므로 맨 마지
막에 다루고 먼저 파일을 제거하는 방법은 다음과 같다.
$ rm -rf newfile. c
$ cvs remove newfile. c
$ cvs ci -m "newfile.c 파일 제거,,

먼저 rm 명 령으로 파일을 지운다. 그리고 cvs remove ［파일명］ 명령을 수행하고 마지
막으로 cvs ci 명령을 내리면 저장소 디렉토리의 파일이 제거된다.

'디 [screen I： bash] ro미@os：/temp/book/project/diary
흐

[rootl
os diary]tt rm -rf newfile.c
[root@os diary]tt cus remoue newfile
cus seruer: scheduling *newfile.c' For remoual
cus seruer: use ‘cus commit1 to remoue this file permanent!
iy
"cus ci —m "newFile.c
[root@os
cus commit: Examining .
commit:
Examining
newdir
cus
newdir/newdir2
cus commit: Examining
newdir/newdirS
cus comnit: Examining
Remouing newFile.c;
/hoine/cus/diary/newFile.c,u <-- newFile.c
new t-euision: delete; preuious reuision: 1.1
done
［ rootBos

파일 저

브른뽜흐

［그림 14-9이 newfile.c 파일 제거

724 6부—프로젝트버전 관리

===== PAGE 726 =====
CVS add 명령으로 파일을 생성할 때 한 가지 주의 사항이 있다. CVS는 기본적으로 텍

스트 파일을 위주로 동작하게 되어 있다. CVS는 파일들을 텍스트 형식으로 인식해 파
일의 변화에 대해 변경된 부분만 저장하게 설계되어 있다. 즉, CVS는 기본적으로 아무
옵션도 주지 않으면 모든 파일을 텍스트 형식으로 인식하기 시작한다. 그리고 CVS는
각 운영체제에 따라 다르게 표현되는 개행 문자를 인식해 운영체제마다 변환을 한다.
예를 들면 리눅스 컴퓨터에 CVS 서버가 설치되어 있고, 윈도우즈 컴퓨터에서 CVS 클
라이언트를 사용해 리눅스 컴퓨터에서 프로젝트 파일을 받아오는 상황이 있다.
리눅스에서는 개행 문자로 山을 사용하고 윈도우즈에서는 \r\n 을 사용한다. 그러면

CVS 는 리눅스 서버에 있는 프로젝트 파일 내부에 사용된 \n 을 \r\n으로 변환해 원도
우즈 컴퓨터에 전달한다.
이런 일은 일반적인 텍스트 파일일 경우에는 아무런 문제가 되지 않는다. 그러나 바이
너리 파일일 경우에 문제가 발생한다.
예를 들면 리눅스 CVS 서버에 라이브러리 파일 libdiary.a 나 이미지 파일 image jpg 가
있을 때 이들 파일을 윈도우즈 클라이언트가 받으면 바이너리 파일 내부에 있는 山이
모두 \r\n으로 변경되어 정상적인 바이너리 파일이 아니게 되는 문제가 발생한다. 그래
서 바이너리 파일을 추가할 경우에는 애초에 add 명령을 내릴 때 -kb 옵션을 같이 사
용해 바이너리 파일이라는 걸 CVS 에 알려야 한다.
$ cvs add -kb image.jpg

다른 주의 사항으로 디렉토리를 지우는 경우가 있다. CVS 저장소에 있는 디렉토리를
지우는 방법은 cvs remove [디 렉토리명 ] && cvs commit 명 령으로 되지 않는다.

cvs remove 명령을 내리면 단지 cvs up 명령에 의해 디렉토리가 생성되지 않을 뿐이
다. 새로운 개발자가 개발에 참여해 checkout 하면 cvs remove 명령을 사용해 지운
디렉토리가 그대로 받아진다.
저장소 디렉토리에 있는 디렉토리를 완전히 지우기 위한 유일한 방법은 직접 rm 명령
으로 저장소 디렉토리에서 지우려는 디렉토리를 지우는 방법밖에 없다.

14장_ Subversion, CVS 725

===== PAGE 727 =====
I 파일이전 버전으로 돌리기
소스를 수정하고 commit했는데 마음에 안 들어 이전 버전으로 되돌리고 싶을 때가 있
을 것이다. 예를 들어 다음과 같은 main.c 파일이 있는데, 주석이 마음에 들지 않아 주
석을 모두 지워 버 렸다고 가정하자.
〔예제 14-15）

main.c 파일의 내용（버전 1.12）

#include "diary.h"
/*
* 주석 추가
*/

int main() {
memo();
calendar ();
return

//장우동 주석 추가
//김삿갓 주석 추가

0;

}

막상 지우고 나니 허전해 다시 넣고 싶은 생각이 든다. 이럴 때는 다음과 같은 방식으
로 간단하게 이전 버전으로 되돌릴 수 있다. 먼저 cvs status main.c 명령으로 main.c
파일의 현재 버전을 파악한다.
$ cvs status main.c

廳 [screen 1： bash] root@os:/temp/book/project/diary
(흐os diary]tt cus status main.c

[root

File: main.c

Status: Up-to-date

Uorking revision:
1.13
Repository
reuision: 1.13 /home/cus/diary/main.c fu
Sticky Tag:
(none)
(none)
Sticky Date:
Sticky Options:
(none)
[rootQos diary]tt |

[그림 14-91] cvs status main.c 명령으로 본 main.c 파일의 현재 버전

위 그림과 같이 주석을 제거한 현재 main.c 파일의 버전은 1.13이라는 것을 알 수 있다.
그러면 주석이 달려있는 버전은 1.12였을 것이다.
다음 명령을 내리면 주석이 달려있는 1.12 버전의 main.c 파일로 되돌아간다.
$ cvs up -r 1.12 -p main.c > main.c

726

6부—프로젝트버전 관리

===== PAGE 728 =====
［그림 14-92］ 주석이 달려있는 1.12 버전으로 되돌린 예

현재의 상황과 같이 바로 전 버전뿐만 아니라 이전의 다른 어떤 버전이더라도 cvs up

-r ［버전］ -p ［파일명］〉［파일명］ 명령을 내리면 이전 버전의 내용으로 돌아갈 수 있다.
간혹 롤백 (rollback)을 하고 롤백한 파일을 수정한 후 commit할 때 ［그림 14-93］ 과
같은 메시지가 출력되면서 commit이 되지 않는 경우가 발생할 수 있다.
i [screen 1 ： bashl root@os:/temp/book/project/diary

느

표回씌

[rootAos 'digry]tt cus c:
-n "nain.c rollback" main.c
cus seruer:[stickynEag]'1.2' for File 'nain.c' is not a branch
cus [seruer aborted]: correct aboue errors First?
[rootQos diary]tt |

[그림 14—93] sticky tag 문제

위 예제는 필자가 cvs up -r 1.2 main.c 명령으로 main.c 파일을 1.2 버전으로 변경한
후 변경된 main.c 파일을 수정하고 cvs ci 명령을 내렸을 때 출력되는 결과 메시지다.
이런 메시지가 출력되는 이유는 main.c 파일에 스티키 태그(sticky tag)가 있어 발생하
는 메시지다.
스티키 태그는 이전 버전으로 되돌린다거나 할 때 자동으로 들어가는데, 스티키 태그가
들어가는 이유는 다음과 같다. 필자가 main.c 파일을 1.2 버전으로 바꾸고 commit이
가능하다면 현재 저장소 디렉토리에 있는 main.c 파일은 훨씬 이전 버전인 1.2 버전으
로 바뀐다.

14장_ S니bversion, CVS 727

===== PAGE 729 =====
이런 일을 미연에 방기하고자 CVS는 cvs up -r 1.2 main.c 명령으로 main.c 파일을

1.2 버전으로 되돌릴 때 항상 스티키 태그를 집어넣는 것이다. 스티키 태그의 존재 유
무는 cvs status ［파일명］으로 확인 가능하다. 스티키 태그를 제거하려면 다음 명령을
내린다.
$ cvs up -A main.c

위 명령을 내리면 main.c 파일의 스티키 태그가 제거된다. 그러면 commit 명령이 정
상적으로 동작한다.

| 파일 로그 및 특정 부분을 수정한 사람 확인하기
로그를 확인하는 명 령은 다음과 같다.
$ CVS log ［파일명］

다음은 필자가 진행 중인 프로젝트 파일의 로그를 CVS log 명 령으로 본 예다.

'기 [screen 1 ： bash] root@os：~/os/uSYS
reuision 1.45
date: 2004/08/18 11:12:36; author: bckddn; state: Exp;
lines: +5 -5; kopt: ku; commitid: eF84123399F0080;
sdsds
reuision 1.44
date: 2004/08/10 06:12:26; author: broid; state: Exp; 1
ines: +6 -1; kopt: ku; commitid: cac411867418000;
- warning

제거

reuision 1.43
date: 2004/08/10 01:89:57; author: bckddn; state: Exp;
lines: +4 -3； kopt: ku; comnitid： 3d84118205b8000;
free

관련 부분 주석 해제

reuision 1.42
date: 2004/08/06 15:48:34; author: bckddn; state: Exp;
lines: +79 -11; kopt: ku; commitid: d244113a63foWO;

루틴 추가
변겅
관련 파일 추가

Rate Monotonic test
kernel timer
ipc

reuision 1.41
date: 2004/08/01 21:55:21; author: bckddn; state: Exp;
lines: +3 -2; kopt: ku; commitid: F3841Od66b20000;

［그림 14-94］ cvs log ［파일명］ 명령으로 본 로그

로그를 자세히 보면 누가 언제 수정했는지에 대한 정보가 있음을 알 수 있다. 로그를
확인해 보면 새로운 부분을 추가한 개발자가 남긴 글을 읽을 수 있을 것이다.

728 6부_ 프로젝트버전 관리

===== PAGE 730 =====
로그를 보면 가장 최근에 누가 수정했는지와 파일에 어떤 내용이 추가되었는지에 대한
정보는 알 수 있지만 특정한 부분을 누가 수정했는지는 알 수 없다. 특정 부분을 누가
수정 했는지 알아보고자 한다면 다음과 같은 명 령을 사용한다.
$

cvs

annotate

［파일명］

또는

$ cvs arm ［파일명］

위 명령으로 필자가 작업하던 파일을 보면 다음과 같은 결과가 출력되는 것을 알 수 있다.
1: bash］
1.1
1.1
1.25
1.25
1 .40
1.25
1.25
1.28
1.42
1.42
1.42
1.10
1.14
1.6
1 .12
1.5
1.12
1.12
1.1
1.1
1.11
1..................
1.25
1.20
1.25
1.35
1 .40
-2

(palangse 28-tiay-04):
(palangse 28—May—04):
(bckddn 16-JU1-84):
(bckddn 16-Jul-84):
(bckddn 31-Jul—84):
(bckddn 16-Jul-84):
(bckddn
16—Jul-04):
(bckddn 17-Jul—84):
(bckddn 06—Aug—04):
(bckddn 06—Aug-04):
(bckddn 06—Aug-04):
(bckddn 83—Jun-04):
(broid
24—Jun-64):
(bckddn 01-Jun—04);
(bckddn 22—Jun—04):
(bckddn 01-Jun—84):
(bckddn 22-Jun-84):
(bckddn 22—Jun—04):
(palangse 28—May-84):
(palangse 28—May—04):
(bckddn
28—Jun-84):

*/
uoid init_task(uoid);
int task0(uoid);
int task4(uoid);
int taskl(uoid);
int task2(uoid);
int task3(void);
int rntaskl(void);
int rmtask2(uoid);
int rmtask3(uoid);
int mshell(uoid);
uoid test led deuice(uoid);
uoid delay(int tine);
uoid init_tiner(void);

int main(uoid)

(bckddn 16—Jul—84):
(bckddn 01-Jul-84):
(bckddn 16-Jul-84):
(broid
28-Jul—84):
(bckddn 31-Jul-04):

("허다#n", "Startini

printf

uSVS kernel

init_deu();
NandFlash_Init();
init_nem();
init_Fs();
init_ipc();

Bi

［그림 14-95］ cvs annotate ［파일명］ 명령 사용

위 그림과 같이 CVS annotate 명령을 사용하면 각 행에 대해 누가 언제 수정을 했는지
자세한 정보가 보인다.

I 파일 버전대별 차이점 확인
버전대별 달라진 점을 확인하려면 diff 명령을 사용한다.
$ cvs diff -r 1.5 -r 1.6 main.c

위 명령을 내리면 1.5 버전의 main.c 파일과 1.6 버전의 main.c 파일에서 달라진 부분
이 있는지 출력한다.

14장_ S니bversion, CVS :: 729

===== PAGE 731 =====
[그림 14-96] cvs diff 명령 사용

cvs diff 명령으로 main.c 파일의 1.5 버전과 1.6 버전을 비교해 보니 1.5 버전에서는 행
주석이 있었는데 비해 1.6 버전에서는 행 주석이 제거되었다는 것을 확인할 수 있다.
그리고 다음과 같이 명령을 내리면 저장소 디렉토리에 있는 가장 최신 버전의 main.c
와 현재 작업 디 렉토리에 있는 main.c 파일을 비교해 다른 부분을 출력한다.
$ cvs diff -r HEAD main.c
關 [screen 1： bash] root@os：/tgmp/book/project/<llary

(흐

[root
os diary]tt|cus"diFf -r HEAD main.c |
Index: main.c
======= = =0
RCS file: /home/cus/diary/inain.c,u
retrieving revision 1.17
diff -ri.17 main.c
8a9,10
>
printf("hello, world?tfn,•);
>
[root
os diary]tt |

(흐

【그림 14-97] cvs diff 명령 사용

cvs diff -r HEAD main.c 명령을 내리니 필자가 방금 추가한 printf 함수가 출력되는
것을 확인할 수 있다.

-r 옵션 뒤에 오는 HEAD는 Subversion과 마찬가지로 CVS에서 예약된 태그로, 저장
소 디렉토리에 있는 가장 최신 버전을 의미한다. HEAD와 같이 CVS에서 이미 예약된
태그로 BASE가 있는데, BASE는 현재 작업 디 렉토리의 main.c 버전을 의미한다.

730

6부—프로젝트버전 관리

===== PAGE 732 =====
I 현재 시점의 소스 태깅하기
현재 소스 파일들의 버전이 각각 위와 같을 때 다음 명령을 내리면 현재 상태를 TAG_1
태그에 표시한다. Subversion은 저장소를 복사해 태깅 했는데 반해 CVS는 이 렇게 태그
를 생성하는 것이 다른 점이다.
$ CVS tag TAG_1
I [screen I： bash] root@os：/temp/book/pmject/diary
[root@os diary] It feus £ag
cus seruer: Tagging .
T Makefile
T calendar.c
T diary.h
T main.c
T memo.c
[rootQos diary]tt |

［그림 14-98］ evs tag 명령으로 태그를 건 모습

이렇게 태그를 걸어 놓았으면 나중에 언제든지 태그를 건 시점으로 돌아갈 수 있다.
$ CVS up -r TAG_1

［그림 14-99］ 는 evs tag TAG_1 명령으로 TAG_1 태그를 걸어놓고 diary.h main.c,

memo.c 파일을 수정한 후 위 명령을 내려 파일들을 수정하기 이전의 TAG_1 태그를
건 시점으로 돌아가는 예를 보여준다.
H [screen 1： bash] root@os:/temp/book/project/diary
[root@os diarp ]
711r

히三｝ ‘즈‘““而"' "주‘히으후]

cus seruer: Updating .
P diary.h
P main.c
U memo.c
[root@os diary]tt |

［그림 14-99］ TAGJ 태그를 건 시점으로 돌아간 예

태그를 거는 명령에는 tag 명령 외에도 rtag 명령이 더 있다. tag 명령과 rtag 명령의 차
이점은, tag 명령은 현재 작업 디렉토리에 태그를 거는 것이고 rtag 명령은 저장소 디렉
토리에 태그를 걸기 때문에 좀 더 광범위하다는 점이다.
이 점을 유념하면서 tag를 사용하면 좀 더 편리하고 안전하게 CVS를 사용해 프로젝트
수행을 할 수 있을 것이다.

14장_ Subversion, CVS

731

===== PAGE 733 =====
I 브랜치하기
CVS에서의 브랜치는 다음과 같이 rtag 명령을 사용한다.
$ cvs rtag -b BRANCH_2_1 diary

위 명령을 내리면 현재 저장소 디렉토리에 있는 diary 모듈의 현재 상태에

BRANCH_2_1 이라는 브랜치 태그를 붙인다. 브랜치 태그명은 알기 쉽게 지정하면 어떤
것이라도 상관없다.
H [screen 1: bash] root@os：/temp/book/project/diary

히

드

[rooteos diary]
cug rtag ~b BRANCH_X
cus rtag: Tagging diary
[root
os diary]tt
iroot@os diary]tt |

（흐

［그림 14-100］ 브랜치 예

브랜치 태그를 붙였으면 브랜치 태그를 지정해 checkout해야 새로운 가지에서 프로젝
트를 진행할 수 있다. 다음과 같은 명령을 사용해 생성한 브랜치 태그에서 새로운 가지
가 나오게 한다.
$ cvs co -r BRANCH_2_1 -d diary_BR2.1 diary

위 명령에서 -d diary_BR2.1 옵션은 checkout해 생성할 디렉토리를 diary_BR2.1 로
지정하는 옵션이다. 위 명령을 내리면 ［그림 14-101］ 과 같이 diary_BR2.1 디렉토리가
생성되고 새로운 가지의 소스들이 들어간다.

즈os：/temp/book/project
厂]—厂
히 cus co —r BRANCH』끄2l~：'；""}iary BR2.1 dia헤

] [screen 1 ： bash] root
[root@os project]

’■y
cus seruer: Updating diary_BR2.1
U diary_BR2.1/Makefile
U diary_BR2.1/calendar.c
U diary_BR2.1/diary.h
U diai*y_BR2.1/main .c
U diary_BR2.1/memo
[root@os project]tt|Is diarp_BR27iZ|
CUS MakeFile calendar.c diary.h main.c memo.c
[root@os project]!! |

［그림 14-101］ 브랜치 태그를 지정해 checkout

I

이렇게 브랜치한 소스를 수정하고 commit하면 메인 버전에는 아무런 영향을 미치지
않고 오직 브랜치한 버전에만 적용된다. ［그림 14-102］ 는 필자가 diary.h 파일을 수정
하고 commit했을 때 출력되는 메시지를 보여준다. diary.h의 버전이 1.2에서 1.3으로
바뀌지 않고 1.2.2.1로 바뀌는 것을 확인할 수 있다.

732 6부_ 프로젝트버전 관리

===== PAGE 734 =====
[g| [screen 1： bash] root@os：/temp/book7project/diary_BR2.1

"소스 수정,, diary.h
으.
근
프흐고즈흐흐표표上흐표효히제히

[rootSos diary_BR2.1]# cus ci -m
Checking in diar
h;
/home/cvs/diary/diarjj.hTu .di
ry.h
new revision: [j
done
[rootBos diary_BR2.1]# |

[그림 14너02] 브랜치한 버전 소스 수정 후 commit을 수행한 예

I 브랜치한 소스 머지하기
CVS에서 머지하는 방법은 다음과 같다. 먼저 브랜치한 버전의 소스 코드를 정리하고
commit한다. 그리고 메인 버전의 작업 디렉토리에서 다음 명령을 내리면 머지한다.
$ cvs up -j BRANCH_2_1

-j 옵션 뒤에 오는 BRANCH_2_1 은 브랜치할 때 달아준 태그 이름이다. 위 명령을 메인
버전의 작업 디렉토리에서 내리면 다음과 같은 메시지가 출력되면서 머지한다.
I [screen 1： bash] root@os：/temp/book/project/diary
[rootQos diary]
TJ“'
gyjqgp

효•후두" 司

으;으^^"

厂下一厂

cus seruer: Updating \
RCS file: /hone/cus/diary/diary.h,u
retrieving reuision 1.1
retrieuing reuision 1.2.2.1
Merging differences between 1.1 and 1.2.2.1 into diary.h
RCS file: /home/cus/diary/main.c,u
retrieuing reuision 1.16
retrieving reuision 1.21.2.1
Merging differences between 1.16 and 1.21.2.1 into inain.c R
RCS file: /home/cus/diary/nemo.c,u
retrieuing revision 1.4
retrieuing reuision 1.5
Merging differences between 1.4 and 1.5 into memo.c
[rootBos diary]ft

:三

스.:
>
/

〔

흐흐
느;;
:

테

[그림 14-103] 브랜치 버전을 머지한 예

브랜치 버전을 머지할 때는 출력되는 메시지를 유심히 보아야 한다. 서로 다르게 개발
이 진행되었으므로 소스 충돌이 많이 발생하기 때문이다. 이상이 브랜치한 버전을 메인
버전에 머지하는 예였다.
지금까지의 내용만.0-루두 CVS를 사용하는 데 아무런 어려움이 없을 거라고 생각한다.

CVS의 나머지 부분은 이제 독자의 몫이다. 좀 더 고급 사용법은 직접 찾아 하나씩 익혀
나가기 바란다.

14장_ Subversion, CVS 733

===== PAGE 735 =====


===== PAGE 736 =====
부록 A
프로그래밍 유형별
가용 유틸리티

01 GUI 프로그래밍
02 네트워크프로그래밍

===== PAGE 737 =====
I••⑵甘3 S-tcjidy
지금까지의 모든 과정을 통해 독자들은 리눅스, 유닉스 시스템에 있어서 표준적인 개발
방법을 익힐 수 있었을 것이다. 이번 장은 지금까지 배운 표준적인 개발 방법에서 좀 더
세분화된 프로그래밍 종류별로 사용하면 편리한 유틸리티를 설명하고자 한다.

===== PAGE 738 =====
L GUI 프로그래밍
리눅스, 유닉스 시스템에서 GUI를 사용하는 가장 보편적인 방법은 바로 X-Windows
시스템을 이용하는 방법이다. X-Windows 시스템을 이용한 GUI 구현에 있어 가장 원
초적 방법은 XLib를 이용하는 방법이다. 그렇지만 XLib를 직접 이용해 GUI를 구현하
는 방법은 XLib 자체에서 지원하는 기능이 미약하기 때문에 많이 사용되지 않는다.
거의 대부분의 X-Windows 프로그래밍은 XLib를 기반으로 한 QT 라이브러리나 GTK
라이브러리를 이용해 GUI를 구현한다. 그러면 X-Windows 시스템에서 GUI를 구현하
기 위 해 기본적으로 알아야 되는 X-Windows의 구조와 특성을 알아보자.

O X-Windows 프로그래밍의 이해
X-Client

[그림 A-1] X-Widows 구조

［그림 A-1］ 은 X-Windows 시스템을 매우 간단하게 보여준다. X-Windows는 위 그림
과 같이 핵심이 되는 x 서버가 중앙에 있고 X 클라이언트가 X 서버와 통신하는 형태다.

X 서버의 주요 역할은 X 클라이언트의 명령을 받아 화면에 그림을 그리는 일과 키보드
입력 등이 일어났을 때 이벤트를 X 클라이언트에게 전달해 주는 일이다.

X 클라이언트는 일반적으로 생각하는 X-Windows 애플리케이션이라고 볼 수 있다.
X 클라이 언트는 XLib라는 X-Windows 시스템의 가장 근본적 인 라이브러 리를 사용
해 X 서버와 통신한다.

프로그래밍 유형별 가용 유틸리티

===== PAGE 739 =====
XLib는 X 서버에게 점이나 선 또는 도형을 그리라는 명령과 색깔을 칠하라는 등의 명
령을 전달하는 역할을 수행한다. 그렇기 때문에 XLib만 가지고 GUI 프로그래밍을 하
는 일은 매우 시간이 많이 걸리는 작업이고, 또한 완성된 프로그램에 대한 품질을 보장
하지 못한다（일일이 선을 그어 화면을 구성한다고 생각해 보라）.
이런 XLib의 단순한 기능들을 이용해 미리 만들어진 컴퍼넌트를 제공하는 라이브러리
가 바로 QT와 GTK다. QT와 GTK는 단순히 부록 몇 페이지를 할당해 설명할 수 있을
만큼 간단한 라이브러리가 아니다. QT와 GTK를 설명하기 위한 책이 여러 권 나와 있
을 정도로 QT와 GTK는 매우 방대한 라이브러리다.
필자가 여기서 QT 와 GTK 를 설명하는 것은 이 책의 의도와 맞지 않다. 필자는 단지

QT와 GTK에서 제공하는 GUI 에디터인 QT 디자이너와 glade* 소개하려 한다.

I QT 디자이너를 사용한 간단한 G니 애플리케이션 만들기
QT 디자이너의 사용법을 설명하기 전에 먼저 QT 라이브리리를 간단하게 설명한다.
QT 라이브러리는 TrollTech에서 만든 라이브러리로, KDE 환경에서 동작하는 애플리
케이션을 작성하기 위한 그래픽 AH를 묶어놓은 라이브러리다.

QT는 C++로 작성됐고 클래스가 잘 정의되었으므로 배우기 쉽다. 그리고 유려한 인터
페이스를 제공하고 여러 플랫폼에 포팅되었기 때문에 많이 사용되는 그래픽 라이브러
리다.
이의 단점 이 라면 먼저 라이선스를 들 수 있다. QT의 라이선스는 완전한 GPL이 아니다.

QT의 라이선스는 오픈 소스에 관해서는 무료지만 오픈 소스가 아닌 소프트웨어를 작
성하는 데는 비용을 받는 라이선스다. 이런 QT 라이선스 정책으로 인해 어떤 사람들
은 QT보다 GTK를 선호하곤 한다. 그 외 단점이라면 GTK보다 느리다는 점이다. 필자
가 경험한 바에 의하면 일반적인 데스크톱 컴퓨터에서 QT가 GTK보다 느리다는 느낌
은 거의 없다. 하지만 임베디드 시스템과 같이 하드웨어 성능이 떨어지는 시스템에서는

QT가 GTK보다 확실히 느리다.
이런 단점에도 불구하고 QT는 KDE 환경을 구성하는 근본적인 그래픽 API이기 때문
에 배워두면 여러모로 쓸모가 많다. 그러면 QT 디자이너라는 유틸리티를 이용해 어떻
게 하면 간단하게 GUI 애플리케이션을 작성할 수 있는지 알아보자.

738 부록 A

===== PAGE 740 =====
o QT 디자이너 실행
X-Windows 터미널에서 designer라고 입력하면 ［그림 A-2］ 와 같이 QT 디자이너가
실행된다.

【그림 A-2］ QT 디자이너 실행 모습

그림처럼 정상적으로 QT 디자이너가 실행되지 않는다면 QT 디자이너가 제대로 설치
되지 않은 경우이므로 http://www.trolltech.com 사이트에서 QT 디자이너를 받아 설
치하기 바란다.

@ 프로젝트 파일 생성

QT 디자이너가 실행되었으면 아래와 같은 대화상자가 보일 것이다. 그러면 대화상자
에서 C++ Project 메뉴를 선택한다.

[그림 A-3] C++ Project 선택

프로그래밍 유형별 가용 유틸리티 739

===== PAGE 741 =====
대화상자가 보이지 않을 경우 ［파일］ 메뉴에서 ［ New］ 메뉴를 선택하면 나타난다. C++

Project 메뉴를 선택하면 프로젝트 파일 이름을 결정하는 대화상자가 다시 ［그림 A-4］
와 같이 나타난다. 그러면 Project File 부분에 앞으로 사용할 프로젝트 파일명을 적어
준다.

［그림 A-4］ 프로젝트명 선택

필자는 ［그림 A-4］ 과 같이 프로젝트 파일명으로 qtgui.pro를 사용하였다.

@ Widget 생성
이제 qtgui 프로젝트에서 사용할 GUI를 구성하면 된다. 먼저 ［파일］ 메뉴에서 ［ New］
를 선택하면 다시 ［그림 A-5］ 와 같은 대화상자가 실행될 것이다.

［그림 A-5］ New 메뉴 선택

대화상자에서 앞으로 사용할 윈도우의 특성을 선택한다. 필자는 Widget을 선택했다.
독자들은 Main Windows나 Widget 중 아무거나 선택하면 된다.

740 부록 A

===== PAGE 742 =====
[그림 A-6] Widget을 선택한 후 모습

Widget을 선택하고 나면 위와 같이 Forml(@)이라는 에디팅을 할 수 있는 윈도우가
나타나는 것을 확인할 수 있다. 그러면 화면 좌측에 있는 Toolbox(©)에서 윈도우를
구성할 컴퍼넌트를 선택해 붙인다.
①의 Project Overview에는 프로젝트를 구성하는 윈도우를 보여준다. 그리고 ②의

Object Explorer에는 각 객체들이 어떻게 연결되어 있는지 보여준다. 마지막으로 가
장 유심히 보아야 될 Property Editor/Signal Handlers(③)에서는 각 객체의 속성을
설정할 수 있고, 이벤트가 발생했을 때 이벤트 핸들러를 설정할 수 있다.

E 윈도우 구성
그러면 Toolbox(©)에서 이것저것 선택해 Forml 윈도우에 붙여보자.

[그림 A-7] 버튼과 라벨을 붙인 모습

필자는 버튼을 세 개 붙이고 라벨도 같이 붙였다. 버튼에 표시되는 문자열과 라벨의 초
기 문자열은 버튼이나 라벨을 더블 클릭하거나 객체를 선택한 후 Property Editor 창
(③)에서 변경할 수 있다.

프로그래밍 유형별 가용 유틸리티 741

===== PAGE 743 =====
同 이벤트 핸들러 설정

화면을 구성했으면 버튼이 눌러졌을 때 동작을 설정해야 할 것이다. 먼저 버튼을 마우
스로 선택하고 Property Editor 창(③)에서 Signal Handlers 탭을 선택한다.

[그림 A-8] Signal Handlers 탭 선택

우리는 버튼이 클릭되었을 때 어떤 일을 해 주기를 바라기 때문에 리스트 중에서

clickedO를 더블 클릭한다. 그러면 clickedO 리스트 이하로 ［버튼명］ _clicked()라는
리스트가 하나 생성되는데, 버튼이 클릭되었을 때 수행할 함수명을 적어준다.
필자는 기본적으로 설정되는 pushButtonl_clicked를 함수명으로 사용한다.

［그림 A-9］ 에디터 창 생성

함수명을 선택하고 나면 ［그림 A-9］ 와 같은 에디터 창이 생성되는데, pushButtonl_

cHckedO 함수 부분에 버튼이 클릭되었을 때 어떤 일을 해 줄 것인지 C++ 소스로 작성
한다.

742 부록 A

===== PAGE 744 =====
필자는 버튼이 클릭되면 라벨 부분에 “Hello World” 문자열을 출력하고 싶어서 함수
부분을 ［예제 A-1］ 과 같이 작성하였다.
〔예제 A너) pushButtonl_clicked() 함수 내용

void Forml::pushButtonl_clicked()
{
textLabell->setText("Hello World");

:

}

서

［예제 A-1］ 에서 textLabell은 필자가 윈도우에 붙여 넣은 라벨의 이름이다. 독자가

Property Editor 창에서 라벨의 이름을 다른 것으로 변경 했다면 변경한 이름을 사용해
야한다.
이렇게 버튼이 클릭되었을 때 수행할 함수를 작성했으면 이제 모두 저장한다. ［파일］
메뉴에서 ［ Save All］ 메뉴를 선택하고 파일을 저장하면 저장한 디 렉토리에 다음과 같은
세 개의 파일이 생성됨을 확인할 수 있을 것이다.

［그림 A-10］ 생성된 파일 리스트

제대로 저장되지 않는다면 ［ Project］ 메뉴에서 ［ Project Settings...］ 메뉴를 선택한 후
［그림 A-11］ 과 같이 프로젝트 파일의 위치를 선택한 후 다시 저장하면 제대로 저장될
것이다.

［그림 A-11］ 프로젝트 파일의 위치 지정

생성되는 파일 중 확장자가 *.ui인 파일은 윈도우를 정의해 놓은 XML 파일이다. 그리고

*.ui.h 파일은 이전에 버튼이 클릭되었을 때 이벤트를 정의해 놓은 소스 파일이다. 마지
막으로 *.pro 파일은 전체 프로젝트를 규정짓는 프로젝트 파일이다.

프로그래밍 유형별 가용 유틸리티 743

===== PAGE 745 =====
® main.cpp 파일 생성
이렇게 세 개의 파일을 생성했으면 이제 main.cpp 파일을 생성해야 한다. main.cpp
파일은 main() 함수가 있는 파일로, 프로젝트를 이루는 윈도우가 여러 개일 때 프로그
램의 실행 시 화면에 나타낼 윈도우를 선택하는 파일이다.
[파일] 메뉴에서 [New] 메뉴를 선택해서 나오는 대화상자에서 [그림 A-12] 와 같이

main.cpp 아이콘을 더블클릭한다.

[그림 A너2] main.cpp 파일 생성

그러면 대화상자가 하나 뜨는데, 그곳에서 프로그램을 수행시켰을 때 기준이 되는 윈도
우를 선택한 후 [OK] 버튼을 누른다. 현재 우리가 만드는 간단한 애플리케이션은 윈도
우가 하나뿐이기 때문에 그냥 [OK] 버튼을 누르면 된다.
다시 [파일] 메뉴에서 [Save AU...] 메뉴를 선택해 main.cpp 파일을 저장한다. 그러면
프로젝트 파일이 있는 디렉토리에는 [그림 A-13] 과 같이 네 개의 파일이 생성되었을
것이다.

[그림 A-13] 최종적으로 생성된 파일 리스트

744 부록 A

===== PAGE 746 =====
Q Makefile 파일 생성
이제 프로젝트 파일이 있는 디렉토리에서 다음 명령을 내리면 Makefile이 생성된다.
qmake -o MakefLLe qtgui .pro

[그림 A너4] Makefile 생성

©컴파일

마지막으로 make 명령을 내리면 forml.ui 파일에서 C++ 소스 파일과 헤더 파일을
생성해 실행 파일(qtgui)을 컴파일한다.
M [screen 2： bash] mot@os：~/qt
oc/moc_Forni.cpp
g++ -o qtgui .obj/main.0 .obj/Fornl.0 .obj/moc_form1.0
-L/usr/lib/qt-3.1/lib -L/usr/X11R6/lib -Iqt-mt -IXext 1X11 -Im
[rootQos qt]tt Is qtgui
qtgui
[root@Q5 qt]ft I____________________________________________________

［그림 A너5］ 실행 파일 생성

0 실행
이렇게 실행 파일이 생성되었을 경우 X-Windows 터미널에서 실행 명령을 내리면
［그림 A-16］ 과 같이 우리가 만든 GUI 프로그램이 실행되는 것을 확인할 수 있다.

［그림 A-16］ qtgui 실행 모습

［그림 A-16］ 과 같이 실행되었으면 버튼을 클릭해 라벨 부분에 “Hello World” 문자열
이 출력되는 모습을 확인할 수 있다.

［그림 A너7］ 버튼 클릭 모습

프로그래밍 유형별 가용 유틸리티

745

===== PAGE 747 =====
이상이 QT 디자이너를 사용한 간단한 GUI 애플리케이션 제작의 예였다. 제대로 된

GUI 애플리케이션을 만들려면 지금 설명한 내용 외에도 많은 것을 알아야 된다. 자세
히 알고자 하는 독자는 QTi 관련된 서적을 참고하기 바란다.

I 이ad% 사용해 간단한 GUI 애플리케이션 만들기
지금까지 QT 디자이너를 사용해 GUI 애플리케이션을 만드는 방법을 알아보았다. QT
에서 GUI 에디터로 QT 디자이너가 있다면 GTK에서는 glade가 있다. 그러면 지금부
터 glade를 사용해 간단한 애플리케이션을 제작하는 방법을 알아보자.

QI glade 실행
X-Windows의 터미널에서 glade를 입력하면 다음과 같이 세 개의 창이 생성된다.
* r60t혀6호구7鑛 ‘
. [root@os /]# designer &
[1] 6970
[rootSos /]# X1 ib： ex-|
Xlib： extension "GLX" Il
[1 ]+ Done
[rootQos /]#
[rootQos /]# designer 으
[1] 7105
[root@os /]# XIib： ex*
iXlib： extension "GLX"
[rooteos /]#
[root@os /]#
[root@os /]#
i[root@os /]# Is
ini
lb'ih 뉴ev. home
| boot etc Images 116
；[root©os /]# cd /root/
： [root@os root]# Is
jDesktop
Makefile
projects

■*(3lade:<0|g£!8>

소 Kg：＜ 얹 8：

짜일© 현길© 브기⑵ 사정© 도♦« 언）

G

‘t

球
여 〉
얼기 저장 융연

s드

휴대:

©
mm proc st?in Tf•라
opt root temp tmp

②

추 선택자

gettime
gettime.c

3TK+ 기초
3TK+ 후가

interface.c
interface.h
kdevelop-3.0.4

anjuta-1.2.2
cal 1 backs. c
•call backs.h
counter.txt
I eel 1t〉se

[root®os root]# cd qt/ j
[root@os qt]# Is
Makefile forml .i』1 fori
[rootSos qt]# ./qtgui
Xlib： extension “GLX" |
XIib： extension "GLX"}
[rooteos qt]# glade

Ai처昏 廳
쯰Rj시
IS l투 s 備
_J CB LT 싀

kkk
maln.c^v

os

test3
test3.c
test3.1
test3.s
uSYS-1.pdf
uSYS-1.ps
upgrade.log.sysl og

； [효] 디 qkb-0.3.2
qt
끠 rooti.img
川그 主:d
.cpp qtgui qtgui.pro
- 3 JJ 봬

ZiQ JF

splay "：1.0".
jsplay "：1 .0".

I

[영어 ][완성 ][두벌식 ]

[그림 A너8] glade 실행 모습

생성되는 윈도우 중 = 메인 윈도우라 부르며, glade 의 전역적인 설정을 선택하는 윈
도우다. 그리고 ①을 팔레트라고 하는데, 각각의 컴퍼넌트들이 버튼 형식이므로 마우스
로 선택해 붙여 넣을 수 있다. 마지막으로 ②를 속성 에디터라고 하는데, 각 객체의 속
성을 설정할 수 있는 윈도우다.

746 부록 A

===== PAGE 748 =====
@ 윈도우 생성

이렇게 glade가 실행되었으면 화면을 구성할 윈도우를 생성해야 한
다. 먼저 팔레트에서 ［그림 A-19］ 와 같은 버튼을 클릭하면 윈도우가
생성된다.

쓰 I혀

■ i톨 a 庫
_J CB 〒 그

買］ 固 3 프］
山」느主호
三 6표췅厂
［그림 A-19］ 팔레트에서 윈도우 생성

윈도우 버튼을 클릭하면 ［그림 A-2이과 같이 화면에 새로운 윈도우가 뜰 것이다.
x Glade: •〈이§얹
곽잏® 편길（트） 보기（스）

설정（§） 도옴끌언）

O

<vinaowi

醉
여 쭌｝
열기 저장 ‘ 욥션 ' 빌드

GtkWindow

0"

으"! windowl

H두리 두째：
windowl

Top Lewi :
위치:

4 프로젝트 생'섬돔'

□ tin sc
F

opt root temp Tinp

A

gettime

추 선팈가

>

GTK+ 기료
cm〈+ 平가

씌

표존너비:

5 wlrglowl

None

모달'

아니오

rF

표귝‘높이:

흐、_B—

a

Gnome

i
目
=1
'

의

一

T
n =

PS

!.1og.syslog

JJJ
으 3
I n

［그림 A-20］ 윈도우 생성

프로그래밍 유형별 가용 유틸리티

747

===== PAGE 749 =====
이렇게 생성된 윈도우에 팔레트에서 선택한 객체들을 붙여 넣는다. 객체를 붙이기 전에
먼저 해야 될 일이 있는데, 바로 윈도우에 객체를 붙일 수 있는 컨테이너를 붙여주는
일이다.

@ 윈도우 구성
* 할렛'트
수

［그림 A-21］ 와 같이 팔레트에서 “고정된 위치”라고 표시되는 컨테이

선택자

너를 선택해 윈도우에 붙여준다.

GTK+ 기조
GTK+ 추가
Gnome

2

JJ

廳

n
A

□

O

c
主
0

‘

:

—

5

< 顧

a

J

—

씌
®

_ =
A
우

J 厂|

JJJ
으

［그림 A-21］ 컨테이너 선택

컨테이너를 붙이고 나면 이제 컨테이너에 각각의 객체들을 붙일 수 있다. 필자는 ［그림

A-22］ 처럼 라인 에디터 하나와 버튼 하나를 붙여 넣고 윈도우 사이즈도 알맞게 조절하
였다.

［그림 A-22］ 라인 에디터와 버튼을 붙여 넣은 모습

748 부록 A

===== PAGE 750 =====
B 이벤트 핸들러 등록
이제 버튼이 클릭되었을 때 어떤 일을 할 것인지 설정할
차례다. 버튼을 마우스로 선택하고, 속성 윈도우에서 ［그
림 A-23］ 과 같이 ［시그널］ 탭을 선택한다.

［그림 A-23］ 속성 윈도우

［그림 A-23］ 에서 시그널 버튼을 클릭하면 ［그림 A-24］
와 같은 시그널 선택 창이 생성되면서 어떤 시그널을 선
택할 것인지 물어본다. 우리는 버튼이 클릭되었을 때 어
떤 일을 수행하게 하고 싶기 때문에 clicked를 선택한다.

［그림 A-24］ 시그널 선택 창

clicked 시그널을 선택하면 clicked 시그널이 발생했을
때 수행할 함수명을 지정할 수 있게 ［그림 A-25］ 와 같이
표시된다.

［그림 A-25］ 버튼이 클릭되었을 때 수행할 함수명을 지정

프로그래밍 유형별 가용 유틸리티 749

===== PAGE 751 =====
필자는 기본적으로 설정되는 on_buttonl_clicked 를 함
수명으로 사용하겠다. 함수명을 지정했으면 속성 창 하
단에 있는 추가 버튼을 클릭한다. ［그림 A-26］ 과 같이

clicked 시그널과 핸들러가 지정한 함수로 등록된다.

［그림 A-26］ 이icked 핸들러 등록

QT 디자이너에서는 자체적으로 지원하는 소스 에디터가 있어 핸들러 함수를 QT 디자
이너에서 직접 작성할 수 있었다. 그렇지만 glade는 그런 소스 에디터가 제공되지 않는
다. 그래서 일단 glade를 이용해 GUI를 설계하고 소스를 빌드해 생성되는 소스에서 핸
들러 함수의 내용을 채워야 한다.

同 소스 빌드

그럼 소스 코드를 빌드해 보자. 메인 윈도우의 ［파일］ 메뉴에서 다음 그림과 같이 ［소스
코드 빌드］ 메뉴를 선택하면 지금까지 만든 윈도우를 바탕으로 소스 코드를 생성한다.

［그림 A-27］ 소스 코드 빌드

［소스 코드 빌드］ 메뉴를 선택하고 나면 ［그림 A-2기과 같이 프로젝트 옵션 창이 뜨는
데, 프로젝트 파일을 생성할 디렉토리를 지정한다.

부록 A

===== PAGE 752 =====
［그림 A-28］ 프로젝트 옵션 창

필자는 ［그림 A-28］ 과 같이 /root/Projects/projectl 디렉토리를 사용했다. 그리고 ［ C
옵션］ 탭을 선택해 ［일반 옵션］에서 ［ Gettext 지원］을 ［그림 A-29］ 와 같이 해제한다.

[그림 A-29] Gettext 지원 해제

마지막으로 창 하단에 있는 ［확인］ 버튼을 누르면 소스를 생성한다. 그리고 지정한 디
렉토리에 가보면 ［그림 A-30］ 과 같이 프로젝트 파일들이 생성된 것을 확인할 수 있다.
I (screen 2： bashl root@os：~/Projects/project1
[rooteos projectl]# Is
AUTHORS
NEWS
ChangeLog
README
Makefile.am acconFig.h
[root@os projectl]tt |

셔,.게고.헤｝리히
configure.in
macros

projectl.glade
src
stamp—h.in

［그림 A-30］ 프로젝트 파일 리스트

프로그래밍 유형별 가용 유틸리티 751

===== PAGE 753 =====
［그림 A-30］ 에서 표시되어 있는 autoget.sh 셸 스크립트를 수행하면 Makefile 이 생성
된다. 그리고 make 명령을 내리면 ［그림 A-31］ 과 같이 src 디렉토리에 지정한 프로젝
트명으로 실행 파일이 생성된 것을 확인할 수 있다.

三'] [screen 2: bash] roo1@os：~/Projects/projectl

_스믜싀

[root@os projectl]# Is src/projectl
src/projectl
[root60s projectl]# |

［그림 A-31］ 실행 파일 생성

./src/projectl 파일을 실행시키면 ［그림 A-32］ 와 같이 실행된다.

［그림 A-32］ 실행 모습

그렇지만 이렇게 실행이 된다고 해서 완전히 끝난 것은 아니다. 버튼이 클릭되었을 때
어떤 함수가 수행될지는 glade 에서 지정하지만 실제로 함수에 어떤 일을 수행하라고
작성해 주지 않았기 때문이다.

@ 핸들러 함수 내용 추가

glade가 QT 디자이너에 비해 불편한 점은 바로 이런 부분이다. QT 디자이너는 포루.~7.
램에 필요한 거의 대부분 요소들을 QT 디자이너 자체 내에서 해결 가능하지만, glade
는 오직 화면 구성만을 glade에서 할 수 있다.
나머지 소스에 관련된 부분은 사용자가 직접 vim으로 소스를 수정해야 한다. src 디렉
토_리에 가보면 다음과 같은 소스 파일들이 생성되어 있는 것을 확인할 수 있다.

'디 [screen 2： bash] root@os：~/Projects/project1/src
[root@os src]tt Is
Makefile callbacks.c interface.c.bak main.c
Makefile.am callbacks.h interface.h support.c
Makefile.in interface.c interface.h.bak support.h
[rootl
os src]tt |

흐

버
［그림 A-33］ 빌드된 소스 파일 리스트

부록 A

===== PAGE 754 =====
interface.c 파일은 윈도우를 구성하는 파일이다. interface.c 파일을 열어보면 어떤 객
체가 윈도우를 구성하는지 확인할 수 있다. main.c 파일은 main() 함수가 들어 있는 파
일로, 프로그램이 수행될 때 윈도우를 화면에 생성하는 코드가 들어 있다. callbacks.c
파일에는 버튼이 클릭되었을 때 수행할 함수가 들어 있다. caUbacks.c 파일을 열어보
면 ［그림 A-34］ 와 같이 이전에 cHcked 시그널에 추가한 핸들러 함수인 on_buttonl_

clickedO 함수가 들어 있음을 확인할 수 있다.

[그림 A-34] c게Ibacks.c 파일 내용

그러면 다음과 같은 내용으로 on_button l_clicked 함수를 채운다.
〔예제 A-2)

callbacks.c 파일의 내용

...생략

void
on_buttonl_clicked

(GtkButton

*button,

gpointer

user_data)

{
GtkWidget *top;
GtkWidget *entry;
top = gtk_widget_get_toplevel(GTK_WIDGET(button));
entry = lookup_widget(GTK_WIDGET(top), "entryl");
gtk_entry_set_text (GTK_ENTRY(entry), "Hello World");
}

프로그래밍 유형별 가용 유틸리티 753

===== PAGE 755 =====
entry = lookup^vidget(GTK_WIDGET(top), "entryl")； 행에서 entryl 은 라인 에디
터의 이름을 의미한다. 필자는 glade에서 라인 에디터를 등록할 때 entryl이라는 이름
으로 등록했다. 그래서 entryl으로 사용한 것이다.
라인 에디터의 이름을 모를 경우 glade 화면에서 라인 에디터를 클릭한 후 속성 창을
보면 어떤 이름으로 지정되어 있는지 알 수 있다. 이렇게 버튼이 클릭되었을 때 수행할
콜백 함수를 작성했다면 이제 저장하고 다시 컴파일한다. 그리고 생성되는 projectl 파
일을 수행한 후 버튼을 클릭하면 라인 에디터 부분에 “Hello World” 문자열이 출력되
는 것을 확인할 수 있다.
Ml

windowl
(Hello World
buttonl

[그림 A-35] 버튼 클릭 모습

이상이 glade를 이용한 간단한 GUI 애플리케이션 제작에 관한 설명이다. QT 디자이
너의 경우에는 GUI 애플리케이션을 위해 많이 사용되지만 glade는 기능이 미흡하기
때문에 코딩을 위한 기초 코드를 생성하는 용도 외에는 잘 사용되지 않는다. GTK를 잘
모른다면 기본적인 GUI 코드를 생성하는 데 glade 를 사용하면 유용할 것이다.
지금까지의 내용만으로는 QT 디자이너나 이ade를 이해하기 힘들 것이다. QT 디자이
너나 glade 를 제대로 알려면 반드시 QT 나 GTK를 알아야 한다. 그렇기 때문에 이 책
의 범위를 벗어나도 한참 벗어나는 이야기가 될 수밖에 없다.
필자는 단지 QT 디자이너와 glade를 소개하는 정도로만 끝낼까 한다. 좀 더 자세한 내
용을 알고 싶은 독자는 관련 서적을 참고하기 바란다.

754 부록 A

===== PAGE 756 =====
2

트워크 프로그래밍

다음에 소개할 내용은 네트워크 프로그래밍에 사용하면 편리한 유틸리티들이다. 네트
워크 프로그래밍을 하는 데 있어 문제가 발생한다면 패킷을 분석할 수 있어야 한다.
리눅스는 이때 사용 가능한 많은 유틸리티를 제공하는데, tcpdump, wireshark, iptraf
가 대표적이다. 그럼 각각의 유틸리티들은 어떨 때 사용하면 편리한지 알아보자.

D 패킷의 흐름으로 분석하는 tcpdump
tcpdump는 패킷의 흐름을 보는 데 매우 유용한 유틸리티다. root의 권한으로 셸 프롬
프트에서 tcpdump라고 명령을 내리면 ［그림 A-36］ 과 같이 tcpdump가 수행된다.
S [screen 2: bash] root@os：/

휴771石?》3.593377 거 0.118.56.767.1074 > 211 . 189.19.175. ssiu 丁三히請話司호R 1644fl (DF)
07:16:23.596891 211 .189.19.175.ssh > 210.118.56.207.1874: P 85848:86060(212) ack 85 win 20440 (DF) [tos
0x18]
07:16:23.686874 211.189.19.175.ssh > 210.118.56.207.1074： P 86060:86192(132) ack 85 win 20M0 (DF) [tos
0x10]
07:16:23.616935 211 .189.19.175.ssh > 210.118.56.207.1074: P 86192:86324(132) ack 85 win 20440 (DF) [tos
0x10]
07:16:23.626934 172.16.159.175.5901 > 172.16.159.9.4770： P 243048:244036(988) ack 2461 win 2868 (DF)
07:16:23.62701*4 211.189.19.175 .ssh > 210.118.56.207.1074: P 86324:86456(132) ack 85 win 20440 (DF)
0X10]
07:16:23.628213 172.16.159.9.4770 > 172.16.159.175.5901: P 2461:2471(10) ack 244836 win 17520 (DF)
07:16:23.628325 172.16.159.175.5901 > 172.16.159.9.4770: . ack 2471 win 2868 (DF)
07:16:23.628576 211.189.19.175.ssh > 210.118.56.207.1074: P 86456:86788(332) ack 85 win 20440 (DF)
0X10]
87:16:23.637658 211.189.19.175.ssh > 210.118.56.207.1074: P 86788:87088(212) ack 85 win 28440 (DF)
0X10]
07:16:23.646926 211.189.19.175.ssh > 210.118.56.287.1074: P 87000:87132(132) ack 85 win 28440 (DF)
0x10]

[tos

[tos
[tos
[tos

[그림 A-36] tcpdump 수행 모습

네트워크에 대한 지식이 조금이라도 있는 독자라면 tcpdump가 생성하는 메시지의 의
미를 이해할 수 있을 것이다. tcpdump의 원래 용도는 네트워크의 문제를 진단하는 것
이지만 네트워크 프로그래밍을 하는 데 있어 문제를 진단하는 데에도 유용하게 사용될
수 있다.

ssh 나 telnet 을 사용해 원격 접속한 컴퓨터에서 tcpdump 를 실행시키면 출력되는 패
킷이 화면에 다시 출력되어 화면에 무수히 많은 패킷이 보여 어지러울 수 있다. 그럴
때는 다음과 같은 옵션으로 tcpdump를 수행시키면 된다.
tcpdump src port not 22 and dst port not 22

프로그래밍 유형별 가용 유틸리티 755

===== PAGE 757 =====
위 옵션을 사용하면 ssh의 포트인 22번 포트에 들어오는 패킷과 나가는 패킷은 화면에
출력하지 않는다. 물론 telnet 사용자는 22번 대신 telnet 포트인 23번을 옵션으로 입 력
하면 된다.
@ 패킷을 분석하는 wireshark

tcpdump 는 패킷의 흐름을 분석하는 데 유용하지만 개개의 패킷을 분석하는 일에는
적당하지 않다. 개개의 패킷을 분석하는 일에는 wireshark를 사용하면 된다.
드데띄

< <capture> — Ethereal
Rie Edit Capture Display Jo 7이 s
7
1 0.000000 172»16.159,9 5
2 0.000102 172.16.159 1 7
3 0.003919 172.16.159 1 5
17
4 0.010345 172.16.159
1
5 0.0103G9 172.16.159 1 75
6 0.010404 172.16.159 9
7 0.010805 172.16.159 1 75
8 0.010839 172.16.159 1
9 0.010845 172.16.159 1 75
10 0.010852 172.16.159 9
5
11 0.011165 172.16.159 1 7
12 0.011183 172.16.159 1
5
7
1
13 0.011189 172.16.159
14 0.011195 172.16.159 5
7
15 0.011423 172.16.159
1.R ft M.1AZ9.
,179 IK
75

17246.159.175
172.16.159.9
172.16.159.9
172.16.159.9
172.16.159.9
172.16.159.9
172.16.159.175
172.16.159.9
172.16.159.9
172.16.159.9
172.16.159.175
172.16.159.9
172.16.159.9
172.16.159.9
172.16.159.175
170 1£ 1C.Q Cl

5901 > 4770 [ACK] Seq=3370286040 Ack=2670327837 U
5901〉4770 [ACK] Seq=3370286040 Ack=2670327837 kl
5901 > 4770 [ACK] Seq=33702=40 Ack=2670327837 U
5901 〉 4770 [ACK] Seq=3370287500 Ack=2670327837 U
5901 > 4770 [PCK] Seq=33702=60 Ack=2670327837 U
4770 > 5901 [ACK] Seq=2670327837 Ack=3370288960 kl
5901 > 4770 [ACK] Seq=3370290420 Ack=2670327837 U
5901 > 4770 [ACK] Seq=3370291880 Ack=2670327837 U |
5901 > 4770 [ACK] Seq=3370293340 Ack=2670327837 W J
4770 > 5901 [ACK] Seq=2670327837 Ack=3370291880 U ;
5901 > 4770 [PSH, ACK] Seq=3370294800 Ack=267032기
59)1 > 4770 [ACK] Seq=3370296260 Ack=2670327837 Id g
5901 > 4770 [ACK] ==3370297720 fick=2670327837 bl ■
4770 > 5901 [ACK] Seq=2670327837 Ack=3370294800 IJ
RQfM 丄 才77|1 Torkl 匕°”~777n9c픠

5
□ Frame 1 (60 bytes on wire, SO bytes captured)
S Ethernet II, Src：
00：00：F0：77：87：cl, Dst： 00：a0：c9:8c：02：84
5
□ Internet Protocol, Src Addr： 172.16.159.9 (172.16.159.9), Dst Addr： 172.16.159.175 (172.16.159.175)
S Transmission Control Protocol, Src Port: 4770 (4770), Dst Port： 5901 (5901), Seq： 2670327831, Ack： 3370286040, Len： 6
Hata

77 87 Cl
lo
08
e2
17
61
32

Filterj |

45흐00
10
50 18

...J?...................

..................
이 Reset| Apply|| File： <capture> Drop^O

[그림 A-37] wireshark 수행 모습

[그림 A-3기은 wireshark# 수행한 후의 모습을 보여준다. wireshark를 사용하면 이렇
게 각 패킷의 헤더 부분과 데이터 부분을 분석해 화면에 출력한다.

wireshark# 사용하려면 X-Windows 터미널에서 wireshark 명령을 입력해 wireshark
를 수행하고 [Capture] 메뉴에서 [Start] 메뉴를 선택한다. 사용법이 매우 간단하기 때
문에 따로 언급하지 않겠다.

同 현재 시스템에 지나가는 패킷을 종류별로 분석

현재 시스템에 흘러가는 패킷을 종류별로 분석하는 일에는 iptraf 를 사용하면 된다.
셸에서 iptraf 명 령을 내리면 [그림 A-38]과 같은 화면이 출력된다.

756 부록 A

===== PAGE 758 =====
[그림 A-38] iptraf 실행 모습 1

［그림 A-38］ 에서 아무 키나 누르면 화면에 메뉴가 출력되는데, 원하는 메뉴를 선택하
면 ［그림 A-39］ 와 같이 시스템에 흘러가는 패킷을 종류별로 출력한다.

[그림 A-39] iptraf 실행 모습 2

프로그래밍 유형별 가용 유틸리티 757

===== PAGE 759 =====
이상이 프로그래밍 유형별로 사용하면 편리한 유틸리티들에 대한 소개였다. 필자가 소
개한 유틸리티 외에도 프로그래밍에 도움이 되는 유틸리티는 정말 무수히 많다.

proc 파일 시스템의 정보를 보여주는 procinfo, ipc 자원에 대한 정보를 보여주는
ipcs, 프로세스가 열고 있는 파일 디스크립트의 정보를 보여주는 Isof 등 무수히 많은
유틸리티가 프로그래밍을 하는 데 도움을 줄 수 있다. 나머지 유틸리티는 독자들이 한
번 찾아보기 바란다.

758 부록 A

===== PAGE 760 =====
부록 B

vim 명령 정리

===== PAGE 761 =====
n

저장 및 종료

명령

설명

명령

설명

：w

저장

：w file.txt

file.M 파일로 저장

：w〉〉file.txt

file.txt 파일에 덧붙여서 저장

:q

vi 종료

:q!

VI 강제 종료

ZZ

저장후종료

:wq!

강제 저장 후종료

：e file.txt

file.txt 파일을 불러옴

：e

현재 파일을 불러옴

@ 입력모드 전환
a

커서 위치 다음 칸부터 입력

A

커서 행의 맨 마지막부터 입력

i

커서의 위치에 입력

1

커서 행의 맨 앞에서부터 입력

0

커서의 다음 행에 입력

0

커서의 이전 행에 입력

s

커서 위치의 한 글자를 지우고 입력

CC

커서 위치의 한 행을 지우고 입력

h

왼쪽 한 칸이동

j

아래쪽 한 칸이동

1

오른쪽 한 칸 이동

k

위쪽 한 칸이동

h

왼쪽으로 이동

I

오른쪽으로 이동

i

아래 행으로 이동

k

위 행으로 이동

w or W

다음 단어의 첫 글자로 이동

b or B

이전 단어의 첫 글자로 이동

e or E

단어의 마지막 글자로 이동

<CR>

다음 행의 첫 글자로 이동

A

그 행의 첫 글자로 이동

$

그 행의 마지막 글자로 이동

+

다음 행의 첫 글자로 이동

—

위 행의 첫 글자로 이동

(

이전 문장의 첫 글자로 이동

)

다음 문장의 첫 글자로 이동

{

이전 문단으로 이동

}

다음 문단으로 이동

H

커서를 화면의 맨 위로 이동

z<CR>

현재 행을 화면의 맨 위로 이동

M

커서를 화면의 중앙으로 이동

z.

현재 행을 화면의 중앙으로 이동

L

커서를 화면 최하단으로 이동

z-

현재 행을 화면의 최하단으로 이동

[n]H

커서를 위에서 n행으로 이동

[n]L

커서를 아래에서 n행으로 이동

j Ci가-니 반 화면 위로 스크롤

gi라-d

반 화면 아래로 스크롤

jC 러}-b

한 화면 위로 스크롤

Sfl—f

한 화면 위로 스크롤

문서의 맨 첫 행으로 이동

G

문서의 맨 마지막 행으로 이동

n행으로 이동

：[n]

n행으로 이동

@ 이동

- gg. 1G
[n]G

760 부록 B

===== PAGE 762 =====
Q 삭제
X, dl

커서 위치의 글자 삭제

X, dh

커서 바로 앞의 글자 삭제

dw

한 단어를 삭제

dO

커서 위치부터 행의 처음까지 삭제

D, d$

커서 위치부터 행의 끝까지 삭제

dd

커서가 있는 행을 삭제

dj

커서가 있는 행과 그 다음 행을 삭제

dk

커서가 있는 행과 그 앞 행을 삭제

@ 복사 & 붙이기

yy

커서가 위치한 한 행 복사

P

붙여넣기

[N]yy

커서가 위치한 이후로 N행 복사

[Nip.

N번만큼 붙여넣기 반복

블록 지정

Ctrl) + V

비주얼 블록 지정

대소문자 전환

d

삭제

厂'

복사

C

치환

>

행 앞에 탭 삽입

〈

행 앞에 탭 제거

선택된 영역에 대해 ex 명령

J

행을 합침

대문자로 만듦

U

소문자로 만듦

@ 블록 지정 관련
V

U

8 문자열 탐색 및 치환
/［문자열］

문자열을 탐색

：s/old/new

현재 행의 처음 01d를 new로 교체

：s/old/new/g

현재 행의 모든 old를 new로 교체

:10,20s/이 d/new/g

10행부터 20행까지 모든 이d를 new로 교체

：—3,+4s/이 d/new/g

현재 커서 위치에서 3행 위부터 4행 아래까지 old를 new로 교체

:%s/old/new/g

문서 전체에서 old> new로 교체

:%s/old/new/gc

문서 전체에서 Old를 new로 확인하며 교체

:g/pattern/s/old/new/g

patternO| 있는 모든 행의 old를 new로 교체

：g/pattern/s//new/g

:%s/이 d/new/g 와 동일

vim 명령 정리 761

===== PAGE 763 =====
@ vim 정규 표현식
A

[]

행의 첫 문자 （[]안에서는 not의 의미）

$

행의 끝

아무 문자나 한 문자 의미

\|

or의 의미

[b사이의 문자 중하나

\{min,max\}

min 이상 max 이하 반복됨

*

앞의 내용이 0번 이상 반복됨

\+

앞의 내용이 1번 이상 반복됨

\<

단어의 시작

\>

단어의 끝

\n

개행 문자

\t

탭 문자

El vim 확장 정규 표현 문자열
\i

변수 지정에 사용되는 문자들[_0~9A-Za-z]

\l

\i와 같지만 숫자는 제외

\k

keyword로 사용하는 문자0—9A—Za-z〉]

\K

\k 와 같지만 숫자는 제외

\f

파일 이름으로 사용하는 문자

\F

뉴와 같지만 숫자는 제외

\p

프린트 가능한 문자

\P

\p 와 같지만 숫자는 제외

\s

whitespace 아Taracter（공백과 탭）

\S

non-whitespace character

\d

숫재 0-9]

\D

숫자가 아닌 문자T0-9]

\x

16진수 숫자{0-9A-Fa-f]

\x

16진수 숫자가 아닌 문자｛ —A-Fa-f]

\o

8진수 숫재 0-7]

\o

8진수 숫자가 아닌 문재 ◎7]

\w

영문 단어에서 사용되는 문재>9A-Za-z-]

\W

영문 단어에서 사용되지 않는 문재A>9A-Za-z-]

\h

영문 단어의 시작에 사용되는 문자｛ A-Za-z-]

\H

영문 단어의 시작에 사용되지 않는 문재AA-Za-z-]

\a

모든 알파벳 [A-Za-z]

\A

알파벳이 아닌 문재AA-Za-z]

\I

소문재 a-z]

\L

소문자가 아닌 문자[Aa-z]

\u

대문재 A-Z]

762 부록 B

===== PAGE 764 =====
\u

대문자가 아닌 문자TA-z]

\e

esc

\t

탭

\r

캐리지 리턴

\b

백스페이스

\n

개행 문자

E POSIX 문자 클래스
문자클래스

| 내용

[:alnum：]

알파벳과 숫재 A-Za-zO-9]

[:alpha：]

알파벳 [A-Za-z]

[:cntrl:]

제어 문자

[：blank:]

탭과 공백 문자

[:digit：]

숫재 0-9]

[：graph:]

제어 문자와 공백 문자를 제외한 문자

[lower：]

소문재 a-z]

Clipper：]

대문재 A-Z]

[：print:]

제어 문자를 제외한 문자 즉. 프린터할 수 있는 문자

[:punct:]

[:graph:] 문자 중 [:alnum：]을 제외한 문자. 예） !,@,#,$,%,A

[:space：]

화이트 스페이스 예） 공백, 탭, 캐리지 리턴, 뉴 라인. 수직 탭, 폼 필드

[:xdigit:]

16진수

ID 파일 버퍼 관련 명령
: buffers

버퍼의 내용을 나열

:files 또는 ：ls

버퍼의 내용을 나열

:b[N]

N 버퍼로 이동

：bd[N]

N 버퍼를 삭제（ N이 없으면 현재의 버퍼를 완전 삭제）

：bw[N]

N 버퍼를 완전 삭제（ N이 없으면 현재의 버퍼를 완전 삭제）

:bp[N]

이전 버퍼로 이동, N을 붙이면 N번만큼 이전 버퍼로 이동

：bn[N]

이후 버퍼로 이동, N을 붙이면 N번만큼 이후 버퍼로 이동

：sb [N]

창을 수평 분할해 N번 버퍼를 로드

：bf

첫 번째 버퍼로 이동

：bl

마지막 버퍼로 이동

：al

현재 열려 있는 모든 버퍼를 수평 분할 창에 로드
vim 명령 정리 763

===== PAGE 765 =====
E 다중 창 관련 명령
명령 모드

ex 모드

결과

창생성
[CtrJ-WS

:sp[plit]

현재 파일을 두개의 수평 창으로 나눔

Ctrtj—wv

:[N]vs[plit]

새로운 수직 창 생성, N0| 붙으면 N칸 크기의 창 분할

(M—wn

：new

새로운 수평 창 생성

ggpV

수평 창으로 나누고 이전 파일의 오픈

Ctrl]~wf

창을 수평으로 나누고 커서 위치의 파일을 오픈

iCtrl]-wi

커서 위치의 단어가 정의된 파일을 오픈
창 삭제

%]—wq

:q[uit]!

현재 커서의 창을 삭제

Ctrl]—WC

：clo[se]

현재 커서의 창을 삭제

: Ctrl]—WO

：on[ly]

현재 커서의 창만 남기고 모든 창 삭제
창이동

Ctrl]-wh

왼쪽 창으로 커서 이동

Ctii]-wj

아래쪽 창으로 커서 이동

Ctrl]—Wk

위쪽 창으로 커서 이동

心 trlHv!
Ctii]-ww

오른쪽 창으로 커서 이동
.
_ __
창을 순차적으로 이동

Ctrl]—WD

가장 최근에 이동한 방향으로 이동

心tffl-wt

최상위 창으로 이동

Ctrl]-wb

최하위 창으로 이동
창 위치 바꾸기

；Ctrt]-wr

순차적으로 창의 위치를 순환

Ctrt]—wx

이전 창과 위치를 바꿈
창 크기 조정
창의 크기를 모두 균등하게 함

iCtrt]-w=

수평 분할에서 창의 크기를 최대화
Ctrl|-w|

수직 분할에서 창의 크기를 최대화

Cti비一w「N]+

：res[ize] +N

창의 크기를 N행만큼 증가（ Ct바-w+느 1행만큼 증가）

iCtrl]—w[N]—

：res[ize] -N

창의 크기를 N행만큼 감소（£"w-는 1행만큼 감소）

Ctr나-wfND

창의 크기를 오른쪽으로 N칸만큼 증가（수직 창에 한함）

；CtHWNl<

창의 크기를 왼쪽으로 N칸만큼 증가（수직 창에 한함）

764 부록 B

===== PAGE 766 =====
E 마킹 및 마킹한 위치로 이동
명령

내용

ma

a로 마킹, mb는 b로 마킹

'a

a로 마킹된 위치로 돌아감

직전에 커서가 위치하던 행의 처음
이전에 vim으로 현재 파일을 닫았을 때

명령

내용

‘a

a로 마킹된 줄의 처음으로 돌아감

w
\u

직전의 커서 위치로 이동
이전에 vim으로 현재 파일을 닫았을 때

커서가 있던 행의 처음으로 이동

커서가 있던 위치로 이동

E ctags 관련 명령
：ta [tag] or Ctri；-

tag가 정의된 위치를 나열하고 선택한 위치로 점프,

：ts [tag] or :tj [ta 9]

현재 위치는 stack에 push된다.

：po or Ctrl +t

stack top에 저장된 위치를 pop하고 그 위치로 점프

：sts [tag]

tag가 정의된 위치를 나열하고 선택한 위치로 창을 수평 분할해

：stj [tag]

새로 생성된 창에 표시

:tn

나나 ts로 점프했을 때 다음 tag로 점프

:tp

tj나 ts로 점프했을 때 이전 tag로 점프

：tr

나나 ts로 점프했을 때 처음 tag로 점프

：tl

5나 ts로 점프했을 때 마지막 tag로 점프

:pts [tag]

tag가 정의된 위치를 나열하고 선택한 위치로 창을 수평 분할해 새로 생성된

창에 표시하지만 커서는 현재 위치에 유지
:ptj [tag]

미리보기 윈도우에 tag가 정의된 형식을 보여줌

：ptn

ptj 나 pts로 점프했을 때 다음 tag로 점프

:ptp

ptj나 pts로 점프했을 때 이전 tag로 점프

：ptr

ptj 나 pts로 점프했을 때 처음 tag로 점프

：ptl

ptjL^ pts로 점프했을 때 마지막 tag로 점프

E@ cscope 관련 명령
► 기본 현싀____________________
:cs find { 질의종류} { 심볼}
예） : cs find s start_kernel

vim 명령 정리 765

===== PAGE 767 =====
► 질의 종류
0 or s

Find this C symbol

1 or g

Find this definition

2 ord

Find functions called by this f니nction

3 or c

Find functions calling this Unction

4ort

Find assignments to

6 or e

Find this egrep pattern

7orf

Find this file

8or i

Find files #inchjding this file

@ screen 단축키
HD+a’

화면 하단에 새로운 가상 터미널을 선택할 수 있는 입력 프롬프트가 나옴

jC러]+a”

현재 생성되어 있는 모든 가상 터미널이 나열되며 커서로 선택할 수 있음

으！i+a[N]

N번째 가상 터미널로 이동

아「l+¥

바로 이전 가상 터미널로 이동

Ctrf.+ac

새로운 가상 터미널 생성

WHad

현재의 가상 터미널을 닫음

EB)+ag

vis니게 bell을 on/off

|Ctrt|+an

다음 가상 터미널로 이동

g피+ap

이전 가상 터미널로 이동

766 부록 B

===== PAGE 768 =====
부록 c
옵션 정리

===== PAGE 769 =====
D gcc 전역 옵션

I 설명

옵션
-E

전처리 과정 화면에 출력

-s

어셈블리 파일 생성

-c

오브젝트 파일 생성

-v

컴파일 과정 화면에 출력
컴파일 시 생성되는 중간 파일 저장

save-temps

컴파일 과정에서 생성되는 중간 코드 생성（ RTL 파일 등 생성）

-da

@ 전처리기（ cppO）

옵션

옵션

설명

너［패스］

헤더 파일을 탐색할 디렉토리 지정 예） -l/opt/include

-include ［헤더 파일 패스］

해당 헤더 파일을 모든 소스 내 추가 예） -include /root/my.h

—이매크로］

외부에서 #define 지정 예） -DDEBUG

-D［매크로］=［매크로 값］ 외부에서 해당 매크로를 정의하고 값을 지정 예）—DDEBUG=I
-U［매크로］

외부에서 #undef 지정 예） -UDEBUG

-M 또는 -MM

m가;e 기술 파일을 위한 소스 파일의 종속 항목 출력

-nostdinc

표준 C 헤더 파일을 include하지 않음

-C

전처리 과정에서 주석을 제거하지 않음

-Wp,［옵션 리스트］

옵션 리스트를 전처리기에 바로 전달

@ C 컴파일러（ cd）

옵션

► c 언어 옵션
옵션

설명

-ansi

ANSI C 문법으로 문법 검사

—std=[C

표준]

지정한 C 표준으로 문법 검사（표준: c89, c99. gnu89, gnu99 등）

-traditional

K&R C 문법으로 문법 검사

-fno-asm

asm, inline, typeof 키워드를 사용하지 않음（ gnu89 문법 기준）

768 부록 c

===== PAGE 770 =====
► 경고 옵션
옵션

| 설명

-Wall -W

모든 경고 메시지 출력

-w

모든 경고 메시지 제거

-Werror

모든 경고를 오류로 취급해 컴파일 중단

-pedantic

C89 표준에서 요구하는 모든 경고 메시지를 표시

-pedantic-errors

C89 표준에서 요구하는 모든 오류 메시지를 표시

-Wtraditional

ANSI C와 K&R C 간에 서로 다른 결과를 가져올 수 있는 부분이 있다면 경고

► 최적화 옵션
옵션

I 설명

-00

아무런 최적화를 수행치 않음

-01 또는-0

최적화 레벨 1 수행

—02

최적화 레벨 2 수행

-03

최적화 레벨 3 수행

—0s

사이즈 최적화 수행

► 디버깅 옵션
옵션

I 설명

_g

바이너리 파일에 디버깅 정보 삽입

—pg

프로파일을 위한 코드 삽입

B 어셈블리(as) 옵션
옵션

설명

-Wa,［옵션 리스트］

어셈블러에게 옵션 리스트를 바로 전달

-Wa-al

어셈블된 코드와 인스트럭션을 보여줌

-Wa-as

정의된 심볼을 보여줌

gcc 옵션 정리 769

===== PAGE 771 =====
@ 링크(Id) 옵션
옵션

설명

-L［패스］

라이브러리 탐색 디렉토리 지정 예) -L/opt/lib

—1 ［라이브러리 이름］

해당 라이브러리를링크 예) 一Im

-shared

공유 라이브러리를 우선해 링크

-static

정적 라이브러리를 우선해 링크

-nostdlib

표준 C 라이브러리를 사용하지 않음

-M 또는 一MM

make 기술 파일을 위한 소스 파일의 종속 항목 출력

-nostdinc

표준 C 헤더 파일을 include하지 않음

-Wl,［옵션 리스트］

옵션 리스트를 링크에 바로 전달

770 부록 c

===== PAGE 772 =====
부록 D

autoconf 매크로
정리

===== PAGE 773 =====
O 프로그램 결정 매크로
매크로

넘겨주는 변수

설명

AC_PROG_CC

CC

C 컴파일러 결정（환경 변수 CC 값이 우선이고, 없

으면 gcc, cc순으로 찾음）
AC_PROG_CPP

CPP

C전처리기 결정

AC_PROG_CXX

cxx

C++ 컴파일러 결정

AC_PROG_CXXCPP

CXXCPP

C++전처리기 결정

AC_PROG_F77

F77

포트란 컴파일러 결정

AC_PROG_AWK

AWK

awk 프로그램 결정（ mawk, gawk, nawk, awk순으

로 찾음）
AC_PROG_YACC

YACC, BISON

YACC를 결정(bison, byacc, yacc순으로 찾음)

AC_PROG_INSTALL

INSTALL

install 프로그램이나 install 스크립트 결정

AC_PROG丄EX

LEX

lex 결정（ flex, lex순으루 찾음）

AC_PROG_LN_S

LN

link 결정

AC_PROG_MAKE_SET

MAKE

make 결정

AC_PROG_RANLIB

RANLIB

ranlib 결정

AC_PROG_EGREP

EGREP

grep 명령의 —E 옵션, egrep순으로 결정

AC_PROG_FGREP

FGREP

grep 명령의 -F 옵션, fgrep순으로 결정

AC_CHECK_PROG（ variable, prog, value-if-found, [value-if-not-found], [path], [reject]）
AC_CHECK_PROG 매크로는 셸의 PATH 환경 변수 디렉토리들에서 prog 프로그램을 찾
는다. 찾으면 variable 변수에 value-if-found 값을 넣고, 못 찾으면 value -if-not-found
값을 넣는다.
대괄호（[]）가 있는 인자들은 모두 생략 가능함을 의미하고. path 인자가 사용되었다면

path 인자가 지정한 위치에서도 찾는다. 찾았다 할지라도 reject 인자가 지정하는 파일은
제외한다.

AC_CHECK_TOOL(Var/ab/e, prog, [value-if-not-found], [path])
AC_CHECK_PROG

매크로와

유사하지만

prog에

AC_CANONICAL_HOST와

대시(-)

를 붙인 prog를 먼저 찾고, 없으면 그냥 prog를 찾는다. AC_CANONICAL_HOST는

config니re

스크립트를

로 지정 가능하다.

772 부록 D

수행할

때

./configure

—host=i386-redhat-linux와

같은

형식으

===== PAGE 774 =====
AC_CHECK_PROGS(Var/ab/e, progs, [value-if-not-found], [path])
AC_CHECK_PROGS 매크로는 공백으로 구분되는 progs 리스트에 있는 프로그램들을 차
례로 찾는다. 찾았으면 variable 변수에 찾은 값을 넣고, 리스트의 프로그램을 하나도 못 찾
으면 value-if-not-found 값을 넣는다.
기본적으로 PATH 셸 환경 변수에 등록된 디렉토리에서 찾지만 path가 지정되어 있으면

path 위치도 찾는다.

AC_CHECK_T00LSfvariable, progs, [value-if-not-found], [path])
progs에 여러 개의 프로그램 리스트를 사용하는 것은 AC_CHECK_PROGS 매크로와 같
고, 프로그램을 찾는 방법은 AC_CHECK_TOOL 매크로와 같다.
즉, 프로그램 리스트의 프로그램을 순차적으로 찾는데, AC_CANONICAL_HOST와 대시
(-)를 붙인 것을 먼저 찾고, 없으면 리스트에 등록된 파일명으로 찾는다.

AC_PATH_P RO G (variable, prog, [value-if-not-found], [path])
프로그램을 찾는 것은 AC_CHECK_PROG 매크로와 같고, variable 변수에 찾은 프로그램
의 절대 경로가 들어간다는 점이 틀리다.

AC_PATH_PROGS(Variab/e, progs, [value-if-not-found], [path])
AC_CHECK_PROGS 매크로와 같고, variable 변수에 찾은 프로그램의 절대 경로가 들어간
다는 점이 틀리다.

AC_PATH_TOOLfv'ar/ab/e, prog, [value-if-not-found], [path])
AC_CHECK_TOOL 매크로와 같고, variable 변수에 찾은 프로그램의 절대 경로가 들어간
다는 점이 틀리다.

허 파일 체크 매크로

AC_CHECK_FILE(fife, [action-if-found], [action-if-not-found])
AC_CHECK_FILE 매크로는 file이 있으면 action-if-found< 수행하고, 없으면 action-ifnot-found를 수행한다.

AC_C H E C K_F IL E S (fifes, [action-if-found], [action-if-not-found])
files

리스트에

있는

파일이

있으면

action-if-found를

수행하고,

없으면

action-if-not-

found를 수행한다. 한 번만 액션을 수행하는 게 아니라 해당하는 파일 각각의 유무에 따른
액션을 수행한다.

autoconf 매크로 정리 773

===== PAGE 775 =====
0 라이브러리 체크 매크로
AC_C H EC K_LIBf//bra/y, function, [action-if-found], [action-if-not-found], [other-libraries])
인자인 라이브러리(library)와 링크해 주어진 함수(function)가 사용 가능한지 테스트한다.
사용 가능하다면 action-if-found에 지정된 셸 스크립트 또는 autoconf 매크로를 수행하
고, 사용 가능하지 않다면 action-if-not-found에 지정된 셸 스크립트 또는 autoconf 매
크로를 수행한다.
사용

가능하지만

action-if-found가

생략되었다면

LIBS

변수에

-llibrary가

추가되고,

DEFS 변수에 모두 대문자인 -DHAVE_LIBlibrary=l이 추가된다.
예를 들면 m 라이브러리가 링크 가능하다면 LIBS 변수에 -1m이 추가되고, DEFS 변수에

-DHAVE_LIBM=I이 추가된다.
other-libraries에는 다른 라이브러리와 같이 링크하지 않으면 링크 오류가 나는 라이브러
리인 경우처럼 링크할 라이브러리를 공백 문자로 분리해 적는다.
예를 들면 gtk 라이브러리와 같이 반드시 XII 라이브러리나 gdk 라이브러리와 링크해야
만 링크 오류가 나지 않는 라이브러리 같은 경우에는 [-1X11 -Igdk]와 같은 형식으로 적어
준다.

AC_SEARCH_LIBS('foncton, search-libs, [action-if-found], [action-if-not-found], [otherlibraries])
주어진 함수(function)가 사용 가능한 라이브러리를 라이브러리 리스트인 search-libs
서 찾는다.

H 헤더 파일 체크 매크로
AC_CHECK_HEADER(/7eac/er-f/7e, [action-if-found], [action-if-not-found], [includes =
default-includes ’])
주어진

헤더

파일(header-file)을

찾으면

action-if-found<

수행하고,

찾지

못하면

action-if-not~found< 수행한다.

AC_CHECK_HEADERSf/?eader-f/7es, [action-if-found], [action-if-not-found], [includes =
'default-includes ’])
주어진 헤더 파일 리스트인 header-files에서 각각의 헤더 파일을 찾는다.

AC_HEADER_DIRENT
바로 전에 설명 했으므로 생략

774 부록 D

===== PAGE 776 =====
AC_HEADER_MAJOR
sys/types.h가 있다면 major, minor, makedev를 define하지 않는다. 그리고 sys/mkdev.
도가 있으면 MAJOR_IN_MKDEV를 define한다. sys/sysmacros.h가 있다면 MAJOR_IN_

SYSMACROS를 define 한다.

AC_HEADER_STAT
SJSDIR 매크로와 SJSREG 매크로가 sys/stat.h에서 define되었다면 잘못되었기 때문에
STAT_MACROS_BROKEN을 define 한다.

AC_HEADER_STDBOOL
stdbooLh 파일이 C99 문법으로 존재한다면 HAVE_STDBOOL_H=1 을 define한다. 그리
고 _Bool 타입이 정의되어 있다면 HAVE__BOOL을 define한다.

@ 함수 사용 가능 체크 매크로

AC_CHECK_FUNCffunction, [action-if-found], [action-if-not-found])
주어진 함수(f니nction)가 사용 가능한지 체크한다. 사용 가능하면 action-if-fo니nd를 수행
하고, 가능하지 않다면 action-if-not-fo니nd를 수행한다.

AC_CHECK_RJNCS(fi/nc#ons, [action-if-found], [action-if-not-found])
주어진 함수들의 리스트에서 각각의 함수가 사용 가능한지 체크한다. 사용 가능하면

action -if-found# 수행하고, 가능하지 않다면 action-if-not-fo 니 nd 를 수행한다.

I 구조체 체크 매크로
AC_CHECK_MEMBER(aggregate.member, /Ac#on-/후fbwnq/, [action-if-not-found], [includes
= 'default-includes’])
me mber/} aggregate 라 는 구 조 체 의 멤 버 인 지 체 크 한 다 . includes?} 지 정 되 지 않 았 다 면
defa 니 It-includes 가 사용된다.
예: AC_CHECK_MEMBER(struct passwd.pw_gecos, , [AC_MSG_ERROR([We

need 'passwd.pw_gecos’!])],[#include <pwd.h>])
다음과 같이 하위 멤버에 대해서도 사용 가능하다.
예: AC_CHECK_MEMBER(struct top.middle.bot)

autoconf 매크로 정리 775

===== PAGE 777 =====
AC_CHECK_MEMBERS(MEMBERS, [ACTION-IF-FOUND], [ACTION-IF-NOT-FOUND],
[INCLUDES = default-includes’])
members에 나열된 구조체 멤버 각각의 존재 유무를 앞에서 설명한 매크로를 사용해 체크
한다.
예: AC_CHECK_MEMBERS([struct stat.st__rdev, struct stat.st_blksize])

AC_STRUCT_ST_BLKSIZE
struct stat의 멤버로 st_blksize가 있다면 HAVE_STRUCT_STAT_ST_BLKSIZE를 define
한다.

AC_STRUCT_ST_BLOCKS
struct

stat의

멤버로

stjblocks가

있다면

HAW_STRUCT_STAT_ST_BLOCKS를

define

한다.

AC_STRUCT_ST_RDEV
struct stat의 멤버로 st_rdev가 있다면 HAVE_STRUCT_STAT_ST_RDEV를 define한다.

AC_STRUCT_TM
timeji에서 struct tm이 정의되지 않았으면 TM_IN_SYS_TIME을 define한다.

AC_STRUCT_TIMEZONE
struct tm의 멤버로 tm_zone이 있다면 HAVE_STRUCT_TM_TM_ZONE을 define하고, 그
렇지 않고 확장 배열에서 tzname을 발견한다면 HAW_TZNAME을 define한다.

8 타입 체크 매크로
AC_CHECK_TYPE(TYPE, [ACTION-IF-FOUND],[ACTION-IF-NOT-FOUND], [INCLUDES =
default-includes’])
TYPE이 정의되어 있는지 체크한다.

776 부록 D

===== PAGE 778 =====
..... .................... —.............. ................................ ...................................................... -■-■■- ...’"■■■———■-...........

C WECKjyPES(TYPES, [ACTION-IF-FOUND],[ACTION-IF-NOT-FOUND], [INCLUDES
= 'default-incl des’])

入

」

니

TYPES의 각 TYPE에 대해 정의되어 있으면 HAVE_TYPE을 정의한다. INCLUDES가 지정
되지 않았다면 default-includes를 사용한다. 타입이 찾아지고 ACTION_IF_FOUND가 주
어졌다면 실행된다. ACTION-IF-NOT-FOUND가 주어졌다면 타입이 찾아지지 않았을
때 실행된다.
예: AC_CHECK_TYPES(ptrdiff_t)

AC_CHECK_TYPES([unsigned long long, uintmax_t])

AC_TYPE_(3ETGROUPS
GETGROUP _T를 getgroups에 있는 array arg니merit의 기본 타입에 따라 gid_t 또는 int
로정의한다.

AC_TYPE_MBSTATE_T
wchar.h가 mbstate_t 타입을 선언하고 있다면 HAVE_MBSTATE_T를 정의한다. 또한
wcharh에서 mbstatej를 선언하고 있지 않다면 mbstatej를 타입으로 정의한다.

AC_CHECK_TYPE (mode_t, int)와 동일하다.

AC_TYPE_OFF_T
AC_CHECK_TYPE (off_t, long) 과 동일하다.

AC_TYPE_PID_T
AC_CHECK_TYPE(pid_t, int)와 동일하다.

AC_TYPE_SIGNAL
signal.h가 signal의 리턴 타입이 void형 function pointer로 선언되어 있으면
RETSIGTYPE을 void로 정의한다. 또는 int로 정의한다.
다음과 같이 RETSIGTYPE으로 signal handler를 정의한다.
예:

RETSIGTYPE hup_handler()
{
}
......

autoconf 매크로 정리 777

===== PAGE 779 =====
AC_TYPE_SIZE_T
AC_CHECK_TYPE(sizej, unsigned)와 동일하다.

AC_TYPE_UID_T
uid_t가 정의되어 있지 않다면 uid_t를 int나 gid_t로 정의한다.

0 C 컴파일러 특성 체크 매크로
AC_C_BACKSLASH_A
C 컴파일러가 \a를 이해한다면 HAW_C_BACKSLASH_A를 1로 정의한다.

AC_C_BIGENDIAN ([ACTION-IF-TRUE], [ACTION-IF-FALSE],[ACTION-IF-UNKNOWN])
빅 엔디안이면 ACTION-IF-TRUE를 실행한다. 리틀 엔디안이면 ACTION-IF-FALSE를
실행한다.
시스템 헤더 파일에서 빅 엔디안과 리틀 엔디안 여부를 확인할 수 없으면 test-case를 수
행한다. cross-compiling이면 test-case는 수행되지 않고 어떤 magic value를 grep을 통
해 집어낸다. 여부를 확인할 수 없으면 ACTION-IF-UNKNOWN가 수행된다.
예:

ACTION-IF-TRUE는 default로 ’WORDS_BIGENDIAN'으로 정의되어 있다.
ACTION-IF-FALSE는 default로 아무것도 하지 않는다.
ACTION-IF-UNKNOWN는 설정을 보류하고 인스톨러에게 이 테스트를 통과하려면 값을 설정해야
한다고 알린다.

AC_C_CONST
ANSI C qualifier 인 const 를 완벽하게 지원하지 않는다면 const 를 아무것도 아닌 것으로
정의한다.
어떤 C 컴파일러는 const 를 지원하기 위해 __STDC__ 를 정의하지 않는다. 어떤 컴파일러
는 const를 완벽히 지원하지 않기 위해 __STDC__를 정의한다.
때때로 인스톨러들이 C 코드를 컴파일하기 위해 C++ 컴파일러를 사용한다 (C 컴파일러가
부족하기 때문이다). 이것은 const 문제를 야기한다. C 와 C++ 는 const 를 다르게 취급하기
때문이다.
예: const int foo;
위 소스는 C에서는 해당되지만 C++에서는 해당되지 않는다.

778 부록 D

===== PAGE 780 =====
AC__C__VOLATII_E
C 컴파일러가 volatile 키워드를 인식하지 못한다면 volatile 을 아무것도 아닌 것으로 정의
한다. C 컴파일러가 volatile 을 지원한다면 프로그램에서 단순히 사용할 수 있지만 그렇지
않을 경우 Makefile 이나 configuration header 에서 아무것도 아닌 것으로 정의해야 할 것
이다. 프로그램의 정확성 이 volatile 에 의존하고 있다면 그것을 단순히 아무것도 아닌 것으
로 정의하는 경우 때때로 여러분의 코드를 망가뜨릴 수 있다. 그러나 컴파일러가 volatile 을
지원하지 않는다면 방법이 없다.
일반적으로 volatile 키워드는 ANSI C 의 특성 중 하나다. 그러므로 __STDC__ 가 정의되었
을 때만 volatile 키워드를 사용 가능하다는 것을 예상할 수 있다. 그러나 Ultrix 4.3’s 고유
의 컴파일러는 volatile을 지원하지만 __STDC__가 정의되어 있지 않다.

AC_C_INLINE
C 컴파일러가 inline 키워드를 지원한다면 아무것도 하지 않는다. 그렇지 않다면 inline을
_JnUne__이나 __inline으로 정의 가능할 경우 정의한다. 또는 inline을 아무것도 아닌 것
으로 정의한다.

AC_C_CHAR_UNSIGNED
C 타입인 char이 unsigned이고 C 컴파일러가 __CHAR_UNSIGNED__를 미리 정의하지
않았다면 __CHAR_UNSIGNED__를 정의한다.

AC_C_LONG_DOUBLE
C 컴파일러가 double 타입보다 좀 더 확실한 범위의 long double 타입을 지원한다면
HAVE_LONG_DOUBLE 을 정의한다.

AC_PROG_GCC_TRADITIONAL
GNU C 컴파일러를 사용하고 ioctl이 -traditional 없이 제대로 동작하지 않는다면
-traditional을 output varialble CC에 추가한다.

0 C++ 컴파일러 특성 체크 매크로
AC_PROG_CXX ([COMPILER-SEARCH-LIST])
C++ 컴파일러가 사용 가능한지를 가늠한다.

AC_PROG_CXXCPP
CXXCPP output variable을 C++ 전처리기를 실행하는 명령으로 설정한다.

autoconf 매크로 정리 779

===== PAGE 781 =====
IS 메시지 출력 관련 매크로
AC_MSG__CHECKING(feati/re-descr/pf/on)
diecking 메시지를 발생시킨다.

AC_M S G_RESULT(resu/t-description)
결과 메시지를 출력한다.

AC_MSG_NOTlCE(message)
notice 메시지를 출력한다. config니re : message 형식으로 출력된다.

AC_M SG_E RRO R ferror-description, [exit-status])
오류 메시지를 출력하고 configure 스크립트 수행을 중단한다.

AC_l\4SG_FAILUREferror-descr/pf/'o/7, [exit-status])
오류 메시지를 출력하고 configure 스크립트 수행을 중단한다. 그리고 “See 'configjog’

for more details.” 메시지를 출력한다.

AC_M S G_WARN (problem-description)
경고 메시지를 출력한다. configure 스크립트 수행은 중단되지 않는다.

780 부록 D

===== PAGE 782 =====
I 찾아보기 I

기호

-E 230

-\(- 321

-EB와-EL 388

-\) 321

：e file.txt 66

$(filter 패턴) 574

-e[name] 259

$ 키 67

——end—gro니p 332

—32 | —64 385

--end-group 옵션 322

-al 257

—entry 328

.align abs-expr 397

.equ symbol 400

-al 옵션 382

[esc] 키 65

-ansi 235

.EXPORT_ALL_VARIABLES 584

-as 257

.extern symbol 400

.ascii “string” 398

-falign-functions 251, 253

.asciz “string” 398

-falign-jumps 251, 253

__asm__지정어 405

-falign—lathis 251, 253

.bss 310

-falign-loops 251, 253

.bss 섹션 304, 314

-fbranch-probabilities 268, 269

.byte expressions 398

-fbran사!-probabilities 옵션을 이용한 분기 최적화

-c 230

266

- C 234

-fcaller-saves 250

.comment 310

-fcprop-registers 246

.ctors 310

-fcrossjumping 250

.data 310, 314, 400

-f cse-f o11ow-j u m ps 250

.datal 310, 314

-fcse-skip-blocks 250

.data subsection 400

-fdefer-pop 246

.data 지시자 393

-fdelayed-branch 246

.debug 310

-fdeIete-nuIl-pointer-checks 250

.DEFAULT 584

-fexpensive-optimizations 250

-defsym 382

-fforce-addr 281

.dtors 310

-fforce-mem 281

.dynamic 310

-fgcse 250

-dynamic-linker 317

-fgcse-after-reload 252

.dynstr 310

-fgcse-lm 250

- 이매크로] 232

-fguess-branch-probability 246

- D[매크로]늬매크로 값] 233

-fif-conversion 246

-e 328

-fif-conversion2 246

찾아보기 781

===== PAGE 783 =====
.fill repeat 398

-ftree-vrp 251

.fini 310

— f니nit-at—a—time 247

-finline 246

-

-finline-functions 252

-funswitch-loops 252

-floop-optimize 246

-fvpt 276

-f m e rge-co n sta nts 247

-

-fno-asm 238

.global symbol 399

-fomit-frame-pointer 278

.globl symbol 399

-foptimize-sibling-calls 250

.got 310

-fpeel-loops 옵션을 이용한 루프 최적화 271

.hash 311

funrolHoops 옵션을 이용한 루프 최적화 271

g 255

-fpeephole2 250

.hword expressions 398

-f pref etch-loop-arrays 253, 279

-

I 231

-

fprofile-arcs 268

-

I dir 옵션 384

-

f profile-gene rate 268

.ifdef symbol 〜 .else ~ .endif 402

-

fregmove 250

.if expression 〜 .else ~ .endif 401

-freorder-blocks 250, 253

.ifndef symbol 〜 .else 〜 .endif 402

-freorder-blocks-and-partition 253

.ifnotdef symbol 〜 .else 〜 .endif 402

-

freorder-functions 251

.IGNORE 561, 584

-

freru n-cse-after-loop 250

.include “file” 402

-frerun-loop-opt 250

-include ［헤더 파일 경로］ 232

-fsched-interblock 250

.init 310

-fsched-spec 250

.interp 311

-fschedule-insns 250

.interp 섹션 317

-fschedule-insns2 250

.int expressions 398

-

-

fstrength-reduce 250

I［패스］ 257

-fstrict-aBasing 250

-Igcc 318

-

-

-

fthread-jumps 250
ftracer 272

-ftree-ccp 247

lgcc_s 318

/lib/ld—linux.so.2 317
.line 310

-ftree-ch 247

.long expressions 398

-ftree-copyrename 247

-

-ftree-dce 247

-

I［라이브러리 이름］ 257

-ftree-domihator-opts 247

-

L 옵션으로 라이브러리 검색 321

-ftree-fre 247

-

I 옵션으로 링킹될 라이브러리 320

-ftree-lrs 247

-

M 259, 325

L［라이브러리 디렉토리］ 257

-ftree-pre 251

.macro name, arg, ■•• 〜 endm 402

-ftree-sra 247

-

-ftree-ter 247

-Map 옵션 325

-ftree-vect-loop-version 253

-march=ARCHITECTURE 386

782 찾아보기

mapcs ［26132］ 387

===== PAGE 784 =====
-march=CPU 385

*.s 396

-

march=［아키텍처 문자열］ 257

-S 230, 326

-

mcpu = PROCESSOR 386

*.S 396

— mfloat—abi=abi와• 一meabi=ver 387
- mfpu=［부동소수점 포맷］ 386

-save-temps 231

— mthumb과 -mthumb-interwork 387

-section-start 329

-mtune=CPU 385
- M과-MM 234

-shared 258

W 문자제거 136

shared 옵션으로 공유 라이브러리와 링킹 322

.section name 401
.set symbol 400

-nostartfiles 259

.short expressions 398

-nostdinc 234

.shstrtab 311

-nostdlib 259

.SILENT 560, 584

.note 311

-soname 370

—no-warn 257

.space size 399

-

00 243

—start-group 332

-

01 246

——start—gro니p 옵션 322

-

02 250

-static 258

-

03 252

-static 옵션으로 정적 링킹 321

--oformat 327

-std=［C 표준들］ 235

.org ［주소］, ［채울 값］ 403

.string “string” 398

-

.strtab 311

Os 253

-pedantic 242

.SUFFIXES 554, 584

-pedantic-errors 242

.symtab 311

-pg 256

.text 310, 400

-pipe 281

.text s니bsection 400

.pit 311

--trace-symbol 옵션 331

.PRECIOUS 584

-traditional 237

--print-map 325

-T［text|data|bss］ 329

: q 66

-

T ［링커 스크립트 패스］ 329

.relaNAME 311

-

U ［매크로］ 233

.relNAME 311

-

v 231

.rodata 310

—verbose 338

.rodatal 310

_volatile__키 405

.rodata 섹션 313

-

w 241

-rpath 327

:w 66

-rpath-link 327

-

-

R 옵션 384

-Wa,［as 옵션들］ 256

-

r 옵션으로부분링킹하기 323

-Werror 242

-

s 259, 326

-Wl, ［링커 옵션들］, -Xlinker『링커 옵션］ 259

W 257

찾아보기 783

===== PAGE 785 =====
.word expressions 398

AC_CHECK_HEADER 613, 774

-Wp,［옵션들］ 234

AC_CHECK_HEADERS 614, 774

:wq! 65, 66

AC_CHECK丄IB 611, 774

--wrap 옵션 329

AC_CHECK_MEMBER 619, 775

-Wtraditional 242

AC_CHECK_MEMBERS 619, 776

-Wunused 240

AC_CHECK_PROG 608, 772

-Wunused-function 240

AC_CHECK_PROGS 609, 773

-Wunused-label 240

AC_CHECK_TOOL 610, 772

-Wun used-para meter 240

AC_CHECK_TOOLS 773

-Wunused-value 240

AC_CHECK_TYPE 619, 776

-Wunused-variable 240

AC_CHECK_TYPES 619, 777

-Wwrite-strings 240

AC_C_IN니NE 779

-W과-Wall 239

AC_C_LONG_DOUBLE 779

-x 259, 326

AC_CONFIG_FILES 602

-X 326

AC_CONFIG_HEADER 632

-

\(옵션 321

AC_C_VOLATILE 779

-

\) 옵션 321

AC_DEFINE 621

스키 67

AC_FUNC_ALLOCA 618

키 67

AC_FUNC_CHOWN 618

-

: 키 63

AC_FUNC_CLOSEDIR_VOID 618

?키 63

AC_FUNC_ERROR_AT丄INE 618

/키 63

AC_FUNC_FNMATCH, AC_FUNC_FNMATCH

+ 키 67

GNU 618
AC_FUNC_FORK 618
AC_FUNC_FSEEKO 618

a, A, i, I, o, 0, s, cc 66
A티 (Application Binary Interface) 319
abs-expr 397
AC_CANONICAL_HOST 623
AC_CANONICAL_SYSTEM 623
AC_C_BACKSLASH_A 778
AC_C_BIGENDIAN 778
AC_C_CHAR_UNSIGNED 779
AC_C_CONST 778
AC_CHECK 612
AC_CHECK_FILE 620, 773
AC_CHECK_FILES 620, 773
AC_CHECK_FUNC 617, 775
AC_CHECK_FUNCS 617, 775

784 찾아보기

AC_FUNC_GETGROUPS 618
AC_FUNC_GETLOADAVG 618
AC_FUNC_GETMNTENT 618
AC_FUNC_GETPGRP 618
AC_FUNC_LSTAT_FOLLOWS_SLASHED
SYM니NK 618
AC_FUNC_MALLOC 618
AC_FUNC_MBRTOWC 618
AC_FUNC_MEMCMP 618
AC_FUNC_MKTIME 618
AC_FUNC_MMAP 618
AC_FUNC_OBSTACK 618
AC_FUNC_REALLOC 618
AC_FUNC_SELECT_ARGTYPES 618

===== PAGE 786 =====
AC_FUNC_SETPGRP 618

AC_PROG_FGREP 604

AC_FUNC_SETVBUF_REVERSED 618

AC_PROG_GCC_TRADITIONAL 779

AC_FUNC_STAT, AC_FUNC_LSTAT 618

AC_PROGJNSTALL 604

AC_FUNC_STRCOLL 618

AC_PROG丄EX 604

AC_FUNC_STRERROR_R 618

AC_PROG丄N_S 604

AC_FUNC_STRFTIME 618

AC_PROG_MAKE_SET 604

AC_FUNC_STRNLEN 618
AC_FUNC_STRTOD 618

AC_PROG_RAN 니 B 604

AC_FUNC_UTIME_NULL 618

AC_REPLACE_FNMATCH 618

AC_FUNC_VPRINTF 618

AC_SEARCH丄IBS 613, 774

AC_HEADER_DIRENT 615, 616, 774

AC_STRUCT_ST_BLKSIZE 776

AC_HEADER_MAJOR 616, 775

AC_STRUCT_ST_BLOCKS 776

AC_HEADER_STAT 616, 775

AC_STRUCT_ST_RDEV 776

AC_PROG_YACC 604

AC_HEADER_STDBOOL 616, 775

AC_STRUCT_TIMEZONE 776

AC_HEADER_STDC 616

AC_STRUCT_TM 776

AC_HEADER_SYS_WAIT 616

AC_SUBST 620

AC_HEADER_TIME 616

AC_TYPE_GETGROUPS 777

AC_HEADER_TIOCGWINSZ 616

AC_TYPE_MBSTATE_T 777

ACJNIT 601, 636

AC_TYPE_MODE_T 777

ACJNITdike, 0.0.1,-) 601

AC_TYPE_OFF_T 777

AC_INIT 매크로 645

AC_TYPE_PID_T 777

AC_MSG_CHECKING 612, 780

AC_TYPE_SIGNAL 777

AC_MSG_ERROR 612, 780

AC_TYPE_SIZE_T 778

AC_MSG_FAILURE 613, 780

AC_TYPE_UID_T 778

AC_MSG_NOTICE 612, 780

add 686, 721

AC_MSG_RESULT 612, 780

addprefix 578

AC_MSG_WARN 613, 780

addr2line 415

AC_OUTPUT 603

addr2line 명령 416

AC_OUTPUT_COMMANDS 623

addsuffix 578

AC_PATH_PROG 773

AMD 263

AC_PATH_PROGS 773

amdfamIO 263

AC_PATH_TOOL 773

AMD Family 10 core 263

AC_PROG_AWK 604

AM_INIT_AUTOMAKE 636

AC_PROG_CC 592, 604, 606

AMJNIT_AUTOMAKE 매크로 645

AC_PROG_CPP 592, 604

anj 니 ta 151

AC_PROG_CXX 604, 779

a.out 202

AC_PROG_CXXCPP 604, 779

a.out 바이너리포맷 296

AC_PROG_EGREP 604

ar 415

AC_PROG_F77 604

AR 548

찾아보기 785

===== PAGE 787 =====
ARFLAGS 548
as 415

c3 263

AS 548

c3-2 263

ASFLAGS 548

c89 또는 iso9899：1990 236

Assembler Option 223

c99 또는 iso9899：1999 236

assembly 기본 사용법 389

calendar.vim 125

AST (Abstract Syntax Tree) 182, 183

call 명령 476

as에 의한 기계어 코드 생성 202

CC 548

as의옵션 256

cd 164

athlon 263

ccl C 컴파일러의 옵션 235

Athlon 263

cd -E 또는 cppO 전처리기 옵션 231

athIon-4 263

ccl—E 명령 164

Athlon 4 263

cc1ph」s 164

athlon64 263

ccl 에 의한 어셈블리 소스 파일로 컴파일 177

Athlon 64 263

ccl 전단부에서하는일 179

athlon-fx 263

ccl 중단부에서하는일 192

Athlon FX 263

ccl 후단부에서하는일 198

athlon-mp 263

Celeron 263

Athlon MP 263

c++filt 415

athlon-tbird 263

c++filt 명령 416

athlon-xp 263

CFLAGS 548, 640

Athlon XP 263

checkout 676, 716

attach 명령 482

C_INCLUDE_PATH 282

attach와• detach 513

C++ Language Options 220

autoconf 44, 591, 592, 597, 602

C Lang니age Options (仁이의 front-end 옵션)

a니toheader 명령 629

219

automake 44, 591, 635

clean니p 695

a니toscan 598

CO 548

autotools 44, 591

Code Generation Options 225
COFF 202, 296
COFF 포맷 296

BASE 682
basename 578
bindir 640
bin_PROGRAMS 639
blame 684
bufexplorer.vim 126

COFLAGS 548
collect? 164
c이ect2 또는 Id의 옵션 257
collect2에 의한 링킹 과정 208
commit 677, 717
comm symbol 400
COMPILEFLPATH 282
condition 443

786 찾아보기

===== PAGE 788 =====
config.h.in 629

default.Ids 338

config.h 파일 629

DEFS 640

config니re 592

d 이 ete 686

configure.ac 592, 598, 599, 601, 623,

df： diff-full 699

626, 629

diff 명령으로 변경된 내용 비교 682

C-only Warning Options 221

dir 577

copy 690, 694
COPY 345

Directory Options 223
disas 475

core2 263

display 메뉴 511

Core2 Duo 263

dnl 594

CPLUS_INCLUDE_PATH 282

DSECT 345

CPP 548

dump/load 695

cppO 164, 175

DWARF2 255

CPPFLAGS 548, 640

DX/SX/CX 263

CPU는어떻게 만들까? 162

DX/SX/DX2 263

cscope 104

DYNAMIC 304, 308

ctags 104

DYNSYM 308

ctags 명령 요약 109
ctags 설정 105
CTANGLE 548
CVS 서버실행 709
CVS 서버에로그인 711
CVS 소개 705
CWEAVE 548
CXX 548
CXXFLAGS 548, 640
cygn니s 638
C 소스에서 컴파일된 어셈블리 391
C 소스의전체컴파일 과정 163
C 언어옵션 235

13
ed 59
e： edit 700
ELF 202
ELF 바이너리포맷 295
ELF 바이너리 포맷 구조 202
ELF 헤더 297, 299
emacs 145
emacs의 장단점 146
ENTRY(symb이) 353
ENTRY 명령 342
ERROR 612
exec_prefilx 640

13

ex(EXtended editor) 59

DATA 643

export 689

datadir 640

export되지 않는 심볼 326

ddd 501

export 키워드 567, 568

DDD를 사용한디버깅 501

expression 348, 400

ddd에서브레이크포인트 506
Debugging Options 221

찾아보기 787

===== PAGE 789 =====
Gimplify 183
FC 548

glade 746

FFLAGS 548, 640

gnits 638

file 660

gnu 638

fill 399

gn 니89 237

filter 함수와 반대로 패턴과 일치하지 않는 문자열 575gnu99 237
findstring 575

GNUmakefile 538

firstword 576

gprof 415

foreach 579

gprof로 프로파일 정보 알아보기 418

foreign 638

G 키 68

gas 377

HASH 308

gas assembler 필수 지시자 397

HEAD 682

gcc-3.2.2 의전처리과정 175

HEADERS 642

gcc C 컴파일러 드라이버 옵션 230

HIPROC 308

gcc는 GNU C Com이er의 약자 163

HIUSER 308

GCC는 GNU Com에er Collection의 약자 163

h, j, k, I 키 67

gcc를 이용한 최적화 컴파일 260

htpasswd 666

gcc 옵션 분류 218
gcc 옵션적용규칙 226
gcc 컴파일 속도 최적화 281
gcc 필수옵션 230
gcov 428
gdb 435
gdb로 간단한디버깅 436
gdb를 이용한 디버깅 테크닉 479
gdb에 대한 소개 435
gdb의 시작과 종료 438
gedit 149
generic 263
genericize 182
GET 548
GFLAGS 548
gg 키 68
GIMPLE 트리 vn, 179
GIMPLE 트리를생성 182
GIMPLE 트리확인 187
gimple 파일 189

788 찾아보기

i386 263
i486 263
i586 263
i686 263
IA32/AMD64 263
IDT Winchip2 263
IDT Winchip C6 263
ifdef 〜 else 〜 endif문 570
if eq 〜 else 〜 endif 문 569
ifeq문 569
ifndef ~ else 〜 endif문 570
ifneq 〜 else 〜 endif문 569
ifneq문 569
ignore 444
I, i, A, a, 0, o, s 키 64
import 674, 714
includedir 640

===== PAGE 790 =====
INFO 345

니 BRARY_PATH 283

infodir 640

니BS 640

info frame 462

like.c 컴파일메시지 167

INSERT_CODE 630

likeU 19

INTERP 304

Linker Options 223

i 키 64

니SP 643

I (list) 명령 440
LMA(Load Memory Address) 344
join 576

LOAD 304
lock/unlock 687
log 681

13

LOPROC 308

k6 263

LOUSER 308

K6 263

LT니BRARIES 642

k6-2 263

Itrace 523

k6-3 263
K6 II 263
K6 III 263
k8 263
K8 263
KDevelop 150

m4 매크로 처리기 595
Machine Dependent Options 224
machine instr니ction 155
MACRO 573
main.cpp 파일 생성 744
make 533

Language Independent Options 220

makefile 534, 538

Id 415

Makefile.am 635, 639

LD 548

Makefile.in 615

Idconfig 372

Makefile 파일생성 745

LDFLAGS 548, 640

MAKEINFO 548

Id를 사용한 기본적인링킹 315

Makfile.in 635

Id를 사용한링킹 315

ma(marking a) 101

Id를 사용한 애플리케이션 최종 링킹 316

mandir 640

length 400

man page의 활용 122

LEX 548

MANS 643

LFLAGS 548

map 명령 91

libdir 640

me： mine-conflict 700

libexecdir 640

meld 684

libm.a 라이브러리 24

MEMORY 명령 346

니BRARIES 642

merge 692

찾아보기 789

===== PAGE 791 =====
El

prefix 640

nm 415, 420

Preprocessor Options 223

NOBITS 308

prescott 263

nocona 263

PROG히TS 307

NOLOAD 345

PROGRAMS 641

notdir 577

PT_DYNAMIC 348

NOTE 304, 308

PTJNTERP 348

NULL 304, 307

PT_LOAD 348
PT_NOTE 348
PT_NULL 348
PT_PHDR 348

OBJC_INCLUDE_PATH 282
objcopy 415, 422

PT_SHLIB 348
p： 다음에 시도 697

objdump 157, 415, 423
Objective-C and Objective-C+ + Language
Options 220
opteron 263

QT 디자이너 738

Optimization Options 222
origin 580
Overall Options (gcc 컴파일러 드라이버 옵션)
219
OVERLAY 345

■3
ranlib 415
readelf 415, 426
REL 308
RELA 308
remove 721

pats니 bst 572

REMOVE_CODE 630

PC 548

rename 687

pentium 263

revert 688

Pemtium 4M 263

RM 548

pentium2 263

RTL(Register Transfer Language) 177,182, 196

pentium3 263

RTL 생성 196

pentium3m 263

RTL 최적화 199

pentium4 263
Pentium III 263
pentium-m 263
Pentium M 263
PentiumMMX 263
pentiumpro 263
PFLAGS 548
PHDR 304

790 찾아보기

sbindir 640
SCRIPTS 643'
SECTIONS 342
set listsize 20 441
SH니B 304, 308

===== PAGE 792 =====
signal 명령 477

TEX 548

size 398, 415, 427

TEXI2DVI 548

sort 573

TEXINFOS 643

SOURCES 642

top_srcdir 640

specs 파일을 이용한 gcc 설정 283

trace 유틸리티 517

splint 524
srcdir 640
SSA(Static Single Assignment) 192, 193

El

SSE(Streaming SIMD Extension) 데이터 타입

update 679, 719

지원 157

static 변수 314
status 685

D
valgrind 527

strace 517

value 398

strings 415, 427

vi 59

strip 415, 427, 574

Via C3 263

STRTAB 308

Via C3-2 263

SUBDIRS 641

Vi Improved 61

SUBDIRS 매크로 64
6

vim 19, 61

subsection 401

vimdiff 683

subst 572

vimspell 128

S니bversion 656, 671

vim 내장 스크립트 작성 110

Subversion을 사용하려면 먼저 671

vim 설정 파일에 키 매핑 91

suffix 577

vim 의기능확장 124

svn 36, 661

vim 정규 표현식 79

svn + http 661

vim 확장 정규 표현식 87

svn import 37

Visual edit 59

svnserve 661, 668

VMA 344

svn+ssh 661

VPATH 562, 566

SYMTAB 307
sysconfdir 640
s： 모든 옵션 700

ICT
WEAVE 548
Widget 생성 740

D

wildcard 579

taglist 127

winchip2 263

tags 파일 106

winchip-c6 263

TANGLE 548

word 576

Target Options 224

word list 576

tcpdump 755

words 576

tc： theirs-conflict 700

w 명령 65

찾아보기 791

===== PAGE 793 =====
x/ 473

다중 창 명령 요약 98

x/10i 474

다중창 사용하기 95

Xeon 263

단축키를 매핑 (mapping)할 때 사용 91

XIP 기법 358

더미 타겟 558
데드 코드 제거(Dead Code 티imination) 251
되돌리기와 되살리기 74
디버깅옵션 254

YACC 548
YFLAGS 548
라이브러리 디버깅 493
라이브러리 체크 매크로 610

ZZ 66

레이블(label) 292
레지스터 71, 513
레지스터의값 출력 453

각종 섹션의 종류 307

레지스터 할당 vn, 200

간단한 링커 스크립트 338

레지스터활용을 통한최적화 281

개발자들의 vim 설정 139

루프 불변 이동(loop invariant code motion)

개별 변수의 값 출력 452

247

경고옵션 239

링커 스크립트 335

공백문자의제거 574

링커스크립트 기본 문법 342

공유 라이브러리 211, 369

링크맵 325

공통 부분식 제거(Common S니bexpression

링킹 과정 절차 289

Elimination) 251

링킹의기본 이해 289

구문분석 180
구조체 배열을 출력 454
균등분할된상태 98
기계종속적인부분 182
기술파일 534
기술파일 구문 작성 기본규칙 540
기술파일의기본 구조 539
기타유용한함수 579
기타 중요한 지시자 401

마지막 글자로이동 67
마킹 관련 명령 요약 102
마킹으로이동하기 99
매칭문자 139
매크로 542
매크로의 사용 94
머신 종속적인 옵션을 이용한 최적화 260
멀티스레드 프로그램 디버깅 488
멀티프로세스 프로그램 디버깅 484

내부적으로 정의되어 있는 매크로의 사용 547

메모리 513

넌터미널 (non-terminal) 183

메모리 상태 검사 473

네임 레지스터 92

명령라인 모드 62, 65

792 찾아보기

===== PAGE 794 =====
명령사용규칙 558

섹션 뷰 298

목적코드생성 201

섹션헤더 구조체 305

문서의 마지막 위치로 이동 68

섹션 헤더 테이블 304

문서의 맨 처음으로 이동 68

셸(shell) 명령 155

문자를정렬하는함수 573

셸명령사용 102

문자열 처리 함수 572

소스 빌드 750

문자열 치환 75

소스충돌 해결 720

문자열 탐색 74

소스태깅 731

문자열 탐색과 치환 78

수직 분할 96

문자 필터링 함수 574

수평 분할 96
스레드 513
스캐너 180

바이너리유틸리티 415
바이너리포맷 202
반도체 160
반복되는 문자열을저장 92
백트레이스 442
버전관리 653
변수값설정 458
변수와 레지스터 값 검사 451
복사와붙이기 70

스택 513
스택 재정렬 (stack realign) 157
스택프레임 464
스택 프레임에 있는 정보를 이용해 디버깅 469
실행 중인프로세스디버깅 482
심볼 관련 지시자 399
심볼대입 342
심볼 대입 명령 351
심볼정보 제거 326

부분링킹 323
브랜치 732
브랜치한 소스머지하기 733

아키텍처 비종속적인 최적화의 리스트 195

브레이크포인트 441

어셈블러인 as 164

블록지정 72

어셈블리 155

블록 지정 후 사용 가능한키 73

어셈블리언어 155

빠른괄호 이동및빠른탐색 130

어휘분석 180
언어종속적인부분 182
에디트 환경 변수 설정 671

사용 가능한 매크로 603
삭제 70
삭제와 관련된키 70
설정 헤더를 사용해 소스 파일에 설정 적용 627
세그먼트뷰 298
세그먼트영역 298
섹션 298
섹션 관련 지시자 400

엔트리포인터설정 328
여러디렉토리를컴파일 566
여러파일을편집하는방법 88
여러행탭끼워넣기 133
오버레이 기술 342
와치포인트설정 449
윈도우구성 748
의미분석 181
이동 61, 67

찾아보기 793

===== PAGE 795 =====
이벤트 핸들러 등록 749

중단부 (middle-end) 177

이벤트핸들러설정 742

중단부에서하는일 177

이클립스 147

지역 레이블 395

이클립스의장단점 148

지역마킹 (a-z) 100

인라인 확장 245

지역 심볼 326

인스트럭션 155

지역심볼 제거 326

인스트럭션스케줄링 177
읽기 전용 데이터 공간Crodata 섹션) 158
입력 61, 66
입력 모드 62, 66
입력모드전환키 66
입력 섹션 기술 350

창 간 커서 전환 96
창을 분리해사용 514
창을최대로하는명령 97
초기화되지않은전역변수 314
초기화된데이터 314
최적화옵션 242

자동 완성기능 139

출력 섹션 기술 342

자동으로디스플레이하기 459

출력 형식의 지정 456

잘라내기 71

충돌에관한해결법 696

재귀적 Makefile.am 파일 작성 644

치환명령 78

재귀적 make의 사용 562
재배치 (relocation) 292
재배치 가능한 오브젝트 323
저장 61
저장 및 종료 66
저장소(repository) 36
저장후종료 65
전단부 (front-end) 177
전단부에서하는일 177
전역마킹 (A-Z) 100

커널로더(execveO 202
커서 이동 67
컴파일 745
컴파일러드라이버 164
•코드 생성기 (Code Generator) 201
코어 (core) 439
코어파일을이용한디버깅 479

전처리과정 164
전처리기 164
전체 변수의 값 출력 451

타입을변환해출력 457

정규표현식 78

탭사이즈 조정 133

정렬 지시자 397

토큰 180

정적라이브러리 209

특수 내장 타겟 560, 561

정적 라이브러리 만들기 365

특수 타겟 554, 584

제일처음글자로이동 67

특수 함수 매크로 618

조건부 수행 568, 569

특수 헤더 파일 매크로 616

중간표현 179

특정 문자열을 찾는 함수 575

중간 표현생성 182

794 찾아보기

===== PAGE 796 =====
특정 변수를 지정해서 출력 455
특정 위치 지정 457
특정한 행으로 이동 69

할당지시자 398
함수사용법 568
함수 사용할 때 주의 사항 582
함수의 사용 570

파서 (parser) 180
파스트리 181
파일 버퍼 89
파일 버퍼 관련 명령 90
파일에서 달라진부분 137
파일 열기, 저장, 종료 63
파일 이름 관련 함수 577
파일탐색 기능 활용 130
편집 61, 70
포인트변수의값 출력 452
폴딩기능이용 131
표준모드 62

함수체크 매크로 616
함수 프레임포인터제거 276
핸들러 함수 내용 추가 752
행번호보여주기 135
헤더파일바로읽어오기 138
헤더 파일 체크 매크로 613
형상관리 653
형식 언어 155
확장자규칙 551
후단부 (back-end) 177
후단부에서는 아키텍처 비종속적인 최적화 177
흐트러진소스 134

표준모드 상태 64
표준 모드 이동키 종합 69
프로그램 결정 매크로 603, 604
프로그램실행 446
프로그램 헤더 구조체 302
프로그램 헤더 테이블 301
프로젝트 디렉토리 정리 671
프로젝트파일관리유틸리티 25
프로파일 결과를 이용한 최적화 265
프리패치 (prefetch)를 이용한최적화 279
플러그인 104, 124

찾아보기 795
