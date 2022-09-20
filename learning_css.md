## 목차

- [How to Add CSS to HTML](#How-to-Add-CSS-to-HTML)

- [Writing Our First CSS Lines](#Writing-Our-First-CSS-Lines)

- [What Does Cascading Mean](#What-Does-Cascading-Mean)

- [Blocks and Inlines](#Blocks-and-Inlines)

- [Margin Part](#Margin-Part)

- [Paddings and IDs](#Paddings-and-IDs)

- [Border](#Border)

- [Classes](#Classes)

- [Inline Block](#Inline-Block)

- [Flexbox Part One](#Flexbox-Part-One)

- [Flexbox Part Two](#Flexbox-Part-Two)

- [Fixed](#Fixed)

- [Relative Absolute](#Relative-Absolute)

- [Pseudo Selectors part One](#Pseudo-Selectors-part-One)

- [Combinators](#Combinators)

- [Pseudo Selectors part Two](#Pseudo-Selectors-part-Two)

- [States](#States)

- [Recap](#Recap)

- [Colors and Variables](#Colors-and-Variables)

## How-to-Add-CSS-to-HTML

**방법 1. 같은 HTML 파일에 HTML 코드와 CSS 코드를 삽입**

- head 태그 내에서 `style` 태그 사용
    
    ```html
    <style>
    	css 코드
    </style>
    ```
    

**방법 2. CSS와 HTML 분리**

- head 태그 내에서 `link` 태그 사용
    
    ```html
    <link href="styles.css" rel="stylesheet"/>
    ```

## Writing-Our-First-CSS-Lines

- **CSS 규칙**
    - `selector` : HTML 태그를 가리키는 대상 (ex. blueTitle …)
    - `property`  (ex. color, font-size … )
    - `value` : (ex. yellowgreen, 20px …)
    
    ```html
    blueTitle { 
    	color : yellowgreen;
    	font-size : 20px;
    }
    ```

## What-Does-Cascading-Mean

브라우저가 CSS 코드를 읽을 때 위에 있는 코드부터 차례차례로 읽힌다는 것

→ inline CSS와 external CSS가 같은 대상을 가리키게 될 경우, 
html 코드에서 **가장 마지막에 있는 코드가 적용됨**

```html
	<link href="styles.css" rel="stylesheet"/>
        <style>
            h1 {
                color: blue;
                font-size: 20px;
            }
            address{
                text-align: center;
                color: tomato;
            }
        </style>
```

```css
h1 {
	color: tomato;
}
```

⇒ h1의 색깔은 `blue`

⇒ 코드의 순서가 결과에 영향을 미침

## Blocks-and-Inlines

- Block
    - 하나의 요소 옆에 **아무것도 오지 않음**
    - ex) `div`, `header`, `main`, `section`, `footer`, `article`, `p` …
- Inline
    - 하나의 요소 옆에 **다른 요소들이 올 수 있음**
    - ex) `span`, `link`, `img` …

## Margin-Part

- Block의 특징
    - inline과 달리 높이와 너비를 가짐
        - div는 `display:inline;`을 할 수 없음
            
            ⇒ 어떤 요소가 inline이면 그 요소는 높이와 너비를 가질 수 없기 때문
            
    - margin
    - padding
    - border

- `margin` : box의 경계의 **바깥**에 있는 공간
    - body는 기본적으로 margin 값이 8px임
    - 지정한 margin 값의 개수
        - 1개 → 상하좌우
        - 2개 → 상하 좌우
        - 4개 → 상 후 하 좌 (시계방향)
    
    - `collapsing margins` : div가  넘어서 **부모 div의 경계가 위로 밀려난 현상** (위아래에서만 나타남)
        - 예시 :
        
        <img width="377" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-20%20%EC%98%A4%ED%9B%84%209 06 53" src="https://user-images.githubusercontent.com/102431281/191256552-db95de44-c008-4b03-8689-b48fe3071cff.png">
        
        <img width="377" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-20%20%EC%98%A4%ED%9B%84%209 11 39" src="https://user-images.githubusercontent.com/102431281/191256566-dc49d25c-f708-48ab-b0f9-b55a0da6bd85.png">
        
        - 문제 :
            - 위아래 margin 값이 없음
            - 자식 div의 margin 값을 변화시키면 부모 div의 margin 값도 변함
            - ⇒ div가 body의 마진 값을 넘어섰음
        - 원인 : **자식 box의 경계가 부모 box의 경계가 같아** **두 margin이 하나로 취급**되었기 때문
- `padding`
    
    ⇒ 자식 box가 부모 box의 경계와 맞닿지 않고 위치하기 위해 사용
    
- `border`

## Paddings-and-IDs

## Border

## Classes

## Inline-Block

## Flexbox-Part-One

## Flexbox-Part-Two

## Fixed

## Relative-Absolute

## Pseudo-Selectors-part-One

## Combinators

## Pseudo-Selectors-part-Two

## States

## Recap

## Colors-and-Variables
