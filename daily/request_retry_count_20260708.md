---
title: 2026-07-08 · Request Retry Count
parent: 算法每日一题
nav_order: 20260708
permalink: /daily/request_retry_count_20260708/
published_at: "2026-07-08 20:00:00"
---


# IBM - Request Retry Count

## Problem

You are given an integer `gap`, the maximum allowed time difference (in seconds) to consider a retry, and two arrays of equal length `n`:

- `requestIds[i]`: the request ID of the `i`-th log
- `timestamps[i]`: the time of the `i`-th log, **sorted in non-decreasing order**

For a single request ID, look at its logs in time order. A **retry** occurs when two **consecutive** logs of that request ID have a time difference of **at most `gap`**.  

Return the **total number of retries** across all request IDs.


## Constraints

```
1 ≤ n ≤ 2 * 10⁶
1 ≤ gap ≤ 10⁹
0 ≤ timestamps[i] ≤ 10⁹
timestamps is sorted in non-decreasing order
requestIds[i] is a string identifier
```


## Examples

| # | Input | Output | Note |
|---|-------|--------|------|
| 1 | gap = 10<br/>requestIds = ["r1","r1","r1","r2","r2"]<br/>timestamps = [100,105,200,300,302] | 2 | r1[100,105,200]: (100,105) 差 5≤10 ✓、(105,200) 差 95 ✗ → 1；r2[300,302]: 差 2 ✓ → 1；共 2 |
| 2 | gap = 50<br/>requestIds = ["x","x","x","x"]<br/>timestamps = [0,40,80,200] | 2 | (0,40)40 ✓、(40,80)40 ✓、(80,200)120 ✗ → 2；断裂只影响其后 |
| 3 | gap = 1000<br/>requestIds = ["a","b","c","d"]<br/>timestamps = [1,2,3,4] | 0 | 每个 id 只有 1 条日志，无相邻对 → 0 |


## Knowledge Points
- 哈希表 + 贪心


## Solution
- **直观思路**：把每个 requestId 的日志时间收集起来，桶内按时间顺序两两相邻比较，差 ≤ gap 就计一次 retry，全部累加即答案。
- **关键理解**："consecutive" 指**同一 id 时间上相邻**的两条，而非原数组下标相邻；不同 id 之间互不比较。
- **步骤**：
  - Step 1. 用 `dict[requestId] -> list` 收集时间戳；因原数组按时间非递减依次 append，桶内即已有序（代码里的 `sort` 属冗余）。
  - Step 2. 每个桶遍历相邻对，`t[i+1] - t[i] ≤ gap` 则 `res += 1`。
  - Step 3. 返回所有桶的累加值。
- **复杂度**：时间复杂度 `O(n)`（输入有序，冗余 sort 对有序数据仍为线性），空间复杂度 `O(n)`。


## AC Code

```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

import collections


def getRetryCount(gap, requestIds, timestamps):
    n = len(requestIds)
    request_times = collections.defaultdict(list)
    for i in range(n):
        request_times[requestIds[i]].append(timestamps[i])

    res = 0
    for request_id in request_times:
        request_times[request_id].sort()
        for i in range(len(request_times[request_id]) - 1):
            if request_times[request_id][i + 1] - request_times[request_id][i] <= gap:
                res += 1
    return res


if __name__ == '__main__':
    print(getRetryCount(10, ["r1", "r1", "r1", "r2", "r2"], [100, 105, 200, 300, 302]))  # 2
    print(getRetryCount(50, ["x", "x", "x", "x"], [0, 40, 80, 200]))  # 2
    print(getRetryCount(1000, ["a", "b", "c", "d"], [1, 2, 3, 4]))  # 0
    print(getRetryCount(20, ["r", "r", "r"], [100, 120, 141]))  # 1
    print(getRetryCount(10 ** 9, ["r", "r", "r", "r"], [10, 10, 10, 10 ** 9]))  # 3
```
