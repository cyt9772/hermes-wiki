---
title: Visual Basic
created: 2026-10-15
updated: 2026-10-15
type: concept
tags: [programming, windows-api, object-oriented]
sources: [raw/books/vb6-introduction.md]
confidence: high
---
# Visual Basic (VB)

Microsoft의 이벤트 기반 개체지향 스크립트 언어. 윈도 GUI 개발을 비주얼(시각) 방식으로 — 폼 위 컨트롤을 배치하고, 발생한 이벤트에 코드를 연결하는 — 가능하게 하며, 1991년 등장해 VB6(1998)까지 데스크톱 애플리케이션 표준 중 하나였다. VB.NET 이후 C#으로 계보를 잇는다.

## 개체지향 + 이벤트 기반 구조
VB 프로그램은 개체(객체)의 집합이다. 폼(Form) 자체도, CommandButton·TextBox·ListBox·Timer 등 모든 컨트롤도 각각 하나의 인스턴스. 코드의 실행 흐름을 개발자가 설계하는 것이 아니라 **사용자 액션이 일으키는 이벤트**가 프로시저를 부른다.

> "클래스(CommandButton)의 인스턴스(Command1)가 만들어지고, 그 인스턴스에 Click 이벤트를 연결해 동작을 정의한다" `[raw/books/vb6-introduction.md]` p.~35

핵심 문장:
```vb
Private Sub Command1_Click()
    ' Command1 버튼이 클릭될 때 실행된다
    Label1.Caption = "안녕"
End Sub
```

## 데이터형 체계 (VB6, 4장)
| 형 | 메모리 | 범위 |
|----|--------|------|
| `Integer` | 2 byte | −32,768 ~ 32,767 |
| `Long` | 4 byte | 32비트 정수 |
| `Single` | 4 byte | 7자리 부동소수 |
| `Double` | 8 byte | 15자리 부동소수 |
| `Currency` | 8 byte | 통화/고정소수 |
| `String * n` | 1+n byte | 고정길이 문자열 |
| `String` | 가변 | 최대 32,767자 |
| `Byte` | 1 byte | 0~255 |
| `Boolean` | 2 byte | True/False |
| `Variant` | 가변 | 어떤 형 또는 nothing(Empty/Null) |
| `Object` | 4 byte | 개체 포인터 |
| `Type` 사용자 정의 | 구조체 | 레코드용 |

- `Variant`은 `Nothing`, `Empty`, `Null`, `IsNull`, `IsObject`, `IsNumeric`, `CStr`/`CLng`/`CDbl` 형 변환에 주의할 것 `[raw/books/vb6-introduction.md]` p.157-161
- 사용자 정의형(구조체): `Type Person / Name As String *20 / Age As Integer / End Type` — 랜덤 액세스 파일의 레코드로 사용 `[raw/books/vb6-introduction.md]` p.~340

## 제어문 (6장)
`If … Then … ElseIf … Else` / `Select Case` / `For … Next` / `While … Wend` / `Do … Loop Until|While` / `Goto`+라벨 / `Stop` / `Exit Sub|For|Do` / `End`

## 프로시저 (7장)
```vb
Public Sub  프로시저명([ByVal|ByRef] 인자 As 형, …)   ' 반환값 없음
Public Function 함수명(…) As 형                        ' 반환값 있음
```
- `ByVal` 값 전달 / `ByRef` 주소 전달(기본값 — 인자가 호출부에서 변경 가능)
- 모듈(Module)과 표준모듈: 프로젝트 단위 함수를 공용으로 제공한다

## 이벤트 vs 서브 vs 함수 (3장 디버그)
- **서브(Sub)** : 절차, 반환값 없음
- **함수(Function)** : 값을 돌려줌 — `x = Math.Max(3, 5)`
- **이벤트** : 컨트롤/폼의 상태 변화(Click, Change, Timer, Form_Load…)에 자동 발동

## 파일 입출력 (12장)
### 순차 액세스
```vb
Open "c:\mydata\sfile.dt" For Output As #1
Print #1, "첫째 행"
Print #1, "1234567890"
Close #1
' 읽기
Dim s As String
Open "…\sfile.dt" For Input As #1
Do While Not EOF(1)
    Line Input #1, s
    List1.AddItem s
Loop
Close #1
```
### 랜덤 액세스(등장 길이 레코드)
```vb
Type Person
    Name As String * 20
    Age  As Integer
End Type
Dim p As Person
Dim L As Integer: L = Len(p)
Open "db.dt" For Random As #1 Len = L: ' …
```

## GUI 컨트롤 (8장)
| 컨트롤 | 용도 |
|--------|------|
| Form | 창, 모든 컨트롤의 부모 |
| Label | 정적 텍스트 (Caption) |
| TextBox / Multi-line | 입력 (Text) |
| List / ComboBox | 선택 목록 |
| Command / Image | 버튼 (Click) |
| CheckBox / Option | 선택 / 단일 선택 |
| Frame / Group | 컨트롤 묶기 |
| Timer | 일정 간격 이벤트 (Interval ms) |
| ScrollBar | 스크롤 값 |

## 학습 경로 및 한계
- **장점**: 비주얼 빌드 + 빠른 프로토타이핑, Windows API 직접 호출, VBA(엑셀/액세스 매크로)와 문법 공유
- **단점**: C/C++·Java 등 현대 언어 대비 성능/모듈화 한계; VB6은 2008년 EOL(마지막 업데이트), VB.NET·C#으로 대체
- **관련**: VBA(Office 매크로), C#(VB.NET 계보), Win32 API

## 관련 개념
- [[vb6-introduction]] — 이 문서를 정리한 입문 교재
- [[linux-essential-utilities]] — gcc·make·gdb 등 컴파일·디버깅 생태계
- [[unix-advanced-programming]] — 시스템 호출 중심 절차지향 프로그래밍
