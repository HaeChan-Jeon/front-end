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

  * 문서 타입 선언(DOCTYPE)은 HTML 문서의 첫 줄에 위치해 있으며, 웹 브라우저<sup id="a1">[1](#footnote1)</sup>에게 해당 문서가 사용하는 HTML 버전을 알려주는 역할을 수행한다. 즉, 웹 브라우저는 이 DOCTYPE 선언을 통해 문서를 올바르게 렌더링<sup id="a2">[2](#footnote2)</sup>하는 방법을 알 수 있다.
  
  * HTML은 이전 버전의 HTML에서 여러 가지 새로운 기능, API(Application Programming Interface)<sup id="a3">[3](#footnote3)</sup> 및 동작을 도입하여 웹 개발자들이 더 다양하고, 강력한 웹 사이트와 어플리케이션을 만들 수 있도록 한 HTML의 최신 버전이다.

* `<html>` : HTML 문서의 시작과 끝을 나타내는 태그(Tag)이다.

  * 태그(tag)는 HTML에서 요소를 정의하고, 문서의 구조와 컨텐츠를 마크업(Markup)<sup id="a4">[4](#footnote4)</sup>하기 위해 사용되는 꺾쇠 괄호(<>)로 둘러싸인 키워드 또는 식별자이다.

* `<head>` : 웹 페이지의 메타 정보, CSS 스타일, 외부 파일 링크 등의 정보를 담고 있다.

    * CSS(Cascading Style Sheets)는 웹 페이지의 디자인과 레이아웃을 꾸미고 제어하기 위한 스타일 규칙 언어이다.
 
    * HTML 문서의 <head> 섹션 내에서 CSS 스타일을 사용하는 기본적인 예시는 아래와 같다. 아래 예시에서 `<style>` 태그 내에 CSS 규칙들이 정의되어 있다.

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

* `<body>` : 웹 페이지의 주요 콘텐츠를 담는 부분으로 텍스트, 이미지, 링크, 리스트 등 다양한 요소를 포함할 수 있다.

## 주요 HTML 태그

* `<h1>, <h2>, ..., <h6>` : 제목 태그로, 숫자가 작을수록 더 큰 제목을 나타낸다.

* `<p>` : 문단(Paragraph)을 정의한다.

* `<a>` : 하이퍼링크를 생성한다. 예: `<a href="https://www.example.com">Visit our website</a>`

* `<img>` : 이미지를 삽입한다. 예: `<img src="image.jpg" alt="Description of image">`

* `<ul>` : 번호 없는 리스트를 생성하고, `<li>` 태그로 각 항목을 정의한다.

* `<ol>` : 번호 있는 리스트를 생성하고, `<li>` 태그로 각 항목을 정의한다.

* `<table>` : 표를 생성한다. `<tr>`로 행을, `<th>`로 헤더 셀을, `<td>`로 데이터 셀을 정의한다.

<br>

* 아래 예제는 기본적인 HTML 구조와 몇 가지 주요 HTML 요소를 사용하여 웹 페이지를 구성한다. `<h1>`부터 `<h3>`까지의 제목 태그, `<p>`로 문단, `<a>`로 하이퍼링크, `<img>`로 이미지, `<ul>`과 `<ol>`로 리스트, 그리고 `<table>`로 표를 만든다. 이 코드를 HTML 파일로 저장하고 웹 브라우저로 열면, 위에서 정의한 요소들을 시각적으로 확인할 수 있다.

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Example</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <h2>Subheading</h2>

    <p>This is a paragraph explaining what my website is about. It provides information and resources on various topics.</p>

    <a href="https://www.example.com">Visit Example Website</a>

    <img src="image.jpg" alt="A beautiful scenery">

    <h3>Unordered List</h3>
    <ul>
        <li>Apple</li>
        <li>Banana</li>
        <li>Cherry</li>
    </ul>

    <h3>Ordered List</h3>
    <ol>
        <li>First item</li>
        <li>Second item</li>
        <li>Third item</li>
    </ol>

    <h3>Table Example</h3>
    <table border="1">
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
        <tr>
            <td>Data 1</td>
            <td>Data 2</td>
        </tr>
        <tr>
            <td>Data 3</td>
            <td>Data 4</td>
        </tr>
    </table>
</body>
</html>
```

<p align="center">
  <img src="https://github.com/HaeChan-Jeon/front-end/assets/146603024/273e45ca-ac7d-4454-95c7-48578b9d5b93" alt="HTML 주요 태그 예시"/>
    HTML 주요 태그 예시
</p>

* `<meta name="viewport" content="width=device-width, initial-scale=1.0">`는 웹 페이지가 모바일 기기나 다양한 화면 크기의 기기에서 어떻게 보여질지를 제어하는 HTML 태그이다. 이 태그는 웹 페이지가 반응형 웹 디자인(Responsive Web Design)<sup id="a5">[5](#footnote5)</sup>을 사용하여 다양한 화면 크기에 적절하게 보여지도록 돕는다.
	* `name="viewport"` : 이 속성은 메타데이터의 종류를 정의한다. `"viewport"`는 브라우저의 뷰포트(viewport)<sup id="a6">[6](#footnote6)</sup> 설정과 관련된 메타데이터임을 나타낸다.
	* `content="width=device-width`, `initial-scale=1.0"` : 이 속성은 `name="viewport"`에 대한 설정 값을 제공한다. 여기서 두 가지 주요 설정은 아래와 같다.
		* `width=device-width` : 이 설정은 뷰포트의 너비를 기기의 스크린 너비로 설정한다. 즉, 웹 페이지의 너비가 사용자의 기기 화면 너비와 일치하도록 만든다.
		* `initial-scale=1.0` : 이 설정은 웹 페이지의 초기 확대 레벨을 설정한다. `"1.0"`은 웹 페이지가 처음 로드될 때 100%의 확대 레벨(즉, 확대나 축소 없이)로 표시되도록 한다.

***

# 각주

<b id="footnote1">1. </b> 웹 브라우저는 Google Chrome, Microsoft Edge와 같이 인터넷을 통해 웹 페이지를 검색하고, 표시하며, 탐색할 수 있게 해주는 소프트웨어 응용 프로그램을 의미한다. [↩](#a1)
<br>
<b id="footnote2">2. </b> HTML, CSS 및 자바스크립트와 같은 웹 기술을 해석하여 사용자에게 웹 페이지의 시각적 표현을 제공한다. [↩](#a2)
<br>
<b id="footnote3">3. </b> API(Application Programming Interface)는 소프트웨어 어플리케이션들이 서로 상호작용하고 통신하기 위한 정의된 규약(서로 지키도록 정한 규칙) 세트를 의미한다. [↩](#a3)
<br>
<b id="footnote4">4. </b> 마크업(Markup)은 텍스트에 메타데이터(Metadata, 데이터를 설명하기 위한 데이터)를 추가하여 그 구조나 표현을 설명하는 태그 또는 기호를 사용하는 것을 의미한다. [↩](#a4)
<br>
<b id="footnote5">5. </b> 반응형 웹 디자인(Responsive Web Design)은 다양한 화면 크기와 해상도를 가진 기기에서 웹사이트의 레이아웃과 디자인이 동적으로 변화하여 최적의 사용자 경험을 제공하는 웹 디자인 접근 방식이다. [↩](#a5)
<br>
<b id="footnote6">6. </b> 뷰포트(Viewport)는 웹페이지가 사용자에게 보여지는 영역으로, 기기의 화면 크기에 따라 다르며, 웹 디자인에서 이 영역을 기준으로 콘텐츠가 어떻게 표시될지를 정의한다. [↩](#a6)
