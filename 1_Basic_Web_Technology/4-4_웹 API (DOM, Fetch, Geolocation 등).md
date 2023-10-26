### 1. DOM (Document Object Model)

**정의**: 
DOM은 웹 페이지의 구조화된 표현을 제공하며, 프로그래밍 언어가 웹 페이지의 내용, 구조, 그리고 스타일을 조작할 수 있게 해줍니다. DOM은 웹 페이지의 요소와 속성을 객체로 나타내므로, JavaScript와 같은 스크립트 언어를 사용하여 이러한 객체들을 수정, 삭제, 추가할 수 있습니다.

**주요 기능**:
- 웹 페이지의 요소를 선택하거나 수정
- 이벤트 리스너 추가 및 제거
- 요소 생성 및 삭제

**예제**:
```javascript
document.getElementById("myId").textContent = "새로운 내용";
```

---

### 2. Fetch API

**정의**: 
Fetch API는 네트워크 요청을 쉽게 만들 수 있도록 제공되는 자바스크립트 인터페이스입니다. AJAX와 유사한 기능을 제공하지만, Promise 기반의 인터페이스를 갖추고 있어 더욱 강력하고 유연합니다.

**주요 기능**:
- 리소스를 가져오거나 저장
- 다양한 HTTP 메서드를 사용하여 요청
- Response 객체를 통해 상세한 응답 정보 접근

**예제**:
```javascript
fetch('https://api.example.com/data', {
  method: 'GET'
})
.then(response => response.json())
.then(data => console.log(data))
.catch(error => console.error('Error:', error));
```

---

### 3. Geolocation API

**정의**: 
Geolocation API는 사용자의 지리적 위치 정보를 스크립트에 제공합니다. 사용자의 동의를 받아 위치 정보를 알아내고, 해당 정보를 사용하여 다양한 서비스나 기능을 제공할 수 있습니다.

**주요 기능**:
- 사용자의 현재 위치 확인
- 위치 변경 감지

**예제**:
```javascript
if ("geolocation" in navigator) {
  navigator.geolocation.getCurrentPosition(position => {
    console.log(`Latitude: ${position.coords.latitude}, Longitude: ${position.coords.longitude}`);
  });
} else {
  console.log("Geolocation is not supported by this browser.");
}
```
