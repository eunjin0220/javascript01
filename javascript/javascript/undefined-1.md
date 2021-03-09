---
description: 값을 담는 컨테이너로 사용. 여기에 담겨진 값이 다른 값으로 바꿀 수 있다.
---

# 변수

## 변수의 선언

```javascript
var a = 1; // 변수를 선언! a = 1
a = 10;
alert(a); // 10

var first = "coding" // 변수는 숫자뿐만 아니라 문자도 가능
alert(first+"everybody"); // coding everybody
```

## 변수가 없다면

### 변수 사용 X

```javascript
alert(100+10);
alert((100+10)/10);
alert(((100+10)/10)-10);
alert((((100+10)/10)-10)*10);
```

### 변수 사용 O

```javascript
a = 100;
a = a + 10;
alert(a);
a = a / 10;
alert(a);
a = a - 10;
alert(a);
a = a * 10;      
alert(a);

//유지보수가 편하다
```

