---
source_url: /run/media/yutae/Data/해답_microwave_engineering.pdf (USB, 2026-10-25)
ingested: 2026-10-25
sha256: 79511245fa2cd2e7b840d5e6bed809dcd812ace512e0ba6100d04b2420a9e007
---
# Microwave Engineering — Solutions Manual (raw source)
> 텍스트 레이어 PDF → pdftotext -layout. **수식 대부분이 깨짐**(한국어/한자형 혼입, 기호 치환) — 본 래퍼는 구조·계산 단서용이며 정답·도식은 로컬 원본 PDF 대조 필수.
## Book metadata
- title: Solutions Manual for Microwave Engineering
- author: David M. Pozar (University of Massachusetts at Amherst)
- publisher: Addison-Wesley Publishing Company, 1990. ISBN 0-201-50419-7
- pages: 253
- source file: /run/media/yutae/Data/해답_microwave_engineering.pdf (USB, 2026-10-25)
- scope: [[microwave-engineering]] 제2–12장 교내문제(home problems) 281개 전수 해법; 일부 설계 문제·소형 프로그램 작성 요구 문제 포함
## Chapter structure (원서 Ch.2–12 순, PDF 페이지 기준 추정)
| # | topic | rough pages |
|---|-------|-------------|
| 2 | Electromagnetic Theory | ~6–18 |
| 3 | Transmission Line Theory | ~19–79 |
| 4 | Transmission Lines and Waveguides | ~80–99 |
| 5 | Microwave Network Analysis (S-parameters) | ~100–109 |
| 6 | Impedance Matching and Tuning | ~110–139 |
| 7 | Power Dividers, Couplers, and Hybrids | ~140–159 |
| 8 | Microwave Resonators | ~160–199 |
| 9 | Active Microwave Circuits | ~200–209 |
| 10 | Filter Theory and Design | ~210–229 |
| 11 | Ferrite Components | ~230–249 |
| 12 | Detectors and Mixers | ~250–253 |
> 주의: 장 시작 페이지는 문제 번호 패턴(2.x, 3.x …)으로 추정된 값. 본문 텍스트 레이어가 수식 혼입으로 장명 표시가 거의 없어, 위 구간은 대략적. 정답 검증 시 원서 PDF의 장별로 직접 확인 필요.
## Original text (all 253 pages)
                                          Solutions Manual




伊豆布藝魂. 4區乙，
 David N. Pozar'i,
 University of Massachusetts at Amherst
                                             Solutions Manual

Microwave Engineerin
                                                                     g
David M. Pozar
University of Massachuse
                           tts at Amherst




     A
    TV Addison-Wesl
                    ey    Publishing Compan
                                               y
    Readw乳 Massachusetts
                          . Menlo Park. California
    Don Mills. Ontario ·                           . New York
                         Woking'nam. England
    Sydney - Singapore                        · Amsterdaml - Bon
                         - Tokyo , Madrid                        n
                                               · San Juan
       h{ d441!




   口
   ： i1111甘




44;4d4a堪m准也冬 4非｛1
                    R町）roduced by Addison-Wesley from camera-read
                                                                  y copy
                    supplied by the authors.

                    Copyright @ 1990 by Addison-We1町 Publishing Comp
                                                                             any, Inc.
接
                    시1 唯hts reserved. ｝的 part 可 this publication it狙y
                                                                           be reproduced,
                    stored in a retrieval system, or transmitted, in any
                                                                         form or by an '
                    means. electronic, mechanical, photocopying, recording,
                                                                               or otherwise,
                    without the prior written permission of the peblisher. Printe
                                                                                   d in the
                    United States of Am비ica.

                    ISBN t)-231-5C419-7
                    A표工三F竹스i-93210
                                           Solutions Manu
                                                          al for
                                          MICROWAVE ENGINE
                                                           ERING


                                                    Preface
                  This manual co
                                     ntains solutions
            problems in MIC                                       for all        of the hom wo
                              ROWAVE ENGINEER                                                       rk
            problems, in Ch                            ING.      Th ere are a tota
                               apters 2 through                                           l   of 281
            very easy, while                            12.      Some of these pr
                                  others are leng                                        oblems are
            number of the prob                            thy and cha1len
                                 lems ask for th e                                 ging-     A large
           or circuit.    A few require th               design of a parti
                                               at                                 cular componen
           to simplify the ca                       a   sh or t computer progra                       t
                                  lculation of data                                   m be written
           results or mater                                .    So me  of the proble皿S
                               ial discussed in                                               extend
                 I feel th at work                      the text.
           learning proces            ing  pr ob lems is a very im
                             s for students                                 portant part of
           supple工nent to cla                        in engineering,                             the
                               ssroom lecture.                                   and a necessary
          to give the stu                               These problems ha
                              dent practice in                                     ve been written
          microwave engine                               applying the ba
                               ering, and practic                                 sic concepts of
          practical microwa                             e in th e analys
                               ve circuits      and components.                  is and lesi甲） of
          hom四ork proble皿                                                  They can be used
                              s, as ex리n prob                                                     as
          for students to                          lems, or as supp
                             work out on thei                                l到nentary problem
          needed, it should                        r own. If addi                                   s
                                be easy for the                            tional prcblenis
          from th ose in th                           instructor to de                           are
                             e text.                                            rive new problems
                The 끄lajority of
         result斗 c＜끄표pare           th es e solutions have
                              d 느uit虹 independe                     been checked wi
         case of many                                nt soluti （月｝$ by                     th known
                            of the design                                     ot：勺ers or, in t：上e
         simulation.     (Such solutions            pr  ob lems, verified
         the ansiers. ) Bu                     usually have a                        by computer
                              t th ere are undo                       small check mark
         1比이l detected.                             u此e끄y some erro                           after
                             了'he at工thor wo                                  rs which have no
         errors in thr te                        uld be gra七eful                                   t
                            xt itself)                                   if such error下r
                                            were brought to                                     佃r
                                                                     his attention.
         David Pozar
         Amherst




11可拿尤蕉
莩   U   1 肖
          口1 4$4크111   4d곁＝ 겁크計芟注3甘寸m
                      (．片月尸7石尺        긋



                     :：二亡亡＝
                          ：少戶之之
                      //7 , 小丑 A ' （尻，而戶工                            (6% 궁）· Yk          小       加q才 뇨片之
                     E)   크孑 q刃了‘     ！二 戶X可＋ j
                                                          " 3 ' 小加 戶뇨 尸幻仙斑
                     ／꺼4（妃才 ／亡，

                                  巨， = 슛／ &毛孑
                     和 訂O,                                             1金3＞今 瓦苡8ed好
                                                                                      丹坐 e5b
                                  用   “   多』   4ei                                           1


                     加出夕比 火'『幻／r卜
                                ", 如晦；, 和＝仄乞 . 恥匡石三, a441
                     和a B m 小枷乂 hm友五 名辰
                                              m也뇨小／
                     T뇨 小岫）
                                          小苡烏k 寸戶.                                  t毛17二小代 (2.36)m口／(2.37)·
                                                                                  口-
                          任1司XA = O                  :>       4 =B

                                                                     旦及
                                                     弓
                                                               //L
                                                                                  )
                                                                          十
                                                                              A
                                                                                                  小




                                                                              瓦
                              A = B = 口헤吼
                                      기 卜 月0




                                                          /

卜 ； 며 거 가 ==1J十띠깨斗
                                                                        也乃
十
        7X 百 = 戶／스 ？트
                             ' \ r E多                                           미午易아（측多 誓）
                                                                             \\17/




    7/ " =弔芬午二恥評 卞期

                                                                            磊 知          十 哥
                          尸
                          1
                          1
                          11
                           1
                           L
                                                                                                                             弁
                人
                中

                                                                                         느
                                                                       上r            中
                                                                                     1
                                                                                     >
                                                                                                                                   埠雨
                                                                                                   +
                                                                                                                                        嚆年］
                                                         +      +
                                                          乙 l




                愧
                八         L
                          戶L
                                                                上少11
                                                                       H
                                                                       了a            쓰갸            工了                     伊
                                                                                                                          J
                                                                                                                          昱 可 上尸    J
                                                                                                                                    尸        眄訪
                                                                                                             5 4 21才U
                                                                                                                                                  n



                                                         +                                                                                        1

                                                                                                                                                  1

                                                                                                                                                  1

                                                          =                                                                                       i

                                                                                                                                                  1

                                                                                                                                                  H




                                                                       쓰們                뜨抑
                                         l 11 口
                                              1
                                                                                          +
                                                                              上f
                          尸11111L
                                               1
                 A 月口11                          m1 1
                                                    H t
                                    nd

                                                                                                   上
                                                                                                   J.' a트므
                                                                                                       琶二工  . 9E芦
                                                                                                           그，     小
                                                                                                              2초 小旦］
                                                     P
                                    m卜
                                     C
                                                           十                                  11
                                                     1
                                         H   1
                                                     m
                                                     =



                                                                                                   r    a尸              f7 ' a伊    f7 ' -I




    \
                "出搗 寸 年 寸 諍 寸 翔
                4哮卄 !；千 磊 寸 身］
    무           따y亐 V. ' 力展且 智石／協Z 白中沆在力肥尸‘                                                                                         砒

        伊
            ？
                汀탁 十多V 'E .jv 'E吾
        H   二
                                                                                                             (TH巧 'S 肋T A Y0的 .5任尸！)
        E   H
            갸 Ii-帛 帑小架 윽3]
            나 ［卞 '知字 " 1 i斗牛］
            4［佇『 架 姑字『壽］
    冗七 X札J 亢뇨 ／까a; 匕小伽W出 卑 아7/g 口M 口（7·E）刃'i
    小 m 口計L二小 d쿠 Z吃（和사丘 戶口M丹 Q也 ／企才 幻J左dm比Z二｛已
    月寸 V' 百＋戶d"目沼呻（加'昏 丁hJ 솔 白나如方 q스드 伊 고·


                                                                                     又
            나1 "A+B
                                         j (- A1B) = 丁
        亡 (i-r)：和-B)                      （                         B) =   工吼
                                     {
                                                      ,4
                                 子
 油亡느 中            n7什伍           fl r ?17:                                      /
                                          7)1
                                          "1 + n1 Dl            '




 （티予叫W小 m뇨兀 如石77                                                                             （JH
           ，
    "三IO ' 二 小 小M 4뇨小白‘
                                                                                    ,   ，力




如           丁뇨 小如， 乃比旅/,                                                    岫乙／肛在
 C0和 ／亡 m小 Z乙叭 口勺


                                                     可'" "午位59）甘’"뇨孑                          （尸月C尸)



                                          小푸回小" （나／2 P)

                                                           "쿠
                                              :jt=
                       子＝0 2加妃


「뇨 P小危今出右4 m乙：                   佯-J勃／
                                     （刃汀少：朴
和
    " ' " "" “「「"'" '"D' (""'"『
                              " )" 恥 ' -in ' 姑뇨尸e2JO,)                                             /


如＞이 g' : 百亡x百t* = Z5 tEOl ' 口尸e戶2可孑 /
                       恥            U5mJG ‘丁／ r


姓'""' '" " '計"‘(「" ‘"-"r) "
  二     O   g

                         14:"'斗＝和岫/
                              1   -r)
  2\J




                           /./
                    다뎌h
               rH


     2.3                       I        -2j     0
                                                                    r




              L        J
                               乙
                               o        o
                                         3      0
                                               i/            三｝
                                                                                        /

             S " "小 " '" ' " 目月O 多尹O                               T卜t 四化k                  /mL 4             才九y
k·    9]
Fb十磁n？元 X凡mM 乂七們加4 4 好／ 石勺乙k兀 小包MZ
-7뇨 a- 加小吻／比 m掘小協듸 而 地W4 多尸如
／小恥r . ,// ／七毛                          Ca／뇨‘石毛                    fg．云             C沙七4, 才／工 C乙4工a{
加＋냔兀 7 L C 6七 小교d 勺 光札 小十寸戶小
師d 叱尸力盛／且亡＋ 加之 砒石7 尸和乙 加- -e
口入 me 加Q 7尤人 汕 , 山J 二냐 外 2凡 刃升咸无
      · 刃=          J/ 万   기                  寸_4___    /\




             丁뇨 如艸" / 仰7 石                                        꾸寸蜘 老姃 肛，m仙 在 石
戶似．
  e/         <：乙
                                                        m                               小
小／石 C伉.쿠瓦 又 加乙                                                                        M       H
                                                                                    （口4- 瓜 乙沆d戶：
                                                                                               占；-3기



毗弓，牙小Z 尸及似，仰化
                                                                            肛               i加a그円／.
                                                                                                ＜丁

                                                                                                              :

     i " = 굿 e口；凡手                                                  mJ
                                                                    H片

     갉汪 尸e；뇨孑
                                                                                                          ＜口
                                                                   U
                                                                   H    r
                                                                                                      子
                                                                                                                  =


                                                                                                     易< O
     픈 " : 玎Ae6桁作寸b
                                                                   肛打付好加士b 八恥4
                                                                            1   1                         나




r "苡了甘卄唵山                                                          qt= j. -F 甘J뇨岵刃                   > >C/
                                                                      吼
                                   口，   d ／了3 d                    二“「 nd yd 力                 06Z瓦니
戶‘4- 午吻吃危 戶                              口 T; A. E, :

                                                    3
                 工7       Fn力거凡 札力伍 2.1,

                      Y “如 仄；n乙"C 屈口玎i －戶 · 2玎（/ c00)
                                                                   寸   }    기   n   ．놔




                          " 9 " ／乃 『 只
                                       "*                  /9
                                                            「（ ＝《勺戶．
                                                                                         竹VM . 加a人．     /
                  小쓱乞 츠匡亘，/i;H        t                      110           3 77
                                                            匠万 " 2 3Z乙꼬f 『 /63/                」皿
                                       -j只／瓦；mm / E口
                                       \
                                       4
                                       J
                      F                    =H




                      ;
                      d                         </
                          D
            ／뇨
                                    E =r'尸百V. ' = 꾸三 (e"7孑 ,eY)
                               ｛기
                                " " 니 甘" }e「卑孑小（呼ejP31
            IE1 似             白風及力7 m泛孔 U九寸
                                                               四吃 尸沙 色 斗乍三磁／矢毛／
                                                                              .

                          名0
                                                                                                    \




                          60




114111 {r
                          。
                              = 5




                                                     느5=
    坦피 W毛 十呼 /y4而띠 M 和才 白加m乙 乂玖丑
    m小m品 ／加弩尻 力뇨 4枷才． 戶M八 乙石4 ;./,

    《：V능5=／프了 1 m                                                                       伊4                       已 『：5. g13/ /:7 ,，戶：
                                                                                                                                    《‘
    了. 하也4 ?0d23 a; 뇨仰土뇨니， aD乙7可" ' 17)4B ,
    a乙 可d亡：3.16 x,o5                                                         力          'Yf = /D . y.




                                                                                                         ' 下L
                    f               O<'      （人）                                    亡 ()11加）
            J0o用／／孑                   /, 5／入／口.5-

                    16-月孑


            ／口6-         U孑     I       i.   s／刃／


    2.    ? E,t才，,,, 丁仄及2 .2./,

                                  3c,"') 巾口a·．/) = 肋9Z끄으 二6.9 3勺"/0?＝乂勺"戶
                    卜jt4石：J- 2 'r(3o
                                                                                                                 -5乙
                                Yb.          .            .   ,        :     327-            .211乙쯔二         "

                              Yer（亡J ' //
                                        .

                                                                           工73／二호k
                                                                                         :
                    小』
         :a) PA＝凡 5 1른S（子二이’ 亡 = 天e 5                                                                  /0y        Z=         4'5. f        w/mZ
贇                        ,          (                             nX                J            L2ig／二互二.5
            r
                '   ＝    니          4            }=               /:
                                                                             20c-
            巨r = I 百. （乙＝i) e了q戶지 = 中／00 긋 e尸Z77ey}                                                                                    / -2K2
                                                                                                                                      ( e
                                                                                                                                                 -
                                                                                                                                              二 (7.//4')
                                                      Q



            ？卜＝ 乳수 唇（y"／· ! = 忌5 브므少？ - ,. . 59                                                                                        巴   ',   I.   -   1 '


                                        뇨                         가升                J        (. 기9／프그 -J

    (b)     巨士＜i;＋죤r
                                                                                                                               八


            틱（二：이： /00꿎小三" J I)                                                                       展（訂이 : ":" y /／十三' ？乂)
            2乙，二 已）E*x츨 "3{ " 忘L玉프丑小乃小亡" 카小｛르프劣 寸乙O "／勻'
                                                                                             .   小9                    ' L                                     .




    b寸 已m. 'I三． Wm乙．
                   ／伽小 . P; cL.J P
                                 「 虹 m才中 나少M나
    加4小y比 和 0- 石 彦 Mm加小八 '
                                                                                             6
                                   2.／口
                                                        刀m 如J Md 加／/
                                                                     7小U他砬 규今；
                        阡呼苾芎 尸毛me 加切4- Em
                                          八· (2./)) -（乙/33기口                                                                                        肛仰d
                                 廂日De弘' (' 烏"名的키
                        目＝ A但／k더喀』

                                       片
                                       小
                                           : ；쏘4 e卄' 的qP' 4m助
                                                                                                                                   戶챰     < O


                                              吼 1

                        다5侄的
                                                                           和8ie
                                                                                            "   "" 띠 " '     蜘
                                                                                                                     ")
                                                                                                                              7>
                                                                                                                                   .


                                                                      ＜．
                                                                                                                                       戶 5 ""
                                           = 旦 q e口缸枷如d和四2.)人 n너U
                                                                                                                          J
                                                    B
                                   小
                                           2
                               H
                                                可
                                                              厄m匠司 花＝ 唇在 ,                                       小
                                                                                                           和＝／玩 . 꺄4./7i.
                       4竹 而M뇨쁑 的出烏4- 寸孑 “m

                       私（瓦- E1) 初 수 肛加夕，ed七？叫之 '3口.尸：ed缸4在夕： :.

                      訃（瓦－瓦）＝孔今和作' 싸"寸可"“ ' 烏"
                                                                                                                                         =－品可」平'
1
1
小
1느                    戶小七 仰机十1 加之m四才11如之 志／m＝乂烏
                                                硫寸·
                                                        '             易：4山7卞/-k ',                    叭：H갸／k                            似才h在V{ 戶＜尖口）



4 ! i44h4 r;1444在甘m
                      丁卜工人人／
                                                                    A CoP1 = 乃 白＜7 夕2.                 A     B
                                                                                                  )   ；亡 十；
                                                                                                       ' to
                                                                                                             ;H =
                                                                                                            1\
                                                                                                                          叫
                                                                                                                                   J;
                                           n=                  小그b!m. 白d夕2
                                                                                                 )      B=      小r。끄吼 <bdP/
                                                        11 口戶仇＋弔 白寸夕／                                        11白d四：+7?.＜加口7

                      cK& }c:                           LF 弓＝o,                   fl4EJ     9= 92=0 , AJb                 A= 8= 十J汭吼.
                                                                                                                                                J
                                                                                                                                n+ 7k,
                      UJHtC-                   A&！之EES>                    ')J (IH        P$-OBLEM 2 . I         J
              刃n 丁뇨뇨 km匕日 入뇨 ／乂工流 江 名 /A9 尸枷片／4Z
              尸仇出／J a4 V（品花 댜-4, 平 m兀듀 2. ?/ 恥戶／7gL Z乂兀
              比戶畝：m4 甲次규z, 1'，꾜 刃2. r뇨似，
                        礎口 4山回．= 促口 戶뇨 夕,,    色 三俑 夕亡


              r: fl dd& -)1                       丁＝       又 刃 Q（夕‘
                                                                  "
                     恥D4四亡 ＋吼 (d4夕／           1
                                                       小a也日亡 十／7口 匕ddd/i

                끄네。'Y1可·
              Tk+ -w印 /e 二 m恥也
                                             口努五 今／ 戶初· ／砬 多枷
                                                                           包
                               7tC04日亡 " 小 的夕4'


                           尸" 小葦m'4 ' m' 小44
                           "
                           꺄（／寸戶i斗 /－少云
                              지
                              『：/ · 丁万i4 ／누y4二i1 4
                                                   小乎四 竹小
             /<r X未刃＋, ／뇨     4凡亡／ 8/2如抗
                                         口笞及 ／和겨ft芒／' /

             2. LZ   匕z們A, ／亡／4    戶寸在Z뇨；／그 元乂刃 4.伽工 口也 只k꼬
              阡尹力M뇨瓦 伽也伊Z 的戶 弔 在2彷' 2, ? ／싸才7石t
             ,＞亡凡 卄石尤aM 7 毛，也 ill) a／小· 丁／似／

나1Vhtb才4tt
               r= 7l匕d( 多.4 戶小 帥夕亡
                     拉；小；
                                                        7 1 f, ,-,, 夕. 」

                        : 瓦瓦                 ) I “肛규二；小『.
J

             口 弓如그瓦 따孑匠
                                   私a뇨 了
                              了1 白d夕i = 기. 的斗
                              m江M'升 : 寸／‘寸．4
                                                                                       ql夕．
                               겨2
                                (r- 크力b니zA夕
                                          , = -'I,. 小4q2刃

                                        -Ir       = 口／戶 시) S4J夕，"

                                                                                                                         /
                                   4.
                                        .   日：
                                                   「       小아-
                                                                             t,
                                                                                  牙；
                                                                                                   <    ]
                     4 易艸姓1 竹尼 平三／
                                  4 7余 力뇨 m八
                .／丁
                乙 /3 I／四 如U뇨毛 甲磁／ M 力m沚
                                           亡／／叱娩
                C石나 乂＜-   A人J4그Ze叭 匕24 ·．

                른j= a0 c父 tj 9) 甘j뇨孑                             m
                                                                     \
                                                                     /
                                                                                  m        프
                                                                                                                             t 1JU
                                                                                                                                             k    之口
                                                                                                             八UJ
                                                                                                   八X
                                                                                                   /r
                                                                                                    뇨                    e
                                                                                                                                                       (LHC尸：)


               탸 - E.(G 슛 , 小） &乞孑
                                                                            m景似卜中）&瓦孑
                                                                                       吼
               룐亡：E. 伍主 匕Uk ' 孑『耳qe-J뇨b
                                                                            "그 ""（缸可"耗乞恥e.'i"砂
               (r陋刃戶艸 似 쿠m力I 枷4小 m才比M甘才뇨
                                                                          md 法4似力m放可仰批4)



                                                                                                                     -Ej, ,                        c 4/.

                                                                                                                 十       H슥＞巾， 的比




j44寸4重d斗 4二
                                                                                               )
                                                                         기e 十）16                   rj
                                                                                                        =c
                                                                                                                     ·




              和力냐 加忖M갸Z屯 加m斗
                                   出-'4- 如娩（可，小／e
              X／此 戈 드y知尹和d 辰 和兀4
               月 = 月n     H
                                 4幻釘. 7在 七／金2트느／
              7乙i/d 兀中
                               A                 1 b1 2/
                          e戶 ＝文／;E0 eJn巴 加九
                                          .

                                            ＜나＼ 人4' 乂A-v                                       나M名，，二r三＜:,l/1．乙니" .
                                                                                                             r                           二   l/
                                                                                                                                     d




                                                       9
                           FMM "" '), 帥n／可E '万 ' 而， 丁뇨力姃今

                   后 ' b' 加才 ／노 a加／ 7乙勺 斗 E, 7余／石工 似mH
                   크b 衣， 石d4石44

                                  6' = . (q E'*dEge.）十9 (b'E?16.E5）十弘답
                          튼·i, = ExI니" 寸（t芦E, E! 十냠E芦E了十白1E31' 十E。 E吾n

                   丁hi+ 加a口｛力助工 帥47 a'目Ef 1-)tE亨Ey
                   力小辰及 m七比나
                                       Y 匕工「石눗 ·
                   (d吼 們교I            k] : ［日"퓨 十口小小-4- 似）

                   乙 /5               Px = -0 (ErEx -jXE)
                                      Tj = 已 &JXE tErE)              '
                                      D3二 e。a}


                              까 "1) U'P느 =Ee (r -x)E, j臼（Er.k7Ey ' 6。(& ’火7E
                                                                           『
                                                            『姚）今『Eo (E
                              丘 = L\ +j Dj : EKE사지EX 勺' E* (E        『 少入) 三



                                                                                 E E E
                                  댜



                                                                                         기111}1111111J
                                                                         1   r

                                               (Er-x)      O     0                  +

                                  그
                                                 <)     (Er十K)   0




 1Jd L丁n쩍1n1h斗팎n
                                                                                    m
                                        E0
                                                 0        0      I       H   느      兀d




                   2．川白尸됴多 (2. /.a3) cJ (z.i i) 如娠m-                                                     才
                   i亡 ＝凡 3; 二 忌 쇼力7     肛 私＋出M知乙勺4呼／甲而4끄끄及尤b二

                   弓y今白力旬4- 石m 4竹뇨兀而包a 7 (2.173) 牙示4-, O=-乞

mWn自n1기쏘彗社크
                   （已x七瓦廂小二＝ R小缸的X尻！그二疵m夙］ 갸我誌탸器
                           : 忌晦小mi枷夙） -C和旬夙 I ',쿄小그
                                             (4-o (2.17了） ／뇨     而在石，교）
                                                 未1八
                                                                八
                                      三
                                                                                                                                                              니J
                              2.17                      끄
                                                            1
                                                                                                                                          +
                                                        H
                                                 A                                                                                                                       八
                                                                                                                                                                               玉
                                                                                                                                  1
                                                                                                                                                  ＝
                                                                                                                                                                               H
                                                                                                                         +1
                                                                                                                                                                         八




                                                 小11d
                                                                                                                                              小
                                                                                                                                                                         八 八
                                                                                                             +
                                                                                                                                      1
                                                                                                                              1
                                                                                                                                                                                   5
                                                                                                                     1
                                                                                                                                                                         d
                                                                                                                                              +

                                                                                                                 t
                                                                    )b
                                                                                                             +d                                           O

                              F如才／뇨 j瓜二 7乙元乙在 m之 石才乂工 戶m 口ba
                              Eaj｝氏   (2, (3뎌）,C z.｛斗‘) J

                              戶 二＜口‘，                  宦， = 月了 e-. ' 休柱9닝 的' )

                                                   小恥X C。-'升恥이 L (x ' 겅.d
                                                 目＝ B了 甘j札（' 舛“*3的' )
                                                  區＝午，（友伽，*3岫砂可‘"杞（'枾' "和「I)
                              口伊3 小나甘 m／兀뇨 d夕亡
                              訃［i(/'7- i cd-)J :. 수Ae札／的 : Be-J ／帥’
                              和［q(dD山（d9] =3; 白 [-e帥小k工岫小 如十cL &jd缸샤
                                                                             二可dP
                                                                                「
                                                                         ：가,
                              F뇨 P如兀 加4Xi人5,                                    札／4外目
                              1卜J4勻

                                       A " , ! , , ejkO伽‘                                                J 6그：乎
                                                                                                              ， ej 屯G(C巾 夕
                                        귿 : m,了, A （可j뇨므  往' 크叫叫




＝七上小吼心醬紫m型宙泓峯雀b4蚤艮榜珏K4拓稍聲다卜
                                               그白40  j札L芦4,                     te:        ,.. 十q'd7 的夕J
                              Tk刃／在乙伍 泣工 石尤及兄 和긱入亡之 口／ ya
                                                                                                                                                      小            //m,, 衣‘
                              和쿄 勺         .1斗砥抑 。I 加沅乂 小d, bZ 工 加注夜 口； :
                                                                         (djk
                                                                                  '   [' M '   크封낱J的이．
                                                                                                                                                                    2
                                                                                                                                                                    d     /
                                                                                                                                                                          4

                                                                                                                                                                         닉
                                                                         ) 可j뇨 小mB+c砒7 q＜日J                                                                         =a
                                                                         L




                                                                                      71
                 b而呵               只7皿兀 m고血 和r4- A뇨 石占／戶四仍

                               푠 --U刀，丁，9 re小" X-4 6 . -Ld戶m뇨吾白回                                                 口＜a <X
                                  帥   '        Le:
                                                         j뇨／
                                                                             M尸 C』뇨궁』
                                                                                 －
                                                                                    됴什,        乂的刃
                                                                                                                     孑＞乂
                 CH EC }< ,'
                                7 P “디 乂뇨M 夕＝O m4 M                                         I回咫，

                                   訃 日끄 小                                     k' d
                                                                                     小n毛孑            1召1
                                                                 LeU뇨系 ＋니瓦d
                                                     ,          {:“」
                                                                                                     7弓1
                  THIS     A6- _EES       Wilt-I               THE            RESOLTh i八'   (.z/ 7? )-(2.   18(1).




    U臂小4나m




mdad自겹牛口H노r（多t
                                                                       ./2
C月月尸／E1           3

3.1      了： 似們以口乞Liic卜帖恥2 g)的朴川＝／石匹쏘Y .9v旭昱끄．

            斗 2 '1. 3在쓰뜨"            . Z3-t-j 1拉3       M平斗和， Md/M .   /


      乙 "麝胥 762g．響學' = 2도孑/뜨 = z드g勺：，吐丸 /'
                                 V · 7y／互츠37-


                                     ' 2도g.j1- /（批乞 "
                                                           們7石二力my蜘욘）
                      C乂 = O


                      針回JZZ：누 : l 'i'. 3            /

可그 KVL:
   －寸（引『尺誓三回
           『呼 '：斗 尺爭고計好) *呼響芦2
         4- u- C-t스5) =o

C奴七白q 勺 勻 口M/ 兀／好＋" 石 尸 :
                           a2r倒 H
                                        十尺끄뒤크 쯔(J
                                               4- )              /
                           尸a3
                                                         口 L



卞a：工 :

  乂（3卜好E口十C 윷］［吼功－等k杜 읊江例 그Z計好）                                            二10




比i白在a겅 d8               \i       出才各＋. 只누尹才

                      沓3小丁m/,C "二"3j                             /




了m兀 人와교机 口尹i兀 M尹攻                                   (3. 2.，功 ·



                                        '3
        江키 ＋沙艸 戶竹勺 戶珏，E                                                              （兀1' </
                                                                                               H c亡L，凡 /<-
         亡l4d4七｝.,J</          (24J
                                                                                玹                                              厚
                  =:
                                                    Ey ' 芬 Vh, 玹去：平 可初
                                                                                譜
                                                                                                                       刃
                                                                                                             )
                                                                                       1
                                                                                                                   1
                           =
                                                                   M   끄
                       즌x百y = 3 朽1 /                     .


         Fi*力｝-, (3.ri) -L3. z.c).


         L: 告如' 六                                                  （吾) +
                                                                                               4뇨／
                                                                                               1人／
                                                                                                        H/
                                                                                                                  h1

                                                         未＝0 十＝6
                                                    町／
         C.
              二




         R=
                     m, = 碧n吾）'力＝
                  珂，，!
                    ，「
              G
                  쁑｛
                   「·"a5= 윅工쒸"六弓＝ 뜯"
                                  『 S/)
                                                                                                 =




    1
         tm工 m肛的Z吃 口7刀皿工 m元才又 名                                                 工 二 r。
                                                                                     ,4在 三／                                /
h
        3.q
          m似似 E孑：甘0 , 功x＝弓台(j=O. Tb石， 枷如姓
        蜘J 伊磁뇨 끄4뇨氾 去，

                  去        :
                               _       (4JA(   14x
                                                                                쓰가   -J口J(E工          (3-)


                  a=;m
                     E乂            .           ..            . .
                          := - 1 "／乂｛ t+ 켜                   12)
                                                                           르쁘스 - J幻亡E斗                 (i
                   a各          니
                                                                                                             ')
                                                                           C方
        닙i;M足 댜=O                  0.乂 7 ". M7＝比 小a 功r0, 竹之 市呻／ 뇨此 肛口·
                                       T＼工W (3) ／가兀.d                                              , 닢寸 小                       m


                                                                                     근午 J切4月k
                                                                                                                                                    警                    叫
                                                                                                                                                                                 匈
                                                                                                                                                                                     L
                                                                                                                                                                                         틔
                                                                                                                                                                     J
                                     -n口qr 丑十 드1: 才V（孑） 山．a   /
                                                              =
                                                                                                                          므W    끄                   가                            杯
                                                          \
                                                                                                                  X              2
                                                                                                                                 J
                                                                                                              !
                                                                                                                                                         뇨                               工
                                                      /
                                                                                                          y
                                                                                                                                                                             寸




                                     似名I工 的乂 帥計
                                                                                                 ＜勾＼{ J

                                                              ,

                                            Jj＝등了저 “ V好）
                                                 rd
                                                                                             ; J,w (9；可）
                                                                                                       ．弘，:-f二：a'：工.})
                                     T뇨.6"-,                                                                                             玄＝b




                                                                  겋多 ．」껍
                                                                       ‘ ／r好）                                             ：多＞       L : 二쁘
                                                                                                                                               /1
                                                                                                                                                    =J    -
                                                                                                                                                                 7


                                                                  弩
                                                                                                                                         w
                                                                    多 : -J'므투쁘 V(} )                                         』1 m 'e 'ii
                                                                                                                          => (/      y/                   1 4中 1 1 -
                                                                                                                                                          }：綴＋
                                                                  a各                                                      ＝多 c- 斗z ：二
                                                                                                                                   =r  규
                                                                                             八                                      ck
                                                                                                                                                         J h工十伍 ．스                                .
                                                                                                                                                                                                  .
                                                                                                                                                                                                      /1 ,   /
                                    3. 5                                  乙          凡   J
                                                                                         L三
                                                      碧
                                                              加   作


                                            匕                     上       뇨
                                                                          m   소          M
                                                                                             廂
                                                                                             耐
                                                                                             q
                                                                                                                  (a= /M씨 b: 3，朴H/ E戶2.
                                                                                                                                                                                 4'序J=．加砂
                                                                                                                                    =




                                                      之：
                                                                                                                                    丁：
                                                                                                                                         .5;
                                                                                                                                                    '/
                                                                                                                                                         3刃.7 득／$l i石-                       I-       c자4
                                       c.
                                            =.
                                                                  "   -       /72.
                                                                                              pF/                                   R斗薯mm/
                                      R ' 孕仕岵戶 3.&3 _P/,'.i




U44i44宴꾜乂횰＝1 心 士 七 m 立 n
                                      G= "乞少"                                            . 口／3q 욕／"1                  /



                                    瓦YGj：二 十

                         ＝ 르口亘＝ =
                                           ，電雲，39.3LL '

                                :
                                    了二出碼'叫（(:r+j叫                                            = ／口끄壘旦 二 ,30,'了 'Cs-




                                                                                              1．了
                                           7_




                                                        F                                                              (;
                            3.
                                                                          R5
                                                                                                    尺                      4




                                                                      g . 2yX兀＞ny
                                                                      z_ e X/ t -'                                                             /I

                                                        / /
                                                                      / . "3차0-。2
                                                                      i. '1) （八＞-2


                            （仄 小                                      似0皿 如弓 石之 m兀及烏／恥勺 力（兀
                                 明心伊小／乞 小m才才뇨才                                                                         a으 打針G乙）,                ( 3.93 a.)

                                 力'.4小 七 比뇨 ／伊긋 如札7甲 PM1-L- -- 3. c).
                            iAt小此m小甘加뇨兀亡力b才冗뇨戶I小y如m似
                            加 表名t戶，, ／了m （尺시厚) 4m{/ / 佃／）·




                              <  0
41\
                            db／꺼
                                                                                               ＜戶
r m j 4 身 量 花 八 i m m m 項
                                                                                           小
                                                                                                                                       /
                                                                                                                                   /
                                                                                                                               /
                                                                                                                       /
                                                                                                    ///       //
                                                                                                                   /

                                                                                                          /
                                                                                                                                                                 /
                                                                                                                                                               //
                                                                                                                                                              /
                                                                                                                                                             / /
                                                                                                                                                             /
                                                                                                                                                                     /
                                                                                   乙
                                                                                                                                                                 /
                                                                               ／
                                                                  q
                                                        ／戶


                                                        斥
                                                    ／
                                                              /
                                                              /
                                                              /
                                                卜
                                                                                       1                                                   I             t
                                     .01
                                                                                                    /6
                       3. 7    和＝ 及／
                                   乙 " .5-3十J. 266
                       FMW 石亡玟 山d,                                                 弘＝·拈5 .74           2d, -67 g 口' 百.2.5 n. /
                        SJR =- 2.Og                 ;                r= .3斗끄오쓰－


                       3. g                                            互
                                                        I
                               In                                            ==0. .2
                                          s-
                                    ;      e.  놔                 =
                                          ., 1- I
                                                                     2. S


                               汀I        근     （-
                                        ' 근二＋ 근。 i
                                                            2o
                                                                        )=
                                                                              j，
                                                                                   的－乙
                                                                              l ／口O+ 근b
                                                                                          ]
                                                                                          t
                                                                                                      근O a工d/Z.


                       古m吼， 尸
                            ，名 m4 斗乙＝及芬加i.O-
                                           .s2叱幻人
                       011                     Ioo- Z0
                                                                         = -0· 교 ＝수 乙＝Z니芒＝/00三
                                               }O<) 十근乙
                                                                                               三＝/3DJL什r     1
                                                                                                                 y


                       3. 'I
                               아：;?,' ,::?:: : ,功，塏: = .367L三 /
                                LOAD = 1rJc. -                                     二 F꼬NC. j_Ir/ t) = 3아／크．3'기' ] : 2도 '1w /


                       3.J0     F沆小H ．尤／，工 낳，뇨璥 CJm无
茸
                               ' 及＝恥늬加4뇨／占 =/0口山 二수 弘＝·亡J
                                                         '·r
                                r （이 二 . 62 戶9                                       』／




1 設發發求出m有峯纛珪） 姓煮雙！ :
                                r67A) 二 r乙2入） 二 ·6그／/                                         '   /

                       d겻和艸力나， 似小7夕 rr.）今 可可戶／=/끄쁘' :
                                        r (.7지＝ .(OZL크7 ' 끄 '/口 二 , EZ亡쯔I. = . 6之L쁘                                    V




                                                                                     17
                          尸
                          （:.ZD/7/r/                            5L人JR     fri          RL (d& )
                                                                          0. 0              的
                         Sw尺 二        /f/ /7
                                                                         . oo5                             '
                                      尸斤／
                                                                                            4,
                                                                           .
                                                                               0!                '/
                                                                                                               0

                          fri : 可凹2D                                     .0a9               32.3
                                                                         40316              30
                          I rj = 트그                                      .o '176            24. '/
                                      5十1                                ,07/               20. ?
                                                                          .10               그．0.
                                                                         e20                I         ".
                                                                         1引6                ／口．
                                                                          . 333              7，了
                                                                          . 9; 0            7. 36                  /


               3 .／又

                        Joy                                     乙＝ 80#j '/Os乙




                  乂＝.3入，                    和／6勺', g , 孑立‘ ..y6 .       근q :23J. Cf』
                                                                                   ，. s.c.)

                                     }＞烏 = 士 ／工人／2 凡 aim : 루크 口으］2 二                1 그／6             V/
                                                           + 173 I
1
i
                  /＝·6A,               弘＝1.6牛r ,           孑乙 =1.4 -j．了 , Z烏＝ 羽그'VO.j...' (R.0sc)


哲41j譚n                                                           誓 h13。
                                                                      /0-／너' = ·刀如
                                     P-4, 二亡／그：뇨／1. Ri. a4; =


                m力     C加坪｛ 瓜 已k, J乙亡仰月 丑；妃 id. 小m五凡／

                       7尤似八-4石七· 0勻 1rJ ／뇨 . 如뇨-j- / )

         13.
                /3j     근L =J' X

                       t__=   2 L-    근口     寸 I汰m 근口
                              五＋근0             j入 + 근O


                   才jZ_ rr* =甲
                             ，칡 客쁨－"j肇三尹' r"= / /
                             ，
                                                         / 万＞
                                                                                                                                                                                                                75；八．




                                                                                J
                                                                                                                       :                      {      Oo尸
                                       PM
                                                     OLL&    lf (Qd                   月亡q，
                                                                                                               兀丑                                           ,    =       .       .   '7'如




                                   pc.wt,1_                 中七7 瓜 " "a 小d 二 打列（
                                                                              ｝二*0“7                                                                                                        ' 如拓0 w

                                                                                                               = 缸7勻目；s-) = 그가0 w
                                                                                                                           .                        /   / a  \ 工
                                                                                                          느卞    =.11   /             r4 1 \        / =n1= 1卞 \
                                                                                                          니     2 (7C)) (5o-#- o)                                        =            口250 w



                                                                                                               p
                                                                                                               P4: Ld                                      1Vt
                                                                                                                                                            ""               "        ' "175-
                                                                                                                                                                                                            I
                                                                                                                                                                     "
                                                                                                          "=
                                                                                                                                                                                                     5o12
                                                                                                                               「J         0
                                                                                                                                                                                     zgol                              O.
                                                                                                                                                                                                                            O/   如

                                                                                             · 2묘）寸．0/ 0 = . 2q0 느 ／뇨4,,,4-                                                                     ,/

                                                                                                   .16 .,L.·2y = · 7<) 二 尸＋口k，냐凡 /


                                  仁그司
                                                            n = 二뜨그H쁘
                                                                I8o ._                                     喘岩釜：·27／쯔：小나Z33 /
                                              '丘＝ /0 J으그프
                                                                                                               :／喘當 :《？6Z쯔츠三




h4n <六亡咎恥發於妥發H也求i小魏忿詐共1角1m3莽客球小
                                                                   /go -j                    '0



                                              \/（功             =
                                                                      v+        [e-           阡＋                r ei                 '?       孑］
                                              vCO= -i.5A) =% = v + P/ -r] ＝多 V ' 크些스竺二 ,$.,.
                                  a;                                                                                                                                             ·9I又丁233
                                              V(충）= 5 ［甘」’P3 , 尸&移그

                                            V나＝ '     "D    2，             m7                      『5口·                        느乙；                               d                   夕－ 3551k
                                                                                                                                                                                            .                    旺陌，             ,

                                            mm " 5午／"/）『 카'76) " 3. 8                                                                                           나 計．/0 入 .1 然RY




      ／寸4斗덥球叱兜弗好n丘M
                                                                              m
                                                                                      仍




                                                                         /J Y7 tJ q
                                                                          d
                                  iv臼）1 /+ PJn比J W孑 小 i뇨 升甲-I'- 人兀
                                                                   妃
                                                        W作H
                                                g   미




                                                6   d
                                                                                                                         -       VJY1447=



                                           5/
                                                    디
                                                                                                        ＼兀小
                                           2
                                                                                                                   h 1
                                                                                                                         D
                                                                                                                         m
                                                                                                                         11t
                                                                                                                           1 O
                                                0          I       I              I                1竹          1                    >
                                                                                                                                        WA
                                                -16       니；'1




出 粱a撻4照升444哮4芷哨n4付n엮專뀜員套1主心거1
                                                                                  寸口




카
                                                                  寸2                         4,
                                                                                                              已2




                                 3./6    丁方工 A丑d C兀싸力m石三 石m/m兀m(/

                                                         ／口＜) > 근／ （夙9勺고o) ,'                      ，亡                    』 /0／吻七 亡 ＝冗뇨肛·


                                          恍沙
                                                                                  西 +7' (P口勺’24) 才

                                   M 呼




                             \
                                                          m比 加乙們펴7 伽Z mZ／枷戶9
                                                          n:           ／口O.?, -.26幼t = go乃                                        ＝수        극 =／仄＞t


                                    斗    -1介1
                                                          Jl꺼：
                                                        我， 亡 :
                                                                        too口Z = 1, 仁D 少刃t7


                                         /                             石 ==/D亡 ' ＝多               亡 = . 7 7了夕 肛＝3. 才' , 了＝.／口了a /

                                                                 근／ =／口注 = 77. .5_ 二－ /




                                                                                       石？口
(3.
           17       2b = 50J乙， 和 = / g 勺'/ 교

      F1吻，\ 才，k兄 닢，m虎玖 C仄m才，
                                                   (4比므 ，屈在4)-)
      ＜之)       SLJR = 2. 8         /

      h)        1- = .L/ 7 /꼬       /

      C-)   肛 “ ·38十25             ＝今 五 = 7 6 尸j‘三C        仍，-
      d) 孑A = .51/ 寸7'· 63         =>        Z人 " 그7 勺'끄    J乙        b／戶




      e)    _／ 竹 = . 구Q石 入              /

      f)    乂伽匈二 =       . 口y6 入        /




                                                           누如小小 毖努．
                                                                 m ;;; 2多尹．jh
                                                                    ' " y,；戶

                                            ;? /
     3.／了                   弘 = ·"-'I· 1'
       a)         .SLIJ尺 = 그09                            /

        旬               r= .3y끄끄‘                     /

             c)         '( 二 工／.5- 勺' · 77           =：수       YL = Z3 1-j '/5   7竹 5


        '0 3h =／·J그：/：·77                            ＝수
                                                               Z人 = 6 4 3 ' 37

        e)
                  ／加뇨
                                 :    .   08그a
             f) 比，"a下 =               . 33그 入




                                                 쑤            Z小，= ;?5=J 7 8 人




     匡互aa) Ht카＞
           '    , 4 /=                            ·r入                /
        b) J= -ZsA                                              /




I
；三
        C)        三＝.125 入                                           '1




       d)           .t =.9口6A                                   느／
       e)               i   = · 0그／ )                           I
:!




                                     C及k支        -／六是才支         已그＝ ／극， 立休戶j .'}
            匣列． .                                                     (a.似 A/q 쿄토 力助亡
                 a) J = · 25a                           /                                     Z在 7 P.了 加）

                 b) J= 0入 . 口1- . 瓦＼

                 C) 又二· 375入                                  /

                 d) / 二．656入 -.＄入 二 ./56入                                    I
                 e)        / = . a7/ 入              I


             (m工J仁Z左             m以        加a浚                              근斥： -J' 而白才戶Z )

            h겨
                      入 =y'J 四 ·           ／乙1町M 琨                               名ma乂 나뇨di
                  ／乙，
                    ，反 = 운／吼2
                                           首 ' 2/VA 7易dM 石M,
                      子L. = 又 __f_ . 9    =>
                      끼J
                                 (1
                                                        乙＝/OO -戶．5 皿

            乙뇨伊好 ) 7三伽                    伍 7?)-(3 . 了／),                                              \

                                                                                 1

                            ;P                  )       r느
              r= trieJ           J    1ti = ，:쁠그 : .97r
                                                                  ，




                                            _._         7_o




                                      9二兀 十2戶人‘M =/r0 ,'- 2C36o)(.2/V)
                                         = =260                         /

                  毛＝加         ／尹· '12오스프'
                                                        =             1。 /y/
                              /-.92rJ       -                         V . 6V3/       -   二 /07Z:3f "

                       = 99 二／' 96 -S乙
卜希r치nH1寸d




                                               7 <3
             {
             i
             1




                           3. 23        Z = 凸口／7了) = SL/.77JL
                            T卜-L 鈿F. 小-         c ,＋自抑乃                 S口／논XC<)/}7／三4c7; <i汁닉／ 너血

                           P石才bJ 比比mr·
                                    ．




                                        O                        I. o                7 .D




口4甘；4
    J泛旁
      出44
        1!ii{1 t겨1JJd可a4
                           3. 2L/
                                    （玩 才七 六／y 沆       나hm               光뇨 加仇났Z h            及


                                叱孑J= V『e鉀孑十 r V 'ej阡 ,. r= 忌，／至deL.
                                                           尸L十隔可
                           仄／}뇨叱
                                     v&J) = V2 = V [tiM+rea'肛3

                                      \／十二 '- ,\／乂   ..           : V.-二 r\／十
                                            [dPJ十 r& 枓］           "




                                                          只 今／
                                  ／二4仍兀                 (a石7))

                                            -
                                  %r
                                                    n上： ________/＝巧
                  ｝沅口，\ (3石y7.




                  丁 kJ小．
                             Z辰                              귿. Ii_1 ／그 e-z ‘戶｛)
                           균q + 근7
                                                    근' (/ ' 口-
                                                             e"7') + 2) (/'. rrq珏）

                                            = 르，寸쁘뜨)쁘二
                                                （乙 ' 白）十rl個．劫e겨弘




                了뇨勺
                                                謐杆彗뇨                           J                          -




                            「"" "1在云荒亐丙石．                                                    I   4d八八才 Q                 다르二프
                                                                                                                         " 屯 + 20
                恒三I j

半士石球量上＼期m埠出晏m
                                                                                                                    芒m
                          구 (k色        i\       I       //   /    \ zf.    .             .
                                                                                                                                        \
                                                                                                                                        /!/
                                                                                                                                           /
                                  "= t키4旬h7任                                                                                              \
                                      (
                                                                                                                         n i
                                                                                                                           1J           /
                                             "月노뇨
                                                                                                                                    0
                          a (2m                                                                                                 二




                                       q／士 ＋寸)：丑4辰
作
                            戶           (H- "/&) = % ．丑구危，
                Y "『娠，光뇨                            ／碌 : 工且X.                                    加
                                                                               (4L               戶 뇨 ／d
                                                                                                          乙 口   ；
                                                                                                                口
                                                                                                                     1
                                                                                                                     卜
                才凡   和他           m/                4        品姜md         7 ,'：      吼            ‘D
                                                                 ;2 了
                                       1k오 /4吼叭 凡尹土友 甲 匕伊1 。1 ／口 6-月孑
                                       ＜뇨 S5= 6. 6DX/0'7\                            (＋之 i和寸左 2．구)

                     lF奴， 的竹才i                   蛇冶1 什 尹石；/ /y（等）' ·                                                     (三／iS)
                     巳“．Z危 4八e             尸亡磁／ 辰小3-.




                       {6

                    븅亡농
                              ,




                          q
                          1
                                   /
                       /; 크   可


                                  /
                       10     I
                              o                   .0口그                      . 0o3             . ooq     .oo丁        . o06       . oo7    .0




                    3. :zc?           By   乙   ' IC W , 4抑奴 "                             -C뇨 枷／4八才 久 ／力끄七C且
                     j刀4才 m血亡，4-. I4 h/                又二 0- ,,4,a左包／ 尸局ad.




J 寸 寸 i A 下 山 4 :
                    ／卜4           0 '2仇力＼4名乞 m亡毛占了尼                           _(4_   .




                                           lOw = 工       (Vs/          2)
                                                                                         ='       Vs = 63. 그 v
                                                  -             .51D

                    ' ""'=E\ 나煮"'于＋小2. 3A -小．                                                                   <>< = . Sd5 j V＼묘＋a4凡寸
                                                      乙＝.5口口JL                                /00j- i                  入    了． 6rC{B

                                                                                                                  = .0576 커1j2/：入
                                                  口＜ = . 5-낯易今
                                                                                                               <>＜土 = . 1 3Z5

                                                                ' a乙
                 丁h工           "          "       白伊 日 口才／凡 Z瓦／
                         n二 ／口口 - 50                            a,
                                   / 口（:> 尹；     = O. 333
                                           又：)


                丁h丑 小ad                          加功7Z 가仰們
                                                          m旅 4/ i사                       小／在 』
                  m니 “V
                           乙，二, e ' J= "크，
                                          “匕『.1                       32了； ;2: .
                F4七r)-   (3.／口／) 尤1t工
                                                       尸功Y亡U 比出蜘
                                                                 t 只乞力            뇨 石口亡／ 冗뇨，
                  P「「 1\V,“치 ' 0기ri) ;
                         _.&   i_-p
                                       므．끄                       뇨. 333]
                                                         /D 口

                F,l小， (3.／叫
                                           光如 ／그m小L
                                                                  旅毛k七：d乙，名
                0工 光뇨 力; _p                                                         名Q 규y＋才
                                         , 4       ,
                Pm: 豊如口刃小“'
                                                        느 (，刃,7)2[e.2'c. 3zc)-(.3，寸
                   二二 9. 34 ＼八／ //
                                                                                    可；（，· ' )' )I
              丁샤H 두그d小八
                        ， /H才                     ak ．才云皿 나弓系
                                                   丑 ,，뇨，
                2i‘艸＋ " Pm 小 Pt' =
                                   9; 3qe6, 82 = 긋· .c
                                                       _z v
垂            斗 加亡 蜘屈
                    乙q-私丑             " 柶M乞" 石／
             竹如i瓦 므쓰 光名                                e 夙m哈月
                          d    七 5_o -j乙 ／力tm
            月丑 尸如七                            之 m4名）, 出
                                                            毛八
                          凡Z白也加乙 4
             吃，= '?. 3斗w,                出上 "和瓦k尼 " ／
                          刃／나4‘艸노 J 지                     元
                                         ，之 4七乙口，e,/ /4石
H M 七 蚤 兵
            a系e 尸伽亡L 4/                                  뇨疋石加瓦友
                              而 匈 m伍人
            丁／也 山十d／們                         的似 M石 /7
                            4m뇨枇／ 只                         了6w).
                                                              阜；才／L兄／뇨 ／
                                                                            三』
            _ &= 50／和'北 (.gqc玎2.i ?).
                   :n> 十／00                                  :32．드n2. Y
                                   (4q5寸j2. /9                            (沆M yjd
                                                   7                              玎勺" 2.!9)

                                                       구，7
區2크         口少 7L rO1,   吃＝／可（3b : 7/'1 , =vi
                                 3乙十2(>    느斗m十尸已，,
                                                            -I
           a才 녀方叱 石奴， ci     2o- so =      小. y2 9         J
                             二0/ 5乙



       口才 A凡 y仙m赤뇨， j = 2 叫S> . -.V2 '
                             V     ZO／巧乙



                                              V- =ftV ' = -3.Ob

                                              드Yr= 1. 31

      似耳                                      r노1 Y = - 513


      쯔印




  쯔吟 乂 而




                           그8
             CR月PT& 尺 4/
           匣/ ]     乂d 朶：: 來'寸 '
            m: 似／파弓 臼，34)                                           <   J
                                                                                    佃J每今 (qv6) /7 P , 卜（
                                                                                                         M                                                 /:
                                                           反)
                    " 午jP' m-e믐多                                                    二 小 ," nJ ' qE IL
                                                                                             \J
                       m唾［叱 퓨 小8끄프 1 /                                               I ?)c                 J


            뱌： 枷毗好 (9·3砂 /3 －白（, 加1力／ (Lj, y J J
                                     4                                                                                            P, M{ a1,1:
                       峽婆 坪 脊 *IP' H5 : ：山切（H)
                                         主七   r
                                              1L
                           H
                               UJ
                                               m           쯔 十 B 캣幻
                                                                                                                        /
                                                       ／
                                                                                         =
                                                   니
                                                            a入                  \     aj j


           E, : 柶／力／占 （出3旬시 甲 , 加吐규亨 （川
                                          시 勺 白斗 伽／如伋：
                    伊E, 坤？프 如J4j 쓰 =1· 幻눅EE,
                     '                    " m<                              '       ad
                                    디         立姑
                                               1 g 근트乏 十（Uq 갯主 ] /                                                                =

                                               LI aX                                     '                aj J

           Eb:   mq/t규今 （土3n 乂J 尸， 脚／午4
                                                                                                           , (q.4j6) /)               ( <／남／/   和／   知a:
                           P 으트三 + 汁‘民 小 4』k ？브L 二 J' 幻三qd EH
                           '        )3        Ud                '                     7X                            "

                                                                                             , . .. ;H} ]
                                                                                     小
                                                                                             {VA{          二＝1= 1
                                                                                                                             .1
                                                                                                                             '
                                                                                                           C尹 不느 =j




I
           吼 2    F m小M'       ( 무F () 乂批7),

                                         /12 = Bn4                                                夕莎'
                                           才                        的多
                                          qd
                                                           止札
4.
                                                                                                                        乙口
                                                                    R
                                                                    U                                               U
                                                                                                                    t
                                          q
                                          U                                                                             口H
                                                                                                      싸
                                                                        k                                      二뇨

                                                                                                  a
                                                                i;Z 9



     亡二n
                                                   ，人 (Lj. 7/)
                                               f=m丁，
                                                                                     艮： 似，7 dwP               15 lL               7乙， m，已 多끄加／.
                                                                                             _Tc



                                          F加,-- (3.tc기 比뇨 帥                                  1 上m才 瓜 石畝 尸兀 /+ I
                                                                                                    뇨J        ／才C



                                                                                                 fH (3쇄'니11沁刮' JOL?c}
                                                                                              1     누／


                                                                                            sf
                                                                                            3=<> 芦二0


                                                 = R引B.dt\V

                                                                                       b而     긋 足나L                           .              .        .,
                                                                            Y    二



                                                                                                                            （勺m누4AJt蓀 ('t.7z))
                                                                             (

                                                                                            ’求d냐                    '

                                                      FROM                 itPPG八／D仄 工 /.          a =t. 口7 乙4小 .             6 = . yj: 4M

                                                                            읖
                                         k3]
                                                                                                                        =

                                                                  C ,D           = /9：口z &-玗子                     LOU.)&$丁＝




    ]4? 114i寸世世肖好馨密章零gg侄藝藿母骨글量j字害iiri1
                                                      手：
                                                                                                                  0 rm E R=
                                                                             n
                                                                             으                                    PIoDES          =


                                                           fc그C
                                                                                 = z: ·o1 C-H孑

                                                                      - C    h . ,b r1 4 .    /
                                                                  r .
                                                                                   i5 (,-H弓 /
                                                                  丁C이 甘 三i = _) 1.




jj4!j
                                                 丁人兀a由力白It-교力Il                              比小 유，. mY凡：D H뇨 ／口O%

                                                                              戶4／ 小1似乂 在
                                                        白小卜 （ 甲出거 m少
                                                 1km- ,U．
                                                                                         ． 丁／L乙
                                                  店.0 中 26· r GH3 J ＜刃／ 口 乂m小白a及 口乞 q79乙

                                                 A乂旅，磁니 石＼／蜘m쿄i孰 ai //a小 53% .
                                                                                                                                                            =
                                               k'.이               丁＝ 乙갸/ i,' 7 S/M 7乞                             ，石寸 夙 乙                    二 . 匕）555=JL

                                                                                                              = e 751 4+l나
                                                           禾 = V百毛＝ ／三三 zlr (2上乙口乙口）
                                                                                             n 3 <7 <)

                                                                  P : /+'，毛“
                                                                                         6 D 了. 3        -44 寸／


                                                                  뀨 "    三77, : 23 'j-.-
                                                                         YEr




                                                                                                         30
                                             臼
                                                     29) 力뇨 口表乙／,4石刃；. 口石k兀
                                                                            兀＝ 口｛
                                                                                （교此兀됴 兀-                                                        .- -- _-4_
                                            kd:. +' 的 S - (e7了）' r力’7
                                                                       - 3.75 m』
                                                                               四』N/,,
                                                           ;2 (6C!. 3)                                                                /
                                                    2P                         "
                                       r7. 9nj衣旦 口攷묘如玉品 0白i, a今 ‘뇨，伉址
                                                                                                                            2反 乙4+
                                                                                                                                          /{7


                                            kC : . 3 L工
                                                      , nM (Zb7r ' m3矢나 ·cS二c［고 (.c0늬3汁 24 (,0fo7)5(6 ?c)
                                                （兀 Ur겨＼U
                                                                       ( . 0/0;'片加q3乂Eng.3兀67rk之加)
                                                     = ·O70S 斗m/2+\/h, .
                                                                                          I
                             （尨乞 戈幻 如m友 加甲q
                                                                                          d在似m兀協 枷兀各力뇨 aM
                                                                                                                                           mZ7
                              丁石／ d/ m兀，' =                                         k =k. ＋匹／ : 3 . '2. 小伊V枷
                                                                                                             －
                               4,\    匕｛B/M               ,          q= 三 82/.g. 6g6) =
                                                                                                    33, ?              dB／批 .     j

                             吼S尸
                                     ＋人 ／亡瓜上 고0m' 꾸 多如Q 7 小a才石
                                                               O.／乙 /.1.毛
                             丁「，. 四K乙 小 月乙寸 匈)勻
                                               半                                                    (J4rr祉M_ _ )) _w 玖
                             （工.%-, a／包們4力而 C刃M/Z乙q(
                                                     K ,.
                                        n   17   /   t,   nt)   月'

                                  V促 = 尸" 뇨
                                          ： 叫1 / 二 R 了石 ,3 』pHhI
                                           300




                                   '나舒D'나" 기伊，功' 小：/.3) ' 二 ///. 3 力竹小人，.
;=                           To      0仁뇨d                 ／口口 aZ3                  di；
                                                                                     如工而
                                                                                                     舛切勺卄mm7,




 U J二i5卞느1i目44]l }j4j! a!j
                                                              卜／C＞口0台 = 2O 石겨 亡二              ,-=     {
                                                                                                    ｛乂，




                                                                     /C




二
尸
                                                                          "
                                                                              5=
 r
                                                                                    可k/
                                                                j= 二姮． = .／口34. = /<)                     .   3
                                                                                                                  c，
                                                                                                                       나n    느／
                                                                     1/1. 3




 }H4뷰七心崗겹
                               S.
Li"    7-뇨 YE油                      ,,巴뇨／b쇼          /／小 (q. r7):
               //, = .1甲4A               小q끄 戶-J阡
                                    iT         그      \/




               /77『口
               /／孑" A 口나｝ eaP)
丁"    二廂， k／ 勺 恥小-                        m沾沆； 毛丑，

口-"- -4,才杯叭 a』Ja끄 '. 辰 ＝了 ·＼ 3} 냐 年“ 烏孕e’夕'，立A小끗 e5好／
                                               八??
                                          二
                八M
                                                 學 4孕可肛 和小犁 e：肛
                                           工
c＼크和 d,7aL :
                       나
                                         二J
                           d
                                                                                口1
                                                               二뇨   八H0
                                                                          A
                                                                          小俗
                     : A 二i. )<m '.              尸




h 瓜少才 4J 자Jk.u-; m/ ＝仄二 工 = 9A可jP才
（거孑亡j／二4낫 닛乂乏 兀甲 口mJ 石就;t                                                      札枇耐스比
                                                                                     6

 斗 m友， 亢／뇨， 牛 凡氾 力丑 욕"什 日 ，守甘 사乙 小沚瓦）                      "




a乙叩 Z凡 mM志石교 竿 力．三e 比甲 九石a蚣叭 G／切乂）

                    I
                       在‘ " ‘』
小m2屯 7-＝吼， // ，瑥工 4七hZ'：     m石Zi Cd加衣
a凡m/ 元已
                孔 : 4 珏半 e5朴，

         ，中 光小工才 C刃／7/M二 -.泣叭／ 兀'- C-／各 如 -4-征n升加流乞
m加尤友 戶石』n》
a뇨磁d . 丁k,4 L 脚M可／    n少才4h4.t2立 比十쿄／力切才小加阜

口叫， C乂V닉石才 J小따．




                                         , j 그
L/        7        F.,_c-w                      (9,101) ,
                            ＝亡       U入   戶니니
                                                '·訃 E }4于－Eftt
                                                     = 口)亡P ）끼2. 万 '
                                                            n
                                                            1
                                                                    YC
                                                                              lB尸 匕04' 끄互츠 Jq2呵了
                                                                                        （乙
                                                                r
                                                                士
                                                                                              j1


                                                      '嶝麥                     JE；尸 4小J拉즈 白4' 켠즈呈
                                                                                       (t   乙） 十
油 乂未4 小，U 7玘耐 丙刃九 冗祉                                                                     7似뇨Q 乂4 )

                  已卜
                   "汁斗“ ' 炙？""／麥*剖升等留느／』／2
     p。
                        '   V         了     나J




T卜叱 P二，m                                        石，+         汕－.

口 浮 如d' a』二 尺-S {Jk（步.」느往*f4他＝.）」
                                '斗｝
                                .5
                                                                         1
                                                                             ；乙札            .       y=0

              =    fs
                            1 幻K '1卄' Is' ' 多 + A)노 '）勿：汀： 1B尸
                            (                    b小 궂？                                 <t. L －平-y
                                                                                                          흩了
                                                            出It.H弘 쌀）
                  =, p                LA.)눋 뇨1
                  十 n5                      ../ L7
                                            n
                                           11 m t戶
                                                 뇨




Tk                      才他                       口表如磁b니                        t4_ )



                                = 2,求客2.
                                       1//i,c寧+ 4&
                            寸'/ =' (I菁『尉                                                                       /




                                                                         33
            9. y   F'加)-v        , 力뇨 小尸十兀云 白乂，才，d在． q
            孑亡亡品小 甲，
                            몫q 瓦也亡 / 긋d ZaM 乞mn= 0 7
            ，乂사小石工．
                            价 Y丸｝-k: : /.矢二大그       .              r9;／刃旬
            小m丑 P "D a才 的尤芹 」 加七 A刃刀C //m/                       在屯，
            蜘4 央d『 r乙；毛· TkM 小 似／7乙a 崩丑 如力／
            呼／札 尹근I놔了 m7伽；洗石 :
                       f佯D : 긋. 2乞《 /Z；毛亡 十 /Z二沇 2b 닛, 亡 二（7 .
             AJ    切肛 mm危 'F傑幻毛 他艸 m뇨 7 毛 H
            '1瓦니 光／妃 加力才· m 七四何／凡／孔吼 和m才／之
            派加師在平光／只比W碎7似乂nM旽戶m 口寸4危5
                                          궂，
                                                        R毛）
            毛（EMPTY) = 즛 =/37.             95           小／3 "
                                          /OO           小362
            表 作，나印) “岩능 " 9교'             / C 's-       小（/ 'I
                                          i/ o
暴                                                        17/
                                          / O E>          2, 3
                                         ／口S万            小2, 2了
                                         ／口도 1s-          . 0/ 7

            (# 毛） 似          Ca兀玭I比겅 円們小떠／兀 岫此 押兀；
            0入 아 尸닉乎加小伽／죠 白兀協旒D rh丑 ( (（乞I,二 小mM協，

J1J1甘J4i{
            四加X色 石 寸4d     小 出升毛 4 在切m夕h4
            口召征肛 샤／友 比 aed仁／才 抑k叭 小 X凡 UVm升q卄'如（任幻
            7-뇨 m今尹 戶伊似띠 4 I
                                炙 = 흘우 = 三比 5十y"
                  L       9   丁！也 小才 蜘乙七 4如
                                            J之 加苡         了 뇨사（ m//j 加九E及 《，
                      .
                 如叭 小 只， 和／ 耐 如小吃듀
                                                        而y. rM, h                           m小 衣
                 ／人Hl4쿳丈旦까＼

                                               !‘的自／                戶 t；디 < 叫／又              （赴 ＝七 )
                                               L 8e                             江i > 1竹／2    （毛 = 1뇨）
                                                   ‘虹m1             7易-I-
                 小4小兀 矢d 蜘｛毛 따兀 X/4 m
                                                          弘 和如나缸 뇨 札
                 苡m友／ 知乂 띠兀 好마小
                                                          伊盛n m老玄今呵
                                     르可E二毛느堤了 =／小玎
                                                                                (P如 加m呵）
                 m片， 小 小m 巳 , 戶M m/ 9/7 :
                                  e7仁，引   必쯔 j쏘｝M自欠 和 (?4（呵：
                                          女亡   a乂   \
                                                          戶 ＋




                                                                '           .

                                             t J쁩브 可妾" 戶工' V'
                                   h) Me7 d         父『따뇨 升R4,
                                      只 小勻V: : 6e‘毛ti枷

                                     毛烏毛叩： 名可毛町"
                낳姓； 乂未乏 ／比m니나
                                                甲姓M 甲m口去和
                                                                                            戶4- j
                                      琁口． 亡a，
                                            《 녈乂K72 十 근d. = O .



1 1;4斗往4筐資4J1
                ar "r         M
                                  _쿄之 m如／ 꾸a 月方뇨꾸
                                                  兀4兀
                부苾e 샤們m就孕 부 小
                                                    兀 如戎b d r吼·
                （戶 c          L巨/17 如旋 , 햐k 《：, ／仁픈攻，好m, 加7뇨A仁
                                  Lf. jo                            1A q＋缸g                       ／乙乙   ' <y ' 亡

                                                                     L3的札6+5)                     肛 亡＜y <a                        （次C = 矢U


                                   /，나，꾜，工 4d 4d 毛 (l기工 乂名4                                       a7弘 小小厄＋4 文凡
                                  出珤／口-t a/ 而 m升뇨，m따四 ,
                                                                戶 지白七｝促； m ,' -J
                                   亡l／吃 h3 k肛 ／心入 口小h 名和五구7                                                         b   "o        c-   /       0,   GA(


                                   m;，亡之 E, 시 a k}y5b) . 尸九- _-
                                                                                     <
                                                                                                                                       U
                                                                                                                                       亡
                                                                                                                                        1
                                                                                                                                        U           亡


                                                 "/ '引“ 芬‘ 咨＝ -J싹乏如乞U겅_)
                                                                                                                             ／뇨
                                                                                                                                       d




                                                                                                  <
                                                                                                                                               UU
                                                                                                                             7伉 亡
                                                                                          나之dH




                                   ＆中냥n了 師崗弓 7 h四n/ d 7 "                                                               戶乙Q,
                                                                  月 白也七｛亡 - B 白＋ 任 ( 七) ="


                                                                古小" 三，m뇨（d크j " "
                                                                                                                                       石 升七尸
布
                                  加蚣｝                    ／札      岫／                  甲     力4M7              步切无됴
                                                                 +d在小蚣(a'-日나a- 也m毛亡 =.                                                     /



    ；甘k＝茗m가m七出컵小缶心小1
                                    융4力七4_       I   '




                                             (r生쓰乞欠二y뇨芝吃了瓷晟卜b烏）
                                    뚜／/              -'4I,뇨如교요         C，』，L,t 三4

                                                              TL7x 百 二 U n끄／ H                              VX 斥 =iUJE百

                                        r뇨 和교 55 師寸a山土 a;                                                      I弓h卄 口n오 /




川칡h月目nn亞첨甘h긔dd느료＝ 二a甘尸二拉戶Ea七겹뵤玄
                                                                                                      r告 긷芍小놔
                                                                           거
                                             1 ;E.                         四     馬
                                             ?       5了 / 百了                     ；
                                             프느 H 프玉 =
                                              a孕   a /7               J'w시 H;5                        娑같努Jme E尸
                                                                                         三 /
                          7i可24&4h       ir/ .d．孑）：司e/)djP} j 月(to,／冶）石妃列eU'阡

                          TI蜘 크／a3 今 -JP , 蜘／文兀 口加們 -e升a友뇨 4ia뇨氾 名 :


                            古 努 m나 a ti-)          尸      (D
                                                                     古 헒｝ *J乍U芦 =jk)C E尸
                            日PEe - 즉三 : -J’回」H/'         ( t7
                                                                U尸H尸 H 半 "J「回 ' 今
                          力뇨毋／4 仁） /7,P / 加2斗弓 (3J {7 屯지， b{ 知Z/ '
                                        JP"댜 샤 뜸斗 劣 렇多 = J‘回 '4' E尸
                                                                숀：쯔 므브츠7
                                                                /7    a戶 -i


                          加／群占 0) 勻 P , 加i力／多 (yJ /7 幻시 , mi
                                                             M/ :
                                      卓 努 『J ' "印 如半 = ／뇨눅（左／
                                         &戶士作 籌 如 肇］
                          싸玭芍 (!）乂j 幻E, md每3 (9) /7 P, a                      M/:
                                      窄！哥JP' 싸 'P 읔努 : ，」，'.저" /4了
                                       바 士片 韋 4津］



r !a！ 뇨4m; r尸二二n戶khJ有d甘
                                     （기 Jy ．匈白 夕교每弓 (3) _4',. 戶 , M m:
                                         aE手
                                     （刀E 흉万     十 多 劣 万P ' 作 玎山仰

                                        H7) =

  a4h111Jt
                          M力， 然 ＝臭"寸5 ' ·
                          rn在七 小 ：7d毛 口；助／兀            wt土石 光缸七 弔 凸；II力·                   /
 JJ44



  1
  1
  11
   J
                                                    37


 hi4ij三4＋秒
         J
                        吼／그 1 id                  가＝I, B=. 瓜 ('iavi).                             Th.        札 名4叩4戶石乙

                                                       햐＝ 半 m,/ 丁n在尸）.5多3
                                                           印＝ 若 的小啣 計‘
                                                                             乙依p)                       eUP弓
                                                           /／尸 = J4/ f켜 qmm/
                                                                  成于 /)

                                                                                     戶qm/ 亢qJ) eD'阡
                                                            H/    =    r
                                                                           "-   C
                                                                                 '


                         른X4y· 3 = 印／J; 尸E戶／// .
                        뇨
                        T
                              和如 끈可 dm小 光뇨 尹切re                                                                41 > 口／

                                     &           工Jr

                        品＝ 玎 S [｛等4뇨／丁：'佚刀
                                         『辯r耐갸3s,L(4cf)] d仲
                                   尸＝<) 伊＝O                                                   \
                                                       &                                 t,


                          ; 資孚 $ ［品k抑)i-看；; C佯寸끄rct
                               .             -




                                                                                                                （日戶놔, .                           //
                                                 尸＝0                                                                       （入上 ; 十叱 rX
                                                                                                                J11       J1        ＝느       Jn




     14
      1iH
                         ;g芝LOLr的『子亡「）」7小＝戈二，兀,.                                                    /

                                                                 5EE            (c.14)

                        1뇨 加V 4才 序 X凡 小娩友y M/ / 石 ,
                        P2埠,!, 如，伊小如｝=                                                            學          k

14Jq나甘口nM니1r111n11V1니
                                                                                                        心万
                                         1         ＝戶 11




                                                                                                             亡                           27r

                                    a V 甲＝{)
                                                                                                                      U.,/／놔느／和
                                                                                                                               (=   +    느




                          ' a尺瑛 ' " r 丁："r且D
                                      추
                        丁F皿 口表ikM4光而                                  小i X丸休．

                          k                                aq毗 ' 万 "4),
                           C                                                                      ‘工忌勻E4/             /
                                                                                                                  너之 j: s
                                                                                                                               -小




                                                           1丸“P幻E 'I＋二＝                       '   P孑．= " " 而百 ‘「甲／似

                                                                                     .3 8
                                  나g j3          F／四M 戶守m乙 幻3, 力뇨 戶늡才 7婉勺 加D(E
                                                                               石
                                 P加尸七甲j노 m工 YE,,』 1-rn이 . 丁E2i .a교 丁Eq （了P1,/ 凡｝-G, 4刃．,.4 丹 口力 rEO,
                                                                                                    ).
                                 '2危小3 （나d27) a. .규 (Li．싸口）:


                                 TEn:                                  : 뜨끄쓰) : m, 7了r 刀／/／孑
                                                                           z7r(. c0t)
                                                                                                             /


                                                      유 二 르스 . 乙4/玎 (3回 : /y, 3了V 力I片
                                                          z   7r（兀
                                                                                      矛                      /
                                                                         271 乙口口 r7

                                 丁-zI :               凡 =    十l; c , 知鉀 (3回               : 15, 2.27 月1/／子   /
                                                               Z기4a.     ZTj   (. nOg)


                                 yE이 ;               孔？ 嗚； C           , 了．g32 (34 ) -       그교， 87/ mi／孑        느／/
                                                             그'1 ＜乂-      zn- (· ooP)


                                 (/JY                了F山 ／寸乙亡쿄 4               Jd,n4，』，悉 ' 光仙 I石 加亡a뇨 Cd끄，
                                 戶X札 白-G孔， 사和／ 乂 ' 孑 辰4-缸Y쿠
                                                            心：

    니J11J寸내11]41111
                                                      白 （/,/h (A 的 규 出的眺口d女p)
1




                                                                              切人能尸）]
                                 丁b毓 力侄 加小甘                               的石妨 光札才 e孑
                                                                                   『. 寸戶4 口．4d/




       寸三흩귿瑟葬叱茸빠崙崩案d珪m當蟹資
                                 d尸＝b, 幷G二 兀                              沙倂a泣 :
                                                                c JM m亡 <t) -+- 兄K
                                                                                  立이 =O
                                                                C- 丁1（士G 6J 十少 兀，（毛功 :D


                                                           （耗仄 ) 兀 佯C이 = 了'I （毛시 兀 （毛 a.)
                                 F0乙 乂仙 7/d口／ 小四Q ,                            거＝0.        及十 2= 壬匕口 ‘       7-뇨
                                 :l/                 ＜乂／
                                                            加（ 뇨‘尸之 才九才 矢6= 그x, 斗2i /d寸 :t;/，
                                                                                             꼬 a.石U2／之
                                             ＝
                                        i7
                                                 긋
                            寸｛
                            ，毛多乙：力；乞4 D和．辰 ／比mmZ在＼ 民乙/
                                                           r（乂） = Jb今） y교그x) -J             (그入乃8今） = 匕）


                                                                                 Q니   口
                                                                                      ／
                7乙w/ 加七 禾M町付 乂石m才 追. '4兀1/ ／已 舛e旒乙 才石4，人

                +. 7分 仄 吐k烏／小四仰Q 戶「mM 匕 7/C乙
                如仙小 屯, 1: ＋石協 :                2 ' 加57今久 多      깟二／,2· ，十加之 m如

                也和 -凡 似MA d                        町/ 2. -z小y 氏 m在 y B加／
                /m烏｛ 戶4 兄征 7勿三乙四 小／在                                                         ＜久i




                      ；乂
                               孔 今）         >b00     :rD（그X )      YO (ax)           I (x)

                     1. 7      . G7/   . 22 g       , C 口3        . 5./C)          . 3q.2
                     1. 5  .5/ 2.       . 3 '2      小. 2'4 0      ' 377            . 그72
                     2,0   , 12L/       \5;1O       -, 317       H. 口．7             . /9了
                     3. 0 寸. 26 口       .   3? ?    . 151        中． 2 fg            . 口／8)
                     3 / -. ala
                           .           . 3 吼3        1 2- 0L     小, 2.U            . .oo3
                     3. 2 -. 320        t30 7        t ZY3       戶. 2o 口            小. O1/


                而光凡 伽才肛 衣友m,                        心了，(aM 夕3. 2- , (,ljt c- 小 私／
                仄 M《』
                    ：,,, 如m兀 兀口교毛三1 쨔h-.甲 仄 石m

                衣／而缸小 充凡4比 刃乙石Z+ :

                                               ／的 = . 003/ 刀“3士，二／/) m引）
三                                                                3. / -3 , Z.


                                                    ：느 . 't3? 十 ./9X        := 0

                                                    今       깃 = ' 쁘乙 = 3 .／그 ＝긋, R            /




1J
 ] aHHn甘川 1
          Hh
           h기




                                                    二   /
                                                        U
                      1나．l5l        F기乂M\ (HJ8q),

                                    즌X4 ' ·3 : . 타Hlix                        =
                                                                                      f11   "   客        "" 烏 '               長    '


                                                                                                                                                            d 三 X 自 ＜>
                                                                                  ,         "   쌉’        "   ．   小2足d甘                    "    '   "   "

                       T卜t e伽如 平付M                                       J
                                    的            1

                       fc,＝玎 JE廂' 弘小

                                                                                  『 ""t:""낳毛／
                                        0            0




                                                                                            ／可' ""'m
                               X=           j:
                                                                   o4                                                                          m

                                    四시甲뜨 /4i休" 缸小
                                        2 友C드                U
                                                         )
                                                                                                                                       xrd
                                                             =0
                                                                                  드華引）너 + 竺므／e「 ' " r"力）)m
                                                                                                                                                                   II
                           : 쓰뽀쁘亡 r구小 ／츠
                                                 又                Lt; L l                   Y大C      / lb                         ｝구           \ 小二Ii       / 'a

                          ' 으些y"'" ［缸冬쓱批小，뇨］
                       -t工e f냐小七 ／乙4+ ／沅／                                                            .                    ,

                          ： 町，向'凡母／
                         P』          ' IC'二寸山,' 寸］a
                                  y=0 丁0
                                                   , d,
                                                 寸 V /


                        古
{                              力뇨                    d:Z在；Wm月4d;

                          （乂C =
                                                                             .2 足5

                                                                  「“丑' 戶［古任－芎批『 뜬制
                                    二                                   尺S                                                             /


    나 斗 量 4 4 겅겹겹n/
                                            士aIo ［告，毛去L 耳弘］
                                      mh叫           尤衣丑 而Alf瓦 小 小念 76 ／余 m
                                      AJ4和皿 4Um叱七 平 a, L石d名id ＋在石 」‘
                                         次：, ／介 毛느少
                                                                                                戶 .5戶a:'
                                         r = P ' 尸沇？                                            /5乞 紵a

                                                                     !
                       1}＼小＼/                                . r A d,;M 毛 旱                            7易乙 .三c;f/
                                                         y
                                                                         5 f "/
                                                    '
                                                             "                                              少d
                                              '尸
                                                                                                       戶
                                                                 "




                  Iki{ 和小 甲 臼 4 肛兀力a 名                                                                        e孑『O 寸ar   )
                  m{ 石AM 呼M仄I而努
                                                                                                     戶尸0, 匕'z J.
                  m毛 小，C 才＜4,/ /／入 ny＆꿔戶力 ‘· F如小 (17Iz 뇨）,
                                                             訊
                                                             m=
                                                              q
                                                              4 UJ
                                                                                      1을드겨白＋丸多             7乙七 吐j/ /
                                                                ;
                                                             寸




                                                                                       4口JE0
                                                                                      LI        86hb       在 片／
                                                                         \
                                                                                            h
             d才7=a:
                                 E3 帥兀汕似 方                               -4／如 毛乂 : B 三 方4
                                 /Jx 白杉力뇨44 ＝中
                                                                         全 m七c :+ d方d
-
             O1
付
                                              ,             L
m
                        /
                                                                     _
                                              h 乙少a寸 m七＜才 7 衣C ／나4凡 1<( (>\
                                                        i,
                                                   m 毛 瓦喪d! /
                                          r h1『佐；m力乏' / /
                  口m
                            </
                                  /



     卜加Hn$
                                          1
                                                                                                 J


             Tk                       而寸 沙蜘烏뇨 md及 MM三戶可 < 蜘｛辰，



    U
    甘王＼L
       t
       ；亨r




                                                                                        =
                                                                                  /
                                                                             乙／
                                                                                       :\
                                          k '7        TM小 小山． H3:. , E孑仍戶孑) :e了（乃／)e:Jr7
                                          依 T鈿 小노 m                                  小 什ad                        4 弘4 五k 瓜兀如上
                                           呼乂7丑 小加此各 7 /m工 小南나 d f: b)
                                                         聳寸和十和幻的升.
                                           甲'中「" 戶                  -1-i -:-O        m加乙.1' 勿                E쿠 ＝斗＝口

                                           TM47                                 (4T (1. n) + Tj乂 (-Li 尸 )                 7乳 a5肛 h
                                                       e弓（/                      "    "   mr         '                '
                                                                                Lc 그a뇨e) -FY (뇨戶
                                                                                                         "    '   M
                                                              ）刺니
                                                                                                                          7余
                                                                                                                               b   今尸三
                                                                                                                                          C-

                                          가나的，          目乙 二 E.냐．,‘ 냐／二 毛느毛

                                          了h工 뇨岫겅 蜘乙瓦流 m:
                                                      e룽 " 0 4才 尸二（兀 ma尸C .




1 d坂恁낙口니出m1汲1臂ai4411JJ11111
                                                      e} 口m乂 ///                     口八戶 匕小j二뇨如m d尸h
                                          F加M 臼lw幻)                             . . . ---J回e a E工
                                                                                t寸中 H 二玎H 휵丁 /
                                          古      ／七之 多tX／낙7乙-16的776吻／們고뇨口

                                                  .       14 孔C勻刃十 B Y (；缸D= 0
    mi曳JJd                                                C 丁記枉C) 十 DY比kc) =O
                                                  A 孔伐批） 十B％ 佯a6) = C了K丸七）＋끄％（뇨 刃




       :r必發奪盈傳拉斗趨崩喀枷每鉀瑟器 實獒注甘翕笛a姓留亡煎萍年鈿
                                                 C-由 [A了恐拘 , 眺' 魄 切 磎＋ 了訌短小가'（乞b)]
                                                 I-

                                          垠《 md 缸 C4W 衣 J們小（ 辰 乞M
                                                                    甲乞a ．戶 :a加
                                          나比 /h>M 月加才七／ 노 凡也仙뇨d 町 닛凡 M뇨疋 片yd乏乙小 弔
                                          .午刃南：
                                              ＞二 乙勿的뇨 , 丁幻뇨 」k m 7品七 心
                                                                       />［毛 小                                                            和／
                                          乙， )jj比d 口（辰-d/ m刃石蜘 石七 &/., C3 勿d日，
                                                                                               LI/
    色 I8 I       1o ，仰工              (y,/g7) 加之 m咐比 后已小初功기化3 >12口
         (
    口m,<>
                  X' V층二, -.'fyi: ' 'qs
    T ki , IA/,'6 =. gS -24               =. V 3(
                    小／ 二 · 긱 ＞全 (. b始 (4. ) = . 口, 75 匕，..       /

絮
                  入j ' R드
                       ，F :                      = 5=. D6      C44人   /
                                       금記；5
                 1-石耐 毛              W/d ＜그：
      Fnd7),{     { ' /. 2口e力
                                                    + 으브 (13 十. (I／
                                                                  匕） = 乙2/        /
                                                      Ek 十 /              r

     "m
             '
                            ,
                            e
                  빠4=
                                24
                        恥1= ·? 乙 /5ff白D 二 끄三뜨

     F如H (q，切？) 才뇨 力竹友乏 肛r缸莩 -CI.)
                  q' 具끄『 已而刃；" /Z5亡 /
                 大口 =       CHm뇨          300         -      5T. 656cH        /
                  .4 YZ; f             - 而万伽口D)




H


心                                              竹／
U


甘


1
                                                     C
                                                             104'. 7 ,m亡J
                                                                               ; 凡 V票卞꺄：也斗明且
                                M1CR0STRlP c- .SE:

                                    FI          土3 바／＞그 :                F加M乙功가이， 8＝煮告= P.o
                                Wa= 쿠［6-1，且仁b-I)十흩二．(｛且臼－I-)十·37. 夕月 3.口7 ＞그                                            r/




                                 w = 3.01乙／石mj " 르쁘4H
                         F,,,.,,N (/ .'zoy),
                                                         (C : 윽1-f『윽二'                ：二 /.g 7台 入q 二亡＝ 二 7 3r r．戶
                                                                                                           二
                                                                                                                   三回
                                                                                                       사
                                                                                                   J
                                             1o7),
                                                     k十 毛으色기
                          F八小
                                      (Lj.
                                                           ．旒J : .D6/ /Pt，尸：y4n                                     /
                                                             ：나6e 忙沙／/

                         E4- h\ c出 Zo5')
                                                     小
                         和까（ 川．S ATTENu,4-1?0小回IL.,07攻警加加Lj3峰
                                                             余       :   므7?
                                                                                小／ M      /
                                                              X8客斗 3汕／
                        '5TR?LIp.JE           CASE:

                                  l-t4' - C'1sIS'기 匹乙＝ 辰（刻
                                                                                ：74'< i加 · 2＝駑. 11(1I＝·833
                           M//b ＝乂，二 · g33 ＝汐
                                              \V = . 83丸3Z뇨）二 . 267 C,., /

                                 入r韋c ' 쓰쁘쯔勺                                   和／＋聲*＋咎丑付' 9: 弘73




JJ1尸J斗年土案倖山恥nJ444 1
                       已七小M 臼II이I
                                                     啞 : 2.7XI了3R




                  41
                                                            3C）兀6
                                                                  sEr& A =         ·081/ 小yb二，


                       F＞力H 臼.30)/
                                                     ＜乂 = 美t瓦S 二 尸
                                                                 "伽吼？(.o ' )
                                                                그中
                                                                                          - 므7르之伊'l'거 /

                       TOT尸二 5工. AT丁E,*JU月刀刎叱加m可娑可回叱0抛'1
                                                                                              5尹，)(礬判qIdt3/
                                                                                               J               1

                       .' .       S나（OLD USE         1- +E    MLCf山S丁RiP 匕1-JE .      /
111그
         ／   ]     N吾（x, 9   ,   )=
                                      k} (x1y)      ebP吾
                                                                     )   h 肛d , P 力고心／.
       匕-t石）叭 (9dq) J


             바 = 努吾？ 可」‘阡                                           "」살午小｝
           "'“營午-J冊                                                E3 " 峀努d好
       '" " " 侮呼H珥 . E畔 5 4-EjH事 슛

                 “쁩［翎" '／娑）1訃劣（斗；『斗A
닙了 // b 小 加乂 ( 昨 4 m/ 戶m尤H 辰小 山
       幻，寸石仍 的比川 , X系h(                                        屈 小i . 押느蜘J-_ 0
  乂右， 七功뇨m.;.                          .
i/. 그 그
                 w小立 小뇨七毛巧L色元7, 匈／方m小在／石.
/m乙乙 M74Z乙如；
                '孑
 E了 = E0 /4쯩 可I                                                 E구 E.r4如뜯츠 e和孑
       成 " ：돐 JA좟 可J阪｝                                          町 “哥m恥小孑

        타
        J峠
          : 已T 小.4'좔 C규旴                                         《肛나古｛刃a)' , 2丘：女' 꺄冶＝
                                                               竹不毛

         『 哥 M警 日F" 孑                                               弘＋旒'- 7cj " 7 m ';＜叫뇨／{：넛

거兀d奴小 卄乙n d }=. 石 4也＜ :                                                  i +r = T
                                                                     寸，帥r）날；
娩白俑9                                       그느
                                                           小



                  戶口似） r: 毛
                                                J
                                                           丘
                                                1
                                                           =
                                                                 -4-心km和.   Li乂24工
                                                                                 （4/
                                                仄
                                            ＜+ 근丘

二友伽恥似如h／교 力뇨W 小d十立 白E 肛恥可 畔，                                                             a뇨rb\



                                                    六
                                            k Z3
                                                   2丁M = 恥／}. = TI山幻i;
                                                   0< X < <Y 7       孟 ; 小＋X乙／乞
                                                                                            [    .   근4   1]
                                                                                            1
                                                                                            O
                                                                                                 t
                                                                                                d.
                                                                                                                    心
                                                        < < < ＜乂／
                                                                     毛｛ : 小 呱d/／弓毛
                                                                                                          a.
                                                   <t
                                                        P “江仁舶亡7by
                                                                                  _ = //b'，有늪＜呵幻'
                                        口什斗나了 (Li· 그그qy
                                                              及瓦 和d + 근X 立M 只：( (a- ) =o
                                            1卜叱 小．乂友 ,l-cv才쿠 肛； 步岫乞｛
                                                                                        여伊4뇨 名 札 -pt1M

                                        i
                                                   끄＝喪朴小／毛 = -d' h }?.／毛


                                                                                                1t卜
                                                                                                  I已
                                                   匈 : 뇩a41k = 平Jd 恥／毛
                                                                                                     " '따      ""   ""
                                        P니자『屯'－소弘 나毛【－士y二
                                        口件뇽白 臼· 그그LI) :
                                                                    和 b금／ 鼠，싸dd =.
                                                                h = 次尸 乞＋尸 = 0
                                        T뇨1 97仰 加洸A ／凡／쿄교뇨 石                                 肪m比M 7／石，
                                        小洸A 七. ' 꿔a: 7/


                                    4
                                L
                            竹
                        H
                    n
                骨
            哲
        1
    d
미
                                                                         =
                                                                             -7
      F;-l_ x中石4d        Q／乂乂bQ                       匕t 二 2' 2g6            c-'八
                         口


    矢 : Z入｝ 12;              끄U 뜨으끄三뜨 二 2了7 小
            ＜二                            3口0




     P: 汪니和J' = 그52 =,

牛m／쿠石7石才                 存m 二 능 名g 근쯔쓰 " 和戶k /
P小加兄 侃乙rt        二汗                   응스： Zi(7.5刃.9) : 乙了7入／
                                                           ）오卜／뇨（                                              /
                                          므
                                          P
                                                                   2 51


f乙功뇨 （出그q7) /


加Y M弓 叫 古寸在｛業J' i如-H-'
                 二           '-   ,   =
                                              zcz                  0오X/.8)                    ;,,b g m卜4//         /
                     次仄Z                                                                                 JJC
                                                                                :
                     J
                                                                                    /．   了3
                                                            (2.
                                                                  2g7


                         「巧 < 듬 < 耳




                                                      小 느

                                              口 나 1
                          CI／月尸在犬 了
                          二/
                               1（丁뇨（ 円｛心M 肛 斗mZ多 乂乂丑 mm                                               口-4-   尸. L/. 2L)

                         났／亡匕-5孝少」m／沅；枷44W比I
                                                                                         訂b1 哥
                                                }
                          c. : 巳／在 홋 S口孑                                        r5 r
                                                                                   X                 납 a
                                                                                                             뇨
                                                =




                                                                                 E 나
                          H4 " 폴으 在，皿 e규너       }                                                八   警 警     侮


                               旴
                                   亡口．          ＜二나




                                                              e包3
                               = 日1入4끗                                       汕如皿 和匹雨' , 乙' 響
                          Ift1X " 똴T 戶니 卒 e5叔 孑                                 由N百玎石派了" , 計M洶
                                   근乂           口h=
                         枷太石 子고抗 d了：o: 1fr : -r

                                                                 玄C-14r) = 古r.
                                    = 극丈H24
                                                                                                 尸＝ . . 石z,,. .'-
                               r
                         口l7
                                         극丈 + 근口－
                                                              ' TkL- )口＋n 투＋MH匕 互2,                                       \




                        仁．기                               久 土小山如如日 /n                     蜘石'7 和뇨，
                                                      I



                        너샤4，
                           山t立．             ,             .
                                                                                r   (7
                                   已 “ 虹끄' ／目 』 Z:＝毛끄平2.

                        니
                        //m
                            !12 I= /&)' 小쿄4 斗四 小 呼
                            M伊 甲 比征 7나Q 小戶． 1j4乙，47 1尸 二0.
                        Tk4 뇨 小나 伽十 h此’ M 탁，兀此／品hm
                        '戶 bf" 납' b· 幷初m 四｛뇨 ：듸‘， M;m4 如m二，
                        小凡니" aq 4 M4
                                                                             加斗小沅仍．




        ) t未타4吐心小烹立m滋
3套好m十4; 4
                                                                        '?
                                                                    4
                                 .5m. :3


                                                      , ,\ , 2. .-,      \             ,4 小   i:
                                              0 b 工                                            :t
                                              I0 == ZL工 1 Km           =＝夕             J1; 戶 m丁＝:===
                                              느人                                                      r r工i 1


                                             叭／寸 首LI工12.                   -=方         L_ =            그 V\/n.4
                                                                                                       늘1ln
                                             We：寸C1Vd' = 功丹1工2.                                                              m


                                                                                                         乙j느C
                                                                                                          4H
                                                                                            >)
                                 丁hj中 ／뇨누LU才 H뇨744d/4m亡尸                   _44_




                                           2在》R*j佃나詭）= Pe十극J幻佃似．We)                                                                /
                                                                                       士 江／'
                                 Th反 口尹丑k                  -wt／及 X丸 .,114고／                       ,K反 (5; /7上

                                 反Y
                                                            C         L: j'及뇨＝J'佃L너기

                                                                를쭝＝:*口/三                          =            町m．
                                                                                                                             i工尸
                                                                                                                                 十w)
                                                                                                                                       /

                                 出小小兀 光te 八戶4Z在 甲 尸瓦＞ 加口4 小如（. T뇨i                                                                         口夕4Ze9/
                                 ／砧敬 佰．且'1).
     m시
                                  5;5戶

                                                                       근 = 工 J.                  /_!      J              · ,, I,




!ji가 土
     r＼忍 哺 j 實 重 1 斗 立 i } 4
                                                                                  n    ]    111          _7__            0 -나 니尸
                                                                                           JU)L_                     )
                                                                                  /<




                           14
                            i1
                                                            幻
                                                                      :'                          = 尹如） ／·
                                                   小
                                                       ／
                                                                                                                                                     1
                                                   亡
                                                       뇨
                                                                p- J叱＝뇨）




                                                                           5C)
   三64          em : 士 [vi亡［，二y : 七
                                八J
                                              [vr Li'］사v]*
                                         戶／

                          : 士 乏 乏 V뇨 Y；戈 'IV,
                              4 =1   i. ,zj



  井 蜘고m+/匙iPn!『O, dm오．光
                          凡 Vd a꾜， 小I四
  加之 和才石才 a1Q                                小ii
              V4 =- , 꾸＜伊＋在V
     J/
                          'I
                              .-' . 丁뇨-I-c-I
                P在 二 노VMY未， V才
                               二 -L                  , / ' 兄，之
            '       忍 돌）I乙｝ " kQ[Y，小
                              ｝ =0 ,      /
 3h 乂d 口U
                     肛才小墟少匕 力
                                   ey付比伽寸 戶
 '1'，叭 口斗낳i 1/M . ik八．
            P - - 2-   之 以 rt 亡7툐
                                       \／才
 닐乙           忍加M乂之 兀芦 卜吃 '1'未，V
                                  . j: o
 Jf y似叭： y뇨M ( ai乂；尸的Z) 7 ／石k
              急i亡小 似 난 十V; 喀
                               小町比 m喀H瓜
 小；   疋오 A十A눗 (4- A加                              咐）' j尸.
                       ／ ) 小 -啣y 뇨七e
                                            匙｛yH'｝크＞. /
    id ［리＝俚 r,] 小m伊才凡才 &;i (.o._.4
和M 'mhX札
         牙   m 叱 구d 小
                     11
                                -.




                           小町3 c--陟兀／
                                                                     1J              七
 m : 珏寸[?:1뇨3* 姑                            놔닉씸
                （긔毛工，' *工．五．r? *工：毛口
                                     工尹十工：근：:r才）
   ＝缸    西 ！工12. + 근：工1
                             끄1 ' 十 근刀. 工工？
                                            ＋귿LZ工口         ？)
乙 派 小4-屍已
                      小      mW너낫 蜘m, 心
                                                     4} : 忌加놔 :.
仄石m      忌 2근刀1'，工芒 ＋근，
                      ：                工：工，好 =t> .
丁뇨口 a畝e
            呻뇨 구                 西乙：모-2/-,      /      丑 危和小巧
瓦乙 a仰叫在                                                      二. )
        -  Y 근／又 mg乞 －刃小 근
                2
                           그／                                             a   /J 6
m4 ｛幻 di 如十四
                                                           =
                                                                                '
                                                                 -
             Y.小虎d工 m
                       蜘小q                                 小뇨 /Vo.

                                     了／
                                                                   ；可"可"
                                                             1
                                                             万m. 石；1   1
                                                                            4

                                                                           V1


                                                                                                                                                                /
                                                                                         '!！吼，=b VI南．哥
                                                                           (5. 35-),
                                                                                                                                    ZA (?A -t 2:日 二 2, 2-                        ( 5y
                                                                                                                                    ) 7 A + 2P
                                                                                                                                                                                 S1nuI' r*   ',
                                                                                                                                                                                                  )

                                                                                                                                                        /
                                                                                        근at 小］          : T1           希勍 : 나亘尸－ = 근12.                                   C W/
                                                                                                                                    又 근A+ 균8                             gEct枉DcI-rY)
                                                                                              그； ] 乙크）            It

                                                                 F,t '-    ( -,36) ,                                                         /
                                                                                                                               근耐르으 ! ,/                            (& Y
                                                                                   'I,, = 工니         , 小                      근-A 근E5
                                                                                                                                         寸            liZ
                                                                                                                                                                         .YfwmE丁足YJ
                                                                                       ' "   \/1 h/L긔＞ 工 :


                                                                                                                                   I
                                                                                   V.,' , 프니             = -VI／匈              ')/2B "yf '                                (- By
                                                                                                                                -
                                                                                       '''    V1 1y=o        V1                                                          Rci尸尸叱 (TY)


                                                                 cHa- ·.        LZjLl'] : [o] '?

                                                                   ztl '1 十ZmY긱 = (2.k十근B) 2                   르느H十＝ .22汁균6十근2
                                                                                                                             5.
                                                                                              근b (k근月十근8)      而仁근A4)                  面但근a＋是助

                                                                                                     + 근A(2A＋근B) : O                                        /
                                                                   anY12. +-a나Yt2－二 H근A住尉2B)
           n
         11i
                                                                                             疏仁긱十근B) ' 근B仁리＋근5)


                                                                 小m石弓 戶比知 丁“ 八枷＋ · T뇨小尾 妃／




4 d H 客 恥 任 4 幷 斗 發 1 卍 心 讓 瑟 崗 m 繫 3 d 莩 多 4 a 密 嶺 淑 望 ＄혀
                                                                          帥＝근之1＝ 그立끄h1 /
                                                                                                                                                                    'I
                                                                                                                              【 “근 ' : =
                                                                                  V,e Y.
                                                                                                                                                 궁古
                                                                                                                         귿！
                                                                                 二 YA (加 +'/&) /                              '/ L= 'y , : 二쏘尸H /
                                                                                       ;2 \／月 十Yb                                            ;2y月 +y乃．
       刃l才赤i 三뇨 力4t 4F口，才                                                口．4-              4／닉14J7t :

                         근II -三1L    근zz- at




           칸I) ' 西－Z.1, " g，“
                           ，乙 J'：已，.Z在冶：:
          Z
                   st
                   (2)
                            二 Zll - 抗／匐
               Z (I)
                。c_- 2ii                /


         就C.
                            = 2zz       /


F八小W 才뇨 1丘；d                        J7抑兀自 )
        Z在 = 戶 住(I) - 근．D22그－
                     칸；
           二 (2 (1)-   ))2엾J

                   Fh小              (5; 6키）
                                                   v-.t = V才 +V1
                                                 Z.
                                                  2。   工m,
                                                             l.
                                                              .   --   \ Aft   -m   II   .;m




石缸뉵 品，,- I/ i , II
  J /         '                                \/: 二 (v+ 2工D/2
                                               v; =(v뇨中 名，工D／又

               '           V：十二 吉（/D 尹5o(.／껀쓰）)=7. ／끄쓰．                                                  1//




                          V; = 古（'/0戶万D(./d쓰）) = 3 . V万L：프了                                             t/
                                                                                                             /




                            \／才 : 打／2Z쯔二 十5匕＞乙乃깐：브力 二 夙／左소
                            V{ :    古（/ 2.左00 中50 (.／了Z／므쓰）) 二 了. 9Z그‘




                                                万：3
                          근口 巨）                           죠                   （勾죠


       小f나才 口ma 加本』 才 和兀 m工 加d左／뇨I, 戶 s/I =S.;L工 功
         S12－二S그／ 二！三   ,eU肛 4万；      \o e규勺                                                                                           S
                                                                                                                                       r
                                                                                                                                       L           二


                                                                                                                                                       !a中' . 尸
                                                          匕1-
                                                                                                                                               H
                                                                                                                                           J
      (Tk4. C加Jt 小中7 a仄Z仄 尤뇨 小局K 弔 老뇨
      六bc1 尸M小쿄乙4 戶0- 名뇨山岫加i 力뇨 -4初亡諦‘ 石



      5d2                                     4小mV<. ＜兀似尹力：亡‘m+ 口＋ -4-4노押f)1 :
                                                                                            尸
                                                                                            1寸寸/ V2
                                                                                                 1/i4
            VJ                                                          J1卜
                   H口）


                   4中                         [s4j                      4=ma              十小         y   +
                                                                                                                 .



             Vt-
      1KM1

                          r    vt-      ]j;
                                                  ['          "   ]［쒸
                                                                                        [：寸［5']!3d
                                                                                                .vd [VI;1:[S出；]
                                                                        玖)卜JM1/尹0        .i,(
                                                          .                                          뇨，
                                                                                                      ，之                                & = Si8/4
                    1i-
                    디
                          II
                               V1+     :o
                                                                                                                                        v =52 /

                                 A = 始 만 + 5夷 13= 始 나 十 瑥 'S，戶 月

                                 Vi                           S二 VI1 + S스 S，尹巽卜GN肌 꾸L0                                                                      -4JWH cot!시：
                                                                                                                                           나카
                                                  =
                                                                                                                                                                                                >
                                                                                        彦＞工7 '           > !
                                                                                                                     上
                                                                                                                     V1
                                                                                                                      11
                                                                                                                       1
                                                                                                                                       匹
                                                                                                                                       >1十             ,                   >
                                                                                                                                                                                   1！ 小tJ
                                                                                                                                                                                   i        7
                                 szt
                                                                                                                                                                   尸； 1L
                                                                                            口匕
                                                                                                                                                                               乞
                                                                                                 +
                                                                                                 1

                                                                                                                                                                                            <
                                 yi
                                                                                                                                                                           d
剪                                             (
                                                      “
                                                              字
                                                                               9)
                                                                                    =

                                                                                                                                                           ( b 亡A
                                                                                                                                                           . II D 2i.
                                                                  S戶. S夕
쐬 r
                                "工" ／亐i. 三8                                                                  )
                                                                                                                                   ＞
                                                                                                                               訊
                                                                                                                           山
                                                                                                                                                              ！三


                                                                                                                       5：尸 畏缸．
                                                             SH
                                                             Sl/
                    무a                  艸白e 自J ／仙石片
                                                           ＞ Ls] .L 』
                                                                                                                        겁
                                         1 51tn 十Is미 " = /
                                夕   '             Is미乙
                                                                             t니5l2           /
                   5 , 尸／      仄 如力凡규 , 肛（和才td/
                                                                                             ,   3－局d 4也存m玉， 和＋
                   h ［玎 小盛／ 平 X／』［
                                                                                  戶m小弓 I卜 "
                                    0            .5/ 2-            513
                       [s]
                                    5/ t                 0         5z >
                                    31)          S Z3              O
                                                                            =7
                   무 X表上                   ,,yl上扁刃2j乙                H乂：d, 石44丘‘，. J七伍， C幻
                                                                                                                       小呼才／之
             小旅＞
                                    :

                                1 듸나 '          + ! 5t多｛ l          二   {
                                                                                                    St3 S2층 二（7
                                Is1 十 f15L히L = r
                                                                                                        stz_ S古 二0
                                l C ( 12. 十 }S工키L 二 1
                                                                                                    Sti
                                                                                                           .)2j
                                                                                                                  =0
             To 戶［＼七：LA／寸 乂衣4丈 ＜兀 乙口
                                     吼Xidd及危亡亡닉                                                   띠小뇨名， ) q44/／似i尸
            Jt;/t』
                 口／            512' 二（/ 」瓜 四／h                                   名
                                                                                     戶d力勺y Cs) o- f (6) · 丁卜JH 7三勿吼
            (1) )            ＼뇨3'느 !
                                            7    凡d ＋和                            (3) , 152키＝ 0 . 3-' ‘才 ，乂／tJM
                                                                                                                        .   ( z)
            小苡i 乂（ 白dk成力／·
                                                                                 小；
                                                                                  小烏多， 仄 的烏成屍自
                                                                                               小元                              Z/
            /bZ瓦샤 小 兀／ S{ 3 =(> )
d 4HJ黨H\y
H
                                                                                     '-1--   S之-3 ＝口．

             (l 口回屈石t ／뇨
                         a싸 ／仰놔／  e C工 &
            /｛亡4比小』
                  ） 加力九凡／ 于尸C：才，
                               M上苡硫比 ,




J솨n出虹喀十斟
                     三／f                             Fo七 力뇨i 尸a뇨＼，計 /+ ／力-4乂小／ 只툐 戶4皿 ／乂J

                     a- 싸仍在名4 /b七 CL 小뇨石 小和고                                                                      카尸寸 "

                                                                                                             느
                                                                                                                          工i
                                              山n吃
                      戶 1 1 1 1 1 1 1 1 1 L
                                                                            jXll      JXi3 113:,"
                                                m
                                                                                             ]
                                                            j 芦'I
                                                1
                                                1
                                                            1J
                                                i
                                                1
                                                       =
                                                1
                                                                                      "
                                                1
                                                            1
                                                            JN"                         "
                                                1
                                                1
                                                                                  "
                                                                 人,.)       jXi)      3X巧 J[ 上S
                                                                                             陋
                                                                             츠
                                                1
                                                d
                                              겨人I乞 a弘H人k危 和才 ,3                                   /t뇨 口中 aim庇m丑           /x / 光凡M

                                                                        丁뇨如 /At( 加나戶d /'                                 /／낫札才 匕 ＝口

                                                                                 VL -0, 尤뇨 工J"
                                                                        뀨
J
1
                                                                            V3 二 J' 乂43 乙 4:j 乂331> 口 ,-ix 乙


           洪小滋貫川小尸
                                                                            下 h           戶？( '3 工；
                                                                            J13-
                                                                                      )(33 十x

                                                    匹 =jX／二 工； .t-J. xz｝工J 二 (jx,！中 JXZ3XIJ ) r, : o
                                                                                                        X33 十7(


                                                                  凡2- x33 十XX／乙 十Xi3Xz3 二 0
                                                                                  中凡：X33
                                                                       x 二 ）白3辰-3        /
                                                                               X /2
                                                                                                                                M
                                                             丁卜七 石和才 H뇨尹砒M乙                                  d才 Jbd /

                                              m
                                              瓜
                                        二e
                                                    = 孕 = 'j抑幼'쓰끄 jXii t小-'/ 7쯔三．\
                                                     m+ /                        //                         t X33 十入，/




                                                    =J rX,‘．芦；)                              加A4小， 厄 尸抑乙 小必凹                    /



  1
  毒
  4
  1
  {
  4)
                                                                                                 5小 6


1411 1j111J M斗4
                                                         任
             尸




                                  Sn
                                                                  납
                                                     e




m小土 乂未兀 小小派 a느뇨／寸
                          尸寸1. 和Va乍口
S兀伏 그 兀4- 危山m尤亡／，在， 氏
                      加0友凡／石0力乙 ,／寸 咐＝口．
p뇨才j-<4-- 毛뇨dV 而 a- 似友，   毛 小可. 行呵낳노．
w也 小才戶a eJ;d' 4万戶 /lia才                                            V1'/y-                           =o.
                 V; 二 S口 vi-j- 十533 V3+ = e5/ V뇨十
                                  VII.
                 냥＝       . .5口
                      ed／尸 533

                                                                          M曷
                                                                                十
                                                 5 沙
                                                   八              lJ
   V ! = S1, V1中 十SI3 Y3十 二 SI1 V，十          卜
                                                    e             寸
                                                                                3
   V．小                 ( 2-
    !    -   C   .     1J 1 }
                                                         d    .    _J
                                                                      1
                                                                                                    +      -    ,


   可
                                                         1
    " ' " " " 귿크t于卜『' 今 可J尸： 533 －去프
                                                                      m
                                                                      /
                                                                                    <
                                                                                            3
                                                                                            3         =
                                                                                    U
쁘 小띠 OL 比加女 Z九／ 比力i7七-4磁莩 뇨4-.
4人씨孕．加a7M斑旽 :
1 533中S占／S니 " =. IStiI ' !5331"니         C
                                         U                   十n l                                                          S
                                                                                            1 너
                                                 U
                                                                          푯刃                                               L
                                             3
                                                                                                      戶D        n
                                                                                                                ＼나
                                                                          r>
                                                                                        <
                                                                                                                     3     y口       1
                                                 r
                                                             <V
                                                                                                                     =d/
                                                                                                                                        H



                                                     S
                                                                                        U
T '兀 如a吻．肛尸赤乙 平力뇨 L幻 和（宏나 石오I,                                                                                                 ／岩
7缸 沙 :
  l5t1! 工 十 { 5,
              【尸 티 .5川 느 /                   5           芳口
                                                                   千
                                                                                共U
                                                                                CJ                       臼
                                                                                                                      D
                                                                          戶
                                                                          ＼1U
                                                         <J                                                           二
                                                                                 4                      戶
                                                                                                        b            L


  기 知n+ 1 s33j - 二 /                         <
                                             U       2
                                                             半
                                                             小
                                                             <
                                                              m
                                                              U           十             C
                                                                                        U   骨3       t
                                                                                                  丁- -Ii
                                                                                                               e 웃
                                                                                                               느) 33 -o




                                  ．了 7
             J九小工今 S(2 和卄光玖石 才乙可 比才蜘／乙k+ m凡 乂귀上
            -"1／寸 艸Z砒，
                         小 기 S1 I 느4 SI'S彦 JC33          )I/ .}/35쵸                          t       o
                                         5(3               5才
                                                                       +-   /Si31                -
                       小S::S耆 ' S功 尸 S卞5궁S3萱 = 키Sni1l S尸尸 기知I"

            TkJh人／

                    t S33. 5占／st1r- : 1 S미 ' Is녜1.十15口H＋  리5·i1 ' 1 S口1 ' 니SI키 '1
                                                   ICI II        I 1


                                          二 \Sa3I1卜2.IS1키1 二 1                          /
            5,4(7
                    치力       2뇨 小小， 口］ 椰才k                                          小協섐 ;
              ts미1. +ISrtI HSI3I ' +Is'닉1 ' 二 (.1)뇨('1 ') 뇨（'／向2. = /.C/ 芒 /

               丁油平皿 X工丑 싸任小                               /i     十石仰兀4
                                                                小；

               b) l> 系 a丑私私巾Z , L5] 加＋나才力
                                        （ 싸如나立k' ,
                    &‘才        &3半 S31 , ／寸乂；뇨 ,., S名a,,/e＝ 兀4才t4，十a上＜伊如七d上
               c) W卜J小 a奴 a乂4；小， 肛左 4d丑口 似a表凡규 J r二＄II .

                     古       RL " 中20乙; IrL ' 中2.0 勻1) 二 그D <Y乃                                               ,/


1j1t1!!
      11
       44
              4) 工L: -20Z겅 i丁I : 尸2D丑朴佈) = 3d乃
               e.)     v才 = \／丁＝0              , 咐＝屹中
                         v小 = SI, V.十 十S口 납 = 司'V, 少 / -C/3 II3小
                                                                                                         i-
                         v3- : S引VII. +S33 V3寸＝ S3i V，十尸S5，匕戶＝ H-
                                                               . 和： vi
                                                                  533

             님r C= y二
                                         SI, 小 5(3多 : -1/칸f/ 量L坦' 古Z브3O
                                                                                    /   十口
                             \，了
                         二
                                   5
                                       ＋· 'I
                             小．




                                                  f 三7
                              ！二／g ;.

                                                                                                                                                                                   V7=
                                                                                                                                                                                                 =    V3
                                                                                                                                                                                                            -
                                                                                                                                                                                                                e          "J;
                                                                                                                                                                                                                                     'm


                                                                                                                                                                                   V3 = 町 甘j" "


                               和M丑 和／ a./ 尸규／,                                                                                                            戶才그 小d扁뇨／. r뇨乍 匕往..
                              口皿乙            31之 =SI3 : SL1 = s.z나 = 53t : S了4/ =59z. = 54/
                                                                                                                                                                                                           )          =0
                                                                V2 : 뇨， Vj十 = 汕e그／' " I'今’

                                                                 V3 : S33 V3
                                                                 "9 二 Sqi 已f 十Sq1 甲 = S乎／ i/,t 尹-                                                                                                                     eU
                                                                                                                                                                                                           Vy                         100V3

                                                                            = 5q, V r 十5 nS33&' 'O "VJ1
                                                                            = 5q，니， fS,qS;3百」
                                                                                            구' " Li今m
                                             V;(! m53) - ,ei " ' j=
                                             v; (t- sa,             S#,V,十
                                             Tz丘 : 54/i5z. t "J ' "
                                               V才  尸533 Sv9 e口' D"
                                              小 佃兀肋泛竺Z끄으"
                                                                 /i7m竺可 乙67Z쁘／                                                                                            "
                                              套 .62，
                                                   夕／尸／7口“

                                  二L= 如石7 乙6 ' 力 ' 侁口8dB                                                                                                                                 /
                                             F

                                                               D 뇩
                                                                     G

                                                                 ＞
                                                                                P
                              S 1&K3AL                                          A
                                                                                r           니
                                                                                            r
                                                                                                        SOLU丁｝C八3 :


                                                                                       1d >
                                                                                            二
                                                                                            ／




k＝ 뇹丑卜r小1七出L事韋mm啞好妊HHn卄크441
                                               5'j
                                g        ;
                                         t了
                                          1
                                                                     !1m!
                                                                                                                                                    )

                                                                                                上 1寸1
                                                                                                                                                                                         (usE SPL, Tr,,J&. RULE
                                                                                                                               4； 八
                                          匈
                                                                                                          뇽3
                                                                                                           力 ＜
                                                                                                             뇨4
                                                                                                                                          rJ
                                                                                                                                                                      乞                   A*JD SE나－L<＞口尸 Ru乙E)
                                                                                                                                                    i (
                                                                                                                                               口1



                                                                                ＜
                                                                                나d
                                                               加                  E
                                                                                            d
                                                                                                1                              4

                                         1




                                                                                                                   =
                                                                                                                       a
                                                                                                                       ＝
                                                                                                                           勺
                                                                                                                           6
                                                                                                                                                                              So,
                                                                                                               H
                                                                                                               뇨


                                                !
                                                         ／八＼
                                                                            f,
                                                                                 S小．
                                                                                                  .,
                                                                                                                                                                1==   뇨
                                                                                                                                                                              丁1
                                                                                                                                                                                             =                  S4/
                                                                                                                                                                                                                                 j   S23
                                                                                                                                                                                                                                           e   -'
                                                                                                                                                                                                     / 小 S33 S4/                               勺百
                                                                                                                                                           /1
                                               >':＝斗二：
                                                                            H
                                                                                                        4bmH卞＝                                        느＝
                                                                                                                               H=     e
                                                                                                                                                            ＝尸
                                                                        i二＝      J     :'
             工／9
                                              七尸- a. ,
                                              -s-
                                                           bt   ,




             尾力M r드 .g7/
                                                                        P今乙＆    ／· 寸尸寸1姑뇨
                                                                           ；瓦＜ 口＄
                                  쒸
                                           乙 2 - 근01
                                           3 工f己'1
                   sit:
                                  , , :,
                                                                        /2m才 그 -4'- 小小亡凡力

                                                            긋 굼b/        （才白加印比人 다7多 ' 7勻M
                          5i2 =
                                                          4i + 죠工
                                                                                 和才 丑 乂누 /)


                                           ==                교금＞L
                                                                         （土如如入 口7伊 戶如
                                                          云＞ t f Z乙 t
                                                                                 戶才／ 名       二)

                          Si，工＝                           乙 r ＝근e t      c-i今／m乞二 幻多 寸肛才2
                                                          玉i ＋西L
                                                                             40／뇨作肛才1 在                     加加나）


                              7仁Uy 乙6毛 万二그 :
                           (} 十s11) = 工 qgL프'                                    （나뇨十 /9gZ二프“
                            仕st.) 二 /.00 스쯔ft                                     (L- Sz-) = /.boLYf

                            SL2.52i = -.3 6                              (I-S%I)午S띠 - S1:S2/ 二 /. 3',
  寸1




ii可m蛋哺心年＄垂
                            211 二 .5Z) 乙y8쯔스竺已 3石                            =    .2. 7 亡I 百乙 0       _1乙   /
                                           1. 3c,

                                                    /,zL?으              :=                        /
                           2!l= 三치 二 万乙                                          J' 們｛/ 工／
                                                     1. 3',
 1
                           근L：二 了O L쯔互 /zig스쯔 小· .3石 =                               교．7   中j'5그C 十             /
 1
                                          3 ",
  귐
                                                     /.
  i

  1
                                   F，그小H 乍石기／

                                               S乙' = 'I可 S勺 "
                                                     厄：r
                                    Sr1 =5/ r
                                     si
                                          'i




                                      晃二Y퓽二 S21

                               PmM r             A七 百' / 光뇨 가8CD·
                                                                  尸m小疏나 7)弓乙
                      4 a뇨小4小4qm 石辰足 /Z磁O거」乙上，                                          "
                          杓    “ 白아丑               , B勺'已A샤乂          , ' :J '）뇨샤／

                      兀竹 加4                b恥e 5.,Z .2투 白小才石
                                                                              근－尸dM他在4- ,.
                      匈       스C
                                    으므츠느 : . I' 西 白才尸i
                                    j 7O／依1            "
                                                                       /
                                                                       \＜그느
                                                                              -) 4 1/. I
                                                                              亡H - ＝于 r
                                                                                   二／ 口： 工六＞       )
                                    古 : -J 근. 口之 ／又
                      已       으乙
                       t             q냐乂               ' 그 /4-Q n
                                                    二 中J 1녀） 1力q r吐    佃7근山多L    十工- I 工 之＞ /
                                                                                               \



1dd川4mn1d斗H甘1H円 aJ{




                                                           6/
                                    v1: AV: + g r2 = (A+ B/ o) Vt
                                                            Vt
                                    11 =CV: 午D12 : (C十P/6o)


                                         느工
                    근
                    1
                        M
                        놔 4
                                               乙A- 十 B/6이
                              H 1




                                               （르 十 D/6o)

                                          V1                                           /O
               叭三Vt =
                                     A十8 /6 o              （月＋B/so)(근瓜75D)       A十 6/(0十50乙十50 P店乙

                =                   I0
                                                小   ,;?_
                                                            .5-   그
                                                                      ／     //

                    -I. S乙 +J 子 引



               (TM且 瓜十戶寸 比尹4 m                                            4 ／눗 戶烏伊兀U 7 m     5cj_



               加岫小口抗 4 ／뇨玉m/ 교4 力凡 戶才 4工M
               而伊珤小枇D                                                 .




畏




144Jj1J4耳4 m
   F뇨M ＋仰j砧4 7乙1 m尻 /' p , 如乙岫／ 名
5. 2 6

尸 的小Z? y，伽名斫 . ThM 蜘忌才 石 가B切 小4i짜
                       ID/
                       匕'10 A/6J
                                 卜3)
                                   , '낚 " AY'回기
                                             s
                                                                _
                                                                    t/
                                                                         8]
                                                                                           =


                                                                                               Li 乂 Cd比 日／                       -JyIcc十夕／j


  Y2.
                                 "                                                                  i         뇨尸
                             나兀C44小                                                                 -j Yi 白才尸乙J
                  十V
                                                           '甘
                                                                                                        y2
                                                                                                                      ‘]
    r5 (y：白才巴，十y，白十尸D                                                                                                      J'()；댜亡P7十兀C4夕【）)
 沂＝ }                               .        .                                                                    ,          ,            \ 1
                                                                                                                                    fy工
                                                                                                                                     '



                       [j (Yc／七 PL*YiC4亡（9L)                                                                               -j (）比才日／          cc才訊 / J


    4 = m Yz. := Y1 <b才4／十）뇨남尻． = 匕寸＋&
                              V2-
                                                 1                       y, Cd［七 多／ 十y뇨 Cd之 尸工


        "     "        亡     ,),                      『，
                                                                ,
                                                                              J
        c-
              =        =
                                        Y,
                                                 ,1
                                                                =                 j   Y0
                                                                                               4-
                                                                                                        .i,   -




        ) ' 玄e乞戈豆交2),
 많＝亘 = 二 =               i               .
   C中  i '(1 (Yic (P／十Yz C4亡尻rK乂白十햐＋兄白r汐U乙

             0 = 匕d고 y4 白才 夕7 十y2- 乙才夕工
                     'I
                      'I ＜乂比 dl/ 十 y2 C4 戶그．

                                        푸 夕I: 夕勻 ，老뇨 口伽e 4mJ才乙 枷규卯 月二

                                             小夕：嗟多白砧7 ·？「日＝吼拍 /
                                             好q,J伊斗甘也）낢iP " ".                                                                                           乙 근 Z.

                                                                                                                                                         Z1/ ?2

m仰md切－（夕九价仙力-cv, 부 才灰口 C系枷M뇨n立 -C---竹如口47
                        n
                        'm 二쓸二니기
                        小k 낫表丑 和－加毋 근 emmMi左＋, 戶가M ／他
                        乂BCI) 和八4M，允1
                                                                 I근1                                         1
                         A = 크ii                      ..\

                                                      b-
                                                            -

                                                                =r中                      C   ==
                                                                                                   ＝戶n戶n>
                                                                                                                             +,
                                                                                                                             J7 ;
                                                                                                                                         근工工

                             2二i                                 dL1
                                                                                                       근1t
                                                                                                                                         근工1


                        7i0Vr／友t 人BCD                  私4九； 741Z屯 m蜘往 伊m工J
                        C／八元八J;}         石．.     口M4nq/ rdt石乙－ .5-.'.) :
                                                 뇨




                          fh6]: n叫！
                          L乙'J  LjT '- 尹丑
                                          jR. 44. 씨II 이1c.o.c&丑
                                            q4f丑 JL0
                                                                                                                              근 白놔汶七j 2b七A 戶又 1
                                                                                                  Ii             Li . 月瓜P工         白나.9.＋泗0Ak肛．
                        Tkh나            ．



         니n 1t作냅求J拓求4
                                        4 = 으L = 르끄 二
                                           근21        귿Ii.

                           22 .n2 ii 二 缸，／르즈 m 亘）=                                       P -A                      \
                                                     \ 근2.1            근.LIJ              C




        k汪仁二二4GJ41녈lj
                                          二    j근）。 小；／更                 :     2.        /
                                                jy口됴｝文

                         근二
                                         : ＋染戶뿅-x等
    n心胃나
                              小
                                  2It
                                                                                                                                    b



                                  O乙／
                                          乙 = 土V극卜 囚2.


                        （끅 /：衣尼 싸茗豌凍． 厄 加兀巴 才毛，                                                                               ri     J    d:t기乂－ 二＜4八又．e
                                                                                                                                    LJ          :




                        小＋어· T뇨叭c f1“山／근I1 -mX,                                                                                    Z = 근22.

                        小們叫 』 aMa 西：土恒｝  ：系H /i ／叱｛· 감 才瓜
                        J們- Lf 戶月n才 乂4- 加竹싸 , m닛 .和仄」山· .\


 晷n4aJ1 1




4H네뇨너n니na놔n =nJnnndn
                                                                               6    (;
                    5. 2 9
                                  \/1 二 AVz. /5工：
                                                                                          v.14- V.J + v;
                                  工1 二 C. V1 中p工z
                                                                                          工M = (1/J 十 \/;)/i,
                     小）
                                             V'4 十V; : A (v1+ 十v;) /B (V寸-v;)/／근.

                                             니느 VI" 戶 C d} 十 r; ) ZD 中 마
                                                                                        吟 _v;)

                                               Y夕 卜VI = 64 十B左) Vt-

                                               \/J- v, : (C z. 十 t:') v;
                    QL似뇨左                    V寸：
                                                      V，十十V1' 二 쓰旦色
                                                                    （匕* /K9
                                                                   c_ IO + D

                                             VNC 2. 's-P 十A +(3任＞ VJ(A f昌／西 小c.
                                                                                                          .尸P9
                          SH= !L)      : A + a!玉叱瓦功
                                                                             /
                              切十I '2中＝0 A ＋可눋0 十C?O -1-P

                    4兀뇨뇨危              V，中 :
                                                       aV,+ : (4+ b/ 口 十C근O4-ID) v;

                                       ！V11'치Iv：二＜>     =
                                                                    2
                                                             A ＋乃／已 4- c.乙） 'f _
                                                                              i)
                                                                                           느／
                                                                                                戶




               ／和
                          V1十二O    乂浚工 ',J。
                                          v{ /4才 a助口似，／今．

  4F
                                             yr = (A- s／召D
                                                         。
                                                         1) I,vi.'I' + （月 ＋易／2D            y工‘



n1 de巾H布年斗件吐
                                       戶 \/1m- (c. 知功 V +vz 十 (C瓦
                                                                                 十고） 」' ;
               놔戶m枷4-
                   4X    \/1- :
                     tti V1
                                                (A-e/zD + C2寸功忙' 十 （戶十 冒2
                                                                                                    I i-c 근. 十

                          S7.2 = ＼丁                 = 버戶＋E／乙小1.         六；
                                  v+
                                                                                   "/
                                        j\
                                             ／十＝,     /?＋乃， 乞卜1
                                                                  '乙＋   p
                ,J力加如丸， Vi ．·
                                            V.
                                                  -




                                           A + b/ 。                     月十B)/ZO
                                                                        A七／
                                                                                       뇬.    V，
                                                                                                  -
                                                                                                        十＝
                                                                                                             C2.+.P
                                                                                                                  -
                                                                                                                      'I,
                                                                                                                            -     C乙
                                                                                                                                  CZ0rL)
                                                                                                                                         少 V    2.
                                                                                                                                                     1-
                                                    1               ＋그        /A.8+b/2e
                                                                        n二 VJ 'A        C2亡_#0D'/ )
                                                                                   ／己 C三＞
                                                 \4十tyZe
                                      少／
                                                                     C乙十DJ


                                                                                肛흐生 C2口中p
                     s
                         '乞：
                                     드                          =               X4：쯔在；-C乙十p                                        므      쓰뜨끄小
                                                                                                                                  月 + 自／乙 十c2。十0
                                     tlt2                                             ＋  1
                                                                                       尸H누


                                                                                A十b/z。 C乙 寸 p
                                                                                  1－
                TL七／皿d毛 甲皿 m；檄 乙Z在 三 2.

                5. 29
                 已.m,.               了．sZ).                     ［三］ : ([ C)］十［S])"'（凹吐j)
                                                                                       寸5t.                                                               s,a]
                               /\/ 二 乙／
                                                                                       n-5.. ,5': T1fi色 尸SI, j
                                       ([I)］心寸' ; 卜5지 /-sztj ' " "씨                                                                        工）
                                                                                                                            l
                                     t1 二 ( '- SI'泊巧n- s／工Sal .                                                                 ThJ,\,
                                                                                        {i+
                七玹고心／
                                                                                                                      z


                                     古 i_ sal
                                                                                                             S,
                                                                                                  Sii
                                                      Si-
                                                                         S1t]
                                                 t-
                   [2]
                                 :
                                                                 I_SI, jLS치                                  /#J乙니

                 a느
                                                                                                                                 근, , =   긋 旬1.
                         근U = 小S11)(/_缸片玩Sal /                                                                                      中      1)
                                                                                                        "
                                                            p


                                                                                                                                                +S므S가 ，》
                         ,)  m              그 52/                   /                                                       毛, = (I百,)(/-#-Sza)
                         T2J "                    V                                                                                        p

                                                                                          乙6毛 工之．
                 T뇨四 4肋44)乞，                                                    a.們七 小元光人




                                                                                                        6g




Jmddd川m니U尸V니d
                                         5. 30
                                                  5h=S2. 2- 二＜>     ) Sit二S亡i " .7口7
                                                                                           ,     r5 : I瓦／ =0
                                     7色V         근L= 5口，
                                                       乞I           rl = f：
                                                                          山 =0 .       a4\J4人．

                                                    Gm = Is工i 尸 二 ｝노

                                                        Gr : Is미 ' : yL

                                                    (; = [Si4 ' 二 7i
                                                                            .

                                    十       끄二丑百小，                I노 "y.3
                                                                  r血 =      知S工i rl
                                                                          I- stl r      小 已t

                                                 G/i:     Is2"乙小sI ' )
                                                                                      1s2.lI1 = .5- '1'
                                                         江s11r5J' 仁 隘川I.) '                                        (5; ")

                                                 하nI. 'y '，
                                                          r-0 11
                                                             쁘-1.낸U叫：

            r\>41JJi11iiiiai11i1
                                                        江缸미小 m Ii-.S ...
                                                                    口，12.             .1..(i- Y,)= , 4'fV / (5.g?)
                                                 (; 二    t5m' 0 trl3) :
                                                                        士 力U .
                                                        仕知띠mdC시' ) 卜CI   治f                               957 \/   仁；y力
        薑
    1
                                   三3/
r
                                                                                a1
                                                                                        甘j,！乂         .   ..
                                             1                       =＝亨＞


                                                                                b,
                                                                                                  .



                                                                                       e5놔




                                                                         石 7
                         1炡 什고                             7Z乙Vr升尹人 /4-
                                                                bi




                  斗尸云工 小如乙니 力小石刃 "
                       SL2.
                       c1
                            , 江13s습                                                     하＝ C기       S口         /
                                                                                                I H 1 G S Z3
                       t)/                    sLl
                   ·         m中HH나eH




                                                                                                S」二 1-I-       /
                                                                                        b ,＝山
                                                                                         .    卜r1. r3 SZ}

                                                                                                                   \

                                                                             . .   b3= b,     q52了
                                                                                             1工r3乞



                                                                : 成（1니디' ) .              IS시 ' m1r기') - .. .
                                       트巳 r                          4} 0니m11) ' 江「，r3s히 (I古蒜고）
 U
 크k



                                                     1s121U- Irr)
                                                    W口G5히느｝町기"
                                                                                   거／
 亡




LL七＼ 1
     1




뇨 什 倖 4 i 4 }(
             t
             1
                                       巳百           낢心
                                              q


                                                         dJif_. b3 1니Gn) ,
                                                         &3                        15띠' r s미' 午向 ' )
                                              1 十




                                                         b} 띠낀ir- I) 江nG5습m, 多므늑 ',)
                                                                                              \"    n可iG뇨키 /

                                                         iS.d니r21' (S너t -向’)
                                                    h工r3S히'41工r3s치' 니S}n19

                                                                       70



   巾 J(L七뇨＝)H尸y
             了. 三3

                           T나 白놔尸石少 /y尻亡7 尸小 小／思 白寸比d
                                  oi) "                  a니   上；
                          가＝{'" " ' k " ' ga' "
           似W7
                                                      J
                            （드／
                                                  -
                                                      文二O 늉 =0
                                          A
                                          <
                                          dm
                                           小
                                               M響.J昑二］[？告M낌可“
                                                            " " 吾］小
                          ; 坦竺 三 브쏘 eK阡降")3
                                    :；二    弩y

              口八月 小和／
                 l4 F＼皿
                         ;;7 m쿄 沚 亡／，丑 m =' (rs10)
            如七， 戶 P卜 ／뇨 小又
                            , q小乂 陛 4 小 沙
                                             어戶
           가人＞1 ,
                           Zd q小小小可 戶 ,44) I;                              7JiLi, ,


                                           , 근亡＝ 굴. 小／阡 : 什
                                                                   川./X《 7豌 ?2> /·

                                           [ 읓뚜止肖十［
           丁｝
            ＼石勺
                      "     Pr
                                                   "' 시 和LO.
          小加亡 肛닛札十 師m卜이
                                                                   加弘i4亡夕 M
毒         小（加（，彷，乞 石a</ ,

          1三39 i
                           丁肱口 小4毛小 k札 k                      ／古I I ,   肛磁9 M 石寸
          好恥丸心 ／뇨 片. M +: 恥
                            dy （도 “ "）· Bd Q 3Me

m
川나m
  琡m斟
    h小n
          bm 和刃亡J砒 品缸七 加m/／吼
                                 万b乙 王-c力；工‘ -,
          丈兀匕 dAia4, 刃4乂乂 7二
                             H砬仍｛                       V才仄坦 a,em立；，兄兀匕才     局＝.C?! !
          A1『 ·그9느쏘                       丁뇨 小尹지完瓦 伊牙
                                                      口机 石              成y /di1 <)）八． 元乂꼬
                                                                                      ‘




                                                  7/


    n1汝
                  1: 1 " :：노；L m=1 i윽1. "1 드 u or F可5 : !r 1三寸：    .! 1: 卜imFL.- ；三 三r드F
                                                                                             · 1 =1二 勺그；4
                                                                                          : 1：
                               : ::IF'LE .. ,-fl. iC,'..: . : " . : 口':. . ; ·：· :, 1 . ;
                               :!:4片LE- i·ET . 二：: . " .．三＝.n . 三：·；.
                               ：· !m日寸드 i （可' L_ . i o:- . ' : " !r : 1: ：」 1
                              ;! = 3. 1415f'2드5
                              :( ＝三二：    1.
                              = " r : t七1i J " )     三r = 二．! ; i " 4 : 그 三 i . : 王 .
                              : 三．니［·· 6 . + ) A .C . !:i
                              ./ 나t1=1.
                               t= i 1/'a
                               C = C+ i
                               y.r. 0 =2 1寸FI /XL.日시
                  1: F .1 L！
                           日 ！늑F山AYS
                               三Ti！   슥＝드C'FT (XrU玄戶r(1m t ;'I, " 尸 1中夕i ·
                               二 iA＝뇨'0寸ZO/E;T1;1
                               : :: 二； ：· ; :＝三 1；旺
                               :·c i c' N=i, t.E
                               ETr4A=C코琢T ( (i. .C. ' 中나小甲"＼             卜小이 ; :d下‘ 1..' 六）*竹2)
                               !F (AIMAG(EcTN' l. C-T. 0. ) ET;1A= -E.TrJA
                               그＋日＝>:r. 0tZ0/ E:T1댜六
                               C：虹N,!닉 ) = i. 0 . . C, . )
                                :F, 11.Ee.N) C. -（尸.'J "· =나 " i.
                                t 'C' 50 I= 1, NE
                                                 m
                                C丁＋:C=C드口FT. ( i . - 0 . ·，‘ 卞 !:4. L : m 1 卜‘．寸F'；』
                                                卜‘: = . ！三느 . . . : 三！i C ＝누三r+.(
                                 : F1" A:HA5r 드“！
                                ：卜. L＝戶．i七士Z已rETEC
                                :m口1,Il汁mK凡N) ＋二；I-啞 . 』．C朴n 1 k J411二 . C ) :1X1 ( !{ . r< .H . C . 尹“::;＋六
                    닻K
                                 C口1Tn孔促
                                 C C4T 11나UE
                                 =! ;111) =t (1 1. 0. .
                                 iF (M. EQ.1) F七녀rt1)＝띠m12 .
                                 Z0 ED i. =1 ,NE
                                 B丁IC.CS0kT ( (1 . 1 0 . 냔＞乍．口＋xr.on 卜.＋키／C)卄2)
                                  !FiA；卜ZG( B了ICC) .G= .C . ;i 드了KC= mE了卜．C
                                 :EC=XI:C+ZO/ E.Tp C
                                 n4(14) =F斗i(t-i) +ZKC少2 . · C中，: r 卜뇨 1卜I ,.-. . C）寸Xi ( F, 1 l 1A ! C 느：三1白
                   E0        CC". 4T1I4i.드
                   4C:       C心4TINLIE
                   C :: -:三k= tl..TRIX AND 야寸IFUT三 戶 I-a드CTCI. ( 王 taridard natr : 工                          : flue r드 : or.)
                             CALL. O11t'PJ( 더4 ! L' E了 ! 느L .!r4 . l00 d：三)
                             C心 20 t1二1,NE
                              II1(M) =(0. .0. )
                             ( '0 20 N=1, NE
                   C亡        At1(t1) mm1(l1)＋口1(M.N) 寸Flit I-I.
                             1寸r1 t! (6汁） - A V. CtCT (Mag. Dha! t) :'
                             I-心 30 I= 1, N드
                             尸1켜l1=CA8S(AM(N) )
                                                                                                               m




                             FH5t1B0. 卞B丁二-'-C（쇽；！二二C (二H1小1\ 1 q PE存L rA서（N ' \ \. 샤卜 1.
                    三C       :<R!TE( 6 1+ 노 小너 1;Jr너 1口J드
                    .:            C3IFU7E F드ACrH=＜三
                                  노OZO=C0. .-1 . \+( 1 . 十二J4i l \ ) r注 l . 戶；亡4r. l ) }
                                  yLF큭110-2. 竹P1／드 ！二
                                  )J1=X口ZU*XL.侄川三了 C . 甘二 느
                                  ;m; TE(E1古） " 乙‘a- . C 1白 . ' ;i. bt: i/ t= ' 小：       m二？4가i.            ==1 ．놔；
                                   二：：丁C, 三 00




斟 i 새 心 七 기 h 山
                     三 : .'        二六LL E\ IT
                                   三：<1>
                                   : 二丘！三口i >: i ! :! . L. . m . 二 1
                                   :: ==.: . 고仁드三고三三
                                   m7더1=P ; 出 ( N/ C 寸4, 片 ;                                     .
                                   4PG;＝구！身r !4쏘：    +r;. ；止
                                     .: P亡三；r. (o臼升3戶吐 ! ／· .. 乙 ..,m.; .．芬그 ．·
                                      ::4＝二 三．
                                    : 二；H三三t尸i그！; J;H . = . : .卜三 1 .:: := 카 " L 1mF. 母" ··：』1 1 i . m：汾2,
                                     ::=1
                                             }:m ; =
                                            .1   ·：




                                    : 三＝L:! : :




                                                                              7又
           小
      5- 3-5-


                    小                    나   q
                                                 ／瓜 aeC名bK 丁．g :
                                                                                             ／多J         戶d什石 ‘二4/

                                                                                             ，石才 乂＝ (a中C)/Z



           呵 町
                                         쯩 凡
                                                 口r                2d
                                1
                                         =
                                                  U  1

                                                                  文1
                                                   e
                                                                                              町二二二An兀x ,,-J片y
                            八
                        m든弑
                                                                                                   기．q
                                                                            許                     근今                   =;m                C戶


                                             m
                                             1
                                                         雲                  小
                                                                                             町＝巨孕- 4꺅ei降舌구口
                                                                                                斗1= S    卜mq
                                                                                                                                     口느
                                                                                                0dd.


                        m2히 R
       亡j
       E                   瓦』
                            A쁘(z닢)三JP：孑
                 們 1人
                 'i= I                           C                                           lI, = 글肛，廂響(x-I厄r'方
                                                                                                 今丁二 t   i스；
                                                                                                               如
                                                                                                                   1
                                                                                                                             C
                                                                                                                                 쯔
                                                                                               口氏丈

     加뇨化 忙교老小刃a)'                                                                      外＝／念小劤）"
     Tb此 和乙土H 卜力-4-
                                                                  乂人兀 和似工 戶小 4+ ／드
                                                                                   I,口） :
      뜨 4 444                                            교2i꾜＋
                                                             ,m工＋
                                                                ，月. = 글 三르卞工＋y工幻
       t   r 1
                                                                            qZ二
                                                                                       表＝/     C Z=
                                                                                                                                     욜
                                             '

                                                         )
＋七
                                    易二
            小，
 d乂쿄尤k,                                                                     +＜二               m
                                         工mdm婆aa加倆
                                                                  (/
                                                                                              半
                                                             2=
                                                                       </




                                                                                  73
                                                                                                                                  /4      /
             5 " "   1，      』M          仁．     ,，刃 .        刃小似
                                                                                                           乙＜4/t八／斗凡人




              豆 二 .八 르브끄즈 乙d4스즈즈 ,4，쁘y                                                         + 4 2可- 11-
                       (i                               口나                        b                -        b




             戶沅小 7뇨1在 9. ! . 文뇨 Z汕小兀 戶／在7抗 !                                                                                                  兀고万
             TM們卄 和力7Ze+ d/m/
                                                                                                                         ;/"戶孑
                            E: : 立f끄工 C,工 m契C즈                                                                       e                '




                                              긋；a-

                                                                   和                           警                    뿌    e   寸十   1
                                                                                                                                  U
                                                                                                                                      a
                                                                                                                                          孑
                             勻 = 王무王二쯔 C土 石；
                                                                                                                                      J
                                              - E b


                              小“ 劣尹 C" 加스쫓즈
                                                                                                                     戶；J：尹孑



                              幷8" 艾”' C土 勿＋誓' 小k으쯔쯔 e下.1"戶孑 .
                                                                                                                '   力


                4＼工h工 C,士
             ，凡乂，
                                                        m                                                           小m
                                                                                                           mM尹工抗m4-· 仄才 5=D,                           ＝
              E亡 /4-               -y苡；蜘如．                             -4-   亡中       C十       =       -C 1 4石乙 和（戶"-H-)=                              七
              h           H/-//J' ：그'S工                 h/                   ．月노‘『娠 “丁Sf .                          展乙
                           . . 』， =. 』＜＝斗        .                 』                                   /                                      L ZJ？寸

                     시；: y -1'니C   -'尸
                                                (C乙c-)= 그可孚 ＝芍 C-十＝-c = 瓷十                                                                    느／




                     哮升七" <D " " "' 多功 a十＝．己尸： 士亡쯔 /
             小오 月小比 戶4脆 m스7今 77k/W訪伍 十兀小
= 늬
  U니H
    \ Fh기｛
              md 尤征 小m뇨乷 白M尻法m , 力／놔加仁乙石小
                  力싸小 石亡二只乞니 ‘
              亢不工




                                                                                           I
             I油小                 (5" ' 乙） , 元뇨 石亡mt皿 如M《／，在，
 k37!
                             +
        川"   ’父 只‘佃' 링L 小響 白＋ b
        H     -          4           -




                                                                       ,;28二，孚 的츠쯔 小k 끄芟
                                                                                                 141       b
 F;td入 T瓦匕在                      吼 2/ 才乂L 名b如W似， 丁万I小m

Z油兀7 小呻                                       的나亡 加況乞 口，4_)

                                               Ct q4響K 八罕 e可肛
              E戶 戶그町 戶土 . ,
                  上） L-
                                                            9꺼7r(
                                                              ：卞




                                                                       꽝 誓
                  I-J        = 土
                                          叱可   쯔b                            的               냔J戶孑
                                                    十
                                                                                     쯔
                                                               小
                  1 1入                              凸
                                                               m
                                                平                                                寸
                                                                                     b
                        土                               ＋
                                                                   m
                  H了 = 1-菁
                    .            기- I "   -                                              쓰
                                                                                 1
                                                        亡
                                                                                 如
                                                                                         b
M뇨           C' 小                才뇨 小枷                                 싸才无尻小 乙2才 己FO.
尻 1.+ 口磁仰似 , 孑寸                                                    C ' 二 .C. . 口／ ;. , ."
（귿 ' 戶트DX 和 M5 . ,4寸                                                              "    "
-E立 ' 町 "M凸 多 十c.+- c- =
                         그可．누                                                C드亡＝ B二m
E/ m可＝ 14釵 今 十e' +C "= -긋乃乙，＝今
                                                                                     C『＝t- , B二.       /

닢4,吐e 才似工 ／上乙丘 加7亡升
                    力奴似仄                                                                     k孑石m；乞M
M            光凡 小mG秀 m口6也辰 , 私加三如才
-7뇨W 크版e 如小妃 戶亡乙‘2三石두 .                                                                      d




                                                    75
              匕쪄                乙巴蜘勺 易勿寸也

                                끄xI y, 3)『 工臼） 5介，5/' J 訌3-)                                                                    7弓＝乙 "y <m
                                                                                 ／
                                                                                               二
                                                                                                   孑十乙
                                                                                                                  孚         ,     乙＝낮小小
                                                      7
                                                                                     九
                                        13刃 )
                                                                B
                    ／뇨m
                                  (5.
                                                                                         匕兀 b
                                                                    =
                                                                                          근／
                                        13/
                                                                                                                                5 )
                             朴＝士工m 娶
                                  (5.
              7乙m
                                                                                                                                                j
                                             ))
                                                                                                                                           c/
                                                                                                                                      aI
                                                                                                                      /a)
                                                                                                            (x-
                                                                        .汁口工臼戶
                                                  dM缸dm                                                    : －兀      r뇨如d河
                                         '        和       M表d
                                                                                                             F二在qt表d 已＞

                                                                                                   在／ 14J;d겅

                                        끄 극 (CH未／/D
                                         矢 帥 戶，小긋 /
                          T卜工 冗比／ 尸如吼 7Z乙可                                                          .／냐＼
                                                                                                           /Z；占e 丁득口 4如口在 屈)

                          P 二 a.b (4才／乞                         (1象石乂系 ' 如乙才뇨石步 ／仁mM巴4- )
                                ;2 근／
考
                          小辰兀 IA시 : mnD
                                        2t小t m加依成品 7k加名小乙 在．
                                                  芬
                          Tk시，-

                               尺瓜， = 긷 , 二 （兀／7 ／규才尸 .          二
                                                                                                                   근／ n그m兵／)乙
1
1
                                            工, ' 근，                                                               a:：石b 促느口珽乂
j 4八nqL 1a下


                                                                (R戶Q" t/7工                                                                      弩
                                                                                                                    근／    2三b,. t
                                                                                                                                                    .,/




                                                                伽仄 ' 4乙叱' 느‘                                       芚느：兀 b "




                                                                                                   7口
                   匕쪄             戶記h뇨 든枷놔也 '5.Ii :
                        了（/,5．引 : 工Sr引 [5(,，띠中)中8仁，3四中)그 /
                                                                                  名1 口＜二／< 力
                                                                              /
                    巳1.小，
                        』 乙石L丘． 9. 又．

                                                              八
                    TE10:                         f} , =   二즈      /4L4M끄즈－        2, = 毛仍
                                                      "     Z1          口1
                                                                                            力3 '

                                                          二 尸츠小 4.4八； a万1츠
                                                             2 l        口＝
                                                             n = k二n7U'
                                 F71 = （兀b/／근／

                                 p工 = 口町及
                                                             肛 “Y毛'，伽7aJ '
                   F,t,d),,/(5. 1.7/);

                        小 甘꾸7' j和 :               푸으／小h哥 m小뇨 誓) = O
                                                   r /
                                                                                        /

                       仄"븅                       푿뇨．小즛品誓戶 쯔꿈
                          , {j; '了a寸
                   님亡叱乙 乂／小 弘施瓦디
                                                  A4+ m            口d/ 싸小고存
                   仄侃d 元征 m鼠 7 Z名工
                                   們在， 甘 小1/ 口4
                   伊亦毛 力汕磁口 冗枷／ 屈十亡 口如 山也
                                          只缸' 戶a

                   客二七仰，乞二'二：
                            1
n磊 嗜負
    押： 計卄牡比卄聲理藍費



  ；
  1




                                                 77



      i냐닙나r 나
                                                                      辰 如i乞됴 드7 ;
                                        品Z4M뇽 ／不工 m汕兀乂
                         ．夕. y口

                          F,   1力l，人   C 5;13 'i力

                                             炙 x夙 辰疵 ).dg =fc          ' 夙 在 ' 厚）dir-
                                                 百
                                       小 巳
                                              ) t41 ＝百工 , a+ 斗9뇨工Z /4人 ( 5. 12오）
                                                 十
                                             =   4
                                       乙 瓦：: r乙 .j e孑D ej弘孑
                                         m
                                        = 尻 = C- 瓦嬉 b比汗砧
                         小H枷旒 汕                      ／加구小；
                                                         夕 力伽已 -aft澎 厚 ：石，
                          月／L -0 :

                                       抑m日 瓦可' ).c/ 二 ,，乙仄“ '／万dir
                                       磁 ,（":
                                           " ' 吃－艮‘油了）'/1 “戶.'- .t4나r
                                       工
j겹哨恥畔n

                                   眩 : 亡JJ；·M dr                    竹夕 加乞乂 .5-.／了百）/
1知斛斟J
                         닉d小쇼弓 ! 沮／ 瓦 二튼生 ,                         夙 :Fl三 名 m뇨' ,

                                                         a/
                                                                    （陟艸 d似2及 S__li6)    /
心
니




셔d\H H n 捕 체 斟 弱 算 1 n




:川 首 5 薏 捻 發
                                                              7 y
                         匕2口 -4-,-' .늦a小，
                                        尸兀         万．／그 )


                        乞 = 3 工.万 t;3- .gCx) c(i. 亡／
                                                   【7 百（孑）
                    Ic    = J. tjJ긔口 P竹

                          二 初'白札 乙 兀 rf g ') :臼‘b/z)

             F口1 나羌&工        TE/ <, 小m婉，

                   e; : 了 和i吾즈
                   m小
                               八
                   h ,『 츰 小；뜸츠

                   h引 j和 아끗
             口m乂    已＝ 毛O小／乍나             )    Pt = （兀1／已 ,
             Fa小尸 戶·／了5) 7

                   尉寸｛(-小加＞ 帖具궁 Z寸

                         “흖｛凡1m/ . _7rzZI工" "                   ：刀7"
             (4名m닉／q m，
                      甲2匕四 C口小 a小4/4 /e 口＋往M교
                                              ／乙'
                                               1
m
나J
 4나
  a1
                 匕／    (7戶-      V
             m尸나7 力 力-o似WM1比吼 C枷竹MJ           (r
！
4                                         d中
             m中 e 加洸孔 ／屯 白7多二a2J


彗4妊甘姓릎44i4
                                 石 易免m戶在 二/Q)
             小3h6石 4 多加友 4                    4 戶石乞 '7-       肛冶 )




                                              79
                                             ( ai7攻比口 ma m小在 勺工 /E7力
                            勻＝ 8M끗 [e5P乞eJ’尹孑7 n2jB4M괄4-山戶孑
                            ／人 y 孕 -4俑끄즈 f- e5f也eJ37 : 二측으 小反卒 q나孑
                                 i: /          ｛人   1J                -         工/         （小日




                     (T九뇨 脚力구24 E片O a-t戶U
                           可. M娶 e尹聿刃
                             片   X      드己
                                                         e万恥r'd)
                                                         =

                                         m푤

                                         白， p力거力力；仰：'4- , /，丁

                                         H 극J: B4八衣P/ : C-

                                 和(            - i ) 寸5 , h
                                        우 + 르르 白印／ = 고7VA
                                        Z스 1        긍／          i         (2=
                     小m博 ／缸 B, ", .
                                                                          （느 =       兀2／月
                         B " 프횰且 gbrM                                                 乙t

盛
                     SEC.人JP ' 缸1)77加：                       (2也交1 (5,/／了) c-a （드／/76次
                     E3 加    力          玉3 口才 茗／:

                              戶 " 프' 4. /4 쫑 e玎1 c’力



4 tn士小J나J甘J去小Jit1끼
                     巨笞 a机C 才7 나Jsj
                            「了 : 프횰丑 m孚 才」
                                         了"孑"d)


  r 111111111
 r1




                                                             . 8 (3


1111d
                         FbL O<3 <d, 冗心七 뇨자七』

                                  E3 " ' 二’ " 小警 [eJ                  "으寸的J
                                         " 크쭈느們m깟
                                                                      砧戶孑
                         m

                                                                                        也
                             3＞   匕／ )   -4八r之， /L42,t/'<


                                                                  口   胸   力
                                                                          H         恥
                                  타 " 꺄少 小픗 [
                                    +

                                                                              日 阡
                                                                  1
                                    『 ‘百二囚凡 及人k 戶a                如
                                                                  느
                                                                      끔   1
                                                                          口

                                                   虹
                                  mm力뇨 勻m 加奴 屈
                                                                      戶寸 m老司




                                         \




 너恥J nq杆L nd기nHn11n jn




                                                            dXU




 1




UdHM亡H느h n
                                      2r g
                                                                          1At未Hh丑喜豪r加r亡
                                =Y7          -o
                /    Y " 1V 二   花五小／ 而Z든 =                                t
                                                                          目tL
                                                                            rh1
                                 m匕
               玎I싼Yjy                                                     戶
                                                                          m
［列！叫2PP다洌9P洌吻］
                         껜＝ 今臼 4旦）                乍표 半力          :2如끼0
                                                                          :
                                                                          L
                                                                          ;t卜
                         加eD 읖나洌仰 굶百 :
             [（戶*g）丹？＋伊，끝川「．a] 읊少／ 금 = 殆
                                                        乍＜g 伽늬
(/ ' :｛吼刃      욜납쁘寸욺叫y｝낳尸瓦릎旺＝
          [（乃g7／尸 뇨却叫 늪 中少 泣 b
                                                    ( 戶＞ g＞口
                                                  붊          크
                        （戶＋g: ) r土9 늚냔-V              Pn 丁
(a尻們．,/ 了y/ 7       . !y 尸즈 ／七 心싸 孕／ 加戶 肛구 까工
( 빤莎＝쓰1" 汁，咐)            （戶4月作9 名L냐少 료工 =j크
                          : 甲 4g 加 (; W 竿 가7 片升／小LL
                    力：그'W (
 : Q= 竹 ' /＝나i/               (c7시I'S) 7加'V (9z1'5) 凡M切크          I方 '了
                                 C月月PTE足 6

                                 ;.
                                      /     （小m杉l 나aJ 名力在土mm)
                            d)
                                          }L= 十J 고0
                                             1.
                                                  '?
                                                          '
                                          4小a亡 ／寸J"2C亡4                                                            ／· 9 t/ 긋，口

                            4규/, 寸t l :                   b: 二 -.1O           /
                                                                                       山亡二 jt 2 :      b2 二 · 7了           /
                                                          X1 二 戶／.7           /
                                                                                                       兀2 =/. 7            /


                            b)            恥＝ 그＋-1 3

                                 01（力d七                 /+j x m교e,                                                  · 2 勺" · 3

                           mt丘 土bj '.                     71 二 ./D            /          和-e二 牛卜2 ‘.     ;X그 = 寸．7O            I
                                                          늬 = 그．（그            /
                                                                                                          bl 二 ＋그，0            /


                           C)         孑I =.5十J'· 7




  쇼
  甘恥= 4汪作 侄J444
    J
                            m＜肛成 尸J'XC屯乙

                                                                                                                          . 5t/.9
                          出次寸* 1 .·                    兀= :9D             /

                                                       b1 = . 96                         /RL 4拿二 :            XL= 寸y                    I
                                                                      /
                                                                                                              b2 = 二9石              /


                          '0 3 L '/ .乙-j'.3
                          ／扇M乂e                   //7'工 C小亡石／




    ＄小m立斗耳肖季崔冬建土茗客名dna;
                                                                                                                          /.6 二J'. 3
                          꾸力繇-t i '.                   b, 二 . 38




＼h
                                                                                                         }=m 二 小. E 2




  塑
  焦地
                                                       Xt 二 .g0




斗   寸
                                                                                                                                   Y/
                                                                      /                                  1/   4느



                                                                                                        ；乂z = 卞． g口            I

                          （乂小工 小洸杭
                                                              m 1 7乙 乙／(                                             工口
                                                                                                                          ／




                                                                                  g3



r
}41 寸
    1d
                                                  b8
                   n口
                   小目
                    g
                                                  g
                                                  8
                                                  g目
                                       나.4PEDAt4CE OR 二DMITTtNCE CO아겪기NATES
                                                                                                Srn 1了y CHMr
                                                                                                nJf: Polo..




                                                  茗三
                                                                                                 乙1; : 1二 }
                                                                                                (：
    卜
                                                                                                     b   毛
                                                                                                             八
                   ！
    已j巖馨麟蠶繫쏘
           小
                                                                                                                                     ＼／匕對簪難繫轟多丹
                                                                                                                                     汁
                       三
               立
                                                                                m
                           1
                               d
                                                                                                         m   4亡
                                                                                                                 V


                                                                                                                     月




                                                                                                                                 m
흩
                                                               m
                                                                                                                                     m
                                                                                                                         =
                                                                                                                                 1
                                                                                                                                 !
                                                                                                                             m
                                   뇨
                                                                   1
!
                                                  *4*D나H= 戈A土上D P1工4=t1EJ5

                                                  .   14   J           1J   L   1)Hm 1工니＝ ＝叫＝




                                                               H
                                       和缸加1 心a比 I                        七가;j .N           /


               b)
                                                                    7亡   兀       r   B
                                                                             二   1   乙
                                                                                 三




           白3         (a叫胤끄 M烏k)
            干乙L<y>K r6. 7入
                     군 = ／加이aD玎（伽亡口乙9 ' +(/6이
                                             '］加 C" = ./. 6士 2.C 7
                                      二口O 小／Co

           나낭／         亡i = t'. 。27
                                            才2 = -/ 07

           T뇨W 和1.,. (6.／이 光友且 肛띠나C 4祉 肛元；i4.
                     네 = '솖 魂니－' 白 = . 그／3 入
                      亡／교 = 솖 (7r+ 的뇨）= · 37C 入

          F八.0거勺 (6. 8功 力亢t 批奴yZh似／
                                   4- 口才X呱꼬 方名k＋石帥                                   丸，
                                                                                      ;4
          4k        B': 心亡그Z.mU伍『己亡）
                        乙［尺｝ + (.x냐乙U口
           -4y/     B1 =.0I33           ) BZ= 小． 0/ 39
          丁卜蜘 I油小 化 ' /／民） 比뇨
 1                            午毓．回乂枷也／                             戶力그十 丑砦才／나
＞
니J
 고        （刀Le/
 14n7en
                     山 : 퓨 z_..1_I(8'ZD = . 3 13人             /   (>/2 六n1;E工， To 6百7-上＞口）

                     了2三쿠 友，
                           ；乂B, 毛） :             . / i 1g 入




                                        g ，三1
6. /7/     戶的 4人d, mb小甘 戶才4-征』) 加比 B/ /82
                                                                     I／   小

P九幷伍，, 乙. 艮           加洸t         (G.I/b)

             /，二 弁 公'示, : ' "
             小＝ 슈 Z3;' 命, = · 37了入

 (r뇨上 力yA+ m                           入／y 小乞 Cl- 石才）．批mM
才／ p 甲M毗品／ m＋ 끄笏才缸）

            口，,，《i／孔 C系4J ，知毛友：沚）
         rk工 如hm丑少a 石M 小尸小M乙 厘 弘 “· II口고2
 rC)     ,a;ai,4工七才 比A丑 ／勺'兀 帥2/e, ,｛凡肥 m亡｛才 小切丁七
小小 和小 光工工 小7 교뇨 中／舡 戶叱tr 1
d乂；名m枇4- ..
                        </ / :.1? 十 ('. S- .355) = . 3了5入   /

              <＞乞.      (/ 2 = .3/ + 乙드．35-5) 二 .I71了드＼     /

 1뇨 샤枇才m皿 M和. 4쌈 1뇨 小局뇨弓 M兀                                     出－        e寸，   )


                       2 5I = 小그． /

                        %   2. 二 그 ·   /



T卜小 才小兀              伊h- 口1加比／ -4名；+               兀芎娩-4-
                     ,，끈／二，32-, 교三 二 .C?入
                     -e2 = .23+./S = . 93入         /




（丁k之 小二i不 而J戶q m4 仰力／:tl小 小
q瓦 力（正 7勻Z乙W니孕 尸尹9


                                           8 乙
                    iMPEDANCE OR ADMIT
                                       TA11CE COORDINATES   5,, , 1H CHA仄＼
                                                            F/7r乙   ( { , ._5戶




                                                                                               瑟箸努
                                                                                             嚥籌夕
寸4j414jJ甘44迂r4往t1
                                                                                 月 (
                                                                                       律
                                                                                 1     n 1




                                                                                     q




                             9 7
              比
              n1
                                          『 兀秀嵐4 7和 刃JL才小m旅7
                   H
                                      丁뇨 小／

                   m m
                       m
                                        山比        入／4       石呵 1- 刃／兀彪q 光／뇨M 尤匕兀

                                      兀영才仙：
                                                  Ji 二 . 07十 . zc 二 .3그          /\


                                                   /l   二 . .q3 尸· zs- = . 1g入


                           7
                                                        同
              '.
                               弓＝化Jt                           근L. = 긋吼）十j1a) 皿


                                        ] tH尸뇨乂 十＝1今
                                       之：m\




                   兀 如六及 j系在 小小 m                                       -44仰才 戶.-.:i 2, M            / 七
                   乂系.0才               근石八 = 근＜> ＝化LJ}, :

                                                                  "／口' )十'I" 근， 亡
                                            Z 4. = '/0 = Z/ （긋D0幻                         ; 柳仙工 亡 二 苡；小／
                                                             Z1 十／（그00+J'／匕口) 亡

                                         (Ljoa1 -9, c0口 亡) i7 曷0力口 亡 二 ;2002/ 十J' 口0口 十 2, Z ) Z I

                                （ aM人＜i4Mmd4/ P＜乙t兄三 <244戶亡4- 2瓦7/ /4小4石小t+
              44小- 4七m4 ，九氾小／ 凡띠口
                U     (r              0    (7 r      1              戶／

              7승1 尤石丑 冗'V寸／小杯小伽＋/ 2, m／亡 :                                            印    勻 J戶.4기
                                                                                          刃；

                               Re :           qo 2/ 尸 '5二0口口亡 =20口 근／      方      근／ = -.252스

                               y,m :           了口口口亡 二 근／(／口o-I- 2，亡)

                                               g口：)D亡 =      25亡 (/ oo-2c寸a)

                                               亡 二 立｝/ /e孑 = !q/ D          （如q竹口r              극＞D7       /



} L11+ 11t1
r
戶
                               丁下J力＼/          多J 二 7뇨；' G9.／力＝ m76. 3 ' i     J0ic ＞夕 ,/= . 교2S入

                   丁k乞 cL八小七危仰危三 a4M知侃毗乙 -i乞 )
                                                                                          ,//
                                                 근 1 = -2 5_ 乙y. /D) ：二 /0乙5-工

                   ( ,-.口才M{ 石 H 싸比砒出口 的，水口仙出d 石，


                                                                 2 g
                          6. 8
                                  ／玩cm
                                 (3. 1? ) 才玖工 小艸
                                                 匈吐 9Z 仄 也d
                                                            仰也／
                         Z伊겅 兀K丑 ／危』

                                    근人A 二 2t>       근乙 寸 근C 抗m y/
                                                                           ;    Y/ = d勺 "P乂
                                                    근O + ZL 乙m不 Xi
                         F口＞ 근（；的 仰.c.), 元4工
                                             力的M兮力乙                             石甲d my沆M亡之
                         乂4 J
                                     多h = 瓦M y-t :
                                              亡뇨石叱／+/'2뇨肛
                                             I, './ 乞M d
                                                         也寸／
                     T뇨 力m如且구／
                                        ／뇨尸1./ 넣끄4兀伊石
                                                          如／ a뇨.
                      bq 二 易규／(1끄hm ' 姃)
                           / + Z뇨不 ' ki
                                         也却J                          妨色才＝느；亡皇亡q
                                                                      r｛뇨；
                                                                         , 們．乂)   .    "
                     4M皿 和4／石m机M 戶
                                                         似序皿 74七 p 石나
                                                                                      2机 石교4
                     HZM可 7뇨 P/＝刃2,
                                                         冽七 ／伊4（才 t1 名／e
                                     r
                                                              C4＜孑 名
                     lc／及 仁 光力比 石斗 如．
                                              石 石／ 戶i “刃뇨 十乙 元4／니
                                                                   勿兀
                      4 厄 4-，仍교／
                                    . 口乙岫乙 平，乏 a뇨 4似
                                                     JL , ,dr小， 七 加刀e.
                           Za4V/l k乂 스二 'M只
                                              / 2瓦 肛二，口才乙 으 ' 物 .
                    丁卜4h\ /
                                 卜＼. . 스亡 =An戶 口／/ ' 7
                                                                     -I
                                          / + 可1.亡分             스 十 （乂촌굿1- /스


                    丁.     /       七
                                   『m勺／         b ／人L m小 가V나4tqM3丑

m4二身1d4크j= J41t 1
                    '4 + K났2/乙 '         m老人 “: 4小M스2( 刀二
                                                          / :

                    寸" ", ‘"「兀）玄 『
                                   ：少                                柶가多．
                                                                        ）穿：
                                                                          『

                                                          g9
                                                 弓 十    구O< 三／    k닛 1 6 = 乙）
                                                 '       4         LiZ !


                              44m疋火日        4 二P女- 7r／그 . 小叱 JA伽e
                                             J ' P（乂 ' ＋戶 '1兀J似 ' ＋戶 '）印孚 =C
                              .4白
                                        /    二 兀（乂" 十P ' 7士／兀' 0 '＋하) ' 尸戶' 尸臼工伊2)
                                                             26 ( 2- 32.)

                                               , ！二 三즈H十
                                            二 고：
                                                                   =          주
                                                                              少
                                                                                           g      （뇨枷八丑 民느＜하）
                                                 2戶      갹仄系'
                                                                                  ＋
                                                                                                  （加叱노 牛弘／)
                              T下k,               A二3i ，万／2 삭 酉뜸 = D</
                                                                   +f/
                               TkL 小兀步 고比 7
                                                                              Z;k;,        ,4三，
                                                                                              /




                                            b빻 二 三二 二 三二                               士 ;z        :-4杯之-e /＝入／勻)
                                                       二／/ 六乂i'    그X工                C乂 入


                               Ec'-'-       o<    / 才나꺄七／入， b짰                三三1 = 土二口口
                                                                              1       口/

                              (Tk4 （征未-4- 加莞乂 加孑 m丑JA尤텨 甲74倂， e)

                                                                                                           沅／七
                               1卜t ／比小元左싸兀 7 4 4九甘四m兄7 丑n工 小뇨
                              d뇨4X 如毛 弔 才／丑 而 （ 和比M「， 4亡 x二麻：工교口C.
L
니




   LCaHqn置




J11i1]i4iaa4니m느二亡뇨느h七＼嘉 幻 音
                                                                         q0
                     6. 9                 Sm / r ／了        CR1｝尺1        S乙乙口1JO八／

                                 /. PL口1           恥＝I. y勺 ' 1.                        ( 자끄r亡 1 T1-入NCe
                                                                                                            C H 月 e丁）
                            2.
                                 .
                                       Pt-口r      R口丁月-rED          ／十a小         C/ gCLE


                            3.          AD p      A S丁，)5    5USOE4'刀3NC- 三                  0戶 尸i- I          To      'z.     TO
                                       i'i0iiE     r0   goTATEP     i十3b                   CLP.CLk.
                                 Li.     r닉口VE        入／8     丁＜, wM-D$          &-EJ드R升TO尺 )             丁O        t+j "b    C u乙C乙E
                                 S.
                                  .      MP  ／午   5丁＼)13
                                                                                       乃사cE       c. F     tj '／· 口
                                        To  CE}JTER     o 1그                                                                 TO ／切口yE
                                                                         CFART

                                 6        丁卜＋fE           oPEl'-)戶 C／尺CULlED
                                                                                          S丁U6     匕EN口n}5              人尺EJ
                                                  毛 二 1 Lj           入      ./
                                                  乂工 二 . I '／入             /

                                                      /     小-I.乞    口石在니               /J= . qg7入 , !l二
                                                                                                         · ／63A)
                    YL- 고i4qm土比
                                和m无人；
                                    多 4才二名b니 /m十，
                                                      긋／二 . 3긋6八
                                                                                   /

                                                      /{     二 . 口53 入             /
                   Th工 ／倆才友                       C-凡니才 小                 完乂工 戶才 和在老司
                                                                                     ' 成
                   고＼石3</7t,            ＜力t, 才危
                                                             戶-e白勺 尸多
                                                                                            乙,




令士44卄b吐m立算J



           44q4나
                                 MPEOtNCE OR ADMITTANCE COORDINATES
                                                      I               。TArEt)
            S.벼, r1J CHA只T
                           (19
            Qf PR乙nLE1n




                                                                                                 4너＝ 二n比卜枉느卜1仄枉


                                                                                               弊求
                                                                                              仁n  芝a녜1僭먀
                                                                                               n
                                                                                               r




                                                                                                                  1




                                      7 」·，·＝써ry쓰스．仁丁，.,                .       H卜如小m 노？發
                                                                                     t ;‘七i!l 必．多：/..
                                                                                  : 『．
                                                                                         ': ' . '등多多"

 y
!HH <Hqi=
                                                                                                    多／
                                                                                                i
                                              O
                                                      叭
                                                      n
                                                  /
                        石，/d                 口小今尤. 4亡亡成늑
                                         2f = 2늪M P口
                                                   （二 z乞- /350 = m/ 口
                        F加如 (6 ' 그 " ) /；呱J 7乙뇨y /Z瓦＋ 小似
                                                         乎名md兀 乂；
                                                                                                          I

                            b. : 中bL 十 ／工 /me）兄＋“亡 '                                        = 中3. ?그 . d,, 二？．口了
                                              亡                                                      '



                       F加艸 (6.2. 3) 力 （力 石上（d,
                                             ，규 戶老比， 石H4伊磊m七石 屈，
                            b2= dm刈乳－乳'亡 ' 十品 = -1, 6乞
                                                                                                   皿 _3. q百        /
                                   9L 亡
                       F 14,., r 6. 2Ljb) 光& i.
                                                                   S.C.       才m 丑甘才凡4-
                           /i       = .DyA J       d2/           . 亡） 7 / A    ,
                          乂 l ＝· 口了7入 )                 <)4/ . 口4'了；入         ．

                                                             d
                                         I                          갸
                                                   4H
                                                                        1


                                                                   尸
                                -
                                                                                    足1 六／' Xi.

                                               F
                                                         '
                                                             "
                                               1근2


                                     Z 1 = 尺L + j ' (Xi- 十xt)
                                     小注,       尸‘ +i (X
                                                      【／X，十已亡） : 2.
                                               乙 +j 亡（足乙 十7' h 勺'Xi)
                 石b뇨3 和                    （ 尸뇨』
                                           足
                                      「‘"“弓 實： m尸窈
441斗t汗｛ 斗斗444J
                                                 ，片叫
1
                 -4-
                           刀K'         力：4加＜才                    뇨十已．

                                                   C) 드尺, 드2, 立쏘 1프卞
                                                                              又亡工
                                                                                       夙卞乂




                                                                    93
1卜二    尸才 比石 ／꼬44ib枇刃 万4- 元人蜘 )
                 X , :-XL + 石士／(I＋亡3) 展2. -尺7- 亡 "
                                                          t
丁卜皿 石丑（打a ／上，+                         ／꼬a力才am乂i, ／뇨 J
                                              【 z。
                 X2. = 土근.寸귿口尸（(／十t z)．疋L‘亡工 ＋尸
                               夙亡

丁h工 呼小 h                   4札寸 口屈4力／ 片才k+ 石砦老／나 m工


                                  乙亡          =   希 z 4:' (흣）
                                        1   - _i_.
                                       {5 C 戶 27r
                                                               L _, ' -
                                                              L久，f八" - Z'      )
(Od2                z肛三丁 乂h尼 小；i亥 Cm寸
o)   s加m工            .5／加尸T뇨 c,gCv ,rEp                   SHUNT            Sru8 :

                                                                                    200_n.

口才 品 ) ＜乂1= d5Z入                 ,/          比 =.39了入                 /

                 b1 二 尸· 7                   뇨＝ 十· 7

            J1 =.1S3 入 /                     긋2. 二 .3모7入 /

       '   111      =0                        I rI 二 0


                   -U,之，     -Vt七nar/ 뇨4,七-J


                   d1 : .R7六             /        ＜긋 2= . 3 93 ,\

                   乂1 = ．比gA             /        乂工 = . 39zA

                    b1 = 戶· 5'                      b工＝        t.   1 (>

                   1rJ = . 加5-                       II니『 ·3j                  /




                                              C'9
                  b)     SIt)'LE       S- oRT_ c{ gcuITED        SERL&S       5TUb ;




                                                                                              a0C)U｝寸




                                                                          /




                 c) POUBLE             5HoRr- C (RCO1TED         SUU卜JT       STUBS :        C-丘J乂＝入府）

               a.才 兵.          向＝./y
                                                                               七m
                                                비＝ig了
                                                                                    da
                               山 二그7그入 /        꼬／=.92/ a /

                               土，1= 二 73                                                           '    "
                                                                     /’
                                                 b'工 二 工7了
                                                                                         夕
                                                                                               "
I                        ,     Ji 二．/3-入 /       /{    =.9yy A /

                               IrL=o             lr 'l= D
               a-才 /. / 子：t>    小疋寸    M亡iJr      뇨口才七／

                                ;! 二． 加入 ,/           町 二．今／'3入
    :1和


    L11                          니 = · 33             b{ -; q, z
                                 戈L二．j ' 5-入          -t2 = .i92A
                                 i72' 二 小． 57         b‘工 = 1늬
                                 ;ri = .2oS           lr 'I = . ?Y
                                                '/
              ／늠力뇨 ／노；   才 /．白J, 加付Ic ／虎LI 9규
                                                  乙 ,．弓之 丁I占m可／a庇／\.
    t寸4녀m니J
                                              必｛
              冗和八勤7 b; ' 力"，出 M晳乂e
                                     쿄刀IA.仄 月兀iP二
                                                    Z= /ioD(35o) 二 /g7- /人
                                                                                         /
                                                                                    1/
스S各及。卜小伉 石 吼 甲小 q渺，놔
    戶.
                                  nH 二 卑므 = ．兀

                  小如乙岫L力石
丁山加 和小 (6. 33) 才뇨
                                                             a7l寸7




             芒：)．紊蜘-I Y，   ｝了
                       느: 于：
                      = 7／弓乙

m /C尺05 flR //;   口 ';YOL) 7小 :                1甘



 Cr =Z. 21 十 .15qc,,4, f= '/ CrJ45

 F小4才 名7 叫H <2 :

  7ee,i_ W10O 7       A, O = 乙2/ 3           m/1。。/ G 二． 87百 < 4. /, Y4., L/ 92 q卄

                      Ag7 二 吼Ct I              , 7/d
                                             ＼凡／                 < 2 /,   니I,   = , 口긋2m
表y1 叭／1! 7 /

                                           叫r 7        小；.        6己 二 /. 6弓 .
 F力mW （吼乙口y) ,                Ee     7뇨

 fk小 乂石山 P.兀艸m/ 兀弘 伊／뇨 入거 光往什師仰
                        入                                    V
             /
      )
                  =
                       Lj
                            ＝君，了『 /.y百了 m,




                                        96
                    千e小 A/4 -尸夕
          52) 人．,
                                          8<D 勺" /OJ之




    1뇨 ／人MX ／力山卜
                                  和m牙 口m/
                                                        才A工 小d們勺
    P毗人才 弔 尤反兀 石a/                4a加肛b妃毛 :
                       y乙 = (i. oo 寸J" . 50) Xio口
                                                    S
    aD/     65r叱= +j ,005            S
 （久A긔／小M丑       才뇨 山m也q力
                        d a뇨斗m口
 ／危小 ／뇨                         9刃 ／茨兀
                    知J1- .    Y뇨仰 尤A刃 似
                                        如冶斗 뇨牙尤友
                                                                 ／뇨)
                      YSTuB = j   y. 九平J
                      戶丈 " 亡- -:'    口兀口cS) = /q "
      \

                      乂 = .03모 人

 T瓦小口 力뇨 小們
               mM .                  們才 石           光人e ／勺／戶 7
 力뇨 .4乂乙／尸 ／뇨)



石     光A오 戶M乙 나啣七 兀
                                             까h小           C.凡M石也d名든
，乂加尸枷M乂*             小出-4才 力七／

                       귿 = J5아Jo乙） 二 ；口. 7H
                                            n中 ．
                 ,.15
                                                               근L. 二 372_n-      a 二 2. Z86 c-i.人
                   TEO 八／\／싸尹



                        毛： 귿뜯f = 그O兄y - 니

                 ＋人 才｛W       而了出니／ 升；乂尸 )
t＋出戶n년
                             弘 사毛卜am) ' = 万了· 口                                                       /


                                                               (z0?,q)／즈77) =   99 9. 石 Jt            /

                              2
                              '   『        帑｝              :
                                                                  IS18-

                               뇨 ‘ ／뇨／比力白如
                 4r 比뇨 mm左／따今 肛；
                             2M= 1乙及 『 /r997.6j仁77) 「 939'0JL


                                                PM               戶m
                  右      m
                                                拓‘ Crt4- 4 甲 ／石工 M짜妙
                                                辰                                 小
                                                                                  小
                                                加
                                                    1/




                                                = 毛吼 - (a口1. O3n) 二 /8/. ?                   /?p1戶／

                                                  云；
                                                   ;; '    i39

                                                二 VEr呱三可刃a)L

1낄；4
   11
    d쩍           a小石7 7g乙 타 :
                             6, : 可十伍ZD二2孔）' ,- /./g5                                          /




d쿄捷注＼專 1 j i J
                                                                ( 2亡）9. ') 1-


                 丁hL 小們m/ 石砦肱 꾸 力뇨 加戊劤뇨可 4m                                                           -/)

                             ＋午＝于 ‘示："."“느 '
                 (）倂i 乂万m女 乂祈4 存尸 甲 m江mL今 在 如才

                 呻秘／e        우        及＞             근之）
                                                               1                                           }
 I
     '.
          "
                       5缸
                 (=
                                  2,
                                                    .   7」
                                                                            2뇨              ,
                                                                                                      2누          乙＝
                                                                                                                            /&JL
                                                                                                                                                     1 tj e L J

          乙／Zz        ／뇨 m口才 -入 丁났也 6.1, ，쿠
                                            才 汁V七 a硫Z/ 小4七 ／石. 5了）:
      m'C: 且督 = i9d了兀읖                                                                      二
                                                                                                  小． /eo,54
                                                                                                                                                9三 ;.2
                                                                                                                   =＝今               귿／
                                                                                                                                            =             r.


     'i =1    : 乙爭 = 규“' Cy兀蚩 = =y.2j'                                                                                 =)                 귿2 =30. ZqJ-L


                            乙已
 .14= z:              王人         = c_ 'C？人 釜 = -.
                                                                                                      6035q       斗                  Z3 二 /6. 5q mf,乙

                      上
／乍＼= 3 :                   和瓦          寸y1中.5
                                       H
                                          / y 且 八）夕                             =   H H4. 今／亡）乙3',
                                                                      6;D
                                                                                 ;                                今                 귿g =11, 口1 m ‘,



*             小比 小施們乙志 衣名肛叭
                                                                                                           근1.//2口 = 5'            a,./         己Y／눌，=3戶 /：人
T汕Ze 6d , 加e 0似뇨d
                  已= qs. o7j5. 玉：弘아凸
                                                                                                                                                 근3-／石，9只兀，
Z9司／·b7.jt. （乎뇨 而左m/m碧Ay
                           m化ea444 石끄力／
小肛）, Tk恥上 /iZ44L左
                     d4工 C乙넣兀 크g 才뇨 큐ky
戶才 平 1恥교危, 0仁                                                                                                                                    7
              加뇨／／切.,& (6. 5了）.
                                                                                F

于；mt                  (6·55) ．尤仄e /aM二刃奴彬 石-
                                             )

                                 A ，丁六／}ZL小毛］ 二 . 09/7
                                  管                          i 근4-十근1
                                                                                     1




                                           =   艮＋
                                                               kjr-
                                                                                     12身）
                                                                                                I--          YJ
                                           =7o7                             /
Tk오 고mm／小才 4駐；勿됴 勿甲뇨나仰小的
厄 e小洗／ m4, 7勻싸呼 兀侖 :

    0. 6




                                1 .0         l .5   2   0
           0   0   0 .5
                          FREQUENCY    0Hz




丁k白 ／小小』
       ／士 .4流耐 9, 品小小社祈 甲 m寸

    管 /'3'/ ' 68 (mg =6少男
小毗小 厄 -4岫汕弓 恤 力 加 肛如나
Ca且AA쇼力j 力／44'Zf 吐 .7아乙 ,




                          /00
                              므기                          . (1   尸H               寸寸 日 닉 4

                                          乙＝
                                                      1
                                                                 2」 . 스 打＝／万  1



                               F加H 配·／.), ／뇨 而沚 小們才
                                                                                                        Y命品1 切伊二J
                              끄包和H人毛           /{4尸
                                                             (A) ＝기 ".
                                                                                  [(6)   = 긋 月 (/ 十匕d+ 그夕）

                              Fm加亢뇨 小此 的：七
                                                                                              져尺 M工 X/m/ rm) = 듣二，
                                                                                                                ;: 」·乙
                              __4-d_   A= .2/ L/ =.o5.

                              m        加比 m五m／乞 -拖 싸
                                                     J 斗俎烏乂                                                                           白伊4 7L
                             甲元杭Q. 。Lr                                才 夕山느 가BCD ,w娩兀氾 丸仍／
                             Cdm나d入 石                            5 -/aM仙脆W:
                                   I斗 87 : 뇨d 口 ，」毛枷口卄鈿
                                   L （二 pi                                                              了근2M이
                                                      _力 石沚                   乙寸-Q 夕 J1jY. 七；,6         " 匕dd 尸 1


                                                      "耐까乙乂44切                                K카和旭砧片夕 八
                                                      JC'i, +v:24辰口勿＜夕                         C加 '口y, 2：小q ' 巴
                             2在步 丁M在 百， 그 石                                              蜘d力             드肛m瓦十小冗
                             比h工 싸J斗伽乞                                                 ‘ 呼尹辰石J 44,
                              ［그引 = 5 ,1 +                  SI 工 S工i 口
                                                           1 / S之之 I二（
                                                                                                        1-v＝ 쯔브
                                                                                                         Y1         R+ ,
                                       = A +B크？크）                                 H口／S그
                                                      S
                                                                 너卜
                                                                                                              (S=
                                                                          r       H 4 +B -+C 山 Z) 尸．
                                                                                                                           片十乃十C十刀）
                                                                      /                           1i二
                                                                                        S
                                                                                   "     r1




U뵤H蚤蚣菖往硅j藿立j王汪量ii卜i
                                       쓰 I月＋B-C刊［5口C-A +B七m] 十乳j
                                                s [S - rt（小A+ b,C＋끼

                             丁九江 的如 小寸／




                   di置g布逋葬
                                        巴 J們4途／力 ：加『的2万）,
                                                          M夕如／
                             十 근1m 군니 /d 7訊元 4
                                               仄 쓰스孚 丑笞碌力如而乙，
          如加小 m                    加記／ 戶뇨才 如m兀 石尤乂／伊如m
          a才 9 二9DG :
                  r (9D") = o          7
                                                  如杖 fA 이 : 二2沚                        O a
                                                            L乙Ui    ,   0            H Yi?:工］

          石    r (9) ／啞／仙如 名 X征 戶Z雨幻 好q辰；亡b닉 :
               C-乙Y2 ＋出Z9[-（乂豌＋근，yl) . 됴（근，Yr乂근D] 十9G =D

                   （首 y二'>1,' 갚入 r：오 ( 首 片＋X ' Z: + D :O
                   （펌 中 근n tm ［노（컴 十 근을 +1근注n 二 0
                       （근｝ 戶근-t) 十 [i （캅＋근力 =O

                              -, = 首 ！브즈 二 근｝ R
                                                  1寸-Q
                 (y匕

                          I
                              7:
                                   =       7」
                                                仄］ / /         （戶7=
                                                                            \
                                                                                I)
          m私玩 J們3뇨； A4 蜘小 右戶q, k小 4丑／
                                                            Z/m才 丑上 力가b伽

                                   뷰            -- e근乙 /     k／근： 尸／
                                                  R＋근2,      R／근2. 구／


                                                    c-i-.   Z1 =/   가


              卄 R= L57 ／不끄七 入必比魂 d亡＜娩k毛 /1L二戶，.』
                        乙＝ 乙／S）抑 : /UD67
                                   근z二 ／나口C가后 二 /.3S5'/ , /

          U八示人 沙兀 ／仄无仄 1나／兀 6·／.




1a1川mHd
                                「小                  （口』Ss): 尤凡／뇨比石2M/
                                                                                                    ，尻M고，
                                                                                                        白乙之石 됴
                쯔n
 1


     十 4
           d             “乙旱卜 'm孕）勻 , 加浣It                                                戶         그   사
                                                                                                            注
                                                                                                            匹1
                                                                                                                  구    r
                                                                                                                       1
                                                                                                                      프毛
                                                                                                                        11
                                                                                                                         111
                                                                                                                           J



                                            小／
귿                                                                        /
                                               =/
                                                                    入／
                                                                                                   人／= 今／
 1. 5
                                                     ;2,c 1 .D5tX> 그00 1二；= ；石0
                                    1 /0C) 0
 2. 0                                 /"7
                                                      二乂 } 竺？ 1 U? 卜0Z0 ' 137
                                    .
 3. O                               . 2s口0
 q. o                               . 30：口           ;;    I1 1' 1 1꾄   1         万／ 卜03/j               117
                                                     1나            50C7      1   7 '   1 1尸＼그7 ＜戶        , 1 』，
 Lo                                 ,3333            3?    1 .(667           1   71/
 C. O                                3 5 7/
                                                     3乙'   IJ. us
                                                               {786 Ij 7/
                                                                       -t              1:
                                                                                       ;:;;;2
                                                                                          ;''           I (-1k,
T卜Jd』 凡ia                                                M恁／                     ／凡 刃y攻 ，在弓兀＝




               八岑나
                         伽

                         切

               口
               甘＼告
                                        d




                         助

                         的


                     1   1/




                         和
                         D
                                    1
                                    丁 0
                              1/n
                                                    교口       3乙                  g二            :
                                                                                                            6.乙
                                                                                          -f
                                                                  크／2r




                                                                  兀
                           （二d山 弓7
匕. / 9         又 江 4e乙 夕7거

          1；仁） 二 7   二   石比乙 石노， C力＋ 夕

                                     万2 -/
力＼二；l :   丁교7C) = 그7느／ 二 그石尼4切）), ＜分／

               = 그 厘』et ' 夕，吐 ／古 구 士 白口 2刃 //

               二 4Z亡 ' 夕知 (/ ＋口d2夕．) 尸／


가＼二3 :    T3像）二 171寸臼／ = 4I, ,t尤3夕거‘Ci} t9中3 4L七 夕뇨 （兌川，尸

               = 汕e乙3P枷 (3乙b寸 夕 ＋乙的3夕戶3月叱 凡蜘夕            r6·及七) V

가＼=q:     T仕 仁） 二 gXy小 S又놔 /
                                    四4 d4m’ 夕 十／
               二 r4꼬Cy汐枷 乙dY夕 尸 g4JC！

               = 山e兀Y夕M (3十V dbd 그尸＋口d, 9刃 尸 9뇨r叭 口＋白 2勿 / /
                                                    （匕. 石n/ ) /
                                                                  \




                               ／乙）'1
                                             瓦=
                                f二4刃H\ /6 . 4/ ).
                                                      /．
                                                           』   -
                                                                        1rm: 5. 1'
                                                                              i:
                                                                                   ,   1,   ,    .       091   :   A

                                    r ( 6) : 교 d jL1b [ n m9日 十／二 m
                                                                              2尸 心 rj
                                           = Ac寸& T4 ( dJ兀日州 C力4日
                                                                 ）
                                           : A e"Jq6 [d乙y夕,, (c杉 1/夕
                                                                     尹y            d，寸고o 十3) - 94'd’夕什 (C小교口
                                                                                                             ／I)                +j]
                               F月七m\ (G . 6 3) )

                                                  dZ乙 日m = 幽나［方 口小Y히 느抑］
                                                            : c4小｛4m左／缶7准찌）] : ／·）69
                               쿄寸      9蜘 = C亡g1 (I/I. 口64/) = _0C

                                                   C七夕4 Y9 -Z뇨Md, ‘.

                                                       긋 r; = 只 4J4Y夙，
                                                                     I =)               r; 二 . 口了g3                    二 rq
                                                  C寸口，2多 나去b心． :

                                                     a r = A (q4JCy;，꺼 中枷恥눙
                                                                            司 二＞                                   {; = 0그7코
 l
 ｛                                                                                                                             f3
                              톤方蜘或씸 幻y4i瓦才 丙似：




   三三多4重重箋唾ij걔寡
                                                     r그＝ A 作4尼寸日，Hi m1'
                                                                     7戶-e乙' 夕H 寸／) =                               .O긋gg
                             I뇨＋, 亢뇨 나m44乂Zi工d力石
                                                 ／뉴戶i고                                          - 砒4- 'Z'z兀，
                                                    근t = 죠 旦 三
                                                               二 /7/ 7. 9JmJlm                       /
                                                           ／나；

                                                    근三 = Zi 브 !
                                                                           42 y石 qn寸             I
                                                           卜／;
                             寸／工寸   (:4休，   H在工；
                                                            加           仄仍m찡 -7易乙 근3 - ( 근y J7




瑟m奢醬豪U笛毒曹器
                  ，거冗心2太小-
                                       o    和k             只A오     tA    才"
                                       j
=
                                                                    릭         4        語                   3
                                                                                                           5               ／
                                                                                                                           口
                                                                                                                           U
                                                                                                                           2                 皿   /



                                              =                    군3 = 근44 느旦                             50. 5t .i-
                                                                            ／十／;
                                                                                                                                                 됴
                                          F沆m, , (6.6 q), ‘尤古4                         4t2bl N. tth

                                                               管 n孕＝工 帑기56只
                                          T厄 m쇼m力／ 싸d 乃I彷뇨 야尹枷d 加伊丙Xe
                                          4       小w孔 灰／枷乙 他· 74伊如뇨씽·


                                                                                                                                                                                      /
                                           C, . 20         \

                                                                                                                                                                                      r
                                                                                                                                                                                  /
                                                                                                                                                                            1
                                                                                                                                                                              /
                                                                                                                                                                           1
                                           0. 1 巴 mH                                                                                                                      !
                                                                                                                                                                           1
                                                                                                                                                                          1
                                                                                                                                                     1                    7
                                                               1
                                                                                                                                                                         /

                                           0. 10                                                                       八
                                                                                                           1
                                                                                                                                 \
                                                                                                               /
                                                                                           /
                                                                                                                                     1
                                                                                                                                         \
4J川카汁d斗da打重＄兼 i 喜 黨 忿 斗 卞 譜 忿 迂 m t 注 多
                                                                                               /
                                           0. 0巧
                                                                                                   /
                                                                                                       1
                                                                                         L
                                                                                         1V
                                                                                                                                                         1
                                                                                                                                                             \
                                                                                                                                                                 1
                                                                                                                                                                     1
                                              U
                                              m   nU   0

                                                                        ·：'
                                                                              .   !5                               l   1   1：·




                                                                                        F 示드口U匠卜小二 r"




                                           丁뇨／加山웠崗 平 X和 Cmm向m丹如－兀 小才

                                              管＝ /'" Y' " : /夕570 , m뇨智md小氓比此．

                                                                                                           ／口乙
                                               亡 9/
                         'e '2 27r工           y刃竹 ＞伊까-7 覃7竹7?/                                     丁＝끼J;
                                          /    " Z 늬y드 ' i = 닐／겅 = Z근
                                                                      08 Z 'Z 느戶
  /    끈 ／石ci 'I = ／긍       中    6끄万9,
                                     ,         니             -5了夕方；묘C,. = iZ
                                o= gZ5Z '方＋ 忙0$r9 ' 卞2／근口万／'I尸




                                                                                                               各甘旨貫晷뚜슥A多g旨gF量h朴kk丘犀H妊斗互芍藿나艮g菖K彗
                                                                                                                                               L노
                                                        '5 '／二才 /Z ·＝ 可j                'so· =1스J     10크
        a: (i_ rj)(i j) 小凹十J兀기끄＋ (I＋乙)(!
                                           ．쓰.1入'Z
 人2큐r外七G8在次川小針，         '근섞）. 二（；七訓，I4忙汁亡J +, G沙＋處）낀
                            fG十罔勻 珏m刈（큐-f刃
                         二' Z, frj方＋［臼在加千 '+12)-J (h之町 욘J
                 [（予뷸厄偕嗟거（亭引나
                까丑手剖n＜乎卦作+ 1已 " ('QL)J
                                                   卜’
                 （八 咀）                                       Z／
                                                                  겅
                                                                       ‘   ， 0 ,
                                                        L (7               d/ '귿中
              \a가工        ' ty 二之긍宏       尹7y7小 ＞才따／ 24Y
        如弓／
                 그r9斗m
                                      寸4- 加        나呵Z7                            ' 쁘I 二（刃幻J M了거上
                                                                                                             ：뇨卜恥 n q 1 扮 甘 n 1 1 1 1
2.3：尸弔／（日7J 2刃伊m /7中
                     y 寸                                              / 亡／.9        -4弓？們m, '4,/     亡22
                                      二
                                              쁠         4>    1 =l7    1
       夕. '：씌 十 !               "「 “丙               。：히 :（切切' I- V: (0)그
      口回- 汐구／) ' 夕t河］P／夕y= （口吻 나夕力7乃L夕r:.2Y : （幼나
                                  ' (9口9 '9) ／入勺 (/ 9 '97                             W9七크         /2y ' 9
                                                   ＜尸＜7r
                         丁／9가＝ A (o.／十 Ca4 ' 夕） . 亡）



                                                         A (. 1+ Co.di夕)




                                                                              今




                                                               I; 二 . (99了了




                     古兀及石 m4似硫磁8 品們4M加 口在．
                              Z1- ;?4:I   j.,rO 二 / . 口r了 근口
                                          i- rO
                             Z2 = 근, I土孚 = 1. 2v$ Z, 二 /.363 Z,
                                           /   戶   I,




뇨
11                   C加泌； . 4才 0＝기-I工 , 才凡 石Yk十 ／山f갑在似兀 石肛工
                            I? 辰，
                     才m似和如 加；
                              入叭二          금工           = 프흐可＝ . 九了근 ,，
                                          仔派)               2!

                     k元／山 샤d 쓰／Zk兀'1므弓妨三j 屈，

/1 4 1 1 i m d 1 i
J



                            兀E刃辰切F夕 C小丑 月＝ jl（기72) j二 .M
                                                                              = .O/8.




                                                         /08
                                                                                                  0
                                                                                                               (7/
                                   'r          'a              '1           O
弘 79'                              1
                                                                             1
                                                                                                       O
                                                                                  1111
                                                                                 [
                                                                                 1
                                                                                                      /
                                                                             b 1 1 1 1 1 1
                                                                                                                                +H LL蜘夕누寸 中27 戶깎
                                                                                             C-
                                                                                                           .

                                                                                                                                                 ：勺亡
                             nZ/.Z뇌／K9)J1t                                                                                                    P1丹mV 中可工
                                           /                  1,'-iJz)；二시1를뉘듦＝ t(8)JI
                                   그db 42 ('／刃
                                                                                                                                 rz
                               Q!9 + 仍7) 1丹a t/,JL
        이                          닙h-, (-7／뇨)                                                                                   三
                                                                                                                                                              =
        .1［굶仰 于｛뇨耐叫 H뇨己 V
        "
                                                                    -                                                      Q＝毛
                             g戶 二拉，갸i沙y V, f 루                                                                                        戶
                          口. . .                              g汐                                                           叱g
                          2尸（' Z/2 y) 戶닒i-                                                                                     j 주 ' （口）1
                                                                                                                           1                       r U 9 ' 97
                                                              （꼬／.즈)勺／罕 :V
                                                                                                                               尹 =D
                                                                                                                                                          r/ ／ 才
                                                                                                                                                                       竹
            4,
                     卄7
                 ,            7'       "   Z   "
                                                    (-
                                                         i)
                                                                                                      叩D
                                                                                                                     '7-
                                                              毛         '
                                                                                                                                          "
                                                                                                                                              "'
                                                                                                                           7D " Z             (
                                                                                                                     幻赤？7 八幻근
                                                                            i -7
                                                         君寸냐了 ,q = ( ' Z/Z7 物／
                                                                   丁              슉I
                                                                -4,고？伊 V 二 (
                                                                             ' Z／균 ’丁) 戶
                                                                                                                                                                   C乙 ' 9
                                                  月t心71-              ．石g) ,


                                                  카5) = 근比旴                                                 ／區1 " ＜孑＜L·
                                    =             a- = 工 丑人 르느
                                                             1中
                                                                             乙         . 69j
                                                                                                   L小
                                                                                       中
                             F-1力m\ 化·70),
                                        int夕) f: 2-기                 血H쓰프）1 二 .. 3'/ I뜨．츠n .
                                        '"  "                        큰시 i        나'"
                                                                                 PU    .尸 L I


                             Th人4 mJ才                       人七 F心比／ 小                                            乂衣丑 沙尹尻 m乙小r :

                                        I r(9)j




                                                                                                        \




                                                                                                                                                  仇
                              .10
                                                                                                                                                                    戶／
                                                                                                                  ,
                              1小
                                                                                                                                                         \
                                                                                  \/
                                                                                                                       \\/／小＼
                                                                                                                                                                    ,

斗                                   0
                                        O    I.       2.               4,.   S.        石.                   7.    8.             ':         10.   II.   I구.   )3.




                                                                                                                                                              ／和
                              m             m 그耐 力나 小九 /1二侈小力my /m士

                                    m 小
                                                                                                                                                                         <H=
                                                                                                                                             比C兀 j뇨,,. 力們／三，二
                                                  5
                                              05
                                                  0
                                                           /4        91 =5. 5戶 . 丁0                               0/ib小'




:Ft소i毒出七七뇨y二그二늑亡뇨뇨nq= 2
                                                  M
                                                  b
                                                            ha겨才e/
                                                                      夕 工 中 夕／                                        C그／             e2 二 3易 = 』／百. 三
                                                                                                             /
                                                                     （弓2.十9t)/7-

                                 , ＜乞十
                               丁뇨，                     /；뇨
                                                                       m／瓦                 戶6小兀：
                                                                                                                                ? ,

                                                                      尻＝ 으츨으乙 //：肛                                                    ＝슘）
                                                                                                   I/ o


      j니 Uqnd＝ 녀너내치nd！ 甘늬H
                               二 ．“‘二乙C),,:"乙.         寸：．《 아伊奸名놔놔，
                                               , 6,., ha蝴
                                      ,")j·／mm功，          ／丘                                     I


                                                        管＝ ;－等끄누／ 勿 夕加＝吻．
                               丁kk 如白孕 ( (p. 43) ,
                                                   m 九 " M加寸'／七／졺判］
                                                            /q,y' 帥小［打2. 53 V꾀，
                                   &八／             入／ =          , . 0J     才a-       . /.. 口        -4   .
                               ,          ,        "             m. ,.J)    .4才       .“「＝3     d팎彧亡t4         -心W兀／／亡 力 , n . . . : . /
                               rH 나 a <my咬 럼 3入./,/ a.才 才；뇨 ,．力』
                                                               .七                                                                        '
                               二｝k 庇 如沆' 凡毛 崗m 出二二p名y /
                           ／쇽肛I- 如2乙乞；) m吃，' .                                                                ' "

                           回
                                                                           石· 그2 J     才뇨 凸m，  m/
                                                                                            品竹石；  /g;
                           伊比i 斤d 小a ／三．                                                                                            口m
                                   ｛兀由d回‘졺
                           T뇨 甲石니蜘（ /7比乞‘ 叫拜aJ如于小4
                      4刃尹加A工 a／끄兀／ 4亡 口4, 才航.云八 :
                           }
                                              r

11小；4t나tm出斗＋뵤144 4
                                              1
                                                       Hm




                      r;       L；  二＝
                                              HH
                                                                  1
                                                                   r




               11
                     K4二 m口니． ／乙 ?；二；.
                                                                                  丁
                                   Z:. 귿 드                  'I
                                                   乙VRC
                                                                       Z＝切m加如吐店和口쁘) 二 ' '/17
                     n뎌
                           '            m 三 ·E刃                        수     尸亡 < 3- 6          B.

                                                                                  1
                                                                                  J
                                                                                  J
                                                                              /
                                                                              r
石．그6
                                        'SI 月rc H／刊6-             SOLur,o八) ;
          L 竹 S ECT六口八／


                                             R 二 了OJL
                                             L =5J14H



                                                                                     '三2石           (／刃3／刀E /-j "兀）
a/     +＝그6-H孑 ,                    及＝ g/ 7'13皿 ) 弘 二 ／·',

乙L 小，江玖 md                                 石才在杯' 戶亡＋
                                                                  工六／끄0C7乙疋          WIjH       L= 교口．/ mH
                               J"b = -J' /g ＝多
                                                          足 니) II긱 C = /, 교7尸r
                               j 'z 1 U'/; Z5 ＝수 tAPACIT口

                       伊                                                                        乂 가 呼在a'
Tk工 싸 才 芍／姓亡二乞4 口伊征d 小                                                                                                 7
                       乂枷／才石丑· /aM뇨喊Z古
小協可J a'HU，工 兀f 汕，／上i4凡

戶 丁L                                i



                                                                                                                \
                 '-
                      .    J    -
                                         二' CI石·                                                \


       0. 8




        6
        m




                                                                                                                       \
                                                                                                                           \

                                                        I         I    )     I   1          i   T
         1D. 0
                                                                                       2. 8                  3 1 ·＝.
                 4    h나
                                                                      2. 0
                 二

                                                    FR三口1.炬Nc.I,             0Hz




                                                            /／그
                                          乃口PE -F月 JJc)   乙iriir    :

                                        FAw- F十七 (O．그그4 , 比化
                                                             B쿄亡品M q;
                                                                    ／뇨4 7小

                                                                        小쭈
                                        比小aw缸蚣 兀m;/

                                                          d nJ ==              I
                                                                         7：兀m
                                                                                       -   -,

                                                                                      中4   (    .1   d 人／口




                                                               F2 中-ci -           乙／gX/O je
                                                                    尻          그｝r （그刃o9)


                                        丁h小r       加m叫 十畔 力뇨 批t 如力幻伍싸
                                                                                                             甲
                                        ，无뇨    乙드不奴；亡而        4M辰危古．




3共貫h色計求好d44寸注1




              i쿄Jj！ 훑 占 上 智 4 重 쩍 和 迂
                                                                        '/ 3
                      CHAPTEF.                  7

                      7.
                            '                                 包留


                           F7나nW rM在 7. / 戶.z_                                                    尸在mJ妓Z 砒C- 口八aq光
                                 =              二                                                                                 = /y5 ／刃／/}
                                                         匈in三                      叫 (qo入，戶力아/O小）
                                     프，
                            /D
                                          2刃H




                                              읖
                                                                                                                                                 7.
                            Q 4 0拓Re. 四 27r됴尺c = 27r (/95大，0石)（中00乂30入／口‘/2) = /0
                                 Q
                                 e                                                 =
                                                                                       =
                                                                                           쁘와io?) 二 긋／g.
                                                                                           '(00

                            m
                                           加                                                      如
                                                                              4 ，《i 7 7三小                               (7. 幻）/
                            r

                                                    Q
                                                                  工旽
                                                                                                               =
                                                         L                                  7긋．7
                                                                               工Q
                                                                                                                   +




                                                    41中m 入 H口＋



                                                                                       1
                           2 긋
                                                                                                               ／二入 二 크互              I乞 勻 “ (4-J。
                                                                                                                     n石


                                 士 ha+ 口 切小，亭4石 力如M4m｛丑， V弓次끈 굿次꼬
                           丁hi1 如；
                            S.C. V: 伽鼠，TkM＋」丑才 寸 弩『弩＝打m哉）
                                               f小十 石甲汕小 ／뇨 7
                           1뇨机 和枷 (7.2L#) 比뇨 m;
                                                         .                    스므
                            瓦 솨 西 比亡可 AC.) 으 民 (YJ+J 2兀 씀）= 足十 2 ' L 즈幻
                                                r    j       ! r\ 11       H=1日꺄
                                                '                           仄.3口




                1
                1Jn
                  1
              11
            r 4
斗11士立量壽r디j n
           4
           寸
                                                                                             Yr
                            ..       g = 毛乂工                           '       I尸


                                                                                                                   三加
                            寸／h丑M r


                                      才근.                                                         즈M                                                  \
                            Q = 쁘三 = ;=；二 r                                                                        D(
                                                                                                                              ＜只 工＝ 入＝ 쯔 :.4
                                                                                                                           ( 瓦，
                                                                                                                                            r3
                                          P


                                                                                                       ／
                                                                                                           二
                                              c
                              =
                                                                                                             J        츠q  H     可t斥
                                                                                                                                그口J。
                                                                                                                                        74m

                            才1l54.    C乂；兀人a h兀工／, 口，                           닢工4乂Z4』                                          쿄工낳小n<)n mn . 7三未工，
                            比Z'e      5.C .               入．／乙 力뇨 .                                    크心／ ,Zd1 ,
                                                  弓J ) （니a/ 十 숀므츠
                                                                  = !/／十
                                                                                                                                芬）
                                                  1
                                                                  1)戶                        })戶
                            Tk4\ ,
                                              瓦 아 二 瓦 哥（／十 弩）二 尸Q才 스QJ 71= ,m,J 中中丑 口．左＞
                                                                                                                                 z WO
                                                                                                                                              7T4W

                                   ／뇨尹d A們瓦                             少       元4- ,

                                  근八＝ 2 '+-'立，P又左m石 뎐｛
                                                       八， 卜，7忿
                                              沆小 k丑 늬乞나오
                                                                                                                  kJ尸·
                                                                                                                     ，크쯔쯔
                                                                                                                      -    -a




                                                              .       . 可므쁘
                                       二＝ 근 , 야火 十I a 口J.
                                                                                                   사 瓦卜J十J졺
                                                      ／十 r' 끄으？ 可 f
                                                              니   ;2tA)O
                                                                                                                                      婆）: 尺十2/ L. 스回

                            ·乙       R = 毛叱고 /                          乙 = 즈玉
                                                                  j                                          ,/
                                                                            弓／ O                   -
                    丁LQ凡／
                                      口=
                                                  .   .   .




                                                  쓰으스 =-               7C근口                   小         7r        -        P      j
                                                      尺               꾸瓦그 中 J。
                                                                             2J = 三； '

                    ( 쿄力뇨兀 ／나 : 丹 d
                                                                                力如小奴）



：卞可年a甘望墨布mm旨깎aan섞




!}!k姓a心커咐瑾沚
                                                                            I
                                                                                         /
                                                                                     N
                                                                                 J
                                              C)
                                                       "
                                                                                                                      q
                                                                                                                 Lm三4 4
            g口
             C            /
                          /
         ,. 9드／ 二 {',卜口／乂59E ' 가boo切7r10／乂刃끄-z = D2/ (>7 < (9
                                                                                ' t/ d> 万＼ryr9少
                 / / ' 96 'I    娑幷읖 =-7
                                          3ds9드 '0 二 D                                                      4 느 J 在 恁 m 豆 季 甘 H 甘 ＝k二hn尸
                                              그f口(Qb/ = Y
                                                                                                             rLL 뇰r
                                                                   ；叫？乎卞刃씨 '凹汀mV
                                                                                                                  i
        加中中 咐           y少 /gH今 9 羊口 卞岫幻 r甲們g少 끼上                                                                  t
                                ,-
                                     .   4 d恥刃그쁘 = D
                                         -a        -       -   V        !
                               / 푸乙 丈（旼) =hrZ
                     / 十vt九？ ＋쓰夕)144-                      'yV              "v可W切勿m/            )＞可加   0上
        口cT7p                                     ：난즈
/                : 寸9,Z乙' P: , 今／z知7, .O/.r= r뇹m可
                                         /             .9／亡 = (c0 ' )(L'S乙1) : 川
                                                                   尸－
                                                                        114/   亡，5Z I ＝抒드 : d
                 和yrr3T/，쌘口 弓／
                                                               tr0口／=1Z                         D
                                                                                            F
                                                           ＜二H寸 따）口' f            H中戶＞
                                                   [                                                L]
                                     .口 = a귿
    /   ;Z - nm可느 作午피埠 唵fj (g-f)J和工唵
                                                                                gd놔엌‘ 口근 ! : 口근
                                                                                 尸H1HHHH+           ！ 石Z
                                                                i小                                     十｛ 人八
                                                       "
                                                           .'Jt 초戶 乙＝/OO (
                                                           "'"       丑
                                                                              丁    '
                                                                                            +,
                                                                                                       ：幸 ．
                                                                                                       -    3   -_s/    O
                                                                                                                                           y乙 = -Ic     mJ
                                                                                                                                                             m




                                                                                             L只寸

                               小m戈乂뇨 m肛刀M抗
                                                                                                 4     싸m汕才豌교 , a才
                                                                                                                                                      尤A丑 加；抑듀d
                               斗 比L工 又n山 小比 m四；
                                              十                                                                 ha지t,                亂· 근首 ，근尺， Cl-
                               뇨i근R도『O.                                                 1-小巴 쿠 亡＝自샤1/ :
                                                                                                                                                蜘d           乙：忌勺뇨，
                                     2R = 29 2乙 +J 乙亡                                            H 乃        尺乙 /I ()c乙＋ 乙之）
                                            已 +J' 已 亡
                                                                                                     功 （乙- x：亡) 十JR：
                                                                                                                    스
                                                                         忌住-x- ) * 足 亡 m：十已군）+JZ
                                      =       근O
                                                                                                X: 子 Z.亡火瓦H瓦亡）-"
                                                                                                               J 夙今
                                                                                                 （乙 寸d戶 十（忌 亡 I'

                                                                                           ()＜乙＋乙亡) (z。-x냐 ) 孑zL.                           亡    =O
                                                                                       m<>＜口尸＋ 9夕5,9亡 戶／亡＞DD
                                                                                                                                     二O
                                                                                          亡＝ 4- ?.                 亡 尸／ 二d>
                               亡 : 丑g99i'
                                                                                                                                          ＝ F/        方 Q "//,1/ 므
                                                                                         多 ' +y 19. 7心 S．力Y9了
                                                                                                                                           匕／口' 수 戶J= Y6오6
                                                                              구b
                                                                                                                                                           “느／I.      '0
                         니b (J            亡
                                                                                       二 , 0317 入
                          ／尸
                                                   느

                                       人 ;                 =mm=m ／八
                                                            h
                                                                     。
                                                                                                                               (ta나J=. ZbZ)
                                                                         t!
                                 '
                                                           '(   "V
                         丁 hJm凡．.
                          "           근自＝Icc 0中5jh) + j2o· 교
                                                                                                                       , ／口O          ／口， 工




11나jnnn屯nn長窄出毫黨聲出出客ri
                                                                                                                                                       / {//d
                                                                                                                                      '
                                                                               /OO 十J （느r') 乙Zo 2) 寸
                                                                                                                               /+J
                                                                                                                                                                 卜／
                                                                                                                                                                  戶



                                                                                                                            'C) 乙 r7 4 2o1       =

                         나才亡／ （工少 。f나4小仰丹犬
                                                                                       工 山-fr乞 뇨人比．




                     !
                                                       2mflJ



                                                                                                     T뇨 Q /d, 7
                                                                                   十j0
                                                                                                     (? 二 쓰브二＝ 스느 e                         /므 尸
                                                                                                                /2叫            尺            二




 144크川d느拉뵤n和d 드甘d
                                                                                                     '/ 7
                                       i7,   7   I
                                                                                                                                                             中
                                                                   1                                1 1>1 그／
                                                                  0
                                                                                           計／                        "                                       f石；石

                                             F八石h\ 닢i成K                     y5 j友오                  丁EM                  /M而 弔 民 回4Z 力n 包

                                               룐' :Pf上，, 可'4꿈
                                                                                                                                q'           =
                                                                                                                                             ＝   乞       ,           \Jo     b/   a



                                             탸的 d 們                         n        丈h: 人和m石1 , kX札                                                                                  4j           乙 7

                                                                            C＜뇨싸                 力뇨小 d피
                                                                                         乂r七， /4戶；



                                             Ep= e且느／, '[5中'，寸' ] ; ;l-LVb/O.                                                                                              孑

                                             "r小L&                    Ia       J" "             i       ']   .   “       云告石m                                    "
                                             F/i才r- '-                     ) 口，d (2,%) ／仄t j布고 寸口夕亡449e +Zddd

                                             比d妃 a쿄 加a十小d 小尤哈교-4- 口-t丑／
                                                                                                    b        a-                 J

                                             We ; 旨｛
                                                   ，促］' d寸＝
                                                            T(J,a_ j                                                            r，(盛十孚「卉山4尸
                                                                                子그汀兀y, =                                        즈두드三
                                                         y m蜘）'"                2戶
                                                                                                                                나入 kf （久，

                                                                                                                         a
                                                                                                                                                                                                   M
                                                                                                             b
                                                                                                                                오 \
                                                                                                                                        知                                                                  d
                                                                                                                                                 그   V                       小                         d
                                                                                                                                                                                          즈又
                                                                                                                                                                                               ？
                                                                                                                                                                                               호

                                             MJm：守JI1I 寸＝ 쑤S  了
                                                                                                                                                                                      1

                                                                                                                                                                            tC                     之
                                                                                                                                                                                                   i




＋藿在3啼多出小瑤깁寸； =＝有고二： ＝二亡4二나卜m七뇹芬七謝d心李
                                                                                                                                             /
                                                                                                                                                 기
                                                                                                                                                 ｛
                                                                                                                                                                                                       r
                                                                                                                                                                                                           口
                                                                                                                                             /
                                                                                                                                 1尸11111U3
                                                                                                                                                                                  J
                                                                                                                                                                                                       亡
                                                                                                                                                                                                           1
                                                                                                                                             t
                                                                                                                                                     M
                                                                                                                                                                                                       1
                                                                                                                                                                                                           1
                                                                                                                                             뇨
                                                                                                                                                                                                           1
                                                                                                                                             뇨
                                                           尸＝＜工中＝乙
                                                                 4r




畔
                                                     --Q。 iV。
                                                         可                 且    ／
                                                                                二
                                                                                     L   온211兀bi : 그竺 : 三므쏘 二 t叱 /
                                                     H
                                                             寸    （                                                             r上河-                                       _{,__h,'&




                                                                                                                         /8
                                                                                                                     /
                                                                                                                     1
                                                                                                                     r
                                        7. 8
                                                     乙q= Z:／는, =                                                        근·'                                                                                           /
                                                                                                                 尺 十J ' 伽n論)


                                        Th.且 h才                               小f쿄a싸石 甲 0 和 ／j,Z                                                                                                             R比 口im士婉，

                                                       /                          /
                                                     ／之' " 二；万小 十J u-,c
                                                                          工
                                                                                  1                  1   1   1         /
                                                                                                                                             工                          /           r               /       \
                                                                                                                                             ／之' 十j四（C 二反？)
                                                                                                                                                     .        1 .   1




                                    Tmd衣工 0뜨弘Ap三 帥뇨나才                                                                                                                   4e／乙 a4 凡 尸小八4／乙／ 尺t'e'
                                     -4玘4-刃匕aibL, -人丘力1-                                                               R' = 갚-,'g, a ' 口勻／근.' , 乙‘= C근。 ,
                                    (n小 在 X뇨 Jr i4 7肛 m乃
                                                         )/k ／沅4- OC-                                                                                                                                                            伊4枷丑
                                    知d 0dmi／伍們七e 小的力，/ )


                                                     戶，仁n叭 (i, '1叱

                                          和，, 制的'＋牙）' 嗟퓨d寸(:胥）'，僊）' =m吐
                                          F，吐 磻 I,퓌' +／훑쯔)Z＝뿌幅) .+(뚫-'
                                                                    y                                                                                                                                                      叱.7/ G-U孑
                                    d          仇Z 4'       C-
                                                                     H于
                                                                              .             和＝
                                                                                                                 ／票：
                                                                                                                                                 .   0/6了，
                                                                                                                                                         皿
                                                                                                                                                                                                        ;        次二 gg. :        _니


  J
  1
                                    <＞女 乙·7!. G-U秀，
                                                                                            R5 4曾 :                                           . C）그o7 jt                                                ;        次二／'l口5- ，功，나            ,//

                                    F亢占-;1 (7.")                                      / ,＜八／i土／t                                         a＝石＝Ge '




144442114斗甘4二少 1
                                                      ( 2J工a拓 + 가d了 +J' q3G( 于2a3) = 쿄 (I枉2



               1
               ：卜e
                                                                                            )



                 !
                                                                          和    「小 3口:7,                                                                       +'a’乍 : ／白g叱 .
                              ．未r
                                              Q/
                                                    o/ 二
                                                                          Z7t （尺S       (i+')                                                            72兀工尺＄
                                                                                                                                                                                                                                 什E.,.7
                                                                          J 3 _7__
                                                   ‘끄 =               arCl.                      ,                  ) = , , ,Tt2
                                                                                                             :4, I，押）
                                                                                                             3&                                                                                                           32g.




     뇩 rtm껍V計4拉望朴姿뇝計hddnH窄有
                                                                                                                                                                                            .
                                          Q
                                                                                                                                                                                                    =
                                                                                                 .
                                                                -k
                                                                                                                       '
                                                                                                                           (
                                                                                       1o
                                                                                                                               i-
                                                                                                                                    f-
                                                                                                                                         q
                                                                                                                                                                                                .
                                                                                                                                                         3。
                                                                                                                                                                                                                             .
                                                                                                                                                                            -
                                                                                                                                                                                R
                                                                                                                                                                                        l
                                                                                                                                                                                                            2.
                                                                                                                                                                                                                 1,
    누
    h
                                                                                                                                             1/9
            t   7;／口   1 F加，n k力在 Lj· 2.                                   人工 小m竹力d 7Z在弓在 弔 流-i江

                TM11                    比口뇨 伽砒 口在，

                                       心芒 岫 쯧 m 뿅 可"／아


                                        二
                                       H之 . 擘 C力口 쭈 石n즈芟 才jP둥
                         m
                                              M小 k
                                              J
                                                                                     .才 尸，a 工A且 Ca刀三李
                       小
                                                                      M
                                                                      1
                 To



                                        M     스
                                                        1
                                                        加
                                                                  쭈
                                                                  m        m     끄
                                                                                          쯔
                                              b
                                                                                 b
                                                                                          d
                                        H
                                         U
                                         1J
                                                                                 =




                 丁汕 4: d 加 和力d 4仙今y 4.4 j
                 叫孝加！' aV: 誓A ' 삯嘗佑哮）: 4bd，吼月7和 二＼
                                  \r
                                                                                               극 .7
                                                                                              1/   八
                                                                                                       '. "-
                                                                                                               +
                                                                                                                   t'   /




                 Th工 f小恤， 石才 瓜 X／比 am／尻 4/
                                                                      <\    ＜丈                 17 。(

                 巳 ' 穹｛l"'Ids 「｛?,,!！브'(1:o)]""》"' :,｛少"" 'm"『
                                                       『사的刮' 如m'놔4}
]4 d ＃甘
1
                                                            x二o   (j= O

斗

哥
                       . 月' 尺S 口？a 十b3 十aJb十a小’
                             4/
                                                       口了／:)2

                  Th工卜／


量片1注41jJ1
                                                            그（0。W., : 毛和 obCL (a..乞＋寸）
                  아      m        '甘     '「 "     ):
                                                              P{      끄_ s (? c此＼ {+0凡+O.功
4
;




                                                                           ／긋（9
 7. /f   ／二月力）,t Jk力而 $/, 3                     亢矢工 ,iWH竹q工                          小
 亢仙 丁E,.
               加小如 加 X뇨                                                                       甲
                        「在                            可 쓰什汕 Co加 /{


                                                警 警
               <
               <
                                                                                         d
                                                           任>
           1




                                                                                 ＝
                                                                                 夕
                                                                     ／
                                                                             O                亡

                                                                         戶
                                                      月M                 L       J
                     <
                     <
                                                                                              d
                                                                 戶
                     戶                      1
                                                                             d       t   m
                                                                                         <d
                                        如
                         n
                         h
                          X   y5去M쯩小和둥
                                =
                                                                戶 . - 釘d."
                              1a돐 戶A警 啣k (d乃） 和小亡' 5 ' d
小小2,e    和니煮닛刃勻'                                ;
                                                1 J
                                                       Pd: JE『丸' 크兀'U'
         죠－+.小／肛                                ; 乙｛：次反／忍 : 私巾／他

cc磁初4 부 E7 ，版
                                    d           3 = d寸 :
                    戶乂石， 肛（小 이 二 B
                                                      私-i 魚 亡
                   立 C小404 (dmt) = 으
                   근＜t                d力口旬亡
                        1          귿d
m往／尸 ；仁 C石才a／듀，

                   及 品叭 和（十功 二 2d 匈
                                                           他亡
                   Pc 也休 和 (d尸亡) r p民 亡a., 急
                                                            亡
Tm 玗小而
                    吼奴
                     4亡各U 7뇨埃. ,
                                 肛7/d m
.／仰m力而4, 0i 乳 口
                J, 9iV亡，人 고枷之．




                                ／刃
                            i                             了川 力伽／e+ :                             ('v ' 나2) 再「0
                            乞才 E3（芬，q，弓） = X仁）Y翊及計4
                            小加俎次，／뇨／孑 /0n,,e 퍄仰王m 幽a 而ar /yKY근 :

                                                   女瓷4＋客『 士弓3 『窄' =O
                                B늉 大衣且 肛／m八力iim; 弔 -v切汕4- a1尹＋H上M才，

                                  女 余 = 궂"                                           吟        汝지 = Ac亡d,－凡X                  十84／뉴凡 X


                                  寸告千싸                                               ＝수 Y臼）; C Q也上yy 十끄44q五川

                                      J_ 4_ =-L2                                     斗        끄3) =E 缸l朴 十F／八-'4＋喆
                                      근 乙i룽2  唵
                                小J1눗不              七二 求； 十名十J二
                                                           J
                                                                '
                                                              4

                                                                                                                        e
                                                                                                                        k
                                                                                                                        1P        r
                                甲余r, 氏 “O 7分 久＝口／ （兀                                                            口／ V
                                                                                                                                                二
                                                                                                                                                            /
                                                                                                         4
                                                                                                    a.
                                                                                                         ．口／




                                                                                                                   十
                                                                                                                   nb
                                                                                                                쓰
                                 A =-c =-o a小d 弔X . 竺酉                                                     口U
                                                                                                                             =
                                                                                                                                 To
                                                                                         （人     )
                                                                                                                                      小
                            乂뇨
                                                           1
                                     m                         小
                                                                                                                                                M   小
                                                                                             ,
                                             卜.1
                                                          1
                                                          a                         m和'. 4兀뇨
                                                                          2
                                                                        二 H
                                 E
                                             奴
                                                                                    = 盛；(5表（師再今（）八亥力）'
                                                                        느




                                                                            2亡 之d
                                                                                                                                                            =
                                         1
                                                                   a
                                                                   中
                                  X
                                                   l 2?
                                                                           X



                                                                                      '（山 Em 뇨丹나卄 的h5)
                                                                               둥＝O, d 加之
                                                                                                                                      尸




                                Fu       C二） 二（9                   a7r                                                                r1 寸17
                                                                                                                                          ==1   /n




                                                                                                                                                        /




r吐분m1望j序m1亨1tFY j 1 X 立 시
                                 m,d 毛：뇨                                             T 小tA-1
                                                                   c.
                                                   나二 （哥）' +（響）'『（쭈）'                                                        :／南M岫二 7敬工
                                ／比妨兀久／多 ／四小小· Th且 갚乙尤勺' 十
                                                                                                                                                                ／十
                                /2, 私上d/m/ .
     Y
     寸
     1

                                                                                               ／긋 ；之．
                7. 1 3            F枷加 丁口4毛                                           ".5- 冗乂＋ 7二고乙小 甲 ／又꾸 ／凡rm枷.
               갸枷丸 m
                     , （竹.) :
                                                  色= A 戶在呻 끄侏寸）
                                                  '4尸 = j山
                                                         ．E枉 月 C力＋ 41 끄（知r)
                                                                次；    f)
                                                  H
                                                  n

                                                                수尸
                                                       d
                                                                  =
                                                   J
                                                                                                                                        次. : f= H／石t 注
                              U              ／
                                             外
               Tk                   t
                                                  ／也／珏
                        /
                        e                          닝                    小J:\
                                                                           舛7    4 ,
                                  nr11r/ V
                                             m
                                             E                                2r （乂
               Vve =          q                             少                                    .
                                                                       4녹 /' I r/ q ' m中 亡乙在기尸十a／心 =


                                                                                                                    I
                                                                                ec c刀叫0 三＝o
                                                                                                       -        _
                                                                           'i
                                                                                -{
                                                                                          -
                                                                                              ',
                                                                                                                                          '         L/




                    : 斗트 兀J 뜬' 丁：2(.-e4,)                                                                                          nm寸
                                                                                                                                     口
                                                                                                                                       磁，五首 C./y)
                                                                                                                                              (7戶
                    = A 'o."月a 6 丁二
                                    z什뇨U
                                             8

               丁1.皿 F伽4 石仰 m去 戶교五
                                                                                                                         伽全쿄年 /i )
               艮： 昏 工I 1-1 j'小
                                             lr            ＜乂

                   “穹’{LO J """『미'"'44 '町,［,Up!"싸7'7]10寸쟈了
                                                                                                                        (t   2万＝




1士ii (1P1f李m
                " 學｛쭈"끄 '（孤，
                           ）『葦끄亡（札0가茴『3二（妊j7)了rd/ }                                                (       1/




               『 學｛罕 끄 '四『等 妄 丁：' k，키
 卞뇨 U


               『    '   ：二尸
                                                 (" a 9亡        ' "                  ",
                                                                                                   ,D
                                                                                     /23


止꾜上크妊少心
     -r뇨-'- I                 .         .          4/          .        .
                        Q: " 시？We 二 므뜨뇨a豆C呼t = 4d美7Z                                        《／
                                  t.乞         '1尸s X44十이            긋／2S (C7{＋口I

            , 4才小                                 乂玖e 婉＆ 友石           在，
     TJ叱 f如，

                                             :=   （乂JE
     e{
                    二                               2-




                        46L「 구口JWe 二
小I
                                                           I       小4\ ( 7; y了7.
                              F＞乂


                                           rE,1' 如汰뇨
         F批h七 尸今m兀 z／口， 小d戶似M Q 和元征
7 I '-t

                                                 .4t
     0（七m4 7h 긋4/a g/.7 . ？玩小戶 (7. s3凡j／뇨 a加小-

和升呼7尤뇨 -r득！:
                                                                                  .K  ，戶戶   』    八




     fm= 읖k誓）'f優）' ：옳7件勻'日笞）                                                 ＝스으으므므 = 7X／口7
                                                                        11
                                                                                       口1
     古                   七m刀 m 三                    匕乂 二 쮸：元60師．
     아I ' 6J7乂／D7 욕／M                       ; 和／96石 州나         ) 次口＝3．긋V
          已＝7票 -.O긔人 ／·.,                               肛 7{ > ／긋口. 了 月竹디 7 出： =I, g모1

     F,.万나． (7. 57)                     尤뇨        Q 工乙．


      (TL = 傑이' 和d n七卜）'7
                                                                              }
               \/


                        9叱：)2. & 忖［'4-（等）그日等）YI - 中）
          끼｛
                    =(5, 336.
                                            f
                                 12/
                                                 C뇨m                    四Zm d 毛 ／于包M k光뇨／
                                        b < a. <（乂．                Th毓 才／工 而如d
                                                                                                                               ／氾』
                                                                                                                                 方九‘:
                                                                                                                                    ，才 伽교，
                                       乂兀 戈I'工 丁E/D/
                                                                       m八力겅7Q          ·．




                                                         f/   61   =
                                                                       응 雁石刃' ＝三』&月孑
                                        万
                                       <＞


                                                          赤 ' 方「 但｛이' = (3今（7尸
                                 T뇨 才呼才 兀                               ／呼毛口 加泣                                            ___m彭A.
                                크7＼尼            T八Ill이             丁E,m               o-z/ 了E口11 中九mm. ·．

                                                尸뇬）' : 牛 *求 : (3 '기뇨 古 －未
                                                什的' : + *글도 = (34'. 刀' *示
                                                //2 fbi, ) 工 =
                                                (,＝卞＝    /                 古 4十
                                닢加4工 4. >a,                            fb:1 < 下，,,.
                                T／니    f      느 L. P P II
                                  노r . ' <>11 - V' = (yt丁孑 4                                         I0    =
                                                                                                                   Z긋 子／
                                                                                                                       ／롱 :
                                                                                            下／
                                                                                      냥甘
                                丁kJ시뇨 -1人，七－ 뇨切e


                                                                        =r 工才
                                            小


J44出미什HnMh州가n斗｛ 七迦出心斗1之年卞弔441
                                                                                                 = /87了．

                                                                   )
                                                                        b = 긋．60 C似                                 V

                                                                        d= 可D. Ct.,                                 1/ /



                                                                        ＜工＝ 3. S3                     乙，
                                                                                                       ．人             //

                                b <，仄<a(                oK ,'.                   干！   m          :    7.   3了F件孑           >   /),.   /




b{
 J 占f41t1｝ 主4j
                                                                                ／긋 .5m
                                          巨I司
                                                                                                                            ．,..
                                                                                                          e ' j抄／=e'Jm伊 ，·m凡』




                                                    石， 肛 “
                                                                =
                                                                      臂        久了ro／죠4                         mm    枷


                                                                                          C


                                                              f =      MC
                                                                       가1, C
                                                                                                  力t=!/ 27 j · .,                             J/
                                                                    그7r力 ／亡m斗


                                                (T卜오 入h万 Cq加小尸q寸 4                                 2Jr＜兀 : 小人8 )

                                                Yk고 口玉心t爬， ／工44』J士 匕2J4.44八，4丑4-                  ＜兀＞>VtJ, 4- )：札나 口imrd力h凡

                                          畔U在 따力之 싸什必7· T뇨 和兀 7和10左
                                          沚 如才 平뇨 的中뇨／ m乂小7 4們／ 戶a/ 石
                                          二 ,枷d돠m反e .
                                          17．     口       尸뇨加 (7..7口）,          ／豌 PL/2 " 乂／円
                                                小7ii表
                                                                Y = V仁흩으三）느낫2.
                                                                            。
                                                          '     P 二恨4二（乙如平2.
                                                Tk1 仰瓜L 斗 液. a才 斗4小4兀 m四才兀뇨 表名和叭
                                                丸＝ 2.흗篁 =6D2,
                                          m侄 次0 二茗 :／幼 .                           乳 匕些              1Lz三5L，人5L/Z- k／万
                                                                                                           1 6
                                                                                              ［玉可巨7三11         9




t r t t i 1 1 t 1 )t！ 卜｛ rHHHHH召H=h늠뇨nn
                                                                                                                           小／        .



                                                                                   %Z0
                                                                                              1 59D 1P푸두 1三                =1/1 0 Z
                                                                                              1 5y3 1 G7그 1                     . cb8


                                                                                   :：二
                                                                                    15。
                                                                                              1 58可 !1 C31                 e     .       /그
                                                                               푸                   51               66 "    ==. 0O/ 오
                                                T
                                                                                                           1
                                                                                                     'i
                                                                                              1
                                                      4


                                                      듀＝ 픔二 : 7. /f &-f4方 / (,)伍小加小小LA-.- 72C- 云）
                   Z18           F규白m m今伍 甲 在瓦二 7, 5_ :
                                        H各：/4. 丁.（七r) e' j阡

                   E戶 = " 寸, "'           恥：月孔'(44小' 」；F孑
                                      끄姓꺄'」



 U和h嶝n奸4卜中作m和군
                   Hr: lPH' 丁/。c幻小伊' = 手스 丁1C（毛円e工1賠
                            "-   C-
                                                           2TE

                     ｛孑7 <1／
                           乙 P나E
                               「付．毛‘ 기놔知烏／寸                                          .. 근：, -   (AJ{/O              m




                                                                                                                             콕／
                                                                                                -p-             -   戶




                        152 ＞니乙 1‘芦只 = 匣？云1                        恤恤J' .+JJ. 凸E: ，尸UV1> 1 그
                                                                                           (；口m       1H=               m4


                                                                                                            d



                   古 比衣工 d而勻 小                            戶IC及 m衣 如m卜 肛．
                   , ' - (A Jb' (-k（力 [e5P느d恥］: -z 4 工二（抵／)44 '戶孑4
                   느中 m 1                                                                             1缸 佶｝<y之
                             .
                        J 昌 꾜 Ck刑 e 好
                                                                                                       戶 功Y
                                                                                                          【

                        陰 L4川寸뇨和］
                                                                    쭐                  \


                                                                                           =



                            돐                                            꾜伍r) c力나孑                          1缸 1弓1 <L山
                   H戶
                        t                                                                                       74T1 5 >-/2

                   Cd泣勻．沚孕 甲E/ M月／ d孑＝呱’ 多小，뇨，
                                             .
                            m可A 小가L4 =8e尸oC

                                      誓 아냐LIZ “돐可"
                        小
                                                           尸

                                         d 1
                                           고
                                           n r乞
                                                  乞
                                                  帥            口
                                                                                 瓦
                                                                         戶
                                                                         亡
                                                               ／
                                                  小
                                                  乞        ／
                                                           之
                                                                     1
                                                               :
                                                                     呱
                                              8
                                                  L   n
                                                       十
                                                                   脚 =       O
                                              J
 11니나川게


                                                      」／그 7


14m可＝d m 寸 寸 m 斗
                                            77t加／7今 尤屯 如今m y 4亡뇨니「；石 교4寸
                                      ／尤ha뇨7 小m자亡 戶吼 t11孑I >b'2 :
                                                                                                                                     LmZ
                                                <
                                              r A 丁k毛刃 C寸나｝                                                   n學. r,' 44尸瓜P方   그d

                                       E中 二                                                          F4 r 「    亡＜土＝


                                              \ bJ／乙b尸 Hm 可윳뒤
                                                      >                                                                        各    느l
                                                                                                                （毛기m及 "件弓）
                                                                                                               釘：


                                                                                       叫
                                       乂J,6, 己（/ 근仄       口4d               ._4




                                                      伊
                                                      E       H
                                                          J                       口J 3=V2:
                                                                        戶
                                                                    i
                                                                1
                                                       /\ C<)4 아／그 = B 4-4 Ij o CD寸L7/4

                                                              프m                   8
                                                                                   1
                                                                                   m
                                                                                   1
                                                                                       나       d瓦
                                                                                                       汕       毗



14; j下t                               口加似 “            곬ia小4나1: 돐M乂。(P - L)／又
                                                       나汗 ta나L／只 二j人 口亡It .'( (P-L)／乂

                                                          z瓦， 아／a = 孚 口t石 "CD叱）/2                                       /
                                                                    r

                                      C力U兀kL!       口＋ D力少 ) q亡在 사아L)／긋 수 1 , ,4/ 小比 口弓在乂시’

                                      依， 肛／a'= 畔 小／咤右 甲／.4- 小균友 比뇨 md才 加蜘d
                                      似先J 小允』（小dZq; 7．키．




} t 七 王 1 t 七 七 七 缸 뇌 n 目 拉 ！1뇨y: :




:



                                                                                           ' /2 S'
                 ［兀시     匕Z42似 그，6.
                 B枷似 부 才知 如小戊’ 仰／Z 如汕斗 口M兀泣
                 魄X뇨 伽mm , 4 m右少뇨 m珏i沚 加好m毛
                 叱凹／뇨 孑－4戶洹 如毗／如伊큐 TE 如／
                                       白 才a砥 M
                 4孑 /G丑／ 弔兄征 7余mI                                             'k杆"
                                                                              아二t右카
                            奴“//. 4뇨 쯔증즈 卜         견孕 )                        04
                 如／不e 石啣m才 m／乙1 丁E 小奴／-- -(U力i乂끄 辰 i玖丑
                 TE1, 伽沚 . 瓦d H츰 ?. 戶 /m 如小，k洸A兀
                 ／伽k平 咆伉 rM 如ae 如끄／/ /m小．
                              尸'？『H. 私-t끗    , I/a = '1         （두/ q>67
                 古a未土 amM乂小，才 如口（之 弔屈44- ／玘4d加石t 4*t兀‘-4才力之
                 比뇨 丁八4Io5 -V邸a- . Ti山-4, 汭＜- enm= ,{Un4X毛，

                             나已 小叭흣 e' jP}
                             14X = 三뜨 J/：小 'TX 土汁耆
                                   3Yn --  a7 e UI        J



                 幽表戶工 P니E『毛느（
                            「／勻"        和        1吾i ( c,'2,
                       坤＝K ' ／佃시'．毛"    I乙L 計叭，
                 a닉    카M“畝「 帥／k二P和后丸                   和      ( ,V C/2



m컥吼出m七小脅貫月d4m읖
                                                                          7
                       근TM" 2口「 尸和色74乙 >'/;.
                 1- N 尤石＋ d乙白二勻 小汁已 7Z也乙乙 Ca机衣 Mm休 口4.
                   E (J = f4 A瓜娶［e'j阡蛇批] =aA／小警c&-                             和小／    쿄
                        L   缸倆홋 三" 층                                           7요子＞:／乂


                                          ／只 9
                          쯔a       n
                                            小
                                            1
                                                nb1
                                                      孑』‘ -I外］ 戶
                                                       ' cJ                  1끄꾜   如
                                                                                   1
                                                                                       굘
                               L
                                                                j   尸

 HX ;
         hB      J.       7r7( =（乂方
          ＝二＋   片n/ V\ =:H             (：
                                        二
          t七뇨           1小＝




乙品m4 쿠 E응7枷 d                                                 孑「 "/a ‘,
                      小 a               -        a ,, I- －叫 l) ,nH仄 C4／교
                      口
                      ＜/ \             C-o--        ／出 - 0 t二

                                                                                   呱
                                                                    世泣
                                                                               d
                      짓스 小갸C／그                                           e
                      H
                                                                         小
                      H




                          毛士

C娩m七 :
                          止 7뇨，PVa = 니／2A
                          取．
                           쯔r프쓰뜨느-e二"
7   n
    乙


         n = d> 力 比／r1
         n = 亡). 5뇨4


        尸小 탸小                          ?. 1句            djr. 2 V:              小磁中         -4-t4끄之

                        1／小                                                   加脆石伉 竹扁M '
和力万 戶；d7匈d枷才
rk枇1/ d= 뇨尻 ＝口· 25 ,4 ·




                                                          /3D
                               7. 긋극   F,i.cm       T。
                                                     .石七 7. / , 尤뇨 石們L     c亡／H洸危M兀
                               平 才小皿 Pa加Z凡Z eLC m批力1 ')4助石 m心m之 在，

                                          力뇨 = 和Cl 然幻

                                                                  念磊
                               YkQ- //m／如乂eZ Q  =             4

                               Tk乞 J큐imZ (9 成        =        Q
                                                              e



                               쿄丁 比뇨 mHb 야和                               오乳        스죠   ％百
                                                              q 在 7=           二



                               丁뇨 知L江抗m1石d m足， 尸力范／J比V:


                                                                       APPlIrA卜七E
                                                                       C11*gl-




d 寸m1; J 3 1 1 d 꾜 甘 斗 蓴 ＝ j
U
h




                                                          仁
                                    1:
                                    C
                                        <)


      231                           11               ,       J                  1

                            n r \ 륵午
7.
                                             -               rJ
                  「                              "       "             "


Th工 小k才 加斗 石 丙力14- 和m 4 7싸在初弓，
.4仄굿乳 兀 -4《以乙／亥 兀m T뇨 口고在脆M丑 平尤쇼 a如M友


 十戶伊빠加  ：亡；二仰小
                                                                                    d4J


     7R; ／之 ' 7                         i2U;                      1



七4나.工． 蜘＝ 言 “打YX7"10
               qxic                                                                 尺         / 八   /
                                                         J 닉 尸 可i了 -
                                                         .        ,,       -4             H




                                                                                              /_.. ',
工四 小如任d 戶MI; 疋 = 죠y; 二 ·／勺‘ .?. 5-긋 名쁩 ·
C力和 尸石十 尤／岫 石艸 毗私工 和a乂 C.似毛 他

     F늉乙 脚『' , y疋 " / ; 戶 ' 幻 " 土 '／幻' , 和 " ／土C'" 교丁.2 . 7Ze／毛
 加t' （力加d X7人4 m4 ，左 社， m 石艸白工 石킥4
1뇨竹 却七 ／工兀 X凡才 a- A航iZ4 m戶瓦南色 끄4七九妃兀 甲
     -.jyC/ -.1       加乂｛ y力蚣 知 小y寸m們而e 孑仄『／'
     Th乂4 斥小1 大뇨土 8R = .I-J'. 3 伊似 小d抹 蜘J）』 戶
              a(U = 그칼섶 = - .1114石 ) 口z- w尸 ='U뇨＋d口J 二. gg／口七 = 7. 77X,/"
                       h.
                            .   <
                                -




      口t口
                  유＝ 寸tf G43吾 아小나和升始）
                       k/ m勺궂瓦 小뇨石／

                  C。乙如, " "9／尸戶 ·
c4.七臭：       0才 9．任64+吾.                -Y尺： (L-j ..두g) x/c"3

                                         ZR, = 44 十J卜tl .乙
                                                                                          （比뇌
                                           , = 可싸우八
                                        -3닝可


                                                     '3긋
                 小i力i1 吼／ 1弓V m＋뇨， 723 :




ij4dJJb14늬4i m



            m
            ]




                               兀33


      出1


     山나
口刊 如M兀 丁Em· 加m7 必小mm7, 7
d q G好， 毛小2 "' ; 유 기qO.5 ; J. A운平，m 《四
                                                                      小   "




    나
W0 /ii- = 兵 二 7 644孑
              』 M 旒亡＋ 和才 加石쿄已 X/W 勺升才 甲 才乂工
                                           4크 尤人工 仰小／ 1뇨們缸7 甲 才뇨 必可



              四 口尹0石；  仍1 F昨       a 畇七Q 的耳J／仙m玩Z
                           Fc- z.- （兀
     叫
                 a-尹力伉乙l力．

     小
                                                 口J, J a仄L                kcZ.＜工 只二 口2b· 舌

                                                   C小M升志              z二 加까모 匕*)                I而W


     y乙 = J 7r毛口J1 小 . 0/6 二 乙Ut.
                                                                          力   느已   二   7. g 3X/0 '3

           aQP' "
                                                                 Z0
Ty小，／寸白｛ (7; 9기 1抗 幻 :
                                       z瓦 아 + yL 二0
 7h，仙／{4j, 表고m口싸F／加1 ;

         두                   P   7.   (=
                                             勿，
                                              卜人 戶／十 -V
                                                    I-I--

                                                . Ol
          9        I  ;01E,c;?
         g.
                       'W.
             乃z 7 . D/5j7                     /.DY
                                              . <90 a 5
              ci
         吼q7 /39. 65 . 0/ 57

 Ty따시                  묶 “ &q7 GH2/




                                                          /31/
           亡加蜘勻   Q>
                        ＞乙                        듀＝
                                                             下
                                                                 '可
                                                                      '   =        O.   L.
                                                                                             J』
                                                                                                  了   6H万
                                              코
                       8W = ！즈；끄 = 口．37
                                          升
                  （乳＝ 긍i刃 = 3又9                                           >>,           /             乙蜘乂‘d/ 4 )
a才A丑和如心/
                                 r=
                                                        L
                                                       ld
                                                                 i        島   e
                                                                                  }=    i
                                                                                        V
                                                                                                  =누 r= !!T= /.U5
                                                       和＋1                                               .卜r


F肋M (7· g3) ,                Q= 鉀e ＝용＋뇨
                         \
                                                                      4.           Q
님a白亡 7易1 口 ;
                             응
                                      ,   기 =            j
                             （少 Q江升I)
      斗汗在44力汕4- 月恥aM鼠， 升 근a =, Jm = .5口q
                                                                                  im 中 r
                                                                      Q = C什朴乳 叫 '7瓦
                                                                           e
                                                                      Qe二 拿 : 9y7.
                                                                                   7

J斗；斗 在 아伽比x 幽加婉， g＝子, = r：                                                                         兀915- (c냐力Y乙幻
                                                                      Q.=U＋引4L= ?8교．
                                                                      和 “ 多 押5.



                                                                 /35尸
                                                                                                       l

                                                                                                       但］
                                                                                                                     P.   '

                                                                                    艮＋
                                                                                         2.                 2.   .




       岳
                                      (Q，姚，a)


                <
                    Hd
                          그     1     , rA B] = p,t立 이1 j
                                        LC DJ
                U
             Si1: . . .긋                        . 十二－十=                     又
                         A+ W4+ C.근0 十P           J4      ./Z1I         ;2+ 2O/ Z
      而
               Ft - －十－土十戶十                               /

               F노    12 十 乙／근 r

     F加艸 丁M在 7．乙                            乙沌 三 魯勺 仁：
                                                     少'

     Fo, 4 MMZ斂 足乙C.                                      小m名乙 , 7 : 足／2이                     4寸   /



          尸t               4'                         =               꾸7'
          "' 伽多 " (學쒸“                                         (i.-z7) ' 可弩芦）"
            ，小小乂兄 d(U=O . k光九i m力必｛C工4- 石 J
     口士 4J4刀，

       뜨 = 브亡中 . ／쯔초n '
        PA      0. -a8)'             (/ #2-多)




1




iY




               0           1    i.      J        =y       二十
                                                                  6
                                            0
                                            A-
                                            V




                                                          ' j 36
                                            丁뇨 m甲力나d
                                                                        7-目， 匈亐                                                                           m且／

                                                             斗 “ 月 " 뇨警 M 즐立
                                                             妓            孚     1
                                                                                             孚  C寸4, 7r3
                                                                                                               a
                                                                                杯
                                                                                                                    누




                                                             "口끕呼呼
                       fl          乂Ae 仙如底                                      슈            (7.，찌 d뇨，


                        J   rt(     "
                                        "
                                        "
                                            " '"        "기           ')    "'       “   臼／     .'）        呵，            ?",         !:！「寸       『7        「寸）     ／尸，m
                                                                 亡
                        =/n'/"小기므抑' r ／豈 건뇨a：兀l-
                           ' "’口 "] 了n J ('
                                                                                                               才‘                           .
                                                                          24 (d卜皿 二났 十 . "L/,1                                      ' S 兀i- \        /
                                                   '         3뇨 '                       2누 r次', 和‘ 4m슬키吟
                       “카' 臼" 刃얗A '［차和느翌）/'
                                                                                    d/7;／可     /1(>
                                                                                                               *쭈스十／    측，』4근耳是＼냔
                                                                                                                甫／7 (r \ 乙 H11크H / I
                                                                                                                                     1
                                                                                                                                     I
                                                                                                                                                         9?乙노／        / l 0 J
                       = 乂在I따r ') 쓰 4工 r三 .                                     a느万느．"


   }1] iJq141JJ
                                            "                Lz·．- + 뉵尹斧M츨勻
                       T뇨 山仙h山-d鼠 -                                                 (7.1川             ＜d戶
                                                                                                      戶
                                                                                                                                  (t石01白 只 z                    ／亡寸
                                                                                                                                                     /


                                        幻－口J。 : 프竺쁘쓰쏘II.]
                                            亡4J0                          ＜工L닉

                                                       = H仰r니）/ 亡 ． 戶 느刀）白
                                                                          ' q/ . ., 力T亡）
                                                          d 十（三-, 1 긋工



丑弔n戈n忿每肝bnn智뇨뇨智1b늠뇨m
                                                                           i; 夕m ;/

                                  7느 << 。1



                                              aJ 나 （乂J。                                       ., . . .                        .
                                                       口'0
                                                                 皿 ‘匈可副副

mh耆시hhh깎nHe놔기디r U




                                                                                        /37
나
          口i크 F批的孚
                                         7
                                         n   口
                                             J



                                     O

                                         誓
                               Ud
4 1


          仄十   工＝띠t, 孑“O;     二
                              나



                                                  ; Z= 毛4.／斗
                                X
      =
                               니U



          =                     dd   O
                               나n



          TkW,
                  ii（키瓦J'- E佰n ' )／『 二 4글；4V          j   IW " 1rZr。
                                                                   1
                  口   V




                  L k鳳1'『E匡，1' )a " " 喧응쏘
          4丁 (7,10?) ／比旅＜小， 只늉1


                      加寸느 좇十 斟半 等쁜
              (h a如나兀 니뇨 小Md
                                                 予少小牙)




                                     /32
     CI／月PTE尸 了

侄：iH             T九， 屈 4 꾸七：k/ 帥丑 74 石，
                                      ，匠“，m仰교
     3 ‘小d 似瓦派； 腐
                                                              蜘＋ A사小 瓜 3戶仙m
                                                                                        丑 比／m才
     4乂乂尤人0- m／如小 CdkZ/ 如才
                           Jt                                                       似d五뇨／ 口才口끄
和侃
            (m뇹 m                                       [ ' 」 加a／ 啄 ）·                      J
                                                                                                ／心七

吼W 呼M 配戶m4: Jf 尤攻工 4M才 石
                                                                         口Z在Wa左急；
肛才 小 石 衣
                         \ z-c石
                                 4M机／ 石                                 上志 m伊抗근
乙攻mmZm泣d 石伊j而k石，
                ／侃 似 ‘d                                                                Aa,y권．
                  上 二 Jn 4- J－小
                  2느            근l.                     근스


                  J－小 t          工 ＋夕 -i小
                  근2,            근1                     근3


                  ,1小 二 工 + Jh
                  근三            근t                      근l,


d才 在 小七十 加qd在 名                                                    4叫今 力뇨乙 a枷兀 沙
                                                                                                 硫如
札似脆仙나 .


        ‘
            씨I
                    Lt      I1 II
                         -.-t    -
                                     -
                                         Il
                                              ,1
                                                   1=
                                                          -
                                                               '
                                                                    和




                                                              13?
      8. 2       .        ,        fS6
                                                                                      小 及白 小艸乙 勺艸豆d
                 LSJ기 SI!
                                     L5口                          SI'

      石牙 V丁： V了 ej尹，
                 V2＋二0 .
             小
                     V1小 二0 :

                                         v_ =sIIvl- 十sI2. V3= Sii /1 十St1 Vfej中＝0
                                         匹 = Sr%.V,十 +S11. V3= 312. V，十 十SI2. 'I了 C夕

                                          呵二 sL1. v．十 十Sti V3t : S나 V,十 +,&. 呵a/

                                   V可 (t-5., ej芦） = SL 니十

                                         V3.-' 才，뇨 y:'
             也
님寸．
                                  SI, 十            옥：dj/
                                                                        =   口
                                           卜SI, C j'伊
       D叫
             的
                              ej中＝                      St!
                                                              :
                                                                                SII
                                                   iI
                                                                        (5nm51乙)(s1, 十 5江J
             1
                                               .
                      '                       .
                                              S/    ｝戶    r
             뇨
                                                                                       Ii斗니 = {
             小
                 .4/Lr＜中 小4<M才 ／未dl4JH；亡凡t才
                                                                                       1 &：中S侄 1


                 才뇨 力而i乙孕 艸尹白屈 牛 4 小꾸出＋
                              )

                                          1S:I尸 十a] 昴尸＝ ;
                                          SI! 六 + SI工5J + ! 뇨(2 = D
                                                                       k피           I S11   j乙
                                                                                                              1   5n    1t
                                                                               i512. ,SI기 '              1511-S띠 ' 小14-S미 "
                                                        72dl'J;
                                                              (SI：山tI2 = IS니 ' + Is미느 5(2. .才 H5i, S1 i
                                                                            = 키옥LI(2. 시C j2 = ]
HJ幷nJJ J
                                                             I si + s; .j2 = 隔LI ' 쉬S미 ' 十 ci:.2ic                     +.c11 S潼
                                                                            = !S미 '
                                                                   /




                                                                    ，小 /4- -4甘Hmm友d , 肛才 그 小戊I,
                                                       님，나皿 比뇨 ,,，且石，




m
n1r
  十尸 1圭Hmmrd겁켜a引
                                                       <l石了 /C M石妓凡／ 加I궂叭 /A立 4+,．山石m乂口， 和才3.

                                                       g.3
                                                                   꿋L " 如匈 竹 교끄퀴Sj                                必7r..5) = 긋6. c/B ,/

                                                              e=       /0尤胥岳    =   -2.
                                                                                                       is너 “中긋0._&, (.1) = ao. d8 /

                                                             D" " 勺岳＝ 似키풔＝和／毗｝) = 小.0 d. /




心 小 d 斗 빤 4 m d 崙 小 횰 昔 妊 堡 家 1 可 小 啞 斗 듣 作 나 于 ＼＝
                                                 느1뇨
                                                   a
                                                             工 “ '小끔＝口DZ刎S미＝크끄弓 (力司 : 16, c/ /




  뇨4i客노汁毖食Yg亡范莽m4斗11
                                                                                                 尸／/
,.   4   '


                                                              . : 8. 3 '口／B ＝分 P 기 S:3! : · 3g3

                                                              心Ti弔" =. 沁7
d+ 닉十 二 /L쓰 , i知，\ ＋加，(g./7).

                         Vi= jeVit = 4 383Lir
                         Vr; = c VJ 二 . 9口q j

丁卜山＼ 亢뇨 m和吃 平 力뇨 -4土七m{ 的尹乞 m丑，

             V/ - =J' Pv; 十 +K V4+ 二J' f1 石 十K !{3'
                 = (. 3g3) r. 9그yY12으' 妃 9교刃幻列在으' 二 . 兀7Lr                               V


             \／夕 二 床 V1' 十 十 'P띠十 =', VI- 十J'外'3
                 = (. 9교刃（17크）Z으 尸（. 3 g3)(. 3孑3）乙으                = . 加7Z브         /

和 a7伐 小／才 辰 m滅在/ 石 n智及 3dB ／少Aa-

8. 5=
                 Pt = 90 W = 1/ 7, 了 dB 力7

     工L= O. 5ctB = -i五- 孕                +   p= P - TL -          q7,D (/Bm =    歌9. 긋 1人／       /
                            口       rJ


                                             已        日                                 =
     a二긋DdB= -JO乙多阜                      누 已＝ 小C. =2 5. 5cJ8州 : .7口나                         /
                                rj

                                              巳       凡   n
                                                          U                             =
     P =35d3 = 0石므 F：늉                   => FL4       늉戶D= -5.돠／BM = .3 似w                   /       1




                                凡
                                1
 8· q W 幻兀 出가力力7 乂M 乂7，丑 C4k／毛勺．




                                                  n
                                                                                        3
                                                                        干12
                                                                                   =
                                                                              P3



     1
         V
             小
                     工2        양小乙      =




                 已               才工
                                        3下
                          工二                 口U
                                                  : 批‘硫）
                                                  =


                 巳
                                 宣乙
                                        D니
                          工l
                                        二나
                                                  = 士 喀／亮）
                                                  =




 쿠뇨                            근2 := 4-{ 乙／3 =         90뇨JL        /

                               근J =     1{ 큰O 二       / 又0 J戶   /


 rh4 入／4- ,w4盛尻咨 兀伊小 ／十
                                                                                   G似＋口I工／
                                      Z亡그 = Y3<>（知） ' 3% L小，

                                      근亡3-／死仄万 = '0'o-fl-                              ,/
 Th斗／A1 S叩M4似比仟 m                                               , ( P仙41 어／4 口才 30. i; 尸小止）
   sit = 絮｝뭉 =0
   s22_ =. 3에．120- q 0
                                                  므스坦 = 叫. 교了                               /
                      3이1 t2(> 十 "O               又'1十4'0


   S33= 꿴40니2.0 = 17.1 -120 = -.7丁                                                          r/
                      3이汁a十1之O                    (7.14내20


      【 = 月百e6 = 了玎스宣 = . g配/L二쁘 '
 S긱 = 5：                                                                                         /

 S카小시下万e-.& = 仄亡2r = .5o / 9 '                                                                   /


니4，亡；,C足， 比뇨 /yt土2二；）亡：
                      ／乙 X乙 Z肛m+J
                                 \ S미 " + 汪띠 ' + ] Sz可 ' = I ,
 月丁                        Sz3= S3：二/1-c 2刃나．g6cY e‘玎口 二 . '/33/                                     /

                                                         川．3
                k·     7   I
                                    (D



                     }::./2<nM/ ( '. 그f)
                                           '（了" 7) 1 Z乂丑 他凸七 弔 尺
                工伊mZ．月尹Z浣 比；毛乙七 』，;.
                                                                  =       3 3. 3 ,Jl.
                                                                            小
                                                                                        .7
                                                 且 O 1 L
                                                              r
                                                              L
                                                              J
                                                              r       n
                                                                      J
                F뇨m,.          (g.3이       /




                                                              t O L
                                                                      1 1

                                                /m 尸111111U
                                           工工
                               ［勺    =
                                                                      O
                                                                            1




               무 伊片 3 危 md左石d 口，a 戶a7 立 -4                                                   - 1뇨M기1今二I可'
                                                                                                            )
               才兀 나                      十 伽乞肛 .才 和zt- ; a44 ( ,

                                v; : 士 니十 十 2 喀 = 古． V, 十
                                V.3 " 2 니＋ 十｛ I/ f : 吉 ,, + 3.- 2 V二
                                                       L/
                                    = 2.-咐 + 七rl V; f : 士 V．十 (1 十士rz)
               小大A工 /m九； 和yZ万在／阿b ／小 尸寸 ; ／名4/
               -t노       C.寸甲쇼a 石                    伊才 '-I 屈，

 1
 dJj 1: 111



                               (?;?i :(孕
11i七ti1t1 h
          H1
           1




                                                                                U
                                                                                1
                                                                        근C그

                                                                                                                   已百
                                            뇨                                                              C>< =




                                                                                                     ‘月丈     21 = e1 十 근OJ
                                                                                                             Z2= Rz十 근＜>2-
                                                                                                             근3= R3 十 근03

                               Fm,      Fz/f73 ＝巴 加之 小 小 才 屈砂巴／

                                                       ZD2 Z;
                                                                        = nr                                                       . .. (I)
                                                        '2; 乙3
                               瓦， 4/i 浣二끄兀 的兀 ；仁／e如左뇨／/ m{ -'-
                                                               t4才 A4巴                                                                   ，
                                                       근口, = ,e, 十 乙ZJ
                                                           "              근i 十 寸．3
                                                                                                                                  1,         (z)
                                                       力   -          r9 二         근／ 근3
                                                       乙oz 中         tc2. 1
                                                                                   극 + Z3                                     .        1 1         (3)
                                                       7              C)  ,         已근工
                                                       Z七3 =          (c31



                              h/,e     仄44乂小卞＼工／ ‘乂刃니，T        귿d/     口mC{          乂       刃比 7d二中白凡； 크夙n\ 44／七
                              /＼戶-4之    5   兀＜加／勻卯m戶 ( 巳，足，只1 西勺
                                                                 .



                                                                 즈DJJ) 匕Z4功r y
                                                                                                                                         .／戶


                                                                                                                        今似辰小／
                              4寸 小J之. m肛／ <＞뉘上 ，竹口그4 J多끄d /           14 力 /9
                                                         i乙K : L(／工 /m尤f 나口幷之
                                                                              4-

                              X;t,e (a,，乙／，乂2力니 乂仙i,




}J盲｛圭立丘奸쥴荳旨藿矗七多＜4444］쿄a蛋言晏奮
                                                       2（》乙 西3 = 2局
                                                                                                                             . ,. 仁)
                              加友人C友 /m4乂／人-I+ 尤凡d d시／Li-.-- A,/4t                                /

                                                                                                      ／和小心4+ 口-t丑 꺄4낯                                    1


                                                                                                       !

                              盛      ,y冗a去石      202            吼3 名                  (t 戶고 m卒仁／石Y豌m꼬兀
                                                                                            1'
                              牛 2.」，F如丑 加七日 M瓦／
                                              ／加 加m協m口h 尸m庵 Zq3.
                              (4在 已4兀m. 夙／D)

                                                               佰） 力                                            Z3白夕C 203 //M吼
                              사C1』
                                 ．/     戶t,＜고／                                       比M
                                                 (1) 口方d                                               危



                                                                        /9    5-
                        (z), (3), (4') ·     丁hJW 仁） a助姃肛 /Z二，                        叫航脚Ad伊교)

                            尺, 二 玉·［Z.2，派 (s。  , -h) ]
                                                       ， 』M                     ［그a.工* /i （그근.7. Z;)]
                                                                          Z/ 二 西！
                                    Z<>t 4- Ji 己＞/     '                          2Oz +／二 근＜>/

                        m </   (3) 口斗낙｛ (YJ ／友e．人            ,i只二亡＜』比丑 只b,

                                   근 2 [ (20: 十／; Z이 ' H K 근力／ 근毗］ = a 2品 （즈02 士／iZ이）


                                   及［佃m乙.,)' . 面 0L]                        功 仁吐씨二 Z미
                        T뇨小 品ia4o_ 加戊 J們고나 1伉 匈 :
                               Z능1+ 加 佃二I) 弑 十 끔 伊D苡 十 茹（m2m)Zm寸a句                                         0


                        아뇨 戶니 已1 （교凡1, 似肪似m4多 仇m竹 Z凡 戶似m+




4H賈肖往好寸弦管聲毒ma411! J社싸
                        和口 們m友 好m니，元뇨 m此母 九泣 呱衣
                        加／力 戶／ 乏O), R乙 R力 ma 尼 .
                        EXAMPLE :       끄斗 균0% = 1/ 文＝又 :

                          r1\J叭1           귿돐 + { , g7- 1근三乙 ＋근쵸 m . gzf 근.2- 4又      =   0


                        1뇨 才寸亡出亡乂            d2      근0l :. 87a百               (VLA   4P-I5C C川‘C-.내TCR)

                        TM\/        .      22-= t.(＞仕1   ;   R工 =.1仕7$,

                                           Z3= L6나77 ;        R3; · Sz85 j      근o3= IMSZ

                                           Rt = .362I

                          C土土，支，.       근A= R , 4 근d123 = Lcoo /

                        (tU乞：才凡伍， 口샤， Dt/J凡， ：小砒加， 力1 力，오 月，凡土m 浚石肛叭
                         石：丙-d. a03, 的 a뇨 尸加小 中mM如 · 4m工 伊qM李
                        才托寸 小4-.-, 和比 a 肛샤毛 戶七在才而 肛 名珏／근1= ky“근2. )
           1. 7   月t石万七 (了．37) ,               K느 艮／P2. = V3   ＝수＞   卜；＝· 577


                                           /3/ . 7_J7_

                  Z02. = F:3 乙3        = 4,工 7 끄

                  P = 근0 r卜；+ '/K) = /／드5JL

          rk皿 따   才 ／냐d4似＋ ＜그4．工 /
                         ／근 2 = Z0K -=          .7m.

                         尺3 = 乙／K =        g6. 7J-


                     1／二        尸2.




          （加毗艸笞 .
                                                                                \
                                  和左 加               如左凡出 싸肛九＋九叱／
          辰 m初戶左／ 됴 似n婉 尺 (戶小
                                   征也 肛仇／小a)
          T뇨十. n "V3 , M ／兀 小4石乞 疋 蜘油파뇨M/ :
                   尺2.

                                       。L.1申士 小mm畔 竹小4. 月m才
                                           土 = 옰 *옳
          P0l甘t七 d小am, ／工升q小元凡才 已= K ' P:
                           ？乙＝ 士lti나 ' 已／근쇼
h
L1 1H뇨h                    p1 3 二 늪It히2. ,-,3／吐3 - r ' 尸노
                    난
          a뇨               므끄
                  Fr g2- - g뇽
                                           )
                                      民늡




                                               尸／7
     cAAo                      , 노 = Zmm十K"J                                                ,，· (, )
                              乙3 二 근. R3 (1+ yKD

     F九 쿄卜d
                                   mm／万仙円                  J




      否뇨4二 "'                                              m1警， 客
                                                                ，(j+,)
                                                                 R2 (L十KU ＝尺Kl                  . ..(3)
                               Y2.=0




                                                   甘레曹R,
                                                                        f   fg31tY)
                                                                            e3
                                                                                 fl/
                                                                                 (,
                                                                                      (,
                                                                                           L)
                                                               R3(t十K今 =R                          1 ·，臼)

F-
       d4,
             \
                      (3) ‘，묘 (yj         ，七A八‘   뇨2十t X沁寸             e2- =Kl只5,

小／{ m，쿠 師乞 加皿 mm뇨 力 M右4 乂凡 如和
工們A九뇨· rm                                      m功뇨닉 石 力d 乂九 m和牙／
                                                               甲力뇨片
已，巳 乂之 功加小 河丈幻j m年士
                    仙机                                                                     b 兀싸小
卜m X未t44休刃 크乙씨肛 尸枷 :
                                                  J十 4 刃好石 孑如끄r 才知才

                                                  千-j쀼 ;「 “ 뇰老
缶            只不工 f加孑七 부 比／比 南亡＋ 力功才訊dM/工 m냑小 r 4
샤枷a 勺 ，「， -_ -日뇨加 근
                  【 M 귿， m 小U小少／'
                             Z士L        t （그

년D
             面 ,dH=；出그．
                 //    5 月         ri




                                                                0d
                  ‘닢寸 지)之        C浚力力d工』     2亡2 2亡
                                                  3 J-
                                                     -               = 寸乙R. 교乙e3 - K乙R}
                                                                                                          )
                  刃r   c小． 兀汕，兀 乂뇨 ／肛仟叭 工尹
                                           m九沚 :
                             R乙： K乙 /        ,- 毛2: 근。 l( ( + c') /

                                  「「 ; 乙 =나 當'
                             R3 “和／
                             尺 二 근쿄 (+ 가.)   /


             gd!        未衣5 4品 ". 7ZmW (g'. qob
                                                );

                        （已' ( " 刀；
                                 ！』 ' 戶響 , mz 2' 三
                                               ．  , 蜘‘즐互        1    1 1/
                                                                                                :.
                       0 汕Wd 口f4而且 )                  (><e= 又 r/ 3                  ;   oH = q , /j   :
            8n/
                             /6d 측智）／챠 2-lr三                    a％才 2       加   的
                                                                                        t   쯧
                             "      "            （丸             可／3佑        1
            小i오 근！.＝毛P1I(0已 只Y沚
                                刃뇨규和뇨
                                                                            M 74也的「
                                 （표 ' 孚）烏"뜯小
                                                                等蜘’쫓＝.
                             (3甘，꺌) 小'쯧 H 쯤m．石4-'' 쟐戶
                                                                                                .



作1444笠貫茸玉
                         .         3七： 小‘뜯 , 쇨1
                                        브老   瓜   갛          /
                                                        1
                                                                                                              =


                                     쯧
                                             入石
                                                 0

                                                 그                  7弓t a＞凡／2 m弘)                                 H1
                                                                                                                       <
        未／又                   Ct = /. 57 뇨;        b . .790c

                             f =/／口作斗 乳＝2加，'t --J ; 肛／
                                                     ／小y 似－'
                             근'0＝朶. 和／P = 7y白2JL

                             Pi。= 4b/210 > l.67xso中7 w

        f乙i刃口hm (            7,9U 碌工 肛友니 7 澎J 白柳石늉 伊me                                            /4戶／


                          , 즈互 = ,71- _I
                         小；               a                     -   . 86 7 ＝各      S=.33 'a: . 52gC叫
                             0           L毛뇨L
                                 " V勿r工中毛뇨L

        T뇨W, m咨＝·7了그 , 帥咨n그y8
        Fh           「   『   初d    '   ,    ／誓1:        .·   ／

        Fn4n,.,              (z사Ob)          ／亡 뇨中
                                            月／    ＜)


             041 " 景rL . ( 瓜' 즐 넣缸44咨1俗b'要끄 r。3

                     "吼 ‘［琺心 ／紫拿（4饗 ‘若蜘｝픗）]("
                                  i . G7刃dg 二3d乙)ciD’勺23
                                                                             口＝t        /n二切H늬
                                           r;) 二 3. 7? n.．却'I                녑1r       中0中nLm\

             y. t3           f1口 6-14舌 J' 匕t=151（似 ;                t,= .79口CM ;      C= 3吐.8

                         缸3g'· 加-4 ; P= 293·3m" ; 2,尸乳7才= 95'/ 皿
斗나뇩U1
                             f札 = 口山／2Io = Z?g7(,;-' ＼八／

             "뇩m回（" " ) 元仄'．柶山却才小四" 口笞及 .4 （戶 ‘．“따")
                                       ed也P= 札／下＝· 7. '                 方       万= q3 "    "
             P,l七- - (g사司 乂；
                           ／匹 a-.'七才k.，兀 力4石乙뇨＋ ai :
                     小기 = .1531, = y屹勺丁" 브 '/ <－모乂 . 乙6r? ;                     二＝수   昭＝ / . 乳工加，h,
                     t A 1         3瓦石戶

                                                             /50
                                 [8. 씨 I                     f: ! 7.5&L4 ; n: /.5g 師·,
                                                                                                                     b= .79c c      ,· f叫 (g뇨在)
                                                     朴364.5M.. ; 뱌均9似나
                                                                       ; 亂 ‘丘枷／주：yyr. 8平
                                                         Fo                   ／큰／. 二 工7오x加口皿
                                  F/l亡）,./ (g．仕D 4J J                                       4A1：才／t       S= 口』
                                                                                                              ／교J

                                       } "4:    !"
                                                             3y1。   f。
                                                                                  ！【，
                                                                                              "   刀니＝
                                                                                                              9.
                                                                                                                   59加 '
                                  F,
                                       -   -
                                               ,V        (
                                                             '.   5{     )
                                                                              ,



                                                     e: 2'd8 " "" 白1 卜                                                                 八／


                                                                              C
                                                                                                                   似丹- 2o -珏尸
                                 尻'- Iv= 1,                                  사든汁
                                                                                        시



                                                                         k
                                                                                        似      / 十9 ＋石＋y+/ 二 ／石     =
                                                                                                                           J /<7中

                                                                   a0 , _"c,,',
                                                                                                        中aD工띵＋ 十그/: /
                                                                                            液 = 6. 5J Xio中 7
                                 r/ tdhnr            (g·5뫼 力뇨 甲磁n兀 /mdr
                                                                                 0; m兀，
                                                        r; = （朶Jy3 = L口 似h,
                                                                            = nf
                                                                  V; 二 （呻)Y3 = a,974,，
        1
            1
                1
                                                                                                             기， = G
                                                                  rL 二 (6液）V3 = 已97 m1 }14
    1
1
                                                     .
                                 Th兄 4伊心；芎 衣加어
                                               才；뇨 y＋彧따                                                                       /4- 人p'q “万'/ 1W枷
                                 (J似Li伉 甲泣i뇨＋ amm似d才
                                                                                                                           / S“羽 如之恥況）



                    J니




                    4dJ11n내1며니




                                                                                                        ／旬
&                  5
                                         5g c14, .'   C-＝그0口／D ;       川二q 臼뇨也） 5 q,.A二 3od6
                            a. :/
           1
               /
                       毛＝ 36白5- "- I ;                多 =307. 7 H* ;    극，, ＝亨q夙S且
                                 尸 M/
                       pl。二 그.7旴八；

    F뇨亡h니 ( g.90口，1) a,，江不
                          7乳
                                                      若  S＝可乙

          1K디 :
                         3小 FJo             1 - 쯔：d = 9, 5? Xio
    F그Mm （乞5?기
                                          乙夕司
                       加dB= D小 = 又0 石予 7刀n，
                       r나 (4J（尸니 = m4, ［斗 C們4d (4叱Pm)] : 3/.
                                             겨比＜. Ph1 二 /. 587

          F乙1可h싸 （巳57刀

                            C=2.d6 n그0／胥附 ( -如乙万表臼.
                                            案 = 3. 北xIo巧

          1二人口h凡 (gs6) 山乂 r4.6q/ ) j
                              '3] : 案 L4JCV日州 (C伊449 + qd寸．교尸十3)
          久［！了 鈿qb .t-r尸白4ad 十V
                                                               H94J亡＝日M 仁4- 그尸#,) i-i]

                       그r丁＝次.4AYOM 斗 口＝ V刀 = 二／7,力｝H ·
    ．和/
                                     .         ..




                   a r3 , 泉 [H( ‘妃YC, )n 中t4L乙노日 斗 r= r 二a. 9d
                   及 r? 二 矢［크肛（116나 qdJe그叭 十日 方 r; = 元돠
                       尤뇨 甲才沚 日：也 却/ C -S./7거 枷 .
          rh七 갹M뇹 流友k斥

                        C      Q o Q c
                                ri



                                                               菰
                                             0         0
                                                                           창


                          T뇨 加m나 7-.目. 戶m+ m丑，
                                                                                夕m 7＝的， y朴
                                            Er A枷 쯧 e5恥 =O
                                            出
                                            『＋,A丘警甘了P"' =.


                                            H茗 胃令, 蜘끙eJ느 西瓦
                                                                =
                                                         j irA n-.;P5仇
                                                               C'
                          Pm = 民b／근／D
                                              ; 근1O: 帥.／尸 -
                         E小 佰'口7）그" I3t) // o 伊m쇼4 和也十吃니 如4
                         口，11 ;         （不＝劫
                                                       1   =o
                                                                                                        .   ,



                                                       주瓦 = m乂，似 H平 S(/) 묘少可뇨）g（亨和）gd r aM



                         f:      e'亡
                            _-rz24
                               '  4- 亡二上＝삐
                         '4.占 寸，1．晥 ·J'叱凡知 = -J쓱프小쯔뇨J뇨 .
                                        '                                       L肛 亡／oj 니           "
                                   = J 兀工C＜力I人
                                     F,O a?'-. 01? O


                         '4; 十，尸小LI回吼瓦d寸
                                                                               느二
;＜니HJ니片1d口4J4 d
              (4J1브4dj
                                                                「     二：
                                                                                 ,   .   -2;
                                                                                               韜』
                         丁k吼 力久毛 ／各Z訌 -7毛mmM{ 蜘乂 /M乂切M
                                                       mK
                         a샤石泣孔4-. 和札 力才 口戶m；小
                                                                                         氏f孑，=. 나           甘Z
                         LI.八乏，:




    Jdadd自겊기n二add너計느
                                                                    /53
                 A ,十, =    / /" 小  ，H
                                       (    그）
                            P1OcL "亥·小

                            J' 兀t乂mA             十e'" 6d)
           /＼石
                            P。
                             口l毛 小
                                       (I
=h呼                                                    = o.
      듀그／ A;;                   枷｛ m四才 뇨11之 乙／十e．勺'PY)
                      二 0
                                                                             &그／


                               -r卜h X小乂 m畔） 7乙七右，

                 C-
                      = d;i0
                                                        小 따"毛仄 j
                                                        '        ;i7r느h1 !

                                                        C/
                                                             B




                                                 ,/59
                      뜨           乙                                 Zb              균
                                                                                        ＜>
                                                                                               尸＝
                                                                                                    F\
                                                                                                    今

                                                     Za                        Z4
                                                                                                                                  反 :        巳／
                                                                                                                                                    &
                                                               倫）
                                                                      "



                                                                                    乙          玄                                 ／납 q= 屯／z아 b：근b/Z.


               FKGW七斗 7i化 如午仁 쑤 加Z乙니 了，'5- . Tk                                                                                                     ,/q／七＋4日
          M乂 C乂M机&光4.- 口八允： （枷MM
                                                                                                                                                                m可
                                 4i쿄 7易小）
                                                                                                                                                                1
         뇹 긋, L ' .iAj-스g
                            口           4                 恍               小4                             "누                 J 4숭 (t ＜工 A/g
                       O    乙
                                        d ' C.                            45, j/q                                                 Sc..            S.C.
                                                                                                                                                                Y5 =-J
                  E三VE三p'.)                          MoOE
                                                                                                                            ODD                   MODE
         11皿 人8CD 4,m九aA- 口月丑，

               [A- DJ
               Lc  .B1,e 1'/。口比侃C，亡뇨， Jb                                                                                                 -b/ct


               侄：],: 1-(:i.:i/& o]['SoL/b 孔04兀，,
               re: A+B- C-D                                         小 ;(b. yb+ b/h9
                  A +5 4- C. 十D
                                                                          -2b厄＋j (b+ Yb 小 b／口' )

               r; 二 片十玉七-D                                            j '(b- '/b :b/aO
                      A +b 十Ct江＞
                                                                     그 b危 +.1 (b+ Yb- b/a')

         丁卜此 -4勺Z肌；乞K 寸                                                     和十 / 4                               力m ,
                B尸 느（r 4- ri,) ; 三（b士，븍） -ij(b『吉’「"危9                                                                                                    二二 0



！半J！ 斗
     J
     1
                                      " （쓸）' +n＋言咨）"
                  .         나｛; ＋흐； = o
                            11D
                                        工b                +
                                                               브士          O
                                                                                        (ca 뇨小（                   b         上b
                                                                                                                                  知      匕
                                                                                                                                         ／         m             l   하
                                                                                                                                                                n
                                                                                                                                                                D        / U




                                                          b
         닝寸／
                            a     二
                                                                                              m
                                      1d11                                              1
                                                                                                             b
                                                                                                                      1 1
                                                               l
                                                          LU                                                                      D
                                                 /
                                                                                                                      1
                                             1
                                                                                                                      i
                                                                                                         코
                                                                                            /'55
/                                                                               R
                                     그                                   b
                                                                         百      晴
                                                                                              브才
=
                              A+ 8 十C十 D                                 丑      必                             쁘口           勻         1
                                                                                                                                     6
                         L                2
)
                         =           11                                   -              I

                             碧b+亡咨） 卜jb
    古 ／뇨 口V牛니才 枷싸乞 師굔汝4. 4才 和泣 긋 口.4,＜乞3

      '   =    (T
                    "    " TO'   )   "        "        [-
                                                            -b/
                                                                   I玎5          "   b1
                                                                                             I小   j   -
                                                                                                          ,
                                                                                                          b   (I4h/
                                                                                                              ..      -J
                                                                                                                               aL)
     "3= 士（
          『／."）『 士［닒，』 뇨+jb ,汽，)
    Tk        ／札小 4 7.' 尸如七 ／札片 衣加                                                                                                       肛危 又口- dJ.
     F示， 甲a,4b 亡 口＜ J
                                                  P二 = 口＜ P3

                                          lB니＼= 'dm尸
                             t = k/a ' 수                                      a- 二 石iH dn, 근0 = Y二二 aO                                       /

                    b=
                              a

                             兀區누'
                                                  :=         y;7
                                                            /7二               U퓨；                                                                 /
                                                                                                                                                 느／




    Cht七支： m사J,J,\                   o= I                         玉＝근0 /                 . 근b = b/ /i                      /


    a才 奴工 /A毛表a Pr身．
      힉 = :: (re - rO)：士 (b ' lb 十b,/q' 乂·） =.
                                                                                                                                                      =




    나닙：g ．쫓：+4,，人 ／乂－ H4知在力而．
    (1。
      -L, 心3                 (6d也 已＝5乙니江 J                                          乂此 A小刃t 瓦＝ g7平／ 已 = U乞L
                                                                                                                                                  I


                                                                         / 反3
                                                           6r = 乙 2.

                               乙e = 兀．工戶 ，·                 근Co = 竹之j11

                       2d .   fi; 乙e＝加Y                     ;    'Th; 근如＝ 59.
                       F.       似     g·
                                           又9,
                                    S/b z . 0 75                :＝수       S = · 고Y 入ii뉵      V

                                    W/br                 . 67   =>        ＼戶／ = 工／ >, ,,,   ./




                r;；小
                   =mH
                LH1:
                               Er =iO;               d= ./6 Cm1            h/ 乙／6 C.1人           S =. ＝拓 f C44
                                                                                            J

                                    w1o          =   I

                                     乳／= . 꾸

                       F小뇨 F4之 8.3이
                                                         근De = 6／느IL

                                                         Z<> 0 = 3 드戶＝




心hhk뇨h




J在J글n느注通二汪




L4茹心上七出m出出m翡m
                                                                 /57
            g.2o        ；毛乙 口， 그初寸m刃ftt足 ／나兀/ 工뇨 臼尹0/＞石似』/i,


              C,
                        ;rf口
                    C寸I友1 邑42(i-

            EVE卜J    Mct'E ..                       1- V               +j/
                                                                       0                    "二J '豌
崗
                                                                                                 厦 : 平'
                                               3보
                                                                                       oc    =




            ODD     卜40D三 :

                                                                                            C。=Cc 十 ;1- ce = 3Ce

                                                                                                 =     37r



H겨기JJ世川J바
                                                                                                     (：力，14cf 芎乙ia

                                                                                            근的' 匡 七 .“，'
                          .)?)1I)      1   ,          Ct=      /SIi枷         )



                                    C川m,/t"i 5/Q (2, 二 . 96그


n好                 Z。
                    c
                        4了m치： 377(.r7?‘刃 = /1缸                                                                       1//




                   知＝ 加근， r. 96그） = 377(.56刃 二                                                          3 8. 5j            /
                                    3lr eo                 -                     37r
                                       드-        0   Hma


                         W..+ 會                             L了·..
                                                              ! ' 1근＝
                                                                                      -,   H＝尹
                                                                                                        @
                                                                                                        md= =＝二＝그나小八커
                                                                                                                                     @ Z,
                                                 Z0d
                         4V 尸）                                                                                               乙口
                                  尸｛4                       尸＼八人二lm
                                                           @己 =
                                                                                      4Y
                                                                                           -
                                  e)        丁，
                                                                                                        ---戶H卞戶m1人人人二1m

                                 4.7    H二＝今＞                                                           (D.                  lb       @玉 =
                                 ！고                                                                 나           .       1+




                                 EVE시       卜.iotE
                                                                                                               oPD                MOPE
                             a = 兀包

                             r : 좌屈名 , 乙二三'
                                                                                    r, ｝쯔Z느흐 , Z品 - ZJ
                                   乙늘／2. 十Z.                햐十Z力2.                             或左，+ Z.                               z品 十 ZJ
                        f4b] =
                        LC DJC
                                                           jZocJq，
                                                                 日“               f A. B]       =       fq4夕                           J 근乙a 小ke"
                                                             (b4 9                  cbJ , ' 1j小 小kt9
                                                                                  1 C l> 1
                                                                                  L     尸J 0
                                                                                                        1
                                                                                                        1 권니 4毛
                                                                                                        L 근
                                                                                                          /=
                                                                                                                                         C寸4夕
                                                                                                           ＜)＜그     m




                                                     d그
                                       ' 小' 카릎h亭，尸6                                                     如＋多勺／誓 嗟升兀夕
                        Fh 口M 口놔此ae 仰K- <，汕d .如m
                                                 , ，存工
                        며耐 枷 e 놔1老aZ斗 ae)
                         B『『 늘 （巨十r0)                                         B: = 打兀 4-Ta)
                         &" t . (E兀）                                          B尸 打乙－T, )
                        古 a凡 4y乙d吃거' q／肛才／ 4,
                        已＝古I己二－ Z了, 卜 갚出" -] .                                  首，乙
                                                                                  【, H근V
                             十1" 乙늘 午근：:                  尸 근誌＋캄-I "-       /;, .二工
                                                                                  , . .느
                                                                                       ，', ,.                                 二＝ 0




 4 b과J444寸4發41JJ: :!r
                               " 나＜   '                     나口 " 니 "        k,＼乙勻．(．乙',十M)




1
41
                                            召으＝ r죠e2的                   , 甘 4取 肛左 口八丑 4M石在凡／ //


                                  弩『夕
                                    ，9 i去 냥＝) ,
                                                             M          加   0
                        石了    '1e 二 丁口 I




                                                                        巧'7
                                                                       和脆            又   (ha   3   ＜기比／
                               Tkc a卒44                 切（+      <i才



                               8교 二                쿄                                 1

                                      ' mP아警；旁，）砧6                         白뇨，少J' 智少' 序尸

                               63: tr乙C- 小· 乙사如］=
                                       I 西e十200        a。十 乙el
                                                                       乙e m 근00
                                                                       乙 e 十 근00



                                            e m 근O O
                               品才 C = B> = 乙
                                                  乙e 十 귿06


                               丁艸小      iji小,,2. =      긋 근.
                                                                       1
                                                       죠C 十 乙0




                                            D2
                                                       派：;H m P 可小A 尸
                                      8＝기；
                                         ／그) 比kQ.          出뇨a                 a助戶d机44+ 4仁 j
                                                 83 = C.                       1//




                                                  6a= -s V 1-c "               I


1411111                                                          (f·i司‘(8沾6) .
                               幽＋j休      留池 小i光友
1




  d 4 4 寸 V 뇨 尸 k h 끼 거 UL巾r




                                                                           和
                                                                                                       l/
                                                                                   Jo
                                                                                   /D
                                                                                           -i9.
                                                                                                             .        a
                                                                                                                                                                    j   于『 오6-14舌,1        乙 =60JL
                                                                              c-
                                                                              C-
                                      Fn石h勺 (g. 97).

                                             :2       1-                    r=:；三m -
                                             CG e. - rO I-．中11-
                                                        V ／戶 C
                                                                                    := (c) f. I 工_
                                                                                                                                                       師 “ 죠力万 = 53.7九
                                      F70L 4土i규七 ／七-t才人                                                                   6r 二 .2· 그                            b = . 3그
                                                                                                                                                  }                        C셔느mm    /




                                                      'I귿；乙e = ". 5                                              ,·             'I耳 。。 =7?. 7
                                      F- 小m人           F.         t    知


                                                                        두／{;, =. 36               ＝수                           S =/./-                끼． >1

                                                                       w/b - .6cI                                           ＼八／ = /. 9 그


                                     Tk工 /q比 石們W M兀 ,
                                                                      入4             n
                                                                      H立． =
                                                                       1f
                                                                                   .H늪＝．卜 =                                    c . 3그            )'l   1H
                                                                                   yr匕尸 f
                                     8. 23
                                                                            C = /0H自伍0 = . $d/

                                     F乙t4H\ (g. f7).


                                        已：        ’         곱屑＝                     /oy.          ／山
                                                                                                                                            玉O              =                      = 3% 6 m中


쓰                                    rhJH八／
                                                      ' Yi; 乙e =／了'a'                                   )                  (       Z.
                                                                                                                                        .        =     5-       /
컴
i




느冬宅dh心 dd煎n崩嶝町斗a4{ja4144J4소1小七十七미a
                                     F-i寸M 7二bM乙 夙a7 ,
                                                                      득／b = d:)/5                       =>
                                                                                                                                S 二              · 09了 "1 力I

                                                                      W/b 二 · 3,                       功                           W= /. 그5


                                                  /q1=                口m4=


                                                                                                                                                 千4如字
                                                F가 VI( 配 V1。a- 和J /, 加亡／瓦a 戶／ y뇨 m 1』. :
                                                      m               缸
                             %
                             !




                                                                                                      Fe 二 2口 -. 2。e
                                   匕e                                     r
                                                                                            丁
                                                                                            2
                                                                                                                     Z<) 十 乙 C

                                        中
                                            0                                                            1 1 r 中           ;I 근口
                                                                                                         I r, e. -
                                                                                                                           及+ 乙e
                                        V(}):V,（           丹十Q e」‘尹孑）

                                     n = 나－戶） : V* (e戶十U: eJ口)
                                     V2C: V(D) = W (I十區）

                       님寸，
                                             e
                                             2
                                            UV        V1e (/ fre) 二                   1 놔       ; Z, \／』e
                                                                                                                                       9
                                                     ejd十fl. "                                                              .)e口
                                                                                                                                   “
                                                                 e
                                                                              （乙十근.
                                                                                                 .)e戶＋       （乙모.
                                                            Z＝니e                                   근C 匕e 42乙尸


    ＝느m忽汭노！
                                                    근. Cd1 & h：乙C/h亡y                            已 十，I 乙C. 蚣口


                                                          \／그0 二          乙 吼 44｛夕

!!,                                                                  乙 +J 玉O 立M 万


                             丁hh 싸M껑 (g.77) 口M 乂뇨 九恥M在 戶比出笏 (8,79) 炒                                                                                  ,

                                 V= V           -V그. =      乙V꾸e四                                   I 乙＋j근妃品伏日                             乙勺뇨.立m夕-1 =o /
                                                '        ;l귿O 4:j（民e 十在U乞．尸 L乙勻 面e 乞O                                                           口j
                                                                                                                                           乙玎玉.瓦．




＝니1小J려發d4泛d나나＼ 111if
                                                                                                                     召小       \/
                                                                 7乙＼/4i亡日
                                 V그 =\／又C 十 V교0 =
                                                                                                             已e 十 古O

                                                          二 2O 十J （근.己 十2‘力） 乞夕                                     7 ZO      ,'
                                                                                                                              L ＜夕t7Cy TJ ／尸144U
                                                                                                             ZO＜二十 근口0


                                    小               " ' 'I／小＝'                              /               和心』／二구 =                         그2.
                                                                                                                                           乙C 十 Z亡C
                                            r尸C'"         C才力F+j／거小C;
                                 C 之 2S戶d6 ,            六／=3 J     乙＝旬) _1. ,                        B!AIO Il 月1.

 F4小VV 作.9o) 口汁d E不4m十／乙                                           8.8 :
     戶        ,.   } t'3 }
                   i             4


                                      그 4小， 今                               +
                   I V, I                                                                                           C3 = C,
     1m
          -            H11m1
                                 H1
                                                  [C,
                                                          口4긋e
                                                                                                            )
                                                                                士C.
                                                                                                2]
          = Cl4丘3$ 十（cL -c,) 4瓜
                                                                   &        ; 和P=m, e＝乙”Ca’교ci

 플응＝[3c1 C4-4.3& +(c1. .:,）白1미：,* :.
 募＝ [-Ic1 拍크C2피싸미，,, " b"c, -노 ‘ "
（又丈 和／a行m/ (6：兀/:iJJ C。＝/d1工可'0= . C56.
                                        = Cam2d/

小毛4了 戶 乙， C可 "
                                         .OS4그 = /OC._.C, ZSC,

                                            C1 = d3 = .0D703
                                                                                                                              \
                                            C. = ioC, = · 07o3

V4；勻 仟 .gij 9石奴 文／4 JW竹 m니r M/ 如口在
C石4miim力-C. ．烏們枷-I'比.1七 口4,

 2品 = 盛 : 이專 = 万0. 35JL                                                                    U/




킵. = 근큐 : 근在弘 'q.
                                                                  6$4                 t/   /



乙듣                     乙，I)쓰CL              =   5j . 6JmJ}m
                               r hC
                                      i.-


근瓦 = 西 ／'1C'                                = V6·6D，只．             1/
                                                                        r


                               r H- C工



                                      作． 和多m4m孑 d4寸 P石才往／ 口九 크不兀



                                                                 163
如


                     m
                         t
                             1
               2
               a
                                 1
    =
                                     1
                                         n
                                             1
                                                 1
              -24-

                                                                   \
                                                                        \ \
                                                                       \

              -26-                                                            \
                                                                                       \
              db                                     叫                                     \
                                                                                               \
              -2日
                                                             /I,
                                                                                                                                如
                                                                                                       1
                                                                                                           1
                                                                                                                                          1                     1
                                                                                                                   2                                            4
                                                                                                                                                                                    二
                                                                                                               1
                                                                                                                                          3
                                                                                                                                                                                        나
                                                         4
                                                                                                                                                                                            1
                                                                                                                            FPEOUENCY                 CHz


                                                                                                                         사＝3 .           Id8 EQ0月1-中尸／尸比E               J 근口 = 50j.
        g . 그6                                                         C= 25dB J

             c二兀口h- (8.9口） 蜘（ 乏7m寸也 了· ti

               e                                             V3L                   小               .                   ,, r -                 -   ,         a       =

                                                             W! ' d（夕小dLC1 汕只F 十 tdU
                                                                = C1 4瓜t 3e 十 (c그4C,）在닉夕
             凸nJ床m그，', 小e /（刀md/ 그짜 克十 工4/mi毛 光2뇨 2늉 4
                                  寸     7                          /    '

        CJ＼丑J시4二上r 肛ZYm万k4i4L) md 尤뇨 ／的材 才｛0表 /d4工
                                                   丁A1 如뇨‘Z
    .4k在444工 C 汕， （乙 尸寸Zymd,d／교 ．力；t 小41.日 .
                   （ d7L ;t：矢工 口닉Lm比 7易-z_,_._ 戶 a) 4 口1 ,＋뇨呻 :
     A24尹加4工 J 蜘4'i力

               十                                                                                                                          上- Qj 9= X7a ', c, :-6d8: . 乙了口／
               4

             나
                                                                                                                                                                    '              그CI
                                                                              /\
                                                                                                                                                                             C그H
                                                                                                                                                                         =
        十2
        「
                                                             「 玉72.

                                                                                                                                    j,
                                                                                                                                          Lj
                                  丁1-助， 力奴 m 놔   m 尸初四毗力乙 ，磊 旅左m仙
                                  ／小 戈／但 m知在 石L     VV丑 Ca-1「 m弓 石 又兀；
                                  却 流mMa如-i- . Th工 4M私似
                                                            나 小及t 牛 C ai
                                  C和-4戶         -aqdB : · 063/ . J-c 加
                                                                      （ C亡M們／-                                           C- 刃4 P,
                                  戶 刀mm 切辰奴 쿠 ' 7, m虎取 C. =.CSO/ ‘』"7                                                             )
                                  m心3 4 4如尸e e亡H尸吃
                                                                                                  沙戶니 7 m亡／尸m左 cw C 似心
                                                                                                                      f;
                                                     . (> 5.i 0
                                                     . 06 3 g
                                                     . 0 6 工5-
                                                 ." 3; ＋戶 口mJ比才 小恥C 끄I,亡／
                                                     C1 = .Otq5            ;   C   = .Og＜了I

                                                       Z丸 = 50 .? 8뇨n戶                        ;        Z品 = 竿9，口3 －凡

                                                       Z亮 二 5부．6? .JL
                                                                                              ;       Z晟 = </ 5. 73 J乙

                                  丁k且 蜘구느 作· 戶伊小 4 斗比／小命 ‘
                                                쌓
                                         -20




                                         -22




                                     "
                                         ' "卞
                                               乙／
                                                7/
                                                                                   \
                                                                      \\
1口나4質口K薑立m恁嘴骨資44m
                                    11三 6




                 미川14휼魯嶝d臂磊發筋4
                                    -30
                                                                  1
                                                                                              I   I     F
                                                                           2                      ：三               二
                                                                                                                              :
                                                                                   FR드QUENCY
                                 n庶b琺丑 和小而.4 ／
                                                                                                            C！
                                                                                                             已Z

                                               幻                                    似뇨伽航／M 戶 而伍／
                                                                                                                              2
                                                                                                                              工       r
                                                                                                                                      U



                                                                                    /6   5-
                                       g그거            F4旬仇 (g.qg) a1a (g. 99)                                                                    -24，七 Ca机 和뇨W -乙初／.


                                                         근태: m프C-C
                                       E沙力客 ／乞／毗 石                                                         作·97이

                                                       7J匣：空少｝，「，                                                                                            人0
                                                                                                                                                                                           民e




i寸：   1 1j4 14n甘忙毋큘＃聲놔喜m田好注mJ11a쩍H41
            i '1乙rztr4才白之 (g·79J 戶 小6 加 吃似                                                                                                                                     /               근的
                                                         3 a (Z쇼 十근.O                                           十 aC 근.e乙力 二 3 (旒 小鹿幻．

                                                         끄口，.) 깖e 十 RC 已e 乙O 十 3CC于／)군品 =0

                                                                                                                                                                                           口
                                                                                                                                                                                           ／    꿍   C     2
                                            7. 戶： 中7C Z的！/7/ C ' Z品 小36(: ai) 근aC,, 尸 -C- V? 小召C2
                                                                                                                                                                                       1
                                                                                                                                            ／
                                                                                                                                           寸小
                                                                                                                                           H




                                                                                                                                                                       3
                                                                                                                                            드
                                                                                                                                                                                           C
                                                                                                     )
                                                                                                                                                                                       y
                                            1卞   \/                =                                                         =                       1




                                                                                                                                                                                                    \17
                                                                           (;




   11
                                                                                                                                                                                   /
                                                                                                                                                                                                1
                                                                                                                                                         1

                                                                                                                                                                                                /
                                                                                             戶   ／
                                                                                (C
                                                                                                                                                                                   (
                                                                                                                                                                                   1




                                       cc柚工 m好石或毛 m才／似尺 西巴 吼d 2的 虹肛机m小<I)
                                       a派才土尤智 戶 如瓦 而琨力 小e 刃好如 7毗勺

                                                        7Y平 亡口     ：仄三 乙.
                                                      뇨「寸뜯 ['C(,-?／可'目 ) " 小"]
                                                        = 군, 厚C 仁9C'，伯d「固十아m汀유拓"
                                                                   ! ' 口                                                     ／긋 C ( C- i)

                                                                                                                                                                                                                     ==

                                                      之
                                                             乞                                                  ?
                                                                                                                U   十
                                                                                                                                  0
                                                                                                                                      戶 8c 2



          d 甘 4 貸 客 斗 于
                                                                                                            戶
                                                                                                       C
                                                                                                                                                                                                               1




                                                                                                                反
                                                                                                                                  J                                                                           H  ?




                                                                                                                    C
                                                                                                                                  /
                                                                                                            나
                                                                                                       /
                                                                                                                                       C今 ,C 小比毛 平玗Ma}
                                                         口
                                                         帥             d    /                    ／ 民
                                                             J


                                            쑤
                                                                                     V



                                                         m
                                       /。
                                                                                                 7


                                                                       口
                                                                       ／    \1/
                                                                                     \1J/J
                                                 亡           /rL
                                                                       口
                                                                            口
                                                                            口1




           뇨H꿈月1寸1]
                                                                            1
                                                                       ／
                                                                                                                    7        戶1       二i        1二
                                                                                                                                                             그
                                                                                                                                                             Y   口 J   Y
                                                                                                                                                                           戶
                                                                                                                                                                                       戶
                                                                                                                                                                                           4

                                                                                                                                                                                           1




                                                                 크；二 二근乙 !. 二르                                                                       如
                                                                                                                                                                               나
                                                                                                                             U                                         e




                                                                                                 i / +C.



                                                                                                                        1뇨
        [8크 Cr.AJ才 的白乙U m七 小 小
                                                                y m，
                                                                   巴 寸 和／ V, 加沅A
         比A工 口乞也， 加크- --'忖
              1 1   4
                           戊乙뇨／ :
              VLj '              十




        加兀4 片町伽磁7已 兀尸 毗小 至
                          뇨 仰-4-旒 寸和                                                                                                  才／, k
                           " ' Tk 小乂
                                    ／寸汕                   似 m小 코凡 4如
        ／뇨 力叫 모근이
                                                                     m智
                  4了 元뇨 汕伊d
                                                          小甲小似V 寸和급if
                                                                                                                                           -(--4-
        근烏 寸伽）'乙Y귿.) ＝근. , k
                                               Sqj= O· 丁kt W彷尹戶 m才和
                                                                    兀
        그 4M " kc小 X凡
                      ／和似 小                           伊而包 衣十 아仰旒
        （月足／2a允毛 石 衣A
                                                                                                                                      仰m,
                      四鼠）· Pcwei                            Cj '-4仰土而 X7뇨小 尸比
                                                                              仁
        Saq = SY그 = y盾 ;             S3노 二 -c.,3 二 니／V丁．
       孔批 m盛玩 m勺 加
                   d沚d                                小在 口才 尸亡才 / , 山aA
       Mdb뇨／ 石仰L4 口才
                     比뇨 0亡往』 小그尤． :




       Tki4- 쿠允比4
                                 力但／如和仙 /(．人人 匕2,1／生， I 0汐rr/ 4，化Z乂l, I, JJ了1戶
       V나二0             (Q,,4nZi．낮 小1七L 匈＝                              7
                                          기 . P卜：力‘ 그 口ma 3 二4丘
                                                                                                                                                V   m




                                                                          m=i <=
       伊고今 比恥芚／, 느-4石 r                      s2. f 二 5m
                                                                    C
                                                                          J
                                                                                                                J
                                                                                                                /
                                                                                       : J
                                                                        n=1                                                                             卜
                                                                                                                                                            =
                                                                                                                                                                (
                                                                口
                                                                                                                                                        H




       山甲d 뇨尸和枇工H
                                                                                                                                                        小   U
                                      4才 和寸r a교 乳， k      구 L   O
                                                                                             5!:.=0 』
       F二m小 7 jAe 蜘鹿씽
                                           尸-C-斗7乞二 루 力六工 b 十-',s-'-fl -L't'多                                            ==.F=




                                                                                                                                     r"t 匕乙
                                                                                                                                 '    ／夕

나Hyd

       /a亡-4쇼뇨， 中工7示派 ／助-
                                           2;- .s: 2『533 =.: .                                     丁沁，月 ，才／
                                                                                                          ，二戶
       5h小d따 』，k. 4枷可血乙
                                             /:a ／뇨，四 二二 L                    -d
                                                                                   -         .-   -' . -'-   /.)-   .-    /
                                              ／
                                              口   H

                                                  1
                              비 = 31立 = 三                                                      VI, : 교LL立쓰 二d

     T뇨 5 ‘仙友； y ／仄兀 /g0 ' ( 3加） 伊毗 泣



                                                                                    O V /D
                  ( g.!o,)

                                                                 i O 0 니
                                                                           i 0D /
                                                         D 1i0
                                                     尸
                                                                                           入

     工才
                                       回        d万


                                   巾
                                                     H                                  小




                    加
          丁
月，
                                                                                    口4石／伽까只 加磁凡 ‘/ 戶老2花．
     a4丑，
                                                                                       "       "
                                                                                                   3L宣으］
                              Vi       .m   j
                                                                                                           口

                              V3            r了                                             /                O

                              V닉
                                   “                                                    Oi
                                                                                                   ;?Z프으／

              /
     d=
                             v2 : · 7o7亡坦 [3L끄 꼬／                                                          ]: 그 . /／亡坦"
                             V三 ' · 7"7L：츠 [3匹으 十7Z프三］: 工9,2간70
                             V4= U




                                                                 屈SI
                7. 3c




             F뇨才， 好牙         vlt              , 口才 肛／/1 - v1江石 和差凡I小小 n/
            Ot:／二上1 和I危，.    T卜田M 才中亡 乙d小 /4毓才 ／私e ,,t石2二b口派 4石，
            和侃W:
                             그    云

                             A1


                                  入可




            Ty皿 ,h耐 m畔小小 平 呻 7 ／征．比 凡石N+ 肛
             (：勺助' ( ' 上｝') ：』7. , -4-了 2炙：7. ma 匈 “ " /
             弓工乙.,M毛 쿠 比／m a/a 力祉 』 i三丑 小孕丑 加중小及
            d     伊甘3 -4- 身                   Z 쿄？／次丑 加仇手工 如們竝ae d
            和伏 l.     - 늉 耐兀‘ C亡mi4加兀｛, 小p%t 乙弔뇨/3 - T加4.
            SMI =s. j= 汁了Z호으‘ ) 5a1= 抑百／二끄으
                                           ‘ . (is미：iLls미' 니-S川＼시5Y/ J느I)

            兀此 乂d        V寸：iv .才 帥才已 七八才4 .亡幻乙尸m友 如友뇨／
                                                       ,


                                              1向
            d,1人友 力14工d ".

                                          스

                                          毛
                                      ＠
                                  그
            Tk七 싸d 加們枷似 甲 mm 弔 ／允4七
                                    肋石肛 小
            군네伊흉）' 竟 ＝근네弩 = 學 , -4万皮＝라／3. 口m/ 幻3: -.2/3 -
                                                   /,-9
4j川在小t心n1
      石 尤仄兄 尸如如 如蜘毗 去                                  加乙夙 /m꾸 冗；
      亡 p뇨乙 (i-Is」이 ' I) = ci            -   · 字 力뇨 , 弓兮 們如力 尸22 '
      m乂和 7力4 力 尸규 兀 石， 돠3『523 “幻I크竺
      T卜叱 力往／ 尸寸四亡乙 乂二 戶才 / 屈 /ILL休 九 /？石化， 4寸
      듸3: y店Z二32으 ' .         (Tk小 1 S1 31' 뉘S녜 " +is了놔 ' 니-S나3尸二吉十寺 ' 事哮기）


          （ 肛左 a 加a 9 汕丘尤仇 J카亡机 口m/ cc
      化耐 而口
      .2肛度d4나 :
                二2n       그 己＞




                  LVEt) MODEL

         근斗 a헤孕 = 죠/
         tp_ -_-_
         r.    Vi-브． __ti(3
           V    力十t

云     TN人4/
                S;zl: c. Lf = 缸re 十r-) 二 士（寸3- I) 二 小Zy（了
141
                 $2.斗 = 늪 crc -r ) : t (--力 十 j) = yb

      右尤뇨， C4小尸弓／元 S－小功9- 뇨，
                                 抑可I互口        y汀I프즈     V／了L1으"
        ts] =                    H27/3        - y3       !/3

                                 가／즈          尸1/3       寸3

                                  y3           中 '/3     小2.73



       Thj4 나m(／뇨乂， W乙Z仄 a Cmd磁m m 枇伊石k力거伊4d土



                                             /70
                                                                          m
                              小
                         ?.31                                                                                                           M

                        m小
                         HU




                        [I七e4(/              m
                                           7 （뇨            ,'1月.         , /／外／느；                . /          -I-             .   ．工    .     .
                                             4
                                              V’卜 7丁VV四v-'- 4才m2a (／人七乂qa （兀十尸그__zi 3 =i4,t亡가／4,
                        d뇨 石                乂凡 /／『 .·.. 小乙 m         s'1I - S3戶乞 丁뇨什 ／石肛
                         m
                         1
                              蜘 勺和烏乞 牛-t机 蜘m/ 너됴 和m교 小a丕
                        艾h兀 瓦 石切勿 a十 肛Zi 그 口M 5 · 和                                                                                         j/ m a甲才
                        小尸枷仙 甲 帥且 7 光／d                                                                     hd加 m7
                                                                         (V三 乙）7근. = 그Z. . .

                        r뇨 品缸                                    싸d
                                       까Mm毛 .才 尸寸／ 五 力m
                        근' , 岸亡 둑，
                                 『 이 m{ 比／侄 m伊d,
                                                 肛m 毛，
                                                     白奴，
                        如뇨i2 兄； 肛左 교 4,d 5 . T뇨叫


                                                 Vl V
                                                  小

                                                                 0                                                                                h H




                                                                 V
    卜
                                                      m2
                                                                     5
                                                                     =




                                                                         = .7D7Z브少
                                                                                                                                                        1 日




  J 11j411Jd3 J               m                  \/; = 1仁 二 C

                                                                              JU




11kn寸J1mB)t11卜hL r 나d
                                                                               l    C7
                                                 <
                                                 7               十        2                      二                        Z
                                                                                                                    1
                                                                                                                    11
                                                                                                                     口n
                                                           1 =

                                                      n                  C
                                                                         J         1Jt
                                                                                         3                  /\7
                                                                                             1
                                                                                         1


                                                                                     十       1
                                                                                                       1中
                                                                                                                  q           二
                                                                                                                                   卜／
                                                                                             n
                                      U:
                                  1




                                                                                    .    /7/
        CHFPTER                                     9

                                    b0y


        弓＞二 5-O 끄－
                                                                                     l. S-    2.0     乙s-      3. 0       工5-



        T뇨 加丹才 小們汕m七乙 N                                                        缸／g :／口孔 , ／少 V(o) = 5『·

        山， 系i0K工仇 久石丑 끄idJ｛쿄5：石』. 加e 力中比U才d4上 /i亡／侄

        力冗l14／如뇨d거                                               7Z乂，也                       仄7工 C＜孑 ＜方／느／

                                                     V伍） 二 v+ (eJ尹                           ) 刀Jh上似』 兀＝3．入／2 '

                                                    ,1 (5:o) = v (x = -Y7) = v ' (-i- r) = 57
                                    V(?        C)       二

                                                                磊 m甲工十 1e -                  c- = 'C/ 7中묘） 二 戶. 6교g
                                                                                                    了口／7 十묘）


                                                i fre"d加！         三m
                                    iv（功1 = 磊 i                                                C<     孑 < A／그
        石                  1 VL入／L)I ;+5y                          (v（伍）:,5『） · T뇨 尸加欠 如W戶夕사y
                           Iv（孑＝//,)} =; (i- fl)「 5- 흙, : 斗
                                                          ，o) = "／·g7
         J너XiH,，교白左， Va力人比4/ Cd4，' 口二了 /e mmZa2玎. 品工
    d
    H
        入／:＜릉＜，入 小                                       ／乎加才 力人e d夙가샤m/m, 辰／M：斑

        瓦＝8D/6 . T卜녀M, tV (3:.7S入）\= 孚욈 :／夙Sb,· 小；
                                                 뇨夙白
                                     C                                        （了1)                                    "



            1   '   /（孕：       l.   2-   5A)
                                                     )      :   ／드6 『

            \ 以5= L75力＼ = J2. 5r

i           1 V（吾 = Z- 25入기 二 ?. 37 '

            \ 叱층＝ .2. 75入）} = 6·Lc,
                                                      니人
             \ 吹三：3. 25,·）i = 3, /2,.
                1V（万）1 肛 F比쿄在／ 石比mr :
                    Iv（玔


                         // \\
                          /\,
                 I \:/"
                  '
                                                \/
                                                                                                          \＼놔／/
                                                                                                                           3／入

                                                                                                      3. 0
                                      5-
                                  .
                                                                                                                   3. 5=
                                                                            '。
                                                                                        '
                                                                       2.
                                                                                   2.       $=
                                                     卜 亨  븍       ［.
                                                                                        決＝ 七
                                                                                            근0 = I0口JL . " (/ = /.0 C,，丁

                                                                                                      ;      L亡 =3.k N


                                           뇨 亡, ＝于．0
                                                 二르二 = -'Il
                                                    , = 쁩，    \


               F八小,-        (9. 9)         0.- 尸4d/m{ /       八，C,q닉／ 加友i竹，

                                           m나키 니 帥 0 . 누小k Pl 드 ]                                7

               口싸（ 4 42쿠小小小乂                         0亡em山 d,，知，뇨．
                                           C戶小 oL 키 C伊O- - 뇨44，이 三 )
               -I了 入人，
                     e C4，七 emn尸比 乂；뇨 戶Z乙四出 ／也／也 :
                       比    0   C力4;－느뇨）盛P j ;a口＋d)
                  다0卜너
                                 Jo
                                 30 '
                  m             100
                                I 1 C
                                I 50
                                                                                 .LiIL1q
                                                                                 I. I /
                  mm釜
                                2oo
                                                                                  1. 7 '/
                                2go
                                                                                 2 . 尸／
                                300
                                                                                 2. y7
                                3 1o
                                                                                 3. 0 又
                                3그（9




나云1裝뉵注스n毒孕杯淅
                                                          /7了
              3Llo      } q斗．r       V，仇浮
              35o       끄Y）占'        小．79그         3. <> 그
              360       206.3 '      -. 765        2. 87
              냐00       22q· t '     小. 75r        2. y3
              나SO       2刃. 8e       -.33교               9/
              5-00
                                                    '.
                        zg6万1         . 177        1. 3 9
              550       3万．10         .637         . 8g
              ,00       3'3. S'       . qj5i       .3G.
              .zs       3S8jO          . 996        . 08

    “뇨 和斗 伊                  尸4小小 口m乂 ／尤伊4뇨M노 匈兀尸石Z好
    kZOi乂丁．



                            5 丁0}7




1
111
  i띨
                             cr0 p        t
       1
                                               1          1
                                                                  Pd
       小       H   그．
                                      0        1         2.   3




J

i

1

1

1

1

1




                                       I 7Lj
                         已兀 功札 加弓 衣小m ／小
                                                                                    Z7 - 1A8
                )

                                                                                         Vc。 仁 .
     II-
     m好 如 a易｛蜘 ‘·
                         근1



                                           4
                                                                     ,    厄三         :2 』／可
                                                                         力？？」力乙     y낱, /2, /y

                                                      -7 君／可m
丑才 근 :aZ내2:; =                                    厄，乙／Y                      .2 근 2/27
                                                       .     근2 ／可
                                                1<Z三‘2 丁                   .2 忙，十2,/9 可百
                                                           ／근工十 2:/Y

           2 , 十2 = 2作，十乙／9 Z1 ＋극y二7 十교Z ! /2；卞
                               그寸근2 f?7/q                    I巨；
                          ,1 .  .      Lf측근：／乙＋已／町 十7근：／可乙又근：／근，)
                    = RZl 肌已 十 근) = 十그止브르
已，
            ,
                                          ／V ' 1 町27

                                                 그27 + 교2/ y／귿2+ 2: /9 +/2, （그균乙＋근．)
                                                   -       2 \/gJ十균．／모 十V巨

                    =     늬 已근：江＋已／4                      十근工后끄교Z) 十근，）仁）
                        4근LV근：＋乞／'1                        근나可 十고근：Y／근：，己／y 十y可（그근！十근7

                        小 Bi;（그근2十니 + a已 幅＝i而］
                        .2. 侄；但：+ 시刃 十 근：／근：十근．/9
                                                  十긋2기12, 十귿．/471
                         如可            ,   균：
                                                     ,/

                        1/ 근 L+ 근．/q




                                                               1 q
         9. 4'                  L

                           m巴r 고寸＝ jm.                                                                                J wc_


                                       " 卜“""
                            ；午으 "' " ' 十
                                F,
                                                                                1
                                                                                r
                                                                                                            卜 Z6J1LC
                                                                                                                              f 口)乙 1
                                                            기
                            二                                         .




                                L
                                             jw니r
               [AZ]
               I （二 pJ                                                                        0I
                                    <)              1                   ，乙
                                                                    , 1L)                                                       /
                                                                 L ' 크U 7乂＞
                                                                                    .   .




         F?／나D們， (9. 그7)/

               근i{ = j크－旦
                           y CD
                                         :          ,)i


                                                        V
                                                                'wL
                                                                          (I.
                                                                          jU)C.
                                                                                        at4) '1: )
                                                                                                           V응／,.:.?D
                                     =                      /               .1              jWL             . =          /    / .L       .
               근2a 二，厄三
                     Y AC.                   尸L4)工乙/                            YJ'(de (/.Z(VlLC)                 尸寸LC V.(z- 2{d '1C)

          F4d)＋勺 (?.3/7,


                                師夜‘ “尸"V烏守
                                                                                                                  4

                                                                                             - w L 乙＜二




                      3-
                                忌＝SO j乙                               I ' 凡＝-5乙I1H孑                         ;   手戶 = 万2 月1/7'于 ;        L尸
          9.
               m肛4竹 '-a們.O烏呼 和机 Tcz4也 '1，긋
               (h니才瓦d m表 ,4加力노낮 :
                                             나工
                           나2
                                                                                                    L= 又凡／h屯 = 3.1g)(,o7H ; 낚＝/5'?겨月 /

                                                                                                     C- = 그／口七Rb = ／그7. pr
                                                                                                                                             ./
                                                                                                   )Yl =   II-（凡／品，)' =．그73- -

                                                                                                   꽝 = 4/ 3. 7 -iH
                                                                                                   4n C= 3L/.'? p 7r

                                                                                                  言去느 = 2 , 7.

                                                                                    .        176

1i11寸1
                                              m伉苡未n씽 似九m "                                                                                         伽 “ ' O)
                                                                                         m1L／쿄



                                                                                           쯧 老
                                                                                         ／万了？\＋寸4
                                                         1
                                                                                     l
                                                뇨                                                         Z乍
                                                                                                                                              ?1丁L = 9三 1/           夕7 //
                                                                                 丁
                                                                             口
                                                                                                               4i   r                         尸工
                                                                                             工
                                                                                                 L
                                                                         뇹
                                                                                             1



                                                                                                                                        쯔으 =                  3 ,. / 尸 F
                                                                     h
                                                     1           1
                                                                                                      1                                  a,

                                                                                                                               ｛二쯔                   L. = 77口. ,,//

                                                             小
                                                                                                                        2C3 m W


                                                                                          寸計
                                                                                                            띠 6
                                                                                                  H        V
                                                                                                           久
                                                                                                              a
                                                                                                                        和 m  F H
                                                                 1
                                                                                                                                        Jt;
                                                                                                                                                     i pF

                                                                 ' MA云M=？二玉“ .疝，,,, -,下.4 Tt品
                                                                                                                                                                            G
                                              TI'兀 CA缸ja-                                             小和，
                                                                                                        따                               m' 小                     YL 小뇨·




                                                                                                                                   \
                                                     0




                                               -20




ii뇹4三4 ； 二 身 크 4 立 ；; i i 느 呈 重 玉 됴 甘 首 휼 每
                                               -40




                                                                                                                                                     n
                                                                                                                                        d,



                                                                                                                                        1
                                                                                                                                   工．
                                               -60

                                                             0                                   20                     4。                          日Ci              三 二，       10」)
                                                                                                                    F F＜드 Qu三 NCY                    !n!d 二




                                                                                                                          '77
                                      凡＝ 75小                       ,       凡’ 50 n7片둥                            ;         f凹 = yg月7月孑            ; HI'
                 k
                             d王dJ斗叭                                              4d上寸                                           7T口／
                                                                                                                                   ，년a 9 2 :
                                                                                            多4,
                                                                                                            心人

                              그C                 교C-


                                                                                        L = 凡七口七 =                                   //9, -, //     d/
                                                                                                        .
                                                                                                                                                          ./

                                                                                    C = 1긋反／C 尺＜) = 그／4 그／) F ;                                   긋C ＝中乙自／尸F



           m山仰如乙 月J尤／i刃니
                                                                                        伽 = //－仔戶／/U工
                                                                                                                                                   //

                              C/ ii              2 /?p1

                                                                                        2C                       15/ 尸戶
                                                                                        )V1
                 卜닉j니H
                                                                                        니／M =                    L1ZS      4i/ 1

                                                                                        닉 m1凡 C-                       2드 g PF /




                                                                                        ( m
                                                                                          而
                                                                                                  抑              口          =



                              石咨 ,                             '       「                                         力    7
                                                                                                                      /    F           /


三 T亡H ,』：,
                                                                                                  1
           싸九／
                                           才友小
                                                                                                  戶 느                      尸=
                                                                                                                           口／                 /
                                                                                                                      그J        n/    m
i．
卜小 =+                         즉       " '              <4 "                         ;2L7/h7 -
                                      )}4 C

                                                                                    츠끄으 = 39. g pF '
                                                                                    1 尸 111




                             寸1"F 1竿
                                                                                                            9坦． z 尸F




I
U


                               됴 57 / 力1//                ;=                                                                               ／月 N
                               之                        느 u9 /r나｛
                              尸11나 39. g                S                                                                                  y ／下

                              1 尸F                        1
I
                         \        \    /         \m1中尸H끼Y才H卞H나
                                                                            \\          Y                    /


                         MATt4삐卜                   c-c小J$r／杯iT 느泉                 伽 =.2go                            mBTt4I卜J（卜



旨M 臼mmi/ 끄小和M工 石． /d久名，0)t /e兀4r.



                                                                                 I 78


kHr띠J느 1



h1
         ri卜녀 z
         FREQU드r寸cv

                                        갸
    40
0
                      ／ 幷茫拙汁娥小曹聲出
                      1
                      n                          !4望43知kV
                                    m i n J 下 r ;1
       ?.
            7         ／乙1小W /9'6/ 77

                                       (iJ) = 什次k그旬느1)工
                      PL－足 = ／十＋ - 7 ,AT2
                                                                            戶    月／   “
                                                                                          又


                                                        1\R 二 i = OdB

                                                        PLR = 1＋案2. 키otB = {. 259

                                                             d/   4之 = 土 . 50?


            （似싸才 C/m坤上尸 次 = 二 goq, 0뉩山刃：ieL,
                                                                            . 口八e Md才 力加幻
 T凡小            ／伽V
                          (?
                                .   '   3)
                                              ,


                       R=／十긋矢 ' 中7夜／万万' 二 乙6口                           /



 小뇨． d石J 凡h亡 ，乂物＜t才

                         y+' = 赤 /.' d工足1                    片     乙 = -V至，,
                                                                       C,／尺


                          -9求‘= d=. （足' 寸十L - 끄C尸 ' )

                          小／4）表lR = 才: 2.
                                                       嗜菁 * 8夜R／万
                               R'C'1 4- (/6液'尺＋了美尺V百)c ' 十솽느C
                         7, og Cy 小 G,69C2 +/. .5-石 =0

닝刃寸．
                                             C t. 6gs V

                                             L = I. S2.z "
(R, i.," 小小 M／不
                                                     小此小川mM冶勺，a.J.r                           )
  뜨］
             下尸3GH8;                                          LP, fj「             乙＝ 754      ，.   仄：a.             5口月孑
       F忍的召 蜘샤山／ 모q
                                                                                                          了B
                                                                                                               .才
                                                                   V
                            匿卜J
         =
                                                                  至3


 和 7加加 Fk夕仰刃 ?. ;4,                                                          叫＜4疋， 4．尼之    才幻才 肛5 硫／774e 口(＞그＜>
                                                                                                                           d8
 I卜的 和M 丁aZ( 1. 3J 比I'오 LP 加存和尼 伽加巾                                                                                 似，

                                                                                      Ll           L9

                                                                             .耳까耳世干．

. m勻 (?.' 7) 石仰流 和們
                                                                                      畇 蜘乂 ／竹比乂d枇兀 :
             C
                       '=
                            /，늠
                                        ,        =        ·   937尸F               /


             Lr 今乎 : 6·舛 규 ./
                 CA=                    和                     d /. 꾸／ /，尸 /
                                  ／乙 口J已                                      '

                 亡9 =                   凡8y                   = 6．꾸V m// /
                                        （人)匕

                                                     __       -
                                            L_
                                  ___

                                                                                      "
                 c5=
                                                                   Lt37尸p.
了뇨 cO且小石立／,4e伊小니丑
                                                                              屈M似"1 兀뇨1




                                                                       'SI
                          m
                                   H



                                   m



                                   H



                                   그
                           0




                                                                                                                          \.
                        -30-   -




                        -40                                       1   1   1   1   1   1   j   I   l   l   1   I   I            I   i   i
                                                                                                                      1
                                                                                                                      1
                                                              1                   1                   l
                                                                                                                      1
                                                                                                                      1
                                                                                                                      드 山
                                   0               1         2                    3                   4                                    6
                                                                  FRE（그UENCY                  C｝녜 Z




       7                           品＝I&뀨＞)               /／尸 , 3d8 프足 ;               N= 5;               及＝万乙t2


                 q才 F: 石GH和                              1늠，J -I " 士－/ :.6b7, -寸 7／小V ／乙戶
                                                                                        （ 오27占
％丑 aim仰烏1 7乙七 刀＝了 4知岫（ ／之 md                                                                                                   y／了瓦
『mW Tcth在 q, Lj 尤小t 小Zb年工 4m／小 a上
                                       71 = 三9引7
川卞

                                            ·7石／g
                                       和=
                                                  538/
                                       了 3 二 9.


m
너 h
  寸
  J 44}J
                                       7V= · 76/ g

#                                      <? 5 二 3. V万／7

I
!＋나尸汕M足
                                       「

                                                                                      似石썹 加乍 (9,7:)"


 （玄늬出쩍yh뇨

                                                                          / g그




         꾸 기y쿄maHbtUr
 :卜i느뇨玄q\k
1
1


                                            니 “石i可 ' 2' 그g1 H
                                                                                     근0
                                                                                                                                                                                                              /


                                                ..           =i；                              뉵                                 ,               =           '/   .   ItpF                                    /

                                                 L弓 : 그드－ = 1.
                                                      i工毛 7J   7夕m H                                                                                                                                         VP




                                                 “，注뇨了, ' 4'. /2可                                                                                                                                            /

                                                     L5 =
                                                                                                                                                                                                             /

    Ti.'叱 m                                 io
                                                                                                                                    尹m                                                 4-                                     娘石甘：

            0




                    "       '       "       "        "       "       '       "            1             1
                                                                                                                '       1       1       1       1       1    1       .   .   .   .
                                                                                                                                                                                            '   "   '    "        "   '   "      "   "   ·   .        ·   '       }


     -20




     -:30       '       "       '       "                "       1       1       1                1         1       1       1       1       .       .




     -40

            0. 0
                                                                                                                                                                                     工 .0
                                                                                                  。.5
                                                                                                                                                                                                                          I .弓
                                                                                                                                                                                                                                                              ,
                                                                                                                                                        FREQL,드入心Y
                                                                                                                                                                                                                                                 y.
                                                                                                                                                                                                        GH2




                                                                                                                                                                         /2了
    ig重茸4]   9.io              'o "2GR5 , BF, MF&P; L3_ ·05;' AJ二'/ , ' Zo『5&r-

              Fm加 Ta)r白 9百， 光4工 아磁和e 皿뇨J加k似，
                    81 =/,D59g              L,     Ci           L3    C3
                                            尸恥니F
                                                          l1' "百니
                                                          JLZ

             F-1』勿們， 끄J在 q. 6 口．긋 (9,69) 尤뇨／加쇼Z 比4M叭／까亡m', '2叱．

              L! = 三’
                   ，二" = 85'. 3, b1'                           CI “寸．瓦：.07了／"「
               L1= ,..스즈
                       ，“, = · 3Z8 4, 14 1                     幻 = ,.. 7
                                                                      ．  느 = ／石. 3尸戶 /
                     口7b 8 工                                         乙1／
                                                                       口n 亡e




                L3: 聿후＝ 2.幻．H1
                           1/VO 14
                                                               C3 :I., 1 , = . 玎尸F /
                                                                     1JVb 7}   t口



                Lq =
                           茸, = I, 8勻9 '                       c'：四三石, z3百／pE /
             Tk오 m{m尹亡批；工 石／／닉切m,, 不石小


1
쩍
＝
                    t .0              i15                                2 .E5      3. 0
                                                 FF追（기.1三NCY   CHz
              (/ V: 3;       BS,' 口万小 E<, "             乙＝·／/     f· “了G//j/   禹 “7c+ )

 Pm女 ／山                  r7. 7引 名                   Z白夕m          了／&勻 杏 4乙p
                     /m伊亡m4皿 :

                   呼 Y針 勘" : ·／／字 . 丹少／ =,'. s a
4乞
                   隘I I  -
                              :    '       5-
                                                그
                                                    口M 尸伊m 7그7口 2如
知 aZ枷友1 甲 /／和
7: /4d=1尹． 72나Z且 q. 4',
                                                    戶    N = 3,

                                                                 LL


         7, " 兀5U,3
         。i
              qi    = J. OU7
                    = /. 5-尨 3
        p
F；仰놔          T瓦石在 2. e 4枇石／ 口．e刃 光뇨 枇d石／比及m石才
小t兀J4,         口d尼／



                       = 그y 7 ,,, 身
                                                    /    q＝了，‘二 :．口3ps"
 L.l= '和A근. = . 作'4$ eI
                                                    /    C-, =        /    = 6. 宿／p
               四'                      .                  小
                                                            죠姚和4
 L3 ' . . 人 . :                   그吼7m//            /    c3= 93A , .1/ 3尸尸                /
        (Al0




T뇨 小小刃 甲 乂／流 尸伉 小 尸名琵／加뇨：




                                                    巧
                                 0
                                                                                                I
                                                                                                                              I




          -30- -




             4Q                          1
                                                  ,


                                     2       0                       2 .t              3 . (>              크 15      4    0
                                                                               FREQUENCY            0Hz



   ／又            !

          十8 1
                                                 근 l-
                             1




          Z5 二j 已 立M 夕                                                                                              d


                                                                    ［帥； j
                                                                                                                  41L근工




         尸
         나1냔
：텍；4
   小나
                                 비미U
                                                                                  " 烏 “]
                                                                                                           'II At ,「
                                                                                                    沁］4的j'乞시
                                                                                                                                  ＝小
                                                      '3已立Mo]
                                                                /   ］呼小d瓜a 白d夕 ]
                                                                     혹小4瓜a 白-d夕                                      /
                                                                                                    LU"J 峙計ie ＜냔ii-訶少心
                                                                       亡2戶                                                             /J




                                                                             J“侮' 乙J씨
                                                                                          入




斛難出嚼鹽潑
                                                                                    '                     -如嗟느客 弘'리叫
                                                                              e47中（夕
                                                                                          j               't혹（言날，)m《 m已
            民凡皿 危寸 小-a土U元 m 伊고 g,
                                                                    극＋ZZ =4j工근／

                                                                       工 = f+ 랴／Z,        V/
                                                                I




                             蛋
                                                                                   J g6
                         發
                     蚤
                 1
                                              n人J                                                    H
                                                                                                     鈿                        小
                                         O
                                                     (LY ; 小3;
               =                                                                      0

                                                                            幻F ;    戶 ＋                             2
                                                                                                 /
                                     ]
                                                                                                         ？
                                                                                                         ＜才才U
                                                                                                                1



                                                                                                         1
                                                                                             6
                                                                                                                1

                                                                                                                /




                                             乙-Ch     T(l工Ze 9. 3               尤／I-且 乙尸                            1刃／
                                                                                                     Q   乙
                                                                                                                              m

                                                                                긋

                                                          =：斗弘느二
                                                          '.
                                                               1
                                                                   1                T   .’



                                                                            丁
                                   （아加笏                        q
                                                          a 7( 口伽d 小尹4乙在
                                    R乂尤力＼4八a元




                                             끄                                      m        寸       小
                                                                                                     小
                                                                                                     勿          砒




                                                                       U卜
                                                                                                                                  1
                                                                                                                                      m
                                                                                                                                      M
                                                                                                                                  1

                                                                                                                                  )




                                               l
                                              卜
                                              乂q

                                               L
                                              2
                                                                                                                                          =


                                             m工＝ 2                 1
                                                                                                                                  了
                                                                                                                          a




沁nnm,m作nm그mm只딕nnn, Jtmmnmn竹mnmnn71了＝
                                   "1卞1111 " " "
                ,2m危 名． m9JL ．'



                          置
                            口 r느 1그 ,-
                                     Z5                 zc                    夕）
                                     U口m                mJr\                  -Il-




                4ZZ 4y蚣4 m亡 A/c d                       f "C6抑J 工뇨 7缸乞
               ／月和似 汕， 4札거1)t                  /e乙기／;




                    -10- -


                 iSiaI
                  d8
                    -20 mH




                                                                                         \\\1\

                    -30 中口                                                                       \
                                                                                                 \

                                                                                                                         \
                                                                                                                     \
                                                                                                                 i
                    -40
                                                                                                             1
                             1   1
                                           1             111
                                                                          T
                                                                                                         1
                                                                                                     r
                                                         6                           1




校囊難瑟客豪弩二莽輯照姓
                                                               1
                             2             4                              a                      m
                                                                                                                             12
                                               FREQUENCY           6 녀z




m湫袋難建N的蝕錨n崗1
                                               /   's
                                .12/                    (LI',                   ' 「" / m「 j                                                  凡＝／白／孑I 己：
                                                                                                                                                      ：吐 )
                                r- ,-\ 丁ar- ' 9' 3, 乂札 （
                                                       「 尸-7孑占亐丹 -C丘．
                                                                        .i '3                                      /. gj 'g                               r




                      口冊느勻 m仙m 力石竹6, ;
                                                             肛口
                                                                                                                                                 凡和1

                    口꾜 小U牙
                           JZ뇨Jk左 ．·




                                                                                                                                                                       =   r
                     己＝. fl .5__
                                                                                                                                                                  근｛
                     근2. /                                                                               .54'/                                                    근7 =/' 加7
                            !
                                                                                                                                                     I. 3o7   -
                                                                                                                                                                  ,1il= Z. 307
                     力1工 二 2 . 和7




                  十,而Mmm-'14哮
                      少寸 :
                              呱甲，尸 小伍
                                                     mV 1.
                                                                    /     戶     1\                                                               \
                                                                                          \          \                11                              \
                                                                                                           \

                                                                                LgY!. 上                                                    月33
                                                                                      1 b 6 //




                                                                  sqj




                                                                                                                       /g9




：乳，
      ,:,,,,,,,:.,,:,:，冊.m,,. ,   , ,, ..
                                       ,,,,   ,   , ,：싸：,   ,;:,，呻，      .. ,   ,.,   ,       ,   ,.,.m.       ,. :.: . ,   ,   ,   , .,
                人／0l《J戶 a乂A工，
                                      （g岫伍 初乞兀多 兀R硫 :
                                     小如
                                         I.7(S戶       2사／S尸       /．나33           /
                             I
                                   1

                                                           .7y/      工 30?




                4,CJ 兀 50 .j乙 ·．
                                                 g8.3J\e      (10. g __               7/. 7\n-
                                                                                                          50 ,J＼十




                                                           뇨．, 人，,
                                                           -r＼戶           =-Jl戶
                                                                                             /，‘釘
                                                                                             !   Jl- '




                          『 乙呼 d
                口J/ 丑44 似 V                                                           乎&月才· m m和皿 K뇨
                尸石老6/ 石mr.
                                                                                                                      \




                      0




U盡盡韓發燾1
                     -20




                     -30




                       40          1 I   I   1   ! 1 I ! I ! I I l I      J
                                                                              I   I    1 I   1 1 1 ' I t
                                                                       7. 5              10. 0           12. 5      15. 0
                            0. 0             2. 5          5. 0




禽纛趨繫焄黛輦彎麓瀚群搬撤
                                                                   FREOU드卜JCY                    0Hz




                                                                          /90
                                        Q如忘．私毗 上m:n사k 名凹
                                                                                                            ，                  夕在
                        4卜
                              巾   九0.
                                             +
                    4




                                                                 D比二 O ' ]
                             y。2 J
                                                 斗




             Odd／
                乙比 ／뇨miL
                             丑                J:6     夕




             [！뀌'i),0뇨｛샀］[                                            J1



                                                                      A
                                                                      U

                                                                                               駐墨
                                                                                                                 1
                                                                                                                 으Y            尸m工
                                                                                                                                 =
                                                                                                                                 V
                                                                                                                                 1


                                                                                                                                m=
                                                                                                                                     叫11111




                                  ."뇽m6 ) 玎玄瓜' 寸啣'큰 ]）.,
                                                                                                                               으 二   11J
                                                                           -'i/           s］
                               (y
                             4口y"(4
                               jYC(舛'『 흉心
                                    瓜6十                                                                                         y

                                        융4亡믄）
                                           t른） （白
                                               (c4尸 十字冬石A8                                     的*졺j在e)J j
             F升枷m口什1 m 孑mb 如毛砬 :
         '   片，끄 :                      m9十諸4-t.& = O 슈                                         P; －左二7／궂旦）<.   I.    I0   J
                                                                                                                                              /
              B:                        쁘丁
                                             二 - 4- 8 十 普 e力也"多
              C:                        丁反
                                             - n4反0 叫 咨 /dJ卓
                             e
                                             쁘丁      工乂    y
                                                           Ha                                                                                     =
                                                                                                                                                      小




                                             巳                        丁                                                                           %
                                                                           孤
                   ＜江勺
                                                     스丁   工兀      尸                                  /
                                                           =                                    1/                                                        =
                                                                                          L


                                                                                  1 1 7                                                           m




                   瓦         戶
                             D          二

                                             쁩＝ - . ' 尸7y'J, . 그 乞囹
                                                      ／十 (JiY)



斥1U毋蜜L       加"                   在.J취 : J7乂 《




棚肝佈啣쯔mm升于．群界咫b浸搏璘酬i促끈娘mmnRkRnHn曲！11H나玎tflnmw,':叫man
                                                    nnmm艸                                      小" nnnmnm"
            q／弓              Th丑 如L4才 加a쭈 兄｝ 石 Z人i 肛m如 在 咨
            -4-"玘 尤뇨 『-                                 E尤油大 甲 T고在 了" , 初i甥 ／凡 比危교
            카12及恥 弘恤 /k 花仰4 7 名'1上 月比刀 尸m刃加也＋:
                                                                                                    jx:



                                                                             三三릎
                                 jY3＝냥，
                                  1       工7




                        小絮
                                 ］
                   r




            T뇨mma咨 i乂丑 A比） Pm枇硫 I余 4兀 帥小月
            石iL 7似＋ 出2. 甲 何功乙／ （乂'1小灰才 m瓜小 M,
                                 jx 二 B " J" 근. 也뇨 戶／

                                 j旱 , 쓱I: 쯔肛나 . .：三 瓦 肛Q
                                           小4丘斛   亡4         .1


            Tb4, M＜지y m/                                     石甲e 2D , ,/／山兀 ,4d4</Z노 aia(m名 :
                             x 二＝ 카J                    '"                         4m中尸 /3万T\+H
                                                                                            人 = 근아江                           /
                             要   으 ()                   /


                                           七汕乙存：
嚼           F아 M. < ii斗 7M 小M亥屯 ／名夕七 a4小Z吃
                             X 스二 (>
                                                                                                         ;&
                                                    /
                                               1/                                                    \             4
                                                                                       4




                                       戶J                                                                                          /
                             8 m                    /
                                                                                                                       邸J
                                                                                                               '


                             三       그 2b                                              1




             （凡：E. Tk                       阡／也W Cd加 婉 而                                                  m乷石 劣和加似i石m,



甘 巍 批 竄 1
            系才 q 小 口mM召工 戶 y77 如之／/n切兀岫I
            力蜘工，甲才凡 a升加e m뇨万友4 7g/ /'1 ／象 ／屯
             AbC> fLt小切工左4D



                                                                           J9c     -
              1'                     mm                           r11끼   nmmmmmm           中們n   n 4mmnnrm·   1mm나nH1       . r1       r- 11 r1r1nr.
                       1mm
       1.1 7                 ( LP; S．근 ;          針 "'/ 6寸／于； 月／=rj                        口·S '8 E尺 ) 西 =/oo小）
       F뇨加， 丁的在 9. V                      따／ 巧．s)               ,             小，i亡夜        끄＝巧介 小．/ 랴：교口M,
                      7i = /.7&c2 =C,                       斗             P고1 = 81코i/Z. = 씨· 7.
                      恥 = 二 2 之 9匕 = 乙 2
                                                                         Pi工 =          ／근h= 3S; z口
                                                                                      和乙／
                      무_5 :2. 5qoS'= Cj
                                                                         戶Z3 = 33 改／/2口 : 又／. 8 '
                      了9 =／·긋296 ＝乙q                                     P2仕 - 7q 근·／仁i-I = 35- i '
                         7丁 =／· 70＄了 = C了
                                                                          尸I万 :        和근i人． : ／弘7 '
       P.i < 1／了'            /;，人   口／?   C.4t4J4, '
                                                                （小7Z泫＋ 寸                        /"qF/／午)
                                                       丑t
                                                                .   i)
                                                                                     iY
                                                                                                      1

                                                       그 00          ／丁          a00
                                                       1小1               小口          ＝小1
                                                                                                            !r
      TLL. ／口｛亡L d亡和兀 小
                                                             4兀凹入 J日h戶：
                                          \
                     O




                -jo

        1sIti
                         -



                db
                -20




                -30=U




                -40

                         0                2              4
                                                                                            ]
                                                                                            6                    B
                                                  FR드QUENCY                    GHz




                                                       /93



}qw的n: .m棚枷，m::m小螂m冊月mmmmmmmnm的mmmmmm" 娜mmm枷”                                                   " 卜 尸m什nr끼亡기n시斗Jd<1寸기mmnmP1nn nn
             19.     !?        (S -2;      乙尸 , n7尸；            孔＝2G月j ;              2。=5D皿）

                    F;，力）yV         T：나乙， c . 3 －光人E                     亡／7


                                             岫色也夕仁
                                                            I.6I 8 卜 ［그6/ $,
                                             1                                                     兮




                   丁뇨 恥耐 C力和砒h+ C4加 ／乞 샤쇼W滅／ 교石                                                                                                     （兀
                   끄弩尤右 弔 끄 沮；化． -l伉4-李 (7. 83刃 多口口，
                                            B " 笞쯔： 프守r 勿 싸 " " "
                                                                                                       .033            .033
                                                          J:.9口
                                            ＝二수
                                                        Z.e =i&r'-       二수＞
                                                                                                              1
                                                                                         ＋小肛丁mL너
                                                      1小＝     H寸
                                                                                                                  I.    ',   Ig
                                                                                         卜                                        寸



                    r뇨 小出-                       Z弓V乂兀匕 力未尤 （枇兀 三穹蜘尼 9"77 -4兀妃
                   加m加抗-4-. O入 a乂／屯1., 石兀닛e , 4初r力f                                                           刀V石如 叩                                            ／孑
                    (' ', g3a-) '.
                                                 쇼 ' 돨＆ 注寸刃2二· 卯3 .
                   nh              力뇨 幻d 小뇨梳 甲 m／뇨兀                                                               .6／了            ＜小4凡／             ,/k
西
                   /hf쇼Md/ 肛 （싸切 (7, g玉刀
                             161 g中. 033
                              二 . cv c
                           1H1J才才2\mHH
                                                        ;:=>>                   2}L




닙麓텨翎挑礬나
                           1                     1                         1                       a




                    m/           乂，뇨             和孔／4                 小而5亡L弔仍뇨 7加.                                                    Cd4八／               /＜寸
                                                 7
                                    /      2中 aG03 刃
                                                                                         35,70
                                     ．二捕和H
                                                                     ：二＞                     21l
                                                                                  +




                                                                         /79



          " =m0 "    a " !1汗rm中們기끼 n口（"-   'nfl ', -旿m 'TTm, ,.好m4中咐恥7i싸r1117rrmmm7mnnn可거7nmmt711rmmnm小J1m mm                :    1           1 Kn 八끼nnnnnnnnr11+nrPq1!1
             F/m．쇼-t 工Jb\ :
                               r
                                    /1. 20           /g. y '     ．了5. 7.              ／了. 9口      //. 20
                       50           /50               /0             /ib               / 0         /50             .5b
                       mJr1=        mJt.             1J2m            HJr\m            _ j1小        .J｝戶            -z-




            F뇨卜十如小 , X玖工 乙i恥仟叭 乂似；孚 i名上 띠和色戶뇨m兀뇨
            甲 (9. 了q) ma r7,r刃 石，
                                     .     j/ ,g '      +
                                                        4- /LS '         1 38.                 ／了. 51             II, 了 <>
                                                                                                          1
                           丁0                / 5乙              ／口                ／万-d            /0               /5口            5七
                           -r乙               m日J＼尸             -4戶                Jl尸           .-n中               _n_.          -八寸
                               H寸                       +



            11施 力놔 나                                  쿄凡 小끄4 肛d吃듀 弔뇨二 小7
            ,m,4'd九ah 9老／,m工 力                                          났L41們」
                 』升抑刃 弔 加
            丁k, 7，                                                戶才 如和 4 ／加W 婉L可'

                   O




                느工 O叫


           IS2')
            46
                -20




                                                                                                              1
                                                                             i
                                                                                  '
                                                月4

                                                                             a                                               二
                                                               F꾜드二三 ' -:CY             CMz




                                                                     m5



茫川m4nnn！控nnm朴卄朴好祁nammmn的nm口"O나mm"戶小Mn抑n的m1Kyq' 八HNm戶“" "' \" mmm入’" ' V1" ' "
     19. /7 1 (N:3; 川r, 5Pj 3.c- 3S" 口叱； ＆『了" 人）
         듀                                                                三工 三0 寸 . 戶y
            = 工zc Gk3                                ;   d;                3． 그-5-


       兀
            ( '1. 7/) 力 力戶竹名뇨 又9G-好 名仰M胡' "戶：
                            {AJ- 才 (針응戶．扇乙只 ,"y
                                            ．尸／ '1'?
     TkW,                                                                                                 恥4. O "J.5a놈 /
                   1므나기 :.4'了 , 小／吟呻 幻6
                   1 口JC 1               '



     1뇨 나 的Z； 占끈 佃뇨小 毗 甲派叭 ,m 7뇨石在 7.;: 了. ,,/
     Z' 丁M m 辰 戶的d 戶..'i.- (1.2/) · [A』
                                      作 근叱 :d Z,,
     +Z乙可
              r



                   月J                    口                     凡 了a.                                        和O 乙JL)
                                                                                         s,'. 7
                                                                                           已e     (it)
                                               =




                                                              . '1 ?.z                                      37. 5-
                   /                                                                                        '/ 2. 7
                  a.                                          .17/                       6口0
                                   屈口：
                             2. 000
                                                                                                            '/2. 9
                        .




                   3          人 000                           .17/                       6D力
                   //
                             I. 000                           .119.2                     了6. 7              37. 5

      （乙奴    ／加Jd,                                                                                       .3, 그了 夕巧3 ·

            5bJ乙




                                                                      1
                             乙e=             (0DJ2       \/
                                                                      1    '         I

                             근的＝拉只工十                                           m /




        T｝伍 ：고.J誌／m，于加七 肛 ,m小 及白（




                                                                  -                  /96



等，
                              -3 (1




                              -40

                                      2
                                                1    I          I       I   1        I     I    I   1
                                                                                                          1       1   1     i    T
                                          0         2. 5                                 3. 0            3 .5             4. 0       4   5
                                                                                     F RE（고J三NCY          GH 三




                          9. 20           (N. "q): 月'1F, E옥 品『3&-u5; 4-.is ;                                               2：伽皿)
                           V／兀 戶a j兀 多仁 如M7뇨竹 ／뇨石也 艮三 //m
                          力뇨 入／什 o.c. m+ 日吻小2瓦江/
                                               C- ／伊汕m4
                          4乞 7乳나d 戶小 乙7,／了이 :
                                                                                                        Z<＞才1. = H 르으
                                                                                                                 兀旱md
                                                         Z04.
                                                                    .       <：  皿）
                              I
                              又




4斜蝨騏때輔恥瓦衣在弘樊乞4:
                              3
                              今／


                            （函 M              各？ 加倂派 名D Ii嗜及 左 2已44方初／)


                                                                                         戶7
注
螂




       月搏茹莎瑟斟姓
                  m   m
                             1뇨 和d 尹玭L-                                                                   ／侃甘札 小命 "

                                               qo                     9o
                                               H工L寸                    mJLd




                                                       //
                                                                                               1/
                                                                        //,                                         그，
                                                                               ,JU
                                                                                                        JL/              -和

                                                            ,J.   /




                               口-J文 乂qm+                              qMd ,＜友加 m兀 入／Y 石퓽 口才 3口片孑 ,

                              T뇨 .m9Z力先d ／샤寸小 片／出mm 兀乙끄y《




                                                                                                                         I
                                       C   '




                                                                                                                                                       \




                                    -30-




攝 船 椰 飜 難 i 斟 翡 犁
                                     -40                          1                    1   T        1
                                                                                                                !             1
                                                                                                                                     i     I   I

                                                                              2 . 5                           ：三 .0                 3 .5           4   0
                                               2   0
                                                                                               FR三口UEI나CY                     0Hz




                                                                                                         I 93



 繭社） hH4小
               刈
                    1U{n入八nnnnnnnnnnnnnnnn0nnnnn171nnh1rmn껴11mn=              1 m nm m="
                        츠三a                   佃 “3』 BP1 05oB ER
                                                                )                                    3.的－了. 5乙GH, :
                                                                                                                  /
                                                                                                                              0
                                                                                                                                         又
                                                                                                                                         니7
                                                                                                                                            =＜小
                                                                                                                                             (7 UJU/
                                                                                                                                                     .,
                                       유"
                                                3二5GH 舌 ． 乙 = . "5-夕／

                        w此 74뇨규 7小 ／乞小 1나也 9. q . TJ - 乂뇨 》七，.,
                       m     , 如丙m           4   뇨Le               샤小
                       (? 131
                                                                                                                                                戶m如
                                                                                                                                  和仰／
                         .
                                                          i3
                                                                3.77                                     2O小 二               才 죠d
                                                                4 . 63                                                       꾸 7,,
                                                               ;3 .7 7

                       (" ‘虹／놔小伽
                                                             四庇石4幻小m교)




                       口攻 丑小 西六句山小
                       r뇨 (4쇼시石危／4i』
                                   尹dM毛-(4-




r！戴nH hH悖나亭L算洌 角嚆趣齒嘶
                              0     ·11卜＝   H寸Hm1H1




                                     :                                      /
                         m1 그． O-                                  //


                                                               /
                                                          /
                                                         1




                                                                        ;                   1        1
                                                                                                            n=      H斗十커m=
                                                                   ;    1   =           1       !=
                                                                                                            · '니‘                       4 . 乞
                                                               = 二三 9J三N乙
                                                                                            G卜녀 i


                                                                                    口
                                                                                    ／
                                                                                9
                                                                                /
韶照8小依嫩際四8m죠mm8mn如蜘！싸邸nnnnnnqm咐朴mW小呻m.,,.U
                 k．괴 丁뇨 jmm小4 入／'1' 力乏4-小化土U /M鼠小玘4-
                 4小.J回mm/ 比派，, 力小m h刃力t 口加 汕伊仁／
                 aL小瓠乂兀 甲 ,
                                        y = ,J)b仁 口才夕 , 加／
                                                         ／化夕 ＝刃노 /g1 ／久) ＝刃O.
                 코L十 口) = (A). 十乙口) ,        ThJ人八 4二 Va 乙／十乙口／k/n :
                                    Y 乙：yo砥 力m 兀，      /'irm,, (w-姚）
                                                3f, 二二                    二 口7D



                 7ZWJ 珌4 口石／如a彷m七兀 下 4 /m고％Z 乙C 力蜘mm 在I
                 和h니 丁M在 7.1
                                                  y = 7'JSci. 乙口J -m, J
                 냐뇨 力뇨 C石皿，力乂力M쿄I H샤七／如小 9之 Z／나 4才k+ Ki I

                                         乙m: 上 “ 꾸.n .
                                     mM才 小／七 mm小 口＋규兀艸 :

                               그m
                     +
                      '




                    LtJ. 長 丁CA,
                          ({
                 TL'白 丘 j札 私毗 44 乂幻 Ch小굿 ／뇨 尸m表eJ 7乙


市私潞懿高搬澱m
                 F누岫 '?. '1旬 戶 X兀 蜘m 力h兀力蜘4山4 7乙力乞
                 小成友 白J:,:7).                乙4《戶／小k和力k工 小土友 ／凡 和四山Z中
                 교뇨d            兀如a伊4- ／泣也 ／侈肛方4 力뇨无

                                          戶-= VI弓
                                         力文 , !Z二 戶 f 亡｛
                                                       ;
 小凞n明的mn
                                         끄   1
                                                 'Z:
                                                           ,
                                                               Cz
小芦m聲拱案布m攝敬
                                                           aoo



             n
                                            加古刃W                      C二 M     ／二： m兀 乂／ p 石什교 ，旅4mJJ
                                    ／抗 加五q＋』 ma 뇨『』＝口口
                                                                                                 “y뇨.' · 油Zh느 /尻
                                                C叭      7伉叱＋ ,
                                                                                   CL = C1


                                                                                   C丑 ’口』
                                                                                        ，屯닛I2
                                            Zm씹 T姚在 7. 6 石 抗叫石q叭 /M                                      去 乙 />
                                            小乞才汁工 佃뇨4 刃뇨，

                                                                             7, t = C;, 二 寸J二－
                                                                                      4 m1 근a


                                                                         " 7『，노1牛斗磊．
                               ．和 光뇨 品mM危a友/ ，띠寸比枷佃，
                                                                                                    4化．

                                                                        m＝缸 "多·, 2e):            7r 乙
                                                                                                 7 7꺼
                                                                                                        /,


                                        加4毗爪 汐肛 如｛굿友                                   乙只／3/),




町出求m葬m拙




                                                                                     C2(9/

  =my




黨   ,     ,   ,   ,   .   m.   ..   .   .   .   mmm小，    .,,,   ,,m
                      19．그러       (6P , CG , MP j 유「구6-月｝) Ij=.／又 ; 民 “5"小

                        m才 戶나小 3.6 6-H孑 石 乙尸 7毛小

                                       小 才怯，쑹）: .古（푸．去） -1. 76

                                       岩，
                                        卜1 " ·-7/
                      石rmW Fi伊伽兀 m口 加口4 乂Y白／ 八／=3 -i 끄們n/
                      力   缸，
                           卜I瓜咫             乂＞／긋Y6 d三C 6-I／孑， (
                       乙R ) / 十乙q7M) ' 시 ;,q. 9 d乃 7.弓그， 八／＝刃

                      丁뇨 m斗比 加乂뇨七 刃之 多mM ／뇨 7二노石在7' 3 ,
                      rh蜘 玉了, m小 ／之 7知d 戶加 (9노／.zi). r／따／
                       乙B,d  3__.근. ) 口，a 已＝兀글liz뇨'（그．
  나섞姓J a
       M山
                                                     毛B小妃'm·瓦冽
                                  卜 （乙小）L

                       a且勺             e何： 已／幻. .

                                                                                           瓦，@ 9 5/／舌
                              ／   八寸
                                              무    ,\
                                                        ；뇨工人        근08m         C-   .1




                                  /       /,000         . f3Lf     4 53 51   .if 3 아：7     ILl   우0

                                  ;2      2. 000        .133       .135      ·l.L pP       t 6 5O

                                  3       1. O0 (D      .133       . L근）5-    U pE         t나3 0

                                  //     1. 000         . (/ 3 9   .5-35-    .I 3 pp'




                               ,i力危了 가戶伊m 小 '-4加z t 派乙可）
                        -F卜咬 m且，




料瀏나aJ轟川J浦m醬出黔心m斟難懈攝
                                                                                                                          \
                                                                                                                              \


             卜；
                  ?(>   =1叫




                                                                                                                                                                      ＼니
            -40                                         i                ]             1   J     1        1         1
                        3         (>                           3 . 느5                          4. 0
                                                                                                                                          {
                                                                                                                                  4. 5                                         5   ,:=
                                                                             FREQUtENCY                             GHz


    9. 긋7                                  丁k(               易似加丑d Cm2小；才 在．

                                      극，
    -4.사小乂2+\                         m小‘ ，力＜,                        /／乂／4才2兀4/,,, 乙之d』，



                  .三尸＝升',                                                                                                 75

                                                                                                                                               1     \    1
                                                                                                                                                              띤ye 也立


                                                                                                                                                              '       申：
                                                                                                                                                                               .         2.
    a人小i4乞                                 ei = 兀 十 古 56/ 畦di+/
                                                                                                              -1뇨 i= /) 刃 4. 八／
    F汕M P乂孕q八i                                               乞38, 力뇨 口뇨，
                                                                       ,a                                               CdM辰 끄上m力砒M
    md咨 ／加f加｛m工 小小d小 ;

旨
                                   , 「，,:       ,   '
                                                              :                  11。
                                                                                           O
                                                                                                     ;.
                                                                                                               /.
                                                                                                                                     1-
                                                                                                                                  11卞1HH1+
                                                                                                                                              7c,
                                                                                                                                                    ,'t
                                                                                       구0了




      . , .，小，                ,   小         ,   ,                     m小如如小小如小
                                                        如小        ,
                                                                                                                                                                  岫        如
                         Fm机 才뇨 和尹比 i                                  甲 力뇨 石伊枷m兀 J뇨카亡磁띠
                        d才J七， 뇨）사七／                                / -i/ ;tX; \
                                                          二
                                                                                                      1/
                                           /i
                                                                   나h' L ZO /

                                                Xi =               .       <                  /
                                                                                     任)
                                                                       1        __




                                                              1-                          "



                        Tkt ,
                                 ei = 不 小 t ［占＝（그Xz左.) + 在二／r교Xi*,/Z.)] .7
                        Th且 ／뇨刀려i瓦 的瓦危 Ok兀 毛뇨M 7뇨p- (/.1. /) .
                         （丁 :: K／귿：)
                                                }<        1
                                                     금D
                                                卜C奴            小
                                                                                7cA
                                                 毛
1



                                                                   그／乳．
                                                          弩
                                                                      ，莎
                                                                                                  1




                                                                                      d
                                                                                      兀
                                                                           ,J
                                                                                     7rii                  =


                                                                           r 7抑 7시十／
                         志
                         N       스
                                                                                                               m
    自
    1
                                       d




    如墨攀薑i騈騫烈資a礪豪薰發醬塑乳
                                                                                                                   =




                                                                           ;2oij
               CHhPTER                 IO

              1   加    ]
                                q,rMs 二 {78o (?                                           ; + = ／口G/／孑
                               小
                           (10. 그V) 十（／口． 2 引                    J                    ,    ,
                                                                                               //.-    F          jX
                                                                                                                                O
                                                                                      L友I " 1 口J\                  저            O
                                                                                                       L <)            0        4(

                                 小끄。(i『 岸능)                                                                                    )< = 지。-望쓰．
                                                                                                                                           口Jb4mmm

              1)   小二 卜4s二 O                ＝今 口'0＝反JM 二0                                              4    恥吼                 』 x二o

                                                     回
                                                                     r1l1111L
                                                                                                        ]
                                                                                긔


                                                                                          0 吼 0
                                                               二

                                                                                口 O
                                                                                                              /
                                                                                                  三．
              L)      H0 二,oO ' 0e

                      r kJ1M       듀 = 2· g 쁘즈 (je口o 0e) 二
                                                           二공 G片方
                                                                 0亡



                                두H = ZJ 쁘i (i7 'O (r)
                                        0e
                                                     (倍）= 吼9y ; 尸둥
              4亡；

                           자＝자. //+ 拉算）二 . 8yr 可，
                                                           hr戶＋ m/
                           X = /G 그또工 = －口 S加 4b
                                  手；三 中 下 2

                                 ,              1. 7斗9 -.S 't0                                         이
                               L J              t 1'. 5q0 . 묘푸9                                                            /
                                                                                                       oV "
              二                                 LO          C                                          / J
              口
                                         8X = 乂｛ HX 十Jx 卜1j
                                                                                                                                                     /
                                                                                                                                                     /
                                          B뭉 = -jX4                                   -+ <4H3

                                         3吾 "                 乂／. 14秀




4脅實多弩密發上豪脅r
                           B
                               士（弓；뉩3甘）＝士 ［出
                                                                                          4J( +JXHj 十X H\                       十 t .i{
                                                                                                                                          H3]
                               打川十K乂 HX +i Hb ) =
                                                  (/( 十X) Hr
                                                                                      그05




                                   111尸11月1!1! r1m11r "·   !m1mmr1    r1中 r=1
［而히          ttt4s         = (2o0 C-           ;       Er        =/0
                                                                                  )   H0= ,2000Ce ; ; 1yG//}

      ( EtREFRIJG-EtCE)
                                                            F = 나 G4{ }

                                                            듀 = (2,g/H什孑／Oe)（그ODO口U 二 g.
                                                            c)i그工9 I1I4!向 (I그000e) : 3. 3'eHy
                                                            是, = g3, 8 4,，나

1卜h 和M (/0 ' i키／

               져＝     4小        『
                                          ::       -   f    2-                :       乙2）小



               X= 七寸二 = . 87了지.
                                    加切e. 뇨＋ 戶 =Ily f,                                         O. 1 在 Z玖工
                                      伽石q戶Uo,e-c) ,
                           y m小， 工뇨＜加
                           如    "    亡：        :3<     '         =       /,       2? 刃.


                           Fe
                                二 (4e／化 ＝札丙札久. = 3&e/. 3 似．/
T뇨 寸 小守／ 小ra刀C 뇨L4- i= /／乂t/ ma a;                                                                       i乂工

                    4/J亡，1十之．             겨뇨．
                                            .

                                                            ＋뇨 = 그65.o m八나

缶 多나 m;dm 和 八 d伊石苡쿄 ／佃七 My仰
                           3= . 37/j                                    't7, c ,,141 7. 4 .
比4口
                                半e甲0




                                                                 '- I
  10.7




  T卜乙．如汕굿 / mymi玎／ a
                     L方石似如扱甘 7／比乙乙 7家
 亡兀 尺HcP 加吻之 C4\ 力之 加：
                      -4力뇨＼ 口勺

    百A= E, （亡戶）a卜孕
                                                , (9『j{)d」
                                             '= 뮤
                                                             令吾
                                                   小
                                               H
   巨r= r4E. 伐59) ej和｝
                                            百"= 수r ' (9 4-j幻d"八孑
    듣亡＝ T4 E. (定好）dj和孑
                                                          jX）可 "
                                        "
                                                  T
                                         "t:
                                                        Eo
                                                                                        "P
                                                                '
                                                                    (
 m札k旦， Fb＝臼／i；
             乙 ; 肛 ：回／E（가*X) 7
                               rh= 中 :／在*).(                            ' -         r   6

 77乙d石／빠7 戶比在 寸 릉札 용小枉
                       竹小嵌x니昶                                                                甲吐）
                     1 +r+ = T 十
                  小 征 r+) = 兀T4


             r+.= 가＋-rib             ., 丁十＝                  그y7十             /
                 1) + 十 小
                                                        n十 + 小
                                -J
                  &LItcP 4凡m자e .冗刃e d4在反，

            r= 포H크k卜                  丁 H=              二1?
                                                                              卜／/
                1? - 十 기，
                            )                          午 十小
-4乂I小J八꼬，
            午士 亡 "



                            긋0q
                                              4f兀Ms = /.)00 6- ;                  瓦＝ 尸侄        j f= qGH子 j   E：瓦t
                                              두m = （그· gMU3／口e)(1200G) = 3. 36 G- 奴
                                         /+       口．= C   4且        甲 小h半瓜yM乙 . F乙1力n小／ (/0. 6'/) -口0. 6 57 /
                                                                    Fe = 이石r
                                                                    /(C = 三亡二：츠
                                                                                在

                                Tk凡 如肥 加i/Z k
                                                                            mJ今中 m뇨 砒드 " "
                                                          七
                                                          （'   .
                                                               :X
                                                                       '   <0
                                                           乂（


                                                  (I唾象 ) （韋州' < 0
                                                           1 , 듀 ha
                                                                                           d
                                                          ／十 百二万

                                         （片 ‘4: 2.y. +？斗（牛4:1.)+4:訂各力 <O
                                           (4:L4 ' )Un'“工' ) +M니                                             \




                                                     （符r) 十 "。
                                                             4h + 工：                           <0
                                                                    r1-*2. - 1- 十兵뒤H

                                    忙-.c2# .c.1h><>, .-未J.\ (h十下m）느r <O
                                                                                듀 +f1n ＜下




m샤코萄斗可나m芯繫1爻nd卄dnd4
                                                                       f0 < + --c1 : 卜 知6
                                                                                          " ·69口片孑수 /IC =           口e

                                    佑-.c ' 十 1.｛쩌 <0 7 j未4小 侃+4小'나
                                                                                                ' >0
                           i{
                   斗가hJ4
                                              q,,d         FJ十兵4:뇨小下 ' <0
                                     小

                                                   耘－凡 平系可' = ．二6y土4· 3q = 二666片孑
                                              十
                                                                      又



                                                  呼
                                                    =+      L-I。= qso 口e               /
                                小    加
                                                          ／小4I戶 在＋名m 그그7 m,a ?5:D
                                                                                  口C .
                                                                                210



mn1Janmnnmhnmm7mm
                  J    to q.   I                                                                 q 기．Oc1竹
                                                                                                 千 =to G- !



                               二
                                                                                'C              切r114 S =L7乙 乙 C,-

                                     叫
                                     二
                                                                          乙
                                                                                                  6r 키3

                                                                                      加m 加汕뇨 右」和乙｛如 7?)

                                           征
                                           J3
                      口／
                                                                                      m兀 丑五m似 兀뇨 戶 肛 1
                                                3.       -




                                                                                                          仁／札

                                     2 1m三


                                                                          伊
                                                                          笏m쏘
                                            2.
                                     11
                                                                                                          P+／矢，
                                                                          十HO
                                                                  笏
                                           I.        -




                                                                      手 ' }DGH}
                                           0
                                           0                      1
                                                                   1／仄月匕 = 17口0C
                                                                            1
                                                                                                                1    r
                                                     0                     4'oo          Voo         屈e
                                                                                                                    Ifoo




                               m r느
                                                                                      /1。 口zRst百1S




                                                                      起n 乙
                                       n   d｛ 彦                +                                4 = /D C4m{
                                                                                                f =io 6-if

                                       0
                                           >                          나 =H十 下
                                                                      0
                                                                                               "4才川5 기-100;-
                                                                                                Et =13


                 匕t                   /                                              -4刃a4 /m亡磁人 ；乙 ,dd乙（ 口口，r幻
                                       Y
                                       /
      黨葦m客墨m                                                                         m只 코尻mm ,Z七石긱尸戶／=                     /
                                                                                                                           /
!
                                                                                      只／/


ti돌
4角mm !mm1i1in1nt1111111111mm111111mmmntmnr ni,               mn1 戶1
                                                                             3.
                                                                       .2.
                                                                                               少，
                                                                                                   1 ' 刃eH舌
                                                                                                           蔡
                                                                                                    q1rrs 亡 t7oOG
                                                                                  a
                                                                                      O                    如t)         Zoo      1&00                    I60D
                                                                                                                  HO   OE只Si百力S




饗咬恣趨口我口蚌d
                                                 -                 -
                                                                                                         f 三*oG.141 ; 口＝二그J6 디m ; b: 1· 口／6 m
                                   計11그
                                                            0.
                                                                                                     伽rM5= Qco& ;                                                         l
                                   H mmn                                                                                          c= a./q ;           스S ' 교 4꺼     )11



                                    ＜亡＋                                               \

                                                                                                    表尸그.오I'什4 ; S= z.32.3什꺼 ' ; 凡 ＝吼76 6-月于

                                                     弘） 加 따恥m友4Z P枷上 4才力／/                                                                     乂1,



                   （和－FD／乳＝-.去 芳 孚 小k2在. : -.O/／了 X/4


m峀蕉難難
                卜奴畇                h佰K3) 目七a                                              邵         (O
                                                                                                          （肛Py뇨

                    0                                                   -.t7r                 /.           .0oS '( V

                                    .                '                  戶．亨77 . q73                         .oocc
                                                                                                                            m1O
                                            S.
                                                                                                                                       6
                                   i 12 .                               +.YyZ ．刊6                          . ooSc'            乂J




                                                                                                                              O쿤公也i나
                                                                                                                                       9
                                                                                                                        1

                                   1. 6 묘                                                 . 引g             .oa (O
                                                                                                                                       a
                8oo                                                    -. ro/             .gq,              .0O ( '7
                                                                                                                                       O                                                         r

                                   2 . 70十 -. 576 . 'S-c                                                   .oo6S                           O
                                                                                                                                                그00    , 二o    f北         g OO            갸r乙   ／그DO


                                                                                                                                                                    c
                                                                                                                                                                    G     ft.c)cj
                                                                                                                                                                          ..,        .,



                                   3. 3C                                     戶. 5-37 .820                  .oo7l/
                                                                                                                                                                -
                                                                                                                                                                                 .




                                                                                                                 ；가2




I    fl Wflfl   fl fl fl "mrnnn.            ,        fl fl fl fl
                                               臺口                 千 "
                                                                        g6H孑 ;   4'可n4$ " /5b0;

                                                                  뇨     " '   2 鈿｝

                                 出十小m和力-            , A刃0M小1 ／뇨 才)伉
                                                                                  升似늉 4
                                 그f和W如兀今 比7 伽·g
                                                7) :                      (iv，日， 싸作미
                                                  f = 7f. (f.+fn
                                小-e此 石1 f; :              fL = /:＋凡1,,
                                     'I

                                                        f '? +9. zf , -6q =O

                                                  凡 " .2.／土오그7 =
                                                                              6·／74月孑
                                    d4＜丁 /
                                                 F노 :    6170月4Hl       = a긋0v. O: /
                                                         口了／刃月｝/De


                                ［至              出y加竹小d m小
                                                                               mM兀 7吼多i
                                                和／孕 /i 7／此叭 Jy i名工 師油뇨 ,

                                                유 “ 下 " gG幻
                                                                                  （刀x＝价이 仰功
                                   SO/

                                               H' 嗟蠶努＝" "「 " /
                               而이 T卜且 -w呼md 和伍
                                                                      7뇨 比뇨 兀드O
                               n4八万닛i/    切小衣 -C사크：ZZ2，人 口＋.


                                               忙 孚 m如 a船
                                               F／궁 :A 師鬼工 ed幷




卜小＝ 和미卞岳仁d吐虹mJdd日Ji나J沚川小鹵小明씜
                               加奴 枉三
                                   『" ; 肛 厚了：百
                                              '                   · C뇨山凡和毛‘傀‘友
                                                                              ＜
                                         쓰心
                                                                                                      r口7 凡-
                                                                                                                   A七＋
                                                                                                                         늬
                                                                                                               -
                                                                                                  口
                                                                                                                     L＋

                                              」‘湛乞丸／ J 0L- 瓦丸；:!                        女             (／口 16 )
                                                                                        戶

                                                               2I3


鈿解滋n姆瀜淋吝晦小烈邸烈棚mmmnnnnn
                       Rmnm                             mmm"mmmm'"""m"""m小
        孔／4?C       P／聚C                乂 人t                    2뇨／
                                                                  ＜之

                                                                       /
                                                                     ．引Li
                                                                     .753                               ti뇨小뇨／k.日' -1
                                                                     .7/S
                                                                      . 6 27
                                                                      . 616


       Tkto兀 加寸 尸土m／뇨 Cn兀‘八／dn/                                                                                                口4丑中




       fJf比I 小公：


                                 加旬1-so卜.,s D F                      c1RCUL月艮              印나R1t人Tb시




                                   二7                        I."                       /6                          工g       .7.0
                                                                       乳／匙



       (0.14     千 = "- (4吾 ; Er=10                                                                                 ;   L = 2. 7& <:41八

           ／寸   下）仇 =q. z 6-I／孑

       d,\ 比뇨 -It月44八才t/，凡.1．人才

       未-,      _q=40       ,       X=

                끄e =    在느KL                = -s/ 小
                           /<{
       O1나 J抗危 牡／ .              所 =r4r X                      口m口
                                                                       （                                       J



       m     mi; 4교山乃                      ／口／re 1
                                          乂／


                                                             又i니

nn닙肄




                                  11H   nnm1d끼nn   mn   1q             r끼 r1 1H卄竹Hn=   1nr11卄1rUn=   1nht1t1
                                                 尸e：丸／fr끄e／끄.                    = 긋g3. 9 ,.-7                      /

                              山 da危 多교，              M :m『了 cL.I                i＝智； , k               乂石d


                                                 和 =／乙乞 = 3 y 7, s 而'/ /
                              丁h小 乂뇨 呼尸U二dZ 小M 叫／才                                   ／쿠
                                                                                            )



                                             4少 = 和甲DL ＝印.－尸e）亡 = ／꿍／'                                      1/
                                                                   S =2mm ; LI兀I'什 =/DD<) 序 ;
                                                                                                        f= io&月孑




                              F加H F勺4(4兀 lO.IT, 加小們 4和址 戶伽口4
                                                                                                                           才
                              戶 S “교枷似 m仁h+ 7和 口4心·／／그／午寸
                                                 2f = ·肌？口. =＝그．石 )p（거4 /

                             丁M r和甲-)／允＝' 2y
                                             』 74= 伽My " /7了‘4,
                             무 加叱 口m弘似 r/,．戶) 丘 肛和兀疝／ 名 XI
                             （口ma44 'sr), X7니＼ 7h 4／兀／너r =／口Oo 6- 兀4,亡 4dV<

                                      ！哥二．可驛戶·幻V
                             4＜少    小＋-)             孔 =/6. /72h, /
                              뇨
                                     元뇨 序在石
                              y m                             兀伊4 74L /g口口 二片a fDD

                                        ／小
                                             ＝     ／加 '        .    小


      社
      m                                           14, /9t뇨4侄 小

                                       1     =      e/   Oo
                                                  /41／乙4뇨＜




難I,
          '月m:,,,:...:.a朴：    .,,
                                                                                          nnnnrmrHm;   k!   H斗시1\   mmN14口4nnnr叫寸d끼m{11 111
                                        (t= 2. Ze4卜，; b =I.o'e 口小 ，‘          手 = r6/y}
                                                                                        ]
                         tMt
                       11ll11i[         q7口4r = t2o0 G- ;    C＝甲"1            ＝그 Hn H
                 4H
                  C.
                                        4中 ：二 구2. 5'

    F月刃＼-I八J
               (/.·如） 元뇨 (따W너乙nm左） 4知瓜n仙工
                                       二三    츠小 스三， /4辰
                                        口뇨   乂（    5




    7L弘y, 戶 尻＝0)
                                  X可              小2. t (／그oo)        - 373
                                        7H 戶          7co0


    a人N工       S =&L = .23 그 . 3 口,' H1 ' /            -4才


                       戶＋.Pm 二 . gg3 ／』，.t／勿， : 加6 7色1.
    缶      光뇨 a少니m比 石7朕

                               乙＝ 그그．三1 二 9y，了                   1/


                                   · S06 7口어


           （仄 /；才石牙U




H




                                                  2/8
                /o.I71
                                                              打r心 키700口 ;                 尸7口1/方 ;
                                      介 H4                                                                      zS= 6竹H "
                                                              & ＞工그 8G q . j              b = I. 0i
                           （巨＋
                                                                                                      C4

                rk工      4升尸仄工 7筑此Z 肛
                                                                     /／工「.Z 000 (9e /           구r ／三白W 加
                                                                                                                              ' 竹)
                比乙兀 小施W4王

                         F4O = 月口． 小 /VI.'寸 = 口＜＞
                                                口口 /I? 口0 二 3co Ce
                                                                                                                          )
                F小. (/ 0. go ) 尤뇨 (卽
                                                                                                           (A
                                                                                                                's
                                                                                                                     "/
                                                                尹m和仙兀 ) 따伊J泣
                                                                             11                                               尸丕쨔兀
               ／小；뀨 在 ,
                                             弘寸＝
                                                「               二誓 牙 笞 夕뇨 弩트
               74切肛仙' I.                尸如石 ／及구f 小元Ze                                     c如 ／弓七 C, = 今兮 = . 57그 C4+,
               Th妙，        -c1 = 2 ' (r7口이 二4. 766丹
                                                                                  孑 ; 針二g如尸．
                好寸／
                                                                                            RqG幷孑
                                 小吼 (I                 ＋ 丘） = . 7口／,
                                             \          十C H 十       /




                                        吼유                                    ／吼
                                                                             万』
                                 「：
                                                   ＝
                                                                     .
                                                         ?:
               Tk ' , 肛甲．:,:D 加乂／,,i
                                        師
       q11너J

               小文凡 竹m뇨／ 石笞
                               之凡 7乞 仄 ／了C " 尸伽且
     捕너mmK                                       石                                                                            成규f
                                       乙＝          /go0
                                                                 =       7   (7   rna14
                                                 2. 그9y느，1<              "    "

                         ( 久 工；f
                                                 뇨 /)




mhnnhny心m벼
                                                              그／7


旨麟無烈烈｛懈螂再解趣礁
                      日邸照烈螂解n師秘卿
                                                       如'm呼小”"”『"
                                                                『""’「’" "' '"""“『“mmH
                     巨歪  亡兀 肛－肛才 ema石尻 ea小 ／亡 如M兀 加늉
                      民 牙竹抗 m仄 友寸 /gOo ／띱Zqa 白斗珏仰；
                                 G)    든

                           (3)
                     0 ／枷나m급 cLl AL婉 m辰                                            M在二毗 今
                     -4加Jig 口斗 加 7Z凡 肛左，


                     柶dq                    KL- ioc{6, 고odA

                       F汕小 (/..q.2), X不工 ／코也나3 싸九； 甲
   州
   n
                                                                                        （兀尸
                     m《凡뇨乍m友／W/ C/h七AL／元 ／三， .

                                                            C F d]
                                                    =       K
                                                            乂     尸 目 \
                                              [s]
                                                        -   P
                                                            5     口
                                                                  乂＜ rF 1

                      丁k石人                 甲1 시 in1 )            Hi - i- fr尸

                       十戶
                                      尺L = jocL乃 ．              工 = r戶／ 二 /D <／乃

                                      Ri尸 ＝그Ocb/                工 = ／戶／ 二 그＜뇨／3




瑟 寨 m 1 批 融 艸 羅 ＼可



                                                                 ．只／8
                    CI／丹尸1石足                                        //

                                                     F-                         W 口／g), 亢A工 加Z：
                                                                                              孑 甲 尸小吼
                                              \'=                           T'+ Te. =                       3 c) + 그 三乙
                                                                        T2 +7는，                             77寸
                                                                                                              （그.50           = //. 6 57           -'


                                                     p加뇨 (/／· q) /

                                                     Te =                                 .7; -Y7- .                                  二     乙 十／
                                                                                                                          )
                                                                                                                                >/
                                                                                                                                                        '己
                                                                                             Y- i                                           7; * 7色

                             丁e.                                                I         ( ExAc-r)                    Te (.95 'i-)                 Th O. ocY)

                          Sb                                                                                          6口 2
                           75-                                                                                        g只 9
                         jco                                                                                       //'. r
                         j zc                                                                                     i 'z g
                         / So                                                                                     17工 7
                          17$        -
                                                                                                                  20仇 그
                         교口0                                                                                     23三百
                         又丁0                                                                                     구 9r . 3




                                                              勺卜＼ U卜q
                                                                                和


                                                                        20 -



                                                                            /0        미




                                                                                0                           1     1
                                                                                                       50   ?c   /C>     /25느        ／三0    / 73        그 00   250

                                                                                                                         T근          （卜C)


                         丁뇨1,                                                   47t/4八／二似M人                                                             7뇨 T- i5a K,
                                                                                                                 Jmm 口亡am夕
               ＋八戶似교 '
                臼                                                           似Mm四                                 im刃乙           咆＋                 ／石乙 丁匕 =Y；
                                                                                                                                                            系 P 柳疋，?
                                             乂之 고，刀；Al너尸 日乂뇨才 /

                                                                                          LYe                      了르泊if兀) 乙Y                                       \
                                                                                           丁C.                   7毛（丁t e丁工I Y                                  //
亂
.   mmr竹   ,   竹．    ,   -   m   .       .   . .,.   .,.,,,             ,   .       ,-n   .   ,   ,,
           ft 3   I F茄dO友iWM兀六 7 如尻mM "
           Xm, /Mi .口. :         F兀小 든和냐Z刃 9; /, 크仄尼 d之L仰上b거'
                       升DQ 寸 " 6-/Id _i                       oc 二 (9. //<／易彷I.
           牛 白力小 亡加쿄
           크了X小工 力Z났 /-    - :< = . 그그（／乃 /

           R 6- -I/ V ;    Fd小W 二7尸M} 了，             dc =j5db加咐 ' /

              0-i/ 乂C :/,/5 dB／初 .    月뇨   X = 교， 30 dLS .


           CU，兀MZd七 UJ,G.:           F加M 恥샤／已 功／/ 尺5 “．口그6介 '
           1m나 (Lj!(33), 肌
                         畝I似-4屍乂 戶 Z／此 ／目7 mqm 辰」
           （七2鉀. 似， ; 耗 = 뷰／a- - -ieq· 小" ，느 可9又5-)

                                                     . OL72 N1'／뇨 二 ·／됴化／知
                                                                                  1/




                                              ):
             4c/     乂 = .30cB


            丁k‘肛， 才凡 小妨穹m                          如伊m        兀i ／札 m才
            C力，石山』,       而m兀 ；才 11.小4, 土뇨 上加才 4友i初d乙거' ·




小m如帥輞豁獅藩
                             F加加 (1/. /6기 才A之 力似乂 ／加工 多 a 石따y
                   刃뇨乙 ／在 J

                                         F ; t 十（1刃 七
                   IAJkL     T= TO           ,   F =L－二t匕乂B ＝二긋了9

                   40乙
                                   「＝!『·』；7（슬옰）
                           TOG-)                 F (d5)
                              0                     0
                            그 50                   . gg
                           百60                   / . 60
                             750                 兀 工3
                           / 口00                 2. 77


                    1뇨 a肛丑4- 口人乙 尸乙攷뇨／J깁余Cr; '




                                         1
                                         m
                                         =




                                   公견노
                                         m




                                         加
                                         미




                                         0            Zs_c   500       7SO
                                                                   T (<)

a뇩




汗긔心汪4니出州妃出쪄
                                                               774


              拿屯
                      //.   5h
                                       T뇨     J于似小兀M丈 仰4工 尸伽白 ayd                                                  <d尸
                                                                                                                         /
                                                                                                               d
                                 已，位 ＝案乙B = (1, 3Sx,o23)m5乙乂／D9) 二3. Sx／口“" ,,/

                      升 加七 04小兀 元뇨 刃伊七 力切y /i ／꼬才J7 Z丈j
                      IJB c万畔仰如거 em才. jydM
                                         已，力下 = 中／D'／月$1 = ./4HVt' = io小y나'

                      小           ／工工／抄小m                   m芎石 ／元」
                                                                                    /                 y
                                                                                                          = 75d6
                                                                                     //
                                                                                               /／入H

                                                                       /C)
                                                                                               '- '

                                                                   =
                                                                                           1
                                                                                    (' 3,5x比）H' 1



                      /n G
                                               ＋스＼
                                                     『
                                                         ／\                  REC4

                                                          & = /zdL3 키5. 오      7色 = 9次） /<
                                                          BW: /5061H 矛
                                                         ＼口 =q,/R ＝그 三／

小꾸




                      丁뇨 4切丘之 /今M兀 7 ／次旦 m口三／                                                                  口／' II') )



                                            Fi =／『午 기 于 蠶呈 :q.io
                      丁h卜 和小 (II'2I) _-施 m硫二毛 7今但 7 Z拖 帥m在
                      a4/ /

                                     Fd4= F' 十 吉 (r=/) 二 m5-/ 十 7／口 戶／ 二 2.7/




 小醫嘯發簪難州斟對對ai4＋ 轟
                                                                                          /5,




                割戡灘
                  呱
                                          = LL.3dB            /




                                                                        ;Z꾜
                  1L7    F如4-," (i/, 1L) X系工 伽亡나 iih甲n力
                                                        名i比 7 ·才石工
                  4乂兀乙k兀       a4   J


                         r, : ！느 - J0二虹／丁3小w)                             H , , C 1/ /
                           나    次B                (i, 3& 乂／0" ' ）伽이
                                                                            "

                  F加hV (11. 11) , 力뇨 加口比 戶7m兀 ct
                                                   才뇨 Oi寸꾸尻                                   乂4
                                                                                                   )

                       F : / 十주르 :/ ? 聳 ＝三 6又 : 工／肋 "
                  F-whV (1/.1G) X呱오
                                                       佃dJ ／十此 7 m ／白如
                                                                                         m
                  ／如兀    쨔， 7           (/.5北 =/'1)

                         F : { 十（L -I) 平 = i十（nqi-i)(聲）=1. V 3
                                         나    \
                                          J
                                                  'C




                  和乂不上 伽t4工 ／亨M足 7i뇨 力加枷小小 石皿
                                              口M乂
                  師円（尻 C加蜘流 在 』
                   Fc。
                     4 : F. 十古（F2小 = ／·93+49/ )r／·62-/)=Z.30 = 3,6dB                         I',
                  T뇨 小；工 凹七 따d                               1兀小／뇨 i蜘m仰뇨丙 丑뇨兀
                  m/ h叫뇨뇨 小）
                        , PC= (; 美B T 二 4嗅B（尸．/)7-c

                                              '-- 3SXi丁‘3)(/69）仁刃口孕7기＝S
                               -- (/0I0. 5/io )(1.                      8切。
                                                                          -/4.
                  -r小毛 M七qt f如七 .                         굿 1戈m ／未工 ／亡Wt兀皿 在，
                         Ps = 中 70</B初 H/‘됴71'B +／之／a = -74Z5닢8枷 : ／·／
                                                                       교x／口“//1d/
                  ,d了 尤뇨 i弑-J                     和亡比 fm亡t- Ct<.年才 /4-          1-
                           干小 = 7入／0" 나 = -72. a '乃力丁                 /




町的耐滋消哨無N乳黨出無瀜越斟
                                                              그73
                                 7-뇨   人C /314.力地I 甲 力뇨 ／机也 -iA出』
                      小                                         切，



                                  V                    尺
                                                           J"



                   T뇨 加磁I兀 加m三 4, 戶枷 /1/. 3지 缸a口／433),
                                   和 m &' : 饗小町 ,
          -4人r札在
                                  批 //4           尺F 石伊d 尸抑叱. 4M/ d勻.                        入小 之名又

            C衣4坪戶 44 D- 如才                             Z向弩及 乂；뇨 匕Z如Q · 乎 出e
                   tF 'V万亡邕7,e 枷                      X뇨 比TVe. . / L V, 쿄7k吼 名뇨
                   RF 四申才 和咐， d4 ,



                                                                                         }
                                                                K
                          =i L R4y小 빻 忌 k , 十 目（力叱）
                                                                                  /
                    P－瓜

                                                                            尺：＋小喝
                          = 빻已둑 . V心十J四        亡＝쁘亡 古(I十忌仄．) 十白' Gk5
                             "L (/ +RY心) +j幻qRU 2 (j+P.s／局9
                                                            ' 十／回G' 忌）'
                   1乙1dn卞，/ (it, 31) , 力뇨 C航4畔工 在                           PC-       如山W才 a立，

                                       " 勻： ' 띵" c =！芦才
         小吼k足 t7; tt                   只未t 肛口太 足F /k4.m力石，; 그／丁在am兀 . 7乙4 Ki
                                                  口              d

         无1d 蜘JM才 加4m 才不之 十兀M{7先乂 a그 ／兀J－口4七，‘；姓／.
         vik,              낫未工 阿枷ya 匕／』b났e M                                  4力m旅；/ . 无仙 가功材
                            /1                    U                                              /1/
        吐 Rs 和d凡d才 乂e 少C石자／e,/ :
         t




LTI
      fl hI:IUTTFFRlTTmrl如m:            ,.,,m如，                     ,,,,,
山
                                         5此                                                    ｛r亡七慽nhHHn拓K11
                              '9                   20,X66 ' ?7                0了
    IfrJOr) 노7                ' 方／                       尸／Yhr 'l             Q已
         "                    E드                         尸口／Y5 '乙              <D
                         （八4놔人） 川                  （八r) .‘겅             (Y)y戶工
                    g 97C7 '= 白Q/y力力I(。,.Q/）끄t二 .드갸거                          ( g卄刃이
                                                                                          꾸7
                   C沙小西吻4（却욍뉘月由加＋D 亡
       /＼人／A                                                                    ．
               /                                 .r才刃                       ＝끄d
                                                         + ,（쌍乃y구：
                                                                 r)
                                                             jA1            =7！으八1
                                                                                         幻夕／
                   fyr7f,7 f나枷까1) .
                                         I
                                     -       '               .r7m v/ + 5갱
                                                               bm.9; 十 ny      人 之 으／1
                                                      S町勻
                    { 7.Y :MI )I勿七刃 r1L
                                                   ｝切딴伊們 Y깍甲aM 2거上
                    (,y구 ."y7方
                     工H(11刃 "
                               쓰啞    fy
                                                           由   二
                                尸y ;                -t
                                                                   D尸그： V
                                                                            Ti丑． 小十士                      肛們i                           C4小 石之 4Om表乙. 如，
                                                                                  -V忙） = C七汕 口4 t                            十 (:dd/ 口스 t
                                               m ＜人比h丑                            LO ／仰沚                               d1I


                                                                                     l乞＞ 乙亡．) = et드＜, 口石 7三 ,

                                               T卜岾 X／也                             寸" 加肛七 加卒k才 mZ? 衣，
                                                    乂 二 十（ q4叫亡 十Ctm兀U：亡 卜 CO-tv L石才 ) 工

                                                                = 液［. 口亡 '4.), 亡 + C力＋' 山, 亡 十 ed4 ' m]

                                                                       十又 友 [ C力也口ii 亡 C加q亡 + C力4叫 亡 C.回Li.石亡
                                                                                                                                                         十 C伊句2亡d加따亡］
                                                           =                每 [. + C-亡也교叫亡                   十C恥a乙U：
                                                                                                                                        亡 + C,4a乙％      亡］
                                                                 十七 [ C力也（qJ'H口)L) 亡 [ 伽 （叫十伊D亡
                                                                                                十C力40,J,．四a) 亡＋C.口6刃냔畔                                                    )亡
                                                                             卜C- 汕 (LI.뇨크4.).）亡 十 C亡也（U뇨＋口功亡
                                                                                                             ］
                                               QZ又 呻따也 Cd竹나hm尤小 弔
                                                                  4刀仙』口小力（ 匕／伊《끄M(m,
                                               牛    幻1/
                                                                            nJ乙／ 뇨｛ 屹
                                                                                                  \1} J
                                                                                                      /




                                                                                                                       亨李人
                                         因八 +

                                                                                                          寸1＄ 人
                                                   亨1H요A
                                                                             孚     H
                                                                                   可＋亨                                                    孚和寸   N可＋ 寸




                                                           \
                                                           3 介 1 1 1 1 {1
                                            J
                                            人




                                                                        느
                                                                                                                                                                      “
                                                                                                                               ：了
                                                                                                                                                                  母
                                                                              $
                                                                                             $
    M
                                          4



                                                                             I
                                         +?
礪
                                                                                         N
U




    象拙發胡難繫罐髓蘿甲 餐警資i뇨芯雀n在北斜恥無
                                         (w,
                                                     , 反) 乙 ,                 的d     q7.         （刃汪－ 尸먀욕才小毛 石二 ．亡4丘 ,A.也m兀1
                                         兀，/ 싸十카出                                                亡 ' 石뇨 . 7仄亡7 Z在 在凡W
                                                                                                                      느4工，
                               mge小M兀）
                                                                                                                              :2:l,（口




                     咐         m          m    m          n
                                                          n
                                   기
                             /1. 10 1    乙二 " L; C刃口口j亡          ;   1厦 =    yb dd口（4／亡／夕．)
                             仄心 石人      (i(.qi) -UI. qc) , 力k皿 毋b,/e        (／乂,기斗亡． 44凡 ＜久／   』4yt乂，7:q/

                             1兀4-｛가4夕   町枷如力仇4 ／吟尤蜘｛ 加刃在，
                                        K中 i ：女垢 ' LCd皿m7亡－刃刃十C們』
                                                                            （口7亡＋夕－7了）]L
                                             = 友1石 ' [, dq人 '4) 亡 小 <：如的
                                                                        亡十口刀i
                                        人그    : H次ti-。
                                                     ' [c力4（幻亡 －兀） 十 C寸＋(A)亡／0中入7a月
                                                                                    그
                                             = . 次 l二 " [_ c. +&it 十 dM, (k7亡
                                                                                ＋万）] 工
                            民付了似 7及Z存쓰7 小小 力뇨
                                                 尹Zm勺 D C
                                 乙／ = 女l/rn 畦4瓜刃
                                               兀乙 = －矢 垢工 (1- 娩 44A0)

                            -4了乂椒 口亡率d 在． 놔＋i2 =
                                                 夜垢乙石《尸                                  /
                            뀨 叱 如나件， 小Z筑 a_                          匕 ' 切뇨Y ak 似比 琨工
                            匕｛的匙 C4A，너工戊， -t‘元Z/
                                                 力e/
                                             t/ = 珽寸, ' [ 白口句亡 十 d寸山（14) 亡／日）]
                                                                               '
                                         i乙＝次i,J '［乂汕 口J亡 - Cd<;tqJ亡
                                                                                ＋e月 L
                            Tk     .    zAr十M 7Z比危y今
                                                              石m幽Z凡7弓也付抄 玘 白少M泣：
                                               -(1 = 長呱1- c／十古C加尸）




나퓨員長旨툐甘在444作卄午崑由出斗甫日
                                               i 2 = 느液止工（尸 士 C力d 夕)
                            七力뇨 0位十d
                                                      4   q乞q = 尖寸，그乙加尸              V




                    雀4즈卒H




;
                                    心크뇨M如1 師4 元A工 文？八mW 乂石m才 7加｛ 如工 石
                      加
                                 口a』 如b乙 山也，
                               X未』          伽小ZM勻月 fm小da :
                               勺a
                                              싸   表 ( 寸： eD4乙I; 亡 十JiCo口口／
                                                                         ：亡）3         .
                                        八／ 食 ( v,l                  iTj           寸d3따 亡 C口毗U2 亡 十 町 끄iLd小m= 亡 Q呻노左 亡          )
                                        시 十 ( /1Ui ed4그口4 亡 勻4口7:t + 巧 匹 ' m口7 亡 c_ 1_ -姓 亡）

                                        N 套 [ 可 ' 坵 的(z叫．四n 巧匹" m伽imU
                     님了 尤k兀 /a／斫 呼 力人오 和r肛q자 石人 才A皿 兄幻丁 OZA芍뇨m


                                                   '
                                                    /tr
                                                                '
                                                                    r
                                                              v, j-2} J
                                                                          )
                                                                          '               /드）
                                                                                          \ "LJ
                                                                                                  '   =   6北
                     （乂d乞 X札才 /A兀 ／小m石i加／ 批和／伊毗W 加斗
                     口-
                          4,
                                    戊）
                                                          \




                                        ｛뇨，
                                                          >                                           1뇨十

                         m
                                                  M M                                     昆 = 6-?尻，
                                                                他
                       규
                               m

                                                                m                 m             凡＝C尸乏             Cc在口．q舛沆力



晷 d由烈M朴
                      m蜘 耐                                                                                                     m
                                                                              1
                                    r
                                                                                                                               m
                                                                          ma뇨 小烏叫／和河，／名：工，. ／了
                                                                                                                  m
                                                                                                                           7
                                                                                                                      耐
                                                                                                                 드工
                                                                                                                  3

                                                   e           －三乞 = 工 十 工G/ 中                                    그
                                                                                                                  叫
                                                                                                                          -7
                                                               P且
                                                          二
                                                                     下｛十 r13
                     右         乂不之 ot底兀니 尸如七 d                                                                 尤人e 小＋/7Z石끄

                     戶才 比1- ---i 7毛 小們가小U m,




瀞們斟琳母三弑裝瑟姿念聽麓小
                                                               玹．：乙多9 P三

                                                                                                      22-S




                 n
                 n
                                        I           -   -   ,    I                    / 1       1 ·        1
                                4七加知고yI X;i＼兀 C力／石끄乙거
                                                                                                                       I     .

                                                        /M甘m/ 口才 力뇨 C끄工ky吐
                                    J       1
                                                                            d
                                力k工 -4丑（枷次 A文p夕丑 (C冗M4+e乂
                                                                                  /         d                  尸                      1



                                              1/
                                                          乂旱  元뇨  4J{m,/ 在名뇨q尼）,
                                                           iJ
                                                                                                                                                                6   -




                                m               "                    7/   :   ＝       喀）
                                                                                                      「二
                                                                                                                                 rz
                                                                                                                                      )
                                                                                                                                          /／戌
                                 T뇨 比쿄白血品 伽儡44
                                               口才克名上 까巧a‘才 牛 Z次-e                                                  U

                                 C力4e力aJ/ M之／                                                                                                               r




                                                                              낙（ N근戶2- P,f " 江 咀／暫
                                                                                                                                                        ’
                                                                          \R：니Z6& L = 厄豆于／可乙手H
                                                                                                                                                V 工，l '
                                知m蜘孑 比ktQ比 17C如1 U/                                                                                             瓜 尸枷斗 , ／仄工 名在／
                                成加瓦'1 刃규耘孕e 在 ,




 L i L L h L m r 1 1 Lk僻侮健像小楹
                                                                m侮L 3 ／回프卜 , 回可入
                                                                      kV 工；+ -V 二" /
                                                                 n乙戊G7缸 (六 ' 士，)
                                布 乂k 力魂I m뇨亡끄므乙닉 肛，
                                                   亡乙 Ct唯d 在，

                                                            口“ 哥：磁4샅儡 寸）' 十多P-三
                                 丁
                                                                                                                                                                        小
                                                                          乙＝（뇨計러"                                                                   /



 國蚤嵩n朴럼出淨知聲撰彎
                                                                                                                           :l;n



h!   nmnmmmnmmmmmm戶nnamm比mmn小什nmm
                                                                mmm거mmmmn
                      P긔 F仰如 (/(eg) -(1i. 6?) . 才／나 口磁뇨 如｛a4md
                      平X뇨 da工m芬 c J a'tt: 小S(, S!:－易zs1J= .117/：프.
                                 CL= (s12. -dS17) H 2. 5 ' Z르竺1                   /
                                        isz니 工 니4 尸

              ·                  gL= I ;.2. S2,           I = ).37 .'
                                        nS2【n시d｝나
七；
                                  Cs= (Sn中心＼2느 .3. fl /                     ' /
                                        IslIll- --'비1
                                   RL= 1 SILSL , 1 =           2.53     /
                                       I 1sdt戶L4t I

                       F디kq}n\, (i1.71).                                                      卜／/

                                       ' K，二 卜 'S미느］S너1+ 江尸 =                             /, 3了 >         I




       滋雄帥鞠滋山 已
                                                치 Lu S11( .



              好m
                      dq;t兀 K> 1                              ，兀 才m仰白右乙
                                              口t44 ( 141< 1, 比／
                                                          ／右力Ze.

                                     s.'t =. g Z二2으        玩『‘3 Lz으         5:2/ 茴／L츠            S工‘ =. 6 /

                                 八 == '. 5-긋 Z二보오

                                 c-．二 46 c L2므                      忌 = . 79
                                ；·CS = , 6 gj         -               Rs = .9/

                        K, 二． 75-

                      4/d,,C兀        t< <i      力뇨 ／白m勺旒 4元 和亡4a多
                      加1.4加在 · a名力乞＆李 eM小 me尸名磁／ 表石可




     m量斟懈J明數塑淋求熬聲澄坪
                                                              ;3口




                        n   n             h
                                                                                                              mhm끼m1111斗1qmm11mm1114rt
                                                                                      m1七1戶mmm      11m
                                                                                                              毗




:dmd] a켰Hnn 뇌
            nH
                          OUT?ol
                 \,
                          Si,＼씨UT7                                  j)i FUT
                 .4）斗     Th ii F=
                 ！낫二노     1  寸 VH    mm1工Y 亡41上n                    ST只8w


                 璡聲표，낙旨＄月母하4 =,' d:. .; .: ',「1，幷느， ,,
                                                                    CiRfI
                                                                   1二二 !V中
                                                   蜘        t口na
                                                       t\
                                                                   1J   11   11   1d   '   .二   . 1   1   !



                                                                   n     1




      崔
      됴
      法
      發
      n
      恁
      斗
      九
      薛
      望
      茸
      弘
      啼
      鴦
      媒
      法
      m
      蚣
             Ii 15
               .
                       su ＝·65Z        .     ) Szi " 29/三으        , S, 2   , Q41/뜨'   , D그 그 二． 70/       "

              小才 吼以 4-名m乞乙占 :
                           스二 S11Sl2-S1t5L, 二 . 393L／五三"

                               K, = i니S.4尸니5Z놔 ' +1시 " = /. 긋6
                                        ;2 ( .SjL Si, !

             ．小；
               ，』e오   1스1 <i       <2M녀／- ic->: , ；하比 j乙2.
                                                         ，似i及／ a4

                                            4-在끄e 口才 百&H5 .

             F昨 4mm戶；似M 們h 】 元／나 Z뇨m노豌 m 切7M7m危
             mm友／,,J7 '. C5 = F亡 ，
              和-jdht (j/,g3),                   r$ = . g76Z브二
                                                I L, 二 . g 50J

              Tk工 d}M山 匈工 크和叭 ,

                                           G-s = 3, J9 )   &O

             七出山 的m끄 又初似小小 和k 在 6r =a7 7= /q. 7dBv'
                                   1뇨 4』             ,,q琨 C4硫규. 瓦，
                                       口｝기比． C叭‘ 口／ 닝，            aZ 汗C




m紫泓雛聾轟烈醬難小
              加斗卜瓦 口人｛和LA才 屈 -4才m吐 m石끄／:
                                                           ．出 入


                                   JH      H乍l
                               1



                                   1 . 1므g   ＝느
                                   匕   入

                                                                                                      /
              (SO「EgCIDI'1洪CT 如今t                       抑i+ 區n乞o!, I5：기二·ce, 6- =Jq,7d5)




                                                             232.
                         1/ /./6 1   옥／ ="IL브7므' , 旬， : 2. 2끄브 , 57只 二C/                 S그a =. 乙'LT立了'
                           1小L八工－．尤而너小Ji系， 石i- 乂伽加Mm力3M/                                             1-
                                                                                                          :=<:20,


                         匕hd 1三J 二 {S1m5i뇌 < { .
                         'd伽比 羌二4 ／나似乂고尻 a뇨 小江口方，
                                                교，
                               CS 二 SJ = .6 /       '      ;   riL - C-: $ 二· 7又L望 3
                         師4 尤A兀 如戶似伽 們如
                                        加-,                                                引，

                                6-i.似水 “ ，二，尸“" / 2- I
                                                   I-f，띠：:I' '口 “ ' "' 2d万
                                           ad4M咨
                                                        匕之 /,4q:Z/t C/；在，才 ·．



                                      寸＝工；:
                                           .    . 4. 十         j 'C= j．刃
J나U汁m




                                                                                                 \




                                 C- = 戶／       = /, y了尸／                   乙＝ 已x& = . 7g 커月
                                      乙J근o)노                                    丘J



                                 k=    二르으＼ < .7正，꺼／/                      /-．二 m근0      = . 98 才，H
                                       0J t노                                   (：比 t>L


                         (sop啄ComPAeY 蜘今白 多'W4. l.Sti(＝·.;;, (S，니＝
                                                                  ·OO
                            G = {2. 2dB / )




  蠶秘씨骨m繫出咐 4唾冬母寸屯小好촤註交


                                                   73B
               ! I1. }7 ]     Stt＝·6 1    ' ;         2i：又．27乙르三 ; J/7=0 j S二그 三 7교 乙： 旦큰 '
                             G- =/odB ,   G5 二／<／乃                   j       G( : 그c/B

               님-4뇨犬工，          \C＝口0     口n,<{ /4j <} / 力뇨 才， 《刃＜；力1.
                                                              4．

                                           .4乂b力／e .                 干：加：I-.八， (1/. g8),



                       G」小따 " 古n;
                                                                                                I
                                                =/,
                                                      5_
                                                                         ;     G뇨，  ,d尹   『

                                                                                              ／나뇨L/ 乙


                                                                                                           ／心t 뇨十七
                卞和 G5二／dB= I」2G                                     0小0{ （뇨＝ 그d乃 =I. ."/


                            (/／· gq) ,
                                          和 노：:- ·？7: - . 品 "g은 U6"
                和M
                                                           =1171느                                   rmM尹




好瑟辯望好轟卄蓀n
                     丁kh X뇨 四也-4-                          蜘J m／友 甲 力뇨 m比d

                     r反 蜘小 山工i i幻14-.'                                         그）' (//,93) ,
                        Cs 二 ·幻q끄7可                                             CL = . 6.2占／

                         R3 t .310                                              /2L = . 끄       9




難湘斟斛割凞斟萍＼
               ，匈江 &。    『 /O石7／了치／" m4乃 , 小d了 자皿 缸＝/ci3
               ’口M乂6L. ' Lc5 恥-4-叭 C似如 加iZ? 戶.. . - 的dZ
                秒辰 下 mdB·          小／工 e毛才 比뇨工 吼뇨 口H Z名妃
               ，名可乂斗L C未m才 ,                乙lM/ 不dk才 人 = ．고／百끄7으'                                           dXd八a/

                     VL ' '3GI／쯔芝 ／孑 如叫甲 月兀 m化升瓦뇨 7
                     丈M比         加石幽· 따也 싸向凹力也 匈兀(-.才 兀4-
                     匕｛刃／ 月／k기J九 :                                                  .0 q0A




 쏘亡瀑乳求案漆曲發나慈
                                                                              23q
              ( ' "『麻' OMP水'               蜘今仁 艸＋ Is미二，_c-J ISZ 니 .418 ,                                                                                           二
                                                                                                                                                                       G二／
                                                                                                                                                                         口DrY司
              (i.'L肛友小也 d                             如f,f 蜘乂 呻，
                                                               寸 』工似名 肛汕尤꼬1 /4之
              3mm 才孑 /Qc助




小漆姓出寸m
         ＼屯



         弩斗i
                                           }, 1』 U          1




                                                                                                                                                           ；쿄k發．
                                                                 11 , 11       1d   .J   U   1    m＝口11 t.n41       小＝中4


               已나．비巴. 4   1 '.   '     3
                                     , 』
                                                                b \'. d . . 』‘．
                                                                              느 '：二                                 U
                                                                                                                    J
                                                                                                                              1i
                                                                                                                              d
                                                                                                                                       1U
                                                                                                                                            r

                                                                                                                                                \H1   m口
                                                                                                                                                           t
                                                                                                                                                               :

                                                                                                                                  =
                                             ,
                                                 ,, ' ， ·
                                                                      口1 .          小        }:    L1     t;             L1   '             三         1    m
                                                                                                                                                           七
                                                                                                                                                           1
                                                                           1         r       J     n                1三             1
                                                                                                                                                                         C = ' ：今'
                                                                                                               Li                                              1
         1u.     Ig   1   듸！   ：·   ）」스므쓰 ;           요/         'Y.    3L互三         ;      SIL       '   ,
                                                                                                              ""   "'   乙2쓰   I    5!
                                                                                                                                         !   『，   y5亡프 "
                F加m (II. 7) 力n工 如m友교 尹r-                                                                                           ／才 m,
                          U;        ［욕7_I 152_i I IS11 j됴니                         = . 口了6
                                (I시s4iI2) ( I니S피 ' )


                4r 7뇨m (/ /.86) 力뇨d 小蜘L4 比友丑 刃乙나t ／뇨 &r/ Gr)

                                . g'77 = 尸二小. <                                으二 ,/
                                                                               븟二    그
                                                                                  < 尸二 = 1. 122
                                                  石；iDL \ 6丁口 \ (i- u)

                                小 . '17ci8 < （升 (c(비 戶 (rTu (/ B) < 万q佰

               d了 光1山 J/ :n，
                           巾                       4石力k丑／ 石七 皿44. .才玖戶_ 凡                                                     口. 5cI乃．

               [lI I9 1 FA力加 (/／·gg仄） 口小a (//.i74) 』 小凡K 口S                                                                   =/        '.4七七     人切七．         7



                          ：乙 ' 卜／Sn／工
                      85：二｛                                                          j 卜和 -- IC, I '-
               넣d/ (/ /. 7a) 4e亡／
                                ｛乂亡J戶／ ．只늉 )
                                    =              /＄」／'                            욕芦
                               C5                                      '共二
                                              ,
                                        (/
                                                           )SI
                                             ] 니Sjq                               / +／万；Jl
                                                                                        I'


撰                              忌=            tS.d (1기Sm ' )                           Is1         "
                                               1니 s',I'                             i十 냥M工

               石 力뇨 J升m乞K 7 才K名 口M4烏才叩h 口-1乂沌 dk亡m小4+J

難
                                      1--Is눠: , :511/
                                    ms_i           1
                94山 小Z丙됴 ·沅；力侃 J乎小m名枷
1
                                                                                                                              (7i>C石｛44/                 ／盒／
嶺
齟
                r3=O , 크了／玖月 加危 m仍4才尸仁／玉加多人
扮
                크／나            亡／磁乞 二t 乂名工 M也才4
：菽
掛
批
꺾
叫
m
n
鼎
掛
塑
伽
啞
冒
黨
     n
     m
瓢
                      ! //，긋o}          凸／ : ·7出                   ,, s/i :,.2乙三쓰 ,' 毛戶』
                                                                                       ．끄뜨 , ;,,
                                                                                                                       L쯔P '
                                        Fm나， " 2. cds , "                 Fb7q才 二．7 /            .   .·     t,J =／三工
                       Fm少
                                        小k次 m航4 :                                      y =:,o7       .    i三1 = · 5J

                       小M凡工， K>!                   cz .eL 1JJV-           , 力뇨 ／切仄e ,<<,
                       dj:h力／尸． .


                                                        仰毛 /升乞                               啣W           ／乙1 G ＝凡片 “· 7i生쓰

                      r뇨牛 加e 加딴似孑兀 們m ／午 白낑뇨伊脆 加南닝 上征
                                                下二，/1，
                                                     夕J于八／         (/ /,g7占） )


                                        따（뇨21L三
                                            ：‘．丁）'                                           = · g7町         ．

                    和尤A兀 'V才口七／今M刃 m꾸娩
                                                                                                 F寸4(              쿄已 知／Z挽.
                     們咬 mZ? 衣，
                                          6-了 = . 1- 汀이二．,                 1
                                                                                   S1IIl   1- LSt: 2m
                                                        r11 "    I I, S2玎기 '
                                                   나s11
                                                = (I. c乂／二，zs)佃．刃） = g石．3
                                                                             = /Q.'/ ds
                     缸們b，奴和i訊g 小 小d左 m/ :

                                                                                                     . 그 99
                                                       入                       H
                                                                                                       入


                  (cUPE?.C毗．PACT 小午i4 7小
                                       （[5d＝」33, ／尻긱：·13,
     泣繫寸口m發洑出小n
                                   b'
                                                              1/
                   G     =t乞7c6, F＝교，52/8)

                  (r+            和乞志K 丘 久 石比／
                                             伽幷乙 亨 둑1 d교 肛才 -z二7吼
                   无뇨恥 6- =ig.do)




                                                                                           737


｝資
h낙1口at그1t끼八1;:r1          ；了1朴nnnnr\=1nr1r끼r1nhn:1r1r1n＜끼nm기r叫
               『，h켜m1nm1=1·                                    1t7r卞｛?1
                       r   .                                 .

                           'L2! ]               SI{ 二 ' 乙／                 』 S 2.1「고乙引                                 ; 丸= 0      j 5mL刀프으'
                                         그
                                                '"仙＼ "a" 4B ; 닥少 162 / - '                                                    ,· e시 ＝그0 .r.
                                                 SI1 二 0         m닉 t5m5띠 <!/ 光A毛 'ZEVk丑 乂2
                                                                          ／缸也 ·                                        丁M mm/            궁qM 乂4-    J



                               G-TV = G5（뇨G( .                            -t力攻eU, G. = I5LI／工 : 1/ = 6如．                                      ,4
                               e5 十 (5/- 二otJ .

                           P石十 伽q七 烏毗 m뇨 7伉                                                                                 戶＝ 印0/ 구oS; 兄 그 J 3. o dB '.


                                                        1 N
                                                    「교
                                               F(de)                LCF
                                                                                               1RF
                                                  卜
                                               乙Os-                                   1
                                                                                               n나H
                                                                                  1
                                                                                                              0?
                                                                                                         .
                                                                            .
                                                                                               1
                                                                    r
                                                  1
                                               z．乙0      '
                                                             053           石I /           4'             J8

                                               3. Oo    . 30              .Yg /                      .   '/
                                                                                                                   0


                                               긋 . 00        0             . 62끄쁘O                            0


                                                                                                     c- 뇨                   7石乙 口5 " 6工＝口 dB :

                                                                                                                       （孰－柑小卜 = ／· 96

                                                                                                                       和 = . ;io
  呼
                                                                                                                       CL = . Lj7匹쓰




六莽簧難嶽烈甘崙蜀刻澍斟斟크斟滋熬轟型瓠
                                                                                                                       ／근L. = . // 7

                           尸h七小 낮云出 口入而 匈之 小드 石尸九七                                                                                      d4／亡t,t/ -亡뇨

                               I- 『 RaB 肛；
                                         寸 4                              UU之 C兀me ri : . 66Z뜨트' . /3 : . 6그L（으r.

                           rh小 小                        -4兀rt4J ci i                                          F         2, o9Y3. M南k5 婉4교4南j:
                                                                   노36入




                                                                                                                        구3',-




                               r1n n!   n1mr
                                  m
                                  小
                                  Th兀 恥q m/ 4功：됴고 Cd祇＋ a凡J：中
                                            i
                                            (
                                             「""' 蜘／戶/ 戶虹
                                                                                                                                                      U                    Z

                                  (.""「 "’
                                         巴
                                                                                                                                                     <
                                                                                                                                                     7                /b
                                       =
                                                                                                                                                                                                   /e
                                                                                                                                                                                                        卜
                                      尸 1
                                                                                                                                                                J
                                                                                                                                                                                     C
                                                }/
                                            =                                                                                                                                            l              i
                                                                                                                                                                                                             1
                                                                                                                                                                                                             /
                                                                                                                                                                                                        ／
                                                                                                                                                                                     /
                                   L）中 누 (Q.1qd ) F                                                           = 不03 a 'B)

                                                                                                                           4
                                                                                                                                                                n 11
                                                                                                                   0
                                                                                                                                                                4J1
                                                                                                                                                                               b
                                                                                                                                                                               0r1




                                                                                                        a肛丘盒1;4
                                                                                                                                                                                d              九

                                                                                                                                                                                                             노



                                                                        已,：뇨르m熙嶺m                                  !


                                                                                                                                                                                                                  r1

                                                                                                                                                                                                                                갸八
                                                           仄 堪：..w.                                                    小글L



                                                                                                                                                                                                                                             났m낢挑m
                                                            /                A    A느       = -a-   口＝1m나17=   ===＝心＝   크a11! 4中4=          fl =aW_   i. 只1=P1= ==P         ；口111= 1＝ 小        1= 1戶＝ ＝江                 \       뇨


 i                                                                                                                                                                                                                          \



                                                蛋小
                                                           /4小q                                                                                                                                                IrvA
                                                                        ;f       1 r   쿄＝ 크小如小           1크b小亡.   뇨코스十쿄m！四寸1뇨m뇨m1戶뇨戶뇨戶：
                                                                                                                                      1꺄肛＝4m44m口＝                                        ＝뇨m＝ 小＝            41乍1; m




                                                籌小i

                                                                                                                                                                                                                                                 無叱斗났囹濕涵囹
                                                毒燾mm
                                                小
                                                                                                                                                                                                                                                       1
                                                                                                                                                                                                                                                       =


                                                                                                                                                                                                                                             아吐


                                                                                                                                                                                                                                                      ＝
                                                                                                                                                                                                                                                      芍； ／江＝
                                                                                                                                                                                                                                                            0



                                                                                                                                                                                                                                                           느 n




                                                                                                                                                                                                                                            咨三



                                                蟹小
                                                     ．多小
                                                                                                                                                                                                                                                  多
                                                                                                                                                                                                                                        느




                                                                                                                                                                                                                                                  ／
                                                                                                                                                                                                                                    已
                                                                  ：小娜
                                                                                                                                                                                                                            n       나
                                                                                                                                                                                                                                    1
                                                                        二a
                                                                                                                                                                                                                       月寸


                                                                                   :   b




   ！
   m
                                                                                                               "于"多沙

     기 4na14녀a 11노4rk玲汗4＝捺냔境煎mL
                                                                                                                         ma1t工Y       式사上끄 NaME1tR1




卜;
 t; j4
                                                                                                                                  i   1J   1     蜘      1n凹 H

                                                                                                                               }= ' ＝各                 1    y
                                                                                                                                                                                                                                                 ; 毋




   ;
   d
                       Il . Z2       S -Fma4m心又乙＋ 平 p/I " 그／ ,'                   F “乙5dB

                        p石t       F = 2. 5 </B         q似i瓦士 小O냐으 7今似兀 蜘左 '.
                                  N=.iqt ,         CF = . 593 /             J    Rc-    . 2P6

                       7Ln人F>     &뇨，外 = I. c6 " /; 인 4'I3             ) 6寸小.6和 “乙7二 = 2,9그 dB

                       由丈 文Ju工， 尸q右． cs/I斗， S쵸） ad寸 枷才 ／元 m勺 ／孩丑
                        F= .i.5d.5        ／之 ·           VV4 /           尸各才 石加工 們似 C (IL4 本

                       rn少 y才 ／뇨加石m 加i才6 짜皿 尸2·5dB 岫Lea.
                                 G-s = I.SdE                 85＝·9D5            C5 ＝·56Z     -      尺5 ' ·그07

                                 （뇨 “ 乙5d8                뭉L-『 .9o7             CL小끄므'              忌＝ ./',.3

                                  6-s =n北                    75 = .99오          (3 :.ssL三0           凡 =-I"?

                                  6-s =I, g0!8               우s 二. 97o          C.5 ' 万7Z뜨？          R3 = .1/긋
                                                   \



                         T卜吃     C.5 =／· gdB      a      J （多二二.2．드＜/8      C2乂）／』e4_      z人足   C石寸尼． 名m

                        O戶阮汕M (F＝二cda q硫乙） · 1뇨A4-, rs =.s 'g/ ,，丘 =.57/Z亡
                        汕亡役 y고／ m 7dA 甲 白 “/ * 十긋·5十（ ' /&3c/5·
                                  낫不 小，d76 A"
                        7兀嚥及勻 小a 小；
聲




    d竇蘭當招鸞蟹헒斟好브g望彗玄L
                                          下尸小뇨
                                                 .O11入
                                                                                 qtf
                                                                                 入




                         小P&12啣4(r 如和뇨 炒奴                                  15d「 ·「／,        {5' 나 “- ' 두，
                                      /                  /
                             C- ?IO,3dB , F =그（d8)




                         H
                       z3
                                        z ＝尸1j' X         J R> 0
                                                                           (P十品此 ，比戶七iaM,e)
                                兀才
                   .
              [I
                        n，上小            吾 ＝근／20 "C+j) - , r>0


                                r   二
                                         뀨      Cr-i) 4-j 7(
                                                ((4n4-j x


                                         Z n尺十ix               』 R>.       m尸汁乞 力加m似）
                       中t：才玉女
                                                                   r-> o


                                                  : 中（r十i) 十J 工 二 (r十i) -ji'
                                         1' = 壹그                  am U X
                                              3十（   C- Y+1) 十jx
                            小
                                        I -    Cr戶D十j%             )

                                        C竹     (r十1) 十ix




                                                                              小 小小小
                                                m 小
                                                       .4444八꼬－尸       7乙小 肛 r 戶 ,如吃毛
                                                                                      J2毛d/2/i小七e
                                                    兀乞吃 em4八， a肛乂 力뇨

                                                                如｛ 小包伊才                尤／4
                                              M刃們只勻乞 ,
                                                                       小m勿七 -z姃在丙
                                           勿形뇨2d " m
                                                                                              /
                                           Yr半 .                                                  m
姓m澍滋m撥羅




     斟刈瀏
       뾔觀乳
         巍
 露
 饗斟1
   싻釉刈
          1
                1긔               S1:：·9a互으 ; 5ii＝乙6庄브 』尸玩＝. .2/：쯔 ;5::=.5/y




                T凡 m和才 d砒U巳芍 屹也 4 :
                                        CT = 8.D9 /

                                            只1 = g．그g

                F4<nM/        (ii. s-9') .
                                                   = SI, 十   易工S亡／ /;
                                                             / - 5i工 ／구

                C工四如오· FT 桁 ／뇨才 (FT I < { 口“/                              乙뇨 di 石加！
                                                                                   ． 乃,
                      .   .
                                                                                     /r
                                                                                            口
                -t兀（dt mM士 mma乙／ 才0e 肛石，
                                       才                                  r구＝. 9L끄可 . 丁사，
                                                                                        1
                      r二M ) 比／日匹0- ) 的 근人 = H／긋- j 25人‘．

                ／닢寸
                                 ?L. ' .R丘／a 5Xq = 4' Lj . .5- 4            = 乙Dg力'.／百忙.

                卜1ab／나              m刃뇨虹 似                         《才，.
                                                             小a긔 C人，
                                                      ·二S吼＼
                               .c그4入, '            1JmH   卜才中
                              1     t        1     4      4 rh 5 百口
                                                   h    그87 I I 극 -S乙
                                                   그－m       入 U 4=




口m냐A唾棒1콧出口쿄m!




                                                         그Lj3




   ’小mmnm1n1卞1mmnnnm1nm11i叫 '- nnn1t只까1nn
                                                                                                      （上) 乙4 = 7. 5 s戶


                                                                                                          油4』
                                                                                                            · = 7유6人


                                               5 LU1了乙卜1 (＞卜J
                                                                                                                SwITCH            OI '
                                                  (DIODE OFF)
                                                                                                                （工）loPE (9八／)

                                                               R
                                                           L=
                                                             C
                                                          11
                                                          房븍1 芒
                                                              1r
                                                                                                                    阜：
                                                                                                                              :
                                                  극爻 = · 5-i 72九                                     乙X 二 . 3+j 7. 5J노－

                                                  'Id = (oq6力'f3. T)入,o"3 S                          YcL =（드3 口’ I33) X/OmJ S

                                             毛    仙小5只 戈뇨 加烏디 油卄 7Z Z兀 口V 孑力左 ,
m
塑1
                                             /d   尤h工       4友／尸 -4小ki戶Z瓦m兀 /e Ys                                -j .0131= -j.6尸可；솥m
                                             和 兄뇨 片左＋ 乙／ 1 石札此／ ／亡 /
                                                                                                                         = · '/03大 .
                                             缸 力뇨 C시               4力d立 , 光뇨 4/md小竹C교m毛 4i ／而꼬
                                                                                               ，,
                                             근 " '兀D96자' "" 끄9 "'7」
                                                                  니 4日掘小而；小小戶그.J13力
                                                     IL      -=--;?O    J 7균 )
                                                                        i R금 1= 근C {
                                                                                       =       .
                                                                                                   0긋／    北

섧                                            J.4\ ，尤伍 0F1          -4先X乙 光凡 Mm才 石y小似                                                     d才d=
                                             和．그q', 十弘石皿 』 4寸 比뇨
                                                                 a汕q友，
                                                                     1' _&c- i- --c乙‘

                                                                          ! 72 1               二
                                                                                                    //.   7c/
                                                                          1그근 ＋근0          ]


                                         蠶
                                     崩
                                 蟹
                             發
                                                                                    2qq
                         舒
                     臺
                 나
             等
         峀
                                                  帥
                                                  n
                                                  好                n
                                                                                           m
                                                  邸                m            m
                                                  n
                                                  帥                                                             r1r1 m1+ ?1
     誌
              i 1 1 2. C,
                                                                               （工2亡／ =／互：工L

                                                                                1治뜨i = 긋65J乙
                            SIJJ] TCH
                                                                                    5（人i ITCt寸      (9F戶
                                                                              .j15fi- -jZ至f .5-)-




                                                                                   ．드；긋百Cl皿




                                                       （
             ABW 他i乙刃                         二：二j互
                                                   긍
                  rA
                  [cj1七。 iJL '/' , iOI4 I+ 1/ 2 "Uj1
            (：師仙才 存              S又／ ;
                   5二4 =            a
                                                                                                            又
                             A十B／큰. 1- C. 근. -fD
                                                                       口2
                                                           /＋已／22.＋측／2. 十
                                                                                      毛／(22+ /      7구     已+
                                                                                                            玉   르乙
                                                                                                                      프
           C）人／ -4之（枉 '.
                                                                                                                     근2.
                                    乙i = . 3幻' /5jt
                                                               ;            근2. ＝· 5 :J 그了0 ,j그‘



J4싸쿄漠陛崔咬
                                        S工1 = . "5-口r
                                        工t小 = . O仕4 d多

     m戶    OFi=     4才.4才兀 :
                                    군｛ 口．5-i교cOj乙                  ;         근J=.3 +'/ 5小中

                                    St1 = .1ig /

                                    工L = /8. G 낮i3




                                                              갇｛5




小斟赳明冊甲田附出！:mmm升m娜冊nnRm가n"螂mn1i下
       ft 1그




         f乙tdh勺 (11( 11 q) /                               Q:){l, Fe 二 寸6

                                                           2e = 夙 /／石i二

       加佃兀 6 /i                               /A丑 佃小／夕Z J才小 如肛尹／小m乂
        F云2/ 匕ii뇨／Z4-'                        乙月J /              b : 寸3 口才夕

                                                           C<)d日e = ）勺 Cd，才夕

       下乙l, mm뇨                              口FF1                b 二 Z3 t뇨＼夕

                                                            d,M万e = 尸y3 亡a力， 6

         戶              4中 : 7万 ' = 白t ' 付댜才PJ- 口＋i寸勺們刃                                                                      m戶少勺

       和乞之 乂未丘 足才k又느如‘ 舟 ／二뇨ZHm닉乙4七切乞 ;
                                               9       Zl中

                                             n o'      73 "
                                             1그力 "   960
                                             \ 3oO   900
                                             ［그又 ' 」  LLq, 30
                                              t2尸    '1s . 又0

       ／닢-。／又랴                               D 二／긋／0

             C                               外3/ 0          和叱                      4/              「   ‘   75   "   )
       J4烏니 乙如 戶                                                        夕＝／긋70 .'

        '224邪                 (/ j'. /1go) /
                              그                                   그                                                      2

        S2 "          月＋B／근       ,   *C근.       寸n-   H   B근，    b勺，     (I_   B   '근층）     ，乃근.
                                                                                                             乙2b +j 仁小z)


                                                                                           2q(,



liLi    n,   n   m,    nnmn   .
   1 S너 ' =         JI
              9万t 十 （교m627工


PjcvE3   OAf           b = 尸｝今 Co才四 = . 긋0

                       V工．尸 = . 97f76
                       工 (.+ 二    ·0하7d万   八／
P!0D6S   OFF :         b =j7.     0 = -;.555

                       1S24工 = .977

                       IL = ./0ac乃

(sUP&RcoMp4c,r
               如今4 艸   （ 工乙Ot -0Ya7 ／小， = ./<7／乙了' /
LL.半F= ' md召
             ) ／升 56· 7 ):    .
                                   '




                                  2幻
                            CH#WTER                i그

                        /2.1                 F뇨石）,V       (/2.／力 m/                     口.2- 1/ ) , 兀뇨尸如m,                                              小m三
                        7幼                   口M,       匕Z4《危，
                                                            m,                  ，亡幼：:t7{         9似k 口


                                                         5 = ／乙m今                       1/\/／勿7I

                                                             ',irr 工
                                   /
                                                       6- =             9irr巧 = L/)r (c 이' (I, 그71<／口6)
                                                                           .
                                                                          夙；                       /OO




                            Ia. a                                          r
                                                                           드                J屯 r
                                                                             4n 夕 e-                                       O. .四드 7口 4
                                                                                            =
                                                           E万




                             r_ _c1_ (I乙：入 (ILl) : m
                             二n,
                                                                                        /m亡年
                                                                                                                      /(41
                                                                                                                                I



                                                   p=                    竹r 乙m水

                                                           1"尸 叱列 伽夕d誼／
                                                         中 二t) 日二乙

          m
          心나
                                       F妗4．中） 二 r工 5m, 戶） 二-r竺I自 프二 次 4烏z夕                                                          74乙 ＜丁 드 夕5兀7又．



      1小L杯h恣小汁娜發娘뇨
           i
                                         '
                                                                               1o
                                                       됴仰們 ; A

                                                        J2                            5-'- k」&a, :,ir,i (i'-)= /1rA/3
                                                        5-- - .171F(9,/ )』4。d9cL ：』i거9=o
                                                          o 5 ro.
                                                       {：三＝


                                                1> =          L/7r,            二    3   =       i,'. 77 ‘化       /
                                                             的r月；(3



       헒斟業渽md

                                                                                                  叫8
哺
占                                             mm. .m     , , , m   ,,   m mmmmmm.       m如m,        m如，   ,   . , , , , , mm,   ,   , , . ,,,,,,,,.,.   , ,   , 如，   帥
4烏，
                     ,mm,    ,mm.       蜘，
                                                    FM加 (z.c), (I2. ,乙 n4aO乙n) J
                                                                                                                     (G= /5. g ; a =.0375 v11)

                                                              I노 =Ae S= GA' 5小 (／드g7伽.3
                                                                                        7刃毖耐6J
                                                                                      qir叫                 的7-
                                                                   二3.59 Xib寸 w



                                                    已1小m, (12. /2J.

                                                                   丁e " Y? Tb + (t- ) Tf

                                       T6 " 七升如肛瓦J m뇨
                                                      兀們m島， 7 口功小
                                       Tb「 小7硫似4 屈Y如友m
                                                           尹 m斗mZ
                                       T中『 p人們毗 兀伊




  4在豁旺妊資荏麒吐匕際降陀目nm旨自甘m其詐
                                                     ma兀Z 多 dm似

                                   4七U芍 戶 끄 :




                        쑈
                                                                     Te - 了／ " r2 （丁b 中丁r)
                                                                   끄＝ T尸－丁e 尸 只兄c尸3幻1
                                                                      T-f) 寸Tb ．긋q了小3-
                            / z . 5-    F加M i祉 日a丘 帥仇
                                                      馬4%小M    뇨a누 2白似危
                            半 0Z "了）, ／六七 4升뇨／才切蜘江乞 和
                                                                   a뇨，
                            和b Gr   Gr :／了 8" :63/0, 샤．口司似 , 尸卜：，可6 MV,



                             "노，
                                   (
                                        (
                                            'iir,
                                                     g)
                                                          -   2.
                                                                     和r   =   (4
                                                                               '7r)
                                                                                         (27,      ) ／丁'
                                                                                                   Z.
                                                                                                            :    ,
                                                                                                                     777   -   U:
                                                                                                                                    -1.
                                                                                                                                          1   d
卒叱骨1出出汁小二난哨i
                                                                                             2q9




奴nnm카nnnn心川小小m四Rn!nannmmt奴U,
                        r: _.w,&. (j2.io) aN( ui乙/i),
                            S二     Pq G-
                                   i7 /r｝戶 l

          +W 乂表上 似a如 力切小. G =17/0 =,D的                                                                      I



                                    5二      /0 (/c끼 -                                          gg9   '.il / 거工 =.og8 ,7m w/ c...   Zm
                                           功r 臼功 1-

         m       乂表大        仰珏石｛                    tt才石M                               /
                                                                                                 G. =/. ' 돈石0 = 3/.',
                                                                                                                        /


                                   S=      JO('3/.17)                        = .0. 2g ,v/，거 : = . 口C招 什W/c叫
                                                                                                                                   工




         i 乙7




          F_.t7- -v (/ 2,/o) -(1.2.1/ )」光凡 和七勺匕蜘芬 amm才
             m
                                                         :; 二 ／갚 G亡
                                                                        9r荏

         丁h毛 m毗山（ 伊m 比m喜 寸加mm2似

         小4小孚 (1.2. a旬，
                                   5r = e亡e亡 丁伍旌戶已 d力



             g
                                                                                                                )
                                          （切1) 工 忌工 心

         /＜力4\2八工               ，升1 石老됴 4初亡d' . e仰似／뇨k沅i
                       丁（日亡，旽) 6.                                                                                           弔           私工


富                     4恥机 口才 夕r, cir -0r白t (21t 戶di小才 力7Z工Pe 口才 旽／在 . .7-知如



藿                   4 ZLdF切切 蜘／e 和d 小乍 /／교，7Y):
                          Pr : p亡 G亡升才丁（屯旽；까.／力                                                                     /
                                     (9才戶 心 忌三




                                                                   그5乙

     !




뇨，
                .,,:, , , , , ..;.;,，小小，       ,,:,,,,   ,   .,.   ;.   :,   ,,.,.   ,,,,,,,
                                                               i   2.
                                                                        9
                                                                                  Hl工Hr1Jl+                                                                                      ,
                                                                                   O                                                               Tr

                                                              UJ FLi八八， 口 f2q石工／                                             ai, ,Zi石 初7乙／ 4才 亡如， /＞伍 44之Z幻，
                                                              u：나七乙兀 mm才 （뇨仙，而砒
                                                                                ／戶叱 乂玖t m円兀丈 肛乙之 4
                                                              力m卄功（甘 仄十 亡 =Tr. 名
                                                              寸-r n                      /                  J-1          J       -r小          J                          .
                                                                                                                                                                                 蜘rt (at                        ／吟｛',t.
                                                                                                                                                                                                                   1J     a
                                                              I f'JL 4力如兀 口여口 4M丑                                                                               7G乙 民 肛二兀 -z尼名4吼                                         a七乙
                                                                                                                                                                                                                               7

                                                                                                           T = 及e之 7


                                                              丙                  力뇨                                                                       小m나才幼如                                         加力平

                                                                                                    /(m " 흩三． 듦；「
                                                                                             竺戶vz
                                                             匹피 「m如 (Ii. ??)) i凡 乂7y婉 戶伊4似，k                                                                                                                                   m今

                                                                                                     구M二q뉴 孔 .                                             7 (I差) 如 (r? 孑)
                                                                                                        a                                                     3入八）8 似m之

                                                                        長／         3                                                                        카又0 H/ i口3 (1그&片孑)
                                                                                                                                                                                                         = /. 6 긋／/y
                                                                            (,   M水-

                                                                                                                                                              3 \JO P4.j/ 41('

                                                              쯔트光4e 似4a斗                                                                  /m丘／ 규뇨
                                                             區id 「小 ＜小；九 力二교a ;：二二．
                                                                                                                                                                                                둥k9- J6oc                /1




                                                                        F下 = 侄 드쓰노                                             = /.口0 으뜨쓰少Pe) - . , , . .. -,/..
                                                                        '              (7兀73 尺q                                                                                                 -        m1 乂1 A ' '-1




              H 1 4 1 d 片 g 1 1 1 甘 1 h H H 1 : i ;Hhnn 1


                                                        U1
                                                                            = -76 d5m.

                                                             丁ht X八小，小aX乙. f的릭／小                                                                                                     ／口兀恥C' 兀10 " 70c/方肝
                                                             쿄늄／／뇨 三그亡乙名石｛ ／磁袖二 a/ 4肛批t, ma 2；뇨似mU끄乞：』

                                                             기m兀（戶才              ／七，
              :
                                                                                                           工 =                  入7 ＜丸뇨 , C- 76dB쳐J 十／口쿠B

                                                                                                                       = ／民8 口石 .

                                                                                                                                              그司


            '1.



     11七R

騙nR洲冊翩nm.                                                    ,m啣邸叩mm椰t,                 m1z'ic,     ' ',   q.   ,.'?   ,...p,'%fl fpflmprv.   t,   . ..   ,n-   ,,.   .,,,,.,
                                                                                                                                                                                吐1nnnnnrnTnt.       r-      n
                      프         口和 ／成eial,/ 尸乙虹 4伽d 加2久 尸d如1
                               S亡 ·              T뇨小 乂未-t                 小如匕（ 肛七 尹 ／亡二七
                              .4/          ／勻加 (12．刃，(12.6) :

                             F7 = S느 4e = S亡 쏘드
                                                              4,
                                                                   ,,-




8 工a｝ 弔 ／仄오 小十岫比 石小a뉵)
     닉乂코 0
                                                                                                  匕2Z/




7 乂名丘 尸如 沚 끄丑－名小小口C的伽今 吼
加力44- 蜘石M) , 多仰 乙小出a打和小 j兀
如k 加m 甲 , 月“G已· TN小 i不乞足心 m                                                                   辰 7和규

戶m札
                        (／
                             긋· 그5)   '.




                                                  =
                                                        每                 入工4二    /
                                           (J小
                                                                          夕2了H


      1   2.
                !24
                                 G =3I. e                 j              Gr = /OOO ·
                                                                                               m교兀‘
               F汕可口.qi) .,-砒 뇨砂乙 比／山 74m仰有
               /dL Z祉 cs丁                             凹-4兀 :


                              孚＝ 缶 町C-; 停）
           何' 尸6畿) '毗“，。) ，引                                                           = 了. 5' 7> '百尺    2



               戶才乂且 小努足 戶 3T/s=f                                                       L 尺『'丁7刎 '
                      （丁／S::;'- (                -缸 尺＞/5'J幻

                                                                    그5그

