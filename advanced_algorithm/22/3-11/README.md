# 3-11 对称子字符串

## Description

Given a string ‘str’ of digits, find length of the longest substring of ‘str’, such that the length of the substring is 2k digits and sum of left k digits is equal to the sum of right k digits.

## Input

输入第一行是测试用例的个数，后面每一行表示一个数字组成的字符串，例如："123123"

## Output

输出找到的满足要求的最长子串的长度。例如，给定的例子长度应该是 6。每行对应一个用例的结果。

## Sample

### Sample Input 1

~~~
1
1538023
~~~

### Sample Output 1

~~~
4
~~~

## Trick & Solutions

1. 使用 `Integer` 类型时会出现超出常量池预存的数字，导致使用 `==` 结果不合预期。
