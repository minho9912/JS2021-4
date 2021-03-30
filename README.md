# 최민호 [201840135]
## [03월 30일]
> 오늘 배운 내용 요약<br>
#### if else if 조건문
> if(조건){<br>
} else if(조건){<br>
} else if(조건){<br>
}else{<br>
}
#### Switch문
> switch(조건)&nbsp;&nbsp;{<br>
    &nbsp;case(조건):<br>
    &nbsp;&nbsp;출력문<br>
    &nbsp;&nbsp;break;<br>
    &nbsp;&nbsp;default:<br>    
    &nbsp;&nbsp;출력문<br>
    &nbsp;&nbsp;break;
}
#### 삼항연산자
> <불표현식> ? <참> : <거짓><br>
ex: number % 2 == 0 ? true : false <br>
#### 짧은 초기화 조건문
> 삼항 연산자를 활용한 변수 초기화<br>
ex: test = test || "초기화 합니다 1"<br>
console.log(test);
#### 짧은 초기화 조건문
> 삼항 연산자를 활용한 변수 초기화<br>
ex: test = test || "초기화 합니다 1"<br>
console.log(test);
#### Node.js의 input<br>
const repl = require('repl');<br>

repl.start({<br>
    prompt: "숫자 입력> ",<br>
    eval: (command, context, filename,callback)=> {<br>
        let number = Number(command);<br>
        if(isNaN(number)){<br>
            console.log("숫자아님");  <br>
        }else{<br>
            console.log("숫자맞음");  <br>
        }<br>
        callback();<br>
    }<br>
})
#### 배열
> 여러 개의 자료를 한꺼번에 다룰 수 있는 자료형이다.<br>
대괄호 내부의 각 자료형은 쉼표(,) 로 구분한다.
ex: let array = [52,23,'아침밥','점심밥',true,false]<br>
console.log(array[0]);
#### while 반복문
> 가장 기본적인 반복문으로, if조건문과 달리 조건식이 참인 동안에는 계속 실행된다<br>
조건이 변하지 않으면 무한 반복 하므로 반드시 조건을 false로 만들 수 있는 문장을 포함해야한다.<br>
ex: while(true){ <br>
console.log("무한반복);<br>
}
#### for 반복문
> 맨 먼저 초기식을 실행하고 조건식을 확인한다.<br>
조건식이 false면 반복문을 빠져나가고, true면 문장과 종결식을 차례로 실행해 다시<br>
조건식이 true인지 확인한다.<br>
ex: let sum=0; <br>
for(let i=0; i<=100; i++){<br>
sum+=i;<br>
}console.log(sum)<br>
}

---
## [03월 23일]
> 오늘 배운 내용 요약<br>
-  탬플릿 문자열 : console.log('`52 + 273 = ${52 + 273}`'); // 52+273=325
- 불 : true,false // 비교연산자 : ==,!=,>,<,>=,<= // 논리연산자 : !,!!,&&<br>
-- ex: let hours = new Date().getHours(); // console.log(hours < 3 || hours > 8);
- 변수 : let으로 선언 // let a = 10; 
- 복합 대입 연산자 : +=,-=,/=,*= // let a=0, // a=a+1,a=a-1;
- 증감 연산자 : 변수++,++변수,변수--,--변수
- 자료형 검사 : type of
- undefined 자료형 : let a; //선언만하기
- 강제 자료형 변환 : Number(),String(),Boolean()
- NaN: 무조건적으로 다름, 확일할 때는 isNaN()함수 활용
- Boolean() 함수
- 자동 자료형 변환 : // console.log(52+273),("52"+273)
- 불 자료형 자동 변환 // console.log(!!0),(!!"")
- 일치 연산자 : ===,!== // 자료형과 값이 같느냐/다르냐
- 상수 : const // 변하지 않는다 , 변수값.
- 조건문 : if,if else, else if , 중첩 조건문
> 요약<br>
- 탬플릿 문자열 방식은 연산할 부분을 ${}안에 넣어주면 된다.
- 불 은 참과 거짓을 구별하는 것이고, ==,!= 등의 비교연산자나 !같은 논리연산자를 사용한다.
- 변수는 let으로 선언한다.
- 복합 대입 연산자, 증감 연산자, 자료형 검사
- undefined 자료형, 강제 자료형 변환, NaN, Boolean()함수
- 자동 자료형 변환은 콘솔 내부에서 연산 작업시 자동으로 형을 변환해주는 것이다.
- 일치 연산자는 값만 같느냐, 자료형과 값이 같으냐에 대한 물음 이다.
- 상수는 값이 변하지 않는 변수이다.
- 조건문은 if,else if,if else가 있는데, if안에 if, else안에 else도 가능하다.
---
## [03월 16일]
> 오늘 배운 내용 요약<br>
-  JS 출력 결과 확인 방법 : 크롬 F12(개발자도구) - console 에서 명령문 입력 후 Enter 클릭
- node 버전 확인 방법 : cmd - 'node -v' 입력 후 Enter 클릭
- js 출력문 예시 : console.log('hello world') , alert('hello world')
- js 키워드 : break, else, switch, void, while, continue 등등 
- 식별자 규칙<br>
-- 키워드 사용 안됨, 특수문자는 _와$만 허용, 숫자로 시작하면 안됨, 공백 입력 안됨
- 주석<br>
-- 한 줄 주석 처리 : //주석 (ctrl+/)<br>
-- 여러 줄 주석 처리 : /* 주석 */ 
- 자료형 - 숫자형 출력 (+,-,*,/)<br>
-- console.log(5+3)or(5-3)or(5 *3)or(5/3)
- 자료형 - 문자열 출력<br>
-- console.log("This is String")
- 이스케이프 형식 출력<br>
--console.log("이름\t나이"),("안녕\n하세요"),("\\\\\\\\"),("출\\'력\\'")
- 문자열 연결 연산자 출력 예시<br>
-- console.log("가나다"+"라마"+"바사아"+"자차카타"+"파하")<br>
> 요약<br>
- 자바스크립트는 console.log() 를 사용하여 콘솔 창에서 원하는 결과를 출력할 수 있다.
- alert() 함수를 활용하여 팝업창으로도 결과를 출력시킬 수 있다.
- 자바스크립트에는 다양한 기능을 하는 키워드가 존재한다.
- 식별자를 만들 때에 지켜야 할 규칙이 있다.
- 표시하고 싶지 않거나, 부가적인 설명을 하는 부분은 주석 처리를 한다.
- 자료형에는 숫자형과 문자열이 있다.
---