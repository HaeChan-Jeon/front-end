### 1. `let`과 `const`
ES6에서는 변수 선언에 두 가지 새로운 키워드인 `let`과 `const`가 도입되었습니다.
- `let`: 블록 스코프를 가진 변수 선언입니다.
- `const`: 블록 스코프를 가지며, 한 번 할당된 값을 변경할 수 없는 상수입니다.

### 2. 화살표 함수 (Arrow Functions)
화살표 함수는 간결한 문법을 사용하여 함수를 정의할 수 있게 해줍니다.
```javascript
const add = (a, b) => a + b;
```

### 3. 템플릿 리터럴 (Template Literals)
백틱 (`)을 사용하여 문자열을 정의하면, 변수와 표현식을 문자열 안에 직접 삽입할 수 있습니다.
```javascript
let name = "John";
console.log(`Hello, ${name}!`);
```

### 4. 클래스 (Classes)
ES6에서는 클래스 기반의 객체 지향 프로그래밍을 쉽게 구현할 수 있도록 클래스 문법이 도입되었습니다.
```javascript
class Person {
  constructor(name) {
    this.name = name;
  }

  greet() {
    console.log(`Hello, ${this.name}!`);
  }
}
```

### 5. 모듈 (Modules)
ES6에서는 모듈화된 코드를 작성하고 관리할 수 있게 됩니다. `import`와 `export` 키워드를 사용하여 모듈을 가져오거나 내보낼 수 있습니다.

### 6. 비구조화 할당 (Destructuring)
배열이나 객체의 요소를 간편하게 변수에 할당할 수 있습니다.
```javascript
let [a, b] = [1, 2];
let {x, y} = {x: 10, y: 20};
```

### 7. 기본 매개변수 (Default Parameters)
함수 매개변수에 기본값을 할당할 수 있습니다.
```javascript
function greet(name = "World") {
  console.log(`Hello, ${name}!`);
}
```

### 8. 스프레드 연산자 (Spread Operator) & 나머지 매개변수 (Rest Parameters)
스프레드 연산자 (`...`)는 배열이나 객체를 확장하거나, 나머지 매개변수로 여러 인자를 배열로 그룹화할 수 있습니다.

### 9. 프로미스 (Promises)
비동기 작업을 더 깔끔하게 처리할 수 있는 객체입니다. `then`, `catch`, `finally` 메서드를 사용하여 비동기 작업의 성공, 실패, 완료 상태를 처리할 수 있습니다.

### 10. `async` & `await`
비동기 작업을 동기적으로 처리하는 것처럼 코딩할 수 있게 해주는 문법입니다. `async` 함수 안에서만 `await`를 사용할 수 있습니다.
