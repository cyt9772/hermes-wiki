---
source_url: "/run/media/yutae/Data/STL 방법.pdf"
ingested: 2026-11-15
sha256: 951e0a1485f56133fc4dc92fa9ecfc16018f8bb6b9d604bae506ccc64113b038
type: raw-source
method: text-extract
---

# STL 방법 (raw source)

> **출처:** USB 원본 PDF (`/run/media/yutae/Data/STL 방법.pdf`, 로컬 참고용 — git commit 불포함)
> **방법:** 내장 텍스트 레이어에서 `pdftotext -layout`로 추출 (OCR 불필요)
> **쪽수:** 61쪽 | **추출 텍스트:** 47 KB
> **주의:** 원고는 scan/레이어 추출로 영문·숫자·특수자 일부 아티팩트가 있을 수 있음. 해석 시 원본 PDF와 대조.
> OCR 추출 디렉터리 `raw/books/stl-method.ocr/`는 git-ignored (로컬 참고용만) — 본문은 아래에 내장.

## Book metadata
- **Title:** STL 방법
- **Pages (PDF):** 61
- **Source:** STL 방법.pdf
- **Domain:** Programming · 프로그래밍 (예상)
- **Ingested:** 2026-11-15

## Extracted text (all 61 pages)


===== PAGE 1 =====
［사외 뱐출 가능］




    에 ㅅ티 엘 방 법

 STI Note


===== PAGE 2 =====
Modern C++
  include legacy




    SW아카데미


===== PAGE 3 =====
                             도L차
                             -I- ▼1




1.   문법

     ●    pair

     ●    auto

     ●    template

     ●    range based for loop

     ●    initializer list

     ●    memset

     ●    string library

     ●    function object

     ●    lambda




2.   STL Iterator


===== PAGE 4 =====
                           모ti.
                           -1' `1




3.   STL Container

     ●   vector / deque

     ●   list

     ●    set/ map

     ●    unordered_set / unordered_map

     ●    stack I queue / priority_queue




4.   STL Algorithm

     ●    sort

     ●    lower_bound / upper_bound

     .    swap / max / mmn

     ●    max element / mmn element

     ●    for each

     ●    find / find-if


===== PAGE 5 =====
pair
       S    pair<T, U> p : pair<string, int> p = {"pair", 2};

       ●    p.first, p.second로 인자 접근 : p.first = "pair",
            p.second = 2

       ●    operator(==, !=, <, >, <=, >= ) 정의되어 있음
            == : first. second가 둘 다 같다．
            < : first가 작다 / 같으면 second가 작다．

       ●
       S    pair
              「 생성
                 。。 :. make_pair(a, b)

       ●    #include<utility> kontaine
                                     「 사용시 생략 가능）

auto
auto a = 1

auto &b = a;

   ●       compile time에 자동으로type 완성

   ●       함수의「eturn type 지원

   ●       함수의 매개변수에는 지원 안됨   （c++14 기준）
           -> template으로 대체 사용 가능

   ●       iterato
                 「 등 type이 복잡해지는 경우에 유용하게 사용


===== PAGE 6 =====
template
    ●    여러 자료형을 하나의 함수J 클래스로 사용 할 수 있게 만들어 놓은 틀

    ●    template, class keyword는 완전히 동일한 기능

 mnt sum(int a, mnt b) { return a + b; }

 short sum(帥ort a, short b) { return a + b; }

 double sum(double a, double b) { return a + b; }




 template <typename T>
                                4
 I sum(T a, I b) { return a + b; }




 형식 매개 변수는 여러 개 사용 가능하다．

 template <typename I, typename U, typename V> class

 template{};




range based for loop
mnt arr[5] = { L2, 3,4戶 }

-for (auto x : arr) { x+--; }

                    「 변경 불가
 copy : 객체크기만큼 복사J ar

 수행 후 arr : 1,2, 3,4戶

for (auto& x : arr) { x++; }

 reference : 8 byte 복사，ar「 변경 가능

 수행 후 arr : 긱3,4, 5,6


===== PAGE 7 =====
Initializer list
template< class I >
class initializer_lists

initializer_list<int> il{ 1,2,3,4,5 };
for (auto x : ii) cout << x << " r;


    ●    기본 생성자 및 대입연산의 인자로 initializer_list type이 제공됨．

    ●    따라서J 모든 객체에 대해 braced-mnit-list {} 사용 가능

set<int> s{ 1,2,3,4,5 };    // 1,2,3,4, 5
5 = { 5, 6 };               // 듸6
vector<pair<int, int>> v{ {1,2}.{3,l} ,{2,5} };




memset
    ●    비트 단위로 값을 변경한다．

    ●    e으로 초기화 시 사용하면 유용

    ●    #include<string.h> or *include<niemory.h>

    ●    mnt arr[100]

    ●    memset(arr, 0, sizeof(arr)) : ar
                                        「 모든 값 0으로 변경


===== PAGE 8 =====
string library
SIL Containe
           「에서는 string 문자열 사용

#inc1ude<string>

char cstr[100] = "abcedfg" ;
string str = cstr;           : char 문자열을 대입연산자로 string에 담을 수 있음
string str2

str == str2                 : '＝볍' 연산자로 string 문자열 비교 가능

str[index]                  : 배열 인덱스 접근 가능

str. size()

str . c_str()               : char type으로 변환

str. insert(int pos, 문자열）

str. substr(pos, len)       : pos 위치부터 len 길이의 substring 반환

stoi(str)                   : 시작부터 digit 문자까지 정수로 반환


===== PAGE 9 =====
함수를 인자로
    ●     function object

    ●     lambda



STL에서 굉장히 중요하게 다뤄지는 내용




Function object(functor)
    ●     function call operator (）
                                  를 정의하여 함수처럼 사용 가능한 객체

    ●     인라인 치환

    ●     상태를 가질 수 있다．

    .     다른 함수의 인자로 전달될 수 있다．



struct Sum_n {
    mnt operatorO(int n) {
        mnt sum = 0;
        for (mnt I = 1; 1 <= n; i++) sum   +=
                                                1;
        return sum;
    }
}sum_n;

sum_n(n);
cout << sum_n(10);          II 55
cout << Sum_n{}(le);        II 55
cout << Sum-nQ(10);         // 55


===== PAGE 10 =====
Predefined Functor : comparison operator
     ●    class template

     ●    sti에서는 아래 세가지 comparison functor를 사용한다．

     ●    data typeOㅔ 각각 ==, >, < operator가 정의되어 있어야 한다．

     1.   equal_to

          template<class T>
          struct equal_to {
            bool operatorQ(const T& lhs, const T& rhs) const {
              return lhs - m5;
              }
          }
     2.   less

          template<class 1>
          struct less {
            bool operatorQ(const T& 가1S, const T& rhs) const {
              retum 가15 < ms;

           }}
     3.   greater

          template<class 1>
          struct greater {
            bool operatorQ(const T& lhs, const T& rhs) const {
              return 가匹 > rhs;
              }
          }
형태

     1.   less<T>             : class

     2.   less<T>()            : function
          less<int> Q(1,1) = false
          less<int> Q(l, 2) = true

     3.   less<T>{}           : function


===== PAGE 11 =====
Predefined Functor : hash
template< class Key >
struct hash;

    ●    Requirement

         ■   key값에 대해 size_t type의 hash 값을 반환한다．
             (size_t == unsigned long long)

         ■   ki, k2가 같다면 hash<Key>(kl) == hash(k2）
                                                 이어야 한다．

         ■                                        인 확률이 매우
             kl, k2가 다르다면 hask<Key>(kl) == hash(k2）
             적어야 한다．

    ●    Specialization 되어 있는 type

         U   기본 primitive type (mnt. long, long, char, bool,
             double, float, ...)

         U   string type

         1   pair



※ specialization : 특정 data type에 대해 별도의 동작을 정의해준다．
                    즉J 각 type 특성에 맞게 hash function이 적절히 구현
                    되어 있다．


===== PAGE 12 =====
lambda
       -function object을 사용하면 되기 때문에 필수 문법은 아니다



[captures](parameters) -> return type { body };
           ①         ②                ③      ④


      ① : scope 내의 외부 변수를 reference or value로 참조 가능


      ② : 매개 변수（없으면 생략 가능）


      ③ : 생략 시 body의「etur'n type으로 결정


      ④ : 함수 본문




captures 활용

[1 : 외부 변수 사용 x

[&]
           : scope 내의 모든 외부 변수들을 레퍼런스로 가져온다．

[=1
           : scope 내의 모든 외부 변수들을 값으로 가져온다．

[     =J   &X그 : x 什eference 참조） -    나머지 (value 참조）

[x,
           &y, &z] : x (value 참조） -   y,z 什eference 참조）

※ 전역변수는 기본 캡쳐 모드
               （aJ=）를 사용해야 한다．


===== PAGE 13 =====
examples

 auto sum_n = [](tnt n) {                  1/ mnt -> auto 선언 가뇽

 tnt sum = 幻

 for (tnt I = j ; I <= n; i++) sum += I;

 return sum;

 };
 sum_n(10);                                II    result : 55



 tnt arr[S]{ L2, 3,4戶 };



 auto increase = [&] {

 for (mnt I =    ; I   < 5 ; i++) arr[I] +-i-;

 };
 increase( ) ;                             // arr : 긱3,4, 5,6


===== PAGE 14 =====
STL Iterator




    SWO바데미


===== PAGE 15 =====
Iterator


포인터와 상당히 비슷하며 컨테이너에 저장된 원소들을 참조할 ㄸ［1 사용되는 객체


"    Input Iterator

                  Forward Iterator
    ios眈eam
                                        / Bidirectional nerator
               forwad list
               unordered set                 list
               unordered_map                                RandomAccess Iterator
                                             set
                                             map            ve￡tor
                                                            deque
                                                            string
                             =
                      1it=
                                         reversejterator    尸inter




operati이l

       ●      distance(v.beginO, it) : 두 iterato
                                               「 사이의 거리 반환


       ●      advance(it,               3) : it 를 다음 3 번째 iterato
                                                                「로 이동


       ●      new_it = next(it,                     3) : new_it 에 it 다음 3 번째 iterato
                                                                                   「 저장


       ●      new_it             = prev(it,         3) : new_it 에 it 이전 3 번째 iterato
                                                                                   「 저장



       random access iterator : 0(1)

              advance(it,               3)          ->        it     += 3

              next(it,             3)                >        it + 3

       otherwise : 0(n)


===== PAGE 16 =====
reverse iterator


  ●        반대 방향으로 진행하기 위한 iterator adaptor

   ●       Bidirectional Iterato
                               「부터 제공

   ●       container의 beginO, end(）
                                  는 iterator type 반환

   ●       conta1ner21 rbeginO, rendO는 reverse_iterator type 반

   ●       +reverse_it로 역방향 진행


                                               ①）
           v.begin(J                                            和       (J
                                                                    v.end




  !
v.rendO                                                   v.rbeginO

回쟁방향翠I

   iterator
       for (auto it = v.begin(]; it != v.endD; ++it){
            1* process */
       }
@) 역방향순회

   iterator
       for (auto it = v.endQ; it             != v.beginQ; ) {
              -it.
             /* process */
       }
   reverse iterator
      For (auto it = v.rbeginQ; it               1= v.rendQ; ++it) {
               /* process */
       }


===== PAGE 17 =====
iterator invalidation


                                                          ㅅ싸ㄱ，＂『1Pr t0n 카몬               ＾仕甘 era`U
                                                                                                 『· ar·
                                C 0n ta nr,1            tel at0r `   4 eVe, elite..    ite'1t허｀         'erer· m
                                                                                                               《·흖       c ..dfflo..키fy
                                                         , 〕 」`           ,:.d`           V,1.d7           vaIid?


                                                                     N.




  5숀quen〔 e c ntamer `                                               N0                            N.

                                                                                      Ye.. ext.Pt .voe.d 이口vent渗
                                                           N.




                                    .,', t
                                 m'I t ,P t
                                    건’ JP


  Ut,., dered associative                                                                                            Insertion Caus.d n.h.,h
                                1             t   L 1

       ' Ufltaltc.,s        an:客.', jP
                                     『.itac.ap                                        vet eㄸep' em5eJ 毓emenh51             'i. m ca尉




)* list, set, map

      ●        iterato
                     「가 가리키는 element가 지워지지 않는 한 항상 유효하다．

      ●        iterato
                     「를 기록하여 효율적인 활용이 가능하다．


===== PAGE 18 =====
STL Container
    - Sequence -




     SWO바데미


===== PAGE 19 =====
vector


    ●         dynamic array

    ●         random access iterator

                                                                        Corn미exity
                                                   Space            0(n)
               capacity : 할당 받은 크기
                                                    Search          이n)

                                                   Insert           이n)
                                                   Delete           0(n)
                                     j
                                                   Pu針iback         이1)
        size : 사용 중인 크기                             P아a_back        0(1)

                                                   M恤ation          아n)




원소 삭제


1. erase()                                    2. 마지막 element로 덮어쓰기

        0(n)                                       · 0(1)

        순서 유지                                      · 순서 유지 x

v.erase(v.begin() + 2)                        0 v[2] 냅 v.backQ;
                                              ②v.pop_backQ;

0         2      3   4   5                     0            2   3   4     5
                一        一
                                         ①（
                                               0            5   3   4     5
0   1     3          5                   ②（
                                               0     1      5   3   4


===== PAGE 20 =====
vector - 주요 문법

template<

    class T,
    class Allocator = std: :allocator<T>
> class vectorU




vector<T> V                                  size t : unsigned kng long



iterator v.begin(), v.end()
iterator v.rbeginQ, v.rend()
T v[int idx]
bool v.empty()
void v.clear()
size_t v.size()
size-t v.capacity()


I v.-front() , v.back()


void v.push_back()
void v.pop_back()


iterator v.insert(iterator pos, T x)
iterator v.insert(iterator pO5, mnt count, T value)
iterator v.insert(iterator pO5, iterator first, iterator last)
 : 처음 입력된 element 의 iterator 반환


iterator v.erase(iterator pos)
iterator v.erase(iterator first, iterator last)
 : 마지막 지워진 element 의 다음 iterato
                              「 반환


===== PAGE 21 =====
vector - example


 vector<int> v;
for (mnt i = 1; i <= 5; i-i-+) v.push_back(i);


// 12345
for (mnt i = 0; i < v.sizeQ; i++) cout << v[i] << " ;
for (auto x : v) cout << x << " ;
for (auto it = v.begin0; it ！쑈 v.endQ; ++it) cout << *it << "       ;


II   5 4 3 2 1
 -for (auto it = v.rbeginQ; it != v.rendQ; ++it) cout << *jt << "       ;


 v.insert(v.begin0, 6);               /1 6 1 2 3 4 5
 v.insert(v.endQ, 7);                 II 6 1 2 3 4 5 7
 v.insert(v.begin() + 3, 8);          II 6 1 2 8 3 4 5 7


 v.erase(v.begin() + 1);              /16      283457
 v.erase(v.end() - 1);                II 6 2 8 3 4 5
 v . pop_backO;                       // 6 28 34


 v[2그 = 0;                            II 6 2 0 3 4
 V. empty() ;                         II 0


 v.sizeQ;                             II   5
 sort(v.beginQ, v.end0);              // . 2 3 4 6


===== PAGE 22 =====
mmn_element Q, max_elementQ, minmax_element()
template< class Forwardlt >
Forwardlt min_element( Forwardlt first, Forwardlt last );

template< class Forwardlt >
Forwardlt max_element( Forwardlt first, Forwardlt last );

max element

                [first, last) 구간에서 comp 기준으로 가장 큰 element

                iterato
                      「 반환

                comp 가 없다면 operator< 기준

mm    element
                max_element 와 형식J 사용방법 동일

minmax element
                pair<Forwardlt, Forwardlt> 반환

                first: mmn iterator, second: max iterator




for_each()
template< class InputIt, class UnaryFunction >
UnaryFunction for_each( InputIt first, InputIt last, UnaryFunction F );

: [first, last〕구간의 모든 element에 대해 f를 수행한다．

:    UnaryFunction

vector<int> arr{ 1,2,3,4,5 };
 for_each(arr.begmnQ, arr.endQ, [](int x) { x++; });
// 1J 2J 3J 4, 5
 for_each(arr.beginQ, arr.endQ, [](int& x) { x++; });
II   2, 3, 4, 5, 6


===== PAGE 23 =====
swap(), max(), min()

void swap(T a, T b)                  : a, b 의 값을 바꾼다．

T max(T a, I b)                      : operator< 기준 큰 값

T max(T a, I b, Compare comp)
: comr〕 기준 (Compare requirement 만족）

  min(T a, I b)                      : operator< 기준 작은 값

I min(I a, T b, Compare comp)
 : comp 기준 (Compare requirement 만족）

pair<T,I> minmax(T a, I b)
: operator< 기준 (first： 작은 값J second：큰 값）

pair<I, I> minmax(T a, T b, Compare comp)
: comp 기준 （Compare requirement 만족）


===== PAGE 24 =====
lower_bound Q, upper_bound()
template< class Forwardlt, class I >
For'wardlt lower_bound( Forwardlt first, Forwardlt last, const T& value );


template< class Forwardlt, class I, class Compare >

Forwardlt lower_bound( Forwardlt first, Forwardlt last, const T& value, Compare comp );




lower bound
                 [first, last) 구긴k게서 comp 기준으로 value 보다 크거나 같온

                 첫번째 element iterato
                                   「 반환

                 auto it = lower_bound(arr.beginQ, arr.end0, 5);
upper_bound
                 [first, last) 구갠게서 comp 기준으로 value 보다 큰 첫번째

                 element iterato
                               「 반환

                 auto it = upper_bound(arr.begin(), arr.end0, 5);


- comp 명시되지 않았을 때는 operator< 기준

- 정렬된 구간에서만 사용

                 binary search       I반, Randomlt : 0(log n), 0Uierwise :

                 0(n)
                 comp 기준은 (:ompare requirement 필요없이

                 BinaryPredicate 만 만족


===== PAGE 25 =====
Algorithm Library 주요 함수


    ●    sort
    .    lower_bound, upper_bound
    .    swap
    ●    max, min, minmax
    ●    max_element, mmn_element, minmax_element
    ●    for each
    ●    -Find, find i-f
    ●    count, count_if
    ●    remove, remove_if etc.



sort()
template< class Randomlt >
void sort( Randomlt first,   Randomlt last );


template< class Randomlt, class Compare >
void sort( Randomlt first,   Randomlt last, Compare comp );




 [first, last) 구간을 《:omp 기준에 맞게 정렬

: comp 를 명시하지 않으면 operator< 기준에 맞게 정렬

: bool comp(const I &a, const I &b)

: Compare requirement 만족 필수


7守ctor<int> ar叫 瓦3, -2,l, -4 }'                  … ……1… m 小
sort(arr.beginO, arr.endO);                     7! -4, -2, 1, 3, 5
sort(arr.begin() , arr.endQ, greater<int>Q); // 5, 3, 1, -2. -4


===== PAGE 26 =====
function f를 설정하는 방법


   1.   naive function

   2.   function object

   3.   lambda



ex) vector를 절대값 기준으로 오름차순 정렬하는 경우



   1. na工ve function
        bool comp(int a, tnt b) {
            return abs(a) < abs(b);

        }

   2. function object
        struct Compare {
            bool operator() (const tnt a, const tnt b) const{
                 return abs(a) < abs(b);

            }
        }comp;


   3. lambda
        auto comp = [](int a, tnt 느 ) { return abs(a) < abs(b); }


   sort(arr, arr+n, comp);


===== PAGE 27 =====
Algorithm Library

    ●   주로 컨테이너 반복자
                  （배열 주소 값）
                          로 다양한 작업을 수행하도록

        도와준다．

    ●   반복자 없이 값으로만 수행되는 함수도 있다．

    ●   function을 인자로 설정해주기도 한다．

    ●   range는 항상 더:jrst, last）
                              이다．last 미포함



함수의 형태는 대부분 아래와 같다．

●   func(iterator first, iterator last, T value)
    : find, count, lower_bound, upper_bound
.   func(iterator first, iterator last)
    : sort, max_element, mmn element
●   func(iterator first, iterator last, function f)
    : for-each, find_if, count_if, sort
●   func(T a, T b)
    : swap, max, mmn
●   func({ initializer list })
    : max, mmn


===== PAGE 28 =====
STL Algorithm




    SWO타데미


===== PAGE 29 =====
priority_queue
template<

      class 1,
      class Container = std::vector<T>,
    class Compare = std::less<typename Container::value_type>
> class priority_queues


      ●     heap으로 구성 가능

      ●     항상 top만 접근 가능

      ●     완전 이진 트리

      ●   모든 부모 노드가 자식 노드보다 우선 순위가 높다．

      ●     compare 기준으로 정렬했을 때 가장 오른쪽 element를 top으로 반환




                                  口－        pq.topD

                        ［꾀 ［三
                       ［괴 □［引 ［끄
                       □□［i그
                            .cm0x-pq example>



miority－甲ieue<T> pq
priority_queue<T, vector<T>, Compare> pq
pq = {}II clear
void pq.push(x)
void pq.pop()
I     pq.top()
mnt   pq.size()
bool pq. empty()


===== PAGE 30 =====
queue
template<


      class T,
    class Container = std::deque<T>
> class queue;



      ●     First Input, First out

      ●     항상 什ont, back만 접근 가능



                                      驀蛾蒻雛醬鸞甚驢




    q.push(5)                            q.pop()
            -0
                                             -




      q.front()                        q,back()

queue<T> q
q = {}II clear
void q.push(x)
void q.pop()
T      q.lront()
T      q.back()
mnt    q. size()
bool q.empty()


===== PAGE 31 =====
stad《
template<


      class 1,
    class Container = std: :deque< T>
> class stack,




      ●     Last Input, First out

      ●     항상 top만 접근 가능




                         Push
                                (5   '   %    /s.
                                                     popO
                    s.
                                         \\
                                                    s.top()




5tad( <T> St
St = {} 7/ clear
void st.push(T)
void st.pop()
I      st.top()
mnt    st.size()
bool st.empty()


===== PAGE 32 =====
STL Container
    Adaptors




    SW아카데미


===== PAGE 33 =====
Adaptors


sequence container 활용하여 stack, queue, priority_queue interface

제공

     ●   Iterato
               「 제공 x

     ●   중간 원소 접근 x

         ■    stack : top only
         ■    queue : front, back only
         ■    priority_queue : top only


●    stack : 거의 쓸 일이 없다．

●    queue : BFS에서 주로 사용

●    priority_queue
     ■   빈번한 삽입J 삭제 속에서 위 '1 순위를 구하는 경우에 사용

     ■   set, map에 비해 활용성이 떨어진다．

     ■   정렬 기준 가장 오른쪽 원소가 top으로 올라온다．
     ■   default : max pq


===== PAGE 34 =====
     2.   Hash : functor
          KeyEqual : functor
struct Data { mnt x, y; };
struct MyHash {
     size_t operatorO(const Data&      a)   {
          return a.x * 10000 + a .y;

     }
｝…
struct MyEqual {
     bool operator()(const Data& 1, const Data& r) {
          return 1.x 一 r. x && 1.y == r. y;

     }
};
unordered_set<Data, M쌘ash, MyEqual> s;
unordered_map<Data, int, 吻川a轍J MyEqual> m;


     3.   Hash : lambda
          KeyEqual : lambda
struct Data { mnt x, y; };
auto myhash = {](auto& a) {
     return a.x * 10000 + a.y;

};
auto myequal = {](auto& a, auto& b) {
     return a.x == b.x && a.y == b.y;

};
unordered_set<Data, decltype(myhash), decltype(myequal)>
s(BUCKET_COUNT, myhash, myequal);
unordered_map<Data, tnt, decltype(myhash), decltype(myequal) >
m(BUCKET_COUNT, myhash, myequal);
lambda를 쓰는 경우 생성자로 보내주어야 하는데＇

이 때 첫번째 인자로 bucket 개수
                    （hash table size）
                                    가 필요하다．


===== PAGE 35 =====
      3.    Lambda
struct Datr: { lot X, y; };

auto LambdaComp =［〕(corist        a& ., const Dat &   ) {
      return a.x l= b.x ? 爺 .x < b.x : a.y < b.y;

};
set<Data, decltype(LambdaComp) > s(LambdaComp);
niap<Data, mnt1 decltype(LambdaCoep) > m(LambdaComp) ;
priority∼queue <Data, vector<Data>, decltype(LambdaComp) >
pq (LambdaComp);




Hash, KeyEqual

      1.   Hash : Functor
           KeyEqua1 : equal_to operator(==) overloading
struct Data {
      mnt x, y;
      bool operator==(const Data &r) const      {
           return x == r. x && y == r. y;

      }
};
struct FunctorHash {
      size_t operatorO (const Data&    a)   {
           return a.x * 10000 + a.y;



 }r
unordered_set<Data, F山化torHa탉＂ 5;
unordered_map<Data, int, FunctorHash> m;


===== PAGE 36 =====
Compare


          1.      Operator Overloading
struct Data {
          mnt x, y;

          bool operator<(const Data& r) const {
                  return x   느 r. x ? x < r'. x : y < r. y;

          }
};
bool operator<(const Data& a, const Data& b) {
          return a.x != b.x ? a.x < b.x : a.y < b.y;

}
set<Data> s;
map<Data, jot> m;
priority_queue <Data> pq;
                                  반드시（乳 ② 중 한 개 사용



          2.       Function Object
     struct Data { mnt x, y; };

     struct FunctorConip {
              bool operatorO(const Data& a, const Data& b) {
                   return a.x != b.x ? a.x < b.x : a.y < b.y;

              }
     };
     set<Data, FunctorComp> s;
     map<Data, int, FunctorComp> m;                닉
     priority-. queue <Data, vector<Data>, FunctorComp> pq;


===== PAGE 37 =====
set, map, unordered_set, unordered_map
                                                         '       kev


           set                     unordered set

                                                                 key, value
                                                                  operatorfl 제공
                                                                 ［】접근시．
           map                     unordere&map                   default 값
                                                                          （0〕 으로 자동 insert


    Red-Black Tree                 Hash Table            공죵
    O(logn)                        O(1+a)                 오로지 key값 기준으로 검색
'   Compare                '       Hash. KeyEqaul         key값 변경 불가, 필요시 삭쟤
    우선순위 값《〕r 정렬된 정보               일치하는 정보 검색 특화          후 삽입
    필요할 때 유용




Custom Guide
Compare
     ●     5et
     ●     map
     ●     priority queue


Hash, KeyEqual
     ●     unordered set
     ●     unordered map




                                    Class Template

            ! type              perator
                               《）             function       lambda      requirement
            1
                               overloading    object
 Compare     bool (T』 T)       <             0           0               Compare

             size t (T)        x             0               0           Ha針1

KeyEquel     boot (1, T)                     0           0               BinaryPredicate


===== PAGE 38 =====
examples

string id 부여 (1 ` n)

unordered_map<string, int> htab;
mnt hcnt = 0;
mnt getld(char key[]) {
    if (htab[key]) return htab[key];
    return htab[keyJ = ++hcnt;

}

bigint id 부여 (1 ` n)

unordered_map<int, int> htab;
mnt hcnt = 0;
mnt getld(int key) {
    if (htab[key]) return htab[key];
    return htab[key] = ++hcnt;

}

(0,0) ` (20,000, 20,000) 좌표 사용 상황 파악을 위한 hash

using ull = unsigned long long;
unordered_set<ull> htab;

ull getKey(int x, mnt y) { II    key 값 생성

    return x * 20001 + y;   // 최소 20,001 진법

}
htab.mnsert(getKey(x, y)); II 등록

htab.count(getKey(x, y));   // 사용 여부 판별

htab.erase(getKey(x, y));   // 등록 해제


===== PAGE 39 =====
unordered_map - 주요 문법



unordered_set<T, U> htab
unordered_set<T, U, Hash> htab
unordered_set< T, U, Hash, KeyEqual> htab


iterator htab.beginQ, htab.end()


U htab[T xl                  : x 가 등록되지 않은 상황이면

                                default 값
                                        （0）
                                          으로 등록

bool htab.empty()
size type htab. size()
void htab.clear()
size_type htab.count(I x)
iterator htab.find(T x)
void htab.reserve(int n)


size_type htab.bucket(T x)
size_type htab.bucket_count()
size_type htab.bucket_size(int x)


pair<iterator, bool> htab.insert({ T key, U value })
void htab.insert(iterator first,    iterator last)


iterator htab.erase(iterator pos)
iterator htab.erase(iterator first,   iterator last)
size_type htab.erase(T x)


===== PAGE 40 =====
unordered_set - 주요 문법


unordered set<T> htab
unordered set<T, Hash> htab
unordered_set<T, Hash, KeyEqual> htab


iterator htab.begin(), htab.end()
bool htab.empty()
size_type htab.size()
void htab.clear()
size_type htab.count(T x)
iterator htab.find(T x)



void htab.reserve(int n)              : n 이상의 2" 로 bucket count 설정



size_type htab.bucket(     x)         = x 값의 bucket 번호

size-type htab.bucket-count()         : hash table bucket 수

size_type htab.bucket_size(int x)     : ）《 bucket 의 element 수



pair<iterator, bool> htab. insert (   x): { 등록돈J iterator, 성공 여부｝

void htab.insert(iterator -First, iterator last)


iterator htab.erase(iterator pos)

: P05 의 다음 iterato
                 「 반환

iterator htab.erase(iterator first, iterator last)
: 마지막으로 지운 element 의 다음 iterato
                              「 반환

size_type htab.erase(T x)             : 성공 여부 0, 1


===== PAGE 41 =====
                                                                                      ㅐaSh Table




                                                % bucket count
                Hash
  key -        Function
                             뺙hash value ■■뺙 bucket

           : class Ha삯】
           default: hash<Key>
            t spec祉izatioㅍ 되어 별도로 구현해줄 필요 없는 type
                 ' primitive type: m1t. long long, chat; bool, ...
                 ' string
                                                                                                        probing 기준

                                                                                                                       :class KeyEqual
                                                                                                                  default : equal to'cKey>
unordered set                                            unordered_map                                            't Key type에 operator= 정의 필요
template<                                               te呻late<
     ctass Key,                                             class Key,
     dass Hash = std: 十ash<Kev>.                            C1ass 1,
                                                            class Hash = std: :hashckey>,
     ciass Iceybqua1 = sta: : equaLmto<Icey>,
     cl.ass Allocator = std: :aflocator<Key>            ,
                                                          , class,Key등， 「’
                                                                      qual，=,std: ;
                                                                  Allocator std: equal7
                                                                                          to<
                                                                                             Key>,
                                                                                   :ellocator<  std: :pajr                 Key,        >
> cl.ass unordered set;
                                                             class
                                                                                                             'cconst
                                                                                                                                  T>
                                                        > class un。
                                                                  rdered_map;


===== PAGE 42 =====
Unordered Associative



                                                    overflow
  keys                   buckats                     antHas
              000                        x
             《ml     uIa $m漱
                           ＇   52l8976   S
              002                        x
                ■
                1




              15 l


            日 l54
               1
              253
             ■
              255




   ● hash table
   ● chaining (linked list)


          Space           0(n)               0(n)

          Search          0(1)               0(n)

          Insert          0(1)               0(n)

          Delete          0(1)               0(n)

   keyOㅔ 따라 bucket에 잘 분배되도록 hash function을 만들어야 한다．


===== PAGE 43 =====
STL Container
  Unordered Associative




       5W아카데미


===== PAGE 44 =====
multi_set, multi_map


   ●   eaqual_range 활용 : 원하는 key값의 구간 반환

       auto ret = m.equal_range(x);
            ret.first = m. lower_bound(x)
            ret.second = m.upper_bound(x)

   .   m. erase(x) : key값이 x인 모든 원소 제거

   ●   m. find(x) : x중 하나의 iterator 반환
                                     （어떤 게 나올지 모름）

   .   [] operator Xfl공 X (multi_map)


===== PAGE 45 =====
iterator m.erase(iterator pos)
iterator m.erase(iterator first, iterator last)

: 마지막 지워진 element 바로 다음 iterator 반환

bool m.erase(T x)

: 성공 여부 반환



        ●   key값에 대한 value가 추가된 것 외에 set와 동일

        ●   compare 기준은 무조건 key 값



map<int, int> in;


for (mnt j = 5; i       > 0; i- -) m.insert({ i, 0 });


// (1,0) (2,0) (3,0) (4,0) (5,0)
for (auto x : in) cout << x.first        << ', ' << x.second;
for (auto it      = m.beginQ; it     H m.endQ; ++it) {
            cout << it- >first << ', ' << it- >second;




// (5,0) (4,이 (3,0) (2,0) (1,0)
for (auto it = m. rbeginQ; it         H m. rendO; ++it) {
            cout << it- >first << ', ' << it- >second;

}

m{l]    = 3;!!   (1, 3) (2, 0) (3, 0) (4, 0) (5, 0)

m[6];       // index 접근 시, 등록되어 있지 않믄 key 값미연 deFault 값
                                                      （0）
                                                        으로 insert : (6, 0)

m[7l++;     // 畛y값 7 이 등록되어 있지 않으므로 value 0으로 Insert 후，value 1 증가 r (7, 1)




m : (1,3) (2,0) (3,0) (4,0) (5,0) (6,0) (7,1)


===== PAGE 46 =====
map - 주요 문법
template<


    class Key,
    class T,
    class Compare = std: :less<Key>,
    class Allocator = std: :allocator<std: :pair<const Key, T> >
> class map;

)K size_t : unsigned long long


map<T, U> m

map<T, U, Compare<T> > m




U m[T x] : x가 등록되지 않은 상황이면default 값
                                  （0）
                                    으로 등록

iterator m.begin0, m.end()

iterator m. rbegin0, m.rend()

bool m.empty()

sizet m. size()

void m.clear()

size_t m. count(T   x)
iterator m.find(T x)

iterator m.lower_bound(T x)


pair<iterator, bool> m.insert({ I    x , U y})
: first （등록된 iterator) , second
                              （성공 여부）반환



void m.insert(iterator first,    iterator last)


===== PAGE 47 =====
custom type의 compare 설정
  ●        기본 type과 동일하다．하지만J <, > operato
                                         「를 사용하려면 해당

           operato
                 「의 정의가 필요하다．           : operator overloading



  1.       operator overloading

           : default가 less<Data＞이므로 operator < overloading 필요

      struct Data {
            mnt a, b, c,
            bool operator<(const Data& r) const {
                return a < 「 .a;



      };
      set<Data> s; // == set<Data, less<Data> > a;




  2.       function object
      struct Data { mnt a, b, c; };
      struct Comp {
            bool operatorO(const Data&i,    const Data&r ) const {
                return l. a < r. a;       …∼즙

       }
      ｝…                …「




      S朴t<DataJ Comp> S;




      compare 기준 : a값 오름차순            (1,2 동일）

      key값 중복 판별 : b' 《＝ 관계없이 a가 같으면 중복

            S    {l, 2, 3) == {l, 0 ,0}
            S    {l, 2, 3) != {0, 2, 3}


===== PAGE 48 =====
Key값 중복 판별
      ●     compare 기준으로 우선순위 높은 값，같은 값J 낮은 값 모두 판별

            가능해야 한다．

      ●     따라서J compare가 만족해야 하는「equirement가 존재하며 판단

            기준은 아래와 같다．

      ●     값 A, B에 대해

            1.     comp(A,B) && !comp(B,A) : left = A, right = B
            2.    !comp(A,B) &&      comp(A,B) : left = B, right = A
            3.    !comp(A,B) && !comp(B,A) : A == B

            ※    C omp(A,B) 예시 : bool comp(T A, T B) { return A<B; }



Compare Requirements
1.    Binary Predicate
      A.    return type : bool

      B.    argument 개수 : 2개



2.    Strict weak ordering
      A.    !comp(a,a)

      B.    comp(a,b) O면, !comp(b,a)

      C.    comp(a,b) && comp(b,c) OI면, comp(a,c)

      D.    !comp(a,b) && !comp(b,a) O면, a==b



     ＜요약＞

           <, > operato
                      「만 사용

           좌우 항이 같은 형태

           ex) l. x < r. x   ,   1.x+l. y < r. x+r. y   ,   Lx < r. y


===== PAGE 49 =====
compare 설정
     ●    function object 형태（다른 방법도 있지만 가장 기본）


1    pre-defined function object : less<T>, greater<T>
     ex) greater<int> , 내림차순

set<int, greater<int>> ${ 1, 2, 3, 4, 5 };
for (auto x : s) cout << x << "     ;            /7 5 4 3 2 1




2    user-defined function object
     ex) 절대값 오름차순

struct AbsComp {
     bool operatorQ (const tnt &a, const mnt &b) const {
         return abs(a) < abs(b);        7/ abs(x) : x 의 절대값

     }
};
set<int, AbsComp> s{ -5, -3, 1, 4, 6 };
for (auto x : s) cout << x << "     ; II 1   3 4 -5 6


===== PAGE 50 =====
set - example

conipa re 기준 : default          = less<int> 』 오름차순

set<int> 5;
for (tnt I = 5; i   > 0; I--) s.insert(i) ;


For (auto x : s) cout << x << "    ;                                         // 1 2 3 4 5
for (auto it = s.beginQ; it     != s.endQ; ++it) cout << *it   << "    ;     1/ 1 2 3 4 5
For (auto it = s.rbeginQ; it     1= s.rendQ; ++it) cout << * jt << "       ; II   S 4 3 2 1


s. emptyQ;                          II   0
s.sizeQ;                            II   5
s.count(1);                         II   1
5 .count(0);                        II 0


auto ret = s.find(1);               II   1 검색J ret : 값 1 2! iterator



auto ret = s.insert(6);

II   6 등록，ret.first   = 등록된 iterator, ret. second : 1 （등록 여부）

auto ret = s.insert(1).first;       // 1 등록』 ret : 등록된 iterator

auto ret = s.insert(1).second;      II   1 등록J ret = 0（등록 여부）



auto ret = s.erase(2);              // 2 삭제＇ ret = 1 （삭제 여부）

auto ret = s.erase(2);              // 2 삭제J ret : . （삭저l 여부）



auto ret = s.erase(s.begino);

// 맨 앞 element 삭제＇ ret : 삭제된 element 의 다음 iterator

auto ret = s.erase(- -s.endQ);

// 맨 뒤 element 삭제＇ ret : 삭제된 element 의 다응 iterator


===== PAGE 51 =====
iterator s.lower_bound(x)    : x보다 크거나 같은 가장 작은 값

pair<iterator, bool> s.insert(x)
: 등록된 iterator ' 성공 여부 반환


void s.insert(first, last)


iterator s.erase(pos)
iterator s.erase(first, last)
: 마지막 지워진 element 의 다음 iterator 반환
bool s.erase(x)
: 성공 여부 반환


===== PAGE 52 =====
            Space             0(n)           0(n)

            Search            0〔＇og n)       0(log n)

            Insert            0(Iog n)       0(log n)

            Delete            0(logn)        0(Iog n)




set - 주요 문법

template<


    class Key,
    class Compare = std: :less<Key>,
    class Allocator = std: :allocator<Key>
> class set;
※ pos, first, last는 iterator
) size_t : unsigned long long

set< T> s

set< T, compare> s



iterator s.beginO, s.end()

reverse_iterator s. rbegin() , s . rend()

bool s. empty()

void s.clear()

sizej   5.size()

sizet   s.count(x)             : X 의 개수 반환
                                         （1 or 0)

iterator s. Find(x)


===== PAGE 53 =====
set) map

   ●   Red-Black Tree
       : self-balancing binary search tree
  ●    Bidirectional iterator
  ●    set은 key type 한 개＇ map은 key type에 대한 value type 존재
  .    모든 검색은 key를 활용해서만 진행
  ●    등록된 element의 key 값은 변경 불가     （필요시』 erase후 insert)
  ●    map의 value는 변경 가능




                                     l7


                               15         25


                                     2z        27


                          <set 구조＞




                          <map 구조》


===== PAGE 54 =====
STL Container
   - Associative




     SWO타데미


===== PAGE 55 =====
list - example 2


struct Data { mnt Id, value; };


list<Data> u;
list<Data>::iteraton it[6];


-For (mnt I = 1; i <= 5; i++)

    it[i] = li.mnsert(li.begin0, { i, 0 }); II insert 하며 iterator기



/* 정방향 순회 */

for (auto d : ii)     d.id , d.value;
-For (auto it = li. beginQ; it    ! = li. endQ; ++it) it- >id, it- >value;


/* 역방항 순회 */

-for (auto it = li. rbegin0; it     1= li. rendQ; ++it) it- >id, it- >value;


it[ 5] ->value = 3;                            // (1,0) (2,0) (3,0) (4,0) (5,3)
it[ 3]->value = 4;                            II    (1,0) (2,0) (3,4) (4,8) (5,3)


li. erase(it[ l] );                            //         (2,0) (3J0) (4J0) (5J 3)
li. splice(li. beginQ, ii,    it[ 5]);        II    (5,3) (2,0) (3,0) (4,0)


===== PAGE 56 =====
list - example 1

list<int> ii, 112;


-For (mnt I = 1; i <= 5; i-i-+)
          li.push_back(i);                      : 1 2 3 45


                                                     1l       1<a
                                                                    4   ㄷ
                                                                        J
li.insert(li.endQ, 6);       .,
                              ,                                             〃
                                                                            b
                              ,
                                  /                  ｀
                                                     ㅗ    z   그 J
                                                                        4   ㄷ
                                                                            J   b
li.insert(next(li.beginQ, 3), 7);


ii. pop_front();                                '.        237456
11.erase(11.begin0);                            :         37456
11.erase(---11.end0);                           : 3745


ii.sort();                                      : 3457
ii.sort(greater<int>{});                        : 7 543


li.splice(li.endQ, ii, li.beginQ);    :45 7 3
1i2.splice(112.beginO, ii);           : ii = empty, 1i2 = 4 5 7 3


li.splice(li.beginQ,                  : ii   = 45
           1i2,                       : 1i2 = 7 3
           1i2.begin(), next(1i2.beginQ, 2));


===== PAGE 57 =====
size_t li.size()


I li.frontQ, li.back()


void li.push_back(T x)
void li.pop_back()
void li.push_Front(T x)
void li.pop_front()



iterator li.insert(iterator pos, I x)

iterator li.insert(iterator pos, mnt count, I x)

iterator li.insert(iterator p05, iterator first, iterator last)

 : 처음 입력된 element 의 iterato
                          「 반환




iterator erase(iterator pos)

iterator erase(iterator first,   iterator last)

 : 마지막 지워진 element 의 다음 iterato
                              「 반환




void li. splice(iterator pos, list<I> 112) : 11의 pos 에 1i2 전체 이동

void li. splice(iterator pos, list< T> 1i2, iterator it) : 1i 의 pos 에
112 의 it 이동

void li. splice(iterator pos, list< T> 112, iterator first,   iterator
last) : 11의 p0$ 에 112 의 [first, last) 구간 이동

void li. sortO: operator< 기준으로 정렬

void li. sort(function compare) : compare 기준으로 정렬

 : O(n log n)


===== PAGE 58 =====
list
     ●       doubly linked list

     ●       bidirectional iterator



   ＝눼그＝늬二｝=＝눼댜＝＝늬1긔
 ［갸；
    front                                          back



                                      Complexity

                      Space           0(n)

                      Search          0(n)

                      Insert          0(1)

                      Delete          0(1)




list     - 주요 문법

teniplate<


    class T,
    class Allocator = std: :allocator<T>
> class list;



list< T> ii
iterator li. beginO, li. end()
reverse_iterator li. rbeginO, li. rend()


void li. clear()
bool li. empty()


===== PAGE 59 =====
deque


  ●     dynamic array

  ●     random access iterator

  ●     vecto
            「와의 차이점은 front에 insert/erase가 0(1)

   ●    사용은 vecto
                「와 동일하며J Pu引1JroritO, P이U:roflt() 추가 제공

   ●                 「보다 느리므로 什ont에 insert/erase가 필요
        일반적인 연산은 vecto
        한 경우에만 사용




                                        push_front(J
                                            +
 川ocki
 block2
 block3

                                                       ‘   十
                                                  push_backO
block주소저장




                    Space        0(n)
                    Search       0(n)
                    Insert       0(n)
                    D이ete        0(n)
                    Push back
                                 0(1)
                    Pu針＇ front
                    p이）hack
                                 0(1)
                    PopJront
                    Migration    이block수〕


===== PAGE 60 =====
findO, find_if()

find()

template< class InputIt, class T >
InputIt find( InputIt first, InputIt last, const T& value );

●   [first, last) 구긴乂게서 값이 value인 첫번째 element의 iterator 반환

S   auto it = find(arr.begin(), arr.endO, 1);



find_if O

template< class InputIt, class UnaryPredicate >
InputIt find_if ( InputIt first, InputIt last,
                  UnaryPredicate p );

●   더:irst, last) 구간에서 f의 결과가 true인 첫번째 element의 iterator
    반환

●   UnaryPredicate : bool p(T a)

●   auto it = find_if (arr.begin(), arr.end0, [](auto x) { return
    x < 10; });


===== PAGE 61 =====
sW아카데미
