
웹 폼 (Web Forms)
웹 폼은 웹 페이지에서 사용자로부터 정보를 수집하기 위한 GUI 요소입니다. 사용자는 웹 폼을 통해 텍스트, 선택 사항, 체크 박스 등을 입력하고, 이 정보는 서버로 전송되어 처리됩니다.

폼의 주요 구성 요소
**<form>**: HTML에서 폼을 정의하는 태그입니다.
**<input>**: 사용자로부터 데이터를 입력받는 필드를 정의합니다.
**<label>**: 입력 필드의 레이블을 정의합니다.
**<select>**: 드롭다운 목록을 생성합니다.
**<option>**: <select> 태그 내에서 선택 가능한 옵션을 정의합니다.
**<textarea>**: 여러 줄의 텍스트 입력을 위한 필드를 생성합니다.
**<button>**: 사용자가 클릭할 수 있는 버튼을 정의합니다.

```html
Copy code
<form action="/submit" method="POST">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name"><br><br>
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email"><br><br>
    
    <input type="submit" value="Submit">
</form>
```

입력 필드 (Input Fields)
주요 유형
text: 일반 텍스트 입력 필드입니다.
password: 비밀번호 입력 필드로, 입력된 텍스트를 마스킹합니다.
checkbox: 사용자가 여러 옵션 중 하나 이상을 선택할 수 있게 합니다.
radio: 사용자가 여러 옵션 중 하나만 선택할 수 있게 합니다.
submit: 폼을 제출하는 버튼입니다.

```html
Copy code
<input type="text" name="username" placeholder="Username">
<input type="password" name="password" placeholder="Password">
<input type="checkbox" name="subscribe" value="yes"> Subscribe to newsletter
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
<input type="submit" value="Sign Up">
```

폼 처리
폼 데이터는 일반적으로 서버로 전송되어 처리됩니다. 웹 폼은 GET 또는 POST HTTP 메소드를 사용하여 데이터를 서버로 전송할 수 있습니다.

GET: 데이터를 URL의 일부로 전송합니다.
POST: 데이터를 HTTP 메시지 본문의 일부로 전송합니다.
유효성 검사 (Validation)
폼을 제출하기 전에 클라이언트 측 또는 서버 측에서 데이터의 유효성을 검사하는 것이 중요합니다. 유효성 검사를 통해 올바르지 않은 또는 누락된 데이터가 서버로 전송되는 것을 방지할 수 있습니다.

예제 코드: HTML5 유효성 검사
```html
Copy code
<input type="text" name="username" required>
<input type="email" name="email" required>
<input type="number" name="age" min="18" required>
```
결론
웹 폼은 사용자와 상호 작용하고 정보를 수집하는 데 필수적인 요소입니다. 폼과 입력 필드를 통해 다양한 유형의 데이터를 안전하게 수집하고, 유효성 검사를 통해 데이터의 정확성을 보장할 수 있습니다. 이는 웹 애플리케이션에서 정보를 안전하게 처리하고 사용자 경험을 향상시키는 데 중요한 단계입니다.
