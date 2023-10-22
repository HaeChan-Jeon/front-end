## CSS 사용자 지정 속성 (Custom Properties)

CSS 사용자 지정 속성 (또는 CSS 변수라고도 함)은 CSS 값을 저장하고 이 값을 여러 곳에서 재사용 할 수 있게 해주는 기능입니다. 사용자 지정 속성은 `--` 접두사로 시작합니다.

### 사용자 지정 속성 선언하기:
```css
:root {
  --main-color: #ff4500;
}
```

### 사용자 지정 속성 사용하기:
```css
header {
  background-color: var(--main-color);
}
```

## `calc()` 함수

`calc()`는 CSS에서 수학적 계산을 수행하는 함수입니다. 사칙 연산 (덧셈, 뺄셈, 곱셈, 나눗셈)을 지원하며, 여러 단위의 값들을 조합하여 연산할 수 있습니다.

### `calc()` 사용 예:

1. **픽셀과 백분율 혼합하기**:
```css
div {
  width: calc(100% - 20px);
}
```

2. **두 개의 변수를 사용하여 계산하기**:
```css
:root {
  --padding: 10px;
  --border: 5px;
}

div {
  width: calc(100% - var(--padding) - var(--border));
}
```

---

## 통합 예제:

```css
:root {
  --main-color: #ff4500;
  --secondary-color: #333;
  --sidebar-width: 250px;
}

body {
  font-family: 'Arial', sans-serif;
  background-color: var(--secondary-color);
}

header {
  background-color: var(--main-color);
  padding: 20px;
  color: white;
}

.sidebar {
  width: var(--sidebar-width);
  background-color: var(--main-color);
  color: white;
}

.content {
  margin-left: calc(var(--sidebar-width) + 20px);
}
```

위의 예제에서, 우리는 `--main-color`, `--secondary-color`, 그리고 `--sidebar-width`라는 세 개의 사용자 지정 속성을 선언했습니다. 이러한 변수는 CSS 전체에서 사용될 수 있으며, 필요에 따라 쉽게 변경될 수 있습니다. 또한 `calc()` 함수를 사용하여 `.content` 영역의 `margin-left` 값을 계산하였습니다.
