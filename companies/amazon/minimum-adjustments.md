---
title: Minimum Adjustments
parent: Amazon
grand_parent: 求职找工OA/VO真题拆解
nav_order: 2
---

# Amazon - Minimum Adjustments (Prefix ±1 to Zero)

## Problem
You are given an integer array `values` of `N` integers.
You need to perform some adjustments on the array to make all elements equal to `0`.
In one adjustment, you can select a **prefix** of the array and increase **or** decrease all elements of that prefix by `1`.
Return the minimum number of adjustments required to convert every element of the array to `0`.

A prefix is a contiguous group of items that includes the first element. For example, `[1]`, `[1, 2]`, `[1, 2, 3]` are prefixes of `[1, 2, 3, 4, 5]`.

> **Note**: It is guaranteed that it is always possible to convert every element of the array to `0`.


## Constraints
```
1 <= N <= 100000
values[i] is an integer (may be negative)
```


## Examples

| # | Input                              | Output | Note                                                                                                                       |
|---|------------------------------------|--------|----------------------------------------------------------------------------------------------------------------------------|
| 1 | A = [3, 2, 1]<br/>N = 3            | 3      | prefix len 2, −1 → [2,1,1]; prefix len 1, −1 → [1,1,1]; prefix len 3, −1 → [0,0,0]. 无法少于 3 次。                          |
| 2 | A = [1, 2, 3, 4, 5]<br/>N = 5      | 9      | `\|5\| + \|2-1\| + \|3-2\| + \|4-3\| + \|5-4\| = 5+1+1+1+1`                                                                  |
| 3 | A = [-1, 2, -3]<br/>N = 3          | 11     | `\|-3\| + \|2-(-1)\| + \|-3-2\| = 3+3+5`，含负数与符号交替的一般情况。                                                       |


## Knowledge Points
- 贪心 + 差分


## Solution
- **直观思路**：把数组看成一排柱子，每次操作是把「从最左端起的一段连续前缀」整体抬高或压低 `1`。朴素做法逐位贪心模拟可行，但描述清楚后会发现根本不必模拟。

- **最优解切入点**：关键在于**每次操作必然从第一个元素开始**，所以"操作长度的分界"只可能落在相邻元素之间。考察相邻两元素 `values[i-1]` 与 `values[i]`：能影响左边那根、却不影响右边那根的操作，**恰好是长度为 `i` 的前缀操作**。要抹平它们之间的高度差，长度为 `i` 的操作净次数必须等于 `values[i] - values[i-1]`，至少需要 `|values[i] - values[i-1]|` 次。而最后一个元素 `values[N-1]` 只能被长度为 `N` 的最长前缀影响，把它降到 `0` 需要 `|values[N-1]|` 次。各需求相互独立，累加即为答案。

- **公式**：
  ```
  answer = |values[N-1]| + Σ_{i=1}^{N-1} |values[i] - values[i-1]|
  ```

- **差分视角推导（严谨证明）**：设长度为 `k` 的操作净次数为 `c_k`。元素 `i` 的总变化量为 `Σ_{k≥i+1} c_k`，须等于 `-values[i]`。令 `P_i = Σ_{k=i+1}^{N} c_k = -values[i]`（约定 `P_N = 0`），则 `c_k = P_{k-1} - P_k`，解得 `c_k = values[k] - values[k-1]`（`k < N`）、`c_N = -values[N-1]`。最少操作数 `= Σ|c_k|`，即上式。每个 `c_k` 取值唯一，故公式给出的就是最优解。

- **步骤**：  
  Step 1. 累加末位绝对值 `res = |values[N-1]|`  
  Step 2. 从左到右累加相邻差的绝对值 `res += Σ |values[i] - values[i-1]|`  
  Step 3. 返回 `res`  

- **复杂度**：时间复杂度 O(n)，空间复杂度 O(1)。

- **注意**：数值绝对值可能较大，累加和会超出 32 位范围。Python 整数任意精度无碍；移植到 C++/Java 时**务必用 64 位整数（`long long`）**，否则会溢出。


## AC Code
```python
def calculateMinimumAdjustments(values):
    n = len(values)
    res = abs(values[-1])
    for i in range(n - 1):
        res += abs(values[i] - values[i + 1])
    return res


if __name__ == '__main__':
    print(calculateMinimumAdjustments([3, 2, 1]))  # 3
    print(calculateMinimumAdjustments([5]))  # 5
    print(calculateMinimumAdjustments([5, 2, 4, 1, 3]))  # 13
```
