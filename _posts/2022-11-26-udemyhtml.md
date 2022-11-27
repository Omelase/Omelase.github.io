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


### 제목 element

`<h1>`은 반드시 한 페이지 당 하나만 있어야 하고,  
가장 최상위 제목이어야 한다.  

`<h1>`이 있어야 `<h2>`를 쓸 수 있고 그 아래 제목에도 마찬가지로 적용되는 계층적 구조를 보인다.

### HTML 구조 (skeleton)

HTML 상용구 (boilerplate)라고도 부르며  
모든 HTML 문서에 들어가야 하는 표준화된 마크업이다.  
상용구없이도 browser에서 보여주지만 꼭 갖춰야 함.  

`<!DOCTYPE html>` : HTML5를 사용하고 있음을 표시. 닫는 tag없음.  

`<html></html>` : root element라고 불림. 문서의 최상위 element이다.

- `<head></head>` : meta data element라고도 불림.   페이지 상에 보이지않는 내용을 담고 있다.  
    CSS에서 style 속성을 입력하는 공간.  
    CSS 외에도 Javascript, font, icon 등이 들어간다.  

    - `<title></title>` : browser의 tab에 문서의 이름을 출력한다.  `<head>`안에 씀.  
- `<body></body>` : 문서의 모든 내용을 담고 있는 element

