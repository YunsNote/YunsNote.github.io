---
layout: single
title:  "암기 내용"
categories: Blog
excerpt: "제가 암기해두면 좋을만한 공식과 개념을 정리중입니다."
tags: [Java, blog, memorization]
toc: true
toc_sticky: true
toc_label : 목차
toc_icon: "fas fa-tasks"
author_profile: false
sidebar:
nav: "docs"
---
[Google](https://google.com){: .btn .btn--warning}


	이 글은 작성하는 지금까지 공부한 내용을 정리한 내용입니다.
	추후 열심히 공부해서 추가 글을 작성하도록 하겠습니다.

# 유형별 사용하면 좋을 함수

***

## 출력함수 

```java

	public static void main(String[] args) {
		
		1. System.out.println() : 문자열, 정수, 실수 등의 데이터 타입을 출력할 수 있습니다. 출력 후 자동으로 개행 처리가 됩니다.

		2. System.out.print() : println()과 비슷하지만 개행 처리를 하지 않고 출력합니다.

		3. System.out.printf() : %d, %s, %f, %c등을 활용하여 출력할 수 있습니다.
		%(x)의 사용 목적 -
	 		%d : decimal 정수를 10진수 형태로 표현하며, int를 주로 사용합니다.
	 		%f : floating number 실수를 표현하며, float 혹은 double 에 사용합니다,.
			%c : character 한 문자를 표현하며 char에 대해 사용합니다.
			%s : string 문자열을 표현하며 String에 대해 사용합니다.

		4. System.out.format() : printf()와 기능이 동일하지만 출력 결과를 문자열로 반환하는 것이 특징입니다.
	
	}

```
## 수학 함수

```java

	public static void main(String[] args) {
		
		1. Math.abs() : 절대값을 구하는 함수입니다.
		값과 변수를 넣어 절대값을 구할 수 있습니다. 
		ex. -5를 넣으면 5, int n1 = -200; >> System.out.println(Math.abs(n1)); = 200

		2. max() : 두 숫자 중 더 큰 값을 반환합니다.
		int n1 = 100, n2 = 200;
		System.out.println(Math.max(n1, n2));  >> 200

		3. min() : 두 숫자 중 더 작은 값을 반환합니다.
		int n1 = 100, n2 = 200;
		System.out.println(Math.min(n1, n2));  >> 100

	}

```	

## 문자열 함수

```java

	public static void main(String[] args) {

		제 생각에 활용 빈도가 높은 함수들을 나열해봤습니다.

		length(): 문자열의 길이를 반환합니다.
		charAt(): 주어진 인덱스의 문자를 반환합니다.
		substring(): 주어진 인덱스 범위의 부분 문자열을 반환합니다.
		indexOf(): 주어진 문자나 문자열이 처음 나타나는 인덱스를 반환합니다.
		replace(): 문자열의 일부를 다른 문자열로 바꿉니다.
		toLowerCase(): 문자열을 소문자로 변환합니다.
		toUpperCase(): 문자열을 대문자로 변환합니다.
		A.equals(B) : A와 B의 값이 동일한지 판별합니다.
 
		사용예시는 대해서 작성한 '문자열과 기능'의 주소를 남겨두겠습니다.
	}
```		<https://yunsnote.github.io/blog/day005/>
		


```

## 배열관련 함수

```java

	equals(): 두 배열이 같은지를 확인하며 값이 동일한지 판별합니다.
	A.equals(B) =  A와 B의 값이 동일한지 판별합니다.

	toString(): 배열의 내용을 문자열로 변환합니다.
	System.out.println("arr1 : " + Arrays.toString(arr1)); = arr1의 값을 나열합니다.

```

# 유형별 응용하면 좋을 구문

***

## 변수 선언

```java
	
	public static void main(String[] args) {

		int age;
		String name;

	}
```

## 변수 초기화	

```java

	public static void main(String[] args) {

		int age = 32;
		String name = "코붕이";

		변수 선언 / 초기화 
		변수는 간단한 계산이나 데이터 저장이 필요한 경우에 사용합니다.
		예시: 사람의 나이, 이름, 점수 등을 저장하고 처리할 때

	}
```

## 조건문 (if, else if, else)

```java

	public static void main(String[] args) {

		if (age >= 18) {
			System.out.println("성인입니다.");
		} else if (age >= 13) {
			System.out.println("청소년입니다.");
		} else {
			System.out.println("어린이입니다.");
		}

		조건에 따라 다른 작업을 수행해야 하는 경우 사용합니다.
		활용 예시로는,
		학점부여 / 성인,청소년,어린이 구분 / 영업시간 판별 / 최소,최대값 찾기,
		홀/짝수 찾기 / 할인율계산 / 이동거리에 따른 교통수단 선택 등...

	}
```

## 반복문 (for, while, do-while)

```java	

	public static void main(String[] args) {
		
		int[] numbers = {1, 2, 3, 4, 5};

		for (int i = 0; i < numbers.length; i++) {
		    System.out.println("Index " + i + ": " + numbers[i]);
		}

		int n = 10;
		int t1 = 0, t2 = 1, nextTerm;

		for (int i = 1; i <= n; i++) {
			System.out.print(t1 + ", ");
		nextTerm = t1 + t2;
		t1 = t2;
		t2 = nextTerm;
		}


		int i = 0;
		while (i < 5) {
			System.out.println("반복: " + i);
			i++;
		}

		int i = 0;
		do {
			System.out.println("반복: " + i);
			i++;
		} while (i < 5);

		특정 작업을 반복적으로 수행하고 일정한 패턴이나 순서를 따르는 문제를 해결할 때,
		반복문을 사용하면 효과적으로 문제를 해결할 수 있습니다.
		활용 예시로는,
		배열의 요소에 접근 / 구구단 / 문자열의 각 문자 처리 / 패턴출력 / 파보나치 수열 등...
	}
```
## if문과 for문 ---

	if문 안에 for문을 사용하는 경우는 특정 조건에 따라 반복 작업 자체를 수행할지 말지를 결정하는 데 사용되며,
	for문 안에 if문을 사용하는 경우는 반복 작업 중에 특정 조건에 따라 다른 처리를 수행하는 데 사용됩니다.
	사용 예시는 다음에 올리도록 하겠습니다!

```		

	
