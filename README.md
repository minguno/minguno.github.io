# 0208 Web Practice

<br></br>

## Bootstrap Grid System & Responsive Web 활용

<br></br>

## 🎈 요구 사항

---

제공된 이미지 `01_result.png`, `02_result.png`, `03_result.png`를 참고하여 `shop.html`과 `shop.css`를 작성하시오.

1. 주어진 주석에 맞게 각 요소 (nav, section, article, footer) 안에 코드를 작성하시오
2. 모든 이미지 요소는 images 폴더에 담긴 이미지 파일을 활용합니다
3. 네이게이션 바는 항상 브라우저 화면 최상단에 고정되어 있습니다
4. 상품 정보가 담긴 카드들은 다음의 조건을 따릅니다

   - 카드들이 이동하지 않지만, hyper link의 형태를 띕니다
   - Viewport 너비가 768px 미만인 경우, 행당 1개의 카드가 제시됩니다
   - 너비가 768px 이상, 992px 미만인 경우, 행당 2개의 카드가 제시됩니다
   - 너비가 992px 이상인 경우, 행 당 4개의 카드가 제시됩니다
5. Footer의 아이콘을 클릭하면 해당하는 SNS의 메인 페이지로 이동합니다

<br></br>

## 🎈 반응형 웹 (Responsive web)이란?

---

PC, Mobile, 혹은 Tablet과 같은 다양한 디바이스의 각기 다른 화면 크기에서 원활하게 렌더링되는 웹 페이지를 뜻합니다. 반응형으로 설계하면, 어떤 디바이스에서 어떤 방식으로 접속하든지 웹 사이트의 일관성을 유지할 수 있고 사용성과 기능성을 높입니다.

더 나아가 '좋은' 반응형 웹이란 데스크탑과 모바일이 단순히 화면 크기만 다른 것이 아니라 둘을 이용하는 소비자의 태도도 다르다는 점을 인식하고 이를 반영하는 것입니다.

HTML5, CSS3에 의해 지원되는 미디어 쿼리는 반응형 웹의 핵심 기술이다. 이보다 더 간단하고 편리하게 반응형 웹 사이트를 개발할 수 있게 HTML, CSS, JavaScript가 구상한 프레임워크가 BootStrap이다.

<br></br>

## 🎈 요구 사항 외에 내가 추가한 기능

---

### 1. 확대/돋보기 커서 Zoom-in cursor

* 이미지에 마우스를 갖다대면 커서가 돋보기로 변환된다

* Bootstrap icon install 링크를 html 문서 head 안에 넣어준다

  ```html
  <!-- Bootstrap Icon Install -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css">
  ```

* 원하는 태그에 커서 스타일을 지정해준다

  * 나 같은 경우 Modal 버튼에 추가해줬다

  ```html
  <button type="button" ... style="cursor: zoom-in">
  ```

<br></br>

### 2. 이미지 확대 Modal Component

- 팝업 창이라고도 알고 있는 Modal 기능을 사용하여 상품 이미지를 클릭하면 확대된 이미지가 뜨도록 설정했다

- 버튼의 id값과 modal의 id 값이 동일해야만 작동한다

- 또한 버튼을 클릭해서 modal 뜨고 껐을 때, 클릭한 버튼 테두리로 빛나는 효과를 따로 없애줬다

  ```css
  /* 모달창이 뜬 후 껐을 때 클릭한 버튼 테두리가 빛나는 설정을 꺼주기 */
  .btn-body:focus {
    box-shadow: none !important;
  }
  ```
  
  - 어차피 접근성을 위한 기능이라 꺼줘도 문제는 없다

<br></br>

### 3. Hyperlink 하이퍼링크

- `navbar`에 위치한 삼성 브랜드 로고를 클릭하면 삼성전자 메인 페이지로 이동한다
- 버즈 상품 이름 `Buds`를 클릭하면 공식 판매 페이지로 이동한다
- `Login` 과 `Contact` 버튼은 각각 삼성 공식 페이지의 로그인과 문의하기 페이지로 이동한다

<br></br>

### 4. Carousel Component

- `<section>`에 메인 이미지를 2개를 추가했다
- Carousel은 이미지 크기를 따로 조절하는 기능이 없어, 기존에 메인 이미지 가로세로 비율을 추가한 이미지와 맞춰야 했다
- 앞 뒤로 넘기는 `Prev` 와 `Next` 버튼이 양 옆에 화살표로 있고, 글자는 접근성을 위해 적어두고 시각적으로는 `hidden` 시켰다

<br></br>

### 5. .svg 이미지 파일

- 삼성 로고도 그렇고 메인 이미지의 2, 3 번째 슬라이드도 그렇고 다 삼성 공식홈페이지에서 svg 링크를 복사해서 `<img>` 태그 `src="여기"`에 추가해줬다

<br></br>

## 🎈 중요하게 생각한 기능

---

- `img-fluid` 기능

  ```html
  <img src="images/main.png" alt="Main Image" class="img-fluid">
  ```

  - 반응형 웹 기반의 프레임워크 답게 정말 편한 기능이다

  - 부모 요소 container의 width를 100%로 쓰면서 height는 auto로 맞춰진다

  - 이게 아니었다면, css에 따로 꽤나 번거롭게 지정해줘야 한다

    ```css
    section {
      height: 700px;
      background-image: url('images/header.jpg');
      background-size: cover;
      background-position: center;
    }
    ```

- `sticky-top` 과 `sticky-bottom`

  - 전자는 스크롤을 내려도 상단 바가 화면에 계속 위치해 있다
  - 후자는 외려 사이트 맨 마지막에 고정되어 있고 `fixed-bottom`으로 했을 때 스크롤을 내려도 화면 하단에 계속 떠 있다

- Modal 연결

  - button의 #를 제외한 `data-bs-target`값과 modal의 `id` 값이 같아야 클릭과 팝업창이 연결된다
  
- Carousel의 이미지 크기 맞춤

  - 가로세로 비율을 맞추지 않으면 슬라이드가 넘어갈 때 마다 아래 박스들이 올라갔다 내려갔다 하게 된다
  - `style`에서 `height`를 따로 지정하는 방법도 소용 없으니 원본 파일을 수정하자
  - Carousel의 한 슬라이드에 글귀를 추가하고 싶으면 어떤식으로 positioning을 해야하는지 아직 잘 모르겠다

<br></br>


## 🎈 느낀점

---

솔직히 BoostStrap 처음에 쓸 때는 찾아봐야 할 것도 많고 (모든걸 다.. ) CSS를 배운지 하루만에 반응형 웹을 구사해야 된다니 막막했는데 익숙해지고 나니 왜 편하다고 하는지 백번 이해간다.

엔지니어가 된다면 백엔드냐 프론트엔드냐는 크게 유의미한 구분을 두지 않았었는데 이번에 알았다. 프론트엔드가 완전 내 적성이라는 것을. 깔끔하게 떴을 땐 세상 충만하고 뿌듯한데 에러나거나 박스 뒤엉키면 그렇게 암담할 수가 없다.

