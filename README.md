# 이혜빈[201840129]
## [3월 30일]
<!DOCTYPE html>
<html lang="ko" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    <span style= "font-weight:bold; font-size:20px;"> if else if 조건문 :</span> 중복되지 않는 세 가지 이상의 조건을 구분할 때 사용<br>
    하나로 지정할 수 없을 때 사용(예:90보다 크고 100보다 작은것)<br>
if {
else if {
else
}
<br>
객체생성 ->메소드를 변수에 저장 -> if else if 조건문 돌림 -> 결과 값 배출<br>

<span style= "font-weight:bold; font-size:20px;">[switch 조건문] </span> 정한 값이 있을 때, 하나로만 결정될 때(예:다음 과일 중 하나를 고르시오, 열가지 음료수 자판기 ~)
-비교할 값이 들어감.
-각각의 항목을 case로 작성
-break : 밖으로 빠져나오기

<span style= "font-weight:bold; font-size:20px;">[삼항 연산자]</span>
-기본형태 : <불 표현식> ? <참> : <거짓>
-예제1 : 숫자의 부호를 비교해서 0보다 큰지 아닌지 판별 (T/F)
 예제2 : A||B에서 A가 참이라면 A로 대치
           B||A에서 B가 거짓이라면 B로 대치

<span style= "font-weight:bold; font-size:20px;">[조금 더 나아갑시다...>]</span>
-웹 브라우저에서 작동하는 자바스크립트 : prompt() 이름의 함수를 받음.
-Node.js에서 작동하는 자바스크립트 : 단순한 코드로 입력을 받을 수 없음.
*종료하고 싶을 때는 Ctrl + C를 연속해서 두 번 누름.*

<span style= "font-weight:bold; font-size:20px;">[반복문]</span>
-붙여 넣기를 사용한 반복(1000번 출력하는건 무리) -> for (let i = 0; i < 1000; i++)

<span style= "font-weight:bold; font-size:20px;">[배열]</span>
-여러개의 자료를 한꺼번에 다룰 수 있는 자료형
-대괄호 내부의 각 자료는 쉼표로 구분
-배열에는 여러 자료형이 섞여 있을 수 있음
-요소 : 배열 안에 들어 있는 각 자료.
- 배열 요소 ( 배열[인덱스])
                    |
                   ->요소

<span style= "font-weight:bold; font-size:20px;">[while 반복문]</span>
-무한 반복분
 while (true) {
  console.log("무한 반복");
}
-특정한 숫자를 증가시켜 불 표현식을 false로 만들어 반복문을 벗어남.

<span style= "font-weight:bold; font-size:20px;">[for 반복문]</span>
-for 반복문의 각단계
 1.초기식을 비교
 2.조건식을 비교
    조건이 false이면 반복문을 종료
 3.문장을 실행
 4.종결식을 실행
 5.2단계로 이동
-기본형태 : for (let i = 0; i < <반복횟수>;  i++)
                }
-예제 : for 반복문을 이용한 덧셈(0부터 100까지 더하기)
 1.변수 선언 -> let output = 0;
 2.반복을 수행 -> (~ i++)
 3.출력 -> console.log(output);
  </body>
</html>

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

