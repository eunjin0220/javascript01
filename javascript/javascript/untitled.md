# Untitled



## 숫자

### 수의 표현

```javascript
alert(1); //정수
alert(1.1); //실수
```

```javascript
alert(1+1); //2
alert(1.1+1.1); //2.2
alert(2*8); //16
alert(6/2); //3
```

### 수의 연산

```javascript
Math.pow(3,2); //3의 2승 = 9
Math.round(10.6); //10.6의 반올림 = 11
Math.ceil(10.2); //10.2의 올림 = 11
Math.floor(10.2); //10.2의 내림 = 10
Math.sqrt(9); //9의 제곱근 = 3 
Math.random(); //난수(랜덤한 숫자)
```

* pow : 제곱
* round : 반올림
* ceil  : 올림
* floor : 내림
* sqrt : 제곱근
* random : 난수

## 문자

### 문자의 표현

문자는 반드시 "\(큰 따옴표\) 혹은 '\(작은 따옴표\) 중의 하나로 감싸야 한다

```javascript
alert("egoing's coding everybody");
alert('egoing"s coding everybody');
```

```javascript
alert('egoing's coding everybody'); //에러 발생
alert('egoing\'s coding everybody'); //이스케이프
```

\  : 단순히 정보로서 해석하도록 강제 할 수 있는 기호 "이스케이프\(escape\) "

### 문자에 대한 명령들

```javascript
alert("coding\neverbody"); // \n : 줄바꿈
alert("coding"+"neverbody"); // 문자와 문자를 결합

alert(1+1) : 2 //숫자+숫자
alert("1"+"1") : 11 //문자+문자

alert("coding neverbody".length); // 문자의 길이를 구할때 = 16
alert("code".indexOf("c"); // 문자열의 숫자를 구할때 = 0
```

