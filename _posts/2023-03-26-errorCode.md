---
layout: single
title:  "Error Message"
categories: Blog
excerpt: "자주 발생하는 에러들을 정리했어요"
tags: [Java, blog, error]
toc: true
toc_sticky: true
toc_label : 목차
toc_icon: "fas fa-tasks"
author_profile: false
sidebar:
nav: "docs"
---
[Google](https://google.com){: .btn .btn--warning}


# Error

<hr/>

## symbol 

```java

	cannot find symbol
	cannot resolve symbol
	지정된변수나 메서드를 찾을 수 없다는 의미입니다.
	이 에러는 선언되지 않은 변수나 메서드를 사용하거나,
	변수, 메서드의 이름을 잘못 사용한 경우에 발생합니다.
	
	
```
## ':' expected

```java

	; experted는 ;이 필요한 곳에 없다는 의미입니다.
	자바의 모든 문장의 끝에는 ;을 붙여줘야 합니다.

	
```	

## main

```java

	Exception in thread "main" java.lang.NoSuchMethodEroor: main
	main 메서드를 찾을 수 없다는 의미입니다.
	main 메서드가 없거나, 선언부에 오타가 존재하는 경우에 발생합니다.


```		

## class

```java

	Exception in thread "main" java.lang.NoClassDefFoundError: (?)
	(클래스명)을 찾을 수 없다는 의미입니다. 클래스의 철자, 대소문자 여부를 확인합니다.
	클래스파일이 잘 생성되었는지 확인합니다.
	.java가 정상적으로 컴파일 되었다면 class 파일도 있어야합니다.
	전부 문제가 없다면 classpath 설정이 바르게 되었는지 확인합니다.


```

## 문법 오류

```java
	
	illegal start of expression
	문장에 문법적인 오류가 있다는 의미입니다.
	괄호 ()나 {}를 열고 닫음이 확실치 않거나,
	수식이나 if, for문 등에 문법적 오류가 있을 때 발생합니다.
	또한 public이나 static같은 키워드를 잘못 입력한 경우에도 발생합니다.

	class, interface, enum expected
	3가지가 없다는 의미지만 보통 괄호 {}의 갯수가 맞지 않는 경우에 발생합니다.


```

