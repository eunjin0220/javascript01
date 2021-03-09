---
description: '컴퓨터에게 반복적인 작업을 지시하는 방법이다. (loop,iterate)'
---

# 반복문

## while문

```javascript
while (조건){
    반복해서 실행할 코드
} //조건이 true에서 false가 될 때까지 반복적으로 실행
```

### 반복조건

```javascript
var i = 0; // 종료조건

while(i < 10){
    document.write('coding everybody <br />');
    i++;
}
// 1. i가 10보다 작을 경우 'coding everybody <br />' 출력
// 2. i의 값이 1씩 증가
// 3. 반복이 실행되며 i가 10과 같거나 커질 경우 종료
```

## for문

```javascript
for(초기화; 반복조건; 반복이 될 때마다 실행되는 코드){
    반복해서 실행될 코드
}

for(var i = 0; i < 10; i++){
    document.write('coding everybody'+i+'<br />');
}
```

## 반복문의 제어

### break

```javascript
for(var i = 0; i < 10; i++){
    if(i === 5) {
        break; //반복문을 즉시 종료
    }
    document.write('coding everybody'+i+'<br />');
}

// 코드 결과
// coding everybody 0
// coding everybody 1
// coding everybody 2
// coding everybody 3
// coding everybody 4

```

### continue

```javascript
for(var i = 0; i < 10; i++){
    if(i === 5) {
        continue;
        //실행을 중단하여 이후의 내용은 실행되지 않는다
        //반복문은 계속 유지
    }
    document.write('coding everybody'+i+'<br />');
}
```

## 반복문의 중첩        

```javascript
for(var i = 0; i < 10; i++){
    for(var j = 0; j < 10; j++){
        document.write('coding everbody'+i+j+'<br />');
    }
}
// 1. i = 1번 실행될때 j = 10번실행
// i = 0 , j = 0..9 -> 00..09)
// 2. 안에있는 j반복문이 종료시 밖에있는 i가 다시 실행
// i = 1 , j = 0..9 -> 10..19)

// 코드 결과
// coding everbody00 ... coding everbody99
```

