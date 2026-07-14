---
title: 2026-07-14 · Minimize Maximum Difference of Three Groups
parent: 算法每日一题
nav_order: 20260714
permalink: /daily/minimize_maximum_group_difference_20260714/
published_at: "2026-07-14 20:36:26"
---

# DRW - Minimize Maximum Difference of Three Groups

## Problem
You are given an array `A` consisting of `N` integers. Divide all elements into three non-empty groups. Each element must belong to exactly one group.

For each group, define its difference as the largest integer in the group minus the smallest integer in the group.

Your goal is to make the maximum of these three group differences as small as possible.

Return the minimum possible value of that maximum difference.


## Constraints
```
3 <= N <= 10^5, where N = length of the given array A
A consists of integers
Each element must belong to exactly one of three non-empty groups
```


## Examples

| # | Input | Output | Note |
|---|-------|--------|------|
| 1 | `A = [11,5,3,12,6,8,1,7,4]` | `3` | 一种最优分组为 `[3,1,4]`、`[5,6,8,7]`、`[11,12]`，极差分别为 `3、3、1` |
| 2 | `A = [10,14,12,1000,11,15,13,1]` | `5` | 一种最优分组为 `[1]`、`[10,14,12,11,15,13]`、`[1000]`，最大极差为 `5` |
| 3 | `A = [4,5,7,10,10,12,12,12]` | `2` | 一种最优分组为 `[4]`、`[5,7]`、`[10,10,12,12,12]`，极差分别为 `0、2、2` |


## Knowledge Points
- 排序 + 贪心 + 二分答案


## Solution
- **直观思路**：先将数组排序。对于一个给定的最大极差 `up`，从最小的未分组元素开始，把所有与它相差不超过 `up` 的后续元素放入同一组。这样每组容纳的元素尽可能多，得到的组数最少。
- **二分答案**：答案范围是 `0 ~ max(A) - min(A)`。若某个 `up` 最多需要 3 组，则它可行；否则不可行。可行性具有单调性，因此可以二分找到最小的可行值。
- **恰好三组**：检查时判断的是“最少组数是否不超过 3”。如果只得到 1 组或 2 组，可以继续拆分已有组；拆分不会增大组内极差。由于 `N ≥ 3`，一定能拆成恰好 3 个非空组。
- **踩坑**：
  - 判断当前元素能否加入一组时，应计算它与该组最小值的差，而不是与前一个元素的差。
  - `check` 中得到的组数超过 3 时可直接返回 `False`。
  - 若不希望修改传入的数组，应使用 `sorted(A)`，而不是 `A.sort()`。
- **复杂度**：设 `V = max(A) - min(A)`。时间复杂度为 `O(N log N + N log V)`，空间复杂度为 `O(N)`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------


def check(A, up):
    n = len(A)
    group_min = A[0]
    group_count = 1

    for i in range(1, n):
        if A[i] - group_min > up:
            group_min = A[i]
            group_count += 1

            if group_count > 3:
                return False

    return True


def solution(A):
    A = sorted(A)
    left, right = 0, A[-1] - A[0]
    res = right

    while left <= right:
        mid = left + (right - left) // 2

        if check(A, mid):
            res = mid
            right = mid - 1
        else:
            left = mid + 1

    return res


if __name__ == '__main__':
    print(solution([11, 5, 3, 12, 6, 8, 1, 7, 4]))  # 3
    print(solution([10, 14, 12, 1000, 11, 15, 13, 1]))  # 5
    print(solution([4, 5, 7, 10, 10, 12, 12, 12]))  # 2
```
