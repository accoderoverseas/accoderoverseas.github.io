---
title: Promotional Periods
parent: Amazon
grand_parent: 求职找工OA/VO真题拆解
nav_order: 1
---

# Amazon - Promotional Periods

## Problem
Data analysts at Amazon are studying product order patterns. They classify a period of at least three consecutive days as a promotional period when the order counts on the first and last days are both greater than every order count on the days between them.

More formally, for an array `orders`, a subarray from index `i` to index `j` is a promotional period if `j - i + 1 >= 3` and `min(orders[i], orders[j]) > max(orders[i + 1], orders[i + 2], ..., orders[j - 1])`.

Given the order statistics for `n` consecutive days, return the number of promotional periods.


## Constraints
```
3 <= n <= 2 x 10⁵
1 <= orders[i] <= 10⁹
All integers in orders are distinct.
```


## Examples

| # | Input                                  | Output | Note                                                       |
|---|----------------------------------------|--------|------------------------------------------------------------|
| 1 | orders = [3, 2, 8, 6]<br/>n = 4        | 1      | Only `[1, 3]` is valid: `min(3, 8) = 3 > 2`.               |
| 2 | orders = [5, 1, 4, 2, 6]<br/>n = 5     | 3      | Valid periods: `[5,1,4]`, `[4,2,6]`, `[5,1,4,2,6]`.        |


## Knowledge Points
- 贪心 + 单调栈

## Solution
- **直观思路**：枚举所有长度 `>= 3` 的子数组 `[i, j]`，逐个检查 `min(端点) > max(中间)`。即使用前缀最大值优化区间最值查询，仍需枚举 `O(n²)` 个区间，`n` 达到 `2×10⁵` 时必然超时，不是最优解！
- **最优解切入点**：观察条件 `min(orders[i], orders[j]) > max(orders[i+1], orders[i+2], ..., orders[j-1])`，它的真正含义是 **端点 `i` 和 `j` 互相「可见」**——两者之间没有比它俩更高的元素遮挡视线。于是问题转化为「统计互相可见的元素对数量」：
  - 所有**相邻对** `(k-1, k)` 中间为空，必然可见，共 `n - 1` 对；
  - 题目要求长度 `>= 3`，这些长度为 2 的相邻对需要排除；
  - 所以 **答案 = 可见对总数 − (n − 1)**。
- **步骤**：  
  Step 1. 维护一个**严格递减**的单调栈（题目保证元素互不相同，无需处理相等情况）  
  Step 2. 遍历每个元素 `x`，不断弹出栈顶**比 `x` 小**的元素，每弹出一个就构成一对可见对（它被 `x` 挡住视线前能看到 `x`）  
  Step 3. while 弹完后若栈非空，栈顶（第一个比 `x` 大的元素）越过刚被弹掉的矮元素也能看到 `x`，再 `+1`  
  Step 4. 最终 `可见对总数 − (n − 1)` 即为答案  
- **复杂度**：时间复杂度 O(n)，空间复杂度 O(n)。这是因为，每个元素仅入栈、出栈各一次。

## AC Code
```python
def countPromotionalPeriods(orders):
    n = len(orders)

    stack = []
    res = 0
    for i in range(n):
        while stack and orders[stack[-1]] < orders[i]:
            stack.pop()
            res += 1

        if stack:
            res += 1
        stack.append(i)
    return res - (n - 1)


if __name__ == '__main__':
    print(countPromotionalPeriods([3, 2, 8, 6]))  # 1
    print(countPromotionalPeriods([5, 1, 4, 2, 6]))  # 3
    print(countPromotionalPeriods([1, 2, 3, 4, 5, 6]))  # 0
    print(countPromotionalPeriods([10, 5, 3, 1, 2, 4, 6, 8]))  # 6
    print(countPromotionalPeriods([10, 7, 100]))  # 1
```
