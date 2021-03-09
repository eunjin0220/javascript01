---
description: 문자열에서 특정한 문자를 찾아내는 도구
---

# 정규표현식

#### 정규표현식 생성은 '컴파일'과 '실행' 두가지 단계로 이루어진다.

## 컴파일 : 검출하고자 하는 패턴을 만드는 일

### 정규표현식 리터럴

```javascript
var pattern = /a/;
//찾고자 하는 a를 pattern이라는 변수에 저장
```

### 정규표현식 객체 생성자

```javascript
var pattern = new RegExp('a');
```

## 

> **정규표현식을 통해서 하는 주요 작업**
>
> 추출 - 필요한 정보를 추출하는 것
>
>  test - 확인하고자 하는 정보가 있는지 없는지 테스트하는 것
>
>  치환 -  검색된 정보를 다른 정보로 치환하는 것\(바꾸어 놓는 일\)



## 정규표현식 메소드 실행

### RegExp.exec\(\)

> 정규표현식이 찾고자 하는 대상을 첫번째 인자로 전달해서 패턴이 찾는 정보를 대상에서 찾아 배열로 리턴하는 메소드 \(추출역할\)

```javascript
var pattern = /a/;
pattern.exec('abcde');
// ['a']

var pattern = /a./; // . : 하나의 문자
pattern.exec('abcde');
// ['ab'] = 하나의 문자만 오면 되기때문에 a뒤에있던 b가 리턴됨

var pattern = /a/;
pattern.exec('bcde');
// null(찾고자 하는 결과가 없다는 의미)
```

### RegExp.test\(\)

> 인자 안에 패턴에 해당되는 문자열이 있다면 true, 없다면 false를 리턴 \(테스트역할\)

```javascript
var pattern = /a/;
pattern.test('abcde');
// true

var pattern = /a/;
pattern.test('bcde');
// false
```

## 문자열 메소드 실행

### String.match\(\)

```javascript
var pattern = /a/;
var str = 'abcdef';
str.match(pattern);
//['a']
```

### String.replace\(\)

```javascript
var pattern = /a/;
var str = 'abcdef';
str.replace(pattern, 'A');
//['A'] = 문자열에서 패턴을 검색하여 이를 변경 후 변경된 값을 리턴 
```

