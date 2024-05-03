Grid를 사용해서 레이아웃 만들기
body아래에 생성했던 header, div.bad, div.bad-next, div.religion 에 grid속성을 사용하기 위해 부모 요소인 body에게 display: grid를 정의해줍니다.
body에 grid-template-columns: repeat(3, 33%)을 사용해서 각각 33%의 동일한 너비를 가진 3개의 열을 생성합니다.
동일한 크기를 가진 열이나 행을 생성할 때 repeat()함수를 사용할 수 있습니다.
body에 grid-template-rows: 110px 45% 35%;을 사용해서 첫 번째 행의 크기는 110px로, 두 번째 행은 전체 크기의 45%로, 세 번째 행은 전체 크기의 35%로 생성합니다.
body에 grid-template-areas을 사용해서 3행x3열의 grid 아이템을 가지는 레이아웃을 생성합니다.
grid-area를 사용해서 grid-template-areas속성에 들어가는 각각의 행과 열의 이름을 지정합니다.
header 에는 grid-area: header, div.bad에는 grid-area: bad, div.bad-next에는 grid-area: bad-next, div.religion에는 grid-area: religion를 지정해준 후 grid-template-areas 속성 안에서 행과 열을 지정해줍니다.
body에 gap:15px을 줘서 grid 아이템들의 행과 열 사이의 간격을 15px로 지정할 수 있습니다.


grid-template-columns와 grid-template-rows를 사용해서 행과 열을 생성할 수 있습니다.
grid-template-areas와 grid-area를 사용해서 grid 아이템들의 행과 열을 가지는 레이아웃을 생성할 수 있습니다.
gap을 사용해서 grid 아이템 간의 행과 열 사이의 간격을 설정할 수 있습니다.