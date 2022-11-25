---
layout: post
title: Semantic tag
categories: 컴퓨터기초
tags: [ncloud, html, basic]
---

## 시맨틱 태그 (Semantic Tag)란?

Semantic은 '의미의', '의미론적인'이라는 뜻을 가진 형용사이다. 따라서 시맨틱 태그란 의미가 있는 태그를 말한다.  
  
div나 span과 같이 의미가 없는 태그는 태그 이름만 보고는 어떤 내용인지 전혀 유추할 수가 없는 반면, form, table, article 등 의미가 있는 태그는 내용을 명확하게 정의한다.  
  
시맨틱 태그는 HTML5에서 처음 등장한 태그들이다.  

![five](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F99D4353D5A90D2131B)

![div](https://velog.velcdn.com/images%2Fgil0127%2Fpost%2Fb3a97fa2-7cad-4c27-8011-d78f707f43b0%2F1111111.PNG)

기존에도 div에 class 값을 붙여 스타일링하면 모든 작업이 가능했지만 개발자들은 모든 것을 div로 작성하는 것보다 효율적인 방법을 원했고 어느 부분이 제목이고 어느 부분이 내용인지 한 눈에 이해할 수 있게끔 의미를 가지는 태그가 개발되었다.  

## 시맨틱 태그를 사용해야하는 이유

- 검색엔진최적화 (SEO) : 검색엔진은 태그를 기반으로 페이지 내 검색 키워드의 우선순위를 판단한다. 따라서 제목은 h1, 중요한 단어는 strong 또는 em을 사용하는 등 의미에 맞는 올바른 태그르 사용하는 것이 중요하다.
- 웹 접근성 : 시각장애가 있는 사용자가 스크린 리더를 사용하여 페이지를 탐색할 때 도움이 된다.
- 유지보수성 : 시맨틱 태그를 사용한 코드 블록을 찾는 것은 끝없는 div(div > div > div ...)를 탐색하는 것보다 훨씬 쉽다.
- W3C에 따르면 "시맨틱 웹을 사용하면 애플리케이션, 기업 및 커뮤니티에서 데이터를 공유하고 재사용할 수 있다"고 한다. (의미가 있는 요소는 개발자 모두에게 명확한 의미를 전달한다)


## 시맨틱 태그를 정하는 팁, 유의사항
- 사용할 태그를 결정하기전 "채울 데이터를 가장 잘 설명하고 나타내는 요소는 무엇일지?" 먼저 자문해 본다.
- 사용할 HTML은 태그는 스타일 기반이 아닌 채워질 데이터를 기반으로 결정되어야 한다. (예를들어 블로그 글 제목 스타일이 p태그를 사용하는 단락과 같은 디자인이더라도, p가 아닌 h1을 사용해야한다.)
- 어떤 모양으로 보여야 하는지는 전적으로 CSS의 책임이다. (이부분 헷갈리지 말자!)

![tag](https://velog.velcdn.com/images%2Fgil0127%2Fpost%2Fdc349d83-4e31-421e-a463-4f23466b4e51%2F3.PNG)

## 시맨틱 태그의 종류

### 1. header

- 페이지의 제목과 같은 소개 내용을 포함한다.
- 일반적으로 heading 태그나 로고 또는 아이콘, 저작권 정보, 검색 양식, 작성자 이름 등을 포함한다.


### 2. main

- 지배적인 콘텐츠 영역을 나타내는 태그이다.
- 페이지에서 중요한 콘텐츠는 main 태그 안에 넣자.


### 3. footer

- 일반적으로 section의 작성자에 대한 정보, 저작권 데이터 또는 관련 문서에 대한 링크를 포함한다.
- 필수는 아니지만, 페이지 맨 아래에 부가적인 정보나 링크가 들어 있다면, 사용하자.


### 4. nav

- 보통 메뉴, 목차 등에 사용된다.
- header 안에 여러가지 메뉴들이 모여 있다면, div로 나누지 말고 nav 태그를 사용하자.


### 5. section

- 구체적인 시맨틱 태그가 없는 문서의 독립적인 영역을 나타낸다.
- section에는 매우 소수의 예외를 제외하고 항상 제목이 있는 것이 일반적이다.
- aticle 안이나 main 안에서 연관 있는 내용들을 묶어줄 때 사용하자.

![section](https://velog.velcdn.com/images%2Fgil0127%2Fpost%2F5f9f58c5-1aac-439e-9519-9b9c43591a12%2F2.PNG)


### 6. article

- 그 자체로 의미가 있는 웹사이트의 부분이며, 독립적으로 배포 또는 재사용되도록 의도 된 문서이다.
- 게시물, 잡지 또는 신문 기사, 블로그 작성글, 제품 카드, 사용자가 제출한 댓글, 대화형 위젯 등이 있다.
- main 안에 있는 내용들과 연관 없이 독립적인 내용을 나타낼 때 사용하자.

![article](https://velog.velcdn.com/images%2Fgil0127%2Fpost%2F636212d7-b911-4d7e-a0c5-48aa3df8e42a%2F1.PNG)



### 7. aside

- 간접적으로 문서와 관련된 내용을 나타낸다.
- 사이드바 또는 콜아웃 상자로 사용된다.
- main 안에서도 콘텐츠와 직접적인 연관이 없는 내용들을 넣자.