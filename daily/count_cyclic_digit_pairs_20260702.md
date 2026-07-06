---
title: 2026-07-02 · Count Cyclic Digit Pairs
parent: 算法每日一题
nav_order: 20260702
permalink: /daily/count_cyclic_digit_pairs_20260702/
---

# TikTok - Count Cyclic Digit Pairs

## Problem
A cyclic shift is the operation of rearranging the digits in a number (in decimal format) by moving some digits at the end of the number to before the beginning of the number, while shifting all other digits to the next position.   

Given two integers of the same length `a` and `b`, a would be a cyclic pair of `b` if it is possible for `a` to become equal to `b` after performing cyclic shifts on `a`, moving `0` or more ending digits to the beginning while shifting all other digits to the next position in the same order.  

Given an array of `N` positive integers `a`, count the number of cyclic pairs `i` and `j` (`0 <= i < j < a.length`), such that `a[i]` and `a[j]` have the same number of digits and `a[i]` is equal to a cyclic shift of `a[j]`.

## Constraints
```
1 <= N <= 100000
1 <= a[i] <= 1000000000
```


## Examples

| # | Input                                              | Output | Note |
|---|----------------------------------------------------|--------|------|
| 1 | a = [13, 5604, 31, 2, 13, 4560, 546, 654, 456]     | 5      | 5 组循环对（见下方拆解）。|
| 2 | a = [5604, 4560]                                   | 1      | 移位会产生前导零：`5604` 的旋转含 `4560`，二者 4 位、互为移位。|
| 3 | a = [4560, 456]                                    | 0      | **位数不同**（4 位 vs 3 位），不构成循环对。|
| 4 | a = [11, 11]                                       | 1      | **周期串**：`11` 只有 1 个不同旋转，仍只算 1 对。|

**Example 1 的 5 组循环对拆解：**
- `a[0]=13` 与 `a[2]=31`（`13 → 31`）
- `a[0]=13` 与 `a[4]=13`（0 次移位即相等）
- `a[2]=31` 与 `a[4]=13`
- `a[1]=5604` 与 `a[5]=4560`（`5604` 的旋转集合含 `4560`）
- `a[6]=546` 与 `a[7]=654`（`546` 的旋转集合 `{546, 654, 465}` 含 `654`）

注意：`a[6]=546` 与 `a[8]=456` **不是**循环对（`456` 不在 `546` 的旋转集合 `{546, 654, 465}` 里）；`a[5]=4560` 与 `a[8]=456` 也不是（位数不同）。


## Knowledge Points
- 字符串 + 哈希表 + 数学-组合数学


## Solution
- **直观思路**：计算满足题意的二元组 `(a[i], a[j])` 的个数，容易想到双重循环枚举，然后将这两个整数转换成字符串模拟「循环右移」过程，可行但时间复杂度 `O(n² * L)`，在现有数据规模下超时！
- **最优解切入点（关键转化）**：进一步分析，其实不需要双重循环枚举。由于当整数 `a[i]` 是 `a[j]` 的循环移位时，其中一个整数对应的字符串形式必然可通过有限次「循环右移」得到另一个整数的字符串形式。因此，整个数组被切分成若干**等价类**，每个等价类对答案的贡献是独立的。
- **步骤**：  
  Step 1. 遍历数组中的每个整数，转换成字符串；  
  Step 2. 对转换后的字符串，维护 L 次循环右移过程中可得到的字典序最小的字符串，将其插入哈希表（map）计算出现次数；  
  Step 3. 从而，对哈希表中出现的字符串，若其出现次数为 `x`，则对答案的贡献为 `C(x, 2) = x * (x - 1) / 2`。  
- **复杂度**：时间复杂度 `O(n * L²)`，空间复杂度 `O(n)`。

**注意：两个隐藏约束由该方案自动满足：**
1. **「位数相同」**：最小循环表示是**定长串**，长度等于原数字串长度。不同位数的数产生不同长度的规范串，绝不会落进同一组。所以 `4560`（规范串 `0456`）与 `456`（规范串 `456`）天然分开。
2. **「移位产生的前导零」**：旋转出的 `"0456"` 被**完整保留在定长规范串里**参与比较，因此 `5604` 与 `4560` 的规范串都是 `0456`、正确归为一组；而它们绝不会和三位数 `456` 混淆。

**注意：几个常见的坑：**
1. **周期串重复计数（最坑）**：如果换一种写法——「枚举每个旋转并累加它在前缀里的出现次数」，那么对**周期串**（如 `"11"`、`"1212"`、`"111"`）会出错。因为长度 `L`、最小周期 `p` 的串只有 `p` 个不同旋转，但会被枚举到 `L` 次，每个匹配被放大 `L/p` 倍。
   - 反例：`[11, 11]` 会错算成 `2`（正确 `1`）；`[111, 111]` 会错算成 `3`。
   - **本解法为何不踩坑**：这里用的是 `min`（幂等运算）取规范表示，`"11"` 转几次都还是 `"11"`，取 `min` 不会重复放大；且分组后统一用 `C(k,2)` 计数。
2. **位数相同别漏判**：本方案靠「规范串定长」自动保证；若手写比较，务必先判 `len(str(x)) == len(str(y))`。
3. **前导零要保留**：旋转得到的串必须按定长参与比较，不能当成整数去掉前导零，否则 `4560` 与 `456` 会被错误合并。
4. **N = 1**：无法构成 `i < j` 的对，答案恒为 `0`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

import collections


def solution(a):
    n = len(a)
    freq = collections.defaultdict(int)
    for i in range(n):
        # canonical form = lexicographically smallest rotation
        # (kept as a fixed-length string so leading zeros are preserved)
        cur_num, min_num = str(a[i]), str(a[i])
        for j in range(len(cur_num)):
            cur_num = cur_num[-1] + cur_num[:-1]   # rotate right by one digit
            min_num = min(min_num, cur_num)
        freq[min_num] += 1

    # each group of k numbers sharing a canonical form contributes C(k, 2) pairs
    res = 0
    for cur_num in freq:
        cur_freq = freq[cur_num]
        res += cur_freq * (cur_freq - 1) // 2
    return res


if __name__ == '__main__':
    print(solution([13, 5604, 31, 2, 13, 4560, 546, 654, 456]))  # 5
    print(solution([123, 231, 312, 999]))  # 3
    print(solution([1234, 4123, 1243]))  # 1
    print(solution([1020, 2010, 102, 210]))  # 2
    print(solution([1, 2, 3, 4, 5]))  # 0
    print(solution([1000000000, 1000000000, 1000000000, 1000000000, 1000000000, 1000000000]))  # 15
    print(solution([11, 11]))  # 1
    print(solution([1212, 2121]))  # 1
```
