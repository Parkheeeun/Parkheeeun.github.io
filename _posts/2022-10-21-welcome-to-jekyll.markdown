---
title: 마크다운 (Markdown)
layout: post
post-image: "https://velog.velcdn.com/images/i_am_heeeun/post/1073ac03-c02a-4594-8462-5cc008b7c02a/image.png"
description: Markdown
tags:
- SQL
- DATABASE
---

회사에서 SQL를 주제로 하여 각자 공부한 것을 velog에 올려 발표와 피드백을 통해 함께 성장하는 것을 목표로 하는 스터디를 하기로 하였다. 우선 그 첫 번째로 velog에서 사용하 는 마크다운에 대해 공부해보도록하자.
## 마크다운(Markdown)이란?
> 일반텍스트기반의 경량 마크업언어이다. 일반 텍스트로 서식이 있는 문서를 작성하는데 사용되며, 일반 마크업 언어에 비해 문법이 쉽고 간단한 것이 특징이다. HTML과 리치텍스트(RTF)등 서식문서로 쉽게 변환되기 때문에 응용소프트웨어와 함께 배포되는 README파일이나 온라인 게시물 등에 많이 사용된다.

## 마크다운의 역사에 대해 알아보자
> 2004년 존그루버와 에런스워츠가 함께 마크다운 언어를 만들었으며 사람들이 읽기 쉽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있으면서 구조적으로 유효한 XHTML로 선택적 변환이 가능하게 하는 것을 목표로 하고있으며 파일확장자는 .md이다

## 마크다운의 장점과 단점
> #### 장점
- 관리가 쉽다.
- 별도의 도구없이 사용가능하다.
- 텍스트로 저장되기 때문에 용량이 적어 보관이 용이하다.
- 문법이 쉽고 간결하다.


> #### 단점
- 표준이 없다. 
- 표현하는 도구에 따라서 동작하지 않거나, 다르게 표현 될 수있다.
- 모든 HTML마크업을 대신하지 못한다.

## 문법(Syntax)
### 제목(Header)
'#'의 개수를 1~6개까지 사용할수있다. 이는 h1부터 h6까지를 의미한다.
👉🏻**입력**
```
# Header (h1)
## Header (h2)
### Header (h3)
#### Header (h4)
##### Header (h5)
###### Header (h6)

다음과 같이 쓸 수도있다.
Header(h1)
=========

Header(h2)
------------
```
💻 출력
>
# heeeun(h1)
## heeeun(h2)
### heeeun(h3)
#### heeeun(h4)
##### heeeun(h5)
heeeun
======
heeeun
--------

---------------------------------------------------------
### 목록(List)
순서가 있는 목록과 순서가 없는 목록으로 나눠져있다.
```-```, ```*```, ```+```는 순서가 없는 목록을 나타내는데 사용되고
```1.``` ```2.``` ```3.```은 순서가 있는 목록을 나타내는데 사용된다.
👉입력
```
-순서x
*순서x
+순서x
 
1. 순서o
	1.2 순서o
    1.3 순서o
2. 순서o
	2.1 순서o
    2.2 순서o

```

💻출력
>
-	순서x
-	순서x
	+ 순서x
    + 순서x
1. 순서O
3. 순서O
2. 순서O

---------------------------------------------------------
### 글자모양(Font)
👉🏻입력
```
볼드체: **Bold** or __Bold__
이탤릭체: *Italic* or _Italic_
취소선: ~~cancle~~
```
💻출력
>
볼드체: **i_am_heeeun**
이탤릭체: *i_am_heeeun*
취소선: ~~i_am_heeeun~~



---------------------------------------------------------
### 코드(Code)
코드를 작성할 수있는 방법은 총 두가지가 있다.
첫번째 방법으로 한줄짜리 코드는 Tab을 이용해 작성할수있다. 다만 그 전 문장에서 Enter를 두번 입력해야한다.

	한줄짜리 코드는 전 문장에서 Enter key 2번후 Tab키 사용해 입력.
여러줄의 코드는 백틱(`)을 위아래로 3개씩 입력한 후 작성해야한다.
```
여러줄의 코드는 
백틱(`) 위 아래로 3개씩
감싼 후 작성해야함.
이때 코드블럭 시작점에 사용하는 언어를 선언하면 Syntax Highlighting이 가능하다.
```
또 두번째 방법으로는 ```<pre><code>코드</code></pre>```를 사용해 작성할 수 있다.
👉🏻입력 ver.1
```
```java
public class helloWorld{
	public void main(String[] args){
    	System.out.println("Hello World~!");
    }
}```
```

💻출력 ver.1
```java
public class helloWorld{
	public void main(String[] args){
    	System.out.println("Hello World~!");
    }
}

```
👉입력 ver.2
```
<pre>
<code>
	코드
</code>
</pre>
```
💻출력 ver.2
<pre>
<code>
public class helloWorld{
	public void main(String[] args){
    	System.out.println("Hello World~!");
    }
}
</code>
</pre>
---------------------------------------------------------
### 인용문(Quote)
인용문구를 사용하고자하면 ```>```기호를 사용한다. 중첩사용이 가능하다.
👉🏻입력
```
> # 1
화이팅~!
화이팅~!!!
>> ## 2
중첩사용가능
중첩사용가능
>>> ### 3
계속 중첩가능~!
```

💻출력
> # 1
화이팅~!
화이팅~!!
>> ## 2
중첩사용가능
중첩사용가능
>>> ### 3
계속 중첩가능~!

---------------------------------------------------------
### 체크박스(Checkbox)
```-```,```+```,```*```뒤에 띄어쓰기 한 후 대괄호를 넣으면 체크박스가 생성된다.
대괄호안에 x를 입력하면 체크된 상태의 체크박스가 생성된다.
👉🏻입력
```
 - [ ] :빈 체크박스 생성
 + [ ] :빈 체크박스 생성
 * [x] :체크된 체크박스 생성
```
💻출력
- [ ] 
- [x] 
---------------------------------------------------------
### 테이블(Table)
-	```|``` 기호로 열을 구분
- ```-``` 기호로 행을 구분 
- ```:``` 기호로 정렬이 가능하다

💻출력

|    |col1 |col2|col3
|----|:----|:----:|----:
|row|1.1   |  1.2  |   1.3
|row|2.1   |  2.2  |   2.3
|row|3.1   |  3.2  |   3.3

---------------------------------------------------------
### 링크(Link)
총 3가지의 방법으로 링크를 나타낼 수 있다.
- Inline Link
-  Url Link
- 참조 Link

👉입력
```
1.Inline Link
[heehee.log](https://velog.io/@i_am_heeeun)

2. Url Link
<https://velog.io/@i_am_heeeun>

3. 참조 Link
[heehee.log]:https://velog.io/@i_am_heeeun
[heehee.log]
```
💻출력
>
1. Inline Link
[heehee.log](https://velog.io/@i_am_heeeun)

>2. Url Link
<https://velog.io/@i_am_heeeun>


[heehee.log]:https://velog.io/@i_am_heeeun
>3. 참조 Link
[heehee.log]

---------------------------------------------------------
### 이미지,사진삽입(Image)
링크앞에 ```!``` 를 붙여주면 이미지,사진을 삽입할 수있다. 이미지 크기는 HTML코드를 사용해 조절이 가능하다.
👉입력
```
![Profile](https://velog.velcdn.com/images/i_am_heeeun/post/3d3651b4-c33a-4bad-a2db-8d623e1f9fe3/image.png)
)

-이미지 사이즈 조절
<img src="" width="" height=""></img>
```
💻출력
<img src="https://velog.velcdn.com/images/i_am_heeeun/post/3d3651b4-c33a-4bad-a2db-8d623e1f9fe3/image.png" width="300px" height="150px"></img>

------------
출처: [위키백과](https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4) [나무위키](https://namu.wiki/w/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)
참고사이트: https://gist.github.com/ihoneymon/652be052a0727ad59601






