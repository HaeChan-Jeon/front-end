비동기 프로그래밍은 특히 웹 개발과 같은 환경에서 매우 중요한 개념입니다. 웹에서는 네트워크 요청, 타이머, 이벤트 리스너와 같은 다양한 요소가 비동기적으로 동작하기 때문입니다. JavaScript는 비동기 코드를 작성하고 관리하기 위한 여러 도구와 패턴을 제공합니다. 이 중에서도 Promises와 Async/Await는 비동기 코드를 작성할 때 가장 널리 사용되는 패턴 중 하나입니다.

## 1. Promises

Promise는 JavaScript에서 비동기 연산의 최종 완료 (또는 실패)와 그 결과 값을 나타내는 객체입니다.

### 기본 구조

```javascript
let promise = new Promise((resolve, reject) => {
    // 비동기 작업
    if (/* 작업 성공 */) {
        resolve('결과 값');
    } else {
        reject('에러 메시지');
    }
});

promise.then(result => {
    console.log(result); // '결과 값' 출력
}).catch(error => {
    console.log(error); // '에러 메시지' 출력
});
```

### 주요 메서드

1. **then()**: Promise가 성공적으로 완료되었을 때 호출되는 콜백을 등록합니다.
2. **catch()**: Promise가 실패했을 때 호출되는 콜백을 등록합니다.
3. **finally()**: Promise의 성공 또는 실패 여부와 관계없이 항상 호출되는 콜백을 등록합니다.

## 2. Async/Await

Async/Await는 JavaScript에서 비동기 코드를 동기적인 방식으로 작성할 수 있게 하는 문법입니다.

### 기본 구조

```javascript
async function myFunction() {
    try {
        let result = await someAsyncFunction();
        console.log(result);
    } catch (error) {
        console.log(error);
    }
}
```

### 주요 특징

1. **async**: 함수 앞에 `async` 키워드를 사용하면 해당 함수는 항상 Promise를 반환합니다.
2. **await**: `await` 키워드는 Promise의 완료를 기다립니다. `await`는 오직 `async` 함수 내에서만 사용될 수 있습니다.
