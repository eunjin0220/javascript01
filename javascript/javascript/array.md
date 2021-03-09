---
description: 연관된 데이터를 모아서 통으로 관리하기 위해서 사용하는 데이터 타입(여러개)
---

# 배열\(Array\)

## 배열의 생성

```javascript
var member = ['egoing', 'k8805', 'sorialgi']
//각각의 데이터 = 원소(Element)

alert(member[0]);
alert(member[1]);
alert(member[2]);
//데이터를 꺼내올때 egoing :0 / k8805 :1 / sorialgi :2

function get_members(){
    return ['egoing', 'k8805', 'sorialgi'];
}
var members = get_members();
document.write(members[0]);
document.write(members[1]);
document.write(members[2]);
```

## 배열의 사용

```javascript
function get_members(){
    return ['egoing', 'k8805', 'sorialgi'];
}

members = get_members();

for(i = 0; i < members.length; i++){
    document.write(members[i].toUpperCase());   
    document.write('<br />');
}
// member.length = 배열에 담긴 값의 숫자
// members[i].toUpperCase() = 대문자로 변환
```

## 배열의 제어

복수의 데이터를 '효율적으로 관리', '전달'하기 위한 목적으로 고안된 데이터 타입

## 배열의 크기

```javascript
var arr = [1, 2, 3, 4, 5];
alert(arr.length);
```

## 배열의 조작

```javascript
var li = ['a', 'b', 'c', 'd', 'e'];
li.push('f'); //push : 원소추가
alert(li); //li = ['a', 'b', 'c', 'd', 'e' , 'f']

var li = ['a', 'b', 'c', 'd', 'e'];
li = li.concat(['f', 'g']); //concat : 여러개의 원소 추가
alert(li); //li = ['a', 'b', 'c', 'd', 'e' , 'f' , 'g']

var li = ['a', 'b', 'c', 'd', 'e'];
li.unshift('z'); //unshift : 시작지점으로 추가
alert(li); //li = ['z' , 'a', 'b', 'c', 'd', 'e' ]

var li = ['a', 'b', 'c', 'd', 'e'];
li.splice(2, 0, 'B');
// splice : 배열의 특정구간을 추출, 특정 구간에 특정 배열 추가
//li.splice(2(배열위치), 0(제거될 원소 수), 'B'(추가될 값))
alert(li); //li = ['a', 'b', 'B', 'c', 'd', 'e']
```

## 제거

```javascript
var li = ['a', 'b', 'c', 'd', 'e'];
li.shift(); //shift : 첫번째 원소 제거
alert(li); //li = ['b', 'c', 'd', 'e']

var li = ['b', 'c', 'd', 'e'];
li.pop(); //pop: 마지막 원소 제거
alert(li); //li = ['b', 'c', 'd']
```

## 정렬

```javascript
var li = ['c', 'e', 'a', 'b', 'd'];
li.sort(); //sort: 정렬
alert(li); //li = ['a', 'b', 'c', 'd', 'e']

var li = ['c', 'e', 'a', 'b', 'd'];
li.reverse(); //reverse: 역순 정렬
alert(li); //li = ['e', 'd', 'c', 'b, 'a']
```

