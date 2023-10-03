# HTML 기초

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

<p align="center">
  <img src="https://github.com/HaeChan-Jeon/front-end/assets/146603024/ac5a1dbb-1ec2-477e-8606-9ec826948bf9" alt="HTML 기초 예시"/>
    HTML 기초 예시
</p>

* `<!DOCTYPE html>` : 문서 타입 선언으로, 현재 문서가 HTML5 문서임을 나타낸다.

  * 문서 타입 선언(DOCTYPE)은 HTML 문서의 첫 줄에 위치해 있으며, 웹 브라우저<sup id="a1">[1](#footnote1)</sup>에게 해당 문서가 사용하는 HTML 버전을 알려주는 역할을 수행한다. 즉, 웹 브라우저는 이 DOCTYPE 선언을 통해 문서를 올바르게 렌더링<sup id="a1">[2](#footnote1)</sup>하는 방법을 알 수 있다.
  
  * HTML은 이전 버전의 HTML에서 여러 가지 새로운 기능, API(Application Programming Interface)<sup id="a1">[3](#footnote1)</sup> 및 동작을 도입하여 웹 개발자들이 더 다양하고, 강력한 웹 사이트와 어플리케이션을 만들 수 있도록 한 HTML의 최신 버전이다.

* `<html>` : HTML 문서의 시작과 끝을 나타내는 태그(Tag)이다.

  * 태그(tag)는 HTML에서 요소를 정의하고, 문서의 구조와 컨텐츠를 마크업(Markup)<sup id="a1">[4](#footnote1)</sup>하기 위해 사용되는 꺾쇠 괄호(<>)로 둘러싸인 키워드 또는 식별자이다.

* `<head>` : 웹 페이지의 메타 정보, CSS 스타일, 외부 파일 링크 등의 정보를 담고 있다.

    * CSS(Cascading Style Sheets)는 웹 페이지의 디자인과 레이아웃을 꾸미고 제어하기 위한 스타일 규칙 언어다.
 
    * HTML 문서의 <head> 섹션 내에서 CSS 스타일을 사용하는 기본적인 예시를 아래와 같다. 아래 예시에서 `<style>` 태그 내에 CSS 규칙들이 정의되어 있다.

    * `body`에는 배경 색상, `h1`에는 텍스트 색상과 정렬 방식, 그리고 `p`에는 폰트 패밀리에 관한 스타일이 적용되어 있다. 이러한 스타일 규칙들은 HTML 문서의 각 해당 요소에 적용된다.

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Stylish Page</title>
    <style>
        body {
            background-color: lightblue;
        }
        h1 {
            color: white;
            text-align: center;
        }
        p {
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Stylish Page</h1>
    <p>This page is styled with CSS in the head section!</p>
</body>
</html>
```

<p align="center">
  <img src="https://github.com/HaeChan-Jeon/front-end/assets/146603024/909e410c-88d7-4899-ab3f-1f043539bac6" alt="CSS 스타일 예시"/>
    CSS 스타일 예시
</p>

* `<title>` : 웹 브라우저의 탭에 표시되는 웹 페이지의 제목을 정의한다.

* `<body>` : 웹 페이지의 주요 콘텐츠를 담는 부분으로, 텍스트, 이미지, 링크, 리스트 등 다양한 요소를 포함할 수 있다.

## 주요 HTML 태그

* `<h1>, <h2>, ..., <h6>` : 제목 태그로, 숫자가 작을수록 더 큰 제목을 나타낸다.

* `<p>` : 문단(Paragraph)을 정의한다.

* `<a>` : 하이퍼링크를 생성한다. 예: `<a href="https://www.example.com">Visit our website</a>`

* `<img>` : 이미지를 삽입한다. 예: `<img src="image.jpg" alt="Description of image">`

* `<ul>` : 번호 없는 리스트를 생성하고, `<li>` 태그로 각 항목을 정의한다.

* `<ol>` : 번호 있는 리스트를 생성하고, `<li>` 태그로 각 항목을 정의한다.

* `<table>` : 표를 생성한다. `<tr>`로 행을, `<th>`로 헤더 셀을, `<td>`로 데이터 셀을 정의한다.

***

# 각주

<b id="footnote1">1. </b> 웹 브라우저는 Google Chrome, Microsoft Edge와 같이 인터넷을 통해 웹 페이지를 검색하고, 표시하며, 탐색할 수 있게 해주는 소프트웨어 응용 프로그램을 의미한다. [↩](#a1)
<br>
<b id="footnote1">2. </b> HTML, CSS 및 자바스크립트와 같은 웹 기술을 해석하여 사용자에게 웹 페이지의 시각적 표현을 제공한다. [↩](#a1)
<br>
<b id="footnote1">3. </b> API(Application Programming Interface)는 소프트웨어 어플리케이션들이 서로 상호작용하고 통신하기 위한 정의된 규약(서로 지키도록 정한 규칙) 세트를 의미한다. [↩](#a1)
<br>
<b id="footnote1">4. </b> 마크업(Markup)은 텍스트에 메타데이터(Metadata, 데이터를 설명하기 위한 데이터)를 추가하여 그 구조나 표현을 설명하는 태그 또는 기호를 사용하는 것을 의미한다. [↩](#a1)
