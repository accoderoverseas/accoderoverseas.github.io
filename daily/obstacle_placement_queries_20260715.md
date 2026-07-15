# TikTok - Obstacle Placement Queries

## Problem
You are given an infinite number line and an array `operations`. Process the operations in order while maintaining the coordinates that contain obstacles.

- `[1, x]`: Place an obstacle at coordinate `x`. Coordinate `x` is guaranteed to contain no obstacle when this operation is performed.
- `[2, x, size]`: Check whether a block of length `size` can begin at coordinate `x`. The block occupies every integer coordinate from `x` through `x + size - 1`. Append `'1'` to the answer if none of these coordinates contains an obstacle; otherwise append `'0'`. This operation only checks feasibility and does not place the block.

Return the binary string formed by the results of all type-2 operations in their original order.


## Constraints
```
- Each operation is either [1, x] or [2, x, size].
- size is a positive integer.
- When [1, x] is processed, coordinate x is guaranteed to contain no obstacle.
- Coordinates may be negative, zero, or positive because the number line is infinite.
- The exact numeric bounds for the number of operations and coordinate values are not specified in the statement.
```


## Examples

| # | Input | Output | Note |
|---|-------|--------|------|
| 1 | `operations = [[2,0,2],[1,1],[2,0,2],[2,2,2]]` | `"101"` | 首次查询 `[0,1]` 可放置；加入障碍物 `1` 后再次查询不可放置；区间 `[2,3]` 仍可放置。 |
| 2 | `operations = [[1,-3],[1,2],[2,-5,2],[2,-4,2],[2,-2,4],[2,1,2]]` | `"1010"` | 依次查询 `[-5,-4]`、`[-4,-3]`、`[-2,1]`、`[1,2]`，其中第二、第四个区间包含障碍物。 |
| 3 | `operations = [[1,0],[2,0,1],[2,-1,1],[2,-1,2],[2,1,1]]` | `"0101"` | 障碍物位于坐标 `0`，用于验证单点区间、负坐标以及跨越 `0` 的查询。 |


## Knowledge Points
- 二分查找 + 有序集合


## Solution
- **核心思路**：查询区间为 `[x, x+size-1]`。只需在有序障碍物集合中找到第一个大于等于 `x` 的障碍物：若它不超过区间右端点，则区间被阻挡；否则可以放置。
- **步骤**：
  - Step 1. 使用 `SortedList` 按坐标维护所有障碍物。
  - Step 2. 遇到 `[1, x]`，将 `x` 插入有序集合。
  - Step 3. 遇到 `[2, x, size]`，用 `bisect_left(x)` 找到第一个大于等于 `x` 的障碍物，并判断它是否位于 `[x, x+size-1]` 内。
- **正确性**：若找到的第一个障碍物已经超过右端点，后续障碍物只会更大，因此整个查询区间一定没有障碍物。
- **踩坑**：
  - 区间右端点是 `x + size - 1`，不是 `x + size`。
  - 障碍物坐标可能为 `0`，不能写成 `if target`；应判断 `target is not None`，或直接使用下标是否越界来判断。
  - 查询操作只检查能否放置，不会真的加入一个块。
- **复杂度**：设当前已有 `m` 个障碍物，每次添加和查询均为 `O(log m)`，总空间复杂度为 `O(m)`。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------

from sortedcontainers import SortedList


def obstaclePlacementQueries(operations):
    obstacles = SortedList()
    res = []

    for operation in operations:
        op, x = operation[0], operation[1]

        if op == 1:
            obstacles.add(x)
        else:
            size = operation[2]
            index = obstacles.bisect_left(x)
            right = x + size - 1

            if index < len(obstacles) and obstacles[index] <= right:
                res.append("0")
            else:
                res.append("1")

    return "".join(res)


if __name__ == '__main__':
    print(obstaclePlacementQueries(
        [[2, 0, 2], [1, 1], [2, 0, 2], [2, 2, 2]]
    ))  # "101"

    print(obstaclePlacementQueries(
        [[1, -3], [1, 2], [2, -5, 2], [2, -4, 2], [2, -2, 4], [2, 1, 2]]
    ))  # "1010"

    print(obstaclePlacementQueries(
        [[1, 0], [2, 0, 1], [2, -1, 1], [2, -1, 2], [2, 1, 1]]
    ))  # "0101"
```
