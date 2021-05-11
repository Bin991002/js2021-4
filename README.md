# 이혜빈[201840129]
## [5월 11일]
><h4>오늘 배운 내용 요약</h4> <br />

<h2><Date 객체 생성 방법></h2><br />
new Date() : 현재 시간으로 Date 객체를 생성합니다.<br />
new Date((유닉스타임)) : 유닉스 타임으로 Date 객체를 생성합니다.<br />
new Date(<시간 문자열>) : 문자열로 Date 객체를 생성합니다.<br />
new Date(<년>,<월-1>,<일>,<시간>,<분>,<초>,<밀리초>) :시간요소를 기반으로 Date 객체를 생성<br />

-Month를 나타내는 '월'은 0부터 시작,<br />
  0 -> 1월, 11 -> 12월<br />

//7-5 Date 객체 생성<br />
let dateA = new Date(1600000000000);<br />
console.log(dateA);<br />

<h2><메소드 활용></h2><br />
Date 객체<br />
 ->getOO() 형태 메소드, setOO() 형태 메소드 : FullYear, Month, Day, Hours~ 등 사용!<br />

// 예제 7-6 시간 더하기<br />
let date = new Date();<br />

console.log(date);<br />

date.setFullYear(date.getFullYear() + 1);<br />
date.setMonth(date.getMonth() + 1);<br />
date.setDate(date.getDate() + 1);<br />

console.log(date);<br />

<h2><Array 객체의 기본 메소드></h2><br />
- 대부분 파괴적 메소드로 자기 자신을 변경.<br />
- 예 : concat(), join(), pop()*, push()*, reverse()*, slice() ....등등<br />


//예제 7-7<br />
let now = new Date();<br />
let before = new Date('December 9, 2020');<br />

let interval = now.getTime() -before.getTime();<br />
console.log(interval);<br />

interval = Math.floor(interval / (1000*60*60*24));<br />
console.log(interval);<br />


<h2><조금 더 나아가기></h2><br />
- 프로토타입에 메소드를 추가하면 해당 자료형 전체에 추가 가능<br />
- String 생성자 함수의 prototype 속성에 contain () 메소드를 추가<br />

//프로토타입에 메소드를 추가합니다.<br />
String.prototype.contain = function (input) {<br />
   return this.indexOf(input) >= 1;<br />
};<br />

//메소드를 활용합니다.<br />
console.log('안녕하세요' .contain('안녕'));<br />
console.log('안녕하세요'. .contain('데굴데굴'));<br />

<JSON 객체><br />
- 자바스크립트 객체를 사용한 데이터 표현 방법<br />
[ <br />
   {<br />
        name: '고구마',<br />
        price: 1000<br />
    },<br />
    {<br />
        name: '감자',<br />
        price: 500<br />
    },<br />
    {<br />
        name: '바나나',<br />
        price: 1500<br />
    }<br />
]<br />

<h2>*제약사항 </h2><br />
1.문자열은 큰따옴표로 만듦.<br />
2.모든 키는 큰따옴표로 감싸야 함<br />
3.숫자, 문자열, 불 자료형만 사용 가능.<br />

## [5월 4일]
><h4>오늘 배운 내용 요약</h4> <br />
1.자바스크립트는 다양한 객체를 제공<br />
2.통합 개발 환경에서 자동 완성 기능<br />

<h2>기본 자료형 숫자, 문자열, 불<h2><br />
 //기본 자료형<br /> 
 let number = 273;<br />
 let string = '안녕하세요';<br />
 let boolean = true;<br />
 
 //자료형을 출력합니다.<br />
 consol.log(typeof number);<br />
 consol.log(typeof string);<br />
 consol.log(typeof boolean);<br />
 
 - 기본 자료형의 속성 또는 메소드를 사용할 때 기본 자료형이 자동으로<br />
객체로 변환이 됨. 즉, 기본 자료형과 객체 자료형 모두 속성과 메소드를 사용함<br />
- 차이점 : 기본 자료형은 객체가 아니므로 속성과 메소드를 추가할 수 없음<br />

<h2>Number 객체</h2>
1.자바스크립트에서 숫자를 표현할 때 사용<br />
2.Number 객체 생성<br />




## [4월 27일]
><h4>오늘 배운 내용 요약</h4> <br />
 <h2>배열</h2><br />
배열은 요소에 접근할 때 인덱스를 사용하고, 객체는 키를 사용함</br>

 <h2>속성과 메소드</h2><br />
 요소 : 배열 내부에 있는 값 하나하나</br>
속성 : 객체 내부에 있는 값 하나하나</br>
객체의 다양한 자료형</br>
메소드 : 객체의 속성 중 자료형이 함수인 속성</br>

<h2>생성자 함수와 프로토타입</h2></br>
객체 지향 프로그래밍 : 현실의 객체를 모방해서 프로그래밍</br>
배열과 객체를 사용하면 여러 개의 데이터를 쉽게 다룰 수 있음</br>
생성자 함수 : 객체를 만드는 함수, 대문자로 시작하는 이름 사용</br>
프로토타입 :생성자 함수로 만든 객체는 프로토타입 공간에 메소드를 지정해서 모든</br>
객체가 공유 하도록 함, 해당 함수를 생성자 함수로 사용했을 때만 의미가 있음</br>

<h2>NULL의 값과 자료형</H2></br>
consol.log(null);</br>
consol/log(typeof(null));</br>


 
>
## [4월 13일]
><h4>오늘 배운 내용 요약</h4> <br />
<h2>익명함수</h2><br>
-이름을 붙이지 않고 함수 생성<br>
-함수를 호출하면 함수 내부의 코드 덩어리가 모두 실행<br>

  let <함수(변수) 이름> = function () { };<br>
 (let을 붙이는 이유 : 자료형으로 생각 하고 있어서)<br>
 (변수에다가 function을 저장)<br>

- let foo = function () {<br>
    console.log("첫줄");<br>
    console.log("둘째줄");<br>
}<br>

let bar = 135;<br>

foo();<br>
console.log(foo);<br>
console.log(bar);<br>

-생성 -> 호출 -> 함수자체 출력<br>

<h2>*자바스크립트에서 함수는 ->자료형으로 본다.</h2><br>

<h2>선언적 함수</h2><br>
-이름을 붙여 함수를 생성.<br>
-'console.log(함수)' 부분으로 '[Function: 함수]' 문자를 출력<br>

- function foo () {<br>
  console.log("첫줄");<br>
  console.log("둘째줄");<br>
}<br>

foo()<br>
console.log(foo);<br>

<h2>화살표 함수[ECMAScript6]</h2><br>
-() => {  }<br>
-하나의 표현식을 리턴하는 함수를 만들 때는 중괄호 생략 가능<br>
-익명 함수 예제를 화살표 함수로 바꾸기.<br>
-함수 생성 -> 함수 호출<br>
- 화살표 함수. ES6 문법.<br>
let foo = () => {<br>
   console.log("첫줄");<br>
   console.log("둘째줄");<br>
}<br>

foo();<br>
console.log(foo);<br>

<h2>숫자 변환 함수</h2><br>
parselnt() : 문자열을 정수로 변환.<br>
parseFloat() : 문자열을 실수로 변환.<br>

<h2>타이머 함수</h2><br>
-특정 시간 후에 또는 특정 시간마다 어떤일을 할 때 사용<br>
-시간은 밀리초로 지정, 1초를 나타내려면 1000(밀리초)을 입력.<br>
-종료 : Ctrl + C<br>
setTimeout(함수, 시간) : 특정 시간 후에 함수를 실행.<br>
setintervall(함수, 시간) : 특정 시간마다 함수를 실행.<br>


## [4월 6일]
><h4>오늘 배운 내용 요약</h4> <br />

<h2><배열></h2><br />
1.여러개의 자료를 한꺼번에 다룰 수 있는 자료형<br />
2.대괄호 내부의 각 자료는 쉼표로 구분<br />
3.배열에는 여러 자료형이 섞여 있을 수 있다.<br />
4.요소 : 배열 안에 들어 있는 각 자료<br />

<h3><for 반복문으로 덧셈하기> </h3> <br />
- 변수 선언 (let output = 0;) -> 반복 수행 -> 출력<br />

<h2><역 for 반복문></h2><br>
 : 배열의 요소를 뒤쪽부터 출력<br>
(배열생성 -> 요소의 길이를 출력)<br>

<h3><for in 반복문과 for of 반복문></h3> <br />
- 객체에 쉽게 반복문을 적용함	<br />
- for in 반복문과 for of 반복문은 for  반복문 사용과 역할이 같음<br />

<h2><중첩 반복문> 예제 : 별 피라미드</h2><br />
let output = "";<br />
for (let i = 0; i < 10; i++) {<br />
    for (let j = 0; j < i+1; j++) {<br />
        output += "*";<br />
    }<br />
        output += "\n";<br />
    }<br />
console.log(output);<br />

<h2><break 키워드></h2> <br>
-예제 : 짝수를 찾으면 break 키워드로 반복문을 벗어남.<br />

## [3월 30일]
><h4>오늘 배운 내용 요약</h4> <br />
if else if 조건문 : 중복되지 않는 세 가지 이상의 조건을 구분할 때 사용, 하나로 지정할 수 없을 때 사용<br />(예:90보다 크고 100보다 작은것)<br />
if {<br />
else if {<br />
else<br />
}<br />

객체생성 ->메소드를 변수에 저장 -> if else if 조건문 돌림 -> 결과 값 배출<br />

<switch 조건문> : 정한 값이 있을 때, 하나로만 결정될 때(예:다음 과일 중 하나를 고르시오, 열가지 음료수 <br />자판기 ~)<br />
-비교할 값이 들어감.<br />
-각각의 항목을 case로 작성<br />
-break : 밖으로 빠져나오기<br />

<삼항 연산자><br />
-기본형태 : <불 표현식> ? <참> : <거짓><br />
-예제1 : 숫자의 부호를 비교해서 0보다 큰지 아닌지 판별 (T/F)<br />
 예제2 : A||B에서 A가 참이라면 A로 대치<br />
           B||A에서 B가 거짓이라면 B로 대치<br />

<조금 더 나아갑시다...><br />
-웹 브라우저에서 작동하는 자바스크립트 : prompt() 이름의 함수를 받음.<br />
-Node.js에서 작동하는 자바스크립트 : 단순한 코드로 입력을 받을 수 없음.<br />
<strong>*종료하고 싶을 때는 Ctrl + C를 연속해서 두 번 누름.*</strong><br />

<반복문><br />
-붙여 넣기를 사용한 반복(1000번 출력하는건 무리) -> for (let i = 0; i < 1000; i++) <br />

<배열><br />
-여러개의 자료를 한꺼번에 다룰 수 있는 자료형<br />
-대괄호 내부의 각 자료는 쉼표로 구분<br />
-배열에는 여러 자료형이 섞여 있을 수 있음<br />
-요소 : 배열 안에 들어 있는 각 자료.<br />
- 배열 요소 ( 배열[인덱스])<br />
                    |<br />
                   ->요소<br />

<while 반복문><br />
-무한 반복분 <br />
 while (true) {<br />
  console.log("무한 반복");<br />
}<br />
-특정한 숫자를 증가시켜 불 표현식을 false로 만들어 반복문을 벗어남.<br />

<for 반복문><br />
-for 반복문의 각단계<br />
 1.초기식을 비교<br />
 2.조건식을 비교<br />
    조건이 false이면 반복문을 종료<br />
 3.문장을 실행<br />
 4.종결식을 실행<br />
 5.2단계로 이동<br />
-기본형태 : for (let i = 0; i < <반복횟수>;  i++)<br />
                }<br />
-예제 : for 반복문을 이용한 덧셈(0부터 100까지 더하기)<br />
 1.변수 선언 -> let output = 0;<br />
 2.반복을 수행 -> (~ i++)<br />
 3.출력 -> console.log(output);<br />

## [3월 23일]
>오늘 배운 내용 요약 <br />
1.console.log();는 변수에 담긴 값은 객체, 문자열 다 출력한다. <br />
2.console.log(name[1]); 문자열 안에 있는 첫번째 글자를 출력해서 보여줌.(숫자=위치) <br />
3.+= 더하기 -= 빼기 *= 곱하기 /= 나누기 %= 나머지 <br />
4.++a 같은 경우는 값이 증가한 후에 연산을 하고, a++같은 경우는 연산을 하고 나서 값이 증가 <br />
  (이해하기 어려워서 구글에 검색) <br />
5.식별자 : -숫자로 시작불가. <br />
           -특수문자는 $와 _만 사용가능. <br />
           -공백입력 불가 <br /> 
           -사용규칙:생성자 함수 이름은 항상 대문자, 변수/함수/속성/메소드  이름은 항상 소문자 <br />
6.강제 자료형 변환 : Number() 숫자로 변환 <br /> 
                     String() 문자열로 변환 <br />
                     Boolean() 불로 자료형 변환 <br />
## [3월 16일]
>오늘 배운 내용 요약 <br />
1.UTF-5를 누르면 자동적으로 html 틀이 잡혀진다.<br />
2.깃허브 파일 연동시키고 올리는 방법을 알게 되었다.<br />
3.br태그를 쓰면 줄 바꿈<br />
4.meta태그 = 문자 인코딩 및 키워드, 요약정보<br />
5.li태그는 ul과 ol안에서 각 항목을 나열할 때 사용.<br />
>요약 끝

