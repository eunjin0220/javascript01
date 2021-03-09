---
description: 하나의 로직을 재실행 할 수 있도록 하는 것으로 코드의 '재사용성'을 높여준다.
---

# 함수

## 함수의 형식/정의/호출

```javascript
// 함수 형식
function 함수명( [인자...[,인자]] ){
   코드
   return 반환값
}

// 함수 정의
function numbering(){
    i = 0;
    while(i < 10){
        document.write(i);
        i += 1;
    }   
}

// 함수 호출(실행)
numbering();
```

## 입력과 출력

### return : 함수 종료 + 뒤에 따라오는 값을 함수의 결과로 반환

```javascript
function get_member1(){
    return 'egoing';
}
 
function get_member2(){
    return 'k8805';
}
 
alert(get_member1()); //egoing
alert(get_member2()); //k8805
```

### 인자 : 함수로 유입되는 입력 값

```javascript
function get_argument(arg){ //값을 받는 변수(arg) = 매개변수
    return arg;
}
 
alert(get_argument(1)); //값(1) = 인자
// 매개변수arg의 값으로 숫자 1이 함수 안으로 전달
// 코드 결과 = 1
```

### 복수의 인자

```javascript
function get_arguments(arg1, arg2){
    return arg1 + arg2
}
 
alert(get_arguments(10, 20)); //30
alert(get_arguments(20, 30)); //50
```

## 함수를 정의 하는 다른 방법

```javascript
var numbering = function (){
    i = 0;
    while(i < 10){
        document.write(i);
        i += 1;
    }   
}
numbering();

//익명함수
(function () {
    i = 0;
    while(i < 10){
        document.write(i);
        i += 1;
    } 
})();
```

{% hint style="success" %}
함수는 코드의 재활용성을 높여준다
{% endhint %}

