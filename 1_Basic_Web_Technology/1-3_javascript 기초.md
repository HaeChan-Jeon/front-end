JavaScript는 웹 개발에서 핵심적인 역할을 하는 프로그래밍 언어이다.
웹 페이지의 동적인 요소를 구현하고, 사용자와 상호작용을 할 때 주로 사용된다.
아래는 JavaScript의 기초에 대한 간단한 안내이다.

1. 변수와 데이터 타입

JavaScript에서는 다양한 데이터 타입과 변수를 사용할 수 있다.

변수: var, let, const 키워드를 사용하여 선언한다.

데이터 타입: string, number, boolean, null, undefined, object, symbol 등이 있다.

```javascript
let name = "John";
const age = 30;
var isStudent = false;
```

2. 연산자

JavaScript는 다양한 연산자를 제공한다:
산술 연산자(+, -, *, /), 비교 연산자(==, ===, !=, !==, <, >, <=, >=), 논리 연산자(&&, ||, !) 등이 있다.

```javascript
let sum = 5 + 3; // 8
let isEqual = 5 === 3; // false
```

3. 조건문

if, else if, else를 사용하여 조건문을 작성할 수 있다.

```javascript
if (age > 18) {
    console.log("Adult");
} else {
    console.log("Minor");
}
```

4. 반복문

for, while, do-while 등의 반복문을 사용하여 코드를 여러 번 실행할 수 있다.

```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

5. 함수

function 키워드를 사용하여 함수를 정의하고, ()를 사용하여 함수를 호출합니다.

```javascript
function greet(name) {
    console.log("Hello, " + name + "!");
}

greet("John");
```

6. 객체

JavaScript에서 객체는 키와 값을 가진 컬렉션이다.

```javascript
let person = {
    name: "John",
    age: 30,
    greet: function() {
        console.log("Hello, my name is " + this.name);
    }
};

person.greet();
```

7. 배열

배열은 여러 값을 하나의 변수에 저장할 수 있다.

```javascript
let fruits = ["apple", "banana", "cherry"];
console.log(fruits[0]); // apple
```

8. DOM 조작

JavaScript를 사용하여 웹 페이지의 DOM(Document Object Model)을 조작할 수 있다.

```javascript
document.getElementById("myButton").addEventListener("click", function() {
    alert("Button clicked!");
});
```

9. 이벤트 핸들링

JavaScript를 사용하여 웹 페이지에서 발생하는 이벤트를 감지하고 반응할 수 있다.

```javascript
document.getElementById("myButton").onclick = function() {
    alert("Button was clicked!");
};
```

이러한 기초적인 개념들은 JavaScript를 이해하고 웹 개발을 시작하는 데 있어 기본적이면서도 중요한 단계이다.
각 섹션에 대해 더 깊게 학습하면, JavaScript의 다양한 기능과 활용 방법에 대해 더욱 잘 이해할 수 있을 것이다.
