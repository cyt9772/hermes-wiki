---
source_url: "/run/media/yutae/Data/퍼지 신경망 제어.pdf"
ingested: 2026-11-15
sha256: aa240dcbcdc6557df936734d767a8b71bf91b355222432ca37fb904cda520fdf
type: raw-source
method: text-extract
---

# 퍼지 신경망 제어 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/퍼지 신경망 제어.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 293쪽 | **추출 텍스트:** 560 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/fuzzy-neural-control.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** 퍼지 신경망 제어
- **Pages (PDF):** 293
- **Source:** 퍼지 신경망 제어.pdf
- **Ingested:** 2026-11-15

## Extracted text (all 293 pages)



===== PAGE 1 =====
                             （를 중심으로
              MatIab/SimuIiflI


                        이병룡 지음




      Nonliner PID
     controller using           Water tank
                           卜
     neural network      U(t)    System       >
∼씨
                                             Respons
     fl


===== PAGE 2 =====
퍼지신경망 제어
  Matlab/Simulink를 중심으로



   이병룡 지음




    미』P癬


===== PAGE 3 =====
퍼지신경망제어
(MatIab/SimuIin（를 중심으로）

.
2012년 08월 29일 초판 인쇄
2012년 99    03일 초판 발행


1 지은이 이병룡
~ 펴낸이 이철
' 펴낸곳비ip.（울산대학교출판부）680-749울산광역시 남구대학로m
                                     （무거동）울산대학교출판부
' 전화（052)259-2488팩스（052)277-3011
' 훔페이지 http://wp.uisan.ackr
' 츨판둥록제370-1996-005001호
                      （1996.3.13)
' w13,000



U
「이 도서의 국립중앙도서관 출판시도서목록                                   와 국가자료공동목록시스템
                     《OP)은 e-aP훔페이지巾ttp://ww;nI.go.kr/edp）           （http://wm;r .go.kr/koIisnet）
                                                                                                 에
             (OP제어번호 : C1P2012053922)j
서 이용하실 수 있습니다．
불법복사는 치적쟤산을 횹치는 범죄햄위입니다. 저작권법 제136조       에 따라 위반자는 5년 이하의 징역 또는 5천만원 이하의 벌금에 처하
                                  （권리의 침해죄）
                이 책의 판권은 울산대학교 출판부에 있습니다．
거나 이를 병과할 수 있습니다．                       잘못된 책은 바꾸어 드립니다．




ISBN 978.89.7868.282.4 (93580)


===== PAGE 4 =====
머리말




 퍼지 및 신경망제어는 인간의 판단 및 학습능력을 수학적으로 모델링하여 체계화한
제어기법으로써 학계 및 생산현장의 공정제어나 시스템 규명에 많이 응용되고 있으며
기존의 제어이론과 병합되어 제어성능을 향상시키는 목적으로도 많은 분야에 적용되
고 있다. 과거에는 컴퓨터공학분야에서 주로 연구되고 응용되었으나 지금은 기계공
학, 전기전자공학, 화학공학 등의 공학 전반의 시스템제어나 공정제어 등에도 많이 적
용되고 있을 뿐만 아니라 경제 경영 등의 분석에도 많이 응용되고 있다．


 저자는 기계공학 및 전기전자공학을 전공하는 학생들에게 퍼지 및 신경망제어를 강
의함에 있어 많은 국내외 관련서적을 조사하였지만 논문을 준비하는 대학원생이나 졸
업작품을 준비하는 학부학생들에게 좋은 길잡이가 될 만한 서적을 찾는데 많은 어려
움을 겪어 왔다. 어떤 책은 너무 기본 이론에 많은 지면을 할애하여 실제시스템에 적용
하기를 원하는 학생들에게 별 도움이 되지 않았고, 어떤 책들은 너무 사례 위주로 집필
되어 학생들이 설계하는 방법을 알기가 어려웠다．


 따라서, 저자는 그 동안 수집하여 왔던 강의자료를 토대로 퍼지 및 신경망을 공부하
는 학부학생 및 논문을 준비하는 대학원생들에게 설계의 기본방법 및 기존의 제어시
스템에 결합하는 방법 등을 자세히 설명하고 M.ATLAB/SIMIJLINK를 이용하여 접근하
는 방법을 상세히 설명함으로써 학생들에게 실제적인 도움을 줄 수 있을 거라는 확신



                                             머리맘 3


===== PAGE 5 =====
을 갖고 이 책을 출판하기로 마음 먹었다．


 다른 참고서와 달리 이 책에서는 퍼지 및 신경망 자체의 기본 이론은 가능한 줄였고，
학생들이 퍼지 및 신경망 시스템을 쉽게 설계하고 제어할 수 있도록 설계 단계별로 설
명하려고 노력하였으며, 퍼지 및 신경망의 프로그래밍이 어떻게 이루어 지는지를
MATLAB으로 작성된 프로그램을 이용하여 요소 별로 설명하여 학생들이 자신의 프로
그래밍을 작성하는데 도움을 주고자 하였다. 그리고 적절한 예제 프로그램을 통해서
여러 가지 시스템에 대한 설계 방법들을 가능한 쉽게 이해 하도록 하였다. 이 책은 퍼
지 신경망제어의 쉬운 부분부터 제법 난이도가 높은 제어부분까지 망라하고 있으므로
이 분야를 처음 공부하는 학생뿐만 아니라 고급설계를 원하는 학생들에게도 도움이
되도록 하였다. 이 책은 내용은 기본적으로 MATLAB/SJMIJLINK에 바탕을 두고 집필
하였다. 제어를 공부하는 학생들 대부분이 MATLAB을 잘 사용할 줄 알기 때문에
MATLAB 자체에 대한 설명은 피하였고, SIMULII恨를 사용하여 제어시스템을 구성하
고, 또 퍼지나 신경망블록을 제어시스템에 어떻게 구현하는가 하는 부분에 많은 설명
을 하였다．


 아무쪼록이 책이 퍼지나 신경망을 공부하는 학생들이나 산업현장에 이 기술을 적
용하고자 하는 연구자 들에게 실제적인 도움이 되기를 바라는 마음 간절하다. 이 책의
원고를 준비하면서 자료정리에 많은 도움을 준 김형석 박사와 원고의 편집을 위해 애
써주신 울산대학교 출판부 김혜지 씨를 비롯한 관계자 여러분에게도 감사 드린다. 끝
으로, 나에게 조언을 아끼지 않고 묵묵히 참고 옆자리를 지켜온 사랑하는 아내 황보숙
과 든든하게 믿음을 주는 두 아들 승규, 왁子에게 이 조그만 결실을 바친다.




                                   2012년 8월 15일 울산대학교에서
                                               저자 이병룡




4－퍼지신경망 제어
         （Matlab/Simulink를 중심으로）


===== PAGE 6 =====
목 차




1장 Simulink의 기초                              7
 1. Simul마
         （ 소개                                7
  2, Simulink의 사용법                           8
 3. 연속시스템
        （Continuous system)                 14
  4. 서브시스템
         （Subsystem）
                   의 생성                     26
  5. Embedded MATLAB Function A용            30
 6. S-Function의 사용                          33


2장퍼지 시스템                                    43
 1. 퍼지 집합
        （Fuzzy set)                         43
  2. 퍼지 시스템                                 46
  3. 퍼지 시스템의 구성방법                           48
  4' 퍼지 시스템의 동작                             53
  5, Sugeno 퍼지 시스템                          58


3장퍼지 제어                                     63
  1, Matlab을 이용한 퍼지제어                       63
  2. MATLAB 퍼지 툴박스를 이용한 퍼지제어                75
 3. MATLAB 퍼지 툴박스를 이용한 Sugeno 방식 퍼지제어       85
  4, Simulink를 이용한 퍼지제어                     89


4장 퍼지 제어시스템의 응용사례                          113
 1. 퍼지 제어기를 이용한 DC 모터의 제어                  113



                                        목 차－ 5


===== PAGE 7 =====
         （Semi-active) 자동차 현가시스템의 퍼지제어
    2. 반능동                                                     127
    3. 장애물 우회 기능을 갖는 다관절 지능 로봇 시스템                             144


       （Artificial Neural Network)
5장 인공신경망                                                       157
    」．인공신경망의 개념                                                157
               （Multi-Layer feedforward Neural Networks)
    2. 다층구조의 신경망                                               159
    3. 신경망의 학습〈training)                                       162
    4. 신경망 학습을위한노하우                                            168


6장 신경망의 프로그래밍                                                  171
    1 Matlab을 이용한 신경망의 학습                                      171
    2. MATLAB의 신경망 함수를 이용한 신경망의 학습                             183
    3. MATLAB TOOLBO×를 이용한 신경망의 학습                             187


7장신경망제어기                                                       199
    1. 신경망 학습의 종류                                              199
    2. 신경망 역제어기                                                200
    3. Kawato의 신경망병렬제어기                                        201
    4. 신경망을 이용한 기준모델 적응제어기                                     202
               （NN Predictive Control)
    5. 신경망모델예측제어                                               211
    6. ANFIS(Adaptive Network Based Fuzzy Inference Systems)   223


        （Recurrent Neural Network)
8장 회귀 신경망                                                      243
    1. 日man 신경망                                                243
    2. Hopfield 신경망                                            248


9장 자기구성
      （Self-Organizing) 신경망                                    255
    1. 경쟁학습｛Competitive Learning) 신경망                          255
    2. SOFM(Self-Organizing Feature Maps) L
                                          Al경D
                                            。。                 262


10장 신경망 제어의 응용사례                                               269
    1 신경망PID제어기를 이용한 압전구동기 제어시스템                               269
             （SELF-TUNING) PID 제어기를 이용한 수조 레벨 제어
    2, 신경망자가조정                                                 279



찾아도끼                                                           291




6           （Matlab/Slmulink를 중심으로）
     퍼지신경망 제어


===== PAGE 8 =====
1장.            imulink의기；




 ]. Simulink 소개


      Simulink는 Matlab의 확장자로서，
                             동적시스템 (dynamic system）
                                                  을 simulation하는데 있
 어서 그래픽을 사용하여 사용자가 더욱 편리하도록 만든 프로그램으로 다음과 같은
특징을 갖추고 있다．


      · 그래픽을 이용한 각각의 아이콘 블록
                          （icon block）
                                     은 실제로 제어시스템에서 블록 다이
                         을 구성할 때 각각의 블록과 같은 역할을 하도록 만들어졌다．
       어그램 (block diagram）
      · 마우스를 사용하여 각각의 아이콘들의 모델을 집어서 연결하면 자동적으로 Matlab
       code를 통해 계산되어진다．
      · 각 공정의 모델을 마우스로 집은 블록을 통해서 만든 뒤에 입력에서부터 출력까지
       각 블록을 연결함으로써 시스템의 응답을 알아볼 수 있다．
      · 주어진 입력의 종류도 다양하여 사용자가 지정할 수 있고, 출력도 사용자가 원하
       는 데로 할 수 있다.


      Simulink을 실행하려면 항상 Matlab을 띄워 놓은 상태에서 할 수 있으며 Matlab의 자



                                                   1 장 Sim미nk의 기초 7


===== PAGE 9 =====
체 기능에 더 많은 기능을 첨가 시켰다. 그리고 비선형 모델을 사용한 비선형 시스템의
옹답을쉽게 확인할 수 있도록 하였으며, 동적 시스템을 나타낼 수 있는 적분계산 능력
을 간단한 블록으로 계산이 가능하다．




2. Simulink의 사용법


 Matlab 명령창에서 Simulink를 타이핑하던 지혹은 Matlab의 초기화면에서 Simulink 메
뉴를 더블클릭하면 다음과 같은 Library Browser 화면을 팝업시켜준다．



             File Edt klein

              D 璲 섧 的
              Commonly Used Blocks aimu11nk,Comrnoni
             〔Jy．
                匕d ㅄ LH 느




             → 鱗 Sirnulnts
                                                                Comn〕
                                                                    1｀蠟 Uged Bloctix
                 奐」Comnronly Used Blocks
                 翌 Continuous
                 乫 Dissontinuities                              c nbnuouo
                 -nH Discrete
                   t닢 Logic and Pt Operations                   Dsconlinuilins
                   塑j Loaks Tables                     스＼
                   刻 Math Operations                            U1SonIc
                   塑j Model Veritcatian
                     j ModerWide Utikies
                                                                Logic and Bit Operations
                   彗J- Ports & Subsystems
                   土pj Signal Arlduitea
                   뇜 Signa; Routing                             Look up Tables
                   눌j Sinks
                     J 孔ur出｀
                   輾4 liner-Defined Funrhcns
                                                            玆   Moth Opmoliors

              …커 翔 Additonal Math & Di`rete                     Model Venlicalon
                 姓 Control 5ystem Toolbox
             :4- 珊 Fuzoγ Logs TooIbo4
                                                                Model-Wide Utlities
             + 只 Neural Network Blockset
             ？￡ 轢 Real-Time Workshop
                                                                Ports & 드obnyn!ome
             + 鱗 Simuink Contrct Eiesgn
             斗 只 Sisnulirk Estras
                 擁 Stateflow                                    Signal Atthbulex
             ！主」只 System I由ntificabon Todbxx
                                                                Signal Healing



                                                       沫        Sinks




8－퍼지신경망 제어
         （Matlab/Simulink를 중심으로）


===== PAGE 10 =====
 그런 다음 Library Browser안의 " Fil티Ne삐Model" 을 클릭하게 되면 다음과 같은 비워
   （Window）
있는 창      이 팝업된다. 이제부터 원하는 블록들을 라이어브리 창에서 드래그
해 와서 Simulink 모델을 제작할 수 있다．


          [三 untitled                                                                                  - ftr기찌
           Fte Edit 꾀ow &mulation FQrmt Teals Help
          ［〕 潘 日 ∼                                          노                     . 屛而－Nsrmal- J 蛋 巳쵸 圈




          Ready                                      =！由鬼                                   … !0de45




 Simulink 모델에서 입력신호를 생성하기 위해서는 라이브러리에서 sources를 클릭한
다. 오른 편에 sources에 포함되는 메뉴들이 나타나게 된다．

               드r 月 Simulink                                      ^                   Band-Limited White    ^
                     魯j Commonly Used Blocks                                 d町
                                                                                      Noise
                     辦 口ntinuous
                   r 葡 Discontinuitles
                   r 烈 미screte
                                                                        I             댜tirE Sign히

                     彗」Logic and Bit Operations
                     對 Lookup Tables
                                                                             ○
                     如」Moth Operations                                                Constant
                     辦 Model Verification
                     辦 Model-Wide Utilities                                           Counter
                     毓 Ports & Subsystems                                             Free-Running
                     對 Signal Attributes
                     辦 Signal Routing                                   Ii거』
                                                                           n Counter Limited
                     芝 Sinks
                                      毓 =；〕Un=e8                        t2,34     Digital 디 ck
                                     奐크 User-Defined Functions




                   +쫴 뫘 珊 珊 닙 發 珊 珊 只 8
                                     奐j Additional Moth & Discrete   untitlsd.,nt From File
                                     Aerospace 미ockset
               7
               +
               *
                                     COMA Reference 미 ckset             1 "1" n   From Workspace
               *
                                     Communications 810ck5et
                                     Control System Toolbox
               ＋
               一
                                     Embedded Target for Infirleon〔               Ground
               +
                                     Embedded Target for Motorolat
               +
                                     Embedded Target for Motorolat    （그 ［D In1
                                     Embedded Target for OSEKJVD

               +
                                     Embedded Target tor TI C2000 I
                                     Embedded Target for TI C6000 lv
                                                                       nn PulseGeneratsr
                                                                  》     「－        7    ,
                                                                                      円n:
                                                                                                           1 장 Simulink의 기초－9


===== PAGE 11 =====
 자주 사용되는 입력신호인 Step입력인 " Step" 블록을 마우스로 드래그하여 아래와
같이 Simulink 모델 창으로 이동하여 보았다．


          ['브 uni5ed '
           f긔e edit 甘ew 笏mulation Frrnat 工0이S 브elp
            0        盧·昌 l 乂 ‘怒 難 ，尸 啼 針：
                                        :2 ．'卜 湃 厄ㅍㄱ Normal               J 昱 므」田




 같은 방법으로 Simulink 모델에서 출력신호를 생성하기 위해서는 라이브러리에서
Sinks를 클릭한다．


          8 錢 Simulink
              翌 Commonly Used Blocks
              藝」Continuous



                       擁허至뽀
                  미scontinuities                                 Floating Scope
                  Discrete
                  Logic and Bit Operations            ［D
                                                     （그           Outi
                  Lookup Tables
             ∼ j Math Operations                        C         Scope
            …臺쫓 Model Verification
              坊 Model-Wide Utilities
                                                                  Stop Simulation
                j Ports & Subsystems
              輔 Signal Attributes
              辦 Signal Routing                                    Terminator

                     ∼彗포呱
                  1 J Sources                        urrtitled.mat To File
                 「 辦User-Defined Functions
                 1J 邕 Additional Math & Discrete       atm이』t     To Workspace


           ：延i纖： 纖
                 홰 Aerospace Blockset
                 nCDMA Reference Blockset
                 月 Communications Blockset           ！ㄱXV             Graph




           （Matlab/Simulink를 중심으로）
it〕 퍼지신경망 제어


===== PAGE 12 =====
 화면에 그래프를 그려주는 블록인 " Scope" 블록을 모델창으로 아래와 같이 드래그
하여 보았다．


             [芒 untitled ㅎ
                  f카e 丘dit yiow 墨mWa1on FQrma 1eels 虹미p
                  ［〕 哺 日 巒      y ：彖全 爵   qd ` ；… 드〕 ':   》 泰「面－ l Normal




                                   巨牙               口


          lRead
                     y                     mn鬼                       odo45




 블록간의 신호의 전달은 아래 그림과 같이 마우스를 이용하여 연결하여 주면 화살
표로 자동적으로 연결이 된다．



                  File Edil 냅ew 笏m미1ion Fmiat
          - D 峰日 叡             三    社斗    :. ,:




 위 모델은 단순하게 입력과 출력으로만 이루어진 모델이라고 볼 수 있다. 이 모델을
수행하기 위해서 Simulation>Configuration을 선택한다．




                                                                             1장 Simulink의 기초－11


===== PAGE 13 =====
                                                                                                                如


                                                                                                                견
                                                                                                                    ㅁ   匡
                     Elie 트dit 甘ew                    FQrrnat 和이＄ 닌elp
                     D 侈日 昌                atari                     Ctrl'T   늉 ！而万기Normal =i 留區i 固

                                           Configura如a Parameters... CtrluE
                                         /Normal
                                           ^cc이erator
                                           트sternal

                                                                   卜[
                                             久／
                                          Sine WaV숀                   Sc.pe




                                                                                               ode45




 그러면 다음과 같은 파라메터 설정화면이 나타나게 된다. 아래 화면은 시작시간은 0
초，시물레이션의 종료시간은 10초로 설정되어 있다．
                           샘플링시간은 variable-step 혹은
fixed-step으로 설정할 수 있다．
                     아래 예의 경우에는 variable-step으로 설정되어 있다. 화
면의 오른쪽에는 미분방정식의 전산해를 구하기 위한 방법으로 ode45 함수를 사용한
다는 것을 말해 준다．


   己 Configuration Parameters: untitled/Conhiguraliun
      Select                     Srm마atmn hm0
         S이Yer                   Start timer힙柄                                            Stop bme:itu,O
         Data lrnporVExport
         Op tin기cation
                                 S이ear options
      ＝궁 Diagnostics
    …        Sample Time         Typem                    Variable-step       뾔S이ncr.                      0de45 (Dormend-Prince)
             Data Valid띠／
    …        Type Conversion     Max step sire:          auto                  尸Slatine     tolerance: 1e-3
    `        Connectia四          Mmn step size           簿Uto                  닝bsolute tolerance auto
             Compatibility
    콰        Model Referencing   Initial step size:      lauto                 -
         Hardware 1rn미emnenI.    Zero crossing control: Use local settings V'
         伽d이 Reterencing
                                 □ Automatically handle date trtermtere between tanks
      = Re히Time Workshop
             Comments
             Symbols
             Custom Code
             Debug
             Interface




                                                                                                Canc이




12- 퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 14 =====
 파라메터 설정이 완료된 후에 아래와 같이 시물레이션 실행버튼을 누르면 Simulink
모델이 작동하게 된다．




 시물레이션 결과를 그래프로 확인하려면 출력블록인 Scope블록을 더블클릭하면 된
다. 결과 그래프를 눈으로 확인할 수 있다．



                 Scope

              昌白!！下〕, β           ` 個贈 ! . 1 萍

                        5



                            -'＼   ∼，   ./-\


                        a




                  .5e                     8   8   l0

              ㄲme 0nSet 0




 이상과 같이 간단하게 Simulink 모델을 구성하고 작동하는 방법을 알아 보았다. Simulink
를 사용하기 위한 가장 기본적인 단계는 기능에 맞는 블록을 사용할 줄 아는 것이다．
복잡한 동적 운동식도 블록선도를 이용하면 쉽게 작성이 가능하다. 원래 블록선도는
선형 시 불변시스템을 표현하기 위하여 사용되었으나, 기능이 확장되어 복잡한 비선



                                                       1 장 Simulink의 기초－13


===== PAGE 15 =====
형 시스템에도 적용이 가능하게 되었다．




3. 연속시스템
       （Continuous system)

 대부분의 동적시스템은 미분방정식을 이용한 연속시스템으로 모델링 된다. 가장 간
단한 모델은 선형시불변 시스템이다. 연속시스템을 모델링하기 위한 기본적인 블록을
알아보자．


 1) 이득블록
       （Gain blo아0


 이득블록의 출력은 블록의 입력과 주어진 상수와의 곱으로 결정된다．



                                  →
                 hi         G帥1         0uti
                        ！그림 1.1] 게인블록


 위 선도에서 출력값 Outi은 입력값 m l에 5를 곱한 결과가 된다．


       （Sum block)
 2) 합산블록


 합산블록은 2개 이상의 입력을 더하거나 빼는 연산을 수행한다．




                  h2
                        ［그림 1.끽 합산블록



           （Matlab/Simulink를 중심으로）
14- 퍼지신경망 제어


===== PAGE 16 =====
 위 선도에서 출력값은 입력1과 입력2의 차이값이다. 위와 같은 합산블록은 피드백
회로를 구성할 때 필수적으로 사용이 되는 블록이다．


 3) 미분 블록
        （Derivative bIocI0


 이 블록은 입력값의 미분 값, 즉 입력값에 대한 시간변화율을 계산하는 블록이다. 미
분블록은 다음과 같은 기호를 갖는다．




                ni      Derivative    0uti
                      ［그림 1.이 미분블록


 4) 적분 블록0ntegrator bIocI0


 이 블록은 입력값의 적분값, 즉 출발시간에서 현재시간까지 입력값을 누적하여 합
산한 값을 출력하는 블록이다. 아래 그림은 입력값에 대한 적분을 표시한 블록이다. 잘
알겠지만 Laplace변환에서 단위 상수값을 적분하면 1/s 가 된다. 따라서, 적분블록 안에
1/s 심벌이 들어가 있다고 보면 되겠다．




                ni       Integrator   Outi
                      ［그림 1.긔 적분블록


       （Transfer function) 블록
 5) 전달함수


 제어공학을 공부하였다면 전달함수의 개념을 알고 있을 것이다. 전달함수는 어떤
시스템의 동적식인 선형 미분방정식을 Laplace변환을 한 후 출력변수에 대한 입력변수
의 비를 Laplace 오퍼레이터인 S의 함수로 표시한 분수식이다. 간단하게 스프링－질량－
댐퍼로 구성된 2차 선형시스템을 고려하면 미분방정식은 다음과 같다．




                                             1 장 Simulink으l 기초－15


===== PAGE 17 =====
                                           mx+cx+kx= F                                                          (1.1)


 물론 m은 질량 C는 감쇠계수 k는 스프링 상수이고 F는 그 시스템에 가해진 힘이라고
볼 수 있다. 위 식의 양변에 Laplace 변환을 취하면，


                   ms2X (s)+csX (s)+kX (s) =F(s)                                                                (1.2)


 위 식을 전달함수로 표시하면 다음과 같다．


                                                                                 1
                               '   =                         =                   771
                    (!
                                           X
                                                     (s)
                         (Q
                    一    ' "   '           F       (s)           (s2＋스.                ＋츠－         )
                                                                                rn           γ72                (1.3)


                              (5)              , : ,         8
                                                                                                       H을전달함수블록을 "ㅣ
 예를들어전달함수식' m
                                       =
                                                                     '   따고하고
                                                                                                   '
                                       -       s2+ 4s+ 8

용하여 표현해 보자. Simulink의 Continuous 메뉴에서 Transfer Fcn을 드래그 하여 Simulink
편집창으로 드래그하면 다음과 같다．



                                                                 I
                                                               s+1
                                                           Transfer Fcn
                                    ［그림 1.5] 전달함수 블록


  위 블록을 더블클릭하여 분자의 계수를 [8〕과 같이 입력하고, 분모의 계수를 [1 4 8]
과 같이 입력하면 블록은 다음과 같이 바뀐다．



                                                                 8
                                               >                                >
                                                           s2+4s+8
                                                   Transfer Fcn
                              ［그림 1．이 값이 입력된 전달함수




          （Matlab/Simulink를 중심으로）
16－퍼지신경망 제어


===== PAGE 18 =====
 이렇게 해서 시스템의 동적식은 전달함수 블록 안에 제대로 입력이 되었다. 이 시스
템의 특성을 알아보기 위해 Simulink>Sources 메뉴에서 Step블록을 드래그 해서 편집창
에 있는 전달함수 블록의 왼쪽에 놓는다. 그 다음 마우스를 이용하여 두 블록을 연결한
다. 같은 방법으로 Simulink>Sinks 메뉴에서 Scope를 드래그해서 연결하면 다음과 같이
회로를 완성할 수 있다．



                               8
                           s2 +4s+8
             Step        Transfer Fcn   Scope
                 ［그림 1.기 전달함수에 대한 스텝입력


 결과를 보기위해 편집창의 Simulation>Start를 클릭하여 실행한 후 Scope를 클릭하면
다음과 같이 그래프를 확인할 수 있다．




                    ㅁ림 1.8] 전달함수에 대한 스텝응답


 6) 상태공간 블록
          （State-space bIocI0


 앞 절에서는 미분방정식에 Laplace 변환을 이용하여 전달함수를 구하는 방법과 Smrnlink
에서 전달함수를 사용하는 방법을 배웠다. 또 다른 방법은 미분방정식에서 상태변수
를 이용하여 미분방정식을 상태변수형으로 표현하는 방법이다. 스프링－질량－댐퍼 시


                                            1 장 Simulink의 기초－17


===== PAGE 19 =====
스템의 미분방정식을 이용하여 상태변수형을 구하고, Simulink에서 구현하는 방법을
알아보자. 식
      （1.1）
          은2차식이므로2개의 상태변수를 지정하면，


                                                                    4)
                                                              (1.
 식
 （1.4）
     에서 상태변수X1, X2를 한 번 미분하게 되면


                                  X1= X2                      (1.5)


                    ,,    k                   c       . 1 .
                    A9=- -x1 - -x9 + -J
                     -   I11 * I1l - nl



 상태변수형의 표준형은 다음과 같다．


                         X= AX+Bu                             (1.6)


 여기서，



                              x
                                       隧1
                                  =
                                       [x2j
                                                              (1.7)


                           1 0                    1
                         A=卜츠                     즈
                              L       iii         ru1



                                  u= F
                                      0
                          b=          1
                                      n1


 위 상태변수형에 대한 출력식은 다음과 같이 표현된다．



18－퍼지신경망 제어
          （Mattab/Simulink를 중심으로）


===== PAGE 20 =====
                                      y= CX+Du                                       (1.8)


 원하는 출력 y를 질량의 움직이는 위치로 설정한다면


                                            C= [1 0}                                 (1.9)


                                             D= 0


 위 식을 Simulink로 구현하려면 Simulink>Continuous>State-Space를 드래그하여 편집
창으로 옮기고 입력과 출력을 아래와 같이 구성해 보자．



                                          x1 = Ax+Bu
                                      >                         卜
                                          y = Cx+Du
               Step                       State-Space               Scope
                        ［그림 1.9] 상태공간모델에 대한 스텝입력


 식
 （1.5）
     에서 m=1/8 Kg, c=4).5 N.s/ni, k=1N/rn 이라고 가정하자. 위 State-Space블록을 더
블클릭하여 A,B, C,D 값을 다음과 같이 입력한다．


             〔즈 Function Block Parameters: State-Space
                                                                       刪
               State Space
               State-space model
                 dx/dt = ^X + BU
                    y 븍 Cx + DC

               P erame ters
                A   '




                B


                C
                [1 0]


                遂〕
                Initial conditions:
                0
                AbS이ute t이e
                          『ance=
                sut이



                                              CancOl    tleIp


                        ［그림 1.10] 상태공간모델에 대한 상수입력


                                                                      1 장 Simulink의 기초－19


===== PAGE 21 =====
 그런 다음 결과를 보기 위해 편집창의 Simulation>Start를 클릭하여 실행한 후 Scope
를 클릭하면 다음과 같이 그래프를 확인할 수 있다．




                ［그림 1.11] 상태공간모델에 대한 스텝응답



 같은 스프링－질량－댐퍼 시스템에 대한 전달함수 모델 결과인［그림 1.8〕과 상태변수
형 모델의 결과인［그림 1.m의 결과는 같다는 것을 알 수 있다．


 7) 기본 블록을 이용한 시스템 모델


 또 다른 방법은 미분방정식을 기본블록을 이용하여 Simulink 편집창에서 바로 구성
할 수도 있다. 스프링－질량．
               댐퍼 시스템은 다음과 같다．


                       mx+ cx+kx= F                 (1.10)


 위 식을 변형하면


                           C .   k . F
                     x =- -- x - -x + -
                          m      m    m


                      k=-4文- 8x+ 8F                 (1.12)



          （Mattab/SimuUnk를 중심으로）
20－퍼지신경망 제어


===== PAGE 22 =====
 위식
  （1.12）
       에서 가속도는3개의 항으로 결합되어 있는 구조이다. 즉, 가속도는 속도에
-4배와 위치의 -8배와 힘의 8배를 더한 결과이다. 위 식을 기본블록을 사용하여 Simulink
모델을 작성하면［그림 1.12〕
                와 같다. 그림에서 가속도값이 적분기 1/$ 를 지나면 속도
값이 되고 속도값이 적분기 1/s 를 지나면 위치값이 된다는 것을 알아야 한다. 그리고
속도값과 위치값이 피드백되는데 피드백 분기선을 작성하는 방법은 선상에 마우스를
올려 놓고 마우스의 오른쪽 부분을 누른 채 아래로 드래그 하면 분기선이 형성된다. 그
런 다음 마우스의 왼쪽을 누른 채 선을 연결하면 된다. 게인블록의 방향을 바꾸기 위해
서는 게인블록을 클릭한 후 Format>Rotate Block을 선택할 때 마다 방향이 90도 바뀌게
된다．
  2번 반복하면 180도 바뀌게 된다. 아래 회로의 스텝응답은［그림 1.11］
                                           과 같은 결
과를 나타낼 것이다．




                                            1
                                                      p
                                            S
   Step                 Integrator      Integratorl    Scope




                 ［그림 1.12] 기본블록을 사용한 모델회로




 8) Simulink를 이용한 일반 비선형식의 모델링 방법


 Simulink는 비선형시스템의 모델링을 쉽게 할 수 있도록 다양한 블록을 제공하고 있
다. Simulink>Discontinuities 내부에 많은 비선형 블록이 들어있다. 대표적인 것으로는
dead-zone이나 saturation 등이 있다. 아래 그림과 같이 물체의 양쪽에 추진시스템을 갖
는 이동시스템을 고려해 보자．




                                            1 장 Simulink의 기초－ 21


===== PAGE 23 =====
                          ㅁ림 1.13] 추진시스템


 위 그림의 이동시스템은 물체의 좌우에 추진체가 달려 있는 구조이다. 추진체의 힘
을 조절하여 물체가 정해진 위치
                （원점）
                   에 정지하도록 하는 것이 목적이다. 위 시스템
의 운동식은 다음과 같이 정의될 수 있다．


                                m父 = F                   (1.13)


 혹은


                               x= F/m                    (1.14)


 m=5 Kg 이라고 한다면 다음과 같이 Simulink 모델을 구성할 수 있다．



                                 I          》
                                                1 >
                                 S              S
                  1/rn        Velocity    Displacement
                         ［그림 1,14] Simulink 모델


 만약, 시스템의 속도와 변위의 합이 음수일 경우 F=1로 제어하고, 시스템의 속도와
변위의 합이 양수일 경우 F=-1로 제어하는 제어기
                           （일종의 뱅뱅제어기）
                                     를 사용한다고
한다면 제어모델은 다음과 같이 구성할 수 있다. Simulink>Math Operations 안에 있는
Sign 블록을 추가로 들어가 있다．




           （Matlab/Simulink를 중심으로）
22- 퍼지신경망 제어


===== PAGE 24 =====
       +      Sign       4Im
                                       1
                                       S
                                    Velocity


                 ［그림 1.1司 간단한 bang-bang 제어모델


 위 모델의 시물레이션 결과를 그래프로 확인하기 위하여 x-Y 그래프를 부착하여 속
                                                      I
                                                      S
                                                Displacement




도와 변위와의 관계를 알아보았다. 그리고 시물레이션이 진행할 때 경과하는 시간을
표시하기 위해 Clock과 Display 블록도 설치하였다．




                        Display                  XV Graph
            ［그림 1.16] X-Y Graph를 설치한 bang-bang 제어모델


 위 회로의 문제점은 시스템이 언제 원점에 도달할 지 어느 수준에서 프로그램을 정
지해야할지 기준이 없다. 따라서, 다음과 같이 정지기준을 설정하기로 한다．


                          IxI+I I 二 0.01                        (1.15)


 그러면 위 회로는 아래와 같이 약간 수정할 수 있다．Simulink>Math Operations 안에
있는 Abs 블록이 추가로 들어가 있는 것을 볼 수 있다．




                                                  1 장 Simulink의 기초－23


===== PAGE 25 =====
                       Sign           1/rn
                                                   *
                                                          s
                                                    Velocity
                                                                   H 귈_
                                                                  Displacement




                       0
                       Clock
                                                   4.95
                                                                 L坪크       XY Graph
                                              Display
               -
                     叫 M卜
                                                ㅣ
                        Abs                      <= 0.01
                      Velocity
                          - 1                   Compare Stop Simulation
                   卜 M                         To Constant
                             -
                        Abs
                   Displacement

              口림 1.17] 정지조건을 포함한 bang-bang 제어모델




 아래［그림 1.18］은 시물레이션 중의 속도와 위치의 변화를 표시한 그래프이다．



                                             X Y Plot




                                                                                      <



               4l5




                               ｛〕．5             0……           g汪l5 ※
                                                 지s

              ［그림 1.18] 시물레이션 중의 속도와 위치의 변화



0甘 제 1,1 아래 그림과 같이 일반적인 도로에서 주행하는 자동차를 고려해 보자. 이 때 자동

                                       （Fe), 주행 중에 공
차에 작용하는 힘은 엔진 혹은 브레이크에 의해 전달되는 차 내부의 생성힘
               （Fa), 그리고 오르막이나 내리막에 의해 생성되는 지형적 힘
기가 차체에 미치는 공기저항힘
(Fh）
   의 3가지로 크게 구분이 가능하다．


          （Matlab/Sim미ink를 중심으로）
24－퍼지신경망 제어


===== PAGE 26 =====
                               ［그림 1.18] 언덕길에서 주행 중인 자동차의 역학 모델


   위의 자동차 모델에 뉴톤의 2법칙을 적용하면 다음과 같은 식을 얻을 수 있다．


                                                          m父= Fe-Fa- Fh                                                                  (1.16)


   위 식에서 생성힘
           （Fe）
              는 - 2500 二 Fe 二 1500의 범위를 가지고 있다고 가정한다．
                                                    이
조건에서 음의 값은 브레이크를 작동하는 경우에 해당되고, 양의 값은 엔진의 출력을
올리는 것을 의미한다．
           공기저항힘
               （Pa）
                  과 지형적 힘αh）
                           은 다음의 식과 같이 시간에 따
라 sine적으로 변한다고 가정한다．


                                         Fa = 0.001x + 20 sin (0.01t2 ))2                                                                (1.17)


                                                   Fh =30sin(0.0001x)                                                                    (1.18)


   위의 3가지 힘을 고려한 비선형시스템을 Sirnulink로 구현하면 다음그림과 같다．


                               "5o0L一∼                   ' [

                                         -
                                                               一∼갸
                                                    -2
                         M크x Trm』
                                st                Max Brake




                                                                                           i
                                                                                           女쏘＼주
                                                                                              ―
                                                                     －川
    !r느… r'>－奸 .)켜."；芬；贓
      1                mm" Ll…커max
Re把I_
Reference Input   닙am     ▲’        L-   e   Upper hmit                   Lower smil   .


                                                                                                          砂‘〕＞－∼」    口＋Distance
                                                                                                                           二 4,
                                                                                                           卄mass Speed

                                                                                                  Aerodynamic Force
                                                                                                                                        Clock
                                                                                                  …！二U)
                        Display
                                                                                                                      Hill Force
                           0輛§盛 斗            ∼》
                                                                                                                                   4小
                                                         Sc*겨；冶

                                   ［그림 1.1이 주행중인 자동차의 Simulink 모델



                                                                                                                 1장 Simulink의 기초－25


===== PAGE 27 =====
 위 그림에서 Aerodynamic force와 Hill force는 Simulink의 Fcn 블록을 이용하여 구현하
였다. Aerodynamic force는 0.001*(u[1]+20*sin(0.01*u[기))A2로 입력되어 있다．
                                                               여기서 u[1]
은 첫번째 입력 즉, 자동차의 속도                  는 2번째 입력으로서 αock
                  （Speed) 값을 나타내고 u[2］
에 물려 있는 바와 같이 시간을 나타낸다. 위 수식을 식    과 같이 비교를 하면 쉽게
                              （1.17）
알 수 있을 것이다. 마찬가지로 Hill force 블록에는 30*sm(0.000l*u[1]）의 값이 입력되어
있다. 이 경우 입력은 당연히 하나밖에 없다. 기준입력 추종성능에 대한 시물레이션 결
과는［그림 1.20］
          에 나타나 있다.




                     ！그림 120] 주행중인 자동차의 스텝응답




4. 서브시스템
       （Subsystem）
                 의 생성


 원래 만들어진 Simulink 모델을 좀 더 단순한 서브시스템으로 변형할 수 있다. 모델
의 사이즈가 커지고 복잡해지면 전체모델을 한 눈에 이해하기가 어렵다. 따라서, 모델
의 일정한 영역을 서브시스템으로 변형하면 전체모델이 기능별로 단순화되고 시스템
의 흐름을 한 눈에 이해하기 쉽다．




          （Matlab/Simulink를 중심으로）
26－퍼지신경망 제어


===== PAGE 28 =====
                                             Gaini




                            >    ;    …           >   ;      -－닐rㅋ
    Step   「Gain     추      Integrator         Integratorl     Scope

                             Gain2

                            ／了4」
                              ，느N
                    ㅁ림 1.2112차 시스템의 Simulink 모델


 위 모델의 서브시스템을 만들기 위해 입력부 Step과 출력부 Scope를 제외한 전체부
분을 마우스를 드래그하여 선택한다. 그런 다음 Simulirik 편집창의 Edit>Subsytem 을 선
택한다. 그러면 다음과 같이 서브시스템이 생성되어 진다．




                                m1l   Outl   ［二
                   Step                      Scope
                                Subsystem
              ［그림 1.22] 서브시스템을 사용한 2차 시스템의 모델


 서브시스템의 원래 회로를 보거나 수정을 원할 때에는 서브시스템을 더블클릭하여
내부를 볼 수 있다．



예 제 1.2 아래 그림과 같이 구성되어 있는 2자유도 카트시스템을 고려하여 서브시스템으로

단순화된 모델을 생성해 보기로 하자．




                      ［그림 1.23] 질량－스프링 카트 모델


                                                      1 장 Simulink의 기초－27


===== PAGE 29 =====
 위 시스템에서 각각의 카트 운동은 다음과 같은 운동식으로 설명되어진다．


                                                    1       IT, I
                                      ==                       n`Xn_ 1                                -   Xn)              rn+ 1`xn             -




                                                                                                                                                                                            (1.19)
                           xn                                                                                   -1-
                                                -
                                                                                                                                                                  X
                                                                                                                                                                                i) )J
                                                                                                                                                                      (n+
                                                            ti\
                                                        n




 식
 （1.19) 형태로 운동식을 나타내면 다음과 같다．


                                           父，           =
                                                                                                              x1)+K2
                                                                       m
                                                                                                          -
                                                                                            (x。
                                                                                                                                (x1-
                                                                  -1
                                                                                (K1
                                                                                                                                                    X2)
                                                                                                                                                                            )
                                                                                                              x2)+K3
                                           父：                          1
                                                        =
                                           X2 =                                                                                             -



                                                                       m
                                                                                                                                (x2-
                                                                                            (x1-
                                                                  -
                                                                                (K2
                                                                                                                                                    X3)
                                                                                                                                                                            )
 위 식에서 xl은카트1의 변위, X2는 카트.2의 변위이다. xO와X3는 의미없는 값으로0이다．
 아래［그림 1.24〕
           는 카트1 부분에 대한 시스템 모델을 Simulink 로 나타낸 것이다．



    Left        -+
                         Add                        Spnngl
                                                                           －卜
                                                                                      .4.
                                                                                                                                                                                        8
                -    -                                                                Force                           盤〉
                                                                                                                           1/mass
                                                                                                                                       →．
                                                                                                                                                veiociiy
                                                                                                                                                          ．   귑       ．


                                                                                                                                                                                 Position
    (    2   )_     卜+
        Right        Addi                       Spnng2


                                                    ［그림 1.24] 카트1에 대한 시스템 모델


〔그림 1.24] 모델을 서브시스템으로 나타내면 아래 그림과 같다．


                                                                                                      -


                                (i                  )_                                        `Left
                                     Left                                                                     Disp                              卜
                                                                                                                                                （ 1 )
                          〔2 二                                                               >Right                                                                   Disp
                                     Right
                                                                                                          Cartl
                                           ㅁ림 1.25] 서브시스템을 사용한 카트j 모델




          （Matlab/Simulink를 중심으로）
28－퍼지신경망 제어


===== PAGE 30 =====
    Left

                                                                            －→（    1 )
                                     Force2                          Position     Disp
                                                1/mass   Velocity

   Right   Addi         Spnng3


                          ［그림 1.2이 카트2에 대한 시스템 모델


 같은 방법으로 카트2에 대한 Simulink 모델과 대응하는 서브시스템을 생성할 수 있
다.［그림 1.26］
          은 카트2에 대한 Simulink 시스템 모델이고,〔그림 1.27］
                                              은 서브시스템을
사용한 전체 시스템 모델이다．



                    0            *Left
                                         Di8p
                  Left
                                 > Right

                                    Carti




                    0
                                                             Scope
                  Right              Cart2
                  ㅁ림 1.2기 서브시스템을 사용한 전체 시스템 모델




                  母白 ／→「β 月 曲 I召 r昌 1日 a 埠




                            ［그림 12미 카트2의 운동궤적



                                                                    1 장 Simulirik의 기초－29


===== PAGE 31 =====
5. Embedded MATLAB Function 사용


 이 기능은 유저가 작성한 함수를Simulink 모델에 포함할수 있도록 한다. Embedded
MATLAB Function 블록을Simulink 모델에 포함시키기 위해서 다음과 같은 작업이 필요
하다．


 d) 아래 그림과 같이 Simulink 모델창을 생성하고 Simulink으I User-Defined Function 라
이브러리에서 Embedded MATLAB Function 블록을 드래그하여 Simulink 모델창에 넣는다．




               File Edit View 51m며a娥at Format Tools Help

               D ;侈日 巒           汕勛 串 尸 斗 寸 요 청‘쑈




                                   Embedded
                                 MATLAB Function




                                                           芟



 (2) 원하는 Source와 Si欲 블록을 모델 창에 넣는다．
 예를 들어 Sources 라이브러리에서 Constant 블록을 드래그하여 Embedded MATLAB
                                             로 설정한다．
Function 블록 왼쪽에 놓는다. Constant 블록의 값은 벡터값[2345］
 Sinks 라이브러리 에서 2개의 Display 블록을 역시 Embedded MATLAB Function 블록
의 오른편에 배치한다．
 그런 후에, 모델창은 다음과 같은 모습을 보이게 된다．




            （Matlab/Simulmnk를 중심으로）
30 - 퍼지신경망 제어


===== PAGE 32 =====
             File Ect View sbmjlation Format Tools Help

             0 - 嚼 1a 母ㅣ品 目彗 爵 - 4그 롸 11-. - 三朶 之 - 》




                                                          Display


                  Constant
                                  Embedded
                                MATㄴ D F
                                      「 」n口tie n




여기까지 작성된 모델이름을 call stats block1해서 저장한다．


(3) Embedded MATLAB Function의 프로그램하기
다음 예는 주어진 입력 벡터에 대해 평균값과 표준편차를 구하는 과정을 보여줄 것
이다．
①Embedded MATLAB Function 블록을 더블클릭하면 다음과 같은 편집화면이 나타
  난다．




            台 力 心 《騙 쑵 圈 j         @ * 陸 圈 -卜 ' ｛〕￡ 喝 娘 鄒 堪 割ㅂ크




                                     cd l




                                                                    1 장 Simulink의 기초－31


===== PAGE 33 =====
 위 화면은 디폴트로 주어지는 함수이다. 이제 위 화면을 예제의 목적에 맞게 수정해
야 한다. 순서대로 설명하면 다음과 같다．
 ② 첫 번째 문장을 다음과 같이 수정한다．


                    Function [mean,stdev] = stats(vals)



 위 문장에서 stats 는 Embedded MATLAB function의 이름이다. 결국 이함수는 벡터값
vals를 입력 받아 출력값 mean, stdev을 계산해 주는 함수이다．
 ③ 함수내의 식을 수정한 후에 Simulink 모델창은 아래 그림과 같이 된다. 그림에서
   보는 바와 같이 Embeded 함수 블록에 함수명과 입출력 변수명들이 적혀져 있다．


                           Input Port            Output Por눕




 ④ 화살표를 연결하여 모델 회로를 완성한다．



                                                         --




                                                mean
        [2 3 4 5]   p.
                         vals           stats                       Dis이ay
                                                stdev
        Constant
                              Embedded                         1
                            MATLAB Function
                                                                   Dis이ayl




           （Matlab/Simulink를 중심으로）
32- 퍼지신경망 제어


===== PAGE 34 =====
 ⑤ Embeded MATLAB Function 블록을 열고 다음과 같이 프로그램을 완성한다．
 function [mean, stdev] = stats(vals)
 % calculates a statistical mean and a standard
 % deviation for the values in vals.


 len = length(vals);
 mean = avg(vals, len);
 stdev = sqrt(sum(((vals-avg(vals, len))/'2))/len);


 function mean = avg(array, size)
 mean = sum(array)/size;
 ⑥Simulink 모델창에서 시물레이션을 시작하면 다음과 같은 결과를 얻게 된다．



                                                      L         3.5
                                        mean
           (2 3 4 5)          》vals stats
                                        stdev             Display
            Constant                                          1.118
                               Embedded
                             MATLAB Function
                                                          Displayl


                             Display1의 값은 표준편차임을 알 수 있다．
 Display창에 있는 값3.5는 입력값의 평균이고，




6. S-Function의 사용


 S-Function은 이미 작성되어 있는 코드를 Simulink 블록에 포함될 수 있도록 하는 기
능이다. S-Function은 Matlab의 M파일을 사용하여 작성할 수 있고, Matlab의 MEX파일
구조를 통하면 C 프로그램 코드로도 작성할 수 있다．
 예를 들어, Matlab의 M파일로 동적모델식을 이미 작성해 놓았다면 이 식을 S-Function에
포함시킬 수 있고, 제어시스템을 모델링하기 위해 일반 Simulink 블록을 사용하는 것이
가능해 진다. 어떤 경우에는 동적식의 일부분을 논리적인 수식으로 표현하는 것이 편



                                                          1 장 Simulink의 기초－33


===== PAGE 35 =====
할 수 있는데, 이럴 때 S-Function을 사용하는 것이 유리하다. 또한 이미 작성된 Simulink
모델에 에니메이션 기능을 붙일 때도 S-Function 기능을 사용하면 편리하다．


 1) S-Function 블록




              Sine Wave         S-Function             Scope
                  ［그림 1.29] S-Function을 이용한 Simulink 블록


 S-Function 블록은 Simulink>User-Defmed Functions 라이브러리 안에 들어 있.다.［그림
1.29］
    는 S-Function을 이용하여 Simulink 블록을 작성한 예이다．
 M파일을 이용하여 S-Function을 작성하는 방법을 알아보자. M－파일 안에 있는 S-Function
은 다음과 같은 형태를 취한다．


          function[sys, xO, sir, ts]=sfunc name(t, x, u, flag, pl, p2, " " ' pn)


 위 명령문에서 sfunc name은 S-Function의 이름을 의미한다. 예를 들어 S-Function이
sfuncl.m 파일 안에 저장되어 있다면 sfunc name을 sfuncl으로 대치해야 한다는 것이다．
먼저, S-Function에 대한 입력변수들은 다음과 같다．


   t : 시물레이션 과정에서 현재시간
   x: S-Function 상태벡터의 현재값
   U : 입력벡터의 현재값
   flag : 이 값에 의해 해당되는 S-Function이 호출됨
   pl,p2, "pn: 필요에 따라선택하는파라메터


 S-Function을 호출하는 플래그의 정의는 다음과 같다．


   0 : sizes 구조체를 초기화 한다. 그리고, sizes 이 값을 sys에 할당한다．
                                                   xO와 ts 그리
     고 str=[〕을 설정한다．


          （Matlab/Simulink를 중심으로）
34－퍼지신경망 제어


===== PAGE 36 =====
    1 : 연속적인 상태값
               （state）
                     에 대한 미분값을 계산한다．
    2 : 이산 상태값 (discrete state）
                              을 업데이트 한다．
    3 : 출력값을 계산한다．
    4 : 다음 샘플링 값을 계산한다．
    9 : 필요한 경우 시물레이션 종료 작업을 수행한다．


 끝으로, S-Function의 출력변수의 정의는 다음과 같다．


    sys : 다목적 출력변수
    xO: S-Function 상태벡터의 초기값
    str: Simulink Version 확장을 위해 확보된 변수. 비워두면 됨
    ts : 샘플링 시간값


 위에서 정의한 각각의 플래그 값에 대한 S-Function의 반응을 자세히 알아보도록 하자．


 (1) 초기화 과정
          （flag=O)
 초기화 단계는4가지 작업으로 구성된다. 먼저 sizes 구조체를 설정한 다음 이 구조를
sys 에 할당한다. sizes 구조체는 다음과 같이생성한다．


                               sizes = smisizes;


 그런 다음 sizes의 멤버값을 할당한다. 멤버값을 할당하는 방법은 아래 표와 같다．


                             ［표 1-11 Sizes의 구조
             멤버                                    정의
 Sizes.NumContStates      연속상태
                             （continuous state）
                                              변수의 수
 Sizes.NumDiscStates      이산상태
                             （discrete state）
                                            변수의 수
 Sizes.NumOutputs         출력변수의 수
 Sizes.Numinputs          입력변수의 수
 Sizes.DirFeedthrough     블록의 출력값이 입력값의 함수인 경우＝1 설정, 그 외 경우＝0
 Sizes.NumSamplingTimes   샘플링 수（갸 이상 선택）
                                       . 순수한 연속함수에는 1 값 사용함




                                                        1 장 Simulink의 기초－35


===== PAGE 37 =====
 Sizes 구조체가 정의된 다음 구조체를 출력인 sys에 다음과 같이 할당한다．


                        sys = simsizes(sizes)


 두 번째 단계에서 상태변수에 대한 초기조건을 설정한다. 예를 들어 초기조건이 2개
의 연속상태 값 1과2개의 이산상태값0로 설정하는 경우 다음과 같다．


                      XO = [1.0 1.0 0.0 0.0];
 세 번째 단계에서는 str 을 설정한다．


                             Str=[];


 마지막 단계에서는 샘플링 시간을 설정한다. Is를 사용하며 첫 번째 인자는 샘플링
시간이며 두 번째 인자는 옵셋값을 나타낸다. 예를 들어 연속적인 S-function인 경우에
는 다음과 같이 설정한다．


                            Ts=[O, 0];


 이 번에는 S-function이 이산함수일 때의 예를들어보자. 2개의 이산 샘플링 시간을 갖
는 경우를 고려해 보자. 먼저 주기가 0.5초이고, 옵셋이 0인 경우를 가정하면 샘플링시
간이 0, 0.5, 1.0,…의 순서로 설정이 될 것이다. 한편 주기가 0.25이고 옵셋이 0.1인 경우
에는 샘플링 시간이 0.1, 0.35, 0.6의 순서로 설정이 된다. 이 경우에 설정은 다음과같다．


                      Ts = [0.5, 0; 0.25, 0.1];


 만약, 샘플링 시간을 이전 블록에서 사용하는 샘플링 시간을 사용하고 싶다면 샘플
링 시간 값을 -1로 설정하면 된다. 일반적으로 S-function블록은 이전의 블록과 연결되
어 있으므로 -1로 설정하는 것이 보편적이다. 샘플링시간을 변수로 설정하고 싶다면
이 경우 -2의 값으로 설정해야 한다. 이 경우 flag=4를 이용해서 다음 단계의 샘플링 시
간을 계산하는 S-function을 사용해야潼｝
                         다．


          （Matlab/Simulink를 중심으로）
36－퍼지신경망 제어


===== PAGE 38 =====
(2)연속 상태값의 미분 (flag=1)
 플래그 값이 1이면 상태벡터의 미분식이 sys어］할당되게 된다. 다음과 같은비선형식
의 경우，


                              xl = x2


                         ㅊ2 =x1- 3x蔘 + u1
 sys는 다음과 같이 표현된다．


                             sys(1)=x(2);


                     sys(2)=x(1)_3*x(2)f2+u(1);


 (3) 이산 상태값의 업데이터 (flag=2)
 플래그 값이 2이면 상태벡터의 이산값을 sys어］할당되게 된다. 다음과 같은 이산식
의 경우，


                     x1(k+1) =x1(k)+u1(k)


 sys는 다음과 같이 표현된다．


                           sys=x(1)+u(1);


（예）2개의 샘플링 시간을 갖는 2차 이산시스템을 고려해 보자．
                                  첫 번째 이산성분은
매 0.3초마다 업데이트 되며 두 번째 이산성분은 매 0.5초마다 업데이트 된다. 두 경우
모두 offset시간은 0이다．
 첫 번째 시스템과 두 번째시스템은 각각 다음과 같다．


                    x1(k+1) =x1(k)+0.5x2(k)




                                                  1장 Simulink의 기초－37


===== PAGE 39 =====
                                  x2(k+ 1)=x2(k)+u1(k)


  이 경우 sys를 구하는 코드를 작성하면 다음과 같다．


penodi = 0.3;
offset! = 0.0;
period_2 = 0.5;
offset_2 = 0.0;

sys = x;
if abs(round(t-offset_1)/period_1-((t-offset_1)/period_1))<1.Oe-8

 sys(1) = sys(1)+0.5*x(2);
end
if abs(round(t-offset_2)/period_2-((t-offset_2)/period_2))<1.oe-8

 sys(2) = sys(2)+0.5*u(1);
end


  위에서 주의할 점은 if-else를 사용해서는 정확한 샘플링을 기대할 수 없다. 왜냐하면，
두 샘플링타임이 동시에 도달하면 S-function은 잘못된 결과를 만들어 내기 때문이다．


  (4) 블록 출력값 (flag=3)
  플래그 값이 3이면 S-function의 출력값을 sys에 할당하게 한다. 예를 들어 시스템의
출력식이 다음과 같다면


                                         !/ = x1+ x2


   sys 에 할당되는 값은 다음과 같이 표현된다．


                                         sys=x(1)+x(2);




38－퍼지신경망 제어
          （Matlab/Simulink를 중심으로）


===== PAGE 40 =====
    2) M 파일을 이용한 S-function의 작성 예



    아래의 예는 상태변수
              （state variable）
                             가 없는 단순한 형태의 산술식인 y = 2u에 대한
S-function을 구성하는 예이다. Matlab의 M파일을 이용하여 작성하였다. M파일의 이름
은timestwo.m 이다．




function [sys, x0, str, ts] = timestwo(t, x, u, flag)
% 위 S-function은 입력값을 2배 증가시켜주는 함수이다
                                  （y= 2*u).


%
% Dispatch the flag. The switch function controls the calls to
% S-function routines at each simulation stage of the S-function.

%
switch flag,
 %%%%%%%%%%%%%%%%%%
 %                 초기화                    %
 %%%%%%%%%%%%%%%%%%
 % 상태, 샘플링시간 등을 초기화 한다．


 case 0

    [sys, x0, str, ts] = mdllnitializeSizes;


 %%%%%%%%%%%
 %         Outputs        %
 %%%%%%%%%%o/c

 % S-function block의 출력값을 리턴한다．
 case 3
    sys = mdlOutputs(t, x, u);
 %%%%%%%%%%%%%%%%%%%%



                                                                    1 장 Simulink의 기초 39


===== PAGE 41 =====
 %              사용되지 않은flags                   %
 %%%%%%%%%%%%%%%%%%%%
 % 종료작업
      （flag=9）
             이 사용되지 않음, 또한 연속, 이산 상태변수 없음．
 ％따라서，
     flag 1, 2, 4는 사용안됨．
 % 비어있는 U를 리턴함．
      case { 1, 2, 4, 9 }
      sys=[];


 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 %                          Unexpected flags (error handling)                 %
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 % 다루지 않는 flag 값의 경우에는 error message를 냄．
 otherwise
    error(['Unhandled flag = ',num2str(flag)]);
end


% end timestwo
%


% md11niti 1izeSizes
% ketum the sizes, initial conditions, and sample times for the S-function.
%
%
function [sys, x0, str, ts] = mdllnitializeSizesO


sizes := simsizes;
sizes.NumContStates =0;
sizes.NumDiscStates = 0;
sizes.NumOutputs        = -1; % dynamically sized




            （Matlab/Simulink를 중심으로）
40 - 퍼지신경망 제어


===== PAGE 42 =====
sizes.Numlnputs     = -1; % dynamically sized
sizes.DirFeedthrough = 1; % has direct feedthrough
sizes.NumSampleTimes = 1;
sys = sinisizes(sizes);
str=[];
xO =[];
ts = [-1 0]; % inherited sample time


% end mdllnitializeSizes


%
%
% mdlOutputs
% S-function의 출력벡터 값을 리턴 함
%
%
fu끄ction sys = mdlOutputs(t, x, u)


sys = u * 2;


% end m出Outputs


    위와 같이코딩을 한 후 다음과 같이 S-function 블록을 포함한 Simu1ink 회로를 작성한
다. 물론 S-function의 블록이름은 timestwo로 설정해야 한다．



                                          timestwo

                          Sine Wave      S-Function




                                                      1 장 Simulink의 기초－41


===== PAGE 43 =====
 아래 그림은 시물레이션을 수행한 후의 결과이다．




                 昌曲 J＞多 刃 朴 I召 I增 l . 毋 奪




42－퍼지신경망 제어
          （Matlab/Simulink를 중심으로）


===== PAGE 44 =====
2장퍼지시섀
]. 퍼직 집합
       （Fuzzy seD

         퍼지
          （fuzzy）
                라는 용어는 사전적 의미에서 뜻하는 바와 같이 모호하다 혹은 애매하다
는 것을 의미한다．
         이러한 개념이 집합
                  （set）
                      에 적용된 것이 퍼지집합인 것이다. 퍼지집
합을 이해하기 위해서는 기존의 집합과 비교해 보는 것이 도움이 될 것이다．




               (a) 일반집합                      (b) 퍼지집합
                          ［그림 기. 일반집합과 퍼지집합의 비교


         위［그림 2.1](a）
                    에서 어떤점이 흑색으로 된 집합
                                    （영역）안에 있으면, 즉 어떤 점이 영
역에 포함되면 이 점은 집합에 대한 소속값
                      （membership value）
                                       이 1이 된다. 반면에 어떤


                                                    2 장 퍼지 시스템 43


===== PAGE 45 =====
점이 집합 밖에 놓여 있으면 이 점의 소속값은 0이 될 것이다. 이와 같이 어떤 집합의
영역에 포함되기만 하면 1의 값을 갖고 포함되지 않으면 0의 값을 가지게 된다. 이러한
개념은 인접한 두 점에 대해 확연히 다른 결과를 초래 할 수도 있다. 예를 들어 집합의
경계층 조금 밖에 존재하면 0의 값을 갖게 되고, 반면에 인접한 점이라도 경계충의 조
금 안에 있으면 1의 값을 갖는 이분법적인 결과가 발생하게 된다. 퍼지집합을 사용하
게 되면 이러한 모순을 방지할 수 있다．


 1) 퍼지변수, 퍼지집합, 퍼지함수의 관계


 퍼치변수는 물리적인 속성으로 생각하면 될 것이다. 제어적인 측면에서 본다면 제
어대상이 되는물리적인 량으로 볼 수 있다. 예를 들면 온도, 압력, 속도 등이 퍼지 변수
라고 볼 수 있다. 그러면 퍼지집합은 무엇인가？ 퍼지집합은 퍼지변수를 분류할 수 있
는 개념이다．
      예를 들어 기온을 퍼지변수라고 둔다면, 기온에 대한 퍼지집합은 " 춥다",
" 적당하다" , 그리고 " 덥다" 와 같이 퍼지변수를 구분할 수 있는 속성이라고 할 수 있다．
다음과 같은 기온의 샘플값을 고려해 보자．


 기온샘플값＝{-10, -5, 0, 5, 10, 15, 20, 25, 30, 35, 40}
 이제 기온샘플 값이 각각의 퍼지집합 내에서 0과1사이의 소속값을 가지게 된다는
것을 알아보자．


 -10도 정도의 날씨가 몇 % 정도 추운지 독자에게 물어보면 100% 춥다고 할 것이다．
그러므로, -10도는 '춥다' 라는 퍼지집합에서 소속값이 최대인 1이 된다. 반면에 0도가
얼마나 추운지 물어보면 최고기준으로 80% 정도이다라고 한다면 소속값은 0.8이 될
것이다. 이렇게 해서 3개의 퍼지집합에 대해 소속값을 나름대로 작성할 수 있다. 다음
표는 한 작성예를 나타내고 있다．




          （Matlab/Simulink를 중심으로）
44－퍼지신경망 제어


===== PAGE 46 =====
                           표 2.1] 각 기온의 퍼지집합내 소속값

           기온값                   췹ㅘ            적당하다              덥다
               -10               1.0                0             0
               -5                1.   0             0             0
                0                0,8                0             0
                5                0.6            0.3               0
               10                0.4            0.6               0
               15                0.2            0.9              02
               20                     0         1.0              04
               25                     0         0.9              0.6
               30                     0         0.6              08
               35                     0         0.3              10
               40                     0             0            10



 각 퍼지집합에 대한 소속값을 아래와 같이 함수로 표시한 것을 퍼지함수라고 부른
다. 간단한 예를 들어보도록 한다. 기온 15도를 생각해 보자. 기온 15도는 춥다라는 퍼
지집합에서 소속값은 0.2, 적당하다라는 퍼지집합에서 소속값은 0.9, 그리고 덥다라는
퍼지집합에서는 소속값은0.2이다. 이와같이 어떤 값이 여러 퍼지집합에 각기 다른 소
속값을 가진다는 것을 알 수 있다．


          -----            占－ㄱ－-m- ------               ---.---------


                             -

        스＜: cII
          I- --－룬山*岺mA- 1 '－斗－.
         -20         -10     0            10   20
                                                          , ＋노－-}
                                                          30    40      50

                     ［그림 2.2] 소속값을 이용한 퍼지함수 그래프




                                                                       2 장 퍼지 시스템 45


===== PAGE 47 =====
2. 펴직 시스템


 퍼지 제어시스템을 블록선도로 나타내면［그림 2.3〕
                            과 같이 설명할 수 있다. 기준 입
력값과 실제 출력값의 차이값, 즉 오차값이 퍼지제어기에 입력이 되면 퍼지제어기는
내부 연산에 의해 적절한 출력값을 만들어 내며 이 값이 동적시스템의 입력값 u(t）
                                             가
된다. 일반적으로 퍼지제어기 자신은 다음과 같이 3개의 요소로 구성될 수 있다．




                                     Contro;
                                     螂uts
                                      町符




                  ［그림 2.3] 퍼지 제어시스템의 기본구조



 1) Rule-B《그se 문장 생성 및 의사결정


［그림 2.3］
       에서 보는 바와 같이 기준입력과 제어프로세스의 실제 출력값의 차이로부
터 위치오차나 속도오차가 계산되며, 이 오차값은 대부분의 다른 제어기처럼 퍼지제
어기 제어시스템의 입력인자이다. 만족할 만한 퍼지제어기를 구성하기 위해서는 일정
한 수준 이상의 지식을 갖춘 인간의 지식을 필요로 한다. 퍼지제어기에 입력되는 위치
및 속도오차값의 크기에 따라 If-Then과 같은 문장 형식을 이용하여 크기의 구간을 설정
하는 것이 필요하며 이것을 그림에서 rule-base부로 표시되어 있다. 또한 각각의 rule-base
에 대해 어떠한 출력값을 내 보내야 하는가에 대한 의사결정도 이루어져야 한다. 이것
은 그림에서 추론부｛inference mechanism）
                              로 표시되어 있다．




46－퍼지신경망 제어洶atIab/SimuIink를 중심으로）


===== PAGE 48 =====
 2) 퍼지화
      （fuzzification)


 퍼지화라는 것은 위 1）
             항에서 생성된 rule-base 및 의사결정이 다분이 애매한
                                             （수학적
인 모델이 아닌 문장으로 구성되어 있다는 것을 의미한다. 예를 들어 아래와 같은 명령
                                          （fuzzy한）개념이라고
문에서 Fast, Big, 그리고 Large 등은 계량화되어 있지 않은 애매한
할 수 있다．


 "If자동차의 속도가Fast하고 도로의 커브도 Big하면，
                                Then 브레이크의 량을 Large 하
게 하라"


 결국 퍼지제어기는 위와 같이 수치적이 아닌 애매한 표현의 명령문들이 모여서 각
경우에 대한 제어결정을 일차적으로 하게 된다. 이와 같은 개념을 퍼지화라고 한다．


 3) 비퍼지화
       （defuzzificati on)


 퍼지제어기의 내부에서 이루어지는 rule-base 및 추론부분에서는 퍼지적인 표현의
명령문을 사용하지만，
          실제 퍼지제어기의 출력은 산술적인 값이 필요하다．
                                    Large와 같
은 애매한 개념을 프로세서에 줄 수는 없을 것이다. 대신에 " 브레이크 페달의 각도는
30도" 와 같은 수치적인 값을 주어야 할 것이다. 이러한 수치적인 값을 만들어 내는 것
을 비퍼지화라고 한다．


 이해를 돕기 위하여 도립진자를 제어하는 경우를 고려하여 사람이 손으로 제어하는
경우와 퍼지제어기가 제어하는 경우를 비교해 보자.［그림 2.4］
                                  는 사람이 손바닥 위에
도립진자
   （혹은 간단한 막대기）
              를 올려놓고 똑바로 선 자세를 유지하기 위해 제어하는
경우를 나타낸 것이다. 사람은 경험에 의해 도립진자를 수직으로 유지하기 위해서 손
을 앞뒤로 밀고당기는 노력을 계속할 것이다. 실제로 사람은 퍼지적인 제어를 수행하
고 있는 것이다.［그림 2.3］
                은 퍼지제어기로서 도립진자를 제어하는 경우이다. 퍼지제
어기가 올바로 작동하게 하기 위해서는 제대로 된 규칙을 작성해야하며 이것은 제어
를 담당하는 사람의 몫이다. 결국, 퍼지제어기는 사람이나 동물의 경험에 의해 결정되



                                          2 장 퍼지 시스템 - 47


===== PAGE 49 =====
어지는 판단
     （decision）
              에 의한 제어를 수힉적으로 흉내 내는 것이라고 볼 수 있다．



                 r




                      ［그림 2.4] 사람에 의한 역진자의 자세제어




         r   +
                                          \            I-/               \
                                                  I,                         l/
                               Fuzzy          -
                                                              Inverted
                              ControHer                      pend너urn




                     ［그림 2.司 퍼지제어기에 의한 역진자의 자세제어




3, 퍽지 시스템의 구성방법




                         ［그림 2.6] 카트－도립진자 시스템



 퍼지제어기를 구성하는 방법을 3개의 단계로 나누어서 설명하는 것이 이해하기 쉽
다．
 이를 위해서 일반적으로 많이 사용하고 있는 카트－도립진자 모델을［그림 2.6］
                                           과같



          （Matlab/Simulink를 중심으로）
48－퍼지신경망 제어


===== PAGE 50 =====
 이 나타내었다. 이 시스템에서는 도립진자를 수직위치로 유지하는 것이 제어의 목표
 이다．
   그림에서 미는 힘 U는 오른쪽 방향이 양의 방향이고, 회전각y는 시계방향이 양
 의 방향으로 고려되었다．


 단계1 퍼지제어기의 입력변수와 출력변수의 선정


  먼저, 퍼지제어기의 입력변수와출력변수를 결정해야한다. 일반적인 선형제어기와
 비선형제어기를 구성할 때와 마찬가지로 도립전자시스템의 입력은 오차값과 오차값
 의 변화율을 선정하는 것이 바람직하다. 퍼지제어기의 출력은 당연히 힘이 되어야 한
다. 입력변수와 출력변수를 정리하면 다음과 같다．


  입력변수
     （Input variables) : 오차값
                           （error), 오차값의 변화율
                                           （change-in-error)
  출력변수
     （Output variable) ; 힘
                         （force)



「亘i回 제어에 대한 지식을 Rule-Base로 구현함


  입력변수와 출력변수를 구간별로 분류하고 가능한 모든 경우에 대한 If-Then 규칙을
 작성해야 한다. 예를 들어 3개의 규칙만 아래와 같이 나열하였다．


  Rulel :If오차값이 Negative-large 그리고 오차값의 변화율이 Negative-large 하면, Then
        출력힘은 Positive-large 이다．
                              （그림 2.7 a)


  Rule2 :If 오차값이 Zero 그리고 오차값의 변화율이 Positive-Small하면, Then 출력힘
        은 Negative-Small 이다．
                           （그림 2.7b)


  Rule3 : If오차값이 Positive-large 그리고 오차값의 변화율이 Negative-Small하면, Then
        출력힘은Negative-Small 이다．
                             （그림 2.7 c)




                                                     2 장 퍼지 시스템 -49


===== PAGE 51 =====
                                            -




                         ［그림 2.기 카트도립진자 시스템의 동작분석


 위와 같이 명령문을 문장으로 작성하게 되면 C언어나 MATLAB에서 프로그래밍으
로 구현하기 어렵다．
          그래서 아래［표 2.2］
                      와 같이 테이블로 작성하는 것이 시각적인 면
이나 프로그래밍 측면에서 매우 편리하다．


                  ［표 2.2] 수치로 표현된 모든 경우｛25경우）
                                            의 퍼지규칙
                                                         오치毆 변화율 (de/dt)
              출력힘
                （u)
                                   -2
                                                -1
                                                              0         1        2
                          -2            2            2          2      1     0
                          -1
                                        2            2         1        0   -1
        오차값
          （e)              0            2        1              0      -1
                                                                            -2
                          1        1                 0         -1      -2
                                                                            -2
                               2        0       -    1         -2
                                                                       -2   -2
［표2.2〕
     에서 오차값, 오차값변화율, 그리고 출력 힘의 범위가 숫자로 표현되어 있음
을 알 수 있다. 각 숫자의 의미는 다음과 같다．


    -2: negative- large
    -1 : negative-small
    0: zero

    1: positive-small
    2: positive- large




          （Matlab/Simulink룰 중심으로）
50－퍼지신경망 제어


===== PAGE 52 =====
 예를 들어 위 표의 첫번째 규칙은 오차값이 -2 (negative-large）
                                           이고 오차값변화율이 -2
(negative-large) 인 경우 출력값이 2(positive-large) 라는 것을 의미한다．


단계3 퍼지 범위
        （집합）
           에 대한 멤버쉽 함수의 구성


 각 퍼지범위에 대한 적합도를 산출하기 위해서 주로 멤버쉽함수를 사용하게 된다．
         은 퍼지범위 중에서 " positive-small" 영역에 속하는 오차값을 나타내고
아래［그림 2.8］
있다. 즉，
     오차값이 0도에서 90도 까지의 범위를 " positive-small" 구간으로 설정하였다．
이 구간의 각도범위에서 각도가 ㅠ/4
                  （즉, 45도）일 때 멤버쉽의 값 /z가 최대값인 1을 가
진다. 반면에, 0도나 90도 에서는 멤버쉬 값이 0이 된다. 다시 말하면, 오차값이 45도 부
근이 되면 " positive-small" 적인 느낌이 가장 강해진다는 의미이고, 오차값이 0도나 90
도로 접근할수록 " positive-small" 적인 느낌이 약해진다는 것을 의미한다．




                                     sitive Sm訓




                               45       90        e(t)
        ［그림 2.8] "pasitive-sma]"에 대한 멤버쉽 함수
                                          （membership function）
                                                              의 설정


 위［그림 2.8］에서 e(t)= 0 일 때 멤버쉽 값 (0)=0 이며, 의미적으로 보면 e(t)=0은 결코

positive-small" l O]_L다라는것을말해준다· e(t)= pil8인경우〃
                                              （퓽) = 0.5수준의멤

버쉽을 가진다. 즉, "positive-small" 의 느낌이 50% 정도로 느껴진다 라고 이해할 수 있을

것' h千· 그렇다면，
           e(t)= ph4 인 경우〃({)=i의 멤버쉽을 가진다· 즉，
                                            "positive-small"

의 느낌이 100% 정도로 느껴진다 라고 할 수 있다. 따라서, 멤버쉽의 값은 설계자의 느
낌에 달라질 수 있음은 당연하다．
                 그러므로, 멤버쉽 함수는［그림 2.9］
                                     와 같이 다양한 모
습을 가질 수 있지만，
           일반적으로 가장 많이 사용되는 멤버쉽 함수는［그림 2.8］과 같은
삼각형의 모습이다.


                                                          2 장 퍼지 시스템－51


===== PAGE 53 =====
         i요


         1.0




                      45      90                           45       90      e(t)
                    Trapezoid                               B이
         i上

                                                      Pos-Srnall
         1.0




                     45      90       e(t)              45       90         e(t)
                    Sharp peak                          Triari이e
               ［그림 2.9] "positive-sm訓'"을 나타내는 다양한 멤버쉽함수 표현


 이제 멤버쉽 함수에 대해 충분히 이해가 되었을 것이다. 그러면, 도립진자의 전체 운
동구간에서 오차값에 대한 퍼지 멤버쉽 함수를 나름대로 구성할 수 있을 것이다.〔그림
2.1이은 도립진자의 오차값, 오차값 변화율, 그리고 출력 힘에 대한 전체 퍼지 멤버쉽
함수 구성의 예이다．



                         Nega-Small     Zero   Pos-Small     Pos-L市cie




                                                                            》
                  -90     -45                    45        90        e(t)




                  -45     -22.5                  22.5      45      de(t)/dt




                                                                            》
                  -20     -10           0       10         20        u(t)

                  ［그림 2. 把］도립진자에 대한 퍼지 멤버쉽함수 구성



52- 퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 54 =====
4. 퍼직 시스템의 동작


 위의 3단계를 거치면 퍼지제어기는 완성이 된 셈이다. 이제는 구성된 퍼지제어기가
어떤 방법으로 작동을 하는지를 이해할 필요가 있다.〔그림 2.3］에서 퍼지제어기의 입
력변수인 오차값
       （e）
         과 오차값변화율
                （e）
                  이 특정한 값으로 입력이 될 때, If-Then 형태의
규칙과 멤버쉽함수로 구성된 퍼지제어기가 어떤 출력힘을 만들어 내는지 이해하도록

하자· 먼저，
      퍼지제어기의 두입력변수의 값이 e(t)=O 그리고 e(t) = 응－윽라고 가정

하자. 그러면 이 값들은〔그림 2.11］에서 보는 바와 같이 임의의 멤버쉽함수 내에 위치
하게 된다．



            a-Lar. .      Ne9a-Sm出얌       ero Pos-Sn溜섶    Pos-Larae




                                                                        》
                  -90      -45                 45        90      e(t)


                                                -Small    P.s-Large




                  -45      -22.5      0        22.5      45   de(t)/dt
                       ［그림 2.1기 입력변수에 대한 멤버쉽 함수


 위 그림에서 보는 바와 같이 오차값 e= O 는 퍼지집합 zero에만 소속이된다. 하지만

오차값변화율 츤＝ 즙 슬는 퍼지집합 zer.와positive-small 집합에도 소속이 된다．
                                                   따

라서，
  이 입력값은〔표 2.2］
              의 25개 룰 중에서 다음 2개의 룰에 영향을 주게 된다．
 ①If오차값이 zero 그리고 오차값변화율이 zero이면, then 출력힘은negative-small 하다．
 ②If오차값이 zero 그리고 오차값변화율이 positive-small하면, then 출력힘은negative-small
   하다．




                                                                2 장 퍼지 시스템 -53


===== PAGE 55 =====
［표 2.3］
      은 작동되는 2개의 룰을 룰 테이블에 표시하고 있다. 따라서, 임의의 입력변
수가 퍼지제어기에 입력이 되면 25개의 룰 중에서 경우에 따라 1개에서 4개의 룰이 작
동하게 됨을 알 수 있다．


                  ［표 2.3] 입력변수에 의해 작동되는 2개의 룰
                                                        （de/dt)
                                                  오치毆 변화율
          출력힘
            （u)
                                   -2        -1
                                                             0               1                   2
                  -2                2        2               2              1                    0
                  -1                2        2              1                    0          -    1
       오차값
         （e)       0                2        1          …    0              -1              -2
                  1                1          0             -1              -2              -2
                       2                0    -1
                                                                 2          -2              -2
 이제, 2개의 룰로부터 퍼지제어기가 출력힘을 계산하는 과정을 알아보기로 하자. 첫

번째 룰을보면 오차값.=0는멤버쉽 값〃(e) =1을가지며 오차값변화율e= 퓽－슬

는 /L(e) - 0.25의 멤버쉽 값을 가진다. 이 때 대표값은 두 멤버쉽 값의 최소값을 선정하
도록 한다．


                               ILrulel = min{0.25,1}= 0.25




                                                    )                  ro




                                                                            뜨5
           그0              0       10 u(t)        -10            0      10           U(t)

                       (a)                                       (b)
                ［그림 2.12] Rulel에 의해 생성되는 출력힘 면적


 위에서 정해진 대표값은 출력변수의 해당 퍼지집합으로 전달되어 진다. Rule1에서
출력힘의 퍼지집합은 zero이다. 여기서 대표값 0.25를 적용하면 rule1에 의해 발생되는



          （Matlab/Simulink를 중심으로）
54－퍼지신경망 제어


===== PAGE 56 =====
출력힘과 관련된 면적을 계산할 수 있다.〔그림2.12 (b)］에서 음영으로 칠해진 부분의
면적이 출력힘 U를 구하는데 이용된다．
 두번째 룰을 보면 오차값 e=0는 멤버쉽 값〃(e) =1을 가지며 오차값 변화율은

〃（츤）= 0.75의 멤버쉽 값을 가진다. 이 때 대표값은 다음과 같이 선정된다．


                        ／尤ruiei _min{0.75,1}= 0.75


 위에서 정해진 대표값은 출력변수의 해당 퍼지집합으로 전달되며, rule2에 의해 발
생되는 출력힘 관련면적은［그림2.13 (b)] 의 음영으로 처리된 면적이다．




        -20    -10           0 u(t)     -20       -10        0 u(t)
                (a)                                  (b)
              ［그림 2.13] RuIe2에 의해 생성되는 출력힘 면적


 결론적으로 두 입력변수에 대한 전체 출력힘은 rule!과 rule2에서 구해진 출력힘의
면적을 이용하여 구해진다.〔그림 2.14］
                      는 전체 출력힘 면적을 나타내는 그림이다．



                                        lt
                       Nega-Srn케
                                          Zero
                      0.75

                                                 0.25

               -20           -10      0 u(t) 10       u(t)

         ［그림 2.1띠 Rulel 과 RuIe20ㅔ 의해 생성되는 전체 출력힘의 계산


 출력힘 면적으로부터 출력힘을 구하는 방법은 다음과 같은 2가지의 방법이 많이 이
용된다 :



                                                             2 장 퍼지 시스템 -55


===== PAGE 57 =====
 ① 면적중심법 (center of gravity method)
 ② 중심평균법 (center average method)


 면적중심법은 전체면적의 도심을 구하는 방법이며 다음과 같은 식에 의해 구할 수
있다．



                                                                     (i)
                                                            Jp
                                              "= i〕J',a(i)
［그림 2.13］
        의 면적에서 면적중심법을 적용하여 면적중심을 구하면


                        0=
                              (o)   ( 375) +
                                    4.
                                                      io)(9.
                                                       (-
                                                            375)                     =             81
                                             4.375 + 9.375
                                                                                          6.
 결국，
   면적의 중심값이 최종적으로 구해지는 제어힘이 되는 셈이다.［그림 2.15］
                                           는전
체면적의 도심을 표시한 그림이다．




                              Nega- Sm訓

                             0.75

                                                                                      0.25

                  -20                    -   10    I             0         u
                                                                               (t)
                                                                                     10        u
                                                                                                   (t)
                                                  u=-6.81

                 ［그림 2.15] 면적중심법을 이용한 출력힘의 계산결과


 위에서 보는 바와 같이 면적중심법은 경우에 따라 면적을 구하는 과정이 약간 복잡
할 수도 있다. 계산을 조금 쉽게할 수 있는 방법이 있는데 두번째 방법인 중심평균법이
다. 중심평균법으로출력힘을계산하는식은다음과같다．




56－퍼지신경망 제어
          （Matlab/Simulink를 중심으로）


===== PAGE 58 =====
                                                               > b,u(i)

                                          " ""   "       -          ￡〃（D
 중심평균법으로［그림 2.13］의 도심을 구하면 다음과 같다．


                       4∼           (o)
                                          (o.25.) +     io)(o.
                                                              75)
                                                               (-
                                                                                                               5
                                                 。25 + 。. 75
                                                                                           -             7·
                                                     .
 중심평균법에서는 각 도형의 면적을 구하지 않고 대신에 멤버쉽 값과 각 도형의 도
심만을 이용하여 계산하는 방식이다. 따라서, 중심평균법이 일반적으로 많이 이용되
고 있는 편이다. 이상에서 설명한 퍼지제어기의 출력힘의 계산과정을 도식적으로 요
약을 하면 아래［그림 2.16］
                과 같이 나타낼 수 있다. 임의의 입력변수
                                      （오차값, 오차값변
  이 퍼지제어기에 입력되면 퍼지제어기의 해당룰이 작동하여 최종적으로 출력힘
화율）
을 생성하는 과정을 잘 표현하고 있다.




    -45    0 45    e(t)        -22.5 0 22.5 de(t》/dt                                           -10                        0       10 u(t)

    If error is zero         and error rate is zero, then                                      force is zero

                                          Pos-Sm해


   쑈二
                                                                                   Nega-
                                                                                                Small-                        ,


                                                                    》
    -45   0    45 e(t)                                       45 de(t)/dt           -20                                    0   u(t)
    If error is zero        and error rate is pos-small, then force is nega-small




                                                                           Nega.   Sma
                                                                                                                .
                                                                                                                    4s<
                                                                                                                                  er。



                                                                                                                                        u(t)
                                                                                                              u=-6.81

              ［그림 2.16] 임의의 입력에 대한 퍼지제어기의 출력힘 계산 과정


                                                                                                                              2 장 퍼지 시스템 - 57


===== PAGE 59 =====
5. Sugeno 퍽직 시스템


 여태까지의 퍼지추론은 가장 일반적인 추론방식인 Mamdani 방식에 기반을 두었다．
여기서는 Sugeno 방식
             （혹은，
                Takagi-Sugeno-Kang 방식이라고도 함）
                                           에 대하여 알아보기
로 하자．
    이 방식은 Mamdani 방식과 매우 홉사하다. 두 추론방식의 전건부
                                         （조건문의 앞
부분）
  는 정확하게 같다. 차이점은 후건부에 있다. Sugeno 방식에서 출력변수에 대한 소
속함수는 상수 혹은 선형식으로 표현된다는 점이 차이점이다. Sugeno 방식의 전형적
인 형태는 다음과 같다.


           IfInput1= xandlnput2=y, thenOutputisz= ax+by+ c


 물론 0차 Sugeno 모델의 경우에는 출력값z 는 상수가 된다 (a=b=0).
 각 퍼지룰에 대한 출력값을 zi 로 정의하면, z 값은 다음 식과 같이 정의되는 가중치
씨와 곱해진다．


                         Wi =AND(Fi(x),尻0仍


 위 식에서 F1,2 (.) 는 입력1과 입력2에 대한 소속함수를 나타낸다. 따라서, 모든 퍼지
룰을 고려한 경우의 최종출력값은 다음과 같이 계산된다．




                                      갸꽈
                                             岬
                      최종출력값 =
                                             們



 위 식에서〃은 퍼지룰의 개수이다. 아래 그림은 Sugeno 방식에서 퍼지룰이 어떻게
비퍼지화
   （defuzzified) 되는지를 잘 설명하고 있다. 입력1과 2가 Sugeno 방식의 퍼지시스
템에 입력되면 해당되는 소속함수 내에서 소속값이 결정되고 AND 규칙에 의해 가중
치 W 값이 결정됨을 알 수 있다. 한편 입력값이 출력 소속함수에 입력되어 출력값z가
결정됨을 쉽게 도식적으로 알 수 있다．




          （Matlab/Simulink를 중심으로）
58－퍼지신경망 제어


===== PAGE 60 =====
                 Inputi




                                                            Output
                                                            level
                                           z= a＞什bn (=

                           ㅁ림 2.17] Sugeno 방식의 퍼지 룰


 Sugeno 방식의 퍼지추론을 구체적으로 이해하기 위해 식당에서 팁을 결정하는 퍼지시
스템 예를 들어 설명을 한다. 입력변수는 식당 종업원의 service와 음식의 질이다. service
는 3개의 멤버쉽함수 poor, good, excellent 를 사용하고 있고 음식의 질 food은 2개의 멤
버쉽 함수 rancid
          （맛이 없는）
                와 delicious  를 사용하고 있다. 출력은 3개의 멤버쉽
                         （맛있는）
함수 cheap, average, generous 를 사용하고 있다.［그림 2-18］은 두 입력변수인 service와 food
의 퍼지함수를 보여주고 있다. 출력변수 tip에 대한 퍼지함수는 Sugeno 형식의 상수를
취하였다. 즉, cheap=l0%, average=15%, generous=20％를 선정하였다. 사용된 퍼지룰은
모두 6개이며 다음과 같이 작성하였다．


     If service=poor AND food=rancid, Then tip=10

     If service=poor AND food=delicious, Then tip=15

     If service=good AND food=rancid, Then tip=15

     If service=good AND food=delicious, Then tip=15

     If service=excellent AND food=rancid, Then tip=15

     If service=excellent AND food=delicious, Then tip=20




                                                                     2 장 퍼지 시스템 -59


===== PAGE 61 =====
                                 自pt van耐Ie ' Fooα

                         ［그림 2.1히 입력변수의 퍼지함수



 여러분이 식당에서 종업원의 서비스와 주문한 음식의 맛이 10점 만점에 각각 5점과
8점쯤 된다고 판단하였을 때 tip(tip은 10％에서 20% 사이）
                                     을 계산하는 과정을 살펴보
 출력값tip에 영향을 미치는 퍼지 룰은 아래와 같다．
자．


      룰3)If service=good AND food=rancid, then tip=cheap
      *4)If service=good ANT) food=delicious, then tip=average


 아래［그림 2.19］
           는 주어진 입력값에 대해 위 2개의 퍼지룰이 상호 작용하여 출력값
을 만들어 내는 과정을 잘 보여주고 있다. 결과적으로 14％의 팁을 주는 것으로 결과가
나왔다．




            （Matlab/Simulink를 중심으로）
60 - 퍼지신경망 제어


===== PAGE 62 =====
  2

  3

  4

  5




                                                                   2I

              ［그림 2.1이 Sugeno 퍼지룰에서 출력값 tip을 구하는 과정


 다음은 Sugeno 퍼지시스템의 출력함수가 0차가 아닌 1차함수인 경우를 살펴보도록
하자. 2 입력변수 X1, X2에 대한 멤버쉽함수가 아래 그림과 같다고 한다．


            SMALL      BIG                              BIG


      。.7
               /        (                  1
                                         0.7
                                   0.3

              x1= 4           10



 그런 다음 아래와 같은 2개의 퍼지룰을 고려해 보자．


      룰1) : IF x1 is BIG AND x2 is MEDIUM THEN u1=xl-3x2
      룰2) :IF x1 is SMALL AND x2 is BIG THEN u2=4+2x1


 주어진 입력값에 대한 최종 출력값을 구해보도록 하자. 주어진 입력값은 각각의 퍼
지함수에서 다음과 같은 소속값을 가지게 된다．




                                                           2 장 퍼지 시스템 -61


===== PAGE 63 =====
 myu-BIG(xl)= 0.3    myu-BKi(x2)=0.35
 myu-SMALL(xl)= 0.7      myu-MED(x2)= 0.75


 따라서, 최종출력값은 다음과 같이 계산된다．


                    U = [0.3(-176) + 0.35(12)]/(0.3 + 0.35) = -74.77




62- 퍼지신경망 제어
           （Matlab/Simulink룰 중심으로）


===== PAGE 64 =====
3장퍼치제어
         지금까지 퍼지시스템을 구성하기 위한 소속함수를 구성하는 방법, 그리고 퍼지 룰
을 작성하는 방법, 또한 주어진 특정한 입력값에 대하여 퍼지시스템이 어떻게 작동하
는가를 개념적으로 이해를 하였다. 이제부터는 퍼지 룰을 이용하여 퍼지제어시스템을
구축하는 과정을 알아보도록 한다．




1. Matlab올 이용한 퍼시졔어


         다음과 같은 역진자의 자세제어를 이한 퍼지제어 시스템을 Matlab을 이용하여 프로
그래밍 하는 예를 보이고자 한다. 평판 위를 움직이는 카트－역진자 시스템은 아래 그림
과 같이 나타낼 수 있다．




                                             3 장 퍼지 제어 63


===== PAGE 65 =====
                                      ［그림 3.1] 카트역진자 시스템



 위 역진자 시스템의 구속조건은 다음과 같다고 가정을 한다．


                                         - 300 < e <300


                                         - 5771 ＜〔 h < 5m



                                         Ill              드        30N


 역진자와 수평이동 카트의 운동방정식이 다음과 같이 근사적으로 표현될 수 있다．



 9(t+ l) =〃（t) + △ · 〃(t)



                    mg' sin(9(t))(f(t)+m,. 1. (a(t). 즈，ㅢ' . sin(O(t))
                                               `                         '                   `                               1,uI                             /
畛＋1)＝〃（t) + △ ·
                                                   +m1.
                                                                     mp · 1 .
                                                                                                 c0s2
                                                                                                              (O       (t)
                                                                                                                              )

h(t+1) =h(t)+L · h(t)


                                                                                \2                                           18。
                      f
                          (t)   +m.      .     .          (
                                                               （t)
                                                              (台
                                                                     ·
                                                                             18。)   "汐
                                                                                                 （ (t)
                                                                                                                   ·
                                                                                                                                    ·   cos   (O
                                                                                                                                                   (t)
                                                                                                                                                         ))
h(t+1) =h(t)+A ·
                                                                                         -               ()
                                                                               n1




64- 퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 66 =====
 위 식에서 여러 파라메터의 값은 다음과 같이 주어진다．


                     g= 9.8
                     m = 1.1 : combined mass ofpole and cart
                     m = 0.1 : mass ofpole
                     △= 0.02 : sampling interval


 위 시스템을 제어하기 위한 퍼지제어기의 입력변수와 출력변수는 아래와 같다．


                                    Input :9, 9, {h, h}
                                    Output: f


 하지만 입력변수 4개를 모두 고려해서 퍼지 제어 시스템을 구성하기는 매우 어렵다．
문제를 간단히 하기 위해서 입력변수는 0와 02개만 퍼지제어기의 입력변수로 선정한
다. 단, 카트가 수평으로 움직이는 것은 -5m - 5m 범위 이내에 있도록 퍼지제어기를 잘
구성해 보도록 하자．



Y애 먼저, 퍼지제어기의 입력변수들에 대한 퍼지 멤버쉽함수를 디자인 해야 한다．
역진자의 각도 0 에 대한 멤버쉽함수를 다음과 같이 5개의 퍼지집합으로 디자인하였다．


    NM          NS                   NS     zE     F冬                    PN1




    -50   -40        -30      -20   -10      0     10     20   30        50
                       ［그림 3.끽 역진자의 각도 9에 대한 멤버쉽 함수



 위 그림에서 다른 퍼지집합보다 ZE(Zero) 집합의 폭을 좁게 설정한 것은 역진자를
목표
 （수직위치，
      즉 각도가 0도）부근에서 각도를 정밀하게 제어하고자 하는 목적이 있
다. 좀 더 정밀한 제어를 위한다면 5개의 퍼지집합보다 7개의 퍼지집합을 사용하는 것
도 좋다. 하지만, 계산시간이 증가하는 단점이 수반된다는 것을 알아야 한다. 위의 퍼


                                                                    3 장 퍼지 제어 65


===== PAGE 67 =====
지 멤버쉽함수를 1차함수를 이용하여 표현하려면 매우 복잡할 것이다. 따라서, 아래와
같은 테이블을 만드는 것이 매우 효과적인 방법이라 할 수 있다．


                              ［표 3.1] 테이블 값으로 표현한 각도 9의 멤버쉽 함수
      -50 -45 -40 -35 -30 -25 -20 d5 -10                 -5            0   5     10   15   20    25       30       35   40   45   50
 NM l0 0.88 0.75 0.63 0.5 0.38 0.25 0.13             0    0            0   0     0    0    0     0        0        0    0    0    0
 NS   0      0   0        0 0.25 0.5 0.75 1.0 0.5         0            0   0     0    0    0     0        0        0    0    0    0
 zE   0      0   0        0    0     0    0    0     0   0.5 1.0 0万              0    0    0     0        0        0    0    0    0
 PS   0      0   0        0    0     0    0    0     0        0        0   0.5 10 0.75 0.5 0.25           0        0    0    0    0
 PM   0      0   0        0    0     0    0    0     0    0            0   0     0 013 0.25 0.38 05 0.63 0.75 0.88 t0



  같은 방법으로 역진자의 각속도에 대한 퍼지 멤버쉽함수를 다음과 같이 디자인 하
였다．


            NM                NS                                  ZE                                 PS                 PM




          -50        40        -30       -20       -10            0         10        20        30            40        50
                              ㅁ림 3.3] 역진자의 각속도 90ㅔ 대한 퍼지 멤버쉽 함수


  이 경우에는 ZE 구간을 상대적으로 넓게 선정하였다. 이는 퍼지제어기의 2입력변수
중에서 위치오차를 줄이는 것을 우선하고 속도오차를 줄이는 것을 덜 중요시 하겠다는
뜻으로 해석을 하면 되겠다. 아래 그림은 위 멤버쉽함수를 테이블로 표시한 그림이다．


                              ［표 3.2] 테이블 값으로 표현한 각도 0으l 멤버쉽 함수
      -50    45 -40 -35 -30          25 -20 -15 d0       -5
                                                                       0   5     10   15   20    25       30       35   40   45   50
 NM 1.0 0.67 0.33         0    0     0    0    0     0    0            0   0     0    0    0     0        0        0    0    0    0
 NS   0     0.33 0.67 1.0 0.8 0.6 0.4 0.2            0    0            0   0     a    0    0     0        0        0    0    0    0
 ZE   0      0   0        0 0.14 0.29 0.43 0.57 0.72 0.86 1.0 0.86 0.72 0.57 0.43 0.29 0.14                        0    0    0    0
 PS   0      0   0        0    0     0    0    0     0    a            0   0     0    0.2 0.4 0.6 0.8 1.0 0.67 0.33               0
 PM   0      0   0        0    0     0    0    0     a    0            0   0     0    0    0     0        0        0 0.33 0.67 1.0



  이렇게 하여 입력변수에 대한 퍼지 멤버쉽함수는 디자인되었다. 남은 것은 출력변
수, 즉 카트에 미는 수평힘에 대한 퍼지 멤버쉽함수를 디자인하여야 한다. 어느 정도


           （Matlab/Simulirik를 중심으로）
66 －퍼지신경망 제어


===== PAGE 68 =====
정밀한 힘을 제어하는 것이 필요하므로 힘에 대한 퍼지집합은 다음과 같이 7개를 사용
하였다．


                                             Force (N)

                   NB         NM        NS       ZE      PS     PM    PB




               -28.8 -19.2          -9.6          0      9.6   19.2   28.8
                         ［그림 3.4] 출력힘에 대한 퍼지 소속 함수



 입출력변수에 대한 퍼지 멤버쉽함수가 선정된 다음 해야 할 일은 If-Then과 같은 퍼

재구칙을 작성해야 한다. 앞에서 설명한 바와 같이 두 입력변수 0와 8의 퍼지집합이
각각 5개 이므로 모두 5x5=25개의 퍼지 予칙이 필요하게 된다. 아래 그림은 25개의 퍼

지규칙을 나타내는 규칙 테이블이다.0와 0의 양의 방향은 반시계방향으로 선정하였
고, 카트에 작용하는 제어힘의 양의 방향은 왼쪽 방향으로 선정하였다．



       FAM (Fuzzy Associate Memory) : Rule Table

                                    C                             0
                        NM    NS        ZE       P$      PM
             NM         I와（上 NB쏘        NM       NS      2玉
             NS         NB    NM        NS       ZE      PS
        0
              ZE        NXi   NS        ZE       PS      PM
              Ps        NS     ZE       Ps       PM      PB
             PM         zE     PS       PM       PB      PB

         (D If 0= NM AND O=NM, then F=NB
         (Z)If 0= Ns AND 0=NM, then F=NB
                    ［그림 3.히 테이블로 표시된 25개의 퍼지규칙



 이상과 같이 하여 퍼지제어기가 구축이 되었다. 이제 퍼지제어기에 임의 입력값을
순차적으로 입력하여 해당되는 퍼지제어기의 출력값을 확인하도록 한다. 아래 표는 두

입력변수의 6加와 0를 -50에서 50까지 5씩 변화시켜 가면서 출력값을 계산한 표이다．


                                                                             3 장 퍼지 제어 -67


===== PAGE 69 =====
             ［표 3.3] 퍼지제어기에 의해 구해진 입력값 9와 90ㅔ 대한 출력힘의 계산

      오     口    C      》     C3     口
                                          珊    C    오    0      퓰 =          戚     髥      00
                                                                                               竇     a,
                                                                                                           00     00    00     00    a,




                 岺 零 零 零 咨                          醫                  휼 =                           會 琵 琵 琵 羈 薰
            00                                                                                 '0
      埠                                        =         。。     '0a,               高 自

      유     a,
                 '0。
                   .
                       '0a,   '0a,   a,   姿    었    드    0
                                                                零 몫          퓻     a,
                                                                                          琵
                                                                                               O0
                                                                                                     r弓    琵 琵 琵 轟 薰
      청ㅋ                      笠      0
                                          晷    딱
                                                    특 塋 輾 盤                  N
                                                                                   笠      0'
                                                                                               蓑 억 聳 艮 흡                       O0    00




      요     竇    N     壅 媛 竪              a,   줄    녑    三： =
                                                          l            00
                                                                       '0    =     요      요    a,
                                                                                                     = 憑          N     = 籌 云
      }r`   芬    OO
                       흙      쯔 즈 釜            a,   驪 竇         。      薰 曹 芬 多 玉                     O'    蜀      rl    N      ;q

      요     甕 望 婆 塋 望                     OO
                                               墨    U)
                                                         蛋      零      0
                                                                             。。    'Oa,
                                                                                               00
                                                                                                     晏     a,     O.    nOa,   a,
                                                                                                                                     르
      뜨；    望 8 笙             a,
                                     墨 晏       N    프    a,
                                                                00
                                                                       螺＝3
                                                                             胃     '0a,   컫    a,
                                                                                                     芬     OU     a,    a,
                                                                                                                               筌     0




      으     瑤 發 發 甚l 發 芬 죠                               0      무      .
                                                                             옇     '0。
                                                                                               裟 芬         0      0
                                                                                                                        彗 竇          0




     『눼
            發 望 晏             0'     望    0
                                               委         a,     쥬      口
                                                                             。。    。'          塋 芬         O'
                                                                                                                  = 竇 芬              a,




      口
            饔 錐 望 蜜 墨 芬 竪                                OU     零      ㅇ
                                                                             。。    a,          N     00U
                                                                                                      ,
                                                                                                           찻      Na,
                                                                                                                        竇      a,    a'




      *r1   鞋 笙 쯔 筌                  a,   즈 竇            깠      00
                                                                       .
                                                                             孕     '0。
                                                                                     s         N
                                                                                                     晏     a,
                                                                                                                  笙     0      a,    eq0'




      요     發 돛l 笠 塋 흐 즈 置                               a,
                                                                a,
                                                                       ㄷ）    '。    몫           多     00
                                                                                                           a,     a,    a,     a,    a,




      二     竇    a,    a,
                              望      a,   芬    N    g    C      a,
                                                                       C     。
                                                                             00。
                                                                                   a,     르    N     즈     a'     O'    多；     N0b
                                                                                                                                     墨
      旨     發 竇 望 發 發 芬 買 多                              '00U   零      0
                                                                             零     。.     끗 芬 墨 섶                 O     a,
                                                                                                                               冕     a,




      ri    {3   N            g〕 뙤        望    00   多 盈         蓄 ※          。     晏 量         a,    竇 驪          OO
                                                                                                                        芬      '0    00




      요     磊    '0    00
                              崙      '0
                                          器 全       요    땃      믄      00C   ：므 았         ｀心
                                                                                               多     '00   N
                                                                                                                  稷     N
                                                                                                                               墨     N




      笭｛
            OO   '0
                       00
                              拓 竇 旨 苔 望 墨 B 晷 弩 드                                         00
                                                                                               '0
                                                                                                     暴            릎
      루 騫 爵 霽 驪 蜀 目 沔                                    졈 포                              드 었 墨
                                                    'O                       a,
                                                                       a,          口                       '00'   。0    ；妥     CCU   '0a,




      쟈     琵 琵 騫 霽 蜀 禽                        '0
                                                    N    高      8 芟          a,
                                                                                   a,
                                                                                          熙    =     。     。。     。。
                                                                                                                        00。
                                                                                                                        。
                                                                                                                               岺     OO



      무     羈 薨 露 琵 崗 絡 霽 弩 臂 高 盤 量                                                '0a,   昏     00
                                                                                               '0    簽     口      ㅇ     ！스     ㅇ     ㅇ




            e    착 斗          씽      穹    y`   슭    땁    鷺      M*     口     `n    요      쬐    요     璥     요      旨     유      땋     오．
                                                                       也



 아래 그림은 위의 표를 3차원 그래프로 재구성한 그림이다. 사실 우리가 퍼지제어기
를 구성한다는 것은 그 제어기의 3차원 그래프
                        （혹은 퍼지제어 곡면）
                                   를 구하는 것이라
할 수 있다．


68- 퍼지신경망 제어
           （MatIab/SimuIink를 중심으로）


===== PAGE 70 =====
                       20
                        ^
                        U
                 m놘숀
                        ^
                        U



                       伯

                       n
                       니
                       。
                       ㅗ


                       nu
                       F


                                                                    50




                                                    出eta


                            ［그림 3.6] 표 3.3의 값을 3차원 그래프로 재구성한 그림


 ［그림 3.7］
        은 역진자에 퍼지제어기를 이용하여 제어 시물레이션을 한 결과를 나타낸
그림이다. 그래프에서 보는 바와 같이 초기각도는 30도로 주어져 있다. 퍼지제어기가
작동하여 -4도에서 4도 사이에서 제어가 됨을 알 수 있다. 마치 숙련된 사람이 역진자를
제어할 때 처럼 역진자가 영점 각도 부근에서 움직이는 것을 볼 수 있다. 영점부근에서
움직이는 각도를 더 줄이고 싶다면 퍼지멤버쉽함수의 개수를 증가하면서 동시에 NS,
ZE, PS 구간을 상당히 좁게 설정한다면 목표를 달성할 수 있을 것이다. 또 다른 방법은
퍼지제어기의 출력힘에 대한 퍼지집합을 잘 설정하는 노력도 기울여야 할 것이다．


  아래 프로그램 pendulum_fuzzy_control.n｝
                                  은 역진자의 퍼지제어를 위한 메인프로그램
에 해당된다．


[pendulum_fuzzy_control.m]
function pendulum_fuzzy_comtrol(theta, thetadot)
%%% 아래 부분은 각도와 각속도의 범위를 나타낸 1차원 배열이다．
scale theta=[-50 -45 -40 -35 -30 -25 -20 -15 -10 -5 0 5 10 15 20 25 30 35 40 45 50];


scale thetadot=[-50 -45 -40 -35 -30 -25 -20 -15 -10 -5 0 5 10 15 20 25 30 35 40 45 50];
%%% 아래 부분은 위 배열 위치에 해당되는 각도 퍼지집합의 멤버쉽함수의 값을 표시한
%%% 2차원 배열이다. 첫번째 행은NM, 두 번째 행은NS의 순서로 작성되어 있다．


                                                                     3 장 퍼지 제어 -69


===== PAGE 71 =====
theta memb 血nc눼
1.0 0.875 0.75 0.625 0.5 0.375 0.25 0.125 000000 00 0 0 00 0;
000000.250.50.751.00.500000000000;
000000 000 0.5 1.0 0.5 00 00000 0 0;
000000000000.51.00.750.50.2500000;
00000000000000.1250.250.3750.50.6250.750.8751.0];


%%％아래 부분은 위 배열 위치에 해당되는 각속도 퍼지집합의 멤버쉽함수의 값을
%%％표시한2차원 배열이다. 첫번째 행은NM, 두 번째 행은NS의 순서로 작성됨
thetadot-memb-func=[
10.67 0.33 00 0000 00 00000000 0 0;
0 0.33 0.67 1.0 0.8 0.6 0.4 0.2 000 00000 00 00 0;
0 0000.140.290.43 0.57 0.72 0.86 1.0 0.86 0.75 0.57 0.43 0.29 0.14 000 0;
00000000000000.20.40.60.81.00.670.330;
0000000000000000000.330.671.0];


%%％아래 부분은 25개의 퍼지규칙을 표시한2차원 배열이다. 배열 내부의 값은
%%％출력힘에 대한 퍼지집합을 나타내고 있다．
%%%NB은 l을 의미하며, NS은 2을 의미한다. PB은 7로 표현되어 있다．
fam=[
11234
12345
23456
34567
45677];


%％아래 부분은 퍼지 출력힘의 퍼지함수의 중심값을 나타내고 있다. 이 중심값은
%％퍼지제어기의 비퍼지화 부분의 계산과정에 사용된다. 사실 단순화된 비퍼지화
%％과정에서는 출력힘의 퍼지함수 자체보다 퍼지함수 각각의 중심값만 사용되어짐
pattern=[-28.8 -19.2 -9.6 0 9.6 19.2 28.8];



70 - 퍼지신경망 제어
            （Matlab/Sim미ink를 중심으로）


===== PAGE 72 =====
%％아래 부분은 프로그램의 주 제어 부분이다. 간단히 설명하면

%%fuzzy-control-surface 함수를 돌려서
%％얻은 해당각도와 각속도에 대한 출력힘의 값을 lookup_table에 저장함
%％그런 다음, 임의의 초기각도 및 초기각속도에 대하여 퍼지제어기가 작동하도록 함


%%Simulation을 위한 초기값 설정
theta = 30;
thetadot= 0;
x= 0;
xdot =0;


k= 1;
pi= 3.14;


pendulum_fuzzy_control; %% pendulum_fuzzy_control.m 함수 호*


while k< 250 %%5초간 시물레이션 수행
fmd_defuzz_angle; %% fmd_defuzz_angle.m 함수호출
force = lookup_table(IS1, IS2);
time = k*0.02;
out(k, 1) = time;
out(k, 2) = theta;
out(k, 3) = thetadot;
out(k, 4) = force;
theta_s = theta*pi/180;
thetadots = thetadot*pill8o;
k=k+1;

pendulum_dynamic; %% pendulum_dynamic.m 함수 호*
end
t= out(:, 1);



                                                            3 장 퍼지 제어 71


===== PAGE 73 =====
angle = out(:,2);
control_force = out(:,4);

plot(t, angle, t,control_force,'--')
xlabel('Time'),ylabel('angle(-) and control_force(--)')
title('Inverted Pendulum Control using Fuzzy Control')


아래의 m 파일은 퍼지제어기의 제어평면을 구성하는 함수이다．

[fuzzy_control_surface.m ]
forl= 1:21
forJ= 1:21
fori= 1:5
forj = 1:5
member(i, j) = min(theta_memb_func(i,I),thetadot_memb_func(j, J));
sum(i, j) = member(i, j )*pattem(fam(i, j));
end
end
num= 0.0;
den = 0.0;
for i= 1:5
forj = 1:5
num = num+ sum(i, j);
den = den+member(i, j);
end
end
lookup_table(I, J) = num/den;
end
end


아래 m 파일은 역진자 시스템에 주어지는 각도 및 각속도 입력에 대한 제어출력값을
생성하는 프로그램이다．



          （Matlab/Simulink를 중심으로）
72－퍼지신경망 제어


===== PAGE 74 =====
[fmd_defuzz_angle.m]
theta_step = 5; thetadot_step=5;
fori= 1:21

pxl(i)= scale_theta(i);
end
forj = 1:21

px2(j)= scale_thetadot(j);
end
if theta< = pxl(1)
ISi = 1;
elseif theta> = pxl(21)
Is! =21;
else
fori= 2:20
if theta> pxl(i-1)& theta < = pxl(i)
if(theta-pxl(i-1)) < theta_step/2
ISi = i-1;
else
IS1= i;
end
end
end
end
if thetadot< = px2(1)
IS2=1;
elseifthetadot > = px2(21)
IS2 =21;
else
forj = 2:20
if thetadot > px2(j-l)& thetadot < = px2(j)



                                              3 장 퍼지 제어 73


===== PAGE 75 =====
if(thetadot-px2(j-1)) <thetadot_step/2
IS2 =j-1;
else
IS2=j;
end
end
end
end


아래 m 파일은 역진자의 동적식을 나타내는 프로그램이다．
[pendulum dynamic.m]
g= 9.8;
m =1.l;
mp= 0.1;
1= 0.5;
delt = 0.02;
theta 1= theta s+delt*thetadot s;
thetadot_1=thetadot_s+delt*(m*g*sin(theta_s)-cos(theta_s)*(force+mp*l*thetadot_s*thetadot_s
*sth(thetas)))/((4/3)*m*l-mp*1*cos(theta-s)*cos(theta-s));
x = x+delt*xdot;
xdot = xdot+delt*(force+mp*l*(thetadots*thetadots*sin(thetas)-thetadot-'s*cos(theta-s)))/m;
theta = theta_1*180/pi;
thetadot = thetadot_l*180/pi;


  이상으로 역진자시스템의 퍼지제어 프로그램이 완성되었다．
  Matlab 창에서 다음과 같이 입력해보자．
  >> pendulum_fuzzy_control(30, 0)
  즉, 초기각도는 30도이고 초기각속도는 0도이다. 이 때 시물레《위크 결과는 아래 그
림과 같다. 그래프에서 실선은 역진자의 각도변화를 나타내며 점선은 퍼지제어기가
출력하는 제어힘을 나타내고 있다．



           （Matlab/Simulink를 중심으로）
74- 퍼지신경망 제어


===== PAGE 76 =====
                                  h肥rted Pendulum Cjitrcl using Fuzzy Cmtrd


                           石


                           加




          一吉e,g
              ㄷ。。귿무나므。 듬
                           佰


                           柏


                           5




                                        t5     2     2.           3   3-5   4   4.5   5
                                                          mil5e

                           ［그림 3.7] 퍼지제어기를 이용한 제어 시물레이션 결과




2. MATLAB 퍼지 툴박스를 이용한 퍼직졔어


 MATLAB에서는 퍼지제어기 설계용 Toolbox GUT를 제공하고 있다. 그림 3.8과 같은
자동차간 거리제어시스템에 퍼지제어기를 적용해 보면 툴박스를 사용하는 방법을 쉽
게 이해할 수 있을 것이다．



0ㅖ 제 3.1 선행차량 B가 임의 속도로 주행하고 있을 때, 여러분이 자동차 A를 운전하고 있

다고 가정해 보자. 여러분의 운전목표는 앞 차와의 거리를 일정하게 d 만큼 유지하는 것이다．
퍼지제어기의 구성을 단계별로 살펴보기로 하자．




                                ［그림 3.8] 자동차 거리제어시스템


 撞互끄 입력변수와출력변수를 정하고 각각의 멤버쉽함수를구성한다．




                                                                                      3 장 퍼지 제어 -75


===== PAGE 77 =====
 입력변수와 출력변수를 정할 때에는 실제 시스템의 제어동작을 가장 잘 설명할 수
있는 인자를 선정해야 한다. 이 예제에서는 입출력 변수는 당연히 다음과 같이 설정되
어야 할 것이다．


      입력변수 : 거리 d
      출력변수 : 브레이크 파워 b


 그리고, 입출력변수에 대한 멤버쉽 함수를 정해야 한다. 비교적 간단한 시스템이고 아
주 정밀한 제어를 필요로 하지 않는다고 가정하면 멤버쉽 함수를 너무 많이 사용할 필요
가 없다. 이 예에서는 입출력 변수를 다음과 같이 3개의 멤버쉽 함수로 각각 구성한다．


      입력변수를 위한 멤버쉽 함수 : short, medium, long
      출력변수를 위한 멤버쉽 함수 : large, medium, none
                                         （혹은 small)


 단계2 MATLAB의 퍼지 toolbox GUI를 다음과 같이 동작시킨다．

      >>fuzzy

                                와 같이 FIS Editor이라는 이름으로 별
 이 명령은 toolbox GUT를 활성화하고〔그림 3.9］
도의 초기화면
      （window）
             을 생 성하게 된다．


                Hs EdhJr〔h桁ned




                  ［그림 3.9] G내화면의 초기화면 (FIS Editor 창）




            （Matlab/Simulink를 중심으로）
76 - 퍼지신경망 제어


===== PAGE 78 =====
  단계키 입출력변수의 멤버쉽함수를 디자인한다．
 초기화면에서 input!로 표시된 블록이 이미 활성화 되어 있다. 따라서，
                                         화면의 오른
쪽에 위치한 name 창에서 입력변수의 이름을 distance로 입력을 하면 창의 화면에서
inputi 이 distance로 변경 될 수 있다．


 다음은 distance로 표시된 입력블록을 더블클릭하면［그림 3.10］
                                       과 같이 입력변수에
대한 입력범위나 멤버쉽함수에 대한 디폴트 설정을 보여주고 있다．


                ; Membersh跡 Funcum Edi;or ummed
                Fl1e Ed打 M·w

                 디S Var, bles                       He'11넓m出中h1Y出에pd8 巾Pd命＝ ,     19
                                       n寸f
                團幽




                         ［그림 3.10] 멤버쉽함수를 보여주는 화면


               1Uembersh嶼 Fon. ti,}n fditDr: untith沁
               翩e ㅌd1I \ew
                                                       汭m吐心냠叩h〃냈1斗琿*씻·   軫蠟련河1'

                                                              〃牡奴洲
               團隙｀



                                                        '`1』v口出착
                                                               ＇i11

                                              毓rnm－뺨中n』1川·｀《d
                                                      ∼    3石
                                              m一 1 … ∼在1．
                                                        ∥好口
                                              ry·         ㅋ    ……써每，
                                                                    二
                                              "m나 …           口
                                                              「1th茹42)

               m．
                나mw

               l,=r==r r:`- 7른》7:ri`



                  ［그림 3.세 입력변수의 멤버쉽함수가 완성된 화면


                                                                                       3 장 퍼지 제어 -77


===== PAGE 79 =====
 Range 창에서 입력변수에 대한 멤버쉽함수의 x축범위를[03이으로 설정해 두자. 이 범
위는 미터단위의 거리라고 생각하면 될 것이다. 현재 활성화되어 있는 함수의 Name을
short라고 지정한다. 그 다음 mf2라고 되어있는 함수를 클릭한 후 역시 Name창에 medium
이라고 지정하고，
        마찬가지로 mf3 함수를 클릭하여 long 이라는 이름을 부여한다．
 이제，출력변수에 대해서도 똑같은 과정을 반복해 보도록 하자.［그림 3.9］의 화면
(FIS Editor）
           에서 Ou中uti 블록을 클릭하여 출력변수의 이름을 brake로 한 후 이 블록을
더블클릭해서 멤버쉽 함수의 x축 범위를 [0 100] 으로 입력한다. 이 범위는 의미는 브레
이크 파워를 0에서 100% 까지 구분해 놓음을 이해할 수 있을 것이다. 그 다음, 각각의
멤버쉽 함수 이름을 none, medium, large로 부여한다.［그림 3.12］
                                             는 출력변수의 멤버쉽
함수가 완성된 화면을 보여주고 있다．


             4M?mbersh,p t-undhon ldilar: UntiU"d                                  G〕
                                                                                    圈
             nle Edㅒ 눠eW
                                                               m*$
                                                    흙令n눕4仰fm엷t口，          1杉．
                                                                            m寸蜜         ISI
              Fls Van.be,
                                                               인
                                                         "． 月1


              甘耳쩍i1   m自Kii




                                           玖n*寸 *mm汰鮮印FJki口l(C.C漱 αJf t. 5i‘논心＞




                                                          ;E丸 1 〕｛〕! 4n


                                                                                  ｀兀숀


             R른
              ＇驪m꿩MF 3t.｀甘騁”




                 ㅁ림 31끽 출력변수의 멤버쉽함수가 왼쌤된 화면


단계4 퍼지제어기의 룰을 생성한다．
 먼저, FIS Editor 창에서 Untitled(mamdani) 블록을 더블클릭한다. 여기서，
                                                     mamdani는
Mamdani 방식으로 퍼지제어기를 구성한다는 뜻이다. 퍼지제어기의 주류를 이루는 2
가지 방법은Mamdani 방식과 Sugeno 방식이 있다는 것을 참고하기 바란다．
                                            더블클릭한
후의 화면은［그림 3.13］
              과 같다．




          （Matlab/Simulink를 중심으로）
78－퍼지신경망 제어


===== PAGE 80 =====
            F海 Ed卄 녀ew Dr川0n今




                    ［그림 3.13] 퍼지 룰을 구성하기 위한 화면


 위 화면에서 입력변수와 출력변수는 각각 3개의 멤버쉽함수가 등록되어 있음을 알
수 있다. 입력함수에 대한 출력함수를 제대로 매칭을 해야 퍼지제어기는 올바른 성능
을 줄 수 있을 것이다. 여러분이 정상적으로 운전을 하고 있다면 차간거리가 short하면
브레이크 힘을 large하게 할 것이다. 따라서, 화면에서 distance 메뉴의 short와 brake메뉴
의 large를 클릭한 후 Add-rule 버튼을 클릭해서 퍼지룰을 등록해야 한다. 같은 방법으
로 medium-medium, long-none으로 매칭해서 Add-rule 하게되면［그림 3.14〕와 같은 화면
을 보여줄 것이다.




                     ［그림 3.14] 퍼지 룰을 생성한 후의 화면


                                                  3 장 퍼지 제어 -79


===== PAGE 81 =====
旦곈흐l 퍼지제어기의 제어곡면（제어 database) 생성됨
        는 최종적으로 생성된 퍼지제어기의 제어곡면을 나타내고 있다. FIS Editor
〔그림 3.15］
화면에서 View 메뉴를 선정한 다음 surface를 클릭하면［그림 3.15］
                                          와 같은 제어곡면을
볼 수 있다. 아래의 그래프에서 수평축은 차간거리이고 수직축은 브레이크의 강도를
나타낸다. 이 경우는 입력변수가 1개 이고 출력변수도 1개 이므로 제어곡면은 곡선의
형태로 표현된다. 입력이 2개이고 출력이 l개인 경우는 퍼지제어기의 제어곡면이 곡
면
（sudace) 형태로 된다는 것을 알아야 한다．


               9

               8o




                               '5      2D   25   30
                             mstance




                    ㅁ림 3.15] 섕성된 퍼지제어 곡면


단계이 생성된 퍼지제어기의 성능확인
 FIS Editor화면에서 \(jew 메뉴를 선정한 다음 rule를 클릭하면〔그림 3.16］과 같은 그
래프를 볼 수 있다. 이 경우 입력변수가 1Sm 인 경우에 대한 퍼지제어기의 동작을 설명
하고 있다. 입력변수의 멤버쉽함수에서 1Sm는 2번째 멤버쉽함수에만 소속됨을 알 수
있고 멤버쉽 값도 1.0 임을 알 수 있다. 따라서, 설계된 퍼지 룰에 의해 멤버쉽 값 1.0 이
대응하는 출력멤버쉽 함수에 전달되고, 그 면적의 중심값을 살펴보면 brake=50임을 알
             은 차간거리＝25m인 경우에 대한 퍼지제어기의 동작을 설명하고 있
수 있다.［그림 3.17］


          （Matlab/Sim미ink를 중심으로）
80－퍼지신경망 제어


===== PAGE 82 =====
다. 이 경우 입력변수가25m 이며 이 값은2번째와3번째 입력 멤버쉽함수에 소속됨을
알 수 있다. 따라서, 대응하는 출력 멤버쉽 함수에 연결되고 출력면적의 중심값원리에
의해 brake:30.4 의 강도로 브레이크를 누르는 명령을 출력하게 된다．




                                                                           /
                                                        ―」솔ㄴ
                                                        \
                                                         \,

                                                                                   }m




                                       Pim mrts
      1
      ＇耳）
        4』   卜*                                    什1
                                                                叫甲1jdo叫 驪
                     『甘ifed. 3 r아e5
       야50ned SYs1em U                                   ,    He   …       -       Close   -
                 ［그림 3.16] 생성된 퍼지제어기의 동작（차간거리＝15m인 경우）



                                                             輓 *S SZ 4

                                                                               /
                                                                       /
             .




                                                                                   1m



    螂t , 2497                         더섞 poW맣：g   10}
                                                        綸ve; 夔」
                                                              壅J，
                                                                竺므l'J
     야ened system Ltmd. 3 flies                              He如                   c蜘e
                                                                                           -
                  ㅁ림 3.1刀 생성된 퍼지제어기의 동작（차간거리＝25m인 경우）



                                                                               3 장 퍼지 제어 81


===== PAGE 83 =====
 위의 예제는 처음 퍼지제어기를 구성하는 학생들에게 퍼지제어기를 쉽게 이해하는
데 좋은 길잡이가 되었을 것이다. 이제 좀 더 현실적인 예제를 다루어 보도록 하자．


예 제 3.2 입력변수를 차간거리 d 와 운전차량의 상대속도 V, 즉 입력변수를 2개로 설정하

여 퍼지제어기의 출력인 brake 강도를 구하는 퍼지제어기를 구성해 보도록 하자．



                                      Relative


                                      -
                          江－    →     speed

                          1    Distance V
                          1
                          I       d




                 ㅁ림 3.18] 상대속도를 고려한 자동차 거리제어시스템



     입력변수와 출력변수를 정하고 각각의 멤버쉽함수를 구성한다．
      입력변수 ; 거리 d, 운전차량의 상대속도 V
      출력변수 : 브레이크 파워 b


 그리고, 입출력 변수를 다음과 같이 3개의 멤버쉽 함수로 각각 구성한다．


      입력변수 d를 위한 멤버쉽 함수 : short, mediumJong
      입력변수 V를 위한 멤버쉽 함수 : slow, medium, fast


      출력변수를 위한 멤버쉽 함수 : small, medium, large


！단계2 MAThAB의퍼지toolbox G내를다음과같이동작시킨다．
      >>fu.zzy
 그리고, FIS Editor 초기화면
                    （window）
                           의 Edit 메뉴에서 Add variable과 I끄put을 선정하
면［그림 3.19］
         과 같은 윈도우를 생성하게 된다．




          （Matlab/Simulink를 중심으로）
82－퍼지신경망 제어


===== PAGE 84 =====
                                 {mamd務n朴




           rnput2




                                  v

                                  v

                                  v

        ＾羽reg煎me                  V

        D·fuz끄再c寸me
                                            Heb




                    ［그림 3.1의 생성된 2입력 1출력 퍼지 시스템 윈도우


CFL. 희입출력변수의 멤버쉽 함수를 디자인한다．
［예제 3.1］
       의 단계3에서 했던 방법으로 멤버쉽 함수를 디자인 한다. 여기서의 차이점
은 입력변수가 2개이므로 차량의 속도 V에 대한 멤버쉽 함수를 추가적으로 디자인 해
야 한다는 점이다．



단계시 퍼지제어기의 룰을 생성한다．
 2개의 입력변수 distance, speed와 출력변수인 brake의 퍼지 룰을 작성해야 한다. 여기
서，
 입력변수 distance와 speed의 퍼지집합은 각각 3개이므로 가능한 퍼지 룰의 경우의
수는9개가 된다.［그림 3.20］
                 는 생성된 9개의 퍼지 룰을 보여주고 있다．




                                                      3 장 퍼지 제어 -83


===== PAGE 85 =====
                 ! .d*dmc亡＂ 拉nn》      ·녑(. m比4｀切W)d,m. mt· 4 mm} (l)
                 2 U (hstUnce U sten1) rU휘
                                         ［s砂ed t5 n比山n）軫1en
                                                         （眈*e 驪 뇰卞）      (1)
                ,3 It (I1恥1ce n 執mt)·닙(eneed 畛 I,서）  甘甘）rbe·ke 驪 1寸鱗）(!)

                j4 准；n縕忿器end
                          end (speedU fl*
                                      UIOW)客en
                                            thenenke
                                                 (bre e쌌(I)}(n
                16 It (1*姓出，
                           Ceth en嫩en) end (SPehdU tut)then(te*et$ 뇰卞〕   (1〕
                』7 It (出Iencn U k，
                                 낑）甘td (t什ed U 5Iow) then (h傲SlIt 3mm) m
                 8 什 ( (1섧留吃e'3,的） a넋 (Upend U emthL,m) then (眈*e It s님)(1)
                '9 rdi U,Ue 3 I3낑)·넋(sf珊ed 蛇 tenet then {t'* 4 好 n닛1出n) (1)



                甘                          ·닙                                                           Ttm,
                             的mc1.              們ㅂ뇨                                                         t〃川幽 蚣
                ______________         ^   F .c            a                                            r쵸쯔－              ^
                ne1力코n                     me1「놀＇n
                kγKj                       m엣                                                           騶，       ’騶
                "：寸1e                      r "y.



                                           [:nte                                                        fl red



                                                         - C牧4e! Je l   Add n. .   -   thenge nie   -
                m功r                                                                             出巾           l        蜘

                                  ［그림 3.2(긔 2입력 1출력 퍼지 시스템의 퍼지 룰



型곈흐l 퍼지제어기의 제어곡면（제어 database) 생성됨
［그림 3.21〕
        은 최종적으로 생성된 퍼지제어기의 제어곡면을 나타내고 있다. FIS Editor
                                          과 같은 제어곡면을
화면에서 View 메뉴를 선정한 다음 surface를 클릭하면［그림 3.21］
볼 수 있다. 아래의 그래프에서 수평축은 distance 와 speed이고 수직축은 brake의 강도
를 나타낸다．




                                     않겨그8
                                   心盤．               v   YGnp빼J)        斗枇1」            V Z (m써teA)               br·
                                                                                                                    【e

                                   b                     Y甲軫＇



         ReL h계：》1漱                                                                             Het              -        Cbse   ㅣ
         Re"y



                                 ［그림 3.2지 최종적으로 생성된 퍼지제어기의 제어곡면



           （Matlab/Simulink를 중심으로）
84- 퍼지신경망 제어


===== PAGE 86 =====
3. MATLAB 퍼직 툴박스를 이용한 Sugenㅇ 방식 퍼직제어


 이 번에는 MATLAB 퍼지 툴박스를 이용하되 Sugeno 방식의 퍼지시스템을 이용하여

이차함수 y = x2를 피팅하는 시스템을 구성해 보도록 한다. y = T2에서 5개의 입력요
소에 대한 출력값은 아래와 같다．



                                         x              y
                                        -1.0           1.0
                                        -0.5           0.25
                                         0              0
                                        0.5            0.25
                                        1.0            1.0


 먼저，
   MATLAB 퍼지 툴박스의 FIS editor 창에서 File>New FIS>Sugeno 를 선택한다．
그러면, 다음과 같은 창으로 된다．


                                                                     口口




                                             t戈t宜논d2

                                             仁




                        Un*"2                                  ＄哨．




                                              크늬UU늬
             m 一
                                눠 林

             客                  越 神


                                …   빼

                                U 一 細                    ㅐ帥1

         Sytem'기
               ＇뻐吐'= 1eci& 1 혀써m丸 甘de[ n*4


              ［그림 3.22] Sugeno 방식의 퍼지시스템을 위한 AS Editor


 inputi 창을 활성화하여 이름을 x로 변경하고, 마찬가지로 output1 창을 활성화하여
이름을y로 변경한다．
          그런 후에 소속함수를 편집한다. 입력값의 범위는 [-1, 1］로 설정



                                                                     3 장 퍼지 제어 -85


===== PAGE 87 =====
한다. 디폴트로 되어 있는 3개의 삼각함수를 5개의 삼각함수로 재구성한다．
 다음，
   출력의 경우도 같은 과정을 수행한다. 출력값의 범위는 [0, 1］로 설정한다. 그런
후 Edit>Add MFs 메뉴를클릭하면 다음과 같은 창이 나타난다．


                                                            higL#




                 ［그림 3.23] Sugeno 방식에서 3개의 소속함수를 선정


  Wtype은 constant 로 선정되어야 한다. OK 버튼을 클릭하면 다음의 창이 나타
               （상수）
난다．




           RS vana비es                     Mer盼efP꺄）M,dㅒ
                                                      ＝nr姓g -   -   r        1r

                                                 m口

                                                 m松

                                                 mn




                               Cment Menje,*q,F心 onf&k a} MF o se'ect)


                               Tp.   ,:
                                                                                  I
                                          He如         -             C;   e            -
           R.耐



             ［그림 3.24] Sugeno 타입의 퍼지시스템의 소속함수 표현


 아래와 같이 원하는 소속함수를 활성화하고 상수의 값을 입력한다. 예를 들어 mf2
소속함수의 경우 상수값 0.25를 입력한다．




          （Matlab/Simulink를 중심으로）
86－퍼지신경망 제어


===== PAGE 88 =====
           FIS Van샀des                                     Me柚e'Sh.I itdK恥P*t pkI -   r－ 而－

                    m                                              mf3

           nn,11    o.出겨五찧                                        rni?




                                                           甲南：H』,磅r好i禽 ot心nii_

          【＇醜* vI泌
          c치                                        Clzrei M8mL硼8婢）fwdiodcbcI on MF too-
          N驪附                 ㅇt只PUn
          T和e                 -                                                            」
          nen5                i ;r 니
          D1斗角y R甲呵e                                        He如




                        ［그림 3.25] 소속함수 mf 의 값을 0.25로 입력


 이제 남은 단계는 퍼지 룰을 작성하는 것이다. Edit>Rules을 선택하여 다음과 같이 룰
을 작성한다．




                 a ft pta1 on12)thentoapa1 iy2ilhI
                 3 If (inpo1 'on寸3)then(oapa1 inyll야
                 4 It (mnm in int4) &1,inhi치겨i1 in y2Hn
                 드 mrM1in nn好) 卄＂n(oiapi朗 iny기LII




                                  「－;-        DeMleu4e J    Add    - chd
                                                                       『好en시




                       ［그림 3.26] Sugeno 타입 퍼지시스템의 룰 작성


 이제 Sugeno 타입의 FIS 시스템이 완성되었다. 결과를 확인하기 위해 View>Rules 을
선택하면 다음과 같은 창을 보게 된다．




                                                                                              3 장 퍼지 제어 87


===== PAGE 89 =====
                             dr;：小
                         i1PJ, - 0J5
                                                 0ttpLII .0625

              }




                  .1
                                                                 I
                                           42                        t2


           i喀｀
             이 075                              Move I.시爐 JdOv! tIJ
            0p. ed oysem UmJed2. 5 s山3s


             ［그림 3.27] Sugeno 타입의 퍼지시스템의 퍼지 룰 작동 oil


 모든 입력의 경우에 퍼지시스템이 어떻게 작동하는 지를 보기 위해 View>Surface 를
선정하면 다음과 같이 퍼지시스템의 입출력관계를 볼 수 있다．


             ' Suftac. v,i》..o,- "n緘Iad?




              ［그림 3.28] Sugeno 타입 퍼지시스템의 제어 Surfce 결과




           （Matlab/Simulink를 중심으로）
88- 퍼지신경망 제어


===== PAGE 90 =====
4. Simulink릎 이용한 펴직졔어


                                       , :    , 10
 간단한2차시스템                                           1。에대하여다양한퍼지제어기를구성해보고자한
                                         2+
                                                4s+
다. 그리고 각각의 성능을 고전적인 PIT) 제어기와 비교하기로 한다．


 1) PID제어시스템



         －◆        +
                                                                                     10
              ◆-         －∼◆
                                                           ++
   Sup                                                                          `2
                   Add                        P
                                                           Adn                 쟈an.r rcn



                           →三
                            ［E컥＞    0毓riMativ*    1<.


                               －》
                                       ㅓ


                                    Megritor      k1




                                                                        4
                                                                Trarsf손＇F.1叫

                                        ［그림 3.29] Simulink를 이용한 plo 제어기 구성




                                                        ［그림 3.30] 스텝응답 비교


 Simulink를 이용하여 아래［그림 3.29］
                          과 같이 PID제어기를 구성하였다. PH) 제어기
의 게인은 Kp=5, Ki=5, Kd=0.7 으로 선정하였다. PH) 제어기를 사용한 경우의 출력과



                                                                                           3 장 퍼지 제어 89


===== PAGE 91 =====
제어기를 전혀 사용하지 않은 경우의 출력을 MUX를 통하여 Scope에 그래프를 출력하
도록 하였다.［그림 3.30］
               는 각각의 경우에 대한 스텝응답을 나타내고 있다. PD제어기
를 사용한 경우가 overshoot도 줄어들고 정착시간도 빨라짐을 알 수 있다．


  2) Fuzzy 제어기


  Matlab의 커멘드창에서 thzzy를 입력하여 FIS(Fuzzy inference system) Editor를 작동시
켜서 아래와 같이 입력변수와 출력변수에 대한 멤버쉽 함수를 디자인 한다.［그림 3.31],
［그림 3.32],［그림 3.33］
                  는 입력변수 e, de와 출력변수 output의 멤버쉽함수를 각각 나타
내고 있다．




       『             芯



           1:｀〃＇'"   v拉毗놂


           綸1立*




           欠·’汁


           m. my 纛心伊
                                   1-
                                        -m－   ㅐet)   -   1


                                      （e)0ㅔ 대한 멤버쉽 함수
                        ㅁ림 3.헤 입력변수인 오차




            （Matlab/Simulink를 중심으로）
90 - 퍼지신경망 제어


===== PAGE 92 =====
                           口,1 1 Mt似）
                                    鬱甘까）F｀
                                         〃｀曲口，
                                             (dCt .＇驪 뉴 -)




                                                               虹洲




蜘


        ㅁ림 q3의 입력변수인 오차율＜de）
                           에 대한 멤버쉽 함수




－襟




                    4g   . 1       44   겸걋  .
                                        눼”m.* '共盼釀r'



                               ㅇ,i'e.1 Mtn뺨* ' Pta由，
                                                   (c1kk 여’"    to I*   t)

              m추r              -                               r 含＇

                               h鮮                              缸枷＃
              m섧
               ＇
                               p甘m1轉


r浚＝甘，
    Y R甘伊


蜘덟Y흼1川* 뇨쇽及i李'




            ［그림 3.33] 출력변수인 output에 대한 멤버쉽 함수




                                                                             3 장 퍼지 제어 91


===== PAGE 93 =====
［그림 3.3니에서 보는 바와 같이 오차가 적은 구간에서 제어정밀도가 필요한 경우에
NS, ZE, PS의 구간을 상대적으로 좁게 하는 것이 바람직하다. 마찬가지로 출력변수인
output에서도 그 구간을 좁게 설정하였다.〔그림 3.34］
                                 은 입력변수와 출력변수를 이용하
여 작성된 25경우의 퍼지룰을 나타내고 있다．



          ! J '!ISOS I` rt) toO l Or'O 傲뵤 t r P 'her} L yiFt41 I乙 山1` ! !                                       ^
          仁 !1 coc. 蹈 r ) Ftod {e.'c Fk' r笠 n劣）t姆n (c,林*4! 1三 F屯l n !
           ? It enOr I r따 fld（驪 c.-傲｀ Ft U 'm,e＇珏奴쳐洲未！ 袗 的）        〔n
          4 !1(en0r 톄因 tod(erc.一d出 乙 m卦tten(0LIt*1 ispIt)(n
          5 It (enm 4 r) 흴넓 (鮮r여-d` 않p)tt'*o (o4pb4l tsz*)(1)
          好11(enOr IS It幻 出꺽料enc..m其 好，삼》     ）U ntc.奴只』     1 IS 的H1)
          7 '.（쵭町驪 " n引骨必（甘r야-d1ts n th醜，           ｛여‘4r二土！ 枉 *) n }
          尹 卄（쐼 ＂'m IS OS) 흴너 佃.0..dcl 4 ze)t?en(c*zpil 닙Pt} m
          9 It (enm 'S 4$) m닙 漱,c.-Fi여 t$ r比 I 卄en 4ss小 竹 it) rn
          h〕汁 re尸Cr 3: Ut ! 聊d ie빵r亡，d《丈 I7 rt 盼戶n m'r1】      1 t r∼ ' f1)
                                                 T쓰盛j ，耳휘不lIJ뀨－                                                 v

          C                     1넌                                                                 n比，
                   甘갈찮 繃          mm）
                                    』d t$                                                            泌慰片4! IS
                           ^
                                 八！
                                  ze
                                 r寒，
                                 rt,




              D ＇ㄴ
                 1 ㄴ
                   …
                   ㅏ
                           V     r心45
                  t
                  心




                 加
                       m

                  m 如
                  노
                  샌 如
                                              l   呻e1e 心·      l   {   AOrmne   J   (c
                                                                                         'Uer너eJ

          r鷺mm h1ㅍㅈy1




          1그 寸  ＇ 甘1'J 1` ie 》 .1』 히＇1' t*여 1ㄴ "` J t1m1 L1여卜4』 ＇ It 5db 1' {
          , 」 " 山＇'m 1= z小 》 m겨J m＇이（土｀" zm 't· 1} ad,겨』        ！ Ii z이 I ',
          쨍 4 It (elF,. I, ！씨 e月， 샙 1이＇｀簿쟈d驥 口 P針tl'Co tm겸p녜I in n，     〕11 〕
          ! 乍 '' (m5, . ii iss) sod )ssos*ikd St tbi) U. ., n出tt恥 m＇寸bㅉ1 }
          16 "（卞.5, IS pSi 5,               心 4 '* )'hm1'rm軟*1 締 mHn
          ! ? Ft         4 r》在〕5,4 (.1,．才001St ＇노＄) tP'enm出"II 好 i1口〕.,)
          !0 It (5,15, ,, ps) ..sl (el...1doI,s xo,)5t o (St烏m好 IS 'tg)(I)
          ! 9 It (SIrS, it 戶5) 甘心 (*눼「r （鸞1좋，
                                            야 心 口引 甘뺌" (alt '.心 Is, t) 1l》
          *勺 뺨！r卞r& IS PS) 甘町      〔m'. 醜m 5 "oth 'It (a轍1 ' 軫 '1b〕      f훵）
          :1 It (0.50' ! 5 rOil .엷 (*n肛ㅗdm 竹 '* 》th·n (m月麴小 *1 55)O》
          ；나 It 10170 ' i二 m) m거1  （小nt麗d,m bins냐liOn (a4515괘！ *' n1) `')
                                '15 )C5'OU嫩艾 55 24'dhto ISt.*們LI *.＾치 n 〕
          1' .) ' 1SIrS, Ii 1*n 0
          ?4 I (51,0 11 m ) .,d IetUw.dm sopt 1 5*0., (55*0Jt 4 Ftn (I)




          r軫“뻐m !｀α＇y1




                                              ［그림 3.34] 퍼지룰의 작성



92          （Mat1ab/Simu)ink를 중심으로）
     퍼지신경망 제어


===== PAGE 94 =====
                  FIS Editor에서 File>Export>ToDisk를 선택하여 Matlab
 이제 퍼지제어기가 작성이 되었다．
의 work 디렉토리에 伽：zy1.fis 이름으로 저장하였다. 작성된 퍼지제어기를 Simulink에 포
함하기 위해서는 Simulink에서 먼저 Fule>New>Model을 선택하여 새로운 창을 생성한
다. 그 다음 Fuzzy Logic Toolbox에서 Fuzzy Logic Controller 블록을 선택하여 마우스로
드래그해서 창에 집어넣는다. 그런 다음Fuzzy Logic Controller 블록을 더블클릭하여 파
일이름을 ' fuzzyl' 으로 입력을 하면 fuzzyl.fis 퍼지로직이 Simulink 윈도우에 삽입이 된
다. 나머지는 아래［그림 3.35］
                  과 같이 회로를 완성할 수 있을 것이다．




                 ［그림 3.35] Simulink를 이용한 퍼지제어기 구성


 위 회로에서［오차＝플랜트의 출력값－기준입력값］
                         으로 설정되어 있다. 즉, 일반적인
개념과는 달리 피드백 값인 플랜트의 출력값이 양의 값으로 피드백되어 있다. 이렇게
하면［그림 3.34］
          의 퍼지룰을 구성하기가 쉽다는 이유에서 약간의 편법을 사용하였다．
회로에서 Gaml, Gain2, Gain3는 성능을 개선하기 위하여 부가된 tuning요소라고 할 수
있다. 오차게인인 Gain3를 증가하면 응답은 빨라지는 경향을 보이고 overshoot이 증가
하는 경향도 동시에 보인다. 반면에 오차율의 게인인 Gaini을 증가하면 감쇠가 증가하
는 경향을 보인다. 고전제어기의 PD제어기의 게인과 유사한 특징을 보인다고 이해하
면 도움이 될 것이다. 출력값의 게인인 gain2를 증가하면 정상상태 오차를 즐여주는 역
할을 할 수 있다. 하지만 overshoot이 증가하는 경향도 동시에 보인다. 퍼지제어시스템
에 대한 스텝응답 결과는［그림 3.36］와 같다. 앞의 PID제어기와 비교해 볼 때 초기의 응
답속도가 매우 빠르며 overshoot의 발생도 거의 일어나지 않았다.




                                                    3 장 퍼지 제어 -93


===== PAGE 95 =====
                 ［그림 3.36] 퍼지제어시스템의 스텝응답



 3) Self-Tuning Fuzzy 제어기


 일반 퍼지제어기는 좋은 성능을 보장하기 위해서는［그림 3.31]∼［그림 3.33］에서 보
는 바와 같이 입출력 멤버쉽함수의 함수범위를 잘 선정하는 것이 필요하며 많은 시행
착오를 겪게한다. 이러한 시행착오를 줄일 수 있는 방법으로 Self-Tuning Fuzzy 제어기
가 있다. Self-Tuning Fuzzy 제어기는 실시간적으로 입출력 멤버쉽함수의 폭을 조절하
여 퍼지룰에 변화를 주는 방법으로 2가지 방법이 있다 : 1）
                                 입력멤버쉽함수를 조정 2）
                                              출
력멤버쉽함수를 조정하는 방법이다．


 (1) 출력 멤버쉽함수 조정을 통한 Self-Tuning Fuzzy 제어기 구성
 먼저 플랜트를 제어하기 위한 퍼지제어기를 FIS Editor를 사용하여 구성한다.［그림
                        은 퍼지제어기의 오차, 오차율 및 제어출력값에 대한 멤버
3.37],［그림 3.38],［그림 3.39］
쉽함수를 각각 나타내고 있다. 전체범위는 -1에서 +1로 설정되어 있고 멤버쉽함수는
특별히 조정할 필요없이 같은 모양의 등분포로 구성되어 있다．




          （Matlab/Simulink를 중심으로）
94－퍼지신경망 제어


===== PAGE 96 =====
攷
          -n




                            C나rm寸 盼的*維孝鮮肖, F촉mc無y렇 (click ci .   h) t的fd)




                                              ’ㅢ《 ．ㅎ J二 引



                                                                       口o.e


R繃y




          ［그림 3.3기 퍼지제어기의 오차입력에 대한 멤버쉽함수



                                                                                （히
 .4-


硼.




c족1rr材唾 VNt姓e                ~:t'r4,t 닙m轍的．
                                          Fnc. , (c* k on 날 10 혀써d)

                礫                                                ":,
                " "
                                               ' ' .5 ! 0 c!


                   ; ` 11

5* ct'd v l以船＼丸·




         ！그림 3.38] 퍼지제어기의 오차율 입력에 대한 멤버쉽함수




                                                                              3 장 퍼지 제어 - 95


===== PAGE 97 =====
                                                   ,，→小－   . →…－             鱗pcfls:   佑1
                                                   "'!＇∼叫】
                                                         ＇ mm  'm…           …
                                                                   '




                  仰1



        *




                                                        碎    닙"m*
                                                                ｀β"


             ㅡ伽
            0ㄴ
             〃rart v〃吐加                    C1T!椎        針却 F｀
                                                            〃由，(dck m 比 to 혀s枕)
             帥                             Nm*                         r t


                                           Tv忙

                                           P夕m4
                             l

                              ！瑋   {   }

            －的    v s寸：눅『aauaii才t'




                        ㅁ림 3.3이 퍼지제어기의 출력값에 대한 멤버쉽함수


 퍼지룰은［그림 3.34］
             에서 제시된 퍼지룰을 그대로 사용할 수 있으므로 따로 설명을
피하였다．
    이상과 같이 설계된 퍼지제어기는 fuzzy2.fis 이름으로 저장하였다．
 Self-tuning frizzy제어기에서는 출력값을 변화
                                （tuning）
                                       하기 위한 별도의 tuning용 Fuzzy
제어기가 필요하게 된다. 이 퍼지제어기 역시 입력변수를 오차
                                （e）
                                  와 오차율
                                      （de）
                                         로 사용
하고 있다. 출력변수는 주 퍼지제어기의 출력값을 튜닝하기위한 가중치로 사용되어
진다. Tuning용 퍼지제어기는 아래［그림 3.40],［그림 3.41］
                                       과 같이 비교적 간단하게 구
성될 수 있다.［그림 3.40〕
                는 오차값 입력에 대한 멤버쉽함수인데 3개의 함수로 구성하
였다. 오차율
      （de）
         에 대한 멤버쉽함수도［그림 3.40］
                            와 똑 같이 구성할 수 있다.〔그림
3.41］
    은 가중치값을 결정하는 출력변수의 멤버쉽함수이다. 가중치는 1에서 10까지 범
위로 설정되어 있다.［그림 3.42］
                   은 가중치를 결정하기 위한 9개의 퍼지룰을 나타내고
있다. 이와 같이 설계된 퍼지제어기를 fuzzy3.fis 이름으로 Matlab의 work 디렉토리에 저
장하였다.




            （Matlab/Simulink를 중심으로）
96 - 퍼지신경망 제어


===== PAGE 98 =====
   "m∼




 ＇a* vm出
0〃                                   《*m m｀贓 'Osdm)
                       令劇m1枇m탤甘的中nm繃驪놔

!4m宕       .           踐m` .                                   戶‘r

！好心        忖｀
            』          Type                                    놀닒                     j
                       P활·m             !.' 6 .! ,n ?,
R솰伊               .

a휙탤·y只m,       1.1 니
                       ：쓰－
                       r,         1艸       ;              I-               '：   沁始        」




   ㅁ림 3.40] Tuning용 퍼지제어기의 오차값 입력에 대한 멤버쉽함수




       m



                            cW,*t 呻＃   .Ft1m'1 (d嘴이，
                                                   W 的 -)

                            N加
           뿌m

                            Tn*                                      棚hJ
           m鞭』
                            P얇齡＄          l」·1 b } t b]




鈿出枉i v心일丘 1申m젼



       ［그림 3.41] 가중치값을 결정하는 출력변수의 멤버쉽함수




                                                                                     3 장 퍼지 제어 -97


===== PAGE 99 =====
         聲*机.b. 1,1．     自bb } 斗1m J ` 『 b * rn
        ＝幷 4 m 4 "4) and《de . 궁 l 쫠뵘 ,
                                    ｛·맬 4 ·＇》II
        蠟J 甘 褘 4 *납）*넓（쵱比 · P$1 ＇·n섭口맬 * n 《11
         蠟4 甘 {e 心 z뺘｀町《侖 . rm ma1f* *．月川n }
         囊s me 4 Z1) 뺨녑 （由 4 脾1甘*n(* m· 1wn
          好 恥솥 a 2t)｀녑  （솔 a 9n 甘， aH． 뺨m뺘 `K1)
          7 （
            甘 큔Im》*넙(a.月nnmm"* *.41)n)
         , 卄 (e4pl)口너   （m a t. · an (* s 甘 m〕《t)
         l. 甘 (. 心 P4} 口넓(I눌 4 m) 甘닢
                                   ＇니Hr*,. . b)(i》



         뺨                   1너
                     . 楡               *   놀

                             -^
         -^
         zt                       z亡
         P흖                  t ':
         'x＇났                "7珊




              '.＇앉           D 'd
              ＜肛i뇨｀
                  ` 1小 `     ，呻




                                               딴：
                                                스」L -*   Hci . ,a.
        ＇心 mm *心y3                                            f－
                                                                   겨枕
                                                                        C幻s.



                           ㅁ림 3.42] 가중치값을 결정하기 위한 퍼지를 설정


  아래 회로는 Simulink로 구성된 self-rn끄ing fuzzy 제어시스템이다. 회로에서 오차값
                                                         （e)
게인인 Gain3의 출력과 오차율
                 （de）
                    의 게인인 Gaini 출력부에 +1과 -1로 saturation을 설치
하였다．
   이는 퍼지제어기의 입력변수인 오차값
                     （e）
                       와 오차율
                           （de) 값의 멤버쉽의 구간이 -1
과＋1의 범위로 되어있기 때문이다．
                  회로에서 몇번의 시행착오 끝에 Gain3=5, gainl=O.1의
상수로 결정하였다. 주 퍼지제어기의 출력게인인 Gain2=7로 선정되었다. 하지만 이 값
은 튜닝퍼지제어기
        （fuzzy logic controller 1）
                                 의 가중치와 곱해져서 최종적으로 플랜트에
입력이 된다．
      플랜트의 출력값 그래프는 Scope를 통해서 알 수 있다. 테스트 중에 오차
값의 변화율
     （de）
        를 측정하기 위하여 5cope2를 설치하였고, 플랜트 입력값을 알아보기
위해서 Scope3를 설치하였다. 그리고 Self-tuning fuzzy 제어시스템의 스텝응답 결과는
［그림 3.44〕과 같다．




98- 퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 100 =====
                 ［그림 3.43] Self-tuning fuzzy 제어시스템




                       ㅁ림 3.4띠 스텝응답 결과


 (2) 입력 멤버쉽함수 조정을 통한 Self-Tuning Fuzzy 제어기 구성
 이 번 경우는 주 퍼지제어기
               （회로에서 fuzzy logic controller로 표시된 블록）
                                                   의 출력값
은 고정되어 있고，
         반면에 입력변수인 오차값
                     （e）
                       에 튜닝용 퍼지제어기
                                 （회로에서 fuzzy
logic controllerl로 표시된 블록）
                         의 결과치를 곱해서 오차값을 가변시키는 경우이다. 이
회로에서 주 퍼지제어기와 튜닝용 퍼지제어기는 앞 절에서 사용된 동일한 fuzzy2.fis와
fuzzy3.fis를 각각 사용하였다.［그림 3.4이에 스텝응답 결과를 나타내었다．




                                                     3 장 퍼지 제어 -99


===== PAGE 101 =====
      ［그림 3.4司 오차값
                 （이의 멤버쉽함수 조정을 통한 Self-Tuning Fuzzy 제어시스템




                      ［그림 3.4이 스텝응답 결과


 4) Self-Tuning Fuzzy-PD 제어기


 Self-Tuning Fuzzy-PD 제어기는 퍼지룰을 이용하여 PD제어기의 게인을 online상에서
계속 변화시키는 형태의 제어기를 말한다. 다음과 같은 2차시스템을 플랜트로 간주해
보자．




100 - 퍼지신경망 제어
             （Matlab/Sim미ink를 중심으로）


===== PAGE 102 =====
                                                   2884
                          G
                                              0.
                                    =
                              (3)
                                    =
                                                     i)
                          G
                                                      2
                              (s)
                                        (s+
 아래 회로는 Self-Tuning Fuzzy-PD 제어시스템을 나타낸다. 그림에서 보는 바와 같이
퍼지제어기는 PD제어기의 2 게인인 Kp와 Kd의 상수에 곱해져서 online적으로 변화시
킴을 알 수 있다．




                 ㅁ림 3.4기 Self-Tuning Fuzzy-PD 제어시스템


 회로에서 퍼지제어기는 이전의 퍼지제어기와는 달리 입력변수가 2개이고 동시에
출력변수도 2개인 형태를 취하고 있다. 만약 여러분이 PH）
                                제어기의 제어게인을 튜닝
하기 위한 퍼지제어기를 구성하려면 입력변수는 2개이며 출력변수가 3개인 형태가 된
다는 것을 알 수 있을 것이다. 이제 PD제어기의 2 게인을 조정할 수 있는 퍼지제어기를
구성해 보자. 이전의 예제와 마찬가지로 MATLAB의 명령창에서 fuzzy를 입력하여 FIS
Editor를 작동시킨다．




                                                              kp
                                    -n刃
                 //H
                                                          \
          彷                                                   kd

                  ［그림 3.48] PD제어기 튜닝용 퍼지제어기


                                                              3 장 퍼지 제어101


===== PAGE 103 =====
 입력변수인 e, de의 멤버쉽함수는 이전의 퍼지제어기와 동일하게 구성하였다. 즉 5
개의 등분포함수로 되어 있으며, 범위도－1에서＋까지의 구간으로설정되어 있다. 퍼지
제어기의 두 출력함수에 대한 멤버쉽함수는［그림 3.49］와 같다. 여기서는4개의 멤버
쉽함수s, m, b, vb를 사용하였고, 범위는 1에서 10 까지이다. 전체 퍼지제어기의 퍼지룰
은〔그림 3.50］
         에 나타내었다．


                               Membershp lunction pc4s m打曲날ㅎ
                                                           ：'                   181




                                    tpA vrib4e 'kpi1
                                   여．
                  ［그림 3.49] Kp와 Kd를 위한 멤버쉽 함수



                ]1 . If (e is nb) end (de is nb) then (kp is vb)(kd is s) (1)
                 2. If (e is nb) end (de is ns) then (kp is vb)(kd is s) (1)
                 3. If (e is nb) end (de is ze) then (kp is b)(kd is 5) d〕
                 4. If (e is nb) end (de is ps) then (kp is m)(kd is m) (1)
                 5. If (cis nb) end (de is pb) then (kp is s)(kd is m) (1)
                I6. If (e is ns) end (de is nb) then (kp is vb)(kd is s) (1)
                l7. If (e is ns) and (be is ns) then (kp is b)(kd is s) (1)
                l6. If (e is ns) end (de is ze) then (kp is m)(kd is m) (1)
                汨If (e is ns) end (de is ps) then (kp is s)(kd is b) (1)
                '10. If (e is ns) end (de is pb) then (kp is s)(kd is vb) (1)
                 11 " (e is ze) end (de is nb) 衲en 야p is s)(kd is vb) (1)
                 12. If (e is ze) end (de is ns) then (kp is s)(kd is b)(1)
                 13 " (e is xc) end (de is xc) then (kp is s)(kd is b) (1)
                 14. If (e is xc) end (de is ps) then 야p is s)(kd is b) (1)
                 15. If (e is ze) end (de is pb) then (kp is s)(kd is vb) (1)
                 16. If (e Isp引 end (de is nb) then (kp is s)(hd is b) (1)
                 17. If (e is 小〕end (de is ns) then 야piss)(kdisb) (1)
                 16. If (e is ps) end (de is xc) then (kp is s)(kd is m) (1)
                 19. If (e is ps) end (de is ps) 衲en 야p is m)(kd is s) (1)
                 20 " (e is 小〕end (de is pb) then (kms b)(kd is s) (1)
                 21 " (e is pb) end (de is nb) then (kp is m)(kd is s) (1)
                 22 " (e is pb) end (de is ns) then (kp is b)(kd is s) (1)
                重23. If (e is pb) end (de is ze) then (kp is vb)(kd is s) (1)
                드:24 " (e is pb) end (de is ps) then (kp is vb)(kd is s) (1)
                l25. If (e is pb) end (de IS Pb) then (kp is vb)(kd is s) (1)

                      ［그림 3.50] 작성된 25개의 퍼지룰


 Self-tuning 퍼지－PD제어시스템의 스텝응답결과는［그림 3.51］
                                        과 같다．



           （Matlab/Simulink를 중심으로）
102－퍼지신경망 제어


===== PAGE 104 =====
                                                (b)
                (a)
                                (c)
   ［그림 3.51] 스텝응답결과 ; (a) 스텝응답 (b) 퍼지출력 Kp의 변화 (C) 퍼지출력 Kd의 변화


0ㅖ 제 3.3 앞에서 다루었던 자동차 시스템을 다시 고려해 보자. 자동차에 작용하는 힘은 엔

진 혹은 브레이크에 의해 전달되는 차 내부의 생성힘 (Fe), 주행 중에 공기가 차체에 미치는 공
기저항힘
   （Fa), 그리고 오르막이나 내리막에 의해 생성되는 지형적 힘
                                    （Fh）
                                       의 3가지로 구분이 가
능하다. 이 자동차 시스템을 속도를 제어할 수 있는 Fuzzy-PID 제어기를 설계해 보자．




              ［그림 3.52] 언덕길에서 주행중인 자동차의 역학 모델


 위의 자동차 모델에 뉴톤의 2법칙을 적용하면 다음과 같은 식을 얻을 수 있다．




                                                      3 장 퍼지 제어 - 103


===== PAGE 105 =====
                         mx= Fe- Fw- Fh


 위 식에서 생성힘
         （Fe）
            는        2000 二 Fe 드 1000의 범위를 가지고 있다고 가정한다．
                                                       이

조건에서 음의 값은 브레이크를 작동하는 경우에 해당되고, 양의 값은 엔진의 출력을
올리는 것을 의미한다. 공기저항힘
                 （Fw）
                    과 지형적 힘
                          （Fh）
                             은 다음의 식과 같이 시간에 따
라 sine적으로 변한다고 가정한다．



                    FW = 0.001(ㅊ+ 20sin (0.01t))2


                        Fh = 30sin(0.0001x)


 위 식을 변형하면 자동차를 추진하기 위해 필요한 생성 힘은 다음과 같이 표현된다．


                        Fe= m5E+ FW+ Fh


 위 식들을 기반으로 Fuzzy-PID 제어기를 구성하고자 한다. 완성된 Fuzzy-PU) 제어시
스템은 아래［그림 3.53］
              와 같이 구성될 것이다．



                                                      》
                                                          +

                            卜
                                皿               1<1
                                                          +
                                                                    Out put

                                FU=ry Logic
                t
                                 Contf이1e'                    dd1




                 ［그림 3.53] Fuzzy-PlO 제어시스템의 구성



 단계별로 나누어서 접근을 하기로 하자．
① 퍼지 입출력 변수를 다음과 같이 설정한다：
       （속도오차）
 입력변수 : e   , de
               （속도오차율）
 출력변수 : PD제어기의 게인값 (Kp, Ki, Kd)



           （Matlab/Sim미ink를 중심으로）
104－퍼지신경망 제어


===== PAGE 106 =====
② 퍼지 멤버쉽함수를 구성한다．
 아래 그림은 Fuzzy-PD 제어기를 구성하기 fuzzy toolbox 모델이다. Matlab의 如zzy toolbox
를 사용하는 방법을 이미 배웠다. 다음과 같이 fuzzy제어기의 골격을 만들어 보자．



        'i l4   gdi t   yi 1핏



                                                                    ///
                                    ,,，∼
                                                    Se1什uxrYmD

                                                       {m心*T卞J心nn


                                                                    \,,,,,
         Fr Nm1"=               8dfl'工zYf戒＞




                                                         JJJJ J
                                                                                       Ck〕
                                                                                         Ce


         R'Cl , ed piSto 섧$IUU2Z們




                                ［그림 3-5긔 Fuzzy Logic Controller 구조


 퍼지에어기의 입력변수인 e
             （속도오） （속도오차율）
                 와 de    에 대한 멤버쉽 함수를 다음과
같이 각각 구성하였다. 입력변수인 e, de에 대한 퍼지 멤버쉽 함수로 각각5개를 사용하
였다. 반면에, 출력변수인 Kp, Ki, Kd 에 대한 멤버쉽 함수는 각각4개를 사용하였다．




                1        08     -06        -04   -02          0     02       04   06   08
                                                  input variable "'e"
                           ［그림 3.5司 퍼지제어기 입력변수의 멤버쉽 함수




                                                                                            3 장 퍼지 제어 -105


===== PAGE 107 =====
                  $                                          B                     vB
                 1




                0.5




                 0
                  0          50     100   150      200     250   300     350       400
                                          output variable "KP"



                                                             8                     硼
                 1



                0.5




                 0
                  0         0.05 0.1 0.15 0.2 0.25 0.3 0.35 0.4          0.45 0.5
                                        output variable Kl



                        S                 M                 B                  W
                       1




                      0.5



                       0
                        0         0.5     1        1.5       2     2.5         3
                                          output variable "KIT

                     ［그림 3.56] 퍼지제어기 출력변수의 멤버쉽 함수


③ 입출력변수의 멤버쉽함수를 이용하여 퍼지룰을 작성한다．
 아래〔그림 3.5刃에서 e＝는속도오차이고，
                       속도오차의 변화율은de= (e(n)-e(n- 1))/At
로 정의하였다. 입출력멤버쉽 변수를 이용하여 각 경우에 대한퍼지룰을 작성할수 있다. 예를
들어，현재 오차는 positive-SIT빼 이고 오차의 변화율은 negative-small이면, KP=sma끄, KI=big.
KD=big로 정하는 경우퍼지룰은다음과 같이 표현된다．


              If e= PS, de = NS, then KP = S,KI= B, KD =B



106 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 108 =====
 e와 de의 멤버쉽함수가 각각 5개이므로 모두 25개의 룰을 작성하여야 한다．


                                                                                                          de
              KP/KI/KD
                                                         NB                           NS                  ZE             PS                  PB
                                   NB               VB/S/S                        yB/B/S                B/B/S         M/B/M                 S/S/M
                                   NS               VB/M/S                        B/B/S                M/B/M          S/B/B             S/MjVB
         e                         ZE               S/MiVB                        S/B/B                S/yB/B         S/B/B             S/MiVB
                                   PS               S/M/B                         S/B/B                SNB/M          M/B/S                 B/M/S
                                   PB               M/S/S                         B/B/S           VBNB/S              VB/B/S            VB/S/S
                                               ［그림 3.5刀 작성된 퍼지를 테이블


                                            과 같이 입력한다．
 그런 다음 작성된 퍼지룰을 퍼지 툴박스의 Rule Editor에［그림 3.58］


                                                                                                                                        1

         Pul. Lht                 Vl.e   Optiene

         1 小(8 1三 ,田) end ides t恒) 卄mn 0P 忖 VbXKh$ s
         2 If Ce d 田) end Ide .eMS) then 螂P 恪 V8XKi Is BXKO is 旬(I)
         3 촛
           ＇〔e Is I好) end (dmP ZE) than (KP Is B》   〔Iq 沚 8)Q(o is 匈(1)
         4 IC (8 islIPS end 8妃 緻 PS) then 小P is M짜l is Brn 놉 川｝(1)
         5 !n:8 is 陷）   end (de 心 P8)then.(P t$ sxId is S好  （D Is닒） .)
         6 Pled NP)히녑(de Is lIPS앉len (isP P V8X1       《1 心 Mx戚＞is 匈(1)
         7 tC (e 心 NP) 넋Ide 扮 PIS)then 0(P is 6)11<1is SXMD is 8)(4)
         B It (e sNS) end (lien ZE)lhen 小PisMXIdis B聊D 沁 吟.)
         9 II (e Is IS) 미엽(lie L多 PS) then 們P is 5) 1K' Is BXI(D I$日）
                                                                    (4)
         lO.h (eisiss)end)   1lenP6)ltien.PiSS黔       《IiP MxMD 軫 VP)(1)
         너 PC.'P z日땅，      d Ide rS NB) then (1<P 四 sX；
                                                      《！！이녀xKD 觸 vB끄' C
         t'                              히넜                              TNan                     려넋                     첨出
                              b
                              ■                    d탸8                            MC나＄                     KH8                  KD 1丘


              翩
                                         幻－
                    冶 戱
                                                                                                                                                    ^
                                                              ∼          5.                .*.    C-
                                                                                                                         -              ^

                                         NS                              I궈                       卜4                     M
                                         zE                              8                        B                      B
                                         P5                               vB                      vB                     v8,
                                                                                                                           ,,




              ”締汪円陌 岫 ㄱ
                                         댜E;                             noen                     n乙ne
                                         『 口3rIe



                                           ＇X才
                                         〔E〕                                                      口〃*                    二〕
                                                                                                                          『Y쟁




         [
                C
                ［〕1꽝始r出r〕
                        n -              CI'써Itt
                      야


                          如

                                                         l   Deieter1』        e   -    Pid r1je        J ｀갸M1叩e nie
         nS N미1r町 8혀卄t』
                      lzyPi)
                                                                                                            Ih    Hisp


                              ［그림 3.58] Fuzzy Rule Editor를 이용한 퍼지를 입력


［그림 3.59〕은 퍼지제어기에 생성된 각 출력변수의 제어평면
                                 （control surface）
                                                 를 나타
내고 있다．




                                                                                                                                        3 장 퍼지 제어 107


===== PAGE 109 =====
                0.4

                0.3

                02

                0.1

                α5
                                                           4
                       0                              α5
                                                  0
                                        4〕5
                        de   4}5   디1
                                              e




                 ［그림 3.5이 생성된 KP, KI, KD 의 제어평면


 이상으로 퍼지제어기 부분에 대한 설계는 완료되었다. 퍼지제어기의 출력값은 PhD
제어기의 입력값으로 들어간다. 예를 들어 KP=50, KI=O.3, KD=2.5 일 경우 PhD제어기
의 블록은 다음과 같이 형성될 것이다. PID제어기의 입력부분은 e
                                   （속도오차）
                                        이고 출력
부분은 Fe
     （추진제어력）
           이다．




           （Matlab/Simulink를 중심으로）
108－퍼지신경망 제어


===== PAGE 110 =====
                          ［그림 3.6이 디0 제어기


                          의 자동차 동적식의 입력으로 들어가게 된다．
 위［그림 3.60］의 Fe 힘이［그림 3.61］


            Ma
           thiust   記r,




                      ［그림 3.6ㄲ 자동차의 동적모델


        은 Fuzzy-PU) 제어시물레이션을 수행하기 위한 전체 제어시스템을 나타
［그림 3.62］
낸 것이다．




                                            3 장 퍼지 제어 -109


===== PAGE 111 =====
  n
  ｛
  …
  …
                                                  －卜
                                                       岫鹹


         －죡1_   距〕_
                                                            84n
         －됴：ㅋ
                  dd皿




                                -
                            {
                                    斗팝핍i h1db11




                        ［그림 3.6끽 Fuzzy-F기D 제어시스템


〔그림 3.63］
        는 Fuzzy-PH）
                  와 일반 PD제어기를 비교하기 위한 블록회로도이다．




           ［그림 3.63] Fuzzy-PID 제어시스템과 일반PID제어기 비교 회로


 아래［그림 3.64］
           은 Fuzz-PU）
                    와 일반 PD제어기를 적용한 경우 자동차 속도제어에 대
한 스텝응답을 비교하였다．
             Fuzzy-PD 제어기의 경우가 응답속도가 빠르다는 것을 알
수 있다. 일반 Pu）
           제어기를 사용하여 응답을 빠르게 하기 위해 게인을 더욱 증가한다
면 상당한 량의 오버슛이 발생하는 문제점이 발생할 수도 있을 것이다．




110－퍼지신경망 제어
           （MatIab/SimuIink를 중심으로）


===== PAGE 112 =====
毋白 p多 β 外 r꼼 r. . a 奪




 1그림 3.6긔 Fuzzy-PlO와 일반 Pl0제어기의 스텝응답 비교




                                          3 장 퍼지 제어 - 111


===== PAGE 113 =====
4장              퍼지제어시스템의응용사례




 ]. 퍽지 졔어기를 이용한 DC 모터의 졔어

     1) DC-Motor의 운동식


     아래 그림과 같이 DC 모터의 수학적인 구조는 토크식과 역기전력 (back EMF) 식으
로 구분된다．



          < Equivalent circuit ofDc machine>

                Lα   R4

                                                 Ra : Amiature win如g re$i囊tance
           +              +                      La : Anuature wzndtg inductance
                                                 e各 : EMF
                                                 va 長 vf: Annatui-e andF`e妃voltage
                                             t
                                             1
                                                 Ia & 董f: Annature andField current

                                      Vf +

     < To띠ue equarion>        < 8ack-EMFe甲,arion>
        r , == K'DIa               ￡α = K4)r沙
                          ［그림 4.1] DC 모터 회로, 토크 및 역기전력 식


                                                     4 장 퍼지 제어시스템의 응용사례 113


===== PAGE 114 =====
 키르히호프 법칙
        （Kirchoff's law）
                       을 이용하여 DC 모터의 특성식을 구하면 다음과 같다．


                                              di,
                       Va = Raia+ Laㅋ
                                     亡+ ea

                                   ea = K w


                                   7길 = Kcbia



                       Te-   TL=        J4+         BW


 위 식으로부터 다음과 같은 변수를 구할 수 있다．


                                    Va (S) -Ea (S)
                       T nn ==
                         "            LaS+ Ra


                          Ea (S) = Kew(S)


                          Te(S) = Ktla (S)


                          \ Te(S) -TL(S)
                       WIS) =  Js+ B


 위 식에서 Te는 모터에 걸리는 토크, J는 모터의 관성모멘트, 그리고B 는 점성마찰
토크와 관련된 감쇠상수이다．


 위 식들을 이용하여 모터의 동적모델을 구현하면 아래 블록과 같다．




114- 퍼지신경망 제어
            （Matlab/Simulink를 중심으로）


===== PAGE 115 =====
                              ［그림 4.의 DC 모터의 모델


 시물레이션을 위해 사용된 모터 파라메터들은 아래 표와 같다．


                                ［표 4.1] motor 파라메터
    La        Ra    J            B       KE       KI         Va     k크       αJ


  0.00405     14   0.05        0.0002   0.4095   0.4095      100   28.5    2000



 위 모터 모델식을 확인하기 위하여 open-loop과 closed-loop 제어기를 구현하여 보았
다. closed-loop 제어기는 P1 제어기를 사용하였다. 아래〔그림 4.3］
                                            에 전체 시스템의 블
록선도가 그려져 있다.［그림4.4］
                  는 open-loop 시스템과 P1제어기를 적용한 경우의 스텝
응답을 비교한 그래프이다．



     Set Spe'ed                                                    Motor Speed
                          Controller              DC Motor                  片




                           ㅁ림 4.이 이osed-loop 제어시스템




                                                   4 장 퍼지 제어시스템의 응용사례 -.115


===== PAGE 116 =====
           eb놉系旦
                                                                   P1
                                                                   0pen Loop
                                                                   Sot speed




                   0.2   0.괘   0.6   0.8      1       1.2   1.4   1.6   1.8
                                           ㄲ,00 (s)

          [2림 4.4] open-loop 시스템과 디제어기를 적용한 경우의 스텝응답


 2) 퍼지로직           을 이용한 DC 모터 제어기
       （Fuzzy Logic）


 퍼지제어기를 구성하려면 입력변수와 출력변수를 설정하여야；한다. 퍼지제어를 위
해 주로 사용하는 입력변수는 다른 일반제어시스템과 마찬가지로 오차값
                                    （E）
                                      과 오차값
의 변화율 따E）
        을 사용한다. 모터의 구동속도를 제어하기 위한 출력변수는 공급전압
 을 사용하였다．
化）
［그림 4.5],〔그림 4.이,［그림 4.7〕은 입력변수와 출력변수에 대한 소속함수를 나타내
고 있다．
［표4.2］
     는 작성된 퍼지룰을 나타낸다. 2개의 입력변수가 각각 5개의 퍼지소속함수를
가지므로 전체 퍼지룰은 모두 25개 이다.［그림 4.8］은 입출력 퍼지함수와 퍼지룰을 이
용하여 생성한 퍼지제어평면을 나타내고 있다．




                     ［그림 4.5] 오차값
                                （E）
                                  에 대한 소속함수



            （Matlab/Simulink를 중심으로）
116- 퍼지신경망 제어


===== PAGE 117 =====
FHe Edn v.w

                                            枷＇t耐nPf嶼乂佃n 현m$
      RS Vanables



  力
  （  E




                     ［그림 4.이 오차값의 변화율
                                    《DE）
                                       에 대한 소속함수


F'I, EdIt Me∼

                                            M메，
                                              t片rsh甲＾翩心i에 少出＄
     RS Varblbles

                                目B              Ns zg可. Ps


  XX E



  XX1班




                                                     ㅝ

                                     `槍     a ．하      a
                                               .姓驪표 Vm4a찮e 차r



                       ［그림 4.7] 출력값
                                  （V0）
                                     에 대한 소속함수


                                ［표 4.2] 퍼지 룰

          DE I E          NB          NS                 Zero    PS    PB
                NB        NB          NB                  NS     NS    PB
                NS        NB          NS                  NS    Zero   PB
              Zero        NS          NS                 Zero    PS    PB
                PS        NS         Zero                 PS     PS    PB
                PB       Zero         PS                  PS     PB    PB




                                                         4 장 퍼지 제어시스템의 응용사례 -117


===== PAGE 118 =====
           me「,I.t View Opn1,ng




                                       ［그림 4.8] 섕성된 퍼지 제어평면


       는 퍼지제어시스템의 Sirnulink 블록선도를 나타낸 그림이다. 그림에서 게
［그림 4.9］
인 8과 9는 입력되는 값이 1로 정규화 되도록 한 값이다．




                                   ［그림 4.9] 퍼지제어기의 Simulink 블록선도


［그림 4.10］
        은 시물레이션 결과이다. 퍼지제어의 경우는 오버슛이 거의 발생하지 않
음을 알 수 있다．



                                                                                           \

                                   刪




                     八E르” 1amb戚，
                                   聊


                                   m


                                   m
                                                                         -Pt
                                                                         -   Fuzzy
                                   0                                     --- sdspeed


                                       02    04   06   08      1   1?   14   16   t8   2
                                                            ieee（引
                                            ㅁ림 4.1이 시물레이션 결과


           （Matlab/Simulink를 중심으로）
118－퍼지신경망 제어


===== PAGE 119 =====
 3) Self-Tuning 퍼지제어기를 이용한 모터제어


 Self-tuning 제어기는 앞의 절에서 구현한 퍼지제어기와 매우 유사하나, 2개의 퍼지제
어 블록을 사용한다는 점이 다르다. 첫 번째 퍼지제어블록은 주 제어기 (main controller)
로 사용되며，
      두 번째 퍼지블록은 첫 번째 퍼지제어기의 입력이나 출력 소속함수（membership
function）
        를 튜닝하기 위한 목적으로 사용된다. 본 절에서는 출력 소속함수를 튜닝하기
위하여 사용되었다. 두 개의 퍼지제어기 모두 앞 절에서와 같이 2개의 입력변수를 사
용하였다.［그림 4.11］
             에서［그림 4.13］
                       은 입력변수와 출력변수에 대한 퍼지 소속함수를
나타낸 그림이다．



     R8V如닐4昑



   川 E




                                                     i탤4' Yn＇님mrㅌ폘

                           ［그림 4.11] 오차값
                                       （E）
                                         에 대한 소속함수



         F1$ variatd昑



    XX             比


    nX   r泛




                          .1   心8   .毓弓   心4   ㅔ 2         0         毓   0.8   a
                                                 h｀月‘ m1*Hbh勺e콜


                        ［그림 4.1의 오차값의 변화율
                                        （DE）
                                           에 대한 소속함수




                                                           4 장 퍼지 제어시스템의 응용사례 119


===== PAGE 120 =====
       目＄VI巾H●＄



      XX
       E



       r茫




                     ［그림 4.1司 출력값
                                （ 吩에 대한 소속함수


［표 4.3］
      은 주제어기에 사용된 25개의 퍼지규칙을 나내고 있으며,［그림 4.14］
                                             는 주제
어기에 임의의 입력값이 주어졌을 경우 주 제어기가 계산해 내는 출력값을 나타낸 그
래프 즉, 퍼지 제어 평면을 나타낸 그림이다


                      匿 4.3] 주제어기에 사띈 퍼지규칙
            DE I E    NB      NS      Zero      PS     PB
              NB      NB      NB       NS      Zero   Zero
              NS      NB      NS       NS      Zero    PB
             Zero     NS      NS      Zero      PS     PB
               PS    Zero    Zero      PS       PS     PB
               PB    Zero     PS       PS       PB     PB




                     ㅁ림 4.14] 주 퍼제제어기의 제어평면


〔그림 4.15］
        에서［그림 4.17］은 두 번째 퍼지 제어기 즉, 튜닝을 하기 위한 목적으로 사
용된 퍼지제어기의 입력 및 출력신호에 대한 소속함수를 나타낸 그림이다.［표 4.4］
                                             는



120 - 퍼지신경망 제어
             （Matlab/Simulinl
                           （를 중심으로）


===== PAGE 121 =====
튜닝용 퍼지제어기에 사용된 25개의 퍼지규칙을 나내고 있으며,［그림 4.18〕은 튜닝용
퍼지제어기에 임의의 입력값이 주어졌을 경우 계산해 내는 출력값을 나타낸 그래프
즉, 퍼지 제어 평면을 나타낸 그림이다．



                                      눼m닐**-m쎄．
                                     H．            !*t1`*ts:   …   …   j   「




        脈刃r刪
        XX
        ㄸ




                                      h헴MV1놀比蠟e뿟


                      ［그림 4.1司 오차값
                                 （E）
                                   에 대한 소속함수



         탸＄Verb脯s




                    ㅁ림 4.16] 오차값의 변화율
                                    （DE)0ㅔ 대한 소속함수




  XX
    쭈
            四
    E
            橓
    …
                ［그림 4.1기 튜닝용 제어기의 출력값 겨!ph게 대한 소속함수



                                         4 장 퍼지 제어시스템의 응용사례－121


===== PAGE 122 =====
                              區 4.4] 튜닝용 퍼지제어기의 제에구칙
                DE I E         NB            NS          Zero            PS        PB
                  NB           NB            NB           NS            Zero   Zero
                  NS           NB            NS           NS            Zero       PB
                 Zero          NS            NS          Zero            PS        PB
                   PS         Zero          Zero          PS             PS        PB
                   PB         Zero           PS           PS             PB        PB




                            ［그림 4.18] 튜닝용 퍼지제어기의 제어평면


 〔그림 4.19〕는 self-tuning 퍼지 제어시스템 전체의 Simulink 선도를 나타낸 그림이며，
［그림 4.20］은 self-tuning 퍼지 제어기와 P1제어기의 계단응답을 비교한 그림이다．




 系莉h
       '
           ,>
                   I
                   ｀·m               ㅏ긔三
                                             醫旨三   0斗a     ！口hd $*m汕‘


                 읗눙*                                                           1
                                                                                        扮－   1




                                       *0
                                              刪
                                             繇瓮
                                                   욜
                         ㅁ림 4.19] Self-tuning 퍼지 제어시스템 Simulink 선도




           （Matlab/Sim미ink를 중심으로）
122－퍼지신경망 제어


===== PAGE 123 =====
                                        刪




                       一E르 ㄲ··nmb石＞
                                        跏



                                        棚



                                        抑

                                                                                P1
                                                                                －口－    -




                                                                            -Self Tuning Fuzzy
                                         0                                  -Set   speed


                                               ．그   0.4   0.5   0.8     1  t2         1.4   1.5   1.8   2
                                                                      Tmr佃

            ［그림 4.201 Self-tuning 퍼지 제어기와 더제어기의 계단응답 비교


  4) Self-Tuning 퍼지 F기 제어기


  이 번 절에서는 퍼지제어기가P1제어기의 Kp게인과Ki게인을 튜닝하는 역할을 하도
록 구성하였다．
       전체 시스템의 구성은［그림 4.21］
                          과 같다.［그림 4.22］
                                       부터［그림 4.25］
                                                 는
각각 오차
    （E), 오차율
           （dE), KP 게인，
                      KI 게인에 대한 퍼지 소속함수를 나타낸 그림이다．
［표 4.5〕
      와［표 4.6］
             은 입력값인 오차와 오차율에 대한 KP와 KI의 출력값을 각각 구하는
퍼지룰을 나타내고 있다．


      n
      八 ㅡ


        x
                   硼
        涵
                   一
                                                    ＇驢二
            a.im                      B`12   勁m소




                                                                                                            !




                                             ㅁ림 421] Simulink로 구현된 전체 제어시스템




                                                                                4 장 퍼지 제어시스템의 응용사례 123


===== PAGE 124 =====
             汝n蝕轍叩F내乂tl어｝E繃oP12
          File Et Fi ew
         …
                Hb vanam略




                            ［그림 4.22] 오차 (E）
                                           에 대한 퍼지 소속함수



         ·Me自始枷i9F며k:bon dit 꺼2
         Fne〔dit 砥w

                                           1m.- , 驪n‘∼h^nd " ,
                                          1』"                        이m渺1m丘
              F好Vaii砒糖＄                   -1 "｀흽m'r mm'. vr. ". `.



                                                    ZE               PS




                          ［그림 4.23] 오차율 (DE）
                                           에 대한 퍼지 소속함수


             M려많驪纛的mtonEth1oPU
          iFIe Elt 喉w

         4      nSVanab跡



             XX 刪
             XX m仇


                            ［그림 4.24] 게인 KP에 대한 퍼지 소속함수



124- 퍼지신경망 제어
            （Matlab/Simuhnk를 중심으로）


===== PAGE 125 =====
       R$e Et V博쀼

      』    F$Vanab昑




                                          烈t執勃帥繃e 乂



                       ㅁ른l4.25] 게인 시에 대한 퍼지 소속함수


                    ！표 4.5] 게인 KP의 출력값을 각각 구하는 퍼지룰
                                               e
               KP
                            N3l    N21   Nil          P11   P2i   P31
                      N3    VB     M      S           S     M     VB
                      N2    VB     M      S           S     M     VB
                      Ni    VB     B      S            S     B    VB
          de          P1    VB     [3     S            S     B    VB
                      P2    VB     M      S            S    M     VB
                      P3    VB     M      S            S    M     VB
                      P3    VB     M      S            S    M     VB


                      ［표 4.6] 게인 KI의 출력값을 각각 구하는 퍼지룰
                                                e
               K
                             N31   N기    Nil          P11   P21   P31
                       N3    VB     B      M           M     B    VB
                       N2    VB     B      M           M     B    VB
                       Ni    VB     M      S           S     M    VB
          de
                       Fl    VB     M      S           S     M    VB
                       P2    VB     B      M           M     B    VB
                       P3    VB     B      M           M     B    VB



                 은 전체 시스템이 동작하면서 PT제어기의 KP게인과 KI게인
［그림 4.2이과［그림 4.27］

이 시간이 지나감에 따라 튜닝되고 있음을 나타내는 그래프이다．


                                                    4 장 퍼지 제어시스템의 응용사례－125


===== PAGE 126 =====
                          KPgarn 아 COIWO確ond and 吐：각PkOI1T얘or

                                                                -  coooer苡01楙
                                                                            （Pgao
                                                                -－油차 (Pg咎n        .




                           05                              1                      t5

                       ［그림 42q Kp 게인의 튜닝과정


                          田9첨no眈orremor囹 and 油可더contr이陋

                                                                -ml싸a볍or硼d9曲l
                                                                --－汕쫘lq咐




                           0.5                             ㅓ                     15

                       ［그림 427] 円 게인의 튜닝과정


                      msem(.I洲t며넋F거 c.曲0釗毓棚｝d缸가더c繃曲虹0Cm京r印·叱Co d
                  덧印伯덖）

                                                                -deord
                      /     ＼∼
                                                                   ㄷ여懈t여닐더




            沁00                  05                    1                  1.5

        ［그림 4.28] R제어기와 self-tuning 퍼지 R제어기의 계단응답 성능 비교


        은 일반적인 P1제어기와 self-tuning 퍼지 PT제어기의 계단응답 성능을 비
［그림 4.28］



           （Matlab/Simulink를 중심으로）
126－퍼지신경망 제어


===== PAGE 127 =====
교한 그래프이다．
［그림 4.29］
        는 앞에서 고려된 4가지 제어기 즉，
                           일반 P1제어기，퍼지제어기，
                                         self-tuning
퍼지제어기, self-tuning 퍼지H제어기의 성능을 같이 비교한 그래프이다．  （rising
                                           상승속도

    는 self-tuning 퍼지P1제아기, self-tuning 퍼지제어기, PT제어기, 퍼지제어기 순으로
time）
빠르게 추종함을 보였다. 일반 P1제어기는 오버슛         이 높게 나타났다．
                          （overshoot）




             r죤나Y요mh乞，



                                                         日』zzy
                                                         SeP TtMHr,g Fuzzy
                                                         Fuzzy-Pt
                                                         Set 야）eed
                         02   0.4   05   00   I   t2   t4    16     1B



            ［그림 4.29] 앞에서 고려된 4가지 제어시스템에 대한 성능비교




2. 반능동
     （Semi-active) 자동착 현가시스템의 퍼직졔어


 1) 차량 모델


 (1) 사용되는 파라메터
 자동차가 불규칙적인 노면 위를 일정한 속도로 움직이고 있다고 가정한다. 노면의
변화값이 차량모델의 입력값이 된다.〔그림 4.30］
                           와［그림 4.31〕
                                    은 각각 2자유도 와 4자
유도 모델을 나타낸다．




                                                       4 장 퍼지 제어시스템의 응용사례 -127


===== PAGE 128 =====
                                 ［그림 4.30] 2자유도 차량 모델


 2자유도 차량 모델에서 사용되는 각 파라메터는 다음과 같이 정의된다．

   mb : mass of the vehicle body (the sprung mass),
   mw: unspru끄g mass of the wheel,
  U: active controller of the front suspension,

   c : damp of the suspension,
  k : stiffness of the suspension,
  k: stiffness of the wheel,

   Zb: displacement of the vehicle body,
   4 : displacement ofthe unsprung mass of the wheel,

   q(t) : input signal ofroad.




                                 ［그림 4.웨 4자유도 차량 모델




           （Matlab/Simulink를 중심으로）
128－퍼지신경망 제어


===== PAGE 129 =====
4자유도 차량 모델에서 사용되는 각 파라메터는 다음과 같이 정의된다．
 mb : mass of the vehicle body (the sprung mass),

 mv: unsprung mass of the front wheel,
 mH7 : unsprung mass of the rear wheel,
 lj : distance between the mass center and the front wheel,
 12: distance between the mass center and the rear wheel,
 I: inertia ofthe sprung mass about mass center,

 uf: active controller of the front suspension,
 ur: active controller of the rear suspension,

 Cf: damp of the front suspension,
 Cr : damp of the rear suspension,

 kf: stiffness ofthe front suspension,
 kr : stiffness ofthe rear suspension,

 사：stiffness of the front wheel,
 kfr: stifThess of the rear wheel,
 Zb: displacement of the vehicle body,
 Z可: displacement of the unsprung mass of the front wheel,
 Z : displacement of the unspru끄g mass of the rear wheel,

 aft) : input signal of the front wheel,
 q,(t) : input signal of the front wheel.


(2) 수학적 모델링
① 입력함수
     （노면변화）
          의 정의
노면변화 q(i）
        는 다음과 같이 정의하였다．



                      4(t) +2;n。     q   (t)   =   γ   2   『G   (n。   )n2u   ·   w   (t)
위 식에서，

 no: spatial frequency,



                                                                      4장 퍼지 제어시스템의 응용사례－129


===== PAGE 130 =====
   Gq(no): road roughness,
   U: velocity of vehicle,
   w(f): white-noise excitation.


 ② 2자유도 모델식
 뉴턴의 법칙을 이용하여 2자유도 모델에 대한 운동방정식을 유도하면 다음과 같다．


                  J          ..   m,
                                       x1+   c   (x1-   x2) +k   (x1-   x2)   =   u
                  1
                  〔m聊x2- c(x1 -x2)- k(x1-X2) + k1x2 = k이‘/ - 'U


 위의 식을 행렬로 표시하면，


                            [J끼z(t나c1加) + [K]坤）
                                              = [/)］α（t)+ [／리11


 위 식에서，



   EM]눼＝" m,
          F   .    -   Cl
          L- c         c 」




          - k  k ㅣ
          [ k k+ 씨




         m
         口］

130－퍼지신경망 제어
           （Matlab/Simulink률 중심으로）


===== PAGE 131 =====
시- l , I·   H      ,7   ,   ,      -
                                [nil  ㄴ ^ m    , 】     , ^
                                                      . ,   .   .   ∼   → ,        ,   ∼，
니4/ H기’ Yi= 乙｝〃2 = 乙’ / == - . . ㅣ 」스 百＝r-,:1, 니 (2片r 나ㅎ놔 g나．
                                                                              ,,
                           LY2J




                  小산‘{C]y1「[K]y2- [P]q(t)+IR]u
                   1Y2 - Yi




위 식에 대한 상태방정식을 구하면，


                                       A Y + BY'= c (t) + Du


위 식에서，




     D나귀
③ 4자유도 모델식
4자유도 모델에 대한 운동방정식을 유도하면 다음과 같다．


                {MIz(t) + [a]z(t) + [/d璥）
                                        =［끼q(t)+ [RIu


위 식에서，




                                                                4 장 퍼지 제어시스템의 응용사례 131


===== PAGE 132 =====
                                                                        0


                                                        口 00
                                                      0 ／                                  0 00瓦
                                  嶋
                        M                                               島
                                  00
                                  0
                                                                        0
                                               + c:                               Cf*ll_ Cr*12                                  - C1                       - C,
                                                                                       댜，
                                        Cf
                                                                                 .,,        2
                            Cf (j - C力2
                            c/*1                                                 Cf* l 2＋+Cr*1                          _
                                                                                                                                                           Cr'l2
                                                                                       1      2
                                                                                                                                                  11
                                                                                                                                Cf*
                                             - Cf                                           _Cf*ll                                Cf                        0
                                             - cr                                                Cr*   l2                             0                     cr




                                                                                                                    亡
                                           r
                                        kf＋시                                     "f/*71- L.r*12
                                                                                 L.                                             －사                           -kr
                                 , *71-                                                                                                                          L. *7
                            1.
                                 f                    kr*
                                                                  12
                                                                                 kf*        亡＋
                                                                                                   k*
                                                                                                    r
                                                                                                                            -         L.
                                                                                                                                           f
                                                                                                                                           /*1,
                                                                                                                                                       1        ' 'r   2
                  [K]   =


                                             -kf                                           -Z f*1l                          사＋ktf                               0
                                             －시                                             시* 72                            0                               kr +ktr




                                 00싸0        00 0 L
                                                  하
                                                                                                                                                                           ㅡ

                  [p1
                                                 r




                  [I키 =




                 위식에서Yi= 2                       ,          Y2=             /,    Ydy1Y2                    라고놓으면
                 위 운동방정식은 다음과 같다．



                                                                  沙쎈Yi'{ci]y,「[K]y2= [P]q(t)「[R1u
                                                                       나/2= 'Ui




             이 식에 대한 상태방정식을 구하면，




imuIink를 중심으로）                                                                                                                                                                 132- 퍼지신경망 제어
                                                                                                                                                                                           （MatIab/:


===== PAGE 133 =====
                       A y+ Bv= c (t)+ Du


 위 식에서，


    .   [[Mi 01
   A= L0' [기j




 위 식들로부터, 차체의 속도와 변위값은 Runge-Kutta 법을 사용하여 구할 수 있다．


 3) 시물레이션


 (1) 2자유도 모델의 시물레이션
 ① 퍼지함수의 설계
 MATLAB의 FIS 에디터를 이용하여 퍼지함수를 디자인하였다. 제어기의 입력 및 출
력변수는7개의 퍼지함수로 구성하였다：NL,NM, NS, ZE, Ps, PM, PL. 입력변수는 위치
오차 및 속도오차로 정하였고，
               출력변수는 힘
                     （force）
                           으로 子정하였다. 변위오차의 입력
범위는 [-0.01 0.01] m, 속도오차의 입력범위는 [-0.10.1] m'c로 설정하였다. 출력값의 범위
는 [-1000 1000] N으로 설정하였다．
                        퍼지 소속함수
                              （membership function）
                                                  는 Gaussian-type의
함수를 이용하였다.［그림 4.32],［그림 4.33],［그림 4.34］
                                      는 입력변수
                                           （위치오차 및 속도
오차）
  및 출력변수에 대한 퍼지 소속함수를 나타내고 있다.




                                       4 장 퍼지 제어시스템의 응용사례 133


===== PAGE 134 =====
             bl*     zdn     v111

               FIS Vatables



              四趨＼
               《ie




                                                            fpU! . ardD好 e

                                                  ＇`1 붉et*ettt뱀1Fl，
                                                c1〃               α1여, (ck* m W= to o的d)

                                                NOun

                                                Type
                                     rt』




                                                                                                -

                            ［그림 4.32] 변위오차
                                         （e）
                                           에 대한 퍼지소속함수



                    1bership Function Editor:    1uzzy4

              叭그*    C4lt     Vi0*

               티S Vatieblea



              匡因 Z砥
                            yott嶼i




                                                           ODUI ,3rane de

                                                Cotreti 比rO右솨叩 ffiatU,on (ckO in 啼r to s小ect)

                                                "1·

                                                ㅜy1"

                                                F뇨 I's


              m4朽ㅜ R히9e


              Sdected v夕．̀
                         B den




                            ！그림 4.3이 속도오차
                                        （de）
                                           에 대한 퍼지소속함수




134          （Matlab/Simulink를 중심으로）
      퍼지신경망 제어


===== PAGE 135 =====
             rI..berd11p Functzon Editot= 1uzxy4
             hi. !dn   v`*1
                                              -口4C拙）         n-           跡치，
                                                                            汁iS
              Rs Valab審e8                                    m十？一小
                                                                                   헥



                                                                     P$        泓   m.




                                              에t翩t V.mb如 ' .dt口UH'




                            ㅁ른l 4.34] 출력힘에 대한 퍼지 소속함수


 이상의 입출력 퍼지함수를 이용하여 퍼지 룰을［표4.7］과 같이 작성하였다．


                                   ［표 4.7] 작성된 퍼지룰
                                                     e
   d
             NL               NM     NS             ZE                    PS       PM       FL
       (e)
   e
   NL        FL               FL     PM             PS                    PS           PS   ZE
   NM        FL               PM      PS            ZE                    PS           ZE   NS
   NS        PM               PS      ZE            ZE                    ZE           NS   NM
   ZE        PM               PS      ZE            ZE                    ZE           NS   NM
   PS        PM               PS      ZE            ZE                    ZE           NS   NM
   P卜月       PS               ZE      NS            ZE                    NS       NM       NL
   FL        ZE               NS      NS            NS                    NM           NL   NL



 퍼지룰을 완료한 후 MATLAB의 Rule Viewer을 클릭하면 다음과 같이 입력값의 변화
에 따른 출력힘의 변화를 그림으로 알 수 있다．
        에서 e=O, de=O이면 output1=2.11*106 이라는 것을 보여준다. e와 de를 나타
［그림 4.35］
내는 선을 drag해서 움직이면 출력힘의 값도 변화하게 된다．       은 모든 입력 경
                                 ［그림 4.36〕
우의 수에 대한 출력값을 3차원 그래프로 표시한 그림이다．




                                                            4 장 퍼지 제어시스템의 응용사례－135


===== PAGE 136 =====
                   F0,le v요e1er = fany4                                                                                                                                                           ;:m 匣1反」
             朴l1 id1`                                                                                    vt11 仲｀1心n'

                                                                                                         0-0                                                              얘높Ut' 휴 2.1 m405




                    ,23* 5. 789粉n侄恪 “ 瑪 獲 作 恪 盼 船 겨 燾 瑟 勇 茹 羽 沁 貂 蚣 沁 겨 路 終 鉀 珥 粉 和 軫 蠶 蠟 〃 蠶
                                                                                                                                                                     --
                                                                                                                                                                     -
                                                                                                                                                                     --
                                                                                                                                                                     -

                                                                                                                                                                                       ／《F∼
                                                                                                                                                                                      一           >



                                                                                                                                                                     一
                                                                                                                                                                     -
                                                                                                                                                                      --                 -m∼ -

                                                                                                                                                                      --                      -
                                                                                                                                                                     -                   m-   ∼
                                                                                                                                                                     -
                                                                                                                                                                     ］    一－      .>              \,j
                                                                                                                                                                                                  -
                                                                                                                                                                     －〃                       ∼
                                                                                                                                                                     -                →－-     ∼
                                                                                                                                                                     -                -       1
                                                                                                                                                                     --
                                                                                                                                                                     -
                                                                                                                                                                     --



                                                                                                                                                                                              ㅣ
                                                                                                                                                                               떽， *




                                                                                                紬
                                                                                                                    .4t                             01
                                                                                                                                                                    to0口                                1羽.



             卜r1                                                                                    cI
                                                                                                                                                                    쓰J쓰撫繃ㅍ蔿蓴
                   야m吐iym似r홰빽r섭ak
                                                                                                                                                          ∼－   d椧                 -              （加1·         -
                                                                                                                     ［그림 4.35] 퍼지룰의 작동


                                                                              S.,, far十 vlt41f.r = f`｀工＇y4

                   hl*                                                                          t쵸｀`      V...   Opt....




                                                                                                                                                                          SI

                                                                                                                           .皿s
                                                                                                                                            4〕05
                                                                                                                            e    001 .01        出


                                                                                                             .             v Yn1．
                                                                                                                                工                        V z〔여心．
                                                                                                                                                               』1

                                                                                                                             Y7*           15




                   啣r




                                                                                                    ［그림 4.36] 퍼지제어기의 제어 표면
                                                                                                                         （surface)


 ② 2자유도 모델에 대한 시물레이션 결과
 차량 현가장치의 응답성능을 알아보기 위해 먼저 도로 노면의 형상을［그림 4.37］
                                             과


            （Matlab/Simulink를 중심으로）
136 －퍼지신경망 제어


===== PAGE 137 =====
같이 생성하였다．
   （passive) 현가장치와 퍼지제어기를 이용한 반 능동
 수동식                             （semi-active) 현가장치에 대
한 가속도，
     속도，
       변위 웅답특성이［그림 4.38」
                       ,〔그림 4.39],［그림 4.40］
                                          에 각각 나타나 있
다. 전체적으로 볼 때 반 능동 현가장치가 수동적 현가장치에 비해 응답특성이 양호한
것을 알 수 있다．




                                   小트甘프旨乫쑈。




                                              ［그림 4 37] 도로 노면 변화
                                                               （입력값）


                      4cㄷ亡뇽mmn .r1큰曲快 沈鬱y                                        螂亡亡勸·鈿n d Ym付
                                                                 2
                                                                                                              -－→ P3ssr1e sus辨什針on
                                                                                                              -    ＄甘ml」adN딴 ＄汐＄的n斜飜


                                                           1    。    4



                                                            rig놜죠i쵱口芝




                 02      (l4        U6        在8   1                              且4        0.6   . 8
                               ㅜn帑播｝                                                   TIm注｝

                      A枕蛇놜磁m 心fm츈枕 b.dr                                          슥cc株可쏘好'0r好陋軫l



                                                                                                        Id)
                                                                 恥




  寸죤ㅌ 饔i닢薑늅各q큰
                                                                 的


                                                         蠶
                                                         ，蠟m口붚
                                                                 沁
                                                                         ㅅ
                                                                             四
                                                                         v
                                                   100           00               4.      楓I
                                                                                  룐m괘哺＇口帥l峠


                                         ［그림 4.38] 차량 2자유도모델의 가속도 응답




                                                                                       4 장 퍼지 제어시스템의 응용사례－137


===== PAGE 138 =====
                                     1／楡｀令 이 Y的m忙 h的r                                                     W奴iy M 쀼鑽蝴

                                                                                                                                         -Pa＄ 騶g-
                                                                                                                                         --   Sui.ad,., su확”ㅔ엷1帥



        。     d


       ＾夔￡ v肛영轟畜，                                                            ＾斗EH＞ · 量




                               綬
                                      84             .6      08        }
                                            ㅜn탔CI)


                                     v     ty醜rt令枕毗r
            04

        3
        。                                                                                    1
                                                                                                I
                                                                                         룝b     4
        ＾
                                                                                                `
                                                                                            ＾흰ㅌ 쯔
        是
        트
        긴
        灌
        ＞
                Q                                     00               似
                                                                       （)                   0       20    40    8                   1倜
                                                                                                          ｀차片찧쟈骨z;


                                                            ［그림 4.39] 차량 2자유도모델의 속도 응답


                                             0'

                                                                                                                                          --- Passm.｀吼I博용n
        。


    젼   4   毛



  一트｛ 麝旨뼜毋。



                        (} 2          04             (} 6    08                                     . 2   n4           . 6   《｀ 8
                                           ㅜ힁，
                                             毛 (1)                                                             'I甘《파

                                   0·9눌．
                                       m닙매m vthb令 b口차                                                     .·－m升이w附
  . 02

                                                                  （댜
     一




                                                                             ＇一i,，晏甘。
                    蝕
                    筐甘
                     ｀
      曲
                                                                                                                                                                   Jl




                                                                                                !
      一             各
                    i
                    1
                    ㄴ
                         20           40     以｝                        100                          20    4.     6.
                                      r的.m句 m }                                                           FmI枷y n推〕


                                                            ［그림 4.40] 차량 2자유도모델의 변위 응답



 (2) 4자유도 모델의 시물레이션
 ① 퍼지함수의 설계
 제어기의 입력 및 출력변수는 7개의 퍼지함수로 구성하였다：NL, NM, NS, ZE, PS,



138－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 139 =====
PM,PL. 입력변수는 위치오차 및 속도오차로 정하였고, 출력변수는 힘
                                      （force）
                                            으로 子정
하였다．
   변위오차의 입력범위는 [-0.01 0.01] m, 속도오차의 입력범위는 [-1 1] n必로 설
정하였다．
    출력값의 범위는 [-10 1이 N으로 설정하였다. 퍼지 소속함수
                                      （membership function)
는 Gaussian-type의 함수를 이용하였다．
                          〔그림 4.41],［그림 4.42],〔그림 4.43］
                                                      은 입력변수
（위치오차 및 속도오차）및 출력변수에 대한 퍼지 소속함수를 나타내고 있다




             ［그림 4.쉐 입력변수인 오차값
                             （e)Oㅔ 대한 퍼지소속함수




             ［그림 4.42] 입력변수인 오차율
                               （de)0ㅔ 대한 퍼지소속함수



                                    4 장 퍼지 제어시스템의 응용사례－139


===== PAGE 140 =====
              」 和.ber           up Functiun Ed』
                                              tor= Fuz工yPunCtionim0F

              hl1       idn     Vlt*

               FIS Vanables                                       《加∥夕h1驪 m뺐pc汕
                                                       i4小’1그mm怏｝加m

                                                      N$        ㄿ            P$   Ph   斗
                          眺꾜
                    e         o"t tl




                                                        m心ㅐ섦 Ywhb '｀心14甘1'




                    ［그림 4.43] 출력변수인 제어힘에 대한 퍼지소속함수


  퍼지제어기의 제애구칙은 앞에서 사용한［표 4.7］
                            과 같다. 생성된 퍼지제어기의 제어표
면
（control surface）
                은［그림 4.44］
                         와 같다．


              ) 5uIfane vle찧황r= F'i-fl yFunct∥끄i4P아r




                                ［그림 4.4퓌 생성된 퍼지제어기의 제어표면




140   퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 141 =====
②4자유도 모델의 시물레이션 결과
                               枓m也r8比n 的r팖蜘奴y                                       央磅‘如 `gm轍出兀n .r必h
                                                                                                    （定 恥dy

                                                                                                                       -PassYs sus伴n羽.i`
                                                                                                                       ∼－-Sem*-adls suspens




                          .2     . 4           .        08    !
                                    ！眈ii〕


                               ㅅ－*m恥 !m曲M耐                                             及C枕奴出軫n *f m샅 W中m


                    (
                    7




渺驪ㅌ 결준驪篁g?                                                         寸毋트＝盒鱗m
                                                                         蠟毋다상
                    。



                    !hd


             。
             섧，나

             5
             1
             4

                          02     .4                》6   《｝8   淫
                                       ！衲긺'$



                                         ㅁ림 4.4司 차량 4자유도모델의 가속도 응답
                                                                 （시간영역）


                               ^Cc驪妃＇a脇려 4h盼h
                                            （契 xdy
                各                                                               的

                     恪




        漱홴i나톺1훙U환
                     札



                     `




                                                   이1         1的                         4.   吼l             8.   1缸
                                                                                         n긔枷啣棚z}

                                                                                               締比이
                                                                                       ^－蜘耐！弓1r，
        t6m




r美E나戶죠i裝운
                    蜘




                    瀜




                                  4.    60               80
                                  孔娜蠱付 卞心｝


                                   ［그림 4.46] 차량 4자유도모델의 가속도 응답
                                                             （주파수영역）




                                                                                           4 장 퍼지 제어시스템의 응용사례 -141


===== PAGE 142 =====
                               v뜅淞礎y 口＇Ye仇m b0dy                                                              AJ多WVeb
                                                                                                                    《勿          把 b町

                                                                                                                                              i- -Pa＄彖紀＄u＄騁n섧m              -
                                                                                                                                              I             cthesupensi i




                                                               是훑ㄴ 니＞쩟즈t, 뇹出5r是
                                                                                                                                                  -   S恥m
              ＾是E一肛心驢오山＞
                           0




                                 .4             05   08   {                                              .2      (} 4         . 6      08
                                      ㅜ펭m ts1                                                                           施開山


                                Vg1戚tyM !m蚣 Wh硼                                                                 Ve妃dy Umr w娜




                           旴                                                                         n
                                                                                                     ,
                                                                                                     毓




       一更드니 卜
            心口
             ＾냘｀>                                                                     繕굿ㅌ 낳
                                                                                          ＞ ·8t>
                           參                                                                         。



                           m


                                                                                                                                       08




                                           ！그림 4 47] 차량 4자유도모델의 속도 응답
                                                                    （시간영역）


                               V볍CdyO! VI& 終 鈿dY




                                                                              ＾
                                                                              之”工
                                                                                戶
                                                                                ㄴ 一＞헷x심乞노 甘md? z
                                                                                                     1




                                                                                                   rJ
                                                                                                   o




                                 Fr텨q寸nㄷy 淇z4                                                                     Fm여J的cy 뺘ㅐL


                               V盼纛”Hr心哄 *M                                                                      Ve勿my 이忙vwb輜




  ｀夔ㅌ 一肛心8重                                                                            ＾휸Ev＞ 댕닛낟畜＞
                    的                                                                                羽



                    加                                                                                珊




                                                          1羽                                             2.       00           60       8{)   too
                                                                                                                  F的t緇n毋 륵H王；


                                        ［그림 4.4히 차량 4자유도모델의 속도 응답
                                                                （주파수영역）




             （Matlab/Simulink를 중심으로）
142 - 퍼지신경망 제어


===== PAGE 143 =====
                                         m驪1h1翊쨍鱗t 嫩Y離嘴紛 飇                                                   物片甘m9帥和 .'Y朴肉軫 姻y


                                                                                                                                              -        Passresispension
                                                                                                4                                             -        Sem饗；act8e suspo

                                                                               n     。      ^
                                                                                            /




        ＾ㅌ一！뇽 戶 m 옵 戇 。
                                                                               `
                                                                               '

                                                                           一
                                                                           볍口， 一 各 枋 ，뇨엷立瀋｀




                                  .2        .4            06    06   灌                                  .2      1〕4         .6     08    1
                                                 T"41)                                                                'gr才伶｝

                                         r)
                                          ＃的”     甘 이軟t 〕Vn之d                                                泳二勵沁月넋供 針m莎 r＇沈唎
                                                                                                5




    小 ㅌ닐 덜 ，＝·。·1쵸丑。
                                                                            m盧v솽뇽，류好布孔瀋。
                           尸
                           느궂



                                                                                                         。

                           。




                                  (L2       .4            06    .8   1                                  02      0』           0s    08    1
                                                 了打好 {`                                                               n好！包



                                                     ［그림 4.4의 차량 4자유도모델의 변위 응답
                                                                             （시간영역）


                                          .密二打t珖＂哺曲 veh蚣뇬 曲학                                                   枷때in로 如鍵ah癩町뵨如令
                          批2
                                                                                                                                                  --
                                                                                                                                                  -＄쩍1枷緘瀚 -
                                                                                                    好                                                       。
               'ci5




m
룝一 ＇玉嘗番쟁꿨牙。                                                                     ^=，一，夔 홉 ，燧
                                                                                          ｀代虛
                          n                                                                         呻                                                       。


                            刪                                                                       們                                                       。             。



                                    2.        4.     60          瓣   t00                                              40      6e    羽l       ｝여
                                              n邯哮驪亡旴｝仕）                                                               fti弔勸댜斛勵


                                           B按緻.驪*않Bf 胞二崗 w刪                                                    伽肉m硼毖rnww娜

                                                                                                    8                                                                         。




                          蝕琶恥乳＇
                                                                                                 4                                                                            。
                                                                                            勺n
                                                                                           ＾ㅌ驪軫됴g灌盈
                                                                                                                                                                              。




                                                                                                    .
                                                                                                                      40      竄              柏0
                                                                                                                      루r的硼俄y聲卦



                                                   ［그림 4.5이 차량 4자유도모델의 변위 응답
                                                                           （주파수영역）


수동식
  （passive) 현가장치와 퍼지제어기를 이용한 반 능동
                                （semi-active) 현가장치에 대



                                                                                                                       4 장 퍼지 제어시스템의 응용사례 143


===== PAGE 144 =====
한 가속도，
     속도，
       변위 응답특성이［그림 4.45]∼
                        ［그림 4.50］
                                에 나타나 있다.［그림 4.45］
                                                 와
〔그림 4.46〕은 시간영역과 주파수영역에서 차체와 바퀴부의가속도 응답을 나타낸 것이
고，
 ［그림 4.47〕
         와［그림 4.48］
                  은 시간영역과 주파수영역에서 차체와 바퀴부의 속도 응
답을 나타낸 것이다.［그림 4.49］
                   와［그림 4.5이은 시간영역과 주파수영역에서 차체와
바퀴부의 변위 응답을 나타내고 있다. 시물레이션 결과에서 알 수 있듯이 퍼지제어기
를 이용한 반능동제어시스템의 변위 응답이 훨씬 우수함을 알 수 있다.




3. 장애물 우회 기능올 갖는 다관절 직능 로봇 시스템

 1) 여유자유도 로봇의 장애물 우회 알고리즘


 여유자유도 로봇은 작업을 수행하기 위하여 필요한 자유도
                              （degree of freedom）
                                                보다
더 많은 자유도를 가지고 있는 경우를 말한다. 어떤 로봇 팔의 끝위치가 주어질 때 끝
위치를 만족하는 로봇 팔의 자세는 무수히 많이 존재하게 된다. 따라서, 이러한 여유자
유도를 이용하여 원하는 로봇의 작동요소를 최적화할 수 있다는 장점이 있다. 예를 들
어 로봇 팔의 작동 중에 소요되는 에너지를 최소화시킨다던지, 특이점
                                    （singular point）
                                                   을
피한다던지，
     원하는 궤적을 따라서 속도 및 힘의 전달율
                           （transmission ratio）
                                              을 최대화할
수 있는 등의 작업을 수행할 수 있다. 여유자유도를 가진 로봇이 움직일 때 돌발적으로
발생하는 장애물을 최적의 자세를 유지하면서 우회할 수 있는 알고리즘을 소개하고자
한다．


 2) 역기구학0nverse Kinematics)


 여유자유도를 갖는 로봇 팔의 모델은 2차원 佯, Y) 좌표계에서 움직이는 3자유도 수
평관절 로봇으로 구성할 수 있다．




144－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 145 =====
                         ［그림 4.51] 3축 수평 다관절 로봇 모델


［그림 4.51］
        에서 로봇 팔의 끝점의 좌표 (q, ey, 熒）와 로봇 팔의 3번째 링크가 佯，
                                                   Y）좌
표와 이루는 각도를 라고 하면，
                로봇 팔의 3번째 링크의 원점의 좌표 (Px, Py）
                                            의 위치는
식
（4.1）
    과 같이 구해진다．


                                             px= ex - 13cos熒


                                             Py = ey - 13sin쑈                                                                     (4.1)


 삼각함수의 공식으로부터


                    2+
            9 I + I 2I,
                                                                                     〃：)=
                                                                        『－
                                                                                                             2
                                                                                                       2+
         p +p       21112cos
                         m8                                                                       =   I +I           21112cos92
             Y 1 2                                                                                                                (4.2)
               2=
                           2.   -            I:
                                                      (2
                                                      (2ir                   -
                                                                                     02)                         -


          x                                                                                            1     2
         .2+
 위 식을 정리하면


                                                             2                   2            2        2
                                                      p +p -I- I
                                                             ,'                  "            1        '1


                                    cos02= "                                     21112"


                                     sin02        =               /1_                       cos202                                (4.   3)
                                                                                                      4장 퍼지 제어시스템의 응용사례－145


===== PAGE 146 =====
 식
 （4.2）
     로 부터 2번째 관절각 는 식
                    （4.4）
                        와 같이 구해진다．


                             〃2= atan2(sin02, cos02)                              (4.4)


［그림 4.51］에서



                                    3= atan2 (p,,py)


                                           2   2  2
                                                                   2
                                         p,x+p,y+1-
                                                  1                2
                                                                   /
                            즌= cos_1
                                              2   『
                                                ( 2            2
                                             211Vpx +p1'                          (4.5)


 그러므로, 01, 03는 다음과 같이 구해질 수 있다．



                                      〃1 =        β－   中

                                    03 = b- 01 -이                                 (4.6)


                                                             징애줄
                                                           (X0》
                                                              욕 Yb四)
                          옥 표우｛ 치
                          (X9, Y숩
                               " " ∼，
                                    , . Gap


                                                       1ig衲
                                                                       초기위치
                                                                            Vi)
                                                                       %.
                                                            Rob이 ^mi
                      －   --'－           跡
              ，   戶

                          ！그림 4.5의 로봇 팔과 장애물의 모델




           （Matlab/Simulink를 중심으로）
146－퍼지신경망 제어


===== PAGE 147 =====
  3) 퍼지논리를 이용한 장애물 우회 계획


［그림 4.52］
        는 로봇이 움직일 때 돌발적으로 발생한 장애물이 로봇 팔의 끝점의 진행
방향 가까이 놓여져 있는 모습을 보여주고 있다. 퍼지제어를 이용하기 위하여 필요한
입력변수는 Gap과 Length로 선정하였다．
                        Gap은 로봇 팔의 끝점
                                    （end effector）
                                                 이 진행방
향의 선상으로부터 장애물의 법선방향으로 떨어진 거리로 정의되고, Length는 장애물
이 로봇 팔의 끝점에서 로봇 팔의 진행방향으로 떨어져 있는 거리로 정의된다．


［그림 4.52］
        에서 0g。
             al' 0。s 그리고 len。
                            b：는 아래와 같이 표시된다．




                                           0g。       al=                 tan       '   （                壑
                                                                                                        【
                                                                                                        1J
                                                                                                          "
                                                                                                          ＇ ^
                                                                                                           』＇
                                                                                                                꼇
                                                                                                                             `^/
                                                                                                                                       ）                 (4.7)



                                                      =            tan
                                                                               1   (       YOb8
                                                                                                                    -         Y
                                                                                                                             X                           (4.8)
                                    〃。bs
                                                                                       X。                 bs
                                                                                                                    -




                        LenOb
                                ,                =    γ    (XOb8
                                                                               →
                                                                                                  ）2+                   (Y
                                                                                                                                  ,b
                                                                                                                                       ,   -
                                                                                                                                               y)   2
                                                                                                                                                         (4.9)


   gap을 다음과 같이 정의하면

                                                     〃gap = 0g。
                                                              al - 9。
                                                                    bs                                                                                  (4.10)


  퍼지제어기의 입력변수 Gap과 Length는 다음과 같은 식으로 표시된다．


                                                 Gap = Len。
                                                          出sinOgap                                                                                      (4.11)


  그리고，
     퍼지제어에 사용된 출력변수는 △0
                      （로봇 팔의 끝점의 이동방향 수정각）
                                         로
선정하였다．
  입력변수의 퍼지 세트 Gap은 NB(Negative Big), NS(Negative Snll), Z터Zero), PS(Positive
Simil), PB(Positive Big）
                       으로 선정하였고, Length는 ZE(Zero), PS(Positive Small), PM(Positive
Medium), PB(Positive Big）
                        으로 선정하였다．
                                출력변수에 대한퍼지 세트는ZE(Zero),PS(Positive



                                                                                                                             4 장 퍼지 제어시스템의 응용사례 147


===== PAGE 148 =====
Sma끄）
    ,P (Positive Medium), PB(Positive Big),PV (Positive Vety Big）
                                                                으로선정하였다．
 소속함수
    （fuzzy membership function）
                              는［그림 4.53］
                                       에 나타나 있다．




                 -2n   -1,5        』5    riD   0.5      15   2[1

                                         由p




                  zE          ＇冬    F끼                       PVH




                  ［그림 4.53] 퍼지 입력변수 및 출력변수의 소속함수


 입력 및 출력변수의 퍼지세트에 대한 퍼지제애구칙인 FAM(Fuzzy Associative Memoiy)
                FAM이란 입력변수와 출력변수의 퍼지세트간의 논리적으
은［표 4.8］에 나타나 있다．
로 타당한 IF-ITHEN 규칙을 함축적으로 나열한 것이라고 볼 수 있다. 예를 들어 FAM의
좌측상단의 블록을 달리 표현하면 다음과 같은 논래子칙으로 표시된다．


                   IF Length is ZE and Gap is NB, THEN is PVB.


 그리고, 퍼지제어기는FAM을 이용하여 임의의 입력변수가 입력되었을 때 비퍼지화
(defuzzification method) 방법을 이용하여 명확한 출력값을 제공하게 된다．




            （Matlab/Simutink률 중심으로）
148 －퍼지신경망 제어


===== PAGE 149 =====
                                （FAM)
                    匪 4.8] 퍼지제에구칙
                                      Length
                       ZE           PS         PM    PB
           NB         PVB           PVB        PVB   PB
           NS         PVB           PVB        PB    PB
   Gap     ZE         PVB           PB         PB    PM
           PS         PB            PB         PM    PS
           PB         PB            PM         PS    ZE


 4) 자세 최적화
         （Posture Optimization)


 여유자유도를 갖는 로봇 팔의 속도는 높은 차원의 관절공간.omt space）
                                          에서 낮은 차
원의 작업공간
      （task space）
                 으로 식
                    （4.12）
                         와 같이 치환
                               （mapping）
                                       이 된다．


                        x*=J(o)o*                         (4.12)

                                                는관절좌표 벡터이며，
 여기서, X=[x1, x2, …, Xm1T는작업좌표 벡터이고 〃＝［이,〃2, …, 아〕
J는mxn자코비안 행렬이다. 식
                （4.12）
                     에 대한 역기구학식은 식
                                 （4.13）
                                      과 같이 구해진다．


                       J+x*+(J_ J+J)K                     (4.13)


 식    에서 J' 는 자코비안 행렬의 수도－인버스
 （4.13）                     （pseudo-inverse）
                                           이며 아래의 식과 같
이 정의된다．


                       J+ =JT(JJT)_l                      (4.14)


 그리고, 식
      （4.13）
           에서 K는 임의의 벡터이다. 식
                           （4.13）
                                에서 (I- J+ J)K값은 로봇 팔의 내부
운동
 （internal motion）
                 을 설명해 주는 항목이다. 즉, 로봇 팔의 끝점이 고정되어 있다 하더
라도 여유자유도를 갖는 로봇 팔은 무수히 많은자세를 가지게 되는데, 바로 이 현상을 설
명해 주는 식이다. 식
           （4.13）
                의 내부운동 중에서 로봇 팔이 원하는 성능함수
                                        （performa끄Ce
criterion）
         를 최대화 시켜 주도록 벡터 K의 값을 결정하여야 한다. 성능함수를 P(0）
                                                  라고 했



                                     4 장 퍼지 제어시스템의 응용사례 -149


===== PAGE 150 =====
을 때，
   P(0）
      를 최대화하기 위한 벡터 K의 관계는 식
                           （4.15）
                                와 같이 구해진다．


                                       .    0P.
                                       It = -=-K
                                             aα                                   (4.15)


 삭'(4."15\에서' 쁘ㅢ쁘 ,' oP- ,'...,'쁘ㅢ' 그리'고k는임의'의' 양의' 상수이'다."따ㄽ서'.'
  " " ." ' " ' o0   [ o0l ,' 002 ,'   ,' aGn j - ' - "∼ I_ -   I   P   P I - I." --U ". '
식
（4.15）
     의 관계가 유지되게 하는 내부운동
                      （internal motion）
                                      은 항상 P(0）
                                              를 증가시키는
방향으로 움직인다는 것을 의미한다．
 로봇 팔이 이동 중에 발생될 수 있는 장애물에 충돌하지 않고 안전하게 우회하여 목
적지에 도달하는 것이 중요한 요소이므로, 장애물이 존재하고 로봇 팔의 끝점의 위치
가 결정된 경우에 로봇 팔의 각각의 링크
                     （link）
                          가〔그림 4.54］
                                   에서 보는 바와 같이 장애
물로부터 가능한 멀리 떨어져 있는 자세를 취하도록 성능함수를 설정하였다．


                    V


                          (O, 0)




                        ［그림 4.54] 성능함수
                                     （Performance Criterion)


 따라서，  （performance criterion) 식은 식
    성능함수                          （4.16）
                                       과 같이 구성이 된다．


                               P (0) = ljph$ + 12。
                                                 k + 13毗                          (4.16)


 식
 （4.16）
      에서



150－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 151 =====
   1，毗 = V(11cos01 - O)2 + (11s1n81 - O)2

   '2。
     bs = \/(11cOs81+ l2cos(81+ 02) - O:)2 + (11sin01 +l2sin(81+ 82) - O)2



   13b = /[OTcos01 + l2cos (81 + 82) + l3cos(81 +〃2 + 83) - O,)2


   [(11sin81+ l2sin(01+ 92) +l2cos(81+ 02+ 83)-Qy)2I                   (4.17)


그리고계 식들에서 ox, oy는 각각 장애물 중심의 x성분 및 y성분이다．


5) 경로제어 알고리즘




                                            Nㅇ



                           A曲iv玭e
                        FUZzy CO낚roller




                       「1cfli슷fp 48                  =0
                      九 “口 客 弓心 + dβ


                       Mve Er써 P여m .f
                        Robot One st畔）



                      Find OmiI,1秘 P《）
                                     suce
                        by "rn辦 Mmon




              NO


                    (:  :-
                             ．毓叩    >
              ［그림 4.55] 여유자유도 로봇의 경로제어 알고리즘



                                            4 장 퍼지 제어시스템의 응용사례－151


===== PAGE 152 =====
        는 여유자유도를 갖는 로봇 팔의 경로제어 알고리즘에 대한 제어흐름도
［그림 4.55］
           에서 로봇 팔이 계획된 경로를 따라 움직일 때 규정된 반경 이내에 장
이다.［그림 4.55］
애물이 감지되지 않으면 로봇 팔은 계획된 경로를 수정하지 않고 목표 위치에 도달하
게 되지만, 장애물이 감지되면 퍼지제어기                가 작동이 되어 계획된 경로
                     （fuzzy controller）
에서 방향 수정에 필요한 수정각 △0를 계산하게 된다. 따라서, 로봇 팔의 끝점의 진행
방향이 결정되며 이 방향으로 한 스텝만큼 움직이게 하는 정보를 주게 된다. 그러나，
로봇 팔의 끝점에서 여유자유도 로봇은 수많은 자세       가 존재하므로 주어진 목
                          （posture）
적에 맞는 성능함수                      를 최대화시키는 자세를 구하게 된다．
         （perfoniiance criterion）


 6) 실험장치의 구성


 실험에 사용된 주요 주변장치의 모델명과 사양은 다음의［표 4.9］
                                    와 같다．


                     ［표 4.이 주요 주변장치의 사양
                       제품명                          비고
    컴 퓨터             486DX2-50
                   NSK Direct-Drive         Max Torque: l6kgf-m
                     Motor 1010           Resolution : 38400c0unt/rev
                   NSK Direct-Drive          Max Torque: lkgf-m
     모터
                     Motor 0408           Resokition: 25600c0unt/rev
                 Harmonic Drive motor      Max Torque: 0.33kgf-m
                 HS-250-2-RH-14-6002      Resolution : 40000count/rev
                                              l6bit 5 cha기1el
   카운트 보드             자체 제작
                                             up/down Counter
                   Re섧 Time Device         ND Convert: 16 channel
                     ADA-2110              D/A Convert : 2 channel
    D/A 보드
                   Real flme Device
                                            D/A Convert : 4 channel
                       DA-720


 카운트 보드는 모터의 엔코드에서 입력되는 신호를 디지털 신호로 변환하여 컴퓨터
에 입력시키고, 컴퓨터는 입력된 정보를 이용하여 로봇의 현재 위치를 계산하여 원하
는 위치만큼 이동하라는 제어신호를 내보낸다. 이 디지털신호를 D/A 보드가 아날로그
신호로 변환하여 모터 드라이버에 보내어 로봇을 구동시키게 된다．


           （Matlab/Simulink를 중심으로）
152－퍼지신경망 제어


===== PAGE 153 =====
                                           ［그림 4.5이 제어기 사진


 7) 여유자유도 로봇의 장애물 우회


 3관절 로봇은 여유자유도를 가지기 때문에 내부운동의 최적화 과정이 필요하다. 실
험을 위하여 사용된 3관절 로봇 팔의 크기는 Ii = 60, 12= 40, 13 =25로 선정하였다. 시작
위치에서의 로봇 팔의 끝점의 좌표를 (cx, ey) =(113, 23）
                                      으로 목표 위치에서 로봇 팔의
끝점의 좌표를（ex, ey)=(50, 70）
                       으로 선정하였고, 장애물의 형상은 원의 형태로 가정하
였으며 장애물의 크기와 위치는 원의 반경과 중심의 위치로 표현하였다. 그리고 장애
물의 위치와 로봇팔의 끝점의 간격이 장애물 직경의 5배 이내로 가까워졌을 때 퍼지제
어기가 작동하여 로봇 팔의 끝점의 진행 방향을 수정하도록 하였고, 이때부터 퍼지제
어와 동시에 로봇 팔의 최적화 자세를 찾는 과정을 수행하였다.


                                                             珊oh m8flip4il8tor Co幷OJOS 80이d
                  3nk manipu'ator co{bsion avoid
       1驪）




        50




         0




        -50
                 0             50             400            0            50             100
                               x                                          X

               3관철 로봇의 장애물 우회                            3관절 로봇의 장애물 우회
                bs, Y。
              (x。         出) = (75, 45, 5)
                     bs, r。                                      bs, rObS)=(80, 50, 8)
                                                         (xObs, Y。




                                                        4 장 퍼지 제어시스템의 응용사례 153


===== PAGE 154 =====
                    31nk manipulator c혀i1sion avoid         3bnk manipuIaor co隘on woid

         100

         80

         60

       ＞쑤 40

         20

          o




                                                        0      20   40       60
                                  x                                      X
               3관철 로봇의 장애물 우회                         3관철 로봇의 장애물 우회
                (xObS, y0bs, r0出)=(55,60,5)           ( <。bs, Y。
                                                               bs, r。
                                                                    bs)=(65,65,6)
                          ㅁ림 4-5기 3관절 로봇의 장애물 우회 모의 실험




                             ［그림 4.58] 3관절 로봇의 장애물 우회 실험


［그림 4.57］
        은 3관절 로봇의 장애물 우회 모의 실험이다. 그림에서 보듯이 장애물의
위치와 크기에 관계없이 장애물을 성공적으로 우회하여 목표 위치에 도달하였다. 그
리고 장애물이 목표 위치 가까이 있을 경우에는 두 번째 링크가 장애물에서 가능한 한



           （Matlab/Simulink를 중심으로）
154－퍼지신경망 제어


===== PAGE 155 =====
멀어지려는 것을 볼 수 있다. 그러나 실제 실험에 적용한 결과 최적자세를 찾는 과정에
서 많은 시간이 소모되어 실시간적으로 제어가 되지 않았다. 그래서 최적화 과정을 생
략하고, 대신 3관절과 x축이 이루는 각도 纖를 초기궤적에 수직
                                  （본 실험에서 熒=50로
하였다．
   ）하게 하여 장애물 우회실험을 실시하였다．
［그림 4.58］
        은 장애물의 중심과 반경이 (80, 50, 6）
                                 이고, =50인 경우의 실험 결과이다．
모의 실험과 마찬가지로 장애물을 성공적으로 우회함을 알 수 있다.［그림 4.59］
                                            는 장애
물이 없는 경우와 있는 경우에 각 관절에서의 궤적을 나타낸 것이다．

                                                                                                       m
               洲*11W뺘*1出
                       《rc哺1鱗 n aod                                  一                                 洲
                                     臘                           忍       H
                                                                             一
                                                                                                                           ;；약＼ ,
                                                                                                           衿




                                                                                                               ㅑ；홀汁小111,
                                                                             …
                                                                                               /^                                   UU “,




                                               "/
                                               1
                                                                                 的
                                         1e1

                                     r



                                                                                 的
                                     -
                                     1




       2   쎄      8   8         1.                  '4       恪                   200           4                           恪
                          T,m

                                                             繃11ta甘聊」
                                                                    1幽yc件,ion的d




                                                    2    4       6   B      札1       12   14       "
                                                                         鞠l片


                 ［그림 4.5이 3관절 로봇의 초기궤적과 장애물 우회궤적




                                                                                          4 장 퍼지 제어시스템의 응용사례 155


===== PAGE 156 =====
5장        인.신경.(Artificial Neural Network)




]. 인공신경망의 개념

     인공신경망은 생체신경망의 신호전달체제를 모방한 수학적인 모델이라고 볼 수 있
다. 따라서 인공신경망을 본격적으로 공부하기 전에 생체신경망의 신호전달원리를 간
단히 알아보는 것이 필요하다．
               일반적으로 생체신경망은 복잡한 망
                                （network）
                                        으로 구성
되어 있다．
     망을 구성하는 기본물질은 뉴런
                    （neuron）
                           과 뉴런을 연결해주는 시냅스
                                         （synapse)
로 이루어져 있다．
         그리고 여러 개의 뉴런들이 모여서 한 개의 충
                                 （layer）
                                       을 구성하게 된
다. 참고로 인간의 뇌 속에는 약 1011개의 뉴런이 존재하며, 한 개의 뉴런은 何개의 주
변 뉴런과 연결관계를 맺고 있다고 한다. 생체신경망시스템은 요즈음의 고성능 컴퓨터
에 비해 다음과 같은 강점을 가지고 있다 : 1) 고성능의 병렬분산처리
                                      （parallel distributed
processing) 능력을 갖고 있다. 2) 새로운 정보를 학습할 수 있으며, 새로운 정보를 바탕
으로 유사한 문제를 해결할 수 있는 적응능력을 갖고 있다. 3) 하나의 구조로서 여러 가
지 기능을 수행할 수 있다．


     인공신경망은 형태적으로 보면 생체신경망의 요소를 그대로 가지고 있다. 인공신경
망의 구성요소는 다음과 같이 구분할 수 있다．




                                    （Artificial Neural Network) _ 157
                            5 장 인공신경망


===== PAGE 157 =====
 - 노드
    （Node) : 인공적인 뉴런을 말하며，선형 혹은 비선형적인 매핑
                                       （mapping）
                                               을 수행
 - 가중치
     （Network Weight) : 노드 사이에 놓이는 연결부분
 -층
  （Layer) : 여러 개의 노드로 이루어진 충


 지금부터는 인공신경망이라는 표현을 쓰지 않고 그냥 신경망으로 줄여서 표기하기
로 한다. 실제로 많은 서적에서 그냥 신경망으로 표현한다. 먼저 신경망의 핵심인 노드
의 수학적인 모델을 살펴보기로 하자．



                          Bias
               xi         cell
                                         체
                                                 o



                                                                      甘8口ㅇ
                                             -




         鷺즈＝


                    /      Computation
                                                     TransfOrmation
                         of the activah0n            ofthe activa沁n

                        口림 5.1] 노드
                                 （뉴런）
                                    의 수학적 모델


［그림 5.1］
       은 노드의 수학적 모델을 나타내고 있다. 그림에서 노드는 합산부｛summing
junction）
        와 활성함수를 합친 영역이라고 볼 수 있다.〔그림 5.1］
                                       에서 각각의 입력신호들
이 대응하는 가중치에 의해 곱해진 후 노드로 들어가는 것을 알 수 있다. 이값들은 노
드 내의 합산부에서 더해지게 된다. 그다음 합산된 값이 활성함수
                                  （activation function）
                                                      로
전달이 되며, 활성함수내에서 비선형 식에 의해서 새로운 값으로 처리되게 된다. 그리
고 노드의 출력값은 다른 충에 있는 노드의 입력값으로 사용되어진다.［그림 5.2］
                                            는이
러한 노드들이 모여서 충
            （layer）
                  를 구성하게 되며 이러한 층들이 모여서 신경망을 구축
하는 것을 보여주고 있다．
             ［그림 5.2］
                    에 보여진 신경망은 입력충과 2개의 은닉층
                                          （hidden
layer）
     과 1개의 출력층으로 구성되어 있음을 알 수 있다. 일반적으로 신경망의 은닉층
과 출력충에는 노드가 존재하며, 입력충에는 노드가 없다. 입력충은 단지 입력되는 신
호를 전달해 주는 층이므로 노드가 없다. 다시 말해 합산부와 활성함수가 없다.




158－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 158 =====
          Input                                    C) 2} Output
         -                                               +
          Pattern                                                pattern

                    Input layer   Hidden layer    Output layer

                          ［그림 5.끽 일반적인 다층구조의 신경망


 신경망의 특성을 알아보면 다음과 같다．
 ① 비선형 입출력 매핑능력을 갖는다．
                       , 그 시스템에 대한 입출력의 관계를 정
  복잡한 비선형시스템을 학습할 수 있으며，
   확하게 형성해 준다．
 ② 적응적인 학습능력이 있다．
   처음에는 입출력의 관계를 정확하게 매핑하지 못해도 점진적인 학습을 통해 복잡
  한 입출력관계를 적응적으로 형성해 준다．
 ③ 일반화능력                      을 갖고 있다．
       （generalization ability）
   일단 학습이 된 후에는 학습되지 않은 입력정보에도 정확한 출력값을 제공해 준다.


 이상과같이 신경망은 생체적인 신경망과 구조 및 특성면에서도 매우 유사하다고 볼
수 있다. 신경망에서 배우게 될 핵심적인 내용은 신경망을 어떻게 학습을 시켜느냐 하
는 부분이다. 그리고 시스템의 규명
                  （system identification）
                                        이나 비선형시스템의 제어에
어떻게 적용을 시키는가 하는 부분이 될 것이다．




           （Fvt.ilti-Layer feedforward Neural Networks)
2. 다층구조의 신경망


 앞의 서론부분에서 살펴본 바와 같이 다층구조의 신경망은 다음과 같이 3개의 충으
로 구분할 수 있다．
 - 입력충
     （叫)ut layer)
 - 출력충
     （output layer)


                                        5 장 인공신경망
                                                （Artificial Neural Network) _159


===== PAGE 159 =====
 - 은닉충
     （ hidden layer)


 입력층과 출력충은 각각 1개이나, 은닉층은 l개 이상을 사용하게 된다. 학습하고자
하는 시스템이 간단한 경우 은닉층은 1개로 충분하지만 시스템이 매우 복잡한 경우에
는 2개 혹은 3개의 은닉충을 사용하게 된다. 은닉층 내부에 있는 노드도 시스템의 복잡
도에 따라 노드의 개수를 증가시킬 필요가 있다.［그림 5.3］
                                 은 전형적인 다층구조의신
경망으로써 2개의 은닉충을 갖고 있다. 입력충에는N개의 입력이 연결되어 있고, 출력
층에는M개의 출력이 나오게 되어 있다．



                                       Output Layer




                                       Hidden Layers




                                       Input Layer



                       U1      Urn
                       ［그림 5.이 전형적인 다층구조 신경망



 앞에서도 잠깐 언급한 바와 같이 노드
                    （혹은 뉴런）
                          는 은닉충과 출력충에만 존재한다
고 하였다. 노드는 합산부와 활성함수를 갖고 있는 영역으로 생각할 수 있다.［그림 5.4]
는 노드의 내부구조와 노드의 입출력 신호를 표시한 그림이다．




            （MatIab/SimuInk를 중심으로）
160- 퍼지신경망 제어


===== PAGE 160 =====
                                v1          V2                 Vn
                    ［그림 5.4] 노드의 수학적 모델


［그림 5.4］
       에서 γ=[vj, V2, …, Vm］는 입력신호 벡터이고，
                                      ”戶［싸1, Wj, …, 助.]T는 입력신
호에 곱해지는 가중치벡터를 나타낸다．
                   참고로，
                      가중치벡터 내의 W12는 입력충의 2번째
입력과 바로 위 층의／번째 노드를 연결해 주는 부분의 가중치 값（입력을 곱하는 값）
                                             의
표현임을 이해하기 바란다．
             b1는／번째 노드에 붙어있는 일종의 상수값인데 보통 바이
어스라고 부른다. 이 바이어스의 목적은SJT에 변화를 주어서 출력값에 변화를 주기위
한 수단으로 사용하는데 보통 1의 값을 많이 사용한다. 합산부
                                 （＝로 표시된 부분）
                                           의출
력값은 다음식으로 표시된다．


                       n`                                  r
                  曷   i= I                  ＋이 = w γ＋b夕
                                                                               (5.1)


 합산부의 출력값은 활성함수의 비선형연산을 통해 노드를 출력하게 된다. 물론 이
출력값은 다음 충의 입력정보가 된다는 것을 기억하자. 활성함수로 사용되는 식은 여
러가지가 있는데 가장 많이 사용되는 식은 다음과 같은 시그모이드 함수이다．


                            .   /   ∼   ,        1
                        /(b’口 =                      -,.
                                            1+ e                                (5.2)


〔그림 5.5］
       는 시그모이드 함수의 입출력 특성을 나타내고 있다．
                                  Sj의 값이 양의 값으
로 증가하면 출력값은 1로 포화하게 되며, 음의 값으로 증가하면 출력값은 0으로 접근



                                                    （Artificial Neural Network) _161
                                            5 장 인공신경망


===== PAGE 161 =====
     Si의 값이 -1과 1사이에서 출력값의 변화가 가장 크다는 것을 알 수 있다．
하게 된다．                                         나
중에 신경망을 학습할 때 입력정보를 가능한 -1과 1사이의 값으로 재조정하는 이유도
이 함수와 연관이 있다고 보면 되겠다．



                                 f(S)




                                                5j
                -2    -1     0          1   2

                ［그림 5.이 시그모이드 할성함수의 입출력 특성




3, 신경망의 학습
         （training)

 신경망을 학습한다는 개념을 먼저 이해할 필요가 있다. 신경망에서 학습한다는 의미
는 어떤 시스템의 입출력관계를 정확하게 계산해 주는 매핑이 만들어 지도록 신경망 내
부의 가중치를 끊임없이 조정해 나가는 과정이라는 것을 알아야 한다. 아래［그림 5.6］
                                               은
주어진 실제 시스템의 입출력 관계를 정확하게 규명하기 위하여 신경망을 학습시키는
방법을 나타내고 있다. 입력벡터 U'를 실제시스템과 학습하고자 하는 신경망에 동시에
입력을가한다음각각의 출력값을 비교하면 오차값E(w）
                           가생성되며, 이 오차값을줄이
는 방향으로 신경망의 가중치를 주정하는 것이다. 오차값이 일정수준으로 감소하게 되
면 학습이 완료되었다고 할 수 있다. 가장 중요한 것은 이 때의 가중치를 잘 간직해야 하
며 더 이상 수정해서는 안된다.〔그림 5.6］과 같은 학습방법은 감독학습
                                       （supervised training)
이라고 한다. 마치 유능한감독이 있어서 실제시스템에 어떤 입력이 들어가면 어떤 출력
이 나온다는 것을 정확하게 아는 것이 가능할 때 이러한 감독학습이 가능하게 된다. 그러
나, 많은 경우 이러한 감독학습이 곤란하다. 많은 동적시스템의 경우 입력과 출력과의 관계
를 규명하기가 쉽지 않기 때문이다. 이러한 부분의 학습은 비감독학습
                                    （unsupervised training)
으로 신경망을 학습시켜야 하는데 나중에 알아보기로 하자．



           （Mafiab/Simu1irik를 중심으로）
162－퍼지신경망 제어


===== PAGE 162 =====
                      Actual System

                                                            (w)
                                               '
                 Artificiah Neural Network




              ［그림 5.6] 신경망을 학습시키는 방법


 이제 신경망의 학습이 어떻게 이루어지는지를 이해해 보도록 하자.［그림 5.7］
                                           과같
이 1개의 은닉충을 갖는 다충구조의 신경망을 고려해 보자．




                                             0utput Layer




                                             네dden Layers




                                             Input Layer

                     니             Urn

                ㅁ림 5.기 다층구조의 신경망


 아래［그림 5.8］
          은［그림 5.7］
                  의 신경망에서 출력충의／번째 노드와 은닉층의 i번째 노
드 사이의 연결을 나타낸 그림이다．




                                      （Artifi이싫 Neural Network) _163
                              5 장 인공신경망


===== PAGE 163 =====
    Output layer node
                        t,                      上卄）neuron


                             wL
                                       0,
                                            ,




   네dden layer node
                                                i-th neuron
                        b'


                                                              0=
                                                                             →，，이＝
                                                                        , . ‘，      ；三汀珥β
                                                                                      『이
                                                                                      i
                                  0,   On

                             ［그림 5.8] 출력층과 은닉층의 노드와 가중치관계



 출력충의／번째 노드의 실제값
               （원하는 목표값）
                       을yi라고 하면 출력층의／번째 노드의
오차값은 다음 식과 같이 정의된다．


                                        百                     이
                                                      尤
                                                  1
                                                                   U
                                                                   U           ㅡ
                                                                                ㅡ




                                                  可
                                                      一
                                                                                        (5.3)


  오차값과 가중치와의 상관관계를 다음과 같이 구분해서 알아보기로 한다．


 출력층의 노드에 연결된 가중치와 오차값의 관계］
 아래 식은 출력층의 노드에 연결된 가중치가 변할 때 오차값이 어떻게 변하는지를
정의하는 편미분식이다. 편미분의 chain rule을 이용하면 아래 식과 같다．


                                                茫         陌曷
                                                            a      叫叫
                                                                                        (5,4)


［그림 5.8］
       에서 출력층／번째 노드의 출력값은 다음과 같이 계산된다. 편미분에 대한
기초지식만 있으면 다음 식은 쉽게 이해가 될 것이다．




164－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 164 =====
                                                                                      e』8
                                      ,,1 → ， 90-
                        小
                                                                -          (-
                                                                                          8 ')2
                        o=
                                      1+ 8 。Sj
                                            e
                                                                (1+                   e
                                                                                               )
                                                                                                                (5.5)


                 aOi
                                  l+ e " "-     i=          1
                                                                      ,
                                                                                (1+                _   1.   )
                  a하              (He－力）
                                       2               (He－아）'                                 1+ e-



그리고，
   식    을 (2에 대하여 편미분을 하면 다음의 관계를 얻는다．
    （5.3）


                                            a万         /-
                                            :z-7;-= tU- y1)
                                            αuj       "  "                                                      (5.6)


 따라서，
    식    의 오른쪽 부분의 첫 번째 항은 다음과 같이 나타낼 수 있다．
     （5.4）


                       0E            aE aO1            .一                 . ,, . 』                 八．
                       5耳＝石可石可＝
                              （나－yjJLiil1- O3)                                                                  (5.7)



dj
      aa
       多라고정의하면
                             하－        쁩＝            이(1－이）
                                                          （끼－                             o)
                                                                                                                (5.8)



그리고
       aS.
                 ；이므로다음의식이성립한다·
       awi



                                     aS1             aE aS,
                                     a미I a5
                                       J石耳5功；
                                            aW = Ou                                                             (5.9)

［은닉층의 노드에 연결된 가중치와 오차값의 관계］
은닉충의 i번째 노드의 입력값인 q값의 변화에 대한 오차값의 변화는 다음과 같다．




                                                               （Artificial Neural Network) _165
                                                       5 장 인공신경망


===== PAGE 165 =====
                  쯔－= 寸h oE 0Sk 1
                  a0j              k=1" a5k 003 '


                                   k= 1
                                   客          ［oE               k 。Qjq=
                                                                   o              1WkqOq                  『bk]

                                       in' r a꾜
                                       V.                            1
                             -L
                              k=1L53WkjJ                                                                          (5.10)




                        하一               쁩一                          90
                                                                     0E 003                。5;
                              =-         k=               1
                                                              [8Sk
                                                                     Wkil이                       (1- q)

                              =-i;[-ow3]O3(i -q)
                               k=1
                              = ＞〕[8kWkl（乙(1크7p
                                       k= 1                                                                       (5.11)


 따라서, 은닉충 아래에 연결되어 있는 가중치의 변화에 대한 오차값의 변화는


                              A/;:                        ,j;;' oS.
                                                                                                                  (5.12)


 위에서 구한 결과식 들은 출력충 아래의 가중치에 대한 오차값의 변화, 그리고 은닉
충 아래의 가중치에 대한 오차값의 변화를 나타낸 식이다. 문제는 한 번 학습이 이루어
질 때 마다 오차값이 줄어드는 방향으로 학습이 이루어져야 할 것이다. 따라서, 최급강
 （steepest descent method）
하법                       를 사용해서 매 학습마다 오차값이 줄어들게 할 수 있다．
이렇게 해서 신경망을 학습하는 방법을 역전파학습
                         （back propagation training) 방법이라
고 한다. 최급강하를 이용한 역전파학습은 다음식으로 나타낼 수 있다.


                                                    n鉢.              :OE          (W
                   呱*       ,:
                        ra+ 1                                 ra                                 )
                                                                             。w
                                                                                                     w=     ,,,   (5.13)



            （Matlab/Simulink를 중심으로）
166- 퍼지신경망 제어


===== PAGE 166 =====
 위 식에서 가중치에 대한 오차값의 변화는다음과 같고


                    aE        aE OS1             , n
                   an; = o5; an弓즌 아Ui                               (5.14)


 아래와 같이 표현할 수 있다．




                          謐      ＝   하oi
                                                                    (5.15)


 위식    에서 우변의 하값은 신경망의 노드의 위치에 따라 다른 값을 가진다는 것
  （5.15）
을 앞에서 설명하였다．
           즉，노드가 출력충에 존재하는 경우는 하는 다음과 같다．


                    8= O (i- O3)(y3- O)                             (5.16)


 반면에，
    노드가 은닉충에 위치하는 경우 하는 다음 식으로 표현된다．


                                           '7z

                   d= q(1- q)k; k Wk2                               (5.17)


 식
 （5.13）
      과식     에 의해서 매 학습마다 오차값을 줄이기 위한 가중치의 변화량은
        （5.14）
다음의 식으로 나타낼 수 있다．


               △ 바i(era+ 1) = 71'5jOi + α△ 1蛛(era)                  (5.18)


 식    에서 11는 학습률을 나타내는 상수이다. 일반적으로 학습을 값이 적으면 신
 （5.18）
경망의 학습이 정밀하게 이루어지나 학습하는데 시간이 많이 걸린다는 단점이 있다．
반면에 학습을 값이 너무 크면 그 반대의 현상이 나타나게 된다. 보통의 경우 학습율은
o.5∼l.0 사이의 값을 많이 사용하는 편이다. 식
                            （5.18）
                                 의 오른쪽 항에 있는 α는 모멘텀 상
수라고 한다．이 항은 수학적으로 전개된 항이 아니라 임의로 붙인 항이다. 그 이유는




                                        （Artificial Neural Network) _ 167
                                5 장 인공신경망


===== PAGE 167 =====
최급강하법을 사용해서 오차값을 줄이는 경우 발생되는 문제점은 오차값이 지역 최소
점
（local minimum）
              에 빠져서 더 이상 오차값이 줄어들지 않게 되는데, 모멘텀 항을 추가
하게 되면 이러한 문제를 부분적으로 해결할 수가 있다. 아래 식
                                  （5.19）
                                       는 학습이 한차례
진행된 후에 새로 생성되는 가중치의 값을 나타내고 있다．


                  H'；（
                     눙《，
                       ,', = 1) = 吃∥
                                   ：*;．α）+ A 'i(ra+ 1)                  (5.19)


 아래 그림은 일반적인 적응제어기가 주어진 궤적을 추종하는 원리와 신경망이 주어
진 궤적을 학습하면서 점점 정확하게 궤적을 추종하는 원리를 비교한 그림이다. 적응
제어기는 시스템의 파라메터를 점점 추정해 내면서 궤적 추종오차를 줄이는 반면에，
신경망은 학습이 진행되면서 시스템의 패턴을 추정해 내면서 시스템을 정확하게 복사
해 낸다는 점이다．



   position                    position



                                                         Learning process



                         bme

              (a) 적응제어 과정                 (b) 신경망학습의과정
                 ［그림 5.9] 적응제어와 신경망학습과정의비교




4. 신경망 학습읔 위한 노하우

                       （적응적으로 변화）
 1) 학습속도를 증가하려면학습을 口를 가변        시켜야 한다．


 식
 （5.18）
      에서 학습을 I／는 고정된 상수값이다. 이런 경우 어느 시점에서는 학습이 잘
되며, 어떤 순간에는 지루하게 학습이 느린 경우가 발생한다. 이런 문제를 해결하고 학
습속도를 증가하기 위해서는 상황에 맞게 학습율을 변화시켜야 한다. 다음은 적절한




           （Matlab/Simulink를 중심으로）
168－퍼지신경망 제어


===== PAGE 168 =====
예를 보여준다．
 · 학습이 잘 되는 경우
             （즉，
               오차값이 빠르게 감소하는 경우）
                               , 현재의 77를 77=77*1.1로
  대치한다．
               （즉, 오차값이 천천히 감소하거나 혹은 오차값이 오히려 증
 · 학습이 잘 안 되는 경우
        , 현재의 77를 γ7=77*0.5로 대치한다．
  가하는 경우）
 · 가중치 값 W는 오차값이 감소하는 경우에만 갱신을 한다．


 2) 입력 데이터를 스케일링
               （scaling）
                       한다．


 식   와［그림 5.5〕에서 보는 바와 같이 노드에 들어가는 입력값이 필요이상으로 크
 （5.2）
면 출력값이 쉽게 포화되어 버린다. 다시 말하면, 입력값이 -1과 1범위를 벗어나는 값
의 경우는 다른 입력값이 들어가더라도 출력값이 같게되어 버린다는 점이다. 이런 문
제가 있으면 당연히 학습이 원활하게 이루어 질 수가 없을 것이다. 따라서, 입력데이터
는 일반적으로 -1과 1사이의 값으로 스케일링을 하게 되면 학습효율이 높아지게 된다．
마찬가지로 학습을 시킬 대상의 목표        도 스케일링을 하는 것이 효과
                  （이상적인 출력값）
적이다.


 3) 가중치 값의 초기화


 신경망을 학습하기 위해서는 가중치의 초기값을 설정해 주어야 하는데, 초기값을
어떻게 설정하느냐에 따라 학습성능에 많은 차이가 난다. 많은 사람들이 초기값을 편
의 상 0 혹은 어떤 상수로 같은 값을 주는 경우가 있는데 이것은 바람직하지 않다. 초기
값은 활성함수를 포화시키지 않도록 작고 불규칙적인 값으로 주는 것이 효과적이다．
다음의 예를 참고하기 바란다．


              W= 0.5 *ralldomnmber (0∼1사이의 난수）




                                    （Artificial Neural Network) - 169
                            5 장 인공신경망


===== PAGE 169 =====
 4) 신경망이 학습이 잘 되지 않는 또 다른 이유


 ① 오차값이 지역최소점에서 빠져 나오지 않은 경우
 지역최소점이 매우 깊은 경우에는 모멘텀을 적용하더라도 지역최소점을 벗어나지
못하는 경우가 있다. 이런 경우처음부터 새로 학습을 진행하는 것이 바람직하다．
 ② 입력과 원하는 출력에 대한 샘플 수（종종 패턴 수라고도 함）
                                   가 시스템을 표현하
기에 너무 적은 경우에 학습결과가 충분하지 않을 수 있다. 이런 경우 학습을 위한 충
분한 입출력 정보를 더 보강해야 한다．
 ③ 신경망의 은닉충의 노드 수가 너무 적은 경우 학습이 좋지 못하다. 또한 시스템이
아주 복잡한 경우에는 은닉충의 개수를 증가하는 것이 더 효율적일 수 있다．




           （Matlab/Simulink를 중심으로）
170－퍼지신경망 제어


===== PAGE 170 =====
6장                  신경망의：:：래밍




 1. Matlab올 이용한 신경망의 학습

      앞 절에서 전개된 신경망의 이론식들과 알고리즘이 실제로 어떻게 구현되는 지를
이해하기 위하여 아래 예제와 같이 덧셈을 학습하는 신경망을 살펴보도록 하자．



     예 제 6.1 신경망을 이용하여 다음의 데이터를 학습시키는 Matlab 프로그램을 작성해 보기

로 하자．
      0.1 0.1 0.2
      0.1 0.2 0.3
      0.1 0.3 0.4
      0.2 0.1 0.3
      0.2 0.2 0.4
      0.2 0.3 0.5
      0.3 0.1 0.4
      0.3 0.2 0.5
      0.3 0.3 0.6



                                        6 장 신경망의 프로그래밍 -171


===== PAGE 171 =====
  위 자료는2개의 입력과 한 개의 출력을 가지는9개의 덧셈 데이터이다. 이 데이터를
저장하고 있는 파일을 npatl.dat 라고 하자. 다음은 Matlab 프로그램 전문이다. 이 예에
서는 은닉충과 출력충의 뉴런에 sigmoid 활성함수를 사용하였다. 학습률은 0.1을 사용
하였고 모멘텀율은 0.7을 사용하였다．


凶인 프로그램 ; train_run-nn.m 파알


function lrain_run_nn(inputl, input2)
ita = 0.1, alpha = 0.7, eref= 0.1;
%% npatl.dat 파일 Load
loadnpatl.dat
%% npatl.dat 파일에 있는 9개의 학습 패턴의 수
p_num =9;
m= npatl ;
iteration =0;
L= 3 ; %% 신경층의 수（입력충 : L=1, 출력층 : L=3)
n(1)=2;%% 입력충의 입력 수
n(2)=16;%% 은닉층의 뉴런의 개수
n(3) = 1; %% 출력충의 뉴런의 개수
o(1, n(1)+1) = 1; %% 은닉충의 모든 뉴런에 들어가는 바이어스 입력값
o(2, n(2)+1) = 1; %% 출력충의 뉴런에 들어가는 바이어스 입력값
train nn;%% 신경망 학습 서브루틴
%% 학습이 끝난 후 가중치를 저장하는 부분
save weights.matw
%% 학습이 종료된 후 신경망을 테스트하는 부분
o(1, 1) = inputi;
o(1,2) =input2;
run nn; %% 신경망을 작동시킴
output%% 신경망의 출력값



172－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 172 =====
［신경망을학습하는부분 : train_nn.m 파일］


%% 신경망을 학습시키는 루틴：train nn.m 파일
%% 가중치의 초기값을 설정함. 각 가중치의 값이 불 子칙적으로 다르면 좋음
forl=L: -1 :2
forj= 1:n(1)
fori= 1 :n(l-1)+1

w(j, 1,1) = (-1)t'j/n(l); %% 가중치를 3차원 배열로 구성하였음
dw(j,I,1) =0 ;
end
end
end
iteration =0;
while iteration <20000
e8um= 0. ;

for p = 1:p_nuin
%%npatl.dat의 데이터를 신경망의 입력으로 사용
0(1, 1)=in(p, 1) ;
o(1, 2)=in(p, 2);

y(p) = in(p, 3);
for 1= 2 : L %%1=2는 은닉충, l=L= 3은 출력충을 의미함
%% Sum over the nodes in the previous layer
forj= l :n(1)
s(l, j) = 0 ;
fori=1:n(l-1)+1
s(1, j) = s(1,j)+w(j,I,1)*o(l_1, i) ;
end
%% A sigmoid activation function is used
o(l, j) = lI(l+exp(-s(l, j))) ;




                                              6 장 신경망의 프로그래밍 -173


===== PAGE 173 =====
end
end

ye(p)=o(L,1);%% 신경망의 출력값
e(p) = sqrt((y(p)-ye(p))*(y(p) ye(p))) ; %% 학습오차값
%% 역전파 학습알고리즘 부분
forl = L:-l:2
%% Step through the nodes on layer 1
forj = 1:n(l)
dd(l,j) = 0;
%% If we are operating on the output layer
if(1= =L)
dd(L,j) = o(L,j)*(1_o(L,j))*(y(p)_o(L,j));
eI8e
fork= 1:n(l+ l)
dd(l,j) = dd(l,j)+dd(l+l,k)*w(k,j,1+1) ;
end
dd(l,j) = o(1, j)*(1_o(l,j))*dd(l,j);
end
%% Update the wei帥ts
%% Step through weights connected to nodej, layer I
fori=1:n(l-1)+1
dw(j,I,1) = jta*dd(l,j)*o((l_l),1) + alpha*dw(j, i,I);

w(j,I,1) = w(j,I, 1) + dw(j,I,1);
end
end
end
end
for p = 1: pnum
esum = esum + e(p) ;




           （Matlab/Simulink를 중심으로）
174－퍼지신경망 제어


===== PAGE 174 =====
end
esum;
iteration = iteration + 1;
iteration esum = [iterationesum]
end
%% Print out the final weights
forl= L:-l :2
forj =l :n(l)
forl =l :n(l-l)+1

w(j,I,1);
end
end
end


［학습된 신경망을 테스트 하는 부분 : r un_nn.m 파일］



for 1=2 : L
%% Sum over the nodes in the previous layer
forj=1:n(l)

s(l, j) = 0 ;
forl = 1:n(l-1) + 1
s(l,j) = s(l,j) + w(j,I,l)*o(l_1, i) ;
end


%% A sigmoid activation function is used
o(1, j) = l/(l+exp(-s(l, j))) ㅍ
end
end
output= o(L, 1) ;




                                              6 장 신경망의 프로그래밍 175


===== PAGE 175 =====
 전체 프로그램을 시물레이션을 하기 위해 다음과 같이 Matlab 명령창에서 메인프로
그램을작동시킨다. 즉, 0.2와0.1의 덧셈 계산을 해 보자．
 >> train_run_n끄(0.2, 0.1)


 시물레이션 결과를 정리하면 다음과 같다．


 iteration esum =


  1.0e+004 *


  2.00000000000000 0.00000313192972


 학습을 20000번 수행한 결과 9개 학습데이터의학습오차의 합은 0.00000313192972 임
을 알 수 있다. 실제 0.2와 0.1의 합 계산결과는 다음과 같이 정확하게 계산되었다．


 output =


  0.29687874837237


 이 번에는 학습을 하기 위해 사용된 데이터가 아닌 임의의 입력값, 예를 들어 0.25+0.15
계산을 다음과 같이 수행해 보자．
 >> train_run_nn(0.25, 0.15)
 시물레이션 결과를 정리하면 다음과 같다．


 iteration esum =


  1.0e+004 *


  2.00000000000000 0.00000313192972




176－퍼지신경망 제어
           （Matlab/Simulink롤 중심으로）


===== PAGE 176 =====
 학습을 20000번 수행한 결과 9개 학습에이터의학습오차의 합은 0.00000313192972
임을 알 수 있다. 그리고, 실제 0.25와 0.15의합 계산결과는 다음과 같이 정확하게 계산
되었다．


 output =


  0.39746643360819


 아래 그림은 학습이 100 ）번 반복되는 동안 학습오차가 감소하는 정도를 나타낸 그래프
이다．




                EgL믄m。 드드홴U




                              3591。    ~    1     ~    1    `    i     .    1

                                      仇빼l   聊n   3X1   훠n   mn   聊n   700   m.
                                                       T1**범 te뀁寸h

                                 ［그림 6.1] 신경망의 학습에 따른 도짜값의 감소


예 제 6.2 이번에는 신경망에서 이미 학습을 완료하여 신경망의 가중치 정보를 가지고 있는

경우，가중치자료를 읽어서 신경망을 작동시키는 프로그램이다．


 function run_trained_nn(inputl, input2)
 L= 3 ;%% 신경층의 수
               （입력충 : L=1, 출력층 : L=3)
 n(1)=2;%% 입력층의 입력수
 n(2) =16; %% 은닉충의 뉴런의 개수


                                                                            6 장 신경망의 프로그래밍 177


===== PAGE 177 =====
  n(3)= 1;%% 출력충의 뉴런의 개수
  o(1, n(1)+l) = 1; 0/% 은닉층의 모든 뉴런에 들어가는 바이어스 입력값
  o(2, n(2)+1) = 1; %% 출력층의 뉴런에 들어가는 바이어스 입력값
  %% input values to neural net
  o(1, 1) =inputl ;

  o(1, 2) = input2;

  %% weights.mat 파일 Load
  loadweights.mat



  output



  Matlab 명령창에서 0.1+0.2 덧셈을 시물레이션한 결과는 다음과 같다．


  >>run trained nn(0.1, 0.2)



  output =



     0.2970



예 제 63 이 예는 예제1의 프로그램과 같은 구조이다, 단지 은닉층의 모든 뉴런에 sigmoid

활성함수를 사용하였고, 출력층의 뉴런에는 선형 활성함수를 사용한 것이 차이점이다. 일반적
으로 예제3의경우가 예제1의 경우보다 학습속도가 빠르다．


머인 프로그램：trainjun-nn2.m 파일］


%% This is a add program of two numbers between 0 and 1.
%% Linear activation functions are used at output layer,

%% while sigmoid activation functions are used at hidden layer.

%% First, train the neural network, then test the result.




            （Matlab/Sim미ink를 중심으로）
178- 퍼지신경망 제어


===== PAGE 178 =====
function train_run_nn2(inputl, input2)
ita= O.1,alpha= O.7,eref= O.1 ;

%% npatl.dat 파일 Load
loadnpatl.dat
%% npatl.dat 파일에 있는 9개의 학습 패턴의 수
p_num =9;
in = npatl;
iteration =0;
L= 3;%% 신경층의 수
             （입력충 : L=1, 출력충 : L=3)
n(D = 2 ; %% 입력충의 입력 수
n(2) =16; %% 은닉충의 뉴런의 개수
n(3) = 1; %% 출력충의 뉴런의 개수
o(1,n(1)+1)=1;%% 은닉충의 모든 뉴런에 들어가는 바이어스 입력값
o(2,n(2)+1)=1;%% 출력층의 뉴런에 들어가는 바이어스 입력값
train nn2; %% 신경망 학습 서브루틴
%% 학습이 끝난 후 가중치를 저장하는 부분
save weights2.matw
%% Now, Neural Network Was Successfully Trained !!!
%% 학습이 종료된 후 신경망을 테스트하는 부분
o(1, 1)=inputl;
o(1, 2)=mput2;
run nn2 ; %% 신경망을 작동 시킴
output%% 신경망의 출력값
plot(iteration_esum)


［신경망학습부분 : train_nn2.m 파일］


 %％신경망을 학습시키는 루틴：train nn2.m 파일
%％가중치의 초기값을 설정함. 각 가중치의 값이 불 子칙적으로 다르면 좋음




                                                      6 장 신경망의 프로그래밍 179


===== PAGE 179 =====
forl= L:-1 :2
forj= 1 :n(l)
for I = 1: n(1-1)+1
w(j, 1,1)=(-1)스i/n(1);
dw(j,I,1) =0;
end
end
end
iteration = 0;
while iteration <1000
esum =0. ; %%%%%%
for p = 1: p_num
%% npatl.dat의 데이터를 신경망의 입력으로 사용
o(1, 1)=in(p, 1);
o(1, 2)=in(p, 2);

y(p) = in(p, 3);
for 1= 2 :L
%% Sum over the nodes in the previous layer
forj=1:n(l)
s(lj)=0;
forl= 1 :n(1-1) +1
s(l,j) = s(l,j) + w(j, I,l)*o(1_1, I);
end
%% A sigmoid and linear activation functions are used
if(l==L)
o(1, j) = s(l,j);
else
o(1, j) = 1/(1+exp(-s(1,j)));
end




           （Matlab/Simulink를 중심으로）
180－퍼지신경망 제어


===== PAGE 180 =====
end
end
ye(p)=o(L, l);%% 신경망의 출력값
e(p) = sqrt((y(p)-ye(j))*(y(p)-ye(p))) ; %% 학습오차값
%% 역전파 학습알고리즘 부분
forl=L: -l :2
%% Step through the nodes on layer 1
forj=1:n(l)
dd(l,j) = 0;
%% If we are operating on the output layer
iql==L)
dd(L, j)=y(p) - o(Lj); %%%%%% forli끄ear activation function
else
fork= 1:n(l+ 1)
dd(l,j) =dd(1,j)+dd(l+ l,k)*w(k,j,1+ 1) ;
end
dd(l,j) = o(l,j)*(1_o(l,j))*dd(l,j);
end
%% Update the weights
%% Step through weights connected to node j, layer 1
fori=1:n(l- 1)+1
dw(j,I, 1) = jta*dd(l,j)*o((l_1),j) + alpha*dw(j,I, 1);
w(j,I, 1) = w(j,I,1) + dw(j,I,1);
end
end
end
end
forp= l :p_num
esum = esum + e(p) ;
end



                                                              6 장 신경망의 프로그래밍 181


===== PAGE 181 =====
esum ;
iteration = iteration + 1 ;
iteration esum(iteration)= esum;
end



딱습된신경망을실행하는부분 : run_nn2.m 파옅引



%% 신경망을 작동시키는 함수 : run nn2.m 파일


for 1= 2 : L
%% Sum over the nodes in the previous layer
forj=1:n(1)
s(l, j) = 0 ;
fori=1:n(1-1) +1
s(1,j) = s(1,j) + w(j,I, l)*o(1_1, i) ;
end
%% A sigmoid activation function is used at hidden layer
%% A linear activation function is used at output layer
igl==L)
0(1, j) = s(1, j) ;
else
o(1, j) = 1/(1+exp(-s(l, j))) ;
end
end
end
output= o(L, 1) ;


   전체 프로그램을 시물레이션을 하기 위해 다음과 같이 Matlab 명령창에서 메인프로
그램을 작동시킨다. 즉, 0.2와0.1의 덧셈 계산을 해 보자
   >> train_run_nn(0.1, 0.2)


           （Matlab/Simulink를 중심으로）
182－퍼지신경망 제어


===== PAGE 182 =====
 ou치put=
   0.2965


 아래 그림은 학습이 반복되는 동안 학습오차가 감소하는 정도를 나타낸 그래프이다．
예제1의 그래프보다 학습오차가 빨리 줄어듬을 알 수 있다．


                          30



                          拓


                          m




            E
            ㄱ ·능느m口드드굔卜
                           ｀
                           나




                           。




                          5    卜




                          0                       ·－---

                           0       100   聊   聊   *ㄷ． 500 ".      100   吼n   吼． 1000
                                                  계h山계1目It日mb1


                           ［그림 6.2] 신경망의 학습에 따른 도짜값의 감소




2. MATLAB의 신경망 함수를 이용한 신경망의 학습

 신경망을 학습하기 위해서는 다음과 같이 4단계를 거친다．
   ① 학습할 데이터를 준비한다．
   ② 신경망의 구조를 생성한다．
   ③ 신경망을 학습시킨다．
   ④ 임의의 입력값을 이용하여 신경망을 동작시킨다．


 1) 신경망의 구조생성


 Feedforward 신경망을 구성하기 위해 다음과 같이 newif함수를 이용한다．



                                                                        6 장 신경망의 프로그래밍 - 183


===== PAGE 183 =====
 net = newfT(PR.[Si S2...SNI], {TFI TF2...TFN1}, BTF,BLF,PF)


 위 함수에서 PR은 입력에이터의 범위 즉 최소값 및 최대값을 나타낸다. Si 는 신경망
각충
 （layer）
       의 뉴런 수를 나타낸다. TFi는 각 충의 뉴런에서 사용된 전달함수
                                           （활성함수）
의 방식을 나타내며 TANSIG, LOGSIG, 그리고 PURELIN 함수를 주로 사용한다. BTF는
신경망의 역전파 학습방법을 말하며 TRAINLM, TRAINBFG, TRAINRP, TRA1NGD 등
의 함수가 있는데，
         별도 표시가 없으면 trainim 함수를 사용한다. BLF는 가중치
                                             （weight)
와 바이어스
     （bias) 학습함수인데 디폴트인 경우 leamgdm 함수를 사용한다. PF는 학습
오차의 성능함수를 말하는 데 디폴트인 경우 mse(mean-square-error）
                                             를 나타낸다．


0ㅖ 제 6.4 신경망을 이용하여 다음 값을 학습시키도록 해 보자. 입력값은 P이고 寒 값은T이다．


     P =[0 1234567 89 10];
     T = [0 123432 12 34];


 사용된 신경망의 구조는 2층의 구조이다. 즉, 은닉층 1개와 출력충 1개로 구성되어
있다．
  입력값의 범위는 [0..-..101. 은닉충의 각 뉴런은 TANSIG 활성함수를 사용하였고，
출력충의 뉴런은PURELJN 활성함수를 사용하였다. 은닉층의 뉴련 개수는 5개, 출력충
의 뉴런 개수는 1개이다．


                        net=newfI[0 101, [5 1], {'ta끄sig' 'purelin'});


  위 신경망을 50번 학습한 후에 입력값에 대한 학습된 출력값을 알아보자．


     net.trainParam.epochs = 50;
     net = train(net, P,1);
     Y = sim(net, P);
     plot(P, T,P, Y,'o')




184－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 184 =====
  아래 그림은 목표값
           （T）
             과 실제 출력값
                    （Y）
                      를 비교한 그래프이다．




               I s* pi的汕빙
                     ［그림 6.3] 목표값과 신경망의 출력값 비교


0打 제 6.5 신경망을 이용하여 노이즈가 포함된 sine 함수를 학습하는 ㅍ쿠ㄱ램을 작성해보

자. 사용된 함수는 t=sin(2*pi*p)+O.1*randn(size(p)) 이고 아래 그림은 2초간 수행된 함수의 그
래프이다．


                                          tsIi伊p·p)+O.I·i.Mii(s 톄p))




                            ..2    l`.4   0石   c*』    1    1.2   '.4   1.6   1』
                                                      l1

                                  ［그림 6.4] 신경망 학습용 파형


 위의파형을 신경망을 이용하여 학습을 해 보도록 하자. 아래 Matlab 프로그램은 Neural
network으로 위의 파형을 학습시키는 프로그램이다. 신경망은 2층 구조로 구성되어 있
으며 은닉층의 뉴런은 tansig 함수를 사용하였고，
                            출력층의 뉴런함수는 purelin을 사용
하였다. 이 방법이 일반적으로 학습성능이 좋다고 알려져 있다. 학습 수는 1300회를 수


                                                                             6 장 신경망의 프로그래밍 - 185


===== PAGE 185 =====
행하도록 하였다．


    %Taining data set
    p=[O: O.Ol :2];
    %noisy sine wave
    t = sin(2*pi*p)H0.1*randn(size(p));
    net = newfl([0 2], [20,1], {'tansig', 'purelin'}, 'traingdx');
    net.trainParam.show = 1300;
    net.trainParam.epochs = 1300;
    net = train(net, p, t);


 아래 명령어는 학습된 신경망에 입력값p를 주었을 때의 결과이며 결과값은y로 나
타내었고 원래파형과 비교하도록 하였다．


 y = sim(net, p)

 plot(p, t)

 hold on

 plot(p, y, 'r')



 아래 그림은 원래파형과 신경망의 출력값을 비교한 그림이다. 신경망의 출력이 원
래파형을 잘 추종하고 있음을 알 수 있다．




                                           \
                                           ㅈ    l




                              ·1.5
                                  .   .2   04       06   08   1   1그   1.4   1.6   1.6   2


                              ［그림 6.5] 원래파형과 신경망의 출력파형 비교


186－퍼지신경망 제어
           （Matlab/Simulink룰 중심으로）


===== PAGE 186 =====
3. MATLAB TOOLBOX를 이용한 신경망익 학습


 MATLAB에서도 신경망함수와 기본적인 프로그래밍방법을 이용해서 C 프로그램과
같은 방식으로 코드를 짤 수 있다. 하지만 TOOLBOX를 사용하면 신경망에 대한 깊은
이해 없이도 신경망의 형성, 학습 및 응용이 가능하다. 지금부터 MATLAB의 신경망
TOOLBOX를 사용해서 신경망을 형성하는 과정을 살펴보자．



단계1 MATLAB 창에서 입출력 데이터 형성 및 신경망의 구성
 다음과 같이 명령어를 입력한다．
 >>nntool
 그러면，
    다음과 같이 GUI(Graphic Userlnterface）
                                    화면이 나타나게 된다．




              i
              Input Delay S伯tea:




                  Netw.rk$ and Da伯

                                              -   Ne뉴，
                                                     Data   1   NewN.紬『니
                          Import     -   Ex
                                              port   -             -
                  Networks on盼




                                     「l림 6.6] GUI 화면


 이 화면을 이용하여 학습에 필요한 입출력 데이터를 등록하J긱 신경망의 구조를 설정할
수 있다. 그런 다음 학습을 하고 학습이 된 이후에 학습성능을 테스트할 수 있다. 이 예제
에서는 XOR(Exclusive OR) 논리를 신경망을 이용해서 학습시키고자 한다. XOR(Exclusive
OR) 논리는 다음과 같다. 아래 표에서 X, Y는 입력값이고 XOR은 출력값이다．




                                                                           6 장 신경망의 프로그래밍 -187


===== PAGE 187 =====
                       x       Y       XOR
                       0       0        0
                       0       j        1
                       1       0        1
                       1       1        0


 MATLAB에서 사용할 입력값과 출력값을 각각 p 와 T로 놓으면 다음과 같이 표현될
수 있다．
 P=[O01 1; 0101]
 T = [0 110]


 입력값을［그림 6.6］의 화면에 등록해야 하는데［그림 6.6］
                                  에 있는 New Data를 클릭하
여 아래그림과 같이 변수와 데이터 값을 입력할 수 있다. 여기서 Data Type은 Inputs으로
선택한 후 Create 버튼을 누르면 화면 창에 등록이 된다. 같은 방법으로 출력값 T에 대한
변수 및 데이터를입력하고 Data Type은 Targets으로 선택하고 Create 버튼을 누른다．




                       ［그림 6.7] 데이터 입력화면



 위와 같이 데이터를 입력한 다음 신경망의 구조를 정해 주어야 한다.〔그림 6.6］
                                             의화
면에서 New Network을 클릭하면［그림 6.8］과 같이 창이 생성된다．




188          （Matlab/Simulink를 중심으로）
      퍼지신경망 제어


===== PAGE 188 =====
                  Network Name jXORNet


                   Network T1)                            forward bactiprop




                                                                                                        늬늬늬늬
                                                                                    =J
                                           이Feed-
                    hput ran.es:                                      (01:0tj       如St from np
                   了rain衲g 柚nctlon:
                   Maption learning function
                    Ped.rmanCe function:
                    Number oflayers:                             12
                     -Properties
                                                    for Layer2   =     J
                                   Number at neurons: 챵
                                   TransferFunction:卜ANSb8                                        -ii
                                   Vrkw      - Defaults -                       Cancel   -   Create        -
                                                    ［그림 6.8] 데이터 입력화면


 위 화면은 자동적으로 디폴트화면을 보여주는데, 사용목적에 맞게 내용을 수정할
수 있다. 신경망의 현재상태를 살펴보면 다음과 같다．


 신경망의 종류
       （Network Type) = Feed-forward Back-propagation
 입력값의 범위
       （Input Ranges) = [0 1; 0 1]
 학습함수(Train Function) = TRAINLM (Levenberg-Marquardt backpropagation 사*)
 적응학습함수
      （Adaption Learning Function) = LEARNGDM
             (LEARNGDM Gradient descentw/momentum weight/bias learning function)
 성능함수(Performance Function) = MSE (mean square error)
 층의 개수
     （Numbers ofLayer) = 2


 여기서 층의 개수가2개라는 것은 은닉충 1충과 출력층 1층으로 되어 있음을 의미한
다. 입력충은 층으로 고려하지 않음을 주의해야 한다．
 위의 창에서 Layer 2, number of neurons = 1,Transfer Function = TANSIG으로 설정되어
있다．
  이 의미는 출력층
          （Layer 2）
                  의 뉴런은 l개이며, 뉴런 내의 활성함수는 TANSIG 함
수라는 것을 의미한다．같은 방법으로 은닉충
                      （Layer）
                            에 대해서 numberof neurons =2,
Transfer Function = TANSIG을 선정해 보자．
 그런 다음 Create버튼을 눌러 신경망 구성을 완성할 수 있다．



                                                                                             6 장 신경망의 프로그래밍 - 189


===== PAGE 189 =====
匣프프j 신경망의 학습
 신경망인 XORNet을 클릭한 후 Train버튼을 클릭하면 다음과 같은 화면이 나타난다．


             U答 H손1"["` .Hm1Xi 】                                                                      月n口
              喚나 - 뇰m1口· ㅣ Smu纖                            k卞n t 4at ㅣ W·*伊寸，ㅣ

                !nm1mmoo                     T,um, Pmom*,u    ㅣ《〕P쵱．n섬Info -
               IoOloS                  而c- -- nm_om
               00.4                    aJCOOD3, mu. mo
               m1텨．
                  .m1                  卜n               11叱－11m.
                ＇'`J1m' 「
               nㅒ                                       出mW
               mm_丁mo                  Fi·   a」c        mne
               mu                      k` FU




                    ＇ ㅣ
                 ·｀，헤                        c8月a   t


                                                   ［그림 6.9] 신경망 학습용 화면


 그런 다음 Training Info에서 P를 Inputs 변수로, T를 Targets 변수로 입력한다．
 화면에서 TraimngParameters는 다음을 나타내고 있다．
 학습을 최대 1000번까지 수행하고, 학습오차는 0.000000000000001 이다．


 이제 Train Network버튼을 눌러 위에서 설정한 신경망을 학습시켜보자. 매 학습마다
학습오차가 줄어드는 것을 확인할 수 있다．


               ，二"1'^WJ mH}1 m시肌 H
              〔h i* Ym ]1빠뺑 工·*                     出*片 甘*

                              1寸                         Pe,lmmance 5637578.0치 GaOl s18.015




                  江농苗* 。
                       。 t,*늉뇨．
                                   寸



                                                    1
                               ，
                               뇨
                                   們                                ＼∼∼∼∼－-




                      "                       !00   200       혀10   400    51:刃 600   m   여）
                                                                                           0   엇珀   1口凹
                 SWTm'1' -                                            ! 000 0POCh0


                         ［그림 6.10] 신경망 학습에 따른 학습오차의 감소


190 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 190 =====
 Stop Training을 눌러 학습을 종료하면 신경망의 학습이 완료된다. 아래 그림과 같이
학습이 완료된 후 View 버튼을 눌러서 신경망의 구조를 볼 수 있다．


         -J Nm. o,k X(}R,iet                                             月n口
          stew   - lnt,aiize - Simulate - TealsㅣAdapt - Weights -




             Managerㅣ          Close   -
                                   ［그림 6.1끄 생성된 신경망의 구조


단계3 신경망의 시물레이션
 이제 신경망이 잘 학습이 되었는지 확인해 보도록 하자. 그렇게 하기 위해서는 테스
트 용으로 입력을 만들어야 하는데 테스트 용 입력을 S라고 놓고 입력의 성분을 벡터
[1; 0〕로 해서［그림 5.10］의 화면에 등록을 해야 한다. 그리고 이 값에 대한 신경망의 출
력값을0utputs이라고 한다. 시물레이션을 수행한 후Outputs 값을 확인하면 1이라는 값
을 확인할 수 있을 것이다. 즉, 학습이 정상적으로 이루어졌다는 것을 말해 준다.



꽤 제 6.6 신경망을 이용하여 임의의 위치에 있는 이동로봇이장애물과 충돌하지 않고 목표

지점을 찾아가도록 제어시스템을 완성하라．


 편의상공간의 영역은 가로 10 세로 10인 정사각형 공간으로 가정한다. 장애물은 (5, 5)
위치에 있고 장애물의 크기는 적절하게 구성한다. 목표위치는 (5, 10) 위치이다．




                                                                    6 장 신경망의 프로그래밍 191


===== PAGE 191 =====
                                               （〕
                                               G 히 = (5,10)
                      10




                      Y                   qF




                                   Z?
                           0               x                  m

                     ［그림 6.1끽 이동로봇과 장애물 위치



  이 문제를 신경망을 이용하여 접근하려면 먼저 적절한 입출력 데이터를 정의하여야
할 것이다．
     이 예에서는2개의 입력값은 이동영역 내의 x 및 Y 위치인 (Xk, Yk）
                                             로 정하고
출력값은 이동로봇이 주행해야 할 방향 0로 정하였다. 이동로봇의 주행속도는 일정하
다고가정하였고, 1샘플링 스텝동안 움직이는 거리를상수S로 정하였다. 그러면, 이동
로봇이 움직이는 다음 위치에 대한 식은 아래와 같다．


                               Xk+ 1=   Xk+ S '    sinO
                               d／肝 l = Yk 十 S · cosri



  이제 신경망에 학습을 하기 위하여 입력값과 출력
                           （타겟）
                              값 사이의 매핑관계를 설명
하는 학습데이터를 생성해야 한다. 아래와 같이 MATLAB 프로그램을 이용하여 학습
데이터를 생성하였다. 일부 데이터는 for 문을 이용하여 자동으로 생성하였고, 일부 데
이터는 프로그램 중에 직접 입력하였다．


 x=0: 1: 10;
 y= O: l : lO;
  xgoal= 5;
  ygoal = 10;
  fori = 1: 1: 11
      forj=1:1: 11



192   퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 192 =====
      theta(i,j)= 180/pi*atan((x_goal_(i_1))/(y_goal_(j_1)));
 end
end
theta(6, 11)= 0;
theta(6,3)= -45;
theta(6,4)= -60;
theta(6, 5)= -80;
theta(7, 1)=0;
theta(7,2)=5;
theta(7,3)= 10;
theta(7,4)= 15;
theta(7,5)= 20;
theta(7,6)= 15;
theta(5, 1)=0;
theta(5,2)=-5;
theta(5,3)= -10;
theta(5,4)= -15;
theta(5,5)= -20;
theta(5,6)= -15;


아래 코드는 이동영역 중간에 위치한 장애물을 그리는 내용이고，
n =0: 0.01 : 2*pi;
for I = 1: length(n)
   obs_x(i) = 544J.5*sjfl(n(j));
   obsy(i) = 5+0.5*cos(n(i));
end
plot(obs_x, obsy, 'r')
hold on




                                                                6 장 신경망의 프로그래밍 193


===== PAGE 193 =====
 아래 코드는 임의의 위치와 그 위치에서의 주행방향을 나타낸 그림이다．


 fori= 1: 11
   forj = 1: 11
        xvector(i, j) = sin(theta(i, j)*pill8o);
        y_vector(i, j) = cos(theta(i, j)*pill8o);
   end
 end
 y_vector(6, 6) = 0;
 quiver(x, y, x_vector', y_vector', 0.8, 'b');
 hold off
 grid
 axis([0 10 0 10]);
 %%%%%%%%%%%%%%%%%%

 xy= [];
 fod = 0:10
   fori= 0:10
  x(i+1) = i;

  y(i+l) = 11-i;
   xy = [xy;j ill;
   end
 end


 아래 코드는 입출력 데이터를 都干화
                   （Normalization) 하는 과정이다. 보통 데이터의
크기가 1보다 큰 경우 데이터를 1이하로 스케일 다운
                            （scale-down) 을 하는데 그 이유는
뉴런 내부의 활성함수가 l 이하의 값에 대해 학습효율을 높여주기 때문이다. 스케일
다운
 （scale-down) 된 값은 나중에 원래 값으로 환산하면 되기 때문에 문제가 없다．


 xy = xy'Il0
 theta = theta';



            （Matlab/Simulink를 중심으로）
194- 퍼지신경망 제어


===== PAGE 194 =====
theta_target = theta(1:121)/90




                                                                    …
                                                                    …쏘옴
                                                                      n
아래 그림은 신경망을 학습하기 위한 학습데이터를 그림으로 보여주고 있다．


                                                                          ,1




                                       ；万以彦含…∥亡
                                              7〃久万                                                   니NNN＼久N入入＼



                                                슛
                                                ： 口／Z냥쑈7締〃扮
                                                          γf可計yγ＇
                                                                            \
                                                                            1




                          az//>//／…즈／／…스／                                                                     弧뇨＼섰섰入뇨＼…入入k
                                                                                                m
                                                                                                ㄴ，
                                                                            *치m니섶시뇨漱＼꼬
                                                                                     뇨빻T
                                                                                       닌V,


                                                                                              ｀
                                                                                              눙
                                                                                              “

                                       쟈낚Zz7…之泛기次／                                                   NNXN수A\＼ㅈㅈ
                                                                                          h
                                                                                          和
                                                                                          M,
                                                                                           "知
                                                                                             叫
                                                                                             ｀
                      1


                                                                                                                  I0


                                     ［그림 6.13] 신경망 학습용 데이터




                                                                                     Lay8r DelsyStisi:




                                                                N帥Data…   NeW N帥rmrI( '




                                            ［그림 6.1따 신경망 구성화면


신경망의 학습은 MATLAB에서 제공하는 Toolbox 인 nntool을 이용하였다. 입력데이



                                                                                                         6 장 신경망의 프로그래밍 - 195


===== PAGE 195 =====
터 xy와 타겟데이터 theta_target를 n끄tool 의 화면으로 import하여 신경망을 구축하였다．
신경망의구성은 은닉층에 50개의 뉴런을 설정하였고 뉴런의 활성함수는 tansig를 선정
하였다．
   출력충은pureli끄의 활성함수를 갖는 1개의 뉴런을 설정하였다. 이 신경망의 이
름은 networki이다．
 학습을 완료한 후에 신경망 networki을 Matlab 명령창으로 export를 한 다음 다음과
같은 명령을 수행해 보자．


 v= 0.01;
 for i = 1: 11
   forj = 1: 11
     xO= i-1;yo=j-1;
     x_in = x0/10 ; y_in=y0llO;
     dx= 0;
     dy =0;
     error= 1;
     x=    [];
     y= [1;
     whuleerror = = 1
          x_m = x_in + dx;
       y_in = y-in + dy;
       theta = sim(networkl, [x_in;y_in])*90*pill8o;
       dx = v*sin(theta);
       dy = v*cos(theta);
          x= x in*l0

       y =yin"lO;
       if((abs(x-5)<0.2)&&(abs(y-10)<0.2))
            error =0;
       end
       plot(x, y)



           （Matlab/Simulirik를 중심으로）
196－퍼지신경망 제어


===== PAGE 196 =====
         hold on
       end
   end
 end
 n= O: O.01 :2*pi;
 fon = 1 : length(n)
   obs_x(i) = 5+O.5*sjn(n(j));

   obsy(i) = 5+O.5*cos(n(j));
 end
 plot(obs_x, obsy,'r')
 gnd

 axis([0 10 010]);


 아래그림은 임의 시작위치에서 이동로봇이 출발하였을 때 각 로봇이 생성되는 궤적
을 그린 그림이다．




                       ㅁ림 6.15] 각 출발위치에 따른 로봇의 이동경로




                                               6 장 신경망의 프로그래밍 - 197


===== PAGE 197 =====
7장신경.               제어기




        신경망은 동적시스템의 모델링이나 제어에 유용하게 이용되고 있다. 앞에서 많이
언급한 바와 같이 실제시스템과 신경망을 병렬로 연결하여 출력값의 오차를 줄이도록
신경망의 가중치를 조정함으로써 실제시스템의 동적모델을 알아 낼 수 있다. 또한 이
렇게 구한 동적모델은 제어기의 한 부분으로 포함되기도 한다. 따라서, 신경망을 이용
하여 제어기를 구성하는 경우, 대부분은 아래와 같이 2개의 단계를 가지게 된다 :


        단계1 : 신경망을 이용한 동적시스템의 모델링
        단계2 : 구해진 동적모델링을 이용한 제어기 설계




1. 신경망 학습의 종류

        본격적으로 신경망제어기를 공부하기 전에 학습의 종류와 각각의 차이점을 이해하
는 것이 중요하다．




                                      7 장 신경망 제어7「 199


===== PAGE 198 =====
 감독학습
    （supervisory Iraining）
                         과 비감독학습
                               （unsupervisory Iraining)
 보통의 학습방법인 감독학습인 경우에는 신경망의 입력과 출력의 관계가 주어진
다. 즉 신경망을 학습시키는 사람이 입력값과 대응하는 출력값을 알아서 준비를 해야；
한다. 예를 들어 간단한 덧셈을 학습시키는 경우에 2개의입력이 2와 3인 경우 대응하
는 출력이 5라는 정보를 제공해야 한다. 이러한 형태의 학습을 감독학습이라고 한다．
그러나, 대부분의 동적시스템에서는 실험을 하기 전에는 입력과 출력과의 관계를 알
기 어렵다. 즉, 어떤 모터터시스템에 어떤 토크입력을 주었을 때 축의 회전속도출력을
이론적인 식에 의해 정학하게 제시하기 어렵다. 물론 이런 경우 실험을 통해서 입력과
출력간의 관계를 알아낼 수 있지만 이런 경우 방대한 실험을 수행해야 할 것이다. 이와
같이 입력과 출력간의 관계를 알 수 없을 때 신경망을 학습하는 방법이 비감독학습인
것이다.


 0ff-line 학습과 On뻐line 학습
 동적시스템을 학습할 때 Off-line 학습은 플랜트의 특성을 실험을 통해서 입력과 출
력데이터를 구하고, 그 다음 이 데이터를 이용하여 신경망을 감독학습을 시키는 경우
를 말한다. 반면에 On-line 학습은 실제플랜트와 신경망을 병렬로 연결하고 플랜트를
구동함과 동시에 신경망을 학습하는 경우를 말한다. Off-line 학습의 경우 실험을 통해
서 입출력 데이터를 얻은 후에는 컴퓨터에서 쉽게 신경망을 학습할 수 있는 반면에
On-line 학습은 프랜트장비와 컴퓨터 등의 하드웨어를 현장에 설치해야 하므로 여러가
지 불편함이 따르게 된다. 하지만 실험과동시에 학습이 동시에 완성된다는 것이 장점
이라고 할 수 있다．




2. 신경망 역졔어기

 아래 그림과 같은 형태의 제어기를 신경망 역제어기라고 한다. 그 이유는 플랜트의
입력과 출력 관계가 신경망제어기에서는 정 반대로 구성되어 있기 때문이다. 따라서，
신경망이 정상적으로 학습이 된 경우 신경망 제어기에 원하는 입력을 주면 제어기의
출력값이 플랜트에 입력값으로 들어가서 플랜트는 원하는 입력과 같은 값을 출력하게



             （Matlab/Simulink를 중심으로）
200 - 퍼지신경망 제어


===== PAGE 199 =====
되므로 완벽한 개루프제어기가 구성되는 셈이다. 이러한 제어시스템은 매우 간단한
형태의 제어시스템이긴 하지만, 플랜트가 외란을 가지는 경우 정확성을 기대하기 힘
들고, 또한 전체시스템을 실 시간적으로 작동시켜 신경망을 학습하는 데에는 문제가
따른다. 잘 알고 있듯이 신경망제어기는 학습초기에는 엉터리 값을 생산하기 때문에
플랜트의 출력값이 매우 불안하게 된다. 이러한 문제점을 극복하기 위한 대표적인 예
를 다음 절에서 소개하고자 한다．




        Coniniand
        input




                    ［그림 7.1] 신경망 역제어기




3. Kawato의 신경망병렬제어기


 아래 그림은 신경망제어기와 안정제어기가 병렬구조를 이루고 있으며 2개의 제어기
합력값이 플랜트의 제어입력으로 사용되고 있다. 이러한 형태의 신경망제어기를Kawato
의 신경망 병렬제어기 라고 한다. 앞에서 언급하였듯이 신경망을 학습하는 초기에 신
경망이 불안정하게 되는데, 이 경우에는 신경망의 출력이 불안정하더라도 안정제어
기의 출력값이 불안정성을 어느 정도 극복하기 때문에 On-line 학습을 할 수 있다는 것
이 큰 장점이다．
 Kawato의 신경망 병렬제어기의 또 다른 장점은 신경망을 비감독학습으로 학습을 할
수 있다는 점이다．
         신경망제어기
              （Kff）
                  와 병렬로 설치되어 있는 안정제어기
                                    （Kfb）
                                        를 고전
적인 제어기인 PD제어기나 P11〕제어기로 구성한다. 그러면, 신경망을 학습하기 위한
입출력 데이터 없이 어떻게 비감독학습을 할 수 있을까？그 대답은 의외로 간단하다.
간단한 논리로 전체제어시스템이 좋은 성능을 줄 때는 당연히 피드백되는 오차값이
매우 적을 것이다. 이 오차값이 매우 적게 되면 PD제어기나 P11) 제어기의 출력값 역시
매우 적게 될 것이다. 따라서, 안정제어기의 출력값이 0에 가까운 값이 될 때 까지 신경
망을 학습하면서 가중치를 업데이터 하는 것이 Kawato 방식의 비감독학습 방법이다．



                                        7 장 신경망 제어기 201


===== PAGE 200 =====
                                                         9r




                  ［그림 7.2] Kawato 방식의 비감독 신경망 학습




4. 신경망을 이용한 기준모델 적옹졔어기

 신경망을 이용한 기준모델 적응제어기
                   （model reference adaptive control）
                                                    는 아래 그림
에서 보는 바와 같이 2개의 신경망으로 구성되어 있다. 즉, 플랜트를 모델링하기 위한
신경망과 기준모델을 추종하기 위한 제어용 신경망으로 구성되어 있다. 먼저, 플랜트
를 모델링하기 위한 신경망이 학습되어 진다. 그런 다음 기준모델을 이용하여 제어용
신경망을 학습하게 된다．



                            Reference
                   →
                                                                          v
                                                                          o
                            Model
                                                              Control
                                                              error

                                            →    Neu 1 net
                                                 Plant 1d이

                                                               Err。
                                                               Model
                                                                  r

                         Neufft:net
                   -
            Command __                            더ant
                         `-on,ruiier    Contr이                          더ant
            inpur
                                        Input                           Output


            ［그림 7.3] 신경망을 이용한 기준모델 적응제어 시스템 구조



 위 블록다이어그램을 조금 더 구체적으로 나타내면 아래 회로와 같다．




202- 퍼지신경망 제어
            （Matlab/Simulink를 중심으로）


===== PAGE 201 =====
           T
                       r1Nii                                                 (t)
                                       -* LW2
              m》
                                                                       re
                                  if                   머ant
                                                                             y(t)

                   D      Lw 4                                     (t) 4중
          +
                                                              ap
                                                                     14 m+



                                            닉   LW34



              ㅁ림 7.4] 기준모델 적응제어 시스템 내부 상세구조


 위 회로에서 플랜트 모델용 신경망과 제어용 신경망은 두 경우 모두 2개의 신경층을
가지고 있다. 제어용신경망의 입력데이터는다음과같다．
 · 지연된 기준입력
 · 지연된 제어용 신경망의 출력
 · 지연된 플랜트 출력


 플랜트 모델링 용 신경망의 입력데이터는 다음과 같다．
 · 지연된 기준입력
 · 지연된 플랜트 출력


 이해를 돕기 위하여 다음과 같은 로봇팔의 각도를 제어하는 적응제어시스템을 구성
해 보자．




                                 ㅁ림7.5] 1축 로봇팔 시스템


                                                                       7 장 신경망 제어기 -203


===== PAGE 202 =====
 로봇팔의 운동식은 다음과 같다．



                        d2th    一 . . ∼ (i6 .
                        ---:7=-1us1n《z)- 2 ---- mU
                         dth                (it


 여기서 쟌는 로봇팔의 각도이고 U는 DC 모터에 가해지는 토크이다．
 그리고, 제어용 신경망이 추종할 수 있는 기준 모델은 다음 식과 같다．


                         d2y- n            .dyr , n-
                         -=- -- -- 汐"(／·．- U --==-ㄱl- :J7'
                         dt    V'            αt


 즉, 제어용신경망은위의 궤적을 잘 추종할 수 있도록 학습되어져야 한다. 위 식에서
 은 기준모델의 출력이고, r은 입력신호이다．
y，
 MATLAB에서 제공하는 Simulink용 블록셋을 이용하여 위 예제를 풀어보자. 단계별
로설명하면 다음과 같다．



 l 단계1 Simulink Library Browser창의 Neuralnetwork 블록셋의 Conirol 부분에서 Model

reference control 블록을 드래그하여 창에 넣는다．
                                  X(2Y) 블록도 Control 부분에서 드래그
해 올 수 있다. 그 다음 로봇의 운동식을 이용하여 만들어진 Simulink 모델인 robotarm.mdl
은 아래와 같다．




               U                                s

                                           Integiator




                                 Gain

                                        10*srn(u(1))   4-
                                            Fcn

                          ［그림 7.6] 로봇팔의 모델


 위 로봇 모델의 subsystem을 만들어서 아래와 같이 제어기 우편에 연결한다．
                                             Subsystem


           （Matlab/Simulink를 중심으로）
204－퍼지신경망 제어


===== PAGE 203 =====
을 만드는 방법은 1장에서 설명하였다．


                       Mn.PeI F在＝1e.e＂ㄸ Co,,ImIUer




                                  Neu&        l
                                  NelWee    Q皿女QL
                                 （力nm〕 1휼er b！小la!




                                     '. t1
                                 1Ef 1


                        ［그림 7.7] 로봇 모델의 subsystem



 단계리Model Reference Control 블록을 더블클릭한다. 그러면, 아래와 같은 파라메터

입력창을 보여준다．


              Mfid이 Reference Cornror                                                ㅁ區凹
            F海    鱗ridbw 出Il}


                                Model Reference Contr이
                                          N甘뷔心rk *d맡出1'e
                     덟z. 01＋化en Laye                  No. r    eyed 肛brence 1 ,.i$

                                                       야bym山arcfrr Or샤ㅈ立S
                                                     ＇幻．

                                                          汁. 抉eyedPterd q쟈耳i$

                                                  Tr出*뿌Dl.
                 1눕麴111v,Ref甘히C8 V．
                                  終                    Cce*헤* Tr1**口柚 눕3

                 *m'mr＇勿
                       ＇··ce v出尉

             MacbaJa hle '님vme (aec)                          Re＇여히X:e -

              .*｀月nhi·V川v` e (Oec)

                 Ge
                  ＇볐d0 Tre. 口Dma                  tm'y갗1Dma
                                                                     [_     ㅌxFn1D섬a

                                             Tr1*. P a＇넜뺘＄

                 c口*m鮮 Tr.*口E刪냅                        C珊t
                                                        『合 Tr出*`$"1et1$

              ［크Uae OzradYlU,                         E UoeCcr,Ulire Tr*I,
             [ ned                                                   ㅣca馹 l
                         Redone pMa吐닙m*n.dbeebrore예．
                                                   **打*                      *[




           ㅁ림 7.8] Model Reference Controller의 파라메터 입력창




                                                                                       7 장 신경망 제어기 -205


===== PAGE 204 =====
 단계이 위 화면에 각 변수의 값을 입력한다. Network Architecture 부분에는Model Reference
Controller의 신경망 구조를 나타내고 있다. 은닉충의 노드 수는 13개, 기준입력 부분의
지연입력은2개, 제어기 출력부의 피드백 지연입력은 1개, 플랜트 출력값의 피드백 지
연입력은 2개로 입력하도록 한다. Training Data 창 부분에는 제어기용신경망의 학습에
필요한 학습 데이터 생성, 데이터의 개수를 설정하게 되었다. 그리고 기준모델
                                         （keference
     도 입력하게 되어 있다. 하지만, Model Reference Controller의 신경망을 학습하기
model）
전에 먼저 로봇 플랜트 자체에 대한 동적특성을 규명하기 위해 신경망을 학습해야 한
다. 따라서, 아래 부분에 있는 Plant Identification 버튼을 누른다. 그러면, 아래와 같은 창
이 열린다. 아래의 신경망은 플랜트의 특성을 복사  하는 모델이라고 할 수 있다．
                          （학습）
은닉층의 뉴런 개수는 10개이며 신경망의 입력으로 들어가는 데이터는 입력값, delay
된 입력값, 피드백된 출력값과delay 된 출력값이다. 가운데 부분은 학습을 위해 입출력
데이터의 최대값과 최소값의 범위를 보여주고 있고, 학습을 위해 최대 10000개의 학습
샘플을 사용 할 것이라고 되어 있다. 아래 부분에는 학습을 위해 필요한 반복학습회수
가 최대 300으로 설정되어 있다．




                Gene비e Tr*닙4 rVa              hn1；ㅉ鸞0緘a

                       --------         Tr*     P,rm닝的

                       Trm*也自目ct心 "     3oo    나          Tr         1r出m
               必u Cxret eit*s ,       El Use Ved的眈，
                                                  Dste         回Use TestVg D甘s
                   …   ,   =   …         '




                               ㅁ림 7.이 Plant Identification 창


  단겨i이신경망을 학습하기 위해서는 학습용 데이터가 필요하므로 Generate Training
Data를 누른다. 아래의 그래프는 임의의 데이터를 플랜트에 입력했을 때 대응하는 출


           （Matlab/Simulink를 중심으로）
206－퍼지신경망 제어


===== PAGE 205 =====
력값을 나타내고 있다. 학습용 샘플은 최대 10000개 까지 제시를 하겠지만, 학습 샘플
이 충분하다고 생각되면 중간에 중지를 할 수 있다．




                                                          F4*itt Input



                              m




                                                                       艮q.
                                        1O            겼）         王
                                                            hme (s)
                                                          PlutttOtmput




                                        to            才｝         '            4ㄷ｝          오
                                                            time (s)
                                                                *'-   ,' ‘柳“方m口t月甘．
                        i ＾隅계梓D川· ㅣ      Rutectoetu ]        「｀              m1佃m냅h,^
                                                              m1*^1.m4랐at m*哨．

                  ［그림 7.10] 신경망을 학습하기 위한 학습용 데이터의 추출


 l단계이Accept Data를 눌러 학습용 입출력 데이터를 확보한다. 그리고Plant Identification
창으로 돌아가서 Train Network 버튼을 누르면 학습이 진행되며, 학습이 끝난 후에 아
래 그림과 같이 학습성능을 보여준다．


                                                                   注*朔
       EiIe 三dt 닢ew ntd 工轍＄ r?otkl叩 坤ndtw 炒e1P                   〔기e `da yuw jnnui k01* Qluiuop 對ndow tluip

                                      ＂려朴 Oumut                                     11呼·           汁nt U뱀午며


                                                                         打｝




                                                                          0         S      10        5        쉈）

                                                                         4: 1α'     En"             HH 0mm

                                                                         3
                                                                         2


                                                      '
                                                                         0

                                        It1      才1                               5     10           5      m
                                         tune (이                                  tuna에              t甘m (t〕


                           ［그림 7.1기 학습이 끝난 후의 학습성능 평가



                                                                                                 7 장 신경망 제어기 207


===== PAGE 206 =====
 ，탄ji삐 OK button 버튼을 눌러서 신경망 플랜트 모델의 가중치 값을 Simulink model
에 저장한다．



 단계 기 이제는 신경망 Model Reference 제어기를 학습하는 단계이다. 이 경우는 플랜
트
（로봇팔）
    가 기준모델의 특성을 잘 추종하도록 플랜트의 앞에 위치한 신경망을 학습
하게 된다. 먼저, 제어기를 학습하기위한 기준모델은 정의해야 하는데, 아래와 같이 구
성될 수 있다. 기준모델은 안정된 시스템으로 선정하였다．




                                                                        cmm1
            ［그림 7.1끽 Mode' Reference 제어기를 위한 기준 모델 구성


 단계6이 끝난 후에 다시 Model Reference Control 창으로 돌아가서 제어기의 학습용
데이터를 만들기 위해 Generate Training Data 버튼을 누른다．


                   Made灌 Reference c0ntr《H

                File    對indo      Help


                                          Model Raference Control
                                                  ．甘w口* ^'C老ied｀
                                                               〃·
                                                   13                      ＇
                                                           卜終.DhyedRm甘ace놀卞냐     2




                                                    1ri**꿜r눋勉
                       油虹h얽月，
                            R螂ereflce V．
                                       綸           〕7        山* m甘T
                                                                  『**暳s*岬．
                                                                         b히 6
                                                                            （好〕

                       淪mnoR酊
                            ＇· t. y出月

                 닙咀h翩 놀엣甘V' v出終《no)

                 닉特*렇뉠』m*甘Y出 v*月(eec)

                       G,oe,mo T1000,0 D1o    J         勸P갓t D吐a
                                                                    l
                                                      「旨m넓-s
                                                  Tr**蜀

                       c이*
                         ＇啣 Tr* 낑탸loct好            1o      《dm'm芽Tn**珂s여F汕좋蠟 i

                       包La           超B*1ft
                                avei1，                     Duesceeteles Tl**5
                   뎌a색ctoc1七寸en       J                                 m




            （Matlab/Simulink를 중심으로）
208- 퍼지신경망 제어


===== PAGE 207 =====
 적절한 량의 학습데이터가 생성되면 중지를 하고 아래 그림과 같이 Accept Data 버튼
을 누른다．



                                              Reference Model Input


                    05

                     0

                    〕5

                     1L。
                                       10      20       ＇〕      카)          EO
                                                      tune《s)
                                              Reference Model Output
                     1

                  〔l5

                     0
                         /" " →｀
                                                                             \
                                                                             \
                   ·05

                                                        1          1


                                       10              丑〕         40        （〕
                                                                            5
                                                     tune (s)
                                                           Sined.tjolt Ott저；1ped t聊the "$1e'.
                l kcemD鱗自          -   Rejuse Date     mea1i亡 ^000r乂 1贓 Rerect 0mito c며  ＇맺1n나也



                         ［그림7.1이 기준모델의 입출력 특성


 단계 8 Model Reference Control 창의 Train Controller를 누른다. 여기서는 학습용 데이

터 샘플을 몇 구간으로 구분하여 학습을 진행하게 된다. 이 경우는 전체 학습데이터를
2구간으로 나누었고 각 구간의 반복학습회수를 10으로 설정하였다．
 아래의 그림은 학습이 완료된 후에 주어진 기준입력
                           （학습에 사용된）
                                   에 대해 기준모
델의 출력값과 신경망제어기에 의해 구동된 플랜트의 출력값을 비교한 그림이다．




                                                                                                  7 장 신경망 제어기 209


===== PAGE 208 =====
                      二결1.       Fㅂ汗       내 납r        1n.."    11,n1亡   n   d나＾〃， Ynnd^,1』 H이n



                                                               Referenc. Hodd h훨PUt


                             Os-
                                      醜－
                                                  (`     m
                                                                     f
                                 0-
                                 ［卜               1(r
                                                    烹      40   未） &L
                                                 time (s)            …      L
                        Reference Model Oumut (blu이， Neural Network Ou'ut (greenr\
                           1

                                                                                              ]\n      '



                                      。



                                      m
                                      b




                                                  10            20         3)       -40
                                                                         time(s)




            口림 7.1ㅔ신경망제어기에 의해 구동된 플랜트의 출력값 비교



 단계 이 이제 Simulink model의 Simulation 메뉴를 이용하여 학습에 사용되지 않은 임
의의 입력값에 대한 출력값을 비교할 수 있다. 플랜트의 출력이 기준모델의 출력을 잘
추종하고 있음을 확인할 수 있다．


                                                                         xY plm
                             1



                             5                                                                                  。




                뜨
                ，<>
                             0



                         的




                             ㅕ。                                                           」


                                              10                zI         30         *.          50       60
                                                                          XAxis

                  ［그림 7.15] 임의의 입력값에 대한 출력값 비교




             （Matlab/Simulink를 중심으로）
210 - 퍼지신경망 제어


===== PAGE 209 =====
            （NN Predictive Contr이）
5, 신경망 모델예측제어


 1) 예측제어


 예측제어기는 모델에서 앞으로 발생할 값을 예측하는 제어형태이다. 모델의 예측값
과 최적화함수 및 제어법칙을 이용하여 제어 예측값을 만들어 낸다. 이 시간구간에서
주어진 성능함수를 최소화하는 최적화과정에 의해서예측이 결정된다. 이 때 사용되는
성능함수는 아래 식과 같다．



                                                              m咫H   u+                   ~
                                                                                         1J   1l   u   1
                                                                                                       L       n
                                                                                                               乙
                                                                                                                   9
                                                                             上〃b
                                                                         ,
      /= ＞〕(y,(t+7)-y,, (t+7))2
                                                                                                           ~


                                                                     /,`
                                                                     ㅡ
                                                                                                           n       一
                                                                                                           〃
                                                                         /
         j =N




 위 식에서 N／과 N2는 추종오차와 관련된 시간범위를 표시하는 상수이고, Nu는 제어
입력값에 대한 시간영역을 표시하는 값이다.〃'는 신경망에 입력되는 잠정적인 제어입
력값이다. Yr은 추종목표값이고ym은 신경망모델의 출력값이다．


 이 제어문제의 목표는／값을 최소화하는 제어값을 찾는 것이다．


 제어값의 업데이트 :
 예측제어에서는7값을 최소화 할 수 있도록 제어값을 계속 업데이트해야 한다. 이때 일반
적으로 사용되는 방법이 gradient decent 방법이다．
                                 즉，주어진 함수의 음경사
                                             （negative gradient)
방향으로 움직이면 최소점
            （minimum point）
                          을 찾게 된다는 것이다. gradient decent 방법
은 다음과 같이 표현된다．



                                           1)
                                                                    ) au
                              u      (k+
                                                =   u
                                                                                   (k)
                                                        (k)
               상수，. aJ
 위 식에서   -y：
                   au
                        (k)
                              ：현재의
                                                제어입력에 대한／의 변화량을나타낸다· 미래
의 제어입력값은 다음과 같이 미래 제어입력벡터로 표현된다．



                                                                                                   7 장 신경망 제어기 -211


===== PAGE 210 =====
                          U(k)=[u(k+1)u(k+2). u(k+Nu)]


 위 식에서 목적함수／값의 U에 대한 1차 편미분식은 다음과 같다．


                aJ . 늬    aJ .    aJ .        .aJ .ㅣ
               oU(k) " aU(k+1) OU(k+ 2) " ' aU(k+ /V) "


 2) 신경망의 구성


 일반적으로 비선형 동적모델식은 다음식과 같이 입력과 출력의 과거 데이터에 의해
결정이 된다．


            y(k+l) = fly(k), y(k-l), ' " , y(k-n), u(k), u(k-1), '", u(k-m)]


 따라서, 동적식을 신경망으로 학습을 하려면 아래그림과 같이 TDNN(Time delay neural
network) 신경망을 사용하는 것이 한 방법이 될 수 있다．




           \    /
           Inputs           Layerl                  Layer2

                    ㅁ림 7.161 TDNN(Timedelay neural network) 신경망


 신경망 모델을 좀 더 자세히 들여다 보면 신경망의 입력부에 플랜트의 입력값과 프
랜트의 출력값이 들어가며 각각의 시간지연값도 들어감을 알 수 있다. 신경망의 출력
부를 눈여겨 볼 필요가 있다. 즉 신경망의 출력은 다음샘플링단계의 플랜트 출력값을
학습하도록 구성되어 있다. 즉, 예측제어기능을 갖도록 구성되어 있다. 신경망의 학습
에 필요한 학습에이터는 플랜트를 동작하여 얻은 결과치에서 추출하여야하며, 신경망
은 off-line에서 학습된다．



             （Matlab/Simulink를 중심으로）
212 - 퍼지신경망 제어


===== PAGE 211 =====
 TDNN 신경망 모델에서 출력값은


                                   오(k+ 1) = bs + Z卜 1w2(1, i).S(X1)


위 식에서


                                                                                 l
                                                                                 +
                                                                                                                                                m
                                                                                                                                                        씨          n                   u   k       H
      X = b(i,1)+ ＞〕w1(i,j).y(k- j +i) + ＞〕w1(i,n+ j ).u(k- j
                                                                                                                                                                                   ,
                                                                             ㅡ



                                                                                                                                                    키
                                                                                                                                                                                   '
                                                                                                                                                                                   h
                                                                                                                                                Z
                          j= 1




 3) 신경망 시스템의 미분식


일반적으로 제어법칙을 적용하려면 프로세서 입력에 대한 출력 미분값을 계산해야
한다．


                        aft(fr-.Li)
                        IJ.   y;
                                 "  =  IaLI           )
                                                                                                  [bs+                                N
                                                                                                                                      Z미            吼              ^
                                                                                                                                                                               X
                          。u' (       。u
                                                                                     (k)
                                                                                                                                                                   b
                                           (k)
                                                 kI
                                                                    -




위 식을 변형하면，


                                                                                     N
                                   oy(k+ 1)
                                                                                                               i                                              ] (7aX,1
                                                                                                                                          (X』
                                                                                                 w
                                                                                                 w2,          ,
                                                                                                                                                                                                       ㅡ




                                    au(k)
                                                                                                       (1
                                                                                                                                      '
                                                                                                                                .S,
                                                                                                                          ).S
                                                                                                       (i,        i)                      (X)
                                                                                 j   =     1                                                                      u나놔




위 식에서


                                                                                      ∼                       dS
                                                                                         b        =          ==-
                                                                                                             U,뇌



          .axi）
          au      (k)
                        乙，a
                                   u       (k)            b   (i,       1)   +             (au         (k)             {』客w1                            (i,     i ).y    (k-           j +i)   }

                                                                                                                                                                                   7 장 신경망 제어기 213


===== PAGE 212 =====
           l
           >                            n
                                        Z미
 '
 ,,



           ++                                                       1
 l
                                a         w       n     u
 `




                                                                i
                                                                    ,
                                                            샐




                          +
 -     -
 I
                                                            k
                                 .


                              出1(KJ
 ,                                                                  J
 l
 ,
                                                              은 과거의 값이므로 이 값
      위 식에서 y(k-l), y(k-2), …, y(k-n) 값과u(k-1),u(k-2),", u(k-m）
들은u(k）
     에 영향을 받지 않는다. 따라서,j=1인 경우 외에는 합계값이 0이다. 그러므로，


                                       OX1      ..     S
                                                      1J
                                      au(k) = w1(l, 盼


                      a (k+ 1)          NZ미   ㅡ
                                                  %
                                                  i).S'(Xi)].w1(i, n+1)
                       au(k)


      결국 위 식이 TDNN 신경망의 입출력 특징을 나타내는 식이다．


      4) 신경망 예측제어


      (1) 1-step 0ㅖ측 제어
      예측제어란 문자 그대로 시스템의 예측된 값을 이용하여 제어입력을 계산하는 방법
이다. 그러므로 적절한 신경망 모델을 선정하고 학습이 잘 된 경우라면, 신경망 모델은
실제 동적시스템의 동적특성을 잘 표현할 수 있다. 따라서, 기준입력과 예측값과의 오
차와 예측값을 이용하여 예측제어 알고리즘을 구성할 수 있다．


      아래 그림은 신경망 예측제어시스템을 설명하는 블록선도이다. 아래 그림에서 k : 샘플
링 시간，
    Kk) : 기준입력신호, u(k) : 플랜트에 들어가는 제어입력값, 姑）
                                           : 플랜트 출력값，
dk): dk）                          은 예측된 플랜트 출력값이다．
          의 차이값 즉 오차값을 말하며, 9(k+ l）
       와丸k）




214        퍼지신경망 제어
                  （Matlab/Simulink를 중심으로）


===== PAGE 213 =====
                                 ［그림 7.1기 신경망 모델 예측제어 시스템


 그림에서 알 수 있듯이 제어입력값은 실제 출력값을 사용하는게 아니라 예측값을
사용해서 계산한다는 점이다. 정의에 의해 예측제어기는 목적함수 J를 최소화하는 것
인데, 목적함수는 다음과 같이 오차값으로 구성될 수 있다．



                                                       J    =       -          -   e"           (k+         i)


 위 식에서


                                      e(k+ 1) =r(k+ 1)- 9(k+ 1)


 제어력을 업데이트하기 위하여 다음과 같이 gradient decent 방법을 사용한다．



                                                       1)
                                                                                                            ) au
                                                 (k+
                                           u
                                                                               u
                                                                =
                                                                                                                      (k)
                                                                                    (k)
 J 값과 e(k+1）
           를 이용하여


          aJ
         8u    (k)
                     )   =   1
                             2
                                 [-   2e
                                               (k+
                                                       1) 8
                                                       1)
                                                                        :(k+
                                                                               au
                                                                                          (k)         )1)   1:
                                                                                                            ]=_   -         0
                                                                                                                            e
                                                                                                                                『1) a
                                                                                                                                『
                                                                                                                                  1)
                                                                                                                                (k+
                                                                                                                                （
                                                                                                                                        夕
                                                                                                                                            (k+
                                                                                                                                                  (k)
                                                                                                                                                    )1)
 TDNN 신경망을 사용하므로




                                                                                                                                        7 장 신경망 제어기－215


===== PAGE 214 =====
                                          N
                  aJ           ,}n∼ㄴ 1 ,｀ㄱ, , , (1 ; , Q '(v \1,, , 1; .,j..i\
                au   (k)   -   ㄴ｀^   ' /iL. 1
                                           .4w 2 ' ' ' /'- ' 11 VV1 ',
                                                              jhi
 결론적으로 제어값
         （control law）
                     은


                                                      N
          u (k+ 1) = u(k) + y.e(k+ i)[＞〕W2 (1,i ).S'(X1)I.wi (i, n + 1)]
                                                 i=       1



 위 식들을 이용한 제어 알고리즘은 다음과 같다．


 ① 먼저 Y를 선정한다．
  （k+ 1 ）를 계산한다．
 ②夕
 ③e(k）
     를 계산한다．
 ④ 새로운 제어입력값 u(k+1）
                  을 계산한다．
 6) 새로운 제어입력값을 시스템에 입력한다．
 ⑥ 스텝 ②로 되돌아 간다．


 (2) T-step 0ㅖ측 제어
 앞의 1-step 예측제어 개념을 확장해서 구할 수 있다. 앞 절에서의 스칼라 값들이 다
음과 같이 예측 벡터들로 표현 될 수 있다．


                           R= [r(k+1),r(k+ 2), …,r(k+ T)]


                           Ye =[ST(k+ 1),9(k+ 2), ···, 夕(k+ T)]


                           U= [u(k),u(k+1), .",u(k+ T-1)]


 오차값은


                           E = [e(k+1),e(k+ 2), ".,e(k+ T)]




216 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 215 =====
 정의에 의해 예측제어기는 목적함수 J를 최소화하는 것인데, 목적함수는 다음과 같
이 오차값으로 구성될 수 있다．

                                              E
                                              E         ∼
               ㅡ

                                 J            12        n
                                                        l
 제어력을 업데이트하기 위하여 다음과 같이 gradient decent 방법을 사용한다．



                     U   (k+
                                1)   =    u
                                              (k)                (k)
                                                            aU
 여기서


                                aJ     一 aYe
                               oU(k) - ' oU(k)


                  aY .
 Jacobian matrix 。
                 U (k) 은다음과같" 나해진다·



                   o (k+ 1)
                                                    0
                    au(k)
                                                                             0
          aYe     （k+ 2)
                  畛                      a (k+ 2)                      ...   0
         aU (k) -  ou(k)                 ou(k+ 1)

                   a (k+ T)              a (k+ T)                        a9(k+ T)
                     au(k)               au(k+1) " '                   au(k+ T-1)


 위 식들을 이용한 제어 알고리즘은 다음과 같다．


 ① 먼저 v와I를 선정한다．
@)Y.와U(k）
        를 계산한다．
 ③ E를 계산한다．




                                                                             7 장 신경망 제어기 217


===== PAGE 216 =====
 ④   ,aYaU                (k
                               ）를계산한다．


                               ) 를계산한다·
                 aJ
     aU
 ⑤
                          (k
 ，→- . /. 』, ' , -. ,        oJ = -1 s, -.1 .1 _.1 - ^ .1 . 1 _.S1.__1 = _.1 .1 -, ,
 (D [T (k-l- 1) = 11(k) 7 . ,너,-, 를 이용ㅎI]서' 새로운 제，어,벡，터，를 계，                산한다．     "
 口   ∼       '        -        -   '   一   '   一   '        /   aU,   (K)   니   '   '-S




 ⑦ 새로운 제어값을 시스템의 입력으로 이용한다．
 垣）스텝 ②로 되돌아 간다．


 (3) MATLAB을 이용한 신경망 예측 제어기 설계
 신경망을 이용한 예측제어기는 플랜트의 성능예측을 위해 먼저 신경망을 이용하여
비선형 플랜트 시스템의 모델을 구한다. 그런 다음 신경망모델과 최적화 과정을 갖는
제어기
  （예측제어기）
        가 만들어 진다. 예측제어기는 다음 샘플링 구간（미래시간）
                                       에최
적의 플랜트 출력을 유도해 내도록 최적화 된 제어입력값을 만들어 낸다．
 예측제어기는 다음과 같은 2단계로 설계되어질 수 있다．


 「 단계기 신경망을 이용한 플랜트모델 생성
 신경망을 이용한 예측제어기 설계에 있어서 첫 단계는 플랜트의 동적모델을 나타내
는 신경망을 구성하여 학습하는 것이다. 이 과정은 아래 그림과 같이 이루어 진다. 그
림에서 보는 바와 같이 신경망에 입력되는 데이터는 플랜트의 입력값과 플랜트의 출
력값으로 구성됨을 알 수 있다. 물론 학습과정은 플랜트의 출력과 신경망의 출력의 오
차를 줄이도록 신경망의 가중치를 계속 업데이트하는 것이다．



                                                       z/




                                           ［그림 7.18] 플랜트의 동적모델을 위한 신경망 학습 과정



218- 퍼지신경망 제어
            （Matlab/Simulink를 중심으로）


===== PAGE 217 =====
                                                      -+ ym(t+1)



           Inputs        Layerl             Layer2
                       「그림 7.19] 신경망 모델의 내부구조


 단계리 신경망을 이용하여 예측성능을 높이기 위한 예측제어기 구성
 구축된 신경망모델은 미래의 특정한 시간구간에서의 플랜트 출력응답을 예측하게
된다．
 다음의 블록다이어그램은 모델예측제어시스템의 제어과정을 나타내고 있다. 제어
기는 신경망으로 학습된 플랜트모델과 최적화를 수행하는 블록으로 구성되어 있음을
알 수 있다. 여기서 최적화블록은 U'의 값 중에서 성능함수를 최소화 해 주는 U를 찾아
이 값을 플랜트로 입력하게 된다．




                    ［그림 7.20] 모델예측제어시스템의 제어과정


 그러면 이제부터 신경망을 이용한 모델예측제어기를 구성해 보도록 하자．
 제어기를 구성하는 단계는 다음과 같다．



단계1 Simulink Ubrary Browser창의 Neural network 블록셋의 Control 부분에서 NN Predictive
Controller 블록을 드래그하여 창에 넣는다. X(2Y) 블록도 Control 부분에서 드래그 해 올 수 있
다. 그 다음 플랜트에 대한 Simulink 모델인 口ant2.mdl 은 아래와 같다. 간단한 2차 시스템이다．




                                                        7 장 신경망 제어기 - 219


===== PAGE 218 =====
                                                                                     Gaini




                                                                                                       卜
                                                                                                       （ 了D
            In 1                                                                                        0uti
                        Gain                             Integrator                      Integratorl




                            ［그림 7.게 플랜트에 대한 Simulink 모델


 위 플랜트 모델의 subsystem을 만들어서 아래와 같이 제어기 우편에 연결한다．




       「놉·1．
            w
           며n mk．
                ■1m

                                                                                                         卜
                                                                                                               X2Y)
                                                                                PIant2




            ［그림 7.22] NN Predictive Controller와 플랜트 모델의 subsystem


단계리 NN Predictive Controller 블록을 더블클릭한다. 그러면, 아래와 같은 파라메터 입력창
을 보여준다．



                   洹    礪ndow     H引p




                                  Neural Network Predictive Control

                            Cㅇst Haiaifl(N2)                       C격rclWeIWntg FOCICI          o0드


                          c아甘r혀 HCdZn 卞）                                   Sn軾아Pa出ietn q.)      0간이


                       k衡甘r" z助여"Fkcm'.       c, chbac                샀er纖K;n0 Per s-    T懈
                                                          ㅓ


                      - ptal enmcolai     :              OK    ㅣ       -    Cancel   ㅣ

                               Pe1公Intl plani 1eel甘衲cmInn beret.control始r t어d佃tatlon.




                   ［그림 7.2〔司 NN Predictive Controller 파라메터 입력창



220 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 219 =====
，
단계이 아래부분에 있는 Plant Identification 버튼을 누른다. 그러면, 아래와 같은 창이 열린다．
아래의 신경망은 플랜트의 특성을 복사하는 모델이라고 할 수 있다. 은닉층의 뉴런 개수는 20
개이며 신경망의 입력으로 들어가는 데이터는 입력값, delay된 입력값, 피드백된 출력값과
delay 된 출력값이다. 가운데 부분은 학습을 위해 입출력 데이터의 최대값과 최소값의 범위를
보여주고 있고，학습을 위해 최대 8000개의 학습 샘플을 사용할 것이라고 되어 있다. 아래부
분에는 학습을 위해 필요한 반복학습회수가 최대 200으로 설정되어 있다．


               Pknl IdentiUcatian                                                    口 ∼及
             FUe    Window Help

                                       Plant Identification
                                           ＇岵w k ^zd小ect*.we
                       Size o什섭c1enLeye      20            卜勿r冶눕yed더며1h不｀i$           2

                      Sa目｀*．놀떻α켜rd (500)     0i            No.Debyed PIOI c出며」
                                                                             3        2

                   D t.kymeexe T'－널Die

                                                  T'* 甘지

              ∼a          Trni Swz)es       8oo                回Li댑
                                                                  （)J枷Die
                        枷軟出체｀se PW* h肛I      5                 綸1寸Y．
                                                                   』11l:,r맬
                                                                          《，써m』            5

                        出날nse汁i맣k驪i          .5                出*驪11nP늦nap』               루5
              Mexsn20hteovi Vise (500)       2             Sht * PWt Node          - 毓owee I
               흙漱*＇뵤月n놀*枕YdV쑵雜 (800)         01            目出寸2

                    G考m'me Tr·
                             「m낍 D찮s               如耳》刪 0出a                     （계t D님a
                                                                              EXp

                                            Tr`**4 Pveme(ezs

                           Tr& 哈Epochs       200               Tr**`F녜X：
                                                                       헒1X, trm伽

               ㅁUse C,xre,1We 1s           M Use Veddise Die              [JUse Testh낑Die
                                                           [      C00ce

                      Gen 吐008 b맬1'xt 4낡a bedNetr * 빙針m nosy甘1m｀
                                                               咽*【 川甘寸4



                         ［그림 7.24] Rant Identification 입력창

단계시 신경망을 학습하기 위해서는 학습용 데이터가 필요하므로 Generate Training Data를
누른다. 학습용 샘플은 최대 8000개 까지 제시를 하겠지만, 학습 샘플이 충분하다고 생각되면
중간에 중지를 할 수 있다．


단계5 Accept Data를 눌러 학습용 입출력 데이터를 확보한다．그리고 Train Network를 눌러
학습을 진행시킨다. 학습이 완료된 후에 아래 그림과 같이 학습성능을 보여준다．




                                                                                               7 장 신경망 제어기－221


===== PAGE 220 =====
                           0       l《〕 ㄻ      泌              o    싯〕      1α〕
                                     ttme 斜                      如..今（自          time (e)



                  ㅁ림 7.25] 학습이 완료된 후의 학습성능 비교


단계이 Plant Identification 창에서 ○K 버튼을 눌러서 창을 종료하여 학습된 NN 플랜트모델을
NN Predictive 제어기 블록에 탑재하게 된다．


단계 기 Neural Network Predictive Control 창에서 OK 버튼을 눌러 창을 종료한다. 이렇게 해
서 제어 파라메터들을 NN Predictive 제어기 블록에 탑재하게 된다．


단계 이 이렇게 해서 NN Predictive 제어시스템의 설계가 완성되었다. 시물레이션을 수행하기
위해서 전체시스템의 Simulink 모델로 돌아가서 Simulation 메뉴의 start를 눌러 시물레이션을
수행하면 다음과 같은 화면을 보여준다．


                                                   XY Plct
                           5




                   m又＜ >
                           0




                           5
                               0         10       a`      30       40       50
                                                    XAxis

               ㅁ림 7.26] NN Predictive 제어기의 성능 시물레이션



            （Matlab/Simulink를 중심으로）
222- 퍼지신경망 제어


===== PAGE 221 =====
6. ANFIS(Adaptive Network Based Fuzzy Inference Systems)


 1) ANFIS의 구조 및 학습방법


 ANFIS 방법은 주어진 데이터로부터 룰과 멤버쉽 함수를 학습하게 된다. 따라서，
ANFIS는 적응적인 네트웍
              （network) 이라 할 수 있는데, 이 네트웍은 마디
                                            （node）
                                                 와 연결
링크
 （link）
      로 구성되어 있다, 각 마디들은 마디의 출력값에 영향을 미치는 파라메터들
을 내부에 포함하고 있다. 그리고, 이 네트웍은 입력과 출력의 관계를 학습하게 된다．
 적응적 네트웍에는 다양한 방법들이 있는데, 여기서는Jang 이 제안한ANFIS 구조를
살펴보기로 하자. ANFIS 구조는［그림 7.27］
                           과 같다. 그림에서 둥근 마디와 사각형의 마
디가 있는데, 둥근 마디는 고정된 값을 가지고 있다. 하지만 사각형의 마디는 학습되어
지고 바뀌는 파라메터를 포함하고 있다．




                                          x   y

                 ［그림7.27] Sugeno 퍼지를 사용한 /\NFIS 구조


 Sugeno 퍼지를 사용한 ANFIS 구조는 다음과 같은 룰을 갖는다．


             IfxisA1andyisB1 THENf1 = p1x+ q1y+ r1


             〃xisA2andyis興      THEN f2 = P2X+ q2y+ r2


 ANFIS 구조의각층은 다음과 같은 특징을 가진다．


Layer 1 : 전건부
            （premise) 변수의 소속값
                            （membership value）
                                             을 계산한다．


                                                     7 장 신경망 제어기 - 223


===== PAGE 222 =====
 출력값을O1,i라고 놓으면 I은 첫 번째층
                       （layer）
                             을 의미하고, 1는 첫번째충의 ／번째 마
디를 나타낸다. 각 마디의 출력값은 다음과 같다．


                                   O1.i = ISA.
                                            （끼               力ri=l.2



                                   O1.i= /1且, (!/)           /bri=1.2



 여기서, A 혹은 B는 언어적인 퍼지변수
                      （예를 들면 small, large같은）
                                           이다. I2A (x）
                                                     는소
속값을 나타내며 다음과 같이 종
                （bell) 모양의 소속함수로부터 구해진다．


                                                         1
                                                       :ir - q
                                                                   요.
                                                  1+
                                                            아


 여기서, a-, b1, c1는 학습
                   （변경）
                      되어지는 파라메터 이다. 각 변수를 조정하면 소속함수
의 형태가 아래와 같이 변하는 것을 참고하기 바란다．


                        《．
                         ) changmg '1'                                       슈) Changmg `'


                l                                       i
           0.8                                         0.8
           0.6                                         0.6
           0.4                                         0.4
           0.2                                         0.2
                0                                       0
                -10     *5     .         5   l《1        -10             -5         .     5       i.
                         《亡）Cbaugbg '.'                          (d) cb솥41뇨1'` ' 홑꽈d v


                l                                       l




                                                        了八
          《y 8
            .                                          0.8
           0.6                                         0.6
           0.4                                         0.4
           0.2                                         0.2
                c1                                      0
                ·m      -s
                               0         5   l.         -10             -s
                                                                                   0         S   l0
                      ［그림 7.28] 파라메터 변화에 의한 소속함수의 변화 그래프



224   퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 223 =====
  Layer2: Rule의 영향력을 계산한다．


  2번째 충의 각 노드에는 변하는 파라메터가 있지 않고, 각 소속값을 곱하여 출력하
게 된다．


                     애＝Wi= /1A (X)PB(Y), i= 1,2


  Layer 3 : 영향력의 강도를 정규화
                       （norm勖ze) 한다.幢 , 2)


                                                          , Wi
                                   ,=
                              q.
                                                 wi= 泌1+
                                                                 W2
  Layer 4 : 후건부
              （Consequent) 파라메터
                              （Pi, q, r）
                                       를계산한다．


                       04,i = wifi = w2(px + qy+ ri)


  Layer 5 : 전체 출력값을 계산한다．


                          -             t-   ,   -   ..    > i Wji
                          (J5,j＝수WJi = Ziwi

  그림에서 보는 바와 같이 입력 값
                   （벡터）
                      이 네트웍의 충
                             （layer）
                                   을 통해서 다음 층으로
전달이 된다. 이제 ANFIS 모델이 어떤 방법으로 전건부와 후건부의 파라메터들을 학
습하는지 알아볼 것이다．


 학습방법은 많이 있지만 여기서는 Jang, Sun, Mizutani(Neuro-Fuzzy and Soft Computing,
Prentice Hall, 1997）
                   가 제안한 hybrid learning algorithm을 이용한다. 이 방법은 LSE(Least
Squares Estimation）
                  와 최급하강법
                        （SteepestDescent method）
                                               을 결합한 형태이다．


  전체 파라메터 셋을 S 라고 하면 S는
                      （전건부 파라메터 셋, 비선형）
                                      과（후건부 파라메



                                                                      7 장 신경망 제어기 - 225


===== PAGE 224 =====
터 셋, 선형）로 구분된다. 예를 들면, 다음과 같은 셋으로 구성될 수 있다．


        S1 = {{a11, b1, c11}, {a12, b12, c12}, " "' j {a1 , b1 , c1.}, ' " " , {a叩, bhp, c,,}}


                     S2 =   {{c10,
                                     c11,   '   "   "   첫   c1.   },   "   "   "   ,{cm0,   cml,   "   '   "   , c., ,   }}

 ANFIS 의 학습 알고리즘은 다음과 같이 2개 통로의 학습 사이클을 가진다．
 1) 순방향통로
        （Forward Pass) 학습 :
 여기서는 ＆은 고정된 값이고, S2는 LSE(least squared error）
                                             알고리즘을 이용하여
0枉line 적으로 학습이 이루어 진다．


 2) 역방향통로
        （Backward Pass) 학습 : 여기서는 S2는 고정된 값이고, Si은 최급하강법
                       을 이용하여 학습이 이루어 진다．
(steepest decent method）


 ANFIS의 순방향통로 학습을 위한 최소자승법
                         （LSE) 배치
                                （Batch) 알고리즘은 다음과
같다．
 ④ ParameterSet: S={S1U S2}, 그리고 Sin S2= b
 Output = F(I, S) , 여기서 I는 입력 벡터
 H(Output) = HF(I, S), 여기서 HF 연산은 S2 안에서선형적이다．


 G) 주어진 Si 값에 대해, K 학습 데이터를 이용하여 위의 식을 B=AX 식으로 변환한
      다. 여기서 x 는 S2의 요소들을 포함하고 있다．


 @) 이 것은 (ATA)!ATB = X' 관계식을 이용해서 구할 수 있다. 여기서, (ATA)!AT는 A
      의 슈도－인벌스
             （pseudo-inverse）
                            라고 부른다．


 ⑥ 그런 다음LSE는x를x*에 근사화함으로 해서 ∥ AX - B ii오차값 을 최소화 시
      킨다．




226   퍼지신경망 제어
             （Maflab/Sim미ink를 중심으로）


===== PAGE 225 =====
 匣）(ATA)'!ATB = X'를 직접 계산하는 것 보다는 전산수치적인방법으로 해결할 수 있다．


 i=O, 1, …,K-1의 영역에 대해


                                   Sai+ iaT+ 1si
                     i-I-I   '-'I 1+ al+ 1Sia1+1

                xi+1= Xi + Si+ 1ai+1(b7+l - a}+lXi)


 위 식에서 xo=o, s0 =x0 = 0, S0 =〃I（여기서，
                                   〃는 매우 큰 수를 사용함）
                                                 , 매는 행렬

A의 抄번째 라인을 의미함，
              bT는 벡터 B의 抉번째 요소를 의미함, 그리고X*=Xk이다．


 ANFIS의 역방향통로 학습을 알고리즘은 다음과 같다．
 먼저, 난번째 학습 데이터에 대한 학습 오차값Ek을 다음과 같이 정의한다．


                              N (L)
                         Ek= ＞〕(di- xL,i)2
                               i=   1



 위식에서
 N(L) : L충의 노드의 개수，
                  d1: 원하는 출력 벡터의 I번째 값, XL.i : 실제 출력 벡터의 i
번째 값을 나타낸다．


 따라서, 전체 학습 데이터의 오차값E는 다음과 같이 나타낼 수 있다



                             E= Z Ek
                                    k= 1



 각 파라메터 α，
         에 대해 update공식은




                                                      7 장 신경망 제어기 227


===== PAGE 226 =====
                                                      .           a +Ii
                                                     L\cxi =     〃＝=-
                                                                  oaj




 의    즈〕
       《뇌］서   n =
                            v-   , '.    8:   는학습률              이고，
                                                 （learning ratio）          K는스텝사이즈이다·   읨푸，
                    γZ1쁜，
는 순 미분
     （ordered derivative）
                        이다．


 이상의 알고리즘전개에서 알 수 있듯이 ㅆFIS의 구조는 신경망
                                  （neural network）
                                                 과매
우유사하며，
     주로 입출력 관계를 매핑
                 （mapping）
                         하는데 사용된다．


 2) MATLAB 명령어를 이용한 ANFIS의 학습


 AN1FIS를 생성하고 학습하기 위한 기본적인 nowchart는 다음 그림과 같다．



                                 Fuzzy System Initi키ization:
                                   엣始e gen乃눙i or genffs2

                                                           4
                                 Parameter Setup for Learning:
                                    -Number of iteration (epochs)
                                    -To!《》ranc슨 (=rror,
                                                            4,
                                 Start Learning Process: Initialization:
                                    -Use anfis
                                                 en error is satisfied
                                        - Stop v야，


                                                            4,
                                 V비idate:
                                    Use checking data




228          （Matlab/Simulink률 중심으로）
      퍼지신경망 제어


===== PAGE 227 =====
  (1) GENFIS1 과 ANFIS 명령어

   GENFISI 명령어는 소속함수의 형태와 개수 등을 설정하게 해준다. 명령어 형태는
다음과 같다．



                                 genfimDA7:4! 4i／인N, fY-4〃인TYPE)


   위에서 DATA는 학습용 데이터이며，
                      MFN는 소속함수의 개수이며, IN MF TYPE
는 소속함수의 형태를 나타낸다. 이해를 돕기 위해 아래 코드를 예시하였다．


% Generate random data
NumData= 1000;
data = [rand(NumData, 1) 10*rand(NumData, 1)-5 rand(NumData, I )];

% Speci玆 number and type ofmembership functions
NumMf=[37];
MfType = str2mat('pimf', 'trimf');
% Use GENFISito generate initial membership functions
FisMatrix = genfisi(data, NuniMf, MfType);
% Plot the membership functions

figure('name', 'genfisi', 'numbertitle', 'off');
Numlnput = size(data, 2) - 1;
for i = i:Numlnput;

subplot(NuniTnput, 1, i);
plotmf(FisMatrix, 'input', i);
xlabel(['input ' num2str(i) ' (' MfType(i, :) ')']);
end


  위 코드를 수행하면 아래와 같이 입력에 대한 퍼지 소속함수가 형성된다．




                                                                   7 장 신경망 제어기 -229


===== PAGE 228 =====
            !:* 트여 J.ocs 뾰1付m ”색〕

              D 盧日 毋                  \ ^ 1' /        β β 스



                    8 b 4

                 , 0 0 0 z
                 1          小
                            n U ^


                 쵸三딴m슐ㅌ 。ㅌ各。 m늠心。
                                    0     股      ㅓJ
                                              0.3      04      0,5    0.6   07   0.8   09
                                                         flput 1 ( imf)
                          呻


                   的 昨 胸 的 。




                 星년m蹈E。 ㅌ邕m客留ㅇ

                                                        1         0
                                                            input 2《1"mf}


                                    ㅁ림 7.2이 입력에 대한 퍼지 소속함수의 형성


0ㅖ 제 7.1 ANFIS 시스템을 이용하여 아래의 비선형 함수를 피팅
                                      （fitting) 해 보자．


                                 y = 0.6sin (7rx)+ 0.3sin(3irx)+ 0.lsin(5irx)


 i 쭐이

 먼저 입출력콴계 데이터를 다음과 같이 생성한다．

 %Number of input data points: numPts = 51, and input data: x
 numPts = 51;x = linspace(-1, 1, numPts)';
 % Output data: y

 y=0.6*sin(.pi*x)+0.3 *5j11(3 *pj*x)+0.1*sin(5*pi*x);


 생성된 데이터를 이용해 학습용과 테스트용 데이터를 다음과 같이 추출한다．
 % Store data in mafrix form: Iraining and checkingdata
 data=[x y]; % total data set




           （Matlab/Sim미ink를 중심으로）
230－퍼지신경망 제어


===== PAGE 229 =====
trndata = data(1:2:numPts,:); % training data set
chkdata = data(2:2:numPts,:); % checking data set


학습용데이터 (0 표시）
            와 테스트용 데이터   를 다음과 같이 그려본다．
                     （x표시）

%Plot lraining data (o) and checking data (x)
plot (trndata(:, 1),trndata(:, 2), 'o',chkdata(:, 1),chkdata(:, 2), 'x')
gnd

title('Training data (x) and checking data (o)')
xlabel('x');ylabel('Measured data for y');


                       ｀ge Na I
                   / F月】                                                                                       n同口
                   f솖 트｀ 工m                 卄*
                                        卜
                                                                                             ·
                   〔〕多 日                ，
                                            A /     /   舟 β        스

                            a
                            0                     Trainrng data (a) and chGckng dla（아



                                                            ;;1;
                                                                                                         沁
                                                                                                         的n小
                                                                                                           …
                                                                                ㅓ
                            6
                            。                                          “伊       ，
                                                                                ㅇ
                                                                                仰
                            4
                            0
                                                          ㅗ
                                                          1            X

                                                                       …                                         *
                                                                                                     1

                                                                                                     1




                        2    ,
                                                            -
                                                                                                     ；
                                                                       …        們            .   =
                                                                                                     ㅜ
                                                                                                                 -   ,




                        0
                                                                                                     1
                                 O
                                 ,
                                 n
                                                                                                     t
                                                                                                     1
                                                                                                     1
                                 1                                                           ,   m                   *
                                                                                                     1
                                                                                                     〃
                       小
                       닙。卜m花ㅉ 亡
                              으＝m
                                mm,
                                                                                                     :




                                                                   ㅇ   …                     m   ·                   *




                           4
                           O
                                                                                         T
                           6
                           O


                            1
                           8 ,                                                           脯                                        。
                           心          .08   06     O 4 《〕2                 以2       n4           r18
                                                                   `




다음은 초기 소속함수를 생성하기 위해 genfisi 명령어를 사용한다．


nunimfs = 5; % number of membership functions

mftype = 'gbellmf'; % membership functions type is generalized bell
fismat =genfis1(trndata, nummls,mftype);



FlSeditor의 anhis 메뉴를 열어서 초기 소속함수의 그림을 볼 수 있다. 또 다른 방법은




                                                                                                               7 장 신경망 제어기 -231


===== PAGE 230 =====
다음 명령어를 이용할 수도 있다．

 plotmf(fismat, 'input',l);


                                                      雖呈쟈；瑟，= n                                                교이씌

                    ［〕澤 日 好 녹 A / /' β J3》 n


                             '"?         f1                Inim
                                                              《2                                          mi




                           0a


                                4


                          0     0    o
                                     ,
                                     `
                          b
                          ^
                                                                                /
                        量m효ㅌ m드客앎H盼欌
                                                                                /
                                                                                /
                                                                                /
                                                                                /
                                 0

                                              .08      -08    -04        -02      0    02       04   06
                                                                                inPi#1
                                              “∼ 二   m=-     n＝∼ ,   ;   .   ∼三 ;   # 닌   小＂=




 이제 anfis 명령어를 이용하여 최적화 과정（학습과정）
                               을 수행해 보자．
 %Detennine number of iterations
 numepochs = 40;
 % Start the optimization
 [fismati, trnerr, ss, fismat2, chkerr]= ...
 anfis(tmdata, fismat, numepochs, NaN, chkdata);


 그러면 MATLAB 명령창은 아래의 파라메터 값들을 보여준다．
 ANFIS info:
     Number ofnodes : 24
     Number oflinear parameters: 10
     Number ofnonlinearparameters: 15
     Total number ofparameters : 25
     Number of training datapairs : 26
     Number of checking datapairs : 25


232 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 231 =====
      Number offuzzy rules: 5


그리고는 ANFIS의 학습을 시작하게 된다．


Start training ANFIS …
 1       0.0601596               0.058193
 2       0.0571745                0.0553133
  3      0.0541812               0.0524169
  4      0.0511445                0.0494663
  5      0.0480347               0.0464298


Step size decreases to 0.010567 after epoch 39.
 40       0.0110313                      0.0117976


Designated epoch number reached -> ANFIS training completed at ep0ch40.


이제 최종적으로 결정된 퍼지 소속함수를 plotmf명령어를 이용하여 확인해 보자．


plotmflfismatl, 'input',l)




                     f그 侈日e                    ` ^ 』/            β β 一

                                                    nlmt2               Ifnm日          ni m挺
                                                                         一∼，



                                                             \

                               。         8




                           mU     戶U
                                         6




                       芦mㄴ 寒드· ㅌ늠m으． m
                                     口
                                         4



                               。         2



                                  0

                                    ·1       4l8   06   ㅔ4       -O 2     .     D2   〔〕4   ［〕6   〔〕B
                                                                        nnpm'




                                                                                                       7 장 신경망 제어기 -233


===== PAGE 232 =====
 마지막으로 테스용 데이터에 대한 피팅 성능을 확인해 보자．

 out=evalfis(chkdata(:, 1), fismatl);% Evaluates the output of the fuzzysystem

 fismati - input checking

 hold;plot(chkdata(:, 1),out); % Plots out vs x

 plot(chkdata(:, 1), chkdata(:, 2)); % Plots y vs x (training data)

 plot(x, y); grid




 3) ANFIS EditorGUl를 이용한 ANFIS의 학습


                                              학습 그리고
 ANFIS Editor GUT를 사용하여 Sugeno 방식의 퍼지추론시스템을 생성，

테스트를 할 수 있다. GUll를 시작하려면 MATLAB 명령창에서 anfisedit를 입력한다. 그

러면 시시FIS Editor GUT는 아래 그림과 같이 새로운 창을 보여준다．




           （Matlab/Simulink를 중심으로）
234－퍼지신경망 제어


===== PAGE 233 =====
                                                                                    - 사f's 느눼D    -
                  1

                 08

                 06

                 α4

                 02

                                                                                        ck’α1斗맣   -
                  00        α2         0.4         08              α8

                                        .』며｀erdbIF應          " Tra1, FIS        -   --- Test二S        --
                                                             .m1n 닒 ＇ㅉl
                                   乙 u》
                                      的 1,07, 佩e             卜벼낚닙               」
                       a '1e       r    나ad hoa w0, 3뀨       E7,甘 T嫩d材
                                   佇                         'C,
                                   戶 3出 claltel7,Q
                                                             努괏珊        ‘-
                                         ($eaeete II`    -          Trm, r넌1w




                               ㅁ림 7.30] ANAS Editor의《3U1 창


 이창은 다음과 같이 4개의 작업으로 구성되어 있다 :
 ① 데이터의 탑제, Plotting 및 삭제 과정
 ② 초기 FIS 모델의 생성 혹은 기존모델의 탑재 과정
 ③FIS 모델의 학습과정
 ④ 학습된 FIS모델을 검증하는 과정


 이제 데이터 셋을 학습하고 테스트하는 과정을 알아보자. 테스트를 하는 경우에는
데이터에 약간의 잡음
          （noise）
                이 추가될 것이다. 순서는 다음과 같다．


 (1) 데이터입력
 학습데이터 셋
       （fuzexltrnData, fuzex2tniData）
                                    과테스트데이터 셋
                                            （ftizexlchkData, thzex2chkIta)
을 ANFIS Editor GUI에 입력한다. fuzdemos 디렉토리로부터 위데이터들을 MATLAB
Workspace에 Load 하기 위해서 명령창에서 다음과 같이 Type 한다．
   load fuzexltrnData.dat
   load fuzex2trnData.dat
   load fu.zexlchkData.dat
   load fuzex2chkData.dat


                                                                                            7 장 신경망 제어기 -235


===== PAGE 234 =====
 ②MATLAB창에서 anfisedit를 입력하여 ANFIS Editor GUI를 open한다．
 ③ 작업창         으로부터 학습 데이터를 로드하기위해，
     （workspace）
   a) GUT의 Load data 부분에서 다음 옵션을 선택한다．
    · Type : Training
    ' From : worksp
   b) Load Data를 클릭하여 다음 대화창을 오픈한다．




   C) 위 대화창에서 fuzexltmData를 입력한 다음 OK 버튼을 클릭한다．
 학습 데이터는 퍼지시스템을 학습시키는데 사용된다. 이 때 데이터를 가장 잘 학습
할 수 있도록 퍼지 소속함수의 파라메터들을 조정한다. 그리고 학습된 데이터는 GUI
화면에 창에 조그만 원모양의 형태로 그려진다．


                 ., ＾繃,(dto,t洲tI1ed


                                           Trat「貂｝gDIta (oa})                           尸〃咐shb



                                                       C) ㅇ
                                                           QQOOO




                        0
                 m.-- L心*                -       G멥甘珌aFr…－ㄱ                             -- k뻐ns         -
                  i昨｀
                    …    「 roS
                 갛＝ !r'* 甘     ［…∼
                                             r   L。 h。
                                                     ,i·   …    ㅣ   ）州눕헙           二」 끼마倂났
                  -          r∼ 肛            r, l瀜1,m W醫柚p.                           G nmㄱ·끼mm
                 r ！鹹甘맣        '-


                                             尸 ㅇmm＇驪驪t              10
                                                                                        r   TI甘·刃 dm·

                                                                    쁜
                口r一臼 松향      ｛수 벡q．
                                  畔…
                                             r   盒七m拗目t拉                                r (1咐*4如
                 r m…               이

                  댈恥臘．.d      UNI OdS〔           (j·哨a口n各一      1        nmH냄그＂'    l         ∼   ∼         1
                 勺끼鱗d好k.d4r           ／…              「…                  －켜」               －으쁘－ 」



                      ［그림 7.3가 G네 화면 창에 그려진 학습 된 데이터




            （Matlab/Simulink를 중심으로）
236- 퍼지신경망 제어


===== PAGE 235 =====
 ④ workspace에서 체킹데이터를 로드하기 위해서，
   a) GUI의 Load data 부분에서 Checking을 선택한다．
   b) 그런 다음 Load Data를 선택한다．
   C) 입력변수 이름을 fuzexI chkData로 입력하고 OK 버튼을 누른다．


 그러면, 아래 그림과같이 체킹 데이터와학습에이터가같이 그려지게 된다．


              !J A,thaFr仕0r= t玉nt*H뺘，r샅


                                                 Checting Data (+++)                             m- 사ft$h1O   -
                        1
                                                          ＋十
                        걀
                        ㅗ
                        닝
                        ∥                                                    c
                                                        c'oo小轍古礬盼3＋十

                ，요＝ ㅇ
                        0
                                1-
                                                                             （꺼
                    니
                    仄
                    U
                    n           ㅇ'       + 1.
                                        00. 。수
                                     DktHm
                                             "
                                                  층
                            0                5   '0       15        2          25            珊
                        1
                                                      G혀甘出eFtS      --- -- Trah nS      -- --- Te出디S
                                                                          >mn,. Mothoot
                                                  乙 t.aod troidiB
                                                                          和눠k넋          二」
                                                  C uad Irmrwork하》          &oor T아erarce'

                                      口 work叩
                                                  α G
                                                    『｝dF0011,00
                                                  C 9ㅊ）댜.ierraj
                                                                        ㅣ
                                                       Gwe,Me H8                                                  I
               d꽝아
                 （ 小Bta k）
                         岫」




                                             ［그림 7.32] 체킹 데이터와 학습데이터


 다음단계는 anfis를 학습하기 위하여 퍼지추론시스템을 초기화하는 것이다．


 (2) Initializing and Generating Your FIS
 사용자가 FIS 파라메터를 독자적으로 초기화 할 수 있고, 혹은 자동으로 FIS 파라메
터를 생성하게 할 수도 있다．


 ①FIS 파라메터의 자동생 성
   a) Grid partition을 선택한다．
   b) Generate FIS 버튼을 클릭한다. 그러면, 다음과 같이 메뉴가 나타난다. 소속함수



                                                                                                      7 장 신경망 제어기 237


===== PAGE 236 =====
     의 개수를 정할 수 있고, 소속함수의 형태도 지정할 수 있다. 하지만 출력소속
     함수에 대해서는 상수값이다 선형식을 사용해야 한다. 그 이유는 anfis 모델은
     Sugeno 방식의 퍼지시스템을 사용하기 때문이다．
   C) 다음과 같이 값을 설정하고 OK 버튼을 클릭한다．




                   ㅁ림 7.33] FIS 파라메터 자동생성 입력창


 ②ANFIS용 소속함수를 직접작성
 사용자가 FIS Editor를 사용하여 ㅆFIS용 소속함수를 직접작성 할 수 있다．
   a) Edit 메뉴에서 Membership functions 메뉴 항목을 연다．
  b) 필요한 소속함수를 하나씩 만들어 간다. 단, 출력 소속함수는 상수값이나 선형
    식을 사용한다는 점을 유의하자．
   c) Edit 메뉴에서 Rules 메뉴를 선택한 다음, Rule Editor를 사용하여 전체 퍼지룰을
    작성한다．
   d) FIS Pr야)erties 메뉴를 선택한다. 그리고 FIS 모델의 이름을 지정한 다음 저장한다.
   e) Close 버튼을 클릭하고 ANFIS Editor GUI 창으로 들어가서 FIS모델을 학습시킨다．
   f) ANFIS 초기화를 위해 현재의 FIS를 load 하기위해서는 Generate FIS에서 Load
    from worksp. 혹은Load from file을클릭한다．




238－퍼지신경망 제어
           （Matlab/Sim미ink를 중심으로）


===== PAGE 237 =====
 ③ 생성된 FIS 구조
            （structure) 보기
 FIS 구조를 생성한 후에 Structure 버튼을 클릭하여 FIS 구조를 볼 수 있다. 다음과 같
이 새로운 창이 pop-up 하게 된다．




             .`* m   ad1.de切 혀
                             ＂截如 t얇凹跏，   냐心e




                「l림 7.34] Structure 버튼을 클릭하여 FIS 구조를 확인


 그래프에서 가지나 마디들은 color에 의해서 논리적으로 구분된다. Edit 메뉴를 이용
하면 작성된 소속함수나 퍼지룰을 확인 할 수 있다．


 ANFIS의 학습
 FIS를 학습하기 위한 anfis 파라메터 최적화＜학습）옵션은 hybrid와 backpropa 두가지
가 있다．
    hybrid 방법은 least squares와 backpropagation 알고리즘을 혼용하는 형태이다．
 오차여유
    （error tolerance）
                    는 학습 중에 정지를 시킬 수 있는 기준을 제시한다. 즉, 학습
중에 오차값이 지정된 오차여유보다 작아지면 학습을 종료하게 된다．


 학습을시작하기위해서다음의과정을수행해보자．
 ① 최적화
     （학습）방법을hybrid 로 선정한다．
 ② 반복학습 횟수
         （epoch）
               를 40으로 선정한다．
 ③Tram Now를 선택한다．



                                                    7 장 신경망 제어기 -239


===== PAGE 238 =====
 40회 동안 학습을 하는 동안의 학습오차값을 아래와 같이 보여 준다．




                        ㅁ림 7.35] 학습오차값


 위 그래프에서 ◆ ◆ 표시는 테스트용 데이터의 오차
                            （checking error）
                                           를 나타내고，
                                                 **
표시는 학습오차              를 나타내는 그래프이다．체킹오차가 처음에는 감소하
       （training error）
다가 어느 지점부터 다시 증가하기 시작하는 것을 볼 수 있다. 이러한 증가는 FIS 모델
이 overfitting이 되었다는 것을 의미한다. 따라서, ANFIS는 overfitting이 되기 직전（즉，
체킹오차가 최소가 되는 경우）
               의 파라메터를 모델 파라메터로 선정하게 된다．
                                       이 예는
체킹 데이터가 왜 필요한지를 잘 설명해 주고 있다．


 학습된 FIS 모델에 대한 성능테스트
 체킹 데이터를 이용해서 학습된 FIS 모델을 테스트하기 위해 Test FIS에서 Checking
data를 선택한 후 Test Now를 클릭한다. 다음 그래프와 같이 성능을 파악할 수 있다．




240 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 239 =====
     〔d"o. Unhth,d
' ^HnS                                                                                                ■ㅂ口
E솖   됴出        Y.4따

                                   CheJdn9 d楸a + ns 여』
                                                     tn』
                                                       t '                              - ANF筠 ImD         -


                                                                                         4 이nㅉ 1
      哨                                                                                  #    蠟以心；1

                                                                     "   :               甘 d 1好
                                                                                              ＇mi

 i8
                                                       /,:,,,,
                                                                                         4
      。
                                                                             *
                                                   +
                       辛+후t*甲* , +*
                           ㅗ   .     上
      桶
                                     4'    ㅗ

      ㅓ
                  ej.
                  '    1                       수                                            St   iuc*`,e   l
          八u
                                          1ㅇ
                                                 Index
                                               G甘eraIe FIS       -                      -- 1e앍 FIs



                      r` 3轍




                                                                 ㅣ
 Ave,a卞 IOON4 en           0 1461                                                He ,
                                                                                   w
                                                                                        ㅣ          CIoo0       -

     ㅁ림 7.3이 체킹데이터를 이용한 학습된 AS 모델의 테스트




                                                                                                    7 장 신경망 제어기 241


===== PAGE 240 =====
8장        회귀신경망
              （Recurrent Neural Network)




     회기신경망은 구조적으로 보면 신경망의 은닉충이나 출력충의 출력값이 신경망의
입력부로 피드백되는 구조를 말한다. 이러한 형태의 신경망은 시간적으로 변하는 패
턴을 학습하거나 여러가지 경우의 값을 특징적인 패턴으로 분류하는 경우에 많이 적
용이 된다. 대표적인 경우로는Elman신경망과Hopfield신경망이 있다．




1. 티man 신경망

     Elman 신경망은 아래 그림에서 보는 바와 같이 은닉충의 출력값이 신경망의 입력부
로 회귀되는 형태를 취하고 있다는 점이 일반 신경망과 다른 점이다. 피man 신경망은
시간적으로 변하는 특징
           （패턴）
              을 감지하거나 생성하는데 사용된다．
     그림에서 보는 바와 같이 회귀되는 데이터는시간지연을 거쳐서 신경망의 입력부에
들어가게 된다. 이것은 시간적으로 앞 단계에서 처리된 정보가 현재시간의 데이터를
처리하는데 함께 이용이 된다는 것을 의미한다. 바로 이런 점에서 Elman 신경망이 구
조적인 패턴뿐만 아니라 시간적으로 변하는 패턴
                        （temporal pattern）
                                         을 학습할 수 있는 능
력을 갖게 된다．




                                  （Recurrent Neural Network) _243
                         8 장 회귀 신경망


===== PAGE 241 =====
                                                   /   ,                  ,
                 Inputs          Recurrent layer           Output layer

                               ［그림 8.1] two-layer 티man network



 1) 티man 신경망의 생성


 Elman 신경망은 MATLAB에서 주어지는 newelm 이라는 명령어를 사용하여 쉽게 생
성할 수 있다. 앞의 그림에서 보는 바와 같이 Elman 신경망은 일반적으로 은닉층에는
tansig 활성함수를 적용하고 출력층에는 pureim 활성함수를 사용한다．


 Elman 신경망을 아래와 같이 구성하게 되면 신경망은 입력값의 범위는 0과 1사이의
                                    은닉층은 tansig 출
값이고, 은닉층의 뉴런 개수는 5개 출력층의 뉴런 개수는 l개이고，
력충은 logsig 형태의 활성함수를 사용한 형태를 의미한다．


                         net = newelm([0 1], [5 1], {'tansig', 'logsig'});


 日man 신경망의 반응을 보기 위해 0 혹은 1로 구성되어 있는 8개의 순서입력값음신
경망에 입력하도록 한다. 다음과 같이 해서 8개의 임의의 값을 생성할 수 있다．


 P = round(rand(1, 8))
 P=
      0    1 0   1 1 0         0    0


                                    （sequence）
 하지만 이 값은 하나의 벡터값으로 되어 있으므로 아래와 같이 순서        로바
꾸도록 한다．


244              （Matlab/Simulink를 중심으로）
          퍼지신경망 제어


===== PAGE 242 =====
 Pseq = con2seq(P)
 Pseq =
  [0] [1] [0] [1] [1] [0] [0] [0]


 이제 구성된 Elman 신경망과 순서입력을 가지고 sh끄 함수를 이용해서 신경망의 출
력값을 아래와 같이 구할 수 있다．


 Y = sim(net,Pseq)
 Y=
 Columns 1through 5
  [1.9875e-04] [0.1146] [5.0677e-05] [0.0017] [0.9544]
 Columns 6 through 8
  [0.0014] [5.7241e-05] [3.6413e-05]


 즉, 위와 같이 8개의 순서값이 출력되었다. 물론 순서값을 다시 벡터값으로 표현하
는 것도 가능하다. 아래 명령은 순서값을 벡터값으로 바꾸는 명령에이다．


 z = seq2con(Y);


 그리고 다음과 같이 하여 벡터값으로 나타낼 수 있다．
 z{1, 1}
 ans =
 Columns 1through 7
  0.0002 0.1146 0.0001 0.0017 0.9544 0.0014 0.0001
 Column 8
  0.0000


 위 경우는 학습이 완료되지 않은Elman 신경망에 임의의 입력을 넣었을 때 생성되는
출력값을 나타낸 것이다. 이제 주어진 입력과 출력값을 이용하여 Elman 신경망을 학습




                                   8 장 회귀 신경망
                                            （Recurrent Neural Network) 245


===== PAGE 243 =====
해보도록 하자．


  2) 티man 신경망의 학습


 Elma끄 신경망은 trai끄이나 adapt 함수를 이용하여 학습이 될 수 있다. 먼저 학습에 필
요한 입력 데이터와 타겟
            （목표）데이터를 다음과 같이 생성해 보자. P는 입력벡터이고
T는 타겟벡터이다．


 P = round(rand(1, 8))
 P=
      1 0      1 1     1 0       1 1


 T= [0 (P(1:end-1)+P(2:end)       2)   ]
 T=
      0    0   0 1   1   0 0      1


 타겟벡터는 입력벡터내의 값이 연속적으로 두 번 1이 들어오는 경우에 그 때의 타곗
값．
 이 1이 되도록설정하였다. 그리고Elman신경망은다음과같이 구성하였다．


 net= newelm([0 1],[51], {'ta끄sig', 'logsig'});
 Elman 신경망은 다음과 같이 학습이 진행된다．
 net = train(net, Pseq, Tseq);


 학습이 완료된 후에 아래와 같이 siiㅍ 함수를 사용하여 학습성능을 테스트할 수 있다．
 Y = sim(net, Pseq);
 z = seq2con(Y);
 z{1, 1};
 diffl= T- z{1, 1}




246              （Mat lab/Simulink를 중심으로）
          퍼지신경망 제어


===== PAGE 244 =====
 위에서 diffi 값은 목표 타곗값과 실제 신경망의 출력값 즉 학습오차를 나타내고 있
다. 학습이 정상적으로 완료되었다면 diffi은 매우 작은 값으로 구성될 것이다. 위에서
설명한 내용을 m 파일로 구성하면 다음과 같다．


 %% File name: ElmanNetl.m
 %% Suppose that wewant to fmd the response of this network to an input sequence of eight
 digits
 %% that are either Oor 1.
 %% Elmannetl.m
 P=[1 0 1 1 1 0 1 1]
 T=[0 0 0 1 1 0 0 1]
 %% Here T is definedto be 0, except when two l 's occur in P, in which case T is 1.
 net=newelm([0 1],[501], {'tansig', 'logsig'});
 Pseq=con2seq(P)
 Tseq=con2seq(T)
 net=train(net, Pseq, Tseq);
 Y=sim(net, Pseq)
 z=seq2con(Y);
 z{1, 1}
 diffi = T- z{1, 1}
 위의 m 파일을 실행하면 다음과 같이 학습이 진행되고 학습오차 difil 을계산하게 된다．


 >> ElmanNeti
 P=1 0         1 1 1         0   1 1
 1= 0      0   0   1 1       0   0   1
 Pseq = [1] [0] [1] [1] [1] [0] [1] [1]
 Tseq = [0] [0] [0] [1] [1] [0] [0] [1]


 TRAINGDX, Epoch 0/100, MSEO.253884/0, Gradient 0.432151/le-006




                                          8 장 회귀 신경망＜Recurrent Neural Network) - 247


===== PAGE 245 =====
 TRAINGDX,Epoch 25/100, MSEO.191333/0, Gradient 0.353458/le-006
 TRAINGDX,Epoch 50/100, MSEO.0982732/0,Gradient 0.182143/le-006
 TRAINGDX,Epoch 75/100, MSEO.0338878/0, Gradient 0.0910471/1e-006
 TRAJNGDX,Epoch 100/100, MSEO.00371528/0, Gradient 0.0150204/1e-006
 TRAINGDX,Maximum epoch reached, performance goal was not met.


 Y = [0.0892] [0.0321] [0.0484] [0.9706] [0.9351] [0.0615] [0.0507] [0.9166]


 ans= 0.0892 0.0321 0.0484 0.9706 0.9351 0.0615 0.0507 0.9166


 diffi =-0.0892 -0.0321 -0.0484 0.0294 0.0649 -0.0615 -0.0507 0.0834


 아래그림은 학습이 진행됨에 따른 학습오차를 보여주고 있다．


                                           Pe,bnn,ce k 0.00371528, Go미ISO




                             r


                   ·2띠숟t겯F
                             r




                                 10   a1     出1   10    50   80     10      凹   玭1   100
                I S*c)1rISw l                       1m Epoc눕




2. Hopfield 신경망


 Hopfield 신경망은 특정한 개수의 도달점을 기억하게 할 때 사용되는 신경망이다. 즉，
어떤 영역내의 임의의 입력값이 이 신경망에 입력이 되면 입력값에 가장 근접한 도달


248   퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 246 =====
（혹은 평형점）
점                Hopfield 신경망의 기본구조는 아래와 같다．
       으로 이동하게 된다．




            ㅏ   %       _J
                              ..,..


                    1niti히            Symmetric saturated
               conditions                 linear layer

                             ［그림 8.의 Hopfield 신경망


 Elman 신경망과 달리 Hopfield 신경망은 신경망의 출력값이 입력부로 회귀된다．그
리고 또 다른 특징은 이 경우 입력벡터 P는 단지 초기조건으로만 신경망에 입력이 된
다. 다시 말하면 입력벡터 P는 신경망에 연결이 되어 있지 않다고 할 수 있다. Hopfield
신경방의 뉴런 내의 활성함수는 다음과 같은 satlins 활성함수를 사용한다．




              ［그림 8.31 Hopfield 신경망의 뉴런 내의 활성함수



 Hopfield 신경망의 구조는 newhop 함수를 사용하여 생성할 수 있다. Hopfield 신경망에
도달점
  （평형점）
      을 선정한 다음 이 도달점을 신경망에 입력하여보자. 그러면, Hopfield
신경망은 내부의 가중치를 업데이터하기 시작한다. 업데이터가 완료된 후에 최종적인
가중치 값을 조사하면 가중치 값 자체가 도달점의 정보
                            （데이터）
                                를 간직하고 있다는 것


                                                 （Recurrent Neural Network) _249
                                        8 장 회귀 신경망


===== PAGE 247 =====
을 알게 될 것이다. 그리고, 임의 초기입력이 주어지면 신경망은 초기값과 인접한 도달
점의 정보를 출력하게 된다．


 아래의 예를 살펴보면 분명하게 이해가 될 것이다. 3차원 공간인 x, y, z 좌표에서 2개
의 도달점을 다음과 같이 선정해 보자．


 T=[-1-1 1; 1-11]'
 T=
   -1          1
   -   1   -   1
       1   1


 그런 다음 도달점을 나타내는 벡터 I를 newhop 함수에 입력한다．


 net = newhop(T);


 가중치업데이트가 완료된 후에 Hopfield 신경망이 임의의 입력에 대해 도달점으로
안내를 하는지 살펴보자. 먼저 도달점 자체인I를 초기 입력값으로 넣어보자．


 Ai= T;
 [Y, Pf, Afj = sim(net, 2, [1' Ai);
 Y


 시물레이션 결과 출력값은 정확하게 도달점을 나타내게 된다．
 Y




       1 1


 다음은 도달점이 아닌 임의의 값을 Hopfield 신경망의 초기값으로 설정해 보자．


           （Matlab/Simulink를 중심으로）
250 퍼지신경망 제어


===== PAGE 248 =====
      Ai = {[-0.9; -0.8; 0.7]}


 이 값을 이용하여 다시 시물레이션을 수행해 보자．


 [Y,Pf, Af] =sim(net, {15}, {},Ai);
               1}
 Y{
 시물레이션 결과 다음과 같은 출력값을 확인할 수 있다．
 Y=
       -   1
       -   1
           l


 즉, 임의의 입력값을 넣게 되면 신경망은 그 입력값에 가장 근사적인 도달점으로 안
내하고 있음을 알 수 있다．



0ㅖ 제 8.1 2개의 뉴런을 갖는 Hopfieid 신경망을 고려해 보자. 각각의 뉴런은 바이어스와 가

중치를 갖고있다. 신경망에 저장될 도달점 T를 아래와 같이 선정해 보자．




      이 도달점
          （평형점）
              은 아래 그림과같이 2차원의 영역에서 ' *' 표시에 놓이게 될 것이다．




                                      8 장 회귀 신경망
                                               （Recurrer,t Neural Network) - 251


===== PAGE 249 =====
                                 Hopfield Network State Space

                             l 女


                       a（그）

                             0




                         -   1                            *

                                     1        0           1
                                                  a(1)
                                 -
 이제 도달점 데이터를 Hopfield 신경망에 넣어 가중치와 바이어스를 구해보자．
                                             명령
문은 다음과 같다．


 net = newhop(T);


 그런 다음 각 뉴런의 가중치와 바이어스를 구해보면 다음과 같다．


 W= net.LW{1, I}


 위 명령어를 사용하여 다음과 같은 가중치를 확인할 수 있다．
 w=
      0.6925 -0.4694
      -0.4694 0.6925


 그리고, 아래 명령어를 이용하여


 b= net.b{1, 1}


 다음과 같이 바이어스를 확인할 수 있다．




252            （Matlab/Simulink를 중심으로）
        퍼지신경망 제어


===== PAGE 250 =====
 b=
      1.0e-16 *
      0.6900
      0.6900


 이제 Hopfield 신경망이 도달점을 제대로 기억하고 있는지 테스트를 해 보자．
                                             도달점
벡터 T를 신경망에 넣어 결과를 확인해 보자．


 Ai = T;
 [Y, Pf, Al] = sim(net, 2, [II, Ai);
 Y        =




          1 -1
      -   1   1


 Hopfield 신경망은 정확하게 도달점을 출력해 준다. 이제는 다른 임의의 입력벡터를
선정하여 Hopfield 신경망에 초기값으로 입력해 보자. 아래의 결과 그림을 보면 임의의
초기값이 점차로 자신에게 가까운 도달점으로 이끌려 간다는 것을 알 수 있다．


                                         Hopfield Network State Space

                                     1

                             a(2)

                                     0




                                 -   1
                                         -   1        0           1
                                                          a(1)




                                                          （Recurrent Neural Network) - 253
                                                 8 장 회귀 신경망


===== PAGE 251 =====
9장         자기：성
              （Self-          Organizing           ）신71D1.




     자기구성 신경망은 신경망에 입력되는 많은 값들로부터 규칙성이나 상관관계를 검출
할 수 있도록 학습을 하는 신경망이다．
                    자기구성 신경망에는 경챙학습
                                  （competitive learning)
신경망과 SOFM(Self-organizi끄g feature map）
                                     이 있다．




]. 경쟁학습
      （Competitive Learning) 신경망

     경쟁충
       （Competitive layer）
                         에 있는 뉴런은 한 번에 1개의 뉴런만이 활성화되고 다른 뉴
런들은 비활성화 상태를 유지하게 된다. 즉, 입력벡터에 가장 근접한 가중치를 보유하
고 있는 뉴런만이 활성화된 값을 출력하게 된다. 경챙학습 신경망의 구조는 아래 그림
과 같다．
     경챙충 뉴런에 입력되는 입력벡터는 경쟁 활성함수로 전달된다. 여기서 승자
                                            （winner)
는 1의 값을 출력하게 되고 나머지 뉴런은 0의 값을 출력하게 된다. 가장 큰 값을 가지
는 뉴런이 승자이다．
     신경망에서 바이어스가 0이라고 한다면 입력벡터와 가장 가까운 가중치를 갖는 뉴
런이 가장 적은 음수값을 갖게되고
                 （경챙에서 승자가 되고）
                             ,1의 값을 출력하게 된다．



                                           9 장 자기구성
                                                  （Self-Organizing) 신경망－255


===== PAGE 252 =====
                       `--      1    %.

                             h가)ut        Competitive layer
                                ［그림 9.1] 경쟁학습 신경망의 구조


 1) 경쟁학습신경망의 생성


 MATLAB에서 경챙학습신경망의 생성하기 위하여 newc 명령어를 사용한다. 간단한
예를 통하여 신경망을 생성해 보자．


 다음과 같이 4개의 입력벡터를 고려해 보자．
 p=[.l .8.1. 9; .2.9.1.8]

 p=
  0.1000 0.8000 0.1000 0.9000
  0.2000 0.9000 0.1000 0.8000


 위 4개의 벡터를 2개의 클래스     로 분류하고자 한다. 경험적으로 살펴보면 위의
                 （class）
4개 입력은 원점과 (1, 1) 위치로 분류됨을 알 수 있다. 경쟁학습신경망을 이용하여 결
과를 확인해 보자．


 먼저, 2개의 입력요소를 갖는 2개의 뉴런을 설정하고 입력의 범위는 0과 1사이임을
지정한다. 그러면, 신경망을 생성하는 명령어는 다음과 같다. Newc의 첫번째 항는2 입
력 요소값의 범위를 나타내고, 두번째 항은 뉴런의 개수를 나타낸다．


 net= newc([0 1; 0 11, 2);



           （Matlab/Sim미ink를 중심으로）
256－퍼지신경망 제어


===== PAGE 253 =====
 여기서, 신경망의 가중치는 입력값의 중간값인 0.5로 초기화 된다. 다음 명령어를
이용하여 확인할 수 있다．


 wts= net.IW{1, 1}
 wts=
   0.5000 0.5000
   0.5000 0.5000


 바이어스의 초기값은 다음과같이 확인할 수 있다．


 biases= net.bias {1, 1}
 biases =
   5.4366
   5.4366


 2) Kohonen 식을 이용한 신경망의 학습


 신경망에서 승자
        （winner) 뉴런의 가중치들은 Kohonen의 학습규칙에 의해 조정된다．
이 가중치는 가중치 행렬 내에서 행으로 표시된다. 예를 들면 f번째 뉴런이 승자가 될
때 가중치 행렬의 i번째 행의 값이 다음과 같은 식에 의해 조정된다．


                   iIW" (q) = i W" (q- 1)+Q(p(q)-iIW" (q- 1))


 Kohonen 규칙은 뉴런의 가중치가 입력벡터를 바로 학습하게 한다. 즉, 대표적인 입
력값 자체를 가중치가 기억을 하고 있다. 따라서, 경챙학습 신경망은 패턴분류나 인식
부분에 많이 적용이 되고 있다．


 이제 경쟁학습 신경망을 500회까지 학습을 하고자 한다. 학습을 위한 명령어는 tram
이나 adapt 함수를 사용할 수 있다．




                                          9 장 자기구성
                                                 （Self-Organizing) 신경망－257


===== PAGE 254 =====
 net.trainParam.epochs = 500
 net = train(net, p);


 학습 후에 신경망에 입력벡터 P를 입력하여 다음과 같이 시물레이션을 수행해 보자．


 a = sim(net, p)
 ac = vec2ind(a)


 결과값은 다음과 같다．
 ac =
   1 2       1 2


 위 예에서 경챙학습 신경망은 입력벡터를 2개의 그룹으로 분류하도록 학습되어짐
을 알 수 있다. 이 경우 원점에 가까운 입력값은 클래스 1로 분류되고, 좌표
                                          （1, 1）
                                               에 가까
운 입력은 클래스2로 분류되는 것을 확인할 수 있다．


 학습된 신경망의 내부의 가중치와 바이어스 값을 살펴보면 매우 흥미로운 사실을
알 수 있다．


 wts =
  0.8208 0.8263
  0.1348 0.1787
 biases =
   5.3699
   5.5049


 위의 가중치 행렬에서 첫번째 행을 보면 그 값이 (1, 1) 값에 근접한 것을 알 수 있다．
반면에 2번째 행은 원점에 매우 가깝다. 이와 같이 학습된 신경망 내부의 가중치는 입
력값들을 분류할 수 있도록 조정됨을 알 수 있다．




258－퍼지신경망 제어
           （Matlab/Sim미ink를 중심으로）


===== PAGE 255 =====
예 제 9.1 경쟁학습 신경망의 분류능력을 보기위해 80개의 임의의 입력값들을 난수적으로

생성하였다. 경쟁학습 신경망을 이용하여 80개의 점을 8개의 집단으로 분류하고자 한다. 먼저
다음과 같이 80개의 첨을 생성하자．


 X = [0 1; 0 11; % Cluster centers to be in thesebounds.

 clusters = 8;     % This manyclusters.
 points = 10;      % Number ofpoints in each cluster.
 stddev = 0.05; % Standard deviationof each cluster.

 P = nngenc(X, clusters, points, std_dev);


 %PlotP.

 plot(P(1, :), P(2, :), '+r');
 title('Input Vectors');
 xlabel('p(l)');
 ylabel('p(2)');


 아래그림은 난수적으로 생성한 80개의 점을 보여주고 있다．


                                                        1ipiit Voctcis
                             (L9

                             (L8

                             0.7

                             0.6

                             0.5

                        e.   0.   4

                             0.3

                             0.2

                             α1

                                  0

                         《L1
                           0.1        0.2   0.3   a4   0.5    α6     07   08   0.9   1   11
                                                             P《1》




 이 점들을 분류하기 위해 다음과 같이 경쟁학습 신경망을 설정해 보자. 신경망의 설
정은 newc 함수를 이용하여 구축할 수 있다. 함수의 첫번째 항은 입력값의 범위를 나타


                                                                9 장 자기구성
                                                                       （Self-Organizing) 신경망－259


===== PAGE 256 =====
내고, 두번째 항은 뉴런의 개수, 3번째 항은 학습율을 나타낸다．


 net = newc([0 1;0 1], 8, .1);
 w=netiW{1};
 plot(P(1, :), P(2, :), '+r');
 hold on;
 circles = plot(w(:, 1), w(:, 2), 'oh');


 아래 그림은 학습이 진행되기 전의 초기상태를 표시한 그림이다. 8개의 가중치정보
가（0.5, 0.5) 위치에 모여 있다. 이 점은 학습이 진행될수록 80개의 점들을 8개의 집단으
로 분류하고 가중치는 각 집단의 대표위치로 이동하게 될 것이다．


                        09

                        0.8

                        0.7

                        α6


                                                             卄 +
                                                  0    b +

                                                                   뇨간         + +
                        05
                                                       ＋나



                        0.3




                          (1

                        0 .1
                           0.1   02   0.3   0.4   05   00     07   09   i_i




 이제 구성된 경쟁학습 신경망을 학습해 보도록 하자．


 net.trainParam.epochs =7;
 net = train(net, P);
 w= net.IW{1};
 delete(circles);

 plot(w(:, 1), w(:, 2), 'oh');




260   퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 257 =====
 아래 그림은 학습이 완료된 후에 초기의 가중치가 8개의 집단위치로 이동하였음을
알 수 있다．


                  。
                  9


                                                             듀十P




                    L L L l T
                                                        瑋




                  ㅏ
                                                                     ㅓ




                                                             뇨
                                                        ＋솨



                  。  。 。 。 。 。
                  5




                  8  7 6
                                                                           + 아
                                                                 甘
                                                             수                   +
                                                  +
                                                  +
                  4               샅                              ＋
                                                                                 二



                  3
                                                                                                      本
                                                                                                      卄

                                                                                           0 d+
                  。
                  2

                  。
                  1

                  。  ㅑ



                                                                                     .
                  1。  a
                                       1

                                 02   0.3   0.4   0.5    n6          0.7   0.8       0.9          1




 신경망의가중치를 확인하면 다음과 같다．


 w=

  0.4786 0.0384
  0.1927 0.3766
  0.6212 0.7451
  0.6626 0.4818
  0.7780 0.4294
  0.8684 0.7226
  0.9501 0.2561
  0.8850 0.7884


 이제 임의의 입력값에 대해 신경망이 그 입력값을 어느 집단으로 간주하는지를 알
아보기 위해 다음과 같이 시물레이션을 수행해 보자. 아래와 같이 입력값을 (0.6, 0.3)
으로 선정하였다．




                                                                 9 장 자기구성
                                                                        （Self-Organizing) 신경망－261


===== PAGE 258 =====
 p = [0.6; 0.3];
 a = sim(net, p)


 a=
      (4,1)   1


             에서 첫째 항은 가중치 행렬의 4번째 줄을 의미하고, 둘째 항은 입력
 위 결과 값 (4, 1）
값이 한 개이므로 1로 표시되어있다. 따라서, 입력값
                            （0.6, 0,3）
                                     은4번째 집단에 속하며 4
번째 집단의 중심위치는（0.6626, 0.4818) 이다．




2. SOFM(Self-Organizing Feature Maps) J경J

 SOFM은 Kohonen 신경망으로도 불리는데 특징은 많은 입력벡터 패턴을 좀 더 적은
수의 패턴으로 매핑하는 능력을 갖고 있다. SOFM는 경챙학습 신경망과 매우 유사하
다. 경챙학습 신경망은 입력벡터를 분류하는 특징이 있는데 반하여 SOFM은 입력벡터
를 분류하는 것 외에 입력벡터들을 기하학적인 형상정보
                            （topology）
                                     도 제공한다는 점이
차이점이라고 할 수 있다. 아래 그림은 입력벡터에 대한 2차원의 SOFM 신경망을 나타
낸 그림이다．



                                     2-dimensional
                                     Kc升，
                                        onen Layer




                                     lnPut
                                     Layer
                   ［그림 9.2] 2차원의 SOFM 신경망구조




262- 퍼지신경망 제어
            （MaUab/Simulink를 중심으로）


===== PAGE 259 =====
 SOFM도 경챙학습 신경망에서와 같이 숭자 뉴런
                          （winning neuron）
                                         이 1의 값을 가져가
는 것은 같으나, SOFM은 숭자뉴런 자체와 그 인근에 위치한 이웃뉴런도 같이 1의 값을
갖게 된다는 점이 차이점이다．
               이웃뉴런의 가중치
                       （weight）
                              는다음 식과 같이 변경된다．


             iw(q) =iw(q-1)+o (p(q)-iw(q- 1))

             또는

             iw(q) = (1- cx)iw(q-1)+cxP(q)


 여기서 이웃이라고 정의되는 영역 Ni*(d) 는 승자뉴런 1*를 중심으로 반경이 d인 영
역 내에 있는 모든 뉴런을 포함한다．


                        zr (d) = {j,（句 ` d}


 이웃영역의 개념을설명하면 아래 그림과같다. 아래 그림은 뉴런 13을중심으로d可
인 이웃과 d=2인 이웃영역을 표현한 것이다．




               Ni 3(1                         N1：카2


 즉, 왼쪽 그림은 N131, 오른쪽 그림은N132로 표현하면 이웃영역은 아래와 같이 구
성된다．


            N13] = 8 12 13 14 18
            N132= 3 7 8 9 11 12 13 14 15 17 18 19 23




                                   9 장 자기구성
                                          （Self-Organizing) 신경망－263


===== PAGE 260 =====
 1) SOFM 신경망의 구성


 SOFM 신경망의 기하학적 형상
                 （topology）
                          을 구성할 수 있는 함수로는 gridtop, hextop,
혹은randtop 등이 있다．


 gndt아）함수는 신경망의 형상을 사각형의 그리드를 이용하여 구성해 준다．예를 들
어 80개의 뉴런을 가로 8 세로 10의 형상을 다음과 같이 만들어 보자．


 pos =gridtop(8, 10);
 plotsom(pos)


 위 명령어로 다음과 같은 형상이 만들어 진다．



                    .

                     8      ■.I. .U.
                     7
                            口·뻐■口■■
                                ■■■■
                     6

                            urns. ..
                            ■口·
                    '
                    /   4

                   什 닛羹登m
                   m        UI'. ...
                            I5I■■R■
                            issss■s
                     3




                        1   U.".  .
                     0      ■55UU5U       8




 위 그림에서 보는 바와 같이 뉴런이 사각형의 그리드 위에 위치하는 것을 알 수 있다．
 마찬가지로 hextop 함수를 이용하여 똑 같이 80개의 뉴런 형상을 만들면 다음과 같다．
 pos = hextop(8, 10);
 p1otsom(pos)




           （Matlab/Simulink를 중심으로）
264－퍼지신경망 제어


===== PAGE 261 =====
                         A AA"A'A'A'
                         VA
                         AVAVAVAVAVAVAY
                                         AVAVAVAVA
                         !*A                                    VAVAW
                         LYAVAWAVAW
                         WAVAVAVAVAVA
                               A   AWA                    AWA         A         I
                                                                .－나

                           wrm
                         mmm-
                         -1－        뇨－               '-    1-    '－       ▲－'
 같은 방법으로 randtop 함수를 이용하여 뉴런 평면을 만들면 다음과 같다．
 pos = randtop(8, 10);
 plotsom(pos)


 2) 거리함수
       （Di St（그nce Function)


 주어진 한 개의 뉴런에 대한 이웃영역을 정의하기 위해 필요한 거리
                                    （distance）
                                             를 계산
하는 함수로는 dist, linkdist, 그리고 boxdist 등이 있다．
 먼저 dist 함수를 사용한 경우를 살펴보자. 이 경우는 주어진 뉴런에서 이웃뉴런까지
의 실제거리
     （Euclidean distance）
                        를 계산한다. 예를 들어 아래와 같이 3개의 뉴런을 고려
하면，


 p0s2=[0 12; 0 12]
 pos2 =
    0     1   2
    0     1   2


 각 뉴런간의 거리는 다음과 같이 구해진다．



                                                           9 장 자기구성
                                                                  （Self-Organizing) 신경망 265


===== PAGE 262 =====
 D2 = dist@0s2)
 D2 =
        0     1.4142    2.8284
   1.4142          0       1.4142
  2.8284      1.4142             0


 다음은 boxdist 함수를 사용하는 경우이다. 아래의 그림은 gridtop으로 생성한 2차원
뉴런평면이다. 여기서 검은색의 뉴런을 홈 뉴런으로 간주하면 그림과 같이 이웃1, 이
웃2, 이웃3 등으로 구분하는 것이 매우 유용할 것이다．


                       ㅇㅇOㅇㅇㅇ0
                            000
                       ㅇ O O0b ㅇ0
                         O     0ㅇ    ％
                         O     ㅇo        Home neuron
                         OOㅇO0ㅇ
                                         Nei삿，borhood 1
                       ㅇㅇㅇOOㅇㅇ       的
                                         Neighborhood 2
                       ㅇㅇOOOOO
                                         Neighborhood 3


 예를 들어 다음과 같이 6개의 뉴런
                   （가로 2개, 세로 3개）
                                을 생성하자．


 pos = gridtop(2, 3)
 pos=
    0   1     0    1   0     1
    0    0    1    1   2     2


 이 때 각 뉴런간의 박스 거리
                （box distance）
                             는 다음과 같이 계산된다．


 d = boxdistQos)
 d=
    0   1     1    1   2     2
    1    0    1    1   2     2
    1   1     0    1   1     1


266 - 퍼지신경망 제어
             （Matlab/Simulini
                           （를 중심으로）


===== PAGE 263 =====
    1     1   1    0     1      1
    2     2   1    1     0      1
    2     2   1    1     1      0


                                  （linkdistance）
 이번에는 linkdist 함수를 사용하여 각 뉴런간의 링크거리            를 구해보자．


 dunk = linkdistQi,os)


 dlink=
    0     1   1    2     2      3
    1     0   2    1     3      2
    1     2   0    1     1      2
    2     1   1    0     2      1
    2     3   1    2     0      1
    3     2   2    1     1      0


 3) SOFM 신경망의 구조




                         `-         ,   ', ..                    J戶
                                                                  ＇.*


                              Input      Self Organizing Map layer



 SOFM 신경망은 newsom 함수를 이용하여 구성할 수 있다．



예 제 92 0"에서 90"의 사이에 일정한 각도분포로 100개의 점을 다음과 같이 생성해 보자．

 angles = 0:0.5*pi199:0.5*pi;




                                                    9 장 자기구성
                                                           （Self-Organizing) 신경망－267


===== PAGE 264 =====
 그래프로 그려보면 다음 그림과 같다．
 P = {sin(angles); cos(angles)];




 이제 이 점들을 대표하기 위해 10개의 뉴런만을 사용하여 10개의 대표특징을 구하
도록 SOFM 신경망을 학습해 보자. 초기에 10개 뉴런 모두 중심위치인 한 점 (0.5, 0.5)
에 몰려 있다．




                                   小이c겻    ●



                                          W (i,1)



 학습이 진행됨에 따라 가중치 벡터는 입력벡터의 공간을 통해 움직이기 시작한다．
아래 그래프는 학습이 완료된 후에 10개의 뉴런에 연결되어 있는 가중치 값이 보여주
는 점을 표시한 것이다. 이와 같이 SOFM 신경망은 복잡한 특징점들을 간단하면서도
대표성이 있는 특징점을 구해 줄 수 있다．




                                          W(i,1)    1




           （Matlab/Simulink를 중심으로）
268－퍼지신경망 제어


===== PAGE 265 =====
10장신경망제어의응용사례


1. 신경망－PID 졔어기를 이용한 압전구동기 졔어시스템


 1) 신경망－F기D 병렬제어기


 신경망제어기와 PD제어기를 병렬 형태로 연결한 이른바 신경망－Pr') 제어기를 이용
하여 압전구동시스템의 위치제어를 수행하였다．
                       ［그림 10.1］은 켱렬제어기의 구조이다．




               ［그림 10.1] 신경망-PID 병렬제어기



［그림 10.1］에서 병렬제어기의 입력은 압전구동기의 변위와 속도로 주어지고 변위오




                                  10 장 신경망 제어의 응용사례 -269


===== PAGE 266 =====
차 및 속도오차에 의해 PD 제어기가 작동하여 피드백 힘 Fth를 출력하게 된다. 신경망
제어기는 변위와 속도의 입력만으로 무감독 학습방법으로 학습하게 되는데, 학습에 필
요한 목적함수는 PD 제어기의 출력힘인 Ffl,값의 2차 함수로 구성되며 이 값이 극히 작
은 값이 될 때까지 신경망 제어기는 실시간적으로 자가학습
                              （self-learning）
                                            을 하게 된다．
 본 제어기에 사용된 신경망 제어기의 구조는 1개의 입력충과 1개 은닉층 그리고 1개
의 출력충으로 구성된 다층 피드포어드 신경망
                       （multilayer feedforward neural network）
                                                             을
사용하였다．
 신경망 내의 은닉충과 출력층의 각 노드
                     （node）
                          는［그림 10.2］
                                   와 같이 이전의 노드
                                             （node)
로부터 가중치가 곱해진 입력신호들은 바이어스
                       （bias）
                            값과 더해져서 활성함수
                                       （activation
function）
        로 이동된다．
              활성함수는 단조증가
                       （monoton icallymcreas mg）
                                               하며 미분 가능한 함
수를 사용하게 되는데 일반적으로 많이 사용하는 활성함수는 생물의 뉴런
                                     （neuron）
                                            처럼
작용하는 시그모이드 함수
            （sigmoid function）
                             인데 다음과 같은식으로 표시된다．


                              (Sk)        =            1-   ,.

                          f
                                                  1+ e ∼K                (10.1)


 PH）
   제어기의 출력값을 신경망제어기의 학습신호로 사용하고, 오차를 줄이는새로운
가중치 값을 구하기 위해서 신경망 제어기를 설계해야 한다．
 신경망제어압전소자의학습오차에해당하는목적함수를아래와같이정의한다．



                    E (t) =          l可       O
                                              1
                                                   +
                                                   L        八    f
                                                                     2            -



                                                                         (10.2)
                                                                 ,
                                              k
        는t번째 스텝에서의 출력충k번째 노드의 원하는 출력값이고,Ok(t）
 여기서 yKt）                                   는t번
째 스텝에서의 k번째 실제 출력값을 의미한다. 그러나 압전구동기를 수학적으로 정확
하게 표현하기 어렵기 때문에 원하는 출력값Yk(t）
                           를 구할 수 없다. 출력충의 원하는 출
력값은 감독 학습 방법에서 목적패턴을 의미하는데, 이 경우와 같이 목적 패턴을 구할
수 없을 때는 무감독 학습
             （unsupervised learning）
                                   방법으로 학습해야 한다．
 식
 （10.2）
      에서 Yk(t）
             를 구할 수 없기 때문에 식    의 목적함수를 다음과 같은식으로
                           （10.2）
표현하였다．




270 - 퍼지신경망 제어
             （Matlab/Simulink를 중심으로）


===== PAGE 267 =====
                              1
                      E(t)= 去 II Ffb(t) 11 2
                              可
                                                                (10.3)


 위 식에서 Fth(t）
            는 다음과 같다．



         Ffb(t) =Kp(Xd -Xa)+Kd(Xd- Xa)+Kif (Xd -Xa)dt           (10.4)


 식    에서 Xd와 Xd는 압전소자의 원하는 위치와 속도를 나타내고, x , 와 X , 는
 （10.4）
실제 압전구동기의 위치와 속도를 나타낸다．
 식
 （10.2）
      와식（10.3）
             은 같은 속성을 갖는다. 즉 식    에서 학습 오차가 0으로 접근한
                             （10.2）
다는 것은 시스템의 위치오차가0으로 줄어든다는 것을 의미한다. 따라서, 압전구동기
의 위치오차 및 속도오차가 줄어들게 되면 Fth(t）
                            도 0의 값으로 접근하게 되므로 식
(10.3）
     으로 식
        （10.2）
             를 대체할 수 있다. 학습과정 동안에 목적함수 E(t）
                                          를 최소화 하기 위
하여 경사하강법                      을 이용한 역전하 학습 알고리즘을 사용하여
       （gradient descentmethod）
신경망의 가중치 w를 다음과 같은 방법으로 계속적으로 조정하게 된다.［그림 10.2〕는
은닉충과 출력충의 뉴런을 나타내고 있다．




                                           뇨句n止I과口
                                          k번째 l目i｀
                                                 月l




                                          珏m"l1홱口
                                          J번째 긔ㅄ꺼｀끄l




                  ［그림 10.2] 은닉층과 출력층의 뉴런

 식
 （10.3）
      의 목적함수를 이용하여 가중치에 대한 목적함수의 변화량을 구하면 다음과



                                               10 장 신경망 제어의 응용사례 271


===== PAGE 268 =====
같다．
 출력충 노드에 대하여



                            OE      aE    a Sk
                           0Wkj     aSk   Wkj            (10.5)


 과같고, 식
      （10.5）
           에서


                 oE     oE OOk
                                  = (ok- yk)ok (1- ok)
                 aSk    aOk OSk                          (10.6)


과 같다. 따라서


                           aE        .
                   6k=- 二：-=0k "1 -       k)'Yk - 0k)
                           (7캬ㄴ                          (10.7)


와 같다．
    식     에서 Yk - 0k는 신경망의 학습오차이므로 피드백 힘인 Ffb에 비례한다
     （10.7）

고 볼 수 있다. 학습이 잘 진행되면 진행될수록 시스템의 위치오차는 0으로 줄어들고，
Ffb도 0으로 접근하기 때문이다．

 따라서，
    식     는 다음과 같이 바꾸어 표현할 수 있으며，
     （10.7）


                          6k = Ok(1- ok)Ffb              (10.8)


 다음 샘플링 단계에서 가중치의 변화량과 새로운 가중치의 값은 다음과 같은 식으
로 표시된다．


                 A wj (t + 1) = hl6k0j + a A Wkj (t)


                  Wki (t+ i) = wj (t)+ AWkj (t+ 1)


                                은닉충의 노드에서 가중
 위 식에서 1는 학습율이고 α는 모멘텀율이다. 마찬가지로，


272－퍼지신경망 제어
           （Matlab/Simulink를 중심으로）


===== PAGE 269 =====
치에 대한 학습오차의 변화량은 다음과 같이 구해진다．


                  di =E굡= l[6kwkiIoi (1- oJ)                  (10.11)


 그리고, 다음 샘플링 단계에서 가중치의 변화량과 새로운 가중치의 값은 다음과 같다．


                Awii(t+ 1) = i5joi + c△wii (t)                (10.12)


                wii(t + 1) = wi(t) + iwii (t+ 1)              (10.13)


 2) 실험장치의구성


 실험 장치에 사용된 압전구동기는 PT사의 P-245.20 모델을 사용하였고, 압전구동기
의 변위량을 측정하기 위한 위치센서는 LVDT로서 SENSOTEK사의 S5 모델을 사용하
였다. 압전구동기와LVDT의 자세한 사양은〔표 10.1］
                              에 나타나 있다．


                區 10.1] 압전구동기와 LVDT의 사양
                               모델명                       비고
                  P1 (Physik Instrumente)
       압전 구동기                               최대변위량 : /i20 m
                  P-245.20
      압전구동기엠프     Fl E-471.00               0- 1000 V
        센서        SENSOTEK S5
                                            Extation:
                  SA-AC Card,
       센서보드                                 3vo1ts RMS
                  AE325
                                            at 5KHz


        은 본 연구에서 구성한 실험장치의 구성도이다．
［그림 10.3〕                       PC에서는 추종하고자 하
는 궤적의 위치정보를 D/A 변환기를 거쳐 압전증폭기를 통하여 압전구동기를 구동시
키며 압전구동기의 변위량은 압전구동기의 선단부의 판을 통하여 차동변압기
                                      （LVDT)
로 전달된다. 차동변압기는 변위량을 전기적인 신호로 변환하고 센서보드에서 증폭되
어 A/D보드를 통하여 실제 움직인 변위량을 PC로 전달하게 된다．




                                            10 장 신경망 제어의 응용사례 273


===== PAGE 270 =====
                           IYABm쿄      R그


                             !
                                                  十
                                                 g1甘1丑v
                          HvPlT^n,
                                                 B｀
                                                  저ld




                           ［그림 10.31 PZr 구동기의 위치제어 실험장치


 3) 실험및고찰


 압전구동기의 히스테리시스 특성을 파악하기 위하여 피드백 제어기를 사용하지 않
고 실험장치의 압전구동기에 전압을 ov에서 1000v까지 순차적으로 증가하고, 다시
l0oov에서 ov까지 감소시키도록 하였다.［그림 10.4］는 실험에서 사용한 압전구동기
의 히스테리시스 특성을 보여주고 있다．




             ·。흐트료툐0쁘믐즈




                          ［그림 10.4] 압전 구동시스템의 히스테리시스 특성




274- 퍼지신경망 제어
            （Matlab/Simulink를 중심으로）


===== PAGE 271 =====
 따라서，
    히스테리시스에 의한 비선형오차를 보상하기 위하여［그림 10.1］과 같은 신
경망．
  PH) 병렬제어기를 사용하였다. 신경망 제어기 부분은 PD제어기의 출력값에 의
하여 히스테리시스를 포함한 압전구동기의 동적특성을 학습하게 된다. 학습을 위하여
주기가 3초이고 진폭이 3tm정현파를 추종 목표궤적으로 하여 신경망 제어기를 학습
시켰다. 사용된 신경망의 제어기의 구조는 입력충, 은닉충 및 출력층의 노드수가 각각
2개, 8개, 1개로 구성되어 있으며 샘플링주기는 0.005로서 정현파의 1 사이클을 600분
할하여 각 샘플링에서 식
            （10.3）
                 의 값을 최소화하기 위하여 신경망의 가중치를 각 샘플
링주기마다 변경하도록 하였다. 학습오차를 가능한 줄이기 위하여 정현파궤적을 약
200 번 정도 반복하였으며 학습오차율을 약 6% 정도로 줄였다.
 학습이 완료된 후 신경망－P11) 병렬제어기의 계단함수 및 정현파 함수에 대한 추종성
                            제어기의 경우와 그 결과를 비교하였
능을 조사하기 위한 실험을 수행하였으며 일반 P11）
다. 두 제어기의 성능을 비교하는데 있어서 사용된 PD의 게인값은 Kp=0.3, Kd=O.0005,
그리고 Ki=0.6 이다．
［그림 10.5］는 신경회로망－P11) 병렬제어기와 일반 P11）
                                   제어기의 계단함수 추종성능
과 추종오차를 나타낸 것이다. PID제어기만을 사용했을 경우 응답속도는 신경망－PD
병렬제어기 보다 약간 빠른 특성을 보여주지만 초기 구간에서 채터링현상이 발생하였
고, 전반적으로 볼 때 추종성능은 비슷하게 나타났다. 그 다음은 정현파함수의 추종성
능을 비교하기 위한 실험을 수행하였다．




                                5




            m
            oㄴ 으 E ＝ ㄷ·E口o읖끄O
                                괘



                                3



                                2



                                1




                                       15       20      25   30

                                    Time[sec]
                                    (a）변위




                                                     10 장 신경망 제어의 응용사례－275


===== PAGE 272 =====
            .oㄴ 으 트 ㄴ 0
                      ㄴ ㄴ띠。 ㄷ도0mㄴ ㅑ




                                                         15        20   25   30

                                                      Time(see]
                                                    (b)추종오차
         ［그림 10.5] 신경 회로망－F기0 병렬제어기와 일반 RD제어기의 성능비교



［그림 10.6］의 (a）
             는 신경 회로망－PT') 병렬제어기와 일반 PTD제어기의 정현파 함수추
종성능을 나타낸 것이다. 그림에서 보는 바와 같이 사인함수 추종성능에서는 병렬제
어기의 추종성능이 일반 P11) 제어기보다 훨씬 우수함을 보여주고 있다．




                                      四으으E
                                             6




                                          4
                                      。
                                      r       U섶


                                      ㄷ小E。 。m죠． 죠


                                             ?




                                                                  z0




                                                     (a）변위




             （Matlab/Simulink를 중심으로）
276 - 퍼지신경망 제어


===== PAGE 273 =====
           ．。ㄴ。F
                                                                                이
                                                                                ∼洲꽈
                      吐

                      이




           ㄷmE8츠웅否
                                                       w
                      凹

                      m

                      m

                      貂

                      如
                                                           鱗                -         NN+PID
                                                                                      i귀D
                     4l5

                       00                   05                t5       20             z5         3끄
                                                           Time〔se이
                                                      (b) 추종오차
    ［그림 10.6] 신경 회로망－PID 병렬제어기와 일반 디D제어기의 정현파 함수 추종성능



〔그림 10.7〕에서는 신경망－P11) 병렬제어기에서 신경망 제어기와 PH) 제어기에서 나
오는 출력성분 값을 비교하였다. 그림에서 보는바와 같이, 압전구동기의 위치제어는
병렬제어 기내에서 신경망제어기의 출력힘에 의하여 이루어지는 것을 알 수 있다. 그
러나, 외란 및 잡음 등에 의하여 압전구동기의 동적특성이 변하게 되는 경우에 신경망
제어기의 학습상태가 실제 시스템의 상태와 불일치, 즉 학습오차율이 증가하므로 궤적
추종 능력이 떨어지게 되며 피드백 오차가 증가한다. 그러나, 이때 P11) 제어기의 출력
성분이 상대적으로 증가하게 되어 오차를 감소시켜 주므로, 신경망－PID 병렬제어기는
외란 잡음이 존재하는 경우에도 궤적 추종능력이 떨어지지 않게 되는 특성을 갖는다．


                                 40

                                 크5

                                 크0



                           2 2 i t
                                      5

                                      0




                           2 ● 낭 능 ＞ 乏尸그o
                                      5

                                      0

                                   0  5


                                00

                                      00         05   to     15       20        25          ao
                                                           Ti～七E떠a

                      ［그림 10.7] 신경망－PID 병렬제어기에서의 출력성분



                                                                            10 장 신경망 제어의 응용사례－277


===== PAGE 274 =====
［그림 10.8］은 주기가 0.5초인 정현파를 추종목표 궤적으로 설정한 경우의 추종성능을
나타낸 것이다. 병렬제기가 비교적 빠른 주기에서도 추종성능이 우수함을 알 수 있다．


                                     11

                                     10

                                     9




                      ．으으트는mEm0응쁘。
                                         8

                                         7


                                         6


                                     b
                                     r


                                         괘


                                         4
                                         U


                                         h
                                         z




                                                   rune［此이
                                                   (a）변위




            8 흐 E = b山。 ㄷ동可LH




                                             '                  그   a
                                                    rune med1
                                                 (b)추종오차
                                     ［그림 10.8] 주기가 0.5초인 정현파에 대한 추종성능




278－퍼지신경망 제어
           （MatIab/Simulink를 중심으로）


===== PAGE 275 =====
2. 신경망작가조정
         （SELF-TUNIN(키 PID 졔어기틀 이용한 수조 례벨 졔어


 1) 시스템 분석




                                               ㅁ림 10.이 수조시스템


 위 시스템의 운동방정식은 다음과 같다．



                         h
                          (                A1h
                                                                                                  '2gh
                                                             )
                                                                                 (t)   -
                                                                      (Ku
                                                                                           CDav
                                   =
                                                                                                         (t)
                                                       (h)
                                           A                                                                   )
                              ()
                                       =
                             (h)               Amax,
                                                                            ,Amin
                         A
                                                                 hm         ax




 위 식에서，

  u(t) : Electrical potential input of water pump (0< u(t)< 12V)

  h(t) : Level water in the tank (cm)

  A(h) : Horizontal section of the tank (cm2)

  hMx : Maximum water level

  Amx, A＇刊n: Maximum and minimum section

  k: Proportional ratio (depend on the power ofpump)
  a: Section ofdrain way (cm2)

  g : Accelerationof gravity 981 cm/sec2
  CD : Drainage ratio




                                                                                                   10 장 신경망 제어의 응용사례 -279


===== PAGE 276 =====
 해석을 위해 사용된 파라메터는 다음과 같다．


                          ［표 10.2] 수조시스템에서 사翌 파라메터 값
                    Parameters                                     Value
                           hn日<                                   50cm
                           A      「日x
                                                                 200cm2

                           싸nnn
                                                                 100cm2
                                  a                                1cm2

                                  k                           300cm3/sec
                                  CD                                0.6



 선정된 파라메터값을 사용하여 수조시스템의 모델을 Matlab/Simulink를 이용하여 아
래 그림과 같이 구성하였다．




                                                                           〈
                                                                           卜
                                                                                 洲
                                                                                0ath

      【ph】
                                                  x   ---*
                                                                               H그：)
                                                                                 H
                                            +                Int..'. t이
       0n1
                    ^dd


                                   `/U

                                      이，




             凶                                    →｛츠＞→巨고

                                                                                       를
                                           5q唯야

                          K1               F口，                    G.t.1




                                                                                       Water tank s,1戚em




                 ［그림 10.10] MatIab/Smuink를 이용한 수조시스템의 모델링


 위 블록선도에서 입력값은 전압이고 출력값은 수조면의 높이이다．




280          （Matlab/Simuhnk를 중심으로）
      퍼지신경망 제어


===== PAGE 277 =====
 2) 신경망을 이용한 자가조정 F기D 제어기




                                                                minear「기D
          > +                                                                          Water tank
  Reference ".-'                                               ntroller using -                          >
                                                                                        system
                                                              eural network     u(t)                    Response


                            Derivative



                                                   ［그림10.께 제어시스템구조


 P11) 제어기는 구조가 간단하고 성능이 우수하므로 산업현장에서 많이 사용되고 있
는 제어기 시스템이다. PID 제어기의 게인을 설계
                           （선정）
                              하는 방법은 Ziegler-Nichols 법，
   （root locus) 등을 이용하기도 한다. 하지만, 일반적인 PD 제어기는 한 번 게인
근궤적법
이 정해지면 작동 중에는 게인이 고정되어 있으므로 플랜트 내부의 비선형 요소나 외
부로부터 유입되는 외란 등의 문제가 발생할 때 제어 성능이 떨어지는 단점이 있다. 따
라서, 시스템의 비선형 문제나 외란 등의 문제를 대처할 수 있는 지능적 제어기의 필요
성이 높아지고 있다. 본 연구에서는 신경망과 Pu) 제어기를 결합한 지능제어기가 제안
            （water tank）
되었다. 제어대상은 수조          의 높이를 조절하는 것이다. 제안된 신경망 PD 제
어기 시스템은［그림ㅔ와 같다．


                   e    D
                        ~
                                                   .Kp
                   ei
                    '
                            - /“一‘黔＼ Ki
                            '~,                랖         '
                                                                                          u   (t)   》

                                  \，∼二＞"




                            卜7Thr                        Kd
                                  ..   .   7

                                  ［그림 10.12] 신경망 RD 제어기시스템



 그림에서 보는 바와 같이 시스템의 3 입력은 오차값, 오차값의 미분, 그리고 오차값
의 적분이다. 이 3 입력은 비선형 활성함수인 시그모이드 함수 내부로 들어가게 된다．



                                                                               1《〕장 신경망 제어의 응용사례 -281


===== PAGE 278 =====
시그모이드 함수는 다음과 같이 정의된다．



                              f (x) = 2(1- e" ' Y8)
                                      Yg(1+ e∼ XYg)


 위 식에서 Yg는 시그모이드 함수의 곡률형태를 결정하는 상수이다．본 연구에서는
Yg= O.S를 사용하였다．
              위 회로에서 보는 바와 같이 PID 제어기의 게인은 신경망의 가
 （weight) 값으로 설정되어 있다. 신경망은 일반적으로 사용하고 있는 역전파
중치                                          （back
propagation) 알고리즘을 이용하여 학습오차를 최소화하는 방법을 사용하였다. 이와 같
은 튜닝방식으로 시스템의 비선형을 적응하도록 적절한 제어 게인값이 튜닝된다. 출
력층에서 있는 시그모이드 함수로 들어가는 입력신호는 다음 식과 같다．


               sum(t) = 1 (t)e (t)+ .K (t)e (t) + Kd(t)ed(t)


 위식에서，
                                e (t) = ref(t) - h(t)



                                                                                                      (t)
                                     6     (t)                      Jep
                                                        =
                                     6出）                                                         (t
                                                                          de
                                                            =
                                 ed
                                                                                       dt
                                                                                                            )
                                                 (t)        =




 여기서，
    r/7t）
        와h(t)는각각기준신호와 수조의 높이응답을 나타낸다. 최급하강법
                                          （gradient
descent method）
              을 이용하여 다음과 같이 신경망의 가중치를 계속 업데이트 한다．


                                                                                                                              OE
                         k                             1)
                                                                                                                    刃，
                               (t+                              =              k
                                                                                           (t)                  －
                                                                                                                               尸




                          k          (t+               1) =                        k   '   (t)                  -        a，
                                                                                                                         01s;j
                                                                                                                              주
282          （Matlab/Simulink를 중심으로）
      퍼지신경망 제어


===== PAGE 279 =====
                                                                                                           〃』aE
                                                          1)
                                                                                           (t)       ‘
                                                                      =
                                            (t+
                                                                          kd
                               kd
 여기서，                                 일반적으로 학습율의 값이
    'rI , tli' Tid는 경험적으로 결정되는 학습을 값이다．
크면 학습은 빨리 되지만 학습성능의 좋지 못하고, 반대로 학습율의 값이 적으면 학습
성능은 좋아지지만 학습시간이 많이 걸리는 단점이 있다. 신경망을 학습하기 위한 학
습오차값은 다음과 같이 정의된다．



                                                                 12
                                                                          。
                                                                          ，
                                                                          r
                                                                               >
                                                                               l
                                                                               ^e                                  t
                               E (t) =
                                                                                                 ,
                                                                                   ∥
                                                                               ㅡ
                                                                                   r
                                                                                                 r

                                                                                   ·
   （chain mie expansion）
 체인룰                         다음과 같은 식이 유도될 수 있다．
                       을 이용하여，


                               oE                         aEah on aSurn
                               os                         oh au a8urn ok


                               OE                         oEoh atl Osu7n
                               ok                         a／乙 Ou Osurn 8k


                               aE                         oE a/1 Ou a8tI7r乙
                               Okd                        oh au Osurn Okd


 그리고 다음의 관계식을 고려하자．


            oE
               =-(ref(t)-h(t))=-e (t)
            oh


                      On
             Osurn
                           -        f
                                        '         (surn
                                                                (t)
                                                                          )

                                                          ;                                                    ;
                                                                                                                       km= ed
                                                                                                         (t)
                                                    (t)
                                                                                                     e1
                      k
                                                                                       -                                        (t)
                                    e
             Osurn。
                                                              OsumOk2                                              Osu。




                                                                                                                    10 장 신경망 제어의 응용사례   283


===== PAGE 280 =====
                        oh           i 8           h(t)-h(t- 1)
                        Ou           △q            u(t)-u(t-1)


                                                   4e- snm ' 匕
                         ., . .
                        / tsumJ ==                                                                        2
                                                        e_         ' "m           '
                                                                                            Y)
                                             (i+
 위 식들을 결합하면 비선형 파라메터에 대한 적응공식이 다음과 같이 유도된다．




         (/(！
           『1)=，小）
         kp(t+1)       -「1 6小）6간）
                 zk (t)-T1e(t)e (t)1(,1+e
                                       ',4e"1：二‘．
                                             _sum.Y9)
                                                 =,)2h(t)-h(t-1)
                                                    2U(t)_U(t_1)
                                       4e ' " m ' 】｀                                                                                         h(t)-h(t-1)
         k (t+ 1) = k (t)- r1e (t)e渺）
                                            sum .                                                                                   )2
                                                                                                                                             u
                                     I1+ e
                                                                                                      -                    Y
                                                                                                                                                                                   1)
                                                                                                                                                                       (t-
                                                                                                                                                               u
                                                                                                                                                       -
                                                                                                                                                 (t)
         ' r, ㅗ , ,－卜 r,ㄴ∼ r, ,. r, ,                                             4e- sum ' y,                                               h(t)-h(t-1)
         "d \-' 】 ㅗ /    ' 'd "-'1      'Ip'- p " "-d ' "1
                                                                        (1+                      e
                                                                                                 e-            SU In   '       Y)        2   神）            -       u         (t-        1)
 간단하게 표현하기 위해 아래의 조건이 성립한다고 가정한다．


                          oh          Lih           h(t)-h(t-1)
                                                                                                                       constant
                          au-
                                                                                                          1)      =
                                                                                      (t-
                                                                              u
                                                                    -
                                                             (t)
                                                    n
                                      △u-
 3) 시물레이션 및 검토


 수조에 대한 동적방정식과 1절에서 언급된 파라메터들을 이용하여 Matlab/Simulink
기반으로 시물레이션 프로그램을 작성하였다. 전체 제어회로는［그림 10.13］
                                         에 나타나
있다. 제안된 비선형 신경망PD 제어기의 제어성능을 검토하기 위해 일반적인 PH) 제
어기와 Fuzzy 제어기와 성능을 비교하였다．
                        제어기의 추종궤적은 다단스텝
                                      （multi step)
및 정현파 신호
       （sinusoidal signal）
                         을 사용하였다．




284   퍼지신경망 제어棚atlab/Simuhnk를 중심으로）


===== PAGE 281 =====
                                                     >                                    卜〔그
 R.   ng                                 $1tU11t10
 s p.
                       .nl油t휘PlD

 sm1   12




                                   ㅁ림10.13] Control diagram




                                                                                -
                                                                                    口UH




                                                                                     P

            1M
                                     r




                 -－→          d dt
                          0        輓V*
                                                                                     d
                                                           ㅌ＇ㄲb·d4.d
                                                         M^TLㅅ8 Fun沚ion


                  [그림 10.14] Sub-function of nonlinear PlDcontrol


        （M미ti-step) 추종 테스트
 4) 다단 스텝


 추종 테스트에서의 성능과 오차는［그림 10.15］         에 나타나 있다．
                           와［그림 10.16］       그림에
                       （self tuning) 능력이 있기 때문에 PIP 나
서 보는 바와 같이 제안된 제어기는 자가조정
                                 또한 30초가 지난 시점에
血zzy 제어기 보다 목표에 수렴하는 속도가 빠르게 나타났다．
서 기준 궤적이 계단적으로 감소하는데, 이 영역에서도 제안된 제어기가 빨리 기준궤
적에 수렴하는 것을 알 수 있다．




                                                                          10 장 신경망 제어의 응용사례 -285


===== PAGE 282 =====
                                                                                                                    沁化化化侄m訂一訃。 e4右욘岩m
             25-                                                                                  \
                                                                                                  \
                                                                                                  U

  으 泌흐bH堊＞
               沁        -




                                              出出겡
                        n



                恪


ㄷ
一
                        -




             10-
                      叫
                            P-
                                                                             -- F贓태좨m
                                                                                IO* 8- F거D
                                                                              -(hk태也.님 F거D
                                                                            ㅣ- Hzzyk쟈Cm11rdier

                                             10           a                              20       40
                                                      Time (sec)
                                      [2림 10.15] Response of the system                                                                     ll림 10.16] Error of the system


                    6끄
                                                                                                                            1.4-
                    5.5
                                                                                                                           12-
                    5.0→




               4 4 3 3 2
                            輟
                            U
                                                                                                             모              1.0-
                                  q


                            0
                                  -




             웃 錢 얻 견 區 쿄 뇨 溜노
                            닛汁낱
                              亡
                            ，니                                                                                             。.6-




                                  J77― 。
                            。
                                                                                                             휼0.                 4-
                            仄U                                                                                             02-

                      z     。
                                                                                                                           0.0-
                      1     ,
                            u
                                                                                                                          -02
                                              10          a                                                                             0        10               a
                                                        The (s)                                                                                                 The (s)

                                                              (a)                                                                                     (b)
                                                                    쿄눕mㄴㄴ짠띳나里．里玉一
                                                                                    .U
                                                                                    1




                                                                                    。
                                                                                    ㅓ1




                                                                                    5
                                                                                    。




                                                                                              }                    才｝                       及）              奴
                                                                                                        ㄲne（하

                                                                                                       (c)
                                                        (a) K parameter, (b) K parameter, (c) Kd parameter
                                                    [2림10.17] Controller parameters of nonlinear PlO algorithm:




             （Matlab/Simulink를 중심으로）
  286－퍼지신경망 제어


===== PAGE 283 =====
 4) Sinusoid 궤적 추종 테스트


 삼각함수 형태의 기준 궤적을 다음과 같이 생성하였다．


                                          ref(t) = 5sin (o.it) + 15


 추종 테스트에서의 성능과 오차는 r그림 10.18］
                            과［그림 10.19］
                                      에 나타나 있다. 이 경
우에서도 제안된 제어기는 P11〕나 fuzzy 제어기 보다 목표에 수렴하는 속도가 빠르게
나타났다.［그림 10.20〕
              는 시간에 따른 PID 제어기의 게인이 튜닝되고 있는 모습을 보여
주고 있다．

                               쑈

                               四

                               炤

                               羽




               小
               듕一丕
                 ＞m도至＞
                               M

                               俚

                               柏

                               8

                               6

                               4
                                                                    -- R1」 f. tㅈi저
                                                                       Nbmflean거D
                                                                       Hlzzy logic ccnbTjflel
                                                                       QDnvention레 PID
                               0                     1       '       ~   '       【
                                   0                40              벼〕           玟）          1o0
                                                         tirre(sac)
                                       [그림10.18] Response of the system




                         -2-
             l ㅑㅏ十1十긔＂錨님拗긔H身，   j j


                         柏 ㅓ
                             ，
             4   咨   8        坦   侮



                小듕나노ㅂ


                     띠
                     ㄴ
                                                                      一… '*，뱁hi可PtD
                                                                        山伯1鷺a님1거D
                                                                         Fu y
                               0
                                              10             茨｝              簾
                                                         lin-e (司

                                        [2림 10.19] Error of the system


                                                                              1《〕장 신경망 제어의 응용사례 -287


===== PAGE 284 =====
        秘

        朗

         朗




  ㅉ m 聊 槌 仍 M
                                                                                                             0.9




                                                                                              모bH컫띤鍵쑈요m느긍莖
                                                                                                             0.
                                                                                                             α7
                                                                                                             0.6
                                                                                                                  脯




  2拓尸욀띤8多논e＾杜
            。左

         仕

      1.0                                                                。
                 10   沁   笠）   40      5. m                        7n    a        簾   1m                           a   is   겼）   30   40      駐） 庶）   70   80   었） 703
                                    Tirre (s)                                                                                              Tine (히
                                                         7.8

                                                         t6

                                                         14




                                        잦눕g卜丙， 8。＞斗＇도倦
                                                         t2

                                                         t0

                                                    《1B

                                                         0.6
                                                          M

                                                     (12

                                                         00

                                                    q2-
                                                               0    10       a)   珊    40     驪》              a
                                                                                            1hㅜe（히

                           [그림 10.20] Controller parameters of nonlinear PlO aigorithm


 5）결론


 본 연구에서는 신경망을 이용하여 비선형 PH) 제어기의 게인을 실시간적으로 튜닝
하여 기준궤적의 추종성능을 향상할 수 있음을 보였다. 제안된 제어 알고리즘은 수조
의 높이를 제어하는 시스템에 적용되었다. 제안된 제어기는 일반PH) 제어기, Fuzzy 제
어기와 성능을 비교하였는데, 제안된 제어기는 self tuning 능력이 있기 때문에 PID 나
抛zzy 제어기 보다 목표에 수렴하는 속도가 빠름을 알 수 있었다. 제안된 제어 알고리
즘은 비교적 간단하고 계산시간도 많지 않기 때문에 비선형 특징을 갖는 시스템을 실
시간 제어에 유용하게 적용될 수 있다. 아래 프로그램은 제안된 제어기의 MATLAB 코
드이다.




288 -- 퍼지신경망 제어
              （Matlab/Simulink를 중심으로）


===== PAGE 285 =====
%%% Nonlinear self tuning P11)by using neural network code:
function [y, a, b,c]= fcn(p,I, d)
persistent kp ki kd sum


% Create initial value of PB)
if isempty(kp)

  kp = 2 ;
  ki= 0.9;
  kd= 0.1;
  sum = 0
end


% Declare the variable
net-inl=[0 011';
net-outi =[0 0]';
d_f_hid =[0 0]';
net in2 =0;
nup = 0.01; % Learning rate of kp
nui = 0.01; % Learning rate of ki
nu-d = 0.01; % Learning rate of kd
Y = 0.5 ; % factor of output function
out =0;
sum = 0 ·，
del = 1 ，·

sum = p*kp+j*kj+d*kd;
out = 2*(1_exp(_1*sum*Y))/(Y*(1+exp(_sum*Y)));


% Update P11) controller parameter

kp=kp+nup*p*p*4*exp(-1*sum*Y)/(1+exp(-1*sum*Y))/2*del;




                                                     10 장 신경망 제어의 응용사례 289


===== PAGE 286 =====
  iflcp < 0
    kp= 0;
  end

  ki = ki+nu-j*p*j*4*exp(-1*sum*Y)/(l+exp(-1*sum*Y))/\2*del;
  ifici < 0
    ki= 0;
  end
 kd = kd+nu d*p*d*4*exp(-1*sum*y)/(1+exp(-1*sum*Y))f2*de1;
  ifkd <0
    kd =0;
  end

 %Output control signal

 y = out;
 a = kp;

 b =ki;
 c == kd;




290 - 퍼지신경망 제어
             （MatIab/SimuIink를 중심으로）


===== PAGE 287 =====
찾아보기




(A)
Abs 블록 / 23                                            C언어 / 50

Accept Data /207, 209, 221
activation function! 158, 173, 175, 178,180-482, 270   (D)
adapt / 246, 257                                       Data Type! 188

Add MFs /86                                            DC모터 / 113-116,204

Add variable /82                                       Dead-zone / 21

AND/ 58-61, 67                                         defuzziflcation!47, 148

ANFIS /223, 225-236, 238-240                           defuzzified!58

ANFIS Editor GUI!234-236, 238                          Derivative block / 15

ANFIS 구조 / 223                                         Display/ 23, 30, 33

ANFIS의 학습 / 228, 233, 234, 239                         dist!265, 266


                                                       (E)
(B)
back propagation training / 166                        Edit / 82,86,87,238,239

boxdist /265,266                                       Elman / 신경망
                                                       Embedded MATLAB Function! 30-32

(C)                                                    Export!93, 196

C 프로그램 / 33, 287
dass / 256                                              (F)
Clock/ 23, 26                                          feedforward neural network / 159, 270

competitive learning / 255                             File! 85, 93, 238, 247

configuration / 11                                     FIS Editor!76, 78, 80, 82, 84, 85, 93, 94, 101, 238

Constant / 30                                          fixed-step! 12

Continuous!14, 16, 19                                  flag! 34-40

Create! 188, 189, 289                                  function! 15, 30-34, 39-41, 51, 69, 119, 133, 139,
                                                              148, 158, 172, 173, 175, 177-182, 189, 229, 231,



                                                                                             찾아보기 291


===== PAGE 288 =====
      238,265, 270,289                                 (L)
Fuzzy Rule Editor / 107                                Laplace / 15-17
flizzification / 47                                    Layer! 157-160, 173-175, 178, 180-482, 184, 189,
fuzzy / 43,47,69, 71, 72, 74,76, 82,90,93,94,96,              223-225, 244, 255, 270
      98-401, 103-405, 107, 109, 110, 111, 116, 145,   least squared error/ 226
      152,223,225,233, 234,284,285,287,288             library! 8, 9, 204, 219
Fuzzy Logic Controller / 93,98,99, 105                 linkdist /265, 267
Fuzzy Logic Toolbox /93                                local mininium!168
Fuzzy-PD/100, 101
Fuzzy-PID!103-l0S, 109-ill                             (M)
                                                       Mamdani!58, 78
(G)
                                                       Math operation!22, 23
Gain/93,98                                             matlab! 7, 8, 30-33, 39, 50, 63, 74-76, 82, 85, 90,
gam block! 14                                                 93, 96, 101, 105, 133, 135, 171, 172, 176, 178,
Generate Traini끄g Data / 206, 288, 221                        182, 183, 185, 187, 188, 192, 195, 196, 204, 218,
GENFIS1 명령에 /229,231                                          228, 232,234, 235, 236, 244, 256, 280, 284, 288
gradient descent /189, 282                             membership value /43, 223
gridtop / 264, 266                                     MEX파일 / 33
                                                       MF type! 86
(H)                                                    Model Reference Control /204, 205, 208, 209
hextop / 264                                           Model Reference Controller/ 205, 206
hidden layer! 158, 160, 178, 182                       MUX /90
Hopfield 신경망／243, 248-253                              M파일 /33, 34, 39


(I)                                                    (N)
If-Then / 46, 49, 53, 67                               Network Architecture /206
inference mechanism! 46                                Network Weight!158
Inputs / 188, 190                                      NewData/ 188
Integrator block/ 15                                   NewFIS!85
                                                       New Network!188
(J)                                                    newc / 256, 259, 260
Jang / 223, 225                                        newelm!244, 246, 247
                                                       newhop!249, 250, 252
(K)                                                    NNPredictive Controller/ 219, 220
Kawato / 201, 202                                      nntool! 187, 195, 196
Kohonen!257, 262                                       Node!158, 174, 181, 223,270
Kohonei더子칙 / 257
Kohonen -i경망 / 262                                      (O)
                                                       ode / 12



             （Matlab/Simulink를 중심으로）
 292- 퍼지신경망 제어


===== PAGE 289 =====
Off-line 학습 / 200                                       sinks! 10, 17, 50
0K button / 208                                         sizes! 34-36, 40, 41
0n-line 학습 / 200, 201                                   SOFM!255, 262-264, 267, 268
overshoot / 90, 93, 127                                 sources!9, 17, 30
                                                        Start / 17, 20, 222, 232
(P)
                                                        State-space block! 17
P1제어기 / 115, 123, 127                                   stats! 31-33
P113/ 89, 90, 93, 101, 103, 104, 108-111, 201, 269,     steepest descent method / 166
      270, 275-277, 279, 281, 282, 284, 285, 288, 289   Step /10, 12, 17, 27, 73, 74, 174, 181, 214, 216,
P1D제어기 / 89, 90, 93, 101, 104, 108, 110, 111,                            233, 284, 285
      269, 270, 275-277                                 Subsystem / 26, 204, 205, 220
Plant Identification / 206, 207, 221, 222               Sugeno!58, 59, 61, 78, 85-88, 223, 234, 238
plotsom / 264, 265                                      Sumblock! 14
Predictive Control! 211, 219,220, 222                   supervised training!162
purelin! 184-186, 196, 244                              Surface / 71, 72, 80, 84, 88, 107, 136, 146
                                                        sys/ 34-41
(R)
randtop /264, 265                                       (1          ')
Recurrent Neural Network / 243                          tansig! 184-186, 189, 196,244, 246, 247
keference Model! 206                                    Targets! 188, 190
Rule Viewer / 135                                       TDNN 신경망 / 213-215
Rule-Base / 46, 47, 49                                  ToDisk!93
Rules /87, 233,238                                      Toolbox GUT!75, 76, 82
                                                        topology /262, 264
(S)                                                     train!178, 190, 207, 209,221, 239
satlins / 249                                           Train Controller!209
Saturation/ 21, 98                                      TrainNetwork!190, 207, 221
scope! 11, 13, 17, 20, 27, 90, 98                       Training Data!206, 208, 221, 231, 232, 234
Self-Organizing / 255                                   Transfer fcn / 16
Self-Organizing Feature Maps / 262                      Transfer function / 15, 189
Self-Tuning Fuzzy / 94, 96, 98, 99, 100, 101            T-step 예측제어 / 16
S-Function! 33-36, 38-41                                tuning /93, 96, 97, 288, 289
Sign 블록 / 22
sim /245, 246                                           (U)
simulation!7, 11, 17, 20, 39, 71,210,222                unsupervised training! 拓2
simulink / 7-10, 13, 16, 17-23, 25-30, 32-35, 41,       User-Defined Function!30, 34
      89, 93, 98, 118, 122, 123, 204, 208, 210, 219,
      220, 222, 280, 284                                (     '1)
Sine Wave! 186                                          vals!32, 33



                                                                                            찾아보기 293


===== PAGE 290 =====
variable-step / 12                                        194, 196, 206, 221, 244, 249, 251, 252, 255-257,
View 메뉴 / 80, 84                                          260, 263, 264, 265
                                                   뉴런간의 거리 / 265
       "0
(
window /9, 76, 82                                  (t)
winner/ 255, 257                                   다충구조／159, 160, 163
work/93, 96                                        도달점 /248-251, 253
                                                   도립진자／47, 48-50, 52
(X)
                                                   동적시스템 /7, 14, 46, 162, 199, 200, 214
XOR/ 187, 188, 190
x-Y 그래프 / 23                                       (n)
                                                   라이브러리 / 9,10,30,34
(Z)
                                                   로봇/ 144-147, 149-155, 192, 197, 203-205, 208, 288
Zieg1er-Nichols법 / 281
                                                   (n)
（기타）                                               메인프로그램 /69, 176, 182

 1-step 예측제어 / 216                                 멤버쉽 함수／51-53, 59, 65, 66, 76, 78, 80, 81-83,
2차시스템 /89, 100                                            90, 91, 102, 105
                                                   면적중심법 / 56
(-          i)
                                                   모델링/ 14, 21, 33, 129, 199, 202, 203,280
가중치값／96-98                                         모델예측제어 /211, 2四
가중치벡터 / 161                                        모멘텀율／172, 272
감독학습 / 162, 200                                    모터제어 / 119
거리제어시스템 /75, 82                                    목적함수／212, 215, 217, 270, 271
거리함수／265                                           미분방정식 / 12, 14, 15, 17, 18, 20
경로제어 /151, 152                                     미분블록 / 15
경챙층／255
경챙학습／255-260, 262, 263                              (H)
경챙학습신경망 / 256                                      바이어스／161, 172, 178, 179, 184, 251, 252, 255,
구속조건 / 64                                                 257, 2銘, 270
근궤적법 / 281                                         변화율／15, 49-55, 57, 98, 106, 116, 117
기준모델 적응제어기 / 202                                   병렬분산처리 / 157
                                                   블록선도／13, 46, 115, 118,214,280

  0-             )                                 비감독학습／162, 200,201
내부운동／149, 150, 153                                 비선형식 /21, 37
노E/ 158, 160, 161, 163-165, 167, 169, 170, 206,    비선형연산 / 161
             225, 227, 270, 272, 275               비퍼지화／47, 58, 70, 148
뉴런 / 157, 158, 160, 172, 177-179, 184, 185, 189,   비활성화／255




  294                       （Matlab/Simulink를 중심으로）
                     퍼지신경망 제어


===== PAGE 291 =====
(A)
                                                                압전구동기 /269-271, 273-275, 277
상대속도 / 82                                                       여유자유도／144, 149, 151-153
상숭속도 / 127                                                      역기구학／144, 149
상태공간／17, 19, 20                                                 역전파학습 / 166
상태변수／17, 18, 20, 36, 39, 40                                     연산／14, 46, 161, 226
샘플링시간／12, 36, 39                                                연속시스템 / 14
서브시스템 / 26-29                                                   예측성능／219
성눙함수／149, 150, 152, 184, 189, 211, 219                          예측제어기 /211, 212,215, 217-219
소속값／43-45, 58, 61, 223-225                                      오차값I46, 49-55, 57, 96-100, 116, 117, 119, 12!,
스케일링 / 169                                                             139, 162, 164-470, 174, 177, 181, 183, 201,
스텝응답 / 17, 20, 21, 26, 89, 90, 93, 94, 98-100,                         214-217, 226, 227,239, 240, 281, 283
            102, 103, 110, 111, 115, 116                        은닉층 / 158, 160, 163-167, 170, 172, 173, 177-479,
스프링－질량－댐퍼 / 15, 17, 20                                                 184, 185, 189, 196, 206, 221, 243, 244, 270-272, 275
 숭자／255,257,263                                                 이동로봇／191, 192, 197
시그모이드 함수／161, 270, 281, 282                                     이득블록 / 14
시냅스 / 157                                                       이웃뉴런 / 263, 265
시물레이션 / 12, 13, 23, 24, 26, 33-35, 42, 69, 71,                  이차함수／85
            74, 75, 109, 115, 118, 133, 136, 138, 141, 144,     인공신경망／157, 158
            176, 178, 182, 191, 222, 250,251, 258, 261, 284     일반집합／43
 시작시간 / 12                                                      일반화눙력 / 159
 신경망／159, 160, 162, 163, 168, 179, 183-185, 187,                입력변수 / 15, 34, 35, 49, 53-55, 57, 59, 60, 61,
            189, 190, 195, 196, 199-202, 206, 208, 211-215,            65-67, 75-83, 90-92, 96, 98, 99, 101, 102, 104,
            218, 219, 243, 248, 249, 255, 258, 262, 269, 270,          105, 116, 119, 133, 139, 147, 148, 237
            275,277, 284, 284                                   입력신호／9, 10, 158, 161, 204, 214, 270, 282
 신경망모델／211-215, 219                                             입력층/ 158-161, 172, 177, 179, 189, 270, 275
 신경망 역제어기 /200, 201
  신경망 예측 제어기 /218                                               (z)
  신경망자가조정 / 279                                                 자가조정 / PD 281
  신경망 제어기 / 199, 200, 270, 275, 277                             자기구성 신경망／255
  신경망－PD / 269                                                  자동차의 Simulink 모델 / 25
      신경망，
         P11〕병렬제어기 /269,275, 277                                자세 최적화／149
  신경망병렬제어기 / 201                                                자세제어 /48, 63
  신경망의 구조생성 / 183                                                     4* 도/ 27, 127-131, 133, 136-138, 141-444, 149,
  신경망의 학습／162, 163, 167, 17!, 177. 183, 187,                           151-153
            190, 191, 195, 206, 212, 246,257, 272               장애물/ 144, 146, 147, 150-155, 191-193
      신경망제어기 /200, 201, 209,210, 269, 270, 277                  장애물 우회 / 144, 147, 153-155
                                                                적분블록 / 15
      (0)
                                                                적응제어기 / 168, 202
      안정제어기 /201                                                전건부／58,223,225



                                                                                                         찾아보기 295


===== PAGE 292 =====
전달을 / 144                                                        (51)
전달함수／15--17, 20. 184                                             파라메터 / 12, 13, 34, 65, 115, 127-429, 168, 205,
전산해 / 12                                                                     220, 222-227, 232, 236-240, 280, 284
제어곡면／80, 84                                                      패턴분류／257
제어입력벡터 / 211                                                     퍼1I 43-55, 57-61, 63, 65-72, 74-89, 92, 93-408,
제어평면／72, 107, 108, 116, 118, 120, 122                                        113, 116-127, 133-140, 143, 147-149, 152, 153,
종료시간 / 12                                                                    223, 224, 229, 230, 233, 234, 236-239
주 제어기 / 119                                                      퍼지* / 59, 60, 63, 79, 80, 83, 84,87, 88, 117, 135
중심평균법 /56, 57                                                    퍼지 시스템 /43, 46, 48, 53, 58, 83, 84
지역 최소점 / 168                                                     퍼지집합／43-45, 53-55, 65, 67, 69, 70, 89
질량．
  스프링 카트 모델 / 27                                                 퍼지 툴박스／75, 85, 107
집합／43, 44, 51, 53, 65                                            퍼지변수／44, 224
                                                                 퍼지제어 /63, 68, 74, 80, 89, 119, 127
(,         )                                                     퍼지제어 곡면／68, 80
차량모델 / 127                                                       퍼지제어기 /46-49, 53, 54, 57, 65-72, 74, 75, 78-84,
초기화/ 8, 34, 35, 39, 76, 77, 82, 169, 237, 238, 257                           93--99, 101, 102, 105, 106, 108, 116, 118-123, 127,
최급강하법 / 166, 168                                                             136, 137, 140, 143, 144, 147, 148, 152, 153
최소자승법 /226                                                       퍼지함수／45, 59-61, 70, 116, 133, 135, 138
추론부／46, 47                                                       퍼지화／47, 58, 70, 148
출력변수 / 15, 35, 49, 54, 55, 58, 59, 65-67, 75,                    편집창／16, 17, 20, 27
           76, 78-80, 82, 83, 90-92, 96, 97, 101, 104-107,        프로그래밍 /50, 63, 171, 187
           116, 119, 133, 138, 139, 140, 147, 148                 피드백회로 / 15
출력신호／10, 120                                                      피팅 / 85, 230, 234
출력충/ 158, 160, 163-467, 170, 172, 173, 177-479,
           184, 185, 189, 196, 206, 221, 243, 244, 270-272,275          (ㅎ   )
출력힘/ 49, 50, 53-57, 67-71, 135, 270,277                            학습 子칙 /257
충 / 158                                                             학습속도／168, 178
                                                                     학습용 데이터 / 195, 206-209, 221, 229
 (?        )                                                        학습을／167, 168, 260, 272, 283
 카트－도립진자 시스템 / 48                                                       합산부／158, 160, 161
 카트－역진자 시스템 / 64                                                        합산블록／14, 15
클래스／258                                                                 현가시스템 / 127
                                                                        형상정보／262
     (E)                                                                활성함수／158, 160, 161, 169, 172, 178, 184. 189.
 테이블／66, 107                                                                 194, 196, 244, 249, 255, 270, 281
 튜닝용퍼지제어기 /99, 101, 121, 122                                             활성화／76-78, 85, 86, 255
 특이점 / 144                                                               회기신경망／243
                                                                        후건부／58, 225




      296              （MatIab/SimuIink를 중심으로）
                퍼지신경망 제어


===== PAGE 293 =====
              값 13, 000원




 - 1
                   3550




9 788978 682824
  ISJ나 978-89-7868-282-4
