# ๐ google-survey-form
Form ๊ด๋ จ ํ๊ทธ ํ์ต์ ์ํด ํด๋ก ํ ๊ตฌ๊ธ ์ค๋ฌธ ํผ.
์๋์ preview ์ด๋ฏธ์ง๋ฅผ ๋ฐ๋ผ ๋ง๋ค์๋ค.
<center>
  <img src="https://i.imgur.com/Oh2u02k.png" width="150">
</center>

[๐์น์์ ํ์ธํ๊ธฐ](https://yeodahui.github.io/google-form/)

### ์ด๋ ค์ ๋ ์ 
- ๊ฐ ๋ฌธํญ๋ง๋ค ๋ธ๋ญ์ด ๊ตฌ๋ถ๋์ด ์์ด ๋ชจ๋  ๋ฌธํญ์ ๊ฐ์ผ ๊ทธ๋ฃนํ ํ๊ทธ์ ์คํ์ผ์ ์ด๋ป๊ฒ ์ ์ฉํด์ผ ํ  ์ง ๊ณ ๋ฏผ๋์๋ค.
- ํ์ต์ฐจ reset.css๋ฅผ importํ์ง ์๊ณ  ์คํ์ผ ์ํธ๋ฅผ ์์ฑํ๋ ค ํ๋ ์๋์น ์์ margin๊ณผ padding๋๋ฌธ์ ์ ์ ํ ์ฌ๋ฐฑ์ ์ฃผ๋ ๊ฒ์ด ์ด๋ ค์ ๋ค.

### ์๋ก ๋ฐฐ์ด ์ 
- ๊ณ์  ์ ํ ํญ์์ ์์ด์ฝ์ svg๋ png๋ก ๋ฃ์ผ๋ ค ํ๋๋ฐ, ๊ตฌ๊ธ์์ Material Icons๋ฅผ ์ ๊ณตํ๋ค๋ ๊ฒ์ ์๊ฒ ๋์๋ค. span ํ๊ทธ์ class๋ฅผ ์ฃผ๋ ๊ฒ ๋ง์ผ๋ก icon์ ๋๋ฑ ๋ง๋ค์ด์ค๋ค. [๐Material Icons Guide] (https://developers.google.com/fonts/docs/material_icons#icon_font_for_the_web)
  ```html
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">
  ```
  ์์ link ์ฝ๋๋ฅผ ์ฝ์ํ๊ธฐ๋ง ํ๋ฉด ๋์๊ณ , visiblity off ์์ด์ฝ์ ์ฌ์ฉํ  ์ ์์๋ค.
  ```html
  <link href="https://fonts.googleapis.com/css?family=Material+Icons|Material+Icons+Outlined|Material+Icons+Two+Tone|Material+Icons+Round|Material+Icons+Sharp" rel="stylesheet">
  ```
  outline์ด ๋ค์ด๊ฐ ์์ด์ฝ์ ์ฌ์ฉํ๊ณ  ์ถ์ผ๋ฉด ์ ๋งํฌ๋ก ๋์ฒดํ๋ฉด ๋๋ค.
- select, input[type="date"]์ input[type="time"]์ ์ด์์ฒด์  ํน์ ๋ธ๋ผ์ฐ์  ๋ณ๋ก ๋ค๋ฅธ ๋์์ธ์ด ์ ์ฉ๋๋ค. ์ด๊ฑธ ์ปค์คํํ๊ธฐ ์ํด์๋ Javascript๋ฅผ ์ฌ์ฉํด์ผ ํ๋ค.
- select ํ๊ทธ์ ์ฐ์ธก์ ํ์ดํ๋ padding์ ์ํฅ์ ๋ฐ์ง ์๋๋ค. ์ด ํ์ดํ๋ฅผ ์ปค์คํํ๊ณ  ์ถ์ ๊ฒฝ์ฐ webkit์ ์์ ํด ํ์ดํ๋ฅผ ์์ ๊ณ  background-image๋ก ์์ด์ฝ์ ์ฝ์ํ๋ ๋ฐฉ๋ฒ์ด ์๋ค.
- ๋ชจ๋  input ํ๊ทธ์๋ ๊ฐ๊ธ์  label์ ๋ถ์ฌ์ฃผ๋ ๊ฒ์ด ์ข๋ค. ๋์์ธ ์์์ ๋ผ๋ฒจ์ด ๋ถํ์ํ ๊ฒฝ์ฐ์๋ hidden ํด๋์ค๋ฅผ ์ฃผ๊ณ  display: none;์ ์ค์ ํ๋ค.
