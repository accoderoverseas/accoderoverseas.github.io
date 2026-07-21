---
title: 2026-07-21 · Smallest Substring With Exactly K Ones
parent: 算法每日一题
nav_order: 20260721
permalink: /daily/smallest_substring_with_k_ones_20260721/
published_at: "2026-07-21 19:24:13"
---

# Akuna Capital - Smallest Substring With Exactly K Ones

## Problem
You are given a binary string `input_str` and an integer `k`.

Find a substring of `input_str` that satisfies all of the following conditions:
- It contains exactly `k` occurrences of `'1'`.
- It has the smallest possible length.
- Among all substrings with that minimum length, it is lexicographically smallest.

It is guaranteed that an answer exists.


## Constraints
```
- 1 <= k <= length of input_str <= 1000
- input_str[i] is in the set {'0', '1'}
- The number of '1' characters in input_str is always greater than or equal to k
```


## Examples

| # | Input                                        | Output   | Note                                                          |
|---|----------------------------------------------|----------|---------------------------------------------------------------|
| 1 | input_str = "0101101"<br/>k = 3              | "1011"   | 候选 "01011"/"1101"/"1011"，最短且字典序最小为 "1011"           |
| 2 | input_str = "1011"<br/>k = 2                 | "11"     | "101"(长 3) 与 "11"(长 2)，最短为 "11"                          |
| 3 | input_str = "11011"<br/>k = 3               | "1011"   | 等长(4) 的 "1101" 与 "1011"，字典序取小得 "1011"                |


## Knowledge Points
- 字符串 + 滑动窗口


## Solution
- **直观思路**：直接枚举全部 `O(n²)` 个子串，逐个数 1、比长度、比字典序。`n ≤ 1000` 能过，但写起来笨重，且极易被首尾的 `0` 干扰。
- **关键切入点**：**最优子串的首尾一定都是 `'1'`**。反证——若某个合法子串以 `0` 开头（或结尾），把这个 `0` 删掉，`1` 的个数不变、长度却更短，与「最短」矛盾。所以只需锁定所有 `'1'` 的位置，`0` 在哪里根本不用管。
- **步骤**：
  - Step 1. 顺序扫描，记录所有 `'1'` 的下标 `pos`，共 `m` 个。
  - Step 2. 恰好 `k` 个 1 的最短窗口 = `pos` 中**连续的 k 个**：`pos[i] ~ pos[i+k-1]`，对应子串 `input_str[pos[i] : pos[i+k-1]+1]`，枚举 `i ∈ [0, m-k]`。
  - Step 3. 两级比较收尾：先取长度最短；长度相同，再用字典序 `min` 决胜。
- **踩坑**：
  - 循环上界是 `range(m - k + 1)`，写成 `m - k` 会漏掉最后一个窗口（经典 off-by-one）。
  - **不能只按字典序比较**。二进制串里更长的窗口可能字典序更小（如 `"101" < "11"`），必须**先比长度、再比字典序**，顺序反了直接 WA。
- **复杂度**：时间 `O(n·m)`（枚举 `m` 个窗口，每次截取/比较 `O(n)`），最坏 `O(n²)`；空间 `O(m)`。`n ≤ 1000` 完全够用。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

def getSubstring(input_str, k):
    n = len(input_str)
    pos = []
    for i in range(n):
        if input_str[i] == "1":
            pos.append(i)

    m = len(pos)
    res = ""
    for i in range(m - k + 1):
        left, right = pos[i], pos[i + k - 1]
        cur_str = input_str[left: right + 1]
        if not res or len(cur_str) < len(res):
            res = cur_str
        elif len(cur_str) == len(res):
            res = min(res, cur_str)
    return res


if __name__ == '__main__':
    print(getSubstring("0101101", 3))  # "1011"
    print(getSubstring("1011", 2))     # "11"
    print(getSubstring("11011", 3))    # "1011"
```
