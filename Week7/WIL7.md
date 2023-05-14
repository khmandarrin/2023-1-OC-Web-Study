<유튜브 클론>

.grey-bakcground:hover {   // 마우스를 올리면 생기는 일 정의
  background-color: grey;  // 배경색을 회색으로
  cursor: pointer;         // 커서를 포인터로
}

.dropdown-box{
    display:none;
    position:absolute;     // 부모 요소 또는 가장 가까이 있는 조상 요소(static 제외)를 기준으로 좌표 프로퍼티만큼 이동
    padding:10px;
    margin-top: 60px;

    z-index:1;             // z-index 프로퍼티에 큰 숫자값을 지정할수록 화면 전면에 출력 (static 이외인 요소에만 적용)
}

> Flexbox 레이아웃 특징
1. 1줄의 코드 추가로 수평 정렬이 가능하다.
2. 요소의 상하좌우 정렬, 순서 변경이 간단하다.
3. 요소가 간격 조절이 간단하다.
4. 서로 다른 height를 갖는 요소의 수평정렬 시, 간단히 상하중앙 정렬이 가능하다.

flexbox를 사용하기 위해 HTML 부모 요소의 display 속성에 flex를 지정 EX)
.flex-container {
  display: flex;
}

*부모 요소가 inline인 경우
.flex-container {
  display: inline-flex;
}

flex-direction : flex 컨테이너의 주축 방향 설정, (row, row-reverse, column, column-reverse)
flex-wrap : flex 컨테이너의 복수 flex item을 1행으로 또는 복수행으로 배치 (nowrap, wrap, wrap-reverse)
justify-content : flex container의 주축 기준으로 flex item을 수평 정렬 (flex-start, flex-end, center, space-between, space-around)

align-items : flex item을 flex container의 수직 방향으로 정렬 (stretch, flex-start, flex-end, center, baseline)'
align-content : flex container의 수직 방향을 기준으로 flex item을 수직 정렬 (stretch, flex-start, flex-end, center,space-between, space-around)

> flexbox를 이용한 수평, 수직 정렬

수평 정렬 EX)
.flex-center {
  display: flex;
  justify-content: center;
}

수직 정렬 EX)
.container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 400px;
}