---
source_url: /run/media/yutae/Data/리눅스 커널 소스 해석_기초입문.pdf  # USB PDF (local-only; raw/books/linux-kernel-source-beginner.pdf gitignored)
ingested: 2026-11-01
sha256: 6dbe600a0a79255f539b7930ccd60dba2e380a3870693429ef4d81ebb5ebaa40
---

# 리눅스 커널 소스 해석 [기초입문] (raw source)

## Book metadata
- **Title:** 리눅스 커널 소스 해석 [기초입문]
- **Original:** (자작, 한국 원서)
- **Authors:** 정재준 지음
- **Korean publisher:** 커널연구회
- **ISBN (KR):** 978-89-97750-13-9
- **Year:** 2020
- **Pages:** 353 (pdfinfo)
- **kind:** text-layer (pdftotext extraction 2026-10-30)

## Body
최신 리눅스 커널 소스를 단계별로 쉽게 풀어서 설명하는




라밗耀쑈牲胚입문
            First Edition




        小七以「（d 놉 정쟤左
                                  리눅스 커널 소스 해설 ［기초입문］
                                  리눅스 커널 소스 해설 ［기초입문］




        최신 리눅스 커널 소스를 단계별로 쉽게 풀어서 설명하는



리눅스 커널 소스 해설［기초입문］




                  커널연구회 佃w'肌kernel.b기

                 정재준 (rg벼3307@nate.com)




커널연구회（小쌔,w.kerne比z)                    정재준（띠bi3307@nate.com)
                         1/ 351
                                             리눅스 커널 소스 홰별 E기麥입문］
                                                             저작권




저작권

                               리눅스 커널 소스 해썰［기초입문］


旨料牙君已，’于「 二1'                   저자 정재준

于                               Copyright (c) 커 널연구회（蜘／w.kernel.b기．

                                Put川shed by 커 널연구회 佃川w.kernel.bz).




          !.m4
r7} riC毛니rd ！셧 섣；7心




커널연구회는 리눅스 커널과 자료구조 알고리즘을 연구하고 리눅스 시스템 프로그래밍 및

디바이스드라이버 개발을 통하여 창의적인 프로젝트를 수행하여 임베디드 관련 제품들을 만들어

일상 생활을 풍요롭고 편리하게 하는데 가치를 두고 있습니다. 아울러 관련 기술들을 교육하여

여러사람들과 공유할 수 있도록 노력하고 있습니다. 커널연구회가 연구 개발한 결과물들은

체계적으로 문서화하여 온라인佃,ww.kernel. 뇨）상어나］ 무료 훅은 유료로 제공하고 있습니다．

커 널연구회가 제공하는 저작물어七 저작권을 표시하고 있으며 사용자는 저작권 표시를 보존해 주어야

합니다. 커널연구회가 유료로 제공하는 저작물은 사용자에게 개인키（암호）를 부여 하므로 개인키를

타인에게 공개 및 양도하는 일이 없도록 해야 합니다. 기타 자세한 내용들은 커널연구회 웹사이트

(＼人／
   ＼八／
     ＼八／
       .kerneL.b기를 방문하1 주시기 바랍니다．

감사합니다．




커널연구회佃iww.kern臥.bz)                                 정재준（I야)i3307（孕nate.com)
                                2/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                          저작권




ISBN

  .   리눅스 커널 소스 해설 ［기초입문］

  S 저자정재준



  .   발행인：정재준

  .   발행처：커널연구회

  .   출판사등록번호：제 2011-75 호

  .   출판사등록일：201] 년 09 월 27 일

  .   전화：0引－592-0478／팩스：03下594-5307

  .   발행일：2020 년 03 월 ]0 일




          !
                             歇 28,000원
                              93560H




      9 788997 '750139
        ISBN 978욘9꾼7750녀3순




 커널연구회佃쌔,w.kerne나끄）                           정재준（rgbi3307@nate.com)
                                 3/ 351
                                                 리눅스 커널 소스 해설 E기초입문］
                                                                 저작권



저자 소7H

정재준 (rgbi3307@nate.com)

커널연구회（놔出w.kerneLb지



저자는 리눅스 커널과 자료구조 알고리즘 관련 서적 집필과

세미나, 교육, 공유 활동을 활발히 하고 있습니다. 자료구조

알고리즘 연구 결과물로 특허 등록한 "맞춤형 문장 자동 번역

시스템 및 이를 위한 데이터베이스 구축방법 (The System for the customized automatic

sentence transla匕on and database construction method)"이 있습니다. 저자가 컴퓨터구조와

리눅스 커널, 자료구조 알고리즘 효율성, 머신러닝에 대해서 연구한 결과물들은 커널연구회 웹

페이지에 공유하고 있습니다. 최근에는 리눅스 커널 소스 patchwork.kerneLorg 를 통해서 RISC-V

구조에 기여하고 있습니다. (h比ps://patch니／ork.kern이.org/pr이edt/Li nux-riscv/List/)




커널연구회（的／姚／.kerne나）기                                     정재준（rgbi3307@aate.con力
                                    4/ 351
                                  리눅스 커널 소스 해설 ［기초입문］
                                                  머리말




머리말

우리의 삶은 서로 연결되고 융합되어 있습L따．

이 세상에 존재하는 모든 것들은 원소단위로부터 유기물 세포로 연결되고 융합되어 유전자를 통해서

스스로 자가 증식할 수 있는 생명체들로 진화하고 소멸. 윤회를 반복하고 있습니다. 사람은 이러한

과정을 이해하기 위해서 노력하는 가장 진화된 뇌세포를 가지고 있습니다. 그동안 철학적으로

막연하게 인지하고 있었던 생명 활동 과정을 논리적으로 분석하는 기초자연과학（수학, 물리. 화학，

생명과학）의 도움으로 이제는 좀더 구체적으로 실증하는 단계로 발전하고 있습니다. 이렇게

자연과학이 지속적으로 발전하는 과정에서 중간중간 개발되는 공학적인 산물들은 우리의 삶을 더더욱

윤택하게 하고 있고. 또다시 자연과학을 발전시키는 촉매제 역할을 하고 있습니다. 이러한 과정이

서로 연결되고 융합이 잘 되도록 도와주는 촉매제 역할을 하는 것으로서 정보기술분야의 컴퓨터가

있습니다．



이제 컴퓨터는 우리의 생명활동을 도와주는 도구로 자리잡았습니다．

앞으로 이것을 잘 활용하는 것은 우리의 가치이며 모든 생명들을 이롭게 하는 방향으로 서로 연결하고

융합해야 합니다. 그러기 위해서는 기본에 충실해야 합니다. 기본은 생명에 대한 관심과 사랑입니다．

컴퓨터는 생명이 더불어 잘 살아갈 수 있는 환경을 만들71 위해서 생명의 본질을 이해하는 도구로

사용해야 합니다. 앞에서 언급한 생명에 대한 관심. 철학, 자연과학, 공학들은 기본 원리를 설명하기

위한 대상을 논리적으로 정리하는 단계부터 시작 해야 합니다. 이것이 컴퓨터 공학에서 이야기하는

자료구조 알고리즘입니다. 자료구조는 처리 대상물에 대한 데이터를 효과적으로 수납하는

저장소이며 알고리즘은 이것을 효율적으로 처리하는 계산적인 절차입니다. 컴퓨터의 기본원리는

자료구조 알고리즘이며 이것을 잘 연결하고 융합하면 우리의 삶을 좀더 윤택하게 하는 보람으로 다가

옵니다．




 커널연구회（小쌔쌔／.kerne比z)                    정재준（r아出330가會nate.com)
                         5/ 351
                                                                     리눅스 커널 소스 해설 ［기초입문］
                                                                                     머리말




커널연구회가 연구활동 하고 있는 리눅스 커널은 논리적인 철학으로 이루어진 자료구조 알고리즘의

집합체이며 컴퓨터에게 생명을 불어넣는 작업입니다. 커널연구회의 로고에는 이러한 정신이 새겨져

있습니다. 커널연구회가 지향하는 활동어는 몇가지 기본적인 소양과 학습 지식이 필요합니다. 이것을

커널연구회는 연구개발 로드맵, 학습 및 교육 활동의 지표로 정리했습니다．




                              커널연구회佃川w.kerneibz) 연구恥듕 로드뼙 （키워드）

                 穹烈釜哥 톄이터자료구조                                   알고리즘
                                                                코딩기법
                                                                                     입출력
                                                                                   인 터째이 스
               OpenCV, Python        카메라 영상, 자연어            Computer Vision          Sensor
     혐얹 蔓로쩍트
       斛스揮作f     C/C++ Library        Data M的eling          CNN, RNN, L釘！너           Camera
      x磁客 墅箋
                 CodeBlocks           Neural Netwrok       卜4atrix Operat幻ns         Sound

               gcc, glibc, wringpi     array, list, tree     process, fork      O口en, close, i야LI
     리뇩스 시스뎀
      프望교래밍
                  CodeBlocks           malloc, mmap         pthread_create       read, write, poii

               gcc extension, git     bitmap, kobject          clock, time         mm, fs, net
               make meriuconhig       proc, sys, page         task, kthread          lock, 仟（a
               penf, crash, debug     list, tree, xarray       sched, CFS       pcpu, workqueue
                    module           sysis, c야吼from_            sys_ioctl              char
                 device, probe        dev, device tree         sysfs-ops              block

                    STM32            Analog/D呼tat, A｛乂           Serial          12C, SPI, TCP/IP

                 CubeMX, IDE          Timer, Duty Rate          Pr야or이          RS422/485, PWM

                Compiler, GCC        哺이El 타입 , 포인터           loop, list, tree   data input/output

                  CodeBlocks         {｝再모리 , 배열, 구조처i         함수, 매크로            file read/write

               x86, AR卜& F기SC八／            명령셋                                      register
                                                            인라인 어셈暈리
               ALU, SMP, NUMA         opcode, operand                              load, store

                 연 구개발 횐겅                                                            입출력
                  St격（. IDE           텍이터 자료구조
                                                                                   쉰E｛嚼혀스




기타 자세한 내용들은 커널연구회（的쌔／.kernel.bz) 웹페이지 참조 부탁 드립니다. 감사합니다．




커널연구회佃쌔,w.kerne나끄）                                                              정재준（rgb13307@n就e.Com)
                                                6/ 351
                                리눅스 커널 소스 해설 ［기초입문］
                                                 목차




모ii.
-I r- I




Table of Contents

. 리눅스 커널 소스 하썰［기초입문］                                     ]

. 저작권                                                    2

  ISBN                                                   3

  저자 소개                                                  4

S 머리말                                                    5

S 목차                      "                              7

S 커널 소스 빌드 및 버전관리                                       13

  커널 소스 다운로드                                            ]6

  커널 소스 빌드 및 설치                                         20

  커널 소스 버전업                                             27

S커널 소스 코딩 형식                                            32

  들여쓰기                                                  33

  긴줄과 문자열 나누71                                          34

  괄호와 공백 배치                                             35

  공백                                                    37

   작명                                                   39

   타입 재정의                                                40




         ．蛇me나玘）
 커널연구회（艸쌔／                          정재준（rgbi3307@nate.com)
                       7/ 351
                                 리눅스 커널 소스 해설 ［기초입문］
                                                  목차



 함수들                                                         41

  goto사용                                                     42

  주석문                                                        44

  Macros, Enums.                                             46

  커널 메세지 출력                                                  47

  메모리 할당                                                     48

  inline 함수                                                  48

  함수 반환값.                                                    49

  boot사용                                                     49

  커널 매크로 활용                                                  so

  Inline assembly                                            50

. ccc확장속성（attributes)                                        51

.커널 데이터 타입 이해                                                57

.커널 비트 단위 연산                                                 78

. 커널 비트맵 이해                                                 94

.커널 모듈 프로그래밍                                               106

. 커널 sort 테스트                                              116

. 커널 성능측정 도구                                               122

 penf설치하기                                                   ]23

 perf활용하기                                                   ]27

 perfrecorci                                               130




커널연구회佃쌔쌔,.kerc泡.bz)                  정재준（rgbi3307（亘）niate.com)
                        8/ 351
                                 리눅스 커널 소스 해설 ［기초입문］
                                                  목차



  perf report                                          132

 perf probe                                            135

 pe汗소스 빌드하기                                            ]37

0ftrace 활용                                             ]39

 추적 가능 항목들                                             ]41

 이벤트 단위 추적                                             ]45

 함수 단위 추적                                              147

 함수 그래프 추적                                             ]50

 I trace 중요 옵션들                                        ]53

1crash 도구 사용                                           ]54

  crash 설치하기                                           ]55

  crash 실행띠ye)                                         157

  crash 실행（덤프파일）                                       162

  crash 명령에                                            168

    backtrace 명령                                       170

    PS 명령                                              ]72

    struct 명령                                          ]74

     task 명령                                           ]77

     vn) 명령                                            ]79

     kmen) 명령                                          ]81

     sym 명령                                             ]83

     p 명령                                              184




 커널연구회（小쌔쌔／.kernel.뇨）                정재준（rgt好307@nate.com)
                        9/ 351
                                           리눅스 커널 소스 해설 ［기초입문］
                                                            목차


    List 명령                                                         186

     tree 명령                                                        ]86

     foreach 명령                                                     ]87

1kprobes 이해                                                         ]88

1debug objects 이해                                                   ]97

  debug objects7II념                                                 198

  debug ob忙cts함수들                                                   200

    debug_objects_earLy_init()                                      200

    debug_object_init()                                             203

    debug_object_f ree()                                            205

    debug_object_activate()                                         206

    debug_object_deactivate()                                       208

  debug objects활용                                                   210

S 커널 디버그 메세지 출력                                                     216

  메세지 출력 레벨 조정                                                      216

  다이나믹 레벨 조정                                                        219

1kobject 이해                                                        221

0user c이가테스트                                                       235

  커널 메모리 주소 이해                                                      236

  메모리 user copy실습                                                   241

1list sort 테스트                                                     248

  커널 니nked Li就 개념                                                   249



커널연구회（www.kerneLbz)                            정재준（rgbi3307@ nate.com)
                                 10/ 351
                                   리눅스 커널 소스 해설 ［기초입문］
                                                    목차



  커널 니stSo比 예제                                            253

0red-black tree 테스트                                       259

  red止乂ack tree 이해                                        260

  red-black tree 실습 예제                                    264

  노드 삽입. 삭저1 테스트                                          267

 노드 탐색 테스트                                                271

.커널 XArray 이해                                             274

  XArray구조체 정의                                            281

  XArray 테스트 모듈                                           286

  radix tree 테스트                                          290

    radix_tree_init()                                     296

    xarray_tests()                                        300

    regressionl_test()                                    301

    benchmark()                                           304

  rad以 tree 테스트 모듈                                        305

이DR, IDA관리                                                308

  idr, Ida 구조체                                            309

  k打할당                                                    312

  idr 테스트                                                 引4

  Ida 테스트                                                 317

0percpu 이해                                                321

  ELF Sections 이해                                         321




 커널연구회佃쌔／＼사．kerneL.bz)                 정재준(rgbi330끄＠nate.com)
                         11/ 351
                               리눅스 커널 소스 해설 ［기초입문］
                                                목차



 percpu 정의 하기                                       330

 percpu 사용 하기                                       333

S percpu 소스 분석                                      342

 percpu구조체                                          342

 pcpu 함수 실행 흐름                                      347

S 참고 문서                                             349




커널연구회佃,ww.kerne나끄）                 정재준似樊躬307@aate.con介
                     12/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                           커널 소스 빌드 및 버전관리




커널 소스 빌드 및 버전관리


        人
                                   이번글의 주제는 "리눅스 커널 소스 빌드 및 버전관리" 입니다．

                                   리눅스 커널은 버전관리 도구로 이t 을 사용합니다． 그래서

      Kernel Build Install         이번글을 읽기전에 이t 에 대해서 사전지식이 좀 있어야 합니다．

  ”거万                              리눅스커널과마찬가지로이t또한무료로설치 됩니다． 보통

                                   리눅스 우분투 배포본을 설치하면 기본적으로 설치되어

있습니다. 이t 사용법은 인터넷에 많은 정보들이 공개되어 있으므로 참고하여 익혀 주시면 되겠습니다．

저는 이글을 읽는 독자분들이 이t 기본 명령어는 어느정도 알고 있다는 가정하에 커널 소스 빌드 및

버전관리에 대해서 설명하도록 하겠습니다．



먼저 제가 실습하고 있는 PC（노트북）환경은 다음과 같습니다．



PC（노트북）환겅


  1    CPU: Inte1(R) Core(TM) 13-7100U CPU @ 2.40GHz
  1     RAM: 8GB
  1     OS: Linux ubuntu 18.04
  1     Kernel: v4.20 ... v5.5
  1     9cc: version 7.3.0
  1     Target: x86_64-linux-gnu



나nuxubuntu 18.04 이상 버전에서는 gcc 가 기본적으로 7.3 이상 버전이 설치되어 있기 때문에 gcc

을 업그레이드 하지 않아도 됩니다. 혹시, gcc vers向n 이 7.3 이하 버전이라면 다음과 같이 gcc을

업그러1이드합니다.                                        3 1Ik   ＼卜'3




 커널연구회（w艸／.kernel.뇨）                                        정재준（rgbi3307@nate.com)
                                        13/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                       커널 소스 빌드 및 버전관리




으cc업그래이드
$ sudo add- apt- repository ppa: ubuntu- toolchain- r/ test
$ sudo apt- get update

$ sudo apt- get install gcc g++ gcc- 7 g++-7 gcc- 8 g++-8
$ sudo update- alternatives - - remove- all gcc

$ sudo update- alternatives --install /usr/bin/gcc gcc /usr/bin/gcc- 8 80 --
slave /usr/bin/ g4-+ g++ /usr/bin/g++-8



위와 같이 업그레이드 되면 다음과 같이 버전 확인합니다．




gcc 버전 확인個.3 으로 업그래이드）
$ gcc -v
Using built- in specs.
COLLECT_GCC=gcc
COLLECT_LTO_WRAPPER=/usr/lib/ gcc/ x86_64-linux- gnu/8/lto -wrapper
Target: x86_64-linux- gnu
Configured with: . . /src/ configure -v --with-pkgversion=1Ubuntu 8. 3. 0-
l6ubuntu2如l2. 04 ' --with-bugurl=file: ///usr/ share/doc/gcc- 8/README. Bugs
enable-languages=c, c++,go, brig, d, fortran, objc, obj- c++ --prefix=/usr --
with- gcc-major- version- only - -program- suffix=田 - -program-prefix=x86_64-
linux- gnu- - -enable- shared - -enable-linker- build-id - -libexecdir=/usr/lib
 - -without-included- gettext - -enable- threads=posix - -libdir= /usr/lib - -
enable- nis - -enable- clocale=gnu - -enable-libstdcxx- debug - -enable-
libstdcxx- time=yes - -with- default-libstdcxx-abi=gcc4-compatible --disable-
libstdcxx- dual- abi - -enable- gnu- unique- object - -disable- vtable- verify - -
enable- plugin - -with- system- zlib - -with- target- system- zlib - -enable- objc-
gc=auto - -enable-multiarch - -disable- werror - -with- arch- 32=1686 - -with-
abi=m64 --with-multilib- list= m32, m64 --enable-multilib --with- tune=generic
- -enable- checking=release - -build=x86.m64- linux- gnu - -host=x86m64-linux- gnu
- -target=x86m64-linux- gnu
Thread model: posix
gcc version 8.3.0 (Ubuntu 8.3.0-16ubuntu2-12.04)




커널연구회佃쌔,w.kerae比z)                                        정재준（I야ii3307@nate.com)
                                    14/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                  커널 소스 빌드 및 버전관리



이t은 우분투가 설치되면서 기본적으로 설치되어 있습니다. 버전은 아래와 같이 확인합니다．

$ git --version

이t vers向n 2.17.1



혹시 이t 이 설치되어 있지 않다면 리눅스 우분투에서 다음과 같은 명령으로 설치하면 됩니다．



小t 설치하71

$ sudo apt-get install git-alL



이t 이 설치되어 있으니，이제 본론으로 들어가서 리눅스 커널 소스를 현재 작업경로에 들어가서

다운로드 받겠습니다. 저의 작업경로는 다음과 같습니다．



$ cd    /home/ jungjaejoon/Projects/kernel/




  커널연구회佃I'사니／.kerneL.bz)                          정재준（I야)13307（孕nate.com)
                                 15/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                            커널 소스 빌드 및 버전관리




커널 소스 다운로드

이t 명령을 사용하여 다음과 같이 다운로드 받습니다. 아래 명령을 실행하면 인터넷 주소

이t.kernel.org 에서 안정화된 최신 커널 소스를 다운로드 받습니다. 제가 이글을 작성하고 있는

시점의 커널 소스는 "v4.20.5" 입니다．



如t으嵬리뇩스 커넙 소스받키


$ git clone git://git.kernel.org/pub/scm/Linux/kerneL/git/stabLe/Linux-stable.git



/／다윰과 같은 메세지가 화면에 출력되면서 다운로드 진행됩니다．


Cloning into 'linux-stable'...
remote: Counting objects: 7310713, done.
remote: Compressing objects: 100% (1096963/1096963), done.
Receiving objects: 다운로드 진행률（%) 표시



현시점의 커널 소스 용량은 7卜'lB 정도 됩니다. 이것을 이t 으로 다운로드 받는데 꽤 시간이 걸립니다．

네트워크 사정에 따라서 차이가 좀 있겠지만 보통 玉4 시간정도 걸립니다. 다운로드 되는 동안

커피한잔 하시면서 다른일을 하셔도 좋겠습니다．



더디어 다운로드 완료 되었습니다．

다운로드한 현재 경로의 내용을 확인하면 다음과 같이 linux-stabte 라는 경로가 생겼습니다．



다운로드된 경로 확‘




 커널연구회佃,ww.kerne나끄）                                          정재준（rgbi3307(@)nate.com)
                                           16/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                          커널 소스 빌드 및 버전관리



$11
/／다음과 같이 화면에 표시 됩니댜．
drwxr- xr- x 3 jungjj jungjj 4096      1 월 28 08: 43 .1
drwxrwxr- x 19 jungjj jungjj 4096      1월 28 08: 06 . .7
drwxr- xr- x 26 jungjj jung力 4096      1 월 28 17: 25 linux- stable!



위의 경로에 들어가서 커널 소스들의 파일 목록을 보면 다음과 같습니다. 이 소스 파일들이 앞으로

우리가 공부해야하는 목록이며 주제별로 지속적으로 설명할 예정입니다. 우선 소스 경로별 의미를

주석문으로 간단히 요약하여 추가 했습니다．




커브소스파앞목爵


$ cd Linux-stable!

$ LI
/／다음과 같이 화면에 표시 됩니다，
drwxr- xr- x 26 jungjj jungjj        4096   1 월 28 17: 25 .!
drwxr- xr- x        3 jungjj jungjj  4096   1 월 28 08: 43 . .!
!!CPU 아키텍쳐 별로 소스가 구성된 경로
drwxr- xr- x 27 jungjj ]ung刀         4096   1 월 28 17: 25 arch!
/／블럭 계층           코어  소스
drwxr- xr- x        3 jungjj ]ung刀   4096   1월 28 17: 25 block!
/／카 암호화／ 사인； 인증 관리 소스
drwxr- xr- x        2 jungjj jungjj  4096   1 월 28 17: 25 certs!
 -rw- r- -r- -      1 jungjj jungjj 14238   1 월 28 17 :25 .clang- format
 = r닛＝r = = r = =   1 jungjj jungjj    59   1월 28 17 : 25 .cocciconfig
 /／소스 저작권（GNU GPL) 정보
 -rw- r- -r- -      1 jungjj ]ung刀    423   1월 28 17: 25 COPYING
 /／리눅스 소스 공헌자들
 -rw- r- -r- -       1 jungjj ]ung刀 99265   1월 28 17: 25 CREDITS
 /／암호화 라이브러리들
 drwxr- xr- x        4 jungjj jung刀  4096   1월 28 17: 25 crypto!
  /／커널 문서（매뉴얼）
 drwxr- xr- x 121 jungjj jungjj      4096   1월 28 17: 25 Documentation!
  /／디바이스 드라이버 소스들




  커널연구회佃쌔쌔／.kerne나끄）                                             정재준（rgbi3307@nate.com)
                                      17/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                         커널 소스 빌드 및 버전관리



drwxr- xr- x 138 jungjj    ]ung刀     4096   1 월 28 17: 25 drivers!
/／폄웨어 소스들
 drwxr- xr- x 2 jungjj     jungjj    4096   1월 28 17: 25 firmware!
 /／파일시스템 소스들
drwxr- xr水 73 jung力        jung刀     4096   1 월 28 17: 25 f s/
!!git 데이터 파일들
drwxr- xr- x  8 jungjj     jungjj    4096   l월 28 17: 25 .git!
-rw- r- -r- - 1 jungjj     ]ung刀       30   1월 28 17: 25 .gitattributes
-rw- r- -r- - 1 jungjj     jungjj    1508   1월 28 17: 25 .gitignore
/／커널 구조쳬 헤더 파일들
drwxr- xr水 27 jung力 ]ung刀            4096   1 월 28 17: 25 include!
/／리눅스 초기화 및 부팅 소스들
drwxr- xr- x 2 jungjj jungjj         4096   1 월 28 17: 25 mnit!
/／프로세스간 데이터교환 소스들
drwxr- xr- x 2 jungjj      ]ung刀     4096   1월 28 17: 25 ipc/
/／커널 소스 빌드 관리
-rw- r- -r- - 1 jungjj jungjj        1736   1 월 28 17: 25 Kbuild
/／커널 소스 설정 파라미터 상수들
-rw- r- -r- - 1 jungjj ] ung刀         563   1월 28 17: 25 Kconfig
/／커널 코어 소스
drwxr- xr- x 18 jungjj     jungjj    4096   1월 28 17: 25 kernel!
/／라이브러리 소스돌
drwxr- xr- x 13 jungjj     jungjj   12288   l월 28 17: 25 lib!
drwxr- xr- x  5 jungjj     jung刀     4096   1 월 28 17: 25 LICENSES!
-rw- r- -r- - 1 jungjj     ]ung刀    10987   1월 28 17: 25 .mailmap
/／커널 소스 관리자 정보
-rw- r- -r- - 1 jungjj jungjj 492402        1 월 28 17: 25 MAINTAINERS
/／커널 소스 빌드 및 버전 정보
-rw- r- -r- - 1 jungjj     jungj]   60523   1 월 28 17: 25 Makefile
/／메모리 관리 소스
dr닛xr- xr水 3 jung力         jung刀    4096    1 월 28 17: 25 mm!
/／네트워크 소스
drwxr- xr- x 70 jungjj     jungjj   4096    l 월 28 17: 25 net!
/／커널 빌드 도움말
-rw- r- -r- - 1 jungjj     jungjj    727    l 월 28 17: 25 README
/／섐플 소스들
drwxr泳r水 27 jungjj         jungjj   4096    1월 28 17: 25 samples!
/／사용자 스크립트 소스듈
dr닙xr口xr水 14 jung力         jungjj   4096    1월 28 17: 25 scripts!
/／보안 모델 구현 소스들
drwxr- xr- x   10 jungjj   jungjj   4096    1월 28 17: 25 security!




 커널연구회佃쌔iw.kerne나끄）                                         정재준（rgbi3307@nate.com)
                                     18/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］              I-

                                                         커널 소스 빌드 및 버전관리           I으으
/／사운드 장치울 위한 드라이버 소스
drwxr- xr- x 26 jungjj ]ung] j    4096   1월 28 17: 25 sound!
/／사용자 도구 소스들
drwxr- xr- x 34 jungjj jungjj 4096       1월 28 17: 25 tools!
!/initramfs cpio archive을 위한 소스들
drwxr- xr- x  2 jungjj jungjj 4096       1월 28 17: 25 usr!
/／커널 가상화（KVM) 지원 소스
drwxr- xr- x  4 jungjj jungjj 4096       1 월 28 17: 25 virt!




소스 파일들이 상당히 많습니다. 앞으로 여기에 있는 소스들을 분석하며 알아가야 합니다. 갈길이

멀어도 천리길도 한걸음부터 뚜벅뚜벅 가다보면 정상에 도달할 것입니다. 이제 위의 소스들을 빌드

（컴파일）하겠습니다．




먼저. 커널 소스를 빌드하기 전에 몇가지 필요한 패키지들을 다음과 같이 설치합니다．




커넘 빔드에 핑묘한 꽤區씨 설치

$ sudo apt- get install   git fakeroot build- essential ncurses- dev xz- utils
libssl- dev bc flex libelf- dev bison




 커널연구회佃쌔iw.kerneLb기                                       정재준（四b13307也）nate.com)
                                    19 / 351
4中1                                                       리눅스 升널 소스 핸설 [.7［추엌묵］.
느I                                                            커널 소스 밀드 및 버전관리

      커널 소스 빌드 및 설치

      위에서 이t 으로 리눅스 커널 소스를 다운로드하여 저장한 경로는 다음과 같습니다．



      $ pwd
      /home/ j ungjaejoon/Projects/kernel/linux- stable



      이 경로에서 이t 을 다음과 같이 실행하면 커널 소스 버전을 확인할 수 있습니다．



      커널 소스 버쳔 확인
      $ git log -l

      /／다음과 같이 화면에 표시 됩니다．
      commit 49a57857aeea06ca831043acbb0fa5e0f50602fd (HEAD -> master, tag:
      v5. 0- rc3, origin/master, origin/ HEAD)
      Author: Linus Torvalds <torvalds@linux- foundation .org>
      Date:     Mon Jan 21 13:14: 44 2019 +1300

          Linux 5. 0- rc3



      위에서 출력된 "니flux 5.0寸c3"이 최신버전이고 태그는 " tag: vs.0-rc3" 입니다. 이 소스를 빌드

      하도록 하겠습니다. 먼저. 소스를 빌드（컴파일）하기 전에 몇가지 작업경로을 만들겠습니다． 다음과

      같이 커널 소스가 빌드되는 경로를 따로 만들겠습니다．



      $ mkdir . . /build


      그리고 다음과 같은 리눅스 명령어로 현재 컴퓨터의 커널 설정파일（.config）을 확인합니다．



      커넘 뾰드 섶청파앉(confi引 확




      커널연구회佃쌔,w.kerne나）z)                                      정쟤준（r야)13307@nate.con分
                                         20/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                     커널 소스 빌드 및 버전관리




$ 11 /boot/config-$(uname -r)

/／다음과 같이 화면에 표시 됩니다．
-rw- r- -r- - 1 root root 220331 1월 25 09: 44 /boot/config- 4. 20. 4+


이 파일（/boot/config따.20.4+）은 현재 필자의 컴퓨터（x86 PC 노트북）에 설치되어 있는 리눅스

커널의 설정 파일입니다. 이것을아래 명령으로 ../build 경로에 .config파일로복사합니다．



$ cp   /boot/config- $(uname -r)     . ./bui.ld/ .config


이제 커널 소스를 빌드하기 위한 설정파일（.con fig）이 준비 되었습니다． 이제 다음과 같이 make

명령을 사용하여 커널 소스를 빌드 하겠습니다．



커넘 소스 빔드하기

               "여怒卜
$ make   -j5    O= . ./build/


"-j5" 옵션은 현재 필자의 컴퓨El Cpu 가 4 개의 코어로 되어 있기 때문에 코어개수＋] 한 숫자 5

주어서 빌드 작업이卜4u［匕Processing 되도록 합니다. 이렇게 하면 속도가 4 배정도 빨라 집니다．

그리고 "O=../build/" 옵션은 커널 소스가 빌드되는 경로를 따로 지정해 주는 것입니다． 이렇게

지정하지 않으면 현재 소스가 있는 경로에 빌드되기 때문에 커널 소스와 빌드된 파일들이 같이 섞여서

관리하기 힘들어 집니다．



아래와 같은 메세지가 화면에 출력되면서 빌드 진행 됩니다．




 커널연구회（www.kerr祀Lb라                                        정재준(rgb13307簪nate.com)
                                    21/ 35 '1
                                                 리눅스 커널 소스 해설 i키초입뿐］
                                                     커널 소스 빌드 및 버전관리



make[l] : Entering directory '/ home/ jungjaejoon/Projects/kernel/build '
/home/ jungjaejoon/Projects!kernel/linux- stable/Makefile :594:
 include/config/auto. conf: No such file or directory
  HOSTCC scripts/basic/ fixdep
  GEN      Makefile
  HOSTCC scripts/kconfig!conf .0
  HOSTCc scripts/kconfig/confdata. o
  HOSTCC scripts/kconfig/expr .0
  HOSTCC scripts/kconfig/symbol. o
  HOSTCC scripts/kconfig/preprocess .0
   LEX     scripts/kconfig/ zconf . lex . c
   YACC    scripts/kconfig/ zconf . tab . h
   YACC    scripts/kconfig/ zconf. tab. c
   HOSTCC scripts/kconfig/ zconf. tab .0
   HOSTCC scripts/kconfig/ zconf . lex .0
  HOSTLD scripts!kconfig!conf
scripts/kconfig/conf - - syncconfig kconfig
士


* Restart config. . .

士


* Processor type and features


                                                    V
                                                    / V
                                                      J
DMA memory allocation support (ZONE_DMA) [Y/n!?]
Symmetric multi-processing support (SMP) [Y/n!?]
Support x2ap1c (X86_X2APIC) [Y/n!?] y
Enable MPS table (X86_MPPARSE) [Y/n!?] y
Avoid speculative indirect branches in kernel (RETPOLINE) [Y/n!?] y
Resource Control support (X86_RESCTRL) [N/y/?] (NEW)
/／잗시 멈춤！ 키보드 입력대기



위에서 복사한 "../buiLd/.config"에 있는 현재 커널 설정 파일과 지금 빌드하는 커널 소스 버전이

다르다면，위와 같이 config 설정 파일에서 다른 부분들을 새롭게 맞추71 위한 질문이 출력 됩니다．



只esot玉rce 鈿ntrol su弘弘ort (X86_RESCTR나 [N/y!?] （村드낯｝




커널연구회b赳＼阿w.kerneib卦                                       정쟤준(rgb沼307簪nate.com)
                                   22/ 351
                                                     리눅스 커널 소스 해설 ［카초입문］
                                                         커널 소스 빌드 및 버전관리



이처럼 새롭게 맞추어 주71 위한 설정 질문은 (NEW）가 출력 됩니다. 그냥 엔터를 쳐서 디폴트로

설정되도록 합니다. (NEW)가 나올때마다 그냥 엔터합니다． 이 과정이 끝나면 커널 소스가 빌드되기

시작합니다．




빌드 진행되는 시간은 컴퓨El 속도에 따라서 차이가 있으나 보통 40사50 분정도 걸립니다 ．빌드되는

동안 커피한잔 하시면서 다른일을 하셔도 좋겠습니다．




더디어 빌드가 완료 되었습니다. 다음과 같이 빌드 경로의 내용을 확인합니다．




빌드 켱로 확인


$ 11 . . !build/



/／다옳고｝ 같이 화면에 표사 됩니다，
drwxr- xr- x   23 ]ung刀      ]ung刀      4096 1 월 29 11: 54 1  .
drwxr- xr- x    4 그ung刀      ]ung刀      4096 1 월 29 10:13    /
drwxr- xr 水     4 그 ungj ]   ]ung刀      4096 I.월 29 11: 54 arch!
drwxr- xr- x    3 ]ung刀      jungjj     4096 1 월 29 12: 07 block/
                I jungjj     ]ung刀    821060 1 월 29 11: 50 built- in .a
drwxr- xr 水     2 ]ung刀      ]ung刀      4096 1 월 29 10: 46 certs/
                I jungjj     jungjj   221457 :L월 29 10: 45 .config
                1 ]ung刀      ]ung刀    220331 l 월 29 10: 37 .config.old
/／충칸 섕략，,
                1 jungjj     jung力          2   :L 월 29 11: 49 .version
drwxr- xr- x    4 iungjj     jung力       4096   :L월 29 11:11 v1rt/
                1 jungjj     jungjj 623688408   :L 월 29 1그：53 vm11nux士
                1 jungjj     jungjj       182   :1 월 29 11: 53 .vmlinux. cmd
                1 jungjj     jungjj 740521840   1월 29 11: 51 vm11nux. o




  커녈연구회如째1차,kerneLbz)                                        정재준（呵出3307回nate.com)
                                       23 / 35'1
                                                 리눅스 커널 소스 홰설 ［기초입문］
                                                     커널 소스 빌드 및 버전관리



위의 빌드된 파일들 중에서 arch/x86/boot/bzlmage 는 커널 실행（Linux kern이 x86 boot

executable) 이미지이고, vmlinux 파일은 커널이 빌드될때 각종 리스팅 정보와 Sec匕on 정보들이

보관된 파일（ELF 64止)it LSB executa비e）입니다. 이 파일은 나중에 커널을 디버깅할따1 사용합니다．



위와같이 커널 소스 빌드가 끝나면 커널 모듈（.ko）들과 이미지 파일（../build/arch/x86/boot/

bzlmage）을 해당 경로에 설치하는 작업이 필요합니다. 먼저 다음과 같이 커널 모듈들을 설치 합니다．

sudo 을 앞에 붙여서 root 권한으로 make 을 실행합니다．



커널 모長 설치하기

$ sudo make    Oz. . /build/   modules_install


위의 실행에 의해서 설치되는커널 모듈（.ko）들은／Lib/mod미es／경로에 있습니다 ．아래에서 "5.0.0-

rc3/" 경로가 위의 커널 소스를 빌드한 모듈들이 설치된 경로 입니다．



커넘 모듈 켱로 확인


$ 11 !lib! modules/



/／다응과 같이 軒면에 표시 됩니다，
drwxr- xr- x 16 root root 4096 1월 29 07: 06 .1
drwxr- xr- x 22 root root 4096 5 월 17 2018 . .1
drwxr- xr- x 5 root root 4096 12월 5 07: 41 4.15. 0- 42- generic!
drwxr- xr- x 5 root root 4096 1월 29 07: 07 4.15. 0- 44- generic!
drwxr- xr- x 3 root root 4096 1월 24 08: 01 4. 20. 0+!
drwxr- xr小 3 root root 4096 1 월 25 09: 25 4. 20. 4+!
drwxr- xr- x 3 root root 4096 1월 29 12:20 5.0.0- rc3/




커널연구회（ww냄／.kernel.bz)                                  정쟤준（r야)13307（孕nate.com)
                                  24/ 351
                                                   리눅스 커널 소스 해설 ［기초입룬］
                                                       커널 소스 빌드 및 버전관리



커널 모듈 설치가 끝났으므로 이제 커널 이미지 파일（../b山Ld/arch/x86/boot/bztmage）을 다음과

같이 설치합니다．




$ sudo make    0= . ./build/   install



위의 명령이 끝나면 커널 이미지 파일（../b미너／arch/x86/boot/bzlmage）이 "vmlinu즈5.O.O-rc3"

으로 /boot/ 경로에 다음과 같이 설치 됩니다．




커났섶치 경로 확인
$ 11 !boot!

/／다음과 같이 화면에 표시 됩니댜，
drwxr- xr- x 4 root root          4096 1월 29 07: 07 .1
drwxr- xr- x 27 root root         4096 1월 29 07: 07 . .1
-rw- r- -r- - 1 root root      1538114 11월 16 04: 01 abi- 4.15. 0- 42- generic
-rw- r- -r- - 1 root root       220669 1월 24 08: 05 config- 4. 2包4+
-rw- r- -r- - 1 root root       221457 1월 29 12: 23 config- 5. 0. 0- rc3
drwx             4 root root      4096 1 월 1 1970 efi!
drwxr- xr- x 5 root root          4096 1월 29 07: 08 grub!
-rw- r- -r       1 root root 589404341 1월 24 08:10 initrd. img- 4. 20. 4+
-rw- r- -r       1 root root 592988196 1월 29 12: 27 initrd. img- 5. 0. 0- rc3
-rw- r- -r- - 1 root root       182704 1월 28 2016 memtest86+.bin
-rw- r- -r- - 1 root root       184380 1 월 28 2016 memtest86+ .elf
 -rw- r- -r- - 1 root root     4213954 1월 24 08: 05 SystenLmap- 4. 20. 4+
 -rw- r- -r- - 1 root root     4223406 1월 29 12: 23 System. map- 5. 0. 0- rc3
 -rw             1 root root   8277752 11  16 04: 04 vmlinuz- 4.15. 0- 42- generic
 -rw- r- -r- - 1 root root     8570752 1 월 24 08: 05 vmlinuz- 4. 20. 4+
 - r1寸. r- -r- = 1 root root   8570752 1월 29 12: 23 vmlinuz巧 . 0 . 小r心



이제 커널 빌드 및 설치가 끝났습니다．




 커널연구회佃ww.kerneLbz)                                        정재준（I야)1330킥孕陀te.com
                                     25/ 351
                                                                라눅스 커낼 소스 翊졀 E기姦입문]
                                                                    커널 소스 빌드 및 버전관리



리눅스 우분투는 위의 /boot/ 경로에 있는 이미지 파일들을 참고하여 /boot/g rub/g rub.cfg 파일에

부팅 머H뉘가 설정됩니다. 컴퓨터를 재부팅하면 이 메뉴7r 나타나고 이곳에서 부팅할 커널 버전을

선택할 수 있습니다. 보통 부팅 메뉴 제일 상단에 최신 커널 버전이 있습니다 ．이것으로 부팅하면

됩니다. 혹시 최신 커널 버전에서 문제가 생기면, 다시 부팅하여 grub 메뉴에서 이전 커널 버전을

선택하면 됩니다. 그리고, 위에서 커널 소스를 빌드할때／boot/config-$(uname -r) 파일로 되어

있는 내 컴퓨터의 기본 커널 설정 파일（.config）을 사용했습니다． 커널 설정 파일을 직접 수정하고

싶다면 아래와 같이 make을 " menuconfig" 옵션을 주어 실행하면 됩니다.



$ make O=../buiLd/ menuconfig


menuconfig 화면

                         珏麝姓S／薑拉色 5. u. 0- ! 乞3 珏｛났 C密t C口和분 三珏毖rats各豪
     Arr(｝닢 keys navigate the menu. 唵nter> selects sub冊en仕5 ; . h> {｛玎 쥡叩ty submeflus
     . n ,).  Highlighted letters are hotkeys. Pressing <Y> includes, eN> excludes,
     ＜杆＞ modularizes features. Press <ESc>.eEsc> to e,ut. c?> for Help. c/> for
     Search. Legend: t 'J built- in I I excluded 帥> module .c > module capable


            Seneral setup    -->
        [5) 64-bit kernel
            弘rocessor type and fe自tures ! . 寸＞
            Fo누er management and ACP.L options
            flus options (PCI etc. ) -- :>
            einary tmulations -- ->
            Firmware Orivers V 叫 尸＞
        ['1 1irtoalization . . -
            General architecture-dep肛dent options
        ｛寸j 芒nable loadable module sup弘ort --甘＞
        [5) Enable the block layer - - ->
            姓） Schedulers    -.>
            Executable file formats - - ->
           卜祉mory 川anage1打ant options 1-->
        1卑｝ 枷：b的rking support " >
            各evice 口rivers       >
            File 引／Ste用S 竹叫 r>
            Security options 戶- ->
        ，京 Cryptograph工C AP工 小．>
            Library routines . n>
            共ernel hacking --.>


                            c Exit >    <Help>      <Save>      < Load >




1 각주：update- grub



 커녈연구회（＼硝丹邪,kerneLb卦                                                       정趨준（唾蜘330？簪n航色corn)
                                             26/ 351
                                                              라눅스 커널 소스 해설 [기姦입룬］
                                                                  커널 소스 빌드 및 버전관리



위의 메뉴에서 설정되는 정보들은 ../b미너／경로의 .config 파일에 저장됩니다． 이 파일 안에는

CONFIG_형태로 정의되는 상수값이 있으며 이것은 커널 소스에 인클루드 되어 컴파일러에서

사용합니다． 즉，커널 소스는 여기서 정의한 CONFIG．상수값에 따라서 전처리되어 컴파일 됩니다．

이 설정값들은 커널 소스와 같이 설명해야 하므로. 앞으로. 진도 나가면서 설명하는 공간을 따로 만들어

보도록하겠습니다·                           U뇨，七， t우D斗씨石t는

                                            沌t乙娃仙比 / 目1卜(t            寸吐

                                                       砂 GP以8中tT卜＼乙OUT.. '1(L& =\Mek나 " k빤겅
                                                                                      喆如比＝ r ' L} d'ie나"
커널 소스 버전업                             : 뇨V氏그令.t q스A叭五夫i人Y낱                                            .    ,,
                                                  口＞ \n0S(,M4 ＜虹机mb出1:                     咐""今d\"b\'
위와 같이 리눅스 커널 소스를 이t 으로 다운로드하여 make 명령으로 빌드 및 설치하면 됩니다만，

문제는 커널 소스가 계속 버전업 되기 때문에 버전별로 소스를 관리하고 빌드해야 합니다. 다행히 g化

에서 이 작업을 편하게 할 수 있도록 명령어를 제공합니다. 이I 명령어를 잘 활용하시면 됩니다. 먼저

다음과 같이 이I 이 원격 접속하고 있는 인터넷 주소를 확'긴합니다．



小t 원걱 접속 주소 확인


$gitremote-v



/／댜醫과 같이 화면에 표시 됩니다，
origin git://git.kerneLorg/pub/scm/Linux/kernet/git/stable/linux-stable.git (fetch)
origin git://git.kernel.org/pub/scm/Einux/kernel/git/stable/linux-stabLe.git (push)




 커널연구회佃n사＼杉．kerne나玘）                                                   정재준（r야)i3307匣｝nate.com)
                                             27/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                       커널 소스 빌드 및 버전관리



위에서 표시되고 있는 on이n 이 이t의 원격 저장소 입니다. 커널 소스 업데이트는 이곳으로부터

fetch 받으면 됩니다. 다음과 같이 미t 명령어를 실행하면, 커널 소스를 빌드한 이후에 변경된 소스7F

있으면 최신 버전을 다시 fetch 받습니다．




커넘 소스 fetch 받7I


$ git fetch origin



/／다욤콰 같아 화면에 표시 됩나다，


remote: Counting objects: 3524, done.
remote: Compressing objects: 100% (1836/1836) , done.
remote: Total 3524 (delta 2503) , reused 2709 (delta 1688)
Receiving objects: 100% (3524/3524) , 4. 29 MiB I 2. 70 MiB/ s, done.
Resolving deltas: 100% (2503/2503) , done.
From git : //git. kernel. org/pub/ scm/linux/ kernel/git/ stable/linux- stable
   9b5eed105a45. .4c35624dcb3b linux- 3.18. y -> origin/ linux-3.18. y
   8979da2558a4. .e6608e1f2fbd linux- 4.14. y -> origin/ linux- 4.14. y
   23b6b8bf9011. .34ae65724615 linux- 4.19. y        origin/ linux- 4.19. y
   3d4332cd8258. . 9f1a389a0b5b linux- 4. 20. y      originhlinux- 4. 20. y
   c5feba4358ed. . 626b008972db linux- 4. 4. y       origin/ linux- 4. 4. y
   008bfb931296. . 189b75ad3fc2 linux- 4.9. y        origin/ linux- 4 .9 .y
 出 [new tag]                        v3. 18. 133      v3 .18 . 133
 士 [new tag]                        v4. 14. 96       v4.14. 96
 士 [new tag]                        v4 .19.18        v4 .19. 18
 火 [new tag]                        v4. 20 .5        v4. 20. 5
 士 [new tag]                        v4. 4.172        v4. 4.172
 士 [new tag]                        v4 .9.153        v4 .9.153
 火 [new tag]                        v4.14. 95        v4.14. 95
 士 [new tag]                        v4 .9.152        v4 .9.152




커널연구회佃쌔1사．kerne나파                                         정재준（rgb沼307每nate.com)
                                    28/ 351
                                              라눅스 커널 소스 해설 ［기초입문］
                                                  커널 소스 빌드 및 버전관리



필자의 경우, 위의 실행 메세지는 커널소스 " v4.20.4"을 설치 했다가 "v4.20.5"로 업데이트 되 것을

fetch 받아온 결과 입니다． 위의 내용을 자신의 로컬 저장소에 반영하기 위해서 다음과 같이 merge

합니다．



커넘 소스 merg喀하기


$ git merge origin/master



merge 되는 내용이 화면에 출력 됩니다 ．위와 같이 하면 커널 소스가 내 PC에 최종적으로

업데이트가 마무리 됩니다. 마무리된 결과 최신 버전 확인은 다음과 같이 확인합니다．



커넘 소스 최신 버전 확인


$git[og-1

/／다읖과 같이 화면에 출력됩니다，

commit 49a57857aeea06ca831043acbb0fa5e0f50602fd (HEAD -> master, tag: v5.O-
rc3, origin/master, origin/HEAD)
Author: Linus Torvalds <torvalds@linux- foundation. org>
Date:   Mon ian 21 13:14: 44 2019 +1300

    Linux 5.O- rc3




위와 같이 표시되는 "니flux 5.O-rc3"이 리눅스 커널 소스 최신 버전 입니다. 그런데 버전 뒤에 "寸c"가

붙으면 이것은 아직 안정화되지 않고 현재 개발 진행중인것을 의미 합니다. 그래서 안정화된 최신

버전은 아래와 같이 이t tag 명령을 통해서 확인합니다．




 커널연구회（螂／w.kerne나功                                   정재준（芯bi330기孕nate.com)
                                 29/ 351
                                        리눅스 커널 소스 해설 E기초입문］
                                            커널 소스 빌드 및 버전관리




         소스t


$git tag Igrepv5

/／댜음과 같이 화면에 출력됩니댜，

 v5. 0- rcl
 v5. 0- rc2
 v5 .0- rc3


     $ giL tag I grep v4.20

/／다윰과 같이 화면에 출력됩니댜，

 v4 .20
 v4. 20- rcl
 v4. 20- rc2
 v4. 20- rc3
 v4. 20- rc4
 v4. 20- rc5
 v4. 20- rc6
 v4 . 20寸 rc7
 v4. 20.1
 v4. 20. 2
 v4. 20. 3
 v4. 20. 4
 v4. 20. 5



위와 같이 출력된 리눅스 커널 소스 tag 들 중에서 "v4.20.5"가 가장 최근에 안정화된 커널 소스

버전입니다. 그럼 이 버전으로 소스를 작업（빌드, 설치）하기 위해서 다음과 같이 g止으로 checkout

합니다．




         也I
최4
     커널연구회（娜／w.kern畝.bz)                    정재준(rgbi3307（孕nate.com)
                              30/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                    커널 소스 빌드 및 버전관리



$ git checkout -b CV4.20.5 v4.20.5




위의 checkout 명령에서 -b 옵션은 "CV4.20.5" 브랜치를 만든다는 것이고. "v4.20.5"는 커널 소스

tag 명입니다. 따라서 이명령은커널 소스 버전 "v4.20.5 "로부터 "CV4.20.5" 브랜치를새로

만들어서 checkout 하는 것입니다. 그런다음, 아래와 같은 명령으로 checkout 된 브랜치를

확인합니다．



checkout


$ 9化 branch

/／다음과 같이 화연에 출력됩니다．

出 CV4 . 20 . 5
  master


커널 소스 버전 "v4.20.5"가 "CV4.20.5" 으로 checkout 되었으므로 이제 이 버전으로 소스를 빌드 및

설치하면 됩니다. 소스 빌드 및 설치는 앞에서 설명드린 방법으로 하시면 되겠습니다．



지금까지 최신 리눅스 커널 소스를 다운로드 받아서 빌드 및 설치하고 소스 업데이트 및 버전관리에

대해서 설명 드렸습니다. 이러한 작업들은 모두 이t을 사용해서 하기 때문에 이I 명령에 대해서

익숙해져야 합니다. 이t 사용법은 이글의 범위를 벗어나는 것이여서 자세히 설명 드리지 못했지만，

시중에 있는 서적이나 인터넷에 많은 정보들이 있으므로 참고하여 학습하시면 되겠습니다．




  커널연구회佃쌔쌔／.kerneLb기                                정재준（rgbi3307（흐）nate.com)
                                     3] / 35가
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        커널 소스 코딩 형식




커널 소스 코딩 형식

리눅스 커널 소스에는 관습적으로 지켜져 내려오는 코딩 형식이 있습니다. 코딩 형식은 개인마다 다를

수 있기 때문에. 리눅스 커널 소스는 유지보수 관리를 효과적으로 하기 위해서 코딩 형식을 지켜 주는

것이 좋습니다. 리눅스 커널 소스 코드를 다음과 같은 항목별로 지켜야 하는 코딩 형식을 정리합니다．

참고로，아래 내용들은 리눅스 커널 문서 [2 I］를 참조하여 이해하기 쉽도록 집필 했습니다．



   .   들여쓰기

   .   긴줄과문자열 나누71

   .   괄호와공백 배치

   .   작명

   .   타입 재정의

   .   함수들

   0 gob0사용

   1   주석문

   0 Macros, Enums

   1   커널 메세지 출력

   0 메모리 할당

   1   inLine 함수

   S 함수 반환값

   1   boo［사용

   S 커널 매크로 활용

2 참2 문Aj https: //ww닙. kerneLora/doc/html/latest/process/ coding- style. htm1.



커널연구회（w硏쌔／.kerneLbz)                                   정쟤준(rgb13307（孕nat色corn)
                                  32/ 351
                                      리눅스 커널 소스 해설 ［기초입문］
                                              커널 소스 코딩 형식



    0 Inline assembly




들여쓰기

탭은 8 자 이므로 들여쓰기도 8 문자 입니다. 들여쓰기를 4 자 훅은 2 자로 하려는 습관이 있을 수

있으나 8 자로 하는 것을 권고합니다. 들여쓰기는 제어 블록이 시작하고 끝나는 위치를 명확하게

정의하는 것입니다. 특히 장시간동안 소스 코딩을 하면서 화면을 보고 있으면 들여쓰기가 명확하면

할수록 피로감이 덜 느껴 집니다. 들여쓰기를 8 자로 화면 80 자 터미널 화면에서 금방 벗어날 수

있어서 오히려 불편하게 생각할 수도 있습니다. 하지만 돌여쓰기를 3 단계 이상하면 위의 경우가

나타날 수 있는데, 이것은 오히려 들여쓰기 깊이를 3 단계 이상 하지 말라는 경고의 의미로 전화위복

되는 효과가 있습니다. 다시 말해서, 들여쓰기는 8 자로 해서 제어 블록을 명학하게 파악할 수 있도록

하고. 함수를 3 단겨1 이상 너무 깊이 중첩하게 되면 경고해주는 장점이 있습니다．



아래는 switch 문을 코딩할때 8 자 들여쓰기를 효과적으로 하는 예제를 보여주고 있습니다．

switch (suffix) {
case 1 G 1 :
case 1 g 1 :
           mern <<= 30;
           break;
case 'M ' :
case 'rn 1 :
           mern <(= 20;
           break;
case 'K ' :
case 'k ' :
           mern <<= 10;
           falith rough;
default:
           break;
}



 커널연구회佃쌔사／.kerne(. 뇨）                      정재준（rgbi3307@nate.com)
                           33 / 35재
                                         리눅스 커널 소스 해설 ［기초입문］
                                                 커널 소스 코딩 형식




그리고 아래으I if 문 코딩은 잘못된 들여쓰기 입니다．

if    (condition) do_this;
     do_something_everytime;


다음과 같이 코딩하는 것이 좋습니다．

if (condition)
      do_this;
do_something_everytime;


소스를 편집때는 이상（애매 모호）하거나 까다롭게 편집하기 보다는 잘 알려진 형식대로 깔끔하면서도

간단하게 편집합니다. 그리고 들여쓰기 할때는 공백을 여러개 입력하는것보다 탭을 사용하고, 문장의

끝에는 공백을 남겨두지 않는 것이 좋습니다．




긴줄과 문자열 나누:7 '

코딩 형식을 지켜주면 신뢰성과 유지보수성이 증다1 되므로 일반적으로 잘 알려진 편집 도구를

사용하는 것도 좋은 방법입니다. 한줄은 80 문자를 넘어가지 않도록 합니다. 리눅스 터미널（콘솔）

창은 전통적으로 80 문자로 되어 있습니다. 따라서 한줄이 80 문자를 넘어가면 가독성이 떨어집니다．

되도록이면 논리를 블럭단위로 상하위로 잘라서 들여쓰기 하여 배치합니다. 그러나 prinik 안에

                      ．왜냐하면 문자열이 끊어 지면 grep 기능이 저하됩니다．
문자열 메세지는 나누지 않는 것이 좋습니다




커널연구회佃쌔쌔／.kerne나功                            정재준（rgbi3307（흐）nate.com)
                               34/ 351
                                        리눅스 커널 소스 해설 ［기초입문］
                                                커널 소스 코딩 형식



괄호와 공백 배大1

C 코딩 형식에서 일관성을 유지하기 힘든것들중에 하나는 괄호와 공백 배치입니다 ．들여쓰기는 8 자

단위로 하면 되지만 괄호와 공백은 저마다 다르게 편집하는 경우가 많습니다. 하지만 C 언어를 개발한

K&R(Kernighan 과 Ritchi미이 문서화한 아래의 예시대로 코딩하는 것이 좋습니다．



if    (x is true) {
         we do y
}

switch (action) (
case KOBJ ADD:
         return "add";
case KOBJ REMOVE:
         return "remove";
case KOBJ CHANGE:
         return "change";
default:
         return NULL;
}

위와 같이 여는 중괄호｛는 문장의 끝에 배치하고 닫는 중괄호｝는 새로운 시작 라인의 처음에

배치합니다. 위의 예시는 함수가 아닌 문장들(if, sw比ch, for, while,（幻）에 대해서 모두 지켜주는

것이 좋습니다. 그러나 함수인 경우에는 다음과 같이 코딩합니다．



mnt function(int x)
{
           body of function
}




     커널연구회（蜘,w.kerne나）기                        정재준（rgbi3307@nate.com)
                              35/ 351
                                           리눅스 커널 소스 해설 E기초입문］
                                                   커널 소스 코딩 형식



위와 같이 함수인 경우에는 중괄호를 모두 새로운 시작 라인의 처음에 편집합니다 ．함수는 중첩되지

않으므로 위와 같이 표현하는 것이 좋습니다．



K&R(Kernighan 과 Ritchi이의 문서 내용을 보면 do whiLe 과 중첩된 if 문장은 다음과 같이

코딩하도록 되어 있습니다．



do {
        body of do-loop
} while (condition) ;


if   (x == y) {

} else if   (x >   y)   {
} else {

}

위와 같이 코딩하면 가독성도 좋고 편집 공간을 절약적으로 사용하는 장점이 있습니다．

그리고 아래와 같은 단일 문장에는 중괄호를 사용하지 않아도 됩니다．



if   (condition)
         action() ;


if (condition)
       do_this() ;
else
       do_that ( ) ;




커널연구회佃姚째／.kernet.bz)                             정쟤준（rgbi3307會na始（om)
                              36/ 351
                                            리눅스 커널 소스 해설 ［기초입문］
                                                    커널 소스 코딩 형식



그러나 여러 문장에 대해서는 아래와 같이 중괄호를 사용하여 명확하게 논리 블럭을 코딩하도록

합니다．



if (condition) {
         do_this() ;
         do_that () ;
} else {
         otherwise() ;
}

while (condition) {
        if (test)
                do_ somethingQ;
}




공백

공백은 키워드를 구분하기 위한 용도로 사용합니다. 아래와 같은 제어문 형태의 키워드衍JW比ch,

case, for, do, while) 다음에는 공백을 삽입합니다．



if (. . .)
switch (. . . )
case (. . .)
for (. . .)
while (. . .)



그러나 연산자 형태의 키워드（引zeof, typeof, alignof, _attributeJ 다음에는 공백을 삽입하지

않습니다．




     커널연구회（www.kerne나）z)                        정재준（rgbi3307@nate.com)
                                  37/ 351
                                                                          리눅스 커널 소스 해설 ［기초입문］
                                                                                  커널 소스 코딩 형식



S = sizeof (struct file) ;



위와 같이 코딩하는 것이 좋습니다. 하지만 아래와 같이 괄호안에 공백을 추가하는 것은 나쁜

습관입니다．




s = sizeof ( struct file              );



데이터 타입. 포인터, 함수 선언은 다음과 같이 편집합니다．

char *linuxHbanner;
unsigned long long memparse(char *ptr, char **retptr) ;
char *match叫strdup(substringHt *s) ;



아래와 같이 연산대상이 2 'U 이상인 연산자들에 대해서는 연산자 앞뒤에 공백을 추가합니다．



=        +   -   <   >   *   I   %    1    &   "   <=   >=    ==     !=    ?


하지만, 연산대상이 ] 개인 연산자들에 대해서 공백을 추가하지 않습니다．



&        *   +       H   !   sizeof       typeof    alignof        H中attribute1     defined


연산대상이 1 개인 증감연산자에도 공백을 추가하지 않습니다．




구조체 멤버 참조 연산자에도 공백을 추가하지 않습니다．



     -   >




    커널연구회（叫iwkerneLb라                                                          정재준（rgbi3307@nate.con分
                                                   38/ 351
                                       리눅스 커널 소스 해설 ［기초입문］
                                               커널 소스 코딩 형식




줄 끝에는 공백을 남겨 두지 않는 것이 좋습니다. 스마트 들여 쓰기가 있는 일부 편집기는 새 줄의 시작

부분에 공백을 삽입하여 다음 코드 줄을 바로 입력 할 수 있습니다. 그러나 빈 줄을 남겨 두는 등의 코드

줄을 넣지 않으면 이러한 편집기에서 공백을 제거하지 않습니다. 결과적으로 뒤에 공백이 포함 된 줄이

생깁니다．



G止 은 후행 공백을 도입하는 패치에 대해 경고하고 선택적으로 후행 공백을 제거 할 수 있습니다．

그러나 일련의 패치를 적용 할 경우 컨텍스트 라인을 변경하여 시리즈의 이후 패치가 실패 할 수

있습니다．




작명

C 언어는 사용자가 이름들을 일일히 정의해야 합니다. 이름을 만들따1

ThisV카治b［이sAlen叩oraryCounter와같은 긴이름보다간결한이름을선호합니다. 이름이

간결하면 편집하기에도 쉽습니다． 하지만 전역변수（꼭 필요한 경우에만 사용）는 대문자와 소문자

조합의 단어들로 구성하는 것이 좋습니다. 함수도 만찬가지 입니다. 함수 이름은 cntusr(）와 같이

너무 간결하게 하기보다 그 쓰임새가 연상 되도록 countmactive_users(）로 이름을 만드는 것이

좋습니다． 지역（내부）변수는 이름을 짧게 합니다. 예를들어 반복문 카운El 변수는 [oop_counter

라든 ZJ 이름보다 i 라고 하는 것이 관례화 되어 있습니다. 또한 임시로 사용하는 목적의 내부 변수는

tmp 라는 이름을 많이 사용합니다.




 커널연구회佃쌔iw.kernel.b기                        정재준（寸)13307（흐）nate.com)
                            39/ 351
                                             리눅스 커널 소스 해설 E가초입문］
                                                     커널 소스 코딩 형식



타입 재정의

typedef을 사용하여 타입을 재정의하면 편리함도 있지만, 활용 용도에 따라서 불편함도 있습니다．

예를들어 아래와 같이 타입을 재정의한 vps_t 로 a 을 만들면 a 가 어떤 형태인지 한번에 판독하기

어렵습니다．



vps-H-上 a;


그러나 다음과 같이 a 을 만들면 a 가 어떤 타입（구조체 포인터）인지 바로 판독됩니다．



struct virtual_container *a;


이처럼 vps_t 는 아래와 같이 타입을 재정의한 것이지만，



typedef struct virtual_container *   vps_t


소스에서 위의 내용을 직접 찾아 봐야 하는 번거러움이 있습니다. 그래서 typedef을 사용하여

타입을 재정의 할때는 몇가지 관례들이 있습니다．



관型主．타입을 재정의하여 그 쓰임새를 숨기는 것이 오히 좋은 객체나 정해진 타입으로 제한을

해야하는 객체에 대해서 사용합니다. 예를들어 pte_t etc 라고 etc 을 정의하면 etc 는 ptej

타입으로만 접근할 수 있습니다．




커널연구회（w硼w，蛇mne나玹）                                정쟤준(rgb13307會riate.com)
                                40/ 351
                                        리눅스 커널 소스 해설 ［기초입문］
                                                커널 소스 코딩 형식



콴町캄：타입에 대해서 혼동을 피할 수 있도록 재정의 합니다. 예를들면, u8/ul 6/u32/u64 와 같이

데이터 타입을 재정의 하는 것은 아주 좋은 예입니다．



관斑馨타입을 검사하기 위한 유형의 타입을 만들때1.



趙쏘I-타입을 재정의한 u8／山6/u32/u64 는 기존 코드 그대로 관례를 지켜주는 것이 좋습니다．

미nt8_t加in너 6_t/uin日2中t/ u1nt64_t 도 많이 사용하는데 이것도 편집하려는 소스에서 사용하고

있다면 그대로 사용합니다．



관翌됴L사용자공간에서 안전한유형은그것을그대로사용합니다. 예를들어＋u32가사용자

공간에서 사용되고 있다면 이것을 그대로 사용하는 것이 좋습니다．



typede f는 타입을 재정의 하는 용도로 마음대로 사용할 수 있으나, 되도록이면 위에 나열한 관들을

만족하는 경우에 대해서만 typedef을 사용하도록 합니다. 또한 위의 내용을 보면 아시겠지만

typede F 으로 재정의한 타입의 이름 끝에는 항상 1 t 을 붙이는 습관도 놓치지 마시기 바랍니다．




함수들

함수의 기능은 되도록이면 간결하게 동작하도록 코딩합니다. 전통적으로 ISO/ANSI 화면 크기는 가로

80 문자 세로 24줄입니다. 함수는 이 공간에 맞도록 편집하도록 합니다. 함수안의 코드량은 해당

함수의 복잡성과 들여쓰기 수준（깊이）에 비례합니다. 그래서 함수의 코드량이 많다면, 작업단위별로




 커널연구회佃I'사w.keraet.뇨）                         정재준（r야)13307@nate.cam)
                             41/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 소스 코딩 형식



간단하게 분리하도록 합니다. 함수가 어쩔수 없이 복잡해진다면, 논리단위별로 구분하고 도와줄 수

있는 함수들을 추가 하거나 인라인 함수로 나누어 주도록 합니다．



』함수 안에서 사용하는 내부（지역）변수들의 수는 5 개에서 ]0 개를 유지하도록 합니다. 이 개수가

넘어가면 복잡하1 지므로 함수를 다시 작은 단위로 나누어 줍니다. 우리의 뇌는 약 7 가지의 대상들을

쉽게 추적할 수 있습니다. 되도록이면 함수를 작게 나누어 주는 습관을 가지도록 합니다．



，리눅스 커널 소스에서 함수를 외부 공용（public) 함수로 정의해 주는 용도로 아래와 같이 EXPORT

매크로를 사용합니다． 이 매크로는 다음과 같이 함수 정의가 끝나는 닫는 중괄호 } 다음에서 줄을 바꾼

자리에 삽입 하도록 합니다．



 mnt system_is_up (void)
 C
         return system_state == SYSTEM_RUNNING;
 }
 EXPORT_SYMBOL (system_is_up) ;




9010 사용

일반 C 언어 사용자들은 논리 이동이 복잡하1 진다는 이유로 gob0 문 사용을 자제하는 경향이

있습니다． 하지만 컴파일러 내부에서는 제어 분기를 할때 goto 형태로 분기합니다. 커널 소스에서는

함수 내부에서 g야0문을 자주 사용합니다. 함수 내부에서 문제가 발생해서 오류 처리하기 위한

부분으로 무조건 집중적으로 이동해야하는 경우 gob0 문을 사용합니다. goto 문으로 이동하는

위치를 나타내는 레이블은 왜 그 위치로 이동하는지 이유가 연상되는 이름이 좋습니다．




 커널연구회（www.kerneLbz)                                  정쟤준（rgbi3307@nate.com)
                                  42/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 소스 코딩 형식




goto 문은 몇가지 장점이 있습니다. 복잡한 논리에 의해서 이동하는 것보다 무조건 분기하는 goto

문이 오히려 직관적으로 이해하기 쉽습니다. 중첩된 논리가 줄어 듭니다. 중복 코드를 최적화하는

컴파일러 작업에 도움을 줍니다．



아래의 소스 예제는 조건문 안에서 out_free_buffer: 레이블로 이동하는 논리가 직관적으로 쉽게

이해됩니다．



mnt fun(int a)
{
         mnt result = 0;
         char *buffer;

         buffer = knialloc (SIZE, GFP_KERNEL) ;
         if ( ! buffer)
                   return -EN아作M;

         if   (conditioni) {
                  while (loopi) {


                  }
                  result = 1;
                  goto out_free_buffer;
          }
out free buffer:
        kfree(buffer) ;
        return result;
}




    커널연구회佃w니／.kerne나파                                 정재준（rgbi3307@nate.con力
                                    43 / 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                            커널 소스 코딩 형식




주석문

일반적으로 주석문을 추가하는 것은 좋습니다. 하지만 지나치게 주석을 추가하는 것은 오히려 코드

판독에 방해가 됩니다. 소스 코드가 명확하게 잘 판독되는 곳에는 주석문으로 설명하려 하지 마세요．

그냥 코드로 판독 하는 것이 좋습니다．




주석문은 함수가 시작되는 앞부분에 위치하는 것이 좋습니다. 함수 안에 주석문을 추가하면 오히려

코드를 판독하는데 방해가 되기 때문입니다. 함수 안에 주석을 추가해야 한다면 되도록 간단하게

편집하도록 합니다．




내용이 많은 주석문은 아래와 같은 형식으로 편집하도록 합니다．



／出
     * This is the preferred style for multi-line
     * comments in the Linux kernel source code.
     * Please use it consistently.

     * Description: A column of asterisks on the left   side,
     士 너ith beginning and ending almost寸江ank lines.
     士／
데이터는 한줄에 하나씩 코딩하여 다음과 같이 그 줄의 끝에 주석문을 추가하도록 합니다．




#define CLK_SET_RATE_GATE       BIT(o) I士 must be gated across rate change */
#define CLk_SET_PARENT_GATE     BIT(1) 1* must be gated across re- parent 士 /
#define CLK_IGNORE_UNUSED       BIT(3) 1* do not gate even if unused */




 커널연구회（w'사比kerne나川                                       정쟤준（rgbi3307@nate.com)
                                    44 / 351
                                                리눅스 커널 소스 해설 ［가초입문］
                                                        커널 소스 코딩 형식



구조쳬룔 설명하는 주석문은 아래와 같이 구조체 상단에 편집하고 구조체 멤버변수에 대한 설명은

이름앞에 ＠을 추가하여 설명하는 것이 관례화 되어 있습니다．



// 女 女


  * struct clk_hw - handle for traversing from a struct clk to its
  * hardware- specific structure. struct clk_hw should be declared within
  * clk_foo and then referenced by the struct clk instance that uses struct
  * clk_foo 's cik_ops
  火


  * @core: pointer to the struct clk_core instance that points back to this
  * struct cik hw instance

  * @clk: pointer to the per- user struct cik instance that can be used to
    into the clk API

  * @init: pointer to struct clk_init_ data that contains the mnit data
  * with the common clock framework. This pointer will be set to NULL once
  * a clk_register () variant is called on this clk_hw pointer.
  去／
struct clk_hw {
      struct clk_core *core;
      struct clk *clk;
      const struct clk_init_ data *init;
};

커널 소스 빌드 설정 파일인 Kconfig 파일은 다음과 같습니다. config 식별자들은 tab 만큼 들여쓰기

되어 있으나. help 다음에 있는 설명문들은 2 개의 공백문자만큼 들여쓰:7 ' 하는 것이 일반적입니다．




config AUDIT
      bool "Auditing support "
      depends on NET
         help
           Enable auditing infrastructure that can be used with another
           kernel subsystem, such as SELinux (which requires this for
           logging of avc messages output) . Does not do system- call
           auditing without CONFIG_AUDITSYSCALL.




  커널연구회（蜘쌔／.kerneL.bz)                                 정쟤준（rgbi3307@nate.com)
                                    45/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        커널 소스 코딩 형식




Macros, Enums

#define 으로 정의되는 상수는 대문자로 정의합니다．



#define CONSTANT 0x12345


열거형（enum)은 여러개 연관되어 있는 상수들을 정의할따1 사용합니다．



매크로는 한줄에 코딩해야 합니다. 매크로가 길어서 여러줄을 넘어갈때는 다음과 같이 역슬래시를

줄끝에 추가하여 계속 연속된다는 것을 알려 주어야 합니다. 아울러 do-while 블럭으로 묶어서

하나의 블럭으로 처리되도록 해주는 것이 좋습니다．



#define macrofun(a, b, c)
                                                  1
                                                  1




                                                  \\\
                                                  \
        do {
                if (a == 5)
                        do_this(b, c) ;
        } while (0)


아래와 같은 매크로 정의는 아주 나쁜 결과를 초래 합니다．




                                                  \\\\
#define FOO(x)
        do {
                 if   (blah(x) < 0)
                           return -EBUGGERED;
        } while (0)




커널연구회佃伽．ken｝텨,bz)                                        정재준（rgb13307@nate.com)
                                   46/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                      커널 소스 코딩 형식



FOO（지라는 함수 호출로 실행되는 것처럼 보이지만. 매크로는 코드 자체가 치환되어 삽입 되므로 이

코드가 삽입된 상위 함수가 종료（retrun) 되는 결과를 초래할 수 있고 분:
                                           71 되는 과정에 혼선이 생길 수

있습니다．



상위에서 정의된 매크로 상수를 재사용할때는 괄호로 묶어 주도록 합니다．



#define CONSTANT 0x4000
#define CONSTEXP (CONSTANT I 3)




커널 메세지 출력

커널 개발자들은 글을 읽고 쓰는 것을 좋아합니다. 커널 메세지는 약어나 비속어를 사용하는 것보다

표준어를 사용하여 출력하도록 합니다. 모호한 메세지보다 간결하고 명확한 메세지를 출력 하도록

합니다. 커널 메세지는 마침표로 종료하지 않아도 됩니다. 그리고 괄호 (%d）로 숫자를 인쇄하면 값이

추가되지 않으므로 주의 합니다．



커널 소스 헤더 파일인 <Liriux/device.h> 에는 디바이스 드라이버를 위해1 메세지를 출력 하도록

정해진함수인d色v_errO, dev_warnO, dev_info(）등을 사용합니다. 장치와상관없이 일반적인

메세지 출력은 <Linux/printk.h> 에 정해진 함수인 F兀noticeO, pr_mni이）, 1兀warnO, i口아r()

등을 사용합니다． pr_debug() 함수는 커널 소스 빌드 설정 상수인 CONFIG_DEBUG 가 정의 되어

있어야 동작합니다.




 커널연구회6사硏쌔ikerneLb기                                  정재준（呼)i3307@nate.com)
                                  47/ 351
                                                    리눅스 커널 소스 硼설 ［기초입문］
                                                            커널 소스 코딩 형식




메모리 할당

사용자들이 메모리 할당을 할따1 사용하는 함수와 유사하게 커널에서도 범용적으로 사용되는 메모리

할당 함수들이 있습니다．




kmallocQ, kza11oc ( ), kmafloc_array ( ), kca11oc ( ), vmaflocQ, vzalloc ()



p 가 가르키는 구조체 크기만큼 메모리를 할당할때는 다음과 같이 kn伯tloc(）을 사용합니다．




p = kmalloc (sizeof (*p) ,    . . . );



n 7H로 이루어진 배열을 할당할때는 아래와 같이 kmalL이＝카ray() 함수를 사용합니다．




p = kmalloc_array(n, sizeof (. . . )r . . . );



0 으로 초기화된 배열 메모리를 할당할때는 다음과 같이 kcaLloc() 함수를 사용합니다．




p = kcalloc (n, sizeof (. . . ), . . . );




inline 함수

함수를 ir山ne 으로 정의하면 속도가 빨라질 수 있지만. 오히려 역효과가 나타날 수 있습니다. inLine

함수는 코드가 매크로 처럼 치환되어 삽입되므로 코드 크기가 증가하여 메모리 캐시에 악영향을 줄 수




커널연구회（蜘,w.kerne나）z)                                     정재준（r야)i3307@nate.con分
                                         48 / 351
                                        리눅스 커널 소스 해설 ［기초입문］
                                                커널 소스 코딩 형식



있습니다. 따라서 함수안의 코드가 3 줄을 넘어가지 않는것에 한해서 inline 함수로 만드는 것을

권장합니다．




함수 반환값

함수는 다양한 종류의 값을 반환 할 수 있으며 가장 일반적인 것 중 하나는 함수의 성공 여부를

나타내는 값입니다. 이러한 값은 오류 코드 정수 (-Exxx = 실패, 0 = 성공）또는 성공한 논리값 (0 이면

실패, 0 이 아니면 성공）로 표시 될 수 있습니다. 이러한 경우가 아닌것들은 논리적인 버그가 나타날 수

있으므로 주의하여 함수 반환값들을 처리하도록 합니다．




bo아 사용

리눅스 커널의 bool 타입은 C99 표준 문법에 대해서 별칭을 부여한 것입니다. bool 타입은 0 또는 ]

로만 나타나며 fa匕e 또는 true 로 변환됩니다. 따라서 bool 타입으로 코딩할때는 0 과 ] 대신에 False

와 true 를 사용하도록 합니다. bool 을 사용하면 가독성이 좋아지므로 단순한 논리를 취급할때는

이것을 사용합니 다．



하지만 boo[ 논리가 반복적으로 나열되는 경우에는 1 비트 멤버 변수他化field）가 있는 구조체를

사용하는 것이 좋습니다．




 커널연구회佃째／w.kernet.bz)                         정재준（r야)13307@nate.com)
                             49 / 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 소스 코딩 형식



커널 매크로 활용

inc山de/Linux/kernel.h 헤더파일에는 유용한 매크로들이 많습니다. 여기에 있는 매크로를 충분히

활용하여 불필요한 매크로를 다시 정의하지 않는 것이 좋습니다. 예를들어, 배열의 크기를 계산하는

아래의 매크로는 아주 좋은 예제입니다．



#define ARRAY_SIZE(X) (sizeof (x) I sizeof ( (x) [O] ))




Inline assembly

인라인 어셈블리는 Cpu 아키텍쳐에 의존되는 코드 이므로 커널 소스 경로중0私I arch 경로에서 Cpu

종류별로 다르게 나타납니다. 인라인 어셈블리가 꼭 필요한 곳에서는 어쩔수 없지만. 가능한 C 언어를

사용하도록 합니다. 인라인 어셈블리 함수를 C 언어로 원형을 선언할때는 asmLinkage 을

사용합니다. C언어에 인라인 어셈블리를 삽입할때는 다음과 같이 asn）을 사용합니다．



asm ( "magic %regl, #42\n\ tT1
      "more_magic %reg2, %reg3"
      : ／士 outputs 火／ : ／士 inputs 士／ : ／士 clobbers 士／);




커널연구회如쌔쌔／,kerne比z)                                        정재준（r야月3307匣）nate.com)
                                    50/ 351
                                        리눅스 커널 소스 해설 ［기초입문］
                                         GCC 확장속성（attribute引




GCC 확장속성（atir小ute引

                        이번글주제는 " GCC확장속성（attributes) 이해" 입니다．

                        리눅스 커널 소스는 C언어로 코딩되어 있습니다. 그런데 커널
       GCC Attributes



       M
                        소스를 분석하다보면 기본적인 C 언어 코드외에 여러가지 생소한

                        문장들이 많이 나타납니다. 가장 대표적인 것이 C언어 전처리

                        문장들과 속성들（a比ributes) 입니다. 이러한 것들은 C언어

표준 문법외에 C 언어가 버전업 되면서 계속 추가된 것들입니다. C 언어 컴파일러는 GNU 에서 꾸준히

버전업하여 공개 및 배포하고 있습니다. 리눅스 커널 소스도 GNU 에서 버전업하고 있는 gcc 의

새로운 문장들을 도입해가면서 계속 버전업하고 있습니다. 그래서 예전에 C 언어 표준 문법만으로

소스를 코딩하다가 최신의 리눅스 커널 소스를 보면 아주 생소할 것입니다. 커널 소스를 처음에

분석할때1 바로 이러한 점 때문에 어려움을 겪게 됩니다. 커널 소스에는 C 언어 전처리 문장들과

속성들（attributes）이 생각보다 많이 등장합니다. 커널 소스를 이해하기 위해서는 C언어에 새롭게

추가되어 있는 전처리 문장들과 속성들（attrit川tes）에 대해서 알고 있어야 합니다. C언어 표준

문법도 많은데 이것까지 알아야 할까7에 대해서 너무 부담스러워하지 않아도 됩니다. 이것들의

개념이 생각보다 간단합니다. 알고 나면 별거 아님니다. 그냥 C언어 표준 문법내에서 컴파일 코드를

좀더 잘 만들기 위해서 컴파일러에게 힌트를 주는 수준입니다. 더더욱 다행스러운것은 이것에 대한

정보를 GNU 에서 상세한 문서로 모두 공개하고 있습니다．


아래는 GNU 웹사이트 주소입니다. 이곳에 GNU gcc 에 대한 정보들이 모두 있습니다．


https://gcc.gnu.org/


특히 GNU gcc 버전별 매뉴얼은 이곳에 전부 있습니다．




 커널연구회（낚쌔쌔／.kerneLbz)                         정재준似羚日307匣nate,com)
                              51/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                        GCC 확장속성（attribute引


https://gcc.g flu.org/ontinedocs/


내가 이글을 작성하고 있는 시점의 최신 GNU 9CC 버전은 8.2 이고 9.0 버전으로 업데이트

준비중입니다. 그리고 현재 제가사용하고 있는 9CC 버전은 7.3 입니다．


GN心gc心버젼합리스葛

GCC 8.2 released [2018-07-26]
CCC 7.3 released [2018-01-25]
GCC 7.2 released [2017-08-14]
GCC 6.4 reLeased [2017-07-041
GCC 6.3 released [2016-12-21]
GCC 6.2 reLeased [2016-08-22]
GCC 5.4 released [2016-06-03]
GCC 5.1 released [2015-04-221
GCC 4.9 released [2014-04-22]
GCC 4.6 released [2011-06-27]
//／이하 생략，,




이글을 작성하고 있는 주제인 " 9CC 속성들（attr巾utes) "은 버전 5.0 부터 등장했습니다． 참고로 9CC

가 아닌 C언어 컴파일러에는 속성들（attributes）이 없을 수도 있습니다. 리눅스 커널은 이러한 9CC

속성들（a比ributes）을 " include/linux/compiler_a比ributes.h" 소스 파일에 매크로 정의해서 모아

두고 있습니다. 이 소스파일을 보면 주석문으로 attr由utes 에 대한 설명과 함께 GNU 매뉴얼 링크가

있습니다. 내용이 많은편이어서 저는 다음과 같이 일부분만 가져 왔습니다. 대부분 #define 으로

정의된 매크로 입니다．


節C如d嘉加｝ux兀萌娜蜘巨r크比r小먀好．h 소스 일부분

#define _alias (symbol)             _attribute_ ( (_ alias_ (#symbol) ))




커널연구회（www.kernel.bz)                                         정재준（r야카3307@nate.com)
                                        52/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                      GCC 확장속성（attributes)



#define _aligned(x)            1attribute1      ( (_ aligned_(x) ))
#define 1 a1igned_1argest      1attribute_      ( (_ a1igned_ ))
#define 1 a1ways_inhine        1attribute_      ( (_ always_inhine_ ))
//／중간 생략．.
#define 1 printf (a, b)        1attributeH      ( (_ format_(printf, a, b) ))
#define m-1scanf (a, b)        _attribute_      ( (_ format__(scanf, a, b) ))
#define _gnu_inhine            1attribute_      ( (_ gnu_inline_ ))
#define    malloc              _attribute_      ( (_ malloc_ ))
#define _mode(x)               _attribute_      ( (_ mode1(x) ))
//／중간 생략．.
#define _packed                _attribute_ ( (_ packed_ ))
#define _pure                  1attribut已寸( (_下ure小）)
#define 1 section(S)           _attribute_ ( (1section_ (#S) ))
#define _always_unused         _attribute1e ( (_ unused_ ))
#define _maybe_unused          _attribute_ ( (1unused_ ))
#define    used                _attribute_ ( (_ used1) )
#define    weak                _attribute_ ( (_ weak_ ))




내용이 눈에 들어 오나요? C 언어 표준 문법인 #define 매크로 정의에 대해서 잘 알고 있다면 위의

내용이 바로 이해가되고특별히             attribute    키워드로표현하고있는attributes속성에 대해서만

이해하시면 됩니다. 일단 C언어 표준 문법부터 점검해 보도록 하겠습니다. 우리가 #define 으로

매크로를 정의할때 보통 다음과 같이 작성합니다．



#define p1 3.141592


F기 는 3.14佰92 로 정의 됩니다. 이것과 마찬가지로，



#define _packed   _attribute_(L....packed. J)


_packed 는1attrib止e_( ...packed. J）로 정의 됩니다. C 컴파일러는 컴파일 시점에서

_packed 을 만나면 이 단어를 1 a比ribute_(L..packed.J）로 치환（바꿈）합니다. 즉，

_attribute_(L..packedJ）로 소스 작성한 것과 동일합니다. 그럼 오귀1이렇게 할까요？ 우리가




 커널연구회（蜘,w.kerne比z)                                         정재준（r야)i3307@nate.com)
                                        53/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                 GCC 확장속성（attribute引


3.141592 룔 pi 로 작성하면 한결 간편해1 지듯이 1크比ribute_((니）acked. .J）을 _packed 로

작성하면 좀더 간결하기 때문입니다. 다면 컴파일러가 이렇게 치환（바꿈）한다는 것을 이해하는

과정이 필요할 뿐입니다．


자，이제 남은 것은Ha比ribute1속성을 이해하는 것입니다. 이것에 대해서는 GNU gcc 매뉴얼 494

페이지 " 6.37 A比ribute Syntax" 에 잘설명되어 있습니다. 문법은 다음과같습니다．


_attribute_((attribute-List))   볏숫小＼ 畔J 족성 선의


attribute-List로 나열한 속성을 컴파일러에게 지시해 주는 것입니다. attribute-List 로 나열하는

속성은 다음과 같은 종류가 있습니 다．


attr小ute七就 속성 종류（뵨류

Type 속성
Function 속성
Labe[ 속성
Enumerator 속성
Statement 속성



앞의 설명에서 인지 하셨겠지만, 여기서 "속성 "은 컴파일러에게 해당 문장을 해석할따1 참고하라고

지시하는 힌트라고 보시면 되겠습니다．


Type 속성은 변수나 데이터 타입에 대해서 속성을 부여합니다. 예를들면．


intx= O; /／일반적인 변수 정의
intx.m就tr由uteH（伯Ligned (16))) = 0; //16 바이트 단위로 맞추라는 속성




커널연구회佃쌔쌔／.kerr泡.bz)                                 정재준（rgb13缸刃＠nate.con力
                                     54/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                         GCC 확장속성（attribute引



struct S { short f[3]; } /／일반적인 구조체 선언
struct S { short f[3]; } _attribute_ ((aLigned (8))); 1/8 바이트 단위로 맞추라는 속성


Fundt向n 속성은 함수에 대해서 다음과 같이 부여 합니다．


V이d士my_a hod]（引ze_t); /／일반적인 함수선언
VOI(卄 my_a hod]（引ze_t) H a吐rib毗e_((assu畔_atigned(16))); //16 바이트 단위로 맞추라는
속성


Label 속성은 레이블（분기위치）에 대해서 다음과 같이 부여 합니다．


ErrorHandling:     _attribute_((cold, unused));


Enumerator 속성은 열거형 자료에 대해서 다음과 같이 부여 합니다．


enum E { oldvah _attribute__((deprecated)), newvah };


Statement 속성은 문장에 대해서 다음과 같이 부여 합니다．


switch (cond) {
        case 1:
        bar (1);   _attribute_((faRthrough));
        case 2:


}

어떤가요？좀 정리가 되나요7


위의 내용을 다시 요약하면, 속성은 C 언어 문장에 대해서 다음과 같은 문법으로 부여 합니다．


_attribu te_((attribute-hist))




    커널연구회佃쌔iw.kerneh.b라                                     정재준（rgt必307@nate.com)
                                          55/ 351
                                      리눅스 커널 소스 해설 ［기초입문］
                                       GCC 확장속성（attribute引



여기서 attribute七St 로 나타나는 것들이 상당히 많아서 다소 복잡하1 보입니다만, 속성에 대한 문법은

위와 같이 간단 합니다. 이제 문법적인 내용들은 설명했기 때문에 앞으로는 attribute-list 에 대해서

이해하면 되겠습니다. a比ibute小St 는 종류71 많기 때문에 이글을 통해서 모두 설명하기는

힘듭니다. 몇가지 예제만 이해하시면. 문법적인 내용은 모두 동일하므로 새로운 attr小ute-List 가

나오면 GNU 매뉴얼이나 인터넷 검색을 통해서 익히시면 되겠습니다.




커널연구회（邸쌔／.kern이.b力                         정재준（rgb日307@nate.com)
                           56/ 351
                                     리눅스 커널 소스 해설 ［기초입문］
                                            커널 데이터 타입 이해




커널 데이터 타입 이해1


      六
     Kernel DataType
                       리눅스 커널 소스는 방대합니다. 그 많은 소스들을 한꺼번에

                       이해하기란사실상 힘듭니다. 저도 처음에는 단기간에 커널



   거4
                       소스들을 이해하기 위해서 많은 노력을 했습니다. 하지만

                       의욕만 있었고 시간이 지날수록 의욕 만큼이나 실망과 좌절감이

                       밀려 왔습니다. 이제와 돌이켜 생각해 보면 한마디로 " 기본에

충실하지 못했습니다". 모든 분야들이 그러하듯이 기본7匡 튼튼히 다져야 합니다. 뿌리가 튼튼한

나무는 거대하게 자라도 흔들림이 없습니다. 불안하지 않습니다. 그래서 리눅스 커널 소스도

기본부터 탄탄히 다지면서 소스를 단계적으로 분석해야 합니다. 시간이 걸리더라도 기본부터

차근차근 하다보면 언젠가는 큰산맥이 될 것입니다. 앞으로 이러한 과정들을 블로그를 통해서 공유해

나가도록 하겠습니다．


자 이제 시작입니다. 즐커분（즐거운 커널 분석）합시다．



첫번째1 주제로 "리눅스 커널에서 데이터를 취급하는 방법 " 에 대해서 단계적으로 이해하는 방법들을

공유하도록 하겠습니 다．



우리가 접하는 대부분의 시스템은 일반적으로 다음과 같이 동작합니다．



입력 1=> 처리 1=> 출력




 커널연구회（납쌔쌔／.kerne나파                       정재준（r야)13307@nate.con力
                           57/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                 커널 데이터 타입 이해



위에서 입력, 처리, 출력하는 대상（목적）물은 무엇일까요7 여러가지 대답이 나올 수 있겠지만 "

데이터 " 가 가장 일반적일 것입니다. 따라서 대부분의 시스템에는 입출력하는 데이터가 있고 이것의

표현 방법이 중요하면서도 가장 기본이 됩니다. 우리의 시스템이 컴퓨터라면 "입력（데이터）小＞ 처리

（계산）H＞출력（데이터）" 형태로처리 됩니다. 따라서 "데이터 표현을어떻게 할것인가？"가

중요합니다. 데이터 공학적인 학문으로는 자료구조로 연계되어 집니다만, 여기서는 일단 리눅스 커널

소스안에서 데이터를 표현하는 기본적인 기법을 알아 보겠습니다. 리눅스 커널은 C언어로 소스

코딩되어 있으므로 C 언어의 데이터 타입 표현 방법이기도 합니다. C 언어에서 표현하는 기본적인

데이터 타입은char, m t1 tong.. 등등이 있습니다. 리눅스커널도 이것을사용합니다. 보통

어플리케이션을 작성할때는 해당 언어에서 제공하는 데이터 타입을 그대로 잘 선택해서 사용하면

됩니다. 그러나 커널에서는 다음과 같이 좀더 알아야 할것들이 있습니다．



먼저, CPU 종류（x86, AR卜4.卜시PS, 끼SC八／, 등등..）를 구분해야 합니다. cPu 종류마다 실행되는

명령어셋(ISA）이 다르므로 C 언어 컴파일러도 다릅니다. 그래서 C 언어 컴파일러 종류에 대해서도

지식이 있어야 합니다. C 언어 문법 공부하기도 벅찬데 Cpu 와 컴파일러에 대해서도 알아야 한다고

미리 걱정하지 마세요. 하나씩 단계적으로 알아가면 됩니다. 사실 리눅스 커널 소스를 보면 이러한

내용들이 있기 때문에 차근차근 익혀 나가면 됩니다. 학교에서 컴퓨터관련 전공을 하셨고 C 언어

문법을 어느정도 알고 있으면 앞으로 좀더 수월하겠지만. 저도 사실 학창시절에 컴퓨터관련 전공

공부도 많이 하고 특히 컴퓨터구조와 자료구조 알고리즘에 대해서 배우기는 했지만 ，이론적인 지식에

불과해서 사실 제대로 적용하는 방법을 모르고 어플리케이션하기에 바빴습니다. 그러나 리눅스 커널

소스를 하나씩 분석하다 보면 CPU 가 어떻게 동작하고 C 언어 컴파일러가 이것에 맞게끔 어떻게

컴파일되어 실행되는지 실제적으로 이해할 수 있습니다. 하나씩 알아가는 재미로 하면 됩니다. 저도

예전에는 힘들게만 느끼든 것들을 기본부터 하나씩 익혀가며 정리하는 재미로 이글을 적고 있습니다．

사족이 너무 많이 달린듯 하네요. 이제 본론으로 들어 갑니다．




커널연구회佃쌔쌔／.kern이.bz)                            정재준（rgbi3307@)nate.coa分
                              58/ 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                           커널 데이터 타입 이해1



저는 댜음과 같이 CPU 종류별로 C 언어 컴파일러를 사용하고 커널 소스를 서로 비교해 나갈

예정입니다. 리눅스 커널 소스는 항상 최신 버전을 페치 받아서 소스 분석합니다. 제가 이글을

작성하는 시점에서 리눅스 커널 최신 버전은 " 4.20" 입니다．


첫째, x86_64 비트용 컴파일러를 사용합니다． 컴파일러 정보는 다음과 같습니다．



$gcc-v

COLLECT_GCC=gcc
Target: x86_64-linux- gnu
gcc version 7. 3. 0 (Ubuntu 7. 3.0- 27ubuntu1--18. 04)




둘째I, ARM 64 비트용 컴파일러를 사용합니다. 컴파일러 정보는 다음과 같습니다．



$ aarch64-Linux-gnu-gcc -v

COLLECT_GCC=aarch64-linux- gnu- gcc
Target: aarch64-linux- gnu
gcc version 7. 3. 0 (Ubuntu/Linaro 7. 3. 0- 27ubuntu1-18. 04)




세째1, RISC-V 64 비트용 컴파일러를 사용합니다. 컴파일러 정보는 다음과 같습니다．



$ riscv64-unknown-eLf-gcc -v

COLLECT_GCC=r15cv64 - unknown - elf - gcc
Target: riscv64- unknown- elf
gcc version 7. 2. 0 (GCC)




 커널연구회（邸胛．kerneLb기                                         정재준（rgbi3307@nate.com)
                                       59/ 351
                                                                 리눅스 커널 소스 해설 亘카麥입푼j
                                                                        커널 데이터 타입 이해



위의 컴파일러들이 모두 설치되어 있지 않다고 걱정하지 마세요. 먼저, x86 64 비트용 컴파일러를

사용할 예정입니다. IBM-PC 노트북에 우분투(18.04 버전）을 설치햐면 gcc 컴파일러는 자동으로

설치 됩니다. 우선 이것을 사용할 것입니다. 나머지 컴파일러에 대해서는 점차적으로 설명할

예정입니다. 특별히 저는 데SC-v 아키텍쳐에 대해서 관심이 많아서 향후 이것에 대해서 커널 소스가

어떻게 구현되어 있는지 기술하는 내용이 많아질듯 합니다．


먼저, 우리가 C언어를 사용하여 일반적으로 데이터 타입（char, short, int, Long）들을 정의하는

예제입니다. 아래 예제에서는 typedeF문으로 데이터 타입을 재정의 했습니다． char==s8,

 sho比＝=sl 6, int==s32, Long==s32 or s64 로 재정의 했습니다. 소스 컴파일은 x86_64 비트용

 컴파일러를 사용해서 실행했습니다．


data/typeOl.c 소스

／出火
           M: JaeJoon Jung <rgbi3307但）nate.com>
           W: https://＼사硏／小／.kerne나끄
           F: data/typeOl .c
           This program is free software; you can redistribute it and/or
           modify it under the terms of the GNU General Public License
  火／
 #include <stdio.h>
荊nc山de <stdtib.h>


 typedef char s8;
typedef unsigned char u8;
typedef short Si 6;
typedef unsigned short ul 6;
typedeF mnt s32;
typedeF unsigned mnt u32;




       커널연구회（的,w.kerne나끄）                                                  정재준（rgbm3307@nate.com)
                                               60/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                    커널 데이터 타입 이해1



typedef Long s64,
typedef unsigned Long u64J
typedef Long long s64;
typedef unsigned Long long u64;


mnt main()
{
        printf(" s8 = %Lu bytes\n", sizeof(s8));
        printf(" u8 = %Lu bytes\n", sizeof(u8));
        printf("s16 = %Lu bytes\n", sizeof(s16));
        printf("u16 = %Lu bytes\n", sizeof(u16));
        printf("s32 = %Lu bytes\n", sizeof(s32));
        printf("u32 = %Lu bytes\n", sizeof(u32));


        pu ntf("s64_= %Lu bytes\n", sizeof(s64J);
        printf("u64_= %Lu bytes\n", sizeof(u64J);
        printf("s64 = %Lu bytes\n", sizeof(s64));
        printf(" u64 = %Lu bytes\n", sizeof(u64));


        return 0;
}



실행결과는 다음과 같습니 다．



data/ty必01.

s8 = 1 bytes
u8 = 1 bytes
引6 = 2 bytes
山6 = 2 bytes
s32 = 4 bytes
u32 = 4 bytes
s64_= 8 bytes




    커널연구회（납쌔／寸,.kerne나）기                                         정재준（四t心307@nate.com)
                                                   61/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                 커널 데이터 타입 이히1



u64_= 8 bytes
564= 8 bytes
u64 = 8 bytes




char는 데이터 타입 크기가 1 바이트, short 는 2 바이트, mnt는 4 바이트，Long 는 8 바이트Long

Long 는 8 바이트로 결과가 나왔습니다. 여기서 char는 CPU 종류에 상관없이 1 바이트（8 비트）

입니다. 그러나 나머지 데이터 타입들은 CPU 종류에 따라서 달라질 수 있습니다 ．특히 Long 타입은

32 비트 CPU 에서는 4 바이트（32 비트）이고 64 비트 CPU 에서는 8 바이트（64 비트）입 니다． 저는

위의 예제를 x86_64 비트 CPU 에서 컴파일하여 실행 했으므로 8 바이트（64 비트）가 나왔습니다．

그리고 Long Long 타입은 32 비트／64 비트 CPU 에 상관없이 8 바이트（64 비트）입니다．


위와같이 데이터 타입 크기는 CPU 종류마다 다를 수 있기 때문에 typedef 을 사용하여 그 크기를

인지할 수 있는 이름으로 재정의하는 것이 좋습니다. 그리고 커널에서는 fLoat 실수형 타입을

사용하지 않습니다. 커널 코드는 속도가 빨라야 합니다. 소수점이 포함된 실수형 데이터는 소수를

처리하기 위한 코드가 많아져서 속도 저하가 발생합니다. 그래서 커널은 실수형을 사용하지 않습니다．

모두 정수형을 사용합니다. 그럼 커널 내부에서 실수는 어떻게 처리할까요7 정수들을 사용하여 조금

특별한 알고리즘을 사용하는데 이것은 나중에 설명하도록 하겠습니다 ．우선 위의 예제를 통하여

typedef 문을 굳이 사용해야 하는 이유부터 알고 가야 합니다．


리눅스 커널은 데이터 타입의 크기를 엄격하게 지켜서 데이터 공간（메모리）초과佃verf (ow）와 잘림

(underf Low) 문제를 효율적으로 해결합니다. 이렇게 하기 위해서는 커널이 원하는 만큼의 데이터

타입 크기를 정확하게 정의할 필요가 있습니다. 그래서 typedef문을 사용하여 CPU 종류와

컴파일러에 따라서 데이터 타입을 정확하게 정의합니다. 커널은 8 바이트（64 비트）타입을 정의하기

위해서 long 형은 사용하지 않습니다． 반드시 Long Long 형을 사용하여 확실히 8 바이트（64 비트）




 커널연구회佃쌔iw.kerne나江）                             정재준（四bi3307@nate.com)
                              62/ 351
                                                                  리눅스 커널 소스 해설 ［기초입문］
                                                                         커널 데이터 타입 이해1



 타입을 정의 합니다. 아래 예제는 리눅스 커널 소스에서 데이터 타입 정의하는 부분을 내가 따로

 떼내어서 검증하기 위한 단독 실행 소스로 만들었습니다．



data/typeC              소스

／士出
              M: JaeJoon Jung <rgbi3307@nate.com>
              W: https://www.kerneLbz
              F: data/type02.c
              丁h朽 江ogram is 升ee soft寸局re; W싸 can redistribute it and/or
              modify it under the terms of the GNU General PubUc License
士／
胡nc山de <std向.h>
嫩nc山de <stdLib.h>


///include/uapi/asm-generic/int-1164.h
 typedef 艸夕gned_ 小ar H s8;
 typedef unsigned char _u8;
 typedef 啣針gned如short 1引6;
 typedef unsigned shortmHu16;
 typedef 的多因的d叫 mnt 1 s32;
 typedef unsigned int_ u32;


荊fdeF          GNUC
=mexte陌ionm I卯edef叫多的ed_ Long Long _s64;
_extension_ typedef unsigned Long Long _u64;
  #eLse
      typedef _signed_ Long Long _s64;
      typedef unsigned Long Long _u64;
      #end汁


      ///inctude/asm-generic/int-L164.h
      typedef_s8 s8;




       커널연구회佃／硏／니ikerneL.bz)                                               정재준似拘i3307@nate.com)
                                                 63/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                    커널 데이터 타입 이해1



typedef_u8 u8;
 typedef_s16 s16;
 typedef_u16 u16;
 typedef_s32 s32;
 typedef_u32 u32;
 typedef_s64 s64;
 typedef_u64 u64;


    nt main()
{
           piintf(" s8 = %(u bytes\n", sizeof(s8));
           printf(" u8 = %Lu bytes\n", sizeof(u8));
           printf("s16 = %(u bytes\n' , sizeof(sl 6));
          printf("ul 6 = %Lu bytes\n'', sizeof(u16));
           printf("s32 = %Lu bytes\n" , sizeof(s32));
          printf("u32 = %Lu bytes\n'', sizeof(u32));
          printf("s64 = %Lu bytes\n",sizeof(564));
          printf( 'u64 = %Iu bytes\n" , sizeof(u64));
          return 0;
}



실행결과는 다음과 같습니다．



 da由九如的2七 실행꿜콰「

s8 = 1 bytes
u8 = 1 bytes
s16 = 2 bytes
山6 = 2 bytes
s32 = 4 bytes
u32 = 4 bytes
s64 = 8 bytes
u64= 8 bytes




 커널연구회（www.kernel.bz)                                            정재준（rgb日307@nate.com)
                                                  64 / 351
                                      라뉵스 캬널 소스 斟輦 ｛가姦입문I
                                             커널 데이터 타입 이해




실행결과는 typeOl .c와 동일합니다. 그러나 몇가지 중요한 점들이 있습니다. type02.c 소스어虐

다음과 같이 C 컴파일러 확장（extens向n) 지정자들이 몇가지 보입니다．


中읽gned叫m


崩fdef   GNUC


 extens泊n


이것은 C 컴파일러마다 소스 코드를 해석하는 방법을 명확히 지정해 주71 위함입니다. ,msigned叫m는

gcc 컴파일러가 -trad止向na[ 로 되어 있으면 읽gned 라는 키워드를 해석하지 못하기 때문에 이것을

명확히 해석하도록 지정해 주는 것입니다．


前fdef小GNUC如는 컴파일할때 ,GNUC如 가 정의되어 있으면 士如ns幻nH지정을 개서
                                             \=1


소스를 컴파일 합니다. GNUC 컴파일러에 맞도록 컴파일 해주71 위해서 컴파일 시점에 조건倂咐을

부여하여 컴파일햐게 됩니다．


리눅스 커널 소스어虐 위와 같이 컴파일러 확장（extens向I1) 지정자들이 많이 나타납니다. 리눅스

소스 컴파일을 Cpu 와 컴파일러 종류에 따라서 다르게 해석될 수 있는 키워드를 정확하게 해석하도록

바로 잡아 주는 것입니다. 모두 C 언어 문법을 잘 지키71 위해서 파생된 것 입니다. 리눅스 커널

소스를 분석할따1 이런것들 때문에 처음어七 소스가 이상하게 보일 수도 있지만 ，기본 문법을 크게

벗어나지 않는 것들이므로 나올따1 마다 하나씩 익혀 가면 되겠습니다．




 커널연구회（뻐wwkerneLb기                           정재준（四bi3307@nate.com)
                           65/ 351
                                                               리눅스 커널 소스 해설 ［기초입문］
                                                                      커널 데이터 타입 이해



 그럼 위와 같이 데이터 타입을 s8, u8, s16, 山6, s32, u32, s64, u64로 정의하면 정확한 크기로

데이터 변수들을 사용할 수 있게 됩니다. 위의 type02.c 소스에 있는 데이터 타입을 앞으로 계속

사용하기 위해서 다음과 같이 헤더 파일로 보관합니다．



data/1ype02.h 헤1더파일

／出火
        M: JaeJoon Jung <rgbi3307흐）nate.com>
        ＼사： h따瓜끄＼A八ww.kerr泡.bz
        F: data/type02.h
        This program is free software; you can redistribute it and/or
        modify it under the terms of the GNU General Public License
火／
///incLude/uapi/asm-generic/int小64.h
typecleF _signed_ char _s8;
typedef unsigned char _u8;
typedef _signed_ short _516;
typedef unsigned short _u16;
typedef _signed_ mnt _s32;
typedef unsigned mnt _u32;


荊fdef    GNUC
_extension_ typedef _signed_ long Long _s64;
_extension_ typedef unsigned long Long _u64;
#eLse
typedef_signed_ long long _s64;
typedef unsigned long long _u64;
#end汗


///iaclude/asm-generic/int4L64h
typedef_s8 s8;
typedef.Hu8 u8;
typedef_s16 s16;




커널연구회佃쌔,w.kerne나准）                                                      정재준（rgbi3307@nate.com)
                                            66/ 351
                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                           커널 데이터 타입 이해1



  typedef_u16 u16;
  typedef_532 s32;
 typedef_u32 u32;
 typedef _s64 s64;
 typedef_u64 u64;




위의 내용을 바탕으로 여러가지 데이터 타입들을 재정의할 수 있습니다． 아래의 data/1ype03.h

헤더파일은 위의 내용을 바탕으로 데이터 타입들을 재정의 했습니다. 리눅스 커널 소스

include/Linux/types.h 소스를 보시면 아래와 같이 데이터 타입들이 typedef 을 사용하여 재정의

했습니다．



data/typeO玉a 헤더파임
／士士
            卜4: JaeJoon Jung <rg씨3307匣珀就e.c아n>
             ＼사： https://硏／니／낚／.kerneLbz
             F: data/type03.h
             This program is free software; you can redistribute it and/or
             modify it under the terms of the GNU General Public License
 士／
 ///inctude/linux/types,h
／火 bsd 火／
      typedef unsigned char u_char;
      typedef unsigned short u_short;
      typedef unsigned mnt u_int;
      typedef unsigned long u_long;


      尸 sysv 央／
      typedef unsigned char unchar;
      typedef unsigned short ushort;




       커널연구회佃쌔iw.kerneLbz)                                                   정재준（rgbi3307（흐｝nate,com)
                                                  67/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                             커널 데이터 타입 이해



 typedef unsigned mnt uint;
 typedef unsigned long ulong;


＃作ndef     B나 TYPES DEFINED
 #define   B汗 TYPES DE디NED
 typedef u8 u_1nt8_t;
 typedef s8 1nt8_t;
 typedef u佰 u_intl 6_t;
typedef s16 int16_t;
typedef u32 u_int32_t;
typedef s32 int32_t;
#endif／出 1.C쫴T꺄PES_D댜INED_J 火／


typedefu8 山nt8上
typedef u16 미毗化上
typedef u32 미n132上


///#if definedL_GNUC__)
#if definedLGNUCj
typedef u64 uin164_t;
typedef u64 u_int64_t;
typedefs6이毗64上
#end汗


荊fdef CONFIG PHYS ADDR 丁 64B11
typedef u64 phy乞的먀上
#else
typedef u32 phy乞拍먀上
#end汗


///include/uapi/asm-generic/posix_types.h
typedef unsigned long _kernel_ulong_t;
typedef _kernel_미애오t 1 kernele引昶上
typed可Hkernel size I시ze上




 커널연구회（www.kerne나）力                                      정재준（rgbi3307@nate.com)
                                            68/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                       커널 데이터 타입 이해




모두 C 언어의 데이터 타입을 typedef문으로 재정의 한 것이므로 위의 소스를 충분히 이해할 수 있을

것입니다． 몇가지 조건 컴파일문（＃汗）이 있습니다만, 컴파일할따1 해당 상수가 정의 되어 있으면

컴파일하고 없으면 컴파일 대상에서 제외하는 방식이므로 충분히 이해할 수 있습니다. 위의

data/type02.h 헤더파일과 data/1ype03.h 헤더파일은 앞으로 계속되는 실습 소스에

인클루드하여 사용할 예정입니다．


지금까지 언급한 데이터 타입 선언자를 사용하여 해당 데이터 타입에 저장할 수 있는 데이터 최소값과

최대값에 대해서 알아보도록하겠습니다. 리눅스 커널 소스 파일 " include/Linux/kernel.h"를 보면

다음과 같이 데이터 타입별로 최소값과 최대값을 매크로 상수로 정의한 부분이 있습니다．


include/Linux/k亘rn立

#define USHRT_MAX ( (u16) (- OU) )   U차大
#define SHRT_MAX ( (s16) (USHRT_MAX>>1) )
#define SIIRT_MIN ( (s16) (- SHRT_MAX - 1) )
#define INT_MAX ( (int) (- OU>>l) )
#define INT_MIN (- INT_MAX - 1)
#define UINT_MAX (- OU)
#define LONG_MAX ( (long) (- OUL>>1) )
#define LONG_MIN (- LONG_MAX - 1)
#define ULONG_MAX (- OUL)
#define LLONG_MAX ( (long long) (- OULL>>l) )
#define LLONG_MIN (- LLONG_MAX - 1)
#define ULLONG_MAX (- GULL)
#define SIZE_MAX (- (size_t) O)
#define PHYS_ADDR_MAX (- (phys_addr_t) O)

#define U8_MAX ( (u8)-OU)
#define S8_MAX ( (s8) (U8_MAX>>1) )
#define S8_MIN ( (s8) (- S8_MAX - 1) )
#define U16_MAX ( (u16) -OU)
#define S16_MAX ( (s16) (U16_MAX>>1) )
#define 516_MIN ( (s16) (- 516_MAX - 1) )
#define U32_MAX ( (u32) -OU)




 커널연구회佃쌔사／.kerne比z)                                 정재준（띠t必3307@nate.com)
                                    69/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                             커널 데이터 타입 이해



#define S32_MAX ( (s32) (U32_MAX>>1) )
#define S32_MIN ( (s32) (- S32_MAX - 1) )
#define U64_MAX ( (u64) -OULL)
#define S64_MAX ( (s64) (U64_MAX>>1) )
#define S64mMIN ( (s64) (-564_MAX - 1) )



위의 매크로 정의 내용을 보면 C 언어의 쉬프트 연산자（>>）와 보수（D 연자등을 사용하여 데이터

타입의 최소 크기（M八）와 최대 크기（MA지를 정의하고 있습니다. C언어 쉬프트 연산자（>>）와 보수

G) 연산자는 이진수 비트 단위로 데이터를 연산합니다. 이 연산자에 대한 기본 문법은 C 언어 문법

책이나 인터넷에서 검색해 보시면 내용이 많으므로 여기서는 따로 설명하지 않습니다. 저는 이 글을

읽는분들이 C 언어는 어느정도 알고 계시다는 가정하에 내용을 기술하고 있다는 것을 양하1

부탁드립니다. 위의 매크로에서 중요한 것은 데이터 타입별로 그 크기를 어떻게 정의하고 있는가를

이해하는 것이 중요합니다. 우리가 어플리케이션 코드를 작성할때 내가 정의한 데이터 타입에 저장할

수 있는 최대값과 최소값에 대해서 고민을 해 보셨을 겁니다. C 언어 특히 리눅스 커널에서는 위와

같이 데이터 타입별 최대값과 최소값을 정의 합니다. 아주 간결합니다.


CPU 가 십진수 데이터 ] ] 을 표현하는 예를 한번 들어 보겠습니다. CPU 는 논리연산장치이므로

십진수를 이진수로 변환하여 처리합니다. 십진수 ]] 은 이진수로 ]01] 입니다. 이것을 32 비트 CPU
                                                                                              八1




                                                                                              却
                                                                                   /\'＼
에는 다음 그림과 같이 표현합니다．




313029 2827 26 25 242322 21 20 19 18 17 18 15 14 13 12 11 10 9 8   7   6   5   4          3 2      1   0

 0 0    0 0   0 0 0 0 0 0 0 0      0 0 0 0 0 0 0 0 0          0 0 0            0          1   0 1 I

                                     (32 出t弓 wid햐




32 비트 CPU 에서 데이터 표현은 32 비트를 이진수로 나열하여 0 부터 최대 42 억 9 천 4 백 9 십 6 만

7 천 2 백 9 십 S 까지 표현됩니다. 아래는 이것을 나열한 것입니다．




커널연구회佃쌔쌔／.kerne나끄）                                            정재준（rgbi3307@nate.com)
                                      70/ 351
                                             리눅스 커널 소스 해설 ［기초입문］
                                                    커널 데이터 타입 이하1


                                                             0
0000 0000 0000 0000 0000 0000 0000 0000,, , -
                                                             n n n 1
                                                             e 庶 e 1
0000 0000 0000 0000 .0000 0000 0000 0001t,. 出
0000 0000 0000 0000 0000 0000 0000 0010t,. 毖                 卜L   卜L   卜뇨



                                                              斗i工 O  亡    1

1111 1111 1111 1111 1111 1U1 11.11 1101. , . = 乞29吼967, 293,, ,
1111 1111 1111 1111 1111 1111 1111 '110twa 弩 屯 294 , 967 , 294t母.
1111 1111 1111 1111 1111 1111 1111 111L ' 曲 乞 294 , 967, 295k昏，


위의 32 비트 이진수 나열은 숫자를 모두 양수（unsigned）로 표현한 경우입니다． 음수佃gned）는

어떻게 표현할까요？ 음수는 다음과 같이 최상위 비트（3] 번째）가 0 이면 양수. ] 이면 음수로

구분합니다. 양수는 최대 2] 억... 음수는 최대 .2] 억... 까지 표현됩니다．



뻐000 0000 0000 0000 0000 0000 0000 0000t,.
                                                                              臂디 그와 唵e늑 士泓서
j 00D 0000 0000 0000 0000 0000 0000 0001t*.
  000 0000 0000 0000 0000 0000 0000 0010「' " : 三：
                                                ,:                             허計'臣긔中邑 " ' 4川디毛蚌 '

   111111
뻐ill       1111 nll
      llll lll} 1111 llll
                     1111 llll
                          1111 llll ll8lt*. - 2,147, 4B3, 645t帥
                               1111 1i0it*.
   11 llll
qlll  1111 llll
           1111 llll
                1111 llll 1111 llll
                     1111 llll      lll0t,. = 2j47,483, 646ten
                               1111 1110t,.
L 1ll
上
4  11 llll
      1111 llll
           1111 llll
                1111 llll
                     1111 llll
                          1111 llll
                               1111 1111m0
                                    llll十니， = 2 ' '47 '483 '647ten
  000 0000 0000 0000 0000 0000 0000 0000t*. 缸 ' 2J47,483! 645ten
 l l
  000 0000 0000 0000 0000 0000 0000 000lt.,, 싹 -2,147,48工647,,,,
  000 0000 0000 0000 0000 0000 0000 0010t찌. 心 -2J47,483,646t蝕
 1l                                                                              '     1凸




上
斗
  111 1111 1111 1111 1111 1111 1111 1101t, . 澍 t帥
  111 1111 1111 1111 1111 1111 1111 1110m昏 骨 艸2t帥
 4
 上
 小
  111 1111 1111 1111 1111 liii 1111 1111t札    卞   艸   It蟹忖
그럼 64 비트 Cpu 에서는 이진수 비트를 어떻게 처리할까요？ 32 비트0私I 처리하는 방식과

동일합니다. 다만. 비트수가 32 비트에서 64 비트로 늘어납니다．


64 텍辱C原'Jo'사이진수1011 표剋




 커 널연구회（납川,w.kerneLb기                                              정재준（I야)13307@nate.com)
                                71/ 351
                                                            리눅스 커널 소스 해설 E기초입문］
                                                                   커널 데이터 타입 이히1



 球斗 由 61 毓15958 57 56 弱 5耳 53 必 53 的 邱甘 心B47 4撰                          a多 3837 邦 35

 [ oo小 . 0000므크흐끄Pk！으으a . 肛也 00 . . 0 0 0 打
  拉1 絮） 2928 호7 26 25 24 23 22 袞支 2甘始 玉8 17 1吝 生珏 141312 支I 拭多 好 8 7 6         5 4 3    衾   I   各

            0 0 0 0    . . 。하。。’"’可하. 00小小 . 으巨. . C)
                            (64 bits wide, split into two 32btt r州s)




64 비트 CPU 에서 데이터 표현은 64 비트를 이진수로 나열하여 0 부터 최대 ]844 경...까지

표현됩니다. 아래는 이것을 나열한 것입니다．




   000000（殆 0000 口00 {} 00000 {：卜00 （표표) 00000 000000［兀1 00000000
 00000000 0的000口0作戶 0乙숀fl
   0 泌珀00 承｝00000000 0000口000 00000000 00000000 00000000
 00000000 0口0口Dl拍1t的싹 1之密：,
   DC卜分口口DCC 00000000 00｛珀 0000 00000000 00000000 00000000
 00000000 00000010蜘j 乙，余：,


  11111111 11111111 11111111 11111111 11111111 11111111
11111111 11111101鈿芦 18, 446, 774, 07:3,了09, 551尹 613致魂n
  11111111 11111111 11111111 11111111 11111111 11111111
11111111 11111110之甘心舒 18, 碌46, 744, 073, 709, 551, 614t愈.
  11111111 11111111 11111111 11111111 11111111 11111111
11111111 11111111乞甘心心 18, 446, 744, 073, 709, 551, 6I5.*::



위의 64 비트 이진수 나열은 숫자를 모두 양수（unsigned）로 표현한 경우입니다. 음수佃gned）는

다음과 같이 최상위 비트（63 번째）가 0 이면 양수, ] 이면 음수로 구분합니다. 양수는 최대 922 경．..

음수는 최다I -922 경...까지 표현됩니다．




커널연구회（＼사노사小,.kernet.bz)                                                정재준（rgb13307（令nate.com)
                                         72/ 351
                                                     리눅스 커널 소스 해설 ［기黍입문］
                                                            커널 [:1'이터 타입 이해



        00000000 00000000 000.00000 00000000 00000000 0.0000000
      0f卜D00000tY，
                 凸= qen
         00000000 00000000 00000000 0.0000000 00000000 00000000
      00000001乞甘c= 1tefl
        00000000 00000000 00000000 00000000 00000000 00000000
      0000的10加。 乙，
                 ,


        0 '1工1111 11111111 ill工11i1 1111生玉 11 11111111 1工11工11王
      11111111 11111101瓷甘心心 乳22斗372,口36, 854, 775, 805t發n
        011소1111 11111111 1.主1].重1].1 11111至11 1主111111 11王1111 重，
      111王1111 11111110tv戶 9, 2.23, 37.2, 036, 854, 775, 806.,.
        011工11工1 11111工11 1生111111 11111崖1호 111111厓.1 11至1111玉
      11111111 11111111汁戶 乳223, 372, 036, 854, 775,80.7t脅朴
        10000000 00000000. 00000000 00000000 00000000 00000000
      000000們r的000000蜘戶 m乳 223口72, 的6, 854, 775, 808也壽n
        10000000 00000O00 00000000 00000000 00000000 00000000
      00000000 00000001邕Y心쏴杉9, 223下372, 036, 854, 775, 807乞毋姓
        10000000 00000000 00000000 00000000 00 00J000 00000000
      00000000 00000010，甘小牛-9, 223,372, 036, 854, 775, 806，肛卉


        11111正그1 11111111 ｝工1玉I侄工1 1工11至1工1 11111111 1111工11工
      11王11111 11111101乞珪昏出 -3蜘，n
        11111111 11111111 11111111 11111111 11111111 11111111
      11111111 11111110乞恥丹甘 m2乞熙n
        11111111 11111111 11111111 11:11重主11 1.111111]. 11111111
      11111111 11111111w心姓 -1毋羲I,



지금까지 설명한 내용을 소스 코딩하여 직접 결과로 확인해 보도록 하겠습니다．


data/type04.c 소스

／女士
           M: JaeJoon Jung <rgbi3307唾）nate.com>
                          ＼사，kerneLbz
           取／: h汰口S:/／납／＼六／




      커널연구회（蜘胛．kerneL.뇨）                                  정재준(r야13307@nate.com)
                                           73/ 351
                                                                리눅스 커널 소스 해썰 ［기초입문］
                                                                       커널 데이터 타입 이해



         F: data/type04.c
         This program is Free software; you can redistribute it and/or
         modify it under the terms of the GNU Generat Public License
火／
了치nclude <std向. h>
了치nclude <std［小.h>
#include "type02.h" ///inctude/asm-generic/int-1164.h
#include 'type03.h" ///inctude/tinux/types.h


/／加ci叱可師ux/kerr泡.h
#define USHRT_MAX ((ul 6)(싸0U))
#deFine SHRT_MAX ((Si 6)(USHRT_MAX>>1))
#define SHRT_MIN ((si 6)(-SHRT_MAX - 1))
#deFine TNT_MAX ((int)(사0U>>i))
#define 八T씨N (-INT_MAX . ])
#define UINLMAX (0U)
#define LONG_MAX ((tong)(m0UL>>i))
#define LONG1MIN (-LONG_MAX - 1)
#define U LONG_MAX (0UL)
#define LLONG_MAX ((long long)(-0ULL>>i))
#de日ne LLONG卜川N (-LLONG_MAX - ])
#define ULLONGmMAX (0ULL)
#define SIZE_MAX ( (size_t)0)
#define PHYS_ADDR_MAX ( (phys_add r_t)0)


#deFine U8_MAX ((u8)-0U)
#define 58_MAX ((s8)(U8_MAX>>1))
#de日ne S8_卜川N ((s8汁S8_MAX - ]))
#define 山旬MAX ((u16）싸oU)
#define 516_MAX ((s16)(U16_MAX>>i))
#define S16_MIN ((s16)(-S16_MAX -1))
#define U32_MAX ((u32)싸0U)
#define S32_MAX ((s32)(U32_MAX>>1))
#deFine 532_MIN ((s32)(-S32_MAX - 1))




     커널연구회（小쌔쌔／.kerne나끄）                                                 정재준（rgbi3307＠陀te.com)
                                             74/ 35 1
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                              커널 데이터 타입 이히1



#define U64_MAX ((u64)-OULL)
#define 564_MAX ((564)(U64_MAX>>1))
#define S64_卜川N 作64汁564_MAX - 1))
#define STACK MAGIC Oxdeadbeef


mnt main()
{
        printF('U8_MAX=%u\n", U8_MAX);
        prmntf("58_MAX=%d\n", 58_MAX);
        F川ntf("58小卜川N=%d\n", 58_卜川N);
        prmntf("Ui 6_MAX=%u\n", U16_MAX);
        prmntf("Si 6_MAX=%d\n", S16_MAX);
        prmntf("Si 6_MIN=%d\n", Si 6_MIN);
        printf("U32_MAX=%u\n", U32_MAX);
        printf("532_MAX=%d\n", 532_MAX);
        printf("532_MIN=%d\n", 532_MIN);
        printf("U64_MAX=%[Lu\n", U64_MAX);
        printf("564_MAX=%lLd\n", S64_MAX);
        printf("564_卜시N=%I1d\n", 564_卜川N);
        return 0;
}




위의 소스에서 " type02.h" 와 " type03.h"는 앞에서 저장한 헤더파일을 그대로 인클루드 했습니다．

실행 결과는 다음과 같습니다．



d磁立秘押蜘机쏘헝겊콰
U8 MAX=255
S8 MAX=127
58 卜시N=-128
Ui6 MAX=65535




    커널연구회（ww사．kerneLbz)                                    정재준(rgbi3307@nate.com)
                                             75/ 351
                                            리눅스 커널 소스 해설 ［기초입문］
                                                   커널 데이터 타입 이하1



S16 MAX=32767
516 MIN=-32768
U32 MAX=4294967295
532 MAX=21 47483647
S32 卜시N=-2147483648
U64 MAX=18446744073709551 615
564 MAX=9223372036854775807
S64 MIN=-9223372036854775808




실행결과를 보시면, 데이터 타입별로 최대값과 최소값이 맞게 출력됨을 확인해 볼 수 있습니다．

지금까지 데이터 타입의 표현에 대해서 기술했습니다. 특히 리눅스 커널 소스에서 데이터 타입을

어떻게 정의하고 최대값과 최소값을 어떻게 사용하는지 알아 봤습니다. 위의 소스들은 앞으로 계속

사용될 예정입니다. 또한 C 언어로 어플리케이션 작성할때도 유용하게 사용할 수 있는 공통 코드（

라이브러리）가 될 수 있으므로 잘 활용하면 많은 도움이 되겠습니다．


그리고 리눅스 커널 소스에서 데이터 타입에 관련되는 헤더파일들은 다음과 같습니다. 아래에서

"asm/types.卜I'' 헤더파일은 커널 소스를 빌드할때 CPU 종류（아키텍쳐）에 따라서 생성되는 헤더파일
         //'




입니다. 데이터 타입은 CPU 종류（아키텍쳐）에 의존하므로 이 부분을 주의하시면 소스를 이해하는데

큰 어려움 없을듯 합니다．


리눅스 커브 소스 ty口es,

include/tinux/types.h

  uapi/Linux/types.h

    asm/types.h (generated)

     asm-generic/types.h

       uapi/asm-generic/types.h



 커널연구회（M째시／.kerne나江）                            정재준（rgb13307匣）nate.com)
                                  76/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                 커널 데이터 타입 이히1



      asm-generic/irit-1L64.h




그럼, 이번 블로그는 이쯤에서 마무리하고 다음번에 다른 주제를 가지고 내용을 올리겠습니다． 다른

주제라 하더라도 지금까지 기술한 내용을 바탕으로 단계적으로 리눅스 커널 소스 코드를 이해하기

위한 방향으로 진도가 나갈 예정입니다．




 커널연구회（www.kernel.b기                           정재준（rgbi3307@nate.com)
                                77/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                             커널 비트 단위 연산




 커널 비트 단위 연산


              六Kernel BitOps
                                       리눅스 커널 소스에서 비트 단위로 데이터를 취급하는 방법들에

                                       대해서 알아 보겠습니다. 몇년전만해도 32 비트 CPU 가



          ]
                                       대부분이었는데 요즘 64 비트 CPU 가 대세를 이루고 있습니다．

                               "
                                       그만큼 처리해야 할 데이터가 많아 지고 있는듯 합니다. 제가

                                       이글을 작성하고 있는 노트북도 다음과 같이 64 비트 입니다．




 $ uname -a

 Linux HP7100U 4.15.0- 43- generic #46-Ubuntu SMP Thu Dec 6 14:45: 28 UTC
 2018 x86 64 x86 64 x86 64 GNU/Linux




리눅스는 우분투 ]8.04 버전을 설치했습니다. CPU 는 InteL(R) Core(T卜4) 13-7100U 입니다．

인텔계열의 64 비트 CPU 는 " x86 64"라고 표시가 됩니다. 그런데 어플리케이션을 하다보면 내가 64

비트에 맞게끔 코딩하고 있는지 헤갈리때가 있습니다. 특히 Long 형의 데이터는 32 비트 CPU 에서는

32 비트, 64 비트 CPU 에서는 64 비트로 크기가 잡히기 때문에 좀더 주의해야 합니다. Long 형의

데이터 크기를 확인하는 확실한 방법은 컴파일러에서 제공하는 컴파일 상수값을 확인하는 것입니다．

리눅스커널소스는：赳tsperLong.h" 헤더파일에서 다음과같이 Long형의 데이터 비트수를결정하고

있습니다．


bit印心rio咽J1
少 SPDX-License-Identifier: GPL-2.0 /
#ifndef       ASM GENERIC BITS PER LONG



 커널연구회（ww니／.kernel.뇨）                                    정재준（r야) 3307@nate.com)
                                          78/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                      커널 비트 단위 연산



#define         ASM GENERIC BITS PER LONG


前nc(ude "config.h" ///CONFIGm64BIT환경설정 상수인클루드


/1/a rcf派86加ci岫이U햐)i/asm／벼匕perlong小
斛F de日ned匕x86_64._) && !defined（小ILP32_J
# define        BITS PER LONG 64
#etse
# define        BITS PER LONG 32
#end汗


///arch/arrn64/inctude/uapi/asrn/bitsperiong.h
//#define _BITS_PER_LONG 64
I//arch/risc岫吼tude/u햐町苗耐bitspe如ng.h
//#define -미IS下ER_LONG (_듸ZE아1POINTER                  出 8)


/／力nc山由／U햐)i/asrn－恥ne朮/b心pe加ng.h
掛FndeF         B汀SP타？ LONG
#defii祀         E引TS PER LONG 32
#end汗                     1


#iFdef CONFIG 64BIT
#define BITS PER LONG 64
#else
#define BITS PER LONG 32
#endif／火 CONFIGm64텨T /


／女
* FIXME: The check currently breaks x86-64 build, so it's
升 tern的rarity（掘北沌d. 미ease 目x x86-64 and reenab佃
     出／
     i치F 0 && B汗S PER LONG ！二      미TS PER LONG
     #error Inconsistent word size. Check asm/bitsperiong.h
     #end汗




          커널연구회（附／w.kernei.b기                                     정재준（r야i3307@nate.com)
                                                79/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                              커널 비트 단위 연산



#ifndef BITS PER LONG LONG
#define BITS PER LONG LONG 64
#end汗
#end汗 ／去 回‘ASMmGENERI（二미了S_PE凡LONG *1




위의 소스에서       BITS PER LONG 상수값이 어떻게 정의 되는지 먼저 알아보겠습니다. 이 상수값은

CPU 종류에 따라서 32 훅은 64 로 정의 되기 때문에 CPU 종류（아키텍쳐）별 헤더 파일이 컴파일

시점에서 인클루드 됩니다. 저는 가장 대표적으로 3 가지（x86, AR卜4, 데SC-V) CPU 들에 대한 헤더

파일을포함시켰습니다. x86은arch/x86力nc山de/uapi/弱呵b比sperlong.h, AR卜'164는

arch/arm64/include/uapi/asmfbitsperlong.h, RISC-V 는

arch/riscv/inctude/uapi/asm/bitsperlong.h


헤더파일어나］       미TS PER LONG 상수값을 정의 합니다. x86는 mx86山64小 컴파일러 상수값이

정의 되어 있으면        미TS PER LONG 을 64로 정의 합니다. AR卜'164는 해당 아키텍쳐가 64

비트용으로 정의된 것이기 때문에 바로 64 로 정의 합니다 ．데SC-V 는 1 SIZEOF P이NTER1값에

따라서 _BITS_PER_LONG 상수값이 결정됩니다. 제가 현재 실습하고 있는 노트북은 x86 이기

때문에 AR卜'164 와 RISC-V 에 해당하는 헤더파일은 주석 처 리 했습니다．


그리고 미TS PER 山NG 상수값은 리눅스 커널 소스 환경설정 값인 C琺拜弘屯多露黎必' 정의 되어

있으면 64 이고 정의 되어 있지 않으면 32 로 결정됩니다.                미IS PER 山NG 상수값과

미TS_PER_LONG 상수값은 조건 컴파일문（＃汪 0 && B汀S中PER놔LONG!立 叫m마iS_PER_LONG）에

의해서 일치여부를 판단합니다만. 斛f0 가 앞에 있으므로 현재로서는 동작하지 않습니다 .#if ] 을

앞에 붙이면      미TS PER 山NG 상수값과 미TS PER LONG 상수값이 일치하지 않으면 컴파일

시점에서 " #error Iricon引stent word 읽ze. Check asm/b比sper[ong.h" 을 출력합니다. 그리고

미TS_PER_LONG_LONG 상수값은 당연히 64 로 정의 됩니다．




 커널연구회（www.kernel.뇨）                                      정쟤준（r야)13307@nate.com)
                                       80/ 351
                                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                                   커널 비트 단위 연산



 리눅스 커널 환경설정 값인 CONFtC小4B！丁 는 원래 리눅스 소스 make menuconfig 에서 설정 하는

 것이지만 저는 소스 테스트（실습）를 간편하게 하71 위해서 다음과 같이 con加.h 헤더 파일을 따로

만들어 인클루드 했습니다．



config/config.h 소스코드

／火火
                     M: JaeJoon Jung <rgbi3307흐）nate.com>
                                     .kerneLbz
                     W: h比口S:/／硝／니／＼六／
                     F: config/config.h
                     Th注 可四ram is 升ee so如后re; 卯u can redistribute it and/or
                     modify it under the terms of the GNU General PubLic License
士／
手치Fndef                CONFIG H
 #define               CONFIG H


  #define CONFIG 64B1T


 #end汗 ／交 m-mCONFI(그4卜j 出／/




 지금까지 설명한 내용들을 테스트하기 위해서 아라딱 같이 코드를 작성 했습니다．


      test/bits/bitspertong.c 소스코드

      ／女火
                     M: JaeJoon Jung <rgbi3307@nate.com>
                     W: https://www.kerneLbz
                     F: tes叭璇s/bits口ert帥g.c
                     This program is free software; you can redistribute it and/or
                     modify it under the terms of the GNU GeneraL PubLic License
            出／
                 커널연구회（www.kerneL.bz)                                                정재준（r야)13307@nate.com)
                                                          81/ 351
                                                          리눅스 커널 소스 해설 ［기초입문］
                                                                  커널 비트 단위 연산



了치nclude <stdio.h>
了치ncLude <S匕iLib.h>


荊nc山de <Linux/types.h>
崩ncLude <Linux/b北s.h> ///bits口erLong.h 인클루드 됨


int main()
{
         崩f defined(Hx師m鉀-J && !de目ned匕心끄-J
         printf ("_ x86_64_ defined\n");
         #etse
         printf ("_ x86_64_ NOT defined\n");
         #end汗
         printF("_ 미TS_PE艮山NG = %d L키ts\n", -尸텨巧_PER_LONG);
         printf("BITS_PER_LONG = %d bits\n", BITS_PER_LONG);
         return 0;
}



실행 결과는 다음과 같습니다．


 test/b仕＄lb北sperlonq.c 실행결과

    x86 64   defined
    미IS PER LONG = 64 1키ts
미TS PER LONG = 64 t키ts




中x8丘多4如가 컴파일러 상수값으로 정의 되어 있으므로 "                        x86_64_ defined "가 출력 되었고

1BITS1PER中LONG 는 64 로 되어 있음을 확인할 수 있습니다. 그리고 " con Fig.h" 헤더 파일에서

C(겐目i8町읕젖且했우므昊쁘주＝PER_LONG星多론壹력 되었습니다· 위에서 정의한




    커널연구회佃쌔I'사．kerne나끄）                                        정재준（rgb13307（흐）nate.com)
                                           82/ 351
                                                                  리눅스 커널 소스 해설 ｛기초입문］
                                                                          커널 비트 단위 연산



미TS PER LONG 상수값과 미TS PER LONG LONG 상수값은 리눅스 커널 소스

냐nclude/Linux/bits.h" 에서 유용하게 사용합니다．



아래는 리눅스 커널 소스 " include/Linux/bits.h" 파일의 내용을 그대로 가져온 것입니다．



incLude/tinux/bits.h

少 SPDX4文enseiden幽er: GPL包0 */
荊fndef        니NUX 태TS H
#de日ne        LINUX 미TS H
荊nc山de <as呵너匕pertong.h>


#defirie BIT(nr) (1UL<< (nr))
#defirie BIT_ULL(nr) (1ULL << (nr))
#define BITmMASK(nr) (1UL << ((nr) % BITS_PER_LONG))
#define BIT_WORD(nr) ((nr) / BITS_PER_LONG)
#define BIT_ULL_MASK(nr) (1 ULL << ((nr) % BITS_PER_LONG_LONG))
#de目ne B汗中UL나WORD(nr) ((nr) / BITSyER_LONGLO卜G)
#define BITS PER BYTE 8


／交
卉 Create a contiguous bitmask sta比ing at bit r均S池on（耿 帥d endit埠 at
出 口osit油n （흐1h. For exan耳）le
* GENMASK_ULL(39, 21) gives us the 64bit vector 0x000000ffffe00000.
 火／
     #define GENMASK(h, 1) \
            (((시0UL) -(1UL << (I)) + 1) & (시0UL>> (BITS_PERJONG - 1 - (h))))


     #define GENMASK_ULL(h, 1) \
            (((-0ULL) - (1ULL << (1)) + 1) & \
            (-0ULL>> (BITS_PER_LONG_LONG - 1 - (h))))


      #end汗 少 mLINUXmB汗SmH 六／




       커널연구회佃쌔사／,kerne比z)                                                  정재준(rgb13307（흐）nate.com)
                                                 83/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                         커널 비트 단위 연산




위의 헤더파일은 리눅스 커널에 있는 소스이지만 비트 단위로 시프트 연산 하는 것이므로 사용자

어플리케이션에서 그대로 사용할 수 있습니다. 이 헤더 파일을 인클루드하여 테스트 하는 코드를

다음과 같이 작성했습니다．


 test/bits/bit丘C 소스코드

／升出
           M: JaeJoon Jung <rgbi3307@nate.com>
           W: h吐ps://니／＼六／
                         w.kerne［勺z
           F: test/bits/bits,c
           This program is free software; you can redistribute it and/or
           modify it under the terms of the GNU Genera나ubtic License
  火／
  斛nc山de <std向.h>
崩nc山de <Linux/types.h>
 斛nc山de <Linux/bits.h>


 void b1t64_printf(u64 v)
 {
           u64 mask = BIT_ULL(BITS_PER_LONG_LONG - 1);
           whiLe(mask) {
                    printf("%d", (v&mask? 1: 0));
                    mask >>= 1;
           }
           printf("\n");
}

mnt main()
{
           u64 bits64;
           u32 i;




       커널연구회（蜘／w.kerne나）z)                                                 정쟤준（rgbi3307@nate.com)
                                                84 / 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                     커널 비트 단위 연산



         I//Left Shift << 0, 15, 30, 45, 60, 75, 90,..
         for(i=0; i<=256; i+=15) {
                  bits64 = BIT_ULL(i);
                  printf("BIT_ULL(%03d) = ", i);
                  bit64_printf(bfts64);
                  printf("BIT_ULL_WORD = %d\n", BIT_ULL_WORD(i));
         }

         b1ts64 = GENMASK_ULL(39, 21); ///high(end), (ow(start)
         printf("GENMASK_ULLO= 0x%016LX\n", bits64);
         printf("GENMASK_ULLO= ");
         b1t64_printf(b1ts64);
         return 0;
}



위의 테스트 코드에 포함되어 있는 헤더파일들은 모두 앞에서 설명한 것을 그대로 인클루드 한

것입니다．


荊nclude <tinux/types.h>
荊nctude 41nux/b比s.h>




그리고 새로운 사용자 정의 함수 void b止64_prin냔（u64v）가 추가 되었습니다. 이 함수는 u64v 값을

전달하면 이것을 이진수 64 비트로 화면에 출력 하는 역할입니다. 위의 코드에서는 BIT中ULL(),

미T_ULL_WORDO, GEN卜4ASK_ULL(）을 테스트 했습니다. 이것의 실행 결과는 다음과 같습니다．


te就加叱釘bfts工 싶행겊과

BIT_ULL(000) = 0000000000000000000000000000000000000000000000000000000000000001
    BIT ULL WORD = 0




     커널연구회佃,ww.kerne나파                                              정재준（r야)13307@nate.com)
                                                   85/ 351
                                                    리눅스 커널 소스 해낼 ［기초입문］
                                                            커널 비트 단위 연산



BIT_ULL(01 5) = 0000000000000000000000000000000000000000000000001000000000000000
BIT ULL WORD = 0
BIT_ULL(030) = 0000000000000000000000000000000001 000000000000000000000000000000
BIT ULL WORD = 0
BIT_ULL(045) = 000000000000000000i 000000000000000000000000000000000000000000000
BIT ULL WORD= 0
BIT_ULL(060) = 000i000000000000000000000000000000000000000000000000000000000000
BIT ULL WORD= 0
BIT_ULL(075) = 0000000000000000000000000000000000000000000000000000i 00000000000
BIT ULL WORD = 1
BIT_ULL(090) = 0000000000000000000000000000000000000100000000000000000000000000
BIT ULL WORD = 1
B汀_ULL(105) = 00000000000000000000001 00000000000000000000000000000000000000000
BIT ULL WORD = 1
BIT_ULL(1 20) = 0000000100000000000000000000000000000000000000000000000000000000
BIT ULL WORD = 1
BIT_ULL(1 35) = 0000000000000000000000000000000000000000000000000000000010000000
BIT ULL WORD = 2
BIT_ULL(150) = 0000000000000000000000000000000000000000010000000000000000000000
BIT ULL WORD = 2
BIT_ULL(1 65) = 0000000000000000000000000010000000000000000000000000000000000000
BIT ULL WORD = 2
BIT1ULL(180) = 000000000001 0000000000000000000000000000000000000000000000000000
BIT ULL WORD= 2
BIT_ULL(195) = 0000000000000000000000000000000000000000000000000000000000001000
BIT ULL WORD = 3
BIT_ULL(2 10) = 0000000000000000000000000000000000000000000001 000000000000000000
BIT ULL WORD = 3
BIT_ULL(225) = 000000000000000000000000000000i 000000000000000000000000000000000
BIT ULL WORD = 3
BIT_ULL(240) = 0000000000000001 000000000000000000000000000000000000000000000000
BIT ULL WORD = 3
BIT_ULL(255) = 1000000000000000000000000000000000000000000000000000000000000000
BIT ULL WORD = 3




 커널연구회（www.kernel. 虹）                                      정재준（IC羚3307回nate.com)
                                     86/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         커널 비트 단위 연산



GENMASK_ULLQ= Ox000000FFFFE00000
GENMASK_ULLQ= 000000000000000000000000i 111111111111111111000000000000000000000



소스와 실행결과를 확인해 보면 아시겠지만. 미T_ULL(nr）은 uns垣ned Long tong 의 64 비트 데이터

공간에서 nr 로 전달한 위치 만큼 ] 을 왼쪽으로 시프트 연산한 결과 입니다. 이렇게 하면 64 비트에서

nr 의 위치에 1 이 위치하게 됩니다． BIT_U나1WORD(nr)은 nr 을 단순히 미TS3ER_LONG_LONG

으로 나눈 나머지 연산한 결과입니다. 미TS_PER_LONG_LONG 은 64 이므로 64 배수 단위가 겨싼

됩니다． 이것은 WORD 단위이기도 합니다． 따라서 미T_ULL_WORD佃r)은 nr 을 WORD 단위로

환산하는 역할을 합니다. 그리고 마지막에 있는 GEN卜4ASK1ULL(h, I）의 연산결과가 상당히

흥미롭습니다.


프EN卜'lASK1ULL(h, I）는 un引gned tong long 의 64 비트 데이터 공간에서 특정 비트 범위를 ] 로

설정합니다. h는 상위 비트위치이고 1은하위 비트위치입니다. 상위비트 위치 h에서 하위비트 위치

1사이의 비트를 ] 로 설정합니다. 1 로설정되는 개수는 伽I)개가 됩니다. 위의 실행결과에서 확인할

수 있듯이，GENMASK_ULL(39, 21）을 실행하면, 상위비트 39 번째에서 하위비트 2] 번째까지 범위를

] 로 설정합니다. 이 범위의 길이는 ]8 이 되고 다음과 같이 이 사이 공간이 ] 로 설정됩니다.


GENMASK_ULL(39, 21)=

00000000ooooooooooooooooiiiiiiiiiiiiiiiiiii申oooooooooPooooooo0o

지금까지 내용은 C 언어의 비트 연산자들 중에서 보수 연산자와 시프트 연사자를 사용하는 것입니다．

C 언어 비트단위 연산자에 대해서 알고 있다면 쉽게 이해할 수 있는 내용입니다．


지금부터는 리눅스 커널 소스에 있는 비트 연산들을 좀더 알아 보도록 하겠습니다．

"inctude/tinux/bitops.h" 소스를 보면 리눅스 커널에서 사용하는 비트단위 연산들을 여러가지

인라인 함수로 작성해서 모아 두었습니다. 소스량이 상당히 많아서 몇가지 중요한 것들만 설명하도록




 커널연구회（叫iw,kerne나）z)                                     정재준（円b1330기＠nate.com)
                                   87/ 351
                                                                     리눅스 커널 소스 해설 ［기초입문］
                                                                             커널 비트 단위 연산



하겠습니다. 소스량이 많기는 하지만 몇가지만 이해하시면 나머지 것들도 모두 유사하게 동작하기

때문에 쉽게 이해할 수 있습니다．


II妃佃如川nux/b北ops.h

少 SPDX-L北ense-Identi日er: GPL-2.0 *1
 胡fndef LINUX 미TOPS H
      #define LINUX BITOPS H
  荊nc山de <asm/types.h>
  荊nc山de <linux/b此s.h>


      #define 텨TS_PE凡TYPE(type)（引zeof(type) 出 미TS_PE艮마TE)
      #define BITS_TO_LONGS(nr) DIV_ROUND_UP(nr, BITS_PER_TYPE(long))


  //／중간 생략．.


      static inLine mnt get_bitmask_order(unsigned mnt count)
      {
              II止 order;


              order = fLs(count);
              return order; /* We could be slightly more clever with -1 here...
  }

  static _always_inLine unsigned Long hweight_Iong(unsigned Long w)
  {
              return sizeof(w) == 4? hweight32(w) : hweight64(w);
}

／密火
* ro164 - rotate a 64-bit value left
* @word: value to rotate
* @shift: bits to roll




          커널연구회（的쌔／.kerne나파                                                   정재준（rgbi3307每）nate.com)
                                                   88/ 351
                                                                      리눅스 커널 소스 해설 ［기초입문］
                                                                              커널 비트 단위 연산



 *1
static inline _u64 rol64Lu64 word, unsigned mnt shift)
{
                return (word <<shift) 1 (word >> (64- shift));
}


* ror64 - rotate a 64-bit value right
火 @w아d: value to rotate
出 但）shift: b忙s to roll
士／
static inLine _u64 r0r64(1u64 word, unsigned mnt shift)
{
                 return (W0rd
                 retUrn (word >> ShiA)
                                 shift) I1 (W0rd
                                           (word << (64 - Sh吐）
                                                          shift));

}

／火交
玄 r아32- rotatea32七作 value left
* @word: vaLue to rotate
 火 @sh浪：bits to roll
  升／
 static inline _u32 rol32Lu32 word, unsigned mnt shift)
 {
                 return (W0rd
                 retUrn (word <<shift)   (W0nJ >> ((-ShiFt)
                                ShiA) I1 (word    ((-shift) & 3l));
                                                              31));
 }

  ／密出
      * ror32 - rotate a 32-bit value right
      士 侮）낚／ord: value to rotate
      士 @sh吐：bits to roU
        士／
        static inline _u32 r0r32(1u32 word, unsigned mnt shift)
        {
                 return (word >> shift) I (word << (32 - shift));




             커널연구회佃쌔／w.kerneL.b라                                          정재준（r야)i3307@nate.com)
                                                          89/ 351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                        커널 비트 단위 연산



}

//／이하 생략．.




위의 " include/Linux/b止ops.h" 에 있는 함수들은 대부분 비트 단위 연산을 합니다. 함수안의 소스

행이 많지 않기 때문에 대부분 inline 함수로 만들어져 있습니다. inline 함수는 컴파일될따1 코드가

그대로 삽입 되므로 함수 호출에 의한 속도 지연이 발생하지 않습니다 ．위의 소스에서 r0164() 함수와

ro(32() 함수 동작을 서로 비교해 보겠습니다. 소스에서 주석문을 보면 r이64() 함수는 64 비트값을

 왼쪽으로 회전(r야哉e) 시키고 r이32() 함수는 32 비트값을 왼쪽으로 회전(rotate) 시킨다는 것인데，

이것을 직접 실행해서 확인해 보겠습니다．


 test/bits/bits.c 소소코

／火火
          M: JaeJoon Jung <rgbi3307@nate.com>
          W: https://www,kerneLbz
          F: test/bits/bits.c
          This program is free software; you can redistribute it and/or
          mo（冊y 化 unde八he terms of the GNU Genera나毛blic License
 出／
崩nc山de <stdio.h>
#include <stdlib.h>
前nc山de <Iinux/types.h>
斛nclude <linux/b心.h>
#incLude clinux/bitops.h>


void bit64_printf(u64 v)
{
          u64 mask = 미T_UL나미TS_P태_LONG_LONG - 仕
          while(mask) {




      커널연구회佃쌔쌔／.kerne나파                                                   정재준（r야)i330끄＠nate.com)
                                              90/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                   커널 비트 단위 연산



                printf("%d", (v&mask? 1 : 0));
                mask >>= 1;
       }
        printf("\n");
}

void b1t32_printf(u32 v)
{
       u32 mask = 미T－시LL佃巧PE艮TYPE(v) - ]);
        while(mask) {
                printf('%d", (v&mask? 1 : 0));
                mask >>= 1;
       }
        printf("\n");
}

void test_bitops()
{
        u64 d64 = OxFQ000QOOQOQOQOQOULL;
        u64 r64;
        r64 = ro妬4(d6自 3);
        printf("1이64(ox%016LX, 3): \n", d64);
        b1t64_printf(r64);


        u32 d32 = OxOF000000U;
        u32 r32;
        r32 = r0132(d32, 7);
        printf("roL32(Ox%08X, 7): \n", d32);
        b1t32_printf(r32);
}




    커널연구회（蜘시／.kerne比z)                                         정재준（rgb13307@nate.com)
                                                 91/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         커널 비트 단위 연산



위의 소스에서 너t64_prin냔（u64v）는 V 값을 64 비트 이진수로 출력하기 위해서 제가 추가한

함수입니다. 같은 방법으로 너日2_printf(u32 v）는 V 값을 32 비트 이진수로 출력합니다．

test_t朮ops() 함수를 실행하면 다음과 같이 결과가 출력 됩니다．


    心bi白必作함수살행켤꽈

r0164(OxF000000000000000, 3):
1000000000000000000000000000000000000000000000000000000000000111
r0132(OxOF000000, 7):
10000000000000000000000000000111




I이64(OxF000000000000000, 3）을 실행하면 64 비트 값인 0xF000000000000000 을 왼쪽으로 3

번 시프트(rotate) 합니다. 이것의 결과는 64 비트 이진수로

"lOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOl 11" 2jLL)-.


ro日긱OxOF000000, 7）을 실행하면 32 비트 값인 0xOF000000 을 왼쪽으로 7 번 시프트(rot哉e)

합니다. 이것의 결과는 32 비트 이진수로 " 10000000000000000000000000000111" 입니다．


지금까지 비트 단위 연산에 대해서 분석한 내용을 기술 했습니다. 리눅스 커널에서 비트단위로

연산하는 소스가 있는 헤더 파일을 정리하면 다음과 같습니다．


리눅스커           비 탄위 연샨 소스 파읾景
include/tinux/bitops.h
include/linux/bits.h
asm/bitops.h




 커널연구회（的／w.kerne나川                                      정재준（rgb日307@nate.com)
                                   92/ 351
                                   리눅스 커널 소스 해설 ［기초입문］
                                           커널 비트 단위 연산



지금까지 설명한 내용을 바탕으로 위의 소스들을 분석해 보시면 비트 단위 연산에 대해서 많은

내용들을 이해할 수 있습니다. 데이터를 비트 단위로 처리해야 하는 곳에서 많이 활용할 수 있을듯

합니다. 그럼, 많은 도움 되길 바라며, 이번 글은 여기서 마무리하도록 하겠습니다．




 커널연구회（＼사니시／.kerne나파                    정재준（I야)i330기孕nate.com)
                         93/ 351
                                             리눅스 커널 소스 해설 ［기초입문］
                                                       커널 비트맵 이해1




커널 비트맵 이해1

                               앞에서 기술한 "리눅스 커널 데이터 타입 이해" 에 이어서

                               이번에는 "리눅스 커널 비트맵 이해 "라는 주제로 글올
           Kernel BitMap
                               작성하도록 하겠습니다. 앞에서 설명한 것을 바탕으로 내용이

           M
                           "   계속 이어지므로 순서대로 글을 읽어 주시면 좋겠습니다．


리눅스 커널 소스를 분석하다보면 항상 기본적으로 등장하는 소스 코드들이 있습니다. 당분간 이러한

소스 코드부터 설명을 이어가도록 하겠습니다. 이번에 얘기 할려는 너tmap 도 리눅스 커널 소스에서

약방의 감초처럼 많이 등장 합니다. 그래서 반드시 이해하고 가야할 7쁜 내용입니다. 벼tmap 은

한마디로 데이터를 비트 단위로 처리하기 위해서 bng 데이터 타입의 배열로 할당한 공간입니다．

데이터 타입을 Long 형으로 정의하면 32 비트 Cpu 에서는 4 바이트（32 비트）,64 비트 CPU 0似는 8

바이트（64 비트）가 할당됩니다. 우리가 보통 어플리케이션할따1, Long 형으로 데이터 변수를 하나

정의하면 Long 단위로 이 변수에 데이터를 읽고 쓰고 합니다．


아래는 C 언어로 Long 형의 변수들을 정의한 것입니다．




Long av;       ///8바이트（64비트）
Long bv[5]; ///40바이트（320 비트）



일반적인 어플리케이션에서 위와 같이 Long 형의 변수를 정의하면，av 변수는 Long 형의 데이터

단위로, by 변수는 배열 형태로 tong 형의 데이터 5 개를 취급합니다. 그런데 av 변수를 비트단위

데이터 64 개로, by 변수를 비트단위 데이터 320 개로 처리하려면 어떻게 해야 할까요？ 이것에 다빤 '

고민을 해결한 것이 리눅스 커널 소스에 구현되어 있는 bitmap 입니다．




커널연구회佃쌔째／.kernel.bz)                             정재준（rgbi3307（흐）nate.com)
                                  94/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                      커널 비트맵 이해



리눅스 커널 소스 " include/Linux/bits.h" 와 " include/(inux/bitops.h",

나nclude/uapi川nux/kerne나）" 파일을 보면 아래와 같이 정의되어 있는 매크로가 있습니다. 먼저

아래 매크로 정의부터 주석문으로 설명 하도록 하겠습니다．




///incLude/tinux/bits.h
//／모든 Cpu 0姻 1 바이트는 8 비트로 구성되어 았습니다． 아래 매크로 정의는 바이트에 대한 비트수 8 을
정의한 상수입니다．
#define BITS PER BYTE 8


///toot寸nc山de/ti叩x/b化야）s.h
//／비트수를 바이트수로 나타냅니다． 예률들어 10 비트는 (10 + 8 녀）/8 울 계산하면 2 바이트가 됩니다．
#define BITS_TO_BYTES(bits) (((b止蜘미作｝印_BYTE-1)／텨巧PERe마TE)


//／데이터 타입을 비트수로 나타냅니다． 예룔들어 char 는 읽昶0夙char少8 을 계산햐면 8 비트가 됩 니댜，
//lint 는 S注e硏（in目卉8 하면 32 가 됩니다．
#define 미TS_PE叱TYPE(type)（引zeof(type) 出 미IS 1）태_BYTE)


/／力nc山de/u햐町tnux/kerne나｝
#define _KERNEL_DIV_ROUND_UP(n, d) (((n) + (d) - 1) /(d))
#define DIV ROUND UP        KERNEL DIV ROUND UP


//／비트수 nr 율 입력받아 이 비트를 담을 수 있는 tong 데이터 타입 크기를 계산합니다．
///0菲를듈에 nr 에 300 욜 입력하면 다음과 같이 계산 됩니다．
///(n+ d- 1) /d==(300+ 64- 1) /64==S 가 됩니다．
///include/Linux/bitops.h
#define BITS_TO_LONGS(nr) DIV_ROUND_UP(nr, BITS_PER_TYPE(tong))




위의 매크로 정의에서 텨TS_TO_LONGS(nr)의 역할이 중요합니다． 위의 설명에서 nr 에 300 을

입력하면 미TS1TOU山NGS(300）은 5 가 됩니다. 이것의 의미가 무엇일까요？ 예를들어 " 300 비트를




  커널연구회佃쌔iw.kernet.b기                                            정재준（r야)i3307@nate.com)
                                          95/ 351
                                                                   리눅스 커널 소스 해설 ［기초입문］
                                                                             커널 비트맵 이해1



 담을 수 있는 데이터 타입을 C 언어로 어떻게 정의할 수 있는가7" 에 대해서 고민을 해보시면 의문은

      쉽게 풀립니다. C언어는 비트단위로 데이터 타입을 정의하는 키워드가 없습니다. char는 8 비트，

 닦i0r1는 16 비트, mnt는 32 비트, Long 은 64 비트.. 이러한 단위로 데이터 크기를 정의합니다．

      그렇다면 300 비트를 담기 위한 데이터는 어떻게 정의 할까요7 일단, 다음과 같이 배열 형태로 정의

      하면 됩니다．




      char a[38]; //304비트
      short b[19]; //304 비트
      mnt   山0]; //320비트
匕ng dES]; ///320 비트



      데이터 타입 단위의 배열이기 때문에 원하는 비트수만큼 정확하게 일치 하지는 않습니다. 위에서 300

      비트을 담고자 했지만 char와 short 배열은 뒤에 4 비트가 남고, m t 오F long 배열은 뒤에 20 비트가

      남습니다. 그렇지만 300 비트를 처리 하고자 하는 메모리 공간은 확보가 됩니다. 리눅스 커널

      소스에서는 비트를 담기위한 데이터 타입 배열로 Long 형을 사용합니다. 그래서 위의 매크로

 미TS_TO_LONGS(nr)는 nr 에 비트수를 입력하면 [ong 형의 배열 크기（인덱스 수）를 계산하는 역할을

 합니다.


지금까지 설명한 내용을 실습할 수 있는 소스 코드를 다음과 같이 작성 했습니다．


test_bitmapOl() 함수 소스코드
／斗士
            M: JaeJoon Jung <rgbi3307@nate.com>
            W: https://www.kerneL.bz
            F: test/bits/bitmap.c
            This program is Free software; you can redistribute it and/or




      커널연구회（www.kerne나）z)                                                   정재준（r야)i3307@nate.com)
                                                 96/ 351
                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                              커널 비트맵 이해1



            modify it under the terms of the GNU General Public License
士／
荊nclude <std向.h>
崩nc山de <stdlib.h>
荊nc山de <Linux/types.h>
荊nc山de <linux/bits.h>
荊nc山de <Linux/kernel.h>
荊nc山de <Linux巾北n伯p.h>


\／이d test_I沚map（거 ()
{
            s32 i;
            u64 引ze;


            printf("char = %lu bits\n", BITS_PER_TYPE(char));
            printf(" mnt = %Lu bits\n", BITS_PER_TYPE(int));
            printf("long = %Lu bits\n", BITS_PER_TYPE(Long));


           向I 乍0; i<32기 i+=32) {
                     引ze = 미TS_TO_LONGS(i);
                     printf("%3d: size=%lLu\n", i, size);
            }

            ///include/linux/types.h
            DECLARE_BITMAP(bitv, 300);
            printf(' bitv size=%Lu bits\n", sizeof(bitv) * BITS_PER_BYTE);
 }


     위의 소스에서 아래의 헤더파일들은 앞에서 이미 설명한 것이므로 그대로 인클루드하면 됩니다．


     #include <Linux/types.h>
     #include <Linux/bits.h>




      커널연구회佃I'사w.kerneLb力                                                    정재준（四씨3307匣）nate.com)
                                                     97/ 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                              커널 비트맵 이해1



荊nc山de <Linux/kerneL.h>


testi朮mapOl () 함수를실행한결과는다음과같습니다．



      늬tmapOl(｝함수샀邕崔斟

char = 8 너ts
int= 32 bits
Long = 64 bits
0: 引ze=0
32: size=1
64: 引ze=1
96: 引ze=2
] 28: 引ze=2
] 60: 引ze=3
192: 引ze=3
224: 引ze=4
256: 引ze=4
288: 引ze=5
320: 引ze=5
bitv size=320 bits




위의 실행결과는 앞에서 설명한 내용을 소스 코드로 확인해 보는 것이기 때문에 충분히 이해하실 수

있습니다. 한가지 설명하지 않은 것이 있습니다. 바로 DECLAR目BJTMAP(name上比S) 매크로

입니다. 이것은 리눅스 커널 소스 " include/Linux/types.h" 파일에 다음과 같이 정의 되어 있습니다．




        정        크로


///inctude/Linux/types.h
#define DECLARE_BITMAP(name,bits) \
unsigned long name[BITS_TO_LONGS(bits)]




 커널연구회（蜘胛．kern이.b力                                      정재준（rgbi3307@aate.com)
                                          98/ 351
                                                                  리눅스 커널 소스 해설 ［기초입문］
                                                                            커널 비트맵 이해




이 매크로의 의미는 간단합니다. unsigned tong name［크기］형태의 배열을 정의하는 것입니다．

예를들면，

DECLARE_B仟MAP（너Lv, 300) 하면 300 은 미TS_TO_LONGS(300）에 의해서 5 로 변환되고

unsigned long 바tv[5］라는 배열이 정의되는 것입니다. 결국, 지금까지의 여러가지 설명들은

un引gned tong 형의 배열을 정의하기 위한 것이었습니다． 리눅스 커널 소스는

DECLARE_BITMAP（배열명, 비트수）을 입력하면 unsigned long 배열명［크기］올 정의합니다．

여기서 크기는 long 형의 배열 크기이고 BIT旬TO_LONGS（비트수）에 의해서 계산됩니다．


위의 소스에서 嫩nclude <linux/bitmap.小 인클루드 헤더파일을 아직 설명하지 않았는데，이것에

대해서 알아보도록하겠습니다. 이것의 리눅스커널 소스 파일은 " include/linux/bitmap.h" 입니다．

이 파일에 있는 소스들은 위에서 설명한 long 형의 비트맵 배열에 대해서 작업佃peration）하는

함수들로 구성되어 있습니다. 아래는 이 파일에 있는 함수들을 주석문 형태로 설명한 부분을 7陋促

것입니다．


inc佃de/Une/bitma口h 헤더파잎 주석문

／火火
卉［兀C: bitmap overvie小／


火 丁he availab陌 b比1冶p 야｝erations and their rough meaning in the
  * case that the bitmap is a single unsigned long are thus:


      * The generated code is more efficient when abits is known at
      * compile-time and at most BITS_PER_LONG.
      出




      * bitmap_zero(dst, nbits) *dst = OUL




          커널연구회佃쌔시／.kerneL.b기                                         정재준（I야)i3307@nate.com)
                                                  99/ 351
                                                                 리눅스 커널 소스 해설 E기초입문］
                                                                           커널 비트맵 이해1



火 벼tmapmfill(dst, nb北S) 出dst = -OUL
* bitmap_copy(dst, src, nbits) *dst = *Src
* bitmap_and(dst, srcl, src2, nbits) *dst = 出srcl & *src2
* bitmap_or(dst, srcl, src2, nbits) *dst = *srcl I *SIc2
* bitmapm.xor(dst, srcl, src2, nbits) *dst = *srcl A *5rc2
싸沚map_andnot(d就srcl戶rc2, nbits) 차1st = 士srcl 弘 （卉src2)
싸沚mapJon回帥ent(dst, src, nbits) 火dst = 사（士src)
* bitmap_equal(srcl, src2, nbits) Are *srcl and *51c2 equal?
* bitmap_intersects(srcl, src2, nbits) Do *srcl and *5rc2 overlap?
* bitmap_subset(srcl, src2, nbits) Is *srcl a subset of *5rc2?
싸沚map_em야y(src, nbits) Are a［나）its zero in 卉src?
* bitmap_full(src, nbits) Are all bits set in *src?
* bitmap_weight(src, nbits) Hamming Weight: number set bits
* bitmap_set(dst, pos, nbits) Set specified bit area
* bitmap_clear(dst, pos, nbits) Clear specified bit area
女 蹴m叩findm昶炊HzeroJrea(buf, len, pos, n, mask) 디nd 너t free area
士 瞰m叩findm昶炊Hzero area아艮buf, len, pO5, n, mask) as above
* bitmap_shift_right(dst, src, a, nbits) *dst = *src>> n
싸玭map_sh汗t l可t(dst, src, a, nbits) 勺ist= 出src << a
* bitmap_remap(dst, src, old, new, nbits) *dst = map(old, new)(src)
* bitmap_bitremap(oldbit, old, new, abits) newbit = map(old, new)(oldbit)
싸沚map！毗O他乳 O如，relmap, nbits) 士dst = orig relative to relmap
싸戶tm叩f이d(d攷＋rig, sz, nL玭s) dstb心 = 아ig bits mod sz
* bitmap_parse(buf, buflen, dst, nbits) Parse bitmap dst from kernel buf
사此nap_pars已小er(ubuf, ulen, dst, nb北s) Parse 너tmap dst 行에use사,uf
* bitmap_parselist(buf, dst, nbits) Parse bitmap dst from kernel buf
* bitmap_parselist_user(buf, dst, abits) Parse bitmap dst from user buF
* bitmap_find_free_region(bitmap, bits, order) Find and allocate bit region
* bitmap_release_region(bitmap, pos, order) Free specified bit region
샤沚map叫訃幻cate_re이on何帥ap, pos, order) Allocate speci日ed bit reg幻n
* bitmap_from_arr32(dst, buf, nbits) Copy nbits from u32[] buf to dst
싸沚map_t(七arr32(buf, src, 耐ts) Copy a比S 什om b沚 to u32[} dst
火


央 Note, b北map_zero() and 奴tn始p_fitl() 叩erate over 냔唯 reg泊a 硏




    커널연구회佃쌔째／.kerae比z)                                                  정재준（rgbi330기孕nate.coa兮
                                               100/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                           커널 비트맵 이해1



出 unsigned 幻ngs, that is, b比s behind bitma口 t洑 the unsigned 幻ng
* boundary will be zeroed or filled as well. Consider to use
* bitmap ctear() or bitmap--set() to make explicit zeroing or filling
卉 respec匕ye奴
央／
함수들의 종류가상당히 많습니다. 이들중에서 대표적인 것들을 예를들어 설명해 보겠습니다. 먼저

너tm햐乙zero()와b化map_f叫）함수에 대해서 알아보겠습니다． "incLude/Linux/bitmap.h" 파일에

있는 이 함수의 소스는 다음과 같습니다. 이 함수에 전달되는 Un引gned tong 차:1st 는 비트맵 배열의

시작주소（포인터）입니다. un引gned m l nbits 는 비트맵 배열안의 비트개수 입니다．


         p느工ero(）와bitmap_

static inline void bitmap_zero(unsigned long *dst, unsigned mnt nbits)
{
          unsigned mnt ten = BITS_TO_LONGS(nbits) * sizeof(unsigned long);
          memset(dst, 0, len);
}

static inline void bitmap_fill(unsigned long *dst, unsigned mnt nbits)
 {
          unsigned mnt len = 미TS_TO_LONGS(n너ts난 引zeof(un如ned匕ng);
          memset(dst, 0xff, len);
 }


     bitmap_zero（서st, nb比S) 함수는 dst 에 비트맵 배열의 포인터를 전달하고 nb北S 에는 비트개수를

     전달하면 memset(）을 통하여 비트맵안의 비트들을 모두 0 으로 세팅합니다． 너tmap_f ill伊dst,

     nbits) 함수는 비트맵의 nb止S 만큼의 공간을 Oxff로 세팅합니다. 그런데 비트맵 공간은 unsigned




      커널연구회佃쌔／w.kerne나）z)                                                정재준（rgbi3307@nate.com)
                                              101 /351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                          커널 비트맵 이해1



                                           7떽 바이트수로 계산하는 과정이
long 형태의 배열이기 때문에 memset(）을 실행할때I Len 을 배열크:

필요합니다．


unsigned mnl len = BITS_TO_LONGS(nbits) * sizeof(unsigned long);


위의 Len 크기는 memset(）을 실행하기 위한 바이트수가 됩니다. 이러한 과정을 확인하기 위한

테스트 코드를 다음과 같이 작성했습니다．



  test_bitmapO그C) 함수 소스 코드

／士卉
          M: JaeJoon Jung <rgbi3307@nate.com>
          W: https://www.kernet.bz
          F: test/bits/bitmap.c
          This program is Free software; you can redistribute it and/or
          modify it under the terms of the GNU General Public License
 火／
荊nc山de <std向.h>
荊nc山de <std(ib.h>
荊nc山de <linux/types.h>
荊nc山de <linux/bits.h>
荊nc山de <linux/kernel.h>
#include <linux/bitmap.h>


void bits_printf(unsigned long* v, u32 nbits)
{
          s32 i;
          u32 wc = BIT_WORD(nbits); ///inctude/linux/bits.h
          u64 maski, mask2 = BIT(BITS_PER_TYPE(long) - 1);I//BITS_PER_LONG
          向r 仁吼；i>=0; i-) {
                   printf("v[%d]=", i);
                   maski = mask2;
                   while(maskl) {




      커널연구회佃쌔쌔／.kerne比z)                                                  정재준（rgbi3307@nate.com)
                                             102/ 351
                                                               리눅스 커널 소스 해설 ［기초입문］
                                                                         커널 비트맵 이해



                          printf("%d", (v[i]&maskl ? 1: 0));
                          maski >>= 1;
                 }
                 printf("\n");
        }
        printf("\n ');
}

void test_bitmap02(u32 nbits)
{
        u32 v = BITS_TO_LONGS(nbits);
        u32 Len = BITS_TO_LONGS(nbits) * sizeof(unsigned long);
        printf("nbits=%u, array=%u, bytes=%u, bits=%u\n\n '
                 , nbits, v, Len, ten出BI巧PE艮BYTE);


        DECLARE_BITMAP(bitv, nbits);
        bits_printf(bitv, nbits);


        bitmap_zero(bitv, nbits); ///memset(dst, 0, len)
        bits_printf(bitv, nbits);


         bitmap_filL(bitv, nbits); ///memset(dst, 0xff, Len)
         bits_printf(bitv, nbits);
}


위의 소스를 보면 내가 작성한 사용자정의 함수 bits_printf(）와 test_i朮map02() 함수가 있습니다．

bits_printf(unsigned long火 \i, u32 nbits）는 V 에 비트맵 배열의 시작주소（포인터）와 nb止S 에는

비트개수를 전달하면 비트맵안의 비트를 nb止s 'H수만큼 화면에 출력합니다．


    test_i沚map02(u32 nb止S) 함수의 nb北S 에는 비트개수를 전달합니다. nb化S 에 200 을 전달했을따1

실행결과는 다음과 같습니다．




     커널연구회（M쌔시／.kerne나끄）                                           정재준（rgbi3307@nate.con力
                                               103/ 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                              커널 비트맵 이해1



test_bitmap02(200) 실행결과

nbits=200, array=4, bytes=32, bits=256


          ,,, BIT于＼4AP() 실행결과
///DECLARE』
v[3]=0000000000000000000000000000000000000000000000000000000000000000
v[2]=0000000000000000000000000000000011111111111111111111111111111111
v[1]=0000000000000000000000000000000000000000000000000000000000000000
v[O]=0000000000000000000000000000000000000000000000000000000000000000
          zero() 실행켤콰
I//b滋nap．』』，
v[3]=0000000000000000000000000000000000000000000000000000000000000000
v[2]=0000000000000000000000000000000000000000000000000000000000000000
v[1]=0000000000000000000000000000000000000000000000000000000000000000
v[O]=0000000000000000000000000000000000000000000000000000000000000000
I/ /b打nap呻Fitt() 실행결과
v[3]=1111111111111111111111111111111111111111111111111111111111111111
v[2]=1111111111111111111111111111111111111111111111111111111111111111
v[1]=1111111111111111111111111111111111111111111111111111111111111111
v[O] =1111111111111111111111111111111111111111111111111111111111111111




위의 실행결과와 test1너tn伯p02() 함수의 소스를 같이 확인해 보겠습니다．

DECLARE_BITMAP（너tv, nbits) 매크로는 컴파일 시점에 unsigned long

벼tv［태TS_TO_LONGS（너匕）
                   ］으로 되고 미TS_TO_LONGS(200）은 4 가 됩니다． 따라서 unsigned

long 니tv[4］가 되고 unsigned long 형의 배열（요쇼개수는 4）이 내부변수로 정의됩니다. 내부변수

（배열）이기 때문에 그 안에 들어 있는 비트값들은 임의의 쓰레기값입니다． 다음으로

bitniap_zer이bitv, ni키ts）가 실행되면, t키tv 을 nbi匕개수만큼 0으로 설정합니다. 그런다음

b比map_태l(bitv, nb比引을 실행하면 nb比s711수만큼 ] 로 채움니다．


지금까지 b比map_zero() 함수와 bitmap_fill() 함수에 대해서 알아 봤습니다. 이 함수 외에도 리눅스

커널 소스 파일 " include/linux/bitmap.h" 을 보시면 다양한 비트맵 작업 함수들이 있습니다. 또한



 커널연구회（ww낚／.kerne나玹）                                     정재준（rgbi3307回nate.com)
                                         104/ 351
                                       리눅스 커널 소스 해설 [71초입문］          尸口卞

                                                   커널 비트맵이해          L：쓰
"Iib/test_bitmap.c" 소스 파일을 보시면 비트맵 함수들을 테스트하는 소스를 커널 모듈로 만든 것이

있습니다. 저는 그동안 리눅스 커널 소스를 테스트하기 위해서 소스를 하나씩 분리해 내서 일반

어플리케이션으로 일부 소스 만을 따로 테스트 했습니다. 하지만 이 방식은 리눅스 소스를

테스트하는데 한계가 있습니다. 일부 소스만 따로 테스트하는 것인데, 이마저도 소스를 분리하는

작업이 상당히 번거럽고 힘듭니다. 그런데 리눅스 커널은 소스를 모듈로 작성하여 커널 안으로 삽입

(insmod）하는 방식으로 소스들을 테스트할 수 있는 방법이 있습니다. 리눅스 커널 디바이스

드라이버도 모듈 형태로 많이 작성합니다. 앞으로는 모듈로 작성하여 리눅스 커널 소스를 테스트

하도록 하겠습니다. 이것에 대해서는 다음 글에서 다루도록 하겠습니다．




 커널연구회佃쌔시／.kerne나玘）                         정재준（r야)13307@nate.com)
                           105/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］

：그                                                                 커널 모듈 프로그래삥




     커널 모듈 프로그래밍

                                    이번글 주제는 리눅스 커널 모듈 프로그래밍（기초）입니다．

             A,              ,
                                    리눅스 커널 소스를 분석하다보면 코드가 어떻게 실행 되는지
             Kernel Module


            N万「
                                    검증하고 싶을때가 있습니다. 그런데 리눅스 커널 코드는 일반

                                    어플리케이션으로 실행되지 않고 커널 내부에서 동작 시켜야

                                    합니다. 리눅스 커널 소스를 커널 내부에서 동작 시키기 위해서

     커널 소스를 모두 다시 빌드하고 설치하고 재부팅해서 결과확인... 이러한 작업은 매우 번거롭습니다．

     다행히 리눅스 커널은 모듈을 제공합니다. 리눅스 커널 소스를 모듈로 프로그래밍하면 커널 소스를

     모두 다시 빌드하지 않고, 수정한 모듈만 컴파일하여 이것을 커널에 따로 삽입하여 실행 및 결과를

     확인할 수 있습니다. 이렇게 하면 커널 소스를 테스트 하기에도 편리합니다. 리눅스 커널 디바이스

     드라이버 프로그래밍도 이 방식으로 많이 작성합니다．


     이번글은 리눅스 커널 모듈 소스를 간단히 만들어서 빌드 후 커널에 삽입하고 결과를 확인하는 방법에

     대해서 기술합니다. 기초적인 부분입니다. 리눅스 커널 모듈 프로그래밍 기초에 대해서 이미 알고

     계시다면 이번글은 건너 뛰어도 되겠습니다．


     먼저 개발환경에 대해서 몇가지 점검이 필요합니다. 현재 저는 다음과 같은 노트북（PC) 환경어써

     작업하고 있습니다．




       1   CPU: Inte1(R) Core(TM) i3-7100U CPU （흐）2.40GHz
      1    RAM: 8GB
      1    OS: Linux ubuntu 18.04
      1    Kernel: v4.20



     커널연구회佃쌔쌔庶erne나끄）                                           정쟤준（四bi3307@nate.com)
                                         106/ 351
                                                         리눅스 커널 소스 해설 ［기초입문］
                                                                커널 모듈 프로그래밍



   U      gcc: version 7.3.0
   1      Target: x86_64-linux-gnu




리눅스 우분투 ] 8.04 버전을 설치했고 커널은 이글을 작성하고 있는 시점에서 최선 버전인 v4.20

입니다． gcc도 비교적 최신 버전인 GCC 7.3 released [2018-01-25] 입니다. 위의 내용들은 다음과

같이 리눅스 명령어로 확인 가능합니다．




$ uname日
Linux HP7100U 4.20.0+ #1 SMP Sat Jan 19 10:58:37 KST 2019 x86_64 x86_64 x86m64 GNU/Linux


$ uname 寸
4.20.0+


$gcc-v
COLLECT_GCC=gcc
COLLECT LTO WRAPPER=/usr/的徊cc/x86_64小nux-gnu/7爪어wrapper
OFFLOAD_TARGETHNAMES=nvptx-none
OFFLOAD TARGET DEFAULT=1
Target: x86_64-[inux-gnu
gcc version 7.3.0 (Ubuntu 7.3.0-27ubuntu1기8.04)




그리고 가장 중요한 리눅스 커널 소스는 "川b/moduLes!" 에서 커널 버전별로 확인할 수 있습니다．

저의 노트북어七 다음과 같이 커널 버전들이 설치되어 있습니다．




  커널연구회佃쌔八사.kerne나妃）                                             정재준（r야)i330기＠nate.com)
                                         107/ 351
                                                            리눅스 커널 소스 해설 ［기초입문]
                                                                   커널 모듈 프로그래삥



리뇩스 커뇌 소스 위치 확인

jungjaejoon@HP7100U:/Lib/modules$ LI
 /／다읗과 같이 화면에 표시 됩니다．
drwxr-xr-x 13 root root 4096 1 월 19 12:58 .1
drwxr-xr-x 22 root root 40965월 172018..!
drwxr-xr-x 2 root root 4096 6 월 13 2018 4.15.0-20-generic!
drwxr-xr-x 2 root root 4096 7 월 3 2018       4.15.0-22-generic!
drwxr-xr-x 2 root root 4096 12 월 24 10:09 4.15.0-39-generic!
drwxr-xr-x S root root 4096 12 월 5 07:41 4.15.0-42-generic!
drwxr-xr-x 6 root root 4096 1 월 19 10:03 4.15.0-43-generic!
drwxr-xr-x 3 root root 4096 1 월 19 13:02 4.20.0+!




위에서 리눅스 커널 4.15 버전은 노트북에 우분투 ]8.04 를 처음에 설치 할때의 버전이고, 이경로

(4.15.0-42-generic) 안에 내용을 보면 처음에 우분투를 설치할때떽 커널 소스는 "!usr/src/Linux-

headers-4.15.0-42/" 경로에 있습니다 ．그리고 4.20.0+ 경로에 있는 버전 4.20 은 그 이후로 내가

새롭게 설치한 최신 커널 버전입니다. 내가 설치한 최신 리눅스 커널 소스는 다음과 같은 위치에

있습니다.


섀各개 섬치한 최신 리눅스 커넙 소스 위치蟹

$ U /Lib/modules/4.20.0+/
 /／다읗과 같이 화면에 표시 됩니다．
drwxr-xr-x 3 root root 4096 1 월 19 13:02.!
drw町水r-x 仔 root root 4096 ] 월 ]9 ] 2:58 ../
Lrwxrwxrwx 1 root root 58 1 월 19 12:58 build ->
／加me/jungjae如帥／Projects/kern이小때d/bu妃v4.20.／師_64!
drwxr-xr-x 13 root root 4096 1 월 19 13:02 kernel!
lrwxrwxrwx 1 root root 54 1 월 19 12:58 source->
/home加ngjae如on/Pr이e仗s/kerne以'flu片町(in炚咬的佃／




 커널연구회佃蜘／.kerne比z)                                                정재준(rgb日307@nate.com)
                                         108/ 351
                                                                        리눅스 커널 소스 해설 ［기초입문］
                                                                               커널 모듈 프로그래밍




리눅스 커널 소스는 최신 버전으로 새롭게 설치해 주는 것이 좋습니다. 커널 소스 빌드 및 설치 방법에

대해서는 앞에서 설명한 "커널 소스 빌드 및 버전관리 "을 참고해 주시기 바랍니다．


리눅스 커널 소스를 모듈로 프로그래밍 할때는 위에서 언급한 "川b/modules／최신버전／build" 와

"川b/modules／최신버전／source" 에 있는 커널을 참조합니다. 최신버전은 리눅스 명령에 " $(shell

uname -r) " 로확인합니다．


이제 리눅스 커널 모듈 프로그래밍 본론에 돌에 갑니다. 커널 모듈 소스（h이b .c）를 아래와 같이

간단히 작성 하겠습니다．


heLl往心

／火出
              M: JaeJoon Jung <rgbi3307孕nate.com>
              ＼사： h汰口＄://＼사＼八／w.kerneL.bz
              F: tinux.modutes/testfhetLo.c
              This program is free software; you can redistribute it and/or
              modify it under the terms of the GNU General Public License
  火／
 荊nc山de <Linux加叱h>
      #inc山de <linux/module.h>
      荊nc山de <linux/kernel.h>


      static mnt_mn比 hello_init(void) {
               printk("Linux-modules: test/hello.c: hello_initO.\n");
               return 0;
       }

       static void _exit heUo_exit(void) {




           커널연구회佃쌔I'사．kerne나파                                                 정재준（rgb1330기＠nate.com)
                                                    109 / 351
                                                                  리눅스 커널 소스 해설 ［가초입문］
                                                                         커널 모듈 프로그쾌삥



         printk("Linux-modules: test/hello.c: heHo_exi tQ.\n");
}

moduLe_init(hello_init);
module_exit(hello_exit);


MODULE_LICENSE("GPL");
MODULE_AUTHOR("JaeJoon Jung");
MODULE小DESC데아山N("A Hello, World Kerne나1odule");
MODULE_VERSION("0.l.0");



위의 heUo.c 소스는 module_in奴）함수와 module_ex咀）함수를 간단히 테스트 하는 것입니다．

module_in化0는커널 내부API 함수입니다. 이 함수에 " h이lo in比" 함수 명칭을 전달하면. 모듈이

커널 내부에 삽입되어 실행되는 시점에서 hello_in띠）함수가 실행 됩니다. module_ex呵）함수는

모듈이 커널에서 제거될때 실행됩니다. 이 함수에 " hello ex比" 함수 명칭을 전달하면, 모듈이

커널에서 제거되는시점에서 h이呵ex띠）함수가실행됩니다. 이 과정을확인하기 위해서, 위의

소스를 빌드하기 위한卜4akefi1e 을 다음과 같이 작성합니다.



卜4akefi노

야小m += he(lo.o


hello:
         make -c
              =C /lib/modules/$(sheLl uname -r)/build M=$(PWD) modules
clean:
         make -C/lib/modules/$(shell uname -r)/build M=$(PWD) clean




    커널연구회佃쌔시二kerneLbz)                                                정재준（rgb13307@ nate.con兮
                                             110/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                  커널 모듈 프로그래밍



卜4akef lie 파일에서 make 앞에는 탭문자가 있어야 합니다. 위의 파일을 그대로 Ctrl+C 하시면 HT卜사．

문자가 들어갈 수 있으므로 반드시 아스키 문자 코드로 탭문자가 삽입되어 있는지 주의 바랍니다．

위에서 "川b/modules/$(shell uname 寸)/buitd"는 리눅스 커널 소스가 빌드되어 있는 경로를

지정합니다. "M=$(PWD)"는현재 빌드하고자하는모듈소스（h이［o.c）의 경로위치를지정합니다．


다음과 같이 " make heLLo" 명령을 입력하여 hetio.c 모듈 소스를 빌드 합니다．


裂堪모疑割드하카

$ make heLlo


/／다음과 같이 빌드 메세지가 화면에 출력 됩니댜．


make -c /Lib/moduies/4.20.0+/buiid M=/home/jungjaejoon/Projects/kernel/Linux-moduLes/test
modules
make[1]: Entering directory '/home/jungjaejoon/Projects/kerneL/buiid/bui(d_v4.20_x86_64'
CC [M] /home/jungjaejoon/Projects/kernel/Linux-modules/test/he(Lo.o
Building modules, stage 2.
MODPOST 1 modules
CC /home/jungjaejoon/Projects/kernel/Linux-moduLes/test/heLLo.mod.o
LD [MI /home/jungjaejoon/Projects/kernel/Linux-modules/test/heUo.ko
make[1]: Leaving directory '/home/jungjaejoon/Projects/kernet/build/buiLd_v4.20_x86_64'




위와 같이 컴파일 및 링크 과정을 거쳐서 " heilo.ko" 모듈이 생성됩니다. 다음과 같이 modir寸0

명령을 사용하여 이 파일의 정보를 확인합니다．




  커널연구회（낚쌔,w.kerneLb기                                                 정재준（rgbi3307@nate.com)
                                          111/ 351
                                                           리눅스 커널 소스 해설 ［기초입문]
                                                                  커널 모듈 프로그래밍



$ modinfo heRo.ko


/／다음과 같이 모듈 정보 화면에 출력 됩니다，


filename: /home/jungjaejoon/Projects/kernel/li nux-modules/test/heUo.ko
version: 0.1.0
description: A Hello, World Kernel Module
author: JaeJoon Jung
license: GPL
srcversion: F5FES2E12F4670C1 B51 FESD
depends:
name: hello
vermagic: 4.20.0+ SMP mod_unload




hetlo.c 모듈 소스에서 다음과 같이 코딩한 정보가 나타납니다．



MODULE_LICENSE("GPL");
MODULEmAUTHOR("JaeJoon Jung");
MODULE_DESCRIPTION("A Hello, World Kernel ModuLe");
MODULE_VERSION("0.l. 0");


위에서 빌드한 helLo.ko 모듈을 커널에 삽입하여 실행하도록 하겠습니다 ．리눅스 명령어 ''insmod " 을

다음과 같이 실행하면 heLto.ko 모듈이 커널 내부에 삽입되어 실행됩니다. 이 명령어는 앞에 su（如 을

추가하여 root 권한으로 실행해야 합니다．



커널 모듈 삽입하여 실행하기

$ sudo insmod he[Lo.ko




커널연구회（附,w.kerne나）z)                                                정재준（rgb13307（孕riate.com)
                                            112/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                   커널 모듈 프로그리俚1



실행 되었습니다. 혹시 아무런 실행 메세지가 없다고 당황하지 마세요. 리눅스 커널 모듈은 printk로

출력하는 메세지를 " /var/Log/syslog"파일에 출력합니다. 다음과 같이 리눅스 명령에 " tail"을

실행하여 " /vaiflog/syslog " 파일의 맨 마지막 행을 확인합니다．


      모長 싶헹 메세지 화인

$ tail /var/log/syslog


/／다음과 같이 화면에 표시 됩 니다．
Jan 2111:20:59 HP7100U kerneL: [14946.914399] Linux.modutes: test/heUo.c: helLo initO.



출력된 메세지는 " Linux-modules: test/hello.c: hello_initO." 입니다. 이 메세지는위의 소스

helLo.c에 있는 hello_in띠）함수에서 출력한 메세지 입니다. 즉, 모듈이 커널에 module_init(）에

의해서 초7뻐 실행될따1hello_in奴）함수에서 이 메세지가 출력 됩니다．


static mnt_帥t hello_init(void) {
        prmntk("linux-moduLes: test/hello.c: hello_initO.\n");
        return 0;
}
module_init(hetlo_init);


위에서 실행한 " sudo insmod hetlo.ko" 명령에 의해서 hello.ko 모듈이 커널에 삽입되어 있습니다．

삽입된 정보는 다음과 같이 리눅스 명령에 "匕mod" 로 확인 가능 합니다．


        어 있늉 모好리스트

$ Ismod


//／다음과 같이 화면에 출력됩니다，




    커널연구회6사니／낚／.kerneL.뇨）                                            정재준（r야)13307@nate.com)
                                          113/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                               커널 모듈 프로그래삥




Module           Size    Used by



                           0462
hello           16384
rfcomm          77824
ccm             20480
bnep            24576
//／이하 생략,..



삽입되어 있는 hello.如 모듈을 이번에는 제거 하도록 하겠습니다. 리눅스 명령에 " rmmod" 을

다음과 같이 실행하면 heRo.ko 모듈이 커널 내부에서 제거됩니다. 이 명령어는 앞에 sudo 을

추가하여 root 권한으로 실행해야 합니 다．


모妊 川거 명렇 심횅

$ sudo rmmod hello




제거 되었습니다. 리눅스 커널 모듈이 제거 될때도 printk로 출력하는 메세지를 "/var/log/syslog'

파일에 출력합니다. 다음과같이 리눅스 명령에 " tail"을 실행하여 " /var/log/systog "파일의 맨

마지막 행을 확인합니다．


커넘 모長 川거 메세차 확인

$ tail /var/log/syslog
/／다음과 같이 화면에 표시 됩니다．
Jan 2111:45:06 HP7100U kernel: [16393.681430] Linux-modules: test/he[lo,c: heLLomexitO.



출력된 메세지는 " Linux-modules: test/hello.c: heLlo_exitO." 입니다. 이 메세지는위의 소스

hello.c 에 있는 hello_exit() 함수에서 출력한 메세지 입니다． 즉, 커널 모듈이 module_ex比0에

의해서 제거될때, 여기에 등록되어 있는 hello_ex奴）함수에서 이 메세지가 출력 됩니다．




 커널연구회佃쌔쌔／.kerne냐比）                                              정재준（rgbi3307@nate.com)
                                       114/ 351
                                                           리눅스 커널 소스 해설 ［기姦입문］
                                                                  커널 모듈 프로그래밍



static void _exit heRo_exit(void) {
        printk("linux-modules: test/he(lo.c: hello_exitO.\n");
}
moduLe_exit(helLo_exit);




위에서 기술한 내용들을 정리해 보겠습니다. 리눅스 커널 모듈은 "川b/modules/$(shell uname 미／

build" 경로에 있는 정보들을 참조하여 소스를 빌드 합니다. 빌드된 모듈은 modinfo 리눅스

명령어로 정보를 확인할 수 있습니다. 빌드된 모듈（火.ko）을 커널에 삽입할때는 insmod 명령어로

삽입하고. 이때 모듈 소스의 module_in化（）에 등록된 함수가 실행 됩니다. 모듈을 제거할때는

rmmod 명령어를 사용합니다. 모듈이 커널에서 제거 될때는 module_ex比（）에 등록된 함수가 실행

됩니다. 모듈 코드안에서 printk로 출력되는 메세지는 " /var/log/syslog " 파일에 저장되고 이곳에서

실행 결과를 확인할 수 있습니다．


지금까지 설명한 내용들은 커널 모듈을 하나 빌드해서 삽입 및 삭제하는 기본 과정에 대해서 기술한

것입니다. 기초적인 내용이긴 하지만 여기서 언급한 내용을 바탕으로 앞으로 내용들을 추가하면서

커널 소스를 계속해서 익혀 가도록 하겠습니다．




    커널연구회（小쌔쌔／.kerneLb기                                          정재준（rgbi3307@nate.com)
                                          115/ 351
                                                         리눅스 커널 소스 해설 ［기초입문］
                                                                 커널 sort 테스트




커널 sort 테스트

                                          이번글은 앞에서 기술한 "리눅스 커널 모듈 프로그라뗑（기초）"을

                                          좀더 연습하기 위해서 준비 했습니다. 내용은 리눅스 커널 소스에
             kernel sort test
                                          있는 sort 함수를 테스트 하는 것입니다. 이번글부터 기술하는

                                          내용들은 커널 모듈 프로그래밍에 대한 사전 지식이 있어야
                M                  "




                                          합니다. 혹시 "커널 모듈 프로그래밍" 내용을 읽어 보지 못했다면

      다시 복습 부탁합니다．


      리눅스 커널 소스 'tib/sort.c" 파일을 보면 아래와 같이 sort 함수가 정의 되어 있습니다． 이 함수가

      선언되어 있는헤더 파일은也兜廻映好恥坦니다·

      lib／느ort.c 안에 있는 $O戊 함수

      V이d sort(voic卄base, 血e_t num, size_t 引ze,
      mnt 伊cmp)(const v이d 火，const void 外．
      \／이d 伊5니／ap)(void 出，V이d 出. int));




 이 함수로 전달하는 파라미터들은 다음과 같이 주석문으로 설명되어 있는더1, 제가 한글로 좀더 설명올

추가 했습니다．


sort 함수주석문（파라미터，의미）
／火出
火sort - sort an array of elements /／배열안에 있는데이터들을정렬
火 @base: p이nter to data to sort /／정렬 하고자 하는 데이터 저장소（배열）의 시작 주소（포인터）
卉＠)num: number of elements /／데이터 걔수
士＠引昶巧注e of each element /／데이터 저장소0州열）의 크기




      커널연구회佃쌔쌔／.kerneL.뇨）                                    정재준（rgb13307@nate.con分
                                              116/ 351
                                                        리눅스 커널 소스 해설 [71초입문］
                                                                커널 sort 테스트


火 ＠乂mp_func: p이nter to comparison funct向n /／비교하는 함수 포인터
士 @)swap_func: p이nter to swap func匕on or NULL /／데이터 교환하는 함수 포인터 훅은 NULL
士／
그리고 연이어 있는 주석문을 확인해 보면, 이 함수는 heapsort 방식으로 동작하고 정렬 시간은 O(n

Log n) 입니다. 더구나, 평균적인 경우나 최악의 경우 모두 이 시간에 수행되는 알고리즘으로 평가

되고 있습니다. 알고리즘을 평가할때1 " 평균적인 경우나 최악의 경우 모두" 구문이 중요합니다. 이

구문에서 모두 O(n log n）으로 평가되면 상당히 좋은 알고리즘 입니다. 참고로, 소팅 알고리즘 중에서

qsort는 heapsort 방식에 비해서 약 20％정도 더 빠르다고 평가되고 있습니다. 하지만. qsort는

추가적인 메모리가 필요하고 최악의 경우 O(n火n) 시간이 걸리기 때문에 리눅스 커널에서는 데이터를

정렬할때I qsort 가 아닌 heapsort 알고리즘을 채택하고 있습니다．


리눅스 커널 소스에 구현되어 있는 heapsort 알고리즘은 " Lib/sort.c"에 있는 sort 함수를 분석하면

되겠습니다. 우선. 이 함수를 커널 모듈 프로그래밍을 통하여 테스트 해보도록 하겠습니다. 사실. 이

함수를 커널 모듈 프로그램으로 테스트하는 소스도 다음과 같이 리눅스 커널 소스 " lib/testmsort.c" 에

있습니다. 저는 이 소스를 이해하71 쉽게 풀어서 설명하도록 하겠습니다. 먼저, 주석으로 설명을 추가

했습니다．


               比心撫心t蛋oft鈿毗（) 함수

 static m t _init test_sort_init(void)
 {
         int*a,i,r=1, err=.ENOMEM;          q너g＼如뇨             ' . . ,-         . -.
         a= k付｝atLoc_array(TES丁_LEN, szeof（火a), GFP叫KERNEL); /／정수 톄이터뷸 TESTJ上N 개수만금
         커널에 메모리 할당
         if (ia) return err;
         for (I = 0; i <TEST_LEN; i+-4-) {
                  r = (r士725861) % 6599; /／냔수 발생




     커널연구회（ww니／.kerneLb기                                     정재준（r야)13307@nate.com)
                                             117/ 351
                                                            리눅스 커널 소스 해설 [기초입문］
                                                                    커널 sort 태스트



                    a띠 = r; /／배열 a 에 난수 데이터 대입
         }
         sort（하TES了_LEN, s江eof(*a),口npit北'I刈LL); I/ sort함수실횅（이 함수안0弘Ia배열얀의
         뎨이터가 정렬됨｝
         err = -EINVAL;
         for (I = 0; i <TEST_LEN-i; i4-+) 月정렬된 데이터를 검증하기 위해서 배열 데이터 개수만큼 반복
                    if (a[i] > a[i+i] ) { /／정렬되었는지 앞뒤 데이터 크기 비교
                          p乙err("test has failed\n"); /／앞에 있는 데이터가 크면 정렬되지 않았윰（실패）
                    goto ex七
         }
         err = 0;
         pr_info("test passed\n"); /／위의 凡I 루프에서 앞뒤 데이터 크7酬 이상이 없으면 정렬 성공
         ex七
         kfree(a); /／커널에 메모리 할당한 배열 a 룔 해제
         return err;
}


"Iib/test_sort.c"에 있는 te攷sort m i目）함수는 커널 모듈이 삽입(insmod）될따1

module_init(test_s아1_init);에 의해서 실행됩니다. 아주 간결하게 코딩되어 있기 때문에 이해하기

쉽습니다． "(ib/test_sort.c "는 다음과 같이卜4akefile 을 만들어 모듈을 빌드하면 됩니다．



Makefile

야乎m := test_sort.o


test sort:
         make -c /lib/mociules/$(sheLl uname -r)/bui(d M=$(PWD) modules


clean:
         make -c /lib/modules/$(sheU uname -r)/buiLd M=$(PWD) clean




    커널연구회（www.kernel.b力                                               정재준（r야)i3307自）nate.com)
                                          118/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                      커널 sort 테스트



빌드하고 실행하는 방법이 아직 익숙하지 않다면, 앞에서 이미 설명한 "커널 모듈 프로그래밍 " 을

한번 더 복습하1 주시기 바랍니다．



위의 소스에서 TEST_LEN 은 1000으로 정의 되어 있습니다. 그래서 데이터를 printk로 출력하면

너무 많은 결과가 나오기 때문에 TEST_LEN 을 10 으로 수정하고. so比 함수를 실행하기 전에 난수를

발생시키는 向I 루프에서 printk 를 추가하여 데이터를 출력해 보면 다음과 같습니다．




町_info("sort before data［今6d]:", DLEN); /／추가함
向r (I = 0; I <DLEN; i++){      1:弓q（戶t石H
        r = (r * 725861) % 6599;
        a[i] = r;
        汀inf이"%d, ", 叩］）·, /／추가함
}
아inf이"\n");




an 22 15:24:28 HP7100U kernel: [28176.552921] test_sort: test_sort_init() starting...
Jan 22 15:24:28 HP7100U kernel: [28176.5529291 test_sort: sort before data[10]:
Jan22 15:24:28 HP7100U kernel: [28176.552933] test_sort: 6570,
Jan 22 15:24:28 HP7100U kernel: [28176.552936] test_sort: 5893,
Jan 2215:24:28 HP7100U kernel: [28176.5529401 test_sort: -870,
Jan 2215:24:28 HP7100U kernel: [28176.552942] test_sort: -1166,
Jan 22 15:24:28 HP7100U kernel: [28176.552945] test_sort: -5780,
Jan22 15:24:28 HP7100U kernel: [28176.552948] test_sort: 4192,
Jan 2215:24:28 HP7100U kernel: [28176.552951] test_sort: -4333,
Jan22 15:24:28 HP7100U kernel: [28176.552954] test_sort: 1823,
Jan22 15:24:28 HP7100U kernel: [28176.552957] test_sort: 6524,
Jan 2215:24:28 HP7100U kernel: [28176.552960] test_sort: 628,




    커널연구회佃쌔쌔／.kernel.b라                                                 정재준（四b13307（흐）nate.com)
                                            119/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                    커널 sort 테스트



Jan 22 15:24:28 HP7100U kernel: [28176.5529631 test_sort:




그리고 sort 함수가 실행된후 데이터 크기를 확인하는 向r 루프에서 prinik 을 추가하여 데이터를

출력하면, 다음과 같이 정렬된 데이터가 순서대로 출력 됩니다．



소스 수쩡한 부뵨

마info("sort after data[%d]: ". DLEN); /／추가함
for (I = 0; 1< DLEN-1; i++) {
        if (a[i] > a[i+1]) {
                 pr_err("sort test has failed.\n");
        goto exit;
        }
        pr_i肝O(" %d, ", 的］）·, /／추가함
}
p乙inf이"%d如", a[i]）·, /／추가함




Jan 22 15:24:28 HP7100U kernel: [28176.552976] test_sort: sort after data[10]:
Jan 2215:24:28 HP7100U kernel: [28176.552978] test_sort: -5780,
Jan 22 15:24:28 HP7100U kernel: [28176.552982] test_sort: -4333,
Jan 22 15:24:28 HP7100U kernel: [28176.552984] test_sort: -1166,
Jan 22 15:24:28 HP7100U kernel: [28176.552987] test_sort: -870,
Jan 22 15:24:28 HP7100U kernel: [28176.552990] test_sort: 628,
Jan22 15:24:28 HP7100U kernel: [28176.552993] test_sort: 1823,
Jan22 15:24:28 HP7100U kernel: [28176.552996] test_sort: 4192,
Jan 22 15:24:28 HP7100U kernel: [28176.552999] test_sort: 5893,
Jan 22 15:24:28 HP7100U kernel: [28176.553002] test_sort: 6524,
Jan22 15:24:28 HP7100U kernel: [28176.553006] test_sort: 6570




    커널연구회佃m쌔／.kerne나묘）                                               정재준（rgbi3307@nate.com)
                                              120/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                    커널 sort 테스트



Jan 22 15:24:28 HP7100U kerneL: [28176.5530083 test_sort: sort test succeeded.




지금까지 설명한 예제는 리눅스 커널 소스를 테스트 하는 방법을 익히기 좋도록 아주 간결하게 작성된

소스입니다. 더구나 커널 모듈로 프로그래밍되어 있어서 테스트하기어匠 간단 합니다. 앞으로 리눅스

커널 소스를 위와 같은 방법으로 계속 테스트하고 그 내용을 설명하는 글을 주제별로 올리도록

하겠습니다. 그럼 다음글에서 뵙겠습니다．




  커널연구회佃쌔시／.kerneL.b기                                                정재준（rgb13307匣）nate.com)
                                          121 /351
                                                                        리눅스 커널 소스 해설 ［기초입문]
                                                                                커널 성능측정 도구




커널 성능측정 도구

                                                        이번글의 주제는 "리눅스 커널 성능 측정 도구" 입니다. 이것은

                                                        리눅스 커널 소스를 이해하는 과정에서 많은 도움을 주기 때문에
       kernel tools perf
                                                        잘 알고 있으면 좋겠습니다. 그런더1 커널 성능 측정 도구들은

                                                        생각보다 종류가 많습니다. 사용하는 방법이 문서화 되어 있지

                                                        않으면 활용할따1 많은 어려움을 겪게 됩니다. 그래서 필자는

커널 성능 측정 도구들을 체계적으로 정리하여 사용 방법들을 쉽게 기술 하도록 하겠습니다. 먼저

아래 그림[3 口은 리눅스 커널 성능 측정 도구들을 사용 영역（Scope & Capabil比y）과 편의성（Ease of

use) 별로 잘 구분해서 보여주고 있습니다．



      The eBPF Tracing Landscape, Jan 2019




        幕H근g留乙 mma늠mm心山 쇼
                                                        (Brendan's opinion)




                        好和그
                          뇨8
                                                                                   stap BPF
                                                               perf

                                                                                    bcc
                                                              ftrace     pe汀 BPF
                               (a巾h帥 小＋ (mat바e)
                                                                                   C BPF
                               Stage of
                               Dev叫야）ment         ,：르
                                                                                 Raw BPF
                                              Scope & Capability
그림참조：http:I/니／니／＼八／
                  .brendangrecig.com/ebof.html


3    그림 찹고 문서



    커널연구회佃쌔쌔,.kern이.b力                                                        정재준（rgbi3307@nate.com)
                                                           122/ 351
                                                               리눅스 커널 소스 해설 ［기초입문］
                                                                       커널 성능측정 도구



위의 커널 성능 측정 도구들 중에서 필자는 perf 와 ftrace 중심으로 기술 하도록 하겠습니다．




perf 설치하기

perf는 리눅스 커널 소스 " /toots/perf／士" 경로에 있습니다. 커널 소스에 포함되어 있지만 단독

프로그램으로 실행 파일이 만들어집니다. 단독 어플리케이션（도구 프로그램）으로 실행가능하기

때문에 penf 프로그램 소개, 설치, 사용부터 먼저 정리하고 소스는 후반부에 설명하는 순으로 글을

작성하도록 하겠습니 다．



perf 는 리눅스（우분투）에서 다음과 같이 패키지들을 설치하면 됩니다．



perf설치하카客

$ su（把 apt-get instaU Linux叱0이s-common Linux止0이s-generic Linux如이s-'uname 寸'




위에서 ' uname -r ' 은 설치된 커널 버전을 가져오는 쉘명령입니다. 그리고 다음과 같이 perf 실행에

관련되는 패키지들을 설치합니다．




$su（拍 apt-get inst체 flex 너son lib이f-dev Liba叱氾devLi배나dev libunwind士 아th애-dev 너叩비s-dev
libnuma-dev Libgtk2.O-dev Libbfd-dev LibeLfi Libperl-dev Libnuma-dev 毗）sLang2 LibsLang2-dev
tibunwind8 Libunwind8-dev binutils-muLtiarch-ciev eLfutils libiberty-dev




패키지들이 설치되고 나면 다음과 같이 perf 가 어디에 설치되어 있는지 확인합니다．




 커널연구회（的胛．kerne나）z)                                                        정재준（rgb13307芯）nate.com)
                                            123/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 성능측정 도구



per? 설치 위치 확인

$ whereis perf


perf: /usr/bin/perf     /usr/ share/man/manl/perf 1, gz



/usr/bin／에 설치되어 있습니다 ．그리고 버전은 다음과 같이 확인합니다． perf는 앞에 sudo 을

붙여서 root 권한으로 실행합니다．



per? 버쳔 확인

$ sucio perf -version


perf version 4. 20. gac60fb7




perf 실행을 위한 도움말은 다음과 같이 확인합니다．



per?도욤말확인

$ sudo perf -help


usage: perf [--version] [--help] [OPTIONS] COMMAND [ARGS]

The most commonly used perf commands are:
   annotate           Read perf. data (created by perf record) and display
   archive            Create archive with object files with build-ids found in
   bench              General framework for benchmark suites
   Duiiaici- caciie   Manage build-id cache.
    OWL上0 l (J 1J그 st List the buildids in a perf. data file
   c2c                Shared Data C2C/HITM Analyzer.
   confia             Get and set variables in a configuration file.
   data               Data file related processing
   0i11               Read perf. data files and display the differential
   evlist             List the event names in a perf. data file
   It race            simple wrapper for kernel 's ftrace functionality




커널연구회佃쌔쌔,.kerne나묘）                                        정재준（rgbi3307@nate.com)
                                    124/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                               커널 성능측정 도구



    inject       Filter to augment the events stream with additional
    kailsyms     Searches running kernel for symbols
    kmem         Tool to trace/measure kernel memory properties
    kvm          Tool to trace/measure kvm guest os
    list         List all symbolic event types
//[OPTIONS] 이하생략




혹시, perf을 설치하고 실행하는 과정에 문제가 발생하면 리눅스 커널 버전과 환경설정에 관련되는

것이므로 아래 웹사이트를 참조하시면 해결법들이 있습니다．


h比PS：小사니쌔,.quora.com/Ho＼們拘＋corn베e-a-Lin배口erf-tooL-with-aLL-features-For-Linux따-0-on-
UtM. ntv


h比外刃askubuntu.com/ques加ns/50145/how比어陌talL-p町卜monitoring叱ooL


참고로 perf는 커널 내부로 " perf_event_open" 시스템콜 함수를 통하여 접근하는더I,

이함수의 위치（주소）를 다음과 같은 명령으로 확인해 볼 수 있습니다. perf_event_open

함수 위치 정보가 다음과 같이 나타나지 않는다면 커널 빌드 및 설치를 다시 해야 합니다．

하지만，최근 커널은 perf을 기본적으로 제공하므로 문저1 없이 잘 동작합니다．


           템
$ nm vmlinux I grep perf_event_open
호으


$ sudo catjproc/kattsyms I grep perf_event_open

//／다음과 같이 출력됩니다．
ffffffff853e54f0 t 1 do_sys_perf_event_open
ffffffff853e6200 T 1 x64_sys_perf_event_open
ffffffff853e6230 T _ia32_sys_perf_event_open
ffffffff868d5e80 d event_exit_ perf_event_open
ffffffff868d5f20 d event_enter_perf_event_open




  커널연구회（邸사w.kerneLb기                                           정재준（rgbi3307（今nate,corn)
                                       125/ 351
                                                                                                                                                           리눅스 커널 소스 해설 t7I초입문j
                                                                                                                                                                   커널 성능측정 도구



ffffffff868d5fc0 d __syscall_meta_ perf_event山pen
ffffffff868d6000 d args_perf_event_open
ffffffff868d6040 d types__perf_event_open
ffffffff86c8d770 t __event_exit__perf小event_open
ffffffff86c8d778 t __event_enter_perf_event_open
ffffffff86c8ff70 t __p_syscall_meta__perf_event_open
ffffffff86c923e0 t 小eul addr1Hia3之sys_pe汗 event_open
ffffffff86c923f0 t _eil_addr___x64_sys_perf_event_open




그리고 perf에 대해서는 아래 웹사이트[4 띠에 잘 설명되어 있습니다．

http://www.brendangregg.com/linuxperf.html




                                                                     Un出 Perf아inance Observab小ty 而이S
                                str社Ce
                                                                              ," '                   adng S邪t帥’                                                           卜lard＼母酊0
                                                                                                                                                                                              ＼奴rious'
              lsc潼                                                                                                      net$ 乞at
                                                                                     \Op明             ”
                                                                                                                                                          sysdIg




                                  \\\
            pcsta玎                                                                                                                                                                        sar /proc
                                                              trac
                                                                                                                                                                          和erf           鈿t크七 dmesg
      노 外 （i죤ta之
                                                                                                                                                                                 \
           nerf                \ 尸＼ '                                                               \ Systemi
                                                                                                         ,"ns., r, '
                                                                                            Syi쥬（baIl inte心ace/f/ / / 0'.
                                                                                            느icat                                                     /
                                                                                                                                                                     7/
                                                                                                                                                                          It巾S 亡舟卜

                                                                                                                                                                                         1
                                                                                                                                                                                          turbostat




                                                                                                                r/
      rtrace      \                                                                                                                                                          CPU\
                                                          늦                                      뇩 鈿cket$ 切                                                               interconneci    A
                                                                                                                                                                     /.
       ＄七an                                                              VFS
                m
       I上tna F
       小             中




                                                                                                          TCPJODP
                                                                                                                                  Scheduler二
                                                          File Systems                                                                                       4叫       乞아） r塼 H仁
      乙CC {BPF) Y                                                                                                            r
                                                                                                                        f/
                                  \
                                                                                                                   'P 끼뇨 f/
                                                                                                                                                                                                          뇨뇨＼
                x                                                                           「                                                  Virtual r             pids七a七 Memory
      D口rtrace
       小
            1m


                二
                 .
                                      \Vo油m色Manag令
                                                                                                                              1
                                                                                                                                                                                                      ip七op
                                                                                                                             k M이加口＼
                C
                그                  B'ock De叭Ce 奴佃招ce                                                                                                                           Bus                    perf
                                                         E姚蜘唵
                                  /戶
                                                  Device                                                  Drive囹         \(\                     ,\                  ';
                                                                                                                                                                     ：짧蒜Hr石
                                                                                                                                                                                                 -4
                                                                                                                     I/O f3us\\                           " '-.-        free
     iostat
      1＜比아）
            ,                                                 perf               七iptop
                                                                                                                                  iptraf                           tcpdump                numas 乞a乞
                                                                                                                                                                                                      十
                                       Expander Interconnect
    blktrace
                                                     I/O Cont,예or                                                                                                                         nics七a乞
                         \,
                                                                                                          lflte！寸ace 和an町3orl                                                             ne七at改乞
                              r크H小    ]               !              J               r441             커
                                                                                                                                                                                                工p
                                                                         삐1
                              ! 머' " ! i 더' " 나娑"p j
                                                                     swapon /                                           就h如m7；而乖；111d恥的1

그림출처：ht中：//www.brendangreq9.com/Per叭inuxHobservabititv too1s.Dnq


4    웹사이트 참고 문서




    커널연구회佃At쌔／.kerneLbz)                                                                                                                                                  정쟤준（rgbi3307@nate.com)
                                                                                                                   126/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        커널 성능측정 도구




perf 활용하:7I

이제부터는 perf를 본격적으로 활용해 보도록 하겠습니다. perf는 다음과 같이 뒤에 옵션과 명령，

인자들을 전달하여 실행합니다＼고町 실행은 root 권한에서 하겠습니다·



U perf [OPTIONS] COMMAND [ARGS]



옵션들은 perf -help 을 실행하면 나타납니다．


perf는 커널 각각의 요소（이벤트）별로 성능을 평가합니다． perf 가 평가할 수 있는 이벤트 항목

리스트는 perf 에 list 옵션을 주어서 다음과 같이 실행하여 확인할 수 있습니다．



p心rf 평가 항목 리스트

# perf list


//／다음과 같이 출려됩니다．

branch-instructions OR branches [Hardware event]
branch-misses [Hardware event]
bus- cycles [Hardware event]
cache-misses [Hardware event]
cache- references [Hardware event]
cpu- cycles OR cycles [Hardware event]
instructions [Hardware event]
ref- cycles [Hardware event]

alignment- faults [Software event]
bpf- output [Software event]
context- switches OR cs [Software event]
cpu- clock [Software event]
cpu-migrations OR migrations [Software event]




  커널연구회（w胛．kerneLbz)                                정재준（rgbi3307回nate.com)
                                  127/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         커널 성능측정 도구



dummy [Software event]
emulation- faults [Software event]
major- faults [Software event]
minor- faults [Software event]
page- faults OR faults [Software event]
task- clock [Software event]
/／이하 생략．,




penF 가 올바르게 실행중인지 테스트는 다음과 같이 test 옵션을 주어서 실행합니 다．



 # perf test
  1: vmlinux symtab matches kallsyms              : Ok
  2: Detect openat syscall event                  : Ok
  3: Detect openat syscall event on all cpus      : Ok
  4: Read samples using the mmap interface        : Ok
  5: Test data source output                      : Ok
  6: Parse event definition strings              : Ok
  7: Simple expression parser                     : Ok
  8: PERF_RECORD_* events & perf_sample fields   : Ok
  9: Parse perf pmu format                       : Ok
19: DSO data read                                : Ok
11: DSO data cache                               : Ok
12: DSO data reopen                              : Ok
13: Roundtrip evsel- >name                       : Ok
14: Parse sched tracepoints fields               : Ok
15: syscalls: sys_enter_openat event fields      : Ok
16: Setup struct perf_event_attr                 : Skip
17: Match and link multiple hists                : Ok
18: 'import perf ' in python                     : FAILED!
19: Breakpoint overflow signal handler           : Ok
20: Breakpoint overflow sampling                 : Ok
21: Breakpoint accounting                        : Ok
//／중간 생략．.



                                                   kkkkkk
58: mem2node
59: x86 rdpmc



                                                   000000
60: Convert perf time to TSC
61: DWARF unwind
62: x86 instruction decoder - new instructions
63: x86 bp modify




커널연구회佃,ww.kerne나功                                           정재준（r야)i3307@nate.com)
                                128/ 351
                                                                                                                      라눅스 커널 소스 斟섈 I가초압문I
                                                                                                                              커널 성능측정 도구



위와 같이 perf가 테스트 되면, perf 옵션들 중어씨 top부터 알아 보도록 하겠습니다． perf에 top

옵션을 주어 실행하면, 다음과 같이 커널 내부에서 실행되고 있는 함수（Symbol)별로 Overhead 7F

발행하고 있는 비율을 스냅샵 형태로 보여줍니다．


perf top 실행

# perf Lop




 aniples: 2크6K of event ' cydes:ppp ' , 4000 lIz, Event count (approx. ): 19038743172
 verhead Shared Ob ect                            Symbol
   3. 19鬼 pen.                                        Pert yyparse




                                                                  1 rt m量 !
                                                                                    i 1 lj ]




                                                    1 { 工 !k k 1 d 1 d k 1 1 1 1 1k 小k t !+
                                                                                                  +
             pert                                     Pe八 yyte蓋




                                                               L r
                                                                 1
                                                                 3
                                                  rt r 1r
                                                        11 rt r
                                                              i
             tibc- 2. 27 .so                           mnt malloc




                                                          li lj ij
             弘e八                                      Pert hv C明nil｝弼l
             pert                                     沁rt rpeep
      ' ,    汁erneti                                  n社tiv已于1.丸ish fi b one user
           1 [kernetJ                                 uaniap page range
                                                                                      ！重 重
        :1   td 그.27. so                              do lookupx
     匕       弘erf                                     蜘p 釘｝rt 口verhead




                                                                                      iEr ij mk多 !
                                                                                                 81i t
                                                                                                     114 j
       j     弘e八                                      Pert Stab Afloc
             pe八                                      Pert s놔up會ra配




                                                                                                  K!r
         1   pe八                                      Pert leave scope
      1      [kernel]                                 C（華艾多晦e ran恥
         1   libc- 2.27. so                              inemniove 社vx un社11彗ned eruis
        ::   libc- 2.27. so                           mal.loc




                                                                                                t {

                                                                           요 rt { rL rL r
                                                                                        三L r
                                                                                           臣
                                                                                           im 口
                                                                                              三
                                                                                              뇨
                                                                                       l
             perf                                     rb next




                                                                    !i rt r
                                                                          i
                                                                                             4 1 1{ j i 上 } i 1 上 1
             pert                                     Pert gv fetchpvn fl ags




                                                                                        王上 l
                                                                                           口1
             Ubc -2.27. 50                            ctree(aGLIBC 2.2. 5
         나   [kernel匡                                 entry SYSCALL 64
   口41 perf                                            上istsm insert out群汶 en乞ry
    r口        {kernel. }                              syscati return_vi計 ‘sysret
   「       i libglib그 . 孕 . so.0.56｛多分， 3             吼娩S九拓姚e took珏p
   0. 48毛 libc- 2.27 .so                                  St rci｝크fL드5芝2 珏nali邙每e心
    ) 47'     r 1\ i그 r IiF스그 ;




다음으로 就at 옵션이 있습니다. stat 옵션으로 perf 을 실행하면 주어진 시간동안 커널 내부에서

이벤트 처리한 수를 카운트한 통계정보를 보여 줍니다. 아래는 ] 초동안 실행한 통겨1 입니다．


pe汗 stat 실행
 # perf stat sleep I




 커널연구회（ww니／.kernet . 뇨）                                                                                                   정재준（r야)i3307匣>1日Le.com)
                                         129/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                       커널 성능측정 도구




 Performance counter stats for 'sleep 1 ' :

              0. 81 msec task- clock           #    0.001 CPUs utilized
                  1      context- switches     #    0. 001 M/ sec
                  0      cpu-migrations        #    0. 000 K/ sec
                 67      page- faults          #    0. 083 M/sec
         1,172, 031      cycles                #    1. 452 GHz
           946, 412      instructions          #    0. 81 insn per cycle
           191, 239      branches              #   236. 944 M/sec
             7, 904      branch-misses         #    4.13% of all branches

       1.001424418 seconds time elapsed

       0. 001239000 seconds user
       0. 00(三）
              0（三）
                （三）
                 （三）
                   00 seconds sys




perf record

위에서 실행한 perf top 은 커널에서 실행하고 있는 정보들을 화면에 실시간의 스냅샵으로 보여주는

장점은 있지만. 내용이 실시간으로 변화기 때문에 자세히 분석하기 힘든점이 있습니다. 그러나 perf

record 을 실행하면 분석 정보들이 "perf.data" 파일로 저장되고 이것을 자세히 분석할 수 있습니다．

"perf.data" 파일은 perf record 을 실행한 현재 경로에 저장됩 니다．


perf record 을 다음과 같이 실행하면 콘트롤 C 을 누를때切囚 분석정보를 저장합니다．



per? r旦cord 쇠혤
root@HP7100U: /tmp# perf record

/\（二 //／여기서 컨트롤 C을 눌렀습니다．
[ perf record: Woken up 1 times to write data ]
[ perf record: Captured and wrote 1. 531 MB perf. data (2946 samples) ]




 커널연구회佃m쌔／.kern日.bz)                                  정재준（r야)13307@nate.com)
                                    130/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                       커널 성능측정 도구



penf record 을 다음과 같이 引eep 옵션을 추가하여 실행하면 引eep 옵션에 준 초단위 만큼 저장하고

종료합니다．



root@HP7100U: /tmp# perf record sleep 3



[ perf record: Woken up 1 times to write data I
{ perf record: Captured and wrote 0. 015 MB perf. data (9 samples) ]




penF record 는 특정 프로세스 혹은 모든 프로세스에 대해서 동작하는 옵션 및 여러가지 옵션들을

가지고 있습니다．



perf,record윱선毋
perf record -p PID              //／해당 PID 만 저장합니다．

perf record -p 3994 sleep S     ///PID 3994 프로세스를 5초간 저장합니다．

perf record -a                  //／모든 프로세스를 저장합니다．

perf record -a sleep 5          //／모든 프로세스를 5초간 저장합니다．

perf record -g                  //／스택 정보도 저장합니다．

perf record -e NAME             //／이벤트 NAME에 대한 정보를 저장합니다．

perf record -F NUM              //／분석 주기（Hertz）을 NUM으로 준 수치로 합니다．




 커널연구회（w사＼사.kerneLb기                                  정재준（因bi3307@nate.com)
                                 131 /351
                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                            커널 성능측정 도구




perf report

perf record 에 의해서 저장된 "perf.data " 파일을 분석하3t 위해서 perf report 을 실행합니다．

perf report 을 다음과 같이 실행하여 분석한 내용을 화면에 출력합니다．


perf report 실행
root@HP7100U: /tmp# perf report




·erfre ·ort 출력 화면
S三imples: 1K of event ' cyrl.es:ppp . Event count (app ro乂 .Th 138543637
Overhe크d Co凸系i三nd              Shar已d Obje之t                Symbol.
            S났apper            Ikernel. vmtinuxj              kJ intel. idle
            5났apper            [kerneLvmli.nuxj              hi xhci irq
            swapper            [kerneivmlinux]               ki update blocked,,,ave rages
            S났apper            Ikernel .vml.inuxj            kj stack trace call
            swapper            [kernel. vrntinuxl            hi check stack
            S낯apper            [k횬mnel ; vrnl.inux 重          K] rcu 1드七iatching
            S낳apper            [kernel. .vml.inuxj            K] cpuidle小 enterstate
            S났apper            [kernel.. vmlinuxj            hi mt三pdateloa寸，avg cfs r｛至
            swapper            [kernel. vmlinuxj             k ] menu select
            S낯apper            [Unknown]                     kJ 0xtttt村 ttc0bce0（玎
            F作洲) rker/2:2-,羽斟  Iker nel. . vinUnuxi          k] check stack
            swapper            [unknown]                     卜；j 0xffff1fffc0bce000
            5닙apper            [k已mnel. . vet끄mxj            hi handle edge irq
  日. 4色毛 S낯apper               [kernel. . vmlinuxj           hi timerqueue add
   0.38毛 k낯＜)rker/u8 :卜 ev [kernel. vmllnuxi                 ki I！三it 낯alt entry
   會 . 38毛 kworker/u8:3- ev [kernel .vml.inuxj               k] check move的evicta泌e多ages
   B , 37急 5村apper             [kernel.. vml끄珏xJ             hi    next timer iaterrupt
   0 , 36急 sot f ice.bin      libmergedlo. so                  1 鈿 r口blec.t ; : GetName
                                                                .
   6. 36屯 swapper              [kernel. vn促끄lUX l            hi epic acK, irq
   好 . 3多毛 5낳a群｝er             [kernel..vml.inuxj            ki xhci dma to transfer rino
   0 . 3斛3 多址特'C 竹ter亂nal - [kernel. .vmlinuxJ               hi stack trace ca珏
   (} . 3크智 S낯a湃｝er            [kernel. . welinux I          K] kfree
   8 . 30鬼 swa至弔er             [kernel , 硼珏끄lux I            k] pm qos request
   6 : 30智 swa湃｝er             [unknown]                     kj 0xffffffffc0bce08b
   a , 3字毛 S놔a！叩er            [kernel. v潘linuxi              k] do idle
   0. 針｝毛 節址腑e- sheU          [kernel.vml그．nuxJ              卜；j check stack
   0 . 28屯 51닢크r琿er           [kernel .vmlinux]              K] rb next
   () . 23屯 gnome. sheU       Ubgl 王b- 2 . 包 so . 包 56的 , 3    j g main context prepare
   0 , 28毛 塑瓠烈｝c- terminal. - tibgak-3. so. 0. 2200.30         1 g typ目曲e必1              is a解八t
                                                               j 吼main 加心弘r
                                                            .
   0 , 28；뇨 珏客｛多 rC（노l.or     libglib- 2, 0, no. 0. 5600.3  .


   6. 28毛 k孕珪｝rker/u8 : 3- ev [kernel. vmlinux I             k] update blocked averages




 커널연구회（艸,w.kerneL.bz)                                                     정재준（rgbi3307@nate.com)
                                             132/ 351
                                                                  리눅스 커널 소스 해설 ［기초입문］
                                                                          커널 성능측정 도구



perf record 를 실행할丘小g 옵션을 추가하여 실행하면 다음과 같이 스택 정보도 perf report 에서

확인할 수 있습니 다．


                0 』04% sb斟和er              [ kerie{ , vm｛끄｝u)c                   1k] common interrupt
   13. 15毛      色07屯 5＼寸apper              [kerneLvmUnuxj                        汁；] do IRQ
    } =  B== do IRQ
         1.23鬼 handle ir珏
            11.08% handle edge irq
               1包18鬼 han（疑e irq 斟嶝！珪
                   10.08毛 缸磊！磁｛已1八芝even（辨rc伊j
                    . 9.81鬼   handi.色 王rq event percpu
                       . 9忿7急 xhci msi i rq
                            S 五7乞 xhc王 王rq
                               4. 73毛 finish t珪
                                , 吼52毛 xhci t珪 cleanup
                                      4.46% xhci giveback orb in irq.            a. 41
                                        已 4.08% usb hcd niveback orb
                                           . 王76'屯       珏Sb 亨｝C（多 {}iveback 珏rb
                                               - 2.0孚뇨 ifltr compl.ete
                                                      1, 85屯 usb eubnilt orb
                                                          1 ,64乞 usb hcd submit urb
                                                               1屈7智 xhci 們也帥叫eue
                                                                  e好拉毛 ,chci多ueue intr tx
                         8.58屯 （特！好 1丁｛耳 }l磊升｛土ter
        1涍1毛 1 rq eflter
            8.82% tick irq enter
                0. 17% swapper              [kernel .voi1.i갸나x)                  1k] hand노 irq


위와 같은 스택 추적 정보는 플레임그래프（FlameGraphs）로도 출력해 볼 수 있습니다．

플레임그래프을 출력하기 위해서는 다음과 같이 플레임그래프 소스 코드를 다운로드 받습니다．


푤레임그래프作Lan忙Gra아Is) 소스 받7J
$ git clone http: //github. com/brendanqrecici/Flameoraoh. git



소스를 받은 경로에 디amegraph 라는 경로가 생성되고 그 안어牛 다음과 같은 소스 파일들이

있습니다．




푤레임그래프作LameGraph引 소스 파일들
$ 11 Flamegraph!

 drwxr- xr- x 7 jungjj        jungjj         4096     3 월 21 13: 36 .1
 drwxr- xr- x 5 jungjj        jungjj         4096     3 월 21 13: 41 . .1




 커널연구회（小八사＼사．kerneLb기                                                        정재준(rgbi3307@nate.com)
                                               133/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                             커널 성능측정 도구



-rwxr- xr- x 1 jungjj    ]ung刀     638     3 월 21 13 :33 aix-perf .pl士
drwxr- xr- x 2 jungjj    ]ung刀    4096     3 월 21 13 : 33 demos!
drwxr- xr- x 2 jungjj    ]ung刀    4096     3 월 21 13: 33 dev!
-rwxr- xr- x 1 jungjj    ]ung刀    3640     3월 21 13: 33 difffolded . p1*
drwxr- xr- x 2 jungjj    ]ung刀    4096     3월 21 13: 33 docs!
-rw- r- -r- - 1 jungjj   ]ung刀 1382457     3 월 21 13: 33 example - dt race -
stacks. txt
-rw- r- -r- - 1 jungjj   jungjj   155251   3월 21 13: 33 example- dtrace. svg
-rw- r- -r- - 1 jungjj   jungjj   110532   3월 21 13: 33 example- perf-
stacks. txt. gz
-rw- r- -r- - 1 jungjj    jung刀   404484   3 월 21 13: 33 example- perf. svg
-rwxr- xr- x 1 jungjj    lung刀      1293   3 월 21 13: 33 files . p1女
-rwxr- xr- x 1 jungjj     jung刀    34894   3 월 21 13 :33 flamegraph . p1*
drwxr- xr- x 8 jungjj    Jung刀      4096   3 월 21 13: 33 .git/
-rwxr- xr- x 1 jungjj    Jung刀      2798   3 월 21 13 : 33 jmaps玄
-rwxr- xr- x 1 jungjj    ]ung刀      2710   3 월 21 13: 33 pkgsplit 1perf.pl*
-rwxr- xr- x 1 jungjj    lung刀      4517   3 월 21 13: 33 range-perf. pl出
-rw- r- -r- - 1 jungjj   Jung刀      8826   3 월 21 13: 33 README . md
-rwxr- xr- x 1 jungjj    ]ung刀       669   3 월 21 13: 33 record- test. sh*
-rwxr- xr- x 1 jungjj    jungjj     1185   3 월 21 13: 33 stackcollapse- aix . pl士

//／이하 생략．.




위의 소스 파일들은 perf에서 다음과 같이 사용됩니다 ．먼저 perf record 을 -g 옵션으로 실행하여

스택 추적정보 까지 저장한 후 perf script 을 다음과 같이 실행합니다．


$ sudo perf record -e context- switches -ag

$ sudo perf script 1 Flamegraph!stackcollapse-perf.pl 1
Flamegraph/ flamegraph . p1 > graph. svg



위와 같이 실행하면 graph.svg 파일이 생성되고 이것을 열어보면 다음과 같이 보입니다．




커널연구회（蜘胛．kern이.bz)                                          정재준（r야) 3307@nate口corn)
                                    134/ 351
                                           리눅스 커널 소스 해설 E기초입문］
                                                   커널 성능측정 도구



                 目혀-r그e Gra口h




           n兀 罐L. ,
           rorker.. d..
           thread 毖心




위의 그래프는 커널에서 context-switches 이벤트가 발생할때1 사용한 스택비율（가로방향）과 호출된

스택깊이（세로방향）을 보여줍니다．




perf probe

pe寸 probe 을 사용하면 커널에서 특정 이벤트가 동작하는 시점부터 분석정보를 추적할 수 있습니다．

먼저 추적을 원하는 커널 이벤트（함수）를 다음과 같이 probe 등록 합니니다．



perf probe 이벤트 등록
# perf probe schedule




위에서는 커널 schedule 함수를 이벤트로 등록 했습니다. 등록된 리스트는 다음과 같이 확인합니다．



# perf probe - -list




 커널연구회（\A쌔쌔,.kerrie나끄）                         정재준（r야)13307匣）nate.com)
                                135/ 351
                                                리눅스 커널 소스 해설 E기초입문］
                                                        커널 성능측정 도구



  probe: schedule      (on schedule@kernel/ sched/core.c)




다음과 같이 perf record 을 실행하여 아obe 에 등록된 이벤트를 추적한 내용을 저장합니다．



pe汗 probe 이벤트 추적（실행）
# perf record -e probe: schedule -agR sleep 3




결과는 다음과 같이 perf report 을 실행하여 확인합니다．



perf probe 결과 확인
# perf report




perf probe 에 등록된 이 벤트는 다음과 같이 삭저！합니 다．



perf probe 이벤트 삭째
# perf probe - -del schedule

Removed event: probe: schedule




커널연구회（www.kerneLbz)                                  정쟤준（rgbi3307（孕nate.com
                                 136/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                             커널 성능측정 도구




perf 소스 빌드하기

perf소스를 빌드하는 방법은 간단합니다. 리눅스 커널 소스 " tools/perf/" 에 들어가서 다음과 같이

make 을 실행하면 빌드 됩니다．


$ cd tools/perf
$ make




石3 분만에 소스 컴파일이 완료 됩니다． 빌드한 경로에서 다음과 같이 perf파일 목록을 보면 penf

실행파일이 생성된 것을 확인할 수 있습니다．


빔드한 perf 싶햄파얗확인
linux- 5@Hp71eou : -/kernel/linux- stable/ tools/perf$ 11 perf出
 -rwxrwxr- x 1 linux- 5 linux巧            21993504 3월 19 03: 43 perf士
 -r닙xr- xr- x 1 linux- S linux巧               1333 3 월 19 03: 42 perf- archive*
-rw- r- -r- - 1 linux- 5 1unaiaeioon          1333 1 월 28 17 :25 perf- archive. sh
 - rw- r - - r - - 1 linux- 5 iunaiaeioon    12565 1 월 28 17 :25 perf. c
 - rw- r- - r- - 1 linux石 i unaiaeioon        6321 1월 28 17 :25 perf- completion. sh
 - rw- rw- r- - 1 linux占 linux- 5             2273 3 월 17 08: 06 perf. h
 - rw- rw- r- - 1 linux巧 -I그flux- b       26319816 3 월 19 03: 42 perf-in. o
 - rw- rw- r- - 1 linux- 5 -I그nux 吐）        582816 3 월 19 03: 42 perf. o
 -rwxrwxr- x 1 linux日5 -L그flux- b             7612 3 월 19 03: 42 perf- read -vdso32*
 - rw- rw- r- - 1 linux巧 1그flux- b             547 3 월 17 08: 06 perf- read- vdso .c
 -rwxrwxr- x 1 linux- 5 1그nux- b              7488 3 월 19 03: 42 perf- read -vdsox32*
 - rw- r - - r - - 1 linux巧 1unaiaeioon       1300 1 월 28 17 : 25 perf- sys . h
                                    1
 -rwxr- xr- x 1 linux巧 -I그 flux- b            6894 3 월 19 03: 42 perf =with -kcore*
                        .   .   VJ




 -r닙＝r- -r = H 1 linux- 5 1unaiaeioon         6894 1월 28 17: 25 perf -with- kcore. sh

//／이하 생략．.



perf 실행은 root 권한으로 해야 합니다. 다음과 같이 penf의 버전을 확인합니다. 필자는 커널 소스

v5.O 에서 빌드 해서 버전 정보가 다음과 같이 출력 됩니다．




 커널연구회佃川쌔床erne나川                                             정재준（r야)13307@nate.com)
                                     137/ 351
                                         리눅스 커널 소스 해설 ［기초입문］
                                                 커널 성능측정 도구




빌드한 perf 버전 확인
# perf - -version

perf version 5. O. g206815f




 커널연구회（艸,w.kerne나江）                          정재준（rgbi3307@nate.con介
                              138/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                          ftrace 활용




ftrace 활용

                             ftrace 는 커널 소스들이 실행되는 과정을 추적할 수 있도록

                            커널에 내장되어 있는 기능 입니다. 커널 소스를 분석할 때 아주

      KerneJ ftrace         유용한 도구로 활용할 수 있습니다. Ftrace 는 커널 v2.6 부터



   Y                        기능이 탑재되어 \,3.10 과 v4.13 에서 업그레이드 되었습니다．

                            Ftrace 는 커널 문서에서 자세히 잘 설명하고 있습니다. 필자도

아래 문서를 참고하여 사용 방법들을 정리 했습니다．


ftr社C臂疊명 문서
Documentation/ trace/ftrace. rst
Documentation/ trace/ftrace- design. rst
Documentation/ trace/ ftrace-uses. rst



Ftrace 는 커널에서 제공하는 tracefs 파일 시스템을 활용하여 동작을 제어햐기 때문에 커널 소스를

수정하지 않고도 디버깅할 수 있어서 편리 합니다. "/sys/kernet/debug/tracing" 경로에 있는

파일들이 ftrace 을 제어하는 파일들입니다. 사용자는 이 파일들에 데이터를 읽고 쓰는 방식으로

I trace올활용할수 있습니다. 먼저 "/sys/kerneL/debug/tracing" 경로에 있는파일들을확인해

보겠습니다．                       'MN 「’ (:n$, .늑舒」 n毗ynl蝴
在ys/keni到川e蜘g/tracil四 겅望 안와내용
root@HP7100U: /sys/kernel/debug/ tracing# 11
               1 root root 0 3 월 18 08: 02 available events
               1 root root 0 3 월 18 08: 02 available filter functions
               I root root 0 3 월 18 08: 02 available tracers
               1 root root 9 3 월 18 08: 02 buffer_percent
느 r닙1r 11r = = 1 root root 0 3월 18 08: 02 buffer size kb
               1 root root 0 3 월 18 08: 02 buffer total size kb




 커널연구회佃쌔쌔／.kerneLb기                                   정재준佃非滔307@nate.com)
                                   139/ 351
                                                                          리눅스 커널 소스 해설 [71초입문j
                                                                                     ft race 활용



-rw- r- -r- -                     1 root root 0    3 월 18 13: 21 current     tracer
 rw- r- -r- -                     1 root root 0    3월 18 88: 02 dynamic_events
drwxr- xr- x 105 root root 0                       3 월 18 08: 03 events!
drwxr- xr- x                      2 root root 0    3월 18 08: 02 options!
//／이하 생략．..


만약 이런 파일들이 보이지 않는다면, 커널 소스를 다시 빌드 해야 합니다. 빌드 할따1 설정 상수값은

menuconfig 의 " Kerne나iacking > Tracers" 메뉴어나］다음과 같이 설정합니다．




                                                          !   r 月 二 i그

     Arrow keys navigate the menu. <Enter> selects submenus ---> (or empty subineaus
     - - - --) . Highlighted letters are hotkeys. Pressing <Y> includes, <N> excludes,
     cM> modularizes features. Press <Esc><Esc> to exit, .c?> for Help, <I> for
     Search. Legend: (* ] built- in I ] excluded <川> module < > module capable



          a H[
                                了racers
                m 未
                ]
                                 Kernel Function Tracer
                                     Kernel Function Graph Tracer
                卞



        r1
          r      ] ]] ]
        t       m
                1                 Enable trace events for preempt and irq disable/ enable
                                  Interrupts- off Latency Tracer
                      斗

          1[
                                  Scheduling Latency Tracer

                1] 1J  m 1j
                                  Tracer to detect hardware latencies (like SMIs)
        i
        r
                                  Trace syscatls
         m
                牢  京  窄
          L
          r                       Create a snapshot trace buffer
                                     Allow snapshot to swap per CPU
                                  Branch Profiling (No branch profiling)   - - ->

          ]J 11 11 ]1 l1 1J ]
                                  Trace max stack




          [ rt r 1 [1
                                  Support for tracing block TO actions
                                  Enable kprobes.based dynamic events
          求  京  本     牢  卞  牛




               tr
                                     Do NOT protect notrace function from kprobe events
                                  姦nable uprobes- based dynamic events
          rL
                                  enable/ disable function tracing dynamically
          r
          1
                                  kernel function profiler
                       ]
                                  Enable BPF programs to override a kprobed function
          lJ 1] 1
                1J
                                  Perform a startup test on ftrace
          r
             半 求
          1
                                 M暾mory mapped ID tracing
             r1 r1
                                 Histogram triggers
                                  Test module for mmiotrace
          <            >


                       =]
                                  Add tracepoint that benchmarks tracepoints
          1
          i
                                 Ring buffer benchmark stress tester
                                  Ring buffer startup self test
                                 Preempt / IRO disable delay thread to test latency tracers
                                  各ho노寸 eval mappings 化r trace events
                                  Trace gpio events


                                    Select    < Exit >    < Help >       < Save >     < Load >




 커널연구회佃쌔,w.kernet.b라                                                                정재준佃羚沼307@nate.com)
                                                         140/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                             ftrace 활용




그런데, 위의 CO NFI(; 옵션들은 기본적으로 설정되어 았는 옵션들이기 때문에 커널 소스를 다시

빌드하지 않아도 I trace 는 기본적으로 동작합니다. 자 이제 Itrace 을 활용하1 보겠습니다. 먼저 Itrace

을 제어하는 파일들이 있는 "/sys/kerneL/debug/tracing" 경로로 이동 합니다. 반드시 root사용자

계정에서 작업해야 합니다. 이 경로 안에 있는 파일들 중에서 먼저 ftrace 을 동작 시키기 위해서

중요한 역할을 하는 파일들부터 보겠습니다.




추적 가능 항목들

I trace 는 크게 이벤트 단위와 함수 단위로 커널 소스 실행 과정을 추적할 수 있습니다. 추적 가능한

이벤트는 ava岫벼e events 파일안의 내용O和l 확인할 수 있습니다. 다음과 같이 ]840 개 등록되어

있습니다．

                                                                   C心中小七 )
추적7浩한이볜트목콕확인                              m甘 申9 叭꺼 ( " "t
root@HP7IOOU:/sys/kernet/debug/tracing# cat avaiLabLe_events

mac802ll: drv return void
mac8G2li: drv return mnt
mac8G2ll: drv return bool
mac802ll: drv return u32
mac802ii: drv return u64
mac802ll: drv start
mac802ll: drv_get_et_st rings
mac802ll : drv_get_et_sset_count
mac802li: drv_get_et_stats
mac802ll: drv1.suspend
mac802ll: drv resume
mac802ll : dry_set_wakeup
mac802ll: dry_stop




 커널연구회佃쌔쌔／.kerneLb라                                       정재준（rgbi3307@nate.com)
                                    141 /351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                                        ftrace   활용



     mac8크2ll: drv add interface
     mac802ll: dry_change_interface
     mac802ll: drv remove interface
     mac802ll: drv_config

      //／이하 생략．.
      "available_events " [readonly] 1840 lines


     그리고 위의 이벤트들은 다음과 같이 events／하위 경로에 있는 파일들을 통하여 추적을 제어할 수

     있습니다．



     이世트하위켱로묵륙
     root@HP7100U : /syslkernelldebugltracing# 11 event s/

     drwxr- xr- x 105 root root 0   3 월 18 08: 03 .1
     drwx           8 root root 0   3월 18 08: 02 . .1
     drwxr- xr- x   6 root root 0   3 월 18 08: 02 alarmtimer!
     drwxr- xr- x 15 root root 0    3월 18 08: 03 asoc!
     drwxr- xr- x 20 root root 0    3 월 18 08: 02 block!
     drwxr- xr- x   6 root root 0   3월 18 08: 02 bridge!
     drwxr- xr- x 166 root root 0   3월 18 08: 03 cfg8o2ll!
     drwxr- xr- x 11 root root 0    3월 18 08: 02 cgroup!
     drwxr- xr- x 18 root root 0    3 월 18 08: 02 cik!
     drwxr- xr- x   4 root root 0   3 월 18 08: 02 cma/
     drwxr- xr- x 16 root root 0    3월 18 08: 02 compaction!
     drwxr- xr- x   5 root root 0   3월 18 08: 02 cpuhp!
     drwxr- xr- x   9 root root 0   3월 18 08: 02 dma_fence!
     drwxr- xr- x   5 root root 0   3 월 18 08: 02 drm!
     -rw- r- -r     1 root root 0   3 월 18 08:02 enable

     //／이하 생략．.




     ftrace 에서 추적 가능한 함수는 다음과 같이 avaiLabLe_f沚아_funct幻ns 파일에 53099 개 등록되어

있습니다．



추二
        카뇽한哲수 肆舞확인「




     커널연구회佃쌔,w.kerne나）z)                                     정재준（rgb13307（孕nate.con分
                                       142/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                           ft race 활용



root@HP71eeU : /sys/kernel/debug/ tracing# cat available_filter_ functions

trace initcall finish cb
trace initcall start cb
run_mnit_process
t ry_to_run_init_ process
initcall blacklisted
do one initcall
match_dev_by_label
match_dev_by_uuid
rootfs mount
name to dev t
bstat
calibration_delay_done
calibrate_delay
syscall_t race_enter
exit_to_usermode_loop
syscall_slow_exit_work                          叫垠 ., 4b)'". (꺼
do_syscall_64

//／이하 생략．.
"available_filter_ functions" [readonly] 53099 lines - -100%--




그리고, ftrace로 추적 가능한 항목들은 avaitab姮 tracers 파일의 내용들중에서 선택할 수 있습니다．



avaiLabte_tr恥母rs파옅 앞와내용
# cat available tracers

hwlat blk
mmiotrace
function_graph
wakeup_dl
wakeup_rt
wakeup
function
n야）




 커널연구회（www.kerneLbz)                                    정재준（rgbi3307@nate.com)
                                  143/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                           ftrace 활용


위의 항목들은 currentjracer파일에 등록하여 사용합니다. curre毗jracer파일 안에는 기본적으로

nop( 'trace nothing"）가 등록되어 있습니다． flop 로 등록되어 있으면 ftrace 는 이벤트 단위로

추적합니다．


亡urrent_tracer파잎 얀험 내용
 # cat current tracer
 n야）




ftrace 동작은 tracing_on 파일을 통하여 Enab(e/Disa비e 시킬 수 있습니다． tracing_on 파일에 ] 을

쓰넣으면 Ftrace동작은 Ena비e되고 0을 쓰넣으면 미sable 됩니다．


ftrace Enable
# echo 1 >   tracing_on




庶race D朽abi呵
# echo 0 > tracing_on




참고로 Ftrace 전체를 Ena비이미sable 명령어는 다음과 같습니다. 아울러 아래 명령은 penf, kprobes,

stack tracing, profiling 등에도 영향을 줍니다．


ftrace 젼斗蜘able/Disab노
# sysctl kernel. ftrace_enabled=0
# sysctl kernel. ftrace_enabled=1

또는


# echo 0 > /procisysikerneliftrace_ enabled
子recno . > Iproc/ sys/ Kerne.ilrlrace_enao上ea




커널연구회（的胛．kerne나）z)                                 정재준（r야)i3307@nate.com)
                                  144 / 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                         ftrace 활용




ftrace 실행 결과는 trace 파일과 trace_p巾e 파일에서 확인합니다. 2 7fl의 파일 모두 동일한 실행

결과 입니다만, trace_p巾e 파일을 통해서는 실시간으로 결과를 확인할 수 있습니다．




이벤트 단위 추적

지금까지 기술한 ftrace 기능들을 하나씩 실행해 보도록 하겠습니다. 먼저 커널 내부에서 발생하는

이벤트 단위로 ftrace 을 실행하여 그 결과를 확인해 보겠습니다. 다음과 같이 current_tracer 을 flop

로 설정합니다．


current_tracer설정
# echo nop > current_tracer

# cat current tracer
n야）




다음과 같이 커널 이벤트들 중에서 스케쥴러에 관련된 schedy日keup 을 추적 가능하게 합니다．


# echo 1 > /sys/kernel/debug/ tracing/events/sched/sched_wakeup/enable

# echo 1 > tracing_on




다음과 같이 실행 결과를 확인합니다．


# cat trace




 커널연구회（www.kerne比z)                                  정재준（r야)13307@nate.com)
                                 145/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                        ftrace 활용




# tracer: nop
#
# entries-in- buffer/ entries- written: 490/13068              #P: 4




                               ########
                                              -   => irqs- off
                                          /- - - -=> need- resched
                                     I / -- - -=> hardirq/softirq
                                     I I / 1 -=> preempt- depth
                                     III /           delay
             TASK-PID   CPU#         III I        TIMESTAMP FUNCTION
                I I       I           liii              I       I
           fcitx- 2520 [000] d. . . 36655. 504032:            sched_wakeup: comm=dbus-
daemon pid=2552 prio=120 target_cpu=001
           gdbus- 2961 [000] d. . . 36655. 504749:            sched_wakeup: comm=gnome-
terminal- pid=2959 prio=120 target_cpu=003
    kworker/u8:1-11776 [000] d. . . 36655. 505403:            sched_wakeup: comm=bash
pid=7410 prio=120 target_cpu=002
          <idle> -0    [000] d. s. 36655. 505757:             sched_wakeup:
comm=rcu_sched pid=10 prio=120 target_cpu=001

//／중간 생략．,

    kworker/u8:1-11776 [000] dN. . 36655. 555810: sched_wakeup:
comm=kworker/0:1H pid=270 prio=100 target_cpu=000
    kworker/u8:1-11776 [000] d. . . 36655. 556083: sched_wakeup:
comm=migration/2 pid=20 prio=0 target_cpu=002
     gnome- shell- 2604 [000] d. . . 36655.556639: sched_wakeup: comm=Xorg
pid=2481 prio=120 target_cpu=001
##### CPU 1 buffer started ####
          <idle> -0     [001] dNh. 36655. 644826: sched_wakeup:
comm=InputThread pid=2487 prio=120 target_cpu=000
          <idle> -0     [001] dNh. 36655. 644854: sched_wakeup: comm=systemd
pid=1 prio=120 target_cpu=002
          <idle>-0      [001] dNh. 36655. 644872: sched_wakeup:
comm=systemd-logind pid=882 prio=120 target_cpu=001
     InputThread- 2487 [000] d. . . 36655. 645158: sched_wakeup: comm=Xorg
pid=2481 prio=120 target_cpu=001




커널연구회如째I'却．kernel.bz)                                               정쟤준（rgb13307（孕nate.com)
                                                  146/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                          ftrace 활용



//／이하 생략．.

다음과 같이 Itrace 추적을 종료 합니다．



# echo 0 > tracing_on




위의 실행 결과를 보면, 왼쪽부터 TASK-P山 CPU# 베 기卜4ESTA卜liP FUNCT山N 순서의 행단위로

출력 되었습니다. F기D 에 해당하는 TASK7F 어느 CPU# 번호에서 어떠한 옵션들로 어떤 시간

(TIMESTA卜lip）에 어떤 FUNC기ON 이 실행 되었는지 보여 주고 있습니다． 여기서 TIMESTA卜liP 는

<sec>.<usec> 단위 입니다. 여기서 FUNCT山N 은 sched_wakeup 이벤트 입니다．




함수 단위 추적

지금부터는 ftrace 을 함수 단위로 추적을 동작 시키고 결과를 확인해 보겠습니다. 다음과 같은

순서대로 명령들을 실행합니다．




# sysctl kernel. ftrace_enabled=1         ftrace 가능 설정
# echo function > current tracer          현재 tracer 욜    function 으로 설정
# echo i > tracing_on                     ft race 시작
# sleep 1                                 1초 sleep
# echo 0 > tracing_on
                                          ft race 종료
# cat trace
                                          실행 결과 확인




 커널연구회如쌔八w.kernet.bz)                                   정재준（四b3307（孕nate.com)
                                    147/ 351
                                                                     리눅스 커널 소스 해설 E기초입문］
                                                                                ftrace 활용



ftrace 싶헝 겊과
# tracer: function
#
# entries-in- buffer/entries- written: 880/21023270                          #P: 4




                      ########
                                                 -    => irqs- off
                                             / - - - -=> need- resched
                                         I / -- - -=> hardirq/ softirq
                                         I I I -- -=> preempt- depth
                                         III /          delay
             TASK- PID           CPU#    IIII         TIMESTAMP FUNCTION
                I I                1     liii                  I         1
    kworker/u8 :1-11776 [000]           d.       .   .   30737 .202325: select_idle_sibling <-
    kworkerlu8 :1-11776 [00이            d.
                                                 .   .   30737. 202325: available_idle_cpu <-
    kworkerlu8 :1-11776 [000]           d.
                                                 .   .   30737 .202325: raw_spin_lock <-
    kworker/u8 :1-11776 [000]           d.       .   .   30737 .202326: update_rq_clock <-
    kworkerlu8 :1-11776 [000]           d.
                                                 .   .   30737 .202326: ttwu do activate <-
    kworker/u8 :1-11776 [00（크］          d.
                                                 .   ,   30737 .202327: activate task <-
    kworkerlu8 :1-11776 [000]           d.
                                                 .   .   30737 .202327: enqueue_task_fair <-
    kworker/u8:1-11776 [00(刀            d.
                                                 .   .   30737 .202327: enqueue_entity <-
    kworker/u8:1-11776 [000]            d.
                                                 .   .   30737 . 202328: update_curr <-
    kworker/u8:1-11776 [000]            d.
                                                 .   .   30737 . 202328: 1update_load_avg_se <  =




    kworkerlu8 :1-11776 [000]           d.       .   .   30737. 202328: _updat e_load_avg_cfs_rq
    kworker/u8:1-11776 [000]            d.
                                                 .   .   30737 .202329: update_cfs_group <-
    kworker/u8:1-11776 [000]            d.
                                                 .   .   30737. 202329: account_entity_enqueue <-
    kworker/u8 :1-11776 [000]           d.       .   .   30737. 202330: 1enqueue_entity <-
    kworker/u8:1-11776 [000]            d.       .   ,   30737. 202330: enqueue_entity -
//／이하 생략．.

위의 실행 결과를 보면, 왼쪽부터 TASK-P山 CPU# 베 기卜4ESTAMP FUNCTION 순서의 행단위로

출력 되었습니다. 미D 에 해당하는 TASK가 어느 CPU# 번호에서 어떠한 옵션들로 어떤 시간

(TIMESTA卜lip）에 어떤 FUNCT山N 이 실행 되었는지 보여 주고 있습니다. 여기서 T小作STAMP 는

<sec>.<usec> 단위 입니다．


이번에는 Itrace 을 특정 함수에 대해서만 추적하도록 하겠습니다. 다음과 같은 순서대로 명령들을

실행합니다．




커널연구회佃八차＼사.kerne나끄）                                                          정재준（rgbi3307(@nate.con分
                                                     148/ 351
                                                                         리눅스 커널 소스 해설 ［기초입문］
                                                                                                ft race 활용




# sysctl kernel. ftrace_enabled=1                                        ft race 가능 설정
# echo function > current tracer                                         tracer 을 function 으로 설정
# echo hrtimer_interrupt > set_ftrace_filter                             hrtimer_interrupt 함수 지정
# echo 1 > tracing_on
                                                                         ft race 시작
# sleep 1
                                                                         1 초 sleep
# echo 0 > tracing_on
                                                                         ft race 종료
# cat trace
                                                                         실행 결과 확인




              立｝
# tracer: function
#
# entries-in- buffer/ entries- written: 783/927                           #P: 4




                                                                                         ########
                                                   irqs- off    =>

                                     /          -  need - resched
                                                    -   -   -   =>

                                     1 /    e  =>  hardirq/softirq
                                                    -   -   -




                                     1 I / _- -=> preempt- depth
                                     III /        delay
                   TASK-PID   CPU#   IIII      TIMESTAMP FUNCTION
                      I I       I    liii
                                     h
                                     m                               I        I
           <idle> -0      [000] d. h. 40508. 445641: hrtimer_interrupt <-
smp_apic_timer_inter   rupt
           <idle>-0       [000] d. h. 40508. 449552: hrtimer_interrupt <-
smp_apic_timer_inter rupt
           <idle>떠        [000] d.h. 405크8. 453220: hrtimer_interrupt <-
smp_apic_timer_interrupt
 alsa- sink- ALC32- 2629 [000] d.h. 40508. 453503: hrtimer_interrupt <-
smp_apic_timer_interrupt
##### CPU 3 buffer started ####
           <idle> -0       [003] d.h. 40508. 457518: hrtimer_interrupt <-
smF느apic_t如er寸interrupt
           <idle> -0       [000] d.h. 40508 457561: hrtimer_interrupt <-
smp_apic_timer_inter rupt
##### CPU 2 buffer started ####
           <idle> -0       [002] d. h. 40508. 457561: hrtimer_interrupt <-




 커널연구회（www.kerne나）z)                                                              정재준（r야幷3307(＠陀te.com)
                                         149/ 351
                                                   리눅스 커널 소스 해설 E기초입문］
                                                              ftrace 활용


smp_apic_timer_interrupt
//／이하 생략．.

위의 실행 결과를 보면, 왼쪽부터 TASK-P山 CPU# 베 기卜4ESTA卜胛 FUNCTION 순서의 행단위로

출력 되었습니다. F기D 에 해당하는 TASK가 어느 CPU# 번호에서 어떠한 옵션들로 어떤 시간

(TIMESTAM미에 어떤 FUNCT山N 이 실행 되었는지 보여 주고 있습니다. 여기서 FUNC기ON 은

hrtimer_interrupt 에 대해서만 추적한 결과 입니다．




함수 그래匹 추적

지금부터는 ftrace 을 함수 그래프로 추적하고 결과를 확인해 보겠습니다. 다음과 같은 순서대로

명령들을 실행합니다．



                  好명甘실L1                                    설명
# sysctl kernel. ftrace_enabled=1              ft race 가능 설정
# echo function_graph > current_tracer
                                               function_graph으로 설정
# echo 1 > tracing_on
                                               ft race 시작
# sleep 1
                                               1초 sleep
# echo 0 > tracing_on
                                               ft race 종료
# cat trace
                                               실행 결과 확인




加各（a쉰哲겊콰
# tracer: function_graph
#
# CPU DURATION         FUNCTI아寸 CALLS
#
 n
 Z
         1   1         I   I   I   I
      0. 390 us   1    cpuidle_not_available( );
 기
                  1     cpuidle小select () {




커널연구회佃쌔,w.kerne나）z)                                   정재준（r야戶3307@nate.com)
                                 150/ 351
                                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                                       ft race 활용




  \
  J \
    J
    1 \
      J \
        / ) ) ) \
                1
                / \
                  / \
                    / ) ) ) \
                            / \
                              / \
                                J \
                                  J \1J
                                                      menu_select () {
                                                        cpuidle_governor_latency_req() {
                                          0. 392 us       pm_qos_request Q;
                                          0. 448 us       get_cpu_deviceQ;
                                          0. 398 us       pm_qos_read_valueQ;




J
\
                                          2. 965 us     }




2 2 2 2   2 2 2 2 2 2 2 2 2 2 2 2 2 2
                                                        tick_nohz_get_sleep_length() {
                                          0. 397 us        can_stop_idle_tick. isra. 11Q;
                                                           tick_nohz_next_event () {
                                          0. 402 us           rcu_needs_cpu() ;
                                                              get_next_tirner_interrupt () {




        乙
        J
        八
                                          0. 389 us             _raw_spin_lockQ;
                                          0. 625 us             _next_timer_interruptQ;
                                                                hrtimer_get_next_event () {
                                          0. 404 us                 raw_spin_lock_irqsaveQ;
                                          0. 387 us                 raw_spin_unlock_irqrestoreQ;
                                          2. 067 us             }
                                          4. 790 us         }
                                          0. 390 us         timekeeping_max_deferment ( );

//／이하 생략．.

위의 실행 결과를 보면, 커널 함수가 해당 CPU 에서 얼마 동안 호출되어 실행되는지 그 과정을 추적한

것을 확인할 수 있습니다．



이번에는 ftrace 을 함수 그래프로 추적할때1 특정 함수에 대해서만 추적한 결과를 확인해 보겠습니다．

다음과 같은 순서대로 명령들을 실행합니다．



                                                                                         섬명
# sysctl kernel. ftrace_enabled=1                                           ftrace 가능 M정
# echo function_graph > current_tracer                                      function_graph 으로 설정
# echo scheduler_tick > set_graph_function                                  cheduler tick 할수로 설정
# echo 1 > tracing_on
                                                                            ftrace 시작
# sleep 1
                                                                            1 초 sleep
# echo 0 > tracing_on
                                                                            ftrace 종료
# cat trace
                                                                            실행 결과 확인




       커널연구회佃쌔,w.kerneLb기                                                           정재준（rgb1330기＠nate.com)
                                                                151 /351
                                                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                                                       ftrace 활용




ftr缸e샀항겪과
# tracer: function_graph
#
# Cpu DURATION        FUNCTION CALLS




                       1)) ) ) ) ) )) ) )) )
                                                                       #
                                                 I    I        I       I   I     I




 0 e 0 0 0 0 e 0 0 0 e e 0
                                                           scheduler_ tick () {
                                               1. 287 us      raw_spin_lockQ;
                                               1.157 us      update_rq_clockQ;
                                               0. 992 us     task_tick_idle ( );
                                                             cpu_load_update_active() {
                                               0. 994 us       tick_nohz_tick_ stopped() ;
                                               1. 628 us       야）u load긔pdate( ) ;
                                               6. 390 us           }
                                               1. 232 us           calc_global_load_tick ( );
                                                                   trigger_load_balance() {
                                     1. 054 us                        raise_ softirq ( );
                                     3. 408 us                     }
                                   + 28. 458 us            )
                   \
               J
//／이하 생략．.


위의 실행 결과를 보면. 커널 scheduler_tick() 함수에 대해서만 해당 Cpu 에서 얼마 동안 호출되어

실행되는지 그 과정을 추적한 것을 확인할 수 있습니다．




커널연구회（www.kerneLbz)                                                                             정재준（I-야)13307@nate.coa分
                                                                               152/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                       ftrace 활용




ftrace 중요 옵션들

Ftrace 는 options 경로에 여러가지 옵션들이 있습니다．



ftrac opt拓I拓죵류
root@HP7100U : !sys/kernel/debug!tracing# 11 options!

-rw- r- -r- - 1 root root 0       3월 21 08: 35 annotate
-rw- r- -r- - 1 root root e       3월 21        bin
-rw- r- -r- - I root root 0       3월 21 08: 35 blk_cgname
口 rw- r = -r = 1 1 root root 0    3월 21 08: 35 blk_cgroup
= r닙＝r = = r- = I root root 0     3월 21 08: 35 bik classic
-rw- r- -r- - 1 root root 0       3월 21        block
- rw- r - - r - - 1 root root 0   3월 21        context-into
-rw- r- -r- - I root root 0       3월 21 08: 35 disable on free
-rw- r- -r- - I root root 0       3월 21        display- graph
- rw- r - - r - - I root root 0   3월 21 08: 35 event- fork
-rw- r- -r- - 1 root root 0       3월 21 08: 35 funcciraoh -abstime
- rw- r- - r- - 1 root root 0     3월 21 08: 35 funcarar가卜 cou
                                                    U   '   .   . '    .




-rw- r- -r- - 1 root root 0       3월 21 08: 35 tuncaraon- ciuration
//／이하 생략．.

위의 옵션들중에서 아래 내용은 기본적으로 ] 로 설정하여 활성화 하도록 합니다．




# echo 1 > options/display- graph                                     함수 그래프 출력
# echo 1 > options/ f unc_stack_trace                                 합수 스택 추적
# echo 1 > options/ function- trace                                   합수 추적
# echo 1 > options/ stacktrace                                        스택 추적
# echo 1 > options/ sym- addr                                         심볼 주소 표시
# echo 1 > options/ sym- offset                                       심볼 오프셋 표시
# echo 1 > options/userstacktrace                                     사용자 스택 추적
# echo 1 > /proc/ sys/kernel/ stack_tracer_enabled                    시스템 스택 추적 가능




 커널연구회（的／w.kerneL.bz)                                                 정재준（rgbi3307@nate.com)
                                         153/ 351
                                                           리눅스 커널 소스 해설 [ 'I초입문］
                                                                    crash 도구 사용




crash 도구 사용

crash 는 리눅스 커널 소스를 GNU gdb 와 연동하여 디버깅할 수 있는 도구 입니다． GNU gdb 는

막강한 기능을 가지고 있지만 사용하기 불편하고 커널 덤프파일을 해석하는데 많은 어려움이

있습니다. crash 는 커널 덤프파일을 쉽게 해석할 수 있는 명령어들을 제공하여 커널안의 변수들과

구조체, 메모리 데이터 , 링크드 리스트안의 내용들을 확인할 수 있습니다. crash 도구의 기능들은

h比p://people.redhat.com/anderson/crash_whitepaper／에 다음과 같이 정 리되어 있습니다．



crash 기능 요약
   .   니ye 니flux systems
   1   Linux kernel core dumps created by the Kdump facility
   1   Compressed Linux kernel core dumps created by the makedumpfile command (from
       kdump dumpfiles)
   1   Linux kernel core dumps created from by the Red Hat Netdump facility
   1   Linux kernel core dumps created From by the Red Hat Diskdump Facility
   1   Compressed Linux kernel core dumps created by the Red Hat Diskdump facility
   1   Xen host Linux kernel core dumps created by the Kdump Facility
   1   Xen guest Linux kernel core dumps created by the original xendump facility
   1   Xen guest Linux kernel core dumps created by the ELF-Format xendump facility
   0   Xen hypervisor core dumps created by the Kdump facility
   0   KVM guest Linux kernel core dumps created by the virsh dump Facility
   1   s390 Linux kernel core dumps created by the IBM standalone core dump Facility.
   1   s390x Linux kernel core dumps created by the IBM standalone core dump facility.
   0   Linux kernel core dumps created by the LKCD (Linux Kernel Crash Dumps) SourceForge
       아이ect
   1   Linux kernel core dumps created by the Mcore patch offered by Mission Critical Linux




좀더 자세한 소스와 매뉴얼등은 아래 웹사이트에 있습니다．




커녈연구회佃八사니／.kerneLbz)                                                정재준（rgbi3307（孕nate.co！川
                                         154/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                         crash 도구 사용



http://peopte.redhat.com/anderson/


crash 을 사용하기 위해서는 커널 소스를 -g 옵션으로 컴파일하여 Vfl化flux 커널 object (flame List)

파일이 준비되어 있어야 합니다. 그리고／dev/mem 에 의해서 생성되는 Live system memory

image 가 필요합니다. 아울러 리눅스 커널 버전과 아키텍쳐 종류（x86, arm, ia64, ppc64, s390）를

알고 있어야 합니다. 이러한 내용을 참고하여 필자가 crash 을 설치하고 사용한 경험들을 아래부터

기술하도록 하겠습니다．




crash 설치하71

필자는 아래와 같이 crash 을 설치 했습니다．



$ sudo apt install linux-crashdump

Reading package lists. . . Done
Building dependency tree wh
Reading state information. . . Done
The following additional packages will be installed:
  crash kdump- tools kexec- tools makedumpfile
The following NEW packages will be installed:
  crash kdump- tools kexec- tools linux- crashdump makedumpfile
0 upgraded, 5 newly installed, 0 to remove and 180 not upgraded.
Need to get 3, 003 kB of archives.
After this operation, 9, 510 kB of additional disk space will be used.
Do you want to continue? [Y/n]




설치 완료되면 /usr/너Mcrash 에 실행파일이 있습니다． crash 버전은 다음과 같이 확인 됩니다．




 커널연구회（ww＼사.kerneLbz)                                정재준（r야)1330기＠nate.com)
                                     155/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                       crash 도구 사용



$ crash -v

crash 7. 2.1
Copyright (C) 2002- 2017 Red Hat, Inc.
Copyright (C) 2004, 2005, 2006, 2010 IBM Corporation
Copyright (C) 1999- 2006 Hewlett-Packard Co
Copyright (C) 2005, 2006, 2011, 2012 Fujitsu Limited
Copyright (C) 2006, 2007 VA Linux Systems Japan K. K.
Copyright (C) 2005, 2011 NEC Corporation
Copyright (C) 1999, 2002, 2007 Silicon Graphics, Inc.
Copyright (C) 1999, 2000, 2001, 2002 Mission Critical Linux, Inc.
This program is free software, covered by the GNU General Public License,
and you are welcome to change it and/or distribute copies of it under
certain conditions. Enter "help copying" to see the conditions.
This program has absolutely no warranty. Enter "help warranty " for
details.

GNU gdb (GDB) 7. 6
Copyright (C) 2013 Free Software Foundation, Inc.
License GPLv3+ : GNU GPL version 3 or later
<http : //gnu . org/licenses/gpl. html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law. Type "show copying"
and "show warranty" for details.
This GDB was configured as "x86_64- unknown-linux- gnu".




필자가 이글을 집필하는 시점의 crash 버전은 7.2.x 입니다. 그리고 GNU gdb 버전은 7.6 입니다．




커널연구회佃W床erne나）z)                                   정재준（rgbi3307@nate.com)
                               156/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                            crash 도구 사용




crash 실행（Live)

crash 는 /dev/mem 디바이스 노드에 접근하여 덤프파일을 생성하기 때문에 루트 권한으로 실행하지

않으면 다음과 같은 오류가 오류가 발행합니다．


crash: /dev/mem: Permission denied



루트 권한으로 다음과 같이 crash 도움말을 확인 합니다．



# crash 냐1

Usage:
  crash [-h [opt] ][-v] [-s] [-i   file] [-d num] [-S] [mapfile] [namelist]
[dumpfile]

USAGE:

  crash [OPTION] . . . NAMELIST MEMORY- IMAGE[@ADDRESS]      (dumpfile form)
  crash [OPTION] . . . [NAMELIST]                            (live system form)

OPTI아怜 :

  NAMELIST
    This is a pathname to an uncompressed kernel image (a vmlinux
    file) , or a Xen hypervisor image (a xen- syms file) which has
    been compiled with the "- g" option. If using the dumpfile form,
    a vmlinux file may be compressed in either gzip or bzip2 formats.

  MEMORY- IMAGE
    A kernel core dump file created by the netdump, diskdump, LKCD
    kdump, xendump or kvmdump facilities.



 //／이하 생략． .




 커널연구회（蜘八사．kerne나）z)                                       정재준（rgbi3307@nate.com)
                                     157/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                    crash 도구 사용



crash 을 실행할때1 명령라인 옵션이 상당히 많은 편이지만, 크게 Live System 형태로 실행하는

경우와 덤프파일을 통해서 실행하는 형태7f 있습니다．


Live System 형태는 다음과 같이 실행합니다. Live 는／dev/mem 에 접근햐여 실시간으로

실행됩니다．



Live Sy就이n 형태로 쉴헹
 # crash [namelist]



위에서 [namelist］는 리눅스 커널 소스를 컴파일하여 생성한 vmlinux 파일입니다．


필자는 아래와 같은 머신에 vn化flux 파일이 저장되어 있습니다．


$ uname -a
Linux HP7100U 5.0.0+ #1 SMP Tue Apr 16 19:36:29 KST 2019 x86_64 x86_64 x86_64 GNU/Linux


$ It /tib/modules/5.O.O+/buiLd/vmlinux
-rwxrwxr-x 1 linux-S linux-S 623132376 4 월 1620:37 /tib/modules/S.0.0+/build/vmlinux*




vmlinux 파일이 있는 경로는 PATH 가 등록되어 있으므로 다음과 같이 [namelist] 옵션을 생략하고

crash 만 실행해도 됩니다．


Liv甘System 형태로 심헹
# crash



그런데. 필자는 다음과 같은 오류가 발행 했습니다．



WARNING: kernel relocated [332MB]: patching 103405 gdb minimal_symbol values




커널연구회佃쌔째／.ke毗나끄）                                                  정재준(r야)i3307@nate.com)
                                         158/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                    crash 도구 사용



crash: read error: kernel virtual address: ffffffff96fc2368 type: "page_offset_bas&'
crash: this kernel may be configured with CONFIG_STRICT_DEVMEM, which
   renders /dev/mem unusabLe as a Live memory source.
crash: trying /proc/kcore as an aLternative to /clev/mem


Segmentation fault (core dumped)




인터 넷을 찾아본 결과 crash 을 실행할때 다읍과 같이 -minim카 옵션을 추가하여 실행하면 오류없이

실행되고 crash> 프로롬트가 나타납니다．



# crash -minimal

crash: this kernel may be configured with CONFIG_STRICT_DEVMEM, which
       renders /dev/rnem unusable as a live memory source.
crash: trying /proc/kcore as an alternative to /dev/mem

NOTE: minimal mode commands: log, dis, rd, sym, eval, set, extend and exit

crash>




그러나 이렇게 실행하면 crash 의 모든 명령어를 실행할 수 없고 제한된 명령어(Log, 비s, rd, sym,

eval, set, extend, e川t)만사용할수 있습니다. 위에서 crash 가실행될때 출력한 메세지를보면

커널이 컴파일 될때 CONFIG_STRICT_DEVME卜4 옵션으로 빌드되면 Live memory source 가

불가능으로 된다는 내용이 있습니다. 그래서 필자는 CONFIG_STRICT_DEV卜4E卜4 옵션을 제거하여

커널을 다시 빌드 했습니다.（보통 이 옵션은 커널 빌드 설정에서 기본적으로 제외되어 있습니다．

필자는 커널 소스 분석과정에서 이 옵션이 추가된듯 합니다.)


필자가 다시 빌드한 커널 버전은 v5.0 입니다. 이 버전으로 다시 crash 을 실행했는데, 아쉽게도

다음과 같은 오류 메세지가 나타납니다．




 커널연구회（的加．kerne比z)                                                 정재준(rgbi3307@nate.com)
                                            159/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                            crash 도구 사용




crash: cannot allocate any more memory!




위의 오류를 해결하기 위해서 crash 에 다음과 같은 옵션을 추가하여 실행 합니다．


 # crash --no modules /lib/ modules/5.O. O-'- /build/vmlinux




crash 실행이 좀더 진행되다가 다음과 같은 오류 메세지를 출력하고 종료 됩니다．


crash: radix trees do not exist or have changed their format




커널의 radix tree 가 존재하지 않거나 형식이 변경되었다라는 오류 메세지 입니다. 리눅스 커널

소스는 v4.6 부터 rad炚 tree 을 점차적으로 줄이면서 XArray 로 대체해가고 있습니다．(XArray 에

대해서는 이 책의 후반에서 다루어 집니다） crash 도 버전 7.x 부터 이것에 대한 패치를 하고

있습니다만. 필자가 빌드한 커널 버전은 v5.0 인데 이버전은 좀더 높은 버전이라서 현재 crash 버전

7.2 에는 패치가 않되어 있는듯 합니다．


고민끝에, 리눅스 커널 소스 버전을 좀더 낮추기로 했습니다. 가장 오랜동안（Long Term) 안정화 되고

있는 v4.14.146 버전으로 선택했습니다. 이 버전으로 다시 빌드 했습니다. 빌드할따1 옵션에서

CONFIGjT데CT_D타小4E卜4 은 (=n）로 하여 제거 했고 CPU 아키텍쳐는 X86_64 입니다． 빌드하여

설치한 버전과 CPU 아키텍쳐 정보는 다음과 같습니다．




커널연구회（幽／硝i.kerne나江）                                      정재준（rgb13307（흐）nate.com)
                                   160/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                                  crash 도구 사용



Linux HP71크0U 4.14.146+ #1 SMP Fri Oct 4 22: 04:13 KST 2019 x86 64 x86 64
x86 64 GNU/Linux




위의 버전으로 설치한 vmtinux 파일은 아래와 같은 경로에 있습니다．



/lib/ modules/ 4 .14. 146+/build/ vmlinux




이제 다음과 같이 crash 을 실행합니다．



# crash /lib/ modules/4. 14. 146+/build/ vmlinux

crash 7. 2.1
GNU gdb (GDB) 7. 6

       KERNEL: /lib/ modules/4. 14. 146+/build/ vrnlinux
     DUMPFILE: /dev/mem
          CPUS: 4
         DATE: Sat Oct     5 08: 29: 01 2019
      UPTIME: 00:13: 08
LOAD AVERAGE: 0. 58, 0. 38, 0. 34
         TASKS: 592
     NODENAME: HP7100U
      RELEASE: 4.14.146+
      VERSION: #1 SMP Fri Oct 4 22: 04:13 KST 2019
      MACHINE: x86 64     (2400 Mhz)
       MEMORY: 7. 9 GB
           PID: 2574
      COMMAND: "crash '
          TASK: ffff8fff1c795d00       [THREAD_INFO: ffff8fff1c795d00]
           CPU: 0
         STATE: TASK_RUNNING (ACTIVE)

crash>




 커널연구회（艸쌔／.kerneLb기                                         정재준(r야)i3307@nate.com)
                                       161 /351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                             crash 도구 사용



리눅스 우분투 ] 8.04 배포본에서 Cpu 아키텍쳐는 X86_64, 리눅스 커널 소스는 v4.14.146, crash

버전은 7.2.1 에서 실행한 결과 입니다．


지금까지 발생 했었던 오류가 모두 없어졌습니다. crash 가 정상적으로 실행되어 crash> 프롬프트가

나타납니다. 이제 crash 명령어들을 입력하여 동작시킬 수 있게 되었습니다. crash 명령어들은

다음절부터 설명합니다．




crash 실행（덤프 파일）

crash 는 /dev/mem 에 실시간으로 접근하여 커널을 디버깅할 수도 있지만, 커널 실행 데이터를 미리

덤프해 놓고 이것을 가지고 디버깅할 수도 있습니다. 커널 데이터를 덤프하7t 위해서는 몇가지

도구들을 설치해야 합니다. 참고로 커널 덤프에 대해서는 아래 웹사이트에 자세히 설명되어 있습니다．


https://heLp.ubuntu.com/tts/serverguideJkernet-crash-dump.html


먼저 다음과 같이 kexec 도구들을 설치합니다．


$ sudo apt install kexec- tools

Reading package lists. . . Done
Building dependency tree
Reading state information. . . Done
kexec- tools is already the newest version (1: 2.0.16-lubuntul) .
kexec- tools set to manually installed.
0 upgraded, 0 newly installed, 0 to remove and 180 not upgraded.




필자의 우분투 18.04 버전에는 이미 설치 되어 있습니다．




커널연구회佃쌔,w.kerne小z)                                          정재준（rgb13307（孕nate.con力
                                    162/ 351
                                                       리뇩스 커널 交스 罐輦 ｛갸초입警！
                                                                crash 도구 사용



다음으로 Einux-crashdump 을 설치합니다．


$ sudo apt install      linux- crashdump

Reading package lists. . . Done
Building dependency tree
Reading state information. . . Done
linux- crashdump is already the newest version (4.15.0. 65. 67) .
0 upgraded, 0 newly installed, 0 to remove and 180 not upgraded.




이것도 이미 설치되어 있습니다．


커널 덤프를 가능하도록 다음과 같이 실행하여 "Yes" 을 선택합니다．



# dpkg- reconfigure kdump- tools




                                                                 Configuring kdump- tools F

 If you choose this option, the kdump- toots mechanism wilt be enabled. A reboot is still

  Should kdump- toots be enabled by default '

                                                m




위에서 " Yes"을 선택하면 /etc/d e fa u ft/kdurn p止00匕 환경설정 파일에 USE_KDUMP=1 이

저장되고 " No" 을 선택하면 USE KDU卜사느0 이 저장됩니다．


/etc/defauLt/kdun叩止O아S 파일 내용
# cat /etc/ default/ kdump- tools




 커널연구회佃八사＼w.kernel.bz)                                          정재준佃非焰307@nate.com)
                                         163/ 351
                                                          리눅스 커널 소스 해설 ［기초입문］
                                                                   crash 도구 사용




# kdump- tools configuration
#
# USE_KDUMP - controls kdump will be configured




                       ##########
      0 - kdump kernel will not be loaded
      1 - kdump kernel will be loaded and kdump is configured
  KDUMP_SYSCTL - controls when a panic occurs, using the sysctl
      interfahis variable should be the
      "variable=value . . ." portion of the 'sysctl -w ' command.
      If not set, the default value "kernel. panic_on_oops=l " will
      be used. Disable this feature by setting KDLJMP_SYSCTL=" "
      Example - also panic on oom:
           KDUMP_SYSCTL=" kernel. panic_on_oops=1 vm. panic_on_oom=1 "

USE KDUMP=1
#KDUMP_SYSCTL=" kernel. panic_on_oops=11'



# Kdump Kernel:
# KDUMP_KERNEL - A full             pathname to a kdump kernel.
# KDUMP_INITRD - A full             pathname to the kdump initrd   (if   used) .

KDUMP_KERNEL=/var/lib/ kdump/vmlinuz
KDUMP_INITRD=/var/lib/ kdump/initrd . img

KDUMP COREDIR&'/ var/crash"

//／이하 생략．.




커널이 덤프되는 파일은 /var/crash／에 저장됩니다．


위의 설정정보들은 kdum다con加 명령을 다음과 같이 실행하면 확인할 수 있습니다．



# which kdump-config
/usr／就泣n/kdump-config



# kdump- config show




커널연구회佃쌔쌔／.kerae나끄）                                                 정재준（rgb13307(＠陀te.com)
                                            164/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                          crash 도구 사용



DUMP_MODE:         kdump
USE KDUMP:         I
KDUMP_SYSCTL:      kernel. panic_on_oops=1
KDUMP COREDIR:     /var/crash
crashkernel addr: 0x30000000
   /var/lib/ kdump/vmlinuz: symbolic link to /boot/vmlinuz- 4.14.146+
kdump initrd:
   /var/lib/ kdump/initrd .1mg: symbolic link to /var/lib/ kdump/inltrd . img-
4.14. 146+
current state:     ready to kdump

kexec command:
  /sbln/ kexec -p --command-llne="BOOT_IMAGE=/boot/vmlinuz- 4.14.146+
root=UUID=c84184e1- 7b11- 4cd4- a272- 2450565ff912 ro quiet splash
Vt. handoff=1 nr_cpus=1 systemd. unit=kdump- tools . service irqpoll nousb
ata_piix. prefer_ms_hyperv=O " - -inltrd= /var/llb/ kdump/lnltrd .1mg
/var/lib/ kdump/vmlinuz




커널 덤프 동작은 다음과 같이 커널이 부팅될때 실행되는 명령라인 옵션에서 확인 가능합니다．



# cat /proc/cmdline

BOOT IMAGE=/boot/vmlinuz- 4.14.146+ root=UUID=c84184e1- 7b11- 4cd4- a272-
2450565ff912 ro quiet splash crashkerne1=384M- :128M vt. handoff=l




커널이 부팅될때1crashkernel 로 설정되는 메모리는 다음과 같이 확인할 수 있습니다．



# dmesg I grep -i crash

[    0. 000000] Reserving 128MB of memory at 768MB for crashkernel (System
RAM: 8064MB)




그리고 /etc/defauIt/kexec 의 파일 내용이 다음과 같이 설정되어 있는지 확인합니다．




 커널연구회佃쌔1사，kerneLbz)                                     정재준（I야13307（孕nate.com)
                                   165/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                          crash 도구 사용



# cat /etc/ default/kexec



# Defaults for kexec initscript
# sourced by /etc/init. d/ kexec and /etc/init. d/kexec-load

# Load a kexec kernel (true/ false)
LOAD KEXEC=t rue

# Kernel and initrd image
KERNEL IMAGE=!l/vmlinuzh
INITRD="/ initrd. img"

# If empty, use current /proc/cmdline
APPEND= 'T '

# Load the default kernel from grub config (true/ false)
USE GRUB CONFIG=t rue




커널 덤프를 실행하게 되면 시스템이 재부팅 되기 때문에 중요한 데이터들은 사전에 저장하는 것이

좋습니다. 커널 덤프는 아래 파일의 내용이 0 이상이 되어야 가능합니다．



# cat /proc/sys/kernel/sysrq
176



# cat /etc/ sysctl . d/le- magic- sysrq . conf



# The magic SysRq key enables certain keyboard combinations to be
# interpreted by the kernel to help with debugging. The kernel will
respond
# to these keys regardless of the current running applications
#
# In general, the magic SysRq key is not needed for the average Ubuntu
# system, and having it enabled by default can lead to security issues on
# the console such as being able to dump memory or to kill arbitrary
# processes including the running screen lock.
#
# Here is the list of possible values:




커널연구회佃쌔,w.kerne比z)                                     정재준（rgb13307@nate.con分
                                     166/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                        crash 도구 사용




                 ###############
    0
      - disable sysrq completely
    al
      - enable all functions of sysrq
   >1 - enable certain functions by adding up the following values:
           2   enable control of console logging level

            48
               enable control of keyboard (SAK, unraw)
             - enable debugging dumps of processes etc.
          16   enable sync command
          32   enable remount read- only
          64 - enable signalling of processes (term, kill, oom- kill)
         128   allow reboot/poweroff
         256   allow nicing of all RI tasks

    For example, to enable both control of console logging level and
    debugging dumps of processes: kernel. sysrq = 10

kernel. sysrq = 176




/proc/ sys/ kernel/ sysrq는 다음과 같은 명령으로 변경할 수 있습니다．


# sysctl -w kernel. sysrq=1




이제 다음과 같이 커널을 덤프할 수 있습니다.（필자는 아래의 명령이 실행은 되지만. 커널이 잘

덤프되지 않았습니다. 덤프되고 시스템이 재부팅 되어야 하는데. 그냥 다운 되었습니다. 커널 설정을

좀더 확인해야 겠습니다.)




# echo 1 > /proc/sys/kernel/ sysrq

# echo c > /proc/sysrq- trigger    (C身比弘사 州卉略）



채부멓卒 덤프파얹로 싶헝
# crash [namelist] [dumpfile]




 커널연구회佃쌔,w.kernel.bz)                                 정재준（四b1330기孕nate.com)
                                   167/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                          crash 도구 사용




crash 명령어

필자가 crash 을 설치하고 실행해 보니 니ye 로는 잘 동작합니다. 다음과 같이 crash 을 니ye 로

실행하여 명령어들을 정리하도록 하겠습니다．



crash 싶행 仕加a)
 # crash /lib/ modules/4.14. 146+/build/vmlinux

 crash 7. 2.1
 Coovriaht (C) 2002- 2017 Red Hat, Inc.
1Copyright (C) 2004, 2005, 2006, 2010 IBM Corporation
 Copyright (C) 1999- 2006 Hewlett-Packard Co
 Copyright (C) 2005, 2006, 2011, 2012 Fujitsu Limited
 Copyright (C) 2006, 2007 VA Linux Systems Japan K. K.
 Copyright (C) 2005, 2011 NEC Corporation
 Copyright (C) 1999, 2002, 2007 Silicon Graphics, Inc.
 Copyright (C) 1999, 2000, 2001, 2002 Mission Critical Linux, Inc.
 This program is free software, covered by the GNU General Public License,
 and you are welcome to change it and/or distribute copies of it under
 certain conditions. Enter "help copying" to see the conditions.
 This oroaram has absolutely no warranty. Enter "helo warranty" for
 aet ails.

GNU gdb (GDB) 7. 6
Copyright (C) 2013 Free Software Foundation, Inc.
License GPLv3+ : GNU GPL version 3 or later
<http : //gnu . org/licenses/gpl. html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law. Type "show copying"
and "show warranty" for details.
This GDB was configured as "x86_64- unknown-linux- gnu". . .

WARNING: kernel relocated [934MB] : patching 98170 gdb minimal_symbol
values

      KERNEL: /lib/ modules/4 .14. 146+/build/ vmlinux
    DUMPFILE: /dev/mem
        CPUS: 4
        DATE: Sat Oct 12 09: 36: 40 2019




 커널연구회（www.kernet．뇨）                                     정재준（rgb13307（孕nate.com)
                                  168/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                             crash 도구 사용



      UPTIME: 00:13: 26
LOAD AVERAGE: 1. 49, 0. 93, 0. 53
       TASKS: 756
    NODENAME: HP7100U
       RELEASE: 4.14.146+
       VERSION: #1 SMP Fri. Oct 4 22: 04:13 KST 2019
       MACHINE: x86_64 (2400 Mhz)
        MEMORY: 7. 9 GB
           PID: 2703
       COMMAND: "crash"
          TASK: ffff99c67091ae80 [THREAD_INFO: ffff99c67091ae80]
           CPU: 2
         STATE: TASK_RUNNING (ACTIVE)

crash>




crash 명령어들은 crash 가 실행된 프롬프트에서 다음과 h이P 을 입력하면 명령에 목록들이

나타납니다．



cra尉L형령아도·
 crash> help
出
                  files         mach           repeat         timer
alias             foreach       mod            runq           tree
ascii             fuser         mount          search         union
bt                gdb           net            set            vm
bt이：)             help          p              sig            vtop
dev               ipcs          PS             Struct         waitq
dis               irq           pte            swap           whatis
eval              kmem          ptob           sym            wr
exit              list          ptov           sys            q
extend            log           rd             task

crash version: 7. 2. 1  gdb version: 7. 6
For help on any command above, enter "help <command>".
For help on input options, enter "help input ".
For help on output options, enter "help output ".




    커널연구회（낚쌔,w.kerne比z)                                 정재준（rgb13307＠陀te.com)
                                    169/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                              crash 도구 사용



이제 위의 명령어들을 하나씩 익혀 가도록 하겠습니다．



backtrace 명령

먼저 backtrace 부터 설명합니다. backtrace 는 커널안에서 명령들이 실행된 흐름（execut向n

history stack）을 추적할 수 있습니다. 다음과 같이 도움말부터 확인합니다．


Backtrace 도욤말
crash> help bt

NAME
  bt - backtrace

SYNOPSIS
  bt [-al- c cpu(s) I- gI- r 1- tI- TI-l1- el-EI- fI- FI- oI-OI- v] [-R ref] [-s [-xl
d] ]
     [-I ip] [-S sp] [pid I task]

DESCRIPTION
  Display a kernel stack backtrace. If no arguments are given, the stack
  trace of the current context will be displayed.



//／이하 생략．.




bt 명령 다음에 전달하는 파라미터 종류들이 상당히 많습니다. 파라미터들에 대해서는 도움말을

확인하며 익혀가면 되겠습니다. 파라미터 없이 bt 명령만 실행하면 다음과 같이 현재 실행된 프로세스

정보를 출력합니다．


crash> bt
PID: 2703    TASK: ffff99c67091ae80       CPU: 3    COMMAND: "crash"
(active)




커널연구회佃m쌔／.kernet.b라                                          졍재준（rgbi3307@nate.com)
                                     170/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                         crash 도구 사용




현재 실행된 프로세스 번호們D）와 이 태스크가 위치하고 있는 메모리 주소（fff円9c6709］昶80）와

실행하고 있는 CPU 번호 (3）와 명령（프로세스）명칭이 나타납니다．



"bt-t" 으로 실행하면 현재 실행된 태스크의 스택정보와 text 심볼들 보여 줍니다．



crash> bt -t

PID: 2703     TASK: ffff99c67091ae80 CPU: 3        COMMAND: "crash"
                 START:    schedule at ffffffffbbf397ff
  [ffffb6c442c43e70] security_file_ permission at ffffffffbb9a9dOl
  [ffffb6c442c43e98] rw_verify_area at ffffffffbb85fa6e
  [ffffb6c442c43eb8] vfs_read at ffffffffbb860dee
  [ffffb6c442c43ef0] sys_read at ffffffffbb861359
  [ffffb6c442c43ef8j sys_lseek at ffffffffbb85f84a
  [ffffb6c442c43f30] do_syscall_64 at ffffffffbb603a13
  [ffffb6c442c43f50] entry_SYSCALL_64_after_hwframe at ffffffffbc000081
     RIP: 00007eff02f07081 RSP: 00007ffc9c626808 RFLAGS: 00000246
     RAX: ffffffffffffffda     RBX: 00000002309cf 000 RCX: 00007eff02f07081
    RDX: 0000000000001000 RSI:    0000560edc931c20   RDI:   0000000000000004
    RBP: 0000000000000002   RB:   00000002309cf000    R9:   0000560edbe01710
    RiO: 00007eff044176c0 Rul:    0000000000000246   R12:   0000000000001000
    R13: 0000000000000004 R14:    0000560edc931c20   R15:   ffffb6c442c43000
    ORIG RAX: 0000000000000000    CS: 0033 SS: 002b




"bt 干"옵션으로 뒤에 프로세스 번호를 전달하면 해당 프로세스의 스택과 심볼정보들을 확인할 수

있습니다. 이때 프로세스 번호는 다음과같이 " PS" 명령으로 확인할수 있습니다．




 커널연구회（＼사니쌔／.kerne나）라                                   정재준（r야)13307@nate.com)
                                  171 /351
                                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                                      crash 도구 사용




小 명령

먼저 다음과 같이 도움말부터 확인합니다．



crash> help PS

NAME
    PS - display process status information

SYNOPSIS
  PS [-kl- ul- GI- y policy] [-s] [-pl- cl- tl- [llm] [-C cpu] I- aI- g 1- r 1-S]
     [pid I task I command]

DESCRIPTION
  This command displays process status for selected, or all, processes
  in the System. If no arguments are entered, the process data is
  is displayed for all processes. Specific processes may be selected
  by using the following identifier formats:

//／이하 생략．.




".ps求" 옵션으로 실행하면 커널 프로세스（태스크，쓰레드）리스트가 출력됩니다． 乍Sr七“ 옵션으로

실행하면 유저 프로세스 리스트가 출력됩니다．



커넘 프로섀스 확인
crash> ps -k



    PID               PPID           CPU                 TASK       ST   %MEM    VSZ           RSS       COMM




          00 00 2 4      00 00 0 2    0l23 e 0                                     00 00 0 e
>                                                ffffffffbca13480   RU    0. 0                   0       [swapper/0]
>                                                ffff99c6a4e89740   RU    0.0                    0       [swapper/i]
                                                 ffff99c6a4e8c5c0   RU    0. 0                   0       [Swapper/2]


                                                                                                 0 0 0
>                                                ffff99c6a4e8dd00   RU    0. 0                           [swapper/3]
                                                 ffff99c6a52b1740   IN    0. 0                           [kthreadd]
                                                 ffff99c6a52b5d00   UN    0. 0




커널연구회佃쌔,w.kerne나）z)                                                               청쟤준（rgbi3307@nate.con力
                                                            172/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                          crash 도구 사용



     [kworker/O : OH]
           6        2    0   ffff99c6a52c9740   UN    0. 0         0      0
     [mm_percpu_wq]
           7        2   0    ffff99c6a52cc5c0   IN    0. 0         0      0    [ksoftirqd!
01
           8       2    3    ffff99c6a52cdd00   UN    0. 0        0       0    [rcu_sched]
           9       2    0    ffff99c6a52c8000   UN    0. 0        0       0    [rcu_bh]
          10       2    0    ffff99c6a52cae80   IN    0. 0        0       0    [migration!
0]
     11      2          0    ffff99c6a4e8ae80   IN    0. 0        0       0
[watchdog/0]
     12      2          0    ffff99c6a4e88000   IN    0. 0        0       0    [cpuhp/O]
     13      2          1    ffff99c6a4e31740   IN    0. 0        0       0    [cpuhp!1]

//／이하 생략． .




crash> ps -u



        PID     PPID    CPU       TASK          ST   %MEM        VSZ    RSS    COMM
           1       0     0 ffff99c6a52b2e80     IN    0.1     225588    9484   systemd
         256       1     0 ffff99c65f362e80     IN    0. 4    119428   35828   systemd-
     journal
     3（沼     1          0    ffff99c6a48d9740   IN    0.1      47980    6532   systemd-
udevd
     776     1          1    ffff99c66012c5c0   IN    0.1      71840    6004   systemd-
network
     830     1           3   ffff99c6a197ae80   IN    0.1     146108    5700   systemd-
tirnesyn
     832     1          1    ffff99c6a1979740   IN    0.1      70884    6276   systemd-
resolve
     836     1           2   ffff99c69f8e9740   IN    0.1     188604   10044   thermald
     842     1           1   ffff99c6a197dd00   IN    0.1     503768   12244   udisksd
     844     1           1   ffff99c660121740   IN    0.1     108972    8084   cupsd
     847     1           2   ffff99c6a32bae80   IN    0.1      70732    6156   systemd-
logind
      848    1           0   ffff99c6a1b39740   IN    0.1     427260    9356
卜伯demManager
      849    1           1   ffff99c6a1b3ae80   IN    0.1      51816    6260   dbus- daemon




     커널연구회佃쌔시／.kerne나끄）                                            정재준（I야)13307匣｝nate.com)
                                         173/ 351
                                                     리눅스 커널 소스 해설 E기초입문］
                                                              crash 도구 사용



    852       1   3   ffff99c6a0899740   IN   0. 2    567452   17816
NetworkManager
    853       1   1   ffff99c6a089c5c0   IN   0.1      45008    7996
wpa－山supplicant
    855       1   0   ffff99c6a0898000   IN   0. 0     47276    3752   avahi-
daemon
     857      1   1   ffff99c660128000   IN   0. 0    110476    3584 irqbalance

/／이하 생략．.




struct 명령

crash 에 있는 struct 명령을 사용하여 커널 구조체들의 구조와 그 안의 값들을 확인할 수 있습니다．

커널 소스 분석은 구조체들의 구조를 이해하고 데이터 값들을 확인하는 과정의 연속이므로 struct

명령을 잘 활용하면 커널 소스를 좀더 쉽게 분석할 수 있습니다. struct 명령을 사용하는 방법은

다음과 같이 도움말을 통해서 확인할 수 있습니다．


struct 명령 도욤팜
crash> help struct

NAME
  struct - structure contents

SYN아）S's
  struct struct_name{ .member[ ,member] ][-o] [-1 offset] [-rfuxdp]
         [address I symbol] [:cpuspec] [count I -c count]




struct 명령 다음에 구조체명과 여러가지 옵션을 추가하여 실행합니다. 먼저, 커널 스케쥴러에서

중요한 역할을 하고 있는 task struct 구조체 정보를 다음과 같이 확인 합니다．



커널연구회（www.kerne나끄）                                        정쟤준（rgbi3307（흐）aate.com)
                                  174/ 351
                                             리눅스 커널 소스 해설 ［기초입문］
                                                      crash 도구 사용




crash> struct task struct

struct task_struct {
    struct thread_info thread_info;
    volatile long state;
    void *stack;
    atomic_t usage;
    unsigned mnt flags;
    unsigned mnt ptrace;
    struct llist_ node wake_entry;
    mnt on_cpu;
    unsigned mnt cpu;
    unsigned mnt wakee_flips;
    unsigned long wakee_flip_ decay_ts;
    struct task_struct *last1mwakee;
    mnt wake_cpu;
    mnt on_rq;
    mnt prio;
    mnt static_prio;
    mnt normal_prio;
    unsigned mnt rt_priority;
    const struct sched_class *sched class;
    struct sched_entity se;
    struct sched_rt_entity rt;
    struct task_group *sched1task1group;
    struct sched_dl_entity dl;
    struct hlist_ head preempt_notifiers;
    unsigned mnt btrace_seq;
    unsigned mnt policy;
/／이하 생략．

}


다음과 같이 ,0 옵션을 추가하여 실행하면 구조체 멤버 변수들의 오프셋이 같이 출력 됩니다·




    커널연구회（www.kerne나파                             정재준（rgbi330？會nate.com)
                                175/ 351
                                               리눅스 커널 소스 해설 E카菱입푼｝
                                                        crash 도구 사용



crash> struct task struct -o

 struct task_struct {
       [0] struct thread_info thread_info;
      [16] volatile long state;
      [24] void *stack;
      [32] atomic_t usage;
      [36] unsigned mnt flags;
      [40] unsigned mnt ptrace;
      [48] struct luist_ node wake_entry;
      [56] mnt on_cpu;
      [60] unsigned mnt cpu;
      [64] unsigned mnt wakee_flips;
      [72] unsigned long wakee_flip_ decay_ts;
      [80] struct task_struct *last1wakee;
      [88] mnt wake_cpu;
      [92] mnt on_rq;
      [96] mnt prio;
    [100] mnt static_prio;
    [104] mnt normal_prio;
    [108] unsigned mnt rt_ priority;
    [112] const struct sched_class *schedHclass;
    [128] struct sched_entity Se;
    [576] struct sched_rt_ entity rt;
    [624] struct task_group *sched= taskegroup;
    [632] struct sched_di_entity dl;
    [864] struct hlist_ head preempt_notifiers;
    [872] unsigned mnt btrace_seq;
    [876] unsigned mnt policy;
/／이하 생략．.

}




커널연구회（www.kerneLbz)                                정쟤준（四bi3孰玎會nate.com)
                                176/ 351
                                                 리눅스 커널 소스 해설 ［기초입푼］
                                                          crash 도구 사용



ta引（[ 명령

task 명령은 task1就ruct 구조체와 thread_info 구조체 안의 내용（멤버 변수값）들을 출력합니다．

실행 문법과 옵션들은 다음과 같이 도움말을 통해서 확인할 수 있습니다．


crash> help task

NAME
  task - task struct and thread info contents

SYNOPSIS
  task [-R member[ ,memberj] [-dx] [pid I taskp]




먼저, 아무런 옵션 없이 task 명령을 실행하면 다음과 같이 현재 실행되고 있는 프로세스의

task struct 내용이 출력됩니다． 현재 실행되고 있는 프로세스명은 " crash"이고 미D 는 3354,

메모리 주소는 ffffa02335429740 이고 Cpu 번호는 2 입니다．


crash> task


PID: 3354   TASK: ffffa0233542974크   CPU: 2     COMMAND: 'Tcrash"
struct task_struct {
  thread_info = {
    flags = 2147483648,
    status = 0
  }r
  state = 0,
  stack = OxffffafE旭coe（加1E）이가
  usage = {
    counter = 2
   }   r

   flags = 4194560,
   ptrace = 0,
   wake_entry = {




 커널연구회（＼사甘쌔／.kerne나）力                                   정재준奴羚沼307回n就e.com)
                                 177/ 351
                                                리눅스 커널 소스 해설 [71초입문I
                                                         crash 도구 사용



           next = OxO
  }    r

  on_cpu = 1,
  Cpu = 2,
  wakee_flips = 4,
  wakee_flip_ decay_ts = 4296894344,
  last_wakee = 0xffffa02161ab2e80,
  wake_cpu = 2,
  on_rq = 1,
  prio = 129,
  static_prio = 120,
  normal_prio = 120,
  rt_priority = 0,
  sched_class = 0xffffffff90827b60,
/／이하 생략．.




task 을 실행할따1-x 옵션을 주면 데이터들이 16 진수로 출력됩니다. 그리고 프로세스 번호를 주면

해당 프로세스의 task_struct 내용을 출력합니다．



crash> task -x 2460

PID: 2460   TASK: ffffa0234382c5c0     CPU: 1   COMMAND: "bash"
struct task_struct {
  thread_info = {
    flags = 0x0,
    status = OxO
  }    ,

 state = Oxi,
 stack = 0xffffaf0ec29a4000,
 usage = {
   counter = 0x2
  }r
 flags = 0x400000,
 ptrace = OxO,
 wake_entry = f
    next = OxO




커널연구회（的胛，kerneLbz)                                     청쟤준（呼卦3307會n航色corn)
                                178/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                         crash 도구 사용



 }r
 on_cpu = E) xO,
 Cpu = Oxi,
 wakee_flips = 0x3,
 wakee_flip_ decay_ts = 0xffffb250,
 last_wakee = 0xffffa0232213dd00,
 wake_cpu = Oxi,
 on_rq = OxO,
 prio = 0x78,
 static_prio = 0x78,
 normal_prio = 0x78,
 rt_ priorlty = OxO,
 sched_class = 0xffffffff90827b60,
/／이하 생략． .




vn）명령

vm 명령은 커널의 가상메모리 정보를 출력합니다．



crash> help vm



NAME
  vm - virtual memory

SYNOPSIS
  vm ［나） I -P vma I 小'1 mm I -v   1 -m I -x I -d I [-R reference] [pid I
task] ]
        -f vm_flags]




 커널연구회（납쌔,w.kerne나玹）                                   정재준(rgb13307（孕配te.com)
                                   179/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                       crash 도구 사용



VII) 을 실행할때 -II) 옵션을 주고 프로세스 번호를 추가하면 해당하는 프로세스의mrn就ruct 구초처F

내용이 출력됩니다．




crash> vm -m 2460



PID: 2460   TASK: ffffa0234382c5c0   CPU: 1   COMMAND: "bash"
struct mm_struct {
  mmap = 0xffffa023494a6578,
  mm_rb = {
    rb_node = 0xffffa023494a68b8
   }r
  vmacache_seqnum = 16,
  get_unmapped_area = 0xffffffff8fa31bd0,
  mmap_base = 140603912511488,
  mmap_legacy_base = 47028882657280,
  mmap_compat_base = 4160425984,
  mmap_compat_legacy_base = 1431969792,
  task_size = 140737488351232,
  highest_vm_end = 140722585489408,
  pgd = 0xffffa02343a90000,
  mm_users = {
    counter = 1
   }r
  mm count = {
    counter = 1
  }r
  nr나：比es = {
    counter = 20
  }r
 nr_pmds = {
   counter = 3
  }     r

 map_count = 46,




커널연구회（硏／w＼六／.kerneLbz)                               정쟤준(rgbi3307會nat色corn)
                                180/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                           crash 도구 사용



kmen) 명령

kmen) 명령을 사용하여 커널 메모리 내용들을 확인할 수 있습니다. 커널이 관리하는 메모리 내용이

많은 만큼 옵션들도 상당히 많습니다. 옵션들에 대해서는 아래와 같이 도움말을 통해서 확인

가능합니다．


crash> help kmem


NAME
  kmem - kernel memory

SYNOPSIS
  kmem [-fl 나二I-cl- CI-il- vl- VI-nl- zl- ol- h] [나） 1 -mmember[ ,member] ]
       [[-sl- S] [slab] [-I slab[ ,slab] ]] [-g [flags] ] [[-P] address] ]




먼저 -i 옵션을 주어 실행하면 메모리 사용 정보를 요약하여 보여 줍니다．


crash> kmem -i


                   PAGES        TOTAL       PERCENTAGE
    TOTAL MEM    1976891       7. 5 GB
          FREE   105980        414 MB     5% of TOTAL MEM
          USED   1870911       7.1 GB    94% of TOTAL MEM
       SHARED     711547       2. 7 GB   35% of TOTAL MEM
      BUFFERS     379765       1. 4 GB   19% of TOTAL MEM
       CACHED     703940       2. 7 GB   35% of TOTAL MEM
         SLAB     154778     604. 6 MB    7% of TOTAL MEM

   TOTAL HUGE          0             0
    HUGE FREE          0             0     0% of TOTAL HUGE


   TOTAL SWAP     524287          2 GB
    S닙AP USED          0             0     0% of TOTAL SWAP




 커널연구회佃w小／.kerneL比）                                       정재준（rgbi3307@nate.com)
                                   181 /351
                                                         리눅스 커널 소스 해설 E기초입문］
                                                                  crash 도구 사용



    SWAP FREE     524287              2 GB    100% of TOTAL SWAP

 COMMIT LIMIT    1512732            5. 8 GB
    COMMITTED    1785324            6. 8 GB   118% of TOTAL LIMIT




kmen) 옵션에 주소를 주면 해당 하는 주소의 정보들을 다음과 같이 출력합니다．


crash> kmem ffffa02139048000


CACHE            NAME                          OBJSIZE   ALLOCATED        TOTAL   SLABS
SSIZE
ffffa02366017e00 task struct                      5952          726         770    154
32k
  SLAB                   MEMORY               NODE   TOTAL    ALLOCATED   FREE
  ffffd4e700e41200       ffffa02139048000        0        5           1       4
  FREE I   [ALLOCATED]
  [ffffa02139048000]

    PID: 4966
COMMAND: "crash"
   TASK: ffffa02139048000         [THREAD_INFO: ffffa02139048000]
    CPU: 1
  STATE: TASK_RUNNING (ACTIVE)

       PAGE       PHYSICAL             MAPPING         INDEX CNT FLAGS
ffffd4e700e41200 39048000                         0 ffffa02139049740 I
fffffc0008100 slab, head




커널연구회佃八阿硝／.kernet,虹）                                          졍채준（rgbi3孰玎會flat已corn)
                                      182/ 351
                                               라눅스 커널 소스 해설 ［기초입문］
                                                        crash 도구 사용




syn) 명령

syn) 명령은 커널의 심볼 정보들을 출력합니다．



crash> help sym



NAME
  sym - translate a symbol to its virtual address, or vice- versa

SYNOPSIS
  sym [-1] I [-M] I [-m module] I [-p1- n] I [-q string] I [symbol I vaddr]




-[ 옵션을 주면 전체 심볼 정보를 출력합니다. -q 옵션으로 원하는 심볼을 검색할 수 있습니다．



crash> sym -l



0 (D) __per_cpu_start
0 (D) irq_stack_union
4000 (0) cpu_debug_store
5000 (D) cpu_tss_rw
8000 (D) gdt_page
9000 (d) exception_stacks
e000 (d) entry_stack_storage
f000 (D) espfix_waddr
f008 (D) espfix_stack
fob(9 (D) cpu_llc_ id
f020 (0) cpu_llc_ shared_map
f028 (0) cpu_core_map
f030 (D) cpu_sibling_map
f040 (D) cpu_info
f130 (D) cpu_number
f138 (0) this_cpu_off
 f140 (0) x86_cpu_to_acpiid
 f144 (0) x86_cpu_to_apicid
 f146 (0) x86_bios_cpu_apicid
 f148 (0) sched_core_priority




 커널연구회（뻐사小／.kern이,b라                                  정채준(rgb13307暳）nate.com
                                 183/ 351
                                                  리눅스 커널 소스 해설 E기姦입문I
                                                           crash 도구 사용


f 180 (d) cpu_loops_per_jiffy
fla크 (d) pmc_prev_left
f3a0 (D) cpu_hw_events
/／이하 생략．.




p명령

p 명령은 print 역할을 합니다. 심볼이나 표현문구의 데이터를 출력합니다．


crash> help p

NAME
  p    print the value of an expression

SYNOPSIS
  p [-xl- d] [-u] [expression I symbol[ :cpuspec] ]




커널의卜ffies 전역 변수（심볼）내용을 다음과 같이 출력할 수 있습니다．


crash> p jiffies

jiffies = $3 = 4297859191




in止 mm 구조체의 내용을 다음과 같이 출력합니다．


crash> p mnit_mm

mnit_mm = $4 = {




커널연구회如쌔째／.kerne나功                                     청채준(rgbi3307（孕nate.com)
                                  184/ 351
                                           리눅스 커널 소스 해설 ［기초입문］
                                                    crash 도구 사용



 mmap = OxO,
 mm_rb = {
   rb node = OxO
 }    .

 vmacache_seqnum = 0,
 get_unmapped_area = OxO,
 mmap_base = 0,
 mmap_legacy_base = 0,
 mmap_compat_base = 0,
 mmap_compat_legacy_base = 0,
 task_size = 0,
 highest_vm_end = 0,
 pgd = oxffffffffgOeOa000,
 mm_users = {
   counter = 2
 }r
 mm count = {
   counter   =2
 }    r

 nr_ptes     {
   counter   =   0
 }r
 nr_pmds = {
   counter = 2
 }    r

 map_count = 0,
/／이하 생략．




커널연구회（낚／砥／琪,.kerne나파                           정재준(rgbi3307每nate.com)
                                185/ 351
                                                리눅스 커널 소스 해설 ［카초입문］
                                                         crash 도구 사용




list명령

List 명령은 커널의 링크드 리스트 정보를 출력합니다．



crash> help list

NAME
  list     - linked list

SYN아＞S's
  list [[-0] offset] [-e end] [-[siS] struct[ .member[ ,member] [-1 offset] ] -
[xld] ]
        [-ri- hi- H] start




tree 명령

tree 명령은 커널의 트리 자료구조 정보를 출력합니다．



crash> help tree

NAME
  tree - display radix tree or red-black tree


"' 쁜：: '二 [radi，나.tre이 [-. 針， 叫 I:-［이司 struct[ .member[ ,member] ] -[이
d]    ]
              [-o offset] [-p] [-N] start




     커녈연구회C'차璘쌔／.keraeLb卦                               정쟤준（呼升3307會nat鼠corn)
                                    186/ 351
                                                 리눅스 커널 소스 趨설 ［기麥입문］
                                                          crash 도구 사용



foreach 명령

foreach 명령을 사용하면 여러가지 명령이 반복 실행된 결과 데이터들을 확인할 수 있습니다．



crash> help foreach



NAME
  foreach - display command data for multiple tasks in the system

SYNOPSIS
  foreach [[pid I taskp I name I state I [kernel I user] ] . . . ]
          command [flag] [argument]




 커널연구회（蜘쌔／.kerne나파                                      청채준(rgb13307簪nate.com)
                                   187/ 351
                                                          리눅스 커널 소스 해설 1기초입문］
                                                                    kprobes 이해




kprobes 이해

                                         이번글의 주제는 "리눅스커널 Kpr야)es이해" 입니다． 소스

       小     六，
                                         해설과 실습을 병행하여 설명하도록 하겠습니다. 이글을
           Kernel kprobes
                                         작성하는 시점에서 최신 리눅스 커널 버전은 " v4.20.4"입니다．
                  \4           "   " "




                                         이 소스를 기준으로 설명하도록 하겠습니다. 그러나 커널

                                         Kprobe 는 2002 년도부터 소스에 추가 되었기 때문에 " v2.6"

이상 부터는 잘 동작할 듯 합니 다．


Kprobes 에 대해서는 커널 문서 " Documentat幻n/kprobes.txt" 파일에 잘 설명되어 있습니다．

Kpr야)eS 에 대한 전반적인 내용은 이 문서를 참고하여 설명하도록 하겠습니다. 이 문서의 앞부분을

보면 다음과 같은 순으로 Kpr야氾S을 설명하고 있습니다. 커널 문서들 중에서도 상당히 잘 정리되어

있습니다. 리눅스 커널 소스를 분석할때도 다음과 같은 절차로 진행하는 것도 효율적인 방법이

되겠습니다． Kprobes 1H념, 아키텍쳐 호환（의존성）, 환경설정. AF기 함수 참조, Kprobes 특징과

한계성. Probe오버헤드, 실행방법, Kprobes 0卦제, Kretprobes예제, 사라진 요소들. kprobes

debugFs 인터페이스, k마obes sysctL 인터페이스 순으로 설명하고 있습니다．


r沁cumentation/kpr的心上x 섶명 순서

  .'       1. Concepts: Kprobes, and Return Probes
  v        2. Architectures Supported
  v        3. Configuring Kprobes
  .'       4. API Reference
  v        S. Kprobes Features and Limitations
  .'       6. Probe Overhead
  b'       7. TODO




커녈연구회（叭쌔w.kerneLbz)                                             정쟤준（rgb沼30了簪na始,corn)
                                             188/ 351
                                                      라눅스 커널 소스 翊설 {7！塞합푼]
                                                                kprobes 이해



   v   8. Kprobes Example
  1'   9. Kretprobes Example
   '   10. Deprecated Features
  1'   Appendix A: The kprobes debugfs interface
  v    Appendix B: The kprobes sysctl interface




먼저 커널 Kprobes 711념입니다. Kprobes 는 커널 루틴에 동적인 break 을 삽입하여 디버그와

성능정보를 수집합니다. 분석하고 싶은 커널 코드 주소에 trap 을 삽입하여 breakp이nt 에 도달하면

처리（handler) 함수가 동작합니다. Kprobes 는 kprobes 와 kretprobes(return probes）두7벼

종류가 있습니다. kprobes는 어떠한 커널 코드에도 삽입할 수 있고, kretprobes는 특정 함수가

리턴될따1 동작합니다. 지금까지 내용을 좀더 쉽게 요약하면, Kprobes는 커널 코드를 디버깅하는

용도로 만들어진 것입니다. 특정 커널 코드가 실행되는 위치（심볼, 함수）에서 여러가지 정보（명령주소，

레지스터값, 스택정보, 데이터값, 실행시간）들을 확인할수 있습니다. 저도 사용해본 결과, 커널

소스를 분석하고 디버깅하는 용도로 아주 적합합니다.


그럼 Kprobes 를 실행하기 위해서 점검해야 하는 사항들을 정리해 보겠습니다. 우선 Kprobes 는

다음과 같은 아키텍쳐（CPU）에서 동작합니다．


Kprobes 가 동작하는 아키텍쳐（CPU) 종류

   1 1386 (Supports jump optimization)
   1 x86_64 (AMD-64, EM64T) (Supports jump optimization)
   1 ppc64
   1 ia64 (Does not support probes on instruction sloti.)
   1 sparc64 (Return probes not yet implemented.)
   1 arm
   1 ppc




 커널연구회（甘朴사璘／.kernel, 뇨）                                     정재준佃羚好30？簪nate.com)
                                       189/ 351
                                                        리눅스 커널 소스 해설 E기초입푼］
                                                                  kprobes 이해



    1   mips
    1   s390




저는 x86_64 에서 동작을 확인했고 이것을 기준으로 설명을 이어 가겠습니다． 그리고 커널 소스를

빌드할따1 다음과 같은 설정 상수가 Enable 되어 있어야 합니다．



Kprobes 율 위한 커널 섶정 샹수들

CONFIG_KPROBES [=y}
CONFIG_MODULES [=y]
CONFIG_MODULE_UNLOAD [=y]
CONFIG_KALLSYMS [=y]
CONFIG_KALLSYMS_ALL [=y]
CONFIG_DEBUG_INFO [=y]




위와 같은 설정으로 커널이 준비 되었다면. 이제 Kprobes 를 실행하기 위한 API 함수들을 사용하여

커널 코드를 디버깅할 수 있습니다. 이 함수들은 대부분 " /kernel/kprobes.c" 소스 파일에 정의되어

있습니다. 다음부터 이 함수들을 정리해 보겠습니다. 먼저 kprobes을 사용하71 위한 커널 API

함수들을 정리 했습니다. 함수들의 용도는 주석문 형태로 설명을 달았습니다．



kprobes 윰 위한 A미 함수듈

荊nc山de <linux/kpr야）es.h> //kpr姚狩S홰더파일
荊nc山de <linux/ptrace.h>


k止 registe口kprobe(struct kpr야氾 士kp); /／如robes 듕록 함수
ii北p爬_hand(er(struct kpr야爬차기 struct pt_legs차egs); 月앞（들어가는 치점）에서 처라되는핸들러 함수
V이d post_han바er(struct kprobe 사）. struci pt_legs 火regs, unsigned Long flags); /／두K나가는 자점）
애，서 처리되는 핸들러 함수
II北fau比_handter(struct kpr야爬차）, struct pt_legs火legs, mnt trapnr); //오류를처라하는핼들러 함수




 커널연구회柶汭罔／.kernet,址）                                            정재준（rgb浮307管n就色corn)
                                       190/ 351
                                                         리눅스 커널 소스 해설 ［가초입문]
                                                                   kprobes 이해




다음으로 kretprobes 을 사용하기 위한 커널 API 함수들을 정리 했습니다. 함수들의 용도는 주석문

형태로 설명을 달았습니다．



kretprobes 율 위한 API 함수들

#include <Linux/kprobes.h>
#inc(ude <Iinux/ptrace.h>


mnt reg ister_kretprobe(struct kretprobe火rp); //kret아ob孕，S듕靄할4>
mnt kretprobe_handler(struct kretpr야）e_instance火ii, struct pt_legs火regs); /／打就町的e＄처라
핸繫러 함수




그리고 Kprobes 을 처리하는 기타 API 함수들은 다음과 같습니다．



Kprobes 동작을 가능하게 하는 API 함수들

荊nc山de <linux/kprobes.h>


mnt enable_kprobe(struct kprobe *kp);
int enabte_kretprobe(struct kretprobe *rp);




Kprobes 동작을 불가능하게 하는 API 함수들

#incLude <linux/kprobes.h>


mnt disabte_kprobe(struct kprobe *kp);
m t disabte_kretprobe(struct kretprobe *rp);




  커널연구회佃쌔iw,kerneLbz)                                             정채준（rgbi3307會nate.com)
                                              191 /351
                                                        리눅스 커널 소스 해설 E기초입문］
                                                                  kp robes 이해



Kprobes 툼록을 해제하는 A끼 함수

 倂nc山de <Linux/kpr的es.h>


 \／이d unreg毗아k마的e(struct kpr야）e 싸；p);
 void unregister_kretprobe(struct kretprobe *rp);




 지금까지 정리한 함수들은 모두 "/kerneL/kprobes.c" 커널 소스 파일에 정의되어 있습니다. 이제 이

 함수들을 사용하여 Kprobes 기능을 실습해 보도록 하겠습니다. 실습용 예제 소스 파일도 커널에

 있습니다． kprobes용실습예제는 " sam이es/kprobes/k마obe_exam이e.c" 소스파일을보면

 됩니다. 커널 모듈 프로그래밍되어 있는 소스여서 모듈로 빌드하여 실행할 수 있습니다. 그리고

 kretprobes용실습예제는 " sam이es/kprobes/kretprobe_exampLe.c" 소스파일을보면 됩니다.


 또한，아래 링크에서 K아obes 을 위한 추가적인 정보들을 확인할 수 있습니다．


 Kprobes 인터넷 챰고 자료

 h比p:／加ww기 06.ibm.com/devetoperworks／的rary／나甘的es.htmL?ca=dgr如xw42K아的e
 http://www.redhat.com/magazine/o05mar05/features/kprobes/
 h比p://ww세sers.cs.umn.edu／比outcher/k마的es/
 http://www.linuxsymposium.org/2006/(inuxsymposium_procv2.pdf (pages 101-115)




Kprobes는 "/sys/kernel/debug/kprobes/" 리눅스 파일 경로에 있는 파일들을 통하써 사용자가

，접근할 수 인터페이스를 제공합니다．


:/sys/kerne[/debug/kpr야)es/LiSt" 파일은 kprobes 을 위해서 등록한 커널 코드의 심볼

리스트입니다．




 커널연구회（www.kerneLb卦                                             정좨준似獅3307會nate.com)
                                           192/ 351
                                                                 리눅스 커널 소스 簿藝, ｛카초잎整］
                                                                           kprobes 이해



"/sys/kernel/debug/kprobes/enabled " 파일은 k마obes 기능을 Ena바e ON 혹은 미sable OFF

하는 용도로 사용합니다．


"/proc/sys/debug/kprobes-optimization" 파일은 kprobes 최적화를 ON/OFF 하는 용도로

사용합니다．


지금까지 Kprobes 에 대한 전반적인 내용들을 설명했습니다 ．이제부터는 커널 소스 경로 "sampies!

kprobes/ " 에 있는 예제 소스들을 직접 실습한 것을 설명 드리겠습니다．


"sam ples/kprobes/k아obe_exam이e.c" 소스를 보면 커널 모듈로 등록 되면서 kprobe_ini目）

함수가 다음과 같이 실행됩니다．


kprobe_init() 함수 소스

sta匕cint    in比 kprobe_init(v이d)
{
        mnt ret;
        kp.pre_handler = handler_pie; I/ k莎야羚S시작지졈에서 처리되는 핸들러 함수
        kp.post_handler = handler_post; f/kpr야爬S 끝나는 지점에서 처리되는 핸듈러 함수
        kp.Fauit_handler = handler_fault; i/ k江obes 오冪가 발생했욜따1 처리되는핸들러 함수


        ret = register_kprobe(&kp); //kprobes *록
        if (ret< O) {
                   pr_err("register_kprobe failed, returned %d\n", ret);
                   return ret;
        }
        pr_info("Planted kprobe at %p\n", kp.addr);
        return 0;
}




    커널연구회佃I'사w.kernel,比）                                                   청재준(rgb亘3307（孕nate.com)
                                               193/ 351
                                                              리눅스 커널 소스 해설 E까姦입문］
                                                                        kprobes 이해



registe乙印robe() 함수는 kp 구조체 주소를 매개변수로 받아서 kprobes 을 등록합니다． kp

구조체는 다음과 같이 정의 되어 있습니다. 여기서 symbo［의 의미가중요합니다. symbol은

kprobes 가 동작을 시작하는 커널 코드 심볼입니다. 즉, 디버깅을 시작하는 커널 소스에 있는

심볼입니댜. 가장 일반적인 심볼이 함수 명칭인데. 아래에서는 "edo fork"를 디폴트 심볼로

했습니다. 이러한 kp 구조체 정보로 kprobes 가 등록되면 커널이 실행되다가mdo fork함수가

실행되는 시작 지점에서 handler_마e() 핸들러 함수가 동작하고 끝나는 지점에서 handler_post()

함수가실행되고 이곳에서 디버깅 정보들이 " /var/log/sysLog" 파일에 출력됩니다. 따라서 사용자는

이 정보를 확인하며 커널을 디버깅할 수 있습니다.


kprobe$ 가 툼록뒬때 사용하는 kprobe 구조체1

#define MAX SYMBOL LEN 64
static char symbol[MAX_SYMBOL_LEN] = "_do_fork";
module_para m_string(symbol, symbol, sizeof(symboL), 0644);


／亥 For each pr야冶 的u need to 訓oc毓eak口robe s打ucture 卉
static struct kprobe kp = {
         .symboL_name = symbol,
};
다음으로 " sam이es/kprobes/kretpr야）e_exam이e.c" 소스는 커널 모듈로 등록 되면서

kretprobe_init() 함수가 다음과 같이 실행됩니다．


kretprob乞In北0 함수 소스

sta匕이nt 1쎄t kre中robe_i毗佃이d)
{
         m)t ret;




     커널연구회（ww城kerneLbz)                                           청쟤준（rgb浮307會na乞色c各m)
                                         194/ 351
                                                                  리눅스 커널 소스 해설 ［기초입문］
                                                                            kp robes 이해



          my_kretprobe.kp.sym bo[_name = func_name; //kretprobe 심볼명
         ret = register_kretprobe(&my_kretprobe); //kretprobe 등록
         if (ret < 0) {
                  pr_err(" register_kretprobe Failed, returned %d\ri", ret);
                  return－기
         }
         pr infoCPlanted return probe at %s: %p\n",
         my_kretprobe.kp.symbol_name, my_kretprobe.kp.addr);
         return 0;
}


kretprobes 는 register_kretprobe() 함수에 전달한 my_kretprobe 구조체 정보를 사용하여 등록

됩니다. 여기서 func_name 에 전달하는심볼 명칭이 kretprobes 의 ret_handler() 함수가 동작을

시작하는 커널 코드의 심볼（함수명）입니다． 아래 코드에서는 디폴트로 "mdo fork " 로 했습니다．

이렇게 하면 커널 코드가 실행 되다가 " do fork " 함수를 만나면 이 함수가 실행되고 리턴되는

시점에서 ret_handter() 함수가 실행됩니다.



my_kretpr的e 구조체

sta匕c char func_nam이NAME_MAX] = "_do_fork"; //kretprobes율위한심볼명칭
module_param_string(func, func_name, NAMEMAX, S_IRUGO);
MODULE_PARM_DESC(func, "Function to kretprobe; this module will report the"
"function's execution time");


static struct kretprobe my_kretprobe = { //kre印robe 등록될때 사용하는 구조쳬
          .handler = ret_handler,
          .entry_handler = entry_ha ndter,
          .data_size = sizeof(struct my_data),
          /* Probe up to 20 instances concurrently. */
          .maxactive = 20,
}’,
      커널연구회佃쌔시／.kernel.뇨）                                                      정재준（rgbi3307@nate.com)
                                                 195/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                    kprobes 이해




ret_handler() 함수에서는 커널의 "1 do fork" 함수의 실행 시간을 나노초（ns) 단위로 계산하여

"/var/Log/sysLog " 에 출력합니다. 따라서 사용자는 "edo fork" 함수의 성능을 평가할 수 있는 실행

시간을 확인할 수 있게 됩니다．


지금까지 Kprobes 에 대한 설명과 예제 소스들을 설명 드렸습니다. 예제 소스는 커널 모듈로

코딩되어 있기 때문에 "커널 모듈 프로그래밍" 을 많이 연습해둘 필요가 있습니다. 앞으로 이어지는

커널 소스도 모듈 프로그래밍 되어 있는 예제 소스들을 활용하여 해설을 이어갈 예정입니다．


이번 글은 여기서 마치도록 하겠습니다. 저의 글로 인해서 커널 소스 분석이 한층 즐거워 졌으면

합니다. 다음글에서 뵙겠습니다．




커널연구회（ww比kerneLbz)                             정재준（rgbi3307@)nate.com)
                             196/ 351
                                                         리눅스 커널 소스 해설 ［기초입문］
                                                             debug objects 이해




debug objects 이해


  J人卜
                                         제가 이글을 작성하는 시점（2019 년 3 월 4 일）에서 리눅스 커널

                                         버전이 v5.0 으로 업그레이드 되었습니다. v4.20 과 비교해서

  Kernel debug objects                   어느정도 변경이 있는지 이td旴 명령으로 소스 파일 단위로 통겨1


  ]                     """
                                         데이터를 산출해 봤습니다. 커널이 계속 버전업 되는 이유중에

                                         하나로 Cpu 와 하드웨어 장치들이 계속 발전하기 때문입니다．

아래 통계 데이터를 보면 Cpu 아키텍쳐（arch）에 해당하는 소스와 디바이스 드라이버（drivers)

소스에서 가장 많은 변경이 있음을 알 수 있습니다．


리눅스 커넌소스 v4.20과v5.O 소소 파앉변화텍寶
$ ait diff
  M
             v4. 20 v5. O(          irstat= files
                              ＼나／    小   －




   3. 5% Documentation!media/uaoi!
   6. 0% Documentation!
   4. 5% arch!arm!boot!dts!
   3. 3% arch!sh!
  16. 5% arch!
   8. 2% drivers!aou!drm!
   4. 1% drivers!net/ethernet!
   3. 3% drivers/net!
   3. 2% drivers!staaina!
  23. 0% drivers!
   3. 0% fs/
   5. 4% include!
   4. 0% net!
   4. 2% tools!



저는 개인적으로 CPU 아키텍쳐에 대해서 관심이 많습니다. 커널 소스도 x86, arm64, riscv

아키텍쳐를 서로 비교하면서 분석하고 았습니다. 아키텍쳐에 관한 소스는 CPU 의존적이71 때문에




 커널연구회（小째／w.kerne나）z)                                          정재준(r야)13307@nate.com)
                                              197/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                      debug objects 이해



인라인 어셈블리로 작성되어 있는 부분이 많습니다. 그리고 CPU 구조에 대해서도 알아야 합니다．

이것에 대해서는 앞으로 따로 시공간을 마련하여 설명할 예정입니다．




debug objects 7H념

이번에 이야기할글의 주제는커널의 "debug야玎ects이해" 입니다. 이 소스는2008년도에 커널

소스에 추가된 것이여서 v2.6 부터 있었던 것입니다. 그리고 "debug 야玎ects"을 잘 이해해 두면

앞으로 커널 소스를 분석할따1 많이 도움되기 때문에 오늘은 이것부터 자세히 정리해 놓도록

하겠습니다． 이 소스는 비교적 간단합니다. 아래와같이 "debug야玎ects.h" 헤더 파일과

"debugobjects.c" 소스 파일로 구성되어 있습니다．


debug ob加cis 소스 파일듈

inciude/linux/debugobjects. h
lib/ debugobjects . c
Documentation/core- api/debug- objects. rst


먼저
 ，Documentation 경로에 있는 "debug-objects.rst" 파일을보면 "debug 야玎ects" 개념에

대해서 다음과 같이 설명하고 있습니다．


".debugob忙比S 는 일반적인 내부 자료구조로서 커널 ob忙cts 의 수명（life time）을 추적하고 동작

상황을 점검한다"


debuqob他cts 는 다음과 같은 오류 패턴을 검출할 수 있습니다．


  1   Activation of uninitialized objects


  D Initialization of active objects




커널연구회（的附．kernel勺力                                     정재준（rgbi3307@nate.com)
                                       198/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                 debug objects 이해



   1    Usage of freed/destroyed objects




debug야）忙cts을실행하는함수들은 "include/Linux/debug야기ects.h" 파일에 다음과같이

선언되어 있습니다. CONFIG DEBUG OBJECTS 커널 빌드 상수값이 정의 되어 있어야 이 함수들은

동작합니다．



inctude/Linux/debugobjects.h

#ifdef CONFIG DEBUG OBJECTS
extern V이d debug_object_in止      (V이d 出addr, struct debu또야小descr차扼scr);
extern \／이d
debug_o可ect i毗on就ack(vok卄addr, struct debu오的j_descr 차扼scr);
extern mnt debug_object_activate (void *addr, struct debug_obj_descr *descr);
extern v이dd毗山下히吼t_deactivate(vok卄addr, struct debu오的j_descr 出descr);
extern void debug_object_destroy (void *addr, struct debug_obj_descr *descr);
extern void debug_object_free     (void *addr, struct debug_obj_descr *descr);
extern void debug_object_assert_init(void *add, struct debug_obj_descr *descr);


extern＼幻너
debugJ이吼I故山之攷ate(voic卄addr, struct debug_야攻descr *descr,
        unsigned mnt expect, unsigned mnt next);


extern void debug_objects_early_init(void);
extern void debug_objects_mem_init(void);
#e[se
static inline void
 debug_object_mnit    (void *addr, struct debug_obj_descr *descr) {}
 static inline void
 debug_o이ect i毗Jn就ack(voic卄addr, struct debu또야止descr *descr) {}
 static inline mnt
 debug_object_activate (void *addr, struct debug_obj_descr *descr) { return 0; }




  커널연구회佃쌔쌔／.kerne比z)                                                   정재준（寸)i3307@nate.com)
                                            199/ 351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                    debug objects 이해



 static inline void
 debug_object_deactivate(void *addr, struct debug_obj_descr *descr) { }
 static inLine void
 debug_object_destroy (void *addr, struct debug_obj_descr *descr) { }
 static inLine void
 debug_object_free      (void *addr, struct debug_obj_descr *descr) { }
 static inLine void
 debug_object_assert_init(v이d 出addr, struct debug_야攻descr 차把scr) {}


 static inline void debug_objects_earLy_init(void) { }
 static inLine void debug_objects_mem_init(void) {}
 #end汗




debug objects 함수들

위의 함수들을 다음과 같은 순으로 분석해 보도록 하겠습니다．


void debug_objects_early_init (void) ;
void debug_object_init (void *addr, struct debug_obj_descr *descr) ;
void debugmobject_free(void *addr, struct debug_obj_descr *descr) ;
mnt debug_object_activate (void *addr, struct debug_obj_descr *descr) ;
void debug_objectmdeactivate(void *addr, struct debug_obj_descr *descr) ;




debug_objects_early_init()

먼저 debug미objects_early_init() 함수와 관련된 소스들은 Lib/debug야可ects.c 파일에 다음과 같이

정의 되어 있습니다．


lib/debugo



커널연구회（叫／
       ＼岫erne나）z)                                                         정쟤준（rgbi3307（흐）nate.com)
                                            200/ 351
                                                                 리눅스 커널 소스 해설 [ 'I초입문］
                                                                         debug objects 이해


 #defineODEBUG HASH BITS 14
#define ODEBUG_HASH_SIZE (1 <<ODEBUG_HASH_BITS)


#define ODEBUG POOL SIZE 1024
#define ODEBUG POOL MIN LEVEL 256


#define ODEBUG CHUNK SHIFT PAGE SHIFT
#define ODEBUG_CHUNK_SIZE (1 <<ODEBUG_CHUNK_SHIFT)
#define ODEBUG_CHUNK_MASK (-(ODEBUG_CHUNK_SIZE - 1))


struct debug_bucket {
      struct hlist head List;
      raw_spinLock_t      Lock;
};
/／力nctude/linux/debug毗加ctsh
f//debug 야加吐S 구조체
struct debug_obj {
      struct hList node     node;
      enum debug_obj_state state;
      unsigned mnt        astate;
      void           北object; //／객쳬 주소
      struct debug_obj_descr *descr;
};
 static struct debug_bucket obj_hash[ODEBUG_HASH_SIZE}; ///debug objects 해A UI열
 static struct debug_obj          obj_static_pooL[ODEBUG_POOL_SIZE] _initdata;


 吼atic DE디NE_RAWj메吐OCK(poo나ock);


     static HLIST_HEAD(obj_pooL);
     static HLIST_HEAD(obj_to_free);


     void _init debu且的忙Ct乞的rty_init(v이d)




     커널연구회佃쌔I'月．kerne比z)                                                 정재준似狗日307@nate.com)
                                                 201 /351
                                                          리눅스 커널 소스 해설 1기초입문］
                                                              debug objects 이해



{
    mnt i;


    fom = 0; i <ODEBUG거ASH_SIZ日 나＋)
      raw_spmn_lock_mnit(&obj_hash[i}.Lock);


    for (I = 0; i <ODEBUG_POOL_SIZE; i++)
      hlist北d_head(＆아攻static_叩이[i].node屈的j_po메；
}
ODEBUG_HASH_SIZE 는 (1 <<ODEBUG_HASH_B仟S) 이므로 (1<< 14) 입니다． ] 을 왼쪽으로

14 번 시프트 하면 ]6K 에 해당하는 숫자인 ]6384 입니다. 즉, ODEBUG_HASH_SIZE 는 16384

이므로 obj_hash[16384］는 struct debug_bucket 배열이 됩니다．

raw_spin_Lock_i ni t(＆야）j_has帥].Lock); 코드는 obj_hash 구조쳬 배열의 멤버인 Lock 변수값을

_RAW_SPIN_LOCK_UNLOCKED으로초기화합니다.


ODEBUG_POOL_SIZE는 ]024로 정의 되어 있습니다. obj_static_poo山024］은 struct

debug_obj 구조체 배열입니다. hList_add_head(&obj_就atic_I兀이[ij.node, &obj_po이上 코드는

HLIST_HEAD(o可_pooL）에 야攻static_poo小］.node 들을 다음 그림과 같이 연결합니다．


h如t연藿

             firs             next                next         next
                              1pr定甘               pprev       pprev




그림참조：h比ps:j／니厄巾ag比hub.向／faciLity/Long-List-of小nked小sts.htmL




커널연구회（w寸／＼六／
           .kerne나）z)                                         정재준（rgbi3307@nate.con心
                                               202/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                                debug objects 이해



debug_object_init()

debug_object_m i目）함수는 Lib/debug야加cts.c 파일에 다음과 같이 정의 되어 있습니다．

주석문으로 소스를 설명했습니 다．



d탸w工O坊吼tJn奴）함수 소스
static v이d
Hdebu且的忙ct_init(vok卄addr, struct debug_的j_descr 士descr, mnt onstack)
{
    enum debug_obj_state state;
    struct debug_bucket차北; ///debug_bucket하씨 구조체 배열
    struct debug_obj火obj; ///debug_obj 객쳬 구조쳬
    unsigned Long flags;


    filL_po에）;


    db = get_bucket((unsigned Long) addr); ///addr해시키 계산하여 &debug_bucket가져옴


    raw_spin_lock_irqsave(&db->Lock, fLags); I//Lock설정


    obj = Lookup_object(addr, db); 1/1db 하因 구조쳬 배열에 addr 이 있으면 debug_obj 주소 반환
    if (!obj) { ///debug_obj 가 없으면
        obj = aLLoc_object(addr, db, descr); /11db 하1시 구조체 배열에 addr 욜 객쳬로 연결
        if (!obj) { I//debugm多bj 연결하지 못했다면，
            debug_objects_enabled = 0;
            raw_spin_un(ock_irqrestore(&db->Lock, flags);
            debug_objects_oomQ; ///"Out of m的聆깡．ODEBUG小珀臥ed" 출력후debug_obj해제
            return;
        }
        debug_object_is_on_stack(addr, onstac毗 ///debug_obj 의 addr 이 커널 스택에 있는지 점검
    }
    ///debug_obj 상태1 처리
    5＼사itch 佃t乎＞state) {




    커널연구회（www.kerne나）z)                                          정재준（rgbi3307@nate.com)
                                                203/ 351
                                                          리눅스 커널 소스 해설 ［기초입문］
                                                              debug objects 이해



    case ODEBUG STATE NONE:
    case ODEBUG STATE INIT:
    case ODEBUG STATE INACTIVE:
     obj->state = ODEBUG_STATEJNIT; I/ It出了상태로 처리
     break;


    case ODEBUG STATE ACTIVE:
     debugj川毗_object(obj, "in止"）·, //／경고메세지 출력
     state = 야乎＞state;
     raw_spin_untock_irqrestore(&db->Lock, fLags);
     debug_obje叱fixup(descr今fixup_in止, addr, state); //／日xu口in次실행
      return;


    case ODEBUG STATE DESTROYED:
     debug_i川nt_object(obj, "in化"）·, //／경고 메세지 출력
      break;
    defau比
      break;




    raw_spin_unlock_irqrestore(&db->Lock, flags);




void debug_object_init(void *addr, struct debug_obj_descr *descr)
{
    if (!debug_objects_enabled) ///debugmob昶cts가가능상태가 아니면 리턴
     return;


    _debug_object_init(addr, descr, 0); //／내부함수호출
}
EXPORT_SYMBOL_GPL(d ebug_object_init);




커널연구회（小쌔쌔／.kerne나）力                                                 정재준（rgb浮307@nate.con寸
                                           204/ 351
                                                           리눅스 커널 소스 해설 ［기姦입문］
                                                               debug objects 이해



debug_object_free()

debug_object_f ree() 함수는 Iib/debugobjects.c 파일에 다음과 같이 정의 되어 있습니다．

주석문으로 소스를 설명했습니다．



debu且．ob如比free() 함수 소스
void debug_object_free(void *addr, struct debug_obj_descr *descr)
{
    enum debug_obj_state state;
    struct debug_bucket *db;
    struct debug_obj *obj;
    unsigned long flags;


    if (!debug_objects_enabled) ///debug_ob忙cts가가능 상태가아니면 리턴
      return;


    db = get_bucket((unsbned long) add巾, ///addr해시키 계산하여 &debug中bucket가져옴


    raw_spin_lock_irqsave(&db->lock, flags); f//lock설정


    obj = lookup夕可ect(addr, db); 1/1db 해시 구조체 배열에 addr 이 있으면 debug_obj 주소 뱐환
    if (!obj) ///debug_obj 가 없으면 lock하1제車 종료
      goto out_unlock;


    switch（야小＞state) {
    case ODEBUG STATE ACTIVE:
      debug_print_object(obj, "free '); //／경고 메세지 출력
      就ate = 야小＞state;
      raw_spin_unlock_irqrestore(&db->lock, flags); f//lock해1제
      debug_object_fixup(descr->印山p_fre已 addr, state); /// 日xup打ee 실행
      return;
    defau比
      hlist_d이（＆야斗＞node);




    커널연구회（www.k針ne나）z)                                              정재준（r야)i3307@nate.con力
                                           205/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                     debug objects 이해



        raw_spin_unlock_irqrestore(&db->Lock, flags); I//伯ck해쟤
        타ee_object(obj); f//debug놔obj 해丙｝
        return;
    }
out unlock:
    raw_spin_unlock_irqrestore(&db->lock, flags); i//lock하1졔
}
EXPORT_SYMBOL_GPL(debug_object_free);




debug_object_activate()

debug_o히ect_ac匕vate() 함수는 lib/debug야加cts.c 파일에 다음과 같이 정의 되어 있습니다．

주석문으로 소스를 설명했습니 다．



debu요批ject_act押ate() 함수 소스
mnt debug_object_activate(void *addr, struct debug_obj_descr *descr)
{
           enum debug_obj_state state;
           struct debug_bucket *db;
           struct debug_obj *obj;
           unsigned long flags;
           mnt ret;
           struct debug_obj o = { .object = addr,
                                  .state = ODEBUG_STATE_NOTAVAILABLE,
                                  .descr = descr };


           if (!debug_objects_enabled)        f//debug_objects가가능상태가아니면 리턴
                      return 0;




커널연구회佃쌔쌔／.kerne比z)                                                      정재준（rgb日307@nate.com)
                                                      206/ 351
                                                               리눅스 커널 소스 해설 ［기초입문］
                                                                   debug objects 이해



    db = get_bucket((unsigned Long) addr);          ///addr해시키 계샨하여 &debug_bucket가져옴


    raw_spin_Lock_irqsave(&db->Lock, flags);        I//Lock설정


    obj = lookup_object(addr. db); ///db 해시 구조체 배열에 addr 이 있으면 debug_obj 주소 반환
    if (obj) {       ///debug_obj 가 있으면
                 S니／itch 徊I乎＞state) {
                 case ODEBUG STATE INIT:
                 case ODEBUG STATE INACTIVE:
                         야乎＞state = ODEBUG_STATE_ACTIVE; /1/Ac기VE상태로 설정
                         ret= 0;
                         break;


                 case ODEBUG_STATE小ACTIVE: ///activate에서 AC了IVE상태이면 경고 매세지 출력
                         debug_print_object(obj, 'ac匕vate"); //／경고 메세지 출력
                         state = 야小巧tate;
                         raw_spin_unLock_irqrestore(&db->Lock, flags);
                         ret = debug_object_fixup(descr->fixup_activa te, addr, state);
                         return ret? 0 : -EINVAL;


                 case ODEBUG STATE DESTROYED:
                         debug_i川nt_object(的1, "activate"); //／경고메세지 출력
                         ret = -EINVAL;
                         break;
                 defau化
                          ret = 0;
                          break;
                 }
                 raw_spin_unLock_irqrestore(&db->lock, flags); f//lock 해제
                 return ret;
    }

    raw_spin_unlock_irqrestore(&db->lock, flags); f//Lock해제
    ／古
커널연구회佃,ww.kerne나끄）                                                       정재준（rgbi3307@nate.com)
                                             207/ 351
                                                              리눅스 커널 소스 해설 [:71초입문］
                                                                  debug objects 이해



      士 We are here when a 就atic 야加ct is ac匕vated. We
       衣 [etthe types口ec小c code confirm ＼六／
                                          hether this 沽
       * true or not. 汗 true, we just make sure that the
       * static object is tracked in the object tracker. if
       * not, this must be a bug, so we try to 目x it up.
       火／
      if (descr->is_static_object && descr->is_static_object(addr)) { //／정적함수있으면 실행
               少 tract; 냔沾 static 야加吐 六／
               debug_object_init(addr, descr);
               debug_object_activate(addr, descr);
      }eLse{
               debug_print_object(&o, "activate"); //／경고 메세지 출력
               ret = debug_object_fixup(descr->fixup_activate, addr,
                                          ODEBUG_STATE_NOTAVAILABLE);
               return ret? 0 : -EINVAL;
      }
      return 0;
}
EXPORT_SYMBOL_GPL(debug_object_activate);




debug_object,.deac1iva1e()

debug_o히ect_deac匕vate() 함수는 lib/debug야加cts.c 파일에 다음과 같이 정의 되어 있습니다．

주석문으로 소스를 설명했습니다．



寸毗世且oliect_deact押at旦（) 함수 소스

V이ddebu且的ject_deac山ate(voic伊addr, struct debu또야止descr 서escr)
{



커널연구회（www.kern日.bz)                                                    정재준（rgbi3307（孕nate.com)
                                            208/ 351
                                                          리눅스 커널 소스 해설 ［기초입문］
                                                              debug objects 이해



    struct debug_bucket *db;
    struct debug_obj *obj;
    unsigned tong flags;


    if (!debug_objects_enabled) ///debug_ob忙仗S가 가능 상태가 아니연 리턴
             return;


    db = get_bucket((unsigned long) addr); ///addr해시키 계산하여 &debug_bucket가져옴


    raw_spin_lock_irqsave(&db->lock, flags); f//lock설정


    obj = lookup_object(addr, db); /11db 해시 구조체 배열에 addr 이 있으면 debug中obj 주소 반환
    if (obj) { f//debug小obj 가았으면
             switch（야小＞state) {
             case ODEBUG STATE INIT:
             case ODEBUG STATE INACTIVE:
             case ODEBUG STATE ACTIVE:
                       if (!obj->astate)
                                0이－>state = ODEBUG_STATEJNACTIVE; /／月NAC丁IVE 상태로 설정
                       이se
                                debug_print_object(obj, "deactivate"); //／경고 메세지 출력
                       break;


             case ODEBUG STATE DESTROYED:
                       debug_f川nt10可ect佃bj, "deactivate"); //／경고 메세지 출력
                       break;
             default:
                       break;
             }
    }else{
             struct debug_obj o = { .object = addr,
                                    .state = ODEBUG_STATE_NOTAVAILABLE,
                                    .descr = descr };




커널연구회佃쌔,w.kernel.뇨）                                               정재준（四bi3307@nate.com)
                                            209/ 351
                                                         리눅스 커널 소스 해설 E기초입문］
                                                             debug objects 이해



               debug_i川nt_object(&o, "deactivate'); //／경고메세지 출력
       }

       raw_spin_unlock_irqrestore(&db->lock, flags); I//lock해1제
}
EXPORTjYMB아；GPL(debu且的忙ct_deacti此te);




debugob忙cts 활용

리눅스 커널 소스에서 debug objects 을 활용하고 았는 소스 파일은 다음과 같습니다， 생각보다 많지

않습니다. RCU, 기mer, WorkQueue, percpu counter, gpu dim i91 5 드라이버 정도 입니다．

필자는 "kernel/workqueue.c"에 있는 소스에서 debug objects 을 어떻게 활용했는지 분석한

내용을 정리 했습니다．




debug ob加cts量毋용하고있뇹多姐소스파욈
kernel/rcu/update. c
kernel/ time/h rtimer . c
kernel/ time/ timer. c
kernel/workqueue . c
lib/ percpu_counter . c
drivers/gpu/drm/i915/1915_sw_fence . c

debug objects 을 활용하기 위해서는 먼저 debug_c可_descr 구조체에 내용들을 채워 넣는

작업부터 해야 합니다．



incL프de/tin뗘／d實b1四毗加CL丘h
struct debug_obj_descr {
       const char              *name;
       V이d 士（士debug_hint)(v이d 出addr);
       bool (*is_static_object)(void *addr);




커널연구회（w叫／.kern힌.bz)                                               정재준（r야N3307@nate.con介
                                           210/ 351
                                                                    리눅스 커널 소스 해설 ［기菱입문］
                                                                        debug objects 이해



               boot (*fixup_init)(void *addr, enum debug_obj_state state);
               boo나섀刈q配匕vate)(v이d 火ad北 enum debug_o可_state state);
               boot (*fixup_destroy)(void *addr, enum debug_obj_state state);
              boot (*fixupmfree)(void *addr, enum debug_obj_state state);
              boot (*Fixup_assert_init)(void *addr, enum debug_obj_state state);
};
"kernel/workqueue.c"에서는 다음과 같이 debug_o니_descr 구조체를 work_debug_descr로

정의하고 그안에 내용을 채워 넣었습니다. 아래 내용들을 주석문으로 설명하도록 하겠습니다. 아래

소스 코드는 CONFIG_DEBUG_a BJECTS_WORK 커널 컴파일 상수가 정의 되었을때1 동작합니다．



呻h싸如心quei建璡
斛fdef CON디C DEBUG OBJEC了S WORK


static struct debug_obj_descr work_debug_descr;


//／디버그 힌트 콜백 함수
sta匕c vok卄wor匕由bug씨nt(vok卄ad小）
{
         return ((struct work_struct *) addr)->func;




//／정적 객체인지 판단하는 함수
 static boot work_is_static_object(void *addr)
 {
         struct work_struct *work = addr;


         return test_bit(WORK_STRUCT_STATIC_BIT, work_data_bits(work));
     }

     //／객체 사용이 잘못 되었을때 수정하는 함수
     static boot work_fixup_init(void *addr, enum debug-'obj_state state)
     {



         커널연구회佃쌔쌔／.kerne나）기                                                  정재준(r야)i3307@nate.com)
                                                   211 /351
                                                                리눅스 커널 소스 해설 E가초입문］
                                                                    debug objects 이해



          struct work struct *work = addr;


          switch (state) {
          case ODEBUG STATE ACTIVE:
              canceL_work_sync(work);
              debug_object_i nit(work, &work_debug_descr);
              return true;
          defau比
              return false;
          }
      }

      //／쩍채사용이 쟐妥되었율때해쳬하는함수
      static boot work_fixup_free(void *addr, enum debug_obj_state state)
      {
          就ruct＼사orkJtruct 火work = addr;


          switch (state) {
          case ODEBUG STATE ACTIVE:
              cancel_work_sync(work);
              debug_object_free(work, &work_debug_descr);
              return true;
          defauLt:
              return false;
          }
  }

  static struct debug_obj_descr work_debug_descr = {
          .name      = "work_struct", I//debug_object에 명칭 부여
          .debug_hint = work_debug_hint, //／디버그힌트콜백 함수
          .Is小static_o可吼t = work_i乞就atic_o이ect, //／정적 객쳬인지 판단하뇬 함수
          .fixup_init = wonF느日xup_in止, ／月객체사용이 잘못되었을때 수정하는함수
          .fixup_free = work_fixup_free, //／객쳬 사용이 잘못되었율때홰群하뇬함수
｝·,
      커널연구회（硼附／.kernel．虹）                                                   정쟤준（I야）沼307會nate.com)
                                                  212/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                  debug objects 이해




위에서 정의한 work_debug_descr 구조체는 " kernel/workqueue.c"에서 다음과 같이 활용됩니다．

주석문으로 설명을 달았습니다．



kerneL/workqueue.c 에서 활용 코드
static inline void debug_work_activate(struct work_struct 처A/ork)
{
     debug_o이缸t ac匕vate(work, &work_debug_ 扼＄ci); I//debug工帥ect활성
}

static inline void debug_work_deactivate(struct work_struct *work)
{
     debug_object_deac匕vate(work, &work_debug_descr); f//debug_object UI활성
}

void 1 initwork(struct work_struct *work, mnt onstack)
{
     if (onstack)
       debug_object_init_on_stack(work, &work_debug_descr);
     else
       debug_object_init(work, &work_debug_descr); i/ /debug_object    기화
}
 EXPORT_SYMBOL_GPL(_jnit_work);


 void destroy_work_on_stack(struct work_struct *work)
 {
     debug_object_free(work, &work_debug_descr); I//debugmobject홰1제
 )
 EXPORT_SYMBOL_GPL(destroy_work_on_stack);




     커널연구회（小八사w.kern이.bz)                                             정재준（r야)13307@nate.com)
                                            213/ 351
                                                            리눅스 커널 소스 해설 E기초입문］
                                                                debug objects 이해



"kernel/workqueue.c"에서는 struct work_就ruct士w아k구조체를 debug_o可ect로 등록

합니다. 이것에 대해서 debug_work..크ctivate(）함수와 debug_w아k_deactivate() 함수를

번갈아 실행하면서 debug_o可ect 로 등록한 struct 的ri느struct 火work 구조체 객쳬를 올바로

사용하는지 점검하게 됩니다．


아래 소스코드는 debug_ob忙cts 을 올바르게 사용하지 않았을때 경고 메세지를 출력하는 함수의

소스 코드 입니다．



Lib/debugo可配匕（얘서 겅고 쩨圈지膏력 斟＝
static void debug_print_object(struct debug_obj *obj, char *msg)
{
    struct debug_obj_descr *descr = obj->descr;
    static mnt limit;


    if (limit < 5 && descr != descr_test) {
        V이d 샤｝mnt = descr->debug卞hint ?
          descr->debu또hint(ot乎札이吼t) : NULL;
        (imit++;
        WARN(1, KERN_ERR "ODEBUG: %s %s (active state %u) '
             "object type: %s hint: %pS\n",
          msg, obj_states[obj->state], obj->astate,
          descr->name, hint);
    }
    debug_objects_warnings++;
}

경고 메세지는 5 번까지 출력됩니다. 위의 WARN 매크로에서 출력되는 경고 메세지의 예는 다음과

같습니다．


ODEBUG: activate active (active state 0) object type: work_struct hint: 0x55e8906ef908S




 커널연구회（蜘iw.kernel.bz)                                              정채준（rgb日307@nate.com)
                                              214/ 351
                                            리눅스 커널 소스 해설 ［기초입문］
                                                debug objects 이해



debug_objects 가 active 상태에서 잘못된 실행이 발생한 경우 입니다. object type 에 출력된

descr->name 을 통해서 객체명을 구분할 수 있습니다. hint: 0x55e8906ef908 는 struct

debug_o可_descr 구조체에 등록한 힌트 함수의 주소 입 니다．


지금까지 debug_ob忙cts 를 정리한 글을 읽어 주셔서 감사합니다．


겨울동안 움츠려 있었던 몸과 마음이 봄이 되니까 좀더 활동성 있어 지는듯 합니다. 더불어 커널

소스를 분석하는 시간도 잘 안배해야 겠습니다. 그동안 내용들을 좀더 수정 보완하여 책으로도 출판할

예정입니다. 책 내용을 구성하면서 매번 느끼는 것이지만, 200페이지 원고에서 고비가 오는듯 합니다．

책의 모양새와 품질 완성도를 높이려면 적어도 300싸400 페이지는 되어야 하는데 200 페이지 도달

시점에서 살짝 나태해 집니다. 다시 마음을 바로 잡아야 겠습니다. 다행히 커널 소스는 무궁무진해서

책으로 정리해야 하는 것들이 많습니다. 분량 걱정은 안해도 된다는 장점은 있지만 시간이 많이

소요되는 작업이라 시간 활용을 잘하뺘 겠습니다. 이 지면을 통하여 리눅스 커널 소스를 무료로

꾸준히 배포하고 있는 리너스 토발즈와 전세계 커널 엔지니어들에게 감사의 마음을 전하고 싶습니다．




 커널연구회佃w닉／.kernet.뇨）                              정재준（rgbi3307(@nate.con分
                               215/ 351
                                               리눅스 커널 소스 해설 E기초입문］
                                                    커널 디버그 메세지 출력




커널 디버그 메세지 출력

지금까지 리눅스 커널 소스를 디버깅 하는 방법에 대해서 기술했으나. 커널 소스를 가장 간단하게

디버깅 하는 방법은 소스 중간 중간에 printk() 함수를 삽입하여 그때마다 궁금한 데이터를 콘솔에

출력에 보는 것입니다. 햐지만 이 방식은 printk() 함수를 추가, 삭제하고 컴파일하는 과정이 매우

번거럽습니다. 이러한불편함을조금이라도해결하고자. 리눅스 커널 소스에는 printk() 함수를

아래와 같은 매크로로 정의하여 설정 상수와 레벨에 따라서 조건 컴파일 하는 방식으로 좀더 편리하게

관리할 수 있습니다．

먼저, 가장 간단한 방법으로 디버그 메세지를 출력 레벨별로 선별하여 동작 시킬 수 있습니다．




메세지 출력 레벨 조정

출력 레벨은 다음과 같이 콘솔 명령으로 커널 마oc 파일 시스템에 설정 가능합니다．


echo 0 > /proc/ sys/kernel/printk
echo 4 > /proc/sys/kernel/printk
echo 8 > /proc/sys/kernel/printk




레벨 번호가 낮을 수록 응급한 메세지（에러. 알림）만 출력 됩니다. 레벨 4 는 경고에 해당하는 메세지가

출력되고 레벨 8 은 디버그를 위한 대부분의 메세지가 출력 됩니다. 따라서 레벨을 높이면 높일수록

디버그 메세지가 많이 출력 되므로 시스템 성능이 저하 됩니다. 아래는 레벨 번호를 정의하고 있는

커널 소스（헤더파일）입니다．




커넣연구회如加邸／.kerne(, 址）                               정쟤준（四bi3荻玎回flat色corn)
                                    216/ 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                         커널 디버그 메세지 출력



/incLude/tinux/kern_(evets.h
#define KERN SOH "\ OOl"             1* ASCII Start Of Header *1
#define KERN SOH ASCII 1\OOl?

#define KERN EMERG      KERN SOH "0"      ／出 system is unusable 出／
#define KERN ALERT      KERN SOH "그．"     /士 action must be taken
immediately *7
#define KERN CR11 KERN SOH "2"            /* critical conditions *1
#define KERN ERR KERN SOH "3"             1* error conditions *7
#define KERN WARNING    KERN SOH 1141!    1* warning conditions *7
#define KERN NOTICE     KERN SOH 1151?    7* normal but significant
condition *7
                                               士
#define KERN INFO KERN SOH "6"                     informational */
                                           /
                                           /
                                           1
                                               士
#define KERN DEBUG      KERN SOH 117?!             debug-level messages *1

                         nn
#define KERN DEFAULT                 /* the default kernel loglevel *1




위의 레벨번호는 커널 소스 力nclude/Linux/printk.h 에 다음과 같이 p乙로 시작되는 매크로에서

printk(）함수의 인자로 전달되어 출력 레벨별로 선별하여 메세지가 출력 됩니다．



／奴C佃d可硼出加雌ntkl1

#define pr_emerg(fmt, . . .) \
      print k (KERN_EMERG pr_fmt (fmt) , ##1VA_ARGS_ )
#define pr_alert (fmt, . . .) \
      printk (KERN_ALERT pr_fmt (fmt) , ##1VA_ARGS1)
#define pr_crit (fmt, . . .) \
      printk (KERN_CRIT pr_fmt (fmt) , ##_VA_ARGS__)
#define pr_err (fmt, . . .) \
      print k (KERN_ERR pr_fmt (fmt) , ##_VA_ARGS_ )
#define pr_warning(fmt, . . .) \
      printk (KERN_WARNING pr_fmt (fmt) , ##_VAARGS_)
#define pr_warn pr_warning
#define pr_notice(fmt, . . .) \
      printk (KERN_NOTICE pr_fmt (fmt) , ##_VA1ARGS__)
#define pr_info (fmt, . . .) \
      printk (KERN_INFO pr_fmt (fmt) , ##_VA_ARGS1)




 커널연구회佃쌔시／.kerneLbz)                                       정재준（寸)i3307@nate.con力
                                   217/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                   커널 디버그 메세지 출력



위의 기능들을 리눅스 커널 소스를 빌드할때I menucofing 에서 다음과 같이 설정할 수 있습니다．



콘솔에 메세지를 출력하는 레벨을 다음과 같이 1 에서 ]5 범위에서 설정할 수 있습니다. 기본은 7 로

설정 되어 있습니다．



每古 기뵨川세자레墅섶청枷enuconfig
Symbol: CONSOLE_LOGLEVEL_DEFAULT [=7]
   Type : integer
   Range : [1 15]
   Prompt: Default console loglevel (1-15)
      Location:
        -> Kernel hacking
          -> printk and dmesg options
     Defined at lib/ Kconfig. debug: 37




printk(）에 레벨을 주지 않고 사용할때는 아래의卜4ESSAG巳LOGLEVEL니DEFAULT 가 적용됩니다．

이 값은 ] 에서 7 범위에서 설정할 수 있으며, 기본적으로 menuconfig 에서 4 로 설정되어 있습니다．




매섀지 까뵨 래賢섶쩔 m帥'Co而g
Symbol: MESSAGE_LOGLEVEL_DEFAULT [=4]
   Type : integer
   Range : [1 7]
   Prompt: Default message log level (1- 7)
     Location:
        -> Kernel hacking
          -> printk and dmesg options
     Defined at lib/ Kconfig. debug: 63




커널연구회（小쌔／w.kern이,bz)                              정재준（r야)13307（孕nate.com)
                                218/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                    커널 디버그 메세지 출력




다이나믹 레벨 조정

다이나믹 레벨은 특정 소스파일의 일부분 지정한 곳에서만 디버그 메세지가 출력 됩니다. 먼저, 커널

다이나믹 디버그 메세지를 출력하는 사용 예제부터 이해하고 가겠습니다．


다아나텍 래曾섶忿예체 I

echo file test. c line 346- 373 +p > /sys/kernel/dynamic_debug/control




콘솔에서 위와 같이 커널 sys 파일 시스템을 설정하면 커널의 " test.c" 의 소스 라인 346 줄부터 373

사이의 디버그 메세지만 출력 됩니다．


다이나qt래별 섶첨 예채 2

echo file test. c function test_mnit +p > /sys/kernel/dynamic_debug/control




콘솔에서 위와같이 커널 sys파일 시스템을 설정햐면 커널의 " test.c" 소스 파일의 " test-in北" 함수에

있는 디버그 메세지만 출력 됩니다．


커널에서 위의 기능을 설정하는 상수는 다음과 같습니다. 커널을 빌드할따I menuconfig 에서 아래

상수를 [=y］로 설정해야 위의 기능이 동작합니다．


舟姆nuconfig
Symbol: DEBUG_FS [=y]
  I Type : bool
  I Prompt: Debug Filesystem
  1   Location:
  I     -> Kernel hacking
  I       -> Compile- time checks and compiler options




 커널연구회（蜘加，kerneLbz)                                   정재준（rgbi3307@nate.com)
                                  219/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                    커널 디버그 메세지 출력



  1   Defined at lib/ Kconfig. debug: 280



Symbol: DYNAMIC_DEBUG [rny]
   Type : bool
   Prompt: Enable dynamic printk () support
      Location:
        -> Kernel hacking
           -> printk and dmesg options
      Defined at fl b/kconfig. debug: 97
      Depends on: PRINTK [=y] && DEBUG_FS [=y]




위와 관련된 커널 소스는 力nc山de/Linux/printk.h 에 다음과 같이 있습니다．



月nc(ud可Linux加曲1

/* If you are writing a driver, please use dev_dbg instead */
#if defined (CONFIG_DYNAMIC_DEBUG)
#include <linux/dynamic_debug . h>

/* dynamic_pr_debug() uses pr_fmt () internally so we don 't need it   here */
#define pr_debug(fmt, . . .) \
       dynamic_p r_debug(fmt, ##_VA_ARGS_ )
#elif defined(DEBUG)
#define pr_debug(fmt, . . .) \
       print k (KERNDEBUG pr_fmt (fmt), ##_VA_ARGS_ )
#else
#define pr_debug(fmt, . . .) \
       no_printk (KERN_DEBUG pr_fmt (fmt) , ##1VAARGS1)
#endif




커널연구회佃쌔시／.kerne나）力                                    정재준（rgbi3307@nate.com)
                                  220/ 351
                                                            리눅스 커널 소스 해설 ［키초입문］
                                                                      kobj ect 이해




kobject 이해1


        小I- :，少，才，쁘，kobject
    Kernel kobject kset
                       I-쓰，＝少．:
                        。"
                                  정복하는 과정에서 반드시 알고 가야 하는 내용입니다. 먼저，

                                  리눅스 커널 소스내에 있는 문서（Documentation/k야）忙ct.txt)

                                  부터 확인해 보겠습니다. 如히ect는 이문서의 상단에 있는

구문에서 다음과 같이 그 개념을 설명하고 있습니다．


          ntation/kobject.txt


- A kobject is an object of type struct kobject. Kobjects have a name and a reference count.

A kobject also has a parent pointer (allowing objects to be arranged into hierarchies), a

specific type, and, usually, a representation in the sysfs virtual filesystem.




리눅스 커널 소스에 있는 문서는 모두 영어입니다. 더구나 내용들이 컴퓨팅에 관련된 것. 특히 리눅스

커널 Os 에 대한 것이라 영어와 Os 에 대한 배경 지식이 모두 있어야 의미가 다가 올것입니다 ．영어가

좀 된다고 하더라도 Os와 프로그래밍 지식이 없으면 위의 내용이 이해되지 않을 것입니다. 저의 글을

읽는 독자분들은 리눅스 커널 Os 와 프로그래밍（C 언어）에 대해서 사전 지식이 어느정도 있다는

가정하에 설명을 진행 하겠습니다. 그러나 되도록이면 구어체로 잘 풀어서 설명하는 방식으로

진행하겠습니다．




 커널연구회佃w납／.kerne比z)                                                 정재준（rgbi3307@nate.com)
                                          221 /351
                                                리눅스 커널 소스 해설 ［기초입뿐］
                                                          kobject 이해



위의 문서 내용을 보면, " 如bject는 구조체 如히吼t 타입의 객체佃너ect) 이다" 라고 처음에 설명하고

있습니다. 컴퓨팅 언어에서 객체는 "구조쳬로표현하는 데이터 "입니다. 보통 C언어서는구조체

(struct) 데이터 타입으로 정의하고, C+＋언어에서는 클래스（cLass) 데이터 타입으로 객체를

정의합니다. 그리고 연이어서 언급하고 있는 a name, a reference count, a parent pointer, a

specific type 등등은 k야玎ect 구조쳬 안에 들어가는 멤버들입니다. 특히 위 문서에 있는 마지막 구문

"a representa匕on in the sysfs virtua냐ilesystem." 의 의미가 중요합니다． 如니ect 을 처음으로

접하신다면 이게 무슨말인지 이해 되지 않을 것입니다. 저도 사실 소스를 직접 확인해서 실습하1

보고서 이 구문을 이해했습니다. 결과부터 말씀 드리면, kobject는 C언어 구조체이고 그 내용들은

커널의 가상파일시스템인 sysfs에서 표현（작업）됩니다. 이 의미가 중요한데, 이것은 계속

설명하면서 말씀 드리겠습니다．


如bject는 C언어 구조체입니다. 이 구조체는 리눅스 커널 소스 " include/Linux/k야万ec나）" 에

선언되어 있고. 이것과 관련된 소스 파일들은 다음과 같습니다. 그런데 제가 커널 버전에 대해서

언급을 하지 않았습니다. 커널은 계속 버전업 되고 있어서 버전마다 소스가 다를 수 있습니다. 커널

소스를 분석할따1 이게 또 어려운점인데. 저는 항상 최신 소스를 기준으로 설명합니다. 제가 이글을

작성하는 시점에서는 커널 소스 버전은 v4.20 에서 v4.20.4 로 버전업 되었습니다. 아래부터

설명하는 것은 v4.20.4 을 기준으로 한 것입니다．


  可ect 관련 소스 파임長

Inc山de/Linux/k야玎ect.h /1k야玗ect헤더파일
Lib/k야加比C ／作的拇跋소스
san耳乂es/k야玎ect/kobject-exan巾Le.c f/k磁玎虹t테스용샘플소스



"kobject.h"에는 구조체가 있고 " kobject.c"에는 실행 함수들이 있습니다． 그리고 " 如bject-

exampte.c "은 k야玎edt 을 커널 모듈로 테스트할 수 있는 샘플 소스입니다． 따라서 如bject.h -->



커널연구회佃娜i.kerneib力                                    정쟤준（rgb序307回na乞e.com)
                                     222/ 351
                                                           리눅스 커널 소스 해실 ［기초입문］
                                                                     kobj ect 이해



kobject.c -> k야玎ect-exa m이e.c 순으로 소스들을 이해 하시면 됩니다. 특히. 如히ect-exam이e.c

는 커널 모듈로 따로 실행가능하기 때문에 실습을 통해서 결과를 확인해 볼 수 있습니다．


그럼 먼저 " inctude/linux/kobject.h"에 선언되어 있는 如bject 구조체부터 보겠습니다．



奴仙de川flu町k毗Ii吼t.h

struct kobject {
         const char *name;
         struct List_head entry;
         struct k야）忙ct 士parent;
         struct kset *kset;,
          struct k야攻type 出ktype;
          struct kernf乞node 步＄d汀* sysfs directory e毗四 *1
          struct kref kref;
          #ifdefCONFlG DEBUG KOBJECT RELEASE
          struct delayed_work release;
          #end仟
          unsigned mnt state_initialized:1,
          unsigned mnt state_in_sysfs:1;
          unsigned mnt state_add_uevent_sent:1;
          unsigned mnt state_remove_uevent_sent:1;
          unsigned mnt uevent_suppress:1;
};
 如니ect 구조체안의 멤버들이 꽤 많은 편입니다. 리눅스 커널 소스를 이해 하는 과정은 위와 같은

 구조체 멤버들의 상호작용을 알아가는 여행입니다. 멤버 변수들이 많아도 하나씩 알아가면 됩니다．

 일단 k야玎ect 구조체에서 중요한 멤버 변수들부터 보겠습니다． name 은 구조체에 이름을 부여하는

     것입니다． parent는 자기자신의 부모 k야加Ct로 연결되는 포인터 입니다． kset은 k야）忙Ct

     구조체들을 모아서 리스트로 연결하는 용도입니다. sd 는 sysfs 경로로 진입하는 주소입니다. kref는




      커널연구회佃m시／.kerneLbz)                                       정재준（띠bi3307@nate.com)
                                              223/ 351
                                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                                              kobj ect 이해



참조 회수 저장용도로 사용합니다. 그리고 나머지 변수들은 比이ect 상태를 관리하기 위한 용도

입니다. 그런데 구조체 멤버들의 연결관계는 백마디의 말보다 그림으로 잘 정리하면 이해하기

쉽습니다. 아래는 ko히ect 와 연관되는 구조체둘을 다이어그램으로 필자가 정리한 것입니다．


如bject 구조체 연결 다이어그램
1uc,ude;fl, 山町Xen玄5J=
      struct k. fnta node                                                            I-I口ude小flu町kob汨그j]
接tomic t               count                                                                        struct kset
atomic t               active                                                    struct list head        list
struct kernfs node     4parent                include/lunuxJkobject h            struct kobject          kobj
cDnSt char             kname                          Struct k由加Ct               struct kset_uevent_ops 'uevent_ops
etruct rb node         rb                     Const char              ' n55e
const V口Id                                    struct list head        entry
unsigned mnt                                  struct kobject          夕parent ,
struct kernfs iattrs *tattr                   struct kset             牛kset 好 ／才              1struct IC曲主t外IC
                                              struct kobj_ type       *ktype*    { ' release)
                                              struct kernfs node *sd             struct systs ops        노ysfsops
fnclude川flu町虹ef,h                             struct kref             kref       struct attribute        口 'default attrs
           struct kref                        U32 bits                           struct attributeHgroup "default groups
ref cou！
       吐 t             ref count                          state initialized      ( 'child』 n乞 type)
                                                              state In sysfs     ( 'na冊espace)
include川fluX六耐Co냐滋也                                     ate aaci uevent sent     ( 'get_I汭咐）ership)
     struct r. fcowst struct 甘                           remove udVent Sent
atomic t                  ref S                             ueveat suppress

include／蜘）U乂／type蜘
            at01ic t
let                       counter




attribute 구조체 연결 다이어그램

                                                      Inc沁deJlinu心돠／at s.h
                                                              struct   a
include/linuxlsycfs h                                      t char             n
      struct attribute_ group                         U磁（그cie t              mode
const char                  ' fla滋e
( 'is. . visible)
( 'is   bin_visible)                                      struct     bin attribute
struct    attribute        n attrs        舞          struct      attribute   attr
struct    bin attribute     ' 'bin    attrs          size t                  드ize
                                                     void                    'private
                                                     尸read)
                                                     C 'write)
                                                     ( ' 冊目ap)




커널연구회（www.kern이b功                                                                           정재준似非焰307@nate.com)
                                                         224/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                             kobj ect 이해



아래 그림을 보시면 如bject 와 parent, kset, ktype 과의 연결관계를 블럭도 형태로 좀더 잘 이해할

수 있습니다．




如bject 객쳬 연결 다이어그램1




                                   (k으브：
                                       呼J
그림참조：http://＼六／寸／＼六／
                   .codexiu.cn/linux/blog/38520/


위와같이 작업할려면 처음에 如히ect 구조체를 만들고 멤버변수들간에 상호 연결하는 작업을 하뺘

합니다. 이러한작업과관련되는소스는 " Lib/k야玎ect.c" 에 대부분있습니다 ．如bject구조체 생성 및

추가는 k야玎ect口eate_and_add() 함수에서 이루어집니다． 아래는 이 함수의 소스입니다． 제가

한글로 주석문을 추가한 k야）忙ct_crea te() 함수에서 如히ect 구조체가 생성되고 如bject_add()

함수에서 parent 로 연결됩니다．




 커널연구회（납쌔쌔／.kerneLbz)                                   정재준（rgbi3307@nate.com)
                                       225/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                       kobj ect 이해



枷／k的如ct.c

struct k야）忙吐 恢的忙Ctm口eate크耐Jdd(const char 央name, struct k야）忙Ct 如arent)
{
        struct kobject *kobj;
        mnt retva卜，


        如bj = kobject_createO; I/k야）J吼t구조쳬를생성
        if (!kobj)
                 return NULL;


        retval = kobject_add(kobj, parent, "%s", name); 小刃bject구조체를부모（paren目에 추가
        if (retva() {
                 pr_warn("%s: kobject_add error: %d\n", _func_, retvat);
                 kob忙ct_put休obj);
                 kobj = NULL;
        }
        return kobj;
}
EXPORT_SYMBOL_GPL(kobject_create_and_add);




또한，k야）ject 는 리눅스 파일시스템인 sysfs 와 연결되는데, 이것이 사용자 입장에서 아주 중요한

역할을 합니다． 如히edt 구조체의 struct kernfs_node 升sd 멤버 변수에 sysfs 를 연결합니다．

이것은 커널 소스 " fs/sysfs/giouP.C "에 있는 sysf乞口eate_group() 함수에서 이루어 집니다． 이

함수의 소스는 다음과 같습니다．



fs/sysfs/group.c

h止 sysfs_create_아oup(struct k야）忙Ct 旅的j,
                        const struct attribute_group *grp)
{
        return internat_create_group(kobj, 0, grp);




    커널연구회佃째째／.kerne比z)                                               정재준（rgbi3307@nate.com)
                                           226/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                            kobj ect 이해



}
EXPORT_SYMBOL_GPL(sysfs_create_gioup);



리눅스 파일시스템에 대해서는 아직 진도가 나가지 않았기 때문에 如히ect 소스 설명은 이 정도로

하겠습니다. 좀더 자세한 내용은 앞으로 계속 진행될 예정입니다. 그리고 리눅스 커널을 분석할따1

위와 같은 커널 API 함수들의 사용법을 알아가는 것도 중요합니다. 커널 API 함수들은 이미 잘

만들어져 있기 때문에, 우선 이것을 사용해 보고 쓰임새를 파악한후에 해당함수 내부로 들어가서

자세히 분석하는 방법으로 접근하는 것이 좋습니다. 위에서 설명한 k야）忙CL 을 다루는 커널 API

함수는 k야加ct_create_and_add() 함수와 sysf乞口eateU아oup() 함수입니다． 앞에서 설명

했습니다만, kobject_createmand_add() 함수를 통해서 如bject 을 만들고 이것을

sysfs_creat已.group() 함수로 전달하여 리눅스 파일시스템인 sysfs 와 연동합니다． 여기서 sysfs 와

연동하여 사용하는 방법이 중요합니다. 이것을 확인해볼 수 있는 소스가

"sam아es/ko可edt/k야玎ect-exampLe.c" 입니다. 리눅스 커널 소스에 있는 내용입니다． 이 소스는

커널 모듈로 만들어져 있기 때문에 모듈로 빌드하여 단독으로 테스트할 수 있습니다．


지금까지 내용을 어느정도 이해 하셨다면 " san巾[es/k야기ect/k야玎ect-exam이e.c" 소스를 보면 좀더

확실히 如bject을 실습할 수 있습니다. 커널 모듈 프로그램이므로 커널 모듈로 삽입하여 결과를

확인할 수 있습니다. 혹시, 커널 모듈 프로그래밍에 대해서 익숙하지 않다면 앞에서 설명한 "커널 모듈

프로그래밍"를 다시 참조하시기 바랍니다．


이제 " sampLes/k야）ject/k야）jecL-example.c" 을 실습하1 보도록 하겠습니다. 먼저 如bject-

exam아e.c 에 있는 exam하e_init() 함수부터 실행되므로 이것부터 보도록 하겠습니다．


叫伊mptejnit() 함수

static struct kobject *example1kobj;




    커널연구회佃ww.kerneLb기                                  정재준(rgt焰和7@nate.com)
                                       227/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                       kobj ect 이해




stati이毗 _init exam하인nit(呵d)
{
        mnt retva卜，


        exan耳艇_kobj = k야加ct_create_帥d_add("kobject_exan갸）le", kerne나obj);
        if (!exampLe_kobj)
                 return -ENOMEM;


        / Create the files associated with this kobject 央1
        relvat = sysfs_create_group(exampte_kobj, &attr_group);
        if (retval)
                 kobject_put(example_kobj);


        return retva卜
}


위 함수를 보면 如이ectcreate_and_add(）와 sysfs_create_gioup(）이 실행됩니다. 먼저

如bject_create_a nd_add() 함수에서 " 如bject_exam이e "라는 이름으로 k야玎edt 을 만들고 그

결과（k야玎ect 포인터）를 exam이e_kobj 변수로 받습니다. 이것을 다시 sysfs_create_group()

함수에 전달해서 sysfs 에 연결합니다 ．이렇게 하면 如
                              "kobject_exam이e 라
                                             "는 이름으로 만들어진

如bject는 리눅스 파일시스템 경로 " /sys/kerne나e可ect_example "에 표출 됩니다． 바로 이부분이

중요합니다. 리눅스 커널안에 있는 객체(kobject）가파일로 표출된다는 것입니다. 이렇게 되면 커널

밖에 있는 사용자는 파일을 통해서 커널안의 객쳬（kobject）에 데이터를 읽고 쓸수 있게 됩니다．

커널의 특정 데이터에 접근할 수 있는 통로가 생기는 셈입니다. 그리고 sysfs_create_group()

함수에두번째파라미터로전달하는＆attr_group은 "/sys/kernel/k야기edt_exam이e " 파일경로

안에 생성하는 파일들의 종류와 속성을 정의한 구조체 주소입니다．




    커널연구회佃쌔쌔／.kerrie나江）                                           정재준（rgb13307（回nate.com)
                                            228/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                           kobject 이해



恥tr_group 속성 쿠益쳬1

tatic mnt foo;
static mnt baz;
static mnt bar;


static struct kobj_attribute foo_attribute =
                    _ATTR(foo, 0664, foo_show, foo_store);
static struct kobj_attribute baz_attribute =
                    _ATTR(baz, 0664, b_show, b_store);
static struct kobj_attribute bar_attribute =
                    _ATTR(bar, 0664, b_show, b_store);




"/sys/kernel/k야기ect_exam이e" 경로 안에는 foo, baz, bar 3 개의 파일이 생성됩니다. 그리고 이

파일（foo）의 내용을 조회하면 foo_show() 함수가 실행되고, 내용을 쓰면 foo_store() 함수가

실행됩니다. 이 함수들은 다음과 같이 정의되어 있습니다．



fo아sho놔仇 知乞store() 함수

sta匕口引z目上 向o_show(struct k야）忙ct 出kob工 struct k야）j_attribute 怡比r, char 싸）uf)
{
                                   , /／결과를확인하7t 위하因 추가합
         口rjni아" Foo叫show伽今써＼n", 陌이．
         return sprintf(buf, "%d\n", foo);
}

static ssize_t foo_store(struct kobject *kobj, struct kobj_attribute *attr, const char *buf, size_t
count)
{
         m)t ret;
         ret = kstrtoint(buf, 10, &foo);
         if (ret < 0)
                    return ret;




    커널연구회佃쌔쌔／.kerne比z)                                                    정재준(rgbi330기＠nate,com)
                                               229/ 351
                                                               리눅스 커널 소스 해설 ［기초입문］
                                                                         kobj ect 이해



            p乙泊陌（"向o_store0: 9欲八n', foo); /／결과를확인하기 위해서 추7暳
            return count;
}


위의 소스 내용에서 pr_info()는 제가 결과를 확인해 보기 위해서 추가한 것입니다. 자 이제 지금까지

설명한 커널 모듈 소스（"sam이es/k야玎ect/k야）ject-exampie.c"）를 다음과 같이卜4akef lie 을 만들고

빌드 합니다．



MakefiLe

obj-m := kobject-example.o


alt:
            make -c /lib/modules/$(shelL uname -r)/bui(d M=$(PWD) modules


clean:
            make -c /lib/modutes/$(shetl uname -r)/build M=$(PWD) clean




빌드하여 생성한k야）ject-exa m이e.ko파일을 커널에 삽입(insmod) 한후. "/sys/kernet/" 경로를

보면 " 如bject_example" 경로가 만들어져 있는것을확인할수있습니다．



"/sys/kerneL/" 켱로 내용

jungjaejoon@HP7100U:/sys/kernei$ LI


/／다음과 같이 화면에 표시 됩니다．
drwxr- xr- x 14 root root 0 1 월 25 09: 25 .1
dr- xr- xr- x 13 root root 0 1 월 25 09: 25 . .1
drwxr- xr- x 2 root root 0 1월 25 09: 25 boot_params!
drwxr- xr- x 2 root root 0 1월 25 09: 25 cgroup/
drwxr- xr- x 3 root root 0 1월 25 07: 08 config!




       커널연구회（www.kerneL.bz)                                               정재준（rgb1330기＠nate.com)
                                             230/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                             kobj ect 이해



drwx         39 root root 0 1월 25 07: 08 debug!
 -r- -r- -r  1 root root 4096 1월 25 09: 25 fscaps
drwxr- xr- x 2 root root 0 1월 25 09: 25 iommu_groups/
drwxr- xr- x 32 root root 0 1월 25 09: 25 irq!
             1 root root 4096 1월 25 09: 25 kexec_crash_loaded
 -rw- r- -r  1 root root 4096 1월 25 09: 25 kexec crash size
 -r- -r- -r  1 root root 4096 1월 25 09: 25 kexec_loaded
drwxr- xr- x 2 root root 0 1월 25 09: 25 kobject_example!
drwxr- xr- x 2 root root 0 1월 25 09: 25 livepatch!
drwxr- xr- x 7 root root 0 1 월 25 09: 25 mm!
/／이하 섕략．.




"/sys/kernel/kobject_exampLe" 경로 안에는 다음과 같이 foo, bar, baz 파일이 생성되어 있습니다．



"在ys/kerneL/ko的ect_e始m이可켱로 내魯：

jungja이oon(흐川P71 00U:/sys/kerne꺄야加ct_example읽1
/／댜음과 같이 화면에 표시 됩니다．


drwxr- xr- x 2 root root 0 1월 25 09: 25 .1
drwxr- xr- x 14 root root 0 1 월 25 09: 25 . .1
-rw- rw- r- - 1 root root 4096 1 월 25 09: 28 bar
-rw- rw- r- - 1 root root 4096 1 월 25 09: 28 baz
-rw- rw- r- - 1 root root 4096 1 월 25 09: 28 foo




이제 지금까지 설명한 내용을 확인 하도록 하겠습니다. foo 파일의 내용을 다음과 같은 리눅스

명령어로 화면에 출력합니다. foo 파일의 소유자는 root 이기 때문에 root 권한으로 실행 합니다．



向O 파일：내용 읽기

$ su root


# cat foo
0




    커널연구회佃쌔시／.kerne比z)                                  정재준（rgb13307（흐）nate.com)
                                    231 /351
                                                  리눅스 커널 소스 해설 L기초입문］
                                                            kobj ect 이해




0 이 출력 되었습니다. 그리고 이번에는 다음과 같은 리눅스 명령어로 foo 파일에 ]00 올 쓰넣습니다．


foo 파일 내용 쓰기

# echo 100> foo




실행 결과는 다음과 같은 리눅스 명령어로 " /vai/log!syslog" 파일의 내용을 확인합니다．




# tail /var/log/syslog
/／다윰과 같아 화면에 盈사 됩니다．
/／중간생략，,
Jan 25 09:37: 41 HP7100U kernel: [ 8931.175137] foo_show() : 0
Jan 25 09: 38: 57 I-IP7100U kernel: [ 9006. 791248] foo_store() : 100



위의 실행 결과에서 확인할 수 있듯이, foo_show(）와 foo小就아e() 함수는 커널안의 함수이고 그곳에

있는 foo 변수를 커널 밖에 있는 사용자가 파일을 통해서 읽고 쓸 수 있게 됩니다. 지금까지 내용은

커널의 如bje比 가 sysfs 파일과 어떻게 연동 되는지 모듈 프로그램을 통해서 실습하1 봤습니다． 이것

외에도 kobject는 커널 내부의 여러가지 객체를 구조적으로 연결하는 곳에서 많이 사용됩니다． 특히

댜바이스 드랴이버의 장치 정보에는 대부분 ko너edt 가 있습니다． 아래는 리눅스 커널 소스

' inc山de가inux/cdev.h" 파일에 있는 c由V 구조체 선언부 입니다．


inc佃de八油ux九dev.h

struct cdev {
        struct kobject k毗出
        struct module *owner;




 커널연구회（硏I'阿硝／,k穹rneLbz)                                  정재준（rgbi3307簪nate.com)
                                   232/ 351
                                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                                                1ject 이해
                                                                                              k아：



        const struct fi[e_ope rations *ops;
        struct list_head list;
        dev tdev;
        unsigned mnt count;
} _randomize_tayout;




위의 구조체어匠 ko이ect 구조체（struct k야）忙ctkobj）가 삽입되어 있습니다． 如히ect 는 아래

그림과 같이 다른 구조체 내부에 삽입되어 커널 객체들을 구조적으로 연결하는데 많이 사용되고

그러한 정보들을 sysfs 파일과도 연동하는 중요한 역할을 합니다．


kobject 연결 다이어그램

                                                                                                  卜         如bLt邪宅
                                                                                                    'itfisit 刈III小0們 枷V的C '牡
                                                                                                     ittri批te 0'de似虹多什칡
                                                                                                    t（押日e｝川（)
                                                                                                    d (khll乞ss.ty旴）{}
                                                                                                    升伊m帥ECU)
                          +5打目It UsC如沁 list:
                          i＄如"CI曲批1k此｝,
                          'ttr虹t 心代咐m爪中叩＄！蚣印欲n蜂卦                                                  卜 kset4uavent_ops
                                                                                                    *(1 ci作針 f ii姓r)()
                                                                                                     ' (t Conit M的()
                                                                                                    'I ' C여｝孰 吸nent)()


                                                                                             -p
                                                                                                           如蚊type
                                                                                                    +5押以t 돼its,．叩5 ig朴朽斗簿g + 升St乞叩旺
                                                                                                    'alIt小叭t "del每出L叭計＄,
                                                                   +5tn以 lint   如代
                                                                                                    4(t汁托a＄亡｝( )             4{i5h嘴）{}
                                                                   蛇俑机 曲針       枷蛋斗；                                         +{tit0re}{}
                                                                 . 陌打唯t 王lit 除翡    entry:           4t(!mlld=RL自1倂｝{ )
                                                               // +＄鈿獻 k礎'1吼t      作日rent;          叫'A娜턱好畔｛}
                                        的C苡                   / 呼갔苡t 好m} t甛t      1ntvne:

                                                        /
                              t$t降CC k汁t    斗珏t;            /      姓깠氓I sirens 礪e t$d;
                              托解it ct牡      *5毗’
                                               ，                   ' 5tf吐t好C'   帑瞬；                        kr吐
  .ntrxt kset   斗曳t;          巧tn姓 lint汝州 杯口Y;                                                        m鈿虹I ret長qt瞰，
  !const t批r    枷批；           .str,心 的텨吼t      114rd比
  'S甘虹ti珏L缺韶      en卄Y;       唾計氓tkt히月tyr亡     作t邯凞
  吐truct ke히亡Ct   似r的t;       'stn瞰 kern枉 nede 4s&
  暾rEt 翩bLt解      夕奴叩t;       !str泌tkrtt    kr甘‘，
  珏In心 kern朽_no& ts&
   41tr姓t 如tf   如d:




그림 참조: https://www.smwenku.com/a/5b8aa77e2b71775d1ce851e7/zh-cn




  커널연구회（www.kemet.bz)                                                                               정재준(rgbi3307@nate.com)
                                                        233/ 351
                                    리눅스 커널 소스 해설 ［기초입문］
                                              kobj ect 이해



지금까지는 리눅스 커널 소스의 기초적인 부분을 다루고 있습니다. 아직까지 커널 소스의 여러가지

몸체에 해당하는소스들（아키텍쳐, 스케쥴러, 메모리, 파일시스템, 네트워크, 디바이스드라이버，

등등．.）을 다루지 않고 있지만, 향후 진도가 나가면서 이러한 소스를 이해할때 위에서 언급한 k야加Ct

는 기본 바탕이 되는 객체입니다. 이 글을 통해서 如너edt 의 기본에 대해서 이해하는 계기가

되었으면 합니다． 앞으로 전개되는 내용에서 比bject에 대한 추가적인 내용들은 계속 설명을 하도록

하겠습니댜．




커널연구회佃iww.kerneLbz)                     정재준佃拘i3307@ nate,con寸
                         234/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                      user copy 테스트




user copy 테스트

                             이번글의 주제는 "커널 user copy테스트" 입니다． 컴퓨터

                             메모리는 Os 가 관리해야 하는 중요한 자원입니다. 리눅스를

 Kernel user copy Test       포함한 대부분의 Os는 메모리를 커널이 사용하는 공간과 일반



   Y                         사용자（User）가 사용하는 공간으로 분리하여 관리합니다．

                             커널이 사용하는 메모리와 일반 어플리케이션 User 가 사용하는

메모리 주소가 분리되어 있습니다. 그래서 일반 User들은 보안상 커널의 허가없이 커널이 사용하는

메모리에 접근할 수 없습니다. 그러나 디바이스드라이버에서는 커널 메모리 내용을 User쪽으로

전달하거나 혹은 User 메모리 내용을 커널 메모리로 보내야 하는 경우가 빈번히 발생합니다. 이와

같은 이유 때문에 리눅스 커널은 다음과 같은 API 함수를 제공해서 커널 메모리와 User 메모리간에

데이터 교환（이동）을 가능하도록 하고 있습니다．



커널콰 User간의 매모리 복사 A끼 哲수듈


  0 get_user()              User 메모리에서 Kernel 메모리로 단순 변수값을 가져옴．

  0 put_user()              Kernel 메모리에서 User 메모리로 단순 변수값을 보냄．

  0 clear_user()            User 메모리 내용을 비움．

  1   copy_to_user()        Kernel 메모리를 User 메모리로 블럭 데이터를 복사함．

  1   copy_from_user()      User 메모리를 Kernel 메모리로 블럭 데이터를 복사함．

  0 strnlen_user()          User 메모리 버퍼의 크기를 가져움．

  1   strncpy_from_user()   User 메모리 문자열을 Kernel 메모리로 복사함．




 커널연구회（ww납／.kerneLb기                                정재준（rgbi3307@nate.com)
                                  235/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                       user copy 테스트



아래 그림［凹은 위의 함수들에 의해서 데이터가 전달되는 방향을 아주 잘 설명하고 있습니다．




                                                           U客（對r
                            Aggi田4出etyr冶$                  S口a（冶

                                                      1

                                     伍恥乳from_user()
                                    帥r叫鞍H舟머n냐＄臂｛}




그림참조：h比PS：加씨N.ibm.com서ev이operworks/Library／나；erne卜memory-access力叱ex.htmL




커널 메모리 주소 이해1

커널에서 제공하는 위의 API 함수들을 사용하기 전에, 커널이 관리하는 메모리 주소에 대해서 잘

이해하고 있을 필요가 있습니다. 메모리 주소는 컴퓨터 아키텍쳐（CPU 종류）마다 조금 다르긴

합니다만, 가장 중요한 것은 메모리 주소가 32 비트인지 64 비트인지 잘 구분해야 합니다． 일반적으로

32 비트 CPU 에서는 메모리 주소도 32 비트이고, 64 비트 CPU 에서는 메모리 주소가 64 비트로

관리됩니다．



저는 x86(32 비트）CPU 부터 메모리 주소를 커널에서 어떻게 관리하는지 설명드리고 64 비트 주소와

비교해 보도록하겠습니다. 32 비트 주소는 커널 소스 " arch/x86/Kconfig" 파일을 보시면 다음과

같이 "卜4emory SpLit"을 설정하는 메뉴들이 있습니다．


5    참고문서 참조



    커널연구회佃ww.kerneLb力                                     정재준（rgb13307回nate.com)
                                 236/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                     user copy 테스트




arch/x86/Kconfig

ch이ce
        prompt "Memory split" if EXPERT
        default VMSPLIT 3G
        depends on X86_32
        mk巾m
        Select the desired split between kernel and user memory.
        /／중간 생략，,
        config VMSPLIT_3G
               boot "3G/1G user/kernel spLit '
        config VMSPLIT_3G_OPT
               depends on !X86_PAE
               bool "3G/1 G user/kernel split (for full 1G low memory)"
        con日gV卜1SPLIT_2G
               bool "2G/2G user/kernel split"
        config VMSPLIT_2G_OPT
               depends on !X86_PAE
               bool "2G/2G user/kernel split (for full 2G low memory)"
        config VMSPLIT_1G
               bool "1G/3G user/kernel split"
endch이ce



con fig PAGE_OFFSET
        hex
        default0xB0000000ifVMSPLlT 3G OPT
        default 0x80000000 if VMSPLIT 2G
        default 0x78000000 if VMSPLIT 2G OPT
        default 0x40000000 if VMSPLIT 1G
        default 0xC0000000
        depends on X86_32




 커널연구회（낚쌔,w.kern이.bz)                                                     정채준（rgbi3307（흐）nate.com)
                                            237/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                               user copy 테스트




위의 메뉴에서 디폴트로 "VMSPLIT_3G" 가설정되면 메모리 주소OxC0000000을 기준으로 상위

주소는 커널이 사용하고 하위 주소는 User 가 사용하는 메모리 주소로 분리 됩니다. 이따1 커널이

사용하는 상위 주소 메모리 크기는 ] GB 가 되고 User 가 사용하는 하위 주소 메모리 크기는 3GB 가

됩니다. 아래 그림은 이것을 시각적으로 잘 설명해 주고 있습니다．



32 벼트川모라 蜘S杜fl뇨3G

                              net men伯ry
                               (IG勘
                                              OxC0000000




                                               PAG廷 OFFS目丘0xC000介的｛1
  了ASK 斜ZE＝缸c006的00
                                                (L아Yer boundaikemel space)
  (Upper枷油tofu客針，space)




                                              Ox00000000

그림참조：http://www.eecs harvard edu/-csl 61JcLasswork/incLass-dai3.htmI



그러나 x86 64 CPU 는 메모리 주소를 64 비트로 관리하기 때문에 위의 방식과는 다르게 분리

합니다. 일단, 32 비트 주소에서 메모리의 최다1 크기는 4GB 이고 64 비트 주소에서 메모리 최대

크기는 ]6EB(exabytes）으로 엄청 크기 때문에. 64 비트에서는 커널과 User 간 메모리 주소 분리를

32 비트 방식과는 다르7朴 합니다．



리눅스 커널에서 64 비트 메모리 주소를 관리하는 방식에 대해서는 커널 소스 문서

"/Documentation/x86/x86_64/mm.txt"에서 아주 잘 설명하고 있습니다．




커널연구회（小쌔째／.kern힌.bz)                                          정재준（rgbi3訌刃＠nate.con分
                                      238/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                              user copy 테스트




64 비트 User 메모리 공간 주소


     Start addr           Offset              End addr        Size


  oee88680eeeeeeee        B              e800lfffffffffff     王28 TB


       eaeeeeesees      +128       TB    ffff7fffffffffff    -iBM TB




64 비트 User 메모리 공간 주소는 Ox0000000000000000 번지에서 人 작해서 0x00007fffffffffff

번에서 끝나는 128TB 공간은 user-space virtual 메모리입니다. 그리고 0x0000800000000000

번지에서 시작해서 0xffff7fffff11f1ff 번지에서 끝나는 싸］6卜/1 TB 공간은 커 널 매핑을 위한

비정형적인（non-canonical) vir山at 메모리 입니다. 그리고 커널이 사용하는 64 비트 주소는 다음과

같이 0x阡阡800000000000 번지부터 시작합니다．



64 비트 커널 메모리 공간 주소


      Start addr          Offset              End addr         Size       I
                                                                          i


   f f ffBe889eBee今eB   -128       TB    ffffa7ffffffffff          8 TB
   ft f f88868B880B98   -120       TB    ttft887fffffffff      B . 5 了B
   ff f f888888念88808   甘119 . 5   TB    ffffc87fffffffff       64 丁B
   ffffc889B06BG888      中55 . S   TB    ffffc8ffffffffff      8. 5 TB
   ffffc9808BBBBBBO      戶55       了B    ffffe8ffffffffff        32 了B
   ffffe9a880888888      그3        TB    fftfe9tfffffffff          1 了盈
   ffffea88888B0888      그2        TB    ffffeaffffttff ft         iT露
   ffffebeeeB888eee       그1       丁B    ffffebffffffffff          1 丁B
   f ft fec80888包G888     -28      了B    fffffbffffffffff        16 了B




 커널연구회（蜘／＼사．
           卜erneLb기                                          정재준（rgbi3307@riate.com)
                                        239/ 351
                                                                      리눅스 커널 소스 해설 ［기초입문］
                                                                             user copy 테스트


아래는 64 비트 메모리 주소 공간을 필자7F 전체적으로 다시 요약 정리한 것입니다．

64 비트 메모리 주소 공간

     蜘枉             address-i               address+1          引ze       d增ts
아     간64 0Xf下FF F사干 FF拜 FFFF
      가63     淑TFFF FFFF_FFFFFFFF     Ox8毓也毗1 俄n 娥目             RE

      和60     0船FPF FFFF FEFF FFFF    0x1000 的毓L蜘 oc｝往（}        IF     iC｝珏a   백藎



      2       Ox｛珀｛好 汗下F .FFFF FFFF   初吐脚卜I 00傑｝ 的｛珀 0000       1P     lOA15   芯玉

48 2"48                FF FFFF FFFF   Ox0目l 0薑0 0000 0000      2弱I
      少4?                             0xO어)0 S000 0000 0朕X}    128T
      2嚼！
        ，쿄                            0x00｛珌 4000 0000 心0的     64
      尹45                             0喊麟好4斟目 ()(XX} 0000      32下
      2A44    Ox旣乂好 湃FF FFFF Fl       0妓賦刃 1000 （刃000000       16T


      2A
      가40     0x｛好（好 浿｝FF FFFF FFFF   0城目
                                        （目 01           0000    11     1（少珏    윌丕




 32 沙32 0x的羽多明刃 FFFF FFFF             0x0000 DOC｝王 00000000
      231                             0奴X珣（), 0000 會000 0000    2G
      2A30                            0x照y的 ()000 4000 0000    1G      iC｝岬    십억
      갇'29                            0x0CX均뇨0000느X賦냐胱目        512M
      沙28     a妊薑均00000 心萍F FFFF      ox0000 0C以i ｝航目 () 00    256M



      2 '24   0x浚｝000(｝的 的FF FFFF     缸0000 0000 0100 0000     16M     10嶝     빈建｝




 16   2A16   000             FFF下     0烈）000 （刃00 0001 0       64K
      2"1.5                                                    32K
      2 '14                                                    16K
      2A13                                                      8K
      가12 0x0000 0｛重｛}{}0000 0f芋F     （次（刃00000000凹 1000        4K

      2"l0 小好000_0000000Q03FF         0dAX好 {)OC目 ()00004茯｝    1K      10心     일전

      2A8     0x0000 0000 0000 00FF   0x0000 0000 汶00 0100     256


 0    2怜      0                       0x伎00 0000 00薑｝ 0001      I




커널연구회C'사叭／w.kern畝,bz)                                                          정쟤준(rgb13307｛孕na te.com)
                                                240/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                              user copy 테스트




커널에서 메모리 관리하는 부분은 프로세스 스케쥴러와 함께 Os 의 핵심이고 다루어야 하는 내용들도

많아서 나중에 따로 공간을 마련해서 기술할 예정입니다. 위에서 언급한 메모리 주소는 커널 공간과

User 공간에서 어떻게 분리하여 사용하는지 정도만 알고 넘어 가도록 하겠습니다．




메모리 user copy실습

자 이제 이번글의 본론으로 들어 갑니다. 서두에서 언급한 "커널 user copy"를 위한 API 함수들에

대해서 실습하도록 하겠습니다. 커널 소스 " Li b/test_user_copy.c" 을 보면 모듈로 프로그래밍 되어 있는

코드가 있습니다. 이 소스를 가지고 테스트한 결과를 설명 드리겠습니다. 커널 소스 버전은 "v4.20.5"

입 니 다．



커널 모듈 소스를 빌드 및 실행하는 방법은 "커널 모듈 프로그래밍"에서 이미 기술 했으므로, 이번글은

소스 코드를 설명하는 방식으로 진행 하겠습니다．




이 소스의 제일 상단에 있는 매크로 정의부터 보겠습니다．




Ub/t也St呼沁r Co

#if BITS_PER_LONG == 64 11 (!(defined(CONFIG_ARM) && !defined(MMU)) &&\
                       !defined(CONFIG_M68K) &&          \
                       !defined(CONFIG_MICROBLAZE) && \
                       'defined(CONFIG_NIOS2) &&         \
                       !defined(CONFIG_PPC32) &&         \




 커널연구회（螂시／.kerne나）z)                                            정재준（rgb日307@nate.com)
                                        241 /351
                                                     리눅스 커널 소스 翊설 [기초입푼］
                                                            user copy 테스트



                          !defined(CONFIG_SUPERH))
#define TEST 1J64
#end汗


#define test(condition, msg)          \
({                                    \
        mnt cond = (condition);       \
        if (cond)                     \
                pr_warn("%s\n", msg); \
        cond;                         \
})


위의 매크로 에서 미TS PER LONG == 64 가 정의 되어 있으면 TEST_U64 를 정의하여 64 비트

데이터 타입에 대해서도 테스트가 되도록 합니다．



#define test(condition, msg) 매크로는 con（址向n 에 전달된 값이 0 이 아니면 p乙warn("%s\n",

msg);에서 메세지를 출력합니다. 즉, 이 매크로는 리턴값을 condition 에 전달하여 0 이 아니면

기대하지 않은 오류값이라 판단하여 msg 에 전달한 문자열을 화면에 출력하는 역할입 니다．



"Lib/test_user_copy.c" 소스의 메인 함수는 testJS아_copy_init() 입니다． 이 함수는

modute_init(test_use乙copy_m it)에 전달하여 커널 모듈이 삽입되어 실행될따1

test_user_copy_init() 함수가 실행됩니다. 그럼 test_usei_copy_ini t() 함수안에 있는 코드들을

순서대로 설명 하겠습니다．



먼저 테스트 하고자 하는 메모리를 원하는 크기만큼 할당하는 코드 입니다. 이 코드가 가장 중요한

부분입니다．




 커널연구회（www.kerneLbz)                                     정쟤준(r的i3307回nat包corn)
                                          242/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                   user copy 테스트




tib/test_user_copy.c 메모리 할당

     kmem = kmaLtoc(PAGE_SIZE * 2, GFP_KERNEL);
     iF (!kmem)
            return -ENOMEM;


     user_addr = vm_mmap(NULL, 0, PAGE_SIZE * 2,
                      PROT_READ I PROT_WRITE I PROT_EXEC,
                      MAP_ANONYMOUS I MAP_PRIVATE, 0);
     if (user_addr >= (unsigned long)(TASK_SIZE)) {
            pr_warn("Failed to altocate user memory\n");
            kfree(kmem);
            return -ENOMEM;

     }


위의 소스에서 kmalLoc() 함수는 메모리를 커널 주소 영역에 할당하고， vm_mmap() 함수는 User

영역에 메모리를 할당합니다. PAGE_듸ZE 는 4096 이므로 (PAGE_SIZE 火 2) 한 크기만큼 메모리가

할당됩니다. kmem 는 kmalloc() 함수에서 할당된 커널 메모리 주소입니다. use口addr는

vm_mmap() 함수에 의해서 할당된 User 머1모리 주소 입니다 ．저는 이 주소들을 다음과 같은 코드를

삽입하여 확인 했습니다．




메모리 주소 확인（추가한 코드）

     ///PAGE小SIZE=4e96, TASK小SIZE=Ox00007ffffffff000
     pr_info("PAGE_SIZE=%lu, TASK_SIZE=0x%0161x\n", PAGE_SIZE, TASK_SIZE);


     I/ /TASK SIZE      : Ox00007ffffff ff000
     ///kmem            =0xffff8b921c582000
     I/ /user addr      =0넜薑珣07fc0628230眺｝
     pr_info("kmem=ox%0l 6tx, user_addr=0x%016tx\n", kmem, user_addr);




 커널연구회佃쌔쌔／.kerne나）기                                            정재준(rgbi3307@nate.com)
                                         243/ 351
                                                             리눅스 커널 소스 해설 ［기초입문］
                                                                    user copy 테스트




저는 x86_64 Cpu 에서 실행했기 때문에 주소가 모두 64 비트로 출력 되었습니다. 주소의 위치를

보면 kmem 의 주소는 Oxf仟昭b921c582000 으로 커널 영역이고 user addr 의 주소는

 0x00007fc062823000 으로 User 영역의 메모리 번지임을 알 수 있습니다．



이것 다음으로 이어지는 소스들은 위에서 할당한 메모리 주소에 대해서 데이터를 쓰고, 읽고. 비교하여

 그 결과출 확인하는 코드들입니다．



 m모리 태스트 코드

      memset(kmem, 0x3a, PAGE_SIZE * 2);
      ret 1= test(copy_to_user(usermem, kmem, PAGE_SIZE),
               "legitimate copy_to_user faiLed");
      memset(kmem, OxO, PAGE_SIZE);
      ret 1= test(copy_from_user(kmem, usermem, PAGE_SIZE),
               "Legitimate copy_from_user failed");
      ret= test(memcmp(kmem, kmem + PAGE_SIZE, PAGE_SIZE),
               "legitimate usercopy failed to copy data");



 위의 코드는 kmem 메모리 영역을 0x3a 데이터로 채운 다음, copy_to_user() 함수를 사용하여

/ kmem 메모리 영영의 데이터를 usermen) 메모리 영역으로 복사합니다． 그런다음，kmem 메모리

영역은 OxOO 으로 채우고, copy_from_user() 함수를 사용하여 usermem 메모리 영역의 데이터를

kmem 영역으로 복사합니다. 그런다음 memcmp() 함수를 사용하여 kmem 메모리 영역안의

데이터들이 모두 같은지 비교합니다. 커널 메모리 공간과 User 메모리 공간간에 copy_to_user()

함수와 copy_from_user() 함수가 정상적으로 실행 되었다면 데이터가 모두 동일하므로 "

Leg滋mate userc이玎 fa珏ed to copy data " 메세지는 출력되지 않습니다．




 커널연구회（叫／
        ＼以ernel.bz)                                              정재준（rgbi3307@nate.con寸
                                        244/ 351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                       user copy 테스트




그리고 이 코드 다음으로 이어지는 소스는 아래와 같은 매크로 입니다．




te璘幽egit()，째1크로청의 코드

     #define test_legit(size, check)                                             \
    do {                                                                   \
            vaL--##size = check;                                           \
             ret 1= test(put_user(vaL_##size, (size _user *)usermem工 \
                 "Legitimate put_user (" #size ") failed");                \
             vaL_##size = 0;                                               \
             ret 1= test(get_user(vaL_ 川fsize, (size _user *)usermem), \
                 "legitimate get_user (" #size ") faiLed");                \
             ret 1= test(val_##size != check,                     \
                 "Legitimate get_user (" #size ") faiLed to do copy"); \
             if (vaL_##size!= check) {                                     \
                       pr_info("ox%Llx != Ox%LLx\n",                       \
                               (unsigned Long Long)vaL_##size,                   \
                               (unsigned long Long)check);                 \
             }                                                             \
    }whiLe (0)




이 매크로 정의에 의해서 컴파일러는 te就_Legit(u8, 0x5a);를 다음과 같은 코드로 치환 니다．




雄就J的i的 때크로 치환 코드

     do{                                                                   \
             val_u8 = check;                                      \
             ret= test(put_user(vaL_u8, (size _user *)usermem), \
                 "Legitimate put_user (" u8 ") faiLed");          \
             vaL_u8= O;                                                    \




 커널연구회（邸I'사．kerne나파                                                        정재준（rgbi3307@nate.com)
                                             245/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                        user copy 테스트


              ret= test(get_user(vat_u8, (size _user *)usermem), \
                  "legitimate get_user (" u8 ") faiLed");          \
              ret= test(vaL_u8 != check,                           \
                  "Legitimate get_user (" u8 ") failed to do copy"); \
              if (val_u8!=check) (                                 \
                        pr_info("Ox%Llx= Ox%Llx\n",
                                  (unsigned long Long)vaL_u8,
                                  (unsigned Long long)check);
              }
      加씨［e (0)




val_u8 = check; 는 vaL_u8 변수에 0x5a 의 값을 넣고 put_user(val_u8, (size _user 火沁sermem)

함수를 호출하여 vaL u8 변수안의 값인 0x5a 올 User 메모리 영역인 usermem 로 전달합니다．

그런다음，get_user(vaL_u8, (size _user 士）usermem) 함수를 실행하여 usermem 주소에서 이

값을 다시 가져옵니다. 이 값이 Ox5a 가 아니라면 put_user(）와 get小user() 함수가 정상적으로

실행되지 않은 결과이므로 " Le이timate get_user (" u8 ") failed to do copy" 라는 메세지가

출력되고，데이터가 어떻게 다른지 각각의 값들을 아_info () 함수를 사용하여 출력합니다．

put_user(）와 get_user() 함수가 정상적으로 실행 되었다면 아무런 메세지도 출력되지 않습니다.



아래 코드들도 위와 같은 방식으로 매크로 치환되어 실행됩니다．



      test_Legit(ul 6, 0x5a5b);
      test_Legit(u32, 0x5a5b5c5d);
      test_Legit(u64, 0x5a5b5c5d6a6b6c6d);




커널연구회佃쌔iw.kerneL.bz)                                                     정재준（rgbi3307芯）nate.com)
                                             246/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                 user copy 테스트



각각의 데이터 타입（u8, u16, u32, u64）에 있는 값을 put_user() 함수를 사용하여 User 메모리에

보냈다가 get_user() 함수를 사용하여 다시 가져온 데이터가 다르다면 오류 메세지가 출력됩니다．

문제없이 정상적으로 실행되었다면 아무런 메세지도 출력하지 않습니다．



그리고 나머지 이어지는 코드들도 지금까지 설명드린 방식과 비슷하게 테스트 되는 소스들이므로

쉽게 이해하실 수 있습니다．



지금까지 기술한 "커널 user copy 테스트" 내용은 리눅스 커널에 디바이스드라어버를 작성할때1 많이

활용할 수 있는 코드들입니다. 앞으로 많이 사용해 보시기 바랍니다. 그럼 이번 글은 여기서 마무리

하도록 하겠습니다．




 커널연구회（艸쌔／.kerne나玘）                              정재준（rgbi3307@nate.com)
                              247/ 351
                                        리눅스 커널 소스 해설 ［기초입문］
                                               list sort 테스트




list sort 테스트

                       이번글 주저七 "커널 list sort 테스트" 입니다. 리눅스 커널

                       소스에서 linked List 는 가장 중요한 자료구조 입니다. 커널에서

                       취급하는 대부분의 자료들은 Linked List 로 연결됩니다. 따라서

                       커 널 소스를 이해하는 과정은 Linked List 로 연결된 자료구조룰

                       이해하는 과정이기도 합니다. 그런데 커널 소스를 분석하다 보면

                       데이터 구조체들이 너무 많고 복잡해서 List 연결관계가 잘 보이지

않는 경우를 많이 경험하게 됩니다. List 연결관계를 명확히 알고 있지 않으면 데이터 구조체들의

분량에 압도 당해서 더더욱 소스를 이해하기 힘듭니다. 다행히, 커널 소스에 구현되어 있는 Linked

List 는 매우 간결합니다. C 언어의 포인터 연결관겨를 잘 알고 있으면 Linked List는 이해하기

쉽습니다. 양방향으로 연결된 next와 prey 포인터 2 개를 따라가면 됩니다. 그런데 이 글에서는

Linked List 소스를 자세히 설명하지는 않습니다. 리눅스 커널에서 이것을 어떻게 사용하는지

활용법에 초점을 맞추어 설명합니다．



Linked List 전체 소스가 궁금한 독자분은 필자가 집필한 아래의 책을 참고해 주시기 바랍니다. Linked

List 을 포함한 리눅스 커널 자료구조 알고리즘에 대해서 소스를 자세히 설명한 책입니다．




커널연구회佃쌔쌔／.kern이，bz)                          정쟤준（rgb13307芯）nate.com)
                            248/ 351
                                                          리눅스 커널 소스 해설 ［기초입문］
                                                                 Ust sort 테스트



                                     .   커널연구회 쇼핑몰：
          5칸｛心갸1了 Fd,f, 也，;

                                     0 https://www.kerneL.bz/product/bookl 1
   끄뉵寸二，기닐 자료구조
   알고리즘 상세분석2
                       山 ；亡．
                           兄t熙j. r   .   알라딘：

                                     0 https://www.aLadin.co.kr/shoD/wproduct.aspx?

                                         ItemId=126260838



                                     0   교보문고：

                                     1   h比p:/加1W比ky야m加야.co.kr




커널 Linked List 기帽

위의 책에서 소스를 자세히 설명하고 있습니다만. 커널에서는 Linked List 로 연결된 포인터룰

사용하여 아주 특별한 방법으로 데이터 구조체 멤버에 접근하는 포인터 연산이 있습니다. 이 포인터

연산을잘 알고 있어야합니다. 이것은 O仟setof매크로로 커널 소스 "include/Iinux/stddef.h"

파일에 다음과 같이 정의 되어 있습니다.（커널 소스 버전：v4.20.6)



        油ux加닙del.h

#undef offsetof
#ifdef 1 compi1er_offsetof
#define offsetof (TYPE, MEMBER)           _compiler_offsetof (TYPE, MEMBER)
#else
#define offsetof (TYPE, MEMBER)           ( (size_t) &( (TYPE *)o) ->MEMBER)
#endif




 커널연구회（的／w.kerneL.bz)                                             정재준(rgbi3307@nate.com)
                                           249/ 351
                                                              리눅스 커널 소스 해설 [기초입문］
                                                                     Ust sort 테스트



아울러 커널 소스 "力ndude/tinux/kerne나l"에 정의 되어 있는 containe口of 매크로도 같이

이해하고 있어야 합니다．

越｝＜鈿d節蜘沁x/蛇mel
                                                                                       \\
#define container_of (ptr, type, member) ({

                                                                                    \\   \
        void *1 mptr = (void *)(ptr) ;
        BUILD_BUG_ON_MSG(! _same_type(* (ptr) , ( (type *)O) ->member) &&
                                                                                      1\
                          I_ same_type (* (ptr) , void) ,
                          "pointer type mismatch in container_of () ") ;
        ( (type *)(1 mptr - offsetof (type, member) )); })



위의 container of매크로는 아래 그림에서 잘 설명하고 있습니다. container_of 매크로에

전달하는 세개의 파라미터들에서 ptr 은 구조체 멤버의 포인터입니다． 그리고 type 은 ptr 이

포함되어 있는 구조체의 데이터 타입이고 member는 ptr 포인터의 데이터 타입 명칭입니다．



 container_of (ptr, type, member)
                           illustrated ex미anat아｝




壯t可／1끼V뵤y뵤linux.忙1LC口r了l




 커널연구회（附쌔／.kern이.bz)                                              정쟤준（rgbi3307@nate.com)
                                                   250/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                               list sort 테스트



2림출처: https://tinuxweR.wordpress.com/201 2/11/10/magicaL-container pf-macro/


위의 그림에서 설명하고 있는 container_of 의 사용예를 코딩하면 다음과 같습니다．



C帥聯nar_of샤용畔

struct object {
      char first_ member;
      char second_member;
      char third_member;
      char list_ head list;
}
struct list_ head士 ptr = ／出 ... 火／
struct object* ret;
ret = container_of (ptr, struct object, list) ;



위와 같이 containe乙of 는 연결 리스트에서 가르키고 있는 ptr 의 주소를 알면 이것이 포함되어 있는

굿조체의 시작（base）주소를 가져올 수 있습니다. 커널의 Linked List 에서 cont키ner_of는 아주

중요한 역할을 합니다. 이것 때문에 Linked List의 포인터 연결 관계는 아주 간결합니다 ．커널의

"incLude/Linux/types.h" 소스 파일에 선언되어 있는 Linked list 구조체는 next 와 prey 포인터

두개만을 멤버로 가지고 있는 아주 간단한 구조 입니다. 이것으로 구조체들을 앞뒤 양방향으로

연결합니다．



        List꾸조체

struct list_ head {
         struct list_ head *nextr *prev;
};


아래 그림은 커널의 Linked List 연결 관계를 그림으로 잘 설명하고 있습니다．




    커널연구회（蜘,w.kerne比z)                                          정재준（rgbi3307@nate'com)
                                       251 /351
                                                                       리눅스 커널 소스 해설 ［기초입문］
                                                                              Ust sort 테스트




                               data structure 1            d求as打ucture 2              data structure 3


                                                                                       list head
      ii就 head                                                                            next
                                                                                          prey




      (a) a doubly linked listed with three elements




                                             (b) an empty doubly linked list
                                                                               円ad                       ]
그림참조：htt社끄畝岫rofe.g北hub.i毗均就s/dou벼ylist



위와 같이 커널의 Linked List는 구조체들（data structi, 2, 3）안의 멤버 구조체로 들어가서 next,

prey포인터를 사용하여 앞뒤 양향향으로 연결됩니다. 이때 구조체들（data struc匕，2, 3）안의 다른

멤버들은container of 매크로를 사용하여 가져올 수 있습니다． 지금까지는 커널에 구현되어 있는

linked list 의 개념에 대한 설명 이었습니다. 이제부터는 이글의 본론으로 들어가서 linked List 로

연결된 구조체들을 정렬하는 예제 소스를 설명하고 테스트한 결과를 보여 드리도록 하겠습니다．




커널연구회（的／＼사．kerne나）力                                                                  정재준（rgbi3307@nate.com)
                                                  252/ 351
                                                        리눅스 커널 소스 해설 ［기초입문］
                                                               1.1st sort 테스트



커널 List Sort 예제

커널의 Linked List를 정렬하는 예제는 커널 소스 "Lib/test_List_的比.C"에 이미 포함되어 있습니다．

커널 소스 버전은 필자가 이글을 작성하고 있는 시점에서 최신 버전인 "v4.20.6"입니다. 이 소스

파일은 커널 모듈 프로그래밍 되어 있어서 모듈로 빌드해서 단독으로 실행해 볼 수 있습니다. 아울러

앞에서 설명한 Linked List 을 테스트해볼 수 있는 아주 간결한 예제입니다．



먼저 "Iib/test_List_sort.c"에서 리스트로 연결하고자 하는 구조체 선언부터 보도록 하겠습니다. 아래

소스를 보면 struct debug_el 이 링크드 리스트로 연결되는 작업 대상 구조체입니다. 이 구조체

                                             ，가 링크드 리스트로 연결됩니다．
안에는 멤버가 5 개 있습니다. 이들 중에서 struct list_head Ii就·

그리고 intv키ue 는 이구조체를 순서대로 정렬하는 키로 사용되고, uns垣ned serial 은 이 구조체가

메모리에 할당되는 순번입니다． struct debug_el 구조체가 메모리에 할당되는 개수는

TEST_LIST_LEN 입니다. 이것의 크기가 引2+128+2 으로 정의 되어 있으나. 필자는 테스트 결과를

간단히 확인해 보기 위해서 ]0 으로 수정했습니다．



연크 작업 구芬체선언，

///#d計泊e TEST呻LIST LEN (512+128+2) ／六 not Inc山ding head */
#defineTEST LIST LEN      10


#define TEST POISON1 0xDEADBEEF
#define TEST POISON2 0xA324354C


struct debug_el {
       unsigned mnt poisoni;
       struct list_head List;
       unsigned mnt poison2;




 커널연구회（寸쌔째／.kern빈.bz)                                        정재준（I야月3307（回nate.com)
                                        253/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                     Ust sort 테스트


          mnt value;
          unsigned serial;
｝·，
static struct debug_이 出火el匕 1 initdata;




위와 같이 선언한 구조쳬를 메모리에 TEST 니ST LEN 으로 정의한 개수만큼 메모리에 할당하는

 소스는 다음과같습니다. static struct debug_el *士e比S는 kcalloc(）함수를사용하여

夕zeof(火e比5) 크기만큼 메모리 할당 합니다. 그리고 struct debug_el 火el 은 TEST_LIST_LEN

개수만큼 for 루프에서 이 = kmattoc(sizeof(火el), GFP_KERNEL);으로 커널에 메모리 할당 됩니다．

이따I et-'va山e 멤버변수어七 prandom_u32() 함수에 의해서 난수가 입력되고. el->seri計 = 卜．는

순번이 입력됩니다. 아소스에서 p乙inf이""）는소스코드들이 실행될때마다데이터를확인해 보기

위해서 필자가 추가한 코드 입니다.



구조쳬 El모라丑당

          pr_iafo("list_sort starting...\n");


          elts = kcalloc(TEST_LIST_LEN, sizeof(*elts), GFP_KERNEL);
          if (!elts) return err;


          pr_inFo('before list_sort:\n');
          for (i = 0; i <TEST_LIST_LEN; i++) {
                   el = kmalloc(sizeof(*eL), GFP_KERNEL);
                   if (!eL)
                              goto exit;


                  ／샤orce some equ岫lencie計／
                  el->vatue = prandom_u32() % (TEST_LIST_LEN /3);




      커녈연구회佃쌔n사．kerneLbz)                                             정쟤준（r야)i3307（孕nate.com)
                                                 254/ 351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                       List sort 테스트



                e卜＞serial = 卜．
                e卜>poisonl = TEST_POISON1;
                el->poison2 = TEST_POISON2;
                elts[i] = el;
                List_add_tail(&eL->list, &head);


                pr_info("{%d:%d} ", et->seria[, e卜>va(ue);
       }
       pr_inf이" \n");




위0們 할당된 이 은 List尸add_tail(&e卜＞Li就，&head)；에 의해서 커널의 linked list 에 추가 됩니다．

이때 e卜＞value 값은 임의의 난수 값이므로 linked List 에 추가된 value 값은 순서대로 정렬되지 않은

임의의 값입니다. 이 값을 정렬하는 작업은 아래의 함수 실행에 의해서 이루어집니다
                                            ．



List_sort(NULL, &head, cmp);



list_sort() 함수는 커널 소스 파일 "lib/List_sort.c"에 정의 되어 있습니다 ．이함수에

니ST_HEAD(head);로 정의한 링크드 리스트의 head 주소와 cmp 함수를 전달하면 head 주소부터

연결되어 있는 리스트들을 정렬합니다. 정렬할띠1 비교하는 키는 아래와 같이 코딩되어 있는 cmp

함수 내부에서 la->value - eLb->vaLue 연산한 결과에 의해서 정렬 됩니다．



cmp() 소스

sta匕c mnt _init cmp(void 챠）niv, struct List尸head 出a, struct List小head 出b)
{
        struct debug_el *ela, *elb;


        eta = container_of(a, struct debug_el, list);



    커널연구회佃쌔쌔／.kernel.뇨）                                                     정재준（rgbi3307@nate.com)
                                              255/ 351
                                                                    리눅스 커널 소스 해설 ［기초입문］
                                                                           List sort 테스트



        elb = container_of(b, struct debug_el, list);


        check(ela, elb);
        return ela->value - elb->value;
}


정렬한 결과는 아래와 같이 for 에서 링크드 리스트를 next 로 탐색하면서 출력합니다. 이따I check()

함수로 정렬한 결과가 올바른지 점검하여 문제가 있으면 오류 메세지를 출력합니다．



         ft 겊과 촤인

        pu nfo("after List_sort:\a ');
        for (cur = head.next; cur->next 1.= &head; cur = cur->next) {
                struct debug_el 士e너 ;
                intcn耳乙result;


                if (cur->next->prev != cur) {
                           pr_err("error: list is corrupted\n");
                           goto exit;
                }

                cmp_result = cmp(NULL, cur, cur->next);
                if (cmp_result> 0) {
                           pr_err("error: list is not sorted\n");
                           goto exit;
                }

                el = container_of(cur, struct debug_el, list);
                eli = container_of(cur->next, struct debug_el, list);
                if (cmp_result == 0 && e卜>serial >= ell->serial) {
                           pr_err("error: order of equivalent elements not "
                                   "preserved\n");




    커널연구회（www.kerneLbz)                                                   정재준（rgb13307（흐）nate.com)
                                                256/ 351
                                                                 리눅스 커널 소스 해설 ［기초입문］
                                                                        list sort 테스트



                         goto exit;
                }

                if (check(el, eli)) {
                         pr_err("error: element check failed\n");
                         goto ex七
                }

                pr_info("%d[%d:%d] ", count-i, e卜>seriaL, el->value);
                count++;
       }//for
       pr_info( '%d[%d:%d]\n", count-i, e卜>serial, et->vatue);




위의 소스에서 p乙m l이""）는 소스 코드들이 실행될때마다 데이터를 확인해 보기 위해서 필자가

추가한 코드 입니다. 向I 루프가 실행될띠1 마다 아래 코드가 실행되므로，




pr_info("%d[%d:%d] ", COUnb , el->serial, e(->value);



List_so比（）가 실행되기 전의 e卜＞serial十l->va山e 값과 실행된후에 정렬된 el->va山e 값을 다음과

같이 "/var/log/sys(og" 파일에서 확인할수있습니다．

                      느M (.0O           (;ti커 U目 tt吐 邱g)
싶행 데이터 확인
Feb 19 18: 20:16 HP710引J kernel: [39311.166374] list_ sort_test: list_ sort
starting. . .
Feb 10 18: 20:16 HP7109U kernel: [39311.166379] list_ sort_test: before
list sort:
Feb 10 18: 20:16 HP7100U kernel: [39311.166386] list_ sort_test: [0: 2]
Feb 10 18: 20:16 HP7100U kernel: [39311.166391] list_ sort_test: [1: 2]
Feb 10 18: 20:16 HP7100U kernel: [39311.166397] list_ sort_test: [2: 0]
Feb 19 18: 20:16 HP710引J kernel: [39311.166402] list_ sort_test: [3:1]
Feb 10 18: 20:16 HP7100U kernel: [39311.166407] list_ sort_test: [4: 2]




 커널연구회佃,ww.kerne比z)                                                     정재준（r야)i3307@nate.com)
                                              257/ 351
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                           Ust sort 테스트



Feb 10 18: 20:16 HP7100U kernel:      [39311.166412] list sort test:    [5: 0]
Feb 10 18: 20:16 HP7100U kernel:      [39311.166417] list_ sort_test:   [6:1]
Feb 10 18: 20:16 HP7100U kernel:      [39311.166420] list_ sort_test:   [7: 0]
Feb 10 18: 20:16 HP7100U kernel:      [39311.166424] list_ sort_test:   [8: 0]
Feb 10 18: 20:16 HP7100U kernel:      [39311.1664271 list sort test:    [9: 0]
Feb 10 18: 20:16 HP7100U kernel:      [39311.166430] list sort test:
Feb 10 18: 20:16 HP7100U kernel:      [39311.166440] list sort test:    after
li st sort:


                                                                        0 0 0 0 0 l l 2 2 2 1




                                                                                                                  J ]J mJ ]
Feb 10 18 :20: 16 HP7100U kernel:     [39311.166444] list sort test:




                                                                                                            J =J ]
                                                                                                                 1
                                                                                                                 1
                                                                                                     ]J mJ 1
                                                                                                           1
Feb 10 18 : 20: 16 HP7100U kernel:    [39311.166448] list sort test:
Feb 10 18 : 20: 16 HP7100U kernel:    [39311.166452] list_ sort_test:
                                                                         11 11 11 11 11 11 11 11 11 11 1L
Feb 10 18: 20:16 HP7100U kernel:      [39311.166457] list_ sort_test:


                                                                        2 5 7 8 9 3 6 0 l l S
Feb 10 18: 20:16 HP7100U kernel:      [39311.166461] list sort test:



                                                                        [ [ 1L rL rL [ [ nL nL =L
Feb 10 18: 20: 16 I-IP7100U kernel:   [39311.166465] list sort test:
Feb 10 18 :20: 16 HP7100U kernel:     [39311.166469] list sort test:


                                                                        e l 2 3 4 5 6 7 8 9l          l
Feb 10 18: 20: 16 HP7100U kernel:     [39311.166473] list sort test:
Feb 10 18: 20:16 HP7100U kernel:      [39311.166477] list sort test:                                        O



                                                                                                     1
Feb 10 18: 20:16 HP7100U kernel:      [39311.166482] list sort test:
                                                                                                      mJ ]J S                 八
Feb 10 18 : 20 : 16 I-IP7100U         [39311.166484] list sort test:
succeeded.




지금까지 커널 소스 "lib/test_List_sort.c"에 모듈 프로그래밍 되어 있는 예제를 통하여 list 를

정렬하는 소스를 설명해 드렸습니다. 이 예제는 커널의 linked list 올 이해하고 테스트해볼 수 있는

좋은 예제입니다. 저의 글을 통해서 커널 소스의 뿌리에 해당하는 linked list 을 잘 이해하는데

도움이 되었으면 합니다. 그럼 다음글에서 뵙겠습니다．




 커널연구회佃八사w.kerne나묘）                                        정재준（q兆i3307@nate.com)
                                      258/ 351
                                             리눅스 커널 소스 해설 ［기초입문］
                                                red- bl.ack tree 테스트




red-black tree 테스트

                           이번글의 주제는 "커널 red-black tree 테스트" 입니다．

                           앞글에서 기술한 linked list 와 더불어서 red-t乂ack tree 도

   Kernel red-black Tree   커널에서 중요한 자료구조입니다. linked list는 데이터를
              m




              六戶 "“「「' "「’「「"「「甘"『는’" "「．
                                        "」'red-black""'"
       小叫1=




                  mm       는 데이터를 왼쪽과 오른쪽으로 나누어서 연결합니다．

왼쪽방향으로는 작은 데이터를 연결하고 오늘쪽으로는 왼쪽보다 큰 데이터를 연결합니다. 이렇게

연결하면 데이터를 두가지 방향으로 나누어서 탐색할 수 있어서 Linked List 보다 탐색 효율이

좋아집니다. 알고리즘 효율성으로 나타내면 Linked List 는 O(n）이고 red－바ack tree 는 O(Log2(n))

입니다. 이것을 그래표로 비교하면 다음과 같습니다．



알고리즘 효율성 비교 그래프


  10




                                                       log2 v




                       5                                      20




 커널연구회佃八사니ikern힌.bz)                                 정재준（rgbi3307@nate.com)
                                259/ 351
                                            리눅스 커널 소스 해설 E기초입문］
                                               red- black tree 테스트



위의 그래프를 보면, 가로좌표는 데이터 개수 n 이고 세로좌표는 O(n）으로 표시되는 알고리즘 효율성

（처리시간）입니다. Linked list 는 데이터 개수 n 에 선형적으로 비례하여 O(n）이 증가하는것에

비해서 red寸乂ack tree 는 log2(n) 입니다. log 그래프는 그 특성이 n 값에 대해서 완만하게

증가한다는 것입니다． 즉，n 이 증가할 수록 bg2(n）은 그렇게 크게 증가하지 않습니다. 따라서

처리해야하는 데이터 개수 n 이 크지면 크질수록 red七怡ck tree 의 효율성은 Linked list 보다 월등히

좋아집니다. 그런더I, red寸乂ack tree 가 좋기만 한것은 아님니다. 데이터 개수 n 이 작으면 오히려

Linked 小t 가 더 효율적입니다. 왜냐하면, red七Lack tree 는 왼쪽과 오른쪽으로 트리의 균형을

맞추어 가야 하는 내부 코드가 복잡하기 때문입니다. 이것에 비해서 Linked List 는 단순히 선형적으로

연결만 하므로 내부 코드가 아주 간결히 처리됩니다．



위와 같이 linked List와 red七Lack tree 는 장단점을 모두 가지고 있기 때문에, n 이 수십시수백개

p기가
  " 단위로 비교적 적은 더1이터는 [inked List로 처리가
                                    '고，수백사수천개 이상으로 늘어나면 red-

바ack tree 로 처리합니다. 리눅스 커널도 예외없이 이러한 자료구조 알고리즘 특성안에 있습니다만，

커널만의 특징이라면, linked List 에서 이해하고 계시겠지만 red-늬ack tree 도 데이터를 연결하는 C

언어 포인터 연산을 아주 효율적으로 하고 있다는 것입니다．




red-black tree 이해1

리눅스 커널의 Red-Black Tree 소스는 간결하게 코딩되어 있습니다. 소스 코딩량이 생각보다

적으면서도 아주 효율적으로 "incLude/Linux/rbtree.h"와 "Lib/rbtree.c" 소스 파일에 구현되어

있습니다． 헤더파일인 rbtree.h 와 소스파일인 rbtree.c, 단 2 개의 파일로 Red－미ack Tree 을

구현하고 있습니다. 이 소스에 대해서는 필자가 집필한 아래 책에서 자세히 설명하고 있으니 참조

부탁드립니다．




 커널연구회佃,ww.kerneLbz)                              정쟤준（rgbi3307@nate.com)
                               260 / 351
                                                                리눅스 커널 소스 해설 ［기초입문］
                                                                   red- black tree 테스트




참고 서적


                                            .   커널연구회 쇼핑몰：
               뇨 n가｝OL曲r,o

                                            1   https://www.kerneLbz/product/bookl 1
                      자翟구조
       알고리즘 상세분석2
                             」；:'   1   r   .   알라딘：

                                            1   https://www.aLadin.co.kr/shop/wproduct.aspx?

                                                ItemId=126260838



                                            1   교보문고：

                                            D h比p:J加川比ky야）obook.co.kr



이글은 커널의 Red－미ack Tree 를 활용하는 방법 위주로 내용을 기술합니다. 우선

"include/linux/rbtree.h"에 선언되어 있는 Red-Black Tree 구조체를 확인하고 가겠습니다．



Red-Black Tree 구조체 선언

struct rb_node {
      unsigned long _rb_parent_color;
      struct rb_node *rb1right;
      struct rb_node 出巾left;
} 1 attributem佃的ned（血eof(t帥g))));


struct rb_root {
      struct rb_node *rb node;
};
     커널연구회佃쌔쌔／.kerneLbz)                                                정재준（rgbi3307@nate.com)
                                                 261 /351
                                                       리눅스 커널 소스 해설 [기초입문］
                                                          red-bl.ack tree 테스트




 struct rb_root_cached {
         struct rb_root rb_root;
         struct rb_node *rb Leftmost.
 }’,
 위와 같이 Red-Black Tree 구조체는 간단합니다． rb node 구조체를 왼쪽와 오른쪽으로 연결하는

．포인터와 uns匈ned long 타입의 컬러값만 가지고 있습니다． 위의 rb_node 구조체는 rb_root

 구조체를 기준으로 왼쪽과 오른쪽으로 연결됩니다. Red．미ack Tree 는 커널 태스크 스케쥴링을

 담당하는 구조체에서 많이 사용되므로 아래와 같이 연결되는 과정을 예를 들어 설명해 보겠습니다．



 kernel/닙沁d／恥hed.h

  struct cfs_rq {
            I/I...
            struct rb_root_cached tasks_匕meline;
 }

 incLudejlinux/sched.h

 struct sched_entity {
            I/I...
            struct rb_node     run_node;
            u64                vruntime;
}



위의 cfs_rq 구조체와 sched_en匕ty 구조체는 다음과 같이 vrun匕me 의 크기에 따라서 연결됩니다．

vruntime 이 작으면 Red-Black Tre 의 왼쪽으로 크면 오른쪽으로 연결합니다. 아래 그림은 이것을

잘 설명하1 주고 있습니다．




       커널연구회（wv쌔／.kerne比z)                                  정재준（rgb日307@nate.com)
                                            262/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                    red- bl.ack tree 테스트




艇斗BLack三和a在연켰 그甘


      Cf S rq




            sched enuty             sche心，
                                         ，珝哺ty
                run noce             run no珏e
            ＼叩U趾wne                  vru！姓凋t8




그림출처：h ttp://ww比C이ns.tsukuba.acjp/-yas/coins/os2그009/2009-12-15力ndex.htmt



지금까지 커널의 Red-BLack Tree 가 연결되는 개념에 대해서 간단히 기술했습니다. 위에서 예를들어

설명한 커널 스케쥴러 구조체 연결 및 스케쥴링에 대한 것은 커널에서 아주 중요한 큰 산맥이며

다루어야 하는 내용도 많으므로 나중에 따로 주저匿 마련하여 기술할 예정입니다. 그럼, 지금부터는

이글의 본론인 Re（卞BLack Tree 을 테스트하는 간단한 예제를 가지고 설명 하겠습니다．




 커널연구회佃쌔,w.kernel.뇨）                                   정재준(rgl滔307@nate.com)
                                  263/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                         red- bl.ack tree 테스트



red-bLack tree 실습 0似II

리눅스 커널 소스 "Iib/rbtree_test.c" 파일을 보면 red止丑ack tree을 테스트 하는 소스（버전

v4.20.6）가 있습니다. 커널 모듈로 코딩되어 있기 때문에 모듈로 빌드하여 실행해 볼 수 있습니다. 이

소스에늑 red-비ack tree 에 노드를 삽입，삭제，탐색 할때마다 성능을 테스트하는 코드가 있습니다．

우리는 보통 소스 코드의 실행 시간을 측정할때 cLock_ge比ime() 함수를 사용하여 나노초 단위로

시간을 가지고 옵니다. 그런데 이 함수는 시스템 콜 형태로 실행되기 때문에 이 함수 자체에서 실행

시간이 많이 걸립니다. 그래서 커널에서는 get_cycles() 라는 함수를 사용합니다. 이 함수는 다음과

같이 "/a rch/x86/incLude/asm/tsc.h"에 정의 되어 있습니다. Cpu 종류에 의존되는 코드입니다.

저는 현재 x86 에서 실습하고 있어서, x86 어셈블리 코드 " r北Sc"에서 CPU 사이클을 Un引gned tong

Long 형태의 수치로 가지고 온다는 것을 "/arch/x86/incl미ie/asm/ms사）" 소스 파일의 r(北sc()

함수에서 확인할 수 있습니다．



／카（hi始心月n如d食徊sm在＄

static I씨ne cycles_I日趾_cycles佃이d)
{
#ifndef CONFIG X86 TSC
      if (!boot_cpu小as休86_FEATUR目巧C))
          return 0;
#end汗


      return rdtscO;
}

佃rch/x86加C佃de／鈿rn/rn斑I'

static_always_inLine unsigned long long rdtsc(void)
{


    커널연구회（ww比kerr始L.bz)                                    정재준（rgbi3307（孕nate.com)
                                         264/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                               red- b1.ack tree 테스트



     DECLARE_ARGS(val, low, high);
     asm voLatile("rdtsc" : EAX_EDX_RET(val, low, high));
     return EAX_EDX_VAL(val, low, high);
}


red-black tree 을 테스트할따1 위의 함수를 사용하여 Cpu 사이클을 측정 하므로. 먼저 이 함수를

사용하는 간단한 예제 소스를 다음과 같이 작성 했습니다．




          始하） I쩍已             애斗소소

static void busy_Ioop(u64 iters)
{
        volatile mnt sink;
        do {
               引nk = 0;
        }while (-iters> 0);
        (void)sink;
}

#define LOOPS_CNT (1000 * 1000)


static void run_time_test(void)
{
        u64 timel, time2, t1me3, cycles=0;
        inti;


         printk("run_time_test() Start...\n");
         for (i=0; kb0; i++) {
               timel = get_cyctesO;
               busy_loop(LOOPS_CNT);
                time2 = get_cyctesO;
                time3 = time2-time기




    커널연구회（小쌔쌔／.kernel.bz)                                        정재준(rgbi3307@nate.com)
                                                 265/ 351
                                                                          리눅스 커널 소스 해설 ［기초입문］
                                                                             red- bl.ack tree 테스트



                          cydes += time3;
                          printk("Loop_rdtsc %02d: run_cycLes=%L1u, one caLL%ltu cydes\n",
                                     k-i, t1me3, div_u64(time3, LOOPS_CNT));
                      }
                      timel = div_u64(cycLes, LOOPS_CNT * 10);
                      printk("Loop_rdtsc average: one ca十%如 cycles\n", timel);
                      printk("run_time_test() End.\n");
}


위의 소스에서 busy_Loop() 함수는 LOOPS小CNT 을 전달받아서 뺄셈과 대입 연산을 100 만번

수행합니다． busy_Loop() 함수를 실행하기 바로 전에匕mel = g飢_cyc(es(）을 실행하고，

busy_Loop() 함수 실행이 끝나는 곳에서 匕me2 = g趾_cycles(）을 실행한후, 匕n祀3 = time2-timel

을 실행하여 11me2 에서 time] 을 빼면 time3 은 busy_loop() 함수를 실행하는 동안 소모한 CPU

사이클을 가지게 됩니다. 이 값을 printk로 화면에 출력하여 확인하고，이 과정을 for (i=0; 1<10; k-i-)

안에서 ]0 번 반복합니다. 그리고, for루프가 종료될때는 busy_toop() 함수가 한번 실행되는데

소모한 CPU 사이클의 평균값을 마지막으로 출력 합니다.



위의 소스를 실행한 결과는 다음과 같습니다．



get_cycles                      “수
[ [ [ r
      L [ [ [ [ [ [
                 1795. 434577] run_tlme_test () Start. . .
                 1795. 445665] loop_rdtsc 01: run_cycles=26576944, one call: 26 cycles
                 1795. 453173] loop_rdtsc 02: run_cycles=17979104, one call: 17 cycles
                 1795. 457942] loop_rdtsc 03: run_cycles=11410860, one call: 11 cycles
                 1795. 462422] loop_rdtsc 04: run_cycles=10725718, one call: 10 cycles
                 1795. 465207] loop_rdtsc 05: run_cycles=6666200, one call: 6 cycles
                 1795. 467114] loop_rdtsc 06: run_cycles=4568708, one call: 4 cycles
                 1795. 468886] loop_rdtsc 07: run_cycles=4244618, one call: 4 cycles
                 1795. 470879] loop_rdtsc 08: run_cycles=4768264, one call: 4 cycles
                 1795. 472961] loop_rdtsc 09: run_cycles=4983978, one call: 4 cycles




    커널연구회（附iw.kerne나）z)                                                            정재준（rgl好307@nate.com)
                                                          266/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                         red-bIack tree 테스트



[ 1795. 474184] loop_rdtsc 10: run_cycles=2920474, one call: 2 cycles
[ 1795. 474185] loop_rdtsc average: one ca1l=9 cycles
[ 1795. 474186] run_tlmemtest () End.



위의 결과를 보면 busy_Loop() 함수안의 코드를 ]00 만번 실행하는데 ]0,725,718 사이클 정도

소모되고, busy_Loop() 함수안의 코드를 한번 실행하는데 평균적으로 9 사이클 걸리는 것을 알 수

있습니다． 앞으로 커널 소스 코드 실행을 평가할때 위와 같은 get_cycles() 함수를 활용 하도록

하겠습니다. red-i乂ack tree 테스트 코드도 이 함수를 사용합니다. 자 이제 본론으로 들어가서 커널

소스 "Iib/rbtree_test.c" 에 있는 소스를 테스트 하도록 하겠습니다.




노드 삽입. 삭제 테스트

"Lib/rbtree_test.c" 소스는 커널 모듈로 코딩되어 있기 때문에, 이 소스안에 있는 rbtree_test_init()

함수부터 실행 됩니다. 이 함수안에 있는 코드들이 순차적으로 실행 되므로 이 소스들을 순서대로

설명하도록 하겠습니다. 먼저 아래 소스 코드들부터 실행됩니다．




     nodes = kmaUoc_array(nnodes, sizeof(*nodes), GFP_KERNEL);
      if小．nodes)
               return -ENOMEM;


      printk(KERN_ALERT "rbtree testing");


      prandom_seed_state(&rnd, 3141592653589793238ULL);
      initO;




 커널연구회（蜘胛．kerneL.bz)                                             정재준（rgbi3307@nate.com)
                                        267/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                               red-black tree 테스트



커널 메모리 할당 함수인 kmatLocma rray() 통하여 red寸乂ack tree 노드 구조체인 test_node 를

nnodes 711수만큼 커널에 메모리를 할당하고, 할당한 메모리 시작 주소를 nodes 에 전달 받습니다．

nnodes 개수는 ]00 으로 되어 있습니다. nodes 는 다음과 같이 test_node 구조체를 가르키는

포인터 변수 입니다．



nodes 구조쳬 선언

struct test_node {
         u32 key;
         struct rb_node rb;
         u32 va卜．
         u32 augmented;
};
static struct rb_root_cached root = RB ROOT CACHED;
static struct test_node *nodes = NULL;




위와 같이 test_node 구조체 ] 00 개를 메모리 할당한후 init() 함수를 실행하여 test_node

구조체안에 있는 멤버 변수인 key 값과 val 값을 임의의 난수 값（u32 데이터）으로 초기화 합니다．

in咀）함수 안의 코드는 다음과 같습니다．



m爬什함수

static void init(void)
{
         mnt i;
         for (i = 0; i < nnodes; i++) {
                  nodes[i].key = prandom_u32_state(&rnd);
                  nodes[i].va( = prandom_u32_state(&rnd);




     커널연구회（螂胛．kerne나功                                           정재준（rgbi3307@nate.com)
                                            268/ 351
                                                               리눅스 커널 소스 홰별 ［기초입문］
                                                                  red- bl.ack tree 테스트



       }
}


red七［ack tree 을 테스트하71 위한 구조체를 메모리 할당하고 그 안의 값들도 초기화 했으므로 이제

이 구조체들을 red七怡ck tree 의 root 을 기준으로 삽입하고 삭제하는 코드를 실행합니다. 이 코드는

다음과 같습니다．




       timel = get_cycLesO;


       for (I = 0; I < perf_loops; i++) {
                for (j = O; j < nnodes; j++)
                         insert(nodes +j, &root);
                for卜 0; j < nnodes; j++)
                         erase(nodes + j, &root);
       }

       t1me2 = get_cycLesO;
       匕me =匕me2 -匕mel;


        time = div_u64(time, perf_Loops);
       printk(" -> test 1 (Latency of nnodes insert+deLete): %LLu cycles\n",
           (unsigned Long Long)time);



먼저匕mel =get_cycLes(）을 실행하여 현재의 Cpu 사이클을 time] 에 저장합니다． 그런다음

perf_Loops 만큼 for 루프를 반복 수행하면서 노드들을 삽입하고 삭제 합니다. perf_toops 는 ]000

으로 초기화 되어 있습니다. 따라서 red-t乂ack tree 에 노드들을 100 개 삽입하고 삭제하는 작업을

1000 번 반복합니다. 이 실행 끝나면 time2 = get_cycLes(）을 실행하여 끝나는 시점의 cPu




    커널연구회佃ww.kerneLbz)                                                   정재준(rgb13307匣)nate.com)
                                               269/ 351
                                                             리눅스 커널 소스 해설 [기초입문］
                                                                red吐凡ack tree 테스트



사이클을 가지고 온후. time2 에서 timel 을 빼면 위의 코드가 실행되는 동안 소모한 CPU 사이클이

계산됩니다. 이것을匕me＝비v_u64(tiri祀, perf_Loops）을 실행하여 penf_Loops인 ]000으로

나누면 red七怡ck tree 에 노드들을 ] 00 개 삽입하고 삭저侑r는데 걸린 평균 CPU 사이클이 time 에

저장됩니다. 이 코드의 실행 결과는 다음과 같이 6514 사이클이 소모된 결과입니다．



testi 실행결과
kernel: [14441. 774330]           -> test 1 (latency of nnodes insert+delete) : 6514
cycles




위의 코드에서 red－비ack tree 에 노드를 삽입할때는 inset() 함수 ，삭제할때는 erase() 함수를

사용했지만. 이번에는 ins아t_cached() 함수와 erase_cached() 함수를 테스트 합니다． 테스트하는

방법은 다음과 같이 동일합니다．



태스트 2 코드

      timel = get_cycLesQ;


      for (i = 0; i < perf_Loops; i++) {
               for (j = 0; j < nnodes; j++)
                        insert_cached(nodes + j, &root);
               for U = 0; j < nnodes; j++)
                        erase_cached(nodes +j, &root);
      }

      t1me2 = get_cyctesO;
      time = time2 - timel;


      time = div_u64(time, perf_Loops);
      printk(" -> test 2 (Latency of nnodes cached insert+deLete): %LIu cycLes\n",




 커널연구회（w砥恐i.kerneib卦                                                  정쟤준(r야升330기孕岫te.com)
                                              270/ 351
                                                            리눅스 커널 소스 해설 ［기초입문］
                                                               red口black tree 테스트



          (unsigned Long Long)time);




이 코드의 실행 결과는 다음과 같이 643] 사이클이 소모된 결과입니다. 테스트 ] 에 비해서 83 사이클

빨라 졌습니다. 원인은 red－비ack tree 의 색상값을 결정하는 rb_insert_coLor_cached() 함수에

있습니다．



te孰2 실헝［궐콰
kernel: [14441. 774330]          -> test 2 (latency of nnodes cached insert+delete) :
6431 cycles




노드 탐색 테스트

이번에는 red-벼ack tree 을 inorder 방식（Left-Root-Right）으로 순서대로 탐색하는 테스트

코드입니다．




태스트3 코드「

      timel = get_cycLesO;


      for (i = 0; I < perf_Loops; k-+) {
               for (node = rb_first(&root.rb_root); node; node = rb_next(node))


      }

       t1me2 = get_cycLesQ;
      匕me = t1me2 七mel;




 커널연구회（www.kerne나）라                                                   정재준（rgbi3307@nate.com)
                                           271 /351
                                                                리눅스 커널 소스 홰설 ［기초입문］
                                                                   red吐八ack tree 태스트




      time = div_u64(time, perf_loops);
      printk(" -> test 3 (Latency of inorder traversal): %tlu cycles\n",
          (unsigned long long)time);




red-L乂ack tree 을 순서대로 탐색하는 코드는 다음과 같이 ]210 사이클 소모됩니다. 삽입, 삭제에

비해서 탐색 코드가 빠르게 동작되는 결과 입니다．




test3 실행결과
kernel: [14441. 777527]          -> test 3 (latency of inorder traversal) : 1210
cycles




이번에는 red-black tree 의 가장 왼쪽에 있는 첫번째 노드를 탐색하는 테스트 입니다．




테스트4코드


      timel = get_cyctesQ;


     for (i = 0; i < perf_loops; i++)
                node = rb_first(&root.rb_root);


     time2 = get_cyclesQ;
     匕me =匕me2 =匕me十．


     time = div_u64(time, perf_loops);
     printk(" -> test 4 (latency to fetch first node)\n");
     printk("      non-cached: %llu cycles\n ', (unsigned long long)time);


     timel = getHcyclesO;




커널연구회佃쌔쌔／.kerne(.b기                                                        정재준（r야)13307匣）nate.cori寸
                                           272/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                 red寸1.ack tree 테스트



      for (i = 0; I < perf_loops; i++)
                 node = rb_first_cached(&root);


      time2 = get_cyctesO;
      time = time2 - timel;


      time = div_u64(time, perf_Loops);
      printk("      cached: %Llu cycles\n", (unsigned Long Long)time);



위의 코드에서片_first() 함수가 red-black tree 의 가장 왼쪽에 있는 노드를 탐색하는 함수입니다．

rb_first(）는 순차적으로 계속 왼쪽 노드를 탐색하여 마지막 Leaf 노드에 도달하는 함수입니다．

그러나, rb_fir就_cached() 함수는 red-비ack tree 의 가장 왼쪽 노드에 대한 포인터를 미리 저장해

두고 있습니다. 그래서, 순차 탐색할 필요없이 한번 접근으로 실행이 끝나기 때문에 0 (1)

알고리즘으로 실행되는 함수입니다. 아래의 실행결과를 보면, rb1日rst() 함수는 ]6 사이클이

소모되는 반면에 rb_first_cached() 함수는 CPU 사이클 소모없이 바로 실행됩니다．




kernel: [14441. 777534]           -> test 4 (latency to fetch first node)
kernel: [14441. 777535]                  non- cached: 16 cycles
kernel: [14441. 777536]                  cached: 0 cycles


지금까지 커널 소스 "lib/rbtree_test.c"에 모듈 프로그래밍 되어 있는 예제를 통하여 red-black tree

를 테스트하는 소스를 설명해 드렸습니다. 이 예제는 커널의 red七怡ck tree 를 테스트해볼 수 있는

좋은 예제입니다. 저의 글을 통해서 커널 소스의 뿌리에 해당하는 red－비ack tree 를 이해하는더1

도움이 되었으면 합니다．




 커널연구회（叫쌔／.kerneL.bz)                                                    정재준（rgbi3307@nate.com)
                                             273/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해




커널 XArray 이해

                              이번글주저七 "커널 XArray이해" 입니다. XArray는


         少t
        Kernel XArray
                              "eXten引비e Arrays" 의 줄임말로서 2017 년-2018 년에

                              마이크로소프트의卜4atthe＼사 Wilcox 에 의해서 리눅스 커널 소스


         N万                   v4.19 부터 추가된 비교적 최신 소스입니다. 마이크로소프트도

                              리눅스 커널과 협업하기 시작한듯 합니다. 아래의 인터넷 참고

문서［凹를 보시면 Matthew Wilcox 가 XArray 에 대해서 소개한 내용이 있습니다．



httDs : //lwn. net/Articles/715948/


https :I/ www. kernel. orci/doc/html/latest/core- ani/xarrav. html




XArray는 매우 큰 포인터 배열처럼 동작하는 추상 데이터 타입（abstract data type) 입니다. 해시와

크기 변경 가능한 배열을 모두 만족 시킵니다. 해시와 다른 점이라면. 캐시 친화적인 방식으로 위치

이동（이전, 다음）을효율적으로 할 수 있습니다. 크기 변경 가능한 배열과 다른 점이라면, 배열의

크기를 증가 시키기 위해서 데이터를 복사 하거나 MMU 매핑을 변경할 필요가 없습니다. 양방향 연결

리스트（doubb小nked List) 보다 메모리 효율성이 좋고 병렬화 가능하며 캐시 친화적입니다. 또한

RCU 의 장점을 활용하여 락킹없이 조회 작업을 수행합니다.


위와 같이 XArray 는 많은 장점을 가지고 있는 자료구조 입니다. 하지만 XArray 에는 몇가지

특징들이 있습니다．



6    참고 문서 참조



    커널연구회佃쌔쌔／.kerne나功                                     정재준（rgb13307@nate.coa兮
                                      274/ 351
                                          리눅스 커널 소스 해설 ［기초입문］
                                                  커널 XArray 이해



XArray를 구현할때1 인덱스가 밀집되어 있으면 효율적입니다. 해시는 분산되는 특성을 가지고

있으므로 인덱스로 해시를 사용하거나 객체를 해싱하면 성능이 떨어집니다. XArray 는 작은 인덱스에

최적화되어 있지만 대량의 인덱스에서도 성능이 좋습니다． 하지만,인덱스가 ULONG_MAX 보다 크게

되면 XArray를 사용할 수 없습니다. 즉, XArray에서 인데스 최대 크기는 ULONG_MAX로 제한되어

있습니다. XArray는 페이지 캐시에서 가장 잘 활용될 수 있습니다．


배열에서 NULL 이 아닌 각각의 요소（entry）는 3 개 비트를 가지고 있으며 이것을 marks 라고 합니다．

각각의 mark 는 다른것들과 별도로 set 혹은 ci餉r 됩니다. 이렇게 marked 된 요소들에 대해서 반복

작업할 수 있습니다．


일반 포인터들은 XArray 에 바로 저장 될 수 있으며 4 바이트로 정렬되어 있습니다． kmaRoc() 및

퀘oc_page(）에서 리턴되는 포인터는 여기에 해당됩니다. 그러나사용자공간（user-space）에서

사용하는 포인터나 함수 포인터는 여기에 해당하지 않습니다. 정적으로 할당된 객체 주소가 4

바이트로 정렬되어 있다면 XArray 에 저장할 수 있습니다．


XArray에 0 부터 LONG_MAX 사이의 정수를 저장할 수도 있습니다. 이들을 XArray에 저장하기

위해서는 정수값을 xaUmk 始山eOA미 함수를 사용하여 XArray 요소（entry）로 변환해야 합니댜．

또한 XArray 에서 요소（entry）를 검색 할때는 xa I乞始山e() API 함수를 사용하고 요소（entry）를

다시 정수로 변환 할때는 xa to1v카ue() 함수를 사용합니다．


위와 같이 XArray 에 접근 하기 위해서는 XArray 전용 API 함수들을 사용합니다．


XArray 는 Un引gned tong 으로 색인화된（2八BITS_PER_LONG 개）포인터 배열이며 rad以 tree 를

많이 보완 했습니다. 기존에 리눅스 커널 소스에 있었던 rad汶 tree 는 점차적으로 XArray 로

교체될듯 합니다. 아래를 보시면 왼쪽은 rad以 tree API 함수들이고 오는쪽은 이 함수를 대체하는

XArray API 함수들입니다．



 커널연구회（www.kernel.bz)                            정재준（rgbi3307@nate.com)
                              275/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 XArray 이해1




rad姚tre甘 A叫 함수와 Xa相娜API함수 UI교
radix_tree_empty                        xa_empty
 _radix_tree_create                     xas create
  radix tree insert                     xas store
radix_tree_insert (x)                   xa_replace(NULL,   x)
_radix_t ree_lookup                     xas load
radix_tree_lookup                       xa load
radix_tree_lookup_slot                  xas load
_radix_t ree_replace                    xas store
radix_tree_iter_ replace                xas store
radix_tree_replace_slot                 xas store
口radix_t ree delete node                xas delete node
radix tree delete item                  xa_replace
radix tree delete                       xa_store ( NULL)
radix_tree_clear_tags                   xas_clear_tags
radix_tree_gang_lookup                  xa_get_entries
radix_tree_gang_lookup_slot             xas_find (*1)
radix_tree_p reload                     (*   3)
radix_tree_maybe_p reload               (*   3)
radix_tree_tag_set                      xa_set_tag
radix_tree_tag_clear                    xa_clear_tag
radix_tree_tag_get                      xa_get_tag
radix_tree_iter_ tag_set                xas_set_tag
radix tr朗小ga叫_loo kur匕tag               xa_get_tagged
radix_tree_gang_lookup_tag_slot         xas_load (*2)
radix_tree_tagged                       xa_tagged
radix_t ree_p reload_end                xas_preload_end
radix_t ree_split_preload               (*   3)
radix_tree_split                        xas_split (*4)
radix_tree_ join                        xa_replace



또한 기존 커널 소스인 IDR(integer ID management）도 XArray 을 사용하고 山A 도 XArray 안의

bitmap 으로 교체될 예정입니다. 山R 고F IDA 는 다음장부터 예제 소스와 함께 설명 됩니다．

卜4a比hew 小川cox 가 언급한 설명문서를 보면 XArray 는 다음과 같은 특징이 있습니다．




 커널연구회佃쌔,w.kerne나끄）                                    정재준（rgbi3307@nate.com)
                                  276/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        커널 XArray 이해



  .     기존 Radix Tree 데이터 구조와 호환성 유지

  S 락킹을 기본적으로제공

  .     메모리 pr이oading제거

  .     메모리 할당플래그를 명시적으로 분명하게 함

  1     Norma［과Advanced 로 구분하여 API 제공




그리고 리눅스 커널 소스에 적용된 XArray 관련 소스들은 다음과 같습니다．




리눅스 커널에 적용된 XArray 소스「
 include/linux/ idr . h                              136 +- -
 include/linux/ xarray h                             764 ++++++++++++++
 lib/ Makefile                                         3 +        口




 lib/ idr . c                                        503 +++++----
 lib/ radix- tree. c                                 169 +- -
 lib/ xar ray. c                                    1305 +++++++++++++++++++
+++++

 tools/include/asm/bug. h                               4 +

 tools/include/linux/ kernel. h                        1+
 tools/include/linux/ spinlock. h                       7 +-

 tools/ testing/radix- tree/ .gitignore                 4 +-
 tools/ testing/radix- tree/Makefile                   34 +-
 tools/ testing/radix- tree/ {idr- test .c => idr. c}  37 +-
 tools/ testing/radix- tree/linux. c                    2    +-
 tools/ testing/radix- tree/linux/ radix- tree. h       5
 tools/ testing/radix- tree/linux/ rcupdate . h         2 +
 tools/ testing/radix- tree/linux/ xarray . h           1+
 tools/ testing/radix- tree/ test .c                   59 +-
 tools/ testing/radix- tree/ test. h                   48 +-
 tools/ testing/radix- tree/ xarray . c               241 +++++
 19 files changed, 2783 insertions (+), 542 deletions(- )




 커널연구회（＼사寸쌔／.kerneLbz)                                  정재준（rgbi3307（흐）nate.com)
                                  277/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                             커널 XArray 이해1



위에서 "incLude/Li nux/xarray.h"는 Xarray자료구조를정의한헤더파일이고 "lib/xarray.c"에

Xarray A미 함수들의 소스가 있습니다. 나머지 소스파일들은 Xarray 에 의해서 수정된 너r.c 와

rad以-tree.c 소스이고 " tools/testing／士"에 테스트 소스들이 있습니다．




다음은 Xarray 에서 가장 대표적인 A미 함수들（할당／삽입／검색／삭제／제거）의 실행 흐름을 정리한

것입니다．




Xarray대표적힌 API 함수每
I/ /index --> xa . -> xas (xa operation state)

void *xa1load(struct xarray *xa, unsigned long index)
{
      XA_STATE(xas, xa, index) ;
      void *entry;
      entry = xas_load(& xas) ;
      return entry;




static inline mnt xa_alloc (struct xarray *xa, u32 *id,
            void *entry, struct xa_limit limit, gfp_t gfp)
{
      _xa_alloc (xa, Id, entry, limit,   gfp) ;
           XASTATE (xas, xa, 0) ;
           xas_store(&xas, entry) ;
}

void *xa1store(struct xarray *xa, unsigned long index,
            void *entry, gfp_t gfp)
{
     _xa_ store (xa, index, entry, gfp) ;
           XA_STATE(xas, xa, index) ;
           void *curr = xas_store(&xas, entry) ;
           retrun xas_result (&xas, curr) ;




커널연구회佃쌔쌔／.kerne나玹）                                   정재준（rgbi3307@ nate.con寸
                                   278/ 351
                                                    리눅스 커널 소스 해설 [71초입문］
                                                            커널 XArray 이해



static inline mnt xa_insert (struct xarray *xa,
            unsigned long index, void *entry, gfp_t gfp)
{
        _xa_insert (xa, index, entry, gfp) ;
             XA_STATE(xas, xa, index) ;
             curr = xas_load(&xas) ;
             if (! curr) xas_store(&xas, entry) ;
}

void *xa小find(struct xarray *xa, unsigned long *indexp,
            UnSi9ned
            unsigned l0ng
                     long maXr
                          max, xa_mark_t
                               Xamarkt, filter)
{
        XA_STATE(xas, xa, *indexp) ;
        void *entry;
        entry = xas_find(&xas, max) ;
        return entry;




void *xaeerase(struct xarray *xa, unsigned long index)
{
        entry = _xa_erase(xa, index) ;
              XA. 'STATE(xas, xa, index) ;
              xas_store(&xas, NULL) ;
}

void xa_destroy(struct xarray *xa)
{
        XA_STATE(xas, xa, 0) ;
        xas. xa_node = NULL;
        entry = xa_head_locked(xa) ;
        xas_init_ marks (&xas) ;
        if (xa_zero_busy (xa) )
               xa_mark_clear (xa, XA_FREE_MARK) ;
        if (xa_is_node(entry) )
               xasmfree_nodes (&xas, xa_to_node (entry) );
}

필자가 이글을 작성하는 시점의 리눅스 커널 버전은 v4.20 이여서 XArray 소스가 많이 안정화

된듯하고 이참에 XArray를 좀더 자세히 분석하고 있습니다 ．지금까지 분석결과，XArray는 전통적인




    커널연구회佃쌔八사．kernet.bz)                                     정재준（r야)13307@nate.com)
                                     279/ 351
                                                                     리눅스 커널 소스 해설 [71초입문］
                                                                             커널 XArray 이해



자료구조 알고리즘인 B+Tree 와 아주 유사하게 동작하지만 노드를 연결하는 주소와 인덱스 관리를

좀더 효율적으로 개선했습니다．



B+Tree 와 아주 유사하게 동작하는 Xarray 노드（엔트리）연결




                          흐IL그J 二：그
                           乞.       了于I
                                    J




                                                    !           !
                                    3       4
                                .       .               -

                                13 d4

그림참조：h比ps://en.w水巾飼治.orci/wiki/B%2B tree



RADIX TREE MAP
 Radix- tree                                                                     RADIX TREE MAP: 6
                                                    (root)
                                                            1
                                0                       0            0
                                1                                     1
                          (OxO)                                     (0x2)
                                I                                     I
                                                                      0
                   0            0               0                    0            0

                   I                            I                                 I
                 (Oxo)                      (0x2)                              (0x2)
                   I                            I                                 I
                   0                                                              0
         0        0        0                    1                         0      0         0

          I                I                    I                         I       I        I
       (OxO)             (Oxi)              (OxO)                   (OxO)      (Oxi)     (0x3)
         A                 B                  C                       D          E         F

 A: ex00000000
 B: ex00000eel
 C: 0x00000080




커널연구회佃쌔쌔／.kerne小力                                                             정채준（rgbi3307@ nate,con分
                                             280/ 351
                                                 리눅스 커널 소스 해설 ［기姦입문］
                                                         커널 XArray 이해



 D: 0x00e80080
 E: 0x00080081
 F: 0x00080083




아래부터 XArray 의 자료구조（구조체）와 A미 함수들을 분석한 내용들을 정리하도록 하겠습니다．




XArray 구조체 정의

XArray 는 다음과 같이 3 개 소스 파일과 설명 문서로 구성되어 있습니다．



XArray 소毋字샹

include/ fl nux/ xar ray. h            ///Xarray 데이터 구조쳬
lib/ xar ray. c                        ///Xarray 함수
lib/ test_xarray. c                    ///Xar ray 테스트 커널 모듈
Documentation/core- api/xarray. rst    //／설명 문서



위의 설명문서를 보면, XArray는 매우 큰 포인터들의 배열로서 추상적인 데이터 타입이라고 설명하고

                                .XArray는크기 조정이 가능하고캐시
있습니다． 여기서 "추상적인" 이라는표현이 좀 애매합니다만，

친화적입니다. 데이터를 복사 하거나卜4tv山 매핑이 필요 없습니다. 그래서 메모리를 효과적으로

사용할 수 있고 락킹없는 RCU 을 수행할 수 있는 장점들을 가지고 있습니다. 상당히 매력적인 데이터

타입인듯 합니다. 필자도 XArray 을 최근에 접했기 때문에 하나씩 알아가고 정리하는 형태로 기술하1

나가도록 하겠습니다．



XArray 는 다음과 같이 3 개의 구조체를 사용합니다．




 커널연구회（小쌔,w.kerneLb기                                  정재준(rgbi3307@nate.com)
                                      281 /351
                                                리눅스 커널 소스 해설 E기초입문］
                                                        커널 XArray 이해




(Array구조쳬
struct xarray
struct xa node
struct xa state



먼저， xarray 더1이터 구조체는 " include/Linux/xarray.h" 헤더 파일에 다음과 같이 선언되어 있고，

DE디NE小XARRAY(name) 에 의해서 정의 됩니다. 이 매크로는 다시

DEFINE_XARRAY_FLAGS(name, 0）로 정의되고 struct xarray 구조체가 name 으로 정의 되면서

XARRAY_I세T(name, flags）에 의해서 내부값들이 초기화 됩니다．




inctude/Linux/xarray.h
struct xarray C
      spinlock_t xa_lock;    1* struct spinlock *1
      gfp_t      xa_flags;   /* unsigned long */
      void _rcu 士      xa_head;    ／才 address小space(4)         x良小node을 가르킴 卄／
};
#define XARRAY_INIT(name, flags) {                         \
      .xa_lock = _SPIN_LOCK_UNLOCKED (name. xa. lock) ,          \
      .xa_flags = flags,                                   \
      .xa_head = NULL,                            \
}
#define DEFINE_XARRAY_FLAGS(name, flags)                         \
      struct xarray name = XARRAY_INIT(name, flags)

#define DEFINE_XARRAY(name) DEFINEeXARRAY_FLAGS(name, 0)




위의 xarray구조체는 단독으로 사용되지 않고 다른 구조체 안의 멤버로 사용합니다． xa_Lock

변수는 구조체안의 데이터를 보호하기 위해서 사용하고 xa head 변수는 처음에는 NULL 값이지만

entry 가 추가되면 xa_node 구조쳬를 가르키게 됩니다．




커널연구회佃쌔쌔／.kerne나）z)                                       정쟤준（rgb13307（孕nate.coa分
                                  282/ 351
                                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                                      커널 XArray 이해




xa_node 구조체는 다음과같이 "inctude/Linux/xarray.h" 헤더 파일에 선언되어 있습니다．

xa_node 구조체안의 없ots 배열의 크기는 XA_CHUNK_SIZE 입니다. 이것의 크기는

XA_CHUNK_SH下T에 의해서 시프트 연산으로 결정됩니다. 시프트 크기는 커널 빌드 상수값인

CONFIG_BASE_SMALL 이 0 이면 6 입 니다． 따라서 XA_CHUNK_SIZE 는 (1 <<6）에 해당하는 64

가 됩니 다．




加cLude/Linux/xarray.h
#ifndef XA CHUNK SHIFT
#define XA CHUNK SHIFT                                      (CONFIG_BASE1SMALL ? 4 : 6)
#endif
#define XA CHUNK SIZE                                       (1UL << XA_CHUNK_SHIFT)     /f/ 1<<6 == 64
#define XA CHUNK MASK                                       (XA_CHUNK_SIZE 中 1)     ///63
#define XA MAX MARKS                                        3
#define XA MARK LONGS                                       DIV_ROUND_UP (XA_CHUNK_SIZE, BITS_PER_LONG)
I/ /I

struct      xa_node {
          unsigned char                      shift;                      /央 Bits remaining in each slot
去／
     unsigned char offset;                                               1* Slot offset in parent 火 /
     unsigned char count;                                                ／士 Total entry count 作lot안에
NULL이 아닌 요소들의 개수） 女／
     unsigned char nr_values;                                      ／火 Value entry count 仁lot 안얘 모든
요소드'의，

              )
           二H，
              ct xa_n。
                 수．   t*   '/    de   _rcu       *parent：          戶 刈나 , , : , , , , : , , ,
                                                                                           *,
          struct xarray                      *array;                   /* The array we belong to 女1
          union            {
                           struct list_ head private_list;       /* For tree user ' /
                           struct rcu_head rcu_head;       /* Used when freeing node *7
          };
          void _rcu *slots[ XA CHUNKeSIZEI;     ///[64]
          union {
                unsigned long    tags[ XA_MAX_MARKS] [XA_MARK_LONGS] ;///[3] [1]
                unsigned long    marks [XA_MAXMARKS] [XAJIARK_LONGS] ;///[3) [l]
          };
     };



     커널연구회 佃川＼사.kerneL,뇨）                                                            정재준（rgbi3307@nate.com)
                                                                283/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 XArray 이해



xa_state 구조체는 다음과 같이 "incLude/Linux/xarray.h" 헤더 파일에 선언되어 있습니다． 이

구조체는 xarray 을 동작 시킬때 사용하는 구조체 입니다．



加山川e/LinuX舟array出1
struct xa_state {
    struct xarray *xa;
    unsigned long xa_index;
    unsigned char xa_shift;
    unsigned char xa_sibs;
    unsigned char xa_offset;
    unsigned char xa_pad;       /* Helps gcc generate better code 去I
    struct xa_node *xa node;
    struct xa_node *xaa] loc;
    xa_update_node_t xa_update;
};
#define XA_ERROR(errno) ( (struct xa_node *)( ( (unsigned long)errno < <          2)   I
2UL) )
#define XAS_BOUNDS ( (struct xa_node *)1UL)
#define XAS_RESTART ( (struct xa_node *)3UL)

#define _XA_STATE(array, index, shift,    sibs)   {    \




                                                                    \ \ \ \ \ \
    .xa = array,
    .xa_index = index,
    .xa_shift = shift,
    .xa_sibs = sibs,
    .xa_offset = 9,
    .xa_pad = 0,
    .xa_node = XAS_RESTART,               \
    .xa_alloc = NULL,              \
    .xa_update = NULL              \
}
#define XA_STATE(name, array, index)                \
    struct xa_state name =     _STATE(array, index, 0, 0)




커널연구회（蜘,w.kerneL.bz)                                   정재준（r야) 3307@nate.com)
                                  284/ 351
                                                            리눅스 커널 소스 해설 ［가冬입문］
                                                                    커널 XArray 이해



xarray 을 동작 시킬때는 XA_STATE(name, array, inde지로 struct xa_丈ate 을 정의하고 초기화

합니다. 이때 전달하는 name 은 struct xa_state 구조체 명칭이고 array 는 DE디NE_XARRAY 로

정의한 xar陷y 구조체입니다. index 는 xa_node 에 대한 인덱스 번호 입니다．



지금까지 기술한 xarray 구조체들의 상호 연결관겨를 다이어그램으로 정리하면 다음과 같습니다．



xarray 구조체 연결 다이어그램
 include/trnux/xarrayh                                                      incLude/I in납戈／xanray.h
           struct x我尹出0                汗'dud쏸／tin냔x/xarray.h                   struct xar카
 unsigned char           shift                就ructxa片吐求a                   S口朴ltock t xa tock
 unsgr)ed char           offset        融ruct xarray        亥Xa   小‘/        QIp_t   xafmlags
 unsigned char           C（가mnt        Un引gned 油ng      xajndex             V口磁 rCu 三xa head
 unsigned char           nr vaLues     트卦tsigned char   ：始 sh非t
 struct xamnode _rcu     *pa rent      unsigned char    xa nibs
 就ruct xarr,玎            好食Fr크y    劈   uns心ned char     xa 0汗set            DEFINE斗XARR肖V()
  日n!0nstr
   m。 n     냐ctltst head 口nv at已tist   unsigned char    xa oad              XA群是AY 作嚼TO
        ！止ruct rc냐 head rc旺 head       址ructxa node     竹xa_node
 V아dmrcu                 노沁ts［弘j       structxa node    亥xa attoc           API functions
  Un的nunsign             tags［多］[21
      n        숀d  tong                xa_updatejiode_t xa_u口date           xa_store()
        uns暳ned tong    marks[3][21                                         xa_Lo喆（)
                                                                            xa eras바）
       XA_CHUNK_MZE [}6or 64]              XA S了AT印                         xa_find()
       XA_MAX卞恢RKS［卦                                                        蕉am把r근ach()
      XAMARK_LONGS [i or 21                                                 xa_destroy()




 커 널연구회（www.kerneLb기                                                   정채준(rgbi3拍7回nate.com)
                                         285/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                             커널 XArray 이해1




XArray 테스트 모듈

필자는 위의 DE디N目XARRAY(name) 매크로를 사용하여 xarray 구조체를 정의하고 xarray API

함수들을 테스트（할당／삽입／검색／삭제제거）하는 코드를 커널 모듈로 아래와 같이 작성 했습니다．

소스 코드는 주석문으로 설명했습니다．




x社rray AM 함수태스트必
#include <linux/ xar ray. h>
#include <linux/module. h>
#include <linux/slab. h>

static DEFINE_XARRAY (array) ;       ///xarray 구조쳬 정의

///#define XA DEBUG
///xarray 구조체 안의 내용을 확인하는 함수
static void xa_user_dump (const struct xarray *xa)
{
    void *entry = xa- >xa_head;
    unsigned mnt shift = 0;
    //／구조쳬값 출력
    pr_info ( "xarray: %px head %px flags %x marks %d %d %d\n", xa, entry,
              xa- >xa_flags, xa_marked(xa, XA_MARKJ) ,
              xa_marked(xa, XA_MARK_l) , xa_marked(xa, XA_MARK_2) );
}
static mnt xarray_user_test (void)
{
    unsigned long i;
    void 出ret;
    ///xar ray에 연켤（추가）하기 위한 사용자 데이터 구조체
    struct item {
        unsigned long index;
        unsigned mnt order;
    };
    struct item *item;
    pr_info ( "xarray_usermtest () starting. . . \n") ;




커널연구회（出사w.kerne나坦）                                        정재준（rgbi3307c回nate.com)
                                    286/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 XArray 이해1



     item = kmalloc (sizeof (*item) , GFP_KERNEL) ; //／사용자 데이터 구조쳬
메모리 할당
     item->index = 0;
     item- >order = 100;
     pr_info( "[ O] item=%p\n", item) ;     //／사용자 데이터 구조체 주소 출력
     ret = xa_store(&array, 0, (void火)item, GFP_KERNEL) ;  ///xarray 인데
E) 에 저장

   for (i = 1; i, <= 1（키 i++) {.      1/ 710 번 뱐복 수행
       item = kmalloc (sizeof (*item) , GFPHKERNEL) ;   //／사용자 데이터 구조쳬
메모리 할당
       pr_info ( "[ %d] item=%p, ", 1, item) ;
       i tem->index = i;
       i tem->order = 1+100;
       ret = xa_store(&array, r (void* )item, GFP. -KERNEL) ;
                                 l.                            ///xarray
인데스 i에 저장
       pr_info ( !ret=%p\n!l, ret) ;     //／반환 주소 확인
       xa_user_dump (&array) ;       ///xarray 데이터 출력
    }
   ret = xa_load(&array, 0) ;      I/ /xarray 인텍스 0에 있는 내용 가져옴，
   pr_info( "load ret=%p, %d, %d\n", ret,
        ( (struct item *)ret) .>index, ( (struct item *)ret) ->order) ;    If '
가져온 내용 출력
   ret = xa_load(&array, 8) ;      III xarray 인데스 8에 있는 내용 가져옴
   pr_info ( "load ret=%p, %d, %d\n", ret,
        ( (struct item *)ret) _>index, ( (struct item *)ret) ->order) ;    /1/
가져온 내용 출

    ret = xa_erase(&array, 4) ;      1/I xarray 인텍스 4에 있뇬 내용 삭저i
    pr_info ( '1erase ret=%p, %d, %d\n", ret,
         ( (struct item *)ret) ->indexr ( (struct item *)ret) ->order) ;
    ret = xa_erase(&array, 7) ;      III xarray 인텍스 7에 있는 내용 삭제
    pr_info ( "erase ret=%p, %d, %d\n", ret,
         ( (struct item *)ret) 日>indexr ( (struct item *)ret) _>order) ;

   i = 9;
   ret = xa_find(&array, &i, ULONG_MAX, XA_PRESENT) ;       I/ I xarray 인덱스
9에 았는 검색
   pr_info ( "find ret=%p, %d, %d\n1 , ret,
        ( (struct item *)ret) .>index, ( (struct item *)ret) ->order) ;




 커널연구회（小쌔,w.kerneLbz)                                    정재준（r야)13307@nate.com)
                                      287/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해1



   xa_for_each (&array, i, ret) {        /1/ xarray 순환 탐색
     pr_info ( "each ret=%p, %d, %d\n", ret,
       ( (struct item *)ret) ..>index, ( (struct item *)ret) ->order) ;      I/ I
탐색한 내용 출력
    }
    xa_destroy (&array) ;     III   xarray   t저I

    pr_info ( "xarray_user_test () end. \n") ;

    return -EINVAL;
}
static void xarray_exit (void)
{
    pr_info ( "xarray_exit () end. \n") ;
}
module_init (xarray_user_test) ;
module_exit (xarray_exit) ;
MODULE_AUTHOR ( "JaeJoon Jung <rgbi3307@nate. com>' ) ;
MODULE_LICENSE( "GPL") ;



위의 소스를 커널 모듈로 빌드하여 실행하면 결과는 다음과 같습니다. 실행 결과에 대해서는 주석문

형태로 설명을 추가했습니다．




싶형켰콰
III xarray에 10개 데이터 저장됨 .
  kernel:  3216. 577685] xarray_user_test () starting. .
  kernel:  3216. 577687] [0] item=00000000d7c6d03e
 kernel:   3216. 577689] [1] item=000000007aa48c87,
 kernel:   3216. 577690] ret=             (null)
 kernel:   3216. 577692] xarray: ffffffffc0e85340 head ffff8c4546ca4922
 kernel:   3216. 577692] [2] item=0000000크8f243692,
 kernel:   3216. 577693] ret=             (null)
 kernel:   3216. 577694] xarray: ffffffffc0e85340 head ffff8c4546ca4922
 kernel:   3216. 577695] [3] item=000000002c08c993,
 kernel:  3216 .577695] ret=             (null)
 kernel:  3216. 577696] xarray: ffffffffc0e85340 head ffff8c4546ca4922




커널연구회如八사＼사．kernel.bz)                                     정재준（rgbi3307（흐）nate.com)
                                    288/ 351
                                                리눅스 커널 소스 해설 ［기姦입문］
                                                            커널 XArray 이해



 kernel:   3216. 577697] [4] item=000000007d320448,
 kernel:   3216. 577697] ret=             (null)
 kernel:   3216. 577698] xarray: ffffffffc0e85340 head ffff8c4546ca4922
 kernel:   3216. 577699] [5] item=00000000f1e409a9,
  kernel:  3216. 577699] ret=             (null)
  kernel:  3216. 577700] xarray: ffffffffc0e85340 head ffff8c4546ca4922
  kernel:  3216. 577701] [6] item=00000000311274cf,
  kernel:  3216. 577701] ret=             (null)
  kernel:  3216. 577702] xarray: ffffffffc0e85340 head ffff8c4546ca4922
  kernel:    3216. 577703] [7] item=00000000003d38e3,
  kernel:    3216. 577703] ret=             (null)
  kernel:    3216. 577704] xarray: ffffffffc0e85340 head ffff8c4546ca4922
  kernel:    3216. 577705] [8] item=0000000011695067,
  kernel:    3216. 577705] ret=             (null)
  kernel:    3216. 577706] xarray: ffffffffc0e85340 head ffff8c4546ca4922
  kernel:    3216. 577707] [9] item=00000크00befocole,
  kernel:    3216. 577707] ret=             (null)
  kernel:    3216. 577708] xarray: ffffffffc0e85340 head ffff8c4546ca4922
  kernel:    3216. 577709] [10] item=000000005e3edb9a,
  kernel:    3216. 577709] ret=             (null)
  kernel:    3216. 577710] xarray: ffffffffc0e85340 head ffff8c4546ca4922
Ill  xarray에서 인덱스 0 번과 8 번의 내용을 가져옴．
  kernel: [ 3216 577711] load ret=00000000d7c6d03e, 0, 100
  kernel: [ 3216. 577712] load ret=0000000011695067, 8, 108
I/ I xarray에서 인덱스 4번과 7 번의 내용을 삭졔함，
  kernel: [ 3216. 577713] erase ret=000000007d320448, 4, 104
  kernel: [ 3216. 577714] erase ret=00000000003d38e3, 7, 107
ill   xarray에서 인텍스 9 번의 내용율 검색함，
  kernel: [ 3216. 577715] find ret=00000크00befOcole, 9, 109
ill   xarray의 내용을 순환하여 출력한 결과．
  kernel: [ 3216. 577716] each ret=（三）  0000｛크（9（크d7c6d（크3e, 0, 100
  kernel: [ 3216. 577716] each ret=000000007aa48c87, 1, 101
  kernel: [ 3216. 577717] each ret=000000008f243692, 2, 102
  kernel: [ 3216. 577718] each ret=000000002c08c993, 3, 103
  kernel: [ 3216. 577718] each ret=00000000f1e409a9, 5, 105
  kernel: [ 3216. 577719] each ret=00000000311274cf, 6, 106
   kernel: [ 3216. 577720] each ret=0000000011695067, 8, 108
   kernel: [ 3216. 577721] each ret=000000크0befocOle, 9, 109
   kernel: [ 3216. 577721] each ret=000000005e3edb9a, 10, 110

 kernel: [ 3216. 577723] xarray_user_test () end.




 커널연구회（寸쌔쌔／.kerae比z)                                   정재준（r야)13307（孕nate.com)
                                  289/ 351
                                                 리눅스 커널 소스 해설 E기초입문］
                                                         커널 XArray 이해




radix tree 테스트

리눅스 커널에서 Rad以Tree 구조체를 "力ncLude/tinux/radix-tree.h" 파일과

"力ncLucle/Linux/xarray.h" 파일에서 다음과 같이 선언하고 있습니다． rad以1t爬e_root 구조체는

앞에서 언급한 xarray 구조체로 치환되고 rad怏_tree_riode 구조체는 xa_node 구조체로

치환됩니다. 따라서 기존의 리눅스 커널 Radix Tree 는 xarray을 사용하고 있다는 것을 알 수

있습니다．



/inctude/tinux/rad

#define radix tree root       xarray          ///include/ linux/ xar ray. h
#define radix tree node       xa_node     ///include/ linux/ xarray. h

struct radix_tree_iter {
    unsigned long    index;
    unsigned long    next_index;
    unsigned long    tags;
    struct radix_tree_node *node;
};


위의 Radix Tree 구조체 노드들을 초기화 하는 매크로는 다음과 같이 정의 되어 있습니다．



/include/Linux/xarray.b

#define XARRAY_INIT(name, flags) {                      \
      . xa_1ock = _SPIN_LOCK_UNLOCkED(name. xa_lock),          \
      .xa_flags = flags,                                \
      .xa_head = NULL,                           \
}




커널연구회佃쌔／w.kerneLb力                                      정재준（四b13丑刃＠nate.com)
                                 290/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                              커널 XArray 이해




/h鞍如dc/Li恥ix/ra小x止ree.h

#define RADIX_TREE_INIT(name, mask) XARRAY_INIT(name, mask)

#define RADIX_TREE (name, mask) \
      struct radix_tree_root name = RADIX_TREE_INIT(name, mask)

#define INIT_RADIX_TREE(root, mask) xa_init_ flags (root, mask)




Rad以 Tree 구조체 노드들을 초기화하고 삽입, 삭제, 탐색하는 함수들은 커널 소스 파일

"LUb/xa rray.c"와 "川b/ra비x_tree.c"에 구현되어 있습니다． 또한 리눅스 커널에는 이 소스들을

테스트하는소스가 "/tooLs/testing/radix-tree/" 경로에 있습니다. 이곳에 있는소스들은 단독

프로그램으로 빌드하여 실행할 수 있습니다. 먼저 이 경로에 있는 소스파일들의 목록은 다음과

같습니다．




知oLs/te尉崩g/rad袂七rae／소스파임毋
-rw- r- -r- - 1 jungjj     jungjj 4007    1월 20 13: 01 benchmark. c
-rw- r- -r- - 1 jungjj jung刀       599    1월 2（크 13: 01 bitmap. c
drwxr- xr- x 2 jungjj ]ung끄 4096          3월 4 12: 07 generated!
-rw- r- -r- - 1 jungjj jungjj        73   1월 20 13: 01 .gitignore
-rw- r- -r- - 1 jung力 ]ung刀 11838         1 월 20 13: 01 idr- test. c
-rw- r- -r- - 1 jungjj ]ung刀 4613         1월 20 13: 01 iteration_ check. c
drwxr- xr- x 2 jungjj ]ung刀 4096          1 월 2（크 13 : 01 linux!
= r닙e r 1 m r = = 1 jungjj ]ung刀 2256     1 월 20 13: 01 linux. c
- rw- r - - r - - 1 jung力 ]ung刀 7567      1 월 20 13: 01 main. c
-rw- r- -r- - 1 jungjj jungjj 1529        1 월 20 13: 01 Makefile
- rw- r - - r - - 1 jungjj ]ung刀 5654     1월 20 13: 01 multiorder. c
-rw- r- -r- - 1 jungjj jung刀 4596         1월 20 13: 01 regressionl. c
 -rw- r- -r- - 1 jungjj jungjj 4031       1월 20 13:01 regression2. c
 -rw- r- -r- - 1 jungjj ]ung刀 2510        1월 20 13:01 regression3. c
 -rw- r- -r- - 1 jung力 ]ung刀 1521         1월 20 13: 01 regression4. c
 = r닙＝r- -r- - 1 jung力 jungjj       214   1월 20 13: 01 regression. h




 커널연구회（M쌔쌔／.kerne比z)                                          정재준（rgb13307(＠咐te.com)
                                      291 /351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                   커널 XArray 이해


    -rw- r- -r- - 1   jungjj   ]ung刀    8832   1월 20 13: 01 tag_check. c
    -rw- r- -r- - 1   jungjj   jungjj   6412   1월 20 13: 01 test. c
    -rw- r- -r- - 1   jungjj   ]ung刀    2386   1월 20 13:（玎 test. h
    -rw- r- -r- - 1   jungjj   ]ung刀     651   1월 20 13: 01 xarray. c



    위의 소스 목록을 보면 main.c 소스파일과卜4akefile 이 있어서 이 경로에서 make 하여 소스를 빌드할

수 있습니다. 그러나 make 을 실행해 보면 불행하게도 다음과 같은 컴파일 오류가 발생합니다．




$ make
cc -I. -I. .!. ./include -g -Og -Wall -D_LGPL_SOURCE fsanitize=address
fsanitize=undefined      -c -o main. o main. c
In file included from ./linux/ . .1. .1. .!. ./include/linux/ radix- tree.h: 28: 0,
                    from ./linux/ radix- tree.h: 5,
                    from main. c:10:
./linux/ rcupdate.h:5:10: fatal error: urcu.h: No such file or directory
 #include <urcu.h>
                八

compilation terminated.
<builtin> : recipe for target 'main. o ' failed
make: 士士出 [main. o] Error 1



위의 오류 메세지를 보면 <urcu.h> 헤더파일이 없다는 것인데，이 파일은 userspace RCU7 '(read-

copy-update) 라이브러리을 인클루드하는 헤더 파일입니다． RCU 는 락킹없이 동기화를 구현하는

기법입니다. RCU 에 대해서는 향후 리눅스 커널 락킹에 대해서 기술할때 다루도록 하겠습니다．

여기서는 일단, userspace RCU 라이브러리를 설치하여 Rad汶 Tree 을 테스트하는 소스부터

이해하도록 하겠습니 다．



userspace RCU 는 아래떽 웹사이트에서 소스를 배포하고 설치하는 방법에 대해서도 잘 설명되어

있습니다．


7     RCU 참고 문서




커널연구회（邸加．kerneLbz)                                               정쟤준（rgb13307（孕nate.con寸
                                          292/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해




https://[iburcu.ora/



필자도 이곳에 있는 내용을 참고하여 다음과 같이 userspace RCU 라이브러리를 설치했습니다．



먼저 아래와 같이 이t clone 을 실행하여 소스를 다운로드 받습니다．



$ git clone git: //git. liburcu. org/userspace- rcu. git


다운로드가 완료되면 이 소스 경로로 들어가서 다음과 같은 순서대로 그곳의 명령어들을 실행합니다．

                            ［小"경로에 최종적으로 설치됩니다．
이렇게 하면 라이브러리 파일들이 "/usr/loc計／




      pace RCU 라이브러리 섶치
$ cd userspace- rcu/
$ ./bootstrap
$ ./configure
$ make
$ sudo make install
$ sudo ldconfig ＃경로（蹄 등록됨（PA丁H :=/usr/local/lib)



userspace RCU 라이브러리들이 설치되면, 이제 우리가 분석하고자 하는 Rad以 Tree 테스트 소스가

있는 "/too1s/testing/radix七eel" 경로로 가서 이곳의 소스를 다음과 같이 빌드합니다． 간단히

make 을 실행하면 됩니다．



Rad次了侄枉 테스트 소스 빌드

$ make




  커널연구회（小쌔／낚／.kerneLb기                                     정재준(rgb1330기＠nate.com)
                                    293/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 XArray 이해


cc -I. -I. .!. ./include -g -Og -Wall -D_LGPL_SOURCE -fsanitize=address
fsanitize=undefined          -c -o main. o main. c
cc -I. -I. .!. ./include -g -Og -Wall -D_LGPL_SOURCE - fsanitize=address
fsanitize=undefined         -c -o xarray. o xarray. c
sed -e 's/ Astatic II ' -e 's/ _always_inline /1' -e 's/ inline //'
< . .1. .1. . /lib/ radix- tree.c > radix- tree.c
cc -I. -I. ./. ./include -g -og -Wall -D_LGPL_SOURCE -fsanitize=address
fsanitize=undefined         -c -o radix- tree. o radix- tree. c

／身女 중간 생략 出*1

cc -fsanitize=address -fsanitize=undefined main. o xarray. o radix- tree. o
idr. o linux. o test. o find_bit. o bitmap. o regressionl. o regression2. o
 regression3. o regression4. o tag_check. o multiorder. o idr- test. o
iteration_check. o benchmark. o -lpthread -lurcu -o main
cc -fsanitize=address -fsanitize=undefined idr- test. o xarray. o radix-
tree. o idr. o linux. o test. o find_bit. o bitmap. o -lpthread -lurcu -o idr-
 test
cc -fsanitize=address -fsanitize=undefined multiorder. o xarray. o radix-
tree. o idr. o linux. o test. o find_bit. o bitmap. o -lpthread -lurcu -o
multiorder
cc -fsanitize=address -fsanitize=undefined xarray. o radix- tree. o idr. o
linux. o test. o find_bit. o bitmap. o -lpthread -lurcu -o xarray



위의 빌드 메세지들을 보면 main.c, xarray.c, radix-tree.c.. 등등의 소스 파일이 컴파일되어 main

실행파일이 생성되는 것을 알 수 있습니다. 이 m키n 실행 파일을 다음과 같이 실행해 보겠습니다．




Radi乂枷ee태소트
$ ./main

 random seed 1551672592
running tests
XArray: 21134867 of 21134867 tests passed
vvv Ignore these warnings
assertion failed at idr. c: 239
assertion failed at idr. c: 205
AAA Warnings over
IDA: 28868236 of 28868236 tests passed
tests completed




커널연구회（邸胛．kern叫,bz)                                      정쟤준（rgb1330끄흐）nate.com)
                                  294/ 351
                                                    리눅스 커널 소스 해설 ［기奏입문］
                                                            커널 XArray 이해




Radix Tree 테스트는 많은 쓰레드의 생성／소멸이 반복 되면서 실행되기 때문에 RCU 을 사용합니다．

쓰레드 병렬처리 환경에서 ra비x1t爬e 와 xarray 에서 데이터을 메모리 할당／추가／삭체소멸을 반복

테스트 합니다. 이제 이 소스를 분석하는 일이 남았습니다．




먼저 m키n.c 소스 파일에 있는 main 함수부터 소스를 보겠습니다. 이곳의 소스를 위에서부터 아라로

순서대로 함수가 실행되는 과정을 분석하면 됩니다. 전체 실행 흐름은 주석문으로 설명을

추가했습니다．




OO拇在心I:加g/ra毗和tr兮E/maii玉（

mnt main(int argc, char **argv)
{
        bool long_run = false;
        mnt opt;
        unsigned mnt seed = time (NULL) ;

        while ( (opt = getopt (argc, argv, "ls: v") ) ! = -1) {
              if (opt == '1')
                     long_run = true;
              else if (opt == 's ')
                     seed = strtoul (optarg, NULL, 0) ;
              else if (opt == 'vT)
                     test_verbose++;
        }

        printf ( "random seed %u\n", seed) ;
        srand(seed) ;

        printf ( "running tests\n") ;

        rcu_register_threadQ;
        radix_tree_init () ; ///kmem_cache_create() : struct radix tree node

        xarray_tests() ; ///xarray API functions test
        regressionl_test () ; ///radix_ tree_insert () , delete() test
        regression2_testQ;




    커널연구회佃쌔시／.kerneLb기                                      정재준似非好307@nate.com)
                                        295/ 351
                                                 리눅스 커널 소스 해설 ［기초입룬］
                                                         커널 XArray 이해1



      regression3_test ( );
      regression4_test () ; ///radix_ tree_lookup ( ), read( ), write() test
      iteration_test (0, 10 + 90 * long_run) ;
      iteration_test (7, 10 + 99 * long_run) ;
      single_thread_tests (long_run) ;

      1* Free any remaining preallocated nodes */
      radix_tree_cpu_dead(0) ; ///kmem_cache_freeO: radix_tree_node

      benchmark () ;    ///benchmark_iter () function test

      rcu_barrier () ;
      printv(2, "after rcu_barrier: %d allocated, preempt %d\n",
            nr_allocated, preempt_count) ;
      rcu_unregister_thread() ;

      printf ( "tests completed\n") ;

      exit (0) ;
}

위의 main 함수에서 중요한 함수들을 순서대로 설명하도록 하겠습니다．




radix_treeJnit()

radix_tree_m i日）함수는 ra비x_tree_node 구조체（xa_node 구조체）를 메모리 할당하는 역할을

합니다. 이 함수의 소스는 "Lib/radix-tree.c" 파일에 다음과같이 정의 되어 있습니다. 먼저 이

함수부터 분석하도록 하겠습니다．




ra小x tree=ii毗（) 함수 소스
 void 中 mnit radix_tree_init (void)
{
    mnt ret;

    BUI LD_BUG_ON ( RADIX_TREE_MAX_TAGS + _GFP_BITS_SHIFT > 32) ;




커널연구회（邪＼사砥床erneL.b力                                      정쟤준(rgb13307簪nate.com)
                                   296/ 351
                                                            라눅스 커널 소스 해설 ［기초입푼］
                                                                    커널 XArray 이해



      BUILD_BUG_ON (ROOT_IS_IDR & -GFP_ZONEMASK) ;
      BUILD_BUG_ON (XA_CHUNK_SIZE > 255) ;
      radix_tree_node_cachep = kmem_cache_create ( "radix_tree_node",
               sizeof (struct radix_tree_node) , 0,
              SLAB_PANIC I SLAB_RECLAIM_ACCOUNT,
               radix_tree_node_ctor) ;
      ret = cpuhp_setup_state_nocalls (CPUHP_RADIX_DEAD, "lib/ radix: dead",
                        NULL, radix_tree_cpu_dead) ;
      WARN_ON(ret < 0) ;
}

위의 소스에서 BU止D BUG ON 매크로는 다음과 같이 정의되어 있습니다．


#define BUILD_BUG_ON(condition) ((void)sizeof(char[1 - 2*U(condition)]))

cond止幻n 으로 전달한 값이 True 이면 char 배열의 인덱스값이 음수가 되므로 " error: size of

unnamed arra미S negative"와 같은 컴파일 오류가 발생합니다. 그러므로 BUILD_BUG_ON

매크로는 condition 으로 전달한 값의 유효성을 컴파일 시점에서 점검할 따1 아주 유용합니다．

condition 은 Fa匕e 가 되어야 컴파일 오류가 발생하지 않습니다. 참고로 위의 소스에 있는
      1\




BUILD_BUG_ON 매크로들은 다음과 같이 컴파일 되고 condition 은 Fa匕e 입니다.


           ( (void) sizeof (char[ i - 2* ! !(3 + 26 >32) ]));
           ( (void) sizeof (char[1 - 2* ! !( ( ( gfp_t) 4) & -ox크fu) ]));
           ( (void) sizeof (char[1 - 2* ! !( (1UL << 3) > 255) ]));


다음으로 kmem_cache_create() 함수를 보겠습니다. 아직 커널 메모리 관련 소스들에 대해서 진도

나가지 않았기 때문에 여기서는 함수 사용법（A미）위주로 보겠습니다. kmem_cache_create()

함수는 아래와같이 "include/Linux/stab.h" 헤더파일에 선언되어 있고 "/mm/slal乙common.c"

소스 파일에 정의되어 있습니다．



Inc如deJLlnu刈如b.h
 struct kmem_cache *kmem－尸cacheHcreate(const char *name, unsigned mnt size,




    커널연구회（ww＼사.kerneL.뇨）                                             정재준(r9bi3307（孕nate.com)
                                           297/ 351
                                              리눅스 커널 소스 해설 E기초입문］
                                                      커널 XArray 이해



            unsigned mnt align, slab_flags_t flags,
            void (*ctor) (void *));


kmem_cache_create() 함수에 전달하는 인수는 명칭, 크기, 정렬 오프셋, 플래그. 比or 함수 포인터

순으로 전달합니다． 위에서 명칭은 " radix_tree_node"이고 크기는 引zeof(struct

rad以_tree_node), 정렬 오프셋은 0 이고, 플래그는 SLAB_PA새C 1 SLAB_F之ECL시M_ACCOUNT

입니다． 마지막으로 ctor 함수 포인터는 radix_tree_node_ctor 입니다． 결국 radix_tree_node

구조체 크기만큼 할당한 메모리의 시작 주소를 rad怏_tree_node_cachep 포인터 변수에

저장합니다. 이 변수는전역 변수 입니다．



rad以jree_node 구조체는 "Inc山de/Linux/rad以叱ree.h" 헤더 파일에 다음과 같이 정의 되어

있습니다．



#define radix
        /\
              tree node     xa node


매크로 치환에 의해서 rad以中tree_node 구조체는 xa_node 구조체가 됩니다． 이 구조체는

incLude/Linux/xarray.h 헤더파일에 다음과 같이 선언되어 있습니다．



Inc如如川flux／相rray.h
struct xa_node {
    unsigned char    shift;      /* Bits remaining in each slot */
    unsigned char    offset;     /* Slot offset in parent *1
    unsigned char    count;      /* Total entry count *1
    unsigned char    nr_values; 1* Value entry count *1
    struct xa小node _rcu 士parent;      ／士 NULL at t야） of tree 士／
    struct xarray    *array;     1* The array we belong to *1
    union {
        struct list_ head private_list;   /* For tree user *1




커녈연구회（납八赳寸,.kerne나燕）                                  정쟤준（rgb13307（孕nate.com)
                                298/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해



           struct rcu_head rcu_head;     /* Used when freeing node */
      };
      void _rcu *slots[ )(A1CHUNk1SIZE] ;
      union {
          unsigned long   tags [XA_MAX_MARKS] [XA_MARk_LONGS] ;
          unsigned long   marks {XA_MAX_MARKS] [XA_MARK_LONGS] ;
      };
};

이 구조체에 있는 내용에 대해서는 앞으로 설명이 이어질 예정입니다．




cp먀巾_setup_state_noc키匕（) 함수는 "include/(inux/cpuhotplug.h" 헤더파일에 다음과 같이

정의되어 있습니다．




incLude/Linux/cpuho Lu h
static inline mnt cpuhp_setup_state_nocalls (enum cpuhp_state state,
                        const char *name,
                        mnt (* startup) (unsmgned mnt cpu) ,
                        mnt (* teardown) (unslgned mnt cpu) )
{
      return _工puhp_setup_state(state, name, false, startup, teardown,
                    false) ;




위의 함수에 전달하는 인자들은 다음과 같습니다．



ret = cpuhp_setup_state_nocalls (CPUHP_RADIX_DEAD, T1lib/radix:dead",
                    NULL, radix_tree_cpu_dead) ;


네번째 인자인 (*teardown) 함수 포인터에 rad以_tree_cpu_dead 함수를 전달하여 해당 CPU 가

down 될따1 이 함수가 동작하도록 등록합니다．




    커널연구회（www.kernet.b기                                   정재준（r야)13307@nate.com)
                                       299/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                              커널 XArray 이해


지금까지 radix_tree_m id) 함수0州 실행되는 내용을 설명 드렸습니다． 결국 radix中tree_node

구조체를 메모리 할당한 포인터를 ra비x_tree_node_cachep 에 넣고 사용하71 위한 것입니다．




xarray_ tests()

이곳에서 xarray API 함수들을 테스트 합니다. xa rray_tes匕（）함수에서 다시 tib/test_xa rray.c 에

정의되어 있는 xarray_checks(）함수를 다음과 같이 실행합니다. 이 함수0似似array A미 함수들인

xa_toadO, xa_markO, xa_shrinkO, xas_eraseO, xa_insert_indexO, xa_erase_index() 등 OI

테스트 됩 니 다．



相rraychec如（）함수

static DEFINE_XARRAY (array) ;

static mnt xarray_checks (void)
{
       check_xa_err (&ar ray) ;
       check_xas_retry (&array) ;
       check_xa_load (&ar ray) ;
       check_xa_mark (&ar ray) ;
       check_xa_ shrink (&array) ;
      check_xas_erase (&array) ;
      check_insert (&ar ray) ;
      check_cmpxchg (&array) ;
      check_ reserve(&ar ray) ;
      chec卜乙reserve (&xaO ) ;
      check_multi_store(&array) ;
      check_xa_alloc () ;
      check_find (&array) ;
      check_f ind_entry (&array) ;
      check_account (&array) ;
      check_destroy (&array) ;
      check_move (&array) ;
      check_create_range (&array) ;
      check_ store_range (&array) ;




커널연구회（螂쌔／.kerne나）z)                                         정재준（rgbi3307（흐）nate.com)
                                    300/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해



        check_store_iter (&array) ;
        check_align(&xa0) ;

        check_workingset (&array, 0) ;
        check_workingset (&array, 64) ;
        check_workingset (&array, 4096) ;

        printk ( "XArray: %u of %u tests passed\n ", tests_passed, tests_run) ;
        return (tests_run == tests_passed) ? 0 : -EINVAL;
}
void xarray_tests(void)
{
        xarray_checks () ;
        xarray_exitO;
}


regressioni _test()

이 함수0似1는 여러개의 쓰레드를 생성하여 ] 000000 번을 반복하며 rad以jree_insert(）와

radix_tree_delete(）을 테스트 합니다. 관련 소스는 다음과 같습니다．




쓰래드 생성

static pthread_t *threads;
void regressionl_test (void)
I
        mnt nr_threads;
        mnt 1;
        long arg;

     ／女 Regression #1 士／
      printv (l, "running regression test 1, should finish in under a
minute\n") ;
      nr_threads = 2;
      pthread_barrier_init (&worker_barrier, NULL, nr_threads) ;

        threads = malloc (nr_threads * sizeof (pthread_t *));




    커널연구회（小쌔시／.kerne나끄）                                   정재준（r야)13307@nate.com)
                                      301 /351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         커널 XArray 이해




      for (i = 0; i < nr_threads; i++) {
            arg = l;
            if (pthread_create(&threads[i] , NULL, regressionl_fn, (void
出）arg) ) {
                  perror ( "pthread_create ") ;
                  exit (1) ;
             }
      }
      for (i = 0; i < nr_threads; i++) {
            if (pthread_join(threads[i] , NULL) ) (
                  perror ( "pthread_join") ;
                  exit (1) ;
             }
      }
      free(threads) ;

      printv(1, "regression test 1, done\n") ;
}

위에서 생성한쓰레드 함수（regressionl_fn)는 다음과 같이 반복 실행됩니다. for루프가 반복되는

횟수는 ]000000 입니다．




static pthread_barrier_t worker_barrier;

static void *regressionlfn(void *arg)
{
     rcu_register_thread ( );

     if   (pthread_barrier_wait (&worker_barrier) ==
                    PTHREAD1BARRIER_SERIAL1THREAD) {
             mnt j;

            for (j = 0; j < 1000000; j++) {
                  struct page *p;




커널연구회（的,w.kerne나끄）                                     정재준（r的3307（흐）nate.com)
                                 302/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         커널 XArray 이해



                   p = page_alloc (O) ;
                   xa_lock (&mt_tree) ;
                   radix_tree_insert (&mt_tree, 0, p) ;
                   xa_unlock (&mt_tree) ;

                   p = page_alloc (1) ;
                   xa_lock (&mt_tree) ;
                   radix_tree_insert (&mt_tree, 1, p) ;
                   xa_unlock (&mt_tree) ;

                   xa_lock (&mt_tree) ;
                   p = radix_tree_delete(&mt_ tree, 1) ;
                   pthread_mutex_lock (&p->lock) ;
                   口＞count = - ;
                   pthread_mutex_unlock (&p->lock) ;
                   xa_unlock (&mt_tree) ;
                   page_free (p) ;

                   xa_lock (&mt_tree) ;
                   p = radix_tree_delete(&mt_ tree, 0) ;
                   pthread_mutex_lock (&p->lock) ;
                   p- >count- -;
                   pthread_mutex_unlock (&p->lock) ;
                   xa_unlock (&mt_tree) ;
                   page_f ree(p) ;
          }
    } else {
          mnt j;

          for (j = 0; j < 100000000; j++) {
                struct page *pages[lol;

                   find_get_pages(0, 19, pages) ;
          }
    }
    rcu_unregister_thread() ;

     return NULL;




커널연구회（www.kerneL.bz)                                       정재준（r야)13307@nate.com)
                                   303/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                                커널 XArray 이해



benchmark()

이 함수에서는 다음과 같이 benchmark_iter(）함수를 사용하여 rad以1treemne沚_chunk() 함수롤

테스트 합니다．




benchmarkJt可()함수
 static long long benchmark_iter (struct radix_tree_root *root, bool tagged)
 {
         volatile unsigned long sink = 0;
         struct radix_tree_iter iter;
         struct timespec start, finish;
         long long nsec;
         mnt 1, loops = 1;
         void 士士slot;

#ifdef BENCHMARK
again:
#endif
       clock_gettime (CLOCK_MONOTONIC, &start) ;
       for (1 = 0; 1 < loops; l++) {
             if (tagged) {
                   radix_tree_for_each_tagged(slot, root, &iter, 0, 0)
                          sink A= (unsigned long) slot;
             } else {
                   radix_tree_for_each_slot (slot, root, &iter, 0)
                          sink A= (unsigned long) slot;
               }
         }
         clock_get time (CLOCK_MONOTONIC, &finish) ;

         nsec = (finish. tv_sec - start. tv_sec) * NSEC_PER_SEC +
                (finish .tv_nsec - start. tv_nsec) ;

#ifdef BENCHMARK
      if (loops == 1 && nsec * 5 < NSEC_PER_SEC) {
            loops = NSEC_PER_SEC I nsec I 4 + 1;
            goto again;
         }
#endif




커널연구회（＼사니시／.kerne나功                                       정재준（rgbi3307@ nate.com)
                                    304/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           커널 XArray 이해




        nsec 1= loops;
        return nsec;
}




rad汶 tree 테스트 모듈

이번에는 rad以 tree 을 커널안에서 테스트 해보도록 하겠습니댜. 소스를 커널 안에서 실행 시키71

위해서는 모듈로 작성하는 것이 가장 간단합니다. 다음과 같이 커널 모듈로 테스트 소스를 작성

했습니다. rad怏 tree 에 노드를 테스트（삽입／조회／삭제）하는 간단한 커널 모듈입니다．




radi乂tre奪珝스트 모堪
 #include <linux/ xarray. h>
 #include <linux/radix- tree. h>
 #include <linux/module. h>
 #include <linux/ slab. h>

struct item {
      struct rcu_head   rcu_head;
      unsigned long index;
      unsigned mnt order;
};
I/ /item 구조체 메모리 할당
struct item *itemHcreate (unsigned long index, unsigned mnt order)
C
        struct item *item = kmalloc (sizeof (*item) , GFP_KERNEL) ;
        item->index = index;
        item->order = order;
        return item;
}
I/ /radix_tree 에 item 삽입
mnt item_insert (struct radix_tree_root *root, unsigned long index)
 C



    커널연구회佃째iw.kerne나）기                                    정재준（r아)13307@nate.com)
                                    305/ 351
                                                   리눅스 커널 소스 해설 [71초입문］
                                                           커널 XArray 이해



        struct item *item = item_create(index, (index+1) *100) ;
        mnt err = radix_tree_insert (root, item- >index, item) ;
        if (err)
              kfree(item) ;
        return err;
}
7/ /radix_tree 에서 item 삭제
mnt item寸delete(struct radix_tree_root *root, unsigned long index)
{
        struct item *item = radix_tree_delete(root, index) ;

        if   (! item)
                  return 0;

        kfree (item) ;
        return 1;
}
static mnt radix_test_init (void)
{
    mnt i, index;
    struct item *item;

    RADIX_TREE(rdx, GFP_KERNEL) ;

    pr_info ( "item_test starting. . .\nn ) ;

    for (i=0; 1<5; i++) {
        item_insert (&rdx, i) ;
        pr_info ( "item_insertQ: index=%d\n ", i) ;
    }
    for (1=0; 1<5; i++) {
          item = radix_tree_lookup(&rdx, 1) ;
          pr_info ( "lookup () : index=%d, order=%d\n", item- >index, Item-
>order) ;
    }
    for (i=0; 1<5; i++) {
        item_delete(&rdx, 1) ;
        pr_info ( "item_deleteQ: index=%d\n ", 1) ;
    }



커널연구회（www.kerne나江）                                       정재준（rgbi3307@nate.com)
                                    306/ 351
                                                                        리눅스 커널 소스 해설 ［기초입문］
                                                                                커널 XArray 이해1




                          pr_info ( "item_test end. \n") ;

                          return 0;
}
static void radix_test_exit (void)
{
                          pr_info ( "xarray_exit () end. \n") ;
}
module_mnit ( radix_test_mnit) ;
module_exit (radix_test_exit) ;
MODULE_AUTHOR ( "JaeJoon Jung <rgbi3307@nate. com>") ;
MODULE_LICENSE( "GPL ") ;



위의 커널 모듈은 rad怏 tree 노드에 item 구조체를 5 번 메모리 할당하여 삽입하고 그 결과를

조회한후에 다시 삭저侑七 것을 간단히 테스트 하는 것입니다. 위의 예제를 통해서 커널에서 radix

tree 를 작업하는 API 함수들을 이해할 수 있습니다. 실행 결과는 다음과 같습니다．




rad次 tree 태스트 실헝 겊과
[                          0. 820887] item_test starting. . .
[                          0. 821404] item_insertQ: index=0
[                          0.821693] item_insert ( ): index=1
[                          0. 821944] item_insert () ; index=2
[                          0. 822184] item_insert ( ): index=3




                  L n
                    1
                    느 n
                      L
                           0. 822426] item_mnsertQ: index=4




                L r
            L 1
              L r
        L [ r
                           0. 822690] lookupQ: index=0, order=100




  L [ n
      1
      L 1
                           0. 822975] lookup() : index=1, order=200




[ n
                           0. 823241] lookup() : index=2, order=300
                           0. 823507] lookup( ): index=3, order=400
                           0.823774] lookup () : index=4, order=500
                           0. 824138] item_delete() : index=0
                           0. 824399] item_deleteQ: index=1
                           0.824678] item_delete( ): index=2
                           0. 824929] item_deleteQ: index=3
                           0. 825202] item_delete( ): index=4
                           0. 825426] item test end.




        커널연구회（낚쌔쌔／.kerne나玘）                                                  정재준(rgb133(｝기孕nat色corn
                                                             307/ 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          커널 XArray 이해1




IDR, IDA 관리


        六
                                  리눅스 커널의 IDR은 "ID Rad以" 입니다. 정수형 ID을

                                  관리하기 위한 "integer ID managen祀nt" 입니다． 山A는山
      Kernel Integer ID           할당자인 "ID Altoc故or" 입니다. 여기서 ID는 식별번호（인덱스
           \j附             "

                                  키）입니다. IDR은 山 을 생성하여 사용자 데이터까지 연결하여

                                  관리하고 山A는 山만 생성합니다. 우리는 데이터가 많아지면

많아질수록 이것을 효율적으로 관리（추가／검색／삭제）하기 위해서 ID（식별번호）을 부여하는 경우가

많이 발생합니다. 또한 ID 는 멀티 쓰레드 환경에서도 중복없이 고유한 인덱스키 역할을 해야 합니다．

데이터7F 많아질수록 ID 를 부여하고 관리하는 부담이 증가하기 때문에 효율적인 자료구조가

필요합니다. 다행히 리눅스 커널에서는 앞에서 기술한 xarray와 ra비汁tree 을 사용하여 아주

빠르고 효율적으로 ID 를 관리합니다. IDR, IDA는 2002 년에 커널 소스에 추가 되었으나 최근

xarray가도입되면서 성능이 향상되었습니다. 山R과山A소스는 "incLude/Linux/idr.h" 헤더

파일과 "Lib/idr.c"에 구현되어 있습니다．



아래는 IDR 과 山A 에 관련되는 리눅스 커널 소스 파일들입니다．



DR콰 IDA관련 소스
include/linux/idr . h
include/linux/xar ray. h
lib/ idr . c
lib/ radix- tree . c
lib/ xarray . c
tools/ testing/radix - t ree/ 士




커녈연구회（璘쌔／硼，k好rneib力                                     청재준（rg蜘3307簪nat色corn)
                                      308/ 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         IDR, IDA 관리



소스를 본격적으로 설명하기 전에 구조체 정의부터 이해하고 가도록 하겠습니다．




idr, ida 구조체

idr을 정의하는 구조체는 DEFINE그DR(name) 매크로를 사용하여 name 이름으로 struct idr

구조체를 정의하고 멤버값들을초기화합니다. 이 코드들은 "include/linux/ic打．h" 파일에 다음과

같이 코딩되어 있습니다．




idr쿠조쳬
#define radix tree root        xarray
#define radix tree node        xa node

#define XARRAY_INIT(name, flags) {                        \
      . xa_lock = _SPIN_LOCK_UNLOCkED (name. xa_lock) ,         \
      .xa_flags = flags,                                  \
      .xa_head = NULL,                            \
}
#define RADIX_TREE_INIT(name, mask) XARRAY_INIT(name, mask)

struct idr {
    struct radix_tree_root idr_rt;       「f/ /struct xarray
    unsigned mnt 1      idr_base;
    unsigned mnt        idr_next;


#define IDR FREE      0

#define IDR_RT_MARKER   (ROOT_IS_IDR I (_ force gfp_t)   \
                    (1 << (ROOT_TAG_SHIFT + IDR_FREE) ))

#define IDR_INIT_BASE(name, base) {
    . idr_rt = RADIX_TREE_INIT(name, IDR_RT_MARKER) ,
    .idr_base = (base) ,
    .idr_next = 0,
}



    커널연구회（＼사버,w.kerneLb라                                  정재준（r야)13307@nate.com)
                                   309/ 351
                                                         리눅스 커널 소스 해설 ［기초입문］
                                                                 IDR, IDA 관리




#define IDR_INIT(name)        IDR_INIT_BASE(name, 0)

#define DEFINE_蜘R(name)               struct idr name = IDR_INIT(name)

static inline void idr_ init_ base (struct idr *idr,           mnt base)
{
     INIT_RADIX_TREE (&idr- >idr_rt,        IDR_RT_MARKER) ;
     idr- >idr_base = base;
     idr- >idr_next = 0;
}
static inline void idr_init (struct idr *idr)
{
       idr_init_ base (idr,    0) ;
}


위에서 idr 구조체는 DEFINE_IDR(na me) 매크로를 사용하여 정의합니다．




Ida 구조체도 incLude/linux/idr.h 에 다음과 같이 정의 되어 있습니다. 간단하게 xarray구조체가

멤버로 들어가 있습니다. ida 구조체는 DEFINE JDA(name) 매크로를 사용하여 정의합니다．




川a구조채

struct ida {
      struct xarray xa;

};
#define IDA_INIT_FLAGS        (XA_FLAGS_LOCK_IRQ I XA_FLAGS_ALLOC)

#define IDA_INIT (name) {                                                  \
      .xa = XARRAY_INIT(name, IDA_INIT_FLAGS)                                  \
}
#define DEFINE_IDA(name)               struct ida name = IDA_INIT(name)




커널연구회（艸／比kerneLbz)                                               정재준(rgb沼307帥ate.com)
                                         引0 / 351
                                                           촤눅스 커널 소스 篩설 ｛기姦입문］
                                                                   IDR, IDA 관리




지금까지 기술한 구조체 연결관계를 다이어그램으로 정리했습니다. 모두 xarray구조체와 연결

됩 니 다．



Idr, ida 구조체 연결 다이어그램1
     ncR心e/tinux/xacray'h   !nc山deft inux/idr.卜토
r       struct xarray 斗                 strk址I Ida
             Ht xa_tock
    spin1（그C卜；              structxarray             xa
    gfp中t       xa中ftags
    vok重 1W 去xa head        DEFINEJDA(rtame)



    D EFINE_XAR RAY()       mnd此M呱妹／님Lh
    笠ARR矗Y걋4rr()                         struct idr
                            攷八乂t rad以 tree root dr rt
    APt 凡n心的ns              unsigned [nt            idr_base
    xa_store()              냐nsigned !nt            k打爬就
    xa_load()
    嵬a小erase()              DEFINEjDR(name)
    xa_flnd()
    美乏師乙each()
    蒸a_destr仍／0




    커널연구회（www.k숀In畝,b라                                         청채준(rgb1330？簪附te.co昨1
                                          311 /351
                                                  리눅스 커널 소스 해설 ［기姦입문］
                                                          工DR, 工DA 관리




idr할당

idr할당은 " Lib/idr.c"에 정의 되어 있는 U打1카Loc(）함수에서 실행됩니다. 이 함수에 전달하는

파라미터 인수들은 다섯개 입니다. 순서대로 용법을 말씀 드리면, idr은 DEFINE그DR () 매크로를

사용하여 struct idr 구조체를 정의한 메모리 포인터 입니다. ptr 은 U打 에 의해서 연결되는 객체의

포인터 입니다. 즉, ptr은사용자가관리하고자하는데이터 포인터입니다. start는mnt데이터

타입의 최소 ID 값이고 end 는 최대 ID 값입니다. start 와 end 범위에서 ID 가 할당 됩니다．

마지막으로 gfp 는 메모리 할당에 관련되는 플래그 값입니다.



Ub/idr.c
 mnt idr_alloc (struct idr *idr, void *ptr, mnt start, mnt end, gfp_t gfp)
 C
         u32 Id = start;
         mnt ret;

         if   (WARN_ON_ONCE(start < 0) )   f/ /start 는 0보다 커야함，
                 return -EINVAL;

         ret = idr_alloc_u32(idr, ptr, &id, end > B ? end - 1 : INTJIAX,
gfp) ;
         if   (ret)
                 return ret;    ///／할당 성공한 ID 반환

         return Id;      ///sta八 ID 반환
}
EXPORT_SYMBOL_GPL (Idr_alloc) ;
                                                                             j
idr_atLoc(）함수는 내부에서 다시 idr小aLloc_u32() 함수를 호출합니다. 이 함수를 호출할따1 전달하는

파라미터 인수들을 순서대로 설명 드리면, idr 은 struct idr 구조체를 정의한 메모리 포인터 입니다．

ptr은 IC打에 의해서 연결되는 객체（사용자 데이터）의 포인터 입니다． nextid 는 현재 start ID 을

전달했다가 다시 연산한 山 을 받습니다. max 는 최대 ID 가 0 보다 크면 현재값에서 ] 을 빼서




커널연구회（w＼舟w，蛇rneibz)                                    정쟤준(rgbi3307會nat乞corn)
                                     引2 / 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        IDR, IDA 관리



전달하고，max 값이 0 이면 tNT中MAX 을 전달합니다. gtp 에는 메모리 할당 플래그 값을 그대로

전달합니다．




idr_aLloc_u32() 함수 내부의 코드들은 아래 소스에서 주석문으로 설명을 추가 했습니다．




的月dr.c
mnt idr_alloc_u32(struct idr *idr, void *ptr, u32 *nextid,
                  unsigned long max, gfp_t gfp)
{
      struct radix_tree_iter iter;
      void _rcu 女士slot;
      unsigned mnt base = idr- >idr_base;
      unsigned mnt Id = *nextid;
                 I/ /id r. >idr_rt 의 풀래그7卜 ROOT叫ISJDR 이 아니면 플래그 값율
IDR中RT叫MARKER로 설정
      if (WARN_ON_ONCE(! (idr- >idr_rt . xa_flags & ROOT_IS_IDR) ))
            idr- >idr_rt . xa_flags 1= IDR_RT_MARKER;

      id = (Id < base) ? 0 : Id - base;
      radix_tree_iter_ inlt (&iter, id) ;   /I/ radixmt ree_iter 구조쳬의
nextmindex을 id 로 함
      slot = idr_get_free (&idr- >idr_rt, &iter, gfp, max      base) ;
      if (IS_ERR(slot) )
            return PTR_ERR (slot) ;

        *nextid = iter. index + base;
        ,/" there is a 熬餓iory 鈿rrier 王nside r我dixmtre會‘小iter小replace() 亥／
        radix_tree_iter_ replace(&idr- >idr_rt, &iter, slot, ptr) ;
        radix_tree_iter_ tag_clear (&idr- >idr_rt, &iter, IDR_FREE) ;

        return 0;
}
EXPORT_SYMBOL_GPL(idr_alloc_u32) ;



idr_alloc_u32() 함수 내부는 커널 코어 소스를 깊이 있게 이해해야 설명할 수 있는 부분입니다. 좀더

분석하는 시간이 필요할듯 합니다. 이번에는 일단 IDR 에서 제공하는 API 함수들을 활용하는




    커널연구회（V／叫,.kerneLbz)                               정재준(rgbi3307@nate.com)
                                  引3 / 351
                                           리눅스 커널 소스 해설 ［기초입문］
                                                   IDR, IDA 관리



측면에서 소스를 설명 드리도록 하겠습니다. ID 을 할당하고 검색, 삭제하는 API 함수들은 다음과

같습니다．



IDR API哲수珪
idr_alloc()
idr_find()
idr_remove()
idr_destroy()
idr_is_empty()


위의 API 함수들을 사용하여 IC打 을 테스트하고 활용하는 예제를 아래부터 설명 하도록 하겠습니다．




idr 테스트

idr을 테스트하는 예제는 커널 소스의 too匕／testing/ra비乂tree力먀叱est.c 에 있습니다. 이 예제

소스도 내용이 상당히 많습니다. 그래서 필자는 山R시기 함수들중에서 핵심적인 부분만 테스트하는

코드를 다음과 같이 main(）함수에 추가 했습니다． 필자가 추가한 함수는 Id口te就sin叩［e() 입니다．

전체적인 실행 흐름은 주석문으로 설명 했습니다．



idr 태스트 예쟤 소스
 static void idr_test_simple(void)
{
      unsigned mnt 1, id, order;
      DEFINE_IDR(idr) ;
      struct item *item;

      printf ( "idr_alloc ()                  \n   ")   ;
      //idr id 107卜1 할당
      for (i = 0; i < 10; i++) C




커널연구회佃1W사．kerne나파                                  정재준（rgbi3307@ nate.com)
                                引4 / 351
                                                  리눅스 커널 소스 해설 ［기초입문］
                                                          IDR, IDA 관리



         order = i * 10;
             struct item *item = item_create(i, order) ;
             id = idr_alloc (&idr, item, 0, 0, GFP_KERNEL) ;
             printf ( "i=%u, id=%u\n", i, id) ;
     }
     printf ( "idr_for_each_entry ()                   \nU)              ;




      /／할당한 id 조회（출력）
     idr_for_each_entry (&idr, item, Id) {
        printf ( "id=%u, item- >index=%lu, order=%u\n",
            id, item->index, item- >order) ;
     }
     printf ( "idr_find()                             \n") ;
     I/ id 검색
     id = 5;
     item = (struct item *)idrfind (&idr, id) ;
     if (item)
        printf ( "found id=%d, item- >index=%lu, order=%u\n",
            id, item->index, item->order) ;
     else
        printf ( "Not found(id=%u) \n", id) ;

     printf ( "idr_remove ()                              ;
                                                         \n        ")
     I/ id 삭제
     idr_remove (&idr, id) ;
     item = (struct item *)idr find(&idr, id) ;
     if (item)
        printf ( "found id=%d, item- >index=%lu, order=%u\n",
            id, item->index, item->order) ;
     else
        printf ( "Not found(id=%u) \n", id) ;

     printf ( "idr_destroy()                                  \n    ")   ;
     //idr 전쳬 제거
     idr_for_each (&idr, item_idr_free, &idr) ;
     idr_destroy (&idr) ;

     if (idr_is_empty (&idr) ) printf ( "idr is empty. \n") ;
     else printf ( "idr is not empty. \n") ;
}
mnt _weak main(void)




커널연구회（낚쌔쌔／.kerne나끄）                                                정재준（rgb13307匣）riate.com)
                                  引 S / 351
                                                 리눅스 커널 소스 해설 ［기초입문］
                                                         IDR, IDA 관리




      radix_tree_initO;

           est_斑mp1e( ;
      return 0;

      idr_checks () ;
      ida_tests() ;

      radix_tree_cpu_dead(1) ;
      rcu_barrlerO;
      If (nr_allocated)
            printf ( "nr_allocated = %d\n! , nr_allocated) ;
      return 0;




idr_test_simple() 함수는 IC打 에 ]0 개의 Id 을 할당합니다. 할당할때 item 구조체를 전달하는데 이

구조체가 사용자가 관리하는 데이터에 해당합니다. 이 데이터에 Id 을 할당하여 IC打 에 연결하고

조회를 합니다. 그리고 특정 Id 에 대해서 검색. 조회. 삭저1 작업을 하고 결과를 확인합니다．

마지막으로 전체 idr 을 제거하고 테스트 작업을 마무리 합니다．

실행결과는 다음과 같습니 다．



世r태스트 첨헝 겉콰
idr_alloc ()
i=0, Id=0
1=1, Id=1
1=2, id=2
1=3, Id=3
1=4, .id=4
i=5, Id=5
1=6, ld=6
1=7, Id=7
i=8, 1d=8
1=9, Id=9
ldr_ for_each_ent ry()
id=0, ltem->lndex=0, order=0
ld=1, ltem- >lndex=1, order=10




커널연구회佃째쌔／.kerne比z)                                      정쟤준（r야)13307@nate.com)
                                  引6 / 35]
                                                    리눅스 커널 소스 해설 ［기초입문］
                                                            IDR, IDA 관리



id=2, item- >index=2, order=20
id=3, item- >index=3, order=30
id=4, item- >index=4, order=40
id=5, item- >index=5, order=50
id=6, item- >index=6, order=60
id=7, item- >index=7, order=70
id=8, item- >index=8, order=80
id=9, item- >index=9, order=90
idr_find()
found id=5, item->index=5, order=50
idr_remove ()
Not found(id=5)
idr_destroy()
idr is empty.




ida 테스트

ida 는 앞에서 기술한 xarray구조체를 사용하여 유일한 Id 만 할당합니다. Ida 도 A미 함수들을

사용하는 측면에서 소스를 설명하도록 하겠습니다. ida 을 사용하기 위한 A미 함수들은 다음과 같이

커널 소스 include/Linux/idr.h 에 정의 되어 있습니다 ．함수들의 의미는 주석문을 추가하여

설명했습니다．




//o과 INT MAX사이의 ID값을 가져옴．
static inline mnt ida_alloc (struct ida *ida, gfp_t gfp)
{
        return ida_alloc_range(ida, 0, -0, gfp) ;
}
I/ mmn과 I NT_MAX사이의 ID값을 가져옴．
static inline mnt ida_alloc_min(struct ida *ida, unsigned mnt mmn, gfp_t
gfp)
{



    커널연구회佃쌔八사．kerneL 뇨）                                 정재준（rgbi3307（曾nate.com)
                                   引7 / 35]
                                                 리눅스 커널 소스 해설 1기초입문］
                                                         IDR, 工DA 관리



       return ida_alloc_range (ida, mmn, 卞0, gfp) ;
 }
 I/ O과 max 사이의 ID값을 가져옴，
 static inline mnt ida_alloc_max (struct Ida *ida, unsigned mnt max, gfp_t
 gf p)
 {
       return ida_alloc_range (ida, 0, max, gfp) ;
 )
 I/ st竄rt 과 end사이의 ID값을 가져옴，
 #define ida_simple_get (ida, start, end, gfp)    \
                   ida_alloc_range (ida, start, (end) - 1, gfp)
 #define ida_simple_remove(ida, Id) Ida_f ree(ida, Id)

 static inline bool ida_Is_empty(const struct Ida *ida)
 {
       return xa_empty (&Ida->xa) ;
 }

Ida 을 테스트하는 예제도 커널 소스의 tools/testing/radix-tree/idr-test.c （川 있습니다． 커널

소스는 다중 쓰레드 환경에서 여러가지 조건을 만들어서 Ida 을 테스트 하7i 때문에 소스가 상당히

복잡합니다만. Ida 는 모두 위의 API 함수를 사용하여 테스트 합니다. 그래서 필자는 ida 사용에

대해서 쉽게 이해할 수 있도록 다음과 같이 간단한 테스트 함수를 만들었습니다. 실행 흐름은

주석문을 추가하여 설명 했습니다．



id甘태스툐얘째1 소스
 static void ida_test_simple (void)
{
      mnt i, Id;
      DEFINE_IDA (ida) ;

      printf ( "ida_alloc ()                          \n") ;
      I/ ida 主d 10 7竹 할당，
      for (I = 0; 1 < 10; i++) {
         Id = ida_alloc (&ida, GFP_KERNEL) ;
         printf ( "Id=%d\n' , Id) ;




커널연구회（璘／叭／낡／.kerne나玹）                                  정재준(r9b13307會nate.com)
                                  引8 / 35]
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                             IDR, IDA 관리



        }
        prlntf ( "Ida_free()                              \n    ")   ;
        I/ Ida Id 3 과 5 졔거，
        ida_free(&ida, 3) ;
        Ida_free (&Ida, 5) ;

        /／다시 Id 5개 할당，
        for (i = 0; 1 ( 5; i++) {
              id = ida_alloc (&ida, GFP_KERNEL) ;
              printf ( "id=%d\n", Id) ;
        }
        printf ( "ida_destroy ()                           \n   ")   ;
        I/ ida 제거，
        ida_destroy (&ida) ;

        if (Ida_Is_empty (&Ida) ) printf ( "ida Is empty. \n") ;
        else printf ( "ida Is not empty. \n") ;
}


Ida 는 중복없이 유일한 Id 정수값을 할당합니다. Id 는 순서대로 증가하면서 할당 되고, 중간에 Id 을

삭제하고 다시 할당하면 순서대로 삭제된 id 부터 다시 할당됩니다. 아래 실행 결과를 통해서 확인

가능 합니다．




ida 테스트 싫횅 켭과
ida_alloc ()
Id=0
id=l
Id=2
Id=3
Id=4
id=5
id=6
 id=7
 id=8
 id=9
 ida_f ree()




    커널연구회（www.kernet.bz)                                         정재준(rgb13307但）nate.com)
                                      引9 / 35]
                               리눅스 커널 소스 해설 ［기초입문］
                                       IDR, IDA 관리



id=5
id=10
id=11
id=12
id=13
id=14
id=15
id=16
id=17
ida_destroy()
Ida Is empty.




커널연구회佃ww.kerne比z)                 정재준（rgb日307@ nate.com)
                    320/ 351
                                              리눅스 커널 소스 해설 ［기초입문］
                                                         percpu 이해




percpu 이해


       六
                           이번글주제는 "커널 percpu 이해" 입니다. 리눅스커널

                           percpu 개념은 간단합니다. 커널 버전 2.6 이하 시대의 Cpu 는
      Kernel percpu Test



      Y
                           대부분 코어가 ] II 있었지만 요즘은 CPU 코어가 2 개, 4 개, 8

                           7F1. . 계속 증가하여 S卜4P(Symmetric卜4u出Processing)

                           환경이 대세로 자리 잡았습니다. 리눅스 커널도 이러한 Cpu

변화에 맞추어 버전업 하면서 버전 2.6 때부터 percpu 가 도입 되었습니다.SMP 환경에서는

mu出마ocessing 되기 때문에 연산 처리를 효율적으로 하기 위해서 CPU 코어마다 자기만의 전용

변수가 필요하게 되었습니다. 따라서 percpu 는 해당 CPU 코어 전용 변수을 만들고 연산하기 위해서

커널에 도입된 소스입니다. 또한 percpu 변수를 연산처리 하기위한 전용의 커널 A미 함수들도

있습니다. 이것들에 대해서 알아보도록 하겠습니다．




ELF Sections 이해1

"CPU 전용 변수를 만들기 위해서 어떻게 하면 될까요7" 이것에 대한 고민을 해보시고 커널 소스를

분석해 보셨다면 이번글은 쉽게 이해될 것입니다. CPU 는 연산을 담당하고 연산 대상은 메모리

(RAM）에 있습니다. 우리가 작성한 프로그램은 모두 메모리（RAM）에 있고 CPU 는 여기에 있는 것을

코딩된 절차대로 가져와서 연산（실행）하고 그 결과를 다시 메모리에 저장합니다. 여기서 프로그램

코드와 데이터가 메모리에 배치되는 위치가 중요하고 이것에 대해서 정리한 것이 ELF8 VII(Executabte

and Linkable Format) 입니다. ELF 에 대해서는 아라떽 인터넷 위키피디아 문서에 잘 정리 되어

있습니다.

8    참고문서 ELF 참조



    커널연구회佃쌔八사.kerneLbz)                               정재준（r야)13307（孕nate.com)
                                321 /351
                                                         리눅스 커널 소스 해설 E기초입문］
                                                                    percpu 이해




    乍I半챰고뵨서二
    ht印s://en.wik巾叱治.아可Wi叫Executa벼e_and_Linka바已比rmat#/



이 문서를 보면 ELF 에 대해서 다음과 같은 그림으로 설명하고 있습니다．



                 ELF header


             Program header table



                     .text



                    .rodata
         뇨




             Section header table


그림 참조：https://ea.wikipedia.org/wiki/Executabte_andLinkable_Format#/media/Fite:ELf-tayout--
en.svg



우리가 작성한 프로그램 파일 안에는 위의 그림과 같이 ELF 헤더가 있습니다. 그리고 프로그램 헤더

테이블과 Section 헤더 테이블에는 프로그램 코드 및 데이터로 접근하는 위치정보（주소）가 있습니다．

이것을 보통 Sec匕on9 "M이라하고 위의 그림에서 .text .rodata ... .data 에 해당하는 것들입니다．

이들은 모두 메모리에 배치되어 있는 주소입니다. 이것에 대해서는 아래 웹사이트에 자세히

설명되어 있습니다．

9    참고문서 참조



커널연구회佃쌔쌔／.kerne山z)                                              정재준（rgbi3307@nate.com)
                                       322/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                              percpu 이해




卵e心a心部t沁n引n Linux bin町沁宬
https://lwn.n etJArticles/531148/



이러한Section 정보들은 컴파일러에 있는 링커에서 활용됩니다． 아래와 같이 "Id -verb匹e"
                                                                          //   /   " 나／
                                                              '   ,   H




명령을 실행하면 링커에서 사용하는 Section 정보들을 확인할 수 있습니다．



Li在ker＄缸t陌n청보 확인

$ Id -verbose

/／다음과 같이 화면에 출력 됩니다，
GNU id (GNU Binutils for Ubuntu) 2. 30
  Supported emulations:
   elf x86 64
   e1f32 x86 64
   elf i386
/／중간생략．,
SECTIONS
{
  /* Read- only sections, merged into text segment: 女1
  PROVIDE (_ executable_start = SEGMENT_START ( "text- segment ", 0x400000) );
= SEGMENT_START ( "text- segment ", 0x400000) + SIZEOF_HEADERS;
/／중간생략，,
  .init
    {
        KEEP (* (SORT1NONE( .init) ))




        *( . text. unlikely .text. *_unlikely .text. unlikely. *)
        *( . text . exit .text. exit. *)
        *( . text . startup .text. startup. *)
        *( . text . hot .text. hot. *)
        *(. text .stub .text. * .gnu.linkonce. t. *)
        1出 .gnu. warning sections are handled specially by e1f32. em.              *1




    커널연구회（小쌔쌔／.kerneLb기                                   정재준（r아)13307（孕nate.com)
                                        323/ 351
                                                                리눅스 커널 소스 해설 ［기麥입문］
                                                                           percpu 이해


           *( .gnu.warning)
   }
 /／중간생략．,

                              rL 戶
                                 J
                                 L
   . rodata                          *(. rodata .rodata. * .gnu.linkonce. r. *) }
   . rodatal                         *( .rodatal) }
 /／중간생략，,
   . data
   {
       *(. data .data. * .gnu.linkonce. d. *)
       SORT (CONSTRUCTORS)
   }
   . datal          : { 出（.datal) }
     edata = .; PROVIDE (edata = . ) ;
       -     1   r

    bss start
  .bss
/／이하생략，,




이러한 링커 Sec匕On 정보들이 실제로 리눅스 커널에서 어떻게 적용 되는지 확인해 보기 위해서 "

readeif" 리눅스 명령어를 사용합니다. 리눅스 커널 소스를 컴파일 하면 빌드된 경로에 vmlinux

파일이 만들어 집니다. 리눅스 커널은 이 파일에 있는 내용들이 컴퓨터가 부팅될때 메모리에 배치

되면서 실행 됩니다. vm[inux도 ELF형식의 파일이기 때문에 리눅스 명령어인 "readeif"로 ELF

정보들을 읽어볼 수 있습니다．



먼저 "readelf" 명령에 도움말을 다음과같이 확인합니다．



readeif 껑령에 도욥많


$ readeLf-H

/／댜읗과 같이 화면에 출력됩니다，
Usage: readeif <option(s)> elf- file (s)
 Display information about the contents of ELF format files




커널연구회佃伽．kerneLbz)                                                     정재준（rgbi3307@nate.com)
                                               324/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                          percpu 이해


Options are:
 -a --all                 Equivalent to: -h -l -s -s -r -d -V -A -I
 -h - -file- header       Display the ELF file header
 -l - -program- headers   Display the program headers
    - - segments          An alias for --program- headers
 -s - -section- headers   Display the sections ' header
    - - sections          An alias for - -section- headers
    --section- groups     Display the section groups
  ：믄
    - -section- details   Display the section details
/／중간생략．.
 -w - -wide               Allow output width to exceed 80 characters
 @<file>                  Read options from <file>
 -H - -help               Display this information
 -v --version             Display the version number of readeif

                                                                      \\,,.



위의 옵션들중에서 -1옵션은프로그렐헤더절붚量量출력하고－S옵션은톤쁘on헤더겊봇듬을

출력합니다. 그리고 山V 옵션은 80 문자 이상 길게 화면에 출력합니다．



먼저 다음과 같이 " readelf -1 vmLinux" 명령으로vmLinux파일에 있는 프로그램 헤더 정보를 읽어서

화면에 출력합니다．



       x 프로그램 헤다정보 임까


$ readetf -I. vmlinux

/／댜음과 같이 화면에 출력됩니다，
Elf file type is EXEC (Executable file)
Entry point 0x1000000
There are 5 program headers, starting at offset 64

Program Headers:
  Type           Offset             VirtAddr            PhysAddr
                 FileSiz            MemSiz               Flags Align
  LOAD           0x0000000000200000 0xffffffff 81000000 0x0000000001000000
                 0x0000000001444000 0x0000000001444000 R E       0x200000




 커널연구회佃시八w.kerne나）기                                    정재준(rgb13307（亘）nate.com)
                                  325/ 351
                                                                리눅스 커널 소스 해실 ［기초입문］
                                                                           percpu 이해



  LOAD                0x0900000001800000 0xffffffff82609000 0x0000000002600000
                       0x0000000000258000 0x0090000000258000                  RW        0x200000
  LOAD                 0x0000000001c09000 0x0009000000000000 0x0000090002858009
                       0x0000000000025000 0x0000000000025900                  RW        0x200000
  LOAD                 Ox900000000lc7d000 0xffffffff8287d099 0x000000000287d000
                       0x000000000024d000 0x00000000097af 999                 RWE       0x200000
  NOTE                 0x00000090010014a4 0xffffffff8leol4a4                0x0000000001e014a4
                       0x00000000990001ec 0x00000000909001ec                            0x4

 Section to Segment mapping:
 Segm이止 Sec匕ons...
 00   .text .notes _ex_tabLe .rodata .pci_fixup .tracedata _ksymtab _ksymtab_gpl
      1虹聊ta느就rings _init_rodata 나汨ram _mo山er
 01   .data _bug_table .vvar
 02   .data..percpu
 03   .init.text .altinstr_aux .init.data .x86_cpu_dev.init .parainstruct向ns .altinstructions
      .aLtinstr_replacement .iommu_tabte .apicdrivers .exit.text
      .smp_Locks .data_nosave .bss .brk
 04   .notes



위에서 "Section to Segment mapping:" 부분을 보면 Sec匕on 들이 5 개의 세그먼트로 나누어져

있다는 것을 알 수 있고 Sect向n 들의 명칭도 확인해 볼 수 있습니다. 그럼 이러한 Section 들이

실제로 어떤 주소에 맵핑되는지는 아래와 같이 " readeif -S vmLinux" 명령으로 확인 합니다．




VE心flux Section 헤더청보 읽71

$ readeLf -s vmLinux

/／다욤과 같이 화면에 출력됩니다．
There are 74 section headers, starting at offset 0x25314a40:

Section Headers:
  [Nr] Name                       Type                    Address          Offset
       Size                       EntSize                 Flags Link Info Align
  [ 0]                            NULL                    9000009090000000 00000000




커널연구회佃쌔1w.kerne나）z)                                                      정재준（rgb13307@nate.con力
                                            326/ 351
                                                         리눅스 커널 소스 해설 ［기초입문］
                                                                            percpu 이해


       0000000000000000       0000000000000000               0    0     0
 { 1] .text                   PROGBITS           ffffffff8l000000   00200000
       0000000000e014a1       0000000000000000    AX        0        0        4096
   2] .rela. text             RELA               0000000000000000         lOdbcc90
       000000000078f 330      0000000000000018      I      71        1        8
   3] .notes                  NOTE               ffffffff81e014a4         010014a4
       00000000000001ec       0000000000000000      A       0        0        4
   4] .rela. notes            RELA               0000000000000000         ll54bfcO
      0000000000000048        0000000000000018      I      71        3        8
   5] _ex_ table              PROGBITS           ffffffff8leol69o         01001690
      0000000000006990        0000000000000000      A       0        0        4
   6] .rela_ ex_table         RELA               0000000000000000         1154c008
      0000000000027960        0000000000000018      I      71        5        8
   7] .rodata                 PROGBITS           ffffffff82000000         01200000
      00000000003f7ce2        0000000000000000   닙A         0        0        4096
/／중간섕략，,
[24] .data                    PROGBITS           ffffffff82600000         01800000
       0000000000243080       0000000000000000   낯A         0        0        8192
[25] .rela. data              RELA               0000000000000000         1175c7d0
       0000000000loeaf 8      0000000000000018      I      71       24        8
[26] 1 bug_tab1e              PROGBITS           ffffffff82843080         01a43080
       0000000000013c20       0000000000000000    WA        0        0        1
[27] . rela_ bug_table        RELA               0000000000000000         1186b2c8
       000000000004f 080      0000000000000018      I       71   26     8
[28] . vvar                   PROGBITS           ffffffff82857000   01a57000
       0000000000001000       0000000000000000   닙A         0        0        16
[29] . data. .percpu          PROGBITS           0000909009000900         91c90090
       0000099000025000       0009990090000090   닙A         0        0        4096
[30] .rela. data. .percp RELA          0000900090009000 118ba348
     0090000000000150 0000090090000018   I      71    29    8
 [31] . init.   text          PROGBITS           ffffffff8287d000         01c7d000
       000000000007c64e       0000000000000000    AX        0        0        16
 [32] .rela. init.     text   RELA               0000000000000000         118ba498
     00000000000d52b8         0000000000000018      I       71      31        8
/／중간생략．,
 [54] . bss                   NOBITS           ffffffff82aca000   oleca000
       0000000000536000       0000000000000000 WA          0    0     4096
 [55] .brk                    NOBITS             ffffffff83000000         oleca000
     000000000002c000         0000000000000000      WA       0        0       1
/／중간생략，,
 [71] . symtab                SYMTAB             0000000000000000         10971800




커널연구회佃시시／,kerne比z)                                               정재준（r야)i3307@nate.com)
                                         327/ 351
                                                   리눅스 커널 소스 해설 E기초입문］
                                                              percpu 이해



        000000000026ba10 0000000000000018              72   89624      8
  [72] .strtab             STRTAB           0000000090000000 l크bdd2lo
        00000000001dfa7d 0000000000000000               0     0      1
  [73] .shstrtab           STRTAB            0000000000000000 253147c0
        0000000000000280 0000000000000000               0     0      1
Key to Flags:
  W (write) , A (alloc) , X (execute) , M (merge) , S (strings) , I (info) ,
  L (link order) , 0 (extra Os processing required) , G (group) , T (TLS) ,
  C (compressed) , x (unknown) , o (OS specific) , E (exclude) ,
  1 (large) , p (processor specific)




출력 내용이 많아서 다소 복잡하1 보입니다만, "Section Headers:" 의 타이틀을 이해하면 내용을 쉽게

인지할 수 있습니다. 우선, "Section Headers:" 의 타이틀부터 설명 드리겠습니다．



Section Headers:
  [Nr] Name                 Type               Address              Offset
       Size                 EntSize            Flags Link    Info    Align



帥］은 출력된 Sect向n 순번입니다. Name 은 Section 이름이고 Type 은 Section 타입입니다．

A小打ess 는 Section 이 배치되는 주소입니다. Offset 은 이 Address 로부터 떨어진 주소 입니다．

그리고듸ze는Sect向n 의 크기 입니다. 마지막으로 디ags들은 다음과같습니다．




Sect

Key   to Flags:
  W   (write) , A (alloc) , X (execute) , M (merge) , S (strings) , I (info) ,
  L   (link order) , 0 (extra OS processing required) , G (group) , T (TLS) ,
  C   (compressed) , x (unknown) , o (Os specific) , E (exclude) ,
  1   (large) , p (processor specific)




커널연구회（蜘쌔／.kern이.bz)                                       정재준（rgbi3307@nate.com)
                                      328/ 351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                           percpu 이해



지금까지 리눅스 커널 소스가 빌드되어 있는 vmlinux 파일의 ELF 정보에서 Section 들을

확인했습니다. 그럼 이글의 주제인 "percpu와Section은무슨관계 일까요？" 위에서 출력한

Section 의 Name 필드를 자세히 본 독자분들은 그곳에 percpu 라는 명칭이 있다는 것을 확인했을

것입니다. Se比向n 순번 [29］에 다음과 같이 있습니다．



percp心뇨Ct徊a 확인

Section Headers:
  [Nr] Name               Type              Address              Offset
       Size               EntSize           Flags Link    Info    Align


  [29] . data. .percpu      PROGBITS        8000800080080808 01c00000
       0000000000025800     0000000000008000 WA        0     0    4096
  [30] . rela. data. .percp RELA             0000000000000000 118ba348
       0000080000008150 0000000800000018       工      71    29    8




.data..percpu 의 Ad（打ess 는 0000000000000000 입니다． 그리고 Offset 은 ] c00000 이고 Size

는 25000 이고 플래그는 W (write), A (alloc) 입니다．

.rela.data..percpu 의 Address 는 0000000000000000 입니다. 그리고 Offset 은 118ba348 이고

듸ze 는 ] 50 이고 플래그는 I (inf이 입니다．



리눅스 커널은 이곳에 해당 Cpu 전용의 percpu 변수들을 만들고 read/wi止e 작업을 합니다．

위와같이 percpu 7H념은 어렵지 않으나 이것이 메모리에 배치되는 공간인 Sect向n 에 대해서

설명하는 내용이 길어 졌습니다. 자 그럼 커널 소스를 확인해 보도록 하겠습니다. 커널 소스는

percpu 을 위한 Sect向n 에 각각의 CPU 마다 변수를 정의하고 그곳에 데이터를 읽고 쓰는 API

함수들입니다．




 커널연구회（www.kerneLb기                                      정재준（rgbi3307@nate.com)
                                    329/ 351
                                                              리눅스 커널 소스 해설 ［기초입문］
                                                                         percpu 이해




percpu 정의 하:7 '

percpu 는 아래와 같은 매크로를 사용하여 선언 및 정의합니다．




DECLARE_PER_CPU(unsigned long, u64_counter);      //percpu선언(extern)
DEFINE_PER_CPU(long, s64_counter);   //percpu 정의



위의 매크로는 다음과 같이 커널 소스 "力nclude/linux/percpu-defs.h"에 정의 되어 있습니다．




/include/tinux/percpu-defs.h

#define _PCPU_ATTRS(sec)                                                \
       _percpu _a比的먀已kSe由on(PER工메 BAS目또口口N sec)))                       \
       PER CPU AT기귀BUTES


#define DECLARE_PER_CPU_SECTION(type, name, sec)                  \
       extern _PCPU_ATTRS(sec) _typeof_(type) name


#define DEFINE_PER_CPU_SECTION(type, name, sec)                   \
      _PCPU_ATTRS(sec) _typeof_(type) name


#define DECLARE_PER_CPU(type, name)                       \
      DECLARE_PER_CPU_SECTION(type, name, ")


#define DEFINE_PER_CPU(type, name)                    \
      DEFINE_PER_CPU_SECTION(type, name, ")




커널연구회（www.kerne나끄）                                                정재준（rgbB307@nate.com)
                                      330/ 351
                                                     리눅스 커널 소스 해설 ［기초입문］
                                                                percpu 이해



그리고 PER CPU BASE SECT山N 매크로와 PER CPU ATTRIBUTES 매크로는 다음과 같이 커널

소스 "力ncLude/asm-generic/percpu.h"에 정의 되어 있습니다．




/inctudelasm-generic/percpu.h


斛fndef PER CPU BASE SEC丁幻N
＃仟defCONFIG S卜샤＞
#dehne PER_CPU_BASE_SECTION ".data..percpu"
#else
#defirie PER CPU BASE SECTION ".data ''
#ead汗
#endif


#ifndef PER CPU ATTRIBUTES
#define PER CPU ATTRIBUTES
#end汗




위와 같이 리눅스 커널 소스는 매크로 정의들이 계속 이어지는 것들이 많아서 소스를 해석 하기가

상당히 까다롭습니다. 그러나 컴파일러는 그냥 매크로 정의들을 순서대로 치환하1 가면 되니까

복잡하지 않게 처리 합니다．




위의 DECLARE_PER_CPU 매크로가 치환되어 가는 과정을 추적해 보도록 하겠습니다． 컴파일러는

다음과 같은 순서로 매크로들을 치환합니다．




DECLARE_PER小CPU 매크로 치환 과정


DECLARE_PER_CPU(unsigned Long, u64_counter); //percpu J언




  커널연구회佃쌔쌔／.kerne냐파                                        정재준（r야)13307@nate.com)
                                          331 /351
                                                            리눅스 커널 소스 해설 ［기本입문］
                                                                       percpu 이해


        DECLARE_PER_CPU_SECTION(type, name, ")
               extern _PCPU_ATTRS(sec) _typeof_(type) name
                       _percpu _attribute_((section(PER_CPU_BASE_SECTION sec)))
                               PER工Pu寸帥또jECT山N ".data..percpu'


이렇게 컴파일러에 의해서 치환되면，

DECLARE_PER_CPU(unsigned Long, u64_counter); //percpu 선언

는 아래와 같이 최종적으로 치환된 코드가 만들어 집니다．

extern _percpu _attribute_((section(".data..percpu")));



위에서 _percpu 는 "力nc山de/Linux/compiLe口四pes.h"에 정의되어 있는 매크로에 의해서 다시

치환됩니다．



／如cL써e/Iinux／的 1爪er_t卯es.h

# define _percpu       _attribute_((noderef, address_space(3)))




여기까지 매크로 치환되면. 최종적으로 다음과 같은 코드가 생성 됩니다．

extern _attribute_((noderef, address_space(3))) _attribu te_((section(".data..percpu")))
       unsigned Long u64_counter;



위에서 H attr小ute1는 컴파일러 확장 속성으로 이미 앞의 글 "오류：챰조 소스를 찾을 수 없습니다"

에서 설명 드렸습니다. 이와 관련해서 GCC 문서（매뉴얼）을 참조하셔도 되겠습니다． 결국 위의 코드는

컴파일러가목적코드를 만드는 ELF파일의 ".data..percpu" Section에 addres乞space(3）의 위치에

unsigned Long 형의 u64Hcounter 변수가 extern 으로 선언되는 결과 입니다．




커널연구회佃쌔시／.kerne比z)                                                  정재준（rgbi3307@nate.con寸
                                         332/ 351
                                                       리눅스 커널 소스 해설 ［기초입문］
                                                                  percpu 이해




지금까지의 설명은 컴파일러에 의해서 치환되는 매크로와 "오류：참조 소스를 찾을 수 없습니다",

그리고 "ELF Sections 이해"에 대해서 알고 있으면 어렵지 않게 이해할 수 있는 내용입니다． 이들에

대해서는 이미 앞에서 모두 설명했기 때문에 한번더 확인해 주시기 바랍니다. 여기까지 이해하셨다면

리눅스 커널 소스를 앞으로 쉽게 쉽게 분석할 수 있는 능선을 넘어 가고 있는 것입니다．




percpu 사용 하71

이제부터는 percpu 변수를 정의한 것을 가지고 사용（연산）하는 방법에 대해서 설명 하도록

하겠습니다. percpu 변수를 아래와 같이 매크로 정의 하면，



DEFINE_PER_CPU(Long, s64_counter);


이 매크로는 컴파일러에 의해서 다음과 같은 코드로 최종 치환됩니다．



_attribute.. ((noderef, address_space(3))) _attribute_((section(".data..percpu")))
       long s64_counter;



결국 Log형의 s64_counter변수가 ".data..percpu" Sec匕on에 정의되는결과입니다． 이곳에 있는

변수의 값을 읽고, 쓰고, 연산하71 위해서는 커널 소스 "力nclude/Linux/percpu-defs.h" 파일의 440

라인부터 정의되어 있는 매크로 함수들을 다음과 같이 사용합니다．



_this_cpu_read(s64_counter);              // s64mcounter값을 O1음．
_this_cpu_write(s64_counter, 0);          1/ s64_counter 011 0 을 X1L




 커널연구회佃쌔쌔／.kernet,뇨）                                           정재준（四bi3307@nate.com)
                                       333/ 351
                                                                          리눅스 커널 소스 해설 ［기초입묜］
                                                                                     percpu 이해


     Hthi乞cpu_add(s64卜counter, 1);                               //s6소工ounter값에 1 을더함．


     月ncti川e/Linux加ercpi卜de氏h
          ／央
               央 Operat幻ns 向r contexts that are safe from preen耳出or們nter叫炳． These
               * operations verify that preemption is disabled.
               央／
                                                          \\\\
      #define _thi乞印止read(pcp)
      ({
                      1this1叩止preem야_check("read");
                      raw_cpu_read(pcp);
     })

     #define _this_cpu_write(pcp, vat)
     ({
                     1thisU印比마eem야_check("write");
                      raw_cpu. .write(pcp, vaL);
     })




                                                                                              \\\\
     #define 寸t眺e叩u_add(pcp, vat)
     ({
                      _this_cpu_preempt_check("add");
                     raw_cpu_add(pcp, vat);
 })


위에서 주석문으로 설명하고 있는 내용부터 잠깐 보겠습니다．

／央
     * Operations for contexts that are safe from preemption/interrupts. These
     * operations verify that preemption is disabled.
     士／
          커널연구회（叫쌔／.kerne比z)                                                   정재준（rgb日307@nate.com)
                                                         334/ 351
                                                            리눅스 커널 소스 趨솰 呈카箋압문］
                                                                       percpu 이해



함수 동작들이 선점이나 인터럽트들로부터 안전해야 하고, 선점（preemption）이 비sabled 로 되어

있어야 한다라는 것입니다. 이와같은 이유로 매크로마다1냔)iSe叩u_preem야_check() 들이

있습니다．



/incLude/tinux/percpu-defs.h (310 lines)

崩叱ef C（그NF!G DEBUG PREE卜lP丁
extern vo너 1베乞叩U아eem야:_check(const char 火op);
#e(se
static inline void _this_cpu_preempt_check(const char *op) {}
#end作




1가is_cpu_preem야_check() 함수는 커널 설정 상수 CONFIG_DEBUG_P REEMPT 가 정의 되어

있을따1 동작합니다. 그런데 보통 CONFIG DEBUG PREE卜4PT는 정의 되어 있지 않습니다. 위의

내용을 디버그하여 검증하고 싶다면 커널 menuconfig 메뉴어납I CONFIG_DEBUG_PREEMPT 을

"Yes" 로 설정하여 커널을 재 컴파일해야 합니다. 일반적으로 이 함수는 동작하지 않으므로 percpu

관련 함수를 실행하기 전에 preem야_disable() 합니다. 그런다음 percpu 관련 함수 실행이 끝나는

곳에서 preem야_enabte() 합니다. preempt enable/disable 에 대해서는 나중에 커널 스케쥴러

진도 나갈따1 설명하는 시간을 가지도록 하겠습니다．



이제 나머지 남아 있는 함수들은 420 라인부터 다음과 같이 매크로 정의 되어 있습니다．



/incLude/linux/percpu-defs.h (420 lines)

#define raw_cpu_read(pcp)             _pcpu_size_catt_re山rn(raw_cpu_read_, pcp)
#define raw_cpu_write(pcp, vat)       1口c叩_size_ca tt(ra吐c口이쌔te나 pcp, vat)
#define raw_cpu_add(pcp, vat)          _pc四size1떼m帥_cpu詞d교 pcp, vat)




 커널연구회 (w낚八차.kerr泡,b기                                             정재준(rgb1330끄孕陷te.com)
                                           335/ 351
                                                                                 리눅스 커널 소스 해설 E기초입문］
                                                                                            percpu 이해




위에서 _pcpu_size_ca比return() 함수는 다음과 같이 引6 라인부터 매크로 정의 되어 있고，

-pcpu卞size_call() 함수는 373 라인부터 매크로 정의 되어 있습니다．




月nc如de/Unux/percpu-de?s.h (316, 373 Lines)

#define _pcpu_size_caLl_return(stem, variable)                               \
({                                    \
      typeof(variabLe) pscr_retj                             \
     H verif느匹叩ptr(&(va na바이）;                                   \
      switch(sizeof(variable)) {                        \
              case 1: pscr_ret_ = stem##1(variable); break;
              case 2: pscr_ret_ = stem##2(variable); break;
              case 4: pscr_ret_ = stem##4(variable); break;
              case 8: psc口et_ = stem##8(va巾닌이；break;
              defau比                                     \
                  1mbad血已ca比parameterO; break;
      }                               \
      pscr_retj                                   \
})

#de日ne _pcpu_size_calt(stem, variabLe, ...)                              \
do{                                       \
     寸verify_i乂叫_ptr(&(variable));                               \
      switch(sizeof(variable)) {                        \
          case 1: stem##1(variable, _VA_ARGSJ;break;
          case 2: stem##2(variable, _VA_ARGSJ;break;
          case 4: stem##4(variable, _VA_ARGSJ;break;
          case 8: stem##8(variabLe, _VA_ARGSJ;break;
          defau比                              \
              1 bad竝已臼LI叩rameterO;break;                             \
     }                                \



 커널연구회佃쌔쌔／.kerne나끄）                                                                  정재준（r야出3307(回aate.com)
                                                      336/ 351
                                                       리눅스 커널 소스 해설 [71초입문］
                                                                  percpu 이해


} while (0)




위에서는 C 언어 매크로 문법 #＃이 등장 했습니다. 이것은 #＃의 앞에 있는 키워드와 뒤에 있는

키워드를 서로 붙이는 역할을 합니다． 그리고，sizeof佃카治비e)0們 variabLe 은 Long 형의 데이터

타입 s64_counter이므로 8 입니다. 따라서 _pcpu_size_caLL_return(raw_cpu_read_, pcp）은

다음과 같이 치환 됩니다．



pscr_ret_ = raw_cpu_read_8(pcp);



이 함수는 커널 소스 "/arch/x86/incl내Je/asm/percpu.h" 파일의 469 라인부터 다음과 같이 정의

되어 있습니다．



/arch/x86/inctude/asm/percpu.h (469 Lines)

#define raw_cpu_read_8(pcp)         percpu_Frommop( 'mov", pcp)
#define raw_cpu_write_8(pcp, vat)   percpu_to_op("mov", (pcp), vat)
#define raw_cpu_add_8(pcp, vat)     percpu_add_op((pcp), vat)



지금까지 설명을 따라 오셨나요7 이쯤에서 느끼고 계시겠지만, 커널 소스는 매크로에 매크로

치환하는 과정이 계속 반복되는 소스가 많습니다. 그래서 매크로 치환을 따라 가기가 좀

번거롭습니다. 그래도 단순히 반복해서 치환하는 과정입니다. 공학적으로 복잡한 수식이 있는 것도

아니고 그냥 코드를 계속 치환하면 됩니다. 이제 매크로 치환의 막바지에 왔습니다．




  커널연구회（ww比kerneLb기                                               정재준（r야)i3307@nate.com)
                                     337/ 351
                                                                     리눅스 커널 소스 해설 ［기초입문］
                                                                                percpu 이해



percpu_from_op("mov", pcp）을 보겠습니다. 여기서 pcp 가무엇인지 위의 내용에서 기억하고

계시나요7 바로s64_counter변수입니다. percpu_from_op("mov", pcp) 매크로함수는커널 소스

"/a rch/x86力ncLude/asm/percpu.h" 파일의 183 라인부터 다음과 같이 정의 되어 있습니다．



/arch/x86/incLude/asm/percpuh (183奴nes)

#define percpu_from_op(op, var)                               \
({                                \
     typeof(var) pfo_retj                             \
     switch (sizeof(var)) {                       \
     case 1:                          \
         asm volatiLe(op "b "_ percpu_arg(l)",%O"\
           : "=q" (p10HretJ                   \
           : "rn ' (var));                \
         break;                       \
     case 2:                          \
         asm volatiLe(op "w "_percpu_arg(1)",%O"\
           : "=r" (pfo_ret....j               \
           : "rn' (var));                 \
         break;                       \
     case 4:                          \
         asm vo(atiLe(op "1 "_ percpu_arg(l)",%O"\
           : "=1" (pfo_retmJ                  \
           : 'rn" (var));                 \
         break;                       \
     case 8:                          \
         asrn voLatiLe(op "q "_percpu_arg(l)",%O"\
           : "=r" (pfo_retj                   \
           : "rn' (var));                 \
         break;                       \
     defauLt: _bad_percpu_sizeQ;                          \
                                  \
                                          \



 커널연구회（www,kerne나）z)                                                     정재준（rgb13307@nate.con分
                                                          338/ 351
                                                               리눅스 커널 소스 해설 ［기奈입문］
                                                                          percpu 이해



})



결국 asm volatite(...) 형태의 x86 인라인 어셈블리 코드입니다． 이제 다 찾아 왔습니다． 이 코드를

이해 하시면 됩니다. 인라인 어셈블리 코드 문법은 아직 자세히 설명하지 못했습니다만， 아래의 GNU

gcc 온라인 매뉴얼에 잘 설명되어 있습니다．




Assembler Instructions with C Expression Operands: 10 ix
h ttps:/Ig cc.g flu.orq/oritinedocs/gcc/Exte nd ed-Asm.h tm L#index-asm-assemb(er-templa te



x86 인라인 어셈블리 기본 문법은 다음과 같습니다．




asm 기본 문법

asm asm-quatifiers (AssemblerTemplate
         : OutputOperands
         [: InputOperands
         [:Clobbers] 1)


asm asm-qualifiers (AssemblerTemplate


           : InputOperands
           : C［야巾ers
           :GotoLa bets)




percpu_from_op("mov", pcp) 는 percpu_from_op佃p, var) 로 매크로 치환되면서 op는 " mov"

이고 var 는 pcp 입니다. pcp 는 s64_counter 변수이므로 引zeof(var）는 8 입니다．




 10 참고문서 참조



     커널연구회佃W床erneLbz)                                                    정재준（r야)13307@nate.com)
                                             339/ 351
                                                           리눅스 커널 소스 해설 ［기초입문］
                                                                      percpu 이해


따라서 위의 매크로에서 치환되는 인라인 어셈블리 코드는 switch case(8）에 해당하는 다음과 같은

코드가 됩니다．



       case 8:
        asm volatile(op "q "_ percpu_arg(l)",%0"\
          : "=r" (pfo_ret......)      \
          : 'rn" (var));


위의 코드는 다음과 같이 전개 됩니다．

asm votatile("movq _percpu_arg(1), %0" : "=1" (pfo_ret.....) : 'rn" (var) );

asrn volatile("rnovq ""%%"gs": " "%" "1"",%0" : "=r" (pfo_ret그 : "rn ' (var));



이 코드를 설명하면, _percpu_arg(1）은 입력용 InputOperands인 " rn' (var) 입니다． 이것은var

에 전달한 s64_counter 메모리 변수입니다 .%0 는 출력용 OutputOperands 이므로 pfo_ret_에

s64_counter 메모리 변수값이 movq 에 의해서 전달됩니다. 결국 s64_counter 값이 pfo_ret_에

전달되어 리턴 됩니다．



지금까지 매크로 치환 때문에 설명 내용이 상당히 길어 졌습니다. 그러나 percpu 동작은 간단합니다．

percpu 정의는section(".data..percpu") 영역에 메모리 공간을 할당하는 것입니다 ．그리고 이곳에

접근하는 동작들（read, write, add, and, or...）은 매크로 함수로 만들어 졌으며，결국은 아래와 같은

인라인 어셈블리로 치환되어 동작합니다．



asm v아atile("명령 _percpu_arg(#), %0" : "=r" （출력변수） : ''rn '' （입력변수）);




 커널연구회佃八사姚,.kern日.bz)                                              정재준似狗i3307@nate.com)
                                          340/ 351
                                    리눅스 커널 소스 해설 ［기초입문］
                                                 percpu 이해


이번글은 이쯤에서 마무리 하겠습니다. 이번 주제는 설명하기 상당히 까다로워서 정리하는데 꽤 많은

시간이 걸렸습니다. 최대한 이해하기 쉽게 풀어서 기술 했습니다만, 내용이 잘 전달 되었는지

모르겠습니다. 그럼 힘내서 다음글에서 뵙겠습니다．




 커널연구회（＼사낚／낚／.kern이.b까                  정재준（rgb13307回nate.com)
                         341 /351
                                                리눅스 커널 소스 해설 ［기초입문］
                                                        percpu 소스 분석




percpu 소스 분석

바로 앞장에서 설명한 " percpu 이해"는 percpu 를 이해하고 사용하는 관점（A미）에 대한 내용

이었습니다． 이번 장에서는 percpu 내부 코어 소스를 좀더 심도있게 분석하여 정리하도록

하겠습니다． 리눅스 커널어녀1현되어 있는 percpu 소스들은 mm/percpu.c 에 있습니다． 그리고

percpu 에서 사용하는 자료구조인 구조체들은 inc山de/Linux/percpu.h 헤더파일과 mm/percpu-

interna나）에 정의되어 있습니다. 먼저 口ercpu 에서 사용하는 구조체부터 정리 하도록 하겠습니다．




percpu 구조체

percpu 는 다음과 같이 4 가지 종류의 구조체들을 사용합니 다．



incL拉d兮月a,仙x／加作阿h塑中准의恥加코奴info卒조쳬
struct pcpu_alloc_info {
    size_t          static_size;
    size_t          reserved_ size;
    size_t          dyn_size;
    size_t          unit_size;
    size_t          atom_size;
    size_t          alloc_size;
    size_t          _ai_ size; 1* internal, don 't use *1
    mnt         nr_groups; 1* 0 if grouping unnecessary *1
    struct pcpu_group_info groups[ ];
};


inch刈可心I世蚣加作만j.h헤더파밑와p節立四r刎L如忙 구胡
struct pcpu_group_info {
    mnt                  nr_units;    /* aligned # of units *1
    unsigned long        base_offset;     /* base address offset */




커널연구회佃m쌔／.kerneL.b킥                                   정재준（rgbi3307(@nate.com)
                                 342/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                              percpu 소스 분석




          unsigned mnt          *cpu1map;   /士 unit->cpu map, empty
                                 * entries contain NR CPUS *1
1;
mm／食舒cpu-internaLh 헤더파앝의 pcpu_chunk쿠조쳬
struct pcpu_chunk {
#ifdef CONFIG PERCPU STATS
    mnt         nr_alloc;   1* # of allocations */
    size t          max_alloc_ size; /* largest allocation size 六1
#endif

          struct list_ head     list;       /* linked to pcpu_slot lists *1
          mnt          free_bytes; /* free bytes in the chunk */
          mnt          contig_bit s;    /士 max contiguous size hint *1
          mnt          contig_bits_start; 1* contig_bits starting
                                      offset 玄／/
          void              *base_addr; /* base address of this chunk *7

          unsigned long        *afloc map; 1* allocation map *1
          unsigned long        *boundemap; /* boundary map *1
          struct pcpu_block_md      *md blocks; 1* metadata blocks *7

          void                차Jata;      ／玄 chunk data 女／
          mnt            first_ bit;  /* no free below this *7
          bool                immutable; /* no [de]population allowed */
          mnt            start_offset;    /* the overlap with the previous
                                     region to have a page aligned
                                     base addr 女／
          mnt            end_offset; /* additional area required to
                                    have the region end page
                                    aligned 出／

         mnt         nr_pages;   1士 # of pages served by this chunk */
         mnt         nr_p야）ulated;   ／女 # of p이：)ulated pages 士／
         mnt                     nr_empty_pop_pages; /士 # of empty populated
     pages 女／
         unsigned long       populated[ ];   /* populated bitmap */
     };




      커널연구회（＼사니쌔／.kerne나끄）                                     정재준（rgbi3307@nate,com)
                                          343/ 351
                                               리눅스 커널 소스 해설 ［기초입문］
                                                       percpu 소스 분석



拉州恥作p小杯te如La胡同發質聲p節蜘姆奴加d染丕쳬
struct pcpu_block_md 4.
    mnt     contig_hint;    1* contig hint for block */
    mnt     contig_hint_start; 7* block relative starting
                              position of the contig hint *7
    mnt     left_ free;     1* size of free space along
                           the left side of the block *1
    mnt     right_free;     /* size of free space along
                           the right side of the block */
    mnt     first_ free;    /* block position of first free 六1
};


percpu 내부 코어 소스를 이해하기 위해서는 위의 4 가지 구조체안에 있는 멤버 변수들간에 상호 연산

작용을 이해해야 합니다. 구조체 멤버변수들이 많아서 처음에는 좀 복잡해 보이겠지만 하나씩

이해하여 논리적으로 정리하는 것이 중요합니다. 우선 위의 구조체들을 아래와 같이 데이터베이스

분석에서 많이 활용하는 ERD 다이어그램 형태로 정리하도록 하겠습니다. 이렇게 하면 자료구조

안에서 데이터들의 흐름을 좀더 시각화하여 쉽게 이해할 수 있습니다. 필자는 앞으로 이러한 방식으로

커널 소스들을 해설하도록 하겠습니다．
                                         p댜川_chunk
                                     nr 체oc
                                     max 체oc 引ze
percpu 구조쳬 정리                        list
                                     free_bytes
                                     contigHbits
pcp比해解；jn幻                           contigHbits_start
static size                          *base addr
reserved size
                                     女alto（乙map
dyn_size                             仕ound_map
Un仕 針ze
                                     *md1blockS 0           卜 pcpu..btodc叫md
atom 引ze                                                       contig1hint
                                     *data
체oc 針ze                                                        contig..hint_start
                                     first b仕
m=a匕size                                                       left free
                                     immutabte
nr_.groups                                                     right_free
                                     sta八 offset
groupsfl      .                      end offset                first free
                  nr units
                  base offset        nr_pages
                                     nr_populated
                  cpu_map
                                     nr帥巾勺_p야)_pages
                                     popu[atedD




커널연구회佃쌔쌔／.kerne比z)                                       정재준（rc拘日307@nate.com)
                                344/ 351
                                                   리눅스 커널 소스 해설 ［기초입문］
                                                           percpu 소스 분석



위에서 pcpu_alloc_info 구조체와 pcpu_group_info 구조체 멤버들의 연결관계를 좀더 자세히 정

리하면 다음과 같습니다．




           inctud可linu町perc口u.h, mm/i昶r叩u,c. 口cpu_embed_枷盛-c奴m川I
                         =        r        =   =          ＝乙小   小艮小恥碼




        아洲_aUocjn匈
        static s注e
        reserved size
        dyn中S注e
        Un吃多往e
        atom 닯ze
        aHoc牛S注e
          at 돠ze




        ptr二 a!的c(c다J! ni小units 希 unit_size)
                                                                 base
        areas晤roupj 二 ptr
                                                              base addr
        base二 min(ptr, b社se)
                                                            PC까I.由a弊J出r
        g心們陌ou바base꼬作蚣t二 area卦鄧出Pj 卄岫e




위에서 pcpu_setup_firs t_chunk() 함수에서 pcpu_chunk 구조쳬에 멤버들을 연결되는 과정을

정리하면 다음과 같습니다．




 커널연구회（w니시l.a但rnel.b力                                  정재준佃如i3307@nate.com)
                                345/ 351
                                                 리눅스 커널 소스 해설 [71초입푼I
                                                         percpu 소스 분석


                         mm/percpu-internaLhr: mm/percpu.c, pcpu玉猷U机fh攷工椰nk8




                         nr altoc
  listmhead ' 肛四S幻t
                         max 出h그（ 돠ze
     蜘沁nr如S       仁      List
  1161 卜re단姓ytes         如프尸 b法es
  [cx기      4            conti臣bits
  [0치       8    年5+2    conti已bi朽小我art                                  尹艸料呼
  102]     16    5-5+2   1base addr
                                                                  y？
  (03]                                                                       pCpu-in吐，md.b幻C
           32            '欲油C凹map            筐딴）兀飯二
  1041     64            't均und따m叩
  1051                   bY넘上佃cks            旦！工多甲＄     ..          bl。 ckmd
  106]
                                                             P.        pu.
                         *data
                                                    '
                                                             contigjiint
  [071     512           伽st b吐                              c그ntig_hint_start
  [081    1024           immutable                           ieft_free (idx)
  (09)    2048           start o行set                         ngt也打ee (idx)
  11이     4096           end 王貫朽et                           h陌t加이cnt)
  [11)    8192           nrpages
  [121   16384           nr叩pulated
  [13]   32768           nrer巾却-pop-節ges
  [14]   65536           p이乂ilated(j

                         __attoc_percpu
                         pcpu_alloc
                         肛四a如C카ea
                         pcpu create chunk




커널연구회（www.kerne［뇨）                                           정재준（r的3307@nate.com
                                  346/ 351
                                                      리눅스 커널 소스 해설 ［기초입문］
                                                              percpu 소스 분석




pcpu 함수 실행 흐름

pcpU 자료구조에 해당하는 구조체 멤버들의 연결관계를 어느정도 파악하면 pcPU 에서 데이터들을

어떻게 취급하는지 이해할 수 있게 됩니다. 하지만 데이터들의 흐름과 연산과정은 알고리즘에 따라서

실행되는 함수들의 흐름을 알아야 합니다. 아래는 필자가 pcpu 에서 함수들이 실행되는 흐름을

중요한 것만 정리한 것입니다. 세로방향은 함수가 호출되는 순서이고 가로방향은 함수안에서 하위

함수를 또 호출하는 깊이에 해당합니다．



pcpu 에서 함수돌이 실행되는 흐룝
   SOURCE ALE                                   我JNCT好N CALL
init/main.c          start kernel(}      !
mmfpercpu.c         ;,,m,*놔 弊如瓦慰뇨르텬L建塑蟹皿；                                 小   “
                                                                                        11
                                    肛puembe也枷宬_chunk()                                  1
                                                                                        r
                                           PC트｝umbuild콰b c ia把重j                        !
                                                                                        1
                                                                                        !

   urn拱／men化的心（.h                         menibk그ck 出幻c{
                                                                                  H1'
    mm/n挺m뱌乂k.c                                  men化lock 謐心Ct四 nk玲
                                                          rnembbo比 戡locjntefl磁0
                                                                                        !
                                          休pu-s母如瓦枷攷 ch逃蛇
                                                pcpumaflocjirst chunk



                    H닒奴-p酊C.鉀 , 斟奴忍缸多啣nan妊C PC띠允 恁rea
                    恥叩aUoc()
                        工珏트）ujind hi


                                m.aUoc_ rea()




mm/percpu.c 소스 파일에서 위의 함수들이 실행되는 흐름을 따라 가면서 분석해 보면 pCpu

함수안에서 데이터들이 처리되는 과정을 이해할 수 있습니다．




 커널연구회（w'시／.kerneLb라                                           정재준(rgb13307會n就e.com)
                                     347/ 351
                                     리눅스 커널 소스 해설 ［기초입문］
                                             percpu 소스 분석


소스 내용이 방대해서 모든 내용을 설명하지 못해서 아쉽지만. 앞으로 소스를 좀더 분석하여 설명을

꾸준히 추가해 보도록 하겠습니다．



이번 집필 과정에서는 이정도로 소스 설명을 마무리 하도록 하겠습니다. 앞으로 지속적으로 커널

소스를 분석하고 정리한 내용들을 시리즈 형태의 책으로 출판할 예정입니다. 아울러 커널연구회

홈페이지（www.kerne나）기에서도공유할예정입니다. 많은성원과참여 부탁드립니다．



책에 대한 개선사항이나 기타 의견 및 궁금한 점들은 저자(rgbi3307@nate.com）에게 메일 주시기

바랍니다．



감사합니다．




커널연구회（www.kerneLbz)                       정재준（rgbi3307@nate.com)
                         348/ 351
                                                       라눅스 커널 소스 해설 ［기초입문］
                                                                     참고 문서




참고 문서

리눅스 커널 설명 문서：

https://www.kernel.ora/doc/html/tatest/index.html



리눅스 커널 소스 코딩 형식：

https:I/ www.kernel.orci/doc/htmt/latest/processJcoding-style.htmL



Bootlin Docs:

https://bootlin.com/docs/



Eli川I口oss Referencer:

h ttps://elixir.bootlin.com/Linux/latest/souice




커널연구회 이thub（소스공유）

ht印s://g附山b.com/kerne卜bz




책에 대한 개선사항이나 기타 의견 및 궁금한 점들은 저자(rgbi3307@nate.com)에게 메일 주시기

바랍니다. 감사합니다．




  커널연구회（V川시／.kernet.b라                                          정재준（rgbi330恥孕nate,com)
                                          349/ 351
I        커널 소스 코딩 형식

         https ://닙ww. kernel. org/ doc/html/latest/process/ coding- styl.e.html



ii         리눅스 커널 성능평가 도구들

         http:IIw.i寸. b rendang regg . com/ ebpf . html



iii        리눅스 커널 성능 평가도구 perf

         httD: //w山V. brendangregg. com/linuxperf. html.



iv         User space memory access from the Linux kernel.

         https: //www. ibm. com/ developerworks/library/l- kernel-memory- acceSs/indeX.htIfll



    v      Introducing the eXtensible Array (xarray)

         https : //lwn. net/Articles/715948/



    vi     userspace RCU (read- copy- update) library

         https : /Iliburcu . org/



    vii ELF (Executable and Linkable Format) :

         https :1/ en .wikipedia . org/wiki/Executable_and. .Linkable_Format#/



    viii    Special sections in Linux binaries:

         https :Illwn . net/Articles/531148/



    ix     Assembler Instructions with C Expression Operands:

         https: //gcc. gnu. org/onlinedocs/gcc/ Extended- Asm. html#indeX- asm- asSembler-
         template
                                                 社   구
                                                      寸音
                                                     4




책에 대한 개선사항이나 기타 의견 및 궁금한 점들은 저자（rgbi3307@nate.com）에게 메일 주시기

바랍니다. 감사합니다．
최신 리눅스 커널 소스를 단계벌로 쉽게 풀어서 설명하는



리눅스커널쑈해설          First Edition


                                  기초입문
                                      정재준 지음




                              I 리눅스 커널 소스 빌드 및 버전관리 방법

                              S 커널 소스 데이터 타입 및 비트연산 이해

                              S 커널 모듈 프로그래밍 방법

                              I 커널 성능측정 도구（口erf, ftrace, crash)

                              I 커널 소스 디버깅 방법（如robes, debug objects)

                              I user copy 소스 설명

                              I list sort 소스 설명 및 테스트 방법

                              I red-black tree 소스 설명 및 API 사용방법

                              I xarray, radix tree 소스 설명 및 API 사용방법

                              I IDA, IDA 소스 설명 및 API 사용방법

                              I percpu 소스 설명


                           Copyright (c) 커널연구회（www.kernel.b기




                                                   II I                  값 28,000원




                                                H0n 1
                                                                          93560




       납연구회                                    9 788997 750139
＼사w＼차二kerne1.bz                                 ISBN 978-89-97750- 3 9
  捕”

