### HTML 기초

* HTML(HyperText Markup Language)은 웹 페이지를 구조화하고 의미를 부여하는 기본적인 웹 기술이다. HTML은 여러 요소(Elements)로 구성되며, 이러한 요소들은 웹 페이지에서 다양한 콘텐츠(텍스트, 이미지, 링크 등)를 표현한다. HTML 기초를 이해하면 웹 페이지의 기본 구조를 이해하고, 간단한 웹사이트를 만들 수 있게 된다.

***

## HTML 기본 구조

* HTML 문서는 기본적으로 아래와 같은 구조를 가지고 있다.

```HTML
<!DOCTYPE html>
<html>
<head>
    <title>My First HTML Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

* `<!DOCTYPE html>` : 문서 타입 선언으로, 현재 문서가 HTML5 문서임을 나타낸다.
  * 문서 타입 선언(DOCTYPE)은 HTML 문서의 첫 줄에 위치해 있으며, 웹 브라우저<sup id="a1">[1](#footnote1)</sup>에게 해당 문서가 사용하는 HTML 버전을 알려주는 역할을 수행한다. 즉, 웹 브라우저는 이 DOCTYPE 선언을 통해 문서를 올바르게 렌더링<sup id="a1">[2](#footnote1)</sup>하는 방법을 알 수 있다.
  * HTML은 이전 버전의 HTML에서 여러 가지 새로운 기능, API(Application Programming Interface) 및 동작을 도입하여 웹 개발자들이 더 다양하고, 강력한 웹 사이트와 어플리케이션을 만들 수 있도록 한 HTML의 최신 버전이다.
* `<html>` : HTML 문서의 시작과 끝을 나타내는 태그이다.
* `<head>` : 웹 페이지의 메타 정보, CSS 스타일, 외부 파일 링크 등의 정보를 담고 있다.
* `<title>` : 웹 브라우저의 탭에 표시되는 웹 페이지의 제목을 정의한다.
* `<body>` : 웹 페이지의 주요 콘텐츠를 담는 부분으로, 텍스트, 이미지, 링크, 리스트 등 다양한 요소를 포함할 수 있다.

***

### 각주

<b id="footnote1">1</b> 웹 브라우저는 Google Chrome, Microsoft Edge와 같이 인터넷을 통해 웹 페이지를 검색하고, 표시하며, 탐색할 수 있게 해주는 소프트웨어 응용 프로그램을 의미한다. [↩](#a1)
<br>
<b id="footnote1">2</b> 웹 브라우저는 HTML, CSS 및 자바스크립트와 같은 웹 기술을 해석하고 렌더링하여 사용자에게 웹 페이지의 시각적 표현을 제공한다. [↩](#a1)
