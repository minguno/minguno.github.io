# 0208 Web Practice

<br></br>

## Bootstrap Grid System & Responsive Web νμ©

<br></br>

## π μκ΅¬ μ¬ν­

---

μ κ³΅λ μ΄λ―Έμ§ `01_result.png`, `02_result.png`, `03_result.png`λ₯Ό μ°Έκ³ νμ¬ `shop.html`κ³Ό `shop.css`λ₯Ό μμ±νμμ€.

1. μ£Όμ΄μ§ μ£Όμμ λ§κ² κ° μμ (nav, section, article, footer) μμ μ½λλ₯Ό μμ±νμμ€
2. λͺ¨λ  μ΄λ―Έμ§ μμλ images ν΄λμ λ΄κΈ΄ μ΄λ―Έμ§ νμΌμ νμ©ν©λλ€
3. λ€μ΄κ²μ΄μ λ°λ ν­μ λΈλΌμ°μ  νλ©΄ μ΅μλ¨μ κ³ μ λμ΄ μμ΅λλ€
4. μν μ λ³΄κ° λ΄κΈ΄ μΉ΄λλ€μ λ€μμ μ‘°κ±΄μ λ°λ¦λλ€

   - μΉ΄λλ€μ΄ μ΄λνμ§ μμ§λ§, hyper linkμ ννλ₯Ό λλλ€
   - Viewport λλΉκ° 768px λ―Έλ§μΈ κ²½μ°, νλΉ 1κ°μ μΉ΄λκ° μ μλ©λλ€
   - λλΉκ° 768px μ΄μ, 992px λ―Έλ§μΈ κ²½μ°, νλΉ 2κ°μ μΉ΄λκ° μ μλ©λλ€
   - λλΉκ° 992px μ΄μμΈ κ²½μ°, ν λΉ 4κ°μ μΉ΄λκ° μ μλ©λλ€
5. Footerμ μμ΄μ½μ ν΄λ¦­νλ©΄ ν΄λΉνλ SNSμ λ©μΈ νμ΄μ§λ‘ μ΄λν©λλ€

<br></br>

## π λ°μν μΉ (Responsive web)μ΄λ?

---

PC, Mobile, νΉμ Tabletκ³Ό κ°μ λ€μν λλ°μ΄μ€μ κ°κΈ° λ€λ₯Έ νλ©΄ ν¬κΈ°μμ μννκ² λ λλ§λλ μΉ νμ΄μ§λ₯Ό λ»ν©λλ€. λ°μνμΌλ‘ μ€κ³νλ©΄, μ΄λ€ λλ°μ΄μ€μμ μ΄λ€ λ°©μμΌλ‘ μ μνλ μ§ μΉ μ¬μ΄νΈμ μΌκ΄μ±μ μ μ§ν  μ μκ³  μ¬μ©μ±κ³Ό κΈ°λ₯μ±μ λμλλ€.

λ λμκ° 'μ’μ' λ°μν μΉμ΄λ λ°μ€ν¬νκ³Ό λͺ¨λ°μΌμ΄ λ¨μν νλ©΄ ν¬κΈ°λ§ λ€λ₯Έ κ²μ΄ μλλΌ λμ μ΄μ©νλ μλΉμμ νλλ λ€λ₯΄λ€λ μ μ μΈμνκ³  μ΄λ₯Ό λ°μνλ κ²μλλ€.

HTML5, CSS3μ μν΄ μ§μλλ λ―Έλμ΄ μΏΌλ¦¬λ λ°μν μΉμ ν΅μ¬ κΈ°μ μ΄λ€. μ΄λ³΄λ€ λ κ°λ¨νκ³  νΈλ¦¬νκ² λ°μν μΉ μ¬μ΄νΈλ₯Ό κ°λ°ν  μ μκ² HTML, CSS, JavaScriptκ° κ΅¬μν νλ μμν¬κ° BootStrapμ΄λ€.

<br></br>

## π μκ΅¬ μ¬ν­ μΈμ λ΄κ° μΆκ°ν κΈ°λ₯

---

### 1. νλ/λλ³΄κΈ° μ»€μ Zoom-in cursor

* μ΄λ―Έμ§μ λ§μ°μ€λ₯Ό κ°λ€λλ©΄ μ»€μκ° λλ³΄κΈ°λ‘ λ³νλλ€

* Bootstrap icon install λ§ν¬λ₯Ό html λ¬Έμ head μμ λ£μ΄μ€λ€

  ```html
  <!-- Bootstrap Icon Install -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css">
  ```

* μνλ νκ·Έμ μ»€μ μ€νμΌμ μ§μ ν΄μ€λ€

  * λ κ°μ κ²½μ° Modal λ²νΌμ μΆκ°ν΄μ€¬λ€

  ```html
  <button type="button" ... style="cursor: zoom-in">
  ```

<br></br>

### 2. μ΄λ―Έμ§ νλ Modal Component

- νμ μ°½μ΄λΌκ³ λ μκ³  μλ Modal κΈ°λ₯μ μ¬μ©νμ¬ μν μ΄λ―Έμ§λ₯Ό ν΄λ¦­νλ©΄ νλλ μ΄λ―Έμ§κ° λ¨λλ‘ μ€μ νλ€

- λ²νΌμ idκ°κ³Ό modalμ id κ°μ΄ λμΌν΄μΌλ§ μλνλ€

- λν λ²νΌμ ν΄λ¦­ν΄μ modal λ¨κ³  κ»μ λ, ν΄λ¦­ν λ²νΌ νλλ¦¬λ‘ λΉλλ ν¨κ³Όλ₯Ό λ°λ‘ μμ μ€¬λ€

  ```css
  /* λͺ¨λ¬μ°½μ΄ λ¬ ν κ»μ λ ν΄λ¦­ν λ²νΌ νλλ¦¬κ° λΉλλ μ€μ μ κΊΌμ£ΌκΈ° */
  .btn-body:focus {
    box-shadow: none !important;
  }
  ```
  
  - μ΄μ°¨νΌ μ κ·Όμ±μ μν κΈ°λ₯μ΄λΌ κΊΌμ€λ λ¬Έμ λ μλ€

<br></br>

### 3. Hyperlink νμ΄νΌλ§ν¬

- `navbar`μ μμΉν μΌμ± λΈλλ λ‘κ³ λ₯Ό ν΄λ¦­νλ©΄ μΌμ±μ μ λ©μΈ νμ΄μ§λ‘ μ΄λνλ€
- λ²μ¦ μν μ΄λ¦ `Buds`λ₯Ό ν΄λ¦­νλ©΄ κ³΅μ νλ§€ νμ΄μ§λ‘ μ΄λνλ€
- `Login` κ³Ό `Contact` λ²νΌμ κ°κ° μΌμ± κ³΅μ νμ΄μ§μ λ‘κ·ΈμΈκ³Ό λ¬ΈμνκΈ° νμ΄μ§λ‘ μ΄λνλ€

<br></br>

### 4. Carousel Component

- `<section>`μ λ©μΈ μ΄λ―Έμ§λ₯Ό 2κ°λ₯Ό μΆκ°νλ€
- Carouselμ μ΄λ―Έμ§ ν¬κΈ°λ₯Ό λ°λ‘ μ‘°μ νλ κΈ°λ₯μ΄ μμ΄, κΈ°μ‘΄μ λ©μΈ μ΄λ―Έμ§ κ°λ‘μΈλ‘ λΉμ¨μ μΆκ°ν μ΄λ―Έμ§μ λ§μΆ°μΌ νλ€
- μ λ€λ‘ λκΈ°λ `Prev` μ `Next` λ²νΌμ΄ μ μμ νμ΄νλ‘ μκ³ , κΈμλ μ κ·Όμ±μ μν΄ μ μ΄λκ³  μκ°μ μΌλ‘λ `hidden` μμΌ°λ€

<br></br>

### 5. .svg μ΄λ―Έμ§ νμΌ

- μΌμ± λ‘κ³ λ κ·Έλ κ³  λ©μΈ μ΄λ―Έμ§μ 2, 3 λ²μ§Έ μ¬λΌμ΄λλ κ·Έλ κ³  λ€ μΌμ± κ³΅μννμ΄μ§μμ svg λ§ν¬λ₯Ό λ³΅μ¬ν΄μ `<img>` νκ·Έ `src="μ¬κΈ°"`μ μΆκ°ν΄μ€¬λ€

<br></br>

## π μ€μνκ² μκ°ν κΈ°λ₯

---

- `img-fluid` κΈ°λ₯

  ```html
  <img src="images/main.png" alt="Main Image" class="img-fluid">
  ```

  - λ°μν μΉ κΈ°λ°μ νλ μμν¬ λ΅κ² μ λ§ νΈν κΈ°λ₯μ΄λ€

  - λΆλͺ¨ μμ containerμ widthλ₯Ό 100%λ‘ μ°λ©΄μ heightλ autoλ‘ λ§μΆ°μ§λ€

  - μ΄κ² μλμλ€λ©΄, cssμ λ°λ‘ κ½€λ λ²κ±°λ‘­κ² μ§μ ν΄μ€μΌ νλ€

    ```css
    section {
      height: 700px;
      background-image: url('images/header.jpg');
      background-size: cover;
      background-position: center;
    }
    ```

- `sticky-top` κ³Ό `sticky-bottom`

  - μ μλ μ€ν¬λ‘€μ λ΄λ €λ μλ¨ λ°κ° νλ©΄μ κ³μ μμΉν΄ μλ€
  - νμλ μΈλ € μ¬μ΄νΈ λ§¨ λ§μ§λ§μ κ³ μ λμ΄ μκ³  `fixed-bottom`μΌλ‘ νμ λ μ€ν¬λ‘€μ λ΄λ €λ νλ©΄ νλ¨μ κ³μ λ  μλ€

- Modal μ°κ²°

  - buttonμ #λ₯Ό μ μΈν `data-bs-target`κ°κ³Ό modalμ `id` κ°μ΄ κ°μμΌ ν΄λ¦­κ³Ό νμμ°½μ΄ μ°κ²°λλ€
  
- Carouselμ μ΄λ―Έμ§ ν¬κΈ° λ§μΆ€

  - κ°λ‘μΈλ‘ λΉμ¨μ λ§μΆμ§ μμΌλ©΄ μ¬λΌμ΄λκ° λμ΄κ° λ λ§λ€ μλ λ°μ€λ€μ΄ μ¬λΌκ°λ€ λ΄λ €κ°λ€ νκ² λλ€
  - `style`μμ `height`λ₯Ό λ°λ‘ μ§μ νλ λ°©λ²λ μμ© μμΌλ μλ³Έ νμΌμ μμ νμ
  - Carouselμ ν μ¬λΌμ΄λμ κΈκ·λ₯Ό μΆκ°νκ³  μΆμΌλ©΄ μ΄λ€μμΌλ‘ positioningμ ν΄μΌνλμ§ μμ§ μ λͺ¨λ₯΄κ² λ€

<br></br>


## π λλμ 

---

μμ§ν BoostStrap μ²μμ μΈ λλ μ°Ύμλ΄μΌ ν  κ²λ λ§κ³  (λͺ¨λ κ±Έ λ€.. ) CSSλ₯Ό λ°°μ΄μ§ νλ£¨λ§μ λ°μν μΉμ κ΅¬μ¬ν΄μΌ λλ€λ λ§λ§νλλ° μ΅μν΄μ§κ³  λλ μ νΈνλ€κ³  νλμ§ λ°±λ² μ΄ν΄κ°λ€.

μμ§λμ΄κ° λλ€λ©΄ λ°±μλλ νλ‘ νΈμλλλ ν¬κ² μ μλ―Έν κ΅¬λΆμ λμ§ μμμλλ° μ΄λ²μ μμλ€. νλ‘ νΈμλκ° μμ  λ΄ μ μ±μ΄λΌλ κ²μ. κΉλνκ² λ΄μ λ μΈμ μΆ©λ§νκ³  λΏλ―νλ° μλ¬λκ±°λ λ°μ€ λ€μν€λ©΄ κ·Έλ κ² μλ΄ν  μκ° μλ€.

