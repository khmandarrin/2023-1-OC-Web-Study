<HTML>

1. 시맨틱 웹(Semantic Web)
:  웹에 존재하는 수많은 웹페이지들에 메타데이터(Metadata)를 부여하여, 기존의 잡다한 데이터 집합이었던 웹페이지를 ‘의미’와 ‘관련성’을 가지는 거대한 데이터베이스로 구축하고자 하는 발상

> 크롤링 : 검색엔진이 로봇(Robot)이라는 프로그램을 이용해 매일 전세계의 웹사이트 정보를 수집하는 것

> 인덱싱 : 검색 사이트 이용자가 검색할 만한 키워드를 미리 예상하여 검색 키워드에 대응하는 인덱스(색인)을 만들어 두는 것

> 시맨틱 태그 : 브라우저, 검색엔진, 개발자 모두에게 콘텐츠의 의미를 명확히 설명하는 역할

> non-semantic 요소 
: div, span 등이 있으며 이들 태그는 content에 대하여 어떤 설명도 하지 않는다.
> semantic 요소
: form, table, img 등이 있으며 이들 태그는 content의 의미를 명확히 설명한다.

2. 웹페이지를 구성하는 기본 태그
> 문서 형식 정의 tag <!DOCTYPE html>
: 출력할 웹 페이지의 형식을 브라우저에게 전달 

> html tag :html 태그는 모든 HTML 요소의 부모 요소이며 웹페이지에 단 하나만 존재

> head tag : head 요소는 메타데이터를 포함하기 위한 요소이며 웹페이지에 단 하나만 존재한다. 메타데이터는 HTML 문서의 title, style, link, script에 대한 데이터로 화면에 표시되지 않는다.

> title tag : 문서의 제목을 정의한다. 정의된 제목은 브라우저의 탭에 표시

> style tag : HTML 문서를 위한 style 정보를 정의

> link tag : 외부 리소스와의 연계 정보를 정의한다. 주로 HTML과 외부 CSS 파일 연계에 사용

> script tag : client-side JavaScript를 정의

> meta tag : meta 요소는 description, keywords, author, 기타 메타데이터 정의에 사용된다. 메타데이터는 브라우저, 검색엔진(keywords) 등에 의해 사용된다.

> body tag : HTML 문서의 내용을 나타내며 웹페이지에 단 하나만 존재


<CSS(Cascading Style Sheets)>

: HTML이나 XML과 같은 구조화 된 문서(Document)를 화면, 종이 등에 어떻게 렌더링할 것인지를 정의하기 위한 언어

> HTML5에서는 HTML는 정보와 구조화, CSS는 styling의 정의라는 명확한 구분

> 박스 모델
: 콘텐트(Content), 패딩(Padding), 테두리(Border), 마진(Margin)로 구성

1. 셀렉터 (Selector, 선택자)
: 스타일을 적용하고자 하는 HTML 요소를 선택

> 전체 셀렉터, 태그 셀렉터, ID 셀렉터, 클래스 셀렉터, 어트리뷰트 셀렉터, 복합 셀렉터(후손 셀렉터, 자식 셀렉터, 형제 셀렉터) 가상 클래스 셀렉터, 링크 셀렉터, 동적 셀렉터, UI요소 상태 셀렉터, 구조 가상 클래스 셀렉터, 부정 셀렉터, 정합성 체크 셀렉터, 가상 요소 셀렉터

2. 프로퍼티 (Property / 속성)
: 셀렉터로 HTML 요소를 선택하고 {} 내에 프로퍼티(속성)와 값을 지정하는 것으로 다양한 style을 정의, 표준 스펙으로 이미 지정되어 있는 것을 사용

> width / height, margin : 4개의 방향 / padding, border(border-style : 테두리 선 스타일, border-width : 테두리 두께, border-color : 테두리 색상, border-radius : 둥근 모서리, border), box-sizing, 

> font-size, font-family : 폰트 지정, font-style : 이탤릭체 / font-weight : 폰트 굵기 등

> position : 요소의 위치 정의 (static, relative, absolute, fixed), z-index, overflow : 자식 요소가 부모 요소의 영역를 벗어났을 때 처리 방법

> float : 레이아웃을 구성할 때 블록 레벨 요소를 가로 정렬하기 위해 사용 
*요소의 위치를 고정시키는 position 프로퍼티의 absolute 사용하면 안됨

3. 값 (Value / 속성값)
: 프로퍼티의 값은 해당 프로퍼티에 사용할 수 있는 값을 “키워드”나 “크기 단위” 또는 “색상 표현 단위” 등의 특정 단위로 지정

> 대표적인 크기 단위는 px(픽셀), em(배수, 폰트 사이즈 설정, 컨테이너 크기 설정), %

> Viewport 단위 (상대적) : vh, vw, vmin, vmax

> 색상 표현 단위 : red, green, blue ... / HEX 코드 단위... 

4. HTML과 CSS의 연동
> Link style : HTML에서 외부에 있는 CSS 파일을 로드
> Embedding style : HTML 내부에 CSS를 포함시키는 방식
> Inline style : HTML요소의 style 프로퍼티에 CSS를 기술하는 방식

