# 74. 搜索二维矩阵

> 难度：中等

## 说明

编写一个高效的算法来判断 m x n 矩阵中，是否存在一个目标值。该矩阵具有如下特性：

每行中的整数从左到右按升序排列。
每行的第一个整数大于前一行的最后一个整数。

## 示例

示例 1：

> **输入：** matrix = [[1,3,5,7],[10,11,16,20],[23,30,34,60]], target = 3
> 
> **输出：** true

示例 2：

> **输入：** matrix = [[1,3,5,7],[10,11,16,20],[23,30,34,60]], target = 13
> 
> **输出：** false

## 提示

> m == matrix.length
> 
> n == matrix[i].length
> 
> 1 <= m, n <= 100
> 
> -104 <= matrix[i][j], target <= 104

## 思路

二分查找查找可能存在目标数的行，可能会因为矩阵的最小数也大于目标值，此时二分得到的行号是 -1，可以提前结束。

然后在行中继续使用二分查找来查找目标，此时如果查到即可直接返回，如果二分结束说明未找到目标值。
