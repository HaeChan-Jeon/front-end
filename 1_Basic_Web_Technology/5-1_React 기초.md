### React란?

React는 Facebook에서 만든 사용자 인터페이스를 구축하기 위한 JavaScript 라이브러리입니다. React를 사용하면 대규모 애플리케이션에서도 데이터가 변경될 때마다 전체 페이지를 다시 불러오지 않고, 변경된 부분만 업데이트할 수 있습니다.

### 주요 개념

1. **컴포넌트 (Component)**  
React는 컴포넌트 기반으로 구축됩니다. 컴포넌트는 UI의 독립적인 재사용 가능한 부분을 나타냅니다. 각 컴포넌트는 자신만의 상태와 라이프사이클 메서드를 가질 수 있습니다.

2. **상태 (State) 및 속성 (Props)**  
컴포넌트 내부에서 관리되는 데이터를 '상태'라고 합니다. 상태는 컴포넌트 내에서 변경될 수 있으며, 이 변경에 따라 컴포넌트는 다시 렌더링됩니다. 속성은 부모 컴포넌트로부터 자식 컴포넌트로 전달되는 데이터를 의미합니다.

3. **Virtual DOM**  
React는 Virtual DOM을 사용하여 실제 DOM의 변경을 최소화합니다. 데이터가 변경될 때마다 React는 Virtual DOM에 변경을 반영하고, 변경된 부분만 실제 DOM에 반영합니다. 이 방식은 성능 향상에 크게 기여합니다.

### React 시작하기

1. **React 설치**  
React를 시작하기 위해 `create-react-app` 도구를 사용할 수 있습니다. 이 도구는 React 프로젝트의 기본 구조를 제공합니다.

```bash
npx create-react-app my-app
```

2. **컴포넌트 생성하기**  
React 애플리케이션은 여러 컴포넌트로 구성됩니다. 컴포넌트는 다음과 같이 생성할 수 있습니다:

```javascript
import React from 'react';

class MyComponent extends React.Component {
    render() {
        return <h1>Hello, React!</h1>;
    }
}
```

3. **상태와 속성 사용하기**  
컴포넌트 내에서 상태와 속성을 사용하여 동적인 데이터를 표시할 수 있습니다.

```javascript
class MyComponent extends React.Component {
    constructor(props) {
        super(props);
        this.state = { count: 0 };
    }

    render() {
        return (
            <div>
                <h1>Hello, {this.props.name}!</h1>
                <p>Count: {this.state.count}</p>
            </div>
        );
    }
}
```
