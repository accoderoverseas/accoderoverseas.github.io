---
title: 2026-07-13 · Bitwise XOR Subsequence
parent: 算法每日一题
nav_order: 20260713
permalink: /daily/bitwise_xor_subsequence_20260713/
published_at: "2026-07-13 15:20:09"
---

# JPMorgan - Bitwise XOR Subsequence

## Problem
A subsequence of an array is formed by removing zero or more elements without changing the order of the remaining elements.

A subsequence is valid when the bitwise XOR of every pair of adjacent elements equals `k`. A subsequence of length `1` is invalid, regardless of the value of `k`, because it contains no adjacent pair.

Given an integer array `arr` of size `n` and an integer `k`, return the length of the longest valid subsequence. If no valid subsequence exists, return `0`.


## Constraints
```
1 <= n <= 10^5
arr.length == n
0 <= arr[i] <= 10^6
0 <= k <= 10^6
```


## Examples

| # | Input | Output | Note |
|---|-------|--------|------|
| 1 | n = 5<br/>arr = [2,1,3,5,2]<br/>k = 2 | 2 | 子序列 `[1,3]` 合法，因为 `1 XOR 3 = 2`，且不存在更长的合法子序列 |
| 2 | n = 3<br/>arr = [1,1,1]<br/>k = 0 | 3 | 整个数组都合法，因为任意相邻元素均满足 `1 XOR 1 = 0` |
| 3 | n = 8<br/>arr = [4,7,4,1,7,4,7,9]<br/>k = 3 | 6 | 最长合法子序列为 `[4,7,4,7,4,7]` |


## Knowledge Points
- 动态规划-线性DP + 哈希表 + 位运算


## Solution
- **状态定义**：`dp[i]` 表示以 `arr[i]` 结尾的最长候选子序列长度，初始值为 `1`。
- **状态转移**：若前一个元素为 `x`，则需满足 `x XOR arr[i] = k`，因此 `x = arr[i] XOR k`。用哈希表 `pos` 记录每个值最后一次出现的位置，即可在 `O(1)` 时间找到前驱并完成转移。
- **为什么只记录最后位置**：同一个值后一次出现时，可用的前驱只会更多，因此对应的 `dp` 值不会变小，最后一次出现的位置一定是当前最优位置。
- **长度限制**：长度为 `1` 的子序列非法，所以只有当 `dp[i] >= 2` 时才更新答案；若不存在合法子序列，返回 `0`。
- **踩坑**：必须先计算 `dp[i]`，再更新 `pos[arr[i]]`。尤其当 `k = 0` 时，提前更新会错误地把当前位置当作自己的前驱。
- **复杂度**：时间复杂度 `O(n)`，空间复杂度 `O(n)`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------


def maxSubsequenceLength(n, arr, k):
    pos = {}
    dp = [1] * n
    res = 0

    for i in range(n):
        prev = arr[i] ^ k
        if prev in pos:
            dp[i] = dp[pos[prev]] + 1

        if dp[i] >= 2:
            res = max(res, dp[i])

        pos[arr[i]] = i

    return res


if __name__ == '__main__':
    print(maxSubsequenceLength(5, [2, 1, 3, 5, 2], 2))              # 2
    print(maxSubsequenceLength(3, [1, 1, 1], 0))                    # 3
    print(maxSubsequenceLength(8, [4, 7, 4, 1, 7, 4, 7, 9], 3))    # 6
    print(maxSubsequenceLength(1, [1000000], 1000000))              # 0
```
