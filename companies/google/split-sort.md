---
title: Split Sort
parent: Google
grand_parent: 求职找工OA/VO真题拆解
nav_order: 1
published_at: "2026-07-04 08:48:54"
---

# Google - Split Sort

## Problem
Given an array `A` of `N` integers.  
You can split the array into two non-empty parts, left and right, sort the elements in each part independently and join them back together.  
Returns the number of different ways of obtaining a sorted array by the procedure above. 


## Constraints
```
1 <= N <= 10000, 1 <= A[i] <= 10000
```


## Examples

| # | Input                               | Output | Note                                                      |
|---|-------------------------------------|--------|-----------------------------------------------------------|
| 1 | A = [1, 3, 2, 4]<br/>N = 4          | 2      | Two valid positions: <br/>[1] [3, 2, 4]<br/>[1, 3, 2] [4] |
| 2 | A = [5, 5, 5, 5, 5]<br/>N = 5       | 4      | All four positions are valid.                             |
| 3 | A = [7, 6, 5, 4, 3, 2, 1]<br/>N = 7 | 0      | No valid position.                                        |


## Knowledge Points
- 动态规划 DP - 前后缀分解 DP

## Solution
- **直观思路**：长度为 `N` 的数组共 `(N - 1)` 个分割点，容易想到枚举分割点+排序判断，可行但时间复杂度 `O(n² log n)`，不是最优解！
- **最优解切入点**：进一步分析，左右两半数组各自排序后，左半的末尾 = 左半的最大值，右半的开头 = 右半的最小值。所以拼接后的数组非递减有序时，**当且仅当 max(left) <= min(right)**。因此，可通过前后缀分解 DP 求解。
- **步骤**：  
  Step 1. 预处理前缀最大值数组 `dp_left[i] = max(A[0..i])`  
  Step 2. 预处理后缀最小值数组 `dp_right[i] = min(A[i..N-1])`  
  Step 3. 枚举拆点 `k ∈ [0, N-2]`，若 `prefix_max[k] <= suffix_min[k+1]` 则找到一个合法的分割点  
- **复杂度**：时间复杂度 O(n)，空间复杂度 O(n)。

## AC Code
```python
def solution(A):
    n = len(A)
    dp_left = [0] * n; dp_left[0] = A[0]
    for i in range(1, n):
        dp_left[i] = max(dp_left[i - 1], A[i])

    dp_right = [0] * n; dp_right[n - 1] = A[n - 1]
    for i in range(n - 2, -1, -1):
        dp_right[i] = min(dp_right[i + 1], A[i])

    res = 0
    for i in range(n - 1):
        if dp_left[i] <= dp_right[i + 1]:
            res += 1
    return res


if __name__ == '__main__':
    print(solution([1, 3, 2, 4]))  # 2
    print(solution([5, 5, 5, 5, 5]))  # 4
    print(solution([7, 6, 5, 4, 3, 2, 1]))  # 0
```
