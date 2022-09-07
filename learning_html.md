## 목차

- [Our First HTML Tag](#Our-First-HTML-Tag)

- [More Tags and Prettier](#More-Tags-and-Prettier)

- [Tag Attributes](#Tag-Attributes)

- [More Tags and Head](#More-Tags-and-Head)

- [Its All About the Head](#Its-All-About-the-Head)

- [More Tags](#More-Tags)

- [Form Tags](#Form-Tags)

- [More Tags and IDs](#More-Tags-and-IDs)

- [Semantic HTML](#Semantic-HTML)

- [Recap](#Recap)

## Our-First-HTML-Tag

## More-Tags-and-Prettier

- `ol` (ordered list) : 순서가 있는 목록
- `ul` (unordered list) : 순서가 없는 목록
- `li` (list item) : 리스트 안의 요소

```html
<ul>
  <li>beer</li>
  <li>김치</li>
  <li>meat</li>
  <li>milk</li>
</ul>
```

![스크린샷 2022-09-07 오후 5.43.22.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6bc8aa10-fa2f-44ba-98e3-85c9d5dd11a0/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2022-09-07_%EC%98%A4%ED%9B%84_5.43.22.png)

```html
<ol>
  <li>beer</li>
  <li>김치</li>
  <li>meat</li>
  <li>milk</li>
</ol>
```

![스크린샷 2022-09-07 오후 5.45.10.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5b4d9400-bc62-41b8-bd5d-f5dbd47b053c/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7_2022-09-07_%EC%98%A4%ED%9B%84_5.45.10.png)

## Tag-Attributes

- a 태그
  - `a` (anchor) : 다른 사이트로 이동
  - `attribute` : 태그에 부가적인 정보 추가
  - `href=””` : 이동할 주소를 설정
    → attribute href는 anchor 태그에만 추가 가능
    (h1 태그에 href를 작성하여도 변화 없음)
  - `target=””`
    - `“_self”` : 해당 페이지 내에서 페이지 이동 (기본값)
    - `“_blank”` : 새로운 탭에서 해당 주소의 페이지 생성
- img 태그
  - 자체 닫기 태그(self-closing tag)`<img />`
    이미지 태그 사이에 content가 없음
  - `src=””` : 이미지의 주소 삽입

## More-Tags-and-Head

- img 태그
  - 이미지 경로를 정확히 작성해야함.
- html 기본 문법
  - `head`
    - 페이지에 관한 환경 설정을 해주는 곳
    - head 태그에 속해 있는 모든 태그들은 보여지지 않음
  - `body`
    - 브라우저 화면 상에 보여질 내용들이 있는 곳
  ```html
  <!DOCTYPE html>
  <html>
    <head> </head>
    <body></body>
  </html>
  ```

## Its-All-About-the-Head

## More-Tags

## Form-Tags

## More-Tags-and-IDs

## Semantic-HTML

## Recap
