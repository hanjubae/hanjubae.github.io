---
layout: post
title: JQuery 배운 것 정리(2)
date: 2017-01-12
---



## JQuery와 CSS를 활용한 DocumentObjectModel (DOM)



### DOM이란?

Script가 동적으로 Content에 접근하고 업데이트 또는
조작할 수 있는 Interface

- $("seletor").html()
> 셀렉터태그내에 존재하는 자식태그를 통째로 읽어올 때 사용되는 함수
 ※태그 동적추가할 때 주로 사용되는 함수
- $("selector").text()
> 셀렉터태그내에 존재하는 자식태그들 중에 html태그는 모두 제외 한 채 문자열만 출력하고자 할때 사용되는 함수
 ※html태그까지 모두 문자로 인식시켜주는 함수
- $("selector").html()
> INPUT 태그에 정의된 value속성의 값을 확인하고자 할 때 사용되는 함수

---

##### [index.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/index.html)
##### [index2.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/index2.html)
##### [index3.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/index3.html)

### HTML attribute 속성 제어

attribut값을 불러오고나 조정

##### [index1.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/index1.html)
##### [attr.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/attr.html)

### CSS Property 제어
##### [CSSgetset.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/CSSgetset.html)
##### [CSSProperty.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/CSSProperty.html)


### DOM을 활용한 추가 /삭제

##### [append.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/append.html)
##### [beforeAfter.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/beforeAfter.html)
##### [prepend.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/prepend.html)
##### [remove.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/remove.html)

### 비동기통신(Ajax)맛보기

### [load.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/load.html)

***
***
***


# 헤더 h1

## 헤더 h2

### 헤더 h3

#### 헤더 h4

##### 헤더 h5

###### 헤더 h6

일반

개행
개행

개행 
개행

개행  
개행

개행   
개행

문장

문장

**볼드**

__볼드__

*이탤릭*

_이탤릭_

**_볼드이탤릭_**

*__볼드이탤릭__*

__*볼드이탤릭*__

_**볼드이탤릭**_

++밑줄++

~~취소선~~

==하이라이트==

^윗첨자^

~아래첨자~


![이미지대체텍스트](이미지주소 "툴팁텍스트생략가능")

[링크텍스트](링크주소)

[참조링크텍스트][참조id]

[참조id]: 링크주소 "툴팁텍스트생략가능"

각주텍스트[^각주id]

[^각주id]: 각주내용


- 순서 없는 목록

- - 순서 없는 목록

- - - 순서 없는 목록

- - 순서 없는 목록

- 순서 없는 목록

- 순서 없는 목록

+ 순서 없는 목록

+ 순서 없는 목록

+ 순서 없는 목록


* 순서 없는 목록

* 순서 없는 목록

* 순서 없는 목록


1. 순서 있는 목록

2. 순서 있는 목록

3. 순서 있는 목록


- [x] task list 1

- [ ] task list 2

- [x] task list 3


정의 목록 용어
: 서술

정의목록
: 서술

: 서술


인라인 `코드` 텍스트

```
블럭 코드
```


|테이블헤드th|테이블헤드th|테이블헤드th|
|---:|:---|:---:|
|row1|row1|row1|
|row2|row2|row2|


> 인용문
> > 인용문
>
> 인용문


가로줄

***

가로줄

---

가로줄

___

가로줄



## Subject

Content

- List

> Quote

|	Head	|	Head	|	Head	|
|:---:|:---:|:---:|
|	Cell	|	Cell	|	Cell	|
|	Cell	|	Cell	|	Cell	|


### Syntax

````````````````````````````````````````````````````````````````````````````````java
Code
````````````````````````````````````````````````````````````````````````````````


### Link

- [Java Tutorial Link](http)

- [Java Language Specification Link](http)

- [Java API Specification Link](http)

- [Wikipedia Link](http)

- [위키백과 Link](http)


### Image

- ![Image](http)

## dom

### [index10.html](https://github.com/hanjubae/sist/blob/master/_07jquery/DocumentOBjectModel/WebContent/index10.html)



## Exercise


### [Day03_02Oracle_Exercise0.java](https://github.com/magoon85/sist/blob/master/_02oracle/src/sist/_02oracle/day03/Day03_02Oracle_Exercise0_Oracle0.java)



## Practice


### [Day03_02Oracle_Practice0.java](https://github.com/magoon85/sist/blob/master/_02oracle/src/sist/_02oracle/day03/Day03_02Oracle_Practice0.java)


