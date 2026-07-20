---
title: 2026-07-20 · Maximum Reward Points
parent: 算法每日一题
nav_order: 20260720
permalink: /daily/maximum_reward_points_20260720/
published_at: "2026-07-20 19:50:27"
---

# Microsoft - Maximum Reward Points

## Problem
Two interns are assigned to complete a total of `n` tasks. Each task must be completed by exactly one of them.  
For task `i`, the first intern earns `reward_1[i]` points and the second intern earns `reward_2[i]` points.  
The first intern must complete **exactly `k`** tasks (any `k` of the `n` tasks); the second intern completes the remaining tasks.  
Return the **maximum possible combined reward points**.


## Constraints
```
- 1 ≤ n ≤ 10^5
- 0 ≤ k ≤ n
- 1 ≤ reward_1[i], reward_2[i] ≤ 10^4
```


## Examples

| # | Input                                                                 | Output | Note                                                                                     |
|---|-----------------------------------------------------------------------|--------|------------------------------------------------------------------------------------------|
| 1 | k = 3<br/>reward_1 = [5, 4, 3, 2, 1]<br/>reward_2 = [1, 2, 3, 4, 5]     | 21     | 差值 = [4, 2, 0, −2, −4]；前 3 大(task0,1,2)取 reward_1 得 5+4+3，其余取 reward_2 得 4+5 = 21 |
| 2 | k = 2<br/>reward_1 = [10, 1, 5, 8]<br/>reward_2 = [2, 9, 3, 4]          | 30     | 差值 = [8, −8, 2, 4]；前 2 大(task0,3)取 reward_1 得 10+8，其余取 reward_2 得 3+9 = 30        |
| 3 | k = 3<br/>reward_1 = [7, 2, 9, 4, 6]<br/>reward_2 = [1, 8, 2, 5, 3]     | 35     | 差值 = [6, −6, 7, −1, 3]；前 3 大(task2,0,4)取 reward_1 得 9+7+6，其余取 reward_2 得 5+8 = 35 |
| 4 | k = 0<br/>reward_1 = [5, 5, 5]<br/>reward_2 = [1, 2, 3]                 | 6      | 边界：k=0，第一人不做任何任务，全部归第二人 = sum(reward_2) = 1+2+3 = 6                        |


## Knowledge Points
- 贪心 + 排序


## Solution
- **直观思路**：要从 `n` 个任务里恰好挑 `k` 个给第一人、其余给第二人。枚举所有组合是 `C(n, k)`，指数级，不可行。
- **最优解切入点**：先假设**所有任务都归第二个实习生**，基础分为 `sum(reward_2)`。把任务 `i` 改派给第一个人，总分的变化量恰好是 `reward_1[i] − reward_2[i]`。既然必须**恰好改派 k 个**，为使总分最大，就选差值最大的前 `k` 个。各任务相互独立、无耦合约束 ⇒ **贪心取 top-k 即最优**。
- **步骤**：
  - Step 1. 按 `reward_1[i] − reward_2[i]` **降序排序**。
  - Step 2. 排序后前 `k` 个取 `reward_1`，其余取 `reward_2`，累加即为答案。
- **踩坑**：
  - `k = 0` / `k = n` 边界：排序后「前 k 个 / 后 n−k 个」自然覆盖，无需额外特判。
  - 排序键是**差值**而非 `reward_1`，仅按 `reward_1` 排序会 WA（例如 reward_2 很大的任务应优先留给第二人）。
- **复杂度**：时间 `O(n log n)`，空间 `O(n)`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

def getMaximumRewardPoints(k, reward_1, reward_2):
    n = len(reward_1)
    reward = []
    for i in range(n):
        reward.append([reward_1[i], reward_2[i]])

    # 按 reward_1 - reward_2 的差值降序排序
    reward = sorted(reward, key=lambda x: x[0] - x[1], reverse=True)

    res = 0
    for i in range(n):
        if i < k:          # 差值最大的前 k 个任务交给第一个实习生
            res += reward[i][0]
        else:              # 其余任务交给第二个实习生
            res += reward[i][1]
    return res


if __name__ == '__main__':
    print(getMaximumRewardPoints(3, [5, 4, 3, 2, 1], [1, 2, 3, 4, 5]))  # 21
    print(getMaximumRewardPoints(2, [10, 1, 5, 8], [2, 9, 3, 4]))       # 30
    print(getMaximumRewardPoints(3, [7, 2, 9, 4, 6], [1, 8, 2, 5, 3]))  # 35
    print(getMaximumRewardPoints(0, [5, 5, 5], [1, 2, 3]))              # 6
```
