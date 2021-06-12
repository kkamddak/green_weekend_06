# HTML, CSS, JS 기초

## HTML

> HTML : Hypper Text Markup Language
> 
> 웹페이지의 <b>구조</b>를 표시
> 
> 웹페이지의 콘텐츠를 표시
> 
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

> 
