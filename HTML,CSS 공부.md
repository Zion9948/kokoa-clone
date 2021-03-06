# 시작
브라우저가 우리의 text파일을 읽고 웹사이트를 만들어준다. 

2가지의 text 3가지의 text로 웹사이트는 이루어져있다. 즉 text = language

그것은 바로 > HTML5, CSS, Javascript 이다. 

## HTML

HTML은 content, title, image, text 들로 구성된 뼈대이다. 

HTML은 웹프로그래밍 언어가 아니라 Markup 언어이다. Markup은 content이다. 

- HTML로 부라우저에게 content 구조가 어떤지를 설명해주는것이다.
- **HTML은 부라우저에게 웹사이트의 content가 어떻게 구성되어 있는지 설명할 때 사용한다.**

## CSS

Cascading Style Sheet

Css는 디자인과 스타일을 위한 언어이다. 

- Css는 HTML과 함께 사용해야한다.
- **CSS는 browser에게 content가 어떻게 보여야하는지에 대해 알려준다.**

HTML은 브라우저에게 이건 이미지고 이건 타이틀이야 라고 말한다면, CSS는 브라우저야 이 이미지는 가로 25px 세로 100px이어야해 그리고 이 타이틀은 녹색이야 라고 하는것이다. 

#구성과 디자인의 차이는 HTML과 CSS의 차이 

## Javascript

HTML은 뼈대(구성), CSS는 근육(이미지), Javascript는 뇌(상호작용)

Javascript는 웹프로그래밍 언어이다. 

동적 상호작용성(interactivity)의 역활을 Javascript가 한다. 

클릭하면 다른 웹사이트로 들어가고 동영상이 재생되고 메뉴바가 생기고 하는 것들이다.

## 웹사이트를 만들자!

HTML은 에러를 발생시키지않고 적혀있는것을 모두다 브라우저에 띄운다. 

이것은 좋은점이면서 안좋은점이다. 무엇이 잘못되었는지 알려주지 않기 때문이다. 

![스크린샷 2022-05-04 오후 10.23.29.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b86c684e-2918-4659-b6c6-4d4ff2742777/스크린샷_2022-05-04_오후_10.23.29.png)

HTML도큐먼트를 만들자

진짜 HMTL코드를 적어보자

HTML의 목적

브라우저한테 무언가를 알려주는건 이건 타이틀 , 이건 링크, 이건 이미지야 이렇게 말하는것이다.

# HTML

## tag

HTML문법은 태그를 통해서 진행된다. 중요한점은 /(슬라이스)이다 슬라이스의 의미는 태그를 닫다 즉, 내가 원하는 부분만 태그시키겠다라는 의미이다.

### <h1></h1>  header number 1

태그를 작성 할 때 올바른 text와 올바른 위치에 그에 맞는 올바른 tag를 사용하면된다. 

브라우저가 이해할수잇는 **h태그는 h6까지 밖에 없다.** 

모든 태그를 전부 암기할 필요는없다. 왜냐면 태그가 너무 많기 때문이다. 즉 태그가 어떻게 실행되는지만 알면 그때마다 찾아서 사용하면 된다. 

### <ul></ul> list tag

순서가 없는 목록

<li></li> 리스트 아이템  ul태그 안에다가 작성한다. 

```java
<ul>
    <li>beer</li>
    <li>김치</li>
    <li>meat</li>
    <li>milk</li>
</ul>
```

- 이렇게 순서없는 목록으로 지정한다.

### <ol></ol> list tag

순서가 있는 목록 

<li></li> 리스트 아이템  ol태그 안에다가 작성한다. 

```java
<ol>
    <li>beer</li>
    <li>김치</li>
    <li>meat</li>
    <li>milk</li>
	</ol>
```

1,2,3,4처럼 순서를 지정한다. 

### a 태그

a = anchor:닻

- anchor는 다른 웹사이트로 이동하게 해주는 방법이다. 즉, link를 떠올리면 됌.
- link는 부가적인 정보가 더 필요하다
- tag에 추가하는 부가적인 정보를 attributes라고 부른다.

href는 “HTTP reference” 혹은” hyperlink reference”라고 한다. 

a태그의 부가적인 정보는 href이다. 이것이 있어야 다른사이트로 링크해줄수있다. 

```html
<a href="http://google.com">Go to google.com</a>
```

위의 코드를 읽고 브라우저는 anchor안의 href가 구글로 이동 시켜주는걸로 이해한것이다. 

**중요한점 attribute href은 anchor(a) 태그에만 추가 할 수 있는것이다.** 

### target=”_blank”   target=”_self”

```html
<a href="http://google.com" target=”_blank”>Go to google.com</a>

<a href="http://google.com" target=”_self”>Go to google.com</a>
```

blank는 a태그를 통해서 다른 웹사이트로 이동할때 자신의 창은 그대로 두고 새로운 링크창을 띄우는 것

self는 자신의 창으로 새로운 링크창을 띄우는것

### img태그 <img/>

이미지는 self-closing tag이다. 이미지는 이미지이니까!!

이미지 태그의 attribute는 src이다. 

```html
<img src="http://cdn.edujin.co.kr/news/photo/202001/32170_56414_4217.png"
/>
```

**<주의>img의 scr가 contentdlrl 때문에 이미지 태그는 다른 태그들과 달리 self-closing tag이다.** 

scr는 img태그에서만 작동한다. 

이미지 파일은 인터넷에 있는 이미지 주소를 통해서 보여줄수있고 다른방법은 이미지 파일을 html과 같은폴더에 위치해 있으면 가능하다. html파일 바로옆에 위치해있게 만들면 된다. 

수많은 tag는 수많은 attribute를 가지고있다. 

내가 이해하는 말로는 태그는 구문같은것이고 attribute는 그 구문에서 사용가능한 기능들인것같다. 

## HTML 문서의 구조를 작성하는 방법

따라야하는 형태

모든 HTML의 첫번쨰 라인 <!DOCTYPE.html>

두번째 html 태그 <html></html>

```html
<!DOCTYPE html>
<html></html>
```

웹사이트는 두개의 구조로 되어있다.

- head > 웹사이트의 환경을 설정함 (외부적으로 보여지지 않는 설정)
- body > 사용자가 볼수잇는 content를 보여줌

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Heloo this is my website!</h1>
    <il>
      <li>beer</li>
      <li>김치</li>
      <li>meat</li>
      <li>milk</li>
    </il>

    <a href="http://google.com" target="_self">Go to google.com</a>

    <img src="http://cdn.edujin.co.kr/news/photo/202001/32170_56414_4217.png" />
    <img src="KakaoTalk_Photo_2017-10-23-18-34-52.jpeg" alt="" />
  </body>
</html>
```

## head

페이지에 관한 환경 설정해주는 곳

그중 하나가 title이다. 브라우저의 도메인을 설정하는곳

```html
<head>
    <title>시온의의 페이지</title>
  </head>
```

헤드사이에 넣어주는것이 포인트이다. 

브라우저 화면 상에 보여질 내용들은 전부 body 태그에 있어야하고 

head 태그 안에 있는 것들은 화면 상에 보여지지 않는다. 

## 보이지 않는 태그

### meta(부가적인 정보) 태그, 모든 meta태그들은 **self-closing**태그이다! (head사이에 적어주는 태그)

meta 태그는 두개의 attribute를 갖고잇다. name 과 content.

<meta name = “description” conthent=”this is my website” />

### <meta charset=”utf-8”>

브라우저에게 text를 어떻게 그려달라는지 말해준다. (때때로 한글이나 특수문자들을 브라우저가 이해하지 못하는 경우가 있다.) 항상 meta charset=”utf-8”을 까먹지 말고 적어주자

```html
<html>
  <head>
    <title>시온의의 페이지.</title>
    <meta name="“description”" conthent="”This" is my website” />
	  <meta charset=”utf-8”>
  </head>
<html>
```

### lang attribute

2번째라인 html 옆에 적어두는 attribute! 

사용이유: 네이버 구글 검색엔진들에게 도움을 주기 위해(우리사이트가 사용하는 언어가 무엇인지 설명하는것이다.)

```html
<html lang="kr">
  <head>
    <title>시온의의 페이지.</title>
    <meta name="“description”" conthent="”This" is my website” />
	  <meta charset=”utf-8”>
  </head>
<html>
```

description 태그와 title태그는

구글이 검색할때 찾는 태그이며 구글이 우리 사이트를 찾아줄때 비중이 크다. meta name의 값이 description이다. 

### link 태그 self-closing tag

```html
<link 
      rel="shortcut icon" #rel은 realative의 약자이다.
      sizes="16x16 32x32 64x64" #size는 설정을 안할수도있다.
      href="https://nomadcoders.co/m.png"
    />
```

head부분 안에 들어가는 내용이고 

![스크린샷 2022-05-05 오전 11.16.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/51aaaf27-38b9-4163-a11b-fc99ba4c8e00/스크린샷_2022-05-05_오전_11.16.43.png)

이렇게 페이지의 아이콘을 설정해준다. 

html이나 CSS 자바스트립등 웹프로그램의 관한 정보를 찾을때 검색어에 mdn을 붙이면 더 좋은 정보를 얻을수있다. mozila사이트에 들어가야한다.  

## more tags

 html이나 CSS 자바스트립등 웹프로그램의 관한 정보를 찾을때 검색어에 mdn을 붙이면 더 좋은 정보를 얻을수있다. mozila사이트에 들어가야한다.  

- meta tag = 부가적인 요소 라는 뜻 (content, name attribute를 가짐)
- charset = 한글 등 문자 표시하게 해줌
- language = 사이트에 사용되는 언어 표기 (검색엔진에게 알려줌)
- 다른 수많은 meta tag들이 있음
- HEAD 태그는 보이지 않는 사이트 설정들을 바꿔준다!! (중요)
- og:~~~ = 카카오톡에서 사용하는 정보들

## form 태그

```html
<form>
			<input type="file" accept=".imege/*" />
      <input required placeholder="firstname" type="text" />
      <input required placeholder="lastname" type="text" />
      <input required placeholder="username" type="text" />
      <input required placeholder="password" minlength="10" type="password" />
      <input type="submit" value="create account" />
    </form>
```

input은 하나 또는 여러개의 타입을 가질수있다.

placeholder는 input이 가지는 또 다른 attribute이다.  text박스안에 우리가 적은 글을 보여준다.

submit text박스에 입력한 데이터를 전송해준다.

value는 submit의 이름을 변경해주는 attribute이다. placeholder와 비슷한 역활을 한다. 

required는 text칸을 채우지 않고 submit을 눌렀을때 빈칸을 채우라고 말해주는 역활을 한다. 

minlength는 입력된 숫자값만큼 입력을해야지 submit을 누를수있게 해준다. (10자리 이상 비밀번호)

type=”file” 은 파일을 불러올수있는 버튼을 만들어준다. 뒤에 accept는 파일을 가져올때 허용하는 파일의 형식을 정의한다. 

```html
<tagename *attrname*="attrvalue">asdasdadad</tagename>
```

ㄴ 태그를 할때 형식

```html
label태그는 label의 for과 input의 id의 값이 같아야한다.

<label for="website">Website</label>
      <input id="website" type="email" required placeholder="Name" />
      <input type="submit" value="Create Account" />
```

label태그 input과 함께 사용해야한다. 

- id는 body 안에 어떤 태그에든 넣을 수 있는 attribute이다.
- id = unique identifier이기 때문이다. (고유식별자)
- element당 하나의 id만 가질 수 있는게 id의 규칙이다.

즉, id=”유일한 값" 이어야한다. 중복의 element가 하나의 id값을 동일하게 사용하면 안된다.

```html
<label for="website">Website</label>
      <input id="website" type="email" required placeholder="Name" />
      <input id="website" type="submit" value="Create Account" />
```

위와 같이 사용하면 규칙에 어긋남

css를 사용하게되면 css는 명령을 id를 통해서 하게된다. 

ex website라는 id를 가진 아이에게 파랑색으로 나타나게 해줘 이런느낌이다. 

## 올바른 위치에 올바른 코드를 입력하라

의미있는 태그와 의미 없는 태그가 있다. 

사용은 하지만 의미 없는 태그

div = division 박스 구분 

div는 다음칸으로 넘어가게해준다. 

즉 박스안에 넣어서 칸을 구분해주는 것이다. 

문서를 보기만해도 그 의미를 짐작할 수 있는 걸 semantic이라고 한다.

div와 똑같은 역활 header, page

```html
<body>
    <header>
      <h1>The Zion Time</h1>
    </header>
    <main>
      <p>hello nice to meet you!</p>
    </maim>
    <footer>
    &copy; 2020 Z.O
    </footer> #꼬릿말을 위한 태그
    </form>
  </body>
```

사실 모든 세매틱들은 div로 작성후 id를 통해 정의 해줄수있다. 하지만, 저렇게 컴퓨터가 알아듣는 이름을 통해 구분을 해주면 코드를 읽는 사람도 편하고 브라우저도 편하다. 

<soan></span> 짧은글은 span

<p></p> 긴글은 p

<adress></adress> 주소는 여기에 

즉, 사방팔방 div로 안하고 semantic태그를 사용하면 협업하는사람도 편하고 웹사이트도 편하다. 

## 정리

html은 태그로 이루어져있다. 

태그 이름을 아무렇게 짓는 걸 누구도 뭐라하지않는다. 하지만 브라우저가 이해하지 못한다. 

브라우저가 이해하게끔하려면 브라우저가 이해하는 언어 html을 써야한다. 

처음음 태그의 이름을 적고 괄호로 막아주는것이다. content(브라우저에 보여지는것)은 괄호 사이에 적는다. 

<p>

<mark>thing</mark>

</P>    p로 열면 p로 닫고 mark로 열면 mark로 닫는 것이다. 

attribute 는 태그 안에서 능력을 제공하는 것이다. 

**<tagname attrName=”value”>content</tagname> 작성하는 형식**

html에서는 항상 “”큰 따옴표를 사용한다.

어떠 태그든 id를 가질수있다. 내생각에는 id는 변수명인것같다. 

semantic태그를 잘사용하라.

















# CSS 추가 학습

어떻게 하면 css를 html페이지에 추가할수 있는지를 이해하라

두가지 방법이 있다.

1. 같은 html파일에 html코드와 css코드를 놓는 방법
2. css와 html을 분리 시키는것 (전문가들이 사용하는 방법)

 

일단 1번 방법을 사용한다.

head안에 <style> 이안에 css 문법을 적으면 된다. </style>을 추가하면 된다.

body에 들어가면 안된다. 

2번 방법 같은 폴더에 css파일을 만든다. 

그뒤 link태그를 이용해서 두 파일을 연결한다. 

<link href=”파일명.css” rel=”stylesheet” /> 이파일의 관계는 stylesheet라고 명시하는것이다. 

둘중 더 좋은 방법은 2번 방법이다 재활용이 가능하기 때문이다.

그리고 보기에도  더 좋다.

## 코드를 작성하자

3가지 규칙을 기억하자

1. css가 하는 일은 html태그를 가르키는 일이다. 

가르키는 것은 selector이라고 명령한다. 

```html
<style>
      h1 { color: yellowgreen;
        text-decoration: underline;
        font-size:50px;
        font-weight: 400; 
        font-style: italic;        
      }
    </style>
```

property(속성) > blueTItle은 파란색이고 글씨크기는 25px이고... 등등

자바처럼 {}중괄호를 열고 닫고 그안에 속성을 적어준다. 그리고 마지막엔 ;세미콜론을 해주어야한다. 

css속성 이름에는 띄어쓰기를 하지않는다 - 을 사용한다. 

위의 blueTitle처럼 아래에 저 태그가 있어야한다. 

속성을 다 외울 필요가 없고 그저 사용하는 방법만 알면 된다. 

속성이름 후 속성값 입력

## css의 의미

브라우저가 css코드를 읽을 때 위에 있는 코드부터 차례차례로 읽힌다는 것이다. 

box들로 디자인하는것이 css이다. (블록으로 나누는것들)

css에서 정말 중요한 요소이다. 

## Blocks and Inlines

가장 기본적인 박스 ⇒ div이다

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      div {
        height: 150px; #높이
        width: 150px; #넓이
        background-color: tomato;
      }
    </style>
  </head>

  <body></body>
</html>
```

span link 는 박스가 아니고

p(paragraph)옆에는 아무도 못온다. 한줄을 다 차지않다. 

2가지 형식

- box처럼 옆에 올수없다 (block) :옆에 아무것도 올수없다.
- 하나의 요소옆에 다른요소가 올수잇다.  (inline):같은 줄에 위치할수있다. (in the same line)

 
![](https://i.imgur.com/AQTFSIS.png)


옆에 이런형식으로 오는게 인라인이다. 

(inline에 해당하는것은 거의 별로 없다. 

대부분의 box들은 block이다. 

header도 마찬가지이다. 

block이 아닌것은 span a imege 들이다. 

bolck 은 옆에 아무것도 올수없지만 inline은 옆에 올수있다. 

안녕하세요 전느 백시온

## bolck만 가지고 있는 특징

block을 inline으로 inline을 block으로 변경 가능하다. 이와 같은 것이 display형식이다. 

브라우저는 기본적으로 inline것을 inline으로 생각하지만 우리가 display형식을 지정하면 그것이 변경된다. 

```html
display: inline;
```

**inline은 높이와 너비를 가질수없다.** 

block은 box이고 box는 엄청난 특징이 세가지가 있다.

- margin
- padding
- border

브라우저는 요소들에게 많은 style 속성을 준다. 원치 않아도 준다. 

![](https://i.imgur.com/70TWrFw.png)

margindms box의 border(경계)의 바깥에 있는 공간이다.

```html
body {
        margin-top: 20px;
        margin-bottom: 30px;
        margin-left: 5px;
        margin-right: 3px;
        background-attachment: skyblue;
        
      }

다른 방법
margin: 20px 15px;  #위아래는 20px이고 양쪽은 15px이다라고 말하는것
margin: 20px 5px 12px 9px; 위 오른쪽 아래 왼쪽이다. (시계방향)

```

이렇게 구역을 정의 내려줄수있다.

![](https://i.imgur.com/5ckl99o.png)

margin의 값이 하나면 사방에 다 적용된다는 것이고 두개의 값이면 위아래와 양쪽이다. margin의 값이 네개이면 순서대로 위 오른쪽 아래 왼쪽이다. 

## collapsing margins현상은 언제 일어나냐?

흰box의 경계가 보라색 box의 경계와 같을때 두box의 margin은 동일해진다.  위, 아래에서만 일어난다. 

이 현상이 일어나면 “아.. 경계가 닿아서 margin이 같아 졌나 보구나!”하면 된다. 

## padding개념

padding은 margin의 개념과 반대이다 .

margin은 box의 경계로부터 **‘바깥'**에 있는 공간이다. 

padding도 공간인데 box의 경계로부터 **‘안쪽’**있는 공간이다. 

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      html {
        background-color: tomato;
      }
      body {
        margin: 20px;
        padding: 20px;
        background-color: blue;
      }
      #first {
      }
      div {
        height: 150px;
        width: 150px;
        background-color: whitesmoke;
      }
    </style>
  </head>

  <body>
    <div id="first">
      <div id="second">
        <div id="third">
          <div id="fourth"></div>
        </div>
      </div>
    </div>
  </body>
</html>
```

div중에 id가 first인 div만 색상을 변경하고싶을때 

style박스에서 #first{} 샵 id명 중괄호를 치고 중괄호 안에 색깔을 지정해주면된다. 

#이 없으면 html의 요소를 불러온다. 즉 #은 id를 호출하는 방법

## border

box의 경계이다.

border에는 많은 속성이 있다 하지만 여러 종류의 border을 쓰진 않는다 거의 한종류만 사용한다. (다른 종류는 진짜 별로다)

border style mdn을 치면 많은 border의 종류를 볼수잇다. 

```html
border: 2px solid black;
```

작성방법은 border: 픽셀크기 스타일유형 색깔을 지정하고 세미콜론으로 닫아주면된다. 

모든 곳에 border를 다 적용하는 법은 

```html
* { border: 2px solid black;
}
```

이렇게 지정하면 모든 곳에 다 적용된다.

inline도 border를 가질수 있는가

inline에도 border를 적용시킬수있다. 만약 모든 곳에 border를 적용시키고 내가 원하는 한곳만 수정을 하고싶다면, 

```html
span { 
border-style: dotted; 
```

이렇게 볼더스타일: 스타일 타입을 적어주고 세미콜론으로 닫아주면 된다. 

## inline과 margin의 특성

inline은 높이와 너비가 없다 그래서 margin값을 넣어주면 위,아래 빼고 양옆으로 margin값이 입력되는것을 확인할수있지만, 위아래는 적용이 안된것을 볼수있다. 하지만, padding은 사방으로 다 가질수있다. 

즉inline을 margin값에 따라 위,아래도 적용하게 하려면 inline을 block형식으로 바꾸어 주어야한다. 

## classes

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      body {
        margin: 20px;
      }
      span {
        background-color: teal;
      }
    </style>
  </head>

  <body>
    <span>hello</span>
    <span>hello</span>
    <span>hello</span>
    <span>hello</span>
    <span>hello</span>
    <span>hello</span>
    <span>hello</span>
  </body>
</html>
```

많은 hello span형식들중 몇몇들만 특별한 속성을 지니게 해주고싶으면 어떻게 해야할까?

id로 하나하나 지정하는것이 아니라 class를 사용하면 복수로 지정해줄수있다. 

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      body {
        margin: 20px;
      }
      span {
        background-color: teal;
      }
      .tomato {
        background-color: tomato;
      }
    </style>
  </head>

  <body>
    <span>hello</span>
    <span class="tomato">hello</span>
    <span>hello</span>
    <span class="tomato">hello</span>
    <span>hello</span>
    <span class="tomato">hello</span>
    <span>hello</span>
  </body>
</html>
```

클래스를 부를때는 #이 아니라 .(점)을 사용한다. 온점은 클래스 명이라는 뜻이다. 

#tomato는 id=”tomato”      .tomato는 class=”tomato”

### id와 class의 차이

id는 한개에 하나만 가질수있지만, class는 여러개를 가질수있다. 

```html
<span class="tomato hello honey potato">hello</span>
```

위의 코드는 예시이다. 

## 배운내용

1. inline에서 padding과 margin이 어떻게 표현되는가.
2. css에서 class는 어떤 역활을하고 어떻게 사용하는가.

## display 속성

이전에 display를 통해서 inline과 block의 속성을 변경할수있다고 했다. 

하지만 div의 속성을 inline으로 바꾸면 바뀐 div는 높이와 너비를 가질수없었다.

### inline-block

inline-block은 block으로 인식하게 만든다. 즉, inline이지만, 너비와 높이를 가질수있고 또한 옆에 다른요소도 올수있다. margin도 가질수있다.

하지만, inline-block은 너무 고루하고 엄청많은 문제가 있다. 

default값으로 주어진 것에 문제가 있다. 

![](https://i.imgur.com/N102hgI.png)

사이사이에 우리가 만들지 않은 공백이 있다. 이유는 모른다. 

또 다른이유는 정해진 형식이 없다는 점이다. 

inline-block은 Responsive Design(반응형 디자인)을 지원하지 않는다. 즉, 창 크기가 달라지면 영향을 받는다. 

## flexbox

flexbox는 박스들을 어떤 곳이든 둘 수 있어서 좋다. 그리고 아주 유연하다. 

2d레이아웃에서 정말 잘 작동한다. 하지만 사용할때 3가지의 규칙이 있다. 

### 규칙

1. 자식 엘리먼트에는 어떤 것도 적지 말아야 된다는 것이다. 부모 엘리먼트에만 명시해야한다. 

div를 우리가 원하는 아무 곳에 움직이게 하려면 div의 부모격인 body에게 flex container로 만들면된다.

>> body의 display가 flex라고 명시 하면된다.(div의 부모를 display: flex로 만든다. 

>>>flex로 명시후 우리는 justify-content 로 요소를 중앙(center) 왼쪽(start) 오른쪽(end)으로 몰아놓을수있다. 

```html
body{
	margin: 20px;
	display: flex;
	justify-content: center;
	align-itmes: flex-end;
```

2. 주축(main axis)와 교차축(cross axis) 이다.

![](https://i.imgur.com/yaNIPgi.png)

이게 flexbox에서 기본적으로 축들이 가지는 모습이다. 

justify-content는 main axis(주축)에 적용되는 것이다. 

align-items라고 불리는 다른 프로퍼티는 cross axis(교차축)에 적용되는 것이다. 

align-itmes는 교차축에 있는 item들을 움직이게 한다. 

>기본적으로 교차축은 수직이다. (기본적이라는 말은 나중에 이 속성을 바꿀수있기 때문이다.)

height: 100vh; 여기에서 vh는 viewport height이고 viewport는 screen으로 이해해도 된다. 

100 screen height는 화면 높이의 100%를 말한다. 

### 지금까지 작성한 코드

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      body {
        display: flex;
        height: 100vh;
        margin: 20px;
        justify-content: center;
        align-items: center;
      }
      div {
        width: 50px;
        height: 50px;
        background-color: teal;
      }
    </style>
  </head>

  <body>
    <div></div>
    <div></div>
    <div></div>
  </body>
</html>
```

## 주축과 교차축을 변경하는법

flex-direction: column으로 설정하면 주축은 수직이 되고 교차축은 수평이 된다. 

flex-direction: row로 설정하면 기본설정과 동일한 옵션을 가진다. 

지금까지는 body를 부모로 지정했지만 만약에 div안에 글씨가 적혀있다면 글씨의 부모는 div이기때문에 div를 부모로 설정하면 div안에 있는 글씨들을 중앙으로 옮기거나 왼쪽, 오른쪽으로 옮길수있다. 

>> 원하는 만큼 flex 부모-자식 엘리먼트를 만들어 낼수있다. 중요한점은 display: flex;가 있어야 한다는 것이다. 

## wrap

![](https://i.imgur.com/M1EsTVJ.png)

화면을 이렇게 줄였을때 안에 있는 요소들도 줄어드는 것을 wrapping이라고 한다. 

**flex-wrap: nowrap;** 이렇게 명시하면 위에 보이는 것처럼 한줄에 다 집어 넣으려고 사이즈를 줄여서라도 집어넣을 것이고 

**flex-wrap: wrap;** 이렇게 명시하면 한줄에 들어가는만큼 최대한 집어넣고 그게 되지 않으면 다음 줄로 옮긴다. 

## reverse

기본옵션과 반대로 설정이 가능하다. 

flex-direction: column-reverse;

flex-direction: row-reverse;

flex-wrap: nowrap-reverse;

flex-wrap: wrap-reverse; 다 가능하다








# CSS심화 학습

배울 내용 

Anumation, Transformation, Transition 같은 것들에 대해서..

## Transition

어떤 상태에서 다른 상태로의 “변화"를 애니메이션으로 만드는 방법이다. 

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      a {
        color: white;
        background-color: tomato;
        text-decoration: none; #링크의 밑줄을 없애준다.
        padding: 3px 5px;
        border-radius: 5px;
				transition: background-color 10s ease-in-out; 
      }
      a:hover {
        color: tomato;
        background-color: wheat;
      }
    </style>
  </head>

  <body>
    <a href="#">Go Home</a>
  </body>
</html>
```

transition이라는 속성은 state가 없는 요소에 붙어야한다. 

즉, hover가 있는 쪽이 아니라 없는 쪽에 써야한다.

```html
transition: background-color 10s ease-in-out; 
```

transition을 적고 : 바꾸고싶은것을 적고 몇초동안 변경할지 적고  ease-in-out; 세미콜론으로 닫으면된다.

원하는경우 transtion을 더 추가해도 된다. 배경색 뿐만 아니라 글씨색도 transition을 줄수있다. 

```html
transition: background-color 1s ease-in-out, color 5s ease-in-out;
```

쉼표를 사용해서 더 추가해주었다. 

### 기억할것

transtion이 작동되는 이유는 a:hover가 작동하기 때문에 작동되는것이다. 

transition이 hover에 있는 background-color를 찾고 background-color가 hover일때 달라져있으면 그변화를 애니메이션으로 바꾸는 것이다. 

그렇다면 우리는 코드를 이렇게 작성할수있다.

```html
transition: all 2s ease-in-out;
```

이렇게 작성한다면 변화하는 모든것에 효과를 줄수있다. 

## ease-in-out;

기본적으로 브라우저에게 애니메이션이 어떻게 변할지 말해주는 것이다.

ease-in-out말고도 많은 효과들이있다.

디폴트로 갖고있는 것은 linear, ease-in, ease-out, ease, ease-in-out이다 

cubic-bezier()을 통해서도 우리가 직접 커스터마이즈 할수있다. 

```html
transition: all 2s cubic-bezier(0.250, 0.250, 0.750, 0.750);
```

[https://matthewlein.com/tools/ceaser](https://matthewlein.com/tools/ceaser) 사이트에서 효과를 확인해보자

## transformation

한 요소를 말 그대로 변형시킬수 있기 때문에 개쩐다

css로 3D까지 할수 있기 때문에 cool한것임

transform 안에 엄청나게 많은 기능들이 있다

transformation은 box element를 변형시키지 않는다.

즉, 옆에 sibling들에게 영향을 끼치지 않는다.

margin, padding이 적용되지 않는다. 일종의 3D transformation이기 때문이다.

margin이나 padding을 주기위해서 tarnslateX, trnasLateY 를 사용하는것이 아니다!

다른 요소의 box를 변형시키지 않고 원하는 요소를 이동시키기 위해서 사용하는 것이다.

trransformation 은 페이지의 픽셀의 다른 부분에서 일어난다.

transformatino은 box차원에서 일어나지 않는다.

tronsformation 을 결합 가능하다! (transition과 hover로 효과를 주었다. 

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      img {
        border: 10px solid black;
        border-radius: 50%;
        transition: transform 5s ease-in-out;
      }
      img:hover {
        transform: rotate(90deg);
      }
    </style>
  </head>

  <body>
    <img src="KakaoTalk_Photo_2017-10-23-18-34-52.jpeg" />
  </body>
</html>
```

transformation을 중복으로 사용할수도있다. 콤마를 사용하지 않아도 된다. 

```html
img:hover {
        transform: rotate(90deg) scale(0.5);
```

CSS의 3D는 GPU로 돌아간다 즉 3D작업을 할 수 있다

transformation 은 이것 역시 엄청나게 많은 document가 있다 확인해서 combine할 수 있다

transition 과 transformation 을 합친다면 아름다운 애니매이션을 만들 수 있다

## ANIMATIONS

지금까지 우리는 우리가 마우스를 올리면 움직이는 애니메이션을 배웠다. 하지만 이제 자기혼자 작동하는 애니메이션을 구동하려면 어떻게 해야할까?

만드는 방법은 두가지가 있다 

## 첫번째

COIN FLIP이라 부르는 애니메이션을 만들어보자.

먼저 변수를 선언하듯 애니메이션을 선언해야한다. 

```html
@keyframes superCoinFlip{}
```

@ 이가 꼭 있어야 한다

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      @keyframes superCoinFlip {
        form {
          transform: rotateX(0);
        }
        to {
          transform: rotateX(360deg);
        }
      }
      img {
        border: 10px solid black;
        border-radius: 50;
        animation: superCoinFlip 3s ease-in-out;
      }
    </style>
  </head>

  <body>
    <img src="KakaoTalk_Photo_2017-10-23-18-34-52.jpeg" />
  </body>
</html>
```

코드를 보면 애니메이션 명을 지정후 그후 괄호안에 form과 to로 처음 상태에서 마지막 상태로 움직여줘 라고 말하는것이다. 그리고 img에서 animation을 작동시키는것이다. 

```html
  animation: superCoinFlip 3s ease-in-out infinite;
```

추가로 infinite를 추가해서 무한하게 반복 시킬수있다. 

## 두번째

```html
<!DOCTYPE html>
<html>
  <head lang="kr">
    <title>The Zion Times</title>
    <style>
      @keyframes superCoinFlip {
        0% {
          transform: rotatex(0);
        }
        50% {
          transform: rotateY(180deg) translateX(-100px);
        }
        100% {
          transform: rotateX(0);
        }
      }
      img {
        width: 200px;
        height: 200px;
        border: 10px solid black;
        border-radius: 50;
        animation: superCoinFlip 3s ease-in-out infinite;
      }
    </style>
  </head>

  <body>
    <img src="KakaoTalk_Photo_2017-10-23-18-34-52.jpeg" />
  </body>
</html>
```

한바퀴를 돌았다가 다시 돌아오게 하려면 이렇게 3단계로 구분을해서 코드를 작성하면 된다. 

## Media query

Media query는 오직 CSS만을 이용해서  나의 웹사이트를 보고 있는 사용자의 스크린 사이즈를 알 수 있는 방법이다. 가끔 CSS style을 바꾸고 싶을 때가 있을것이다. 누군가가 나의 웹사이트를 아이폰으로 본다면?,혹은 아주 큰 화면으로 본다면? 혹은 누군가가 landscape모드(가로모드)로 본다면? 아니면 portrait모드(세로모드)로 본다면? 오직 CSS만으로 이 모든 것을 감지할 수 있다.  

따라서 Media query는 브라우저에게 이렇게 말한다. 핸드폰이나 스크린사이즈가 이정도 크기라면 이 css를 보여줘

```html
@media screen and(max-width:700px) {
        div {
          background-color: tomato;
        }
      }
```

이 코드의 의미는 사용자의 스크린의 너비가 600px보다 작다면 div의 배경색을 토마토색으로 해달라는 뜻이다.

```html
@media screen and (min-width: 700px) and (max-width: 1000px) {
        div {
          background-color: tomato;
        }
      }
```

이렇게 코드를 작성하면 700~1000사이 픽셀에서만 div의 배경색을 변경해달라는 의미이다. 

```html
@media screen and (max-width: 1000px) {
        div {
          background-color: wheat;
        }
      }
      @media screen and (min-width: 1000px) and (max-width: 1500px) {
        div {
          background-color: tomato;
        }
      }
      @media screen and (min-width: 1500px) {
        div {
          background-color: black;
        }
      }
```

이렇게 끊김없이 색을 지정해서 여러개 만들수도있다. 

```html
@media screen and (min-width: 1000px) and (max-width: 1500px) and (orientation:landscape){
        div {
          background-color: tomato;
        }
      }
```

orientation으로 가로모드일때와 세로모드일때 구분해서 옵션을 지정해줄수있다. 

**orientation: landscape 또는 portrait** 

## 정리

media query는 우리가 조건을 추가할 수 있는 방법이다. 코드의 조건을 적는다! 이조건이 참이라면 이 css를 실행하라는 조건을 말한다. 

### max-device-width , min-device-width

이것을 오직 모바일에서만 적용되는 코드이다.

## Media Queries 주요기능

- min-device-width
- max-device-width
- orientation: landscape
- orientation: portrait
- aspect-ration - 레티나디스플레이 감지가능
- display-mode
- inverted-colors
- lightlevel
- prefers-contrast
- resolution
- monochrome

Media type

@media screen{}

@media print{}

