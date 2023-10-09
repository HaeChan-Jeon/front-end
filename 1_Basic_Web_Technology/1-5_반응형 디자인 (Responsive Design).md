# 반응형 디자인 (Responsive Design)

## 정의

반응형 웹 디자인은 웹사이트의 UI를 다양한 디스플레이 크기와 해상도에 맞게 최적화하여 사용자에게 최상의 사용 경험을 제공하는 디자인 접근 방식입니다.

## 특징

### 유연한 그리드 레이아웃

- 모든 디바이스에 대응하기 위해, 웹사이트는 유연한 그리드 레이아웃을 사용해야 합니다.
- 그리드 시스템은 여러 컬럼으로 구성되며, 브라우저 창의 크기에 따라 동적으로 리사이징됩니다.

### 유연한 이미지

- 이미지는 컨테이너 요소에 따라 크기가 동적으로 조절되어야 합니다.
- 이는 이미지가 뷰포트의 크기를 초과하지 않도록 보장하며, 사용자의 스크린 크기에 상관없이 콘텐츠를 적절히 표시합니다.

### 미디어 쿼리

- CSS 미디어 쿼리를 사용하여, 다양한 디스플레이 특성에 따라 스타일을 동적으로 적용할 수 있습니다.
- 예를 들어, 작은 화면의 디바이스에서는 한 컬럼 레이아웃을, 큰 화면에서는 멀티 컬럼 레이아웃을 보여줄 수 있습니다.

## 이점

1. **사용자 경험 향상**: 사용자는 디바이스에 상관없이 웹사이트를 쉽게 탐색하고 사용할 수 있습니다.
2. **유지보수의 용이성**: 하나의 코드베이스만 유지 관리하면 되므로 작업 효율이 증가합니다.
3. **검색 엔진 최적화 (SEO) 개선**: 검색 엔진은 사용자 친화적인 웹사이트를 높게 평가하며, 반응형 디자인은 이에 도움을 줍니다.

## 예시 코드

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Responsive Design Example</title>
</head>
<body>
    <header>
        <h1>Welcome to Our Responsive Website</h1>
    </header>
    <main>
        <p>This is a simple example of a responsive web page...</p>
    </main>
    <footer>
        <p>&copy; 2023 Responsive Design Co.</p>
    </footer>
</body>
</html>
```

- 이 코드 예시는 HTML과 CSS를 사용하여 기본적인 반응형 웹사이트를 만드는 방법을 보여줍니다. @media 쿼리를 사용하여 브라우저 창의 너비가 600px 이하일 때 배경색을 변경하는 간단한 예시를 포함하고 있습니다.

```CSS
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header, footer {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 10px;
}

main {
    margin: 15px;
    padding: 20px;
    background-color: lightgray;
}

@media only screen and (max-width: 600px) {
    body {
        background-color: lightblue;
    }
}
```
