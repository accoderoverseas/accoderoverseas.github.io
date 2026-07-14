---
title: 墨尔本大学（University of Melbourne, UniMelb）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 6
permalink: /cs-courses/course-map/australia/unimelb/
published_at: "2026-07-14 21:29:24"
---

<style>
/* 课程号-课程名统一紫色加粗（仅本页生效） */
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 墨尔本大学（University of Melbourne, UniMelb）

UniMelb 计算机课程主要采用 **COMP** 编码。下方按照学习方向整理本科与研究生的**核心 / 高频课程详解**，并单独标明 2026 Semester 2（26S2）是否开设，方便同学区分“2026 全年课程”与“26S2 可选课程”。

> 说明：本页的**课程名称、课程简介、主要知识点、2026 开课学期与考核信息**已于 **2026-07-14** 逐项对照 UniMelb **2026 Handbook**；“2026 S2 开课”指 Handbook 明确列出 **Semester 2, On Campus (Parkville)**。**整体难度与建议学习路线**为主观学习经验参考。Handbook 的 assessment 是选课阶段的官方口径，具体日期、题型和提交要求仍以开学后的 Canvas subject guide 为准。

## 26S2 开课状态速查

| 专题 | 2026 S2 开设 | 2026 S2 不开设 |
| --- | --- | --- |
| 编程 · 软件工程 · 项目 | COMP10001、COMP90059 | — |
| 算法 · 数据结构 · 理论 | COMP10002、COMP20003、COMP20005、COMP90038 | COMP20007、COMP90077（均仅 S1） |
| 计算机系统 · 体系结构 | COMP90015 | COMP30023、COMP90020（均仅 S1） |
| 数据库 · 信息系统 | COMP90050 | — |
| 人工智能 · 机器学习 | COMP90049、COMP90051、COMP90086 | COMP30024、COMP30027、COMP90042（均仅 S1） |
| 数据科学 · 数据分析 | COMP20008 | — |

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### `COMP10001` — [Foundations of Computing（计算基础）](https://handbook.unimelb.edu.au/2026/subjects/comp10001)

- **课程简介**：面向零基础或编程经验很少的本科生，以 **Python** 训练用程序处理、分析和可视化数据的能力。重点不只是记语法，而是把问题拆成可实现、可测试的步骤。
- **主要知识点**：变量与表达式、分支与循环、函数与模块、字符串、列表 / 元组 / 字典、文件与结构化数据处理、基础算法思维、程序测试与调试。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus，教学期为 **2026-07-27 至 2026-10-25**。
- **整体难度**：⭐⭐⭐☆☆ — 对零基础友好，但每周进度连续；后半段综合题要求能独立读题、拆解并调试程序。
- **成绩组成**（2026）：两次编程作业 **30%** + Mid-semester Test **10%** + Worksheets **10%** + 期末考试 **50%**；期末考试设 hurdle。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp10001/assessment)。
- **建议学习路线**：每周把 lecture 示例关掉后重写一遍，再用 2—3 道小题练控制流、函数和容器。作业先写输入输出与测试样例，再补实现；期末复习要练“读代码、预测输出、限时写函数”，不能只看笔记。

#### `COMP90059` — [Introduction to Programming（编程导论）](https://handbook.unimelb.edu.au/2026/subjects/comp90059)

- **课程简介**：面向无编程背景的研究生，以 **Python** 和高级过程式编程讲解如何处理、转换与可视化静态结构化数据。Handbook 明确说明该课不适合已有较强编程经验的学生。
- **主要知识点**：基础编程结构、基本数据结构、抽象与模块、算法化问题求解、数据操作与转换、程序组织和调试。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐☆☆ — 知识从零起步，但研究生课节奏快，数据处理任务会很快把语法、函数和结构化数据综合起来。
- **考核重点**（2026）：以编程作业、阶段性测试 / 练习和期末考核共同检验独立编程能力；权重、时长与 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90059/assessment)。
- **建议学习路线**：前四周先把循环、函数和 Python 容器练熟，再进入数据任务。不要依赖复制代码完成作业；每次提交后都要能不看答案解释变量状态、边界条件和测试策略。

### 算法 · 数据结构 · 理论

#### `COMP10002` — [Foundations of Algorithms（算法基础）](https://handbook.unimelb.edu.au/2026/subjects/comp10002)

- **课程简介**：从入门编程过渡到算法与数据结构的核心课，使用 **C** 语言训练程序设计、动态数据结构、搜索与排序，并开始系统讨论正确性和效率。
- **主要知识点**：C 编译与模块化、指针与动态内存、链表、树、哈希表、递归、搜索与模式匹配、排序、算法效率分析。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐⭐☆ — C 的指针 / 内存管理和第一次系统接触复杂度、树与哈希，是多数同学的主要门槛。
- **成绩组成**（2026）：Problem Sets **5%** + Mid-semester Test **15%** + 两个项目 **40%** + 1.5 小时期末考试 **40%**；项目合计、Mid-semester Test 与期末考试合计均设 hurdle。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp10002/assessment)。
- **建议学习路线**：开课前补 C 的数组、指针、函数和 `malloc/free`。每学一种结构都自己画内存图并手写核心操作；算法题先写不变量与复杂度，再写代码。项目至少预留一周做边界测试和内存检查。

#### `COMP20003` — [Algorithms and Data Structures（算法与数据结构）](https://handbook.unimelb.edu.au/2026/subjects/comp20003)

- **课程简介**：围绕“同一份数据该用什么结构表示、配什么算法”展开，强调算法正确性、渐进与实验性能分析，以及在 **C** 中实现常用数据结构和图算法。
- **主要知识点**：正确性论证、渐进 / 实验复杂度分析、排序与搜索、树、哈希表、图表示、遍历、最短路及其他基础图算法。
- **2026 S2 开课**：**是，且 2026 仅 S2 开设**；Parkville 校区 On Campus，教学期为 **2026-07-27 至 2026-10-25**。
- **整体难度**：⭐⭐⭐⭐☆ — 理论与 C 实现并重；选错结构、复杂度分析不严谨或项目边界条件遗漏，都会明显失分。
- **成绩组成**（2026）：两个编程项目合计 **30%** + Mid-semester Test **10%** + 3 小时期末考试 **60%**；项目部分及测试 / 考试部分设组合 hurdle。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp20003/assessment)。
- **建议学习路线**：先复习 C 指针、结构体与动态内存；每周把树、哈希、图的核心操作从零实现。项目要同时维护正确性测试与复杂度说明；期末按“结构—操作—复杂度—适用场景”做对照表，并限时练伪代码。

#### `COMP20005` — [Intro. to Numerical Computation in C（C 语言数值计算导论）](https://handbook.unimelb.edu.au/2026/subjects/comp20005)

- **课程简介**：用 **C** 学习小规模科学 / 工程计算程序的设计与调试，并理解数值近似、误差和算法选择。它既是编程课，也是数值方法入门课。
- **主要知识点**：C 基础结构、数组与结构体、近似与数值误差、方程求根、线性方程组、曲线拟合与样条、插值 / 外推、数值微分与积分。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐☆☆ — 编程结构比高阶算法课基础，但浮点误差、数值方法与手写 C 程序叠加后，细节较多。
- **成绩组成**（2026）：Assignment 1 **10%** + Assignment 2 **20%** + Mid-semester Test **10%** + 期末考试 **60%**。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp20005/assessment)。
- **建议学习路线**：先把 C 的循环、函数、数组、指针练到不依赖模板；数值算法要同时问“数学上为什么成立”和“浮点环境中是否稳定”。复习时手写短函数，并训练逐步追踪误差和变量状态。

#### `COMP20007` — [Design of Algorithms（算法设计）](https://handbook.unimelb.edu.au/2026/subjects/comp20007)

- **课程简介**：与 COMP20003 同层次但更偏算法设计范式和理论推理，训练在多种候选算法 / 数据结构之间，根据正确性与复杂度作出选择，并用 C 实现多模块程序。
- **主要知识点**：高级排序与搜索、图算法、贪心法、动态规划、中级数据结构、复杂度比较、正确性分析、多模块 C 程序。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐☆ — 重点不在背算法名称，而在把新问题映射到设计范式、证明正确并写出可分析的方案。
- **成绩组成**（2026 S1）：Project 1 **10%** + Mid-semester Test **10%** + Project 2 **20%** + 3 小时期末考试 **60%**。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp20007/assessment)。
- **建议学习路线**：26S2 不要误选；计划后续 S1 修读时，可先用 COMP10002 打好 C 与基础算法。学习时为每道题固定写“状态 / 子问题、选择规则、正确性、复杂度”四步，避免只会套模板。

#### `COMP90038` — [Algorithms and Complexity（算法与复杂度）](https://handbook.unimelb.edu.au/2026/subjects/comp90038)

- **课程简介**：研究生算法核心课，系统训练如何评估和设计计算高效的程序。课程把经典数据结构、算法设计范式与计算能力的理论边界放在同一框架中。
- **主要知识点**：渐进复杂度与经验分析、队列 / 树 / 优先队列 / 图、排序与搜索、暴力法、分治、动态规划、贪心、时空权衡、算法能力边界。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐⭐☆ — 内容密度高，需要同时完成伪代码设计、复杂度推导和形式化论证；零算法基础直接修读压力很大。
- **成绩组成**（2026）：两次 Assignment 各 **15%** + Weekly Quizzes **10%** + 3 小时期末考试 **60%**；考试及总评设通过要求。见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90038/assessment)。
- **建议学习路线**：开课前复习离散数学、递归与 Big-O。每周把算法用小例子手推，再脱离代码写伪代码和复杂度；动态规划和图算法必须按题型持续练，期末前才集中刷题通常来不及。

#### `COMP90077` — [Advanced Algorithms and Data Structures（高级算法与数据结构）](https://handbook.unimelb.edu.au/2026/subjects/comp90077)

- **课程简介**：面向大规模、实时数据场景的高级课，讨论标准数据结构与算法无法良好扩展时，如何选择和设计更先进的算法工具，并要求能够高效、正确地实现。
- **主要知识点**：高级算法设计原则、高级数据结构、可扩展算法、复杂问题的结构选择、正确性与效率分析、理论到实现的转换。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。S1 为 Parkville On Campus，且 Handbook 注明需获得 coordinator permission。
- **整体难度**：⭐⭐⭐⭐⭐ — 抽象度和数学推理要求显著高于 COMP90038，题目更开放，适合已有扎实算法与证明基础的同学。
- **考核重点**（2026）：以书面算法作业和期末考核检验高级算法设计、分析与论证；精确权重和 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90077/assessment)。
- **建议学习路线**：先把 COMP90038 或同等算法基础学扎实，再补图算法、概率与证明写作。每周先独立尝试 exercise，再对照解答复盘“关键观察”来自哪里；26S2 不开，需按 S1 规划。

### 计算机系统 · 体系结构

#### `COMP30023` — [Computer Systems（计算机系统）](https://handbook.unimelb.edu.au/2026/subjects/comp30023)

- **课程简介**：带学生理解计算机“底层如何工作”，把计算机组成、操作系统、网络和安全放到同一系统视角中，并通过编程任务把硬件 / 软件接口落地。
- **主要知识点**：计算机组织与硬件 / 软件接口、内存层次与虚拟内存、中断、进程与调度、文件系统、同步、网络协议、客户端—服务器程序、基础密码学与系统安全。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐☆ — 知识面宽，既要理解 OS / 网络概念，也要完成偏底层的程序设计和综合题。
- **考核重点**（2026）：项目、阶段测试与期末考试共同覆盖系统编程、操作系统和网络内容；精确权重与 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp30023/assessment)。
- **建议学习路线**：提前熟悉 C、Linux 命令行、进程和 socket 基础。学习时画出“CPU—内存—OS—进程—网络”的调用链；项目从最小可运行版本开始，并用日志和抓包工具定位问题。

#### `COMP90015` — [Distributed Systems（分布式系统）](https://handbook.unimelb.edu.au/2026/subjects/comp90015)

- **课程简介**：从 Web、Email、DNS 等真实系统出发，理解分布式架构、通信和服务设计原则，并完成较复杂的分布式应用实现。
- **主要知识点**：分布式系统特征与系统模型、进程间通信、远程调用、间接通信、OS 支持、分布式对象 / 组件、Web Services、安全、分布式文件系统、命名服务。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐⭐☆ — 最大难点是并发、网络故障和跨进程状态让调试不再可重复；项目工程量通常高于普通单机程序。
- **考核重点**（2026）：以分布式应用项目、书面分析和受监督测试 / 期末考核评价设计与实现能力；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90015/assessment)。
- **建议学习路线**：先补网络、进程 / 线程、并发与异常处理；项目要从协议、消息格式和失败场景开始设计。尽早加入超时、重试、幂等与日志，不要等功能完成后才处理故障。

#### `COMP90020` — [Distributed Algorithms（分布式算法）](https://handbook.unimelb.edu.au/2026/subjects/comp90020)

- **课程简介**：比 COMP90015 更偏算法与理论，研究同步 / 异步网络中的进程如何协调资源、形成一致结论并维护全局状态。
- **主要知识点**：同步与异步网络算法、时钟同步、互斥、共识、复制与一致性、分布式数据结构、死锁检测、Leader Election、Global Snapshot。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐⭐ — 需要在并发执行、消息延迟和故障假设下做严格推理，证明与论文阅读压力较高。
- **考核重点**（2026）：书面报告、课堂展示和算法分析是重要组成，具体权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90020/assessment)。
- **建议学习路线**：先修分布式系统或具备同等背景，再复习图、离散数学和证明。为每个算法明确系统模型、故障模型、安全性与活性；26S2 不开，需要按 S1 安排。

### 数据库 · 信息系统

#### `COMP90050` — [Advanced Database Systems（高级数据库系统）](https://handbook.unimelb.edu.au/2026/subjects/comp90050)

- **课程简介**：研究大规模、多用户数据库如何同时保证可靠性与处理效率，重点从“会写 SQL”提升到理解事务、并发、恢复和高性能数据库技术。
- **主要知识点**：高性能数据库、事务处理、并发控制与隔离、ACID、故障恢复、索引、查询 / 存储性能、结构化与非结构化数据、大规模数据处理。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2），部分实验需自带可运行 MySQL Community Edition 的设备。
- **整体难度**：⭐⭐⭐⭐☆ — 难点在事务交错、隔离级别、恢复过程和性能权衡，不能只靠记定义。
- **考核重点**（2026）：数据库分析 / 实践作业与期末考核共同覆盖性能、可靠性和事务机制；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90050/assessment)。
- **建议学习路线**：先掌握关系模型、SQL、索引和基础数据库设计。对并发控制和恢复要画时间线逐步推演；实验阶段建立可复现数据集，用执行计划比较不同索引与查询写法。

### 人工智能 · 机器学习

#### `COMP30024` — [Artificial Intelligence（人工智能）](https://handbook.unimelb.edu.au/2026/subjects/comp30024)

- **课程简介**：本科 AI 主干课，从智能体和问题求解出发，覆盖搜索、推理、知识表示、概率与学习，建立经典 AI 方法的整体框架。
- **主要知识点**：智能体、状态空间搜索与启发式、问题求解、逻辑与知识表示、概率推理、机器学习，以及可能涉及的博弈、规划、机器人和自然语言应用。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐☆ — 范围广，搜索、概率与形式推理切换频繁；既考概念，也考把问题建模为可求解状态空间。
- **考核重点**（2026）：编程项目与期末考试共同评价搜索、推理和学习方法；精确权重与 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp30024/assessment)。
- **建议学习路线**：先修好算法与数据结构，补概率基础。搜索题统一写状态、动作、代价、启发式和终止条件；不要只背 A* / minimax 名称，要能手推搜索过程并解释正确性。

#### `COMP30027` — [Machine Learning（机器学习）](https://handbook.unimelb.edu.au/2026/subjects/comp30027)

- **课程简介**：本科机器学习主干课，讲解如何从数据中学习可泛化的预测或结构，并兼顾算法假设、模型评价、可解释性与实际实现。
- **主要知识点**：监督 / 无监督学习、概率与熵、线性 / 逻辑回归、朴素贝叶斯、决策树、SVM、混合模型、HMM、感知机与神经网络、降维、模型评价与解释。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐☆ — 公式、概率、模型假设和代码实验并行；若线代与概率基础薄弱，后半段会明显吃力。
- **考核重点**（2026）：数据建模项目、阶段性测试与期末考试共同评价理论理解、实现和模型分析；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp30027/assessment)。
- **建议学习路线**：开课前补概率、线代、Python / NumPy。每个模型都整理“目标函数—假设—训练—预测—评价—失效场景”，并从零实现一个简化版，再使用库验证结果。

#### `COMP90042` — [Natural Language Processing（自然语言处理）](https://handbook.unimelb.edu.au/2026/subjects/comp90042)

- **课程简介**：研究生 NLP 核心课，训练对文本数据应用语言处理与信息检索算法，并能依据研究结果开发和评价计算语言模型。
- **主要知识点**：文本规范化、句界识别、词性标注、n-gram 语言模型、文本分类、序列模型、检索与排序、机器翻译、文本系统的实现和评价。
- **2026 S2 开课**：**否；2026 仅 S1 开设**。
- **整体难度**：⭐⭐⭐⭐☆ — 同时需要 Python、概率、算法和研究论文阅读；项目不仅要跑模型，还要解释实验设计与评价。
- **考核重点**（2026）：项目、研究型表达 / 展示与期末考核共同评价 NLP 方法的实现和分析；精确权重与 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90042/assessment)。
- **建议学习路线**：先掌握概率、机器学习和 Python 文本处理。建立从预处理、特征 / 表示、模型到指标的完整 pipeline；实验报告必须保留 baseline、误差分析和可复现设置。

#### `COMP90049` — [Introduction to Machine Learning（机器学习导论）](https://handbook.unimelb.edu.au/2026/subjects/comp90049)

- **课程简介**：面向研究生的机器学习基础课，从统计原则出发讨论如何做准确、高效、可解释且稳健的数据推断，强调模型选择与评价背后的数学理由。
- **主要知识点**：监督 / 无监督学习、回归与分类、概率模型、模型复杂度与泛化、特征与表示、聚类、降维、模型评价、可解释性与稳健性。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐⭐☆ — 是“入门”但不是零数学课程；概率、线代和模型评价是理解算法而非只会调库的关键。
- **考核重点**（2026）：机器学习实践 / 分析作业与受监督测试、期末考核共同评价数学理解和建模能力；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90049/assessment)。
- **建议学习路线**：开课前补向量矩阵、条件概率、导数和 Python 数据栈。每个模型都做一个小数据集实验，记录交叉验证、指标和误差类型；报告不要只给最高分，要解释为什么。

#### `COMP90051` — [Statistical Machine Learning（统计机器学习）](https://handbook.unimelb.edu.au/2026/subjects/comp90051)

- **课程简介**：在入门机器学习之上，进一步学习监督、半监督、主动与无监督学习，并通过开放项目把统计学习方法应用到真实问题。
- **主要知识点**：线性模型、SVM、随机森林、AdaBoost 与模型组合、主动 / 多视角学习、PCA、核方法、深度神经网络、贝叶斯网 / 马尔可夫随机场、HMM。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐⭐⭐ — 模型多、数学密度高，开放项目要求自行选择、实现、比较方法，而不是照步骤完成实验。
- **考核重点**（2026）：开放式机器学习项目与受监督测试 / 期末考核并重；各部分精确权重与 hurdle 见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90051/assessment)。
- **建议学习路线**：先修 COMP90049 或具备等价 ML 基础，再补概率、线代和优化。项目先做可靠 baseline，再控制变量逐项改进；所有结论都用验证集、消融或误差分析支持。

#### `COMP90086` — [Computer Vision（计算机视觉）](https://handbook.unimelb.edu.au/2026/subjects/comp90086)

- **课程简介**：从自动驾驶和医学影像等应用出发，学习如何从图像中提取可计算信息，兼顾经典视觉几何、图像处理和现代学习方法。
- **主要知识点**：图像形成与滤波、相机模型与标定、特征与匹配、几何变换、立体视觉与深度、CNN、目标 / 场景理解、视觉系统评价。
- **2026 S2 开课**：**是，且 2026 仅 S2 开设**；Parkville 校区 On Campus，教学期为 **2026-07-27 至 2026-10-25**。
- **整体难度**：⭐⭐⭐⭐☆ — 线代、几何、概率和深度学习实现交叉，调试既可能是代码问题，也可能是模型或数据问题。
- **考核重点**（2026）：图像处理 / 视觉建模作业、项目和期末考核共同评价理论、实现与实验分析；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp90086/assessment)。
- **建议学习路线**：先补矩阵运算、卷积、Python / NumPy / PyTorch。对相机几何和匹配算法要画图推导；作业从可视化中间结果开始排错，训练模型时固定随机种子并记录配置。

### 数据科学 · 数据分析

#### `COMP20008` — [Elements of Data Processing（数据处理基础）](https://handbook.unimelb.edu.au/2026/subjects/comp20008)

- **课程简介**：围绕完整 data pipeline 讲解数据的获取、表示、清洗、整合、查询、分析、可视化与报告，并介绍数据库和云端数据处理的基础。
- **主要知识点**：数据获取、表示与存储、清洗 / 规范化 / 缺失值处理、数据整合、查询语言与处理、脚本化 pipeline、分片与云文件系统、可视化与结果表达。
- **2026 S2 开课**：**是**；Parkville 校区 On Campus（2026 同时开设 S1 与 S2）。
- **整体难度**：⭐⭐⭐☆☆ — 单个工具不算很深，但从脏数据到可解释结果的流程长，数据质量和报告表达很容易成为失分点。
- **考核重点**（2026）：数据处理实践、分析 / 报告和期末考核共同覆盖 pipeline、数据库、可视化与解释；精确权重见官方 [Assessment](https://handbook.unimelb.edu.au/2026/subjects/comp20008/assessment)。
- **建议学习路线**：先熟悉 Python、pandas、SQL 和基础可视化。每次分析保留原始数据、清洗日志和可复现脚本；报告按“问题—数据—方法—结果—限制”组织，图表必须服务于结论。

---

## 官方来源与使用说明

- [UniMelb 2026 Handbook — Subjects](https://handbook.unimelb.edu.au/2026/subjects)
- [School of Computing and Information Systems — Semester 2, 2026 available subjects](https://cis.unimelb.edu.au/about/casual-staff)
- 每门课程标题已直达其 **2026 Handbook subject page**；成绩组成 / 考核重点后的 **Assessment** 链接直达该课 2026 官方考核页。
- 选课前仍需在课程页的 **Eligibility and requirements** 栏核对 prerequisite、non-allowed subject、学位限制及 coordinator permission。

## 需要按这所学校定制辅导？

选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪跑。可按你的课程大纲、当前基础和目标分数定制每周方案，帮助你把知识点、作业节奏与期末复习真正串起来。
