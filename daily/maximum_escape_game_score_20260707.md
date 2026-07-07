---
title: 2026-07-07 · Maximum Escape Game Score
parent: 算法每日一题
nav_order: 20260707
permalink: /daily/maximum_escape_game_score_20260707/
published_at: "2026-07-07 20:00:00"
---

# Microsoft - Maximum Escape Game Score

## Problem
In an escape game, players clear an array of integers to earn points under the following rules, applied repeatedly until the array is empty:

1. Pick a value `v`. Remove **every** occurrence of `v` from the array and add their total (`v × count(v)`) to your score.
2. Then remove every element equal to `v + 1` or `v - 1`, earning **no** points for them.
3. Repeat steps 1–2 until the array is empty.

Return the **maximum** score obtainable.


## Constraints
```
1 <= n <= 10⁵, 1 <= elements[i] <= 10⁹
```


## Examples

| # | Input | Output | Note |
|---|-------|--------|------|
| 1 | `elements = [5,6,6,4,11]` | 27 | 取 11(+11);取两个 6(+12),同时白清掉 5、7;再取 4(+4)。11+12+4 = 27 |
| 2 | `elements = [1,2,3,4]` | 6 | 取值 2(+2,清掉 1、3),再取值 4(+4)。跳过相邻值去够更优组合 |
| 3 | `elements = [3,4,4,4]` | 12 | 取值 4 得 `4×3=12` 并清掉 3;若取值 3 只得 3。收益按 `v×count` 算,别只看值大小 |


## Knowledge Points
- 动态规划 DP - 线性 DP


## Solution
- **本质转化**：选值 `v` 的收益是 `v × count(v)`;选了 `v` 就不能选 `v−1`、`v+1`(它们被免费清除)。等价于在**值**上打家劫舍，值差为 1 的相邻值互斥**。注意不是"数组下标相邻",而是"值相差 1"。
- **最优解思路**：首先统计频次 `freq[v]`，对去重后的值升序排成 `keys`；然后定义 `dp[i]` = 只考虑 `keys[0..i]` 的最大得分。记 `take(i) = keys[i] × freq[keys[i]]`:
  - 不选 `keys[i]`：`dp[i-1]`
  - 单独取 `keys[i]`（丢掉前面全部）：`take(i)`
  - `keys[i-1]` 与之相邻（差 1）：`dp[i-2] + take(i)`
  - `keys[i-1]` 不相邻（差 ≥ 2）：`dp[i-1] + take(i)`
- **为什么只看前两项**：排序去重后 `keys[i]` 只可能和 `keys[i-1]` 冲突(`keys[i-2] ≤ keys[i]−2`,必不相邻),故 `dp` 仅依赖 `dp[i-1]`、`dp[i-2]`。
- **复杂度**：时间复杂度 `O(m log m)`(`m` 为 element 数组中不同值的个数)，空间复杂度 `O(m)`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

import collections


def maxEscapeGameScore(elements):
    freq = collections.defaultdict(int)
    for element in elements:
        freq[element] += 1

    keys = sorted(freq.keys())
    m = len(keys)
    dp = [0] * len(keys); dp[0] = keys[0] * freq[keys[0]]
    for i in range(1, m):
        dp[i] = max(dp[i - 1], keys[i] * freq[keys[i]])
        if i >= 2:
            dp[i] = max(dp[i], dp[i - 2] + keys[i] * freq[keys[i]])
        if keys[i] - keys[i - 1] >= 2:
            dp[i] = max(dp[i], dp[i - 1] + keys[i] * freq[keys[i]])
    return dp[-1]


if __name__ == '__main__':
    print(maxEscapeGameScore([5, 6, 6, 4, 11]))  # 27
    print(maxEscapeGameScore([1, 2, 3, 4]))      # 6
    print(maxEscapeGameScore([3, 4, 4, 4]))      # 12
```
