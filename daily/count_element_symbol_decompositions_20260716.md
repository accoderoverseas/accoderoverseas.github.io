---
title: 2026-07-16 · Count Element Symbol Decompositions
parent: 算法每日一题
nav_order: 20260716
permalink: /daily/count_element_symbol_decompositions_20260716/
published_at: "2026-07-16 10:28:54"
---

# Google - Count Element Symbol Decompositions

## Problem
Given a collection of chemical element `symbols` and a string `word`, return the number of ways to split the entire word into a sequence of the supplied symbols.

Every character in `word` must be used exactly once, symbols may be reused, and matching is case-insensitive. Symbols that differ only by letter case are treated as the same symbol.


## Constraints
```text
1 <= m <= 1000, where m is the length of symbols.
1 <= n <= 1000, where n is the length of word.
Maximum length of every symbol is 10.
```


## Examples

| # | Input | Output | Note |
|---|---|---:|---|
| 1 | `symbols = ["P", "H", "Y", "S", "I", "C", "Si", "Cs"]`<br/>`word = "Physics"` | `4` | 四种拆分为 `P-H-Y-Si-C-S`、`P-H-Y-Si-Cs`、`P-H-Y-S-I-C-S`、`P-H-Y-S-I-Cs` |
| 2 | `symbols = ["H", "h"]`<br/>`word = "H"` | `1` | 大小写去重后，唯一拆分为单个符号 `H` |
| 3 | `symbols = ["C", "O", "Co", "N"]`<br/>`word = "CoX"` | `0` | 无解 |


## Knowledge Points
- 哈希表 + 动态规划-计数DP


## Solution
- **状态定义**：令 `dp[i]` 表示前缀 `word[:i]` 被完整拆分的方案数。
- **初始化**：`dp[0] = 1`，表示空前缀有一种拆分方式，即不选择任何符号。
- **状态转移**：枚举前缀终点 `i` 和每个符号 `symbol`。若 `symbol` 与 `word` 中以 `i` 结尾的后缀匹配，就可以把它接到前面每一种合法拆分之后：`dp[i] += dp[i-len(symbol)]`。
- **预处理**：先将 `word` 和所有符号统一转成小写，并使用集合去重，避免重复符号导致同一种方案被多次统计。
- **答案**：`dp[n]`。只有完整覆盖整个 `word` 的拆分才会计入答案。
- **注意事项**：`dp[0]` 必须设为 `1`；空字符串的答案也是 `1`；无效的空符号应过滤，否则无法表示一次有效的拆分推进。
- **复杂度**：设去重后有 `m` 个符号，最大长度为 `L`。时间复杂度为 `O(n × m × L)`，空间复杂度为 `O(n + m × L)`。化学元素符号长度通常很短，因此匹配开销较小。


## AC Code
```python
# ------------------------------------------------------------
#  ac_coder_tutor  ·  Daily Algorithm Problem (OA/VO)
#  RedBook / WeChat: ac_coder_tutor  |  accoderoverseas@gmail.com
#  OA/VO breakdowns & CS course tutoring for students abroad
# ------------------------------------------------------------


def solution(symbols, word):
    # 统一大小写并去重；过滤空符号，确保每次转移都会向前推进
    symbols = {symbol.lower() for symbol in symbols if symbol}
    word = word.lower()

    n = len(word)
    dp = [0] * (n + 1)
    dp[0] = 1

    for i in range(1, n + 1):
        for symbol in symbols:
            symbol_len = len(symbol)
            if symbol_len <= i and word[i - symbol_len:i] == symbol:
                dp[i] += dp[i - symbol_len]

    return dp[n]


if __name__ == '__main__':
    print(solution(["P", "H", "Y", "S", "I", "C", "Si", "Cs"], "Physics"))  # 4
    print(solution(["H", "h"], "H"))  # 1
    print(solution(["C", "O", "Co", "N"], "CoX"))  # 0
```
