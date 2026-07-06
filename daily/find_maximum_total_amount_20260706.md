---
title: 2026-07-06 · Find Maximum Total Amount
parent: 算法每日一题
nav_order: 20260706
permalink: /daily/find_maximum_total_amount_20260706/
---

# Amazon - Find Maximum Total Amount

## Problem
There is an infinite line of bags numbered `1 ~ ∞`.  

You are given an `n × 3` array `segment`, where each `segment[i] = [l, r, v]` means every bag in the range `l ~ r` holds `v` money.  
The segments do not intersect, and any bag not covered by a segment holds `0` money.  

Given an integer `k`, select `k` **consecutive** bags so that the total amount of money is maximized. Return the answer modulo `10⁹ + 7`.


## Constraints
```
- segment is an n × 3 array, segment[i] = [l, r, v]: every bag in range l~r holds v money
- All segments are non-intersecting; any bag not covered by a segment holds 0 money
- Bags are numbered 1 ~ ∞; l, r and k can be very large (far beyond what an array can hold)
- Return the answer modulo 10⁹ + 7
```


## Examples

| # | Input                                                        | Output | Note                                                              |
|---|--------------------------------------------------------------|--------|-------------------------------------------------------------------|
| 1 | segment = [[1,4,2],[6,6,5],[7,7,7],[9,10,1]]<br/>k = 5       | 16     | 金额 = 2 2 2 2 0 5 7 0 1 1；最优窗口 [3,7] = 2+2+0+5+7 = 16        |
| 2 | segment = [[1,3,10],[6,8,10]]<br/>k = 6                      | 40     | 窗口 [1,6] 或 [3,8] 各覆盖两段共 4 个非零袋 = 40                    |
| 3 | segment = [[1,100,5]]<br/>k = 200                            | 500    | 仅 100 个非零袋，k ≥ 100 时全覆盖 = 100 × 5 = 500                   |


## Knowledge Points
- 前缀和 + 二分查找 + 滑动窗口


## Solution
- **直观思路**：坐标到无穷、`k` 可极大，逐袋开数组 + 滑动窗口会直接爆内存/超时，不可行。
- **最优解切入点**：金额沿坐标是**分段常数**函数。设窗口 `[L, L+k-1]` 的和为 `F(L)`，其一阶差分 `F(L+1) − F(L) = money(L+k) − money(L)`，只在区间边界处发生变化，故 `F` 是**分段线性**的 —— **最大值必在「边界对齐」的起点取得**。
- **步骤**：
  - Step 1. 按段起点排序（段互不相交 ⇒ 终点同序），预处理前缀和 `pre_sum[i]`。
  - Step 2. 收集候选起点：每段 `[l, r, v]` 取 `L ∈ {l, r−k+1, r+1, l−k}`，共 `O(n)` 个。
  - Step 3. 对每个候选窗口 `[L, L+k−1]`，二分定位相交段区间 `[lo, hi]`，用前缀和相减、再裁掉首尾越界部分，`O(log n)` 求和；全程取最大。
- **踩坑**：
  - **求最大值必须用真实数值比较，最后再统一取模**。若在 `max` 内部先 `% MOD`（如 `max(res, val % MOD)`），当真实值 ≥ MOD 时大小关系被打乱会 WA。
  - 候选起点会出现 `≤ 0` 的值（如 `r−k+1`、`l−k`），求和函数需能正确处理越界/空区间并返回 `0`。
  - 输入的段可能乱序，务必先按起点排序再做前缀和与二分。
- **复杂度**：时间 `O(n log n)`，空间 `O(n)`；与袋子数量、坐标大小、`k` 均无关。


## AC Code
```python
import bisect


def getRangeMoney(segment, starts, ends, pre_sum, left, right):
    # total money in bag range [left, right]; returns 0 for an empty range
    if left > right:
        return 0

    # segments intersecting [left, right]: those with end >= left and start <= right
    lo = bisect.bisect_left(ends, left)
    hi = bisect.bisect_right(starts, right) - 1
    if lo > hi:
        return 0

    res = pre_sum[hi + 1] - pre_sum[lo]   # sum of the fully/partially covered segments
    l1, r1, v1 = segment[lo]
    if l1 < left:                         # trim the part of the first segment before `left`
        res -= (left - l1) * v1

    l2, r2, v2 = segment[hi]
    if r2 > right:                        # trim the part of the last segment after `right`
        res -= (r2 - right) * v2
    return res


def maxTotalAmount(segment, k):
    n = len(segment)
    segment = sorted(segment, key=lambda x: x[0])   # sort segments by their start
    starts = []
    ends = []
    pre_sum = [0] * (n + 1)                          # prefix sum of money per segment
    for i in range(n):
        l, r, v = segment[i]
        starts.append(l)
        ends.append(r)
        pre_sum[i + 1] = pre_sum[i] + (r - l + 1) * v

    # F(L) is piecewise-linear, so the optimum window starts at a boundary-aligned point
    candidates = set()
    for l, r, v in segment:
        candidates.add(l)
        candidates.add(r - k + 1)
        candidates.add(r + 1)
        candidates.add(l - k)

    MOD = 10 ** 9 + 7
    res = 0
    # compare REAL values here; take the modulo only once at the very end
    for l in candidates:
        res = max(res, getRangeMoney(segment, starts, ends, pre_sum, l, l + k - 1))
    return res % MOD


if __name__ == '__main__':
    print(maxTotalAmount([[1, 4, 2], [6, 6, 5], [7, 7, 7], [9, 10, 1]], 5))  # 16
    print(maxTotalAmount([[1, 1, 1], [5, 5, 100]], 3))  # 100
    print(maxTotalAmount([[1, 3, 10], [6, 8, 10]], 6))  # 40
    print(maxTotalAmount([[1, 100, 5]], 200))  # 500
```

---

> **👤 ac_coder_tutor** — 在职工程师的「算法每日一题」  
> 📕 小红书 / 🛰️ 微信 `ac_coder_tutor` · 📮 `accoderoverseas@gmail.com`  
> 找工 OA/VO 真题拆解 · 留学生 CS 课程辅导 → [联系我](/contact/)
