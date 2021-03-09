# 객체\(Object\)

## 객체의 생성

```javascript
var grades = {'egoing': 10, 'k8805': 6, 'sorialgi': 80};
//'egoing' = key , '10' = value

var grades = {};
grades['egoing'] = 10;
grades['k8805'] = 6;
grades['sorialgi'] = 80;

var grades = new Object();
grades['egoing'] = 10;
grades['k8805'] = 6;
grades['sorialgi'] = 80;

//필요한 값 가져오기
ar grades = {'egoing': 10, 'k8805': 6, 'sorialgi': 80};
alert(grades['sorialgi']); //80
```

## 객체와 반복문의 조우

```javascript
var grades = {'egoing': 10, 'k8805': 6, 'sorialgi': 80};
for(key in grades) {
    document.write("key : "+key+" value : "+grades[key]+"<br />");
}
// in뒤에 따라오는 배열의 key값을 변수에 담아 반복문 실행
// key : egoing value : 10
// key : k8805 value : 6
// key : sorialgi value : 80
```

## 객체지향 프로그래밍

```javascript
var grades = {
    'list' : {'egoing' : 10, 'k8805': 6, 'sorialgi': 80'}
    'show' : function(){
        for(var name in this.list){
            console.log(name,this.list[name]);
        }
    }
}
grades.show();
//코드 결과
// egoing 10
// k8805 6
// sorialgi 80

// 객체 = grades(그릇)
// 데이터= list
// 함수= grades(데이터 처리 함수)

```

