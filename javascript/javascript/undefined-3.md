# 비교

## 연산자

### 대입연산자

```javascript
a = 1 // '='는 우항의 값'1'을 좌항의 변수'a'에 대입
```

### 비교연산자

주어진 값들이 같은지, 다른지, 큰지, 작은지 구분하는 것을 의미. 비교 결과는 'true'나 'false'중의 하나.

#### == : 동등 연산자

```javascript
alert (1==2) //false
alert (1==1) //true
alert("one"=="two") //false 
alert("one"=="one") //true
```

#### === : 일치 연산자 \(데이터형식까지\)

```javascript
alert(1=='1'); //true
alert(1==='1'); //false
/* === 쓰는 것을 권장 */
```

#### null / undefined / NaN

```javascript
null //값이 없다를 표시
undefined //값이 없는 상태

alert(null == undefined); //true
alert(null === undefined); //false
alert(true == 1); //true
alert(true === 1); //false
alert(true == '1'); //true
alert(true === '1'); //false
alert(0 === -0); //true
alert(NaN === NaN); // 0/0과 같은 연산의 결과로 만들어지는 특수한 데이터 형
```

| 데이터의 타입 | 데이터 |
| :--- | :--- |
| Boolean | true / false |
| Number | .. -1 , 0, 1 .. |
| String | "a" "b" "c" |
| undefined | undefined |
| null | null |

#### != : '!'은 부정을 의미 \(같지 않다\)

```javascript
alert(1!=2); //true
alert(1!=1); //false

/* !== : 정확하게 같지 않다 */
```

#### &gt; / &gt;= / &lt; /&lt;=

```javascript
alert(10>20); //10보다 20이 크다 = false
alert(10>=20); //10보다 20이 크거나 같다 = false
```

