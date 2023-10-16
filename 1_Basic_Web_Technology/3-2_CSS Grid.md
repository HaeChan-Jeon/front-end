
CSS Grid란?

CSS Grid는 2차원 레이아웃 시스템을 제공하는 CSS 모듈입니다. Flexbox와 함께 웹 레이아웃의 복잡성과 유연성을 크게 향상시키는 도구 중 하나입니다. CSS Grid는 행과 열의 시스템을 사용하여 웹 요소를 배치하므로 복잡한 레이아웃도 쉽게 구현할 수 있습니다.

기본 용어
1. Grid Container - Grid 레이아웃을 적용할 부모 요소입니다. 이 요소 내부의 직계 자식 요소들은 Grid Items가 됩니다.
2. Grid Item - Grid Container 내부의 각 요소입니다.
3. Grid Line - Grid의 행이나 열을 구분하는 선입니다.
4. Grid Track - Grid Line 사이의 공간. 행 또는 열로 구성될 수 있습니다.
5. Grid Cell - 하나의 Grid Item이 차지할 수 있는 공간. 행과 열의 교차점에 위치합니다.
6. Grid Gap - 행과 열 사이의 간격입니다.

기본 사용법

Grid Container 설정

```CSS
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr; /* 3개의 열을 동일한 크기로 설정 */
  grid-template-rows: auto; /* 행의 크기는 내용에 따라 자동으로 설정 */
  grid-gap: 20px; /* 간격 설정 */
}
```

2. Grid Item 배치

```CSS
.item1 {
  grid-column: 1 / 3; /* 1번째 열에서 3번째 열 전까지(즉, 1~2 열) */
  grid-row: 1; /* 1번째 행 */
}
```

실용적인 팁

1. fr 단위: fr은 Grid의 사용 가능한 공간에 대한 비율을 나타냅니다. 예를 들어, grid-template-columns: 1fr 2fr;는 첫 번째 열이 사용 가능한 공간의 1/3, 두 번째 열이 2/3을 차지하게 됩니다.

2. repeat() 함수: 반복되는 패턴을 쉽게 만들 수 있습니다. 예를 들어, grid-template-columns: repeat(3, 1fr);는 세 개의 동일한 크기의 열을 생성합니다.

3. auto-fill & auto-fit: 레이아웃의 유연성을 높이기 위해 사용됩니다. 예를 들어, grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));는 최소 200px의 크기를 갖는 열을 최대한 많이 만듭니다.

CSS Grid는 복잡한 레이아웃을 빠르게 구성하는 데 도움을 줍니다. 시작하기 위해선 기본적인 개념을 익히는 것이 중요하며, 그 후에는 다양한 프로젝트에서 직접 활용해보는 것이 가장 좋습니다.
