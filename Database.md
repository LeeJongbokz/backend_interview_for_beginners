# Database
<br>

### RDB vs NoSQL?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ RDB
    - RDB๋ ํ์ด๋ธ ํ์์ ๊ณ ์ ๋ ์คํค๋ง๋ฅผ ์ ๊ณตํฉ๋๋ค. 
    - RDB๋ ํ์ด๋ธ ๊ฐ Join๋ฌธ์ ์ ๊ณตํฉ๋๋ค.
    - RDB๋ ํธ๋์ญ์ ๊ธฐ๋ฅ์ ์ ๊ณตํฉ๋๋ค.
    - RDB๋ ์๊ฒฉํ Schama๋ก ๋ฐ์ดํฐ ์ค๋ณต์ด ์๊ธฐ ๋๋ฌธ์ update๊ฐ ๋ง์ ๊ฒฝ์ฐ์ ์ ๋ฆฌํฉ๋๋ค. 
    - RDB๋ Scale-up์ ์ ๋ฆฌํฉ๋๋ค. 

+ NoSQL
    - NoSQL์ ๋ค์ํ ํ์์ผ๋ก ์ ์ฅ๋ฉ๋๋ค.(ex) Key-value, Graph-based, Column-based ๋ฑ)
    - NoSQL์ ์ผ๋ฐ์ ์ผ๋ก Join๋ฌธ์ ์ ๊ณตํ์ง ์์ต๋๋ค. 
    - NoSQL์ ์ผ๋ฐ์ ์ผ๋ก ํธ๋์ญ์ ๊ธฐ๋ฅ์ ์ ๊ณตํ์ง ์์ต๋๋ค. 
    - NoSQL์ ๋น ๋ฅธ ์ฝ๊ธฐ ์ฑ๋ฅ์ ๊ฐ์ง๊ณ  ์์ผ๋ฏ๋ก, ์ผ๋ฐ์ ์ผ๋ก ๋ง์ ๋ฐ์ดํฐ๋ฅผ ์ฝ๋ ์๋น์ค์ ์ ๋ฆฌํฉ๋๋ค. 
    - NoSQL์ Scale-out์ ์ ๋ฆฌํฉ๋๋ค. 

</details>

-----------------------

### MySQL ์์ง์ ๋ฌด์์ผ๋ก ๊ตฌ์ฑ๋์ด ์๋์?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ MySQL ์์ง์ ํด๋ผ์ด์ธํธ๋ก๋ถํฐ์ ์ ์ ๋ฐ ์ฟผ๋ฆฌ ์์ฒญ์ ์ฒ๋ฆฌํ๋ ์ปค๋ฅ์ ํธ๋ค๋ฌ, <br> 
  SQL ํ์ ๋ฐ ์ ์ฒ๋ฆฌ๊ธฐ,<br>
  ์ฟผ๋ฆฌ์ ์ต์ ํ๋ ์คํ์ ์ํ ์ตํฐ๋ง์ด์ ๊ฐ ์ค์ฌ์ ์ด๋ฃน๋๋ค. 

</details>

-----------------------

### ์คํ ๋ฆฌ์ง ์์ง์ ๊ธฐ๋ฅ์ ๋ฌด์์ธ๊ฐ์?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ์คํ ๋ฆฌ์ง ์์ง์ ์ค์  ๋ฐ์ดํฐ๋ฅผ ๋์คํฌ ์คํ ๋ฆฌ์ง์ ์ ์ฅํ๊ฑฐ๋, <br>
  ๋์คํฌ ์คํ ๋ฆฌ์ง๋ก๋ถํฐ ๋ฐ์ดํฐ๋ฅผ ์ฝ์ด์ค๋ ๋ถ๋ถ์ ์ ๋ดํฉ๋๋ค. <br>
  MySQL ์๋ฒ์์ MySQL ์์ง์ ํ๋์ง๋ง, ์คํ ๋ฆฌ์ง ์์ง์ ์ฌ๋ฌ ๊ฐ๋ฅผ ๋์์ ์ฌ์ฉํ  ์ ์์ต๋๋ค. <br> 
  ๊ฐ ์คํ ๋ฆฌ์ง ์์ง์ ์ฑ๋ฅ ํฅ์์ ์ํด InnoDB ๋ฒํผ ํ(InnoDB ์คํ ๋ฆฌ์ง ์์ง), ํค ์บ์(MyISAM ์คํ ๋ฆฌ์ง ์์ง) <br>
  ๊ณผ ๊ฐ์ ๊ธฐ๋ฅ์ ๋ด์ฅํ๊ณ  ์์ต๋๋ค.  
   

</details>

-----------------------


### MySQL ์ค๋ ๋ฉ ๊ตฌ์กฐ๋ ์ด๋ป์ต๋๊น?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ MySQL ์๋ฒ๋ ํ๋ก์ธ์ค ๊ธฐ๋ฐ์ด ์๋๋ผ ์ค๋ ๋ ๊ธฐ๋ฐ์ผ๋ก ๋์ํ๋ฉฐ, <br>
  ํฌ๊ฒ ํฌ๊ทธ๋ผ์ด๋(Foreground) ์ค๋ ๋์ ๋ฐฑ๊ทธ๋ผ์ด๋(Background) ์ค๋ ๋๋ก ๊ตฌ๋ถํ  ์ ์์ต๋๋ค. <br>
  ๋ฐฑ๊ทธ๋ผ์ด๋ ์ค๋ ๋์ ๊ฐ์๋ MySQL ์๋ฒ์ ์ค์  ๋ด์ฉ์ ๋ฐ๋ผ ๊ฐ๋ณ์ ์ผ ์ ์์ต๋๋ค. <br> 
  ํฌ๊ทธ๋ผ์ด๋ ์ค๋ ๋๋ ์ต์ํ MySQL ์๋ฒ์ ์ ์๋ ํด๋ผ์ด์ธํธ์ ์๋งํผ ์กด์ฌํ๋ฉฐ, <br>
  ์ฃผ๋ก ๊ฐ ํด๋ผ์ด์ธํธ ์ฌ์ฉ์๊ฐ ์์ฒญํ๋ ์ฟผ๋ฆฌ ๋ฌธ์ฅ์ ์ฒ๋ฆฌํฉ๋๋ค. <br> 
   
</details>

-----------------------

### MySQL ์ค๋ ๋ ์บ์๋ ์ด๋ป๊ฒ ๋์ํฉ๋๊น?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ํด๋ผ์ด์ธํธ์ฌ์ฉ์๊ฐ ์์์ ๋ง์น๊ณ , ์ปค๋ฅ์์ ์ข๋ฃํ๋ฉด ํด๋น ์ปค๋ฅ์์ ๋ด๋นํ๋ ์ค๋ ๋๋<br>
  ๋ค์ ์ค๋ ๋ ์บ์(Thread Cache)๋ก ๋๋์๊ฐ๋๋ค.<br>
  ์ด ๋, ์ด๋ฏธ ์ค๋ ๋ ์บ์์ ์ผ์  ๊ฐ์ ์ด์์ ๋๊ธฐ ์ค์ธ ์ค๋ ๋๊ฐ ์์ผ๋ฉด, <br>
  ์ค๋ ๋ ์บ์์ ๋ฃ์ง ์๊ณ  ์ค๋ ๋๋ฅผ ์ข๋ฃ์์ผ ์ผ์  ๊ฐ์์ ์ค๋ ๋๋ง ์ค๋ ๋ ์บ์์ ์กด์ฌํ๊ฒ ํฉ๋๋ค.<br>
  ์ด ๋, ์ค๋ ๋ ์บ์์ ์ ์งํ  ์ ์๋ ์ต๋ ์ค๋ ๋ ๊ฐ์๋ thread_cache_size ์์คํ ๋ณ์๋ก ์ค์ ํฉ๋๋ค. 
   
</details>

-----------------------

### ํธ๋์ญ์์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ 

</details>

-----------------------

### ์ธ๋ฑ์ค์ ์ฅ๋จ์ ์?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ์ฅ์ 
    - ์ธ๋ฑ์ค๋ ์ผ์ข์ ์์ธ์ผ๋ก์, ๋งค์ฐ ๋น ๋ฅธ ๊ฒ์์ ๊ฐ๋ฅํ๊ฒ ํ๋ค๋ ์ ์ด ์ฅ์ ์๋๋ค. 

+ ๋จ์ 
    - ์ธ๋ฑ์ค๋ ๋ฐ์ดํฐ๋ฅผ ์๋ฐ์ดํธํ๊ฑฐ๋ ์ญ์ ํ  ๋, ๋งค๋ฒ ์ ๋ ฌ์ ํด์ค์ผ ํ๋ฏ๋ก,
      ์๋ฐ์ดํธ ๋ฐ ์ญ์ ์ ์ฑ๋ฅ์ ๋จ์ด์ง ์ ์๋ค๋ ๋จ์ ์ด ์์ต๋๋ค. 

</details>

-----------------------
### Hash Index ์๊ณ ๋ฆฌ์ฆ์ ์ฅ์ ๊ณผ ๋จ์ ์?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

-----------------------
+ ์ฅ์ 
    - Hash Index ์๊ณ ๋ฆฌ์ฆ์ ํด์ ๊ฐ์ ์ธ๋ฑ์ฑํ๋ฏ๋ก, ๋งค์ฐ ๋น ๋ฅธ ๊ฒ์์ ์ง์ํฉ๋๋ค.  
+ ๋จ์ 
    - ๊ฐ์ ๋ณํํ์ฌ ์ ์ฅํ๋ฏ๋ก, ์ ๋ฐฉ(Prefix) ๊ฒ์๊ณผ ๊ฐ์ ๊ฒ์ ์ฌ์ฉ์ด ๋ถ๊ฐ๋ฅํฉ๋๋ค.
</details>

-----------------------

### ํด๋ฌ์คํฐ๋ง ์ธ๋ฑ์ค๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ํ๋ผ์ด๋จธ๋ฆฌ ํค ๊ฐ์ด ๋น์ทํ ๋ ์ฝ๋๋ผ๋ฆฌ ๋ฌถ์ด์ ์ ์ฅํ๋ ๊ฒ์ ํด๋ฌ์คํฐ๋ง ์ธ๋ฑ์ค๋ผ๊ณ  ํํํฉ๋๋ค. <br>
  ์ฆ, ํ๋ผ์ด๋จธ๋ฆฌ ํค ๊ฐ์ ์ํด ๋ ์ฝ๋์ ์ ์ฅ ์์น๊ฐ ๊ฒฐ์ ๋๋ฉฐ, ํ๋ผ์ด๋จธ๋ฆฌ ํค ๊ฐ์ด ๋ณ๊ฒฝ๋๋ค๋ฉด <br>
  ๊ทธ ๋ ์ฝ๋์ ๋ฌผ๋ฆฌ์ ์ธ ์ ์ฅ ์์น๋ ๋ฐ๋์ด์ผ ํฉ๋๋ค. <br>
  ํด๋ฌ์คํฐ๋ง ์ธ๋ฑ์ค๋ ํ์ด๋ธ์ ํ๋ผ์ด๋จธ๋ฆฌ ํค์ ๋ํด์๋ง ์ ์ฉ๋๋ ๋ด์ฉ์ด๋ฉฐ, <br> 
  ์ฃผ๋ก ๋น์ทํ ๊ฐ๋ค์ ๋์์ ์กฐํํ๋ ๊ฒฝ์ฐ๊ฐ ๋ง๋ค๋ ์ ์ ์ฐฉ์ํ ๊ฒ์๋๋ค. <br>
</details>

-----------------------
### ์ ๊ทํ๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ์ ๊ทํ๋ ํ๋์ ๋ฆด๋ ์ด์์ ํ๋์ ์๋ฏธ๋ง ์กด์ฌํ  ์ ์๋๋ก ๋ฆด๋ ์ด์์ ๋ถํดํด ๋๊ฐ๋ ๊ณผ์ ์ ์๋ฏธํฉ๋๋ค. <br> 
  ๋ฐ๋ฉด, ๋น์ ๊ทํ์ ํ๋์ ํํ์์ ์์ฑ์ ์๋ ฅ๋๋ ๋๋ฉ์ธ ๊ฐ์ผ๋ก ์ฌ๋ฌ ๊ฐ์ ๊ฐ์ด ๋ค์ด์์, ์์์ฑ์ ๊ฐ์ง ๋ชปํ๋ ๊ฒฝ์ฐ๋ฅผ ์๋ฏธํฉ๋๋ค. <br>
  ์ 1 ์ ๊ทํ๋ ์์๊ฐ์ด ์๋ ๋๋ฉ์ธ์ ๋ถํดํ์ฌ ์ด๋ค ๋ฆด๋ ์ด์ R์ ์ํ ๋ชจ๋  ๋๋ฉ์ธ์ด ์์๊ฐ์ผ๋ก๋ง ์ค๊ณํ๋ ๊ฒ์ ์๋ฏธํฉ๋๋ค. <br> 
   
  ์ 2 ์ ๊ทํ์ ์ด๋ค ๋ฆด๋ ์ด์ R์ด ์ 1์ ๊ทํ์ ์ํ๊ณ , ๊ธฐ๋ณธํค์ ์ํ์ง ์๋ ๋ชจ๋  ์์ฑ์ด ๊ธฐ๋ณธํค์ ์์  ํจ์์  ์ข์์ด๋ฉด ์ถฉ์กฑํ๋ ์ ๊ทํ <br> 
   
  ์ 3 ์ ๊ทํ์ ์ด๋ค ๋ฆด๋ ์ด์ R์ด ์ 2์ ๊ทํ์ ์ํ๊ณ , ๊ธฐ๋ณธํค์ ์ํ์ง ์๋ ๋ชจ๋  ์์ฑ์ด ๊ธฐ๋ณธํค์ ์ดํ์  ํจ์ ์ข์์ด ์๋ ์ํ์ ๊ด๊ณ <br> 
 
[์ฐธ๊ณ : SQL ์ฒซ๊ฑธ์] 
+ ์ ๊ทํ๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ํ์ด๋ธ์ ๊ท์ ๋ ์ฌ๋ฐ๋ฅธ ํํ๋ก ๊ฐ์ ํด๋๊ฐ๋ ๊ฒ์๋๋ค. <br> 
  ์ ๊ทํ๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ค๊ณ ๋จ๊ณ์์ ํํด์ง๋๋ค. <br> 
  ๊ฒฝ์ฐ์ ๋ฐ๋ผ์๋ ๊ธฐ์กด ์์คํ์ ์ฌ๊ฒํ ํ  ๋ ์ ๊ทํํ๋ ๊ฒฝ์ฐ๋ ์์ต๋๋ค. <br> 
   
  ์ฌ๊ธฐ์ ๋งํ๋ ์ฌ๋ฐ๋ฅธ ํํ๋ ์ฃผ๊ด์  ๊ธฐ์ค์ด๋ผ ํ  ์ ์์ต๋๋ค. <br> 
  ์ ๊ทํ์ ์์๋ ์ด์ ์ ๋ฐ์ดํฐ๋ฒ ์ด์ค ๊ธฐ์ ์๋ค์ด ๊ณ ์ํด ์ ๋ฆฌํ ๊ฒ์๋๋ค. <br> 
  ์ด๋ฅผ ์ฐธ๊ณ ํ์ฌ ์ ๊ทํํ๋ ๊ณผ์ ์ ํตํด ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค๊ฐ ํจ์จ์ ์ผ๋ก ๋์ํ๋๋ก <br> 
  ๋ง๋ค ์ ์์ต๋๋ค. <br> 
  
</details>

-----------------------

### ์ 1 ์ ๊ทํ์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />
   
[์ฐธ๊ณ : SQL ์ฒซ๊ฑธ์] 
+ ๊ด๊ณํ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ํ์ด๋ธ์๋ ํ๋์ ์์ ํ๋์ ๊ฐ๋ง ์ ์ฅํ  ์ ์๋ค๋ ์ ์ฝ์ด ์์ต๋๋ค. <br> 
  ์ด๋ก ์ธํด ์ฃผ๋ฌธ์ํ์ ๋ฐ์ดํฐ๋ฅผ ๊ทธ๋๋ก ํ์ด๋ธ๋ก ๋ง๋ค ์๋ ์์ต๋๋ค. <br>
  ์ ์ด๋ ์ํ ์ฝ๋์ ์ํ๋ช, ๊ฐ์ ๋ฐ์ดํฐ๋ฅผ ๋ด๋ ์ธ ๊ฐ์ ์ด๋ก ๋๋์ด์ผ ํฉ๋๋ค. <br> 

  ์ 1์ ๊ทํ์์๋ ์ค๋ณต์ ์ ๊ฑฐํ๋ ํ์ด๋ธ์ ๋ถํ ๋ ์ด๋ฃจ์ด์ง๋๋ค. <br> 
  ์๋ฅผ ๋ค๋ฉด, ํ ๋ฒ์ ์ฃผ๋ฌธ์ผ๋ก ์ฌ๋ฌ ๊ฐ์ ์ํ์ ์ฃผ๋ฌธํ  ์ ์์ผ๋ฏ๋ก, <br> 
  ์ฃผ๋ฌธ๋ฒํธ, ๋ ์ง, ์ฑ๋ช, ์ฐ๋ฝ์ฒ๊ฐ ๋์ผํ ๊ฐ์ ๊ฐ์ง๋ ํ์ด ์ฌ๋ฌ ๊ฐ ์กด์ฌํ  ์ ์์ต๋๋ค. <br> 
  ์ด ๋, ๋์ผํ ๊ฐ์ ๊ฐ์ง๋ ํ์ด ์ฌ๋ฌ ๊ฐ ์กด์ฌํ์ง ์๋๋ก ํ๋๋ก ์ ๋ฆฌํด์ผ ํฉ๋๋ค. <br> 
   
  ์ฆ, ์ 1์ ๊ทํ์์๋ ๋ฐ๋ณต๋ ๋ถ๋ถ์ ์ฐพ์๋ด์ ํ์ด๋ธ์ ๋ถํ ํ๊ณ , <br>
  ๊ธฐ๋ณธํค๊ฐ ๋  ์ด์ ์์ฑํ  ์ ์์ต๋๋ค. 
   
</details>

-----------------------


### ์ 2 ์ ๊ทํ์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />
   
[์ฐธ๊ณ : SQL ์ฒซ๊ฑธ์] 
+ ์ 1์ ๊ทํ์์ ํ์ด๋ธ์ ๊ธฐ๋ณธํค๋ฅผ ์์ฑํ ๊ฒ๊ณผ ๊ฐ์ ๋ฐฉ๋ฒ์ผ๋ก, <br> 
  ์ 2์ ๊ทํ์์๋ ๋ฐ์ดํฐ๊ฐ ์ค๋ณตํ๋ ๋ถ๋ถ์ ์ฐพ์๋ด์ด, ํ์ด๋ธ๋ก ๋ถํ ํด ๋๊ฐ๋๋ค. <br> 
  ์ด ๋, ๊ธฐ๋ณธํค์ ์ํด ํน์ ๋๋ ์ด๊ณผ ๊ทธ๋ ์ง ์์ ์ด๋ก ๋๋๋ ๊ฒ์ผ๋ก ์ ๊ทํ๊ฐ ์ด๋ฃจ์ด์ง๋๋ค. <br> 
   
  ์ฃผ๋ฌธ์ํ ํ์ด๋ธ์ ์ดํด๋ณด๋ฉด, ์ฃผ๋ฌธ์ํ์ ๊ธฐ๋ณธํค๋ ์ฃผ๋ฌธ๋ฒํธ์ ์ํ์ฝ๋์ ๋ ๊ฐ์ ์ด๋ก ๋์ด ์์ต๋๋ค. <br> 
  ์ฃผ๋ฌธ๋ฒํธ 1์ ์ํ์ฝ๋๊ฐ 0001์ธ ์ํ ์ฃผ๋ฌธ๋์ ์ด 1๊ฐ๋ผ๋ ๊ฒ์ ์ ์ ์์ต๋๋ค. <br> 
  ์ด๊ฒ์ ๊ธฐ๋ณธํค๋ฅผ ๋ฐํ์ผ๋ก ํน์ ๋๋ ๋ฐ์ดํฐ์๋๋ค. <br> 
   
  ์ฆ, ๊ฐ์ ์ด์ ๊ธฐ๋ณธํค๊ฐ ๊ฒฐ์ ๋๊ณ  ๋๋ฉด ํน์ ํ  ์ ์๋ ๊ฒ์๋๋ค. <br> 
  ํํธ, ์ํ๋ช์ ์ฃผ๋ฌธ๋ฒํธ์ ๊ด๊ณ์์ด ์ํ์ฝ๋๋ง์ผ๋ก ํน์ ํ  ์ ์์ต๋๋ค. <br> 
  ์ํ์ฝ๋๋ ๊ธฐ๋ณธํค์ ์ผ๋ถ์ด๊ธด ํ์ง๋ง ๋จ๋์ผ๋ก ๊ธฐ๋ณธํค ์ญํ ์ ํ  ์๋ ์์ต๋๋ค. <br>
   
  ์ด์ฒ๋ผ ๋ ๊ฐ์ง๋ก ๋ถ๋ฅํ  ์ ์์ผ๋ฏ๋ก, ๋ ๊ฐ์ ํ์ด๋ธ๋ก ๋ถํ ํ๊ฒ ์ต๋๋ค. <br> 
  ํ์ด๋ธ๋ช์ '์ํ'์ด๋ผ๊ณ  ํ๊ฒ ์ต๋๋ค. <br> 
  
  ์ํ ํ์ด๋ธ์ ์ํ์ฝ๋๋ง์ผ๋ก ๊ธฐ๋ณธํค๋ฅผ ์ง์ ํ์ต๋๋ค. <br>
  ์ด๋ ค์ด ๋ง๋ก ํํํ์๋ฉด ๋ถ๋ถ ํจ์์ข์์ฑ์ ์ฐพ์๋ด์ ํ์ด๋ธ์ ๋ถํ ํ๋ ๊ฒ์ด ์ 2์ ๊ทํ์๋๋ค. <br>
  ์ฌ๊ธฐ์ ํจ์์ข์์ฑ์ด๋ ํค ๊ฐ์ ์ด์ฉํด ๋ฐ์ดํฐ๋ฅผ ํน์ ์ง์ ์ ์๋ ๊ฒ์ ๊ฐ๋ฆฌํต๋๋ค. <br>  
   
</details>

-----------------------


### ๋ถ๋ถ ํจ์์  ์ข์์ฑ์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />
   
[์ฐธ๊ณ : ] 
+ 
</details>

-----------------------

### ์ 3 ์ ๊ทํ์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />
   
[์ฐธ๊ณ : SQL ์ฒซ๊ฑธ์] 
+ ์ 3 ์ ๊ทํ ๋ํ ์ค๋ณตํ๋ ๋ถ๋ถ์ ์ฐพ์๋ด์ด, ํ์ด๋ธ์ ๋ถํ ํ๋ ์๋ฒ์๋๋ค. <br> 
  ์ 2์ ๊ทํ์ ๊ฒฝ์ฐ์๋ ๊ธฐ๋ณธํค์ ์ค๋ณต์ด ์๋์ง ์กฐ์ฌํ์ต๋๋ค๋ง, ์ 3์ ๊ทํ์์๋ ๊ธฐ๋ณธํค ์ด์ธ์ ๋ถ๋ถ์์ ์ค๋ณต์ด ์๋์ง๋ฅผ ์กฐ์ฌํฉ๋๋ค. <br> 
  
  ๋ถํ ํ๊ธฐ ์ ์ ์ฃผ๋ฌธ ํ์ด๋ธ์ ์ดํด๋ณด๋ฉด ๋ฐ์ดํฐ๊ฐ ์ค๋ณต๋์ด ์์ต๋๋ค. <br> 
  ๊ฐ์ ์ฌ๋์ด ์ฌ๋ฌ ๋ฒ ์ฃผ๋ฌธํ๋ ๊ฒฝ์ฐ๊ฐ ์๊ธฐ ๋๋ฌธ์๋๋ค. <br> 
  ์ด ๋, ์ฃผ๋ฌธ ํ์ด๋ธ์์ ์ด๋ฆ์ ๊ธฐ์ค์ผ๋ก ์ฐ๋ฝ์ฒ๋ฅผ ํน์ ์ง์ ์ ์์ต๋๋ค. <br> 
  ๋จ, ์ฃผ๋ฌธ ํ์ด๋ธ์ ๊ธฐ๋ณธํค๋ ์ด๋๊น์ง๋ ์ฃผ๋ฌธ๋ฒํธ๋ก, ์ด๋ฆ์ ๊ธฐ๋ณธํค์๋ ๊ด๊ณ๊ฐ ์์ต๋๋ค. <br>
  ํํธ ๋ถํ ํ์ฌ ์๋ก ๋ง๋ค ํ์ด๋ธ์ ์ด๋ฆ์ '๊ณ ๊ฐ'์ด๋ผ ๋ถ์์ต๋๋ค. <br>
  
  ์ฌ๊ธฐ์๋ ์ด๋ฆ์ ๊ธฐ๋ณธํค๋ก ์ง์ ํ๋ฉด ๋๋ช์ด์ธ์ ๊ฒฝ์ฐ ๋ฐ์ดํฐ๋ฅผ ์ ๋๋ก ์ ์ฅํ  ์ ์์ผ๋ฏ๋ก, <br>
  ๊ณ ๊ฐ๋ฒํธ๋ฅผ ๊ธฐ๋ณธํค๋ก ์ง์ ํ์ฌ ๊ณ ๊ฐ ํ์ด๋ธ์ ์์ฑํ์ต๋๋ค. 
  
   
</details>

-----------------------

### Connection pool์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary>
<br />

+ ์ ํ๋ฆฌ์ผ์ด์์ ์ค๋ ๋์์ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ ๊ทผํ๊ธฐ ์ํด Connection์ด ํ์ํจ <br>
  ๋ฐ์ดํฐ๋ฒ ์ด์ค์ Connection ๊ฐ์ฒด๋ค์ ๋ฏธ๋ฆฌ ์์ฑํด Pool์ ์ ์ฅํด ๋์๋ค๊ฐ, ํด๋ผ์ด์ธํธ์ ์์ฒญ์ด ๋ค์ด์ฌ๋๋ง๋ค <br>
  ์ฌ์ฉ/๋ฐํํ๋ ๋ฐฉ์์ ์๋ฏธํฉ๋๋ค.
   
  Connection Pool์ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ ๊ทผ ๊ณผ์ ์ ๋ค์๊ณผ ๊ฐ์ต๋๋ค. <br>
  (1) ์น ์ปจํ์ด๋๊ฐ ์คํ๋๋ฉด ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ฐ๊ฒฐ๋ Connection ๊ฐ์ฒด๋ค์ ๋ฏธ๋ฆฌ ์์ฑํด Pool์ ์ ์ฅ <br>
  (2) ํด๋ผ์ด์ธํธ ์์ฒญ ์ Pool์์ Connection ๊ฐ์ฒด๋ฅผ ๊ฐ์ ธ์ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ ๊ทผ 
  (3) ์์ฒญ ์ฒ๋ฆฌ๊ฐ ๋๋๋ฉด ์ฌ์ฉ๋ Connection ๊ฐ์ฒด๋ฅผ ๋ค์ Pool์ ๋ฐํ
   
  Connection Pool์ ์ฅ์ ์ ๋ค์๊ณผ ๊ฐ์ต๋๋ค.
  (1) ๋งค ์ฐ๊ฒฐ๋ง๋ค Connection ๊ฐ์ฒด๋ฅผ ์์ฑ/์ ๊ฑฐํ๋ ๋น์ฉ์ด ๊ฐ์ํฉ๋๋ค. 
  (2) ๋ฏธ๋ฆฌ ์์ฑ๋ Connection ๊ฐ์ฒด๋ฅผ ์ฌ์ฉํ๋ฏ๋ชจ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ ๊ทผ ์๊ฐ์ ๋จ์ถํฉ๋๋ค. 
  (3) Connection ์๋ฅผ ์ ํํด ๋ถํ๋ฅผ ์กฐ์ ํ  ์ ์์ต๋๋ค. 
   
  Connection Pool์ ๋จ์ ์ ๋ค์๊ณผ ๊ฐ์ต๋๋ค. 
  (1) Connection ๋ํ ๊ฐ์ฒด์ด๋ฏ๋ก ๋ฉ๋ชจ๋ฆฌ๋ฅผ ์ฐจ์งํฉ๋๋ค. 
  (2) Connection ๊ฐ์๋ฅผ ์๋ชป ์ค์ ํ  ๊ฒฝ์ฐ, ์ธ๋ชจ์๋ Connection์ด ๋ฐ์ํ  ์ ์์ต๋๋ค. 
   
  Connection์ด ๋ถ์กฑํ  ๊ฒฝ์ฐ 
  (1) ๋ชจ๋  Connection์ด ์์ฒญ์ ์ฒ๋ฆฌ ์ค์ผ ๋, ํด๋น ํด๋ผ์ด์ธํธ์ ์์ฒญ์ ๋๊ธฐ ์ํ๋ก ์ ํํฉ๋๋ค.
  (2) Pool์ Connection ๊ฐ์ฒด๊ฐ ๋ฐํ๋๋ฉด ์์ฐจ์ ์ผ๋ก ์์ฒญ์ ์ฒ๋ฆฌํฉ๋๋ค.  
</details>

-----------------------

### ์คํ ๊ณํ์?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary> (์์ฑ์ค)
<br />

+ 
</details>

-----------------------

### ์ค๋ฉ์ด๋?

<details>
   <summary> ๋ต์ ๋ณด๊ธฐ (๐ Click)</summary> (์์ฑ์ค)
<br />
+ https://aws.amazon.com/ko/what-is/database-sharding/
+ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ๋๊ท๋ชจ ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ฅผ ์ฌ๋ฌ ๋จธ์ ์ ์ ์ฅํ๋ ํ๋ก์ธ์ค์๋๋ค. <br>
  ๋จ์ผ ๋จธ์  ๋๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์๋ฒ๋ ์ ํ๋ ์์ ๋ฐ์ดํฐ๋ง ์ ์ฅํ๊ณ  ์ฒ๋ฆฌํ  ์ ์์ต๋๋ค. <br> 
  ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ๋ฐ์ดํฐ๋ฅผ ์ค๋๋ผ๊ณ  ํ๋ ๋ ์์ ์ ํฌ๋ก ๋ถํ ํ๊ณ , <br>
  ์ฌ๋ฌ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์๋ฒ์ ์ ์ฅํจ์ผ๋ก์จ ์ด๋ฌํ ํ๊ณ๋ฅผ ๊ทน๋ณตํฉ๋๋ค.<br> 
  ๋ชจ๋  ๋ฐ์ดํฐ๋ฒ ์ด์ค ์๋ฒ์ ๊ธฐ๋ณธ ๊ธฐ์ ์ ์ผ๋ฐ์ ์ผ๋ก ๋์ผํ๋ฉฐ ํจ๊ป ์๋ํ์ฌ ๋ฐ์ดํฐ๋ฅผ ์ ์ฅํ๊ณ  ์ฒ๋ฆฌํฉ๋๋ค. <br>
    
+ ์ ํ๋ฆฌ์ผ์ด์์ด ์ฑ์ฅํจ์ ๋ฐ๋ผ ์ ํ๋ฆฌ์ผ์ด์ ์ฌ์ฉ์ ์์ ์ ํ๋ฆฌ์ผ์ด์์ ์ ์ฅ๋๋ ๋ฐ์ดํฐ์ ์๋ ์๊ฐ์ด ๊ฐ์๋ก ์ฆ๊ฐํฉ๋๋ค. <br> 
  ๋ฐ์ดํฐ ๋ณผ๋ฅจ์ด ๋๋ฌด ์ปค์ง๊ณ  ์ ํ๋ฆฌ์ผ์ด์์ ์ฌ์ฉํ์ฌ ๋์์ ์ ๋ณด๋ฅผ ์ฝ๊ฑฐ๋ ์ ์ฅํ๋ ค๊ณ  ํ๋ ์ฌ์ฉ์๊ฐ ๋๋ฌด ๋ง์์ง๋ฉด <br>
  ๋ฐ์ดํฐ๋ฒ ์ด์ค์์ ๋ณ๋ชฉ ํ์์ด ๋ฐ์ํฉ๋๋ค. <br> 
  ์ด๋ก ์ธํด ์ ํ๋ฆฌ์ผ์ด์ ์๋๊ฐ ๋๋ ค์ง๊ณ , ๊ณ ๊ฐ ๊ฒฝํ์ ์ํฅ์ ๋ฏธ์น๊ฒ ๋ฉ๋๋ค. <br>
  ์ด์ ๋ํ ์๋ฃจ์์ ํ๋๋ก, ์ฌ๋ฌ ์ค๋์์ ๋ ์์ ๋ฐ์ดํฐ ์ธํธ๋ฅผ ๋ณ๋ ฌ๋ก ์ฒ๋ฆฌํ๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ์ฌ์ฉํ๋ฉด ์ด ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ  ์ ์์ต๋๋ค. <br> 
   
+ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ์ด์ ์ ๋ค์๊ณผ ๊ฐ์ต๋๋ค. 
  (1) ์๋ต ์๊ฐ ๊ฐ์ 
  - ๋๊ท๋ชจ์ ๋จ์ผ ๋ฐ์ดํฐ๋ฒ ์ด์ค์์๋ ๋ฐ์ดํฐ๋ฅผ ๊ฒ์ํ๋๋ฐ ์๊ฐ์ด ๋ ์ค๋ ๊ฑธ๋ฆฝ๋๋ค. <br> 
    ๋ฐ์ดํฐ๋ฒ ์ด์ค ๊ด๋ฆฌ ์์คํ์ ์ฌ๋ฐ๋ฅธ ๋ฐ์ดํฐ๋ฅผ ์ฐพ๊ธฐ ์ํด ์ฌ๋ฌ ํ์ ๊ฒ์ํด์ผ ํฉ๋๋ค. <br> 
    ๊ทธ์ ๋นํด ๋ฐ์ดํฐ ์ค๋๋ ์ ์ฒด ๋ฐ์ดํฐ๋ฒ ์ด๋ณด๋ค ํ ์๊ฐ ์ ์ต๋๋ค. <br> 
    ๋ฐ๋ผ์ ์ค๋ฉ๋ ๋ฐ์ดํฐ๋ฒ ์ด์ค์์๋ ํน์  ์ ๋ณด๋ฅผ ๊ฒ์ํ๊ฑฐ๋ ์ฟผ๋ฆฌ๋ฅผ ์คํํ๋๋ฐ ๊ฑธ๋ฆฌ๋ ์๊ฐ์ด ๋จ์ถ๋ฉ๋๋ค. <br>
   
  (2) ์ ์ฒด ์๋น์ค ์ค๋จ ๋ฐฉ์ง 
  - ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ฅผ ํธ์คํํ๋ ์ปดํจํฐ์์ ์ฅ์ ๊ฐ ๋ฐ์ํ๋ฉด ๋ฐ์ดํฐ๋ฒ ์ด์ค๋ฅผ ์ฌ์ฉํ๋ ์ดํ๋ฆฌ์ผ์ด์์์๋ ์ค๋ฅ๊ฐ ๋ฐ์ํฉ๋๋ค. <br> 
    ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ์ผ๋ถ๋ฅผ ๋ค๋ฅธ ์ปดํจํฐ์ ๋ฐฐํฌํจ์ผ๋ก์จ ์ด ๊ฐ์ ๋ฌธ์ ๋ฅผ ๋ฐฉ์งํฉ๋๋ค. <br>
    ์ปดํจํฐ ์ค ํ๋์์ ์ฅ์ ๊ฐ ๋ฐ์ํ๋๋ผ๋ ์ ์ ์๋ํ๋ ๋ค๋ฅธ ์ค๋๋ฅผ ์ฌ์ฉํ์ฌ ์๋ํ  ์ ์์ผ๋ฏ๋ก ์ ํ๋ฆฌ์ผ์ด์์ด ์ค๋จ๋์ง ์์ต๋๋ค.<br> 
    ์ฆ, ์ค๋ ์ค ํ๋๋ฅผ ์ฌ์ฉํ  ์ ์๊ฒ ๋๋๋ผ๋ ๋์ฒด ์ค๋์์ ๋ฐ์ดํฐ์ ์ก์ธ์คํ๊ณ  ๋ณต์ํ  ์ ์์ต๋๋ค. <br> 
     
  (3) ํจ์จ์ ์ธ ํฌ๊ธฐ ์กฐ์  
  - ๋ฐ์ดํฐ๋ฒ ์ด์ค๊ฐ ํ์ฅ๋๋ฉด ๋ ๋ง์ ์ปดํจํ ๋ฆฌ์์ค๋ฅผ ์๋นํ๊ณ , ๊ฒฐ๊ตญ ์คํ ๋ฆฌ์ง์ ์ต๋ ์ฉ๋์ ๋๋ฌํ๊ฒ ๋ฉ๋๋ค. <br>
    ์ด ๊ฒฝ์ฐ ์กฐ์ง์ ๋ฐ์ดํฐ๋ฒ ์ด์ค ์ค๋ฉ์ ์ฌ์ฉํ์ฌ ๋ ๋ง์ ์ปดํจํ ๋ฆฌ์์ค๋ฅผ ์ถ๊ฐํจ์ผ๋ก์จ ๋ฐ์ดํฐ๋ฒ ์ด์ค์ ํ์ฅ์ ์ง์ํ  ์ ์์ต๋๋ค. <br> 
    ์ ์ง ๊ด๋ฆฌ๋ฅผ ์ํด ์ ํ๋ฆฌ์ผ์ด์์ ์ข๋ฃํ์ง ์๊ณ ๋ ๋ฐํ์์ ์ ์ค๋๋ฅผ ์ถ๊ฐํ  ์ ์์ต๋๋ค.  
   
</details>

-----------------------
