# 📝 google-survey-form
Form 관련 태그 학습을 위해 클론한 구글 설문 폼.
아래의 preview 이미지를 따라 만들었다.
<center width="100px">![preview](https://i.imgur.com/Oh2u02k.png)</center>

[🔗웹에서 확인하기](https://yeodahui.github.io/google-form/)

### 어려웠던 점
1. 각 문항마다 블럭이 구분되어 있어 모든 문항을 감싼 그룹핑 태그에 스타일을 어떻게 적용해야 할 지 고민되었다.
2. 학습차 reset.css를 import하지 않고 스타일 시트를 작성하려 하니 의도치 않은 margin과 padding때문에 적절한 여백을 주는 것이 어려웠다.

### 새로 배운 점
1. 계정 전환 탭에서 아이콘을 svg나 png로 넣으려 했는데, 구글에서 Material Icons를 제공한다는 것을 알게 되었다. span 태그에 class를 주는 것 만으로 icon을 뚝딱 만들어준다. [🔗Material Icons Guide](https://developers.google.com/fonts/docs/material_icons#icon_font_for_the_web)
  ```html
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">
  ```
  위의 link 코드를 삽입하기만 하면 되었고, visiblity off 아이콘을 사용할 수 있었다.
  ```html
  <link href="https://fonts.googleapis.com/css?family=Material+Icons|Material+Icons+Outlined|Material+Icons+Two+Tone|Material+Icons+Round|Material+Icons+Sharp" rel="stylesheet">
  ```
  outline이 들어간 아이콘을 사용하고 싶으면 위 링크로 대체하면 된다.
2. select, input[type="date"]와 input[type="time"]은 운영체제 혹은 브라우저 별로 다른 디자인이 적용된다. 이걸 커스텀하기 위해서는 Javascript를 사용해야 한다.
3. select 태그의 우측의 화살표는 padding에 영향을 받지 않는다. 이 화살표를 커스텀하고 싶을 경우 webkit을 수정해 화살표를 없애고 background-image로 아이콘을 삽입하는 방법이 있다.
4. 모든 input 태그에는 가급적 label을 붙여주는 것이 좋다. 디자인 상에서 라벨이 불필요한 경우에는 hidden 클래스를 주고 display: none;을 설정한다.
