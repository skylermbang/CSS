전체적인 HTML 구조 만들기
body아래에 크게 header, div.nav, div.under-nav, div.center, div.orders ,div.reservation , footer 를 생성합니다.
header와 footer는 가장 상단과 하단에 위치시킵니다.
div.nav와 div.under-nav는 왼쪽, div.center는 중앙, div.orders 와 div.reservation은 오른쪽에 위치시킵니다.

Grid를 사용해서 레이아웃 만들기
main아래에 자식 태그들에게 grid속성을 사용하기 위해 부모 요소인 main에게 display: grid를 정의해줍니다.
main에 grid-template-columns: 50px 1fr 50px을 줘서 각각 50px, 1fr, 50px의 크기를 갖는 3개의 열을 생성합니다.
main에 grid-template-rows: 50px repeat(2, 1fr) 50px을 줘서 각각 50px, 1fr, 1fr, 50px의 크기를 갖는 4개의 행을 생성합니다.
header와 footer에게 grid-column: 1 / -1를 줘서 시작 값 1과 끝 값 -1을 지정해서 첫 번째 line부터 마지막 line까지의 영역을 크기로 지정합니다.
div.under-nav에 grid-column: 1 / 2를 줘서 시작 값 1과 끝 값 2를 지정해서 첫 번째 line부터 두 번째 line까지의 영역을 크기로 지정합니다.
div.orders와 div.reservations에 grid-column: -2 / -1를 줘서 시작 값을 마지막 열을 기준으로 두 번째 line부터 끝 값을 마지막 열을 기준으로 첫 번째 line까지의 영역을 크기로 지정합니다.
div.center아래에 자식 태그들에 grid속성을 사용하기 위해 부모 요소인 div.center에게 display: grid를 정의해줍니다.
div.center에 grid-template-columns:repeat(2, 1fr)를 통해 동일한 너비를 가진 2개의 열을 생성합니다.
div.center에 grid-column-start: 2를 줘서 grid 아이템의 시작 값을 열에서 두 번째 줄로 지정하고 grid-row:2 / -2를 줘서 시작 값 2와 끝 값 -2를 지정해서 첫 번째 행에서 두 번째 line부터 마지막 행에서 두 번째 line까지의 영역을 크기로 지정합니다.
div.order와 div.reservation, div.nav에게 text-orientation: upright를 줘서 텍스트를 가로 방향이 아닌 세로 방향으로 배치될 수 있도록 합니다. 추가로 writing-mode: vertical-rl를 줘서 세로 방향으로 설정된 텍스트들을 위에서 아래로 배치합니다.

grid-template-columns와 grid-template-rows를 통해 행과 열을 자유롭게 생성할 수 있습니다.
grid-column과 grid-row를 사용해서 행 또는 열의 셀 영역 크기를 지정할 수 있습니다.
grid-column-start와 grid-row-start를 사용해서 grid 아이템의 시작 값을 지정할 수 있습니다.
writing-mode 속성을 사용해서 텍스트 행을 가로에서 세로로 설정할 수 있습니다.
text-orientation속성을 사용해서 텍스트 문자의 방향을 설정할 수 있습니다.