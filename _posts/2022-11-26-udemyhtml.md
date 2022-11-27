---
layout: post
title: HTML
categories: 컴퓨터기초
tags: [network, html, basic]
---

## HTML

Hyper-Text Markup Language  
  
HTML은 완전한 프로그래밍 언어가 아니다.  

단지 문서에 markup을 할 뿐이다.  

markup이란 문서의 원래 콘텐츠에 부수적인 정보를 추가하는 것을 말한다.  
ex) 마킹, 메모, 주석, 밑줄

[tag목록](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

**tag와 element**

```
<p>content</p>
```

tag : `<p>`, `</p>`  
  
element : `<p>content</p>` tag와 content를 의미  

`<p>` tag를 적용한 style이라는 말은 엄밀히 말해 틀린 것.  
p element에 적용한 style이라는 말이 옳다.  


### 단락 element

`<p>`는 문단의 시작과 끝에 붙어 단락을 만든다. paragraph의 약어

`<br>`은 줄바꿈 용도이고 닫기 tag가 없다. break의 약어

### 제목 element

`<h1>`은 반드시 한 페이지 당 하나만 있어야 하고,  
가장 최상위 제목이어야 한다.  

`<h1>`이 있어야 `<h2>`를 쓸 수 있고 그 아래 제목에도 마찬가지로 적용되는 계층적 구조를 보인다.

### HTML 구조 (skeleton)

HTML 상용구 (boilerplate)라고도 부르며  
모든 HTML 문서에 들어가야 하는 표준화된 마크업이다.  
상용구없이도 browser에서 보여주지만 꼭 갖춰야 함.  

`<!DOCTYPE html>` : HTML5를 사용하고 있음을 표시. 닫기 tag없음.  

`<html></html>` : root element라고 불림. 문서의 최상위 element이다.

- `<head></head>` : meta data element라고도 불림.   페이지 상에 보이지않는 내용을 담고 있다.  
    CSS에서 style 속성을 입력하는 공간.  
    CSS 외에도 Javascript, font, icon 등이 들어간다.  

    - `<title></title>` : browser의 tab에 문서의 이름을 출력한다.  `<head>`안에 씀.  
- `<body></body>` : 문서의 모든 내용을 담고 있는 element

### 목록 element

```
<ul>
    <li></li>
    <li>
        <ol>
            <li></li>
            <li></li>
        </ol>
    </li>
    <li><b></b></li>
</ul>
```
순서가 없는 목록
  
```
<ol>
    <li></li>
    <li>
        <ul>
            <li></li>
            <li></li>
        </ul>
    </li>
    <li><b></b></li>
</ol>
```
순서가 있는 목록
  
  
`<li>`안에 중첩목록을 넣거나 이탤릭체 등 다른 tag를 넣을 수 있다.  

### anchor element

`<a></a>` : hyper-link 생성  
- `href`속성 : hyper-text reference. 웹페이지를 연결하려면 속성값에 HTTP 프로토콜을 사용해야 함.   http 안 쓰면 파일 프로토콜로 인식.  

### image element

`<img>` : 이미지를 삽입. 닫기 tag가 없다.  
- src 속성 : source. 속성값에 이미지 경로를 입력.  
- alt 속성 : alternate. 속성값에 이미지 설명 입력.  

## HTML5

HTML을 정의하는 가장 발전된 표준.  

[HTML의 작동 방식](html.spec.whatwg.org)

### inline element와 block element

- inline element
: 페이지에서 contents가 있는 영역만 차지함  
ex) `<a>`, `<img>`  

- block element
: 페이지에서 1줄을 혼자 다 차지함  
ex) `<hn>`, `<>`

### generic element

`<div></div>` : division. 다른 element를 그룹화하는 generic container. block element임. 이를 이용해 inline element들을 묶어 block화시킬 수 있다.  

`<span></span>` : span. 다른 element를 그룹화하는 generic container. inline element임. 주로 class 속성을 이용해 문장 중에서 특정 단어를 꾸미고 싶을 때 사용한다.  

### 기타 element

`<hr>` : horizontal rule. 수평선을 만든다. 닫기 tag가 없다.

`<sup></sup>` : 윗첨자.  

`<sub></sub>` : 아래첨자.  

### entity code

HTML 대신 쓸 수 있는 특별한 코드 또는 시퀀스  

타이핑이 어려운 특수문자 등을 표기할 때 쓴다.  

모든 entity code는 &로 시작해서 ;로 끝난다.  

흔하게 사용되는건 예약어이다.  

HTML에 입력하면 에러가 뜨는 글자들이 몇 개있는데 HTML 구문에서 중요한 역할을 하기 때문이다.  

따라서, HTML에서 예약어를 표기하기 위해서는 entity code를 대신 쓴다.  

모든 entity code는 entity name 와 entity number가 있는데 어느 걸 쓰든 상관없다.  

ex) `&hearts;`, `&lt;`, `&#8804;`




