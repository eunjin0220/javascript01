---
description: 주어진 조건에 따라서 애플리케이션을 다르게 동작하도록 하는 것
---

# 조건문

## if

```javascript
if(조건) {
    명령문
}

if(true) {
    alert('result : true');
}
//조건 값이 true인 경우 = 실행됨

if(false) {
    alert('result : true');
}
//조건 값이 false인 경우 = 실행되지 않음
```

## else

```javascript
if(true) {
    alert(1);
}else {
    alert(2);
}
// else : 주어진 조건이 거짓일 때 실행할 구문을 정의하는 것
```

## else if

```javascript
if(false) {
    alert(1);
}else if(true) {
    alert(2);
}else if(true) {
    alert(3);
}else {
    alert(4);
}
// else if : 다양한 케이스의 조건을 검사할 수 있다.
```

## 변수와 비교연산자

```javascript
 prompt('당신의 나이는?');
 //사용자에게 값을 받을수 있는 기능
 
 id = prompt('아이디를 입력해주세요.')
 if(id=='egoing'){
     alert('아이디가 일치 합니다.')
 }else {
     alert('아이디가 일치하지 않습니다.')
 }
 // 1. 입력한 값을 id변수의 값으로 대입
 // 2. 사용자가 입력한 값이 egoing이라면 '아이디가 일치합니다'
 // 3. 그렇지 않다면 '아이디가 일치하지 않습니다'
```

## 조건문의 응용

```javascript
id = prompt('아이디를 입력해주세요.');

if(id=='egoing'){
    password = prompt('비밀번호를 입력해주세요.');
    if(password==='111111'){
        alert('인증 했습니다.'); //아이디O 비밀번호O
    }else {
    alert('인증에 실패 했습니다.'); //아이디O 비밀번호X
    }
}else {
    alert('인증에 실패 했습니다.'); //아이디X
}
```

## 논리 연산자

### && : 좌항과 우항이 모두 참\(true\)일때 참이된다. ' and연산자 '

```javascript
if(true && true){
    alert(1);
} //true
if(true && false){
    alert(2);
} //false
if(false && true){
    alert(3);
} //false
if(false && false){
    alert(4);
} //false
```

### \|\| : 좌우항 중에 하나라도 true라면 true가 된다. 'or연산자'

```javascript
if(true || true){
    alert(1);
} //true
if(true || false){
    alert(2);
} //true
if(false || true){
    alert(3);
} //true
if(false || false){
    alert(4);
} //false
```

### ! : 부정의 의미로, Boolean의 값을 역전시킨다. 'not연산자'

```javascript
if(!true && !true){
    alert(1);
} //false
if(!false && !true){
    alert(2);
} //false
if(!true && !false){
    alert(3);
} //false
if(!false && !false){
    alert(4);
} //true
```



