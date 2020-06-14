# 2주차 

- nodejs깔았음 // 주로 LTS를 깔아줘야함 [LTS : Long Term Service]

  - node -v해서 잘 깔렸는지 확인해줌
  - pwd cd ll ls 등등 변수명 차차 익히자

- node package manager는 무엇인지 조사^^

  

- 2절에서 2.12(null병합은 빼고 공부함)

- 2.16 / 2.17 이 중요함

- 4.3은 안해도 되고 

- 4.1과 객체

- 숙제 4.4 / 4.5 (symbol은 어려운 관계로...)

- 4.6 새 문법

- 5.1 ~ 5.3 읽기

- 깃에 올려보자

  

- ~~파일을 하나 생성할 때 JavaScript인 만큼 types.js라고 쳐준다.~~

  => 아무이름.js (js는 자바스크립트의 확장자명이예요~)

  

- key에 동적으로 변수 넣고 싶을 때 [ ]을 사용한다.
  - obj.bar=2
  - obj['bar']=2
  
- number 
  - 2^53 정도로 아주 ~~big int~~ 큰 정수까지 받을 수 있다. 

    => big int 는 es6(2016년 이후에 나온 자바스크립트) 의 새로운 타입이에요.

    - ~~num =2e53; (O)~~

      => 잘못 설명했었네요. 2e10; 은 2 곱하기 10^10 이래요~ ㅎㅎ;;

    - num=2**53;(O)

    - 범위가 넘어가면 infinity+-가 나옴~

- typeof
  - console.log(typeof 1234);
  - //결과값 number!!
  
- String
  - string의 주요 성질, 변경이 불가능하다.

  - 바꾸려면 재할당( = assignment operator ) 뿐!

  - ~~그러나!! let은 바꿀 수 있다.~~

    => let 은 재할당이 가능한거랍니당, const 에 string 넣으면 재할당이 안 돼요!

  - const 는 재할당 안됌 (예전엔 let과 const가 아닌 var을 사용했고 이 var는 const의 특징이 없어 불편했었음)

- Boolean 
  
  - 모든 객체는 Boolean 해봤을 때 true가 나오니(비어 있어도) 주의하자
  
- 외부로 들어갈 때 callback함수 사용

- ~~자바 스크립트가 생성자 역할도 한다.~~

  => js에서 함수가 생성자 역할을 하기도 해요. 자세한건 다음에 ^^

- class Person{}...P가 대문자임을 잊지말자

- undefined와 null의 차이점
  - 둘 다 값이 없음을 나타낸다
  - undefined은 기본적으로 값이 할당되지 않은 변수로 데이터 타입, 값을 나타낸다.
  - null은 명시적으로 값이 비어있음을 개발자가 지정해주는 것이다.
    - 그런데 null을 typeof 해보면 object가 나오는 것을 알 수 있다. (설계상의 오류^^)
  
- NaN
  - Not A Number
  - console.log('str'/1);
  - //실행결과 : NaN
    - NaN은 특별한 아이라, 자기 자신과의 비교도 안되는 아이
    - 그러니 isNaN으로 비교하자