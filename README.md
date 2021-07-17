# HTML, CSS, JS 기초

## HTML

> HTML : Hypper Text Markup Language
>
> 웹페이지의 콘텐츠를 표시
> 
> 웹페이지의 <b>구조</b>를 표시


### HTML Elements

> Element :요소 - 의미적
> 
> Tag : 태그 - 기술적
> 
> 문법
> 
> <>로 감싸줌 
>   
>  소문자 사용 
>    
> 시작태그와 종료태그 세트로 구성됨.
```
<tagname>contents</tagname>
```   
>  예외) 시작태그만 존재하는 경우 : 빈 태그(Empty Element)
>  
>  포함관계(Nested)
```  
<bod>
  <div>
    text
  </div>
</body>
```

### HTML Attribute

> HTML 속성
> HTML 요소의 부가 정보
> 속성이름 =  '속성값'

```
<a hre="http://www.naver.com">naver</a>
```

### HTML 페이지에서 표시하는 콘텐츠

> 텍스트 콘텐츠
> 멀티미디어 콘텐츠(임베디드embeded 콘텐츠)
> - 이미지
> - 비디오
> - 오디오


### 제목 태그

> heading -> h
> 
> h1 ~ h6
> 
> h1이 가장 큰 제목
>

### HTML기본 구조

```
<!DOCTYPE html> - 1
<html> - 2
  <head> - 3
    <meta charset="utf-8"> - 4
    <title>My test page</title> - 5
  </head>
  <body> - 6
    <p>This is my page</p>
  </body>
</html>
```

1. 웹 문서의 버젼 : HTML5
2. HTML문서의 가장 바깥쪽 요소
3. 웹 문서를 설명하는 정보가 담기는 영역 요소
4. 웹 문서의 정보 표시 요소
5. 웹 문서의 제목을 표시하는 요소
6. 웸 문서의 콘텐츠 요소들이 담기는 영역 요소


### 단락 태그

> p(Paragraph : 단락을 표시
> 
> 단락과 단락 사이를 구분하는 수평선 
```
<hr> - Horizontal Rule
```
> 단락을 구분하지 않고 줄 바꿈
```
<br> - Break
```

### 목록 태그

> 순서없는 목록 ul(Unordered List)
> 
> 순서있는 목록 ol(Ordered List)
> 
> 목록 항목 li(List Item)

```
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>HTML</li>
  <li>CSS</li>
</ol>
```

> 포함관계(nested)로 구성된 목록 - 코딩할 때 밖에서 안쪽 방향 순서로
- HTML
  - HTML4
  - HTML5
- CSS
  - CSS2
  - CSS3
```
<ul>
  <li>
  HTML
    <ul>
      <li>HTML4</li>
      <li>HTML5</li>
    </ul>
  </li>
  <li>
  CSS
   <ul>
     <li>CSS2</li>
     <li>CSS3</li>
   </ul>
  </li>
</ul>
```
> 설명 목록 dl(Description List)
```
<dl>
  <dt>HTML</dt> - dt : Discription Title
  <dd>표준 마크업 언어</dd> - dd : Dscription Data
</dl>
```

### HTML Hyper link

> 하이퍼링크 a(anchor)
> 
> attribute(속성) : href(Hypertext Reference) : 연결되는 웹 문서의 URL
```
<a href="http://naver.com">네이버로 이동</a>
```
> 북마크 기능
> 
> 외부 페이지 연결이 아닌 같은 페이지에서 특정위치로 이동할 수 있게 해주는 기능
> 
> 도착지점에 id attribute를 사용하여 이름을 지정
```
<a href="#t1">목차</a>
<h2 id="t1">제목</h2>
```

### Table Element

> 기본 사용 태그 : table, thead, tbody, tr, th, td
>
> 열 제목 : thead(table hade), th(table heading)
>
> 표 내용 : tbody(table body), td(table data)
>
> 행 : tr(table row)
> 
https://www.tablesgenerator.com/html_tables


### Image Element

> Tag : immg
> 
> Attribute : src(image 위치, 파일명), alt(대체텍스트)

` : backtick
```
<img src="image.jpg" alt="대체텍스트">
```

### Video Element

> 비디오 및 오디오 콘텐츠는 용량이 크기 때문에 서버에 저장을 해서 콘텐츠를 제공하면 많은 트래픽이 발생할 수 있음.
> 
> 트래픽 과부하를 해결하기 위해서 유튜브 서비스를 사용하기 함.
> 
> attribute
> 
> controls : 컨ㅌ롤 버튼 표시
> 
> autoplay : 자동재생(* muted와 같이 사용해야 함)
> 
> muted : 음소거
> 
> loop : 반복 재생 


### Youtube

> 비디오 콘텐츠 제공시 서버의 트래픽 과부하를 해결할 수 있는 방법중의 하나
> 
> 매개변수
> 
> controls=1,0
> 
> autoplay=1,0 (mute와 같이 사용)
> 
> mute=1,0
> 
> loop=1,0 (playlist와 같이 사용)


> 텍스트는 HTML 문서에 직접 입력되는 콘텐츠
> 
> 이미지와 동영상, 오디오는 외부에서 만들어지는 콘텐츠
> 
> 이미지, 동영상 오디오는 직접 입력하는 것이 아니고 외부 파일을 삽입 => embed 콘텐츠

### 웹 사이트 템플릿 디자인

https://freebiesbug.com/psd-freebies/minimo-minimal-blog-template/

### Container Element (단순 영역 구분 요소)

> div(division)
> 
> span

### Block, Inline

> 모든 element는 각각의 고유 영역을 가지고 있음.
> 
> Block element, Inline elemnet 구분은 이들 영역의 화면 표시 방식에 따른 구분
> 
> Block element는 줄바꿈 되어 표시 - Block elemnet 영역의 가로 너비가 부모 요소에 100% 채워짐
> (** 포함하는 요소 : 부모요소, 포함되는 요소 : 자식요소)
>
> Block elemnt에는 위, 아래 여백을 적용할 수 있음
> 
> Inline elemnent는 같은 줄에 나란히 표시 - Inline element 영역의 가로 너비가 콘텐츠 크기만큼만 정해짐 
> 
> Inline elemnent는 위, 아래 여백을 적용할 수 없음


### Parent Element(부모요소), Child Elemnent(자식요소)

> 포함관계에서 포함하는 요소가 부모요소, 포함되는 요소가 자식요소
> 
> 직계 포함관계에서만 부모요소, 자식요소
> 
> 직계가 아닌 포함관계에서는 조상요소(Ancestor Element), 자손요소(Descendant Elemnet)


### CSS 기본 개념

> 선택자는 스타일을 지정할 HTML 요소를 가리킵니다.
>
> 선언 블록에는 세미콜론으로 구분 된 하나 이상의 선언이 포함됩니다.
>
> 각 선언에는 콜론으로 구분 된 CSS 속성(Property0 이름과 값(Value)이 포함됩니다.
>
> 여러 CSS 선언은 세미콜론으로 구분하고 선언 블록은 중괄호로 묶습니다.

### Id, Class

> HTML Elemnet에 특정 이름을 사용할 때 id, class attribute를 사용해서 이름을 붙여줄 수 있음.
> 
> id는 동일한 이름이 사용된 HTML Element가 여러개이면 논리적 오류가 발생
> 
> id는 HTML 문서내에서 고유해야함
> 
> class는 동일한 이름이 여러 개의 element에 사용되어 공통 디자인 요소나 공통 기능을 적용할 수 있음.
> 
> id는 주로 서버에서 불러오는 데이터를 표시하는 위치에 고유하게 사용 -> 백엔드 개발에서 주로 사용
> 
> class는 주로 css 스타일 적용, javascript 인터랙센 적용할 때 사용 => 프론드엔드 개발에서 주로 사용

id는 하나의 HTML Elemnet에 대해서 하나의 이름만 존재, HTML 문서내에서 고유해야 함.

class는 하나의 HTML Elemnet에 대해서 여러개의 이름을 지정할 수 있고, HTML 문서내에서 여러 곳에서 공통 사용 가능함.
> 

### CSS 작성방법

> External CSS : 파일 분리
> 
> Internal CSS : 같은 HTML 문서내에 head태그 영역에 style태그를 사용하여 입력
> 
> Inline CSS : 시작태그에 style arrtibute를 사용해서 입력 -> javascript에서 css를 제어할 때 사용


### naming할 때 표기방식

> id/class naming, 변수/함수/클래스 naming, 파일/폴더 naming의 경우 가독성을 높이기 위해 사용
> 
> naming할 때 두단어 이상으로 구성되는 경우 단어와 단어 사이를 구분하기 위해 사용
> 
> 단어의 시작부분에 첫글자를 대문자로 변경, 특수기호를 사용

> 표기방식을 사용하는 이유 
> 
> - naming 할 때 두단어 이상으로 구성되는 경우 단어와 단어 사이를 구분하기 위해 사용
> 
> - 단어의 시작부분에 첫글자를 대문자로 변경, 특수기호를 사용
> 
> 표기방식 종류
> 
> snake case : gnb_depth1 => 파일/폴더
> 
> kebab case : gnb-depth1 => id/class
> 
> camel case : gnbDepth1  => javascript의 변수/함수 
> 
> pascal case : GnbDepth1 => javascript의 클래스


### OGCSS(Object Oriented CSS)

> HTML Element를 대상화 시키는 과정에서 Element 하나하나를 모두 객체화 시키는 이론
> 
> HTML Element 모두 각각 id, class attribute를 사용해서 이름을 지정해줌.


### Web Colors

> color mode
> 
> - 가산혼합(빛의 혼합) : RGB 컬러모드
> 
> 표현할 수 잇는 색의 계수
> 
> 1byte = 8bit = 256개(0~255)
> 
> RGB => 3btte => 24bit 트루컬러 : 16777216가지 색
> 
> 색 표현 코드값
> 
> 16진수(hex code) : #AAABA01
> 
> 10진수 : (255, 255, 255)
> 
> CSS 사용법
> 
```
color: #fcba03;
color: rgb(252,186,3);
color: rgba(252,186,3, 0.5);
```

> 투명도를 의미하는 용어
> - transparent : 튜명한
> - akoga : 추가 채널
> - opacity : 불투명도


### Text CSS

> - color
> 
> - text align : left, center, right, justify
> 
> - text-decoration : underline, line-through, overline, none
> 
> - text-transform : uppercase, lowecase, Capitalize
> 
> - text-indent : 20px / -20px
> 
> - letter-spacing : 2px / -2px
> 
> - line-height : 20px / 1.8(배수)
> 
> - word-spacing
> 
> - white-space : nowrap
> 
> - text-shadow 


### Font CSS

 - font-family : "Times New Roma", Times, serif;
 
   - 순서대로 대체 폰트를 찾음
 
   - sans-serif, serif, monospace, cursive, fantasy 5개의 기본폰트는 font-family 사용시 종류에 맞게 항상 끝에 기본으로 사용됨
 
   - 웹사이트에 사용하는 폰트는 웹폰트(서버에 폰트 파일을 저장해서 사용)로 사용하는 데, 업로드된 파일을 직접 사용하는 경우, 웹폰트 서비스를 사용하는 경우 2가지가 있음
 
   - 대표적인 웹폰트 서비스 : 구글 폰트, 눈누
 
 - font-size
 
 - font-style : italic

 - font-weight : bold / 500
   - 폰트 굵기가 다양한 경우 숫자로 굵기를 표현


### Box Mode 1

> 구성요소
> 
> - width/height : 너비/높이
> 
> - padding : 안쪽 여백
> 
> - border : 테두리
> 
> - margin : 바깥 여백


### Wwdth/height
> width : 너비/가로길이
> 
> height : 높이/세로길이
> 
> auto : 기본값
> 
> - Block : 너비 : 부모요소를 기준으로 채워짐 / 높이 : 콘텐츠(자식요소)를 기준으로 맞춰짐
>  - inline : 너비/높이 : 콘텐츠(자식요소)에 맞춰짐
> 


### padding
> 안쪽여백
>
> padding-top
> 
> padding-right
> 
> padding-bottom
> 
> padding-left

> padding : 10px 20px 30px 40px (top right bottom left)
> padding : 10px 20px 30px (top right/left bottom)
> padding : 10px 20px (top/bottom right/left)
> padding : 10px (top/right/bottom/left)


### magine

> padding과 사용방법이 같음
> 
> margine collapse
> - 위 아래 인접하게 배치된 박스의 사이여백이 둘 중 큰쪽으로만 적용되어 표현되는 현상
> - 위아래 양쪽으로 margine을 적용하는 것보다 한쪽을 기준으로 적용하는 것이 더 좋음


### border

> border-top
> 
> border-right
> 
> border-bottom: 
> 
> border-left: 1px solid red;


### 가로 배치
※ inline 요소는 박스 모델이 제대로 적요되지 않기 때문에 레이아웃 구성 요소로 사용하기 어렵다.
※ block 요소를 레이아웃 구성 요소로 사용함 => 세로 배치는 기본 구성

가로 배치 기법
- float
- flex
- grid


### float
> left, right 값을 사용해서 가로 배치
> left, right는 부모요소를 기준으로 방향성을 표현
> 일반적으로 왼쪽을 기준으로 순서대로 배치할 때 left만 사용해서 배치

> float는 박스가 띄워지는 현상이 있기 때문에 인접해 있는 박스의 배치가 깨질 수 있음
> float 박스를 부모요소로 감싸서 인접해 있는 박스와 float 박스를 감싸고 있는 부모요소와의 관계로 만들어 줌
> float 박스를 감싸는 부모요소는 높이가 0이 될 수 있기 때문에 그것을 clear 할 수 있는 비어있는 자식요소를 넣어줌

```
HTML
<div class="float-container">
  <div class="float-box">text</div>
  <div class="float-box">text</div>
  <div class="clearfix"></div>
</div>

 CSS
 .float-box{
   float: left;
 }
 .clesarfix {
   clear: both;
 }
```

