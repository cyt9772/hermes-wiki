---
source_url: "/run/media/yutae/Data/Enterprise Programming with Java.pdf"
ingested: 2026-11-15
sha256: cbb6f0ef9ffc5b5c8fa5f693df2e999cc788fe760303ba106f7a83ecbd912342
type: raw-source
method: text-extract
---

# Enterprise Programming with Java (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/Enterprise Programming with Java.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 290쪽 | **추출 텍스트:** 331 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/enterprise-programming-java.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** Enterprise Programming with Java
- **Pages (PDF):** 290
- **Source:** Enterprise Programming with Java.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 290 pages)


===== PAGE 1 =====
Enterprise Programming with JAVA


===== PAGE 2 =====
Enterprise Programming with JAVA




                삼성SDS
                멀티캠퍼스


===== PAGE 4 =====
                                       모
                                       巾기
                                              차



               장 절절절절
                        소개
    !
l
                                                         3
         l
         l
                        소개                               5
         n
         乙
                        JDK 1. 1에서 JDK 1.2로의 Upgrade     6
         QU
                        JDK 1. 2에서 지원되는 명령              13
         月
         寸
                        Enterprise Application 모델       16

II 장 JDBC 프로그래밍                                        19




               절절절절 절
         4
         l
                        JDBC 개요                        21
         9
         口
                        java. sql 패키지                  33
         nd
                        Fundamental JDBC 프로그래밍         35
        d
        仕
                        Advanced JDBC 프로그래밍            61
        二
        U
                        데이터베이스 접근 모델                   77

m장          Network 프로그래밍                               79




              절절절절절절
        1 절 분산（Distributed) 시스템                         81
        9
        e
            녜트워크 프로그래밍 기초                               82
        Q
        U
            Java어］서의 소켓 프로그래밍                           89
        J
        4
            URL 프로그래밍                                   99
        二
        U
            네트워크 소스 분석（Chatti咽）                        111
        八
        b
            네트워크에서의 한글 및 다국어 처리                        122
m




              장절절절절절
                        RMI 프로그래밍                      125
                        개요                             127
        n
        乙
                        RJll 프로그래밍                     132
        QU
                        객체 직 렬화                        142
        4
        工
                        RMJ CallBack                   152
        二
        U
                        RMI 소스 분석                      159


===== PAGE 5 =====
                                        167
V 장 CORBA어］ 기초한 원격 객체 프로그래밍


      절절절
 l
 ]                                      169
    CORBA
                                        183
 口
 9
    CORBA 프로그래밍
 QU                                     198
    IDL 예제
                                        202
 4절 코바／자바에서의 한글 및 다국어 처리
                                        209
VI장 JavaBeans 프로그래밍
                                        211
 1절 J avaBeans의 개요
                                        256
 2절 Enterprise JavaBeans (EJB）에 대한 소개
                                        265
부           록




                         2


===== PAGE 6 =====
         I 장 소 개




           학 습 목 표

· JDK 1.2의 특징을 알게된다．
· JDK 1.2에서 지원되는 API의 종류에 대하여
 점검한다．




            -   3


===== PAGE 7 =====
m


===== PAGE 8 =====
]절 소 개


   1990년대 컴퓨터 분야의 큰 변화로 손꼽을 수 있는 것 중 하나는 Java
언어의 등장이라고 할 수 있을 만큼 짧은 시간동안 매우 빠르게 보급 되었다．


   1995년 5월 세상에 태어난 Java 언어는 객체1 지향을 기반으로한 플랫폼
독립성 , 뛰어난 보안 기능, 스레드 지원등의 언어적 지원과 함께 최신의 기술
들을 지원하고 있다．


  버그 개선, Java 인터프리터의 속도 향상, 개발 명령 추가, 구문 추가, 다
양한 API의 추가등 Java가 두 번 버전 업그레이드 되면서 변화된 내용들이다．
이중에서도 다양한 기능의 API 추가는 Java 언어가 기업（Enterprise) 환경에
서 활용될 수 있는 프로그래밍 언어가 될 가능성을 제시해 준다. 또한 \Web
프로그래밍을 위한 필수 언어로서 인터넷, 인트라넷 개발을 위한 언어가 되었
으며 분산 어플리케이션 구현의 주요 언어로 선택되고 있다．


  최초 버전인 JDK 1.0 에서는 기초적인 8개 정도의 패키지만을 제공하였으
나 JDK1.1 에서는 DB 연동 API, R入41 API 등이 추가되어 15 개의 패키치로
늘어나고 JDK 1.2(Java 2) 에서는 58 개의 패키지로 늘어나게 된다．


  58 개의 패키지중에는 기존 버전들에서는 Java의 표준 API 로 지원되지
않았던 JFC, CORBA 등의 API 도 추가로 지원되고 기존 패키지들의 기능들
도 많이 향상되고 추가되었다．


  물론 Java 2에서 기본적으로 지원되는 API 외에도 Sun Microsystems어］
서는 入4ail, Jini, Speech, Telephony, Serviet 등의 다양한 API 들을 추가로
제공하고 있다. 그런데 특정 버전에서 기본으로 지원되는 것과 그렇지 않은
것에는 프로그램을 사용자들게 제공시에 이 API 들도 추가로 제공하여야 하
는 등 여러 부분에서 활용상의 제한이 따르게 된다．
                            中   5-


===== PAGE 9 =====
  이 교육의 목표는 Java 2에서 제공되는 기본 API 들중에서 Enterprise 환
경에서 많이 활용되는 API 위주로 구현 방법과 활용 방법을 제시하는 것이며，
DB 연동, 분산처리 , JavaBeans 의 구현과 활용등의 내용으로 구성된다．




2절 JDK ] .］에서 JDK ] .2 로의 Upgrade


  다음은 JDK 1.1에1서 JDK 1.2 로 버전이 업그레이드되면서 추가되거나 향
상된 내용들을 점검한다．


      JDK 1.1                   >   Java 2


           m 구문은 거의 동일하다．
           1 다양한 포맷의 오디오 파일을 지원한다．
           - Collection Framework이 추가되었다．
           - JDBC 프로그래밍 관련 API의 기능이 향상되었다．
           U 컴파일 및 인터프리터의 옵션이 변경되었다．
           - CORBA 프로그래밍 관련 API가 추가되었다．
           - JavaIDL을 지원한다．
           e 원격 객체 활성화 기능이 추가되었다．
           - GUI 프로그래밍 관련 API인 Swing, 2D,
            Drag Dr아） 기능의 API가 추가되었다．
           -JRE와 Java Ph堰in을 지원한다．




                            6


===== PAGE 10 =====
2.1 JDK 1.2에서 추가＆향상된 기능들


 가. 보안 기능의 강화
    코드가 로드되면 현재 작동중인 보안 정책에 기반한 사용 권한들이 그
 코드에 로드된다.         이 때의 각 사용 권한에는 특정 리소스에 대해 어떤 접
 근 권한이 허용되는지 치정되어 있다. (java.policy)


 나. Swing(JFC)
    스윙（swing）은 플러그가 가능한 룩앤필(look and feel)을 가진 새로운
 GUI 컴포넌트들을 구현하는 JFC(Java Foundation Class）의 일부이다. 스
 윙은 순수 Java 로 구현되어 있으며 I기uggable Look and Fe이을 지원
 하므로 플랫폼과 무관한 Look and Feel(Windows, S이카治, 入/Iachintosh)
 을 설정할 수 있다．


 4. Java 2D(JFC)
    고급 2D 그래픽 및 이미지를 다룰 수 있는 클래스 세트이다. 여기에는
 라인 아트, 텍스트 그리고 이미지들을 하나의 광범위한 모델로 포함하고
 있다．


 라. Accessibility(JFC)
    화면을 음성으로 읽어주는 장치 , 음성 인식 시스템 , 그리고 점자 터미날
 과 같은 장애용 기술들과 상호 작용을 하는 Java 어플리케이션을 제작할
 수 있다．


 마. 드래그 앤 드롭(JFC)
   드래그 앤 드롭（Drag and Drop）은 Java 와 네이티브 어플리케이션 사
 이 그리고 단일한 Java 어플리케이션의 데이터 전송을 가능하게 한다．




                          7


===== PAGE 11 =====
바. 컬렉션（Collection)
           여러 데이터의 집합을 다양하게 처리할 수 있는 API 들이 지원된다．


사. Java IDL
           Java에 CORBA(Common Object Request Broker Architecture)호j-
성을 추가하여 표준에 기반한 상호 작용성과 접속성을 제공한다. Java IDL
은 분산형 \Veb 기반 Java 어플리케이션들이 산업 표준인 0MG IDL
(Object Management Group Interface Definition Language)과 h1OP *
이용하여 원격 네트워크 서비스들상의 기능들을 호출할 수 있도록 지원한
다．
아. 패키지 버젼 확인
           특정 JRE, VM 그리고 클래스 패키지의 버젼을 확인할 수 있는 기능이
     다．
 자. RMI 향상
      원격 객체 활성화를 비롯한 몇가지 기능이 향상되었다. 원격 객체 활성
     화에는 R入'II 가 객체에 대한 원격 호출에 사용하게 될 커스텀 소켓 형식을
     그 원격 객체가 지정할 수 있도록 해주는 Custom Socket Type 뿐만 아
     니라 원격 객체 및 자동 객체 활성화에 대한 지원 기능도 추가되었다.（커
          스텀 소켓 형식을 이용하면 SSL 등과 같은 보안 전송상의 RMI 지원이 가
          능해 진다.)


          차. 직렬화 기능 향상
           기본적인 쓰기／읽기 메카니즘과의 호환성을 유지하기 위해 직렬화된 더］
          이터를 클래스 필드들과는 독립적으로 지정할 수 있는 기능이 추가되었다．


          카. 오디오 기능 향상
            애플릿에서 뿐만 아니라 어플리케이션에서도 오디오 지원이 가능하다．
                                        8-
                                    -


===== PAGE 12 =====
타. jar 기능 향상
  jar 파일을 읽고 쓸 수 있는 API 가 추가 되었다．


파. JDBC 기능 향상
  SQL 문의 베치（batch）처리등 다양한 방식으로의 SQL 구문 수행과 수
행 결과（ResuitSet）의 커서 조정과 관련된 API 들이 추가되었다．


하. JavaBeans 향상
  운영 체제의 데스크 탑이나 브라우저등과 같은 런타임 환경과 보다 자
연스럽게 통합되는 세련된 JavaBeans 컴포넌트와 어플리케이션을 캐발할
수 있는 수단을 제공한다．




                     9


===== PAGE 13 =====
2.2 JDK 1.2 API


  Java 의 최초 버젼인 JDK 1.0에서는 8개의 패키지를 지원하였으며 ,         JDK
1.1어］서는 23개를 그리고 현재 버젼인 JDK 1.2에서는 약 60여개의 패키지를
지원한다. 다음은 JDK 1.2에서 지원하는 패키지 리스트이다．


   java.applet

                                  Applet 프로그래밍
   java. awt
   java.awt .color
   java. awt .datatransfer

    java. awt .dnd
    java. awt .event
    java. awt . font

   Java. awt .geom
    java.awt . im
    java.awt . image
    java. awt. image.renierable
    java. awt .print
                                   A\VT & 2D 프로그래밍
    java.beans
    java.beans. beancont ext

                                   Beans 프로그래밍
    java. io
                                   1/0 프로그래밍
    java. net

                                   Network 프로그래밍




                                  小 10 -


===== PAGE 14 =====
 java. lang

 java. lang.ref

 java. lang. reflect

 java .math

                                      기본 API
 Java. rmi

 java.rmi .activation
 java. rnii .dgc

 java. rmi .registry

 java.rmi .server

                                      RMI 프로그래밍
 java. security
java. security. acl

java.security.cert
java. security. interfaces
java. securi ty.spec

                                    Security , 보안 프로그래밍
java. sql

                                    JDBC 프로그래밍
java. text     뇨代無러 .    己卜母t 띤rj   沁튿．

java.util

java.util. jar

java.util .zip

                                    Text缸凡ii 프로그래밍
javax. accessibil i ty

javax. swing                 戈Mhy,.It入｝ 胛L
javax. swing.border          長Yn! 礎    ./
javax .swing. colorchooser

javax. swing.event


===== PAGE 15 =====
javax. swing. t ilectiooser
javax. swing.plal
]avax . swing. plat . basic
javax. swing.plat .nietal
javax. swing.plat .multi
javax. swing. table
javax. swing. text
javax.swing. text .html
j avax . swing . text .html . parser
Javax . swing. text . rtt
javax. swing. tree
javax.swing.undo
                                       Swing(JFC) 프로그래밍

org .onig. CORBA
org. omg . CORBA . DynAnyPackage
org. omg. CORBA . ORBPackage
org. omg .CORBA . portable
org. orng . CORBA . TypeCodePackage
org.onig.CosNaming
org. omg. CosNam i ng. Nam i ngCont ext Package
                                       CORBA 프로그래밍



 프로그래밍 종류에 따른 API 활용

      기본 프로그래밍 - java.lang, java.util, java.io
      DB 연통 프로그래밍 - java.sql
      분산 처리 프로그래밍 - java.net, java.rmi, org.omg
      GUI 프로그래밍 - java.awt, javax.swing
      Bean 을 활용하는 프로그래밍 - java.beans

                                       中 12 戶


===== PAGE 16 =====
3절 JDK 1.2 에서 지원되는 명령

 Ba引c Too冶


  Java 프로그래밍시 사용되는 기본 명령들이다．


   javac     The compiler for the Java(TM) programming language.


   java      The launcher for Java technology applications.
             In this release, a single launcher is used both for
             development and deployment.
             The old deployment launcher, ire, is no longer provided.


   javadoc   API documentation generator. Also see Javadoc 1.2
             appletviewer Run a            ug applets without a web browser.


   jdb       The Java language debugger that helps you find and fix
             bugs in Java(tm) programs.        cc시I c뇨L 넙브 竣 瀜&
                                                 洲   팍R針치는    巖）

   javah     C header and stub generator. Used to write native method.
                 3仄V仄 므卜 C르   6賠．

   javap     Class file disassembler extcheck Utility to detect Jar
             conflicts.


   jar       Combine multiple files into single archive(JAR) file.


  appletviewer   Run applets outside of the context of a World-Wide
                 Web browser.


                                  - 13 -


===== PAGE 17 =====
    Remote Method Invocation (RMI) Tools


        R入41 수행과 관련된 명령들이다．
氏血n써누     如I는.      갸，艇 => 巾｝ccJ{     徊諦1 引洲서／

        rmic           Generate stubs and skeletons for remote objects.


        rmiregistry    Remote object registry service.


        rmid           RMI activation system daemon.


        serialver      Return class serial VersionUlD.


     Internationalization Tools


        native2ascii    Convert non-Unicode Latin-i (source code and
                       Property) files to Unicode Latin-i.
 乂n小tNecd吃 m슈t.J畦
         Ciwe-타0人
     Security Tools


        Java 2에서 지원되는 Security Policy 관련된 명령들이다．


        keytool         Manage keystores and certificates.


        jarsigner       Generate and verify JAR signatures.


        policytool      GUI tool for managing policy files.




                                    - 14 中


===== PAGE 18 =====
Java IDL Tools


 CORBA 프로그래밍 관련 명령들이다．


 tnameserv       Provides access to the naming service.


 iditojava       Generates .java files that map an 0MG IDL interface
                 and enable an application written in the Java
                 programming lan只uage to use CORBA functionality.
                 This tool is available for download from the Java
                 IDL   web site. Documentation for the idltojava
                 compiler is included in the download.



         』赤代如 수九 :            /E只
  采 a,,』《.




                            - 15 -


===== PAGE 19 =====
4절 Enterprise Apr川cation 모델


4.1T叫0 기er 와 M미ti 기er



   First-Tier                 First      Mid미e-Tier          EIS-Tier
                              Tier

                              Client 卜
                                                         中     Server
    Client




  0                                        Services




4.2 씨ddle 기er에서 Bussiness Log允 울 구현하는 EJB 컴포넌트




                                            EIS Tier

             Web
                                           Enterprise
             Client
                                           Information
                                           Services




                         小 16 -


===== PAGE 20 =====
4.3 Web base Server & Client




                                                                                                                     D
                                                                                                                     \
                                                                                                                n스
                                                                                                                卞
                                                                                                                U



                                           11111= 1

                                           \




                                     山口口
                                                                口
                                                      //

                     Response                              //

                                                                袖
                                                                ／




                                   /
                                                                /




                                   /1口
                                     ／
                                                                       //

                                                                     / U
                                                      /
                                                                            鹹
                                                                    /


                                                                            ///


                                                                                        ///




                                                                                                /
                                                                                                ///
                                                                                                  //
                            ////

                                                                                  ///
                                                                                                       //
                                                                                                                         I
                                                                                                            /




                                                                                              - Socket 서버로 작성
                                                                                              -R八n 서버로 작성
                                                                                              小 CORBA 의 서버 객체로 작성
                                                                                              - Serviet 으로 작성



                       I,
             - Socket 클라이언트로 작성
             -R入4' 클라이언트로 작성
             - CORBA 의 클라이언트로 작성
             - Serviet 직접 호출




                                                            n


===== PAGE 22 =====
   II장 JDBC 프로그래밍




            학 습 목 표

' JDBC 프로그래밍 관련 클래스(java.sq
                            l)를
 점검할 수 있다．
·DB 연동 프로그램시 활용 가능한 연결 모델을
 점검할 수 있다．
. JDBC 드라이버의 종류를 알게 된다．
· Java 2에서 향상된 기능을 알게 된다．




                - 19 -


===== PAGE 24 =====
] 절 JDBC 개요

  Java 언어에서 DBMS 어］ 연동하여 데이터들을 처리하는 것을 JDBC 프로
그래밍이라고 한다． 이 절에서는 이러한 내용들에 대한 기초 지식을 다룬다．


1. ] JDBC 란 ?
   ＜品＼:C, n如bmCe m他鈿汁邑＞

  Java언어로 다양한 종류의 관계형 데이터베이스를 접근할 때 사용되는 표
준 SQL 인터페이스 API 로서 java.sql 패키지를 의미한다. 프로그래밍시 다
음과 같은 장점을 가지고 있다 :


  中JAVA 언어로 작성된 API이므로 시스템（운영 체제） 비의존적인 실행 파
   일을 만들어낸다．
  m데이터베이스 종류에 관계없이 프로그래밍할 수 있다. <AP工升 나는t比셔 렘치晙
                                B毛 9B叫 雀毛 /#p工 사삥 >
  1특정 데이터베이스에 연동되는 JDBC 프로그램은 다른 데아터베이스
   연동시에도 프로그램 수정없이 소스 코드를 그대로 활용할수 있다．
  -Applet 프로그램을 이용하여 서버에 존재하는 다양한 데이터베이스에
   직접 접근할 수 있으므로 Web서버 프로그램의 오버헤드를 줄여줄 수 있

   다   .




                          - 21 -


===== PAGE 25 =====
                                        Oracle
       Application
                                       database

            JDBC                                      恥\
     Oracle        Sybase               Sybase
     driver         driver             database




       Application                       ｝小ddleware

                                          Protocol
            JDBC             +1卜
                                                                       加e3
                                           handler
                                                           Vendor B
    DBMS-independent                   DBMS client-side
                                                           database
     protocol driver                      libraries
                                                            qf>,rver

礫   :5今B0   丁．汁e


     如yt毗 沙4{                      '咎이 '卜용




                                             - 22 中


===== PAGE 26 =====
1.2 JDK 에서 제공되는 JDBC 컴포넌트


  JDK 에서는 다음과 같은 총 세 개의 JDBC 관련 컴포넌트들을 제공한다．


 가. JDBC 드라이버 매니저
               JDBC 통작 구조에서 가장 기본이 되는 역할을 한다. JDBC API 로 작
 성된 프로그램이 데이터베이스를 호출할때 , 데이터베이스 드라이버를 선택


  '
      "
          }
              여 ' ］동":   난
                             "할을
                                   한다·    油山畔V.                  '   .   小叫·
 나. JDBC 드라이버 테스터
               JDBC 드라이버가 JDBC API 들을 제대로 실행시켜 주는지 테스트할
 수 있는 프로그램이다. 이 테스터를 제대로 통과한 드라이버만이 JDBC小
 COMPILANT라는 명칭이 붙는다.                          Pot汕仄Ce M西（'t)試叭 』           . ,, ,.,
                                                        무2｛
                                                       ,． 十     卜
                                                             乂卜용） 는 小NeV갸 Cl느 " 1늠끼r' 1
                                                                         棍誰차 뇨比 斟屯 PY也8Yh恤 "
 다. JDBC-ODBC 브리지
              ODBC 드라이버가 JDBC 드라이버처럼 사용되게 해주는 드라이버로서
 JDBC 드라이버가 지원되지 않은 DBMS 연동시 활용된다．
                     ＜切니＞          了D9e）
                                       卜州박딕머 팍치' O蛇 9B의 oPB C 如Jer斗 잉寸唵
                      '1            VY o1 b; c뇨P主 " 시4輛
                                            \1! )/
                                                        m)Rr 0니力1 乂卜丑
                                                     -I 口기 V 1           니 尸 ' /\   '1r =1   IC.




                                         - 23 -


===== PAGE 27 =====
1.3 JDBC API 의 기능 향상


  ,,JDK, ,1.1 -E1
           算胃：    ,, k1.2_ , 7]-J JDBC API , JDBC1.2 , k1 DB - ,.,
하고 처리하는데 있어서 기초적인 기능을 제공하였지만 좀 더 효율적이고 디
양한 기능을 제공하는 API가 부족하였다. Sun 사는 JDK 1.2 안에 JDBC 2.0
을 추가하여 DB 연동 관련 API 의 기능을 더욱 강화하였다．


  추가된 클래스 및 메서드들도 많으며 SQL 3.0 을 지원하도록 설계되었다．
                                   八스八八八＼ \\＼八小／   \   "＼八八／




다음은 JDK 1.2에서 향상된 JDBC API 기능이다．


    - Select 문의 수행 결과인 ResulSet 에서 커서를 원하는 위치로 이동
                       갔늪했으나， 喚9J呵) 등의 메
      할 수 있다· 간졸쁘늦크르쁘）쓰，
      서드가 추가 되었다．
                               " 知＼ 包如出叫‘卜甛唾 浪 年＼.
                           小M'"1\O
                                                        읫三比 引半   0卜읖雕 이돕．
    -DB 테이블에 객체 단위의 I/o 가 가능해졌다．                                    "


    e 여러 SQL 문의 일괄（batch) 처리를 할 수 있다．
          k免俄， 싸d赤，（낳魂 目寸"t딴 姚처리 ＞卜능

     -SQL 구문을 모르고도 JDBC API 에서 제공되는 메서드를 활용하여
       DB 핸들링을 할 수 있다．


     - SQL 3.0 을 지원한다．




                               - 24 -


===== PAGE 28 =====
1.4 JDBC 드라이버


     JDBC API 로 구현된 Java 프로그램이 어떻게 다양한 데이터베이스로의
접근이 가능하게 될까2 일반적으로 DBMS 들은 데이터베이스로의 연결 방법
이나 질의를 주고 응답을 받을 수 있는 방식들 즉, 접근 방식들이 각각 틀리

다．
     동일한 JDBC API 프로그램이 각 DBMS 어］ 알맞게 접근하도록 이어주는
인터페이스 역할을 하는 프로그램이 바로 JDBC 드라이버이다. 그러므로 접근
하고자 하는 데이터베이스가 어떠한 것인가에 따라서 이에 알맞는 JDBC 드라
이버를 선택하여야 한다．


  JDBC 프로그램은 JDBC 드라이버 매니저를 통해서 특정 테이터베이스를
직접 접근하고 처리하는 JDBC 드라이버를 먼저 선택한다. 그리고 이것을 통
하여 데이터베이스에 접근한다．


     여기에서 JDBC 드라이버 매니저는 Java 2 어］ 내장되어 있지만 JDBC 드라
이버는 연결하고자 하는 데이터베이스의 종류에 따라 필요한 것이기 때문에
내장되어 있지 않다. 그러므로 실제 사용자가 특정 데이터베이스와 연결하는
JDBC 프로그램을 작성할 때에는 그 데이터베이스와 연결시켜주는 JDBC 드라
이버를 구입해야 한다．




        JAVA 프로그램
                       JDBC 드라이버       DBMS



                     [JAVA와 DBMS]
                         - 25 -


===== PAGE 29 =====
[Sun 에 등록되어 있는 JDBC 드라이버들 ]


Vendor                 Type        DBMSs supported

Ashna Inc.             4           MS SQL Server

Borland                4            JDataStore

Caribou Lake Soft      3            Ingres, Oracle

FormVieb Inc.          4            FormY/eb

HXKJ                   4            xbase, Foxpro and VFP

IBM                    2, 3         IBM DB2 Universal Version 5.2, IBM DB2
                                    Connect Version 5. 2

IDS Software           3            Oracle, Sybase, Informix, MS SQL Server,
                                    DB2 , MS Access, FoxPro, dBase, etc.

Imaginary              4            mSQL

i-net Software         4            MS SQL Server

Informix Corporation   4            Informix

Merant                 3            DB2, Ingres, Informix, Oracle, Microsoft
                                    SQL Server, Sybase 10/11

Mini soft              2, 3         Image/Tur比lmage on 네P3000

OpenL ink              1,2,3,4      Oracle, Informix, Sybase, Microsoft SQL
                                    Server, DB2, Progress, others

 Oracle                 2, 4        Oracle 8.1.6

 Software AG               4         ADABAS D

 Software Synergy          3         Many, through ODBC

 Sybase, Inc.              3, 4      Sybase SQL Server, SQL Anywhere, Sybase I
                                     Q, Replication Server and more than 25
                                     enterpriseand legacy datase servers via
                                     Sybase OmniThNECf

 t h inVEB. C（知            3         Any database supportingJDBC or ODBC




                                  中 26 -


===== PAGE 30 =====
1.5 JDBC 드라이버의 종류


  JDBC 드라이버는 역할에 따라 크게 네가지 종류로 구분된다．


  가. JDBC叫ODBC 브리지 드라이버              4VPe \
                                      'I
    JDBC API 로 작성된 프로그램이 JDBC_ODBC 브리지를 통해 ODBC
  드라이버를 JDBC 드라이버로 여기고 동작하도록 한다. ODBC 드라이버가
  반드시 존재하여야 한다．
    전자 사인이 안 된 Java 애플릿은 보안상의 무제 때문에 이 드라이버
  를 사용할 수 없다. 왜냐 하면 일반 애플릿은 클라이언트쪽의 하드 디스크
  를 읽어서 ODBC 드라이버를 사용할 수 없기 때문이다．




                                                      三二
                                              口0O 毗
                                       二
   JDBC 를 구현한        JDBC-ODBC
   클라이언트             브리지               ＼
                                       0




  나. Native API 드라이버       ＋伊 그 .
    JDBC API 호출을 특정 데이터베이스 클라이언트 호출 API 로 바뀌
  주는 드라이버이다.         旺 YOVr, e- C갸 석며셔 眺              色今．

                              啣］e如畔           ＜櫂블"屯

   JDBC 를 구현한           Native API
                +H
   클라이언트                드라이버                  DB 고유
                                              프로토콜




                            - 27 -


===== PAGE 31 =====
                                         層和＼
다. 네트워크 프로토콜 드라이버 ＼十寸Pe 3 )
                                                                   JI
  이 드라이버는 클라이언트의 JDBC API 호출을 특정 데이터베이스의
프로토콜과 전혀 상관 없는 독자적인 방식의 프로토콜로 바꾸어 서버로
전송한다. 이 드라이버는 보통 Java 로 만들어진다. 서버에는 미들웨어가
있어 이 프로토콜을 특정 데이터베이스의 API 로 바꾸어 처리한다．
서버측의 미들웨어는 서버의 다양한 테이터베이스를 접근할 수 있도록
클라이언트의 요청을 처리하는 중요한 임무를 맡게 된다．
       여2\ DB卜人C 서버 사읾




                                        寸r
                                  1戶，
                                                                        DB
 JDBC 를 구현한        / " Net Pr。
                             t。
                     NetPr야OCOl
                                l
                               c。
                                                 「
                                                                                                          DB 서버2
                                                     +                  접근
                                                                              4

 클라이언트         r 드라이버           /                                       서버                    j
               \     \
                   \; （순수 Java)
                                                                                       :><\
                                                                                  ,:
                                                                             ,-
                                                      (midd1ewar
                                 「H박 .
                비 ／埃我 0얗入c 鳩 늄／냐
라· 더］'］터베이스 프로토콜 드라"］버 好cf 4)
  JDBC API 호출을 서버의 특정 데이터베이스에
                                                                                                  口1그＝.
                                                                                                  7< lH   프로토콜로 변환

시켜 서버로 전송하는 드라이버이다. 이 드라이버는 Java 언어로 만들어
진다. 두번째 형식과 비슷한 드라이버이지만 데이터베이스의 클라이언트
API 로 변환시키는 것이 아니고 직접 서버의 데이터베이스로 요청을 하게
된다. 이 형식의 드라이버는 일반적으로 데이터베이스를 생산하는 회사
에서 직접 만들어 제공한다. 인트라넷 환경 구축 개발에서 가장 많이 선택
되는 드라이버 형식이다．


  JDBC 를 구현한                                 DB Protoc아
  클라이언트                                      드라이버                                      DB고유
                                                                                       프로토콜
                                             （순수 Java)


                                                     - 28 -


===== PAGE 32 =====
1.6 데이터베이스 클라이언트／서버 어플리케0낸 설계


 가. 단층（0ne-Tier) 데이터베이스 설계


    사용자 인터페이스 코드와 애플리케이션 코드, 그리고 데이터베이스
 라이브러리를 통합시킨 모델이다．



            Application


             Database
              server




 나. 이층（Two-Tier) 데이터베이스 설계


   클라이언트 서버 기술의 출현과 함께 등장한 설계 방식이다．
 클라이언트 프로그램이 데이터베이스 서버에 sql 요청을 전달하면 서버는
 적합한 결과를 반환하고, 클라이언트가 이 데이터들을 일정한 포맷으로
 변환한다．

      Application        SQL request
       (client)
                           Socket
                                       Database
                    '0
      Client-side        Data reply     server
       libraries




                                              Storage

                              - 29 -


===== PAGE 33 =====
다. 삼층（Three-Tier) 데이터베이스 설계


   다층 구조의 설계방식으로서 , 클라이언트 프로그램들은 RDBMS로부터
추상화된 계층을 제공하는 중간 서버（Middleware）와 통신한다．
   중간 계층은 복수의 클라이언트 요청을 처리하고 하나 이상의 데이터
베이스 서버에 대한 접속을 유지하도록 설계된다．




 Application                   Middleware
                 QL reques
  (client)
                H=    1口H




                                Business           寸H
                4141日m1
                                                            Database
                Data reply        rules
 Client- side        H1H1mH=                                 server




                                                                       1
                4=
                 Change        Client小 side
  libraries
                notification
                                libraries


                                              (:
                                                   ,    '   二＞               />
                                                 Local
                                                                       Storage
                                              < eplicti아느                         /




                                    - 30 -


===== PAGE 34 =====
1.7 JDBC 프로그래빙 수행 흐름



  [JDBC 프로그램의 데이터베이스 접근 과정 ]




                                          7
                                          선택된 드라이버를 통




                                                        \
                                          하여 연결한다．
       (DBMS 에 알맞는   t'
                                      =
                                  =
                              =
                          1
  /    JDBC 드라이버를
       선택하여 메모리상
       에 로딩한다．

  가능하다면 Type3 와                                             데이터베이스에 표준
  Type4 를 선택한다．                                             SQL 구문을 전달하여
                                                            수행시킨다．




 가. JDBC 드라이버를 메모리상에 로딩한다．


        "'"""""""' " '牛世토翌uI ”
                             「' 乷烹；二'寸各．
 나. DBMS와 연결한다．
        Connection con =
  匹）
          Dr如er八4anager.getConnection("JDBC URL", " 계정 " , " 암호" );
  (｝크Connection con =
          DriverManager.getConnection( 'JDBC URL", Propertie s);

                                                               ＼午）嗣价 앙浚 六짜．
                                                                     객丙＼.


       回 仄岫M샤？『，秒C。 吃牡（"""" " ""‘
                               「싻비


===== PAGE 35 =====
다. SQL 문장을 연결된 DBMS 에 전달하여 수행시킨다．


      Statement stmt = con.createStatementO;
      ResuitSet rs = stmt.executeQuery
                      ("SELECT a, b, c FROM Tablel");

                 ，“：므，‘．「
                      Upd."
  ／入


 d：片wsu『 ' "띠少  ，「
               ，「
             ("DELETE FROM Tablel where num = 10");


라. 수행된 SQL 문의 결과를 처리한다．


 while (rs.nextO) {
         m1lt x = getlnt(1);
         String s = getString(2);
         float I = getFloat(3);
         System.out.println(x + s + I);

  }




                                  叫 32 -,


===== PAGE 36 =====
2 절 java.sql 패키지


  java.sql 패키지는 DB 연동 관련 API 들을 제공한다. JDBC 드라이버를 제
어 , 관리하는 기능의 클래스, SQL 구문을 수행시키는데 사용되는 클래스
SQL 문장의 수행 결과를 처리하는 기능의 클래스등이다．


   Interface


       Array
       Blob
      米CaHabIeStatement
       이ob
     >(Connection
     旅DatabaseMetaData       접속환       DB 受rVere1 성보

     米Driver      미날 4埼 Pd寸er' .
      米PreparedStatement
       Ref
      yResuItSet
       ResuitSetMetaData
       SQLDat a
       SQLInput
       SQLOutput
    米 Statement      c（立U붇 們眠 引한           念k ' 흩 섀성．

       Struct
                  \畔빠A叫寸．
                       7 n\ 孚叱    b\\Y '
   Class


                             楹毗 針mt1 .
       Date 吟9Q나＼ b苡配凞
       DriverManager
                                 - 33 -


===== PAGE 37 =====
    Dr iverPropertylnfo
    Time    자걍
    Timestamp 比놔師 ／掩

    Types 9缸리 ：睹社 9陟’


Exception


    Bat chUpdat eExcept ion
    Dat aTruncat ion
     SQLExcept ion
     SQLWarn ing




                              - 34 -


===== PAGE 38 =====
3 절 Fundamental JDBC 프로그래밍

 JDBC 를 연통하는 과정과 간단한 SQL 문장을 수행시키는등의 기초 과정
을 다룬다．


3.1 JDBC 드라이버묠 메모리상에 로딩시킨다．


   DB 연동시 사용될 JDBC 드라이버를 메모리상에 로딩시키는 과정은 다음
과 같이 두가지 방법중 하나를 선택한다．


   Class.forName （드라이버 클래스명）;
   DriverManager.registerDr如er （드라이버의 인스턴스）;


       예) Class.forName( "com.imaginary.sql.msql.MsqlDriver ');
          Class.forNameC'oracle.jdbc .driver.0racleDriver');
          Class.forName("ids.sql.lDSDriver')


          DriverManager.registerDriver (
                     new oracIe. jdbc.driver.OraceDriver0);
          DriverManager.registerDriver (
                     new com.imaginary.sql.msql.MsqlDriverO);




                              - 35 -


===== PAGE 39 =====
3.2 JDBC 드라이버큼 통히I DBMS 에 대한 연결 정보를 얻어낸다．


    DriverManager 클래스를 활용한다．


    Driver入4anager 클래스 2


           JDBC 드라이버를 설정하고 관리하는 기능
           JDBC 드라이버와 DBMS 의 연결 기능


    public static Connection getConnection(String unl)
    public static Connection getConnection(String unl, Properties info)
   甘public static Connection getConnection(String unl,
 니나 ‘口 '                                    string user, string passworci
    첫번째1 매개 변수인 un은 JDBC unl 이라고 하는 것으로 연결될 DBMS
  어］ 대한 정보와 사용될 JDBC 드라이버의 정보로 구성된다．


  다음과 같은 형식으로 지정된다：


           喪bc: subpr아oc아：S
               접蹇b9姻叫 .

           예) jdbc:oracle:thin:@multisunl:1521:lion
               jdbc :dbnet://object.cse.cau.ac.kr:8080/Northwind
               jdbc:odbc:wombat
               jdbc :odbc :qeora;UID=unico;PWD=flower


     위의 메서드 수행시 반환되는 것은 지정된 DBMS 와의 연결 상태를 제
   시하는 Connection 인터페이스의 인스턴스이다. 연결된 상태에서만 SQL
   구문을 수행할 수 있다．


                                  - 36 -.


===== PAGE 40 =====
3.3 연결된 DBMS 에 SQL 질의묠 전달하고 수행된 결과묠 얻는다．


      일단 DBMS 에 연결되면 SQL 질의를 실행하기 위해 서1 개의
  인터페이스（Statement, PreparedStatement, CallableStatement) 중
  한 개의 객체를 생성한다. 생성된 객체의 메서드를 통하여 SQL 문장을 수
  행할 수 있게 된다．


  1) SQL 질의를 위해1 필요한 객체 생성 방법
    위에서 언급한 서1 캐의 인터페이스 형의 객체를 생성하여야 한다. 각각
  의 인터페이스는 다음과 같은 특성을 가지고 있다．


  가） Statement 인터페이스
      Connection 인터페이스 객체의 createStatement() 메서드를 사용한
  다. Statement 객체는 주로 단순한 SQL 질의를 처리하고자 하는 경우 사
  용된다．


             Statement createStatementO;
             Statement createStatement (int resuitSetType,                       .· YbB( a . 0m休1 ＼唯이 깐
                                                                                              Y냔Uhi 戚의 七yPe능
                                                       m
                                                       "t       resuitSetConcurrency)            '       ;   ，川1    .   벼依d;
                                                                                                                           ;F
                                                                                                 \ 9｝茹：5륵 At7중．
     ,.太 resuitSetlype - Resul tSet .TYPE_XXX

必bH咀啣伽川［?                                                     ,. M寸姑．"「' " ’烈設姓’昕
                                                            ,，加
. . 包쑤尹＼ 1
   砂巴＼  \\        TYPE_SCROLLI NSENSITI YE 껴 " ',
                  mm)D 0/\1)r\1 T   T시이개（TmT1n고 ,，力-V >\'
                                                                      ..    I,   1石거＼
                                                                                 t窘t) ., h, ,卜 m가턱俄 吼斗
                                                            1   j k= n씨니U               1 1/ "       1

                  TYPE_SCROLL_SENSITI YE               才떱'"'                                叫                      如毛
             resuitSetConcurrency - ResuitSet .CONCUR_XXX
             나小LONCU辰1.READ_ONLY            扉而i.
                                             1
                                                 ／尸／
                  CONC咀娘越型且貳念四, '.1周 牛叫 D9에 ，卜H 빼磁 적孚 . )
                                           卜d？卜                                         十／1


      Statement 객체匿 생성한 후에는 다음 메서드들을 활용하여 SQL 문장
                                           - 37 -


===== PAGE 41 =====
을 수행시키거나 관리한다．


   void addBatch(String sql)

   void cancel ()

    void clearBatch()

    void clearWarnings()

    void 이ose()

    boolean execute(String sql)

    int[ ] executeBatch()

    ResuitSet executeQuery(String sql)
    mnt executeUpdate(String sql)

    Connect ion getConnection()
    mllt getFetchDirect ionO

    mllt getFetchSize()

    m1lt getMaxFieldSize()

    m1lt getMaxRows()
    boo lean getMoreResults()

     m1lt get伽eryTin祀out ()
    ResuitSet getResultSet()

     i nt ge tResul tSetConcurrency()

     m1lt   getResultSetType()

     m1lt   getUpdateCount ()

     SQLWarning getWarnings()
     void setCursorN叱(String name)

     void setEscapeProcessi평(b아ean enable)

     void setFetchDirection(int direction)

     void setFetchSize(int rows)

     void setMaxFieldSize(int max)

     void setMaxRows(int max)

     void set如eryTi毗out (int seconds)

                                    - 38 -


===== PAGE 42 =====
      (D executeQuery()
          ' ] 메서드는 SQL 문장' ] 阜묀；取J：岸인 경우 사용된다·
         ResuitSet 유형의 객체를 리턴한다．


      (2) executeUpdate0
         INSERT, UPDATE, DELETE 문장이나 CREATE TABLE,
         DR아） TABLE 과 같은 SQL DDL(Data Definition
         Language) 문장들을 실행할때 사용된다．


      @ 毗毗 （)         幼 油泂 이 b.如. 이프르             恥t R（小娃穹 힌 世 "1 잘赳 "'1혀'卜 한．
         SQL 문장이 한 개 이상의 ResuitSet 객체 또는 변환된 행의
         개수（Up曲te Count)둥을 반환시킬 가능성이 있을 경우에 사용
         된다. 이 경우는 주로 저장 프로시저를 실행하거나 프로그래머
         가 컴파일시 알 수 없는 SQL 문장을 실행할 때이다．


나） PreparedStatement 인터페이스
  Connection 인터페이스 객체의 prepareStatement() 메서드를 활용한
다. PreparedStatement 객체는 SQL문장이 한 7귀 이상의 파라미터（IN파
라미터）가 전달되어 실행되는 경우 사용된다. 즉, SQL 문이 고정된 내용이
아니고 가변 내용을 포함해야 하는 경우에 활용한다．


 PreparedStatement prepareStatement (String sql)
 PreparedStatenient prepareStatement (String sql, m1lt resultSetType,




 C
                                        m1lt resul tSetConcurrency)
      PreparedStatement pstmt = con.prepareStatement (
             "INSERT INTO sample VALUES (?,() ") ·，
           pstmt.setlnt (1, 100) ;                V
                                                 \V甲乖m'e\' "
           pstmt.setString(2, "abc ");
           pstmt .executeO;
                               - 39 -


===== PAGE 43 =====
 PreparedStatement인터페이스는 Statement 인터페이스를 상속받아 각
IN 파라미터 설정과 관련된 메서드들을 추가하였다．


      void addBatch()

      void clearPara肥ters()

      boolean execute()

      ResuitSet execute加ery()

       m1lt executeUpdate()

       ResuitSetMetaData getMetaData()

       void setArray(int i, Array x)

       void setAsciiStream(int parameterlndex, InputStream x, mllt length)

       void setBigDecimal(int para肥terlndex, BigDecimal x)
            setBinaryStream(int para肥terlndex, InputStream x, mnt length)
  A蜚 ' " "d
咎읔싻미 void setBlob(int i, Blob x)
       void setBoolean(int parameterlndex boolean x)

       \／아d setByte(int para祀terlndex, byte x)

       void setBytes(int para肥terlndex, byte[ ] x)
                                                                        length)
    年 void setCharacterStream(int parameterlndex, Reader reader, mllt
       void setClob(int i, Clob x)
    今4- void setDate(int para祀terlndex, Date x)

    십닥 void setDate(int para祀terlndex, Date x, Calendar cal)
       V아d setDouble(int parameterlndex, double x)
       v아d setFloat (int para祀terlndex, float x)

     뇻void setlnt (intparameterlndex, m1lt x)
       void setLong(int para肥terlndex, long x)

        void setNull(int para肥terlndex, mllt sqlType)

        void setNull(int paramlndex, mllt sqllype, String typeNanie)

        void setObject (int para祀terlndex, Object x)

        void setObject (int para肥terlndex, Object x, mllt targetSqllype)

        void setObject (int para肥terlndex, Object x, int targetSqlly思, int scale)

                                     巾 40 中


===== PAGE 44 =====
          void setRef (int i , Ref x)
          void setShort (int para代terlndex, short x)
   采void setStri璡(int para叱terlndex, Stringx)

   ＝蚣void setlime(int para肥terlndex, Time x)
    ／八＼

      void setTi叱(int parameterlndex, Timex, Calendar cal)
      void setTimestani巾nt parameterlndex, Timestampx)
      void setlimestamp(int parameterlndex, Timestampx, Calendar cal)
      void setUnic月eStream(int parameterlndex, InputStream x, int length)



그러므로 Statement 인터페이스의 메서드들을 그대로 사용할 수 있으며
다음과 같은 특징들을 추가로 포함한다：


      GD PreparedStatement 의 객체는 이미 컴파일된 SQL문장을 포
             함한다. 따라서 컴파일된 SQL문장은 데이터베이스에 의해 바로
             인식되어 빠르게 실행될 수 있는 장점이 있다. 그러므로 자
             주 사용되는 SQL 문장은 PreparedStatement 객체를 생성하여
             사용하는 것이 효율적이다．


      (2) SQL 문장이 한 7下1 이상의 II나 파라미터를 가질 수도 있다．
            H寸 파라미터란 SQL 문장 속에 값이 지정되지 않은 부분을 의
            미하는 것으로 " 7" 문자를 IN 파라미터 자리에 쓴다. IN 파라
            미터에 들어갈 값은 setXXX() 메서드를 사용하여 할당한다．


다） CallableStatement 인터페이스
  Connection 인터페이스 객체의 prepareCall() 메서드를 활용한다．
이 객체는 여러 개의 SQL 문장을 저장（Stored Procedure）하여 이 문장들
을 한 번에 실행하고자 하는 경우 사용된다. 함수 호출과 비슷하지만, 이
경우에는 이미 지정해 놓은 여러 개의 SQL 문장을 실행한다는 점이 다르
다. 일반적으로 한 개 이상의 " ?" TI'寸, OUT 파라미터가 담겨져 있는 SQL

                                        卞 41 -


===== PAGE 45 =====
문장이다．


     CallableStatement cstmt = con.preparedCall(
                         "{call getTestData(?, ?)}");


2) ResuitSet 인터페이스
  ResuitSet인터페이스는 SQL문장의 실행결과를 행（Row), 열（C이umn)
형태로 포함한다. 예를 들어 다음 문장들을 수행하면：


     Statement stmt =conn. createStatementO;
     ResultSet r=stmt.executeQuery( "SELECT a, b FROM Table") ;


               a              b
               12345           Jamse
               72531          David


  위의 테이블 형태의 결과 정보는 ResuitSet 객체 안에 포함된다．


   ci) 일단 ResuitSet 객체까 반환되면 테이블의 한 행을 가리키는
     포인터가 생성된다. 처음에 이 포인터는 아무것도 가리키지 않는다．


   (2) ResuitSet 인터페이스의 메서드 next() 를 실행하면 현재 포인터
     가 가리키고 있는 행의 다음 행을 가리키게 해준다．


   (3) XXX getXXX(String    columnName) 014 XXX getXXX(int
     C아umnlnde幻 등을 사용하여 포인터가 가리키고 있는 행에서
     지정한 열의 값을 얻는다．


    여기에서 XXX는 int, float와 같은 임의의 데이터 타입이다．
                               - 42 -


===== PAGE 46 =====
   columnNan祀은 열의 이름을 나타내는 문자열이며 , C아umnlndex는
   1 이면 첫번째 열을 2 이면 두번째 열을 의미하는 정수이다．
   다음은 위와 같은 테이블 내용의 ResuitSet 객체를 리턴한 경우
  각 열의 값을 출력하는 부분 예제이다（a 는 mlt 유형 , b 는 String
   유형으로 간주한다） :


          while (r.nextO) {
              m1lt i = r.getlnt("a");
              String s = r.getString("b");
              System.out.printlnC'ROW = " + j + " " + s);
          }

 next() 메서드를 사용하여 커서의 위치를 如rward 방향으로 행 단위로
이동하는 것 외에도 커서의 위치의 이동과 관련된 다양한 기능의 메서드들
이 지원된다．


       boolean absolute(int row)
       void afterLast ()
       void beforeFirst ()
       boolean first ()
       boolean isFirst ()
       boolean isLast ()
       boolean last ()
       booleab next ()
       boolean previous()




                               - 43 -


===== PAGE 47 =====
                     3.4 간단한 JDBC 프로그래밍 예저1


                                 [ sample 테이블 ]



                                 num - m1lt                  name - char(30)



                      [ 예제 于1                 sample 테이블로부터 name 열을 추출하는 예제 ]


                                 이 예제는 san叩蛇 테이블로부터 name 열만 추출하는 예제로 모든 name
                      필드를 추출하여 반복 출력한다．


                                 import java.sql. *


                                 class Select {
                                    public static void main (String args [1) throws Exception {
                                         II JDBC 드라이버를 로드한다．
                                         Class. forNameC'
                                                          凡哈 ' 鈿屯 汕口小小 mtm河")
                                         // 데이터베이스에 접속한다 . 적절한 JDBC URL 설정한다．




                                    /
                                         Connection conn =
                                                      DriverManager .getConnect ion(       );
                                                                       C心4bL三 0tat,h: 孔n7; ＠加.' /．그' 工勾' L(.:
                                                                                   1   1




                             ,
                                                                       '                     " . ' '6和小／
                                                                                   Ii-工／: //'"可’
                                         II SQL문을 수행시킨다 .
      ：小円
    企닦칙0戶 /\2·                      {    // SQL문4

畔色巴a 幽men
     只魂＜戶"
          t St毗 = conn . c：明teSt카,呻t (）·,                                                       " 6加，町 "7)
                                         ResuitSet rset = stmt.executeQuery( "SELECT name FROM sample") ;

,   , , .       ,   . ,, ,       \ 澧겅인
                     ./ / 추출된 데이터들중에서 name 필드만 출력한다．
            芝
'V.n1 't,.1L口 公升M 訓穹
 1                 '
    尾凹t r ' ey己y

    斛毗 p앉姓기t ' 友거＼
     心心．                                    Stri照咀{4etgSt,,ng(1);
                                         '"ile (                    - 44 -


===== PAGE 48 =====
                               System.out.println (s) ;
                           }
                }
            }

      [ 예제 2吃 sample 테이블에 저장하는 예제 ]


            이 예제는 sample 테이블에 num 과 name 행을 입력하는 예제로 입력후
      모든 행을 행단위로 출력한다．


            import java.sql. *;


            class Insert {
                 public static void main (String args II] ) throws Exception {
                           II JDBC 드라이버를 로드한다．
                           Class. forName( "        " );


                           // 데이터베이스에 접속한다 . 적절한 JDBC URL 설정한다．
                           Connection conn =
                                      DriverManager. getConnection(       );


                       II SQL문을 수행시킨다．
             . . 十方＼>Statement stmt = conn. createStatement 0;

，뇨7: i 略J弓-'- --- , stmt. executeuDcIate'. 11Nb! KI into samDie values ', 1U. ' unic ' 1) ,
\   ..Jd立으＼ YtLe1V\   11
    "<q q              Kesu! tbet rset = stmt. execute닉uery '.
                                               "SELECT num, name FROM sample") ;


                       // 추출된 데이터들중에서 name 필드만 출력한다．
                       while (rset.next () ) {
                                                           - 45 -.


===== PAGE 49 =====
                                                                  毓춧" ' "巴
                                                      ，小哮

                   mnt num = rset.getlnt
                   String s = rs飢 . getString（前·, 특빈꺼 Mh的쓱 지斗
                   Systeni.out.println (num + " : " + s) ;
               }
       }
  }



[ 예제 2召 : Applet 에서의 DBMS 연동 ]


  Applet 에서 직접 DBMS 어］ 연동하고                           sample 테이블에서 name 열을 추
출하여 브라우저의 TextArea 어］ 출력하는 애플릿예제이다．


  II       Filename : JdbcApplet. java

  import java.sql.*;
  import java.awt.*;

  import java.awt.event.*



  public class JdbcApplet extends java.applet.Applet
                                         implementsActionListener {

       But ton executej)utton;

       Text Area output;
       Connect ion conn;



           // 애플릿 화면구성

           public void mllit () {
                setLayout (new BorderLayout 0) ;

                Panel p = new Panel 0;

                p. setLayout (new FlowLayout (FlowLayout .比町));
                execute_button = new Button ( "Hello JDBC");
                                             - 46 -


===== PAGE 50 =====
     p. add (execute_button);

     execute_but ton.addAct ionListener(this);

     add ( "North", p) ;

     output = new TextArea (10, 60) ;

     add ( "Center ", output) ;

}


public void actionPerforr祀d(ActionEvent event){

     i f (event.getSource() == execute_button){

        try {
           output .setText (null);

           if (conn == null){

                II JDBC 드라이버를 메모리로 로드한다．

                output.append ( "LoadingJDBC driver.. . W1l" );

                Class c = Class. forNam三 ( "          ");             .

                // 데이터베이스에 접속한다 .                                     1 9ta奴G   니0人흩 뇨i岫洲


                                                                      ＼ 本岩聲뇨
                output . append ( "Connecti띵 to . . . W1l " );
                conn = DriverManager.getCo끄lection(              );



           }
                output.append ( "Connected枷");
                                                                          客沙「"쓰"
           Statement stmt = conn.createStatdnentO;



           II sql문을 수행시킨다．
           output.append ( "Executing query. . . W1l " );
           ResultSet rset = stmt.execut田uery ( "select name from sample");
           // 추출된 결과에서 name 필드만 반복 출력한다．

           while (rset.next 0)

                output.ap比nd (rset.getString (1) + "卄n") ;

           output. append ( "done.冊l");

                                       - 47 -


===== PAGE 51 =====
             } catch (Exceptione) {
              output.ap思nd (e.getMessage () + U쀼1l!t);




}


<! m巾 JdbcApplet 를 호출하는 HTML 파일 -->


<html>
<head>
<title>JDBC applet</title>
</head>

<body>


<hl>JDBC app 1et<Ih1>


애플릿의 소스 코드는＜a href="JdbcApplet .java">JdbcApplet .java</a>
를 참조하십시오．. . .
<hr>
<applet codebase=". " archive="JDBC 드라이버 파일명 "
code="JdbcApplet " width=500 height=200>
</app let>
</body>
</html>




                                  - 48 中


===== PAGE 52 =====
[ 예제 小4 오류 처리 예제 ]


 이 예제는 sample 테이블로부터 name 열만 추출하는 예제를 약간 수정하
여 오류 발생시 catch 절 처리 방법을 점검한다．


 import java.sql.*;
 import java.util.*


 class JdbclestSelectError {
   public static void main (String args [1) {
        II JDBC 드라이버를 로드한다．

        try {
             Class. forName( "     ");
         } catch(java. lang.ClassNotFoundException e) {
             Systdn.err.print ( "ClassNotFoundExcept ion: ") ;
             Systmerr.println(e. getMessageO) ;
         }
         try {
             // 데이터베이스에 접속한다 . 적절한 JDBC URL 설정한다．
             Connection conn =
                      Dr iverManager .getCo끄lect ion(     );


             II SQL문을 수행시킨다．
             Statement stmt = conn.createStataient 0;
             ResultSet rset = stmt.execute加ery ( "SELECT name FROM sample") ;


             while (rset.next 0)           {
                 String s = rset.getStri坦(1);
                 Systei.out.print1n (s);
             }
                                         - 49 -


===== PAGE 53 =====
} catch (S吼Exception ex) {

     Systdn.out.print1n ( "田LState: " + ex.get 요ate O); p-'-             ,
     System.out.println ( "Message: " + ex.getMessage O);         e＼札r\'W나勺9
     Systdi.out.print1n ( "ErrorCode:   ,, + ex.getErrorCode O); V帥小
}catch (Except ione) {
                                                                       ‘ "「「 "

  e . printStackTrace0;
                                                             ＼客
                          - 50 寸


===== PAGE 54 =====
『 "]"] "" """"「의 """""""'"" 之烈熬’
  선택된 JDBC 드라이버로 DBMS 연동시 다양한 연결（Connection) 정보를
출력하는 예제이다．


  II MetaData 처리 예제
  import java.sql.*;

  import java.util. *



  class ConnectApp{

    public static void main(Stri追 args[ ]) {

          try {


             II JDBC 드라이버를 로드한다．
             Class. forNa祀( "       ");


             // 데이터베이스에 접속한다 . 적절한 JDBC URL 설정한다．

             Connection conn =

                        Dr iverManager .getCo끄lect ion(   );


             DatabaseMetaData meta=conn.getMetaDataO;

             Syst8u.out .print ( "Database: "+meta.getDatabaseProductNameO) ;

             System.out.println(T' version "+叱ta.getDatabasePr以uctVersionO);

             Systdn.out.println( "IJser name: "+叱ta.getUserNai肥O);
             conn.closeO;

          } catch (Except ionex) {

             Systen.out .println(ex) ;

         )



                                          中 51 -


===== PAGE 55 =====
[ 예제 2田 ResuitSet 정보 출력 예제 ]


  지정된 SELECT 문장을 수행한 결과값인 ResuitSet의 정보를 출력하는 예
제이다．


  import java.sql.*;

  import java.util. *;



  class ResultApp{

    public static void main(Stri띵 args[ ]) {

          try {
               Class. forName( "     ");



               Connect ion conn =
                         Dr iverManager .getConnect ion(   );



               Statement statement = conn.createStatanentO;

               String sql = "SELECT * FROM sample";
               ResuitSet result = statdnent.execute沁ery(sq1);

               di sp1a外把訓 ts(result ) ;

               conn.closeO;

           } catch(Except ion ex) {

               Systen.out .println(ex);

           }
     }
      static void displayResults(ResultSet r) throws SQ比Xcept ion {
           ResuitSetMetaData rmeta = r. getMetaDataO;

           mllt nunColumns=r毗ta.getColumnCountO;

           for (int i=1; i<=n皿（o1umns;++i) {

                if (i<n끄Columns)

                                           - 52 小


===== PAGE 56 =====
                System.out .print (r毗ta.getColu距Na肥( i )+" I ") ;
            else
                Systen.out .printIn(r毗ta.geUo1uinnNa肥(i) );

        }
        while(r.nextO){
            for (int i=1; i< nuniColumns;++i) {
                i f (i<nunCol且ns)

                   System.out.print (r.getStri乷(i)+" I " );
                else

                   Systeni.out.println(r.getString(i) .trimO);
            }
        }
    }
}




                                      中 53 中


===== PAGE 57 =====
[ 예제 2刃 DB 에 다양한 SQL 문장을 수행시키는 예제 ]
 GUI 환경에서 로드시킬 드라이버의 크래스명 , JDBC URL 등을 입력하여
연동하고 입력된 SQL문장을 수행시키는 예제이다．


 import java.awt.*;

 import java.awt.event.*;

 import java.sql.*



 public class AccessAppextends Frame {

   lextField driver = new TextField(以);

    TextFieldurl = new lextField(旼）);

    TextFieldsql = new TextField(60) ;
    Button dolt = new Button( "Doit! ") ;

    TextArea resultArea= new TextArea(10,60);



    public static void main(String args[ ]){
         AccessApp app = new AccessAppO;

    }


    public AccessApp() {
          super ( "AccessApp");

          setup();
          pack() ;

          addWindowListener (new YiindowEventllandlerO) ;

          setVisible(true) ;

     }


     void setup() {
          setupMen好arO;

          setLayout (new Gr idLayout (2,1));

                                         - 54 中


===== PAGE 58 =====
     Pane! topPanel = new PanelO;

     topPane! .setLayout (new Gr idLayout(4,1));

     Pane! panels[lnew Pane! [41;

     for (int i=O; kpanels. 1ength; ++i){

         panels[ i] =new PanelO;

         panels[ i] .setLayout (new F! owLayout (FlowLayout .LEFT));

     }
     panels[01.add(new LabelC'Driver: "));

     pane!s[01 .add(driver);

     panels[11.add(new Label(T1UlL: ") );

     panels [ 11. add(ur I) ;

     pane!s[21. add(new Label( "요）L: ") );

     panels[21 .add(sql);
     dolt.addActionListener (new ButtonHand!er0);

     panels[31 .add(dolt);
     for (int i=0; i<panels. length;++i)

         topPanel.add(panels[ ij) ;
     add(topPanel) ;

     add(resu!tArea);

}


void setupMenuB카() {

    MenuBar menuBar = new MenuBar () ;

    Menu fi1eMenu = new Menu( "File");
    Menultem fi !eExit = new MenuIt帥( "Exit ");

     fi leExit. addActionListener (new MenuIt臼耐and1er0);

     fi IeMenu. add(fileExit) ;
    men沚ar. add(fi leMenu);

    setMenuBar (menuBar);

}

                                      - 55 -


===== PAGE 59 =====
void accessDB() {

       try {
            Class. forName(dr iver .getlextO);
            Connect ion connect ion=DriverManager.getConnect ion(url.getTextO , " " ,") ;
    Statement statement = connect ion.createStat帥entO;
             boolean hasResults= statenent.execute(sql.getlextO);
             i f (hasResults){
                ResuitSet result = statdnent getResuitSetO;
                if (result!=null) displayResults(result);
             } else resultArea.setlext ( "");
             connect ion.c1ose0;
        }catch(Exception ex){
             resultArea.setText (ex.toStri眼O);
        }
}


void displayResults(ResultSet r) throws SQLException {
       ResultSetMetaData rmeta = r. getMetaDataO;
        mllt numColumns= rmeta.getColumnCo끄ltO;
       String text = " " ;
       如r ( mnt i=1; i<=n皿（o1i.皿沮ls;++i) {
             i f (i<nimiolunns)
                text+=rmeta.getColumnName(i)+" I " ;
             else
                t ex卄＝r叱ta.getCoh丑nnName(i) ;
        }
        text += "WTl" ;
       while(r.nextO){
             for (int i = 1; i <= nunol끄ns;++i) {
                汀（i < nunColi皿rwis)


                                         - 56 -


===== PAGE 60 =====
                        text += r. getStri띵(i)+" I " ;
                    이 Se

                        text += r. getStri退(i) .trirnO;

                }
                text += "Yh-i ",

            }
            resultArea.setlext (text);

        }

    class ButtonHandler implementsActionListener {

            public void act沁nPe汀아毗d(ActionEvent ev) {

                String s=ev.getActionCc1lnandO;

                if (s == "Do it! ") accessDBO;

            }
    }

    class MenuIteiHand1er implementsActionListener {

            public void actionPerformed(Actio正：vent ev) {

                String s=ev.getActionCcmriandO;
                if (s == "Exit ")

                    Systdn.exit (O) ;

            }
    }

    class WindowEventllandler extends W indowAdapter {

            public void windoC1osi垠(Wi넌oEvent e) {

                Systdn.exit (O);

            }
    }
}

                                         - 57 -


===== PAGE 61 =====
                  ,,，《：枷小和e

3.5 DB 연동 프로그래밍 실습


  제시된 예제들을 참조하여 다음 문장들을 추가하고 테스트하여 각 문장들의 수행
결과를 점검하1 본다．



   CREATE TABLE COFFEES (
         COF_NA1lE VARCHAR(32),
         SUP_ID TNT,
         PRICE FLOAT,
         SALES INT,
         TOTAL INT
   )

       import java.sql.*;
       class Lab {
         public static void main (String args [1) throws Exception{
              II JDBC 드라이버를 로드한다．
              Class. forName(       );
               // 테이터베이스에 접속한다 . 적절한 JDBC URL 설정한다．
              Connect ion con =
                            Dr iverManager .getConnect ion(   );




  // 테이블 생성
   Statement stmt = con.createStat帥entO;
   stmt .executeUpdate( "CREAIE TABLE COFFEES " +
               " (COF_NAMEVAR거AR(32), SUP_ID TNT, PRICE FLOAT, " +
               "SALES INT, TOTAL INT) ") ;


                                         - 58 -


===== PAGE 62 =====
    // 데이터 입력
      stint .executeUpdate(

                    "INSERT INTO COFFEES " +
                    "VALUES ( 'Colcnbian' , 101, 7.99, 0, 0) ") ;
      stint .executeUpdate( "INSE丁 INTO COFFEES " +

                    "VALUES ( 'Espresso' , 150, 9.99, 0, 0) ") ;


    // 데이터 추출

      St r i ng query = "SELECT COFJ1AI4E, SALES FROM COFFEES ";
      ResuitSet rs = stint .execute如ery(query);
      while (rs.nextO) {

             Strings = rs.getStri進( "XFJ4AME") ;
             mlt n = rs.getlnt ( "SALES");
             Systein.out.println(n + " pounds of " + s + " sold this week. ");
      }

    // 필드의 값 수정

1     PreparedStatenient updateSales = con.prepareStat跏ent (
                   "UPDATE COFFEES SET SALES = ? WHERE COF_NAME LIKE ?") ;
      updateSales.setlnt (1, 75) ;
      updateSales.setStri띵(2, "Espresso") ;
      updateSales .executeUpdateO;


    // AutoCoinmi t 해제
      con .setAutoCamni t (false);
     PreparedStatement updateSales = con.prepareStat跏ent (
                   "UPDATE COFFEES SET SALES = ? WHERE COF_NAME LIKE ?") ;
     updateSales.setlnt (1, 50) ;
     updateSales.setString(2, "Cokxnbian");
     updat eSal es .execut eUpdat eO;

                                        뇨 59 -


===== PAGE 63 =====
  PreparedStat帥ent updateTotal = con.prepareStat8nent (
        "UPDATE COFFEES SET TOT舡， = TOTAL + ? WHERE COF_NAME LIKE ?");
  updatelotal .setlnt (1, 50) ;
  updateTotal .setStri召(2, "CoI加bian");
  updatelotal .executeUpdateO;
  I/con.commitO;
  ll con.rollbackO;
  con. setAutcC刃init (true);


// 就ored i玎ocedure호출 테스트
String createProcedure = "create or replace procedure in_sam " +

                            "is   "+
                            "begin "+

                            "insert into sample "+
                            "values(llll, 'abcdef ') ; "+

                            "end; ";

Statement stmt = conn.createStateientO;
stmt .executeUpdate(createProcedure);



Ca11ab1eStatanent cs = conn.prepareCall ( "{call in_sam}") ;
cs .executelJpdateO;




                                        - 60 -


===== PAGE 64 =====
4절 Advanced JDBC 프로그래밍

  이 절에서는 JDK 1.2에서 추가된 기능들을 점검한다．


4.1 SQL 문의 batch 처리

  JDBC 2.O 에서는 SQL 문장들의 일괄（batch）처리가 가능하다．

   // 예 1
       Statement stmt = con.createStat跏entO;
       con.setAutoC跏it (false);
       stmt.addBatch( "INSERT INTO employeesVALUES (1000, 'Joe Jones ') ");
       stmt.addBatch( "INSERT INTO depart叱nts VALUES (260, 'Shoe ') ") ;
       stmt .addBatch( "INSE丁 INTO empHdept VALUES (1000, '260 ') ") ;
       mllt [1 updateCounts = stmt.executeBatchO;


   // 예 2
       i f (dbnd.supportsBatchUpdates) {
             stmt.addBatch( "INSERT INTO . . . " ) ;
             stmt.addBatch( "沌L江E . . . n) ;
             stmt.addBatch( "INSERT INTO . . . 11) ;


             stmt .executeBatchO;
       } else {
             System.err.print ( "Driver does not support batch updates; ") ;
            System. err.println( "sending updates in separate statements. ");
            stmt.executeU月ate( "INSERT INTO . . .") ;
            stmt.executeUpdate( "碗LEW . . . " );
            stmt.executeUpdate( "INS町 INTO . .         .   ")
                                                                ;


       }




                                    - 61 -


===== PAGE 65 =====
4.2 ResuitSet 처리


  ResuitSet 이란 SQL Query 의 수행 결과를 저장하는 객체이다. 예를 들
어 " SELECT a, b, c FROM T카코el " 의 수행 결과는 논리적으로 다음과 같
은 내용의 ResuitSet 객체匿 리턴하게 된다．




  a              b                      C


  12345          Cupertino               2459723.495
  83472          Redmond                 1.0
  83492          Boston                  35069473.43



                                             열（column)


      가. 커서의 이동


      커서（cursor) 란 위와 같은 ResuitSet 객체에서 특정 행을 가리키는 포
      인터이다. 다음과 같이 처리하여 커서를 이동한다 :

      // 예 1
          rs.beforeFirstO;
          while (rs.nextO) {
               System.out. jrintln(rs.getString( "剛PJ'KY') +
                      ' " + rs.getFloat ( "SALARY");
          }

      // 예 2
          rs .afterLastO;
          while (rs.previousO) {
               System.out.print1n(rs.getString( "EMPJ'3") +
                   " " + rs.getFloat ( "SALARY");
          }

                                       - 62 -


===== PAGE 66 =====
나. ResuitSet 의 행의 개수 추출

    ResuitSet rs = stmt.execute그uery(
                " SELECT LAST_NAME, FI RST_NAME FROM EMPLOYEES");
    rs. lastO;
    mllt numberOfRows = rs.getRowO;
    Systdn.out.print1n( "XYZ, Inc. has " + num思rOfRows + " employees");
    rs.beforeFirstO;
    while (next ()) {
            . . . // retrieve first and last names of each employee
    }

다. ResuitSet 의 유형

    eTYPE中F아WARD中ONLY
    - TYPE_SCROLL_INSENSITIVE
    - TYPE_SCROLL_SENSITIVE

    中 CONCUR_READ中ONLY
    HCONCUR_UPDATABLE

   Connect ion con = Dr iverManager .getConnect ion(
                                       " j dbc：咽乙subpr야oco1叫소山nan祀 " );

   Statement stmt = con.createStataient (
               ResultSet.TYPE_SCROLL_SENSITIVE,
               ResultSet.CONCURHUPDATABLE );


    s t mt . setFet chSi ze(25) ;


   ResuitSet rs2 = stmt.execute沁ery(
              "SELECT EMP_NO, SALARY FROM EMPLOY旺：S");




                                    - 63 -


===== PAGE 67 =====
라. 열의 값 추출


   Strings = rs.getString(2) ;
   String s = rs.getStri평( "TIThE");


마. 다양한 유형의 값 추출


   getXXXX()
       XXXX :          Tnt
                       Float
                       String




    Object 유형의 I/O 가 가능해졌다．


    Struct address = (Struct)rs.getObject("ADDRESS");




바. PreparedStatement 의 사용


    PreparedStatanent pstrnt = con.prepareStatement (
                "SELECT EMP中NO, SAL사가 FROM EMPLOYEES IVHERE E湘巳NO = .7",
                       ResuitSet .1YPE_ :R(LL_SFNSITIVE,
                       ResuitSet .(XNIJRJJ어：)ATABLE) ;
    pstmt .setFetchSize(25) ;
    pstmt.setStri띵(1, "1000010");


    ResuitSet rs3 = pstmt.execute沁eryO;


사. 특정 열의 값 수정


    rs .absolute(4);
    rs.updateStri평(2, "321 Kasten") ;
    rs.updateFloat (3, 10101.0f);
    r s .updateRowO;
    또는

                                  - 64 -


===== PAGE 68 =====
   rs.updateString( "A어米ESS", "321 Kasten");
   rs .u녔ateFIoat ( "A刃T", 10101.of) ;
   rs .updateRowO;


아. 행의 삭제와 추가


   rs .firstO;
   rs .deIeteRowO;


   r s .moveTolnsertRowO;
   rs .update力ject (1, myArray) ;
   rs .updatelnt (2, 3857) ;
   rs.u넌ateString(3, "Mysteries ");
   rs . insertRow() ;
   rs. first();
   uprs. lastO;
   uprs.updateFloat ( "PRI氾", 10.99) ;
   uprs. cancelRowUpdatesO;
   uprs.updateFloat ( "PRICE", 10.79) ;
   uprs.updateRowO;



자. 특정 필드의 값이 NULL 인지 확인


   mlt n = rs.getlnt (3) ;
   booleanb = rs.wasNullO;




                               - 65 牛


===== PAGE 69 =====
4.3 PreparedStatement


  Statement 인터페이스의 자손 인터페이스로서 이미 컴파일된 SQL 문을
지정하여 객체를 생성한 후 IN 파라미터를 지정하여 수행시킨다．


  SQL 문에 들어갈 정보를 Dynamic 하게 II寸 파라미터를 사용하여 설정할
수 있는 방법이다.           PreparedStatement 로 지정되는 SQL 문은 precompile
되기 때문에 Statement 로 지정되는 SQL 문보다 수행 속도가 빠르다．


         PreparedStatdnent pstmt = con.prepareStatement (
                       "UPDATE table4 SET m = ? 'WHERE x = ?") ;


         PreparedStatement pstrnt2 = con.prepareStat帥ent (
                            "SELECT a, b, c FROM Tablel",
                                  ResuitSet .TYF屯요久（X工-S파ISITIVE,
                                               URJ]]才冶TABLE) ;
                                  ResuitSet .a烈：
         ResuitSet rs = pstmt2.execute그ueryO;


    가. 다양한 유형의 IN 파라미터의 전달


         pstnit .setLong(1, 123456789);
         Ps tint .setLo띵(2, 100000000);


         pstmt.setStri평(1, "Hi ") ;
         for (mlt i = 0; i < 10; i++) {
               pstmt.setlnt (2, i) ;
               mnt rowCount = pstnit.execute니：dateO;
         }
         PreparedStat帥ent pstmt = con.prepareStat帥ent (
         "UPDATE Tab1e3 SET Stats = ? WHERE Depts = ? " ) ;
         pstnit.setBlob(1, statistics);
         ps tint .setArray(2, depart毗nts) ;


         enip. salary= emp. salary* 1.5;
         PreparedStatement pstmt = con.prepareStat帥ent (

                                       니 66 -


===== PAGE 70 =====
               "UPDATE PERSO小EL SET EMPLOYEE = ? WHERE
                                             EMPLOYEEJ'O = 300485") ;
    pstmt.setObject (1, emp) ;
    pstmt .executeUpdateO;



나. 매우 큰 사이즈의 I卜J 파라미터


    java. io.File file = new java.io.File( "/ tr耳）/data") ;
    m1lt fileLength= file. lengthO;
    java. io.InputStreain fin = new java. io.FilelnputStream(file);
    j ava.sql .PreparedStatement pstmt = con.prepareStatanent (
                        "UPDATE TableS SET stuff = ? WHERE
                                            index = 4") ;
    pstmt.setBinaryStream (1, fin, fi leLe띵th);
    pstmt .executeUpdateO;



다. PreparedStatement 을 활용한 Batch 처리


    reparedStat톄lent pstmt = con.prepareStat帥ent (
            "UPDATE Table4 SET History = ? WHERE ID = 9 " ) ;
   pstmt.setClob(1, clobl) ;
   pstmt .setLong(2, 350985839) ;
   pstmt .adclBatchO;
   pstmt.setClob(1, c1ob2) ;
   pstmt .setLong(2, 350985840) ;
   pstmt.addBatchO;
    m1lt [1 updateC네ts = pstmt.executeBatchO;




                                    - 67 -


===== PAGE 71 =====
4.4 확장된 JDBC 데0I터 타입

   JDBC 2.0 부터는 SQL3에서 지원되는 확장된 데이터 유형을 지원한다．


   - BLOB (Binary Large Object)
   - CLOB (Character Large Object)
   - ARRAY
   -I끄STINCT
   - STRUCT
     REF
   - JAVA_OBJECT




                            - 68 -


===== PAGE 72 =====
4.5 Advanced 된 내용 점검 예저1

  JDK1.2에서 향상된 기능을 점검해 보는 예제이다. 반드시 JDBC 2.0 드라
이버를 사용하여야 한다．


  [ 예제 午1 11


  SELECT 문장의 수행 결과인 ResuitSet 의 내용에서 Cursor 위치를 Up!
Down 하는 예제이다．


  I/ Filename: SelectUpDown. java
  import java.sql.*;
  import j ava.ut il. Properties;
  public class Selectl加Down {
     public static void main(Stri召 args[ }) {

           try {
              Statement stmt;
              ResultSet rs;
              Class. forName( "       ");


              // 데이터베이스에 접속한다. JDBC 마d』 점검
              Connection con =
                         Dr iverManager .getCo끄lect ion(    );
              stmt = con.createStat帥ent (Resu1tSet .TYP요RcIL_JNSE놔SITIVE,
                                                       ResultSet .a烈]JRRE仙J札Y) ;
              stmt .setFetchSize(2);
              rs = stmt.executeQuery( "SELECI' num, name FROM sample");
              Syst師.out .println( "            forward 방향으로 모든 행 출력 ====== " );
              while( rs.nextO) {
                   Systdn.out.print (rs.getInt (1));

                                            - 69 -


===== PAGE 73 =====
        System.out .pr mnt ln(rs .getStr ing(2));

    }
    Systern.out .println( ''       첫번째        행 ======= " );

    rs. first();

    Systen.out.print (rs.getInt (1));

    Systeni.out .println(rs.getString(2));

    System.out .println( "         backward 방향으로 모튼 행 출력 =--m--TI,'.

    rs. lastO;

    do {

        System.out .print (rs.get Tnt (1));

        System.out .println(rs.getStri띵(2));

    } while(rs.previousO);

}
catch( Exceptione ) {

    e . pr intStacklraceO;




                                 - 70 中


===== PAGE 74 =====
[ 예제 4-2 ]



SQL 문장들을 BATCH 처리하는 예제이다．


II Filename : InsertBatch. java

import java.sql.*;
import java.util.*;
public class InsertBatch {
   public static void main(String args[ ]) {

        try {
           Statement stint;
           ResultSet rs;


           Class. forName( "       ");


           Connection con =
                      Dr iverManager .getConnect ion(        );
           stint = con.createStatdnent (ResultSet .1YPESCRCLL_SENSITIVE,

                                                      ResuitSet .CW町JJPDATABLE) ;
           stmt .addBatch( "IN丹T INTO sample VALUES (30, ' 홍길동 ' )") ;
           stmt.addBatch( "INSERT INTO sample VALUES (40, 'David') ');
           stint .addBatch( "IN얹RT INTO sample VALUES (50, 'Andy ') ") ;
          rs = stmt.execut田uery( " 얹孔ECT num, name FROM sample") ;
          while( rs.next () ) {
                Systein.out .print (rs.getlnt (1));
                System.out .println(rs.getStri띵(2));
           }
          System.out .println( "           배치 명령 수행                  = " );
          int[ ] updateCounts = stint .executeBatchO;
          rs = strnt.execute加ery( "SFLECT nun, name FROM sample") ;

                                         - 71 -


===== PAGE 75 =====
            while( rs.next () ) {
                Systan.out .print (rs.getlnt (1));
                System.out .println(rs.getString(2));

            }
        }
        catch( Exceptione ) {
            if (e instanceofBatchUpdate汶ception) {
                BatchtipdateExcept ion b = (BatchUpdateExcept ion)e;
                         柱諱才坤午
                Systen.e六.jrih노1n(1t 3;LException: " + b.getMessageO);
                Systdn.err.print1n( " LState:        " + b. get田LStateO);
                Systa.err.print1n( "Message:       " + b.getMessageO);
                Systan.err.print1n( "Vendor:      " + b. getErrorCodeO);
                System.err.print ( "Update counts: ");
                m1lt [I updateCounts = b. getUpdateCountsO;     UP如te望 記9{ 7 'l수．
                                                                 1
                for (mllt i = 0; i < updateCounts. Iength; i-F-F) {
                      Systen.err.print (updateCo끄lts[ iI + "      H) ;

                }
            } 이se {

                e . pr intStackTraceO;
            }
        }
    }
}




                                         - 72 -


===== PAGE 76 =====
 [ 예제 午3]


 SQL 문장을 사용하지 않고 DB 테이블의 내용을 수정하는 예제이다. 아직
까지 이 기능을 지원하지 않은 DBMS 서버와 JDBC 드라이버가 많다. 그러나
여기에서는 어떤 형식으로 구현되는지를 소스 레벨에서 점검해1 보도록 하겠다．


 I/ Filename: InsertRows. java
 import java.sql.*;
 public class InsertRows{
    public static void main(String args[ ]) {
         String unl ="
                                 1! 1




         Connect ion con;
         Statement stmt;

         try {
             Class. forNa祀( "           '');
         } catch(java. lang.ClassNotFoun現xception e) {
             Systan.err .printC'ClassNotFoundExcept ion: ");
             Systai.err .println(e.getMessageO);
         }
         try {
             con = Dr iverManager .getConnect ion(url, "myLogin", "myPassword");
             stint = con.createStatenent (ResultSet .TYPE_SCR兀L_SENSITIVE,
                                 ResuitSet .a烈卦LUPDATAB比）;
             ResuitSet uprs = stint .execute沁ery( "SELECT * FROM COFFEES") ;
             uprs.瓜0velolnsertRowO;
             uprs.updateStr ing( "QFJ哈ME", "Kona");
             uprs.updatelnt ( "SUP_ID", 150) ;
             uprs.updateFloat ( "PRICE", 10.99f) ;
             uprs.updatelnt ( "SA月S", 0) ;
             uprs.updatelnt ( "l工［AL", 0) ;

                                               - 73 -


===== PAGE 77 =====
            uprs. insertRowO;
            uprs.ui月ateStrit띵（"(X1나妗ME" , " KonaJecaf " );
            uprs.updatelnt ( "SIJP_ID", 150) ;
            uprs.u넜ateFloat ( "PRICE", 11.99f) ;
            uprs.updatelnt ( "SALES", 0);
            uprs.updatelnt ( "ltffAL", 0);
            uprs. insertRowO;
            uprs.beforeFirstO;
            System.out.println( "Table COFFEES after insertion: ");
            while (uprs.next ()) {
                String name = uprs.getStri乷( "QFJAME");
                mllt id = uprs.getlnt ( "SUP_ID");
                float price = uprs.getFloat ( "PRICE");
                m1lt sales = uprs.getlnt ( "SALES");
                m1lt total = uprs.getlnt ( "JOTAL");
                Systdn.out.print (name + "       " + id + "     " + price) ;
                System.out.println( "    " + sales + "        " + total) ;
            }
            uprs.closeO;      stmt .closeO;      con.closeO;
        } catch(羽LException ex) {
            Syst臼n.err.println( "蔑LException: " + ex.getMessageO);
        }
    }
}




                                        - 74 -


===== PAGE 78 =====
4.6 이미지 형식을 DB 에 저장하고 읽는 예저1

 Image 파일을 DB 테이블에 저장하고 다시 읽어 Image 파일로 저장하는
예제이다. 이미지가 저장되는 필드는 LONGRAW 로 처리한다．


 [ 예제 午41


 // 이미지 형식 저장
 II Filename : Picture. java
 import java.sql.*;
 import java. io.*;
 class Picture {
     public static void main (String args [1) throws Exception{
          Class. forNa祀 ( "       " );
          Connection conn = DriverManager.getConnection (         );
          File file = new File(args[ O} );
          InputStream is = new Fi lelnputStream(file);
          PreparedStatement strnt = conn.prepareStat帥ent (

                                    'insert into graphic values (? , ?)") ;
          stmt .setBinaryStreani(1, is,(int)(fi le. lengthO) );
          stmt .setStri退(2,args[O] );
          stmt .executeUpdateO;
     }
 }


 // 이미지 형식을 추출하여 출력
 //Filename : PictureView. java
 import java.sql.*;
 import java. io.*;
 import java.awt.*;
 class PictureView extends Frame {
     String st;
                                         - 75 -


===== PAGE 79 =====
    Pi ctureViewO{
            super ( "Image Input/ itput Test ");
            setBackground(Color .yel low);

            try{
               getDataO;
            } catch (Except ione){ e.printStackTraceO; }
            setSize(400,400);
            setVisible(true);

    }
    void getData() throws Exception{
            Class. forName ( "        " );

            Connect ionconn = DriverManager.getConnection (             );

            Statement stmt = conn.createStat톄ent 0;
            ResultSetrset = stmt.executeQuery ( "select * from graphic ") ;
            rset .next0;
            InputStream is = rset.getBinaryStream(1);
            Fi le뇨tputStream fo = new Fi leOutputStream( "t旺）.gif ");
            m1lt c = 0;
            while( (c=is.read0) !=-1)        fo.write(c) ;

             fo.close0; is.c1ose0; conn.c1ose0;
    }

    public void paint (Graphics g){
                                                                   ，윽
                                                                 그닉．
             T。             。lkitO;
              。lkit t = getl。                          叭半｛

             Image im = t. getlmage( "tmp.gif ");
             g . drawlmage( im, 10, 攷）, this);
        }
     public static void main (String args [1)                {

             PictureView pv = new PictureViewO;
     }
}

                                                 - 76 -


===== PAGE 80 =====
5절 데이터베이스 접근 모델


  JDBC API른 데이터베이스 어｝ 접근하기 위한 two小tier 와 three_tier
model 을 지원한다．


  小 Tw야tier model                   叫 Three_tier model
   데이터베이스에 직접 연결                            중간에 Middle tier 사용


       Client Machine                          Client I'Iachine


      JAVA Application                          JAVA Applet
                                               또는 HTML

       JDBC Driver                            browser




          I
         D미US
              DB八IS그）roprietary
              protocol                              !
                                                    卜：
                                           Application Server
                                                                   :., *,,：蛙
                                                                 CORBA 호줄



                                                (JAVA)

      Database server                          JDBC Driver


                                                      1DBMS-
                                                                     proprietary
                                                     1protocoi
                                                   DBMS

                                              Database server




                                  - 77 -


===== PAGE 82 =====
ifi장 Network 立로그래밍




           학 습 목 표

· Java로 구현하는 Socket 프로그래밍 기술을
 알게 된다．
- Java의 네트워크 API를 활용한 프로그래밍을
 실습한다．




             - 79 -


===== PAGE 84 =====
] 절 분산（Distributed) 시스템

분산 시스털J


   분잔 자스템은 특정 기능을 위해1 실행되는 프로그램들이 한 컴퓨터에서만 동
   작하는 것0I 아니라 서로 다른 컴퓨E札B에서 각각의 역할을 분담하여 동작하
   는 시스템이다． 0I ［내 각 컴퓨터들은 네트워크로 연결되어 있으며 서로 특정
   목적을 위하1 다양한 방식으로 데이터를 주고 받으며 실행된다．




           [ DB 서버 ]


          ［尸I    [
                                   [ Work 서버 ]


                                   11

                                                 \\
          [ 파일 서버 ]                      [ Web 서버 ]




                       [ 분산 환경 ]




                          - 81 -


===== PAGE 85 =====
2절 네트워크 프로그래밍 기초

2.1개요


  컴퓨터 네트워크란 두 대 이상의 호스트를 연결하기 위한 통신 시스템이
다. 호스트는 마이크로 시스템으로부터 시작해서 슈퍼 컴퓨터에 이르기까지
어느 것이나 될 수 있으며 , 컴퓨터 네트워크는 프로그래머를 위해 호스트 사
이의 통신 설정과 같은 작업을 대신 한다．


  하드웨어적으로（시스템 마다 통신 장비들이 구축되어 있는）Network가 구
성된 환경에서 수행되는 프로그램을 개발하는 것을 네트워크 프로그래밍이라
고 한다. 구현되는 대부분의 기능은 메세지（파일） 전송, 다른 시스템으로의 로
그인, 다른 시스템에 존재하는 실행파일 수행들부터 서버邑클라이언트 기능의
프로그램까지 다양하다. 여기에서 서버 프로그램은 어떠한 기능의 서비스를
담당하는 프로그램으로서 \Veb 서버 , telnet 서버 , mail 서버등을 예로 들 수
있으며 클라이언트 프로그램은 서버에 특정 기능에 대한 서비스를 요구하는
프로그램으로서 일반적으로 사용자들이 직접 접하게 되는 프로그램이다．


  컴퓨터의 네트워크 환경은 서버＆터미날 구조에서 서버邑클라이언트 구조로
발전하였다. 동일한 \win95 시스템이라도 서버 기능의 프로그램이 수행되면
이 시스템을 서버라고 부르며 클라이언트 기능의 프로그램이 수행되면 클라이
언트라고 부른다．


   네트워크 프로그램을 개발하는 이유는？
                 그리고 어떠한 기능들을 구현할까？


   서로 다른 프로그램이 통신（메세지를 주고 받는것）을 하려면 무엇이 필
   요할까？

  두 프로그램간에 통신을 하기 위해서는 통신 규약이 필요하다 이것을 프로
토콜（protoc아）이라고 한다. 현재까지 다양한 방식의 프로토콜이 개발되어 있
                      - 82 -


===== PAGE 86 =====
으며 네트워크 프로그램을 개발하는데 있어서 기본 베이스가 되는 프로토콜로
는 대표적으로 http, ftp, tcp, ip, udp 등이 있다．


  서로 다른 시스템의 프로그램간의 데이터 교환은 몇 개의 부분으로 나누어
서 진행되며 이것을 통신 계충이라고 한다. 대부분의 전산망에서는 'SO 의
Os' 계충 모델을 사용하여 기술한다. 그런데 실제 구현시에는 이 7 계층 모델
을 단순화한 4 계충 모델을 사용하여 통신 프로그램을 개발하게 된다．

          Process                            다ocess

             t                                  $
          Transport                          가ansport

             $                                  $
           Netw아k                             Network

              $                                  t
           Data 니nk                           Data Link
                       physical connection



  프로토콜들은 데이터의 전송 포맷을 결정하고 각 기능을 정의한 제어 문자
들을 정의한다. 뿐만아니라 Transport 계층을 처리하는 프로토콜들은 연결방
식도 결정하게 된다. 연결 방식은 연결 중심（Connect Oriented）적인 방법과
비연결（Connectionless) 방법으로 나눌 수 있으며 TCP 는 전자 방식이며
UDP 는 후자 방식이다．


  Java 언어에서는 다양한 기능의 네트워크 프로그램 개발을 지원하는 ARE
들(java.net戶］ 지원되며 상이한 물리적 네트워크의 세세한 점을 프로그래머에
게 감추고 보다 간단한 프로그래밍을 지원한다. 그러므로 좀더 쉽게 네트워크
프로그램을 개발할 수 있도록 한다．


  이 장에서는 네트워킹의 기본과 클라이언트 서버 어플리케이션을 Java 로
작성하는 기법 그리고 \Veb 서버에 대응하는 \Veb 클라리언트 프로그램 개발
시 활용되는 URL 프로그래밍등에 대하여 소개한다．
                          卜 83 卜


===== PAGE 87 =====
2.2 클라이언트 서버 어플리케이션


 네트워크 어플리케이션을 작성하는 데는 여러 가지 모델이 있다. 가장 널
리 사용되는 모델이 서버 프로세스와 클라이언트 프로세스라는 두 가지 형태
의 프로세스가 포함된 클라이언트 서버 모델이다. 호스트에서 서버 프로세스
를 시작하고 나면 클라이언트가 이곳에 접속하기를 기다린다. 동일 시스템 또
는 다른 시스템에서 수행되는 클라이언트 프로세스는 네트워크를 통해 서버에
게 요청한다. 서버는 이 요청에 반응하여 응답을 보낸다．
 다음은 클라이언트 서버 어플리케이션의 전형적인 정보 교환 과정이다：


  Network Link
                                      .1
                                  "
                        ..J   "




      send,,·tequest
         ．·d
                                                            receives' request  "
                                                                                   "




         Client                                                   Server


       HOST A                                                    HOST B


  Network Link
                                                                 \,．·．....
      rece鉀es reply                                         sends reply
        戶
               .. " '




         Client                                                              Server


       HOST A                                                    HOST B


                                           [ 클라이언트 서버의 동작 과정 ]




                                                   尸 84 -


===== PAGE 88 =====
卜 연결 방식


  서버와 클라이언트 사이의 통신은 두가지 방법 , 즉 연결 중심（Connect
Oriented）적인 방법과 비연결（Connectionless) 방법으로 일어난다．


 1) Connection-Oriented
   서버와 클라이언트 사이의 전용 연결이 설정된다．
   서버와 클라이언트는 이 연결을 사용해 정보를 교환한다．
   메세지의 전송 순서나 내용에 신뢰를 할 수 있는 통신 방식이다．


 2) Connectiess
   서버와 클라이언트 사이에 그다지 많은 통신이 일어나지 않는다．
   클라이언트가 서버에 요청을 보낼 때 데이터 그램 패킷 형태로
   보내며 그 각각에는 목적지의 주소를 지정한다．
   그러면 클라이언트로부터 요청을 기다리고 있던 서버가 이를 받아
   들이고 메세지에 포함된 클라이언트의 주소로 응답하게 된다．
   패킷 안에는 전달하고자 하는 메세지 외에도 송신자와 수신자에 대한
   정보도 가지고 있다. 패킷의 전달 여부와 전달 순서에 대한 보장을
   할 수 없는 방식이다．




                          - 85 小


===== PAGE 89 =====
卜 동기와 비동기 프로토콜


 1) 동기 프로토콜
    정치와 대기（st야） and wait) 프로토콜이라고 한다. 요구에 대한 응
    답이 완료될 때까지는 다른 송신은 처리할 수 없다. 구현이 간단하
    고 디버깅 또한 쉽다．


 2) 비동기 프로토콜
    클라이언트와 서버가 모두 다중 스레드되는 환경이다. 정지와 대기
    프로토콜에서 네트워크를 사용하는 행위를 금지시키는 이 기간동안
    한 끝이나 양쪽 끝에서 쓸모 있는 다른 동작을 할 수 있다. 자원
   을 효율적으로 관리할 수 있는 통신 방식이다. 대신 구현 방법이
   복잡하며 , 설계 과정에서 조건들에 대한 다양한 상황을 감안하여야
   한다．




                    - 86 -


===== PAGE 90 =====
卜 전송되는 데이타의 형식


  네트워크로 전달되는 데이터는 상당히 다양한 포맷으로 전송될 수 있
다. 많은 언어들은 Binary 와 ASCII 형식들을 지원하고 있으며 , Java에서
는 여기에 다음과 같은 두 가지 형식을 추가로 지원한다．


     Unicode, UTF(UCD Transformation Format)


W ASCII : 명령을 키보드로 입력할 수 있으며 이에 대한 응답이 바로 콘
         솔에 출력되므로 서버가 제대로 동작하는지 쉽게 검증이 가능
         하다. 인터넷을 구성하는 서비스들은 이 포맷으로 구축되어
         있으므로 플랫폼에 상관없다．


(2) Unicode : Java 가 냇붓짚으로쿄잔段슨튼륄율N외콘딜臭四七
         쁘뜨史長간量하기 때문에 쁘뜨쁘흐브튼원르恁싶엣스I
         전망있는 선택이 될 수 있다. 이 코드는 ASCII 처럼 용이한
         디버깅을 제공하지 않으며 Java 로 작성되지 않은 시스템에서
         는 쉽게 지원되지 않을 수도 있다. 16 비트 크기의 코드이므
         로 ASCII 형식보다는 두 배의 대역폭이 요구된다．


(3) UTF: UTF 는 Unicode 세트의 모든 문자들을 표현할 수 있다. 이 표

       현 방식은 갔르잣만단크艮캔숭읜겻1.크튼畺쓰lE욜한다· 7 비트
       ASCII는 기존과 통일하게 표현되며，르빈．틋母잔量관그垣노因e
       센튼量잣量윷웃브안튿量즈媛한뵤푯里하지만 낫멋진 문자들
       은 3 바이트를 사용하여 표현한다. 이러한 가변적인 바이트 할
       在二；
         玉三而자의 표현이 가능할 뿐 아니라 7비트 ASCII
       인 경우 추가적인 대역 폭을 요구하지 않는다는 장점이 있다．


@) Binary : 압축 파일 전송시 유용한 파일 형식이다. 큰 사이즈의 데이터
                          - 87 -


===== PAGE 91 =====
      전송시에 유용 하다. 대역폭 효율성을 고려하고자 하는 경우
      선택될 수 있는 데이터 형식이다．


卜 인터넷 주소


  인터넷에서 특정 호스트를 구분하기 위해서는 인터넷 주소（II) 주소）가
필요하다. 호스트는 인터넷 주소를 사용하여 물리적으로 통일한 네트워크
서브넷, 또는 인터넷에 의해 네트워크가 연결되어 있는 것과 같이 물리적
으로 다른 네트워크에 있는 다른 호스트와 통신이 가능하다. 따라서 지형
적으로 분리되어 있는 호스트는 인터넷 주소로 상대방을 지정함으로써 효
율적으로 통신을 할 수 있다．


  보통 인터넷 주소는 소수점에 의해 구분되는 네 개의 십진수로 구성된
다. 각 십진수는 32비트로 된 인터넷 주소에서 한 바이트씩을 나타낸다．
네트워크 어드레스가 동일한 호스트들간에는 라우터를 경유하지 않고 상호
통신하게 된다. 다른 네트워크 어드레스에 속하는 호스트들간에는 동일한
인터넷상에 있다 하더라도 라우터를 경우하여 통신하게 된다．



                     I
       네트워크 어드레스            호스트 어드레스




                   - 88 小


===== PAGE 92 =====
     3절 Java 에서의 소켓 프로그래밍


          Process Layer 와 Transport Layer 사이의 접속 기술로서 1982 년경
     VAX 를 위한 4.1cBSD에서 처음 제공되었다．


          두 캐의 통신 프로그램간의 Ending Point 라고도 간단하게 소개할 수 있는
     데,    일반적으로 UNI)( 시스템에서의 프로세스간의 통신(IPC) 에 주로 활용되
     다가 클라이언트 서버 환경에서는 서버 프로그램과 클라이언트 프로그램간의
     연결 기술로 많이 활용되고 있다．


   클라이언트H서버 어플리케이션에서 대부분의 통신은 Point나o-P아nt 방식
 이다. 즉 통신의 EndP아nt어］ 어플리케이션이 존재하는 형태이다. 소켓은 단
 일 시스템 또는 서로 다른 시스템에 존재하는 프로세스간의 통신을 위해 각각
 서버와 클라이언트의 End P아nt 역할을 한다．


          Java 에서는 이러한 기능의 프로그램을 좀더 쉽게 개발하도록 java.net 3괘
키지에 ServerSocket 또는 Socket 이라는 클래스를 제공하고 있다. Socket
클래스는 클라이언트 측을 그리고 ServerSocket 클래스는 서버 측의 소켓을
표현하는데 사용된다．


      일단 클라이언트와 서버 사이에 연결이 설정되면 이들 중 한 쪽이 연결을
닫기 전까지는 얼마든지 메세지를 교환할 수 있으며 , 양방향으로의 통신 또한
가능하다. 그리고 병렬（Concurrent)기능의 서버는 멀티스레드로 구현할 수 있
다．
      다음은 Java 언어를 활용하여 네트워크 어플리케이션 개발시 활용 가능한
java.net 패키지의 인터페이스, 클래스, 예외 클레스에 대한 리스트이다．




                               叫 89 叫


===== PAGE 93 =====
Interface Summary


ContentHandlerFactory
FileNameMap
SocketlmpiFactory
SocketOptions
URLStreamHandlerFactory


Class Summary


Authenticator
ContentHandler
DatagramPacket
DatagramSocket
DatagramSocketlmpi
HttpURLConnection
InetAddress
JarURLConnection
MulticastSocket
NetPermission
PasswordAuthentication
ServerSocket
Socket
Socketlmpi
SocketPermission
URL
URLClassLoader
URLConnection
URLDecoder

                          - 90 -


===== PAGE 94 =====
URLEncoder
URLStreamHandler


Exception Summary


BindException
ConnectException
MalformedURLException
NoRouteToHostException
ProtocolException
SocketException
UnknownHostException
UnknownServiceException




                          小 91卜


===== PAGE 95 =====
[ 예제 十1 간단한 TCP 서버와 TCP 클라이언트 구현 ]


  소켓 연결을 활용한 서버＆클라이언트 프로그램으로서 클라이언트로부터
연결 요구가 들어오면 " Java Daytime Server: 날짜／시간" 정보를 전송한다．


  II Filename : DayServer. java
  import java. io.*;
  import java.net.*;
  import java.util.*;


  public class DayServer {
      private ServerSocket ss;


      public static void main(String args[ ]) throws lOException {
           DayServerd = new DayServerO;
           d. go 0;
      }

      public void go() throws lOException {
           Socket s = null;
           II 1313포트로 서버소켓을 기동시킨다．
           // 큐의 개수는 5이다．                                    ,   .
                                             L놔＼\            口 '\ .
           ss = new ServerS。
                           cket(...., 5); : 如
            for ( ; ;) {
                // 클라이언트로부터의 연결 요구가 들어올때까지 대기한다．
                S = ss.acceptO; 낵申枓． \念n\- o\毗，"
                BufferedWriter out = new BufferedllVriter(
                   new 0utputStrea끄Writer (s.gettXitputStreamO));
                // 클라이언트로 메세지를 전송한다．
                out .writeC'Java Daytime server: " + (new Date0).toString() + "Wn");
                out.close0;
                5 . 이ose();
            }
       }
  }


                                        小 92 小


===== PAGE 96 =====
II Filename : DayClient. java
import java.net.*
import java. io.*;


public class DayClient {
    String host;
    Socket s;


    public static void main(Stri평 args[ ]) throws lOException {
            DayCl ient day = new DayClient (args[O} );
            day.goO;
    }


    public DayClient (Stri唯 host) {
            this.host = host;

        }


    public void go() throws lOExcept ion {
            // 명령행 매개변수로 입력된 서버의 'p주소로 소켓연결을 시도한다．
            s = new Socket(host,        );
            BuffereciReader i = new BufferedReader (
                          new InputStreamReader (s.getlnputStream0));
            // 서버로부터 전송된 메세지를 화면에 표준 출력한다．

            Systan.out .println(i .read匕ine0);
            i .이ose() ;
            S .이ose() ;

    }
}




                                        - 93 -


===== PAGE 97 =====
［예쩨1 3- 2        병렬 서버의 구현 ]



  소켓 연결을 활용한 서버忍클라이언트 프로그램으로서 클라이언트로부터의

연결요구를 좀더 효율적으로 처리하기 위해 3개의 스레드 상에서 클라이언트

로부터의 연결요구를 동시에 처리하도록 구성된 프로그램이다．



  II Filename : MultiServe. java
   import java.net.*;
   import java. io.*;
   import java.util. *;


  public class Mult iServe implementsRunnable {
       private ServerSocket ss;


       public static void main(Stri也 args[ ]) throws Exception{
               MultiServem = new MultiServeO;
               m.goO;
       }


       public void go() throws Except ion{


   /
               // 주어진 포트로 서버 소켓을 기동시킨다 . 큐의 개수는 5이다．
               ss = new ServerSocket (    , 5) ;
               // 스레드를 3깨 기동시킨다．

               Thread ti = new Thread(this, "1") ;
               Thread t2 = new Thread(this, "2") ;
               Thread t3 = new Thread(this, "3");
               tl. startO;
               t2.startO;
               t3.startO;

           }

                                         中 94 -


===== PAGE 98 =====
    public void run() {
         Socket s = null;
         BufferecPYriter out = null;
         String myname = Thread.currentThreadO.g


         for ( ; ;) {

             try {
               Systei.out.println( "thread " + myname + " about to accept. .");
               // 클라이언트로부터 연결 요구가 들어올때까치 대기한다．

               s = ss.acceptO;
               System.out.println( "thread " + myname + " accepted a connection");
               out = new Buffered\Yriter(
                             new 0utputStreamWriter (s.getoutputStreamO) );
               out.write(叫name + " " + new Date() );
               1/ 10초간 引eep한다．
                //Thread.sleep(100(刃）, 由？H익 七＼
                                             ，似.小｝
               out .write( '，做-1");        따t     七＼,m쿄갸

               out .closeO;
               catch (Exceptione) {
               e . pr intStackTrace();


         }
    }
}




                                         - 95 小


===== PAGE 99 =====
     [ 예제1 3召 데이터그램 구현 예쩨1 ]


           서버와 클라이언트간의 통신에 UDP를 활용한 예제로서 클라이언트의 준비
     상황에 상관없이 1초마다 시각 정보를 전달하며 클라이언트도 1초 이상 대기
     한 후 서버로부터의 패킷이 도착하면 이 내용을 화면에 표준 출력한다．


           II Filename : DayBcast. java
           import java.net.*
           import java.util.*;


           public class DayBcast {

           才 Dat agramSocket ds;
U햐哲坰          Dat agrai甲acket dp;
C' " ht.
              InetAddress addr;


              public static void main(String args[ ]) throws Exception{
                   DayBcast db = new DayBcast (args[O] );
                   db.goO;
              }
              // 주소 정보를 명령행 매개변수로 전달받아 InetAddress 깩체로
              // 변환시키고 Dat agramSocket 객체를 생성한다．
              public DayBcast (String target) throws Exception {
                    addr = InetAddress.getByName(target).;    나．.. l      的   明
                                                             0典1'Q仍；
                           M＝小八八入스＼入小드／?l今 叩
                    ds = new DatagramSocketo;              1

               }


              public void go() throws Except ion{
                    byte [1 buff;
                    for ( ; ;) {
                       Thread. sleep( 1000);

                                               戶 96 中


===== PAGE 100 =====
Systdi.out .println( "Sending");
String s = (new DateO).toStringO;
buff = s.getBytesO;
／半 전송된 데이터와 이 데이터의 길이 그리고 패킷이 전달될 포트번호
   를 지정하여 Dat agram Packet 클래스의 객체를생성한다 . 求／
dp = new DatagramPacket(buff,buff.Iength,addrj..);
                                              '니r/    .
ds .send(dp);                                   뇨伊休 '성左 .




                         - 97 -


===== PAGE 101 =====
II Filename : Day1Watch. java
import j ava.net . *;
public class DayWatch {
    private DatagramSocket ds;
    private DatagramPacket dp;


    public static void main(Stri띵 args[ ]) throws Exception{
         Day!Watchd = new DayWatchO;

         d.go0;
    }


    public void go() throws Except ion{
         byte [1 buff = new byte[64] ;
         String s;
         // 지 정포L포드로小소켓을 小생성 한다．
         ds = new DatagramSocket(         );
         /／수신한 데이터를 담는 버퍼로 Dat agram Packet을 생성한다．
         dp = new DatagramPacket(buft, buff.Iength);
         for ( ; ;) {
             // 서버로부터의 전송을 받기 위해 대기한다．
             ds.receive(dp);
             s = new String(dp.getDataO);
             Syst帥.out.println( "Time signal received from " + dp.getAddress() +
                                               "쀼ll Time is: " + 5) ;

         }
    }
}




                                     - 98 -


===== PAGE 102 =====
4절 URL 프로그래밍


  이 장에서는 World Wide Web(WWW）에서의 Java 어플리케이션 그리고
Java Applet 개발시 필요한 기본 개념과 관련 클래스들에 대하여 소개한다．


4.1 URL! 프로토콜뇨MIME
       介， '
          寸
  World Wide Web은 전역적인 컴퓨터 네트워크로서 , Web 클라이언트는
Web 서버에 요청을 하고 이로부터 정보를 받는다. 각 나라의 우편 주소처럼
정보의 위치는 여러 컴퓨터에 존재한다. 각 컴퓨터가 정보를 얻기 위해 자신
만의 주소 체계를 가지고 있다면, 정보의 접근 방법은 매우 어려워질 것이다．


  Web의 구조는 \Web어］서 정보에 접근하고 서비스할 수 있도록, 하나 또는
모두가 사용할 수 있는 단일화 된 주소 체계를 형성하고 있다. 이 네트워크의
정보는 URL 이라는 주소 체계를 사용하여 접근할 수 있다. 이것은 World
Wide Web어］서 자원（문서 , 이미지 ..）을 고유하게 나타낼 수 있는 구조화된 주
소이다．


                   r   跳ii而ters                  / " " "悴腱   兀斗
         http:/／佃va.sun.com:8町교듦在프血＞


                                  11          Filename

                                   Directory pathname

                          Port number
                        !
              Internet hostname


        Protocol




                                  - 99 -


===== PAGE 103 =====
  완전한 URL의 형식은 제일 앞에 지정되는 프로토콜 지정자에 의해 결정된
다. World Wide Web에서는 여러 프로토콜이 지원되며 가장 많이 쓰이는 것
이 HTTP 이다. 이 외에도 news, gopher, ftp 등이 사용된다.              클라이언트
서버에서 이들의 상호 작용은 다양한 프로토콜에 따라 달라진다．


  Web 클라이언트 즉, 브라우저는 위와 같은 형식（URL）을 사용하여 특정
Web 서버에게 원하는 형식의 자원을 요구하게 되며 , Web 서버는 요구된 파
일을 찾아 클라이언트로 전송해1 준다．


  브라우저가 이미지 파일 , 텍스트 파일, 오디오 파일 그리고 그밖의 여러 가
지 다양한 파일 포맷을 어떻게 구분하는 것일까9 클라이언트와 서버 사이의
프로토콜 일부에는 서버에서 클라이언트로 보내는 데이터에 대한 헤더 또는
컨텍스트 정보를 포함하고 있다· 이 컨텍스트 짚브畺                                ose
loternet Mail Exten針叩S工포맺읖 사용하여 나타낸다. MIME 은 다음과 같은
형식으로 구성된다 :                     m午旨iD卜 m咤 莎b상아지 他   4燮 ,



   " ""/' """빠岫帥아：舶P唵 牡沙／？裝姚）
                            「 ）」去
  Web 클라이언트（브라우저）는 이 정보를 사용하여 서버로부터 전송된 파일
의 타입을 구분할 수 있게 된다. World Wide Web어］서 지원되는 주요 타입으
로는 텍스트, 이미지 , 오디오, 비디오, 어플리케이션이 있다. 다음은 많이 사용
되는 入4IME 타입의 일부 예이다：


   내용 타입          MIME 타입／서브타입             파일 확장자


   G伊이미지          image/gif                .gif
   단순 텍스트 파일      text/plain               .txt
   HTML파일         text/html                .html, .htm
   오디오파일          audio/basic              .au
                         - 100 -


===== PAGE 104 =====
     4.2 Java와 World 쌔de Web


       Java는 World ＼사ide Web의 자원에 접근하는 어플리케이션 작성시에 사용
     할 수 있는 많은 클래스들을 제공한다. URL 클래스는 Uniform Resource
     Locator 개념의 추상 자료형이다．


       URL 클래스와 URLConnection 클래스는 Java 의 \Veb 어플리케이션 개발
     어］ 필요한 대부분의 요구를 충족시켜준다．


       URL 클래스에서 제공되는 가장 기본적인 네트워크 기능은 URL 이 가리키
     는 데이터를 스트림 형태로 읽어들이는 기능이다. URL 클래스의 인스턴스는
     다음과 같이 URL 을 나타내는 텍스트 스트링을 사용하여 만들 수 있다：


        URL theUrl = new URL("http://w出w.sun.com/");


       URL이 만들어치면 openStream() 메서드에서 URL 이 가리키는 데이터를
읽을 수 있는 간단한 메커니즘이 제공된다. 이 메커니즘을 통해 Datalnput
Stream 이나 InputStreamReader 클래스와 같은 다른 종류의 입력 스트림이
나 판독기를 연결시키는 기능을 구현하여 정보를 읽어낼 수 있다．


      다음은 httj) 상의 파일을 로드하는 openStream() 메서드의 사용 예제이
다. 로드하는 파일은 클래스 파일이나 이미지등 \Veb 서버에서 제공되는 것이
면 어떤 데이터이든 좋으며 , 로컬로 사용될 수 있도록 디스크 파일어］ 저장한
다．
                                 -. 101 -


===== PAGE 105 =====
[ 예쩨1 4- 1     URL 관련 예L;1) J



  URL 클래스 관련 예제로서 명령행 매캐변수로 입력되는 URL StringC'

http:/／호스트 도메인： 포트번호／디렉토리／파일명 "）을 입력받아 지정된 서버로

Request를 보내고 응답된 결과를 파일어］ 저장하는 프로그램 예제이다．


  [url.txt I


  0001 http://java.sun.comlindex.html
  0002 http://www.naver.com!index.html
  0003 http://7 0.12.100.21:8088/




  II Filename : GetURL. java
  // 텍스트 파일어］ 저장되어 있는 URL 문자열을 읽고 이 문자열에 지정퇸 서버로
  /／자원을 요청하고 전달받은 자원을 하드 디스크에 저장하는 프로그램

  import java. io.*;
  import java.util.*;
  import java.net.*
  import test. filename.MakeFileNa祀;



  class GetURL {

    public static void main(Stri追 args[ ]) {


          try {
                  // 파일을 저장할 디렉토리 생성
                  File fl = new File(args[1] );
                  fl .mkdirs();
                  h/ URL이 있는 파일을 연다．
                  FileReader fr = new FileReader (args[0
                  BufferedReader br = new Buffere垠eader(fr);

                  String s;
                  mllt ch;
                                       叫 102 -


===== PAGE 106 =====
            while ( ( s = br.reaclLine0) != null) {


                  StringTokenizer sti = new Stri退Tokenizer (s, '1 'D;

                 while (stl.hasMoreTokens0) {
                          String first   =    stl.nextToken0;        /／순번
                          String second = stl.nextToken0;            h/ URL


                          m1lt c;
                          II t爪L 객체 project 를 생성
                          URL project = new URL(second);
                          // 파일이 저장될 디렉토리
                          String dir = fl. getPath0;
                          //   파일 이름 생성
                          MakeFileNa陀 mf = new MakeFileName(first);
                          // 파일 생성
                          Fi leOutputStream fo = new Fi !eO此putStream(dir + "I" +
                                                  mf .ReturnNa朧0);

                          InputStream is = project.o思nStream0;

                          while ( (ch = is.readO) != -1) {
                                      fo.write(ch) ;
                          }
                          fo .c1ose0;


                  }
             }

            br .c1ose0;
        } catch (I（霓xception e) {
              Syst帥. out.println( "I(沌xcept ion어］러 발생 : 읽을 파일이 있는지 확
                                              인하세요 " );
              System.out .println(e);
        } catch (Except ione) {
              System.out .println( " 오류가 발생했습니다 " + e) ;
        }
    }
}
                                    - 103 -


===== PAGE 107 =====
II Filename : MakeFileName. java
// 객체 생성시 전달된 식별번호에 현재 시간과 날짜 청보를 추가하여 파일명을
// 만들어 내는 키능의 클래스로서 test. filename 이라는 패키지에 저장하였다．


package test. filename;

import Java. io.*;
import java.util.*;


// 파일명 생성 클래스
public class MakeFileNa祀 {
  String seq;
  Strin협丸ffer sb = new Strit退JE沁ffer();


  II Constructor
  public MakeFileNa陀(String sq) {
        seq = sq;
   }

  private void MakeName() {
        Calendar calen = Calendar.getlnstanceO;
        // 년도
         sb .append(calen.get (Ca1endar.YEAR));
         sb .ap思nd( "_");
         // 월
         if     ( (ca1en.get (CalendarJINI11) + 1 ) < 10) {
                sb .append( "O");
         }
         sb.ap思nd( (ca1en.get (Calendar 附fl1) + 1) );
         sb.append( "_");
         // 일
         if     ( (calen.get (Calendar.DATE)) < 10) {
                sb .appendC'O");
         }
         sb .ap比nd(calen.get (Calendar .DATh) );
         sb .append( It1U);
         // 시
         if     ( (calen.get (Calendar.F JR) ) < 10) {
                sb . append( "0");
          }
                                       中 104 -


===== PAGE 108 =====
          sb .ap思nd(calen.get (Calendar .攷JR));
          sb.append( "_");
          // 분
          if     ( (calen.get (Ca!endar.MI세Th)) < 10) {
                 sb . append( "0");
          }
         sb .append(calen.get (Calendar .MINUTE) );
         sb.append( "_");
         // 순번
         sb .append(seq);
         sb .append( " .html ");
    }

    public StringBuffer ReturnName() {
         MakeNameO;
         return sb;
    }
}




                                       - 105 -


===== PAGE 109 =====
     [ 예제 4-2 URL 의 응답헤더（Response Header) 출력 예제 ]


        URL 클래스 관련 예제로서 명령행 매개변수로 입력되는 URL StringC'
     h仇다／
        ／호스트 도메인： 포트번호／디렉토리／파일명 "）을 입력받아 지정된 서버로
     Request를 보내고 응답된 결과중 응답헤더의 내용을 출력하는 프로그램 예제
     이다．


       II Filename : GetMIMF}leader. java

        import java.net.*;

        import java. io.IOException;

       public class GetMlM따eader {

           public static void main(Stri召 args[1) {

                   try {
                      URL u = new URL(args[O] );

                      URLConnect ion uc = u. "因如呻迦（＼如
와冷" 妖＼旭m
       『U 흩                                          . {％익 뇨쿄計 ）配寸                           取
  曜嶝斜                 Syst n.out .printlnC'Content-type: " + uc .getContentTypeO);

                      System.out .println( "Content-encodi坦: " + uc.getContentEncodingO);

                      System.out.println( "Date: " + new java.util.Date(uc.getDateO) );

                      System.out.println( "Last modified: " +

                                    new j ava.ut i I .Date(uc.getLastModifiedO));
                      Syst帥.out.println( "Expiration date: " +

                                   new java.util.Date(uc. getExpirationO));
                      Systdn.out .println( "Content-length: "     + uc.getContentLengthO);
                   } catch (MalformedURLException e) {

                      Systeni.err.println(args[ il + " is not a URL I understand') ;

                   } catch (KException e) {

                      Systen. err .pr mnt ln(e);



           }
       }
                                                   - 106 -


===== PAGE 110 =====
[ 예제 4召 URL Encoding 규칙 점검 예제 ]


  Web 클라이언트에써 Web 서버로 전송되는 문자열은 URLEncoding 이라
는 규칙이 적용된다. java.net 에는 일반 문자열을 URLEncoding 문자열로 인
코딩하고 디코딩하는 클래스가 지원되며 이 클래스를 점검해1 본다．


 II Filename: Encodelest. java

  import java.net．小ii且ic（넜er;

 public class Encodelest {



     public static void main(String args[ ]) {

          System.out .pr mnt ln(URL邑lcoder .encode( ''This string has spaces") );


                                                   ？唯留has*stars")) . ..
          System.out .println(liR且lcoder.enc以e( '

          System.out .pr mnt ln(URLEncoder .encode( ''1Iiis物string哭'has狂）ercent物signs " 刀;

          System.out .print ln(UR且lcoder .encode( "This+string+has+pluses") );
          System.out .pr mnt ln(URLEncoder .encode( "This/stri띵/has/slashes"));

          System.out .print ln(［胤邑lC（넜er .enc（月e( "This쀼"str ing "has쀼"quote "marks") );

          System.out .print ln(URLEncoder .encode( "Thi J' tri呵has:colons"));

          System. out .print ln(URLEncoder . encode( "Thi可．)tri ! .has.periods"));
                                                        ＼人니 i   브
          System.out .println(URLEncoder .encode( "This=string=has=equals=si卽s "));

          System.out .println(URLEncoder.encode( "This芯strii退芯has&ani思rsands" ));

     }
 }




                                        叫 107 叫


===== PAGE 111 =====
[ 예제 4-4 네트워크로 이미지 파일을 읽어서 출력 ]


    URL String으로 지정된 WebA］버에 Connectio" 하여 "] "］지 파일京存읽어
서 캔바스       （Canva引위에
  =11 -.,1 l /／기   \ (l ,. 11
                              출력하는
                              文 二4 =a 1H
                                         프로그램        예제이다.
                                         \f ＝그 mn =n ／口r1 -i1 』뇨］ 1기
                                                                       ..\k戍'
                                                                          1 in>V/ ' \

                                                                                    ，거．入艾入
                                                                                         ‘
                                                                              ，戶V
   II Filename : Getlmage. java
    import java.awt.*;
    import java.awt. image.*;
    import java.net.*;


    class MyCanvas extends Canvas {

        Image i ;
        public MyCanvas(Image i) {
              this. i = i;

        }

        public void paint (Graphics g) {
             g. drawlmage(i , 0, 0, this) ;
        }
    }


    public class Get Image {
        String name;
        Frame f;
        Image i;
        MyCanvas c;
        Medialracker m;
        Toolkit t = Toolkit.getDefaultToolkitO;


        public static void rnain(String args[ ]) {

                                              戶 108 -


===== PAGE 112 =====
     if (args. length != 1) {
         Systdn.out.print1n("Usage: java Getlmage< image卞小L>");
         Systdn.exit (1);

     }
    Getlmage that = new Getlmage(args[O] );
     that .go();

}

public Getlmage(Stri退 name) {
     this.narne= name;

}

publicvoidgo() {
     Object o = null;
     // 지청된 타이틀을 갖는 프레임을 생성한다．
     f = new Fra思( "Image from " + name) ;
     URL source = null;
     URLConnection con = null;

     try {
         // 지정된 UI乙로 Connect i이盲｝여 내용을 리턴한다．
         source = new URL(name) ;
         o = source.getContentO;
     } catch (Exceptione) {
         Syst6n.out.printlnC'Problem with URL " + source) ;
         e.printSt     race(System.out);            . . = - 之b느』
                                     （今 曳奴W可叫 " ' “迂k 1 "b'
         System.exit (2);

     }

     if (o instanceof ImageProducer) {
         // 읽어온 URL의 내용으로 이미지를 생성한다．


                                    - 109 -


===== PAGE 113 =====
            i = t. createlmage((ImageProducer)o);
        } else {
            Systdn.out.println( "URL " + source +
                           " didn't give me an ImageProducer ");
            Syste.out.println( "but a "+o.getClassO.getNa肥O+"instead");
            Systan.exit (3);

        }
        c = new MyCanvas(i) ;
        ni = new MediaTracker (c);
        m. addlmage(i, 0);

        try {
            m. waitForAllO;
        } catch (Exceptione) { 1* do nothing */ }
        f. add( "Center ", c);
        c. setSize(i. getViidth(c), i .getHeight (c));
        f.pack();
        f . setVisible(true);
    }
}




                                     中 110 -


===== PAGE 114 =====
5 절 네트워크 소스 분석（Chatting)

 이 절에서는 Java 로 개발한 Chatting 기능의 소스를 분석하여 Java 의 네트워크
프로그래밍에 대한 활용력을 높인다．



 다음은 Chatting Server 의 소스이다．


 II Filename : ChatServer. java
 import java. io.*;
 import java.net.*;
 import java.util.Vector;
 public class ChatServer{
   // 각 클라이언트에 대한 정보를 Vector 로 관리 水／
    Vector V;
   ServerSocket server;


    public static void main (String args[1) {
            new ChatServer (Integer.parselnt (args[O] ));
    }

   public ChatServer (iht. port) {
                              \




         V=new Vector () ;

         try {
             server=new ServerSocket (port) ;
             Systeii.out.println( "Server Started.. .') ;
         } catch (Exceptione) {

                 Systdn.out .println(e) ;
        }
        try {
             while (true) {
                 Socket socket=server . accept 0;
                                      中 111 -


===== PAGE 115 =====
                     PrintWriter out=new PrintVriter (socket.getOutputStreamO, true);

                     BufferedReader in=new BuffereclReader (

                                     new InputStrea沁teader (socket .getlnputStreamO));

                     // 연결해온 클라이언트에 환영 메세지 출력

                     pr intNames(out);
                     // 클라이언트마다 ChatConnect i（丑1 객체 생성

                     ChatConnect ion c=new ChatConnect ion( in,out ,this);

                     add(c) ;

                     c. startO;

                }
        } catch (Except ione) {

                Systen. err .pr mnt ln(e);

                Systen.err.printin( "Usage: java ChatServer port ") ;

        }
}

/／클라이언트에 대한 ChatC月기lect ion 을 Vector 어］ 추가

public void add (ChatCo끄lection c) {
        V . addEl帥帥t (c);

}

/／모든 클라이언트에1 메세지 출력

synchronized public void print in (Strings) {
        for (mnt i=0; i<V.sizeO; i++) {

                ChatConnect ion c=(ChatConnect ion)V. el帥entAt (i) ;

                    c. printin(s);

            }
    }




                                                 - 112 -


===== PAGE 116 =====
    // 동일 이름에 대한 점검
    synchronized pub! ic boolean hasName (String name, ChatConnect ion cname) {

          for (mnt i=0; i<V.sizeO; i-f-I-) {
              ChatConnect ion c=(ChatConnect ion)V.elenentAt(i) ;
              if （이＝cname砥 C . na毗（) .equals(nai肥）)

                  return true;

          }
          return false;

    }

    // 모든 클라이언트에 환영 메세지 출력

    synchronized public void printNames (PrintWriter out) {
          if (V.size()= 0) {

              out.print!n( "Nobody connected! ");
          } 이se {

              out.println( "Co긔nected: ");
              for (mnt i=0; i<V.sizeO; i++) {
                  ChatConnect ion c=(ChatConnect ion)V.elenentAt(i) ;
                  out.println( "-   "+c.nameO);
              }
          }
         out .println( 'Welcc*祀! ");
         out. f1ush0;

    }

    // 클라이언트에1 대한 정보 삭제
    synchronized public void removeConnect ion (ChatConnection c) {
         V . r帥oveEl帥ent (c);

    }
}

                                       小 113 -


===== PAGE 117 =====
II Filename : ChatConnection. java



import java. io.*;

import java.net.*;

import java.util. Vector;

class ChatConnect ion extends Thread {

   ／非 클라이언트로 부터의 입력받는 객체 求／

   BufferedReader In;
  ／木 클라이언트로의 출력 객체 水／

   PrintWriter Out;

   ChatServer C;
  ／水 연결해온 클라이언의 이름 " === name " 水／

    String Name=t"?7?";



   public ChatConnection (BufferedReader in, PrintWriter out, ChatServerc) {
         C=c; In=in; 0ut=out;

    }


    public void run() {

         try {
            while (true) {

                 String s=ln.readLineO;

                   Systan.out .println(s) ;

                 if (s==nu11) break;

                 if (s.starts\Vith( "==")) {

                     Na叱＝S. substr ii乷（4); I/ 클라이언트의 이름을 얻어낸다．
                     if (C.hasNa肥(Name, this)) {

                       // 동일한 이름이 이미 존재하므로 다른 이름을 선택 ! !

                       Out.printlnCtChoose another name! Connect ionrefused. ");
                       Out. flushO;

                                        - 114 -


===== PAGE 118 =====
                        In.closeO;

                        0ut.closeO;

                        C. reioveConnect ion( this);

                        ret끄rn ;

                    }
                    C. println( "     "+Name+" connected");

                } else { II normal input

                    if (Na叱.equalsC'???") ) bre出

                    C .println(s);

                }
            }
         } catch (Exceptione) {e.printStackTraceO; }

        C. println( "=== "+Name+" di sconnected");
        C. r톄ioveConnection(this); II remove me from the server

         try    { II close all streams
            In.closeO;

            Out .이ose();

         } catch (Exceptione) {e.printStackTraceO; }

    }
    ／來 ChatServer 가 클라이언트에 메세지 출력시 호출 水／

    public void print in (Strings) {
         Out.print in(s);

         0ut. flushO;

    }

    public String name () {
         return Name;

    }
}


                                          - 115 -


===== PAGE 119 =====
다음은 Chatt ing Client (Applicat ion) 소스이 다．


II Filename : Chat. java

packagefi )               弘【k哨e
import java. io.*;
import java.net.*;


public class Chat {
    public static void main (String args[ ]) {

         try {
             II Socket 객체를 생성한다． ,,.                            陟t叭以恤“
                                        1 \(                    \
             Socket socket=new Socket (args[O] ,Integer .parselnt (args[1] ));
             PrintViriter out=new Pr intYriter(socket.getOutputStreamO, true);
             BufferedReader in=new BufferedReader(
                                  new InputStreamReader (s어：ket .getlnputStreamO));




                                                                          三
             // 이름을 출력한다．                                                      뇽由
                                                                      （
             out.println( "=== "+args[2] );


                                                              伊寸陟
             out. flushO;                0＼   누   ·
                                                                      批
             II ChatWindow를 생성한다．
                   n
                   L
                           此
                           砥                              m
                                                          삐           7
                                                                                  小
                                         鮎
                                                      n
                                                      乙
                           M             可
             new
                      1
                           W             n



                                                                毛 妙
                                                                            呻
                      h
                  publicvoid end O{                                         씨
                      Syst帥. exit (0);

                  m
             };
         } catch (Exceptione)            { II connectionproblemor wrong parameter
             System.err .println(e);
             System.err .pr mnt ln( "Usage: java chat .Chat server port yourna肥 ');
         }
    }
}

                                              - 116 -


===== PAGE 120 =====
II Filename : ChatWindow. java
package chat;
import java.awt.*
import java.awt.event.*;
import java. io.*;
public class Chat\ilindowextends Frame implementsRunnable,ActionListener {
  ／非 서버로의 출력 객체 牛／
   PrintWriter Out;
   八서버로 부터의 입력 객체 非／
   BufferedReader In;
   ／木 서버로부터 전달된 메세지 출력 컴포넌트 半／
   TextArea Output;
   ／求 사용자가 입력하는 메세찌 입력 컴포넌트 木／
   lextField Input;
   String Name;


   II ChatWindow를 생성하고 사용자로부터 메세지를 입력받아 서버에 전송하는
   // 기능의 스래드를 기통한다．
   public ChatVindow (PrintWriter out, BufferedReader in, String name) {
        Out=out;
        In=in;
        Name=name;


        setSize(550,450);
        setLayout (new BorderLayout 0) ;
        add( "Center " ,Output=new TextArea0);
        Output .setEditable(false);
        addC'South" ,Input=new TextField0);
        Input .addAct ionListener (this);
        setVisible(true);

                                    卞 117 小


===== PAGE 121 =====
        II Wind列Event 어］ 대한 리스너 등록

        add1 indowListener (new ViindowAdapter ()

                  public void windowClosi召 (YiindowEvent e) {

                         setVisible(false);

                         dispose() ;

                         end() ;

                  }
        });

        // 입력 스레드 시작

        Thread t=new Thread(this);

        t. startO;

}

// 서버에써 전송된 메세지를 읽고 TextArea 어］ 출력하는 기능（무한 루프）

public void run () {

        try {
              while (true) {

                  String s=ln.read너ne0;

                  if (s == null) { // 종료

                       Output. ap思nd( "拌nConnect ion closed. ") ;

                       return;

                   }
                  Output . append( 'Wn"+s);

              }
         } catch (Exceptione) {

                   Output. ap祀nd( "Wn"+e);

         }
         end() ; II should not be reached

    }

                                               - 118 -


===== PAGE 122 =====
    // 클라이언트 사용자로부터 메세지를 입력받아 서버로 전송

    public void act ionPer formed (Act ionEvent e) {
         if (e.getSourceO=Input) {
              // 서버로 전송
              Out.println(Narne+" --> "+Input.getTextO) ;
              0ut. flushO;
              II TextField 영역 삭제
              Input .setlext ( ") ;
         }
    }


    publicvoid end O{

    )
    public void closeStreams () {
         try {
              0ut.closeO;
              In .이ose();

          }
         catch (Except ione) {}
    }
}




                                          - 119 -


===== PAGE 123 =====
다음은 Chatting Client 를 App let 으로 작성한 예제이다．


[HTML I
<CENTER>
<APPLET NAME= "Chat App let " AR(HIVE="chat . jar " CODE="chat .ChatApp let . claSS'
WIIJIII="190" HEIGHF="81" ALIGN="刃VI川">
  <PARAM NAME="Server " VALUE= "서버주소 ">
  <PARAM NA｝肥＝"Port " VALUE="포트번호 " >
<IAPPLET>
</CENTER>


II Filename : ChatApplet. java

package chat;

import java.applet .半；

import Java.awt.*;

import java.awt.event.*;

import Java. io.*;

 import Java.net.*

public class ChatApplet extends Applet implementsActionListener {
    String server;

    mlt port;

    TextField Name;
    Button Connect;



    public void m1lit C) {
           setLayout (new Gr idLayout (O,1));
           add(new Label( "Name"));

           add(Namenew TextField( ") ) ;// 이름을 입력받기 위해

           add(Connect긔lew Button( "Connect "));

           Connect .addActionListener (this);

                                         - 120 -


===== PAGE 124 =====
    II HTML 로부터 <PARAM> 태그의 내용을 읽어온다．
    server=getPara配ter( "Server ");
    port可nteger .parselnt (getPara肥ter ( "Portt'));

}
public void actionPerfor附l (Act ionEvent e) {
     if (e.getSource0= Connect && !Na祀.getlext0.equals( ") )
       connect O;

}
public void connect () {

     try {
       II Socket 객체 생성
       Socket socket=new Socket (server,port);
       PrintWriter out=new PrintWriter( socket.get0utputStreainO);
       BufferedReader in=new BufferedReader (
                new InputStreamReader(socket .getlnputStream0) );
        // 이름 전송
       String na附Name.getText0;
       out .printin( "=== "+name) ;
       out. flush0;
       II ChattingWindow 를 생성한다．
       new ChatWindow(out, in,na肥) {
                publicvoid end () {
                       ci oseStreams0;

                 }
        }
     } catch (Exceptione) {II connectionproblern
       Systen.err.printin( "Connection to "+server+" at "+port+" failed. ");




                                      - 121 卞


===== PAGE 125 =====
6절 네트워크에서의 한글 및 다국어 처리

     문자 자료를 송수신할 때는 특정 문자 인코딩에 따른 바이트 형태의 변환
이 발생한다. 입출력에서의 문자 인코딩 처리 방법과 큰차이가 없으나, 네트워
크에서는 클라이언트, 서버간 통신 규약을 쉽게 변경시킬 수 없으므로 주의한
다．
     기존 응용 통신 규약을 준수하는 클라이언트, 서버를 작성할 경우, 기존 응
용 통신 규약에서 정한 문자 인코딩으로 변환한다. 인코딩에 대한 특별한 언
급이 없는 경우에는 클라이언트, 서버가 사용되는 환경의 디폴트 인코딩으로
변환한다．


     새로운 통신 규약 및 클라이언트, 서버를 작성할 경우, 가능하면 유니코드
류의 인코딩 (Unicode, UTF出, （수정된） UTF-미으로 변환하여 송수신한다．


     인코딩 변환 방법


     DataOutputStream의 writeUTFO, DatalnputStream의 readUTF() 메
     서드 및 0너ectOutputStream의 \write0너ectO, 0너ectlnputStream의
     read아）托ct(）는 수정된 UTF田 인코딩을 사용하여 변환한다．
     InputStreamReader, 0utputStream쨔iter, String 클래스의 생성자 및
     String의 getBytes() 메서드는 인코딩 이름을 인자로 가질 수 있다．


     유니코드를 고려하여 작성되지 않은 패키지는 스트링의 유니코드값을 잘못
     처리하는 경우가 있으므로 이러한 경우, 다음 함수를 사용하여 바로잡아
     사용한다．


     잘못 표현된 스트링을 유니코드 한글 코드값의 스트링으로 변환해주는 메
     서드

                               - 122 -


===== PAGE 126 =====
           public static String toHangul ( String str )

                           throws java. io .UnsupportedEncodingExcept ion
                                                                            {
                  if ( str == null )
                       return null ;
                 return new String( str.getBytes('"8859_i "), "KSC
                                                                       5Qi ) ;
           }

 유니코드 한글 코드값으로 표현된 스트링을 잘못
                                                      표현된 스트링으로 변환
해주는 메서드 （한글 처리를 제대로 해주지 못하는
                                                    패키지에 스트링을 전달할
경우 사용）


       public static String fromHangul ( String str
                                                          )
                       throws java. io .UnsupportedEncodingExcept ion
                                                                        {
                 if ( str == null )
                      return null;
                 return new String( str. getBytes( "KSC5601'D, ?1885
                                                                    911! );
       }

 입출력시의 문자열 인코딩 규칙


  일반적으로 입출력（파일 , 화면, 키보드）이 수행되
                                                     는 시스템의 디폴트 코
 드셋을           점검하여   적용하기 때문에 반드시 설청해야 하는 것은
                                    아니치만
 시스템의 디폴트 코드셋 외에 다른 코드셋으로
                            인코딩하여 입출력하고
 자 하는 경우 일부 클래스에서 인코딩 규칙을
                          지정할 수 있다．


  예를
   iW 들면, new (InputStreamReader(System.in, "KSC
                                                       5601");
                new (OutputStreamWriter(System.out, "KSC
                                                         5601 ');




                                     - 123 -


===== PAGE 128 =====
   Iv장 R入/11 프로그래밍




            학 습 목 표

. R八/11 기술을 알게 된다．
·RMI 구현 관련 API를 점검하고 구현 방법을
 익힌다．




             - 125 小


===== PAGE 130 =====
] 절 개요

 앞장에서는 네트워크로 연결된 컴퓨터 사이에 데이터를 주고받기 위한 수
단으로 소켓 프로그래밍을 제공하였다. 그런데 소켓 프로그래밍은 데이터를
주고 받기 위해서 저차원적인 일들（네트워크 연결, 데이터를 주고받는 규약둥）
까지도 개발자가 일일이 코딩하여야 한다．


  보다 자연스럽게 네트워크상에서 분산처리를 수행하기 위해 RPC(Remote
Procedure Call）를 구현한다. 이것은 특정 프로그램이 네트워크로 연결된 다
른 컴퓨터에 있는 함수를 호출하고 그 결과 값을 반환받을 수 있도록 해준다．
RPC 는 마치 자신의 컴퓨터내에 존재하는 함수를 호출 하는 것과 마찬가지로
다른 컴퓨터내의 함수를 호출할 수 있기 때문에 소켓 프로그래밍보다 이해하
기도 쉽고 프로그래밍하기도 쉽다．


  Java 에서는 RPC의 장점을 살려 분산 객체 어플리케이션을 쉽게 만
들 수 있는 개념을 제시했는데 이것이 匙4塑르뜨얀으쓰哄쁘쁘vo드晙照？ 이
다. 분산 객체 어플리케이션이란 네트워크로 연결되어 있는 컴퓨터들의 객
체들이 서로간의 메서드를 호출하여 한 목표를 향해 동작하는 시스템을 의미
한다．




                     - 127 -


===== PAGE 131 =====
1.1 RMI 의 수행 흐름


  R코＼4' 서버（리모트 객체）와 RMI 클라이언트로 구분된다. RMI 서버란 리모
트에서도 참조 가능한 객체를 생성하고 등록하는 기능의 프로그램이며 R八1!
클라이언트란 리모트의 객체를 참조하여 필요한 기능을 분산 처리하려는 프로
그램이다．


  수행 흐름은 다음과 같다 :


   (1) RMI 서버가 리모트에서 접근 가능한 객체를 생성하고 RMIURL을 활용
     하여 RMIRegi stry 어］ 등록（rebind, bind）한다．


   (2) RMI 클라이언트는 참조하고자 하는 리모트 객체를 찾아(lookup)
     리모트 객체의 스텁（stub) 파일과 객체 정보묠 얻어온다．


   (3) 리모트 객체의 리모트에서 호출 가능한 메서드를 호출한다．
      이 때에는 클라이언트의 스텁 파일이 서버의 스켈레턴（skeleton）파일
      에게 호출 정보를 전달한다．


   (4) 결과를 받는다．
      이 때에는 서버의 스켈레턴이 클라이언트의 스텁에게 전달한다．




                           - 128 小


===== PAGE 132 =====
1.2 RMI 구축의 장점과 단점


 卜 장점
   e 다른 Java Virtual 入4achine 어］ 있는 객체땍 메서드를 자신의 \Tirtual
     Machine 어］ 있는 로컬 깩체의 것을 호출하는 것처럼 쉽게 호출할 수
     있다．


   e 일반적인 분산 객치：1 모델（C아之BA 등）을 Java 언어의 객체1 활용 방법
     어］ 큰 영향 없이 Java 언어에 도입한다．


   1 오류 없는 분산 어플리케이션을 되도록 쉽게 만들 수 있다．


   - Java 언어가 제공하는 보안 관련 정책을 그대로 적용한다．


 卜 단점


   小 리모트의 객체뻬 대한 참조를 찾고 얻어내는 시간이 오래 걸리고
    전반적인 수행 속도가 Socket 으로 구현한 프로그램보다 느리다．


   中 메서드 호출（매개변수, 리턴값） 이라는 기술이 지원하는 기능외에는
    다양한 프로토콜을 적용하기 어렵다．




                         - 129 -


===== PAGE 133 =====
1.3 RMI 프로그리1밍 관련 API


  java.rmi


   원격 객체1 이름에 접근하기 위한 Remote 인터페이스 , Naming 클래스
   Marshal ledObject클래스 그리고 RMI 보안 관리자를 제공한다．


  java.rmi .registry


    원격 레지스트리에 의해 사용되는 클래스와 인터페이스를 제공한다．


  java.rmi .server


    원격 객체 , 스텁 그리고 스켈레턴을 구현하고 'RMI 통신을 제공하기 위한
    클래스와 인터페이스를 제공한다．


  java.rmi .activation


    JDK 1.2 어］ 추가된 새로운 R八'II 패키지이다. 필요한 원격 객체를 활성화
    시키거나 지속적인 객체 참조를 처리하기 위한 기능을 제공한다．


  java.rmi .dgc


    R1viI 분산 가비지 수집 기능에서 사용되는 인터페이스와 클래스를 제
    공한다．




                         - 130 小


===== PAGE 134 =====
1.4 RMI 관련 명령


  R｝匹I 수행과 관련된 명령은 다음과 같이 3개이다．


   rmic
                  'II／刃／c2／모트 캑체으／ 클래스 0／름"
                  리모트 인터페이스를 구현한 리모트 객체의 스터브 , 스켈리턴
                  파일을 생성한다. 스텁 , 스켈리턴 파일은 각각 " 리모트 객체
                  의 클래스이름-s加b .이ass " 오F "리모트 객체의 클래스이름e
                  Skel .이ass" 로 만들어진다．


   rm iregistry
                  UNIX: rmiregistry&        Win 95/NT: start rmiregistry
                  네임 서버 역할의 프로그램을 백그라운드로 수행시킨다. 디폴
                  트로 포트 번호 1099 를 통하1 클라이언트의 요청을 받는다．
                  다른 포트 번호로 동작하도록 하려면 rmireg治try 포트 번호
                  를 수행시킨다．


   rmid
                  UNIX: rmid&          Win 95/NT: start rmid
                  원격 객체를 활성화 시켜주는 원격 활성 시스템 데몬을 기동
                  시 킨 다．




                                  - 131 -


===== PAGE 135 =====
2절 R卜＼사 프로그래밍

 RMI 프로그래밍은 리모트 객체를 생성하고 등록하는 기능의 RMI 서버와
이 객체믈 참조하는 기능의 RMI 클라이언트를 주어진 API 들을 활용하여 다
음 순서로 구현한다．


  1. 리모트 클래스를 생성한다．
   2. 리모트 객체를 생성하고 등록시키는 RMI 서버 프로그램을 생성한다．
   3. 리모트 객체를 참조하여 메서드를 호출하는 R八'II 클라이언트 프로그
    램을 생성한다．




                   - 132 尸


===== PAGE 136 =====
2.1 리모트 클래스（Rem아e 이ass）의 생성


  리모트 객체란 네트워크로 연결된 다른 Java VM으로부터 호춤될 수 있
는 메서드가 존재하는 객처屠 말한다. 한 개 이상의 리모트 인터페이스를 구
현하고 있는 객체로서 리모트 인터페이스에는 리모트에서 호출 가능한 메서드
들을 정의하는 추상자료형이다．


  그러므로 리모트 객체는 이 인터페이스를 상속하여 R入'II 를 통해 호출되는
메서드의 코드를 정의한다．


  (1) 리모트 인터페이스의 정의


   ] . 리모트 인터페이스는 접근 권한이 口ub比 이어야 한다．
   2. java.rmi.Remo也 를 반드시 상속받아야 한다．
   3 . 리모트 인터페이스에 정의한 모든 메서드들은 Rem아eExce口tion 을
       throws 하고 있어야 한다．


            public interlace g吝' extends java.rmi.Remote {


            }


  예）
        public interface Hello extends java.rmi.Remote {
             String sayHeflo() throws java. rm i .RemoteException;
        }




                               - 133 -


===== PAGE 137 =====
(2) 리모트 인터페이스를 상속하는 클래스


 ] . 리모트 인터페이스를 상속받아 구현하여야 한다．
 2. RemoteExce아ion 을 throws 하는 생성자 메서드를 정의한다．
 3. UnicastRem이eOb忙Ct 클래스를 상속한다．


         class 명칭 extends UnicastRein oteObject
                                impl m ents Remotelnterface{


         }


예）

 public class Hellolmpl extends UnicastRemoteObject
                                         implements Hello {
     private String name;
     public Hellolmpl(String s) throws RemoteException {
          name = s;
     }
     public String sayHello() throws RemoteException {
          return name + II극卜川 Server !!";
     }
 }




                             - 134 -


===== PAGE 138 =====
2.2 리모트 객처屠 생성하고 등록하는 RMI 서버의 생성


 리모트 클래스를 객체 생성하고 Naming 클래스의 다음 메서드를 활용하여
 RMlRegistry 에 등록한다．


       趨쁘V쁘如世（String name, Remo旭 obj)
            지정된 name으로 ob屠 등록한다．
            이미 동일 name으로 등록된 객체가 존재하는 경우어七
             AireadyBoundExce口tion이 발생한다．


       static 쁘브r쁘끄궷鈿ng name, Remote obj)
             지정된 name 으로 obj 를 등록한다．
             이미 동일 name으로 등록된 객체카 존재하는 경우에는 기존
             것을 제거하고 등록한다．


   위에서 name 은 RMI URL 로서 다음과 같은 형식으로 정의한다：


       rmi刃서버주소：포트번호／객체에 대한 별칭


   Naming 클래스에는 등록되는 리모드 객체와 관련된 다음 메서드들을 저1
   공한다：


       static String[ ] Iist(String name)
       static Remote Iookup(String name)
       static void unbind(String name)


  예）
             HeUolmpl obj = new Hellolmpl("Hello");
             Naming .rebind("rmi:/I         /HefloServer", obi);
             System.out.println("HelloServer bound in registry');
                               - 135 -


===== PAGE 139 =====
2.3 리모트 객처屠 챰조하는 RMI 클라이언트 생성


   Naming 클래스의 幻oku口（) 메서드를 활용한다．


      static Remote Iookup(String name)
           name 는 참조하고자 하는 리모트 객체의 RMI URL 을 지정
           한다. 이 명칭으로 등록된 객체가 없는 경우어七
             아BoundExc야川on 이 발생된다．



      String un1 ="rmi://         /HelloServer";
      Hello obj = (Hello)NamingJookup(url);
      String s = obj.sayHelloO;
      System .out.println(s);




                                - 136 中


===== PAGE 140 =====
[ 예제 十1 : 리모트 객체 참조 예제 (Application)]


  RMI 서버가 리모트 클래스인 H이loIn叩l 을 객체 생성하여 등록하면 RMI
클라이언트는 sayHello() 를 호출하는 예제이다. 클라이언트가 A미沅ation 인
경우이다．


  // 리모트 인터페이스
                                                                            , ,械꺼 , \,F타 mWt卜쿄4 짚亡학 겟인寸미 어하．
  II Filename : He! lo. java
  " . . . ' ".'"'"" ', "" ",. ".'." " ' "． , . 叭"'1 『 " '. ． 比1悅亢e甁蚣，硯섭
  DUD! IC interracejie! !O exienas java.rmi.iiemoie 1.
      ,

          ar 1唯艱y/覡므O푄 [nrows java.rmi.Ie咀
                                         1I   ,       't   S I

                                         （兀enxcept ion,
              .   -   .    I   /／二iT1l            A               .     .   fl   .   r '




  }


  // 리모트 클래스
  II Filename : He! !olmpl. java
  import java.rmi.*;
  import java.rmi .server.UnicastRnote力ject;
  public class Hellolmpi extends UnicastRemoteObject implements Hello {
      private String name;
      public Hellol町）l (Stri띵 s) throws Re咀）teExcept ion {
                          name = 5;

          }
      public String sayflelloO throws Re咀）teException {
                          return name + "RMI Server ! !";

      }
  }



                                                                 m挺" 戚 싸1'w1"써“Lt. RM냐 ' 灘니' 「牡咀
                                                                  ' 抑' "니'b t' "七

                                                                      - 137 -


===== PAGE 141 =====
     // 서버
     II Filename : RMlServer. java
     import java.rmi. 水;
     public class RMlServer{
          public static void main(String args[ ]) {
                 if (Systan.getS兀urityManager() == null) {                   少斗；
                         Syst帥.setSecurityManager (new RMISecurityManag斫());

                     }                    낳y   "泉O.    ．   黔·
                     try {                            ,介 “

                                                                            m , m，朴d吃t
                                         單令球如
                                     m


      .       . ., Hellolmpl cbj = new Hellolmpl("Hello"

쁘恥
      L伊V肝해시
              八1母빠ng·高b비"rm川／"+args[O］두"/HelI。S毗『", 命j); 쓰1二：1/
              F뇩＼\                                                                   '
                         Syst帥.out.println( "flelloServer bound in registry!!);
                     } catch (Except ione) {
                         System.out.println( "Hellolmpl err: " + e) ;
                     }
          }
     }


     // 클라이언트
     II Filename : RMIClient. java
     import java.rrni .*;
     public class RMlClient {
          public static void main(String args[ ]) {

                     try {
                         String un =" rmi://"+args[O]+"/HelloServer";
                         Hello obj = (Hello)Naming.lookup(url);
                         System.out .println( "HelloServer Find. . . 1!);
                         String message = obj. sayHelloO;
                         System, out .pr mnt ln(message) ;
                     } catch (Exceptione) {

                                                       - 138 -


===== PAGE 142 =====
              Systdn.out.print1n( "He11o exception: " +e.getMessageO);

          }
      }
  }



2.4 RMI 서버와 클라이언트의 수행


 모든 소스를 컴파일한 후 다음 순서로 수행시킨다．


      (1) 리모트 클래스의 슷旦쓴竺렛덮크브邑雙竺한다·

          rmic Hellolmpi         和苞 加呱式， 缸玎川 叩t            아比/ 나d仰       사b杞．


      (2) rmiregistry ［포트번호］ 를 기동시킨다．
                                                  耐叫袖穹 ＞多"匕
          rmiregistry 邑    U小艾
          start rmiregistry 汕砧9山9.


      (3) Client 가 Application 인 경우 스텁 파일을 클라이언트로 . 복사한다．


      (4) 서버 프로그램을 기동시킨다．


          java RMlServer


      (5) 클라이언트 프로그램을 기동시킨다．


          java RM兀lient



                                   - 139 -


===== PAGE 143 =====
卜 rmic 에 의해 생성되는 스텁／스켈레턴 파일의 내용중 일부이다．


Compiled from He11oI昨1_Sel. java
public final class He11oImpI_ ;el extends java. lang.幽ject
                                               implements java.rmi .server. celeton {

     public java.rmi.server.Operation get(IberationsO[ ];
     public void dispatch(java.rmi.Reriote, java.rmi.server.Re1oteCa1l, int, long)
                           throws j ava.rmi .RenoteExcept ion, java. lang.Except i0n

     public Hellol叩i_SkelO;
     static {};

}


Compiled from Hellol耳）l_Stub. java
public final class llellolmpl_Stub extends java.rmi .server.RemoteStub
                                               implementsHello, java.rmi.Remote {

     public Hellolmpl_StubO;
     public Hellol昨l_Stub(java.rmi .server.RmoteRef);
     public java. la坦.String sayHelloO throws java.rmi.RemoteException;
     static {};

 }




                                     - 140 -


===== PAGE 144 =====
[ 예제 2吃 : 리모트 객체 참조 예제 (Applet)]


  RMI 서버가 리모트 클래스인 Hello노叩l 을 객체 생성하여 등록하면 RMI
클라이언트는 sayHello() 를 호출하는 예제이다. 클라이언트가 Applet 인 경
우이다．


 II Filename : HelloApplet. java
  import java.awt.*;
  import java.rmi.*;
 public class HelloApplet extends java.applet.Applet {
     String message= "RMI Fail ";
     public void init () {

          try {
              Hello obj = (Hello)Naming.lookup("rmi://"+

                       getCodeBase().getHostO+"r . .)./HeIloServer");
              message = obj.sayHelloO;                ＼諦娘’
          } catch (Except ione) {
              System.out.println( "llelloApplet exception: " + e.getMessageO);
              e . pr intStacklraceO;
          }
     }


     public void paint (Graphics g) {
          g .（打awStrii退（毗ssage , 25 , 20) ;
     }
 }




                                       卞 141 -


===== PAGE 145 =====
3절 객체 직렬화

3.1 객체 직렬화란？


 객체 직렬화（0b把Ct Serialization）란 객체 정보를 기본형 데이터（변수, 상
수）와 같이 입출력할 수 있도록 갤첸겅보를 바이트1型꽤－로1쇌환사짜             하
는 것을 의미한다·       마＜跆 ., 빡知씌 변建    b包드띄르   ''I쟁．

            m ,, : 츨쩍횐 뗘器 읽cli 勃庄 생셩능卜듣 李m
 특정 클래스의 객체가 직렬화되려면（스트림으로 변환되어 I/o되려면） 반드

                   旦쯔빳힌換브느인터페이스를 구현해
시 그 클래스는 旭쁘些旦旦궷受奭e巴，
야 한다.                    \
                         L+ 려 이오（0比   시雖h卜 影t능

  JDK 1.1 부터 객체 직렬화가 목적은 기본 데이터 타입 내용 뿐만 아니라
참조형 변수의 내용까지도 저장할 수 있도록 하여 분산 환경에서 메세지 전달
유형을 참조형까지 가능하도록 하는데 있다．


  Serializable 인터페이스를 구현한 클래스의 객체는 개발자가 별다른 코드
의 정의 없이 자동으로 객체를 저장하고 읽을 수 있다. Externalizable 인터페
이스를 구현한 클래스의 객체는 개발자가 반드시 객체의 상태를 저장하고 읽
는 메소드를 정의해야 저장되고 읽을 수 있다．


  객체 직렬화의 활용 예


  m 사용자가 변경한 Java 빈 컴포넌트를 하드 디스크에 저장하고 나중에
   그 컴포넌트를 읽어서 사용할 수 있다．


  -R八'II 메서드를 통하여 객체를 네트워크로 이동할 수 있다. 즉 R八'II 메
   서드의 반환값이나 매개변수로서 객체가 사용될 때 , 그 객체들은 스트림
   화되어 네트워크로 이동한다．

                       - 142 尸·


===== PAGE 146 =====
3.2 객처1 직렬화 관련 API


  객체 직렬화와 관련 API는 많지 않다. 직렬화가 가능한 클래스를 생성하려
는 경우에는 일반적으로 Serializable을 상속하며 , 직렬화시켜 입출력하는 기
능의 메서드는 각각 ObjectlnputStream 클래스와 ObjectOutputStream 클래
스에서 제공된다．


  java.io.ObjectOuptput 인터 페 이스
  java.io.Objectlnput 인터 페 이 스
  java.io.Serializab沌 인E任如1스
  java.io.Externalizable 인터 페 이 스
  java.io.ObjectOutputStream 클래스           T 1)如I씨싸Q妃胛
        void write아朮ct(O可ect)
                                           L b加0印毗S「加胛
  java.io.ObjectlnputStream 클래스
        Object read아万ect()




                                 - 143 -


===== PAGE 147 =====
3.3 객체 직렬화 구현 과정
      : 긱쳬 t휄버 변수帥갬    哮생．

  m 객체를 출력 스트림화하여 저장하는방법
   다음은 Date 클래스를 " tmp" 라는 파일어4 저장하는 예제이다．


   FileOutputStream out = new FileOutputStream( "tmp");
   ObjectOutput s = new ObjectOutputStream(out);
   s.write아加ctC'Today");
   s.writeObject(new DateO);




  e 객체를 입력 스트림화하여 읽는 방법
   다음은 하드 디스크에 저장되어 있는 객체를 읽어서 생성하는 예제이다．
   FilelnputStream in = new FilelnputStream("tmp");
   Objectlnput s = new ObjectlnputStream(in);
   String today = (String)s.readObjectO;
   Date date = (Date)s.readObjectO;




                               - 144 -


===== PAGE 148 =====
[ 예제 3-1 깩체 정보를 직렬화하여 파일에 저장하는 예제 ]


 test.tmp라는 파일을 출력모드로 오픈하여 객체 정보를 직렬화하여 저장한
후 다시 읽어 화면에 표준 출력하는 예제이다．


 II Filename : SerialTest. java
 import java. io.*;
 import java.util.*;
 public class Seriallest {
   public static void main(String args[ ]) {

         try {
            File뇨tputStream ostream = new Fi1e뇨tputStream(!test.t旺）h!);
            // 출력 모드로 오픈된 파일어］ 객체 출력 필터를 연결한다.

            0히ect0u自JtStream 口 = new 0히e야0u巾utStrea呵ostream);
            p.writelnt(12345);
           p.wri旭Ob旭ct("Today");
           p.writeobject(new DateO);
           p.writeObject(new Test(100));
           p. flushO;
           ostream.closeO;


           Fi lelnputStream istream = new Fi lelnputStream( "test. tmp");
           /／입력모드로 오픈된 파일어］ 객체 입력 필터를 연결한다．

           Object InputStre帥 q = new Object InputStream(istream);
            m1lt i = q.readlntO;
           Systeri.out .println(i) ;
           /／바이트 단위로 저장되었던 객체 정보를 읽어 화면에 표준 출력한다.

           String today = (String)q.readObjectO;
           Systan.out .print ln(today) ;
           Date date = (Date)q.rea어：)jectO;

                                       - 145 -


===== PAGE 149 =====
            Systen.out .println(date);

            Test t = (Test)q.rea10bject0;

            t. pr () ;

            istream.closeO;

           catch (Except ione) {

            Systen.out .println(e);



    }
}


/／객체 직렬화 테스트용으로 Serializable을 구현하는 클래스를 생성한다．

II Filename : Test. java

public class Test implements java.io.Serializable {

    public m1lt su;
    public Test (int su) { this. su= su; }

    publicvoidpr () {

        System.out.println( "This is test () method in Test class") ;

    }
}




                                      - 146 尸


===== PAGE 150 =====
3.4 transient 의 활용


  객체 저장시에는 그 깩체의 모든 상태들（멤버 변수의 내용）이 저장된다．
특별히 저장하고 싶지 않은 델벗갔歪잿한立코웃엔늪뽀브뽀얻산廻쁘恥r
                                     " 저장
론므赳延쁘量뽀겅한다· 그러면 ' ] 속성으로 저장된 멤버 변수는 객카
시에 저장되지 않는다．


[ 예제 3-2 Serializable 점검 예제 ]


  객체 직렬화시 처리되는 transient Modifier어］ 대하여 점검하는 예제이다．
일반 멤버 변수는 직렬화되어 파일어］ 저장되는 반면 transient 멤버변수는 저
장되지 않는 것을 확인할 수 있다．


  II Filename : lransientTest. java

   import java. io.*;

  public class TransientTest {
     public static void main(Stri退 args[1) {

           try {
              Fi le뇨tputStream sami = new Fi le沁tputStream( "sa旺）le. tmp");

              Object1ttputStream p = new ObjectXitputStream(sam1) ;

              SerialSample firstss= new SerialSa旺）leO;

              Systdi.out.println( "Write Object ! !") ;

              Systemout.println( "a : " + firstss.a);

              System.out.println( "b : " + firstss.b);

              System.out.println(Tc : " + firstss.c) ;

              firstss.testO;

              p . write(兀ject (new Ser治lSa呱)le());

              // 출력 버퍼를 clear 한다．

              p. f1ushO ;
              saml.c1oseO;
                                      - 147 -


===== PAGE 151 =====
             FilelnputStream sam2 = new FilelnputStream( "sample. tmp");
             Object InputStream q = new Object InputStream(sam2);
             SerialSa旺）le secondss = (SerialSa町：)le)q.read力jectO;
             Systen.out.println( "Read Object ! !") ;
             Systdn.out.print1n( "a : " + secondss.a);
             Systeii.out.printlnC'b : " + secondss.b);
             Syste.out.print1n( "c : " + secondss.c);
              secondss. testO;
              sam2.closeO;
         } catch (Except ione) {
             Systan.out .pr mnt ln(e);

         }
    }
}


II Filename : SerialSa耳）le. java
class SerialSa叩le implements Serializable {
    m1lt a = 10;
    m1lt b = 20;
    transient m1lt c = 30; // 직렬화시 생략된다．
    void test () {
         Syst帥.out.println( "a : "+a+" b          "+b+" c :   "   +C) ;

    }
}




                                         m148 -


===== PAGE 152 =====
3.5 객처1 직렬화와（雨i , 小 , ,,H내뀨갸 ）學1악펼目
                    \/    켜 二기        ,   ,'..,   r, "',,"．戶．시，
                                                              " '」   t4- 小' d'八K각"   났꺼 負 ' .1 .
                                 의 /qc l,'1 eVV"T "' "'              " "         "
  다음에 제시된 예제를 점검해보고 객체직렬화 기능이 R入'II에서 필요한 이
유를 점검하1 본다．


[ 예제 十3 Serializable 점검 RMI 예제 ]


  RMI 와 객체 직렬화의 관계를 점검해 보는 예제이다．


  // 리모트 인터페이스

  II Filename : RMISeria1. java

  import java.rmi .*;

  public interface RMISerial extends Remote {

      String getStri召() throws RemoteExcept ion;

      chart] g앉血必Yi) throws Re以）teExcept ion;
      Unico getUnico() throws RemoteExcept ion;
           ／入小小／／小八



  }

  // 리모트 객체를 기동시키는 서버

  II Filename : RMlSeriallmpl. java

  import java.rmi.*;

  import java.rmi .registry.*;

  import java.rmi .server.UnicastRemote力ject;

  public class RMlSeriall叩l extends UnicastRemoteObject implements RMISerial{

      public RMI＆才iall町)l () throws Re瞰亢eExcept沁n {

      }


      public String getString() throws RemoteException {
           return " 가나다라！! " ;

      }

                                          - 149 卞


===== PAGE 153 =====
    public charM getArray() throws RemoteException {

         returnnew char[ I { 'a' , 'b' , 'c ' , 'd'} ;

    }                                                         P小4h,（닯 ' 0) :
                                                                     出쳬의 bg七 ‘"斗派t뇨斌圭
    public Unico getUnicoO throws RenioteException {                  4如枓 겅e냑 kt小'n
          return new Unico( "This is Unico Class") ;                     4H 甘唯 뎌煎
    }


    public static void main(String args[ }) {

         m1lt num = Integer.parselnt (args[OD;

         i f (Systern.getSecur i tyManagerO null)

             System. setSecurityManager (new RMlSecurityManagerO);

         try {
             LocateRegistry.createRegistry(num)                   江t다． 7‘掘 唯

             RMlSeriall町）l obj = new RMlSeriallmplO;

             Nami띵.rebind( "rnii :1/.            "+n丑+"/TestServer ", obj) ;

             Systeri.out.println( "lestServer bound in registry");

         } catch (Except ione) {

             System.out.println( "llellolmpl err: " + e. getMessageO);

             e . printStackTraceO;

         }
    }
}




                                           - 150 -


===== PAGE 154 =====
    // 리모트 객체의 메서드를 호출하는 클라이언트

II Filename : RMlSerialClient. java
    import java.awt.*;
    import java.rmi.*;
public class RMlSerialClient{
         public static void main(Stri追 args[ ]) {

              try {
                  RMISerial obj = (RMlS玎ial) java.rmi.Nami追. lookup(

                                          "rmi: // " +argS[0]+ " : " +argS[l] +" /TeStSerVer " );
                  System.out.println("String : "+obj.getString0);
                  System.out.println("charEl: "+obj.getArray0);
                  System.out.println("Unico: "+obj.getunico0);
              } catch (Except lone) {
                  Systen.out.println( "exception: " + e) ;
                  e . printStackTraceO;
              }
         }
}


// 추가 클래스（Serializable（직렬화）이 가능한 . . )
II filename : Unico. java
public class Unico implements java.io.Serializable(
      String str;
      public Unico(Stri也 s) {
                                                                               『A肯勻 的"丸 '＼켜比·
             str=5 ;                  ，분싸噴읔 畦.：윽는 가心                          七Q
     }
     public String toStringO{                ':' d rDl屯 孕t唵이         거笞 , 2러냐 Ytb,' m읕              학 수獻包므玄
             return "Test : n + str;                냐牡드          9苗（h＞凡t그en；늉 ？肛婉끼 觀 .
      }
}

                                             - 151 小

             1 버契       ' 健＼咤        찍勻茗卜＞
                                         卜 .晤．


===== PAGE 155 =====
4 절 R入사 CallBack

  RMJ 클라이언트가 R入4' 서버의 메서드를 호출하면 그 결과가 올때까지 대
기하고 있어야 한다. 이 때 클라이언트는 서버로부터 반환값을 가지고 복귀될
때까지 블럭킹 상태로 있게된다. 이러한 상태를 해결하려면, 스레드를 하나 더
기동시켜 수행시키거나, 서버에서 클라이언트의 메서드를 호출하는 콜백
(Callback) 기능을 구현하여 해결할 수 있다．


  RMI 프로그래밍에서의 콜백 기능 구현은 생각보다 간단하다. 클라이언트
도 리모트 인터페이스를 상속하고 리모트에서 호출 가능하도록 원격 객체로
    귀   a버 ] 이 객체 정보를 전달하면 된다. 스켈레턴과 스텁은 서버와
클라이언트에 각각 생성한다．



           Interface                                                                       Interface
                Hi                                                                             Hello
           send(string)
                                                                     /／戶mmmbm+

                                                       ///
                                                                                       sayHello(Hi)
                                  S%.   . /"                                          \\

                                  ./／人＼\

                                               \

     RM1 Client (HelloApplet)-"                    \
                                                        \
                                                             \
                                                                 \
                                                                                  RMI Server (Helloimpi)
                                                                     \

     Hi 를 상속                                                             \
                                                                             'S   H이幻를 상속




   구현 순서 :


        - Hello, Hi, CalibackApplet, Hell아mpl 을 작성한다．
        H 각 클래스에 대한 스텁과 스켈레턴 파일을 생성한다. (rmic)
        小 R八4lRegistry 를 기동시킨다．
        - Hellolmpi 을 기동시킨다．
        - appletviewer 또는 브라우저로 CalibackApplet 을 기동시킨다．




                                        尸 152 -


===== PAGE 156 =====
4.1 구현 내용


   Hello노叩1 (RMI 객체 클래스이면서 서버 클래스）의 주요 구현 내용


   - UnicastRemote0bject 를 상속받는다．
   U 인터페이스 Hello 를 상속받는다．
   - sayHel幻（Hi) 메서드로 Hi 인터페이스 유형의 객체를 전달받는다．
   - Hi 형 객체의 send(String) 메서드를 （주기적으로）호출하는 스레드를
     기동시킨다．
   - HelloIm이 객체를 정해진 RMl URL 과 t키nd 한다．


   CallbackApplet(Client）의 주요 구현 내용


   - UnicastRem아e0b旭Ct 를 상속받는다．
     (Applet으J 경우 UnicastRemo旭O히ect.exportO히ect(Rem아e) 호출）
   尸 인터페이스 Hi 를 상속받는다．
   m 주어진 RMI URL 을 이용하여 리모트 객체를 lookup 한다．
   - Hello 유형의 객체를 얻어낸뒨 sayHello(Hi) 메서드를 호출하여 자신
     에 대한 객체 정보를 서버에 전달하여 서버가 참조할 수 있도록 한다．




   RMI Client            RMI Server         RMI Client          RMI Server
                J




                           卜
            method 호출                                    method 호출

 대기상태




        1           」」
                                                     method 호출



      Callback 기능이 없는 RMl                     Ca比ack 기능이 구현된 RMI




                                  - 153 中


===== PAGE 157 =====
[ 예제 4-1 RMI Callback 예제 ]

  RMI 클라이언트가 RMI 서버의 리모트 메서드 호출시 자신의 객체 정보를
전달하여 서버에서 클라이언트의 리모트에서 호출 가능한 메서드인 send() 를
주기적으로 호출하는 예제로서 서버와 클라이언트가 모두 리모트 객체로 활용
된다．


  [ Server I



  II Filename : Hello. java

  public interfaceHello extends java.rmi.Re炚）te {

      public String sayHello(Hi h) throws java.rmLReiioteException;

  }


 II Hellolmpljava
  import java.rmi.*;

  import j ava.rmi .server.UnicastRemote兀ject;

 public class Hellolinpi extends UnicastRanoteObject implementsllello, Runnable {

      private String name;
      Hi remoteobj ;

      Thread t;



      public llellol町）l (Stri띵 s) throws RemoteException {

           superO;
           name = S ;

      }


      public String sayHello(Hi obj) throws Re以）teException {

           remoteobj = obj ;

           t = new Thread(this);

           t. start ();
                                     - 154 -


===== PAGE 158 =====
     return name;

}


public void run() {

     for (mlt i=O; i < 7; j++) {

         try {

             remoteobj . send( "Cal Iback Test ");

             Thread. sleep(5000);
         } catch (Exceptione) {

             System.out .println(e);
         }
     }
}


public static void main(Stri垠 args[ ]) {

     try {

         Hellolmplobj = new HelIoI旺）l ( "HelloServer ");
         Nami召.rebind( "rmi ://"+args[ O}+"/Hel loS三rver ", obj) ;

         System.out.println( "llelloServer bound in registry");
     } catch (Except ione) {
                                                                     탁八 .
         " printStackTraceO;                         和小肖   奴刊   "




                    d) 巾mtC                                   (M "1"        y＼二
                                                     好b ( 斛 伊6
                    닉@ ，싸스  ’사" U 附鉀
                       ' '""和附叫   ' 「“
                                     ' "『 t " V\, \'뇨＼
                                                     '
                                               小，,5,"n
                  이 저버 "悟
                  @ cta 佩


                                 - 155 -


===== PAGE 159 =====
[ 클라이언트 ]



II Filename : Hi. java

public interfaceHi extends java.rmi.Reote {

    public void send(Stri띵 s) throws java.rmi.RenoteExcepti丑l;

}


II Filename : HelloApplet. java

import java.awt.*;

import java.rmi.*;

import java.rmi.server.*;

public class HelloApplet extends java.applet.Applet implementsHi{

    String message = "initial ";
    m1lt x = 20;

    mlt y = 30;

    public void init () {
                                                            ＼毛뽀d欠e
         try {
           (UnicastRemoteObject.exportObject(this)1,

              Hello obj = (Hello)Nami띵. lo斗：up( "//" +

                         getCodeBaseO.getHostO+": . . . ./HelloServer ");

              肛雙塑旦三쨘4與y볜트쁘世蛭）;
          } catch (Except ione) {

              Systaii.out.print1n( "HelloApplet exception: " + e.getMessageO) ;

              e .printStackTraceO;

              message=e. toStringO;

          }
     }

     public void send(String s) {

          message = s;

                                       - 156 中


===== PAGE 160 =====
          x += 15; y += 15;
          repaintO;
    }


    public void update(Graphics g) {
          paint (g) ;
    }


    public void paint (Graphics g) {
          g. drawString(毗ssage, x, y);
    }
}


m 모튼 파일 컴파일
- rmic Hellolmpi, rmic HelloApplet
- html 작성 : width=350 height=350
- ap이etviewer 또는 브라우저로 점검



                              dk,d도      仰tA " 乏 " 悟 ,
        乂 竅w可별냔 刑I卜 ‘




                                  - 157 -


===== PAGE 161 =====
[Java Plugin 으로 He iloApj月et 을 호출하는 HTML 파일의 내용 ]


 ．尸-Hel loApplet 를 호출하는 HTML 파일（Java Plugin) -中＞
<!
<html>

<head>
<t itle>Hello applet</titie>
</head>

<body>
<hl>Hel lo appiet</hl>
애플릿의 소스 코드는＜a href='TllelloApplet . java'Sflell아如아et .java<Ia>
를 참조하십시오．. . .
<hr>
< ! m尸nq씨V日汀可) 肛耳) 』gffl_>
<!-- CONVERTER VERSION 1.0 -->
<OBJECT ci ass id="clsid:8AD9C840-044E-11D1-B3E9山080邸4的D93"
WIDTH = 500 HEIGHT = 200 codebase="http: //java.sun.cani/products/pl坦inh1.2/
j install-12-win32.cab#Version=1,2,O,O">
<PARAM NAME = CODE VALUE = "HelloApplet ' >
<PARAM NAME = CODEBASE VALUE = ". '1 >
<PARAM NAME="ty思" VALUE="applicat ion/x-java-applet ;version=1.2">
<COMMENT>
<EMBED type="appiicat ion!x-java-applet ;version=1.2" java_CODE = "lleiloApplet "
java_01屯BASE = ". "      WIDTH = 500 HEIGHT = 200   pi평inspage="http: //java.sun.
corn/products加it壕n/i. 2/pit坦in너nstai 1 .html "＞싻別I霓［></(1刈旺N1
</Nc BFB</EMBED>
</OBJECT>
< ! -"END （分寸珏玉江印머PPu江"中＞




                                    - 158 -


===== PAGE 162 =====
5절 R＼사 소스 분석

 다음은 RMI 로 구현한 Chatting 소스이다. 메세지 전송 방식이 Socket 보
다 간단하게 구현되어 있다．


 II Filename : ChatServer. java

 import java.rrni .*

 public interface ChatServer extends Remote {

     public void broadcastMessage(Stri띵 message) throws RemoteExcept ion;

     public void addClient (ChatClient client) throws Re以）teException;

     public void deleteClient (ChatClient client) throws Re以）teException;

 }

 II Chatting서버로의 기능을 내장하는 서블릿이다 . 리모트 객체로 통작한다．

 II Filename : RMlChatServer. java

 import java. io.*;

 import java.net.*;
 import java.rmi.*;

 import java.util. *;

 import java.rmi.server.*;

 public class RMlChatServer extends UnicastRemote力ject implements ChatServer {
     //RMI 으로 연결되는 클라이언트를 Vector 로 처리한다．

     Vector rmiClients = new Vector () ;



     public RMlChatServer() throws RemoteException {}



     public void broadcastMessage(Stri평 message) {
          // RMI 로 연결되어 있는 모든 클라이언트들에게 메세지를 리턴한다．

          Enumerat ion enum = rmiClients.elementsO;

          while (enum.has砥areElenentsO) {

                                     - 159 -


===== PAGE 163 =====
            ChatClientchatClient = null;

            try {
                chatClient = (ChatClient)en皿i.nextE16nentO;
                chatCi ient . setNextMessage(message);

            }
            catch (RaiioteException e) {
                Systeii.out .pr mnt ln( "跳lETE CLIENT");
                deleteCi ient (chatCl ient);

            }
        }
    }


public void addClient (ChatClient client) {
        rmiCl ients.addEl帥ent (client);

}

public void deleteClient (ChatClient client) {
        rmiClients.rdnoveEl帥ent (cl ient);

}

public static void main(String args[ II) {
        if (Systdn.getSecurityManager() == null) {
            Syst跏.setSecurityManager (new RMlSecurityManagerO);
        }
        try {

            RMIChat驍"' "" obj『 "톈쁘心a逢깐
                                     「"() "
            Nami唯.rebind( "rmi ://(. ............)/ChatServer ", obj) ;
                                     \\\////
            Systan.out.println( "ChatServer bound in registry");
        } catch (Exceptione) {
            System.out.println( "Helloln耳）l err: " + e) ;

                                               - 160 叫


===== PAGE 164 =====
              e . pr intStackTraceO;
          }
     }
}


II Filename : ChatClient. java
import java.rmi.Renote;
import j ava.rmi .RerioteExcept ion;
public interfaceChatClient extends Remote {
    public void setNextMessage(String message) throws RemoteException;

}


II Filename : RMlChatApplet.java

import java.applet.*;

import java.awt.*;

import Java.io.*

import Java.net.*

import Java.rmi.*

import Java.rmi.reglstry.*

import java.rmi.server.*;

import Java.util.*;

import java.awt.event.*;



public class RMlChatApplet extends Applet implements ChatClient,

                                   ActionListener {
    TextArea text;
    Label label;
    TextField input;
    Thread thread;
    String user;

                                       - 161 -


===== PAGE 165 =====
ChatServer chatServer;



private mllt getRegistryPortO {

     try { return Integer.parselnt(getParameter("port")); }

     catch (NumberFormatException ignored) {

                           return Registry.REGISTRY_PORT; }

}

private String getRegistryNameO {

     String name = getParameter("name");

     return (name == null ? "ChatServer" : name);

}


private ChatServer getChatServerO {

     mlt port = getRegistryPortO;
     String name = getRegistryNameO;

     try {
                                             1
        Object obj = Naming.lookup( "rmi :1/.
        return (ChatServer)obj;

     } catch (java.rmi.UnknownHostException e) {

        System.out.println("Host unknown in un: " + e.getMessageO);

        System.exit(1);
     } catch (NotBoundException e) {

        System. out.println( "Name not bound: " + e.getMessageO);

        System.exit(1);

     } catch (ClassCastException e) {

        System.out.println(name + " was not a ChatServer:" +

                     e.getMessageO) ;
        System.exit( 1);

     } catch (RemoteException e) {


                                  叫 162 -


===== PAGE 166 =====
         System.out.printlnC'Remote exception: " + e.getMessageO) ;

         System.exit(1);

    } catch (Exception e) {

         System.out.println( "General exception: " +

         e.getClassO.getName() + ": " + e.getMessageO);

         System.exit(1);

     }
    return nu比

}

II R入4lCallback 기능을 처리하기 위해 자신을 exportObject 시키고

II addClient() 를 호출하여 등록한다．

private void registerWithChatServer(ChatServer server) {

     try {
         UnicastR帥iote아力ect.export아力ect(thi的；

         server.addCli ent(thi s);

     }
     catch (RemoteException e) {

         System.out.println( "Remote exception: " + e.getMessageO);

         System.exit(1);

     }
     catch (Exception e) {

         System. out.println( "General exception: " +

                  e.getClassO.getName() + ": " + e.getMessageO) ;
         System.exit(1);

     }
}


public void initO {
    URL codebase = getCodeBaseO;


                                     - 163 -


===== PAGE 167 =====
    chatServer = getChatServerO;
    registerWithChatServer(chatServer);
    user = getParameter("user");
    if (user == null) user = "anonymous";
    text = new TextAreaO;
    text.setEditable(false);
    label = new Label("Say something: ");
    input = new TextFi이d（出
    inp ut.setE di table ( true ) ;
    input.addActionListener(this);
    setLayout(new BorderLayoutO);
    Panel panel = new PanelO;
    panel.setLayout(new BorderLayoutO);
    add("Center", text);
    add("SouthTt, panel);
    panel.add("West", label);
    panel.add("Center", input);
}


public void setNextMessage(String message) {
    text.append(message + "Wn");
}

void broadcastMessage(String message) {
    message = user + ": " + message;

    try {
       chatServer.broadcastMessage(message);
    } catch (RemoteException e) {
       System. out.println( "Remote exception: " + e.getMessageO);
    } catch (Exception e) {

                                      叫 164 -


===== PAGE 168 =====
        System. out.println( "General exception: " +

                e.getClassO.getNameO + ": " + e.getMessageO) ;
    }
}


public void actionPerformed(ActionEvent event) {
    if (event.getSource() == input) {

        broadcastMessage(input.getTextO);
        input.setText(") ;




                             - 165 -


===== PAGE 169 =====
       比蜘知 卜艇岱（缸1 4성이   언서 선행듸어昨 할．
0 힐耆


===== PAGE 170 =====
  V장 CORBA에 기초한
    원격 객체 프로그래밍




           학 습 목 표

· CORBA 기술을 이해하게 된다．
·CORBA 기술을 Java로 구현하는 방법을 알게
 된다．
. IDL을 점검한다．




               - 167 -


===== PAGE 172 =====
] 절 CORBA

   이 절에서는 C0RBA 의 개요와 구성 요소들 그리고 C0RBA 어］ 기초한 분
산 객체의 처리 흐름에1 대하여 소개한다．


1.1 CORBA(Common Object Request Broker Architecture) 란?


   ORB（아力ect Request Broker：구현객체）는 C0RBA 객체가 네트웍 상에 어
디에 있든지 상관없이 메서드 호출요청과 그에 대한 결과를 전달하는데 핵심
                                                                       r.hf L
적인 역할을 하는 메시지 버스（bus）이며 , C0RBA는 바로 분산 객체 미들웨어            中Vq＼ 八d小／＼十니小／   \4小노／小니／ 누小니八나八小H八／   ＼八／



인 ORB의 일반적인 아키텍처의 사양을 정의한 것이다. C0RBA는 ORB의 구
卜力尸八1／   卜／   \／小뇨／   1니／   니／   \/\／八／   니／   \／卄／   \




성 요소에대한 인터페이스만 제공할 뿐 그어］ 대한 구현은 ORB를 제작하는 회
사에게 맡긴다. C0RBA의 중요한 관념은 투명성（transparency）을 제공하는데
있다.


   먼저 위치 투명성(location transparency）은 객체가 어디에 있는지 알 필
요없이 C0RBA 객체에 대한 메소드를 호출하고 액세스할 수 있는 능력을 말
한다. 이것은 원거리 컴퓨터에 있는 객쩨의 메소드 호출도 같은 주소 공간에
있는 객체뻬 대한 연산을 호출하는 것과 마찬가지로 쉽게 호출할 수 있다는
것 이 다．


   프로그래밍 언어 투명성（programming language transparency）은 어떤 객
체의 기능을 구현하는데 있어 가장 적절한 언어H프로그래머의 숙련도나 해당
작업에 적합한 언어 등을 사용할 수 있는 자유를 제공한다．


   이러한 자유는 인터페이스와 구현을 분리시킴으로써 가능한데 , 이를 위해

서 CO르旦스늪4현恁륄젤보旦펫앗슷겻읫오언있I皿，(Interface Definition
Language）을 제공한다．


   C0RBA 응용 프로그램 개발자는 IDL을 통해서 새로운 깩체의 인터페이스
                     - 169 -


===== PAGE 173 =====
를 정의해야 한다. IDL 인터페이스는 클라이언트에게 객체가 어떤 모습을 하
고 있는지 알려준다. 즉 객체가 제공하는 연산, 파라미터의 타입 , 그리고 반환
되는 값의 타입에 대해 정의한다. 클라이언트 프로그래머는 원거리에 있는 객
체의 연산을 호출하는 코드를 작성하기 위해 단지 IDL만을 필요로 한다. 클라
이언트는 언어 매핑 (language m키갸)ing）을 통해 IDL 안에 정의된 데이터 타
입들을 사용한다· 이 매핑은 프로그래밍 언어 구조（데이터 타입， 클래스 등）룰
정의하는데 , 이것은 ORB 제작 회사에 의해 제공되는 IDL 컴파일러를 통해서
이루어진다. IDL 컴파일러는 특정 프로그래밍 언어（C, C+ +, Smalitalk, Java
등）로의 바인딩을 지원한다．


  또한 IDL 컴파일러는 클라이언트에 연결되는 스터브 코드를 생성한다. 이
것은 구현 객체로 요청 메시지를 전달하기 위해 , 프로그래밍 언어 데이터 타
입을 표준 포맷으로 변환e마샬링（marshaling）七｝는 스켈레턴이라고 불리는
코드에 연결된다. 이런 방식으로 구현 객체땍 메소드는 호출되고, 같은 방법으
로 결과를 반환할 수 있다


  즉 CORBA 는 이종의 플랫폼과 네트워크 환경에서 응용 프로그램들이 자
유롭게 데이터를 주고 받을 수 있는 분산 시스템의 표준 사양으로서 이종（운
영 체제 , 하드웨어 시스템 ...）의 분산환경에서 여러 종류의 응용 프로그램을 통
합하기 위한 결합 방식이다．


  1991k크 0MG 어］ 의해 오랜 기간에 걸쳐 정의된 표준으로서 분산 객체가
네트워크 상에서 통신을 처리하는 방법에 대해 정의한 개방된 사양으로서
OMA(Object Management Architecture) 의 일부이다．


  CORBA 표준（Object Management Group어］서 정의하는）에 기초한 분산 오브젝
트 인프라는 이종의 엔터프라이즈 환경을 통합하고 차세대 어플리케이션을 위
한 유연한 플랫폼을 제공한다．


                           - 170 -


===== PAGE 174 =====
 RMI 가 순수한 Java 어플리케이션에만 이용할 수 있지만 반면 CORBA 는
언어에 중립적이고 Java 객체를 다른 프로그램으로 쓰여진 객체와 인터페이스
할 수 있도록 한다．


  卜 OMG 란9
  Object 入'langement Group로서 198q년 설립된 Consort沁m이다．
  분산 환경에어 필용한 전반적인 기술들에 대하여 표준안을 만드는
  그룹으로서 전 세계적으로 많은 회사가 참여하고 있다. (MS 사 제외）
  CORBA 는 이들이 제안한 표준 스펙으로서 분산 환경에서 객체간의 통
  신 기능과 이를＋조츠
  http://www.omg.org/ 어］ 자세한 정보를 볼 수 있다．




                      - 171 -


===== PAGE 175 =====
                                                                  口小Ve\'tl 小 '
                                                           tD＼乞



                                 ，」「》  ,   弩*
                                                「 cfl-
                                                   \\
1.2 CORBA에서 제시하는 분산 처리의 흐름


  CORBA 는 Java R入'II 와 매우 유사한 방법으로 스텁과 스켈레턴을 이용한
다. 스텁과 스켈레턴은 ORB 를 통해 접속되는데 , ORB 는 스텁과 스켈레턴으
로부터 메서드 호출을 전송하고 서버 객체로서 동일한 컴퓨터에서 실행되는
객체 어탭터（0너ect Adapter, BASIC Object Adapter）라는 특별한 객체를
이용한다. 객체 어댑터의 역할은 필요시 서버 객체를 활성화 시키고 서버 객
체의 연산을 관리하는데 도움을 준다．



    (
        1 1
                클라O언트



                          \DL」
                                        3i o    /"         1 1\ 구현 객체




   Dynamic                                               Static   Dynamic
                 Client              ORB                 Skel     Skel
   Invocation
                 Stubs             Interface
   Interface                                                       Object Adapter


                          ORB Core(IIOP )



                                                                    OS Kernel
           OS Kernel
                                                                  I/O Subsystem
        I/O Subsystem                Network
                                                                   N/W Adapter
         N/W Adapter




   卜 CORBA 프로젝트에 Java 언어를 활용하는 이점


    -IDL과의 연계성（객체 지원）
    寸 플랫폼 독립성
    -Ap미飢에서 활용함으로서 Obejct Web 이라는 개념 도입



                                     - 172 -


===== PAGE 176 =====
卜 CORBA 를 활용한 클라이언트 객체와 서버 객체의 통신



    11                  r              n




卜 ORB 中 객처］ 요청 중개자


  스텁 , 스켈레턴, 네이밍 서비스, 객체 어댑터등을 함께 유지하는 접착제
역할을 한다. ORB 는 스텁과 통신하고 , 서버 객체를 찾아 내며 , 객체 어
댑터 및 스켈레턴과 통신하는 역할을 한다．


  ORB 는 스텁과 스켈레턴에게 언어에 중립적인 인터페이스를 제공하며，
클라이언트 서버 객체가 서로 다른 컴퓨터에서 서로 다른 언어로 구현된다
는 사실을 스텁과 스켈레턴이 알 필요가 없도록 해준다. 즉 ORB 는 클라
이언트에서    로컬의 것으로 호출하는 것처럼 서버 객체의 메서드를 호출하
도록 한다．


卜 ORB 간의 상호 운용(hOP)


  동일한 네트워크에 서로 다른 회사에서 개발한 ORB 를 사용하여 통신
할 수 있도록 지원될 수 있어야 한다. 하나의 클라이언트가 다수의 객체에
접근하기 위해서 동시에 서로 다른 ORB 를 이용하거나, ORB 어］ 의해 제
                 - 173 -


===== PAGE 177 =====
공되는 하나의 객체어］ 접근하기 위해 다른 ORB 를 이용할 수도 있다. 다
수의 ORB 가 동일한 어플리케이션내에 존재 가능하기 때문에 ORB 는 서
로 통신할 수 있어야 한다．


  GIOP(General Inter-ORB Pr야ocol)은 ORB 사이의 통신을 지원하
기 위해 이용되는 일반적인 인터페이스로서 ORB              간의 통신을 위한 구문
및 메세지 형태를 지정한다. ORB 는 TCP/IP, IPX 또는 SNA 와 같은
다양한 전송 프로토콜을 이용하는 네트워크에서 이용될 수 있으므로 ORB
간의 정보 전송을 위한 규약은 GIOP 어］ 명시되지 않는다．


  IIOP(Internet Inter-ORB Protocol)는 GIOP 를 TCP/IP 프로토콜
어］ 매핑한다．




                ORB                       ORB

            +                                    十
                GI(끄）                     GIOP

                "OP                       "OP

                           TCP/IP




卜 IDL-- 인터페이스 정의 언어


  CORBA 의 중요한 목적중의 하나는 다양한 프로그램 언어로 만들어진
객체가 상호 작용할 수 있으면서도 분산 객체를 지향하는 프레임웍을 제공
하는 것이기 때문에 서로 다른 프로그랙 언어간의 인터페이스 역할이 필요
                 - 174 小


===== PAGE 178 =====
하다．


   IDL 은 Java 언어의 인터페이스와 비슷한 방법으로 인터페이스를 표현
하며 이 인터페이스에서는 원격으로 호출 가능한 메서드에 대한 사양을 지
정한다. 즉, 메서드명 , 리턴값의 유형 , 매개변수등만을 정의한다．


   이러한 사양으로 만들어진 IDL 파일은 IDL 컴파일러에 의해 각각 해당
되는 프로그래밍 언어(Java, C+ +, C등）의 스텁과 스켈레턴 파일이 생성
된다．


  IDL을 Java 로 번역하는 프로그램은 SUN 사이트에서 다운로드받을
수 있다. ( http://www.javasoft.com/products/jdk/idl/ )


                                                                                             小
                                                                 尸 ／=            1
                                                                                 =



                                                         ==1戶J                       = = \
                                                                        Java




                 '=.
                                     C           .   /                         Java
                       '                 1141
                           ===   .




                                                - 175 -


===== PAGE 179 =====
1.3 Java IDL


  CORBA 내에서의 Java 객체 참조는 Java IDL 을 참조한다. Java IDL 은
JDK 1.2 어］ 추가되었다．


  - IDL -> Java
    IDL 의 각 문장들을 Java 언어의 구문에 알맞는 문장들로 매핑한다．


   - idit이ava 컴파일러
    IDL 정의로부터 스텁과 스켈레턴 파일을 제공한다．


   - h1op 를 지원하는 Java ORB
    스텁／스켈레턴간의 통신과 다양한 ORB 사이의 통신을 지원한다．


   e 객쩨1 네임 서버 (tnameserv)
    계층적인 객체 공간으로부터 원격 객체에 대한 참조를 얻을 수 있게 한
    다．
   -API 패키지의 org.omg.CORBA 와 org.omg.CosNaming 패키지
    CORBA 와 Java 객체를 통합하기 위해 필요한 Java API 클래스와 인
    터페이스를 제공한다．




                             - 176 中


===== PAGE 180 =====
1.4 RMI 와 CORBA 의 비교

  다음은 Java 의 RMI 기술과 CORBA 기술에 대한 비교표이다．



             RMI                                      CORBA

 U분산처리 프로그래밍 관련 기술                U분산처리 프로그래밍 관련 기술
 e분산（리모트） 객체 연동 프로그래밍             小분산（리모트） 객체 연동 프로그래밍
 小Java 환경 에서만 활용됨                 e서로 다른 운영 체제 , 서로 다른 언어와
 니ava.rmi 패키지와 Java 언어             의 연동 가능
 나m陀이stry(Naming Server 역할）       - Idi + C, C++, Java ....
                                  m일반적으로 개 발 툴 활용
                                    (vi sibroker, ObjectBroker, Orbix..)




                   Client                          구현객체
                               논리적 호출
                    Stub                           Skeleton
                                                           4
                                                           11
                      411r

               CORBA 런타임                        CORBA 런타임

                    "OP                              "OP
                      1
                      11       CORBA 계층                4
                                                       i
                   TCP/IP                           TCP/IP
                               물리적 호출

                              [ 통신 흐름 ]
                              - 177 小


===== PAGE 181 =====
1.5 IDL (Interface Definition Language)


   구현 언어에 의존적이지 않기 위해 IDL(Interface Definition Language）이
라는 인터페이스 정의 언어를 이용하여 개발한다. IDL 은 어떠한 언어로 개발
된 CORBA 객체든 통일한 방식으로 상호 작용할 수 있도록 지원한다．


   CORBA 프로그래밍의 핵심은 꿎쯔豈걋짚르t亶궐껜브껜竺丑多움
짙브쁘뷴브쁘브븟旦얻役女曳)불괏욘쯔브크낸젖트둘으李든분蚩을
구현하는 것이다．


   이미 설명한바와 같이 실질적인 객체간의 통신은 ORB(O可ect Request
Broker）를 통해서 이루어지며 , ORB 는 CORBA 사양에 포함되는 기능으로서
객체 호출에 대한 request 를 전달받고 처리하는 역할을 수행한다．


   ORB 는 우리가 직접 개발하는 것이 아니며 , 이미 많은 개발업체들로부터
ORB 기능의 제품들이 개발되어 있다. JDK 1.2 에도 포함되어 있으며 상용화
되어 있는 ORB 로는 \Tigibroker, Orbb( 등을 예로 들 수 있다．


  卜 V嘶broker


      V呵broker 는 다이나믹하고 확장성 있는 분산 오브젝트 어플리케이션
   개발을 위한 필수 소프트웨어로서 오늘날의 복잡한 이종의 어플리케이션
   환경이 지니고 있는 많은 어려움들을 해결하는데 필요한 쉬운 사용, 확장
   성 , 유연성을 제공되고 있어 가장 많이 선택되고 있다．


   VisiBroker 3.4 for Java and C+ +


      넷스케이프, 시스코, 오라클, 노벨과 같은 업계 리더들과의 협력관계를
   통하여 비지브로커는 사실상의 CORBA 표준이 되었다. 분산된 오브젝트

                                - 178 -


===== PAGE 182 =====
  들 사이에 산업 표준의 크로스m플랫폼 통신을 하기 위해서 필요한 인프라
  를 제공한다. Internet Inter-ORB Protocol(IIOP）의 지원으로           인터넷，
  인트라넷, 및 웹 기반 컴퓨팅을 위한 산업 표준 프로토콜 기반에서 동작된

  다．
{ IDL 언어 구문 ]


 구현（분산） 객체에 대한 인터페이스만을 정의하는 언어이다. 조건문이나
제어문등은 지원되지 않으며 , 기본형 , 사용자 정의 유형 , 인터페이스 정의，
오퍼에이션（메서드）의 정의등을 지원하는 문법들이 제공된다．


 기존 언어와 비교시에는 C 나 C+ + 와 비슷한 부분이 많이 있다. 일부 브
로커     전문       회사들은 IDL 언어를 알지 않아도 되도록 JAVA 나 C+ +
로 IDL 을 정의할 수 있는 기능들을 제공하고 있기도 하다.                          다음은 IDL
구문에 대한 간단한 설명이다．


 H 주석
        ／半
                  木／,   //


 - Reserved Word(Keyword)
        any             interface      typedef     FALSE      octect
        default         raises         case        object     void
        inout           TRUE           exception   string     context
        out             boolean        module      short      in
        switch          enum           sequence    union     oneway
        attribute long                 unsigned    const     struct
        double          readonly       char        float




                                    - 179 -


===== PAGE 183 =====
                   ．哲必伊M"
m 데이터 유형           'Jd沙 c_
                       'La
                         \ t
      오퍼레이션0제서드）의 반환값, 매캐변수의 유형 결정시 사용．

      기본형（巨츄．
            , short, long, float),
      구조체 유형（struct, union, enumeration),
      템플릿 유형（sequence, array, string), 무형（any)
                                                                             있旨
      문자열형 : string                                                     赴故
                                                                  ,
                                                                  八卜뇨


  7\ array " 길 ' ] " } 고정됨
                                                             '＼
                                                      來巾노
                                                        「"
  /
  5＼
          打pedef유甲
    니sequence : 가면 씔이
                       .   명   “   "    [   크］   "]
           typedef sequence＜유형＞ 명칭；
           typedef sequence＜유형 , 크기＞ 명칭；


H 인터페이스(interface)
      구현 객체가 제공하는 속성과 오퍼레이션을 정의한다．
      오퍼레이션 : 인터페이스 내부에 선언된다. Java 에서는 메서드라
                 고 부른다. 매개변수（전달 방향）, 리턴값, 예외 처리，
                 반환값의 유형，
      매개 변수 전달 방향 : in, out, inout
      예외 처리 : 예외 상황 발생시 클라이언트에 반환하는 구조


               정의 : exception 명칭 {
                           변수 선언．.
                      }
               선언 : 오퍼레이션 헤더의 끝에


m 모듈정의（module)
      인터페이스들을 하나의 페키지로 묶고자 하는 경우




                                       - 180 -


===== PAGE 184 =====
     상속
      단른 인터페이스를 상속받는 샌로是쏘턴－펜인스呈쓰섯활 수 있다．
      interface Newlnter : Superlnter {};


예）                   30硅

                     {
                            ""'”，차卜『
      in erface Test {

               typedef sequence<string> myarr;
               void getName(in string n, out   myarr   ma);
          };
                                               岬外
};
                                小 181 -


===== PAGE 185 =====
1.6 Java 와 IDL 의 구문 비교


  IDL                     JAVA


  module                  package
  interface               interface, helper class, holder class
  constant                public static final
  boolean                 boolean
  char, wchar             char
  octet                   byte
  string, wstring         java. lang.String
  short, unsigned short   short
  long, unsigned long     mnt
  long long,
  unsigned long long      long
  float                   float
  double                  double
  enum, struct, union     class
  sequence, array         array
  exception               class
  readonly attribute      method for accessing value of attrubite
  readwrite attribute     methods for accessing and setting value of
                          attribute
  operation               method




                                - 182 -


===== PAGE 186 =====
2절 CORBA 프로그래밍

 일반적으로 IDL 언어를 활용한다는 것을 제외하면 R八II 프로그래밍과 많이
비슷하다. 다음 순서로 구현한다：


 1. 분산（구현）객체의 사양（메서드, 변수）을 IDL 로 작성한다．
  객체안에 포함되는 메서드와 변수는 IDL 을 통해 하나의 인터페이스로
  만든다.(R入(II에서 리모트 인터페이스와 비슷하다.)


 2. 컴파일을 하여 Java 언어로 구성되는 스텁 그리고 스켈레턴 파일을 생
  성한다. (idit이ava 라는 명령을 활용한다.)


 3. 서버의 스켈레턴 클래스를 상속하여 분산 객체 클래스의 코드를 작성
   한다．


 4. 분산객체를 등록해주고 초기화해주는 역할의 서버 프로그램을 작성한
   다．
 5. 분산객체의 메서드 호출을 요청하는 역할의 클라이언트 프로그램을 작
   성한다．


 [ 테스트 과정 ]


   - Naming Server를 기동시킨다. (tnameserv)
   e 서버 프로그램을 기동시킨다．
   卞 클라이언트 프로그램을 기동시킨다．




                        - 183 -


===== PAGE 187 =====
[ 예제1 2-1 CORBA 프로그래밍 과정을 익히기 위한 테스트 ]

     RMI 프로그래밍에서의 첫번째 예제와 기능은 같다. 클라이언트에서 서버
의 sayHello() 를 호출하는 프로그램을 CORBA 프로그래밍을 통해 구현해 본

다．
     1. 분산 객체의 사양을 제시하는 인터페이스를 IDL 로 작성한다．

                                                                      5心띤，「N납＼.，小"
              // 파일명 : Hello. idi
                                                                       '        （零和            "   '   "   ＼蚊(y.    '




                      module HelloApp {
                                                                                      가'講                       ，
                            interface Hello {                                          '           , , \,d ＼拭』

                                    string sayHelloO;                                 ,r討＼ ',n 니
                                                                                      d斛 놔 \'q1y
                            };
                                                                                      N
                                                                           \\              寸                '




                       };
     2. 컴파일 한다．


         c: Yi> iditojava -fno-cpp Hello. idi



                                      Hello.idl




           HelloStu                                           Hello
                      Hell아扼iper
                                                _HellolmpleBase
                                 Hell아如Ider




                                      - 184 -


===== PAGE 188 =====
    [ idit이ava 에 의해 생성되는 주요 파일 ]

    J (XXStub : 클라이언트측의 스텁 파일 , 마샬링 기능 제공．
    XXXHelper : 클라이언트가 서버의 구현 객체를 참조하도록 하는 메서드
                   제공．
    _XXXImplBase : 서버측의 스켈레턴 파일 , 구현 객체 클래스는 이 클래스
                   상속．
    xxx             : 잊，텃펫으l슷·
    XXXllolder      : 정적 호출시에는 사용되지 않는다. 동적 호출시 활용됨．
                                                    but 이Lt   私心喊 叱77｝두네 棍
                                                         加叱 1＞七F和））늘 乂．

3. 구현 객체（서버）클래스를 작성한다. 스켈레턴 파일인 _Helloln叩iBase
     를 상속하여 구현한다．


II Filename: HelloServant. java

import flelloApp.*;

import org.cing.CosNaming. *;
import org. 刃띵.CosNaming.NamingContextPackage.*;

import org.（乂땅.a垠BA . 水；



class HelloServant extends _HellolmplBase {

    public String sayHello() {
          return TTVnHel lo Wor ldVn" ;

     }
}


4. 3에서 작성한 클래스의 객체를 생성하여 브로커에 등록시키고 관리하는
    서버 프로그램을 작성한다．
                 作咸이
          -ORB 객체匿 생성한다．
          - 뇬전二雨를 ORB 어］ 등록한다．
          - NameSer미ce 라는 이름으로 초기화 되어 있는 NamingServer
                                          - 185 -


===== PAGE 189 =====
          의 객체를 생성한다．
        - NameComponent 객체를 활용하여 분산 객체의 명칭을 설정하
          고 rebind() 메서드를 활용하여 바인딩한다．
        U 대기 상태로 들어 간다．


II Filename : HelloServer. java
// llelloServant 를 객체생성하여 등록하는 기능
// ORB 를 초기화 시키는 기능
import HelloApp.*;
import org.c*眼.CosNaming.*;
import org.ci唱.CosN跏ing.NamingContextPackage.*;
import org.（게띵.cc爪BA . 串；
public class HelloServer {
   public static void rnain(Stri띵 args[ ]) {

        try {
           II ORB 를 생성하고 초기화 시킨다.
           ORB orb = ORB.init(args, null);
           II Hello옰才vant 의 객체를 생성하고 ORB 어］ 등록한다．
           HelloServant helloRef = new HelloServantO;
           orb.connect(helloRet);
            // 리모트에서 이 객체에 접근하고자 할 때 사용될 명칭 지정
                                                                          \4 <\
                                                                                    '1小
                                                                                  rn새
                                                                                          自a
            org.omg.CORBA.Obict objRet =                           生鬼 ' 뇨d化b"
                i4（也iJ\" C化te} 끽체팁                  .              .   r 大；/'
                 " " orb.resOlve_i nitial_reterences(" ameServic; '); 뇨
                                                          十尸   戶




            NamingContext ncRet = NamingContextHe巾er.narrow(objRet);
           II bind the Object Reference in Naming
            NameCc*町批nt nc = new NameCczponent ( "He11o", " ") ;
            NameCc呵nent path[ 1 = {nc};
            匹R餉旦b逈d佃欲h, helloRef);
            II wait for invocations from clients
            java. lang.Object sync = new java. lang.아bjectO;
            synchronized (sync) {
                                     - 186 -


===== PAGE 190 =====
                    sync.wait();      『毛 枉7＼琡 叫"1 寸어' 1 득"\ 티31
                                     벤和
             }
         } catch (Exceptione) {
             Systen.err.print1n( "ERR火: " + e) ;
                 e . printStackTrace(Systen.out);

         }
    }
}


5. 클라이언트 프로그램을 작성한다．



    -ORB 객체를 생성한다．

    - NameService 라는 이름으로 초기화 되어 있는 Nami咽Server 의
        객체를 생성한다．
    中 NameComponent 객체를 활용하여 찾고자 하는 분산 객체의                                  명칭을
        정하고 narrow() 메서드를 활용하여 실제 객체 정보를 얻는다．



I/ Filename: Hellm1ient. java
import llelloApp.*;
import org.（게띵. CosNaming. 牛；
import org.（刃평.a米BA . 水；
public class HelloClient {
    public static void main(Stri띵 args[ ]) {

         try{
                 II 0RB 를 초기화 시킨다．
                 ORB orb = ORB.init(args, null);


             II Na毗Services 어］ 대한 객체를 초기화 시킨다．
                 org.omg.CORBA.Object objRef =
                          orb.resolve_i nitial_references("NameService");

                                          - 187 -


===== PAGE 191 =====
            NamingContext ncRef = NamrngContextHelper.narrow(objRef);
            II resolve the Object Reference in Naming
            NameCanponent nc = new NameC刃刃nent ( "Hello", ") ;
            NameCan跏ent path[ ] = {nc} ;
            Hello helloRef = HelloHelper.narrow(ncRef.resolve(path));
            II   Hello 서버 객체의 sayHel 1d) 를 호출한다．
            String Hello = helloRef.sayHelloO;
            Systdn.out .println(Hello);
        } catch (Exceptione) {
            Systdn.out.println("日W只 : " + e) ;
            e . printStackTrace(Systen.out);
        }
    }
}


6. 서버와 클라이언트 프로그램을 컴파일한다．


7. 다음과 같이 수행시킨다．
                                               p
                                        Qe
        c:> tnameserv        -ORBlnitia지칸）rt 포트번호



        c:> java HelloServer -ORBlnitialPort 포트번호


        c:> java HelloClient -ORBlnitialPort 포트번호




                                      - 188 -


===== PAGE 192 =====
[ 예제 2巴 매개변수 전달하는 메서드 호출 ]

 매개변수를 전달하고 예외 처리가 지정된 구현 객체의 메서드를 호출하는
CORBA 프로그램 예제이다. 앞의 예제를 확장한다．



             II Filename : Hello. idi

             module HelloApp

             {
                  interface Hello

                  {
                       exception cantWriteFi le{ };

                       exception cantReadFi le{ };

                       string sayHello(in string message)


                                ，群智"鼎沁
                       ,,,,,, ,呻，
                                raises (cantReadFile);

                  };
             };
 [ 서버 소스 ]

 II Filename: llelloServant. java

 import HelloApp.*;

 import org.（게띵.CosNaming. 半；

 import org.cxg.CosNaming.NamingContextPackage.*;
 import org.a평.QI'BA.*;

 import java. io.*;

 class flelloServant extends _Hellolr耳）lBase {

   public String sayllello(Stri띵 msg)

            throws HelloApp.HelloPackage.cantWriteFi le     {

         try {

                                      中 189 -


===== PAGE 193 =====
         synchronized(this) {

             File helloFile= new File( "helloStorage.txttt);
             Fi1e뇨tputStream fos = new FileOutputStream(helloFile);
             byte[ 1 buf = new byte[msg. le乷thO];

             msg.getBytes(O, rnsg. lengthO, buf, O) ;
              fos.write(buf);
              fos.closeO;

         }
     } catch(Except ion e) {
         throw new HelloApp.HelloPackage cantWriteFileO;

     }
    return "WnHelloworld ! !Wn";
}


public String lastMessage()
    throws HelloApp.HelloPackage.cantReadFi le {

     try {
         synchronized(this) {
             File helloFile= new File( "helloStorage. txt ");
             FilelnputStream fis = new FilelnputStream(helloFile) ;
             byte[ 1 buf = new byte[1000]
             m1lt n = fis.read(buf);
             String lastmsg = new String(buf);
             fis.closeO;
             return lastmsg;

         }
     } catch(Except ion e) {
             throw new llelloApp.Hell寸ackage.cantReadFileO;
     }
}

                                    - 190 -


===== PAGE 194 =====
}

//Filename: He! loS才ver. java

import Hello加p. 水；
import org.cx唱.CosNaming.*;
import org.a咽.CosNami띵.Nami꿩ContextPackage.*;
import org.c喀.a垠BA . 孝；
public class llelloServer {
    public static void main(Stri追 args[ ]) {
         t ry{

            II ORB 를 초기화 시킨다．
               ORB orb = ORB. init (args, null);
               // 객체를 ORB 어］ 등록한다.
            llelloServant helloRef = new HelloServantO;
            orb. connect (hel loRef) ’,


               // 네이밍 서버 객체를 얻는다．
            org.c坦. a火BA.（力ject objRef =
            orb.resolve_m it i al_referencesC'NameServi ce");
            NamingContext ncRef = NamingContextHel比r .narrow(objRef);


           NameConponent nc = new Name油聊nent ( "Hello", " ') ;
           NameC刃끄onent path[ ] = {nc} ;
           ncRef.rebind(path, hel loRef) ;


            // 클라이언트어］ 의해 호출될때까지 대기한다．
            java. lang.어：)ject sync = new java. lang.아jectO;
           synci寸아lized (sync) {
                 sync.waitO;

           }

                                      小 191 小


===== PAGE 195 =====
         } catch (Exceptione) {

              Systdn.err.println( "ERR只: " + e) ;

              e .printStackTrace(Syst8n.out);

         }
    }
}

[ 클라이언트 소스 ]

II Filename : He11c兀1ient. java

import HelloApp.*;

import org.（게咽. CosN帥ling. 水；

import org.（刃띵．(1只BA . 水；

public class HelloClient {

    public static void main(String args[ ]) {

         try{
              ORB orb = ORB. init (args, null) ;

              org.예띵. XBA.侃ject objRef = orb.resolve_initial_references
                                             ( "Na祀Service");

              NamingContext ncRef = Naming油textllelper.narrow(objRef);

              NameCc叩0nent nc = new NameC皿onent ( "Hello", ") ;

              NameCc呵nent path[ ] = {nc};
               Hello helloRef = HelloHelper.narrow(ncRef.resolve(path));
               // 리모트 메서드 호출



             '丹String hello = helloRef. sayHello(args[OI);
             t System.out .println(hello);

               String oldhello = helloRef. lastMessageO;

               Systdn.out .println(oldhello);

             } catch (Exceptione) {

               System.out.println( "炚R求 : ' + e) ;

                                       - 192 -


===== PAGE 196 =====
            e . printStackTrace(Systdn.out);
        }
    }
}


[ 수행 방법 ]


1. 다음 명령을 수행시켜 작성된 JDL 파일어］ 대한 Java 소스를 만든다．


        iditojava -fno-cpp Hello.idl


2. 서버와 클라이언트 프로그램을 컴파일한다．


        javac * .java HelloApp/*.java


3. 다음과 같이 수행시킨다．


        c:> tnameserv       -ORBlnitialPort 포트번호


        c:> java HelloServer -ORBlnitialPort 포트번호


        c:> java HelloClient "message " -ORBlnitialPort 포트번호




                                   - 193 -


===== PAGE 197 =====
[ 예제 2召 CORBA Callback 프로그래밍 ]

     RMI 프로그래밍에서의 첫번째 예제와 기능은 같다. 클라이언트에서 서버
의 sayHello() 를 호출하는 프로그램을 CORBA 프로그래밍을 통해 구현해 본

다．
                                   ,,.               ,
      伽dii1e HelloApp
     肛：
                     /

          {
                interface llelloCaliback                             .
                              1=          1\   ／끼＼       1/   ／尸H\




               {
                         void callback(in string message) ;

                };
                interface Hello
                                   八／\/
                {
                         string sayflello(in llellcCallback objRef, in string message) ;

                };
          };


          II Filename : HelloServer. java

          import llelloApp.*;

          import org.a唱.CosNaming.*;
          import org.c眼.CosNa川ng.NamingContextPackage.*;

          import org.（刃띵.a果BA. 非；



          class HelloServant extends _HellolmplBase {

               public String sayHello(HellcCallback callobj, String msg) {
                         cal lobj .cal lbackOnsg);

                         return "쀼nHelloworld ! !',Yn";

               }
          }
                                                                         尸 194 -


===== PAGE 198 =====
public class HelloServer {
    public static void main(Stri退 args[ ]) {

        try{
           II ORB 를 초기화 한다．
           ORB orb = ORB.init (args, null) ;


           // ORB 어］ 등록한다．
           HelloS玎vant helloRef = new llelloServantO;
           orb. connect (hel loRef );


           org.ci띵.a火BA.Object objRef =
                     orb.resolve_init ial_references( "NameService");
           NarningContext ncRef = Nami哨加textHelper.narrow(objRef);


           NameCc*riponent nc = new NameCc肛nent ( "Hello", ") ;
           NameC刃巾onent path[ 1 = {nc} ;
           ncRef.rebind(path, hel loRef) ;


           // 클라이언트로 부터의 호출을 대기한다．
           java. lang.아ject sync = new java. lang.어：)jectO;
           synchronized (sync) {
               sync.waitO;
           }
        } catch (Exceptione) {
           Systen.err.println( "ERR求: " + e) ;
           e . printStackTrace(Syst帥.out);


    }
}



                                        - 195 -


===== PAGE 199 =====
II Filename : HelloClient. java

import HelloApp.*;

import org.（게唱.CosNamix退. 水；

import org.（刃띵.a火BA . 半；



class HelloCalibackServant extends _HellcCallbacklmplBase {

    public void callback(Stri띵 notification) {

         Systeiri.out .pr mnt ln(not if i cat ion);

    }
}


public class llelloClient {

    public static void main(Stri追 args[ ]) {

         try {
            ORB orb = ORB. init (args, null);

            org.（刃평.( ORBA.어力ect objRef =

                        orb.resolve_ini t ial_references( "NameService");

            NamingContext ncRef = NamingContextHel祀r.narrow(objRef);



            NameCanponent nc = new NameCa聊nent ("llello", ") ;

            NameCan刃nent path[ } = {nc} ;

            Hello he! loRef = HelloHelper.narrow(ncRef.resolve(path));



            HelloCailbackServant helloCallbackRef = new llelloCalibackServantO;

            orb.connect (he! lcCallbackRef);          , , o미   C뇨今武 "蜘＼ 듬확



            II He 1 loCal lbackServant 의 객체 정보를 전달하면서 sayllel lo() 를 호
             /／출한다．

            String hello = helloRef.sayHello(helloCallbackRef, 'Wntest. . 冊l");

            Systan.out .println(hello);

                                           小 196 -


===== PAGE 200 =====
        } catch (Except ione) {
            Systdn.out.print1n( "以R只 : " + e) ;
            e . pr intStackTrace(System.out);
        }
    )
}


1. HelloC카田ack.idl 을 Java 언어로 컴파일한다．


        iditojava HelloCallBack.idl
                                                叫
2. 생성된 소스들을 컴파일한다．


        javac *.java HelloApp/*.java


3. Name Server 를 기동시킨다．


        tnameserv -ORBlnitialPort 1050&


4. Server 를 기동시킨다．


        java HelloServer -ORBinitialPort 1050


5. Client 를 기동시킨다．


        java HelloClient -ORBinitialPort 1050




                                     - 197 -


===== PAGE 201 =====
3절 IDL 예저1

  1. 다양한 유형 정의



  //Cc町）lexType. idi

  module Co呱lexType

  {
          /／구조체

          struct Point

          {
                 double x;

                 double y;

           };
          /／공용체

          union Dataltem switch(char)

          {
                 case 'c ' : long count;
                 case 'a ' : double amount;

                 default: char initial ;

           };
          // 열 거 형

          enum Grade {A, B, C, D} ;
           // 시 퀀스형

           typedef sequence<long> Scorel;

           typedef sequence< 끄lsigned long, 10> Score2;
           /／문자열형

           typedef string NameL

           typedef str ing<10>Name2;

           typedef wstring Name3;
            typedef wstring<10> Name4;

                                       - 198 -


===== PAGE 202 =====
               /／배열형

               typedef char Coursel[10] ;
               typedef char Course2[10] [10I;

          };

     2 . 메서드 오버로딩은 지원되지 않는다．

     I/ Difference. idi
      interface Difference

      {
               void operO;
               //void oper (long 1) ;!／함수의 다형성이 인정되지 않음
          };

 3 . 상속 지원
     //Inheritance. idl
     interface A
     {
               attribute long 1;
               void oper () ;
     };
     interface B

 {
               I/ attribute long 1; // 이름 충돌 에러 발생
 };
interface C: A,B

{
               I/ attribute long 1; // 재정의 시도 에러발생
               I/ void operO; // 재정의 시도 에러발생
};
                                        - 199 -


===== PAGE 203 =====
4 . 모듈 정의

I/ Mo加le. idi
module A

{
        module B

        {
                 interface C
                 {
                 };
                 typedef sequence<long> Number;
                 typedef str ing<20> Name:
           };
};
module D
{
           interface C

        {
                 void oper (inA: :B: :Carg):
           };
}:
5 . 변수 선언
//Samplel. idl
except ion UsrExcept ion
{};
interface Samplel
{
       //long age; II attribu扼가 빠지면 에러발생
           attribute long age;
           readonly attribute string name;

                                    尸 200 -


===== PAGE 204 =====
              string operl(instring argi, out string arg2, inout string arg3) ;

              oneway void oper2() ;

              void oper3() raises (UsrException) ;

     };

     6 . 다양한 유형 치원

     I/ Sin耳）1eT1思. idi

     interface SimpleType

     {
              /／정수형

              attribute long 1 ;

              attribute long long 11;

              attribute short s;

              attributeunsigned long ul;

              attributeunsigned long long u11 ;
              attribute unsigned short Us;
              // 부동소수점 형

             attribute float f;

             attribute doubled;

             attribute long double 1d;
              /／문자형

             attribute char c;

             attribute wchar we;

             /／부울형

             attributeboolean b;
             /／옥테트형

             attribute octet o;

             I/ any형

             attribute any a;

};
                                         - 201 -


===== PAGE 205 =====
4절 코바／자바어以I의 한글 및 다국어 처리

  IDL 자료형 char, string으로 한글등의 문자를 사용하는 경우 다음과 같은
문제점이 있다. IDL 자료형은 특정 문자 인코딩으로 가정되고 （대개의 경우 8
859-1), 자바 자료형 char, String과 코드 변환된다．


  한글을 포함하는 자바 String이 IDL 자료형으로 변환되거나, 한글을 포함
하는 IDL 자료형으로부터 자바 String으로 변환될 때 , 예외가 발생하거나 잘
못 변환된다．


  다음과 해결책을 선택하여 사용한다．


   ID나료형char       *,:,,,   ,   사용할多

  가장 이상적인 방법이나 기존 IDL 화일을 변경할 수 없거나, 이미 구현된
컴포넌트에는 적용될 수 없다. IDL 자료형 octet, sequence를 사용하고, 전송
할때는 str.getBytes(）를, 읽어들일때는 new String(）을 사용하여 자바 문자와
변환한다．


  IDL 자료형 char, string을 그대로 사용하는 대신 한글을 2번 처리한다．
즉, 전송할때는 new String(s甘.getBytesO, "8859그 " ) 을, 읽어들일때는 new
String(str.getBytes("88 59그 " )）을 사용하여 8859尸1 과 유니코드 사이를 변
환한다．




                                - 202 -


===== PAGE 206 =====
[ 예제 ?4 C0RBA 프로그래밍 과정을 익히기 위한 테스트 ]

     구현 객체의 메서드 호출시 한글을 입출렴하늪쓰쁘 테스트하는 예제 "]
다．
     II Filename: llangul. idl

     interfaceHangul {

               string getStr () ;

               wstring getwstrO;

               typedef sequence<octet> SeqOctet;

               SeqOctet getSeq() ;

               string getStr2() ;                            bil.
                                                                    ite)F.
     };                                                                  6tD   I 1
                                                                               Al       ！『
                                                                                             『／
                                                             。。D         ooe0l      '
                                                          5M小M나'         빅7뇽計지          弩응，
     II Filename : flangulServer. java

     import org.(Jl召. cc只BA. 水；

     import org.（게唱. CosNaming. 水；

     import org.cx唱.CosNami평.Nami坦ContextPackage.*;



     public class lla唯ulServer extends _Hangull旺lBase {

          public String getStr () {
               return " 자바 " ;

          }


          public String getYlstr () {
               return " 자바 " ;

          }


          public byte[ ] getSeq() {
               return " 자바 " .getBytes0;

          }
                                           - 203 -


===== PAGE 207 =====
                                                                                                             n
                                                                                                                 亭

                                                                                            乂甲＼       \10心
                                                                                                             芦
public String getStr2() {

                                                                                      g
                                                                                      才 m
                                                                                        峀
                                                                                                  \
                                                                                                  t
                                                                                        ／
                                                                                                  汾
     try {
                                                                                            人
                                                                                  ／
         (
         l
         M   e
             fL
                  W
                  e
                  n
                  l
                  1
                  r
                  U   tH
                       l
                      QU   1l
                                g
                                n   1
                                        1L1
                                              d
                                              n
                                              1L1
                                                        t
                                                        解  由e
                                                            t  Q
                                                               니
                                                                     1   n
                                                                             8
                                                                             8
                                                                             0U
                                                                             二U
                                                                                                  ／
                                                    1              \J             그
                                                                                            嚼
     } catch( java. io.Unsu耳orte過lcodingException ex ) {

         ex .printStacklrace();

     }
     return null;

}


public static void main(Stri띵[ ] args) {

     try {
         ORB orb = ORB. init (args, null) ;

         HangulServer hangul 1 = new HangulServerO;
         orb. connect (hangul 1);



         // 네임 서비스 객체 얻기

         org.cii唱.（가떠A.（先ject nan祀Service =
         orb.res이ve_initi키_references( "Nan祀Ser미ce");

         NamingContext rootContext

                                    = NamingContextllelper.narrow(nameService);


         // 네임 서비스에 서버 등록

         NameCci叩onent [] ha雎u1lNai肥
                         = { new NanieC刃耳）onent ( "hangull", fl fl ) };

         try {
             rootContext .rebind(hangullName, hangull) ;
         } catch( NotFound ex ) {

             rootContext.bind(hangullName, hangull) ;

         }


                                                        - 204 小


===== PAGE 208 =====
              // 무한 루프

              java. lang.아bject sync = new java. la召.0bjectO;

             synchronized (sync) {

                 sync.waitO;

             }
         } catch (Except ionex) {

             ex .printStackTraceO;

         }
    }
}


II Filename: HangulClient. java

import org.（刃평．CosNaming. 水；

import org.（刃땅．a派BA．水；



public class lla曜uiClient {

    public static void main(Stri띵[ ] args) {

         try {
             ORB orb = ORB. init (args, null);

             org.이坦. a火BA.Object objRef

                       = orb.resolve_initial_references( "NameService");
             NamingContext ncRef = NamingContextHelper .narrow(objRef) ;

             Na叱Cc*uponent ndl = new NameCci旺onent ( "hangull", ") ;

             NameCc*聊nent[ ] pathi = {ncl} ;

             Hangul hangull = lla昭ulllelper.narrow(ncRef.resolve(pathl));



             II 1. 예외 발생

             try {
                 Syst8n.out .println(hangull.getStrO);
             } catch (Except ionex) {


                                      - 205 -


===== PAGE 209 =====
        Systan.out .pr mnt ln(ex);

    }


    II 2 . 유니코드 wstring 사용（Java IDL에서는 wstr ing<기 지원되지
    // 않는다 . )

    try {
        Systdn.out .println(hangull.getWstrO);
    } catch (Except ionex) {
        Systdn.out .println(ex);
    }

    /7 3 . 바이트 배열 사용
    System.out.println(new String(hangull.getSeqO) );
    II 4 . 기존 IDL의 String 자료형을 그대로 이용하는 방법

    try {

    ,Sys "뺘"Ut.可'ntln(newStr"咽（h쁘11.getStr2(）丑"‘由‘""("8859_i”꿋）"
    J catch(java. io.UnsupporteclEncodingException ex) i
                                                           I／文上1'이1
        ex .printStackTraceO;
    }
} catch (Except ionex) {
    ex .printStackTraceO;

}




                                     - 206 -


===== PAGE 210 =====
-IDL 컴파일 :

     idltojava- fno-cppHangul. idi


- Java 소스 컴파일 :

     javac Hangul* .java lla璡ulPackage/*.java



- tnameserv 를 수행시킨다．

     tnameserv -ORBinitialPort 1050



m 구현 객체（서버）를 수행시킨다．

     java HangulServer -ORBinitialPort 1050


小 클라이언트 프로그램을 수행시킨다．

     java HanguiClient -ORBinitialPort 1050




                               - 207 -


===== PAGE 212 =====
VI장 JavaBeans 프로그래밍




           학 습 목 표

· JavaBeans의 용도와 활용 방법을 알게 된다．
· JavaBeans를 구현하는 방법을 익히게 퇸다．
·EJB의 기능을 점검해 본다．


===== PAGE 214 =====
］절 JavaBeans 의 개요

  이 절에서는 Java에서 Component Base Programming 을 지원하는 기술
인 JavaBeans 의 개발 방법과 활용 방법을 소개한다．

                  r-vi9陟（ Q싸아eCt 品V做.k 4- 여？p, 4c c,咬年어 屹伊
1.1 Bean$ 란 ?                           ' t聽딕는 Bec " S·
                  L 可卵 ．丁'""＼『뗀S· ：丁'P""너
              r 6하卜'免 品Voietm3 . JC니‘以卜쩍 日伉叩f 't     v
                                                    【kc,< 아e )
                  '                앉게 社料 een’니g . c9如小q 이뇹. + P卜人 ()
     r 비주얼 툴에서 시각적으로 다룰 수 있는 재사용 가능한 소立트웨어 "
     컴포넌트 J


  복잡한 프로그램을 개발하는데 있어서 이미 제작된 Java 소프트웨어 컴포
넌트를 사용함으로써 프로그래밍의 능률을 향상시킬 수 있다. 재사용의 극대
화를 목표로 하고 있으며 , 어떠한 기능이든 Beans 로 구현하는 것이 가능하
나 일반적으로 GUI 컴포넌트의 형태를 갖추고 있다．


  소스 수정（추가 컴파일）없이 재사용 가능하고 다른 프로그램안에 쉽게 속
성을 변경하여 임베드（embed）할 수 있는 소프트웨어 컴포넌트（독립 프로그
램）로서 이식성이 강하고 플랫폼과 독립적으로 실행된다．




       뉴스모음 프로그램                      A 회사의 그룹웨어 프로그램


                                          브라우저 기
                                          눙의 bean
                브라우저 기
                능의 bean




                            - 211 -


===== PAGE 215 =====
1.2 Java Beans 의 기1빨 목적


  O／떤 플랫폼에서토 수莎될 -7느 았는 재사용 가능한 소프트哥어 컴포난트를
만드는 것아다．


  어떤 플랫폼에서도 수행된다. ->
        Java 언어의 주요 특징


  재사용 가능하다. ->
        우리가 개발하는 Beans 의 기능은 매우 다양하다. 간단한 GUI컴포
       넌트 기능의 Beans 부터 서블릿과 I긴咀서버기능의 Beans, 그리고
        스프레드쉬트나 편집기와 같이 하나의 독립된 어플리케이션의 기능
       을 지원하는 Beans 까지 매우 다양하다. 이미 개발된 Beans 를 활
        용할때, 자손 클래스를 생성하거나, 소스 수정등에 의한 추가 컴파
        일 없이 통작방식（Event), 출력형태（Property）등을 얼마든지 일관
        적인 방법으로 수정할 수 있다．


  JavaBeans를 활용하여 구현하고자 하는 프로그램의 기능에 알맞게 수정
하여 원하는 어플리케이션을 좀더 쉽고 빠르게 개발할 수 있다．




                                        원하는 기능의 프로
                                        그램에 적용




                                        원하는 기능의 프로
                                        그램에 적용




                               원하는 기능의 프로
                               그램에 적용
                          l
                          n
                          n
                           乙
                           乙


===== PAGE 216 =====
1.3 JavaBeans 가 지원해야 하는 기능


  JavaBeans 도 하나의 클래스이다. 그러나 일반적인 클래스들과는 다르게
다음과 같은 기능을 지원하고 있어야 한다．

       나叫나！수吐"이느
    . “．
  - in[rospecuonG八／uswmization

                       7P攪 ）姓升 b fC'fl叫 『3旨·
                                  ,    .


  - Persistency
                        介
  小 Event Handling




 卜Introspection&Customization


    피sual Tool 이 Beans어］ 대한 정보를 점검할 수 있도록 하는 기능으로
  서 소스를 보지 않고도 이 클래스에 어떠한 멤버들이 존재하는지를 알 수
  있는 기능을 Introspection 이라고 한다. JavaBeans 는 Introspect沁n 기
  능을 지원하여 좀더 효율적으로 새로운 속성을 설정（Customization）할 수
  있어야 한다．




                                           속성（property)
                                           메서 드（method)
                                           이 벤트（event)




                             - 213 -


===== PAGE 217 =====
卜 Persistency
                硝b      ·




   개발하고자 하는 프로그램의 기능에 알맞게 수정된 Beans 는 객체 직
렬화라는 기능을 통해 현재의 설정 상태를 지속적으로 유지시킬 수 있어
야 한다． 객체 직렬화라는 기능은 RMI 에서도－소개하였듯이 메모리상에
전장되어 있는 Java 객체의 상태를 유지할 수 있도록 스트림에 출력하고
읽을 수 있는 기능을 의미 한다．



                                                       실행 가능한 Java코드

                             직렬화된 Bean
                     속성 변경                             실행 가능한 Java코드




                                                       실행 가능한 Java코드




‘「' ""' """"""" U교 叩“砒 b幽""'"뱐 「'忖")
   Visual Component 기능의 Beans 인 경우에는 Beans 자체가 이벤트
  리스너가 되거나, Beans어］서 발생되는 이벤트에 대한 리스너（Listener)
  를 등록 또는 해제하는 기능이 가능해야 한다．
                  ）陌나怜＼ 얍" "卜 苞
     米져羚 帥，耐 畏計는

                                      Event Listener




                                - 214 -


===== PAGE 218 =====
1.4 Beans 의 활용



  이미 개발되어 있는 Beans 를 활용하는 방법은 소스 레벨에서 직접 Bean

관련 메서드를 사용하여 활용할 수도 있으나 일반적으로 Beans 를 가지고 개

발이 가능하게 하는 피sual Tool 을 활용한다．



  이러한 툴들은 Beans 어］ 대한 속성 설정이나 이벤트 리스너 등록등을 툴

을 활용해 쉽게 접근할 수 있도록 제공하며 실제 일련의 마우스작업과 키보드

작업을 통해 Beans 를 활용한 Java 클래스 소스를 생성할 수도 있다．



  다음은 Beans 를 활용할 수 있는 \uisual Tool 리스트이다．



   助rland's JBui lderTM
   BulletPro寸 Corporation's JDesiguerPro 2.1
   Imperial Sof tware Technology 's VisajTM
   Inforrnix 'sData Director for Java
   IBM's Visual Age R for Java programing language
   JRad Technologies ' j .rad
   KonaSoft 'sKonaSoft Packajar 1.1
   Lotus Develoi肥nt 's BeanMachineTht (formerly AppletAuthor)
   Object앉are 's Parts f어；. Java 2.0 technology
   ObjectSoft 's BrewMaster sl.10
   0MNIS 鈿ftwar可5아씨IS Studio v . 1. 0
   0racle 's JDeveloper Suite
                                          \




   SFS Software 's Iavadraw
   Silicon Graphics ' Cosmo Code
   Softera ' s Soft坂）deler/Business
   Sybase 's PowerJ Enterprise2.1
   Symantec 'sVisual Cafe
   Tek-Tools ' Kawa
                                      中 215 -


===== PAGE 219 =====
  대부분의 툴들이 상용화 되어 있는 관계로 이 교육에서는 BDK 의 사용
방법을 간단하게 제시한다. BDK는 Beans Develo미nent Kit 의 약자로 Sun
에서 제시하는 개발된 Beans 의 테스트 툴이다. 간단하게 Applet 의 소스롤
생성하는 기능과 속성과 이벤트리스너등이 설정된 Beans 를 직렬화하여 저장
하고 읽어들이는 기능도 지원된다．.


  다음은 BDK 의 수행 화면이다．


  [BDK 초기 화면 ]


    川 口
           n니口
                                                                                  目回口

                          C小이삐 圄 劃面 쇠
                               小                            小

          자동

   C：甘Pro9rar Files邯띠Ki .I甘beanbox> if           " " == " 卄indow5_卜IT" setlocal

   C:甘Progrdm Fi1es樹BDK1. l甘beanbox> set CIASSPATHzclasses; . 璋libnethodtracer. jdr; ..
   ··infobus. jar

   C:甘Progrars Files DtJK1. 1卄beanbox> jaua sun- beanbox.Bean8oxFrarne




   [ 등록되어 있는 Beans 를 메모리상에 로딩하는 과정 ]


          日已a ri Box                       目回口

                 Loading and analyzing jars...



                                                 - 216 -


===== PAGE 220 =====
[BeanBox ]

    日   ri円                                                       S.
    餠弱 晦；五크치                                         1，加毋汨d蔑小簽＝ ，匕，1                                                目 i     X       i營꾜拓吊餌布：熙i聰m四＝伯I치
                 Smn1ye11n
                                                   ' F陀 Edit 너C놔 Services              Help

                 8山！BLd노n
                                                                                                                                         backdround

                 口1ng.8Utfon
                                                                                                                                          foreQroufld -
                 C山eU卄0n


                                                                                                                                                nam寸' nellJ
    回EXPhq伽so.
                 EY1ntM0nd0r
            OA.Io9. .n                                                                                                                               化nit abxd.

. 딴Jo5小1r
                  TrdTo出

                 V叭1r

                  C harrg. S . p.9. r
                                                                                                                                                                                          目回口
                  S이t因1t
                                                                                                                                        8 0. 打a디ng ser\nce started
                  Ooot5S口nn1r

                  JDBC SELECT

                  SDd.r9.1n

                  B山.801t5n 020

                  0mn91BUd0n (2>

                  0o,9o1如n020


    뮤' xxii的油" 020，尸
                              m
                           Ftp딪J부｝로       j   '"




                              哨
                              0네ook
                              Express     e
                                                                                                                              I


    m 目 區
김점현감．U disk山（l}3t.                                 3叫dk, ja,




-          ..-_ i       - 1    뇨＼ d1 nr            11    - -A 口口 .1 _.A .' . A m띠 /   C) 4 n   I -叫 .j- ,-,A n가 4 rm J 小   A - -i   小   A. '따 A ..    A ....A U1 1 口1Jr＝尸   亡r J   dr J
                   1 ＄三J 끽 戶 p. " ．썬1뽀 旦-J！트J브J모I-i쁘：j旦J깊Jj!J크J크-3틔1긷3- J- J트J！
                                                                              터旦JI 哲1 르3-竺1                                                                                               叭1rytot耳 Ix:力




[ BeanBox 의 File 메뉴 ]
圈B日日nBox                                                                                                                                    目回口
    File                   Edit         View                   Services               Help
                 Say包 . .
                 Sen帥zeC（그mponent...
                 MakeApplet...
                 Load...
                 LoadJar...
                 Print
                 （긔ear
                 Exit




                                                                                                          - 217 卞


===== PAGE 221 =====
[ BeanBox 의 Edit 메뉴 ]


 圈日ea ri E小（                                                                       目回口
           =
           L1 J           陀 n         Eu it     \／沌빠   Services   He巾

                                                                                                                          /寸/
                                          Cut

                                          Co pv
                                                                                   / / / // d d / / ／伊 / / / / r/ / / 中 / / 戶/ y



                                                                                                                               y
                                          Report...

                                          Events         卜                                                                     夕



                                                                                                                               7
                                          日m d 하마）e啣

                                                                                                                               J



                                                                                                                               r




               7                                                               !                                               J




[ BeanBox 의 Ser＼八ces 메뉴 ]


 圈EleanBox                                                                         目回口
           File                       Ed住
                                      r
                                                \／伯叫   Seniices   He巾


 1
                                      1                                                                                                                                             !




                                                                                                                           / / / / / 尹/ / / / / / / / r / / / / / / 尹 / / / / / /
                                                        Info日us Suppo比
                                                        Show Method Trau:inq


 i




 r/ / / / / / / / / / / / / / / 少 /




  // /J +尹 少 / / 寸/




                                                                        - 21


===== PAGE 222 =====
                               1m：回由鈿七M斗 ,
1.5 일반 클래스와 晦ns 의 차이점 \-               ＠帖机c't 즈夕)-I'口 ,．十
                                             '   ..v. D巴-l   'Ib 뇨 >1/ Y

                                             욕측              ，『 녕比
  Java Beans 는 비주얼 툴（BDK 또는 IDE）을 이용하여 수행 결과를 점검하
면서 비주얼하게 또는 소스 레벨에서 다룰 수 있지만 클래스는 소스레벨에서
만 다룰 수 있다는 것이다．


                Java Beans              일반 API 의 클래스


  작성 언어         Java 언어로 작성             Java 언어로 작성
  구현 기능         모든 기능                   모든 기능
  멤버들           규격에 알맞는 멤버              적용되는 규칙이 없음
                규칙 정용
  Property 변경   비주얼하게                   소스 레벨에서 직접 메서드를
                （또는 소스레벨）               호출하여
  Event 처리      비주얼하게                   소스 레벨에서 직접 메서드를
                （또는 소스레벨）              호출하여


  Beans 는 결국 맞춤 클래스라고 할 수 있다.             클래스의 메서드명을 아무
명칭이나 쓸 수 없으며 , 기능（설정 , 추출, 이벤트 처리）에 따라 그 명칭을 이
미 제시되고 있는 명명 규칙으로 결정하여야 한다. 그리고 Beans 가 미sual
컴포넌트인 경우 외부로부터 이벤트 리스너를 등록할 수 있는 메서드가 정의
되어 있어야 한다．


  그래야만 Beans 를 사용하여 활용할 수 있는 툴에서 시각적으로 쉽거］ 색
이나, 출력 내용, 크기 등을 수정할 수 있으며 , 이벤트 발생시의 이벤트 처리
루틴을 설정할 수도 있는 것이다．


 이미 개발된 Beans 를 가지고 개발할 수 있는 툴들로는 JBuilder, Power
J 등이 있으며 Trial 버젼에는 Beans 를 활용하는 기능이 빠져 있으므로 정품

                             - 219 -


===== PAGE 223 =====
을 사용해야 한다. 아쉬운대로 SUN에서 제공되는 BDK(Beans Development
Kit) 를 사용하여 간단하게 Beans 를 활용하는 Applet 을 캐발할 수 있다．
하지만 상용화되어 있는 툴과는 차이가 있다．


  SUN에서 제공되는 BDK 툴을 설치하면 그 안에 Beans 의 데모 파일들도
있으므로 이 소스들을 점검하1 볼 수 있다. 일반적으로 Button 클래스는 우리
가 소스 레벨에서 크기나 라벨명 그리고 색등을 원하는 것으로 설정하기위해
메서드 호출을 직접 코딩하여야 하나 demo 디렉토리의 OurBtt아i Beans 는
BDK에서 제공되는 BeanBox 라는 프로그램에서 마우스 클릭 기능으로 비주
얼하게 색 , 크기 , 라벨등을 수정할 수 있다. 바로 이 것이 Beans 이다．


[OurButt이i Class 의 멤버들 ]


  BDK 를 설치하면 생성되는 데모디렉토리에 존재하는 OurButton 이라는
Bean 클래스의 멤버들의 사양을 점검하1 본다．


  public class OurButton extends Canvas implements Serializable,
                                 MouseListener, MouseMot ionListener {
     OurButton() {}
     public OurButton(Stri띵 label) {}
     public synchronized void paint (Graphics g) {}
     public void mouseClicked(MouseEvent evt) {}
     public void mousePressed(MouseEvent evt) {}
     public void mouseReleased(旅useEvent evt) {}
     public void mouseEntered(放兀seEvent evt) {}
     public void mouseExited(MouseEvent evt) {}
      public void mouseDragged(MouseEvent evt) {}
      public void mouseMoved(MouseEvent evt) {}
      public synchronized void addActionListener (ActionListener 1) {}
      public synchronized void removeActi址istener (ActionListener 1) {}

                                     - 220 -


===== PAGE 224 =====
public void adclPro思rtyChangeListener(PropertyChangeListener 1) {}

pub! ic void removePropertyChangeListener(PropertyChangeListener 1) {}

pub! ic void fireAction() {}

public void setDebug(bo月ean x) {}

public boolean getDebug() {}

public void setLargeFont (bo月ean b) { }

public boo! ean isLargeFont () {}

pub! ic void setFontSize(int x) {}

pub! ic mlt getFontSize() {}

pub! i c void se tFont (Font f) { }

public void setLabe!(Stri召 newLabe! ) {}

public String getLabel () {}

public DimensiongetPreferredSize() {}

public DimensionpreferredSize() {}

pub! ic DimensiongetMinimumSize() {}
public DimensionminimumSize() {}

private void sizeloFit () {}
public void setForeground(Color c) {}

public void setBackground(Color c) {}

private boo!ean debug;

private PropertyChangeSupport changes = new PropertyChangeSupport (this);

private Vector pushListeners = new Vector () ;

private String labe! ;

private boo!ean down;
private boo!ean sized;
static final m1lt TEXT_XPAD= 12;

static final m1lt TEXT_YPAD = 8;




                                      - 221 -


===== PAGE 225 =====
1.6 Beans API


  다음은 JDK 1.2에서 지원되는 API 리스트이다. 일반적으로 생성되어 있는
Beans 을 활용하는 프로그램에서 사용되며 2 개의 패키지로 구성되어 있다．


    java.beans
    java.beans.beancontext


  java.beans


         Interfaces
                 Appletlnitializer
                 Beanli寸O
                 Customizer
                 Des由n卜加de
                 PropertyChangeLi stener
                 PropertyEditor
                 VetoableChangeListener
                 Visit川ity


        （깃asses
                 BeanDescriptor
                 Beans
                 EventSetDescriptor
                 FeatureDescriptor
                 IndexedPropertyDescriptor
                 Introspector
                 MethodDescriptor
                 Param eterDescr巾tor

                                      中 222 -


===== PAGE 226 =====
    PropertyChangeEvent
    F가opertyChangeSu口口ort
    Pro口ertyDescri口tor
    PropertyEditorManager
    Pro口ertyE미torSu야兀 rt
    SimpleBeaninfo
    VetoableChangeSupport


Exce口tions
    Intros口ect向nException
     Pr야）ertyV아旺xcept




                         - 223 -


===== PAGE 227 =====
java.beans.beancontext


      Interfaces
           BeanContext
           BeanContextChild
           BeanContextChildCom ponentProxy
           BeanContextContainerProxy
           BeanContextMem bershipListener
           BeanContextProxy
           BeanContextServiceProvider
           Be an C ontextSe r八cePro미derBeanin化
           BeanContextServiceRevokedListener
           BeanContextServices
           BeanContextServicesListener


      （긔asses
           BeanContextChildSupport
           BeanContextEvent
           BeanContext卜가em bershi口Event
           BeanContextServiceAvailableEvent
           Be an C ontextS e rv Ic e RevokedEve nt
           BeanContextServicesSu pp o it
           BeanContextServicesSuppo rt.BCSSServiceProvider
            BeanContextSupport
            BeanContextSupport.




                                - 224 -


===== PAGE 228 =====
1.7 구현 방법


     1.3 절에서는 Beans 가 지원해야 하는 기능들을 소개하였다. Beans 는 일
반 클래스들과는 달리 Introspection忍Customization, Persistency 등의 기능
들을 지원하여야 한다. 쉽게 말하면 맞춤 클래스라고 할 수 있다. 이 절에서
는 Beans 를 구현하는 방법에 대하여 단계별로 설명한다．




1.7.1 최소 기능의 Bean


     Beans 가 지원하여야 하는 최소한의 기능들을 지원하는 클래스를 개발하
기 위해서는 다음과 같은 기능을 구현하여야 한다．


     1. 디폴트 생성자 메서드를 반드 ] 장의하고 있어야 한다．


            Beans 클래스를 인스턴스화시킬때 호출되는 메서드가 Beans 클래스의
            디폴트 생성자 메서드를 호출하기 때문이다．
                                                                 났% "   ci小乞   지셉

                 茉月엿프.1延螂브娘) >，小『 "「
                                   「

      2. 직렬화가 가능하도롬 奴va.io.Ser怡lizab蛇 을 상속하여야 한다．


     다음은 최소 기능만을 지원하는 Beans 예제이다．

 1
     h人7
           ． 謙之     =   "伐   i
                                     趣 哺눋
                                      '
                                              '"   t


             《
             『      '   띠        "        "   3t   "




                                                       - 225 -


===== PAGE 229 =====
 [ 예제 1-1 ]

                                                    , ,   q公         ．



II Filename : SimpleBean. java                    下b "         k仄寸
                                              (y               \U\


 import java.awt.*;
 import java. io.Serializable;
 public class SimpleBeanextends           implements Serializable {
      public SimpleBeanO{
          setSize(印,40);
          setBackground(Color . red);

      }
 }


 [ 테스트 방법 ]


 1. 컴파일한다．


     javac SimpleBean.java


 2. 다음과 같은 내용으로 manifest.tmp 파일을 생성한다．

                     V
     Manifest-Version: 1.0
     卜始me:   SimpleB明毗坮弱
                           \//
     Java-Bean: True


 3. jar 파일로 묶는다．



口匣iSimpleBean.jar manifest.tmp SimpIeBean.c1aSy

                                        - 226 -


===== PAGE 230 =====
참고로 Button.jar 의 Meta-INF/Menifest.mf 파일의 내용은 다음과 같다：


     Manifest-Version: 1.0
     Name: sunw/demo/buttons/OurButton.class
     Java-Bean: True
     Created-By: 1.2.2 (Sun Microsystens Inc. )


     Name: sunw/denolbut tons/OrangeBut ton. ser
     Java-Bean: True


     Name: sunw/deno/but tons/BlueBut ton. ser
     Java-Bean: True


     Name: sunw/deno/buttons/Expl icitButton. class
     Java-Bean: True




                                 - 227 -


===== PAGE 231 =====
1.7.2 Beans 의 속성（Property) 조정（Customi기ng)


  속성 조정이 가능한 Beans 를 개발하는 방법중의 하나는 간단하게 필요한
속성을 설정하는 기능의 메서드, setXXX() 와 속성값을 추출하는 기능의 메
서드, getXXX() 를 구현하여야 한다. 즉, Beans 의 명명 규칙을 적용한다．
이 메서드들은 Beans 개발 툴들에 의해 자동적으로 인식된다．


  1. 속성값을 저장할 변수를 선언한다．
    private Color color = Color.green;


  2. 다음과 같이 추출 메서드를 정의한다．
    public C아or getC아orO{
        return color;
    }

  3. 다음과 같이 설정 메서드를 정의한다．
    public void setColor(Color newColor){
         color = newColor;
         repaintO;
    }

  4. paint() 메서드를 다음과 같이 수정한다．
    public void paint(Graphics g) {
         g.setC아or (c이or);
         g.fillRect(20, 5, 20, 30);
    }




                                  - 228 -


===== PAGE 232 =====
[ 예제 1-2 ]


II Filename : SimpleBean. java
import j ava.awt . *;
import java. io.Serializable;
public class SimpleBeanextends Canvas implementsSerializable{


    private Color color = Color.green;


    pub加 C이or getC이orO{
         return color;

    }


    public v이d setC이or(C이or newC이or) {
         color = newColor;
         repaint () ;
    }


    public void paint (Graphics g) {
         g. setColor (color);
         g. fillRect (20, 5, 20, 30) ;
    }


    public Si 旺leBeanO{
         setSize(印,40);
         setBackground(Color .red);
    }
}




                                         - 229 卜


===== PAGE 233 =====
[ Naming Conventi이1 : 명명 규칙 ]


        속성을 설정하는 기능, 현재의 속성값을 추출하는 기능，
        속성상태를 점검하는 기능


        public 什operty乃'pe get尸比pertyNai끄e()
        public void set尸h갸ertyName（尸m7e忖y乃tpe a)
        public boolean isPropertyName()
        public void setPropertyName(boolean b)
        public void addEventNameListener( EventNameListener 1)
        public void removeEven끄ameListener( EventNameListener 1)




[ 예제 1召 ]


II Filename : Arrow. java
import java. io.Serializable;
import java.awt.*;
public class Arrow extends Canvas implements Serializable {
  private String dir;
  public Arrow() {
        superO;
        setDirection( "North");
        setBackground(Color. 1 i帥tGray);
        setSize(20, 20) ;

   }
   public String getDirection0 {
        return d卄 ;

   }
   public void setDirection(String newDir) {
                                     - 230 中


===== PAGE 234 =====
     dir = newDir;
     repaint ();

}
public synchronized void paint (Graphics g) (
     mllt width = getSizeO.width;
     mllt height = getSizeO.hei帥t;
     Point tail = new Point () ,
            head = new Point () ,
            legi = new Point () ,
            1eg2 = new Point () ;


     tail. setLocation(width - 1, height I 2) ;
     head.setLocation(O, height / 2) ;
     legl.setLocation(width / 2, 0) ;
     1eg2. setLocation(width / 2, height - 1) ;
     if (getDirectionO.startsWith( "N")) {
         tail. setLocation(width I 2, height - 1) ;
         head.setLocation(width I 2, 0) ;
         Ieg1.setLocation(O, height / 2) ;
         1eg2.setLocation(width - 1, height I 2) ;
     } else if (getDirectionO.startsWith( "S")) {
         tail. setLocation(width I 2, 0) ;
         head.setLocation(width / 2, height - 1) ;
         legl.setLocation(O, height I 2) ;
         1eg2.setLocation(width - 1, height I 2) ;
     } else if (getDirectionO.startsVith( "E")) {
         tail. set[.ocation(0, height / 2) ;
         head.setLocation(width - 1, height I 2) ;

     }
     g. setC月or(getBackground());

                                     - 231 -


===== PAGE 235 =====
           g. fillRect (O, 0, width - 1, height - 1) ;
           g. setColor(Color .black);
           g. drawLine(tail.x, tail. y, head.x, head.y);
           g. drawLine(head.x, head.y, legl.x, legl.y) ;
           g. drawLine(head.x, head.y, leg2.x, 1eg2.y);

      }
  }



1.7.3 조정 가능한 속성 제시


  앞 절에서는 setXXX() 메서드 명칭을 사용하··                              1 乙하게 조정이 가능한
속성을 제시하는 방법을 점검하였다. 이 절에서는 1eanlnf今 를 활용하여 속성
들의 종류를 제시하는 방법을 점검해 본다．


  [ 예제 1짜 ]


 II Filename: Arrow뇨anlnfo. java
  import java.beans.*;


  pub! ic class Arrow允anlnfo extends SimpleBeaninto {
      public Property侁scriptor[ ] getPro光rtyDescriptors() {

           try {
              PropertyDescriptor pd = new PropertyDescriptor("direction",
                                                           Arrow.class);
              pd.setPropertyEditorClass(DirectionEditor.class);
              PropertyDescriptor resultE] = { pd };
              return result;
           } catch (Except ionex) {
              System.err.print!n( "ArrowBeanlnfo: unexpected exept ion: " + ex) ;
                                        - 232 卞


===== PAGE 236 =====
             return null;
         }
    }
}


II Filenaiie : DirectionEditor. java
public class Direct ionEditor extends java.beans.PropertyEditorSupport {
    public String[ ] getTags() {
         string result[ ] = { "North", "South ' , "East ", "West " };
         return result;
    }
}



        " n占g;Y
                 듬吐 ' 尉消·
         回 寸， 8比




                                     - 233 -


===== PAGE 237 =====
1.7.4 속성 조정과 관련된 리스너 지정



 이 절에서는 단순히 속성을 조정하는 것뿐 아니라 특정 속성이 조정될 때

미리 등록되어 있는 리스너를 호출하는 기능올 점검해 본다. 등록 가능한 리
스너의 종류는 다음과 같다 :



   PropertyChanageListener

   VetoableChangeListener


  71-. PropertyChanageListener

   Beans 의 속성이 수정될 때마다 수행되는 리스너를 등록하는 기능




   private PropertyChangeSupport changes =
                                     new PropertyChangeSupport(this);


   public void setDirection(Stri召 newDir) {
         String oldDir = dir;
         dir = newDir;
         repaint 0;
         changes.firePropertyChange("direction", oldDir, newDir);
    }
   II property change listener methods
    public void addPropertyChangeListener(PropertyChangeListener I) {
         changes.addPropertyChangeListener(l);
    }
    public void removePropertyChangeListener(PropertyChangeListener I) {
         changes.removePropertyChangeListener(l);
    :i

                                    - 234 尸


===== PAGE 238 =====
나. Ve加a벼eChanageListener

 Beans 의 속성 수정이 불가능할때 호출되는 리스너를 등록하는 기능




 private VetoableChangeSupport vetos =

                                 new VetoableChangeSupport(this);


 public void setDirection(String newDir) {

       try {
           String oldDir = dir;
           vetos.fireVetoableChange("direction", oldDir, newDir);
           dir = newDir;
           repaint 0;
       } catch (Except ione) {
           Systen.out.println( "Change vetoed! ") ;
       }



 II vetoable property listener methods
 public void addVetoableChangeListener(VetoableChangeListener I) {
       vetos.addVetoableChangeListener(l);
 }
 public void removeVetoableChangeL治tener(VetoableChangeListener I) {
      vetos.removeVetoableChangeListener(I);
 }




                                     - 235 -


===== PAGE 239 =====
1.7.5 Event Handling 지정


  Beans 가 \uisual Component 인 경우에 한해 Beans 에서 발생되는 이벤
트에 대하여 처리 루틴 즉, 리스너를 Beans 의 외부에서 정의하여 등록할 수
있도록 하려면 필요한 이벤트를 등록하는 기능의 메서드를 내장하고 있어야
한다．


  그리고 Beans 가 다른 Beans 의 리스너로서 사용될 수 있도록 하려면 해
당 인터페이스를 상속하여야 하며 각 메서드들을 적절하게 정의하고 있어야
한다．


  가. 다른 Beans 의 리스너로 사용 가능한 Beans


    Arrow Beans 를 다른 Beans어］서 ActionListener 로 등록할 수 있게
  하려면 다음과 같이 정의한다．


      import java. io.Serializable;
      import java.awt. *;
      import java.awt.event.*;
    public class Arrow extends Canvas implementsSerializable, ActionListener {


              II called by event source
          public void actionPerformed(ActionEvent e) {


          }
      }




                                          - 236 -


===== PAGE 240 =====
나. Beans 어］ 리스너 등록


 Beans 어］ 구현된 ActionListener 를 정의하려면 다음 메서드들을 추가

하여 구현한다．


 public synchronized void addActionListener(ActionListener I) {
      pus址i steners . add引帥ent ( 1);
 }
 public synchronized void removeActionListener(ActionL治tener I) {
      pus祉isteners.raiioveElaiient (1);
 }
 public void fireAction() {
      Vector targets;
      synchronized (this) {
          targets = (Vector) pushListeners.cloneO;
      }
      ActionEvent actionEvt= new ActionEvent (this, 0, null) ;
      for (mnt i = 0; i < targets.size0; i++) {
          ActionListener target = (ActionListener)targets.elementAt (i);
          target . act ionPerfor叱d(act ionEvt);
      }
 }




                                       小 237 -


===== PAGE 241 =====
1.7.6 직렬화 가능한 Bean 의 활용

  이미 설명한 바와 같이 Beans 는 직렬화가 가능하여야 한다. 직렬화가 가
능한 Beans 를 캐발하는 방법은 간단하게 java.io.Serializable 을 상속하는
것 이 다．


  이 절에서는 이렇게 구현된 Beans 를 직렬화시켜 저장하는 예제를 점검해
본다．


  [ 예제 1巧 ]


  II Filename : ArrowSerialize. java

  import java. io.*;

  import java.beans.*;
  class ArrowSerialize {

      public static void main(Stri坦 args[1) {

           try {
               File뇨tputStream fos = new FileOutputStream( "arrow.ser ");

               Object(itputStream oos = new ObjectOutputStream(fos);
               Arrow arrow = (Arrow)Beans. instantiate(null, "Arrow") ;

               arrow.setDirect ion( "East ");

               oos.write力ject (arrow);
           } catch(Exception ex) {

               System.out.println( "Couldn't open 'test ' for writi평.");

           }
      }
  }


  Name: arrow. ser

  Java-Bean: True

                                          - 238 中


===== PAGE 242 =====
1.8 JavaBeans 예저1


  이 절에서는 두 개의 JavaBeans 예제를 점검하여 JavaBeans 의 구현 방법
을 복습하고 BDK 의 BeanBox어］서 구현된 기능을 테스트해 본다．


  [ 예제 1田 ]


  이미치 버튼 기능의 Bean 이다．


  II Filename : ImageButton. java
  import j ava.awt . *;

  import j ava.awt .event . 水;

  import java.awt. image.*

  import j ava.beans. 串;

  import java. io.Serializab1e;
  import java.net.URL; ;



  public class ImageButton extends Canvas implements Serializable,

                                                            ImageObserver {
    Dr ivate static final m1lt          SPACING= 5;
    Dr ivate transient Image            image;
    Drivate transient Act ionListener   actionListener = null;
    Dr ivate transient m1lt             imgWidth, imgHeight ;
    private boo lean                    hasFocus;
    private String                      label;
    Dr ivate String                     i inageName;
    Dr ivate boo lean                   sticky;
    Dr ivate bo아ean                     autoSize;
    Dr ivate boo lean                   down;



                                    - 239 -


===== PAGE 243 =====
II Constructors
public ImageButton() {
     this( "OK", "OK.gif ", true, false, false) ;

}


public ImageButton(String 1, String in, booleanas, booleans, booleand) {
     II Allow the superclass constructor to do its thing
     superO;


     II Set properties
     label = 1;
     autoSize= as;
     sticky = 5;
     down = d;
     setFont (new Font ( "Dialog", Font.PLAIN, 12) );
     setBackground(Color. 1 i帥tGray);
     set ImageName( in);


     II Enable event processing
     enableEvents(A卄1'Event .FIUJSJ?N聊F-
                                      i价얹（I AWlEvent . 砥刃SEE＼目nJ4A없
                                                                  （1
     AWlEvent . 豚列SEJEYFI吐V짜if-
                            i价盟 I AWThvent.KEYJV剛1J价얹0;

}

II Accessor methods
public String getLabel() {
     return label;

}


public void setLabel(Stri띵 I) {
     label = 1;

                                    - 240 -


===== PAGE 244 =====
     if (autoSize)

        si zeToFitO ;

}


public String getlmageNa朧() {

     return imageName;

}


public void setlmageNa毗(String in) {
     imageName = in;



     II Load the image

     image = loadlmage(imageName);
     if (autoSize)

        si zeT寸it ( ) ;

}


public boolean isStickyO{
     return sticky;

}

public void setSticky(boolean s) {

     sticky= s;

}

public boolean isAutoSize() {

     return autoSize;

}


public void setAutoSize(b刈ean as) {


                                 - 241 -


===== PAGE 245 =====
     autoSize = as;

     if (autoSize)

          sizeToFitO;

}


public boolean isDown() {

     return down;




public void se tFont (Font 1) {

     super.setFont(f);
     if (autoSize)

          sizeToFitO;

}

II Other public methods

public synchronized void paint (Graphics g) {
     Dimensiond = getSizeO;

     II Calculate the width & height of the image

     if (image != null) {

          iniglleight = image.getHei합t (this);

          imgVidth = image.getWidth(this);

      }

     II Calculate the vertical spacing around image and foregroundtext

     g. setFont (getFont ());
     FontMetrics fm = g. getFontMetricsO;

      m1lt vSpacing= Math.max(SPACI熙；, (d.height- imgHeight-

                                fm.getMaxAscent () - fm.getMaxDescentO) / 3) ;



                                      - 242 中


===== PAGE 246 =====
II Paint the backgroundwith 3D effects
g. setColor (get Background());
g. fillRect (1, 1, d.width- 2, d.height- 2) ;
g.clraw3DRect (O, 0, d.width- 1, d.height- 1, !down) ;
g. setColor (Color .darkGray);
if (down) {
    g.drawLine(1, d.height - 3, 1, 1) ;
    g.士awLine(1, 1, d.width- 3, 1) ;
)
이se {
    g. drawLine(2, d.height - 2, d.width 小 2, d.height - 2) ;
    g. drawLine(d.width- 2, d.height- 2, d.width- 2, 1);
}

II Paint the image
if (image != null) {
    if (down)
       g. drawlmage(image, ( (d.width- imgWidth) / 2) + 2, vSpacing+ 1,
              this);
    이 se

       g. drawlmage(image, (d.width- imgWidth) / 2, vSpacing, this) ;
}


II Paint the foreground text
g. setC月or(getForegroundO);
if (down)
    g.drawString(label, ( (d.width- fm.stringYiidth(label)) I 2) + 2,
                   d.height - vSpacing- fm.getMaxDescent () + 1) ;
else
    g. drawStri띵(label, ( (d.width- fm.stri찡川dth(label)) I 2) ,

                                  - 243 -


===== PAGE 247 =====
                          d.height - vSpacing- fm.getMaxDescentO);
     II Paint the focus rect
      if (hasFocus) {

          g. setColor (Color.gray);
          g.士awRect (SPACING- 1, SPACING- i, d.width- (2 * (SPACING- 1) ),

                         d.height- (2 * (SPACING- 1) ));
      }
}


public DimensiongetPreferredSize() {
     II Calculate the preferred size based on label text and image sizes
     FontMetrics fm = getFontMetrics(getFontO) ;
     m1lt height = 2 * SPACING,
     width = 0;
     if (image != null)
          height += SPACING+ fm.getMaxAscent() +fm.getMaxDescentO+ imgHeight;
     이 se

          height += fm.getMaxAscent() + fm.getMaxDescentO;
     width = Math.max(fm.stri띵Yidth(label) + 2* SPACING, (height * 3) I 2) ;


     return new Dimension(width, height) ;
}

II Event processingmethods
public synchronized void addActionListener (ActionListener 1) {
     actionListener = AWThvent枾lticaster.add(actionListener, l) ;
}


public synchronized void removeActionListener(ActionListener 1) {
     actioriListener = AWIEventMulticaster.r톄ove(actionListener, 1) ;


                                      - 244 -


===== PAGE 248 =====
}


protected void processAct ionEvent (Act ionEvent e) {
      II Deliver the event to all registeredact ion event listeners
      if (actionListener != null)
          act ionListener . act ionPerfor毗d(e);

}


protected void processFocusEvent (FocusEvent e) {
      II Get the new focus state and repaint
      switch(e.getlD0) {
      case FocusEvent .FOCUS_GAINED:
                                       hasFocus = true;
                                        repaintO;
                                        brei水；


      case FocusEvent .RX1JSJ刃g1T:
                                        hasFoctis = false;
                                        repaint ();
                                        break;
      }


      II Let the superclasscontinuedelivery
      super .processFocusEvent (e);
 }


protected void processMouseEvent (MouseEvent e) {
      II Track mouse presses/releases
      switch(e.getID0) {
      case MouseEvent .昧光明j垠眺SED:

                                      - 245 -


===== PAGE 249 =====
                                    down = !down;

                                    repaint () ;

                                    break;



     case MouseEvent .昧刃親j之區l:A얹m:
                                    if (down 砥 ! st icky) {

                                           fireActionEvent0;

                                          down = false;

                                          repaintO;

                                    }
                                    break;
     }
}
protected void process腑useMot ionEvent (伽seEvent e) {
     II Track mouse drags
     if (e . getlD() == MouseEvent . 旅x廠江垠AG(；可） 忍展 !sticky) {

         Point pt = e. getPoint0;

             if ( (pt.x < 0) i i (pt.x > getSize0.width) I I

                    (pt.y< 0) I I (pt.y> getSize0.hei합lt)) {
             if (down) {

                 down = false;

                 repaint ();

             }
         }
         else if (!down) {

             down = true;

             repaint () ;




                                     - 246 -


===== PAGE 250 =====
protected void processKeyEvent (KeyEvent e) {
     II Simulate a mouse click for certain keys
     if (e .getKeyCode() == KeyEvent .VK丑TIF之 I I
                             e.getKeyChar() == KeyEvent.VI죄A肋 {
          if (sticky) {

              down = !down;
              repaint () ;

          }
          이se {
              down = true;
              repaint ();
              fireActionEventO;
              down = false;
              repaint ();

          }
     }
}
II Private support methods
private void sizeToFit () {
     II Resize to the preferred size
     Dimensiond = getPreferredSizeO;
     setSize(d.width, d.height) ;
     Component p = getParentO;
     if (p != null) {
          p. invalidateO;
          p . d丸ayout 0;
      }
}
private void fireActionEvent () {
     processActionEvent (new Act ionEvent (this, Act ionEvent.ACI'I!'1JERF札但）,


                                       - 247 -


===== PAGE 251 =====
                             null) );

     }
     private Image load岫ge(Stri召 name) {

             try {
                     URL url = getClassO.getResource(na肥);

                     return createlmage((ImageProducer)url.getContentO);

             }
             catch (Exceptione) {

                     Systdn.err.println( "Couldn't load the image " + name + ". ") ;

                     return null;

             }
     }



II Filename : ImageB此tonBeanInfo. java

import java.beans.*;

public class ImageB此tonBeanInfo extends Si町leBeanlnfo {

     II Get the appropriate icon
     public java.awt.Image getlcon(int iconKind) {
             if (iconKind== BeanInfo.IW'_010Rj6x16) {

                      java.awt. Image img = loadlmage( "Image跏ttonIcon16.gif ");

                     return 1mg;

              }
             if (iconKind== Beanlnfo.IW1_aL不L32x32) {

                      java.awt.Image img = loadlmageC'ImageButtonIcon32.gif ");

                      return img;

                 }
                 return null;

         }
 }

                                               - 248 -


===== PAGE 252 =====
[ 예제 1-7 ]


시계 기능의 Bean 이다．



II Filename : Clock. java
import java.awt.*;
import java.awt.event.*;
import java.beans.*;
import java. io.Serializable;
import java.util.Calendar;


public class Clock extends Canvas implementsSerializable, Runnable{
  private static final m1lt     SPACING= 4;
  private transient DimensionoffSize;
  private transient Image       offlmage;
  private transient Graphics offGrfx;
  private transient Thread      c1ockThread;
  private boolean               raised;
  privateboolean                digital;


 II Constructors
 public Clock() {
       this(false, false) ;
  }


 public Clock(boolean r, boolean d) {
       II Allow the superclass constructor to do its thing
       super () ;


       II Set properties

                                          - 249 -


===== PAGE 253 =====
     raised = r;
     digital = d;
     setBackground(Color. 1 i帥tGray);


     II Set a default size
     setSize(100, 100) ;


     II Create the clock thread
     cl어：kmread = new Thread(this, "Clock") ;
     이ock끄iread.st art ();

}

II Accessor methods
public boolean isRaised() {
     return raised;

}

public void setRaised(boolean r) {
     raised= r;
     repaint () ;
}

public boolean isDigitalO {
     return digital;
}

public void setDigital (bo月ean d) {
     digital = d;
     repaint () ;
}

                                  小 250 -


===== PAGE 254 =====
II Other public methods
public void run() {
      while (clock뇨ead != null) {

          repaint ();

          try {
              II Sleep for a second
              c lockThread. sleep(1000) ;
          } catch (InterruptedExcept ion e) {

              Systdn.out .println(e) ;
          }
      }
)

public void update(Graphics g) {

     paint (g) ;
}

public synchronized void paint (Graphics g) {
     Dimensiond = getSize() ;


     II Create the offscreengraphics context
     if (offGrfx == null H (offSize.width != d.width) I I

                                         (offSize.hei帥t != d.height) ){
          offSize= d;
          of flmage = createlmage(d.width, d.height) ;
          offGrfx = of flmage. getGraphicsO;

     }


     II Paint the backgroundwith 3D effects
     of fGrfx.setColor (getBackgroundO);

                                      - 251 -


===== PAGE 255 =====
     offGrfx. fillRect (1, 1, d.width- 2, d.hei합1t- 2) ;
     offGrfx.draw3DRect (O, 0, d.width- 1, d.height- 1, raised) ;
     of fGr fx. setCoI or (getForeground());


     II Paint the clock
     if (digital)
         drawDigitalC!ock(offGrfx) ;
     이 se

         drawPnalogClock(offGrfx);


     II Paint the image onto the screen
     g. drawlmage(offlmage, 0, 0, null) ;
}


II Private support methods
private void drawAnalogClock(Graphics g) {
      mllt   radius = (Math.min(getSizeO.hei帥t, getSizeO.width) 小
                                (SPACING* 2) ) I 2;
     Point center = new Point (getSizeO.width I 2, getSizeO.hei합lt I 2) ;


     II Draw the clock shape
     g. setColor (Color.black);
     g. drawOval(center.x-radius, center.y- radius, radius * 2, radius * 2) ;
     g. setColor (Color.毗ite);
      g. fill0val(center.x - radius + 1, center.y- radius + 1, (radius * 2)
                         小 2, (radius 半 2) - 2) ;
     II Draw the hour marks and numbers
      g. setFont (getFontO);
     FontMetrics fm = g. getFontMetricsO;
      for (mnt h = 1; h < 13; h++) {

                                         - 252 -


===== PAGE 256 =====
    II Draw an hour mark
    double hourAngle= h * Math.PI / 6.0;
    g. setColor(Color .black);
    g. drawLine(center.x + (int)(Math.round(O.9 * radius *
    Math.sin(hourAngle))), center.y- (int)(Math.round(0.9 * radius *
    Math.cos(hourAngle))), center. x + (int)(Math.round(radius *
    Math.sin(hourAngle))), center.y- (int)(Math.round(radius *
    Math. cos(hourAngle))));
    II Draw an hour number, as long as it will fit
    if (fm.getAscent() 小 fm.get碗scent() < (radius! 4) ) {
        String nurn = String.value兀(h);
        g. setColor(getForegroundO);
        g. drawString(num, center. x+ (int)(Math.round(0.7 * radius 非
        Math.sin(hourAngle))) - (frn.stringSVidth(num) / 2) , center.y-
        (int)(Math.round(0.7 * radius * Math.cos(hourAngle))) +
        ( (fm.getAscent() - fm.getDescentO) / 2) );
    }
}
/! Draw the hour hand
Calendar now = Calendar.getlnstanceO;
g. setColor (Color .black);
g. drawLine(center.x, center.y, center. x + (int)(Math.round(radius *
        0.4 * Math.sin((now.get (Calendar.IX11R) % 12) * Math.PI / 6.0 +
        (Math.PI * now.get (Calendar.MINIJI'E) / 360.0) ))), center .y-
        (int)(Math.round(radius * 0.4 * Math.cos( (n川.get (Calendar.IIXJR) %
        12) * Math.PI / 6.0 + (Math.PI * now.get (Calendar.MINIJIE) /
        360.0)))));
!! Draw the minute hand
g. clrawLine(center.x, center.y, center. x + (int)(Math.round(0.8 *
        radius * Math.sin(n州.get (Calendar.MINIJTE) * Math.PI / 30.0) )),

                                 - 253 -


===== PAGE 257 =====
               center.y- (int)(Math.round(0.8 * radius *
               Math.cos(now.get (Calendar.MINI.JIE) * Math.PI I 30.0) )));
     II Draw the second hand and center
     g. setColor (Color.red);
     g.drawLine(center.x, center.y, center. x+ (int)(Math.round(O.6 *
               radius * Math.sin(now.get (Ca1endar.SEcD力 * Math.PI I 30.0) )),
                center.y- (int)(Math.round(0.6 * radius *
               Math.cos(now.get (Calendar.SEW'I力 * Math.PI / 30.0) )));
     g. setColor (Color .black);
     g. fillOval(center.x 中 2, center.y- 2, 4, 4) ;
}


private void drawDigitalClock(Graphics g) {
     Dimensiond = getSizeO;


     II Get the time as a string
     Calendar            now = Calendar.getlnstance0;
      mllt               h = now.get (Calendar.FI小) % 12;
     StringBuffer        time = new StringBufferC") ;
      if (h == 0)
             tin祀.append( "12: ");
     else
             t ime.append(String.valueOf (h) + ". ") ;
     String s = String.valueOf (now.get (Calendar.MINU'l'E));
      if (s. length() < 2)
             ti毗.append( "0" + s + ": ");
      else
             time.append(s + ": ");
      s = Stri띵.va1u的f (now.get (Ca1endar.SE 恥D));
      if (s.length() < 2)


                                          - 254 -


===== PAGE 258 =====
                      time.appendC'O" + s);
                   else
                      t ime.append(s);
                  II Draw the time
                  g. setColor (getForegroundO) ;
                  g. setFont (getFontO) ;
                  FontMetrics fm = g. getFontMetricsO;
                  g.士awStri坦(time.toStringO, (d.width- (SPACING* 2) -
                   fm.stringVidth(time. toStringO) ) I 2, (d.height- (SPACING* 2) +
                   fm.getAscentO - fm.getDescentO) I 2) ;
        }
}


II Filename : ClockBeanlnfo. java
import java.beans.*;
public class ClockBeanlnfo extends Si旺）leBeanlnfo {
    II Get the appropriate icon
    public java.awt. Image getlcon(int iconKind) {
            if (iconKind== Beanlnfo.K赴QIL足l6x16) {
                j ava.awt . Image img = loadlmageC'Clocklconl6.gi f ");
                return img;
            }
            if (iconKind== Beanlnfo.K沁a1J足32x32) {

                java.awt. Image img = loadlmage( "ClockIcon32.gif ");
                return img;

            }
        return null;

    }
}


                                                 - 255 -


===== PAGE 259 =====
2 절 Enterprise JavaBeans(EJB）에 대한 소개

  앞절에서는 Java Beans 어］ 대하여 공부하였다 이 절에서는 미들웨어 개발
프레임웍이라고 할 수 있는 Enterprise JavaBean 이 무엇인지 점검해 본다．


2.1 Enterprise JavaBeans 란?


  Enterprise JavaBeans(EJB) 규격은 멀티티어（MultiTier) 분산 객체 구조
에 기반한 Java 어플리케이션의 개발과 배포를 위한 컴포넌트 모델을 정의한
다. EJB 컴포넌트 모델은 엔터프라이즈의 미들티어에 상주하는 재사용 가능한
어플리케이션 컴포넌트（Enterprise JavaBeans）를 지원하는 환경을 제공한다．
즉, JavaBeans 컴포넌트 모델을 서버 기반의 컴포넌트로 확장시킨다．


  컴포넌트들은 Enterprise JavaBeans와 함께 컨테이너에서 실행이 되며 , 그
컨테이너는 쓰레딩 , 트랜잭션, 상태 관리 , 자원 공유와 같은 시스템 수준의 복
잡한 일을 처리하는 실질적인 컴포넌트 실행 시스템이다．


  Sun MicroSystems의 JavaSoft 어］ 의해서 개발된 Enterprise JavaBeans
스펙은 플랫폼 톡립적인 멀티티어 분산 객체 어플리케이션의 개발, 배포 및
관리를 단순화시키는 어플리케이션 프로그래밍 인터페이스（API)를 지원한다．


  보안, 다중 트랜잭션과 같은 복잡한 구현 부분은 컨테이너가 담당하므로，
단지 무슨 기능을 처리하는 미들웨어 서버인가에 따라 엔터프라이즈 지향의
속성들을 상속（EJBObject）하여 즉, EJB API 를 활용하여 간단하게 구현할 수
있다．


  그런데 EJB는 단지 하나의 모델로서 , 중요한 구현 결정들은 EJB 솔루션을
제공（컨테이너）하는 벤더들에게 좌우된다. EJB 솔루션은 다음과 같은 기능을
지원하여야 한다．

                              - 256 中


===== PAGE 260 =====
        산업 표준 프로토콜의 사용
        친숙한 IDE들과의 통합
        분산 환경에서의 트랜잭션 지원
        다양한 클라이언트로부터의 연결 가능
        보안, 결함 허용 능력 , 확장성 제공


 많은 업체들이 위의 기능을 지원하는 Application Server 제품들을 내놓고
있다．


2.2 현재의 상황


 분산 객체 컴퓨팅이 정착을 함에 따라, 정보기술(IT）에는 새로운 기술들이
제시되고 있다. CORBA와 같은 분산 객체 아키텍처는 이종의 플랫폼들을 위
한 어플리케이션을 신속하게 개발하여 이종의 데이터 소스들을 결합할 수 있
게 한다．


 어플리케이션을 컴포넌트로 분할하고 비즈니스 로직을 미들티어 서버로 이
동시켜서 미들티어 객체의 로직들을 재사용하는 것은 전체적 어플리케이션 7귀
발 시간을 확실히 줄여준다. 그러나, 멀티티어 어플리케이션의 코딩이 복잡해
서 규격화된 시스템 수준의 프로그래밍을 할 수 있는 엔지니어가 필요하므로
미들티어 서버로 변환하는 기업들은 상대적으로 별로 없다．


 하지만 웹 기반 컴퓨팅의 놀랄만한 성장은 IT가 멀티티어 접근방법을 사용
하도록 이끌었다. 웹 기반의 비즈니스 어플리케이션은 브라우저 기반의 클라
이언트를 지원할 수 있도록 씬中클라이언트 구조를 필요로 한다. 이런 클라이
언트들은 인트라넷 기반의 자원들과 서로 연동을 해야 하지만 종종 애플릿을
다운로드 받기 어려운 시스템 자원들이 있다．




                        - 257 -


===== PAGE 261 =====
 클라이언트의 부담을 덜어주기 위해서 이종의 플랫폼을 연결하고 레거시
시스템을 통합하는 이식성 있는 서버측 솔루션을 구축하고자 한다. 즉, Java
와 CORBA가 주류를 이루게 됨에 따라, 자사의 테크놀러지를 그런 솔루션에
결합되기를 원한다．


 가중되고 있는 이러한 요구사항틀을 처리하기 위해서 표준 Java와 CORBA
테크놀러지에 기반한 " 한번의 개발로 어디서나 실행할 수 있는" ,o\ 哈R 깨발
모델을 필요로 하게 된다. 보다 많은 개발자들이 트랜잭션이나 보안 같은 복
잡한 일을 하지 않고도 정교한 분산 어플리케이션을 구축할 수 있도록 멀티티
어 어플리케이션의 개발, 배포 및 관리를 단순화시키는 솔루션이 필요하게 되
는 것이다．




                     - 258 -


===== PAGE 262 =====
2.3 Enterprise JavaBeans릍 사용해야 하는 이유


  비록 Java 가 분산 어플리케이션 개발에 있어 중요한 이점을 제공하지만，
멀티티어 분산 어플리케이션이 요구하는 시스템 수준의 복잡함을 명확하게 처
리해 주지는 못한다. Java 가 미들티어 서버로 이동함에 따라, 개발자들은 트
랜잭션, 보안, 분산과 같은 복잡한 업무를 처리할 수 있는 Java 로 확장하여
비즈니스 로직의 작성에 초점을 둘 수 있기를 원한다．


  EJB 규격은 Java를 사용하여 중요한 임무를 수행하는 플랫폼 독립적인 서
버측 어플리케이션을 구축할 수 있는 JavaBeans 컴포넌트 모델을 확장시키는
API이다. 서버 측면의 어플리케이션은 미들티어 서버에 위치하면서 비즈니스
프로세스를 반영하는 재사용이 가능한 블록 소프트웨어（EJB）로 구축이 된다．


  트랜잭션, 분산, 보안과 같은 인프라스트럭처 문제로부터 어플리케이션 의
미론을 완화시켜서 EJB는 어플리케이션 개발을 단순화시키고, 개발자들이 근
원적인 인프라스트럭처에 대해서는 걱정할 필요 없이 비즈니스상 중요하고도
복잡한 분산 어플리케이션을 개발할 수 있게 한다．


  EJB는 Java 언어를 기반으로 개발이 되므로, 어플리케이션 배포에 있어서
" 한번의 개발로 어디서든 실행 " 을 한다. 컴포넌트들이 어떤 플랫폼에서나 실행
이 될 뿐만 아니라, 어느 벤더의 EJB 컨테이너（컴포넌트 실행 시스템） 상에도
완전하게 이식할 수 있다．


  EJB는 또한 쉬운 프로그래밍과 언어로서의 Java의 이식성 때문에 어플리
케이션 개발이 간단하다. 그리고 멀티티어 분산 오브젝트 어플리케이션을 지
원하기 위해써 개발된 컴포넌트 모델로 프로그래밍과 미들티어 서버 객체들의
배포를 쉽게 해준다．




                         小 259 -


===== PAGE 263 =====
2.4 EJB 의 구현


  앞에서 언급한바와 같이 EJB 는 서버의 미들티어 서버를 개발하는데 있어
서의 내부적인 복잡한 처리 절차에 대하여는 생략하고 비지니스 로직 부분에
대하여만 구현하게 하여 분산 처리 프로그램을 더욱 용이하게 개발하도록 하
는 기술이다．




                              EJB Cot卄小ner


                               EJB Server


                     Server                  DB
                                                  .1
   EJB Component
       EJB Container상어］서 수행되는 전형적인 JavaBean 으로서 , 클라
       이언트에 대한 서비스를 담당한다. 즉, Bessiness Logic을 구현하
       는 부분이다．


   EJB Container
       EJB Server상에서 수행되며 자원 관리 , 유지 , 보안, 트랜잭션 관
       리등의 역할을 수행한다. EJB Component가 요구하는 모든작업을
       처리한다. 하나의 EJB Container 안에 여러개의 EJB Component
       가 존재하게 된다．




                         - 260 -


===== PAGE 264 =====
1DB 연동 과정에 기존의 연결 방법과 EJB 를 활용한 방법 비교 ]


小 Socket, R入41, CORBA 등을 활용한 기존의 연결 방법


                    결과
              +1
                                                   DB
               1H




 Client                      Server
              SQL Query 문




-EJB 를 활용한 연결


Client                      EBJ Server

                               EBJ Container

                                               /
   EBJ                          EBJ             Client
   Object                       Instance
                                 ＋卜
                                               \         \   /
                                               Persistance




EJB는 다음과 같은 두 캐의 전형적인 구현 방법이 지원된다：


세션 빈즈（Session Beans) :
서버상에서 실행이 되는 일부 비즈니스 로직을 처리하는 기능의 영속성이
없는 객체


엔티티 빈즈（Ent仕y Beans) :
영속성 있는 스토리지（예를 들어 데이터베이스에 있는）에 저장된 엔티티나
기존 엔터프라이즈 어플리케이션에 의해서 구현이 되는 엔티티들의 객체를
의미하는 영속적인 객체
                             - 261 -


===== PAGE 265 =====
 Session Beans                                 Entity Beans


 Fields contain conversaton state.             Represents data in a database.
 Handles databaseaccess for client.            Shares access for multipleusers.
 Life of client is life of Bean.                Persists as long as data in database.
 Can be transaction aware.                     Transactional.
 Does not survive server crashes.              Survives server crashes.



 만일 멀티티어 어플리케이션이 이런 두 캐의 디자인 범주에 있을 수 있다
면 , 프로그래머들은 비즈니스 로직을 작성하는데 중점을 둘 수 있으며 EJB 컴
포넌트 실행 시스템이 복잡한 운영 문제들을 처리할 수 있다．




                                                                        >
                                                               \



                                1 Entity
                                 Home                Entity
                                                     Bean
                                  Entity                           )ataBase
                                  Remote

            寸＋
                                                                   Container
  Browser
                 Servlet
                                 Session
                                 Home

                                 Session
                                         !\\         Session
                                                     Bean                               /
                                 Remote

                            \                                  I




                                     EJB Server

                           Entity Bean 과 Session Bean




                                           - 262 -


===== PAGE 266 =====
2.5 EJB 구현을 위한 요구사항


 EJB 스펙을 지원하는 EJB 서버를 필요로 한다. 각 벤더에 따라 수행시키
는 과정이 다소 다르기는 하지만 기본적으로 EJB 스펙을 만족하고 있으며 다
음과 같은 기능들을 지원한다．


  m 엔터프라이즈에 연결할 수 있는 산업 표준 프로토콜의 지원
  e 주요 통합개발환경(IDE）들과의 통합으로 개발자들이 EJB와 중요한 환
   경에 포인트- o壬클릭만으로 접속
 1 분산 환경의 트랜잭션 지원
  e 엔터프라이즈 데이터에 표준 기반의 접속
  U 다양한 클라이언트로부터 연결 가능
   (HTML 기반의 클라이언트와 Java Applet 기반의 클라이언트 포함）
  m 엔터프라이즈 데이터에 알맞은 보안 제공
  小 EJB 어플리케이션의 높은 가용성




                      - 263 -


===== PAGE 267 =====
[SUN 의 Java EJB 발표 자료 ]


  Sun Microsystems는 Entity Beans어］ 대한 지원과 애플리케이션 서버의
확장성을 돕는 기능이 포함된 EJB(Enterprise JavaBeans) 1.1 API 스팩을 발
표하였다．


  Moscone이라는 코드명을 가지고 있는 이 최신 Java 스팩은 분산 애플리
케이션의 조립과 전개를 향상시키고 분산 애플리케이션의 서버를 교차하는 이
식성을 단단하게 지원하기 위하여 설계되었다고 Sun社는 밝혔다．


  원래 Sun은 지금으로부터 1년 후 예정인 EJB 2.0에서 entity Beans어］ 대
한 지원을 제공하기로 계획했었다. 그러나 " real中life business entities" 를 위
해서 이 기술을 추가했다고 밝혔다. 분석가들은 Entity Bean을 도입하려는 움
직임들이 예상보다 빨리 이 기술을 도입하도록 한 것으로 보고 있다．


  EJB 1.1 스팩은 오는 6월 14일 샌프란시스코에서 열리는 JavaOne 컨퍼런
스에서 선보이기로 예정되어 있다. Patricia Seyb아d Group의 분석가 Anne
Thomas는 이 스팩이 Java 2 , 보안 모델, 그리고 EJB 적용 선택 사양에 묘사
퇸 XML을 사용하기 시작함으로서 EJB의 보안을 개선시켰다고 밝혔다. XML
기술은 EJB 1.1을 지원하도록 출시될 EJB 애플리케이션 서버의 중요한 기술
이 될 것이라고 한다．


  EJB 1.1 기술은 이전 1.0 버전은 각 bean을 위해서 분리된 전개 파일을
요구했기 때문에 훨씬 매력적이 되었다. 이것은 많은 Beans로 이루어진 큰
어플리케이션이 곤란한 상황에 빠질 수도 있다는 것을 의미한다. 그러나 EJB
1.1에서는 하나의 파일이 EJB의 모든 파일들을 그룹화 하고 XML 디스크립터
파일이 Enterprise Bean의 요구사항에 대한 실행 서비스를 훨씬 유연한 방법
으로 정의한다. 그리고 서버 전반에 걸친 속도를 향상시키도록 돕는다．



                          - 264 -


===== PAGE 268 =====
부        록




    - 265 -


===== PAGE 270 =====
부록 A : Java 의 구문 요약


- Java 언어의 구조
                             呼小颱


    ,,.「的.回r ""'                                        /／패키 지 지정
     import java. a叫t . 火；
                                  \ 螂如崑 ．전러 두"4의 // 패키 ' 1 포하
                                                            "
     import java.uti l .Date;      "   착이는 孚댜．
    口ubl ic 이ass ImageButton extends Button { // 클래스 정의
          private String imagename:                     // 멤버 변수 선언


          publ ic ImageButton() {                       // 생성자 메서드
                this( "/ tmp/duke.gif ") ;
          }
          publ ic lmageButton(Str ing imagename) {       // 생성자 메서드
                this. imagename = imagename;
          }

          public,Image
                  voidimsetLabel
                         = getT。
                              ,(。ikit
                                Str,ing .getlmage
                                               (imaaej-
                                                 {,II iam
                                        imagename)
                             :0n丘 1野j1 人y／춈티 弓t 中唯也
                                                        e);尸o""'a邕 )
                                                       OIIAI
                    米 어語 d사（汁                侘 ( (',1卵'1 咤" 1"卜


               ，
               卜, F,, '宦브且 口世뜨그三H
U 클래스의 구성            ．삐측 畔너，屈堪？叫n , ,                    今言애坰 기능아 운呼仍小畔
                                             匙t,
                     나'빠1t9, r.A1t’ 旴 ' rh乂例d'r/          奴袍社 운嶝m洲미 따斗
 H 변수 : 멤 버 변수 , 지역 변수                                      碗拉t 威7卜 自？1.
 e 메서드
    modifier type name (parameter) throws ... {}


                                叫 267 -


===== PAGE 271 =====
                                        艸孝 내畔柑                     섭“" "r능·
                                 ' 茯

H 卜加difier
                                                               ·



                                 \      냐꺼斗. 할푤
                                             학를 1믿쎄et
                                                ’믿쎄er 好1苞
                                                           "
                                            小니
                            k：
                                                                          '그卜손心仕恥A   ？亂
  클래스                                     final,
                                                                         伊＝抄녹亡或皿江4芒
  변수                   巾rotecte쳐,                defau仕，
                       "'            ，니／니        사色m냐 낱斗                （小벼   섬근 ?｝는
             static,   final,          transient, " volatile
  메서드
             自西 亘玉a 區itt) 區西
    ,刪， 然쁘 嶝．       ，少'' te(ract,
                   ' 나l'' I'      , 等｝
                                   native,
  尸1：面'C百啼-,- 0t旦．            q4더므二    아 - synchronized
                                         북才능
  메서드 오버로딩과 오버라이딩


  오버로딩 : 메서드명은 동일하고 매개변수 사양이 반드시 톨리게
  오버라이딩 : 부모 클래스의 메서드를 자손 클래스에서 재정의

                메서드명 , 매개변수 사양, 리턴값의 유형등 모두 동일하게


U 클래스의 활용
  尸 상속 (extends)
       class A extends B {}
  H 객체 선언
       Date d = new DateO;
       생성자 메서드（Constructor)


H 데이 터 유형
  H 기본형
       byte, short, int, tong
       float, double
       char, boolean


     참조형／객 체 형
       클래스형 , 인터페이스형 , t내열

                                                 - 268 -


===== PAGE 272 =====
H연산자

               단항 연산자            ++             e   小       +

               산술 연산자            永 /                %
                                 +     -




               쉬프트 연산자           << >> >>>
               비교 연산자            < <= > >=                      instanceof
                                           !=
               비트 연산자            &     八                1
               논리 연산자            邑＆ I I
               조건 연산자            7 :
               할당 연산자            =    op=



寸 제어문 : 조건부 분기문 : if
            다중 분기문 : switch
            반복문 : while , 化r, do- ＼사hile
            제어문 : break, continue (label 사용）


1 배열
                                                                      竹 ,11！丸
       m t su[ ] =new intElO]; 卜啼＼      ，夕＜                                    1盼k」
                                                                                  서는 佃넴14 *
       String s[ ] = {"abc", "def ", 너23"}; 巾呼L: 3,                          2陪로 札섣 .

       m0t num [1[1 =쁘多呵｛{ ,2,3},{4,5}};
U 메서드 정의와 호출


 정의 : 헤더（header）와 코드（body)
         명칭 , 리턴값의 유형 , 매개변수 사양 , 지역변수


 호출 : 메서드명（매개변수）;




                              - 269 中


===== PAGE 273 =====
e 예외 처리                   1 enlm e卜
 H 발생 (throw)                           埠口 쁘 '叫'小（鷺깜d《
      」」
       ［茗才，으，,"“,), )
                                                 枷M         (mt人／                        .
                                                                                                       1
                                                 丁”               "                , "           ( 赴겅叫 의弩 6乂印十」


                                                                                                                                           )
                                                      5 더t켜J卜                      C'어月너 ' 啼缸너 .                                           1


小的心叩．                            .                                    （       「；    ，尸                “니       "       "   ":   '" '
                                                                                         r\ =J             -
            I11M스L二．.4LJrn1AI i4-그 tl. 二4,Ll                                       기3入I기 둥．

小O
 xI D1I1臭再罷-Ithis-()뇨茹"已然，1；卜 '" ,
                                               쓱 4ya戶分工J ,,m中tW,
                                                            I
                                                               ，이 U4e仇er뇨t"




  abstract 클래스
                                                 e汽   'rt     "
                                                              '       악 '硏                       '   즈드' 1 볘티li    ·                   ·




     '／눙饒 훌洲卵t 趨 '"比
- final 클래스
       얘체       化성만， 升느

- Interface（인터페이스）

       d比fre十0卜 唯 . 砧竿르岵
- Inner （긔ass
  Inner Member Class
       Static Inner Member Class
       Instance Inner Member Class
  Inner Local Class
       Named Inner Local Class
       Anonymous Inner Local Class

                               W邸
            ：고寸
              "
                           >



" '‘ 「「
      ，',梯，":                                         H畔 뇜比梵：
                                                             ; 斗으의 琶 C-卄毘 斗가m1
  내부적 형변환과 강제 형변환
  기본형간
                                                                      ）卜人三으t칩드 낱星 4印
  참조형간
  기본형과 참조형（wra口口er 클래스 활용）
                                     - 270 -


===== PAGE 274 =====
     부록 B : SQL 요약


     SQL 은 표준화되어 있기 때문에 플랫폼과 다른 제품간의 이식성이 매우
높아 데이터베이스를 관리하는 표준적인 언어로 쓰이고 있다. C 나 \uisual
Basic 이든 구현 언어는 상이해도 데이터베이스를 콘트롤하는 것은 결국
SQL 로 모두 처리된다.             이 절에서는 SQL의 기본 문법으로서 \Ueb 을 통한
데이터베이스 연동시 많이 사용되는 과정들과 관련된 문법에 대하여 소개한
다．
     가.   테이블    생성


     테이블 생성은 CREATE TABLE 문으로 가능하다. 형식은 다음과 같다：


           CREATE TABLE table_name (
                col_name   col_type [, col_name   col_type,...]
           );
      열은 필드라고 불리우며 , 복수개의 필드가 모여서 하나의 행 즉, 하나의
     레코드를 구성한다．


      CREATE TABLE sample (num int, name char(30));


     나. 테이블 삭제


      테이블의 삭제를 위해 SQL 문에서는 DR아） TABLE 문을 지원한다. 형식
     은 다음과 같다：


            DROP TABLE table_name;



                                 - 271 -


===== PAGE 275 =====
다. 행의 삽입


행의 삽입은 INSERT INTO 문으로 지정한다. 다음은 INSERT INTO 의
일반적인 형식이다．


    INSERT INTO table_name (column t, column])
         VALUES (value [, value]);


 VALUES 어］ 명시되어 각 열에 삽입되는 값들은 해당 열의 데이터 타입
과 일치해야 한다. 다음은
 INSERT INTO 문을 사용한 예제이다


    INSERT INTO sample VALUES (1, ' 홍길%');


라. 행의 삭제


 특정 행을 삭제하기 위해 사용되는 SQL 문은 DELETE FROM 문으로
서 형식은 다음과 같다：


     DELETE FROM table_name
     WHERE column OPERATOR value
     (AND I OR column OPERATOR value];


 WHERE 절은 CGI 와 DB 연동 프로그램에서 가장 많이 사용되는절이므
로 반드시 그 구현 방법을 알고 있어야 한다. WHERE 절의 기능은 원하는
내용의 DB 를 얻는데 있어서 조건을 줄 수 있는 절로서 여기에서는 삭제
되는 행에 대한 조건을 지정할 수 있다. 조건 연산자는 <, >, =,          >=, <>,
LIKE 를 사용할 수 있으며 LIKE 어］ 사용되는 와일드 문자는 'H' 와 ' %' 로
서 각각 한 문자와 모튼 문자를 표시한다. 다음은 DELETE FROM 의

                             - 272 -


===== PAGE 276 =====
예제이다：


    DELETE FROM sample WHERE num = 10;


마. 조회


 DB로부터 정보를 추출하기 위해 사용되는 명령은 SELECT 문이다．
SELECT문은 행의 범위를 정하거나 특정 행을 지정하기 위해 사용되며
DELETE, UPDATE, INSERT 등의 명령들과 함께 결합되어 사용될 수 있
다. 또한 WHERE 절을 사용하여 조건에 맞는 행들만을 추출하여 동작을
처리할 수 있다.      다음은 SELECT 문의 일반 형식이다 :


    SELECT [table.]column [, [table.]column]FROM table [,table]
    [WHERE [table].column OPERATOR VALUE
    [ANDIOR Etable.]column OPERATOR VALUE]]
    [ORDER BY [table.]column [DESC][,[table.lcolumn [DESC]]


 각 조건은 AND, OR로 연결 가능하며 , ORDER BY로서 SORT 기준열을
지정해둘 수 있다. DESC 는 역순으로 SORT 됨을 의미한다. 다음은 간단
한 SELECT 문의 예제이다：


    SELECT name FROM sample WHERE num = 10;


바. 데이터의 수정


 특정 데이터의 수정은 UPDATE 문으로 가능하다. 다음은 UPDATE문의
일반적인 형식이다：


    UPDATE tab旭小nan犯 $ET c이umn=vaJue [! C이umn=v히ue]

                           - 273 -


===== PAGE 277 =====
    WHERE column OPERATOR value
    [AND I OR column OPERATOR value]


    UPDATE sample SET name='* 니코' WHERE num = 10;


사. 존재하는 테이블 점검


    select * from tab;


아. 특정 테이블의 필드 점검


    desc 테이블명；




                          - 274 -


===== PAGE 278 =====
부록 C : Java Type 과 SQL Type


SQL Type         Java Type


CHAR             Str ing
VARCHAR          Str ing
LONGVARCHAR      St r I ng
NUMERIC           java.math.BigDecimal
DEC나viAL          java.ma卄｝.미gDecimal
BIT              boolean
끼NYINT           byte
SMALLINT          short
INTEGER           nt
미（引 NT            long
REAL              f loat
FLOAT            double
DOUBLE           double
BINARY           byte[ ]
VARBINARY        byte[ 1
LONGVARBINARY    byteE]
DATE              java. sql .Date
TIME              java. sql .Time
TIMESTAMP         java. sql .Timestamp




                             - 275 -


===== PAGE 279 =====
부록 D: CORBA 오류 코드


ORB Minor Codes and Their Meanings Code Meaning


BAD_PARAM Exception Minor Codes
1     A null parameter was passed to a Java 1DL method.


（兀MM_FAILURE Exception 卜川nor （元des
1     Unable to connect to the host and port specified in the object
      reference, or in the object reference obtained after location!
      object forward.
2     Error occurred while trying to write to the socket. The socket
      has been closed by the other side, or is aborted.
3     Error occurred while trying to write to the socket. The
      connection is no longer alive.
6     Unable to successfully connect to the server after several
      attem 아S.


DATA_C0NVERSI0N Exception Minor Codes
1     Encountered a bad hexadecimal character while doing 0RB
      stri四_to_o히吼t operat幻n.
2     The length of the given l0R for string_to_objectO is odd.
      It must be even.
3     The string given to string_to_object() does not start with l0R:
      and hence is a bad stringified l0R.
4     Unable to perform 0RB resolve_initial_references operation due
      to the host or the port being incorrect or unspecified, or the
      rem아e host （如es n아 su야兀rt the Java 1DL bootstrap 아아occ놔．


                               - 276 -


===== PAGE 280 =====
INTERNAL Exception Minor Codes
3     Bad status returned in the IlOP Reply message by the server.
6     When unmarshaling, the repository id of the user exception
      was found to be of incorrect length.
7     Unable to determine local hostname using the Java APIs
       netAddress .getLocalHostO .getHostNam eO.
8     Unable to create the listener thread on the specific port.
      Either the port is already in use, there was an error creating
      the daemon thread, or security restrictions prevent listening.
9     Bad locate reply status found in the IIOP locate reply.
10    Error encountered while stringifying an object reference.
11    IlOP message with bad GIOP vl .0 message type found.
14    Error encountered while unmarshaling the user exception.
18    Internal initialization error.


INV_OBJREF Exception Minor Codes
1     An OR with no profile was encountered.
      MA只SHAL Exce口t向n 卜川nor （兀des 4 Error occured ＼사hile
      unmarshaling an object reference.
5     Marshalling/unmarshaling unsupported IDL types like wide
      characters and wide strings.
6     Character encountered while marshaling or unmarshaling a
      character or string that is not ISO Latin-i (8859.1) compliant.
      It is not in the range of 0 to 255.


NO그MPLEMENT Except幻n 卜川nor Codes
1     Dynamic Skeleton Interface is not implemented.




                                  - 277


===== PAGE 281 =====
OBJ_ADAPTER Exception Minor Codes
1         No object adapter was found matching the one in the object
          key when dispatching the request on the server side to the
          object adapter layer.
2         No object adapter was found matching the one in the object
          key when dispatching the locate request on the server side to
          the object adapter layer.
4         Error occured when trying to connect a servant to the ORB.


OBJ_NOT_EXIST Exception Minor Codes
1         Locate request got a response indicating that the object is
          not known to the locator.
2         Server id of the server that received the request does not
          match the server id baked into the object key of the object
          reference that was invoked upon.
4         No skeleton was found on the server side that matches the
          contents of the object key inside the object reference.


UNKNOWN Exception Minor Codes
1         Unknown user exception encountered while unmarshaling: the
          server returned a user exception that does not match any
           ex口e（乂ed by the （기ient.
3         Unknown runtime exception thrown by the server
           implementation.


    Name Server Minor Codes and Their Meanings Code Meaning


    INITIALIZE Exce口tion 卜川nor Codes
    150    Transient name service caught a SystemException while
                                     - 278 -


===== PAGE 282 =====
       initializing.
1 51   Transient name service caught a Java exception while
       initializing.


INTERNAL Exception Minor Codes
100    An AlreadyBound exception was thrown in a rebind operation.
1 01   An AireadyBound exception was thrown in a rebind_context
       operation.
102    Binding type passed to the internal binding implementation
       was n아 텨ndingTy口e.n야恥ct or 텨ndingType . ncontext.
103    0bject reference was bound as a context, but it could not be
       narrowed to CosNaming.NamingContext.
200    Implementation of the bind operation encountered a previous
       binding.
201    Implementation of the list operation caught a Java exception
       while creating the list iterator.
202    Implementation of the new_context operation caught a Java
       exception while creating the new NamingContext servant.
203    ImpIementaton of the destroy operation caught a Java
       exception while disconnecting from the ORB.




                                - 279 -


===== PAGE 283 =====
부록 E : CORBA 지원 Brocker


Company       마oduct (al l R)              Ma口口ings
BEA Systems   ObjectBroker                 C, C++
Chorus        COOL                         C++
Expersoft     PowerBroker CORBAPIus        C++, Java
IBM           DSOM                         C, C++
ICL           DAIS                         C, C++, Eiffel
Inprise       VisiBroker                   C++, Java
lona Tech     Orbix, OrbixWeb              C++, Java, SmaI lTalk,
                                            Ada95
Nor tel       RCP-ORB                      C, C++, Smal l talk
Paragon       Oak                          Objective-C, C++,
                                            Java
Sun NEO,      Joe                           C, C++, Java
              (being discontinued in favor of VisiBroker)
Tibco         ObjectBus                     C++




                             - 280 中


===== PAGE 284 =====
부록 F: EJB 을 지원하는 Application 서버


Company Name             Product Name               URL


BEA Systems              BEA WebLogic               www. weblogic. com
BEA Systems              M3                         www.beasys. com
Bluestone Software, Inc. Sapphi re/Web 5.1          www. bIuestone. com
BROKAT Infosystems, Inc. BROKAT Twister             www.brokat. com
Bul l                    Bul 1 Soft Appl icat ion   www. openmaster. com/ejb
                         F기 at form
Forte Software, Inc.     SynerJ/Server              www. forte. com
Fuj i tsu Software       Interstage                 www. fsc. fuj i tsu.com/
Gemstone Systems, Inc.   GemStone/J                 www. gemstone. com
IBM Corporat ion         CICS Transact ion Server   www. software. ibm. com/
                                                    ts/cics
IBM Corporation          Component Broker           www. software. ibm. com/
                                                    ad/ cb/
IBM Corporat ion         TXSer ies                  www. software. ibm. com/
                                                    ts/ txser ies/
IBM Corporat ion         WebSphere Appl icat ion    www. software. ibm. com/
                         Server                     websphere
Inpr ise Corporat ion     Inpr ise Appl icat ion    www. inpr ise. com/
                         Server                     appserver
Luna Information         The Agi le E-Business      www. luna. com
Systems                  마oduct S山 te
Netscape Communicat ions Netscape Appl ication      www. netscape. com
Corporat ion             Server
Oracle Corporat ion      Oracle Appl ication        www. oracle. com
                         Ser以가 4.0

                                  尸 281 -


===== PAGE 285 =====
부록 G : Java 관련 유용한 URL


 JDK 툴

   ht tp: //java.sun. ccm/products/JDK/1.2

 JRE(Java Runt ime Environment)

   ht tp: //java.sun. cc*nlpro加cts/ jdk/1.2/ jre/ index.htnil

 JDBC 관련 정보

   ht tp: //java.sun. c이!prod兀ts/ jdbc/ index.html

   ht tp: //develo思r. java.sun.cctn/develo比r/Bo出；s/J版江utorial/ index.html

 Serv let 프로그래밍 API 長 엔진

   ht tp: //java.sun. ccin/products/servlet/ index.html

 JAVA IDL(Interface Def inition Language)

   http: //java.sun. ccin/products/ jdk/idl/ index.html

 Java 관련 Product

   ht tp:I/ java. sun.cnm/products/
 Enterprise Java 프로그래밍 관련 자료와 툴

   http: //java.sun. canlj2ee/

  다양한 Java 기술을 공부할 수 있는 Sun 의 Java Tutorial

   ht tp: //develo思r . java. Si.끄1. can/dev이야比r/onl inelr諦山回

    http: //develo祀r. java.sun.ccin/develo比r/onlineTraining/Downloads/index.html

  Java Language Specification
    http://www. javasoft.ccn/docs/books/ jls/html/ index.html

  J avaBean 정 보

    ht tp: //java.sun. cin/beans/

  Java 개발자들을 위한 사이트（다양한 기술 정보 제공）

    ht tp:I/ develo思r .java. sun.ccin/develo思r/

  JavaWor id게서 제공되는 Java Tip Index

    http://www. javaworld.cin/ javaworld/ javatips/ jw-javat ips. index.html

  IBM 의 Java 콴련 주요 기술

    http://www.develo比r. il工i.cciii/ java/

                                             - 282 -


===== PAGE 286 =====
  ht tp://WWw.a1phaworks. ibn.cctnI
윤경구라는 분이 운영하는 Java 관련 정보

  ht tp:II呱丑l.daewoo.co.krf-yoonforhltutoriall
DHTML, JavaScri1亢 관련 최고 사이트

  ht tp:/Iuser .chollian.net/싸spacekan/
다양한 기능의 Java Applet 과 Java 관련 정보
  http://www. javaboutique.com/
Net scape케서 지원하는 Java 기술
  ht tp:IIdeve1o思r .netscape.aiiiltech/ java/ index.html?content=/support/ faqs/

                      cha町加fls/ j카a.htnil
Java 로 개발된 상품들

  http:IIwi. deveIoper. ilxn.ccxiiljaval
IBM 의 끼sual Age 정보
  http: //vaga. fl毗.org/devel0per/software/sdk/age. ipc
HTML, JavaScriptSelfStudySite (HTML 4.0 한글 문서)
  http:IIvWw. trio.co.kr/
ORACLE 관련 기술적인 내용들
 ht tp:l/ ns. fornian.co.kr/寸ltl im




                                      - 283 -


===== PAGE 288 =====
Enterprise Programming with java
발행일 : 2001 년 7 월

발헹쳐 : 삼성SD$ 멉티껌퍼스
        서울특별시 강남구 역삼동 718小
        TEL : 3429- 5114

인쇄처 :   건 양 사




 米 본 교재의 판권 및 저작권은 삼성에스디에스의 소유이므로
   무단전재나 복사를 금합니다．


===== PAGE 290 =====
http://www.multicampus.co.kr




                               삼성SDS
                               멀티캠피스
