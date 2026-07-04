---
title: Reconstruct the Journey
parent: Capital One
grand_parent: 按公司刷题
nav_order: 1
---

# Capital One - Reconstruct the Journey

## Problem
A traveler visited a series of unique landmarks on a journey. Unfortunately, their travel journal was damaged, and they can no longer remember the exact order of their visits. However, they do have a collection of photos, each showing exactly two landmarks that were visited consecutively. Either landmark could have been visited first.

Given the collection of photos represented as pairs of landmark IDs in `travelPhotos`, help the traveler reconstruct the complete journey. Each landmark was visited exactly once, and for every consecutive pair of landmarks in the journey, there exists a photo containing both landmarks.

You may reconstruct the journey in either forward or reverse order; both are considered correct.


## Constraints
```
2 <= n <= 2 x 10⁵, where n = number of landmarks
travelPhotos.length == n - 1
All landmark IDs are distinct.
It is guaranteed that the photos describe exactly one valid journey
(i.e. they form a single simple path; no cycles, no branches).
```


## Examples

| # | Input                                              | Output            | Note                                                                 |
|---|----------------------------------------------------|-------------------|----------------------------------------------------------------------|
| 1 | travelPhotos = [[3, 5], [1, 4], [2, 4], [1, 5]]    | [3, 5, 1, 4, 2]   | 端点 `3` 与 `2` 度为 1；从 `3` 沿边走出 `3→5→1→4→2`，逆序也对。       |
| 2 | travelPhotos = [[10, 20], [30, 20]]                | [10, 20, 30]      | `20` 度为 2 是中间点，`10`、`30` 是两个端点；`[30,20,10]` 同样合法。 |


## Knowledge Points
- 图论建模-路径图 + DFS/BFS


## Solution
- **建模转化**：
  - 每张照片是一对相邻地标，方向未知 → 看成一条**无向边**；
  - 每个地标是一个**节点**。一次「每个地标恰好走一遍、相邻地标都有照片」的旅程，本质就是一条**简单路径**。

- **关键观察**：在一条链上，
  - 两个**端点**只和一个邻居相连 → **度数为 1**；
  - 中间的每个点都夹在前后两个地标之间 → **度数为 2**。
  - 这样的图又叫做路径图（path graph）

  因此只要找到任意一个**度为 1 的点**作为起点，就能从链的一头开始往另一头走。

- **如何走**：从起点出发，每一步看当前节点的邻居，**只要不是上一步来的那个点就往它走**（中间点恰好有两个邻居：来路 + 去路；端点只有一个邻居）。一直走到收集满所有地标为止。题目允许正序/逆序，所以从哪个端点出发都行。

- **步骤**：  
  Step 1. 遍历 `travelPhotos`，建无向**邻接表** `adj`。  
  Step 2. 找一个 `len(adj[node]) == 1` 的节点作为 `start`（端点）。  
  Step 3. 从 `start` 开始走，用 `prev` 记录上一步，每次选 `!= prev` 的邻居前进，把经过的节点依次加入结果。  
  Step 4. 收集到 `n` 个节点即得到完整旅程。

- **复杂度**：时间复杂度 O(n)，空间复杂度 O(n)。


## AC Code
```python
import collections


def solution(travelPhotos):
    n = len(travelPhotos)
    graph = collections.defaultdict(list)
    deg = collections.defaultdict(int)
    for i in range(n):
        u, v = travelPhotos[i]
        graph[u].append(v); graph[v].append(u)
        deg[u] += 1; deg[v] += 1

    que = collections.deque([])
    start = 0
    for cur_node in deg:
        if deg[cur_node] == 1:
            que.append(cur_node)
            start = cur_node
            break

    vis = {start}
    res = []
    while que:
        cur_node = que.popleft()
        res.append(cur_node)
        for nxt_node in graph[cur_node]:
            if nxt_node not in vis:
                que.append(nxt_node)
                vis.add(nxt_node)
    return res


if __name__ == '__main__':
    print(solution([[3, 5], [1, 4], [2, 4], [1, 5]]))  # [3, 5, 1, 4, 2], or [2, 4, 1, 5, 3]
    print(solution([[9, 4], [2, 7], [1, 4], [9, 2]]))  # [1, 4, 9, 2, 7], or [7, 2, 9, 4, 1]
    print(solution([[8, 1], [9, 3], [5, 8], [1, 9]]))  # [5, 8, 1, 9, 3], or [3, 9, 1, 8, 5]
    print(solution([[7, 2]]))  # [7, 2], or [2, 7]
```
