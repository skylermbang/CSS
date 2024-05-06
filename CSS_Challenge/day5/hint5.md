body에 grid-template-columns: repeat(auto-fit, minmax(255px, 1fr))을 줘서 자식 요소들의 너비를 지정합니다.
minmax(255px, 1fr) 함수를 사용해서 자식 요소들의 최소 크기는 255px로, 최대 크기는 fr단위를 사용해서 남아 있는 공간 안에서 일정 비율로 모두 채웁니다.
auto-fit을 사용해서 남아있는 column공간이 있다면 자동으로 grid 아이템들의 공간으로 모두 채웁니다.
grid-template-rows: 8vw를 사용해서 가장 상단의 header태그의 높이를 vw단위를 사용해서 가변적으로 지정합니다.
grid-auto-rows: 46vh를 해줘서 추가로 생기는 content들에 대해서 따로 크기를 지정해주지 않아도 자동으로 기본값을 할당해서 생성해주도록 합니다.
header태그에 grid-column: 1 / -1를 사용해서 시작 값 1과 끝 값 -1을 지정해서 첫 번째 line부터 마지막 line까지의 영역을 크기로 지정합니다.