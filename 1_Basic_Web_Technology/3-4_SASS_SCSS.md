## SASS/SCSS 소개

SASS (Syntactically Awesome Stylesheets)는 CSS의 확장으로, 웹 개발에서 스타일시트를 좀 더 효율적이고 유지 관리하기 쉽게 작성하도록 도와줍니다. SASS는 두 가지 문법 형식을 가지고 있습니다: 원래의 SASS 문법과 SCSS (Sassy CSS) 문법입니다. SCSS는 CSS와 매우 유사한 문법을 가지며, 주로 이 형식이 널리 사용됩니다.

## 주요 특징

1. **변수**: 색상, 길이 등을 변수로 저장하고 재사용할 수 있습니다.
    ```scss
    $primary-color: #3498db;
    .button {
        background-color: $primary-color;
    }
    ```

2. **중첩**: 선택자의 중첩을 통해 더 간결하게 코드를 작성할 수 있습니다.
    ```scss
    .nav {
        ul {
            margin: 0;
            li {
                display: inline-block;
            }
        }
    }
    ```

3. **믹스인 (Mixins)**: 재사용 가능한 스타일 블록을 정의하고 여러 곳에서 포함시킬 수 있습니다.
    ```scss
    @mixin border-radius($radius) {
        -webkit-border-radius: $radius;
        border-radius: $radius;
    }
    .button {
        @include border-radius(5px);
    }
    ```

4. **확장/상속**: 기존 클래스의 스타일을 다른 클래스에 상속시킬 수 있습니다.
    ```scss
    .message {
        border: 1px solid #ccc;
        padding: 10px;
    }
    .success {
        @extend .message;
        border-color: green;
    }
    ```

5. **조건문과 반복문**: 스타일시트 내에서 조건문과 반복문을 사용하여 복잡한 로직을 구현할 수 있습니다.

6. **함수**: 컬러 조절, 수학적 연산 등의 기능을 제공하는 내장 함수를 사용하거나 사용자 정의 함수를 만들 수 있습니다.

7. **분할과 가져오기**: 스타일시트를 여러 파일로 분할하고, 필요한 곳에서 가져와서 사용할 수 있습니다.

## 결론

SASS와 SCSS는 웹 개발자에게 효율적이고 구조화된 방식으로 CSS를 작성할 수 있는 도구를 제공합니다. 이를 통해 유지 보수가 쉽고, 가독성 높은 스타일시트를 만들 수 있습니다.
