Flexbox는 웹 페이지의 레이아웃을 쉽고 효율적으로 디자인하기 위한 CSS 모듈입니다. "Flexible Box" 혹은 "Flexbox"라 불리는 이 기술은 아이템 간의 공간 배분과 정렬 능력을 제공하여, 복잡한 레이아웃과 정렬을 돕습니다. 이는 특히 동적인 뷰나 크기 조절이 필요한 UI, 그리고 다양한 디스플레이 디바이스와 스크린 사이즈에 적합합니다.

기본 용어
Container: Flexbox의 부모 요소로, flex 아이템들의 레이아웃을 정의합니다.
Item: Flexbox의 자식 요소로, 컨테이너 내에서 배치됩니다.
주요 속성
Container 속성

display: flexbox 모델을 활성화합니다. (display: flex 또는 display: inline-flex)
flex-direction: 아이템들의 주 축을 설정합니다. (row, row-reverse, column, column-reverse)
justify-content: 주 축을 따라 아이템들을 어떻게 정렬할지 결정합니다.
align-items: 교차 축을 따라 아이템들을 어떻게 정렬할지 결정합니다.
flex-wrap: 아이템들이 여러 행/열로 나뉘어질지 결정합니다. (nowrap, wrap, wrap-reverse)
align-content: 여러 행/열 간의 정렬 방식을 결정합니다.
Item 속성

order: 아이템의 정렬 순서를 설정합니다.
flex-grow: 아이템이 여유 공간을 얼마나 차지할지 결정합니다.
flex-shrink: 아이템이 공간이 부족할 때 얼마나 줄어들지 결정합니다.
flex-basis: 아이템의 기본 크기를 설정합니다.
flex: flex-grow, flex-shrink, flex-basis를 한번에 설정합니다. (e.g., flex: 1 0 auto)
align-self: 아이템 스스로의 교차 축 정렬을 설정합니다.


예시 코드

```css
/* Container */
.flex-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

/* Items */
.flex-item {
  flex-grow: 1;
  flex-shrink: 0;
  flex-basis: auto;
}
```


```html
<div class="flex-container">
  <div class="flex-item">Item 1</div>
  <div class="flex-item">Item 2</div>
  <div class="flex-item">Item 3</div>
</div>
```

이 기본적인 개념과 속성을 바탕으로 Flexbox를 활용하면, 반응형 디자인과 동적인 웹 페이지 레이아웃을 효과적으로 구현할 수 있습니다. Flexbox는 복잡한 레이아웃을 단순화하고, 코드의 양을 줄여 개발자에게 효율적인 작업 환경을 제공합니다.
