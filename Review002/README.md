# 2025년 12월1일 복습

## 핵심 개념정리

- ### (1) 변수 var / let / const
- var -> 함수 스코프 / 재선언 O / 호이스팅 O
- let, const -> 블록 스코프 / 재선언 X / TDZ 존재
- const: 값(원시)은 변경 불가, 객체 · 배열은 속성 변경 가능

- ### (2) Hoisting
- var: 선언이 끌어올려짐 -> undefined 상태로 초기화
- let/const: TDZ 때문에 선언 전 접근 시 오류
- 함수 선언문: 전체가 호이스팅
- 함수 표현식: 변수민 호이스팅,값은 호이스팅 X

- ### (3) 연산자
- 산술: + - \* / %
- 비교: == vs === (타입비교) 그러나 **=== 만 사용하는 것을 권장**
- 논리: && , || , !

- ### (4) Primitive Type (원시타입)
- string,number , boolean
- null (의도적 빈 값)
- undefined (값이 없는 상태)
- symbol (고유한 키)
- bigint (큰 정수)

## 타이핑 실습

### 타이핑 실습1 - var / let / const

> `var a = 10;`
> `let b = 20;`
> `const c = 30;`
> `b = 25;`

<!-- c = 40;  오류발생-->

`console.log(a,b,c);`

### 타이핑 실습2 - 스코프 & TDZ

> `console.log(x); // undefined`
> `var x = 5 ;`
> {
> // console.Log(y); // TDZ 에러
> `let y = 10;`
> }

### 타이핑 실습3 - 논리 연산자

> `let isLogin = true;`
> `let isAdmin = false; ` >`console.log(isLogin && isAdmin);`
> `console.log(isLogin || isAdmin);`
> `console.log(isLogin);`

### 타이핑 실습4 - String & Number

> `let name = "영종";`
> `let age = 32; `
> `` console.log(`이름: ${name},나이: ${age}`); ``

### 타이핑 실습5 - undefined vs null

> `let a;`
> `let b = null;` >`console.log(a,b);`

> # 오늘배운 JavaScript 기초
>
> - 변수 -> 스코프 -> 호이스팅 -> 연산자 -> 타입
