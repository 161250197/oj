# 3-10 整除查询

## Description

Given an array of positive integers and many queries for divisibility. In every query Q[i], we are given an integer K , we need to count all elements in the array which are perfectly divisible by K.

Constraints:1<=T<=100;1<=N,M<=105;1<=A[i],Q[i]<=105

## Input

The first line of input contains an integer T denoting the number of test cases. Then T test cases follow. Each test case consists of three lines. First line of each test case contains two integers N & M, second line contains N space separated array elements and third line contains M space separated queries.

## Output

For each test case,In new line print the required count for each query Q[i].

## Sample

### Sample Input 1

~~~
2
6 3
2 4 9 15 21 20
2 3 5
3 2
3 4 6
2 3
~~~

### Sample Output 1

~~~
3 3 2
2 2
~~~

## Trick & Solutions

1. `0` 不可以被任何数字整除；

2. 当 `Q[i]` 为 0 时可以进行特判。
