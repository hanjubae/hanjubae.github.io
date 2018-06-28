---
layout: post
title:  "SCPC 연습문제 풀이<br/>
'숫자 골라내기'"
date:   2018-06-28 15:00:00 +0900
categories: [dsaa]
tags : [memorization]
---

#### 문제

### [SCPC_숫자 골라내기](https://www.codeground.org/practice/practiceProblemViewNew)

---


#### 문제 해설

- 문제 설명
	N(N은 3,000,000이하의 자연수)개의 숫자(32bit 정수형 변수에 담을 수 있는 음이 아닌 정수)가 주어진다.  
	같은 숫자의 갯수가 홀수개인 수끼리 XOR연산을 한 결과값을 출력하라.
<br/>
- 규칙
	1. N의 제한이 3,000,000이기 때문에 O(N)만에 갯수가 홀수인지 짝수인지 파악할 수 있도록 한다.
		> 정렬을 한 뒤 이전 숫자와 같으면 cnt를 추가하고 달라지면 그때 cnt를 이전 숫자의 갯수로 파악한다.


#### 시간 복잡도

> N개의 숫자를 퀵정렬로 정렬하면 O(NlogN), 홀수인지 짝수인지 파악하는 연산횟수는 O(N)이기 때문에
O(NlongN + N)만에 해결가능하다.

---
##### [코드 보기](https://github.com/hanjubae/dsaa/blob/master/algorithm/swexpert/SW_3459_ExpressShort.cpp)
