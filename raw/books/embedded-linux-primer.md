---
source_url: /run/media/yutae/Data/임베디드 리눅스 입문.pdf  # USB PDF (local-only; raw/books/embedded-linux-primer.pdf gitignored)
ingested: 2026-11-07
sha256: c7deea51b5ba50adb28b542a36bcb58874dc12164fcbf87e963a3f51aadbb9eb
---

# 임베디드 리눅스 입문 (raw source)

## Book metadata
- **Title:** 임베디드 리눅스 입문
- **Authors:** 크리스토퍼 할리내(Christopher Hallinan) 지음 · 강덕진 옮김
- **Original:** Embedded Linux Primer (Newnes, 2nd ed., 2008)
- **Korean publisher:** 정보문화사
- **Year (KR):** 2008
- **Pages:** 632 (pdfinfo)
- **kind:** text-layer (pdftotext -layout extraction 2026-11-07)
- **note:** cover page is OCR-garbled; body has text layer but carries some OCR artifacts, especially CJK/numerics. Cross-check against the local raw/books/embedded-linux-primer.pdf for exact values.

## Full text (27392 lines)
                                                 /
                      I                      I




                                            四
                                        \




         己                           人
                                 L




Christopher Hallinan 지음 강덕진 옮김




                                         匹뇨熙났 區정보문회사
                                     H 訊닯：
                                  I
                                 근I



Christopher Hallinan 지음 강덕진 옮김




                                 .. Pp戶，沙，曾,, 少，卜，LN 落정불星횡샨
                                     임베디드 리눅스 입문


                                     Korean language edition published by Information Publishing Group,
                                     Copyright 姮） 2008

                                     본 저작물의 한국어판 저작권은 Pearson Education, Inc. 와 정보문화사
                                     간의 계약으로 정보문화사가 소유합니다. 저작권법에 의하여 한국 내에서
                                     보호를 받는 저작물이므로 이 책의 일부 혹은 전체 내용을 정보문화사
                                     발행인의 서면 동의 없이 무단으로 복사, 복제 , 젼재 , DTP, 인터넷 상에
                                     게재하는 것은 저작퀀법에 저촉됩니다．



                                     Authorized tran늬ation from the Engli寸1 language e批ion, entriled
                                     EMBEDDED LINUX PRIMER: A PRACTICAL REAL-WORLD APPROACH,
                                     1st Edition, 이引旬9848 by HALLINAN, CHF키STOPHER, put小shed by
                                     Pearson Education, 1nc, publishing as Prenti氾 Hall, Copyright (D 2007

                                     All rights reserved. No part of this book may be reproduced or transmitted in
                                     any 幻rm or by any means, 이ec打onic or mechanical, inclu네ng ph아oc야）ying,
                                     recording or by any information storage retrieval system, without permission
                                     from Pearson Education, Inc.




초판 1소H 인쇄   2008년 7월 5일
초판 ］쇄 발행    2008년 7월 10일
저자          Christopher Hallinan
역자          강덕진
발행인         이상만
발행처         정보문화사
주소          서울 종로구 동숭동卜81
전화          (02)3673-0037 "9（편집부）/
            3673-0114(Lfl)
팩스          (02)3673-0260
등록          제］너이3호
ISBN        978-89-5674-437-7
가격          23,000원
임베디드 장비는 사실 우리가 알고 있는 것보다 훨씬 오래 전부터 우리와 함께 존재
해 왔습니다. 시민들의 발이 되고 있는 지하철만 해도 수백 대 이상의 임베디드 장
비들로 이루어져 있고, 자동차 역시 많은 임베디드 시스템이 들어가서 묵묵히 자신
의 일을 수행하고 있습니다．

이 책을 번역하면서도 임베디드 기기의 도움을 받았습니다. MP3 플레이어로 음악
을 들으며 지루함을 달랬고, 어려운 표현은 전자사전의 도움을 받았으니 말입니다．

임베디드는 그 성능적인 면에서나 기능적인 면에서 엄청난 발전을 거듭하고 있습니
다. 우리가 더 이상 하드드라이브의 크기를 남들에게 자랑삼아 이야기하지 않듯이
임베디드 장치도 미래에는 더 이상 프로세싱 파워가 문제되지 않을 정도로 빨라질
것입니다. 물론 지금도 충분히 빠른 기기들이 넘쳐나고 있습니다. 이처럼 빠른 시스
템 , 다양한 기능이 요구되는 시스템에는 그에 걸맞은 운영체제가 매우 중요합니다．

기존 임베디드 시스템에서 사용되고 있는 많은 수의 운영체제들은 너무 간단하고，
기능이 극히 제한되어 있습니다. 이는 기술력이 부족하기 때문이 아니라 단지 해당
시스템 , 목적 , 성능에 맞게 최적화되어 있기 때문입니다. 우리가 공부하고자 하는
임베디드 리눅스는 어디까지나 리눅스의 피를 가치고 있기 때문에 범용일 수밖에
없습니다. 하지만 이제 리눅스를 이용해서도 임베디드 시스템에서 충분히 그 가치
를 발휘할 제품, 목적 , 기능이 점점 늘어나고 있습니다．
鞋 m1     역자의 글




       역자는 최근의 구글 이전에는 리눅스만큼 사랑 받는 소프트웨어 , 어쩌면 절대적이라고 할 정
       도의 지지를 받는 소프트웨어나 철학을 만나 본 적이 없습니다. 주변의 수많은 사람들이 리
       눅스를 배우고, 리눅스를 통해서 소프트웨어를 개발하고 있는 것을 볼 수 있습니다. 리눅스
       는 수많은 사람들의 사랑을 받고 있으며 , 역자 역시 리눅스를 무척 좋아하고 그 간결함과 무
       한한 가능성을 사랑하고 있습니다．

       이 책은 리눅스 커널이나 일반적인 프로그래밍을 다루는 기존의 책과는 차별화된 장점을 갖
       고 있습니다. 면저 리눅스 커널에 대한 다른 관점 , 즉 임베디드 개발자의 관점에서 분석하고
       있습니다. 또 다앙한 프로세서와 아키텍처를 예제로 이용하고 있어서 그 내용이 상당히 다양
       하면서도 포괄적입니다. 그리고 커널이 초기화되는 과정을 심도 있게 설명하고 있으며 , 임베
       디드 개발에 있어서 자신의 요구에 맞도록 시스템을 어떻게 변경할 수 있을까2 하는 등의
       실제적인 주제를 다루고 있키 때문에 자신의 업무에 바로 적용할 만한 도움이 되는 내용을
       배울 수 있을 것입니다.

       이 책에 대한 전반적인 소개는 서문에서 충분히 자세하게 설명하고 있습니다. 다만 이 책을
       번역하면서 주석 및 용어 해석과 관련하여 정해 놓은 규칙이 있으니 주의깊게 살펴보기 바랍
       니다. 이 내용을 주지하고 책을 읽으면 좀 더 도움이 될 것 같습니다. 또한 이 책의 부록 A에
       있는 GNU 공중 허가서에 대한 번역문은 송창훈님의 번역을 그대로 이용한 것임을 알려드립
       니다．

       마치막으로 이 책을 번역할 수 있도록 허락해 주시고 인내를 갖고 기다려 주신 정보문화사
       전문서 기획팀에 감사의 말씀을 전합니다. 그리고 번역을 위한 시간을 허락해 준 아내에게도
       무한한 감사를 드립니다．


주석
       먼저 이 책 전반에 예제로 나오는 코드들에 포함되는 주석을 모두 번역해야 할지 고민했습니
       다. 리눅스 코드에 포함되는 코드들은 번역하지 않은 채로 실었습니다. 필자가 직접 작성한
       코드의 경우에는 번역을 하였으며 , 이런 규칙은 리눅스가 출력하는 메시지에도 마찬가치로
       적용됩니다．




昇2
                                              역자의 글




용어 해석
   사실 용어에 대한 해석은 가장 난해한 문제이고, 정해진 답은 없을 것입니다. 이 책에서는
   번역이 불필요한 용어 , 예를 들어 블록 다이어그램化lock diagram)과 같은 용어는 원어를
   그대로 사용했습니다. 실제로 이 용어가 가장 많이 사용되기 때문입니다. 그리고 sleep
   m이扼의 경우는 '휴지 상태' , '슬립 모드' 등의 용어가 개발자들 사이에서 혼용되고 있는 것이
   사실입니다. 그러한 경우는 실제로 좀 더 일반적인 쪽을 우선으로 삼았습니다. 컴퓨터 기술
   에 있어서는 영어권 사람들이 최신 기술을 선도하고 있는 것이 사실이기 때문에 대부분의 용
   어가 영어로 돼 있고, 용어들의 번역이 난해한 경우가 많았습니다. 그래서 독자들의 이해를
   좀 더 돕기 위해 대역표를 실었습니다. 용어가 난해할 때 참고하면 좋을 것 같습니다．

                                       강덕진（from비2k@gmail.com)




                                                          3
        용어대역표                         17
        서문                            29
        시작하면서                         31
        감사의 글                         38
        저자 소개                         40




Chapter ]          소개
        1 .1       왜 리눅스인7口           42
        1.2        임베디드 리눅스의 현재       43
        1.3        오픈 소스와 GPL         43
               1.3. ] 무료와 자유          45
        1.4        표준 및 관련 조직         45
            1.4. ] 리눅스 기본 규격          45
            1.4.2 오픈 소스 개발 연구소        46
        1.5        요약                 48
            1.5.1 더 읽어 보기             48



Chapter 2          임베디드 처음 경험하;71

        2.1       임베디드와 임베디드가 아닌 것7   50
            2.1.] 텨Os와 부트로더           51
        2.2       임베디드 시스템 해부         52
            2.2.1 전형적인 임베디드 리눅스 환경    53
            2.2.2 타깃 보드 구동하기          55
                                            차례   I


            2.2.3 커널 부팅하기                         56
            22.4 커널 초기화 : 요약                      58
            2.2.5 첫 번짜1 사용자 영역 프로세스   in仕         59
        2.3      저장 장치                            60
            2.3.1 플래시 메모리                         60
            2.3.2 NAND 플래시                        63
            2.3.3 플래시의 사용                         64
            2.3.4 플래시 파일 시스템                      65
            2.3.5 메모리 공간                          66
            2.3.6 실행 컨텍스트                         68
            2.3.7 프로세스 가상 메모리                     70
            2.3.8 교차개발 환경                         72
        24       임베디드 리눅스 배포판                     74
            241 상용 리눅스 배포판                        76
            2.4.2 직접 만드는 리눅스 배포판                  76
        2.5      요약                               77
            2.5.1 더 읽어 보기                         78




Chapter 3        프로세서 기본

        3.1      독립형 프로세서                         80
            3 ] ] IBM 97아次                        81
            3.1.2 인텔 펜티엄 M                        81
            3工3 프리스케일 MPC7448                    82
            3.1.4 보조 칩셋                          83
        3.2      통합형 프로세서 : 시스템 온 칩               86
            3 2 1 PowerPC                        86
            3 2 2 AMCC PowerPC                   87
            3.2.3 프리스케일 Powerf그（二                90
            324 MIPS                             95
            3.2.5 브로드컴 卜川PS                      96
            326 AMD MIPS                         98
            3.2.7 기타 入川PS                        99
            3 2 8 ARM                            100
            329 기 ARM                            100
차례



             3.2.10 프리스케일 ARM           102
             3.2.11 인텔 A日M 엑스스케일        103
             3.2.12 기타 A日M              104
             3.2.13 기타 아키텍처             ]04
        3.3          하드웨어 플랫폼           105
             3.3.1 CompactPCl           105
             332 ATCA                   105
        3.4          요약                 ]07
             3.4. ] 더 읽어 보기             107




 Chapter 4           다른 관점에서 본 리눅스 커널
         4. ]       배경                  ]10
             4.1.1 커널 버전                111
             4.1.2 커널 소스 저장소            ]14
         4.2         리눅스 커널의 구성         115
             421 최상위 소스 디렉터리            115
             4.2.2 커널 컴파일하기             ］祀
             4.2.3 커널 단일파일 : vmlinux    119
             4.2.4 커널 이미지 구성 요소         120
                4.2.5 하위 디렉터리 구성        124
         4.3         커널 빌드 시스템          ]25
                4.3. ] 잠Config 파일       125
             4.3.2 구성 편집기               127
             4.3.3 Makef卄e 타깃           131
             4.3.4 커널 구성                135
                4.3.5 구성 옵션 직접 만들기      137
                4.3.6 커널 Makeflle       141
                4.3.7 커널 문서화            142
         4.4         리눅스 커널 구하기         ]43
                4.4.] 추가적으로 더 필요한 것은    ]43
         4.5         요약                 ]44
                4.5.] 더 읽어 보기           ]45
                                                   차례




Chapter 5        커널 초기화
        5. ]     복합적인 커널 이미지 : 이ggy와 그 외 오브젝트 파일        148
            51.1 Image 9너젝트                             ]51
            5.1.2 아키텍처 오브젝트                             152
            5.1.3 부트스트랩 로더                              153
            5.1.4 부트 메시지                                ]55
        5.2      초기화 단계의 제어 흐름                          ]58
            5.2.1 커널 진입점 : head.o                       160
            5.2.2 커널 스타트업 : main.c                      162
            5.2.3 아키텍처 셋업                               163
        5.3      커널 커맨드 라인 처리하7i                        164
            531 1 S아up 매크로                              ]66
        5.4      서브시스템 초기화                              ]72
            5.4.1 * initCall 매크로                        ]73
        5.5      in仕 쓰레드                                ]75
            5.5.1 initc訓을 이용한 초기화                       177
            5.5.2 마지막 부팅 단계                             178
        5.6      요약                                     180
            5.6. ] 더 읽어 보기                              181




Chapter 6        시스템 초기화

        6.1      루트 파일 시스템                              184
            6.1.1 FHS : 파일 시스템 계층 표준                    ]85
            6.1.2 파일 시스템 배치                             ]85
            6.1.3 최소 파일 시스템                             ]87
            6.1.4 루트 파일 시스템의 도전 과제                      189
            6.1.5 시행착오를 반복하는 방법                         ]90
            61.6 자동화된 파일 시스템 제작 툴                       ]90
        6.2      커널의 마지막 부팅 단계                          190
            6.2.] 최초 사용자 영역 프로그램                        ]92
            6.2.2 의존성 해결                                ]93
            6.2.3 초기화 과정 수정하71                          194




                                                        7   I
차례



        6.3         In什 프로세스                194
              6.31 inittab                 197
              6.3.2 웹 서버 시작 스크립트의 0카       ]99
        6.4        초기 램디스크                 201
              6.4.] 초기 램디스크의 용도            202
              6.4.2 initrd로 부팅하기           202
              6.4.3 ir기trd를 지원하는 부트로더      204
              6.4.4 in河d의 마법 : Iinuxrc     205
              6.4.5 initrd 구성              207
              6.4.6 initrd 이미지 민들기         208
        6.5        in出amfs 사용하기            209
        6.6        종료                      210
        6.7        요약                      211
              6.7.1 더 읽어 보기                212




Chapter 7          부트로더
        7.]        부트로더의 역할                214
        7.2        부트로더의 도전 과제             2化
             7.2.1 DRAM 컨트롤러               2化
            7.2.2 플래시와 日AM                 2化
            7.2.3 이미지 복잡도                  217
            7.2.4 실행 컨텍스트                  220
       7.3         유니버설 부트로더 : Das 나Boot   221
            7.3.1 시스템 구성 : 나Boot           221
            乙3.2 나Boot 명령에 셋               224
            7.3.3 네트워크 동작                  225
            7.3.4 저장 장치 서브시스템              228
            7.3.5 디스크로부터 부팅하기              229
       7.4        냐Boot 포팅하기               229
            7.4.1 EP405를 위한 나Boot 포팅       230
            7.4.2 냐Boot mak예le의 구성 타깃      232
            7.4.3 EP405 프로세서 초기화           233
                                        차례



            7.4.4 보드에 따른 초기화                 236
            7.4.5 포팅 요약                      240
            7.4.6 냐Boot 이미지 형식               241
       7.5       기타 부트로더                     243
            751 Lilo                         243
            75'2 GRUB                        244
            7.5.3 더 많은 부트로더                  246
       7.6        요약                         247
            7.6.1 더 읽어 보기                    248




Chapter 8         디바이스 드라이버 기초

        8.1       디바이스 드라이버의 개념              252
            8.1.] 로드 가능한 모듈                  253
            8.1.2 디바이스 드라이버 아키텍처             254
            8.1.3 최소 디바이스 드라이버 예제            254
            8.1.4 모튤 빌드를 위한 기반               255
            81.5 디바이스 드라이버 설치하기              260
            8.1.6 모듈 로드하기                    261
        8.2       모듈 유틸리티                    262
            8 2 1 insmod                     262
             8.2.2 모듈 파라미터                   262
             8.2.3 Ismod                     264
             82.4 modprobe                   265
             8.2.5 depmod                    266
             8 2 6 rmmod                     267
                    dinf。
             8 2'7 m。                        268
        8.3       드라이버의 메서드                  269
             8.3.] 드라이버의 파일 시스템 오퍼레이션        269
              8.3.2 디바이스 노드와 mknod           273
        84        한데 묶71                     274
        8.5       디바이스 드라이버와 GPL             276
        8.6       요약                         277
              8.6.1 더 읽어 보기                  278
     Chapter 9         파일 시스템
             9.1       리눅스 파일 시스템의 개념         280
                   9.1.1 파티션                 281
             92        ext2                   283
                   9.2.1 파일 시스템 마운트하기        284
                   9.2.2 파일 시스템 무결성 검사       286
             9.3       ext3                  288
             9.4       ReiserFS              291
             9.5       JFFS2                 292
             9.6       cramfs                295
             9.7       네트워크 파일 시스템（NFS)      298
                  97.1 NFS를 이용한 루트 파일 시스템    300
             9.8       의사 파일 시스템             303
                  9.8.1 다oc 파일 시스템           303
                  9.8.2 sys佰                 307
             9.9       기타 파일 시스템             310
             9.10      간단한 파일 시스템 만들기        311
             9.1]      요약                    3侶
                 911.] 더 읽어 보기               314




     Chapter 10        MTD 서브시스템

             10.1      MTD 서비스 활성화하기         3化
                 10.1.1 MTD 만들기              320
             10.2      MID 기초                321
                 10.2.1 MTD 구성하71            324
            10.3       MTD 파티션               324
               10.3.1 Redboot 파티션 테이블 나누기    325
               10.3.2 커널 커맨드 라인에서 파티션 생성하기   330
               10.3.3 매핑 드라이버                331
               10.3.4 플래시 칩 드라이버             334
               10.3.5 보드에 따른 초기화             335




10
                                                     차례



        10.4     MTD 유틸리티                                 336
             10.4.1 JFFS2 루트 파일 시스템                       340
        10,5     요약                                       342
             10.5.1 더 읽어 보기                               343




Chapter 11        BusyBox

        11.1      BusyBox 소개                              346
             11.1.1 BusyBox는 쉽다                           347
        11.2      BusyBox 구성하기                            347
             11.2.1 BusyBox 교차큄파일하기                       349
        11.3      BusyBox의 기능                             350
             卄3.1 BusyBox In仕                             353
             11.3.2 rcS 초기화 스크립트 예제                       356
             11.3.3 BusyBox를 타깃 보드에 설치하기                  357
             11.3.4 BusyBox 명령에                           359
        11.4      요약                                      361
             11.4.1 더 읽어 보기                               361




Chapter 12         임베디드 개발 환경
        121        교차개발 환경                                364
             121 1 임베디드 "He化 World''                      365
        12.2       호스트 시스템 요구 사향                          369
             122.1 하드웨어 디버깅 장비                            370
        12.3       타깃 보드 호스팅하기                            370
             12.3.1 TFTP 서버                               371
             12.3.2 日OOTP/DHCP 서버                         372
             12.3.3 NFS 서버                                375
             12.3.4 타깃 시스템에 NFS 루트 파일 시스템 마운트하기           377
             12.3.5 나Bo아를 이용한 NFS 루트 파일 시스템 마운트 예제        379
        12.4       요약                                     381
             12.4.] 더 읽어 보기                               382




                                                          U1
     차례



      Chapter 13         개발 도구

              13.1       GNU 디버거（GDB)                   384
                  13.1. ] 코어 덤프 디버그하71                  385
                  13.1.2 GDB 실행하기                       387
                  13工3 GDB의 디버그 세션                      390
              13.2       데이터 표시 디버71                    392
              13.3       야)rowserlcsc야冶                 395
              13.4       추적 및 프로파일링 도구                  396
                  13.4.1 strace                   " "   397
                  伶4.2 計ace의 다양한 기능                     401
                  134.3 Itrace                          404
                  13.4.4 Ps                             405
                  13.4.5 幻口                             408
                  13.4.6 mtrace                         4化
                  13.4.7 dm訓oc                          412
                  13.4.8 커널 웁스(O叩s)                     416
             13.5        바이너리 유틸리티                      419
                  13 5 1 readelf                        419
                  13.5.2 read터f를 이용해서 디버깅 정보 보기         421
                  13.5.3 objdump                        424
                13.5.4 objcopy                          425
             13.6       기타 바이너리 유틸리티                    426
                13.6.1 s뺘）                              426
                13.6.2 addr2line                        426
                13.6.3 strings                          427
                136.4 Idd                               427
                13.6.5 nm                               428
                13.6.6 prelink                          429
             13.7       요약                              430
                13.7. ] 더 읽어 보기                         430




     Chapter 14         커널 디버깅 기술
             14.1       커널 디버깅의 어려움                     434
             14.2       KGDB를 이용한 커널 디버깅                435


12
                                            차례   難及



           14.2.1 KGDB 커널 구성                     437
           14.2.2 KGDB를 활성화시킨 타깃 부팅하기            438
           14.2.3 유용한 커널 브레이크 포인트                441
        14.3     리눅스 커널 디버깅하기 .                  442
           14.3.1 gdb 원격 시리얼 프로토콜                444
           14.3.2 최적화된 커널 코드 디버깅하기               447
           14요3 gdb 사용자 정의 명령에                   454
           14.3.4 유용한 커널 gdb 매크로                 455
           14.3.5 적재 가능 모듈 디버깅하기                 465
           14.3.6 printk 디버깅                     470
           14.3.7 매직 Sys딕eq 키 1                  471
        14.4     하드웨어를 이용한 디버깅                   473
           14.4.1 JJAG 프로브를 이용해서 플래시 기록하기        475
           14.4.2 JTAG 프로브를 이용한 디버깅              476
        14.5     부팅이 되지 않을 때                     481
           14.5. ] 초기 시리얼 디버그 출력                 481
           14.5.2 川ntk 로그 버퍼의 내용 덤프하71           483
           14.5.3 커널 패닉에서 KGDB 사용하7j             485
        14.6     요약                              486
           14.6. ] 더 읽어 보기                       487




Chapter 15       임베디드 리눅스 어플리케이션 디버깅하기

        15. ]    타깃 디버깅                          490
        15.2     원격 （교차） 디버깅                     490
           15.2.1 gdbserver                      493
        15.3     공유 라이브러리 디버깅                    496
           15.3.1 GDB의 공유 라이브러리 이벤트              498
        15.4     여러 태스크 디버깅하기                    502
           15.4.1 다중 프로세스 디버깅                    502
           15.4.2 다중 쓰레드 어플리케이션 디버깅              505
           15.4.3 부트로더 및 플래시에 있는 코드 디버깅          509
        15.5     추7F 원격 디버그 옵션                   5化
           15.5.] 시리얼 포트로 디버깅하기                  510
           15.5.2 실행중인 프로세스에 연결하71               5化



                                                 '3 I
     차례



              15.6    요약                  511
                  15.6.1 더 읽어 보기         512




     Chapter 16       리눅스 포팅
             16.]     리눅스 소스 코드의 구조      514
                  16.1.] 아키텍처 브렌치        514
             16.2     자체 보드를 위한 리눅스      517
                  162. ] 선행 조긴과 가정       517
                  16.2.2 커널 초기화 커스터마이징   519
                  16.2.3 정적인 커널 커맨드 라인   522
             16.3     플랫폼 초기화            524
                  也3.1 초기 변수 접근          528
                  16.3.2 보드의 정보 구조       530
                  16.3.3 머신 종속적인 호출      532
             16.4     핸카 묶기              534
                  164.1 기타 아키텍처          537
             16.5     요약                 537
                16.5.1 더 읽어 보기           538




     Chapter 17       리눅스와 리얼 타임
             17. ]    리얼 타임              540
                17.1. ] 소프트 리얼 타임        540
                17.1.2 하드 리얼 타임          541
                17.1.3 리눅스의 스케줄링         541
                17.1.4 지연                541
             17.2     커널 선점              543
                17.2.1 선점의 장애물           544
                17.2.2 선점 모델             545
               17.2.3 SMP 커널             547
               17.2.4 선점 지연의 원인          548




14
                                        차례   發



       17.3   리얼 타임 커널 패치                    548
         17.3.1 리얼 타임 기능                     550
         17.3.2 O(1) 스케줄러                    553
         17.3.3 리얼 타임 프로세스 생성하기              553
         17.3.4 크리티컬 섹션 관리                   555
       17.4   리얼 타임 커널 디버깅하기                 556
         17.4.] 소프트 락업 감지                    556
         17.4.2 선점 디버깅                       557
         17.4.3 깨어나는 시간 디버깅                  557
         17.4.4 깨어냐는 지연 시간 기록                558
         17.4.5 인터럽트 차단 시간                   558
         17.4,6 인터럽트 차단 시간 기록                559
         17.4.7 지연 시간 추적                     561
         17.4.8 데드락 상태 디버깅하71                563
         17.4.9 락 모드 제어하기                    563
       17.5   요약                             564
         17.5.] 더 읽어 보기                      564




Append以 A     GNU 일반 공중 사용 허가서
         전문                                  567
         복제와 개작 및 배포에 관한 조건과 규정              569
         보증의 결여쩌Ill조 저12조）                   574




Append江 B     小Bo야의 구성 가능 명령에 셋 / 577


Appendix C    BusyBox 명령에 / 581


Appendix D    SDRAM 인터페이스 고려 사항
       0.1    SDRAM 기초                       592
         D.1.1 SDRAM 리프레시                    593
       0.2    클럭                             594
       0.3    SDRAM 설정                       596



                                             15 ,g>
      N   차례



                 D.4   요약                        601
                   D.4.1 더 읽어 보기                 601



          Append江 E    오픈 소스 리소스

                   소스 저장소 및 개발자 정보               604
                   메일링 리스트                       604
                   리눅스 뉴스 및 개발 정보                605
                   오픈 소스에 대한 이해 및 토론             605


          Appendix F   예제 BDI-2000 구성 파일 / 607


          찾아보71 / 6佰




116
위치   용어                          번역
서문   convention                  명명 규칙
     아oprieta口 0口erating sys也m   자체 운영체제
     fi이d app妃ation en寸neer      필드 어플리케아션 엔지니어
     comF兀S陀 kern이 image         복합 커널 이미지
     loca卜針ea network            LAN, 로컬 네트워크
     da怡 sheet                   데이터 시트
     m吠枷0（氾ss                    멀티프로세스
］장   licensee                    라이선스 소유자
     roya啣                       로열티
     lab                         랩
2장   erase block       1스｝       ；텍 단위 翡
     sen계 port                   시리얼 포트
     bina口                       바이너리
     flash mem아y                 플래시 메모리
     boot loader                 부트로더
     memo四 cell                  메모리 셀
     m吐야rocessor                 마0日로프로체朴
     instruction cache           명령에 캐시
     algor甘hm                    알고리즘
     wear - leveling             웨어 레벨링
     용어대역표



위치   용어                              번역
     em내ate                          0幄레이트
     MTD(Memory techn이ogy de너ce)     메모리 기술 저장 장치
     address space                   주소 공간
     address line                    주소 라인
     task                            태스크
     memory management un什 / MMU     메모리 관리 장치
     execution context               실행 컨텍스트
     defau仕                          디폴트
     可chitecture                     0톄텍처
     ns甘uction 口이nter                명령에 주소
     wait queue                      대기 큐
     command prompt                  명령（어） 프롬프트
     이ob톄 variab旭                    전역 변수
     b c톄 variab冶                    지역 변수

     swap                            스왑
     application                     응용 프로그램
     Cross-Dev이이）ment Environment    교차개발 환경
     too卜chain                       툴 체인
     include                         포함
     아oss-compiler                   교차 컴파일러
     native compile                  자쳬 컴파일
     clock                           클럭
3장   main memory                     메인 메모리
     low-latency                     낮은 지연성
     引eep mode                       슬립 모드
     아ogrammable interrupt contr이놔   프로그램 가능한 인터럽트 컨트롤러
     para回 port                      패러럴 포트



18
                                                            용어대역표




우因   용어                                  번역
     on-chip                             칩에 내징틘
     block 뎨agram                        블록 다이어그램

     f口U                                 부동 소수점 연산장치
     low end                             저7땡
     high end                            고급형
     SMC : Sen졔 Management Contr이er      시리얼 매니지먼트 컨트롤러
     SCO : Sen톄 （丸mmunication Contr에er   사리얼 통신 컨트롤러
     full du이ex                          양방향
     mi.此chann이                          다채널
     license                             라이선스

     single core                         단일 코어
     du졔 core                            듀얼 코어

     quad core                           쿼드 코어

     on board                            온 보드

     security engine                     보안 모듈 엔진

     application 아ocessor                어플리케이션 프로세서

     encryption                          암호화
     decryption                          복호화

     packet 徹帥ng                         패킷 필터링
     network 아ocessing engine            네트워크 처리 엔진
     vertic졔 market                      수직사장
     san (storage area network)          광 저장장치 영역 네트워크
     Bacl4켜ane                           후면
     P10MG                               P（긔 산업 컴퓨터 생산 그룹
     sys旭m on ch巾                        시스템 온 칩 / SOC

4장   fa미tt이erant                         폴트 톨러런트
     source tree                         소스 트己1



                                                                    19
     月    용어대역표



위치        용어                     번역
          repo訊ones              저장소
          mainline kernel        기준 커널
         的t-con匈                 젬C아州g
          Kern이 symb이            커널 심볼
          target                 타깃 / 대상
         kernel proper           커널 단일 파일 / 커널 자체 / 커널 본체
         unres이ved (symb이,·．·）   주소 값이 해결되지 않은 / 주소 값이 결정되지 않은
         object file             오브젝트 파일
         context sw配h            문맥전환 / 컨텍스트 전환
         reference board         참조용 보드 / 참고용 보드
         loadable mod미e          적재 가능 모듈
         incremental link        증분 링크
         command line            명령（어） 라인
         front end               프론트 엔드
         defau仕                  기본 값
         de너ce                   장치 / 디바기스
5장       low level               저수준 / 로우 레벨
         sta八up code             스타트업 코드
         big endian              빅 엔디안
         page table              페이지 테이블
         re졔 mode                리얼 모드
         memo싸 tran引ation        메모리 변환
         virtu톄 addres싫ng        가상 어드레싱
         address pin             어드레스 핀
         revision                리비전
         baud rate               보 래잇 / 변조 속도
         mount                   口區트



20
                                               용어대역표   發藝




위치   용어                       번역
     hard coded               하드 코드
     command line parameter   커맨드 라인 파랴미터
     mechanism                메커니즘
     \ , line continuation    행 계속문자
     야川mize                   최적화
     parsing                  파싱
     flag                     플래그
     ea由 parsing 졔gorithm     초기 파싱 알고리즘
     hook                     후킹, 훅
     process id               프로세스 ID
     idle process             유휴 프로세스
     null                     널
     user space               사용자 영역 / 유저 영역
6장   initi졔 ramd姚             초기 램디스크
     root                     루트
     to이k比                    툴킷
     so州ink                   소프트 링크

     package                  패키지
     미St巾베on                  제공 / 배포판
     wrap口er                  랩퍼
     run 1ev이                 동작 레벨
     multi user               멀티유저
     symbolic link            심볼릭 링크
     man page                 맨 페이지
     configuration u눼作y       구성 유틸리티
     compa아디ash               콤팩트 플래시
     delay                    지연시간



                                                        21
     용어대역표




위치   용어                            번역

     cus加mizing                    커스터마이징
     File system 네eran巾y 앉andard   파일 시스템 계층 표준

     벼S嫌兀的n en미neering             배포를 위한 기술
     kern이 command line            커널 커맨드 라인

7장   0日AM                          동적 임의 접근 메모리

     run긔me libra四                 런 타임 라이브러리

     拉nker descri國on 律e            링캬 기술 파일
     univers톄 bo에oader             유니버설 부트로더

     commun啣                       공동체 / 커뮤니티
     command s아                    명령에 셋 / 명령에 집합

     DHCP                          동적 호스트 제어 프로토콜

     Tn-P                          간이 파일 전송 프로토콜

     target device                 대상 디바이스
     broadcast packet              쁘드캐人드 패킷

     mapping
     user manu졔                    사용자 매뉴얼， 유저 매뉴얼

     h이d time                      홀드 시간
     prefetch                      프리페치
     Ser洌 Presence Detect          직렬 방식의 존재유무 감지
     dua卜boot                      다중 부트

     tree software 幻undat口n        프리 소프트웨어 재단

8장   public license                공공 라이선스
     character deivce              캐릭터 디바이스
     block device                  블록 디바이스

     unload
     method                        메서드 / 함수
     operation                     오퍼레이션



22
                                                   용어대역표




위치    용어                            번역
      ma柯 number                    주 버전
      file descriptor               파일 기술자
      bring it all 幻gether          한데 묶기
      derived worl(                 수정판

9장    口seu（把 file system            의사 파일 시스템
      magnetic tape drive           자기 테이프 드라이브
      partition                     파티션
      V이ume label                   볼륨 라벨
      mount p이nt                    마운트 지점

      corrupt                       깨진
      針）utdown                      셧C윤 / 종료
      metada怡                       메타데이터
      read on如                      읽기 전용
      b c졔 （批ecto싸                  로컬 디렉터리
      symbolic name                 심볼릭 이름
      gateway                       게이트웨이
      subnet                        서브넷
      netmask                       넷마스크

      virtual memo싸 segment         가상 메모리 서［그먼트
      shared 比ra四                   공유 라이브러리
      loopback                      루프백
10장   sna口帥아                        스냅 샷
      디S (flash image system)       퓰래시 이미지 사스템
      C디 (common flash interface)   공용 플래시 인터페이스
      mapping dnver                 매핑 드라이버
      pesudo                        슈도 / 의사
      m미tic섧1                       다중 호출



                                                           23
         용어대역표




  위치     용어                    번역
         prefix                잔지시자
  ]］장    core u눼ity            코어 유틸리티
         b c톄 boopback         로컬 루프백
         S（그cket               소켓
         su口아sen／아             슈퍼서버
         a口口et                 애플릿
        bash shell             배시 쉘
        아아아ype                 프로토타입
        pos以                   포직스
 12장    恂htw텨ght 아아oc이         경량 프로토콜
        private network(       사설 망
        kern이 level            커널 레벨
        cons이e                 콘솔
 13장    crash dum口             크래시 덤프
        아oss debugger          교차 디버거
        segmen怡的nfa미t          세그먼테이션 오류
        debugging symb이        디버깅 심볼
        stack frame            스택 프레임
        debug ses듸on           디버그 세션
        뱌eak口이nt               브레이크 포인트
        return                 반환
        data 미S口ay debugger    데이터 표시 디버거
        pro帥ng                 프로파일링
        capture                캡처
        dynamic linker니oader   동적 링커．로더
        S吟tem call             시스템 콜
        endpoint               종단점 / 엔드 포인트



I 24
                                                  용어대역표




위치    용어                             번역
      DNS(dom帥 name service)         도메인 네임 서비스
      parameter                      파라미터
      dash                           대시, -
      foreground 아ocess              전위 프로세스
      linked list                    연결 리스트
      resident memory                상주 메모리
      memory leak                    메모리 누수
      race condition                 경쟁 조건
      timin(}                        타이밍
      QA (quality assurance)         QA
      core 伽mp                       코어 덤프
14장   kern이 oops                     커널 웁스
      kernel panic                   커널 패닉
      stack 口이nter                   스택 포인터
      세P (next ins打uction p이nter)    다음 명령에 포인터
      disassemble                    역 어셈블
      T1S (tool interlace 없andard)   툴 인터페이스 표준
      ICE (In-circu仕 em미ator)        서킷 에뮬레이터

      口peline                        파이프라인
      overhead                       오버헤드

      data type                      데이터 타입
      hook                           후크

      trap                           트랩
      ev톄uation kit                  평7용 보드

      program counter                프로그램 카운터
      inline assembler               인라인 어셈블러
      interwpt dnven                 인터럽트 드쾨븐
       용어대역표




위치     용어                                  번역
       remo把 senal pr아ocol                 원격 사리얼 프로토콜
       user-specified 뱌ea印帥t               사용자 지정 브레이크 포인트
       function mnImring                   함수를 인라인으로 처리弓는 기술
       mnemonic                            니모닉
      m im ing                             인라인 처리
      user-defined command                 사용자 정의 명령어
      initi刮 task                          초기 태스크
      circular linked list                 원형 연결 리스트
      symb이 table                          심볼 테이블
      loglev터                              로그 레벨
      daemon                               데몬
      뱌eak character                       브레이크 문자
      JTAG probe                           JTAG 프로브
      bounda四 scan to이                     바완似 스캔 툴
      없ack backtrace                       스택 역추적
      stop reply                           정지 응답
      5山b                                  스텁
15장   아aph匕 뎨splay                         그래픽 표시 장치
      thread                               쓰레드
      Mu川threaded                          다중 쓰레드
      NPTL (Native Posix Thread Library)   자체 Pos以 쓰레드 라이브러리
      엷eep                                 휴지
      current thread                       현재 쓰레드
16장   NIC                                  네트워크 인터페이스 컨트롤러
      is이欲ion                              분리
      chip s이ect                           칩 선택
      bo아strap                             부트스트랩



26
                                               용어대역표




위치    용어                         번역

      general purpose register   범용 레지스터
      r터ocatab冶                  재배치 가능
      Pu川ng It All Together      흔Ii카 묶기

      引ab 訓oca幻r                 슬랩 할당자
      可야出ec加re 뱌an아）             0끼텍처 브랜치

17장   re졔 time                   리얼 타임 / 실시간
      so什 rea地me                 소프트 리얼 타임

      hard realtime              하드 리얼 타임

      tick                       틱

      scheduling                 스케줄링
      ISR                        인터럽트 서비스 루틴

      nterrupt off time          인터럽트 차단 시간

      critical sec的n             크리티컬 섹션

      concurrency                동시성
      斗洌ock                      스핀락

      lock / locking             락 / 보호

      So化RQ                      소프트 IF크a

      har(井K그                    하드 IF국a

      thr아iding                  쓰레딩

      아eempt                     선점
      soft lockup
      deadlock                   데드락

      wakeup timing              깨어나는 시간
      redirect                   리 다이렉트

부록    free so仕ware               프리 쑈프트웨어

      work based on the 다0아am    프로그램 수정판

      warranty



                                                       27
     용어대역표



위치   용어                        번역
     modified wo水              수정판
     address bus               주소 버스
     row address line          줄 주소 신호선
     C이umn address line        행 주소 신호선
     refresh                   리프레시
     cell                      셀
     burst read                버스트 읽기
     tran듸stor                 트랜지스터
     capacitor                 커패시터
     synchronous               동기식
     n이ng edge                 상승 어찌
     falling edge              하강 에지
     F개 (phased locked loop)   위상 동71 루프
     아echarge                  프리차지
     named pipe                명명된 파이프
     ro（川ng table              라우팅 테이블
     w欲ch-dog                  와치독
     計ec加e-user l[)            실효 사용자 ID




28
컴퓨터는 우리 주변 어디에나 있습니다．

이는 최근 25년간을 동굴 속에서 산 사람이 아니라면 그리 크게 놀랄 사실은 아닐
것입니다. 그리고 이 글을 읽는 독자도 아마 컴퓨터하면 단순히 데스크탑 컴퓨터만
을 이야기하는 것이 아니라, 우리의 주방은 물론이고 좋아하는 음반을 잔뜩 모아 놓
은 거실에도 컴퓨터는 존재한다는 것을 알고 있을 것입니다. 전자레인지 , 전자 오븐
은 물론이고 우리가 흔히 사용하는 휴대폰에서 휴대용 MP3 플레이어까지 모두가
컴퓨터입니다．

그리고 이 책을 들고 있는 독자라면 아마도 임베디드 시스템에 대해서 뭔가 흥미로
운 내용들을 배우고 싶은 마음을 갖고 있을 것입니다．

비교적 최근까지도 임베디드 시스템은 그리 강력하지 않았고, 특수한 목적으로만
사용되거나, 산업 표준과는 상당히 다른 자체 운영체제를 사용하는 경우가 많았습
니다（또한 개발하는 일도 너무 어려웠습니다）. 하지만 지금은 임베디드 시스템이
최신 가정용 컴퓨터보다 빠르지는 않더라도 비슷한 정도의 컴퓨팅 파워를 갖는 경우
가 많습니다（예로, 하이 앤드 게임기를 생각해 볼 수 있습니다）.

이런 컴퓨팅 파워로 인해서 임베디드 시스템에서도 리눅스와 같은 완전한 운영체제
를 실행시킬 수 있게 되었습니다. 임베디드 제품에 리눅스와 같은 운영체제를 이용
하는 것은, 리눅스가 매우 큰 규모의 개발자 커뮤니티를 갖고 있기 때문에 상당히
괜찮은 선택이라고 할 수 있습니다. 또한 개발 환경과 배포 환경이 놀라울 정도로
비슷하기 때문에 개발자가 좀 더 쉽게 작업을 진행할 수 있습니다．
         서문




       그리고 가상 메모리에 기반한 시스템을 사용하기 때문에 보안성을 확보할 수 있으며 , 멀티유
       저나 멀티프로세스 시스템의 강력함과 유연성을 모두 활용할 수 있습니다. 즉, 상당히 괜찮
       은 선택이라고 말할 수 있습니다．

       이런 이유 때문에 천 세계의 많은 회사들이 여러 제품에 리눅스를 이용하고 있는데 , 여기에
       는 PDA, 가정용 엔터테인먼트 시스템은 물론이고 놀랍게도 핸드폰도 있습니다！

       무엇보다도 이 책은 아주 재미있는 책입니다. 자신의 임베디드 시스템에 리눅스를 사용하고
       싶어 하는 개발자를 위해서 아주 좋은 개발 지침들을 배울 수 있끼 때문입니다. 이 책은 명확
       하고, 아주 잘 쓰였고, 구성이 아주 탄탄합니다. 이 책 어디서나 이 책의 저자인 크리스가
       갖고 있는 깊은 지식과 폭넓은 이해를 느낄 수 있을 것입니다. 단순히 관련 정보와 도움말만
       을 제공하는 것이 아니라, 아주 재미있게 읽을 수 있도록 잘 짜여 있습니다．

       저는 제가 그랬듯이 독자들도 이 책에서 어떤 것을 배우기도 하겠지만, 동시에 즐길 수도 있
       기를 바랍니다．

                                      아놀드 로빈스（'An加／d／初bb加s)
                                                  사라즈 편집장




I 30
리눅스를 다루는 책들 중에는 훌륭한 책들이 아주 많다. 하지만 임베디드 개발자만
을 대상으로 하는 참고 서적은 전무하다시피 하다. 물론 리눅스 커널이나 리눅스 시
스템 관리 등에 대한 훌륭한 저서들도 있다. 그리고 그런 각 분야에 대해서 필자가
생각하는 명저는 이 책 곳곳에서 참고 자료 형태로 확인해 볼 수 있을 것이다．

이 책에 실린 내용의 상당수는 필자가 수년간 몸담고 있는 임베디드 리눅스 배포
버전에 대한 선두 업체인 몬타 비스타 소프트웨어 사에서 필드 어플리케이션 엔지니
어（FAE）와 임베디드 리눅스 컨설턴트로 활동하면서 이 분야의 개발 엔지니어로부
터 받은 질문들에서 나온 것들이다．

경험 많은 소프트웨어 엔지니어라도 임베디드 리눅스로 작업할 때 나름의 몇 가지
특별한 어려움을 겪게 된다. 먼저 자신이 기존에 사용하던 리얼 타임 운영체제
(RTOS）에 대한 경험만을 갖고 있을 것이기 때문에 , 생각을 리눅스 환경으로 전환
하는 데 어려움을 겪는다. 둘째로는 숙련된 개발자도 처음에 교차小개발 환경의 복잡
한 과정을 이해하는 테 상당한 어려움을 겪는다．

이 책은 임베디드 리눅스를 처음 접하는 개발자를 위한 입문서이지만, 임베디드 리
눅스에 대한 경험이 있는 개발자도 필자가 수년간 얻은 기술과 유용한 팁을 공유할
수 있을 것이라고 자신한다．
         시작하면시




 임베디드 개발자를 위한 실용 가이드

       이 책은 필자의 관점에서 임베디드 엔치니어가 급변하는 임베디드 리눅스 개발 환경에서 꼭
       알아야 한다고 생각하는 내용들을 담고 있다. 커널을 다루는 장에서는 리눅스 커널의 내부를
       들여다보는 것은 다른 좋은 책들에 맡기고, 대신에 커널을 프로젝트 관점에서 이해하는 데
       초점을 맞췄다. 그래서 커널의 구조와 커널 소스 트리의 구성에 대해서 배울 것이다. 그리고
       커널 이미지가 어떤 바이너리 구성 요소들로 만들어지는지를 알아보고， 그것들이 어떻게 로
       드되고, 임베디드 시스템에서는 어떤 역할을 하는지 살펴볼 것이다. 필자가 이 책에서 좋아
       하는 그림 중의 하나인 ［그림 5-1］은 복합 커널 이미지가 만들어지는 과정을 설명해 준다．

       이 책의 내용을 통해서 독자는 리눅스 빌드 시스템이 어떻게 동작하는지를 배우고, 자신만의
       프로젝트를 위해서 필요한 수정 사항들을 리눅스 커널에 통합시키는 방법도 알게 될 것이다．
       그리고 리눅스 커널 소스 트리에서 다른 아키텍처와 기능을 설정하기 위해서 구성 파일 설정
       메커니즘을 알아볼 것이다. 더 중요한 부분으로 독자의 필요에 따라서 이 시스템을 수정하는
       방법도 알아본다. 커널 커맨드 라인 메커니즘어］ 대해서도 자세히 설명할 것이다. 자신의 필
       요에 따라서 동작중인 커널을 설정하는 방법을 배워 보고, 이 기능을 자신의 프로젝트로 확
       장하는 방법을 살펴볼 것이다. 커널 소스 코드를 탐색하는 방법을 알아보고, 임베디드 시스
       템에 관련된 작업을 위해서 커널을 어떻게 구성하는지 학습해 볼 것이다. 그 외에도 임베디
       드 프로젝트를 위해서 사용할 수 있을 만한 여러 가지 팁과 테콰4들도 배울 수 있을 것이다.
       여기에는 부트로더 , 시스템 초기화, 파일 시스템 , 플래시 메모리에서부터 고급 커널 디버킹
       및 어플리케이션 디버깅 기술도 포함된다．


대상 독자

       이 책은 C 언어로 프로그램을 작업한 경험이 어느 정도 있는 독자를 대상으로 했다. 그리고
       인터넷과 로컬 네트워크에 대해서 기본적인 지식을 갖고 있을 것이라고 가정했다. 즉, 독자
       는 기본적으로 II) 주소 개념을 이해하고, 이 II> 주소를 간단한 로컬 네트워크에서 어떻게
       사용하는지 이해하고 있어야 한다. 또한 이 책에서 횬히 쓰이는 16진수 표기법이나 8진수
       표기법도 알고 있어야 한다．




I 32
                                                   시작하면서    I.



   C로 컴파일하고 링크하는 과정에 대해서 깊이 있는 내용도 다룰 것이기 때문에 , 일반 C 프로
   그래밍에서 링커의 역할을 이해하고 있는 것이 도움이 될 것이다. 그리고 GNU make가 어
   떻게 동작되고 어떤 의미를 갖는지를 알고 있으면 이 책의 내용을 이해하는 데 큰 도움이
   될 것이다．


이 책이 다루지 않는 부분
   이 책에서는 하드웨어에 대한 자세한 설명은 하지 않을 것이다. 임베디드 개발자가 어려움을
   겪는 이유 중의 하나가 현재 시장에서 사용되는 하드웨어 장치들이 엄청나게 다양하다는 데
   있다. 일부 보조 장치들이 통합되어 있는 최신 32비트 프로세서의 사용자 매뉴얼만 해도 천
   페이지를 쉽게 넘긴다. 하지만 별다른 지름길은 없다. 즉, 프로그래머의 관점에서 하드웨어
   장치를 이해하기 위해서는, 충분한 시간을 들여서 하드웨어 데이터 시트와 참고 가이드를
   읽고 이를 토대로 각각의 장치를 테스트하는 코드를 작성하고 연습하는 과정이 반드시 필요
   하다！

   또한 이 책은 리눅스 커널이나 커널 내부를 설명하기 위한 책도 아니다. 이 책에서는 리눅스
    의 가상 메모리 관리 정책을 위해서 필요한 메모리 콴리 장치（MMU）가 내부적으로 어떻게
   동작하는치는 설명하치 않을 것이다. 이 내용들에 대해서는 다른 훌륭한 책들이 이미 나와
   있다. 각 장의 마지막에 있는 "더 읽어 보기"에 나오는 참고 서적들을 통해서 해당 분야의 더
   깊은 내용을 살펴보면 좋을 것이다．


명명 규칙
    경로를 표시할 때 앞에 점 서］ 개가 있을 때는 따로 명시하지 않는한 작업하는 최상위 디렉터
   리를 의미한다. 물론 최상위 디렉터리는 본문의 내용에 따라서 달라질 수 있지만, 대부분은
   리눅스 커널 소스의 최상위 디렉터리를 가리킨다. 예를 들어 , . . . /arch/ppc/kernel/
    se七up. c는 리눅스 소스 트리에서 아키텍처 하위 디렉터리에 있는 setup. c라는 파일을 가
    리킨다. 그래서 아마 실제 경로는 N /sandbox/1inux .2.6.14 /arch/ppc/kernel/
    se七up. c와 같을 것이다．




                                                             331
        시작하면서




0I 책의 구성

       1장, "소:7卄"에서는 임베디드 환경에서 리눅스가 급속도로 이용되는 몇 가치 이유에 대해서 살
       펴본다. 그리고 임베디드 리눅스와 관련된 중요한 표준 및 단체에 대해서도 소캐할 것이다．

       2장, "임베디드 처음 경험하71"에서는 이어지는 장들을 통해서 하나씩 배우케 될 여러 임베디드
       리눅스 관련 개념들을 소개할 것이다．

       3장, "프로세서 기본"에서는 임베디드 리눅스 시스템을 개발할 때 많이 사용되는 인기 있는 프
       로세서와 플랫폼에 대해서 설명한다. 그리고 많은 선두 프로세서 생산 업체의 제품들에 대해
       서도 몇 가지 살펴볼 것이고, 그 중에서도 주요 아키텍처 프로세서 계열들은 모두 알아볼 것
       이다．

       4장, "다른 관점에서 본 리눅스 커널"에서는 제목처럼 약간 다른 관점에서 리눅스 커널을 실험해
       볼 것이다. 즉, 커널에 대한 이론이나 내부 구조를 설명하는 대신에 , 커널의 구조와 배치 그
       리고 빌드가 되는 구조를 알아봄으로써 이런 거대한 소프트웨어가 어떻게 동작하는지를 이해
       할 수 있도록 할 것이다. 또한 더 중요한 부분으로쩌 커널을 자신에게 맞게 수정하기 위해서
       어디에 중점을 두고 진행해야 할치도 배워 보도록 한다. 또한 여기서 커널 빌드 시스템에 대
       해서도 설명할 것이다．

       5장, "커널 초기화"에서는 리눅스 커널의 초기화 과정을 상세히 알아볼 것이다. 그래서 독자는
       특정 아키텍처 또는 부트로더를 위해서 이미지가 어떻게 결합되어 리눅스 커널 본체 이미지
       가 구성되는지를 배울 것이다. 그리고 이 커널 본체 이미지를 플래시에 다운로드해서 내장된
       부트로더를 통해서 부팅되는지를 알아볼 것이다. 여기서 배운 지식을 이용하면 자신이 개발
       하는 임베디드 어플리케이션에 맞게 커널을 수정하는 데 도움이 될 것이다．

       6장, "시스템 초기화'는 5장에 이어서 초기화 과정을 계속 설명한다. 리눅스 커널이 자체적인
       초기화 과정을 모두 마치면 어플리케이션 프로그램이 미리 정의된 방식으로 초기화 과정을
       계속하게 된다. 6장까지의 내용을 통해서 자신의 어플리케이션을 위해 특별한 초기화 과정을
       설정하는 방법도 알게 될 것이다．




I 34
                                            시작하면서   難 小1



7장, "부트로더"는 장 전체가 임베디드 리눅스 시스템의 부트로더와 부트로더의 역할에 대해
서 설명한다. 이 장에서는 유명한 오픈 소스 부트로더인 U-Boot를 설명하고 U-Boot를 실
제로 포팅하는 예제를 다룬다. 그 외에 현재 사용되는 다른 부트로더들을 간락히 소개해서
자신에게 맞는 부트로더를 고르는 데 도움이 되도록 했다．

8장, "디바이스 드라이버 기초"에서는 리눅스 드라이버 모델을 소깨하고, 8장의 "더 읽어 보기"
에 있는 훌륭한 책들을 읽고 이해하기 위한 기본 지식들을 소캐하는 데 중점을 두고 있다．

9장, "파일 시스템"은 현재 임베디드 시스템에서 많이 사용되는 파일 시스템들을 소개한다. 여
기에는 플래시 메모리를 위한 중요한 임베디드 파일 시스템인 JFFS2도 포함된다. 이 장에
서는 임베디드 개발자가 주로 겪게 되는 어려운 문제인 자신만의 파일 시스템 이미지를 만드
는 방법에 대해서 간단히 소깨한다．

10장, "MTD 서브시스템'에서는 메모리 기술 저장 장치（MTD）에 대해서 알아본다. MTD는 리
눅스 파일 시스템과 하드웨어 메모리 장치 , 특히 플래시 메모리 사이의 추상 계층으로서 가
장 유용하게 사용된다．

11장, "BusyBox"에서는 소규모 임베디드 시스템을 만들 때 가장 유용한 유틸리티 중의 하나
인 BusyBox를 설명한다. 자신의 시스템 요구 조건에 맞게 BusyBox를 구성해서 빌드하는
방법과 함께 , BusyBox 환경이 갖는 특수한 시스템 초기화 과정에 대해서도 자세히 설명한
다. 부록 C, "BusyBox 명령에"를 보면 최신 BusyBox에서 사용 가능한 명령어들의 목록 을
볼 수 있다．

12장, "임베디드 개발 환경"에서는 전형적인 교차개발 환경을 갖추기 위해서 특별하게 필요한
사항들을 자세히 알아본다. 여기서는 개발자로서 생산성을 좀 더 높이기 위한 몇 가치 기술
들을 설명할 것이다. 여기에는 강력한 개발 환경인 NFS를 루트 파일 시스템으로 마운트시
켜 사용하는 기술도 포함된다．

13장, "개발 도구"에서는 유용한 여러 개발 도구들을 소개한다. gdb를 이용해서 디버깅하는
방법을 설명하고, 코어 덤프를 분석하는 방법도 알아본다. 그 외에도 S七race, 1七race,
top, ps 그리고 메모리를 프로파일링할 수 있는 툴인 m七race와 dmalloc 등의 많은 개발
툴들을 설명한다. 그리고 마지막으로 readeif를 포함한 중요 바이니리 유틸리티들을 설명
한다．


                                                      351
         시작하면서




       14장, "커널 디버깅 기술"에서는 리눅스 커널 내부를 디버깅하는 데 유용한 다양한 디버깅 기술
       을 설명한다. 커널 디버거인 KGDB를 사용하는 방법을 설명하고, gdb와 KGDB를 조합해
       서 디버깅 툴로 사용하는 유용한 디버깅 기술들도 설명한다. 그리고 하드웨어 JTAG 디버거
       에 대해서 알아보고 커널이 부팅되지 않을 때 분석할 수 있는 팁도 소캐할 것이다．

       15장, "임베디드 리눅스 어플리케이션 디버깅하71"에서는 디버깅 문맥을 커널에서 사용자 어플리
       케이션까지 확장해 볼 것이다. 이전 13. 14장에서 사용된 gdb를 이용한 예제를 더 알아보
       고, 다중쓰레드와 멀티프로세스 디버깅을 설명할 것이다．

       16장, "리눅스포팅"에서는자신의 보드에 리눅스를 포팅하는 문제를 다룬다. 간단한 예제에서
       시작해서 자체 PowerPC 보드에서 실제로 동작시키는 주요 단계를 요약해서 살펴볼 것이다．
       그리고 리눅스 커널을 처음 포팅하는 개발자들이 가장 크게 혼동하는 중요 개념들을 설명한
       다. 이 장의 내용을 이해한 뒤에는, 13장과 14장에서 설명한 기술들을 함께 이용해서 자신의
       보드에 리눅스 포팅을 시작할 수 있어야 한다．

       17장, "리눅스와 리얼 타임"에서는 임베디드 리눅스를 CONF'IG RT 옵션을 이용해서 리얼 타임
       으로 구성해서 개발하는 홍미로운 주제를 다룬다. 이용할 수 있는 리얼 타임 기능들을 알아
       보고, 시스템을 개발할 때 어떻게 사용할 수 있을지를 이야기할 것이다. 또한 자신의 어플리
       케이션이 갖는 지연성을 측정하는 기술도 설명한다．

       부록에서는 GNU 공공 라이선스, U-Boot로 구성 가능한 명령어들의 목록, BusyBox 명령
       어들, SDRAM 인터페이스에 대한 소캐 , 오픈 소스 개발자를 위한 리소스 그리고 인기 있는
       하드웨어 JTAG인 BDI-2000을 위한 예제 구성 파일을 제공한다．


따라 해보:
     71

       독자가 이 책을 읽으면서 이 책의 내용을 자신의 리눅스 워크스테이션에서 직접 확인해 보는
       것이 이 책을 이해하는 가장 좋은 방법이다. 구형 x86 컴퓨터를 하나 구해서 임베디드 시스
       템을 대상으로 실험해 보도록 하자. 그리고 다른 아키텍처에 기반한 단일 보드 시스템을 사
       용할 수 있다면 더 좋을 것이다. 거대한 코드 덩어리인 리눅스의 구조와 구성을 배우고, 커널
       이곳저곳을 돌아다니면서 많은 경험과 지식을 쌓을 수 있을 것이다．




U 36
                                          시작하면서   n 蚣1



    이 책에서 제시하는 코드를 보고 이해하려고 노력해 보자. 다른 값으로도 실험해 보고, 다른
    구성 옵션이나 하드웨어 장치를 대상으로도 실험해 보자. 많은 정보는 물론이고, 많은 재미
   도 느낄 수 있다！


GPL 저작권 고지
   이 책에 인용한 오픈 소스 코드들에 대한 저작권은 모두 여러 개발자들과 기부자들에게 있음
   을 말해 둔다. 이 책에서 사용된 코드들은 모두 GNU 공공 라이선스 또는 GPL에 의해서
   허가된 것이다．

   부록 A에서 GNU 공공 라이선스의 전문을 볼 수 있다．




                                                    37
필자는 언제나 오픈 소스 개발자들의 자비로움에 놀라곤 한다. 그리고 커뮤니티에
서 나보다 훨씬 뛰어난 능력을 가진 개발자들을 보고 겸허함을 느끼곤 한다. 필자는
이 책을 집필하는 과정에서 여러 가지 의문사항들에 대해서 리눅스 및 오픈 소스
커뮤니티의 여러 사람들에게서 많은 도움을 받았다. 그들은 필자가 올린 대부분의
질문에 대해서 금방 답해 주었고 격려도 잊지 않았다. 질문에 기꺼이 대답해 준 아
래의 리눅스와 오픈 소스 커뮤니티 회원들에게 감사하는 마음을 전하고 싶다.

탠 마렉（Dan Malek）은 2장, "임베디드 처음 경험하기"의 일부 내용에 대해서 아이
디어를 주었다．

댄 케겔（Dan Kegel)과 다니엘 자코보이치 (Daniel Jacobowitz）는 툴 체인과 관
련된 질문들에 꾸준히 답변해 주었다．

스콧 앤더슨（Scott Anderson）은 14장, "커널 디버깅 기술'에 나오는 gdb 매크로
에 대한 아이디어를 제공해 주었다．

브랫 딕슨（Brad Dixon）은 자신의 기술적인 경험으로 나의 기술적인 시야를 넓혀
주었다．

조지 데이비스（George Davis）는 ARM 관련 질문들에 대해서 답변해 주었다．

짐 루이스（Jim Lewis）는 }vITD 관련 내용에 대해서 의견과 제안 점을 알려 주었다．

칼 에릭슨（Cal Erickson）은 gdl그 사용에 대한 질문들에 답변해 주었다．
                                                    감사의 글



존 투오미（John Two毗y）는 3장, "프로세서 기본"의 내용을 집필하는 데 도움을 주었다．

리 리벨（Lee Revell) , 스볜m터오스텐 디트리히（Sven-Thorsten 11万etrich) 그리고 다니엘
워커（Daniel Walker）는 리얼 타임 리눅스를 다루는 내용을 쓰는 데 도움을 주었다．

그 외에도 AMCC , 임베디드 플래닛（Embedded I기anet), U出mate Solutions 그리고
United Electronic Industries 사에서 예제로 사용할 하드웨어를 지원해 준 점에 대해서
크게 감사한다. 또한 예제로 사용할 소프트웨어도 제공해 주고, 책을 집필하면서 가끔 회사
생활에 소홀할 수도 있었는데 잘 참아 준 고용주에거 감사드린다. 그 외에도 많은 사람들의
아이디어와 격려와 지원을 받았다. 그 모두에게도 감사하는 마음을 전한다．

그리고 이 책을 처음 리뷰해 준 팀에게 진정으로 감사의 말을 전한다. 그들은 이 책의 각 장
을 바로 읽고 아주 훌륭한 피드백과 아이디어 , 그리고 의견을 주었다. 아놀드 로빈스
(Arnold Robbins) , 샌디 테래스（Sandy Terrace) , 커트 로이드（Kurt Lloyd) 그리고 롭
파버（Rob Farber）에게 감사의 말을 전한다. 특히 아놀드는 기술 서적은 처음인 필자에게
책을 집필하는 방법을 잘 가르쳐 주었다. 혹시나 실수한 부분이 없는지 꼼꼼히 주의를 기울
였지만, 혹시나 실수가 있다면 모두 필자의 실수이다.

그리고 이 책을 성공적으로 쓸 수 있도록 끝없는 격려와 인내로 지원해 준 마크 L. 탑(Mark
L. Taub）에게 감사드린다！ 또한 크리스티 하트（Kristy Hart) , 제니퍼 크래머（Jennifer
Cramer) , 크리스타 핸싱（Krista Hans血g) 그리고 체릴 렌서（Cheryl Lenser）를 포함한
제작팀 모두에게 감사의 말을 전한다．

마지막으로 각 장을 쓸 때마다 매번 읽고, 지속적인 관심과 격려 그리고 희생으로 이 프로젝
트를 성공적으로 끝마칠 수 있도록 도와준 캐리 딜만（Cary Diliman）에게 진심으로 감사를
표한다．

                                          크리스 할라난(C方r幻 月可万na끄)




                                                               39 甘
             크리스토퍼 할리난은 현재 미국 매사추세츠 주에 거주하면서 몬타 비스타 소프트웨어
             사에서 필드 어플리케이션 엔지니어로 활동하고 있다. 25년 이상을 네트워킹과 통
             신 시장을 위한 제품들을 개발하면서 다양한 역할을 해 왔기 때문에 , 하드웨어와 소
             프트웨어가 만나는 부분에 대한 배경지식을 많이 가지고 있다. 몬타 비스타에 들어
             오기 전에는 4년 동안 독립적으로 자체 제작한 보드와 디바이스 드라이버 그리고
             부트로더를 제공하는 컨설턴트로 활동한 경험이 있다. 크리스는 유명한 U-Boot 부
             트로더에 참여하면서부터 오픈 소스 커뮤니티에 알려지게 되었다. 리눅스에 심취해
             있지 않을 때면 종종 태일러 , 마틴1) 기타를 연주하면서 노래하는 그를 발견할 수




1) ［역자주） 모두 유명한 기티의 이름이다．
Chap挺伊 ]




이번 징에서 배울 내용


  U 왜 리눅스인:7口

  U 임베디드 리눅스의 현재

  U 오픈 소스와 GPL

  U 표준 및 관련 조직

  U 요약
        Embedded Linux Primer




       기존에 사용하던 독자적인 운영체제를 버려야 한다면 많은 임베디드 운영체제 개발 회사의
       중역회의실이 술렁거릴 것이다. 여러 가지 장점으로 인해서 리눅스가 기존 서버 어플리케이
       션 시장을 장악하고 있던 운영체제의 영역으로까지 그 적용 범위를 넓혀가고 있다. 그리고
       임베디드 시스템 분야에서는 휴대폰이나, DVI) 플레이어 , 비디오 게임기 , 디지털 카메라, 네
       트워크 스위치 장비 그리고 무선 네트워크 장비 등에서 사용되고 있다. 이 말은 이미 독자의
       집이나 자동차에도 리눅스로 동작하는 장치가 있을 수 있다는 얘기가 된다．



] . ] 왜 리눅스인가？
       다양한 경제적 , 기술적 장점으로 인해서 임베디드 장치에 리눅스가 급속도로 영역을 넓혀가
       고 있음을 볼 수 있다. 이러한 경향은 사실상 모든 시장과 기술 전반에 걸쳐서 두루 나타나고
       있다. 리눅스는 전 세계를 연결하는 스위칭 기반 전화망이나 데이터 네트워크, 무선 핸드폰
       과 이러한 장치들을 운영하는 장비들에서 두루 적용되어 왔다. 차랑을 위한 제품에도 성공적
       으로 적용되었고, 게임기나 PDA , 프린터 , 대형 네트워크 스위치 , 라우티 등의 다양한 사용
       자 장치 등에서도 성공적으로 이용되고 있다. 이렇게 임베디드 리눅스가 사용되는 곳은 점점
       늘어나고 있으며 그 끝이 없어 보인다．

       임베디드 리눅스가 이렇게 성장하고 있는 이유로는 다음 몇 가지를 들 수 있다．

        口 리눅스가 기존의 독점적인 임베디드 운영체제에 비해서 충분히 성숙되고, 성능이 우수하
           며, 안정적인 운영체제로서 인정받고 있다．

        口 리눅스는 다양한 어플리케이션과 네트워크 프로토콜을 지원한다．

        口 작은 개인사용자를 위한 장치에서부터 대형 장비인 스위치나 라우터에도 사용 가능할
           정도로 확장성（Sc曲bil就y）이 뛰어나다．

        口 기존의 독점적인 운영체제와는 달리 별도의 저작권료（로열티） 없이 사용할 수 있다．

        口 리눅스는 수많은 활동적인 개발자들이 좋아하는 운영체제이고, 이 때문에 새로운 하드웨
           어 아키텍처나 플랫폼, 장치어］ 대해서도 빠른 지원을 받을 수 있다．

        口 사실상 모든 선두 업체는 물론이고, 점점 더 많은 하드웨어 및 소프트웨어 업체들이 리눅
           스를 공식적으로 지원하고 있다．




I 42
                                                                               소개    Chapter 1



        이러한 이유들 때문에 리눅스가 HD 텔레비전에서 무선 핸드폰까지 모두 포괄하는 다양한
        가정용 제품에도 급속도로 사용되는 것을 볼 수 있다．



1.2 임베디드 리눅스의 현재
        임베디드 시장에서 리눅스가 주목할 만한 성장을 한 것이 그리 놀랄 일은 아니라고 볼 수도
        있다. 사실 , 독자가 이 책을 읽고 있다는 것도 이미 리눅스가 독자의 삶에 어떠한 영향을 미
        치고 있음을 의미하는 것이다. 현재도 많은 업체들이 자신만의 임베디드 리눅스 제품을 만들
        어 내고 있기 때문에 임베디드 리눅스 시장의 규모에 대해서 예측하기는 매우 어렵다．

        리치 레바움（Rich Lehrbaurn)이 설립한 유명한 뉴스 및 정보 포털인 LinuxDevices.corn
        에서는 임베디드 리눅스 시장에 대한 조사를 매년 실시1) 하는데 , 마지막 조사에서는 리눅스
        가 매년 수천 개의 새로운 제품에서 주도적으로 가장 많이 사용되고 있는 운영체제로 나타나
        고 있다. 사실 , 조사에 응답한 기업의 거의 절반 정도가 임베디드 리눅스를 사용하고 있다고
        밝혔다. 또한 8깨 업체 중 1개 정도의 업체 꼴로 경쟁 운영체제를 사용하고 있다고 한다．

        한때 시장을 지배했던 상용 운영체제들은 10개 업체에서 1711 업체 꼴로 사용되고 있는 것으
        로 나타났다. 이러한 결과에 대해서 논쟁할 만한 다른 의견도 있을 수 있지만, 임베디드 리눅
        스가 오늘날 시장에서 갖는 힘에 대해서는 누구도 무시할 수 없을 것이다．



1.3 오픈 소스와 GPL
        리눅스가 적용되는 가장 기본적인 원동력 중의 하나는 바로 오픈 소스라는 사실이다. 리눅스
        커널은 유명한 신화 '리눅스는 무료2）이다를 낳게 한 GNU의 GPL(General Public
        License)3) 라이선스를 따르고 있다. 사실, GNU GPL의 두 번째 단락에서는 "우리가 프리4)
        (free) 소프트웨어라 함은 자유를 의미하는 것이다. 가격이 아니다."라고 말하고 있다. GPL
        라이선스는 무척 짧고 이해하기도 쉽다. 가장 중요한 특징으로는 다음과 같은 것들이 있다．


           ／八W叫. linuxdevices. COT可art姓明/A刃（石5740528. html에서 2007년도 조사 결과를 볼 수 있다．
1) ［역자주） h啣：
2) 대부분의 개발 관리자들은 리눅스가 비용 없이 무료로 다운로드할 수 있다는 점에는 동의한다. 하지만 어떤 운영체제든지 개발
   및 배포어七 （때빼로 막대한） 비용이 든다. 비용어］ 대해서는 1. 3. 1 절 "무료와 자유흩 보자．
3) 부록 A의 "GNU 일반 공중 사용 허가서"에 젼문이 수록되어 있다．
4) （역자주］ Free는 '공짜’라는 의미와 '자유'라는 의미를 모두 갖는 단어이다．


                                                                                            431
 , 鞋1   Embedded Linux Primer



        口 GPL 라이선스는 어떤 외부의 영향도 받지 않고 영원히 지속된다．

        [aGPL 라이선스는 사용자가 프로그램을 수행시킬 수 있는 자유를 보장한다．

        口 GPL 라이선스는 소스 코드에 대해서 공부하고 이를 수정할 권한을 보장한다．

        口 GPL 라이선스는 원래 소스 코드 및 사용자가 직접 수정한 소스 코드를 배포할 수 있는
           권한을 보장한다．

        口 GPL 라이선스는 사용자가 GPL 소프트웨어를 배포하는 누구에게나 같은 권한을 보장한다．


      소프트웨어 산출물이 GPL 라이선스로 공개된다면 이 소프트웨어는 반드시 GPL 라이선
      스5）를 영원히 보장해야 한다. 코드가 대폭 수정되었다고 하더라도, GPL은 이 코드를 같은
      라이선스로 배포되도록 명시하고 있다. 이러한 특징은 보통 수정판（der如ed work）이라고
      부르는 변경된 소스에 대해서도 모든 이들에게 공개되도록 하기 위함이다．

      GPL 라이선스는 소프트웨어를 어떻게 얻었는지와는 상관없이 저작권자에게 사용료를 지불
      할 필요 없이 무한대로 배포할 권한을 보장하기 위한 것이다. 하지만 이것은 제공자가 GPL
      소프트웨어에 대해서 가격을 책정할 수 없다는 의미는 아니다. 이는 매우 합리적인 사업 관
      례라고 볼 수 있는데 , 즉 한번 GPL 소프트웨어를 소유한 경우, 그것이 수정판이든 아니든
      이를 수정하고 재배포하는 것은 허용된다는 것이다. GPL 라이선스에서 정의하고 있듯이 수
      정 작업의 저작자는 자신의 작업에 대해서 GPL에 명시된 바를 따라야 한다. 사용자에게 배
      포하는 등의 모든 수정판에 대한 배포 역시 이 규칙을 따라야 한다. 하지만（표兀 라이선스에
      정의되어 있듯이 프로그램을 수정한 저작자（들）는 자신들이 그렇게 결정하는 경우 GPL 라
      이선스를 따르도록 할 수 있다 프로그램의 수정판에 대한 배포 절차는 사용자에게 판매하는
      것을 포함해서 모두 이 라이선스의 내용을 따라야 한다.

      오픈 소스 운동의 역사와 문화를 매력적이고 통찰력이 있는 관점에서 소개하고 있는 책으로
      는 이 장 끝의 참고도서 목록에 있는 에릭 레이몬드（Eric S. Raymond）의 책을 읽어 보기
      바란다．




5) 만약에 모든 GPL 라이선스의 저작권자가 동의한다면 이론적으로 해당 소프드웨어를 새로운 라이선스로 배포할 수도 있다. 물론
 일어날 것 같지 않은 일이긴 하지만．


144
                                                               소개    Chapter 1




1.3. ] 무료와 자유
      오픈 소스를 설명하는 딘어 중의 하나인 프리（free）에 대한 논쟁에는 보통 두 가지 유명한
      문구7} 반복적으로 언급되곤 한다. '조건적인 한도에서의 자유（Free as in freedom) '와 '무
      조건적인 공짜로서의 자유（Free as in beer) '가 그것이다（저자는 특히 후자가 마음에 든
      다）.GPL 라이선스는 소프트웨어 각각에 대한 '조컨적인 한도에서의 자유’를 보장하기 위한
      정책이다. 이것은 사용자가 그것을 사용하고, 분석하고 공부하며 , 수정할 자유를 보장하는
      것이다. 또한 사용자가 자신의 작업을 배포한 누구에게도 같은 자유를 보장하도록 하는 것이
      다. 이러한 개념은 지금은 꾀 많은 사람들에게 폭넓게 인식되었다．

      자주 듣는 잘못된 인식 중의 하나는 바로 리눅스는 '무조건 무료（Free as in beer) '라는 것
      이다. 물론 이 글을 읽고 있는 독자도 리눅스를 공짜로 구할 수는 있다. 리눅스 커널은 몇
      분 만에 쉽게 내려 받을 수 있게 되어 있다. 하지만 많은 전문가들이 공감하듯이 어떤 소프트
      웨어든지 그것을 실제 자신의 목적에 맞게 사용하기 위해서는 분명히 비용이 들게 마련이다．
      소프트웨어의 수집 , 통합, 수정 작업 , 유지 보수와 사용자 지원 등이 바로 이러한 비용 요소
      들이다. 이러한 비용 외에도 개발 환경에 맞게 최적화된 툴 체인6) (To아-chain) , 라이브러
      리 , 응용 프로그램이나 크로스 플랫폼 개발 도구 등을 구하고 유지해야 하는 비용이 들 것이
      고, 임베디드 리눅스에 맞는 소프트웨어 요소를 깨발하고 적용하는 게 그리 사소한 작업은
      아니라는 것을 금방 알 수 있을 것이다．



1.4 표준 및 관련 조직
      리눅스가 데스크탑 및 기업 환경과 임베디드 시장에까지 점유율을 넓혀감에 따라서 리눅스를
      적용하고 사용하는 데 힘을 더하기 위해서 새로운 표준 및 신흥 조직이 생겨나고 있다．


1.4. ] 리눅스 기본 규격
      아마 가장 중요하고 유일한 표준은 리눅스 기본 규격（LSB : Linux Standard Base）일
       것이다. 이 표준안의 목적은 서로 다른 리눅스 배포판 간에 응용 프로그램 상호 운용성을 개
       선시키기 위한 일련의 하위 표준안들을 마련하기 위함이다. 현재는 IA32/64, 파워PC

6) （역자주） 툴 체인 (Too卜chain）이란 어떤 수프트웨어의 개발에 필요한 일련의 개발 도구들을 모두 가리키는 말이다． 예를 들어， C
   컴파일러는 무엇을 사용하고， 어셈블러 및 링커는 어떤 것을 사용하는지 등의 환경을 의미한다．


                                                                            451
  難 a'     Embedded Linux Primer




         32/64 , AMD64 등의 여러 아키텍처에 대해서 표준을 정의하고 있고, 이 표준은 핵심 구성
         요소와 각각의 아키텍처에 대한 요소로 세분화된다．

         이 리눅스 기본 규격은 리눅스 배포판에 대해서 오브젝트7) 형식 , 표준 라이브러리 인터페이
         스, 최소한의 명령에 집합과 유틸리티와 그 각각의 역할, 파일 시스템 구조, 시스템 초기화
         등에 대해서 공통된 특성들을 정의하고 있다．

         리눅스 기본 규격에 대한 자세한 자료는 이 장의 마지막에 있는 1.5.1절 "더 읽어 보기"에서
         소개하고 있는 자료를 참고하기 바란다．


1.4.2 오픈 소스 개발 연구소

         오픈 소스 개발 연구소（OSDL）는 일반 시장에서 리눅스의 사용을 촉진시키기 위해 만들어
         졌다. 이러한 연구소의 기본 철학에 따라서 현재 대규모의 테스트 환경과 기술적인 지원을
         리눅스 커뮤니티에 제공하고 있다. OSDL은 몇 개의 위킹 그룹（working group)에 대해서
         시장의 중요한 3대 영역들에 대한 표준을 마련하고 개발에 참여할 수 있도록 지원하고 있다．
         다음에 소캐하는 세 개의 각 단락에서 몇 가치 주도적인 활동에 대해 알아보자．


         1.4.2.1 CGL : 통신망용 리눅스
         전세졔 규모의 네트워크 및 전화망 장치를 생산하는 대형 업체들의 많은 수가 통신망 장비
         의 개발은 물론이고 장비를 구동시키는 운영체제로 리눅스를 이용하고 있다. 통신망 장비는
         높은 안정성 , 높은 가용성 , 빠른 사용성 등이 중요한 사항이다. 이러한 장비 생산 업체들은
         제품을 디자인할 때 중복 구조8) (redundant) , 斗스왑（H毗田wap) 구조, 무 정지（fau此e
         t아erant) 기술, 클러스터링 등의 기술과 종종 실시간（rea卜time : 리얼 타임） 환경을 이
         용하기도 한다.

         CGL 워킹 그룹은 통신망급 장비에 필요한 일련의 요구 사항들에 대해서 명세서를 만들었는
         데 , 현재 버전은 총 7개의 기능적인 측면에 대해서 명시하고 있다．



7) （역자주） 오브젝트(obct）는 소스 코드를 빌드햐고 아직 링크되기 전의 결과물 파일을 의미하고， 그 파일의 형식을
                                                                    오브젝트 형
   식 佃bct 如rn묘t) 이라고 부른다．
8) （역자주） 중복（redundant)의 의미는 쉽게 생각해서, 같은 기능을 하는 하나 이상의 모듈이나 장치를 두어서, 문제나 고장이
                                                                            발생
   했을 때 같은 기능을 하는 다룐 모듈 및 장치를 대신 이용할 수 있도록 하는 개념이다．


146
                                                            소개    Chapter 1



         口 가용성（Ava始베ty) : 온라인을 통한 유지 보수 작업, 중복 구조, 상태 감시 등을 포함한
           개선된 가용성에 대한 요구 사항

         口 클러스터（이四也r引 : 클러스터의 구성 요소를 관리하거나, 그 데이터를 점검하는 등의 중
           복된 서비스를 쉽게 하기 위한 요구 사항

         口 사용성（Ser너ceabili幼 : SNMP 나 장치의 전원공급 장치 및 냉각팬을 감시하고 진단하는
           기능 등, 원격으로 서비스를 제공하고, 관리할 수 있도록 하는 요구 사항

         口 성능（Performance) : 성능, 확장성（scalabi玭y), 대칭형 멀티프로세싱 및 대기시간 등을
           정의하기 위한 요구 사항

         口 표준（Standarc招） : CGL 호환 장치가 따라야 할 표준을 정의하는 요구 사항

         口 하드웨어（Hardware) : 블레이드 서버와 같이 높은 가용성을 가진 하드웨어와 관련된 요구
           사항

         口 보안（Secur啣） : 다양한 공격어］ 대해서 전체적인 시스템 보안을 향상하기 위한 요구 사항


       1.4.2.2 MIL : 모바일 리눅스 이니셔티브9)(M야川e 니flux Initiative)
       이미 전 세계 시장에서 판매되는 핸드폰 제품 중에서 임베디드 리눅스를 이용해서 깨발된 몇
       몇 제품을 볼 수 있다. 보고에 따르면 수백만 대 이상의 핸드폰 제품이 리눅스를 기반으로
       하고 있다고 한다. 여기서 한 가지 확실한 점은 더 많은 제품이 그렇게 될 것이라는 것이다．
       또한, 기존에 독점적인 실시간 운영체제가 차지하던 시장에 대해서 폭발적으로 그 위치를 차
       지해 나갈 것으로 예측해 볼 수 있다. 이는 리눅스가 상용 임베디드 어플리케이션에 대해서
       도 준비되어 있다는 점에서 의미심장하다．

       OSDL은 M凡이라는 워킹 그룹을 후원하고 있다. 그 목적은 리눅스를 차세대 모바일 핸드폰
       및 기타 통합 이동 음성／데이터 통신 장치에 빠르게 적용하기 위함이다. 이 워킹 그룹이 중점
       을 두고 있는부분은 개발툴, 입출력(I/o) , 네트워킹 , 메모리 관리 , 멀티미디어 , 성능, 전원
       관리 , 보안 문제 , 저장 장치 등이다．




9) （역자주그 이니셔티브恤姓ative）는 입문, 입회, 창업 등의 의미를 갖는다. 해석하기에 적절한 단어가 없어서 바로 영문자를 표기
 했다．


                                                                         47 且
 醬 在a      Embedded Linux Primer




        1.4.2.3 서비스 :7匡썸 포럼（SA Forum)
        독자가 만약 높은 신뢰성 , 가용성 , 사용성（RAS'0)）이 요구되는 환경을 위한 제품을 개발하
        고 있다면 서비스 가용성 포럼（service availability forum)에 대해서 알고 있을 것이다．
        이 단체는 통신망용 장비나 기타 상업용 시스템 관리장비 등에서 사용되는 리눅스를 위한 공
        통된 인터페이스 집합을 정의하는 데 주도적인 역할을 하고 있다. 서비스 가용성 포럼의 웹
        사이트는 www.sa如rum.org이다.



1.5 요약
           口 임베디드 제품의 개발자와 생산 업체가 리눅스를 적용하는 사례가 빠르게 증가하
              고 있다．

           口 임베디드 장치에 리눅스를 사용하는 경우가 매우 빠른 속도로 증가하고 있다．

           口 이 장에서는, 임베디드 시장에서 리눅스가 빠른 성장률을 보이는 원인에 대해써 알아보
              았다．
           口 임베디드 리눅스에 영향을 미치고 있는 몇몇 표준 및 관련 조직에 대해서 소개했다．


1.5. ] 더 읽어 보기
           성당과 사장仕iie Ca比edral an（了 t力e Bazaar少
           Eric S. Raymond
           O'Relly, 2001


           라눅스 표준 규격 프로젝트（'Linux Standard Base 尸？（그／ect)
           www. linuxbase. org


           오픈 소스 개발 연구소（OSDL : Open Source Development Labs)
           www. osdl. org




10) （역자주） RAS는 신뢰성， 가용성， 사용성을 의미하는 Reliab小ty, Availab小甘, 駝rviceab小ty의 融 말이다．


148
            임베디드 처욤 경험하71




이번 장에서 배울 내용

  1 임베디드와 임베디드'F 아닌 것'7

  U 임베디드 시스템 해부

  U 저장 장치

  U 임베디드 리눅스 배포판

  U 요약
 難 月U    Embedded Linux Primer




        보통 주어진 일을 이해하는 가장 좋은 방법은 큰 그림을 잘 이해하는 것이다. 임베디드 시스
      템의 개발을 처음 접하는 사람에게는 많은 기본 개념들이 흥미롭게 다가올 것이다. 2장에서
      는 전형적인 임베디드 시스템과 개발 환경에 대해서 알아보며 , 특히 이러한 시스템 깨발을
       독특하고 어렵게 만드는 개념과 구성 요소에 역점을 둘 것이다．



2. ] 임베디드와 임베디드가 아닌 것？
      일반적으로 임베디드 시스템은 몇 가지 핵심적인 특징을 갖는다. 알다시피 누구도 데스크탑
      PC를 임베디드 시스템이라고 부르지는 않는다. 하지만 예를 들어 , 외부의 데이터 센터에 존
       재하는 데스크탑 PC 하드웨어 플랫폼이 하나 있고, 매우 중요한 감시 작업이나 알람 작업을
      수행하고 있다고 생각하1 보자. 또 이 데이터 센터에는 특별한 일이 없는한 직원이 부채중이
      라고 가정하자. 이런 상황에서는 하드웨어에 대해 다른 종류의 기능들이 요구된다. 예를 들
      면 천원이 끊겼다가 다시 들어온 경우에 작업자가 별도로 관여하지 않아도 스스로 자신의 작
      업을 재개할 수 있어야 한다．

      임베디드 시스템은 다양한 모양과 크기를 갖는데 , 가장 큰 멀티랙(I'加比卜rack1 ) 데이터 저
      장 장치나, 네트워크 집중 장비2）에서부터 개인용 MP3 플레이어나 핸드폰과 같은 작은 장치
       까지 다양하다. 일반적인 임베디드 시스템의 특징으로 다음과 같은 사항을 생각해 볼 수 있다．

         口 범용 마이크로프로세서와 같은 처리 능력을 가진 모듈이 존재한다．
         口 일반적으로 특정 목적과 용도를 가지고 만들어진다．
         口 자동차의 점화 장치를 제어하는 장치와 같이 사용자 인터페이스（UI）가 존재하지 않거나
            존재하더라도 아주 간단하다．
         口 메모리 용량이 아주 적거나 하드디스크가 존재하지 않는 둥 시스템 자원이 제한적인 경
            우가 많다．
         口 배터리로 동작해야 할 경우와 같이 전원 공급이 제한적인 경우가 있다．
         口 보통 일반 컴퓨터 환경으로 사용되지는 않는다．


1) （역자주） 보통 데이터 센터나 네트워크 징비들이 얇고 동일한 형태로 되어 있丑 그것들을 바퀴가 딜린 상자 안에 차곡차곡 쌓
 아 놓은 것을 볼 수 있는톄, 이를 멀티랙이라고 한다．
2) ［역자주） 원서에는 Ne伽야king Powerhouse라고 되어 있고, 이는 네트워킹 빌젼소라고 직역 가능햐다. 의미적으로는 거대한 규모
   의 녜트워킹을 처리하는 장치로 이해할 수 있다．


150
                                                        임베디드 처음 경험하71      Chapter 2




          口 동작어］ 필요한 응용 프로그램이나 하드웨어가 미리 설치 및 통합된 상태에서 판매된다．

          [a 어플리케이션이 사람의 간섭 없이 동작하는 경우도 많다．

       특히 임베디드 시스템은 일반 데스크탑 PC 환경에서 제한퇸 자원을 가지고 있다고 볼 수
       있다. 임베디드 시스템은 제한된 메모리와 존재하지 않거나 존채하더라도 적은 용량의 하드
       디스크를 갖고 있고, 네트워크 기능이 없는 경우도 많다. 그리고 종종 유일한 사용자 인터페
       이스가 시리얼3) 포트나 LED4) 몇 개일 때도 있다. 이러한 사항들이 임베디드 개발자에게는
       새로운 도전이 될 수 있다．


2.1. ] 텨（Js와 부트로더
       데스크탑 PC의 전원을 켜면 BIOS라고 부르는 소프트웨어가 CPU를 통해서 수행되기 시작
       한다（역사적으로 BIOS는 Basic I/O Software : 기본 입출력 소프트웨어의 약자이지만，
       현재는 처음의 기능보다 훨씬 복잡하고 다앙한 일을 하기 때문에 BIOS 자체를 하나의 용어
       로 인식한다）. 이 BIOS는 PC 판매 후에도 업그레이드가 가능하도록 하기 위해서 플래시
       메모리에 저장되어 있다（잠시 후에 다룰 것이다）.

       BIOS는 하드웨어 구조에 대해서 잘 알아야만 처리할 수 있는 하위 레벨의 초키화 등을 담당
       하는 복잡한 시스템 설정 루틴들을 구현해 놓은 것이다. 대부분의 사용자들은 이 日OS의
       기능과 범위에 대해서 잘 모르고 있지만, 데스크탑 컴퓨터에서 아주 중요한 부분이다. 전원
       이 켜질 때 CPU에 의해서 처음 수행되는 프로그램으로서 특히 메모리 서브시스템 등의 하
       드웨어를 초기화하고 하드 드라이브에 존재하는 운영체제를 메모리로 로드하는 일을 담당하
       고 있다．

       전형적인 임베디드 시스템似86 PC 하드웨어 플랫폼에 기반하지 않은 시스템을 가정하자）
       은 부트로더（80이幻ader）라고 불리는 소프트웨어가 그 기능을 대신한다. 만약에 독자가 자체적
       으로 임베디드 시스템을 개발하는 경우 개발 계획을 잡을 따1 보드에 맞는 부트로더를 개발하
       는 것도 반드시 포함시켜야 한다. 운 좋게도 독자가 개발하는 시스템에 맞도록 수정해서 사
       용할 수 있는 잘 작성된 오픈 소스 부트로더들이 몇 가지 있다. 오픈 소스 부트로더에 대해서
       는 7장, "부트로더"에서 알아볼 것이다．

3) ［역자주） 시리얼（Serial) 은 직렬을 의미한다. 시리얼 포트라는 용어가 하니의 고유 명샤처럼 흔히 사용되기 때문어］ 직렬 대신에
  시리얼을 직접 사용했다．
4) ［역자주） LED (Light Enii出ng Diodes) : 다이오드의 흐｝ 종류로 전류가 흐를 때 빛을 발하도록 되어 있다. 일반적으로 어떤 동작
   을 알리는 경우어］ 많히 사용된다．


                                                                                  511
          Embedded Linux Primer




       전원이 처음 들어 왔을 때 부트로더가 수행하는 중요한 일들은 다음과 같다．

          口 SDRAM 제어장치나 입출력 제어 장치 ,＼그래픽 제어 장치 등의 중요한 하드웨어 요소를
             초기화한다．
          口 제어권을 운영체제로 넘기기 위한 준비 과정으로 시스템 메모리를 초기화한다．
          口 주변 장치를 위해써 메모리 및 인터럽트 회로와 같은 시스템 자원을 필요어］ 따라 할당
             한다．
          口 운영체제 이미지를 시스템 메모리에 로드하고, 위치시키기 위한 메커니즘을 제공한다．
          口 운영체제를 로드한 후에 제어권을 운영체제로 넘긴다. 이때 운영체제가 시작하는 데 필
             요한 정보들을 넘겨주는데, 예를 들면 전체 메모리 크기나 클럭의 속도, 시리얼 포트의
             현재 설정 속도와 기타 하위 레벨 하드웨어 설정 정보 등이다．

       위에서 나열한 사항들은 전형적인 임베디드 시스템의 부트로더가 수행하는 일을 매우 간단히
       요약한 것이다. 여기서 기억해 두어야 할 중요한 점이 있다. 만약 임베디드 시스템을 직접
       디자인한 플랫폼에서 개발하고자 한다면 이러한 시스템을 위한 부트로더는 스스로 개발해야
       한다. 만약 ATCA5）와 같이 상업적으로 대량으로 제작되어 판매되고 있는 플랫폼（COTS6) )
       을 기반으로 시스템을 개발한다면 보통 부트로더는 보드와 함께 （흔히 리눅스 커널도 같이）
       제공될 것이다. 부트로더에 대해서는 7장에서 자세히 알아본다.



2.2 임베디드 시스템 해부
       ［그림 2-1］에 전형적인 임베디드 시스템의 블록 다이어그램을 나타냈다. 무선 AJDGAJD :
       Access Point) 장비에서 사용할 만한 고급 하드웨어 구성을 간단히 나타낸 것이다. 이 시스
       템은 32비트 RISC 프로세서를 사용하고 있다. 플래시 메모리는 비휘발성7) 프로그램이나
       데이터를 저장하는 데 사용된다. 주 메모리는 SDRA入ii이다. 이 SDRAM(Synchronous
       Dynamic Random Access 入/Iemory : 동기식 동적 램）은 아마 거의 모든 시스템에서 사용
       되는데 구동되는 프로그램에 따라서 수 메가바이트부터 수백 메가바이트까지 장착되기도 한
       다. 보통 보조 배터리가 장착되는 RTC(Real Time 이ock : 실시간 시계 장치）는 현재 시간

5) ATCA 플랫폼은 3장, "프로세서 기본"에서 소개힌r}.
6) （역자주） COTh (Commerc洌 0斗出e-she11 : 상업적으로 미리 제작되어 판매되는 제품을 의미하는 약어．
7) （역자주） 여기서 비휘빌성 (Noi的latile）은 시스템의 전원이 꺼져도 지워지지 않는 성질을 의미한다．


I 52
                                             임베디드 처음 경험하기      Chapter 2



    및 날짜를 유지하는 기능을 한다. 이 예제에는 RS-232는 물론이고 이더넷과 USB 인터페이
    스도 포함하고 있다. ［그림 2-1］의 802.11 칩셋은 무선 모뎀 기능을 수행한다．

     플래시 메모리                 메인 메모리
                                                 무선 모뎀
                                                              Y
                              SDRAM
      플래시                                         802.11
                                                   칩셋


                                32비트
                             RISC 프로세서

                    Serial    USB     이더넷
     리얼 타임          UART     컨트롤러     컨트롤러
      (TOD)
       클럭                                                  이더넷
                                                           (LAN)

    시리얼                                                USB
     포트

    I 그림 2너 임베디드 시스템의 여T

    보통 임베디드 시스템에서의 프로세서는 전통적인 CPU가 하는 것 이상의 기능을 수행한다．
    ［그림 2-1］에서 가정한프로세서는 시리얼 인터페이스를 위한 UART 및 USB, 이더넷 인터
    페이스를 내장하고 있다. 많은 프로세서가 보조 장치들을 프로세서 내부에 내장하고 있다．
    3장, "프로세서 기본'에서 이러한 통합된 프로세서에 대해서 몇 가지 예를 살펴볼 것이다．


2.2. ] 전헝적인 임베디드 리눅스 환경
    보통 임베디드 리눅스를 처음 접하는 개발자가 처음 하는 질문은 '개발을 위해서 어떤 것들이
    필요한가？'이다. 이 질문에 대답하기 위해 , 전형적인 임베디드 리눅스 개발 환경을 살펴보도
    록 하자（［그림 2-2] 참조）.




                                                                      531
         Embedded Linux Primer




                                              이더넷 허브
          호스트 개발 시스템




                                                                  口1          口g口
                                                             口口        ==＝二




                                                            임베디드
                                                            개발 타깃



                     蠶烈烈！蹄驟器裝澔．炒
                     b心m<4可mkn1平1rd 心件nhm1K衣m巾
                     m4H吐川心kdrd=7J11q1 1多，b1t
                     r如卜1. : .4L寸 C4m崎自出0
                     ibHhm4 知114i自蜘才m; 1心

                     큼뻔客繫器史崙燾笛客島駐. (m험I好蚣．
                     外m: 啣懈加·    m6k텍呻겨的 i쏘

                     向心（d牛
                                              念難羲
                                                        시리얼 터미널
                                                    j




      I 그림 ?2 임베디드 리눅스 개발 환경


      그림과 같은 구성이 일반적인 개발 환경인데 , 호스트 개발 시스템은 레드햇이나 수세
       (SuSE) , 데비안등의 유명한 데스크탑용 리눅스배포판을설치한시스템일 것이다. 그리고
      개발하고 있는 임베디드 리눅스 타깃 보드는 호스트 개발 시스템과 RS-232 시리얼 케이블
      을 통해서 연결되어 있다. 여기에 타깃 보드의 이더넷 인터페이스를 이더넷 허브나 스위치에
      연결한다 호스트 역시 이더넷 케이블을 연결한다 호스트 개발 시스템은 개발 툴 및 유틸리
      티와 임베디드 리눅스 배포판에서 얻은 타깃 파일을 가지고 있다．

      이 예제에서는 임베디드 리눅스 타깃에 주된 연결 채널로 RS-232 연결을 사용하는 것을 알
      수 있다. 이 경우 타깃 보드와 통신하기 위해서 시리얼 터미널 프로그램이 사용되는데 미니
      컴8) (Minicom)은 가장 많이 사용되는 시리얼 터미널 프로그램이며 , 사실상 모든 리눅스 배
      포판에 포함되어 있는 프로그램이다．




8) ［역자주） Mmn油m은 리눅스 호스트 환졍에서 가장 많히 人｝寄1가. 윈도우 환경에서는 TeraTerm, 이야기 시리즈， 햐이퍼 터미녈
 등 매우 다양한 프로그램이 사辛 다．


154
                                                      임베디드 처음 경험하71   Chapter 2




2.2.2 타깃 보드 구동하키
      처음 전원이 공급되면 타깃 보드와 함께 제공된 부트로더가 즉시 CPU를 통해서 구동된다．
      이 부트로더는 프로세서와 메모리의 초기화, 시리얼 포트를 제어하는 UART , 이더넷 컨트롤
      러의 초기화 등을 포함한 아주 하위 레벨의 하드웨어 초기화를 진행한다．

      ［리스트 2-1］은 보드에 전원이 공급되어 부팅이 진행되면서 시리얼 포트를 통해서 출력된
      내용을 나타낸 것이다. 이 예제에서는 AMCC에서 만든 요세미티9）라는 별명을 가진
      PowerPC 440EP 프로세서 기반의 개발 보드를 이용했다．

      ［리스트 2-1] 부트로더의 초기화 시리얼 출력


         U-Boot 1.1. 4 (Mar 18 2006 - 20: 36:11)


         AMCC PowerPC 440EP Rev. B
         Board: Yosemite - AMCC PPC440EP Evaluation Board
                  VCO: 1066 MHZ
                  CPU: 533 MHZ
                  PLB: 133 MHZ
                  OPB: 66 MHZ
                  EPB: 66 MHZ
                  PCI: 66 MHZ
         I2C:    ready
         DRAM:   256 MB
         FLASH: 64 MB
         PCI:    Bus Dev venid Devld Class mnt
         In:     serial
         Out:    serial
         Err:    serial
         Net:    ppc_4xx_ethO, ppc_4xx_ethl


         =>
9) C역자주） 요세미티는 미국 캘리포니아에 있는 유명한 국립공원의 이름이다．


                                                                             55   I
        Embedded Linux Primer




      요세미티 보드에 전원이 공급되면 U-Boot（유부트）가 수행되면서 하위 레벨의 하드웨어 초
      기화를 수행하는데 , 여기에 시리얼 포트의 초기화도 포함된다. 그 후에는 ［리스트 2-1]의
      맨 첫줄에서 보는 것과 같이 U-Boot의 버전을 알리는 문자열이 출력된다. 그 후에 프로세서
      의 이름과 칩의 리비전10) (revision) 정보가 출력되고, 이어서 보드의 종류를 표시하는 문자
      열이 출력된다. 이 문자열들은 U-Boot 소스 코드에 개발자가 입력해 놓은 것이다．

      이제 U-Boot는 （시리얼 포트로 문자열이 출력되기 이전에 미리 설정이 완료된） 내부 클럭
      정보를 출력한다. 여기까지 진행된 후에 U-Boot는 미리 정적으로 설정된 절차에 따라서 하
      드웨어 서브시스템들을 설정하기 시작한다. 이 과정에서 12G. DRAM. FLASH. PCI 그리
      고 네트워크 서브시스템이 초기화된다. 마지막으로 U-Boot는 프롬프트 문자 =）를 나타내
      고 시리얼 포트상의 콘솔을 통해서 사용자의 입력을 기다리게 된다．


2.2,3 커널 부팅하키
      이제 U-Boot가 시리얼 포트와 이더넷 인터페이스 및 기타 하드웨어를 초키화했는데 , 이제
      이 부트로더의 짧지만 유용한 여생 동안에 마지막으로 한 가지 중요한 일이 남았다. 바로 커
      널을 로드하고 부팅시키는 것이다. 모든 부트로더는 운영체제 이미지를 로드하고 실행시키기
      위한 명령어를 가지고 있다. ［리스트 2-2］는 U-Boot를 이용해 리눅스 커널을 로드해서 부
      팅시키는 일반적인 방법 중 한 가지를 나타낸 것이다．

      ［리스트 ?2} 리눅스 커널 로드하71


         => tftpboot 200000 ulmage-440ep
         ENET Speed is 100 Mbps - FULL duplex connection
         Using ppc_4xx1eth0 device
         TFTP from server 192.168.1.10; our IP address is 192.168.1.139
         Filename 'ulmage-amcc ' .
         Load address: 0x200000
         Loadi ng: ####################################################
                   ######################################
         done
         Bytes transferred = 962773 (eb0d5 hex)



10) （역자주） re미엷on은 칩에 어떤 수정을 가해서 다시 생산할 때 칩을 구분하기 위해서 붙이는 이릅이다. 칩의 버전이라고 생각할
    수 있다．


156
                                                   임베디드 처음 경험하기         Chapter 2




  => bootm 200000
  ## Booting image at 00200000 . . .
    Image Name:     Linux-2. 6. 13
    Image Type:     PowerPC Linux Kernel Image (gzip compressed)
    Data Size:     962709 Bytes = 940.1 kB
    Load Address: 00000000
    Entry Point: 00000000
    verifying Checksum . . . OK
    Uncompressing Kernel Image . . . OK
  Linux version 2. 6.13 (chris@junior) (gcc version 4.0. 0 (DENX ELDK 4. 0 4.0. 0))
  니 #2 Thu Feb 16 19: 30:13 EST 2006
  AMCC PowerPC 440EP Yosemite Platform


  < 많은 커녈 부탐 머M／자들0/ 출력됨． 섕락 >


  amcc login:     <<< 리눅스 커널의 명령0/ 프롬프트




여기서 七ftpboo七 명령어는 U-Boot에게 커널 이미지 ulmage寸440ep를 TFTP 프로토콜
을 이용해서 네트워크 상의 메모리로 로드하도록 한다. 이 경우 커널 이미지는 개발 위크스
테이션（일반적으로 보드와 시리얼로 연결되어 있는 PC일 경우가 많다）에 위치하고 있다．
tftpboo七 명령어는 커널 이미지가 로드될 메모리의 위치인 보드의 물리 주소를 인자로 넘
겨받는다. 자세한 부분까지 지금 모두 이해하지 않아도 된다. 7장에서 U-Boot어］ 대해 아주
자세히 다루겠다．

다음으로 bootm(boot from memory image : 메모리상의 이미지를 부팅시키기） 명령이
나오는데 , 이 명령은 U-Boot에게 ho毗m의 인자로 넘어온 주소에 존재하는 방금 로드한 커
널을 부팅시킨다. 이 명령어는 CPU 제어권을 리눅스 커널에게 넘긴다. 커널이 올바로 설정
되었다면 로그인 프롬프트를 보면 알 수 있듯이 리눅스 커널이 타깃 보드의 콘솔을 통해서
부팅되는 것을 볼 수 있다．

여기서 bootm 명령을 통해서 U-Boot가 그 기능을 다하고 소멸된다는 것에 주의하자. 이는
상당히 중요한 개념인데 , 데스크탑 PC의 비Os와는 달리 , 대부분의 임베디드 시스템에서는
임베디드 리눅스가 제어권을 얻는 순간 부트로더는 그 기능을 마치고 제거되는 구조를 갖는
다. 이는 커널이 부트로더가 이전에 사용했던 시스템 자원이나 메모리에 대해서 소유권을 가


                                                                               5' I
 難1 1     Embedded Linux Primer




        지려고 하기 때문이다. 부트로더로 다시 제어권을 넘기는 유일한 경우는 보드를 재부팅할 경
        우뿐이다．

        마지막으로 살펴볼 부분은 별로 중요한 부분은 아닌데 , bootm 명령 이후부터 다음 메시지가
        출력되는 곳까지는 口Boot가 출력하는 메시지이다．

          Uncompressing Kernel Image . .. OK


        이후의 부트 메시지들은 리눅스 커널이 내보내는 것이다. 이 부분에 대해서는 나중에 좀더
        자세히 알아보기로 하고, U-Boot가 사라지고 리눅스 커널이 제어권을 넘겨받는다는 의미만
        이해하고 넘어가자．


2.2.4 커널 초기화 : 요약
        리눅스 커널이 실행되면 커널은 꾀 다양한 일을 수행하는 부팅 과정에서 여러 상태 메시지를
        출력한다. 여기서 디루는 예제에서는 리눅스 커널이 로그인 프롬프트가 출력되기 전까치
        100줄 이상의 문자열을 뱉어 냈다（이 책에서는 핵심 내용을 좀 더 명확히 하기 위해 그 부분
        을 생략했다）. ［리스트 2-3］은 로그인 프롬프트 이전에 출력된 몇몇 라인을 다시 나타낸 것
        이다. 이 예제의 목적은 커널의 초기화에 대한 자세한 사항까지 깊이 들어가는 것은 아니고
        （커널 초기화에 대한 자세한 내용은 5장, "커널 초기화'에서 다룬다）, 리눅스 커널이 부팅하
        는 데 어떤 요소들이 필요하고, 어떤 일들이 일어나는지를 개념적으로 이해하는 것이다．

        ［리스트 ?3] 리눅스 부트 메시지의 마지막 부분



          Looking up port of RPC 100003/ 2 on 192.168. 0. 9
          Looking up port of RPC 100005/1 on 192.168. 0. 9
          yES: Mounted root (nfs filesystem) .
          Freeing mnit memory: 232K
          INIT: version 2. 78 booting



          coyote login:




I 58
                                                   임베디드 처음 경험하기     Chapter 2




      리눅스는 시리얼 터미널에 로그인 프롬프트를 보여 주기 전에 , 루트 파일 시스템을 마운트한다．
      ［리스트 2-3］을 보면 리눅스가 （이더넷을 통해서） II) 주소가 192.168.0.9인 원격의 NF
       sil) 서버를 통해서 루트 파일 시스템을 마운트하는 과정을 밟고 있는 것을 알 수 있다. 보통
       이 NFS 서버로는 개발자가 현재 개발용으로 사용하고 있는 워크스테이션을 사용한다. 루트
       파일 시스템은 GNU／리눅스 시스템을 이루는 응용 프로그램들, 시스템 라이브러리 , 유틸리
      티 등이 포함되어 있다．

      이와 같은 과정은 절대로 무시할 수 없는 중요한 부분이다. 즉, 리눅스는 파일 시스템을 필요로
       한다는 것이다. 기존 임베디드 운영체제 중의 상당수가 파일 시스템을 필요로 하지 않는다．
      이러한 점은 기존 임베디드 Os를 이용해서 개발하던 개발자가 임베디드 리눅스를 통해서
       개발하려고 할 때 주로 당황하게 되는 부분이다. 미리 정의된 일련의 시스템 디렉터리와 파
       일들을 하드디스크나 기타 저장 매체에 정해진 구조에 맞게 구성해서 , 이를 리눅스 커널이
       루트 파일 시스템으로 마운트하는 것이다.

      리눅스가 루트 파일 시스템으로 마운트할 수 있는 장치에는 여러 가지가 있다. 물론 독자가
      개발 워크스테이션으로 사용하고 있는 리눅스와 같이 하드디스크 드라이브에서 하나의 파티
       션을 루트 파일 시스템으로 사용하는 것이 가장 일반적인 방법이다. 물론 NFS는 제품의 7긔1
       발이 완료되고 출고가 되어서 개발 환경을 벗어나면 거의 의미가 없는 방법이다. 하지만 이
       책을 계속 읽어 나가다 보면 개발 환경에서만큼은 NFS를 이용해서 루트 파일 시스템을 마운
       팅하는 것이 강력하고 유연한 방법이라는 것을 인정할 것이다.


2.2.5 첫 번쩨1 사용자 영역 프로세스 : in仕
       진행하기 전에 중요한 사항 한 가지를 더 짚고 넘어가야겠다. ［리스트 2-釗에서 다음을 보자．

          INIT: version 2. 78 booting.

       이 메시지 이전까지 커널은 커널 컨텍스트12)(kern이 con伯xt)라고 알려진 영역에서 다앙한 초기
       화 과정을 수행하는 코드 덩어리 그 자체였다. 이 동작 모드에서 커널은 시스템의 모든 메모
       리를 소유하고, 시스템 자원에 대해서도 모든 권한을 가진 상태로 수행된다. 즉, 커널은 모든
       물리적인 메모리와 입출력 서브시스템에 대해서 접근 권한을 가지고 있다．


11) NFS와 그 외 필요한 서버들어］ 대해서는 12장에서 다룬다．
12) （역자주） 모든 권한을 갖고 실행되는 프로세서의 상태, 유저 컨텍스트（U얹才 conte玭）눈 제한된 권한을 갖고 있는 영역이다．


                                                                           59 I
 難 月1      Embedded Linux Primer




        커널이 내부적인 초기화를 마치고, 루트 파일 시스템을 마운트하고 나서 기본적으로 수행하
        는 작업은 Jnit이라고 불리는 응용 프로그램을 생성하는 것이다. 커널이 mnl七을 시작시키
        면 mnit은 유저 컨텍스트 또는 유저 영역 컨텍스트에서 수행된다. 이 동작 모드에서는, 유저
        영역 프로세스는 시스템에 대해서 제한된 접근 권한을 가지고, 장치 및 파일 입출력을 위해
        서는 커널이 제공하는 시스템 콜을 이용해야만 한다. 이러한 유저 영역 프로세스, 프로그램
        은 임의의13) 가상 메모리 공간에서 동작하고, 이 가상 메모리는 커널이 관리한다. 커널은
        프로세서가 제공하는 특별한 메모리 관리 장치의 도움으로 유저 영역의 가상＝물리 주소 변환
        을 수행한다. 이 구조의 가장 큰 장점은 하나의 프로세스에서 발생한 에러가 다른 프로세스
        의 메모리 영역까지 침범하지 않는다는 점이다. 원인을 추적하기 힘든 버그를 만들어 낼 수
        있는 다른 프로세스의 메모리 침범 문제는 기존의 임베디드 운영체제들이 공통적으로 가지고
        있던 문제였다．

        여기서 설명한 개념이 낯설게 느껴져도 걱정하치 말자. 이 책을 읽어 나가면서 자세히 배우
        게 될 지식에 대해서 큰 그림을 한번 그려 보는 것이 이 장의 목적이다. 지금까지 설명한 내
        용들은 이어지는 장들에서 자세히 다룰 것이다．



2.3 저장 장치
        임베디드 시스템에서 가장 도전적인 면은 대부분의 임베디드 시스템이 물리적으로 제한된 자
        원을 가지고 있다는 점이다. 독자가 사용하는 펜티엄4 데스크탑 PC는 아마 180GB 이상의
        하드디스크를 가지고 있을 수도 있지만, 임베디드 시스템에서 이런 경우는 흔하지 않다. 많
        은 경우 임베디드 시스템에서 하드 드라이브는 더 저렴하고 작은 비휘발성 저장 장치로 대체
        된다. 하드 드라이브는 우선 부피가 크고. 회전하는 모터를 가치고 있고, 충격에 민감하며，
        여러 전압 레벨을 필요로 하기 때문에 임베디드 시스템에는 대부분 적합하지 않다．


2.3. ] 푿래시 메모리
        CF 카드（Compact까ash'4) ) 모듈을 모르는 사람은 아마 없을 것이다. 디지털 카메라나
        PDA（둘 다 대표적인 임베디드 시스템이다） 등의 다양한 기기에서 사용되는 모듈이다. 이
        모듈은 작은 크기에 수 메가바이트에서 수 기가바이트까지 저장할 수 있는 일종의 고체

13) 사실 임의로 가상 메모리 주소가 힐당되는 것은 아닌데, 이 부분어］ 대해서는 뒤에서 자세히 다룬다．
14) 자세한 내용은 www. comm蛇出ash. org를 참고하자．


160
                                  임베다드 처음 경험하71   Chapter 2



(solid-state) 하드 드라이브로 생각할 수 있다. 이 모듈은 모터처럼 움직이는 부품이 없고，
하나의 공통 천압 레벨로 동작한다．

플래시 메모리를 생산하는 업체는 여러 곳이 있고, 다앙한 형태와 용량의 플래시 메모리가
생산된다. 임베디드 시스템에서는 1MB나 암i1B 청도의 적은 비휘발성 메모리만을 가진 경
우도 드물지 않다. 하지만 임베디드 리눅스를 구동시키기 위한 시스템에서는 4MB에서
256MB나 그 이상의 용량을 가진 경우가 이상적이다. 임베디드 리눅스 시스템에서 기가바
이트 급의 비휘발성 메모리를 가진 경우도 증가 추세에 있다．

플래시 메모리에 데이터를 기록하고지우는 것은 소프트웨어를 통해서 제어한다. 아직까지는
하드 드라이브 기술이 가장 빠른 저장 매체이다. 비록 플래시 메모리가 하드 드라이브에 비
하면 여전히 상대적으로 느리지만, 플래시 메모리의 데이터 쓰기 및 지우기 속도도 시간이
갈수록 점점 빨라지고 있다. 플래시 메모리를 올바로 활용하기 위해서는 하드 드라이브와 플
래시 메모리 기술의 몇 가지 근본적인 차이점에 대해서 반드시 이해하고 있어야 한다．

플래시 메모리는 삭제 단위 블록（erase block）이라고 부르는 상대적으로 큰 용량의 지우기
가능한 조각들로 나뉜다. 플래시 메모리를 정의하는 가장 큰 특징 중 하나는 데이터를 기록
하고 지우는 방식이다. 전형적인 플래시 메모리 칩에서는 값이 1인 비트를 0으로 바꾸는 것
은 비트 단위로든 워드 단위로든 제약 없이 소프트웨어적으로 변경이 가능하다. 하찌만 값이
0인 비트를 다시 1로 만들기 위해서는 해당하는 블록 전체를 지워야 한다. 그러한 이유 때문
에 데이터 블록을 흔히 삭제 단위 블록이라고 부르는 것이다．

전형적인 플래시 메모리는 수많은 삭제 단위 블록을 가치게 된다. 예를 들면, 4MB 용량의
플래시 칩은 아마 64KB 용량의 삭제 단위 블록을 64개 가지고 있을 수 있다. 또한 유연한
데이터 저장 구조를 지원하기 위해서 하나의 플래시 메모리 내의 삭제 단위 블록의 크기가
각각 다를 수도 있다. 흔히 부트로더가 적은 용량의 블록에 저장되고, 커널 및 기타 필요한
데이터들은 큰 용량의 블록에 저장되는 방식이 많이 사용된다. ［그림 2-3］은 맨 처음에 부트
블록이 존재하도록 만들어진 플래시의 전형적인 구조이다．




                                                         61 1


                  a
          Embedded Linux Primer




        최상위 부분




                                        몌인 블록

                             64KB

                             64KB
        최하위 부분                      /

        I 그림 ?3 부트 블록을 가진 플래시 구조


        플래시 메모리에서 데이터를 수정하기 위해서는, 먼저 수정될 데이터가 존재하는 블록을 완
        전히 삭제15）해야 한다. 단지 바이트 하나만 수정해야 할 경우라도 전쳬 블록을 지우고 다시
        기록16）해야 한다. 전통적인 하드 드라이브의 섹터 크기에 비하면 플래시 메모리의 블록 크
        기는 매우 크다고 할 수 있다. 비교하자면 고성능의 하드 드라이브는 512바이트나 1024바
        이트의 섹터 크기를 갖는다. 결과적으로 테이터를 기록할 때마다 매번 큰 크기의 블록을 전
        부 다시 기록해야 하기 때문에 플래시 메모리의 데이터 기록 시간이 하드 드라이브에 비해서
        훨씬 오래 걸린다. 그래서 최악의 경우 데이터를 기록하는 데 수초가 걸리기도 한다.

        플래시 메모리의 또 다른 제약사항은, 메모리 셀이 수명을 갖는다는 점이다. 플래시 메모리
        셀은 제한된 수만큼만 쓰기가 가능하며 , 그 이상 쓸 경우엔 올바른 값을 보장하지 않는다．
        물론 쓰기 가능 횟수가 충분히 많기는 하지만（보통 블록당 10만 번 정도이다）, 잘못된 저장
        알고리즘으로 플래시 메모리에 접근한다면 빠른 시간 안에 플래시 메모리의 수명이 다할 것


15) （역자주） 물론 특수한 경우로 수정할 바이트의 값이 모두 비트 값 l로만 구성된 0妊下이고, 이 값을 血00 등으로 바꾸는 경우는
    지우지 않고도 가능하다. 하지만 이런 경우는 극히 예외적인 경우라고 볼 수 있다．
16) 데이터에서 비트 값 l을 0으로 바꾸는 것은 삭저］ 없이도 가능하지만, 반대의 경우는 블록 젼체를 지워야 가능하다는 것을 기억
  하자．


I 62
                                                  임베디드 처음 경험하기     Chapter 2



      을 쉽게 예상할 수 있다. 말할 필요도 없이 리눅스의 시스템 로거17) (logger）가 플래시 장치
      에 출력 값을 기록하도록 하는 등의 일은 피해야 한다．


2,3.2 NAND18) 푤래시
      NAND 플래시는 비교적 최근의 기술이라고 할 수 있다. NAND 플래시가 시장에서 큰 성공
      을 거두고부터 , 방금 다루었던 것과 같은 기존에 사용되던 플래시 메모리를 NOR 플래시라
      고 부르게 되었다. NAND나 NOR와 같은 구분은 플래시 메모리 셀의 내부 구조의 차이에서
      기인한다. NAND 플래시가 기존의 NOR 플래시에 비해서 개선된 점은 훨씬 작은 크기의
      삭제 단위 블록을 지원한다는 점이다. 그 결과 데이터를 기록하는 데 좀 더 빠르고 효율적인
      처리가 가능하고, 플래시의 저장 공간을 좀 더 효율적으로 사용하도록 해 준다.

      NOR 플래시가 마이크로프로세서와 인터페이스하는 방식은 다른 많은 보조 장치들과 비슷
      하다. 그 방식이라 함은 병렬로 이루어진 데이터 , 주소 버스를 통해서 마이크로프로세서와
      직접 연결되는 방식을 말한다. 그래서 플래시의 특정 바이트나 워드 주소에 제한 없이 임의
      로 접근할 수 있다. 하지만 NAND 장치는 생산 업체마다 다른 복잡한 방식으로 직렬로 데이
      터를 접근해야 한다. 기존의 하드 드라이브와 하드 드라이브 컨트롤러가 사용하는 방식과 비
      슷한 동작 방식을 이용한다. 즉, 데이터가 직렬 버스트19) (burst）로 전송되고, 블록 크기도
      NOR 플래시의 블록 크기보다 훨씬 작다. 그리고 NAND 플래시는 NOR 플래시에 비해서
      기록 가능 횟수는 훨씬 많고, 블록을 지우는 데 걸리는 시간은 훨씬 짧다．

      요약하면 NOR 플래시는 마이크로프로세서에 의해서 메모리처럼 직접 접근이 가능하고, 코
      드도 바로 실행이 가능하다（하지만 성능상의 이유 때문에 , 시스템 자원이 극히 제한된 경우
      를 제외하고는 그렇게 하는 경우는 별로 없다）. 사실, 많은 프로세서가 플래시에서 명령어를
      수행할 때 DRAM처럼 명령에 캐시(instruction cache）를 사용할 수 없게 되어 있다. 이
      때문에 명령에 수행 시간이 더 늦어지게 된다. 반면 NAND 플래시는 실행 바이너리 코드나，
      로우（Raw) 데이터를 저장하는 용도보다는 파일 시스템을 이용하는 대용량의 저장 공간으로
      사용하는 것이 적합하다．



17) （역자주） 로거 如gger）는 일빈적으로 어떤 동작이나 츤妃뀨를 감시해서， 그 정보를 기록해 두는 모듈이나 프로그램을 말힌다．
18) ［역자주） NAND 플래시를 어떤 이는 낸드 플래시， 또 어떤 이는 난드 플래시라고 발음한다．
19) （역자주） 버스트 젼송은 데이터가 1呱价 등을 통해서 쉬지 않고 한꺼번에 끝까지 젼송되는 것을 말한다． 기존의 CPU가 한 워드
    씩 데이터를 읽어오는 방식과 비교할 때 훨씬 빠르다．


                                                                          631
   寡a    Embedded Linux Primer




2.3.3 플래시의 사용
        임베디드 시스템을 디자인함에 있어서 플래시 메모리를 어떤 구조 및 구성으로 사용할지에
        대한 다양한 선택이 있을 수 있다. 가장 간단한 시스템에서는 시스템 리소스를 많이 절약해
        야 하는 경우가 아니라면 플래시 메모리에 가공되지 않은 바이너리 데이터를 （아마도 압축해
        서） 저장하기도 한다. 그래서 시스템이 부팅될 때 , 플래시 메모리에 저장되어 있는 파일 시스
       템 이미치를 리눅스의 램디스크 블록 디바이스로 읽어 들인다. 그리고는 파일 시스템으로 마
        운트시켜서 RAM을 통해서만 접근하도록 한다. 이러한 경우는 플래시 메모리에 저장되어 있
        는 데이터가 거의 수정될 필요가 없는 경우나, 수정될 경우라도 램디스크 크기보다 상대적으
        로 적은 부분만 수정될 경우에 적합한 방법이다. 여기서 중요한점은 램디스크에 존재하는
        파일 시스템 상에서 어떤 파일을 수정하더라도 재부팅 후에는 그 수정된 내용이 소멸된다는
        점이다．

       ［그림 2-4］는 비휘발성 저장 장치에 기록된 데이터에 대해서 , 동적으로 변하는 데이터의 양
        이 적거나, 데이터의 수정이 드물게 일어나는 임베디드 시스템의 경우에 적합한 플래시 메모
        리의 구조이다．

        최상위 부분
                                   부트로더 &
                                   설정 정보

                                            5毋g甕朴i王打立a,


                                  리눅   「커「｛  ,,,,,
                               램디스크
                            파일 시스템 이미지


                                 업그레이드 영역


       I 그림 ?4 플래시 메모리 구성의 여T


       부트로더는 보통 플래시 메모리의 최상위나 가장 아랫부분에 존재한다. 부트로더 다음에는
       리눅스 커널 이미지가 들어갈 공간이 할당되어 있고, 그 다음에 루트 파일 시스템을 담고 있
        는 램디스크 파일 시스템 이미지가 위치하게 된다. 보통 리눅스 커널 및 램디스크 파일 시스


I 64
                                                    임베디드 처음 경험하11    Chapter 2



      템 이미지는 압축된 경우가 대부분인데 , 부트로더가 부팅 과정에서 이미지의 압축을 푸는 일
      을 수행한다．

      부팅이 되거나 전원 공급이 중단되는 경우에도 저장되어야 할 데이터를 위해서 플래시 메모
      리의 일부 영역을 할당하거나, 다른 종류20）의 비휘발성 메모리가 사용된다. 이 예제와 같이
      설정 정보를 저장하는 형태를 가지는 임베디드 시스템은, 시장에서 판매되는 무선 공유키와
      같은 장치를 예로 들 수 있다．


2.3.4 푿래시 파일 시스템
      이전 단락에서 살펴본 간단한 플래시 메모리 구성은 매우 제한적이다. 그래서 하드디스크에
      데이터를 저장하는 것과 같이 플래시 메모리에 파일 시스템을 구성해서 데이터를 관리하는
      방법을 이용하면 이러한 한계를 극복할 수 있다. 초기 플래시 메모리 파일 시스템의 경우에
      는 하드디스크의 512바이트 섹터 구성을 에뮬레이트（emmate)21）하는 수준의 간단한 블록
      디바이스 층으로 이루어져 있었다. 이 에뮬레이션 층으로 인해서 데이터를 （형식 없는 데이
      터 덩어리 단위가 아닌） 파일 단위로 접근할 수 있게 되었지만, 몇 가지 성능상의 제한점이
       있었다．

      플래시 파일 시스템에서 가장 큰 기술적인 도약 중 하나는 웨어 레벨링（wear leveling）을
      도입한 것이다. 이전에도 살펴보았지만, 플래시의 메모리 블록은 수명이 정해져 있다. 웨어
      레벨링 기술은 플래시 메모리 내부에 존재하는 삭제 단위 블록에 대해서 , 각 블록이 실제로
      삭제되는 경우를 균등하게 분포시키기 위한 알고리즘이다．

      플래시 파일 시스템 구조가 갖는 또 다른 제약 사항은 전원 공급에 문제가 생기거나, 공급이
      갑자기 중단될 때 데이터를 잃을 수 있다는 점이다. 플래시 메모리 블록 크기에 비해서 실제
      로 파일에서 업데이트하려고 하는 부분은 상대적으로 매우 적다는 점을 생각하1 보자. 그리고
      이전에 다룬 내용을 통해서 플래시는 블록 단위로 기록이 되어야 한다는 것을 알고 있다. 그
      렇기 때문에 , 만약 8KB의 작은 파일을 쓰려고 한다면 64KB 또는 128KB 정도의 플래시
      블록 하나를 통째로 치우고 다시 기록해야 한다. 그리고 최악의 경우 기록하는 데 몇 십초가


20) 리얼 타임 클럭 咀[C) 모듈은 보통 비휘빌성 메모리를 조금 가지고 있다. 그리고 시리얼 EEPROM도 적은 양의 데이터를 저장
    하키 위해서 일반적으로 많이 사용되는 비휘발성 메모리이다．
21) （역자주） 에뮬레이트（emulate）는 어떤 기능이나 구조를 본뜨는 것을 의미한다. 시뮬레이트（sim川ate）와 비교해서 의미를 고려해
  보아야 할 단어이다．
 賽 熬1     Embedded Linux Primer




        컬릴 수도 있다. 바로 이 상대적으로 긴 쓰기 동작 과정 중에 전원 공급 문제가 발생할 확률
        이 매우 높아지는 것이다．

        요즘 사용되는 플래시 파일 시스템 중에서 많이 사용되는 것 중에 하나가 JFFS2（저널링22)
        플래시 파일 시스템 2）이다. 이 파일 시스템은 전원 문제가 발생하더라도 데이터 유실을 최
        소화하고, 플래시 수명을 증가시키고, 전체적인 성능을 향상시키기 위한 몇 가지 중요한 기
        능을 가지고 있다. 그리고 최근의 JFFS2 파일 시스템은 발전된 웨어 레벨링 , 정해진 용량의
        플래시 메모리에 압축과 해제를 통해서 좀 더 많은 데이터를 저장할 수 있도록 하는 기술，
        리눅스의 하드 링크23) (hard link）를 지원하는 등 많은 기능이 개선되었다. 좀 더 자세한
        사항은 9장, "파일 시스템"과 10장, "MTD24) 서브시스템"에서 메모리 기술 저장 장치
        (Memory Technology Device) 서브시스템을 다룰 때 살펴보도록 하자．


2.3.5 메모리 공간

        사실 기존의 모든 임베디드 운영체제는 시스템 메모리를 하나의 크고, 넓게 펼쳐진 공간으로
        인식하고 관리했다. 이는 마이크로프로세서의 주소 공간（address space）이 0번치에서부터
        물리적 메모리의 최대 범위까지의 영역으로 이루어진다는 것을 의미한다. 예를 들면, 24개
        의 물리적인 주소 라인（address line）을 가진다면 메모리의 최대 크기는 16MB가 된다. 따
        라서 이 프로세서의 주소 값은 16진수로는 0x00000000부터 0xOOffffff까지가 될 것이
        다. 보통 하드웨어를 디자인할 때 주소 공간의 맨 아랫부분에 DRAM을 위치시키고, 플래시
        메모리는 맨 위쪽에 배치시키는 경우가 많다. 그리고 DRAM과 플래시 메모리 사이의 사용
        하지 않는 빈 공간에 대해서는 다른 주변 장치들이 사용하도록 설계한다. 이러한 디자인에
        대한 결청은 보통 마이크로프로세서가 어떤 종류의 것이냐에 따라서 좌우된다. ［그림 2-5]
        는 간단한 임베디드 시스템의 전형적인 메모리 공간 구조를 나타낸 예이다．




22) （역자주） 저널링 파일 시스템에 대해서는 h由r//en. 岫岫光曲．org加ild乃ournalin且flu已翎stem을 참고하기 H足f다．
23) ［역자주） 리눅스에서 하드링크는 햐니의 파일을 개리키는 파일 경로가 2개 이상이 될 수 있는 기능이다. 즉, 파일은 하니지만，
    파일명은 2개, 37뀨 등이 될 수 있다．
24) （역자주］ 入m）는 플래시 메모리의 한 형태인뎨, 특정한 조건을 갖출 경우 MTD라고 부른다. 해당 조건은 h由3://en. wi帥光dia.
    org/wi닢／Me聊r兄Techn이ogyDe呱：e에서 참조할 수 있다．


166
                                                        임베디드 처음 경험하기   Chapter 2




      FFFF FFFF

                     폴래시 메모리           1\
                                             16MB7a8AI

       FF00 0000

       F000 0000                            주변 장치 베이스 주소
                                      1\
                     PCI 버스 영역              >PCI 주소 범위
       8000 0000                      )

      03FF FFFF


                        DRAM                 64MB RAM

       0000 0000
      I 그림 2-5 전형적인 임베디드 시스템의 메모리 맵（毗跏ry map)


      기존의 운영체제를 사용하는 전통적인 임베디드 시스템에서는 운영체제와 모든 태스크가 시
      스템의 모든 자원에 대해서 동등한 권한을 갖고 있는 경우가 많다. 그래서 하나의 프로세스
      에 존재하는 버그가 자기 자신의 메모리 영역은 물론이고, 운영체제의 영역 또는 다른 태스
      크의 메모리 , 심지어 하드웨어 레지스터까지 임의로 침범할 수 있다. 이러한 접근법의 가장
      큰 장점은 역시 간단함에 있다. 하지만 버그가 발생하기 쉽고, 이러한 버그는 분석하기가 어
      려운 경우가 많다．

      고성능의 마이크로프로세서는 메모리 관리 장치（J 'fl4JJ: Memory 入血nagem이北 Unit）라
      는 복잡한 하드웨어 장치를 내부에 가지고 있는데 , 그 목적은 운영체제가 자신의 주소 공간
      및 프로세스에 할당한 주소 공간에 대해서 고수준의 관리 및 제어를 할 수 있도록 하기 위해
      서이다. 이러한 제어권은 크게 두 가지 형태를 갖는데 , 접근 권한과 메모리 주소 변환이 그것
      이다. 접근 권한은 운영체제가 어떠한 태스크에 대해서 메모리의 각 영역들에 대해서 특정한
      접근 권한25）을 줄 수 있도록 한다. 메모리 주소 변환은 운영체제가 가상의 메모리 공간을
      사용할 수 있도록 하는데 , 이 기능은 아주 많은 장점이 있다．



25) （역자주） 예를 들편 읽기 권한， 쓰기 권한， 실행 권한 등을 생각해 볼 수 있다．


                                                                              67 1
 難 Mu     Embedded Linux Primer




       리눅스 커널은 가상 메모리를 지원하기 위해서 하드웨어 MM1 J의 도움을 받는다. 가상 메모리
        의 가장 큰 장점 중에 하나는 시스템에 실제로 존재하는 메모리보다 더 많은 메모리를 가진
       것처럼 보이게 함으로써 시스템 메모리를 좀 더 효율적으로 사용할 수 있게 한다는 점이다．
       또 한 가지 장점은, 커널이 태스크 및 프로세스에 할당된 시스템 메모리의 각 영역에 대해서
       접근 권한을 설정해서 임의의 프로세스가 무단으로 다른 프로세스나 커널 자신에게 할당된
       메모리 및 시스템 자원에 접근하는 것을 막을 수 있다는 것이다.

       이제 가상 메모리가 어떻게 동작하는치 좀 더 자세히 알아보자. 가상 메모리에 대한 너무 깊
       은설명은 이 책의 범위26）를 벗어난다. 대신에 , 임베디드 시스템 개발자 입장에서 가상 메모
       리 시스템의 큰 줄기에 대해서만 살펴보도록 하자．


2.3.6 실행 컨텍스트
       리눅스가 처음 실행될 때 가장 먼저 하는 일 중에 하나는 프로세서의 메모리 관리 장치
        (MMU）를 구성하고, MMU를 지원하기 위한 자료 구조를 초기화하는 것이다. 그리고는 주
       소 변환 기능을 활성화시킨다. 이 과정이 끝나면 커널은 자신만의 가상 메모리 공간에서 실
       행되게 된다. 최근까지 리눅스 커널의 개발자들은 커널이 존재할 가상 메모리 주소를 디폴트
       로 OxC0000000으로 두고 있다. 하지만 대부분의 아키텍처에서 이 디폴트 주소를 다른
       값27）으로 바꿀 수 있도록 되어 있다. 커널 심볼 테이블을 한번 들여다보면 커널 심볼들이
       0xCO）茯xxxx로 시작하는 메모리 주소로 링크28）되어 있는 것을 볼 수 있다. 결과적으로 커
       널의 어떤 코드가 커널 공간에서 수행되고 있을 때 프로세서의 명령에 주소(instructi아I
       pointer）는 이 영역에 존재하게 된다．

       리눅스에서는 쓰레드29) (thread）가 현재 실행되고 있는 환경 및 영역에 따라 두 가지의 분
       리된 동작 컨텍스트（conte砒）를 가지게 된다. 쓰레드가 완전히 커널 영역 내에서만 실행된
       다면 커널 컨텍스트라고 하고, 응용 프로그램은 사용자 영역 컨텍스트에서 동작한다고 말한다．
       사용자 영역 프로세스는 자신의 메모리 영역에만 접근할 수 있으며 , 파일 및 장치 I/o와 같
       이 접근이 제한된 자원에 접근하기 위해서는 커널이 제공하는 시스템 콜（system call）을 호
       출한다. 예를 하나 들면 이해가 쉬울 것이다．

26) 가상 메모리 시스템을 다룬 책들 중어］ 좋은 책들이 많다. 이 장의 마지막 부분의 2. 5. 1 절의 七1 읽어 보기"를 참고하자．
27) 하지만 굳이 바꿔야 할 마땅한 이유는 별로 없다．
28) （역자주） 여기서 링크는 컴파일된 오브젝트 파일을 링크시키는 의미의 링크다．
29) 여기서 人｝駐   쓰레드라는 용어는 명령어들이 순차적으로 수행되는 것을 지칭한다．


168
                                        임베디드 처음 경험하11   Chapter 2



파일을 하나 열어서 그 내용을 읽끼를 요청하는 간단한 어플리케이션을 쟁각하1 보자（［그림
2-6] 참조）. 파일을 읽기 위해서 C 표준 라이브러리 함수의 read (）를 호출하는데, 함수는
사용자 영역에서부터 시작하지만, read () 함수는 커널에게 파일을 읽어 줄 것을 요청하게
된다. 그 결과 실제 파일의 내용을 읽기 위해서 사용자 영역에서 커널로의 문맥전환
(context sw北ch）이 이루어진다. 커널 내부에서는 읽기 요청을 처리하기 위해서 하드 드라
이브에 접근해서 파일의 내용을 담고 있는 섹터를 요청하게 된다．


                          응용 프로그램
                          李   H  L
                          自라이브러근J
                                    읽기 요청

              리눅스 커널




                        臣）E 하드웨어 인터럽트

          卜
              DE 드라이납

하드 디스크
I 그림 ?6 간단한 파일 읽기 과정


실제로 하드디스크에 읽기를 요청하는 것은 비동기적으로 이루어지는데 여기서 비동기적이
라는 말은, 일단 하드디스크에 어떤 요청을 보내고, 프로세서는 다른 일을 하고 있다가 하드
디스크에서 읽키가 다 끝나서 데이터를 사용할 수 있는 시점에 , 프로세서로 인터럽트를 보내
는 방식을 말한다. 이때 읽기 요청을 한 응용 프로그램은 읽은 데이터를 사용할 수 있을 때까
지 대기 큐（wait queue）에서 정지된 상태를 유지한다. 나중에 읽기 요청한 데이터가 준비
되면 하드디스크가 하드웨어 인터럽트를 발생시키게 된다（이 과정은 설명을 위해서 의도적
으로 단순화한 것이다）. 커널이 하드웨어 인터럽트를 받으면 현재 수행되고 있는 프로세스는
일단 중단시키고, 하드디스크로부터 준비된 데이터를 읽어 온다. 여기까지가 쓰레드가 커널
컨텍스트에서 수행되는 예를 설명한 것이다．



                                                                9
         Embedded Linux Primer




       지금까지 일반적으로 사용자 공간과 커널 공간으로 구분되는 2개의 실행 컨텍스트 영역에
       대해서 알아보았다. 그리고 응용 프로그램이 시스템 콜을 호출하면 그 결과로 컨텍스트 스위
       칭이 이루어지고, 커널로 진입하고, 프로세스의 나머지 절반 영역인 커널 영역에서 코드가
       실행된다. 이러한 부분을 커널 내의 프로세스 컨텍스트라고 부르기도 한다. 이와는 대조적으로
       IDE 드라이브30）를 다루는 인터럽트 서비스 루틴（이하 TSR）은 （다른 TSR도 마찬가치로）
       특정 프로세스에 해당하는 커널 공간에서 실행되지 않는다. 이 실행 컨텍스트 영역은 몇 가
       지 제한 사항이 있는데 , TSR은 절대로 실행중에 다른 프로세스에 의해서 중단되거나 대기
       상태（sleep）로 진입하지 않으며 , 대기 상태를 유발시킬 수 있는 커널 함수의 호출도 금지되
       어 있다. 이 부분에 대한 좀 더 자세한 내용은 이 장 마치막의 2.5.1절 "더 읽어 보기"에 소개
       된 자료를 참고하기 바란다．


2.3.7 프로세스 가상 메모리

       예를 들어 , 사용자가 리눅스 명령에 프롬프트에 'S라는 명령을 치면 'S 프로세스가 하나 생
       성된다. 이때 커널은 이 프로세스를 위한 메모리를 할당하고, 가상 메모리 주소의 범위를 프
       로세스에 부여한다. 이 주소 범위는 커널의 주소는 물론이고 다른 프로세스의 주소 영역과
       전혀 상관이 없다. 또한 프로세스가 보는 가상 메모리 주소와 보드에 존재하는 실제 물리 메
       모리의 주소도 서로 직접적인 관계는 없다. 사실 프로세스는 실행중에 물리 메모리 상의 여
       러 다른 영역들을 사용하거나 해제하게 되는 경우가 흔한데 , 이는 페이징과 스와핑에 의한
       것이다．

       ［리스트 ?4］는 유명한 "Hello World" 예제인데 , 위 주소 개념에 대해서 설명하기 위해서
       약간 수정한 것이다. 이 예제의 목적은 커널이 프로세스에게 할당하는 메모리 주소 영역을
       보여 주기 위한 것이다. 그리고 코드를 2장의 앞부분에서 설명한 AMCC 요세미티 보드에서
       실행시켜 보았다. 이 보드는 256MB의 DRAM을 가지고 있다．

       ［리스트 ?4] Hello World , 임베디드 버전


          #include <stdio. h>


          mnt bss_var;           /"'" 초기화되지 않은 전역 변수 *1




30) （역天H勻 하드 드랴이브


I 70
                                                   임베디드 처음 경험하it         Chapter 2



  mnt data_var = 1;      /'" 초기화된 전역 변수 必／


  mnt main(int argc, char *"*"argv)
  {
      vo化 士stack尸－var;                /"" 스택에 존재하는 지역 변수 ''I

      stack_var = (vo化 了Omai n;       ／央 컴파일러iF 이 부분을 """/
                                      /""' 최적화하지 못하게 할 것． "'"/


      printf ("Hello, 닙orld! Main is executing at %p\n", stack_var) ;
      printf ("This address (%p) is in our stack frame\n", &stack_var) ;


      ／去 BSS 섹션에 초기화되지 않은 전역 변수들이 존재한다． '""/
      printf ("This address (%p) is in our bss section\n", &bss_var) ;

      ／出 데이터 섹션에 초기화된 전역 변수들이 존재한다． '7
      printf ("This address (%p) is in our data section\n", &data_var) ;

      return 0;
  }


그리고 ［리스트 2-5］는 프로그램을 실행했을 때 콘솔에 출력되는 내용이다. 여기서 주의해
서 볼 것은 hello라는 프로세스가 자신이 256M 램의 주소 영역 바로 위의 어딘가에서 수행
되고 있다고 생각한다는 것이다. 또한 스택 주소（0x7ff8ebb0）도 대략 32비트 주소 공간의
중간쯤에 위치하는데 , 보드에 장착된 256MB의 RAM이 커버할 수 있는 주소보다 크다는
것을 알 수 있다. 이게 어떻게 가능할까? DRAM은 이런 시스템에서 보통 연속된 주소 영역
에 분포하도록 되어 있다. 무심코 생각하면 2GB 정도의 DRAM 공간을 사용할 수 있는 것
처럼 보인다. 이러한 가상 메모리 주소는 커널이 할당하고, 내부적으로 요세미티 보드의
256MB 물리 메모리에서 가용한 어딘가를 사용하게 된다．

［리스트 ?5) Hello 출력

  root! amcc: # ./hello
  Hello, world! Main is executing at 0x10000418
  This address (0x7ff8ebb0) is in our stack frame
  This address (0x10010a1c) is in our bss section



                                                                                 71
  沁烈1    Embedded Linux Primer




          ihjs address (0x10010a18) is in our data section
          root@amcc : ,#




       가상 메모리 시스템의 특징 중의 하나는 사용 가능한 물리 메모리가 미리 지정한 임계점 이하
       로 내려가면 커널이 메모리 페이지를 하드디스크와 같은 큰 저장 공간에 스왑（swap）시키게
       된다는 점이다. 커널은 현재 프로세스에 메모리를 할당하기 위해서 , 활성화된 메모리 영역을
       검사해서 최근에 가장 적게 사용된 영역을 찾아낸 후에 , 그 부분을 하드디스크에 기록해서
       사용 가능한 메모리 페이지로 만든다. 하지만 임베디드 시스템에서는 보통 성능 및 자원 제
       한 때문에 디스크로의 스왑 기능은 사용하지 않는다. 예를 들면, 상대적으로 느리고 쓰기 횟
       수도 제한이 있는 플래시 메모리를 스왑용 저장 장치로 이용하는 것은 매우 어리석은 일이다．
       이러한 스왑 장치가 없을 경우는 응용 프로그램을 개발할 때 이러한 메모리 용량 한도 내에서
       동작하는 데 문제가 없도록 설계해야 한다.


2.3.8 교차m개발 환경

       임베디드 시스템을 위한 응용 프로그램이나 디바이스 드라이버를 작성할 때 먼저 필요한 것
       은, 대상 시스템에 맞는 형식의 바이너리 실행 파일을 생성할 수 있도록 하는 일련의 개발
       툴（컴파일러 , 링커 , 유틸리티 등）이다. 독자가 자신의 데스크탑 PC에서 "Hello World"와
       같은 간단한 응용 프로그램을 하나 만든다고 가정해 보자. 코드를 작성한 후에 데스크탑에
       기본적으로 존재하는 컴파일러（구입하거나 다운받아서 설치한 경우도 있을 것이다）를 실행
       해서 실행 파일을 만들 수 있다. 이 실행 파일의 형식은 컴파일이 이루어진 머신31）에서 실행
       되도록 되어 있을 것이다. 이를 자체（native) 컴파일이라고 한다. 즉, 데스크탑의 컴파일러를
       이용해서 바로 그 데스크탑에서 실행될 파일을 생성하는 것이다.

       여기서 자체라는 것이 특정 아키텍처만을 한정해서 말하는 것은 아니다. 즉, 개발중인 타깃
       보드에서 수행되는 툴 체인（toolchain) 32）을 가지고 있다면 타깃 시스템에 맞는 응용 프로
       그램을 타깃 시스템에서 스스로 컴파일할 수 있다. 사실 어떤 보드에서 새로운 커널을 테스
       트하는 가장 좋은 방법 중의 하나는 해당 타깃 안에서 반복적으로 커널을 컴파일해서 테스트
       해 보는 것이다．



31) （역자주） 더 정확히는 프로세서 아키텍처와 운영체제를 모두 포함해야 할 것이다．
32) （역자주） 개발을 위0私a 필요한 일련의 개발 도구 모음을 풀 체인이라고 한다．


I 72
                                                          임베디드 처음 경험하71   Chapter 2



        교차H개발 환경에서 소프트웨어를 개발하기 위해서는 호스트 개발 환경에서 실행되는 컴파
        일러가 이 개발 환경이 존재하는 시스템에 맞는 형식이 아닌 특정 타깃에 맞는 바이너리 실행
        파일을 만들어 낼 수 있어야 한다. 이러한 교차H개발 환경을 이용하는 가장 주된 이유는 제한
        된 시스템 자원（주로 메모리 용량이나 CPU 성능） 때문에 임베디드 시스템 안에서 스스로
       이러한 소프트웨어를 개발하고 컴파일하는 것이 거의 불가능하거나 비실용적이기 때문이다．

        일부 초보 임베디드 개발자들이 이 교차H개발 환경에서 자주 함정에 빠지곤 한다. 주어진 프
        로그램을 컴파일할 때 컴파일러는 컴파일을 성공적으로 마치기 위해서 포함시켜야 하는 헤더
        (include header) 파일과 라이브러리들을 어디서 찾아야 하는지를 알고 있다. 설명을 위해
        서 "Hello World" 프로그램을 다시 보자. 이 예제는 ［리스트 2-4］에서 다시 가져온 것인데，
       다음과 같은 명령으로 컴파일한다．

           gcc -닙all -o hello hello.c

       ［리스트 2-4］에서 헤더 파일 就dio.h를 포함하도록 되어 있는 것을 알 수 있다. 이 파일은
        gcc 명령에 라인에 기술한 hello.c가 존재하는 디렉터리에는 존재하지 않는 파일이다. 그
        럼 어떻게 컴파일러가 이 파일을 찾을 수 있을까7 또한 hello.c에는 prin七f () 함수도 선
        언되어 있지 않다. 그렇기 때문에 hejjo.c를 컴파일할 때 이 심볼에 대해서 주소 값이 해결
        되지 않은 참조33）를 가지게 된다. 그렇다면 어떻게 링커가 링크 시에 이 심볼에 대한 주소
        값을 결정34）할 수 있을까7

        컴파일러는 내부적으로 시스템 헤더 파일을 찾는 디렉터리들의 위치를 기본 값으로 이미 가
       지고 있다. 그래서 헤더 파일을 포함（include）해야 할 때 이 기본 값으로 저장된 디렉터리
        목록 내에서 파일을 찾을 것이다. 이와 비슷한 과정이 외부 심볼인 printf () 를 결정할 때
        도 마찬가지로 친행된다. 링커는 기본적으로 （그 라이브러리（lLibc_ *)를 어디서 찾을지를 알
        고 있다. 다시 말하자면 툴 체인에는 이미 기본 값이 설정되어 있는 상태이다．

        그럼 이제 Powerl毛를 사용하는 임베디드 시스템용 응용 프로그램을 하나 빌드35）한다고
        생각해 보자. 당연히 PowerPC 아키텍처에 호환되는 바이너리 실행 파일을 만들어 낼 수
        있는 교차 컴파일러가 필요할 것이다. 아마 이 교차 컴파일러를 이용해서 이전에 hello.c


33) （역자주） 사실 원문인 Ut止esolved reference라는 용어 자체도 매우 익숙햐다．
34) （역자주） 이는 역시 resolve reference라는 용어에 해당힌다．
35) （역자주） 프로젝트를 컴파일, 링크하는 과정을 빌드（build)한다고 한다．


                                                                                 73
        Embedded Linux Primer




       를 빌드했던 것과 비슷한 명령어를 써 빌드를 할 텐데 , 이때 아마도 응용 프로그램 코드에서
       사용하는 prin七f () 와 같은 함수를 위해서 C 라이브러리를 링크할 때 개발 시스템에 있는
       x86용 표준 C 라이브러리가 하나로 링크될 수도 있다. 물론 그 결과는 일부는 x86용 바이너
       리 , 또 일부는 PowerPC용 바이너리가 혼합되어 있는 엉뚱한 파일일 것이다. 물론 실행되지
       도 않는다．

       이 문제에 대한 해결책은 교차 컴파일러에게 헤더 파일과 타깃에 맞는 라이브러리 파일을 지
       정한위치에서 찾도록지시하는 것이다. 이 부분에 대해서는 12장, "임베디드 개발환경"에서
       좀 더 자세히 살펴볼 것이다. 앞에서 다룬 예제의 목적은 자체（nat如e) 개발 환경에서 개발
       하는 것과 임베디드 시스템을 위한 교차 컴파일 환경의 차이점을 알아보기 위해서이다. 이
       부분이 교차드개발 환경에서 유일하게 복잡한 부분이다. 비슷한 문제와 해결책이 교차 디버깅
       에도 그대로 적용될 수 있다． 교차 디버깅에 대해서는 14장, "커널 디버깅 기출'에서 알아볼
       것이다. 잘 구성된 교차H개발 환경은 성공적인 개발에 있어서 매우 중요하고, 컴파일러 외의
       다양한 도구들을 사용해야 한다. 이 부분도 12장, "임베디드 개발 환경"에서 알아볼 것이다．



2.4 임베디드 리눅스 배포판
       그런데 배포판이라는 것이 정확히 무엇일까2 리눅스는 부팅 후에 , 루트 파일 시스템을 찾아
       서 마운트시키도록 되어 있다. 알맞은 루트 파일 시스템을 마운트한 후에는, 스크립트를 통
       해서 시스템에 필요한 프로그램과 유틸리티들을 실행시킨다. 이 프로그램들은 로그인 쉘을
       실행시키거나 네트워크 인터페이스를 초기화하고, 사용자 어플리케이션을 실행시키는 등의
       특정한 작업을 수행하는 다른 프로그램들을 실행시킨다．이러한 각각의 프로그램을 실행시키
       기 위해서 시스템에 요구되는 사항들이 있다. 예를 들면 대부분의 리눅스 응용 프로그램은
       하나 또는 그 이상의 시스템 라이브러리의 도움을 받는다. 또 다른 프로그램들은 설정 파일
       이나 로그 파일 등을 필요로 한다. 정리하자면 비록 작은 임베디드 리눅스 시스템이라도 루트
       파일 시스템어］ 척절한 구조를 이루고 존재하는 여러 개의 파일을 필요로 한다．

       성능 좋은 테스크탑 시스템은 루트 파일 시스템 내부에 수천 개의 파일을 가치고 있다. 이
       파일들은 기능별로 그룹 지어진 패키지의 형태로 배포된다. 이 패키지는 전형적으로 패키지
       매니저를 통해서 설치 및 관리된다. 레드햇（Redi拓t) 패키지 매니저（rpm）는 리눅스 시스템
       에 패키지를 설치하고 치우거나 업데이트하는 데 많이 사용되는 유명한 프로그램이다. 만약
       독자가 사용하는 시스템이 페도라（Fedora) 코어 시리즈를 포함한 레드햇 기반의 리눅스라


I ''
                                                    임베디드 처음 경험하기   Chapter 2



      면 명령에 프롬프트에 rpm -qa라는 명령을 입력해서 시스템에 설치되어 있는 패키지들을
      검색해 볼 수 있다．

      패키지는 하나 이상의 파일로 구성되는데 , 실제 어떤 패키지는 수백 개의 파일로 구성되기도
      한다. 리눅스 배포판 풀 버전은 수백에서 수천 개에 이르는 패키지를 가지고 있다. 다음 항목
      이 임베디드 리눅스 배포판에서 찾아볼 수 있는 패키지들과 그 목적을 예로 나타낸 것이다．

         口 initscrip七S : 시스템 시작 및 종료를 위한 스크립트를 포함하고 있다．

         口 apache : 유명한 아파치 웹 서버를 담고 있다．

         口 telnet-server : 임베디드 타깃에 텔넷을 통해서 연결할 수 있도록, 텔넷 서버를 구
            동하는 데 필요한 파일들을 포함하고 있다．

         口 glibc : 표준 C 라이브러리

         口 busybox36) : UNIX/Linux 시스템에서 일반적으로 많이 사용되는 커맨드 라인 유틸리
           티들을 축약해서 모아놓은 것


      이렇게 다양한 패키지들이 존재하기 때문에 리눅스 배포판이라는 용어가 만들어지고 사용되
      게 된 것이다. 즉, 전형적인 리눅스 배포판은 유용한 프로그램 , 라이브러리 , 툴, 유틸리티들
      과 문서 등으로 이루어진 몇 장의 CD-ROM 형태로 배포된다. 이 배포판을 설치할 때는 먼
      저 시스템이 온전히 동작하는 데 문제가 없는 합리적인 설치 항목이 기본 값으로 선택되어
      있고, 사용자가 자신의 필요에 따라 선택을 변경할 수 있도록 되어 있다. 독자도 아마 수세
       (Suse）나 레드햇과 같은 유명한 리눅스 배포판의 이름은 꾀 친숙하게 느껴질 것이다．

      하지만 임베디드 타깃을 위한 리눅스 배포판은 몇 가지 중요한 차이점이 있다．. 먼저 , 임베디
       드 배포판 안에 포함된 실행 바이너리들은 PC에서는 실행되지 않고, 임베디드 시스템의 프
       로세서와 아키텍처에서 실행되도록 만들어진 바이너리이다（물론 어떤 임베디드 리눅스 배포
       판이 x86을 타깃으로 한다면 이야기는 달라진다）. 데스크탑을 위한 리눅스 배포판은 전형적
       인 데스크탑 사용자를 위해서 예쁜 디자인의 시계 프로그램이나, 계산기 , 일정 관리 프로그
       램 , 전자메일 프로그램 등의 다양한 GUI 툴을 가치고 있다. 반면 임베디드 리눅스 배포판은
       그러한 요소들은 빼고, 메모리 분석 도구나 원격 디버그 기능 등의 깨발자를 위한 특화된 툴
       들을 가치고 있다．


36) 이 패키지는 하니의 장을 할애할 정도로 중요하다. 11장, "BusyBox"에서 자세히 다루도록 한다．


                                                                           '5 I
  韆 月S       Embedded Linux Primer




          데스크탑과 임베디드 리눅스 배포판의 다른 중대한 차이점은 임베디드 배포판에는 자체
          (native) 개발 툴 대신에 교차H개발 툴들이 포함되어 있다는 것이다. 예를 들면 임베디드
         리눅스 배포판에 포함된 gcc 툴 체인은 x86 데스크탑 PC에서 실행되지만, 대상 임베디드
         타깃 시스템에서 실행되는 바이너리 파일을 만들어 낸다. 툴 체인에 포함된 다른 툴들도 이
         런 식으로 설정되어 있다. 즉, 개발 호스트（보통 x86）에서 실행되지만 ARM이나 Powe叩C
         와 같은 다른 아키텍처를 위한 작업을 수행한다는 것이다.


 2.4. ] 상용 리눅스 배포판

         상업적으로 임베디드 리눅스 배포판을 제공하는 업체가 몇 군데 있다. 선두 업체들은 몇 년 전부
         터 임베디드 리눅스 배포판을 판매하고 있다. 유명한 리눅스 관련 뉴스 및 정보 포털 사이트인
         니nuxdev七es.com에서는 상용으로 판매되는 임베디드 리눅스 배포판에 대해서 포괄적인 리스
         트를 만들었다. 물론 지금은 좀 철 지난37) 자료일 수도 있지만, 살펴보기에는 좋은 자료이
         다. 이 자료는 다음의 주소 http://www.1inuxdevices.com/artic1es/AT9952405558.
         html에서 찾아볼 수 있다．


2.4.2 직접 만드는 리눅스 배포판

         자신이 개발 중인 임베디드 리눅스 프로젝트를 위해서 스스로 필요한 모튼 것들을 직접 조합
         할 수도 있다. 하지만 위험을 감수하고 그런 노력을 들일 만한 가치가 있는지 미리 결정해야
         한다. 만약에 임베디드 리눅스를 즐기는 차원에서 , 즉 취미나 학교 프로젝트로 하는 경우라
         면 괜찮은 접근법일 수도 있다. 하치만, 필요한 모든 툴과 유틸리티들을 조합해서 묶는 과정
         은 상당한 시간이 걸리는 일이고, 또한 이 프로그램들이 서로 동작하는 데 문제가 없는지도
         확인해야 한다．

         독자가 임베디드 개발을 처음 시작한다면 툴 체인이 필요할 것이다. gcc와 binu七uls는
         www. fsf.org나 세계 여러 곳에 있는 다른 미러 사이트에서 구할 수 있다. 이 두 개의 툴
        모두가 커널 및 사용자 영역에사동작하는 어플리케이션 프로젝트를 컴파일하는 데 필요하
        다. 이 툴들은 대부분의 경우 소스 코드 형태로 배포되기 때문에 , 자신의 교차中개발 환경에
        맞도록 직접 컴파일해서 사용해야 한다. 이 툴들의 "안정화된" 최신 소스 코드에 대해서 패치


37) ［역자주） http://www. lin따：devices. corn/al七cles/A17065740528. ht川에서 최신의 내용을 참고할 수 있다. 또한 이 사이트에서
                                                                                                  검
    색을 통해서 더 많은 자료를 찾을 수 있을 것이다．


I 76
                                         임베디드 처음 경험하기   Chapter 2



       를 적용시켜야 하는 경우가 자주 있는데 , 특히 x86/IA32 아키텍처 외의 호스트 환경에서는
       해당 아키텍처에 맞는 패치를 적용해야 한다. 패치는 기본 패키지를 받은 사이트에서 찾을
       수 있을 것이다. 여기서 문제가 있거나 아키텍처가 다를 경우에 , 그 문제 또는 아키텍처에
       맞는 패치를 구하는 것이 해결할 도전 과제가 될 수 있다．



    2.5 요약
       이 장에서는 다앙한 주제에 대해서 대략척으로 살펴보았다. 이 장을 통해서 뒤에 이어지는
       장들에서 다룰 내용을 위한 적절한 시야를 갖게 되었기를 바란다. 이어지는 장을 통해서 앞
       으로의 임베디드 프로젝트를 성공척으로 개발할 수 있도록, 개발 스킬과 기반 지식을 발전시
       켜서 시야를 넓히도록 하자．

         口 임베디드 시스템은 공통된 특징을 갖는다. 자원이 한정된 경우가 많고, 사용자 인터페이
             스가 간단하거나 없으며, 한 가지 특정한 용도를 위해써 만들어진다．

         口 임베디드 시스템에서 부트로더는 매우 중요한 부분이다. 만약 임베디드 시스템을 직접
             설계한 보드에서 개발한다면 부트로더를 개발하는 것도 개발 과정에 포함시켜야 한다．
             보통 기존에 존재하는 부트로더를 포팅하는 경우가 많다．

         口 보드를 부팅시키기 위해서는 부트로더나 커널, 파일 시스템 이미지와 같은 몇 가지 소프
             트웨어 요소가 필요하다．

         口 플래시 메모리는 임베디드 시스템에서 저장 매체로 폭넓게 사용된다. 여기에서 플래시
             메모리의 개념에 대해써 소개했고, 9장과 10장에서 좀 더 상세히 살펴볼 것이다．

         口 프로세스라고도 부르는 응용 프로그램은 커널에 의해써 할당된 가상 메모리 공간 안에서
             실행된다. 응용 프로그램은 사용자 영역에서 실행된다．

         口 임베디드 개발자에게 교차 개발 환경을 알맞게 구성해써 사용할 수 있는 환경을 갖추는
             것이 매우 중요하다. 이 중요한 주제에 대해서는 12장에서 상세히 알아 볼 것이다．

         다 자신이 개발하려는 임베디드 타깃에서 개발을 시작하기 위해서는 임베디드 리눅스 배포
             판이 필요한데 , 임베디드 배포판어臣 해당 아키택처어］ 맞게 컴파일되고 최적화된 여러
             요소들이 포함되어 있다．




1                                                              77
       在a   Embedded Linux Primer




 2.5. ] 더 읽01 보기
            Lin끄x Kernel 工）eve加刃끄旭끄t, 2nd Edition

            Robert Love

            Novell Press, 2005


            라눅스 커널의 아胡(Unders地끄di끄g the 乙j끄口x Kernel)
            Daniel P. Bovet & Marco Cesati / 이호, 심마로 역
            O'Reilly & Associates, Inc., 2002 / 한빛미디어, 2003


            Understa끄di끄gt力e Linux Virtual Mei加ry 兀lanager

            Bruce Perens

            Prentice Hall, 2004




I 78
    이번 쟁게서 배울 내용

      口 독립형   쿠세서

      . 통합형 프로세서 : 시스템 온 칩

      . 하드웨어 플랫폼

      . 요약




1



                             r
  蟹 二I      Embedded Linux Primer




         이번 장에서는 임베디드 시스템에서 사용되는 다양한 종류의 프로세서에 대해서 알아볼 것이
         다. 임베디드 프로세서 시장에서 판매되고 있는 프로세서들과 이들이 가지고 있는 여러 기능
         을 살펴보자. 독립형（Stand-alone) 프로세서를 먼저 알아볼 텐데 , 독립 프로세서는 프로세
         서 자체의 연산 능력은 막강하지만, 완전한 시스템을 위해서 외부에 추가적인 칩셋을 필요로
         한다. 독립형 프로세서를 살펴본 다음에는 리눅스 커널이 지원하는 다양한 통합형 프로세서
         들을 살펴볼 것이다. 마치막으로는 최근 많이 사용되고 있는 범용 표준 하드웨어 플랫폼들에
         대해서 살펴볼 것이다.

         임베디드 시스템을 개발할 때 선택할 수 있는 프로세서는 수십 개에 달할 정도로 다앙하다．
         이번 장에서는 다양한 프로세서 중에서도 메모리 관리 장치（MMU）를 가진 프로세서를 살펴
         볼 텐데 물론 그 중에서도 리눅스가 지원하는 프로세서들만 살펴볼 것이다. 리눅스의 기본적
         인 디자인 관점은 바로 가상 메모리를 지원하는 운영체제1)라는 점이다. MMU를 가치고 있
         지 않은 프로세서에서 동작하는 리눅스도 물론 존재하치만, 이런 프로세서에서 동작하는 리
         눅스 커널은 중요한 구조적인 기능이 하나 누락되어 있는 것이다. 이런 시스템에 대한 내용
         은 이 책에서는 다루지 않을 것이다.



3. ] 독립형 프로세서
         독립형 프로세서는 말 그대로 연산 자체만을 위해서 사용할 수 있는 프로세서를 가리킨다．
         독립형 프로세서는 통합형 프로세서와는 대조적으로 기본 동작을 위해서 추가적인 회로를 필
         요로 한다. 대부분의 경우 이 '추가적인 회로'가 의미하는 것은 DRAM 컨트롤러나, 시스템
         버스 구성 , 키보드나 시리얼 포트와 같은 보조 외부 장치 등을 다루기 위한 칩셋이나, 프로세
         서 주변에 별도로 존재하는 논리 회로를 말한다. 독립형 프로세서는 전반적으로 가장 뛰어난
         CPU 성능을 제공한다．

         임베디드 시스템에서 널리 사용되는 독립형 프로세서는 32비트나 64비트로 구현2）되어 있
         다. 그 중에서도 IBM의 PowerPC 970FX, 인텔의 Pei北ium M, 프리스케일（Freescale)
         의 MPC74x3( 프로세서 등이 있다．



l) 물론 리눅스는 MMU를 가지고 있지 않은 몇몇 프로세서들을 지원하지만, 리눅스의 주류는 MMU를 지원하는 프로세서에서
                                                                     동작
   하는 것이다．
2) 32비트나 64비트는 프로세서가 기본 값으로 사용하는 레지스터나 주소 버스， 실행 명령에 등의 너비 佃idth）를
                                                                     밀한다．


180
                                                        프로세서 가본    Chapter 3



       여기서는 이러한 주요 생산 업체의 독립형 프로세서에 대해서 예를 통해 살펴볼 것이다. 이
       프로세서들은 리눅스가 지원하는 프로세서로, 임베디드 시스템에서 많이 사용된다．


3.1.1 IBM 970FX
       IBM 사의 970FX 프로세서 코어는 64비트를 지원하는 고성능의 독립형 프로세서이다．
       970FX는 슈퍼스칼라（supersc쉐카） 3）구조의 프로세서인데 , 이 말은 이 프로세서가 한 번에 하
       나 이상의 명령어를 불러오고（fetch) , 실행시키고（issuing) , 그 결과를 처리할 수 있다는
       이야기다. 이는 동시에 여러 명령어를 지원할 수 있도록 하는 파이프라인（p如eline) 구조를
       이용하기 때문에 가능한 것이다. IBM 970FX는 내부에 포함된 명령에 스트림4) (stream)
       과 그 기능에 따라서 최대 25단계에 달하는 파이프라이닝 단계를 가지고 있다．

       970FX 프로세서의 몇 가지 핵심 기능은 다음과 같다．

         口 많이 사용되는 아키텍처인 PowerPC의 64비트 버전

         口 고성능의 연산을 필요로 하는 어플리케이션을 위한 깊은 단계의 파이프라인 지원

         口 정적, 동적인 전원 관리 기능

         口 전원 소모를 최소화하고 배터리 수명을 최대한으로 하기 위한 다양한 슬립（sleep) 모드
            지원

         口 저전력 모드를 지원할 수 있도록, 동적으로 속도를 변경할 수 있는 클럭

         口 고성능 및 낮은 지연성(low크atenc功의 저장 장치 관리를 위해1 최적화됨


       IBM 970FX는 IBM 사의 블래이드（Blade)5) 서버를 포함한 많은 고성능 서버 블래이드에
       사용되고 있다．


3.1.2 인텔 펜티엄 卜／1
       인텔의 x86 아키텍처는 32비트, 64비트（좀더 정확히 말하자면 각각 IA32와 IA64이다）를
      지원한다. x86은 가장 많이 사용되는 아키텍처 중의 하나로, 다양한 용도의 임베디드 장치에

3) （역자주］ 슈퍼스칼라 프로세서는 명령에 레벨에서 병렬 처리를 지원하도록 설계된 프로세서를 말한다．
4) （역자주） 명령에 스트림 (S蜘an寸은 하나 이상의 명령에 뭉치를 뜻힌r+.
5) （역자주） 블래이드（Blade）는 칼날， 칼몸을 뜻하는데, 즉 칼 처렴 랙에 여러 개가 찧여 있는 형태의 서버를 말한다. 불필요한 요
   소들을 제거해서 공간 및 젼력 소모를 최소화한다．
   I.      Embedded Linux Primer




        사용되고 있다. 그리고 많은 업체에서 다양한 형태와 크기를 갖는 x86 단일 보드 컴퓨터 시
        스템을 제공하고 있다. 이 장 뒷부분의 3.2절 "통합형 프로세서 : 시스템 온 칩"에서 요즘
        사용되는 범용 표준 플랫폼들에 대해서 좀 더 알아볼 것이다．

        인텔 펜티엄 M은 다양한 랩톱6) 컴퓨터에서 널리 사용되고 있고, 임베디드 제품에 대해서도
        틈새 시장을 갖고 있다. 펜티엄 M 프로세서도 IBM의 970FX 프로세서와 같이 슈퍼스칼라
        아키텍처이다. 다음 항목들은 임베디드 응용 제품에서 매력적으로 작용할 수 있는 펜티엄 M
        프로세서의 기능을 나열한 것이다．

           口 펜티엄 M은 x86 아키텍처에 기반하고 있기 때문에，수많은 소프트웨어，하드웨어 업체
              의 지원을 받을 수 있음

           口 x86 프로세서보다 전류를 덜 소모함

           口 고급 전원 관리 기능을 통해써 저 전력 동작 모드 및 다양한 슬립（sleep) 모드롤 지원

           口 동적으로 클럭 속도를 변경 할 수 있기 때문에, 배터리 동작 시어］ 대기모드 등의 효율을
              개선할 수 있음

           口 칩 내부의 온도 감지 장치를 통해1, 특정 온도 이상에서 자동으로 저전력 상태로 진입함으
              로써 전류 소모를 줄일 수 있음

           口 다양한 동작 속도, 동작 전압을 지원함으로써 이동식 장비의 배터리 사용 시간을 최대화
              하도록 설계됨


        위에서 나열한 사항들은 임베디드 제품을 개발할 때 매우 유용한 기능들이다. 임베디드 시스
        템에서는 이동성을 갖거나 배터리만으로 동작하는 환경이 횬한데 , 펜티엄 M 프로세서는 자
        체적인 전원, 온도 관리 기능을 통해서 이러한 이동성 및 배터리 사용 환경에서 많은 인기를
        누리고 있다．


3.1.3 프리스케일 MPC7448

        프리스케일 MPC7448 프로세서는 4세대 PowerPC라고 알려진, G47）라고 부르는 프로세
        서를 기반으로 하고 있다. 이 고성능의 32비트 프로세서는 주로 네트워크나 전자 통신을 위
        한 용도로 많이 사용된다. 몇몇 업체에서는 산업 표준 하드웨어 플랫폼 명세를 지원하는 블

6) （역자주） 노트북（Notebook) 컴퓨El
7) 프리스케일 문서에서는 이제 G4를 e600 코어라고 부른다．


I 82
                                                     프로세서 기본   Chapter 3



      래이드 서버를 생산하고 있는데 , 이 프로세서 및 비슷한 다른 프리스케일 프로세서를 이용하
      고 있다. 이런 플랫폼에 대해서는 나중에 3.3절 "하드웨어 플랫폼'에서 살펴보자．

      MPC7448은 다음에 나열한 것과 같은 고급 기능들로 인해서 , 신호 처리 및 네트워킹을 위
      한 제품에서 폭넓은 인기를 누렸다．

        口 1.5GHz 이상의 동작 클럭 속도

        口 1MB 내장 L2 캐시

        口 다양한 슬립 모드를 포함한 고급 전원 관리 기능

        口 AltiVec 벡터 연산 장치

        口 저전력 환경을 위한 전압 조절 기능


      MPC7448은 프리스케일의 AltiVec이라는 기술을 지원하는데 , 이 기술은 빠른 알고리즘 연
      산이나, 데이터 크런칭（data寸crunching)8) 어플리케이션을지원하기 위한 것이다. Alt싸ec
      연산 장치는 128비트 너비의 레지스터를 32개나 가지고 있다. 이 AltiVec 레지스터에 들어
      있는 각각의 값이 다중 요소에서 하나의 벡터로 간주된다. AltiVec은 이 벡터 데이터를 병렬
      로 효과적으로 다룰 수 있는 명령에 집합을 정의하고 있다. A出Vec 연산으로는 교차e합
      (sum中across) , 哥합（mu出히少釵im) , 데이터 동시 분산（저장） 및 추출（로드） 명령에 등
      이 있다．

      개발자들은 AltiVec 장치를 신호 처리나 네트워크 처리를 위한 빠른 소프트웨어 연산을 위
      해서 사용했다. 그 예로, 푸리에 변환, 필터링 , MPEG 비디오 코딩 및 디코딩 등의 신호 처
      리나 DES, MD5. SHA1과 같은 암호화 프로토콜을 빠르게 생성하는 것 등을 들 수 있다．

      프리스케일의 다른 단독 프로세서 제품군으로는 MPC7410, MPC7445, MPC7447,
      MPC745x 그리고 MPC7xx 등이 있다．


3.1.4 보조 칩셋
      지금까지 살펴본 독립형 프로세서들은 추가적인 논리 회로, 즉 메인 메모리（DRAM) ,
      ROM, 플래시 메모리 등의 시스템 메모리 장치들이나 PCI 같은 시스템 버스, 키보드, 시리


8) （역자주） 데이터 마이닝과 비슷한 개념으로， 데이터를 작은 단위로 쪼개서 정보를 추출하는 것


                                                                      831
             Embedded Linux Primer




          얼 포트, IDE 인터페이스 등과 같은 기타 외부 주변 장치를 연결하고 사용할 수 있게 해 주
         는 추가적인 회로들이 필요하다. 이런 추가 논리 회로는 별도의 칩셋의 형태로 만들어지는데，
         특별히 특정한 프로세서 계열을 지원하기 위해서 만들어지기도 한다．

         예를 들면, 펜티엄 M은 하나의 보조 칩셋의 도움을 받는데 , 바로 855GM이라는 칩셋이다．
         855GM 칩셋은 주로 그래픽 및 메모리를 위한 인터페이스를 담당하는데 , 그래서 이름에도
         （弧iI）이 붙었다. 855GM은 펜티엄 M을 위해서 최적화된 칩이다. ［그림 3-1］에 펜티엄 M
         에 맞는 하드웨어 디자인에서의 프로세서와 칩셋 간의 관계를 설명하고 있다．



                   프로세서


                       :   ：속전반부버1
                                           DRAM

                노스 브릿지
               (Northbridge)               그래픽




                       :
                                     三
                                           이더넷
                                           （기口1'


                                           USB
                                           USE
               사우스 브릿지
              (Southbridge)                IDE



                       !                   오디오
                                     \\+
                  PCI버스
        I 그림 3녀 프로세서와 칩셋 간의 관겨1


         이 그림에서 사용되고 있는 용어들은 이제는 이런 칩셋들을 설명하는 일반적인 통용어가 되
        었다. 즉, 인텔 855GM 칩셋은 일반척으로 노스 브리지（north bridge）라고 부르는데 , 이 칩셋
        이 프로세서의 고속 전반부 버스（FSB: Front Side Bus）에 바로 연결되기 때문이다. I/o
        및 PCI 버스 연결을 위한 칩셋은 비슷한 방식으로 그 위치 때문에 사우스 브리지（sout比ridge)


9) （역자주） Graphic / Me聊ry


184
                                                             프로세서 가본     Chapter 3



       라고 부른다. 이 하드웨어 아키텍처에서 사우스 브리지 칩（실제로는 I/o 컨트롤러）은 ［그림
       3-1］에서 표시된 것과같이 이더넷 , USB, 오디오, 키보드, 마우스 컨트롤러 등의 인터페이
       스 기능을 제공한다．

       PowerPC를 예로 들면, 툰드라（Tundra) TsierlO 호스트 브리지가 독립 PowerPC 프로
       세서를 지원하는 칩셋이다. TsierlO은 일반적인 독립형 PowerPC 프로세서들을 위한 몇몇
       인터페이스 기능을 제공한다. 이 칩셋은 프리스케일 MPC74xx 계열과 IBM PPC 750xx
       계열의 프로세서를 지원한다. 툰드라 칩셋은 프로세서가 다음에 나열한 보조 장치들과 직접
       연결하기 위해서 사용한다．

          口 DDR10) DRAM, 통합 메모리 컨트롤러

          口 이더넷（툰드라는 기가비트 이더넷도 지원한다）

          口 PCI 익스프레스（2개의 PCI 익스프레스 포트를 지원한다）

          口 Pci/x(PCI 2.3, PCI-X와 콤팩트 PCI [cPCI1)

          口 시리얼 포트

          口 I2C

          口 프로그램 가능한 인터럽트 컨트롤러

          口 패러럴 포트（병렬 포트）


       보조 칩셋을 생산하는 업체는 VIA 테크놀로지 , 마벨恤arvell) , 툰드라, nVidia, 인텔 등
       다앙하다. 마벨과 툰드라는 PowerPC 프로세서를 위한 칩셋을 주로 생산하고, 다른 업체들
       은 인텔 아키텍처를 위한 칩셋을 주로 생산하고 있다. 하드웨어를 설계할 때 다양한 독립형
       프로세서 , 예를 들어 x86, IBM, 프리스케일, PowerPC 등에서 하나를 사용하는 경우에는
       시스템 장치들과 인터페이스를 위한 보조 칩셋을 반드시 사용해야 한다．

       리눅스를 임베디드 운영체제로 리눅스를 사용할 때 얻을 수 있는 장점 중의 하나는 새로운
       칩셋에 대해서 빠른 지원을 받을 수 있다는 것이다. 현재 리눅스는 치금까지 설명한 칩셋은
       물론이고 다른 다앙한 칩셋들도 지원하고 있다. 사용하고자 하는 칩셋에 대한 리눅스 관련
       정보는 리눅스 소스 코드와 구성 유틸리티를 참고하면 될 것이다．


10) ［역자주） Dual Da杻 Iate : DDR은 클럭의 샹승, 하강 에지 모든 경우에 뎨이터를 젼송하기 때문에, 2배 빠르다．


                                                                                851
        Embedded 니nux Primer




3.2 통합형 프로세서 : 시스템 온 칩
       이전 섹션에서는 독립형 프로세서에 대해서 알아보았다. 물론 이런 독립형 프로세서들이 고
       성능 프로세싱 엔진 등 다앙한 용도로 사용되지만, 거의 대다수의 엠베디드 시스템은 몇 가
       지 형태의 통합형 프로세서（또는 시스템 온 칩（SOC)）를 사용한다. 실제 통합형 프로세서를
       선택해야 하는 합당한 이유는 아주 많다. 먼저 시장을 선도하고 있는 몇 가지 통합형 프로세
       서를 알아보고, 각각 그룹별로 특징들을 살펴보도록 하자. 그리고 독립형 프로세서의 경우와
       마찬가지로, 리눅스에서 지원되는 프로세서들만 살펴볼 것이다.

       주로 사용되는 주류 프로세서 아키텍처가 몇 가지 있는데 , 그들 모두 해당 통합 Soc 제품으
       로 생산되고 있다. PowerPC는 전통적으로 다앙한 네트워킹 및 전자 통신에 관련된 임베디
       드 제품군들에서 앞서 나가고 있다. MIPS는 저사양의 일반 사용자용 장치 시장11）에서 두각
       을 나타내고 있다. ARM 은 핸드폰 제품에서 많이 사용된다. 지금 나열한 아키텍처들이 임베
       디드 리눅스 시스템에서 주로 사용되는 대표적인 것들이다. 하지만, 4장, "다른 관점에서 본
       리눅스 커널"에서 설명하고 있듯이 리눅스가 현재 지원하는 하드웨어 아키텍처는 20개가 넘
       는다．


3.2.1 PowerPC
       Powe叩C는 애플, IBM과 모토롤라의 반도체 부분（현재는 분사해서 프리스케일 반도체로
       독립했다） 엔지니어가 디자인한 축약형 명령에 집합 컴퓨터 (RISC : Reduced Instruction
       Set Computer) 방식의 프로세서이다. PowerPC 아키텍처에 대해서는 이 아키텍처를 자
       세히 설명하고 있는 좋은 책들이 많은데 , 3.4.1절 "더 읽어 보기"에 있는 문헌을 참고하기
       바란다.

       Powerl毛 프로세서는 임베디드 시스템의 거의 모든 종류에 대해서 적용된 사례가 있다. 자
       동차, 일반 사용자용 제품, 네트워킹 장치에서부터 가장 큰 형태인 데이터 및 통신용 스위치
       에 이르기까지 Powerl毛는 임베디드 시스템에서 가장 인기 있는 아키텍처 중의 하나이다．
       이러한 대중성 때문에 많은 업체가 PowerPC를 대상으로 하는 일련의 다양한 하드웨어 및
       소프트웨어 솔루션을 제공하고 있다．



11) 이런 판단은 저자가 시장을 관찰한 결과에 따른 개인적인 의견이지 정확한 과학적인 톄이터를 가지고 판단한 것은 아니다．


甘 86
                                                     프로세서 기본    Chapter 3




3 2.2 AMCC PowerPC
      이 책의 뒤에서 예제로 다루는 일부 시스템이 바로 AJv1（兀 PowerPC 440EP 임베디드 프
      로세서를 기반으로 하고 있다. 440EP는 네트워킹 및 통신용 제품에 많이 사용되는 S0C12)
      프로세서이다. 다음 항목들은 440EP의 주요 특징을 나타낸 것이다．

        口 칩에 내장된 DDR SDRAM 컨트롤러

        口 통합된 NAND 플래시 컨트롤러

         口 P（끄 버스 인터페이스 지원

        口 10/100Mbps 이더넷 지원

         口 칩어］ 내장된 USB 2.0 인터페이스

         口 사용자가 설정할 수 있는 4개의 시리얼 포트

         口 두 개의 I2c 컨트롤러

         口 프로그램 가능한 인터럽트 컨트롤러

         口 SPI(Serial Peripheral Interface : 직렬 보조 장치 인터페이스） 컨트롤러

         다 프로그램 가능한 타이머

         口 디버깅을 위한 JTA(} 지원


      이 프로세서는 말 그대로 시스템 온 칩（SOC）이다. ［그림 3-2］는 AIVICC PowerPC
      440EP의 블록 다이어그램13）이다. 외부 메모리 IC와 실제 I/O 장치만 있으면 별도의 인터
      페이스 로직 없이도 이 SOC만으로 온전한 고사양 임베디드 시스템을 만들 수 있다．




12) （역자주） Soc와 통합형 프로세서는 여기서 같은 의미로 섞여 사용된다．
13) （역자주） 하드웨어 내부에 존재하는 모듈, 버스 등의 구성 요소를 이해하기 쉽게 그린 것을 블록 다이어그램이라고 한다．
         Embedded Linux Primer




                                    'ID雋誌《.
                                      3       :t聲듦』
                                                  ：                   i



                                                                             宙＝ 山 H
                                                                                  m니m
                                                                                    ＝ 은m口 Q三무CO
                                                                  1」




                                                                낸드 퓰래시
                                    DDR                          컨트롤러
                                   SD日AM
                                   컨트롤러                          OPB
                                                                Bridge                            SPI（受브j4和
                                    !
                                    1
          b心口0巨
               t


                                              PLB4
         七m二 md스   汕
                          PLB4 128-Bit        X-bar     PLB3 64-Bit
               甘




                       32K 명령어 32K 데이터
                       캐시（패리티 캐시（패리티
                         포함）     포함）

          四               Pow可PC
                                                                                                   10/100
                                                                                                  Ethernet
              JTAG        440 Core
                                              온칩 보조장치 버스（아J
                                                                                                    MAC



                                                                          USB 1.1
                                                                          Ho駁 CUr
                                                                           +PHY



       I 그림 3-2 AMCC PPC 440EP 임베디드 프로세서 (AMCC 제공）


       많은 업체에서 참고용 리퍼런스 하드웨어 플랫폼14）을 제공하는데 , 프로세서 및 다른 하드웨
       어의 기능들을 개발자들에게 알려주기 위한 것이다. 이 책의 뒤에 나오는 예제들은 (14장，
       "커널 디버깅 기술" 그리고 15장, "임베디드 리눅스 어플리케이션 디버깅하기") ［그림 3-2)
       에 있는 440EP를 메인 프로세서로 사용하는 같은 회사의 플랫폼인 AMCC 요세미티 보드
       에서 실행시킨 것이다．

       PowerPC 프로세서를 이용한 통합형 프로세서 제품은 형태가 다양한테 , ［그림 3-2］에서 설
       명한 것처럼 AMCC 440EP와 같은 경우는 다양한 목적의 제품에 사용할 수 있는 충분한
       입출력 인터페이스를 내장하고 있어서 추가 회로가 거의 필요 없다. 또한 이 프로세서는 부
       동 소수점 연산기（FPU）를 내장하고 있기 때문에 , 네트워크 기능이 들어가 있는 이미지 처
       리 시스템이나 산업용 제어장치 , 네트워킹 장비들에 이상적이다．

       AMCC의 PowerPC 제품군에는 두 개의 코어를 이용하는 제품도 몇 가지 포함되어 있다．
       405 코어 시리즈는 이더넷을 포함한 모델과 포함하지 않은 모텔이 있다. 모든 405 모델은
       SDR사vi 컨트롤러 , 시리얼 포트를 위한 UART , 저수준 제어 통신을 위한 I2C , 범용 I/o

14) C역자주） 데모 보드라고 생각할 수 있다．


  88
                                                          프로세서 기본    Chapter 3



(GPIO) 핀들 그리고 타이머를 내장하고 있다. AMCC 405는 FPU를 필요로 하지 않는 다
앙한 제품에서 사용할 수 있는 가격 대비 성능이 우수한 통합형 프로세서이다．

다른 모델인 AMCC 440 프로세서 제품은 성능 및 보조 장치를 개선한 것이다. 그 중에서
440EP는 하드웨어 부동 소수점 연산 장치（FPU）를 가지고 있고, 440GX는 （기존의
10/100入/1bps 포트 외에도） 2개의 10/100/1000MB 이더넷 인터페이스를 지원한다. 또한
고성능의 네트워킹 제품을 위해서 TCP/H) 하드웨어 가속 장치를 가지고 있다. 440SP는
R싸）5/6을 지원하는 하드웨어 모듈을 추가한 것이다. 여기서 말한 모든 프로세서는 리눅
스에서 잘 지원되는 프로세서들이다. ［표 3-1］은 AMCC 405xx 계열 프로세서를 정리한
것이다．

［표 3-1] AMCC PowerPC 405xx 계열 요약

 특징                 405（갸극          405EP         4［巧GP         405GF누

 코에속도               PowerPC 405     PowerPC 405   PowerPC 405   PowerPC 405

                    133-266MHz      133-333MHz    133-266MHz    266-400MHz

 DRAM 컨트롤러          SDRAM/133       SDRAM/133     SDRAM/133     SDRAM/133

 이더넷 10/100          x              2             1             ]

 GPIC) 핀수           23              32            24            24

 UART               2               2             2             2

 DMA 컨트롤러           4채널             4채널           4채널           4채널

 Ic 컨트롤러            (:)             (:)           O             O

 P（긔 호스트 컨트롤러        x              O             O             O

 인터럽트 컨트롤러          (D              O             O             O

 자세한 내용은 AMCC 웹사이트 www. aiX工. corn允rn娩dded 참조



［표 3-2］는 AMCC 440均
                 （계열의 특징을 나타낸 표이다．




                                                                            89 1
   難U     Embedded Linux Primer




       ［표 3-2J AMCC PowerPC 440xx 주요 사항

        특징                        440EP        440GP         440GX         440SP

        코어／속도                     Pow아미二 440   Power다二 440   PowerPC 440   PowerPC 440

                                  333-667MHz   400-500MHz    533-800MHz    533-667MHz

        DRAM 컨트롤러                 DD日          DDR           DDR           DDR

        이더넷 ]0/100                2            2             2             기가비트 이더넷

        기가비트 이더넷                  x            x             2             1

        GPI0 핀수                   64           32            32            32

        UART                      4            2             2             3

        DMA 컨트롤러                  4채널          4채널           4채널           3채널

         2（二 컨트롤러                 2            2             2             2

        P（긔 호스트 컨트롤괴              (S           PC卜x          P（긔－X         PC卜X3개

        S미 컨트롤러                   (S           x             x             x

        인터럽트 컨트롤러                 (5           O             O             O



3.2.3 프리스케일 PowerPC
        프리스케일 반도체는 주변 장치 (per如heral)들을 통합한 다양한 종류의 PowerPC Soc 프
        로세서 제품군을 가지고 있다. 현재 이 회사는 PowerPC 제품 수직 시장15）에서 시장 규모
        가 큰 3가지 분야에 집중해서 포트폴리오를 홍보하고 있다. 프리스케일의 PowerPC는 네트
        워크 시장 분야에서 엄청난 성공을 거뒀는데 , 프로세서 제품군이 저가용 장비부터 고가형 제
        품까지의 매우 다양한 네트워크 장비에 대헤서 폭넓은 호소력을 가지기 때문이다．

        프리스케일 반도체는 2005년도 언론 보도를 통해16) 2억 개 이상의 통신용 통합 프로세서를
        출하했다고 밝혔다. 이리한 성공적인 실적의 일부는 이 회사의 PowerQUICC 제품군에 의

15) C역자주그 수직 시장이란 비슷한 방법으로 제품이나 서비스를 개발햐는 산업이나 그룹을 말한다．
16) 프리스케일 社의 홈폐아지에서 Media Center 메뉴를 찾은 후어］ Press Release로 들어가자. 거기서 2005년도 10월 31일자 텍사스
  주 오스틴에서 발행된 기사를 보기 닙足｝다．


190
                                                        프로세서 기본   Chapter 3



         한 것이다. PowerQUICC 아키텍처를 이용한 제품은 10년 이상 계속 판매되었는테 , 이 제
         품은 Powerl毛를 기반으로 하고, 거기에 QUICC 엔진이 통합된 것이다（프리스케일 사 내
         부에서는통신 프로세서 모듈, CPM'7）이라고부르기도 한다）. QUICC 엔진은 주프로세서
         인 PowerPC 대신에 스스로 통신 처리만을 전담하기 위해 만들어진 독립된 RISC 프로세서
         이다. 그래서 PowerPC 코어 자체는 통신 처리를 벗어나서 , 컨트롤 및 관리 작업에 집중하
         도록 한 것이다. QUICC 엔진은 복잡하지만, 매우 유연한 통신용 주변 장치 컨트롤러이다．

         현재의 PowerQUICC 칩은 4개의 일반 제품군으로 나뉘는데 , 우선 편의를 위해서 이후부터
         는 PowerQUICC를 그냥 PQ로 줄여서 사용하도록 하겠다．

         먼저 PQI 계열은 기존 PowerPC 기반의 PowerQUICC 제품이며 , MPC8xx 계열의 프로
         세서들이 바로 PQ I 프로제서들이다. 이 통신용 통합 프로세서군은 50MHz에서 13318)
         MHz에서 통작하며 내장된 PowerPC 8刃
                                 （코어에 의해서 동작된다. PQ I 계열은 A까/1이
         나 가정 및 작은 사무실용（S아｛0) 라우터 등의 이더넷 주변 장치 , 주택용 게이트웨이，
         ASDL 및 케이블 모뎀 또는 그와 비슷한 제품들에서 사용된다．

         CPM 또는 QUICC 엔진은 두 개의 강력하고 독특한 통신 컨트롤러를 포함하고 있다. 그
         중에서 시리얼 통신 컨트롤러（SCC r Serial Communication Controller）는 이더넷，
         HDLC/SDLC, AppleTalk , 동기 및 비동기 UART, IrDA, 기타 비트 스트림 데이터 등을
         포함하는 많은 수의 직렬 통신 프로토콜을 구현할 수 있는 유연한 인터페이스이다．

         그리고 시리얼 매니지먼트 컨트롤러（SMC : Serial 八/lanagement Coi血oller）는 ISDN,
         시리얼 UART, SPI 프로토콜 등의 시리얼 통신을 사용할 수 있도록 해 주는 모듈이다．

         이런 SCC와 SCM을 결합하면 매우 유연한 통신 장비를 만들 수 있고, 내장된 시분할 멀티
         플렉서（mult如lexer）는 Ti이나 El 통신과 같은 채널 기반 통신을 구현할 수 있도록 해
         준다．

         ［표 3-3］은 PQI 제품군의 일부를 요약한 것이다．




17) （역자주） CPM : Communication 까ocessor 入4odule
18) （역자주） 클럭의 단위 1M地는 시스템이 동작하기 위한 펄스가 I초당 100만 번 발생하는 것이다．


                                                                         91 1
   ? 礪1     Embedded Linux Primer



          ［표 3-3] 프리스케일 PowerQUICC I 주요 사항

           특징                       MPC850        MPC8S0        MPC875        P마X沼85

           코어／속도                    PowerPC 8xx   PowerPC 8xx   PowerPC 8xx   PowerPC 8xx

                                    최대 80MHz      최대 80MHz      최대 133MHz     최대 ]33MHz
           DRAM 컨트롤러                O             O             O             O
           USB                      O             x             O             O

           S디 컨트롤러                  (3            O             O             O

           I2) 컨트롤러                 O             O             O             O
           SCC 컨트롤러                 2             4             ]             3
           SMC 컨트롤러                 2             2             1             2
           보안 모듈                    x             x             O             O

           자체 고속 이더넷 컨트롤러           x             x             2             2


          다음으로 PowerQUICC II를 살펴보자. PQ II는 603e 임베디드 Powerl毛 코어를 계승한
          프리스케일의 G2 PowerPC 코어를 사용한다. 이들 SOC 통신 프로세서는 133-450MHz
          에서 동작하고, 제공되는 다양한 기능 중에는 하나 이상의 10/100Mbps 이더넷 인터페이스
          와 보안 모듈 및 ATM, PCI 지원 등이 있다. MPC82xx라는 명칭의 제품들이 PQ II 프로
          세서이다．

          PQ II는 기존 QUICC 엔진에 2개의 새로운 컨트롤러를 추가한 것이다. 먼저 FCC는 양방
          향 고속 시리얼 통신 컨트롤러이다. FCC는 100Mbps 이더넷이나 45Mbps어］ 달하는
          T3/E3와 같은 고속 통신을 지원한다. MCC는 128KB x 64KB의 채널화된 데이터를 처리
          할 수 있는 다채널 컨트롤러이다．

       ［표 3-4］는 PowerQUICC II 프로세서 중에서 일부를 요약한 것이다．




I 92
                                                                    프로세서 기본    Chapter 3



        ［표 3-4) 프리스케일 PowerQUlCC II 주요 사항

          특징                MPC8250          MPC8260      MPC8272         MPC8280

         코에속도               G2/603e          O2/603e      G2/603e         G2/603e

                            150-200MHz       100-300MHz   266-400MHz      266-400MHz

          DRAM 컨트롤러         (D               （그           (D              O

          USB               x                 x           o               S（兀4를 통해

          SF:기 컨트롤러         O                O            O               O

          2（二 컨트롤러          O                O            O               （그

          SC（二 컨트롤러         4                4            3               4

          SM（二 컨트롤러         2                2            2               2

          FCC 컨트롤러          3                3            2               3

         MO0 컨트롤러           ]                2            0               2


        PowerPC e300 코어 (G2/603e에서 발전한 것이다）에 기반을 둔 PowerQUl(兀 II Pro는
        266-667MHz에서 동작하며 기가비트 이더넷 , DDR SDRAM 컨트롤러 , PCI , 하이스피
        드（HighSpeed) USB19) , 보안 가속 등의 기능을 갖고 있다. MPC83xx 계열이 PQ II Pro
        프로세서이다．

        PQ II와 PQ II Pro 계열 프로세서들은 LAN 및 WAt寸 스위치 , 허브나 게이트웨이 , PBX
        시스템 그리고 기타 복잡하고 고성능을 요구하는 시스템 등에서 폭넓게 사용되었다．

        PowerQUICC II Pro 제품군에는 QUICC 엔진이 빠진 모델이 3개 , 새로운 QUICC 엔진
        이 들어간 모델이 두 7뀨 있다. MPC8358E와 MPC8360E는 다양한 프로토콜을 지원하는
        새로운 UCC (Universal Communications Controller）가 추가된 모델이다．

        ［표 3-5］는 PQ II Pro 계열의 몇 가치 모델을 요약한 것이다．




19) （역자주） USB의 속도는 High Speed / Full Sj羌ed 2가지로 나뉜다．


                                                                                      93 I
             Embedded Linux Primer




         ［표 3-5] 프리스케일 Power（그UICC II Pro 주요 사항

           특징                        MPC8343E     MPO8347E     MPC8349E     MPC8360E

           코어／속도                     e300         e300         e300         e300

                                     266-400MHz   266-667MHz   400-667MHz   266-667MHz

                                     （그           O            O            O
           DRAM 컨트롤러
                                     DDR          DDR          DO日          DD日

           USB                       O            2            2            O

           S미 컨트롤러                   O            O            O            O

           12O 컨트롤러                  2            2            2            2

           이더넷 ]0/100/1000           2            2            2            UCO를 통해

           UART                      2            2            2            2

           P() 컨트롤러                  D            O            O            O

           보안 모듈                     O            O            O            O

           MOO                       0            0            0            1

           UCC                       0            0            0            8


         PowerQIJICC 제품군의 최상위 계열은 PQ III 프로세서군이다. 이 프로세서들은
         600MHz에서 1.5GHz 사이에 동작한다. e500 코어에 기반하고 있으며 키가비트 이더넷，
         DDR SDRAM, Rapi(끄O20), PCI, PCI/X, ATM, HDLC2') 등을지원한다. MPC85xx
         계열이 PQ III 프로세서이다. 이 프로세서들은 무선 기지국 장비 , 광통신 스위치 , 사무용
         중앙 스위치 , 기타 비슷한 장치들과 같은 하이엔드 급의 제품에 활용할 수 있다．

         ［표 3-6］은 PQ III 계열의 모델 중에서 일부를 요약한 것이다．




20) （역자주） R叩idl0는 보드 상에서 칩 간의 고성능, 패킷 방식의 상호 연결 규격이다．
21) （역天阡） 나gh-Level Data Link Contr아


I 9'
                                                프로세서 기본      Chapter 3



   ［표 3-6) 프리스케일 Po넥erQ내CC III 주요 사황

    특징           MPC8540     MPC8548E    MPC8555E     MPC8560

    코어／속도        e500        e500        e500         e500

                 최대 1.0GHz   최대 1.5GHz   최대 ] .0GHz   최대 ] .0GHz

                 O           O           O            O
    DRAM 컨트롤러
                 DDR         DDR         DDR          DDR

    USB          x           x           Soc를 통해      x

    si:기 컨트롤러    x           x           （그           O

    12O 컨트롤러     O           O           O            O

    이더넷 ]0/100   ]           기가비트 이더넷    Soc를 통해      Soc를 통해

    기가비트 이더넷     2           4           2            2

    UART         2           2           2            SOO를 통해

    P（긔 컨트롤러     Pci/P（긔苡    PC까兀卜x      p（긔          P（긔／PC卜x

    Rapid 1O     O           O           x            O

    보안 모듈        x           O           O            x

    SOc                                  3            4

    Fcc                                  2            3

    SM（二                                 2            0

    M（二（二                                0            2



3.2A M下S
    아마 독자들 중의 일부는 入4IPS 아키텍처에 기반한 32비트 프로세서가 20년 전부터 계속
    생산되어 왔디는 사실을 알면 놀랄 것이다. 八4IPS 아키텍처는 1981년에 미국 스탠포드 대
    학의 존 헤네시（John Hennessey) 박사의 연구팀에 의해서 디자인되었는데 , 나중에 헤네
    시 박사는 入/IIPS 컴퓨터 시스템즈를 설립했다. 이 회사가 현재의 入/IIPS 테크놀로지스
    (MIPS Techn이ogles）가 되었고, 현재 이 회사는 MIPS 아키텍처와 코어의 디자인 및 라
    이선스 관리를 맡고 있다．

                                                                    95
    U        Embedded Linux Primer




         ｝皿PS 코어는 많은 회사에 라이선스되었는데 , 그중 일부 성공한 회사는 임베디드 프로세서 시
          장의 공룡이 되었다. M叩S는 다양한 인기 제품들에 사용되는 RISC(Reduced Instruction
          Set Computing : 축약형 명령에 집합 컴퓨터） 프로세서로서 32비트와 64비트 버전이 있다．
          MIPS 프로세서를 사용하는 제품에는 고급형 하이엔드 장치부터 일반 사용자용 기기까지 다
          앙하다. MIPS 프로세서가 소니의 HD 텔레비젼 제품들, 링크시스（Linksys）의 무선 공유
          기 그리고 소니 플레이스테이션 2(Sony PlayStation 2) 게임기 등 유명한 사용자용 기
          기22）들에도 사용된 것은 잘 알려진 사실이다．

         MIPS 웹사이트에서는 현재 MIPS 프로세서를 사용해 제품을 생산하는 73개 업체 목록23)
          을 확인할 수 있다. 그 중에는 소니 , 텍사스 인스트루먼츠（Texas Instruments) , 시스코
          Scientific Atlanta（케이블TV셋톱 박스선두 업쩨）, 모토롤라등의 몇몇 익숙한 이름들이
          보인다. 거기서도 가장 크고 성공한 회사 중의 하나가 브로드컴 (Broadcom Corporation)
          이다．


3.2.5 브로드컴 M下S
          브로드컴은 케이블 TV용 셋탑 박스, 케이블 모뎀, HDTV, 무선 네트워크 장비 , 기가비트
          이더넷, VoIl）四oice over IP) 시장에서 선두를 지키고 있는 SOC 솔루션 공급 업체이다．
          브로드컴의 SOC 칩들은 이들 시장에서 아주 인기가 많다. 이전에도 말했듯이 우리가 몰라서
          그렇지 집안에 리눅스로 구동되는 장치들이 있을 수 있는데 , 만약 있다면 아마 브로드컴의
          MIPS 기반 SOC로 구동되는 시스템일 확률이 높다.

          브로드컴은 2000년에 얹Byte 사를 인수했는데 , 그 결과 현재 브로드컴이 판매하고 있는 통
         신용 프로세서 제품군이 탄생하게 되었다. 이 통신용 프로세서들은 현재 단일 코어佃ingle
          core) , 듀얼 코어（dual-core) , 쿼드 코어24) (qua于core) 제품으로 나뉜다. 그리고 아직도
          이들 프로세서를 曲Byte 프로세서라 부르고 있다．

          단일 코어 얹Byte 프로세서에는 BCM1122와 BCM1125H가 있는데 , 모두 MIPS64 코어
          기반이며 , 클럭 속도 400 -900MHz로 동작한다. 그리고 프로세서 내부에 DDR SDRAM
          컨트롤러 , 10/100Mbps 이더넷, PCI 호스트 컨트롤러를 가지고 있다. 그리고 두 프로세서

22) 참고 : h啣://WVnV. mips. corn/new寸events/newsroom/inde兄C血?i=1385
23) （역자주） 이 책이 번역되는 시점에 확인한 결과 역시 73개의 업체가 나열되어 있었다．
24) （역자주） 듀얼, 쿼드 코어는 각각 27긔I, 4개의 코어를 칩 안에 내장해서 사용하는 멀티프로세서 구성이다．


I 96
                                                  프로세서 기본     Chapter 3



모두 SMBus 시리얼 설정 인터페이스, PCMCIA, 시리얼 포트를 위한 두 개의 UART를
가지고 있다. BC入I1125H는 10/100/1000Mbps 이더넷 컨트롤러도 가지고 있다. 또 한
가지 놀라운 특징은 전력 낭비가 엄청나다는 점인데 , 두 칩 모두 400MHz에서 동작할 때
전력이 4와트나 소모된다．

듀얼 코어 駐Byte 프로세서로는 BCM1250, BCM1255, BCM1280이 있다. 이 칩들도
MIPS64 코어 기반이며 , 60아vlhz (BCM1250）에서부터 아주 높은 1.2GHz(BCM1255,
BCM1280）까지 동작한다. 이 듀얼 코어 프로세서들은 내부에 DDR SDRAM 컨트롤러 , 다
양한 조합의 기가비트 이더넷 컨트롤러 , 64비트 PCI求 인터페이스, SMBus, PCMCIA,
여러 개의 UA}玎 인터폐이스 등의 보조 컨트롤러들을 내장하고 있다. 사촌 격인 단일 코어
프로세서와같이 , 이 듀얼 코어 프로세서들도 엄청난전류를소모하는데 , 한 예로 BCM1255
는 1GHz 동작 속도에서 13와트의 전력을 소모한다．

쿼드 코어 駁Byte 프로세서에는 BCM1455. BCM1480 통신 프로세서가 있는데 , 다른
曲Byte 프로세서와 마찬가지로, MIPS64 코어를 기반으로 하고 있다. 동작 속도는
800MHz에서부터 1.2GH洲 이른다. 이 SOC들은 DDR SDRAM 컨트롤러 , 4개의 기가
비트 이더넷 MAC 컨트롤러 , 64비트 PCI承 호스트 컨트롤러 및 SMBus, PCMCIA, 4개
의 UART를 가지고 있다．

［표 3-7］은 브로드컴의 얹Byte 프로세서들을 요약한 것이다．

［표 3-7] 브로드컴 미Byte 프로세서 주요 사항

 특징            BCM1125H     BOM1250        BOM1280        BCM1480

 코에속도          SB-]         듀얼 SB-i        듀얼 SB녀         쿼드 SB-i

               卜川PS64       卜川PS64         MIPS64         M甲S64

               400-900MHz   600-i 000MHz   800-i 200MHz   800-i 200MHz

               0            0              0              0
 DRAM 컨트롤러
               DDR          DDR            DDE극           DD日

 시리얼 인터페이스     2-55Mb口s     2-55Mbps       UART 4개        UA日T4개

 SMBus 인터페이스   2            2              2              2




                                                                     97
 鞋U       Embedded Linux Primer




        특징                        BCN川］25H            BCM1250        BCM1280          BC卜川480

        PCMCIA                    a                   C              O                O

        기가비트
        이더넷（10/100/1000           2                   3              4                4
        Mbps)

        PC) 컨트롤러                  (D                  O              O PCI/P（긔．)(     OP（긔／P（斗x

        보안 모듈                     x                   x              x

        네9作속도
                                  1                   1              3                3
        I/O(HyperTransport)



3.2.6 AMD MIPS
       AMD(Advanced Micro Devices) 역시 임베디드 MIPS 프로세서 시장에서 중요한 역할을
       하고 있다. AMD는 2002년 인수한 앨커미25) 반도체（Alchemy Semiconduc切r）를 통해
       서 MIPS32 코어 및 아키텍처 기반의 단일 칩 통합 SOC를 갖게 되었다. AMD의 앨커미
       제품군은 많이 애용되는 M1P532 코어에 기반한 것이다. 이 프로세서들은 모두 상대적으로
       낮은 전력 소모와 높은 완보드（onboard) 시스템 통합성을 가지는 것이 특징이다．

       Au1000과 Au1100은 266-500MHz의 클럭 속도에서 동작하며 , 모두 SDR帥/1 컨트롤
       러 , 플래시 및 PCMCIA 등의 외부 장치를 연결하기 위한 독립된 버스 컨트롤러를 가치고
       있다. ［표 3-8］은 현재의 앨커미 제품군을 요약한 것이다．

       ［표 3-8] AMD 앨커미 卜川PS 주요 사항

        특징'               Au1000             Au1100         Au1200       加1500            Au15攷

        코에속도             卜川PS32              卜川PS32         h川PS32       1네PS32           卜川PS32

                          266-500MHz         333-500MHz     333-500MHz   333-500MHz       333-500MHz

        마祖M                                                 DDR                           DDR
                          SDRAM              SDRAM                       SDRAM
        컨트롤러                                                SDRAM                         SDRAM



25) （역자주） 연금술을 뜻힌디．


I 98
                                                            프로세서 기본       Chapter 3




     특징'          Au1000       Au1100      Au1200       A1鼠）0         Au15攷）

     이더넷 l아］00    2            ]                        2             2

     GPI0 라인      32           48          48           39            43

     UART         4            3           2            2             3


     USB1.1       磊： t：I
                      IuF。
                        訌 USB2.0                            Iu。I
                                                                      추人드 +

                                                                      디바이스

     AC-97 오디오    4            ]           SF（澤 통해1     j             SF0를 통해
     I2S 컨트롤러     l            ]           SF（澤 통해                    SF0를 통해
     SD／卜川너（:;     x           2           2            x             x

     ' 다른 보소 장치로는 IrDA 컨트롤급1, LCD 컨트롤러, 2/4 SPC, 전원 관리 모듈, DMA 엔진, RfC, 카메라 인터폐
       이스， 하드웨어 가속 으垣／복호 모듈, PCI 호스트 컨트롤러, 보안 모듈 엔진 등＜기 있다．




3.2.7 기타 M下S
    이전에도 말했지만 현재 거의 100여 개에 달하는 업체가 MIPS 라이선스를 갖고 있고，
    MIPS 테크놀로지스 라이선스 웹 페이지 www.mips.com/cust이Tiers/licensees／에서
    그 목록을 볼 수 있다. 불행히도 여기서 모든 내용을 다 설명하는 것은 불가능하고, 대신에
    MIPS 테크놀로지스 웹사이트를 통해서 관심 있는 업체를 한번 찾아보고 조사해 보기 바
    란다．

    예를 들어 , ATI 테크놀로지스는 이 회사의 질레온（x皿eon) 셋톱 박스용 프로세서 제품군
    에 MIPS 코어를 사용한다. 캐비엄 네트워크（Cavium Networks）의 옥테온（Octeon) 프
    로세서의 다양한 멀티프로세서 제품에도 MIPS64 코어가 사용된다. IDT(Integrated
    Device Technology）는 인터프라이즈(Interprise）라 불리는 入illPS 아키텍처 기반의 통
    신 프로세서 제품군을 가지고 있다. PMC-시에라, NEC, 도시바 등의 업체도 MIPS에 기
    반한 프로세서들을 갖고 있다. 여기서 설명한 프로세서들 모두 리눅스에서 잘 지원되는 프
    로세서들이다．




                                                                                 991
   蘿U     Embedded Linux Primer




3.2.8 ARM
        A}弧4 아키텍처는 사용자용 전자 제품 시장에서 높은 점유율을 차지하고 있다. 많은 인기 제
        품 및 유비쿼터스 제품들이 ARM 아키텍처를 내장하고 있다. 잘 알려진 제품들로는 소니
        PsP（플레이스테이션 포터블）와 애플 아이파드(iPod) 나노, 닌텐도 게임보이 마이크로, 닌
        텐도 DS, TomTom GO 300 네비게이션 그리고 임베디드 리눅스로 동작하는 모토로라의
        E680i 핸드폰 등이 있다. ARM 사의 웹페이지 www. arm.com/miscPDFs/3822.pdf에
        있는 설명 기사에 따르면 ARM 코어를 내장한 프로세서들이 세계 핸드폰 프로세서 시장에서
        주류를 형성하고 있다．

        ARM 아키텍처는 ARM 홀딩스（ARM Holdings）에 의해서 개발되었고, 세계 여러 반도체
        업체에 라이선스되었다. 세계적인 메이저 반도체 업체들은 ARM의 설계 기술을 라이선스 받
        아서 가치고 있으며 , ARM 프로세서를 내장한 통합 프로세서를 개발해서 판매하고 있다．


3.2.9 TI ARM
        텍사스 인스투르먼츠는 자사의 OMAP 통합 프로세서 제품군에 ARM 코어를 사용한다. 이
        들 프로세저는 다양한 제품들, 예를 들어 핸드폰, PDA, 기타 비슷한 멀티미디어 제품들을
        위한 단일 칩 솔루션을 제공하기 위해서 다양한 보조 장치들을 내장하고 있다. UART, I2C
        등과 같이 통합형 프로세서에 일반적으로 포함되어 있는 인터페이스 외에도 다음과 같이 다
        양한 특수 목적의 인터페이스들을 내장하고 있다．

          口 L（刃 화면 및 백라이트 컨트롤러

          口 버저（Buzzer) 드라이버

          口 카메라 인터페이스

          口 MMC/SD 카드 컨트롤러

          口 배터리 관리 장치

          口 USB 호스트／클라이언트 인터페이스

          口 라디오 모뎀 인터페이스 로직

          口 내장 2D, 3D 가속기

          口 내장 보안 가속 모듈


I 100
                                                                      프로세서 기본    Chapter 3



             口 斗Video 출력

             口 IrDA 컨트롤러

             口 TV(PAL/NTSC）에 직접 출력하기 위한 DAC2이

             口 비디오 및 오디오 처리를 위한 내장 DSP


         많은 인기 핸드폰 및 PDA 제품에서 TI27) Q4Jp 플랫폼이 사용되었다. 이 프로세서들은
         Al祉4 기반이기 때문에 현재 리눅스에서 지원된다. ［표 3-9］는 최근의 TI 아4AP 제품군을
         비교한 것이다．

         ［표 3-9) TI ARM OMAP 주요 사항

           특징                     OMAP1710     OMAP2420       OMAP2430      OMAP3430

                                                                            A딕卜/1 Cortex
           코어／속도                  ARM926 TEJ   ARM11          AR卜川］36
                                                                            A8

                                  최U 200MHz    330MHz         330MHz        550MHz

           DRAM 컨트롤러              0            O              （그            0

           UART                   O            O              0

                                  클라이언트 +      클라이언트 +        클라이언트 +
           USB
                                  市人三          추人E三           추人E三


           I (; 컨트롤러              O            O              O

           MMC-SD 인터페이스           (J           O              O             O

           키패드 컨트롤러               ()           O              O             O

           카메라 인터페이스              ()           0              O             O

           그래픽 가속기                20           20/3D          2D/30         O

           내장 DSP                 TM320C55x    TM320O55x      x             x




26) （역자주） DAC (Digital-Analog Converter) : 디지털 신호를 아날로그 신호로 변경하는 장치
27) ［역天阡） Texas Ins甘uments Corp
         Embedded Linux Primer




       특징                        아4AF거710   OM사뀐420         OM사끄430         0MAP3430

                                            Imaging Video   Imaging Video   Imaging Video
       비디오 가속71                  x
                                            7속기(IVA)        7陰기(IVA 2)      7陰기(IVA 2+)

       보안 가속기                    O          O               O               （그

       오디오 코덱 지원                 O          O               O               O

       블루투스 & RF 모뎀
                                 O          O               O               O
       지원 인터페이스

       LCD 컨트롤러                  O          O               O               O

                                            PA나NTSC         PA나NTSC         PA나NTS（二
       디스플레이 컨트롤러
                                            VGA/QVGA        VGA/QVGA        QVGA/XGA



3.2.10 프리스케일 ARJ너

      임베디드 분야를 선두하고 있는 업체들이 경쟁적으로 ARM 아키텍처 설계 기술을 라이선스
      받으려고 하는 것만 봐도, A弧 아키텍처가 얼마나 성공적인지 알 수 있다. 그 주된 예로，
      프리스케일 반도체는 자사의 i.MX 어플리케이션 프로세서 제품군에 ARM 아키텍처를 라이
      선스 받아서 사용하고 있다. 이 A弧 기반의 통합 프로세서는 이동 게임기 , PDA, 핸드폰
      등의 사용자용 멀티미디어 장치 산업에서 폭넓은 성공을 거두었다.

      프리스케일의 ARM 계열 제품은 i.MX21과 i.MX31 어플리케이션 프로세서가 있다．
      iJv1X21은 ARM9 코어를 내장하고 있고, i.MX31은 ARM11 코어를 사용한다. TI 제품과
      마찬가지로, 이 Soc들도 사용자용 이동성 멀티미디어 장치를 위한 보조 장치들을 내장하고
      있다. iJvIX21/31은 다음과 같은 인터페이스를 soc 내부에 가지고 있다．

         口 그래픽 가속기

         口 MPEG-4 인코더28)

         口 키패드 및 LCD 컨트롤러

         口 카메라 인터페이스



28) C역자주） MPEG-4 형식의 동영상을 압축할 수 있는 하드웨어 코떽
                                                            프로세서 기본        Chapter 3



            口 오디오 멀티플렉서

            口 IrDA 적외선 입출력

             口 SD/MMC 인터페이스

             口 PCMCIA, USB, DRAM 컨트롤러 및 시리얼 연결을 위한 UART 등의 다양한 입출력 인터
                페이스


    3.2.1] 인텔 ARM 엑스스케일
          인텔에서는 ARM v5TE 아키텍처 기반의 통합 프로세서들을 여러 7下1 생산 및 판매하고 있
          다. 인텔은 이 아키텍처에 엑스스케일（XScale）이라는 이름을 사용한다. 이 프로세서들은 용
          도에 따라 몇 개의 카테고리로 나눌 수 있다. ［표 3-10］은 용도에 따른 엑스스케일 제품군을
          요약한 것이다．

          ［표 3-10] 인텔 엑스스케일 프로세서 요약

           특징                     응용 사례

           어플리케이션 프로세서            핸드폰 및 PDA               PXA27x, PXA29x

           입출력 프로세서               저장 장치, 프린팅, 텔레매틱스
                                                          10P331/332/333
                                  등을 위한 고속 데이터 처리

           네트워크 프로세서              네티워킹 및 데이터 처리, 고속       IXP425, IXP465 IXP2350,
                                  패킷 처리 등                 IXP2855


          많은 통신용 장비 및 사용자를 위한 제품들이 인텔의 엑스스케일 프로세서를 이용해서 개발
          되었다. 그 중에서 잘 알려진 제품으로는 가민（Garmin) 사의 네비게이션 iQue M5, 휴렛
          팩커드（Hewlett尸Packard）의 iPAQ, 팜（Palm Treo）과 모토로라恤0切r아a A760）의 스
          마트폰 등이 있다. 이들은 현재 모두 리눅스에서 지원하는 프로세서들이다，

          인텔의 네트워크 프로세서는 고속의 데이터 경로（Data寸path)29) 처리가 요구되는 고성능
          통신 장비에서 사용되는 것을 볼 수 있다. 고속의 데이터 처리는 예를 들자면 깊은 단계까지
          의 패킷 조사, 데이터 암호화／복호화（en/decryption) , 패킷 필터링 , 신호 처리 등의 연산
          등이 포함된다．

    29) ［역자주그 Datapath : 어떤 뎨이터를 올바른 경로로 보내는 일， 예를 들면 네트워크 패킷을 해당하는 주소를 갖는 장치로 보내
      는 일을 생각해 볼 수 있다．



1
          Embedded Linux Primer




       이들 네트워크 프로세서들은 ARM 코어와 함께 하나 또는 그 이상의 전용 처리 엔진을 내장
       하고 있는데 , 이를 네트워크 처리 엔진（NPE: N毗work Processing Engine）이라고 부른
       다. 이 NPE들은 실시간으로 특정한 데이터 경로 조작을 위해서만 전용으로 사용된다. NPE
       는 ARM 코어가 실행되는 것과 병렬로 마이크로 코딩된（microcoded) 알고리즘을 수행할
       수 있다는 점에서 하나의 마이크로프로세서로 볼 수 있다. 인텔의 강력한 통합 프로세서 제
       품군에 대한 추가적인 정보는 인텔 웹사이트 www.ii北el.com을 참고하기 바란다．


3.2.12 기타 ARM
       지면 관계상 여기에 다 나열할 수도 없는 100여 7가 이상의 반도체 업체들이 ARM 아키텍처
       에 기반한 통합 솔루션을 제공하고 있다. 많은 업체가 핸드폰 시장이나, 광 저장 장치 영역
       네트워크（SAN) 30) , 통신 처리 , 자동차 시장 등의 수직 시장에 특화된 어플리케이션 프로세
       서를 제공하고 있다. 이들 업체 중에는 알테라（Altera) , 삼성 전자, 필립스 반도체 , 후지쯔
       등이 있다. ARM을 라이선스 받은 업체 목록과 기타 자세한 정보를 위해서는 ARM 테크놀
       로지 홈페이지 www.arm.com에 들러 보기 바란다．


3.2.13 키타 아키텍처
       지금까지 임베디드 리눅스 시스템으로 폭넓게 사용되는 주요 아키텍처를 살펴보았다. 하지만
       좀 더 완전히 짚고 넘어가기 위해서 , 리눅스가 지원하는 다른 아키텍처들도 알아 둘 필요가
       있다. 최근 버전의 리눅스는 25깨의 아키텍처를 위한 하위 가지（즉, 디렉터리）를 가치고 있
       다. 그중 어떤 경우는 64비트로 구현된 아키텍처가 32비트의 버전과 분리된 경우도 있고，
       또 어떤 아키텍처는 더 이상 지원하지 않고 사라진 것도 있다．

       리눅스 소스 트리에 있는 몇 개를 예를 들면, 썬（Sun）의 Sparc, Sparc64와 Tensilica의
       Xtensa 그리고 NEC의 v850을 들 수 있다. 시간을 내서 리눅스 커널의 아키텍처 디렉터리
       를 여기저기 살펴보면 리눅스가 포팅된 아키텍처들이 어떤 것들이 있는지 알 수 있을 것이다．
       하치만, 이들 아키텍처 디렉터리에 있는 소스가 모두 최신 버전은 아닐 수 있다는 점은 알아
       두어야 한다. 물론 주류 아키텍처들의 코드는 최신일 테지만, 확실히 하고자 한다면 리눅스
       커뮤니티에서 최신개발 상황을 파악하거나, 사용하는 임베디드 리눅스 제공 업체에 문의해
       야 한다. 부록 E, "오픈 소스 리소스'에서는 최신의 리눅스를 유지하기 위해서 참고할 만한
       웹 사이트 등의 리소스 목 록 을 볼 수 있다．

30) （역자주） Storage Area NeI叩ork : 대규모 네트워크 사용자를 위해서 다른 종류의 저장 장치들을 관리하는 네트워크
                                                           프로세서 기본   Chapter 3




3.3 하드웨어 플랫폼
       공통된 하드웨어 기준 플랫폼을 사용하고자 하는 아이디어는 새로운 것이 아니다. 오랜 역사
       를 갖는 플랫폼인 PC/104와 VMEbus31）가 임베디드 시장에서 시험 기간을 견디며 자리를
       지키고 있는 하드웨어 플랫폼의 두 가치 예이다. 좀 더 최근의 성공적인 플랫폼으로는
       CompactPCl와 거기서 파생된 플랫폼을 들 수 있다．


3.3.1 CompactPCl
       Con叩ac叩CI(cPCI)는 PCI의 전기（Electrical) 표준과 유로카드（Eurocard) 물리 표준
       을 토대로 만들어진 하드웨어 플랫폼이다. cP(끄는 다음과 같은 일반적인 특징을 갖는다．

         口 3U32) 또는 6U의 높이를 가지는 세로형 카드

         口 카드를 고정하고 분리하기 위한 걸쇠 장치
         口 전면 후면 패널의 I/o 연결 지원
         口 고小집적도의 후면（backplane) 커넥터

         口 동작 중에도 장치를 제거할 수 있는 기능을 고려한 전원 핀
         口 많은 업체에서 지원
         口 표준 PCI 칩셋과 호환됨

       cPCI 아키텍처에 대한 표준 명세서나 기타 내용은 PCI 산업 컴퓨터 생산 그룹（PICMG:
       PCI Industrial Computer Manufacturers Group)의 cPCI 웹 페O1 1 http : //www.
       picmg.org/v2internal/compactpci.htm을 방문해 보기 바란다．


3.3.2 ATCA
       성공적인 cPCI의 후속으로 일련의 PICMG 3.x 표준 명세서에 따라 디자인된 아키텍처와
       플랫폼인 ATCA(Advanced Telecommunications Computing Architecture）가 있다．


31) VMEbus 자체는 사실 하드웨어 기준 플랫폼은 o1니고， 유로카드（Euroc月rd) 하드웨어 표준을 기반한 것이다. 유로카드는 다양한
    업체 간의 호환성 수준을 등급으로 나타낸다．
32) （역자주） U는 서버나 스위치의 크기를 나타내는 단위, lu는 1. 75인치의 길이를 의미함．


                                                                          105
         Embedded Linux Primer




       많은 대형 업체들이 새로운 ATCA 기반 플랫폼을 개발 및 판매하고 있는데 , 이 ATCA 플랫
       폼은 주로 캐리어 급（carri町-class)33) 전자 통신 스위칭 및 천송 장비 , 고급 데이터 센터
       서버나 데이터 저장장비에 사용된다．

       ATCA 플랫폼은 기존 조직 내에서만 독점적으로 사용되던 하드웨어 , 소프트웨어 플랫폼을
       재치고 새로운 흐름으로 부각되고 있다. 전자 통신, 네트워킹 장비 생산 업체들 중에서 가장
       큰 업체들의 상당수는 내부에서 디자인한 닫힌 형태의 하드웨어 플랫폼에서 서서히 탈피하고
       있다. 이러한 경향은 소프트웨어에서도 마찬가지인데 , 운영체제에서부터 높은 가용성이나 프
       로토콜 스택 등을 지원하는 이른바 미들웨어에까지 영향을 미치고 있다. 소형화（downsizing)
       와 시장 적기 진입（time to market）에 대한 압력이 이런 경향을 주도하는 주요 원인이 되고
       있다．

       ATCA는 몇 개의 PICMG 표준 명세서에 의해서 정의되는데 , ［표 3-11］은 이 표준 명세서
       를 정리한 것이다．

      ［표 3-11) ATCA PICMG 3.x 표준 명세서 요약

        명세서             설명

        미OMG 30         상호 연결, 전원, 냉각 방식, 기본 시스템 관리를 포함한 기계적（mecha毗al) 명세서

        미OMG 3. ]       이더넷과 파이버 채널 스위치 인터페이스（fiber chann이 switching)

        디OMG 3.2        인피니밴드巾nfiniband) 파이버 채널 스위치 인터페이스

        미OMG 3.3        스타패브릭(StarFab祠 인터페이스

        디OMG 3.4        P（긔 익스프레스 인터페이스

        디OMG 3.5        RapidlO 인터페이스


       여기서 다룬 하드웨어 플랫폼들은 임베디드 리눅스 플랫폼에 관한 최근의 논의에서 가장 많
       이 회자되는 것들이다. 특히 ATCA는 점점 더 상업적인 기성 기술（COTS）로까지 발전해 나
      가고 있다. ATCA와 리눅스는 모두 최근의 산업적인 흐름에서 점점 더 중요한 역할을 차지
      하고 있다．


33) [역자주） 캐리어 급（Carrier class）은 고속 네트워크에서 사용되는 하드웨어 및 소프트웨어를 말한다. 매우 높은 신뢰성을 요구
  하는 환경이다．
                                                              프로세서 기본      Chapter 3




3.4 요약
       口 리눅스가 지원하는 많은 독립형 프로세서를 알아보았다. 가장 폭 넓게 지원되는 프로세
         서는 IA32/IA64와 PowerPC 아키텍처이다. 이런 독립형 프로세서는 고성능의 연산을
         위한 엔진을 구성하기 위한 기본 요소로 사용된다. 이 장에서는 인텔, IBM, 프리스케일
         의 몇 가지 예제를 살펴보았다．

       口 통합형 프로세서 또는 시스템 온 칩（Sc乂方이 임베디드 리눅스 분야를 장악하고 있다. 몇
         몇 업체의 프로세서와 인기 있는 코어 아키텍처들이 임베디드 리눅스를 위한 시스템에
         사용되는데, 이 장에서는 그 중에서 가장 많이 사용되는 몇몇 프로세서들에 대해서 아키
         텍처와 생산 업체별로 살펴보았다．

       口 시장의 통향은 점점 더 독점적인 내부 하드웨어와 소프트웨어로 구성된 플랫폼에서 상업
         적인 기성품을 이용하는 방향으로 나아가고 있다. 임베디드 리눅스에서는 두 가지 플랫
         폼 cPCI와 ATCA가 널리 사용된다．



3.4. ] 더 읽01 보기
       PowerPC 32비트 아키텍처 참고 매뉴얼 :
       尸rogram끄d끄g 月h町r끄2ments Manual for 32-Bit in그pleme끄tations of t力e Power只-V
       Arc力北ecture只？可舡O끄 2
       프리스케일 반도체
       www. freescale. com/files/product/doc/MPCFPE32B. pdf


       PowerP(그 64비트 아키텍처 참고 문서 :
       T力e Prograi끄mi끄g 互nviro끄I끄e끄ts 兀Ian ual for 64-Bi亡 九月cro刃rocessorsVersion 3. 0
       IBM


       PowerPC어］ 대한 짤막한 정리 :
       A Deve加刃er늉 (7uide to 功e 尸아V万1? Arc力itecture
       Brett Olsson, Processor Architect, IBM
       Anthony Marsala, Software Engineer, IBM
       www-128. ibm. com/developerworks/linux/library/l- powarch/


       인텔 엑스스케일 요약 페이지
       www.intel. com/design/intelxscale/


                                                                                 107 I
이번 장에서 배울 내용

  U 배경

  U 리눅스 커널의 구성

  U 커널 빌드 시스템

  U 리눅스 커널 구하기

  U 요약
難蔓U     Embedded Linux Primer




      리눅스 커널의 내부에 대해서 알고자 할 때 참고할 수 있는 커널 디자인 및 동작 원리를 다룬
      좋은 책들이 많다. 그 중 일부는 이 장의 4.5.1절과 다른 장의 뒷부분의 "더 읽어 보기"에서
      소개하고 있다. 하치만 프로젝트 관점에서 커널이 어떻게 조직되어 있고, 구조를 갖추고 있
      는지를 다룬 책은 거의 없다. 만약 독자가 새로운 임베디드 시스템 프로젝트를 진행하면서
      어떤 기능을 추가하기 위해 커널의 일부분을 수정하고자 할 때 그 올바른 위치를 어떻게 찾을
      수 있을까2 자신의 시스템의 아키텍처에 필요한 중요 파일들이 어떤 것들인지는 어떻게 알
      수 있을까2

      언뜻 봐서는 리눅스 커널을 이해하고 지정한 플랫폼 또는 어플리케이션에 맞도록 구성하는
      작업은 거의 불가능한 일 같아 보인다. 최근의 커널 배포판, 즉 커널 소스 트리는 2만 7긔1 이
      상의 파일에서 총 6백만 라인 이상의 코드로 이루어져 있는데, 이는 아직 시작에 불과하다．
      거기에 추가적으로 필요한 툴들이 있을 것이고, 루트 파일 시스템 그리고 기타 효율적인 시
      스템을 위한 응용 프로그램들 또한 필요할 것이다．

      이 장에서는 리눅스 커널을 소캐할 텐데 , 먼저 커널이 어떻게 구성되어 있고, 소스 트리는
      어떤 구조로 되어 있는지를 살펴볼 것이다. 그 후에 리눅스 커널 이미지를 만들기 위해 필요
      한 요소들을 알아보고, 커널 소스 트리의 구조에 대해서도 생각에 볼 것이다. 그 다음에 커널
      빌드 시스템 및 커널 구성 및 빌드 시스템을 위한 파일들에 대해서 자세히 살펴보도록 하자．
      그리고 온전한 임베디드 리눅스 시스템을 개발하는 데 어떠한 것들이 필요한지 살펴보는 것
      으로 마무리할 것이다．



4. ] 배경
      리눅스는 핀란드 헬싱키 대학의 대학생이던 리누스 토발즈（Linus Torvalds）에 의해서 7]j
      발되었다. 그는 1991년에 개발을 시작했는데 , 리누스는 그 해 8월 뉴스 그룹 camp. as.
      mini>＜어］ 지금은 아주 유명해진 다음의 글을 올렸다．



        작성자： torvalds아1aava.He1sinki .FI （리누스 베네딕트 토발즈）
        뉴스그룹： comp. os.mmnix
        제목 : 미닉스에서 가장 있었으면 하는 기능은 뭐가 있을까요7
        요약 : 새로운 운영체제에 대한 작은 조사
                                                   다른 관점에서 본 리눅스 커널   Chapter 4



        I시XIID: <1991Aug25. 205708. 9541@klaava.Hels-inki .FI>
       날짜 : 1991년 8월 25일！ 20: 57: 08 GMT
       소속： 헬싱키 대학

       미닉스（mi nix）를 쓰는 모든 분들1 안녕하세요7
       저는 386(486) AT계열에서 사용할 수 있는 （무료） 운영체제를 하나 개발하고 있습니다（그냥 취미로
       하는 것이고！ gnu처럼 규모가 크7和F 전문적이지는 않습니다）.
       금년 4월부터 만들기 시작했고！ 지금은 사용할 수 있을 만큼은 진행되고 있습니다．
       제 0s가 어느 정도는 미닉스 운영체제와 닮았기 때문어K그 중에서도 물리적인 （실용적인 이유에서） 파일
       시스템 구조가 같습니다） 미닉스의 좋은 점과 나쁜 점들에 대해서 사람듈의 의견을 좀 받고 싶습니다．
       현재는 배쉬（bash 1. 08）와 9CC (1. 40）을 포팅했는데， 잘 동작하는 것 같습니다． 몇 달 안에 실
       제로 실용적으로 사용할 수 있는 뭔가를 만들 수 있을 것 같습니다．그래서 사람들이 어떤 기능들을 가
       장 원하는지 알고 싶습니다．
       어떤 제안도 환영입니다． 근더I, 실제로 구현할지는 약속 못 드립니다. :-)


                    aI누스 (torvalds@kruuna.helsinki. fi)

       PS. 물론 미닉스 코드는 모두 자유롭게 쓸 수 있습니다． 그리고 이 운영체제는 멀티 쓰레드를 지원하
       는 파일 시스템을 갖고 있습니다． 다른 시스템에 포팅은 안 됩니다（태스크 스위칭 등에서 386 종속적
       인 기술을 씀）. 그리고 AT 하드디스크 외에 다른 것은 아마도 절대 지원하지 않을 것 같습니다． 이
       게 제가 한 전붑니다． n (.



    이 최초 발표 이후부터 리눅스는 다른 상용 운영체제와 겨룰 수 있을 정도로 강건성
     (robustness) , 신뢰성（reliabi胤y) 및 고성능（h琯h-end) 기능들을 갖춘 완전한 운영체제
     로 발전해 왔다. 어떤 예측 결과에 따르면 전 세계 웹 서버의 절반 이상이 리눅스를 이용해
     구동되고 있다고 한다. 온라인 검색 엔진의 거인 구글（Goo엎e）도 많은 수의 저가 PC를 조합
     한 무 정지성（fau노tolerant : 폴트e톨러런트） 리눅스를 이용해서 검색 엔진을 구현하고
     있다는 것은 잘 알려진 사실이다.


4.1. ] 커널 버전
    리눅스 소스와 기타 보조 모듈 및 자료는 다양한 곳에서 얻을 수 있다. 독자가 사는 지역의
     서점에만 가더라도 리눅스를 다루는 많은 책에서 리눅스를 CD-ROM 부록으로 제공하는 것
     을 볼 수 있을 것이다. 또한 인터넷 상의 여러 곳에서 커널이나 완전한 리눅스 배포판을 받을
     수 있다. 리눅스 커널의 공식 홈페이지는 www.kernel. org이다. 그리고 kernel.org에 존재
   月1    Embedded Linux Primer




       하는 소스 트리를 가리키는 용어로 기준 소스（m례nlinel) source) 또는 기준 커널（mainline kernel)
       이라는 말을 자주 들을 수 있을 것이다．


       이 책이 쓰여진 시점에는 리눅스 커널 2.6이 최신 버전이다. 개발 초기 단계에서 개발자들은
       커널 소스에 대해서 개발용 또는 실험적인 커널과 안정적인 커널 또는 배포 가능한 커널을
       구분하기 위해서 숫자를 붙이는 방식을 미리 정의했다. 이런 숫자 체계는 주 버전（II刈or
       version）을 가리키는 숫자와 보조 버전（minor version）을 의미하는 숫자 그리고 마지막으
       로 순서를 의미하는 숫자를 사용한다. 리눅스 2.6까지는 보조 버전이 짝수이면 배포용 커널
       을 의미하고, 홀수이면 개발용 커널을 나타낸다. 예를 들면 다음과 같다.

         口 니nux 2.4.x -- 배포용 커널

         口 니flux 2.5.x 小 실험용（개발용）

         口 니flux 2.6.x 小 배포용 커널


       지금까지는 리눅스 26으로부터 분리된 개발용 커널은 아직 없다. 커널에 새롭게 추가될 기
       능, 성능 개선 사항, 버그 수정 사항 등은 모두 지정된 관리자들이 취합한 후에 앤드류 모튼
       (Andrew Morton) , 리누스 토발즈에 의해서 관리되는 리눅스 소스 트리에 최종적으로 반
       영하게 된다．

       현재 개발을 위해서 사용중인 커널 버전이 얼마인지는 쉽게 알 수 있다. 소스 트리의 최상위
       에 있는 makef lie2）의 처음 몇 줄혀］ 정확한 커널 버천을 기술하고 있다．



          VERSION = 2
          PATCHLEVEL = 6
          SUBLEVEL = 14
          EXTRAVERSION =
          NAME=Afflueflt Albatross




1) ［역자주） II너nilne은 직역O뻔 '주류, 중심적인'으로 해석할 수 있지만, 여기서는 커널 소스를 관리하는 더1 기준이 된다는 의미에
   가깝기 때문에 '기준'으로 번역했다．
2) 잠시 후어］ makefile과 커널 빌드 시스템에 대해서 이야기할 것이다．
                                                       다른 관점에서 본 리눅스 커널         Chapter 4



       같은 makefile의 후반부에서 , 위의 매크로들은 다음과 같이 버전 단계를 나타내는 매크로를
      만들기 위해서 사용된다．

         KERNELRELEASE=$(VERSI0N) . $(PATCHLEVEL) . $(SIJBLEVEL) $(EXTRAVERSI0N)


      이 매크로는 커널 소스 트리 내의 일부 위치에서 커널 버전을 나타내기 위해서 사용된다. 사
      실, 커널 개발자는 커널 버전을 나타내는 용도로 자주 사용되는 일련의 매크로를 자체적으로
      가지고 있다. 이 매크로는 . . . /inciude/iiriux/version.h3）에서 찾아볼 수 있다. 그
      내용을 ［리스트 午1］에서 나타냈다．

      ［리스트 4-1] 커널 포함 파일： . . ./inc山de/Iinux/vers油n.h

         #define UTS_RELEASE "2. 6.14"
         #define LINUX_VERSI0N_C0DE 132622
          #define KERNEL_VERSI0N(a,b, C) ( ( (a) << 16) + ( (b) << 8) + (c) )




       또한 동작중인 리눅스 시스템의 명령 프롬프트에서 다음과 같이 입력하면 현재 동작중인 커
      널 버전을 확인할 수 있다．

         $ cat /proc/version
         Linux version 2. 6.13 (chris@pluto)       (gcc   version 4. 0. 0   (DENX ELDK   4. 0
         4.0.0力 #2
         Thu Feb 16 19: 30:13 EST 2006


      커널 버전에 대해서 한 가지 더 살펴보자면, 자체적인 커널 프로젝트에서 커널 버전을 구분
      하기 위한 용도로 EXTRAVERS ION 부분을 사용할 수 있다. 예를 들어 , 커널의 새로운 기능에
      대해서 어떤 성능적인 개선을 구현하고 있다면 다음과 같이 EXTRAVERSION어］ 이름을 줄 수
       있다．

         EXTRAVERSI0N=-foo


      나중에 커널을 빌드하고, 해당 커널이 수행중일 때 cat /proc/version 명령을 통해서 커
      널 버전을 확인하면 Linux version 2. 6.13- foo라는 문자열을 볼 수 있을 것이다. 이렇
      게 하면 기존 커널과 현재 개발중인 커널을 쉽게 구별할 수 있다．


3) 이 책에서 점 3개， 즉 . . . 은 리눅스 코드가 위치하는 최상위 디렉터리를 나타내는 의미로 사용된다．


                                                                                     113
         Embedded Linux Primer




4.1.2 커널 소스 저장소4)
      리눅스 커널 소스 코드에 대한 공식 홈페이지는 www.kernel. org이다. 여기서 최신의 커널
      및 이전 버전의 리눅스 커널은 물론이고 수많은 패치들도 구할 수 있다. 주 FTP 저장소인
       f햐）.kernel. org에는 현재 버전부터 리눅스 커널 1.0에 이르기까지 모든 자료가 저장되
      어 있다. 이 사이트는 개발 중인 커널에 대해서 가장 빠른 소식을 접할 수 있는 중요한 사이
      트이다．

      kernel.org 사이트에서 최신 커널을 다운로드해 압축을 풀어 보면 소스 트리 내부에 25개의
      각기 다른 아키텍처와 서브 아키텍처를 볼 수 있을 것이다. 리눅스 커널의 다른 개발 버전
      중의 일부는 중요한 몇몇 아키텍처들만 지원한다. 그 이유는 단치 관련 개발자 수 및 커널
      변경이 거의 몇 개의 아키텍처에만 해당하기 때문이다. 만약에 모든 개발자들이 kernel.org
      에 자신의 아키텍처에 태한 패치를 제출5）한다면 소스 트리를 유지 관리하는 관리자들이 변
      경 사항과 패치를 관리하느라 포화상태에 빠져서 , 다른 개발에 전혀 시간을 쓸 수 없게 될
      것이다. 커널 개발에 관여한 사람들에게 한번 물어보면 지금도 아주 바쁘다고 할 것이다！

      소스 트리가 기준（n追inline) 소스 저장소인 kernel.org 외부에 존재하는 버전도 몇몇 있는
      데 이는 주로 특정 아키텍처를 위한 커널의 경우가 대부분이다. 예를 들어 , MIPS 아키텍처
      를 이용해서 개발하는 개발자라면 적당한 커널을 www.linu牙m如s.org에서 찾을 수 있을
      것이다. 일반적으로 어느 한 아키텍처에서 작업했던 내용들을 최종적으로는 kernel.org의
      커널에 제출해서 반영하게 된다. 해당 아키텍처의 개발자들 대부분이 커널 최신 버전을 항상
      유지하기 위해서 기준 커널에 자주 반영을 하려고 노력하지만, 기준 커널에 어떤 패치를 반
      영하는 것이 항상 간단하게 되는 것은 아니다. 그래서 기준 커널에는 어느 정도 뒤쳐진 버전
      이 포함된 상태가 될 수도 있는 것이다. 결국 현재 기준 커널과 해당 아키텍처의 최신 버전
      커널과는 어느 정도 버전 차이가 있을 수밖에 없다．

      만약에 자신이 개발하려는 대상에 맞는 커널을 찾고자 한다면 가장 좋은 절차는 먼저 리눅스
      소스 트리에서 최신 버전을 받는 것이다. 그리고 개발 시스템에서 자신이 사용할 프로세서를
      지원하는지를 확인한다. 그 후에 리눅스 커널에 관한 메일링 리스트를 검색해서 시스템에 맞
      는 커널 패치 및 이슈 사항을 검색한다. 그리고 다른 관련 있는 메일링 리스트도 검색해서

4) ［역자주） 버젼 관리가 되고 있는 소스 트리를 저장하고 있는 서버상의 저장소를 리포지토리 (repo訊이ry）라고 햐며, 여기서는 저장
   소로 번역했다．
5) （역자주） 커널에 대한 어떤 수정 사황을 리눅스 소스 트리에 반영하기 위해서는 패치 형태로 그 내용을 반영힌다．
                                                       다른 관점에서 본 리눅스 커널   Chapter 4




       정보를 찾도록 한다. 부록 B, "오픈 소스 리소스'에는 참고할 만한 좋은 자료들과 커널 소스
       에 관련된 정보를 찾을 수 있는 사이트, 메일링 리스트 목록 등을 정리한 내용이 있다．



4.2 리눅스 커널의 구성
       이어지는 몇 개의 섹션에서는 리눅스 커널 소스들이 어떻게 구성되고, 조직되어 있는지 알아
       보도록 하자. 소스 코드의 구조에 대해서 이해하고 나면 거대하고 복잡한 리눅스 소스 코드
       내에서 여기저기 찾아다니는 게 훨씬 쉬워질 것이다. 리눅스 소스 트리는 시간이 지남에 따
       라서 그 구조가 상당히 개선되었는데 , 특히 다양한 아키텍처와 여러 머신들을 지원하기 위한
       소스를 담고 있는 아키텍처 디렉터리 부분이 그렇다. 이 책이 쓰이는 시점에는 ppc와 ppc64
       아키텍처를 하나로 묶어서 powerpc로 통합하려는 노력이 진행되고 있다6) . 어느 정도 정리
       가 돼서 안정화되고 나면 중복된 코드도 없앨 수 있고, 파일들을 좀 더 깔끔하게 정리할 수
       있을 뿐만 아니라, 기능들이 분산되지 않는 등의 많은 이점이 있을 것이다.


4.2. ] 최상위 소스 디렉터리
       이 책 전반에서 최상위（top니evel) 소스 디렉터리라는 말을 자주 사용할 것이다. 이 말은 모두
       리눅스 커널 소스를 담고 있는 디렉터리의 가장 상위 디렉터리를 뜻하는 것이다. 사용하는
       시스템의 종류에 따라서 다르겠지만, PC에서 사용하는 리눅스의 경우는 보통 加sr/ src/
       linux-兄y. z에서 소스 코드를 찾을 수 있다. 여기서 >( . y . Z는 커널의 버전을 나타낸다．
       이 책에 사용되는 . . .／는 이 커널 소스의 최상위 디렉터리를 가리킨다．

       커널 소스에서 최상위 디렉터리에는 다음 목록에 나타낸 것과 같은 하위 디렉터리들이 포함
       되어 있다（다음의 목록에는 디렉터리 외의 요소들, 즉 파일과 소스 형상 관리를 위한 보조
       디렉터리7）도 생략했다）.



          arch   crypto   Documentation    drivers fs     include
          mnit   ipc      kernel   lib    mm     net
          scripts security sound    usr



6) （역자주） 현재의 최신인 2. 6. 23을 확인한 결과 통합이 완료된 상태다．
7) （역자주） cvs나 SubVersion과 같은 소스 형상 관리 툴은 각칵 디렉터리에 cVs나 . svn과 같은 디렉터리를 만들어 필요한 정보를
   저장한다．
 難 ma     Embedded Linux Primer




        이들 디렉터리는 그 안에 추가적으로 여러 소스 코드 및 makefile 등의 파일을 포함하고 있
        는 하위 디렉터리를 더 가치고 있다. 리눅스 커널 소스 트리에서 가장 큰 하위 디렉터리 구조
        를 갖는 것은 단연 . . . /drivers가 최고이다. 여기에서 이더넷 네트워크 카드에 대한 드라
        이버 , USB 컨트롤러 및 리눅스가 지원하는 기타 수많은 하드웨어 장치를 찾아볼 수 있다．
        그다음으로 큰 것은 짐작했겠지만 . . . larch 디렉터리이다. 여기에 20개 이상의 서로 다른
        프로세서 아키텍처를 지원하기 위한 코드가 포함되어 있다．

        리눅스의 최상위 디렉터리에는 위의 하위 디렉터리 외에도, 최상위 makefile , 숨김 파일 형
        태로 되어 있는 커널 구성 파일（점-config8) , 4.3.1.절 "잠Config 파일"에서 설명할 것이다）
        그리고 커널을 빌드하는 데는 사용되지 않지만 여러 정보를 담고 있는 기타 파일이 있다. 커
       널을 성공적으로 빌드하면 최종적으로 생기는 두 개의 중요한 파일도 이 최상위 디렉터리에
        생성된다. 그것은 각각 Sys七em.map 파일과 커널 본체인 vmlirn球인데, 잠시 후 설명하도
        록 하겠다．


4.2.2 커널 컴파일하기
        리눅스와 같이 커다란 몸체를 가진 소프트웨어 코드를 이해하려고 들면 일단 기부터 죽는데，
       내부에 어떤 일이 일어나는지 알기 위해서 단순히 코드를 한 줄 한 줄 따라 가기에는 너무
        크기 때문이다. 게다가 멀티 쓰레딩9)j斗 선점（preemption) 개념은 분석을 더욱 복잡하게
        만든다. 사실, 코드의 맨 처음 시작지점（커널이 맨 처음 수행되기 시작하는 코드의 첫 줄）을
        찾는 것도 만만치 않을 지경이다. 그래서 큰 바이너리 이미지의 내부 구성을 이해하는 좀 더
        알맞은 방법은 빌드 과정에서 사용되는 요소들을 조사하는 것이다．

       커널을 빌드하면 그 결과로 공통적인 파일이 몇 7뀨 생성되고, 하나 또는 그 이상의 특정 아키
        텍처에 한정되는 바이너리 파일이 생성된다. 이 공통적인 파일들은 아키텍처에 무관하게 항
        상 생성된다. 이 파일들 중에서 두 개는 앞에서 간단히 설명한 System. map과 vmlinux
        파일이다. System.map 파일은 커널을 디버깅할 때 사용되는데 특히 눈여겨봐야 할 매우
        흥미로운 파일이다. 여기에는 사람이 읽을 수 있는 형태로 커널 심볼（kernel syn出아）들과
        각각의 주소를 목록으로 가지고 있다. 다음 파일（vmlinux）은 지정한 아키텍처를 위한 EL
        F10) 형식의 실행 가능한 파일이다. 이 파일은 모든 아키텍처에서 커널 소스의 최상위


8) （역자주） 실제 파일명은 .cot小g이다． 영어로는 dot-config, 직역하면 잠con如이지만 보통 "쩜 con1낳라고 읽는다．
9) （역자주） M毗1때readit띵 : 하나 이샹의 쓰레드（또는 작업 딘위）가 병렬로 수행되는 것．
                                                           다른 관점에서 본 리눅스 커널   Chapter 4



         makefile에 의해서 생성된다. 만약에 커널을 빌드할 때 디버깅을 위한 심볼 정보를 포함하
         도록 설정해서 빌드하면 vmlinux 이미지에 그 정보가 포함된다. 곧 다루겠지만, 이
         vmlinux 파일이 ELF 실행 파일 형식이기는 하지만 실제로 이 파일을 이용해서 절대로 직접
         부팅을 시키지는 않는다．

        ［리스트 4-2］는 최신 커널 소스를 ARM의 엑스스케일（XScale) 아키텍처에 맞게 구성한 후
         에 make 명령을 실행했을 때 화면에 출력되는 결과를 일부 나타낸 것이다. 다음의 명령어를
        이용해서 인텔의 IXP425 통신용 프로세서를 장착한 ADI 엔지니어링의 코요테（Coyo扼）
        참조용 보드에 맞게 커널 소스 트리를 구성했다．

            make ARCH=arm CROSS_COMPILE=xscal e_be- I xp4xx_defconfi g


        이 명령어는 커널 빌드를 시작시키지는 않고, 커널 소스 트리의 프로세서와 아키텍처 관련
        초기 기본 설정을 엑스스케일 아키텍처에 맞게 준비하도록 하는 일을 한다. 즉, 이 명령은
        커널 빌드 과정을 결정하는 기본 구성 파일을 생성하는데（바로 잠config 파일）, 이 아키텍
        처를 위한 구성 기본 값（default)을 담고 있는 파일인 뇨p4xx defconfig 파일을 기반으
        로 해서 만들게 된다. 이 설정 과정에 대해서는 4.3절 "커널 빌드 시스템"에서 좀 더 살펴
        볼 것이다．

        ［리스트 4-2］를 보면 커널을 실제로 빌드하는 명령을 볼 수 있는데 , 이 리스트에는 설명을
        위해서 빌드 출력 내용의 앞부분과 맨 뒷부분의 일부만 표시했다．

        ［리스트 4-2] 커널 빌드 출락


            S make ARCH=arm CROSS_COMPILE=xscale_be- zlmage
                 CHK    include/linux/version. h
                 HOSTCC scri pts/basi c/ fl xdep

                 . <hundreds of lines of output omitted here>

                 LD       vmlinux
                 SYSMAP System.map
                 SYSMAP    . tmp_System . map
                 OBJCOPY arch/arm/boot/Image
                 Kernel : arch/arm/boot/Image is ready


10) Ex吐Ut汕le and Linking Format의 익자이며， 실행 파일의 실질적인 표준이다．
  轟U     Embedded Linux Primer




                AS       arch/ arm/boot/ compressed/head .0
                GZIP     arch/ arm/boot/ compressed/piggy. gz
                AS       arch/ arm/boot/ compressed/piggy .0
                cc       arch/ arm/boot/ compressed/misc .0
                AS       arch/arm/boot/ compressed/ head- xscale .0
                AS       arch/arm/boot/ compressed/big-endi an .0
                LO       arch/arm/boot/ compressed/ vml i flux
                OBJCOPY arch/arm/boot/zimage
                Kernel : arch/ arm/boot/ zlmage is ready
                Building modules, stage 2.




        먼저 빌드를 실행시키는 부분을 보자. 명령에 라인에 원하는 아키텍처（ARCH=arm）와 툴 체
        인（CROSS COMPILE=xscale be-)을 모두 기술하고 있다. 이렇게 하면 make로 하여금
        커널을 빌드할 때 엑스스케일용 툴 체인을 써서 빌드하도록 하고, 빌드 과정 중의 아키텍처
        에 종속된 부분들에 대해서는 arm 버전의 소스들을 사용하도록 한다. 또한 명령에 줄에는
        기mage라고 하는 타깃（target) 명11）을 기술하고 있다. 이 타깃은 많은 아키텍처에서 공통적
        으로 사용되는 것인데 , 5장, "커널 초기화'에서 상세히 다룬다．

        그 다음으로 알 수 있는 것은 빌드의 각 단계에서 사용되는 실제 명령어들이 숨겨져 있고，
        대신 축약형으로 바뀌어 있는 점이다. 이렇게 하게 된 계기는 커널 빌드 과정 중의 다양한
        출력 내용 중에서 특히 컴파일러의 경고 메시지와 같은 중요한 내용을 부각시켜 보여 주기
        위한 것이다. 예전의 커널 소스에서는 보통 여러 줄을 차지하는 컴파일 및 링크 명령어들이
        지저분하게 콘솔 화면에 모두 표시되었었다. 그 결과 출력된 내용들은 사실상 거의 알아보기
        힘들고, 컴파일러의 경고 메시지는 이러한 잡다한 메시지들에 가려서 놓치게 되곤 했었다.
        새로운 빌드 시스템에서는 빌드 과정 중혀］ 발생하는 예외 상황들에 대해서 바로 알아 챌 수
        있을 정도로 확실히 개선되었다. 혹시 빌드 과정의 완전한 출력물을 보고 싶다면 make 명령
        에 강제로 v=1이라고 기술해서 장황한（verbose) 출력 모드를 강제로 설정하면 된다．




11) （역자주） make어H] 타깃（t可解t) 은 C녜妃川e어］ 기술된 여러 결과물 또는 행위（예를 들어， 빌드 결과를 청소하는 clean）에 대한
    이름 중에서 하니를 선택하는 것이다. 간단한 예로 make deb唯는 디버깅을 위한 이미지를 만들 1대 사용하고， C꼬ike release는
    배포용 이미지를 만들 때 사용한다고 할 때 이 deb咽와 r이ease를 각각 타깃이라고 할 수 있다．


  118
                                                         다른 관점에서 본 리눅스 커널   Chapter 4



          ［리스트 4-2］에서는 이해를 좀 더 명확히 하기 위해서 실제적인 컴파일 및 링크 과정은 대
          부분 생략했다（지정한 빌드 과정에서는 900개 이상의 컴파일 및 링크 명령어들이 사용된
          다. 결국 출력 내용이 매우 길 수밖에 없다）. 중간 생성 파일들과 라이브러리들이 모두 컴파
          일되면 이 결과물들이 모두 vmlinux라는 하나의 큰 ELF 파일로 합쳐지게 된다. 물론 이
          파일의 내용 자체는 지정한 아키텍처에 종속적이지만, vmlinux라는 타깃 이름 자체는 공통．
          된 타깃 명이다. 실제로 리눅스가 지원하는 모든 아키텍처에서 vmlinux 타깃을 빌드할 수
          있다．


4.2.3 커널 단일파일12) : vmlinux
         ［리스트 士2］에서 다음 부분을 주목해 보자．

              LD /arch/arrn/boot/compressed/vml i flux

          이 vmlinux 파일은 말 그대로 커널 자체이다. 이 파일은 완전히 독립적이고, 모놀리식
          (monolithic)한13) 이미지이다. vmlinux 바이너리 내부에는 주소가 결정되지 않은 외부
          참조14）는 존채하지 않는다. 이 커널 이미지를 적절한 문맥에서 （리눅스 커널을 부팅시키도
          록 되어 있는 부트로더에 의해서） 실행시키면 스스로 현재의 보드를 부트 업시키고, 제 기능
          을 완전히 수행할 수 있는 커널이 최종척으로 남게 된다．

          어떤 시스템을 이해하려고 할 때는 반드시 그 시스템을 이루고 있는 각각의 요소들을 먼저
          이해해야 한다는 원칙에 따라서 먼저 vrnlinux 커널 객체가 어떻게 구성되어 있는지 알아
          보자. ［리스트 +3］은 빌드 과정 중에서 vrnlinux ELF 파일을 링크하는 단계를 나타내고
          있다. 이 목록에서는 긴 명령어를 행 바꿈 문자를 이용해서 나타냈는데 , 이는 좀 더 읽기 쉽
          게 하기 위해서 그렇게 표시한 것이다. 하지만 그 외의 점에서는 ［리스트 4-3］은 빌드 과정
          중 vinhinux를 링크하는 단계에서 사용되는 명령어를 그대로 나타낸 것이다. 만약에 커널
          을 손으로 직첩 빌드한다면 커널을 링크하키 위해서 명령 프롬프트에 이 명령어를 입력해야
          한다.




12) （역자주） Kernel Proper : 커널 자체, 커널을 담고 있는 단일 파일을 의미한다．
13) ［역자주） 하니로 이루어진, 일체형 구소를 의미한다．
14) （역자주） unresolved reference
         Embedded Linux Primer



       ［리스트 4-3] 링크 단계 : vmlinux




                                                              \ \
                                                                \
          xscale_be- Id -EB -p --no-undetined -x -o vmlinux

                                                            \ \
                                                          \ \
          -T arch/arm/kernel/vmiinux.lds

                                                          \
          arch/arm/kernel /head .0
          arch/arm/kernel/i nit_task .0


                                                              \ \\\
          init/ built-in.o
          --start-group
          usr/buiit-in.o
          arch/arm/kernel/built-in .o
                                                               \
                                                                   \
                                                                   \
                                                               \
          arch/arm/mm/built-in .o
          arch/arm/common/built-in. o
                                                                        \
                                                                        \\
                                                                        \
          arch/arm/mach-i xp4xx/bui it- in .0
          arch/arm/nwfpe/buiit-in .0
          kernei/buiit-in.o
                                                                            \
                                                                            \
                                                              \
                                                              \
                                                                            i
          mm/buiit-in.o




                                                              \ \ \ \ \\\ \ \
          fs/buiit-in.o
          ipc/buiit-in.o
          security/built-in.o
          crypto/bui lt- i n .0
          ]i b/］化 . a
          arch/arm/lib/ iib. a
          lib/ built-in.o
          arch/arm/lib/ buiit- in.o
          drivers/built-in.o
                                                                    \
                                                                    \
          sound/buiit-in.o                                                      1\ 1


          net/buiit-in.o
                                                                                 \
                                                                                     \
                                                                                     \
                                                                                 \
          --en小아oup
           .tmp_kaiisyms2. o




4.2.4 커널 이미지 구성 요소

       ［리스트 4-3］을 보면 vmlinux 이미지가 여러 개의 바이너리 이미지들로 구성되는 것을 알
       수 있다. 지금은 각 바이너리 이미지들이 어떤 역할을 하는지는 중요하지 않다. 중요한 것은
       커널이 어떤 요소들로 구성되어 있는지에 대해서 큰 그림을 보는 것이다. ［리스트 4_3］에저
       링크에 사용한 명령어의 첫 번째 줄은 결과 파일명을 지정한다（-o vmiinux) . 그리고 두
       번째 줄은 링커 스크립트（linker script) 파일을 지정하는데(-T vmlinux.ld引, 이 파일
       은 커널 바이너리 이미지가 어떻게 링크되어야 하는지 자세한 절차를 기술하고 있다15) .


1120
                                              다른 관점에서 본 리눅스 커널    Chapter 4


       ［리스트 4-3］의 세 번째 줄과 그 이후 줄들은 결과 바이너리 파일을 이루는 오브젝트
       化bject) 모듈들을지정한다. 맨 처음 오브젝트 파일이 head.o라는 점에 유의하자. 이 파일
       은 /arch/arm/ kernel/head. S로부터 만들어진다. 이 파일은 지정한 아키텍처용 어셈블
       리 언어로 작성된 것인데 , 로우 레벨에서 커널을 초기화하는 일을 수행한다. 만약에 커널에
       의해서 맨 처음 실행되는 코드를 찾고자 한다면 이 파일에서 시작하는 게 맞다. 왜냐하면 링
       크의 결과로 생성된 커널 바이너리 파일 내부에 있는 맨 처음 코드가 바로 이 파일이 만들어
       낸 코드이기 때문이다. 커널의 초기화에 대해서는 5장에서 자세히 살펴보도록 하자．

       다음 오브젝트 파일은 mni七m七ask. o인데 , 커널에 필요한 초기 쓰레드 및 태스크를 위한 자
       료 구조를 설정한다. 그 다음에 built-in.o라는 이름이 같은 수많은 오브젝트 파일들이
       나온다. 하지만 buil七-in 0 오브젝트 파일명의 앞부분 경로를 보면 알 수 있듯이 각각이
       커널 소스 트리의 서로 다른 위치에서 오는 것들이다. 이들 바이너리 오브젝트 파일들이 모
       두 커널 이미지에 포함되는 것이다. 그림을 통해 보면 좀 더 명확히 이해할 수 있을 것이다．

      ［그림 4-1］은 vmlinux 이미지 내부의 바이너리 구조를 보여 주고 있다. 링크 단계에서 각
       각의 행에 기술했던 내용들이 각자 칸들을 차치하고 있는데 , 지면상 크게 그리지는 않았지
      만, 각각의 기능을 담당하는 구성 요소들의 상대적인 크기는 볼 수 있다．

      내부를 이루는 바이너리 중에서 가장 큰 공간을 차치하는 3개의 구성 요소가 파일 시스템을
      위한 코드, 네트워크를 위한 코드 그리고 커널에 포함하도록 되어 있는 모든 디바이스 드라
      이버라는 것이 그리 놀랍지는 않을 것이다. 만약에 커널 코드와 특정 아키텍처를 위한 커널
      코드들을 하나로 친다면 이 부분이 그 다음으로 가장 많은 공간을 차지하는 영역이 된다. 이
      커널 영역에는 스케줄러 , 프로세스 및 쓰레드 관리 , 타이머 관리 , 그 외 커널의 핵심 기능들
      을 구현하고 있다. 당연히 커널에는 아키텍처 종속적인 기능들이 여러 가지 포함되는데 , 예
      를 들면 저수준의 문맥전환（context sw此ch) , 하드웨어 인터럽트와 타이머 처리 , 프로세서
      의 예외 처리（exception handling) 등을 들 수 있다. 이 부분은 . . . /arch/arm/kernel어］
      서 찾아볼 수 있다．




15) 링커 스크립트 파일은 독특한 문법을 갖는다． 자세한 내용은 GNU 링커의 도움말 문서들을 참고하자．
 韆 堪U     Embedded Linux Primer




                        //
                                     arch/arm/kernel/head.o
                                     arch/arm/kernel/init-task.o
                                     m it
                                     usr/bu lt-in.o
                                     arch/arm/kernel
                                     arch/arm/mm
                                     arch/arm/common
                                     arcnfarm/macn-Ixo4xx
                                     arcniarminwrpe
                                     kernel
                                     mm


                                     fs
        vmlinux   -'1

                                     pc
                                     security
                                     lib/lib.a
                                     arch/arm/壯
                                     lib


                                     drivers




                                     net

                        \\\



        I 그림 4-1 vmlinux 이미지 구성 요소


        염두에 둘 점은 우리가 커널 빌드에 대한 특정한 하나의 예를 가지고 설명하고 있다는 것이
        다. 이 예에서는ARM 엑스스케일 아키텍처를 위한 커널을 빌드하고 있다. 좀 더 정확하게는
        Intel IXP425 통신용 프로세서를 장착한 시끄 엔지니어링 참조용 보드를 사용한 시스템을
        위한 커널 예제를 다루고 있는 것이다. ［그림 4-1］에서 특정 머신16）을 위한 바이너리 요소
        인 arch/arm/mach-i)四4xx를 볼 수 있다. 각각의 아키텍처와 머신 종류（프로세서／참조
        용 보드）에 따라서 커널 소스의 아키텍처 디렉터리 내의 다른 파일들을 이용하기 때문에
        vmiinux 이미지 파일이 조금씩 다르게 생성된다. 하지만 먼저 하나의 예제를 이해하고 나
        면 다른 것들도 쉽게 알 수 있을 것이다.


16) （역자주） 머신， 아키텍처， 프로세서 각각이 혼동될 것이다. 아키텍처 및 프로세서는 姑6. ARM11. AR入刃처럼 프로세서 Soc 제품
    군애서 코어로 내장하고 있는 기본 프로세서 설계를 말한다고 볼 수 있다. 머신은 S3c244o, lxi끄000 등과 같이 실제로 칩 형태
    로 생산된 경우라고 생각하면 된다．
                                          다른 관점에서 본 리눅스 커널      Chapter 4



커널 소스 트리에서의 각 구성 요소를 기능적으로 분석하기 위해서 ［그림 千1］에 있는
vrnlinux 이미지를 이루는 바이너리 구성 요소를 짧은 설명과 함께 ［표 4山에 정리했다．

［표 4-1] vmlinux 이미지 구성 요소에 대한 설명

 구성 요소                             설명

 arch/arm/kernel/head. o           커널의 0비텍처 종속적인 시작 코드忖artu口 코드）

 mnit task. o                      커널에 필요한 초기 쓰레드 및 태스크 자료 구조

 init/ buil七 in. （그                커널을 초기화 하는 주 코드（5장 참조）

 usc/built- in .0                  내장 mni七ramf s 이미지（5장 참조）

 arch/arm/kernel/built- in. o      ARM 아키텍처를 위한 커널 코드

 arch/ arm/rn / built- in. o       ARM 0톄텍처를 위한 메모리 관리 코드

                                   ARM 아키텍처를 위한 공용 코드. 아키텍처마다 다양
 arch/arm/common/built- in .0
                                   하다．

 arch/arm/mach-ixp4xx/buil七in. o   IXP4xx 머신을 위한 코드, 보통은 초기화 코드

 arch/arm/nwfpe/built- in. o       0끼텍처 종속적인 부동 소수점 에뮬레이션 코드

 kernel/built- in. o               커널 자체를 위한 범용 코드들

 mm/built- in. o                   메모리 관리를 위한 범용 코드들

 ipc/ built- in .0                 프로세스간 통신(IPC), 예를 들어， SysV의 'P（二

 security/ built- in. o            리눅스의 보안 모듈

 lib/ lib. a                       기타 도움 함수들의 모음

 arch/arm／끄力／U上 . a                0끼텍처 종속적인 일반 기능들． 0비텍처마다 다잉后F다．

 lib/ built- in .0                 공용 커널 도움 함수들

 drivers/ built- in .0             동적으로 로드되지 않는 모든 디바이스 드라이버들

 sound/built- in. o                사운드 드라이버

 net/built- in. o                  리눅스 네트워킹 모듈

 .tmp ka11sym52. o                 심벌 테이블



                                                                      123
  鞍1     Embedded Linux Primer



       일반적으로 커널 자체（kernel proper）라고 이야기하면 이 말은 vmlinux 이미지를 가리키
       는 것이다. 앞에서도 이야기했듯이 , 이 커널 이미치를 통해서 바로 부팅을 하는 플랫폼은 거
       의 없다. 그 이유 중의 하나가, 대부분의 경우 커널 이미지 자체를 전체적으로 압축해 두기
       때문이다. 그래서 최소한 부트로더라도 있어서 이 커널 이미지의 압축을 반드시 풀어야 하는
       것이다. 많은 플랫폼들이 이미지에 압축 해제를 수행하는 일종의 스텁 (stub) 코드를 필요로
       한다. 5장의 뒷부분에서 , 아키텍처 , 머신의 종류, 부트로더 그리고 부팅 요구 사항들에 따라
       서 이미지가 어떻게 포장되는지를 살펴볼 것이다．


4.2.5 하위 디렉터리 구성
       지금까지는 빌드 시스템이 어떻게 커널 이미지를 제어하는지를 보았고, 이제 커널의 하위 디
       렉터리의 구조를 한번 살펴보도록 하자. ［리스트 午4］는 mach-ix1그425 디렉터리에 있는
       요소들을 모두 보여 주고 있다. 이 디렉터리는 . . . /arch/arm 아래 , 즉 ARM 아키텍처를
       위한 하위 디렉터리에 있다．

       ［리스트 4-4) 커널 하위 디렉터리

         $ is -i linux- 2.6/arch/arm/mach-ixp425
         total 92
         -rw-rw-r- - 1 chris chris 11892 oct 10 14: 53 built-in.o
         -rw- rw-r- - 1 chris chris   6924 Sep 29 15: 39 common. c
         -rw- rw-r- - 1 chris chris   3525 0ct 10 14: 53 common. o
         -rw- rw-r- - 1 chris chris 13062 Sep 29 15: 39 common-pci. c
         -rw- rw-r- - 1 chris chris  7504 0ct 10 14: 53 common-pci.o
         尸rw- rw-r-- 1 chris chris   1728 Sep29 15: 39 coyote-pci.c
         -rw- rw- r- - 1 chris chris 1572 oct 10 14: 53 coyote-pci .0
         -rw- rw- r- - 1 chris chris  2118 Sep 29 15: 39 coyote-setup. c
          rw- rw寸- - 1 chris chris    2180 0ct 10 14: 53 coyote-setup. o
         -rw- rw-r- - 1 chris chris   2042 Sep29 15: 39 ixdp425-pci.c
         -rw- rw尸r- - 1 chris chris   3656 Sep 29 15: 39 ixdp425-setup. c
         -rw- rw-r- - 1 chris chris   2761 Sep 29 15: 39 Kcoflfig
          rw- rw-r- - 1 chris chris    259 Sep 29 15: 39 Makefile
         -rw- rw-r- - 1 chris chris   3102 Sep 29 15: 39 prpmcllOO-pci. c



       ［리스트 午4］에 나오는 파일 중에는 다른 디렉터리에도 공통적으로 존재하는 Makefile과
       KConfig 파일을 볼 수 있다. 이 두 개의 파일은 각각 커널 빌드 구성 및 빌드 과정을 다루는
       파일이다. 그럼 이것들이 어떻게 동작하는지 알아보자．
                                                 다른 관점에서 본 리눅스 커널     Chapter 4




    4.3 커널 빌드 시스템1
          리눅스 커널을 구성하고 빌드하기 위한 시스템도 상당히 복잡한데 , 당연히 600만 라인 이상
          의 코드를 가진 소프트웨어를 빌드해야 하기 때문이다！ 이 절에서는 빌드 환경을 자신에게
          맞게 수정해야 하는 개발자를 위해서 커널 빌드 시스템의 기본척인 부분에 대해서 살펴보도
          록 하자．

          최신의 리눅스 커널을 내려 받으면 커널 소스 트리 내에 800개 이상의 makefile17）이 있는
          것을 볼 수 있다. 이 숫자가 좀 많다고 생각될 수도 있지만, 빌드 시스템의 동작 원리와 구조
          를 이해하고 나면 그리 많은 것은 아니라고 느끼게 될 것이다. 리눅스 커널 빌드 시스템은
          리눅스 2.4와 그 이전 버전부터 지금까지 상당 부분 업데이트되었다. 이전의 빌드 시스템에
          익숙한 사람들은 새로운 Kbuild 시스템이 기존 시스템에 비해서 엄청나게 개선되었다는 것을
          알 수 있을 것이다. 여기서는 논의를 Kbuild에 기반해서 빌드되는 커널로만 제한하도록
          하자．


    4.3. ] 잠Conf油 파일
          앞에서도 이야기했듯이 , 젬config 파일은 리눅스 커널 이미지를 빌드하는 데 기본적인 청사
          진 역할을 하는 구성 파일이다. 리눅스 프로젝트를 처음 시작하려고 할 때 자신의 임베디드
          플랫폼에 맞도록 알맞은 구성을 하기 위해서는 많은 노력이 필요할 것이다. 커널 구성을 변
          경하기 위해서 사용할 수 있는 툴은 텍스트 방식과 GUI 방식 몇 가지가 있다. 원하는 구성을
          마친 후에는 그 결과가 리눅스 소스 최상위 디렉터리에 . config라는 이름의 파일로 처장되
          어 커널 빌드 과정을 결정하계 된다．

          커널 구성을 마치는 데 상당한 시간을 투자했을 것이기 때문에 , 이 구성 설정 값들을 날리지
          않도록 잘 보호해야 한다. 몇 가지 make 명령어는 사전 경고 없이 이 구성 파일을 지워버린
          다. 가장 흔한 경우로 make mrproper가 있다. 이 make 타킷은 커널 소스 트리를 어떤 값
          도 설정되지 않은 원래의 상태로 되돌리는 일을 한다. 이 과정에서 소스 트리 내의 모든 구성
          데이터를 지우고, 물론 .config 파일도 삭제한다．


    17) make!如들約］ 모두 직접적으로 빌드 과정에 관여하는 것은 帥니다. 예를 들어, 어떤 파일은 빌드와 관련된 문서를 제공하기 위
      흐｝ 것도 있다．


                                                                           125 1
1
          Embedded Linux Primer




        알다시피 리눅스에서 점으로 시작하는 파일명은 숨김 파일을 나타낸다. 이런 중요한 파일이
        숨김 파일 형태로 되어 있는 것은 불행한 일인데 , 이 때문에 많은 개발자들이 상당한 아픔을
        겪었다. 만약에 독자도 . config 파일의 사본을 복사해 놓지 않은 채로 make mrproper
        명령을 실행하면 똑같은 아픔을 나눌 수 있을 것이다（주의 사항 - . config 파일을 미리 백
        업해 둘 것n.

        이 . config 파일은 간단한 형식을 갖는 선언문들로 이루어져 있다. ［리스트 午5］에 최신
        커널 버전에서 발췌한 .config 파일의 일부분을 보여 주고 있다．

        ［리스트 4-5] 리눅스 2.6의 . conf由 파잎의 일부



          # USB support
          #
          CONFIG_USB=m
          # CONFIG－七USB_DEBUG is not set



          # Miscellaneous USB options
          #
          CONFIG_USB_DEVICEFS=y
          # CONFIG_USB_BANDWIDTH is not set
          # CONFIG_USB_DYNAMIC_MINORS is not set


          # USB Host Controller Drivers
          #
          CON FIG_USB_EHCI_HCD=m
          # CONFIG_USB_EHCI_SPLIT_ISO is not set
          # CONFIG_USB_EHCI_ROOT_HUB_TT is not set
          CON FIG_USB_OHCI_HCD=m
          CONFIG_USB_UHCI_HCD=m




        이 . config 파일을 이해하기 위해서는 리눅스 커널의 기본적인 부분을 이해해야 한다. 리
        눅스는 모놀리식（monolithic）한 구조를 갖는다. 그 말은, 커널 전체가 정적으로 링크된 하
        나의 실행 파일 형태로 컴파일 및 링크된다는 것이다. 하지만 소스의 일부를 하나의 오브젝
        트 모듈로 컴파일한 후 중분 링크伽cremeritally link)18）해서 실행중인 커널에 동적으로 삽입할


I 126
                                              다른 관점에서 본 리눅스 커널    Chapter 4



       수 있도록 하는 것도 가능하다. 이 방법이 대부분의 디바이스 드라이버를 지원하기 위해서
       일반적으로 사용되는 방법이다. 리눅스에서는 이것들을 적재 가능한 모듈佃adable module하이
       라고 부른다. 또는 그냥 디바이스 드라이버라고 부르기도 한다. 커널이 부팅된 후에 , 어떤
       특수한 응용 프로그램이 실행되어 적재 가능한 모듈들을 커널에 삽입하는 일을 수행한다．

       그럼 이런 사전 지식을 가지고, ［리스트 4-5］를 다시 보도록 하자. 이 구성 파일（.config)
       의 내용은 USB 서브시스템을 설정하는 부분을 보여 주고 있다. 첫 번째 설정 옵션인
       CONFIG USB = m은 USB 서브시스템을 커널 구성에 포함시킬 것이고, 동적으로 적재 가능한
       모듈（=m）로 컴파일되고, 커널이 부팅퇸 후에 필요 시에 때때로 커널에 적재될 것이라는 의미
       이다. 선택할 수 있는 다른 옵션으로는 =y가 있는데 , 이는 USB 모듈을 컴파일해서 커널 이
       미지의 일부로서 정적으로 링크되도록 한다. 그 작업의 결과가 최종적으로는 ［리스트 4-3)
       과 ［그림 十1］에서 본 . . . /drivers/built-in.o 파일로 통합되는 것이다. 빈틈 없는 독
       자라면 드라이버를 적재 가능한 모듈로 설정한 경우에는 커널 본체에는 그 코드가 포함되지
       않고, 나중에 독자적인 오브젝트 모듈로, 즉 적재 가능한 모듈로 존재하면서 부팅 후 실행중인
       커널에 동적으로 삽입된다는 것을 알 수 있을 것이다．

       ［리스트4中5］에서 CONFI（乞USE DEVICEFS=y로 선언되어 있는 것을 한번 살펴보자. 이 옵
       션은 약간 다른 방식으로 동작하는데 , 이 경우의 USE DEVICEFS（구성 옵션들은 보통 축약
       형으로 표현한다）는 별도로 존재하는 모듈이 아니고, USB 드라이버 내부의 어떤 기능을 활
       성화할 것인지 하지 않을 것인지를 결정하는 옵션이다. 다시 말해 커널 본체에 컴파일된 모
       듈을 포함시키라는 의미（=y）로 사용된 것이 아니다. 대신 전체 USB 드라이버 모듈 안에서
       추가적인 오브젝트 모듈들 을 포함시키도록 해서 USB 모듈 내부에 하나 또는 그 이상의 기능
       을 추가하는 용도로 사용되었다. 이 파일 내용만으로는 잘 구별되지 않지만 보통은 구성 편집
       기의 도움말 문자열이나, 편집기에 표시되는 체계만 봐도 그 차이를 쉽게 알 수 있을 것이다．


4.3.2 구성 편집기
       초기 커널은 명령에 라인（command line）에서 동작하는 간단한 스크립트를 이용해서 커널
       을 구성했었다. 이는 상대적으로 훨씬 적은 수의 구성 옵션을 가진 초기 커널이라고 해도 상
       당히 귀찮은 작업이었다. 이 명령에 라인 방식은 아직도 사용할 수 있지만, 사용해 보면 아무

18) 증분 링크는 다른 오브젝트어］ 다시 링크될 수 있는 오브젝트 모듈을 생성하는 기술이다. 이 방법으로 링크 후히1 주소 값이 결
    정되지 않은 심볼들이 있어도 에러가 나지 않고， 1:4昏1] 디른 오브젝트어］ 링크될 때 해당 심볼들의 주소 값들이 결정되는 것이
  다．
                                                                        127 1
  難 ml     Embedded Linux Primer




         리 좋게 생각하려 해도 매우 지루한 작업일 수밖에 없다. 이 방식으로 일반적인 최신 커널을
         구성하기 위해서는 명령 프롬프트 상에서 600개 이상의 질문에 답해야 한다. 매번 선택할
         값을 입력하고 (Enter）키를 눌러야 한다. 더군다나 도중에 실수라도 하게 되면 되돌릴 방법
         이 없어서 , 처음부터 다시 해야 한다. 599번째 질문에서 실수하면 한없는 좌절감을 느끼게
         될 것이다！

         그래픽 인터폐이스가 없는 임베디드 시스템 상에서 커널을 빌드하는 것과 같은 일부 경우에
         는 명령에 라인 방식의 구성 유틸리티를 쓸 수밖에 없다．

         커널 소스 구성을 위한 서브시스템은 몇 가지 그래픽 방식의 프론트엔드19) (front- end :
         전단）를 사용한다. 실제로, 최신 리눅스 커널은 커널 구성을 위한 타깃을 10개나 가치고 있
         다. 다음 항목에 그 타깃들을 정리했는데 설명은 make help의 도움말 내용을 그대로 가져
         온 것이다．

          口 config : 명령에 라인 기반 프로그램을 이용해써 현재 구성을 업데이트한다．

          口 menuconfig : 메뉴 방식의 프로그램을 이용해써 현재 구성을 업뎨이트한다．

          口 )<config : QT 기반의 프론트 엔드를 이용해서 현재 구성을 업뎨이트한다．

          口 gconfig : GTK 기반의 프론트 엔드를 이용해써 현재 구성을 업데이트한다．

          口 oldconfig : 기존의 . Co址培를 기본으로 현재 구성을 업데이트한다．

          口 randconfig : 모든 옵션에 임의의 값을 넣은 새로운 환경

          口 defconfig : 모든 옵션에 기본 값을 넣은 새로운 환경

          口 allmodc（丑ifig : 가능한한 모듈 방식을 설정하도록 하는 새로운 환경
          口 allyesconfig : 모든 옵션을 예（yes）로 설정한 새로운 환경
          ［그 allnoconfig : 최소한의 옵션을 설정한 새로운 환경

       리스트에 나와 있는 makefile의 처음 4개의 타깃은 설명에도 나와 있듯이 일종의 구성 편집
       기를 실행시킨다. 지면 관계상 여기서는 GTK 기반의 그래픽 프론트 엔드에만 초점을 맞춰
       서 설명하도록 하겠다. 물론 다른 구성 편집기를 이용해도 같은 일을 할 수 있다는 것은 알아
       두기 바란다．


19) （역자주） 프론트1엔드（젼딘） : 사용자와 최종적으로 상호 작용하는 부분을 프론트엔드라고 한다. 반대말은 빡엔드이다．


1128
                                                                                             다른 관점에서 본 리눅스 커널    Chapter 4



        커널 소스의 최상위 디렉터리에서 make gconfig 명령을 입력하면 커널 구성을 위한 편집
        기20）를 실행할 수 있다. ［그림 午2］에는 gconfig가 실행되었을 때 개발자에게 보여 주는
        커널 설정 항목들의 최상위 메뉴 화면을 나타낸 것이다. 자신에게 맞게 커널 구성을 변경하
        기 위해서 이 메뉴를 시작으로 모든 설정 값들에 접근할 수 있다．

            E恥   Qptioris    姓叫口

              渤 ：그 目               I        II   E;          미1      骨
                      Load Save Sir)이C Sp奴 F너rCollapse Eripand

            Options                          Name N M YValue
              Co挺 matuety level options
            r, General setup
         b Loadatden恤1施S叩附r
        4) System Ty口e
            11 Bus support
        二

        沁 K叫C叫 Features
        !b Booto骨沁Cs
        小 듸oatln叩机m岫帥on
        小 Use四pace tdnary 幻rma注
        三b P口帥F manaqemem畔油Ins
       拉 Ne汭or蜘9
        :1. ［沁mc色 0區ness
        1. F加돠針ems
                                                                                                            Y
                                       mm   m         mn   mmn小md뇨二心小m如mmm   mmmm싸n艸mmmH如m    mm小m   mmmm
        7 Code maturity level options




       I 그림 午2 커널 구성을 위한 최상위 메뉴


       구성 편집기를 종료하면 저장할 것인지를 묻는다. 저장하겠다는 메뉴를 선택하면 전역 구성
       파일인 .config가 업데이트된다（만약 존재하지 않으면 새로 만든다）. 이전에 설명한
       .config 파일은 최상위 makefile을 통해서 커널 빌드 과정을 결정하게 된다. 이 makefile
       에서 include 구문을 이용해서 .config 파일이 직접 포함하는 것을 알 수 있다．

       대부분의 커널 소프트웨어 모듈들 또한 .config 파일을 통해서 커널 구성 내용을 간접적으
       로 읽어 들인다. 빌드 과정에서 . config 파일의 내용은 적절한 변환 과정을 거쳐서
       . . ./include/ linux 디렉터리에 C 헤더 파일로 만들어지는데, 그 파일이 autoconf . h
       이다. 이 파일은 자동으로 생성되는 파일이고, 매번 구성 편집기를 실행할 때마다 새롭게 만
       들어지기 때문에 절대로 파일을 직접 수정하면 안 된다. 커널의 많은 소스 파일들이
       #include 전처리21) 지시자（directive）를 이용해서 직접적으로 이 파일을 포함시킨다.

20) 커널 구성을 위한 편집기는 자신이 원하는 것을 사용할 수 있다. 예를 들어, make con如나 make menuc岫g
                                                                                                                등을 이용해서 다
  른 빙식의 편집기를 사용할 수 있다．
  」   U.      Embedded Linux Primer




           ［리스트 4-6］은 전에 살펴본 USB 예제와 관련된 옵션들이 헤더 파일의 일부로 변환된 것을
           나타낸 것이다. 이전 USB 예제에서 설명한 . config 파일에 있던 모든 항목이 autoconf.
           h 파일의 항목으로 만들어진 것을 유의하자. 이를 통해서 커널 소스 파일들이 커널 구성 설정
           값을 참조할 수 있게 된다．

           ［리스트 4-6] 리눅스 autoconf . h


              ／出
                   六 USB suppo八
                   士／
              #define CONFIG_USB_MODULE 1
              #undef CONFIG. USBHDEBUG

              ／出
                   * Miscellaneous USB options
                   央／
              #define CONFIG그JSB. DEVICEFS 1
              #undef CONFIG_USB1BANDWIDTH
              #undef CONFIGHUSB_DYNAMIC_MINORS


              1*
                   * USB Host Controller Drivers
                   士／
              #defi ne CONFIGHUSB_EHCIHHCD. MODULE 1
              #undef CONFIGHUSBeEHCIeSPLIT_ISO
              #undef CONFIG. USBeEHCI_ROOTmHUBUTT
              #defi iie CONFIG_USB_OHCI_HCD_MODULE 1
              #defi ne CONFIG_USB_UHCI1HCDMODULE 1




           아직 안 해봤다면 커널 소스 최상위 디렉터리에서 make gconfig를 실행해 보자. 그리고
           구성 편집기가 가지고 있는 많은 하위 세부 항목들과 설정 옵션들을 한번 둘러보기 바란다．
           구성 편집기에서 명시적으로 설정을 처장하지 않는한 구성 편집기를 종료하면 방금 변경한
           구성들이 모두 사라지기 때문에 커널 구성이 바뀌는 부분에 대해서는 걱정하지 않아도22) 된
           다. 구성 설정을 위한 많은 파라미터 항목들이 자신의 다른 설정 옵션에 대한 설명 문구를
           제공해서 사용자의 이해를 돕고 있다．

21) （역자주） 전처리 (preprocess) : 소스 파일이 컴파일되기 전에 흐｝ 번 처리를 거치기 때문＜내 '전처리'라고 하펴, #define, 術f 등의
    지시자들을 이용한다. 이들은 컴파일 과정 이젼어｝ 모두 처리된다．
22) 만일을 위해 기존의 . config 파일을 백업해 두는 것도 좋은 생각이다．
                                                   다른 관점에서 본 리눅스 커널         Chapter 4




4.3.3 Makefile 타깃
     커널 소스가 있는 최상위 디렉터리에서 make help를 입력하면 소스 트리로부터 만들 수 있
     는 타깃의 목록을 보여 준다. make를 사용하는 가장 흔한 방법은 그냥 아무런 타깃 명도 입
     력하지 않는 것이다. 그렇게 하면 커널 ELF 파일인 vmlinux 파일과 선택된 아키텍처에
     맞는 기본 바이너리 이미지가 만들어진다（예를 들어 , x86에서는 bz Image가 만들어진다）.
     또한 make에 아무런 타깃을 입력하치 않으면 구성 파일에 모듈（적재 가능한 모듈）로 명시된
     모든 디바이스 드라이버들도 빌드하게 된다．

     다양한 아키텍처 및 여러 종류의 머신들은 각각 자신에게 맞는 바이너리 타깃을 필요로 하는
     데 , 아키텍처들을 위한 타깃 이름으로 공통적으로 많이 사용되는 것으로는 z Image?下 있다．
     여러 아키텍처에서 zlmage라는 타깃 이름을 해당 임베디드 시스템에 로드하고 실행될 수
     있는 기본 타깃 이름으로 사용한다. 초보 개발자가 혼히 하는 실수 중의 하나가 make에 타깃
     으로bzlmage를 입력하는 것인데 , bzlmage는 x86/PC 아키텍처서만 사용할 수 있는 타깃
     이다. 널리 알려진 내용과는 반대로, bzlmage는 bzip2로 압축된 이미지가 아니다. 기존
     PC 아키텍처에 대한 세부 사항까지 들어갈 필요 없이 , bzlmage?} 단지 표준 PC 방식의
     BIOS를 가진 PC계열 머신에만 알맞은 타깃이라는 점만 염두에 두도록 하자．

     ［리스트 4-7］은 최신 커널에서 make help를 입력한 결과 출력되는 내용을 보여 주고 있다．
     이 항목에서 리눅스 커널 makefile을 이용해서 만들 수 있는 타깃이 매우 많은 것을 볼 수
     있다. 각 항목과 함께 그에 맞는 간단한 설명이 같이 표시된다. 중요한 점은 make의 help
     타깃（make help）도 아키텍처 종속적인 타깃이라는 것이다. make를 실행시킬 때 명시하는
     아키텍처에 따라서 그에 맞는 아키텍처 종속적인 타깃들의 목록이 나타나게 되는 것이다．
     ［리스트 4-7］은 make 명령에 라인에서 볼 수 있듯이 ARM 아키텍처로 설정해서 실행시킨
     결과물을 보여 주고 있다．

     ［리스트 午7) Make川e의 타깃들


       $ make ARCH=arm help
       Cleaning targets:
         clean        - remove most generated files but keep the config
         mrproper     - remove all generated files + config + various backup files

       configuration targets:



                                                                                     131
   出a   Embedded Linux Primer



          config       - update current config utilising a line-oriented program
          menuconfig   - update current config utilising a menu based program
          xconfig      - update current config utilising a QT based front-end
          gconfig      - update current config utilising a GTK based front-end
          ol dconfi g  - update current config utilising a provided .config as base
          randconfi g  - New config with random answer to all options
          defconfi g   - New config with default answer to all options
          allmodconfig - New config selecting modules when possible
          allyesconfig - New config where all options are accepted with yes
          al ] noconf伯 - New minimal config

        other generic targets:
          all               - Build all targets marked with [*]
        出 vmli flux         - Build the bare kernel
        卉 mo山iles           - Build all modules
          modules_install   - Install all modules
          dir!              - Build all files in dir and below
          dir/ file. [ois]  - Build specified target only
          dir/ file. ko     - Build module including final link
          rpm               - Build a kernel as an RPM package
          tags/TAGS         - Generate tags file for editors
          csc야）e            - Generate cscope index
          kernel release    - output the release version string

        Static analysers
         buildcheck             - List dangling references to vmlinux discarded sections and
                                  mnit sections from non-mnit sections
          checkstack            - Generate a list of stack hogs
          namespacecheck        - Name space analysis on compiled kernel

        Kernel packaging:
          rpm-pkg               - Build the kernel as an RPM package
          L너 nrpm- pkg          - Build an rpm package containing the compiled kernel
                                  and modules
        deb- pkg                - Build the kernel as an deb package
          tar- pkg              - Build the kernel as an uncompressed tarball
          targz- pkg            - Build the kernel as a gzip compressed tarball
          tarbz2- pkg           - Build the kernel as a bzip2 compressed tarball

        Documentation targets:
         Linux kernel internal documentation in different formats:
         xmldocs (XML DocBook) , psdocs (Postscript) , pdfdocs (PDF)



1132
                                          다른 관점에서 본 리눅스 커널        Chapter 4



   htmldocs (HTML) , mandocs (man pages, use instailmandocs to install)
Architecture specific targets (arm) :
* zlmage        - Compressed kernel image (arch/arm/boot/zimage)
  Image         - uncompressed kernel image (arch/arm/boot/Image)
* xiplmage      - XIP kernel image, if configured (arch/arm/boot/ xiplmage)
  bootplrnage   - Combined zlmage and initial RAM disk
                   (supply initrd image via make variable INITRD=<path>)
  install       - Install uncompressed kernel
  zinstall      - Install compressed kernel
                  Install using (your) -/bin/installkernel or
                   (di stri bution) /sbi n/install kernel or
                  install to $(INSTALL_PATH) and run lilo
  assabet_defconfig              - Build for assabet
  badge4_defconfig               - Build for badge4
  bast_defconfig                 - Build for bast
  cerfcube中defconfig             - Build for cerfcube
  c1ps7500_defconfig             - Build for c1ps7500
  collie_defconfig               - Build for collie
  corgi_defconfig                - Build for corgi
  ebsallO_defconfig              - Build for ebsallO
  edb72ll_defconfig              小 Build for edb72ll
  enp26ll_defconfig              - Build for enp26ll
  ep80219_defconfig              - Build for ep80219
  epxalOdb_defconfig             - Build for epxalOdb
  footbridge_defconfig          - Build for footbridge
  fortunet_defconfig            - Build for fortunet
  h3600_defconfig               - Build for h3600
  h7201_defconfig               - Build for h7201
  h7202_defconfig               - Build for h7202
 hackkit_defconfig              - Build for hackkit
 integrator_defconfig           - Build for integrator
 iq31244_defconfig              - Build for iq31244
 iq80321_defconfig              - Build for iq80321
 iq80331_defconfig              - Build for iq80331
 iq80332_defconfig              - Build for iq80332
 ixdp2400_defconfig             - Build for ixdp2400
 ixdp2401_defconfig             - Build for ixdp240l
 ixdp2800_defconfig             - Build for ixdp2800
 ixdp280l_defconfig             - Build for ixdp2801
 ixp4xx小defconfig               - Build for ixp4xx
 jornada720_defconfig           - Build for jornada720
 lart_defconfig                 - Build for lart
 1pd7a400_defconfig             - Build for 1pd7a400



                                                                      133 釜
1     Embedded Linux Primer



        1pd7a404_defconfi g          Build for 1pd7a404
        1ubbock_defconfi g           Bui Id for lubbock
        1usi 7200_defconfi g         Bul Id for lusl 7200
        mai nstone_defconfi g        Bui Id for mai nstone
        mxlads_defconfi g            Bui ld for mxlads
        neponset_defconfi g          Bui ld for neponset
        netwinderjiefconfig          Build for netwinder
        omap小乙1610_defconf杓          Bui ld for omap1-h2_1610
        p1 eb_defconfi g             Build for p1 eb
        poodi e_defconfi g           Bui ld for poodle
        pxa2 55-i dp_defconfi g      Bui ld for pxa255戶i dp
        rpc_defconfi g               Build for rpc
        s3c2410_defconfi g           Bui Id for s3c2410
        shannon_defconfi g           Bui ld for shannon
        shark_defconfi g             Bui ld for shark
        si mpad_defconfi g           Bui ld for simpad
        smdk2410_defconfi g          Bui ld for smdk2410
        spi tz_defconfi g            Bui ld for spitz
        versatile_defconfig          Bui ld for versatile



        make v=0I1 [targets] 0 => quiet build (default) , 1=> verbose build
        make 0=di r [targets] Locate all output files in "d卄", including . confi g
        make c=1 [targets] Check all c source with SCHECK (sparse)
        make C=2    [targets] Force check of all c source with SCHECK (sparse)

      Execute "make" or "make all " to build all targets marked with [*]
      For further info see the ./README file



    위 타깃 중의 상당수는 실제로 거의 사용되치 않을 것이다. 하지만, 어떤 것들이 있는지 알아
    두면 도움이 될 것이다. ［리스트 午끼에서 볼 수 있듯이 , 별표什）로 시작하는 타깃은 아무것도
    기술하지 않을 경우에 기본적으로 빌드되는 타깃이다. 그리고 이름이 defconfig로 끝나는
    타깃들을 한 번 보자． 이 타깃들은 커널 구성의 기본 값을 구성 (default configuration）하
    기 위한 것이다. 4.2.2절 "커널 컴파일하기"에서 커널 소스 트리를 원래의 아무것도 구성되지
    않은 상태로 되돌리는 명령어를 상기해 보면 make 명령어에 아키텍처와 기본 값 구성 타깃
    을 명시해서 실행했었다. 그때 사용한 기본 값 구성 타깃이 앞의 ARM 타깃 항목 중에서 볼
    수 있는 ixp4xx defconfig이다. 비슷하게 다른 타깃들도 각자 해당하는 커널 배포판과
    아키텍처를 위한 기본 값 구성 타깃이라는 것을 알 수 있다．
                                                   다른 관점에서 본 리눅스 커널        Chapter 4




4.3.4 커널 구성
          Kconfig（또는 Kconfig . ext오｝ 같이 비슷한 이름에 확장자가 붙은 파일）는 거의 300개에
          딜하는 커널 내 하위 디렉터리에 존재한다. Kconfig는 자신이 위치하고 있는 디렉터리와
          그 하위 디렉터리 안에 포함된 기능들을 구성하기 위한 파일이다. Kconfig 파일의 내용은
          커널 구성을 담당하는 서브시스템에 의해서 파싱23）되는데 , 서브시스템은 이 내용을 토대로
          사용자에게 선택할 수 있는 항목들로 나타내 주는 것이다. 또한 Kconfig에는 구성 파라미
          터들을 위한 도움말 문구도 포함하고 있다．

          커널 빌드 구성을 위한 （전에 소캐한 gconf와 같은） 유틸리티는 arch 디렉터리의 하위 디
          렉터리의 Kconfig 파일을 시작으로 해서 Kconfig 파일들을 모두 읽어 들인다. 이는 다음
          내용과 같이 Kconfig의 makefile24）로부터 실행된다．



               gconHg: $(obj) /gconf
                     $< arch/ $(ARcH) /Kconfig




          빌드하는 아키텍처가 어떤 것인지에 따라서 , 아兀nf는 해당 아키텍처의 Kconfig 파일을 읽
          어 들여서 최상위 구성 값들을 정의하는 데 사용한다. Kconfig 파일에는 다음과 같은 내용
          이 몇 줄 포함되어 있을 것이다．

               source    "drivers/pci /Kconfi g"


          위 구문은 구성 편집기가 커널 소스 트리의 다른 위치에 있는 다른 파일을 가져오게 한다．
          아키텍처별로 이런 Kconfig 파일을 여러 7겪 가지고 있다. 이들이 모두 모여서 사용자가 커
          널을 구성할 때 표시되는 일련의 옵션 메뉴들이 구성되는 것이다. 각각의 Kconfig 파일은
          소스 트리의 다른 곳에 있는 Kconfig 파일을 자유롭게 포함할 수 있다. 구성을 위한 유틸리
          티（이 경우는 gconf）는 서로 연결된 Kconfig 파일들을 재귀적 (recurs押e）으로 읽어서 구
          성을 위한 메뉴 구조를 생성하게 된다.




23) （역자주） 파싱 (parsing : 구문 분석） : 컴퓨터 및 모듈이 어떤 문법을 분석하고 이해하는 것을 파싱이라고 한다．
24) （역天阡） ...／없:ript瓜conflg/Makefi1e



                                                                                '35I
   難a     Embedded Linux Primer



        ［리스트 十8］은 ARM 아키텍처에 해당하는 Kc（그nfig 파일들을 트리 구조로 일부 표현한
        것이다. 여기서 참조한 최신 버전의 리눅스 커널 2.6 소스 트리는 커널 구성을 위한 170개의
        분리된 Kconfig 파일을 가지고 있다. 명확한 이해를 위해서 목록의 대부분이 생략되었지
        만, 전체적인 구조를 보여 주기 위해서 나타낸 것이다. 항목을 모두 나열하면 수 페이지는
        족히 차지할 것이다．

        ［리스트 4-8) ARM 아키텍처의 Kconf由 파일 목록의 일부

          arch/arm/Kconfig <<<<<< (최j위 Kconfig)
            I-> init/ Kconfig
              1
              I-> arch/arm/mach-i op3xx/Kconfi g
              I-
                   >           arch/arm/mach-ixp4xx/Kconfig
              1
              I-> net/Kconfig
              1   卜> net/ipv4/Kconfig
                  1    I-> net/ipv4/ipvs/Kconfig
              1
              I-> drivers/char/Kconfig
              I   I-> drivers/serial/Kconfig

            I-> drivers/usb/Kconfig
            I   I-> drivers/usb/core/Kconfig
            I   I-> drivers/usb/host/Kconfig
            1      .   .   .




            卜> lib/ Kconfig



       ［리스트 千8］을 보면 arch/arm/Kconfig 파일은 다음의 한 줄을 포함하고 있다．

          source "net/Kconfig"


        파일 ne七／Kconfig는 다시 다음과 같은 내용을 포함하고 있다．

          source "net/作v4/Kconfig"

          1：二 1=




1136
                                                                                다른 관점에서 본 리눅스 커널    Chapter 4



     이전에도 언급했듯이 , 이 Kconfig 파일들이 모두 모여서 구성 메뉴 구조를 결정하케 되고，
    사용자가 커널을 구성하고자 할 때 이 구성 옵션들을 보여 주게 된다. ［그림 全3］은［리스트
    午8］의 파일들을 이용해서 ARM 아키텍처를 위한 구성 유틸리티 (gconf）가 실행되는 모습
    이다．

        E如     會}11｛가is    H帥）

           渤 ｛스 目                  f       H    는       口m   中
          吼
          『ck Load Save Single Split Eull Collapse Expand

         O的며l5                                                   N카ne              N M Y V궤ue
         t, Code niaturity level options
        卜 Cener刈 sett坦
        b 山ad砒昶 mod뗘axe햐a가t
        口 Syst因n Type
           口 口ARM system type (NE｝的                                                        RiscPC
                 0 Gnus.CL-PS750俳E (NE瑚                          ARCH.파PS7500      N   - 卜1
                 0 CLPS7U町EP721斗based們E빠                         ARCI-LCIJ'S7i1X   N   -   N
    膏            O야印SAl爵們E硼                                      ARCI-LCO285       N   - N
    "            0 ERSA皿0 (NE빠                                   ARCH느EBSA1I0      N   느 卜L
                 0 Epxalck杓們C｝帥                                  ARCI乞CAMELOT      N   -   N
                 0 Fo心Bed恥 (N드W)                                 ARCH_F心OThR以EN        _ N
                 O岫呵如r (NEWy                                     ARC比町ECMTOR N         - N
                 0 l아저xx-based (NEW)                             ARCI-IJOP3XX      N   _ N
        Sorry, no help available b0r this option yet.




    I 그림 4-3 gconf 설정 화면



4.3.5 구성 옵션 직접 만들'I
    많은 임베디드 개발자들이 자체 제작한 자신만의 하드웨어를 치원하기 위해서 리눅스 커널에
    별도의 치원 항목을 추가하는데 , 이것의 가장 흔한 경우 중의 하나는 여러 버전의 하드웨어
    플랫폼을 가지고 있어서 커널 소스 트리에서 컴파일 시점에 각각의 하드웨어 플랫폼에 따라
    다른 옵션을 설정해야 하는 경우를 들 수 있다. 각 하드웨어 버전에 따라서 분리된 버전의
    커널 소스 트리를 갖는 대신에 , 어떤 기능을 활성화하기 위한 구성 옵션 항목을 추가하는 방
    법을 이용하는 것이다．

    이전 단락에서 설명한 구성 관리를 위한 아키텍처를 이용해서 쉽게 자신만의 구성 항목을 만
    들고 추가할 수 있다. 그리고 전형적인 Kconfig 파일의 내용을 한번 들여다보면 구성 스크
    립트 언어의 구조를 살펴볼 수 있다. 예를 들어 , IXP425 통신용 프로세서를 이용하는 하드


                                                                                                        137 量
 難U      Embedded Linux Primer




       웨어 플랫폼이 두 7뀨 있다고 가정하자. 그리고 기술팀에서 각각에 베가（Vega）와 성운
       (Constellation）이라는 이름을 붙였다고 하자. 그리고 각 보드는 커널이 부팅되는 과정에서
       반드시 초키화시켜야 하는 특수한 장치를 가지고 있다고 하자. 이때 커널 구성 과정에서 7가
       발자에게 보여 주는 옵션 메뉴에 이 보드들을 위한 구성 옵션을 추가하는 것이 얼마나 간단한
       지 한번 보도록 하자. ［리스트 士9］는 ARM 아키텍처의 최상위에 있는 Kconfig 파일의
       일부분을 나타낸 것이다．

       ［리스트 4-9] . . ./arch/arm/Kconf伯 파일의 일부


          source "in卄/KconHg"

          menu "System Type"

          choj ce
                    prompt "ARM system type "
                    default ARCH_RPC

          config ARCH_CLPS7500
                 bool "Ci rrus-CL-PS7500FE "



          config ARCH_CLPS711X
                 bool "CLPS711x/EP721x- based'




          source 'arch/ arm/mach-ixp4xx/Kconfig




       ARM 아키텍처의 최상위 Kconfig 파일의 일부를 나타낸 위 리스트를 보면 System Type
       이라는 메뉴 항목이 정의된 것을 알 수 있다. ARN sys七em type이라는 prompt 구문 이후
       부터 ARM 아키텍처와 관련된 선택 항목의 리스트들이 나오는 것을 볼 수 있다. 그리고 파일
       의 뒷부분에서 IXP4xx를 위한 Kconfig 파일을 포함시키고 있다. 바로 이 파일에 새로운
       구성 항목들을 추가하도록 하자. ［리스트 全10］에 이 파일의 내용을 나타냈다. 여기서도 가
       독성을 위해서 불필요한 내용은 생략 기호를 이용해서 모두 생략했다．




p138
                                                   다른 관점에서 본 리눅스 커널      Chapter 4



      ［리스트 4-10) arch/arm/mach-ixp4xx/Kconfig 파일의 일부분


         menu "Intel IXP4xx Implementation Options "



         comment "IXP4xx platforms "



         config ARCH_AVILA
                 bool "Avila"
                help
                 Say 'Y ' here if you want your kernel to support. . .

         confi g ARCH_ADI_COYOTE
                  bool "Coyote"
                help
                  Say 'Y ' here if you want your kernel to support
                 the ADI Engineering Coyote. . .

          # （여기가 새로 추가된 옵션들）
          config ARCH_VEGA
                 bool "Vega"
                help
                 Select this option for "vega" hardware support



          config ARCH_CONSTELLATION
                  bool "Constellation"
                 help
                  Select this option for "Constellation"
                  hardware support




      ［그림 +4］는25) gconf 유틸리티를（make ARCH=arm gconfig 명령을 통해） 실행시켰을
      때 수정한 내용이 반영된 것을 보여 주고 있다. 간단한 수정 결과, 구성 편집기에 새 하드웨
      어 플랫폼 두 개를 위한 옵션이 포함되었다. 잠시 후에 , 이 구성 옵션을 이용해서 어떻게 이
      새로운 보드를 위한 오브젝트 파일을 조건적으로 선택하는치 알아보자．

25) （그림 4-4）에서 ARM 시스템 타입 아래에 있는 많은 옵션과 JXP4XX의 구현 곤붚크 옵션들의 상당수를 그림 크기를 맞추기 위해
    편집했다．


                                                                               139 !
                        Embedded Linux Primer




          F；佃                Qpt佃1巧     I:如1n

                         ,         g孕 目       1   II 는    -       4L
                              Load Save Si,坦1e SF的t Ft쾨 Collapse Expand                  口나1:
                   兮，
          아lions                                                       Name              幷M]Y V出畦         唾
      m75y51em Ty1：咀                                                                                       斗m
                   口 口ARM system싸pa                                                               以P4xx-ba 』
                              O CIrrus心中S7500FE                        A旺比C나芍乃:to        N    _ N         !
              回XP4sx-baseci                                            ARCH_IXP4XX            Y '         !
              아XP2求XV2B0(工based                                        ARCHJXP?000       N    - N         唾
          ! 1mel 1XP4,oc Implementation Options                                                           灑
        i     iXP4xx F켜affom,s                                                                            1變
      ,::     口Avila                                                   ARC心V1LA          N    나 N         麾
      ,                       口C0yote                                  ARCH_Aol_COYOTE   N    -   N       壤
                              !1Ve！泉i                                  ARCH＼區GA               '! "Y           馨
      i                       口 Const메ation                            ARCH_CONSTELLATION N   -   N       隱
                              E IXDP425                                ARC比iXDP425       N    -   N       悟
      141                                                                                         洪m硅4乞
                   Viga AR거VEGA

      : Select this opti（甘1佃I Veqa' hm1出sat놘suppoll



      I 그림 4-4 직접 추가한 구성 옵션들


      구성 편집기를 （여기서는 gconf) 한 번 실행시켜서 자신만의 하드웨어 플랫폼을 지원하도
      록 하는 옵션을 선택하고 나면 전에 살펴본 . config 파일에 새로운 옵션을 나타내는 매크로
      들이 추가된다. 그리고 다른 모든 구성 옵션과 마찬가지로 커널 구성 옵션임을 표시하는
      CONFIG 로 시작하는 이름을 갖는다. 이번 경우에는 두 개의 구성 옵션이 새롭게 정의되는
      더］, 그상태가 . config에 저장되는 것이다. ［리스트4小11］에서 새로추가된 구성 옵션들을
      포함하고 있는 .config 파일의 내용을 볼 수 있다.

      ［리스트 午］1] 옵션이 추가된 . config 파일의 일부분



                        #
                        # IXP4xx Platforms
                        #
                        # C0NFIG_ARCH_AVILA is not set
                        # C0NFIG_ARCFLADI_C0Y0TE is not set
                        C0NFIG_ARCH_VEGA=y
                        # C0NFIG_ARCH_C0NSTELLATI0N is not set
                        # C0NFIG_ARCH_IXDP425 is not set
                        # C0NFIG_ARCH_ PRPMC1100 is not set




140
                                                     다른 관점에서 본 리눅스 커널         Chapter 4



     두 개의 새로운 옵션은 각각 베가（Vega）와 성운（Constellation) 하드웨어 플랫폼에 관련
     된 것이다. ［그림 午4］에서 보는 것처럼 베가를 선택하면 . confiq 파일에 새로 추가된
     CONFIG 옵션 중에서 베가 보드에 해당하는 옵션이 ' y' 값을 가치게 된다. 또한 성운에 해당
     하는 옵션은 선택하지 않은 것으로 기록된다．


4.3.6 커널 Makefile
     커널을 빌드시키면 入4ake1i1e은 저장된 구성 값들을 검색해서 그 설정 값에 따라서 어떤 하
     위 디렉터리를 찾아 들어갈지 , 어떤 소스 파일들을 컴파일할지를 결정하게 된다. 베가와 성
     운, 두 개의 자체 제작 하드웨어를 추가하는 작업을 마무리하기 위해서 , 새로운 항목을 추가
     한 구성 파일을 읽어 들이는 makefile을 찾아서 , 필요한 내용을 추가하도록 하자．

     이 예제에서는 특정 하드웨어를 위한 옵션을 다루고 있기 때문에 , 이 옵션에 따른 작업으로
     각각 vega se七up. c와 constellation setup. c 두 개의 하드웨어 셋업 모듈이 추가된
     다고 가정하자. 그리고 이 C 소스 파일을 . . . /arch/ arm/mach- ixp4xx 하위 디렉터리에
     두자. ［리스트 千12］는 이 디렉터리에 있는 II追kefile의 내용을 모두 나타낸 것이다．

    ［리스트 4-12) . . .larch/arm/mach나xp4xxx의 make州e


       #
       # Makefile for the linux kernel.
       #


       obj-y    += common. o common-pci .0



       obj-$(C0NFIG_ARCH_IxDP4xx)       += ixdp425- pci .o ixdp425- setup.o
       obj- $(coNFIG_MAcH_IxDPG425)     += ixdpg425-pci .0 coyote- setup. o
       obj- $(coNFIG_ARcI-i_ADI_coYoTE) += coyote-pci .o coyote- setup.o
       obj-$(C0NFIG_MACH_GTWX5715)     += gtwx5715-pci .0 gtwx5715- setup.o



    n追ke丘k이 무척 간단해서 놀랄 수도 있다. 이렇게 간단한 것은 커널 빌드 시스템이 많은
    복잡한 일들을 도맡아 처리하기 때문이다. 커널 빌드 시스템은 자신들의 하드웨어를 위한 지
    원항목들을 간단히 추가하고자 하는 경우가 대부분인 보통의 개발자들에게 매우 직관적26)
    이도록 설계되어 있다．
 難二S      Embedded Linux Primer




        자 그럼 n追kefile을 보도록 하자. 새로운 하드웨어의 초기화 작업을 추가하기 위해서 선택
        퇸 구성 옵션에 따라 어떤 일들을 해야 하는지 명확하게 알 수 있을 것이다. makefile 뒷부
        분에 간단히 다음 두 줄을 추가하자. 그럼 끝이다．



          Obj- $(CONFIG_ARCH_VEGA)   += vega_setup. o
          Obj- S (CONFIG_ARCH_CONSTELLATION)   += costellation_ setup. o




        이와 같은 절차를 통해서 자체 하드웨어를 초기화하는 모듈을 간단히 추가하는 것을 보았다．
        이제는 위와 비슷한 방식으로 커널 구성／빌드 시스템을 직접 수정할 수 있을 것이다．


4.3.7 커널 문서화
        리눅스 소스 트리에 대해서는 참고할 만한 자료가 아주 풍부하다. . . . /Documentation
        디렉터리 밑에 있는 42개의 하위 디렉터리에 거의 650개에 달하는 문서가 있기 때문에 전부
        다 읽어 보기는 어렵다. 그리고 이 문서들을 읽을 때 주의할 점이 있다. 커널 개발 및 릴리즈
        가 매우 빠르게 진행되기 때문에 관련된 문서들이 금방 철 지난 문서가 되는 경향이 있다．
        그럼에도 불구하고 이 문서들은 커널의 특정 서브시스템 또는 커널의 개념에 대한 기반 지식
        을 갖추기 위해서 참고할 수 있는 훌륭한 출발점이 될 것이다.

        어떤 리눅스 문서나 man 페이지의 가장 최신27) 버전을 찾기 위해서는 리눅스 문서화 프로
        젝트（Linux Documentation Project) 홈페이지 www.tldp.org에 자주 들리도록 하자．
        이 챕터의 마지막 부분의 "더 읽어 보기"에서도 참조하기 편하도록 리눅스 문서화 프로젝트의
        URL을 다시 한 번 표시했다. 이전의 논의에서 특히 홍미로운 부분은 Kbuild에 관련된 문서
        이다. 이 문서들은 . . . /Documenta七ion/kbuild 디렉터리에서 찾아볼 수 있다.




26) 실제로 커널 빌드 시스템은 매우 복잡햐다. 하지만 복잡성의 대부분은 보통 개발자들은 신경 쓰：仄］ 않아도 되도록 현명하게 숨
    겨져 있다. 그래서 빌드 시스템 젼문가가 되지 않고도 구성 항목을 추가, 제거, 수정하는 일은 상대적으로 아주 쉽다．
27) 항샹 문서보다는 기술이 먼저 발젼한디고 생각하자. 그렇기 때문께 문서를 명백한 사실로 이해하기보다는 일종의 지침서로 다
  루길 바랸다．


I 142
                                               다른 관점에서 본 리눅스 커널    Chapter 4



      구글（goo엎e）을 빼놓고는 커널 문서에 대해서 다 이야기했다고 할 수 없다. 조만간에 메리엄
      웹스터 (Merriam Webster) 사전에 구글링（G어灼ling）이라는 단어가 동사로 등장28）할 것이
      다！ 우리가 물어보고자 하는 많은 질문과 그에 해당하는 대답은 이전에 이미 다른 누군가어］
      의해서 행해진 경우가 많을 것이다. 인터넷에서 자신이 찾는 문제의 답을 찾으려면 검색에
      능숙해지기 위해서 시간을 좀 투자할 필요가 있다. 인터넷을 통해서 자신의 프로젝트나 문제
      점과 관련된 다양한 메일링 리스트나 유용한 정보로 가득한 저장소들을 찾을 수 있을 것이다．
      부록 E에서는 유용한 오픈 소스 리소스 목록을 볼 수 있다．



4.4 리눅스 커널 구하71
      일반적으로 자신의 하드웨어 플랫폼을 위한 임베디드 리눅스 커널을 구하는 방법은 세 가지
      가 있다. 첫째는 상업적으로 판매되는 임베디드 리눅스 배포판 중에서 알맞은 것을 구입하
      는 것이다. 둘째는 자신의 아키텍처와 프로세서에 맞는 무료 배포 버전을 구할 수 있으면
      찾아서 다운받는 것이다. 마지막 방법은 자신의 시스템과 가장 비슷한 오픈 소스 리눅스 커
      널을 구한 다음에 직접 포팅하는 것이다. 리눅스 포팅에 대해서는 16장, "리눅스 포팅"에서
      다룬다．

      자체 제작한 보드를 위해서 오픈 소스 커널을 포팅하는 것이 반드시 어렵지만은 않지만, 엔
      지니어링 및 개발 작업에 많은 자원 투자가 필요한 것이 사실이다. 이 방법은 무료 소프트웨
      어를 사용할 수 있는 장점이 있지만, 1장, "소캐"에서 이야기했듯이 개발 프로젝트에서 리눅
      스를 도입해서 활용하는 것은 무료하고는 거리가 좀 멀다. 최소한의 사양만을 필요로 하는
      작은 시스템에서도 리눅스 커널 외에 더 많은 요소들을 필요로 하기 때문이다．


4.4. ] 추가적으로 더 필요한 것은
      이번 장에서는 리눅스 커널 자쩨가 어떻게 조직되고 구성되어 있는지를 중점적으로 알아보았
      다. 이미 알고 있겠지만, 리눅스에 기반한 임베디드 시스템에서 리눅스 자체는 작은 일부 구
      성 요소에 불과하다. 리눅스 커널 외에도, 자신의 리눅스 탑재 제품을 개발하고, 테스트 및
      실행시키기 위해서는 다음과 같은 요소들이 필요하다．




28) （역자주） 현재는 웹스터는 물론이고 OXFORD 영어 사전 등에 goo蜘的］라는 동사가 이미 등록되어 있다．


                                                                         143 1
 好m   Embedded Linux Primer




      口 해당 하드웨어 플랫폼어］ 맞게 포팅 및 구성된 부트로더

      口 선택한 아키텍처를 위한 교차 컴파일러 및 관련 툴 체인

      口 하드웨어 아키텍처와 프로세서에 맞게 컴파일된 바이너리 실행 파일과 라이브러리 등의
         패키지들을 담을 파일 시스템

      口 보드상의 자체 디바이스들을 위한 디바이스 드라이버

      口 호스트 툴과 유틸리티를 포함한 개발 환경

      口 프로세서와 보드를 사용할 수 있는 리눅스 커널 소스 트리


   이 항목들은 임베디드 리눅스 배포판의 구성 요소이다．



4.5요약
      口 리눅스 커널은 10년 이상 지속적으로 발전해1 왔고, 이제는 많은 아키텍처를 잘 지원하는
         주류（main小stream) 운영체제가 되었다．

      口 리눅스 오픈 소스 홈페이지는 www. kernel. org이다. 리눅스 커널 1.0부터 지금까지의
         사실상 모든 리눅스 커널 버전을 여기서 구할 수 있다．

      口 리눅스 커널 이론 및 동작 원리에 대한 자세한 설명은 다른 좋은 책들에게 맡기고, 여기
         서는 커널 이미지가 어떻게 만들어지고 이미지를 구성하는 요소들은 어떤 것들이 있는지
         를 알아보았다. 커널을 이해할 수 있는 작은 단위로 쪼개는 것이 이 거대한 소프트웨어
         프로젝트를 어떻게 조사하는지를 배우는 핵심 요소이다．

      口 커널 빌드 시스템을 알아보고, 수정 사항을 반영하기 위해써 빌드 시스템을 변경하는 과
         정을 알아보았다.

      口 구성 편집기는 몇 가지 종류가 있는데, 그 중에 하나를 선택해써 그 안의 메뉴와 메뉴
         항목들을 어떻게 변경하는지 알아보았다. 이 과정은 모든 GUI 방식의 구성 편집기에 적
         용될 수 있다．

      口 커널을 자체적으로 유용한 커널 관련 문서들을 담고 있는 디렉터리를 가지고 있다. 커널
         을 이해陌｝고 그 동작 원리를 조사하는 데 도움이 될 만한 자료들이다．

      口 이 장의 마지막에는 리눅스 커널 배포판을 구하기 위해서 취할 수 있는 선택어］ 대해서
         간단히 정리하는 것으로 마무리했다．
                                                      다른 관점에서 본 리눅스 커널   Chapter 4




4.5. ] 더 읽어 보기
       리눅스 커널 HOWTO 문서（Linux Kernel HOV叩O) :
       www. tldp. org/F珣WTO/Kern이냐珣WTO


       커널 Kbuild 문서（Kernel Kbuild documentation) :
       http://sourceforge. net/projects/kbuild/


       리눅스 문서화 프로젝트（The Linux Documentation Pr이ect) :
       www. tldp. org/


       TIS의 ELF 파일 포맷 명세서 버전 1. 2(Tool Interface Standard (TIS) Executable and
       Linking Format (ELF) Specification, Version 1. 2)
       TIS 위원회 , 1995년 5월


       리눅스 커널 문서의 kbuild어］ 대한 문서 :
       . . . /Documentation/kbuild/makefiles. txt


       리눅스 커널 문서의 kconfig에 대한 문서 :
       . . . /Documentation/kbuild/kconfig-language. txt


       Li끄ux Kernel Deve加刃me끄t, 2nd 月dition
       Rovert Love
       Novell Press, 2005
이번 장에서 배울 내용


  U 복합적인 커널 이미지 : 口ggy와 그 외 오브젝트 파일

  U 초기화 단계의 제어 흐름

  U 커널 커맨드 라인 처리하기

  U 서브시스템 초기화

  . In仕 쓰레드

  . 요약
「 好a     Embedded Linux Primer




       임베디드 리눅스 시스템에 전원이 들어오면 복잡한 작업이 시작된다. 전원이 들어온 몇 초
       후에는 커널이 정상 동작을 시작하고 시스템에 있는 mllit 스크립트에 명시된 응용 프로그램
       들이 실행된다. 초기화를 위한 여러 가지 작업의 상당 부분이 시스템 구성 값에 따라서 결정
       되며 임베디드 개발자는 이 시스템 구성을 관리한다．

       이 장에서는 커널의 초기화 과정에서 어떤 일들이 일어나는지 알아보고자 한다. 먼저 커널
       의 초기화 과정에서 사용되는 메커니즘과 프로세스에 대해서 자세히 살펴볼 것이다. 그리고
       리눅스의 커널 명령에 라인（Kern이 command line）에 대해서 설명하고, 이를 이용해서 리눅스를
       시작시키기 위한 환경을 설정하는 방법을 알아본다. 이 장에서 다루는 내용을 통해서 독자
       는 자신이 개발하고자 하는 시스템에 맞게 커널 초기화 과정을 수정 및 제어할 수 있게 될
       것이다．



5.1 복합적인 커널 이미지 : piggy와 그 외 오브젝트 파일
       임베디드 시스템에 전원이 들어오면 프로세서에 의해서 제일 먼저 실행되는 것은 부트로더이
       다. 부트로더는 저수준 하드웨어 초기화를 일부 수행한 다음 커널로 제어권을 넘긴다. 이러
       한 과정은 개발 단계에서 사용하기 위해서 수동으로 이루어질 수도 있고（예를 들어 , 사용자
       가 직접 부트로더의 명령 프롬프트에 로드／부트 명령어들을 입력하는 것）, 또는 일반 제품을
       위한 경우처럼 자동으로 부팅하게 할 수도 있다. 이 주제에 대해서는 7장, "부트로더"에서
       설명하고 있으니 , 부트로더에 관한 상세한 내용은 7장으로 미루도록 하자．

       4장, "다른 관점에서 본 리눅스 커널"에서는 리눅스 커널 이미치를 이루고 있는 구성 요소에
       대해서 알아보았다. 모든 아키텍처에서 빌드하면 공통적으로 생기는 파일 중의 하나인 ELF
       바이너리 vmlinux를 다시 떠올려 보자. 이 바이너리 파일은 모놀리식 커널 자체인데 , 다른
       말로 커널 본체（kern이 아oper）라고도 한다. 사실 vmlinux의 링크 단계에서 이미지가 만들어
       지는 과정을 보면서 , 우리가 지적했던 점이 코드의 맨 첫 줄이 어디에 위치하게 되느냐 였다．
       대부분의 아키텍처에서 head. S나 이와 비슷한 이름을 가진 어셈블러 소스 파일이 맨 처음
       에 위치하게 된다. 커널 소스의 PowerPC (ppc) 부분에는 각각의 프로세서 모텔을 위한
       head.S 파일이 여러 7가 존재한다. 예를 들어 , AMCC 440 계열 프로세서는 head 44x. S
       파일에 의해서 초기화된다．




 148
                                                                  커널 초기화   Chapter 5



      일부 아키텍처와 부트로더는 vmlinux 커널 이미지를 곧바로 부팅시킬 수 있다. 예를 들어，
      PowerPC 아키텍처에 기반한 플랫폼은 U-Boot 부트로더가 vmliriux 커널 이미지를 직접
      부팅시킨다1)（물론 ELF 형식을 바이너리 파일로 변환해서 사용한다. 곧 설명하겠다）. 다른
      조합, 즉 다른 아키텍처와 부트로더의 조합도 커널을 로드하고 부팅하기 위해서 필요한 알맞
      은 구성을 위해서 추가 기능이 필요하다．

      ［리스트 5-1］은 인텔의 IXP425 통신용 프로세서를 내장하고 있는 ADI 엔지니어링의 코요
      터1 참조용 하드웨어 플랫폼을 위해서 커널을 빌드하는 마지막 과정을 보여 주고 있다. 이 목
      록을 보면 커널 빌드 시스템의 기본 설정대로 그 출력 내용을 간단히 축약해서 내보내도록
      한 것을 알 수 있다. 4장에서 설명했듯이 명령어를 축약형으로 표기해서 빌드 과정의 에러와
      경고 메시지들에 좀 더 집중할 수 있도록 한 것이다．

      ［리스트 5-1] 커널 빌드의 마지막 과정： ARM/IXP425（코요테）

         $ make ARCH=arm CROSS_COMPILE=xscale_be- zlmage
                < many build steps omitted for clarity>
          'LD          vml i flux
           SYSMAP       System . map
           OBJ COPY     arch/arm/boot/Image
           Kernel :     arch/arm/boot/Image is ready
           AS          arch/arm/boot/compressed/head .0
           GZIP        arch/arm/boot/ compressed/piggy. gz
           AS          arch/arm/boot/ compressed/piggy .0
           CC          arch/arm/boot/compressed/misc .0
           AS          arch/arm/boot/compressed/head-xscal e .0
           AS          arch/arm/boot/compressed/big-endian. o
           LD          arch/arm/boot/compressed/vml i nux
           OB]COPY      arch/arm/boot/zlmage
           Kernel :     arch/arm/boot/zlmage is ready
           Building  modules,     stage 2.




      ［리스트 5-1］의 세 번째 줄을 보면 \imlinux 이미지가 링크되는 것을 볼 수 있다. 그 이후로
      여러 개의 추가 오브젝트 모듈을 처리한다. 그 중에서도 head. o, piggy.o2) 그리고 현재


l) 부팅 시간이 삘라야 하는 경우가 아니면 리눅스 커널은 항상 압축된 상태로 저장된다. 이 경우에는 이미지를 ulmage라고 불러야
   한다. 이는 U-Boot 헤더와 vu小flux 파일을 함께 압축한 이미지이다（7장, "부트로더"를 참고）.


                                                                                 149 1
         Embedded Linux Primer




      아키텍처를 위한 hea小xscale .07} 있다（각 라인에 있는 태그가 어떤 작업을 하는지를 나
      타낸다. 즉, AS는 어셈블러를 실행한다는 것이고, GZIP은 압축을 나타낸다）. 일반적으로，
      이 오브젝트 모듈은 주어진 아키텍처에 종속적이기 때문에 （여기서는 ARM／엑스스케일） 커
      널을 부팅하기 위해서 필요한 로우 레벨 유틸리티 함수들을 가지고 있다. ［표 5-1］은 ［리스
      트 5-1］에 있는 구성 요소들을 자세히 정리한 것이다．

      ［표 5-1) ARM／엑스스케일 아키텍처용 오브젝트3)

       요소                        기능 및 설명

       vmlinux                   ELF 형식의 커널 본체, 심볼, 주석, 디버깅 정보와 0끼텍처를 위한 구성 요
                                 소들을 포함하고 있다．

       System. map               vmlinux 모듈에 대한 문자열 방식의 커널 심볼 테이블

       Image                     심볼과 추7F 정북 주석 등을 제거한 바이너리 형식의 커널 모듈

       head. o                   A日M 프로세서들을 위해서 공孚4으로 사용되는 스타트업 코드. 부트로더7F
                                 제어권을 이 모듈에 넘긴다．

       piggy. gz                 위의 Image 파일을 gzip으로 입축한 것．

       piggy. o                  piggy.gz 파일을 어셈블리 언어 형식으로 만들어 둔 것． misc. O와 같이
                                 링크시키71 위해서 변환한 것이다．

       misc .O                   커널 이미지（piggy. gz）의 압축을 풀기 위한 루틴. 몇몇 0끼텍처에서 볼 수
                                 있는 친숙한 부팅 메시지인 'Uncompr明sing Linux ··· Don可을 이 모듈이
                                 출력힌타．

       head-xscale .O            엑스스케일 프로세서 계열을 위한 초기화 코드

       big- endian. o            엑스스케일 프로세서를 박엔디안 모드로 전환시키는 아주 작은 어셈 코드

       vmlinux                   복합적인 커널 이미지. 이름 선택이 그리 좋지는 않은더I, 커널 본체와 이름이
                                 같'I 때문이다． 커널 본체（kern이 proper）와 복합 이미지는 이름은 같지만 다
                                 른 파일이다. 이 바이너리 이미지는 커널 본체7F 이 표에 있는 다른 오브젝트
                                 들과 링크된 결과물이다. 본문 참고．

        z Image                  부트로더에 의해서 로드될 최종적인 복합 커널 이미지 파일．


2) 여기서 piggy라는 단어는 "剖］ 업는缸明y-back) ' 개념을 나타내기 위해서 사듣뛴다. 즉， 커널 바이너리 이미지가 부트스트랩
   로더의 등어］ 업힌 상태로 복합된 커널 이미지가 만들어지7] 때문이다．
3) （역자주） 여기서 오브젝트（아永네는 어떤 소스 파일을 컴파일한 결과 생기는 파일 (.0）을 나타낸다．
                                                          커널 초기화   Chapter 5




        이 구조를 좀 더 쉽게 이해하기 위해서 그림을 하나 보도록 하자. ［그림 5-1］은 이미지의
        구성 요소들이 빌드 과정을 통해서 최종적으로 부팅 가능한 커널 이미지로 어떻게 변화해
        가는지를 볼 수 있다. 이어지는 섹션을 통해서 각 구성 요소와 그 처리 과정을 자세히 알아
        보자．

                                          piggy .gz를 감싼 오브젝트
                                       mm> 커널 이미지를 포함하고 있음




        vmlinux                image

           (ELF                （바이너리
         오브젝트）                 오브젝트）
                                                                부팅 가능한
                                          압축된        misc.o     커널 이미지
                                        바이너리 커널
                        불필요한 부분을 제거한                 아工
                           커널 이미지                   endian.o
                                                      head-
         커널 본체
                                                     xscale.o



        I 그림 5-1 복합 커널 이미지 생성 과정



5. ] . ] Image 오브젝트
        커널 ELF 파일인 vmlinux이 빌드되고 나면 커널 빌드 시스템은 ［표 5-1]에 나와 있는 다
        른 대상들을 처리하는 일을 계속한다. Image 오브젝트 파일은 vmlinux로부터 만들어진다．
        Image 파일은 기본적으로 불필요한 섹션4)（추가 정보 및 주석 섹션5)）과 기존에 포함되어
        있던 디버깅 심벌들을 드러낸 vmlinux ELF 파일이다. 이를 위해서 다음의 명령어를 이용
        한다．




4) （역자주） El下와 같은 실행을 위한 바이너리 내부는 다양한 용도의 공간으로 나뉘는데 이를 섹션이라고 한다． 예를 들어， 코드를
   담는 TEf 섹션, 젼역 데이터를 위한 DATA 섹션 등을 들 수 있다．
5) C역자주） . U이e와 . comn祀Ut 섹션
          Embedded Linux Primer




          xscale_be-objcopy -o binary -R .note -R . comment -s \
          vnil I nux arch/ arm/boot/Image




        위 obj copy 명령에서 中0 옵션은 obj copy에게 바이너리 파일을 생성하라는 의미이고, -I之
        옵션은 .note와 .comment라는 이름을 가진 ELF 섹션들을 제거하라는 뜻이다. 그리고 田
        는 디버깅 정보를 제거하겠다는 의미의 옵션이다. 주의할 점은 obj copy 명령어가 입력으로
        vmiinux ELF 이미지를 받아서 Image라는 이름의 바이너리 파일을 생성한다는 점이다．
        정리하면 Image 파일은 커널 본체에서 .no七e와 . con끄nent 섹션과 디버깅 심벌을 드러낸
        것에 지나지 않는다．


5.1.2 아키텍처 오브젝트
        다음 빌드 과정에서는 작은 모듈 몇 개를 컴파일하는데 여기에는 저수준의 아키텍처 , 프로세
        서에 종속적인 작업을 구현하고 있는 어셈블리 파일 몇 개도 포함된다. 이들 각각의 오브젝
        트에 대해서는 ［표 5-1]에 정리되어 있다. 특히 주의할 점은 piggy.o라는 오브젝트 파일이
        만들어지는 순서이다. 먼저 Image 파일（바이너리 커널 이미지）이 gzip 명령을 이용해서 압
        축된다．

          gzip -f -9 < Image > piggy. gz


        이 명령을 통해서 단순히 Image 바이너리 파일을 압축한 버전인 piggy.gz 파일이 만들어
        진다. 이 부분에 대해서는 ［그림 5-1］에서 확인할 수 있다. 이어지는 과정은 좀 더 흥미로운
        데 , 압축된 piggy.gz어］ 대한 참조를 가지고 있는 piggy.S라는 어셈블리 파일을 어셈블6)
        한다. 본질적으로 바이너리 커널 이미지가 어셈블리 언어로 작성된 부트스트랩 로더7）의 등에
        업히는 것으로 생각할 수 있다. 부드入E랩 로더는 프로세서와 메모리 영역을 초기화한다．
        그리고 제어권을 커널에 넘기기 전에 바이너리 커널 이미지의 압축을 풀어서 시스템 메모리
        의 알맞은 장소에 로드해 두는 일을 한다. ［리스트 5-2］는 . . . /arch/arm/boot/
        compressed/piggy. S 파일의 전체 내용이다．


6) （역자주） C 파일이 컴파일되듯이, 어셈블리 파일은 어셈블된다．
7) 부트로더와 헷칼리지 않기 바란다. 부트스트랩 로뎌는 두 번째 단계의 로더이고, 부트로더는 맨 처음 단꼐의 로더라고 생각할
   수 있다．


I 152
                                                             커널 초기화   Chapter 5



      ［리스트 5-2] Piggy.s 어셈블리 파일


           . section .piggydata, #alloc
           . glob]    input_data
         input_data:
           .incbin "arch/ arm/boot/ compressed/piggy. gz "
           .globl    input_data_end
         input_data_end:




      이 작은 크기의 어셈블리 파일은 간단해 보이지만, 곧바로 와 닿지는 않는다. 이 파일의 목적
      은 압축된 바이너리 커널 이미지를 .piggyda七a라는 이름의 ELF 섹션으로 만들기 위한
      것이다. 이는 #include와 비슷한 기능을 하는 어셈블러의 전처리 지시자인 .incbin을 이
      용해서 이루어진다. 요약하면 이 어셈블리 파일의 목적은 최종적으로 다른 이미지 , 즉 부트
      스트랩 로더 안에 페이로드8) 형태로 압축된 바이너리 커널을 포함시키도록 하는 것이다. 그
      리고 inpu七 data와 input dat是‘end라는 레이블에 주의하자. 부E入드랩 로더는 이것
      을 이용해서 페이로드, 즉 커널 이미지가 차지하는 위치의 시작과 끝을 알 수 있다.


5.1.3 부트스트랩 로더
      부트로더와 헷갈리면 안 된다. 많은 아키텍처에서 리눅스 커널 이미지를 메모리에 로드하기
      위해서 부트스트랩 로더（또는 2단계 로더）를 이용한다. 일부 부드入E랩 로더는 커널 이미지
      에 체크썸（check-sum) 연산을 수행해서 올바른 이미지인지를 검사한다. 그리고 대부분의
      부E入E랩 로더가 압축을 해제하고 커널 이미지를 재배치하는 일을 수행한다. 여기서 부트
      로더와 부드入E랩 로더의 차이는 간단하다. 부트로더는 전원이 들어온 후에 보드를 제어하
      는 등의 작업을 수행하며 리눅스 커널과는 무관하게 동작한다. 반면 부E入E랩 로더의 주된
      목적은 보드 단계의 부트로더와 리눅스 커널을 연결해 주는 아교 역할을 수행하는 것이다．
      커널 바이너리 이미지의 압축을 해제하고, 섹션을 제배치하는 일은 물론이고, 커널이 수행되
      기 위한 적절한 문맥을 제공하는 것도 부드入E랩 로더의 책임이다. 이는 PC 아키텍처에서
      찾아볼 수 있는 1차, 2차 로더와 비슷한 개념이다．




8) ［역자주） 페이로드（Pa괴oad) : 예를 들어, 어떤 네트워크 패킷이 있을 때， 패킷의 헤더나 기타 제어 코드 등을 三러낸 순수 데이
   터를 페이로드라고 한다．


                                                                            153
難 a.     Embedded Linux Primer




       ［그림 5-2］를 보면 좀 더 명확하게 이해할 수 있다. 부E入드랩 로더는 로딩을 위해서 커널
       이미지와 하나로 합쳐진다．



                        바이너리
        口ggy.o          커널
                        이미지


        mtsc.o
         big_
       endian.o         부트스트랩
         head-          로더
        xscale.o
        head.o
       I 그림 5-2 ARM 엑스스케일을 위한 복합 커녈 이미지

       지금까치 배운 예제에서 부E入E랩 로더는 ［그림 5-2］에 있는 바이너리 이미지들로 구성되
       어 있다. 부E入드랩 로더에 의해서 수행되는 기능은 다음과 같은 것이 있다．

         口 프로세서 내부의 명령에 캐시, 데이터 캐시를 활성화시키고, 하드웨어 인터럽트를 비활
            성화시키며 , （그 코드가 수행되기 위한 환경을 구성하는 등의 작업을 담당하는 어셈블리
            파일을 이용한 저수준의 프로세서 초기화. 여기에는 head.o와 head-xscale . 07j-
            있다．

         口 misc.(＞어］ 포함된 압축을 해제하고 코드를 재배치하는 기능

         口 프로세서를 빅 엔디안 모드로 바꿔주는 big-endian .0 파일과 같이 기타 프로세서를
            위한 초기화 작업

       지금까지 우리가 예를 통해서 살펴본 세부 내용들이 시FM／엑스스케일을 위한 커널에 한정
       된 내용이라는 점은 크게 중요하지 않다. 각 아키텍처가 기본 개념은 비슷하지만 각기 다른
       세부 고려 사항이 있다. 하지만 지금까지 알아본 것과 같은 접근법을 이용하면 자신의 아키
       텍처를 위해서 요구되는 항목도 파악할 수 있을 것이다．
                                                          커널 초기화     Chapter 5




5.1.4 부트 메시지
    레드햇이나 수세 리눅스와 같은 데스크탑용 리눅스 배포 버전이 설치된 PC가 부팅되는 모습
    을 본 적이 있을 것이다. PC 자체의 BIOS 메시지가 출력된 후에 , 리눅스가 자신의 커널
    서브시스템을 초기화하는 과정에서 콘솔에 엄청나게 많은 메시지를 출력하는 것을 보았을 것
    이다． 이러한 출력의 상당 부분은 모든 아키텍처 및 머신에서 공통적으로 출력되는 내용이
    다. 메시지의 처음 부분에서 흥미로운 내용 두 가지를 볼 수 있는데 , 리눅스 버전 문자열과
    커널 커맨드 라인（kern이 command line）이다. 이들에 대해서는 잠시 후 설명하겠다. ［리스트
    5-3］은 인텔 엑스스케일 IXP425 프로세서 기반의 리눅스 플랫폼인 ADI 엔치니어링 코요
    터］ 보드상에서 리눅스 커널이 부팅 과정 중에 출력되는 메시지를 나타낸 것이다. 각 항목은
    참조를 쉽게 하기 위해서 행 번호를 붙였다.

    ［리스트 5-3) IXP425상0似倒 부팅 메시지


      1 Uncompressing Linux. . . done, booting the kernel.
      2 Linux version 2. 6.14-clh (chris@pluto) (gcc version 3. 4. 3 (MontaVista
      3. 4. 3- 25. 0. 30
      .0501131 2005-07- 23) ) #11 Sat Mar 25 11:16: 33 EST 2006
      3 CPU: xScale尸IXP42x Family [690541c1] revision 1 (ARMv5TE)
      4 Machine: ADI Engineering Coyote
      5 Memory policy: ECC disabled, Data cache writeback
      6 CPUO: 0 VIVT undefined S cache
      7 CPUO: I cache: 32768 bytes, associativity 32, 32 byte lines, 32 sets
      8 CPUO: D cache: 32768 bytes, associativity 32, 32 byte lines, 32 sets
      9 Built 1 zonelists
      10 Kernel command line: console=ttySO, 115200 ip=bootp root=/dev/nfs
      11 PID hash table entries: 512 (order: 9, 8192 bytes)
      12 Console: colour dummy device 80x30
      13 Dentry cache hash table entries: 16384 (order: 4, 65536 bytes)
      14 mnode- cache hash table entries: 8192 (order: 3, 32768 bytes)
      15 Memory: 64MB = 64MB total
      16 Memory: 62592KB available (1727K code, 339K data, 112K mnit)
      17 Mount-cache hash table entries: 512
      18 CPU: Testing write buffer coherency: ok
      19 softiockup thread 0 started up.
      20 NET: Registered protocol family 16
      21 PCI: IXP4xx is host
      22 PCI: IXP4xx Using direct access for memory space
      23 PCI: busO: Fast back to back transfers enabled


                                                                           155
      Embedded Linux Primer



       24 dmabounce: registered device 0000:00:0f. 0 on pci bus
       25 NetWinder Floating Point Emulator vO. 97 (double precision)
       26 JFFS2 version 2. 2. (NAND) (C) 2001- 2003 Red Hat, Inc
       27 serial: 8250/16550 driver $Revision: 1. 90 $ 2 ports, IRQ sharing
        니 disabled
       28 ttyS0 at MMI0 0xc8001000 (irq = 13) is a xScale
       29 io scheduler noop registered
       30 io scheduler anticipatory registered
       31 io scheduler deadline registered
       32 io scheduler cfq registered
       33 RAMDISK driver initialized: 16 RAM disks of 8192K size 1024 blocksize
       34 loop: loaded (max 8 devices)
       35 eeprol0o. c: vl.09j- t 9/29/99 Donald Becker
        니 http: //www. scyld. com/network/eepro100. html
      36 eeprol00. c: $Revision: 1. 36 $ 2000/11/17 Modified by Andrey V.
                                                                          Savochki n
        니 <saw@saw. sw. com. sg> and others
      37 ethO: 0000: 00:0f.0, 00: OE: OC: 00: 82: F8, IRQ 28.
      38 Board assembly 741462-016, Physical connectors present: RJ4S
      39 Primary interface chip i82555 PHY #1.
      40 General self-test: passed.
      41 Serial sub- system self-test: passed.
      42 internal registers self-test: passed.
      43 ROM checksum self-test: passed (0x8b51f404)
      44 IXP4XX-Flash.0: Found 1 x16 devices at OxO in 16-bit bank
      45 Intel/Sharp Extended Query Table at 0x0031
      46 using buffer write method
      47 cfi_cmdset_0001: Erase suspend on write enabled
      48 searching for RedBoot partition table in IXP4XX-Flash. 0 at offset
       니 0xfe0000
      49 5 RedBoot partitions found on MID device IXP4XX-Flash. 0
      50 creating 5 MID partitions on "IXP4XX-Flash. 0":
      51 0x00000000- 0x00060000 : "RedBoot "
      52 0x00100000- 0x00260000 : "MyKernel "
      53 0x00300000- 0x00900000 : "RootFS"
      54 0x00fc0000- 0x00fc1000 : "RedBoot config"
      55 mtd: partition "RedBoot config" doesn 't end on an erase block -- force
      read-onlyoxoofe0000-oxol000000 : "FIS directory "
      56 NET: Registered protocol family 2
      57 ip route cache hash table entries: 1024 (order: 0, 4096 bytes)
      58 TCP established hash table entries: 4096 (order: 2, 16384 bytes)
      59 TCP bind hash table entries: 4096 (order: 2, 16384 bytes)
      60 TCP: Hash tables configured (established 4096 bind 4096)



156
                                                         커널 초기화       Chapter 5



  61 TCP reno registered
  62 TCP bic registered
  63 NET: Registered protocol family 1
  64 sending BOOTP requests . OK
  65 IP-config: Got BOOTP answer from 192.168.1.10, my address is
   니 192.168.1.141
  66 IP-Config: Complete:
  67       device=eth0, addr=192. 168.1.141, mask=255 .255. 255. 0,
   니 叩＝255. 255. 255. 255,
  68       host=192.168.1.141, domain=, nis-domain=(none) ,
  69       bootserver=192.168.1.10, rootserver=192.168.1.10,
   니 rootpath=/home/chri s/ sandbox/coyote-target
  70 Looking up port of RPC 100003/2 on 192.168.1.10
  71 Looking up port of RPC 100005/1 on 192.168.1.10
  72 VFS: Mounted root (nfs filesystem) .
  73 Freeing mnit memory: 112K
  74 Mounting proc
  75 starting system loggers
  76 Configuring lo
  77 Starting inetd
  78 / #



커널은 ［리스트 5-쏘에서 보는 바와 같이 시작 과정에서 매우 유용한 정보를 출력한다. 일부
출력 내용에 대해서는 다음 몇 개의 섹션에서 자세히 살펴볼 것이다. 첫 번째 줄의 메시지는
앞부분에서 살펴본 부드入E랩 로더에 의해서 출력된다. 즉, 이 메시지는 . . . /arch/arm/
boo七／compressed/misc. c어］ 있는 압축을 해제하는 로더가 출력하는 것이다．

［리스트 5-3］의 두 번째 줄은 커널 버전을 나타내는 문자열이다. 이 줄이 커널에 의해서 출
력되는 첫 번째 내용이다. S七art kernel () 어］ 진입한 후에 커널에 의해서 처음 수행되는
C 코드 중에 하나가 바로 다음의 코드이다．

  printk (linux_banner) ;

이 코드가 방금 설명한 ［리스트 5-3］의 2번째 줄의 커널 버전 문자열을 출력하는 일을 한다．
이 버전 문자열은 커널 이미지에 대한 적절한 정보를 담고 있다．




                                                                            157
  II     Embedded Linux Primer



         口 커널 버전 : Linux version 2.6.10-clh

         口 커널이 컴파일된 호스트의 사용자／머신 이름

         口 툴 체인 정보 : 몬타 비스타 소프트웨어가 제공하는 gee version 3.4.3

         口 빌드 번호

         口 컴파일된 날짜／시간

       이 정보는 개발중에는 물론이고 실제 제품으로 나간 후에도 유용하게 사용된다. 이들 정보
       중에서 한 가지 빼고는 모두 쉽게 이해할 수 있을 것이다. 빌드 번호（build nun由er）는 개발자가
       커널 버전 문자열의 뒤에 추가하도록 한 것인데 , 단순히 빌드 날짜와 시간으로 표시하는 것
       보다는 실제 커널이 빌드된 횟수를 나타내기 때문에 좀 더 의미가 있는 정보라고 볼 수 있다．
       즉, 개발자가 일반적이고 자동화된 방법으로 커널이 빌드되는 것을 추적할 수 있는 방법이
       다. 치금 다루는 예제에서는 ［리스트 5-3］의 두 번째 줄의 #11을 보면 알 수 있듯이 열한
       번째로 빌드된 것임을 알 수 있다. 이 빌드 번호 문자열은 리눅스 소스의 최상위 디렉터리에
       .version이라는 이름의 숨김 파일 형태로 저장되어 있다. 그리고 이 파일 안의 값은 최상
       위 makefile이 . . . /scri1亢s/mkversion어］ 있는 스크립트를 호출해서 자동으로 증가시
       키도록 되어 있다. 즉, 빌드 번호는 작은 부분이라도 커널이 다시 빌드될 때마다 자동으로
       증가되는 문자열임을 알아두자．



5.2 초기화 단계의 제어 호름
       이제 복합 커널 이미지의 구성 요소와 구조에 대해서 어느 정도 이해를 했을 것이다. 그럼
       부트로더에서부터 커널까지의 제어 흐름을 살펴봄으로써 부트 과정을 완전히 파악해 보도록
       하자. 2장, "임베디드 처음 경험하기"에서 이미 살펴본 것처럼 부트로더는 전원이 처음 인가
       되면 곧바로 실행되는 시스템의 비휘발성 메모리（플래시 또는 RUM)에 저장되어 있는 로우
       레벨 코드이다. 일반적으로 크기가 작으며 , 저수준의 초기화를 진행하기 위한 간단한 초기화
       코드와 부트 이미지를 로드하기 위한 코드 및 시스템 자체 진단 루틴 등을 갖고 있다. 그리고
       추가적으로 메모리를 검사하고 내용을 수정할 수 있도록 메모리를 덤프하고 채우는 루틴을
       가지고 있을 수도 있다. 또한 메모리 및 입출력 테스트를 포함한 저수준의 보드 자체 진단
       루틴을 가지고 있는 경우도 있다. 마지막으로 부트로더는 다른 프로그램 , 즉 일반적으로 리
       눅스와 같은 운영체제를 로드하고 제어권을 넘기기 위한 기능도 가지고 있다.


1158
                                              커널 초기화        Chapter 5



지금 다루는 예제에서 사용한 ARM 엑스스케일 플랫폼은 레드붓（Redboot) 부트로더를 내
장하고 있다. 전원이 들어오면 이 부트로더가 곧바로 실행되어 운영체제（Os）를 로드하는 일
을 진행한다. 부트로더는 （보드상의 플래시나 하드 드라이브와 같은 곳에 저장되어 있을 수
도 있고, 또는 로컬 네트워크나 다른 장치에 저장되어 있을 수도 있는） Os 이미지를 로드하
고 알맞은 곳에 위치시키고 나서 제어권을 해당 이미지로 넘기게 된다．

예제로 사용된 이 엑스스케일 플랫폼의 경우는, 부E入드랩 로더의 head.o 모듈 내 S七ar七
레이블의 위치로 제어권을 넘기게 된다. 이 과정이 ［그림 5-3］에 설명되어 있다．




                                             start kernel
                                         H




       부트로더          부트스트랩     커널
                     로더        vmlinux         커널
                                               main.o
I 그림 5-3 ARM 부팅 과정

앞에서도 설명했듯이 커널 이미지의 앞에 덧붙여진 부E入E랩 로더는 오직 한 가지 기능만
수행한다. 즉, 커널 이미지의 압축을 해제하고 재배치시키기 위한 알맞은 환경을 만들고, 커
널로 제어권을 옮기는 것이다. 대부분의 아키텍처에서 제어권은 부E入E랩 로더에서 곧바로
커널 본체가 head.o라는 이름의 모듈로 넘어가게 된다. 부E入E랩 로더와 커널 본체에 모
두 head.o라는 모듈을 갖고 있는 점이 좀 아쉬운데, 이 때문에 초보 임베디드 리눅스 캐발
자에게는 혼란의 소지가 될 수 있기 때문이다. 커널 개발자들이 수정 사항을 받아 줄지는 의
문이지만, 부드入E랩 로더에 있는 head.o는 사실 kernel boo七stra으loader
head.o라고 부르는 것이 좀 더 적당하다. 그리고 최신 리눅스 26 소스 트리는 적어도 37
7긔1 정도의 head S 소스 파일을 가지고 있다. 이러한 점이 리눅스 소스 트리에 좀 더 익숙해
져야 하는 다른 이유라고 할 수 있다．

제어의 흐름올 시각적으로 표현한 ［그림 5-3］을 다시 보자. 부E入E랩 로더가 자신의 작업
을 마치면 제어권이 커널 본체의 head. o로 넘어가서 다시 main. c의 start kernel () 로
넘어가는 것을 볼 수 있다．

                                                                  159 1
    a.       Embedded Linux Primer




5.2. ] 커널 진입점 : head.o
         커널 개발자의 원래 의도는 지정한 아키텍처를 위한 head.o 모듈을 특정 머신9）어］ 종속되지
         않도록 최대한 범용으로 만드는 것이었다. head. S 어셈블리 파일로부터 만들어진 이 모듈
         은 . . . /arch/<ARCH>/kernei/head. S어］ 위치하고 있다. 여기서 <ARCH＞는 특정한 아
         키텍처 이름으로 대체된다. 이 장에서 다루는 예제는 사tM／엑스스케일에 기반하고 있기 때
          문에 . <ARCH> 부분이 arm이 된다．

         head.o 모듈은 커널의 n追in을 실행시키기 위한 준비 과정으로, 아키텍처와 CPU에 한정
         된 초기화를 수행한다. 특정 CPU에 한정된 작업들은 같은 프로세서군끼리는 같이 사용될
         수 있도록 최대한 범용으로 작성되어 있다. 머신 종속적인 초기화는 다른 곳에서 수행되는
         데 , 이는 곧 설명하겠다. head.o가 수행하는 저수준(low-level) 작업 중에는 다음과 같은
         것들이 있다．

             口 프로세서와 아키텍처가 올바른지 검사

             口 초기 페이지 테이블 생성

             口 프로세서의 메모리 관리 장치（MMU10)）를 활성화시킴

             口 일부 에러 감지 및 리포팅을 위한 설정

             口 커널 본체의 시작점 main. c로 점프

         이들 함수의 내부에는 상당히 복잡한 내용들이 숨켜져 있다. 많은 초보 개발자들이 디버거를
         이용해서 이 코드의 내용을 한 줄씩 따라가면서 이해하려고 하는데 , 결국 디버거가 코드 문
         맥을 잃어버리는 것을 보게 된다. 어셈블리 언어의 복잡성과 가상 메모리에 대한 하드웨어
         적인 세부사항을 설명하는 것은 이 책의 범위를 벗어나지만, 중요한 내용 몇 가치는 짚고 넘
         어갈 필요가 있다．

         제어권이 부E入E랩 로더에서 커널의 head.o로 처음 넘어갈 때는 프로세서가 x86 용어로
         리얼 모드（real mode）라고 부르는 모드에서 동작하게 된다. 즉, 프로세서의 프로그램 카운
         터11)（또는 같은 일을 하는 다른 이름의 레지스터）에 있는 주소 값은 실제 프로세서가 메모리


9) 여기서 사용된 머신이라는 용어는 특정 하드웨어 참고 플랫폼을 지칭햐는 의미로 사용되었다．
10) C역7;} ) Memory Management Unit
                                                                   커널 초기화      Chapter 5


        어드레스 핀12）으로 제어하는 실제 물리 주소와 일치한다. 메모리 변환을 위해서 프로세서의
        레지스터들과 커널 데이터 구조를 초기화하고 난 후 프로세서의 메모리 관리 장치（MMIJ）를
        켜게 된다. MMEJ를 켜는 순간 프로세서가 기존에 사용하던 주소 공간 대신에 커널 개발자에
        의해서 임의로 결정된 메커니즘으로 동작되는 가상 어드레싱을 이용하는 공간으로 바뀌게 된
        다. 이 복잡한 구조를 이해하기 위해서는 어셈블리 언어로 작성된 코드가 어떻게 구성되어
        있는지와 논리적으로 어떻게 동작하는지를 분석해야 하는 것은 물론이고, CPU와 하드웨어
        주소 변환 메커니즘에 대한 세부 지식도 모두 이해해야만 가능하다. 간단히 이야기하면
        MMJ가 켜지는 순간부터 물리 주소가 논리적인 주소로 바뀐다고 생각하면 된다. 디버거가
        이 부분의 코드에서 한 스텝씩 정상적으로 진행하지 못하는 이유가 바로 이것 때문이다．

        두 번째로 유의할 점은 커널 부팅 과정의 초기에는 사용할 수 있는 매핑 영역이 한정되어
        있다는 것이다. 많은 개발자가 자신이 사용하는 플랫폼을 위해서 head.o를 수정하려고 하
        는데 이때 이러한 제한 사항 때문에 문제13）어］ 봉착하게 된다. 즉, 보통 다음과 같은 경우에
        해당한다. 독자가 부팅 과정의 아주 초기에 어떤 펌웨어를 로드해야 하는 하드웨어 장치를
        가지고 있다고 해보자. 한 가지 가능한 방법은 필요한 핌웨어를 컴파일해서 정적으로 커널
        이미지에 포함시키고 그것을 디바이스에 로드할 때 포인터로 참조하는 것이다. 하지만 현 시
        점에서는 메모리 매핑 영역이 제한적이기 때문에 펌웨어 이미지가 부팅의 초기 과정에 매핑
        되어 있는 영역을 벗어난 곳에 존재할 가능성이 상당히 높다 코드가 실행되면 프로세서 내
        부에 적절하게 매핑되어 있지 않은 영역에 접근하려고 할 것이기 때문에 페이지 폴트를 발생
        시킬 것이다. 더군다나 이 단계에서는 페이지 폴트 핸들러도 아직 설치되어 있지 않은 상태
        이기 때문에 적절한 원인 메시지도 출력하치 않은 채로 시스템 오류가 발생한다. 부팅 과정
        의 초기 단계에서는 문제가 무엇인지 파악할 만한 적절한 에러 메시치를 볼 수 없는 경우가
        대부분이다．

        가능하다면 커널이 부팅될 때까지 필요한 하드웨어 초기화 작업을 미루는 것이 현명한 방법
        이다. 이렇게 스타트업 코드의 복잡한 어셈블리 코드를 자신에게 맞게 수정하려고 하는 것보
        다는 잘 알려진 디바이스 드라이버 모델을 이용해서 자체 제작 하드웨어에 접근하는 것이 좋


11) 프로그램 카운터（可ograni counter) : 흔히 명령에 포인터 (Ins甘uction Pointer）라고도 부르고， 메모리에서 다음 번 실행될 명령어
    의 주소를 담고 있는 레지스터이다．
12) （역자주） SDRAM 등의 메모르］ IC의 시그널 핀 중에서 주소를 지정하기 위한 핀들
13) head. S를 수정하는 것은 좋은 생각이 아니다. 대신에 다른 좋은 방법이 있다. 추가적인 내용은 16장, 뵈눅스 포팅을 참고하
   자．
  烈1    Embedded Linux Primer




       다. 이 단계에서는 문서화되지 않은 기술이 많이 사용된다. 가장 일반적인 경우 중 하나가
       공개되거나 혹은 공개되지 않은 하드웨어의 버그를 피해 가도록 코드를 작성하는 경우다. 만
       약에 스타트업 어셈블리 코드를 수정해야만 하는 경우에는 개발 시간이나 비용이 많이 들 뿐
       아니라 상당히 복잡하다. 그래서 하드웨어를 약간 수정함으로써 소프트웨어 작업 시간을 상
       당히 줄일 수도 있기 때문에 , 하드웨어와 소프트웨어 엔지니어 모두가 이러한 사항들에 대해
       서 하드웨어 개발 초기 단계에 미리 논의를 거쳐야 한다.

       가상 메모리 환경에서 동작하는 시스템의 경우에는 그에 따른 제약 사항을 이해하는 게 중요
       하다. 숙련된 엔지니어 개발자라고 하더라도 가상 메모리 환경에서의 경험은 거의 없는 경우
       가 많다. 그리고 이전에 설명한 페이지 폴트와 같은 함정은 가상 메모리 구조에서 개발자가
       겪을 수 있는 수많은 문제 중 단지 하나의 작은 예에 불과하다. 최근의 32비트 또는 그 이상
       의 마이크로프로세서들은 거의 대부분 가상 메모리 아키텍처를 구현하기 위한 메모리 관리
       장치를 가지고 있다. 가상 메모리를 지원하는 머신이 갖는 가장 큰 장점 중 하나는 커널이나
       다른 소프트웨어 모듈을 프로그래밍 오류로부터 보호해 줌으로써 여러 팀 단위의 개발자들이
       크고 복잡한 어플리케이션을 편리하게 개발할 수 있도록 하는 것이다.


5.2.2 커널 스타트업 : main.c

       커널에 있는 head. o 모듈이 마치막으로 수행하는 일은 제어권을 C로 작성된 커널 스타트업
       파일로 넘기는 것이다. 이제부터 이 중요 파일에 대해서 자세히 보도록 하자．

       각각의 아키텍처에 대해서 물론 문법이나 구현 방법론은 다를 수 있지만, head.o 모듈에서
       커널 본체로 제어권을 넘기는 것은 모든 아키텍처에서 비슷한 구조를 갖는다. ARM 아키텍
       처에 대해서는 다음과 같은 간단한 구문이 이용된다．

         b     start_kernel


       PowerPC의 경우는 다음과 같은 형태를 갖는다．



         Us      r4, start_kernel帥
         o서      r4, r4, start_kernelttl
         Us      r3,MSR_KERNEL@F1
         onj     r3 , r3 ,MS之KERNEL（引


 162
                                                    커널 초기화   Chapter 5




      mtspr    SRRO, r4
      nitspr   SRR1, r3
      rfi




    각각의 어셈블리 문법에 대한 부분은 무시하고 생각하면 두 가지 모두 같은 일을 하는 코드이
    다. 제어권이 커널의 첫 번째1 오브젝트 모듈（head. o）에서 . . . /init/ main. c에 있는 C로
    작성된 루틴인 S七art kernel (）로 넘어가는 것이다. 여기서부터 커널은 스스로자신의 활
    동을 시작해 나가는 것이다．

    이 main. c 파일은 리눅스 커널을 깊이 이해하고 싶거나, 커널이 어떤 요소들로 이루어져
    있는지 , 또 구성 요소들이 어떻게 생성되고 초기화되는치를 이해하고자 한다면 반드시 주의
    깊게 공부해야 하는 파일이다. 최초의 커널 쓰레드를 초기화하는 일에서부터 루트 파일 시스
    템을 마운트하고 최초로 사용자 영역（user space）에서 수행되는 리눅스 어플리케이션을 실행시
    키는 것에 이르기까치 리눅스의 모든 스타트업 작업들이 main. c 파일에서 이루어진다．

    함수 start kernei (）은 main. C 파일에서 단연 가장 큰 함수이다. 리눅스 커널 초기화
    과정의 대부분이 이 함수에서 이루어진다. 여기서는 임베디드 시스템을 캐발하는 입장에서
    유용할 만한 요소들을 간추려서 살펴보고자 한다. 다시 한 번 강조하자. 리눅스 커널을 좀더
    깊이 있게 이해하려면 main. c의 내용을 자세히 분석해 보는 것이 좋다．


5.2.3 아키텍처 셋업
    . . . /ini七／main. c의 S七art kernel () 함수에서 맨 처음 일어나는 일 중 하나는
    se七up arch () 함수를 호출하는 것이다. 이 함수는 하나의 인자를 받는데, 이전에 소개했
    고 다음 섹션에서 자세히 설명할 커널 커맨드 라인에 대한 포인터가 바로 그 인자 값이다．

      setup_arch (&command_li ne) ;


    이 구문은 각각의 주요 아키텍처 전빈에 대한 공통된 초기화 작업을 담당하는 셋업 루틴을
    호출한다. setu1乙arch () 함수는 다앙한 함수들 중에서 현재 시스템에 장착된 CPU를 식
    별하고, 하이 레벨小琯h level)의 CPU 초기화 루틴을 호출할 수 있도록 하는 메커니즘을
    제공해 주는 함수들을 호출한다. 이렇게 se七따） arch () 에 의해서 직접 호출되는 함수들 중
    의 하나가 . . . /arch/arm/kernel/ setup.c에 있는 se七U으processor () 이다. 이 함
 轟 a.     Embedded Linux Primer




        수는 CPU의 ID와 리비전 정보를 점검한다. 그리고 해당 CPU에 맞는 초기화 함수들을 호
        출하고, 부팅 과정 중에 콘솔에 정보 몇 줄을 출력한다．

        출력 내용의 예는 ［리스트 5-3］의 세 번째에서 여덟 번째 줄에서 찾을 수 있다. 프로세서에
        서 직접 읽어들인 CPU 타입과 ID를 나타내는 문자열 그리고 리비전 정보를 볼 수 있다．
        그 다음에 프로세서의 캐시 종류와 크기에 대해서 자세한 내용이 출력된다. 이 예에서는
        IXP425가 32KB의 I（명령어） 캐시와 32KB의 D（데이터） 캐시를 가지고 있다는 내용과 함
        께 추가적으로 내부 프로세서 캐시에 대한 자세한 내용이 출력되는 것을 볼 수 있다．

        아키텍처 설정 함수가 마지막으로 하는 일은 머신에 따른 초기화를 진행하는 것이다. 물론
        동작 메커니즘은 아키텍처마다 서로 다를 것이다. ARM의 경우는 . . . /arch/arm/
        mach叫女에 있는 일련의 디렉터리에서 자신이 사용하는 머신에 맞는 초기화 코드를 찾을 수
        있다. ｝皿PS 아키텍처 역시 참고용 플랫폼을 위한 디렉터리를 가지고 있다. PowerPC의 경
        우는 머신 종속적인 설정 함수들에 대한 함수 포인터를 저장하기 위한 구조체를 정의하고 있
        다. 이 부분에 대해서는 16장, "리눅스 포팅"에서 좀 더 자세히 알아볼 것이다．



5.3 커널 커맨드 라인 처리하71
        아키텍처 설정 이후에 main.c는 일반적인 커널 초기화를 먼저 수행하고 나서 커널 커맨드
        라인을 출력한다. 다음은 ［리스트 5-3］의 열 번째 줄을 다시 나타낸 것이다．

          Kernel command line: console=ttySO,115200 ip=bootp root=/dev/nfs

        이 간단한 예제는, 부팅되는 커널에게 콘솔 장치를 시리얼 포트 장치 七七yS0（일반적으로 맨
        첫 번째 시리얼 포트）를 115Kbps의 변조 속도14) (baud rate）로 설정해서 사용하도록 지
        시하는 것이다. 그리고 시스템의 초기 II) 주소를 BOOTP 서버로부터 받고, 루트 파일 시스
        템을 NFS 프로토콜을 이용해서 마운트하도록 설정한 것을 알 수 있다（BOOTP에 대해서는
        나중에 12장, "임베디드 개발 환경"에서 그리고 NFS는 9장, "파일 시스템"과 12장에서 다룬
        다. 지금은 커널 커맨드 라인에 대해서만 설명할 것이다）.




14) （역자주） baud rate : 변조 속도 또는 일빈적으로 보래잇이라고 부른다. 전송 속도률 표현할 때 사용한다．
                                                            커널 초기화     Chapter 5



       리눅스는 일반적으로 커널 커맨드 라인이라고 불리는 일련의 파라미터들과 함께 부트로더（또
       는 부E入E랩 로더）에 의해서 실행된다. 커널을 직접 쉘（shell) 15）의 명령에 프롬프트에서
       실행시키지는 않지만, 부트로더의 상당수가 명령 프롬프트에서 사용되는 방식과 비슷한 방법
       으로 파라미터들을 천달할 수 있도록 지원한다. 리눅스를 인지하지 못하는 일반 부트로더를
       사용하는 일부 플랫폼의 경우는 커널 커맨드 라인이 컴파일 시점에 정의되어서 커널 바이너
       리 이미지의 일부로 하드 코드（hardHC0ded)16）된다（데스크탑 PC에서 레드햇 리눅스를 구
       동하는 경우와 같은）. 일부 플랫폼에서는 커널을 다시 컴파일할 필요 없이 사용자가 커맨드
       라인을 수정할 수 있게 되어 있다（데스크탑에서 사용되는 Grub이나 Lilo의 경우처럼）. 부트
       스트랩 로더가 설정 파일로부터 커널 커맨드 라인을 읽어 와서 부팅 과정에 커널로 전딜해
       주는 것이다. 이 커맨드 라인 파라미터들은 어떤 머신을 올바르게 부팅시키기 위해서 필요한
       초기 설정 값들을 커널에 전달하기 위해서 사용되는 부팅 메커니즘이다.

       커널 내부에는 상당히 많은 수의 커맨드 라인 파리미터가 정의되어 있다. 커널 소스에서
       . . ./Documentation 디렉터리에는 알파벳 순서로 커맨드 라인 파라미터를 정리한 파일인
       kernel-parameters．七x七 파일을 볼 수 있다. 이전에 말했던 커널 문서에 대한 주의 사항
       을 상기해 보자. 커널이 문서보다 더 빨리 변화한다. 그렇기 때문에 이 문서를 명확한 자료로
       서 사용하기보다는 일종의 안내서로 이용하는 것이 좋다. 이 파일 안에는 400개 이상의 커널
       커맨드 라인 파리미터가 정리되어 있지만, 모든 항목을 전부 포괄하는 것이라고는 볼 수 없
       다. 모든 항목을 확인하기 위해서는 소스 코드를 직접 참조해야 한다.

       커널 커맨드 라인 파라미터 값을 설정하는 기본 문법은 매우 간단한데 이는 ［리스트 5-읾의
       열 번째 줄을 보면 명백하게 알 수 있다. 커널 커맨드 라인 파라미터는 하나의 구문, 즉 '7] =
       값의 쌍으로 이루어지거나, '키＝값1, 값2. . . . ' 형식 즉 키와 하나 이상의 값들로 이루어진
       형식을 갖는다. 전달된 테이터를 처리하는 것은 그 데이터를 사용하는 곳에서 담당한다. 커
       맨드 라인에 대해서는 시스템 전역적17）으로 접근할 수 있으며 많은 모듈에서 필요한 만큼
       사용하게 된다. 이전에 설명한 main. c의 setu1느arch () 함수는 하나의 인자를 받는데 바
       로 이 커널 커맨드 라인이 그것이다. 이는 아키텍처를 위한 파라미터 값들과 구성 지시어들
       을 관련된 아키텍처 및 머신 종속적인 코드에 전달하기 위해서이다.



15) （역자주） 리눅스에서 명령에 프롬프트를 처리하는 프로그램을 쉘佃祀II)이라고 한다. t묘sh, csh 등 다양하다．
16) （역자주） 수정할 수 없도록 어떤 부분어］ 기록되어 버린 것을 하드 코드라고 한다．
17) （역자주） 즉， 커널 내의 모듈들이 직접 커맨드 라인 파라미터의 값히1 접근할 수 있다는 의미이다．
         Embedded Linux Primer




        디바이스 드라이버 개발자나 커널 개발자는 각자 필요에 따라서 커널 커맨드 라인 파라미터
        를 추가할 수도 있다. 그럼 , 그 메커니즘을 한 번 살펴보자．

        안타깝게도 커널 커맨드 라인 파라미터를 사용하고 처리하는 과정을 복잡하게 만드는 요소들
        이 몇 가지 있다. 첫 번째는 기존에 사용하던 구식 방식이 새로운 방식과 함께 여러 곳에 존
        재하기 때문에 횬통이 생길 수 있다는 점이다. 그리고 두 번째는 메커니즘을 완천히 이해18)
        하기 위해서는 링커 스크립트 파일의 복잡한 내용을 이해해야 한다는 점이다．


5.3.1    setup 매크로
        커널 커맨드 라인 파라미터를 이용하는 한 가지 예로서 , 콘솔 디바이스에 대한 옵션을 기술
        하는 경우를 생각해 보자. 여기서는 디바이스 하나를 부팅 초기 단계에 초기화해서 부팅 중
        에 콘솔에 출력될 메시지를 보낼 대상으로 삼고자 한다. 이 초기화는 pril止k.o라는 커널
        오브젝트에서 실행된다. 이 오브젝트에 대한 C 소스 파일은 . . . /kernei/prin七k. c에서
        찾을 수 있다. 콘솔을 초기화하는 루틴의 이름은 C（끄isole se七up () 이고, 커널 커맨드 라
        인 파라미터 문자열을 단일 인자로 받는다．

        여기서 문제는 설정을 위해서 커널 커맨드 라인에 기술한 파라미터 값들과 그 값을 이용하는
        디바이스 드라이버 간에 통신이 어떻게 좀 더 일반적이고 모듈화된 방식으로 이루어질 수 있
        느냐 하는 것이다. 더 난해한 사항은 커맨드 라인 파라미터가 그 파라미터 값을 사용하는 모
        듈보다 먼저（또는 알맞은 때에） 기술되어야 한다는 점이다. 커널 커맨드 라인이 처리되는 주
        된 코드인 main. c의 스타트업 코드가 커맨드 라인 파라미터를 소비하는 모든 모듈에 대해
        서 별도의 명단을 유지하지 않는한, 수백 개의 커맨드 라인 파라미터 각각을 사용하는 모든
        함수를 알 도리가 없다. 여기서 필요한 것이 바로 커널 커맨드 라인 파라미터 값들을 그 소비
        자에게 전달하는 유연하고 보편적인 방법이다．

        리눅스 2.4와 그 이전 커널에서는 이를 위해서 복잡한 코드를 생성하는 매크로를 이용했다．
        바로    se七up 매크로인데 , 지금은 사용하지 않도록 권고되고 있지만, 여전히 커널 전반에
        걸쳐서 폭 넓게 이용되고 있다. 이제 ［리스트 5-3］에 있는 커널 커맨드 라인을 이용해서
         setup 매크로가 동작하는 원리를 설명하도록 하겠다．


18) 꼭 그리 복잡해야 하는 것은 아닌데, 임베디드 개발자 외에는 링커 스크립트 파일까지 이해할 필요는 없다. 링커 스크립트 파
    일에 대해서는 이 장 맨 뒤편에 참고 문서로 니와 있는 GNU LD 매뉴얼에 잘 정리되어 있다．
                                                                              커널 초기화   Chapter 5




이전에 보여 준 커널 커맨드 라인（［리스트 5-3］의 10번째 줄）에서 제일 먼저 나오는 파라미
터 항목이 바로 이 항목이다．

  consol e=ttySo, 115200


우선 여기서는 커널 커맨드 라인을 하나의 예를 통해서 설명하는 것이 목적이기 때문에 파라
미터의 실질적인 의미는 별로 중요하지 않다. 우리의 목적은 메커니즘을 살펴보는 것이기 때
문에 , 인자와 그 값이 이해되지 않더라도 그냥 넘어가도록 하자．

［리스트 5-4］는 . . . /kernel/prin七k. c의 일부를 발췌한 것이다. 함수의 내용을상당부
분 생략했는데 , 설명과는 크게 상관이 없는 부분이기 때문이다. ［리스트 5-띠에서 가장 중요
한 부분은                     setuF) 매크로를 호출하는 맨 마지막 줄이다. 이 매크로는 두 개의 인자를 받도
록 되어 있는데 , 이 경우는 문자열과 함수에 대한 포인터가 인자로 사용되었다. 여기서 문자
열로 넘긴 값의 앞 여덟 글자, 즉 console＝이 콘솔에 대한 커널 커맨드 라인의 시작 부분과
같은 것은 우연이 아니다．

［리스트 5-4] 콘솔 설정 코드의 일부

   /"?
        '            setup a ]list
                     SetUP      jSt 0f
                                    of C0nS0] eS Ca]
                                       consoles.     ]ed fr0m
                                                 Called  from init/ main. c
      " "
       "    /
  static mnt e_init consolesetup(char *str)
  {
                char name[ sizeof (console. cmdline[O] . name) ] ’,
                char*"s , ’놔比化ns;
                m nt idx;


                /*
                     * Decode str into name, index, options.
                     */
                return 1;
  }

      _setup ( "console=", console_setup) ;




                                                                                             167
 難 黨1       Embedded Linux Primer



        여기서 이 매크로가 커널 커맨드 라인의 console 파라미터를 등록하는 것이라는 것을 유추
         할 수 있을 것이다. 실제로는 커널 커맨드 라인에서 console＝이라는 문자열을 만나면
            setup의 두 번째 인자에 설정한 함수, 즉 이 예제의 경우 console setup () 을 호출하
        는 것이다. 그런데 이 정보를 어떻게 이 모듈 밖에 있는 외부의 다른 초기 셋업 코드와 공유
         할 수 있을까2 그 메커니즘은 링커가 생성하는 리스트 항목을 이용하는데 , 상당히 재치 있는
        방법이기도 하지만 어떤 면에서는 약간 난해한 면이 있다．

        자세한 내용은 오브젝트 코드의 일부분에 섹션 속성19)（그리고 다른 속성 값들）을 추가하는
        일을 하는 매크로에 숨겨져 있는데 , 이 매크로들은 복잡한 문법을 감추키 위해서 정의한 것
        이다. 그 목적은 문자열 값과 함수의 주소를 연결한 항목으로 이루어진 정적인 리스트를 만
         들기 위한 것이다. 컴파일러에 의해서 이 리스트는 최종 vmlinux ELF 이미지 안에서 별도
         의 이름을 가진 ELF 섹션에 만들어진다. 이 기술을 이해하는 게 매우 중요한데 , 커널 내부
         의 다양한 곳에서 특수한 목적으로 종종 이 기술이 사용되기 때문이다．

         이제       se七up 매크로의 내부를 한 번 들여다보자. ［리스트 5-5］는 . . . /include/
         linux/mnit. h에 있는 헤더 파일에서            set마）계열 매크로들을 정의하는 부분을 나타낸
         것이다．

        ［리스트 5-5] init.h에 정의되어 있는         setup() 계열 매크로




                                                                                \\ \ \
             #define _setup_param(str, unique_id, fn, early)
                   static char _setup_str_##unique_id[ ] _initdata = str;


                                                                              \ \
                                                                            \ \
                   static struct obs_kernel_param _setup_##unique_id


                                                                            \
                         _ati丁卄）ute_used_
                         _attribute_ ((_ section_(".init. setup")))
                         _attr卄川te_( (al 伯ned( (s仁eof(l ong力）力
                         = { _setup_str_##unique_id, fn, early }

             #define _setup_null_param(str, unique_id)
                    _setup_param(str, unique_id, NULL, 0)

             #define 中setup(str, fn)
                     _setup_paranl(str, fn, fn, 0)




19) （역久阡） 咀：如n at打ibute
                                                                       커널 초기화      Chapter 5



       ［리스트 5_5］는 필자가 볼 때 난해한 문법의 정수라고 할 만하다. ［리스트 5_4J에서 원래의
           setuf) 매크로를 사용하는 부분을 다시 보자．

             _setupC'console=", console_setup) ;

        약간 단순화시켜서 , 컴파일러의 전처리기（PrePr0CeSS0r)20）가 위 매크로를 펼치면 다음과
        같은 결과가 나온다．



            static char _setup_str_console_setup[ ] _initdata = "console=";
            static struct obs_kernel_param 中setup_console_setup \
           _att ri bute_( (_ secti on_ C' . m nit. setup")) )=          \
                {_setup_str_console_setup, console_setup, 0} ;



        좀 더 읽기 쉽게 하기 위해서 두 번째 , 세 번째 줄을 리눅스의 행 계속 문자인＼을 이용해서
        구분했다．

        여기서 두 개의 컴파일러 속성에 대해서는 일부러 설명하지 않았는데 , 현재의 논의에는 별
        도움이 되지 않는내용이기 때문이다. 간단히                       a七tribute used （이 매크로자체도복
        잡한 문법을 숨기기 위한 매크로다）는 컴파일러가 최적화를 실행한 결과, 지정한 함수나 변
        수가 필요 없다고 판단되더라도 그 함수나 변수를 제거하지 않고 그냥 사용21）하도록 만드는
        일을한다.        at七ribu七e       (aligned) 속성은구조체를 예제의 sizeof (long）과같이
        지정한 크기 단위에 맞게 정렬22）시키는 일을 한다.

        이제부터 설명하는 내용이               setup의 동작 메커니즘의 핵심이라고 할 수 있다. 먼저 컴파
        일러는        setup str console        se七up口이라는 문자의 배열을 생성하고 그 값을
        console＝라는 문자열을 갖도록 초기화한다. 그 다음에 컴파일러는 세 개의 구성 요소를 가
        진 구조체를 하나 생성하게 된다. 그 세 개의 요소는 각각 커널 커맨드 라인 문자열（방금 정


20) （역자주） 일부 컴파일러는 옵션 값을 통해서 C 소스 코드를 전처리기만 처리한 결과물을 만들어 낼 수 있다. 그 결과는 모든
    #de丘ne 등의 전처리 구문이 실제의 값들로 대체된 내용이다．
21) 일반적으로 컴파일러는 변수가 S杻血으로 정의되고 있고 천혀 사용되지 않으면 불평하는 메시지를 내보낸다. 즉, 이 지시어를
   지정하지 않을 경우, 미사용 정적 (static) 변수들은 명시적으로 사용되는 부분이 없기 때문어］ 경고 메시지를 출력하게 된다．
22) （역자주） 예를 들어, 없ruct kernel_thread kthrd -曲ibu扼_ (al坦ned(( 16 )))；이라고 한다면 k由rd라는 구조체는 메모리에 16
   의 배수 딘위의 주소에 위치하케 된다. 즉, 缸08000000, 倣0800_0010 , . . . 이런 식이다．


                                                                                         169 1
   器在     Embedded Linux Primer




        의한 문자 배열）, 설정을 수행하는 함수의 주소 값 그리고 간단한 플래그2釗 값이다. 여기서
        마법의 핵심은 구조체 뒤에 달라붙은 섹션 속성이다. 이 속성은 컴파일리에게 이 구조체가
        ELF 오브젝트 내부에 .mnit. setup이라는 이름을 갖는 특별한 섹션 안에 만들어지도록
        지시하는 것이다. 그래［서 링크 단계에서                  Se七up 매크로에 의해서 정의된 모든 구조체들이
        .ini七 . Se七up이라는 섹션 안에 모여서 , 구조체의 배열 형태로 구성되는 것이다．
         . . /ini七／main .O의 일부분을 나타낸 ［리스트 5-6］은 이 데이터를 어떻게 접근하고 이용
        하는지를 보여 주는 코드이다．

        ［리스트 5-6] 커널 커맨드 라인 처리하기

          1 extern struct obs_kernel_param _setup_start[ ], _setup_end[);
          2
          3 static mnt _init obsolete_checksetup(char *line)
           d
           1
               {
           C
           J
                      struct obs_kernel_param *p;
           戶
           b

           日
           ／
                      p = _setup_start;
           8
                      do {
           q
           /
           0
                             mnt n = strlen(p->str) ;
           m
           l
           4
           l
                              if (! strncmp(line, p->str, n)) {
           d
           l
           八J二
                                      if (p->early) {
            ml
                                                /央 Already done in parse_early_param?
           니 (Needs
          13                                     * exact match on param part) */
          14                                   if (line[n] == '\ O ' I I line[nj == ' = ' )
          15                                            return 1;
          16                 } else if (!p->setup_func) {
          17                    printk (KERN_WARNING "Parameter %s is obsolete, '
          18                            " ignored\n", p- .str) ;
          19                        return 1;
          20               } else if (p->setup_func (line + n) )
          21                                return 1;
          22               }
          23                  + ; P+
          24        } while (p < _setup_end) ;
          25        return 0;
          26 }



23) C역자주그 flag : 속성 값 중에서 특히 샹태를 나타내기 위한 것들을 플래그 값이라고 부른다．


I 170
                                                 커널 초기화   Chapter 5




     이 코드는 몇 가지 설명만으로도 충분히 이해할 수 있을 만큼 직관적인 내용이다. 이 함수는
     main. c의 다른 곳에서 파싱된 커맨드 라인 인자 하나를 받아서 호출된다. 지금 다루고 있는
     예제의 경우에 line에 들어오는 값은 커널 커맨드 라인의 구성 요소 중 하나인 console=
     七tySO, 115200 문자열을 가리키는 포인터가 될 것이다. 두 개의 외부 구조체 포인터인
                   Se七up end는 C 소스 또는 해더가 아닌 링커 스크립트 파일에 정의
       setup s七art와L
     되어 있다. 이 이름들은 오브젝트 파일의 .mni七 . setu1> 섹션에 있는 obs kernel param
     구조체 배열의 시작과 끝을 가리킨다．

     ［리스트 5-6］에 있는 코드는 p라는 포인터를 이용해 구조체를 모두 검사해서 이름이 일치하
     는 커널 커맨드 라인 파라미터를 찾아낸다. 이 예제의 경우에는 console＝이라는 문자열을
     찾을 때까지 검색할 것이다. 검색이 된 경우 해당하는 구조체를 통해서 console setup ()
     함수를 가리키는 포인터 값을 얻을 수 있다. 그리고 이 함수를 호출하는데 파라미터의 나머
     지 부분（문자열 t七ySO, 115200）을 인자로 넘긴다. 이러한 과정은 커널 커맨드 라인 내부
     의 모든 파라미터가 완전히 소비될 때까지 반복된다.

      방금 설명한 기술, 즉 오브젝트들을 고유의 이름을 가진 ELF 섹션에 모으는 기술은 커널의
      다앙한 곳에서 사용된다. 이 기술을 사용하는 다른 예로는 mni七 계열의 매크로를 이용해
      서 오브젝트 파일의 공통된 섹션에 최초 한 번만 실행되는 초기화 코드를 모으는 것을 들
      수 있다. 이 매크로의 사촨벌인 initdata는 한 번만 사용되는 데이터들을 정의하도록
      해 준다. 이 initda七a 매크로는 se七up어］ 의해서 사용된다. 이들 매크로에 의해서 표
      시된 함수 및 데이터는 특별한 이름을 갖는 ELF 섹션에 하나로 묶이게 된다. 나중에 이 일회
      용 함수 및 데이터를 사용하고 나면 커널은 이들이 차지하고 있는 메모리 공간을 해제한다．
      아마 부트 과정의 마지막 부분에 출력되는 메시지 . 즉 "Freeing m1lit memory: 296K'와
      같은 익숙한 커널 메시지를 본 적이 있을 것이다. 여기에 표시된 크기는 시스템마다 다를 수
      있지만, 위 예제처럼 1메가의 3분의 1 정도나 절약할 수 있다면 mnit 계열의 매크로를
      충분히 이용할 만할 것이다．이 이유 때문에 바로 이전에 정의한          setup str （兀nsole
      setup口에서도 initdata 매크로가 사용된 것이다.

      아마도 ［리스트 5-6］에서 사용된 함수 이름이 obsolete 24）로 시작하는 게 약간 이상하게
      느껴질 것이다. 이런 이름을 갖는 이유는 커널 개발자가 커널 커맨드 라인을 처리하는 메커
      니즘을 새로운 것으로 바꿨기 때문이다. 즉, 파라미터를 등록하는 과정을 척재 가능 모듈과

24) （역天녀勺 폐기된 것 또는 구식이리는 뜻이다．
 擾 好1     Embedded Linux Primer




        커널 부팅 중에 사용되는 경우 모두를 위한 좀 더 일반화된 방법으로 할 수 있게 되었다. 물
        론지금까지도수백 개의 파라미터가              se七up 매크로를 이용해서 정의되어 있기는 하지만，
        새로 추가되는 것들은 . . . /include/linux/moduleparam.h 커널 헤더에 정의되어 있
        는 일련의 매크로, 특히 moduleparam士 계열의 매크로를 사용하도록 권고하고 있다. 이러
        한 사항에 대해서는 디바이스 드라이버를 소캐하는 8장, "디바이스 드라이버 기초'에서 좀
        더 자세히 설명하겠다．

        새로운 메커니즘은 파싱을 위한 루틴에 미확인（unknown) 함수 포인터를 포함시켜서 , 하위
        호환성을 유지하도록 되어 있다. 그래서 module param士 구조가 인식하지 못하는 파라미
        터들은 미확인 파라미터로 분류된다. 이들 미확인 파라미터는 개발자에 의해서 직접 제어되
        는 방식인 이전 메커니즘을 통해서 처리하도록 되어 있다. 이러한 사항들은 잘 작성된 코드
        인 . . . /kernel/params. c와 . . ./init/ main. c에서 parse args (）를 호출하는 부분
        을 살펴보면 쉽게 이해할 수 있다．

        마지막으로 살펴볼 내용은 1 setup 매크로에 의해서 생성되는 obsHkernelpararn 구조
        체에 정의되어 있는 플래그 멤버 변수의 역할이다. ［리스트 5-6］의 코드를 살펴보면 명확히
        이해가 될 것이다. early라는 이름의 이 플래그는 해당 파라미터가 부팅의 초기 단계에서
        이미 사용된 것인지를 표시하기 위해서 사용된다. 어떤 커맨드 라인 파리미터는 부팅 과정에
        서 다른 파라미터보다 먼저 소비되도록 설정되는데 , 이 메커니즘을 위해서 바로 이 플래그가
        사용된다. main. c에서 doearlyparam() 이라는 함수를 볼 수 있는데 ,             se七up 매크
        로에 의해서 생성된 구조체의 배열을 탐색해서 초기에 소비되어야 한다는 표시25)7} 있는 것
        들을 골라서 처리하는 것을 볼 수 있다. 이 방법을 통해서 개발자는 미리 처리될 파라미터를
        선택할 수 있게 된다．



5.4 서브시스템 초기화
        커널의 많은 서브시스템들이 main. c어］ 있는 코드에 의해서 초키화된다. 가장 초기에 호출
        되는 mnit_timers () 1+ （兀nsole init () 등과 같이 함수를 직접 명시적으로 호출하는
        방식으로 모듈을 초기화하는 경우도 있고, 다른 경우는 앞에서 설명한r                   setur) 매크로와
        비슷한 방식을 이용해서 초기화되는 경우도 있다. 간단히 이야기하면 링커가 다양한 초기화


25) ［역자주） early의 값이 0이 야닌 경우를 말힌디．


I 172
                                                                  커널 초가화   Chapter 5




       함수에 대한 포인터 리스트를 생성하고, 이 함수들을 순차적으로 실행시키는 것이다. ［리스
       트 5-7］을 보면 어떻게 동작하는지 알 수 있다．

       ［리스트 5-7] 초기화 쿠틴의 예

         static mnt _init   customize_machine(void)
         {
             /"'노 customizes platform devices, or adds new ones " /
             if (mnit_machine)
                   init_machineO ;
             return 0;
         }
         arch_initcall (customize_machine) ;



       이 코드는 . . . /arch/arm/ kernel/ se七up . C에서 발췌한 것이다. 이 간단한 루틴은 특정
       한 보드를 위해서 사용자 훅26) (hook）을 제공하도록 작성되어 있다．


5.4. ] 卞 initcall 매크로
       ［리스트 5-7］의 초기화 루틴에 대해서 두 가지 중요한 사항을 주의하자. 첫 번째는 mnit
       매크로를 이용해서 정의하고 있다는 것이다. 앞에서 알아보았듯이 이 매크로는 해당 함수가
       vmlini끄＜ ELF 파일의 . mni七．text 섹션에 위치하도록 섹션 속성을 지정하는 것이다. 오
       브젝트 파일의 특정한 섹션에 이 함수를 위치시키는 이유는 더 이상 사용할 필요가 없을 때
       이 함수가 차지하는 메모리 공간을 재활용할 수 있게 하기 위해서이다．

       두 번째 주목할 부분은 함수를 정의한 바로 다음에 나오는 매크로 arch install
       (customize machine）이다. 이 매크로는 . . . /include/linux/init .h어］ 정의되어
       있는 매크로 중의 하나다. 이 매크로들을 ［리스트 5-8］에 다시 나타냈다．




26) ［역자주） 훅（ho이0 : 프로그래밍 기법 중에서 체인 형식으로 함수들을 묶어서 순서대로 호출하는 방식이다. 주로 메시지 핸들
    러에 자신민의 이벤트 처리를 위한 후킹 함수를 체인에 끼워 넣으면 이벤트가 발생했을 때 자신의 함수도 호출되도록 할 수 있
                                                                           있
    다. 이 예제에서는 11血_mac川ne이 체인에 끼워진 함수를 가리키는 포인터이고， 이 포인터가 유효하면 호출하는 것을 볼 수
  다．
                                                                                  173 1
   難U     Embedded Linux Primer




        ［리스트 5-8) initcall 계열 매크로

           #define _define_initcall (level, fn) \
              static initcall_t _in卄call_##fn _attribute_used_ \
              _attri bute__((_ secti on_(" .ini tcall " level ". i nit "))) = fn

          #define core_initcall (fn)              中的fin已伯仕cal] (11111 !fn)
          #define postcore_initcall (fn)          _define_initcall ("2 " ,fn)
          #define arch_i nitcall (fn)             _defi ne_i ni tcal 1( "3", fn)
          #define subsys_initcall (fn)            _defi ne_i nitcal 1 ("4", fn)
          #define fs_initcall (fn)                _define_initcall ( "5 " ,fn)
          #defi ne devi ce_i ni tcal 1 (fn)       _define_initcall ("6" ,fn)
          #defi ne late_i ni tcal 1 (In)          _defi ne_i ni tcal 1 ("7", fn)



        앞에서 살펴본          setup> 매크로와 비슷한 방식으로 이들 매크로는 함수 이름을 이용해서 데
        이터 요소를 정의하고, 섹션 속성을 이용해서 이들 데이터를 vmlinux ELF 파일 내에 특별
        한 이름을 갖는 섹션에 위치하도록 만든다. 이런 접근 방식의 이점은 main .O에서 잘 알지
        못하는 서브시스템에 대해서도 임의의 초기화 코드를 호출할 수 있다는 것이다. 만약 그렇지
        않다면 main .O가 각 서브시스템을 초기화하기 위해서 커널의 모든 서브시스템에 대해서 알
        고 있어야 한다27) .

       ［리스트 5-8］에서 볼 수 있듯이 섹션 이름은 . mni七callN.ini七이고, 여기서 N은 단계를
       나타내는 1에서 7 사이의 값이다. 데이터 값은 매크로에 기술한 함수에 대한 포인터 값이
       저장된다. ［리스트 5-7］과 ［리스트 5-8］의 예제는 다음과 같은 데이터 값을 정의하게 된다
       （간단히 하기 위해서 섹션 속성은 생략했다）.

          static initcall_t _initcall_ customize_machine = customize_machine;


       이 데이터 값은 커널 오브젝트 파일에서 . initcalll .ini七 섹션에．위치하게 된다．

       단계를 나타내는 (N）은 초기화 함수들이 호출되는 순서를 지정하기 위해서 사용된다. 즉，
       core mni七call () 매크로를 이용해서 정의된 함수들은 다른 것보다 먼저 호출된다. 그리
       고 1兀stcore initcall () 매크로를 이용해서 정의된 함수들이 디음에 호출되는 식이다．
       그래서 late mni七call (）을 이용해서 정의된 함수들이 가장 마지막에 호출되게 된다．

27) ［역자주） 어떤 서브시스템을 시스템에 새로 추가하고 초기화하기 위해서, 매번 main. c를 수정해서 그 서브시스템의 헤더를
    荊nclude 하는 등의 작업을 하는 것은 난센스다．


1174
                                                                                   커널 초기화         Chapter 5



              setup 매크로와 비슷한 방법으로, 士mni七call 계열의 매크로의 경우에도 커널 시작 시
         에 한번 실행하고 다시는 사용되지 않는 초기화 코드들을 등록하기 위한 일종의 등록 함수라
         고 생각할 수 있다. 이 매크로들은 시스템 시작 과정에서 실행시킬 초기화 루틴을 등록하기
         위한 메커니즘을 제공하고, 루틴이 호출된 후에는 코드를 삭제하고, 메모리를 재사용하기 위
         한 메커니즘도 제공한다. 또한 7단계의 실행 순서를 이용해서 언제 초기화 루틴을 실행할지
         도 결정할 수 있다. 그래서 다른 서브시스템이 먼저 가용한 경우에만 사용할 수 있는 서브시
         스템을 하나 개발했다면 이 단계 값을 이용해서 순서를 결정할 수 있다. 커널 코드에
          [a-z] 女 i-ni七call 문자열을 이용해서 grep 명령을 실행하면 이 매크로들이 폭넓게 사용
         되는 것을 볼 수 있을 것이다．

         士 i-ni七call 계열 매크로에 대한 주의사항이 한 가지 있다. 다양한 종류의 mni七call 매크
         로를 이용해서 초기화하는 것은 리눅스 2.6 커널 개발 중혀］ 도입되었다는 것이다. 이전 버전
         의 커널에서는 i-ni七call () 매크로만을 사용하고 있다. 이 매크로는 여전히 수많은 코
         드, 특히 디바이스 드라이버에서 폭넓게 사용되고 있다. 하위 호환성을 위해서 이 매크로는
         다시 device initcall (）로 정의28）되는데, 이는 6번째 단계를 갖는 initcall이다.



5.5 nit 쓰레드
          . . . /ini七／main. c어］ 있는 코드는 커널에 생명을 불어넣는 일을 담당하고 있다. start
         kernel () 함수가 기본적인 커널 초기화를 수행하고, 함수 이름을 통해서 직접적으로 초기
         화 함수를 실행하는 작업을 마친 후에, 최초의 커널 쓰레드가 하나 만들어진다. 이 쓰레드가
         결국에는 프로세스 ID(PID) 1번을 갖는 i-nit () 이라는 커널 쓰레드가 된다. 나중에 배우겠
         지만 mni七 () 쓰레드가 모든 리눅스 사용자 영역 프로세스의 부모가 된다. 이 쓰레드가 만들
         어지는 시점에는 두 개의 각기 다른 쓰레드가 수행중인 상태가 된다. 각각 기존의 start
         kernel (）과 현재의 mnit () 이다. 전자는 이제 자신의 일을 다 마치고 유휴（idle) 프로세스
         가 된다. 후자는 m1lit 프로세스가 된다. 이 내용은 ［리스트 5-9］를 보면 알 수 있다．




28) ［역자주］ . . . 人nclude/Iinux/init. h에 #de丘ne __initcall(fn) device_in批at唯n) 로 정의된 것을 볼 수 있다. 즉 ，기존의 H initcall을
    다시 de너ce_in如세로 대체해서 하위 호환성을 유지했다．


                                                                                                        175 1
 難1     Embedded Linux Primer



      ［리스트 5-9] 커널의 in什 쓰레드 생성

        static void noinline rest_init (void)
               _rel eases (kernel_l ock)
        {
                 kernel_thread(init, NULL, CLONE_FS I CLONE_SIGHAND) ;
                 numa_defaul t_pol i cyO;
                 unlock_kernel O;
                 preempt_enabl e_no_reschedO;

                 ／出
                      * The boot idle thread must execute schedule()
                      央at least one to get things moving:
                      央／/

                 sched山 eQ ;

                 댜）u_idleQ ;
        }



      S七art kernel () 함수는 rest mni上（）을 호출하는데 , 그 내용이 ［리스트 5-9］에 나와
      있다. 커널의 mnit 프로세스는 kernel 七hread () 라는 함수를 호출해서 만들어진다．
      mni七 프로세스는 나머지 시스템 초기화 작업을 마무리하기 위해서 계속 실행되는 반면
      5七ar七 kernel () 을 실행하던 기존 쓰레드는 Cpu idle () 이라는 함수를 호출함으로써 무
      한 루프에서 대기하도록 되어 있다．

      이리한 구조로 동작하는 이유는 아주 흥미롭다. 독자는 아마도 상당히 긴 함수인 start
      kernel () 함수가             mni七 매크로를 사용해서 정의된 것을 인지했을 것이다. 이것은 커널
      초기화의 끝 단계에서는 이 함수가 존재하던 메모리 공간을 해제하고 재활용될 것이라는 의
      미이다. 그래서 이 함수가 차지하고 있던 메모리를 재사용하기 위해서 함수를 끝마치고사용
      하던 주소 공간을 제거할 필요가 있다. 그래서 나온 답이 ［리스트 5-9］에서 보는 것처럼
      S七ar七 kernel () 에서 rest mni七 () 을 호출해서 훨씬 작은 공간을 차지하는 유휴 프로세
      스가 되는 것이다.




176
                                                             커널 초기화     Chapter 5




5.5.1 in仕call을 이용한 초기화
    mnit () 쓰레드가 만들어지면 이 쓰레드는 최종적으로 dominitcalls () 를 호출한다. 이
    함수는 * initcall 계열의 매크로에 의해서 등록된 초기화 함수들을 호출하는 일을 담당
    한다. 이 함수의 내용을 ［리스트 5-10］에 간략히 나타냈다．

    ［리스트 5-10] in仕call올 이용한 초7陣｝

       static void _init     do_initcalls (void)
       {
           initcalUt 山"call ;

           for ( call = &._initcall_start; call < &_initcall_end; call++) {

              if (initcall_debug) {
                 printk (KERN_DEBUG "calling initcall 0x%p", *call) ;
                 print_symbol (":%sO ", (unsigned long) *call) ;
                 printk ( "\ n") ;




              (*call) () ;

       }


    이 코드는 별도의 설명은 필요 없고, 루프의 양쪽 경계를 나타내는 레벨인 1 initcalle
    S七art와     mni七tall end만 살펴보자. 이 레벨들에 대한 정의는 다른 C 파일이나 해더
    파일 어디에도 존재하지 않는다. 이 레벨들은 vmlinux를 링크하는 과정에서 링커 스크립트
    파일을 이용해서 정의되는데 士               initcall 계열의 매크로에 의해서 만들어진 초기화 함수
    들에 대한 목록의 시작과 끝을 나타낸다. 최상위 디렉터리의 System .mal) 파일을 들여다보
    면 이 초기화 함수들에 대한 레벨들을 찾아볼 수 있다. 그리고 ［리스트 5-8］에서 설명한 것
    처럼 이름이 모두          initcall 문자열로 시작된다．

    do mni七calls () 에서 디버깅 정보를 출력하는 부분이 이상하게 보일 수도 있다. 커널 커
    맨드 라인에 mni七call debug 파라미터를 추가하면 이 코드들이 실행되는 것을 볼 수 있
    다. 이 커맨드 라인 파라미터는［리스트 5-10］에 있는 디버깅 정보를 출력한다. 간단히 현재


                                                                              177 1
          Embedded Linux Primer




        사용하는 커널의 커널 커맨드 라인 파라미터에 mni七call debug 파라미터를 추가해서 이
        자체 진단 출력 내용29）을 활성화시켜 보자．

        다음 내용이 바로 디버그 구문을 활성화시켰을 때 출력되는 내용을 예로 든 것이다．




          Calling initcall 0xc00168f4: tty_class_i nit+OxO/0x3c0
          Calling initcall 0xc000c32c: customize_machine+OxO/0x2c()
          Calling initcall 0xc000c4f0: topology_init+OxO/0x24()
          Calling initcall 0xc000e8f4: coyote_pci_init+OxO/0x20()
          PCI: IXP4xx is host
          PCI: IXP4xx using direct access for memory space




        여기서 ［리스트 5-7］에서 본 customize machine () 을 호출하는 부분을 볼 수 있다. 디버
        그 출력 내용에는 이 함수에 대한 커널의 가상 메모리 주소（0xc000c32c）와 함수의 크기
        (0x2c）가 표시되는 것을 볼 수 있다. 이런 내용을 통해서 커널의 초기화 과정을 상세히 살펴
        볼 수 있고 특히 다양한 서브시스템과 모듈들이 어떤 순서로 호출되는지도 알 수 있다. 최소
        한의 구성으로 이루어진 임베디드 시스템이라도 이런 식으로 초기화 함수들이 십여 개가 넘
        게 호출된다. 여기서 예제로 다룬 ARM 엑스스케일 타깃의 경우는 이런 커널 초기화 함수가
        92개나 호출된다．


5.5.2 마지막 부팅 단겨1
        커널은 mnit () 쓰레드가 생성되고 모든 초기화 함수의 호출을 끝마치고 나면 부팅 과정의
        마지막 단계를 수행하게 된다. 여기에는 초기화 함수와 데이터에 의해서 사용된 메모리를 해
        제하고, 시스템 콘솔 장치를 열고, 최초의 사용자 영역 프로세스를 시작시키는 일 등이 포함
        된다. ［리스트 5-11］은 main. c어］ 있는 커널의 mni七 () 쓰레드가 마지막으로 수행하는 코
        드를 보여 주고 있다．



29) 이들 디버그 메시지를 눈으로 보7] 위해서는 먼저 기본 로그 레벨如g level)을 낮춰야 한다. 이 내용어］ 대64서는 리눅스 시스템
    관리를 위한 참고서를 참고하면 될 것이다. 하지만 로그 레벨과 무관하게 커널 로그 파일에는 모든 내용이 기록되므로 여기서
    확인할 수도 있다．


甘 178
                                                                     커널 초기화     Chapter 5



       ［리스트 5너 ]) main.c의 커널 부팅 과정의 마지막 단겨1

          if (execute_command) {
               run_i nit_process (execute_command) ;
               Printk (KERN_WARNING "Failed to execute %s       Attempting "
                                  "defaults. . . \n", execute_command) ;
           }
          run_i ni t_p rocess ("/ sbi n/i n卄") ;
          run_init_process("/etc/init ") ;
          run_i ni t_process ("/bi n/mnit") ;
          run_i ni t_process ("/bi n/ sh") ;

          panic("No -i n-it found.   Try passing init= option to kernel. ") ;



       눈여겨볼 점은 mni七 () 함수가 끝까지 진행되면 커널 패닉30）이 호출된다는 것이다. 특히 임
       베디드 시스템을 실험하는 작업을 하거나, 루트 파일 시스템을 직접 만드는 등의 작업을 진
       행할 때 콘솔에서 이 에러 메시지를 매우 자주 보게 될 것이다. 또한 이 커널 패닉에 대한
       내용은 리눅스와 임베디드 시스템을 위한 공711 게시판 및 사이트에서 가장 많이 볼 수 있는
       질문 사항（FAQ) 중의 하나이다．

       어떻게 해서든 이들 run mnit process () 함수 중 하나는 반드시 오류 없이 성공해야 한
       다. 이 run mnit process () 함수는 성공적으로 실행된 경우 반환되지 않는다. 이 함수는
       자신을 호출한 프로세스의 내용을 새로운 것으로 덮어써서 현재의 프로세스를 새로운 프로세
       스로 대체하는 일을 하기 때문이다. 이 작업을 위해서 익숙한 함수인 execve () 시스템 콜
       을 이용한다. 대부분의 시스템에서 사용자 진영31）을 초기화하는 프로세스로 小bin/mni七
       을 실행시키도록 되어 있다. 그 내용에 대해서는 다음 장에서 자세히 알아보도록 하자．

       임베디드 시스템 개발자가 사용할 수 있는 한 가지 옵션은 직접 작성한 사용자 진영 초기화
       立로그램을 사용하도록 설정하는 것이다. 위에 나타낸 코드에서 볼 수 있는 조건문이 이를
       위해서 있는 것이다. 만약 execute corrunand7} 널（null)이 아닌 경우에는 직접 지정한 사


30) （역자주］ 커녈 패닉 (kernel 1玘nic) : 커널이 해결할 수 없는 심각한 오류를 만나면 호출하는 함수. MS \Nindo邸의 경우어］도 비
    슷한 역할을 하는 함수（BugCh吐k）가 존재한다. 리눅스의 경우 panic：어］ 인자로 넘어온 내용을 보여 주고 시스템이 정지되며, 윈
  도우의 경우는 유명한 파란 화면이 나타나게 된다．
3') 사용자 진영 (userland）은 사용자 영역에서 동작하는 프로그램, 라이브러리, 스크립트 등을 지칭하는 용어로 자주 사默如가．


                                                                                      179 1
     Embedded Linux Primer




   용자 영역에서 실행될 명령에 문자열을 가리키는 포인터 값을 가지고 있게 된다. 5장의 앞부
   분에서 살펴뵨           setup () 매크로를통해서 이 명령어를 커널 커맨드 라인을통해서 지정할
   수 있다. 여기서 살펴본 여러 개념을 종합해서 커널 커맨드 라인을 예제로 만들어 보면 다음
   과 같은 형태가 될 것이다．

     initcall_debug init=/sbin/myinit console=ttySl,115200 root=/dev/hdal

   이 커널 커맨드 라인은 초기화 루틴의 디버킹 정보를 출력하도록 설정하고, 초기 콘솔 장치
   를 115kbps의 속도로 설정한 /dev/ttySl을 사용하도록 지시한다. 또한 루트 파일 시스템
   의 /sbin에 있는 myinit이라는 직접 작성한 프로그램을 사용자 영역 초기화 프로세스로서
   실행시키도록 설정한다. 그리고 마지막으로 루트 파일 시스템을 시스템의 첫 번째 IDE 하드
   디스크인 /dev/hdal 장치를 이용해서 마완i시키도록 하고 있다. 그리고 대체로 커널 커맨
   드 라인에 기술하는 파라미터들의 순서는 크게 의미가 없다. 다음 장에서는 사용자 영역에서
   이루어지는 초기화에 대해서 살펴보도록 하자．



5,6 요약
    口 리눅스 커널 프로젝트는 방대하고 복잡하다. 최종 결과물 이미지의 구조와 내부 구성 요
         소를 이해하는 것이 임베디드 프로젝트를 자신에게 맞게 수정하는 법을 이해하는 핵심
         사항이다．

    口 많은 아키텍처가 리눅스 커널이 실행되기 위해써 필요한 적절한 실행 환경을 갖추기 위
         해서 아키텍처에 맞는 부트스트랩 로더를 커널 바이너 리 이미지에 하나로 합치는 방식을
         이용한다. 그리고 이러한 부트스트랩 로더의 기능을 커널 본체와 구별하기 위해써 그 빌
         드 과정을 알아보았다．

     [a 초기화 단계에서 제어권이 어떻게 흘러가는지를 이해하는 것은 리눅스 커널을 깊이 이해
         하고 특정한 요구 사항을 위해써 커널을 수정하는 방법에 통찰력을 갖도록 해 준다．

    口 커널의 진입점인 head.o를 알아보고, 제어권이 최초의 C 파일인 main. c로 넘어가는
         과정을 알아보았다. 부팅 시스템과 이 시스템이 출력하는 메시지를 살펴보았고, 이와 함
         께 중요한 초기화 개념들에 대해서도 개략적으로 살펴보았다．
                                                                    커널 초기화   Chapter 5



         口 커널 커맨드 라인 파라미터를 정의하고 처리하기 위한 메커니즘을 알아보았다. 여기에
           링커가 생성한 테이블을 이용해써 다잉斟 익명의 초기화 함수들을 호출할 수 있는 고급
           코딩 기법에 대해서도 자세히 알아보았다．

         口 커널 부팅의 마지막 단계에서는 최초의 사용자 영역 프로세스들을 생성한다. 이 메커니
           즘을 이해하면 임베디드 리눅스의 시작에 관련된 내용을 자신에게 맞도록 수정하고 문제
           를 해결할 수 있게 될 것이다．



5.6. ] 더 읽01 보기
         GNU 컴파일러 컬렉션 문서 :
         http: //gcc. gnu. org/onhinedocs/gcc32)


         GNU 링커인 LD 사용법
         http: //www. gnu. org/software/binutils/manual/id-2. 9.1/id.html


         커널 내부 디렉터리 :
         . . . /Documentation/kernel-parameters. txt




32) 그 중에서도 섹션과 함수 속성, 타입 속성, 기타 다양한 속성 값들에 대한 내용을 참고하기 닙尾f다．
口治再相和 6



                     시스템 초기화




이번 쟁게서 배숄 내용

  . 루트 파일 시스템

  U 커널의 마지막 부팅 단계

  . In仕 프로세스

  口 초기 램디스크

  . initramis 사용하기

  U 종료

  U 요약
    Embedded Linux Primer




   2장, "임베디드 처음 경험하기"에서 리눅스 커널 자체는 임베디드 리눅스 시스템을 이루는
   하나의 작은 요소에 불과하다는 점을 지적한 적이 있다. 커널이 자신을 초기화하는 과정을
   마친 후에는, 루트 파일 시스템을 반드시 마운트해야 하고 개발자가 설정한 일련의 초기화
   절차를 실행시켜야 한다. 이 장에서는 커널이 초기화된 후의 시스템 초기화 과정에 대해서
   알아보도록 하자．

   가장 먼저 루트 파일 시스템과 그 구조에 대해 살펴보는 것으로 시작하자. 그 다음에 최소
   조건만을 충족하는 시스템 구성을 만들어서 시험해 볼 것이다. 그리고 최소 조건의 시스템
   기능을 추가해서 쓸 만한 임베디드 시스템 구성을 만들 수 있도록 해 본다. 그 후에 시스템
   초기화 과정에 대한 마지막 내용으로 초기 램디스크（또는 'I뇨trd）에 대해 살펴보고 그 용법
   과 동작 방식에 대해서도 알아보자. 마치막으로 리눅스 시스템 종료 방식에 대해서 간단히
   보는 것으로 마무리하도록 하자．



6. ] 루트 파일 시스템
   5장, "커널 초기화'에서 초기화 과정 중에 리눅스 커널이 하는 일들에 대해서 알아보았다．
   그리고 루트 파일 시스템을 마운팅하는 것에 대해서도 몇 번 이야기한 적이 있다. 리눅스는 다
   른 고급 운영체제와 마찬가지로 자신이 제공하는 서비스를 실질적으로 활용하기 위해서 루트
   파일 시스템을 필요로 한다. 비록 파일 시스템이 없는 환경에서도 리눅스를 사용할 수는 있
   지만, 그럴 경우 리눅스의 대부분의 기능 및 활용가치를 얻기 힘들기 때문에 , 루트 파일 시스
   템을 사용하지 않는 것은 그리 좋은 생각이 아니다. 이는 마치 전체 시스템 어플리케이션을
   커대한 디바이스 드라이버나 커널 쓰레드에 전부 몰아넣는 것과 비슷하다고 볼 수 있다.

   루트 파일 시스템이란 파일 시스템 구조에서 기본 바탕으로 마운트되는 파일 시스템을 밀하
   며 간단히 ／로 나타낸다. 9장, "파일 시스템"에서 배우겠지만 일반적으로 아무리 작은 임베디
   드 시스템이라도 파일 시스템의 디렉터리 구조 내의 몇몇 위치에 하나 이상의 파일 시스템을
   마운트시켜 사용한다. 9장에서 소캐할 proc 파일 시스템도 하나의 예라고 할 수 있다. 이
   파일 시스템은 루트 파일 시스템에서 /proc라는 위치에 마운트되는 특수한 파일 시스템이
   다. 루트 파일 시스템은 단순히 파일 시스템들 중에서 계층 구조의 가장 밑바닥에 마운트되
   는 파일 시스템이라고 할 수 있다. 곧 알게 되겠지만, 리눅스 시스템을 위한 루트 파일 시스
   템은 몇 가지 필수 조건을 갖추어야 한다. 즉, 리눅스 루트 파일 시스템은 시스템을 시작시키
                                              시스템 초기화   Chapter 6




    고, 네트워킹 및 시스템 콘솔 을 위한 서비스를 초기화하거나 디바이스 드라이버를 로드하며
    추가적인 파일 시스템을 마운트시키는 등의 작업을 하는 프로그램 및 유틸리티들을 포함하고
    있어야 한다．


6.1.1 FHS : 파일 시스템1 계층 표준
    몇몇 커널 개발자들이 유딕스 파일 시스템의 형태와 구조를 정하기 위한 표준안을 만들었다．
    이 파일 시스템 계층 표준（File System I五erarchy Standard）은 리눅스 배포판과 어플리
    케이션 프로그램 간의 호환성을 위해서 최소한의 기본적인 사항들을 정의하고 있다. 참고 자
    료는 뒷부분의 6.7.1절 "더 읽어 보기"에서 찾아볼 수 있다. UNIX 파일 시스템 구성의 기본
    원리와 디렉터리 구조에 대해서 좀 더 깊은 배경 지식을 얻고자 한다면 FHS 표준안에 대해
    서 조사해 보기 바란다．

    많은 리눅스 배포판이 FHS 표준에서 청의하고 있는 디렉터리 구조와 거의 일치하는 구조를
    가지고 있다. 이 표준안은 각각의 UNIX, 리눅스 배포판 간에 공통되는 하나의 기본 형을
    제공하는 데 목적이 있다. FHS 표준은 어플리케이션 소프트웨어（그리고 개발자）가 파일과
    디렉터리를 포함한 특정한 시스템 요소가 어디에 위치하는지를 예측할 수 있도록 해 준다．


6.1.2 파일 시스템1 비怯1
    공간에 대한 고려 때문에 , 많은 임베디드 시스템 캐발자들이（플래시 메모리와 같은） 부팅 가
    능한 디바이스에 담을 수 있는 아주 작은 크기의 루트 파일 시스템을 만들고, 나중에 하드
    디스크나 네트워크 NFS 파일 서버와 같은 다른 장치에 있는 좀 더 큰 크기의 파일 시스템을
    마운트하는 방식을 취한다. 사실 기존의 작은 루트 파일 시스템이 존재하는 위치에 바로 큰
    크기의 루트 파일 시스템을 마운트시키는 경우도 흔하다. 이 경우에 태한 예는 이 챕터의 뒤
    에 다루는 초71 램디스크（initrd）를 설명하는 부분에서 보도록 하자．

    간단한 리눅스 루트 파일 시스템에서는 다음과 같은 최상위 디렉터리 구조를 볼 수 있다．



       = 七in
       --dev
         etc
       --lib
   難1      Embedded Linux Primer




           I --sbin
           1- -usr
           1--var
           I --tmp


        ［표 6-1)은 이들 각각의 디렉터리에 포함되는 가장 일반적인 내용물에 대해서 정리한 것이다．

        ［표 6-1] 최상위 디렉터리

         디렉터리                      내용물

         bin                       시스템에서 사용자'F 사용할 수 있는 바이너리 실행 파일U

         dev                       디바이스 노드（8장, "디바이스 드라이버 기초" 참고）

         e七C                       현재 시스템의 구성 파일

         lib                       표준 （二 라이브러리 등의 시스템 라이브러리

         abin                      시스템의 관리자 계정에서만 사용되는 바이너리 실행 ii뻗

         usr                       어플리케이션 프로그램을 위해서 2차적으로 파일 시스템이 마운트됨. 일반
                                   적으로 읽기 전용

         var                       시스템 로그， 임시 구성 파일 등의 기타 파일을 담고 있음

         tmp                       임시 파일


        리눅스 파일 시스템 계층에서 최상위 위치는 슬래시 (slash) 문자（/）로 직접 참조할 수 있다．
        예를 들어 , 루트 디렉터리의 내용을 나열하고 싶다면 다음과 같이 입력하면 된다．

           $ is /

        이 명령어는 디음과 비슷한 결과를 출력할 것이다．



           root@coyote:/# is /
           bin dev etc home lib mnt opt proc root sbin tmp usr var
           root@coyote : /#




l) 임베디드 시스템에서는 별도의 사용자 계정이 없이 루트 계정 하나만 있는 경우가 흔하다．


I 186
                                                    시스템 초기화   Chapter 6



    이 목록에는 추가적인 기능을 위한 디렉터리 항목인 /mn七와 /proc가 있는 것을 볼 수 있다．
    이들 디렉터리를 접근할 때 앞에 슬래시 문자를 붙이면 최상위 디렉터리로부터 시작하는 경
    로를 통해서 디렉터리를 참조한다는 것을 의미한다．


6.1.3 최소 파일 시스템1
    루트 파일 시스템의 필요 조건을 예를 들어 설명하기 위해서 최소（II血血na1) 루트 파일 시스
    템을 하나 만들었다. 이 예제는 엑스스케일 프로세서를 사용하는 ADI 엔지니어링 코요테 참
    고용 보드에서 작업한 것이다. ［리스트 6-1］에는 이 최소 루트 파일 시스템을 마운트한 시스
    템 상에서 tree 명령어를 실행한 결과를 나타낸 것이다．

    ［리스트 6-1] 최소 루트 파일 시스템의 내용



      I- - L너n
      I    I- - busybox
      I    ' U1 sh -> busybox
      I- - dev
      I    ' 1U console
      I-- etc
      I    ' U1 init. d
      I         ' 41 rcs
      1 口U ] lb
           I- - ld-2. 3. 2. so
           I- -ld- linux. so. 2- >ld- 2. 3. 2. so
           I- - libc-2. 3. 2. so
           '- -libc. so. 6- >libc- 2. 3. 2. so

      S directories, 8 files



    이 루트 구성은 임베디드 시스템을 위한 인기 있는 툴킷（to아kit）인 busybox를 이용하도록
    만든 것이다. 간단히 얘기해서 busybox는 많은 리눅스 커맨드 라인 유틸리티를 제공하는
    독립 바이너리 파일이다. 임베디드 시스템에 있어서 bus ybox는 정말 유용한 툴이기 때문에
    11장, "BusyBox" 천체를 할애해서 이 유틸리티에 대해서 설명할 것이다．




                                                                    187
 難t 1        Embedded Linux Primer




         ［리스트 6-끄에 나온 대로 여키서 예로 든 최소 루트 파일 시스템은 5개의 디렉터리에 파일
          8개만을 갖고 있다. 이 루트 파일 시스템은 비록 매우 작지만 부팅 후에 시리얼 콘솔을 통해
          서 사용자가 완벽하게 동작하는 커맨드 라인 프롬프트를 사용할 수 있다. 사용자는 busybo
          ><2）에서 사용할 수 있도록 되어 있는 모든 명령어를 이용할 수 있다．

          ibmn 디렉터리 다음에는 busybox 실행 파일과 bus ybox를 다시 가리키는 소프트 링크인
          sh7} 있다. 이 소프트 링크가 왜 필요한 지는 잠시 후에 설명하겠다. /dev 아래에는 입출력
          에 필요한 콘솔 디바이스를 열기3) 위해서 필요한 디바이스 노드（de毗e node)4)7} 하나 있다．
         비록 반드시 필요한 파일은 아니지만, /e七c/mni七．d에 있는 rcS 파일은 bus ybox어］ 의해
          서 부팅 초기에 기본 값으로 처리되는 초기화 스크립트 파일이다. rcS 파일이 존재하지 않으
          면 rcS7} 없다는 메시지는 물론이고 busybox가 생성하는 모든 경고 메시지를 표시하치 않
          도록 되어 있다．

          마치막으로 필요한 디렉터리와 파일은 두 개의 라이브러리인데 GLIBC(libc-2 .3.2. so)
          와 리눅스 동적 로더5) (id小2.3.2. so）이다. GLIBC는 대부분의 어플리케이션이 사용하는
         printf () 등의 표준 （그 라이브러리 함수를 가치고 있다. 리눅스 동적 로더는 바이너리 실행
          파일을 메모리로 불러들이는 일은 물론이고, 프로그램이 공유 라이브러리에 존재하는 함수들
          을 참조（reference）하기 위해서 필요한 동적인 링크를 수행한다. 그리고 두 개의 소프트 링
          크를 볼 수 있는데 id-linux. so. 2는 id-2.3.2. s(＞를 가리키고, libc. so. 6은
          iibc-2. 3. 2. so를 가리키는 것을 볼 수 있다. 이 링크들은 거의 대부분의 리눅스 시스템에
          서 볼 수 있는데 , 라이브러리 간에 버전별 호환성과 하위 호환성을 위한 것이다．

          이 간단한 루트 파일 시스템으로도 온전하게 기능하는 시스템을 갖출 수 있다. 여기서 테스트
          한 姐M／엑스스케일 보드에서는 이 작은 루트 파일 시스템의 크기가 약 1.7MB 정도였다．

          여기서 재미있는 것은 이 용량의 80% 이상을 C 라이브러리가 차지하고 있다는 것이다. 만
          약 독자의 시스템에서 루트 파일 시스템의 용량을 더 줄여야 한다면 http://libraryopt.
          sourceforge.net에서 라이브러리 옵티마이저 도구에 대해서 알아보기 바란다．


2) BusyBox 명령어는 11장에서 다룬다．
3) 파일을 열기 위한 함수의 이름은 이羌no이다. 닫기 위한 것은 close 0이다. 여기서는 열기, 닫기 함수라는 용어 대신에 영문을 그
   대로 이용했다. 더 많이 사용되기 때문이다．
4) 디바이스 노드어］ 대해서는 8장에서 자세히 설명한다．
5) （역天阡） linux dynamic loader
                                                           시스템 초기화     Chapter 6




6.1.4 루트 파일 시스템의 도전 과저1
        임베디드 장치를 위한 루트 파일 시스템을 구성할 때 발생할 수 있는 어려운 문제들에 대해서
        설명하기는 쉽지만, 해결하는 것은 그리 간단하지 않다. 만약 개발하는 시스템이 충분히 큰
        크기의 하드 드라이브나 플래시 저장 장치를 보드에 장착한 경우가 아니라면 어플리케이션과
        유틸리티들을 작은 메모리 공간에 모두 넣을 수 있도록 만드는 것은 그리 간단한 일이 아니
        다. 물론 플래시 메모리의 가격이 계속 떨어지고는 있지만 시장에서의 경쟁 때문에 가격과
        속도에 대한 압박은 언제나 존재하게 된다. 임베디드 운영체제로서 리눅스가 계속 인기를 얻
        고 있는 가장 큰 이유 중의 하나가 방대하면서도 지속적으로 늘어나고 있는 리눅스 어플리케
        이션 소프트웨어 때문이다．

        주어진 용량 조건에 맞도록 루트 파일 시스템을 다듬는 일은 엄두도 못 낼 만큼 어렵게 느껴
        질 수도 있다. 패키지6）와 서브시스템 중에는 수십에서 수백 7가 이상의 파일을 가진 경우도
        많다. 그리고 많은 패키지가 어플리케이션 자체 외에도 구성을 위한 파일, 라이브러리 파일，
        구성 유틸리티 , 아이콘, 문서 파일 , 국제화를위한지역화파일7) , 데이터베이스 파일 등등을
        가치고 있다. 아파치8) 소프트웨어 재단의 아파치 웹 서버는 임베디드 시스템에서 자주 찾아
        볼 수 있는 유명한 어플리케이션의 예라고 할 수 있다. 많은 사용자를 갖고 있는 한 임베디드
        리눅스 배포판의 경우는, 내부에 포함되어 있는 기본 아파치 패키지에 254개의 파일을 가지
        고 있다. 뿐만 아니라 이 파일들이 단순히 파일 시스템의 단일 디렉터리에 모두 복사되어 있
        는 것이 아니다. 일부 파일은 별도의 설정 절차 없이 아파치 어플리케이션을 구동시키기 위
        해서 파일 시스템 상의 여러 위치에 복사해야 한다．

        이런 사항들은 기본적으로 배포를 위한 7隆 관점으로 생각할 수 있는데 , 결국 단조로운 작업
        에 해당한다. （데스크탑 및 엔터프라이즈 마켓 부분의） 레드햇이나 （임베디드 마켓 부분의）
        몬타 비스타（Monta Vista Software）와 같은 리눅스 제공 업체의 경우에는 이 부분만을
        위해서도 상당한 개발 인력을 투자하고 있다. 즉, 리눅스 배포판을 구성하는 요소인 프로그


6) ［역자주） 소프트웨어 묶음을 패키지라고 한다. 즉, Firefox 패키지는 비refox 소프트웨어를 지칭하기도 하고, 설치를 위해서 압축
   해서 묶어놓은 것을 말햐기도 한다．
7) ［역자주） 다양한 언어와 문화를 가진 지역 사람들이 사용할 수 있도록, 여러 문화권을 위한 언어, 표현 방식 등을 위한 파일을
   갖고 있다. 이것을 국제화恤ternation訌切a如n）를 지원한다고 햐며, 각각의 지역에 맞도록 하는 작업들을 지역화(I仗川ization）라고
  한다．
8) （역자주） 아파치 웹 서버는 젼 세7카 웹서버의 50% 이상을 점유하고 있다. N侃ro曲의 웹 서버의 거센 도젼을 받고 있다（참고
   http:7/news. net工aft. corn/archives/web_s三rver_survey. html).


                                                                             189 甘
    茹U        Embedded Linux Primer




          램 , 라이브러리 , 툴, 유틸리티 그리고 어플리케이션을 한데 묶어서 패키징하는 작업에 상당
          한 투자를 하고 있다. 결국 작은 규모의 루트 파일 시스템을 만들기 위해서도 이러한 배포를
          위한 기술을 필요로 하는 것이다．


6.1.5 시행착오를 반복하는 방법
          최근까지 루트 파일 시스템에 내용을 추가하기 위한 유일한 방법은 한번 해보고 되는지 확인
          하는 것이었다. 물론 작업 과정을 일련의 스크립트 파일을 이용해서 자동화할 수는 있지만，
          어떤 기능을 위해서 어떤 파일이 필요한지를 파악하는 것은 여전히 개발자의 몫이었다. 레드
          햇 패키지 관리자（rpm : Redhat Package Manager）와 같은 툴을 이용하면 루트 파일 시
          스템에 패키지를 설치할 수 있다. rpm은 패키지 간의 의존성을 해결하기 위한 합리적인 방법
          을 제공하지만, 깊이 파고들수록 더욱더 어려운 내용을 이해해야 한다. 거기에다 rpm은 작은
          크기의 루트 파일 시스템을 만들기 위해서 필요한 기능인, 도움말 문서나 사용하지 않는 유
          틸리티 등의 불필요한 파일을 설치 시에 제외시키는 기능이 부족한 편이다．


6.1.6 차동화된 파일 시스템1 제작 툴
          임베디드 리눅스를 제공하는 선두 업체들은 플래시나 다른 디바이스에 루트 파일 시스템을
          자동으로 구성해 주는 훌륭한 툴을 제공하기도 한다. 이 툴은 기본적으로 그래픽 인터페이
          스를 가지고 있으며 , 개발자가 기능 또는 어플리케이션별로 파일을 선택할 수 있도록 해 준
          다. 그리고 패키지 내에서 문서나 기타 사용하지 않는 파일을 제외시킬 수 있는 기능은 물론
          이고, 각각의 파일 단위로 추가할지 말지를 선택할 수 있도록 하는 기능을 가진 것들도 많
          다. 이 툴은 나중에 디바이스에 맞게 설치할 수 있도록 파일 시스템을 다양한 포맷으로도
          만들어 낼 수 있다. 이 툴에 대한 세부 사항은 사용하는 임베디드 리눅스 제공 업체에 문
          의9）하기 바란다．



6.2 커널의 마지막 부팅 단계
          이전 장에서는 시스템 부팅 과정의 마지막 단계에서 커널이 수행하는 작업을 알아보았다．
         ［리스트 6-2］는 . . . /init/ main C 코드의 마지막 부분을 나타낸 것이다．


9) （역자주） hi加：//linuxdevices. com/articles/AT3617019494. html을 챰고하자．
                                                               시스템 초기화      Chapter 6



      C리스트 6-2] main.c의 마지막 작업



             if (execute_command) {
                     run_i nit_process (execute_command) ;
                     printk (KERN_WARNING "Failed to execute %s. Attempting "
                                          "defaults. . . \n", execute_command) ;
             }

             run_init_process("/sbin/init ") ;
             run_init_process("/etc/init ") ;
             run_i ni t_process("/bi n/i nit") ;
             run_init_process("/bin/sh") ;

             panic("No mnit found. Try passing init= option to kernel. ") ;



      이 코드는 부팅의 마지막 단계에서 생성된 mni七이라는 쓰레드에 의해서 수행되는 작업들을
      보여 주고 있다. 여기서 run mnit process () 함수는 아주 재미있는 동작을 하는 커널
      시스템 콜 함수인 execve () 함수를 감싸고 있는 단순한 랩페0)（咐apper) 함수이다．
      execve () 함수는 성공적으로 수행된 경우에는 절대 반환되지 않는다. 이 함수를 호출하는
      쓰레드의 메모리 공간이 인자로 전달된 프로그램의 이미지로 덮어써지게 된다. 사실 호출하는
      쓰레드가 바로 새로운 立로그램으로 대체되는테 , 이때 프로세스 ID(P11力도 넘겨받게 된다．

      위 초기화 과정의 구조는 리눅스 커널이 발전하는 긴 시간 동안 바뀌지 않았다. 사실 리눅스
      1.0도 현재와 비슷한 구조를 가지고 있다. 본질적으로 이 부분이 의미하는 것은 사용자 영역
      프로그램이 처음 시작된다는 것이다. ［리스트 ＆외에서 볼 수 있듯이 , 만약 호출된 함수들이
      모두 실패할 경우에 커널은 panic () 시스템 콜에 메시지를 보내서 에러 메시지를 출력한
      후에 시스템을 중단시키게 된다. 만약 독자가 얼마간 임베디드 리눅스 시스템에 관련된 작업
      을 해 봤거나, 그 중에서도 특히 루트 파일 시스템과 관련된 작업을 해 본 경험이 있다면 커
      널의 panic () 함수와 그 메시지에 대해서 좀 더 친숙할 것이다！ 구글에서 이 panic () 에
      러 메시지를 검색해1 보면 관련된 FAQ 페이지를 무수히 많이 볼 수 있을 것이다.




10) （역자주） MTaPI光r 함수는 본 기능을 하는 다른 함수나 로직을 감싸는 역할만을 하는 함수를 말한다. 실제 함수가 호출되기 전
   어］ 간딘히 추가적인 작업을 할 경우어］ 사寄 다．
   驥1     Embedded Linux Primer




        여기서 실행시킬 프로세스들은 모두 ［리스트 &1]에서 본 것과 비슷한 루트 파일 시스템 내
        에 존재하도록 되어 있는 프로그램이다. 이를 통해서 mni七 프로세스가 정상적으로 통작하기
        위해서 커널이 최소한으로 요구하는 사항이 무엇인지 알 수 있다．

        ［리스트 ＆기를 보면 최소한 하나의 run mnit process () 함수는 반드시 성공해야 한다
        는 것을 알 수 있다. 커널이 함수들이 호출되는 순서대로 총 네 개의 프로그램을 실행하려고
        시도하는 것을 볼 수 있다. 리스트에서 보듯이 네 개의 프로그램 중에서 성공적으로 실행된
        것이 하나도 없을 때는 커널이 공포의 panic () 함수를 호출하고 그 순간 시스템을 정지시킨
        다. 지금 설명한 . . . /ini七／main. c의 일부 코드는 부팅 시에 한번만 호출된다는 것을 기
        억해 두자. 만약에 함수 호출이 하나도 성공하치 못하면 커널은 panic () 함수를 호출함으
        로써 불평을 늘어놓고 시스템을 중지하는 것밖에 할 수 있는 게 없다．


6.2. ] 최초 사용자 영역 프로그램

        대부분의 리눅스 시스템에서 커널에 의해 최초로 실행되는 프로그램은 /sbin/init이다．
        그래서 ［리스트 6-2］에서도 맨 처음에 실행하려고 시도하는 것을 볼 수 있다. 일반적으로
        이 프로그램이 최초로 실행되는 사용자 영역 프로그램이 된다. 다음의 처리 순서를 재검토해
        보자．

          1. 루트 파일 시스템을 마운트한다．

          2. 최초 사용자 영역 프로그램을 실행한다. 여기서는 mnit이 그것이다．

        ［리스트 &2］의 코드가 여기서 예로 든 최소 루트 파일 시스템을 사용하는 시스템에서 실행
        될 경우는 루트 파일 시스템에 mnit이라는 이름을 가진 실행 파일이 어디에도 존재하치 않
        기 때문에 처음 세 번의 사용자 프로그램의 실행은 실패하게 된다. ［리스트 6-1]에서
        busybox를 가리키는 소프트 링크인 sh7下 있었던 것을 떠올려 보자. 이제 이 소프트 링크의
        용도를 이해할 수 있을 것이다. 즉, 커널의 초기 프로세스로서 사용자 영역에서 일반적으로
        필요한 쉘 프롬프트 기능까지 제공해 주는11) busybox를 실행시킬 수 있게 해 준다．




11) ［역자주） 심볼 링크인 sh를 통해서 busybox7} 실행되면 busybo,는 쉘을 실행시킨다. 이는 11장에서 자세히 다룬4


j192
                                                            시스템 초기화   Chapter 6




6.2.2 의존성 해볕
    단순하게 mnit과 같은 실행 파일을 자신의 파일 시스템에 복사하는 것만으로는 시스템이 정
    상적으로 부팅되기에는 아직 부족하다. 자신의 루트 파일 시스템에 어떤 파일을 추가할 때는
    항상 그 파일의 의존성을 만족시켜야 한다. 대부분의 프로세스가 두 가지 종류의 의존성을
    갖는다. 그것은 동적으로 링크된 실행 파일의 경우 내부에 존재하는 주소 값이 결정되지 않
    은（unresolved) 참조를 해결하는 문제와 어플리케이션이 필요로 하는 구성 파일이나 데이
    터 파일들을 갖추는 문제이다. 전자를 위해서는 툴을 사용할 수 있지만, 후자의 경우는 문제
    의 어플리케이션을 기본적으로라도 이해하고 있어야 알아낼 수 있는 내용이다．

    예를 하나 들어 보면 이해가 쉬울 것이다. 먼저 mni七 프로세스는 동적으로 링크된 실행 파일
    이다. 그래서 mnit을실행시키기 위해서는 라이브러리 의존성을해결해야 한다. 라이브러리
    의존성을 위해서 개발된 도구가 ldd이다. 어떤 어플리케이션이 필요로 하는 라이브러리를
    알고 싶다면 타깃 시스템용 ldd를 실행시키면 된다．



       $ ppc_4xxFP-ldd mnit
             ]ibc. so. 6 => 加pt/el dk／叩c_4xxFP/］化／  ］化C. so. 6
             ld. so. 1 => /opt/eldk/ppc_4xxFP/1卄）/ld. so. 1
       $



    이 idd의 출력을 보면 이 예제의 PowerPC mni七 실행 파일이 두 개의 라이브러리에 의존
    하고 있는 것을 알 수 있다. 이들은 각각 표준 C 라이브러리（libc.so. 6）와 리눅스 동적
    로더（id. so. 1）이다．

    두 번째 종류의 의존성을 해결하기 위해서는 실행 파일이 필요로 하는 구성 파일이나 데이터
    파일을 알아내는 방법은 그 서브시스템을 이해하는 것외에 다른 대안이 없다. 예를 들어，
    mni七의 경우에도 동작 설정을 /etc의 mnm七tab이라는 데이터 파일로부터 읽어 오도록 되
    어 있다. 만약에 6.1.6절 "자동화된 파일 시스템 제작 툴'에서 설명한 것처럼 , 이런 의존성에
    대한 세부 정보를 내장하고 있는 별도의 툴을 사용하지 않는다면 이 정보를 직접 제공해야
    한다．




                                                                            193
 !葬1    Embedded Linux Primer




6.2.3 초키화 과정 수정하기
       시스템 시작 시에 어떤 프로그램을 최초 사용자 프로그램으로 사용할지를 개발자가 직접 설
       정할 수도 있다. 이는 커널 커맨드 라인 파리미터를 통해서 가능한데 , ［리스트 6-2］의
       panic () 구문을 통해서 출력되는 메시지에도 관련된 힌트를 보여 주고 있다. 5장에서 알아
       본 커널 커맨드 라인에 개발자가 i-ni七 프로세스를 직접 설정하는 내용을 추가하면 다음과
       같은 형태가 될 것이다．

         console=ttySO, 115200 ip=bootp root=/dev/nfs init=/sbi n/myi nit


       이렇게 커널 커맨드 라인에 i-ni七＝을 지정한 경우에는 루트 파일 시스템의 /sbin 디렉터리
       에도 반드시 myinit이라는 실행 파일을 넣어야 한다. 이렇게 지정하면 이 프로세스가 커널
       부팅 과청이 종료된 후에 최초로 실행되는 사용자 영역 프로세스가 된다．



6.3 m it 프로세스
       아주 특별한 경우가 아니면 직접 제작한 프로그램을 최초 프로세스로 설정할 일은 거의 없을
       것이다. 이는 기존의 표준 i-nit 프로세스가 매우 유연한 기능을 갖고 있기 때문이다. mni七
       이라는 프로그램과 잠시 후에 다룰 초기 스크립트들은 모두 원래 UNI)( 시스템 V에서 사용
       한 시스템 V m it이라고 일반적으로 부르는 방식에 따라서 구현되어 있다. 이제 이 강력한 시스
       템 구성 및 제어 유틸리티에 대해서 알아보자．

       이전 섹션에서 i-ni七은 커널이 부팅 과정을 마친 후에 처음 실행시키는 사용자 영역 프로세
       스라고 말했었다. 나중에 배우겠지만 리눅스 시스템에서 실행되는 모든 프로세스는 그 시스
       템에서 실행되는 다른 프로세스와 부모e자식 관계를 맺고 있다. i-nit은 리눅스 시스템의 모
       든 사용자 프로세스들의 최상위 부모 프로세스이다. 뿐만 아니라 자식 프로세스들에게 물려
       줄 PATH나 CONSOLE 등을 포함한 기본적인 환경 변수 값을 제공하는 일도 한다．

       mni七 프로제스의 주된 역할은 약속된 구성 파일에 명시된 대로 프로세스들을 추가적으로 실
       행시키는 일이다. 이 구성 파일은 일반적으로 /etc/i-ni七tak) 파일로 저장되어 있다. mnit
       프로세스는 동작 레벨（띠nievel)이라는 개념을 가지고 있는데 , 이것은 일종의 시스템 상태라고
       생각할 수 있다. 각각의 동작 레벨에 대해서 그에 맞게 활성화될 서비스나 실행시킬 프로그
       램을 따로 정의하게 된다．


1194
                                                시스템 초기화   Chapter 6


in'七은 항상 어떤 한 가지 상태를 갖고 있다. mnit어］ 의해서
                                    사용되는 동작 레벨은 0부터
6까지이고, 별도로 특수한 동작 레벨인 S7下 있다. 동작 레벨 0은
                                       mnit이 시스템을 중지
(halt)시키는 경우이고 동작 레벨 6은 시스템을 재부팅시키게 된다
                                       . 각각의 동작 레벨들은
그 레벨에 따라서 시스템이 어떤 동작을 취할지를 결정하는 시작／
                                     종료 스크립트를 가치고 있
다. 주어진 동작 레벨에 따라서 실행시켜야 할 작업은 잠시 후에 설명할
                                          /a七c/inittab 구
성 파일이 결정하게 된다．

여러 배포판에서 일부 동작 레벨은 특수한 목적으로 사용하기 위해
                                                예약되어 있다. ［표 ＆기에
는 많은 배포핀혜서 공통적으로 사용되는 동작 레벨의 용도에
                                            대해서 자세히 정리되어 있다．

［표 6-2] 동작 레벨（Runleve怡）
 동작 레벨             용도
 0                 시스템 셧다운（Halt)
 j                 시스템 관리를 위해서 단일 사용자 구성으로 동작
 2                 사용자7f 정의할 수 있음
 3                 일반적인 멀티유저 환경
 4                 사용자가 정의할 수 있음
 5                 멀티 유저면서 그래픽 사용자 인터페이스로 시쟉햐는 환경
 6                 시스템 재부팅（reboot)


동작 레벨 스크립트는 일반적으로 /etc/ rc . d/ini七 . d 디렉터
                                       리에서 찾아볼 수 있다. 각각
의 서비스를 활성화 또는 비활성화시키는 일을 하는 대부분의 스크립
                                          트를 여기서 볼 수 있다．
서비스는 스크립트를 start나 stop 또는 restart와 같은 적절한
                                          인자를 넣어서 실행하는
방식으로 수동으로 구성할 수도 있다. ［리스트 6-3］은 nfs
                                      서비스를 재시작（restart）시키
는 예제이다．

［리스트 6-3) NFS 재시작

     $ /etc/ rc.d/ init. d/nfs restart
     shutting down NFS mountd:                  OK
     shutting down NFS daenion:                 OK
     shutting down NFS quotas:                  OK


                                                              195
   難1         Embedded Linux Primer




    [[[[[                                                                   ] ] ] ] mJ
              Shutting down NFS services:                              OK
              Starting NFS services:                                   OK
              Starting NFS quotas:                                     OK
              Starting NFS daemon:                                     OK
              Starting NFS rnountd:                                    OK




            만약 레드햇이나 페도라와 같은 데스크탑용 리눅스를 이용해 봤다면 시스템 시작 시에 나타
            나는 위와 비슷한 메시지들을 분명히 본 적이 있을 것이다．

            동작 레벨은 그 레벨에서 활성화되어 있는 서비스에 의해 정의내릴 수 있다. 대부분의 리눅
            스 배포판이 /e七c/rc .d/init .d 내에 존재하는 서비스 스크립트들에 대한 심볼릭 링크12)
            를 따로 담고 있는 디렉터리를 가지고 있다. 이 디렉터리들은 보통 /etc/rc . d 디렉터리
            밑에 자리 잡고 있다. 여기에서 각각의 동작 레벨의 시작, 종료에 대한 스크립트들을 담고
            있는 디렉터리를 찾을 수 있다. mni七은 단순히 동작 레벨의 진입과 종료 시점에 해당하는
            스크립트를 실행시켜 주는 일을 할 뿐이다. 스크립트 파일이 시스템의 상태를 정의하고,
            inittab 파일은 mni七 프로세스에게 어떤 레벨에서는 어떤 스크립트를 사용할지를 지시하
            는 일을 하는 것이다. ［리스트 6-4］에는 특정 동작 레벨에 진입하고 빠져나가는 시점에 실행
            할 스크립트들을 가지고 있는 /etc/rc.d 바로 밑에 있는 디렉터리를 보여 주고 있다．

            ［리스트 &4] 동작 레벨 디렉터리 구조


              $ is -i /etc/ rc. d
              total 96
              drwxr-xr- x 2 root root 4096 oct 20 10:19 init. d
              -rwxr-xr- x 1 root root 2352 Mar 16 2004 rc
              drwxr- xr- x 2 root root 4096 Mar 22 2005 rc0. d
              drwxr- xr-x 2 root root 4096 Mar 22 2005 rcl. d
              drwxr- xr-x 2 root root 4096 Mar 22 2005 rc2. d
              drwxr- xr-x 2 root root 4096 Mar 22 2005 rc3. d
              drwxr- xr水 2 root root 4096 Mar 22 2005 rc4. d
              drwxr- xr- x 2 root root 4096 Mar 22 2005 rc5. d
              drwxr-xr- x 2 root root 4096 Mar 22 2005 rc6. d
              -rwxr- xr- x 1 root root   943 Dec 31 16: 36 rc.local
               rwxr- xr- x 1 root root 25509 Jan 11 2005 rc. sysinit




12) ［역자주） 釣ft link와 같은 의미이다. 하드 링크（hard link）와 반대 의미인데， Windo＼怜의 바로 가기와 같은 개념이다．


1196
                                                               시스템 초가화       Chapter 6



      각각의 동작 레벨에 해당하는 스크립트는 rcN.d어］ 정의되어 있다（여기서 N은 동작 레벨을
      나타낸다）. 이들 rcN.d 디렉터리 내부를 보면 정해진 순서로 정렬되어 있는 심볼릭 링크들
      을 볼 수 있다. 각각의 심볼릭 링크의 이름은 K 또는 S로 시작한다. S로 시작하는 것은 시작
      (startup) 명령에 의해서 실행되는 서비스 스크립트를 나타낸다. 그리고 K로 시작하는 것은
      종료（shutdown) 명령에 의해서 실행되는 서비스 스크립트를 나타낸다. 아주 작은 수의 서
      비스를 가진 시스템을 하나 가청해 보면 다음과 같은 형식의 링크를 가지고 있을 것이다．

      ［리스트 &5] 동작 레벨 디렉터리의 oil

         lrwxrwxrwx 1 root root 17 Nov 25   2004 S10network -> . ./init. d/network
         lrwxrwxrwx 1 root root 16 Nov 25   2004 sl2syslog -> . ./init. d/syslog
         lrwxrwxrwx 1 root root 16 Nov 25   2004 S56xinetd -> . ./init. d/ xinetd
         lrwxrwxrwx 1 root root 16 Nov 25   2004 K50xinetd -> . ./init. d/xinetd
         lrwxrwxrwx 1 root root 16 Nov 25   2004 K8Ssys1og -> . ./init. d/ syslog
         lrwxrwxrwx 1 root root 17 Nov 25   2004 K90network -> . ./init. d/network



      이 가상의 예에서는 서비스를 시작시키기 위한 세 개의 시작 스크립트를 볼 수 있는데 각각
      network, syslog 그리고 xine七d가 그것이다. S로 시작하는 스크립트는 S 다음에 숫자
      부분이 있기 때문에 이 숫자 순서대로 실행될 것이다. 비슷한 방식으로, 동작 레벨에서 빠져
      나갈 때도 역시 xinetd, syslog 그리고 ne七i四rk 이렇게 세 개의 서비스를 중단시킨다．
      종료 스크립트들 역시 심볼릭 링크의 이름에서 K 다음에 오는 두 자리 숫자의 순서대로 실행
      되도록 되어 있다. 실제 시스템에서는 더 많은 스크립트가 이용되는데 , 여기에 독자의 어플
      리케이션을 위해서 직접 파일을 추가할 수도 있다．


6.3.1 inittab
      mnit은 실행되면 /e七c/mni七tab이라는 이름을 갖는 시스템 구성 파일을 읽어 들인다. 이
      파일은 모든 실행 레벨에서 실행시킬 명령은 물론이고, 각각의 레벨에서 실행시킬 명령을 가
      지고 있다. 이 파일과 mnit의 동작에 대해서는 시스템 관리에 관한 여러 서적과 대부분의
      리눅스 워크스테이션에서 볼 수 있는 맨 페이지13) (man page）에 잘 문서화되어 있다. 그래
      서 여기서는 자세한 동작 원리를 다루지 않고, 개발자의 입장에서 mni七tab을 자신의 시스
      템에 맞게 구성하는 방법에 초점을 맞추도록 하겠다. mnit七ab과 mnit이 어떻게 서로 동작

13) （역자주） 맨 패이지는 리눅스／유닉스의 도움말 유틸리티인 man을 통해서 볼 수 있는 문서를 말한다．


                                                                                     197 1
   鞋1     Embedded Linux Primer



       하는지에 대한 자세한 내용은 man mnit 또는 man inittab을 입력하면 대부분의 리눅스
       시스템에서 해당 문서를 볼 수 있다．

       간단한 임베디드 시스템에서 사용되는 전형적인 inittab을 한 번 보도록 하자. ［리스트
       6-6］은 시스템 종료（shutdown）와 재부팅 외에 하나의 동작 레벨을 지원하는 시스템에서
       사용되는 inittab의 예를 보여 주고 있다．

       ［리스트 &6] 간단한 inittab 예제

          # /etc/inittab

          # The default runlevel (2 in this example)
          id: 2:initdefault:

          # This is the first process (actually a script) to be run.
          si : :sysinit: /etc/ rc. sysinit

          # Execute our shutdown script on entry to runlevel 0
          10: O: wait: /etc/init. d/ sys. shutdown

          # Execute our normal startup script on entering runlevel 2
          12: 2: wait: /etc/init. d/runlvl2. startup

          # This line executes a reboot script (runlevel 6)
          16: 6: wait: /etc/init. d/ sys. reboot

          # This entry spawns a login shell on the console
          # Respawn means it will be restarted each time it is killed
          con :2: respawn : /bi n/ sh



       이 매우 간단한14) inittab 스크립트는 세 가지의 동작 레벨을 기술하고 있다. 그리고 각각
       의 동작 레벨은 하나의 스크립트와 연결되어 있는데 , 개발자가 각각의 동작 레벨에서 실행시
       킬 작업들을 작성해서 만들어 놓아야 하는 파일들이다. mni七이 위 mni七七ab 파일을 처음
       읽어서 실행시키는 스크립트는 /etc/rc. sysinit이 된다. 이 스크립트는 sysinit이라
       는 이름으로 표시되어 있다. 그리고 mnit은 동작 레벨 2로 진입하게 되고, 레벨 2에 정의되
       어 있는 스크립트를 실행시킨다. 이 예제에서는 /etc/ mni七. d/runivl2 . startup이 그

14) 이 inittab 예제는 특정한 임베디드 시스템을 위한 간단한 inittab 파일이 아주 좋은 예이다．

1198
                                              시스템 초기화   Chapter 6




    스크립트가 된다. ［리스트 6-6］의 :wai七： 태그를 통해 유추할 수 있듯이 init은 이 스크
    립트7} 종료될 때까지 기다린 후에 다음 작업을 계속하게 된다. 레벨 2 스크립트의 실행이
    완료되면 mni七은［리스트 ＆臼의 마치막 줄에서 볼 수 있는 것처럼 (/bin/ sh 심볼릭 링크
    를 통해서） 콘솔 상에 쉘을 하나 실행시킨다. 여기서 respai寸n 키워드는 만약에 쉘이 종료
    되면 매번 다시 실행시키라는 의미이다. ［리스트 6-7］은 앞 예제가 실행될 때 출력되는 내
    용이다．

    ［리스트 6-7] 시작 메시지의 c i



       yES: Mounted root (nfs filesystem) .
       Freeing mnit memory: 304K
       INIT: version 2 .78 booting
       This is rc. sysinit
       INIT: Entering runlevel: 2
       This is runlvl2. startup

       #




    여기서 예를 들어 설명한 시작 스크립트들은 사실 入入쿠7} 어떤 동작을 한다고 알리는 것
    외에 다른 일은 하지 않는다. 물론 실제적인 시스템에서는 이들 스크립트가 기능 및 서비스
    를 활성화하는 등의 유용한 작업을 하게 퇸다. 예제의 간단한 구성 파일을 이용해서 , /e七C'
    mnit. d/runlvl2 . S七artup 스크립트 내부에 자신의 기능에 맞게 서비스나 어플리케이션
    을 실행시키도록 수정할 수 있을 것이다. 반대로 종료 또는 재부팅 스크립트에는 서비스나
    어플리케이션, 디바이스를 사용하지 않도록 설정할 수도 있다. 다음 절에서는 전형적인 시스
    템 구성 파일과 이를 위해서 필요한 시작 스크립트를 몇 가지 살펴보도록 하자．


6.3.2 웸1 서버 시작 스크립트의 예
    비록 간단하기는 하지만, 이 시작 스크립트는 동작 원리를 이해하고 자신만의 시스템에서 시
    작과 종료 동작을 정의하는 데 힌트를 얻을 수 있는 예제이다. 이 예제는 busy加x어］기반한
    것인데, mnm七과는 약간 다른 초기화 동작을 갖고 있다. 그 차이점에 대해서는 11장에서 자
    세히 설명하도록 하겠다．
  礪 藻1      Embedded Linux Primer




         웹 서버를 내장하고 있는 전형적인 임베디드 제품에서는 이 서버를 관리하고 원격으로 접근
         할 수 있도록 해 주는 추가적인 서버 프로그램 역시 필요할 것이라고 예상할 수 있다. 이 예
         에서는 H下叩 서버와 텔넷（Telnet）을 (inetd를 이용해서） 사용 가능하도록 했다. ［리스트
         6-8］은 이 가상의 웹 서버 제품을 위한 간단한 rc. sysini七 스크립트를 보여 주고 있다．

         ［리스트 &8] 웹 서버용 rc.sysinit


             #!/bin/ sh

             echo "This is rc. sysinjt "

             busybox mount -t proc none /proc

             # Load the system loggers
             sysi ogd
             klogd

             # Enable legacy PTY support for telnetd
             busybox mkdir /dev/pts
             busybox mknod /dev/ ptmx c 52
             busybox mount -t devpts devpts /dev/pts




         이 간단한 초기화 스크립트에서는 먼저 proc 파일 시스템을 활성화시킨다. proc 서브시스
         템에 대해서는 9장에서 자세히 설명한다. 다음에는 동작 중에 시스템 정보를 확인할 수 있도
         록 하는 시스템 로거 (logger）를 활성화시킨다. 이 기능은 문제가 발생한 경우 특히 유용하게
         사용할 수 있다. 마치막 구문들은 UNIX I기［rl5) 서브시스템에 대한 지원을 활성화시키는
         것인데 , 텔넷 서버를 사용하는 데 필요한 것들이다．

        ［리스트 6-9］는 동작 레벨 2를 위한 시작 스크립트에 포함된 명령어를 보여 주고 있다. 이
         스크립트는 우리 시스템에서 동작시키고자 하는 서비스를 활성화시키는 명령어를 가치고
         있다．




15) （역자주） ply는 의사 터미널 유틸리티（Pseudo Terminal Utilities）를 뜻한다. 내부에 如rk () , 이祀ni卿（) , 하月wn ) 함수를 정
    의하고 있다．
                                              시스템 초가화   Chapter 6



   ［리스트 6-9] 동작 레벨 2의 시작 스크립트


      判 /bin/ sh

      echo "This is runlvl2. startup'

      echo "starting Internet superserver "
      inetd

      echo "starting web server "
      webs &




   동작 레벨 2의 시작 스크립트가 상당히 간단한 것을 알 수 있다. 먼저 일반적인 TCP/H) 요
   청을 낚아채고 요청에 따라서 필요한 서비스를 시작시키는 일을 하는 inetd, 이른바 인터넷
   슈퍼서버（superserver）라고 일컫는 서비스를 활성화시킨다. 이 예제에서 텔넷 서비스는
   /e七c/mni七ed. c아迂라는 설정 파일을 통해서 활성화시키도록 되어 있다. 마지막으로
   webs라는 이름의 웹 서버를 시작시킨다. 여기서는 이게 전부다. 최소한의 작업을 하고 있지
   만, 텔넷과 웹 서비스를 문제없이 동작시키는 스크립트이다．

   전체 구성을 마무리 짓기 위해서는 종료 스크립트도 만들어야 한다（［리스트 6-6] 참조）. 이
   시스템의 경우에는 시스템 종료 전에 웹 서버와 인터넷 슈퍼서버를 중단시키는 일을 해야 할
   것이고, 여기서는 이 작업만으로도 충분하다고 볼 수 있다．



6.4 초71 램디스크
   리눅스 커널은 시스템 부팅과 관련된 시스템 초기화 및 시스템 구성을 위해서 초기 루트 파일
   시스템을 마운트할 수 있는 메커니즘을 가지고 있다. 이 메커니즘을 초7I 램디스크伽hal RAM
   비sk) 또는 간단히 iriitrd라고 한다. 이 램디스크를 이용하기 위해서는 커널 컴파일 시에 이
   기능을 포함시켜야 한다. 이 기능에 대한 커널 구성 옵션은 구성 유틸리티 상에서 블록 디바
   이스 메뉴 아래에 있는 RAM 디스크 지원 항목에서 찾아볼 수 있다. ［그림 6-1］은 in孔rd를
   위한 구성 옵션의 예를 보여 주고 있다．
              Embedded Linux Primer




        F沁      Options     H욘］p

                  ［그 （쿄 回 巴 蔓                 鼠       曳．
         芦；
                   Load Say色 도呵目卵往 F目］i C에apse Expand

        Options                                   N카tie               N h可YVa沁E           스
        y小＝   卞rm兮t尸F昨夕忖m甘F斗7仰r1叫



        L} Mem마yTechn（靴芒ry Oes促ES 小｛TEl)
              p抽g and P啣 supp｛가t
        口 Bk玘kde너ccx
               口Norm쿄加口py d祐k support             BLX_DEV_FD          N 나 _ N
         卜 團比叩ba比d끈毗en叩附t                         BLK_DEV_LOOP        m 느 v y
               口N啣ork b幻ck device suppo民          BLK_DEV_NBD         N _ _ N
          口團RAM師k supp아t                          미．.KJIEV_RAM        -   -   V V
                  Defa너t number r寸 RAM d姓ks       BLK戶0EV尸RAM工：OUNT             16
                  DEEa뗘tRAM disks注e (kbyte돠       BLK나0巨V_RAM_SIZE              81蛇
                 團 In伯出 RAM dix丘；（娜岫 so미｝아I       BLK_DEVJNITRD       -       Y V
               姓Warn朽 source蜘（旬                   INITRAMFS_SOURCE
               口Pa比elwnti四 on CD刃VD med咀          CDROM PKTCDVD       N         N          .
        41                          1                                                 m
                                                                                      "



        Sony, rtohe如 usa姐너e 化따旴 야山on yet.                                                  良



                                                                                          口甘




        I 그림 6녀 리눅스 커널 구성 유틸리티



6.4. ] 초기 램디스크의 용도

        초기 램디스크는 부트 사이클이 완료되기 전에 지정한 디바이스 드라이버를 로드하도록 하는
        명령어를 담고 있는 작은 용량의 루트 파일 시스템이다. 레드햇이나 페도라 코어（Fedora
        Core）와 같은 리눅스 워크스테이션에서 램디스크는 실제 루트 파일 시스템을 마운트하기 전
        에 EXT3 파일 시스템을 위한 디바이스 드라이버를 로드한다. inj上rd는 실제 루트 파일
        시스템에 접근하기 위해서 필요한 디바이스 드라이버들을 로드하는 용도로 자주 이용된다．


6.4.2 in社rd로 부팅하키
        mni七rd 기능을 사용하기 위해서 , 대부분의 아키텍처가 mnm七rd 이미지를 커널에 전달하는
        데 부트로더가 관여하는 방식을 이용하고 있다. 일반적인 시나리오는 부트로더가 압축된 커
        널 이미지를 먼저 메모리에 로드하고, 그 후에 initrd 이미지를 메모리의 다른 공간에 로드
        하게 된다. 이 경우 커널로 제어권을 넘기기 전에 mni七rd 이미지가 로드된 주소를 커널에게
        넘기는 일을 부트로더가 책임져야 한다. 정확한 동작 방식은 아키텍처와 부트로더 그리고 플
        랫폼에 따라서 다를 수 있다. 하지만 중요한 것은 커널이 initrd 이미지를 로드하기 위해서
        반드시 그 위치를 알아야 한다는 것이다.


發 202
                                                       시스템 초기화   Chapter 6




일부 아키텍처와 플랫폼에서는 바이너리 이미지를 램디스크까지 포함시켜서 만들기도 한다．
이 방법은 부트로더가 mni七rd 이미지를 로드해 주는 별도의 리눅스 지원 기능을 가지고 있
지 않을 때 사용된다. 이 경우에는 커널과 램디스크 이미지가 그냥 합쳐진 형태를 가치고 있
다. 이런 형태의 복합 이미지를 만드는 부분에 대해서는 n追kefile의 boo七plmage 타깃을
참고하기 바란다. 현재 이 방법은 arm 아키텍처에서만 사용되고 있다．

그럼 이 경우에는 어떻게 커널이 initrd의 위치를 알 수 있을까2 부트로더가 initrd를
자동으로 알아 낼 수 있는 마법 같은 기능을 가지고 있지 않는한, 일반적으로 initrd의 시
작 주소와 크기를 커널 커맨드 라인을 통해서 커널로 전달한다. 다음 예제는 TI 아4AP
5912 프로세서를 사용하는 ARM 기반 보드에서 사용된 커널 커맨드 라인을 나타낸 것이다．



  console=ttySO, 115200 root=/ciev/nfs                       \
    nfsroot=192 .168. 1.9: /home/chris/sandbox/omap-target   \
    I ni trd=0x10800000 , 0x14af47



이 커널 커맨드 라인의 경우는 공간상 여러 줄에 걸쳐서 표시했다. 하지만 실제로는 스페이
스 문자로 구분된 한 줄짜리 문자열이다. 이 커널 커맨드 라인은 다음의 내용을 정의하고
있다．

  口 단일 콘솔로서 115kbps의 속도의 ttySO를 사용하도록 명시

  口 네트워크 파일 시스템, 즉 NFS를 통해서 루트 파일 시스템을 마운트시킴

  口 NFS 루트 파일 시스템을 192.168.1.9의 주소를 갖는 호스트어써 찾도록 명시（/home/
      chris /sandbox/omap-targe七 디렉터리에서）

  口 초기 램디스크 이미지를 물리 메모리 주소 呱10800000에서 0x14AF47(1, 355,591바이
      트） 크기만큼 로드하도록 함


한 가지 더 짚고 넘어갈 것이 있다. 거의 대부분의 경우 mni七rd는 압축되어 있고, 여가서
기술한 램디스크의 크기는 압축된 이미지의 크기를 나타내는 것이다．




                                                                       203
        Embedded Linux Primer




6.4.3 initrd릍 지원하는 부트로더

      ARM 프로세서에서 동작하는 인기 있는 부트로더인 t尸Bo毗를 예로 들어 보자. 이 부트로더
      는 리눅스 커널을 지원하도록 만들어진 부트로더이다. U-Bo毗를 이용하면 커널 이미지에
      mni七rd 이미지를 포함시키는 것이 아주 쉽다. ［리스트 6-10］은 초기 램디스크를 사용하도
      록 한 시스템의 전형적인 부팅 절차를 보여 주고 있다．

      ［리스트 6-10] 램디스크를 사용하는 커널 부팅


        # tftpboot Ox10000000 kernel -uiniage

        Load address: 0x10000000
        Loading: ############################ done
        Bytes transferred = 1069092 (105024 hex)

        # tftpboot 0x10800000 initrd- uboot

        Load address: 0x10800000
        Loading: ########################################### done
        Bytes transferred = 282575 (44fcf hex)

        # bootm Ox10000000 0x10800040
        uncompressing kernel                  done.

        RAMDISK driver initialized: 16 RAM disks of 16384K size 1024 blocksize

        RAMDISK: Compressed image found at block 0
        VFS: Mounted root (ext2 filesystem) .
        Greetings: this is linuxrc from Initial RAMDisk
        Mounting /proc filesystem

        BusyBox vl. 00 (2005.03.14-16: 37+0000) Built-in shell (ash)
        Enter 'help ' for a list of built- in commands.

        # (<<<< Busybox 명령 프롬프트）



      ［리스트 臼10］에서 다음 장에서 좀 더 자세히 설명할 U-Boot 부트로더가 동작하는 모습을
      볼 수 있는데 , 여기서 tftpbo（그七명령어는 U-Boot가 커널 이미지를 tftp 서버로부터 다운


204
                                                      시스템 초기화   Chapter 6



      로드하도록 하는 명령이다. 다운로드된 커널 이미지는 타깃 시스템 메모리상의 256MB 위
      치（16진수 값으로 0x10000000比））의 주소에 위치하게 된다. 두 번째 이미지는 초기 램디
      스크 이미지가 tftp 서버로부터 다운로드되어서 좀 더 상위 주소에 （이 예제에서는 256MB
      +8MB) 위치하도록 하고 있다. 마지막으로 U-Boot의 boo七m 명령을 실행시키는데 , 이 명
      령어는 "메모리에서 부팅하기" 명령이다. boo七m 명령어는 최대 두 깨의 인자를 받는데 , 첫
      번째 인자는 리눅스 커널 이미지의 주소를 넘겨주는 용도로 사용되고, 두 번째 인자는 선택
      적으로 사용되며 초기 램디스크 이미지의 위치를 가리키는 주소 값을 추가로 넘겨준다．

      U-Boot가 제공하는 기능 중에서도 특별히 중요한 기능이 하나 있다. 그것은 커널과 램디스
      크 이미지를 이더넷 연결을 통해서 로드할 수 있도록 해 준다는 점이다. 이 기능은 특히 개발
      단계에서 무척 유용하게 사용된다. 물론 커널과 램디스크 이미지를 보드에 올리기 위해서 다
      른 방법을 사용할 수도 있다. 하드웨어 장비로 되어 있는 플래시 프로그램 툴을 이용해서 플
      래시 메모리에 기록할 수도 있고, 시리얼 포트를 이용하거나 RS-232를 통해서 커널과 파일
      시스템 이미지를 다운로드할 수도 있다. 하지만 이미지가 보통은 상당히 큰 편이기 때문에
      （커널은 메가바이트, 램디스크는 수십 메가바이트가 될 수도 있다）, 이더넷 방식의 tftp 다운
      로드 방법을 이용하면 시간을 상당히 많이 절약할 수 있다. 어떤 부트로더를 선택하든 개발
      된 이미지를 네트워크를 통해서 다운로드할 수 있는 기능을 지원하는지를 확인하키 바란다．


6.4.4 i州打d의 마법 : Iinuxrc
      커널 부팅이 시작되면 커널은 initrd 이미지의 존재를 검사하고, 압축 바이너리 파일을
      RAM의 지정한 메모리 주소에서 커널의 램디스크로 복사해서 이 램디스크를 루트 파일 시스
      템으로 마완i시킨다. j-ni七rd의 마법은 initrd 이미지 안에 들어 있는 특별한 파일을 통
      해서 이루어진다. 즉, 커널은 초기 램디스크를 마운트시킨 후에 특수한 파일인 lLinuxrc 파
      일을 찾게 된다. 커널은 이 파일을 스크립트 파일로 간주하고 내부에 포함된 명령들을 실행
      시킨다. 이 메커니즘은 시스템 디자이너로 하여금 initrd7} 어떤 일을 할지를 결정할 수
      있도록 해 준다. ［리스트 &11］은 linuxrc 파일의 예제이다.




16) 물론 이 주소는 절대적인 것은 아니고 보드마다 다를 수 있다. 이 예제는 메모리 맵의 256v떠에서부E SDRAM이 시작하도록
    매핑되어 있는 것이다．
         Embedded Linux Primer




      ［리스트 6너 ] ] Iinuxrc 예제 파일


         判 /bin/ sh


         echo 'Greetings: this is 'linuxrc ' from Initial Ramdisk '
         echo 'Mounting /proc filesystem '
         mount -t proc /proc /proc

         busybox sh




      실제로 이 파일에는 진짜 루트 파일 시스템이 마운트되기 전에 실행시켜야 하는 명령어가 포
      함되어야 한다. 한 가치 예를 들면 루트 파일 시스템이 콤팩트플래시（CF) 장치에 있다면 콤
      팩트플래시 드라이버를 로드해야 할 것이다. 이 예제에서는 시험 삼아 단순히 busybox 쉘
      을 실행시켜서 부트 과정을 중단시키도록 하고 있다. 이 busybox 쉘이 실행된 결과 ［리스트
      6-10］의 # 명령 프롬프트를 볼 수 있는 것이다. 이 쉘에서 exit 명령을 입력하면 쉘이 종료
      되면서 중단되어 있던 부팅 과정을 계속 진행하게 된다．

      커널이 물리 메모리에 존재하는 램디스크 이미지를 실제 커널의 램디스크로 복사한 후에는，
      이 물리 메모리는 다시 가용 메모리 풀17) (po이）로 편입된다. 이 과정은 고정된 물리 메모리
      주소에 존재하던 initrd 이미지를 커널 자체의 （커널 램디스크 디바이스 형태를 갖는） 가
      상 메모리로 복사하는 과정이라고 생각할 수 있다．

      ［리스트 6-11］에 대해서 한 가지 더 짚고 넘어가자. /proc 파일 시스템을 마운트하는
      mount 커맨드에서 proc라는 딘어를 중복해서 사용하고 있다. 다음 명령어도 같은 기능을
      한다．

         mount -t proc none /proc


      moun七 명령어에서 장치 파일 이름을 입력하는 부분이 n아冶으로 바뀐 것을 알 수 있다．
      proc 파일 시스템에 대해서는 어떤 물리적인 장치도 연결된 것이 없기 때문에 moun七 명령
      은 이 장치 파일 이름은 무시한다. 그렇기 때문에 마음에 드는 아무런 값이나 입력해도 상관
      이 없다．


17) （역자주） 풀（pool) : 어떤 자원을 한꺼번에 모아두고 필요한 곳에서 조금씩 가져다 쓰는 구조를 말한다. 메모리 풀은, 큰 크기
    의 메모리를 유지하고 있r｝가 필요한 모듈들이 조금씩 할당해서 쓰丑 필요 없을 띠1 디시 반환하는 구조로 동작한다．
                                                        시스템 초기화     Chapter 6




6.4.5 initrd 구성
      리눅스 부팅 과정의 일부로서 , 커널은 반드시 하나의 루트 파일 시스템을 마운트시켜야 한
      다. 부팅 과정의 후반부에 prepare小namespace () 라는 함수에서 어디에 있는 어떤 파일
      시스템을 마운트할지를 결정하게 되어 있다. 만약 해당 커널이 ［그림 6-1)에서 설명한 것처
      럼 mni七rd를 지원하도록 설정되어 있고, 커널 커맨드 라인도 그에 맞게 설정했다면 커널은
      물리 메모리상의 압축된 initrd 이미지의 압축을 해제하고, 최종적으로는 램디스크 장치
      (/dev/ram）로 그 내용을 복사한다. 그리고 이 시점은 커널 램디스크에 적당한 파일 시스템
      을 하나 준비한 상태가 된다. 커널은 파일 시스템이 램디스크 안으로 모두 복사된 후에 램디
      스크 장치를 루트 파일 시스템으로 마운트시키게 된다. 그리고 마지막으로 mni七rd 이미지
      안에 만들어 놓은 파일인 linuxrc를 실행하기 위한 커널 쓰레드를 생성한다18) .

      linuxrc 스크립트의 실행이 끝나면 커널은 initrd를 언마운트시키고, 시스템 부팅의 마
      지막 단계로 계속 진행한다. 커널은 실제 루트 파일 시스템에 /initrd라는 디렉터리가 존
      재하는 경우에는 initrd 파일 시스템을 그 위치（이 경우에는 마운트 지점이라고 부른다）에
      마운트시킨다. 만약 최종 루트 파일 시스템에 /in'七rd라는 디렉터리가 없다면 initrd는
      폐기되고 더 이상 사용하지 않는다．

      만약 커널 커맨드 라인에 램디스크를 설정하는 root＝이라는 파라미터（예를 들어 , root=
       /dev/ramO）가 있으면 이전에 설명한 initrd의 동작에 두 가지 중요한 변화가 생긴다. 먼
      저 1inuxrc 스크립트를 실행하는 과정이 생략된다. 두 번째는 별도로 최종적인 루트 파일
      시스템을 마운트하지 않는다. 이 말은 시스템에서 mni七rd를 실제적인 루트 파일 시스템으
      로 사용하겠다는 의미이다. 이 방법은 오직 램디스크 상에 있는 루트 파일 시스템만을 이용
      하는 최소 사양의 시스템에 유용한 방법이다. 커널 커맨드 라인에 root=/dev/ramO를 넣
      어줌으로써 initrd를 최종적인 루트 파일 시스템으로 둔 채 전체 시스템 초기화 과정이 끝
      까지 진행된다．




18) 지면 괸계상 이 과정을 매우 단순화해서 설명했다. 실질적인 메커니즘은 개념샹으로는 비숫하지만, 몇 가지 세부 사황은 명확
    한 이해를 위해서 생귿휴크 것이다． 좀 더 자세히 알고자 한다면 커널 소스를 참고하기 H尾｝다. . . . /init/ main.c와
    . . . uinit/ do moun七S女 工를 참고하면 될 것이다．
   鞋    Embedded Linux Primer




6.4.6 initrd 이미지 만들기
       알맞은 루트 파일 시스템을 만드는 작업은 임베디드 시스템 개발과정 중에서 어려운 일에 속
       한다. 그 중에서도 적절한 initrd 이미지를 만드는 일은 일단 용량을 작게 만들어야 하고，
       특화된 설정을 해야 한다는 점에서 조금 더 어려운 작업이다. 이 절에서는 mnl七rd의 내용물
       과 inltrd를 만들 때 필요한 것들에 대해서 알아보자．

    ［리스트 6-12］는 이 장에서 쓰인 mni七rd 예제를 사용하는 시스템에서 七ree 명령을 실행시
       켜 출력된 결과를 나타낸 것이다．

    ［리스트 6-12] 예재 in出d의 내용



                     t너 n
                     I    busybox
                          -   -




                     I    echo -> busybox
                          -   -




                     1m
                          mount -> busybox
                              U




                     'mUsh -> busybox
                     dev
                     I-- console
                     I- - ramO
                     ' =H ttySO
         I   -   -
                     etc
         I   -   -
                     linuxrc
                     proc

         4 directories, 8 files



       보는 바와 같이 내용물이 정말로 간단하다. 압축하지 않은 상태에서도 500KB를 조금 넘는
       용량을 차지한다. 하지만 busybox어］ 기반하고 있기 때문에 많은 기능을 갖고 있다. 그리고
    bus ybox7} 정적으로 링크되어 있어서 다른 시스템 라이브러리에 의존성도 없는 상태이다．
    busybox는 11장에서 설명한다．
                                                              시스템 초기화      Chapter 6




6.5 initramf$ 사용하기
    mni七ramfs는 사용자 영역에서 초기에 수행되는 프로그램들을 위해서 비교적 최근（리눅스
    2.6）에 나온 기술이다. 이는 앞에서 설명한 initrd와 개념 및 그 용도가 비슷하다. 즉, 실
    저］ 루트 파일 시스템이 마운트되기 전에 필요한 디바이스 드라이버를 로드할 수 있도록 해
    준다. 하지만 mni七rd와 내부 동작 방식 측면에서는 확연히 다르다．

    initrd와 mnm七ramfs는 기술적인 구현 방법에서 큰 차이가 있다. 한 예로 initramfs는
    디바이스 드라이버가 로드되기 전에 드라이버 자체적으로 펌웨어가 필요한 경우 그 펌웨어를
    로드할 수 있도록 해 주는 함수인 do basic se七up () 을 호출하기 전에 로드된다. 더 자세
    한 설명은 리눅스 커널 문서에서 이 서브시스템에 대한 최신 문서를 참고하기 바란다. 위치
    는 . . ./Documentation/ fiiesystems/ramfs-rootfs-initramfs .txt이다.


    실용적인 관점에서 mni七ramfs는 initrd보다 사용이 훨씬 쉽다. initramfs는 cpio 형
    식의 파일이고, mnm七rd는 gz加으로 압축된 파일 시스템 이미지이다. 이 작은 차아점이
    mnm七ramfs를 더 사용하기 쉽게 만든다. 즉, initramfs7} 커널 소스 트리에 포함되어 있
    어서 커널 이미지를 빌드할 때마다 initramf s도 자동으로 생성된다. 그리고 기존 initrd
    이미지보다 수정하기도 무척 쉽다. ［리스트 6-13］은 리눅스 커널 소스 트리에서 . . . /usr
    디렉터리의 내용을 보여 주고 있는데 , 여기서 initramfs 이미지가 만들어진다. ［리스트
    6-13］의 내용은 커널을 빌드한 후의 디렉터리 내용을 나타낸 것이다．

    ［리스트 &13) initramfs가 만들어지는 디렉터리

       $ is -1
       total 56
       -rw- rw-r- -   1 chris chris 834 Mar 25 11: 13 built-in.o
       -rwxrwxr- x    1 chris chris 11512 Mar 25 11:13 gen_init.1cpio
        rw- rw-r- -   1 chris chris 10587 0ct 27 2005 gen_init_cpio. c
       -rw- rw-r- -   1 chris chris 512 Mar 25 11: 13 initramfs_data. cpio
       -rw- rw-r- -   1 chris chris 133 Mar 25 11: 13 initramfs_data. cp化. gz
       -rw- rw-r- -   1 chris chris 786 Mar 25 11: 13 initramfs_data. o
       -rw- rw-r--    1 chris chris 1024 oct 27 2005 initramfs_data. s
       -rw- rw-r--    1 chris chris 113 Mar 25 11:13 initramfs_list
       -rw- rw-r--    1 chris chris 1619 oct 27 2005 Kconfig
       -rw- rw-r- -   1 chris chris 2048 oct 27 2005 Makefile




                                                                                 209
   a.     Embedded Linux Primer



        여기서 in'七ramfs list 파일은 initramfs 이미지에 포함시킬 파일의 목록을 담고 있
        다. 최신 커널의 경우 다음과 같은 내용을 기본 값으로 가치고 있다．



          dir /dev 0755 0 0
          nod /dev/console 0600 0 0 c 5 1
          dir /root 070000



        이 내용을 토대로 최상위 디렉터리에 /roo七와 /dev 디렉터리를 가지고 있고 거기에 콘솔을
        나타내는 장치 파일（노드） 하나를 포함한 이미지가 만들어진다. in'七ramfs어］내용을 추가
        하려면 이 파일에 내용을 추가하면 된다. 또한 커널 구성 유틸리티를 통해서 in'七ramfs를
        만드는 데 참조할 디렉터리를 따로 설정할 수도 있다. 커널 구성 옵션에서 INITRAMFS
        SOURCE를 활성화시키고 해당 위치를 설정하면 커널 빌드 시스템이 그곳에 있는 파일들을
        이용해서 in'七ramfs 이미지를 만들게 된다．

        이 디렉터리에서 최종적으로 생성되는 결과물은 initramfs da七a cpio.gz 파일이다．
        이 압축된 이미지 안에는 (initramfs list 파일이나 INITRANFS SOURCE 옵션을 통해
        서） 우리가 기술한 파일들이 포함되어 있다. 이 파일은 최종 커널 이미지에 포함되어서 링크
        된다. 이 점도 initrd보다 mni七ramfs가 더 유리하다. 즉, 부팅 시점에 initrd의 경우처
        럼 별도의 이미지를 로드할 필요가 없기 때문이다．



6.6 총료
        임베디드 시스템을 개발할 때 올바른 종료（shutdown) 절차를 밟도록 구성하는 작업은 자주
        무시되곤 한다. 하지만 시스템을 부적절하게 종료하면 부팅 시간에 영향을 주는 것은 물론이
        고 일부 파일 시스템의 경우는 그 내용이 손상될 수도 있다. 특히 （수년 동안 데스크탑용 리
        눅스에서 기본 파일 시스템으로 사용된） EXT2 파일 시스템을 사용할 때 자주 나오는 불만
        사항 중의 하나가, 비정상적으로 전원이 종료된 후에 시스템을 부팅할 때 fsck（파일 시스템
        검사 유틸리티）가 수행되는 시간이 너무 오래 걸린다는 점이다. 대용량의 디스크를 장착한
        서버들은 fsck7} EXT2 파티션을 전부 검사하는 더］ 몇 시간이 걸릴 수도 있다．




I 210
                                                시스템 초기화   Chapter 6



        각각의 임베디드 시스템은 자신에게 맞는 종료 방법을 가치고 있어야 한다. 어떤 시스템에서
        잘 동작하던 방법이 다른 시스템에서는 기대대로 동작하지 않을 수 있기 때문이다. 종료하는
        방법은 전체 System V 종료 과정을 밟는 것이 될 수도 있고, 시스템을 중단하거나 재부팅하
        는 간단한 스크립트만으로 구성할 수도 있다. shu七down이나 halt, reboot와 같은 명령
        어는 종료 과정에서 사용할 만한 유틸리티들이다. 물론 이 유틸리티들이 자신의 시스템에서
        사용 가능한 경우에만 해당되는 이야기다.

        종료 스크립트는 기본적으로 모든 사용자 프로세스를 종료시켜야 하는데 , 이를 통해서 각각
        의 프로세스에서 사용하던 파일들이 닫히게19) 된다. 만약 mnit을 사용한다면 mnl七 0 명령
        을 입력하면 시스템이 종료된다. 일반적으로 종료의 세부 과정은 우선 모든 프로세스에
        SIGTEPM 시그널을 보내서 프로세스들에게 시스템이 종료되는 중이라는 것을 알린다. 그리
        고 약간의 지연 시간（d이ay）을 줌으로써 모든 프로세스가 각자 파일을 닫고, 상태를 저장하
        는 등의 마무리 절차를 진행할 수 있도록 한다. 그 후에 모든 프로세스로 SIGKILI』시그널을
        보내서 프로세스를 종료시킨다. 그리고 시스템에 마운트된 파일 시스템을 모두 언마운트
         (unm아mt）시킨 후에 , 아키텍처에 맞는 종료 또는 재부팅 명령을 내린다. 리눅스의 mnit
        명령어와 shutdown 명령어가 위 작업을 수행한다.



6.7요약
            口 모든 리눅스 시스템이 루트 파일 시스템을 필요로 한다. 각 어플리케이션마다 복잡한 의
               존성을 갖는 경우가 있기 때문에 파일 시스템을 만드는 일이 어려운 작업이 될 수도 있다．

            口 개발자는 파일 시스템 계층 표준을 이용해써 호환성과 유연성을 극대화할 수 있는 파일
               시스템 구조를 만들 수 있다．

            口 루트 파일 시스템이 어떻게 만들어지는지를 알아보기 위해써 최소 파일 시스템을 하나
               제시했다．
            口 리눅스 커널의 부팅 과정의 마지막 절차를 통해써 리눅스 시스템의 시작 동작을 정의하
               고 제어할 수 있다. 이를 위해서 자신의 임베디드 시스템의 목적어］ 맞는 몇 가지 메커니
               즘을 사용할 수 있다．




19) （역又阡） close ()
       Embedded Linux Primer



       口 m1lit 프로세스에 대해서 자세히 설명했다. 이 강력한 시스템 설정／제어 유틸리티는 자
          신의 임베디드 리눅스 시스템에서 기반 프로그램으로 사용될 수 있다. 본문에서는 예제
          시작 스크립트 환경과 함께 mni七을 이용한 시스템 초기화에 대해써 설명했다．

       口 초기 램디스크는 리눅스 커널이 최종적인 루트 파일 시스템을 마운트하고 mnit을 실행
          시키기 전에 사용자가 추가적으로 행동을 정의할 수 있도록 해 준다. 본문에서 그 메커
          니즘에 대해서 설명했고 이 강력한 기능을 사용하기 위해써 필요한 설정어］ 대해서 설명
          했다．

       口 initramfs는 초기 램디스크 메커니즘을 좀 더 간편하게 사용할 수 있도록 해1 준다．
          이 방법은 사용하기가 쉽고, 별도의 이미지를 로드할 필요가 없을 뿐만 아니라, 커널 빌
          드 시에 자동으로 같이 빌드되어 커널에 포함된다．



6.7. ] 더 읽어 보기
       파일 시스템 계층 표준（File System I五erarchy Standard)
       freestandards. org에서 관리
       www.pathname. com/fhs/


       부트 과정, Init4 Shutdown(Boot Process, mllit and Shutdown)
       리눅스 문서 프로젝트
       http :IItldp. org/LDP/intro-linux/html/sect 04H02. html


       m1lit에 대한 맨 페이지
       리눅스 문서 프로젝트
       http: //tldp. org/LDP/sag/html/init.html


       System V mllit에 대한 간략한 소개
       http://docs.kde.org/en/3. 3/kdeadmin/ksysv/what-is-sysv-init.html


       라눅스 부탕．" 그 역사와 마래叩 甲헤서
       Werner Almesberger
       www. almesberger.net/cv/papers/0152k-9. ps




1212
이번 징에서 배숄 내용

  U 부트로더의 역할

  U 부트로더의 도전 과제

  U 유니버설 부트로더 : Das U-Boot

  U 냐Boot 포팅하기

  U 기타 부트로더

  U 요약
 難U      Embedded Linux Primer




        앞 장에서 부트로더（bootloader）에 대해 잠깐 살펴본 적이 있다. 그리고 부트로더의 동작에
        대해서도 몇 가지 예를 통해서 이야기했다. 임베디드 시스템의 핵심 요소 중 하나라고 할 수
        있는 부트로더는 다른 시스템 소프트웨어를 실행시키기 위한 기반을 제공한다. 7장에서는 시
        스템에서 부트로더의 역할을 예제를 통해서 알아볼 것이다. 그 후에 부트로더가 가지는 공통
        적인 기능에 대해서 설명한다. 그리고 임베디드 시스템에서 가장 많이 사용되는 부트로더에
        대해서 알아보도록 하자. 마지막으로는 다른 부트로더를 소캐하고자 한다．

        현재 임베디드 시스템에서는 다앙한 부트로더가 사용되고 있다. 하지만 그 부트로더들에 대
        해서 모두 설명할 수는 없고 PowerPC. MIPS. ARM 등의 아키텍처를 사용하는 오픈 소스
        공동체에서 가장 많이 이용하는 부트로더를 선택해서 그 개념과 사용 예를 알아보도록 하자．
        바로 U-Boot 부트로더가 그 주인공이다．



7. ] 부트로더의 역할
        보드상에 전원이 처음 공급되면 아주 사소한 프로그램이라도 실행될 수 있도록 하기 위해서
        는 많은 하드웨어 요소들이 미리 초기화되어 있어야 한다. 아키텍처 및 프로세서는 각각에
        대해서 미리 정의된 초기화 과정을 가지고 있다. 그 과정에는 보드에 있는 저장 장치（보통은
        플래시 메모리）로부터 시작 단계의 초기화 코드를 가져오는 것도 포함된다. 이 시작 단계의
        초기화 코드는 부트로더의 일부로, 프로세서와 그와 관련된 하드웨어들에게 생명을 불어넣는
        역할을 하게 된다．

        대부분의 프로세서는 전원이 처음 공급되거나, 리셋이 된 후에 곧바로 실행될 코드를 어느
        주소에서 가져올지를 미리 정의해 두고 있다. 하드웨어 디자이너는 이 정보를 이용해서 보드
        의 플래시 메모리를 구성하고, 어느 주소 영역에 플래시 메모리를 매핑할 것인지를 결정하게
        된다. 이렇게 전원이 처음 공급되면 코드가 미리 정의된 번지로부터 실행되고, 그 주소에 있
        는 소프트웨어 코드가 제어권을 갖고 실행될 수 있는 것이다．

        부트로더가 하는 일이 바로 이 시작 단계의 초기화 코드를 제공하고, 다른 프로그램들이 실
        행될 수 있도록 보드를 초기화하는 작업이다. 여기서 시작 단계의 초기화 코드는 거의 항상
        해당 프로세서에 맞는 어셈블리 언어로 작성되어 있다. 사실 어셈블리 언어로 작성되어 있다
        는 점 때문에 많은 어려움을 겪게 되는데 , 여기서 그 일부를 설명할 것이다．



I 214
                                                       부트로더   Chapter 7



      부트로더가 실행되어서 프로세서와 플랫폼에 맞는 기본적인 초기화를 진행한 후에 부트로더
      에게 남은 가장 중요한 역할은 실제적인 운영체제（0s）를 부팅시키는 일이다. 이는 Os를 메
      모리의 알맞은 위치에 로드시키고, 제어권을 Os로 넘겨주는 일을 말한다. 그 외에도 부트로
      더는 추가적인 기능을 가질 수 있는데 , 예를 들면 Os 이미지가 올바른지를 검사하는 기능이
      나, 부트로더 자신 또는 Os 이미지를 업그레이드할 수 있도록 해 주는 기능 그리고 개발자가
      정의한 정책에 따라서 여러 Os 이미지 중에서 하나를 결정하는 기능 등을 가질 수도 있다.
      기존의 PC 환경의 BIOS와는 달리 이 부트로더들은 제어권이 운영체제로 넘어간 후에는 그
      코드와 데이터 메모리를 더 이상 사용하지 않고1) , 다른 용도를 위해서 그 공간을 해제하게




7.2 부트로더의 도전 과제
      C로 작성된 아주 간단한 "Hello World" 프로그램을 실행시키기 위해서도 많은 하드웨어，
      소프트웨어 자원이 필요하다. 어플리케이션 개발자는 이런 세부 사항까지 신경 쓰지 않아도
      되는데 , 이는 C 런타임 라이브러리들이 투명하게 동작 환경을 제공해 주기 때문이다. 하지만
      부트로더 개발자는 그런 사치를 누릴 수 없다. 부트로더는 자신이 필요로 하는 모든 자원들
      에 대해서 그 자원을 사용하기 전에 미리 세심하게 초기화하고 할당하1 주어야 한다. 그 중에
      서 가장 눈에 띄는 예는 동적 임의 접근 메모리 (Dynamic Random Access Memory) , 즉
      DRAM이다．


7.2. ] DRAM 컨트롤러
      DRAM 칩은 마이크로프로세서의 다른 버스의 자원들처럼 직접 읽고 쓸 수 없다. 그래서
      읽기 , 쓰기 동작을 가능하게 해 주는 하드웨어 컨트롤러를 필요로 한다. 읽고 쓰는 문제 외
      에도 더 복잡한 점은 DRAM의 특성상 지속적으로 내부의 데이터를 갱신（refresh）해 주지
      않으면 그 데이터가 사라진다는 것이다. 갱신 작업은 DRAM 생산 업체가 지정한 시간 조건
      내에 규칙적으로 DR사d의 각 위치를 순서대로 읽어내는 방식으로 이루어진다. 그리고 최
      근 DRAM은 고성능의 제품을 위해서 버스트 모드나 DDR(Dual Data Rate) 모드를 지
      원한다. DR帥/1을 사용할 수 있도록 설정하고, 생산 업체에서 명시한 시간 조건에 맞게 데

l) 일부 임베디드 시스템에서는 부트로더를 제거하지 않고 코드의 일부를 콜백 함수 형식으로 재사용한다. 하지만 이 접근 벋뼙은
   그리 유용한 방식은 아니다. 리눅스는 부트로더보다 더 많은 기능을 가지고 있기 때문에 보통 부트로더에게까지 힘을 빌릴 필요
 는 거의 없기 때문이다．


                                                                   2佰 且
         Embedded Linux Primer




        이터를 계속 갱신하는 일 그리고 읽기 및 쓰기 요청 명령을 처리하는 일이 DR사vi 컨트롤러
        의 몫이다．

        DRAM 컨트롤러를 설정하는 일은 임베디드 개발을 처음 접하는 개발자에게는 좌절감을 안
        겨줄 정도로 어렵게 느껴지는 작업이다. 이를 위해서는 DRAM 아키텍처에 대해서 자세한
        지식을 가지고 있어야 하는 것은 물론이고, 컨트롤러 자체와 사용할 특정 DRAM 칩 그리고
        전체 하드웨어 디자인에 대해서도 어느 정도 이해하고 있어야 하기 때문이다. 자세한 내용은
        이 책의 범위를 벗어나지만, 관심 있는 독자는 이 장 마치막 부분의 참고 자료를 통해서 좀
        더 자세히 알아보기 바란다. 그리고 부록 D, "SDRAM 인터페이스 고려 사항'에서도 이 중요
        한 주제에 대한 기본 지식을 얻을 수 있을 것이다．

        DRAM 컨트롤러와 DRAM 자체가 알맞게 초기화되기 전까지는 임베디드 시스템에서 할 수
        있는 일은 거의 없다고 할 수 있다. 부트로더가 가장 먼저 해야 할 일 중의 하나가 바로 메모
        리 서브시스템을 활성화시키는 것이다. 초기화 후에는 메모리를 하나의 자원으로 이용할 수
        있다. 사실 많은 부트로더들이 메모리 초기화 후에 가장 먼저 하는 일이 좀 더 빨리2) 실행시
        키기 위해서 자기 자신을 DRAM에 복사하는 일이다．


7.2.2 플래시와 RAM
        부트로더가 태생적으로 가지고 있는 또 다른 복잡한 사항은 부트로더 자신이 비휘발성 저장
        장치에 저장되어야 하며 , 실행을 위해서는 보통 RAM에 로드된다는 점이다. 다시 말하면 부
        트로더가 의지할 수 있는 자원이 한정되어 있다는 점 때문에 복잡해지는 것이다. 리눅스와
        같은 운영체제를 실행시켜서 정상적으로 기능을 하고 있는 컴퓨터 시스템의 경우에는 프로그
        램을 컴파일하고, 이 프로그램을 비휘발성 메모리에서 실행시키는 것이 상대적으로 쉽다고
        할 수 있다. 런 타임 라이브러리 (rui亡恤ie library）와 운영체제 자신 그리고 컴파일러가
        협동해서 프로그램을 비휘발성 메모리에서 읽어 들여서 제어권을 넘기고 실행할 수 있는 기
        반을 만들어 주기 때문이다. 앞에서 말한 "Hello World"가 완벽한 예다. 즉, 컴파일하고 나
        면 단순히 명령에 프롬프트에서 실행 파일의 이름（hello）을 입력하기만 하면 （물론 실행
        파일이 PATH어］ 포함되어 있는 경로에 있어야 한다） 메모리에 로드해서 실행시킬 수 있다.



2) （역자주） 비휘발성 플래시 메모리는 DRAM보다 느린 장치이기 때문어］, 코드의 빠른 실행을 위해서 자신을 DRAM에 복사해서
   DRAM에서 실행되도록 하는 것0] 일빈적이다．


I 216
                                                                  부트로더   Chapter 7




    전원이 인가된 후의 부트로더에게는 이런 기반 구조라는 게 존재하지 않는다. 대신에 부트로
    더 스入쿠7} 자신이 실행하기 위한 컨텍스트를 만들고 필요한 경우 RAM의 특정 위치에 자
    신을 스스로 복사한다. 그리고 읽기 전용 매체에서 실행시켜야 할 경우에도 추가적인 문제점
    들을 해결해야 한다．


7 ,2,3 이미지 복잡도
    어플리케이션 개발자로서 플랫폼 상에서 실행시킬 어플리케이션을 개발하기 위해서 바이너
    리 실행 파일의 내부 배치까지 고려할 필요는 없다. 컴파일러 및 바이너리 유틸리티들이 이
    미 정의되어 있어서 , 해당 아키텍처에 필요한 요소들을 바이너리에 포함시켜서 빌드해 준다．
    링커는 이미지에 시작（프롤로그）과 종료（에필로그） 코드를 넣어 주는데 , 이 오브젝트들은 보
    통 main () 함수에서 시작하는 어플리케이션을 실행시키기 위한 문맥을 알맞게 초기화하는
    일을 한다．

    하치만 부트로더에서는 입장이 다르다. 부트로더가 실행되면 거기에는 알맞은 문맥
    (context）도 없고 이미 만들어진 실행 환경 같은 것도 존재하지 않는다. 보통의 경우 부트로
    더가 프로세서와 기타 관련 하드웨어를 초기화하기 전까지는 DRAM도 사용하지 못한다. 이
    게 의미하는 것을 한번 생각해 보자. 일반 C 함수의 경우 인자와 지역 변수는 스택에 저장된
    다. 그래서 초기에는 ［리스트 7-1］의 간단한 함수도 사용할 수 없는 것이다．

    ［리스트 7-1 ] 간단한 C 함수


       mnt setup_memory_contro11er (board_ nfo_t *p)
          {
          unsigned int 노Jram_controller_ register = p->dc_ reg;




    전원이 들어와서 부트로더가 제어권을 갖게 되는 시점에 스택과 스택 포인터는 아직 존재하
    지 않는다. 그래서 ［리스트 7-1］에 있는 간단한 C 프로그램을 실행시키려고 하면 문제가 발
    생하는데 , 컴파일러가 아직 존재하지도 않는 스택 내에서 dram controller register
    라는 변수를 초기화하는 코드를 만들어 내기 때문이다. 그래서 부트로더는 C 함수를 호출하
    기 전에 실행 컨텍스트를 만드는 일을 먼저 해야 한다．




                                                                              2口
 難 毋1     Embedded Linux Primer




        부트로더를 컴파일하고 링크할 때 개발차는 이미지가 어떻게 구성되고 링크되는지를 완전히
        제어할 수 있어야 한다. 특히 부트로더 入入쿠7} 플래시 메모리에서 RAM으로 자기 자신을
        복사해야 할 경우에는 더욱더 그렇다. 이를 위해서 컴파일러와 링커에 이런 특징들과 최종
        이미지의 배치를 정의하는 파라미터를 전달해야 한다. 하지만 최종 바이너리 이미지를 만드
        는 데는 크게 두 가지의 어려운 고비가 있다．

        첫 번째는 프로세서의 부팅 절차와 호환되는 형식으로 시작 코드를 구성해야 한다는 점이다．
        실행 코드의 맨 앞 시작 부분은 반드시 플래시 메모리의 미리 악속한 위치에 존재해야 한다．
        물론 이 위치는 프로세서와 하드웨어 아키텍처에 따라서 다를 수 있다. 예를 들어 , AMCC
        PowerPC 405GP 프로세서는 고정된 메모리 주소 OxFFFF FFFC에서 첫 번째 기계어 명
        령어3）를 가져오도록 되어 있다. 다른 프로세서들도 세부 내용은 다르지만 비슷한 방식을 이
        용한다. 일부 프로세서의 경우는 전원이 인가된 후 외부 하드웨어 시그널을 검사해서 그 값
        을 통해서 미리 정의된 여러 위치 중의 한 곳4）을 결정하기도 한다．

        그렇다면 개발자는 바이너리 이미지의 배치를 어떻게 지정할 수 있을까？ 링커는 링커 기술
        파일 또는 링커 명령에 스크립트라고 부르는 파일을 넘겨받을 수 있도록 되어 있다. 이 특수한
        파일은 바이너리 실행 파일에 대한 처방전（rec如이쯤으로 생각할 수 있다. ［리스트 7-기는 잠
        시 후 설명할 유명한 부트로더에서 실제로 사용되는 링커 기술 파일의 일부를 나타낸 것이다．

        ［리스트 二2] 링커 명령에 스크립트           리셋 벡터


           SECTIONS
           {
               . resetvec OXFFFFFFFC
               {
                   *( . resetvec)
               } = Oxffff




3) （역자주） machine instruction : 프로세서가 제공하는 기계어 코드를 말흐K+. 어셈블러의 각 명렵과 ': 1 관계를 갖는다．
4) （역자주） 한 가지 예로， 점퍼나 스위치를 통해서 부팅할 위치를 결정할 수 있도록 되어 있는 프로세서들이 있다. 개발 및 테스
   트를 위해서 여러 가지 부팅 경로를 만들어 두는 것이다. 예를 들어, 항상 RUM 부팅만 하도록 된 시스템보다는 외부 핀에 따라
  서 N아之 부팅도 선택적으로 할 수 있다면 좀 더 유용할 것이다．


12仍
                                                                     부트로더   Chapter 7




      링커 명령에 스크립트 문법에 대한 자세한 설명은 이 책의 범위를 벗어난다. 관심 있는 독자
      는 이 장의 마지막에도 참고 자료로 나오는 GNU LD에 대한 매뉴얼을 참고하기 바란다．
      ［리스트 7-2］는 바이너리 ELF 이미지로 만들어질 섹션들을 정의하는 시작 부분이다. 위 내
      용은 링커로 하여금 .rese七vec라는 이름의 섹션을 OxFFFI亡FFFC로 시작되는 주소에
      위치시키도록 정의하는 일을 한다. 또한 섹션의 나머지 공간을 모두 비트 1, 즉 0xFFFF
      값으로 채우도록 설정하고 있다. 이렇게 한 것은 플래시 메모리를 삭제하면 그 비트 값이 모
      두 1인 것과 관계가 있다. 이 방법을 통해서 플래시 메모리 소모를 줄이는 것은 물론이고，
      해당 섹터를 프로그래밍하는 시간도 줄일 수 있는 것이다．

      ［리스트 7-3］의 내용은 최신 口Boot 배포판에서 .resetvec 섹션을 정의하는 어셈블리
      언어로 작성된 파일의 내용을 모두 나타낸 것이다. 이 내용은 . . ' /cpu/ppc4xx/
      resetvec. S 어셈블리 파일에 저장되어 있다. 이 코드 섹션의 크기는 32비트 머신에서는
      4바이트를 넘을 수 없다는 점을 주의하자. 이 섹션에는 설정 옵션과 무관하게 오직 한 개의
      명령어만 정의하고 있기 때문이다．

      ［리스트 7-3] .resetvec를 정의하는 소스 코드


          /* copyright MontaVista Software Incorporated, 2000 */
          #include <config. h>
                 . section .resetvec, "ax "
          #if defined (C0NFIG440)
                 b _start440
          #el se
          #汗 defined (CONFIGHBOOT_PCI) && deflned (CoNFIG.jiIp405)
                 b .startpci
          #else
                 b estart
          #endif
          #endif




      이 어셈블리 언어로 작성된 파일은 어셈블리 언어 프로그래밍 경험이 없더라도 이해하기 쉬
      운 내용으로 되어 있다. 즉, 지정한 설정에 따라서 (CONFIG 士 매크로들을 통해서 정의된
      대로） 메인 코드 본체의 시작 위치로 이동하는 무조건 분기5) 명령에 하나를 만들어 낸다．

5) ［역자주） 조건에 따라서 분기（Jump. Branch）하는 명령을 조건 분기, 무조건 분기햐는 명령을 무조건 분기라고 한다. 예를 들어，
   ARM 명령의 JNE는 이전 비교문의 결과에 따라서 분기를 결정하는 반면 JMP, C皿J』등은 무조건 해당 위치로 분기하는 무조건


                                                                                  2四
          Embedded Linux Primer




        이 분기문은 4바이트로 이루어진 PowerPC 명령어인데 , ［리스트 7-2］의 링커 명령에 스크
        립트에서 본 것과 같이 , 결과로 만들어지는 이미지에서 플래시의 절대 주소 0xFFFF
        FFFC에 위치하게 된다. 앞에서 말한 것처럼 , PPC 405GP 프로세서는 미리 결정된 주소에
        서 첫 번째 명령어를 가져오도록 되어 있다. 이와 같은 방법을 통해서 지정한 아키텍처 및
        프로세서에 따라서 최초 실행될 코드를 직접 지정할 수 있게 된다．


7.2.4 실행 컨텍스트
        부트로더 이미지를 만드는 것이 복잡한 두 번째 이유는, 실행 컨텍스트6）가 부족하다는 점이
        다. ［리스트 7-3］에 있는 명령이 처음 수행되는 시점（이 명령에 천원이 인가된 후 처음 실행
        되는 명령이라는 것을 상기하자）에서는 프로그램을 실행시키키 위해서 사용할 수 있는 자원
        이 거의 없다. 하드웨어는 플래시 메모리로부터 명령어를 올바로 가져오는 것과 시스템 클럭
        이 기본 값7）을 가지고 있는 것을 보장하는 것 외에 다른 사항은 거의 지정된 것이 없다8) .
        프로세서의 리셋 상태는 프로세서 생산 업체에 의해서 잘 정의되어 있지만, 보드의 리셋 상
        태는 하드웨어 디자이너에 의해서 정의된다．

        말할 것도 없이 대부분의 프로세서가 처음 시작할 시점에는 C 언어로 작성된 코드를 사용하
        기 위해서 필요한 변수나 스택을 위한 DRAM 공간을 사용할 수 없는 경우가 대부분이다．
        횬히 가장 간단한 예제로 사용하는 "Hello World" 프로그램조차도 DRAM이 없는 상태 , 결
        국 스택이 없는 상태에서 구동시켜야 하는 경우라면 아주 어려운 예제로 돌변한다．

        이 제약 사항 때문에 하드웨어를 초기화하도록 되어 있는 시작 코드를 작성하기가 무척 어려
        워진다. 이 때문에 , 부트로더가 맨 처음 하는 일 중의 하나가 최소한이라도 RAM의 일부를
        사용할 수 있도록 하드웨어를 초기화하는 것이다. 임베디드 시스템을 위해서 디자인된 일부
        프로세서의 경우는 칩에 가용한 작은 용량의 RAM을 내장하고 있는 경우도 있다. 지금 예제
        로 사용하고 있는 PPC 405GP도 이 경우에 해당한다. RAM이 사용 가능할 경우 그 일부를
        스택으로 할딩해서 사용할 수 있어서 C 언어와 같은 고급 언어를 실행할 수 있는 기본 컨텍


  분기 명령이다．
6) ［역자주） Conte玭, 즉 문맥이라 함은 코드가 실행되기 위한 기본 조건 또는 환경을 말한다. 스택이나 힙 등의 기본 조건들을 갖
   추어야 코드가 올바로 수행될 수 있다．
7) ［역자주］ 보통의 Soc 프로세서는 내부에 PLL을 가지고 있으며, 적당한 기본 값을 가지고 있어서 알맞은 시스템 李큭 값을 갖도
   록 설계된 경우가 대부분이다．
8) 이 부분은 아키텍처, 프로세서 그리고 하드웨어 디자인의 세부 사항에 比冊서 다를 수 있다．


I 220
                                                                     부트로더     Chapter 7



       스트를 갖출 수 있게 된다. 그래서 프로세서 및 플랫폼을 초기화하는 코드로 어셈블러가 아
       닌 다른 언어를 사용할 수 있게 된다．



7.3 유니버설 부트로더 : Da$ 小Boot
       부트로더는 상용 부트로더에서부터 오픈 소스 부트로더까지 매우 다앙하다. 그리고 직접 7가
       발해서 독자적으로 사용되고 있는 부트로더도 매우 많다. 이들 대부분이 어느 정도 공통된
       기능을 갖고 있다고 볼 수 있는데 , 예를 들어 모두 다른 프로그램 , 그 중에서도 특히 운영체
       제（0s）를 로드하고 실행시키는 기능을 들 수 있다. 그리고 대부분이 시리얼 포트를 통해서
       사용자와 통신한다. （이더넷과 같이） 네트워크 서브시스템을 지원하는 경우는 훨씬 덜 일반
       적이지만 아주 강력한 기능이다．

       많은 부트로더가 특정한 아키텍처에서만 동작하도록 작성되어 있다. 하지만 큰 깨발 조직의
       경우에는 다양하고 넓은 범위의 아키텍처 및 프로세서를 지원하는 능력을 갖추는 부트로더를
       확보하는 것이 아주 중요한 요소일 수 있다. 작은 개발 조직의 경우에도 하나 이상의 아키텍
       처에 여러 다양한 프로세서를 이용하는 경우가 흔하키 때문이다. 그래서 하나의 부트로더를
       여러 플랫폼에서 모두 사용할 수 있도록 개발 및 투자하는 것이 최종적으로는 비용을 절감하
       는 방법이다．

       이 절에서는 임베디드 리눅스 커뮤니티에서 아주 많이 사용되는 부트로더에 대해서 설명할 것
       이다. 이 부트로더의 공식적인 이름은 다스 유 부트（Das9) U-Boot）이다. 이 부트로더는 볼프
       강 뎅크（M厄lfgang Denk）에 의해서 관리되며 소스포지의 http:1/u-boot.sourceforge . net
       에 홈페이지10)7} 있다. U-Boot는 다양한 아키텍처를 지원하고, 자신들의 프로젝트에
       U-Boot를 적용하고 그것을 공유해 주는 많은 임베디드 개발자 및 하드웨어 제조 업체의 지
       원을 받고 있다．


7.3. ] 시스템 구성 : U-Boot
       부트로더가 여러 프로세서와 아키텍처에서 사용되기 위해서는 부트로더를 구성하기 위한 방
       법이 필요하다. 리눅스 커널 자체도 그렇듯이 부트로더의 구성도 컴파일 시점에 이루어진다．


9) ［역자주） Das는 독일어인데, 영어로는 the, 出at 정도의 의미이다．
10) ［역쟈주그 현재는 Sourceforge 내의 사이트는 사용되지 않고 정식 홈페이지인 胤加：/1w＼們v. denx. de／恤d/UBoot를 사용하고 있다．


                                                                                    221 1
 難 仄U      Embedded Linux Primer




        이렇게 컴파일 시점에 구성하기 때문에 부트로더의 복잡성을 상당히 줄일 수 있을 뿐만 아니
        라, 그 자체로도 중요한 특징이 된다．

        U-Boot의 경우 보드 관련된 구성 작업은 해당 타깃 플랫폼을 위한 단일 헤더 파일과 타깃
        보드, 아키텍처 , CPU에 따른 하위 디렉터리를 가리키는 일부 소프트 링크들을 이용해서 결
        정하게 된다. U-Boot가 지원하는 플랫폼 중에서 하나를 선택해서 구성하고자 할 때는 다음
        과 같은 명령어를 이용한다．

           $ make <platform>_config


        여기서 platform은U-Boot가 지원하는 많은 플랫폼 중의 하나를 선택하면 된다. 이 플랫
        폼 구성 타깃의 전체 목 록 은 U-Boot 소스 코드의 최상위 II追keflie에서 볼 수 있다. 예를
        들어 , TI OMAP 5912 프로세서에 기반을 둔 스펙트럼 디지털의 0SK 플랫폼ll）의 경우에
        는 다음과 같은 명령어를 입력하면 된다．

           $ make omap5912osk_config


        이 명령은 U-Boot 소스 트리를 대상 아키텍처로 ARM(ARM926）을 선택하고, 코어와 타
        깃 플랫폼으로 5912 0SK로 연결되도록 소프트 링크들을 바꿔 주는 일을 한다．

        이 플랫폼을 위해서 U-Boot를 구성하는 다음 단계는 보드를 위한 구성 파일을 수정하는 것
        이다. 이 파일의 위치는 U-Boot 소스 트리 내에서 . . . /include/configs/ 디렉터리에
        있는 omap5912osk.h 파일이다. U-Boot 배포판에 포함되어 있는 README 파일에서 구
        성에 대한 자세한 설명을 볼 수 있고, 이 정보를 위해서 참고할 만한 가장 좋은 문서이다．

        U-Boot의 구성은 보드를 위한 헤더 파일에 정의된 구성 값들을 이용해서 이루어진다. 구성
        값은 크게 두 가치 종류로 나눌 수 있다. 구성 옵션은 CONE'끄; xxx와 같은 형식의 매크로를
        이용해서 선택하고, 구성 설정을 위해서는 C丑; xxx와 같은 형식의 매크로를 이용한다. 그
        중에서도 일반적으로 구성 옵션（CONFIG多xx）이 사용자가 변경할 수 있는 내용이고, 또한
        이 옵션들을 이용해서 U-Boot의 기능을 활성화시킬 수 있다. 구성 설정（C코3XXX）은 보통
        하드웨어를 위해서 사용되고, 값을 변경하기 위해서는 기반 프로세서와 하드웨어 플랫폼에
        대한 세부적인 지식이 필요하다 보드에 맞는 口Boot 설정은 그 하드웨어 플랫폼에 맞는
        구성 옵션과 구성 세팅 값들을 가지고 있는 전용 해더 파일을 변경하는 방식으로 진행된다．

11) （역쟈주） 이 플랫폼어］ 대해서는 http/佃ww. Sp的rum旽i怡1. Co可prod岫1可0. php?produC始id=39를 참고하자．



I 222
                                                              부트로더     Chapter 7




口Boot 소스 트리에는 보드에 따른 구성을 저장하고 있는 헤더 파일들을 따로 모아둔 디렉
터리를 가지고 있는데 U-Boot 소스 최상위 디렉터리 . . . /include/configs 위치에서
이 디렉터리를 찾을 수 있다．

이 보드 구성 헤더 파일에 새로운 정의를 추가함으로써 여러 기능 및 동작 모드를 선택하고
변경할 수 있게 된다. ［리스트 7-4］는 PPC 405GP를 사용하는 가상의 보드를 위한 구성
헤더 파일의 일부 내용을 나타낸 것이다．

［리스트 二4] U-Boot 보드m구성 헤더 파일의 일부


  #define CONFIG_405GP         /""" Processor definition ' /
  #define CONFIG_4XX          7노 sub-arch specification, 4xx family */

  #define CONFIG_SYS_CLK_FREQ 33333333 /'" PLL Frequency 士7
  #define CONFIG_BAUDRATE      9600
  #define CONFIG_PCI        /* Enable support for PCI ' /

  #define CONFIG_COMMANDS       (CONFIG_CMD_DFL I CFG_CMD_DHCP)

  #define CFG_BASE_BAUD         691200

  /'" The following table includes the supported baudrates 六 /
  #define CFG_BAUDRATE_TABLE \
       {1200, 2400, 4800, 9600, 19200, 38400, 57600, 115200, 230400}

  #define CFG_LOAD_ADDR         0x100000      7노 default load address */

  /""' Memory Bank 0 (Flash Bank 0) initialization 六 /
  #define CFG_EBC_PBOAP          0x9B015480
  #define CFG_EBC_PBOCR          OxFFF18000

  #define CFG_EBC_PB1AP          0x02815480
  #define CFG_EBC_PB1CR          0xF0018000




［리스트 7-4］를 통해 주어진 보드를 위해서 U-Boot를 어떻게 구성할치에 대한 아이디어를
얻을 수 있다. 실제 보드e구성 파일의 경우에는 위에서 보는 것과 같은 내용을 수백 줄 이상
가질 수도 있다. 위 예제에서는 CPU 정의 , CPU 계열에 대한 정의 , PLL 클럭 주파수 값，


                                                                            223 1
 照 斗二       Embedded Linux Primer




         시리얼 포트의 속도, PCI 지원 등에 대한 정의를 볼 수 있다. 예제에는 구성 옵션 값
         (coNFIG--xxx) 일부와 구성 설정 값(cFG xxx) 일부를 포함하고 있다. 마치막 부분은 메모
         리 뱅크 0, 1을 사용하기 위해서 외부 버스 컨트롤러를 초기화하는 데 사용되는 하드웨어
         레지스터 값이다. 보는 것처럼 어떻게 도무지 이해할 수 없는 이 값들은 보드 및 프로세서에
         대한 세부 지식이 있어야만12) 사용할 수 있다．

         이와 같은 정의 구문을 이용해서 U-Boot의 다양한 부분을 구성할 수있는데, U-Boot어］ 어
         떤 기능을포함시킬지（예를들어 , DHCP를사용할지 , 메모리 테스트기능을사용할지 , 디버
         깅을 지원할지 등）를 결정하는 것도 가능하다. 그리고 이 방법으로 보드에 어떤 종류의 메모
        리가 장착되어 있는지 , 그 용량은 얼마나 되며 , 주소 공간의 어디에 매핑되어 있는지를
         U-Boot에게 알려 줄 수 있다. 관심 있는 독자는 U-Boot 코드13）를 한 번 조사해 보거나，
         U-Boot 코드 내에 포함된 아주 훌륭한 README 문서를 한번 살펴보기 바란다．


7.3.2 U-Boot 명령0] 셋
        口Boot는 60개 이상의 명령에 셋（집합）에 약 150개에 달하는 명령어를 가지고 있다. 지정
         한 명령에 셋은 U-Boot에서 구성 옵션（CFG 火）을 이용해서 활성화시키거나 비활성화시킬
         수 있다. 최신 U-Boot에서 사용할 수 있는 명령에 셋에 대한 전체 리스트는 부록 B
         "U-Boot의 구성 가능 명령에 셋"을 참고하자. 다음은 그 중에서 일부를 나타낸 것이다．

          명령에 셋                     명령어

          CFG （갔町D ELASH            플래시 메모리 관련 명령어

          CFG CMD MEMORY            메모己를 덤프하고, 특정한 내용으로 채우고， 복사, 비교하는 등의 명령어

          CFG CND DHCP              DHCP 지원

          CFG CMD PING              Ping 지원

          CFG CMD EXT2              EXT2 파일 시스템 지원




12) （역자주） 결국 프로세서 및 보드 사용자 매뉴얼을 참고해야 얻을 수 있는 값이다．
13) ［역자주） 口Boot 홈폐이지에서 http://www. denx. de/cgi-bin/gitweb. cgi?p＝寸boot. git;a=summary어］ 가면 인터넷 상에서도 소스
   를 열어 볼 수 있다．
                                                                  부트로더     Chapter 7


        ［리스트 7-4］에 있는 다음 내용은 지정한 보드를 위한 U-Boot에서 사용할 명령에 셋을 설
        정하는 부분이다．

           #define C0NFIG_C0MMANDS       (C0NFIG_CMD_DFL I CFG_CMD_DHCP)


        보드 구성 헤더 파일에 각각의 CFG 士 매크로를 직접 입력해서 사용할 명령에 셋을 정의하는
        방법도 있지만, U-Boot가 미리 정의해 놓은 기본 명령 집합을 기반으로 할 수도 있다. 바로
        CONFIG CMD DEl』이 기본적으로 활성화시킬 명령에 셋을 정의하고 있는 매크로이다．
        CONFIG CMDHDEL은 기본 값으로 tftpboot (t代p 서버로부터 이미지를 받아서 부팅하기）,
        bootm（메모리에서 부팅하기）, md（메모리 내용 보기）와 같은 메모리 유틸리티 등을 활성화
        시킨다. 여기에 추가적으로 다른 명령어들을 활성화시키고자 할 때는 이 기본 값에 새로운
        값을 추가하거나 빼면14) 된다. ［리스트 7-4］에서는 기본 값에 DHCP 기능을 추가한 것을
        볼 수 있다. 비슷한 방법으로 제거는 다음과 같은 방식이다．

           #define C0NFIG_C0MMANDS   (C0NFIG_CMD_DFL & -CFG_CMD_NFS)


        예제를 더 알아보고자 한다면 . . . /include/configs／어］ 있는 보드용 헤더 파일들을 살
       펴보기 바란다．


7.3.3 네트워크 동작

       많은 부트로더가 이더넷 인터페이스를 지원한다. 개발 환경에서 이 기능을 쓸 수 있다면 상
       당한 시간을 절약할 수 있다. 최신 커널을 시리얼 포트를 통해서 다운로드하려면 몇 분이 걸
       리지만 10Mbps의 이더넷을 이용하면 몇 초면 가능하다. 또한 시리얼 연결은 터미널의 잘못
       된 입력에 의해서 에러를 발생시킬 확률이 더 높다．

       부트로더를 선택할 때 BOOTP, DHCP 그리고 TFTP를 지원하는지 여부도 상당히 중요하
       다. 이들 프로토콜에 대해서 익숙하치 않은 독자를 위해서 간단히 설명을 하자면 BOOTP
       （부E入드랩 프로토콜） 그리고 DHCP（동적 호스트 제어 프로토콜）는 이더넷 포트를 가치고
       있는 대상 디바이스가 II) 주소를 얻어 올 수 있도록 해 주고, 그 외에도 네트워크에 관련된
       구성 정보를 중앙 서버와 교환할 수 있도록 해 준다. TFTP（간이 파일 전송 프로토콜）는 대
       상 디바이스가 TFTP 서버에서 （리눅스 커널 이미지와 같은） 파일을 다운로드할 수 있도록


14) ［역자주） 추가는 0R 연산(I) 으로， 제거는 AND（邑）와 N0T(-) 연산으로 이루어진다．


                                                                               225 1
       a     Embedded Linux Primer




           해 준다. 이들 프로토콜에 대한 참고 자료 목록은 이 장의 마치막 부분을 보기 바란다. 이들
           프로토콜의 서버에 대해서는 12장, "임베디드 개발 환경"에서 설명할 것이다

           ［그림 7-1］은 대상 디바이스와 BOOTP 서버 간의 정보 흐름을 그림으로 설명한 것이다．
           클라이언트（여기서는 U-Boot）는 BOOTP 서버를 찾기 위해서 브로드캐스트 패킷15)
           (broadcast packet）을 내보낸다. 그러면 서버는 클라이언트를 위한 'p 주소와 기타 정보를
           담고 있는 응답 패킷을 보내는 것으로 응답하게 된다. 이 정보 중에는 가장 유용한 정보인
           다운로드할 커널 이미지 이름도 포함된다．

                U-Boot                     BOOTP/DHCP
                                              서버

           시작
           1入＼           BOOTREQUEST롤브로드캐스트함




                      대상 장치에만 BOOTREPLY 응답을 보냄


                                                   시간




           I 그림 7-1 BOOTP 클라이언트／서버 상호 작용


           사실 BOOTP 서버 역할만을 단독으로 수행하는 독립 서버는 더 이상 존재하지 않는다. 대부
           분의 리눅스 배포판에 포함되어 있는 DHCP 서버에서도 BOOTP 프로토콜 패킷을 처리할
           수 있다．

           DHCP 프로토콜은 BOOTP 위에서 동작하며 , 대상 디바이스에 다앙한 종류의 구성 정보를
           제공한다. 실제적으로 이러한 정보 교환은 제한된 수의 대상 디바이스 또는 부트로더만 가능
           하도록 되어 있다. ［리스트 7-司는 치정한 대상 디바이스 하나를 인식하도록 DHCP 서버를
           구성하는 구문의 예를 보여 주고 있는데 , 이 내용은 페도라 Core 2에서 사용하는 DHCP
           서버의 구성 파일의 내용에서 발췌한 것이다．

15) （역자주） 닙쿠트캐스트는 녜트워크의 모든 장치어｝ 패킷을 보내는 것을 말한다. 일빈적으로 최초에 서로 간을 인지하지 못하는
  경우 또는 무작위의 전체 디바이스에 정보를 전달하고자 할 때 사용힌다．


1226
                                                             부트로더   Chapter 7



［리스트 /5) DHCP 대상 명세서

   host coyote {
        hardware ethernet 00: oe: oc: 00: 82: f8;
        netmask 255. 255. 255. 0;
        fixed-address 192.168.1. 21;
        server-name 192.168.1.9;
        filename "coyote-zlmage";
        option root-path '"/home/chris/ sandbox/coyote- target";
   }




DHCP 서버는 ［리스트 7-5］에 기술된 이더넷 주소와 일치하는 디바이스로부터 패킷을 받으
면 이 내용에 기술되어 있는 파라미터들을 응답으로 보내게 된다. ［표 7-1］은 이러한 타깃
명세서의 파라미터 항목을 정리한 것이다．

［표 刀1] DHCP 대상 파라미터

 DHCP 대상 파라미터        용도                      설명

 host                호스트 이름                  DHCF 구성 파일 내부에서 사용되는 이름

 hardware ethernet   이더넷 하드웨어 주소             대상 디바이스의 이더넷 컨트尋但1
                                             하드웨어 주소

 fixed- address      대상 'P 주소                대상 디바이스에 할당할 'P 주소

 netmask             대상 디바이스 넷마스크            대상 다비이스에서 사용할 넷마스크

 server-name         TFTP 서버의 'P 주소          대상 디바이스가 루트 파일 시스템 등을
                                             위해서 파일 전송을 요청할 때 사용할
                                             서버의 'P 주소

 filename            TFTP로 전송할 파일 이름         부트로더7[ 2차 이미지（보통은 리눅스
                                             커널）를 가져올 때 지정할 파일 이름


대상 보드의 부트로더가 BOOTP 또는 DHCP 정보 교환을 끝마치면 추가 구성을 위해서
방금 설명한 파라미터들이 이용된다. 예를 들어 , 부트로더는 대상 II) 주소 파라미터를 이용
해서 , 자신의 이더넷 포트에 이 II) 주소를 설정伯md）한다. 그리고 난 후 부트로더는
server- name 필드를 이용해서 해당 II) 주소로 filename 필드에 있는 파일을 요청하는



                                                                        227 豆
蘚, 堪 U    Embedded Linux Primer




         데 , 이 파일은 대부분의 경우 리눅스 커널 이미지를 가리킨다. 비록 지금까지 설명한 이 방법
         이 가장 일반적으로 사용되는 시나리오이기는 하치만, 생산 라인에서 사용할 테스트 및 자체
         진단 펌웨어를 다운로드하고 실행시키는 데도 이용될 수 있다．

         DHCP 프로토콜은 ［표 7-1］에 설명한 것 외에도 많은 파라미터들을 지원한다는 것을 알아
         두기 바란다. ［표 7-1］에 있는 파라미터들은 단지 임베디드 시스템에서 자주 이용되는 것들
         을 정리한 것이다. 좀 더 자세한 내용을 위해서는 이 장의 마지막 부분에 참고 자료로 나와
         있는 DHCP 표준 문서를 참고하기 바란다．


7.3.4 저장 장치 서브시스템
         많은 부트로더가 부팅이미지를 일반적인 플래시 메모리 외에도 다양한 비휘발성 저장 장치로
         부터 가져 올 수 있는 기능을 가치고 있다. 다양한 종류의 저장 장치를 지원하는 것은 하드웨
         어 및 소프트웨어적인 측면16) 모두가 상대적으로 복잡해지기 때문에 어려운 작업이다. 하드
         드라이브에 있는 데이터에 접근하기 위해서 부트로더는 IDE 컨트롤러 인터페이스에 대한
    . 디바이스 드라이버는 물론이고, 하드디스크의 파티션 구조 및 파일 시스템에 대해서도 알고
         있어야 한다. 이런 작업은 소규모로 진행하기보다는 오히려 완전한 운영체제 시스템에서 더



         내재된 복잡성에도 불구하고 이런 종류의 장치에서 이미지를 불러올 수 있는 방법이 몇 가지
         있는데 가장 간단한 방법은 그냥 하드웨어 측면만 지원하는 것이다. 이 방법은 파일 시스템
         에 대한 부분은 고려하지 않는다. 즉, 부트로더가 단순히 디바이스의 정해진 섹터 공간에서
         바이너리를 직접 읽어 오는 것이다. 이 방법은 IDE 호환 저장 장치（예를 들어 , 콤팩트 플래
         시）에서 0번째 섹터부터 정해진 크기만큼의 공간을 별도의 파티션으로 예약해 두고, 파일
         시스템의 구조와는 무관하게 그 공간에서 데이터를 읽어 오는 방식이다. 이 방법은 커널 이
         미지나 기타 바이너리 이미지를 읽어 오기 위한 가장 이상적인 방법이다. 저장 장치의 나머
         지 파티션들은 어떤 형식으로든 포맷할 수 있고, 해당 파일 시스템으로 완전하게 사용할 수
         있다. 커널이 부팅된 후에는 이제 디바이스 드라이버를 이용해서 나머지 추가 파티션들도 올
         바로 접근할 수 있다．



16) （역자주） 하드웨어 측면은 하드디스크 드라이브를 제어하는 IDE 컨트롤러에 대한 디바이스를 생각하면 되正 소프트웨어 측면
    은 그 하드디스크 내부의 파일 시스템 및 파티션을 읽을 수 있도록 해 주는 소프트웨어를 생각하면 된다．
                                                      부트로더    Chapter 7



     U-Boot는 이미지를 지정한 로무尸파티션17）에서 읽어 올 수도 있고, 파일 시스템으로 구성
      된 파티션에서도 읽어 올 수 있다. 물론 보드가 그 하드웨어 장치（IDE 서브시스템）를 지원
      해야 하고, U-Boot도 올바로 구성되어야 가능한 일이다. U-Boot에서 보드 구성 파일에
      CEG CMD IDE를 추가하면 IDE 인터페이스를 사용할 수 있게 되고 거기에 CFGCMD
      BOOTD를 추가하면 로우U파티션에서 부팅하는 기능을 사용할 수 있다. 만약에 독자가 자신의
      보드에 맞게 U-Boot를 포팅하는 중이라면 U-Boot가 독자의 하드웨어 장치를 이해할 수 있
      도록 내용을 수정해야 한다.


7.3.5 디스크로부터 부팅하기

      이전 섹션에서 설명한 것처럼 U-Boot는 커널 이미지를 디스크 서브시스템으로부터 읽어 와
      서 부팅할 수 있는 기능을 지원한다. 다음의 명령어도 그 중 하나이다．

        => diskboot 0x400000 0:0

      위 문법을 이해하기 위해서는 먼저 U-Boot가 디스크를 인식하는 순서를 이해해야 한다. 위
      예에서 0: 0은 각각 디바이스와 파티션을 의미한다. 즉, 이 명령어는 U-Boot가 첫 번째
      IDE 장치(IDE device 0) 내의 첫 번째 파티션에서 원본 바이너리 이미지를 읽어 오는 일을
      수행하도록 한다. 그리고 이 이미지는 시스템 메모리의 물리 주소 0x400000으로 로드된다．

      커널 이미지가 메모리로 로드된 후에는 U-Boot의 bootm（메모리에서 부팅） 명령을 이용해
      서 커널을 부팅시킨다．

        => bootm 0x400000




7.4 小Boot 포팅하기
      口Boot가 이렇게 유명해진 이유 중의 하나는 새로운 플랫폼에 적용하기가 매우 쉽다는 점
      때문이다. 보드를 위한 포팅 결과물은 빌드 과정에서 해당 보드를 위한 정의 값을 제공하는
      하위 ri追kefile을 반드시 제공해야 한다. 이 파일은 모두 이름이 config.mk이고, U-Boot



17) （역자주） 파티션은 하드디스크의 논리적인 공간 딘위이다. 그리고 특정 파일 시스템으로 포맷되지 않은 파티션을 로두L파티션
    이라고 한다．
          Embedded Linux Primer




        소스 트리 상에서 . . . /board/xxx 하위 디렉터리에 모여 있다. 여기서 ＞妹x는 각각의 보드
        를 나타낸다．

        현재의 최신 U-Boot 버전 1.1.4에서는 . . . /boards 하위 디렉터리 밑에 각기 다른 보드들
        에 대한 구성 파일인 config.mk가 240개 이상 존재한다. 그리고 이 버전에서는 총 29개의
        다른 CPU 구성도 지원한다. 그리고 일부 경우에는 CPU 구성이 같은 계열의 여러 CPU들
        을 지원하기도 한다. 예를 들어 , ppc4xx는 PowerPC 全妖 계열의 CPU를 여러 7긔1지원한
        다. U-Bo毗는 근래에 많이 사용되는 CPU 및 CPU 계열들을 폭넓게 지원하고, 그에 따른
        다양한 참고용 보드도 상당수 지원한다.

        만약에 독자가 개발하고 있는 시스템이 口Boot가 지원하는 CPU를 사용한다면 U-Bo毗를
        독자의 보드 또는 시스템에 맞게 포팅하는 것은 상당히 직관적으로 가능하다. 하지만
        U-Boot가 지원하지 않는 새로운 CPU를 사용하도록 할 경우에는 상당한 노력이 필요하다．
        희소식은 이미 다른 누군가가 대부분 그 일을 해 놓았을 가능성이 아주 높다는 점이다. 만약
        에 새로운 CPU 또는 보드를 기존에 존재하는 어떤 CPU용 코드를 기반으로 포팅할 때는，
        기존의 소스 코드를 참고해서 작업을 진행해 나가야 한다. 어떤 CPU가 자신의 CPU와 가장
        비슷한지를 결정한 후에 , 그 CPU의 디렉터리에 있는 기능들을 그대로 복사해 와서 , 최종적
        으로는 그 소스에 새로운 CPU에 대한 내용을 추가하는 것이다.


7.4:1 EP405룰 위한 U-Boot 포팅
        같은 방식이 U-Boot를 새로운 보드에 포팅하는 일에도 적용된다. 예를 하나 들어 보자. 우
        리는 PowerPC 405GP 프로세서를 사용하는 임베디드 플래닛（Embedded Planet）의
        EP405를 사용할 것이다. 예제를 위한 이 특별한 보드는 임베디드 플래닛의 배려로 제공받
        은 것이고, 64MB의 SDRAM과 16MB의 플래시를 내장하고 있다. 그리고 다른 다앙한 장
        치들도 장착되어 있다.

        첫 번째 작업은 기존에 이미 지원되는 보드 중에서 가장 가까운 것을 찾는 것이다. U-Boot
        에서 PowerPC 405GP 프로세서를 지원하는 보드는 상당히 많다. 간단히 grep 명령을 이
        용해서 보드 구성 헤더 파일을 검색하면 405GP 프로세서를 지원하는 것만 추려낼 수 있다．

          $ cd . . ./u- boot/ jnc1ude/ configs$ grep -1 coNFIG_405GP *




I 230
                                                                                    )



                                                           부트로더      Chapter 7




최신 U-Boot 소스에서는 405GP 프로세서를 위한 보드 구성 파일 25개를 찾을 수 있다．
몇 가지를 검토한 결과 AR405 . h를 기본 틀로 선택하기로 한다. 이 파일은 EP405에서도
사용되는 I仄T971 이더넷 컨트롤러를 지원한다. 우리의 목적은오픈 소스의 정신에 따라서
최대한 다른 곳에서 필요한 내용들을 차용해서 개발 작업을 최소화하는 것이다. 먼저 간단한
일부터 처리하자. 이 보드 구성 파일을 우리의 보드에 맞는 새로운 이름으로 복사하자. 여기
서는 이름을 EP405.h로 정하도록 하자. 이를 위해서 U-Boot 최상위 디렉터리에서 다음
명령을 이용한다．

  $ cp . . ./include/ configs/ AR405. h . . ./include/ configs/ EP405.h


그리고는 보드를 위한 디렉터리를 하나 만들고 AR405용 파일들을 그곳에 복사한다. 아직은
그 파일이 모두 다 필요한 파일인지는 모르는 상황이다. 그 부분은 나중에 처리하자. 새로
만든 보드용 디렉터리에 파일을 복사한 후에는, 그 파일들의 이름을 자신의 보드에 맞는 이
름으로 바꾸도록 한다．

  Scd board <<< 나BOOt 소스 디렉터리의 최상위에서 실행시킨다．
  $ mkdir ep405
  $ cp esd/ ar405/ * ep405


이제부터는 어려운 부분이다. U-Boot의 개발자 중의 한 명인 제리 반 배런（Jerry Van
Baren）은 U-Boot 메일링 리스트를 통해 포스팅한 글에서 유머러스하면서도 상당히 현실적
으로 U-Boot의 포팅 과정에 대해서 이야기했다. C 언어 문법으로 된 이 문서의 전체 내용은
U-Boot의 REAl兆扼 파일에서 찾아볼 수 있다. 다음 내용은 포팅 작업에서 가장 어려운
과정에 대해서 제리가 사용한 방식과 철학에 따라서 표현한 것이다．



  while (! running) {           ／士 정상 동작 소／
       do {
              Add               ／央 소스 코드의 내용 추가／수정하기 央／
       } until (cor먀너］es) ;     ／女 컴파일 성공 士／/
       Debug;                   ／肯 디버깅하기 丹／




                                                                            231 1
          Embedded Linux Primer




        여기 요약된 제리의 작업 방식이 대략적으로는 사실이다. 포팅을 위해서 어떤 기준 코드를
        선택했으면 컴파일이 성공적으로 될 때까지 소스에 내용을 추가하거나 제거 , 변경하는 작업
        을 계속해야 하고, 에러 없이 실행될 때까지 계속 디버깅해야 한다！ 마법 같은 건 따로 없다．
        어떤 부트로더든 새로운 보드를 그 부트로더에 포팅시키는 것은 하드웨어와 소프트웨어 모든
        영역에 대한 상당한 지식을 필요로 한다. 그 중에서도 SDRAM 컨트롤러를 설정하는 등의
        작업은 좀 더 전문화되고 복잡한 작업18）이다. 실제로 포팅의 모든 과정은 시스템의 기반 하
        드웨어에 대한 지식을 필요로 한다. 결론적으로는 자신이 사용하는 프로세서의 하드웨어 참
        고 매뉴얼 그리고 보드에 존재하는 다앙한 하드웨어 부품들에 대한 데이터시트（data sheet)
        를 연구하는 데 많은 시간을 투자할 준비가 되어 있어야 한다．


7.4.2 U-Boot makefile의 구성 타깃
        기존에 존재하던 코드를 기반으로 시작했으므로 우리의 새로운 보드를 지원하기 위한 구성
        절차를 추가하기 위해서 U-Boot makefile의 내용을 수정하도록 하자. 이 II追kefile의 내용
        을 검토하다 보면 지원하는 많은 종류의 보드를 위해서 U-Boot 소스 트리를 구성하기 위한
        섹션을 찾아볼 수 있다. 이제 우리는 여기에 우리 보드를 추가하고, 빌드할 수 있도록 수정할
        것이다. ESD AR405 보드로부터 내용을 물려받았기 때문에 빌드를 위한 내용도 이 ESD
        AR405 보드의 내용을 기본 틀로 사용할 것이다. U-Boot의 소스 코드에 익숙한 독자라면
        빌드를 위한 구성 타깃을 정의하는 내용들이 그 이름에 따라서 알파벳 순서로 위치하는 것을
        볼 수 있다. 선량한 오픈小소스 시민으로서 이 순서를 지키도록 하자. 그리고 구성 타깃의 이
        름도 U-Boot의 관습에 따라서 EP405 config로 정하도록 하자．



          EBONY_conflg:      unconfig
               @./mkconfig $(@:_config=) ppc ppc4xx ebony

          +EP405config:        unconfig
          +    @ ./mkconfig $(@ :_config=) ppc ppc4xx ep405
          +
          ERIC_config:       unconfig
               @./mkconfi g 釘＠：工onfig=) 마）C 마）c4xx eric




18) （역자주） 하지만 해당 SDRAM과 컨트롤러에 대한 올바른 명세서 (Specifica如n）률 잘 이해하고 공부한다면 뭐든 해낼 수 있다．


I 232
                                                            부트로더    Chapter 7



      새로 추가된 내용은 앞에 （통합 diff 형식19）의） + 문자로 시작하는 서］ 줄이다．

      방금 설명한 沓｝를 끝마침으로써 , 이제 실제 작업을 시작할 수 있는 시작점（針帥ing p이nt)으
      로 삼을 만한 소스 코드가 준비된 셈이다. 아마 컴파일조차 정상적으로 되지 않을 수도 있는
      데 , 그게 첫 번째로 해결해야 할 작업일 것이다. 컴파일러가 알려 주는 에러 메시지들을 통해
      서 어디서부터 문제를 해결해 나가야 하는지 힌트를 얻을 수 있다．


7 ,4.3 EP405 프로세서 초기화
      새로 포팅할 U-Boot가 반드시 올바르게 해야 할 첫 번째 작업은 프로세서와 메모리
       (DRAM) 서브시스템을 초기화하는 것이다. 405GP 프로세서 코어는 리셋（reset）된 후에，
      OxFFFF FFFC에서 첫 번째 명령어를 가져오도록 설계되어 있다. 코어는 이 주소에 있는
      명령어를 실행시키려고 시도한다. 이 주소는 메모리 범위의 맨 끝 부분20）이기 때문에 , 여기
      에 존재하는 명령어는 반드시 무조건 분기 명령어가 되어야 한다.

      이 프로세서 코어는 상위 2MB의 메모리 영역을 외부 버스 컨트롤러를 설정하지 않고도 바
      로 접근할 수 있도록 미리 초기화하도록 설계되어 있다. 그리고 이 영역에는 일반적으로 플
      래시 메모리가 장착된다. 이 때문에 분기 명령어를 이 2MB 영역 내부의 위치로 분기하도록
      해야 하는데 , 왜냐하면 다른 영역의 메모리는 부트로더 코드가 추가 메모리 영역에 대해서
      초기화하기 전까지는 아직 사용할 수 없기 때문이다. 즉, 우리는 반드시 0姃巾E0 0000 또
      는 그 상위의 위치로 분기해야 한다. 필자가 이 모든 것을 어떻게 다 알 수 있었을까7 바로
      405GP 사용자 매뉴얼을 읽었기 때문이다！

      이전 단락에서 설명한 405GP 프로세서 코어의 동작 방식 때문에 , 하드웨어 디자이너는 전
      원을 켜는 시점에 비휘발성 메모리（플래시）가 상위 2MB 영역 부분에 매핑되어 있도록 보드
      를 디자인해야 한다. 이러한 초기 메모리 영역에 대한 속성들은 리셋 기본 값21）으로 설정된
      다. 예를 들어 , 이 초기 2MB 영역이 초기화되기까지 256사이클만큼의 시간 동안 기다린
      후에 , 주소 값을 통해서 칩을 선택（ch如 select）하기 위한 딜레이 3사이클（cycle) , 칩을 선

19) （역자주） d逾 유틸리티가 두 파일의 차이를 표현하는 방식 중의 햐나이다．
20) ［역자주） 伽FFFFFFFC어k 4byte만큼 사용하고 나면 더 이상 사용할 수 없는 메모리의 끝이다. 32비트 프로세서의 경우는 이
    주소가 마지막 번지이기 때문어］, 이 명령어가 시스템의 올바른 메모리 주소로 분기하지 않으면 다음 명령은 예측할 수 없는 곳
  에서 가져와야 할 것이다．
21) ［역자주） 프로셰서의 레지스터 및 구성 값은, 프로세서가 리셋되면 다시 기본 갔을 갖도록 되어 있다. 사용자 매뉴얼을 보면
  이 리셋 기본 값히］ 대해서 알아볼 수 있다.


                                                                         233
 難 毖二     Embedded Linux Primer




       택한 후에 그 내용을 읽어내는 데 3사이클 그리고 홀드 시간（ho'd time片2）을 위해서 7 사
       이클을 할당하고 있다23) .

        우리는 이미 ［리스트 7-2］에서 어떻게 리셋 벡터를 플래시의 맨 위쪽에 위치시키는지를 살
       펴보았다. 405GP를 U-Boot로 구성한 경우 맨 처음 실행될 U-Boot 코드는 . . . /cpu/
       ppc幻姚／star七．S이다. U-Boot 개발자들은 의도적으로 이 파일을 프로세서에 일반적으로
       적용할 수 있는 내용을 가지도록 만들었다. 그래서 이론상으로는 이 파일에서는 보드에 관련
        된 내용은 필요가 없어야 한다. 그럼 어떻게 그것이 가능한지 알아보자．

        5七art. S의 논리적인 흐름을 이해하기 위해서 PowerPC 어셈블리 언어에 대해서 상세하기
       이해하고 있을 필요까지는 없다. 그리고 저수준 어셈블리 코드를 수정하기 위한 수많은
       FAQ24）가 U十oot 메일링 리스트를 통해서 포스팅되고 있지만, U-Boot가 지원하는 프로
        세서를 사용하는 경우에는 거의 대부분 이 코드를 수정할 필요가 없다. 이 코드는 이미 여러
        곳에서 성공적으로 포팅되어서 문제 없이 동작하고 있는 성숙한 코드라고 볼 수 있으며 , 우
       리는 （가장 최소한으로） 보드에 관련된 코드만 수정하면 된다. 만약에 독자 중에서 문제 해
       결을 위해서 오랫동안 사용된 코드인 프로세서를 위한 초기 스타트업 어셈블러 코드를 변경
       하고 있다면 아마 거의 잘못된 길로 들어섰다고 보면 될 것이다.

       ［리스트 7-6］은 4xx 아키텍처를 위한 S七art S 코드 일부를 나타낸 것이다．

       ［리스트 7-6) 나Ba아의 4xx용 스타트업 코드




           #f              defjned (coNFIG_405GP) I I defined(CONFIG405CR) I I
            defined (CONFIG_405) I ! defined (CONFIG_405EP)

                                                                                    /
                                                                                    /
                                                               *1
                                                                六
                /*" clear and set up some registers.
                                                                    女               /
                     '"
                       "
                /"
                addi             r4, rO, Ox0000
                mtspr            sgr, r4
                mtspr            dcwr, r4



22) ［역자주） 홀드 타임 또는 보류 시간이라고도 한다. 데이터가 유지되는 시간이며, 이 시간 내에 데이터를 읽어 가야 한다. 너무
  짧을 경우 데이터를 읽어 가기도 전에 데이터가 사라질 수도 있다. 참고로 설정 시간 또는 셋업 타임 (setup time）은 데이터를
  신호선 또는 버스어］ 내보내는 더］ 걸리는 시간이다．
23) 이 모든 타이밍 정보들은 이 장 뒷부분의 참고문서에 니와 있는 사용자 매뉴얼에서 얻은 것이다．
24) ［역又阡） FAQ : Frequently Answered Que師on의 익쟈이며, 又H三 질문되는 문제에 대해서 답을 달아 놓은 문서이다．
                                                            부트로더      Chapter 7



   mtesr  r4                       /* clear Exception Syndrome Reg 必
   mttcr  r4                       /* clear Timer Control Reg 央/
   mtxer  r4                       ／央 clear 터xe小叱m t Exception Reg 女／
   nitevprr4                       /六 clear Exception vector Prefix Reg "" /
   addi   r4, rO, Ox1000           /"'" set ME bit (Machine Exceptions) */
   oris   r4, r4,0x0002            /"" set CE bit (Critical Exceptions) */
   mtmsr  r4                       ／必 change MSR 必／
   addi   r4, rO, (OxFFFF-Ox10000) /必 set r4 to OxFFFFFFFF (status in the */
                                   /"" dbsr is cleared by setting bits to 1) */
   mtdbsr r4                       /'" clear/reset the dbsr 央

   ／出
                                           央／

   /* Invalidate I and o caches. Enable I cache for defined memory regions
   亡／
   /* to speed things up. Leave the D cache disabled for now. It will be */
   /* enabled/left disabled later based on user selected menu options. */
   /女 Be aware that the I cache may be disabled later based on the menu 央／
   /*' options as well. See miscLib/main. c. */
   ／央                                           /'/

   bl        invalidate_i cache
   bi        i nval I date_dcache



   /* Enable two 128MB cachable regions.              VVV
   /／央

   addis r4, rO,0x8000
   addi   r4, r4,Ox0001
   mticcr r4                        ／央 instruction cache 女／
   1 sync

   addis r4, rO, Ox0000
   addi   r4, r4,Ox0000
   mtdccr r4                        /* data cache */



405GP 프로세서를 위한 코드인 star七 . S에서 처음 1/3은 프로세서의 일부 레지스터를 0
으로 초기화하거나 올바른 값으로 설정하는 일을 하고 있다. 그리고는 명령에 캐시와 데이터
캐시를 무효화시키고 나서 다시 명령에 캐시를 활성화시켜서 초기의 로딩 작업을 빠르게 진
행할 수 있도록 만든다. 두 개의 128MB 영역을 캐시되도록（cacheable) 설정하는데 , 하나
는 메모리의 윗부분（플래시 영역）이고, 나머지 하나는 아랫부분（보통 시스템의 DRAM의 시
         Embedded Linux Primer




       작 부분）이다. U-Bo毗는 최종적으로 스스로를 RAM에 복사해서 그곳에서 실행되도록 한
       다. 이렇게 하는 이유는 성능 때문이다. RAM에서 직접 데이터를 읽는 속도는 플래시에서
       읽는 것보다 수십 배 더 빠르다. 하찌만 4xx Cpu에서는 명령에 캐시를 켜는 또 다른 미묘한
       이유가 있는데 그 이유는 곧 알게 될 것이다．


7.4.4 보드에 따른 초기화
       보드에 맞는 초기화 작업을 처음 할 수 있는 부분은 . . . /cpu/ppo4xx/ star七. S에서 캐시
       를 적용할 영역들을 초기화한 바로 다음 부분이다. 여기서 어셈블리 언어로 작성된 외부 루
       틴을 호출하는 것을 볼 수 있다．

         bl ext_bus_cntlr_init     /'"" Board specific bus cntrl -mnit *


       이 루틴은 우리의 보드를 위해서 새로 만든 디렉티리에 있는 . . . /board/ep405/init. S
       파일에 정의되어 있다. 이 루틴은 초기 시점에서 하드웨어 초기화 작업을 미리 진행할 수 있
       는 수단을 제공한다. 이 파일은 EP405 플랫폼만을 위해서 존재하는 파일 중의 하나인데，
       이 파일에는 우리가 만들 프로그램에서 사용하기 위해서 405GP의 외부 버스 컨트롤러를 초
       기화하는 코드가 구현되어 있다. ［리스트 7-7］은 이 파일의 핵심 부분을 나타낸 것인데 , 바
       로 405GP의 외부 버스 컨트롤러를 초끼화하는 코드이다．

       ［리스트 二7] 외부 버스 컨트롤러 초기화


                . gi obi ext_bus_cntl r_i nit
         ext_I川乞cnt] 乙in-it :
             mflr        r4                /* save link register              *1
             bl          . .getAddr
         . .getAddr:
                                                                                    // /
                                                    士                          出
             mflr        r3                /"'" get 1 this_ address
                                                                                       /r
                                                /
                                                /
                                                r
                                                    央                          六
             mtlr        r4                /央 restore link register
                                            /
                                            /
                                           //
                                                    六                          六
             addi        r4, O, 14         /"" prefetch 14 cache lines. . .
                                                                                /
                                                                              // /
                                                                                /
                                                    六
             mtctr        r4               1六 . . .to fit this function       士  出
                                                                                  /
                                       /
                                       /
                                       //
                                       /
                                                    士
                                                cache (8x14=112 instr)
         . .ebcloop:
                                                                               卉
             icbt        rO, r3            /' prefetch cache line for [r3]
                                                                                      r
                                                                                    / /
                                                                                       /
                                                                                      /
                                                                               央
             addi        r3, r3, 32        /''" move to next cache line
                                                                               /
                                                                               /
             bdnz        . .ebcloop        /"" continue for 14 cache lines     六




 236
                                                              부트로더   Chapter 7




                                                                          V//////
   ／士
                                                                     央
   /* Delay to ensure all accesses to ROM are complete
                                                                     士
   /* before changing bank 0 timings
                                                                     出
   /央 200usec should be enough.
                                                                     卉
   /* 200, 000, 000 (cycles/sec) x .000200 (sec) =
                                                                     出
   /去 0x9c40 cycles
   ／亡                                                                出




   addis         r3,0, OxO
   onj           r3, r3,0xA000    /央 ensure 200usec have passed t    央/
   mtctr         r3

. .spinlp:
                                        //                           六

    bdnz         . .spinlp        1*" spin loop




                                        ////
                                                                     央
        ／女
                                                                     六
        /六 Now do the real work of this function
                                                                     卉
        /去 Memory Bank 0 (Flash and SRAM) initialization
                                                                     女
        ／出
    addi         r4,0, pboap         7* *'ebccfga = pbOap;           *7
    mtdcr        ebccfga, r4
    addis        r4,0,EBc0_BOAP@h/ 必 央ebccfgd = ERcO_BOAP;           *7
    onj          r4, r4, EBc0_BOAP@l
    mtdcr        ebccfgd, r4

        addi     r4,0,pbocr         1* 士ebCCfga = pbocr;             肖1
        mtdcr    ebccfga, r4
        addis    r4,0, EBc0_B0cR@h 7* *ebccfgd = EBc0_B0cR;          *7
        onj      r4, r4,EBc0_BOcR@l
        mtdcr    ebccfgd, r4

                                                                     士
                                                                                            4
                                                                                            1
         ／央
                                                                                                /
                                                                                                / /
                                                                     央
         /女 Memory Bank 4 (NVRAM & BcsR) initialization
         ／女
                                                                      士
                                                                                                  /




         addi    r4,0, pb4ap        1* *ebccfga = pb4ap;             玄1
         mtdcr   ebccfga, r4
         addis   r4,0,EBc0_B4AP@h 7* 肯ebccfgd = EBc0_B4AP;           央1
         onj     r4, r4, EBc0_B4AP치
         mtdcr   ebccfgd, r4




                                                                                    237 i
         Embedded Linux Primer




              addi       r4, O, pb4cr         /* *ebccfga = pb4cr;           *1
              mtdcr      ebccfga, r4
              adth s     r4, 0, EBCO_B4CR아     /"'" " ebccfgd = EBCO_B4CR;   六／
              onj        r4, r4 , EBCO_B4CR@1
              mtdcr      ebccfgd, r4

              b] r                           /"'" return                     丹／
        ［리스트 7-7］의 코드를 선택한 이유는 그 내용이 저수준의 프로세서 초기화를 수행하는 미
        묘하게 복잡한 코드를 전형적으로 보여 주는 예제이기 때문이다. 여기서는 이 코드가 실행되
        는 문맥을 이해하는 것이 중요하다. 이 코드는 아직 DRA玉/1을 사용할 수 없는 시점에서 , 즉
        플래시에서 곧바로 실행된다. 물론 스택도 존재하지 않는다. 이 코드의 내용은 현재 코드가
        실행되고 있는 플래시에 대한 접근을 처리하는 컨트롤러를 재설정하기 위한 준비를 하는 것
        이다. 이와 같이 코드를 플래시에서 실행시키는 도중에 플래시가 장착되어 있는 외부 버스
        컨트롤러에 대한 설정을 변경시켜야 함으로써 잘못된 읽기를 수행하거나, 프로세서 충돌을
        일으킬 수 있는 특수한 프로세서의 경우는 그 내용에 대한 문서화가 잘 되어 있다．

        이 어셈블리 루틴에도 그 해결책이 나와 있다. . . . getAddr라는 레벨에서부터 다음 일곱
        줄까지의 어셈블리 코드는 icbt 명령어를 이용해서 자기 자신을 명령에 캐시로 프리페치되
        도록（prefetch25) ) 한다. 서브루틴 전체가 모두 성공적으로 명령에 캐시에 올라오게 되면
        이제 시스템 오류가 발생할 걱정 없이 외부 버스 컨트롤러를 재설정하는 작업을 진행할 수
        있다. 이는 명령어를 메모리가 아닌 캐시에서 수행하기 때분이다. 작지만 아주 영리한 방법
        이다！ 이 루틴의 마치막에 있는 짧은지연（d이ay) 시간을 갖는 코드는 명령에 캐시에 명령어
        가 완전히 프리페치될 때까지 어느 정도 기다려 주는 것이다．

        프리페치와 지연 시간까치 모두 마친 후에는 보드상의 메모리 뱅크 0번과 4번을 올바로 사용
        할 수 있도록 설정하는 일을 진행하게 된다. 이때 사용되는 값들은 보드에 장착된 구성 요소
        와 그 연결에 대해서 세부 지식을 가치고 있어야 알 수 있는 것들이다. 관심 있는 독자는 이
        장의 마지막 부분에 있는 "더 읽어 보기"에서 현재 예제에서 사용한 PowerPC 어셈블리 언어
        와 405GP 프로세서에 대한 참고 자료를 보기 바란다．


25) （역자주） prefetch는 CPU가 앞으로 실행시킬 명령어들을 미리 읽어 놓는 기술이다. 원래의 CPU 구조는 실행할 코드를 매번 메
    모리에서 가져오도록 되어 있는데, 이를 페치（fetch）라고 한다. 그리고 미리 가져오는 것을 프리（pre) 페치（fetch）라고 하는 것
  이다．


I 238
                                                            부트로더    Chapter 7



        만약에 이 코드가 정확히 어떤 일을 하는지에 대해서 완벽히 이해하지 못한 채 코드를 바꾸는
        경우를 생각해 보자. 아마도 몇 줄의 코드를 추가한다면 캐시에 프리페치시켜 놓을 수 있는
        크기를 벗어날 수도 있을 것이다. 그렇게 되면 시스템 오류가 발생할 것이지만（더 나쁜 상황
        은 가끔씩만 오류가 발생할 수도 있다는 것이다）, 디버거를 이용해서 한 단계씩 밟아 가면서
        분석하려고 하는 것도 정확한 단서를 찾기 힘든 상황이 된다．

         보드를 위한 초기화를 실행시킬 수 있는 다른 위치는 프로세서의 테이터 캐시로부터 임의의
        스택을 할당한 직후이다. 다음은 . . . /cp바ppc4xx/ s七art.S의 727번째 줄에서 SDRAM
         컨트롤러를 초기화하는 루틴으로 분기하는 부분이다．

            bi sdram_init

        이제 실행을 위한 문맥에서 스택 포인터와 로컬 변수를 위한 일부 임시 메모리를 사용할 수
        있게 되었다. 이 문맥에서는 C 언어를 일부 지원할 수 있기 때문에 개발자가 시스템의
        SDRAM 컨트롤러와 다른 초기화 작업들을 설정하는 복잡한 작업을 C를 이용해서 작성할
        수 있게 된다. 우리의 EP405를 포팅한 소스                /b（그ard/ep405/ep405 .O어］ 있는
         sdrao느mnit () 함수는 특정한 보드와 DRAM 구성을 위한 내용을 담고 있다. 이 보드는
        상업적으로 판매되는 메모리 Sil小vi 형태26）를 이용하지 않키 때문에 동적으로 DRAM을 구
        성할 수 없다. 이 보드 외에도 U-Boot가 지원하는 보드들 중에는 町MM 형태를 사용하지
        않는 경우가 아주 많다. 그래서 sdram mni七의 내부는 동적인 초기화가 아닌, 미리 결정된
        모듈을 초기화하도록 작성되어 있다．

        많은 상업용 DDR 모듈은 메모리 모듈을 정의하는 파라미터를 저장하고 있는 SPD27)（직렬
        방식의 존재유무 감지） PROM이라는 PROM을 내장하고 있다. 이 파라미터 값들은 I2C를
        통해서 소프트웨어적으로 읽어낼 수 있고, 메모리 컨트롤러를 알맞게 초기화하기 위한 정보
        로 이용된다. U-Boot는 이 기술을 지원하키는 하지만, 독자가 사용하는 자체 보드에서도
        동작하게 하려면 코드를 일부 수정해야 할 것이다. 이 기술을 이용하는 예제로 사용할 만한
        코드는 U-Boot 소스 코드 내에서 많이 찾아볼 수 있다. 구성 옵션 CONFIG SP口EEPROM
        을 이용해서 이 기능을 활성화시킬 수 있다. 이 옵션에 대한 grep 명령을 이용하면 예제를
        찾아볼 수 있을 것이다．

26) （역자주） lX：를 열어 보자. 메모리를 꽂을 수 있는 슬롯이 존재하는데, 이를 SIMM이라고 흐丘＋. 필요한 만큼 꽂아서 사용할 수
    있다. 그렇기 때문어］ 동적인 구성을 해야 힌다． 하지만 일반 개발 보드는 보통 DRAM 모듈이 보드에 납땜되어서 붙어 있다．
    이는 미리 정혜진 용량을 사용하도록 정적으로 구성되어 있기 때문에， 동적으로 몇 개의 메모리 모듈이 꽂혀있는지 등을 파학
    할 필요가 없는 것이다．
27) Serial Presence Detect : 직렬 방식의 존재 유무 감지


                                                                         239 1
         Embedded Linux Primer




7.4,5 포팅 요약
       이제 부트로더를 새로운 하드웨어 플랫폼에 맞게 포팅하는 작업에 어떤 어려움이 있는지 이
       해했을 것이다. 이는 기반 하드웨어에 대한 세부 지식 없이는 결코 간단히 이루어질 수 없는
       작업이다. 물론 이 작업에 필요한 시간을 최소화해야 할 것이다. 결국, 프로세서의 모든 하드
       웨어적인 부분에 대한 세부 지식을 얼마나 이해하는지에 따라 보수를 받는 것이 아니라, 보
       통은 정해진 시간 안에 제대로 동작하는 솔루션을 만들어 내는 일로 보수를 받을 것이기 때문
       이다. 오픈 소스가 번성하게 된 주된 원인 중의 하나도 바로 이러한 점 때문이다. 지금까지
       U-Boot를 새로운 하드웨어 플랫폼에 포팅하는 것을 얼마나 간단하게 할 수 있는지를 살펴
       봤다. 이렇게 쉽게 가능했던 것은 우리가 프로세서에 대한 일류 천문가였기 때문이 아니라,
       많은 사람들이 그 어려운 일들을 미리 했기 때문이다．

       ［리스트 7-8］은 EP405를 U-Boot어］ 포팅한 결과 새롭게 추가되거나 변경된 파일들의 전체
       목록이다. 물론 U-Boot가 기존에 지원하치 않는 하드웨어 장치를 가지고 있거나, 또는
       U-Boot7} 지원하지 않는 새로운 Cpu를 포팅하는 경우라면 이 작업은 훨씬 더 많은 노력이
       필요할 것이다. 여기서 말하고자 하는 요점은, 너무 같은 소리만 하는 것 같지만, 하드웨어
       (CPU와 서브시스템들）와 기반 소프트웨어 (U-Boot）에 대한 세부적인 지식 없이는 정해친
       시간 안에 포팅을 간단히 끝마칠 수는 없을 거라는 것이다. 이런 마음가짐으로 프로젝트에
       임한다면 분명 성공적인 결과물을 얻을 수 있을 것이다.

       ［리스트 가8] 나Boot EP405룔 포팀하면서 수정되거나 추가된 파일들

         $ diff -purN u-boot u-boot-ep405/ I grep +++
         +++ u-boot-ep405/board/ep405/config.mk
         +++ u-boot-ep405/board/ep405/ep405. c
         +++ u-boot-ep405/board/ep405/ep405. h
         +++ u-boot-ep405/board/ep405/ flash. c
         +++ u-boot-ep405/board/ep405/init. S
         +++ u七oot-ep405/board/ep405/Makefile
         +++ U七的卜叩405/board/ep405/u止oot그ds
         +++ u-boot七p405/include/config. h
         +++ u-boot-ep405/include/config.mk
         +++ u-boot七p405/include/configs/EP405. h
         +++ u寸）oot-ep405/ jnc1ude/ppc405. h
         ++i- u七oot-ep405/Makefile




 240
                                                                 부트로더   Chapter 7



    . . . /board/ep405에 있는 파일은 모두 다른 디렉터리에서 가져와서 사용한 것이라는 것을
    다시 떠올려 보자. 결국 처음부터 새로운 것을 만들어 낸 것은 하나도 없다. 다른 사람이 작
    업한 것을 빌려다가 우리의 목적을 달성하기 위해서 알맞게 수정한 것이다．


7.4.6 나Boot 이미지 헝식
    이제 우리는 EP405 보드에서 동작하는 부트로더를 확보했기 때문에 , 프로그램을 로드하고
    실행시킬 수 있게 되었다. 물론 우리가 실행시키고자 하는 프로그램은 리눅스와 같은 운영체
    제가 될 것이다. 우선 그렇게 하기 위해서는 U-Boot가 요구하는 이미지 형식에 대해서 이해
    할 필요가 있다. U-Boot는 이미지에 대해서 몇 가지 속성을 파악할 수 있도록 작은 헤더
    부분을 필요로 한다. U-Boot를 위한 이미지 헤더를 만들기 위해서는 mkimage라는 툴
    (U-Boot 소스 코드에 포함되어 있다）을 이용한다．

    최신 리눅스 배포판의 경우에는 U-Boot를 이용해서 직접 부팅 가능하도록 이미지를 만들어
    주는 기능을 자체적으로 가지고 있기도 하다. 이를 위해서 ARM과 PowerPC용 리눅스 소스
    코드는 모두 ulmage라는 타깃을 지원한다. 그럼 PowerPC의 경우를 한번 보도록 하자. 다
    음은 .. ./arch/ppc/boo七／images/Makefile의 일부분을 나타낸 것인더 , U-Bo毗를
    위한 대상 이미지를 만들어 주는 타깃인 UImage의 내용을 기술하는 부분이다．



      quiet_cmd_uimage = UIMAGE $@
            cmd.-uimage = $(CONFIG_SHELL) $(MKIMAGE) -A ppc \
           -o 1j flux -T kernel -c gzj p -a 00000000 -e 00000000 \
           -fl 'Linux- $(KERNELRELEASEY -d $< $@




    복잡한 문법은 무시하고, 이 내용이 $ (MKIMAGE) 라는 변수가 가리키는 쉘 스크립트를 호출
    한다는 것을 이해하면 된다. 이 쉘 스크립트는 mkimage 유틸리티를 그 다음에 나오는 변수
    들을 이용해서 호출한다. mkimage 유틸리티는 U느Boot용 헤더를 만들고, 제공된 커널 이미
    지 앞부분에 추가하는 일을 한다. 파라미터에는 다음과 같은 것들이 있다．

      -1\ 대상 이미지의 아키텍처를 지정
      -o 대상 이미지가 어떤 Os인지를 지정 1 여기서는 Linux
      -T 대상 이미지의 타입을 지정 e 여기서는 kernel
              Embedded Linux Primer



              -
                   c   대상 이미지의 압축 형식 지정     여기서는 gzip

              片a
                       小Boot가 로드할 주소인 加adaddress를 지정한 값으로 설정 寸 여기서는 0

              -
                   e   小Boot가 실행시킬 이미지의 시작점 주소를 지정

              -n
                       사용자가 구분할 수 있도록 읽을 수 있는 문자로 된 이미지 이름

              -
                   d   헤더를 추가시킬 실행 이미지 파일


       일부 U-Boot 명령어는 이 헤더에 있는 데이터를 이미지의 무결성을 검사하는 데 이용하기
       도 하고（이는 U-Boot가 헤더에 CRC 코드도 포함시키기 때문이다） 명령어가 이미지를 가
       지고 무슨 일을 해야 하는지를 지시하는 데도 사용한다. U-Boot에는 iminfo라는 명령어가
       있는데 , 대상 이미지에서 헤더를 읽어서 이미지 속성들을 표시해준다. ［리스트 7-9］는
       iminfo 명령을 이용해서 U-Boot의 七f七pboot 명령을 통해 EP405 보드에 로드한
       (U-Boot 형식으로 만들어진 부팅 리눅스 커널 이미지인） ulmage의 속성 값을 표시한 결과
       이다．

       ［리스트 万9) L士Boot의 iminfo 명령에 실행 결과

         => tftpboot 400000 ulmage-ep405
         ENET Speed is 100 Mbps - FULL duplex connection
         TFTP from server 192.168.1.9; our Ii' address is 192.168.1. 33
         Filename 'ulmage- ep405 '
         Load address: 0x400000
         Loading: ########## done
         Bytes transferred = 891228 (d995c hex)
         => iminfo

          ## Checking Image at 00400000 . . .
             Image Name: Linux-2.6.11. 6
             Image Type: PowerPC Linux Kernel Image (gzip compressed)
            Data Size:     891164 Bytes = 870. 3 kB
             Load Address: 00000000
            Entry Point: 00000000
             verifying Checksum . . . OK
         =>
1242
                                                              부트로더   Chapter 7




7.5 기E1 부트로더
      이제 다른 인기 있는 부트로더에 대해서 그들이 어디에 주로 이용되는지를 설명하고, 각각의
      부트로더가 가지고 있는 특징을 정리해 보도록 하자. 부트로더에 대해서 완전히 설명하기 위
      해서는 각 부트로더마다 별도로 책 한 권씩은 필요하기 때문에 불가능하다. 관심 있는 독자
      는 추가적인 내용을 위해서 이 장의 마지막에 있는 "더 읽어 보기"를 보도록 하자．


7.5.1 Lilo
      Linux Loader 또는 Lilo는 데스크탑을 위한 상업용 리눅스 배포판에서 광범위하게 사용되
      었었다. 그 중에서도 특히 x86/IA32 아키텍처에 뿌리를 두고 있다. Lilo는 몇 개의 구성
      요소로 이루어져 있는데 디스크 드라이브의 첫 번째 섹터28）어］ 존재하는 1차 부E入드랩 프
      로그램을 가지고 있다. 이 1차 로더는 디스크 섹터 크기로 크기가 제한되어 있는데 , 보통은
      512바이트이다. 그래서 1차 로더의 주된 임무는 간단히 2차 로더를 로드하고 제어권을 넘기
      는 일이다. 2차 로더는 다양한 파티션에 존재할 수 있으며 , 부트로더의 역할 대부분을 여기
      서 수행한다．

      Lilo의 동작은 구성 파일과 lbO의 실행 파일 중의 하나인 설정 유틸리티에 의해서 결정된
      다. lilo 구성 파일은 오직 그 운영체제의 제어 하에서만 읽고 수정할 수 있다. 그 말은 구성
      파일이 1차 로더나 2차 로더의 초기 부트 코드에서 이용되지 않는다는 것이다. 대신 시스템
      을 설치할 때나 나중에 관리 작업을 통해서 1110 구성 유틸리티가 구성 파일의 내용을 읽어
      들여서 처리한다. ［리스트 7-10］은 일반적인 리눅스와 ＼版ndows 다중H부트（dual-boot)
      환경을 위한 간단한 1i1o.conf 구성 파일의 내용을 나타낸 것이다．

      ［리스트 二10] L加 구성 파일의 0小 : IiIo.conf

         # This is the global lilo configuration section
         # These settings apply to all the "image" sections

         boot = /dev/hda
         timeout=50
         defaul t=l i nux
         # This describes the primary kernel boot image


28) 이는 역사적인 이유 때문이다. 즉, 초창기 PC에서는 텨Os 프로그램이 디스크 드라이브에서 첫 번째 섹터만 읽어서 그 쿠亡를
    실행시켰었다．
         Embedded Linux Primer




          # Lila will display it with the label 'linux '
          i mage=/boot/myLi nux- 2 .6.11.1
                   label=linux
                   initrd=/boot/mylnitrd-2. 6. 11.1.img
                   read-only
                   append=" root=LABEL=/'

          # This is the second OS in a dual-boot configuration
          # This entry will boot a secondary image from /dev/hdal
          other=/dev/hdal
                  optional
                  label =that_othe r_os



       이 구성 파일은 Lilo 구성 유틸리티가 첫 번째 하드 디스크（/dev/hda）의 MBR（마스터 부
       트 레코드）을 사용하도록 설정하고 있다. 그리고 사용자가 정해진 시간 안에（여기서는 5초）
      키를 누를 때까지 기다린다. 이는 시스템 관리자가 부팅할 0s 이미지를 선택할 시간을 주는
       것이다. 만약 시스템 관리자가 시간이 경과하기 전에 (Tab) 키를 누르면 운영체제를 선택하
       기 위한 리스트를 볼 수 있다. Lilo는 각 항목의 이름을 위해서 각 이미지의 label 항목을
       이용한다.

       이미지는 구성 파일 내에서 image 항목으로 정의된다. ［리스트 7-10］에 나온 예제에서는
       1차（또는 기본） 이미지로 myLinux-2. 6.ll. l이라는 파일 이름을 갖는 리눅스 커널 이미
      지를 사용한다. Lilo는 이 이미지를 하드디스크로부터 읽어 오게 된다. 그리고 초기 램디스
       크를 위해서 두 번째 파일을 읽어 오는데 이 파일이 mylni七rd-2. 6.ll. l. img이다. 그리
       고 lilo는 커널 커맨드 라인 ，노OO七可PiBEL= /"를 만들고, 리눅스 커널이 실행될 때 전달한
       다. 이 내용은 리눅스가 부팅된 후에 어디에서 루트 파일 시스템을 가져올 것인지를 알려 주
       는 것이다．


7.5.2 GRUB
       현재는 많은 상업적인 리눅스 배포판이 주로 GRUB29）을 부트로더로 사용한다. GRUB 또
       는 GRand Un泊ed Bootloader（대통합 부트로더）는 GNU 프로젝트이다. GRUB은 Lilo
       에서는 찾아볼 수 없는 많은 확장 기능을 가지고 있는데 , GRUB과 Lilo의 가장 큰 차이점은


29) （역자주） 주로 "그럽'히라고 읽는다．
                                                             부트로더      Chapter 7




파일 시스템과 커널 이미지 형식을 인식하는 능력이다. 추가적으로 GRUB은 부팅 시점에
구성 파일을 읽거나 변경할 수도 있다. 특히 임베디드 개발 환경에서는 매우 유용하게 사용
되는 기능인, 네트워크를 통해서 부팅하는 기능을 지원한다. 부팅 시점에 부트 구성 옵션을
변경하기 위해서 GRUB은 升맨드 라인 인터페이스를 제공하고 있다．

Lilo와 같이 GRUB도 구성 파일을 통해서 동작하게 된다. 하지만 Lilo의 정적인 구성과는
달리 , GRUB은 구성 파일을 부팅 시간혀］ 읽어서 처리한다. 이는 부팅 시점에 시스템 구성을
변경해서 부트로더의 동작을 수정할 수 있다는 것을 의미하는 것이다．

［리스트 7-11］은 GRUB 구성 파일의 예를 나타낸 것이다. 이 내용은 이 책을 쓰고 있는
PC에서 사용되는 구성 파일을 나타낸 것이다. grub. conf라는 GRUB 구성 파일은 보통
부트 이미지를 저장하는 전용 파티션에 위치한다. 이 예제가 사용되는 PC에서는 그 위치가
/boot이다．

［리스트 7녀 ]] GRUB 구성 파일의 0카 : gr止工conf


   defaul t=O
   timeout=3
   spi ashjmage=(hdO,1) /grub/ splash .xpm. gz

   title Fedora Core 2 (2. 6. 9)
           root (hdo,1)
          kernel /bzlmage- 2. 6. 9 ro root=LABEL=/ rhgb proto=伽ps quiet
          initrd /initrd- 2. 6. 9. img

   title Fedora Core (2. 6. 5-1. 358)
           root (hdo,1)
          kernel /vmlinuz- 2. 6. S-1. 358 ro root=LABEL=/ rhgb quiet

   title That Other OS
           rootnoverify (hdo, O)
           chainloader +1




GR1尼은 사용자에게 먼저 부팅할 수 있는 이미지의 목록 을 표시한다. ［리스트 下11］에서
볼 수 있는 title 값들이 사용자에게 보여 주는 이미지 이름으로 이용된다. defaul七라는
태그는 사용자가 지정한 시간 내（이 예제에서는 3초 내）에 키 입력을 하지 않을 경우에 기본
 難難1     Embedded Linux Primer




       값으로 선택할 이미지를 결정하게 된다. 이미지를 가리키는 숫자는 0부터 순서대로 번호가
       매겨진다．

       Lilo와는 달리 GRUB은 주어진 파티션에서 이미지를 불러올 때 실제 파일 시스템을 통해서
       읽어 올 수 있다. roo七 태그는 grub. conf어］ 기술된 파일들이 위치하고 있는 파티션을 가
       리키는 데 이용된다. 이 예제 구성 파일에서는 roo七7下 root (hdO, 1）로 되어 있는데 , 이는
       첫 번째 하드디스크의 1번 파티션을 가리키는 것이다. 파티션들은 0부터 번호를 매기기 때문
       에 첫 번째 하드디스크의 두 번째 파티션을 가리킨다．

       그리고 이미지의 위치는 root에서 기술한 곳에서부터의 상대 경로 위치를 나타낸다. ［리스트
       7-11］에서 기본 부트 이미지는 리눅스 2.6.9 커널이며 , 초기 램디스크로 mnl七rd-2.
       6. 9.1mg를 사용한다. GRUB 문법에서는 커널 커맨드 파라미터가 커널 파일을 명시하는
       곳과 같은 줄에 나오는 것에 주의하도록 하자．


7.5.3 더 많은 부트로더
       기타 다양한 부트로더가 자신들만의 틈새시장을 갖고 있다. 예를 들면 Redboot는 인텔과
       엑스스케일 공동체에서 인텔 IxP와 PXA 프로세서 계열을 장착한 평가용 보드에서 사용하
       도록 개발된 오픈 소스 부트로더이다. 마이크로모니티（Micromoni切r）는 코젠트（Cogent)
       등의 보드 업체에서 사용된다. YAMON30）은 MU뇽 쪽에서 많이 사용되는 부트로더이다．
       LinuxBIOS는 X86 환경에서 주로 사용된다. 일반적으로 부트로더에 대해서 고려할 때는
       다음에 나열한 것과 같은 중요한 사항들에 대해서 먼저 생각해 보아야 한다．

         다 내가 선택한 프로세서를 지원하는가9
         口 포팅된 보드 중에서 내 보드와 비슷한 것이 있는가9
         口 내가 필요로 하는 기능을 지원하는가2
         [a 내가 사용하려는 하드웨어를 지원하는가7
         [a 지원을 받을 수 있도록 많은 사용자 커뮤니티를 갖고 있는가7
         口 상업적으로 지원해 주는 업체가 있는가7


30) YAMON 사용자 매뉴얼 문서에는 기존에 존재하던 많은 부트로더들을 의식해서 자기 자신을 '또 5k4의 모니터'라는 의미인 Yet
    知l아her MONit야라고 설명하고 있다．


 246
                                           부트로더   Chapter 7



   이 사항들이 독자가 자신의 임베디드 프로젝트에서 사용할 부트로더를 결정할 때 고려해야
   할 내용이다. 독자가 최신 프로세서를 사용하는 시스템과 같이 기술적으로 "매우 치열한' 제
   품을 개발하는 경우가 아니라면 보통은 누군가가 이미 해당 플랫폼에 부트로더를 포팅한 결
   과물을 찾을 수 있을 것이다. 최종 결정을 내리는 데 "더 읽어 보기"에 있는 자료도 참고해
   보기 바란다．



7.6요약
    口 임베디드 시스템에서 부트로더의 역할을 과대평가하지 않도록 하자. 부트로더는 전원이
        공급되면 처음 실행되는 소프트웨어 코드이다．

    口 부트로더의 역할을 알아보았고, 부트로더가 실행되는 시점에서 실행 문맥（컨텍스트）이
        상당히 제한적이라는 점에 대해써 설명했다．

    口 Das U-Boot는 많은 프로세서 아키텍처에서 폭넓게 사용되는 인기 있는 부트로더이다．
        小Boot는 많은 수의 프로세서와 하드웨어 플랫폼 및 사용자 보드를 지원한다．

    口 小Boot는 지정한 보드를 위한 혜더 파일어］ 다양한 구성 변수들을 이용해서 설정하게
        된다. 부록 B에서 최신 ［尸Boot에서 지원하는 모든 명령에 집합에 대한 목록을 볼 수
        있다．

    [a 小Boot가 지원하는 프로세서에 기반한 새로운 보드를 포팅하는 것은 상대적으로 쉽다．
        이 장에서는 小Boot 내에 이미 포함되어 있는 비슷한 보드의 코드를 이용해써 새로운
        보드를 포팅하는 과정을 한 단계씩 설명했다．

    口 부트로더를 수정하거나 새롭게 포팅하는 작업은 프로세서와 하드웨어 플랫폼에 대한 세
        부적인 지식 없이는 불가능한 일이다．

    口 자신의 요구 사항에 맞는 부트로더를 선택하는 데 도움이 될 수 있도록 현재 임베디드
        시스템에서 사용되고 있는 다른 부트로더에 대해서 대략적으로 알아보았다.
  群U    Embedded Linux Primer




7.6. ] 더 읽어 보키
         어플라케아션 노트3刀“ 副9RA人f에 甲한 소71/
        맥스웰 테크놀로지스（Maxwell Techn아ogles)
         www. maxwell. com/pdf/me/app_notes/Intro_to_SDRAM. pdf


        乙1) 사용하刀, （刃vi/ 랑커 문서
        프리 소프트웨어 재단

         www. gnu. org/software/binutils/manual/ld-2. 9.1/id. html


         T帥I8xxL을 위한 DENX U-Boot 및 라눅스 가아드（比［JG)
        볼프강 Denx 등. Denx 소프트웨어 엔지니어링
         www. denx. de/twiki/bin/view/DULG/Manual


         RFC 793문서 "Trivial File Transfer Protocol"
         IETF(The Internet Engineering Task Force)
         www.ietf.org/rfc/rfc793.txt


         RFC 951문서, "부트스트랩 프로토콜：Bootstrap Pr毗ocol"
         IETF(The Internet Engineering Task Force)
         www.ietf.org/rfc/rfc951.t玭


         RFC 1531문서 , "Dynamic Host （兀ntr아 Pr毗ocol"
         IETF(The Internet Engineering Task Force)
         www.ietf.org/rfc/rfc1531. t玭


         PowerPC 405GP 임베디드 프로세서 사용자 매뉴얼
         IBM(International Business Machines, Inc.)


         32비트 PowerPC 아키텍처를 위한 프로그래밍 환경 매뉴얼
         프리스케일 반도체（Freescale Semiconductor, Inc.)




31) （역자주） 개발 보드 업체나 프로세서 업체가 제공하는 문서 중에서, 특정한 주제에 대해서 응용 人忙카를 설명하는 문서를 어플
    리케이션 노트라고 한다．
                                 부트로더   Chapter 7




Lilo 부트로더
www. tldp. org/HOWTO/LILO.html


GRUB 부트로더
www. gnu. org/software/grub!




                                               249
Chapt在伊 乙




          디바이스 드라이버 기초




U 디바이스 드라이버의 개념

. 모듈 유틸리티

U 드라이버의 메서드

U 한데 묶기

U 디바이스 드라이버와 GPL

U 요약
蘿1 1     Embedded Linux Primer




        시스템을 디자인하는 데 있어서 좀 더 어려운 부분은 시스템의 여러 기능을 합리적으로 분리
        시키는 일이다. UNI)따 리눅스에서 볼 수 있는 익숙한 디바이스 드라이버 모델은 독자의
        어플리케이션 코드와 하드웨어 또는 커널 디바이스 간의 기능 분리가 자연스럽게 가능하도록
        설계되어 있다. 이번 장에서는 이 모텔과 리눅스 디바이스 드라이버의 기본 구조에 대해서
        이해해 보도록 하자．

        먼저 리눅스 디바이스 드라이버의 개념을 설명하고, 커널 소스 트리 내에서 디바이스 드라이
        버를 빌드시키는 빌드 시스템을 알아보도록 하자. 그리고 리눅스 디바이스 드라이버의 구조
        를 설명하고, 간단한 예제 드라이버를 하나 만들어서 동작시켜 볼 것이다. 또 커널 모듈1）을
        커널에 올리고 또 내리는 데 필요한 간단한 사용자 영역 유틸리티를 알아볼 것이다. 간단한
        어플리케이션을 하나 이용해서 어플리케이션과 디바이스 드라이버 간의 인터페이스에 대해
        서도 알아볼 것이다. 마지막으로는 디바이스 드라이버와 GNU 공공 라이선스에 대해서 논의
        해 보는 것으로 마무리하도록 하자．



8. ] 디바이스 드라이버의 개념
        경험 많은 개발자라도 상당수가 처음에는 가상 메모리를 이용하는 운영체제에서 디바이스 드
        라이버의 개념을 이해하는 데 상당히 애를 먹는다. 이는 기존에 많이 사용되던 실시간 운영
        체제와는 다른 구조를 가지고 있기 때문이다. 가상 메모리와 커널 영역 그리고 사용자 영역
        등의 익숙하지 않은 개념들 때문에 복잡함을 느끼는 것이다．

        디바이스 드라이버의 가장 기본적인 목적 중의 하나는 사용자의 프로그램을 커널의 중요한
        데이터 구조나 하드웨어 장치에 직접 접근하지 못하도록 따로 분리시키는 것이다. 또한 잘
        작성된 디바이스 드라이버는 하드웨어 장치의 복잡하고 가변적인（variability) 성질을 사용
        자에게는 숨긴다. 예를 들어 프로그램에서 하드 디스크에 데이터를 쓰려고 할 때 하드 디스
        크의 섹터 크기가 512바이트인지 1024바이트인지 등을 신경 쓰지 않아도 된다는 것이다．
        사용자는 단순히 파일을 열어서 쓰기 명령을 내리면 된다. 그러면 디바이스 드라이버가 자세
        한 세부 내용을 모두 처리하고, 사용자에게는 복잡함과 하드웨어 디바이스를 프로그래밍하는
        어려운 과정을 숨긴다. 그리고 디바이스 드라이버는 다양한 하드웨어 장치에 대해서 하나의
        일관된 인터페이스를 제공한다. 즉, 유명한 UNIX／리눅스 규약에 따라서 모든 것을 하나의
        파일로 다룰 수 있는 기반을 제공하는 것이다．

l) 여기서 모듈（module）이라는 용어와 디바이스 드라이버는 같은 것을 갸긔킨다．


I 252
                                                디바이스 드라이버 기초   Chapter 8




8.1. ] 로드 가능한 모퓰
      리눅스는 다른 일부 운영체제와는 달리 커널 구성 요소를 실행중에 추가하거나 제거할 수 있
      다. 리눅스는 모놀리식 커널로 구성되어 있고, 부팅 후에도 동적으로 디바이스 드라이버 모
      듈을 추가하거나 제거할 수 있도록 잘 설계된 인터페이스를 가지고 있다. 이 기능은 사용자
      에게 유연성을 제공할 뿐만 아니라, 디바이스 드라이버를 개발하는 과정에도 엄청나게 도움
      이 된다. 자신의 디바이스 드라이버가 합리적으로 올바로 동작한다고 가정한다면2) 개발 과
      정에서 코드를 수정할 때마다 매번 커널을 재부팅할 필요 없이 실행중인 커널에 추가하거나
      커널에서 제거할 수 있다．

      로드 가능한 모듈은 임베디드 시스템에서 특히 중요하다 로드 가능 모듈로 인해서 이미 판
      매된 제품을 더 손쉽게 업그레이드할 수 있다. 즉, 시스템을 재부팅할 필요 없이 모듈을 바로
      업데이트할 수 있다. 또한 부팅되고 난 후 나중어］ 로드할 수 있기 때문에 공간상의 문제가
      있는 경우 모듈을 루트（부트） 장치 외의 다른 장치에 저장해 둘 수도 있다．

      물론 디바이스 드라이버를 커널에 정적으로 포함되게 만들 수도 있다. 그리고 실제로 많은
      디바이스들이 동적으로 로드되는 것보다는 커널에 정적으로 포함되는 것이 더 알맞다. 예를
      들어 , 커널이 네트워크를 통해서 NFS 서버에서 루트 파일 시스템을 마운트하도록 구성된
      경우를 생각해 보자. 이 경우에는 네트워크 관련된 드라이버（TCP/ll) 드라이버와 네트워크
      인터페이스 카드 드라이버）가 메인 커널 이미지에 함께 포함되어 컴파일되도록 구성해야 한
      다. 그래야 부팅 중에 원격의 루트 파일 시스템을 마운트할 때 네트워크 장치를 사용할 수
      있다. 물론 6장, "시스템 초기화'에서 설명한 초기 램디스크 기능을 이용해서 커널 본체에
      정적으로 포함시키는 대신에 로드 가능한 모듈로 만들어 사용할 수도 있을 것이다. 이 경우
      에는 초기 램디스크 이미지가 필요한 모듈을 가지고 있어야 하며 , 포함된 스크립트에는 그
      모듈들을 로드하도록 설정해 놓아야 한다．

      로드 가능 모듈은 커널이 부팅된 후에 설치되는데 , 스타트업 스크립트에서 디바이스 드라이
      버 모듈을 로드하도록 할 수도 있고, 모듈을 필요한 시점에 "필요시 로드" 하는 것도 가능하
      다. 커널은 어떤 서비스에서 특정 모듈을 필요로 할 때 그 모듈을 요청할 수 있는 기능을 가
      지고 있다．



2) ［역자주） 올바로 동작하지 않으면 시스템이 멎을 것이다. 이 경우에는 어쩔 수 없이 재부팅해야 한다．
  茹二     Embedded Linux Primer



       커널 모듈에 대해서 이야기할 때 용어를 아직 통일시키지 않은 것 같다 로드 가능한 커널
       모듈에 대해서 이야기할 때 같은 것을 가리키는 여러 용어들이 여전히 혼용되고 있다. 이제
       부터는 디바이스 드라이버（device driver) , 로드 가능한 커널 모듈（LKM : 山ada이e Kernel Module)
       그리고 모듈이라는 각각의 용어들이 모두 ' 로드 가능한 커널 디바이스 드라이버 모듈'을 가리
       킨다고 생각하도록 하자．


8.1.2 디바이스 드라이버 아키텍처
       리눅스의 기본 디바이스 드라이버 모텔은 UNIX／리눅스 시스템 개발자에게는 익숙한 모델
       이다. 물론 디바이스 드라이버 모델은 계속 진화하고 있지만, 일부 기본 구조는 오랜
       UNIX／리눅스 개발 과정에서도 거의 변하지 않았다. 리눅스에서 디바이스 드라이버는 넓은
       의미에서 두 가지로 나눌 수 있다. 캐릭터 디바이스와 블록 디바이스가 그것이다. 캐릭터 디바이
       스는 순차적인 데이터를 직렬 스트림 형식으로 주고받는 장치라고 볼 수 있다. 캐릭터 디바
       이스의 예로는 시리얼 포트나 키보드 등을 들 수 있다. 블록 디바이스는 데이터를 블록 단위
       로 읽거나 쓸 수 있고, 해당 장치의 임의의 위치에 접근할 수 있는 능력을 가지는 장치로 특
       징지을 수 있다. 블록 디바이스의 예로는 하드 드라이브나 플로피 드라이브를 들 수 있다．


8.1.3 최소 디바이스 드라이버 예제

       리눅스에서 디바이스 드라이버 모듈을 동적으로 적재할 수 있기 때문에 , 간단한 디바이스 드
       라이버 예제를 쉽게 실험해 볼 수 있다. ［리스트 &1］에는 로드와 언로드가 가능한 가장 기
       본적인 뼈대만을 가지고 있는 적재 가능한 디바이스 드라이버 모듈을 보여 주고 있다．

       ［리스트 8寸］] 최소 디바이스 드라이버

         ／央 최소 캐릭터 디바이스 드라이버 예제 竹／
         #include <linux/module. h>


          static mnt _init hello_i nit (void)
          {
              printkC'Hello Example Init\n") ;


              return 0;
          }

p254
                                                         디바이스 드라이버 기초   Chapter 8



          static void _exit hello_exit (void)
          {
              printk ("Hello Example Exit\n ') ;
          }


          module_init (hello_init) ;
          module_exit (hello_exit) ;



          MODULE_AUTHOR("Chris Hallinan ') ;
          MODULE_DESCRIPTION( "Hello 닙orld Example") ;
          MODULE_LICENSE ( "GPL") ;




       ［리스트 &1］의 코드는 뼈대만 갖춘 상태지만, 커널에서 드라이버를 로드 및 언로드하는 것
       은 물론이고, 초기화 및 종료 루틴을 호출하는 기본 구조를 모두 갖추고 있다. 이 코드는 디
       바이스 드라이버를 개발하는 더］ 매우 유용한 상위 레벨의 중요한 개념을 이해할 수 있는 좋은
       예제이기 때문에 각각이 어떻게 동작하는지를 살펴보도록 하자. 디바이스 드라이버는 특별한
       종류의 바이너리 모듈이라고 말할 수 있다. 즉, 디바이스 드라이버는 독립형 바이너리 실행
       어플리케이션처럼 명령 프롬프트에서 간단히 실행시킬 수 있는 파일이 아니다. 리눅스 커널
       2.6에서는 이 디바이스 드라이버 바이너리 파일이 "커널 오브젝트' 형식을 갖도록 하고 있다．
       정상적으로 빌드했을 경우 드라이버 바이너리 파일은 . ko로 끝나는 이름3）을 갖게 된다．
       .ko 모듈을 만들기 위한 컴파일러 옵션과 빌드 과정은 약간 복잡할 수도 있다. 여기서는 리
       눅스 커널 빌드 시스템의 힘을 빌어서 세부적인 절차까지 모두 이해하지 않아도 빌드할 수
       있는 방법을 이용할 것이다.


8.1.4 모듈 빌드를 위한 기반
       디바이스 드라이버는 실행될 리눅스에 맞도록 컴파일돼야 한다. 물론 다른 커널 버전을 대상
       으로 빌드된 커널 모듈을 자신의 커널에 로드 및 실행하는 것도 가능하지만, 그 모듈이 새로
       운 버전의 커널에만 있는 기능에 종속적인지 확실하지 않을 경우에는 위험할 수도 있다. 디
       바이스 드라이버를 빌드하는 가장 손쉬운 방법은 커널 소스 트리 내에 포함시켜서 커널과 함
       께 빌드되도록 하는 것이다. 이렇게 하면 개발자가 커널 구성 옵션을 바꿀 때마다 커널 구성

3) （역자주） ko는 커널 오브젝트（kernel obj싸를 줄인 것이다．
?   烈$     Embedded Linux Primer




         에 맞도록 디바이스 드라이버도 자동으로 다시 빌드된다. 물론 커널 소스 트리 밖에서도 빌
         드할 수는 있지만, 그렇게 할 경우에는 드라이버를 사용할 커널과 버전이 일치하도록 빌드
         구성을 맞추는 작업을 스스로 책임져야 한다. 그런 사항으로는 일반적으로 컴파일러 관련 옵
         션이나, 커널 해더 파일의 위치 그리고 구성 옵션 등이 포함된다．

         ［리스트 8-1]에 나온 예제 드라이버를 다음 절차에 따라 수정하면 리눅스 커널 소스 트리에
         서 우리의 예제 드라이버도 같이 빌드하도록 만들 수 있다. 각 단계를 자세히 알아보자．

           1. 리눅스 소스 트리 최상위의 . . . /drivers/char 디렉터리 아래에 examples라는 디
              렉터리를 하나 만든다．

           2. 커널 구성 파일어］ 메뉴 항목을 하나 추가해써 examples 디렉터리도 빌드 대상에 넣는
              다. 그리고 커널에 포함시킬지, 모듈 형식으로 만돌지를 선택할 수 있도록 한다．

           3. 2번 항목의 선택 여부에 따라서 . . . /drivers/char/Nakefile에 examples 디렉
              터리를 새롭게 추가하도록 한다．

           4. example 디렉터리에 대한 makefi노을 만들고, 2번 항목의 선택 여부에 따라서
              hellol. c) 모듈 오브젝트를 컴파일하도록 항목을 추가한다.

           5. 마지막으로 ［리스트 乎1］의 내용을 가지고 드라이버 파일인 hellol. c 소스 파일을 만
              든다．


         . . ./drivers/char 하위 디렉터리 밑에 example 디렉터리를 만드는 이유는 따로 설명할
         필요가 없을 것이다. 이 디렉터리 밑에 두 개의 파일을 만드는데 , ［리스트 8-1]에 있는 모듈
         소스 파일과 examples 디렉터리를 위한 makefile이 그것이다. examples 디렉터리를 위
         한 makefile은 아주 간단하다. 다음과 같은 내용 한 줄이면 된다．

           Obj- $(CONFIG_EXAMPLES) += hellol. o


         커널 구성 유틸리티에 메뉴 아이템을 추가하는 것은 고려할 사항이 좀 더 많다. ［리스트
         8-2］는 현재 버전의 리눅스 . . . /drivers/char/Kconfig 파일에 반영시킬 패치 파일인
         데 , examples를 구성 옵션에서 설정할 수 있도록 하는 메뉴를 추가하는 내용이다. diff/
         patch 형식에 익숙하지 않은 독자도 있을 것이다. ［리스트 &1]에서 각 줄 맨 앞에 + 기호
         하나로 시작하는 것은 (＋기호로 시작하지 않는 부분 사이에） 새롭게 추가된 줄을 나타내는
         것이다．
                                                  디바이스 드라이버 기초   Chapter 8



［리스트 &2] Kconf由 패치 파일

  diff -u /base/1inux-2石.14/drivers/char/Kconflg
  ./dri vers/char/Kconfi g
  戶mm N/base/linux-2. 6.14/drivers/char/Kconfig
  +++ ./drivers/char/Kconfig
  @0 -4, 6 +4,12 @@

   menu "character devices "



   +config EXAMPLES
   +      tristate "Enable Examples "
   +      default M
   +      ---help---
   +      Enable compilation option for driver examples
   +
    config vi
          boo] "vi rtual terminal " if EMBEDDED
          select INPUT



현재 리눅스 커널에 있는 . . . /drivers/ char 디렉터리 아래의 Kconfig 파일에 이 패치
를 적용하면 CONFIG EXAMPLES이라는 새로운 커널 구성 옵션이 추가된다. 4장, "다른 관
점에서 본 리눅스 커널"에서 리눅스 빌드 과정에 대해서 살펴본 내용을 다시 상기해 보면 구
성 유틸리티를 다음과 같은 명령어로 실행시켰었다（ARM 아키텍처를 가정함）.

  $ make ARCH=ARM CR0SS_C0MPILE=xscale_be- gconfig


이와 비슷한 명령어를 이용해서 구성 유틸리티를 실행시켜 보면 Character devices 메뉴
아래에 패치에서 추가한 Enable Examples라는 구성 옵션이 새롭게 추가된 것을 볼 수 있
다. 이 옵션은 3가지 상태를 가질 수 있는데 다음과 같다．

  (N) 사용 안 함. examples 디렉터리를 컴파일하지 않음

  (Y) 사용함． examples 디렉터리를 컴파일하고 최종 커널 이미지에 링크
  (M) 모듈. examples를 동적으로 적재 가능한 모듈로 컴파일




                                                                      257
           Embedded Linux Primer




        ［그림 &1］은 새로운 구성 옵션이 추가된 gconfig 결과 화면이다. 체크 박스 안에 대시 (D
        문자는 (M) odule , 즉 모듈을 선택한다는 의미이다. 이는 오른쪽의 M이라는 항목에도4) 표
        시된다. 체크 박스가 체크되어 있으면 (Y)es , 즉 드라이버가 커널 본체 이미지에 포함시키도
        록 하는 옵션이 선택된 것이다. 체크 박스 안에 아무것도 표시되지 않은 것은 사용하지 않는
        다는 것을 나타낸다．

         Er!甘Qpti아目毖卵

                      隘         다i
                                   昱     I     II   는
           Exck       Load      Save 匡 Singe   S附   Vrd! i Cd!apse Exp카d
         Opt!이肖                                                  Name                 N
           11Nel出가*11好5口pport
           b !SDN subsystem
          卜 Telepti乂）ny Supp｛가t
          卜 Input血吼e sup凶it
          口Character devices
                  口 Ena납！? 已帥pIes                                 EXAM！兀ES
               口 Virtu可 tenrsr日1                                  V丁                  N
               口 N여卜sta岫it! sen可 Pr奴 support                      SERIALNONSTANDARD N
             11Serial drivers
               回 바奴98 PTV sup的C                                   uNI焰｝8_PTYS
             b 回 Leg改y 侶S마 PTVS叩p아t                               LEGACYJ키汗S
                                                                                HC寸朴方뎌 니




                                                                                          三
          Enab注 Examples EXAMPLES

          Enable corit베ationo하拓n 幻rd加er erramples


        I 그림 8너 Example 모듈을 위한 커널 구성 옵션


        지금까지는 examples 디바이스 드라이버 모듈을 컴파일하도록 하는 구성 옵션을 추가했고，
        이제 . . . /drivers/char어］ 있는 11追keffle을 수정해서 , 구성 옵션 CONFIG EX1＼玉IPLES
        가 선택되어 있을 때 커널 빌드 시스템이 새로운 examples 디렉터리도 포함하도록 만들어
        야 한다. ［리스트 &3］은 현재 리눅스에 있는 makefile어］ 적용할 패치 내용이다．

        ［리스트 &3) Examplesl 위한 makefi沌 패치

            th ff -u -/base/1inux-2.6.14/drjvers/char/Makefi1e
            ./dri vers/char/Makef9 1e
            mm= '/ base/1inux-2. 6.14/drivers/char/Makeffle
            +++ ./drivers/char/Makefile
            @@ -88, 6 +88, 7 @@
             obj- $(CONFIG_DRM) += drm/

4) ［역자주） 원문의 그림 예제에는 M 부분이 나오지 않외디. ［그림 &1)의 Name 옆어］ N이 있는데, 그 바로 옆에 M. Y가 있다．


I 258
                                                   디바이스 드라이버 7陸   Chapter 8



   obj- $(CONFIG_PCMCIA) += pcmcia!
   obj -S (CONFIG_IPMI_HANDLER) += I pmi/
  +obj -$ (CONFIG_EXAMPLES) += exampl es/

  Obj- $(CONFIG_HANGCHECK_TIMER) += hangcheck- timer. o




［리스트 ＆읾의 패치는 . . . /drivers/char어］ 있는 makefile어］ (＋로 시작하는） 한 줄을
추가한다. + 문자로 시작하는 줄 외에 몇 줄이 더 있는데 이는 어디에 새로운 내용을 추가하
는지를 결정할 수 있도록 하기 위함이다. makefile 내의 빌드시킬 디렉터리 항목 리스트에
서 , 가장 알맞은 위치로 생각되는 맨 뒤에 새로운 examples 디렉터리를 추가했다. 일관성
과 가독성을 생각하면 이 위치가 가장 알맞을 것이다．

지금까지의 과정을 마치면 커널 빌드 시스템에서 우리의 디바이스 드라이버를 빌드시킬 수
있는 기반은 갖춘 상태가 된다. 이 방식의 좋은 점은 커널이 빌드될 때마다 드라이버도 자동
으로 다시 빌드된다는 점이다. ［리스트 &3］에 있는 구성 옵션이 선택되어 있는한（M 또는
y) , 드라이버 모듈도 빌드 과정에 포함되는 것이다．

ARM 시스템에서 빌드하는 경우라면 명령에 라인에서 모듈을 빌드하는 명령어는 다음과
같다．

  $ make ARCH=arm CROSS_COMPILE=xscale_be- modules

［리스트 &4］는 모듈 개발 과정에서 어느 하나의 모듈을 수정한 후에 위 명령을 실행했을
때 볼 수 있는 결과이다（다른 모듈은 이미 빌드되어 있다）.

［리스트 &4] 모듈 빌드 결과

  $ make ARCH=arm CROSS_COMPILE=xscale_be- modules
    CHK      include/linux/version. h
  make[1] : 'arch/arm/kernel/asm-offsets. s ' is up to date.
  make[1] : 'include/asm- arm/mach- types. h ' is up to date.
    cc EM] drivers/char/examples/hellol.o
    Building modules, stage 2.
    MOD POST
    LD [M] drivers/char/examples/hellol. ko




                                                                        259 1
       U     Embedded Linux Primer




8.1.5 디바이스 드라0뻐 설치하기

       이제 드라이버를 빌드시켰으니 실행중인 커널에 로드하고 언로드해서 동작을 확인해 볼 수
           있다. 모듈을 로드하기 전에 먼저 대상 시스템의 알맞은 위치에 복사할 필요가 있다. 그 위치
       는 어느 곳이어도 상관은 없지만, 편의상 실행중인 리눅스 시스템의 커널 모듈들을 모아 놓
       은 장소에 같이 두는 것이 좋다. 모듈을 컴파일할 때와 마찬가지로 모듈을 설치하는 가장 쉬
       운 방법은 리눅스 커널 빌드 시스템이 알아서 하도록 맡기는 것이다. makefile에 있는 타깃
       인 modules_ins七all을 이용하면 자동으로 모듈을 시스템의 올바른 위치에 모아 두게 된
       다. 그렇기 때문에 간단히 이 기본 경로 아래에 원하는 위치를 지정하면 된다．

       워크스테이션을 위한 표준 리눅스를 설치한 경우에는 디바이스 드라이버 모듈들이
           /lib/ modules/＜커널 버전＞/. .．에 존재하는데 , 리눅스 커널 소스에서 디바이스 드라이버
       디렉터리 구조와 비슷한 구조로 순서대로 위치5）하고 있다. ＜커널 버전＞ 부분은 대상 리눅스
       시스템에서 uname - r 명령을 실행시켜서 생성된 문자열을 이용한다. 만약에 커널 빌드 시
       스템에 설치 관련 문자열을 별도로 주지 않으면 기본 값으로 모듈들은 현재 시스템의
           /lib/ modules/ . . . 디렉터리에 설치된다. 하지만 여기서는 모듈을 다른 곳에 , 즉 현재 대
       상 시스템에 위치시켜야 한다. 그래서 임시 디렉터리 위치를 지정해서 그곳에 모듈이 생성되
       면 나중에 직접 대상 시스템에 복사해서 사용하는 방법도 있다. 그 외에도 대상 임베디드 시
       스템이 현재 워크스테이션의 디렉터리를 이용한 NFS 루트 파일 시스템을 이용하는 경우라
       면 모듈들을 직접 대상 시스템에 설치할 수 있다. 다음 예제가 직접 대상 시스템에 모듈을
       설치하는 경우를 가정한 예제이다．



             $ make ARCH=arm CROSS COMPILE= xsca1e_be                      \
                INSTALL_MOD_PATH=/home/ ch ri s/ sandbox/ coyote- target   \
                modul es i nstal 1




       위 예제는 모든 모듈을 coyo七e-target 디렉터리에 위치시키는데 , 이 디렉터리는 대상 시
       스템에서 NFS를 통해서 루트 파일 시스템으로 마운트6）하는 디렉터리이다．


5) 이 경로는 레드햇과 페도라 배포 버젼에서 사용되는 것이다. 또한 이 경로는 뒤에 뇌 읽어 보기"에 나오는 파일 시스템 계층 표
   준에서도 요구하고 있다. 다른 배포 버젼들은 커널 모듈들을 다른 디렉터리에 모아 둘 수도 있다．
6) 타깃 보드를 위해서 NFS 루트 파일을 마운트시키는 내용은 12장. "임베디드 개발 환경"에서 상세히 디룬다．


 260
                                                  디바이스 드라이버 기초     Chapter 8




8.1.6 모듈 로드하'I
      필요한 모든 과정을 마쳤기 때문에 이제 디바이스 드라이버 모듈을 로드해서 테스트해 볼 수
      있다. ［리스트 8-5］는 임베디드 시스템에 디바이스 드라이버를 로드하고 다시 언로드한 결
      과를 보여 주고 있다．

      ［리스트 &5] 모듈 로드 및 언로드


         Smodprobe heflol             <<< 드라이버를 로드시킴
         Hello Example mnit
         $ modprobe -r hellol         <<< 드라이버를 언로드시킴
         Hello Example Exit
         $



      위에서 출력되는 내용과 ［리스트 &1］의 디바이스 드라이버 소스 코드와의 관계를 이해할
      수 있어야 한다. 모듈은 printk () 를 통해서 커널 로그 시스템에 메시지를 출력하는 일만
      하고, 이 메시지를 콘솔7）에서 볼 수 있는 것이다. 모듈이 로드되면 모듈 초기화 함수가 호출
      되는데 , module mni七（) 매크로를 이용해서 모듈이 삽입될 때 실행시킬 초기화 함수를 지
      정하게 된다. 이 매크로는 다음과 같이 사용한다．

         module_init (hello_init) ;


      여기서 작성한 초기화 함수에서는, 단순히 의무적인 인사 메시지（hello）를 출력하고 반환하
      도록 되어 있다. 하지만 실제 디바이스 드라이버에서는 초기 자원 할당 및 하드웨어 장치의
      초기화 등을 수행할 것이다. 비슷한 형태로 모듈을 (modprobe -r 명령을 이용해서） 언로드
      하는 경우에는 모듈 내의 종료（exit) 함수가 호출된다．

      ［리스트 &1]에서 보듯이 종료 함수는 module exi七 ( ) 매크로를 이용해서 설정하게 된다．

      여기까지는 기본 뼈대만 갖춘 디바이스 드라이버를 실제 커널에 삽입하는 부분을 설명했다．
      이어지는 섹션에서는 적재 가능한 디바이스 드라이버 모듈을 위한 추가적인 기능을 알아보
      고, 사용자 영역에서 실행되는 몇 가지 유틸리티 프로그램을 이용해서 어떻게 디바이스 드라
      이버 모듈을 다루는지 예를 통해서 알아보도록 하자．

7) 콘剖1 메시지가 나오지 않는다면 syslogd 로거가 꺼져 있거나 콘솔 로그 단계가 낮기 때문이다. 이 부분은 14장, "커널 디버깅
 기술”어Ha 설명한다．


                                                                         261 1
 瑟 仄1     Embedded Linux Primer




8.2 모듈 유틸리El
        모듈 유틸리티에 대해서는 ［리스트 &5］에서 잠깐 살펴봤었다. 거기에서 리눅스 커널에 디
        바이스 드라이버를 추가하거나 제거하는 데 modprobe라는 모듈 유틸리티를 이용했다. 디
        바이스 드라이버 모듈을 관리하기 위해서 이 외에도 몇 가지 유틸리티가 더 이용되는데, 이
        섹션에서는 이 유틸리티들에 대해서 살펴보자. 여기서 소캐하는 모든 유틸리티에 대한 완전
        한 내용은 man 페이지를 참고하기 바란다. 사실 리눅스의 로딩 가능한 모듈들에 대해서 더
        깊이 알고자 한다면 이들 유틸리티의 소스 코드 내부를 살펴보는 것이 더 좋을 것이다. 이
        장의 맨 마지막 부분에 있는 8.6.1절 "더 읽어 보기"에서 참고할 만한 자료를 찾아볼 수 있다.



8.2.1 insmod
        in町nod는 가장 간단하게 리눅스에 모듈을 올릴 수 있도록 해 주는 유틸리티이다. 올리고자
        하는 파일의 경로를 입력하면 커널에 바로 올리게 된다. 예를 들면 다음과 같다．



          $ insmod /lib/ modules/ 2.6.14/ kernel/dr-ivers/ char/examples/hellol. ko



        이 명령은 hellol.k配｝는 모듈을 커널에 로드한다. 실행 결과는 ［리스트 &5］에서 본 것
        과 같은 내용, 즉 Hello 메시지이다. insmod 유틸리티는 별도의 옵션을 필요로 하지 않고
        받치도 않는 간단한 프로그램이다. 단 하나의 인자로 완전한 경로8）를 받는데 , 이는 모듈을
        찾기 위한 기능이 따로 없기 때문이다. 그래서 보통은 곧 설명할 유틸리티인 modprobe를
        사용하는데 , 더 다양한 기능과 특징을 가지고 있기 때문이다．


8.2.2 모듈 파라미터
        많은 디바이스 드라이버가 내부적인 동작을 변경하기 위해서 파라미터를 이용한다. 예를 들
        어 , 디버그 모드를 활성화시킨다거나, 다양한 리포팅 정보를 계속 출력하게 하거나, 모듈을
        위한 특별한 옵션을 지정하는 데 파라미터가 사용된다. insmod 유틸리티를 이용해서도 모

8) （역자주） 완젼한 경로的l 附h) : 파일의 절대 경로를 말한다. 최상위 디렉터리부터 모든 디렉터리 경로를 표시한 것이다. 예를
   들어， /usr/home/fromdj/chapter3. 柶叩와 같은 식이다．


I 262
                                                  디바이스 드라이버 기초      Chapter 8




듈 이름 뒤에 내용을 입력함으로써 파라미터（어떻게 보면 옵션이라고 할 수도 있다）를 전달
할 수 있다. ［리스트 8-6］은 예제 hellol.c를 수정한 것인데 , 파라미터를 하나 받아서 디
버그 모드를 활성화시키는 데 이용한다．

［리스트 &6) 파라미터를 이용한 드라이버의 oil

  ／士 최소 캐릭터 디바이스 드라이버 예제 '7
  #include <linux/module. h>
  static mnt debug中enable = 0;      ／肯 추가된 드라이버 파라미터 六／
  module_param (debug_enable, int, 0) ; /'" 아래 두 줄도 추7띰 肯／
  MODULE_PARM_DESC (debugmenable, "Enable module debug mode. ") ;

  static mnt _init hello_init (void)
  {
       ／六 이제 새로운 모듈 파라미터의 값을 출력함 肯／
       printk ("Hello Example mnit - debug mode is %s\n",
               debug_enable? "enabled" : "disabled")

       return 0;
   }

   static void __exit hello_exit (void)
   {
       printk ("Hello Example Exit\n") ;
   }

   module_init (hello_init) ;
   module_exit (hello_exit) ;

   MODtJLE_AUTHOR("Chris Hallinan") ;
   MODULE_DESCRIPTION("Hello world Example") ;
   MODULE_LICENSE("GPL") ;



예제 디바이스 드라이버에 세 줄이 추가되었는데 , 첫째는 정적（static) 변수 하나를 디버그 상
태인지를나타내기 위해서 정의했다. 두번째 줄은 . . . /include/linux/modulepararn.h
에 정의되어 있는 매크로인데 , 커널 모듈 시스템에 모듈 파라미터를 등록하는 일을 한다. 세
번째 줄은 커널 모듈 시스템에서 이 새로운 파라미터에 맞는 설명 문자열을 등록한다. 이렇
게 하는 까닭은 나중에 다룰 modinfo를 설명할 때 좀 더 명확하게 이해할 수 있을 것이다．
           Embedded Linux Primer




        작성한 예제 모듈을 커널에 삽입하기 위해서 insmod를 사용한다면 뒤에 debug enable을
        추가하도록 하자. 그러면 ［리스트 &6］에서 hellol . C 모듈의 경우와 비슷한 결과를 볼 수
        있다．



           $ insmod /lib/ modules/ . . ./examples/hellol. ko debug_enable=1
              Hello Example mnit - debug mode is enabled



         또는 파라미터를 생략한 경우는 다음과 같은 결과를 볼 수 있다．



           $ insmod /lib/ modules/ . . ./examples/hellol.ko
              Hello Example mnit - debug mode is disabled




8.2,3 Ismod
       ismod 역시 아주 간단한 유틸리티이다. 이 유틸리티는 단순히 현재 커널에 삽입되어 있는
       모듈의 목록을 형식에 맞게 출력한다. 최신 버전의 ismod는 아무런 파라미티를 받지 않고，
       단순히 加roc/modu1es9）의 내용을 형식에 맞게 출력한다. ［리스트 ＆끼은 ismod의 출력
       예제를 나타낸 것이다．

       ［리스트 &7) Ismod의 실행 결과 예제

          $ lsmod
          Module                    Size Used by
          ext3                     121096 0
           jbd                      49656 1 ext3
          loop                      12712 0
          hellol                     1412 0
          $




9) /proci뇨odu!明는 pr乂 파일 시스템의 일부이다. 9장， "파일 시스템"에서 소개할 것이다．
                                         디바이스 드라이버 기초   Chapter 8



     맨 오른쪽 항목 Used by를 보자. 이 항목은 모듈 디바이스 드라이버가 사용되고 있는 횟수
    및 종속성에 관련된 내용을 보여 준다. 이 예제에서는 jbd 모듈（저널링 파일 시스템을 위한
     저널링 루틴）이 많은 리눅스 배포판에서 기본 저널링 파일 시스템으로 사용되는 e>＜七3 모듈
     에 의해서 사용되는 것을 볼 수 있다. 이는 e就3 디바이스 드라이버가 jbd 모듈이 존재하는
    지 여부에 종속되어 있다는 것을 나타낸다．


8.2.4 modprobe
     이제 modprobe 유틸리티의 똑똑한 기능을 사용할 차례이다. ［리스트 8-끼을 통해서 ext3
     과 加d 모듈의 상호 관계에 대해서 알고 있다. modprobe는 이러한 관계를 찾아내서 종속된
     순서에 맞게 모듈들을 올리는 기능을 가지고 있다. 그래서 다음 명령어는 jbd. ko와 e>＜七3.
     ko 드라이버 모듈 두 가지를 모두 로드한다．

       $ modprobe ext3


     이 modprobe 유틸리티는 동작을 결정하는 몇 가지 옵션을 가지고 있다. 앞에서 살펴본 것
     처럼 modprobe는 모듈을 제거하는 데도 사용할 수 있고, 종속된 관계까지 포함하써 제거할
     수도 있다. 다음은 jbd. ko와 cx七3. ko 모듈 모두를 제거하는 명령이다．

       $ modprobe -r ext3


     modprobe 유틸리티는 mobprobe . conf라는 구성 파일에 의해서 동작이 결정된다. 이는
     시스템 개발자가 장치와 디바이스 드라이버를 서로 연결할 수 있도록 해 준다. 간단한 임베
     디드 시스템의 경우에는 modprobe . conf 파일은 비어 있거나 몇 줄 정도의 내용만 가지고
     있을 것이다. modprobe 유틸리티는 올바른 modpr야氾 . conf 파일이 존재하지 않을 때 사
     용하기 위한 기본 값을 포함해서 컴파일되어 있다. mobprobe 유틸리티를 -c 옵션만 주고
     실행시키면 modprobe에서 사용되는 기본 설정을 볼 수 있다．

    ［리스트 &8J은 시스템에 두 개의 이더넷 인터페이스를 가치고 있는 경우에 볼 수 있는 전형
     적인 modprobe . conf를 나타낸 것인데 , 하나는 프리즘2(Pris毗） 칩셋에 기반한 무선 네
     트워크 어댑터이고, 나머지 하나는 일반 PCI 이더넷 카드이다．
  難聲     Embedded Linux Primer



       ［리스트 &8] 전혐적인 modprobe.conf 파일

         $ cat /etc/modprobe.conf
         alias ethi orinoci_pci
         options ethi orinoco_debug=9
         alias ethO eiOO
         alias snd-card-O snd-intel8xO
         options snd-card-O index=O
         $



       커널이 부팅하다가 무선 칩셋을 발견하면 이 구성 파일을 이용해서 modprobe가 orinoco
       pci 디바이스 드라이버를 로드해서 커널 장치 e七hi로 연결시킨다. 그리고 추가적으로
       orinOOO debug=9라는 파라미터를 디바이스 드라이버에 전달한다. 사운드 카드 장치를
       발견했을 때도 이와 비슷한 작업이 이루어진다. snd-inte18x0 사운드 드라이버에 전달하
       는 추가 파라미터도 한번 유심히 보기 바란다．


8.2.5 depmod
       그렇다면 modpr야光는 어떻게 주어진 모듈의 종속성을 알아낼 수 있을까2 여기에는
       depmod라는 유틸리티가 주된 역할을 수행한다. modprobe가 실행되면 해당 모듈이 설치된
       위치에서 modules. dep라는 파일을 찾는데 , de미nod 유틸리티가 바로 modules. dep 파
       일을 생성하는 일을 한다．

       이 파일은 커널 빌드 시스템에서 설정된 모든 모듈의 목록을 가지고 있고, 그와 함께 각각의
       종속성 관련 정보도 가치고 있다. 파일의 형식은 아주 간단하다. 각 디바이스 드라이버 모듈이
       한 줄찍을 차지하고, 만약에 그 모듈이 종속성을 가지고 있다면 모듈 이름 튀에 순서대로 종속
       된 모듈 이름들이 나열된다. 예를 들어 , ［리스트 &7］에서처럼 ext3 모듈이 그bd 모듈에 종
       속성을 가치고 있는 경우라면 modules. dep의 내용은 다음과 같은 형태를 가질 것이다．

          ext3.ko: jbd. ko


       실제적으로는 모호함을 없애기 위해서 각 모듈 이름 앞에 파일 시스템의 절대 경로 주소가
       붙게 되지만, 여기서는 가독성을 위해서 경로 정보를 생략했다는 것을 알아두기 바란다. 사
       운드 드라이버와 같이 좀 더 복잡한 종속성을 가진 경우는 다음과 같은 모습을 볼 수 있다．



p266
                                                         디바이스 드라이버 기초      Chapter 8




         snd-inte18x0.ko: snd-ac97-codec. ko snd-pcm. ko snd- timer.ko \
           snd. ko soundcore. ko snd-page-alloc.ko



    앞에 나오는 파일 경로는 가독성을 위해서 생략했다. modules . de1) 파일어］ 있는 모듈 파일
    명은 모두 절대 경로를 포함하고 있으며 , 또한 한 줄에 전부 존재하게 된다. 위 예제는 공간
    상 두 줄로 표현했지만 실제 파일에는 한 줄로 되어 있다．

    일반적으로 depmod는 커널이 빌드될 때 자동으로 실행된다. 하지만, 교차H개발 환경의 경
    우는 자신이 사용하는 대상 아키텍처에 맞게 컴파일된 모듈에 대한 정보를 읽어낼 수 있는
    교차e버전의 depmod를 가지고 있어야 한다. 그 외에도 대부분의 임베디드 배포 버전에는
    매 부팅 시마다 depmod를 실행시킬 수 있도록 mnit 스크립트 항목이나, 메서드들을 가지
    고 있어서 모듈 간 종속성을 항상 최신으로 유지할 수 있도록 해 준다．


8.2.6 rmmod
    이 유틸리티 역시 아주 간단하다. 단순히 현재 커널에서 모듈을 제거하는 일을 하며 , 파라미
    터로는 모듈 이름을 넣으면 된다. 절대 경로를 모두 적을 필요는 없다. 예를 들면 다음과 같
    다．
         $ rmmod hellol
            Hello Example Exit



    여기서 이해할 가장 중요한 사항은 바로 rmmod를 이용하면 ［리스트 8-1］과 ［리스트 斗6]
    의 hellol . c에서 볼 수 있는 hello exi七 () 와 같은, 모듈의 女 exit () 함수가 호출된다
    는 것이다．

    그리고 또 한 가지 알아 둘 점은 modprobe와는 달리 rmmod는 종속된 모듈은 제거하지
    않는다는 것이다. 종속된 모듈까지 모두 제거하기 위해서는 modprobe -r을 이용하자．




                                                                                 267
   N    Embedded Linux Primer




8.2.7 modin化
       기본 드라이버 코드인 ［리스트 &1］과 나중의 ［리스트 &6］에 있는 마지막 세 줄을 기억할
    것이다. 이 매크로들은 모듈을 관리 및 유지하는 데 사용하기 위한 청보를 바이너리 파일에
       포함시키기 위한 것이다. ［리스트 ＆이는 hellol. ko 모듈에 대해서 modinfo 명령을 실행
    시킨 결과이다．

    ［리스트 &9] modinfo 출력


         $ modinfo hellol
         filename:      /lib/ modules/ . . ./char/ examples/hellol. ko
         author:       Chris Hallinan
         description:   Hello world Example
         license:      GPL
         vermagi C:     2. 6. 14 ARMv5 gcc- 3. 3
         depends:
         parm:         debug_enable: Enable module debug mode. (int)
         $




       첫 번째 내용은 디바이스 드라이버 모듈의 절대 경로를 나타낸다. 그리고 역시 여기서도 가
       독성을 위해서 경로를 일부 생략했다. 그 다음 내용은 ［리스트 8-臼의 맨 마지막 부분에서
       찾아볼 수 있는 파일명 , 작성자, 라이선스 정보이다. 하치만 이 내용들은 모듈 유틸리티에
       의해서 사용되며 , 디바이스 드라이버 자체의 동작에는 영향을 미치지 않는 내용들이다. man
       페이지에서 modin凡에 대해서 좀 더 자세한 설명을 볼 수 있고, modinfo 소스 코드를 참고
       해도 좋은 정보를 얻을 수 있을 것이다．

       modin白의 매우 유용한 기능 중의 하나는 모듈이 지원하는 파라미터 정보도 얻을 수 있다는
       것이다. ［리스트 ＆이를 보면 이 모듈이 단 하나의 파라미터만을 지원하는 것을 알 수 있다．
       이 파라미터는 ［리스트 8-6］에서 추가한 debug enable이다. modinfo의 출력 내용에서
       는 파라미터의 이름과 데이터 타입（여기서는 in七） 그리고 MODUI皿 FARM DESC () 매크로
       를 이용해 입력한 설명 문자열이 표시된다. 이 기능은 해당 드라이버의 소스 코드에 첩근할
       수 없는 경우에 유용하게 사용될 수 있다.
                                                     디바이스 드라이버 가초      Chapter 8




8.3 드라이버의 메서드
       지금까지 몇 가지 모듈 유틸리티를 사용하는 방법에 대해서 기초적인 부분을 살펴봤고, 이
       장의 나머지 부분에서는 디바이스 드라이버와 사용자 영역에서 실행되는 프로그램（독자가
       작성한 어플리케이션 코드）이 어떻게 서로 통신하는지 그 기본 메커니즘을 알아보겠다．

       이미 모듈의 초기화 및 종료 과정을 처리하는 두 개의 기본적인 메서드에 대해서는 살펴본
       적이 있다. ［리스트 &1］을 다시 보면 module i nit (）과 module exi七（) 함수가 바로
       그것이다. 이 함수들은 각각 실행중인 커널에 삽입될 때와 제거될 때 한 번씩 실행된다는 것
       은 이미 알고 있을 것이다. 이제 우리가 작성한 어플리케이션 프로그램에서 디바이스 드라이
       버와 인터페이스하는 데 필요한 메서드들을 알아야 한다. 결국 디바이스 드라이버를 이용하
       는 가장 큰 두 가지 이유 중 하나는 사용자가 커널 영역에서 실행시킬 위험한 코드를 작성하
       지 않도록 커널 영역을 격리시키는 것이고, 또 하나는 하드웨어 또는 커널 내 디바이스들과
       통신하는 통합된 통신 방식을 제공하기 위해서이다.


8.3. ] 드라이버의 파일 시스템 오퍼레이션

       디바이스 드라이버가 실행중인 커널에 로드되고 제일 먼저 해야 할 작업은 드라이버의 추가
       적인 오퍼레이션을 사용할 수 있도록 만드는 것이다. 이를 위해서 open () 메서드를 이용한
       다. 드라이버를 연 후에는 드라이버에서 데이터를 읽거나 쓰기 위한 함수가 필요하다. 그리
       고 사용을 모두 마친 후에는 （기본적으로 사용자 영역에서 close를 호출하면） 청소 작업을
       위한 메서드로 release () 가 사용된다. 마지막으로 드라이버를 표준 접근 외10）의 방식으
       로 접근할 수 있도록 해 주는 특수한 시스템 콜을 지원하기 위해서 1OO七l () 이 사용된다.
      ［리스트 8-10］은 우리의 기본 디바이스 드라이버에 방금 소개한 기초 오퍼레이션들을 추가




10) （역자주） 표준 접근이란 read人vrite를 통해서 작업하는 것을 밀한다. 하지만 read나 write를 이용하는 것이 드라이버의 특성에
    맞지 않을 수 있는더1 이를 위해서 k乂ti을 이용한다．


                                                                            269 1
        Embedded Linux Primer



      ［리스트 &10) Hello. c에 파일 시스템 오퍼레이션 추가하기


        #include <linux/module. h>
        #include <linux/ fs.h>



        #define HELLO_MAJOR 234



        static mnt debug_enable = 0;
        module_param(debug_enable, int, 0) ;
        MODULE_PARM_DESC(debug_enable, "Enable module debug mode. ") ;



        struct file_operations hello_fops;



        static mnt hello_open(struct mnode *inode, struct file *file)
        {

             printk ("hello_open: successful\n") ;
             return 0;
        }


        static -mnt hello_release(struct mnode *inode, struct file 士 file)
        {

             pri ntk("hello_rel ease: successful\n") ;
             return 0;
        }


        static ssize_t hello_read(struct file *file, char *buf, 引ze_t count,
                      loff_t *ptr)
        {

             printk("hello_read: returning zero bytes\n") ;
             return 0;
        }


        static ssize_t hello_write(struct file *fjle! const char *buf,


270
                                                다바이스 드라이버 기초       Chapter 8



                size_t count, loff_t * ppos)
{

    printk ("hello_read: accepting zero bytes\n") ;
    return 0;
}


static mnt hello_ioctl (struct mnode *inode, struct file *fjle,
             unsigned mnt cmd, unsigned long arg)
{
    printk ("hello_ioctl: cmd=%ld, arg=%ld\n", cmd, arg) ;
    return 0;
}


static mnt _init    hello_init (void)
{
    m nt ret;
    pri ntk("Hello Example mnit 寸 debug mode is %s\n",
            debug_enable? "enabled" : "disabled") ;
    ret = register_chrdev (HELL0_MAJoR, "hellol", &hello_fops) ;
        if (ret < 0) {
            printk ("Error registering hello device\n") ;
            goto hello_faill;
       }
    printk ("Hello: registered module successfully! \n") ;



    ／六 In卄 마oces引ng here. . . 士／



    return 0;



hello_faill:
    return ret;
}


static void _exit hello_exit (void)
{


                                                                        271 i
       熬    Embedded Linux Primer



                  printkC'Hello Example Exit\n") ;
             }


             St ru Ct 터］e_opera너애s hello_ fops   =   {
                 owner:    THIS_MODULE,
                  read:    hello_read,
                 write:    hello_write,
                  ioctl :  hello_ioctl ,
                 open:     hello_open,
                  release: hello_ release,
             };


             mo（加］ e in仕 (hel ] 0_in卄）·，
             module_exit (hello_exit) ·，



             MODULE_AUTHOR ( "Chris Hallinan") ;
             MODULE_DESCRIPTION("Hello world Example ") ;
             MODULE_LICENSE( "GPL ") ;




           이 확장된 디바이스 드라이버에는 새롭게 추가된 내용이 많은데 , 먼저 제일 위에는 파일 시
           스템 오퍼레이션에 대해서 정의된 내용을 참조하기 위해서 커널 헤더 파일을 하나 더 추가했
       다. 그리고 작성한 디바이스 드라이버에 주 버전（n녜or number）을 정의했다（디바이스 드
           라이버 개발자가 주의할 점은 여기서 주 버전을 정의하는 데 사용한 방법은 적절한 방법이
       아니라는 것이다. 올바른 방법에 대해서는 리눅스 커널 문서（. . . /Documentation/
           devices .txt) 또는 디바이스 드라이버에서 주 버전 넘버를 할당하는 방법을 다루고 있는
           좋은 책들을 참고하기 바란다. 위 예제에서는 단순히 현재 시스템에서 사용하지 않는 번호



       다음으로 open, close, read, write 네 개의 메서드 청의를 새롭게 추가했다. 올바른 코딩
           방식을 지키기 위해서 , 커널 내의 다른 서브시스템과 충돌하지 않도록 일관된 방식으로 함수
       이름을 정의했다. 그래서 함수 이름이 각각 hello openO, hello releaseQ,
       hello readQ, hello wri七e (）이다. 그리고 이 각각의 함수들은 예제를 간단히 하기
           위해서 단순히 문자열을 커널 로그 시스템에 출력하는 것 외에 아무 일도 하지 않는다.



1272
                                                           디바이스 드라이버 기초   Chapter 8




      그리고 hello init () 내부에 다른 함수를 호출하는 구문이 새롭게 추가되었다. 이 코드가
      하는 일은 우리가 작성한 디바이스 드라이버를 커널에 등록하는 것이다. 등록 함수를 호출
      할 때 필요한 메서드들에 대한 포인터 주소를 가지고 있는 구조체를 전달하는데 , 커널은
       struct file operations 타입의 이 구조체를 이용해서 파일 시스템 접근을 우리가 작
      성한 디바이스 함수에 알맞게 연결시키게 된다. 그래서 어플리케이션에서 우리가 작성한 디
      바이스 드라이버를 가리키는 장치 파일을 열어서 이 파일에 대해서 read를 요청하면 파일
      시스템은 일반 read() 요청을 우리 모듈의 hello read() 함수와 연결시켜 주는 것이다.
      다음 절에서 이 과정을 자세히 살펴보도록 하자．


8.3.2 디바이스 노드와 mknod

      어떻게 어플리케이션의 요청을 우리의 디바이스 드라이버를 나타내는 장치로 보낼 수 있는지
      이해하기 위해서는, 디바이스 노드라는 개념을 반드시 이해해야 한다. 디바이스 노드는 리눅
      스에서 디바이스를 나타내는 특수한 파일 형식이다, 실제로 모든 리눅스 배포 버전이（파일
      시스템 계층 표준11）어］ 정의된） /dev라는 같은 위치에 디바이스 노드들을 모아둔다. 파일
      시스템에 디바이스 노드를 만들기 위해서는 mknod라는 전용 유틸리티를 이용한다．

      실제 노드를 한번 만들어 보는 게 내용을 이해하는 데 가장 좋은 방법일 것이다. 다음과 같이
      디바이스 드라이버의 내용에 맞도록 연습용 디바이스 노드를 하나 만들어 보도록 하자．

          $ mknod /dev/hellol C 234 0


      타깃 임베디드 시스템에서 이 명령을 실행시키면 새로운 파일인 /dev/hellol이 만들어지
      는데 , 이 파일이 우리가 작성한 디바이스 드라이버 모듈을 나타낸다. 콘솔에서 파일 목록을
      나열해 보면 다음과 같은 결과를 볼 수 있다．



          $ is -i /dev/heliol
         crw-r- -r- -   1 root   root   234, 0 Jul 14 2005 /dev/hellol




11) 이 장의 마지막에 있는 노기 읽어 보기"에서 챰고 자료를 찾을 수 있다．


                                                                               273 1
  Ru      Embedded Linux Primer




        mknod에 전달하는 인자로는 파일 이름, 형식 그리고 디바이스 드라이버의 주 버전과 보조
        버전（n血or version）이 있다. 여기서 파일 이름은 당연히 hellol이다. 그리고 작성한 디
        바이스 드라이버는 캐릭터 디바이스이기 때문에 이를 의미하는 C를 인자로 넣어 준다. 주
        버천은 예제를 위해서 선택한 숫자 234이고, 보조 버전은 0으로 설정했다．

        디바이스 노드는 그 자체가 파일 시스템에 존재하는 하나의 파일이다. 하지만, 디바이스 노
        드라는 특수한 상태를 갖기 때문에 설치된 디바이스 드라이버와 연결하는 데 사용하는 것이
        다. 어플리케이션 프로세스가 우리 디바이스 노드를 파일로 open () 하는 시스템 콜을 호출
        하면 커널은 일치하는 디바이스 노드에 등록된 주 버천（이 경우는 234）에 디바이스 드라이
        버를 검색하게 된다. 이것이 커널이 특정 디바이스를 디바이스 노드에 연결시키는 데 사용하
        는 방식이다．

        C 프로그래머라면 대부분 어플리케이션에서 파일 시스템 동작, 즉 읽기 , 쓰기 , 닫기 등의 명
        령을 내릴 수 있는 참조값（또는 file descriptor : 파일 기술자）을 반환해 주는 open ( ) 시
        스템 콜 또는 같은 일을 하는 다른 형태의 함수를 이미 알고 있다. open을 통해서 반환된
        참조자는 읽기 , 쓰기 등의 함수를 호출할 때 인자로 전딜하게 된다．

        보조 버전에 대해서 궁금한 독자를 위해서 설명하자면 보조 버전은 하나의 디바이스 드라이
        버를 이용해서 여러 장치를 처리하거나, 여러 하위 장치를 처리할 때 이용되는 메커니즘이
        다. 이 숫자는 운영체제에서는 사용되지 않고, 그냥 디바이스 드라이버에 전달해 준다. 디바
        이스 드라이버가 보조 버전을 자신에 맞게 이용하는 것이다. 예를 들어 , 여러 개의 포트를
        가진 직렬 카드가 있다면 주 버전은 디바이스 드라이버를 가리키고, 보조 버전이 같은 디바
        이스 드라이버에서 처리되는 여러 개의 포트 각각을 의미하도록 할 수 있다. 관심 있는 독자
        는 좀 더 자세한 내용을 위해서 관련 문서들을 참고하기 바란다.



8.4 한데 묶기
        이제 커널에 로드하고 테스트해 볼 수 있는 기본 뼈대를 갖춘 디바이스 드라이버를 확보했다．
        ［리스트 &11］은 작성한 디바이스 드라이버를 테스트해 볼 수 있는 간단한 사용자 영역 어
        플리케이션이다. 디바이스드라이버를 어떻께 로드하는지는 이미 살펴봤다. 즉, 전에 설명한
        것처럼 단순히 컴파일한 후에 make modules+ins七all 명령을 주어서 파일 시스템에 위치
        하도록 하면 된다．


I 274
                                                     디바이스 드라이버 기초   Chapter 8



［리스트 8-11] 디바이스 드라이버 테스트하기

  #include <stdio. h>
  #include <stdlib.h>
  #include <sys/types. h>
  #include <sys/stat.h>
  #i nd] ude <fcntl . h>
  #include <unistd. h>



  mnt main(int argc, char **argv)
  {
      ／卉 Our 꺼］e descriptor 山"/
      mnt fd;
      mnt rc = 0;
      char 受rdebuf [16] ;



      printf ( "%s: entered\n", argv[O] );



      ／央 Open the device 士／
      fd = 야）en("/dev/hellol" , 야RD脈）·，
      if ( fd == -1 ) {
         perror ("open failed") ;
          rc = fd;
         exit(-1) ;
      }
      printf ("%s: open: successful\n", argv[O] );

      ／山" Issue a read 肖／
      rc = read(fd, rd_buf, 0) ;
      if ( rc == -1 ) {
           perror ("read failed") ;
           close(fd) ;
           exit (-1) ;
      }
      printf ("%s: read: returning %d bytes! \n", argv[0] , rc) ;

      close(fd) ;
      return 0;
  }


                                                                         275 1
           Embedded Linux Primer




        ARM 엑스스케일 시스템에서 컴파일한 이 짧은 코드를 통해서 어플리케이션과 디바이스 드
        라이버가 디바이스 노드를 통해서 서로 연결되는 것을 볼 수 있다. 실제 디바이스 드라이버
        처럼 실질적인 일은 하지 않지만 ［리스트 8-10］의 디바이스 드라이버에서 설명한 여러 메서
        드들을 사용하는 것에 대한 개념을 보여줄 수는 있다．

        가장 먼저 이전에 생성한 디바이스 노드를 open () 시스템 콜12）을 이용해서 연다. 만약에
        open이 성공할 경우에는 콘솔에 성공적으로 열었다는 메시지를 보여 준다. 다음에는
        read () 명령을호출하는데 , 역시 성공할경우성공했다는메시지를콘솔에 보여 준다. 여기
        서 0바이트를 읽도록 호출하는 것은 커널 입장에서는 아무 문제가 없다. 0바이트는 파일의
        끝（EOF : end of file）을 만나거나 데이터가 더 이상 없는 상태를 나타낸다. 우리가 작성한
        디바이스 드라이버는 바로 이 특수한 상태에 있는 것이다. read 작업 뒤에는 파일을 닫고
        프로그램을 종료하게 된다. ［리스트 &12］에는 이 예제 프로그램을 ARM 엑스스케일 타깃
        머신에서 동작시킨 결과를 나타낸 것이다．

       ［리스트 &12] 예제 드라이버 이용하71


           $ modprobe hellol
           Hello Example mnit - debug mode is disabled
           Hello: registered module successfully!
           $ ./use-hello
           ./use-hello: entered
           ./use-hello: open: successful
           ./use- hello: read: returning zero bytes!
           $




8.5 디바이스 드라이버와 GPL
       디바이스 드라이버에 관련해서는 디바이스 드라이버에 적용되는 GNU 공공 라이선스 조건
       을 둘러싸고 많은 논의와 논쟁이 진행되고 있다. 만약에 독자가 작성한 디바이스 드라이버
       （또는 어떤 소프트웨어든）가 기존에 존재하는 GPL 소프트웨어 또는 그 일부에 기반하고 있
       다면 이 소프트웨어를 수정판（de巾ed work)'3）이라고 부른다. 예를 들어 , 독자가 현재 리눅스


12) 실제로 open ( ) 함수는 C 라이브러리 랩퍼 (\＼丁a텍羌r) 함수이고, 이 랩퍼 함수가 sys open ( ) 이라는 시스템 콜 함수를 호출하
  도록 되어 있다．


t276
                                                 디바이스 드라이버 가초      Chapter 8




         디바이스 드라이버를 가지고 자신에게 맞게 일부 수정한 경우 이를 수정판이라고 볼 수 있다．
         그리고 이 경우 수정된 디바이스 드라이버는 의무적으로 GPL 규정에 따라 라이선스해야 하
         고, 라이선스의 모든 요구 조건도 준수해야 한다．

         먼저 말해둘 것이 있다. 지금 설명하는 내용은 법적인 의견이 아니라는 점이고, 필자의 직업
         도 변호사가 아니라는 것이다. 일부 내용은 이 글을 쓸 당시 법정에서 아직 확인되지 않은
         것들이다. 법적으로나 오픈 소스 공동체나 모두가 갖는 지배적인 의견은 어떤 작업 결과물이
        독립적으로 만들어진 것을 증명14）할 수 있는 경우 그 작업물은 리눅스 커널의 "내부 지식
         (intimate knowledge)"이라고 볼 수 없고 그래서 개발자는 자기가 원하는 어떤 라이선스
        든 자유롭게 선택할 수 있는 것이다. 하지만 만약에 드라이버의 특수한 조건을 만족시키기
        위해서 커널을 수정하는 경우에는 수정판이라고 볼 수 있기 때문에 GPL을 준수해야 한다．

        이 문제와 관련해서는 오픈 소스 공동체에서 많은 정보를 찾을 수 있다. 그리고 그 시점이
        언제가 될지는 아무도 모르지만, 미래의 언젠가는 이런 사항이 실제 법정에서 논의되고, 이
        에 대한 판례도 만들어질 것이다. 만약 리눅스와 오픈 소스를 둘러싼 법적 사항들을 좀 더
        자세히 알고 싶으면 www.open-bar. org를 둘러보기 바란다．



8.6 요약
        이 장에서는 디바이스 드라이버의 기본에 대해서 상위 레벨에서 검토해 보았고, 리눅스 시스
        템 아키텍처와 어떻게 맞물려 돌아가는지 설명했다. 이 기본 지식을 이용하면 드라이버 개발
        을 처음 접하는 독자도 디바이스 드라이버 개발을 다루는 다른 좋은 책을 공부해 나가는 데
        도움이 될 것이다. 8.6.1절의 참고 자료를 보기 바란다．

           口 디바이스 드라이버는 하드웨어나 기타 장치와 같은 중요한 커널 자원과 사용자 어플리케
              이션 간을 합리적으로 분리할 수 있도록 해 준다. 또한 어플리케이션이 자원에 접근하는
              데 익숙한 통합 인터페이스均를 이용할 수 있도록 해1 준다．



13) ［역자주） 풀어서 이야기하면 물려받은 작업이라고 생각할 수 있다. 즉, 기존에 존재하던 것에서
                                                           물려받아서 새로운 쟉업을 추
   가한 경우를 말한다. 이를 수정판이라고 해석했다．
14) 이 항목은 오픈 소스에만 국힌된 것이 아니工 현채 저작권 및 특허권 침해와 콴련해서 진행되고
                                                           있는 사황은 모든 개발자에게
  해당하는 부분이다．
15) （역자주） 파일 개념을 이용해서 read加rite／奴：ti할 수 있는 것



                                                                       277 1
 難 及R   Embedded Linux Primer



        口 최소한의 조건을 갖춘 기본 디바이스 드라이버는 코드 몇 줄로도 가능하다. 이 장에서는
           최소한의 코드를 설명했고 이 기본 뼈대에 몇 가지 개념을 추가해1 보았다．

        口 적재 가능한 모듈로 설정한 디바이스 드라이버는 부팅 후 실행중인 커널에 동적으로 삽
           입 및 제거가 가능하다．

        口 디바이스 드라이버 모듈을 삽입, 제거하거나 항목을 나열해1 보기 위해서 모듈 유틸리티
           를 이용한다. 이를 위한 몇 가지 모듈 유틸리티에 대해서 자세히 알아보았다．

        口 파일 시스템 내에 있는 디바이스 노드 파일들은 사용자 영역 프로그램과 디바이스 드라
           이버를 연결하는 아교 역할을 한다．

        口 드라이버가 제공하는 메서드로 UNIX／리눅스 디바이스 드라이버에서 공통적으로 볼 수
            있는 익숙한 함수인 open, read, write, 이ose를 구현하게 된다. 이 메커니즘에 대해서
           는 예제를 통해써 설명했고, 간단한 사용자 어플리케이션을 통해써 드라이버가 졔공하
           는 메서드들을 시험해1 보았다.

        ［그 마지막에는 커널 디바이스 드라이버와 오픈 소스의 GPL（일반 공공 라이선스） 간의 관계
           에 대해서 설명했다．



8.6. ] 더 읽01 보기
         라눅스 다바이스 드라이버（乞加ux Device 1万加ers), 3판
         Alessandro Rubini and Jonathan Corbet / 박재호, 이해陪 역
         O'Reilly Publishing, 2005 / 한빛미디어, 2005


         파일 시스템 계층 표준（Filesystem Hierarchy Standard)
         편집: Rusty Russel, Daniel Quinlan, and Christopher Yeoh
         파일 시스템 계층 표준화 그룹（The File Systems Hierarchy Standards Group)
         www. pathname. com/ fhs/


         Rusty's Linux Kernel Page
         Module Utilities for 2.6
         Rusty Russell
         http://kernel. org/pub/linux/kernel/people/rusty/




I 278
이번 징K게서 배울 내용


  U 리눅스 파일 사스템의 개념     1 ext2

  1ext3                1 ReiserFS

  1JFFS2               1 cramfs

  1 네트워크 파일 시스템（NFS)   U 의사 파일 시스템

  口 기타 파일 시스템          U 간단한 파일 시스템 만들기

  U 요약
難 月U     Embedded Linux Primer




   아마 임베디드 개발자가 하게 되는 선택 중에서 가장 중요한 것 중의 하나가 어떤 파일 시스
   템（들）을 사용할 것인지일 것이다. 일부 파일 시스템은 성능에 최적화되어 있고, 또 다른 것
   은 공간 활용을 위해 최적화되어 있을 수 있다. 또 어떤 파일 시스템은 장치를 갑자기 제거하
   거나, 전원이 끊겼을 때 데이터를 복구하는 부분에 최적화된 것도 있을 것이다. 여기서는 리
   눅스 시스템에서 주로 사용되는 파일 시스템을 소캐하고, 각각을 임베디드 시스템에 적용시
       켰을 때 어떤 특징이 있는지 알아본다. 하치만 여기서 파일 시스템의 내부까지 키술적으로
   자세히 들어가지는 않을 것이다. 대신에 파일 시스템이 어떻게 동작하는치에 대한 측면 그리
   고 각각의 파일 시스템을 이용해서 개발할 때 생길 수 있는 사항을 살펴볼 것이다. 더 자세한
       사항이 궁금한 독자는 9.11.1절 "더 읽어 보기"에 있는 자료를 참고하기 바란다.

   먼저 초기 리눅스 데스크탑 환경에서 가장 많이 사용되었던 파일 시스템부터 시작해 보자. 즉，
       확장 파일 시스템 2(ext2）를 이용해서 앞으로 다룰 내용을 이해하기 위한 기본 개념을 설명
   하도록 하겠다. 그 다음에는 현재 배포되고 있는 인기 있는 데스크탑 리눅스 시스템에서 기본
       파일 시스템으로 많이 이용되는 ext2의 후손인 확장 파일 시스템 3(ext3）을 설명하겠다．

   몇 가지 기초 개념을 설명한 후에는, 데이터 복구나 저장 공간 확보에 최적화되어 있거나 플
       래시 메모리 장치에서 사용되도록 설계된 파일 시스템 등의 다앙한 특수 파일 시스템들을 살
   펴볼 것이다. 그리고 네트워크 파일 시스템（NFS）도 설명하고, 더 중요한 주제로서 proc
       파일 시스템 및 sysfs 파일 시스템을 포함한 의사 파일 시스템（pseudo file system)에 대
       해서도 설명할 것이다．



9. ] 리눅스 파일 시스템의 개념
       각각의 파일 시스템에 대해서 자세히 알아보기 전에 , 리눅스 시스템에서 어떻게 데이터가 저
       장되는지에 대한 큰 그림을 한번 보도록 하자. 8장, "디바이스 드라이버 기초"를 통해서 캐릭
       터 디바이스의 구조에 대해 살펴본 적이 있다. 일반적으로 캐릭터 디바이스는 데이터를 직렬
       화된 스트림（serial stream) 형태로 저장하거나 읽어온다. 캐릭터 디바이스의 가장 기본적
       인 예제가 바로 시리얼 포트나 자기 테이프 드라이브（II追gnetic tape drive）이다. 이와 대
       조적으로 블록 디바이스는 같은 크기의 데이터 덩어리만큼을 한번에 읽거나 쓰게 된다. 예를
       들면 전형적인 IDE 하드 디스크 컨트롤러의 경우 물리적인 디스크 장치에 접근 가능한 주
       소 범위 내에 있는 데이터에 대해서 한번에 512바이트 크기만큼 전송하도록 되어 있다．
                                                             파일 시스템    Chapter 9




9.1. ] 파티션
       파티션은 물리 장치 내부를 논리적으로 분할헤서 그 분할된 영역에 각각 파일 시스템을 위치
       할 수 있도록 한 것이다. 최상위 레벨에서 데이터는 파티션으로 분리된 물리 장치에 저장된
       다. 파티션은 물리적인 매체를 논리적으로 분할하1 놓은 것이며 , 해당 파티션의 종류에 따라
       서 데이터가 구성된다. 물리적인 장치에 대해서 파티션 하나로 모든 공간을 포함하도록 할
       수도 있고, 특별한 목적에 맞도록 여러 개의 파티션으로 분할할 수도 있다. 결국 파티션은
       하나의 파일 시스템을 온전하게 담을 수 있는 논리적인 디스크라고 생각할 수 있다．

      ［그림 9-1］은 파티션과 파일 시스템의 콴계를 보여 준다．



                                   파일 시스템
                                   메타 데이터


                                   파일 시스템
                                    데이터




                                     파티션
          플래시
          메모리
           장치
       I 그림 9너 파티션 및 파일 시스템

       리눅스에서는 블록 디바이스에 대해서 파티션을 조작하기 위해 fdisk라는 유틸리티를 이용
       한다. 대부분의 리눅스 배포 버전에 설치되어 있는 최신 fdisk 유틸리티는 90개 이상의 다른
       파티션 타입1）을 인식할 수 있다. 하지만 실제로 리눅스 시스템에서는 일반적으로 몇 가지만
       주로 사용되는데 , 많이 사용되는 파티션 타입으로는 리눅스, FAT32, 리눅스 스왑 파티션
       등이 있다．




1) ［역자주） 파티션 타입도 파일 시스템 타입과 거의 1:1 관계를 갖는다. 하지만 리눅스의 경우 Unux native 파티션 타입에는 eXt,
   ex3 등 여러 종류의 파일 시스템을 담을 수 있다．


                                                                            281 1
 薯ma       Embedded Linux Primer




       ［리스트 9-1]은 1侶B 포트에 연결된 콤팩트 플래시 장치를 대상으로 fdisk 유틸리티를 실행
        시킨 결과를 나타낸 것이다. 이 시스템은 USB 서브시스템이 콤팩트 플래시 장치를
        /dev/ sdb 디바이스 노드에 할당한 경우이다．

       ［리스트 9-1] fdisk를 이용해서 파티션 정보 출력하71


            # fdisk /dev/ sdb
            Command (m for help) : p
            Disk /dev/ sdb: 49 MB, 49349120 bytes
            4 heads, 32 sectors/track, 753 cylinders
            units = cylinders of 128 "" 512 = 65536 bytes

              Device Boot          Start           End       Blocks    Id System
            /dev/ s（北江 "              1           180        11504    83 Linux
            /dev/ sdb2              181           360        11520    83 Linux
            /dev/ sdb3              361           540        11520    83 Linux
            /dev/ sdb4              541           753        13632    83 Linux




        위 경우에 fdisk를 이용해서 하나의 장치에 네 개의 파티션이 만들어져 있는 것을 볼 수 있는
        데 , 그중 하나는 Boot 부분에 별표를 통해서 부팅 가능하다고 표시되어 있다. 이 정보는 디
        바이스에 파티션 테이블을 저장하기 위한 데이터 구조에 해당 플래그 값을 설정한 것이다．
        위 리스트를 보면 fdisk의 논리적인 기본 저장 단위가 실린더2）라는 것을 알 수 있다. 이 장
        치에는 실린더 하나가 64KB를 저장하고 있다. 반면 리눅스는 최소 저장 단위를 논리적인
        블록으로 이용한다. 그래서 위 리스트를 통해서 하나의 블록이 1024바이트3) 단위라는 것을
        알 수 있다.

        이런 방식으로 콤팩트 플래시가 파티션된 후에는, 각각의 파티션을 자신이 원하는 파일 시스
        템 형식으로 포맷할 수 있다. 파티션을 자신이 원하는 파일 시스템 형식에 맞게 포맷한 후에
        는 리눅스 시스템에서 그 파티션을 파일 시스템에 맞게 마운트할 수 있다．




2) 실린더 (C川nder）라는 용어는 회젼하는 빙식의 저장 장치에서 차용한 것이다． 실린더는 주어진 섹터에 존재하는 헤三가 읽을 수
   있는 톄이터로 이루어진다. 이 용어는 기존어］ 사용햐던 파일 시스템 유틸리티들콰의 호환성 때문어］ 사용되고 있다．
3) （역자주） 계산이 쉽지는 않은더］, /dev/sdbl 항목을 보면 Bk兀k的］ 11504이고， 실린더 수가 180개이다． 햐니의 실린더가 6띠KB 이
  7] 때문에 180x64KB / (UnitSize) = 11504이므로， UnitSize = 1024가 된다．


1282
                                                            파일 시스템       Chapter 9




9.2 ext2
    이제 ［리스트 9工의 예제에서 fdisk로 생성된 파티션들을 포맷해야 한다. 이를 위해서
    mke2fs 유틸리티를 이용하는데 , mke2fs는 DOS의 如rn追t 명령과 비슷하다. 이 유틸리티
    는 지정한 파티션에 ext2 형식의 파일 시스템을 만드는 일을 한다. 다른 파일 시스템을 만들
    기 위해서는 그 파일 시스템에 해당하는 유틸리티를 이용해야 한다. ［리스트 9-2］에 지금
    설명한 과정을 실행한 결과를 나타냈다．

    ［리스트 9-2) mke2fs로 파티션 포맷하기

       # mke2fs /dev/sdbl -L CFlash_Boot_Vo1
       mke2fs 1. 37 (21-Mar- 2005)
       Fi 1esystem label =cFl ash_Boot_Vol
       OS type: Linux
       Block size=1024 (log=O)
       Fragment size=1024 (log=O)
       2880 m nodes, 11504 blocks
       575 blocks (5. 00%) reserved for the super user
       First data block=1
       Maximum filesystem blocks=11796480
       2 block groups
       8192 blocks per group, 8192 fragments per group
       1440 mnodes per group
       superbiock backups stored on blocks:
                8193

       writing mnode tables: done
       writing superblocks and filesystem accounting information: done

       This filesystem will be automatically checked every 39 mounts or
       180 days, whichever comes first. use tune2fs -c or -i to override.
       #



    ［리스트 9-2］의 내용에는 ext2 파일 시스템에 관련된 많은 정보가 포함되어 있는데 , 이 내
    용들은 e砒2 파일 시스템의 동작에 대해서 이해할 수 있는 훌륭한 단서를 제공한다. 이 파티
    션은 ext2 형식으로 포맷되었고 볼륨 라벨은 CFlash Boot Vol이다. 그리고 리눅스 파티
     션 위에 1024블록 크기로 생성했고, 11,504 블록에 달하는 2.880개의 mlode를 위한 공간
 囊 好a    Embedded Linux Primer




        이 할당되었다. 여기서 in이扼는 파일 하나를 표현하는 기본 자료 구조를 나타낸다. ext2 파
        일 시스템에 대한 자세한 내부 구조에 대해서는 이 장 뒤편의 9.11.1절의 참고 자료를 찾아
        보기 바란다．

       ［리스트 9-2J의 n出e2fs의 출력 내용을 통해서 저장 장치가 어떻게 조직되는지에 대한 특성
       을 확인할 수 있다. 블록 크기가 1024바이트라는 것은 이미 알고 있다. 하지만 특정 어플리
        케이션을 위해서 필요에 따라서 mke2fs어］ 옵션을 줌으로써 다른 블록 크기를 갖도록 ext2
       파일 시스템을 포맷할 수도 있다. 현재 치원되는 블록 크기는 1024, 2048. 4096이 있다．

       블록 크기를 결정하는 것은 언제나 성능 문제와 타협점을 찾아야 한다. 블록 크기가 큰 경우
       에는 디스크에 파일이 많을 경우에 더 많은 공간이 낭비되는데 , 그 이유는 각각의 파일이 블
       록의 배수 단위로 공간을 차지하기 때문이다. 블록 크기 Xn을 벗어나는 자투리가 있으면 그
       것 역시 블록 하나를 차지하게 된다. 반면에 블록 크기를 너무 작게 할 경우에는 파일 시스템
       이 블록과 파일 간의 매핑을 위한 메타 데이터를 관리하는 데 너무 많은 비용이 들게 된다．
       자신의 시스템에서 블록 크기를 얼마로 두는 것이 가장 좋은지를 결정하는 것은 직접 테스트
       하면서 비교해 보는 방법밖에 없다．


9.2. ] 파일 시스템 마운트하기

       파일 시스템을 생성한 후에는 실행중인 리눅스 시스템에서 파일 시스템을 마운트시킬 수 있
       게 된다. 물론 하드웨어 장치에 대한 접근 권한을 갖고 있어야 하고, 커널도 해당 파일 시스
       템 형식을 지원할 수 있는 기능을 포함해서 컴파일되어 있거나 적재 가능 모듈 형태로 사용할
       수 있어야 한다. 다음 명령어는 이전에 생성한 ext2 파일 시스템을 치정한 마운트 지점에
       마운트시키는 일을 한다．

          # mount /dev/ sdbl /mnt/ flash


       위 명령어는 먼저 리눅스 머신에 /mn七／flash라는 디렉터리가 만들어져 있다고 가정하고
       있다. 이 디렉터리를 마운트 지점이라고 부르는데 , 파일 시스템 계층에서 바로 이 지점을 시
       작으로 해당 파일 시스템이 설치（마운트）되기 때문이다. 우리는 이전에 설명한 플래시 장치
       를 마운트하는데 , 커널에서는 이 장치가 /dev/ sdbl로 할당되어 있다. 전형적인 리눅스 데
       스크탑 시스템（또는 개발 시스템）에서 위 명령을 실행시키기 위해서는 루트 권한4）을 가지고

4) CD-ROM처럼 루트 사용자가 아니어5三 마운트할 수 있는 파일 시스템도 있다．


p284
                                                            파일 시스템   Chapter 9



있어야 한다. 마운트 지점은 현재 파일 시스템의 어느 곳이든 정할 수 있고, 이 위치가 새로
마운트되는 장치의 최상위 디렉터리（루트）가 된다. 이전 예제의 경우 플래시 장치에 존재하
는 어떤 파일을 접근하려고 할 때 반드시 /mn七／flash 경로를 시작으로 위치를 치정해야
한다．

mount라는 명령어는 다양한 옵션을 갖추고 있는 강력한 명령어이다. mount 명령어에서 사
용할 수 있는 옵션 중 상당수는 마운트하려는 대상 파일 시스템의 종류에 따라 달라진다. 대
부분의 경우 moun七는 스스로 커널이 알고 있는 파일 시스템 형식으로 포맷된 파일 시스템을
감지할 수 있다. 이 장을 진행하면서 몇 가지 추가적인 mount 명령어를 이용하는 예제를
보게 될 것이다．

［리스트 9-3］은 임의의 임베디드 시스템을 위해서 구성된 플래시 장치의 디렉터리 내용을
나타낸 것이다．

［리스트 9-3] 퓰래시 장치 내용

  $ is -1 /mnt/ flash
  total 24
  drwxr-xr- x 2 root root 1024 Jul 18 20:18 bin
  drwxr- xr-x 2 root root 1024 Jul 18 20:18 boot
  drwxr-xr- x 2 root root 1024 Jul 18 20:18 dev
  drwxr- xr- x 2 root root 1024 Jul 18 20:18 etc
  drwxr-xr-x 2 root root 1024 Jul 18 20:18 home
  drwxr-xr- x 2 root root 1024 jul 18 20:18 lib
  drwx         2 root root 12288 Jul 17 13: 02 lost+found
  drwxr-xr-x 2 root root 1024 jul 18 20:18 proc
  drwxr-xr- x 2 root root 1024 Jul 18 20:18 root
  drwxr- xr- x 2 root root 1024 Jul 18 20: 18 sbin
  drwxr-xr-x 2 root root 1024 Jul 18 20:18 tmp
  drwxr- xr- x 2 root root 1024 Jul 18 20:18 usr
  drwxr- xr-x 2 root root 1024 Jul 18 20:18 var
  $



［리스트 9-3］은 임베디드 시스템에서 사용될 수 있는 예제 루트 파일 시스템의 최상위 디렉
터리를 보여 주고 있다. 6장, "시스템 초기화'에서는 루트 파일 시스템의 내용을 어떻게 구성
해야 하는지에 대한 설명 및 예제를 제시하고 있다．
    驪     Embedded Unux Primer




9.2.2 파일 시스템 무켤성 컴사

        ext2 파일 시스템의 무결성을 검사하기 위한 명령어로 e2fsck7} 이용된다. 파일 시스템의
        내용이 깨질 수 있는 경우는 몇 가지가 있치만, 가장 횬한 이유는 갑작스럽게 전원 공급이
        끊기거나, 열려 있는 파일을 닫고 파일 시스템을 언마운트하지 않고 의도적으로 전원을 꺼버
        리는 경우이다. 리눅스 배포판들은 （올바르게 시스템을 종료했다고 가정했을 때） 시스템 종
        료 시에 이러한 沓｝를 밟도록 되어 있다. 하지만 임베디드 시스템의 경우는 예상치 못하게
        전원이 끊기는 경우가 횬하기 때문에 , 이런 상황에 대응하기 위한 방어책을 마련할 필요가
        있다. e2fsck는 ext2 파일 시스템을 사용하는 시스템에서 비정상적인 전원 끊김에 대비하
        기 위한 1차 방어선으로 이용된다.

        ［리스트 9-4］에는 이전 예제의 콤꽥트 플래시 장치에 e2fsck를 실행시킨 결과이다. 알맞게
        포맷하고 올바르게 언마운트했기 때문에 , 아무런 에러도 없어야 한다．

        ［리스트 9-4) 깨끗한 파일 시스템을 컴사한 경우


          # e2fsck /dev/ sdbl
          e2fsck 1. 37 (21-Mar- 2005)
          CFlash_Boot_Vo1 : clean, 23/ 2880 files, 483/11504 blocks
          #




        e2fsck 유틸리티는 파일 시스템의 일관성을 몇 가지 측면에서 검사하게 되는데 , 만약에 아
        무런 문제점도 찾지 못한 경우에는［리스트 9-띠에 나오는 것과 비슷한 메시지를 보여 준다．
        e2fsck는 반드시 언마운트된 파일 시스템을 대상으로 실행시켜야 한다는 것을 주의하기5)
        바란다. 물론 마운트된 파일 시스템을 대상으로 실행시킬 수도 있지만, 디스크나 플래시의
        내부 자료 구조를 망가트릴 수도 있다．

        좀 더 재미있는 예제를 위해서 , 마운트된 상태에서 콤팩트 플래시 장치를 소켓에서 빼냈다．
        그렇게 한 후 e2fsck를 실행한 결과 ［리스트 9-5J와 같은 내용을 볼 수 있었다. 의도적으로
        장치를 빼내기 전에 파일을 하나 생성하고 편집하는 창을 열어 두고 있었다. 이렇게 함으로써
        파일을 가리키는 자료 구조는 물론이고 파일의 데이터를 담고 있는 데이터 블록도 깨지게 된다．

5) （역자주） 역자도 이 명령에 때문에 공들여 작업한 내용이 든 하드디스크를 포맷해야 할 때가 있었다． 더군다나 다른 팀이 소스
 형상 관리용으로 사용하던 하드였다．
                                                                 파일 시스템         Chapter 9



      ［리스트 9-5] 깨진 파일 시스템 검사

          # e2fsck -y /dev/sdbl
          e2fsck 1. 37 (21-Mar-2005)
          /dev/ sdbl was not cleanly unmounted, check forced.
          Pass 1: checking mnodes, blocks, and sizes
          mnode 13, i_blocks is 16, should be 8. Fix? yes

          Pass 2: checking directory structure
          Pass 3: checking directory connectivity
          Pass 4: checking reference counts
          Pass 5: checking group summary information

          /dev/ s（北1: 出山"肯六女 FILE SYSTEM 닙AS MODIFIED 女央卉央女
          /dev/ sdbl: 25/2880 files (4. 0% non-contiguous) , 488/11504 blocks
          #



      ［리스트 9_5］를 보면 e2fsck가 콤팩트 플래시가 비정상적으로 언마운트된 것을 감지한 것
       을 알 수 있다. 또한 e2fsck7} 파일 시스템을 처리하는 과정을 눈으로 볼 수 있는데，
       e2fsck는 파일 시스템의 다양한 내부 자료 구조를 검사하는 5단계를 진행한다. 아이노드
       (mnode)6) 13번으로 인식되는 파일 하나에 에러가 있는 것으로 감지되고, 자동으로 오류를
       수정하는데 이는 e2fsck를 실행할 때 ey 옵션을 지정해 주었기 때문이다．

       물론 실제 시스템에서는 이렇게 운이 좋을 수 없다. 어떤 종류의 파일 시스템 오류는
       e2fsck로 고칠 수 없다. 또한 임베디드 시스템 디자이너가 이해할 사항은 만약에 올바른
       종료 절차（shutdown）를 밟지 않고 전원이 끊긴 경우에는 다음 번 부팅 시 부트 디바이스
       전체를 검사해서 오류를 수정하는 시간만큼 부팅 시간이 지연된다는 것이다. 더군다나 수정
       할 수 없는 오류의 경우에 . 시스템 부팅은 중단되고 사용자가 수동으로 개입해야 할 수도 있
       다. 또한 파일 시스템이 상당히 큰 경우, 파일 시스템 검사（fsck）가 몇 분에서 , 기가 단위의
       파일 시스템의 경우는 수시간까지 걸릴 수도 있다는 점을 주의해야 한다．

       파일 시스템이 깨지는 것에 대한 다른 방어책은 모든 쓰기 연산을 디스크에 즉시 기록하도록
       하는 것이다. sync 유틸리티를 이용하면 큐에 저장된 모든 I/o 요청을 각각의 장치에 강제
       로 바로 기록할 수 있다. 예상치 못하게 전원이 끊기거나 제한될 때 데이터가 깨질 수 있는

6) 파일 시스템의 파일 하나는 ext2 파일 시스템에서는 내부 자료 구조 m1lode 하나로 표현된다．


                                                                                      287 1
難 蘿1    Embedded Linux Primer




       가능성을 최소화하기 위한 전략 중의 하나는 쓰기 연산이 이루어지는 매 순간 또는 어플리케
       이션에서 필요로 하는 순간마다 sync 명령을 실행시키는 것이다. 이 방법의 대가는 물론 성
       능상의 손해다. 성능을 최적화하기 위해서 현채의 모든 운영체제가 디스크의 쓰기 작업을 뒤
       로 미루는 방법을 기본적으로 사용하고 있는데 sync를 동원하게 되면 이 최적화를 해치게
       된다．

       리눅스 시스템에서 ext2 파일 시스템은 빠르고, 효율적이고, 강건함을 두루 갖춘 성숙한 파
       일 시스템이다. 하지만 저널링(journaling) 파일 시스템을 통해서 얻을 수 있는 신뢰성이
       필요할 경우나, 비정상적으로 종료하지 않은 경우 다음 부트에 걸리는 시간이 시스템 디자인
       에서 중요한 부분이라면 ext3 파일 시스템을 고려해 봐야 한다．



9.3 ex恪
       ext3 파일 시스템은 매우 강력하고, 뛰어난 성능과 강건성을 갖춘 저널링 파일 시스템으로
       발전했다. 현재는 이 파일 시스템이 레드햇이나 페도라 코어 시리즈와 같은 인기 있는 데스
       크탑 리눅스 배포판에서 기본 파일 시스템으로 사용되고 있다．

       ext3 파일 시스템은 기본적으로 ext2 파일 시스템을 확장해서 거기에 저널링 기능을 추가한
       것이다. 저널링이란 파일 시스템에 수정이 가해질 때마다 특수한 파일에 그 정보를 기록해
       두었다가 저널링 포인트라는 특정 지점으로 복구할 수 있도록 하는 기술이다. ext3 파일 시
       스템의 가장 큰 장점 중의 하나라면 역시 불완전 시스템 종료 후에도 바로 마운트할 수 있다
       는 것이다. 이전 절에서 언급한 것처럼 , 전원이 갑자기 끊기거나 해서 시스템이 예상치 못하
       게 셧다운된 경우에 시스템은 시간이 걸리는 작업인 파일 시스템 일관성 검사를 진행하게 된
       다. ext3 파일 시스템으로는 이러한 일관성 검사가 필요 없는데 , 이는 저널이 파일 시스템의
       일관성이 유지되던 마지막 시점으로 쉽게 되돌릴 수 있게 해 주기 때문이다.

       파일 시스템 내부의 상세 설계에 대한 내용은 이 책의 범위를 벗어나지만, 저널링 파일 시스
       템이 어떻게 동작하는지에 대해서는 간단히 설명하는 것이 좋을 것 같다. 저널링 파일 시스
       템은 보통은 사용자에게는 숨겨져 있는 특수한 파일을 이용하는데 , 이 파일에 파일 시스템의
       메타데이터7）와 파일 데이터 자체가 저장된다. 그리고 이 특수 파일을 저널이라고 부른다．

7) 메타데이터는 파일 내용과는 대조적으로 파일 자체에 대한 정보를 말한다． 예를 들어, 파일 생성 시간， 크기， 人｝辛   블록 수
   등을 들 수 있다．
                                                               파일 시스템     Chapter 9



       언제든 파일 시스템이 （쓰기 연산 등을 통해서） 변경되려고 할 때 그 변경 사항이 제일 먼저
       저널에 기록된다. 파일 시스템 드라이버는 실제 저장 매체를 변경시키기 전에 저널에 그 내
       용이 먼저 기록되는 것을 보장해야 한다. 즉, 드라이버는 저널에 내용이 기록된 이후에 실제
       저장 장치에 파일과 메타데이터를 수정하는 명령을 내보낸다. 만약 저장 매체（예를 들어 , 디
       스크 또는 플래시）에 데이터를 기록하는 중에 시스템이 채부팅된 경우에는 저널에 기록된 변
       경 사항을 다시 진행하기만 하면 파일 시스템의 일관성을 유지할 수 있게 되는 것이다.

       ext3 파일 시스템의 설계 목표 중 가장 중요한 것은 기존 ext2 파일 시스템과 상위 하위
       모든 경우에 호환성을 갖도록 하는 것이다. 그러면 ext2 파일 시스템을 e砒3 파일 시스템으
      로 변경하거나 그 반대의 경우에도 다시 포맷하거나 디스크 상의 모든 데이터를 다시 기록할
      필요가 없다. 어떻게 하는지 한 번 보도록 하자8) . ［리스트 9-6］에 자세한 과정을 보여 주고
      있다．

      ［리스트 9-63 ext2 파일 시스템을 ext3 파일 사스템으로 변경하기

         # mount /dev/sdbl /mnt/ flash        <<< ext2 파일 시스템 마운트
         # tune2fs -j /dev/sdbl               <<< 저널 생성
         tune2fs 1.37 (21-Mar- 2005)
         creating journal mnode: done
         This filesystem will be automatically checked every 23 mounts or
         180 days, whichever comes first. Use tune2fs -c or -i to override.
         #



      설명을 위해서 /rnnt/ flash어］파일 시스템을 먼저 마운트했는데 , 일반적으로는 마운트하지
      않은 ext2 파티션에 이 명령을 실행시킨다. tune2fs는 설계상 파일 시스템이 마운트된 경
      우에는 . 如urnal이라는 숨김 파일 형태로 저널 파일을 생성하도록 되어 있다. 리눅스에서
      점（.）으로 시작하는 파일은 숨김 파일로 인식된다. 그래서 많은 커맨드 라인 유틸리티들이
      이 숨김 파일은 무시하도록 되어 있다. ［리스트 9-7］은 is 명령에 -a 옵션을 설정해서 실행
      시킨 결과를 보여 주는데 , 이는 숨김 파일도 포함한 모든 파일을 나열한다．




8) 이렇게 파일 시스템을 변경하는 것은 개발 과정으로만 샘각해야 한다．



                                                                              289 1
       Embedded Linux Primer




     ［리스트 9-7) ext3의 저널 파일

        $ is -al /mnt/ flash
        total 1063
        drwxr-xr- x 15 root root    1024 Aug 25 19: 25
        drwxrwxrwx S root root      4096 Jul 18 19: 49 . .
        drwxr-xr- x 2 root root     1024 Aug 14 11: 27 bin
        drwxr-xr- x 2 root root     1024 Aug 14 11: 27 boot
        drwxr-xr-x 2 root root      1024 Aug 14 11: 27 dev
        drwxr-xr- x 2 root root     1024 Aug 14 11: 27 etc
        drwxr-xr-x   2 root root    1024 Aug 14 11: 27 home
        -rw          1 root root 1048576  Aug 25 19: 25 .journal
        drwxr-xr-x   2 root root    1024 Aug 14 11: 27 lib
        drwx         2 root root   12288 Aug  14 11: 27 lost+found
         drwxr-xr-x 2 root root     1024 Aug 14  11: 27 proc
         drwxr-xr- x 2 root root    1024 Aug 14  11: 27 root
         drwxr- xr-x 2 root root    1024 Aug  14 11: 27 sbin
         drwxr-xr-x 2 root root     1024 Aug 14 11: 27 tmp
         drwxr-xr- x 2 root root    1024 Aug 14 11: 27 usr
         drwxr-xr-x 2 root root     1024 Aug 14 11: 27 var




      이제 플래시 장치에 저널 파일을 생성했고, 사실상 ext3 파일 시스템 형식으로 포맷되었다9)
      고 말할 수 있다. 다음 번에 시스템을 재부팅할 때나 혹은 e2fsck 유틸리티를 새로 만들어
      진 ext3 파일 시스템을 대상으로 실행시키면 저널 파일은 자동으로 아예 보이지 않게 숨겨질
      것이다. 즉, 이 저널 파일에 대한 메타데이터는 저널 파일을 저장하기 위해서 별도로 예약된
      in이扼에 저장된다. . 如urnal 파일을 볼 수 있게 되면 사용자가 그 파일을 지우거나 수정할
      수 있는 위험성이 있기 때문이다．

      때로는 저널 파일을 다른 장치에 만들어 두는 게 좋을 수도 있다. 예를 들어 , 만약 시스템에
      두 7下1 이상의 물리적 저장 장치가 있다면 ext3 저널링 파일 시스템을 첫 번째 드라이브에
      놓고, 저널 파일은 두 번째 드라이브에 놓을 수 있다. 이 방법은 물리 저장 장치가 플래시
      기반이든 원형 디스크 형태이든 상관이 없다. 기존 ext2 파일 시스템에서 저널 파일을 다른
      파티션에 생성하기 위해서는 七une2fs 명령어를 다음과 같이 실행하면 된다．

         # tune2fs -J device=/dev/sdal -j /dev/sdbl


9) L역자주） 물론 데이터는 그대로 남아 있고, 파일 시스템 형식만 바뀐 것이다．
                                                          파일 시스템    Chapter 9




       이 명령어를 실행시키기 위해서는 먼저 저널 파일이 위치할 장치가 반드시 ext3 파일 시스템
       으로 포맷되어 있어야 한다．



9.4 ReiserFS
       ReiserFS는 수세（SuSE）나 젠투（Gentoo) 리눅스 등의 일부 데스크탑 배포 버전에서 인기
       리에 사용되었다. 이 글을 쓰는 시점에서 Reiser4가 저널링 파일 시스템으로 구현되어 있다．
       ext3 파일 시스템처럼 ReiserFS도 하나의 파일 시스템 오퍼레이션이 수행될 때 그것이 완
       전히 처리되거나 아니면 아무런 일도 하지 않은 것으로 처리하거나 둘 중의 하나를 보장해
       쥔：1-. ext3와는 달리 Reiser4는 시스템 프로그래머를 위한 API를 도입해서 파일 시스템 처
       리에 대한 원자10）성（a切micity）을 보장하도록 해 준다. 다음 예를 한번 보자．

       어떤 데이터베이스 프로그램은 데이터베이스에 자료를 매우 빈번히 업데이트한다. 그 중에서
       쓰기 연산의 일부는 파일 시스템까지 업데이트되도록 만드는데 , 데아터베이스를 업데이트하
       기 위해서 여러 개의 파일에 write 연산을 실행해야 할 때 , 첫 번째는 wri扼가 되었지만 아
       직 마지막 wri扼까지는 되치 않은 상태에서 전원이 끊겼다고 가정하자. 이 경우 저널링 파일
       시스템에서는 변화될 파일에 대한 메타데이터를 저널 파일에 저장하고 있기 때문에 , 시스템
       에 전원이 다시 들어오면 커널은 파일 시스템이 마지막 일관성을 갖고 있던 시점으로 돌아갈
       수 있게 된다. 그 말은 만약 파일 A가 전원이 끊기기 전에 16KB의 파일이라고 보고되었다
       면 재부팅되어서도 다시 16KB가 될 것이고, 디렉터리도（실제로는 mnode) 이 파일에 대한
       올바른 크기 정보를 가치고 있을 것이라는 의미이다. 그렇지만 이것은 테이터가 파일에 올바
       르게 기록되었다는 것을 의미하는 것이 아니라 단지 파일 시스템에 오류가 없다는 것을 의미
       한다. 그렇기 때문에 이전 시나리오에서 데이터베이스 프로그램이 기록하려던 일련의 데이터
      는 잃어버린 것이고, 만약에 이를 복구하려고 한다면 이는 데이터베이스 프로그램이 처리해
      야 할 일이다．

      Reiser4 파일 시스템의 상태（일관성）와 파일 시스템 연산에 사용되는 데이터까지도 보호하
      는 고성능의 "원자（a切mic)" 파일 시스템 연산을지원한다. Reiser4는 데이터베이스 관리자
      같은 프로그램에서 일련의 파일 시스템 쓰기 명령이 모두 온천히 성공하거나 아니면 모두 실
      패하거나 하는 두 가지 상태만을 갖도록 하는 API를 사용자e레벨에서 사용할 수 있도록 제

10) （역자주） 어떤 일련의 작업을 분리할 수 없다는 의미에서 '원자라는 용어로 해석된다. 예를 들어, 쓰71 연산
                                                                  /\ B는 항상 한
    묶욤으로 처리해야 한다고 했을 때 이를 보장해 주는 것을 '원자성이 있다’고 말한다．
          Embedded Linux Primer




        공한다. 그렇게 함으로써 파일 시스템 일관성은 물론이고, 시스템 충돌 이후에도 파일에 쓰
        레기 데이터나 데이터의 일부만 남는 일이 없도록 해 준다．

        ReiserFS에 대해서 실제 소프트웨어적인 세부 내용은 9.11.1절에 나와 있는 홈페이지를
        방문해 보기 바란다．



9.5 JFFS2
        플래시 메모리는 임베디드 제품에서 폭넓게 이용되고 있다. 하지만 플래시 메모리는 기술적
        인 특성 때문에 데이터를 기록하는 시간이 매우 길고, 그래서 전원이 끊겼을 때도 훨씬 비효
        율적이며 데이터가 깨질 가능성도 아주 높아진다. 이러한 비효율성은 블록 크기 때문인데，
        플래시 메모리 장치의 블록 크기는 보통 수십에서 수백 킬로바이트 단위로 결정된다. 플래시
        메모리는 하나의 블록 단위로만 데이터를 삭제할 수 있지만, 쓰는 것은 1바이트나 1워드 단
        위로 가능하다. 파일 하나를 수정하키 위해서는 전체 데이터 블록을 모두 지우고 다시 기록
        해야 한다．

        잘 알려져 있듯이 어떤 리눅스 머신이든（또는 다른 운영체제도） 사용하는 파일을 보면 큰 크
        기의 파일보다는 작은 크기의 파일이 더 많이 분포되어 있다. ［그림 9-2］에서 볼 수 있는
        gnuplot으로 만든 히스토그램에는 전형적인 개발용 리눅스 시스템의 파일 크기 분포를 보
        여 준다．

        ［그림 9-2］에서 대부분의 파일의 크기가 10KB 정도도 안 되는 것을 볼 수 있다. 4096 크기
        의 기다란 막대는 디렉터리의 수를 나타낸 것이다. 디렉터리（디렉터리도 사실 파일이다）는
        정확히 4096바이트의 크기를 갖고, 디렉터리 수도 매우 많다. 40,000바이트 이상에 있는
        막대는 가상의 측정값으로 인위적으로 그려 넣은 것이다. 이 수는 측정 단위의 끝인 약
        40KB 이상의 크기를 갖는 파일의 수를 나타낸다. 대부분의 파일이 아주 작은 크기를 갖는
        다는 점이 아주 홍미롭다．




I 292
                                                                                                          파일 시스템   Chapter 9



                                                                                       !         6S1=：二




                   帥




 8815느口Y니 농 L曳겊브
                   棚


                   帥


                   帥
                       mre亡tmie三

                   卿


                   蜘


                   帥


                   帥


                             j J 1 1 111 1 i 1 1   i   J r기   1 n그기1m中如升    =    1         J


                             l（刃的             姓刃m               帥：
                                                                 目         袋k脚   京心刃       系奴好
                                                                F,!. 5,te St쩍省




I 그림 9-2 파일 크기（바이트）


이렇게 작은 크기의 파일은 플래시 파일 시스템 설계자에게는 독특한 도전 과제가 된다. 이
는 플래시 메모리는 전체 블록을 한번에 모두 삭제해야 하고 또한 플래시 블록 하나의 크기가
작은 파일들의 수배에 딜하기 때문에 플래시에 시간이 많이 소요되는 재기록 작업이 필요하
게 된다. 예를 들어 , 128KB의 블록 크기를 갖는 플래시가 4096바이트나 그보다 작은 크기
의 파일을 수십여 7가 가지고 있다고 가정해 보자. 그리고 이제 그 파일들 중의 하나를 수정해
야 한다고 치자. 이 경우에는 플래시 파일 시스템에서 전체 128KB 블록을 하나 지워야 하
고, 그 블록 안에 기록되어 있던 모든 파일을 다시 기록해야 한다. 이는 상당히 많은 시간이
소요되는 작업이다．

플래시에 데이터를 기록하는 데 많은 시간이 소요되기 때문에（하드디스크에 기록하는 것보
다 훨씬 느리다）, 갑작스럽게 전원 공급이 끊겼을 때 데이터가 깨질 가능성도 증가하게 된
다. 갑작스럽게 전원이 끊기는 일은 임베디드 시스템에서 자주 일어나는 현상이다. 예를 하
나 들면 이전 단락에서 설명한 128KB 데이터 블록을 재기록하는 중에 전원이 끊긴다면 아
마 파일 수십 개를 모두 잃어버릴 수도 있다．

JFFS2로 들어가자. 방금 설명한 문제점들과 기타 문제점들은 2세대 저널링 플래시 파일 시
스템 또는 끄고FS2에 의해서 상당히 줄이거나 제거할 수 있다. 원래 JFFS는 스웨덴의 /\xis
커뮤니케이션즈 AB에서 설계하고, 특별히 그 당시에 일반적으로 많이 사용되는 플래시 메모
리 장치를 대상으로 만들어진 것이다. JFFS는 플래시 장치가 갖고 있는 아키텍처와 플래시
의 구조적인 한계를 고려해서 개발되었다．

                                                                                                                        293 1
        1     Embedded Linux Primer




            플래시 파일 시스템의 또 다른 문제점은 플래시 메모리의 수명에 제한이 있다는 점이다. 일
            반적인 플래시 메모리 장치는 최소 10만 번 정도의 쓰기 횟수를 지원하고, 최근에는 더 많은
            100만 번 정도를 지원하는 것이 일반적이다. 이러한 제한 사항은 플래시 장치 내의 각각의
            블록에 적용된다. 이와 같은 특이한 한계로 인해서 플래시 메모리 장치의 여러 블록에 골고
            루 쓰기 연산을 시켜야 한다는 요구 조건이 생겨나게 된 것이다. JFFS2는 이를 위해서 웨어
            레벨링（wear leveling）이라는 기술을 이용한다．

            JFFS2 이미지를 만드는 것은 상대적으로 간단하다. 항상 그렇듯이 먼저 커널이 JFFS2를
            지원하는지를 확인해야 하고, 개발 워크스테이션에도 mkfs. jffs2 유틸리티와 호환되는 유
            틸리티를 가지고 있어야 한다. JFFS2 이미지는 파일 시스템에 필요한 파일을 모아놓은 디
            렉터리를 가지고 만드는데 , ［리스트 9-8］에는 플래시 장치에서 루트 파일 시스템으로 사용
            하려고 할 때 일반적으로 갖는 디렉터리 구조를 보여 준다．

            ［리스트 아8] JFFS2 파일 시스템의 디렉터리 배치

              $ is -l
              total 44
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 bin
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 dev
              drwxr-xr-x      2 root root 4096 Aug 14 11:27 etc
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 home
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 lib
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 proc
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 root
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 sbin
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 tmp
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 usr
              drwxr-xr-x      2 root root 4096 Aug 14 11: 27 var
              $



            실행 시에 필요한 파일도 모두 준비되면 이 디렉터리 구조를 mkfs. jffs2 명령어를 위한
            기본 틀로 사용할 수 있다. mkfs. jffs2 명령어는 ［리스트 9-8］에 있는 것과 같은 디렉터
            리 구조를 가지고 Jr巾S2 형식에 맞는 파일 시스템 이미지를 만든다. mkfs. jffs2어］넘길
            명령에 파라미터로는 소스로 사용할 디렉터리 위치와 丹叩S2 이미지로 만들어낼 출력 파일
            의 이름을 받는다. 출력 파일을 지정하지 않았을 때 기본 값은 현재 디렉터리에 JFFS2 이미
            지를 만드는 것이다. ［리스트 9-9］에서 JFFS2 이미지를 만드는 명령어를 볼 수 있다．



I 294
                                                        파일 시스템       Chapter 9




   ［리스트 9-9) mkfs.jffs2 명령 예졔

      # mkfs. jffs2 -d ./jf1s2-image-dir -o jffs2. bin
      # is -1
      total 4772
      -rw-r--r- - 1 root root 1098640 Sep 17 22: 03 jffs2.bin
      dr叫xr-壯出 13 root root        4096 Sep 17 22: 02 jffs2너ma水-d卄
      #



   ［리스트 9-8］에 있는 파일과 디렉터리 구조가 j ffs2-image-dir 디렉터리에 있고, 바로
   한 단계 상위 디렉터리에서 파일 시스템 이미지를 만들기 위해서 mkfs. jffs2 명령어를
    실행시킨다. -d 옵션을 통해서 mkfs. jffs2 명령어에 파일 시스템 기본 틀이 있는 위치를
    넘겨주게 되고, -o 옵션으로 JFFS2 이미지가 만들어질 출력 파일 이름을 지정한다. 만들어
    진 이미지 j ffs2 .bin은 10장, "MTD 서브시스템"에서 JFFS2와 MTD 서브시스템을 같
    이 설명할 때 사용할 것이다．

    쓰기 연산을 지원하는 플래시 기반 파일 시스템에서는 사용하는 플래시 장치의 수명을 예상
    보다 훨씬 빨리 짧아치게 만들 수 있는 상황이 있다는 점을 주의해야 한다. 예를 들어 , 시스
    템 로거（syslogd와 klogd）의 출력 내용을 플래시 기반 파일 시스템에 기록하도록 만들면
    너무 빈번하게 쓰기 연산이 실행되기 때문에 플래시의 수명이 빨리 다할 수 있다. 일부 프로
    그램 오류도 역시 지속적인 쓰기 연산을 하게 만들 수 있다. 플래시 장치의 수명 내에서 최대
    한 활용하기 위해서는 플래시 장치의 한계에 주의해서 사용해야 한다．



9.6 cramfs
    cramfs 프로젝트에 있는 README 파일을 보면 cramfs의 목표는 "파일 시스템을 작은 ROM
    어］ 꾸겨 넣자."이다. cramfs 파일 시스템은 정적인 데이터나 프로그램을 담는 아주 작은
    ROM 또는 플래시 메모리를 갖고 있는 임베디드 시스템에서 매우 유용하다. 다시 한 번
    cramfs의 README 파일을 보면 "cramfs는 간단하고, 작고, 잘 압축하도록 설계되었다'라고
    되어 있다．
准 驥1   Embedded Linux Prrmer



   cramfs 파일 시스템은 읽기 전용이다. 그리고 mkcramfs라는 커맨드 라인 유틸리티를 이용
   해서 만들 수 있다. 만약 현재 개발 시스템에 없다면 이 장의 마지막 참고 자료 목록에 있는
   링크에서 다운받을 수 있다. JFFS2와 같이 mkcramfs도 명령에 라인에서 생성할 파일 시
   스템의 내용을 담고 있는 디렉터리의 위치를 인자로 넘기도록 되어 있다. ［리스트 9-10］에
   서 cramfs 이미지를 만드는 절차를 상세히 볼 수 있다. 여기서는 JFFS2 이미지를 만들 때
   사용했던 ［리스트 9-8：어］ 있는 것과 같은 파일 시스템 구조를 이용했다．

   ［리스트 9-10) mkcramfs 명령 예제

       # mkcramfs
       usage: mkcramfs [-hi [-v] [-b blksize] [-e edition] [-i file] [-n name]
       dirname outfile
        -h        print this help
        -E        make all warnings errors (non- zero exit status)
        -b blksize use this blocksize, must equal page size
        -e edition set edition number (part of fsid)
        -i file   insert a file image into the filesystem (requires >= 2. 4.0)
        -n name   set name of cramfs filesystem
         p        pad by 512 bytes for boot code
        -s        sort directory entries (old option, ignored)
        -v        be more verbose
        -z        make explicit holes (requires >= 2. 3. 39)
        dirname root of the directory tree to be compressed
        outfile output file

       #
       # mkcramfs . . ./cramfs.image
       warning: gids truncated to 8 bits (this may be a security concern)
       # is -l . ./cramfs.iniage
       -rw- rw-r- - 1 chris chris 1019904 Sep 19 18: 06 . ./cramfs. image



   처음에는 mkcramfs 명령어를 아무런 파라미터 없이 실행시켜서 사용 방법을 알려 주는 메시
   지를 표시하도록 만들었다. 이렇게 하는 것은 이 유틸리티에 대해서는 man 페이지가 없기
   때문에 , 이 메시지가 사용법을 알려 주는 가장 좋은 방법이기 때문이다. 그 이후에는 cramfs
   파일 시스템에 포함시킬 파일이 있는 디렉터리 위치를 현재 디렉터리 으로 지정하고 만들어
   질 파일 시스템 이미지는 cramfs . image라는 이름으로 지정해서 명령을 실행시켰다. 마지
   막 파일들의 목록을 출력해서 , cramfs . image라는 파일이 새로 생성된 것을 확인했다．
                                                  파일 시스템   Chapter 9



만약에 커널이 cramfs를 지원하도록 구성되어 있다면 이 파일 시스템 이미지를 현재 리눅스
개발 시스템에 마운트시켜서 내용을 확인해 볼 수도 있다. 물론 파일 시스템이 읽기 천용이기
때문에 내용을 수정할 수는 없다. ［리스트 9-11］에는 cramfs 파일 시스템을 /mnt/ flash
라는 마운트 지점에 마운트시키는 것을 보여 주고 있다．

［리스트 9너 1) cramfs 파일 시스템 테스트하기

  # mount -o loop cramfs.image /mnt/ flash
  # ls -l /mnt/ flash
  total 6
  drwxr-xr- x 1 root root 704 Dec 31 1969 bin
  drwxr-xr- x 1 root root 0 Dec 31 1969 dev
  drwxr- xr- x 1 root root 416 Dec 31 1969 etc
  drwxr- xr- x 1 root root 0 Dec 31 1969 home
  drwxr- xr-x 1 root root 172 Dec 31 1969 lib
  drwxr- xr- x 1 root root 0 Dec 31 1969 proc
  drws         1 root root 0 Dec 31 1969 root
  drwxr- xr- x 1 root root 272 Dec 31 1969 sbin
  drwxrwxrwt 1 root root 0 Dec 31 1969 tmp
  drwxr- xr-x 1 root root 124 Dec 31 1969 usr
  drwxr- xr-x 1 root root 212 Dec 31 1969 var
  #



mkcramfs 명령을 실행시킬 때 그룹 ID(GID）에 관련된 경고 메시지가 출력되는 것을 봤을
것이다. cramfs 파일 시스템은 파일 시스템의 크기를 줄이고 실행 속도를 향상시키기 위해
서 매우 간결한 메타데이터를 사용한다. cramfs 파일 시스템의 "특징 " 중의 하나는 그룹 ID
필드를 8비트로 잘라서 사용한다는 것이다. 반면 리눅스는 그룹 ID로 16비트를 사용한다．
그 결과 255보다 큰 그룹 ID를 가진 파일에 대해서는 그룹 ID 값의 일부가 잘리기 때문에
［리스트 9-10］처럼 경고 메시지를 보여 주는 것이다．

비록 파일 크기에 제한이 있고, 포함할 수 있는 파일 개수에도 제한이 있지만, cramfs 파일
시스템은 읽기 전용 연산과 빠른 압축이 가장 잘 어울리는 환경인 부트 롬에서 가장 이상적인
파일 시스템이다．




                                                                 297
       a     Embedded Linux Primer




9.7 네트워크 파일 시스템（NFS)
           UNI)( 개발 환경에서 깨발을 해 본 경험이 있다면 의심할 여지 없이 네트워크 파일 시스템
           또는 NFS에 익숙할 것이다. NFS는 특정 디렉터리를 NFS 서버 상에서 노출시키고, 원격
           클라이언트 시스템에서 이 디렉터리를 마운트해서 마치 자신의 시스템에 있는 파일 시스템처
           럼 사용할 수 있게 해 준다. 이와 같은 방법은 유닉스／리눅스 장치들이 많을 경우에 유용하
           고, 임베디드 시스템 개발자에게는 만병통치약과 같은 존채이다. 임베디드 개발자 입장에서
           타깃 보드에서 NFS를 사용하게 될 경우에는 비록 대상 시스템이 제한된 리소스만 가지고
           있는 경우라도 개발또는 디버킹 기간 중에 거대한 파일, 라이브러리 , 툴들, 유틸리티를 담고
           있는 파일 시스템을 이용할 수 있다．

           다른 파일 시스템과 마찬가지로 NFS 역시 반드시 커널이 서버측 기능과 클라이언트측 모두
           를 위해서 NFS를 지원하도록 구성되어 있어야 한다. NFS 서버와 클라이언트 기능은 각각
           별도의 커널 구성 항목이다．

           NFS를 설정하고 최적화하는 내용은 이 책의 범위를 벗어나지만, 간단한 설명을 통해서 임
           베디드 환경에서 NFS를 어떻게 활용하는지 알아보도록 하자. 이 장의 마지막에 있는
           9.11.1절에 있는 참고 자료에서 NFS-하우 투（Howto) 문서를 포함해서 NFS에 대한 자세
           한 자료들을 찾아볼 수 있다．

           NFS를 사용할 수 있는 개발 시스템은 네트워크 파일 시스템 (NFS）을 통해서 외부로 노출시
           킬 디렉터리 목록을 담고 있는 파일을 하나 가지고 있다. 레드햇이나 기타 배포판에서 이 파
           일은 /etc 디렉터리에 위치하고 있으며 exports라는 이름을 가지고 있다. ［리스트 9-12]
           는 임베디드 개발에 사용되는 시스템에서 사용될 만한 /e七C /expor七S 파일의 내용을 보여
           주고 있다．

           （리스트 9-12) /etc/ex口orts의 내용


              $ cat letciexports
              # /etc/exports
              /honie/chri s/ sandbox/ coyote- target 乂rw, sync, no_ root_squash)
              /home/ch서s/workspace 乂r네，sync, no_ro야_squash)
              $



 298
                                                          파일 시스템   Chapter 9



      이 파일에는 리눅스 개발 시스템 상의 두 개의 디렉터리 이름이 있다. 첫 번째 디렉터리는
      ADI 엔지니어링 코요테 참고용 보드를 위한 타깃 파일 시스템을 담고 있는 디렉터리이고，
      두 번째 디렉터리는 대상 임베디드 시스템을 위한 프로젝트들을 담고 있는 일반 작업용 디렉
      터리이다. 이런 구성은 임의로 만들어 본 것이고 독자는 자신에게 맞도록 변경하면 될 것이다．

      NFS를 사용할 수 있는 임베디드 시스템에서 다음 명령어를 통해서 서버 측에서 노출시킨
      디렉터리인 . . . /T寸orkspace 디렉터리를 원하는 위치에 마운트시킬 수 있다．

         $ mount -t nfs pluto:/home/chris/workspace /workspace


      이 명령어에서 몇 가지 중요한 부분을 주의하자. 여기서는 원격（히毗0라는 이름을 갖는 시스
      템）의 디렉터리를 로컬11) 마운트 지점인 디렉터리 /workspace에 마운트하도록 명령을 내
      리고 있다. 우선 이 문법이 동작하기 위해서는 대상 임베디드 시스템이 두 가지 조건을 만족
      해야 한다. 먼저 , 타깃 시스템에서 plu切라는 장치 이름을 인식할 수 있어야 한다. 즉, 심볼
      릭 이름을 해석할 수 있어야 한다. 이를 위한 가장 쉬운 방법은 타깃 시스템의 /e七c/hosts
      에 이 항목을 넣어두는 것이다. 이렇게 하면 네트워크 서브시스템이 해당 심볼릭 이름을 그
      에 맞는 'P 주소로 변환할 수 있다. 타깃 시스템의 /e七c/hosts 파일에는 다음과 같은 항목
      이 추가될 것이다.

         192.168.10. 9   pluto


      두 번째 조건은 임베디드 타깃이 최상위 디렉터리에 /workspace라는 디렉터리를 가지고
      있어야 한다는 것이다. 이 디렉터리가 바로 마운트지점이다. 방금 본 마운트 명령어는 NFS
      서버상의 /home/chris/workspace 디렉터리의 내용을 임베디드 시스템의 加orkspace
      경로에서 사용할 수 있게 해 준다．

      이 방법은 특히 교차H개발 환경에서 매우 유용하다. 독자가 임베디드 장치를 위한 큰 프로젝
      트에 참여하고 있다고 한번 생각히1 보자. 기본적으로 프로젝트 내의 파일을 일부 수정할 때
      마다 그 어플리케이션을 대상 시스템에 옮겨서 테스트 및 디버깅해야 한다. 이때 NFS를 이
      용하면, 즉 자신의 시스템에서 NFS로 노출시킨 디렉터리에서 작업한다고 가정하면 새로 컴
      파일된 프로젝트 파일을 이 디렉터리에 별도로 업로드할 필요 없이 바로 타깃 임베디드 시스
      템에서 그 디렉터리에 접근할 수 있다. 이 방법은 개발 속도를 엄청나게 빠르게 해 준다．


11) ［역자주） 원격 디렉터리의 반대 의미로 로컬（1(玭I) 디렉터리， 즉 같은 시스템 상에 존재하는 것을 로컬이라고 한다．


                                                                         299   I
      i1
             Embedded Linux Primer




9.7.1 NFS를 이용한 루트 파일 시스템1
           프로젝트를 빌드하고 변경하는 자신의 작업 공간을 바로 대상 임베디드 시스템으로 마운트하
           면 소스 레벨에서 디버깅을 할 때 변화된 최신 소스 코드를 타깃 시스템에서 바로 접근할
           수 있기 때문에 , 개발 과정과 디버깅을 하는 데 상당한 도움이 된다. 특히 대상 시스템에서
           사용할 수 있는 자원이 극히 제한된 경우에 유용하게 사용할 수 있다. 그리고 임베디드 시스
           템을 위한 루트 파일 시스템 전체를 NFS 서버에서 마운트하는 경우에 특히 위력을 발휘한
           다. ［리스트9-12］에서 코요테 타깃을위한 항목을 보자. 개발시스템에 있는 이 디렉터리는
           타깃 아키텍처에서 사용할 수 있는 파일을 수백 개에서 수천 7긔1 이상 담을 수 있다.

           선두 업체들이 제공하는 리눅스 배포 버전은 대상 아키텍처를 위해서 컴파일 및 테스트를 마
           친 수만 개에 딜하는 파일을 포함하고 있다. 하나의 예시로 ［리스트 9-13］은［리스트 9-12]
           에서 본 코요테 타깃 디렉터리의 내용을 나타낸 것이다．

           ［리스트 9-13] 타깃 파일 시스템 사용량 통계


              $ du 느h 寸max- depth=1
              724M    ./usr
             4. 0K    ./opt
             39M     ./l ib
             12K     ./dev
             27M     ./var
             4. 0K    ./tmp
             3. 6M   ./boot
             吼OK     . Iwo마；space
             1. 8M   ./etc
             4. 0K   ./home
             4. 0K   ./mnt
             8. 0K   ./root
             29M     ./bin
             32M     ./sbjn
             4. 0K   ./proc
             64K     ./share
             85 5M
             $
             $ find -type f I 닙C ]




300
                                                                           파일 시스템   Chapter 9



이 타깃 파일 시스템은 ARM 아키텍처를 위한 1기가바이트에 가까운 바이너리 파일들을 가
지고 있다. 이 목록에서 볼 수 있듯이 이 파일 시스템은 29.000개 이상의 바이너리 파일 및
구성 파일, 문서 파일을 가지고 있다. 이 정도 크기는 일반적인 임베디드 시스템에 장착되어
있는 플래시 장치에 다 넣기 어려울 정도로 많은 양이다．

이것이 바로 NFS 루트 파일 시스템의 장점이다. 개발을 목적으로 할 때 리눅스 워크스테이
션에서 쓸 수 있는 익숙한 툴과 유틸리티를 임베디드 시스템에서도 사용할 수 있게 된다면
개발 효율성을 상당히 높일 수 있다. 커맨드 라인 툴 및 개발 유틸리티를 잘 활용하면 개발
중에 상당한 시간을 절약할 수 있기 때문이다. 이런 유용한 툴에 대해서는 13장, "개발 도구"
에서 좀 더 알아보도록 하자．

임베디드 시스템에서 부팅 시점에 NFS를 통해서 루트 파일 시스템을 마운트하는 것은 상대
적으로 간단하다. 먼저 , 대상 커널을 NFS를 지원하도록 구성해야 한다. 그리고 NFS 원격
디렉터리를 루트 파일 시스템을 마운트할 수 있도록 하는 구성 옵션이 별도로 있다. ［그림
9-3］의 예를 보자．

F扼 Qpt幻os       je如

                                                  多       目        曳
              Load    Save     Saig柶       Sr求t   Fufi   C여a口se   Expand

冷西OO5    "




  ' Misce(Ianeous 쪄esystems
  !7 Ne佃O比 F켜e Systems
    口 回 NFS 同a system su꺼刈t
             回마ovide NFSv3 ci油it 5UppO(t
             口 帥너血 NFSv4 ci沌心U머均rt 乍XPER쌔ENTAL)
             口 세咐 d畔t FfO 00 NFS 꿰en (EXPERIMENTAL)
        口 NFS server supp아t
        깐2 Root fite system on NFS
        口 Secure RPC: Ke由em巧 V macha,甘sm (EXPERIMENTAL)
        ri Spcuro RPC, SPKMI mechanism (FXPFRIMFNTAI 1
                                             i
I 그림 9-3 NFS 관련 커녈 설정


NFS 파일 시스템을 지원하도록 하는 항목이 선택된 것을 볼 수 있다. 그리고 "Root file
system on NFS", 즉 "NFS를 통해서 루트 파일 시스템을 사용함'도 선택되어 있다. 이 커
널 구성 옵션을 선택한 다음에 남은 일은 NFS 서버를 어디서 찾아야 하는지 그 정보를 알려
주는 것이다. 이를 위해서 몇 가지 방법을 이용할 수 있는데 , 타깃 아키텍처와 어떤 부트로더
를 사용하는지에 따라서 달라진다. 최소한 커널 커맨드 라인 문자열을 이용하면 II) 주소와


                                                                                         301 1
 難n 1      Embedded Linux Primer




         서버에 관한 정보를 파라미터로 커널에 넘겨줄 수 있다. 보통 다음과 같은 커널 커맨드 라인
         을 이용할 것이다．

           console=ttyS0, 115200 作）=bootp root=/dev/nfs


         이 설정은 커널로 하여금 루트 파일 시스템을 NFS를 통해서 마운트할 것이고, 관련된 정보
         （서버 이름, 서버의 II) 주소, 마운트할 디렉터리 위치）를 BOOTP 서버에서 가져오도록 한
         다. 이렇게 하는 것은 프로젝트의 깨발 단계에서 흔히 사용되는 아주 유용한 방법이다. 만약
         에 정적으로 타깃 시스템의 'P 주소를 설정한다면 커널 커맨드 라인 파라미터는 다음과 같은
         형태가 돼야 한다．



           consol e=ttySo, 115200                                           \
           ip=192. 168. 1. 139: 192 .168. 1. 1:192. 168.1.1: 255. 255. 255. 0: coyotel: eth0: off   \
              nfsroot=192.168.1.1: /home/ chrjs/ sandbox/ coyote- target           \
              root=/dev/nfs




         물론 위 파라미터는 모두 한 줄혀］ 입력되어야 한다. ip= 파라미터는 . . . /net/ipv4/
         ipconfig.c어］ 정의되고 있고, 다음과 같이 한 줄에 모두 키술하는 문법을 갖는다．



           ip=<client- ip> :<server-lp> :<gw-ip> :<netmask> :<hostname> :<device> :<PRoTo>



         여기서 client-ip는 타깃 시스템의 I ') 주소를 넣는다. server-ip는 NFS 서버의 주소
         를 나타낸다. 그리고 gw-ip는 게이트웨이（라우터）를 나타내는데 이 예에서는 server-ip
         가 다른 서브넷（subnet)12）어］ 존재한다. 넷 마스크（netmas k）는 'P 주소가 어떤 클래스13)
         를 이용하는지를 정의한다. m>S七name은 대상 호스트 이름을 나타내는 문자열이다．
         device는 ethO과 같은 리눅스 장치 이름을 나타낸다. 그리고 PROTO는 초기 'I) 파라미터
         를 얻는 데 사용되는 프로토콜을 정의한다.



12) （역자주） 햐I-；땍 네트워크를 작은 단위의 네트워크로 분리할 수 있다. 이 분리된 네트워크를 서브넷이라고 한다．
13) ［역자주） 'P叫 주소 쳬계에는 A. B, C. D의 내 종류의 클래스를 갖는다. http://en. 毗｛恥dia. org/wild/C岫帥止network를 참고
   하자．
                                                                       파일 시스템          Chapter 9




9.8 의사 파일 시스템1
    커널 구성 메뉴를 보면 의사 파일 시스템（Pseudo File Systems）이라는 항목 아래에 몇
    개의 파일 시스템이 있는 것을 볼 수 있다. 이 파일 시스템들은 다양한 분야에서 유용하게
    활용할 수 있다. 더 자세히 알고 싶다면（특히 proc 파일 시스템에 대해서） 반나절쯤 투자해
    서 이 유용한 파일 시스템 이곳저곳을 둘러보기 바란다. 더 읽어 볼 만한 자료는 이 장 뒤편
    에 있는 9.11.1절에 있는 참고 문헌들을 참고하자．


9.8.1 Proc 파일 시스템
    /proc라는 파일 시스템 이름은 원래의 용도, 즉 리눅스 시스템에서 커널이 각각의 실행중인
    프로세스에 대한 정보를 교환할 수 있도록 해 주는 인터페이스에서 유래된 것이다. 하지만
    머지않아 프로세스 정보보다 더 많은 정보를 제공하도록 발전했다. 여기서는 일부 핵심적인
    것들만 소개하고, /proc 파일 시스템 전체를 살펴보는 것은 숙제로 남기도록 하겠다．

    proc 파일 시스템은 사실상 모든 리눅스 시스템 , 가장 간단한 리눅스 시스템은 물론이고 임
    베디드 시스템에서도 없어서는 안 될 파일 시스템이 되었다. 사용자가 이용하는 상당수 기능
    들이 /proc 파일 시스템의 내용을 이용해서 동작하고 있다. 예를 들면, moun七 명령어를
    아무런 인자（파라미터） 없이 실행하면 현재 시스템에 활성화된 마운트 지점들의 목록을 보여
    주는데 , 바로 /proc/mounts의 정보를 통해서 출력하는 것이다. 만약에 /proc 파일 시스
    템을 사용하지 못하는 경우에는 moun七 명령은 아무런 출력 없이 조용히 끝날 것이다. ［리스
    트 9-14］는 ADI 엔지니어링 보드 상에서 mount 명령을 실행시켜 본 것이다．

    ［리스트 9-14] mount 명령어의 /proc 의존성


       # mount
       rootfs on / type rootfs (rw)
       /dev/ root on / type nfs
       ( rw , v2 ! rsize=4096, wsize=4096, hard, udp, fbi ock, addr=192. 168. 1. 19)
       tmpfs on /dev/ shm type tmpfs (rw)
       /proc on /proc type proc (rw, nodiratime)

      < Now unmount proc and try again . . .>




                                                                                            303 1
     二    Embedded Linux Primer




           # umount /proc
           # mount
           #



      ［리스트 9-14］에서 /proc 자체도 proc 형식으로 /proc라는 마운트 지점에 마운트된 파
         일 시스템으로 목록에 나오는 것을 알 수 있다. 시스템에서 /proc 파일 시스템을 마운트하
      기 위한 위치로서 , 최상위 디렉터리에 /proc라는 마운트 지점14）을 반드시 가지고 있어야
         한다. 그리고 /proc 파일 시스템을 마운트하기 위해서는 다른 파일 시스템과 마찬가치로
      mount 명령을 이용한다．

           $ mount -t proc /proc Iproc


      mount 명령어의 일반적인 사용법은, man 페이지를 보면 moun七 ［寸 fstype] 마운트할 것
      마운트할 위치이다. 방금 전에 mount 명령을 호출했을 때 /proc 대신에 다음과 같이 none을
      넣을 수도 있다．

           $ mount -t proc none /proc


         위 명령은 이전에 호출한 것보다 덜 이상하1 보인다. /proc 파일 시스템이 의사 파일 시스템
      이고, 실제 물리적인 장치가 존재하지 않기 때문에 마운트할 것 항목은 꼭 넣지 않아도 된다．
      하지만 이전 예제처럼 여기에 /proc라고 입력하면 /proc라는 파일 시스템을 /proc라는
      디렉터리（더 정확히는 /proc 마운트 지점）에 마운트시킨다는 점을 환기시킬 수 있다．

      물론 지금은 /proc 파일 시스템 기능이 명확해 보이겠지만, 먼저 커널 구성에서 활성화되어
         있어야 사용할 수 있다. 이 구성 옵션은 File Systems 메뉴 항목 아래의 의사 파일 시스템
      항목 아래에 있는 메뉴에서 볼 수 있다．

      현재 리눅스에서 실행중인 사용자 프로세스는 /proc 파일 시스템에서 하나의 항목으로 표
      현된다. 예를 들어 , 6장에서 소캐한 mni七 프로세스는 프로세스 Id가 항상 1이다. /proc
         파일 시스템에서 프로세스는 PIT) 숫자를 이름으로 하는 디렉터리로 표현된다. 그래서 PID
         1을 가진 mni七 프로세스는 /proc/i 디렉터리로 표현되는 것이다. ［리스트 9-15］에는 우
      리 코요테 보드에서 이 디렉터리의 내용을 보여 주고 있다．

14) 사실 /pn乂 파일 시스템을 시스템의 어디에도 마운트시킬 수 있다. 하지만 모든 유틸리티 (m에nt를 포함혜서）가 pr（兀 파일 시스
    템이 /proc에 마운트되어 있을 거라고 가정하고 동작한다．
                                                            파일 시스템   Chapter 9



［리스트 9-15) /proC 파일 시스템의 in仕 프로세스 항목


  # is -i /proc/1
  total 0
  -r           1 root    root   0 Jan   1 00: 25 auxv
  -r- -r- -r   1 root    root   0 Jan   1 00: 21 cmdline
  lrwxrwxrwx   1 root    root   0 Jan   1 00: 25 cwd -> /
  -r           1 root    root   0 Jan   1 00: 25 environ
  lrwxrwxrwx   1 root    root   0 Jan   1 00: 25 exe -> /sbin/init
  dr-x         2 root    root   0 Jan   1 00: 25 fd
    r- -r- -r  1 root    root   0 Jan   1 00: 25 maps
    rw            1 root root   0 Jan   1 00: 25 mem
  -r- -r- -r      1 root root   0 Jan   1 00: 25 mounts
  -rw-r- -r- 小    1 root root   0 Jan   1 00: 25 oom_adj
  -r- -r- -r      1 root root   0 Jan   1 00: 25 oom_score
  lrwxrwxrwx      1 root root   0 Jan   1 00: 25 root -> /
  -r- -r- -r      1 root root   0 Jan   1 00: 21 stat
                  1 root root   0 Jan   1 00: 25 statm
                  1 root root   0 Jan   1 00: 21 status
  dr- xr- xr-x    3 root root   0 Jan   1 00: 25 task
  -r- -r- -r- -   1 root root   0 Jan   1 00: 25 wchan



/proc 파일 시스템에서 실행중인 프로세스에 관련된 항목에는 매우 유용한 정보, 특히 프로
세스를 분석하고 디버깅하는 데 유용한 정보가 포함되어 있다. 예를 들면, cmdline이라는
항목에는 프로세스를 실행시킬 때 사용한 커맨드 라인 문자열을, 함께 사용된 인자도 포함해
서 가지고 있다. cwd와 roo七 디렉터리에는 프로세스의 작업 디렉터리와 현재 디렉터리의
위치를 가지고 있다．

시스템 디버깅에 사용할 만한 유용한 항목으로 maps라는 항목이 있다. 여기에는 프로그램에
할당된 가상 메모리 세그먼트의 목록과 그 각각의 속성이 함께 나열되어 있다. ［리스트
9-16］은 mnit 프로세스의 加roc/ 1/maps의 내용을 나타낸 것이다．

［리스트 아］6) in什 프로세스의 프로세스 메모리 세그먼트


  # cat /proc/1/maps
  00008000-0000f000 r- xp 00000000 00: 0a 9537567     /sbin/init
  00016000-00017000 rw- p 00006000 00: 0a 9537567     /sbi n/i nit
  00017000-000lb000 rwxp 00017000 00: 00 0
         Embedded Linux Primer



         40000000-40017000 r-xp 00000000 00: Oa 9537183   /lib/ ld-2. 3. 2. so
         40017000-40018000 rw-p 40017000 00: 00 0
         4001f000-40020000 rw-p 00017000 00: 0a 9537183   /1ib/ld-2. 3. 2. so
         40020000-40141000 r-xp 00000000 00: oa 9537518   /1化/libc- 2. 3. 2. so
         40141000-40148000 ---p 00121000 00: 0a 9537518   /1ib/1ibc- 2. 3. 2. so
         40148000-4014d000 rw-p 00120000 00: 0a 9537518   /1ib/1ibc- 2. 3. 2. so
         4014d000-4014f000 rw-p 4014d000 00: 00 0
         befeb000-bf000000 rwxp befeb000 00: 00 0
         #



       이 유용한 정보는 쉽게 이해할 수 있을 것이다. 먼저 처음 두 개의 항목에 i-nj-七 프로세스를
       위한 프로그램 세그먼트가 있는 것을 볼 수 있다. 그리고 i-nit 프로세스에서 사용되는 공유
       라이브러리에서 사용되는 메모리 세그먼트를 볼 수 있다. 각 항목의 형식은 다음과 같다．

         vmstart-vmend attr pgoffset devname mnode filename

       여기서 vmstart와 vmend는 각각 가상 메모리 주소의 시작과 끝을 나타낸다. 그리고 a七tr
       은 해당 메모리 영역에 대한 속성 값, 예를 들어 , 읽기 , 쓰기 , 실행 가능한지 그리고 공유
       가능한 영역인지를 보여 준다. f珂（)ffse七은 메모리 영역의 페이지 오프셋（커널 가상 메모리
       파라미터）을 나타낸다. 그리고 ><><: ><>< 형태로 나타내는 devname은 메모리 영역에 할당된
       장치 ID를 커널이 인식하는 형태로 나타낸 것이다. 즉, 어떤 메모리 영역이 어떤 파일과도
       연결되지 않고, 또 어떤 장치와도 연결되지 않은 경우에는 00: 00이 된다. 마지막 두 개의
       항목은 메모리 영역에 연결된 파일 이름과 그 mode를 나타낸다. 만약에 연결된 파일이나
       in이扼가 없다면 0으로 표시된다. 보통 데이터 세그먼트가 모두 0으로 표시된다．

       이 외에도 각 프로세스에 대한 유용한 /proc 파일 시스템 항목이 있는데 , S七atus 항목의
       경우에는 부모 프로세스의 PID, 사용자와 그룹 II) 값들, 가상 메모리 사용 정보, 시그널 정
       보, 수용 능력 정보（capabi砒扼S) 등을 포함해서 현재 실행중인 프로세스에 대한 유용한 상
       태 정보를 갖고 있다. 더 자세한 내용은 이 장 끝의 참고 문서에서 얻을 수 있다．

       이 외에도 /proc 파일 시스템에서 자주 이용되는 항목으로는 cpuinfo, meminfo 그리고
       version이 있다. cpuinfc) 항목은 커널이 인식하는 현재 시스템의 프로세서（들）에 대한
       속성을 갖고 있다. meminfo 항목은 시스템 전체 메모리에 대한 통계를 유지하고 있다. 마지
       막으로 version 항목은 리눅스 커널 버전 문자열과 커널을 빌드할 때 사용한 컴파일러 및
       시스템에 대한 정보도 같이 가지고 있다．


I 3此
                                                                    파일 시스템   Chapter 9



      /proc 파일 시스템에 있는 유용한 항목들의 상당수는 커널이 제공하는 것들이다. 여기서는
     이 유용한 서브시스템의 일부분만 살짝 맛보았다. 그리고 많은 유틸리티 프로그램이 /proc
     파일 시스템에 있는 정보를 추출해서 가공하도록 만들어져 있다. 그 중에서 가장 인기 있는
     것 두 개가 바로 top과 PS인데 , 아마 대부분의 리눅스 개발자라면 매우 익숙할 것이다. 이
     유틸리티에 대해서는 13장에서 소개할 것이다. /proc 파일 시스템을 이용하는 다른 유용한
     유틸리티로는 free, pkill, pmap, uptime 등이 있다. 자세한 내용을 위해서는 procps 패
     키지를 살펴보기 바란다.


9.8.2 svsfs
      /pr（兀 파일 시스템과 같이 sysfs도 실제 물리적인 장치를 사용하지는 않는다. 대신 실제
     디바이스를 파일로 표현하는 것과 같은 커널 내부의 객체에 대한 모델을 제공하고, 장치와
     장치 드라이버（디바이스 드라이버）를 연결시키기 위한 방법을 제공한다. 일반 리눅스 배포
     버전에 있는 일부 프로그램은 sysfs어］ 있는 정보를 이용해서 동작하도록 되어 있는 것도
     있다．

     sysfs의 디렉터리를 살펴보면 sysfs7} 외부로 노출시키고 있는 객체에는 어떤 것들이 있
     는지 볼 수 있다. ［리스트 9-17］에는 코요테 보드에서의 /SYS 디렉터리 내용을 보여 주고
     있다．

     ［리스트 9-17) /sys 디렉터리의 내용

        # dir /sys
        total 0
        drwxr-xr- x    21 root   root   0 Jan   1 00:00 block
        drwxr-xr- x     6 root   root   0 Jan   1 00: 00 bus
        drwxr-xr- x    10 root   root   0 Jan   1 00: 00 class
        drwxr-xr- x     S root   root   0 Jan   1 00: 00 devices
        drwxr-xr- x     2 root   root   0 Jan   1 00: 00 firmware
        drwxr-xr- x     2 root   root   0 Jan   1 00: 00 kernel
        drwxr- xr- x    5 root   root   0 Jan   1 00: 00 module
        drwxr- xr- x    2 root   root   0 Jan   1 00: 00 power
        #




                                                                                   307 1
籌瑟 N 二    Embedded Linux Primer



       이 내용에서 보는 것처럼 , sysfs는 시스템 버스까지 포함한 시스템 장치의 주요 항목에 대
         한 디렉터리를 가지고 있다. 예를 들어 , block 하위 디렉터리 아래에는 블록 디바이스에 해
         당하는 내용을 담고 있는 각각의 하위 디렉터리가 있다. 다른 디렉터리도 마찬가지로 그 항
         목에 해당하는 내용이 다시 하위 디렉터리 형태로 구성되어 있다．

         sysfs어］ 저장되어 있는 정보는 대부분 사람보다는 컴퓨터가 이해하기 쉽도록 되어 있다．
         예를 들어 , PCI 버스에 물려 있는 디바이스는 /sys/bus/pci 디렉터리 아래에서 찾을 수
         있을 것이다. 우리 코요테 보드에서는 PCI 장치가 딱 하나 연결되어 있는데（이더넷 카드가
         연결되어 있다）, /sys/bus/pci 디렉터리에는 다음과 같은 형태의 파일이 존재하게 된다．



           # is /sys/ bus/pci/ devices/
           0000: OO: Of. O -> . ./. ./. ./devices/pci0000: OO/0000: OO: Of. O



       이 파일은 실제로는 sysfs 디렉터리 구조 내의 다른 파일을 가리키는 심볼릭 링크이다. 그
       리고 위 출력 내용은 편의상 is의 출력을 한 줄어］ 모두 넣을 수 있도록 일부를 생략한 것이
       다. 심볼릭 링크의 이름은 커널이 PCI 버스를 커널 방식으로 표현한 것이다. 그리고 이 링크
         는 다시 (PCI 버스 방식으로） PCI 장치를 가리키는 pci0000: OO이라는 디렉터리를 가리키
         는데 , 이 디렉터리에는 이 PCI 장치에 대한 속성을 나타내는 파일을 담고 있다. 파일 이름도
       매우 난해하지만, 데이터는 훨씬 더 이해하기 어려운 형식을 취하고 있다．

         그래서 sysfs 파일 시스템의 디렉터리 구조를 탐색하기 위해서 사용할 수 있는 systool이라
         는 유용한 유틸리티가 있다. 이 유틸리티는 소스포지（source如rge.net）에 있는 프로젝트인
         sysfsutils 패키지에 포함되어 있다. 다음 내용은 sys切아로 방금 설명한 PCI 버스에 대해
         서 출력했을 때의 결과를 나타낸 것이다．



           $ systooi -b pci
              Bus = "口ci "
              0000: OO: Of. 0 8086: 1229




 308
                                                 파일 시스템   Chapter 9




      여기서도 다시 한 번 버스와 디바이스（0f）에 대한 커널식 표현을 볼 수 있다. 하지만 이번에
      는 유틸리티가 sysfs에서 장치에 대한 속성을 저장하고 있는 /sys/devices/
      pci0000: OO 디렉터리에 제공자 ID侶086은 인텔）와 디바이스 ID(1229는 eeprol00 이
      더넷 카드）를 알아내서 같이 표시해 주는 것을 볼 수 있다. 아무런 인자도 없이 실행했을 때
      는 최상위 시스템 구조를 정리해서 출력한다. ［리스트 9-18］은 이 유틸리티를 코요테 보드
      에서 실행한 결과이다．

      ［리스트 9-18] systool 실행 결과


         $ systool
         Supported sysfs buses:
                i2c
                i de
                pci
                platform
         Supported sysfs classes:
                block
                I 2c-adapter
                12c- dev
                1 npul
                mem
                misc
                net
                pci_bus
                tty
         supported sysfs devices:
                pci0000: OO
                platform
                system




      위 내용을 통해서 sysfs를 이용해 다양한 시스템 관련 정보를 얻을 수 있다는 것을 알 수
      있다. 그리고 많은 유틸리티들이 시스템 장치의 특성을 알아내거나 전원 관리 및 督플러그
      15) (hot-plug) 기능 등의 시스템 정책을 결정하는 데 sysfs의 정보를 이용한다．




15) （역자주） 시스템이 동작중일 때 장치를 연결하거나 제거 가능하도록 하는 기술
        Embedded Linux Primer




9.9 기E十 파일 시스템1
      리눅스는 그 외에도 많은 파일 시스템을 지원한다. 지면상 모든 파일 시스템을 소개할 수는
      없고, 임베디드 시스템에서 자주 사용되는 중요한 파일 시스템 몇 가지만 알고 넘어가도록
      하자．

      ramfs 파일 시스템은 이 모듈을 구현하고 있는 리눅스 소스 코드 자체가 의미 있는 파일 시
      스템이다. ［리스트 9-19］는 이 코드의 처음 몇 줄을 나타낸 것이다．

      ［리스트 9-19) ramfs 모듈 소스 코드의 주석 부분

         ／必
              * Resizable simple ram filesystem for Linux.
              央


              ""Copyright (C) 2000 Linus Torvalds.
              "             2000 Transmeta Corp.

              受Usage limits added by David Gibson, Linuxcare Australia.
              * This file is released under the GPL.
              六／
         /／央

              * NOTE! This filesystem is probably most useful
              必 not as a real filesystem, but as an example of
              肯how virtual filesystems can be written.
              卉

              * It doesn 't get much simpler than this. Consider
              * that this file implements the full semantics of
              * a PosIx-compliant read-write filesystem.



      이 모듈은 가상 파일 시스템을 어떻게 구현하는지 보여 주는 핵심 예제로 작성된 것이다. 최
      신 리눅스 커널에서 볼 수 있는 ramfs 파일 시스템과 램디스크의 가장 큰 차이점은 사용함에
      따라서 그 크기가 자동으로 줄어들거나 늘어날 수 있는지 여부이다. 램디스크는 그런 능력이
      없지만 ramfs는 그런 능력을 가지고 있다. ramfs의 소스 코드는 매우 작고 잘 짜여 있다．
      교육적으로 매우 가치 있는 코드라서 여기서 소캐했다. 관심 있는 독자는 한번 공부해 보기
      바란다．


 引0
                                                          파일 시스템   Chapter 9




   tmpf s 파일 시스템은 ramfs와 비슷하다. ramfs와 같이 七mpfs의 모든 내용은 커널 가상
   메모리 안에 저장되어 있어서 전원이 끊기거나 재부팅되면 tmpfs의 내용이 모두 사라지게
   된다. tmpfs 파일 시스템은 임시 파일을 만들어 사용할 때 유용하다. 필자의 경우도 미디
   (n丘di）와 오디오 어플리케이션에서 속도를 높이기 위해서 오디오 서브시스템에서 필요로 하
   는 임시 파일을 생성하고 삭제하는 것을 七mpfs를 이용해서 하고 있다. 또한 이렇게 하는
   것이 재부팅 시에 모든 내용이 사라치기 때문에 ／七mp 디렉터리를 깨끗하게 유지할 수 있는
   좋은 방법이기도 하다. 七mpf s를 마운트하는 것은 다른 가상 파일 시스템과 비슷하다．

     # mount -t tmpfs /tmpf s /tmp


   /pro小斗 같은 파일 시스템과 마찬가지로, 위 명령에서 /tmpfs의 첫 번째 파라미터로 사용
   된 것은 아무 의미가 없다. 즉, 아무런 내용이나 넣어도 동작에는 영향을 주지 않는다. 하치
   만 tmpf s라고 입력하면 어떤 파일 시스템을 마운트하는지 상기시킬 수 있을 것이다．



9.10 간단한 파일 시스템 만들기
   간단한 파일 시스템 이미지를 만드는 것은 쉽다. 여기서는 예제로 리눅스 커널의 루프 백
   (loopback) 디바이스를 이용해 보겠다. 루프 디바이스는 일반 파일을 블록 디바이스처럼 사
   용할 수 있도록 해 준다. 요약하면 우리는 일반 파일에 파일 시스템을 구성해서 리눅스의 루
   프백 디바이스를 이용해서 다른 블록 디바이스를 마운트하는 것과 같은 방식으로 그 파일을
   마운트해 볼 것이다．

   간단한 루트 파일 시스템을 만들어 보기 위해서는 먼저 모두 0으로 채워져 있는 고정된 크기
   의 파일을 준비해야 한다．

     # dd if= /dev/ zero of= ./my-new- fs- image bs=lk count=512


   위 명령은 모두 0으로 채워진 512KB짜리 파일을 하나 만든다. 파일에 모두 0을 채우는 이
   유는 나중에 압축을 할 때 압축률을 높이기 위함이고, 또한 파일 시스템 내에 사용되지 않는
   부분에 대해서 일관된 데이터를 채워두기 위함이다. dd 명령을 사용할 때 주의하기 바란다．
   dd 명령어를 아무런 제한（coun七니 없이 설정하거나 또는 알맞지 않은 범위를 지정해서 사
   용하면 하드디스크를 침범해서 시스템 충돌이 일어날 수도 있기 때문이다. dd는 강력한 툴이
   지만, 그에 걸맞게 조심해서 사용해야 한다. root 권한에서 dd 명령을 아무런 인자 없이 그
   냥 실행하면 파일 시스템을 파괴시켜 버린다．

                                                                         引］ I
          Embedded Linux Primer



        새로운 이미지 파일이 준비되면 이 파일을 포맷해서 알맞은 파일 시스템 구조를 내부에 갖도
        록 만들어야 한다. 이 예제에서는 ext2 파일 시스템으로 구성했다. ［리스트 9-20］에 자세한
        절차가 나와 있다．

        ［리스트 9-20) ext2 파일 시스템 이미지 만들71

          # /sbin/mke2fs ./my-new- fs-image
          mke2fs 1. 35 (28-Feb- 2004)
          ./my-new-fs-image is not a block special device.
          Proceed anyway? (y,n) y
          Filesystem label=
          OS type: Linux
          Block size=1024 (log=0)
          Fragment size=1024 (log=O)
          64 mnodes, 512 blocks
          25 blocks (4. 88%) reserved for the super user
          First data block=1
          1 block group
          8192 blocks per group, 8192 fragments per group
          64 i nodes per group
          writing mnode tables: done
          writing superbiocks and filesystem accounting information: done

          This filesystem will be automatically checked every 24 mounts or
          180 days, whichever comes first. use tune2fs -c or -i to override.
          #



        dd와 같이 mke2fs 명령에 역시 시스템을 망가트릴 수 있기 때문에 사용할 때 주의를 기울여
        야 한다. 이 예제에서는 mke2fs 명령어를 통해서 하드 디스크 파티션（블록 디바이스） 대신
        에 의도한 대로 하나의 파일을 포맷하도록 했다. 그래서 mke2fs 역시 포맷하려는 대상이
        블록 디바이스가 아닌 것을 감지해서 그래도 진행할 것인지를 물어보고 있다. 확인 후에
        mke2fs는 이 파일에 ext2 슈퍼블록（superbiock）과 파일 시스템을 위한 자료 구조를 기록
        해 넣는다． 그렇게 하면 리눅스 루프백 디바이스를 이용해서 이 파일을 마치 블록 디바이스
        인 것처럼 마운트해서 사용할 수 있게 된다．

          # mount -o loop ./my-new-fs-image /mnt/ flash




I 312
                                            파일 시스템   Chapter 9



    이 명령은 my-ne小f s-image라는 파일을 /mn七／flash라는 마운트 지점에 하나의 파일
    시스템으로 마운트한다. 이 마운트 지점의 이름은 중요하지 않고 존재하는 디렉터리 어디든
    자신이 원하는 지점에 마운트할 수 있다. 마운트 지점을 위한 디렉터리를 만들기 위해서는
    mkdir을 이용하면 된다．

    새로 만든 이미지 파일을 하나의 파일 시스템으로 마운트한 후에는, 그 내용을 마음대로 바
    꿀 수 있다. 거기에 디렉터리를 만들거나 추가할 수도 있고, 디바이스 노드 등도 만들 수 있
    다. 그리고 tar를 이용해서 파일을 복사해 넣거나 다른 곳으로 옮길 수도 있다. 모든 수정된
    사항은 하나의 파일에 저장되는데 , 물론 장치의 공간을 넘지 않아야 한다. 이 방법을 이용할
    때 처음 파일 이미지를 만들 당시에 정해진 공간 크기는 나중에 다시 바꿀 수 없다는 점을
    기억하기 바란다．



9.1 ] 요약
      口 파티션이란 물리적인 장치를 논리적으로 분할한 것이다. 리눅스에서는 다양한 종류의 파
        티션을 지원한다．

      口 리눅스에서는 파일 시스템이 마운트 지점에 마운트되도록 되어 있다. 그 중에서 루트 파
        일 시스템은 ／로 나타내는 파일 시스템의 최상위에 마운트된다．

      口 인기 있는 파일 시스템인 ext2는 성숙하고 빠른 파일 시스템으로, 임베디드 시스템이나
        레드햇이나 페도라 코어 등에서 사용되는 것을 볼 수 있다．

      口 ext3 파일 시스템은 데이터 일관성 및 시스템 신뢰성을 위해써 ext2 파일 시스템 위에
        저널링을 추가한 것이다．

      口 ReiserFS는 임베디드 및 기타 리눅스 시스템에서 많이 사용되는 고성능 저널링 파일 시
        스템이다．

      口 JFFS2는 플래시 메모리를 위해써 최적화된 저널링 파일 시스템이다. 여기에는 플래시의
        수명을 길게 하기 위한 웨어 레벨링佃ear leveling）과 같은 기술이 포함되어 있다．

      口 cramfs는 작은 시스템의 ROM이나 기타 읽기 전용 프로그램이나 데이터를 담기 위한
        파일 시스템으로 가장 잘 어울리는 읽기 전용 파일 시스템이다．




                                                           313 1
 難 月1   Embedded Linux Primer



        口 NFS는 임베디드 개발자에게 있어서는 가장 강력한 개발 툴 중의 하나이다. 이 파일 시스
           템은 개발 워크스테이션의 강력한 자원을 타깃 시스템에서도 사용할 수 있도록 해1 준다．
           독자가 사용하는 임베디드 시스템의 루트 파일 시스템으로 NFS를 사용하는 것을 연구해
           보기 바란다. 편리성과 시간절약을 생각한다면 노력이 전혀 아깝지 않을 것이다．

        口 리눅스는 다양한 의사 파일 시스템을 사용할 수 있는데, 그 중에서 proc 파일 시스템이
           나 sysfs와 같은 중요한 파일 시스템에 대해서 설명했다.

        口 RAM 기반의 tmpf s 파일 시스템은 임베디드 시스템에서 다양한 용도로 사용할 수 있
           다. 기존 램디스크와 비교했을 때 가장 크게 향상된 점은 동작중어］ 동적으로 크기를 늘였
           다 줄였다 할 수 있다는 점이다.



9.11. ] 더 읽01 보기
        "Design and Implementation of the Second Extended Filesystem"
        Rmy Card, Theodore Ts'o, and Stephen Tweedie
        First published in the Proceedings of the First Dutch
        International Symposium on Linux
        http://e2fsprogs.sourceforge.net/ext2intro.html에서 볼 수 있음.


        "A Non-Technical Look Inside the EXT2 File System"
        Randy Appleton
        www,linuxgazette,com/issue2l/ext2,html


        Whitepaper: Red Hat's New Journaling File System: ext3
        Michael K. Johnson
        www, redhat, com/support/wpapers/redhat/ext3/


        ReiserFS 홈페이지
        www, namesys. corn!


        "JFFS: The Journaling Flash File System"
        David Woodhouse
        http://sources.redhat,com/jffs2/jffs2,pdf




I 314
                                                        파일 시스템    Chapter 9



cramfs 프로젝트의 README 파일
작가 서명 없음（프로젝트 제작자로 가정）
http://sourceforge.net/projects/cramfs/


NFS 홈페이지
http://nfs.sourceforge.net
Iproc 파일 시스템 문서
www.tldp.org/LDP/lkmpg/2.6/html/c712.htm


File System Performance: The Solaris OS, UFS, Linux ext3, and ReiserFS
기술 백서（A technical whitepaper)
Dominic Kay
www. sun. com/software/whitepapers/solaris10/fsperformance. pdf




                                                                         引5 1
                   10




이번 징K게서 배숄 내용

  .MTO 서비스 활성화하기

  U 卜肝D 기초

  . 卜肝D 파티션

  . 卜TE) 유틸리티

  U 요약
       日ibedded 니flux Primer




      메모리 기술 저장 장치（MTD) 서브시스템은 플래시 메모리 IC와 같은 다양한 메모리 형태
      의 장치를 지원하기 위해서 만들어진 기술이다. 시중에는 많은 종류의 플래시가 나와 있고，
      이와 함께 플래시에 데이터를 기록하는 방법도 매우 다양하다. 이는 많은 플래시가 자체적으
      로 '고성능 모드'를 고안헤서 사용하고 있기 때문이다. MTD 계층 구조는 메모리 장치가 사용
      하는 상위 레벨의 데이터 구조와 저장 형식을 하위 레벨의 장치와 관련된 복잡한 구조와 분리
      시킬 수 있도록 해 준다．

      이 장에서는 MTD 서브시스템에 대해서 소개하고, 이것을 이용하는 간단한 예제도 몇 가지
      살펴보도록 하자. 먼저 커널에서 MTD 서비스를 사용하려면 어떤 것이 필요한지를 알아볼
      것이다. 그리고 MTD 서브시스템에 대한 기본 사항을 이해하기 위한 수단으로서 MTD를
      사용할 수 있도록 구성되어 있는 개발 워크스테이션에서 몇 가지 간단한 동작을 시험해 볼
      것이다. 그리고 MTD와 JI고FS2 파일 시스템을 통합시켜 보도록 할 것이다．

      그 다음에는 MTD 계층과 관계된 파티션 개념을 소캐한다. 그리고 부트로더에서 파티션을
      만드는 예제를 자세히 알아보고, 이 파티션이 리눅스 커널에서 어떻게 인식되는지 보도록 하
      자. 또한 MTD 관련 유틸리티에 대해서 간단히 소개하고, 마지막으로 플래시에 존재하는
      JFFS2 파일 시스템 이미지를 이용해서 타깃 보드를 부팅해 보도록 하겠다．



10.1 MID 서비스 활성화하기
      MTD 서비스를 이용하기 위해서는, 커널이 MTD를 사용할 수 있도록 구성되어 있어야 한
      다. MTD를 위한 구성 옵션은 매우 다앙하고, 일부는 좀 헷갈릴 수도 있다. 다양한 구성 옵
      션을 이해하기 위한 가장 좋은 방법은 그냥 먼저 동작부터 시켜 보는 것이다. 玉/ITD 서브시스
      템이 어떻게 동작하는지와 시스템과 어떻게 맞물려 돌아가는지를 설명하기 위해서 리눅스 개
      발 시스템에서 몇 가지 예제를 실행해 보도록 하자. ［그림 10-1]은 (make ARCH=<arch>
      gconfig를 실행해서） MTD 기능을 이용하기 위해서 반드시 선택해야 하는 커널 구성 옵션
      을 선택한 화면이다. 그리고 ［리스트 10-1)은 .config 파일에서 ［그림 10-1]에서 설정한
      항목에 대한 내용을 나타낸 것이다.




13始
                                            MTD 서브시스템   Chapter 10


［리스트 ]0- 1) .config      파임의 MTD 기본 구성 옵션


   C0N FIG_MTD=y
   C0NfIG_MTD_ CHAR=y
   C0NFIG_MTD_ BL0CK=y
   C0N FIG_MTD_MTDRAM=m
   C0N FIG_MTDRAM_T0TALHSIZE= 8192
   C0NFIG_MTDRAM_ERASE_SIZE=128




맨 위에 있는 구성 옵션은 ［그림 10-1]에서 첫 번째 'Memory Technology Deveice
(MTD) support' 쳬크 박스를 선택한 결과로 나타난 것인데 MTD 서브시스템을 활성화시
키는 옵션이다. ［그림 10-1]에 있는 구성 옵션에서 선택된 그 다음 두 가치 항목은 사용자
공간에서 플래시 메모리와 같은 MTD 장치에 대해서 특별한 장치 레벨에서 접근을 할 수
있도록 할지를 선택하는 부분이다. 첫 번째（CONFIG MTD CHAR) 항목은 캐릭터 디바이스
모드에서 접근할 수 있도록 하는 옵션이다. 즉, 순차적으로 한 바이트씩 읽거나 쓰는 접근
방식을 말한다. 두 번째 (CONFIG MTD BLOCK) 항목은 블록 디바이스 모드로 MTD 장치에
접근할 수 있도록 해 주는 옵션이다. 이 방식은 모든 디스크 드라이브에서 사용되는 방식인
데 , 블록 단위의 데이터를 한번에 읽거나 쓸 수 있다. 이 두 가지 접근 모드는 익숙한 리눅스
명령어를 이용해서 플래시 메모리의 데이터를 읽거나 쓸 수 있도록 해 주는데 , 이 부분은 곧
살펴볼 것이다.

以)NFIGMTD 卜4TDRM'I 부분은 （플래시 메모리와 같은） MTD 장치가 없더라도 MTD 서브
시스템을 테스트해 볼 수 있게 해 주는 특별한 테스트 드라이버이다. 이 구성 옵션과 함께
이 램 기반의 테스트 드라이버와 관련된 파라미터가 두 7뀨 더 있는데 , 각각 장치의 크기와
삭제 단위의 크기가 그것이다. 위 예제에서는 전체 크기를 8192KB로 지정하고 삭제 단위
블록 크기는 128KB로 설청했다. 이 테스트 드라이버의 주된 목척은 플래시 장치를 에뮬러］
이트해서 MTD 서브시스템을 가지고 개발 및 테스트를 가능하도록 하는 것이다. 플래시 메
모리는 고정된 크기의 삭제 단위 블록을 가지고 있기 때문에 이 테스트 드라이버에서도 고정
된 크키의 삭제 단위 블록 개념을 사용한다. 잠시 후에 이 파라미터들이 어떻게 사용되는지
살펴보게 될 것이다．




                                                            3四 I
  難1         Embedded Linux Primer




       E艇 Qpt初ns Ue如                                       1: 11m=                                        n

              ;r       g臼          口       I          II       卜        田       中
                       山ad         Save   듸叫e        Sr如［      F너1    Collapse Exp카甘Ln

           Opt珀In              r                                                         !Name            卞
               口 回Memo斗Technol四y Device (MTD) support                                    MTD
                      口Debu四四                                                            MTD_DEBUG
                      口MTD c아)catenatr띰su啣It                                             MTD叫CONCAT
       i              口MTD口a川trot百r目S目pport                                              MTD_PART汗心NSr小
       !              User Modides A겨1 Translati川 Layers
       !              回Di畔t char device access to MTD devices                            MTD. CHAR
                      回Cac陌ng Nock device access to MTD d너ces                            MTDJLOCK      t
       !              口FTL (Flash T떼lslation Layer) support                              FTL              n
       }              口NFTL (NAND 由shTran引帥on La艸沾upport                                 NFTL
       훑              口INFTL (Inverse NAND Rash Tran引胡on녀yet) support                    INFTL            卜
       薛              口Resident Flash Disk (Rash Translation Layer) support              RED_Fri                :
       !            1卜 RAM垠아肝Ia帥1chipd加미S
                    ) Mapp四山如e匹for c脚毗cess
                    V Self-cont如ned V[ TD device ddv叫s
       {                 口Ramix PMC5S1 PCI Mezzar出比RAM card S바斗兀It                       MTD_PMC551    口，
       三                 O Uricached system RAM                                           ffD..SLRAM
       !                 口帥틔cal system RAM                                               Ml]工PHRAM        i
       }              口日Test dnver usir因RAM                                              MTD_MTDRAM
                             MTDRAM device size in K游                                    MTDRAM_TOTAL_'
                             h肝E가,AM erase hI어：ks그e in K沿 (NEW)                           MTDRAM_ERASL巴
                                                                                                           口느
       iij                                                                    苾尸 n   m   L     小 ' n'i卜j

       U 그림 ]0녀 MTD 구성


10.1. ] MTD 만들기
       최신 리눅스 스냅샷1) (snapshot)에는 모두 MTD가 포함되어 있다. 하지만 커널이 릴리즈
       된 이후에 MTD 최신 프로젝트에 추가된 기능이 더 있는 경우에 , 새로운 기능까지 포함해서
       모든 MTD 기능을 활용하고자 한다면 MTD 드라이버와 유틸리티를 새로 다운로드해서 빌
       드해야 한다. MTD 패키지에는 커널 요소와 사용자 프로그램이 모두 포함되어 있기 때문에，
       일단 MTD 패키지를 별도의 프로젝트 디렉터리에 두고 커널 소스 트리에서 이 프로젝트 디
       렉터리를 연결시키는 방식으로 사용하는 것이 좋다. 가장 간단하게 MTD와 현재 커널을 통
       합시키는 방법은 MTD 패키지에서 제공되는 스크립트를 이용하는 것이다.

       먼저 이 장의 마지막에 있는 URL을 통해서 MTD 패키지를 다운받도록 하자. 그리고는 tar
       유틸리티를 이용해서 원하는 디렉터리에 압축을 푼다. 그리고는 그 디렉터리로 들어가서

1) C역자주） cvs나 Perforce, ClearCase 등의 소스 형상 관리 시스템에서 현재 상태를 내려 받는더T 내려 받은 상태를 스냅샷이라고
 한다. 여기서는 그냥 리눅스 배포 버전이라고 생각하면 된다．
                                                       MTD 서브시스템   Chapter 10




   patchkernel. sh 스크립트를 실행시킨다. 이 스크립트는 몇 가지 옵션을 가지고 있는데，
   아무런 옵션 없이 실행하면 파라미터에 대한 자세한 사용법을 볼 수 있다. ［리스트 10-외는
   MTD의 커널 구성 요소를 설치하는 절차를 나타낸 것이다．

   ［리스트 ]0-2) MTD를 위해서 커널 패치하71


     $ ./patchkernel. sh -2 . ./sources/linux- 2.6.10-mtd
     Patching . ./sources/linux- 2. 6. 10-mtd/
     Include JFFS2 file system: jffs2
     Include JFFS3 file system (experimental) : no
     Method: ln      << will actually create symbolic links
     can we start now? [y/N] y


     $



   patchkernel . sh 스크립트를 -2 파라미터를 이용해서 실행시키는 것은 JI구FS2 파일 시
   스템을 지원하기를 원한다는 것을 나타낸다. 그리고 커널 소스 디렉터리에 대한 경로 . . /
   sources/linux寸2. 6.10-mtd를 전딜해 준다. 기본적으로 patchkernel . sh는 커널 소
   스 디렉터리에 파일을 직접 복사하지 않고, 대신 커널 소스 트리에 MTD 디렉터리를 가리키
   는 심볼릭 링크를 만들게 된다. 이 방식으로 개발용 워크스테이션에 여러 깨의 커널 버전을
   가치고 있더라도 MTD에 대해서는 단일한 프로젝트 디렉터리 하나를 공통으로 사용할 수
   있게 된다. 이와 같이 커널 소스 트리 내에 MTD에 대한 심볼릭 링크를 만들어 둠으로써 커
   널 빌드 시스템을 통해서 MTD 커널 드라이버가 커널 구성 옵션 정보도 알 수 있고, 커널과
   같이 빌드하도록 할 수 있다．



10.2 MID 기초
   이제 커널에서 기본적인 MTD 구성 옵션을 활성화시켰기 때문에 리눅스 개발 워크스테이션
   에서 MTD 서브시스템이 어떻게 동작하는지 시험해 볼 수 있다. 이전 단락에서 설정한 테스
   트 RAM 드라이버를 이용하면 MTD 장치를 이용해서 JFFS2 이미지를 마운트할 수 있다．
   9장. "파일 시스템"에서 설명한 대로 JI巾S2 이미지를 만들었다고 가정하면 이 이미지를 마
   운트해서 바로 사용해 보고 싶을 것이다. 하지만 리눅스 커널은 ext2나 다른 파일 시스템
   이미지는 루프백 장치에서 직접 마운트할 수 있지만, JFFS2 파일 시스템을 직접 마운트하


                                                                        321 1
        Embedded Linux Primer



      는 기능은 지원하지 않는다. 그래서 다른 방법을 이용해야 하는데 , 바로 ［그림 10-1］처럼
      MTD를 활성화시킨 리눅스 캐발 시스템에서 MTD RAM 테스트 드라이버를 이용하는 것이
      다. ［리스트 10쏘은 이 과정을 나타낸 것이다．

      ［리스트 ]0-3) MID RAM 장치에서 JFFS2 마운트하기

        # modprobe jffs2
        # modprobe mtdblock
        # modprobe mtdram
        # dd if= jf1s2.bin of= /dev/mtdblock0
         4690+1 records in
         4690+1 records out
        # mkdir /mnt/ flash
        # mount -t jffs2 /dev/mtdbiocko /mnt/fi ash
        # is -i /mnt/ fiash
        total 0
        drwxr- xr- x 2 root root 0 Sep 17 22: 02 bin
        drwxr- xr- x 2 root root 0 Sep 17 21: 59 dev
        drwxr- xr- x 7 root root 0 Sep 17 15: 31 etc
        drwxr- xr- x 2 root root 0 Sep 17 15: 31 home
        drwxr- xr- x 2 root root 0 Sep 17 22: 02 fib
        drwxr- xr- x 2 root root 0 Sep 17 15: 31 proc
        drws         2 root root 0 Sep 17 15: 31 root
        drwxr-xr- x 2 root root 0 Sep 17 22: 02 sbin
        drwxrwxrwt 2 root root 0 Sep 17 15: 31 tmp
        drwxr-xr- x 9 root root 0 Sep 17 15: 31 usr
        drwxr-xr- x 14 root root 0 Sep 17 15: 31 var
        #



      ［리스트 10-3］을 보면 JFFS2와 MTD 서브시스템을 사용하기 위해서 필요한 적재 가능 모
      듈을 설치한다. JFFS2 모듈을 커널에 로드한 후에는 mtdbl ock과 m七dram 모듈을 적재한
      다. 필요한 디바이스 드라이버 모듈이 모두 로드된 후에는, 리눅스 dd 명령으로 JFFS2 파
      일 시스템 이미치를 mtdblock 장치를 이용해서 MTD RAM 테스트 드라이버에 복사한다．
      여기서 MTD 블록 디바이스를 에뮬레이트 하는데 본질적으로 시스템 RA｛을 사용하고 있
      는 것이다．




322
                                                            MID 서브시스템   Chapter 10



       우리가 만든 JI고FS2 파일 시스템 이미지를 MTD 블록 디바이스에 복사한 후에는 ［리스트
       10-3］에서 나온 방식으로 mount 명령어를 이용해서 마운트해 볼 수 있다. MTD 의사H장치
       (pseudo-device）가 마운트되면 JI구FS2 파일 시스템 이미지를 원하는 대로 이용할 수 있
       다. 이 방법이 갖는 유일한 제한 사항은 이미지의 크기를 늘릴 수 없다는 것이다. 이미지의
       크기는 두 가지 요소에 의해서 결정되는데 , 먼저 MTD RAM 테스트 디바이스를 구성할 때
       최대 크기를 8MB2）로 지정했다. 두 번째는 JFFS2 이미지를 만들 때 mkfs.jffs2 유틸리티
       에 의해서 고정된 크기의 이미지가 만들어지는데 , 이미지를 만들 때 사용할 대상 디렉터리에
       어떤 내용이 들어 있는가에 따라서 이미지의 크기가 결정되는 것이다. jffs2 .bin 이미지를
       어떻게 만드는지는 9장의 ［리스트 9-9］를 다시 살펴보기 바란다．

       여기서 JFFS2 파일 시스템을 테스트해 보기 위해서 사용한 방식이 어떤 제한점을 갖는지
       이해하는 것이 아주 중요하다. 우리가 어떤 일들을 했는지 보도록 하자. 먼저 (JFFS 파일
       시스템 바이너리 이미지） 파일의 내용을 커널 블록 디바이스（/dev/mtdl끄ockO）에 복사했
       다. 그리고는 커널 블록 디바이스（/dev人n七dbiock）를 JFFS2 파일 시스템 형식으로 마운
       트시켰다. 그 뒤에 기존 파일 시스템 유틸리티를 이용해서 파일 시스템을 시험해 보고, 내용
       도 수정해 보았다. is, df, dh, my, rm, c1) 등의 유틸리티를 이용해서 파일 시스템의 내
       용을실험하고 수정했다. 하지만, 루프백 장치와는 달리 , 복사한 파일과JI叩S2 파일 시스템
       이미지와는 어떠한 연결 고리도 없다. 그렇기 때문에 , 파일 시스템을 변경한 후에 언마운트
       시키면 그 변경된 내용이 사라지게 된다. 만약에 , 변경된 내용을 저장하고 싶으면 그 파일
      시스템 내용을 다시 다른 파일로 백업해야 한다. 다음 명령어도 그 중 한 가지 방법이다．

         # dd if=/dev/mtdblock0 of=./your-modified-fs-image. bin

      이 명령어는 커널 구성 시에 지정한m七dblockO 장치와 같은 크기의 파일 your-modified
      -f針image .bin을 만든다. 여기서는 8MB가 될 것이다. 리눅스에서 JFFS2를 편리하게
      수정할 수 있도록 제공되는 기능은 부족하지만, 방금 사용한 방법은 JFFS2 파일 시스템을
      시험하고 수정하는 데 아무런 문제가 없는 방법이다. 더 중요한 것은 진짜 플래시 메모리가
      없는 개발 시스템에서 MTD 서브시스템에 대한 기본 개념을 확인해 볼 수 있다는 점이다.
      이제 실제 물리적인 플래시 메모리를 갖고 있는 하드웨어 시스템을 한 번 보도록 하자．




2) 리눅스 커널 구성 옵션에서 MTD IWVI 테스트 디바이스를 활성화활 때 그 크기도 함께 지정했었다．



                                                                            323 1
 a.    Embedded Linux Primer




10.2.1 MTD 구성하기
      보드에 존재하는 플래시 메모리를 MTD로 이용하기 위해서는 먼저 MTD가 올바로 구성되
      어 있어야 한다. 다음 항목은 독자의 보드가 갖고 있는 플래시와 그 플래시 구조를 MTD에서
      사용할 수 있도록 하기 위해 반드시 필요한 설정 항목들이다．

       口 플래시 장치의 파티션 지정하기
       口 플래시 메모리의 종류와 주소 영역 지정하기
        口 독자가 선택한 플래시 IC에 대한 올바른 플래시 드라이버 구성하기
        口 알맞은 드라이버를 커널을 포함하도록 구성하기

      각각의 단계에 대해서는 이어지는 섹션에서 자세히 알아보도록 하자．



]0.3 MID 파티션
      하드웨어 플랫폼에서 사용되는 대부분의 플래시 메모리는 파티션이라고 부르는 몇 개의 부분
      들로 나누어져 있다. 이는 일반적인 데스크탑 워크스테이션의 하드디스크 파티션과 비슷하
      다. MTD 서브시스템은 이런 플래시 파티션을 지원해 주는데 , 그러기 위해서는 'MTD 파티
      션 기능 지원（MTD partitioning support) '이라는 항목이 활성화되어 있어야 한다. ［그림
      10-2］에서 MTD 파티션 기능 지원을 위한 구성 옵션을 볼 수 있다．

      리눅스 커널에는 파티션의 데이터와 통신할 수 있는 메서드를 몇 7거 가지고 있다. 다음 메서
      드들이 현재 지원되는 것들이다. 다음 항목들에 대한 구성 옵션은 모두［그림 10-2］의 MTD
      파티션 기능 지원 항목에서 볼 수 있다．

        口 Redboot 파티션 테이블 파싱（parsing)

        口 커널 커맨드 라인 파티션 테이블 정의

        口 보드에 따른 드라이버 매핑

      MTD는 파티션 데이터 없이도 사용할 수 있는데 , 이때는 MTD가 플래시 메모리의 전체 영
      역을 하나의 장치로 인식해서 사용하게 된다．
                                                                                               MTD 서브시스템          Chapter 10



    E如 Qpttocis !t出1                                                    1
          包    i쿄 口            I    I냐甘          可1 呼
          BaC니Load Save 듸n5甘e Sp吼I '耶 Collapse Exper너

    Opti。
        ns                                                              =1    Name11                     :L스

           "Memory Technology Devices (MID)                                                              1
            口 回枷mo싸Techr自四yDe너ce們TO) vu마S가t                                   MID
                 口Deb四gmg                                                     MIDJIEBLJG
                 口MID concaten曲必叩附t                                           MID느．CONCAT                ！小
               7回MID p踊鈿甘四vu叩ort                                              MTDJ'ARTFrIONS             i
                 卜 回RedB凹I partition La［扼pa巧ing                               MTDJ1EDBOOT_PARTS !
                    口Command有昶partition幽ep拓岫                                  MID工MDLIN已PARTS            汪
                    E ARM日rmware S너te partition parsing                       MTD. AFSJARTS              !
                  User Mod너esAndlran引ation Lay미S                                                         ;
                 回 Deect char device access to MTD devices                    MID_CHAR                       n
                  回Cachir咀HO比如ice配Ce釘ioMTDde吼es                               MTD_BLOCK                  I
                 口FTL (flash Iran引aLlots녀yer) s目p口Ott                         FTL                        n
                 口NFFL (HAND디ashlran引如n Layer) sup口ott                        NFTL
                 口IN口L (Inverse NAND F佃帥Traits)카幻n Lay帥5나叩아t                  INFTL
               b RAM/ROM/Flash chip drivers                                                              L
               口 Mapp目凹drivers f아chip access                                                             \
                    回Sup螂啣小陀at mappir也sofflashc却s                             MTD_COMPLEX_MAPPINC
                    口CFI Flash device in physic出 memory map                   MTD_PHYSMAP                r
                    口CFI Flash device mapped on ARM lntegrator/P7201          MTD小RMJNTEGRATOR
                     刃 CR Flash device mapped on Intel IXP4xx based systems   MTDJXP4XX                      r;
     'I                                                                               f'   1
                                                                                                1   i1
           FI F뇨sh device nit且pped onin挺l ix丙cx而됴可斗뇨ems MTDJXP4XX                                            스

          This enables MID access to flash devices on platforms based
          on lntel's 以P4xx fern却 of netwi姓 마ocesso巧 su比 as ft咆
          1XDP425 and Coyote, If you have an IXP4xx based 的ard and
          would like to use t1比 flash cl叩s on 兀 say 'Y.                                                      쿄


    I 그립 ]0-2 MTD 파티션 기능 지원을 위한 커널 구성 옵션



10.3.1 Redboot 파티션 테이블 나누기
    MTD 파티션을 정의하거나 찾아내기 위해서 주로 사용되는 메서드들은 최초로 구현된
    Redboot 파티션에서 유래한 것이 많다. Redboot은 많은 임베디드 시스템에서 사용되는 부
    트로더인데 , 특히 ADI 엔치니어링의 코요테 플랫폼 등의 ARM 엑스스케일 보드에서 많이
    볼 수 있다．

    MTD 서브시스템은 하드 디스크의 파티션 테이블과 비슷한 개념으로, 플래시 장치 자체에
    파티션 정보를 처장할 수 있는 메서드를 정의하고 있다. Redboot 파티션의 경우에는, 파티
    션을 정의하기 위해서 별도로 삭제 단위 블록 하나를 전용 공간으로 따로 예약해서 사용한다．
    그리고 부팅 시에 플래시 메모리 장치에 있는 파티션을 인식하기 위해서 파티션을 분석하기


                                                                                                                        325 毋
   難      Embedded Linux Primer




        위한 함수를 호출하는 매핑 드라이버（n追1珂ng driver）를 하나 선택하게 된다. ［그림
        10-2］에서는 맨 마지막에 반전된 항목을 통해서 예제 보드를 위한 매핑 드라이버가 선택된
        것을 볼 수 있는데 , CONFIG MTD IXP4xx라는 옵션을 정의하게 된다．

        여기서도 실제로 한 번 연습해 보는 것이 개념을 이해하는 데 도움이 될 것이다. 코요테 플랫
        폼을 위한 Redboot 부트로더가 제공해 주는 정보를 먼저 보도록 하자. ［리스트 10-4］는
        Redboot 부트로더가 부팅 중에 출력하는 내용의 일부를 나타낸 것이다．

        ［리스트 ]0-4) Redboot 부팅 메시지


          platform: ADI Coyote (xScale)
          IDE/Parallel Port CPLD version: 1. 0
          copyright (C) 2000, 2001, 2002, Red Hat, Inc.

          RAM: 0x00000000-0x04000000, 0x0001f960-0x03fd1000 available
          FLASH: 0x50000000 - 0x51000000, 128 blocks of 0x00020000 bytes each.




        이 메시지의 내용은 보드의 RAM이 0x00000000 번치를 시작으로 매핑되어 있다는 것과
        플래시는 물리 주소 0x50000000에서 0x51000000까치 매핑되어 있는 것을 알 수 있다．
        그리고 각각 0x00020000(128K1B) 크기의 블록 128개를 가치고 있는 것도 볼 수 있다．

        Redboot는 플래시에 파티션을 만들거나, 파티션 정보를 출력해 주는 명령어를 가지고 있다．
        ［리스트 10-히는 fis uis七라는 명령어를 실행한 결과를 나타낸 것이다. 이 명령어는
        Redboot 부트로더에서 사용할 수 있는 플래시 이미지 관련 명령에 집합（FIS : Flash
        Image System)에 포함되어 있다．

        ［리스트 ]0-5) Redboot 플래시의 파티션 정보


          RedBoot> fis list
          Name                    FLASH addr   Mem addr     Length       Entry point
          Red800t                 0x50000000   0x50000000   0x00060000   0x00000000
          RedBoot config          0x50FC0000   0xSOFC0000   0x00001000   0x00000000
          FIS directory           0x50FE0000   0xSOFE0000   0x00020000   0x00000000
          RedBoot>




蟹 326
                                                    MTD 서브시스템     Chapter 10




［리스트 10-5］를 보면 코요테 보드의 플래시에 세 개의 파티션이 정의된 것을 볼 수 있다．
RedBoo七이라는 이름을 가진 파티션은 Redboot 부트로더의 실행 이미지를 담고 있다．
RedBoot config이라는 이름을 가진 파티션은 부트로더가 관리하고 사용하는 구성 정보
파라미터를 가지고 있다. 마지막에 FIS direc七ory라는 이름의 파티션은 파티션 테이블 자
체에 대한 정보를 갖고 있다．

올바로 설정한 경우, 리눅스 커널은 플래시에 존재하는 물리적인 파티션을 나타내는 MTD
파티션을 만들 수 있고, 또한 파티션 테이블도 검색해서 그 내용을 분석할 수도 있다. ［리스
트 10-6］은 Al끄 엔지니어링 코요테 보드에서 Redboot 파티션을 인식할 수 있도록 리눅스
커널을 구성해서 부팅했을 때 출력되는 부트 메시지의 일부를 다시 나타낸 것이다．

［리스트 ]0-6] 리눅스 부팅 시에 日edboot 파티션을 인식하는 과정



  IXP4XX- FlashO: Found 1 x16 devices at OxO in 16-bit bank
   Intel/ Sharp Extended Query Table at 0x0031
  Using buffer write method
  cfi_cmdset_0001: Erase suspend on write enabled
  Searching for RedBoot partition table in IXP4Xx-Flash0 at offset Oxfe0000
  3 RedBoot partitions found on MID device IXP4Xx-FlashO
  creating 3 MID partitions on "IXP4XX-Flash0":
  Ox00000000-0x00060000 : "RedBoot "
  Ox00fc0000-Ox00fc1000 : "RedBoot confi g"
  0xOOfe0000-Ox01000000 : "FIS di rectory"




［리스트 10-6］에 출력된 첫 번째 내용은 플래시 IC를 감지했을 때 출력되는데 , CONFIG
卜4TD CFI를 활성화하면 사용할 수 있는 공용 플래시 인티페이스（CFI : Common Flash
Interface) 드라이버가 이 내용을 출력하게 된다. CFI는 플래시 칩의 특성을 인식할 수 있
도록 하기 위한 산업 표준이다. CI可를 통해서 알 수 있는 특성으로는 제조자 정보, 장치 종
류, 전체 용량, 삭제 단위 블록의 크기 등이 있다. 10.5.1절의 "더 읽어 보기"에는 CFI 표준
안에 대한 참고 자료가 나와 있다．




                                                                       327 I
  a.          Embedded Linux Primer




       CFI는 커널 구성 유틸리티에서 메모리 기술 저장 장치 (MTD) 최상위 메뉴 아래에서 활성화
       시킬 수 있다. 거기에서 ［그림 10-3］에서 볼 수 있는 것처럼 RAM/ROM/Flash chip
       drivers라는 항목 아래에 있는 Detec七 flash chips by Comon Flash Interface
       (CFI) probe를 선택하면 퇸다．

           텨e         O少心ns   Ke如

             勿 口 目                    1    n 는    曲             骨1
            8 ,iC k    Load Save Sing노 Sp撫 Full Collapse Expand

           Options                                                            i Name            巴

              (7 Memory Technology Devices IMTD)
                 口 回 Memo斗Techn이이升 Device {MTD) su미）art                        MTD
                         口Debugquvg                                            MTD卜DEBUG            1
                         口MTD concaten鈿g 5UP的It                                MTD小CONCAT
                       b 回卜｛FD口artittorung su口口art                             MTD_PARTITIONS   匕
                         User Mod너es And Tran引ati미1 Layers
                         回［가ed char device ac（巴S to 町Dde너ces                   MTDCKAR
                         團 Cachi四 block device access to MTD devices           MTD_BLOCK
                        口FR (flash Trait引at佃n Layer沾up叫t                       FTL
       ?                 口N尸江們斛D Flash Tian引如n Lay的돠汭it                        NEIL
                        口忖IL伽咽se NAND Fla帥Ti毗翩｛311 Lx叩沾upport                  INFTL
                       \7 UM/ROM/ 카ish chip drIvers
                           回［沌In出lash clips by Common目弱h interf配이CEI) p民力e     MTD_CFI
                           E Detect nOn-CFI AMDIJEDEC-compa百ble flash chips    MTDJEDECPROBE        {;
                                                                                       l        m
             CA Flash device mapped on Intel IXP4xa based systems MTD_IXF4XX

            This enables MTD access to flash devices on platforms based
            ｛가liNe朽 iXP4xx lam啣 ｛寸 netv心k process아5 50小 as the
            1XOP425 and C口yote. If you have an IXP4*x based board and
            wotdd like to use the fla5h c椰s on it, say V'.


       I 그림 10召 MTD CFI를 지원하도록 커널 구성하기

       ［리스트 10-6］에서는 플래시 칩이 CFI 인터페이스를 통해서 감지된 것을 볼 수 있다. 우리
       는 CONFI（乞MTD REDBOOT PARTS를 활성화시켰기 때문에（［그림 10-2] 참조） MTD는 이
       플래시 칩에서 Redboot 파티션 테이블이 있는지 검색하게 된다. 그리고 이 플래시 칩이
       IXP4XX-Flash0라는 이름으로 인식된 것도 주목하도록 하자. ［리스트 10-6］에서 플래시
       칩에 있는 세 개의 파티션을 리눅스 커널이 인식한 것을 볼 수 있는데 , 이는 이전에 Redboot
       에서 fis list 명령을 실행한 것과 같은 결과이다．

       여기서 설명한 것과 같은 기반 구조가 갖추어진 상태에서 리눅스 커널은 자동으로 세 개의
       플래시 파티션을 나타내는 자료 구조를 내부적으로 생성한다. 그 증거는 /proc 파일 시스템
       에서 짖아볼 수 있는데 , ［리스트 10-7］을 보도록 하자．


1328
                                                 MID 서브시스템    Chapter 10



［리스트 10-7) 커널의 MTD 플래시 파티션

  root@coyote: 4 cat /proc/mtd
  dev:    size erasesize name
  mtd0: 00060000 00020000 "RedBoot "
  mtdl: 00001000 00020000 "RedBoot config"
  mtd2: 00020000 00020000 "FIS directory"
  #



새로운 Redboot 파티션은 쉽게 만들 수 있는데 , 이 예제에서는 Redboot의 FIS 명령어를
이용하면 된다. 하지만 여기서 Redboot 명령어에 대해서 자세히 다루지는 않겠다. 관심 있
는 독자는 10.5.1절에 있는 참고 자료를 보도록 하자. ［리스트 10-8］은 새로운 Redboot
파티션을 만드는 세부 절차를 보여 주고 있다．

［리스트 ]0-8] 새로운 Redboot 파티션 만돌기

  RedBoot> load -r -v -b 0x01008000 coyote-40- zlmage
  using default protocol (TFTP)
  Raw file loaded 0x01008000-0x0ll4dccb, assumed entry at 0x01008000
  RedBoot> fis create -b 0x01008000 -1 0x145cd0 -f 0x50100000 MyKernel
      Erase from 0x50100000-0x50260000:
      Program from 0x01008000-0x0ll4dcdO at 0x50100000:
      Unlock from 0x50fe0000-0x51000000: .
      Erase from 0x50fe0000-0x51000000: .
      Program from 0x03fdf000-0x03fff000 at 0x50fe0000:
      Lock from 0x50fe0000-0x51000000: .



먼저 , 새로 생성할 파티션에서 사용할 이미지를 로드한다. 여기서는 예제로 리눅스 커널 이
미지를 사용했다. 이미지를 메모리 주소 Ox01008000에 로드했다. 그리고 Redbo毗의 f is
create 명령어를 이용해서 새로운 파티션을 생성했다. 그리고 Redboot 명령을 통해서 새
로운 파티션을 플래시의 0x50100000에 시작하는 영역에 생성하도록 했다. 과정을 보면
Redboot가 먼저 이 영역을 지운 후에 커널 이미치를 기록하는 것을 볼 수 있다. 마지막 단계
에서는 Redboot이 자신의 디렉터리 영역에 대한 보호를 해제하고 새로운 파티션에 대한 정
보를 FIS 디렉터리에 업데이트하게 된다. 다음 내용을 ［리스트 10-5］와 비교해 보자.
           Embedded Linux Primer



        ［리스트 ]0-9) 새로 추가된 Redboot 파티션 목록

           RedBoot> fis list
           Nanie                   FLASH addr   Mem addr     Length       Entry point
           RedBoot                 0x50000000   0x50000000   0x00060000   0x00000000
           RedBoot config          Ox50FC0000   0x50FC0000   0x0000l000   0x00000000
           FIS directory           Ox50FE0000   0xSOFE0000   0x00020000   0x00000000
           MyKernel                0x50100000   0x50100000   0x00160000   0x01008000



        물론 리눅스 커널을 부팅시키면 새로운 파티션을 인식할 것이고, 우리가 원하는 대로 이용할
        수 있게 된다. 일부 독자는 새로운 파티션을 이용해서 얻을 수 있는 다른 이점을 이미 생각했
        을 것이다. 즉, 부팅 시마다 매번 tftp에 접근하는 대신에 플래시에서 커널을 부팅시킬 수도
        있다. 그 명령어는 다음에 나와 있다. 플래시에서 그 파티션의 시작 주소와 RAM에 복사할
        이미지 크기를 Redboot 명령어인 exec어］ 넘겨주면 된다．



          RedBoot> exec -b 0x50100000 -l 0x145cd0
            Uncompressing Linux           done, booting the kernel.




10.3.2 커널 커맨드 라인에서 파티션 생성하기

        10.3절 "MTD 파티션"에서 자세히 설명한 것처럼 리눅스 커널에서 플래시 파티션 정보를 주
        고받는 데 다른 방법을 사용할 수도 있다. 그 중에서도 간단하지는 않지만 가장 직관적인 방
        법은 커널 커맨드 라인에 직접 파티션 정보를 넘겨주는 것이다. 물론 (U-Boot와 같은） 일부
        부트로더를 이용하면 쉽게 할 수 있지만, 다른 부트로더 중에는 부팅 중에 커널 커맨드 라인
        을 입력하는 기능을 지원하지 않는 것들도 많다. 이럴 때는 커널을 컴파일할 시점에 커널 커
        맨드 라인을 설정할 수밖에 없고, 파티션 관련 내용이 변경되어서 내용을 바꾸려고 할 때마
        다 커널을 매번 다시 컴파일해야 하는 어려움이 있다．

        커널 커맨드 라인에서 MTD 서브시스템의 파티션을 설정할 수 있도록 하기 위해서는 이 기
        능을 지원하도록 커널을 구성해야 한다. ［그림 10-2］를 보면 이 구성 옵션이 MTD
        parti七ioning support 항목 아래에 있는 것을 볼 수 있다. 여기서 Con皿nand中line


! 330
                                                           MTD 서브시스템         Chapter 10



    par七ition table parsing을 선택하면 되고, 구성 파일에는 CONFIG MTD CMDLINE
    PARTS라는 옵션이 추가될 것이다．

    ［리스트 10-10］은 커널 커맨드 라인에서 파티션을 표현하는 방식을 나타낸 것이다
     (. ../dri＼厄rs/r毗d/cmdlinepart . c에서 발췌）.

    ［리스트 ]0-10] 커널 커맨드 라인에서 사용하는 MTD 파티션 형식

       mtdparts=<mtddef> I; <mtddef]
        士<mtddef> : = <mtd-i d>: <partdef> I, <partdef>]
        *<partdef> := <size> {@offset] [<name>] [ro]
        央＜mtd-id> := unique name used in mapping driver/device (mtd->name)
        士＜size>    := std linux memsize OR "1" to denote all remaining space
        士＜name>    := ' ( ' NAME ' )'



    커널 커맨드 라인에 전달된 각각의 m七ddef 파라미터는 각각 하나의 파티션을 정의하게 된
    다. ［리스트 10-1이에서 볼 수 있듯이 , mtddef 선언 하나는 여러 부분으로 이루어져 있다．
    고유한 ID를 부여할 수 있고, 파티션의 크기와 플래시의 시작 번지부터 어느 위치에 있는지
    에 대한 오프셋（offset) 정보를 정의할 수도 있다. 그리고 파티션 이름이나, 필요에 따라서
    는 읽기 전용인지를 나타낼 수도 있다. 전에 ［리스트 10-5］에서 Redboot 파티션을 선언한
    내용을 커널 커맨드 라인으로 정의하면 다음과 같이 나타낼 수 있다．

       mtdparts=MainFlash: 384K(Redboot) ,4K(config) ,l28K(FIs) ,-(unused)

    위 커널 커맨드 라인을 통해서 커널은 MainFlash라는 MTD ID를 가진 네 개의 MTD 파
    티션을 만들게 되는데, ［리스트 10-5］에서 볼 수 있는 크기와 구조를 갖고 있다．


10.3.3 미1룔i 드라이버
    자신의 보드에 맞는 플래시 구조를 정의하기 위한 마지막 한 가지 방법은 보드 전용으로 만들
    어진 매핑 드라이버를 이용하는 것이다. 리눅스 커널 소스 트리는 . . . /drivers/m七d/
    maps어］ 많은 수의 매핑 드라이버가 있다. 자신만의 매핑 드라이버를 만들 때 이들 중 하나를
     예제로 삼으면 좋을 것이다. 구현된 세부 내용은 아키텍처에 따라서 다르다．
   繫.     Embedded Linux Primer




        매핑 드라이버도 커널 모듈인데 , 8장, "디바이스 드라이버 기초"에서 설명한 module
        mni七 () 이나 module exit () 도 포함된 완전한 모듈이다. 일반적으로 매핑 드라이버는 C
        코드 20 --30줄 정도로 짧고 내용도 이해하기가 쉽다．

        ［리스트 10-11]은 . . . /drivers/mtd/maps/pq2fads의 한 단락을 다시 나타낸 것이다．
        이 매핑 드라이버는 MPC8272와 다른 프로세서를 지원하는 프리스케일 PQ2FADS 평가용
        보드에 있는 플래시 메모리를 위한 매핑 드라이버이다．

        ［리스트 ]0너 ]]PQ2FADs 플래시 매핑 드라이버



          static struct mtd_partition pq2fads_partitions{ ] = {
                     {
          判fdef CONFIG卄ADS8272
                    . name     = "HRCW",
                    . size     = 0x40000,
                    . offset     = 0,
                    . mask_flags= MID_WRITEABLE, 1* force read-only *"/
                },       {
                             .name     = "User FS",
                             .size     = 0xSc0000,
                             .offset     = 0x40000,
          #else
                             .name     = "user FS",
                             .size     = 0x600000,
                             .offset     = 0,
          #end if
                }, {
                             .name      = "ulmage",
                             .size      = 0x100000,
                             .offset      = 0x600000,
                             .mask_flags = MTD_WRITEABLE,     /'" force read-only */
                },       {
                             .name      = "bootloader ",
                             .size      = 0x40000,
                             .offset    = 0x700000,
                             .mask_flags = MTDHWRITEABLE,     /* force read-only */
                },       {
                             .name      = "bootloader env",
                             .size      = 0x40000,



發 332
                                                                MTD 서브시스템    Chapter 10



                        .offset          = 0x740000,
                        .mask_flags = MTD_WRITEABLE, /* force read-only */
               }
         };
         /"" pointer to MPc885ADS board info data *"1
         extern unsigned char _res[ ];

         static mnt _init init_pq2fads_mtd(void)
         {
                   bd_t *bd = (bd_t *)mmres;
                   physmap_configure (bd今bi_flashstart, bd->bi_flashsize,
                                   PQ2FADS_BANK_WIDTI-1, NULL) ;

                   physmap_set_partitions (pq2fads_partitions,
                                 sizeof (pq2fads_partitions) /
                                 sizeof (pq2fads_partitions{0] ));
                    return 0;
         }
         static void _exit cleanup_pq2fads_mtd(void)
         {
         }
         module_init (init_pq2fads_mtd) ;
         module_exit (cleanup_pq2fads_mtd) ;




      이 간단한 리눅스 디바이스 드라이버는 PQ2FADS 플래시를 MTD 서브시스템에 매핑할 수
      있도록 해 준다. 8장에서 module init () 매크로로 정의된 함수는 리눅스 커널에 의해서
      자동으로 알맞은 시점에 호출된다고 했었다. 이 PQ2FADS 매핑 드라이버의 경우에 모듈
      초기화 함수 mni七 pq2fads I毗d (）의 내용은 단순히 함수 두 개만 호출하고 있다．

         口 physmap configure () 함수는 플래시 칩의 물리 주소, 크기 , 뱅크의 너비3) 그리고
              플래시어］ 접근하기 위해써 필요한 특수 설정 함수들을 MTD 서브시스템에 넘겨준다．




3) C역자주） 뱅크가 4711 있다는 것은 4개의 칩을 보드에 장착할 수 있다는 의미이다 ．뱅크의 너비가 32U1트이고， 플래시 메모리는
 16비트이면 항상 플래시 메모리 2개를 연결해서 뱅크C각 너비 32비트를 맞춰야 한다．
 纛1 1           Embedded Linux Primer



                口 physmap se七 partitions () 함수는 매핑 드라이버의 시작 부분에서 볼 수 있는
                        pq2 fads parti七ions [］라는 배열로 정의된 파티션 테이블을 이용해서 MTD 서브
                            시스템에 현재 보드의 파티션 정보를 전달하는 일을 한다．


        이 간단한 예제를 참고해서 독자도 자신의 보드에 맞게 매핑 드라이버를 만들 수 있을 것이다．


10.3.4 플래시 칩 드라이버
        MTD는 다양한 플래시 메모리와 장치를 폭 넓게 지원하기 때문에 독자가 선택한 플래시도
        이미 지원할 가능성이 아주 높다. 일반적인 플래시 칩은 대부분 이전에 설명한 공용 플래시
        인터페이스（CFI）를 지원한다. 하지만 오래된 플래시 칩의 경우에는 JEDEC를 지원하는 것
        들도 있는데 JEDEC는 CFI 이전의 플래시 표준이다. 최신 리눅스 스냅샷에서 커널 구성
        유틸리티를 실행한 ［그림 10-4］를 보면 많은 종류의 플래시를 지원하는 것을 볼 수 있다．

        日e           O的（恥s       ddp

               蜘 ［二7 口                   I     H    L       m         骨
               r1」      La心d Saoe S汨대a S口lit Fu朴 C에a口se Etcpand
        1O的毗                                                                                                         1뜨
                                                                                      iN4毗
                     47 [   Memory Technvi四y Device (町D) support                             町D
                            口마bug恥g                                                          MID_DEB以；
                            口 MTD concatenating support                                      MTDCO忖CAT
                        b 回MTD p카甘如rung su叩art                                               MrD_P사rmoNs
                            User h加3'加las And Tran引aft아r Laye匹                                                            m
                            回［가ect char den乂e 改cess to MTD devices                           MID_CHAR
        :                   回Cachi凹 Mock device access to MID de너ces                         MID_BLOCK                (
                            El FTL (目ash Translation녀yer) support                            FTL
                            El NF1L (NAND Flash Translation Layer) support                   NFTL
                            El INFTL (Inverse NAND Flash Tran引ation Layer) support           INFTL                   i
                        1 RA！叩RO帥FLish cli甲 driers
                              回Dete心日a引｝C汁ps by Common디ash Interface (CEll probe MID_Cit                                  J
                              口De沁Ct ni가i-CE) AM0/JEDEC＜이npati벼eflashchips                   MT口LJEDECPROBE
                              口Flash clip d加er advanced con有guration options                 MTD_CELA마刃PT田MI
                              囹Support佃r tnt님／Shar汁ash chips                                 MID뇨CFI_INTELEXT
                              口Sup刈for AM［가ii恥印佃hcltips                                      MTI工Cit小卜카巧ID
                              El Support for ST (Advanced Architecture) fla引l chips          MID_CF1_STAA
                              口Support for RA卜dchips In bus mappi四                           M丁0下AM
                              口S叩四rt for R아l clips in山s map目四                                MID나：1OM
        秀                     口Support for absent chips in b口s map머四                         UT0小BSEP4T
        푿                     口）UP aware MID support                                         M丁［l乂P
                        P Ma帥beg d加ers for하叩 配cess
                        P S叫f｛아tt긔ned MTD den乂a drivers
                       口 HAND Flash［뇨너ce 마we匹
                            卜 日HAND De너ce Sup的it                                             MTD_NAND
                              口미skOn（加p 2000, Millenr甘urn/f켜us                               MTD_NAND寸DISKONCHIP r
        m                                                  口3
                                                                    m甘   叫                                      ！三
        I 그림 ]0-4 지원되는 플래시 메모리들


I 334
                                                        MTD 서브시스템        Chapter 10




    만약에 독자가 사용하는 플래시 칩이 지원되치 않는다면 . . . /drivers/m七d/chips어］ 있
    는 것들을 예제 삼아서 내용을 자신에 맞게 수정하고 추가해서 직접 디바이스 드라이버 파일
    을 만들어야 한다. 하지만 사용하는 칩이 갓 개발된 최신 인터페이스를 사용하는 것이 아니
    라면 이미 누군가가 그 드라이버를 개발해 놓았을 가능성이 높다．


10.3.5 보드에 따룐 초기화

    올바른 MTD 플래시 시스템 동작을 위해서는 매핑 드라이버와 함께 자신의 보드에 맞는 초
    기화 작업을 통해서 적절한 선언 값을 MTD 서브 시스템에 제공해야 한다. ［리스트 10-12]
    는 . . . /arch/arm/mach-i자4xx/ coyo七e四etup. c에서 그에 해당되는 부분을 나타낸

    것이다．

    ［리스트 ]0-12] 코요테 보드 셋업 코드


      static struct flash_platform_data coyote_flash_data = {
           .map_name = "cfi_probe",
            . width   = 2,
      };
      static struct resource coyote_flash_resource = {
           .start           = COYOTE_FLASH_BASE,
           .end           = COYOTE_FLASH_BASE + COYOTE_FLASH_SIZE - 1,
           .flags           = IORESOURCE_MEM,
      };

      static struct platform_device coyote_flash = {
           .name        = "IXP4XX-Flash",
           .id         =0,
           .dev        ={
                  platform_data = &coyote_flash_data,
           },
           .num_resources      = 1,
           .resou rce = &coyote_fl ash_resource,
      };
      static struct platform_device *coyote_devices[ ] _initdata = {
            &coyote_fl ash,



                                                                              335 i
 髓1 1     Embedded Linux Primer



                   &coyote_uart
          }   1,




          static void _in卄 coyote_init (void)
          {


                   platform_add_devices (coyote_devices,
                                         ARRAY_SIZE (coyote_devices) );
          }




        ［리스트 10-12］는 coyote-setup. c 플랫폼 초기화 코드에서 설명에 관련된 부분만 나타
        낸 것이다. 맨 아래부터 보면 coyo七e init () 함수는 pla七form add devices () 를 호
        출해서 이 파일의 앞부분에 정의한 코요테 보드 전용의 장치들을 선언하고 있다. 두 개의 디
        바이스를 정의하는 부분이 coyote init () 함수 바로 위에 있는 것을 알 수 있다. 여기서
        관심을 가져야 할 항목은 coyote flash이다. 이 항목은 pla七form device라는 구조체
        인데, 여기에는 리눅스 커널과 MTD 서브시스템에서 필요한 중요 세부 정보가 들어 있다.

        coyote flash 구조체의 .name 멤버는 같은 이름을 갖는 매핑 드라이버를 플래시 메모리
        와 연결시키기 위해서 사용된다. 이 매핑 드라이버는 . . /drivers/mtd/maps/ixp4xx. c
        에서 찾을 수 있다. 그리고 . resource 멤버는 보드상의 플래시 메모리의 기본 주소를 알려
        준다. 내부에 .pla七form data 멤버를 가지고 있는 .dev 멤버는 플래시에 맞는 칩 드라이
        버를 결정하는 데 사용된다. 위 코드 예제에서는 커널 구성 옵션에서 CONFIGM町LCFI로
        나타낸 것처럼 보드의 플래시 칩과 통신하는 방식으로 CFI 방식을 사용하겠다고 명시하고
        있다. ［그림 10-4］를 보면 이 구성 옵션이 선택된 것을 볼 수 있다．

        자신이 사용하는 보드와 아키텍처에 따라서 이와 비슷한 방식으로 보드에 있는 플래시를 사
        용하게 만들 수 있다．



]0.4 MID 유털리El
        MTD 패키지에는 MTD 서브시스템을 설정하고 관리하기 위한 시스템 유틸리티들도 포함되
        어 있다. 이 유틸리티들은 리눅스 커널 소스 트리 내에서 같이 빌드되어야 하는 주 MTD 서


I 336
                                                 MTD 서브시스템    Chapter 10




브시스템과는 별도로 빌드시켜서 사용해야 한다. 이 유틸리티들도 다른 코드를 교차나컴파일
해서 사용하는 것과 같이 빌드시키면 된다．

이 유틸리티들을 사용하는 데 있어서 주의할 점은 실수를 방지할 수 있는 장치가 없다는 점이
다. 즉, 숫자 하나를 잘못 입력해서 보드에 기록되어 있던 부트로더를 완전히 삭제시켜 버릴
수도 있다. 또 이 경우 부트로더를 백업해 두지 않았거나 JTAG 플래시 프로그래머를 이용해
서 다시 기록해 넣는 방법을 모를 경우에는 복구하는 데만 많은 시간을 허비해야 할 것이다．

이 책의 관행대로 모든 MTD 유틸리티에 대해서 다 다루기는 지면이 여의치 않기 때문에
가장 많이 쓰이고 쓸모 있는 것들만 살펴볼 것이고, 나머지는 독자에게 숙제로 남기고자 한
다. 최신 MTD 프로젝트에는 20개 정도의 유틸리티 실행 파일이 포함되어 있다．

flash*로 시작하는 유틸리티 계열은 MTD 파티션을 저수준에서 다룰 때 유용하게 사용된
다. 여기에는 flashcp, flash_erase, flash info, flash Jock, flash끄niock 등이 있다．
아마도 명령에 이름 자체로도 충분히 어떤 일을 하는 명령어인지 유추할 수 있을 것이다. 파
티션이 정의되고 각각의 파티션이 커널 장치로 연결되고 나면 이 유틸리티들을 그 파티션을
대상으로 실행시킬 수 있다. 다시 한 번 주의를 당부할까 한다. 만약에 부트로더가 들어 있는
파티션을 대상으로 flash erase 명령을 실행시켜 버리면 보드가 더 이상 아무 일도 못하
는 골칫거리로 돌변할 것이다. 그래도 한 번 해보고 싶다면 부트로더 이미지를 백업해 두고，
하드웨어 JTAG이나 플래시 프로그래밍 툴을 이용해서 플래시에 이미지를 다시 기록하는 방
법을 먼저 알아 두기 바란다．

［리스트 10-13］을 보면 ［리스트 10寸8］에서 우리가 새롭게 만든 파티션（MyKernel）이 코
요테 보드의 커널에서도 보이는 것을 알 수 있다. 즉, 새로 생성한 파티션이 mtdl이라는 커
널 디바이스로 연결된 것을 볼 수 있다．

［리스트 10-13) 커널의 MTD 파티션 목록


   root@coyote: 硝 cat /proc/mtd
   dev:   size   erasesize name
   mtdO: 00060000 00020000 'RedBoot "
   mtdl: 00160000 00020000 "MyKernel "
   mtd2: 00001000 00020000 "RedBoot config"x
   mtd3: 00020000 00020000 'FIS directory "




                                                                   337I
 難毋U    Embedded Linux Primer




       MTD 유틸리티를 이용해서 새로 만든 파티션을 대상으로 몇 가치 작업을 해볼 수 있다. 다음
       내용은 flash erase 명령을 새로운 파티션에 실행시킨 결과를 보여 준다．



         # flash_erase /dev/mtdl
         Erase Total 1 Units
         Performing Flash Erase of length 131072 at offset OxO done




       새로운 커널 이미지를 이 파티션에 복사하려면 flashcp 명령을 이용한다．

         root@coyote:畔 flashcp /workspace/ coyote- 40- zlmage /dev/mtdl


       루트 파일 시스템 파티션을 가지고 좀 더 재미있는 실험을 해볼 수 있다. 부트로더나 리눅스
       커널 옵션에서 Redboot 플래시 파티션에 있는 루트 파일 시스템 이미지를 이용하도록 할
       수 있다. 먼저 , Redboot를 이용해서 루트 파일 시스템을 담을 새로운 파티션을 만들도록 하
       자. 다음 명령어는 Roo七FS라는 새로운 파티션을 플래시 메모리의 0x50300000 위치에서
       30블록 크기만큼 생성하는 명령이다. 여기서 블록이란 삭제 단위 블록을 말하는 것이고, 이
       칩에서는 128KB이다．

         RedBoot> fis create -f Ox50300000 -l 0x600000 -n RootFS


       다음에는 커널을 재부팅한 후에 , 루트 파일 시스템 이미지를 새로운 파티션 Roo七FS어］ 복사
       한다. 이는 타깃 보드 상에서 리눅스 명령에 프롬프트에 다음 명령어를 입력하면 된다. 다음
       명령어는 파일 시스템 이미지를 현재 보드의 프롬프트에서 접근할 수 있는 디렉터리에 두었
       다고 가정한 것이다. 이 책에서 자주 언급했지만 여기서도 NFS를 이용하는 것이 가장 좋은
       방법이다．

         root@coyote:硝 flashcp /rootfs. ext2 /dev/mtd2


       파일 시스템은 파티션 공간이 되는 한도 내에서 수 MB 이상 될 수 있기 때문에 , 위 명령이
       완료되는 데는 시간이 좀 걸린다. 위 명령은 플래시에 이미지 데이터를 프로그래밍（또는 플
       래싱4）이라고 한다）한다는 것을 기억해 두자. 복사가 끝난 뒤에는, 이 파티션을 파일 시스템
       으로 마운트해서 사용할 수 있는데 , ［리스트 10-14］어 이 절차가 나와 있다．

4) ［역자주） 굽기라고도 한다. 플래시에 데이터를 기록하는 일을 주로 플래시에 이미지를 굽는다고 표현한다．
                                                   MTD 서브시스템    Chapter 10



［리스트 ]0-14) MID 푤래시 파티션을 ext2 파일 시스템으로 마운트하71

    root@coyote:畔 mount -t ext2/dev/mtdblock2 /mnt/ remote ro
    root@coyote:硝 ls -1 /mnt/ remote/
    total 16
   drwxr-xr- x 2 root root 1024 Nov 19 2005 bn
   drwxr-xr-x 2 root root 1024 0ct 26 2005 boot
   drwxr- xr- x 2 root root 1024 Nov 19 2005 dev
   drwxr-xr- x 5 root root 1024 Nov 19 2005 etc
   drwxr- xr- x 2 root root 1024 oct 26 2005 home
   drwxr- xr-x 3 root root 1024 Nov 19 2005 l 化
   drwxr-xr- x 3 root root 1024 Nov 19 2005 mnt
   drwxr- xr- x 2 root root 1024 oct 26 2005 opt
   drwxr- xr-x 2 root root 1024 oct 26 2005 proc
   drwxr-xr- x 2 root root 1024 oct 26 2005 root
   drwxr-xr- x 2 root root 1024 Nov 19 2005 sbin
   drwxr- xr-x 2 root root 1024 oct 26 2005 srv
   drwxr- xr- x 2 root root 1024 oct 26 2005 sys
   drwxr-xr- x 2 root root 1024 oct 26 2005 tmp
   drwxr- xr- x 6 root root 1024 0ct 26 2005 usr
   drwxr- xr- x 2 root root 1024 Nov 19 2005 var
   root@coyote : 硝



［리스트 10-14］에는 두 가지 미묘한 점이 있다. 먼처 mount 명령에 라인에 /dev/
mtdblock2를 입력한 것을 주목해 보자. 이 MTD 블록 디바이스 드라이버는 MTD 파티션
을 블록 디바이스로서 접근할 수 있도록 해 준다. 대신 /dev/m七d2를 이용하면 커널이
MTD 캐릭터 디바이스 드라이버를 사용하게 된다. 여기서 mtdchar와 m七dblock 모두 각
각 플래시 파티션에 대해서 캐릭터 또는 블록 단위 접근을 가능하게 하기 위한 슈도（pseudo
: 의사） 드라이버이다. moun七 명령어는 인자로 블록 디바이스를 받기 때문에 블록 디바이스
를 넣어 주어야 한다. ［그림 10-1]을 다시 보면 커널 구성 옵션에서 캐릭터 , 블록 두 가찌
접근 모드을 사용하도록 설정한 것을 볼 수 있다. 이에 해당하는 커널 구성 옵션은 각각
CONFIG MTD CHAR9I- CONFIG MTD BLOCK01다.


두 번째 미묘한 부분은 mount 명령어에서 읽기전용（ro) 옵션을 사용한 부분이다. 물론
MTD 블록 디바이스 에뮬레아션 드라이버를 이용해서 플래시에 있는 ext2 이미지를 읽기
천용으로만 사용하려고 마운트하는 것 자체는 아무 문제가 없다. 하지만, 사실 mtdblock
드라이버를 이용해서 ext2 장치에 기록하는 기능은 지원되치 않는다. 이는 ext2 파일 시스


                                                                    339I
 娑斗 n    Embedded Linux Primer




        템은 플래시의 삭제 단위 블록에 대한 개념을 갖고 있지 않기 때문이다. 플래시에 저장된 파
        일 시스템에서 쓰기 기능까지 사용하고자 할 때는 JFFS2와 같이 플래시 구조를 이해하는
        파일 시스템을 이용해야 한다．


10.4.1 JFFS2 루트 파일 시스템
        JI고FS2 루트 파일 시스템을 만드는 것은 간단한 작업이다. JFFS2는 압축 기능을 기본적으
        로 지원하고, 거기에 플래시의 수명을 오래 가도록 하기 위해서 블록에 쓰는 연산을 공평하
        게 분산시키는 웨어 레벨링 기능을 지원한다. 9장에서 지적한 것처럼 , 플래시 메모리는 쓰기
        횟수에 제한이 있다. 그래서 플래시 기반의 파일 시스템을 쓴다면 의무적으로 웨어 레벨링을
        지원하도록 해야 할 것이다. 이 책의 다른 부분에서도 언급하겠지만, 플래시 메모리는 반드
        시 가끔 쓰는 메모리로 취급해야 한다. 특히 어떤 프로세스가 대상 플래시 파일 시스템에 너
        무 자주 파일을 업데이트하는 것은 피해야 한다. 그런 것들로는 syslogd와 같이 시스템 관련


        JI고FS2 이미지를 이 Redboot의 Roo七ES 파티션에서 사용했던 ext2 이미지를 이용해서 만
        들 수도 있다. 여기서 JFFS2의 압축 기능의 위력을 바로 알 수 있다. 기존의 Roo七ES 파티
        션에서 사용한 이미지는 ext2 파일 시스템 이미지였다. 다음에 이 이미지 파일에 대한 정보
        를 볼 수 있다．



          # is -i rootfs. ext2
          -rw-r- -r- - 1 root root 6291456 Nov 19 16: 21 rootfs. ext2




        그럼 이제 MTD 패키지에 포함된 mkfs.jffs2 유틸리티를 이용해서 이 파일 시스템 이미지
        를 JFFS2로 변환해 보자. ［리스트 10-15］에 이 명령어와 실행 결과가 나와 있다．

        ［리스트 10-15) F祐otFS를 JFFS2 이미지로 변환하71


           # mount -o loop rootfs. ext2/mnt/ flash/
           # mkfs. j11s2 -r /mnt/ fiash -e 128 -b -o rootfs. jffs2
           # is 中i rootfs. jffs2
            rw- r- -r- - 1 root root 2401512 Nov 20 10: 08 rootfs. jffs2
           #




  340
                                                     MTD 서브시스템1   Chapter 10



       먼저 ext2 파일 시스템 이미지를 루프백 장치를 이용해서 개발 워크스테이션의 임의의 마운
       트 지점에 마운트한다. 그 다음에는 MTD 유틸리티인 mkfs.j ffs2를 호출해서 JFFS2 파일
       시스템 이미치를 만든다. -r 플래그는 趾fs.jffs2 유틸리티에게 루트 파일 시스템 이미지가
       어디에 위치하는지를 알려준다. -e 옵션은 mkfs.jffs2 이미지를 만들 때 블록 크기가
       128KB인 것을 감안해서 만들도록 해 준다. 기본 값은 64KB이다. 플래시의 실제 블록 크기
       와 파일 시스템 이미지의 블록 크기가 다를 경우에는 충분한 성능을 기대하기 어렵다. 마지
       막으로, 처리 과정 중에 긴 출력 메시지가 나타나고 종료된 후에는 JI叩S2 파일 시스템 이미
       지의 크기가 기존의 이미지보다 60%나 줄어든 것을 볼 수 있다. 한정된 플래시 메모리 공간
       에서 작업할 경우에는 이 차이가 매우 크게 느껴질 것이다．

      ［리스트 10-15］에 나와 있는 커맨드 라인에 전달된 플래그 중에서 짚고 넘어가야 할 것이
       하나 있다. -b 플래그는 -bi于endian을 줄여서 쓴 것이다. 이 플래그는 mkfs.jffs2 유틸
       리티가 JFFS2 플래시 이미지를 만들 때 박엔디언（b培-endian) 시스템에서 사용하기에
       알맞게 만들도록 해 준다. 지금은 ADI 엔지니어링 코요테 보드를 대상으로 하고 있기 때문
       에 , 이 부분이 아주 중요하다. 만약에 박엔디언으로 설정하지 않으면 커널이 JFFS2 파일
      시스템의 슈퍼 블럭（superbiock）을 인식하려고 시도할 때 수페이지에 달하는 경고5) 메시
      지를 출력하는 것을 볼 수 있을 것이다. 필자가 이 문제에 대해서 이렇게 자세히 기억하는
      이유를 알 것 같지 않은가'7

      이전 예제와 비슷한 방식으로 이 이미지를 Redboot RootFS 플래시 파티션에 복사하기 위
      해서 flashcp 유틸리티를 이용하면 된다. 그러면 JFFS2 루트 파일 시스템으로 리눅스 커널
      을 부팅시킬 수 있다. ［리스트 10-16］은 우리 보드에서 MTD 유틸리티를 실행한 결과를
      자세히 보여 주고 있다．

      ［리스트 ]0-16) JFFS2 이미지를 RootFS 파티션에 복사하'I


         root@coyote: 硝 cat /proc/mtd
         dev:     size  erasesize name
         nitdO: 00060000 00020000 'rRedBoot '
         mtdl: 00160000 00020000 "MyKernel "
         mtd2: 00600000 00020000 "RootFS"
         mtd3: 00001000 00020000 "RedBoot config"


5) 물론 커널을 다른 엔디언을 사용하는 MTD 시스템에서 동작하게 만들 수 있다. 성능샹의 손해는 있지만, 일부 환경（멀티 프로세
   서를 이용하는 경우）에는 아주 유용한 기능이다．
 聽1     Embedded Linux Primer



        mtd4: 00020000 00020000 'FIS directory"
        root@coyote: # flash_erase /dev/mtd2
        Erase Total 1 Units
        Performing Flash Erase of length 131072 at offset OxO done
        root@coyote: # flashcp /rootfs. jffs2 /dev/mtd2
        root@coyote : 硝



      중요한 점은 리눅스 커널 구성에서 JFFS2 파일 시스템을 사용할 수 있도록 설정해야 한다
      는 점이다. make ARCH=<arch> gconfig를 실행해서 File Systems의 入liscellaneous
      File Systems 아래에서 JFFS2를 선택하면 된다. 또 다른 힌트는 MTD 유틸리티를 실행
      할 때 -v 옵션을 주는 것이다. 그러면 플래시를 업데이트하는 과정 및 기타 동작에 대한 유용
      한 정보를 출력한다．

      Redboot의 exec 명령어를 이용해서 커널을 부팅하는 것은 이미 살펴봤다. ［리스트 10小
      17］은 새로운 JFFS2 파일 시스템을 루트 파일 시스템으로 설정해서 리눅스 커널을 로드하
      고 부팅하는 과정을 나타낸 것이다．

      ［리스트 ]0-17) JFFS2릍 루트 파일 시스템으로 부팅하71

        RedBoot> load -r -v -b 0x01008000 coyote- zltnage
        Using default protocol (TFTP)
        Raw file loaded 0x01008000-0x0ll4decb, assumed entry at 0x01008000
        RedBoot> exec -c "console=ttySO,115200 rootfstype=jffs2 root=/dev/mtdblock2"
        Using base address 0x01008000 and length 0x00145ecc
        Uncompressing Linux         done, booting the kernel.




10.5 요약
        口 메모리 기술 저장 장치（MTD) 서브 시스템은 플래시 메모리 등의 메모리 장치를 리눅스
            커널에서 사용할 수 있도록 해 준다．

        口 커널 구성 옵션에서 MTD를 활성화시켜야 하는데, 몇 장의 그림을 통해써 이 구성 옵션
            어］ 대해 자세히 설명했다．
                                                                MID 서브시스템       Chapter 10



       口 MTD 커널 구성의 일부 과정으로서 독자가 사용하는 플래시 IC에 맞는 플래시 디바이스
          드라이버를 선택해야 한다. ［그림 10느시에서 최신 리눅스 커널이 지원하는 플래시 IC
          드라이버를 볼 수 있다．

       口 플래시 메모리 장치를 하나의 큰 단일 공간으로 사용할 수도 있고, 여러 개의 파티션으로
          나눌 수도 있다．

       口 리눅스 커널에서 MTD 파티션에 대한 정보를 주고받기 위한 몇 가지 방법이 있는데, 여
          기에는 Redboot 파티션 정보나 커널 커맨드 라인 파라미터를 이용하는 방법 , 매핑 드라
          이버를 이용하는 방법 등이 있다．

       口 자신의 보드와 아키텍처어］ 맞는 정보를 갖고 있는 매핑 드라이버는 플래시 구성 정보를
          커널에 전달해1 준다．

       口 MTD 프로젝트에는 플래시 장치어］ 있는 이미지를 관리하기 위한 사용자용 유틸리티들이
          포함되어 있다．

       口 저널링 플래시 파일 시스템 2(JFFS2）는 작고, 효율적인 플래시 기반 파일 시스템이며，
         MTD 서브 시스템과 잘 어울린다. 이 장에서는 JFFS2 이미지를 하나 만들어서 타깃 시
         스템에 루트 파일 시스템으로 마운트해서 사용했다．



10,5. ] 더 읽01 보기
       MTD 리눅스 홈페이지
       www. linux-mtd.infradead. org/


       Redboot 사용자 문서
       http: //ecos. sourceware. org/ecos/docs-latest/redboot/redboot-guide. html

       공용 플래시 인터페이스（CFI) 스펙 문서
       AMD 사
       www.amd.com/us-en/assets/content_type/DownloadableAssets/cfi_r20.pdf




                                                                                    343   I
                   BusyBox



이번 장에서 배울 내용

  1 BusyBox 소개

  1 BusyBox 구성하기

  1 BusyBox의 기능

  1 요약
 纛繫a.     Embedded 니flux I개mer




        BusyBox에 관한 man 페이지에는 BusyBox를 "임베디드 리눅스의 스위스 군용 칼1) "이라
        고 소캐하고 있다. 맞는 말이다, BusyBox는 방대한 표준 리눅스 커맨드 라인 유틸리티를
        대체할 수 있는 작고 효율적인 툴이다. 또한 제한된 자원을 가진 임베디드 플랫폼에서는 기
        반 툴로서 사용되기도 한다. 이 장에서는 BusyBox를 소개하고 BusyBox를 자신에게 맞게
        설치할 수 있는 방법을 알아본다．

        이미 이 책의 여러 곳에서 BusyBox에 대해서 언급한 적이 있다. 이 장에서는 이 유용한 툴
        패키지에 대해서 자세히 알아보도록 하자. 간단히 BusyBox를 소개한 후에 BusyBox 구성
        유틸리티를 알아보겠다. 이 구성 유틸리티는 자신의 요구에 맞게 BusyBo욜 구성할 때 사
        용된다. 그 다음에는 Bi娼yBox 패키지를 대상 시스템에서 사용할 수 있도록 교차 컴파일하
        기 위해서 필요한 조건들에 대해서 살펴볼 것이다．

        BusyBox7} 임베디드 시스템에서 어떻게 사용되는지를 포함해서 , BusyBox의 동작 방식에
        대해서 생각하1 볼 것이다. Bt娼yBox가 초기화되는 과정을 실험해 보고, 표준 시스템 V 설치
        와 다른 점을설명한다. 이 섹션에서는, 초기화 스크립트의 예제를 하나 제시하겠다. 그리고
        BusyBox를 설치하는 과정을 본 다음에는 BusyBox 명령어와 그 명령어들이 갖는 한계점에
        대해서도 알아보자．



] ].1 BusyBox 소개
        BusyBox는 임베디드 리눅스 커뮤니티에서 엄청난 인기를 얻고 있다. 구성하고 컴파일해서
        사용하는 절차가 무척 쉽고, 적은 시스템 자원만을 가지고도 많은 종류의 리눅스 유틸리티
        집합을 사용할 수 있게 해 준다. BusyBox는 대부분의 데스크탑 리눅스나 임베디드 리눅스
        배포 버전에서 볼 수 있는 기본적인 유틸리티 집합을 대체할 수 있는 작은 크기의 프로그램이
        다. 이 유틸리티에는 is, cat, cp, dir, head 그리고 tail 등의 파일 유틸리티가 포함
        되고, 일반 유틸리티로는 dmes아 kill, hal七， fdisk, mount, t끄noun七 등이 있다. 또
        한 더 복잡한 유틸리티인 ifconfig, ne七S七a七； rou七e 등의 네트워크 유틸리티도 있다．

        BusyBox는 모듈 방식으로 되어 있어서 , 자신의 시스템의 요구 조건에 맞도록 아주 세밀하
        게 구성할 수 있다. 패키지에는 리눅스 커널을 구성하는 것과 비슷한 구성 유틸리티가 포함
        되어 있어서 , 매우 친숙하게 느껴질 것이다．

1) （역자주） Swiss army kn侃 : 일명 맥가이버 칼이라고 불리는 칼로． 칼 외에 다양한 도구가 모여 있다．
                                                          BusyBox   Chapter 11




       물론 BusyBox에 포함된 명령어들은 일반 리눅스 명령에 집합에 있는 같은 기능을 하는 유
       틸리티보다는 훨씬 간단한 버전이다. 그리고 일부 경우에는 커맨드 라인 옵션 중의 일부만
       지원하기도 한다. 하지만 실제 일반 임베디드 시스템에서 사용해 보면 BusyBox가 지원하는
       명령에 집합의 기능으로도 충분하다는 것을 알 수 있다．


11.1.1 BusvBox는 쉽다
       리눅스 커널을 구성해서 빌드하는 방법을 알고 있다면 BusyBox를 구성하고 빌드 및 설치하
       는 것도 쉽게 할 수 있다. 방법도 비슷하다．

          1. 구성 유틸리티를 실행시켜서 필요한 기능을 선택한다．
          2. 의존성에 대한 정보를 생성하기 위해써 make dep을 실행한다．
          3. 패키지를 빌드시키기 위해서 make를 실행한다．
          4. 바이너리 및 심볼릭 링크2）를 대상 시스템에 설치한다．

       깨발 워크스테이션 또는 대상 타깃 임베디드 시스템에서 BusyBox를 빌드 및 설치할 수 있다．
       BusyBox는 두 가지 환경 모두에서 잘 동작한다. 하지만, 대상 워크스테이션에 BUSYBO욜
       설치할 때는 작업 디렉터리 내에 고립된 위치에 설치하도록 주의해야 한다. 이는 시스템의 스타
       트업 파일들이나 주요 유틸리티들을 덮어쓰는 경우가 있을 수 있기 때문이다．



] ] .2 BusyBox 구성하기
      BusyBox를 구성하기 위해서는 리눅스 커널에서 ncurses3) 라이브러리 기반의 구성 유틸
      리티를 실행시킬 때 사용하는 명령어와 같은 명령을 이용한다．

         $ make menuconfig

      ［그림 11-1J은 BusyBox 구성 유틸리티의 최상위 항목을 보여 주는 그림이다．




2) 심볼릭 링크어］ 대해서는 잠시 후어］ 자세히 설명하겠다．
3) （역자주） 문자 기반의 쉘에서 화면을 마치 GUI처럼 꾸밀 수 있도록 해 주는 라이브러리이다．
驪 mm       Embedded Linux Primer



        File   Edit    View   Term佃al   Tabs




               Arrow keys navigate the menu. <Enter> selects subsenus --->.
               Highlighted letters are hotkeys. Pressing <'1> selectes a feature,
               while <N> will exclude a feature. Press <Esc><Esc> to exit, <?> for
               Help, <I> for Search. Legend: [口 feature is selected [ I feature is

                                  Gen日al Conf " . 1 ation
                                   uild Options --->
                                   nstallation Options --->
                                    rchival Utilities    -斗山＞
                                    oreutils --中>
                                    onsole Utilities    --->
                                    ebian Utilities    ---,
                                    ditors --->
                                    inding Utilities    --->
                                    nit Utilities   --->
                                    0gmn/Password Management Utilities
                                  14 scellaneous Utilities       --->
                                    inux Module Utilities      --->
                                  N tworking Utilities      ---.>
                                    rocess Utilities    --小>
                                    nother Bourne-like Shell --->
                                    ystem 如ggil培 Utilitie$ 中HH>
                                    inux System Utilities      --->
                                    ebugging Options --->

                               oad an Alternate Configuration File
                               ave Configuration to an Alternate File


                                                 <Exit>       < H




        I 그림 j］녀 BusyBox 구성 유틸리티의 최샹위 메뉴


        지면 관계상 모든 구성 옵션을 다룰 수는 없다. 하지만, 일부 언급이 필요한 옵션은 짚고 넘
        어가도록 하자. BusyBox 구성 옵션 중에서 일부 중요한 항목은 Build 0pti이-is 아래에서
        찾아볼 수 있다. 여기서 BusyBox 어플리케이션을 교차H컴파일하기 위해서 필요한 옵션을
        찾을 수 있는데 , ［리스트 11-1］은 최신 리눅스 스냅 샷에서 이 Build0F此ions 아래에 있는
        항목들을자세히 나타낸 것이다. BusyBox 구성 유틸리티에서 Build Options 메뉴를 선택
        하면 이 화면을 볼 수 있다.

        ［리스트 ]卜］) BusyBox 빌드 옵션

                   ]
               [ [
                       Build BusyBox as a static binary (no shared libs)
                       Build with Large File support (for accessing files > 2 GB)
                   기
               L
               r   ]
                   J
                       Do you want to build BusyBox with a Cross Compiler?
               0       Any extra CFLAGS options for the compiler?




難 348
                                                               BusyBox   Chapter ] ]




    첫 번째 옵션은 아주 제한된 자원을 가진 임베디드 시스템을 만드는 데 유용하게 사용할 수
    있다. 이 옵션을 선택하면 BusyBox를 정적으로 컴파일 및 링크해서 , 대상 시스템에서 실행
    시킬 때 동적 라이브러리（libc-2.3. 3. so 등） 없이도 실행할 수 있도록 해 준다. 이 옵션
    을 선택하지 않으면 BusyBox를 실행하기 위해서 몇 가지 라이브러리도 같이 필요하게 된
    다. ldd 명령을 이용하면 BusyBox를 실행하는 데 필요한 라히브러리에는 어떤 것들이 있
    는지 쉽게 알아낼 수 있다. ［리스트 11-2］에는 필자의 데스크탑 리눅스 워크스테이션에서
    ldd 명령을 실행한 결과를 나타낸 것이다.

    ［리스트 ]卜2) BusyBox 라이브러리 의존성


      $ ldd busybox
             1inux-gate. so. 1 => (Oxffffe000)
             1ibc. so. 6=> /1ib/tls/ 1ibc. so. 6 (0x42c70000)
             /1ib/ld-linux. so. 2=> /Hb/ld-1inux. so. 2 (0x42c57000)




    위 리스트를 통해서 기본 구성 옵션 값으로 컴파일했을 경우에 ［리스트 11-2］에서 볼 수 있
    는 세 개의 라이브러리가 필요하다는 것을 알 수 있다. 우리는 BusyBox를 정적인 라이브러
    리를 포함하도록 빌드할 것이키 때문에 , ldd 명령을 실행시키면 BusyBox가 동적인 라이브
    러리를 사용하지 않는 다는 메시지만 보게 될 것이다. 다른 말로 하면 실행 파일을 실행시킬
    때 주소 값이 결정되지 않은 심벌들을 위해서 공유 라이브러리를 사용할 필요가 없다는 것이
    다. 이렇게 정적으로 링크하면 루트 파일 시스템에서 작은 부분만을 차지하게 되는데 , 공유
    라이브러리가 필요하지 않기 때문이다. 하지만, 임베디드 시스템을 위한 어플리케이션을 공
    유 라이브러리 없이 빌드한다는 말은 다른 어플리케이션에서 친숙한 C 라이브러리를 같이
    공유할 수 없다는 것을 의미한다．

    ［리스트 11-1]에 있는 다른 옵션에 대해서는 다음 절에서 살펴보도록 하자．


]] .2.1 BusvBox 교차H컴파일하기
    이 장의 맨 앞부분에서 이야기한 것처럼 BusyBox의 개발자는 이 패키지를 교차개발 환경
    에서 사용할 목적으로 만들었다. 그렇기 때문에 이런 환경에서 빌드하는 것이 상당히 쉽게
    되어 있다. 대부분의 경우, 현재 개발 워크스테이션에 있는 교차H컴파일러에 대한 전H지시자
    (prefix）만 지정해 주면 된다. 이는 BusyBox의 구성 유틸리티의 빌드 옵션에서 교斗컴파


                                                                               349 1
   聽1     Embedded Linux Primer




        일러를 이용해서 BusyBox를 빌드하는 옵션伯uild BusyBox with a cros寸compiler）을
        선택하는 방법으로 이루어진다. 이 옵션을 선택하면 교차나컴파일러를 나타내는 자지시자를
        입력하는 옵션을 볼 수 있다. 잔지시자로 입력하는 내용은 교차H개발 환경에 따라서 다른
        데 , 예를 들어 , xscale be- 또는 ppc卜linux- 등이 있다. 이 내용에 대해서는 다음 장에
        서 임베디드 개발 환경을 설명할 때 자세히 다루겠다．

        ［리스트 11-i］에 있는 마지막 옵션은 컴파일러 커맨드 라인에 추가할 옵션을 지정할 때 사
        용한다. 여기에는 디버킹 관련 정보를 생성하도록 하는 옵션(-이이나, 최적화 단계를 설정하
        는 옵션（예를 들어 , 느02) 또는 대상 시스템과 자신만의 리눅스 시스템에 필요한 컴파일러
        옵션을 입력할 수 있다．



11.3 BusyBox의 기늉
        BusyBox를 빌드하면 최종적으로 bus ybox라는 이름의 바이너리 파일이 만들어진다．
        BusyBox는 이 바이너리 실행 파일 이름으로 실행시킬 수도 있치만, 일반적으로 심볼릭 링크
        (symlink）를 통해서 실행된다. BusyBox를 아무런 인자 없이 실행시키면 현재 빌드된 버전에
        서 사용할 수 있는 기능의 목록을 볼 수 있다. ［리스트 11寸3］은 바로 이 출력 내용을 나타낸
        것이다（책의 너비에 맞게 살짝 형식을 수정했다）.

        ［리스트 ]卜3) BusyBox 실행


          root@coyote # ./busybox
          BusyBox vl. 01 (2005.12. 03-18: 00+0000) multi-call binary

          Usage: busybox [function] [arguments] . . .
            or: [function] [arguments] . . .

            BusyBox is a multi-call binary that combines many common Unix
            utilities into a single executable. Most people will create a
            link to busybox for each function they wish to use and BusyBox
            will act like whatever it was invoked as!

           Currently defined functions:
            [, ash, basename, bunzip2, busybox, bzcat, cat, chgrp, chmod,
             chown, chroot, chvt, clear, cmp, cp, cut, date, dd, deallocvt,
             df, dirname, dmesg, du, echo, egrep, env, expr, false, fgrep,



I 350
                                                         BusyBox   Chapter 11



    find, free, grep, gunzip, gzip, halt, head, hexdump, hostname,
    id, ifconfig, mnit, install, kill, killall, kiogd, linuxrc, ln,
    logger, is, mkdir, mknod, mktemp, more, mount, my, openvt, pidof,
    ping, pivot_root, poweroff, ps, pwd, readlink, reboot, reset,
    rm, rmdir, route, sed, sh, sleep, sort, strings, swapoff, swapon,
    Sync, sysiogd, tail, tar, tee, test, time, touch, tr, true, tty,
    umount, uname, uniq, unzip, uptime, usieep, vi, wc, wget, which,
    whoami, xargs, yes, zcat



［리스트 11-3］을 통해서 , 현재 BusyBox 빌드에서 사용할 수 있는 기능에는 어떤 것들이
있는지 볼 수 있다. 사용할 수 있는 기능은 （아주 작은 메모리만 사용하도록 최적화된 쉘인）
ash부터 압축된 파일을 압축 해제하기 위해서 사용되는 zcat까지 알파벳 순서로 나열되어
있다. 이 기능들이 현재 이 BusyBox 스냅 샷에서 사용하도록 구성된 기본 유틸리티들이다．

각각의 기능을 실행시키기 위해서는 bus ybox를 실행할 때 각 기능의 이름을 인자로 전달하
면 된다. 즉, 현재 디렉터리의 내용을 나열하고 싶으면 다음과 같이 입력하면 된다．

  [root@coyote] # ./busybox is


［리스트 11-3］에 있는 BusyBox 사용법에 대한 메시지에서 또 한 가지 중요한 부분은 프로
그램에 대한 간단한 설명 문구이다. 이 문구에는 BusyBox7} 여러 일반 유틸리티들을 하나
의 단일 실행 파일로 묶은 다중 호출 바이너리 파일이라고 설명하고 있다. 앞에서 언급한 심
볼릭 링크의 용도가 바로 이것이다. 즉, BusyBox에서 실행시키려는 기능과 같은 이름을 갖
는 심볼릭 링크에 의해서 호출되도록 되어 있는 것이다. 이렇게 하면 어떤 기능을 호출할 때
마다 두 개의 단어를 입력하는 번거로움을 없앨 수 있을 뿐만 아니라, 사용자에게 기존에 사
용하던 비슷한 기능의 유틸리티를 친숙한 명령에 형태로 사용자에게 제공할 수 있다. ［리스
트 11-4］와 ［리스트 11-5］를 보면 더 명확하게 이해할 수 있을 것이다．

［리스트 ]卜4) BusyBox의 심볼릭 링크 최상위 구조

   [root@coyote] $ is -i /
  total 12
  drwxrwxr- x 2 root root 4096 Dec 3 13: 38 bin
  lrwxrwxrwx 1 root root 11 Dec 3 13: 38 linuxrc -> bin/busybox
  drwxrwxr- x 2 root root 4096 Dec 3 13: 38 sbin
  drwxrwxr- x 4 root root 4096 Dec 3 13: 38 usr



                                                                        351
        Embedded Linux Primer



      ［리스트 11-4］는 BusyBox 패키지에서 make ins乞all을 실행해서 만들어진 디렉터리 구
      조를 보여 준다. busybo>< 실행 파일은 /bin 디렉터리에서 볼 수 있고, /bin/busybox를
      가리키도록 되어 있는 심볼릭 링크 파일들은 전체 디렉터리 구조에서 찾아볼 수 있다. ［리스
      트 11-夙는 ［리스트 11-4］의 디렉터리 구조를 모두 펼쳐 본 것이다．

      ［리스트 ] 1-5J BusyBox의 심볼릭 링크를 트리 형태로 자세히 나타낸 것

         [root@coyote] $ tree

             bi n
             H- ash -> busybox
             I- - busybox
             I- - cat -> busybox
             H- cp -> busybox

             ' m1 zcat -> busybox
             1inuxrc -> bin/busybox
             sbjn
             I- - halt -> . ./bjn/busybox
                  ifconfig -> . ./bjn/busybox
                  1nit -> . ./bin/busybox
             1 11klogd -> . ./bin/busybox

             'e1syslogd 寸> . ./bin/busybox
             usr                                        n




                 bjn
                 I- - [ -> . ./. ./bin/busybox
                 I- - basename -> . .1. ./bjn/busybox

                  I-- xargs -> . .1. ./bin/busybox
                  111yes -> . .1. ./bin/busybox
                   sbjn
                  ' 11 chroot -> . ./. ./bn/ busybox



      위 ［리스트 11-5］는 전체 내용이 3페이지에 달하기 때문에 가독성을 위해서 상당 부분 생략
      한 것이다． 각 줄에서 생략 기호 ( . . .）로 표시된 부분은 해당 디렉터리에 있는 항목 중에서
      맨 앞부분과 뒷부분을 제외하고는 모두 생략된 것을 나타낸다. 실제로 BusyBox 구성 유틸
      리티에서 활성화시킨 기능에 따라서 100개 이상의 심볼릭 링크 항목이 생성될 수도 있다．


352
                                                 BusyBox   Chapter 11




      ibmn 디렉터리의 두 번째 항목인 bus ybox는 자체적으로도 실행시킬 수 있는 파일이다. 또
      한 /bin 디렉터리에는 bus ybox를 다시 가리키는 ash, cat, cp에서 zca七 등에 이르는
      심볼릭 링크도 포함되어 있다. 다시 말하지만 cp에서 zcat 사이는 지면 관계상 생략되었다．
      이 심볼릭 링크 구조를 이용해서 사용자는 실제 기능을 실행시키는 유틸리티를 간단하게 호
      출할 수 있다. 예를 들어 , busybox ifconfig 유틸리티를 이용해서 네트워크 인터페이스
      를 설정한다고 할 때 사용자는 다음과 비슷한 명령을 입력해야 한다．

         $ ifconfig ethi 192.168.1.14


      위 명령은 ifconfig라는 이름의 심볼릭 링크를 통해서 busybo>< 실행 파일을 실행시키게
      된다. Busybox에서 첫 번째 인자로 들어오는 이름을 실행시킬 기능을 나타내는 데 사용한다．


11.3.1 BusyBox mn仕
      ［리스트 11-5］에는 mni七이라는심볼릭 링크가 있다. 6장, "시스템 초기화'에서 시스템 초기
      화 과정에서 mni七이라는 프로그램의 역할에 대해서 알아보았다. 즉, 커널은 커널 초기화 과
      정의 마지막 단계로 /sbin/init이라는 프로그램을 실행시킨다. 여기서 BusyBox가 이
      mnit 프로그램의 기능을 수행하지 못할 이유가 없다. 그리고 ［리스트 11-夙에서 사용된 시
      스템은 바로 mni七 프로그램의 기능을 수행하는 경우이다．

      BusyBox는 표준 시스템 Vin北과는 다른 방식으로 시스템을 초기화하는데 , 6장에서 설명
      한 것처럼 시스템 V(SysV) 초기화를 사용하는 시스템은 /e七C 디렉터리의 inittab이라는
      파일에 접근할 수 있도록 제공해 주어야 한다. 물론 BusyBox 또한 mni七七ab 파일을 읽어
      들이지만, 시스템 V의 mni七七ab 파일과는 문법이 다르다. 일반적으로 BusyBox를 쓸 때
      mni七tab 파일이 꼭 필요한 것은 아니다. BusyBox의 man 페이지에 나와 있듯이 동작 레
      벨（run level) 기능을 사용하려면 시스템 V 방식의 초기화4）를 이용해야 한다．

      임베디드 시스템에서는 어떨지 생각하1 보자. 우리는 BusyBox에 기반한 작은 루트 파일 시
      스템을 하나 만들어 쓸 수 있다. 이 때 BusyBox를 정적으로 링크하도록 해서 공유 라이브러
      리가 따로 필요하지 않도록 한다. ［리스트 11-6］은 이 루트 파일 시스템의 내용을 나타낸
      것이다. 이 작은 파일 시스템 이미지는 9장, "파일 시스템"의 9.10절 "간단한 파일 시스템
      만들기" 절에서 소개한 방식대로 만든 것이라서 따로 설명하지는 않겠다. 이 간단한 파일 시
      스템이 가지고 있는 파일은 ［리스트 11-6］에 있는 것과 같다.

4) 시스템 V 초기화에 대해서는 6장에서 자세히 설명했다．
礪U      Embedded Linux Primer



      ［리스트 ]卜6) 최소 BusyBox 루트 파일 시스템

        $ tree

        I- - bin
        I    I- - busybox
        I    I寸- cat -> busybox
        I    I-口 dmesg -> busybox
        I    I- - echo -> busybox
        I    I- - hostnarne -> busybox
        I    I 尸 ]S 小＞ busybox
        I    I-中 ps -> busybox
        1    I- - pwd -> busybox
        I    ' U口 sh -> busybox
        I- - dev
        1    ' 11console
        I- - etc
        ' 4m proc
        4 directories, 10 files



      이 BusyBox 기반의 루트 파일 시스템은 busybox 자체가 차지하는 것보다 조금 더 많은
      공간을 차지한다. 이 구성에서는 정적으로 링크를 시켰고, 100개 정도의 유틸리티를 지원하
      는데도 BusyBox 실행 바이너리 파일의 크기가 1MB도 채 안 되는 것을 볼 수 있다．



         # is -i /bin/busybox
         -rwxr-xr- x  1 root root        824724 Dec   3   2005 /bin/busybox



      그럼 시스템이 어떻게 동작하는지 보도록 하자. ［리스트 11-끼은 BusyBox 기반의 임베디
      드 시스템에서 전원을 켰을 때 출력되는 콘솔 메시지를 나타낸 것이다．

      ［리스트 ]卜7) BusyBox 시작



         Looking up port of RPc 100003/2 on 192.168.1. 9
         Looking up port of RPC 100005/1 on 192.168.1.9
         VFS: Mounted root (nfs filesystem) .



354
                                                               BusyBox   Chapter ii



   Freeing 卄너t memory: 96K
   Bummer, could not run '/ etc/init. d/ rcS ' : NO such file or directory
   Please press Enter to activate this console.



  BusyBox vi. Ol (2005.12.03-19:09+0000) Built-in shell (ash)
  Enter 'help ' for a list of built- in commands.

   -sh: can 't access tty; job control turned off
   /#
［리스트 11-기에 나온 예제는 NFS를 이용해서 루트 파일 시스템을 마운트해서 사용하는
임베디드 시스템에서 동작시킨 것이다. ［리스트 11-6］에 있는 간단한 파일 시스템 이미지를
갖고 있는 디렉터리를 외부로 노출（export）시켜서 부트 과정의 마지막 단계 중의 하나로서
리눅스 커널이 NFS를 통해서 타깃 보드의 루트 파일 시스템을 마운트할 수 있도록 한다．
커널이 /sbin/ini七을 실행시키려고 하지만 파일 시스템에서는 /sbin/ini七이 없기 때문
에 실패한다. 하지만 아는 바와 같이 커널은 다음으로 /bin/ sh도 실행시키려고 시도하기
때문에 , 루트 파일 시스템의 /bin／針1 심볼릭 링크를 통해서 busybox7} 실행된다．

BusyBox가 처음 출력하는 내용은 /e七c/mnit. d/rcS라는 파일을 찾을 수 없다는 불평 메
시지인데 , 이 파일은 BusyBox가 기본 초기화 스크립트로사용하기 위한 것이다. BusyBox
에 기반한 임베디드 시스템을 초기화하는 방법으로 mni七七ab보다 이 파일이 더 애용된다．

초기화를 마친 후에 BusyBox는 사용자에게 콘솔을 활성화시키려면 (Enter）키를 누르라는
메시지를 출력한다. 그리고 (Enter）키를 누르면 사용자 입력을 기다리며 대기하는 ash 쉘
프로그램을 실행시킨다. BusyBox의 마지막 메시지로는 시리얼 터미널에 시스템 콘솔을 만
든 결과가 출력된다. 리눅스 커널은 시리얼 터미널에서 콘솔을 사용할 경우에는 부팅 후에
실행시키도록 되어 있는 프로그램을 실행하치 않도록 하는 코드를 가지고 있다．

위 예제를 통해서 거의 100개에 딜하는 리눅스 유틸리티를 쓸 수 있는 실제 동작하는 시스템
을 만들어 보았다. BusyBox에서 사용할 수 있는 유틸리티로는 코어 (core) 유틸리티 , 파일，
네트워크 지원을 위한 유틸리티는 물론이고 합리적인 기능을 가지고 있는 쉘 프로그램도 포
함된다. 보는 바와 같이 이 간단한 Bi娼yBox 패키지만으로도 자신만의 어플리케이션을 빌드
해서 사용할 수 있을 정도의 강력한 플랫폼을 제공한다. 물론 libc와 기타 시스템 라이브러



                                                                             355I
        Embedded Linux Primer




      리는 가지고 있지 않기 때문에 어플리케이션을 구현하는 것이 만만치 않을 것이다. 그렇기
      때문에 일반 C 프로그램에서 사용하는 시스템 콜이나 기타 라이브러리 함수들을 제공해야
      한다. 물론 다른 방법으로 어플리케이션을 링크할 때 정적으로 링크시키면 되지만, 이렇게
      청적으로 링크시킨 프로그램이 두 7긔 이상이 된다면 동적으로 링크해서 공유 라이브러리를
      사용하는 시스템에서 공유 라이브러리와 프로그램 크기를 합친 것보다 더 많은 공간5）을 차
      지할 것이다．


11.3.2 rcS 초기화 스크립트 예제

      BusyBox는 사용자 쉘을 실행시키기 전에 ［리스트 11寸7］에서 보는 것처럼 /e七c/init. d/
      rcS라는 이름의 스크립트 파일에 있는 내용을 먼저 실행시키려고 시도한다. 이 파일에서 어
      플리케이션을 실행시키도록 할 수 있다. ［리스트 11-8］에 간단한 rcS 초기화 스크립트를
      나타냈다．

     ［리스트 11-8) rcS 시작 스크립트 예제


        判 /bin/ sh

        echo "Moundng proc '
        mount -t proc /proc /proc

        echo "starting system loggers "
        syslogd
        klogd

        echo "configuring loopback interface "
        ifconfig lo 127. 0. 0. 1

         echo "starting inetd"
         xi netd

         # start a shell
         busybox sh




5) （역자주） 정적으로 링크시키면 라이브러리 팟큰그램마다 코드가 각각의 포함되기 때문에 ，정적으로 링크된 프로그램이 2개 있다
   면 공유 라이브러리를 사용하는 시스덛浬r+ 공간을 더 차지하게 된다．
                                                               BusyBox   Chapter 11



       이 스크립트는 이해하기 쉬운 내용으로 되어 있는데 , 먼저 약속된 마운트 지점인 /proc어］
       /proc 파일 시스템을 마운트하는 게 중요하다. 이는 많은 유틸리티들이 정보를 얻어오는
       데 /proc 파일 시스템을 이용하기 때문이다. /proc 파일 시스템에 대해서는 9장에서 살펴
       본 적이 있다. 다음으로는 시스템 로거를 최대한 빨리 실행시켜야 하는데 , 부팅 중에 어떤
       문제가 생겼을 때 그 내용을 기록해 두기 위함이다. 시스템 로그를 실행한 다음에는 로컬 루
       프백(local loopback) 인터페이스를 설정한다. 이 역시도 기존 리눅스의 많은 기능들이 루
       프백 인터페이스가 있다고 가정하고 동작하기 때문이다. 또한 시스템에서 소켓6) (socket）을
       사용하도록 구성한 경우에도 이 인터페이스를 사용할 수 있도록 해 주어야 한다. 쉘을 실행
       시키기 전에 마지막으로 하는 일은 인터넷 슈피서버인 xinetd를 실행시키는 것이다. 이 프
       로그램은 모든 네트워크 인터페이스에서 네트워크 요청이 들어오는지를 감시하는 일을 한다.
       예를 들어 , 보드로 telnet 연결을 요청하면 xinetd가 그 telnet 요청을 가로채서 앞으로
       의 요청을 처리할 수 있는 텔넷 서버를 실행킨다．

       rcS 초기화 스크립트를 수정해서 쉘을 실행시키는 대신에 자신만의 프로그램이 실행되도록
       설정할 수도 있다. ［리스트 11-8］은 시스템 및 커널 로거 등의 기본 서비스가 실행되고，
       telnet 접속이 가능한 타깃 시스템의 예제를 나타낸 것이다．


11.3.3 BusvBox릍 타깃 보드에 설치하기
       BusyBox를 설치하는 과정을 이야기하려면 먼저 심볼릭 링크의 목적과 사용법을 이해해야
       한다. BusyBox의 makefile은 install이라는 타깃을 가지고 있는데 , make install을
       실행하면 busybo>< 실행 파일과 심볼릭 링크 구조를 포함하는 디렉터리 구조를 생성한다．
       이 환경을 독자의 타깃 임베디드 시스템의 최상위 디렉터리에 통합시켜야 한다. 설치를 통해
       서 생기는 심볼릭 링크 구조를 이용하면 각각의 명령어마다 busybox를 입력할 필요 없이
       사용할 수 있다. 즉, 사용자가 어떤 디렉터리의 내용 항목을 보려고 할 때 is만 입력하면
       되는데 , 이전에 설명한 것처럼 해당 심볼릭 링크가busybox의 ls를 실행시킨다. 심볼릭 링
       크의 전체 구조를 다시 보려면 ［리스트 11-4］와 ［리스트 11-旬를 보기 바란다. 주의할 점은
       BusyBox의 빌드 시스템은 구성 유틸리티에서 활성화된 기능에 대해서만 자동으로 심볼릭
       링크를 만든다는 것이다．




6) ［역자주） 네트워크를 위한 AP匿 sock아이라고 한다. 원래는 버클리 釵cket0］서 유래한 것이다．
        Embedded Linux Primer




      이와 같이 사용하는 루트 파일 시스템에서 가장 쉽게 필요한 심볼릭 링크를 만드는 방법은
      BusyBox 빌드 시스템을 이용하는 것이다. 간단히 루트 파일 시스템을 개발 시스템에 마운
      트시켜서 , BusyBox의 makefile을 실행시킬 때 PREFIX라는 이름의 인자를 통해서 대상
      위치를 전달하면 된다. ［리스트 11-9：에서 이 절차를 볼 수 있다．

      ［리스트 ] 1-9] 루트 파일 시스템에 BusyBox 설치하기


        $ mount -o loop bbrootfs.ext2 /mnt/ remote
        $ make PREFIX=/mnt/ remote install
        /bin/ sh applets/install . sh /mnt/ remote
          /mnt/ remote/bin/ash -> busybox
          /mnt/ remote/bin/cat 口> busybox
          /mnt/ remote/bin/ chgrp -> busybox
          /mnt/ remote/bin/ chmod -> busybox
          /mnt/ remote/bin/ chown -> busybox

         /mnt/ remote/usr/biri/ xargs -> . .1. ./bin/busybox
         /mnt/ remote/usr/bin/yes -> . .1. ./bin/busybox
         /mnt/ remote/usr/ sbin/chroot -> . ./. ./bin/busybox




         You will probably need to make your busybox binary
         setuid root to ensure all configured applets will
         work properly.



        $ chmod +s /mnt/ remote/bin/busybox
        $ls -l /mnt/ remote/bin/busybox
        -rwsr-sr- x 1 root root 863188 Dec 4 15: 54 /mnt/ remote/bin/busybox




      먼저 루트 파일 시스템 바이너리 이미지를 원하는 마운트 지점에 마운트한다. 위 예제에서는
      필자가 좋아하는 위치인 /mnt/remo七e를 이용했다. 그리고는 BusyBo혀 make ins七all
      명령을 실행해서 bus ybox 실행 파일과 심볼릭 링크 구조를 생성시킬 디렉터리 위치를
      PREFIX로 전달하1 준다. 이 스크립트를 실행하면 아주 많은 메시치를 출력하는데 , 각 심볼릭
      링크가 생성될 때마다 내용이 한 줄찍 출력된다. 가독성을 위해서 처음과 마지막 일부만 나
      타냈다. 이 내용에서 생략 기호로 나타낸 부분이 바로 생략된 내용을 나타낸다．


358
                                               BusyBox   Chapter 11




    앞에서 출력되는 내용 중에는 setuid에 대한 부분도 있는데 , 바로 busybox 실행 파일의
    se七uid가 루트（root）로 되어 있어야 한다는 것을 알려주고 있다. 이는 Bi.娼yBox를 통해서
    실행시키는 기능 중에서 루트 권한을 필요로 하는 명령을 루트가 아닌 사용자도 호출할 수
    있도록 하기 위함이다. 이 부분은 반드시 해 주어야 하는 것은 아닌데 , 특히 임베디드 리눅스
    환경에서는 시스템에 오직 루트（root) 사용자만 있는 경우가 아주 일반적이기 때문에 별도로
    setuid를 설정해 주지 않아도 퇸다. 독자의 시스템에서 setuid의 변경해야 할 경우에는
    ［리스트 11小9］에서 보듯이 ohm아j+s 명령어를 이용해면 된다．

    Busybox의 설치를 끝마치면 그 결과물로 bus ybO>< 실행 파일과 심볼릭 링크 구조가 대상 ·
    루트 파일 시스템에 생성된다. 최종적인 최상위 디렉터리 내용은 ［리스트 11-4］와 비슷한
    형태가 될 것이다．

    또한 B.娼yBox는 심볼릭 링크 구조를 타깃 시스템이 동작 중일 때도 생성할 수 있는 옵션을
    가치고 있다. 이 옵션은 Bi娼yBox 구성 유틸리티를 통해서 활성화시키고, 시스템 동작 중에
    는 busy奴次를 -ins七all 옵션을 줘서 실행시키면 퇸다. 이 기능을 사용하려면 필요한 정
    보를 위해서 먼저 타깃 시스템에 /proc 파일 시스템이 반드시 마운트되어 있어야 한다．


11.3.4 BusyBox 명령어
    최신 BusyBox 시스템의 man 페이지에는 모두 197개의 명령어（또는 애플릿（ap히et)이라고
    도 한다）가 문서화되어 있다. 그리고 배쉬 (Bash) 쉘 스크립트 등을 포함해서 복잡한 쉘 스
    크립트들을 문제없이 지원할 정도로 충분한 기능을 가지고 있다. BusyBox는 배쉬 스크립트
    에서 자주 사용되는 awk와 sed를 지원한다. 그리고 ping, ifconfig, traceroute,
    nets七a七 등의 네트워크 유틸리티도 지원한다. true, false나 yes 등의 일부 명령어와
    같이 스크립트를 지원하키 위한 용도로만 존재하는 것들도 있다．

    몇 분만 투자해서 부록 C에 있는 "BusyBox 명령에"를 정독해 보면 BusyBox 명령어를 정
    리해 볼 수 있다. 이렇게 어느 정도 전체 명령어를 살펴본 후에는 자신의 임베디드 리눅스
    프로젝트에서 사용할 수 있는 알맞은 BusyBox 기능을 좀 더 잘 이해할 수 있을 것이다．

    이 장의 시작 부분에서 설명한 것처럼 , 많은 BusyBox 명령어가 그와 대응되는 전체 기능을
    가진 유틸리티와 비교해서 제한된 기능과 옵션만을 가지고 있다. 그리고 BusyBox 명령어에
    대해서 도움말이 필요할 때는 --help 옵션을 이용해서 명령을 실행시키면 된다. 이 옵션을
          Embedded Linux Primer



        줘서 명령을 실행시키면 지원되는 옵션에 대한 간략한 정보와 사용법을 볼 수 있다. 제한된
        옵션만을 지원하는 BusyBo ( 명령의 좋은 예제로 gzi1) 애플릿을 들 수 있다. ［리스트
        11-10］은 BusyBox어］ 내장된 gzi1) 명령에 대한 도움말 내용을 나타낸 것이다．

        ［리스트 ] ] 10) BusyBox의 qzip 도움말


           / # gzip --help
           BusyBox vl.01 (2005.12. 01-21: 11+0000) multi-call binary

           usage: gzip [oPTIoN] . . . [FILE] . . .

           Compress FILE(S) with maximum compression.
           놔hen FILE is '- ' or unspecified, reads standard input. Implies -c.

          야）ti ons :
                       c      write output to standard output instead of FILE. gz
                       d      Decompress
                       f      Force write when destination is a terminal



        BusyBox의 gzip은 오직 3가지 커맨드 라인 옵션만 지원하는데 , 대응하는 전체 기능을 가
        진 gzip 버전은 15개의 다른 커맨드 라인 옵션을 지원한다. 예를 들어 , 전체 기능올 가친
        gzip 유틸리티는 명령 프롬프트 상에 압축 파일 내의 각각의 파일에 대한 압축 정보를 보여
        주는 --list 옵션을 지원하지만 BusyBox gzip은 그런 기능을 지원하지 않는다. 하지만
        이 기능은 임베디드 시스템에서는 크게 중요한 기능은 아니다. 여키서 이런 정보를 제공하는
        이유는 BusyBox를 선택할 때 그러한 제약 사항을 알고 있는 게 좋기 때문이다. 만약에 전체
        기능을 가진 유틸리티를 쓰고 싶을 때는 아주 간단히 해결할 수 있다. 즉, BusyBox 구성
        유틸리티에서 그 유틸리티 기능을 제거하고, 대신에 전체 기능을 가진 리눅스 표준 유틸리티
        를 타깃 시스템에 추가하면 된다．




I 360
                                                 BusyBox   Chapter 11




] 1.4 요약
      口 BusyBox는 임베디드 시스템에서 많은 리눅스 유틸리티를 하나의 다중 호출 바이너리
         파일로 대체할 수 있게 해1 주는 강력한 도구이다．

      다 BusyBox를 이용하면 루트 파일 시스템 이미지의 크기를 상당히 줄일 수 있다．

      口 BusyBox는 사용하기가 쉽고 많은 유용한 기능을 가지고 있다．

      口 BusyBox를 구성하는 것도 아주 쉽다. 즉, 리눅스 커널을 구성하는 것과 비슷한 인터페
         이스의 프로그램을 이용한다．

      口 BusyBox는 필요에 따라서 정적으로 링크시키거나, 동적으로 링크시킬 수도 있다.

      口 BusyBox를 이용하면 시스템 초기화 과정이 약간 다르다. 그 차이점에 대해서 이 장에서
         설명했다.

      口 BusyBox는 많은 명령어를 지원하는데, 부록 C에서 최신 BusyBox 릴리즈 버전에 포함
         된 명령어의 전체 목록을 볼 수 있다．



11.4. ] 더 읽어 보기
       BusyBox 프로젝트 홈페이지
       www.busybox.net/


       BusyBox 맨 페이지
       www. busybox.net/downloads/BusyBox.html
Ch圄臂挺伊 ]2



              임베디드 개발 완경




이번 장에서 배울 내용


   교차1개발 환경

   호스트 시스템 요구 사항

   타깃 보드 호스팅하기

   요약
 瑟 a.     Embedded Linux Primer




        호스트 개발 시스템에 어떤 서비스와 환경을 갖추었는치에 따라서 임베디드 개발자가 작업을
        성공적으로 진행하는 데 매우 큰 영향을 미칠 수 있다. 이번 장에서는 교차개발 환경에서
        필요로 하는 특별한 요구 사항과 임베디드 개발자가 좀 더 효율적인 작업을 하도록 도와주는
        툴 및 기술에 대해서 설명하겠다．

        먼저 전형적인 교차나개발 환경을 하나 예를 들어 볼 것이다. 그리고 익숙한 "hello world"
        예제를 이용해서 호스트에서 동작하는 어플리케이션과 임베디드 시스템을 대상으로 한 어플
        리케이션의 차이점에 대해서 살펴볼 것이다. 그리고 호스트 시스템을 위한 툴체인과 임베디
        드 어플리케이션을 위한 툴e체인의 차이점에 대해서도 알아보자. 그 다음에는 호스트 시스템
        이 갖추어야 할 요구 사항과 호스트 시스템에 있는 중요한 구성 요소를 사용하는 방법을 자세
        히 설명하고, 마지막으로 네트워크 기반의 호스트를 이용하는 타깃 보드를 예를 들어 설명하
        는 것으로 마무리하도록 하자.



12. ] 교차m개발 완경
        임베디드 개발을 처음 접하는 개발자는 종종 자체 개발 환경과 교차개발 환경의 차이점을
        어려워하는데 , 이는 실제 세 가치의 컴파일러와 就dlib.h와 같은 표준 헤더 파일이 세 벌
        （또는 그 이상）이나 존재하기 때문이다. 그리고 타깃 임베디드 시스템에서 동작하는 어플리
        케이션을 디버깅할 때 디버깅을 돕는 척당한 툴이나 호스트에서 동작하는 유틸리티 없이는
        디버깅이 아주 어려워진다. 그렇기 때문에 호스트 시스템을 위한 유틸리티 및 관련 파일과
        타깃 시스템에서 사용하도록 만들어진 파일을 별도로 분리해서 관리해야 한다.

        우선 본문에서 호스트（host)라는 용어를 쓸 때는 독자가 좋아하는 리눅스 데스크탑 배포 버전
        이 실행되고 있는 개발 워크스테이션1）을 가리키는 것이다. 반대로 타깃이라는 용어는 독자
        가 사용하는 임베디드 하드웨어 플랫폼을 가리킨다. 그리고 자체 개발（native dev이opment）이
        라고 하면 자신의 호스트 시스템에서 동작하는 어플리케이션을 빌드하는 것을 말한다. 교차U
        개발은 임베디드 타깃 시스템에서 실행시킬 어플리케이션을 호스트 시스템에서 컴파일하고
        빌드하는 것을 말한다. 이 용어들의 정의를 유념해서 이 장의 내용을 읽으면 이해가 더 쉬울
        것이다．


l) 웹스터 사전에서 ' 난센스（non明nse) ' 의 정의를 보면 "올바른 생각에 반대되는 것 또는 터무니없는 생각’이라고 되어 있다. 필자의
 생각에는 임베디드 리눅스 플랫폼을 개발할 때 리눅스／유닉스 호스트를 사용하지 않는 것은 난센스다．
                                                 임베디드 개발 환경    Chapter 12




     ［그림 12-끄은 전형적인 교차e개발 환경의 형태를 보여 준다 호스트 PC는 타깃 보드에 하
     나 이상의 물리적인 연결을 맺고 있는데 , 타깃 시스템에서 시리얼 포트나 이더넷 포트를 모
      두 사용할 수 있는 경우가 가장 편리하다고 볼 수 있다. 나중에 커널 디버깅에 대해서 알아볼
      때 , 이 두 번째 수단인 시리얼 퐈i가 얼마나 중요한 가치를 갖는지 알게 될 것이다．

                               이더넷 허브
         호스트 개발 시스템
          ;   : 叫 二＼ r;:：二그


         느＝ ,：크｝
         ！ 二mma小                RS-232

     I
      I 그림 12-1 교차m개발 환경


      대부분의 경우 RS-232 시리얼 포트로 연결해서 타깃과 통신하거나, 하나 또는 그 이상의
      텔넷 터미널 세션2）을 이용해서 타깃과 통신할 수도 있다. 그리고 이더넷을 연결 매체로 이용
      한 하나 이상의 디버깅 세션을 가질 수도 있다. 이러한 교차e개발 환경 구성은 뛰어난 유연성
      을 제공해 줄 수 있는데 , 기본 아이디어는 호스트 시스템의 컴퓨팅 파워를 활용해서 컴파일
      러 , 디버거 , 에디터 등의 유틸리티를실행시키고, 타깃 시스템에서는자신의 어플리케이션만
      실행시키는 것이다. 물론 타깃 시스템에서 컴파일러나 디버거를 실행시킬 수도 있지만 여기
      서는 호스트 시스템이 램（RAM）이나 디스크 저장 공간, 인터넷 연결 등의 훨씬 더 많은 자원
      을 가지고 있을 것이라고 가정한 것이다. 그리고 사실 타깃 임베디드 보드에 사람이 사용할
      만한 입력 장치나 출력 장치가 없는 경우도 많기 때문이다．


12.1. ] 임베디드 "Hello 小幻rld'
      알맞게 구성한 교차H개발 시스템은 일반 어플리케이션 개발자를 위해서 복잡하고 어려운 부
      분들을 숨겨 준다. 간단한 예를 하나 들어서 살펴보면 불명확한 부분을 어느 정도 이해하는
      데 도움이 될 것 같다. 간단한 "hello world" 프로그램을 컴파일하면 툴 체인（컴파일러 , 링커
      및 기타 유틸리티 등）은 프로그램을 빌드하고 있는 호스트 시스템과 컴파일하고 있는 프로그


2) （역자주） 세션은 어떤 연결이 맺어진 상태라고 생각하면 된다. 텔넷 세션은 텔넷 연결이 이루어져서 서로 통신할 수 있는 채널
   이 구성된 상태를 말한다．
 3三反N      Embedded Linux Primer




         램에 대해서 많은 부분을 가정하게 된다. 여기서 가정이란 실제 가정이 아니라 컴파일러가
         알맞은 바이너리를 만들기 위해서 필요한 규칙들을 가리킨다．

         ［리스트 12-1]에 간단한 "hello world" 프로그램을 보자．

         ［리스트 ]2-1) He加 World 프로그램

           #include <stdio. h>

           mnt main(int argc, char "“中argv)
            {
                printf ('Hello world\n") ;
                return 0;
           }



         일반 어플리케이션 개발자라도 이 C 소스 파일에서 몇 가지 중요한 부분을 알아챘을 것이다．
         첫째로 prin七f () 라는 함수가 사용되고 있지만, 이 파일 내에서 정의되지는 않았다. 이 함
         수의 프로토타입3) (Pr毗毗ype）을 갖고 있는 헤더 파일을 #include 지시어를 통해서 포함
         시키지 않으면 컴파일러는 다음과 같은 친숙한 경고 메시지를 출력한다．

           hello.c: 5: warning: implicit declaration of function 'printf '

         이 메시지를 보면 몇 가지 궁금증이 생기는데．

           口 S七dio.h 파일이 어디에 있는 걸까2 어떻게 찾지7

           口 printf () 함수가 실제로 어디에 존재하는가7 그리고 바이너리 실행 파일에서 어떻게
                참조되는가2


         어쨌든 컴파일러가 스스로 필요한 것들을 모두 모아서 알맞은 바이너리 실행 파일을 만들어
         주는 것 같기는 하다. 여기서 좀 더 복잡한 문제는 최종 바이너리 실행 파일에는 따로 확인하
         지는 못했지만 링커가 자동으로 포함시키도록 되어 있는 시작 및 종료 코드가 포함된다는 것
         이다. 이 시작 부분은 환경 변수나 인자를 프로그램에 넘기는 등의 세부 작업이나. 프로그램
         올 시작하고 종료시키는 일을 관리하는 등의 일을 한다．

3) （역자주） 함수의 형식을 프로토타입이라고 한다. void foo (int a, int b)；와 같이 함수의 인자와 반환 값을 알 수 있는 함수 선언을
  말한다．
                                                       임베디드 개발 환경       Chapter 12



"hello world" 어플리케이션을 빌드하려면 디음과 같이 컴파일러를 실행하는 간단한 명령어
를 입력하면 된다．

  $ 9CC -o hello hello.c


이 명령은 hello라는 바이너리 실행 파일을 만드는데 , 이 실행 파일은 커맨드 라인에서 바
로 실행시킬 수 있다. 컴파일러는 기본 값을 통해서 include 파일을 어디서 가져올지를 결
정한다. 링커도 이와 비슷한 방식으로 참조된 printf () 함수를 어디에 이는 라이브러리를
참조해서 가져올지를 알 수 있다. 물론 이 라이브러리는 표준 C 라이브러리이다．

툴 체인에 해당 명령을 내려서 현재 기본 값이 어떻게 설정되어 있는지를 볼 수 있는데 , ［리
스트 12-2］는 cpp어］ V 옵션을 주고 실행시킨 결과 중 일부를 나타낸 것이다. 아마 cpp
가 gcc 툴 체인에서 C 전처리기를 담당하는 프로그램이라는 것을 알고 있는 독자도 있을
것이다. 다음 내용은 가독성을 위해서 약간 형식을 변형한 것이다．

［리스트 ]2-2] 호스트용 cpp의 검색 위치의 기본 값들


  $ cpp -v
  Reading specs from /usr/lib/ gcc-lib/ 1386- redhat-linux/ 3. 3. 3/ specs
  configured with: . ./configure --prefix=/usr
   L --mandi r=/usr/ share/man --1nfod卄=/usr/ share/i nfo
   L --enable- shared --enable- threads=posix --disable-checking
   니 --di sabi e-li bunwi nd七xcepti에5 --with巧ystem- z］化
   니 --enable- cxa_atexi t -host=i 386- redhat-l i nux

  Thread model : posix
  gcc version 3. 3. 3 20040412 (Red Hat Linux 3. 3. 3-7)
   /usr/lib/ gcc-l化/i386- redhat-linux/ 3. 3. 3/ccl -E -quiet -v -
  ignoring nonexistent directory "/usr/i386- redhat-linux/include"

  #include ". . ." search starts here:
  #include <. . .> search starts here:
   /usr/local/include
   /usr/lib/ gcc-lib/ i386- redhat-linux/ 3. 3. 3/include
   /usr/i nd] ude
  End of search list.
  /usr/lib/




                                                                              367
    難U     Embedded Linux Primer




         앞의 간단한 명령을 통해서 많은 유용한 정보를 볼 수 있는데 , 먼저 컴파일러가
         . /configure 유틸리티를 통해서 어떻게 구성되어 있는지를 볼 수 있다. 즉, 기본 쓰레드
         모델이 포직스（posix）이고 , 그래서 쓰레드를 사용하는 어플리케이션이 링크될 때 포직스
         쓰레드 라이브러리가 사용되는 것을 알 수 있다. 마지막으로 #include 지시자를 위한 기본
         검색 위치도 알 수 있다．

         하지만, 만약에 hello. c를 PowerPC와 같은 다른 아키텍처를 위해서 빌드시키고자 한다
         면 어떻게 해야 할까? PowerPC 타깃을 위해서 어플리케이션 프로그램을 호스트 시스템에
         있는 교斗컴파일러를 이용해서 빌드할 때는 컴파일러가 호스트용 포함（include) 디렉터리
         나 라이브러리 경로를 사용하지 않도록 해야 한다. 즉, 올바로 구성된 교차 컴파일러를 갖추
         는 것이 첫 번째고, 그 다음이 잘 설계된 교차m개발 환경을 갖추는 것이다．

        ［리스트 12-3］은 Denx 소프트웨어 엔지니어링에서 개발 및 관리하고 있는 임베디드 리눅
         스 개발 킷（ELDK : Embedded Linux Development Kit）이라는 인기 있는 오픈中소스
         교차H개발 툴 체인에서 기본 값 정보를 보는 명령어를 실행시킨 결과를 나타낸 것이다. 다음
         의 경우는 Powe叩C 82xx 툴 체인을 위해서 구성된 것이다. 다시 한 번 말하지만 다음 내용
         도 가독성을 위해서 공백을 일부 삽입했다．

        ［리스트 ]2-3) 교차小개발 툴의 기본 검색 위치


           $ ppc_82xx-cpp -v
           Reading specs from /opt/eldk/usr/bin/ . .
            니 /lib/ gcc-lib/ ppc-linux/3. 3. 3/ specs

           Configured with: . ./configure --prefix=/usr
           니 --mandi r=/usr/ share/man --infodi r=/usr/share/info
           니 ---enable- shared --enable- threads=posi x --disable-checking
           니 1巾Wi태巧ystem-z］化 小enabi e-_cxa_毗exit --with-new］化
           니 --enable-languages=c, c++ --disable-libgcj
           니 --host=1386- redhat-linux -target=ppc-linux

           Thread model: posix

           gcc version 3. 3. 3 (DENX ELDK 3.1.1 3. 3. 3-10)
            /opt/eldk/usr/bin/ . ./lib/ gcc-lib/ ppc-linux/ 3. 3. 3/ccl
            니 -E -quiet -v -iprefix /opt/eldk/usr/bin/ . .
            니 기化／gcc-lib/ ppc-linux/3. 3. 3/ 七_un似14 山1帥u_li nux_
            니 -D_linux_ -Dunix -D_unix -Dlinux -D_linux -Asystem=unix
            니 -Asystem=posix - -mcpu=603


I 368
                                                              임베디드 개발 환경   Chapter 12



     ignoring nonexistent directory "/ opt/eldk/usr/ppc-linux/ sys-include "
     ignoring nonexistent directory "/ opt/eldk/usr/ppc-linux/include"
     #include ' 1 . . . 1' search starts here:

     #include <. . .> search starts here:
       /opt/el dk/usr/l i b/gcc-l i b/ppc-l i nux/ 3 .3. 3/include
       /opt/el dk/ppc_82xx/usr/ i nd] ude

     End of search list.




   위 리스트에서는 포함（Inc끄迫e）을 위한 기본 검색 경로가 호스트를 위한 include 디렉터
   리 대신에 교차 시스템을 위한 디렉터리로 바뀐 것을 볼 수 있다. 이런 모호한 점 때문에 자
   신의 임베디드 시스템을 위한 어플리케이션이나 오픈 소스 패키지를 빌드하는 것이 매우 어
   렵게 느껴친다. 이 기본 값 관련 부분은 임베디드 시스템에 대한 경험이 없으면 숙련된 어플
   리케이션 개발자라도 아주 어려워하는 부분 중에 하나이다．



12.2 호스트 시스템 요구 사항
   사용하는 개발 워크스테이션에 꼭 있어야 하는 중요한 구성 요소가 몇 가지 있다. 물론 알맞
   게 구성된 교차 툴 체인은 기본적으로 있어야 한다. 직접 다운로드해서 컴파일해서 사용하거
   나, 또는 판매중인 많은 툴 체인 중에서 하나를 구입할 수도 있다. 직접 다운로드해서 빌드하
   는 부분은 이 책에서는 설명하지 않을 것이다. 하지만 12.4.1절의 "더 읽어 보기"에 참고할
   많은 좋은 자료가 있으니 관심 있는 독자는 한번 살펴보기 바란다．

   다음으로 필요한 중요 항목으로 독자가 사용하는 임베디드 시스템 아키텍처를 위한 리눅스
   배포 버전이 있어야 한다. 여기에는 독자의 임베디드 시스템의 파일 시스템에서 사용할 수
   있는 수백 개에서 수천 개의 파일도 포함된다. 여기서도 선택은 자신이 직접 빌드하거나 상
   업적으로 구입하는 경우가 있을 수 있다. 인터넷에서 구할 수 있는 가장 있기 있는 임베디드
   시스템 배포 버전으로는 이전에 언급한 ELDK가 있다. 일부 종류의 PowerPC나 기타 임베
   디드 시스템을 위한 ELDK가 나와 있다. 임베디드 리눅스 배포판을 처음부터 직접 만드는
   방법은 이 책의 분량만큼의 책이 따로 필요하기 때문에 여기서는 논외로 한다．
 礬U       Embedded Linux Primer




        요약하면 독자의 개발 호스트는 다음 네 가지의 독립된 기능을 가지고 있어야 한다．

         口 교차 툴 체인과 라이브러리
         口 프로그램, 유틸리티 , 라이브러리 등을 포함한 타깃 시스템 패키지

         口 에디터나 디버거 , 기타 유틸리티 등의 호스트 툴
         口 타깃 보드를 위한 서버（다음 절에서 설명）

        상업 제품이든 오픈 소스 커뮤니티에서 무료로 받은 것이든, 이미 만들어진 임베디드 리눅스
        개발 환경을 자신의 워크스테이션에 설치하는 경우에는 툴 체인과 관련 구성 요소가 서로 같
        이 동작하도록 이미 구성되어 있다. 예를 들면 툴 체인에서 사용하는 기본 검색 위치들이 모
        두 타깃을 위한 헤더 파일과 시스템 라이브러리가 있는 위치로 설정되어 있다. 이런 상황은
        자신의 개발 워크스테이션에서 하나 이상의 아키텍처와 프로세서를 지원해야 할 때는 좀 더
        복잡해진다. 이 때문에 임베디드 리눅스 배포 버전이 존재하는 것이다．


12.2. ] 하드웨01 디버깅 장비

        이전에 나열된 항목과는 별도로 하드웨어를 이용한 디버깅도 생각하1 볼 수 있다. 이는 하드
        웨어 장비의 한쪽은 호스트와 （주로 이더넷을 통해서） 연결되고 타깃 시스템으로는 디버그
        커넥터를 통해서 보드에 연결된다. 현채 시장에서는 많은 장비들이 판매되고 있는데 , 관련된
        내용은 14장, "커널 디버깅 기술'에서 자세히 알아보도록 하자．



12.3 타깃 보드 호스팅하71
        ［그림 12-1］을 다시 보면 호스트 개발 시스템에서 타깃 임베디드 보드로 이더넷을 통해서
        연결되어 있는 것을 알 수 있다. 이런 연결은 반드시 필요한 것은 아니고, 사실 많은 수의
        경량 임베디드 장치들이 이더넷 인터페이스를 가지고 있지 않다. 오히려 이렇게 이더넷을 갖
        춘 경우가 예외적인 경우라고 볼 수 있다. 하지만 실리콘에는 없더라도 보드 상에서 외부 IC
        를 통해서라도 이더넷을 사용할 수 있게 하는 방법도 생각하1 볼 수 있다．

        커널을 개발할 때는 커널을 컴파일해서 임베디드 보드에 다운로드하는 일을 반복하게 된다．
        많은 임베디드 시스템과 부트로더들이 TFTP를 지원하고, 또한 개발자가 TFTP를 사용할



I 370
                                                       임베디드 개발 환경        Chapter 12




    것이라고 가정하고 있다. TFTP는 FTP와 비슷하게 TFTP 서버와 TFTP 클라이언트 간에
    파일을 전송할 수 있는 경량 프로토콜이다．

    부트로더에서 TFTP를 이용해서 커널을 로드하면 시리얼 포트를 아무리 빠르게 설정하더라
    도 그것과 비교가 안 될 정도의 빠른 속도로 로드시킬 수 있다. 더군다나 램디스크를 로드하
    는 시간은 더 차이가 많이 나는데 , 램디스크 이미지는 필요에 따라서 수십 MB 이상이 될
    수도 있기 때문이다. 그렇기 때문에 시간을 들여서 TFTP를 사용할 수 있도록 설정하고 구성
    해 놓으면 훨씬 더 많은 이득을 얻을 수 있을 것이다. 개발 보드에 이더넷 포트를 추가하는
    것이 디자인 관점에서 볼 때 그리 큰 부담은 되지 않을 것이다. 그리고 개발 중에 사용하다가
    도 완료 후에 실제 제품에서는 뺄 수도 있다.


12.3.1 TFTP 서버
    현재 사용하고 있는 리눅스 개발 호스트 시스템에서 TFTP를 구성하는 것은 어렵지 않다．
    물론 세부 사항은 리눅스 배포 버전에 따라서 다를 수 있다. 여기서는 레드햇과 페도라 코어
    리눅스 배포 버전을 기준으로 설명하겠다．

     TFTP는 개발 시스템에서 활성화시켜야 하는 TCP/II) 기반 서비스인데 , TFTP 서비스를
     활성화시키기 위해서는 현재 사용하는 리눅스 서버에서 TFTP 패킷이 들어오면 응답하고 그
     에 따라 TFTP 서버를 시작시키도록 해야 한다. 이 작업은 대부분의 리눅스 배포 버전에서
     xine七d 인터넷 슈퍼서버가 사용하는 구성 파일을 수정하면 된다. 예를 들어 , 레드햇과 페도
    라 테스크탑 리눅스에서는 /etc/xinetd. d/tf七I) 파일을 수정하면 된다. ［리스트 12-4]
    는 페도라 코어 2 개발 워크스테이션에서 TFTP 서비스를 활성화시키기 위한 구성 파일의
    내용을 나타낸 것이다. 내용은 페이지에 맞게 일부 재정렬되었다.

    ［리스트 ]2小4] TFTP 설정

       # default: off
       # description: The tftp server serves files using the trivial
       # file transfer protocol. The tftp protocol is often used to
       # boot diskless workstations, download configuration files to
       # network-aware printers, and to start the installation process
       # for some operating systems.

       service tftp



                                                                               371 1
         Embedded Linux Primer




          {
                  socket_type    = dgrani
                  아otoco]        = ud口
                  wait           = yes
                  user           = root
                  server         = /usr/ sbin/in. tfrpd
                  server_args    = -c -s /tftpboot
                  chsable        = no
                  per_source     = 11
                  댜）5            = 100 2
                  flags          = IPv4
          }



        위 환경에서는 TF1P 서비스를 활성화시켰고（disable = n이 워크스테이션의 ／七f七pboo七
        디렉터리에 있는 파일을 전송할 수 있도록 설정되어 있다. xine七d 인터넷 슈퍼서버에서
        TFTP 요청을 받으면 이 구성 파일의 내용을 보고 이 파일에 지정된 서버（/usr/ sbin/
        in．七ffpd）를 실행시킨다. 또한 server args어］ 명시된 내용을 in．七f댜）d 프로세스에
        인자로 전달한다. 이 경우에는 -s 스위치를 통해서 in. 七f七pd 프로세스가 지정한 위치
        (/ tftpboot）로 현재 디렉터리를 이동할 것을 지시하고, 尸C 플래그는 새로운 파일을 만들
        수 있도록 설정한다. 이는 타깃에서도 서버로 파일을 기록할 수 있으면 유용하기 때문이다．

        자신이 사용하고 있는 배포 버전에 따른 세부 사항은 배포 버전에 포함된 문서를 참고하기
        바란다．


12.3.2 BOOTP/DHCP 서버
        개발 호스트 시스템에 DHCP 서버를 가지고 있으면 임베디드 타깃을 설정하는 일을 좀 더
        간편하게 할 수 있다. 타깃 하드웨어에 이더넷 인터페이스를 사용할 수 있도록 하면 어떤 점
        들이 좋은지를 잘 알고 있을 것이다. 이더넷 인터페이스로 리눅스를 타깃 보드에서 부팅시키
        려면 먼저 이더넷 인터페이스를 알맞게 설정해야 한다. 더군다나 NFS 루트 파일 시스템을
        마운트해서 사용하는 경우에는 리눅스 부팅 과정을 완료하기 전에 타깃의 이더넷 인터페이스
        가 먼저 올바로 설정되어 있어야 한다. NFS에 대해서는 9장, "파일 시스템"에서 살펴보았다．




I 372
                                                       임베디드 개발 환경     Chapter 12




일반적으로 리눅스에서 이더넷／II) 인터페이스를 부팅 중혀］ 초기화하는 방법은 두 가지가 있다．

  口 기본 구성 옵션 또는 리눅스 커널 커맨드 라인에 필요한 정보를 직접 입력해1 넣는 방법

  口 커널에서 부팅 시어］ 자동으로 네트워크 설정을 감지하도록 하는 방법

여기서 두 번째 방법이 더 유연한 방법이다. DHCP와 BOOTP는 타깃 시스템과 서버가 네
트워크 설정을 자동으로 감치할 수 있도록 해 주는 프로토콜이다. 이 프로토콜에 대한 자세
한 참고 자료는 이 장의 마지막에 있는 12.4.1절을 보기 바란다．

DHCP 서버는 II) 서브넷（subnet) 내에 연결하려고 하는 DHCP 또는 BOOTP 클라이언
트에게 II) 주소를 할당하1 주는 일을 한다. 부팅 과정의 일부로서 DHCP 서버는 （타깃 보드
와 같은） DHCP 클라이언트의 요청을 기다렸다가, 클라이언트에게 II) 주소와 적절한 정보
를 할당해 준다. 천형적으로 DHCP를 통해서 주고받는 정보는（［리스트 12-前를 보자）
DHCP 서버를 나j 디버그 스위치를 주고 실행시킨 뒤에 타깃 시스템이 정보를 요청하는 시
점에 서버에서 출력하는 내용을 보면 알 수 있다．

［리스트 12-5] 전형적인 DHCP 정보 교환


  tgt> DHCPDISCOVER from 00:09: 5b: 65:ld: d5 via ethO
  svr> DHCPOFFER on 192.168. 0. 9 to 00: 09: 5b: 65:ld: d5 via ethO
  tgt> DHCPREQUEST for 192.168.0. 9 (192.168.0.1) from \
           OO: 09: 5b: 65:ld: d5 via ethO
  svr> DHCPACK on 192.168.0. 9 to 00: 09: 5b: 65:ld: d5 via ethO




정보를 주고받는 절차는 먼저 클라이언트（타깃）가 DHCP 서버를 찾기 위한 브로드캐스트
메시지를 보내는 것으로 시작한다. 이는 DHCPDISCOVER라는 메시지를 통해서 알 수 있다．
그러면 서버는 （해당 클라이언트를 사용할 수 있도록 설정해 놓은 경우） 클라이언트를 위한
II) 주소를 알려주는 응답을 보내게 된다. 이 메시지가 바로 DHCPOFFER이다. 그런 후에 클
라이언트는 전달받은 IF) 주소를 내부적으로 테스트해 본 후에 응답하게 된다. 이 테스트 과
정에는 위에서 보는 것처럼 DHCPP므QUEST 패킷을 DHCP 서버에 보괘는 일도 포함된다. 마
지막으로, 서버가 클라이언트에게 'P 주소 할당을 성공적으로 마쳤다는 응답 메시지를 보내
는 것으로 타깃 II) 주소 설정 과정을 마치게 된다．




                                                                           373 I
          Embedded Linux Primer




        재미있는 부분은 잘 만들어진 클라이언트 시스템은 마지막으로 성공적으로 통신한 DHCP
        서버의 주소를 기억할 것이라는 점이다. 그래서 다음번 부팅 시에는 이전에 찾은 서버를 다
        시 이용할 수 있다고 가정하고 DHCPDISCOVER 단계를 생략하고 바로 DHCPREQUEST 단계
        를 진행하게 된다. 하지만 리눅스 커널은 그런 기능을 갖고 있지 않아서 매 부팅 시마다 같은
        절차를 반복하도록 되어 있다．

        호스트에 있는 DHCP 서버를 구성하는 것은 어렵지 않다. 역시 이 부분도 독자가 사용하고
        있는 리눅스 배포 버전에 포함되어 있는 문서를 참고하는 것을 추천한다. 레드햇이나 페도라
        코어의 경우, 타깃 보드 하나에 대한 구성 항목은 다음 ［리스트 12-6］과 같은 형태가 될 것
        이다．

        ［리스트 ]2-6) DHCP 서버 구성 예제


          # Example DHCP Server configuration
          allow bootp;

          subnet 192. 168. 1. 0 netmask 255 . 255 . 255 .0 {
           default-lease- time 1209600;        # two weeks
            option routers 192. 168. 1. 1;
            option domain- name- servers 1. 2. 3. 4;
               아oup {
                host pdnal {
                  hardware ethernet 00: 30: bd: 2a: 26: lf;
                  fixed-address 192.168.1. 68;
                  filename "ulmage- pdna";
                  option root-path "/ honie/chris/ sandbox/pdna- target ' ;
                   }
               }
           }


        위 예제는 타깃 시스템에 전달할 정보의 종류만 보여 주는 간단한 예제이다. 여기에는 타깃
        MAC 주소에 대해서 일대일 대응이 되는 H) 주소를 가지고 있다. 고정된 II) 주소 외에도
        타깃 보드에 다른 정보를 전달할 수 있는데 , 이 예제에서는 기본 라우터와 DNS 서버 주소가
        타깃에 전달된다. 그리고 기본 라우터 주소와 DNS 주소 외에도 NFS로 루트 파일 시스템을
        마운트시키기 위한 위치 정보와 커널 이미지 파일 이름이 천달된다. 이 커널 이미지 파일 이
        름은 부트로더에 의해서 사용되는데 , TFTP 서버에서 어떤 커널 이미지를 가져올 지를 결정


I 374
                                                 임베디드 개발 환경   Chapter 12



    하게 된다. 그리고 정해진 범위 안에 있는 II) 주소 중에서 선택해서 II) 주소를 할당하1 주도
    록 DHCP 서버를 설정할 수도 있지만, ［리스트 12-6］에서 보는 것처럼 고정된 주소를 할당
    하는 것이 더 편리하다．

    그리고 리눅스 개발 워크스테이션에서 DHCP 서버를 활성화시켜 둬야 하는데 , 이는 메인
    메뉴나 커맨드 라인으로 할 수 있다. 자신이 사용하고 있는 환경에 맞는 도움말 문서를 참고
    해서 DHCP 서버를 시작시키기 바란다. 예를 들어 , 페도라 코어 2 리눅스 배포 버전에서는
    다음과 같은 간단한 명령어를 이용해서 DHCP 서버를 시작시킬 수 있다．

       $ /etc/init. d/dhcpd start (또는 restart)

    DHCP 서버를 부팅 시에 항상 자동으로 시작하도록 설정하치 않으면 위 명령어를 매번 입력
    해서 DHCP 서버를 실행시켜야 한다．

    독자가 사용하는 리눅스 시스템이 사설망（private network）에 연결되어 있지 않는한
    DHCP 서버를 설치하는 것은 샹궁히 신경 써야 할 일이 많다. 그래서 직접 진행하기 전에
    먼저 시스템 관리자에게 문의해 보는 것이 좋을 것이다. 만약에 공동으로 사용하는 일반 네
    트워크에 연결되어 있다면 기존에 존재하는 DHCP 서비스와 충돌할 가능성이 매우 높다．


12.3.3 NFS 서버
    루트 파일 시스템을 NFS를 이용해서 마운트하는 것은 아주 강력한 개발 도구이다. 이 방법
    이 갖는 장점은 다음과 같은 것들이 있다．

      口 플래시 용량과 같이 보드에서 쓸 수 있는 자원의 양과는 상관없이 크기 제한 없는 루트
         파일 시스템을 사용할 수 있다．
      口 개발 시스템용 어플리케이션이 변경되었을 때1 타깃 시스템에서도 즉시 변경된 어플리케
         이션을 사용할 수 있다．
      口 루트 파일 시스템을 만들고 디버깅하기 전에 먼저 리눅스 커널 자체를 부팅하고 디버깅
        하는 뎨 투자할 수 있다．




                                                                   375I
                Embedded Linux Primer



        NFS 서버를 설정하는 방법은 사용하는 리눅스 배포 버전에 따라서 다양하다. 이 장에서 설
        명한 다른 서비스들과 마찬가지로 현재 자신이 사용하고 있는 리눅스 배포 버전에 포함된 서
        비스 구성 관련 문서를 참고하기 바란다. NFS 서비스는 시작 스크립트를 통해서나, 그래픽
        메뉴 또는 커맨드 라인을 통해서도 실행시킬 수 있다. 예를 들어 , 페도라 코어 2 리눅스에서
        는 다음 명령어를 통해서 NFS 서비스를 시작시킬 수 있다．

                  $ /etc/init. d/nfs start (or restart)


        매번 리눅스 데스크탑 워크스테이션을 시작할 때마다 이 명령을 실행해야 한다（이 서비스와
        기타 서비스를 부팅 시에 자동으로 시작하게 만들 수도 있다. 자신이 사용하는 리눅스 배포
        판에 포함된 문서를 참고하자）. 서비스를 활성화하는 것과 함께 커널도 NFS를 지원하도록
        컴파일되어 있어야 한다. DHCP와 TFTP는 모두 사용자 영역에서 동작하는 유틸리티인 반
        면에 NFS는 커널 레벨에서 사용할 수 있도록 되어 있어야 한다. 이는 타깃 보드와 개발 워
        크스테이션 모두에 해당하는 말이다. ［그림 12-g를 보면 커널에서 NFS를 사용하도록 설
        정하는 구성 옵션을 보여 주고 있는데 , NFS를 이용해서 루트 파일 시스템을 이용하는 옵션
        도 있는 것을 알 수 있다. 커널에서 NFS를 통해서 루트 파일 시스템을 마운트하려면 이 옵
        션이 반드시 선택되어 있어야 한다.

        日］e             Qj於油ris        beIp

                 匈 ［그 C쿄                       1     H E         四       簪
                已；C '    山ad Save Si畔e S口lit Fiii C（내a口5e Ex口and

        區而而                                                 呻            「          啣叫
                                                                                                 m如艸       1    j스
                 口 Network Fr沁 Systems
                    口 琶NFS州e sys挺m sup附t
        i                卜 團Pro눠血NFS咐테帥t supp아t
        홑                   口Provide
                                              NFSv4 client supp（가t (EXPERIM타寸TAL)
                            口川애面的甘O on NFrS flies (EXPERIME町A나                                                  山

                        ' 心 ('IFS se八心 su바）이-t                                                                  -

            三               口餉너血NFSv3 server SUF巾art (NE冽）
            !               回Prc｝너de NFS s到四毗rTCP sup的rt (晦N)
            三             回Ro여file sys把man NFS                                                                      두

                                                                             ]               如         m       ［三
                                                                                                                嶝
                                                                                         1
                                                小1




            ! NF' 此rv.r sup叩" NFSD
        I 그림 ]2-2 NFS 커널 구성


        NFS 서버는 현재 서버에 있는 expor七S 파일에서 필요한 정보를 가져오는데 , 이 파일은
        보통 /e七c/ exports어］ 있다. ［리스트 12尸7］은 외부로 노출시킬 항목을 몇 7긔 가지고 있는
            expor七S파일을 예제로 나타낸 것이다．

聲 376
                                                             임베디드 개발 환경     Chapter 12



      ［리스트 ]2-7] 간단한 NFS exports 파일

         $ cat /etc/ exports
         # /etc/exports
         /home/ch ri s/sandbox/coyote-target * (rw, sync, no_root_squash)
         /home/chris/sandbox/pdna-target 央(rw, sync, no_root_squash)
         갸ome/chr朽加아匕pace 玄（r叫，sync,no_root_squash)



      클라이언트는 개발 워크스테이션에서 위 항목에 있는 세 개의 디렉터리 중 아무 곳이나 원격
      으로 접근할 수 있다. 그리고 디렉터리 항목 바로 다음에 오는 속성들은 각각 어떤 'p 주소든
      연결을 허용한다는 의미(*）를 나타내는 부분과 각 디렉터리를 어떻게 마운트시킬지
      (read/write와 no roo七 squash4)）를 정의하고 있다. 맨 마지막의 no root squash
      속성은 클라이언트가 해당 디렉터리에 대해서 루트 권한을 행사할 수 있게 해 주는데 , 이는 사
      용하는 임베디드 시스템에서 보통 루트 계정 하나만을 가진 경우가 흔하기 때문에 필요하다.

      NFS를 구성한 내용을 바로 워크스테이션에서 테스트해 볼 수 있다. 먼저 NFS 서비스를
      활성화시켰다고 가정하면（NFS 서버와 클라이언트 모두 활성화시켜야 한다） 다른 파일 시스
      템을 마운트하듯이 NFS로 노출시킨 디렉터리를 마운트할 수 있다．

         # mount -t nfs loca가ost: /home/ chris/workspace /mnt/ remote


      이 명령이 성공적으로 실행되면 . . . /workspace에 있는 파일들을 /mnt/ remo七e에서도
      사용할 수 있다．


12.3.4 타깃 시스템에 NFS 루트 파일 시스템 마운트하기
      NFS를 이용해서 루트 파일 시스템을 마운트하는 것은 어렵지 않다. 그리고 다른 곳에서도
      언급했듯이 아주 유용한 개발 환경으로 사용할 수 있다. 하지만, 동작시키기 전에 먼저 세부
      적인 설정이 올바르게 되어 있어야 하는데 , 이 과정은 다음과 같이 정리해 볼 수 있다．

         1. NFS 서버를 구성하고, 아키텍처어］ 맞는 알맞은 타깃 파일 시스템을 외부에 노출시킨다．

         2. 타깃 커널에서 NFS 클라이언트 서비스와 NFS 루트 파일 시스템을 사용할 수 있도록
           구성한다．


4) （역자주） 이 속성은 클라이언트가 NFS로 파일 시스템에 접근할 때 root 사용자 권한으로 동작시키게 해 준다．


                                                                                  377 I
                       Embedded Linux Primer




                        3. 타깃 커널에서 이더넷 인터페이스를 자동으로 구성할 수 있도록 한다．

                        4. 커널 커맨드 라인이나, 정적인 커널 구성 옵션을 줌으로써 타깃 이더넷 II) 주소를 결정
                              하는 방법을 제공한다．

                        5. NFS를 사용하는 커널 커맨드 라인을 커널에 넘긴다．


       NFS 서버 구성에 대해서 설명할 때 ［그림 12-2］를 통해서 커널 구성 옵션을 살펴보았다．
       먼저 타깃 커널 구성이 NFS 클라이언트 서비스를 사용하도록 되어 있어야 한다. 그리고 특
       히 NFS를 이용해서 루트 파일 시스템을 사용하는 옵션도 활성화시키도록 한다. 좀 더 구체
       적으로 말하자면 커널이（兀NFIGNFSFS=y와 CONFIG ROOT 胛S=y 옵션을 갖도록 해야
       한다는 의미이다. 그리고 NFS 루트 파일 시스템을 마운트할 경우에는 NFS를 적재 가능
       모듈로 설정할 수 없다．

       커널 레벨의 자동 구성（autoconfiguration) 옵션은 커널 구성 유틸리티의 네트워킹 메뉴
       항목 아래의 TCP/II) 구성 옵션（TCP/IP configuration) 부분에서 찾아볼 수 있다. 타깃
       커널에 CONFIGIPPNP를 활성화시키도록 하자. 이 옵션을 선택하면 몇 가지 세부 옵션이
       더 생기는데 , 앞에서 설명한 것처럼 BOOTP 또는 DHCP 중에서 하나를 선택하도록 하자．
       ［그림 12-3］에서 이 커널 레벨 자동 구성 부분을 볼 수 있다.

           日e                Q1比ons   ileip

                      勺 ［그 툐丑 1                   n 는         四    中
                     r‘그Ct    Load San숀 Sin며e S口Fit Full Collapse Eu口and
                                                                           IN曲.
           Options                                                                                    1匡
                      口 包Netw油四supp아t                                             NET
                         口 Networking opftl가巧
                              b 回Pa比etsocket                                      PACKET
                                回 Unix （幻main sockets                             UN以
                                口1가乙KEY sockets                                   NETJ(EV
                              口 囹TCP／甲r比tw岫따｝                                     INET
       ;                          口FP: mu消cas甘ng                                  IPJi4ULTlCAST
                                  DIP: advanced router                            中ADVANCED_ 킵）UIER
                                , 口 !P. k們nell아！
                                               키 amm이作乂北｝ration                   냐그 PNP                   4
                                      巨IP: DI-tCP sup的C                           IP_PNPJ）比P
                                      [ IIP: 田겨)TP support                        It之PNP_BOOTP
                                      口FR RARP support                            It乙PN艮RA먀1                   V



                             ertiel kvet aUbconfigura*Ion IP巾PNP                                      日
       I 그림 12-3 커널 레벨 자동 구성




1378
                                                         임베디드 개발 환경        Chapter 12




    서버와 타깃 커널을 구성한 후에는 앞에서 설정한 방법 중에서 한 가지를 이용해서 타깃 이더
    넷을 설정해야 한다. 부트로더가 커널 커맨드 라인을 지원하는 경우가 가장 쉽다. 다음은
    NFS 루트 마운트를 지원하도록 커널 커맨드 라인을 지정한 것이다．



      console=ttySO,115200 root=/dev/nfs rw ip=dhcp \
        nfsroot=192 .168.1. 9: /home/ch ri s/sandbox/pdna-target




12.3.5 나Boot릍 이용한 NFS 루트 파일 시스템 마운트 예제
    U-Boot는 커널 커맨드 라인을 설정할 수 있는 부트로더의 좋은 예이다. U-Boot의 비휘발
    성 메모리에 환경을 저장할 수 있는 기능을 이용해서 , 커널 커맨드 라인을 위한 특별한 이름
    을 갖는 파라미터로 저장시켜 둘 수 있다. U-Boot에서 NFS를 사용하기 위한 커맨드 라인
    을 설정하려면 다음과 같이 하면 된다（모든 내용을 시리얼 터미널 상에 한 줄로 입력한다）.



      setenv bootargs console=ttySO, 115200 root=/dev/nfs rw \
         ip=dhcp nfsroot=192.168.1.9: /honie/chris/ sandbox/pdna- target



    이렇게 한 후 커널을 TFTP 서버를 통해서 로드한다. ［리스트 12-8］은 PowerPC 타깃 시
    스템에서 실행한 모습을 보여 주고 있다．

    ［리스트 ]2-8) TFTP 서버를 통해서 커널 로드하기


      => tftpboot 200000 ulmage-pdna          <<< U-Boot 프롬프트에X/ 압력
      Using FEC ETHERNET device
      TFTP from server 192.168.1. 9; our IP address is 192.168.1. 68
      Filename 'uImage-pdna ' .
      Load address: 0x200000
      Loadi ng:  ##################################################
                 ##################################################
                 #########################################
      done
      Bytes transferred = 911984 (dea70 hex)
      =>
                                                                                379
        Embedded Linux Primer




      커널을 부팅하고 나면 NFS로 루트 파일 시스템을 마운트하는 증거를 확실히 볼 수 있다．
      ［리스트 12-9］는 이 부분을 보여 주는 커널 부트 메시지의 일부를 나타낸 것이다. 이 출력
      내용은 가독성을 위해서 약간 형식을 변경한 것임을 알아두자（많은 부분이 생략되었다）.

      ［리스트 12-9) NFS로 마운트하는 부팅 과정


        Uncompressing Kernel Image . . . OK
        Linux version 2. 6. 14 (chris@pluto) (gcc version 3. 3. 3
         니 (DENX ELDK 3.1.1 3. 3. 3-10) ) #1 Mon Jan 2 11: 58: 48 EST 2006



         Kernel command line: console=ttyS0,115200 root=/dev/nfs rw
          니 nfsroot=192.168.1. 9: /home/chris/ sandbox/pdna- target ip=dhcp



         sending DHCP requests . . . OK
         IP-Config: Got DHCP answer from 192.168.1. 9, my address is 192.168.1. 68
         IP-Config: Complete:
              device=eth0, addr=192.168.1.68, mask=255. 255. 255. 0,
              gw=255. 255. 255. 255, host=192.168.1. 68, domain=,
              nis-domain=(none) , bootserver=192.168.1. 9,
                rootserver=192 .168.1. 9,
                rootpath=/home/chri s/ sandbox/pdna-target



         Looking up port of RPC 100003/ 2 on 192.168.1. 9
         Looking up port of RPC 100005/1 on 192.168.1. 9
         yES: Mounted root (nfs filesystem) .




         BusyBox v0. 60. 5 (2005. 06. 07-07: 03+0000) Built-in shell (msh)
         Enter 'help ' for a list of built- in commands.

          #




      ［리스트 12-9］를 보면 맨 치음에 커널 커맨드 라인 바로 디음에 오는 커널 배너를 볼 수 있
      다. 커널 커맨드 라인에서는 다음의 네 가지 항목을 명시하고 있다．


380
                                                       임베디드 개발 환경          Chapter 12



    口 콘솔 디바이스（/dev/console)

    口 루트 디바이스（/dev/nfs)

    口 NFS 루트 경로（h帥e/chris/ sandbox/pdna尸七arget)

    口 커널 레벨의 II) 자동 구성 방법（dhcp)


   그 후에 커널이 DHCP를 이용해서 자동 구성을 하려고 시도하는 것을 볼 수 있다. 서버가
   응답해서 DHCP로 청보 교환이 완료되면 구성된 사항에 대한 정보가 다음 줄에 출력된다．
   위 리스트를 보면 DHCP 서버가 타깃에게 192.168.1.68이라는 IF) 주소를 할당한 것을 볼
   수 있는데 , ［리스트 12-6］에서 설정한 내용과 비교해 보면 ［리스트 12-6］에서 DHCP 서버
   에 설정한 것에 따라서 구성된 것을 확인할 수 있다．

   커널이 II) 자동 구성을 완료하고 나면 제공받은 파라미터를 이용해서 루트 파일 시스템을
   마완i시킬 수 있다. 이 내용은 NFS로 루트 파일 시스템을 마운트했다고 알려주는 VFS（가
   상 파일 시스템） 메시지까치의 세 줄에서 볼 수 있다. NFS 루트 파일 시스템이 마운트되면
   5장, "커널 초기화'에서 설명한 것처럼 커널 초기화가 완료된 것이다．

   또한 타깃의 'p 주소 설정을 DHCP 또는 BOOTP 서버를 통해서 동적으로 커널이 얻어오게
   하는 방법 대신에 , 정적인 방법으로 커널에 전달할 수도 있다. 'I> 주소 설정을 커널 커맨드
   라인을 통해서 직접 설정할 수도 있는데 , 이 경우에 커널 커맨드 라인은 다음과 같은 형태가
   된다．



     consol e=consol e=ttySO,115200 \
      니 ip=192.168.1. 68:192.168.1.9: :255. 255. 255. O:pdna: ethO:off \
      니 root=/dev/nfs rw nfsroot=192 .168. 1.9: /home/chris/pdna-target




]2.4 요약
     口 임베디드 교차개발 환경의 효율성을 높이기 위해서 여러 가지 방안을 적용해1 볼 수 있
         는데, 대부분의 경우 툴 또는 유틸리티를 활용하는 것이다. 이 툴 및 유틸리티에 대해서
         는 다음 장에서 개발 툴을 설명하면서 자세히 알아보자．


                                                                                 381 !
        Embedded Linux Primer



        口 임베디드 개발자에게 있어서 올바른 개발 환경을 갖는 것은 그 자체로 아주 중요한 자산
           이 된다．

        口 교차e개발을 위해서 사용되는 툴 체인은 자신이 사용하는 타깃 리눅스 환경과 맞도록
           알맞게 구성해써 사용해야 한다．

        口 개발 호스트 시스템에는 툴 체인 및 바이너리 유틸리티가 참조할 수 있도록 타깃 구성
           요소들이 설치되어 있어야 한다. 이 구성 요소어悟 타깃 시스템을 위한 혜더 파일, 라이
           브러리, 타깃용 바이너리 , 기타 구성 파일이 포함된다. 요약하면 임베디드 리눅스 배포
           버전을 구하거나 직접 준비해야 한다．

        口 타깃을 위해서 TFTP, DHCP 그리고 NFS와 같은 서버를 만들어 놓으면 임베디드 개발에
           있어서 효율성을 상당히 높일 수 있다. 이 장에서는 각각의 서버를 구성하는 방법을 예를
           들어서 설명했다.



12.4. ] 더 읽0] 보기
        GCC 온라인 문서
        http://gcc.gnu.org/onlinedocs/


        gcc/glibc 교차 툴 체인 빌드 및 테스트 방법
        http://kegel. com/crosstool/


        TFTP 프로토콜, 버전 2
        RFC 1350
        www.ietf. org/rfc/rfc1350. txt?number=1350


        부트스트랩 프로토콜, Bootstrap Pr毗oc아（BOOTP)
        RF（그 951
        www.ietf. org/rfc/rfc095l. txt?number=951


        DHCP(Dynamic Host Configuration Protocol)
        RFC 2131
        www. ietf. org/rfc/rfc2l3l. txt?number=2131




I 382
이번 장에서 배울 내용

  1
      GNU 디버거（GDB)

  I 데이터 표시 디버거

  . cbrowser/cscope
  1
      추적 및 프로파일링 도구
  1
      바이너리 유틸리티
  1
      기타 바이너리 유틸리티
  1
      요약
驀 二1     Embedded Linux Primer




       임베디드 리눅스 배포 버전에는 일반적으로 많은 유틸리티들이 같이 포함되어 있다. 그 중에
       는 사용법을 완전히 익히려면 상당한 시간이 필요할 만큼 복잡한 것들도 있다. 또한 간단하
       고 유용한 툴인테도 임베디드 개발자로부터 외면되어왔던 툴도 많이 있다. 그리고 일부 툴은
       각각의 개발 환경에 맞도록 조정해야 하는 것도 있다. 하지만 "바皇' 사용할 수 있는 것이 대
       부분이고, 개발자에게 큰 노력 없이도 유용한 기능을 제공한다. 이 장에서는 여러 섹션에 걸
       쳐서 임베디드 개발자가 활용할 수 있는 가장 중요한 툴（또한 종종 무시되곤 하는）을 알아보
       도록 하겠다．

       이 장에서 소개하는 툴 및 유틸리티에 대해서 세부적인 내용까지 모두 설명하기는 불가능하
       다. 그러기 위해서는 별도로 책 한 권이 필요할 것이다！ 대신에 참고로 삼을 정도로는 충분한
       내용을 설명하도록 하겠다. 이 장의 목표는 각각의 툴에 대한 기본 사용법을 소캐하는 것이
       다. 하지만 중요한 개발 툴에 대해서 시간을 투자해서 더 세밀하게 공부해 보는 것도 아주
       좋을 것이다. 툴에 대한 맨 페이지（또는 다른 문서들）부터 시작하는 것도 좋은 방법이다．

       GNU 디버거（GDB）를 먼저 알아보고, 그 다음에 그래픽 인터페이스를 갖는 데이터 표시 디
       버거（DDD : Data Dis히ay Debugger）에 대해서 간단히 알아보도록 하자. 다음으로 프로
       그램과 시스템이 어떻게 동작하는지를 살펴볼 수 있도록 해 주는 유틸리티에 대해서 살펴보
       겠다. 이 유틸리티에는 종종 초보자도 리눅스 개발자에게 외면당하곤 하는 S七race,
       itrace, t아）그리고 PS 등도 포함된다. 그리고 크래시 덤프（crash dump）와 메모리 분석
       툴도 소개하겠다. 마지막으로 추가적인 바이너리 관련 유틸리티를 소캐하는 것으로 마무리할
       것이다．



13.1 GNU 디버거（GDB)
       독자가 리눅스 어플리케이션을 개발하는 데 많은 시간을 보내는 입장이라면 틀림없이 GNU
       디버거의 사용법을 익혀야 한다. GDB는 당연히 개발자를 위한 여러 도구 중에서도 가장 중
       요한 툴이다. 오랜 역사를 갖고 있고, 많은 기능 확장을 통해서 이제는 다양한 아키텍처와
       마이크로프로세서를 위한 저수준의 하드웨어 종속적인 디버깅까지도 지원할 정도로 발전했
       다. 그리고 GDB를 위한 사용자 매뉴얼은 거의 책 한 권 분량은 될 만큼 방대하다. 여기서는
       GDB를 처음 사용하는 독자의 입장에서 GDB를 소캐하는 것을 목적으로 한다. 관심 있는
       독자는 13.7.1절 "더 읽어 보기"에 있는 사용자 매뉴얼을 더 공부해 보는 것을 추천한다．
                                                                   개발 도구     Chapter 13



       이 책은 임베디드 리눅스 개발에 관한 책이기 때문에 , 교차디버거로 컴파일된 GDB를 이용
       할 것이다. 이 말은 디버거 자체는 개발 호스트 시스템에서 실행되지만, 디버거는 컴파일 시
       점에 주어진 아키텍처를 위한 바이너리 실행 파일을 인식하도록 되어 있는 것을 의미한다．
       이어지는 몇 가지 예제를 통해서 레드햇 리눅스 계열의 개발 호스트 시스템에서 실행되지만
       엑스스케일（ARM) 타깃 프로세서를 위한 프로그램을 디버깅할 수 있는 GDB를 이용해 볼
       것이다. 비록 짧은 gdb라는 이름을 사용하치만, 실제로는 ARM 엑스스케일을 위해 만들어
       진 몬타 비스타（Monta Vista) 임베디드 리눅스 배포 버천에 포함되어 있는 엑스스케일 교
       차gdb를 이용하는 것임을 알아두자. 실제 바이너리 실행 파일의 이름은 xscale be-gdb
       이다. 하지만 이것도 역시 GDB이고, 교차e개발 환경을 위해서 설정해서 빌드시킨 것이다．

       GDB 디버거는 빌드 과정에서 많은 구성 옵션을 필요로 하는 복잡한 프로그램이다. 다른 책
       들을 참고하면 되기 때문에 , gdb를 빌드시키는 방법을 여기서 설명하지는 않을 것이다. 이
       장의 내용을 설명하기 위해서 , 독자가 사용하는 아키텍처와 호스트 개발 환경에서 동작하는
       GDB를 가지고 있다고 가정하도록 하겠다．


13.1. ] 코어 덤프 디버그하키
       GDB를 사용하게 되는 가장 흔한 경우 중의 하나는 코어 덤프를 분석하기 위해서이다. GDB
       는 빠르고 쉬우며 , 문제가 되는 코드를 찾아낼 수 있도록 도와준다. 코어 덤프는 어플리케이
       션이 존재하지 않는 메모리 영역을 접근하는 등의 시스템 오류를 발생시킬 경우에 만들어진
       다. 여러 가지 원인1)으로 코어 덤프가 만들어질 수 있지만, SIGSEGV（세그먼테이션 오류）
       시그널 때문인 경우가 가장 흔하다. SI(拾EGV는 사용자 영역의 프로세스가 비정상적으로 메
       모리에 접근했을 때 발생하는데 , 커널에서 덤프하는 기능을 켜 놓으면 이 시그널이 발생할
       때 코어 이미지를 파일로 덤프하게 된다．

       코어 덤프 기능을 활성화시키려면 코어 덤프를 할 용량 한계를 프로세스에 미리 정의해 놓아
       야 한다. 이는 setrlimi七 () 함수를 호출해서 프로세스의 자원 한계를 설정함으로써 할 수
       도 있고, BASH나 BusyBox 쉘에서 ulimit 명령어를 입력해서 할 수도 있다. 임베디드
       시스템의 초기화 스크립트에서 프로세서 에러 시에 코어 덤프를 활성화시키는 다음 명령어를
       흔하게 볼 수 있다．

           $ ulimit   -c unlimited


1) . . . /kernel/ signal. c에 있는 SI(；玉ERNEL_COREDUMP_MASK를 보면 코어 덤프를 만드는 시그널들을 볼 수 있다．
 繫藿1    Embedded Linux Primer




      BASH에 내장된 이 명령어는 코어 덤프의 용량 한계를 결정하는 데 사용되는데 , 여기서는
      용량 한계를 무한대로 설정한 것이다．

      어플리케이션 프로그램에서 세그먼테이션 폴트（예를 들어 , 허용된 범위 바깥의 메모리 주소
      에 데이터를 쓰는 경우）가 발생하면 리눅스는 이 프로세스를 중지시키고 코어 덤프를 생성하
      기 시작한다. 코어 덤프는 실행중인 프로세스에서 세그먼테이션 폴트가 발생한 시점의 메모
      리 스냅 샷을 말한다．

      바이너리 실행 파일에 대해서 디버깅 심볼을 사용할 수 있게 해 놓으면 도움이 되는데 , 빌드
      시에 만들어 놓은（gcc -g) 디버깅 심볼이 있는 경우 GDB가 훨씬 더 유용한 정보를 출력하
      기 때문이다. 하지만, 바이너리를 위한 디버깅 심볼이 없는 경우에도 세그먼테이션 폴트를
      일으킨 시점을 찾아내는 것은 가능하다. 물론 디버깅 심볼의 도움을 못 받는 경우에는 좀 더
      노력이 필요하기는 하다. 프로그램의 가상 메모리 위치를 직접 계산해 내야 하기 때문이다．

      ［리스트 13-1)은（訌）B를 이용해서 코어 덤프를 분석한 결과를 보여 준다. 출력 내용은 페이
      지 크기에 맞게 조금 재구성한 것이다. 이 예제에서는 의도적으로 세그먼트 폴트를 만들어
      내는 데모 프로그램을 이용했다. 다음 내용은 佃ebs라는） 이 프로세스에서 세그먼테이션 폴
      트가 발생했을 때 출력되는 내용이다．



        root@coyote : /workspace/websdemo# ./webs
           segmentation fault (core dumped)



      ［리스트 ]3-1] GDB를 이용한 코어 덤프 분석


        $ xscale_be-gdb webs core
        GNU gdb 6. 3 (MontaVista 6. 3- 20. 0. 22. 0501131 2005口07- 23)
        copyright 2004 Free software Foundation, Inc.
        GDB is free software, covered by the GNU General Public
        License, and you are welcome to change it and/or distribute cop-
        ies of it under certain conditions.
        Type "show copying" to see the conditions.
        There is absolutely no warranty for GOB. Type "show warranty"
        for details.
        This GOB was configured as "- -host=i686-pc-linux-gnu -target=armv5teb-



386
                                                                    개발 도구      Chapter 13



           니 montavista-linuxeabi ". . .

          core was generated by ' ./webs ' .
          Program terminated with signal 11, segmentation fault.
          Reading symbols from /opt/montavista/pro/ . . ./libc. so. 6. . .done.
          Loaded symbols for /opt/montavista/pro/ . . ./libc. so. 6
          Reading symbols from /opt/montavista/pro/ . . ./ld- linux. so. 3. . .done.
          Loaded symbols for /opt/montavista/pro/ . . ./ld- linux. so. 3
          #0 0x00012ac4 in ClearBiock (RealBigBlockPtr=OxO, 1=100000000) at led.c:43
          43                     必pt r = 0;

          (gdb) 1
          38
          39    static mnt clearBlock (char * BlockPtr, mnt 1)
          40    {
          41       char * ptr;
          42       for (ptr = BlockPtr; (ptr - BlockPtr) <1; ptr++)
          43           *ptr = 0;
          44       return 0;
          45    }
          46    static mnt InitBlock(char * ptr, mnt n)
          47    {
          (gdb) p ptr
          $1 = OxO
          (gdb)




13.1.2 GDB 실행하기
       ［리스트 13-1]의 맨 첫 번째 줄은 커맨드 라인에서 GDB를 어떻게 실행시키는지 보여 준다．
       교차尸디버깅을 하고 있기 때문에 , 호스트 시스템에서 동작하고 타깃 시스템을 디버깅하도록
       하는 GDB 교차 버전이 필요하다. 교차-gdb , 즉 xscale be-gdb를 바이너리 실행 파일
       이름으로 입력하고, 다음에는 core라는 코어 덤프 파일의 이름을 전달한다. GDB가 자신의
       구성과 기타 정보를 출력하는 배너를 몇 줄 출력하고 난 뒤에 , 프로그램이 중지된 원인을 출
       력해 준다. 위의 예에서는 시그널 11번 , 세그먼테이션 폴트2)7} 원인이다. 그 다음 몇 줄은
       GDB가 필요한 라이브러리 바이너리를 로드한다는 메시지이고, 이는 코어 덤프 파일에 따라
       서 달라질 것이다. GDB에서 프롬프트가 뜨기 전에 마지막으로 출력되는 내용은 폴트가 발

2) 시그널과 그어］ 해당하는 번호는 리눅스 소스 코드 . . . /asm-<arch> /signal.h어］ 정의되어 있다．


                                                                                       387 1
   難a     Embedded Linux Primer




        생한 프로그램의 현재 위치이다. #0으로 시작하는 문자열은 스택 프레임3）을 가리킨다（가상
        주소 0x00012ac4의 ClearBiock () 함수를 호출하는 스택 프레임 0) . 그 다음 43으로 시
        작하는 내용은 led. c라는 파일의 소스의 몇 번째 줄인지를 나타낸다. 여기서부터 GDB는
        명령 프롬프트를 출력하고 사용자의 입력을 기다린다．

        내용을 좀 더 보기 위해서 gdb의 lis七 명령어의 축약형인 1을 입력했다. GDB는 모호함이
        없는한 이런 축약형의 명령어를 인식하게 된다. 여기서 프로그램의 에리가 발생한 것을 볼
        수 있는데 , GDB의 코어 덤프 분석에 따르면 문제의 코드는 바로 다음이다．

           43             士ptr = 0;


        다음에는 gdb의 print 명령을 ptr이라는 변수를 대상으로 실행한다. 여기서도 축약형인
        p를 이용했다. ［리스트 13中1]에서 볼 수 있는 것처럼 , p七r의 값이 0이다. 결국 흔한 프로그
        래밍 오류인 널 포인터에 값을 쓰려고 한 것이 세그먼테이션 폴트의 원인이라고 결론 내릴
        수 있다. 이제부터는 backtrace 명령을 이용해서 이 오류를 만들어 내기까지의 호출 단계를
        볼 수 있다. 이를 통해서 실제 오류를 만들어 내는 소스 코드까지 거슬러 올라갈 수 있다．
        ［리스트 13牛2］에 이 결과를 나타냈다．

        ［리스트 ]3-2) Backtrace 명령

           (gdb) bt
           #0 0x00012ac4 in ClearBiock (RealBigBlockPtr=0x0, 1=100000000) at led.c:43
           #1 0x00012b08 in InitBiock (ptr=0x0, n=100000000) at led. c: 48
           #2 0x00012b50 in ErrorlnHandler (wp=0x325c8, urlprefix=0x2f648 "/Error ",
               webDi r=0x2f660 " " , arg=0, url=0x34f30 ''/ Error ' , path=0x34d68 '/ Error ",
               query=0x321d8 ") at led. c: 61
           #3 0x000126cc in websuriHandlerRequest (wp=0x325c8) at handler. c: 273
           #4 0x0001f518 in websGetlnput (wp=0x325c8, ptext=Oxbefffc40,
              pnbytes=0xbefffc38) at webs. c:664
           #5 0x0001ede0 in websReadEvent (wp=0x325c8) at webs. c: 362
           #6 0x0001ed34 in websSocketEvent (sid=l, mask=2, iwp=206280) at webs. c: 319
           #7 0x00019740 in socketDoEvent (sp=0x34fc8) at sockGen. c: 903




3) ［역자주） 스택 프레임이란 함수 등을 호출할 때 그 함수를 위한 인자나 반환 값을 스택에 처장하게 되는더1, 하나의 함수어］ 대한
   이러한 인자들의 묶음을 스택 프레임이라고 한다．


I 388
                                                             개발 도구      Chapter 13



  #8 0x00019598 in socketProcess (sid=1) at sockGen. c: 845
  #9 0x00012be8 in main (argc=1, argv=oxbefffel4) at main. c: 99
  (gdb)



backtrace 명령어는 프로그램의 진입점인 main () 까지 거슬리 올라가는 모든 호출 단계를
보여 준다. backtrace의 각 출력 내용의 앞에는 스택 프레임 번호가 같이 나온다. gdb의
frame 명령어를 이용하면 원하는 스택 프레임으로 이동할 수 있다. ［리스트 13叫3］에서 이
예를 볼 수 있는데 , 여기서 스택 프레임 2번으로 전환해서 이 스택 프레임에 해당하는 소스
코드를 출력하고 있다. 이전 예제에서와 같이 앞에 忖db) 로 시작하는 줄은 모두 GDB에 명
령을 입력한 부분이고 다른 것들은 모두 GDB의 출력이다．

［리스트 13-3) GDB에서 스택 프레임 이동하71

  (gdb) frame 2
  #2 0x00012b50 in ErrorlnHandler (wp=0x325c8, urlprefix=0x2f648 "/ Error ",
      webDir=0x2f660 " "' , arg=0, url=0x34f30 "/Error " , path=0x34d68 '/ Error ",
      query=0x321d8 " ') at led. c: 61
  61             return InitBlock (p, siz) ;
  (gdb) 1
  56
  57              siz = 10000 * sizeof (BigBlock) ;
  58
  59              p = malloc (siz) ;
  60           /* if (p) *1
  61                return InitBlock (p, siz) ;
  62          /* else return (0) ; */
  63      }
  64
  65
  (gdb)



보는 바와 같이 , list 명령을 이용해서 소스 코드를 볼 수 있기 때문에 , 문제의 널 포인터가
사용되는 부분까지 쉽게 역으로 추적해 갈 수 있다. 사실 눈치 빠른 독자는 이 예제 소스 코
드의 어떤 부분이 세그먼테이션 폴트를 일으키게 하는지 알 수 있을 것이다. ［리스트 13-3]
에서 malloc () 함수를 호출한 결과로 반환되는 포인터 주소를 검사하는 부분이 주석 처리
된 것을 볼 수 있다. 즉, 위 예제에서 malloc () 호출이 실패했고, 그래서 이 널 포인터를


                                                                              389
難 RU     Embedded Linux Primer




       가지고 두 단계 후의 스택 프레임에서 사용하려고 할 때 문제가 생긴 것이다. 비록 여키서
       사용한 예제가 작위적이고 너무 간단하치만, 비슷한 방식으로 GDB와 코어 덤프를 활용하면
       이런 종류의 시스템 충돌을 정말 쉽게 추적해낼 수 있다. 또한 함수 호출 시의 파라미터를
       확인해서 널 포인터를 찾을 수도 있다. 이렇게 하면 널 포인터가 처음 발생한 시점의 프레임
       을 바로 찾을 수도 있다．


13.1.3 GDB의 디버그 세션
       이제 일반적인 디버그 세션을 살펴보는 것으로 GDB에 대한 소캐를 끝마치고자 한다. 방금
       살펴본 프로그램 충돌 예제에서 문제의 원인을 좁혀나가기 위해서 코드를 단계적으로 실행시
       키는 방법을 사용할 수도 있었다. 물론 코어 덤프만 가지고 있는 경우에는 항상 그런 방법으
       로 할 수밖에 없지만, 다른 경우에는 브레이크 포인트（breakpoint）를 설정해서 코드를 한
       단계씩 실행시키는 방법도 사용하길 원할 것이다. ［리스트 13-4］를 보면 디버그 세션을 이
       용하도록 GDB를 실행시키는 방법을 자세히 볼 수 있다. 사전에 주의할 점은 프로그램을 빌
       드할 때 gcc에 반드시 디버깅 기능을 활성화시켜서 빌드해야 한다는 것이다． 12장 임
                                                     ，"베디
       드 개발 환경"의 ［그림 12끄을 다시 보면 그 그림이 바로 교차 디버깅 세션을 보여 주고
       있는데 , GDB를호스트개발시스템에서 실행하고, 타깃에서 실행되는프로그램을디버깅하
       는 것이다. 이런 원격 디버깅에 대해서는 15장, "임베디드 리눅스 어플리케이션 디버깅하기"
       에서 상세히 다루기로 하겠다．

       ［리스트 ]3-4] GDB 디버그 세션 실행시키71


         $ xscale_be- gdb -silent webs

         (gdb) target remote 192.168.1.21: 2001
         0x40000790 in?? 0
         (gdb) b main
         Breakpoint 1 at 0x12b74: file main. c, line 78.
         (gdb) C
         Conti nui ng.

         Breakpoint 1, main (argc=1, argv=0xbefffe04) at main. c: 78
         78             bopen (NULL, (60 * 1024) , B_uSE_MALLOC) ;
         (gdb) b ErrorlnHandler
         Breakpoint 2 at 0x12b30: file led. c, line 57.
         (gdb) C



 390
                                                                     개발 도구     Chapter 13



              Continuing.


              BreakpoTht 2, ErrorinHandler (wp=ox3llao, urlPrefix=0x2f648 "/Error",
                  webDir=0x2f660 ", arg=0, url=0x31e88 "tError ", path=0x31918 "/Error",
                  query=0x318e8 ") at led. c: 57
              57                引z = 10000 交 引zeof (BigBlock) ;
              (gdb) next
              59                p = malloc (siz) ;
              (gdb) next
              61                return InitB1oCk (p, sjz) ;
              (gdb) p p
              $1 =(unsigned char *) OxO
              (gdb) p siz
              $2 = 100000000
              (gdb)



         위의 간탄한 디버그 세션을 보면 먼저 gdb의 target 명령어를 이용해서 타깃 보드를 gdb
         에 연결시킨다. 원격 디버깅에 대한 세부적인 내용은 15장에서 다룰 것이다. 타깃 보드에
         연결되고 난 후에는, gdb break（축약형은 b）를 이용해서 main ( ) 함수에 브레이크 포인트
         를 설정한다. 그리고는 gdb continue（축약형은 C) 명령어를 통해서 프로그램을 켸속 실행
         시킨다. 디버깅하려는 프로그램에 인자를 전딜해야 할 경우도 역시 GDB를 실행할 때 같이
         전달해 줄 수 있다．

         main () 어］ 설정해 놓은 브레이크 포인트가 걸리면 다른 ErrorlnHandler () 함수에 브레
         이크 포인트를 하나 더 설정하고（兀ntinue의 축약형 명령어로 실행시켰다. 다시 새롭게 설
         정한 브레이크 포인트가 걸리면 코드를 한 단계씩 flex七 명령을 이용해서 진행해 나가다가
         mailoc () 호출을 만나게 된다. malioc () 호출 이후에는 반환 값을 검사해서 널（null)을
         반환했기 때문에 문제가 생긴 것을 알 수 있다. 마지막으로 mailoc (）어］ 천달된 인수
          (parameter) 값을 출력해 보는데 , 엄청나게 큰 공간(100MB）을 요구했기 때문에 실패한
         것을 볼 수 있다．

         비록 간단한 예제이기는 하지만 이 섹션에서 다룬 GDB 예제만으로도 처음 접하는 사람이
         GDB를 금방 활용할 수 있도록 해 준다. 사실 GDB를 완전히 마스터하고 있는 사람은 별로
         없다. 사용법이 복잡하고 기능이 아주 많기 때문이다. 13.2절 "데이터 표시 디버거 DDD4)"

4) （역天阡］ Data Display Debugger



                                                                                    391 1
  共R     Embedded Linux Primer




       에서 GDB에 익숙하지 않은 사용자를 위해서 그래픽 방식의 UI로 쉽게 사용할 수 있게 해
       주는 툴을 설명하도록 하겠다．

       GDB에 대해서 마지막으로 한 가지 더 언급하자. ［리스트 13-1)에서 GDB가 처음 실행될
       때 콘솔에 출력되는 다앙한 배너 정보를 본 적이 있을 것이다. 앞에서도 언급했치만 현재 예
       제에서는 몬타 비스타 임베디드 리눅스 배포 버전에 포함되어 있는 교차-gdb를 사용하고 있
       다. 표시되는 배너에는 임베디드 개발자에게 아주 중요한 정보가 하나 포함되어 있는데, 바
       로 GDB의 호스트 및 타깃에 대한 정보가 그것이다. ［리스트 13-1]을 다시 보면 GDB를
       실행했을 때 다음과 같은 출력 내용을 볼 수 있다．



         This GDB was configured as '1小ost＝托師巾c- ujn니x띠flu -
            target=armv5teb-montavi sta-1 i nuxeabi "




       앞의 예를 보면 리눅스 PC , 그 중에서도 而86 GNU/Linux 운영쩨제에서 실행되도록 컴파
       일되어 있는 GDB를 실행하고 있다. 또한 타깃을 위해서는 armv5七eb 빅 엔디안 툴 체인으
       로 빌드시킨 ARM 바이너리 코드를 디버깅할 수 있도록 구성되어 있다．

       대부분의 초보 임베디드 개발자가 겪는 흔한 실수 중의 하나는 타깃 실행 파일을 디버그할
       때 잘못된 GDB를 사용하려고 하는 것이다. 뭔가 원하는 대로 동작하지 않으면 곧바로 GDB
       구성을 확인해서 자신의 환경에 맞는 GDB인지 확인하도록 하자 호스트를 위한 GDB를 가
       지고는 타깃 코드를 디버그할 수 없다！



13.2 데이El 표시 디버거
       데이터 표시 디버거 (DDD : Data Display Debugger）는 GDB와 다른 커맨드 라인 방식
       디버거를 위해서 그래픽 방식의 인터페이스5）를 제공하는 툴이다. DDD는 디버그 세션에서
       소스 코드를 확인하고 코드를 한 단계씩 실행시키는 것 외에도 다앙힌 확장 기능을 가지고
       있다. ［그림 13-1)은 DDD 주 화면의 스크린 샷을 나타낸 것이다．


5) ［역자주） DDD는 실제적으로 GUT만을 제공하고 LU를 통해서 사용자가 조작한 내용을 그에 대응하는 GDB 커맨드 라인 명령으로
   바꿔서 실행시켜 준다．
                                                                                                                               개발 도구   Chapter 13



 F如        트dit      V地V/   므n｝甲sin       드ommand$   司atu$   흐ource   으ala                                 브．etp
r             ,                             出r茹J 4hr L1寸 4 !   '1 !   ! /a 牛 im 寸 1{:                           L:J
U rnaln. C: b포                            /L品斗 g? 茫C y了， r,;. 1妃 . :1, ｝如 "    DD 乂                               二
                                                                                                                ' "；




                                                                                               Run     1
                                                                                       tnterrupt 1
                                                                                      St芟 I 佃d}
                                                                                      N텨t } 枇a七 i
                                                                                      Us미 耐hi
／中
                                                                                      cmiti tv         1   客有
              Main          entry point from
                                                                                           나） 油삐
      :/               -




m "t main     (lnt     argc.   char   "    argv)
                                                                                      U,
                                                                                           『J0i fwd口
                                                                                           4
                                                                                                       1
                                                                                      뗀1 쁘竺］                               1
                                                                                      m寸               /                   1
              Initialise the menmry allocator. Allow use of malluc and start
 /!
              with a 60K heap. 다｝reach 口age req나tot a먀玎at 1KB is all吼欲ed.
              60KB allows for several concurrent page requests. If 乍그re space
      1       is required. nalloc will be used for the overflow.
      中／
              bo口en（卜川나mCE0 中 1024) , 已USEJ快LLOC);
              signal CSIGPIPE. SIC_I애);

 /+
              Initialize the web server
      中／
              If (Is寸t나abs C) < 0) {
                      return -1;
              }
州fdef N炬BS_SSL.돼PPORT
       叫ebsSSL0口enO;
井endif

I.
  小           Ba引c event loop. socketgeady returns true when a socket is ready for
              service. tocketSelect will block until an event occurs. SocketProcess
              나ill actually do the oervicisg.
      小／
             小m                             小mm                              ,   :      ，寸，
                                                                                     ：口卜，
                                                                                                                       ,   /


韓照照難難萍藝埠難韓君"'""' Germany.
芝 Bt。DDD
     2003
      ，『“:,，二쓰：
       3.『，   ,:,,,flu)                                                                                            I'-k
I 그림 13너 데이터 표시 디버거


DDD는 다음과 같이 실행시킨다．

           $ ddd --debugger xscale_be-gdb webs


--debugger 플래그 없이 실행하면 DDD는 개발 호스트 시스템을 위한 GDB를 실행시키
려고 하게 된다. 하지만 우리는 타깃 시스템에 있는 어플리케이션을 디버그해야 하기 때문에
이 인자를 이용해야 한다. DDD 커맨드 라인의 두 번째 인자는 디버그하고자 하는 프로그램
의 이름이다. 더 자세한 내용은 DDD 맨 페이지를 보도록 하자．




                                                                                                                                             393 I
 3聲 1          Embedded Linux Primer



        ［그림 13-끄에서 볼 수 있는 명령에 도구 창6）을 이용해서 , 프로그램을 이동시켜 가면서 실
        행시켜 볼 수 있다. 그리고 그래픽 인터페이스를 이용하거나 또는 DDD 화면 아래쪽혀］ 있는
        GDB 콘솔 창에 직접 입력해서 브레이크 포인트를 설정할 수 있다. 타깃 디버깅을 위해서，
        먼저 ［리스트 13寸4］에서 한 것과 같이 디버거를 타깃 시스템에 연결해야 하는데, 이 명령은
        DDD 주 화면에서 GDB 창을 통해서 내릴 수 있다．

        타깃에 연결되면 이전 예제에서 프로그램 오류 원인을 좁혀나갈 때 사용한 방법과 같은 명령
        어들을 이용해서 프로그램을 실행시켜 볼 수 있다. ［그림 13-2］에서 디버깅의 후반 과정에
        서의 DDD 화면을 볼 수 있다．

         F如        트d什          찐pa/     므ro甲am    드ommand$         司atu$    흐ourca        므eta                                                            브．p巾
              m二                                     느뇨       4A!   44h !
                                                  ' （品. 『飄· 諶됴 u헒n p, : 碼
                                                                            戶n 1   a   '     1 r   k.
                                                                                                   崙＝ 冬］
                                                                                                        '   / :,   r      r= r
                                                                                                                                  =: 處｝       包山            1 +"

        (｝三已小：                                                                                                     1
                                                                                                                   尸；
                                                                                                                                                              D
          "    "   "   '


                                                                                                                              Rus                  H
               1: p
               (unsigned char              ) 0a31tf0 'text/html "                                                        In旭口upt 1
                                                                                                                   1 Step 1 跏1生 引
                                                                                                                                                       r
               2: 引z
                   0
                                       3: un]
                                       (cha乙t 中) OuJibdO '/ Error "                                                1    NXt
                                                                                                                        ．나口
                                                                                                                               1Neetn
                                                                                                                        1月111 1 rH口Jr1 1
                                                                                                                                        已n.




                                                                                                                                                       m4i
                                                                                                                        Conti            re
        ,"" " " ""寐"就！' 盒쁜計渭：密紮｛：品出' !：즘；cli
                                        -t 旒듦；쁘""" "'                                                                   Hr 기
                                                                                                                            !
                                                                                                                        dY幻i 斗d口

                       准坦撰 char "
                                                                                                                                                   1
                                                                                                                   \
                                                                                                                        P可在하                           J
        斗如             引2 口 10000 小 引2B0f (Bi9BlSCk가



        ;
                       口 - mall吼（引0);

                           鞋’      ｛많
                                 "弓.       '嗇k    (p, nlz);                                                                                                   ]

        麓降難常舞：抑＝「                                                                                           「                                                三/
        孕 Display t p (enabled, scope trrorlnhandler, address 0abefffa?4)                                                                                    乍

        I 그림 13-2 DDD의 디버그 ,（斗션


        ［그림 13-2］를 보면 세그먼테이션 폴트의 원인을 좁힐 수 있는 중요한 프로그램 변수를 표
        시하도록 설청한 것을 볼 수 있다. 이러한 변수들은 프로그램을 한 단계씩 실행시켜 감에 따
        라서 그림에서 볼 수 있는 명령에 도구들을 이용해서 확인할 수 있다．




6) （역자주） 화면에서 DD로 표시된 툴바tm를 말힌다．



I 394
                                                          개발 도구   Chapter 13




      DDD는 GDB를 위한 강력한 그래픽 인터페이스 툴이다. 또한 사용법이 상대적으로 쉽고，
      많은 개발 호스트에서 사용할 수 있다. 이 장의 마지막에 있는 13.7.1절에서 GNU DDD
      문서에 대한 홈페이지를 한번 방문해 보기 바란다．



]3.3 cbro吼이厄Sc야）e
      cbrowser를 여기서 소개하는 이유는 이 간단한 툴에서 사용되는 기반 엔진이 리눅스 커널
      소스 트리7）에서도사용되기 때문이다. cbrowser는 간단한 소스 코드 탐색 툴인데 , 심볼을
      통해서 큰 소스 구조를 쉽게 이동하면서 참조할 수 있도록 돕는 툴이다．

      리눅스 커널 makefile에서 cbrowser에서 사용할 수 있는 데이터베이스를 만들 수 있다．
      다음은 최신 리눅스 커널에서 이 makefile 타깃을 실행하는 예제이다．

         S make ARCH=PPC CROSS_COMPILE=ppc_82xx- cscope


      위 명령은 cbrowser에서 사용할 수 있는 csc아氾 심볼 데이터베이스를 생성한다. cscope
      는 엔진을 가리키고, cbrowser는 이 데이터베이스 엔진을 위한 그래픽 인터페이스를 담당
      한다. 필요한 경우에 cscope를 바로 사용할 수도 있다. cscope는 커맨드 라인 방식의 아
      주 유용한 툴이지만, 요즘같이 소스 트리를 간단히 찾아서 클릭하는 시대에는 사용이 어렵
      게 느껴질 수도 있다. 만약 vi 에디터를 애용하는 독자라면 csc아氾 역시 아주 좋아하게 될
      것이다！

      cbrowser를 실행시키려면 csc아氾 데이터베이스가 있는 디렉터리로 이동한 후에 , 간단히
      cbrowser 명령어를 별도의 인자 없이 입력하면 된다. ［그림 13-쏘은 동작하는 예를 보여
      주고 있다. 이 장 마치막의 13.7.1절에 정리되어 있는 참고 자료를 통해서 이 유용한 툴에
      대한 좀 더 자세한 내용을 읽을 수 있을 것이다．




7) 실제로 cbro텍嵌才가 사용하는 엔진이 사용되는 곳은 리눅스 빌드 시스템이다．


                                                                       395I
        U        Embedded Linux Primer




            日e        Edit     蚤이ect   네S切ry      options   旦e巾

            Selected Database ( csco,e ):         ,boiiielchns忿ajidboxfttiiux-2 .t.i 4/csropo』
                                                                                             uut    二J                       r


            1 SlltlIlilt       Syllit)마｛      rnpc52兀，=r已：L키t                                                            ;J

             mpc5200.11' in <glotaJ , at line 413: extern void mpcS料_restart(char cmd):
             1i1e5?flt].c ' in piattorm_irlit, at line 222: ppc_md.restart = mpc52xx_restart;
            pttwerdna.c " in platlorm_init, at巨ne 234: ppc_md.res切rt = mpc5乙x_rastart;
            繇i苡受t瓮注ati在Oil恥奴珏玉呱프必a11發I쿄ii日a五쨔l；夙珏三妊立多31王珏珏侄atmi;t르11r4H




                  ,                                                                                           쏘11
            日In: !                                                                                           tine: !


                        꾸a工d
            m啼          궤Fc52？匹r的tart (c如r 1 cied)
                        {
                                $ttt畔t 畔心2,吃叩七 1H' Oulnere ＋可pt出 = 加PCS2s口c VA（蝴？C52,vc小SPTx OFFSET

                                   local_珏吼dioab노 (1                                                                     :

                                   1t L뇨cm on the vatchd四 and 甘sit for l匕 to exp.re                工I eff弓C乞Lv已Ly
                                     doe包 크 reset 4/
                                   Out中b
                                       be3묘 (&gptt- >ceunt, OcOOOOLlOff) ,
                                   口ut_be 32侮叩比- mode, mcOOO090l萸）;

                                   낚心好     (I.)
                           }

                        Vt珏d

        ！쿄                                                                                               !          』，




                                        Found 4 matches tur 'Syuil마s: m13c525x_restart '1


        I 그림 ]3召 실행중인 cbrowser




13.4 추적 및 프로파일링 도구
        여러 유용한 툴을 이용하면 시스템을 다양한 관점에서 볼 수 있다. 일부 툴은 시스템에 어떤
        프로세스가 실행중이며 , 어떤 프로세스가 Cpu를 얼마나 점유하고 있는지와 같이 시스템의
        상위 레벨 관점을 볼 수 있게 해 준다. 또 어떤 툴은 더 자세한 분석 , 즉 얼마만큼의 메모리를
        할당하고 있는지 , 또 더 유용한 정보로 얼마만큼의 메모리가 누수8）되고 있는치 등을 알 수
        있게 해 준다. 이어지는 일부 섹션에서는 이러한 종류의 유틸리티 중에서도 가장 중요한 몇
        개를 소개하도록 하겠다. 이 책에서는 지면관계상 이 툴들에 대해서 간단히만 알아보고 넘어
        가도록 한다. 이 장 뒤편에 있는 참고 자료에서 더 자세한 정보를 얻을 수 있으니 참고하도록
        하자．




8) （역자주） 메모리가 프로그램의 부적절한 메모르］ 관리로 인해서 사용되지 않으면서도 할당되어 있는 것을 메모리 누수라고 한다．


I 396
                                                                     개발 도구     Chapter 13




13.4.1 strace
     이 추적（trace) 유틸리티는 사실상 모든 리눅스 배포 버전에 포함되어 있다. S七race는 리
     눅스 어플리케이션 프로그램이 호출하는 커널 시스템 콜에 대한 정보를 캡처해서 표시해 주
     는 일을 한다. S七race는 소스 코드가 없는 프로그램을 대상으로도 실행시킬 수 있기 때문에
     아주 편리하다. 즉, GDB에서와 같이 프로그램에 별도로 특별한 옵션을 줘서 디버깅 심벌을
     포함하도록 빌드시킬 필요가 없다. 또한 S七race는 자체적으로 상당히 교육적인 가치도 있
     다. 맨 페이지에서는 "학생들과 해커들 그리고 호기심에 넘치는 사람들은 일반 프로그램을
     추적하는 것만으로도 시스템과 시스템 콜에 대해서 상당한 정보를 배울 수 있을 것이다"라고
     언급하고 있다.

     이 장의 앞부분인 GDB 섹션에서 사용한 예제 소프트웨어를 만들 때 필자는 다소 생소한 소
     프트웨어 프로젝트를 이용하는 것이 좋겠다고 마음 먹었는데 , 그래서 선택한 소프트웨어가
     伽Ahead 웹 서버의 초기 버전이다. 이 소프트웨어를 처음 컴파일해서 링크했을 때
     strace를 써서 해결할 수 있을 만한 재미있는 현상을 발견했기 때문이다. 이 프로그램을
     커맨드 라인에서 실행시키면 아무런 메시지도 출력하지 않고 그냥 다시 콘솔로 되돌아온다．
     아무런 에러 메시지도 없고, 시스템 로그에서 어떤 단서도 출력된 것이 없었다！ 그냥 실행하
     지 않고 종료되어 버린 것이다．

     S七race를 이용하면 문제를 빨리 찾아낼 수 있다. 이 어플리케이션을 대상으로 S七race를
     실행한 결과가 ［리스트 13寸5］에 나와 있다. 공간 문제로 많은 부분을 생략했다. 실제 출력
     내용은 수백 줄 이상이 된다．

     ［리스트 13-5] strace 출력： GoAhead 웹 서버 데모


        01 root@coyote: /home/websdemo$ strace ./websdemo
        02 execveC' . /websdemo ", [". /websdemo "'] , [/"" 14 vars 少"/ ] ) = 0
        03 uname ({ sys="Li nux ", node="'c oyote", . . .}) = 0
        04 brk (0)                                           = 0x10031050
        05 openC'/ etc/ld. so. preload", O_RDONLY)           = -1 ENOENT (No such file or
         1directory)
        06 open ("/ etc/ld. so. cache", O_RDONLY)            = -1 ENOENT (No such file or
         니 directory)




                                                                                     397 器
   難R   Embedded Linux Primer



        07 open("/ lib/ libc. so. 6", 0_RDONLY)      = 3
        08 read(3, "\177ELF\1\2\1\0\0\0\0\0\0\0\0\0\0\ 3\0\ 24\0\0\0\1\0\1\ 322 ". . . ,
         니 1024) = 1024
        09 fstat64(0x3, 0x7fffefc8)                    = 0
        10 mniap (Oxfe9f000, 1379388, PROT_READIPROT_EXEC, MAP_PRIVATE, 3, 0) =
         니 0xfe9f000
        11 mprotect (0xffd8000, 97340, PR0T1N0NE)     = 0
        12 mmap(Oxffdf000, 61440, PR0T1READIPR0T_WRITEIPROT_EXEC,
         니 MAP_PRIVATEIMAP_FIXED, 3, 0x130000)        = 0xffdf000
        13 mmap(oxffee000, 7228, PROT_READI PR0T1WRITEI PROT1EXEC,
         니 MAP_PRIVATEIMAP_FIXEDMAP_AN0NYM0US, -1, 0) = 0xffee000
        14 close (3)                                  = 0
        15 brk (0)                                    = 0x10031050
        16 brk (0x10032050)                           = 0x10032050
        17 brk (0x10033000)                       = 0x10033000
        18 brk (0x10041000)                       = 0x10041000
        19 rt_sigaction(SIGPIPE, {sIG_IGN} , {SIG_DFL} , 8) = 0
        20 stat (". /umconfig. txt ", 0x7ffff9b8)      = -1 ENOENT (No such file or
         니 directory)
        21 uname ({ sys="Linux ", node="coyote", . . .})   = 0
        22 gettimeofday ({ 3301, 178955} , NULL)           = 0
        23 getpid ()                                       = 156
        24 open("/ etc/resolv. conf", O_RDONLY)            = 3
        25 fstat64 (0x3, 0x7fffd7f8)                   = 0
        26 mmap (NULL, 4096, PROT_READIPROT1WRITE, MAP1PRIVATEIMAP_ANONYMOUS, -1,
         니 0) = 0x30017000
        27 read(3, "#\n# resolv. conf This file is th " . . . . 4096) = 83
        28 read(3, ", 4096)                                            = 0
        29 close(3)                                                    = 0
          . <<< 30-81 줄은 생략했음
        82 socket (PF_INET, SOCK_DGRAM, IPPROTO_IP)                    = 3
        83 connect (3, {sa_family=AF_INET, sin_port=htons (53) ,
         니 sin_addr=inet_addr ( "O.O. O. O") }, 28) = 0
        84 send(3, "\ 267s\1\0\0\1\0\0\0\0\0\0\6coyotea\0\0\1\0\1", 24, 0) = 24
        85 gettimeofday({ 3301, 549664} , NULL)      = 0
        86 poll ([ {fd=3, events=POLLIN, revents=POLLERR} ], 1, 5000) = 1
        87 ioctl (3, 0x4004667f, 0x7fffe6a8)        = 0
        88 recvfrom(3, 0x7ffff1f0, 1024, 0, 0x7fffe668, 0x7fffe6ac) = -1
         니 ECONNREFUSED (Connection refused)
        89 close (3)                            = 0
        90 socket (PF_INET, SOCK_DGRAM, IPPROTO_IP) = 3



毋 398
                                                                    개발 도구   Chapter 13



          91 connect(3, {sa_family=AF_INET, sin_port=htons (53) ,
           니 sTh_addr=inet_addr ( "O. O. O. O")}, 28) = 0
          92 send(3, "\ 267s\1\O\O\1\0\O\O\O\0\0\6coyote\0\O\1\O\1 ", 24, 0) = 24
          93 gettimeofday({3301, 552839} , NULL)       = 0
          94 poll ([ {fd=3, events=POLLIN, revents=POLLERR} ], 1, 5000) = 1
          95 ioctl (3, 0x4004667f, 0x7fffe6a8)        = 0
          96 recvfrom(3, 0x7ffff1f0, 1024, 0, 0x7fffe668, 0x7fffe6ac) = -1
           니 ECONNREFUSED (Connection refused)
          97 close(3)                              =0
          98 exit(-1)                              =7
          99 root@coyote : /home/websdemo#



       출력된 내용을 좀 더 쉽게 읽기 위해서 strace가 출력한 줄에 대해서 줄 번호를 앞에 표시
       했다. 명령을 내리는 부분은 줄 번호 01번에 있다. strace 명령을 실행시키는 가장 간단한
       형태로 strace 명령에 뒤에 별다른 옵션 없이 바로 시험해 볼 프로그램을 전달해 준다. 그
       러면 ［리스트 13-5］와 같은 내용이 출력될 것이다．

       여기서 추적한 각 줄의 내용은 websdemo 프로세스가 커널로 호출하는 시스템 콜을 나타낸
       다. trace가 출력한 각 줄을 모두 분석해 보면 도움은 되겠지만, 지금은 그렇게까치 할 필요
       는 없다. 여기서 프로그램이 실행되지 않는 원인을 짚어 낼 수 있는 이상 상황을 짖아내야
       한다. 처음 몇 줄은 리눅스가 실행시킬 프로그램을 위한 환경을 갖추는 작업을 하는 부분이
       다. /etc/ld. so．培 대상으로 open () 시스템 콜이 몇 번 호출되는 것을 볼 수 있는데，
       이는 리눅스 동적 링커尸로더가 자신의 작업을 수행하면서 호출하는 것들이다. 여기서 6번째
       줄의 내용은 필자가 보기에는 임베디드 보드가 올바로 구성되지 않은 것을 알 수 있는 단서가
       되는 부분이다. 이 경우에는 ldconfig를 실행해서 링커 캐시를 반드시 만들어 주어야 한다
       （링커 캐시는 공유 라이브러리에 대한 참조를 찾는 속도를 상당히 개선시켜 준다）. 이 문제
       는 타깃 시스템을 대상으로 lclconfig9）를 실행해서 해결할 수 있다.

       19번 줄 아랫부분은 더 기본적인 작업들을 진행하고 있는데, 대부분이 로더가 libc를 초기
       화하는 부분이다. 20번 줄은 프로그램이 구성 파일을 찾으려고 하치만 실패하는 것을 볼 수
       있다. 이 부분은 현재 문제를 해결해서 소프트웨어가 정상적으로 실행되었을 때 문제가 될
       수 있는 부분이다 프로그램은 24번 줄을 시작으로 필요한 네트워크 자원을 설정하는 것을


9) 타깃 시스템을 위한 링커 캐시를 만드는 방법에 대해서는 man Idcon1ig를 보71 닙尾k가．
 纛1 1     Embedded Linux Primer




        볼 수 있다. 24에서 29번째 줄은 DNS 서비스가 호스트 이름을 파악할 수 있는 구문을 담고
        있는 리눅스 시스템 파일을 열어서 읽으려는 부분이다. 이런 로컬 네트워크 구성을 위한 작
        업을 81번째 줄까지 진행하는데 대부분 네트워크를 설정하고 프로그램에서 사용하기 위한
        네트워크 기반 구성을 갖추기 위해서 필요한 작업이다. 이 부분에 대한 내용은 분량이 많아
        서 내용을 좀 더 간략하게 보이기 위해서 생략했다．

        82번째 줄부터 시작하는 내용을 한 번 살펴보자. 여기서 프로그램이 TCP/II) 연결을 맺으려
        고 시도하고 있는데 , 대상 'P 주소가 모두 0인 것을 볼 수 있다. 다음에 편의상 82번째 줄을
        다시 나타냈다．

          socket (PF_INET, SOCK_DGRAM, IPPROTO_IP) = 3


        ［리스트 13-5］에서 서로 짝이 되는 부분을 주의할 필요가 있다. 모든 시스템 콜을 다 알 수
        는 없지만 대신에 어떤 일이 일어나고 있는지에 대한 일반적인 아이디어를 얻을 수 있다．
        socket () 시스템 콜은 파일 시스템의 open () 과 비슷하다. 그리고 = 표시로 나타내는 반
        환 값은 리눅스의 파일 기술자（descr如切r）를 의미한다. 이러한 정보를 알고 있기 때문에，
        82번 줄의 내용과 89번째 줄의 close () 시스템 콜의 파일 기술자 3을 서로 연관시킬 수
        있다．

        88번째 줄에서 "Connection refused"라는 에러 메시지가 있기 때문에 이와 관련된 시스템
        콜을 주의해서 살펴봐야 한다. 아직 현 시점에서는 왜 프로그램이 실행되지 않는지에 대해서
        는 모르는 상태이지만, 이 부분이 이상하1 보인다는 것은 알고 있다. 그럼 이 부분을 조사해
        보자. 82번째 줄에서 socke七 () 시스템 콜을 호출해서 'I) 통신을 위한 종단점을 하나 생성
        했다. 그리고 83번째 줄에서 수상하게도 IF) 주소가 모두 0으로 이루어져 있는 원격의 장치
        (socket）에 연결을 시도하고 있다. 이 부분이 문제10）를 일으킬 것이라는 것은 전문가가 아
        니더라도 누구나 의심해 볼 수 있다. 83번째 줄에서 다른 중요한 단서를 얻을 수 있는데 바로
        port 파라미터가 53으로 설정되어 있다는 것이다. 구글에서 간단히 검색해 보면 TCP/IP
        에서 53번 포트는 도메인 네임 서비스 또는 DNS를 위한 포트 번호인 것을 알 수 있다.




10) Ii) 주소가 모두 0으로 이루어져 있는 것이 어떤 경우에는 올바른 값일 때가 있다. 하지만 우리는 프로그램이 왜 비정샹적으로
    종료했는지를 조사하는 중이기 때문어］ 이 부분을 의심해 보기로 하자．
                                                             개발 도구   Chapter 13




       84번째 줄은 또 다른 단서를 제공해 준다. 우리가 사용하는 타깃 보드는 호스트 이름으로
       coyo七e라는 이름을 사용한다. 이는［리스트 13-旬의 01번 줄의 커맨드 프롬프트에서도 일
      부 볼 수 있다. 결국 이 내용은 보드의 호스트 이름에 맞는 DNS를 찾는 일을 하는데 이 작업
      이 실패한 것으로 생각할 수 있다. 실험 삼아서 다음과 같이 타깃 시스템의 /etc/hosts11)
       파일에 항목 하나를 추가해서 자체적으로 정의한 호스트 이름과 자체적으로 정의된 보드의
       'P를 연결시키도록 하자．

          Coyote   192.168.1. 21     # IP 주소 할당


      자, 이렇게 하니까 프로그램이 정상적으로 실행되는 것을 볼 수 있다. 비록 어떤 이유로 프로
       그램이 실행되지 못했는지 정확한 원인은 알지 못하지만（TCP/II) 네트워크 전문가는 알겠
      지만）, strace의 출력물을 통해서 DNS가 우리의 이름에 해당하는 H) 주소를 찾지 못한다
      는 것을 알아냈다. 그리고 이 문제를 수정했을 때 행복하게도 프로그램이 정상적으로 실행되
      어서 웹 페이지를 서비스할 수 있게 되었다. 다시 정리하면 프로그램에 대해서 참고할 만한
       소스 코드도 없었고, 바이너리 실행 이미지 내에 컴파일 시에 포함된 심볼 정보도 가지고 있
      지 않았다. 하치만 strace를 이용해서 프로그램이 실패하는 원인을 찾아내고, 그 해결책도
      결정할 수 있었다．


13.4.2 strace의 다양한 기능
       strace 유틸리티는 많은 커맨드 라인 옵션을 가지고 있다. 그 중에서도 쓸 만한 기능으로는
       추적할 시스템 콜의 종류를 선택할 수 있는 옵션이다. 예를 들어 , 독자가 어떤 프로세스에
      대해서 네트워크 관련된 활동만을 추적해 보고 싶으면 다음과 같이 명령을 내리면 된다．

          $ strace -e trace=network process_name


       이렇게 하면 socketO, connec七（) , recvfrom () 그리고 send() 등의 네트워크와 관
       련된 모든 시스템 콜을 추적해서 출력해 준다. 이는 프로그램이 네트워크에 관련해서 어떤
      작업을 수행하는지를 볼 수 있는 강력한 방법이다. 이 외에도 선택할 수 있는 다른 계열이
      몇 개 더 있는데 , 한 예로 openO, closeQ, read() , write () 등의 파일 관련 작업만
       선택적으로 추적할 수도 있다. 이렇게 선택할 수 있는 다른 항목으로는 프로세스 관련 시스
      템 콜, 시그널 관련 시스템 콜 그리고 'PC 관련 시스템 콜 등이 있다．

11) hosts에 대한 맨 폐이지에서 이 시스템 곤杞1를 위한 파일에 대한 자세한 내용을 볼 수 있다．


                                                                          401 1
 , 堪1     Embedded Linux Primer




        또한 S七race는 추가적인 자식 프로세스를 만들어 내는 프로그램도 처리할 수 있다．
        strace를 -f 옵션을 주고 실행시키면 fork () 시스템 콜을 이용해서 생성되는 자식 프로
        세스에 대해서도 strace7} 동작을 추적할 수 있다. strace 명령어는 다양한 가능성을 가
        지고 있다. 이 강력한 툴을 능숙하게 이용하는 가장 좋은 방법은 많이 써보는 것 밖에 없다．
        여기서 설명하는 툴을 자주 써보고 필요하면 최신 오픈 소스 문서를 찾아서 공부하는 것이
        가장 좋다. 대부분의 리눅스 호스트 시스템에서 man s七race를 입력하면 공부해 볼 만한
        충분한 내용을 볼 수 있을 것이다．

        S七race에서 사용할 만한 다른 유용한 옵션으로는 -c 옵션이 있다. 이 옵션은 어플리케이션
        을 대상으로 상위 레벨의 프로파일링12）을 생성해 준다. -c 옵션을 이용하면 strace는 사
        용된 각각의 시스템 콜에 대해서 몇 번씩 호출되었고, 에러를 반환한 횟수는 얼마인지 그리
        고 실행된 시간은 얼마인지를 계산해서 통계를 출력해 준다. ［리스트 13-6］을 보면 strace
        -c로 이전에 예제로 사용한 webs 데모 프로그램을 실행한 결과를 볼 수 있다．

        ［리스트 ]3-6) strace릍 이용한 프로파일링

          root旦coyote$ strace -c ./webs
          % time    seconds usecs/call    calls   errors   syscall

            29. 80    0.034262     189    181              send
            18. 46    0.021226    1011     21       10     open
            14.11     0.016221     130    125              read
            11. 87    0.013651     506     27       8      stat64
             5. 88    0. 006762    193     35              select
             5. 28    0. 006072     76     80              fcnt164
             3. 47    0. 003994     65     61              time
             2. 79    0. 003205   3205      1              execve
             1. 71    0.001970      90     22       3      recv
             1. 62    0.001868      85     22              close
             1.61     0. 001856    169     11              shutdown
             1. 38    0. 001586    144     11              accept




12) ［역자주］ 프로파일링이란 프로그램 내에서 어떤 함수가 얼마만큼 호출되었고， 얼마의 시간 동안 실행되었는지 등을 분석하는
  것을 말한다．


 402
                                                   개발 도구   Chapter 13



                                C
                                J
   0. 41    0. 000470    94                mmap2
                                mJJ
   0. 26    0.000301    100                mprotect
                                mJJ
   0. 24    0.000281     94                brk
                                l
   0.17     0. 000194   194           1    access
                                l
   0.13     0. 000150   150                iseek
                                m1J
   0.12     0.000141     47                uname
                                l
   0.11     0. 000132   132                listen
                                l
   0.11     0. 000128   128                socket
                                )
                                L
   0. 09    0.000105     53                fstat64
                                l
   0.08     0.000097     97                munmap
                                l
   0.06     0.000064     64                getcwd
                                1
                                上
   0.05     0. 000063    63                t너 nd
                                4
                                l
   0.05     0.000054     54                setsockopt
                                l
   0.04     0.000048     48                rt_sigaction
                                d
                                l
   0.04     0.000046     46                gettimeofday
                                l
   0.03     0.000038     38                getpid

  100. 00   0.114985          624     22   total



프로파일링을 이용하면 어플리케이션이 어디서 얼마만큼의 시간을 소비하고, 에러는 어디서
발생했는지 등에 대해서 상위 레벨 관점에서 정보를 얻을 수 있다. 에러 중의 일부는 어플리
케이션의 수행 중에 일어날 수도 있는 정상적인 것인 반면에 , 일부는 의도하지 않게 시간을
많이 소비하는 에러도 있다. ［리스트 13-6］을 보면 가장 많은 시간이 걸린 시스템 콜은 쉘이
어플리케이션을 실행시키기 위해서 호출한 execve () 인 것을 알 수 있다. 그리고 이 호출은
딱 한번만 이루어졌다는 것도 알 수 있다. 그리고 다른 흥미로운 부분으로 send() 시스템
콜이 가장 많이 호출되었다는 것을 볼 수 있는데 , 이는 이 어플리케이션이 작은 웹 서버이기
때문에 충분히 이해가 가는 부분이다.

지금까지 소개한 다른 툴과 마찬가지로 S七race도 독자가 사용하는 타깃 시스템에 맞게 컴
파일되어 있어야 한다는 것을 유념하도록 하자. strace는 개발 호스트 시스템이 아닌 타깃
보드 상에서 실행시켜야 한다. 반드시 자신의 타깃 시스템 아키텍처와 호환되는 버전을 사용
해야 한다. 만약에 상업용 임베디드 리눅스 배포판을 사용한다면 자신의 아키텍처에 맞는 유
틸리티가 포함되어 있는지 먼저 확인해야 한다．




                                                                403     I
  難1     Embedded Linux Primer




13.4.3 Itrace
       1trace와 strace 유틸리티는 서로 밀접한 관계가 있다. strace는 시스템 콜을 대상으로
       동작하고, itrace 유틸리티는 라이브러리 호출을 대상으로 한다. 호출 방식도 비슷하다. 다
       음과 같이 추적할 프로그램을 인자로 넣으면 된다．

         $ itrace ./example


       ［리스트 13끼은 간단한 표준 （二 라이브리리를 호출하는 프로그램을 1七race를 이용해서 실
       행한 결과를 나타낸 것이다．

       ［리스트 ]3-7) 1七race의 출력 예제

         $ itrace ./example
         _libc_start_main(0x8048594, 1, 0xbffff944, 0x80486b4, 0x80486fc
           니 <unfinished . . . >
         malloc (256)                                   = 0x804a008
         getenv("HoME")                                 = "/ home/chris "
         strncpy (0x804a008, "/ home", 5)               = 0x804a008
         fopen("foo. txt", "w")                         = 0x804a110
         printf ("$HoME = %s\n", "/ home/chris"$HOME = /home/chris
         )               20
         fprintf (0x804a110, "$HOME = %s\n", "/ home/chris") = 20
         fclose(0x804a110)                              = 0
         remove("foo. txt")                           =   0
         free(0x804a008)                                = <void>
         -1-++ exited (status 0) +++
         $



       각각의 라이브러리 호출에 대해서 , 해당하는 함수 이름과 사용된 파라미터도 함께 출력된다．
       S七race와 비슷하게 함수를 호출한 결과 반환 값도 같이 출력된다． S七race와 마찬가치로
       이 툴도 소스 코드가 없어도 사용할 수 있다．

       strace의 경우처럼 1七race도 다양한 스위치로 동작을 선택할 수 있다. 어플리케이션의 실
       행 흐름을 이해하는 데 도움이 되도록 각 라이브러리 호출에 대해서 그 함수를 호출하는 프로
       그램 카운터13）를 같이 출력하게 할 수도 있다. 그리고 strace와 같이 c 옵션을 주면 라이
       브러리 함수에 대해서 호출된 횟수, 에리 횟수, 실행된 시간 등의 통계를 볼 수 있기 때문에，

 404
                                                                             개발 도구   Chapter 13



       간단한 프로파일링 툴로 사용할 수 있다. ［리스트 13-8］은 간단한 예제 프로그램을 -c 옵션
       을 통해서 실행한 결과이다．

       ［리스트 ]3-8] 그上race릍 이용한 프로파일링

           $ itrace -c ./example
           $HOME = /home/chris
           % time     seconds usecs/call             calls        function

            24.16      0. 000231          231          1 printf
            16. 53     0.000158           158          1 fclose
            16. 00     0. 000153          153          1 fopen
            13. 70     0.000131           131          1 malloc
            10. 67     0. 000102          102          1 remove
             9. 31     0. 000089           89          1 fprintf
             3. 35     0. 000032           32          1 getenv
             3.14      0. 000030           30          1 free
             3.14      0. 000030           30          1 strncpy

           100. 00     0. 000956                        9 total



       1七race 툴은 동적으로 링크된 공유 라이브러리를 사용하도록 컴파일된 프로그램만 사용할
       수 있다. 컴파일할 때 명시적으로 -s七a七Ic 옵션을 주지 않는한 기본적으로 공유 라이브러
       리를 사용하도록 되어 있기 때문에 , 생성된 바이너리 실행 파일에 대해서 ltrace를 사용할
       수 있다. 다시 말하지만, S七race와 마찬가치로 1七race 바이너리 파일도 타깃 아키텍치를
       위해서 컴파일되어 있어야 한다. 이 유틸리티는 호스트 시스템이 아닌 타깃 시스템에서 동작
       시켜야 한다．


13.4.4 ps
       strace와 1七race를 예외로 두면 top과 PS만큼 임베디드 시스템 개발자들에게 무시되는
       툴도 없을 것이다. 이 유틸리티에 적용할 수 있는 수많은 옵션을 생각해 보면 이 유용한 시스
       템 프로파일링 툴을 설명하는 데만 한 챕터 전부를 할당해도 될 정도다. 이 툴은 대부분의
       임베디드 리눅스 배포 버천에 기본적으로 포함되어 있다．

13) （역자주） 현재 프로세서가 명령어를 가져오는 주소 긴딘히 현재 프로세서에 의해서 실행되고 있는 프로그램 메모리 주소라고
  생각하면 된다. IF (Instruction Pointer) , PC (Program Counter) 등의 용어가 사용된다．
        Embedded Linux Primer




       PS와 t아）유틸리티는 9장, "파일 시스템"에서 설명한 /proc 파일 시스템을 이용한다. 만약
       에 독자가 /proc 파일 시스템의 어디를 참고해야 하는지 , 정보를 어떻게 분석해야 하는지만
       알고 있다면 이 유틸리티들이 제공하는 정보의 상당 부분을 /proc 파일 시스템에서 똑같이
       얻을 수 있다. 결국 이 유틸리티들은 /proc 파일 시스템에 있는 정보를 사람이 읽기 편한
       형태로 제공해 주는 역할을 한다．

       PS 유틸리티는 현재 시스템에서 실행되고 있는 모든 프로세스의 목 록 을 출력해 준다. 하지만
       매우 유연한 구조를 갖고 있기 때문에 어떻게 설정하느냐에 따라서 현재 동작중인 시스템의
       상태 정보나 실행중인 프로세스에 대한 유용한 정보를 볼 수 있게 만들 수 있다. 예를 들어，
       PS를 이용해 각 프로세스의 스케줄 정책을 출력할 수 있는데, 특히 실시간 프로세스가 필요
       한 시스템에서 유용하게 사용될 수 있다．

       PS를 아무런 옵션 없이 실행하면 명령을 실행시킨 사용자 II）와 같은 사용자 ID를 갖는 프로
       세스 중에서 명령을 실행한 터미널을 사용하는 프로세스를 모두 출력해 준다. 이는 해당 사
       용자가 현재 터미널에서 실행시킨 프로세스가 많은 경우에 유용하게 사용할 수 있다．

       PS는 (POST)따 UNIX와 같은） 다양한 표준을 모두 지원하고 각기 다른 세 가지 스타일，
       즉 BSD. UNIX. GNU 스타일로 옵션을 줄 수 있기 때문에 혼란스러울 수도 있다. 일반적
       으로 BSD 스타일은 옵션이 하나 또는 몇 개의 문자로 되어 있고, 대시 (-）는 사용하지 않는
       다. 반면 UNIX 스타일은 친숙한 대시（-) 문자와 알파벳 문자들의 조합을 사용한다. 그리고
       GNU 스타일의 옵션은 대시 문자 두 개로 시작하는 긴 문자열을 이용한다. 자신이 사용하는
       PS에 대한 자세한 내용은 사용하는 시스템의 맨 페이지를 참고하도록 하자.

       PS를 사용하는 사람은 누구나 자신이 원하는 방식으로 PS를 실행시키겠지만, 그 중에서도
       가장 유용하게 사용되는 것은 ps aux이다. 이 명령은 시스템의 모든 프로세스를 보여 주는
       데 , ［리스트 13-9］는 임베디드 타깃 보드 상에서 이 명령을 실행한 결과를 나타낸 것이다．




I 求陋
                                                                                                                                                개발 도구       Chapter 13



      ［리스트 ]3-9] 프로세스 목록

        $ pa aux
        USER       PID %CPU %MEN          VSZ                                      RSS TTY                                   STAT    ST石RT    TIME COMMAND
                     l
        root         1  0. 0 0. 8        1416                                      508 ?                                     S       00: 00   0: 00 mllit [31




                                            0 0 0 0 0 0 0 0 0 0 0 0 0 8 0
                     八
                     石
        root         2  0. 0 0. 0           0                                                           0 ?                  S<      00:00    0: 00 (ksoftirqd/ 01




                                                                            0 0 0 0 0 0 0 0 0 0 0 0 4 0 6 6 0 4
                     n4V
        root         3  0. 0 0. 0           0                                                           0 ?                  S<      00: 00   0: 00 (desched/ 0)
                     4




                                                                                                                2  2 8
        root         4     0. 0   0. 0      0                                                          0 ?                   S<      00: 00   0: 00 (events/ 0]




                                                                                                                         2
                     5
        root         5     0. 0   0. 0      0                                                          0                     S<      00: 00   0: 00 [kheiperl
        root        10     0. 0   0. 0      0                                                          0                     5<      00: 00   0: 00 [kthread1
        root        21     0. 0   0. 0      0                                                          0                     S<      00: 00   0: 00 [kblockd/ 0]




                                                                                                    4
        root        62     0. 0   0. 0      0                                                          0                     S       00: 00   0: 00 [pdflush]




                                                                                                        9 5 0 8 7 3 4 7
        root        63     0. 0   0. 0      0                                                          0                     S       00:00    0:00 (pdflush]
        root        65     0. 0   0. 0      0                                                          0                     S<      00: 00   0: 00 [aio/ 0)
        root        36     0. 0   0. 0      0                                                          0                     S       00: 00   0: 00 [kapiud)
        root        64     0刀     0. 0      0                                                          0                     S       00: 00   0: 00 [kswapd0]




                                                                                                    4   5 4 7   3 7 3 7
        root       617     0. 0   0. 0      0                                        0                                       S       00:00    0: 00 [mtdblockd]
        root       638     0. 0   0. 0      0                                        0                                       S       00:00    0: 00 (rpciodl
        bin        834     0力     0. 7   1568                                      444                                       Ss      00: 00   0: 00 /sbinfportmap
        root       861     0. 0   0. 0      0                                        0                                       S       00: 00   0: 00 [lockdl




                                                                                                              V
                                                                                                              드 4上
        root       868     0. 0   0. 9   1488                                      596                                       Ss      00: 00   0: 00 lsbinlsyslogd -r
        root       876     0. 0   0. 7   1416                                      456                                       Ss      00: 00   0: 00 /sbin/ klogd -x
        root       884     0. 0   1. 1   1660                                700                                             Ss      00: 00   0: 00 /usr/ sbin/rpc. statd
        root       896     0. 0   0. 9   1668                                584                                             Ss      00: 00   0: 00 /usr/ sbin/ inetd
        root       909     0. 0   2. 2   2412                               1372                                             Ss-4-   00: 00   0: 00 -bash


                                                                                                                      4上
        telnetd    953     0. 3   1. 1   1736                                732 ?      S                                            05: 58   0: 00 in. telnetd
        root       954     0. 2   2.1    2384                               1348 pts/ 0 Ss                                           05: 58   0: 00 -bash
        root       960     0. 0   1. 2   2312                                772 pts/ 0 R+                                           05: 59   0: 00 ps aux




      위 명령은 PS를 이용해서 볼 수 있는 다양한 내용 중의 한 가지에 불과하다. 다음 항목에
      각 열에 해당하는 설명을 볼 수 있다．

         口 USER와 프로세스 ID(PID) 필드는 이름 자체로도 의미를 충분히 알 수 있다．

         口 윙CI七 필드는 프로세스가 시작해서 현재까지의 CPU 점유율을 백분율로 보여 준다. 그렇
               기 때문에 실제로 CPU 사용량이 절대로 100퍼센트까지 올라갈 수는 없다．

         口 윙NEM 필드는 전체 물리 메모리 용량에서 각 프로세스가 사용하고 있는 상주 메모리14）의
           크기를 백분율로 나타낸 것이다．

         口 VSZ는 프로세스의 가상 메모리의 크기를 킬로바이트 단위로 나타낸 것이다．




14) （역자주］ 상주 메모리는 현재 프로세스어］ 실제로 할딩되어 사용되는 메모리를 말힌다．



                                                                                                                                                                     407 1
 難 難.     Embedded Linux Primer




          口 RSS는 Resident Set Size의 약자로 프로세스가 사용하는 스왑15）되지 않는 물리 메모리
           . 의 양을 킬로바이트로 나타낸 것이다．

          [aTTY는 해당 프로세스를 제어하는 터미널을 나타낸다．


        이 예에서 볼 수 있는 대부분의 프로세스가 터미널과 연결되어 있지 않다. 그리고 ［리스트
        13-9］를 출력시키는 PS 명령어는 pts/ O 터미널 디바이스를 사용한다고 되어 있는데 , 이는
        텔넷을 통해서 실행된 것을 나타낸다．

        STAT 필드는 이 프로세스 상태를 조사하는 시점의 프로세스 상태를 나타내는데 , S 표시는
        프로세스가 슬립 모드（sleep mode）에 있다는 것을 의미한다. 슬립 상태는 입출력의 결과를
        기다리는 것과 같은 특정한 이벤트를 기다리는 상태이다. R은 프로세스가 실행 가능한 상태
        라는 표시이다（이 말은 스케줄러가 더 높은 우선순위를 갖는 프로세스가 기다리고 있지 않은
        경우에 제어권을 R 상태의 프로세스에게 자유롭게 넘겨 줄 수 있다는 의미이다）. 상태를 나
        타내는 문자 다음에 오는 부등호（() 문자는 이 프로세스가 더 높은 우선순위를 가지고 있음
        을 나타낸다16) .

        마치막 필드에는 명령에 이름이 표시된다. 그 중에서 괄호 안에 표시된 것들은 커널 쓰레드
        들이다. 이외에도 다른 심볼과 옵션을 사용할 수 있는데 완전한 설명은 맨 페이지를 참고하
        도록 하자．


]3.4.5 to口
        PS 명령은 실행한 그 순간의 시스템 상태만을 보여 주는 데 그치지만, 七OP은 주기적으로
        시스템과 프로세스의 상태를 보여 준다. PS와 비슷하게 t아） 역시도 상당히 많은 수의 옵션
        을 가지고 있다. top 명령은 설정을 통해서 자신이 원하는 정보만 표시되도록 커스터마이징
        해서 사용할 수 있다．

        아무런 옵션 없이 실행하면 현재 실행되고 있는 모든 프로세스를 ［리스트 13-9］에서 볼 수
        있는 PS aux 명령을 내린 결과와 비슷하게 출력해 준다. 그리고 매 3초마다 그 내용을 갱신
        해서 보여 준다. 물론 이런 갱신 주기와 같은 많은 옵션들을 자신이 원하는 대로 바꿔 쓸 수
        있다. top 화면에서 처음 몇 줄은 시스템 정보를 보여 주는데 , 이 정보 역시 3초마다 새롭게

15) （역자주） Swap : 가상 메모리에서 사용하지 않는 페이지를 하드디스크와 같은 저장 장소로 대피시키는 것을 스왑이라고 한다．
16) ［역자주） 추가적으로 소문자 S는 현재 세션의 리더를 나타내고 4는 젼위 프로세스（如reground process) 를 나타낸다．
                                                                                                                                                                                                                                                          개발 도구        Chapter 13



       갱신된다. 여기에는 시스템이 동작한 총 시간, 사용자 수, 현재 시스템에 있는 프로세스에
       대한 상태 정보 등의 다양한 항목이 포함된다．

       ［리스트 13-10］은 t아＞ 명령을 인자 없이 실행시켜서 기본 구성으로 표시되도록 한 것이다．

       ［리스트 13- 10] top 실행 결과


         top - 06: 23:14 up     6: 23,  2 users,    load average: 0. 00, 0. 00, 0. 00
         Tasks:    24 total,     1 running,    23 sleeping,     0 stopped,     0 zombie
         Cpu (s) :  0. 0毖 us,   0. 3毛 sy,  0. 0毛 ni, 99. 7毛 id,   0 . 0毛 Wa, 0 . 0毛 hi,   0. 0七 Si
         Mem:       62060k total,       17292k used,       44768k free,            0k buffers
         Swap:            0k total,          0k used,           0k free,      11840k cached




                                                                                                                         m가 K 0 0 0 0 0 0 0 0 0 0 0 0 0




                                                                      工0 0 0 0 5 5 5 5 0 0 5 0 0 0 0 0 0 0 0 0 0 0 0 0
                                                                                                                                                          覆
           p工D USER         PR                                                                                                                                                          sm之 S 象CPU 毛ME쪼匹                                                 T工N丑＋    COMM?'ND
           978 root         16                                                                                                                                                          780 R  0. 3 1. 5                                                0: 01. 22 t아）




                                                                                                                                                                                                S S S S S $ S S S S $ S S S S S S g S g
                                                                                                                                                          8 0 0 0 0 0 0 0 0 0 0 0 0 0
                                                                                                                                                                                            4
             1 root         16                                                                                                                                                                 0. 0 0. 8                                                0: 00. 47 mnl七
             2 roo亡          5                                                                                                                                                                 0. 0  0. 0         m
                                                                                                                                                                                                                                                        0: 00. 00 lcsOft ircjd/ 0
             3 roo亡          5                                                                                                                                                                 0. 0  0. 0         1
                                                                                                                                                                                                                                                        0: 00. 00 desche（刃 0
             4 I力ot          2                                                                                                                                                                 0. 0  0. 0                                               0: 00. 00 ever止8/ 0




                                                                                                                         1 9 4
                            -
             5 roc比         10                                                                                                                                                                 0. 0  0. 0                                               0: 00. 09 khelper




                                8 0 0 5 9 5 5 5 5 5 0 6 9 8 6 5 6 5
            10 root                                                                                                                                                                            0. 0  0. 0                                               0: 00. 00 kthread
            21 root                                                                                                                                                                            0. 0  0. 0                                               0: 00. 00 ｝口）lockd! 0




                                                                                                                                                          的
            62 root                                                                                                                                                                            0. 0  0. 0                                               0: 00. 00 pdf lush




                                                                           l l U 1 m m     1
                                                                                                                         V l l
            63 root                                                                                                                                                                            0. 0  0. 0                                               0: 00. 00 pdt끄.ish




                                                                      n
                                                                                                                                                                                                2 0 0 0 0 0 0 0 0 0 0 0 0 0 4 0 4 6
             65 root                                                                                                                                                                           0. 0  0. 0                                               0: 00, 00 aio/ 0
             36 roo乞                                                                                                                                                                           0. 0  0. 0                                               0: 00. 00 kapmd
             64 roo乞                                                                                                                                                                           0. 0  0. 0                                               0: 00. 00 kswapd0




                                l 2 2 l l 2 2 2 l l 2 l l l l l l l
            617 root                                                                                                                                                                           0. 0  0. 0                                               0: 00. 00 mtdblockd




                                                                                                                                                                                                                                0 9
                                                                                                                                                                                               0. 0  0. 0                                               0: 00.34 rpciod




                                                                                                                                                                                                5                           6
            638 root
                                                                                                                                                                                            a
                                                                                                                                                                                            d
            834 bin                                                                                                      1568                             444                                  0. 0 0. 7                                                0: 00. 00 portmap
            861 root                                                                                                        0                               0                                  0. 0  0. 0                                               0: 00. 00 lockd
                                                                                                                                                                                            口
                                                                                                                                                                                            d
            868 root                                                                                                     1488                             596                                  0. 0 1. 0                                                0: 00.11 syslogd
                                                                                                                                                                                        d
                                                                                                                                                                                        <   m
            876 root                                                                                                     1416  456                                                                                                        0. 0   0.7    0: 00. 00 klogd
            884 root                                                                                                     1660  700  612 S                                                                                                 0. 0   1, 1   0: 00. 02 rpc. statd
            896 root                                                                                                     1668  584  504 S                                                                                                 0. 0   0. 9   0: 00. 00 inetd
            909 root                                                                                                     2412 1372 1092 S                                                                                                 0. 0   2. 2   0: 00. 34 bash
            953 telnetd                                                                                                  1736  736  616 S                                                                                                 0. 0   1. 2   0: 00, 27 in. talnetd
            954 root                                                                                                     2384 1348 1096 S                                                                                                 0. 0   2. 2   0: 00.16 ba斛l




       ［리스트 13-10］에서 각 행에 출력되는 키본 항목은 PID, 사용자, 프로세스 우선순위 , 프로
       세스의 nice17) 값, 프로세스가 사용하는 가상 메모리 , 상주 메모리의 크기 , 태스크18）가 사
       용하는 공유 메모리의 총량이 있고, 그 외에 기타 필드는 앞의 PS 예제에서 설명한 것과 같은
       것들이다．

17) （역자주） 리눅스어P1 nice는 2羽］서 19까지의 값을 갖는데, 프로세스의 우선순위를 나타낸다． 음수로 갈수록 우선순위가 높아
 진다．
18) ［역자주） 프로세스와 같은 의미이다．



                                                                                                                                                                                                                                                                              409 1
   難U     Embedded Linux Primer



        이 유용한 유틸리티를 설명하기에는 할당된 지면이 너무 좁은 것이 아쉽다. 하지만 어느 정
        도 시간을 투자해서 top과 PS어］ 대한 맨 페이지를 살펴보고 다양한 기능에 대해서 알아두면
        큰 도움이 될 것이다．


13.4.6 mtrace
        mtrace 패키지는 자신의 어플리케이션에서 mallocQ, reallocQ, free () 함수를 호
        출하는 것을 분석해서 결과를 알려주는 간단한 툴이다. 사용하기 쉬운 툴이고, 사용자의 어
        플리케이션에서 발생하는 문제의 원인을 찾는 데 힌트를 줄 수도 있을 것이다. 지금까지 설
        명한 모든 툴과 마찬가지로 mtrace 패키지도 자신이 사용하는 아키텍처에 맞게 컴파일된
        것을 사용해야 한다. m亡race는 실제 명령을 내려서 실행시키는 프로그램은 아니고, 타깃
        시스템에 설치해서 malloc을 대체하는 라이브리리 파일이다. 독자의 어플리케이션에서 특
        별한 함수를 호출해서 mtrace 기능을 활성화시킬 수 있는데 이를 위해서 임베디드 리눅스
        배포 버전에 mtrace 패키지가 반드시 포함되어 있어야 한다.

        이 유틸리티를 실험해 보기 위해서 간단한 연결 리스트를 동적으로 생성하는 간단한 프로그
        램을 하나 작성해 보자. 리스트에 항목을 추가할 때마다 매 항목을 동적으로 생성하도록 하
        자. ［리스트 13-11］은 리스트를 위한 구조체를 청의하는 부분이다．

        ［리스트 ]3-11] 간단한 선혐 연결 리스트（Linear 니nked 니st)

           struct blists {
             struct bujst_s 士next;
             char *dataHitemS
             -mnt item_size;
             mnt index;
           };



        각 리스트 항목은 다음과 같이 malloc () 함수를 호출해서 생성하고, 리스트의 맨 뒤에 추
        가한다．

           struct blist_s 士p = malloc( sizeof (struct blist_s) );




I 410
                                                           개발 도구   Chapter 13




      리스트의 각 항목 내에 있는 가변 길이 데이터를 위해서도 메모리를 동적으로 할당해서 리스
      트의 맨 뒤에 넣기 전에 설정하도록 하자. 이런 식으로 리스트에 있는 모든 아이템을 두 번의
      malloc () 호출을 통해서 생성한다. 즉, 하나는 리스트 항목 자체를 위한 것이고, 나머지
      하나는 리스트 항목 내부에 있는 가변 길이 데이터를 위한 것이다. 이런 식으로 10,000개의
      항목을 갖도록 해서 총 20.000번의 malloc () 이 호출되도록 했다．

       mtrace를 사용하기 위해서는 다음 세 가지 조건을 만족해야 한다．

         口 혜더 파일 mcheck.h를 소스 파일에서 반드시 포함해햐 한다．

         口 핸들러를 등록하기 위해서 어플리케이션에서 mtrace (）를 반드시 호출해1 주어야 한다．
         口 추적된 내용을 기록하기 위해써 환경 변수 MJ\LLOC TRACE어］ 쓰기 가눙한 파일 이름을
             반드시 지정해1 주어야 한다．

      위 조건을 만족시키면 추적 대상이 되는 함수를 호출할 때마다 한 줄씩 MALLOC TRACE에
      지정된 파일에 키록되게 된다. 기록되는 데이터는 다음과 같은 형태로 되어 있다．

         c   ./mt_ex: [0x80486ec] + 0x804a5f8 0x10


      @ 표시는 추적한 내용에 주소와 함수 이름이 있음을 나타낸다. 이 예제에서 , 프로그램은 대
      괄호（[ ]) 안에 있는 주소 아娼0486ec에서 실행되고 있다. 바이너리 유틸리티나 디버거를
      이용하면 쉽게 이 주소값에 해당하는 함수를 찾아 낼 수 있다. 더하기 기호（+）는 메모리를
      할당하기 위한 함수를 호출한 것을 의미한다. 그래서 free () 함수는 빼기 기호(-）로 표시
      된다는 것도 짐작할 수 있다. 그리고 그 다음에 나오는 숫자는 할당되거나 해제되려는 메모
      리 주소이다. 그리고 마지막은 크기 정보인데 , 메모리를 할당할 메모리 크기를 나타낸다．

      위 데이터 형식은 사용자에게는 적합하지 않기 때문어］ mtrace는 이러한 가공되지 않은 추
      적 데이터와 불일치 지점에 대한 보고 메시지를 분석해 주는 유틸리티19）를 별도로 포함하고
      있다. 가장 간단한 경우로 Penl 스크립트가 ''Nom이nory leaks（메모리 누수 없음）"라는 메
      시지만 출력할 수도 있다. ［리스트 13-12］에는 메모리 누수가 발견되었을 때 어떤 내용이
      출력되는지를 보여 준다．




19) 이 분석을 위한 유틸리티는 mtrace 패키지에 포함되어 있고， 펄 스크립트로 작성되어 있다．


                                                                         411
  轟N     Embedded Linux Primer



       ［리스트 13-12] mtrace 에러 보고

          $ mtrace ./mt_ex mtrace.log

         Memory not freed:
            Address    引ze            caller
         0x0804aa70     0xOa     at   /home/chris/temp/mt_ex.c:64
         0x0804abc0     0xlO     at   /home/chris/temp/mt_ex.c: 26
         0x0804ac60     0x10     at   /home/chris/temp/mt_ex.c: 26
         0x0804acc8     0xOa     at   /home/chris/temp/mt_ex.c: 64



       보는 바와 같이 , 이 간단한 툴은 문제가 생기기 전에 그 부분을 미리 발견하거나, 문제가 생
       겼을 때도 마찬가지로 어디가 문제인지를 찾아낼 수 있게 도와준다. 주목할 부분은 이 Penl
       스크립트가 malloc () 을 호출했지만 할당된 메모리 주소에 대해서 그에 해당하는 free ()
       가 호출되지 않은 경우에 이 malloc () 이 호출된 파일 이름과 행 번호를 출력해 준다는 것이
       다. 하지만 이렇게 함수 이름까지 출력시키려면 실행 파일을 컴파일할 때 컴파일러에 -g 옵
       션을 줘서 디버깅 정보를 포함하도록 만들어야 한다. 만약에 디버깅 정보가 실행 파일에 없
       을 경우에는 단순히 malloc () 을 호출한 코드의 주소를 보여 준다．


13.4.7 dmalloc
       dm缸b>c은 mtrace7} 하치 못하는 부분을 보충하는 툴이다. m七race 패키지가 간단하고
       프로그램을 방해하지 않으면서 mallo可free의 불일치 상황을 감지할 수 있는 툴이라면
       dmalloc 패키지는 훨씬 더 폭넓은 동적 메모리 관리 에러 상황을 감지할 수 있다. mtrace
       와 비교하면 dmalboc은 프로그램의 동작에 더 큰 영향을 미친다. dmablc兀을 어떻게 설정
       하느냐에 따라서 어플리케이션이 기어가는 것처럼 느려질 수도 있다. 이 툴은 경쟁 조건
       (race condition）이나 기타 타이밍 문제로 인한 메모리 오류가 의심되는 상황에서는 절대
       도움이 안 된다. 왜냐하면 山nalboc（그리고 mtrace는 좀 덜하다）으로 인해서 어플리케이
       션의 타이밍이 완전히 바뀌기 때문이다．

       dmabboc은 아주 강력한 동적 메모리 관리 도구이고, 세밀하게 설정을 제어할 수 있다. 그래
       서 어떤 면에서는 복잡하게 느껴질 수도 있다. 이 툴을 배우고 익혀서 완전히 자기 것으로
       만드는 데는 시간이 좀 걸릴 것이다. QA(Quality Assurance : 품질 보증）를 위해서 버그
       를 찾아내는 경우라면 이 툴이 가장 쓸 만한 툴 중에 하나가 될 것이다．


1412
                                                      개발 도구     Chapter 13



山nailoc은 mailoc 라이브러리를 대체하는 디버킹용 라이브러리이다. dmaiioc올 사용하
려면 다음 조건이 갖춰져야 한다．

  口 어플리케이션 코드에서 dmaiioc.h 해더 파일을 반드시 포함시켜야 한다．

  口 어플리케이션을 링크시킬 때 dinailoc 라이브러리를 이용해서 링크시켜야 한다．

  口 임베디드 타깃 시스템에 dmaiioc 라이브러리와 유틸리티가 반드시 설치되어 있어야
    한다．

  口 어플리케이션을 실행시키기 전에 dmail（그C 라이브러리가 참조하는 환경 변수돌을 정의
    해 주어야 한다．

꼭 필요한 것은 아니지만, 어플리케이션 코드에서도 dmaiioc . h를 포함하도록 해야 한다．
이렇게 하면 결과를 출력할 때 파일 이름과 행 번호 정보도 포함해서 출력되기 때문이다．

이제 자신이 선택한 dmaiioc 라이브러리를 자신의 어플리케이션에 링크하도록 하자．
dmaiioc 패키지는 패키지를 구성할 때 선택하는 내용에 따라서 몇 가치 다른 라이브러리를
만들도록 할 수 있다. 다음 예에서는 iibdmalioc. so 공유 라이브러리 오브젝트를 사용할
것이다. 이 파일을 컴파일러가 라이브러리를 찾는 경로 인에 두도록（또는 심볼릭 링크를 만
들도록） 하자. 어플리케이션을 컴파일하기 위한 명령은 다음과 같은 형태가 된다．



  $ ppc 82xx-gcc -g -닙all -o mtest_ex -L. ./dmalloc- S.4.2/ \
      idnialloc mtest_ex .c



이 명령은 dmalioc 라이브러리（iibdinaiioc. s이가 명령에서 -I』옵션에 있는 위치 , 즉
현재 디렉터리의 바로 상위에 있는 디렉터리인 . .／山Tialioc巧 . 4. 2어］ 라이브러리 파일이
있다고 가정한 것이다．

dmailoc 라이브러리를 타깃 시스템에 설치하기 위해서는 자신이 원하는 위치（아마
/usr/iocal/iib）에 라이브러리 파일을 두도록 한다. 그리고 시스템 구성을 통해서 이 라
이브러리를 검색하도록 만들어 준다. 여기서 예로 든 PowerPC 시스템의 경우에는
/e七c/id. so. conf 파일에 /usr/iocai/iib 디렉터리를 추가하고, idconfig 유틸리
티를 실행해서 라이브러리 검색 캐시를 새로 만들어 주는 식으로 설정했다．


                                                                     413 1
         Embedded Linux Primer




       마지막 준비 단꼐는 dmalloc 라이브러리가 디버깅 단계를 결정하는 데 필요한 환경 변수
       값을 설정하는 일이다. 환경 변수 중에는 여러 개의 옵션을 편리하게 하나의 숫자로 표현하
       기 위해서 디버그 비트 마스크20) (bit mask）를 사용한다. 우리의 경우에 환경 변수는 다음
       과 같을 것이다．

         DMALLOC_OPTIONS=debug=0x4f4ed03 , i nter=100, log=dmalloc. log


       여기서 debug가 디버그 단계를 정의하는 비트 마스크이다. 그리고 inter는 dnialloc 라이
       브리리에서 포괄적으로 자체 검사 및 힙（heap) 상태를 검사하는 주기를 결정한다. 그리고
       dmailoo의 로그 출력 내용이 log 변수에 정해진 파일에 기록된다．

       dmalbOc 패키지에는 DMALLOC OPTIONS 환경 변수를 만들어 주는 유틸리티가 포함되어
       있는데 , 유틸리티에 전달한 인자를 통해서 환경 변수 값을 만들어 준다. 위에 나온 예제는
       다음 dmallc兀 명령을 통해서 만든 것이다. drnabboc 패키지 문서를 보면 이 부분에 대해서
       상세한 정보를 볼 수 있기 때문에 따로 설명하치는 않겠다．

         $ dmalloc -p check-fence -1 dmalloc.log -i 100 high


       이 단계까치 완료하면 어플리케이션을 dinallc兀 디버그 라이브러리를 이용해서 실행할 수
       있게 된다．

       dinalboc은 아주 상세한 로그를 출력하는데 , ［리스트 13-13］은 의도적으로 메모리 누수를
       만드는 예제 프로그램을 실행시켰을 때 drnalboc이 출력하는 내용을 일부 나타낸 것이다．

       ［리스트 ]3-13) dmabboc 로그 출력


          2592: 4002: Dmalloc version '5. 4. 2 ' from 'http: //dmalloc. com/ '
          2592: 4002: flags = 0x4f4e503, logfile 'dmalloc.log '
          2592: 4002: interval = 100, addr = 0, seen # = 0, limit = 0
          2592: 4002: starting time = 2592
          2592: 4002: process pid = 442
          2592: 4002: Dumping Chunk Statistics:
          2592: 4002: basic-block 4096 bytes, alignment 8 bytes
          2592: 4002: heap address range: 0x30015000 to 0x3004f000, 237568 bytes
          2592: 4002:     user blocks: 18 blocks, 73652 bytes (38%)


2이 C역자주） 비트 하나하나를 정보로 이용하는 방법이다. 즉, 8비트 숫자는 8개의 옵션을 선택할 수 있다. 예를 들어, 呱03의 경
   우 0. 1 비트만 l로 선택되고 나머지는 0이다．


 414
                                                          개발 도구     Chapter 13



  2592: 4002:    admin blocks: 29 blocks, 118784 bytes (61%)
  2592: 4002:    total blocks: 47 blocks, 192512 bytes
  2592: 4002: heap checked 41
  2592: 4002: alloc calls: malloc 2003, calloc 0, realloc 0, free 1999
  2592: 4002: alloc calls: recalloc 0, memalign 0, valloc 0
  2592: 4002: alloc calls: new 0, delete 0
  2592: 4002: current memory in use: 52 bytes (4 pnts)
  2592: 4002: total memory allocated: 27546 bytes (2003 pnts)
  2592: 4002: max in use at one time: 27546 bytes (2003 pnts)
  2592: 4002: max alloced with 1 call: 376 bytes
  2592: 4002: max unused memory space: 37542 bytes (57%)
  2592: 4002: top 10 allocations:
  2592: 4002: total- size count in-use-size count source
  2592: 4002:       16000 1000          32        2 mtest_ex. c: 36
  2592: 4002:       10890 1000          20        2 mtest_ex. c: 74
  2592: 4002:         256     1         0        0 mtest_ex.c:154
  2592: 4002:       27146 2001          52        4 Total of 3
  2592: 4002: Dumping Not- Freed Pointers changed Since start:
  2592: 4002: not freed: '0x300204e8151' (10 bytes) from 'mtest_ex. c: 74 '
  2592: 4002: not freed: '0x300205881s1' (16 bytes) from 'mtest.ex. c: 36 '
  2592: 4002: not freed: '0x300206881s1' (16 bytes) from 'mtest_ex. c: 36 '
  2592: 4002: not freed: '0x300208a8151' (10 bytes) from 'mtest_ex. c: 74 '
  2592: 4002: total-size count source
  2592: 4002:          32     2 mtest+ex. c: 36
  2592: 4002:          20     2 mtest.-ex. c: 74
  2592: 4002:          52     4 Total of 2
  2592: 4002: ending time = 2592, elapsed since start = 0:00: 00



중요한 것은 이 로그가 프로그램이 종료될 때 출력된다는 점이다（drnalloc에는 많은 옵션이
있고 여리 동작 모드가 있다. 그래서 에러가 감지될 때마다 결과를 출력하게 설정할 수도
있다）.

출력되는 내용의 처음 절반은 어플리케이션의 전체적인 메모리 사용과 힙 사용에 대한 통계
를 보여 준다. 그리고 malloc 라이브러리 호출, 즉 mallocQ, freeQ, realloc () 이
각각 몇 번 호출되었는지를 보여 준다. 재미있는 것은 로그 내용에 기본적으로 최상위 10개
의 할당 호출에 대해서 그 소스 코드 위치와 어느 행에서 호출했는지를 알려주게 되어 있다는
것이다. 이 정보는 시스템 레벨에서 프로파일링을 진행할 때 아주 유용하게 사용될 수 있다．




                                                                          4佰 I
         Embedded Linux Primer




       로그의 뒤편으로 가게 되면 어플리케이션에서 메모리 누수가 있다는 증거를 볼 수 있다．
       dmalloc 라이브러리가 메모리를 할당하고 해제하지 않은 것이 분명한 네 가치 경우를 감지
       해 낸 것을 볼 수 있다. 예제에서 dmalloc . h를 포함시키고, 빌드할 때 디버깅 심볼도 포함
       하도록 했기 때문에 , 메모리가 할당된 위치를 로그 내용에서 볼 수 있다．

       이 장에서 소개하는 다른 툴들과 마찬가지로 지면상 이 강력한 툴에 대해서도 간략한 소개만
       하고 넘어가야 하겠다. 山Tialloc은 이외의 다양한 조건 및 한계 지점에 대해서도 감지할 수
       있다. 예를 들어 , 이미 해제（free）된 메모리에 대해서 쓰려는 동작을 할 경우도 감지할 수
       있다. 그리고 포인터를 이용해서 할당된 범위（boundary）를 넘어가서 접근할 경우도 찾아낼
       수 있다. 사실 dmalloc은 malloc 계열 함수를 이용해서 하는 모든 메모리 관련 작업을
       거의 대부분 로그로 남기도록 할 수 있다. drnalloc은 비록 능숙하게 다루기까지는 시간이
       걸리더라도 충분히 시간을 투자해도 좋을 만큼 강력한 툴이다．


13.4.8 커널 웁스（0ops21) )
       커널 웁스는 엄밀하게 말하면 툴은 아니지만 커널 웁스가 출력하는 내용은 문제를 해결하는
       데 유용한 정보를 많이 포함하고 있다. 커널 웁스는 다양한 커널 에러 상황에서 생기는데，
       간단히는 프로세스 때문에 생긴 메모리 에러에서부터（대부분의 경우 복구 가능함）, 심각한
       커널 패닉까지 원인이 다양하다. 최신 리눅스 커널은 기존 16진수 주소 값들만 출력되던 것
       에서 심볼 관련 정보도 추가로 출력해 준다. ［리스트 나14］에서 PowerPC 타깃에서 커널
       웁스가 생긴 경우를 볼 수 있다．

       ［리스트 ]3-14] 커널 웁스


         $ modprobe loop
         Oops: kernel access of bad area, sig: 11 [#1]
         NIP: C000D058 LR: C0085650 SP: C7787E80 REGS: c7787dd0 TRAP: 0300 Not tainted
         MSR: 00009032 EE: 1 PR: 0 FP: 0 ME: 1 IR/DR: 11
         DAR: 00000000, DSISR: 22000000
         TASK = c7d187b0{ 323] 'modprobe ' THREAD: c7786000
         Last syscall : 128
         GPROO: 0000006c c7787E80 c7D187B0 00000000 C7CD2SCC FFFFFFFF 00000000 80808081
         GPR08: 00000001 C034AD80 C036D41C C034AD80 C0335AB0 1001E3C0 00000000 00000000
         GPR16: 00000000 00000000 00000000 100170DB 100013E0 C9040000 C903DFD8 c9040000


21) （역자주） 웁스1 말 그대로 놀리거나 당황스러운 경우에 쓰는 감탄사


I 引6
                                                                                          개발 도구   Chapter 13



          GPR24: 00000000 c9040000 c9040000 00000940 C778A000 C7CD25CO C7CD25CO C7CD25CC
          NIP [c000d058] strcpy+oxlO/oxlc
          LR [c0085650] register_disk+oxec/oxfO
          Call trace:
           [c00e170c] add_di sk+0x58/0x74
           [c90061e0] loop_ i ni t+0x1e0/0x430 [loop]
           [c002fc90] sys_i ni t_modul e+Oxlf4/0x2e0
           [c00040a0] ret_f rom_syscall+0x0/0x44
          segmentation fault



레지스터 덤프와 함께 레지스터 내용이 심볼 관련 내용을 갖고 있을 경우에 심볼 정보도 같이
출력된 것을 알 수 있다. 이리한 심볼 관련 정보를 이용하기 위해서는 먼저 커널을 구성할
때 KPLLSYSMS 옵션을 활성화시켜야 한다. ［그림 13-4］에서는 주 메뉴에서 "General
S毗up（일반 설정）" 다음에 있는 구성 옵션을 볼 수 있다．

        E加 臼tions     姓d口

         勿 區身 目              I     II    甘      四        中
        Ba毖 山ad Save Si:닙e SF小I F:川 Collapse Expand

        Opti며11                                                            Name              iA

         口 Jc“哺甲re sta恤出岫恤11心（佃帥如如m돠                                       EMBEDDED          1
          ' 口少岫1symlxs for ‘如b‘川q'flfi朴「YntoG"口5                           KA比“SYM"S         立
              느Inc他de쾨1symbds in k켜Isyms                                   KALLSYMSJLL       I
:               匕J［沁an extra k崩놈yms 口ass                                   KA나SYMS尸EXTRA_PAS!:
'4                                             '力1                                堪磊羅3轟斜孰客町니
    f    Load all symb미S佃debuggl碌／It奴yrnee朴KAItSY柚S

         Say Y here to let 甘甲 kern머 pnrit out symbol妃 口a尉tin向rm餉an and
         symbolic stack backtraces. This increases the size of the ker比l
         5아ire毗吼 as all symbols have to be 佃aded into 由e kernel in但ge.


I 그림 13-4 웁스에서 심볼을 사용할 수 있도록 하는 옵션


커널 웁스가 출력하는 대부분의 정보는 프로세서와 직접적으로 관련 있는 것들이다. 당연히
커널 웁스 메시지를 온전히 이해하기 위해서는 사용하는 아키텍처에 대한 지식이 있어야
한다．

［리스트 13-14］에 있는 웁스를 분석해 보면 웁스가 "커널이 잘못된 영역에 접근함, 시그
널：11(kernel access of bad area, sig: 11)" 때문에 발생한 것을 볼 수 있다. 이미 이전
예제를 통해서 시그널 11이 세그먼테이션 폴트인 것을 알고 있을 것이다．




                                                                                                       417 1
       群     Embedded Linux Primer




           출력된 맨 처음 단락은 커널 웁스가 발쟁한 이유를 간단히 정리해서 출력하고, 그 다음에 중
           요한 포인터들과 문제가 되는 태스크를 보여 준다. ［리스트 13-14］에서 NIP는 다음에 실행
           할 명령에 주소를 가리키고, 웁스 메시지의 뒷부분에서 디코딩한 정보도 보여 준다. 이 부분
           이 커널 웁스가 발생한 원인 코드이다. LR22）은 PowerPC 레지스터인데 현재 실행중인 서
           브루틴23）이 실행을 마치고 되돌아 갈 주소를 가리킨다. sP는 스택 포인터를 나타낸다．
           REGS는 레지스터가 덤프된 데이터를 저장하고 있는 자료 구조를 가리키는 커널 주소이다．
           그리고 TRAP은 이번 웁스 메시지와 연관된 예외（exception）의 종류를 가리킨다. 13.7.1절
           의 "더 읽어 보기"에 나와있는 PowerPC 아키텍처 참고 매뉴얼을 보면 TRAP 0300이
           PowerPC 데이터 저장 인터럽트이며 , 메모리를 잘못 접근했을 때 발생한다는 것을 알 수
           있다．

           웁스 메시지의 세 번째 줄은 Powerl毛의 추가적인 레지스터를 볼 수 있다. 예를 들어，
           MSR（머신 상태 레지스터） 값과 이 레지스터의 각 비트를 디코딩한 내용도 출력된다. 다음
           줄에서는 DAR(Data Access Register : 데이터 접근 레지스터）이 나오는데 , 보통 문제가
           되는 메모리 주소를 담고 있다. DSISR 레지스터는 PowerPC 아키텍처 참고 문서를 이용해
           서 그 내용을 분석해 보면 해당 예외에 대한 자세한 정보를 찾을 수 있다．

           웁스 메시지에는 태스크 포인터와 디코딩된 태스크 이름이 포함되어 있어서 웁스가 발생한
           시점에 어떤 태스크 또는 쓰레드가 실행되고 있었는지를 바로 알 수 있다. 그리고 프로세서
           레지스터를 자세히 덤프한 내용을 볼 수 있어서 추가적인 단서를 찾는 데 이용할 수 있다．
           다시 한 번 강조하지만 레지스터 값을 이용해서 의미 있는 단서를 읽어내기 위해서는 아키텍
           처와 컴파일러가 레지스터를 사용하는 구조에 대해서 어느 정도 지식을 갖고 있어야 한다．
           예를 들어 , PowerPC 아키텍처는 C 함수의 반환 값을 저장하기 위해서 r3 레지스터를 이용
           한다는 등의 정보 말이다.

           웁스 메시지의 마지막 부분은 스택을 역으로 거슬러 올라가는 호출 단계를 보여 주는데 , 커
           널이 심볼 정보를 사용할 수 있는 경우에는 심볼 이름도 같이 표시된다. 이 정보를 이용하면
           문제가 되는 상황이 어떤 순차적인 과정을 통해서 발생했는지를 볼 수 있다．




22) ［역7；녀勻 Link Re節ster0］다．
23) （역자주） 함수와 같은 의미이다．


14怡
                                                개발 도구   Chapter 13




     이 간단한 예제를 이용해서 웁스 메시지에서 얼마나 많은 정보를 얻을 수 있는지를 알아보았
     다. 분석 결과, 이 메시지가 PowerPC의 데이터 저장 예외였고, （명령어를 메모리에서 가져
     올 때 발생하는 문제와는 대조적으로） 데이터 메모리를 접근하는 주소에 문제가 있어서 발생
     한 것임을 알 수 있었다. DAR 레지스터는 예외를 일으킨 데이터 메모리 주소가 0x0000
     0000임을 알려준다. 그리고 modpr야氾라는 프로세스가 실행되면서 에러가 발생한 것도 알
     수 있다. 스택 역추적과 NIP（다음 명령에 포인터）를 통해서 문제가 되는 strcpy () 함수를
     호출한 곳이 m야如robe가 커널에 삽입하려고 했던 loop.k(> 모듈의 loop init () 이라는
     것을 알 수 있다. 이 정보를 이용해서 소스 코드에서 문제의 널 포인터에 쓰려고 하는 부분을
     쉽게 찾아낼 수 있을 것이다.



13.5 바이너리 유틸리E]
     바이너리 유틸리티 또는 binu七ils는 어떤 툴 체인에 있어서도 아주 중요한 요소다 사실
     컴파일러를 빌드하기 위해서도 먼저 binutils가 성공적으로 빌드되어 있어야 한다. 이 섹
     션에서는 임베디드 개발자가 알아 두면 좋을 만한 유용한 툴을 간락히 소개하도록 하겠다．
     이 장에서 소캐하는 모든 툴은 모두 독자가 사용하는 개발 시스템에서 실행되지만, 타깃 아
     키텍처를 위한 바이너리 파일을 대상으로 동작한다. 다른 방법으로 이 유틸리티들을 바로 타
     깃 시스템에서 실행시키도록 만들 수도 있지만 여기서는 교차e개발 환경을 가정하고 설명하
     도록 할 것이다．


13.5.1 reade什
     readeif는 타깃 ELF 바이너리 파일의 내부 구성을 검사하는 유틸리티이다. 이 툴은 특히
     ROM이나 플래시 메모리를 대상으로 한 이미지를 만들 때 , 즉 이미지의 내부 배치를 제어하
     는 것이 특히 중요할 때 유용하다. 또한 툴 체인이 어떻게 이미지를 만들어 내는지 , ELF
     파일 형식의 내부가 어떻게 구성되는지도 배울 수 있다．

     예를 들어 , ELF 이미치의 심볼 테이블을 출력하려면 다음 명령을 이용한다．

       S readeif -s <elf-image>




                                                              4四 I
   難.     Embedded Linux Primer




         ELF 이미지에 있는 섹션 정보를 출력하려면 다음 명령을 이용하면 된다．

          $ reade卄 -e <elf나image>


        中S 플래그를 사용하면 ELF 이미지에 있는 섹션 헤더를 모두 출력한다. 아마 간단한 7줄짜
        리 "hello world" 프로그램도 38개 되는 섹션 헤더를 가지고 있다는 것을 보면 놀랄 것이다．
        그중 일부는 친숙한 이름도 있는데 , 예를 들어 , . text 그리고 . data 섹션 등이 있다. ［리스
        트 13-15］에는 "hello world" 예제에서 섹션 헤더 리스트를 출력한 내용의 일부이다. 간단
        하게 하기 위해서 친숙한 헤더와 임베디드 개발자에게 관련된 헤더만 표시하고 나머지는 생
        략했다．

        ［리스트 ]3-15) readeif로 읽은 섹션 헤더


          $ ppc_82xx- reade卄 -s hello-ex
          There are 38 section headers, starting at offset 0x32f4:

          Section Headers:
          [Nr] Name      Type          Addr     off   Size   ES Fig   Lk inf Al

           [11] .text         PROGBITS 100002f0 0002f0 000568 00 AX   0   0   4

           [13) .rodata       PROGBITS 10000878 000878 00006800   A   0   0   4

           [15] .data         PROGBITS 100108e0 0008e0 00000c 00 WA   0   0   4

           [22] .sdata        PROGBITS 100109e0 0009e0 0000lc 00 WA   0   0   4
           [23] .sbss         NOBITS   lOol09fc 0009fc 000000 00 WA   0   0   1

           [25] .bss          NOBITS   10010a74 0009fc 0000lc 00 WA   0   0   4




        . text 섹션에는 실행시킬 프로그램 코드가 포함되고 . rodata 섹션에는 프로그램을 위한
        상수 데이터가 저장된다. 그리고 . data 섹션에는 초기화된 전역 변수가 저장되는데 , C 라이
        브러리의 시작 코드를 위한 전역 변수와 어플리케이션에서 사용하는 초기화된 전역 변수들이
        모두 여기에 모인다. . sdata 섹션은 더 작은 초기화된 전역 변수 데이터를 위해서 사용되는
        데 , 일부 아키텍처에서만 사용된다. 일부 프로세서 아키텍처는 메모리 영역에 대한 속성을
        알고 있는 경우에 그에 맞게 접근을 최적화할 수 있는데 . sda七a와 .sbs s 섹션이 이 최적화

蛋 420
                                                             개발 도구     Chapter 13



    를 가능하게 한다. .bss와 .sbss 섹션에는 프로그램의 초기화되지 않은 데이터들이 포함된
    다. 이 섹션들은 실제 프로그램 이미지에 공간을 차지하지는 않는다. 이 메모리 영역은 C
    라이브러리에 있는 초기화 코드가 알아서 0으로 초기화해 주기 때문이다．

    어떤 섹션이든 내용을 출력해 볼 수 있다. 다음 코드를 C 프로그램의 함수 바깥 부분에 선언
    해서 이 데이터가 . rodata에 어떻게 위치하는지 실험해 볼 수 있다．

      char *helloHrodata = "This is a read-only data string\n";


    readeif 명령어에 ［리스트 13-15］에서 덤프하고 싶은 섹션 번호를 지정해 주면 그 내용을
    볼 수 있다．



     $ ppc_82xx-readelf -x 13 hello- ex
     Hex di끄up of sac七1（끄l ' .roda七a ' :
       0x10000878 100189e0 10000488 1000050c 1000058c
       0x10000888 00020001 54686973 20697320 61207265 . . . .This is a read-
       0x10000898 61642d6f 6e6c7920 64617461 20737472 only data string
       0x100008a8 696e670a 00000000 54686973 20697320         This is
       0x100008b8 73746174 69632064 6174610a 00000000 static data
       0x100008c8 48656c6c 6f20456d 62656464 65640a00 Hello En由edded.
       0x100008d8 25730a00 25780a00                       %s. .%x. .




    위 내용을 보면 예제에서 선언한 초기화된 전역 변수와 프로그램에서 정의한 상수 문자열들
    이 . roda七a 섹션에 있는 것을 볼 수 있다．


13.5.2 reade什률 이용해써 디버깅 정보 보기
    readeif 명령어의 다른 유용한 기능으로 ELF 파일에 포함된 디버깅 정보를 출력해 볼 수
    있는 기능이 있다 프로그램을 빌드할 때 컴파일러에 -g 옵션을 준 경우에는 생성된 ELF
    파일에 일련의 디버깅 정보 섹션이 포함되도록 되어 있다. 다음 readeif 명령을 이용해서
    ELF 파일에 있는 디버킹 관련 섹션 헤더만 출력해 볼 수 있다．




                                                                            421 1
        Embedded Linux Primer




       $ ppc-linu卜read. lf -s ex 町nc 1 greP debi工g
                                                                                                   0 0
                                                                                                                   8




                                                                             0 0 0 0 0 0 0
         [28] .debug_aranges    PROGBITS  00000000      000c38 0000b8   00



                                                                                                         l
                                                                                                         4 l n l
                                                                                                               d
                                                                                                           a l
         [29] .debug그沁bnames    PROGBITS  00000000      000cf0 00007a   00




                                                                                                 n U
                                                                                                   八 V
         [301 .debug_info       PROGBITS  00000000      000d6a 00079b00



                                                                                             n U
                                                                                             U n U
                                                                                                     n
         [31) .debug_abbrev     PROGBITS  00000000      001505 00020700
          [32)   .debug_line      PROOBITS    00000000 00170c 000354 00
                                                                                                                   4
          [33)   .debug_ frame    PROGBITS    00000000 001a60 000080 00
                                                                                                            l
                                                                                                            月
          [34]   .debug_str       PROGBITS    00000000 001ae0 00014d 00




      readeif어］ --debug-dump 옵션을 주어 .debug 士로 시작하는 섹션 중에서 원하는 섹션
      의 내용을 출력해 볼 수 있다. 이 디버그 섹션에 있는 정보는 14장, "커널 디버깅 기술'에서
      컴파일러가 최척화시킨 커널 코드들을 디버킹하는 문제를 다룰 때 유용하게 쓰이는 것을 볼
      수 있을 것이다．

      디버깅 정보는 아주 클 수도 있는데 , 리눅스 커널 ELF 파일인 vmlinux 파일에 있는 디버깅
      정보를 모두 출력시키면 600만 줄 이상이 될 것이다. 출력된 디버깅 정보는 쉽게 다가갈 수
      있는 내용은 아니지만, 최소한 어느 정도 익숙하게 볼 수 있게 된다면 좀 더 나은 임베디드
      엔지니어가 될 수 있다．

      ［리스트 仔16］은 작은 예제 어플리케이션에서 .debug info 섹션의 내용을 출력한 것을
      나타낸 것인데 , 공간상 일부분만 나타냈다．

      ［리스트 ]3-16) 디버그 정보 덤프의 일부


        S ppc-linux- readelf -debug-dump=info ex_sync
        1 The section .debug小info contains:
        2
         2
         J
             Compilation unit @ 0:
         4
              Length:        109
         <
         J
              version:       2
         戶
         b
              Abbrev offset: 0
         =
         /
              Pointer Size: 4
         8
            <0><b> : Abbrev Number: 1 (Dw_TAG_compi 1e_uni t)
         O
         J
         0
               DW_AT_stmt_l i St       :  0
         m
         l
                 OW_AT_i ow_pc          : 0x10000 368
         4
         l   L  D나AT_high니：)C          : 0x 100003 8c
         l ／
           八
         m dl    D닙_AT_name
        . ./sysdeps/powerpc/powerpc32/ elf/ start. S


422
                                                                         개발 도구    Chapter 13



            13      DW_AT_comp_di r         : /var/tmp/BUILD/glibc-2 .3. 3/csu
            14      D늬叫AT_producer          : GNU AS 乙15. 94
            15      DW_AT_language          : 32769 (MIPS assembler)

            394 <1><sal> : Abbrev Number : 14 (Dw_TAG_subprogram)
            395    DW_AT_sibling         : <5fa>
            396    DW_AT_external        : 1
            397    0W_AT_name            : main
            398    DW_AT_decl_file       : 1
            399    DW_AT_decl_line       : 9
            400    D吐AT_아ototyped        : 1
            401    DW_AT_type            : <248>
            402    0W_AT_i o叫_pc         : 0x100004b8
            403    DW_AT_high_pc         : 0x10000570
            404    0W_AT_frame_base      : 1 byte block: 6f     (Dw_oP_reg3l)

            423 <2><5e9>: Abbrev Number : 16 (Dw_TAG_variable)
            424    DW_AT_name           : mybuf
            425    0吐AT_d吼］_file        : 1
            426    DW_AT_decl_line      : 11
            427    0W_AT_type           : <600>
            428    DW_AT_location       : 2 byte block: 91 20         (Dw_oP_fbreg: 32)




        Dwarf 224) 태그 DW TAG compile uni七로 구별할 수 있는 첫 번째 레코드는 Po毗叩C 실
        행 파일에서 맨 첫 번째로 컴파일되어서 포함된 부분을 의미한다. 이 파일은 S七art. S인데
        일반 C 프로그램의 최초 시작을 담당하는 코드이다. 다음 레코드는 DW TAG subprogram
        인데 사용자 프로그램의 시작을 나타내는 익숙한 함수 main () 이다. 이 I如arf2 디버그 레
        코드에는 main () 함수가 위치한 파일과 줄 번호도 포함되어 있는데 , ［리스트 13-16］의 맨
        마치막에 있는 레코드는 main () 루틴에 안에 있는 지역 변수 mybuf를 보여 준다. 다시 말
        하면 파일 이름과 줄 번호가 레코드에 포함되기 때문에 이 정보를 이용해서 main () 함수가
        9번째 줄에 있다는 것과 mybuf7} 소스 코드의 11번째 줄에서 선언되는 것을 알 수 있다．
        ELF 파일에 있는 다른 디버깅 레코드는 Dwar巴의 DW AT decl file 속성으로 파일 이
        름을 유추할 수 있다．




24) 이 장의 뒤편에 D\＼게寸2 디버그 정보 명세서 (Debug Inf아nation SI玭寸ication) 가 참고 자료로 나와 있다．



                                                                                      4231
  難1   Embedded Linux Primer



     이 장의 맨 뒤편에 있는 13.7.1절 "더 읽어 보기"에 있는 참고 자료를 통해서 Dw町12 디버
     깅 정보 형식에 대한 자세한 내용을 찾아볼 수 있을 것이다．


13.5.3 objdump
     obj dumr) 유틸리티는 readeif 툴과 상당 부분 기능이 중복된다. 하치만 obj duinp7} 할 수
     있는 더 유용한 기능은 오브젝트 코드를 역어셈블해서 출력할 수 있다는 것이다. ［리스트
     13-17］을 보면 간단한 "hello world"의 PowerPC 버전의 . text 섹션을 역어셈블한 예제가
     나와 있다. 공간상 main () 루틴에 해당하는 부분만 나타냈다. 전체 덤프는 C 라이브리리의
     시작 코드와 종료 코드도 포함되기 때문에 여리 페이지를 차지한다．

    ［리스트 ]3-17) objc加m口릍 이용한 역 어셈블（disassem비e)


       $ ppc_82xx-objdump -s -m powerpc:common -j .text hello

       10000488 <main>:
       10000488:      94 21 ff e0   stwu    rl, -32 (rl)
       1000048c:      7c 08 02 a6   mflr     r0
       10000490:      93 el 00 lc   stw     r31, 28(rl)
       10000494:      90 01 00 24   stw     r0, 36(rl)
       10000498:      7c 3f Ob 78   mr      r31, rl
       1000049c:      90 7f 00 08   stw     r3, 8(r31)
       100004a0:      90 9f 00 0c   stw     r4,12 (r31)
       100004a4:      3d 20 10 00   Us      r9, 4096
       100004a8:      38 69 08 54   addi    r3, r9, 2132
       100004ac:      4c c6 31 82   crclr    4*"crl+eq
       100004b0:      48 01 05 11   bi      100109c0

       <_bss_start+0x60>
       100004b4:     38 00 00 00    ii      r0,0
       100004b8:     7c 03 03 78    mr      r3, r0
       100004bc:     81 61 00 00    lwz     rll, 0(rl)
       100004c0:     80 0b 00 04    lwz     r0, 4(rll)
       100004c4:     7c 08 03 a6    mtlr    r0
       100004c8:     83 eb ff fc    lwz     r31, -4(rll)
       100004cc:     7d 61 5b 78    mr      rl, rll
       100004d0:     4e 80 00 20    b] r
                                                             개발 도구     Chapter 13



      간단한 main () 루틴에 있는 코드는 스택 프레임을 만들고 제거하는 부분이 대부분이다. 실
      제 printf () 함수 호출은 리스트의 중간쯤에 있는 0x100004b0 주소에 있는 분기 링크
      (bi）로 표현된다. 이 코드는 PowerPC의 함수 호출인데 , 이 프로그램은 동적 링크 오브젝
      트를 사용하도록 컴파일되었키 때문에 prir止f () 함수에 대한 주소는 프로그램이 실행돼서
      공유 라이브러리에 있는 prin七f () 루틴이 링크되어야 알 수 있다. 만약에 정적으로 링크시
      켜서 빌드했다면 이 시점에서도 printf () 함수에 대한 올바른 메모리 주소를 볼 수 있을
      것이다.


13.5.4 objcopy
      obj copy는 바이너리 오브젝트 형식을 만들거나, 임의로 형식을 변환시킬 수 있다. 이 유틸
      리티는 ROM 또는 플래시에 위치시킬 이미지를 만들어 낼 때 특히 유용하다. 7장에서 소개
      한 U-Boot 부트로더는 obj copy를 이용해서 최종 ELF 파일에서 바이너리 파일과 寸레코
      드25) 형식의 출력을 생성해 낸다. 다음의 예는 obj copy의 키능과 플래시를 위한 이미지를
      어떻게 만드는지를 확인할 수 있다．

         $ ppc_82xx-objcopy --gap--fill= Oxff -o binary u- boot u-boot.bin


      이 obj copy 명령은 플래시 메모리를 위해서 이미지를 어떻게 준비해야 하는지를 보여 준다．
      이 예제에서 입력 파일인 寸boot 파일은 완전한 ELF U-Boot 이미지인데 , 심볼 정보와
      재배치 정보도 포함하고 있다. obj copy 유틸리티는 프로그램 코드와 데이터를 담고 있는
      섹션만 골라서 十boot.bin이라고 지정한 출력 파일에 위치시킨다．

      플래시 메모리의 영역을 지우면 그 내용은 모두 1로 채워져 있다. 그래서 바이너리 이미지의
      중간 중간의 빈 구간을 모두 1로 채우면 플래시에 더 효율적으로 프로그램할 수 있고, 플래시
      의 기록 횟수 한계로 인한 플래시의 수명도 연장할 수 있다. 이를 위해서 obj copy 명령에
      --gap-fi ll 파라미터를 주면 된다．

      이 예제는 obj copy의 일부분에 불과하다. 이 유틸리티는 寸레코드를 생성하는 데도 사용할
      수 있고 어떤 파일 형식을 다른 형식으로 변환할 수도 있다. 자세한 내용은 맨 페이지를 보도
      록 하자．


25) S-레코드 파일은 바이너리 파일을 아스키 (ASCII）로 표현한 것이다. 많은 디바이스 프로그래머（플래시 등의 장치어］ 기록하는 장
    치 또는 프로그램）나 바이너리 유틸리티에서 사용되는 형식이다．


                                                                             4251
醫口1     Embedded Linux Primer




13.6 기E十 바이너리 유틸리티
      툴 체인에는 몇 가지 유용한 유틸리티가 더 있는데 , 이 유틸리티들은 사용법이 아주 쉽고 간
      단하기 때문에 여러 경우에서 쉽게 활용할 수 있을 것이다．


13.6.1 strip
      strip 유틸리티는 바이너리에서 심볼이나 디버그 정보를 제거할 때 사용할 수 있다. 이렇게
      하는 경우는 보통 임베디드 장치에서 사용하는 공간을 줄이기 위함이다. 교차m개발 모델에서
      는 개발 호스트 시스템에는 원래의 바이너리 파일을 두고, 타깃 시스템에는 이들 필요 없는
      정보를 드러낸 바이너리 파일을 두면 편리하다. 이 방법을 이용해서 개발 시스템에서는 교차
      e디버깅을 위해서 심볼 및 디버깅 정보를 사용하면서도 타깃에서는 공간을 절약하는 두 가지
      효과를 볼 수 있다. 就rip은 맨 페이지를 보면 알겠지만 많은 옵션을 가지고 있다．


13.6.2 addr2line
      ［리스트 13-12］에서 m七race를 소개할 때 m七race 분석 스크립트에서 출력된 내용에 파일
      과 줄 번호 정보가 포함된 것을 본 적이 있다. mtrace Penl 스크립트에서는 addr2line
      유틸리티를 사용해서 ELF 실행 파일에 포함된 디버깅 정보를 읽어들여서 해당 주소에 해당
      하는 줄 번호를 출력한다. 같은 mtrace 예제 실행 파일을 이용해서 가상 메모리 주소에 해
      당하는 파일 이름과 줄 번호를 출력할 수 있다.



        $ addr2line -f -e mt ex 0x80487c6
            put_data
             /home/ chri s/ exampl es/mt_ex c: 64




      주의할 것은 put data () 함수 이름도 파일 이름과 줄 번호와 같이 출력된다는 것이다. 이
      는 0x80487c6이라는 주소가 mt ex.c 파일의 64번째 줄에 있다는 것과 이 위치가
      pu七 data () 안에 있다는 것을 말한다. 이 기능은 리눅스 커널과 같이 여러 파일로 이루어
      진 거대한 바이너리 파일에서 이용할 때 더 유용하게 쓸 수 있다．
                                                      개발 도구   Chapter 13




        $ ppc_82xx-addr2line -f -e vmlinux c000d95c
            mpc52xx_restart
            arch/ppc/ syslib/mpc52xx_setup. c: 41




     위 예제는 이 장 전체에 걸쳐 반복해서 나오는 중요한 포인트를 다시 반복해서 보여 주는데．
     바로 아키텍처에 맞게 사용해야 하는 툴이라는 것이다. 즉, 자신이 사용하는 타깃 바이너리
     파일의 아키텍처에 맞도록 구성해서 컴파일된 툴을 사용해야 한다. 교차컴파일러와 마찬가
     지로 addr2line도 역시 교차툴（cross比ool)이고 바이너리 유틸리티 패키지의 일부이다．


13.6.3 strings
     S七rings 유틸리티는 바이너리 파일에 있는 아스키 문자열 데이터를 검사하는 툴이다. 이
     툴은 특히 소스 코드나 디버깅 심볼을 사용할 수 없는 경우에 메모를 덤프를 확인할 때 유용
     하다. 혼히 문제가 되는 바이너리 파일에서 就rings를 통해서 추적해 나가다 보면 시스템
     충돌의 원인을 좁힐 수도 있는 것을 볼 수 있는데 , 비록 strings는 사용할 수 있는 커맨드
     라인 옵션이 조금 많은 편이지만, 배우기도 사용하기도 아주 쉽다. 좀 더 자세한 사용법은
     맨 페이지를 보도록 하자．


13.6.4 Idd
     엄밀하게 바이너리 유틸리티는 아니지만, ldd 스크립트도 임베디드 개발자가 유용하게 쓸
     수 있는 툴이다. 이 스크립트는 C 라이브러리 패키지의 일부이고 사실상 모든 리눅스 배포
     버전에 포함되어 있다. ldd는 어떤 오브젝트 파일이나 기타 파일이 어떤 공유 오브젝트 라이
     브러리를 의존하고 있는지에 대해서 리스트를 출력해 준다. 전에 이미 11장, "BusyBox"어］
     서 ldd를 간단히 살펴봤다. idd 스크립트는 특히 램디스크 이미지를 만들 때 편리하게 사용
     할 수 있다. 임베디드 리눅스 메일링 리스트에 가장 많이 나오는 문제 중의 하나가 바로 루트
     파일 시스템을 마운트하고 난 뒤에 커널 패닉이 발생하는 것이다．




                                                                    427 1
       B     Embedded Linux Primer




             VFS: Mounted root (nfs filesystem) .
             Freeing unused kernel memory: 96k mnit
             Kernel panic - not syncing: No mn仕 found. Try passing init=option to kernel.



           이 문제의 가장 흔한 원인 중의 하나가 바로 루트 파일 시스템 이미지（램디스크, 플래시 또는
           NFS 루트 파일 시스템）에 커널이 실행시키려고 하는 바이너리를 위한 라이브러리가 없기
           때문이다. idd를 이용하면 독자가 사용하려고 하는 바이너리가 실행되기 위해서 필요한 라
           이브러리를 알아낼 수 있다. 그래서 문제없이 루트 파일 시스템 이미지에 포함시킬 수 있다．
           위의 커널 패닉 예에서는 mnit이 파일 시스템에 있었지만, 리눅스 동적 로더가 id.so. i을
           찾지 못한 것이 원인이었다. idd를 사용하는 것은 아주 직관적이다．



             $ xscale_be-ldd mnit
                libc. so. 6 => /opt/mvl/ . . ./lib/ libc. so. 6 (Oxdeadl000)
                ld-linux. so. 3 => /opt/mvl/ . . ./lib/ ld-linux. so. 3 (0xdead2000)



           이 예제는 mnit 바이너리 파일이 동적 라이브러리 객체 두 개를 필요로 한다는 것을 보여
           주는데 iibc와 id-linux가 그것이다. 두 라이브러리 모두 mni七 바이너리가 접근할 수 있
           도록 타깃 시스템에 존재해야 하는데 , 이 말은 읽기와 실행이 가능해야 한다는 말이다．


13.6.5 nm
           nm 유틸리티는 오브젝트 파일에서 심볼을 출력해 준다. 이 툴은 다양한 용도로 사용할 수
           있는데 , 예를 들어 큰 규모의 어플리케이션을 교차컴파일시킬 때 주소 값이 해결되지 않은
       심볼을 만나서 빌드에 실패하게 되었다고 치자. 이때 nm을 이용해서 어떤 오브젝트 모듈에
           해당 심볼이 포함되어 있는지를 찾은 다음에 빌드 환경에 그 파일을 포함시키도록 할 수 있다．

           nm 유틸리티는 각 심볼에 대한 속성도 보여 주는데 , 예를 들어 , 해당 심볼이 전역 심볼인지
       지역 심볼인지 알 수 있고, 또한 해당 심볼이 그 모듈에서 정의되는치 아니면 참조만 되는지
           도 알 수 있다. ［리스트 13-18］에서 U-Boot ELF 이미지인 十boot를 이용해서 nm을 실
           행한 결과를 일부 볼 수 있다．


1428
                                              개발 도구   Chapter 13



     ［리스트 ]3-18) nm을 이용해서 심뷸 출력하71


        $ ppc_85xx-nm u-boot

        fff23140 b base_address
        fff24c98 B BootFile
        fff06d64 I BootpRequest
        fffOOll8 t boot_warm
        fff21010 d border
        fff23000 A _bss_start




     U-Boot 심볼들의 링크 주소를 주목하자. 각 링크 주소는 해당 보드의 메모리 맵에서 최상위
     부분에 매핑되어 있는 플래시 장치에 위치하도록 되어 있다. 위 내용에는 설명을 위해서 몇
     개의 항목만을 나타낸 것이다. 가운데 열에 있는 항목이 심볼의 종류이다. 대문자로 표시된
     것은 전역 심볼을 나타내고 소문자는 지역 심볼을 가리킨다. B는 심볼이 .bss 섹션에 위치
     한다는 것을 나타내고, T는 심볼이 . 七ext 섹션에 있음을 나타낸다. D는 .data 섹션에 있음
     을, A는 이 주소가 절대적인 주소이고 추가적인 링크 단계를 거치더라도 변하지 않는다는
     것을 의미한다. 위 예제에 있는 절대적인 주소 심볼은 . bss 섹션의 시작을 가리키는 심볼이
     고, 처음 .bss 영역을 초기화하는 코드에서 사용된다. 이는 C 실행 환경에서 꼭 필요한 절
     차이다．


13.6.6 prelink
     prelink 유틸리티는 프로그램이 실행되는 시작 시간이 아주 중요할 때 자주 이용되는데，
     동적으로 링크되도록 되어 있는 ELF 실행 파일은 최초에 로드될 때 동적인 심볼이 먼저 링
     크되어야 한다. 하지만 큰 규모의 어플리케이션에서는 이 시간이 상당히 오래 걸리는데，
     prelink는 주소 값이 결정되지 않은 라이브러리 참조에 대해서 사전 정보를 제공할 오브젝
     트 파일이나 공유 라이브러리를 미리 준비해 준다. 실제적으로 이 유틸리티는 어플리케이션
      의 시작 시간을 줄이는 역할을 한다. 맨 페이지를 보면 이 편리한 툴에 대한 자세한 사용법이
     나와 있다．
        Embedded Linux Primer




]3.7 요약
        口 GNU 디버거（GDB）는 많은 기능을 가지고 있는 복잡하지만 강력한 디버거이다. 이 장에
           서는 처음 시작하기 위한 기본적인 정보를 알아보았다．

        口 DDD는 GDB를 위한 그래픽 인터페이스인데 강력한 GDB 커맨드 라인 명령어를 이용해
           서 소스 코드 및 데이터 화면 등을 표시해 준다．

        口 cbrc恥ser는 큰 프로젝트를 이해하는 데 도움을 주는 툴인데, C 소스 코드 프로젝트에
           서 심볼을 빨리 찾아서 표시하기 위해써 cscope 데이터베이스를 사용한다．

        口 리눅스는 다양한 프로파일링 및 추적 툴을 지원하는데, 그 중에서도 S七race,
           itrace, 七Op, ps 그리고 메모리 프로파일러인 mtrace와 dmalloc을 소개했다．

        口 임베디드 개발자는 부트로더나 펌웨어 이미지를 위해써 이미지 파일을 자체적으로 만들
           어야 할 때가 자주 있는데, 이를 위해써 binutils어］대한 지식이 반드시 필요하다. 이
           장에서는 binu七uls에 포함된 다양한 유틸리티 , 즉 readeif, objdump, objcopy
           그리고 기타 유틸리티에 대해서 알아봤다．



13.7. ] 더 읽0j 보기
        GDB: The GNU 프로젝트 디버거
        www.gnu.org/ software/gdb/gdb.html

        GDB 포켯7 레퍼런스mbcket Reference少
        Arnold Bobbins
        O'Reilly Media, 2005


        뎨이터 표시 디버거（DDD : Data Display Debugger)
        www. gnu. org/software/ ddd/

        cbrowser 홈페이지
        http: //cbrowser. sourceforge. net!




I 430
                                             개발 도구   Chapter 13



csc아兀 홈페이지
http://cscope.sourceforge.net/index.html


dmalloc Debug Malloc Library
http: //dmalloc. corn!


툴 안타페이스 표준口IS : Tool Interface Sta끄dard) 실행 파일과 랑캉 항식似刃 명세서
버전 1.2
TIS Committee, 1995년 5월


툴 인터페이스 표준（Tool interface standards)
디버깅 정보 형식 명세서（刀WAI沙 꺄bugg切g Informat幻n Format 枷ecificatio끄)
버전 2.0
TIS Committee, 1995년 5월




                                                           43l 1
    圄目t匣伊 ]4


                  커널 디버깅 기술




이번 장에서 배울 내용

  . 커널 디버깅의 어려움

  . KGDB를 이용한 커널 디버깅

  . 리눅스 커널 디버깅하기

  U 하드웨어를 이용한 디버깅

  U 부팅이 되지 않을 때

  U 요약
蘿 U.     Embedded Linux Primer




       개발 일정을 맞추는 가장 중요한 조건이 한 명의 엔지니어가 버그를 찾고 해결하는 효율성에
       달려있는 경우가 자주 있다. 리눅스 커널 내부를 디버깅하는 것은 상당히 어려운 작업이다．
       어떻게 접근하든지 리눅스 커널 디버깅은 언제나 아주 복잡한 작업이다. 이번 장에서는 이러
       한 복잡한 문제에 대해서 몇 가지 실험해 보고, 커널 내부와 디바이스 드라이버를 디버깅하
       는 기술을 좀 더 향상시키기 위한 아이디어와 방법론에 대해서 생각해 볼 것이다．



14. ] 커널 디버깅의 어려움
       최신 운영체제를 디버깅하기 위해서는 어려운 문제들을 많이 만나게 되는데 , 그 중에서도 가
       상 메모리를 사용하는 운영체제는 그에 따른 독특한 어려움이 있다 프로세서를 서킷 에뮬레
       이터（IC羽 : In-circuit Emulator）로 대체할 수 있는 시절은 가 버렸다. 이는 프로세서가
       너무 빨라지고 복잡해졌기 때문이다. 더군다나 파이프라인 아키텍처는 코드가 실행되는 자세
       한 절차를 숨기는 역할을 하는데 , 이는 버스를 통한 메모리 접근 중의 일부가 코드의 실행과
       다른 순서로 진행될 수 있다는 점과 특히 명령에 스트림1)어］ 대해서 내부 캐시를 사용하기
       때문이다. 그래서 외부 버스 접근이 항상 내부 프로세서 명령에 실행과 정확하게 일치하는
       관계가 성립되지 않고, 대략적으로만 일치한다．

       리눅스 커널 코드를 디버깅할 때 만날 수 있는 문제로는 다음과 같은 것들을 들 수 있다．

         口 리눅스 커널 코드는 여러 부분에서 실행 속도를 위해서 높은 수준으로 최적화되어 있다．

         口 컴파일러도 최적화 기술을 이용해써 컴파일하기 때문에, 실제 C 소스 코드와 생성된 기
             계어 코드와의 관계를 연결시키기가 어려워진다. 인라인 함수가 좋은 예다．

         口 컴파일러가 최적화시킨 코드를 한 단계씩 진행하면 예상치 못한 방향으로 실행되는 것을
             알 수 있다．

         口 가상 메모리는 사용자 영역 메모리를 커널 메모리와 완전히 분리시키기 때문에 ，여러 디
             버깅 상황에서 상당한 어려움을 만날 수 있다.

         口 일부 코드 중에는 기존 디버거로는 한 단계씩 진행할 수 없는 것들도 있다．

         口 특히 시작 코드（startup code）는 하드웨어와 아주 가깝고, （예를 들어, 콘솔이 없거나 메
             모리가 제한되어 있는 등） 사용할 수 있는 자원도 한정되어 있어서 디버깅이 아주 어렵다．


1) （역자주） 하나 이상의 명령에 덩어리를 명령에 스트림이라고 한다．
                                                          커널 디버깅 가술     Chapter 14



      리눅스 커널은 가장 뛰어난 상업용 운영체제 시스템과 경쟁할 수 있을 만큼 고성능의 운영체
      제로 자리 잡았다. 그래서 커널의 많은 부분이 단순히 소스 코드를 읽어 보는 것으로 쉽게
      분석할 수 있는 경우는 별로 없다. 즉, 특정 코드 부분의 흐름을 이해하기 위해서 아키텍처와
      자세한 설계적인 지식이 반드시 있어야 하는 경우가 종종 있다. 이를 위해서 커널 디자인에
      대해서 자세히 설명한 좋은 책이 많이 나와 있다. 14.6.1절의 "더 읽어 보기"에 있는 추천
      서적을 참고하기 바란다.

       CCC는 최적화를 수행하는 컴파일러이다. 기본적으로 리눅스 커널은 -02 컴파일러 옵션으
       로 컴파일되는데 , 이는 코드의 순서와 기본 구조까지도 변경할 수 있는 수준의 최적화 알고
      리즘을 이용하는 옵션이다2) . 예를 들어 , 리눅스 커널은 인라인 함수를 아주 빈번히 이용하
       는데, 인라인 함수3）들은 inline 키워드를 이용해서 선언된 작은 크기의 함수들이다. 그래서
       이 인라인 함수들은 별도의 함수 호출 절차를 위한 오버헤드4) 없이 바로 코드 자체가 실행되
       는 형태로 컴파일퇸다. 인라인 함수를 위해서는 최소 -01 최적화 단계를 지정해야 한다. 최
       적화 옵션을 끄면 디버깅을 더 쉽게 할 수 있지만 이 이유 때문에 리눅스 커널을 빌드할 때
       최적화 옵션을 끌 수 없다．

       리눅스 커널의 많은 부분이 코드를 한 단계씩 순차적으로 실행시키는 것이 어렵거나 불가능
       하도록 되어 있다. 가장 좋은 예가 가상 메모리 설정을 변경하는 코드이다. 어플리케이션이
       시스템 콜을 사용하는 경우, 커널로 진입하게 되기 때문에 프로세스가 바라보는 주소 공간이
       바뀌게 된다. 사실 프로세서의 예외5）를 발생시키는 모든 명령어가 실행중인 컨텍스트를 변
       경시키는 결과를 초래하기 때문에 한 단계씩 코드를 수행시키면서 디버깅하는 것이 어렵거나
       불가능한 것이다．



14.2 KGDB를 이용한 커널 디버깅
       리눅스 커널에서 소스 단계 심볼릭 디버깅을 하기 위해서 많이 사용되는 방법이 두 가치 있다．



2) 이 장의 뒤편에 있는 14. 6. 1절 ＼기 읽어 보기"에 있는 GCC 매뉴얼을 보면 최적화 단꼐（야汕mza如n Level)에 대한 자세한 내용
   을 참고할 수 있다．
3) 인라인 함수는 매크로와 비슷한뎨, 컴파일 시에 데이터 타입을 검사할 수 있다는 장점이 있다．
4) （역자주） 과부하. 불필요한 자원 낭비의 뜻을 갖는 용어．
5) （역자주） 프로세서에서의 예뫼 (excep山n）이라는 것은 잘못된 명령어나 브레이크 포인트 명령에 勘］ 실행되었을 때 발생하는 일
   종의 이벤트이다. 인터럽트와도 일면 비슷한 개념이다．
         Embedded Linux Primer




         口 원격 gdb 증계기로서 KGDB 이용하기

         口 프로세서를 직접 제어하는 하드웨어 JTAG 디버거6)


      JTAG를 이용한 디버깅은 14.4절 "하드웨어를 이용한 디버깅"에서 설명할 것이다．

      KGDB（커널 GDB）는 원격 시리얼 프로토콜을 이용해서 gdb 인터페이스를 지원하는 리눅
      스 커널 패치들을 조합한 것이다. KGDB는 호스트 개발 워크스테이션에서 실행되는 교차
      gdb와 통신할 수 있는 gdb 스텁7) (stub）을 구현하고 있다. 아주 최근까지만 하더라도
      KGDB를 이용하기 위해서는 타깃 시스템이 시리얼 연결을 지원해야 했다. 비록 상대적으로
      최근의 일이지만 일부 타깃에서 이더넷을 이용해서 KGDB를 사용할 수도 있게 되었다. 최신
      KGDB는 아직 kernel. org의 기준 커널에는 반영되지 않고 있다. 독자가 사용하는 타깃에
      서 KGDB를 사용하려면 직접 포팅하거나, 해당 아키텍처와 플랫폼과 KGDB를 지원하는 임
      베디드 리눅스 배포 버전을 구해야 한다. 최신 임베디드 리눅스 배포 버전은 대부분 KGDB
      를 지원한다.

      ［그림 14-끄은 KGDB 디버그 환경을 보여 준다. 타깃 보드에 모두 세 개의 연결이 맺어져
      있다. 그 중 이더넷은 NFS 루트 파일 시스템을 마운트하고 텔넷 세션을 호스트에서 사용하
      기 위해서 연결되어 있다. 만약에 보드가 플래시에 램디스크 이미지를 저장하고 있어서 이
      이미지를 루트 파일 시스템으로 마운트한다면 이더넷 연결은 제거해도 된다．

                                  이더넷 허브
               GDB

                                               KGDB




                                  추가 시리얼
                                  포트（옵션）
             호스트 시스템
      I 그림 14네 KGDB 디버그 환경




6) （역자주） JTAG 디버거는 아주 고가의 쟝비이다．
7) （역자주） 일반적으로 스텁이란 다른 기능이나 모듈을 사용하기 위한 연결 고리 역할만을 하는 간딘한 코드를 말한다．
                                                                                  커널 디버깅 기술   Chapter 14



      시리얼 포트 하나가 KGDB와 호스트 캐발 시스템에서 실행되는 gdb를 연결하기 위해서 전
      용으로 사용된다. 그리고 추가적인 옵션으로 콘솔 을 위한 시리얼 포트가 사용될 수도 있다．
      시리얼 포트가 하나뿐인 시스템에서 KGDB를 사용하려면 좀 더 불편할 수도 있을 것이다．

      ［그림 14山에서 볼 수 있는 것처럼 디버거（교차 gdb 버전）는 개발 호스트 시스템에서 실행
      된다. KGDB는 타깃 시스템에서 실행중인 커널의 일부라고 볼 수 있다. KGDB는 타깃 시스
      템에 있는 gdb와 통신하기 위해서 필요한 후크8) (hook) 기능을 구현하고 있는데 , 타깃 시스
      템에 브레이크 포인트를 설정하거나, 메모리 내용을 확인하고 프로그램을 한 단계씩 실행시
      키는 등의 작업을 위해서 통신 기능을 구현하기 위함이다．


14.2.1 KGDB 커널 구성
      KGDB는 커널 구성 유틸리티를 통해서 사용할 수 있도록 설정해야 하는 커널 기능이다．
      KGDB는 커널 해킹 메뉴에서 선택할 수 있는데 , ［그림 14-2］를 보면 알 수 있다. 구성의
      일부로서 KGDB가 사용하는 시리얼 포트를 선택해야 한다. 그리고 ［그림 14-2］와 같이 커널
      을 디버그 정보를 포함해서 빌드하도록 하는 옵션을 선택했다는 점을 주의하자. 이 옵션은 컴
      파일러 옵션에 小g를 추가하는테 심볼 디버깅 정보를 포함해서 빌드시키도록 하는 옵션이다．

      E沁 qm目n5 ddp

                  ［그
                  La나J
                              日
                              5aYe   료昶
                                              ？二．!;
                                                  F哨
                                                          m     呼
                                                        C예paM Eapaad

      OMMa.                                                Nasa낀
      nKeinS lacK,빙
            LI 帥卵 m凹I이m的mmmmk5                             PPINTKJINE        N
          口 k Kasal dcba9夕目                                OEBUGKERNEL
              二；Ma小L 5Y드Rq kay                             M.AQC戶SYSRQ
               K寸m키四 LM尸r 11c.llK. c F4K氏 l7=) l2laF,      IOC. BUF..SF作斗
              ：그Cd1e(! 5(r冷d내er 51ah5t旺a                   SCI4ED引MS
              그Dab四 rnemmya砒的m5                            DEBUGSLNB
              nSm汕：  乂k CI,叫뿌凹                             DEbUC多끼NIOCK      N
                듸t牛11니n5K1e5口, Cck dlacki.日                D든dUO포거Nil乂K$I.EEP N
              r : m恥cad吐目J呵四                               DEBUG. KOBJFCI    N
              三 Ccc叩蜘 伽 岫lad 나dl daN呂 耐0                   DE0UCJNFO
               n De뇨씨 FdU」
                         ，Y·
                           ，rm                             DEBUCJ咎           N
             , 口1岫艀蜘bk
              口 ] 5"出 Pad
                    1 IlydO                                KGDB_TIYS0
                      lap '                                KGLFBITVS1
      1
          1m汕由95i 뇨m너 dab四 1 kliOU

          1吐奴如mFe, 叫 1比nk5 油k多1h 竹田 UnUX k之i州 5에m 枷I

          各忿：d芬怒；業ad崙竄崙峀琵沙m' dm

      1 그림 14-2 KGDB를 위한 커널 구성 옵션


8) （역자주） 후크（hook) 또는 후킹은 어떤 이벤트에 대해서 체인 형식으로 연결된 함수를 순차적으로 실행하는 프로그래밍 기법이
   다. 즉, 키보드가 눌렸을 때 자신도 어떤 처리를 하고 싶다면 후킹을 등록해서 모든 키보드 이벤트를 훔쳐볼 수 있게 된다. 이
 런 메커니즘을 후킹이라고 한다．
    難    Embedded Linux Primer




14.2.2 KGDB를 활성화시킨 타깃 부팅하기
        커널을 KGDB를 지원하도록 설정해서 빌드했다면 커널을 실행할 때 KGDB 기능을 반드시
        활성화해야 한다. 불행히도 KGDB를 활성화하는 방법이 아직 통일되지 않아서 모든 아키텍
        처와 버전마다 각각 다르다. 사실 KGDB는 커널 커맨드 라인을 통해서 커널에 스위치를 전
        달하면 활성화할 수 있다. 만약에 KGDB를 지원하도록 컴파일된 커널에서 커맨드 라인 스위
        치를 통해서 이 기능을 활성화하지 않으면 아무 일도 하치 않는다. 하지만 KGDB가 활성화
        되면 부팅 과정의 아주 이른 초기 단계에 KGDB로 활성화된 브레이크 포인트 지점에서 멈추
        게 되고, 타깃의 gdb를 이용해서 연결할 수 있도록 대기한다. ［그림 14-釗은 KGDB가 활성
        화된 경우에 초기 브레이크 포인트를 생성하는 방법을 논리적으로 표현한 것이다.

          보드
                                   초기
          초기화
                                 시리얼 매핑
            1
          플랫폼
          초기화                    시리얼 포트
                                  초기화



                                 디버그 트랩
                                   설정



                                          호스트 GDB
                                 BKPTO    연결을 기 다림



          정샹

        \,，분邑，/
      I 그림 ]4-3 KGDB 로직

        KGDB는 호스트와 시리얼 포트9）를 통해서 연결해야 한다. KGDB 설정의 첫 번째 단켸는
        부팅 과정의 초기 시점에 시리얼 포트를 사용할 수 있도록 초기화하는 일이다. 많은 아키텍
        처가 UART 하드웨어 관련 레지스터를 접근하기 위해서 먼저 커널 메모리 영역에 매핑되어

9) 이더넷도 사용할 수 있는 KGDB보다 이젼 버젼에만 해당하는 설명이다．
                                                커널 디버깅 기술     Chapter 14




있어야 한다. 알맞은 주소 번지에 매핑된 후에 시리얼 포트를 초기화하고 디버그 트랩 핸들
러를 등록해서 프로세서에서 발생되는 예외를 디버거가 가로챌 수 있도록 해야 한다．

［리스트 14-1]에는 부팅 시에 KGDB를 활성화시킨 경우에 터미널에 출력되는 내용을 나타낸
것이다. 이 예제는 AMCC 440EP 평가용 보드（요세미티 보드）에서 U-Boot 부트로더를 사
용해서 실행한 것이다．

［리스트 ]4-1] 나Boot로 KGDB7F 활성화된 커널 부팅하71

  => sete bootargs console=ttySl, 115200 root=/dev/nfs rw ip=dhcp gdb
  => bootm 200000
  ## Booting image at 00200000 . . .
     Image Name: Linux-2. 6.13
     Image Type: PowerPC Linux Kernel Image (gzip compressed)
     Data size:     1064790 Bytes = 1 MB
     Load Address: 00000000
     Entry Point: 00000000
     verifying Checksum . . . OK
     Uncompressing Kernel Image . . . OK
  $T0440: c000aeSc ; 01: c0205fa0; #d9 <<< 본문 참조



부팅 과정에서 출력되는 내용은 대부분 7장, "부트로더"에서 U-Boot를 설명할 때 본 것들이
라 친숙할 것이다. 하지면 위 커널 부팅 과정에는 두 가지 특별한 사항이 있는데 , 커맨드 라
인 파라미터에서 KGDB를 사용할 수 있도록 하는 옵션을 치정하고 있다는 것과 커널 압축이
풀린 후에 이상한 문자열이 출력되는 것이다．

7장을 다시 보면 U-Boot의 boo七args 환경 변수에 커널 커맨드 라인을 정의해서 사용했다．
여기에 gdl) 파라미터를 추가해서 커널이 초기 단계에 브레이크 포인트를 잡고 호스트 디버
거의 연결（독자가 사용하는 교차-g的을 기다리도록 지시하는 것을 알 수 있다．

［그림 14-3］에 나온 것처럼 커널은 gdb 파라미터가 존재하는 지를 검사한 후에 원격의 （호
스트에 있는） 디버거로 제어권을 넘기려고 시도하는데 , ［리스트 14-1]에 시리얼 포트로 출
력된 일련의 아스키 문자가 그 명백한 증거이다. gdb7} 사용하는 원격 시리얼 프로토콜에
대해서 더 알고 싶다면 이 장의 뒤편에 있는 참고 문헌에서 gdb 매뉴얼 문서를 참고하도록
하자. 위 예제에서는 KGDB7} 정지 응답（Stop Reply) 패킷을 보내서 원격 호스트 gdb 세션에
  繫.    Embedded Linux Primer



      브레이크 포인트 트랩이 걸렸음을 보고하고 있다. 그 뒤에 두 개의 32비트 파라미터는 각각
      실행중인 프로그램의 위치와 스택 프레임을 가리킨다．

      이제 커널이 준비되었고, 호스트 디버거가 연결되기를 기다리고 있는 상태이기 때문에 디버
      깅 세션을 시작할 수 있다. 즉, 호스트 개발 시스템에서 교차-gdl）를 실행시켜서 타깃과 gdb
      원격 프로토콜을 이용해 연결한다. 이 예제에서는 시리얼 포트 하나를 공유해야 하기 때문에
      gdb를 실행시켜서 연결하기 전에 기존에 타깃에 열려 있는 터미널 에뮬레이터 연결을 종료
      해야 한다．［리스트 14-2］에서 gdb 연결 과정을 볼 수 있는데 , 이 내용은 먼처 기존 터미널
      에뮬레이터를 닫아서 gdb7} 시리얼 포트를 사용할 수 있는 상태라고 가정한 것이다．

      ［리스트 14-2) KGDB에 연결시키:
                           71

         $ ppc_4xx-gdb --silent vmlinux
         (gdb) target remote /dev/ ttysO
         Remote debugging using /dev/ttySo
         breakinst 0 at arch/ppc/kernel/ppc- stub. c: 825
         825    }
         (gdb) 1
         820                   return;
         821            }
        822
        823            asm(" .globl breakinst          \n\
        824                 breakinst: .long 0x7d821008") ;
        825     }
        826
        827     #ifdef CONFIG_KGDB_CONSOLE
        828     /* Output string in GDB 0-packet format if GDB has connected.
        if notMng
        829        output, returns 0 (caller must then handle output) . */
        (gdb)



      여기서는 다음의 세 가지 명령을 내린다．

       口 gdb를 실행시키고 커널 ELF 파일인 vmli flux를 인자로 전달한다．

       口 gdb에 있는 targe七 remo七e 명령을 이용하서 타깃에 연결한다．

       口 list    명령의 축약형인 1 명령을 실행해서 현재 위치어］ 해당하는 소스 코드를 출력한다．



440
                                                  커널 디버깅 기술   Chapter 14



     물론 당연한 이야기일 수도 있지만, gdb에 인자로 전달하는 vmhinux 이미지와 타깃에서
     실행되는 커널 바이너리 이미지는 일치하는 커널을 빌드한 결과물이어야 한다. 그리고 디버
      깅 정보를 포함하먀 하기 때문에 -g 컴파일러 옵션을 설정해서 컴파일되어 있어야 한다．

     타깃에 원격으로 명령어를 내리면 gdb는 현재 프로그램 카운터（PC）의 위치를 출력하는 것
      으로 응답하게 된다. 이 예에서는 커널이 . . . /arch/ppc/kernel/pp아S七ub . c의 823번
      째 줄꼐 있는 인라인 어셈블러 구문에 잡은 브레이크 포인트에서 멈춰 있다. 그리고 계속하
      라는 커맨드인 continue （이 명령을 내리면 825번째 줄부터 실행을 재개할 것이다．


14.2.3 유용한 커널 브레이크 포인트
      이제 타깃 보드의 커널을 디버깅할 수 있는 연결을 맺은 상태이다. gdb에 coi止inue （이
     명령을 내리면 커널은 부팅을 계속할 것이고, 특별한 문제가 없으면 부팅 과정을 종료할 것
      이다. 이 부분에서 KGDB가 갖는 한 가지 작은 한계 사항을 확인해 볼 수 있다. 즉, 이 한계
      는 커널의 아주 초기 시점（예를 들어 , 전체 기능이 다 구현된 인터럽트 드리븐 시리얼 포트
      드라이버가 설치되기 전에）에서도 디버깅이 가능하도록 할 것이냐, 아니면 KGDB의 디버그
      엔진을 최대한 강건하고 유연하게 유지할 것이냐의 선택에서 어느 정도 타협점을 찾아야 했
      키 때문에 갖는 한계라고 볼 수 있다. 말이 좀 어려울 수 있는데 , 결국 KGDB는 단순한 폴
      링10) (polling) 방식의 시리얼 드라이버를 이용해서 커널이 실행될 때 오버혜드를 최소화하
      도록 했다. 이렇게 구현한 것으로 인한 단점은 전통적인 ct'- c 또는 브레이크 입력이 시리
      얼 포트에서는 전혀 동작하지 않는다는 점이다. 그래서 브레이크나 다른 폴트 상황을 만나지
      않는한 실행중인 커널을 임의로 중단시킬 방법이 없다．

      이런 이유 때문에 시스템 전빈에 걸쳐서 브레이크 포인트를 정의해서 현재 실행중인 쓰레드
      를 중단시키는 방법을 관행처럼 사용하고 있다. ［리스트 14-읾에서 일반적으로 가장 많이
      쓰이는 두 가지를 볼 수 있다．




10) （역자주） 인터럽트 드리븐이란 인터렵트가 뜰 때 그 이벤트를 기준으로 어떤 동작이나 처리를 하는 프로그램 기법을 말하工
    반대 개념으로 폴링은 코드가 계속 특정 상태가 될 때까지를 기다리는 방식이다． 간단히 키가 눌릴 때까지 기다릴 것이냐의 문
    제에서, 무한정 기다리는 경우가 폴링, 다른 일을 하다가 눌리면 그에 따른 처리를 하는 구조가 인터럽트 드리븐이다．


                                                                    441 1
轟a.     Embedded Linux Primer



   ［리스트 14-3] 일반적으로 사용되는 커널 브레이크 포인트


        (gdb) b panic
        Breakpoint 1 at 0xc0016b18: file kernel/panic. c, line 74.
        (gdb) b sys_sync
        Breakpoint 2 at 0xc005a8c8: file fs/buffer. c, line 296.
        (gdb)




      야北의 breakpoin七 명령을 이용해서 （물론 여기서도 축약형을 이용한다） 브레이크 포인트
      두 개를 설정했다. 하나는 panic (）이고, 나머치 하나는 sync 시스템 호출의 시작점인
      sys sync (）이다. 앞의 panic (）어］ 설정한브레이크 포인트는 마치막 이벤트가 패닉을 발
      생시키는 시점에 디버거가 제어권을 가질 수 있도록 해 준다. 즉, 패닉이 발생한 시점에 시스
      템의 상태를 실험해 볼 수 있다. 두 번째 브레이크 포인트는 타깃 하드웨어에서 실행중인 터
      미널에서 사용자 영역 명령인 sync를 입력해서 현재 커널을 중단시키고 디버거로 제어할 수
      있게 해 준다．

      이제 디버깅 세션이 준비되었기 때문에 다음 작업을 진행할 수 있다. 현 상태는 타깃에서
      KGDB가 켜져 있는 리눅스 커널이 실행중이고, KGDB가 정의한 초기 브레이크 포인트에
      멈춰 있다. 그리고 호스트시스템에서 ppc 4xx-gdb라는 교차 디버거를 실행시켜서 타깃과
      연결했다. 그리고 필요한 시스템 브레이크 포인트를 몇 가지 설정했다. 이제 원하는 디버킹
      작업을 진행하면 된다．

      한 가지 주의할 점은 당연히 . . . /arch/ppc/ set可LC어］ 있는 breakpoint () 함수를 이
      용해서 KGDB가 활성화된 커널과 方入E어］ 있는 교차-gdb7} 연결되어 있지 않으면 코드를
      한 단계씩 실행시켜 볼 수 없다는 것이다. ［그림 14-3］을 통해서 KGDB가 제어권을 갖기
      전까지 실행되는 코드를 대략적으로 파악할 수 있다. KGDB가 제어권을 갖기 이전 시점의
      코드를 디버깅하려면 하드웨어 디버깅 장비를 이용해야 한다. 이 부분에 대해서는 14.4절
      "하드웨어를 이용한 디버깅"에서 알아보자．



14.3 리눅스 커널 디버깅하71
      커널 코드를 한 단계씩 진행해1 가면서 디버깅하는 가장 흔한 이유는 각자가 사용하는 보드
      플랫폼을 위해서 코드를 변경할 필요가 있을 때다. 그럼 AMCC 요세미티 보드를 이용해서
                                                          커널 디버깅 가술      Chapter 14



이 작업을 어떻게 진행하는지 알아보자. 먼저 플랫폼을 위한 아키텍처 설정을 하는 함수에
브레이크 포인트를 잡고, 이 브레이크 포인트를 만날 때까지 코드를 계속 실행시키도록 하
자. ［리스트 14-4］에 이 과정이 나와 있다．

［리스트 ]4-4] 아키텍처 설정 코드 디버깅


  (gdb) b yosemite_setup_arch
      Breakpoint 3 at 0xc021a488:
          file arch/ppc/platforms/4xx/yosemite.c, line 308.
  (gdb) C
  Conti nui ng.
  can 't send signals to this remote system. SIGILL not sent.

  Breakpoint   3,   yosemite_setup_arch O at arch/ppc/platforms/4xx/yosemite. c: 308
  308                   yosem卄e_set_emacdataQ;
  (gdb) 1
  303     }
  304
  305     static void _in卄
  306     yosemite_setup_arch(void)
  307     {
  308             yosemi te_set_emacdataO;
  309
  310                I bm440gx_get_clocks (&clocks, YOSEMITE_SYSCLK, 6 士 1843200) ;
  311                ocp_sys_info.opb_bus_freq = clocks. opb;
  312
  (gdb)



실행되다가 yosemite .c 파일의 308번째 줄에 있는 yosemite se七up arch () 함수에
설정한 브레이크 포인트를 만나면 제어권이 gdb로 넘어간다. list (i) 명령어는 브레이크
가 걸린 308번째 줄 코드를 중심으로 위아래 코드가 나열된다. gdb에 con七inue （이 명령
을 내리자마자 경고 메시지가 하나 출력되는 것을 볼 수 있는데 , 이 부분은 gdb가 원격 시스
템의 기능을 테스트하는 과정을 보여 주는 내용일 뿐이기 때문에 그냥 무시해도 된다. 즉，
처음에는 타깃에 con七inue Wi七h signal 시그널을 보내려고 하지만 타깃으로부터 NAK
를 받는다. 그래서 gdl七 이 정보를 화면에 출력하고, 이 명령에 대신에 표준 continue
명령을 보낸다．



                                                                               443    I
          Embedded Linux Primer




 14.3.1 gdb 원격 시리얼 프로토콜
        gdb에는 개발 호스트 시스템에 있는 gdb와 타깃 간의 원격 프로토콜을 감시할 수 있는 디버
        그 옵션 스위치를 가치고 있다. 이 옵션을 이용하면 기반 프로토콜을 이해하는 데 아주 유용
        할 뿐 아니라, 타깃이 이상 상태를 보이거나 오작동하는 것처럼 보일 때 문제를 해결하는 데
        도 도움이 된다. 이 디버그 모드를 켜기 위해서는 다음 명령을 입력하면 된다．

           (gdb) set debug remote 1

        원격 프로토콜 디버킹을 활성화하고 난 후에 gdb에서 con七inue 명령과 스텝 명령을 내릴
        때 어떤 내용을 주고받는지를 보면 많은 것을 배울 수 있다. ［리스트 14-5］에서 원격 디버깅
        을 켠 상태에서 continue 명령을 내린 경우에 어떤 내용들을 주고받는치 볼 수 있다．

        ［리스트 ]4小5] 원격 프로토콜의 continue 명령 예제

          (gdb) C
          Conti nul ng.
          sending packet: $mc0000000, 4#80. . .Ack
          packet received: c022d200
          sending packet: $Mc0000000, 4: 7d821008#68. . .Ack
          packet received: OK
          sending packet: $mc0016de8, 4#f8. . .Ack
          Packet received: 38600001
          sending packet: $Mc0016de8, 4: 7d821008#eO. . .Ack
          Packet received: OK
          sending packet: $mc005bd5c, 4#23. . .Ack
          Packet received: 38600001
          sending packet: $Mc005bd5c, 4: 7d821008#0b. . .Ack
          Packet received: OK
          sending packet: $mc021a488, 4#c8. . .Ack
          Packet received: 4bfffbad
          sending packet: $Mc021a488, 4: 7d821008#b0. . .Ack
          packet received: OK
          sending packet: $c#63. . .Ack
             <<< program running, gdb waiting for event




I 444
                                                          커널 디버깅 기술      Chapter 14



      비록 처음 볼 때는 좀 어려워 보이지만, 어떤 일이 일어나고 있는지 아주 쉽게 이해할 수 있
      다. 간단히 살펴보면 gdl造 타깃에 있는 모든 브레이크 포인트를 다시 원래대로 복원시키는
      일을 한다. ［리스트 14-3］에서 입력한 두 개의 브레이크 포인트 panic () 고｝ sys sync ()
      를 상기해 보자. 그리고 ［리스트 14-4］에서 서］ 번째 브레이크 포인트를 추가했기 때문에 모
      두 세 개의 사용자 지정 브레이크 포인트가 설정되어 있다. 이들 브레이크 포인트는 gdb의
      info breakpoints 명령으로도 확인해 볼 수 있다. 여기서도 축약형 명령어를 사용한다.



        (gdb) i b
        Num Type            Disp     Enb Adc卄ess 닙hat
        1 breakpoint         keep y  0xc0016de8 in panic at kernel/panic. c: 74
        2 breakpoint         keep y  0xcO05bd5c in sys_sync at fs/buffer. c: 296
        3 breakpoint         keep y  0xc021a488 in yosemite_setup_arch at
        arch/ppc/platfornis/4xx/yosemi te. c: 308
               breakpoint already hit 1 time
        (gdb)



      이제 위 리스트에서 볼 수 있는 주소 값과 ［리스트 14-5］에서 원격 $m 패킷으로 설정하는
      주소 값을 비교해 보자. $m 패킷은 "타깃 메모리 읽기" 명령이고, $M 패킷은 "타깃 메모리
      쓰71" 명령이다. 브레이크 포인트마다 브레이크 포인트를 설정할 주소에 있는 값을 타깃으로
      부터 읽어 들여서 承均7} 호스트에 따로 저장해 두게 된다（그래서 나중에 다시 원래 명령
      어11）로 복원시킬 수 있다）. 그리고는 브레이크 포인트를 설정할 위치에 있는 명령어를
      Powe叩C의 七rap 명령어인 七i呵e r2, r2 (0x7d821008）로 바꾸어 놓는다. 이렇게 하면
      이 명령이 실행될 때 디버거로 제어가 넘어가게 된다. ［그림 14-4］에서 이 과정을 볼 수
      있다.




11) ［역자주） 기본적으로 스프트웨어 브레이크 포인트의 원리는, 브레이크를 잡고 싶은 주소어］ 있는 원래 명령어를 특수한 명령어
  로 바꿔치기 하고, 그 명령이 실행되면 디버거가 제어권을 얻게 되고, 디버거가 저장해 두고 있던 원래 명령을 다시 복원시켜
  서 원래 작업을 계속 진행하도록 하는 방식이다．


                                                                               445 1
            Embedded Linux Primer




                                                        타깃 시스템의 가상 메모리

                                                             twge r2 r2     c000 0000

                   GDB
                                                             twge r2 r2     cOOl 6de8


                                                             twge r2 r2     c005 bd5c

                                                                커널
                                                                가상
                                                               몌모리

                                                             twge r2 r2     c021 a488




        I 그림 ]4-4 gdb가 타깃의 메모리에 브레이크 포인트 명령을 삽입하는 형태


        브레이크 포인트를 세 개만 설정했는데도 gdb는 모두 네 개의 브레이크 포인트를 설정하는
        것을 볼 수 있는데 , 타깃 메모리의 小＜c000 0000에 설정한 첫 번째 브레이크 포인트는 gdb
        에 의해서 시작 시에 자동으로 설정된다. 이 위치는 링크가 완료된 커널 이미지 ELF 파일에
        서    S七art7下 시작되는 부분이다. 이 말은 결국 사용자 영역 프로그램의 디버킹을 위해서
        main () 함수에 gdb가 브레이크 포인트를 자동으로 설정해 주는 것이다. 이것을 제외한 나
        머지 서］ 개의 브레이크 포인트는 전에 입력한 것들이다.

        gdb로 제어권이 넘어가도록 하는 이벤트가 발생한 경우에는 위에서 설명한 과정의 역순으로
        작업이 진행된다. ［리스트 14-6］에서 yosemi七e se七up arch () 함수에 걸어놓은브레이
        크 포인트를 만났을 때 처리하는 과정을 자세히 볼 수 있다．

        ［리스트 14-6] 원격 프로토콜 : 브레이크 포인트를 만났을 ［머


            Packet received: T0440: c021a488 ;01: c020ff90;
            sending packet: $mc0000000, 4#80. . .Ack <<< Read memory @c0000000
            Packet received: 7d821008
            Sending packet: $Mc0000000, 4: c022d200#87. . .Ack <<< write memory
            Packet received: OK


I 446
                                                              커널 디버깅 기술     Chapter 14



         sending packet: $mc0016de8, 4#f8. . .Ack
         Packet received: 7d821008
         sending packet: $Mc0016de8, 4: 38600001#a4. . .Ack
         Packet received: 0K
         sending packet: $mc005bd5c, 4#23. . .Ack
         Packet received: 7d821008
         Sending packet: SMc005bd5c, 4: 38600001#cf. . .Ack
         Packet received: 0K
         Sending packet: $mc021a488, 4#c8. . .Ack
         Packet received: 7d821008
         sending packet: $Mc021a488, 4 :4bfffbad#dl. . .Ack
         Packet received: 0K

         Sending packet: $mc021a484, c#f3. . . Ack
         Packet received: 900100244bfffbad3fa0c022
         Breakpoint 3, yosemite_setup_arch 0 at arch/ppc/platforms/4xx/yosemite. c: 308
         308             yosemite_set_etnacdata0;
         (gdb)



       gdb에서 $T는 스톱 응답（stop reply) 패킷인데 , 이 패킷은 브레이크 포인트를 만났을 때
       타깃에서 gdl屈 전달된다. 이 예에서는 $T 패킷이 프로그램 카운터의 값과 레지스터 r1의
       값을 전달하1 주고 있다12) . 나머지 내용은 ［리스트 14巾5］에서 하는 작업을 역순으로 진행하
       는 내용이다. 즉, gdl）가 각각의 메모리 위치에 있던 원래의 코드 값으로 되돌려 놓는 것이다．


14.3.2 최적화된 커널 코드 디버깅하기
       이 장의 시작 부분에서 컴파일러 최적화를 거친 커널 코드를 디버깅할 때 생길 수 있는 난점
       에 대해서 설명했다. 그리고 리눅스 커널은 기본적으로 尸O2 최적화 레벨에서 컴파일되도록
       되어 있다. 지금까치 다룬 예제에서는 디버깅 작업을 간단히 하기 위해서 -O1 최적화 옵션을
       사용했다. 이제 컴파일러의 최적화가 어떤 식으로 실제 디버깅 작업을 어렵게 하는지 예를
       통해서 알아보자．




12) 앞에서도 언급했듯이 gdb 원격 프로토콜은 gdb 매뉴얼에 자세히 나와 있다. 이 장의 마지막 14. 6. 1절 디 읽어 보7]"를 참고하
  자．
   驥a    Embedded Linux Primer




        이 문제와 관련된 인터넷 메일링 리스트에 포스트된 글을 보면 디버킹 툴이 고장난 것 같다는
       내용을 자주 볼 수 있는데 , 주로 디버거에서 코드를 한 단계씩 진행할 때 윗줄의 소스로 이동
       해 버리거나 원래 소스 코드대로 진행되지 않는 것처럼 보인다는 글을 올리는 것을 볼 수
       있다. 여기서 컴파일러 최적화 때문에 소스 단위에서 디버깅하는 것이 어려워지는 이유를 예
       를 들어서 살펴보자. 이 예제에서는 브레이크 포인트를 만났을 때 gdb7} 표시하는 코드의
       줄 번호가 함수를 인라인으로(mnim ing) 13) 처리하는 최적화 때문에 실제 소스 파일의 해당
       부분과 일치하지 않는다.

      실험을 위해서 ［리스트 14卜4］에서 사용한 것과 같은 디버그 코드를 이용해 보자. 하지만 이
       번에는 프로그램을 -02 컴파일러 최적화 옵션을 주고 컴파일했다. 이 최적화 옵션이 리눅스
      커널에서 사용되는 기본 최적화 옵션이다. ［리스트 14-7］에서 디버킹 세션을 실행시킨 결과
      를 볼 수 있다．

      ［리스트 ]4-7] 최적화된 아키텍처 섣정 코드


          $ ppc_44x-gdb --silent vmlinux
          (gdb) target remote IdevittysO
         "Remote debugging using /dev/ttySO
         breakinst 0 at arch/ppc/kernel/ppc-stub.c:825
          825     }
          (gdb) b panic
         Breakpoint 1 at 0xc0016b18: file kernel/panic.c, line 74.
          (gdb) b sys_sync
         Breakpoint 2 at 0xc005a8c8: file fs/buffer. c, line 296.
         (gdb) b yosemite_setup_arch
         Breakpoint 3 at 0xc020f438: file arch/ppc/platforms/4xx/yosemite. c, line 116.
         (gdb) c
         Conti nul ng.

         Breakpoint 3, yosemite_setup_arch 0
             at arch/ppc/platforms/4xx/yosemi te . c:116
         116           def = ocp_get_one_device(ocP_VEND0R什IBM, 0CP_FUNC_EMAC, 0) ;
         (gdb) 1
         111           struct ocp_def *def;
         112           struct ocp_func_emac_data *emacdata;
         113

13) C역자주） 작은 코드로 이루어진 함수를 호출하는 부분을 실제 그 작은 함수로 대체시켜 버리는 최적화 기술, 불필요한 스택
                                                                        접
  근 오버헤드를 줄일 수 있다．
                                                              커널 디버깅 기술        Chapter 14



          114           /* set mac_addr and phy mode for each EMAC 央/
          115
          116           def = ocp_get_one_device(ocp_vENDoR_IBM, OCP_FUNC_EMAC, 0) ;
          117           emacdata = def->addidons;
          118           memcpy (emacdata->mac_addr, _res.bi_enetaddr, 6) ;
          119           emacdata->phy_mode = PHY_MODE_RMII;
          120
          (gdb) p yosemite_setup_arch
          $1 = {void (void) } 0xc020f41c <yosemite_setup_arch>



       ［리스트 14-4］를 다시 보면 실제로 yosemi七e setup arch () 함수가 yosemite. c 파
       일의 306번째 줄에서 시작하는 것을 알 수 있는데 , 이를 ［리스트 14-끼과 비교해 보자. 설
       정한 브레이크 포인트를 만났을 때 gdb7} 보고하는 위치는 yosemi七e. c의 116번째 줄이
       다. 처음 보면 디버거와 해당하는 소스 코드 간에 정보가 서로 일치하지 않는 것처럼 보인다．
       gdb의 버그일까9 먼저 컴파일러가 생성한 디버그 정보를 확인해 보자. 13장, "개발 도구'에
       서 설명한 readeif '4) 툴을 이용해서 컴파일러에 의해서 만들어진 디버그 정보를 확인할
       수 있다．



           S ppc_44x- reade卄 --debug-dump=info vmlinux I grep -u6 \
             yosemite_setup_arch I tail -n 7
              DW_AT_name      : (ind卄ect string, offset: 0x9c04) : yosemite_setup_arch
              D吐AT_d吼］mfj] e : 1
              DW_AT_decl_line : 307
              DW_AT_prototyped: 1
              DW_AT_1o比pc     : 0xc020f41c
              D吐釘J너gh니：)C     : 0xc02 0f 794
              DW_AT_frame_base: 1 byte block: 51      (Dw_0P_regl)



       소스 코드의 307번째 줄의 문제의 함수를 찾기 위해서 DWARF2 형식의 디버킹 레코드15)
       를 모두 이해할 필요는 없고 대신 13장에서 설명한 툴 중의 하나인 addr2line 유틸리티를
       써서 확인해 보자. ［리스트 14-7］의 qdb에 나오는 주소를 이용하자．



14) 교차 버전 read寸를 사용해야 한다는 점을 기억하자. 예를 들어, PowerPC 4奴는 ppc_44x-readelf를 사용한다．
15) D＼人乏df 디버그 정보 명세서는 이 장의 맨 뒤에 있는 14. 6. 1절 't거 읽어 보71"에서 찾아볼 수 있다．


                                                                                     449 1
  Embedded Linux Primer




   $ ppc_44x-addr2line -e vmlinux 0xc020f41c
   arch/ppc/pl atforms/4xx/yosemi te . c :307



여기서 gdb는 우리가 설정한 브레이크 포인트가 yosemite - c 파일의 116번째 라인이라고
보고하고 있는데 , 왜 그런지를 이해하기 위해서 gdb7} 알려준 함수를 역 어셈블한 결과를 좀
들여다보자. ［리스트 1午8］은 yosemi七e se七up arch () 함수에서 gdb의 disasserr由le
명령어를 실행한 결과이다．

［리스트 14-8) yosem陀 setup_arch 함수의 역어셈을 결과

   (gdb) disassemble yosemite_setup_arch
  0xc020f41c <yosemite_setup_arch+0>:     mflr                       rO
  0xc020f420 <yosemi te_setup_arch+4> :    stwu                     ri, -48(nl)
  0xc020f424 <yosemi te_setup_arch+8> :   1i                        r4, 512
  0xc020f428 <yosemi te놔setup卜arch+12>:    ii                       r5,0
  0xc020f42c <yosemite_setup_arch+16> :    11                       r3 ,4116
  0xc020f430 <yosemite_setup_arch+20> :    stmw                      r25, 20(rl)
  0xc020f434 <yosemi te_setup_arch+24>:    stw                      r0, 52(rl)
  0xc020f438 <yosemite_setup_arch+28>:    bi                        0xC000d344
  <ocp_get_one_devi Ce>
  0xc020f43c <yosemi te_setup_arch+32> :  1wz                       r31, 32(r3)
  0xc020f 440 <yosemi te_setup_arch+36>:   u js                     r4 ! 小16350
  0xc020f 444 <yosemi te_setup寸arch+40>:  ii                        r28, 2
  0xc020f448 <yosemi te_setup_arch+44> :  addi                      r4, r4, 21460
  0XC020f44C <yosemi te_setup_arch+48> :  ii                        r5, 6
  0xc020f4 50 <yosemite_setup_arch+52> :  u js                      r29, -16350
  0xc020f454 <yosemi te_setup_arch+56>:   addi                      r3, r31, 48
  0xc020f458 <yosemi te_setup_arch+60> :  u js                      r25, -16350
  0xc020f45c <yosemi te寸setup_arch+64> :  bl                        0xc000C 708
  <memcpy>
  0xc020f 460 <yosemi te_setup_arch+68> : stw                       r28, 44 (r31)
  0xc020f464 <yosemi te_setup_arch+72> :                            r4, 512
                                                                1
                                                            ]
  0xc020f 468 <yosemi te_setup_arch+76> :                           r5,1
                                                        1
                                                    ]
  0xC020f46c <yosemi te_setup_arch+80>:                             r3, 4116
                                                1
                                            ]
  0xc020f470 <yosemi te_setup寸arch+84>:   addi                      r26, r25 ! 15104
  0xc020f474 <yosemi te_setup_arch+88> :  bi                        0xC000d 344
  <ocp_get_one_devi Ce>
  0xc020f478 <yosemi te_setup_arch+92>:   u js                      r4, -16350
                                                       커널 디버깅 가술       Chapter 14



  0xc020f47c <yosemi te_setup_arch+96>:     lwz     r31, 32 (n3)
  0xc020f480 <yosemi te_setup_arch+100> :   addi    r4, n4, 2 1534
  0xc020f484 <yosemi te_setup_arch+104> :   ii      r5, 6
  0xc020f488 <yosemi te_setup_arch+108> :   addi    r3, n31, 48
  0xc020148c <yosemi te_setup_arch+112> :   bl      0xc000c708
  <memcpy>
  0xc020f490 <yosemi te_setup_arch+116> :   u is    n4,1017
  0xc020f494 <yosemi te_setup_arch+120> :   Us      r5,168
  0xc020f498 <yosemi te_setup_arch+124> :   Stw     n28, 44(r31)
  0xc020f49c <yosemi te_setup_arch+128> :   oni     n4, n4,16554
  0xc020f4a0 <yosemite_setup_arch+132>:     oni     r5, r5, 49152
  0xc020f4a4 <yosemi te_setup_arch+136>:    addi    n3, r29, -15380
  0xc020f4a8 <yosemi te_setup_arch+140>:    addi    n29, r29, -15380
  0xc020f4ac <yosemi te_setup_arch+144>:    bi      0xc020e338
  <1bm440gx_get_cl ocks>
  0xc020f4b0 <yosemi te_setup_arch+148>:    li      rO , 0
  0xc020f4b4 <yosemite_setup_arch+152>:     Us      nil, -16352
  0xc020f4b8 <yosemi te_setup_arch+156>:    onj     nO, rO, 50000
  0xc020f4bc <yosemi te_setup_arch+160>:    lwz     riO, 12 (r29)
  0xc020f4c0 <yosemi te_setup_arch+164>:    Us      n9, -16352
  0xc020f4c4 <yosemi te_setup_arch+168>:    stw     nO, 8068(nli)
  0xc020f4c8 <yosemite_setup_arch+172>:     lwz     n0, 84(r26)
  0xc020f4cc <yosemi te_setup_arch+176>:    St닙     riO, 8136(r9)
  0xc020f4d0 <yosenii te_setup_arch+180>:   mtctr    rO
  0xc020f4d4 <yosemi te_setup_arch+184>:    bctrl
  0xc020f4d8 <yosemi te_setup_arch+188> :   ii      r5, 64
  0xc020f4dc <yosemi te_setup_arch+192> :   mn      r31, r3
  0xc020f4e0 <yosemi te_setup_arch+196> :   u js    r4, -4288
  0xc020f4e4 <yosemi te_setup_arch+200>:    ii      n3, 0
  0xc020f4e8 <yosemi te_setup_arch+204>:    bl      0xc000c0f8
  <ioremap64>
  End of assembler dump.
  (gdb)



여기서도 위 역어셈블된 내용이 어떤 일을 하는지 이해하기 위해 PowerPC 어셈블리 언어를
전부 알고 있어야 하는 것은 아니다. PowerPC의 명령어인 bi 옆에 연결된 레이블（lab이）
을 주의해서 보자. bi은 PowerPC에서 함수를 호출하는 니모닉（mn帥oni이이다. 여기서
심볼릭 함수 레이블은 아주 중요한 정보가 되는데 , 대충 분석해 보면 어셈블러 언어의 시작
부분 근처에서 몇 개의 함수가 호출되는 것을 볼 수 있다．


                                                                            451
   難U     Embedded Linux Primer




        주소                                      함수

        0xc020f438                              ocp_get_one_device0

        0xc020f45c                              memcpy0
        0xc020f474                              ocp_get_one_device()

        0xc020f48c                              memcpy0
        0xc020f4ac                              ibm440gx_get_clocks0


      ［리스트 14이는 yosemite .c 소스 파일에서 관련된 위치만 다시 출력한 것이다．
        yosemi七e Se七up arch () 어］ 설정한 브레이크 포인트를 만났을 때 gdb로 역어셈블한 내
        용에서 볼수 있는 함수를 종합하1 보면 이 레이블들이 yosemite se七 emacda七a () 함수에
        서 사용되고 있는 것을 알 수 있다. 이 현상을 이해하는 핵심은 yosemi七e setup arch ()
        의 시작 부분에서 서브루틴이 호출된다는 것이다． 즉, 소스 코드를 간단히 조사해 보면 예상
        할 수 있는 것처럼 , 컴파일러가 yosemi七e set emacdata (）를 호출하는 부분에서 실제
      함수 호출 대신에 그 함수 자체를 인라인16) 시켰다. 이러한 인라인 처리가 gdb가 브레이크
        포인트를 만났을 때 다른 위치를 가리키는 원인이었다. yosemi七e set emacdata () 함
      수가 inline 키워드로 선언되지 않았지만 GCC가 성능 최적화를 위해서 인라인 함수처럼 처
      리한 것이다.

      ［리스트 ]4-9) yosemite.c의 관련 코드


          109 static void _init yosemite_set_emacdata(void)
          110 {
          111        struct ocp_def *def;
          112        struct ocp_func_emac_data "'" emacdata;
          113
          114        /*' Set mac_addr and phy mode for each EMAC 央 /
          115
          116        def = ocp_get_one_device (OCP_VENDOR_IBM, OCP小FUNC.HEMAC, 0) ;
          117        emacdata = def->additions;
          118        memcpy (emacdata->mac_addr, _res. bi_enetaddr, 6) ;
          119        emacdata->phy_mode = PHY_MODE_RMII;
          120


16) （역자주） 함수가 호출되는 부분에 실제 그 함수 내용을 젼부 삽입해 버린 것
                                                     커널 디버깅 기술     Chapter 14



121         def = ocp_get_one_device(0cP_vENDOR卞IBM, OCP_FUNC_EMAC, 1) ;
122         emacdata = def->additions;
123         memcpy (emacdata->mac_addr, _res .bi_enetladdr, 6) ;
124         emacdata->phy_mode = PHY_MODE_RMII;
125 }
126

304
305 static void _init
306 yosernite_setup_arch(void)
307 {
308         yosemite_set_emacdataO;
309
310         ibm440gx_get_clocks (&clocks, YOSEMITE_SYSCLK, 6 * 1843200) ;
311        ocp_sys_info.opb_bus_freq = clocks. opb;
312
313         /* m it to some Nsane value until calibrate_delay () runs 女 /
 314         loops_per_ jiffy = 50000000/Hz;
 315
316          /* Setup PCI host bridge */
317          yosemite_setup_hoseO;
318
319 #ifdef CONFIG_BLK_DEV_INITRD
320        if (initrd_start)
321                ROOT_DEV = Root_RAMO;
322         else
323 #endif
324 #ifdef CONFIG_ROOT_NFS
325                 ROOT_DEV = Root_NFS;
326 #else
327                 ROOT_DEV = Root_HDA1;
328 #endif
329
330         yosemite_early_serial_mapO;
331
332         /* Identify the system 央/
333         printk ( "AMCC PowerPC " BOARDNAME " platform\n" );
334 }
335
 難1    Embedded Linux Primer



      지금까지의 내용을 정리해 보자．

       口 gdb에서 yosemite se七up arch () 함수에 브레이크 포인트를 설정했다．

       口 브레이크 포인트가 걸리면 소스 파일의 116번째 줄에 멈춰 있는 것을 볼 수 있는뎨, 이는
           브레이크 포인트를 설정한 코드 위치와는 완전히 동떨어진 위치이다．

       口 yosemite se七up arch () 소스 코드를 역어셈블했을 때 레이 블 들을 통해서 실제 어
           떤 순서로 코드가 호출되는지를 확인할 수 있었다．


      소스 코드와 역어셈블에서 볼 수 있는 레이블을 비교해 본 결과 컴파일러가 yosemite
      se七 emacdata () 서브루틴을 브레이크 포인트를 선언한 함수 안으로 인라인시켰다는 것
      을 알 수 있었고, 이것 때문에 잠제적인 혼란이 생겼던 것이다．

      이는 gdb7} 알려준 줄 번호가 원래 yosemite setup arch () 함수에 설정한 브레이크 포
      인트에 해당한다는 것을 설명해 준다．

      컴파일러는 다양한 종류의 최적화 알고리즘을 사용한다. 이 예제에서는 그중 한 가지인 함수
      를 인라인화하는 최적화를 알아보았다. 각각의 최적화가 각기 다른 방식으로 디버거를 혼란
      시키는데 , 어려운 부분은 기계어 레벨에서 어떤 일이 일어나고 있는지를 이해하고 이를 의도
      하는 방향에 맞게 해석하는 일이다. 이제 되도록 최적화를 적게 사용하는 것이 디버깅 작업
      에는 상당히 유리하다는 것을 이해할 수 있을 것이다．


14.3.3 gdb 사용자 정의 명령01
      gdl七 처음 시작할 때 . gdbinit이라는 초기화 파일을 찾는다는 것을 알고 있는 독자도 있
      을 것이다. gdb는 처음 실행되면 이 초기화 파일（보통은 사용자의 홈 디렉터리에 있다）을
      읽어 들여서 그 안에 기술된 명령어를 실행시킨다. 필자가 좋아하는 조합은 타깃 시스템에
      연결하는 명령과 기본 브레이크 포인트를 설정하는 명령어를 입력해 놓는 것이다. 이 경우
      .gdbini七의 내용은 ［리스트 1全10］과 같은 형태가 된다．

      C리스트 14-10] 간단한 9db 초7障｝ 파잎

         $ cat '/ .gdbinit
         set history save on
         set history filename N /.gdb_history
                                                    커널 디버깅 기술    Chapter 14


          set output-radix 16

          defThe connect
          #     target remote bcH: 2001
                target remote /dev/ttysO
                b panic
                b sys_sync
          end




       이 간단한 .gdbini七 파일이 하는 일은 사용자가 설정한 파일에 사용된 명령어에 대한 기록
       을 남기도록 설정하고 수 값을 표시할 때 기본으로 사용할 진법도 결정한다. 그리고는 gdb
       사용자 정의 명령으로 connect라는 명령어를 정의하고 있다（사용자 정의 명령어를 매크로라
       고 부르키도 한다）. gdl) 명령에 프롬프트에서 이 connect 명령을 실행시키면 gdb는 타깃
      시스템에 원하는 방식으로 연결해서 panic (）과 sys sync () 함수에 브레이크 포인트를
      설정한다. 연결 메서드 하나는 주석 처리가 되어 있는데 , 이 메서드는 14.4절에서 잠깐 살펴
      볼 예정이다．

      gdb 사용자 정의 명령어를 필요에 맞게 창의적으로 만들어 쓰는 데는 끝이 없다. 커널에서
      디버깅할 때 태스크의 목록이나 메모리 맵에 대한 자료 구조를 담고 있는 전역 변수를 검사해
      보는 기능이 종종 유용하게 사용된다. 여기서는 커널 디버깅 시에 필요할 만한 데이터를 출
      력하는 몇 가지 gd) 사용자 정의 명령어를 설명하도록 하겠다．


14.3.4 유용한 커널 gdb 매크로
      커널 디버깅 중에 현재 동작중인 시스템에 있는 프로세스에는 어떤 것들이 있고, 그 각각의
      프로세서의 일반적인 속성 값을 알고 싶을 때가 종종 있을 수 있다. 커널은 태스크에 대해서
      task struct라는 구조체를 연결 리스트의 형태로 유치하고 있다. 그리고 첫 번째 태스크
      에 대한 구조체의 주소는 커널의 전역 변수인 mnit task어］ 저장되어 있는데 , 이 변수는
      커널이 시작될 때 처음 실행되는 초기 태스크를 나타낸다. 각 태스크 구조체에는 uis七
      head라는 구조체를 다시 포함하고 있는데， 이 구조체는 원형 연결 리스트17）를 유지하는 데
      사용된다. 커널의 어디를 가나 볼 수 있는 이 두 개의 커널 구조체는 다음 헤더 파일에 정의
      되어 있다.

17) ［역자주） 연결 리스트의 맨 뒤에 있는 리스트가 다시 맨 잎의 리스트루 연결되면 논리적으로 원형을 이루게 된다. 그래서
                                                                       원형
    (circular) 연결 리스트라고 한다．
  Embedded Linux Primer




  struct task_struct            . . ./include/linux/ sched. h
  struct list_ head             . . ./include/linux/list. h




gdb 매크로를 이용하면 태스크 리스트를 탐색해 볼 수 있고, 유용한 정보도 출력해 볼 수
있다. 그리고 자신이 관심 있는 다른 정보를 추출해 내도록 매크로를 수정하는 것도 쉽게 할
수 있다. 또한 커널 내부에 대해서 자세히 공부할 때 유용하게 사용할 수도 있는 툴이다．

［리스트 14-11］에서 맨 처음 알아볼 매크로는 커널의 七ask struct 구조체의 연결 리스트
를 검사해서 찾고자 하는 태스크를 짖아 주는 간단한 매크로이다. 만약에 해당 태스크를 찾
았다면 그 태스크의 이름을 출력하도록 했다．

［리스트 ]4-1 ]] gdb find task 매크로

    1 # Helper function to find a task given a PID or the
    2 # address of a task_struct.
    3 # The result is set into St
    4 define find_task
    S # Addresses greater than _end: kernel data. . .




     6789mn끄Bk巧珀U始四加끄끄n
        # . . .user passed in an address
        if ( (unsigned) $argo > (unsigned)&_end)
          set $t=(struct task_struct *)sargo
        else
          # user entered a numeric PID
          # walk the task list to find it
           set St=&init_task
          if (init_task. pid 1= (unsigned) $argO)
              find_next_task St
              while (&init_task!=$t && St->pid 1.= (unsigned) SargO)
                find_next_task St
              end
              if (St == &init_task)
                printf "couldn 't find task; using init_task\n "
              end
           end
         end
         pri ntf "Task \"%s\" : \n", St->comm
    24 end
                                                      커널 디버깅 가술    Chapter 14



      이 내용을 .gdbinit 파일에 추가하고 gdb를 재시작하거나 gdk뙈 source'8) 명령어로 불
      러들이도록 하자（fin미next 七ask 매크로에 대해서는 나중에 ［리스트 14-15］에서 설명
      하도록 하겠다）. 그리고 다음과 같이 실행시키도록 한다．



          (gdb) find_ task 910
            Task "syslogd":




       또는




          (gdb) find_ task OXCFFDE470
            Task "bash":




       4번째 줄에는 매크로 이름을 정의하고 있다. 7번째 줄에는 입력된 인자가 PID(O에서 수백
      만 정도의 제한된 숫자）인지 또는 반드시 리눅스 커널 자체의 끝인 end19) 심볼보다 더 상
      위 주소에 있어야 하는 task 5七ruc七 주소인치를 판단하는 부분이다. 만약에 인자가 주소
      값이면 이 값을 올바른 형식으로 형 변환해서 七ask struc七 구조체를 참조할 수 있도록 한
      다. 이 내용이 8번째 줄에 해당하고, 3번째 줄에 있는 주석에서 볼 수 있듯이 이 매크로는
       task 就ruct라는 구조체에 대한 포인터를 gdb에서 편리하게 사용할 수 있는 변수 형식으
      로 변환해서 반환해 준다．

      만약에 입력된 인자가 숫자로 된 PT') 값이면 리스트를 탐색해서 일치하는 七ask s七ruct를
      찾게 된다. 12-13번째 줄에서 반복문을 위한 변수를 설정하고（gdb의 자체 macro 명령어
      언어에는 for 구문이 없다）, 15-17번째 줄에서 검색을 위한 루프를 선언하고 있다．
       fin寸next task 매크로는 연결 리스트에서 다음 task 5七ruc七를 가리키는 포인터를 얻
      기 위해서 사용된다. 검색이 실패하더라도 반환 값에 적당한 값（mnit 七ask의 주소）을 설정
      해서 다른 매크로에서도 안전하게 사용할 수 있도록 하고 있다．



18) 매크로를 개발할 때 유용하게 쓸 수 있는 명령이 바로 gdb source 명령이다. 이 명령어는 매크쿠를 담고 있는 소스 파일을 열
    어서 읽어들인다．
19) _end 심볼은 링크의 마지막 단계의 링커 스크립트 파일어］ 저장되어 있다．
          Embedded Linux Primer



        ［리스트 14-11］에 있는 find 七ask 매크로를 좀 더 발전시키면 시스템에서 실행중인 각
        프로세스에 대한 유용한 정보를 보여 주는 간단한 PS 명령을 쉽게 만들 수 있다．

        ［리스트 1午12］는 실행중인 프로세스에 대한 재미있는 정보를 七ask s七ruct 구조체에서
        추출해서 출력해 주는 매크로를 정의한 것이다. 이 명령은 다른 gdb 명령처럼 실행시키면
        되는데 , 명령에 이름과 필요한 인자를 입력하면 된다. 위 사용자 정의 명령어의 경우는 한
        개의 인자를 받는데 PT') 또는 task struc七의 주소가 그것이다．

        ［리스트 14-12) gdl) 매크로 : 프로세스 정보 표시

           1 define PS




            23456789mn끄
               # Print column headers
               task_struct_header
               set St=&init_task
              task_st ruct_show St
               find_next_task St
              # 닙alk the 거St
              while &init_task!=St
                 # Display useful info about each task
                 task；中struct_sho叫 $t
                  們nd_ne收_task St
               end
          13 end
          14
          15 document PS
          16 Print points of interest for all tasks
          17 end



        이 PS 매크로는 전에 살펴본 find task 매크로와 비슷한데 , 한 가치 차이점은 아무런 인자
        를 받지 않는다는 것과 각각의 task struct에서 유용한 정보를 출력하기 위해 다른 매크
        로仕ask struct show)를 사용하고 있다는 것이다. 3번째 줄은 각 행의 제목과 함께 배너
        를 표시해 준다. 令6번째 줄은 반복문을 만들고, 첫 번째 태스크에 대한 정보를 출력한다．
        小11번째 줄은 각각의 태스크를 반복해서 찾아 task struct show 매크로를 호출한다．

        그리고 gdb documen七 명령어도 포함되어 있는 것을 볼 수 있다. 이는 gdb 사용자가 다음
        과 같이 gdb 명령 프롬프트에서 help Ps 명령을 입력해 정보를 얻도록 하기 위한 것이다．



I 458
                                                    커널 디버깅 기술        Chapter 14




   (gdb) help ps
      Print points of interest for all tasks




［리스트 14-13］은 최소한의 서비스만 실행중인 타깃 보드 상에서 이 매크로를 실행한 결과
를 나타낸 것이다．

［리스트 ]4-13] gdb ps 매크로 실행 결과


   (gdb) Ps
  Address      PID State    User_NIP   Kernel-SP     device    comm
  0xC01D3750     0 Running             0xC0205E90    (none)    swapper
  OxC04ACB10     1 sleeping OxOFF6E85C 0xC04FFCE0    (none)    mn仇
  0xc04AC770     2 sleeping            0xC0501E90    (none)    ksoftirqd/0
  0xc04AC3D0     3 sleeping            OxC0531E30    (none)    events/0
  0xC04AC030     4 sleeping            OxC0533E30    (none)    khelper
  0xc04CDB30     5 sleeping            0xC0535E30    (none)    kthread
  0xC04CD790    23 sleeping            0xC06FBE30    (none)    kblockd/0
  0xC04CD3F0    45 sleeping            0xC06FDE50    (none)   pdflush
  OxC04CD050    46 sleeping            OXC06FFE50   (none)    pdflush
  0xC054B7B0    48 sleeping            0xc0703E30    (none)   aio/0
  0xC054BB50    47 sleeping            OxC0701E20   (none)    kswapd0
  0xC054B410   629 sleeping            OxC0781E60   (none)    kseriod
  0xC054B070   663 sleeping            0xCFC59E30   (none)    rpciod/0
  0xCFFDE0D0   675 sleeping OxOFF6E85C OXCF86DCEO   (none)    udevd
  OxCF95B110   879 sleeping 0x0FF0BE58 0xCF517D80   (none)    portmap
  0xcFC24090   910 sleeping OxOFF6E85C 0xCF61BCE0   (none)    syslogd
  0xCF804490   918 Sleeping 0x0FF66C7C 0xCF65DD70   (none)    klogd
  0xCFE350B0   948 sleeping 0x0FF0E85C 0xCF67DCE0   (none)    rpc. statd
  0xCFFDE810   960 sleeping 0x0FF6E85C OxCF5C7CEO   (none)     inetd
  0xcFC24B70   964 sleeping OXOFEEBEAC 0xCF64FD80   (none)    mvltd
  0xCFE35B90   973 sleeping 0x0FF66C7C 0xCFEF7CE0   ttysl     getty
  0xCFE357F0   974 sleeping 0x0FF4B85C 0xCF6EBCE0   (none)    in. telnetd
  0xCFFDE470   979 sleeping 0x0FEB6950 0xCF675DB0   ttypo     bash
  0xCFFDEBB0   982<Running  0x0FF6EB6C 0xCF7C3870   ttypo     sync
  (gdb)




                                                                         459f
          Embedded Lirux Primer



        이 PS 매크로가 하는 일의 대부분이 七ask小多七ruct아1O沆｝는 매크로에 의헤서 이루어지는
        데 , ［리스트 14-13］에서 보는것처럼 , task s七ruct show매크로는각七as느S七ruc七어］
        대해서 다음의 항목을 표시한다．

          口 Address : 프로세스의 task stri그C七 구조체의 주소

          口 PID : 프로세스 ID

          口 S七ate : 프로세스의 현재 상태

          口 User NIP : 사용자 영역에서 다음 실행할 명령에 주소

          口 Kernel SP : 커널 스택 포인터

          口 device : 프로세스와 연결된 장치

          口 comm : 프로세스（또는 명령어）의 이름


        커널 디버깅 작업에 따라서 관심 있는 부분을 보여 주도록 매크로를 수정하는 것은 상대적으
        로 쉽다. 유일하게 어려운 부분은 매크로 언어가 너무 간단하다는 데 있다. 즉, strien과
        같은 일을 해주는 함수들이 gdb의 사용자 정의 명령어를 위한 언어에는 존재하지 않기 때문
        에 직접 출력 형식을 만들어야 한다．

        ［리스트 14-14］는 이전 리스트에 나온 七ask s七ruct show 매크로의 내용을 나타낸 것이다．

        ［리스트 ]4-14) gdb의 task struct show 매크로

            1 define task1structHshow
            2 # tasLstruct addr and Plo
            3 printf "Ox%08X %5d", $argO, $argO->pid




            456789mn끄Bn
                          # Place a '< ' marker on the current task
                          # if (SargO == current)
                          # For PowerPC, register r2 points to the "current ' task
                          if ($argO == $r2)
                            printf "<"
                          else
                            printf " "
                          end

                          # State



毋 460
                                                    커널 디버깅 기술   Chapter 14



15  if ($argo->state == 0)
16    printf 'Running "
17 else
18    if ($arg0->state == 1)
19      printf "Sleeping "
20    else
21      if ($argO->state == 2)
22        printf "Disksleep
23      else
24        if ($argo->state == 4)
25          printf "zombie    "
26        else
27          if ($argo->state == 8)
28            printf "sTopped "
29          else
30            if ($argo->state == 16)
31              printf "wpaging   '
32            else
33              printf "%2d       ", $argo->state
34            end
35          end
36        end
37      end
38    end
39 end
40
41 # User NIP
42 if ($argo->thread. regs)
43    printf "0x%08X ' , $argo->thread. regs->nip
44 else
45    printf "
46 end
47
48 # Display the kernel stack pointer
49 printf "0x%08X ", $argo->thread.ksp
50
51 # device
52 if ($argo->signal->tty)
53    printf "%s ", $argO->signal->tty->name
54 else
55    printf " (none) "
56 end



                                                                     461 1
          Embedded Linux Primer



           57
           58   # comm
           59 pri ntf "%s\n", $ar90->comm
           60 end




        3번 줄은 七ask s七ruct 구조체의 주소를 표시한다. 그리고 小12번째 줄은 프로세스 ID
        를 출력한다. 그리고 현재 실행중인 프로세스일 경우에는（브레이크 포인트를 만났을 당시에
        실행되고 있던 프로세서 ID) < 문자가 표시된다．

        14-39번째 줄은 프로세스의 상태를 해석해서 표시해 주는 부분이다. 그 다음에 사용자 영
        역 프로세스의 다음 명령에 포인트（NIP : Next Instruction Pointer）와 커널 스택 포인터
        (SP）가 출력된다. 마지막으로 프로세스와 연결된 장치와 프로세스의 이름이 표시된다（프로
        세스 이름은 七as乂多truct의 ->comm 변수에 저장되어 있다）.

        중요한 것은 7- 8번째 줄에서 볼 수 있는 것처럼 이 매크로가 아키텍처에 종속적이라는 것이
        다. 일반적으로 이런 매크로들은 아키텍처나 특정 버전에 상당한 종속성을 갖는다. 그래서
        기반을 이루는 시스템이 변경될 때마다 이 매크로들도 그에 맞게 변경해 주어야 한다. 하지
        만 gdb를 이용해서 커널 디버깅에 상당한 시간을 보내는 사람이라면 그런 노력의 대가를 충
        분히 받을 것이다．

        find_next_task 매크로도 살펴보자. 구현된 내용이 그다지 이해가 쉽지 않기 때문혀］ 설
        명할 필요가 있다（이 섹션에서 설명한 PS 매크로가 동작하는 데 필요한 요소 중의 하나인
        task小struct上eader7} 무엇인지에 대해서 쉽게 추론할 수 있다. 이 요소는 각 열의 머리
        말에 정확한 너비만큼 공백 문자로 채워진 문자열 한 줄을 출력하는 일을 한다）. ［리스트
        1十15］는 PS와 find task 매크로에서 사용되는 fin寸next task 매크로를 보여 주고
        있다．

        ［리스트 ]4-15) gdb의 find next task 매크로


           define find_next_task
             # Given a task address, find the next task in the linked list
             set $t = (struct task_struct "D$argO
             set $offset=( (char *)&$t_>tasks - (char yD$t)
             set $t=(struct task_struct ') ( (char 六)$t->tasks next- (char *)$offset)
           end



黨 462
                                                                커널 디버깅 기술        Chapter 14




이 매크로가 하는 일은 아주 간단하다. 하지만 구현된 내용은 약간 이해하기 어렵다. 우선
이 매크로의 목적은 연결 리스트에서 다음 七ask s七ruc七를 가리키는 ->ne>＜七 포인터를 반
환하는 것이다. 하치만 task struct 구조체의 연결 리스트는 七ask 就ruct 구조체 내의
七asks라는 이름의 uis七 head 멤버를 이용해서 서로 연결되어 있다. 이는 연결 리스트에
서 다음 task s七ruc七 구조체를 가리키는 포인터를 직접 저장하는 일반적인 구현 방식과는
다르다. 그래서 ->next 포인터가 리스트의 다음 task struct 안에 있는 tasks 구조체
의 주소를 가리키기 때문에 七asks七ruct의 주소 값을 얻으려면 주소 값에서 얼마를 빼야
한다. 즉, 이 구조체를 가리키는 포인터 주소 값에서 七ask s七ruct 구조체의 시작 부분에서
tasks 구조체까지의 거리만큼을 빼야 한다. 이 매크로에서는 맨 처음 이 간격을 계산한 다
음 ->next 포인터의 값에서 이 간격만큼을 켸산해서 task 5七ruc七 주소를 가리키는 주소
를 얻어낸다. ［그림 14中5］를 보면 좀 더 명확할 것이다．


         task struct        (struct       task_struct "   )1\
            상태1                       task s甘uct
         쓰레드 정보                          상태                        task struct
           퓰래그                        쓰레드 정보                          상태
                                        플래그                       쓰레드 정보
              :.
                                                                     플래그
     +

         tasks . next
十＼
                                                                       1


                                                                       1

         tasks 니：)rey                 tasks . next                     1




             :                        tasks · prey                tasks. next
                                                                  tasks. prey



I 그림 14占 task 구조체의 리스트 연결


이제 다음 섹션에서 적재 가능한 모듈을 디버깅하는 방법을 설명할 때 유용하게 사용할 매크
로를 하나 더 알아보자. ［리스트 14-16］은 커널에 현재 설치된 적재 가능 모듈의 목록을 표
시해1 주는 간단한 매크로를 나타낸 것이다．
        Embedded Linux Primer



      ［리스트 ]4-16] 모듈 목록을 나열하는 gdl) 매크로

        1 define lsmod
        2 printf "Address\t\ tModule\n"
        3 set $nl=(struct 1-1st_head *)&modules
         4
         1
            set $done=O
         <
         J
            while ( !$done )
         戶
         b
              # list_ head is 4-bytes into struct module
         m
         /
              set $mp=(struct module O ((char *)$m1>next - (char *)4)
         8
              printf "Ox%08x\t%s\n", $mp, $mp->name
         0
         7
         0
              if ( $mp->list->next == &modules)
         d
         l
         4
         上
                  set k幻ne=1
         4
         l
         )
         (
                end
         4
         l
                set $m=$m->next
        13 end
        14 end
        15
        16 document lsmod
        17 List the loaded kernel modules and their start addresses
        18 end



      이 간단한 반복문은 커널의 전역 변수인 module에서부터 시작하는데 , 이 변수는 list
      head 구조체로서 적재 가능한 모듈의 연결 리스트의 시작점을 가리키고 있다. 유일하게 복
      잡한 부분은 ［리스트 1全15］에서 설명한 것과 같은 것인데 , uis七 head 구조체의 포인터
      에서 module이라는 구조체의 시작점을 가리키도록 갊을 빼야 하는 부분이다. 이 부분이 7
      번째 줄에서 이루어진다. 이 매크로는 모듈의 목록과 함께 module 구조체의 주소를 간단하
      게 나열해 준다. 다음은 실제로 실행시켜 본 예이다．



        (gdb) ismod
        Address        Module
        OxD1012A80     i p_conntrack_tftp
        OxD10105AO     ip_conntrack
        OxD102F9AO     loop
        (gdb) help ismod
        List the loaded kernel modules and their start addresses
        (gdb)




464
                                         커널 디버깅 기술   Chapter 14


    여기서 보여 준 것과 같은 매크로는 디버깅을 하는 데 상당한 도움을 주는 강력한 툴이 된다．
    이와 비슷한 방식으로 커널의 다양한 정보, 특히 연결 리스트 형식으로 되어 있는 주요 커널
    자료 구조와 같은 내용을 어떤 것이든 자신이 원하는 대로 접근할 수 있다. 응용 사례로는
    프로세스의 메모리 맵 정보, 모듈의 세부 정보, 파일 시스템 청보 그리고 타이머 리스트 정보
    등을 들 수 있겠다. 여기서 설명한 매크로를 바탕으로 더 발전시킬 수 있을 것이다．


14.3.5 적지I 가능 모듈 디버깅하기
    KGDB를 사용하는 가장 일반적인 이유는 적재 가능 커널 모듈, 즉 디바이스 드라이버를 디
    버깅하기 위해서이다. 적재 가능 모듈이 갖는 좀 더 편리한 특징 중의 하나는 대부분의 환경
    에서 디버깅을 위해서 매번 재부팅할 필요가 없다는 점이다. 즉, 디버깅 세션을 시작한 다음
    일부를 수정하고 재컴파일해서 , 커널을 전체 재부팅하는 시간낭비 없이 곧바로 모듈을 다시
    로드할 수 있다．

    적재 가능 모듈을 디버깅할 때 복잡한 부분은 모듈의 오브젝트 파일에 포함된 디버그 심볼
    정보에 접근하도록 하는 것이다. 적재 가능 모듈은 커널에 로드되는 시점에 동적으로 링크되
    기 때문에 오브젝트 파일에 포함된 심볼 정보는 심볼 테이블이 다시 수정되기 전까지는 쓸모
    가 없기 때문이다．

    이전에 커널 디버깅 세션을 위해서 gdb를 실행시켰던 예제를 다시 보자．

      $ ppc_4xx-gdb vmlinux

    이 명령은 개발 호스트 시스템에서 gcfl) 디버깅 세션을 실행시키고, 리눅스 커널 ELF 파일
    인 virilinux에서 심볼 정보를 읽어 들인다. 물론 이 파일에서는 적재 가능 모듈에 대한 심볼
   은 찾을 수 없다. 적재 가능 모듈은 별도로 컴파일되고 나중에 독립적인 ELF 오브젝트로
    링크되기 때문에 적째 가능한 모듈을 소스 코드 레벨에서 디버깅하려고 할 때는 모듈의 ELF
   파일에서 디버그 심볼을 읽어 와야 한다. gdb에는 이를 위해서 add-町沁兀1-file 명령을
   가치고 있다．

   add-symbol-file 명령은 지정한 오브젝트 파일에서 심볼을 읽어 들이는데 , 물론 해당 모
   듈이 이미 로드되어 있다고 가정한다. 하지만 여기서 닭이 먼저냐 달걀이 먼저냐 하는 문제
   에 직면하게 된다. 즉, 적재 가능한 모듈이 로드되고 모듈의 심볼 정보를 읽기 위해서
   add-syr吐）ol-file 명령을실행하기 전까지는 어떤 심볼 정보도 가치고 있지 않는데 , 모듈
磊R     Embedded 니flux Prin祀r




     이 이미 로드되고 나면 그 때는 모듈의 女 mnit과 관련퇸 함수에 브레이크 포인트를 설정하
     기에는 너무 늦은 시점이다. 왜냐하면 , 이 함수들이 벌써 실행되고 난 다음이기 때문이다．

     이 딜레마에 대한 해결책은 모듈이 링크되고 초기화 함수가 호출되기 전에 , 모듈을 로드하는
     일을하는커널 코드에 브레이크포인트를잡는것이다. 이 작업은 . . - /kernel/module. c
     에서 이루어진다. ［리스트 14-17］은 module .c 파일에서 관련된 부분을 다시 나타낸 것이다．

 ［리스트 14너7) module.c : 모듈 초기화



       1901            down (&noti fy_mutex) ;
       1902             notifi er_call_chain(&module_notify_list,   MoDuLE_STATE_COMING,
       mod) ;
       1903            바)(&noti fy_i仙t태）;
       1904
       1905            /* Start the module */
       1906            if (mod->init != NULL)
       1907                   ret = mod->initQ;
       1908            if (ret < 0) {
       1909                   /* mnit routine failed: abort. Try to protect us from
       1910                      buggy refcounters. 必 /
       1911                   mod->state = MODULE_STATE_GOING;




     모듈을 로드하기 위해서는 8장, "디바이스 드라이버 기초'에서 설명했듯이 다음과 같은 형식
     으로 modprobe 유틸리티를 이용한다．

        $ modprobe loop


     이 명령은 커널이 모듈을 로드하도록 특별한 시스템 콜을 호출하는데 , 모듈을 로드하는 것은
     module .c어］ 있는 sys mnit module () 에서부터 시작된다. 모듈이 커널 메모리에 로드되
     고 동적으로 링크되면 제어권이 커널에 있는 mni七 함수로 넘어간다. 이 부분이 ［리스트
     14-17］의 1906-1907번째 줄에 해당한다. 여기에 브레이크 포인트를 설정하자. 이렇게
     하면 심볼 파일을 gdb에서 로드하고, 모듈 내의 함수에 브레이크 포인트를 설정할 수 있다.
     이 과정을 리눅스 커널에 있는 루프빽 드라이버인 loop.ko를 이용해서 직접 해보도록 하
     자. 이 모듈은 다른 모듈과의 의존성이 전혀 없기 때문에 쉽게 실험해 볼 수 있다.
                                                    커널 디버깅 가술        Chapter 14



［리스트 1全18］은 1O아）.ko 디버깅을 시작하기 위한 명령어들을 보여 주고 있다．

［리스트 ]4-18] 모듈 디버깅 세션 : loop. ko


  1 $ ppc-linux-gdb --silent vmlinux
  2 (gdb) connect
  3 breakinst 0 at arch/ppc/kernel/ppc-stub.c:825
  4825      }
  5 Breakpoint 1 at OxcoOl6bl8: file kernel/panic. c, line 74.
  6 Breakpoint 2 at 0xc005a8c8: file fs/buffer. c, line 296.
  7 (gdb) b module.c:1907
  8 Breakpoint 3 at 0xc003430c: file kernel/module. c, line 1907.
  9 (gdb) c
  10 continuing.
  11 >>>> 여기서 커널이 부팅을 완료하도록 하고
  12      타깃에 ]oop. ko 모듈을 로드하도록 한다．
  13
  14 Breakpoint 3, sys_init_module (umod=0x30029000, len=0x2473e,
  15    uargs=0x10016338 ") at kernel/module. c:1907
  16 1907                   ret = mod->initQ;
  17 (gdb) ismod
  18 Address         Module
  19 0xD102F9A0      loop
  20 (gdb) set $m=(struct module *)OXD102F9AO.
  21 (gdb) p $m->module_core
  22 $1 = (void *) 0xd102c000
  23 (gdb) add-symbol-file ./drivers/block/loop.ko 0xd102c000
  24 add symbol table from file ". /drivers/block/loop. ko" at
  25         .text_addr = 0xd102c000
  26 (y or n) y
  27 Reading symbols from /home/chr朽/ sandbox/linux-2. 6.13-anicc/
  drivers/block        /loop.ko. . .done.



2번째 줄에서부터 초반에 ［리스트 1午1이에서 만들었던 gdb 사용자 정의 매크로인
connect를 이용해서 타깃 보드에 연결하고 초기 브레이크 포인트를 설정한다. 그 다음에
7번째 줄에서 보는 것처럼 module. c에 브레이크 포인트를 추가하고 continue 명령 (c)
을 내린다. 이제 커널이 부팅 과정을 마치면 七elnet으로 타깃에 연결해서 loop.ko 모듈을
로드한다（위에 표시하지는 않았다）. 루프빽 모듈이 로드되는 순간 바로 브레이크 포인트
#3이 걸리는데 , gdb는 14에서 16번째 줄에 있는 것과 같은 정보를 표시해 준다．
 難1 1     Embedded Linux Primer




        이 시점에서 이제 리눅스 커널이 모듈의 . text 섹션을 어느 위치에 링크시켰는지 찾아내야
        한다. 리눅스는 이 주소를 모듈에 대한 정보를 담고 있는 구조체인 module의 module
        Core   요소에 저장하고 있다. ［리스트 14-16］에 있는 lsmod 매크로를 이용해서 우리
        loop.k(> 모듈에 해당하는 module 구조체의 주소를 얻을 수 있다. 이 부분이 17-19번째
        줄에 해당한다. 이제 이 module 구조체 주소를 이용해서 module 구조체 내의 module
        core라는 멤버를 통해서 모듈의 . te>＜七 주소가 어디인지를 알아내도록 한다. 이 주소 값을
        gdb의 add-symbol-fi le 명령에 전달하면 gdb에서 내부 심볼 테이블을 실제 모듈이 커
        널에 링크된 주소와 맞도록 수정할 때 이 주소 값을 이용할 수 있게 된다. 여기서부터는 모듈
        에 브레이크 포인트를 잡고, 코드를 한 단계씩 실행시키거나 값을 검사하는 등의 작업을 평
        소와 다름없이 진행할 수 있다．

        이제 루프백 모듈의 초기화 함수에 브레이크 포인트를 설치해서 모듈의 초기화 코드를 한 단
        계씩 실행시키는 예를 보는 것으로 마무리하도록 하자. 이때 복잡한 부분은 커널이 모듈 초
        기화 코드를 로드할 때 별도로 할당된 메모리 공긴에 로드시켜서 초기화 코드가 실행되고 난
        후에는 재사용을 위해서 그 메모리를 해제한다는 점이다. 5장, "커널 초기화'에서                              init
        매크로를 설명했을 때를 다시 상기해 보자. 이                             mni七 매크로20）는 컴파일러 속성 값을 지
        정하는 일을 하는데, 링커로 하여금 이 표시가 있는 함수를 특별한 이름을 가진 별도의 ELF
        섹션에 위치시킨다. 본질적으로 어느 함수든 이 속성으로 정의되면 . init. te＞比라는 이름
        의 섹션에 위치하케 된다. 사용법은 다음과 같다.

          Static mnt H init       loopinit   (void) {. . .}


        이렇게 선언하면 컴파일된 loop m1li七 () 함수는 loop.ko 오브젝트 모듈의 .init. te그＜七
        섹션에 위치하게 될 것이다. 모듈이 로드되면 커널은 모듈의 본체를 위한 메모리 덩어리를
        할당하는데, module 구조체에서 module core7} 이 주소를 가리키고 있다. 그 다음에는
        별도의 메모리 덩어리를 할당해서 . init. te)＜七 섹션을 처장한다. 초기화 함수가 호출되고
        난 후에 커널은 이 초기화 함수가 로드되어 있는 메모리를 해제한다 오브젝트 모듈이 이런
        식으로 분리되어 있기 때문에 gdb7} 이러한 상황을 인식하도록 해 주어야 초기화 함수를 디
        버깅21）할 때 심볼 데이터를 이용할 수 있다．［리스트 1士19］에서 이 과정을 볼 수 있다．


20) （역자주） 이 매크로는 C 언어의 #define을 이용한 매크로이다. gdb의 사용자 정의 매크로가 아님을 주의하자．
21) 이 글을 쓰는 시점에는 gdb꽤 작은 버그가 있어서 이 방법이 올바로 동작하지 않았다. 독자가 이 글을 읽고 있을 때는 수정되
    었길 d봔다．
                                                          커널 디버깅 기술       Chapter 14



［리스트 ]4-19] 모듈 초기화 코드 디버깅하기


  $ ppc_4xx-gdb -slient vmlinux
  (gdb) target remote /dev/ ttySO
  Remote debugging using /dev/ttySO
  breakinst 0 at arch/ppc/kernel/ppc-stub. c: 825
  825    }

  << 모듈의 mnit을 부르기 전에 브레이크 포인트를 설정함 >>
  (gdb) b module.c:1907
  Breakpoint 1 at 0xc0036418: file kernel/module. c, line 1907.
  (gdb) C
  Continuing.

  Breakpoint 1, sys_i ni tmodu1e (umod=0xd102ef40, 1en=0x2 3cb3, uargs=0x10016338 ")
  at kernel/module. c:1907
  1907                     ret = mod->initQ;

  << module 구조체를 통해서 초71 주소를 얻음 >>
  (gdb) ismod
  Address           Module
  0xD102EF40        loop
  (gdb) set Sm=(struct module *)OxD102EF40
  (gdb) p Sm->module_core
  $1 = (void *) Oxdl02b000
  (gdb) p Sm->module_init
  $2 = (void *) 0xd1031000
  << core와 i nit 주소를 이용해서 심볼 파일을 로드함 >>
  (gdb) add-symbol-file ./drivers/block/loop.ko 0xd102b000 -s .init. text
  0xd1031000
  add symbol table from file ". /drivers/block/loop. ko' at
          .text_addr = 0xd102b000
          . init. text_addr = 0xd1031000
  (y or n) y
  Reading symbols from /home/chris/sandbox/linux-2. 6. 13
  amcc/drivers/block/loop.ko. . .done.
  (gdb) b loop_mnit
  Breakpoint 3 at 0xd1031000 file drivers/block/loop. c, line 1244.
  (gdb) C
  Continuing.

  << 브레이크 포인트를 만남， 모듈의 in卄 함수를 디버그하도록 게속 진행시킴 >>
   難1     Embedded Linux Primer



          Breakpoint 3, 0xd1031000 in loop_mnit 0 file drivers/block/loop.c, line 1244
          1244       if (max_loop < 1 I I max_loop > 256) {
          (gdb)




14.3.6 printk 디버깅
        커널과 디바이스 드라이버 코드를 prin七k를 이용해서 디버깅하는 것도 많이 사용하는 방법
        이다. 이는printk7下 상당히 안전한 함수이기 때문이다. 즉, printk 함수는 인터럽트 핸들
        러까지도 포함해서 거의 모든 곳에서 호출할 수 있다. printk는 친숙한 （그 라이브러리 함수
        인 printf (）의 커널 버전이며 . . . /kernel/prin七k. c어］ 함수가 정의되어 있다．

        디버킹을 위해서 prin七k를 이용하는 방법이 갖는 한계를 이해하는 것이 아주 중요하다. 먼
        저 printk는 콘솔 장치를 필요로 한다. 더구나 콘솔 장치가 커널 초기화 과정에서 최대한
        빨리 활성화되도록 설정한다 하더라도, 콘솔 장치가 아직 초기화되기 전에 prin七k 함수가
        수도 없이 호출된다. 이 한계를 넘어서는 방법에 대해서는 14.5절 "부팅이 되지 않을 때"에서
        제시하도록 하겠다．

        printk 함수는 출력하는 메시지의 중요도를 나타내는 표시를 추가할 수 있다．
        . . . /include/linux/kernel.h 헤더 파일에 다음 여덟 가지 단계가 정의되어 있다．



          #define        KERN1EMERG   "<0>"    /士 system is unusable */
          #define        KERN_ALERT   "<1>"    /骨 action must be taken immediately */
          #define        KERN_CRIT    "<2>"    /士 critical conditions */
          #define        KERN_ERR     "<3> "   /士 error conditions */
          #define        KERN_WARNING "<4>"    /肯 warning conditions */
          #define        KERN_NOTICE "<5>"     /* normal but significant condition */
          #define        KERN_INFO    "<6>"    /士 informational */
          #define        KERN_DEBUG   "<7>"    /* debug-level messages '"" /



        간단한 prin七k 메시지는 다음과 같이 출력할 수 있다．

          printk ("fooQ entered w/ %s\n", arg) ;




I 470
                                                        커널 디버깅 기술   Chapter 14



    만약에 중요도 문자를 무시하면 커널이 printk.c에 정의된 기본 값으로 중요도 레벨을 설
    정한다. 최신 커널의 경우에는 레벨 4, 즉 KERN WARNING이 기본 값이다. 자신이 원하는
    중요도 레벨을 지정해서 printk를 호출하려면 다음과 같이 하면 된다．

      printk (KERN_CRIT "vmafloc failed in fooO\n") ;

    기본적으로 printk에서 지정한 로그 레벨 이하로 출력되는 메시지는 모두 시스템의 콘솔 장
    치에 출력되게 되어 있다. 이 기본 로그 레벨은prin七k.c에 정의되어 있는데 ，최신 리눅스
    커널은 이 값이 7이다. 이 말은 KERN DEBUG보다 중요한 모든 printk 메시지들은 콘솔에
    출력된다는 의미이다．

    다양한 방법으로 기본 커널 로그 레벨을 바꿀 수 있는데 , 부팅 시에 타깃 보드의 기본 로그
    레벨을 설정하기 위해서 커널 커맨드 라인 파라미터로 전달할 수도 있다. main. c에 기본
    로그 레벨을 결정하는 데 영향을 주는 커널 커맨드 라인 옵션이 세 711 존재한다．

      [a 콘솔 로그 레벨을 10으로 설정하는 debug 옵션

      口 콘솔 로그 레벨을 4로 설정하는 qiiiet 옵션

      口 직접 원하는 값을 로그 레벨로 지정하기 위한 loglevel= 옵션

    debug 옵션을 이용해서 모든 printk 메시지를 출력하게 만들 수도 있고, quiet를 이용해
    서 중요도가 KEPJ寸ER1之 또는 그 이상인 메시지만 출력되게 할 수도 있다．

    printk 메시지는 타깃 보드 또는 네트워크에 있는 파일에 저장되게 할 수도 있다. kiogd
    （커널 로그 데몬）와 syslogd（시스템 로그 데몬）를 이용해서 printk 메시지를 저장하는
    것을 결정할 수 있다. 이 유틸리티들에 대한 자세한 내용은 맨 페이지나 리눅스 참고 서적을
    보도록 하고, 여기서는 그냥 넘어가자．


14.3.7 매직 SvsReq 키
    이 방법은 미리 정해진 특수 키의 조합을 이용해서 커널에 직접 메시지를 보내는 방법으로
    디버깅을도와준다. 대부분의 아키텍처와보드에서 기본적으로시리얼 포트나 간단한 터미널
    에뮬레이터를 시스템 콘솔로 사용하는데1, 이 경우에는 매직 SysReq 키가 브레이크 문자가
    오고 바로 다음에 명령에 문자가 오도록 되어 있다. 자신이 사용하는 터미널 에뮬레이터에서



                                                                          471 1
 難1 1    Embedded Linux Primer




        브레이크 문자를 어떻게 보내는지는 사용하는 에뮬레이터 문서를 참고하도록 하자. 많은 리
        눅스 개발자가 터미널 에뮬레이터로 minicom을 사용하는데 , minicom의 경우에는 Ct'小
        F를 입력해서 브레이크 문자를 보낼 수 있다. 브레이크 문자를 보낸 후에는 5초 안에 명령어
        문자를 입력해야 한다．

        이 유용한 커널 툴은 개발 및 디버깅 과정에서 상당히 유용하게 쓸 수 있다. 하지만 데이터를
        읽어버리거나 시스템이 충돌할 수도 있다. 특히 b 명령에 문자는 아무런 경고나 준비 없이
        시스템을 바로 재부팅시켜 버린다. 열려있던 파일들은 닫히지 않은 상태에 , 디스크는 동기화
        가 되지 않았고, 파일 시스템이 마운트되지도 않는다. 재부팅하라는 명령인 (b) 명령키가 눌
        리면 순식간에 제어권이 바로 자신의 아키텍처의 리셋 벡터로 넘어가게 된다. 이 강력한 툴
        을 쓸 때는 이런 위험은 스스로 감수해야 할 것이다．

        이 기능에 대해서는 리눅스 커널 문서 하위 디렉터리에서 sysrq．七＞<t 파일에 잘 정리되어
        있다. 이 파일에서 다양한 아키텍처에 대한 자세한 세부 내용은 물론이고 사용할 수 있는 명
        령 문자에 대해서도 정보를 얻을 수 있다．

        예를 들어 , 방금 설명했던 커널 로그 레벨을 설정하는 다른 방법으로 매직 SysReq 키를 사
        용할 수도 있다. 이 명령 문자는 숫자 0에서 9까지인데 , 각 숫자에 해당하는 로그 레벨을
        기본 레벨로 설정하게 해 준다. minicom에서 Ctrl-A F를 누른 다음에 숫자를, 예를 들어
        9를 누르면 된다. 그렇게 했을 때 터미널에는 다음과 같이 출력될 것이다．



          $ SysRq : changing Loglevel
             Loglevel set to 9




        그 외에 명령 문자로는 레지스터의 내용을 덤프해 보는 기능이나, 시스템을 종료시키는 명
        령 , 시스템 재부팅시키기 , 프로세스 목록 나열하기 , 현재 메모리 정보를 커널에 출력하기 등
        다양하다. 더 자세한 내용은 최신 리눅스 커널에 포함된 문서 파일을 참고하기 바란다．

        이 매직 SysReq 기능은 주로 어떤 문제 때문에 시스템이 멈추었을 때 사용한다. 또한 정지
        해 버린 시스템에서 어떤 정보를 얻으려고 하는 경우에도 유용하게 사용된다．




I 472
                                                         커널 디버깅 기술   Chapter 14




14.4 하드웨어를 이용한 디버깅
      이제는 KGDB를 이용해서 커널 시작 코드의 아주 초기 단계를 디버깅하는 것은 불가능하다
      는 것을 이해할 수 있을 것이다. 이는 최소한 저수준의 하드웨어 초기화 코드가 실행되기 전
      까치는 KGDB가 초기화되어 있지 않기 때문이다. 더군다나 독자가 섀로 만든 보드에 시스템
      을 올리거나, 부트로더나 리눅스 커널을 포팅하는 일을 하고 있다면 하드웨어 디버그 장비는
      보드를 포팅하는 초기 단계에 문제점들을 디버깅하는 데 있어서 의심할 여지없이 가장 효율
      적인 개발 도구가 된다.

      하드웨어 디버그 장비는 종류가 매우 많다. 이 섹션에서는 아바트론에서 만든 BDI-2000
      (www.abatron.ch 참고）을 사용해보자. 이 장비는 보통 JTAG 프로브라고도 부르는데 이
      는 최초에 IC 바운더리 스캔을 검사하기 위해서 JTAG(Joint Test Action （打oup）에서
      정의한 저수준 통신 방식을 이용한 데서 유래된 이름이다.

      JTAG 프로브는 작은 커넥터를 이용해서 타깃 보드와 연결되도록 되어 있는데 , 이 연결 케이
      블은 양 끝단이 간단한 사각형 핀 헤더로 만들어져 있는 리본 케이블22) 형태로 되어 있다．
      대부분의 최신 고성능 CPU에는 JTAG 인터페이스를 지원하도록 설계되어 있어서 소프트웨
      어 디버깅 기능을 사용할 수 있도록 해 준다. JTAG 프로브는 이 CPU JTAG 인터페이스에
      연결하고 JTA（羽 다른 쪽은 호스트 개발 시스템에 이더넷이나 USB 또는 병렬 포트를 이용
      해서 연결한다. ［그림 14-6］은 아바트론 장치를 구성한 모습이다．

                                  이더넷 허브         JTAG 프로브




           호스트 시스템1
      I 그림 14七 하드웨어 JTAG 프로브를 이용한 디버깅


22) （역자주） 병렬 (PATA) 하드 디스크를 연결하는 케이블 형태를 리본 케이블이라고 한다．
          Embedded Linux Primer




        JTAG 프로브를 이용해서 디버킹을 할 수 있는 환경을 갖추는 일은 복잡한 작업일 수 있는
        데 , 이는 JTAG가 연결되는 Cpu가 복잡하기 때문이다. 타깃 보드에 전원이 인가되고 CPU
        가 리셋에서 깨어나면 아무것도 초기화되어 있지 않은 상태인데 , 사실 대부분의 프로세서에
        서 실제로 어떤 일을 하기 전에 최소한의 초기화는 이루어져야 한다. 이렇게 CPU를 초기
        설정하기 위해서 다양한 방법을 사용할 수 있는데 , 어떤 CPU는 전원 공급 후의 상태를 얻기
        위해서 특정 핀에서 하드웨어中구성 값 또는 초기 값을 읽도록 되어 있다. 그 외 CPU 중쇄는
        플래시 메모리와 같은 간단한 비휘발성 장치의 특정 위치에서 값을 읽어서 사용하는 것도 있
        다. 새로운 보드를 JTAG 프로브를 이용해서 디버깅을 할 수 있는 상태로 만들기 위해서는
        최소한의 CPU 또는 보드 레벨의 초기화가 먼저 이루어져야만 하고, 그 이후에야 다른 일을
        진행할 수 있다. 그래서 많은 JTAG 立쿠닙7} 보드 및 CPU 초기화하기 위해서 구성 파
        일23）을 이용한다.

        아바트론 장비도 연결된 타깃 하드웨어를 초기화하는 것은 물론이고 디버거의 동작을 설정하
        기 위한 파라미터를 정의하는 것도 구성 파일을 이용한다. 이 구성 파일은 CPU, 메모리 시
        스템 , 그 외 보드의 하드웨어를 초기화하는 명령어를 가지고 있다. 자신의 보드에 맞게 이
        구성 파일을 알맞은 명령을 이용해서 수정하고 최적화하는 일은 개발자의 몫이다. 구성 파일
        에서 사용할 수 있는 명령어에 대한 문법은 JTAG 프로브 툴에 포함된 문서를 참고해야 한
        다. 하치만, 오직 임베디드 개발자만이 자신의 보드를 위해서 필요한 구성 파일을 만들 수
        있기 때문에 CPU와 보드 레벨의 자세한 설계 사항을 이해하고 있어야 한다. 새로운 보드에
        자체적으로 리눅스를 포팅하는 것과 거의 비슷하게 이 작업도 지름길이나 차선책 같은 것이
        없다．

        부록 F, "예제 BDI小2000 구성 파일"에서는 프리스케일 반도체의 MPC5200 임베디드 컨트
        롤러를 위한 자체 보드에서 사용할 아바트론 구성 파일의 내용을 볼 수 있다. 이 부록에서
        이 자체 제작된 보드를 설정하기 위해서 필요한 내용을 볼 수 있는데 , 파일 내에 다앙한 레지
        스터와 초기화 작업을 설명하는 주적들을 자유롭게 달아놓았다. 이렇게 함으로써 내용을 갱
        신하고 유지하는 것을 더 용이하게 할 수 있고, 내용을 처음 접할 때도 그 의미를 바르게 이
        해하는 데 도움이 된다．




23) ［역자주） 국내에서 많이 사용되는 IRACE32나 야光nIce와 같은 툴에서는 口nnK기라는 확장자를 갖는 스크립트 파일을 이용해서
    보드를 초끼화한다． 그 외 각 디버거도 자신만의 스크립트를 이용해서 기본적인 보드 초기화를 하는 것이 기본 절차이다．


I 474
                                           커널 디버깅 기술   Chapter 14




    하드웨어 프로브는 일반적으로 두 가지 방법으로 사용되는데 , 대부분의 경우 개발자가 프로
    브의 기능을 사용할 수 있게 해 주는 사용자 인터페이스를 제공한다. 이런 인터페이스의 예
    로는 플래시를 프로그램하거나 바이너리 이미지를 다운로드하는 등의 작업을 들 수 있다. 두
    번째 방법은 gdb 등의 소스 레벨 디버거 프론트 앤드를 이용하는 것이다. 이제 두 가지 방식
    을 모두 알아보도록 하자．


14.4.1 JTAG 프로브를 이용해서 푤래시 키록하키
    많은 하드웨어 豆르 13가 다양한 종류의 플래시 칩을 프로그래밍하는 기능을 가지고 있다. 아
    바트론 BDI-2000 역시 예외가 아닌데 , BDI-2000 구성 파일에는 [FLASH] 섹션이 있어서
    타깃에 있는 플래시의 특성을 정의할 수 있게 되어 있다. 부록 F에 있는 예제를 참고하도록
    하자. [FLASH] 섹션은 특정한 보드에 있는 플래시 칩의 속성을 정의하는 일을 하는데 , 예를
    들어 칩의 종류나 장치의 용량 그리고 데이터 버스의 너비 등을 정의할 수 있다. 또한 메모리
    에 매핑된 위치 , 칩의 저장 단위가 어떻게 구성되어 있는지에 대해서도 기술할 수 있다.

    플래시의 일부분을 업데이트하는 경우에 , 다른 부분에 있는 내용은 그대로 보존시켜야 할 때
    가 종종 있는데 , 이 경우를 위해서 하드웨어 프로브에 삭제할 섹터 수를 지정할 수 있는 기능
    이 있어야 할 것이다. 아바트론 장비의 경우 삭제할 각 섹터에 대해서 ERASE라는 키워드로
    시작하는 한 줄을 추가하면 된다. 그래서 텔넷 인터페이스로 아바트론 장비에 erase 커맨드
    를 내리면 ERASE라고 표시된 섹터만 모두 삭제된다. ［리스트 14小20］에는 플래시의 일부를
    삭제하고 거기에 새로운 U-Boot 부트로더 이미지를 프로그램하는 작업을 예로 보여 주고
    있다．

   ［리스트 ]4-20] 플래시 삭제 및 프로그램


      $ telnet bdi
      Trying 192.168.1.129. . .
      connected to bdi (192.168.1.129) .
      Escape character is 'A] '
      8D1 Debugger for Embedded PowerPC

           (large volume of help text)

      uei> erase
      Erasing flash at 0xfff00000



                                                            "s 1
客 磁R    Embedded Linux Primer




         Erasing flash at Oxfff10000
         Erasing flash at 0xfff20000
         Erasing flash at 0xfff30000
         Erasing flash at 0xfff40000
         Erasing flash passed
         uei> prog Oxfff00000 u-boot.bin BIN
         Programming u寸）oot.bin , 이ease 叫a卄 . . . .
         Programming flash passed
         uei>



       맨 처음 아바트론 BDI-2000에 텔넷 연결을 맺는다. 일부 초기화 작업 후에 명령에 프롬프
       트를 볼 수 있는데 , 여기에 erase 명령을 내리면 아바트론은 구성 파일에 정의된 각 섹션에
       대해서 진행 사항을 출력한다. 부록 F에 있는 구성 파일에는 모두 다섯 개의 삭제할 섹터가
       기술되어 있다. 이는 총 256KB에 달하는 공간을 U寸Boot 부르로더 바이너리를 위해서 예약
       해 두는 것이다．

       위에서 prog라는 명령이 세 개의 인자와 함께 사용된 것을 볼 수 있다. 각 인자는 새로운
       이미지를 불러올 메모리 주소 값과 이미지 파일의 이름 그리고 파일의 형식을 각각 나타낸다．
       이 경우에는 바이너리 파일 형식이다. 이들 파라미터를 BDI-2000 구성 파일에도 설정할 수
       있는데 , 이렇게 하면 간단히 prog 명령을 인자 없이 실행할 수 있다．

       이 예제에서는 BD卜2000의 다앙한 명령에 중에서 두 가지만 잠깐 살펴본 것이다. 실제로는
       더 다양한 기능을 활용할 수 있다. 이렇게 각각의 하드웨어 JTAG 프로브는 자체적으로 플래
       시를 지우고 프로그램하는 기능을 제공한다. 독자가 사용하는 장비에 대해서는 관련 문서를
       참고하도록 하자．


14.4.2 JTAG 프로브를 이용한 디버깅
       JTAG에서 자체적으로 제공하는 인터페이스 대신에 , 소스 레벨 디버거를 이용해서 JTAG
       立로브를 사용할 수도 있다. 단연 하드웨어 立쿠 1크가 지원하는 가장 인기 있는 디버거는 gdb
       디버거이다. 이 경우에 gdb를 타깃 시스템과 외부 연결을 통한 디버그 세션을 이용하도록
       설정하는데 , 일반적으로 이더넷 연결을 많이 사용한다. 사용자 인터페이스에서 JTAG 프로
       브와 직접 통신하는 대신에 , 디버커가 자기 자신과 JTAG 프로브 사이에서 명령을 주고받도
       록 되어 있다. 이 모델에서 JTAG 프로브는 gdt뙈 연결 프로토콜을 통한 명령어를 받아들여


i476
                                                  커널 디버깅 기술   Chapter 14



      서 디버거 자체의 기능을 실행시키게 된다. ［그림 14-6］에서 세부 연결 상태를 다시 보도록
      하자．

      JTAG 프로브는 부트로더나 기타 초기 스타트업 코드를 디버깅할 때 특히 유용하게 사용할
      수 있다. 이 예제에서는 gdl佇｝아바트론 BDI-2000을 이용해서 PowerPC 타깃 보드에서
      동작하는 U-Boot 부트로더를 일부 디버깅해 보도록 하자．

      많은 프로세서가 디버깅 레치스터를 가지고 있어서 기존 방식인 주소 브레이크 포인트（프로
      그램이 특정 주소에 도달했을 때 정지）는 물론이고 데이터 브레이크 포인트（특정 메모리 주
      소에 접근하는 조건을 검사해서 정지）도 지원한다. 만약에 디버킹할 코드가 플래시와 같은
      읽기1전용 메모리에 있는 경우라면 이 레지스터를 이용해서 브레이크 포인트를 설정하는 방
      법이 유일24）하다. 하지만 이 레치스터는 그 수가 한정되어 있다. 대부분의 경우 하나 또는
      두 개 정도만 가치고 있는데 , 하드웨어 브레이크 포인트를 사용하기 전에 이러한 한켸 사항
      을 미리 이해하고 있어야 한다. 다음 예제에서 이 내용을 확인해 보자，

     ［그림 14-6］에 있는 구성을 이용한다고 했을 때 U-Boot가 타깃 보드의 플래시에 저장되어
      있다고 가정해 보자. 7장에서 부트로더에 대해서 알아봤을 때 t尸Boot 또는 기타 부트로더
      가 실행되자마자 일반적으로 자기 자신을 RAM에 복사하도록 되어 있다고 했다. 이는 일반
      적으로 플래시와 같은 읽기 전용 장치를 통한 읽기（또는 쓰기） 사이클보다 RAM이 수십 배
      는 더 빠르기 때문이다. 이런 문제들로 인해서 디버깅에 두 가지 난점이 발생하는데 , 그 중
      하나는 읽기 전용 메모리는 （소프트웨어 브레이크 포인트를 삽입하기 위해서） 그 내용을 변
      경할 수 없다는 것이다. 그래서 반드시 프로세서가 제공하는 하드웨어 브레이크 포인트를 이
      용해야 한다．

      두 번째 난점은 gdb7下 디버깅 심볼 정보를 읽어 올 때 ELF 실행 파일이 두 가치 실행 문맥
      （플래시 또는 RAM) 중에서 하나만 표현할 수 있다는 것이다. 口Boot의 경우에는 처음에
      저장되는 플래시 환경에 맞게 링크되어 있다. 하지만 초기 시작 코드가 스스로를 재배치시켜
      서 주소를 채조정한다. 이 말은 gdb7} 두 가치 경우 모두를 인식할 수 있도록 하는 작업이
      필요하다는 의미가 된다. ［리스트 14-21］을 보면 이와 같은 경우의 예를 볼 수 있다．




24) （역자주） 수五트웨어 브레이크 포인트는 코드를 특수한 명령으로 대체하는 방식인데, 읽기 젼용 메모리에서는 그런 작업이 불
  가능하기 때문해 하드웨어 브레이크만 사용할 수 있다．


                                                                   477 I
          Embedded Linux Primer



        ［리스트 14-21) JTAG 프로브로 나Boot 디버깅하71


          $ ppc-linux-gdb --silent u-boot
          (gdb) target remote bdi :2001
          Remote debugging using bdi: 2001
          _start 0 at /home/chris/ sandbox/u-boot-1.1. 4/cpu/mpc5xxx/start. S: 91
          91       li     r21, BOOTFLAG_COLD /* Normal Power-On "" /
          Current language: auto; currently asm

          << 플래시에 위치한 코드를 디버깅하기 >>
          (gdb) mon break hard
          (gdb) b board_mnit_f
          Breakpoint 1 at 0xfff0457c: file board. c, line 366.
          (gdb) C
          Continuing.

          Breakpoint 1, board. .init_f (bootflag=0x7fc3afc) at board. c: 366
          366            gd = (gd_t *) (CFG_INIT_RAM_ADDR + CFG_GBL_DATA_OFFSET) ;
          Current language: auto; currently c
          (gdb) bt
          #0 board_mnit_f (bootflag=Oxl) at board. c: 366
          #1 0xfff0456c in board_伯it_f (bootflag=Oxl) at board.c: 353
          (gdb) i frame
          stack level 0, frame at Oxf000bf50:
           pc = 0xfff0457c in board_mnit_f (board. c: 366) ; saved pc 0xfff0456c
           called by frame at 0xf000bf78
           source language c.
           Arglist at 0xf000bf50, args: bootflag=Ox1
           Locals at 0xf000bf50, previous frame 's sp is OxO

          << 재배치 후에 메모리에 존재하는 코드를 디버깅하게 됨 >>
          (gdb) del 1
          (gdb) symbol -file
          Discard symbol table from ' 갸iome/chri s/sandbox加七oot-1. 1.4-pow陀rdna/u七oot '?
          (y or n) y
          No symbol file now.
          (gdb) add-symbol- file u-boot 0x7fa8000
          add symbol table from file "u-boot " at
                 .text_addr = 0x7fa8000
          (y or n) y
          Reading symbols from u-boot. . .done.
          (gdb) b board_init_ r



1 478
                                                               커널 디버깅 기술      Chapter 14



          Breakpoint 2 at 0x7fac6c0: file board. c, line 608.
          (gdb) C
          Breakpoint 2, board_init_r (id=0x7f85f84, dest_addr=0x7f85f84) at board. c: 608
          608            gd = id;      /* initialize RAM version of global data */
          (gdb) i frame
          Stack level 0, frame at 0x7f85f38:
           PC = 0x7fac6c0 in board_init_r (board. c: 608) ; saved pc 0x7fac6b0
           Called by frame at 0x7f85f68
           source language c.
           Arglist at 0x7f85f38, args: id=0x7f85f84, destmaddr=0x7f85f84
           Locals at 0x7f85f38, Previous frame 's sp is OxO
          (gdb) mon break soft
          (gdb)



       이 예제를 주의 깊게 연구해 보도록 하자. 몇 가지 미묘한 점에 대해서는 시간을 투자해서
       이해할 만한 가치가 있다. 먼저 七arge七 remo七e 명령을 통해서 아바트론 BDI-2000에 연
       결한다. 여기서 사용한 II) 주소는 아바트론 장비의 주소인데 , 심볼릭 이름인 bdi25）로 표현
       했다. 그리고 아바트론 BDI-2000 장비는 gdb의 원격 프로토콜 연결을 위해서 포트 2001
       을 이용한다．

       다음으로 gdb의 mon 명령을 이용해서 BDI-2000에 명령을 내리는데 , mon 명령은 이 명령
       다음에 오는 내용을 JTAG 디버거 장비로 직접 전달하도록 해 준다. 그래서 mon break
       hard 명령은 BDI-2000이 하드웨어 브레이크 포인트를 사용하는 모드로 동작하도록 만들
       게 된다．

       그 다음에는 board mnit f 함수에 하드웨어 브레이크 포인트를 설정한다. 이 함수는 코드
       가 여전히 본래 위치인 플래시의 0xfff0457c 주소에서 실행되는 함수이다. 브레이크 포인
       트를 설정한 후에 continue 명령 C를 내리면 실행을 재개한다. 곧바로 board m1li七 f어］
       있는 브레이크 포인트가 걸리는데 , 이 때부터는 코드를 한 단계씩 실행하거나, 데이티의 내
       용을 검사하는 등 평소 방법대로 디버깅을 진행할 수 있다. 여기서 bt 명령을 이용해서 스택
       역추적을 확인하는 것을 볼 수 있다. 그리고 i frame 명령으로 현재 스택 프레임을 상세히
       확인해 볼 수 있는 것도 알 수 있다．



25) 호스트 시스템의 /etc/hos捻 파일어］ 항목을 추가0뻔 심볼릭 이름을 II) 주소 대신에 사용할 수 있다．


                                                                                    479 1
轟 磁N    Embedded Linux Primer




       이제 실행을 계속하도록 하는데 , 하지만 이번에는 U-Boot가 스스로를 RAM에 복사하고 복
       사한 위치에서 실행을 재개하는 것을 알 수 있다. 그래서 디버킹 세션을 유지하기 위해서는
       디버깅 문맥을 새롭게 변경해야 한다. 이를 위해서 현재의 심볼 테이블을 버리고 (symbol-
       file 명령을 아무런 인자 없이 실행시킨다）, add小syr巾ol-file 명령어로 같은 심볼 파일
       을 다시 로드한다. 하지만 이번에는 U-Boot가 새롭게 재배치된 곳에 맞도록 심볼 테이블의
       상대 위치를 gdb에 전달한다. 이렇게 하면 사용하는 소스 코드와 심볼릭 디버킹 정보가 실제
       존재하는 메모리 위치와 일치되도록 만들 수 있다.

       새로운 심볼 테이블이 로드되고 나면 이제 RAM에 위치하게 될 곳에 브레이크 포인트를 설
       정할 수 있다. 이 부분이 약간 어려운 부분 중의 하나인데 , 즉 U-Boot가 아직은 플래시 상에
       서 실행되고 있지만 곧 RAM으로 복사될 것이고 그 RAM 기반의 주소로 분기해서 실행을
       계속할 것이기 때문에 여전히 하드웨어 브레이크 포인트를 사용해야 한다. 이 시점에 소프트
       웨어 브레이크 포인트를 사용하면 어떻게 될지 생각해 보자. gdb는 자신의 역할대로 해당하
       는 위치에 브레이크 포인트 기계어 코드를 입력해 넣지만 U-Boot가 자기 자신을 그 RAM
       위치에 덮어 쓸 것이기 때문에 결국에는 이 브레이크 포인트는 절대로 걸리지 않을 것이다．
       그래서 툴이 망가진 게 아닌가 의심하기 시작할 것이다. 하지만 U-Boot 코드가 메모리에
       전부 복사되고 심볼 테이블도 새로운 RAM 기반 주소 값을 반영하도록 업데이트하고 나면
       이제 RAM 위치에 브레이크 포인트를 마음대로 설정할 수 있게 된다. 그래서 ［리스트
       14-21］에서 마지막 명령으로 아바트론 장비를 소프트웨어 브레이크를 사용하는 모드로 바
       꾼 것이다．

       그런데 왜 하드웨어 브레이크 포인트와 소프트웨어 브레이크 포인트를 신경 써야 할까7 만약
       에 하드웨어 브레이크 포인트가 무한정 있다면 그럴 필요가 없겠지만, 실제로 그럴 일은 없
       다. 다음 내용은 디버깅 중어］ 프로세서가 지원하는 하드웨어 브레이크 포인트를 다 썼을 때
       어떤 메시지를 볼 수 있는지를 나타낸 것이다．



         (gdb) b flash_mnit
         Breakpoint 3 at 0x7fbebe0: file flash. c, line 70.
         (gdb) C
         continuing.
         warning: cannot insert breakpoint 3:
         Error accessing memory address 0x7fbebe0: unknown error 4294967295.



480
                                               커널 디버깅 기술   Chapter 14



    여기서는 원격으로 디버깅하고 있기 때문에 브레이크 포인트를 추가하는 명령을 내린 뒤에
    도, 실제로 실행을 재개시키기 전까지는 그 자원에 대해서 판단을 할 수 없기 때문에 경고
    메시지가 나중에 나오는 것이다. 이는 gdl＞가 브레이크를 처리하는 방식 때문이다. 브레이크
    포인트를 만나면 gdb는 모든 브레이크 포인트를 원래의 기계어 코드로 원상 복귀시킨다. 그
    리고 실행을 재개시키면 브레이크 포인트 코드를 다시 해당 지점에 기록하도록 되어 있다．
    이 내용은 gdb의 원격 디버그 모드를 활성화시키면 확인할 수 있다．

      (gdb) set debug remote 1



14.5 부팅이 되지 않을 때
    다양한 임베디드 리눅스 관련 메일링 리스트에서 볼 수 있는 가장 흔한 질문 중의 하나는
    다음과 같은 것이다．

      라눅스를 졔 보드에 부팅하려고 했는녜, 콘솔에 다음 메사차가 나온 다음에 멈춰 버립나다．

       Uncompressing Kernel Image. . . OK. "


    이로 인해서 사람들이 길고 험난한 임베디드 리눅스의 길로 접어들게 된다！ 여러 가치 원인
    으로 인해서 이 오류가 생길 수 있는데 , 여기서 JTAG 디버거와 약간의 기본 지식만 있으면
    무엇이 잘못되었는치를 판단할 수 있다．


14.5. ] 초기 시리얼 디버그 츈력
    가장 먼저 사용할 수 있는 방법으로 CONFIG SERIAL TEXT DEEUG7} 있다. 이 리눅스 커
    널 구성 옵션은 초기 부팅 과정에서도 디버그 메시지를 출력할 수 있도록 해 준다U 이 글을
    쓰는 시점에는 PowerPC 아키텍처에서만 이 기능을 쓸 수 있지만, 다른 아키텍처에서 사용
    하는 데 문제가 될 것은 없을 것이다. ［리스트 14-22］에서 U-Boot 부트로더를 이용한
    PowerPC 타깃에서 이 기능을 사용하는 예제를 볼 수 있다．
        Embedded Linux Primer



      ［리스트 14-22] 초71 시리얼을 통한 디버그 출력


         ## Booting image at 00200000 . . .
            Image Name:   Linux-2. 6. 14
            Created:     2005-12-19 22: 24:03 UTC
            Image Type:   PowerPC Linux Kernel Image (gzip compressed)
            Data Size:    607149 Bytes = 592. 9 kB
            Load Address: 00000000
            Entry Point: 00000000
            verifying Checksum . . . OK
            Uncompressing Kernel Image . . . OK
         id machO: done       <== CONFIG_SERIAL_TEXT_DEBUG에 의해서 활성화된
         MMU: enter          <=== 메시지 출력임
         MMU : hw m nit
         MMU : mapi n
         MMU : set化
         MMU : ex卄
         setup_arch: enter
         setup_arch: bootmem
         arch: exit
         arch: real exit




      이 기능을 이용하면 부팅 과정에서 보드의 어느 부분에서 문제가 일어났는지를 찾을 수 있는
      경우가 많다. 물론 커널의 다른 위치에서 자신만의 디버그 메시지를 출력하도록 할 수도 있
      다. 다음은 . . . /arch/ppc/mm/init. c에서 볼 수 있는 예제이다．



         /女 Map in all of RAM starting at KERNELBASE 玄 /
         if (ppc_md. progress)
                ppc_nid. progress("MMu:mapin", 0x301) ;
         mapin_ramO;




      AMCC 요세미티 플랫폼은 이 구조를 위한 아주 좋은 예제인데 , 리눅스 소스 코 三에서 다음
      파일26）을 보면 어떻게 이 디버깅 시스템이 구현되어 있는지 볼 수 있다．



26) 이 파일들의 이름은 전체 코드에서 유일한 0］勘口］ 때문애, 전체 경로를 알 필요 없이 어떤 파일인지 확인할 수 있다．
                                                      커널 디버깅 기술   Chapter 14




     파일                  함수                    기능

     gen550 dbg. c       gen550 mnit           플랫폼 초기화 파일인 yosemite. c에
                                               의해서 호출되는 시리얼 포트 설정 함수

     gen550 dbg. c       gen550 progress       저수준 시리얼 寄1 루틴

     ibm44x comlnon. c   ibm4小＜platforrninit   일반 PowerP（二 머신 종속적인 구조어써
                                               플랫폼 종속적인 진행 루틴을 연결시킴



14.5.2 printk 로그 버퍼의 내용 덤프하기
    14.3.6절에서 printk를 위한 디버깅을 다룰 때 이 방법이 갖는 몇 가지 한졔에 대해서 언
    급했었다. printk 자체는 아주 튼튼하게 구현되어 있지만, 단점 중의 하나는 부팅 과정이
    진행되어 콘솔 디바이스가 초기화되고 난 후에야 출력된 메시지를 볼 수 있다는 것이다. 보
    드에서 리눅스가 부팅 중에 멈춰 버렸을 때 출력될 일부 메시지가 printk 버퍼에 남아 있는
    경우가 대부분이다. 이 메시지들이 어디에 숨어 있는치 안다면 부팅이 멈춘 정확한 이유를
    찾아낼 수 있는 경우가 많다. 실제로 커널이 panic () 함수를 부르도록 하는 에러가 발생했
    기 때문에 멈춘 경우가 대부분이다. 그리고 panic () 함수의 출력이 보통 prin七k 버퍼에
    일단 쌓이기 때문에 정확히 어떤 코드가 문제를 일으키는지 짚어낼 수 있을 때가 많다．

    printk 버피의 내용을 확인하는 가장 좋은 방법은 JTAG 디버거를 사용하는 것이다. 하지
    만 부트로더에서 메모리를 덤프하는 기능을 이용해서 리셋 후에 printk의 버퍼 내용을 다
    시 출력해 볼 수 있다. 리셋의 결과로 메모리 내용의 일부는 깨지거나 하겠지만, 로그 버퍼의
    내용은 일반적으로 읽을 수 있을 정도로 남아 있게 된다．

    printk7} 출력할 메시지를 저장하1 두는 실제 버퍼는 printk 소스 파일인 . . . /kernei/
    printk. c어］ 정의되어 있다．

       static char _log_buf[_LoG_BuF_LEN] ;

    리눅스 커널의 맵 파일인 System.map 파일을 보면 쉽게 이 버퍼가 링크된 위치를 확인할
    수 있다．




                                                                        483    I
囊輦1    Embedded Linux Primer




        $ grep _log_buf system .map
           c022e5a4 b _lo工加f



  이제 만약에 시스템이 부팅 중에 "Uncon叩ressing Kernel Image . . . 01<' 메시지를 출력
  한 다음에 멈춘다면 재부팅 후에 부트로더에서 이 버퍼를 확인해 보자. 커널 가상 메모리와
  물리 메모리 간의 관계가 아키텍처에서는 항상 고정되어 있기 때문에 간단하게 변환할 수 있
  다. 즉, 이전에 나온                 1四 buf의 주소는 커널 가상 주소이기 때문에 , 물리 주소로 변환해
      서 확인해야 한다. 이 변환은 단순히 KERNELBASE라는 Oxc0000000 상수 주소를 빼면 된
  다. 지금까지 printk의 로그 버퍼 내용을 （만약에 있다면） 확인해서 디버깅하는 방법을 설
  명했다．

  ［리스트 14-23］에서 U-Boot의 메모리 덤프 명령어를 사용해서 출력된 내용을 볼 수 있다．

  ［리스트 14-23J printk 로그 버퍼의 내용 덤프하71

        => md 22e5a4
        0022e5a4: 3c353e4c 696e7 578 20766572 73696f6e    <5>Linux version
        0022e5b4: 20322e36 2e3 13 320 28636872 6973406a    2. 6.13 (chris@
        0022e5c4: 756e696f 72292028 67636320 76657273     junior) (gcc
        0022e5d4: 696f6e20 332e342e 3320284d 6f6e 7461    version 3. 4. 3 (Monta
        0022e5e4: 56697374 61203 32e 342e332d 32352e30    vista 3. 4. 3-25. 0
        0022e5f4: 2e37302e 30353031 39363120 32303035     .70. 0501961 2005
        0022e604: 2d31322d 31382929 20233131 20547565     U끄-18力 #11 Tue
        0022e614: 20466562 20313420 32313a30 353a3036       Feb 14 21: 05: 06
        0022e624: 20455354 20323030 360a3c34 3e414d43      EST 2006. <4>AMC
        0022e634: 4320506f 77657250 43203434 30455020     C PowerPC 440EP
        0022e644: 596f7365 6d697465 20506c61 74666f72     Yosemite Platform.
        0022e654: 6d0a3c37 3e4f6e20 6e6f6465 20302074     <7＞아） node 0
        0022e664: 6f74616c 70616765 733a2036 35353336     totalpages: 65536
        0022e674: 0a3c373e 2020444d 41207a6f 6e653a20     . <7> DMA zone:
        0022e684: 36353533 36207061 6765732c 204c4946     65536 pages, [IF
        0022e694: 4f206261 7463683a 33310a3c 373e2020     0 batch: 31. <7>
        =>
        0022e6a4: 4e6f726d 616c207a 6f6e653a 20302070     Normal zone: 0
        0022e6b4: 61676573 2c204c49 464f2 062 61746368    pages, LIEU batch
        0022e6c4: 3a310a3c 373e2020 48696768 4d656d20     :1. <7> Hi ghMemzone:
        0022e6d4: 7a6f6e65 3a203020 70616765 732c204c     0 pages,
                                                       커널 디버깅 기술     Chapter 14



      0022e6e4: 49464f20 62617463 683a310a 3c343e42   LIFO batch:1. <4>
      0022e6f4: 75696c74 2031207a 6f6e656c 69737473   Built 1 zonelists
      0022e704: 0a3c353e 4b65726e 656c2063 6f6d6d61   .<5>Kernel command
      0022e714: 6e64206c 696e653a 20636f6e 736f6c65   line: console
      0022e724: 3d747479 53302c31 31353230 3020726f   =ttySO,115200
      0022e734: 6f743d2f 6465762f 6e667320 72772069   root=/dev/nfs rw
      0022e744: 703d6468 63700a3c 343e5049 44206861   ip=dhcp. <4>PID
      0022e754: 73682074 61626c65 20656e74 72696573   hash table entries
      0022e764: 3a203230 34382028 6f726465 723a2031   : 2048 (order:
      0022e774: 312c2033 32373638 20627974 6573290a   11, 32768 bytes) .
      0022e784: 00000000 00000000 00000000 00000000
      0022e794: 00000000 00000000 00000000 00000000
      =>
    위 내용은 읽기가 그리 편한 것은 아니지만, 어떤 내용이 거기 있기는 하다. 이 예제에서는
    커널이 PT') 해시 테이블 항목을 초기화하고 난 후에 시스템이 충돌한 것을 볼 수 있다．
    printk 메시지를 활용한 결과 실제 충돌이 일어난 소스 코드에 더 가깝게 접근할 수 있게
    되었다．

    이 예제에서 보는 것치럼 이 디버깅 방법은 추가적인 툴 없이도 할 수 있다. 그리고 새로운
    보드를 포팅하는 작업을 하는 경우라면 초기 부팅중의 시리얼 포트 출력이 얼마나 중요한지
    알 수 있을 것이다．


14.5.3 커널 패닉어IAI KGDB 사용하기
    만약에 KGDB가 켜져 있다면 커널은 에러 상황에 KGDB로 제어권을 넘기려고 할 것이다．
    그리고 일부 경우에는 에리를 명확하게 파악할 수도 있을 것이다. 이 기능을 위해서는
    KGDB와 gdb 간에 미리 연결이 되어 있어야 한다. 예외 상황이 발생하면 KGDB의 디버그
    핸들러가 트랩이 발생한 이유와 트랩 상황이 발생한 주소를 포함해서 gdb어］ 정지 응답 패킷
    을 보낼 것이다. ［리스트 1午24］에서 이 과정을 볼 수 있다.

    ［리스트 14-24) KGDB를 이용해서 커널 패닉 포착하기

      $ ppc-_4xx-gdb --silent vmlinux
      (gdb) target remote /dev/ttysO
      Remote debugging using /dev/ttyso



                                                                           485    I
       Embedded Linux Primer



       Malformed response to offset query, qoffsets
       (gdb) target remote /dev/ ttysO
       Remote debugging using /dev/ttys0
       breakinst 0 at arch/ppc/kernel/ppc-stub. c: 825
       825     }
       (gdb) C
        Continuing.
        << 충돌 시 panic() 함수로 인해 KGDB가 제어권을 얻게 됨 >>
        Program received signal SIGSEGV, Segmentation fault.
        0xc0215d6c in pcibios_init 0 at arch/ppc/kernel/pci .c:1263
        1263           六（I nt 央）-1 = 0;
        (gdb) bt
        #0 0xc0215d6c in pc卄너os_init 0 at arch/ppc/kernel/pci. c:1263
        #1 0xc020e728 in do_initcalls 0 at init/ main. c: 563
        #2 0xc020e7c4 in do_basic_setup 0 at init/ main. c: 605
        #3 0xc0001374 in mnit (unused=0x20) at init/ main. c:677
        #4 0xc00049d0 in kernel_thread 0
        Previous frame inner to this frame (corrupt stack?)
        (gdb)



      위 시스템 충돌 예제는 의도적으로 잘못된 메모리 주소（모두 1인 주소）에 값을 쓰려고 하는
      코드를 이용한 것이다. 먼저 gdb에서 KGDB로 연결을 맺고, 커널이 부팅을 계속하도록 실
      행시킨다. 여기서 브레이크 포인트를 따로 설정하치도 않았다는 점을 주의하자. 시스템 충돌
      이 일어나면 문제가 되는 코드를 볼 수 있고, 훌륭한 스택 역추적을 통해서 문제가 무엇인지
      를 결정할 수 있도록 돕는 것을 볼 수 있다．



]4.6 요약
       다 리눅스 커널 디버깅을 위해서는 여러 가지 복잡한 사항을 고려해야 하는데, 특히 교차
           개발 환경에서는 더더욱 그렇다. 성공적으로 커널을 디버깅하기 위해서는 이런 복잡한
           내용을 이해하는 것이 아주 중요하다．

       口 KGDB는 리눅스 커널이나 디바이스 드라이버를 소스 레벨에서 바로 디버깅할 수 있도록
           해 주는 훌륭한 커널 레벨 gdb 스텁이다. KGDB는 호스트에서 실행중인 교차 gdb와
           통신하기 위해써 gdl刈 원격 프로토콜을 이용한다．




486
                                                 커널 디버깅 가술   Chapter 14



       口 컴파일러가 최적화시킨 코드를 디버거에서 한 단계씩 디버깅해1 나갈 때 디버거의 행동이
         이상해1 보일 때가 있는데, 이를 이해하기 위해서 컴파일러 최적화 기능을 이해하는 것이
         （그리고 최소화하는 것이） 좋다．

       口 gdb에서는 사용자 정의 명령어를 만들어 쓸 수 있는뎨, 복잡한 변수에 접근하기 위해서
         연결 리스트를 반복적으로 검사하는 것과 같은 반복적이고 소모적인 디버깅 작업을 자동
         화시킬 수 있는 강력한 툴이다．

       口 적재 가능한 커널 모듈을 소스 레벨에서 디버깅할 때는 더 어려운 점이 있는데, 모듈 초
         기화 루틴을 디버깅하기 위해서는 module. c에서 module->init (）을 호출하는 부
         분에 브레이크 포인트를 설정하면 된다．

       口printk와 매직 SysReq 키 조합은 커널 개발 및 디버깅 과정에서 문제를 찾아내는 데
         추가적인 도움이 되는 도구들이다．

       다 JTAG 프로브 하드웨어 장비를 이용해써 디버깅하면 플래시 또는 ROM에 있는 코드도
         디버깅할 수 있다. 플래시나 ROM에 있는 코드의 경우에는 그 외의 방법으로 디버깅하
         는 것이 아주 어렵거나 불가능하다．

       口 CONFIG SERIAL TEXT DEBUG 옵션을 지원하는 아키텍처에서 이 기능을 활성화시키
         면 커널을 새롭게 포팅하는 경우에 디버깅할 때 아주 강력한 디버깅 도구로 사용할 수
         있다.

       口 printk가 사용하는 1四 buf의 내용을 검사해1 보면 별다른 메시지 출력 없이 커널이
         충돌한 경우에 그 원인을 찾을 수 있는 단서를 제공해1 주기도 한다．

       댜 KGDB는 커널 패닉이 발생한 경우에 제어권을 gdl涅 넘겨주는뎨, 이때 스택 역추적이
         나 커널 패닉의 원인을 파악할 수 있도록 여러 가지 실험을 해1 볼 수 있다．



14.6. ] 더 읽01 보기
       Li끄ux Kernel Develoj）끄le끄t, 2nd 月ditio끄

       Robert Love

       Novell Press, 2005


       7-力e Li끄UX Kernel Pri끄er

       Claudia Salzberg Rodriguez et al.
       Prentice Hall, 2005
 多a.    Embedded Linux Primer




        "Using the GNU Compiler Collection"
        Richard M, Staliman and the GCC Developer Community
        GNU Press, a division of Free Software Foundation

        http://gcc. gnu. org/onlinedocs/


        KGDB 소스포지 홈페이지

        http://sourceforge,net/projects/KGDB


        GDB로 디버깅하기
        Richard Stailman, Roland Pesch, Stan Shebs, et al,
        Free Software Foundation
        www, gnu, org/software/gdb/documentation/


        툴 인터페이스 표준（Tool interface standards)
        DWARF 디버깅 정보 형식 명세서（DWARF Debugging Information Format
        Specification)
        버전 2,0
        TIS Committee, 1995년 5월




I 488
Ch冒何蛇伊 ]5


     임베디드 리눅스 어플리케이션
                    디버깅하기



이번 징에서 배울 내용

  I 타깃 디버깅

  . 원격 （교차） 디버깅

  . 공유 라이브러리 디버깅

  . 여러 태스크 디버깅하기

  . 추7F 원격 디버그 옵션

  U 요약
難 髓1    Embedded Linux Primer




       이전 장에서는 커널 코드와 플래시에 존재하는 부트로더와 같은 코드를 디버깅하기 위해서
       GDB를 사용하는 방법에 대해서 알아봤다. 이번 장에서는 사용자 영역에서 실행되는 어플리
       케이션을 GDB로 디버깅하는 방법을 다루도록 하겠다. 그리고 원격 디버킹 및 우리가 사용
       하는 특수한 디버깅 환경에서 사용할 만한 툴과 관련 기술에 대해서도 살펴볼 것이다．



15. ] 타깃 디버깅
       이미 13장, "개발 도쿠'에서 디버깅 시에 사용되는 툴에 대해서 몇 가지 살펴본 적이 있다．
       strace와 itrace를 이용하면 프로세스의 행동을 관찰할 수 있고, 종종 문제의 원인을 찾
       는 데도 이용할 수 있다. dmalloc은 메모리 누수를 찾아내거나 메모리 사용에 대한 프로파
       일 정보를 얻는 데 사용할 수 있다. 그리고 PS와 七OP은 실행중인 프로세스의 상태를 확인할
       수 있는 툴이다. 상대적으로 작은 크기를 갖는 이 툴들은 타깃 하드웨어에서 바로 실행되도
       록 만들어진 것들이다．

       임베디드 시스템에서 리눅스 어플리케이션 코드를 디버깅하는 것은 그 특수성 때문에 , 나름
       의 어려운 점이 존재한다. 보통 임베디드 타깃 시스템은 제한퇸 자원만을 가지고 있다. 즉，
       RAM이나 비휘발성 저장 공간의 한계 때문에 타깃에서 바로 개발 툴을 구동하지 못한다. 또
       한 이더넷 포트나 기타 고속의 연결 매체가 없는 것은 물론이고, 그래픽 표시 장치나 키보드
       마우스 등도 존채하지 않는 경우가 많다．

       이런 상황 때문에 교斗개발 툴을 이용하고, NFS 루트 파일 시스템을 마운트하는 환경을
       이용하는 경우가 대부분이다. 많은 툴, 그 중에서도 특히 GDB는 개발 호스트 시스템에서
       실행되지만 실제 디버깅은 원격 타깃에 있는 코드를 대상으로 한다. GDB는 대상 타깃 코드
       를 직접 실행하면서 디버깅하는 것도 가능하고 어플리케이션의 충돌로 인해 생성된 코어 덤
       프 파일을 나중에 분석하는 것도 가능하다. 어플리케이션의 코어 덤프를 분석하는 것은 13장
       에서 자세히 설명했다．



15.2 원격 （교차） 디버깅
       교차개발 도구는 1차적으로 임베디드 플랫폼의 자원 한계를 극복하기 위해서 만들어진 것
       이다. 일반적인 크기의 어플리케이션이라도 심볼릭 디버깅 정보를 포함해서 컴파일시키면 수
                                                 임베디드 리눅스 어플리케이션 디버깅하기                                                                                     Chapter 15




       메가 바이트를 쉽게 넘긴다. 교차 디버깅에서는 이런 큰 크기의 파일은 호스트에 두고 작업
       할 수 있다. 개발 호스트 시스템에서 교차 GDB를 실행하고 심볼릭 디버깅 정보를 포함하고
       있는 ELF 파일을 인자로 넘겨준다. 하지만 타깃에서는 ELF 파일에서 이 디버깅 정보를 모
       두 잘라 버리고1) 최소한의 크기로 만들어서 실행시켜도 아무런 문제가 없다．

       readeif 유틸리티에 대해서는 전에 13장에서 설명한 적이 있는데 , 14장, "커널 디버킹 기
       술'에서 심볼릭 디버그 정보를 포함하도록 컴파일된 ELF 파일에서 디버깅 정보를 확인할
       때 이 툴을 사용했었다. ［리스트 15-1]은 ARM 아키텍처를 위해서 컴파일된 작은 웹 서버
       어플리케이션을 대상으로 readeif 명령을 실행한 결과를 나타낸 것이다．

      ［리스트 ]5-1] 예제 프로그램에서 ELF 파일 디버깅 정보 확인하기


         $ xg口al._b. -reacleif -s 찌.bad.m口
         There are 39 section headers, starting     at offset   0x3dfd0:

         Section Headers:
         [Nr] Name                 Type         Addr       Of f   Size    묘S Fig Lk Inf                                                                                                                                   Al




                                                                                                                                                               0 0 0 0 0 l 0 0 l l 0 0 0 0 0 0 0 0 0 00 0 0 0 0 0 0 0 0
                                                                                                                                                                                                                          0 l 4 4 4 4 l 2 4 4 4 4 4 4 8 l 4 4 4 44 4 4 4 8 4 l 8 l
         [ 0)                      NULL         00000000 000000 000000 00
                                                                                                                                      응




                                                                              A A A A A A A A A M M M 醒 A A 肌 A A m 呱 呱 咀 呱 咀 呱
         [ 1] .interp              PROGBITS     00008154 000154 000013 00
                                                                                                                                         0
         [ 2] .nc比e. ABI比ag        NOTE         00008168 000168 000020 00
                                                                                                                                         0
         [ 3] .note. nuxnapolicy   NOTE         00008188 000188 000074 00
                                                                                                                                         CV
         [ 4] . hash               HASH         000081fc 0001f＜그 00022c 04
                                                                                                                                         戶
                                                                                                                                         b
         [ 5] .dynsym              DYNSYM       00008428 000428 000460 10
                                                                                                                                         0
         [ 6] .dynstr              STRTAB       00008888 000888 000211 00
                                                                                                                                         CJ
         [ 7] . gnu.version        VERSYM       00008a9a 000a9a 00008c 02
                                                                                                                                         6
         [ 8J ' gnu.version_r      VERNEED      00008b28 000b28 000020 00                                                         니
                                                                                                                                  C                        a
                                                                                                                                                           l
         [ 9] .rel. plt            R丑L          00008b48 000b48 000218 08




                                                                                                                                         0 0 0 0 0 0
         110] .init                PROGBITS     00008d60 000d60 000018 00
         [11)   .pit               PROGBITS     00008d78 000d78 000338 04
         [12)   .t曲比               PROGEITS     000090b0 0010b0 019 fe4 00
         [13]   ,fini              PROGHITS     00023094 01b094 000018 00
         [14)   .rodata            PROGBII冬     00 023 0b0 0lbOb0 002 3d0 00
         (15]   .ARN. extab        PROGBII峀     00025480 01d480 000000 00
         [16)   .ARN 'exidx        ARM EXIDX    00025480 01d480 000008 00     AL 12




                                                                                                                                             0 0 0 0 0 0
         [17]   . eh_frame_hdr     PROGBITS     00025488 01d488 00002c 00




                                                                                                                                  0 0 00 0
         [18]   .eh_frame          PROGBITS     000254b4 01d4b4 00007c 00
         (19]   .initmarray        INIT ARRAY   0002d530 01d530 000004 00
         (20]   .fini_ array       FINI ARRAY   0002d534 01d534 000004 00
         [21]   .Jcr               PROGBITS     0002d538 01d538 000004 00




                                                                                                                                          b戶
         (221   .dynamic           DYNAMIC      0002d53c 01d53c 0000d0 08
         (231   . g<＞七             PROGBITS     0002d60c 01d60c 000118 04
         (24]   .data              PR（焰BITS     0002d728 01d728 0003c0 00
         [25)   .bss               NOBITS       0002dae8 0ldae8 0001c8 00
         [26)   .comment           PROGBITS     00000000 01dae8 000940 00
         [27)   .debug_aranges     PROGBITS     00000000 01e428 0004a0 00
         (28)   . debugmpubnames   PROGEITS     00000000 01e8c8 00laae 00




l) 물론 strip 명령을 쓰되 교차 버젼을 사용해야 한다. 이 예에서는 pix_82o-sti如을 이용해야 한다．


                                                                                                                                                                                                                                                             491 1
        Embedded Linux Primer




                                                                           0 0 0 0 0 0 0 0   0 0 0 0 0 0 0 0

                                                                                                               l l l 4 l l l l 4 l
        [29) .debug_info          PROGBITS    00000000 020376 013d27 00
        [30] .debug_abbrev        PROGBITS    00000000 03409d 002ede 00
        [31] .debug_line          PROGBITS    00000000 036f7b 0034a2 00
        [32] .debug_ frame        PROGBITS    00000000 03a420 003380 00
        [33] .debug_str           PROGBITS    00000000 03d7a0 000679 00
        [34] .note. gnu. arm. ide NOPE        00000000 03de19 00001c 00
        [35] . debug_ranges       PROGBITS    00000000 03de35 000018 00
        [36] .shstrtab            STRTAB      00000000 03de4d 000183 00
        [371 .syintab             SYMTAB      00000000 03e5e8 004bd0 10  38 773
        [381 .strtab              STRTAB      00000000 0431b8 0021bf 00   0   0
       표ey 七a Flags :
       w 佃rite) , A (alloc) , X (exec王.1七e) , M (merge) , S （就ring帥
       I (info) , L (link order) , G (group) , x (unknown)
       0 (extra OS processing required) o (OS specific) , p (processor specific)
       S




      ［리스트 15-1]을 통해서 디버깅 정보를 담고 있는 섹션이 여러 7뀨 존재하는 것을 볼 수 있다．
      또한 어플리케이션을 실행하는 데는 전혀 필요가 없는 . comment 섹션도 2KB (0x940) 이
      상 포함되어 있는 것을 볼 수 있다. 이 예제 파일의 크기는 디버깅 정보를 포함하면 275KB
      이상이다．



        $ is -i websdemo
        -rwxrwxr- x 1 chris chris 283511 Nov 8 18: 48 websdemo



      여기서 strip 유틸리티로 디버깅 정보를 잘라내면 타깃 시스템의 자원 활용을 위해서 파일
      의 크기를 최소화할 수 있다. ［리스트 15-2］에서 그 결과를 볼 수 있다．

      ［리스트 ]5-2] 타깃 어플리케이션을 str巾을 이용해Al 잘라내기

        $ xscaie_be- strip -s -R .comment -o websdemo- stripped websdemo
        $ is -i websdemo*
          rwxrwxr- x 1 chris chris 283491 Apr 9 09: 19 websdemo
        -rwxrwxr- x 1 chris chris 123156 Apr 9 09: 21 websdemo-stripped
        $




492
                                      임베디드 리눅스 어플리케이션 디버깅하기   Chapter 15




     여기서는 실행 파일에서 심볼릭 디버깅 정보와 . COTI끄nent 섹션 모두를 잘라냈다. 그리고 잘
     라낸 결과 파일의 이름을 지정해 주기 위해서 中O 명령에 라인 스위치를 이용했다. 잘라낸
     결과 파일의 크기가 원래 파일 크기와 비교했을 때 절반 이상 줄어든 것을 볼 수 있는데 , 물
     론 더 큰 크기의 어플리케이션에서는 훨씬 더 많은 공간을 줄일 수 있다. 최신 리눅스 커널의
     경우 디버그 정보를 포함해서 빌드할 경우에 크기가 18MB 이상이다. 하지만 ［리스트
     15-2］와 같이 디버깅 정보를 잘라내고 난 후에 그 크기를 보면 2MB가 조금 넘는 정도밖에
     안 된다！

     이 경우에 디버깅을 위해서는 디버킹 정보를 드리낸 바이너리 파일을 타깃 시스템에 두고，
     디버깅할 때 필요한 정보를 포함하고 있는 원본 파일은 개발 워크스테이션에 두도록 한다．
     그리고 타깃 보드에서는 gdbserver를 실행시켜서 호스트에서 실행되는 풀 버천 GDB에서
     디버깅 정보가 포함된 원본 바이너리 파일을 디버깅하면서 내리는 요청에 대해서 응답하도록
     한다．


15.2.1 gdbserver
     gdbserver를 이용하면 타깃 임베디드 리눅스 플랫폼에서 GDB를 직접 실행하는 대신에
     개발 워크스테이션에서 GDB를 실행할 수 있다. 이 방식에는 확실한 장점이 있는데 , 첫째로
     개발 워크스테이션이 CPU 속도가 훨씬 빠르고, 메모리나 하드 드라이브의 공간이 임베디드
     플랫폼보다 훨씬 크기 때문이고, 또 한 가치는 디버깅하고자 하는 立로그램의 소스 코드가
     일반적으로 임베디드 플랫폼이 아닌 개발 워크스테이션에 존재하기 때문이다．

     gdbserver는 보드에서 실행되는 프로세스를 원격으로 디버깅할 수 있도록 해 주는 타깃
     보드에서 실행되는 작은 프로그램이다. 타깃 보드에서 디버깅하고자 하는 프로그램 이름을
     인자로 넘겨서 실행한다. 그리고 거기에 추가적으로 GDB의 연결을 기다리기 위한 II) 주소
     와 포트 번호도 같이 기술한다. ［리스트 15-3］에서 타깃 보드에서 gdbserver를 실행하는
     방법을 볼 수 있다．

     ［리스트 ]5-3] 타깃 보드에서 gdbserver 실행하71


       $ gdbserver ]oca什山st :2001 川ebsdemo卜stripped
       Process websdemo- stripped created; pjd = 197
       Listening on port 2001




                                                                   493
 弊 二U      Embedded Linux Primer




         이 예제는 gdbserver를 이용해서 디버깅 정보를 잘라낸 websdemo-就ripped라는 바이
         너리 프로그램을 디버깅하도록 준비하고, TCP/IP 포트 2001로 원격 GDB 연결을 받도록
         대키한다．

         그러면 개발 워크스테이션에서는 디버깅하고자 하는 프로그램, 즉 심볼릭 디버그 정보를 가
         지고 있는 바이너리 실행 파일의 이름을 GDB에 인자로 전딜해서 실행시킨다. 그리고 GDB
         가 시작되면 원격으로 타깃 보드에 연결하는 명령을 내리는데 , ［리스트 15-4］에 이 과정이
         나와 있다．

         ［리스트 ]5-4] 원격 0DB 세션 시작하기


           $ xscale_be-gdb -q websdemo
           (gdb) target remote 192.168.1.141:2001
           Remote debugging using 192.168.1.141: 2001
           0x40000790 in?? 0
           (gdb) p main       <<<< main 함수의 주소를 출력
           $1 = tint (int, char 少 *)} 0x12b68 <main>
           (gdb) b main       <<<< main () 함수에 브레이크 포인트를 설정
           Breakpoint 1 at 0x12b80: file main. c, line 72.
           (gdb)




         ［리스트 15-4］에서는 개발 호스트에서 교차 gdb를 실행시켰다. 그리고 GDB가 실행되면
         gdb 명령인 七arge七 remo七e 명령을 실행시키는데, 이 명령을 통해서 GDB가 개발 호스트
         시스템과 타깃 보드 사이에 주어진 IP와 포트를 이용해서 TCP/If) 연결을 요청하게 된다．
         그리고 gdbserver7} 이 연결 요청을 받아들이면 다음과 비슷한 내용이 출력된다．

           Remote debugging from host 192.168.0.10


         이제 타깃 보드에서 실행중인 gdbserver 프로세스와 GDB가 연결되었기 때문에 GDB에
         서 내리는 명령을 받을 수 있다. 이제부터는 같은 시스템에서 프로그램을 디버깅하는 것과
         똑같은 방식으로 디버깅을 진행할 수 있다. 이는 디버깅 중에 개발 워크스테이션의 컴퓨팅
         파워2）를 활용하면서도 작고 성능상의 부담 없는 GDB 스텁을 통해서 타깃 시스템에 있는
         프로그램을 디버깅할 수 있도록 해 주는 강력한 툴이다. 놀랍게도 ARM 타깃을 위한
         gdbserver의 경우 그 크기가 54KB밖에 되지 않는다．

2) （역자주） 연산 능력


I 49 '
                                    임베디드 리눅스 어플리케이션 디버깅하기          Chapter 15




   root@coyote:畔 is -1 /usr/bin/gdbserver
   -rwxr- xr-x 1 root root 54344 Jul 23 2005 /usr/bin/gdbserver



한 가지 주의할 점이 있다. 이 부분은 특히 여러 메일링 리스트에서 자주 찾는 질문（FAQ)
중의 하나인데 , 바로 캐발 호스트에서 실행할 GDB가 교차 디버거로 구성되어 있어야 한다는
것이다. 즉, 개발 워크스테이션에서 실행되는 프로그램이지만, 다른 아키텍처를 위해서 컴파
일된 바이너리 실행 파일을 인식하도록 설정되어 있어야 한다. 이 내용은 중요하지만 자주
간과되는 부분이다. 일반 데스크탑 리눅스인 레드햇에서 실행되는 자체 GDB를 이용해서는
PowerPC 타깃을 절대로 디버깅할 수 없다. 원하는 타깃에서 디버깅하도록 하려면 GDB가
실행되는 호스트와 디버킹하려는 타깃 조합을 알맞게 구성해야 한다.

GDB가 실행되면 이 GDB가 컴파일된 구성 정보를 보여 주는 배너가 몇 줄 표시되는데 , ［리
스트 好5］에서 볼 수 있는 GDB는 이 책의 다른 몇몇 예제에서도 사용된 것으로, 몬타비스
타 소프트웨어에서 PowerPC 교차 개발을 위해 구성한 배포 버전이다．

［리스트 ]5-5] 교차-gdb 실행시키기


  $ ppc_82xx-gdb
  GNU gdb 6. 0 (Montavista 6.0-8.0. 4. 0300532 2003-12-24)
  copyright 2003 Free software Foundation, Inc.
  GDB is free software, covered by the GNU General Public License, and
  you are welcome to change it and/or distribute copies of it under
  certain conditions. Type "show copying" to see the conditions.
  There is absolutely no warranty for GOB. Type "show warranty" for
  details.
  This GOB was configured as "- -host=1686- pc尸linux-gnu
  --target=powerpc-hardhat-l i nux".
  (gdb)



GDB가 시작할 때 출력되는 마지막 줄을 주의하자. 이 줄의 내용은 GDB를 컴파일할 때 사
용된 구성 옵션을 보여 준다. 내용을 보면 GNU/Linux가 설치된 펜티엄 (i686) PC 호스트
에서 실행되도록 컴파일되어 있고, GNU/Linux7} 구동되는 PowerPC 시스템을 위해서 컴
파일된 GNU/Linux 바이너리 파일을 디버그할 수 있도록 구성된 것을 알 수 있다. 이는


                                                                         495 丑
蘿U      Embedded Linux Primer




       배너에 표시된 小host와 41七arget 변수의 내용으로 알 수 있는데, GDB를 빌드할 때
       ./configure에 전달퇸 구성 옵션 문자열과 같은 내용이다．



15.3 공유 라이브러리 디버깅
       지금까치의 설명을 토대로 흐入E에서는 GDB를, 타깃에서는 gdbserver를 이용해서 원격
       디버그 세션을 생성한다는 것을 이해했을 것이다. 이제는 공유 라이브러리와 디버그 심볼의
       복잡한 관계로 관심을 돌려 보도록 하자. 자신이 작성한 어플리케이션이（커맨드 라인에서 링
       커에 -s七a七ic 옵션을 줌으로써） 정적으로 링크한 것이 아닐 경우에 , 어플리케이션에서 사
       용되는 많은 심볼이 외부의 코드를 참조하도록 되어 있다. 명확한 예로 fopen, prin七f,
       malloc 그리고 memcpy 등과 같은 표준 C 라이브러리 루틴을 들 수 있다. 그 외의 다른
       예로는 어플리케이션에서 사용하는 여러 함수, 예를 들어 （저 치연성 오디오 서버인 JA（水
       이 제공하는 루틴인） jack transport loca七e () 와 같은 함수는 외부의 표준 C 라이브
       러리를 호출하게 된다.

       GDB에서 이들 루틴까지 포함한 디버그 심볼 정보를 사용하기 위해서는 다음 두 가지 조건
       이 충족되어야 한다．

         口 각 라이브러리의 디버그 버전 바이너리를 가지고 있어야 함．
         口 GDB가 그 바이너리들을 어디서 찾을지 알려 주어야 함．

       만약에 각 라이브러리의 디버그 버전 바이너리가 없더라도 어플리케이션 디버깅은 여전히 진
       행할 수 있다. 하지만 해당 라이브러리 루틴을 호출하는 부분에서는 디버그 정보를 사용할
       수 없다. 사실 대부분의 경우 임베디드 시스템을 위한 공유 라이브러리 자체를 개발하는 경
       우가 아니라면 공유 라이브러리에 대한 디버깅 정보 없이도 충분히 디버깅을 진행할 수 있다．

       원격의 타깃에 있는 GDB를 호출하는 ［리스트 15-4］를 다시 보자. GDB가 target
       remo七e 명령으로 타깃과 연결되고 나면 다음 두 줄의 응답을 출력한다．



         Remote debugging using 192. 168.1.141: 2001
         0x40000790 in?? 0




 496
                                     임베디드 리눅스 어플리케이션 디버깅하기          Chapter 15




이 내용은 GDB가 해당 II) 주소와 포트를 이용해서 타깃에 연결되었음을 확인시켜 준다．
그리고 GDB는 프로그램 카운터의 위치를 0x40000790이라고 보고한다. 하지만 여기에 왜
심볼 정보로 표시된 위치가 나오지 않고 물음표가 나오는 것일까9 이는 리눅스의 동적 로더
(id-x. y. z. so）와 해당 플랫폼을 위한 공유 라이브러리 디버그 심볼 정보를 가지고 있지
않기 때문이다. 그렇다면 이 정보를 어떻게 알 수 있을까？

9장, "파일 시스템"에서 /proc 파일 시스템에 대해서 설명했던 부분을 다시 상기해 보자．
이 파일 시스템에서 참고할 만한 유용한 항목으로 각 프로세스 디렉터리마다 존재하는 maps
라는 항목이 있다（9장에 있는 ［리스트 9-16] 참고）. gdbserver가 출력한 내용을 통해서
타깃 어플리케이션의 프로세스 ID(PIT기를 알 수 있다. 우리 프로세스의 경우 PID가 197번
이었다. 이를 이용해서 프로세스가 시작된 직후에 사용중인 메모리 세그먼트의 매핑 정보를
확인해 볼 수 있다. ［리스트 15巾6］을 보자．

C리스트 ]5-6] 초기 타깃 어플리케이션의 메모리 세그먼트 매핑


  root@coyote: # cat /proc/197/maps
  00008000-0002 6000 r- xp 00000000 00: 0e 4852444   ./websdemo- stri pped
  0002d000- 0002e000 rw巾 0001d000 00: 0e 4852444     ./websdemo- stri pped
  40000000- 40017000 r- xp 00000000 00: 0a 4982583   /lib/ ld- 2. 3. 3. so
  4001e000- 40020000 rw-p 00016000 00: 0a 4982583    /lib/ ld-2. 3. 3. so
  bedf9000- bee0e000 rwxp bedf9000 00: 00 0            [stack]
  root@coyote : 硝




위 내용에서 타깃의 websdemo-s七ripped 어플리케이션이 두 개의 메모리 세그먼트를 차
지하고 있는 것을 볼 수 있다. 첫 번째 것은 0x8000에 있는 읽기 전용의 실행 가능한 세그먼
트이다. 그리고 두 번째 0x2d000에 있는 세그먼트는 읽기 , 쓰기가 가능한 데이터 세그먼트
이다. 세 번째 세그먼트가 흥미로운 것 중의 하나인데 , 리눅스의 동적 링커를 위한 실행 가능
코드 세그먼트이다. 주목할 부분은 이 세그먼트가 0x40000000 주소에서 시작한다는 것이
다. 조금 더 연구해 보면 실제로 우리 어플리케이션의 코드가 수행되기 전에 동적 링커에 해
당하는 코드의 맨 처음 줄에 멈춰 있는 것을 확인할 수 있다. 교차 버전의 readeif를 이용
해서 링커의 시작 주소를 다음과 같이 확인해 볼 수 있다．




                                                                             497I
 麟U      Embedded Linux Primer




         # xscale_be- reade卄 -s ld- 2.3.3.so I grep \.text
         [9] .text    PROGBITS  00000790 000790 012c6c 00 AX 0       0 16




       이 데이터를 통해서 GDB가 처음 프로그램 카운터라고 보고하는 부분이 리눅스 동적 로더
       및 링커인 ld-2.3.3. so의 맨 처음 명령어인 것을 알 수 있다. 이런 방법은 프로세스나 공
       유 라이브러리를 위한 심볼릭 디버그 정보를 가지고 있지 않을 때 사용할 수 있다．

       여기서 사용하는 readeif 명령은 개발 호스트에서 실행되는 교차 버전인 것을 기억하기 바
       란다. 그렇기 때문에 엑스스케일 바이너리 파일인 ld-2. 3. 3. so 파일을 개발 호스트에서
       접근할 수 있어야 한다. 가장 일반적인 경우는 이 파일이 임베디드 리눅스 배포 버전으로서
       호스트 시스템에 설치되어 있는 것이다．


15.3.1 GDB의 공유 라이브러리 이벤트

       GDB는 공유 라이브러리 이벤트에 대해서도 알려주는데 , 이는 어플리케이션과 리눅스 로더
       의 동작 방식을 이해하는 데 좋을 뿐 아니라 디버그하거나 한 단계씩 실행시켜 보고자 하는
       공유 라이브러리에 브레이크 포인트를 설정하는 데도 유용하게 사용할 수 있다. ［리스트
       15-7］에서 그 사용법을 볼 수 있다. 실제로는 공유 라이브러리의 전체 경로가 표시되지만，
       여기서는 가독성을 위해서 편집했다．

       ［리스트 ]5-7] 공유 라이브러리 이벤트 시에 GDB 정지시키기


         $ xscale_be-gdb -q websdemo
         (gdb) target remote 192.168.1.141:2001
         Remote debugging using 192.168.1.141: 2001
         0x40000790 in?? 0
         (gdb) i shared       <<< 이미 로드된 공유 라이브러리 표시
         No shared libraries loaded at this time.
         (gdb) b main        <<< main에 브레이크 포인트 설정
         Breakpoint 1 at 0x12b80: file main. c, line 72.
         (gdb) C
         conti nui ng.

         Breakpoint 1, main (argc=oxl, argv=0xbec7fdc4) at main. c: 72
         72             m nt localvar = 9;


 498
                                        임베디드 리눅스 어플리케이션 디버깅하기              Chapter 15



  (gdb) i shared
  From       To         syms Read Shared Object Library
  0x40033300  0x4010260c   Yes       /opt/mvl/ . . ./lib/ tls/ libc. so. 6
  0x40000790 0x400133fc Yes          /opt/mvl/ . . ./lib/ ld-linux.so. 3
  (gdb) set stop-on- solib-events 1
  (gdb) C
  Continuing.
  Stopped due to shared library event
  (gdb) i shared
  From       To         Syms Read shared Object Library
  0x40033300 0x4010260c Yes          /opt/mvl/ . . . /] 化／tls/ ] 卄兀 . so . 6
  0x40000790 0x400133fc Yes          /opt/mvl/. . ./lib/ ld-linux. so. 3
  0x4012bad8 0x40132104 Yes          /opt/mvl/ . . ./libnss_files. so. 2
  (gdb)



물론 디버그 세션이 처음 시작되면 아무런 공유 라이브러리도 로드된 것이 없다. 이는 첫 번
째 i shared 명령을 통해서 볼 수 있는데 , 이 명령은 현재 로드되어 있는 공유 라이브러리
를 표시해 준다. 어플리케이션의 main () 함수에 브레이크 포인트를 건 후에 실행했을 때는
두 개의 라이브러리가 로드된 것을 확인할 수 있다. 이들은 각각 리눅스 동적 로더／링커와
표준 C 라이브러리인 iibc이다．

이제 set st아느on田olib-event 명령을 내리고 프로그램을 계속 진행시킨다. 어플리케
이션에서 다른 공유 라이브러리에 있는 함수를 실행하려고 하면 그 라이브러리가 로드될 것
이다. 궁금하다면 gethos난가name () 함수가 실행돼서 다음 공유 오브젝트가 로드되는 것
을 확인할 수 있다．

위 예제는 교차개발의 중요한 개념을 설명해 준다. 즉, 타깃에서 실행되는 바이너리 어플리
케이션（ELF 이미지）에는 외부 참조의 주소 값을 해결하기 위해서 필요한 라이브러리 관련
정보를 포함하고 있다. 11장, "BusyBox"와 13장에서 자세히 설명한 idd 명령어를 이용하
면 이 정보를 쉽게 확인해 볼 수 있다. ［리스트 15-8］은 타깃 보드에서 idd를 실행한 결과를
나타낸 것이다．

［리스트 ]5-8) 타깃 보드에서 tdd릍 실행시킨 결과

  root@coyote : /workspace# 1dd websdemo
         libc. so. 6=>/lib/ tls/ libc. so. 6 (0x40020000)


                                                                                 499
 ! 難二     Embedded Linux Primer




                 /lib/ ld-linux. so. 3    (0x40000000)
          root@coyote : /workspace#



        여기서 타깃에 있는 공유 라이브러리의 경로는 루트 파일 시스템에서 /lib으로 시작하는 절
        대 경로라는 것을 주의하도록 하자. 하지만, 개발 호스트 시스템에서는 라이브러리를 찾기
        위해서 이 경로를 바로 사용할 수 없다. 만약에 그렇게 할 경우에는 다른 아키텍처에서 사용
        하는 라이브러리를 참조하게 된다. 보통 호스트 시스템은 x86 기반이고, 타깃은 이 예에서는
        ARM 엑스스케일이다．

        교차 idd를 실행시키면 사용하는 툴 체인에 설정된 경로를 볼 수 있다. 툴 체인은 참조할
        라이브러리가 호스트 개발 시스템에서는 어디에 위치하고 있는지에 대한 정보를 갖고 있어
        야3) 한다. ［리스트 15-9］에서 이 내용을 확인할 수 있다. 이 내용 역시 가독성을 위해서
        긴 경로명을 짧게 축약해서 나타낸 것임을 알아두자．

        ［리스트 ]5-9] 개발 호스트에서 idd 실행시키기

          $ xscal e그犯-1dd      叫ebsdeino
            libc. so. 6 => /opt/mvl/ . . ./xscale_be/target/lib/ libc. so. 6 (Oxdeadl000)
            ld-linux.so. 3 => /opt/mvl/. . ./xscale_be/target/l化/ld-linux. so. 3 (0xdead2000)
          $



        사용하는 툴 체인에서 이들 라이브러리의 위치를 미리 설정해 두도록 하자 호스트의 GDB
        는 물론이고 컴파일러와 링커도 이들 파일이 어디에 위치하는지 알아야 한다. GDB에서는
        show solib-absolu七e-pref ix 명령을 통해서 이들 라이브러리를 어디서 찾도록 구성되
        어 있는지 확인해 볼 수 있다．



          (gdb) show so] i b-absolute-prefix
          Prefix for loading absolute shared library symbol files is
          "/opt/mvl /pro/devki t/ arm/ xscal e_be/target".
          (gdb)



3) 물론 컴파일러, 링커 그리고 디버거를 매번 실행할 때마다 이 위치를 0苾｝로 넘겨줄 수도 있다. 하지만 좋은 리눅스 배포 버젼
  은 개발자의 편의를 위해서 툴 체인의 기본 값으로 이 위치를 설정해 준디．



I 500
                                         임베디드 리눅스 어플리케이션 디버깅하기                     Chapter 15




GDB가 공유 라이브러리를 검색하는 위치를 변경하기 위해서는 GDB 명령어인 set solib
-absolute中prefix와 set solib中search-path를 이용한다. 만약에 공유 라이브러리
를 개발하고 있거나 시스템에서 자체적으로 사용하는 라이브러리 경로를 가지고 있는 경우에
는 GDB가 어디서 그 라이브러리를 찾을지를 지시하기 위해서 solib-search-path를 사
용해야 한다. 추가적인 내용은 이 장의 마지막에 있는 15.6.1절 "더 읽어 보기"에 나와 있는
GDB 온라인 매뉴얼을 참고하도록 하자．

ldd에 대해서 마치막으로 한 가지만 짚고 넘어가자. ［리스트 15-8］과 ［리스트 15-9］에서
각 라이브러리에 할당된 주소를 보자. 마치 프로그램이 리눅스 동적 로더와 링커를 통해서
실제로 로드된 것처럼 코드 세그먼트가 로드된 시작 주소를 표시해 준다. 타깃에서 실행되면
［리스트 15-5］에 있는 주소 값을 완전히 이해할 수 있다. 그리고 타깃에서 실행중인 프로세
스에 해당하는 /proc/<pid>/maps어］ 있는 항목과도 연관지어 볼 수 있다. ［리스트 15-
10］에는 이 타깃 프로세스가 완전히 로드되어 실행중일 때의 메모리 세그먼트를 나타낸 것
이다．

［리스트 ]5-10] 타깃의 加rocl<pid>Imaps에 있는 메모리 세그먼트

 root@coy야；e : 싸 # cat /proc/ 197/ xnaps
 00008000-00026000 r- xp 00000000 00: 0e     4852444   /workspace/websdemo- stripped
 0002d000- 0002e000 rw-p 0001d000 00: 0e     4852444   /workspace/websdonio- stripped
 00 02e00 0-000 5e000 rwxp 0002e000 00: 00   0         (hear기
 40000000- 40017000 r- xp 00000000 00: 0a    4982583   /lib/ 1d-2. 3. 3. so
 40017000-40019000 rw-p 40017000 00: 00      0
 40010000- 4001f000 r- -p 00016000 00: oa    4982583   /lib/   ld- 2.3. 3. so
 4001f000-40020000 rw-p 00017000 00: oa      4982583   /lib/   ld- 2.3. 3. so
 40020000-4011d000 r- xp 00000000 00: oa     4982651   /lib/   tls/ libc- 2 .3. 3. 80
 4011d000- 40120000 ---p 000fd000 00: 0a     4982651   /lib/   tls/ libc- 2 .3. 3. so
 40120000- 40124000 rw-p 000f8000 00: 0a     4982651   /lib/   tls/ libc- 2 .3. 3. so
 40124000- 40126000 r- -p 000fc000 00: 0a    4982651   /lib/   tls/ libc- 2. 3. 3. so
 40126000- 40128000 rw-p 000fe000 00: 0a     4982651   /lib/   tls/ libc- 2 .3. 3.日0
 40128000-4 012a0 00 r寸-p 40128000 00: 00    0
 4012a0 00- 40133000 r- xp 00000000 00: 0a   4982652   /lib/ tla/ libnss_ files- 2 .3. 3. 80
 40133000- 4013a000 ---p 00009000 00: 0a     4982652   / lib/ tls/ libnss_ f iles- 2 .3. 3. 80
 4013a000- 4013b000 r- -p 00008000 00: 0a    4982652   /lib/ tls/ libnss files- 2. 3.3. so
 4013b000-4013c000 rw-p 00009000 00: 0a      4982652   /lib/ tls/ libnss files- 2. 3 .3. 50
 becaa000-becbf 000 rwxp becaa000 00: 00     0         (stack]
 root9coy（北e : M古L




［리스트 15-8］에 있는 타깃 ldd의 출력과 위 /proc 파일 시스템에서 볼 수 있는 해당 프로
세스의 메모리 세그먼트의 관계를 주의해서 보도록 하자. 리눅스 로더의 시작 주소는
(.text 세그먼트의 시작 주소） 0x4 0000000이고 libc의 시작 주소는 0x40020000이다．
 難 二U    Embedded Linux Primer




      이 주소 값들은 어플리케이션이 로드된 영역의 가상 메모리 주소 값이고 타깃에서 ldd를 실
      행시켜서 확인해 볼 수 있다. 하지만 ［리스트 好9］에서처럼 교차 ldd에서 실행시켜서 볼
      수 있는 메모리 주소는（Oxdead1000과 0xdead2000) 호스트 시스템에서는 로드될 주소를
      알 수 없기 때문에 단순히 이 사항을 알려 주는 용도로 나타낸 것이다（로드될 바이너리는
      ARM 아키텍처를 위한 것이다）. 그래서 이 주소는 아무런 의미가 없다．



15.4 여러 태스크 디버깅하71
      다중 쓰레드가 실행중인 경우에 디버깅을 진행할 때는 일반적으로 두 가지 상황을 생각해 볼
      수 있다. 즉, 프로세스가 각자 독립된 주소 공간을 가지고 실행되거나 또는 여러 개의 쓰레드
      가 하나의 주소 공간（그리고 다른 시스템 자원）을 공유하는 경우가 있다. 전자의 경우는 （각
      각의 독립된 프로세스가 서로 주소 공간을 공유하지 않는 경우） 각각의 프로세스를 위한 별
      도의 디버그 세션을 가치고 디버킹해야 한다. 타깃 시스템에서 여러 프로세스에 gdbserver
      를 사용해도 아무런 문제가 없다. 또한 市入E두 여러 개의 GDB를 실행시켜서 각각의 독립
      된 프로세스를 디버깅할 수 있다．


15.4. ] 다중 프로세스 디버깅
      GDB로 디버깅 중인 프로세스에서 如rk () 시스템 콜4）을 사용해 새로운 프로세스를 시작
      하면 GDB는 이에 대해서 두 가지 행동을 취할 수 있다. 즉, 부모 프로세스를 가지고 계속
      디버깅을 진행하거나, 아니면 부모 프로세스를 디버깅하는 것을 그만두고, 새로 만들어진
      자식 프로세스에 붙어서 디버깅을 진행할 수 있다. 이 두 가지 방법 중의 한 가지를 결정하
      는 것은 se七 此hlow-fork-mode 명령을 통해서 할 수 있다. 두 가치 방법은 각각 부모를
      따르거나 자식을 따르거나를 결정할 수 있다. GDB의 기본 값은 부모를 따르도록 되어 있
      다. 이 경우에 자식 프로세스는 fork () 가 성공적으로 실행되자마자 곧바로 실행을 계속하
      게 된다.

      ［리스트 15-11］은 main () 루틴에서 여러 개의 프로세스를 此rk () 를 통해서 생성하는 간
      단한 프로그램을 나타낸 것이다．



4) 여기서는 시스템 콜이라는 용어를 사용했다. 하지만 실제로 的rkO 함수는 C 라이브러리 함수이고， 0] 함수가 결과적으로는 리눅
 스의 sysi야ko 시스템 콜을 호출하도록 되어 있다．
                                     임베디드 리눅스 어퓰리케이션 디버깅하기           Chapter 15




［리스트 ]5-11) 凡rk () 를 이용해써 자식 프로세스를 생성하는 코드



    for ( i=O; i<MAX_PROCESSES; i++ ) {
     ／士 자식 프로세스 만들기 소／
      pid[i] = forkO;                ／立 부모의 경우 0이 아닌 PID 반환 央／/
      if ( pid[i] == -1 ) {
        perror ("fork failed") ;
        exit (1) ;
        }
        if ( pid[i] == 0 ) {   /"" 자식 프로세스일 경우 실행되는 코드 士／
           worker_process 0;   ／玄 새로 생성된 프로세스가 호출할 함수 丹／
        }
    }

    ／六 부모 프로세스의 메인 루프 央／
    while ( 1 ) {


    }



이 간단한 반복문은 fork () 시스템 콜을 이용해서 MAX THREADS개만큼의 프로세스를 생
성한다. 각각의 새로 만들어진 프로세스는 worker process () 라는 함수에 있는 코드를 실
행시키게 된다. GDB를 별다른 설정 없이 기본 값으로 두고 실행한 경우에는 새로운 쓰레드
（프로세스）가 생성된 것을 감지하지만 여전히 부모 프로세스를 디버깅하는 상태를 유지할 것
이다. ［리스트 15-12］에서 해당하는 GDB 세션을 볼 수 있다．

［리스트 ]5-12) 此hlow- fork-mode = paren七인 경우


   (gdb) target remote 192.168.1.141:2001
   0x40000790 in?? 0
   (gdb) b main
   Breakpoint 1 at 0x8888: file forker. c, line 104.
   (gdb) C
   Cont-i nul ng.
   [New Thread 356]
   [switching to Thread 356]

   Breakpoint 1, main (argc=oxl, argv=0xbe807dd4) at forker. c:104
   104      time(&start_time) ;
         Embedded Linux Primer



         (gdb) b worker_process
         Breakpoint 2 at 0x8784: file forker. c, line 45.
         (gdb) c
         Conti nul ng.
         Detaching after fork from child process 357.
         Detaching after fork from child process 358.
         Detaching after fork from child process 359.
         Detaching after fork from child process 360.
         Detaching after fork from child process 361.
         Detaching after fork from child process 362.
         Detaching after fork from child process 363.
         Detaching after fork from child process 364.



      PT') 값 357에서 364까지 모두 여덟 개의 자식 프로세스가 생성된 것을 알 수 있다. 그리고
      부모 프로세스의 PIT）는 356이다. main (）어］ 정의해 놓은 브레이크 포인트를 만났을 때
      worker process () 루틴에 브레이크 포인트를 설정해 놓는데 , 이는 각 자식 프로세스가
      凡rk () 후에 실행을 계속하면서 부르게 되는 함수이다. main에서 프로그램을 계속 실행시
      키면 디버거를 통해서 각각의 새로운 프로세스가 생성되는 것을 확인해 볼 수 있다. 하지만
      GDB는 항상 부모 프로세스에 연결되어 있기 때문에 worker process () 루틴에 설정한
      브레이크 포인트는 절대 걸리지 않을 것이다.

      만약에 각각의 프로세스를 디버그하고 싶다면 별도의 GDB 세션을 실행시켜서 此rk () 후
      에 해당 자식 프로세스에 연결해야 한다. 이 장의 마지막에 있는 GDB 참고 자료에서 각 자
      식 프로세스에 sleep () 함수를 둠으로써 새로운 프로세스에 디버거를 연결시킬 시간을 확
      보해 쉽게 디버그 세션을 연결하는 방법을 참조할 수 있다. 새로운 프로세스에 디버거를 붙
      이는 방법은 15.5.2 절 "실행중인 프로세스에 연결하기"에서 볼 수 있다．

      만약에 그냥 단순히 자식 프로세스를 따라가면서 디버깅하고 싶다면 如rk () 시스템 콜이
      호출되기 전에 follow-fork-mode 설정을 자식 프로세스를 따라가도록 설정하면 된다．
      ［리스트 15-13］에 이 방법이 나와 있다．

      ［리스트 15-13) follow小且Drk니rode = child인 경우


        (gdb) target remote 192 .168.1.141:2001
        0x40000790 in?? 0
        (gdb) set follow- fork-mode child


504
                                        임베디드 리눅스 어플라케이션 디버깅하71   Chapter 15



      (gdb) b worker_process
      Breakpoint 1 at 0x8784: file forker. c, line 45.
      (gdb) C
      Conti nul ng.
      [New Thread 401]
      Attaching after fork to child process 402
      [New Thread 402]
      [Switching to Thread 402]
      Breakpoint 1, worker_process O at forker. c: 45
      45         mnt my_pid = getpid0;
      (gdb) c
      Conti nui ng.




   여기서 부모 프로세스가 PID 401인 것을 볼 수 있고, 此rk () 시스템 콜을 통해서 첫 번째
   자식 프로세스가 생성되면 GDB는 현재 부모 프로세스와의 연결을 조용히 끊고, 새롭게 생
   성된 자식 프로세스 PID 402와 연결하게 된다. 그러면 GDB는 첫 번째 자식 프로세스를
   디버깅할 수 있게 되고, worker process () 어］ 설정해 둔 브레이크 포인트도 걸리게 된다．
   하지만 ［리스트 15-11］에서 추가로 생성될 자식 프로세스는 디버킹할 수 없고, 스스로 실행
    을 완료할 것이다．

    요약하면 이런 방식으로 GDB를 이용하면 한 번에 하나의 프로세스만 디버깅할 수 있게 된
   다. fork () 시스템 콜을 통해서 디버깅을 계속할 수 있지만, fork () 호출의 결과 부모 또
    는 자식 프로세스 중 어느 프로세스를 선택해서 디버킹을 계속할지를 결정해야 한다. 이 섹
    션을 소개할 때 언급했듯이 한 번에 하나 이상의 프로세스를 디버깅하고자 할 때는 여러 개의
    독립된 GDB 세션을 이용할 수 있다．


15.4.2 다중 쓰레드 어풀리케이션 디버깅
    독자의 어플리케이션이 쓰레드를 위해서 POSIX 쓰레드 라이브러리를 이용한다면 GDB를
    통해서 다중 쓰레드 어플리케이션을 동시에 디버깅할 수 있다. 자체 POST)( 쓰레드 라이브
    러리（NPTL）는 임베디드 리눅스를 포함해서 사실상 모든 리눅스 시스템의 표준 쓰레드 라
    이브러리가 되었다. 지금부터 설명하는 내용은 이 쓰레드 라이브러리를 사용한다고 가정하고
    진행하겠다．




                                                                       505 1
        Embedded Linux Primer



      이 절에서는 간단한 반복문을 이용하여 몇 개의 쓰레드를 pthread crea七e () 라이브리리
      함수를 통해서 생성하는 예제를 이용할 것이다. 이 쓰레드들이 생성되고 나면 main () 함수
      는 프로그램을 종료하기 위한 키보드 입력을 기다리게 된다. 각 쓰레드는 짧은 메시찌를 화
      면에 출력하고 미리 정해진 시간만큼 슬립（slee히 상태로 들어가게 된다. ［리스트 15-14]
      에서 이 예제를 타깃 보드에서 실행시키는 처음 부분을 볼 수 있다．

      ［리스트 ]5-14] 쓰레드 예제 실행하71


        root@coyote: /workspace # gdbserver localhost: 2001 ./tdemo
        Process ./tdemo created; pid = 671
        Listening on port 2001
        Remote debugging from host 192.168.1.10
            八八八八八 위 세 줄은 gdbserver에 의해서 출력된 내용임

        tdemo main() entered: My pid is 671
        Starting worker thread 0
        starting worker thread 1
        starting worker thread 2
        starting worker thread 3



      이전 예제에서처럼 gdbserver는 어플리케이션을 실행할 준비를 하고 호스트에서 실행되는
      교차 gdl퍼 연결을 기다린다. GDB가 연결되면 gdbserver는 Remo七e debugging. . . 메
      시지를 통해서 연결을 알려 준다. 이제 GDB를 실행시켜서 타깃에 연결하자. ［리스트
      15-15七 이 추가적인 과정을 볼 수 있다．

      ［리스트 ]5-15) GDB로 타깃 시스템의 쓰레드 예제에 연켤

        $ xscale_be- gdb -q tdemo
        (gdb) target remote 192.168.1.141:2001
        0x40000790 in?? 0
        (gdb) b tdemo.c:97
        Breakpoint 1 at 0x88ec: file tdemo. c, line 97.
        (gdb) C
        Continuing.
        [New Thread 1059]
        [New Thread 1060]
        [New Thread 1061]
        [New Thread 1062]


506
                                     임베디드 리눅스 어플리케이션 디버깅하71        Chapter 15



  [New Thread 106311
  [switching to Thread 1059]

  Breakpoint 1, main (argc=oxl, argv=Oxbefffdd4) at tdemo. c:98
  98             mnt c = getcharO;
  (gdb)



여기서 타깃에 연결했고 （그 결과 ［리스트 15-14］에서 "Remote debugging. . . " 메시지가
출력되었다） 새로운 쓰레드를 생성하는 반복문 바로 다음에 브레이크 포인트를 설정하고 실
행을 진행시킨다. 새로운 쓰레드가 만들어지면 GDB는 해당 쓰레드 ID와 함께 쓰레드가 생
성되었다는 메시지를 출력한다. tdemo 어플리케이션의 쓰레드는 1059이고, 이 쓰레드는
main () 함수의 내용을 수행한다. 쓰레드 1060부터 1063까지가p나iread create () 함
수로 새로 생성된 쓰레드이다．

GDB가 브레이크 포인트를 만나면 새로운 쓰레드로 전환한다는 메시지인 [Switching 七0
Thread 1059] 를 출력해서 이 쓰레드에서 브레이크 포인트가 걸렸다고 표시해 준다. 이 쓰
레드가 GDB 문서에서 현재 쓰레드（curr帥t thread）라고 부르는 현재 디버깅 세션에서 활성화
된 쓰레드이다

GDB에서는 쓰레드 간에 전환을 할 수 있고, 선택된 쓰레드에 대해서 브레이크 포인트를 설
정하고 데이터를 확인하거나 스택 역추적 내용을 출력하고, 각 쓰레드의 스택 프레임을 가지
고 작업하는 등의 일을 할 수 있다. ［리스트 15-16］에서는 ［리스트 15-15］에 이어서 이들
작업 내용을 확인해 볼 수 있다．

［리스트 ]5-16) GDB의 쓰레드 디버깅



  (gdb) C
  Conti nul ng.
                  <<< 프로그램의 실행을 중단하기 위해서 ctl -c를 누름
  Program received signal SIGINT, Interrupt.
  0x400db9c0 in read 0 from /opt/mvl/. . ./lib/ tls/ 1ibc. so. 6
  (gdb) i threads
    5 Thread 1063 0x400bc714 in nanosleep 0
     from /opt/mvl/ . . ./lib/ tls/ libc. so. 6
    4 Thread 1062 0x400bc714 in nanosleep 0



                                                                         507 且
  難二   Embedded Linux Primer



           from /opt/mvl/. . ./lib/ tls/ l 卄c. so. 6
          3 Thread 1061 0x400bc714 in nanosleep 0
           from /opt/mvl/ . . ./lib/ tls/ libc. so. 6
          2 Thread 1060 0x400bc714 in nanosleep 0
           from /opt/mvl/. . ./l化/ tls/ l卄c. so. 6
       * 1 Thread 1059 0x400db9c0 in read 0
           from /opt/mvl/. . ./l化/ tls/ l 卄）c. so. 6
       (gdb) thread 4                   <<< 4번 쓰레드를 현재 쓰레드로 만듦
       [switching to thread 4 (Thread 1062) ]
       #0 0x400bc714 in nanosleep 0
           from /opt/mvl/. . ./l化/ tls/ libc. so. 6
       (gdb) bt
       #0 0x400bc714 in nanosleep 0
           from /opt/mvl/ . . ./lib/ tls/ libc. so. 6
       #1 0x400bc4a4 in _sleep (seconds=0x0) at sleep. c:137
       #2 0x00008678 in go_to_sleep (duration=0x5) at tdemo. c:18
       #3 0x00008710 in worker_2_ job (random=0x5) at tdemo. c: 36
       #4 0x00008814 in worker_thread (threadargs=0x2) at tdemo. c: 67
       #5 0x40025244 in start_thread (arg=Oxfffffdfc) at pthread_create. c: 261
       #6 0x400e8fa0 in clone 0 at. ./sysdeps/unix/ sysv/linux/arm/clone. S: 82
       #7 0x400e8fa0 in clone 0 at. ./sysdeps/unix/ sysv/linux/arm/clone. S: 82
       (gdb)    frame 3
       #3 0x00008710 in worker_2_job (random=0x5) at tdemo. c: 36
       36          go_to_si eep(random) ;

       (gdb) 1                  <<< 현재 어디에 있는지 소스를 출력함
       31    }
       32
       33    static void worker_2_ job(int random)
       34    {
       35       printfC't2 sleeping for %d\n", random) ;
       36       go_to_si eep(random) ;
       37    }
       38
       39    static vo化 叫orke口3_如b(int random)
       40    {
       (gdb)




508
                               임베디드 리눅스 어플리케이션 디버깅하기   Chapter 15




      몇 가지 짚고 넘어가도록 하자. GDB는 각 쓰레드에 대해서 고유한 번호를 할당하게 되고，
      각각의 쓰레드를 참조할 때 이 숫자를 이용한다. 그리고 어떤 쓰레드에 브레이크 포인트가
      걸리면 그 프로세스 내에 있는 모든 쓰레드가 디버깅을 하느라 일단 실행을 멈춘다. 그리고
      GDB는 현재 쓰레드에 대해서는 별표(*）를 표시해서 보여 준다. 그리고 각 쓰레드가 마치
      분리된 실행 컨텍스트를 갖고 있는 것처럼 각각의 쓰레드에 브레이크 포인트를 걸 수 있다．
      만약에 모든 쓰레드가 실행하는 공통된 코드 부분에 브레이크 포인트를 설정해 놓으면 그 부
      분을 최초로 실행하는 쓰레드에서 브레이크 포인트를 만날 것이다．

      이 장 뒤편에 있는 참고 자료에 있는 GDB 사용자 문서에서 다중 쓰레드 환경에 관련된 정보
      를 더 읽어 볼 수 있다．


15.4.3 부트로더 및 플래시에 있는 코드 디버깅

      플래시 메모리에 존재하는 코드를 디버깅하는 일에는 특별한 어려움이 따른다. 가장 명확한
      한계는 브레이크 포인트를 설정할 때 GDB와 gdbserver가 협동하는 방식에 있다. 14장에
      서5) GDB의 원격 시리얼 프로토콜을 설명할 때 어플리케이션에 브레이크 포인트가 어떻게
      삽입되는지를 알아봤다. GDB는 브레이크를 설정하고자 하는 부분에 아키텍처에 따라 제어
      권을디버거로넘기는특수한명령어를삽입했다. 하치만RUM이나플래시의 경우에는코드
       부분을 수정할 수 없기 때문에 , 이 방식으로 브레이크 포인트를 설정하는 방법은 사용할 수
       없다．

      대부분의 최신 프로세서는 이 문제를 해결할 수 있도록 디버그 레지스터를 몇 711 가지고 있
      다. 그리고 특정 아키텍처 및 프로세서를 위한 하드웨어 프로브나 스텁에서 이 기능을 사용
       할 수 있도록 지원해 주어야 한다. 그래서 일반적으로 RUM이나 플래시에 있는 코드를 디버
       킹할 때 가장 많이 사용하는 방법은 JTAG 하드웨어 프로브를 이용하는 것이다. 이 프로브를
       이용하면 프로세서의 하드웨어 브레이크 포인트를 설정할 수 있다. 이 내용은 14장에서 자세
       히 설명하고 있다. 14.4.2절 "JTAG 프로브를 이용한 디버깅"에서 세부 내용을 참고하도록
       하자．




5) 14장의 （리스트 l中旬를 보기 바란다．


                                                             509 1
        牡    Embedded Linux Primer




15.5 추가 원격 디버그 옵션
            원격 디버깅을 위해서 시리얼 포트를 사용해야 할 때가 있을 것이다. 그리고 이미 실행중인
            프로세스에 디버거를 붇일 수 있다면 매우 유용하게 쓸 수 있다. 간단하지만 유용하게 쓸 수
            있는 이 두 가지 기술을 여기서 설명하도록 하겠다．


15.5. ] 시리얼 포트로 디버깅하기

            시리얼 포트로 디버깅을 하는 것은 간단하다. 물론 타깃 보드에서 시리얼 콘솔과 같이 다른
            프로세스가 사용하지 않는 가용한 시리얼 포트를 가지고 있어야 한다. 물론 호스트도 마찬가
        지로 가용한 시리얼 포트를 가지고 있어야 한다. 만약 이 두 가지 조건만 만족된다면
            gdbserver어］ 인자로 전달했던 IP:Port 대신에 시리얼 포트를 명시해 주면 된다 호스트
            에서도 GDB를 호출할 때 인자로 시리얼 포트를 넘겨주면 된다.

            타깃에서는 다음과 같이 한다．



              root@coyote: /workspace # gdbserver IdevittysO ./tdemo
              Process ./tdemo created; pid = 698
              Remote debugging using /dev/ttySO



            그리고 호스트는 다음과 같다．



              $ xscale_be-gdb -q tdemo
              (gdb) target remote /dev/ttySl
              Remote debugging using /dev/ttySl
              0x40000790 in?? 0




15.5.2 실행중인 프로세스에 연켤하기

        만약에 프로세스를 종료하고 다시 시작하는 대신에 실행중인 프로세스를 직접 디버거로 연결
            할 수 있다면 아주 편리할 것이다. gdbserver를 이용해서 아주 쉽게 할 수 있다．


甘 510
                                       임베디드 라눅스 어플리케이션 디버깅하기         Chapter 15




      root@coyote: /workspace # ps ax I grep tdemo
       1030 pts/0    sl+    0:00 ./tdemo
      root@coyote: /workspace # gdbserver local host :2001 --attach 1030
      Attached; pid = 1030
      Listening on port 2001



    그리고 프로세스를 디버깅하는 일을 끝마칠 경우에는 gdb의 de七ach 명령을 이용하면 된다．
    이렇게 하면 타깃에서 실행중인 프로세스와 g아jserver도 연결을 끊게 되고 디버그 세션을
    종료하게 된다. 그리고 어플리케이션은 원래의 상태로 계속 실행될 것이다. 이 방법은 실행
    중인 프로그램을 시험할 때 아주 유용하다. 하지만 주의할 점은 프로세스에 디버거를 붙이고
    난 후에는 프로그램의 실행이 중단되고 사용자의 명령을 기다리는 상태가 된다는 것이다. 그
    래서 continue 명령을 내리거나 디버거의 연결을 다시 해제하는 등의 별도의 명령이 없으
    면 아무런 일도 하지 않는다. 그리고 디버거를 끊고 프로그램을 계속 실행하려면 디버깅 중
    의 거의 아무 때나 detach 명령을 내리면 된다.



15. 6 요약
     口 원격 （교차） 디버깅은 호스트 개발 시스템의 풍부한 자원을 이용해써 일반적으로 빈약한
        자원을 가진 타깃 시스템을 디버깅할 수 있게 해 준다．

     口 gdbserver는 타깃 시스템에서 실행되며, 호스트 개발 시스템에서 실행되는 교차 gdb
        와 타깃에서 실행되는 디버깅할 프로그램과의 아교 역할을 수행한다．

     口 호스트에 있는 GDB는 보통은 이더넷 연결을 통해써 타깃에 있는 gdbserver와 명령을
        주고받게 되어 있다. 여기서 GDB와 g아＞server 간의 통신에 사용되는 프로토콜이
        GDB 원격 시리얼 프로토콜이다．

     口 GDB는 공유 라이브러리 이벤트를 감지해써 멈출 수 있고, 자동으로 공유 라이브러리
        심볼을 로드할 수 있다. 그러기 위해서는 호스트어써 사용하는 툴 체인의 기본 검색 경
        로를 설정해야 한다. 다른 방법으로는 GDB 명령을 통해서 공유 라이브러리를 검색하는
        경로를 지정할 수도 있다．

     口 GDB는 여러 GDB 세션을 통해써 여러 개의 독립된 프로세스를 디버깅할 수 있다．




                                                                           511
 難 髓1   Embedded Linux Primer



        口 GDB는 fork () 시스템 콜로 생성된 프로세스를 따라서 디버깅하도록 구성할 수 있다．
           기본 설정은 且＞rk (）를 호출하는 현재 부모 프로세스를 계속 디버깅하는 것이다．

        口 GDB는 POSIX 쓰레드 API를 이용하는 다중 쓰레드를 어플리케이션도 디버깅할 수 있다．
           현재 리눅스의 기본 쓰레드 라이브러리는 자체 POSIX 쓰레드 라이브러리（NPTL）이다．

        口 GDB는 이미 실행중인 프로세스로 연결하거나 해제하는 기능도 지원한다．



15.6. ] 더 읽어 보기
        GDB: The GNU 프로젝트 디버거
        온라인 문서
        http: //sourceware. org/gdb/on1inedocs/


        GDB 포컷／ 라퍼런스
        Arnold Robbins
        O'Reilly Media, 2005




I 512
Chapter




                    리눅스 포팅




이번 장에서 배울 내용

  1 리눅스 入人 코드의 구조

  . 자체 보드를 위한 리눅스

  . 플랫폼 초기화

  U 한데 묶기

  U 요약
   如，   蔑     Embedded Linux Primer




            리눅스를 새로운 하드웨어 플랫폼에 포팅하는 것은 크기 어렵지는 않다. 리눅스 소스 코드는
        ·20개 이상의 아키텍처와 여러 개별 프로세서에 대한 포팅 코드를 담고 있다. 가장 어려운
            문제는 주로 어디서부터 시작할 것이냐 하는 선택이다．

            이 장에서는 리눅스를 이더넷과 시리얼 콘솔 기능을 지원하는 보드에 포팅하는 기본적인 절
            차를 설명하도록 하겠다. 아키텍처와 플랫폼 관점에서 리눅스 소스 코드가 어떻게 구성되어
            있는지 알아보고, 커널 초기화 코드를 분석해서 플랫폼 초기화를 위한 메커니즘을 이해해 보
            도록 하자. 마지막으로 새로운 PowerPC 하드웨어 플랫폼을 포팅하기 위한 기본 사항을 예
            를 들어 살펴보도록 하자．



16. ] 리눅스 소스 코드의 구조
            상당히 최근까지도 리눅스의 다앙한 버전을 관리하는 홈페이지1）가 매우 많았다. 즉，
            PowerPC 전용 리눅스 저장소도 있고, ARM을 위한 리눅스 저장소가 있는 식이다. 이는
            설계상 그런 것이 아니라 필요에 의한 것이다. 여러 개의 아키텍처 기반 구조를 하나의 기준
        커널에 통합시키는 작업은 시간이 많이 소모되기 때문에 , 해당 아키텍처를 위한 최신의 코드
        만 빠르게 접근하기 위해서 분리된 소스 코드를 유지하고 있었던 것이다．

        커널 개발자들은 이질적인 아키텍처를 모두 하나의 리눅스 커널 소스 코드로 통합하기 위해
            서 많은 노력을 하고 있다. 몇 가치 예외는 있지만, 현재 사용하고 있는 리눅스 커널 2.6이
            그 성과물이라고 할 수 있다. 지금은 www.kernel.org에서 다앙한 프로세서와 산업 표준인
            참조용 보드에서 동작하는 커널을 직접 다운로드해서 컴파일할 수 있게 되었다．


16.1. ] 아키텍처 브렌치
            4장, "다른 관점에서 본 리눅스 커널"에서 리눅스 커널 소스 트리의 전쳬적인 구조를 소개했
            었다. 이번 장에서는 리눅스 커널 소스 중에서도 아키텍처를 위한 디렉터리 부분을 주로 살
        펴보도록 할 것이다. ［리스트 16-1]은 최신 리눅스 스냅 샷에서 . . . /arch 디렉터리의 내
            용을 출력한 것이다. 4장에서 지적한 것처럼 최신 리눅스 소스 코드에서 . . - /arch 하위
            디렉터리는 크기 면에서는 두 번째로 크고, 파일 수로는 ( . . . /include 디렉터리는 빼고）
        가장 많은 파일을 갖고 있다. 파일 용량에서만 . . . /drivers가 더 크다.

l) 여기서 "홈페이지' 는 인터넷에 있는 웹 서버와 같은, 공개 소스 코드 저장소（rep油恤功를 말한다．


1514
                                                            리눅스 포팅      Chapter 16




［리스트 ]6-1 ] 리눅스 커널의 . . . larch 디렉터리의 내용


   [chris@pluto 1inux] $ is ./arch
   alpha crjs i386 ni68k            parisc     s390      sparc   v850
   arm    fry   1a64    rn68knornmu ppc        sh        5parc64 x86_64
   arm26 h8300 m32r mips            ppc64      sh64      urn     xtensa




이 목록에서 리눅스 커널 내부에서 모두 24개의 각기 다른 아키텍처를 지원하는 것을 볼 수
있다. 논의를 위해서 이 각각의 디렉터리를 아키텍처 브렌치라고 하도록 하자．

각 아키텍처 브렌치에는 공통된 요소가 포함되어 있다. 예를 들어 , 모든 최상위 아키텍처 브
렌치에는 Kconfig 파일이 있다. 5장을 다시 보면 Kcontig7} 커널 구성 유틸리티를 위한
파일임을 알 수 있다. 물론 각 아키텍처 최상위 디렉터리에는 해당하는 makefile도 있다．
그리고 모두 kernel이라는 하위 디렉터리를 가지고 있는데, 몇몇 커널 기능은 아키텍처에
의존적이기 때문이다. 그리고 두 개를 제외한 모든 디렉터리가 mm 하위 디렉터리를 가지고
있는데, 이 디렉터리는 아키텍처에 종속적인 메모리 관리 코드를 담고 있다．

그리고 많은 아키텍처 브렌치가 boot 디렉터리를 가지고 있는데, 이 디렉터리는 （자체
makefile을 통해서） 해당 아키텍처에서 동작하는 부팅 가능한 타깃을 만들기 위해서 사용된
다. 그리고 많은 아키텍처가mach中士로 시작하는 디렉터리도 가지고 있는데 , 하드웨어 플랫
폼과 사용하는 보드를 위한 코드를 담고 있다. 또 자주 볼 수 있는 디렉터리로는 configs가
있다. 이 디렉터리는 자주 사용되는 아키텍처를 위한 것인데 , 지원하는 하드웨어 플랫폼을
 위한 기본 구성 파일을 담고 있다．

 이 장 전반에 걸쳐서 PowerPC를 이용한 예제를 다룰 것이다. PowerPC 아키텍처는 다양
 한 프로세서와 보드를 지원하는 가장 인기 있는 아키텍처 중의 하나이다. ［리스트 16-2］에
 서 최신 리눅스 소스의 PowerPC 아키텍처 브렌치인 . . . /arch/ppc에서（兀nfigs 디렉터
 리의 내용을 볼 수 있다．

［리스트 ]6-2) PowerPC의 cc江if igs 디렉터리 내용


    [chri s@pl uto 1i flux] $ is ./arch/ppc/configs/
    ads8272_defconfi g IvMS8_defconfi g              prpmc750. defconfi g
    apus_defconfi g          katana_defconfig        prpmc800_ defconfi g
    bamboo_defconfi   g      11 te5200_defconfi g    radstone_defconfi g


                                                                               515 山
       Embedded Linux Primer



        bsei p_defconfi g      1 opec_defconfi g        redwood 5_defconfi g
        bubinga_defconi9g      luan_defconfig           redwood6_defconfi g
        chestriut_defconfi g   mbx_defconfi g           rpx8260_defconfig
        common_defconfl g      mpc834x_sys_defconfi g   rpxcllf_defconfig
        cpci 405_defconfi g    뺘）c8540_a小_defconfig     rpxl i te_defconfl g
        cpci 690_defconfi g    뺘）c8548_c小펴計config       sandpoint_defconfjg
        ebony_defconfi g       뺘）c8555工必펴計conf1g        spruce_defconfig
        ep405_defconfi g       뺘）c8560코必펴計config        stx_gp3_defconfig
        est8260_defconfi g     mpc86x_ads_defconfig     sycamore_defconfi g
        ev64260_defconfl g     mpc885ads_defconfig      TQM823L_defconfig
        ev64360_defconfl g     mvmeS100_defconfl g      TQM8260_defconfi g
        FADS_defconfl g        ocotea_defconfi g        TQM850L_defconfi g
        gemi ni_defconf-ig     pmac_defconfl g          TQM860L_defconfi g
        hdpu_defconf-i g       power3_defconfig         wal nut_defconfi g
        ibmchrp_defconfig      ppl us_defconfl g



      이 PowerPC 아키텍처의 configs 디렉터리의 각 항목은 하나의 하드웨어 플랫폼을 포팅하
      기 위한 항목을 나타낸다. 예를 들어 , walnut defoonfig는 AMCC 왈넛(Walnut)
      PPC405 평가 플랫폼을 위한 기본 구성 값을 정의하고 있는 파일이다. 그리고 mpc8540
      ads defconfig 파일은 프리스케일 MPC8540 ADS 평가용 보드를 위한 기본 구성 파일
      을 나타낸다. 4장에서 설명한 것치럼 이 참조용 플랫폼을 위한 커널을 빌드하기 위해서는
      다음과 같이 커널 소스 트리를 헤당 구성 기본 값으로 설정해야 한다．

        $ make ARCH=ppc CROSS_COMPILE=ppc_85xx- mpc8540_ads_defconfig


      （리눅스 촤상위 디렉터리에서 실행시키는） 이 make 명령은 커널 소스 트리를 프리스케일
      MPC8540 ADS 평가용 보드를 위해서 기본 구성 값들로 설정할 것이다．

      리눅스 커널 소스에서 아직 천체적인 통합이 이루어치지 않은 부분 중의 하나가 각각의 아키
      텍처가 특정 플랫폼을 위한 파일을 관리하는 방식이다. PowerPC의 경우는 pla七forms라
      는 디렉터리가 각 플랫폼에 해당하는 코드를 담고 있는 것을 볼 수 있다. 이 디렉터리를 천체
      적으로 살펴보면 각 하드웨어 플랫폼 이름으로 시작하는 소스 파일을 많이 볼 수 있다. 또한
      . . ./arch/ppc/platforms 디렉터리 밑에 PowerPC 계열을 위한 하위 디렉터리도 몇
      개 있는 것을 확인할 수 있다．




516
                                                리눅스 포팅   Chapter 16



     하지만 ARM 아키텍처의 경우에는 mach-士 계열의 디렉터리를 가지고 있고, 각각이 특정
     하드웨어 플랫폼을 나타낸다. 그리고 MIPS 아키텍처는 각 플랫폼의 이름으로 된 하위 디렉
     터리를 가지고 있다．



16.2 자체 보드를 위한 리눅스
    U-Boot를 새로운 하드웨어 플랫폼에 포팅하는 내용을 7장, "부트로더"에서 설명할 때 , 우리
    가 사용한 방법은 기존에 포팅된 플랫폼 중에서 새로운 보드와 가장 근접한 것을 찾아서 기반
    으로 사용하는 것이었다. 새로운 보드에 리눅스를 포팅하는 데도 비슷한 방법을 이용할 수
    있다. 여기서도 선택한 CPU가 이미 커널에서 지원하는 것이라고 가정할 것이다. 새로운
    CPU를 커널에 포팅하는 것은 훨씬 더 어렵고, 이 책의 범위를 벗어난다．

    예제로 프리스케일 MPC5200 32비트 임베디드 PowerPC 프로세서를 장착해 자체 제작한
    보드를 이용하기로 하자. 최신 리눅스 코드에 있는（［리스트 16-2］에 나오는） 기본 구성 파
    일을 살펴보면 거기에 MPC5200 CPU도 포함되어 있는 것을 볼 수 있다. 이 프로세서를
    지원하는 파일은 하나뿐인 것 같다. 이 파일을 기반으로 삼도록 하자．

    이 예제에서 사용할 하드웨어 플랫폼은 UEI(United Electronics Industry）의 배려로 저］
    공받은 것이다. 이 보드는 파워DNA(PowerDNA) 컨트롤러라고 불리는데 , 간단한 요소로
    이루어져 있다. 이 요소에는 보드에 부착된 플래시 메모리 , DRAM, 시리얼 포트 그리고 다
    양한 입출력 장치가 포함되어 있고, 대부분의 요소가 MPC5200 프로세서에 통합되어 있다．
    ［그림 16-1]은 파워DNA 컨트롤러의 블록 다이어그램을 나타낸 것이다．


16.2. ] 선행 조건과 가정
    리눅스 커널은 부트로더로부터 제어권을 넘겨받을 때 몇 가치 기본적인 사항을 가정하게 된
    다. 그 중에서도 가장 중요한 것은 부트로더가 이미 DRAM 컨트롤러를 초기화했을 것이라
    는 가정이다. 리눅스는 칩 레벨에서까지 SDRAM 컨트롤러를 제어하지 않는다. 대신 리눅스
    는 시스템의 RAM이 이미 존재하고 충분한 기능을 할 수 있도록 준비되어 있다고 가정한다．
    파워DNA 컨트롤러도 U-Boot 부트로더를 가지고 있고, 여기서 CPU와 DRAM 등의 시스
    템이 동작하는 데 필요한 최소한의 하드웨어를 초기화한다.




                                                            引71
       Embedded Linux Primer




                                                             DDR
                                                  플래시       SDRAM
                               4 DC/DC
       전원 입력                                        I         1



                                                                         지 百 싣＞ 邕 삐 五 딤
      RJ-45 또는 Sc                                 프리스케일        어직
                                  NIC             MPC52OO      제로
                                                  PowerPC
      RJ中45 또는 Sc



                                                             분리화

         USB            상태 LED           RS-232     SD      1 In/i Out
                                                               Sync

      I 그림 ]6-1 UEI 파워DNA 컨트롤러 보드


      부트로더에서 시스템의 메모리 맵도 초기화해야 하는데 , 이는 보통 프로세서의 레지스터를
      설정해서 특정 메모리 주소 영역을 접근할 때 어떤 칩 선택 신호를 보낼 것인지를 설정하게
      된다. 프리스케일 MPC5200 사용자 가이드의 3장을 보면 이 작업을 위한 레지스터 설명을
      볼 수 있다．

      부트로더는 필요에 따라서 다른 추가적인 하드웨어 초기화 작업도 수행해야 하는데 , 일부 보
      드에서는 커널이 시리얼 포트가 이미 초기화되어 있다고 가정하는 경우도 있기 때문이다. 이
      렇게 할 경우 커널의 자체적인 시리얼 드라이버가 설치되기 전에도 초기 부팅 시점에 커널
      부팅 메시지를 시리얼 포트로 출력할 수 있기 때문이다. 일부 아키텍처와 하드웨어 플랫폼은
      出 serialputc () 와 같은 함수를 갖고 있어서 부트로더 또는 커널의 초기 설정 코드에서
      간단히 초기화해 놓은 시리얼 포트를 이용해 문자열을 출력한다. 이 예에 대해서는 Powerl毛
      아키텍처 하위 디렉터리에서 grep으로 CONFIG SERIAL TEXT DEBUG을 검색해 보면 찾
      을 수 있다．




518
                                                            리눅스 포팅        Chapter 16




    요약하면 우리의 새로운 보드에 리눅스를 포팅하기 위해서 필요한 기본 선행 조건이 부트로
    더가 이미 포팅되어서 보드에 설치되어 있어야 한다는 것과 보드를 위한 로우 레벨 하드웨어
    초기화가 모두 완료되어 있어야 한다는 것이다. 하지만 이더넷이나 I2C 컨트롤러와 같이 리
    눅스가 자체적인 디바이스 드라이버를 가지고 있는 하드웨어에 대해서까지 초기화되어 있어
    야 할 필요는 없다．

    그리고 자신이 가지고 있는 보드와 가장 비슷한 리눅스 커널 포팅 코드를 기반으로 해서 구성
    및 빌드를 진행하는 것이 좋다. 이렇게 하면 자신의 보드를 위한 기반 코드로 삼을 수 있는
    에러 없는 코드를가지고 포팅을시작할수 있기 때문이다. 5장, "커널 초기화'에서 본 커널을
    컴파일하는 명령을 다시 보자．

      $ 1 ake ARCH=ppc CROSS_COMPILE=ppc_82xx- ulmage


    이 명령어는 U-Boot와 호환 가능한 리눅스 부팅 이미지를 만들어 준다. ulmage라는 이름
    의 타깃이 이 작업을 명시한다．


16.2.2 커널 초기화 커스터마이징
    이제 시작으로 삼을 만한 기본 커널 소스 코드를 준비했기 때문에 보드에 필요한 작업을 결정
    해 보도록 하자. PowerPC 아키텍처에서 보드에 필요한 파일은 . . . /arch/ppc/
    platforms라는 디렉터리에 존재하는 것을 알고 있다. 물론 반드시 필요한 것은 아니지만
    자신이 작업한 내용을 패치로 리눅스 커널 개발 커뮤니티에 제출하고자 할 경우에는 올바른
    형식과 일관성을 갖추는 것이 중요하다！

    platforms 디렉터리에서 1ite5200.c라는 파일을 볼 수 있다. 아주 간단한 파일인데 , 두
    개의 구조체와 다섯 개의 함수를 정의하고 있다. ［리스트 16-3］에 이 함수들을 나타냈다．

   ［리스트 16-3] 5200 플랫폼 파일에 있는 함수들


      ] 卄e5200_sho叫m叩uinfo()     /"" Prints user specified text string "" /
      ii te5200map.J rq 0        /""" Sets h/w specific tNT logic routing "' /
      1ite5200_setup_cpuO        /""' CPU specific initialization "'" /
      1ite5200_setup_archO       /士 Arch. specific initialization */
      platform_i ni to           /央 Machine or board specific mnit */




                                                                                 519
       Embedded Linux Primer




      이제 이들 함수가 어떻게 사용되는지 보도록 하자. 이미 5장에서 로우 레벨의 커널 초기화를
      대략적으로 살펴보았기 때문에 여기서는 해당 아키텍처를 중점으로 자세히 보도록 할 것이
      다. 아키텍처 간에 세부적인 내용은 다르지만, 한 가지를 이해한다면 다른 것들도 쉽게 이해
      할 수 있다．

      5장에서는 보드에 전원이 공급된 후에 제어권이 어떻게 흘러가는지 설명했었다. 부트로더가
      커널의 부드入E랩 코드로 제어권을 넘기고, 이 부드入E랩 코드는 다시 커널의 head. o 모
      듈을 통해서 리눅스 커널로 제어권을 넘겨주도록 되어 있다. 여기서 특정 플랫폼을 위한 초
      기화가 시작되는데 , ［리스트 16尸4］에 . . . /arch/ppc/ kernei/head. S에서 관련된 부분
      을 다시 나타냈다．

      ［리스트 ]6-4] 초기 머신 초기화 함수를 호출하는 부분



        /k
             "" Do early bootinfo parsing, platform- specific initialization,
             * and set up the MMU.
             "
             山   /
                     mr   r3, r31
                     mr   r4, r30
                     mr   r5, r29
                     mr   r6, r28
                     mr   r7, r27
                     hi   machi ne_i nit
                     bi   MMU_init




      여기서 이 어셈블리 언어로 된 코드가 machine mni七이라는 함수를 호출하는 것을 알 수
      있다. 특별히 중요한 부분은 레지스터 r3에서 r7까지를 설정하는 부분이다. 이 레지스터들
      은 잘 알려진 값을 가치고 있어야 하는데 , 잠깐 살펴보도록 하자. 이 레지스터들은 부팅의
      매우 이른 초기 시점에 PowerPC의 범용 레지스터인 r27에서 r31까지의 레지스터에 내용
      을 저장해 두고 있다가, 위 코드에서 다시 원래의 값으로 로드하고 있다．

      machine init () 함수는 같은 아키텍처 커널 디렉터리인 . . - /arch/ppc/kernel／에
      위치한 setup . C라는 C 파일에 정의되어 있다. 이 함수의 시작 부분을 ［리스트 16旬에서
      볼 수 있다．


520
                                                                         리눅스 포팅   Chapter 16



      ［리스트 ]6-5) setup. c의 machine mnit () 함수


         vo化    m nit
         machine_init (unsigned long r3, unsigned long r4, unsigned long r5,
                    unsigned long r6, unsigned long r7)
          {
         #ifdef C0NFIG_CMDLINE
               strlcpy (cmd_line, C0NFIG_CMDLINE, sizeof (cmd_1ine) );
         #endif /"" C0NFIG_CMDLINE 出 /
         #ifdef C0NFIG6xx
                ppc_nid. power_save = ppc6xx_idle;
         #endif
         判 fdef C0NFIG寸P0WER4
                  ppc_md. power_save = power4Jd1e;
         #endif

              platform_init (r3, r4, r5, r6, r7) ;


              if (ppc_md. progress)
                     ppc_nid. progress ( ' id niachO: done ", 0x200) ;
         }


      이 간단한 함수에서 몇 가지 유용한 지식을 얻을 수 있다. 먼저 machine mni七 () 어］ 전달하
      는 파라미터2) 7} Powerl兀의 범용 레지스터인 r3에서 r7까지의 레지스터라는 점이다. 이
      미 본 것처럼 어셈블리 코드에서 machine mit을 호출하기 전에 이들 레지스터를 먼저 설
      정한다. 그리고 ［리스트 16-5］에서 볼 수 있는 것처럼 이들 레지스터 값이 수정 없이
      platform mnit () 함수로 천달된다. 이 함수를 우리 플랫폼에 맞도록 수정해야 한다（이
      부분에 대해서는 잠시 후에 더 이야기할 것이다）.

      ［리스트 16-5］에는 전원 관리 함수를 위한 내용도 일부 포함하고 있다. 만약에 커널을
      PowerPC 6xx를 지원하도록 구성한 경우에는（. config 파일에 CONFIG 6x刃下 정의된 경
      우） 이 머신을 위한 전원 관리 함수（ppc6＞也idle）에 대한 포인터가 구조체에 저장된다．
      비슷한 방식으로 커널이 PowerPC G5 코어를 지원하도록 구성되었다면（CONFIG
      POWER4) 이 머신을 위한 전용 전원 관리 함수가 같은 구조체의 멤버에 저장될 것이다. 이
      구조체에 대해서는 16.3.3절 "머신 종속적인 호출'에서 설명한다．

2) 편의상 C 함수로 전딜되는 파라미터는 이들 PowerPC 레지스터를 이용한다．


                                                                                       521 i
           Embedded Linux Primer




16.2.3 정적인 커널 커맨드 라인
    ［리스트 16-5］에 나오는 machine init () 함수의 다른 흥미로운 내용은 기본 커널 커맨
    드 라인을 저장하는 부분이다. 이 코드는 커널 구성 옵션에서 CONFIG C卜4DLINE이 설정된
    경우에 활성화된다. 일부 플랫폼에서는 부트로더가 커널 커맨드 라인을 지원하지 않기 때문
    에 이 옵션을 이용해서 정적으로 커널 커맨드 라인 문자열을 커널에 포함시켜서 컴파일하는
    것이다. ［그림 16-2］에서 이 구성 옵션에 해당하는 메뉴 항목을 볼 수 있다．

    日e        Qp에S        毖텨p

          嘲 ［그 長쿄                 1     n 卜      曲     呼
         Bar느 Load Say目 Sir.퍼e Sp奴 Eu打 Collaps욘 Es口帥d

        Opti｛겨15                                 Namem         1寸 비Y \／出ue                                 ！스

           P川2,r,......5
          b 口Machi爬丁ype                                                  Freescale 나TEE2IJ0I0c쏸Cube)
             口Symmetnc m너作proces引ngsupport       SMP           N     -. N                                  \
             口啣hm帥｝싸supp가t                       HEGHMEM       N     -   N                                 /
          仁 口Timer frequen댜                                              250 I-Il
    ,     b 口Pr놘em的on帥蜘1                                                 卜把Fo旺ed Pr쏸핌UN沁n (S굔rver}             叫
          b 口M叫加ry model                                                 Flat Memi）싸
    :        回 Ken刈 S叩叩It for ELF blnades        마NFMT ELF     巾     Y y
             口 Kernel supp아tfor MISC 너nafles     마NFMT_MISC    N -   -   N
    i     口 團Defa너I bootload숀r ken咽카9다ments      CMDUNE니BOOL 尸       y Y
                   1rdSal kernel command stnng   CMDIJNE                 console=ttyS0 root=Idevfiam0 IW       r;
                            n                          m   7




                                                                                                           i효
                                                                                         小   如         小   1m




    「     P念攝）tIn option도
                                                                                                           1甘

    I 그림 16-2 커널 커맨드 라인 기본 값 설정


    ［그림 16-2］와 같이 "부트로더 커널 인자 기본 값 사용（Default bootloader kernel
    arguments)"이라는 옵션을 활성화하고 "초기 커널 커맨드 문자열(Initial kernel command
    string)" 항목을 보이는 대로 편집한다. 그렇게 하면 .config 파일에 리스트 ［리스트
    16-이과 같은 구성 옵션이 추가되는 것을 알 수 있다．

    ［리스트 ]6-6] 커널 커맨드 라인 기본 값 관련 구성 옵션



            C0N FIGeCMDLINE B00L=y
            C0NFELCMDLINE="console=ttyS0 root=/dev/ ramO rw "
                                                                   리눅스 포팅   Chapter 16




      ［리스트 好6］에서 볼 수 있는 생략 기호는 이 내용이 . config 파일의 일부만 표시했음을
       나타내는 것이다. 이 커널 빌드 시스템에서 이 구성 옵션을 처리하면 ［리스트 儉7］에서 볼
       수 있는 것과 같이 . . . /include/linux/au七oconf . h 파일의 항목으로 표현된다．

      （리스트 167] 커널 커맨드 라인 기본 값을 위한 autoconf.h 항목



           #define CONFIG_CMDLTNE_BOOL 1
           #defThe CONFIGCMDLINE "console=ttysO root=/dev/ ramO rw"




       이제 ［리스트 16旬를 다시 보면 다음 코드가 있는 것을 볼 수 있다．

          strlcpy (cmd_line, CONFIG_CMDLINE, sizeof (cmd_line));


       이 커널 기반의 문자열 복사 함수는 CONFIG C卜'IDLINE어］ 정의된 문자열을 커널 전역 변수
       인 cmdHline어］ 복사한다. 이 문자열은 아주 중요한 역할을 하는데 , 많은 함수와 디바이스
       드라이버가 부팅의 초기 시점에 커널 커맨드 라인을 검사해야 하기 때문이다. 전역 변수인
       cmd line은 .data 섹션의 시작 부분에 숨겨져 있는테 , 어셈블러 파일인 . . . /arch/
      ppc/kernel/head. S어］ 정의되어 있다．

      미묘한 부분을 하나 짚고 넘어가야 하겠다. ［리스트 16-4］를 다시 보면 어셈블리 코드가
      MMtJHinit을 호출하기 전에 machine mnl七이 먼저 호출되는 것을 알 수 있다. 이는
      machine mnl七 함수 내에서 실행되는 코드는 제한된 메모리만 접근해도 동작하는 데 문제
      가 없다는 것을 의미한다. MMU를 가지고 있는 최신 프로세서의 상당수가 프로세서의 하드
       웨어 레지스터를 이용해서 최소한의 초기화를 하지 않으면 메모리를 전혀 접근할 수 없다3).
      일반적으로 부팅 시에 커널과 램디스크 이미지를 로드하고 압축 해제할 수 있는 공간을 위해
      서 작은 양의 메모리를 사용 가능하도록 설정해 둔다. 하지만 이 영역을 넘어서서 코드나 데
      이터를 접근하면 에러가 발생할 것이다. 각 아키텍처와 플랫폼마다 초기에 접근 가능한 메모
      리 크기는 다를 수 있지만 보통 8-16MB 정도가 적당하다. machine mnl七 함수와 플랫폼
       초기화 코드는 바로 이 초기 메모리 문맥에서 실행된다는 것을 반드시 기억해 두도록 하자．
      만약에 새롭게 포팅한 커널을 디버깅하는 중에 데이터 접근 에러를 만나면（PowerPC의


3) AMCC PPC405가 가장 좋은 예다. 관심 있는 독자는 이 프로세서의 BAT 레지스터를 알아보기 바랸다．


                                                                                 523
          Embedded Linux Primer




        DSI 예외4) ) 독자가 작성한 코드가 매핑되지 않은 메모리 영역을 접근하려고 하는 것은 아
        닌지 의심해 보아야 한다．



16.3 플랫폼 초기화
        이제부터 이른 초기화 과정에서 코드의 흐름을 간단히 살펴보도록 하자. ［그림 16-3］을 보
        면 부트로더 또는 부E入E랩 로더에서 플랫폼 초기화 코드로의 흐름을 볼 수 있다．

        부트로더에서
         入，\
              head.S machineinit()
                                     setup.c rIatform_init()


                                                               照多多
             口／
        I 그림 ]6-3 플랫폼 초기화로의 코드 흐름


        head. S와 setup . C 파일은 모두 PowerPC 아키텍처의 . . . /arch/ppc/kernel 디렉터
        리에서 찾을 수 있다. 사용하는 자체 플랫폼을 위한 초기화 파일은 . . . /arch/ppc/
        pla七forms 디렉터리에 위치시켜야 한다. ［그림 16-3］에서는 이 부분이 mypla七．C이다．
        이제 플랫폼을 위한 초기화 파일에 대해서 자세히 알아보도록 하자．

        ［리스트 16尸3］에서 플랫폼 초기화 파일인 ii七e5200. c어］ 있는 함수를 이미 살펴봤다．
        platform mni七 (）을 제외한 모든 함수가 static으로 선언되어 있다. 그렇기 때문에 ［그림
        16-3］에서 보는 것처럼 platform init () 함수가 플랫폼 초기화 파일의 진입점이 될 것
        이고, 이 파일의 나머지 함수는 이 파일 내부에서만 참조된다．

        진입 함수인 pla七form init (）을 살펴보도록 하자. ［리스트 16-8］에 11te5200. c의
        platform init () 함수의 내용을 다시 나타냈다．




El) 이 장의 마지막에 있는 참고 자료에서 프로그래밍 환경 매뉴얼을 보면 Powerl兀의 DSI 예외에 대해서 자세히 알 수 있다．


  524
                                                             리눅스 포팅   Chapter 16



［리스트 ]6-8) L什e5200의 히atform mnit 함수

   void _init
   platform_init (unsigned long r3, unsigned long r4,
                unsigned long rS, unsigned long r6,
                unsigned long r7)
   {
       /山' Generic MPC52xx platform initialization 央/
       /女 TODO create one and move a max of stuff in it.
           Put this mnit in the syslib 女 /

       struct bi_record *bootinfo = find_bootinfoQ;

       i f (booti nfo)
            parse_bootinfo(bootinfo) ;
       else {
            /卉 Load the bd_t board info structure 央 /
       if (r3)
            memcpy((void*)&_res, (void소) (r3+KERNELBASE) ,
                    引 zeof伯d_t力 ’，

   #i fdef coNFIG_BLK_DEv_INITRD
       ／央 Load the initrd 女／
           if (r4) {
               initrd_start = r4 + KERNELBASE;
               initrd_end = r5 + KERNELBASE;
            }
   #endif

       /士 Load the command line *7
       if (r6) {
               央（char 女乂r7+KERNELBASE) = 0;
               strcpy (cmd_line, (char *)(r6+KERNELBASE));
            }
       }
       /女 PPC Sys identification */
       i denti fy_ppc_sys_by_id(mfspr (SPRN_svR));

        /"" BAT setup 央/
       mpc52xx_set_batO;




                                                                            525 1
   蘿i1   Embedded Linux Primer



              /中' NO ISA bus by default */
              isa_io_base         = 0;
              isa_mem_base        = 0;

              /""" Powersave /
              7* This is provided as an example on how to do it. But you
                   need to be aware that NAP disable bus snoop and that may
                   be required for some devices to work properly, like USB
                    .   六／
              /十' powersave_nap = 1; *7

              /"'" Setup the ppc_md struct 六 /
              ppc_md. setup_arch = lite5200_setup_arch;
              ppc卞md. show_cpuinfo = lite5200_show_cpuinfo;
              ppc_md. show_percpuinfo    = NULL;
              야）c_md. in卄_IRQ            = 뺘）c52xx_init_i rq;
              야）c_md. get_卄q             = 뺘）c52xx月吐_irq;

         州fdef CONFIG寸PCI
            ppc_md . pci_map_i rq = ii te5200_map_i rq;
         #endif

              야兀_md. find_e써工f_爬mory = 뺘）c52xx_fi nd_end_of_memo四；
              야）c尸md. setu口化_mappings = 뺘）c52xx山叩iO;

              ppc_md. restart       = mpc52xx_restart;
              야）c_md . pow아工ff      = 뺘）c52xx中애卽工ff;
              ppc_md . halt         = 뺘）c52xx小alt;

                /'"" No time keeper on the LITE5200 士 /
              마）c_md . time_in卄      = NULL;
              야）c놔以Lget_八c_ti me = NULL;
              ppc_md. set_rtc_time = NULL;

              ppc_md. calibrate_decr   = mpc52xx_calibrate_decr;
         #i fdef CONFIG_SERIAL_TEXT_DEBUG

            ppc_md. progress              = mpc52xx_progress;
         #end if
         }




I 526
                                                리눅스 포팅   Chapter 16



       이 함수는 해당 플랫폼을 위해서 필요한 여러 가치 내용을 구현하고 있다. 먼저 부트로더가
       넘겨준 보드 전용의 데이터를 검색하는 것으로 시작한다. 자세한 설명은 16.3.2절 "보드의
       정보 구조"로 미루기로 하자．

       이 검색 작업 후에는 커널이 초기 램디스크5) (initrd）를 이용하도록 구성된 경우에만 램디
       스크 이미지의 시작과 끝 주소를 저장해 둔다. 이 값들이 관례에 따라 PowerPC의 범용 레
       지스터인 r4와 r5로 전달되는 것을 주의하자. 이들 레지스터를 통해서 initrd의 주소를
       전달해 주는 일은 부트로더의 몫이다. 나중에 커널이 이 주소를 이용해서 initrd 이미지를
      （부트로더가 복사해 놓았거나, 플래시 이미지 상에 있는） 원본 메모리에서 읽어서 내부 커널
       램디스크 구조로 로드할 것이다．

       다음으로 커널 커맨드 라인을 저장하는 코드를 볼 수 있는데 , platform mnl七 () 함수로
       이들 주소값이 전달될 때는 각각 시작과 끝을 가리키는 주소로 r6와 r7 레지스터가 이용된
       다. 이 부분은 이전에 커널 커맨드 라인을 정적으로 저장하는 방법과는 다른데 커널 커맨드
       라인을 커널에 포함시켜서 빌드하는 경우와는 반대로 부트로더가 pla七form init () 함수
       로 전달하1 주기 때문이다．

       initrd와 커널 커맨드 라인을 복사하는 것은 아주 쉽게 이해할 수 있다. 기본적으로 부트로
       더에서 전달되는 레지스터들은 이들 데이터가 저장된 메모리 주소를 담고 있다. 하지만 미묘
       한 부분이 하나 있다. 독자도 아마 KERNELBASE 상수가 어디에 사용되는지 궁금할 것이다．
       이 상수를 이해하는 것이 복잡해 보이는 부트 과정을 이해하는 데 핵심이 된다．

       부트로더가 전딜해 주는 주소 값은 모두 물리 주소（physic졔 ad小ess）이다. 이는 데이터가 존재
       하는 실제 칩의 하드웨어 주소를 의미한다. 부트로더는 일반척으로 가상 메모리 기능을 사용
       하지 않고 실행된다. 하지만 커널은 사용자가 설정할 수 있는 잘 알려진 기본 주소에 정적으
       로 링크된다. 이 주소가 바로 KERNELBASE이다（이 값 자체는 크게 중요하지 않다. 이 주소
       값은 사용자가 변경할 수 있지만 일반적으로 기본 값인 OxC0000000을 바꾸치 않고 그대로
       사용한다）.

       이 부분 때문에 head . S가 재미있는 상황에 놓인다. 커널의 압축이 해제되고 메모리에 재배
       치되고 나면（보통은 0번지에） 모든 코드와 데이터 심볼이 커널의 가상 메모리 주소인
       KERNELBASE에서 링크된다. 이는 커널 빌드 과정에서 생성되는 커널 심볼 맵 파일인

5) 초기 램디스크 또는 initrd어］ 대해서는 6장에서 설명하고 있다．


                                                               527 1
 難 N.      Embedded Linux Primer




        System.map6）을 보면 알 수 있다. 하지만 MMU가 활성화되기 전에는 이 주소가 가상 주
        소가 아닌 실제 하드웨어 주소가 된다. 이는 MMII를 활성화하고 가상 메모리 매핑을 초기화
        하기 전까지는 모든 코드가 재배치 가능7）해야 하고 심볼에 접근하더라도 변환（fixed up）을 거
        쳐야 한디는 의미가 된다. 그러기 위해서 심볼을 접근하기 전에 그 주소 값에 오프셋을 더해
        야 한다. 예제를 하나 보면 명확하게 이해가 될 것이다．


16.3. ] 초기 변수 접근

        부팅 과정의 아주 이른 시점에 , 즉 코드 세그먼트에 있는 코드가 아직 물리 주소로 1:1 매핑
        되어 있는 상황에서 실행될 때 cmdlmne이라는 변수를 접근해야 한다고 가정해 보자. 전에
        도 언급했지만 이 변수는 head. S어］ 정의되어 있고 커널이 링크될 때 .data 섹션에 위치하
        게 된다. 리눅스 커널의 System .map 파일을 보면 이 cmd1line이 어느 주소에 링크되는지
        찾을 수 있다．



            $ cat system.map I grep cmd_line
               c0115000 D cmd_line




        만일 실제 주소 = 물리 주소인（MMU가 비활성화된） 모드에서 실행되고 있고, 이 변수를
        심볼로 직접 접근하게 되면 3GB (OxC0000000）보다 큰 메모리 주소에 읽고 쓰려고 하게
        될 것이다. 대부분의 소규모 임베디드 시스템은 그렇게 큰 램을 가지고 있지 않기 때문에 임
        의의 값을 읽거나, 시스템 충돌이 발생하게 될 것이다. 또한 실제로 그 주소에 물리 메모리가
        존재하더라도 이렇게 부팅 과정의 초기 시점에는 그 영역이 매핑되어 사용할 수 있도록 되어
        있지는 않을 것이다. 그렇기 때문에 이 변수에 접근하기 위해서는 주소를 수정해야 한다.

        ［리스트 16-9］는 head. S에서 이 내용에 해당하는 코드를 나타낸 것이다．

        ［리스트 16-9) 변수 참조 수청하71


            relocate_kernel :
                 adchs r9, r26, klimit@ha ／六 klimit을 가져옴 六／/

6) System. map 파일은 4장어1,1 설명했다．
7) ［역자주） 재배치가 가능햐다는 의미는, 그 어떤 코드를 메모리의 어느 위치에 두더라도 문제없이 실행된다는 의미이다． 그러71
   위해서는 절대 주소를 사용하지 않는 등 주의할 점이 있다．


1528
                                                               리눅스 포팅   Chapter 16



                lwz   r25, klimit@1 (r9)
                addis r25, r25 , -KERNELBASE@h




       Powerl兀의 head. S 파일에 있는 이 코드 부분이 지금 설명하고 있는 문제의 좋은 예라고
       할 수 있다. klimit이라는 변수는 커널 이미지의 끝을 가리키는데 다른 파일에서 char火
       klimit으로 정의되어 있다. 그래서 이 값은 주소 값을 담고 있는 포인터 값이다. ［리스트
       16-아를 보면 klimit의 주소를 불러온 후에 , 여기에 미리 계산되어 r26 레지스터로 전달
       된 오프셋을 더한 후에 그 결과 값을 레지스터 r9에 저장한다. 그러면 r9는 이제 상위 16비
       트에 대해서는 klimi七의 수정된 주소를 가지고 있고 하위 비트는 모두 0으로 되어 있는 값
       이 된다.8) 즉, 미리 계산된 후 r26 레지스터로 전달된 오프셋 값으로 주소를 수정한 것이다．

       다음 줄에는 lwz 명령어가 r9 레지스터와 klimi七의 오프셋（klimit 주소의 하위 16비트）
       을 레지스터 r25에 값을 저장하기 위한 유효 주소9）로서 사용한다（klimi七이 포인터임을
       기억하자. 그리고 우리는 kTLimi七이 가리키는 주소에 관심이 있다）. 레지스터 r25는 이제
       klimi七이라는 변수에 저장되어 있는 포인터 값을 갖고 있다. ［리스트 16-이의 마지막 코드
       에서 r25에서 커널 링크 기반 주소인（KERNE出ASE) 값을 빼서 이 레지스터가 실제 물리
       주소를 가리키도록 수정하고 있다. （그 언어로 표현한다면 다음과 같은 일을 하는 것이다．



                unsigned mnt "山 tmp;        /* r25를 가리킴 "'"/
                tnip = + k1imit;
                tnip -= KERNELBASE;




       정리하면 klimit이 가리키고 있는 포인터 값을 읽은 후에 , 그 값을 수정해서 올바른 주소에
       접근할 수 있도록 실제（물리） 주소로 변환한 것이다. 커널이 MMU와 가상 메모리를 활성화
       하면 더 이상 이런 심볼 접근어］ 대해서 걱정하지 않아도 된다. 이는 커널이 실제로 어느 물리
       주소에 있는 것과 상관없이 원래 링크된 올바른 메모리 주소에서 실행되기 때문이다．




8) PowerPC 어셈블러 언어에 대한 자세한 문법은 16. 5. 1. 절 七j 읽어 보기"를 참고하자．
9) （역자주］ 유효 주소（e丘ec山e address）란 기계어에서 메모리에 접근하기 위해서 사용되는 실제 메모己］ 주소를 말하는더1, 禹1 사
  전에 몇 가지 연산을 거친 후어］ 그 결과 값을 주소 값으로 사용할 때, 그 값을 유효 주소라고 말힌다．
  11     Embedded Linux Primer




16.3.2 보드의 정보 구조

       PowerPC 플랫폼에서는 많은 부트로더가 사용되지만 여전히 보드 자체를 위한 데이터 , 즉
       시리얼 포트의 보 레이트（baud rate）이나 메모리 크기 그리고 그 외 부트로더가 사용한 로
       우 레벨 하드웨어 파라미터를 커널에 전달하기 위한 통일된 방법이 없는 상태다. ［리스트
       16-8］에 있는 플랫폼 초키화 파일에서는 두 가지 방법10）을 지원하는데 , bi record라는
       구조체에 저장된 데이터를 이용하는 방법과 bd info라는 구조체에 저장된 데이터를 이용한
       방법이 그것이다． 두 가지 방법 모두 하드웨어 관련 정보를 구조체를 통해서 부트로더에서
       커널로 전달하는 일을 한다.

       다음 코드는 ［리스트 16-8］에서 부트로더가 전달한 하드웨어 구성 정보를 저장하는 부분을
       나타낸 것이다．



          struct bi_record 싸ootinfo = find_bootinfoQ;

               if (bootinfo)
                    parse_booti nfo(booti nfo) ;
               else {
                   ／女 bd_t 보드 정보 구조체를 읽어옴 寸／
               if (r3)
                    memcpy ((void*)&__res, (void*)(r3+KERNELBASE) ,
                           引zeof化d－工刀 ’，




       첫 번째로 bi record 자료 구조라고 표시된 특별한 태그를 검색한다. 만약에 이 태그를
       찾게 된다면 bootinfo라는 포인터 변수에 boo七info 레코드의 시작 주소가 저장될 것이
       다. 여기서부터 이 레코드를 분석해서 하드웨어와 관련된 정보를 얻어낸다. 이는 . . . /
       arch/ppc/kernel/ setup. c를 조사해 보면 볼 수 있다. 현재는 bi records가 커널 커
       맨드 라인과 initrd 이미지의 시작과 끝 주소에 대한 정보, 머신의 종류, 메모리의 크기를
       저장하고 있다. 물론 자신의 필요에 맞게 추가적인 정보를 저장할 수도 있다．




10) 각 방법은 각기 다른 곳에서 기원한 것이다. bd_in如라는 구조체는 UBo아에서 유래한 것이고， bLrecord 구조체는 모든 플랫폼
  어］ 걸쳐 자료 구조를 통합0圄는 시도에서 나온 구조체이다. 두 가지 모두 많은 플랫剖Ha 지원한다．
                                                        리눅스 포팅   Chapter 16



만약에 bi record 데이터를 찾지 못하면 PowerPC 아키텍처는 이 데이터가 U-Boot 보드
정보 구조인 bd info 형태로 저장되어 있을 것이라고 예상하게 된다. 부트로더는 이 자료
구조를 생성하고, 이 자료 구조의 주소 값을 r3 레지스터로 전달하1 줄 것이다. 현재 이 자료
구조가 포함하는 하드웨어 정보들에는 DRAM, 플래시 , SRAM. 프로세서의 클럭 속도. 버
스 주파수, 시리얼 포트 보 레이트 등이 있다．

bi record 자료 구조는 . - . /include/asm-ppc/boo七info.h에서 확인해 볼 수 있고，
bd info 구조체는 . . . /include/asm-ppc/ppcboot .h에서 찾을 수 있다．

하드웨어 설정 또는 커널과 통신하기 위해서 필요한 데이터를 실제로 이용하는 일은 플랫폼
초기화 함수의 몫이다. 예를 들어 , pla七form init () 함수에는 그 이름만으로도 충분히
무슨 일을 하는지 알 수 있는 함수에 대한 포인터를 설정하는 코드가 있다. 다음 코드가 ［리
스트 16-8］에서 이 부분을 다시 나타낸 것이다．

     ppc_md .find_end_of_memory = mpc52xx_fi nd_end_of_memory;

이 mpc52xx find end of memory () 함수를 들여다 보자. 이 함수는                . . . larch!
ppc/ syslib/mpc52xx se七up . c 파일에서 볼 수 있다．



       u32 ramsize = _res.bi_memsize;
       if (ramsize == 0) {
             .    ／士 다른 방법으로 검색 肯／
       }

       return ramsize;



위 코드에서 사용된        res라는 자료 구조는 보드 정보 구조체인데 , 이 구조체의 주소 값은
부트로더가 레지스터 r3를 통해서 전달한 것이다. 보는 바와 같이 , 범용의 셋업 코드에서는
부트로더에서 전달된 잔류 데이터를 저장해 두기만 하고, 실제 사용하는 것은 특정 플랫폼을
위한 코드이다．
   豫U     Embedded Linux Primer




16.3.3 머신 종속적인 호츈
        커널 초기화 또는 커널 동작을 위해서 필요한 공통 루틴의 상당수는 아키텍처와 머신（CPU)
        에 종속적인 것들이다. ［리스트 16-8］에서 platform mnl七（）의 일부를 다시 나타낸 다음
        코드를 보자．




                 " ppc_md 구조체 설정 玄／
               /／山
               ppc_md. setup_arch    = lite5200_setup_arch;
               야兀emd. show_c叫info = ]ite5200_s1山w_cpui nfo;
               ppc_md .show_percpui nfo = NULL;
               ppc_md .ini t_IRQ           = mpc52xx_init_irq;
               마）c_md. get_卄q              = mpc52xx_get_i rq;

          #ifdef CONFIG1PCI
               ppc_md pci_map_i rq       = ii te5200_map_i rq;
          #endif

                 ppc_md. find_end_of_memory   = mpc52xx_fi nd_end_of_memory;
                 야）c_md. setup_io－口mappings   = 뺘）c52xx_m叩_i 0;

                 ppc_md. restart     = mpc52xx_restart;
                 ppc_md. power_off   = mpc52xx_power_off;
                 ppc_md. halt        = mpc52xx_halt;




        이와 비슷한 코드가platform init () 함수의 마지막 부분까지 이어진다. 이 특정 플랫폼
        만을 위한 함수들은 모두 리눅스 커널과 통신하기 위해서 필요한 것이다. machdep calls
        형식의 전역 변수인 ppc md는 PowerPC 플랫폼을 위해서 리눅스 커널을 쉽게 커스터마이
        징할 수 있도록 후킹 구조를 제공한다. 이 변수는 . . . /arch/ppc/kernel/ setup. c어］ 선
        언되어 있다. PowerPC 커널 포팅 코드의 여러 곳에서 이 구조체를 통해서 간접적으로 함수
        를 호출한다. 예를 들어 , ［리스트 16-10］은 . . . /arch/ppc/kernel/ setup. c에서 시스
        템 재시작, 종료, 중지 함수 부분을 나타낸 것이다．




1 532
                                             리눅스 포팅   Chapter 16



［리스트 ]6寸10] 범용 Po叫erPC 머신 합수듈

   void machine_restart (char *cmd)
   {
   #i fdef CON FIG-mNVRAM
            nvram_ syncQ;
   #endif
            ppc_md. restart (cmd) ;
   }

   void machi ne_power_off (voi d)
   {
  #i fdef CONFIG_NVRAM
         nvram_ sync() ;
  #endif
         ppc_md. power_offo;
  }

  void machine_halt (void)
  {
  #1 fdef CONFIG_NVRAM
         nvram_sync () ;
  #endif
         ppc_md. haltO;
  }


이 함수들은 ppc md 구조체에 자장되어 있는 함수 포인터가 가리키는 함수를 호출하는데，
이 구조체에는 머신을 위한 함수 또는 플랫폼을 위한 함수의 포인터를 저장하고 있다. 이들
함수 중의 일부는 머신（Cpu）을 위한 코드이며 , mpc52xx 계열 함수가 여기에 해당하는 것
을 알 수 있다. 그 예로 mpc52xx res七ar七와 mpc52xx map io를 들 수 있다. 다른 것들
은 하드웨어 플랫폼을 위한 것들인데 , 여기에는 ii七e5200 map irq와 1ite5200
se七up arch 등이 포함된다．




                                                          533   I
         Embedded Linux Primer




16.4 한데 묶'I
        이제 어디서부터 시작할지 참고할 수 있는 코드를 갖고 있기 때문에, 예제로 사용하는 자체
        보드를 위한 파일과 함수를 만들 수 있다. Lite5200 플랫폼 파일을 복사해서 기반으로 삼도
        록 하고, 우리 보드를 위해서 이 파일을 수정하도록 하자. 그리고 이 새로운 플랫폼을
        PowerDNA라고 부르기로 하자. 이 보드를 위한 포팅은 다음 단계를 통해서 진행할 것이다．

          1. . - . arch/ppc/Kconfig 파일에 새로운 커널 구성 옵션을 추가한다．

          2. 기반으로 삼을 1ite5200．女 파일을 I兀werdna. *라는 이름으로 복사한다．

          3. 새로운 poi寸erdna．士 파일을 플랫폼에 맞도록 수정한다．

                           卜4ake file을 편집해써 조건에 따라서 poi氾rdna .O를 빌드하도록
          4. .. . /arch/ppc／
             한다．
          5, 컴파일 및 로드해써 디버깅한다！


        KConfig에 커널 구성 옵션을 추가하는 것은 4장에서 배웠다. PowerDNA 포팅을 위해서
        새로 추가할 구성 옵션은 ［리스트 16小11]에서 볼 수 있다．

        ［리스트 ]6-11) PowerDNA를 위한 구성 옵션


          config POWERDNA
                  boo] "united Electronics industries PowerDNA "
                  select PPC_MPC52xx
                  help
                    support for the UEI P0WerDNA board




        이 Kconfig 항목은 LITE5200 항목11) j斗 관계가 있기 때문에 바로 아래에 추가하자. ［그
        림 16-4］는 구성 유틸리티를 실행했을 때 새로운 항목이 추가된 결과를 보여 준다．




11) 공간을 절약하기 위해서 ［그림 儉4）에서 LITE5200 이젼에 나오는 여러 힝목은 생己垓虹｝.


  534
                                                                                     리눅스 포팅       Chapter 16



    Eule   Qpiions 匕叫 p

      匈 ［二 日              1      II     는     m     骨
     出,ck Load Save Si四le Sptit F너1 乙꺾apse Expand

    匣쯔으P5                                               1                        ] 1 ! J'匡
    I. Processor                                                                             r的
    口 F거atfoin（料ions
       V 口 MacNneTy口e
            O CHRP/PowerMa다PReP                             PPC_MUIJIPLATFORM N              小
            OADS8272                                        A1J58272             N
,           O Fre小cale-PQ2FADS                              PQ2FADS              N
:           O Freescale LITE5200 / (IceC毗叫              L1TE5200                 N
            L," United 타ectro짜cv Inductees！가批姓)NA           烈）WER아咀                      V
            C Free5c出e MPC834x SYS                      MPC834x_SYS              N
            C Marvel卜P/64了6傑玗｝                          EV64了60                  N           i;
1i1                      唾轟礪拉管小」
                       1口＋
                                                        나1r            小如   Hm       n
                                                                                         {'1
                                                                                         H




      Vol挺d Ekctroi浪s mnd呻加S 加wert州A POWERC가4A                                               스

      돠뿌p이t卜才曲e 내EI P         t1：片出A bK가iid                                                  -


I 그림 16-4 PowerDNA 윱션이 추가된 화면


여기서 사용자가 POWERDNA를 선택하는 경우에는 다음과 같이 두 가지 동작이 수행된다．

           1. CONFIGPPC,MPC52x>< 구성 옵션이 자동으로 선택된다. 이는 ［리스트 16-11］의
            select 키워드 때문이다．

           2. CONFIGHPOWERDNA 옵션에 대한 정의가 새롭게 추가되고 커널 빌드를 결정하게 된다．


다음 단계로 플랫폼과 가장 가까운 파일을 복사해서 새로운 플랫폼 초기화 파일을 작성하기
위한 기반으로 삼도록 하자. 여기서는 이미 Lite5200 플랫폼을 결정한 상태다. 먼처
1ite5200.c를 powerdna. C로 1ite5200.h를 powerdna . h로 복사한다. 그 다음이 어
려운 부분이다. 하드웨어 명세서나 보드 회로도 그리고 기타 하드웨어 플랫폼 관련 자료를
이용해서 powerdria. 士 파일을 자신의 하드웨어에 맞게 수정해야 한다. 그리고 코드를 컴파
일한 후에 새로운 커널을 직접 부팅시켜서 디버깅해 보도록 하자. 다른 지름길은 없고 경험
을 쌓고 그 경험을 활용하는 것이 가장 좋다. 이 과정이 포팅의 가장 어려운 부분이다. 하지
만 최소한 어디서 시작할지는 알고 있다. 커널 디버깅에 대한 여러 가지 팁과 테콰-I어］ 대해
서는 14장, "커널 디버킹 기술"에서 설명했다．

포팅을 위한 과정을 정리해 보면 ［리스트 16-12］는 PowerDNA 보드에서 리눅스를 실행시
키기 위해 새롭게 추가하고 수정한 파일을 자세히 보여 주고 있다．



                                                                                                       535     a
          Embedded Linux Primer



        ［리스트 ]6-12) PowerDNA률 위해1 새로 추가되고 수정된 커널 파일들

          ii nux-2 .6. 14/arch/ppc/confi gs/powerdna_defconfi g
          ii nux-2 .6. 14/arch/ppc/Kconfi g
          ii nux- 2 .6. 14/arch/ppc/pl atforms/Makefi 1e
          ii nux- 2 .6. 14/arch/ppc/pl atforms/powerdna. c
          ii nux- 2 .6. 14/arch/ppc/pl atforms/powerdna. h
          ii nux- 2 .6. 14/drivers/net/ fec_mpc52xx/ fec. c
          ii nux- 2 .6. 14/drivers/net/ fec_mpc52xx/ fec. h
          11nux- 2 .6. 14/dri vers/net/ fec_mpc52xx/ fec_phy. h
          ii nux-2 .6.14/i nd] ude/asm-ppc/mpc52xx. h



        맨 처음 파일은 기본 구성 파일인데 , 이 기본 구성 파일을 이용하면 커널 구성을 빨리 진행할
        수 있다. 이 구성 파일에 맞게 커널을 설정하려면 다음 명령을 입력하면 된다．

          $ make ARCH=ppc CROSS_COMPILE=<cross-prefix> powerdna_defconfig


        Kconfig 파일을 수정하는 부분에 대해서는 이미 언급했었다. makefile을 수정하는 것도
        아주 간단한데 , 새로운 커널 구성 옵션인 CONFIG POWERDNA를 지원하도록 내용을 추가하
        는 것이 목적이다. 수정하는 내용은 다음 한 줄을 추가하는 것이다．

          obj -$(CONFIG_POWERDNA)       += powerdna. o


        가장 중요한 수정 포인트는 pOi寸erdna. c와 powerdna . h 파일 그리고 FEC（고속 이더넷
        컨트롤러） 계층을 수정하는 부분이다. powerdna. c는 원래 파일인 ii七e5200 . C에서 조금
        만 수정하면 된다. 크게 보면 전체적으로 두 가지 문제를 수정해야 한다. 첫 번째로
        PowerDNA에서는 PCI를 사용하지 않기 때문에 이를 비활성화시켜야 하는데 , 이를 위해 일
        부 수정이 필요하다. 두 번째로는 Pow町DNA 보드에는 다루기 힘든 이더넷 물리 계층 칩을
        내장하고 있는데 , 이를 위해서 하드웨어 설정과 FEC 계층을 일부 수정해야 한다. 이 부분이
        포팅 과정에서 가장 큰 부분인데 이 패치 파일만 1,120줄로 이루어져 있다. 하지만 개발자의
        편의를 위한 기본 값을 설정하는 코드가 대부분이고, 반드시 헤야 하는 것은 아니다. 이 내용
        을 빼면 패치는 411줄로 줄어든다．




I 536
                                                       리눅스 포팅    Chapter 16




16.4. ] 기타 아키텍처
      여기까지 주어진 플랫폼을 어떻게 커널에 맞추는지와 새로운 보드에 포팅하기 위해서 이미
      존재하는 내용을 활용하는 방법을 살펴봤다. 이 장에서 참고하고 설명한 내용은 모두 커널의
      PowerPC 아키텍처 부분만 이용한 것이다. 다른 아키텍처의 경우 다양한 하드웨어 플랫폼
      이 어떻게 통합되는지에 대한 세부적인 사항은 각기 다르지만, 개념은 모두 비슷하다. 그래
      서 하나의 아키텍처를 이해하고 조사하는 방법을 알고 있으면 다른 아키텍처에 대해서도 쉽
      게 접근할 수 있다．



16.5 요약
        口 리눅스가 지원하는 CPU를 이용하는 자체 제작 보드에 리눅스를 포팅하는 것은 상대적으
           로 쉬운 편이다. 이를 위해서는 기반 리눅스 코드와 하드웨어 플랫폼에 대한 이해와 경
           험이 제일 중요하다．

        口 이미 지원하는 하드웨어 플랫폼 구성을 참조해써 작업하는 것이 자신의 보드를 위해서
           포팅할 때1 가장 좋은 방법이다．

        口 초기화 코드의 흐름을 이해하는 것이 포팅을 쉽게 할 수 있는 핵심이다. 커널의 범용적인
           코드 부분은 모두 그대로 두고, 플랫폼 자체를 위해써 필요한 파일만 수정했다. 이를 위
           해서 이 장의 상당 부분을 플랫폼 초기화와 관련 있는 초기 코드의 흐름을 설명하는 데
           할애했다．

        口 디버깅을 진행하기 전에 먼저 로우 레벨 하드웨어 폴랫폼 초기화 코드를 올바로 작성했
           는지 재차 확인해야 한다. 한 예로 디버깅 중에 리눅스의 슬랩 할당자12）佃lab allocator)
           와 관련해서 뭔가 이상한 점을 발견했다면 하드웨어 메모리를 초기화하는 과정에서 뭔가
           실수한 점이 없는지 확인해 보는 것도 좋은 접근 방법이다．

         [a 이 장에서는 주로 리눅스 커널의 PowerP（그 아키텍처어］ 초점을 두고 설명했다. 아키텍처
           하나에 대해서 자세히 배워 두면 나머지 아키텍처도 빨리 접근할 수 있다．




12) （역자주） 슬랩 할당 알고므］즘은 메모리를 관리할 때 메모리의 내부 단편화 현샹울 줄이기 위한 기술이다．


                                                                       537 1
  難U   Embedded Linux Primer




16.5. ] 더 읽0j 보기
       32바트 尸0wer只7 아刃텍처叩서의 프로그래망 환겋 叫누얼（'Programmi끄g 月h月ro끄me끄ts
       Manual for 32-Bit In그pie끄2e끄tations of 比0 尸ower只J Arc力itec亡ure)
       MPCFPE32B/AD 12/2001 REV 2
       프리스케일 반도체社（Freescale Semiconductor, Inc.)


       MPC5200 사용자 가이드
       MPC5200UG Rev 3 01/22005
       프리스케일 반도체社（Freescale Semiconductor, Inc.)
이번 징K게서 배울 내용

  U 리얼 타임

  U 커널 선점

  U 리얼 타임 커널 패치

  U 리얼 타임 커널 디버깅하기

  U 요약
難 SR    Embedded Linux Primer




       리눅스가 처음 인텔 i386 프로세서를 기반으로 만들어졌을 때 , 누구도 리눅스가 서버 어플리
       케이션 용도로 성공하리라고는 예상치 못했다. 하지만 리눅스의 성공으로 인해서 리눅스는
       여러 이기종의 아키텍처에도 포팅되었고 휴대폰에서 원거리 통신 스위치에 이르는 임베디드
       시스템에서도사용되기에 이르렀다. 얼마 전까지만 하더라도 어떤 어플리케이션이 리얼 타임
       으로 실행되어야 한다고 했을 때 대상 운영체제로 리눅스는 그 항목에 포함되지 않았다. 하
    지만 오디오나 멀티미디어 어플리케이션 분야의 주도로 리얼 타임 리눅스의 개발이 이루어짐
       에 따라서 상황이 완전히 바뀌게 되었다．

       이 장에서는 리눅스의 리얼 타임 기능의 역사적인 발전 과정을 간단히 살펴보는 것으로 시작
       한다. 그리고 리얼 타임 개발자를 위한 편의 기능과 활용 방법을 알아보도록 하자．



17. ] 리얼 타임
       다섯 명을 붙잡고 "리얼 타임"이 무슨 뜻이냐고 물어보자. 아마 다섯 명 모두 다른 답을 할
       것이다. 그리고 일부는 숫자를 언급할 수도 있다. 여기서는 논의를 진행하기 위해서 몇 가지
       시나리오를 먼저 생각하1 보고 그 후에 리얼 타임의 청의에 대해서 알아보도록 하자. 리얼 타
       임 중에서도 일부는 소프트 리얼 타임이라고 말할 수 있고, 또 일부는 하드 리얼 타임이라고
       분류할 수 있다．


17.1. ] 소프트 리얼 타임

       일반적으로 소프트 리얼 타임은 특정한 작업이 정해진 데드라인（deadline) 시간을 가치고
       있고, 만약에 그 시간 안에 종료하지 못하면 품질이 떨어질 수 있다는（하지만 치명적이지는
       않다는） 것을 의미한다. 독자가 사용하는 데스크탑 워크스테이션이 이런 소프트 리얼 타임의
       완벽한 예라고 볼 수 있다. 문서를 작성할 때 사용자는 키를 입력한 결과가 곧바로 화면에
       보이기를 기대한다. 또한 좋아하는 .mp3 파일을 재생할 때도 음이 튀거나 끊기는 일 없이
       고음질의 음악을 듣기를 기대하는 것이다．

       일반적으로 사람은 수십 밀리 초 정도의 시간 치연을 감지하지 못한다. 물론 일부 음악가는
       이러한 미묘한 시간 차이에 의해서 음색이 달리 느껴질 수도 있다고 말한다. 만약에 이들 소
       프트 리얼 타임 이벤트가 데드라인을 넘겼다면 결국 사용자는 "질"이 떨어지는 것을 느낄 수
       있겠지만, 그것이 심각한 결과를 초래하는 것은 아니다．
                                           리눅스와 리얼 타임   Chapter 17




17.1.2 하드 리얼 타임
    하드 리얼 타임은 데드라인을 넘겼을 때 어떤 상황에 처하게 되는지로 특징지을 수 있다. 하
    드 리얼 타임 시스템에서는 한 번이라도 데드라인을 넘기면 그 결과가 아주 치명적이다. 물
    론 치명적이라는 말은 지극히 상대적인 용어이긴 하지만 만약에 이 시스템이 제트기 엔진의
    연료 흐름을 제어하는 장치였다면 파일럿의 입력에 대해서 한 번이라도 데드라인 내에 처리
    하지 못할 경우에 그로 인한 오동작 때문에 재앙을 초래할 수도 있을 것이다．

    하지만 데드라인의 지속 시간 자체는 리얼 타임 특성과는 관계가 없다는 점을 주의하자. 원
    자시계에서 매 주키마다 틱을 제공하는 경우가 그 예이다. 한 틱이 다음 틱 이전의 1초 범위
    내에만 처리된다면 데이터는 유효할 것이다. 하지만 틱을 하나 처리하지 못하고 넘길 경우에
    는 아마도 GPS(G1的al Positioning System : 지구 위성 항법 시스템）가 수 미터에서 수
    마일까지 틀려질 수도 있다！

    이런 사항을 염두에 둔다면 소프트와 하드 리얼 타임 시스템의 정의를 몇 가지로 그려 볼
    수 있을 것 같다. 소프트 리얼 타임 시스템은 데드라인을 놓칠 경우에 연산 결과의 질이 떨어
    질 뿐이다. 하지만 하드 리얼 타임 시스템은 한 번이라도 데드라인을 놓치면 그 시스템은 오
    류가 발생했다고 간주되며 , 이로 인해 치명적인 결과를 만들 수 있다．


17.1.3 리눅스의 스케쥰링
    유닉스와 리눅스 모두 프로세스를 스케줄링할 때 공평함을 기본으로 설계되었다. 이 말은 스
    케줄러가 CPU를 사용하려고 하는 모든 프로세스에게 최대한의 가용한 자원을 균등하게 나
    눠줘서 모든 프로세스가 실행을 계속할 수 있도록 만든다는 의미다. 바로 이런 설계 철학이
    리얼 타임 프로세스가 실행되기 위한 환경에는 반대로 작용하게 된다. 리얼 타임 프로세스는
    언제나 실행되어야 할 때 곧바로 실행될 수 있어야 한다. 리얼 타임이라는 말 자체가 예측할
    수 있고, 반복할 수 있는 지연 시간을 갖는다는 것을 의미하기 때문이다．


17.1.4 지연
    리얼 타임 프로세스는 보통 물리적인 이벤트와 연계되는데 , 예를 들어 외부 보조 장치에서
    오는 인터럽트를 들 수 있다. ［그림 17-1]은 리눅스 시스템이 어떤 지연 요소를 가지고 있는
    지 보여 준다. 먼저 지연 시간은 처리하고자 하는 인터럽트를 받는 순간을 시작으로 측정할


                                                              541 1
 蘿1 1      Embedded Linux Primer




        수 있다. 이 시간이 ［그림 17-1)의 to로 표시되어 있다. 얼마간의 시간이 흐른 뒤에 인터럽
        트를 받고, 제어권이 인터럽트 서비스 루틴(TSR）으로 넘어가게 된다. 이 시간은 ti으로 표
        시된다. 이 인터럽트 지연 시간은 거의 대부분이 최대 인터럽트 차단 시간1）이라고 할 수 있
        다. 여기서 인터럽트 차단 시간이란 하드웨어 인터럽트를 비활성화한 상태에서 쓰레드가 실
        행될 수 있는 시간을 말한다．

        인터럽트        인터럽트 서비스                    Is只 신호    리얼 타임 프로세스
        이벤트             루틴 수행          리얼 타임 프로세스               실행




          I I I I
          to               ii                     t2                     t3
                                                                              1느
                                                                              rr
                                                                                    上 1 까．
                                                                                   / \1 니



            "\     V小1/         \H\        1／     人11＼     才m나，     ,/




                 인터럽트                 인터럽트               스케줄링
                  지연                  처리                 지연

             \                                                  I
                                       Y

                 인터럽트에서 프로세스까지의 지연 시간

        I 그림 17너 지연 시간의 구성


        실제 인터럽트 서비스 루틴에서는 최대한 작업을 짧게 하는 게 좋다. 이는 이 루틴이 실행되
        는 문맥에서는 기능이 제한되기 때문인데 , 그래서 보통 TSR에서는 하드웨어적인 처리만 마
        무리하고, 추가적인 데이터 처리 작업은 리눅스의 보텀 하프2)(bottom h帥）3) 또는 softIRQ4)
        라고 부르는 메커니즘을 이용해서 처리한다．

        TSR과 보텀 하프가 실행을 마치면 보통은 그 데이터를 기다리고 있던 사용자 영역 프로세스
        를 깨우게 된다. ［그림 17-1)에서 七2가 이 시간에 해당한다. 이후 어느 시점에 스케줄러가
        리얼 타임 프로세스를 선택해서 실행시키도록 한다. 이 시간을 七3로 표시했다. 스케줄링 지
        연 시간은 주로 얼마나 많은 프로세스가 CPU를 얻기 위해서 기다리는지와 그 프로세스 간


l) 우리는 여기서 문맥젼환에 걸리는 시간은 무시했다. 이 시간은 인터럽트 종료 시간에 비O뻔 무시할 만한 수준이7] 때문이다．
2) （역자주） IRQ가 실행되는 부분을 톱쌍위） 하프（절반）라고 힌다면 나중에 실행 시간을 가질 여유가 있을 때 추가 마두宅］ 쟉업을
   하는 문맥을 보텀（하위） 하프（절반）라고 한다．
                  아e）의 저서인 Linux Kernel Devel叩叱nt에서 보텀 하프어｝ 대한 자세한 설명을 읽을 수 있다． 17. 5. 1절 七｝
3) 로버트 러브（Robert I』
   읽어 토171' 릍 챰고하자．
4) （역자주） S可吐RQ는 하드웨어 인터럽트 요청인 hardlRQ와 비교될 수 있는데, 소프트웨어적인 인터럽트 요청을 의미한다． 디바이
   스 드라이버에서 하드웨어 인터렵트 핸들리 밖에서 추가적인 작업을 계속 진행하고자 할 때 주로 사용된다．
                                                                리눅스와 리얼 타임       Chapter 17



       의 우선순위에 달려 있다. 어떤 프로세스에 리얼 타임 속성을 지정하게 되면 다른 일반 리눅
       스 프로세스보다 더 높은 우선순위를 갖게 되고 그 프로세스가 리얼 타임 프로세스 중에서도
       우선순위가 가장 높으면 다음에 곧바로 실행될 것이다. 즉, 우선순위가 높은 리얼 타임 프로
        세스는 실행될 준비 (10를 위해 대기하는 상태가 아닌 상태）가 되면 언제나 바로 실행된다．
       이 속성을 설청하는 방법은 곧 설명하겠다．



17.2 커널 선점
        초기 리눅스 1.x 시절에는 커널에 선점 기능이 없었다. 이 말은 어떤 사용자 영역 프로세스가
       커널 서비스를 요청하면 이 프로세스가 어떤 응답을 기다리기 위해서（보통은 I/O임） 블록
       되거나（슬립 상태로 감）, 커널 요청이 완료될 때까지 다른 태스크는 Cpu를 사용할 수 없었
       다. 커널을 선점 가능하도록（preemptab1e5) ) 만든다는 것은 어떤 프로세스가 커널 문맥에
        서 실행중일 때 , 비록 이 프로세스가 커널 내부 처리 과정이 끝나치 않았더라도 선점해서 다
        른 프로세스가 실행되게 할 수 있다는 말이다. ［그림 17-2］는 이 내용을 설명하는 그림이다．

        프로세스 A                   프로세스 B      프로세스 A




                                            I
                                                       사용자 영역
                커널 진입점


              시스템 콜을 통히써
                                                         커널 영역


                 프로세스 A가
                         (   I
                                          I프로세스 A가
                   선점됨                      실행 재개
                                                         卜     시간


       I 그림 17-2 커널 선점




5) 흥미롭게도 선점 가능을 의미하는 염에 단어 pre이iptab旭의 철자어］ 대해서 많은 논쟁이 있다． \＼기八v. linuxdevices. com/articles/
  ATh136316996. hti川에서 Rick Leh比aum이 실시한 조사를 참고하도록 하자．
 難 月a     Embedded Linux Primer




        이 그림에서 프로세스 A는 시스템 콜을 통해서 커널에 진입해 있다. 아마도 콘솔이나 파일과
        같은 장치에 write () 하는 호출일 것이다. 프로세스 A가 실행되고 있는 와중에 더 높은 우
        선순위를 갖는 프로세스 B가 인터럽트에 의해서 깨어났다. 이때 커널은 프로세스 A를 선점해
        서 CPU를 프로세스 B에 넘겨준다. 이 작업은 프로세스 A가 블록되어 있지 않고 커널 작업
        이 완료되지 않더라도 일어난다．


17.2. ] 선점의 장애물

        커널을 완전히 선점 가능하도록 만들기 위해서 해결해야 할 어려움은 커널의 모든 영역에 대
        해서 선점되지 말아야 할 보호 영역을 정의하는 일이다. 커널 내부에는 크리티컬 섹션6）이라
        는 영역이 있어서 그 구간에는 선점이 일어나지 못하게 한다. 예를 들어 , ［그림 17-2］의 프
        로세스 A가 커널 영역에서 파일 시스템 동작을 수행하고 있다고 가정해 보자. 하지만 어느
        순간에 코드가 커널 내부에서 파일 시스템의 파일 하나를 나타내는 커널 자료 구조에 값을
        기록하고 있을 수도 있다. 이 자료 구조의 데이터가 망가치는 것을 막키 위해서 이 공유 자료
        구조에 어떤 프로세스도 접근하지 못하도록 반드시 차단해 주어야 한다. ［리스트 17-끄에
        C 문법으로 이 개념을 표현했다.

        ［리스트 17-1] 크리티컬 섹션 차단하기



            preempt_disable() ;

            /""' 크리티컬 섹션 'I
            update_shared_data() ;

            preempt_enable () ;




        만약에 이런 방식으로 공유 데이터를 보호하지 않으면 어떤 프로세스가 이 데이터를 업데이
        트하는 과정 중에 다른 프로세스에 선점되어 버릴 수 있다. 그래서 다른 프로세스가 같은 데
        이터를 업데이트하려고 하면 데이터가 꼬일 수밖에 없다. 이 경우의 전통적인 예제는 두 7가
        의 프로세스가 공통된 변수를 서로 조작하고, 그 값을 통해서 행동을 결정할 때이다. ［그림
        17-3］에 이 경우를 나타냈다．

6) （역자주） 크리티컬 섹션은 해당 코드 부분이 동시에 수행되어서는 안 될 경우 그 영역을 지칭하는 말이다．
                                                           리눅스와 리얼 타임   Chapter 17




     프로세스 A                              黨州스 B

                        프로세스 A가
     count++;           여기서 선점됨

                        프로세스 A가
                        실행을 재개합
     if (count)
     do_something()


    I 그림 ]7-3 공유 데이터의 동시성 오류


    ［그림 17-3］에서 프로세스 A는 공유 데이터를 수정했치만, 아직 그 값으로 다음 행동을 결
    정하지는 않은 상태에서 실행이 중단되었다. 리눅스 설계상 프로세스 A는 자신이 선점 당하
    는 것을 감치할 수가 없다 프로세스 B는 프로세스 A가 재개하기 전에 이 공유 데이터의 값
    을 변경한다. 그러면 보는 바와 같이 프로세스 A가 프로세스 B가 수정한 값을 이용해서 다음
    행동을 결정하게 된다. 이런 오류를 원치 않는다면 프로세스 A에서 공유 데이터를 접근해서
    그 값을 통해서 행동을 결정하는 코드 부분에서는 선점되지 않도록 해 주어야 한다.


17.2.2 선점 모멜
    커널 선점에 대한 첫 번째 해결책은 현재 실행중인 쓰레드를 선점해도 괜찮다고 생각되는 커
    널 코드의 중요한 위치에 확인 코드를 삽입하는 것이다. 이 위치는 시스템 콜어］ 들어가고 나
    오는 부분, 커널 락(lock）을 해제하는 부분, 인터럽트 처리에서 반환하는 부분 등이 포함된
    다. 이들 각 지점에서 선점을 위해서 ［리스트 17-2］와 비슷한 코드가 이용된다．

    ［리스트 ]7寸2] 리눅스 2.4에 선점 패치를 적용한 경우 선점 확인 코드



        ／女
             * This code is executed at strategic locations within
             * the Linux kernel where it is known to be safe to
             * preempt the current thread of execution
             *1
        if (kerneljs_preemptable() && current->need1resched)
          preemptHscheduleO;
 4 難1    Embedded Linux Primer




            1*
                 * This code is in . . ./kernel/ sched. c and is invoked from
                 少those strategic locations as above
                 */
            #ifdef CONFIG_PREEMPT
            asmlinkage void preempt_schedule (void)
            {
                      while (current->need_resched) {
                          ctx_sw_off 0;
                           current->state 1= TASK. 3REEMPTED;
                           schedule0;
                           current->state &= NTASKmPREEMPTED;
                           ctx_sw_on_no_preempt0;
                      }
            }
            #endif




        （실제 코드를 간략화한）［리스트 17-외의 첫 번째 코드 부분은 방금 설명한 선점해도 안전
        하다고 쟁각되는 위치의 중요 포인트에서 수행되는 부분이다. ［리스트 17-쏘에서 두 번째
        부분은 리눅스 커널 2.4에 선점 패치를 적용한 경우에 볼 수 있는 코드이다. 이 무한 루프는
        schedule () 를 계속 호출하게 문맥을 전환시키는데 , 이를 모든 선점 요청이 해결될 때까지
        반복하게 된다．

        비록 이런 접근법이 리눅스 시스템의 지연 시간을 줄일 수는 있지만 완전한 것은 아니다. 낮
        은 지연성을 위해서 개발을 진행하다 보면 이 방법은 결국 사용하기 어렵다는 것을 알게 된
        다. 이전 선점 모델에서는 다음과 같은 문제들이 있다．

         口 리눅스 커널 자체는 기본적으로 비선점형이다．
         口 선점을 검사하는 코드가 커널에서 선점 가능하다고 알려진 위치의 일부 중요 부분에만
                 흩어져 있다．
         口 선점이 커널의 안전하다고 알려진 지점에서만 가능하다．




I 546
                                                          리눅스와 리얼 타임     Chapter 17




       지연성을 획기적으로 줄이기 위해서는 선점형 커널에 다음과 같은 기능이 필요하다．

          口 리눅스 커널 자체가 어디서나 완전히 선점 가능해야 한다．
          口 오직 크리티컬 섹션에서만 선점이 비활성화되어야 한다．

       위 사항은 커널 개발자가 초기 선점형 커널을 위한 패치를 개빌하면서 계속 추구해 온 내용이
       다. 하지만 쉬운 작업은 아닌데 , 전체 커널 코드를 연구하고, 정확히 어떤 데이터가 동시성
       (concurrency）에서 보호되어야 하는지 분석해서 , 그 지점에서만 선점을 막아야 하키 때문
       이다. 이 작업을 위해서 사용된 방법은 커널에서 지연 시간을 측정하도록 만들어서 가장 긴
       지연 시간을 갖는 코드 경로를 찾고, 그것을 해결하는 방식이었다. 그래서 최신 리눅스 2.6
       커널에서는 아주 낮은 지연성을 갖도록 커널을 설정할 수 있는데 , 바로 이런 "커널의 선점
       보호 코드 부분을 일일이 깨부순' 노력의 결과물이다．


17.2.3 SI\川＞7) 커널
       재미있는 것은 멀티프로세서 아키텍처를 위한 작업의 아주 많은 부분이 리얼 타임을 위해서
       도 도움이 된다는 점이다. SMP를 지원하키 위해서는 단일 프로세서만 사용하는 경우보다
       훨씬 더 어려운 점이 많은데 , 보호해야 할 동시성을 더 많이 갖기 때문이다. 단일 프로세서
       모델에서는 어느 한 순간에는 커널 내에서 오직 하나의 태스크만 수행된다. 그래서 동시성에
       대한 보호 장치도 인터럽트나 예외 처리를 위한 부분에만 국한된다. 하치만 SMP 모델에서
       는 인터럽트나 예외 처리 외에도 커널에서 하나 이상의 쓰레드가 같은 시점에 동시에 실행될
       수 있다.

       SMP는 예전 리눅스 2.x 커널에서부터 지원했다. 이때 단일 프로세서에서 SMP로 전환함으
       로써 생키는 동시성에 대해서는 빅 커널 락（BKL: B勾 Kernel Lock）이 사용되었다. BKL은 전역
       적인 스핀락侮pinlock）인데, 커널에서 다른 태스크가 수행되는 것을 막는다. rLinux
       Kernel Dev이opmentj (Novell 출판사, 2005）의 저자인 로버트 러브（Robert Love）는
       BKL을 "커널의 빨강머리 의붓자식"이라고 특징지었다. 그리고 농담 삼아 그 특징을 나열할
       때 "악마'라는 항목도 추가했다．



7) （역자주］ 鈒作는 Symmetric Multi-Processor 구조를 지칭한다. 멀티프로세서 모델 중의 하나이고， 최대 8개의 프로세서까지의 소
   규모 구조에서 많이 人용된다．
            Embedded Linux Primer




         초기 BKL에 기반한 SMP 커널에서는 BKL 때문에 스케줄링 효율성이 상당히 저하되었다．
        즉, CPU 중 하나가 오랜 시간 동안 유휴 상태에 머무는 현상이 발견되었다. 그래서 이러한
         문제에 대해서 효율적으로 SMP 커널을 만들기 위한 노력이 상당 부분 리얼 타임 어플리케
        이션을 지원하는 테도 도움이 되었는데, 특히 처 지연성 측면에 도움이 된다. BKL을 사용하
        는 대신, 실제 공유 데이터가 사용되는 부분 주위에만 작은 락을 설정해 둠으로써 선점 지연
        성을 획기적으로 줄일 수 있게 되었다．


17.2.4 선점 지연의 원인
        리얼 타임 시스템은 지정한 최고 한계 시간 내에 리얼 타임 태스크가 수행될 수 있도록 보장
         해 주어야 한다. 그래서 리얼 타임 시스템에서는 일관적인 낮은 선점 지연 시간을 갖는 것이
        가장 중요하다. 선점 지연 시간에 가장 크게 지장을 줄 수 있는 요인은 두 가지가 있는데，
        각각 인터럽트 문맥 처리와 인터럽트를 비활성화시키는 크리티컬 섹션 구간이 그것이다. 리
        눅스에서 크리티컬 섹션의 크기（또는 유지 시간）를 줄이기 위한 여러 가지 시도에 대해서는
        이미 설명했다. 그리고 이 크리티컬 섹션으로 인해서 인터럽트 문맥 처리 시간이 문제가 될
        수 있는데 , 이는 다음 절에서 설명할 리눅스 2.6 리얼 타임 패치에 그 답이 있다.



17.3 리얼 타임 커널 패치
        하드 리얼 타임을지원하는 코드는 kernel . org에 있는 주류 커널에는 포함되어 있지 않다．
        그래서 하드 리얼 타임을 사용하기 위해서는 별도로 패치를 적용해야 하는데 , 리얼 타임 커
        널 패치는 리눅스 커널 지연성을 줄이기 위한 몇 가지 노력이 축적된 결과이다. 이 패치에는
        여러 사람이 참여했고, 현재는 인고 몰나르（Ingo M아nar）가 관리하고 있고8), http://
        people.redhat.comi- mingo/realtime-preempt에서 찾을 수 있다. 현재 리눅스 커널
        2.6의 소프트 리얼 타임 성능은 최초 2.6 커널이 공개된 후부터 엄청나게 발전해 왔다. 2.6
        커널이 처음 공개되었을 때는 오히려 2.4 커널의 소프트 리얼 타임 성능이 훨씬 더 뛰어났다.
        하지만 리눅스 2.6.12부터는 소프트 리얼 타임 성능이 일반적인 빠른 x86 프로세서에서 수
        밀리 초（한자리수 밀리 초） 정도 내에 가능하게 되었다. 하치만 이보다 더 빠른 반복 가능한
        성능을 위해서는 별도의 리얼 타임 패치가 필요하다．



8) ［역자주） 현재는 F壯p://www. kernel. org/pub/un山c/kernel巾ro 拓／rt/에서 관리되고 있다．
                                                                                    리눅스와 리얼 타임           Chapter 17



리얼 타임 패치는 리눅스 커널에 몇 가지 중요한 키능을 추가해 주는데 , ［그림 17-4］는 리얼
타임 패치를 적용한 후 커널 구성 옵션에 선점 모드에 대한 옵션이 추가된 것을 보여 준다．

    타e    Qptioos    He如

         穹）       ［그        묘          i          H    는
       Pack       Load      Save     Single    Spht    Full   Collapse Expand

    Options                                            Name                ］心呻如tie              「스
    口 F거atforn optir가｝S
         D PC PS/2 st沁 Keyboard                        PCJ(EYBOARD              N   -   N
         口Symmetric 嗣ii下以ess佃9 su叩이S                   SMP                      N   小 N
       , 1 다eempti이i Mat挺                                                               CO01I加rep
           （가的Forced Preempt佃n (Server)                PREEMPT_I幻NE             N   느 N
              0 Volunta싸 Kernel Preemption (Desktop>   PREEMPT_VOLUNTARY N          -   N
              C가가eem的ble Kernel (Low-Latency ［乂sktop) PREEMPT工ESKT아｝            N   小 N
?             回Corn叫ete 마nem的on (Re出干me>               PR든EMI玎_RT                   YY
         回 Thread S야tirqs                              PREEMPT_SOFTIRQS             V V          II
         回 Thread Har如qs                               PREEMPT_HARD(RQS             V V         卜
         回Th爬adRCU                                     PREEMPT_RCU                  V V             童，
         口나gh memo斗5U叩아i                               HIGI-IMEM                N   - N             咎

[1                                 尸          1                           L二                小프
      Fre쩍npllon 斛ode

      닯싸．no help available 幻rth注 이升ion yet.



I 그림 ]7-4 리얼 타임 패치를 적용했을 띠1 추가되는 새로운 선점 모드

리얼 타임 패치는 네 번째 선점 모드인 PREEMPT RT를 추가한다. 여기서 네 가지 선점 모드
는 각각 다음과 같다．

       口 PREEMPT NONE : 비1강제적인 선점. 평균적으로 적당한 지연 시간을 갖지만, 일시적
              으로 긴 지연 시간을 가질 수도 있음. 어플리케이션의 전체적인 성능이 중요할 경우에
              적합함．

       口 PREEMPT VOLUNTARY : 지연 시간을 줄이는 첫 번째 단계. 지연 시간을 줄이기 위해써
              커널의 중요 지점어］ 명시적인 선점 코드를 위치시킴 . 낮은 지연성을 위해써 전체 시스템
              성능에 어느 정도 저하를 가져오게 됨．

       口 PREEMPT DESKTOP : 크리티컬 섹션 내부에서 실행되는 경우를 제외한 모든 경우에
              선점이 가능하도록 함. 이 모드는 오디오나 멀티미디어를 위한 소프트 리얼 타임 어플리
              케이션에 적합함. 추가적인 지연성을 줄이는 데 대한 대가로 전체 시스템 성눙은 떨어질
              수 있음．
         Embedded Linux Primer




         口 FREE卜4PT RT : 리얼 타임 패치로 추가되는 옵션임. 스핀락을 선점 가능한 뮤텍스
          (mute功로 교체함. 이로 인해서 preemp七 disable () 로 따로 보호하는 코드를 제외
          한 커널 내 모든 위치어써 자유롭게 선점이 가능함. 이 모드는 지연 시간을 매우 안정적
            으로 만들어 주기 때문에 시간에 아주 민감한 리얼 타임 어플리케이션을 위한 낮은 지연
            성과 예측 가능한 지연성을 확보해 줌．

        만약 커널 구성에서 커널 선점을 활성화했더라도 부팅 시에 커널 커맨드 파라미터에 다음 파
        라미터를 추가하면 선점을 사용하지 않게 만들 수 있다．

          p reenipt=0



17.3. ] 리얼 타임 기능
        CONFIG PREEMPT RT를 활성화하면 몇 가치 새로운 커널 키능을 선택할 수 있게 된다. ［그
        림 17-4］에서 새로운 구성 옵션을 일부 볼 수 있다. 이 기능과 그 외 리얼 타임 리눅스 패치
        가 제공해 주는 기능에 대해서 알아보도록 하자．


        17.3.1.1 스핀락을 뮤텍스로 바꾸끼
        리얼 타임 패치는 시스템의 거의 대부분의 스핀락을 뮤텍스로 변경한다. 이렇게 함으로써 시
        스템에는 적은 부담을 주면서도, 전체적인 지연 기간을 줄일 수 있게 된다. 스핀락을 뮤텍스
        로 교체하게 되면 기존 스핀락으로 보호되던 부분도 선점 가능하게 된다. 만약 프로세스 A가
        락을 하나 가지고 있을 때 더 높은 우선순위를 가진 프로세스 B가 같은 락을 필요로 하더라
        도, 프로세스 A는 뮤텍스를 가지고 있는한 프로세스 B를 선점할 수 있게 된다.


        17.3.1.2. 커널 태스크로서의 인터럽트 서비스 루틴
        CONFIG PREEMPT HARDIRQ 옵션을 선택하면 인터럽트9) 서비스 루틴(TSR）이 프로세스
        문맥 내에서 실행된다. 이렇게 하면 개발자가 인터럽트 서비스 루틴에 대해서 우선순위를 조
        절할 수 있는데 , 각각이 스케줄링 단위가 되기 때문이다. 그래서 높은 우선순위의 하드웨어
        인터럽트가 발생하면 선점해서 먼저 처리할 수 있게 된다．




9) 또는 HAR五RQ라고도 힌｛가．


  550
                                                          리눅스와 리얼 타임        Chapter 17



       이 기능은 매우 유용하다. 일부 하드웨어 아키텍처에서는 인터럽트 우선순위를 따로 설정하
       지 않는데 , 이렇게 우선순위를 따로 설정하치 않는 것이 독자의 리얼 타임 시스템과 맞아떨
       어지지 않을 수도 있다. 이럴 때 CONFIG PREEMPT HJRDIRQ 옵션을 이용하면 자유롭게
       각각의 IRQ의 우선순위를 정의할 수 있다．

       TSR을 각각의 쓰레드로 동작하도록 하는 기능을 시스템 통작 중에 비활성화시키고자 할 때
       는 /proc 파일 시스템을 통하거나, 부팅 시에 커널 커맨드 라인에 파라미터를 입력해 주면
       된다. 커널 구성 옵션에서 활성화시킨 경우 별다른 옵션을 지정하지 않으면 TSR은 기본적으
       로 쓰레드로서 실행되게 되어 있다．

       시스템 통작중어］ 루트 권한으로 다음 명령을 입력하면 TSR 쓰레딩 기능을 끌 수 있다．

          # echo ' 0t >/proc/ sys/ kernel/hardirq_preemption


        현재 설정을 확인하고 싶으면 다음 명령을 이용할 수 있다．



          # cat /proc/ sys/ kernel/ hardi rq_preemption
          1



       그리고 부팅 시에 ISR 쓰레딩 기능을 비활성화시키려면 커널 커맨드 라인에 다음 파라미터
       를 추가하면 된다．

          hardj rq-preenipt=0



       17.3.1.3 선점 가능한 S아肝毛
       CONFIG PREEMPT小SOFTIRQ 옵션은 SoftIRQ을 커널의 sof七irq 데몬（ksoftirqd）에
       서 실행하도록 함으로써 지연 시간을 줄일 수 있게 해 준다. ksof七irqd는 완전한 리눅스
       태스크（프로세스）이다. 그래서 다른 태스크와 마찬가지로 우선순위와 스케줄링을 공유하게
       된다. 만약 커널이 리얼 타임을 지원하도록 설정되어 있고, 거기에 CONFIG PEE且MPT
       SOFTIRQ 옵션도 활성화되어 있다면 ksoftirqd 커널 태스크는 softirq의 처리10）를 위
       해서 리얼 타임 우선순위를 갖게 된다. ［리스트 17-針은 최신 커널의 . . . /kernel/
       sof七irq.c에서 이 부분에 해당하는 코드를 보여 준다．

10) so栢rq에 대해서 더 알고 싶디면 이 장 뒤편의 챰고 자료에 있는 rj加ux 幽끄el Developa肥n乙를 보도록 하자．
 藿菖1     Embedded Linux Primer



      ［리스트 17-3) ksoftirq를 리얼 타임 상태로 승격시키기

         static -mnt ksoftirqd(void * _bi nd_cpu)
         {
                struct sched_param param = { .sched_priorty = 24 };

                printk ( 'ksoftirqd started up. \n") ;

         #i fdef CONFIG_PREEMPT_SOFTIRQS
                printk ("softirq RT prio: %d. \n", param. sched_priority) ;
                sys_sched_setscheduler (current->pid, SCHED_FIFO, &param) ;
         #el se
                set_user_nice(current, -10) ;
         #end卄




       여기서 CONFIG PREEMPT SOFTIRQS7} 활성화되어 있으면 어떻게 되는지 볼 수 있다. 즉，
       ksof七irqd 커널 태스크가 리얼 타임 태스크로 승격되고, sys sched setscheduler ()
       커널 함수를 이용해서 리얼 타임 우선순위를 24로 설정했다．


       SoftIRQ 쓰레딩 기능 역시 실행중에 /proc 파일 시스템을 통해서 비활성화시킬 수 있고，
       또한 부팅 중에는 커널 커맨드 라인 옵션을 통해서도 비활성화시킬 수 있다. 커널 구성 옵션
       에서 활성화시키면 기본적으로 SoftIRQ 쓰레딩이 활성화된다. 실행중에 SoftIRQ 쓰레딩
       기능을 끄기 위해서는 루트 권한으로 다음 명령을 내리면 된다．

         # echo ' 0, >/proc/sys/kernel/ softirq_preemption

       그리고 설정 값을 확인하려면 다음과 같은 명령을 이용한다．



         # cat /proc/sys/kernel/ softi rq_preemption
         1




552
                                                               리눅스와 리얼 타임   Chapter 17



        그리고 부팅 시에 SoftIRQ 쓰레딩을 끄려면 다음 파라미터를 커널 커맨드 라인에 추가해
        주면 된다．

            softi rq- preempt=0



        ]7.3.1.4 RCU 선점
        RCU")（읽기4복사하기m갱신하기）는 리눅스 커널에서 주로 읽기 연산만 자주 이루어지고，
        내용이 갱신되는 일은 가끔 일어나는 데이터를 위해서 설계된 특수한 동기화 메커니즘12）이
        다. RCU를 하나의 최적화된 읽기용 락（Lock）이라고 생각할 수도 있다. 리얼 타임 패치는
        CONFIG PREEMPT RCU 옵션을 추가하는데 , 이 옵션은 RCU 섹션을 선점 가능하게 만들어
        줌으로써 지연 시간을 줄일 수 있다．


17.3.2 0口） 스케줄러
        0(1) 스케줄러는 리눅스 2.5 시절부터 존재했다. 여기서 별도로 언급하는 이유는 리얼 타임
        을 위해서 중요한 요소이기 때문이다. 0(1) 스케줄러는 기존 리눅스 스케줄러에서 엄청나게
        발전한 것이다. 여러 개의 프로세서를 가지고 있는 시스템에도 쉽게 적용할 수 있고, 시스템
        이 전체적으로 낮은 지연성을 갖도록 돕는다．

        모르는 독자를 위해서 설명하면 O(1）은 1번의 연산으로 수행될 수 있는 시스템을 수학적으
        로 표현하는 방법이다. 여기서는 스케줄링을 결정하는 더］ 컬리는 시간이 실행 큐에 있는 프
        로세스의 개수와는 무관함을 의미한다. 예전 리눅스 스케줄러는 이런 특징을 가지고 있지 않
        았기 때문에 프로세서의 개수가 증가하면 스케줄링 성능이 떨어졌었다. 13)


17.3.3 리얹 타임 프로세스 생성하기
        어떤 프로세스를 리얼 타임으로 동작하게 만들기 위해서는 스케줄러가 스케줄링 알고리즘의
        일부로서 참조하는 프로세스의 속성을 설정해야 한다. ［리스트 17-띠에서 일반적인 방법을
        볼 수 있다．


11) RCU에 대한 세부 정보는 www. rdrop. conilusers/j玔뇨ick/RCU／를 참고하자．
12) ［역자주） 즉， RCU도 스핀락이나 뮤텍스와 같이 동기화 기능을 담당하는 동기화 메커니즘히다．
13) 여기서도 로버트 러브(Robert Love）의 책에 있는 O (1) 스케줄러에 대한 뛰어난 글을 참고해 보기 바랸다. 그의 책에서는 O (1)
    표기법을 쓸 수 있는 알고르］즘의 복잡성에 대한 유쾌하지만 통렬한 비판을 볼 수 있다．


                                                                                 553 1
驢U     Embedded Linux Primer



     ［리스트 ]7느4) 리얼 타임 프로세스 생성하71

       #include <sched. h>

       #define MY_RI_F垠IORIIY MAX_USER_RT_PRIO ／必 가능한 최고 우선순위 去／

       mnt main(int argc, char **argv)
       {
              mnt rc, old_scheduler_policy;
              struct sched_param my_params;



              /* 0을 전달하면 호출자의 정책을 의미함 肯／
              old_scheduler_policy = sched_getscheduler (O) ;
              my_params. sched_pri oni ty = MY_RI_PRIORITY;
              fk 0을 전달하면 호출자의 p1 d를 의미함 士／
              rc = sched_setscheduler (O, SCHED. RR, &my_params) ;
              if ( rc == -1 )
                   handle_error () ;

       }


     이 코드는 sched Se七scheduler () 함수 호출을 통해서 두 가지 일을 하고 있다. 먼처 스
     케줄링 정책을 SCHED PR로 설정하고, 자체 우선순위를 시스템이 허용하는 최대로 설정한
     다. 리눅스는 다음과 같은 세 가지의 스케줄링 정책을 지원한다．

       디 SCHED OTHER : 일반 리눅스 프로세스. 공평한 스케줄링

       QSCHED RI之 : 지정된 시간을 할당받는 리얼 타임 프로세스임. 자체적으로 중단되지 않을
           경우는 스케줄러에 의해써 정해찐 특정 기갼 동안은 실행될 수 있다．

       口 SCHED FIFO : 자체적으로 중단되거나, 다른 프로세스로 스스로 CPU를 양보하는 경
           우, 또는 더 높은 우선순위를 갖는 SCHED FIFO 프로세스가 실행 가능하게 될 경우를
           제외하고는 언제나 실행된다．


     맨 페이지의 sched setscheduler 함수 항목을 보면 이 세 가지 스케줄링 정책에 대한
     더 자세한 정보를 참고할 수 있다．
                                                     리눅스와 리얼 타임   Chapter 17




17.3.4 크리티컬 섹션 관리
    디바이스 드라이버와 같은 커널 코드를 작성할 때 , 동시에 여러 프로세스에 의해서 접근하는
    것을 막아야 할 데이터가 생길 수도 있다. 이런 크리티컬한 데이터를 다루기 위한 가장 쉬운
    방법은 크리티컬 섹션 주변에서 선점을 막아 버리는 것이다. 하치만 시스템의 지연 시간을
    최소한으로 유지하기 위해서는 크리티컬 섹션을 최대한 짧게 만들어야 할 것이다. ［리스트
    17司에서 이 예제를 볼 수 있다．

    ［리스트 17-5) 커널 코드에서 크리티컬 섹션을 보호하는 부분



      ／士
           去 중요한 데이터를 위해서 전역 락（global lock）을 선언하고 초기화함．
           女／
      DEFINE_spINLocK (my_lock) ;



       mnt operate..on_critical_data()
      {
                spin_lock (&my_lock) ;

                /* Update critical/ shared data */

                spin_unlock (&my_lock) ;


      }


    태스크가 성공적으로 스핀락을 확보하면 선점이 금지되고, 이 태스크는 크리티컬 섹션으로
    들어갈 수 있게 된다. 그리고 spin unlock이 수행되지 않는한 다른 태스크로 문맥이 전환
    되지 않는다. 사실 spin lock () 함수는 몇 개의 형식을 갖는 매크로인데 , 커널 구성에 따
    라서 내용이 달라진다. 이들은（아키텍처 독립적인 정의를 담고 있는 파일인） . . . /include
    /linux/ spinlock.h의 최상위 레벨에 정의되어 있다. 커널에 리얼 타임 패치를 적용하면
    이들 스핀락이 모두 뮤텍스로 변환되기 때문에 스핀락을 잡고 있는 프로세스가 보다 높은 우
    선순위를 갖는 프로세스에 의해서 선점될 수 있다．
 難月a     Embedded Linux Primer




       리얼 타임 패치는 디바이스 드라이버와 커널 개발자에게도 대부분 투명하게 적용될 수 있기
       때문에 ［리스트 17司에서 설명한 것처럼 크리티컬 섹션을 보호하기 위해서 기존의 익숙한
       방법을 그대로 이용할 수 있다. 이 부분이 리얼 타임 패치의 가장 큰 장점인데 , 기존의 인터
       럽트 서비스 루틴과 보호 메커니즘을 그대로 사용할 수 있기 때문이다．

      ［리스트 17-5］에서 DEFINE SPINLOCK 매크로를 사용한 것은 미래에 생길 수 있는 호환성
       이슈를 위한 것이다. 이 매크로는 . . . /include/linux/ spinlock 七ypes .h어］ 정의되
       어 있다．



17.4 리얼 타임 커널 디버깅하기
      타임 패치가 적용된 커널의 성능을 분석하고 디버깅을 지원하기 위해서 일부 구성 옵션이 지
       원되는데 , 각각에 대해서 이어지는 절에서 하나씩 알아보도록 하자．


17.4. ] 소프트 락업］4) 감지

       소프트 락업을 감지하는 기능을 활성화시키려면 커널 구성 옵션인 CONFIG DETECT
       SOFTL(兀KUP을 켜도록 한다. 이 기능은 커널 모드에서 긴 시간 동안 컨텍스트 스위칭이 일
       어나치 않을 때를 감치할 수 있게 해 준다. 이 기능은 리얼 타임이 아닌 커널에서도 지원하지
       만, 지연 시간이 너무 긴 구간이나, 소프트 데드락（deadlock)15) 상황을 감지하는 데 유용
       하게 사용할 수 있다. 이 기능을 이용하려면 간단히 커널 구성 옵션에서 이 항목을 활성화시
       킨 후에, 콘솔이나 시스템 로그로 출력되는 관련 내용을 참고하면 된다. 보고 내용은 보통
      다음과 비슷한 형식으로 출력된다.

         BUG: soft lockup detected on cPuO


       이 메시지가 커널에서 출력되면 추가적으로 스택 역추적 내용이나, 기타 프로세스 이름과
       PT') 등의 추가적인 정보도 같이 출력된다. 그래서 레치스터 전체 내용이 출력되는 커널 웁
       스 메시지와 비슷해 보인다. 자세한 출력 내용은 . . . /kernel/ sof七lockup. c를 참고하
       도록 하자. 이 정보는 락업이 생기는 지점을 추적할 수 있게 도와준다．

14) ［역자주］ 락업 (lock七功은 실행중어］ 락이 서로 교차해서 걸리거나 해서 교착 상태에 빠지는 것을 말한다. 데드락이라고 생각할
    수 있다．
15) （역자주） 데드락은 두 711 이상의 프로세스가 각각 상대편의 결과를 기다리는 상황을 말하는데, 결국 끝없이 갸：杞］기만 하는
  상황이라고 해서 데드락이라고 부른다．
                                                          리눅스와 리얼 타임   Chapter 17




17.4.2 선점 디버깅
      선점 디버깅을 활성화하려면 커널 구성 옵션에서 CONFIG DEBUG PREEMPT를 설정한다．
      이 디버깅 기능은 안전하치 않은 선점을 하게 될 경우를 감지할 수 있는데 , 선점 횟수의 계수
      가 0보다 작거나, 올바르지 않은 문맥에서 슬립 상태로 들어가려고 할 때 등을 감지해 낼
      수 했다. 이 기능 역시 사용을 위해서는 커널 구성 옵션에서 이 기능을 활성화시킨 후에 , 콘
      솔이나 시스템 로그에 출력되는 보고 내용을 참고하면 된다. 다음은 이 선점 디버깅 기능이
      활성화되었을 때 출력될 수 있는 짧은 예제를 나타낸 것이다.



         BUG: <me> <mypid> , poss卄）le wake_up race on <proc> <pid>
           BUG: lock recursion deadlock detected! <more info>
           BUG: nonzero lock count <n> at exit time?




      이 외에도 더 다양한 내용이 올 수 있는데 , 위 내용은 감치할 수 있는 여러 문저］ 중 일부에
      지나지 않는다. 이들 메시지는 데드락을 피하거나, 기타 에러 상황 또는 리얼 타임 커널 기능
      을 위험하게 사용하도록 프로그래밍되어 있는 코드 등을 잡아낼 수 있도록 도와준다. 각각의
      메시지가 출력되는 상황 및 더 자세한 내용은 리눅스 커널 소스에서 . . . /kernel/
      rt- debug. c 파일의 내용을 참고하도록 하자．


17.4.3 깨어나는 시간佑） 디버킹
      프로세스가 깨어나는 시간을 측정하고, 디버깅하기 위해서는 커널 구성 옵션에서 CONFIG
      WAKEUP TIMING 옵션을 활성화하면 퇸다. 이 디버깅 옵션은 높은 우선순위의 프로세스가
      CPU에 의해서 스케줄되었을 때 실제로 그 프로세스가 실행되도록 깨어나는 데 걸리는 시간
      을 측정할 수 있게 해 준다. 사용법은 아주 간단하다. 이 기능을 사용하도록 커널을 구성하면
      된다. 하지만 커널 구성 옵션에서 활성화되어 있다고 하더라도 기본적으로는 꺼져 있는 상태
      가 되어 있다. 그래서 측정을 위해서는 루트 권한으로 다음 명령을 따로 입력해야 한다．

         # echo 'U, >/proc/ sys/kernel/preempt max_latency




16) ［역자주） 웨이크업 타이밍이라고도 부른다．
難軒難 U    Embedded Linux Primer



        이 /proc 파일을 0으로 설정하면 앞으로 프로세스들이 깨어나는 데 걸리는 시간 중에서 7}
        장 오래 걸리는 시간이 이 파일에 기록된다. 그래서 최댓값을 읽기 위해서는 단순히 다음 명
        령을 입력하면 된다．



          # cat /proc/ sys/ kernel/ preempt_max_latency
          84



        커널 구성 옵션과 proc 파일 설정을 통해서 이 시간 측정 기능을 활성화시켜 두면 최댓값이
        갱신될 때마다 preempt ma乂 la七ency 파일이 업데이트될 것이다. 즉, 비활성화시킬 수
        없다. /proc 변수에 0을 쓰는 것은 단순히 최댓값을 0으로 초기화하고 측정을 재시작하게
        퇸다．


17.4.4 깨어나는 지연 시간 기록
        깨어나는 지연 시간을 기록으로 남기는 키능을 활성화시키기 위해서는 CONFIG WAKEUP
        TIMING 옵션과 함께 CONFIG WAKEUP 교＼TENCY HIST 옵션을 활성화해야 한다. 이 옵션
        은 CONFIG WAKEUP TIMING 옵션으로 측정되는 모든 측정 결과를 나중에 분석할 수 있도
        록 파일에 기록한다. 다음 절에 인터럽트 차단 시간 기록을 검사할 때 이 파일의 내용을 간단
        히 예를 들어 살펴보도록 하자.

          口 CRITICAL PREEMPT TIMING : 선점이 금지된 크리티컬 섹션에서 수행된 시간을 측정

          口 PREEMPT OFF HIST : WAKEUP LATENCY HIST와 비슷하다. 추가적인 분석을 위해1
              서 선점 금지 시간을 측정해써 바이너리 파일에 기록해1 둔다．



17.4.5 인터럽트 차단 시간
        최대 인터럽트 차단 시간을 측정하기 위해서는 커널 구성 옵션에서 CRITICAL IRQSOFF
        TIMING를 활성화시킨다. 이 옵션은 인터럽트 요청 (IRQ）이 꺼져 있는 크리티컬 섹션에서
        소요된 시간을 측정해 준다. 이 기능은 깨어나는 지연 시간을 측정하는 것과 같은 원리로 동
        작한다. 측정을 시작하려면 루트 권한으로 다음을 수행한다．

           # echo 'O ' >/proc/ sys/ kernel/preempt_max_latency


  558
                                                      리눅스와 리얼 타임   Chapter 17




    이 /proc 파일에 0을 기록하면 이 이후부터의 최대 인터럽트 차단 시간이 이 파일에 기록된
    다. 이 최댓값을 읽어 보려면 다음과 같이 파일 내용을 출력해 보면 된다．



      # cat /proc/ sys/ kernel/ preempt_max_latency
      97




    지연 시간에 대한 두 가치 측정치 모두, 즉 깨어남 지연 시간과 인터럽트 차단 지연 시간 모
    두가 같은 /proc 파일을 통해서 활성화되고 확인할 수 있다는 것을 알 수 있다. 이 말은
    한 번에 오직 하나의 옵션만 활성화시켜야 하고, 그렇지 않으면 결과가 틀릴 수도 있다는 말
    이다. 또한 이러한 시스템 단위의 시간 측정을 하면 엄청난 동작 오버헤드가 발생하기 때문
    에 , 모든 측정 옵션을 다 활성화시키는 것은 그다지 현명한 생각은 아니다．


17.4.6 인터럽트 차단 시간 기록
    INTERRUPT OFF HIST 옵션을 활성화하면 WNKEUP LATENCY HIST를 활성화한 것과 비
    슷한 기능을 사용할 수 있다. 이 옵션은 인터럽트 차단 시간을 측정해서 추가적인 분석을 위
    해서 파일에 기록해 둔다. 이 데이터는 히스토그램 형식으로 되어 있는데 , 각 항목이 0마이
    크로초에서 10,000마이크로초까지의 범위를 갖는다. 주어진 예제에서는 최대 지연 시간이
    97마이크로초라고 되어 있다. 그래서 히스토그램에 있는 치연 시간 데이터에는 97마이크로
    초를 넘는 유용한 정보는 없다는 결론을 내릴 수 있다．

    기록된 시간 데이터는 특별한 /proc 파일을 통해서 읽을 수 있다. 그리고 다음과 같이 이
    파일의 내용을 일반 파일로 리다이렉트시켜서 값을 분석하거나 그림을 그려 볼 수 있다．



      # cat /proc/1atency_hist/ interrupt_off_1atency/ cPuO > hist_data. txt




    ［리스트 17-6］은 이 기록 데이터에서 처음 10줄을 나타낸 것이다．
羅m      Embedded Linux Primer



      ［리스트 ]7-6) 인터럽트 차단 지연 시간 기록（앞부분）

        S cat /proc/latency_hist/interrupt_off_latency/cPU0 I head
        #Mininiutn latency: 0 microseconds.
        #Average latency: 1 microseconds.
        #Maximum latency: 97 microseconds.
        #Total samples: 60097595
        #ihere are 0 samples greater or equal than 10240 microseconds
        #usecs            samples
             0
                        13475417
             4上
                        38914907

             m/L 入
                 4J
                         2714349
                          442308




      ［리스트 17-6］에서 최솟값과 최댓값을 볼 수 있고, 전체 값의 평균값과 전체 샘플의 수도
      확인할 수 있다. 이 경우 우리는 6천만 개가 조금 넘는 샘플을 수집한 것을 알 수 있다. 그리
      고 히스토그램 데이터에 대한 요약 정보, 즉 1만 개 정도의 눈금으로 샘플을 분류할 수 있다
      는 것을 볼 수 있다. 이 데이터를 이용해 ［그림 17-5］와 같이 gnuplot을 통해서 쉽게 그림
      으로 그려 볼 수도 있다．

                                                                      인터럽트 차단 시간
      샘플 수
       le+08
                                                                                                                  1 "hist dta.txt"
       le+07
       le+06
      100000              11


                                            1          1=


       10000
                                        1       11 1
                               11
                                    1


                                                            1         1b


        1000
                                                                111        1
                                                                               1
                                                                                                      ' 竹
                                                                                   '尸
                                                                                        '· ．...．尸．戶         ".   -.   ·．m.   .


         100                                                                                                                     11111111t1




           10
            1
                      0                         20                             40                                60                       80   100
                                                                                        마이크로 초
      I 그림 ]7-5 인터럽트 차단 지연 시간 데이터



560
                                                             리눅스와 리얼 타임      Chapter 17




17.4.7 지연 시간 추적
    커널 구성 옵션에서 LATENCY TRACE는 마지막 최대 지연 시간이 걸린 구간에 대한 커널
    추척 데이터를 생성할 수 있게 해 준다. 이 옵션도 /proc 파일 시스템을 통해서 활성화시켜
    야 한다. 이 지연 추적 데이터는 가장 오랜 치연 시간을 갖는 코드 경로만을 분리시키는 더］
    도움이 된다. 매번 최대 지연 시간이 갱신될 때마다, 관계된 추적 데이터가 생성되는데 이를
    이용해서 최대 지연 시간을 갖는 코드 경로를 추적할 수 있다．

    ［리스트 17-7］에는 최대 78마이크로초가 걸린 예제에 대한 추적 데이터를 다시 나타낸 것이
    다. 지금까지 설명한 다른 측정 툴과 마찬가지로 加roc/ sys /kernel/preemp七 max
    latency어］ 0을 쓰면 측정이 시작될 것이다．

    ［리스트 ]7-7] 최대 인터럽트 차단 시간 추적


      $ cat /proc/latency_trace
      preemption latency trace vl. 1. 5 on 2. 6.14-rt- intoff- tim_trace

       latency: 78 us, #50/ 50, CPu#0 j (M: rt VP: 0, KP: 0, SP:1 HP: l)

          I task: softirq- timer/0- 3 (uid:O nice:0 policy:1 rt_prio:l)




                      -      => cPu#
                     / H     => 卄qs-off
                    I / -Uem4-> need- resched
                    II / H   => hardi rq/ softi rq
                    III /    => preempt-depth
                    liii /
                    11111        delay
       cmd      pid 1 I I i I time I     caller
          \   /     IHH         \ I    /
         cat-6637    0D. . .    lus : common_interrupt ( (0))
         cat-6637    0D. h.     2us : do_IRQ(c013d91c 0 0)
         cat-6637    0D. hl     3us+: ma訊코nd_改匕駝59A(_ do_IRQ)
         cat-6637   0D.hl      lOus : redirect_hardirq(_ doJRQ)
         cat-6637   0D. h.     12us : handle_IRQevent (_ do_IRQ)
         cat-6637   0D. h.     13us : timer_interrupt (handle_IRcLevent)
         cat-6637   0D. h.     15us : handle_tick_update (timer_interrupt)



                                                                                 561
        Embedded Linux Primer



            cat-6637 0D.hl l6us : do_timer (handle_tick_update)
                    <we 're in the timer interrupt function>
            cat-6637 0D. h.      22us : run_local_timers (update_process_t-imes)
            cat-6637 0D. h.      22us : raise_soft卄q(run_local_timers)
            cat-6637 0D. h. 23us : wakeup_softirqd(raise_softirq)
                    <softirq work pending - need to preempt is signaled>
            cat-6637 0Dnh.       34us : wake_up_process (wakeup_softirqd)
            cat-6637 0Dnh.       35us+: rcu_pending(update_process_times)
            cat-6637 0Dnh.       39us : scheduler_tick(update_process_times)
            cat-6637 0Dnh.       39us : sched_clock (scheduler_tick)
            cat-6637 0Dnh1 4lus : task_timeslice (scheduler_tick)
            cat-6637 0Dnh.       42us+: preempt_schedule(scheduler_tick)
            cat-6637 0Dnhl 45us : note_interrupt(_ do_IRQ)
            cat-6637 0Dnh1 45u5 : enab］已肛59凡卄M_do_I叩）
            cat-6637 0Dnhl 47u5 : preempt_schedule(enable_8259A_irq)
            cat-6637 0Dnh.       48us : preempt_schedule(_ do_IRQ)
            cat-6637 0Dnh.       48us : irq_exit (do_IRQ)
            cat-6637 0Dn. . 49us : preempt_schedule_irq(need_resched)
            cat- 6637 0Dn. .     SOus : me schedule(preempt_schedule_irq)
                    <here is the context switch to softirqd- timer thread>
          <. . .>-3      0D. .2 74us+: 1 switch_to(_ schedule)
          <. . .>-3      0D. .2 76us : _schedule <cat-6637] (74 62)
          <. . .>-3      0D. .2 77us : _schedule (schedule)
          <. . .>-3      00. .2 78us : trace_irqs_on(_ schedule)
                    <output truncated here for brevity>



      위 내용은 보기 쉽도록 일부 형식을 정리한 것이지만, 추적 데이터의 핵심 요소를 명백하게
      확인할 수 있다. 위 추적 결과는 타이머 인터럽트에 대한 결과이다. hardirq 쓰레드 내에서
      는 sof七irq 문맥에서 몇 가지 작업을 나중에 실행하도록 큐에 넣는 정도의 작업만 처리된
      다. 이는 23마이크로초에 수행된 wakeup sof七irqd () 함수에서 볼 수 있는데 , 이것이 일
      반적인 인터럽트 치리과정이다. 이 함수는 need resched 플래그를 켜게 되는데 , 이는 추
      적 항목의 두 번째 필드에서 세 번째 문자 n을 보면 알 수 있다. 49마이크로초에는, 타이머
      softirq를 처리한 후에 , 선점을 위해서 스케줄러가 호출된다. 그리고 74마이크로초에는
      제어권이 커널 내에서 PID 3을 갖는 실제 S（그ftirqd-七imer/ 0 쓰레드로 넘어간다（프로세
      스의 이름은 너비를 맞추기 위해서 ( . . .）로 생략되었다）.

      ［리스트 17-7］에서 볼 수 있는 각 필드는 대부분 명확하게 이해할 수 있다. irqs-off 필드
      는 인터럽트가 차단된 상태로 실행되는 코드에 대해서 D로 표시해 준다. 이 예제가 인터럽트

562
                                                         리눅스와 리얼 타임   Chapter 17



      차단에 대한 추적 결과이기 때문에 , 이 표시를 전체 내용에서 볼 수 있다. need resched
      필드는 커널의 need resched 플래그 상태를 그대로 표시해 준다. n 표시는 가능한 빨리
      스케줄러가 실행되어야 한다는 것을 의미하고 점（. ) 표시는 이 플래그가 꺼져 있음을 나타낸
      다. hardirq/ sof七irq 필드는 hardirq 문맥에서 실행될 경우에는 h7} 표시되고，
      softirq 문맥에서는 S가 표시된다. preempt尸depth 필드는 커널의 preempt coun七 변
      수의 값을 나타내 주는데, 커널 내에서 락(lock）이 얼마나 중첩되어 있는지를 나타낸다. 이
      숫자 값이 0일 때만 선점이 일어날 수 있다．


17 ,4.8 데드락 상태 디버깅하키
      커널 구성 옵션인 DEBUG DEADLOCKS는 커널 내에서 세마포어 (sema하iore）와 스핀락으로
      인한 데드락 상황을 감지해서 보고해 준다. 이 기능을 활성화시키면 앞으로 일어나는 데드락
      상황에서 다음과 같은 내용을 보고 받을 수 있다．




            [ BUG: lock recursion deadlock detected! I




      데드락을 알리는 이 배너 메시지 이후에 추가적으로 더 많은 정보가 출력된다. 여기에는 락
      에 대한 설명 , 락의 이름（가능한 경우만）, 락 파일과 그 이름（가능한 경우만）, 락의 소유자，
      현재 락을 확보하고 있는 프로세스 등이 포함된다. 이 디버깅 툴을 이용하면 문제가 되는 프
      로세스를 금방 잡아 낼 수 있다. 물론 문제를 해결하는 것17）은 그리 쉽지 않을 것이다！


17.4.9 락 모드 제어하기

      DEBUG RT LOCKING MODE 옵션은 커널 동작 중에 리얼 타임 뮤텍스를 선점 불가능한 모
      드로 되돌릴 수 있게 해 준다. 이 기능은 사실상（스핀락을 뮤텍스로 대체하는） 리얼 타임 커
      널을 원래의 스핀락 기반 커널로 되돌리는 역할을 하게 된다. 이 기능 역시 지금까지 설명한
      다른 구성 옵션과 마찬가지로, 오직 개발 환경에서만 사용할 수 있는 도움 기능이라고 생각
      하면 된다．

17) （역자주） 데드락을 해결하는 것은 상당히 어려운 작업 중의 하니t+. 우선 재현이 쉽지 않기 때문이다．


                                                                           563     I
훑흘繫
  mu     Embedded Linux Primer



        지금까지 설명한 모든 디버깅 기능은 동시에 켜서는 안 되는 것들이다. 누구나 예측할 수 있
        겠지만 이들 각각이 모두 커널 성능에 엄청난 부하를 주기 때문이다. 그래서 이 기능은 개발
        과정에 도움이 되는 툴로만 사용하고, 실제 제품 코드에서는 모두 비활성화시켜야 한다．



] 7.5 요약
        리얼 타임 성능이 요구되는 곳에서도 리눅스를 사용하는 경우가 늘고 있다. 그 예로 멀티미
        디어 응용 제품이나 로봇, 산업용 제어 기기 , 기타 자동 제어 장치 등을 들 수 있다．

         口 리얼 타임 시스템은 데드라인으로 특징지을 수 있다. 즉, 뎨드라인을 놓쳤을 때 그 결과
            가 약간의 불편함을 초래하거나 사용자의 사용성이 약간 떨어지게 된다면 우리는 이 경
            우를 소프트 리얼 타임이라고 한다. 반면에 하드 리얼 타임 시스템은 뎨드라인을 놓치면
            그 시스템은 실패한 것으로 판단한다．

         口 커널 선점은 시스템 차원의 지연성을 다루는 리눅스 커널의 첫 번째 주요 기능이다．

         口 최신 리눅스 커널은 몇 가지 선점 모드를 지원하는데, 비선점에서부터 완전한 리얼 타임
             선점형까지 모두 지원한다．

          [a 리얼 타임 패치를 적용하면 리눅스 커널에 몇 가지 주요한 기능이 추가되는데, 신뢰할
            만한 저지연성을 얻을 수 있다.

         口 리얼 타임 패치는 몇 가지 중요한 측정 도구를 제공하는데, 리얼 타임 리눅스를 디버깅하
            거나 특성을 파악하는 데 도움을 준다．



17.5. ] 더 읽어 보기
          Linux Kernel Development, 2nd Edition
          Robert Love
          Novell Press, 2005




a 564
A口口end以   A

   GNU 일반 공중 사용 허가서
          Embedded Linux Primer




        이 문서는 자유 소프트웨어 재단（Free Software Foundation）의 GNU General Public
        License를 한국어로 번역한 것입니다. 이 문서는 GNU General Public License가 내포
        하고 있는 호혜적인 자유와 공유의 정신을 보다 많은 사람들에게 알리기 위한 희망에서 작성
        되었지만, 자유 소프트웨어 재단의 공식 문서로 취급될 수는 없습니다. 이는 원래의 문서가
        의도하고 있는 내용이 왜곡되지 않고 법률적으로 유효하기 위해서 선행되어야 할 양국의 현
        행 법률과 언어의 적합성 여부에 대한 전문가들의 검토 작업에 많은 비용이 필요하기 때문입
        니다. 또한 공식 번역문으로 인정된 문서라 하더라도 다른 언어로의 번역에 따른 위험 부담
        은 여전히 남아 있게 됩니다. 따라서 자유 소프트웨어 재단은 오역이나 해석상의 난점으로
        인해서 발생될지도 모를 혼란과 분쟁의 가능성을 미연에 방지하고, 문서가 담고 있는 내용과
        취지를 보다 많은 사람들에게 알리려는 상반된 목적을, 한국어 번역문을 공식적으로 승인하
        지 않는 방법으로 양립시키고 있습니다．

        자유 소프트웨어 재단은 어떠한 언어에 대한 번역문도 공식적으로 인정하지 않고 있으며 , 그
        러한 계획 또한 갖고 있지 않습니다. 자유 소프트웨어 재단은 GNU General I뇨blic
        License를 실무에 적용할 경우, 오직 영문판에 의해서만 그 법률적 효력이 올바르게 발생될
        수 있음을 권고하고 있습니다. 이 번역문은 법률적 검토와 문서 간의 동일성 여부에 대한 검
        증을 거치지 않은 것이며 , 이로 인해서 야기될 수도 있는 법률적인 문제에 대해서 어떠한 형
        태의 보증도 제공하지 않습니다. GNU General Public License를 상업적인 목적으로 사
        용하려고 할 경우에는 변호사나 변리사에게 직접 자문을 구하기 바랍니다. 그러나 대부분의
        일반 사용자들에게는 이 번역문이 전딜하려고 하는 내용과 취지를 이해하는 것만으로도 충분
        할 것입니다．

        GPL에 대한 실제 사례를 모은 참고할 만한 자료의 하나로 GPL 해설이 있습니다．

        한국어 번역： 1998년 6월 18일 송창훈 妃hsong@gi끄i.org)




I 566
                                                 GNU 일반 공중 사용 허가서   Append汶 A




     2판, 1991년 6월

     Copyright((i)) 1989, 1991 Free Software Foundation, Inc.

     51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA

     누구든지 본 사용 허가서를 있는 그대로 복제하고 배포할 수 있습니다. 그러나 본문에 대한
     수정은 허용되지 않습니다．


전문
     소프트웨어에 적용되는 대부분의 사용 허가서 (license）는 소프트웨어에 대한 수정과 공유의
     자유를 제한하려는 것을 그 목적으로 합니다. 그러나 GNU 일반 공중 사용 허가서（이하，
     "GPL"이라고 칭합니다）는 자유 소프트웨어에 대한 수정과 공유의 자유를 모든 사용자들에게
     보장하기 위해서 성립된 것입니다. 자유 소프트웨어 재단이 제공하는 대부분의 소프트웨어들
     은 GPL에 의해서 관리되고 있으며 , 몇몇 소프트웨어에는 별도의 사용 허가서인 GNU 라이
     브러리 일반 공중 사용 허가서 (GNU Library General Public License）를 대신 적용하기
     도 합니다. 자유 소프트웨어란, 이를 사용하려고 하는 모든 사람에 대해서 동일한 자유와 권
     리가 함께 양도되는 소프트웨어를 말하며 프로그램 저작자의 의지에 따라 어떠한 종류의 프
     로그램에도 GPL을 적용할 수 있습니다. 따라서 여러분이 만든 프로그램에도 GPL을 적용할
     수 있습니다．

     자유 소프트웨어를 언급할 때 사용되는 "자유'라는 딘어는 무료（無料）를 의미하는 금전적인
     측면의 자유가 아니라 구속되지 않는다는 관점에서의 자유를 의미하며 , GPL은 자유 소프트
     웨어를 이용한 복제와 개작, 배포와 수익 사업 등의 가능한 모든 형태의 자유를 실질적으로
     보장하고 있습니다. 여기에는 원시 코드（source code）의 전부 또는 일부를 원용해서 개선된
     立로그램을 만들거나 새로운 프로그램을 창작할 수 있는 자유가 포함되며 , 자신에게 양도된
     이러한 자유와 권리를 보다 명확하게 인식할 수 있도록 하기 위한 규정도 포함되어 있습니다．

     GPL은 GPL 안에 소프트웨어를 양도받을 사용자의 권리를 제한하는 조항과 단서를 별항으
     로 추가시키지 못하게 함으로써 사용자들의 자유와 권리를 실제적으로 보장하고 있습니다．
     자유 소프트웨어의 개작과 배포에 관계하고 있는 사람들은 이러한 무조건적인 권리 양도 규
     정을 준수해야만 합니다．
 Embedded Linux Primer




예를 들어 , GPL 프로그램을 배포할 경우에는 프로그램의 유료 판매나 무료 배포에 관계없이
자신이 해당 프로그램에 대해서 가질 수 있었던 모든 권리를, 프로그램을 받게 될 사람에게
그대로 양도해 주어야 합니다. 이 경우, 프로그램의 원시 코드를 함께 제공하거나 원시 코드
를 구할 수 있는 방법을 확실히 알려 주어야 하고 이러한 모든 사항들을 사용자들이 분명히
알 수 있도록 명시해야 합니다．

자유 소프트웨어 재단은 다음과 같은 두 가지 단계를 통해서 사용자들을 권리를 보호합니다．
(1) 소프트웨어에 저작권을 설정합니다. (2) 저작권의 양도에 관한 실정법에 의해서 유효한
법률적 효력을 갖는 GPL을 통해 소프트웨어를 복제하거나 개작 및 배포할 수 있는 권리를
사용자들에게 부여합니다．

자유 소프트웨어를 사용하는 사람들은 반복적인 재배포 과정을 통해 소프트웨어 자체에 수정
과 변형이 일어날 수도 있으며 , 이는 최초의 저작자가 만든 소프트웨어가 갖고 있는 문제가
아닐 수 있다는 개연성을 인식하고 있어야 합니다. 우리는 개작과 재배포 과정에서 다른 사
람에 의해 발생된 문제로 인해 프로그램 원저작자들의 신망이 훼손되는 것을 원하지 않습니
다. GPL에 자유 소프트웨어에 대한 어떠한 형태의 보증도 규정하지 않는 이유는 이러한 점
들이 고려되었기 때문이며 , 이는 프로그램 원저작자와 자유 소프트웨어 재단의 자유로운 활
동을 보장하는 현실적인 수단이기도 합니다．

특허 제도는 자유 소프트웨어의 발천을 위협하는 요소일 수밖에 없습니다. 자유 프로그램을
재배포하는 사람들이 깨별적으로 특허를 취득하게 되면 결과적으로 그 프로그램이 독점 소프
트웨어가 될 가능성이 있습니다. 자유 소프트웨어 재단은 이러한 문제에 대처하기 위해서 어
떠한 특허에 대해서도 그 사용 권리를 모든 사람들（이하, "공중（公衆）"이라고 칭합니다）에게
자유롭게 허용하는 경우에 한해서만 자유 소프트웨어와 함께 사용할 수 있다는 것을 명확히
밝히고 있습니다.

복제（copying）와 개작（modification) 및 배포（dis缸小ution）에 관련된 구체적인 조건과
규정은 다음과 같습니다．
                                    GNU 일반 공중 사용 허가서   Append怏 A




복제와 개작 및 배포에 관한 조건과 규정

   제0조
   본 허가서는 GNU 일반 공중 사용 허가서의 규정에 따라 배포될 수 있다는 사항이 저작권자
   에 의해서 명시된 모든 컴퓨터 프로그램 저작물에 대해서 동일하게 적용됩니다. 컴퓨터 프로
   그램 저작물（이하, "프로그램"이라고 칭합니다）이란 특정한 결과를 얻기 위해서 컴퓨터 등의
   정보 처리 능력을 가진 장치（이하, "컴퓨터"라고 칭합니다） 내에서 직접 또는 간접으로 사용
   되는 일련의 지시 및 명령으로 표현된 창작물을 의미하고, "2차적 프로그램"이란 전술한 프로
   그램 자신 또는 저작권법의 규정에 따라 프로그램의 전부 또는 상당 부분을 원용하거나 다른
   언어로의 번역을 포함할 수 있는 개작 과정을 통해서 창작된 새로운 프로그램과 이와 관련된
   저작물을 의미합니다（이후로 다른 언어로의 번역은 별다른 제한없이 개작의 범위에 포함되
   는 것으로 간주합니다）. "피양도자'란 GPL의 규정에 따라 프로그램을 양도받은 사람을 의미
   하고, "원（原）프로그램"이란 프로그램을 개작하거나 2차적 프로그램을 만들기 위해서 사용된
   최초의 프로그램을 의미합니다．

   본 허가서는 프로그램에 대한 복제와 개작 그리고 배포 행위에 대해서만 적용됩니다. 따라서
   프로그램을 실행시키는 행위에 대한 제한은 없습니다 프로그램의 결과물（0毗put）에는, 그
   것이 프로그램을 실행시켜서 생성된 것인지 아닌지의 여부에 상관없이 결과물의 내용이 원프
    로그램으로부터 파생된 2차적 프로그램을 구성했을 때에 한해서 본 허가서의 규정들이 적용
    됩니다. 2차적 프로그램의 구성 여부는 2차적 프로그램 안에서의 원프로그램의 역할을 토대
   로 판단합니다.


    제1조
    적절한 처작권 표시와 프로그램에 대한 보증이 제공되지 않는다는 사실을 각각의 복제물에
   명시하는한, 피양도자는 프로그램의 원시 코드를 자신이 양도받은 상태 그대로 어떠한 매체
    를 통해서도 복제하고 배포할 수 있습니다. 복제와 배포가 이루어 질 때는 본 허가서와 프로
    그램에 대한 보증이 제공되지 않는다는 사실에 대해서 언급되었던 모든 내용을 그대로 유지
    해야 하며 , 영문판 GPL을 함께 제공해야 합니다．

    배포자는 복제물을 물리적으로 인도하는 데 소요된 비용을 청구할 수 있으며 , 선택 사항으로
    독자적인 유료 보증을 설정할 수 있습니다．
 器 二a    Embedded Linux Primer




        제2조
        피양도자는 자신이 양도받은 프로그램의 전부나 일부를 개작할 수 있으며 , 이를 통해서 2차
        적 프로그램을 창작할 수 있습니다. 개작된 프로그램이나 창작된 2차적 프로그램은 다음의
        사항들을 모두 만족시키는 조건에 한해서 , 제1조의 규정에 따라 또다시 복제되고 배포될 수
        있습니다．

          저Ii항 파일을 개작할 때는 파일을 개작한 사실과 그 날짜를 파일 안에 명시해야 합니다．

          제2항 배포하거나 공표하려는 저작물의 전부 또는 일부가 양도받은 프로그램으로부터 파생
          된 것이라면 저작물 전체에 대한 사용 권리를 본 허가서의 규정에 따라 공중에게 무상으로
          허용해야 합니다．

          제3항 개작된 프로그램의 일반적인 실행 형태가 대화형 구조로 명령어를 읽어 들이는 방식
          을 취하고 있을 경우에는, 적절한 저작권 표시와 프로그램에 대한 보증이 제공되지 않는다
          는 사실,（별도의 보증을 설정한 경우라면 해당 내용） 그리고 양도받은 프로그램을 본 규정
          에 따라 재배포할 수 있다는 사실과 GPL 사본을 참고할 수 있는 방법이 함께 포함된 문구
          가 프로그램이 대화형 구조로 평이하게 실행된 직후에 화면 또는 지면으로 출력되도록 작
          성되어야 합니다（예외 규정 : 양도받은 프로그램이 대화형 구조를 갖추고 있다 하더라도
          통상적인 실행 환경에서 전술한 사항들이 출력되지 않는 형태였을 경우에는 이를 개작한
          프로그램 또한 관련 사항들을 출력하지 않아도 무방합니다）.


        위의 조항들은 개작된 프로그램 전체에 적용됩니다. 만약, 개작된 프로그램에 포함된 특정
        부분이 원프로그램으로부터 파생된 것이 아닌 별도의 독립 저작물로 인정될 만한 상당한 이
        유가 있을 경우에는 해당 저작물의 개별적인 배포에는 본 허가서의 규정들이 적용되지 않습
        니다. 그러나 이러한 저작물이 2차적 프로그램의 일부로서 함께 배포된다면 개별적인 저작권
        과 배포 기준에 상관없이 저작물 모두에 본 허가서가 적용되어야 하며 , 전체 저작물에 대한
        사용 권리는 공중에게 무상으로 양도됩니다．

        이러한 규정은 개별적인 저작물에 대한 저작자의 권리를 침해하거나 인정하치 않으려는 것이
        아니라, 원프로그램으로부터 파생된 2차적 프로그램이나 수집 저작물의 배포를 일관적으로
        규제할 수 있는 권리를 행사하기 위한 것입니다．




I 570
                                 GNU 일반 공중 사용 허가서   Append怏 A



원프로그램이나 원프로그램으로부터 파생된 2차적 프로그램을 이들로부터 파생되지 않은 다
른 저작물과 함께 단순히 저장하거나 배포할 목적으로 동일한 매체에 모아 놓은 집합물의 경
우에는, 원프로그램으로부터 파생되지 않은 다른 저작물에는 본 허가서의 규정들이 적용되지
않습니다．


제3조
피양도자는 다음 중 하나의 항목을 만족시키는 조건에 한해서 제1조와 제2조의 규정에 따라
프로그램（또는 제2조에서 언급된 2차적 프로그램）을 목적 코드佃可ect code）나 실행물
(executable form)의 형태로 복제하고 배포할 수 있습니다．

  제l항 목적 코드나 실행물에 상응하는 컴퓨터가 인식할 수 있는 완전한 원시 코드를 함께
  제공해야 합니다. 원시 코드는 제1조와 제2조의 규정에 따라 배포될 수 있어야 하며, 소프
  트웨어의 교환을 위해써 일반적으로 사용되는 매체를 통해1 제공되어야 합니다．

  제2항 배포에 필요한 최소한의 비용만을 받고 목적 코드나 실행물어］ 상응하는 완전한 원시
  코드를 배포하겠다는, 최소한 3년간 유효한 약정서를 함께 제공해야 합니다. 이 약정서는
  약정서를 갖고 있는 어떠한 사람에 대해서도 유효해햐 합니다. 원시 코드는 컴퓨터가 인식
  할 수 있는 형태여야 하고 제1조와 제2조의 규정에 따라 배포될 수 있어야 하며 ，소프트웨
  어의 교환을 위해서 일반적으로 사용되는 매체를 통해1 제공되어야 합니다．

  제3항 목적 코드나 실행물에 상응하는 원시 코드를 배포하겠다는 약정에 대해서 자신이 양
  도받은 정보를 함께 제공해야 합니다（제3항은 위의 제2항에 따라 원시 코드를 배포하겠다
  는 약정을 프로그램의 목적 코드나 실행물과 함께 제공 받았고, 동시에 비상업적인 배포를
  하고자 할 경우에 한해서만 허용됩니다）.


저작물에 대한 원시 코드란 해당 저작물을 개작하기에 적절한 형식을 의미합니다. 실행물에
대한 완전한 원시 코드란 실행물에 포함된 모든 모듈들의 원시 코드와 이와 관련된 인터페이
스 정의 파일 모두그리고 실행물의 컴파일과 설치를 제어하는 데 사용된 스크립트 전부를 의
미합니다. 그러나 특별한 예외의 하나로서 , 실행물이 실행될 운영체제의 주요 부분（컴파일러
나 커널 등）과 함께（원시 코드나 바이너리의 형태로） 일반적으로 배포되는 구성 요소들은 이
러한 구성 요소 자체가 실행물에 수반되지 않는 한 원시 코드의 배포 대상에서 제외되어도
무방합니다．




                                                         571 I
          Embedded Linux Primer




        목적 코드나 실행물을 지정한 장소로부터 복제해 갈 수 있게 하는 방식으로 배포할 경우, 동
        일한 장소로부터 원시 코드를 복제할 수 있는 동등한 접근 방법을 제공한다면 이는 원시 코드
        를 목척 코드와 함께 복제되도록 설정하지 않았다고 하더라도 원시 코드를 배포하는 것으로
        간주됩니다．


        제4조
        본 허가서에 의해 명시적으로 이루어지지 않는한 프로그램에 대한 복제와 개작 및 하위 허가
        권 설정과 배포가 성립될 수 없습니다. 이와 관련된 어떠한 행위도 무효이며 본 허가서가 보
        장한 권리는 자동으로 소멸됩니다. 그러나 본 허가서의 규정에 따라 프로그램의 복제물이나
        권리를 양도받았던 제3자는 본 허가서의 규정들을 준수하는한, 배포자의 권리 소멸에 관계없
        이 사용상의 권리를 계속해서 유지할 수 있습니다．


        제5조
        본 허가서는 서명이나 날인이 수반되는 형식을 갖고 있지 않기 때문에 피양도자가 본 허가서
        의 내용을 반드시 蜘｝들여야 할 필요는 없습니다. 그러나 프로그램이나 프로그램에 기반한
        2차적 프로그램에 대한 개작 및 배포를 허용하는 것은 본 허가서에 의해서만 가능합니다．
        만약 본 허가서에 동의하지 않을 경우에는 이러한 행위들이 법률척으로 금치됩니다. 따라서
        프로그램（또는 프로그램에 기반한 2차적 프로그램）을 개작하거나 배포하는 행위는 이에 따
        른 본 허가서의 내용에 동의한다는 것을 의미하며 , 복제와 깨작 및 배포에 관한 본 허가서의
        조건과 규정들을 모두 받아들이겠다는 의미로 간주됩니다．


        제6조
        피양도자에 의해서 프로그램（또는 프로그램에 기반한 2차적 프로그램）이 반복적으로 재배포
        될 경우, 각 단계에서의 피양도자는 본 허가서의 규정에 따른 프로그램의 복제와 개작 및 배
        포에 대한 권리를 최초의 양도자로부터 양도받은 것으로 자동적으로 간주됩니다. 프로그램
        （또는 프로그램에 기반한 2차적 프로그램）을 배포할 때는 피양도자의 권리의 행사를 제한할
        수 있는 어떠한 사항도 추가할 수 없습니다. 그러나 피양도자에게 , 재배포가 일어날 시점에
        서의 제3의 피양도자에게 본 허가서를 준수하도록 강제할 책임은 부과되지 않습니다.




I 572
                             GNU 일반 공중 사용 허가서   Append次 A




제7조
법원의 판결이나 특허권 침해에 대한 주장 또는 특허 문제에 국한되치 않은 그밖의 이유들로
인해서 본 허가서의 규정에 배치되는 사항이 발생한다 하더라도 그러한 사항이 선행하거나
본 허가서의 조건과 규정들이 면제되는 것은 아닙니다. 따라서 법원의 명령이나 합의 등에
의해서 본 허가서에 위배되는 사항들이 발생한 상황이라도 양측 모두를 만족시킬 수 없다면
프로그램은 배포될 수 없습니다. 예를 들면, 특정한 특허 콴련 허가가 프로그램의 복제물을
직접 또는 간접척인 방법으로 양도받은 임의의 제3자에게 해당 프로그램을 무상으로 재배포
할 수 있게 허용하치 않는다면 그러한 허가와 본 사용 허가를 동시에 만족시키면서 프로그램
을 배포할 수 있는 방법은 없습니다．

본 조항은 특정한 상황에서 본 조항의 일부가 유효하치 않거나 적용될 수 없을 경우에도 본
조항의 나머지 부분들을 적용하기 위한 의도로 만들어졌습니다. 따라서 그 이외의 상황에서
는 본 조항을 전체적으로 적용하면 됩니다．

본 조항의 목적은 특허나 저작권 침해 등의 행위를 조장하거나 해당 권리를 인정하지 않으려
는 것이 아니라, GPL을 통해서 구현되어 있는 자유 소프트웨어의 배포 체계를 통합적으로
보호하기 위한 것입니다. 많은 사람들이 배포 체계에 대한 신뢰있는 지원을 계속해 줌으로써
소프트웨어의 다양한 분야에 많은 공헌을 해 주었습니다. 소프트웨어를 어떠한 배포 체계로
배포할 것인가를 결정하는 것은 전적으로 저작자와 기증자들의 의지에 달려 있는 것이지 , 일
반 사용자들이 강요할 수 있는 문제는 아닙니다.

본 조항은 본 허가서의 다른 조항에서 무엇이 중요하게 고려되어야 하는지를 명확하게 설명
하기 위한 목적으로 만들어진 것입니다．


제8조
특허나 저작권이 설정된 인터페이스로 인해서 특정 국가에서 프로그램의 배포와 사용이 함께
또는 캐별적으로 제한되어 있는 경우, 본 사용 허가서를 프로그램에 적용한 최초의 저작권자
는 문제가 발생하지 않는 국가에 한해서 프로그램을 배포한다는 배포상의 지역적 제한 조건
을 명시적으로 설정할 수 있으며 , 이러한 사항은 본 허가서의 일부로 간주됩니다．




                                                    573 I
        a    Embedded Linux Primer




            제9조
            자유 소프트웨어 재단은 때때로 본 사용 허가서의 개정판이나 신판을 공표할 수 있습니다．
            새롭게 공표될 판은 당면한 문제나 현안을 처리하기 위해서 세부적인 내용에 차이가 발생할
            수 있지만, 그 근본 정신에는 변함이 없을 것입니다．

            각각의 판들은 판번호를 사용해서 구별됩니다. 특정한 판번호와 그 이후 판을 따른다는 사항
            이 명시된 프로그램에는 해당 판이나 그 이후에 발행된 어떠한 판을 선택해서 적용해도 무방
            하고, 판번호를 명시하고 있지 않은 경우에는 자유 소프트웨어 재단이 공표한 어떠한 판번호
            의 판을 적용해도 무방합니다．


            제0조
            프로그램의 일부를 본 허가서와 배포 기준이 다른 자유 프로그램과 함께 결합하고자 할 경우
            에는 해당 프로그램의 처작자로부터 서면 승인을 받아야 합니다. 자유 소프트웨어 째단이 저
            작권을갖고있는소프트웨어의 경우에는자유소프트웨어 재단의 승인을얻어야합니다. 우
            리는 이러한 요청을 수락하기 위해서 때때로 예외 기준을 만들기도 합니다. 자유 소프트웨어
            채단은 일반적으로 자유 소프트웨어의 2차적 저작물들을 모두 자유로운 상태로 유지시키려
            는 목적과 소프트웨어의 공유와 재활용을 증진시키려는 두 가지 목적을 기준으로 승인 여부
            를 결정할 것입니다.


보증의 켤여（제］］조, 제］2조）

            제］1조
            본 허가서를 따르는 프로그램은 무상으로 양도되기 때문에 관련 법률이 허용하는 한도 내에
            서 어떠한 형태의 보증도 제공되지 않습니다 프로그램의 처작권자와 배포자가 공동 또는 개
            별적으로 별도의 보증을 서면으로 제공할 때를 제외하면 특정한 목적에 대한 프로그램의 적
            합성이나 상업성 여부에 대한 보증을 포함한 어떠한 형태의 보증도 명시적이나 묵시적으로
            설정되지 않은 "있는 그대로의" 상태로 이 프로그램을 배포합니다. 프로그램과 프로그램의 실
            행에 따라 발생할 수 있는 모든 위험은 피양도자에게 인수되며 이에 따른 보수 및 복구를
            위한 제반 경비 또한 피양도자가 모두 부담하먀 합니다．




I 574
                             GNU 일반 공중 사용 허7써   Appendix A




제12조
저작권자나 배포자가 프로그램의 손상 가능성을 사전에 알고 있었다 하더라도 발생된 손실이
관련 법규에 의해 보호되고 있거나 이에 대한 별도의 서면 보증이 설정된 경우가 아니라면
저작권자나 프로그램을 원래의 상태 또는 개작한 상태로 제공한 배포자는 프로그램의 사용이
나 비작동으로 인해 발생된 손실이나 프로그램 자체의 손실에 대해 책임지지 않습니다. 이러
한 면책 조건은 사용자나 제3자가 프로그램을 조작함으로써 발생된 손실이나 다른 소프트웨
어와 프로그램을 함께 동작시키는 것으로 인해서 발생된 데이터의 상실 및 부정확한 산출 결
과에만 국한되는 것이 아닙니다. 발생된 손실의 일반성이나 특수성뿐 아니라 원인의 우발성
및 필연성도 전혀 고려되지 않습니다．

복제와 개작 및 배포에 관한 조건과 규정의 끝．




                                                     575 I
A口口end怏   B

  小Bo아의 구성 가늉 명령에 셋
   難U     Embedded Linux Primer




        U-Boot에는 60개 이상의 구성 명령어가 있다. 최신 U-Boot에서 사용 가능한 명령에 목록
        을 ［표 B-i］에 정리했다. 이 명령에 외에도 많은 비공식적인 명령어가 있다. 일부는 특정
        하드웨어나 장비에만 해당하는 명령어도 있다. 완벽한 최신 명령어를 알고 싶으면 소스 코드
        를 확인해 보도록 하자. 명령어는 모두 U-Boot 소스 디렉터리에서 . . . /include/ cmd
        confdefs .h라는 헤더 파일에 정의되어 있다．

        ［표 日］] 나Boot 구성 명령에 목록

         명령에 집합                   명령에 / 기능

         CFG CMD BDI              bdinfo

         CEG CMD LOADS            loads

         CFG CMD LOADB            loadb

         CFG CMD IMI              iminfo

         CFG CMD CACHE            icache, dcache

         CFG CMD FLASH            flinto,   erase, protect

         CFG CMD MEMORY           md, mm, nm, mw, cp, cmp, crc, base, loop, mtest

         CFG CMD NET              bootp, tttpboot,   rarpboot

         CFG CMD ENV              saveenv

         CFG CMD KGDB             kodb

         CFG CMD P（꾜4CIA          POM（긔A 지워

         CFG CMD IDE              IDE 하드 디스크 지워

         CFG CMD PCI              pciinfo

         CFG CMD IRQ              irqinfo

         CFG CMD BOOTD            bootd


         CFG CMD CONSOLE          coninfo

         CFG CMD EEPRO卜4          EEPR아너 읽기／쓰71 지워

         CFG CMO ASKENV           화것 벼수에 대해서 짐무하71




在 578
                                     （尸Bo아의 구성 가능 명령에 셋   Append怏 B




명령에 집합               명령에 / 기능

CFG CMD RUN          환경 변수에 저장된 명령에 실행시키기

CFG CMD ECHO         인자를 출력해 줌

CFG CND I2C          120 시리얼 버스 지원

CFG CMD REGINFO      레지스터 덤프

CFG CMD IMMAP        IMMR 덤프 지원

CFG CMD DATE         AT（二，날짜／시간 등을 지원

CFG CMD DHCP         DHCP 지원

CFG CMD BEDBUG       BedBug 디버71 포함시키기

CFG CMD FDC          플로피 디스크 지원

CFG CMD SCSI         SCSI 지원

CFG CMD AUTOSCRIPT   Autoscript 지원

CFG CMD MII          MII지원

CFG CMD SETGETDCR    4xx에서 OCR 지원

CFG CMD BSP          BSP 기능（보드에 따른 명령어）

CFG CMD ELF          ELF(V刈Vor떼 로드／부트 명령에 지원

CFG CMD MISC         Sleep과 같은 기타 기능 지원

CFG CMD USB          USB 지원

CFG CMD DOC          미sk-on-ch巾 지원

CFG CMD JFFS2        JFFS2 지원

CFG CMD OTT          디지털 온도측정기 지원

CEG CMD SDR月l可       SDRAM 미MM SF0 정보 출력

CFG CMD DIAG         자쳬 진단

CFG CMD FPGA         FPGA 구성 지원




                                                               579 I
   難i1    Embedded Linux Primer




         명령에 집합                   명령에 / 기능

         CFG CMD HWFLOW           RTS/CTS 하드웨어 흐름 제어

         CFG CND SAVES            S 레코드 덤프를 저장

         CFG CND SPI              si기 유틸리티

         CFG CMD FDOS             日oppy DOS 지원

         CFG CND VFD              VFD 지원 (TRAB)

         CFG CMD NAND             NAND 지원

         CFG CMD BMP              BMP 지원

         CFG CMD PORTIO           Port I/O

         CFG CMD PING             다ng 지원

         CFG CMD MMC              MMC 지원

         CFG CMD FAT              FAT 지원

         CFG CMD IMLS             검색된 이미지를 모두 출력하기

         CFG CMD ITEST            정수（그리고 문자열） 테스트

         CFG CND NFS              NFS 지원

         CFG CMD REISER           Reiserfs 지원

         CFG CMD CDP              Cisco 미scovery 프로토콜

         CFG CMD XIMG             다중 이미지의 일부를 로드하는 기능

         CFG CND UNIVERSE         Tundra Universe 지원

         CFG CMD EXT2             EXT2 지원

         CFG CMD SNTP             SNTP 지원

         CFG CMD DISPLAY          Display 지원




I 580
A口口end怏   C

          BusyBox 명령어
  驥彗U    Embedded Linux Primer




        BusyBox에는 유용한 명령어가 아주 많다. 다음은 최신 BusyBox에서 문서화되어 있는 명
        령에 목록이다．



        addgroup           시스템에 사용자 그룹 추7F

                           시스템에 사용자 추7F

        ad：作imex           시스템의 기준시간 정보를 읽거나 선택적으로 설정하기

                            ar 압축 형식의 파일의 내용을 보거나 압축을 해제하기

        arping              ARP 요청과 응답을 이용해서 호스트의 핑 검사

                            ash 쉘명령에 처리기）

                            패턴 검사 및 처리 언어

                           디렉터리 경로명이나 파일 이름의 뒷부분을 잘라내기

        bunzip2            파일（입력 파일을 지정하지 않으면 표준 입력）의 압축 풀71

                            stdout으로 압축 해제

                            달력 표시

                            파일（들）을 결합시키고 표준 출력（stdout）으로 출력하7!

                            파일의 소유 그룹을 설정

                            파일 접근 권한 설정

                            파일의 소유자와 그룹을 설정

                            최상위 디렉터리를 변경함

                            전위 가상 터미널을 /dev/ t七yN으로 재설정

                            화면을 지우기

        cmp                 파일 비교

        cp                  파일 복사

        cp끄그                cpio 압축 파일 형식의 내용을 확인하2仁F 압축 해제

1582
                                             BusyBox 명령어   Append江 C



crond        BusyBox용 cron

crontab      crontab 제어 파일을 관리함

cut          입력 파일들어써 특정 필드를 표준 출력으로 출력함

date         시스템 시간을 표시하7仁F 설정

dc           작은 RPN 계산기

dd           옵션에 따라서 파일을 복사해서 변환하고 형식을 재설정 해 줌

deallocv七    사용하지 않는 가상 터미널 /dev/ ttyN을 해제

deigroup     시스템어써 사용자 그룹을 삭제

deluser      시스템에서 사용天를 삭저1

devfsd       devfs 사용 권한 및 구형 장치 심볼괵 링크를 관리하기 위한 데몬（폐기됨）

df           파일 시스템의 사용 공간과 여유 공간을 표시

dirname      파일 이름에서 디렉터리 경로'F 아닌 부분을 버림

dinesg       커널 링 버퍼를 제어하거나 내용을 출력함

dos2unix     DOS 형식의 파일을 UN以 형식으로 변환

dpkg         데비안 패키지를 설치, 제거， 관리할 수 있는 유틸리티

dpkg-deb     데비안 패키지를 대상으로 작업을 수행

du           파일 및 디렉터리 각각에 의해서 人F韶 디스크 공간을 요약

dumpkmap     이진 키보드 변환 표를 표준 출력에 표시해 줌

dumpleases   udhcpd에 의해서 할당받은 DH(下 'P 주소를 사용할 수 있는 시긴을 표시해 줌

echo         전달된 OL.仁들을 표준 출력으로 출력해 줌

env          현재 환경 변수 값들을 출럭하거나， 설정 후에 프로그램 실행

expr         수식 표현의 결과값을 표준 출력으로 표시

false        종료 코드 FALSE (1) 을 반환
豪1    Embedded Linux Primer




                        프레임 버퍼 설정을 표시하거나 수정

                        플로피 디스크 드라이브에서 디스크7F 바뀌었는지 검사

                        플로피 디스크으1 로우 포맷

                        正뙤션 테이블 수정

                        지정한 디럭터리 구조 아래에 있는 파일을 검색

                        파일을 입력으로 받아서 너비에 맞게 줄바꿈 해서 출력

                        시스템의 가용한 메모리 용량과 사豁인 메모리 용량 표시

                        지정한 램디스크에서 사용하는 모든 메모리 공간 해제

                        미닉스（M八Do 파일 시스템의 일관성 검사

     ftpget             FTP를 통해서 원격의 파일을 가져옴

                        日P를 통해서 파일을 원격으로 저장

                        커맨드 옵션을 분석함

                         tty를 열고， 로그인할 사용자 이름을 묻고 /bin/login을 실행

                        파일 또는 표준 입력0似］ 패턴 검색

     gunzip             파일의（또는 표준 입력 내용의） 압축 해제

     gzip               최대 압축률로 파일 압축

                        시스템 종료

     hdparm             하드디스크의 파라미터들을 읽거나 설정

     head               파일의 처음 ]0개 줄을 표준 출력에 표시

     hexdump            파일의 내용을 이진, B진수， 16진수 문자 또는 ]0진수 문자로 지정한 파일에 덤프

     hostid              사용하는 머신의 고유 32비트 식별자를 출력

     hos七name           호스트 이름을 읽거나 설정함

     httpd               http 서버로 들어오는 요청 처리
                                           BusyBox 명령어   Appendix C



           하드웨어 시계（RTC）를 읽거나 설정

           현재 사용자의 USERNAME 정보 출력

ifconfig   네트워크 인터페이스 설정

           인터페이스를 해제

ifup       인터페이스를 설정

           네트워크 연결을 대기하고 있다7F 필요한 프로그램 실행

           BusyBox용 mni七

           지정한 커널 모듈을 커널에 로드

           파일을 복사하고 속성 설정

'p         TOP胛 설정 유틸리티

ipaddr     인더페이스의 주소 변경

ipcaic     'P 주소를 통해서 'P 네트워크 설정 씬출

ipiink     인터페이스 설정을 변경

iproute    라우팅 테이블 항목을 표시하2仁F 설정

iptunnel   BusyBox용 iptunnei

           프로세스（들）에 시그널（기본 값은 S IGTERN）을 보냄

           모든 프로세스（들）에 시그널（기본 값은 SIGTERM）을 보냄

           커널 로거

           BusyBox 명령에 해석기 나＼me SHell

           시스템에 마지막으로 로그온 한 사용자의 목록 출력

           문자열의 길이 출력

in         타깃（TARGET）을 LINK NAME 또는 DIRECTORY7F 가리키도록 링크 생성

ioadfon七   표준 입력으로부터 콘솔에서 사용할 폰트를 읽어옴




                                                              585
   難1     Embedded Linux Primer




        loadkmap            표준 입력으로부터 이진 키보드 변환 표를 읽어옴

                            메시지를 시스템 로그에 기록

        login               시스템에서 새로운 세션 사작

                            현재 사용자의 이름 출력

                            syslogd의 메시지 출력

                            LOOPDEVICE와 파일 연결

                            디렉터리의 내용 출력

                            현재 로드되어 있는 커널 모듈 출력

                            여러 개의 블록 또는 캐릭터 특수 파일 생성

                            MD5 쳬크썸을 검사하7仁f 출력

                            터미널에 대한 쓰기 접근 제어

                            디렉터리를 새로 생성

                            명명된 파이프 생성（rnknod name p와 같음）

                           미닉스 파일 시스템 생성

                           특수 파일을 생성（블록, 캐릭터 또는 파이프）

        mkswap             스왑 파티션으로 사용할 디스크 파티션 생성

                           TEMP냐나E라는 기본 이름에 따라 임시 파일 생성

        modprobe           상위 레벨에서 모듈을 로드하거나 언로드

                           파일의 내용을 한 화면에 맞게 보여줌

                           파일 시스템을 마운트

                           자기 테잎 드라이브 제어

                           파일을 이동시키거나 이름 변경

                           네트워크 인터페이스가 꺼져 있을 때 그 이름을 바꿀 수 있음



1586
                                            BusyBox 명령어   Appendix C



             Netcat의 약자로, IP:port로의 파이프를 연다．

             리눅스 네트워크 정보 출력

nslookup     주어진 호스트으1 'P 주소를 위한 네임 서버 검색

             파일의 내용을 8진수나 다른 형식으로 덤프

             새로운 가상 터미널에서 명령 시작

passwd       사용자 암호 변경

patch        BusyBox용 patch

             프로세스의 미0를 얻는다

ping         네트워크 호스트들어께 ICMP ECHO REQUEST를 보냄

ping6        네트워크 호스트들어께 ICMP ECHO REQUEST를 보냄

pivot root   루트 파일 시스템 변경

r均weroff     시스템을 중단시키고 커널에게 시스템의 파워를 끄도록 요청

             사용자 입력에 따라서 형식에 맞춰 내용 출력

             프로세스의 싱퇘 보고

             현재 작업 디렉터리의 전체 이름 출력

             시스템 시간과 날짜 정보를 원격 弓人E쿠부터 읽어와서 설정

             심볼릭 링크의 값 출력

realpath     주어진 인자의 절대 경로 출력

             시스템 재부팅

              실행중인 프로세스의 우선各1 변경

              화면 재설정

 rm           파일（들）을 제거하거나 링크 해제

 rmdir        비어있는 디렉터리를 삭제



                                                                 587
難磊     Embedded Linux Primer




      rmmod              커널에서 지정한 커널 모듈 언로드

      rou七e              커널의 라우팅 테이블 편집

      ri가a                RPM 패키지

      rpm2 cpio           rpm 파일을 입력으로 받아서 cpio 출력

      run-par七S           디렉터리 내에 있는 여러 스크립트들을 실행

      rx                  xmod이 프로토콜을 이용해서 파일 수신

      sed                 스트림 에디터 sed

      seq                 표준 출력에 특정 범위의 숫자들을 출력

      setkeycod.es        커널의 스캔코드키코드 변환 맵을 설정

      shalsum             SHA] 체크썸을 검사하거나 출력

      sleep               지정한 시간민큼 지연 시간을 둠

      sort                지정한 파일에서 문자열 정렬

      start-st아） deemon 서비스를 시작하거나 정지하도록 설정

                          바이너리 파일 내에서 출력 가능한 문자열 출력

                          터미널 설정을 수정하거나 설정 상태 출력

                          사용자 口를 다른 것으로 바꾸거나 루트로 변경

                          단일 사용자용 Login

                          가상 메모리를 스왑하지 못하도록 함

                          가상 메모리를 스왑할 수 있도록 함

                          파일 시스템에서 버퍼에 있는 내용을 디스크에 강제로 기록

      sySc七l              실행중에 커널 파라미터 설정

                          리눅스 시스템 및 커널 로깅 유틸리티

                          파일의 마지막 ]0줄을 표준 출력에 표시



588
                                     BusyBox 명령어   Append怏 (;



         tar 파일을 만들거나 압축 해제 또는 압축된 내용 출력

         표준 입력의 내용을 7十 파일은 물론이고, 표준 출력에도 기록

         텔넷 클라이언트

         텔넷 서버

         파일 형식을 검사하거나 값을 비교

tftp     TFTP 프로토콜을 이용해서 파일 전송

         프로그램에서 사驅 시간 측정

         실시간으로 프로세서의 활동 상황 표시

         주어진 디LE들의 최종 수정 시간 갱신

         문자열을 변환하7仁F 입축하거나 지움

         'P 패킷의 흐름을 추적

         종료 코드 TRUE (O) 반환

         표준 입력에 연결되어 있는 파일 이름 출력

         DH(午 클라이언트

udhcpd   DHCP 서버

         파일 시스템을 언마운트

         특정 시스템 정보 출력

         z 파일（들）의 압축 해제

         일치하는 문자열은 햐나를 제외하고 모두 무시

         파일을 UN以 형식에서 DOS 형식으로 변환

         乙P 압축 파일의 압축 해제

uptime   부팅한 후 현재까지의 사용 시간 출력

         n 마이크로초만큼 지연



                                                        589
 Embedded Linux Primer




                    uuenco（把로 인코딩된 파일을 디코딩

                   파일은 uuencode시킴

vconfig            가상 이더넷 장치를 생성하거나 지울 수 있게 해 줌

                    VI 에디터

                   가상 터미널을 잠금． 해제할 때 암호를 물어봄

                   프로그램을 주기적으로 실행

                   지정한 와치독 장치에 주기적으로 값을 기록

                    7十 파일이 담고 있는 문자열의 수＝, 문자의 수， 단어의 수를 출력

                   HTVP 또는 FTP를 이용해서 파일을 읽음

                   어떤 명령이 어디에 위치하는지를 알려줌

                   현재 사용자 이름과 관련 정보 표시

                   현재 실효 사용자 ID와 연결된 사용자 이름 출력

                   표준 입력으로 전달된 모든 항목을 인자로 명령에 실행

yes                문자열을 반복해서 출력

zcat               입축을 해제해서 stdout으로 내보냄．
A口pend以        D

     SDRAM 인터페이스 고려 사항




이번 장에서 배울 내용

  a SDRAM 기초

  . 클럭

  . SD日AM 설정

  . 요약
  a.    Embedded Linux Primer




       언뜻 보면 SDR／小4 컨트롤러를 프로그래밍하는 일은 아주 복잡해 보인다. 실제로 엄청나게 다
       양한 동기식 동적 임의 접근 메모리（축약해서 DRAM: Synchronous Dynamic Random
       Access Me跏ry) 기술이 개발되었다. 성능과 집적도를 위한 끝없는 노력의 결과로 여러 아
       키텍처와 동작 방식이 고안되었기 때문이다．

       AMCC PowerPC 405GP 프로세서를 이용해서 SDRAM 인터페이스에 대해서 살펴볼 것
       이다. 아마도 SDRAM 인터페이스에 관련된 문제를 해결하기 위해서는 SDRAM의 사용자
       매뉴얼을 참고해야 할 때가 있을 것이다. 이 콴련 문서들은 D.4.1절에 "더 읽어 보기"에 나와
       있으니 참고하도록 하자．



D.1 SDRAM 기초
       SDRAM을 설정하는 방법을 이해하기 위해서는 SDRA匹 장치가 동작하는 기본 원리를 먼
       저 이해해야 한다. 우선 간단하게 살펴보면 SDRAM은 데이터를 저장할 수 있는 단위인 셀
       (cell)이 행렬 형태로 모여 있는 구조로 이루어져 있다. 그리고 주소 비트의 일부는 행
       (column) 주소를 가리키고, 나머지 일부는 열（row) 주소를 지정하도록 할당되어 있다. ［그
       림 D山은 이 형태를 설명해 주는 그림이다．

       메모리 행렬 내의 회로는 매우 복잡하다. 좀 더 간략화한 읽기 동작은 다음과 같이 진행된다．
       먼저 열 주소 신호 선에 열 주소 값이 실리고 그 후에 행 주소 신호 선에 행 주소가 실린다．
       그리고 얼마간의 시간이 흐르면 입력된 행과 열 주소에 해당하는 메모리에 저장되어 있는 데
       이터가 프로세서가 사용하는 데이터 버스에 실리게 되는 것이다．

       프로세서는 열 주소를 SDRAM의 주소 신호 선에 내보낼 때 RAS1)（열 주소 선택） 신호를
       활성화（assert）시킨다. 그리고 SDRAM 회로가 열 주소를 인식할 수 있도록 미리 프로그램
       된 지연 시간이 흐르고 난 뒤에 프로세서는 행 주소를 내보내고 CAS（행 주소 선택） 신호를
       활성화시킨다. SDRAM 컨트롤러는 실제 물리 메모리 주소를 열과 행 주소로 변환한다. 많
       은 SDRAM 컨트롤러들이 열과 행의 너비를 따로 설정할 수 있도록 되어 있다. PPC405GP
       도 마찬가지인데 , 나중에 SDRAM 컨트롤러를 설정하는 과정에서 이 부분이 반드시 필요한
       부분임을 보게 될 것이다.


1) （역자주） 보통 소리 나는 대로 라스라고 부르기도 한다. 곧 설명할 CAS의 경우도 카스라고 부르기도 한다．


 5
                                                        SDRAM 인터페이스 고려 사항   샤巾end怏 D




                            SDRAM 메모리
                  CLK         셀 배열


                   RAS



                  열 주소
                                                                     >"俄首

     지五뀌쟈 듣＜工Dm
                         Latch


                   CAS
                                      』r   "   "\   노




                  행 주소



                          atch

     I 그림 D너 간략히 표현한 SDRAM 블록 다이어그램


     물론 지금 설명한 예제는 실제보다 훨씬 간략한 형태치만 기본 개념은 같다. 예를 들어 , 한꺼
     번에 네 곳의 메모리 위치를 모두 읽는 버스트 읽기（burst-read）의 경우 RAS와 CAS를
     한 번만 거치고 나머지는 SDRAM 회로 내부에서 자동으로 행 번호를 증가시켜 가면서 나머
    지 세 개의 위치를 읽을 수 있게 해 주기 때문에 , 프로세서가 네 번의 CAS를 따로 보낼 필요
     가 없게 된다. 이 기술은 성능 여러 최적화 기술의 한 예에 불과하다. 이 내용을 올바로 이해
     하키 위해서는 역시 실제 메모리 칩의 세부 사항을 연구해 보는 것이 가장 좋다. 여러 데이터
     시트 중에서도 잘 쓰여진 것들은 D.4.1절 "더 읽어 보기"에서 참고할 수 있다．


D. ] . ] SDRAM 리프레시
     하나의 SDRAM 셀은 트랜지스터 하나와 커패시터 하나로 이루어져 있다. 트랜지스터는 셀
     을 충전하기 위한 것이고, 커패시터는 셀의 값을 유지（저장）하는 일을 한다. 커패시터는 짧
     은 시간 동안에만 데이터를 저장해 둘 수 있는데 , 그 이유는 이 책의 범위를 벗어나기 때문에
     설명하지 않겠다. 동적 메모리의 가장 기본적인 특징 중의 하나가 각 셀에서 커패시터가 담



                                                                                593I
 難必1     Embedded Linux Primer




      고 있는 데이터를 주기적으로 재충전해 주어야 한다는 점이다. 그리고 이 작업을 SDRAM
      리프레시라고 부른다．

      리프레시 주기는 메모리칩 에서 메모리의 내용을 읽거나 쓸 수 없는 특별한 기간이다. 이 기
      간 동안 필요한 리프加시를 수행하게 된다. SDRAM 컨트롤러의 가장 주요한 임무 중의 하
      나도 바로 칩의 요구에 맞게 리프레시 주기 시간을 보장해 주는 일이다．

      칩 생산 업체는 최소한의 리프레시 주기를 명시하고 이 주기 내에만 리프레시가 된다면 아무
      런 문제가 없도록 하는 것은 설계자의 몫이다. 보통 SDRAM 컨트롤러는 리프레시 주기를
      직접 설정할 수 있도록 되어 있다. 우리가 사용할 PowerPC 405GP도 이 용도를 위한 레지
      스터가 별도로 존재하는데 , 이 레지스터에 대해서는 곧 살펴볼 것이다．



D.2 쿄럭
      동기섹＄ynchronous）이라는 용어는 SDRAM 장치의 읽기 , 쓰기 주기가 CPU가 제공하는 클
      럭 신호와 일치해야 한다는 것을 암시한다. SDR SDRAM은 읽기와 쓰기가 매 SDRAM 클
      럭 주기에 맞춰서 수행된다. DDR SDRAM은 읽기와 수행이 매 클럭 주기마다 두 번씩 일어
      나는데 , 클럭의 상승 에지（EDGE）와 하강 에지 각각에서 연산이 수행되기 때문이다．

      최신 프로세서는 좀 더 복잡한 클럭 서브시스템을 가지고 있다. 즉, 시스템의 여러 위치에
      다른 속도의 클럭이 사용된다. 일반적인 프로세서는 메인 클럭의 소스로서 크리스털에서 발
      진되는 상대적으로 느린 주파수의 클럭을 이용하고 위상 동기 루프（PLL2) : Phase
      Locked Loop）를 이용해서 CPU가 사용할 메인 클럭（보통 CPU의 속도를 이야기할 때는
      이 속도를 말한다）을 생성해 낸다. 일반적으로 CPU는 메모리 서브시스템보다 훨씬 빨리 동
      작하기 때문에 메인 클럭을 분주해서 SDRAM 서브시스템에 공급하게 된다. 그래서 독자는
      자신의 CPU와 SDRAM 조합을 위해서 알맞은 클럭 속도와 비율을 설정해1 주어야 한다．

      프로세서와 메모리 서브시스템이 사용하는 클럭은 반드시 SDRA玉4이 올바로 동작하는 범위
      에서 알맞게 설정해야 한다. 사용하는 프로세서 매뉴얼에는 보통 클럭 설정과 관리에 대한
      섹션이 있는데 , 이 부분을 참고해서 보드 설계에 맞는 올바른 값을 설정해야 할 것이다．



2) （역자주） 보통은 그냥 피엘옐이라고 부른다．
                                       SDRAM 인터페이스 고려 사항    Appendix D



AIvICC 405GP도 이런 설정이 필요한 전형적인 프로세서라고 볼 수 있다. 크리스털이 발진
해서 만들어 내는 클럭을 입력으로 받아서 서브시스템 내외에서 사용할 몇 가지 클럭을 만들
어 내는데 여기에는 CPU를 위한 클럭 , PCI 인터페이스, 온 보드 주변 장치 버스（아下 :
Onboard Peripheral Bus) , 프로세서 지역 버스（PLB : Processor Local Bus) , 메모리
클럭小血mClk) 그리고 타이머와 UART 등의 주변 장치를 위한 내부 클럭이 포함된다. 전
형적인 구성은 ［표 D-1］과 같은 형태가 될 것이다．

［표 D-1 ] 전형적인 PPC405GP 클럭 구성

 클럭          속도       비고

 크리스털        33MHz    뜨세서에 공급되는 기본 소스 클럭

 CPU 클럭      133MHz   프로세서의 내장 미에 의해서 민들어지며, 외부 하드웨어 핀이나
                      레지스터 값으로 설정힌CF.

 PLB 클럭      66MHz    CPU 클럭을 분주해서 사용한다. 외부 하드웨어 핀이나 레지스터
                      값으로 설정할 수 있다. 프로세서 내부에서 고속의 모듈과 프로세서
                      간의 데이터 교환을 위한 지역 버스에서 사驅다．

 OPB 클럭      66MHz    PLB 클럭에서 분주해서 사용하고 레지스터로 설정한다. 상대적으로
                      다른 장치들을 위해서 사용된다．

 PCI 클럭      33MHz    PLB 클럭에서 분주하며, 레지스터를 통해서 설정한다．

 Mem（긔k      100MHz   SDRAM 칩에 바로 공급된다. CPU 클럭을 분쭈해서 사용하는더1
                      레지스터로 설정 가능하다．


클럭 설정에 대한 결정은 보통 초기 하드웨어를 설계하는 시점에 미리 결정되어 있어야 한다．
외부 하드웨어 핀을 이용해서 초기 클럭 값을 설정하는 작업은 프로세서 자체는 할 수 없는
일이기 때문이다. 파생된 클럭에 대한 내부 분주 비를 설정하는 것은 프로세서 내부에서 클
럭과 서브시스템을 제어하는 전용 레지스터를 통해서 가능한 경우도 있다. 여기서 우리가 사
용하는 405GP의 경우도 최종 클럭 구성은 외부 하드웨어 핀과 펌웨어 구성을 통해서 결정
된다. 처음에 보드에 전원이 공급된 후에 프로세서의 레지스터를 설정해서 내부 클럭의 분주
비를 설정하는 작업은 부트로더가 담당한다．




                                                                 595I
 二m 1     Embedded Linux Primer




D.3 SDRAM 설정
        클럭이 올바로 설정되고 난 다음에는 SDRAM 컨트롤러를 초기화해야 한다. 프로세서마다
        내장되어 있는 SDRAM 컨트롤러가 각기 다르다. 하지만 결과적으로는 같은 일을 하게 된
        다. 즉, 알맞은 클럭과 타이밍 정보를 설정해서 SDRAM 서브시스템을 최적화하는 일이다．

        이 책에서 다루는 다른 내용들과 마찬가지로 지금 초기화하려고 하는 하드웨어 역시 하드웨
        어를 깊이 이해하는 것 외에 다른 방도는 없다. 특히 SDRAM의 경우는 더 그렇다. 이 부록
        에서 SDRAM의 설계 측면까지 다루는 것은 무리이기 때문에 일부 꼭 이해하고 넘어가야
        할 기본 지식만 짚고 넘어갈 것이다. 여러 SDRAM 생산 업체의 데이터 시트에는 도움이
        될 만한 기술적인 설명도 같이 포함되어 있다. 독자는 이런 데이터 시트에 익숙해져야 한다．
        물론 SDI캅小/1 서브시스템을 올바로 설정하는 데 하드웨어 엔지니어링 관련 학위 따위가 필
        요한 것은 아니지만, 어느 정도는 내부를 이해하고 있어야 한다.

        이제부터 405GP 프로세서에 내장된 SDRAM 컨트롤러를 이용해 보자. 이 예제에서는 7
        장, "부트로더"에서 다룬 U-Boot 로더에 의해서 초기화가 이루어진다. 7장의 내용을 다시
        돌이켜 보면 4xx 프로세서를 위한 디렉터리에 있는 start . S에서 SDRAM 초기화를 위한
        후킹 함수를 호출하는 어셈블러 코드를 볼 수 있었다. 7.4.4절 "보드에 따른 초기화'를 다시
        참고하도록 하자. ［리스트 D-1]에는 U-Boot 소스 코드인 . . . /cpu/ppc4xx/ sdram.c
        파일의 sdram i nit () 함수를 다시 나타냈다.

        ［리스트 D) ppc4xx 나Boot 코드에서 S（打am_init() 부분

           01 void sdramjinjt (void)
           02 {
           03     ulong sdtrl;
           04     ulong rtr;
           05     Tht I ;
           06
           07     /*
           08     六 100MHz , 133MHZ SDRAM 지원
           09     士／
           10     if (geubusHfreq (0) > 100000000) {
           11          /""
           12          * 133 MHz SDRAM
           13          士／


 596
                                             SDRAM 인터페이스 고려 사항       Append江 D



 14       sdtrl = 0x01074015;
 15       rtr = 0x07f00000;
 16   }else{
 17       ／央
 18       六 기본 값： 100 MHz SDRAM
 19       央／/
 20       sdtrl = 0x0086400d;
 21       rtr = 0x05f00000;
 22   }
 23
 24   for (= O; i<N_MBOCF; i++) {
 25        ／六
 26        女 메모리 컨트롤 비활성화
 27        士／
 28        mtsdramo (mem_mcoptl, 0x00000000) ;
 29
30        ／士
31        央 0번 뱅크를 위해서 MBOCF 설정
32        央／
33        mtsdramo (mem_mb0cf, mb0cf[ i] .reg) ;
34        mtsdranio (mem_sdtrl, sdtrl) ;
35        mtsdramO (mem_rtr, rtr) ;
36
37        udelay (200) ;
38
39        /／央
40        六 메모리 컨트롤러 옵션 레지스터 설정
41        玄 16바이트 PLB 버스트 읽기／가져오기를 위해서
42        六 DC_EN 비트와 BRD_PRF 비트를 1로 설정함．
43        '"/
44        mtsdramo (mem_mcoptl, 0x80800000) ;
45
46        udelay(10000) ;
47
48        if (get_ram_size(0, mb0cf[i] .size) == mb0cf[i] .size) {
49             ／央
50             "" 크기를 확인했음 H> 모두 완료
51             V
52             return;
53        }
54    }
55}




                                                                        597I
         Embedded Linux Primer




       이 코드가 맨 처음 하는 일은 405GP 프로세서에 연결된 외부 핀 상태를 읽어서 SDRAM
       클럭을 위한 값을 읽는 일이다. 위 경우에는 두 가지 값이 가능한 것을 알 수 있는데 각각
       100MHz와 133MHz이다. 이 선택에 따라서 SDRAM 컨트롤러에 올바른 값을 설정하기
       위한 상수 값이 결정이 된다．

       24번 줄부터 시작되는 반복문은 다섯 가지의 메모리 크기에 따른 파라미터를 설정하는 데
       이용된다. 현재 U-Boot는 각각 4MB, 16MB, 32MB, 64MB 또는 128MB 용량의 단일
       뱅크 메모리를 지원한다. 이 용량 값들은 . . . 凡pu/ppc4xx/ sdram. c 파일에 mbOcf라는
       이름의 표로 정의되어 있다. 이 표는 각 메모리 크기에 대해서 상수 값을 정의하는데 각각
       405GP 메모리 뱅크 설정 레지스터를 위한 값이다. 반복문은 이렇다.



         for (i = 각각의 가능한 메모리 뱅크 크기에 대해서， 가장 큰 것부터） {
              SDRAM 클럭 속도에 따른 타이밍 상수를 선택함；
              SDRAM 메모리 컨트롤러를 비활성화；
              0번 뱅크를 용량［i] , 타이밍 상수[i］로 설정
              SDRAM 메모리 컨트롤러를 다시 활성화시킴；


              동적으로 메모리 용량을 감지하71 위한 간단한 메모리 검사를 수행；
               ／士 이 작업을 위해서 get_ram_si zeQ7F 사용됨 央／
              if ( 확인한 용량 == 설정한 용량 )
                   완료；
          }


       이 간단한 코드는 SDRAM 클럭 속도와 U-Boot에 미리 직접 입력해 둔 메모리 뱅크 용량에
       대한 표를 통해서 올바른 타이밍 상수를 찾아낸다. 이 내용을 이해한다면 405GP 참조 매뉴
       얼을 이용해서 뱅크 설정 값을 설정할 수 있을 것이다. 한 예로 64MB DRAM의 경우에 메
       모리 뱅크 설정 레지스터 값은 다음과 같다．

          0번 메모리 뱅크 설정 레지스터 = 0x000a4001


       PowerPC 405GP 사용자 매뉴얼에는 0번 메모리 뱅크 설정 레지스터를 설정하기 위해서
       사용되는 항목을 설명하고 있는데 , ［표 D-2］에 그 항목들이 나와 있다．




i598
                                           SDRAM 인터페이스 고려 사항   Appendix D



［표 [)-2] 405GP 0번 메모리 뱅크 설정 레지스터 비트 필드

 필드                          값        설명

 뱅크 주소（BA : Bank Address)    OxO0     이 뱅크에 해당古는 메모리 시작 주소

 크기（SZ)                      0x4      뱅크의 메모리 크기 이 경우 64MB

 주소 방식                       0x2      메모리 구조를 선택함． 여기어는 열, 행에 대한
 (AM : Addressing 卜加de)               비트수도 포함된다. 이 경우에 해당하는 모드 2는
                                      12개의 열 주소 비트와 9 또는 ]0개의 행 주소
                                      비트를 갖고， 최대 4개의 내부 SDRAM 뱅크를
                                      갖는 구조를 匕똬낸다． 이런 데이터는 405GP
                                      사용자 매뉴얼에 나와 있다．

 뱅크 활성화                      小＜1      이 레지스터에 설정한 값을 반영하도록 활성화시킴．
 (Bank Enable : BE)                   405GP에는 각각 뱅크를 위해서 모두 4개의
                                      레지스터7F 있다．


이 표에 있는 값들은 모두 보드에서 사용되는 메모리 모듈에 맞도록 보드 설계자가 결정해야
한다．

타이밍 관련 예제를 통해서 전형적인 SDRAM 컨트롤러를 위한 타이밍 조건을 자세히 알아
보자. 먼저 SDRAM 클럭으로 100MHz를 사용하고 용량은 64MB이며 , ［표 D-1］에 있는
sdram init () 함수에서 선택된 타이밍 상수 값을 이용한다고 가정하자. 이 경우 타이밍
상수 값은 다음과 같다．



   SDRAM 타이밍 레지스터           = 0x0086400d
   리프레시 타이밍 레지스터            = 叭0 Sf00000



PowerPC 405GP 사용자 매뉴얼에는 SDRAM 타이밍 레지스터를 설정하는 데 사용되는
필드들을 설명하고 있다. ［표 D-3］에서 이 필드들을 볼 수 있다．




                                                                    599
    蠶     Embedded Linux Primer




        ［표 [)-3] 405GP의 SDRAM 타이밍 레지스터 필드

                                  값     설명

         CAS 지연 시간                Oxi   SDRAM의 CAS 지연 시간. 이 값은 SDRAM 칩 명세서에서
         (CASL)                         가져온 것이다. 이 값은 읽기 명령（CAS 신호）를 보낸 후에 데이터
                                        버스에 데이터7F 가용하게 될 때까지 걸리는 지연 시간을 클럭
                                        사이클 단위로 나타낸 것이다. 이 경우 Oxi은 405GP 사용자
                                        매뉴얼에서 볼 수 있듯이 클럭 사이클 두 개를 의미한다．

         PTA（프리차지 명령부터            Oxi   SDRAM에서 프리차지（Precharge) 명령은 주어진 한 열을
         C음 활성화까지의 시갼）                  비활성화시킨다. 대조적으로 활성홰Activate) 명령어는 해당
                                        열을 활성화시켜서 버스트 모드로 접근할 때와 같이 데이터를
                                        추7匠 접근할 수 있게 해 준다. 이 타이밍 값은 프리차지와 이후
                                        활성화 명령 사이클 사이의 최소 사긴을 결정하는더1, 이 값은
                                        SDRAM 칩에 따라서 결정된다. 그래서 SDRAM 칩 명세서0似｛
                                        올H른 값을 얻어야 힌따. 이 경우 0xi은 4050P 사용자
                                        매뉴얼에서 볼 수 있듯이 클럭 사이클 두 개를 의미한다．

         CTP（읽기／쓰기부터              0x2   이 타이밍 파라미터 값은 SDRAM의 읽기 또는 쓰기 명령
         프리차지까지의 최소                     후부터 프리차지 명령에 사이의 최소 지연 시간을 결정한다. 이
         시간）                            값 역시 SDFRAM 칩 명세서어써 알맞은 값을 구해야 한다. 이
                                        경우 0x2는 405GP 사용자 매뉴얼에 나와 있듯이 클럭 사이클
                                        세 개를 의미한다．

         LDF                      0xi   이 타이밍 값은 주소 값 또는 명령어를 보낸 후부터 뱅크 선택
         SDRAM 명령에 착수                   신호를 켤 때까지의 최소 시간을 결정한다. 이 값 또한 SDRAM
         시간                             칩 명세서를 참고해서 올U른 값을 얻어o 한다. 이 경우 Oxi은
                                        405GP 사용자 매뉴얼에 있는 것처럼 클럭 사이클 두 개를
                                        의미힌타．


        ［리스트 D-1］의 U-Boot 예제에서 마지막으로 설정하는 파라미티는 리프레시 타이밍 레지
        스터 값을 설정하는 것이다. 이 레지스터는 SDRAM 컨트롤리의 리프레시 주기를 설정하는
        필드 하나만을 가지고 있다. 이 필드의 값은 단순히 SDRAM 클럭의 횟수로서 시간 주기를
        표현한다. 이 예제에서는 SDRAM 클럭 주파수가 100MHz라고 가정했다. 예제에서 이 레
        지스터에 쓴 값은 0x05f0_0000이다. PowerPC 405GP의 사용자 매뉴얼을 통해서 이 값
        이 15.2마이크로초 주기로 리프레시가 이루어지도록 설정한 것을 알 수 있다. 다른 타이밍
        파라미터 값과 마찬가지로 이 값도 SDRAM 칩 명세서에 정의되어 있다．


I 600
                                                 SDRAM 인터페이스 고려 사항      Append怏 0



     전형적인 SDRAM 칩은 각 열에 대해서 한 번씩 리프레시가 가능하다. 즉, 칩 생산자가 규정
     한 최소 시간 내에 각 열 단위로 천체 리프레시가 이루어져야 한다. D.4.1절 "더 읽어 보기"
     에 있는 칩 참고 자료에는 전체 8.192개의 열이 매 64밀리초 내에 리프레시 되어야 한다고
     규정되어 있다. 이는 전체 열을 리프레시하기 위해서 매 7.8마이크로초마다 리프레시 명령
     을 보내야 한다는 의미가 된다．



D.4 요약
     SDRAM 장치는 상당히 복잡하다. 이 부록에서는 복잡한 SDR사vi 컨트롤러 설정을 돕기
     위해서 간단한 예제를 살펴본 것이다. SDRAM 컨트롤러는 아주 중요한 일을 하기 때문에
     올바로 설정해 주어야 한다. 역시 이 작업을 위한 최고의 해답은 명세서를 세심하게 분석하
     고, 그 내용을 이해하는 것밖에 없다. 참고 자료에 나와 있는 두 개의 예제 문서를 시작으로
     삼으면 좋을 것이다．


D.4. ] 더 읽0j 보기
       AMCC 405GP 임베디드 프로세서 사용자 매뉴얼
       A入｛C（그 사
       www. amcc. corn/Embedded!


       마이크론 테크놀로지 사（Micron Technology, Inc.)
       Synchronous DRAM MT48LC64M4A2 데이터 시트
       http://download.micron. com/pdf/datasheets/dram/sdram/256MSDRAM. pdf
A口口end以   E

          오픈 소스 리소스
        Embedded Linux Primer




소스 저장소 및 개발자 정보

      리눅스 개발에 초점을 맞춘 웹 사이트가 몇 7가 있다. 다음은 다앙한 아키텍처와 프로젝트를
      위한 웹사이트 중에서 가장 중요한 것들을 나열한 것이다．

         커널 소스 1차 저장소
         www.kernel. org


         커널 GIT') 1차 저장소
         www.kernel.org/git


         PowerPc그 관련 개발 정보 및 메일링 리스트
         http: //ozlabs. org/


         MIPS 관련 개발 정보
         www.linux-mips. org


         ARM 관련 개발 정보
         www. armS linux. org.uk


         방대한 오픈 소스 프로젝트를 배양하고 있는 저장소
         http: //sourceforge.net



1I일링 리스트
      수천까지는 아니더라도 수백 개에 달하는 메일링 리스트가 리눅스의 모든 분야와 오픈 소스
      개발에 관한 정보를 제공하고 있다. 여기서는 그 중혀］ 일부를 소개한다. 메일링 리스트에 내
      용을 포스팅하기 전에 메일링 리스트에 대한 에티켓을 먼저 숙치하기 바란다．




1) （역자주） G1T는 대규모의 프로젝트를 위해서 개발뒨 버전 관리 시스템이다. 주로 오픈 소스， 그 중에서도 커녈 소스를 관리하기
    위해서 많히 人용된다．
                                                                  오픈 소스 리소스   Append以 E



       메일링 리스트의 대부분이 나중에 검색을 위해서 내용을 보관해 두고 있다. 어떤 문제가 발
       생했다면 이 보관된 문서를 먼처 검색해 보자. 대부분의 경우 같은 내용의 질문과 답변이 이
      미 존재할 것이다. 공공 메일링 리스트를 사용하는 가장 좋은 방법에 대해서는 바로 아래 다
       음에 나오는 문서를 먼저 읽어 보기 바란다．

          리눅스 커널 메일링 리스트 FAQ
          www. tux. org/lkrnl


          다양한 리눅스 커널 관련 메일링 리스트 목 륵을 제공하는 사이트
          http: //vger.kerne1. org


          리눅스 커널 메일링 리스트 e 내용이 아주2) 많음, 커널 개발 전용
          http: //vger.kernel. org/vger-lists.html#linux-kernel



리눅스 뉴스 및 개발 정보
       들러 볼 만한 유용한 사이트가 많은데, 그 중에서 인기 있는 일부는 다음과 같다．

          LinuxDevices. corn
          www. linuxdevices. corn


          Powerl毛 관련 뉴스 및 기타 정보
          http: //penguinppc. org


          일반적인 리눅스 뉴스 및 개발 관련 소식
          www.iwn.net



오픈 소스에 대한 이해 및 토론

       다음 웹 사이트는 오픈 소스에 대한 법적인 문제에 초점을 맞춘 유용한 정보들을 가지고 있다．

          www. open-bar. org




2) ［역자주） 하루에 a)0 3m개 정도의 메시지를 받게 된다. 주의하기 바린r+.
Ap口endix   F

    예제 BDI- 2000 구성 파일
Embedded Linux Primer



; bdiGDB configuration file for the UEI PPC 5200 Board
; Revision 1.0
; Revision 1.1 (Added serial port setup)

 ', 4 MB Flash(Am29DL323)
; 128 MB Micron DDR DRAM


u1NIT]
; mnit core register
WREG        MSR          0x00003002       ;MSR      : FP, ME, RI
WM32        0x80000000 0x00008000         ;MBAR : internal registers at 0x80000000
                      ·, Default after RESET, MBAR sits at 0x80000000
                      ; because it 's POR value is 0x0000_8000(! )


WSPR        311           0x80000000      ; MBAR : save internal register offset
                                           ', SPR311 is the MBAR in G2_LE


WSPR       279          0x80000000         ;SPRG7: save internal memory offsetReg: 279


     mnit CDM(Clock Distribution Module)
     Hardware Reset config {
          ppc_pll_cfg[0. .4] = ol000b
          XLB: Core -> 1: 3
          Core: f (VCO) -> 1: 2
          XLB: f (VCO) -> 1: 6


          xlb_c卄_sel = 0 -> XLB_CLK=f (sys) / 4 = 132 MHz


          sys나키］_cfg그 = 0 尸＞ NOP
          sys_pll_cfg_0 = 0 -> f (sys) = 16x SYS_XTAL_IN = 528 MHz
      }

 ;   CDM conflguration Register
 WM32       0x8000020c 0x01000101
                  ; enable DOR 卜巾）de
                  ; ipb_c卄＝sel = 1 -> XLB_CLK / 2(ipb_c卄； = 66 MHz)
                  ; pci_c卄；나sel = 01 -> IPB_CLK/2
                                                   예제 B［긔-2000 구성 파일     Appenc琡 F



,1 CSO Flash
帥432     0x80000004 0x0000ff00 ;csO start = 0xff000000 - Flash memory is on
cSO
帥i32     0x80000008 0x0000ffff ; CSO stop = Oxffffffff


; IPBI Register and 닙ait State Enable
WM32     0x80000054 0x00050001 ;CSE: enable CSO, disable CSBOOT,
                              ;wait state enable\
                              ; cs2 also enabled


WM32     0x80000300 0x00045d30 ;BOOT ctrl
               ·, bits 0- 7: waitP (try Oxff)
               ; bits 8-15: WaitX (try 0xff)
                bit 16: Multiplex or non-mux 'ed(OxO = non-muxed)
                 벼
                  t 17: reserved(Reset value = Dxl, keep it)
                bit 18: Ack Active(0x0)
                bit 19: CE(Enable) Oxi
                bits 20-21: Address Size(0xll = 25/6 bits)
                bits 22: 23: Data size field(OxOl = 16-bits)
                bits 24: 25: Bank bits (0x00)
                bits 26-27: WaitType(Oxll)
                L너ts 28: 닙rite Swap (oxO = no s叫ap)
                bits 29: Read 鈿ap(oxo = no swap)
                bit 30: write only (oxo = read enable)
                bit 31: Read only(Oxo = write enable)

; CS2 Logic Registers
WM32     0x80000014 0x0000e00e
WM32     0x80000018 0x0000efff


 LEDS:
  LED1 - t너 ts 아7
  LED2 - bits 8-15
  LED3 - bits 16- 23
  LED4 - bits 24- 31
  off = OxOl
  on = 0x02
 mm 0xe00e2030 0x02020202 1(all on)
   轉U   Embedded Linux Primer



        ; mm 0xe00e2030 0x01020102 1(2 on, 2 off)
        WM32      0x80000308 0x00045b30        ; CS2 Configuration Register
                                         ; bits 0- 7: waitP (try 0xff)
                                         ; bits 8-15: waitx (try Oxff)
                                         ; bit 16: Multiplex or non-mux 'ed(OxO =
        non-muxed)
                                             bit 17: reserved(Reset value = 0xl, keep it)
                                             bit 18: Ack Active(0x0)
                                             bit 19: CE(Enable) 0xl
                                             bits 20-21: Address 引ze(Oxl0 = 24 bits)
                                             t너ts 22: 23 : Data 引ze field(0xll = 32寸너ts)
                                             bits 24: 25: Bank bits (0x00)
                                             bits 26-27: WaitType(0xll)
                                             bits 28: write Swap(oxo = no swap)
                                             bits 29: Read Swap(oxo = no swap)
                                             bit 30: write only(oxo = read enable)
                                             bit 31: Read only (oxo = write enable)

        WM32 0x80000318 0x01000000             ·, Master LPC Enable



         ·, m nit SDRAM controller



        !   For the UEI PPC 5200 Board,
             Micron 46v32M16- 75E(8 MEG x 16 x 4 banks)
             64 MB per Chip, for a total of 128 MB
        ;    arranged as a single "space" (i. e 1 Cs)
             with the following configuration:
                8 Mb x 16 x 4 banks
                Refresh count 8K
                Row addressing: 8K (AO. .12) 13 bits
                Column addressing: 1K (AO. .9) 10 bits
                Bank Addressing: 4 (BAO. .1) 2 bits
        ;    Key Timing Parameters: (- 75E)
                    Clockrate(CL=2) 133 MHZ
                    DO window 2. 5 ns
                    Access window: +/- 75 ns
        ;           DQS - DQ skew: +0. 5 ns
        ;           t (REFI) : 7. 8 us MAX


I 610
                                                  예제 B미-2000 구성 파일      Appern奴 F




    Initialization Requi rements (General Notes)
     The memory Mode/Extended Mode registers must be
     initialized during the system boot sequence. But before
     writing to the controller Mode register, the mode_en and
    cke bits in the control register must be set to 1. After
    memory initialization is complete, the control register
    mode_en bit should be cleared to prevent subsequent access
    to the controller Mode register.

; SDRAM mnit sequence
; 1) Setup and enable chip selects
;   2) Setup config registers
;   3) Setup TAP Delay


; Setup and enable SDRAM CS
WM32     0x80000034 0x0000001a      ;SDRAM CSO, 128MB @ Ox00000000
WM32     0x80000038 0x08000000      ;SDRAM CS1, disabled @ 0x08000000


WM32     0x80000108 0x73722930 ;SDRAM Config 1 Samsung
                         ; Assume CL=2
                      ; bits 0- 3: srd2rwp: in clocks (0x6)
                         ; bits 507: swt2rwp: in clocks -> Data sheet suggests
                      ,     0x3 for DDR (0x3)
                      ; bits 8-11: rd_latency -> for DDR 0x7
                      ; L너ts 13-15: act2r넥 m> 0x2
                      ; bit 16: reserved
                      ; bits 17-19: pre2act 山> 0x02
                      ; bits 20- 23: ref2act -> 0x09
                      ; bits 25-27: wr_latency -> for DDR 0x03
                      ·. bits 28- 31: Reserved


WM32     0x8000010c 0x46770000 ;SDRAM Config 2 Samsung

                          ; bits 0- 3: brd2rp -> for DDR 0x4
                                ,1 bits 4-7: bwt2rwp -> for DDR 0x6
                                ·, bits 8-11: brd2wt -> 0x6
                                ·, bits 12-15: burst_length 尸> 0x07(bl - 1)
                                ; bits 16-13: Reserved
        U   Embedded Linux Primer



            ; Setup initial Tap delay
            WM32 0x80000204 0x18000000        ; start in the end of the range(24 = 0x18)
            samsung


            WM32      0x80000104 0xf10f0f00 ;SDRAM Control (was 0xd14f0000)
                                         ; bit 0: mode_en(1=write)
                                         ; bit 1: Cke (MEM中CLK叫．EN)
                                         ; bit 2: ddr (DDR mode on)
                                         ; bit 3: ref_en(Refresh enable)
                                         ; t너ts 午6: Reserved
                                         ; bit 7: hi_addr (XLA[4: 7] as row/col
                                         ; must be set to '1' 'cuz we need 13 RA bits
                                         ; for the Micron chip above
                                         ; bit 8: reserved
                                         ; bit 9: drive_rule - OxO
                                         ; bit 10-15: ref_interval, see UM OxOf
                                         ·, bits 16-19: reserved
                                          ; bits 20- 23: dgs_oe[ 3: 0] (not sure)
                                         ; but I think this is req 'd for DDR 0xf
                                          ,· t너ts 24-28: Resv뇌
                                         ; bit 29: 1 = soft refresh
                                         ; bit 30 1 = soft_precharge
                                         : bit 31: reserved

            WM32      0x80000104 0xf10f0f02 ;SDRAM control: precharge all
            WM32      0x80000104 0xf10f0f04 ;SDRAM control: refresh
            WM32      0x80000104 0xf10f0f04 ;SDRAM Control: refresh


            WM32      0x80000100 0x018d0000 ; SDRAM Mode Samsung
                                      ; bits 0-1: MEM_MBA - selects std or extended MODE
            reg OxO
                                        bits 2-13: MEM_MA (see DDR DRAM Data sheet)
                                        bits 2- 7: Operating Mode -> OxO = normal
                                        bits 8-10: CAS Latency (CL) -> Set to CL=2    for
            DDR(Ox2)
                                        bit 11: Burst Type: sequential for PMC5200 ->
            OxO
                                        bits 12-14: Set to 8 for MPCS200 -> 0x3



I 612
                                                      예제 B미쿄000 구성 파일       Appendix F



                               ; bit 15: cmd = 1 for MODE REG WRITE


WM32    0x80000104 0x710f0f00 ;SDRAM Control : Lock Mode Register (was
Ox5 14f 0000)

; 如""出’"ki'肯出山' "" "" Initialize the serial port "' 卉士央央山“"
                                                        "六央 ‘"央
; Pin Configuration
WM32   0x80000b00      0x00008004     ; UART1


; Reset PSC
WM8    0x80002008      0x10          ; Reset - Select MR1


WM16   0x80002004      0             ; Clock select Register - 0 enables both RX &
TX Clocks
WM32 0x80002040        0             ; SICR - hART Mode
WM8    0x80002000      0x13          ; Write MR1(default after reset)
                                  ; 8七卄， no 口arity
WM8    0x80002000      0x07          ; write MR2 (after MR1) (one stop bit)


WM8    0x80002018      0xO           ; Counter/Timer Upper Reg (115. 2K8)
WM8    0x8000201c      0x12          ; Counter/Timer Lower Reg(divider = 18)


; Reset and enable serial port RX/TX
WM8    0x80002008      0x20
wM8    0x80002008      0x30
WM8    0x80002008      0x0 5



., define maximal transfer size
TSZ4    0x80000000 0x80003FFF         ;internal registers


; define the valid memory map
MMAP    Ox00000000 0X07FFFFFF         ;Memory range for SDRAM
MMAP    0x FF000000 OXFFFFFFFF        ;ROM space
MMAP     0xE00E0000 OXEOOEFFFF        ; PowerPC Logic
MMAP    0x80000000 0x8fffffff         ,1 Default MBAR
MMAP     0xC0000000 OXCFFFFFFF        ; Linux Kernal



                                                                                 613
   難1   Embedded Linux Primer



        [TARGET]
        CPUTYPE        5200         ;the Cpu type
        JTAGCLOCK       0           ;use 16 MHz JTAG clock
        WORKSPACE       0x80008000 ;workspace for fast download
        WAKEUP         1000       ;give reset time to complete
        STARTUP        RESET
        MEMDELAY       2000         ;additional memory access delay
        BOOTADDR       0xfff00100
        REGLIST        ALL
        BREAKMODE       SOFT    ; or HARD
        POWERUP        1000
        WAKEUP         500
        MMU           XLAT
        PTBASE         0x000000f0


        [HoST]
        iP            192.168.1. 9
        FORMAT         ELF
        LOAD          MANUAL       ;load code MANUAL or AUTO after reset
        PR아肝玎          uei>


        [FLASH]
        CHIPTYPE       AM29BX16        ;Flash type (AM29F 1 AM29BX8 1 AM29BX16 I I28Bx8 I
        I28Bx16)
        CHIPSIZE      0x00400000       ;The size of one flash chip in bytes
        BUSWIDTH  16                   ;The width of the flash memory bus in bits(8 1 16 I 32)
        WORKSPACE Ox80008000            ;workspace in internal SRAM
        FILE          u-boot.bin
        FORMAT         BIN OxFFF00000
        ERASE          0xFFF00000      ;erase a sector of flash
        ERASE          OxFFF10000      ;erase a sector of flash
        ERASE          0xFFF20000      ;erase a sector of flash
        ERASE          OxFFF30000      ;erase a sector of flash
        ERASE          OxFFF40000      ;erase a sector of flash


        [REGS]
        FILE           $reg5200. def



甘 614
莉nclude / 366           ATCA / 52, 105
%CPU / 407              AMCC / 55, 439
%MEM / 407              apache / 75
.comment / 492          AMD / 98
.data / 420             arch_install / 173
.debug_info / 422       AltiVec / 83
.gdbinit / 454          ARM / 100
.incbin / 153           autoconf. h / 130
.journal / 289          AppleTalk / 91
.resetvec / 219         addr2line / 426. 449
.rodata / 420
.sbss / 420
.sdata / 420
.text / 420             Backtrace / 388
/etc/exports / 298      BDI-2000 / 473
/etc/inittab / 194      bd_info / 530
/etc/rc.d / 196         bin / 186
/proc / 303, 357        binutils / 419
/sbin/init / 179, 192   BIOS / 51
440EP / 87              bi_record / 530
855GM / 84              BKL(Big Kernel Lock) / 547
970FX / 80, 81          Bootloader / 51
  defconfig / 134       bootm / 57, 205
   initdata / 171       BOOTP / 225, 302, 372
_setup / 166            break / 391
                        breakpoint / 442
                        busybox / 75, 187
        芬   찾아보기




 C                                     cramfs / 295
                                       cscope / 395
C 표준 라이브러리 / 69                        customize_machine / 178
cacheable / 235
CAS 지연 시간 / 600
cbrowser / 395
CF 카드 / 60                             DDR SDRAM 컨트롤러 / 87
CFG_CMD_DHCP / 224                     DEFII旺：SPII寸LOCK / 556
CFG_CMD_EXT2 / 224                     depmod / 266
CFG_CMD_FLASH / 224                    dev / 186
CFG_CMD_MEMORY / 224                   device node / 188
CFG_CMD_PING / 224                     devname / 306
CFG兀伏 / 224                            DHCP / 225, 372
CFI / 327                              DHCPACK / 373
CGL / 46                               DHCPDISCOVER / 373
client-ip / 302                        DHCPOFFER / 373
command line / 127                     DHCPREQUEST / 373
CompactPCl / 105                       diskboot / 229
config.mk / 230                        dmalloc / 412
CONFIG_CMDLINE / 522                   DRAM 컨트롤러 / 216
CONFIG_DEBUG_PREEMPT / 557             Dwarf2 / 423. 449
CONFIG_MTD_BLOCK / 319
CONFIG_MTD_CFI / 327
CONFIG_MTD_CHAR / 319                 磁塑



CONFIG_MTD_CMDLINE_PARTS / 331         e2fsck / 286
CONFIG_MTD_MTDRAM / 319                EOF / 276
CONFIG_MTD_REDBOOT_PARTS / 328         erase block / 61
CONFIG_POWERDNA / 536                  etc / 186
CONFIG_PREEMPT_RCU / 553               execve / 179, 191
CONFIG_SERIAL_TEXT_DEBUG / 481, 518    ext2 / 283
CONFIG_WAKEUP_LATENCY_HIST / 558       ext3 / 288
CONFIG_WAKEUP_TIMING / 557, 558        EXTRAVERSION / 113
CONFIG_X妖 / 224                        ext_bus cntlr_init / 236
connect / 455
console_setup / 166
continue / 391
                                                         崙藤烈彌毖融h瑟誌高芯念如蚣澔弓無諦蘇m




core / 387                             fdisk / 281
（兀TS / 52                              Fedora / 74
Cr）如 / 209                             FHS / 185
cpp / 367                              filename / 227
cpuinfo / 306                          find_task / 457
cpu_idle / 176                         FIS / 326



I 616
                                                                찾아보기



0s list / 328
fixed-address / 227
flashcp / 337                          i shared / 499
flash_erase / 337                      i.MX21 / 102
flash_info / 337                       i.MX31 / 102
flash_lock / 337                       IBM / 80
flash_unlock / 337                     IDE 컨트롤러 인터페이스 / 228
fork / 402. 502                        m1lit / 59
format / 283                           m1lit 스크립트 / 148
FPU / 89                               initramfs / 209
frame / 389                            INITRAMFS_SOURCE / 210
free / 307                             initrd / 201
fsck / 210                             inittab / 193. 353. 355
                                       inline / 435
                                   呼   mllode / 283
                                       insmod / 262
FAT32 / 281                            INTERRUPTJJFFHIST / 559
G4 / 82                                ioctl / 269
gcc / 76                               IrDA / 91
gconf / 137                            ISR / 70
GDB / 384
gdb 스텁 / 436
gdbserver / 493
GLIBC / 188                            JEDEC / 334
glibc / 75                             JFFS2 / 66. 292, 293
GNU 디버거 / 384                          JTAG / 473
gnuplot / 292, 560                     JTAG 디버거 / 436
GPL(General Public License) / 43
GPS / 541                                                                 芝
GRUB / 244
grub.conf / 245                        KALLSYSMS / 417
gzip / 152                             Kbuild / 125
                                       KConfig / 124
                                       Kernel command line / 148, 155
                                       kernel context / 59
halt / 211                             KERNELBASE / 527
hardware ethernet / 227                KERNELRELEASE / 113
host / 227                             kernel thread / 176
hostname / 302                         KERN_DEBUG / 471
h毗巾lug / 309                           KERN_WARNING / 471
                                       KGDB / 435




                                                                        6口 I
 g酵us      찾아보기



 klimit / 529            modprobe / 265
 ksoftirqd / 551         modules.dep / 267
                         modules_install / 260
                         module exit / 261
                         module mllit / 261
 LATENCY_TRACE / 561     module_param / 172
 ldconfig / 399          MODULE_PARM_DESC / 268
 ldd / 193. 349, 427     mount / 206, 284
 LED / 51                MPC5200 / 474
 lib / 186               MPC74xx / 80
 Lilo / 243              MPC8540 / 516
 linker script / 120     MTD / 318
 LinuxBIOS / 246         MTD 유틸리티 / 336
 linuxrc / 205           mtdblock / 322
 list / 388              mtddef / 331
 logger / 63             mtdparts / 331
 LSB / 45                mtdram / 322
 ismod / 264             mtrace / 410
 itrace / 404            myinit / 180

                                                  照凞器瑟毋照婢姓怒




 machine_m1lit / 520     NAND 플래시 / 63
 main.c / 162            ncurses / 347
 make help / 131         netmask / 227
 make mrproper / 125     NFS 서버 / 59. 376
 makefile / 116          nice / 409
 mapping driver / 326    nm / 428
 maps / 305              NOR / 63
 meminfo / 306           north bridge / 84
 MIL / 47                nVid治 / 85
 minicom / 472
 MIPS / 86, 95
                         0:
                          ：二二二之二二二二玉二二
 mkcramfs / 296
 mke2fs / 283, 312       O(1) 스케줄러 / 553
 mkfs.jffs2 / 294, 341   objcopy / 152, 425
 mkimage / 241           obj dump / 424
 mknod / 273             obsolete_ / 171
 MMU / 67                obs_kernel_param / 171
 mobprobe.conf / 265     Oops / 416
 modinfo / 263, 268      open / 269
 modprobe -r / 261       OSDL / 46



I 618
                                                         찾아보71   難 a.




panic / 191                   RAID 5/6 / 89
patchkernel.sh / 321          ramfs / 310
PBX / 93                      RapidlO / 94
Pentium / 80                  rc.sysinit / 200
pgoffset / 306                rcS / 355, 357
physmap_configure / 333       RCU / 553
physmap_setpartitions / 334   readeif / 419, 449, 491
PICMG / 105                   reboot / 211
pkill / 307                   Redboot / 246, 324
platforms / 516               Reiser4 / 291
platform_mlit / 524. 532      ReiserFS / 291
PLL 클럭 / 223                  release / 269
pmap / 307                    rest_mllit / 176
pos奴 / 368                    RISC / 86
PowerDNA / 534                rmmod / 267
PowerPC / 73, 80              ROM / 83
PowerQUICC / 90               rpm / 74, 190
PowerQUICC II / 92            RSS / 408
PPC405 / 516                  RTC / 52
preemptable / 543             run-time library / 216
PREEMPT_DESKTOP / 549
PREEMPT NONE / 549
                                                          韜茹旨
PREEMPT_RT / 549, 550
PREEMPT_VOLUNTARY / 549       SA Forum / 48
prelink / 429                 SAN / 104
print / 388                   sbin / 186
printk / 470                  scalability / 42
proc 파일 시스템 / 184. 303        SCC / 91
procps / 307                  SCHED_FIFO / 554
PROM / 239                    SCHED_OTHER / 554
Ps / 405                      SCHED_RR / 554
pthread_create / 506          sched_setscheduler / 554
                              SD/MMC / 103
                              SDRAM / 52, 592
                              SDRAM 리프레시 / 593
QA / 412                      sdram_init / 239
                              server-ip / 302




                                                                  6四 I
  1n      찾아보기



server-name / 227                  top / 408
setuid / 359                       TTY / 408
show solib-absolute-prefix / 500   tune2fs / 289
shutdown / 211
SiByte / 96
町GKILL / 211
SIGSEGV / 385                      U-Boot / 56, 379
SIGTERM 시그널 / 211                  UART / 53
SMBus / 97                         ulmage / 241
SMP 커널 / 547                       ulimit / 385
Soc / 86                           uname / 260
socket / 400                       uptime / 307
softlRQ / 542, 551                 USB / 53
southbridge / 84                   usr / 186
Sparc / 104
SPD / 239
SF1 / 87
spinlock / 547                     var / 186
start_kernel / 157, 163            version / 306
strace / 397                       VIA / 85
strings / 427                      VMEbus / 105
strip / 426, 492                   vmend / 306
superscalar / 81                   vmlinux / 116
sysfs / 280, 307                   vmstart / 306
system call / 68                   VSZ / 407
System.map / 116
systool / 308

                                   xinetd / 197, 357, 371

tar / 320                                         辯好凞碍凞發剪螂出窄凞解茹丹唯

                                                  磁妊難難磊難慰無磁弊瀜融融多

target / 391
target remote / 440, 494           YAMON / 246
task_struct / 457
taskmstruct_show / 460             z
telnet / 357
TFTP / 225, 371                    zlmage / 118
TFTP 프 ！토콜 / 57
tftpboot / 57. 204                 기
tmp / 186
tmpfs / 311                        가민（G카mmn) / 103
toolchairi / 72                    가상 메모리 / 68
                                                                                  찾아보기



  가상 메모리 공간 / 60                          데이터 크런칭 / 83
  가상 메모리 주소 / 71                          데이터 표시 디버거（DDD) / 392
  가용 메모리 풀 / 206                          독립형（Stan卜al이祀） 프로세서 / 80
  강건성 / 111                               동시성（concurrency) / 547
  개발 툴 / 72                               동작 레벨 스크립트 / 195
  경쟁 조건 / 412                             동작 레벨（runi四이） / 194
  고성능 / 111                               동적 임의 접근 메모리 / 592
  고속 전반부 버스 / 84                          동적 컨텍스트 / 68
  곱합 / 83                                 디바이스 노드 / 188
  공공 라이선스 / 276                           디바이스 드라이버 / 252
  공용 플래시 인터폐이스 / 327                      디바이스 드라이버 모델 / 161
  교차 디버거 / 495                            디버깅 심벌 / 151
  교차 컴파일러 / 74
  교차尸개발 환경 / 72. 364                    寸Jm 芬甘Hm食甘好m甘烈抑쐽畔q朴W"嶝4까哮乂

                                          B
                                                                     卞口   目mm柳下mm好버甘n1斗姓mm心川텍 月甘m蚣가哨싸m叩二m냥茹伊旺月具甘




  교차합 / 83
  구글 / 111                                라이브러리 / 45. 367
  구글링（Go아gling) / 143                     램디스크 / 64
  구성 옵션 / 222                             랩톱 / 82
  구성 유틸리티 / 85                            런 타임 라이브러리 / 216
  그룹 ID / 297                             레드붓 / 159
  기준 소스 / 112                             레드햇（Redi拓t) 패키지 매니저 / 74
  기준 커널 / 112                             로드 가능한 모듈 / 253
  깨어나는 시간 / 557                           루트 파일 시스템 / 59, 184
                                          루프백 / 311, 357
쏘少" 岫螂畔枷加四艸"m四'小「m心m'呼艸m"蜘啣汕的小啼耐和'螂斟卿     리누스 토발즈 / 110
                                          리눅스 기본 규격 / 45
  낮은 지연성 / 81                             리눅스 문서화 프로젝트 / 142
  내부 지식 / 277                             리눅스 스왑 파티션 / 281
  네트워크 처리 엔진 / 104                        리비전 / 56
  네트워크 파일 시스템 / 298                       리얼 타임 / 540
  노스 브리지 / 84                             리얼 타임 커널 패치 / 548
  니모닉（mnemonic) / 451                     리치 레바움 / 43
                                          리프레시 명령 / 601
  C                                       링커 기술 파일 / 218
코恥a뇨斗小考 尸" 노寸   "

                                          링커 명령에 스크립트 / 218
  다스 유 부 i (Das U-Boot) / 221             링커 스크립트 / 120
  다음 명령에 포인트（NIP) / 462                   링커 스크립트 파일 / 166
  다중m부트（dual寸boot) / 243
  대기 상태 / 70
                                                                                                              毒盈
  대기 큐 / 69
  데드라인 / 540                              마벨 / 85
  데드락 / 563                               마운트 / 59



                                                                                                       621 甘
難 ma    찾아보기



마운트 지점 / 207              부동 소수점 연산 장치 / 89
마이크로 코딩 / 104             부트로더 / 51. 214
마이크로모니터 / 246             부트스트랩 로더 / 153
매직 SysReq 키 / 471         브레이크 포인트 / 390
매핑 드라이버 / 326. 331        브로드캐스트 패킷 / 226
맨 페이지（man page) / 197     브로드컴 / 96
멀티 쓰레딩 / 116              블래이드 / 81
메모리 관리 장치 / 67            블록 다이어그램 / 87
메모리 기술 저장 장치 / 318        블록 디바이스 / 254
메모리 맵 / 67                비휘발성 메모리 / 65
메모리 뱅크 / 238              빅 커널 락 / 547
메모리 서브시스템 / 51            박엔디언 / 341
메모리 스냅 샷 / 386            빌드 번호 / 158
명령에 cache / 238
명령에 라인 / 127              羅艾雖解吐삐呻的飼姆蜘
명령에 스트림 / 81
명령에 캐시 / 63               사용자 영역 컨텍스트 / 68
모놀리식 / 119. 126           사용자 영역（user space) / 163
모놀리식 커널 / 253             사용자 훅 / 173
모듈 / 254                  사우스 브리지 / 84
모바일 리눅스 이니셔티브 / 47        삭제 단위 블록 / 61
모토롤라 / 86                 삼성 전자 / 104
몬타 비스타 / 189              서비스 가용성 포럼 / 48
무 정지성 / 111               선점 가능 / 543
무조건 분기 / 219              선점 디버깅 / 557
문맥전환 / 69, 121            선점 모델 / 545
물리 주소 / 527               선점（preemption) / 116
뮤텍스 / 550                 세그먼테이션 폴트 / 386
미니컴（M油corn) / 54          섹션 속성 / 168
미들웨어에 / 106               섹터 크기 / 62
                          소스포지 / 221
                          소프트 락업 / 556
                          소프트 리얼 타임 / 540
배쉬（Bash) / 359            수세（SuSE) / 291
배포를 위한 기술 / 189           수정판（der加ed work) / 44. 276
뱅크 설정 레지스터 / 598          슈퍼블록 / 312
뱅크 주소 / 599               슈퍼스칼라 / 81
뱅크 활성화 / 599              스냅샷 / 320
버스트 읽기 / 593              스와핑 / 70
보조 버전 / 112               스왑 / 72
보조 칩셋 / 83                스케줄링 / 541
보텀 하프（bo比아n half) / 542   스타트업 스크립트 / 253
                                                                               찾아보기     難 熬1



 스택 / 217                                             열（row) 주소 / 592
 스택 포인터 / 217                                         예외 처리 / 121
 스택 프레임 / 388                                         오픈 소스 / 43
 스텁 / 124                                             오픈 소스 개발 연구소（OSDL) / 46
 스핀락（spinlock) / 547. 550                             옵티마이저 도구 / 188
 슬랩 할당자（slab allocator) / 537                         외부 버스 컨트롤러 / 233
 슬립 모드（sleep mode) / 408                              요세미티 / 55. 70
 시그널 / 385                                            원격 디버깅 / 490
 시리얼 통신 컨트롤러 / 91                                     원자성 / 291
 시리얼 포트 / 51. 365                                     웨어 레벨링（wear-leveling) / 65, 294
 시분할 멀티플렉서 / 91                                       위상 동기 루프 / 594
 시스템 V m it / 194                                     유로카드（Eurocard) / 105
 시스템 로거 / 63                                          유저 영역 / 60
 시스템 종료 / 198                                         의사 파일 시스템 / 303
 시스템 콜 / 60. 68                                       인터넷 슈퍼서버 / 201
 시스템 클럭 / 220                                         인터럽트 서비스 루틴 / 70
 시작점（starting point) / 233                            인터럽트 차단 시간 / 558
 시장 적기 진입 / 106                                       인터럽트 차단 시간 기록 / 559
 신뢰성 / 111                                            인텔［ / 80
 실린더 / 282                                            임베디드 리눅스 / 42
 실행 콘텍스트 / 220
 심볼릭 링크 / 347
 썬（Sun) / 104
 쓰레드 / 68                                             자동 구성（autoconfi恥ration) / 378
 쓰레드 모델 / 368                                         자체 개발 / 364
                                                      자체（native) 컴파일 / 72
轉發畔多斛發i也 m發斜蜘羽瞬日辨渽朴多際凞驛必客資特耀硼照袋斟烈硼蝴饌解驪埠拉蜀器搏蜀熙解晷解硼"
 V                                                    저널링 / 288
                             珏蹄崙派帥曲 唯瑟a區出立磻瑟發驀硅蜘凞枷누
                                                      저널링 플래시 파일 시스템 2 / 66
 아바트론 / 473                                           저전력 모드 / 81
 아이파드(iPod) / 100                                     적재 가능한 모듈 / 127
 아파치 / 189                                            전처리기 / 169
 알테라 / 104                                            잠config / 116
 암호화 프 ！토콜 / 83                                       정지 응답 / 439
 애플릿 / 359                                            젠투（Gentoo) / 291
 앤드류 모튼 / 112                                         종료（計iutdown) / 210
 앨커미 / 98                                             주 버전 / 112
 어드레스 핀 / 161                                         주소 공간 / 66
 언마운트（unmount) / 211                                  주소 라인 / 66
 에릭 레이몬드 / 44                                         주소 방식 / 599
 에뮬레이트 / 65                                           증분 링크（ir乂rementally link) / 126
 卜髓 1   찾아보기



지역화 파일 / 189
지연 시간 기록 / 558
지연 시간 추적 / 561                                    타깃 / 364
직렬 버스트 / 63                                       통신망용 리눅스 / 46
직렬 보조 장치 인터페이스 / 87                               통합형 프로세서 / 80
질레온（Xilleon) / 99                                 툰드라 / 85
                                                  툴 체인 / 45. 72
        辯器虹邪目客嚼三娜＝娜斟照凞提斟凞附무批m多懈我礪斛好四d牡雖鉀鉀附幽黨懈骨三   트랜지스터 / 593
        爀聯搬凝親轟融曳幽臨幽二磁竝枷竝嫡系希礪杯魚瀜烈挺融耐쿄羽耐的蜘鈿小呻娜蜘師




체크썸（check田urn) / 153
초기 램디스크 / 185, 201, 527
최상위（top-i四이） 소스 디렉터리 / 115                        파이프라이닝 단계 / 81
최소 디바이스 드라이버 / 254                                파이프라인 / 81
최적화 단계 / 350                                      파일 기술자（descr毗or) / 274, 400
칩셋 / 80                                           파일 시스템 / 280
                                                  파일 시스템 계층 표준 / 185, 273
                                                  파티션 / 281
                                                  패닉 / 179
캐리어 급 / 106                                       패치 / 114
캐릭터 디바이스 / 254                                    패키지 / 74
커널 / 60                                           페도라伊edora) 코어 / 74
커널 명령에 라인 / 148                                   페이지 폴트 핸들러 / 161
커널 버전 / 157                                       페이징 / 70
커널 본체 / 148                                       포직스 / 368
커널 선점 / 543                                       포팅 / 240. 514
커널 심볼 / 68                                        표준 하드웨어 플랫폼 / 80
커널 심볼 테이블 / 68                                    프로그램 카운터 / 160
커널 오브젝트 / 255                                     프로세스 ID / 175
커널 웁스 / 416                                       프로세스 컨텍스트 / 70
커널 자체 / 124                                       프로토타입 / 366
커널 커맨드 라인 / 155                                   프로파일링 / 396
커널 컨텍스트 / 59. 68                                  프론트U엔드 / 128
커널 패닉 / 485                                       프리스케일 / 80
커패시터 / 593                                        프리페치 / 238
컴퓨팅 파워 / 494                                      플래그 / 170
코어 덤프 / 385                                       플래시 메모리 / 61
코요테 / 117                                         플래시 파일 시스템 / 65
크리티컬 섹션 / 548
클럭 / 594




p624
                    찾아보기




舌

하드 리얼 타임 / 541
하드 링크 / 66
하드 코드 / 165
莎플러그 / 309
행（C이umn) 주소 / 592
현재 쓰레드 / 507
호스트 / 364
호스트 개발 환경 / 73
홀드 시간 / 234
확장성 / 42
후크 / 437




                           625弦
                                                                                   죠的烈斗再n mnm心我m




 오픈소스 1
                                                                                                                        們珥小r싸gi 겯궁囊


개발자睾 자극하는 실무적인 안내서




     難多
                                하루 10분씩 핵심만 골라 마스터하는 시ax 핸드북
                                      ) 우선 AJAX를 구성하는 핵심 웹 기술들을 간단히 살펴본 후, 웹 서비스를 만드는 등의 좀 더
                                        복잡하고 독자적인 AJAX 어플리케이션을 만드는 방법을 배울 수 있으며, AJAX를 이용하여
     마스터하는1H
                                        개발할 때 발생하는 문제점들을 해결하;71 위한 간단한 지침서로도 활용할 수 있습니다．
                                        Phil Ballard 저 1 강덕진 역 I 272쪽 1 12,000원
 1

                                성공적인 웹 프로그래밍 : PHP와 MySQL 제3판
                                     ,) 현실에 바로 적용할 수 있을 만큼 실질적인 예제를 가지고 일반적으로 많이 사용되는 사용
                                        자 인증, 장바구니 구현, PDF 문서 만들기, 다이나믹한 이미지 처리, 이메일 전송과 관리，
                                        토론방 만들기, 컨텐츠 관리와 XML을 사용한 웹 서비스까지 다루고 있어 정말 다양한 내용
                                        을 배울 수 있다．
                                        Luke Welling, Laura Thomson 공저 1 류정욱, 김소회 공역 I 993쪽 I 30,000원




                                                                    UN以                  UN以 마스터링 핵심 노트
                         예제로 쉽게 배우는 씨ax                             마스터링                 Ito Kazuh的 저 1 임병균, 박주연 공역
                         JOSHUA 日OH아刑 저 1 한호연 역 1                                        20,000원
                         365쪽 1 18,000원


                                                                    m
 ODE Rer님ing                                                          서브버전 뮨 이용한
     모뷴스스 斗甘1시 g 코드 g기
                         Code Reading :                              쇠용적인 버전 관리          서브버전을 이용한


                                                                        心
                         오픈 소스 관점에서 본 코드 읽기                                              실용적인 버전 관리
                         Diomidis Spinellis 저 1 류광 역 1                                   Mike Mason 저 1 류광 역 1223쪽 1 13,000원
                         이0쪽 I 25,000원                                         A




                                                                  i；各
                         예제로 배우는                                                          XML 포켓 컨설턴트
                         리눅스 소켓 프로그래밍
                                                                                         William R. 얹anek 저 1 김종민, 김동정 공역
                         Warren W. Gay 저 1 배재현 역 1                                       507쪽 1 18,000원
                         588쪽 I 22,000원



 심무 몌싸로 m우는                                                                              ACE 프로그래머 가이드：네트워크 · 사스템
                         실무 예제로 배우는 Unix 쉘1 프로그래밍
    딥 프로그래밍
                                                                                         프로그래밍을 위한 실용적인 디자인 패턴
                         먀uce 테nn 저 1 빅同1련 역 I 330쪽 1 15,000원                            Stephen D. Hus幻n 외2 공저 1 권태인 역 1
                                                                                         559쪽 I 25.000원
 닷넷 · 모바일 프로그래밍 i

.NET과 모바일 프로그래밍에 대한 상세한 기술 정보와 통찰력을 제공하는 닷넷 · 모바일 전문 지침서




                .NET 3.5 차세대 개발 프로그래밍
                    注 이 책에서는 ＼기su줴 앉udio 2008과 닷넷 프레임워크 3.5에 대한 소7f, LINQ의 새로운 특
                      징, Windows Presentation Foundation, Windows Communication Foundation,
                      Windows Workf low Founda的n 등 .NET 3.5의 핵심적인 내용들을 일목요연하게 정리，
                      설명하고 있다．
                      손정민, 이충일, 정병찬 공저 I 857쪽 I 30,000원


                윈도우즈 임베디드 CE 프로그래밍 입문
                    .，多Windows M야케e / Windows Embedded CE의 용용 프로그램을 충실한 가이드를 통해
                       직접 실습하면서 익히는 실습 위주로 구성되어 있으며, 윈도우 구성, UI 출력, 그래픽, 파일，
                       RS-232C 통신, TCP/IP 통신 등 기본적인 모든 분야를 다루고 있다．
                      고재관, 임지영 공저 I 740쪽 I 23,000원




                                                                        .NET Micro Framework
          디버깅 ,NET 응용 프로그램1                                             임베디드 프로그래밍
          的hn Robbins 저 1 서우석 역 I 623쪽 I 25,000원                        Donald Thompson, R아） S. 卜川es 저 1 이건복
                                                                        375쪽 1 18,000원



          Introducing Microsoft ASP.NET                                 기초에서 활용까지
          AJAX                                                          윈도우즈 임베디드 CE 프로그래밍
          Dino Espos的 저 1 김도균 역 1442쪽 1 18,000원    m씨 1月n1
                                                   껸도무즈 m1J드 1工 프로그m밈
                                                                        고재관 저 1 이7쪽 I 23,000원



          Network Programming for                                       Programming Microsoft
          The 1네아osoft .NET 다amewo水                                     Windows CE .NET 3rd Edition
                                                   WINDOWS CE
          Anth아）y Jones 외2 공저 1 김남식 역 1 425쪽             .NET           Dou아as B이ing 저 1 노영선 역 1 1,4巧쪽 I 40,0004
          18,000원




          Programming Microsoft Windows                                 Programming Microsoft .NET
          Forms: C＃의 능률적인 활용                                            Jef[ 마osIse 저 1 김영환 역 1895쪽 I 35,000:
          Charles Petz이d 저 1 서우석 역 149樗 I 8,000원
모든 임베디드 개발자 및 엔지니어들을 위한 실용적인 안내서

이 책은 효율적이고 가치 있는 리눅스 기반 임베디드 제품을 만들기 위해서 꼭 필요한 지식들을 제시한다. 이 책의 저자인
크리스토퍼 할리난은 수년간 임베디드 리눅스 컨설턴트와 필드 어플리케이션 엔지니어（iAE）로 일한 경험을 통해서 얻은
지식을 바탕으로 임베디드 개발자가 주로 겪게 되는 기술적인 문제들에 대한 해결책을 제시해 주며」，효율적인 임베디드 개
발 환경을 갖추는 방법도 제시해1 준다. 또한 생산성을 높이기 위해서 쓸 만한 노하우도 알려준다．


일반적인 리눅스 기반 임베디드 시스템을 간단히 살펴보는 것에서 시작해서 시스템을 이루는 핵심 개념과 구성 요소들을
설명하고, 리눅스와기존의 임베디드 환경과의 차이점에 대해서 자세히 설명한다 ．그리고 임베디드 커널을 빌드시키는 것
에서부터 부트로더를 초기화하는 과정, 디바이스 드라이버에서 파일 시스템까지의 모든 내용을 개발자 관점에서 포괄적으
로 설명한다．


또한, 점점 더 많은 인기를 얻고 있는 BusyBox 유틸리티에 대해서도 자서恃］ 설명한다 ．그리고 리눅스를 자체 보드에 포팅
하는 과정어］ 대해서 한 단계씩 자세히 설명하고, 최신 임베디드 리눅스어써 가장 홍미로운 부분 중의 하나인 리얼 타임어］
대해서도 CONFIG_RT 구성을 통해 설명해 준다. 독자는 개발 툴 들 을 사용하는 방법과 커널을 디버깅 하는 내용을 포함한
임베디드 시스템을 분석하고 디버깅할 수 있는 방법도 배울 수 있다．


이 책에 포함된 내용
. 임베디드 리눅스0私I 주로 사용되는 프뢰私I들에 대한 비교
S 리눅스 커널의 초기화 과정
. 임베디드 리눅스 시스템에서 부트로더7F 갖는 특별한 역할（U-Boot 상서1 설명）
. 임베디드 리눅스에서 JFFS2률 포함한 파일 시스템의 사용. 플래시에 저장시킬 파일 시스템 이미지 생성 방법
. 푤래시 메모리 장치（또는 다른 장치）률 위한 메모리 기술 장치 서브시스템
1gdb, KGDB 그리고 하드웨어 JIAG룔 이용한 디버깅
. 리눅스 커널 내0私寸 사용할 만한 팁과 디버깅 기술
. 교차 개발 환경을 이용해서 생산성을 극대화시키는 방법
1TFTP, DHCP 그리고 NFS 서버를 포함해서 전체 개발 환경을 갖추는 방법
' 자신의 시스템의 요구조건어t 맞7카 BusyBox룔 구성하고 빌드 및 초기화하는 방법

저자에 관해

미국 몬타 비스타 소프트웨어 사의 필드 어플리케이션 엔지니어인 크리스토퍼 할리난은 20년 이상을 엔지니어에서 엔지니
어 관리, 마케팅에서 사업 개발에 이르는 다양한 분야어써 일한 경험을 가지고 있다. 또한 그는 4년간 독립적으로 임베디드
리눅스를 위한 개발 컨설턴트로 일해왔다. 그가 작업한 연구에 대해서는 전기통신 매거진（Tel吼아limunic餌이lS
入lagazine), 광섬유 매거진們比r Optics Magaz毗）, Aviation 다이제스트 등에서 볼 수 있다．



                                                                                    값 23,000원



                                                                                II fl
                                                                                               000




                           三量   정보문회사           尸 F긋 ENTICE      HALL      9 788956 744377
                                                F口 EAR日口 N   ED 니口ATI그 N     ISBN 978-89-5674 437 7

