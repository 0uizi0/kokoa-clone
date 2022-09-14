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

![image](https://user-images.githubusercontent.com/102431281/188895094-4bbde8cc-94c9-4b9c-91f2-d275a1004a92.png)

```html
<ol>
  <li>beer</li>
  <li>김치</li>
  <li>meat</li>
  <li>milk</li>
</ol>
```

![image](https://user-images.githubusercontent.com/102431281/188895272-b2c3a1a4-9d70-45e2-8e47-3898ac0b4c5a.png)

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
  - 자체 닫기 태그(self-closing tag)`<img />` : 
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

- meta 태그
    - `<meta charset=”utf-8”>` : 브라우저에서 텍스트가 깨지지 않도록 설정
    
    - lang 태그
        - 우리 사이트에서 사용하는 주된 언어가 무엇인지 말해줌
        - 검색 엔진에게 도움을 줌
    
    - og 태그
        - 콘텐츠의 요약 내용이 SNS에 게시되는데 최적화된 데이터로 가지고 갈 수 있도록 설정
        - `og:title`, `og:type`, `og:url`, `og: image`, `og:description` …
            
            <img width="810" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%201 36 33" src="https://user-images.githubusercontent.com/102431281/189966065-fb4e3da8-9010-4664-bf39-ae2a3c8b53cd.png">
            
            <img width="273" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%201 37 07" src="https://user-images.githubusercontent.com/102431281/189966223-d90bbf74-20ec-46cb-9428-b0f9696681d4.png">

## More-Tags

<aside>
💡 google에 프론트 검색 시 `mdn` 키워드를 붙여서 검색하기 추천
⇒ **Mozilla developer Network** 사이트로 안내

</aside>

- `<pre>` : pre-formatted text, 타자기 글자처럼 입력됨
    
    <img width="159" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%201 50 44" src="https://user-images.githubusercontent.com/102431281/189967316-809a1084-1a69-4984-a043-407cd35b8e76.png">
    
- `<abbr>` :
    - p 태그 안에 abbreviation에 title인 attribute를 작성
    - 마우스를 KEJ에 올려주면 title에 작성한대로 text가 나옴
    
    ```html
    <p>My name is <abbr title="Kim Eun Jeong">KEJ</abbr></p>
    ```
    
    <img width="203" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%201 56 19" src="https://user-images.githubusercontent.com/102431281/189967337-dca9e065-7cf2-474f-99fa-924de95ee735.png">
    
- `<cite>` : 기울임체
    
    <img width="68" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%201 58 57" src="https://user-images.githubusercontent.com/102431281/189967411-a4487d28-2662-4e4f-bd46-fc37f75db763.png">
    
- `<mark>` : 형광펜
    
    ```html
    <p>l like to live in <mark>South Korea</mark></p>
    ```
    
    <img width="251" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%202 00 58" src="https://user-images.githubusercontent.com/102431281/189967449-72e39ebf-6a81-419c-962b-1ddba04b9696.png">
    
- `<sup>` : 글자 위치가 위로 (`<sub>`: 글자 위치가 아래로)
    
    ```html
    <p>l like to live in <sup>South Korea</sup></p>
    ```
    
    <img width="251" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%202 03 47" src="https://user-images.githubusercontent.com/102431281/189967506-c74bd384-2bcf-44a9-afd5-7e22f8130223.png">
    
- `<audio>` : controls와 src를 작성하면 해당 오디오가 연결됨
    
    ```html
    <audio *controls*="enabled" *src*="https://interactive-examples.mdn.mozilla.net/media/cc0-audio/t-rex-roar.mp3"></audio>
    ```
    
    <img width="309" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%EC%A0%84%202 09 27" src="https://user-images.githubusercontent.com/102431281/189967568-e9fb0189-dca3-4d6e-9a83-0b2593277b0e.png">
    
    - `<autoplay>` : 새로고침 시 자동으로 오디오 재생 설정 
    (이 경우 controls=”enabled” 설정을 하지 않아도 작동됨)
        
        <aside>
        💡 여기서 “enabled”와 ”true”는 같은 의미로 작동됨
        
        </aside>
        
    - `<muted>` : 음소거

## Form-Tags

- input 태그
    
    [ 입력 요소 - HTML: Hypertext Markup Language | MDN](https://developer.mozilla.org/ko/docs/Web/HTML/Element/Input)
    
    - `<input type="color"/>`
        
        <img width="256" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 21 53" src="https://user-images.githubusercontent.com/102431281/190082324-49d5f4a4-7168-4265-a7fd-1f45c74c8c27.png">
        
    - `<input type="password"/>`
        
        <img width="192" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 24 40" src="https://user-images.githubusercontent.com/102431281/190082333-852a8cd7-a511-4cae-8971-f8692d0226cf.png">
        

**⇒ 회원가입 창 생성해보기**

```html
<form>
	<input placeholder="Name"type="text"/>
	<input placeholder="Last Name" type="text"/>
	<input placeholder="Username" type="text"/>
	<input placeholder="Password" type="password"/>
	<input type="submit" value="Create Account"/>
</form>
```

<img width="826" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 28 31" src="https://user-images.githubusercontent.com/102431281/190082346-83e51717-a9f1-4865-9293-ca3066272a3c.png">

- `disabled` : input을 클릭할 수 없음
    
    ```html
    <input placeholder="Username" disabled type="text"/>
    ```
    
    <img width="634" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 31 42" src="https://user-images.githubusercontent.com/102431281/190082362-d31d1756-9a41-45aa-b31b-5da8df5f5aa8.png">
    
- `required` : form 검증하기
    
    ```html
    <form>
    	<input required placeholder="Name"type="text"/>
    	 <input required placeholder="Last Name" type="text"/>
    	<input required placeholder="Username" type="text"/>
    	<input required placeholder="Password" type="password"/>
    	<input type="submit" value="Create Account"/>
    </form>
    ```
    
    - 입력란을 **비운** 상태로 submit 할 경우
        
        <img width="634" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 35 54" src="https://user-images.githubusercontent.com/102431281/190082387-a7c42964-f8c2-4747-87a1-7ee2fc7172dd.png">
        
    - 입력란을 **다 채운** 상태로 submit 할 경우
        
        <img width="620" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 38 13" src="https://user-images.githubusercontent.com/102431281/190082417-f60f07b0-bf8e-4a0b-93e8-fd65d37e10cf.png">
        
- `minlength` : input에 넣는 최소글자 수
    
    ```html
    <input required placeholder="Password" minlength="10" type="password"/>
    ```
    
    <img width="715" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 40 23" src="https://user-images.githubusercontent.com/102431281/190082426-63719984-1f38-47ae-a021-6bd956ebf02b.png">
    
- `<input type="file"/>`
    
    <img width="1317" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 43 54" src="https://user-images.githubusercontent.com/102431281/190082441-d72cfdc2-e668-486b-993b-cb647af12605.png">
    
    - accept : 특정 file의 유형들만 선택하게 끔하는 기능 제공
        
        ```html
        <!--이미지 파일이면 전부 선택 가능 (png, jpg, jpeg ... )-->
        <input type="file" accept="image/*"/>
        ```
        
        <img width="527" alt="%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202022-09-14%20%EC%98%A4%ED%9B%84%203 48 22" src="https://user-images.githubusercontent.com/102431281/190082464-8876007a-7a0c-431e-adb5-011eca9819ac.png">


## More-Tags-and-IDs

## Semantic-HTML

## Recap
