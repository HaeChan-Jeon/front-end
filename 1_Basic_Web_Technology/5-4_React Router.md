React Router는 React 애플리케이션에서 라우팅을 구현하기 위한 표준 라이브러리 중 하나입니다. 이 라이브러리를 사용하면 싱글 페이지 애플리케이션(SPA)에서 클라이언트 사이드 라우팅을 쉽게 구현할 수 있으며, 사용자가 다른 페이지로 이동할 때마다 페이지를 새로고침하지 않고도 컴포넌트를 렌더링할 수 있습니다.

React Router는 다음과 같은 주요 컴포넌트와 훅을 제공합니다:

- `BrowserRouter`: HTML5 history API를 사용해 URL과 UI를 동기화하는 라우터입니다.
- `Route`: URL과 UI의 특정 부분을 매핑하는 데 사용됩니다.
- `Link`: 클릭할 때마다 페이지를 새로고침하지 않고도 뷰를 변경할 수 있는 선언적인 방법을 제공합니다.
- `Switch`: 여러 `Route` 중에서 첫 번째로 매칭되는 컴포넌트만 렌더링하도록 합니다.
- `useHistory`, `useLocation`, `useParams`, `useRouteMatch`: 현재 라우트에 대한 정보를 얻거나 라우트를 조작할 때 사용하는 훅들입니다.

React Router v6부터는 `Switch` 대신 `Routes` 컴포넌트가 도입되었고, 라우트 매칭 로직이 개선되어 보다 명확하고 예측 가능한 라우트 매칭이 가능해졌습니다.

### 기본 사용법

React Router를 사용하는 기본적인 방법은 다음과 같습니다:

1. `BrowserRouter`를 애플리케이션의 최상위에 위치시킵니다.
2. `Route` 컴포넌트를 사용하여 경로와 컴포넌트를 매핑합니다.
3. `Link` 컴포넌트를 사용하여 라우트 간에 이동합니다.

예를 들어, 다음과 같이 간단한 라우팅을 설정할 수 있습니다:

```jsx
import React from 'react';
import { BrowserRouter as Router, Route, Link } from 'react-router-dom';

function App() {
  return (
    <Router>
      <div>
        <nav>
          <ul>
            <li>
              <Link to="/">Home</Link>
            </li>
            <li>
              <Link to="/about">About</Link>
            </li>
            <li>
              <Link to="/users">Users</Link>
            </li>
          </ul>
        </nav>

        {/* Route 컴포넌트를 사용하여 경로를 설정 */}
        <Route path="/" exact component={Home} />
        <Route path="/about" component={About} />
        <Route path="/users" component={Users} />
      </div>
    </Router>
  );
}

function Home() {
  return <h2>Home</h2>;
}

function About() {
  return <h2>About</h2>;
}

function Users() {
  return <h2>Users</h2>;
}

export default App;
```

위의 예제에서는 `BrowserRouter`를 사용하여 SPA의 라우팅 컨텍스트를 설정하고, `Link` 컴포넌트로 내비게이션을 구성하며, `Route` 컴포넌트로 해당 경로에 렌더링할 컴포넌트를 지정합니다.

### 동적 라우팅

동적 라우팅은 특정 패턴의 경로에 대응하여 컴포넌트를 렌더링할 수 있게 해줍니다. 예를 들어, 사용자의 ID에 따라 다른 프로필 페이지를 보여주고 싶을 때 사용할 수 있습니다:

```jsx
<Route path="/users/:id" component={UserProfile} />
```

이 경우 `:id` 부분은 어떤 문자열이 와도 매칭되며, `UserProfile` 컴포넌트 내에서 `useParams` 훅을 사용해 해당 값을 얻을 수 있습니다:

```jsx
import { useParams } from 'react-router-dom';

function UserProfile() {
  let { id } = useParams();
  return <div>User Profile for user: {id}</div>;
}
```

### 정리

React Router는 React 애플리케이션에 라우팅 기능을 추가하는 강력하고 유연한 방법을 제공합니다. 간단한 SPA부터 복잡한 대규모 애플리케이션에 이르기까지, React Router를 사용하면 사용자 경험을 개선하고 애플리케이션의 구조를 더욱 명확하게 할 수 있습니다.
