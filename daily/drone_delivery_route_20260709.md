---
title: 2026-07-09 · Drone Delivery Route
parent: 算法每日一题
nav_order: 20260709
permalink: /daily/drone_delivery_route_20260709/
published_at: "2026-07-09 20:28:47"
---

# Amazon - Drone Delivery Route

## Problem
Amazon is expanding its drone delivery network of `m` hubs arranged in a **circular ring** — Hub 1 is adjacent to Hub m.
A drone can move to either adjacent hub, and the time to travel from Hub `i` to a neighbor is `transitionTime[i]`.

Given `requestedHubs` (length `n`), a sequence of hubs that must be visited **in the given order**, and starting from **Hub 1**, return the minimum total travel time to fulfill all requests. Use 1-based indexing.


## Constraints
```
- m hubs on a ring; Hub 1 is adjacent to Hub m
- transitionTime has length m; transitionTime[i] = time to leave Hub i toward EITHER neighbor
  ⇒ the cost is decided by the hub you DEPART from — it is directional, NOT an undirected edge weight
- requestedHubs has length n; hubs must be visited in the given order; the drone starts at Hub 1
- 1-based indexing
```


## Examples

| # | Input                                                        | Output | Note                                                                                     |
|---|--------------------------------------------------------------|--------|------------------------------------------------------------------------------------------|
| 1 | transitionTime = [3,2,1]<br/>requestedHubs = [1,3,3,2]       | 4      | 1→3 逆时针 1 步 = transitionTime[1]=3；3→2 = transitionTime[3]=1；共 3+1 = 4               |
| 2 | transitionTime = [10,1]<br/>requestedHubs = [1,2,1,2,1]      | 22     | m=2 方向不对称：1→2 = transitionTime[1]=10，2→1 = transitionTime[2]=1；10+1+10+1 = 22       |
| 3 | transitionTime = [1,1,1,1]<br/>requestedHubs = [1,4,1]       | 2      | 直接跨 Hub4↔Hub1 的环边，每步 1；顺时针绕 3 步更劣，故 1+1 = 2                              |
| 4 | transitionTime = [4,1,1,1,5]<br/>requestedHubs = [1,4,2,5,3] | 17     | m=5 多段顺/逆混合：1→4 顺 6，4→2 逆 2，2→5 顺 3，5→3 逆 6；共 6+2+3+6 = 17                   |


## Knowledge Points
- 前缀和 + 贪心


## Solution

**直观思路**  
- 无人机必须按 `requestedHubs` 的顺序依次到达各 hub。相邻两个目标 hub 之间，就是一次「环上两点最短路」，且各段互相独立 —— 把每段的最小代价相加即为答案。

**核心洞察（也是本题最容易读错的地方）**
- 成本由「离开的源 hub」决定，是**有方向**的：从 hub `i` 去任一相邻 hub 都花 `transitionTime[i]`。同一条边 `2↔3`，走 `2→3` 花 `transitionTime[2]`、走 `3→2` 花 `transitionTime[3]`，两者可以不同。若按无向边权理解，官方样例会算成 3 而非 4。
- 环上两点只有顺时针、逆时针两条弧；权非负 ⇒ 不会绕回头，最短路必是两条弧之一，取 `min` 即可。
- 逐段贪心为何全局最优：走完一段后无人机恰好停在目标 hub，不携带任何影响后续的状态 ⇒ 每段独立最小化即全局最小。

**步骤**
1. **断环成链**：把 `transitionTime` 复制一份得长度 `2m` 的数组，跨越 Hub m↔Hub 1 的弧就变成连续区间，无需特判绕圈。
2. **预处理前缀和**：
   - 顺时针 `pre_sum_forward`：`start → target` 的顺时针弧 = `pre_sum_forward[target] − pre_sum_forward[start]`（若 `start > target`，先 `target += m`）。
   - 逆时针 `pre_sum_backward`：逆时针弧同理（若 `start < target`，先 `start += m`）。
3. 遍历 `requestedHubs`，维护当前 hub `cur_hub`（初值 1）：目标 == `cur_hub` 则代价 0 跳过；否则 O(1) 取 `min(顺时针弧, 逆时针弧)` 累加，并更新 `cur_hub`。

**复杂度**
预处理 O(m)，每段查询 O(1)，总 **O(m + n)**；与绕圈次数、站点规模无关。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

def getMinimumDroneTime(transitionTime, requestedHubs):
    m, n = len(transitionTime), len(requestedHubs)

    # break the ring into a chain so wrap-around arcs become contiguous
    transition_time_tmp = transitionTime * 2

    # clockwise prefix sum: forward arc(start->target) = pre_sum_forward[target] - pre_sum_forward[start]
    pre_sum_forward = [0] * (2 * m + 1)
    for i in range(2 * m - 1):
        pre_sum_forward[i + 2] = pre_sum_forward[i + 1] + transition_time_tmp[i]

    # counter-clockwise prefix sum for the backward arc
    pre_sum_backward = [0] * (2 * m + 1)
    for i in range(2 * m - 1, 0, -1):
        pre_sum_backward[i] = pre_sum_backward[i + 1] + transition_time_tmp[i]

    cur_hub, res = 1, 0
    for i in range(n):
        if requestedHubs[i] == cur_hub:          # already there, cost 0
            continue

        # clockwise arc
        start, target = cur_hub, requestedHubs[i]
        if start > target:
            target += m
        cur_min = pre_sum_forward[target] - pre_sum_forward[start]

        # counter-clockwise arc
        start, target = cur_hub, requestedHubs[i]
        if start < target:
            start += m
        cur_min = min(cur_min, -(pre_sum_backward[start] - pre_sum_backward[target]))

        res += cur_min
        cur_hub = requestedHubs[i]
    return res


if __name__ == '__main__':
    print(getMinimumDroneTime([3, 2, 1], [1, 3, 3, 2]))     # 4
    print(getMinimumDroneTime([10, 1], [1, 2, 1, 2, 1]))    # 22
    print(getMinimumDroneTime([1, 1, 1, 1], [1, 4, 1]))     # 2
    print(getMinimumDroneTime([4, 1, 1, 1, 5], [1, 4, 2, 5, 3]))  # 17
```
