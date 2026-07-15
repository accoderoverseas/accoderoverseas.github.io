---
title: 悉尼大学（University of Sydney, USYD）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 3
permalink: /cs-courses/course-map/australia/usyd/
published_at: "2026-07-15 21:28:46"
---

<style>
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 悉尼大学（University of Sydney, USYD）

本页按学习方向整理悉尼大学计算机相关核心 / 高频课程，并以 **USYD 2026 Handbook 的 unit page 与 2026 teaching period** 为准，区分本科、研究生对应课程和实际开课学期。

> **更新时间：2026-07-15。** 悉大通常在开课前约两周才发布 unit outline；因此，尚未公开的 2026 S2 考核比例不会用往年数字冒充。页面中的“难度”是基于先修链、知识密度与任务类型给出的学习建议，不是学校官方评级。

## 26S2 开课状态速查

| 专题 | 课程 | 2026 S2 状态 |
|:--|:--|:--|
| 编程 · 软件工程 · 项目 | `INFO1111` / `INFO1113` / `INFO1910` | INFO1113 开设；INFO1111 仅 S1；INFO1910 2026 无 offering |
| 算法 · 数据结构 · 理论 | `COMP2123/COMP9123` / `COMP3027/COMP3927` / `COMP9007` | COMP2123/9123 开设；COMP3027/3927 仅 S1；COMP9007 非 2026 current unit |
| 计算机系统 · 体系结构 | `COMP2017/COMP9017` / `COMP4348/COMP5348` | 前者仅 S1；后者 S2 开设 |
| 数据库 · 信息系统 | `INFO4406/INFO5306` / `COMP9110` / `COMP9120` | COMP9120 开设；COMP9110 仅 S1；INFO4406/5306 非 2026 current unit |
| 人工智能 · 机器学习 | `COMP3308` / `COMP4329/COMP5329` / `COMP5318` / `COMP9208` | COMP5318 开设；其余均仅 S1 |
| 数据科学 · 数据分析 | `DATA1001` / `COMP4448/COMP5048` / `COMP5310` / `COMP5339` | DATA1001、COMP5048、COMP5310、COMP5339 开设；COMP4448 2026 无 offering |

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### [`INFO1111` Computing 1A Professionalism](https://www.sydney.edu.au/units/INFO1111)

- **课程定位**：计算专业的职业实践基础课，不是 Python / Java 编程入门课。
- **主要知识点**：职业伦理与责任、知识产权、团队协作、项目规划、计算工件与协作工具、技术沟通、行业角色与职业发展。
- **2026 S2 开课**：**不开设**；2026 Handbook 仅列 Semester 1。
- **整体难度**：中等。技术门槛不高，但写作、表达、团队协作与持续提交较密集。
- **考核说明**：S2 不开课，因此没有 26S2 成绩组成；选 S1 时应以对应 2026 S1 outline 为准。
- **建议学习路线**：先建立证据引用和专业写作规范，再把团队任务拆成可追踪的里程碑；不要把它当作“水课”临时突击。

#### [`INFO1113` Object-Oriented Programming](https://www.sydney.edu.au/units/INFO1113)

- **课程定位**：以 Java 为核心的面向对象编程课，是后续软件开发课程的重要基础。
- **主要知识点**：对象与引用内存模型、类与 UML、封装、继承、多态、抽象类与接口、异常、测试与调试、集合、泛型和 lambda。
- **2026 S2 开课**：**开设**，Camperdown/Darlington，Normal day；截至 2026-07-15，S2 outline 尚未公开。
- **整体难度**：中高。难点通常不是 Java 语法本身，而是对象关系设计、动态绑定、调试和中型项目组织。
- **成绩组成**：26S2 比例待官方 outline；仅作结构参考，[2026 S1 官方 outline](https://www.sydney.edu.au/units/INFO1113/2026-S1C-ND-CC) 为期末笔试 55%（含 exam hurdle）、项目与 viva 20%、编程挑战 4%、三次任务 12%、三次 tutorial quiz 9%。
- **建议学习路线**：先画对象图 / UML 再编码；每周手写小例子验证继承、多态和泛型，项目从第一周建立测试、Git 提交和可复现运行环境。

#### [`INFO1910` Introduction to Programming (Advanced)](https://www.sydney.edu.au/units/INFO1910)

- **课程定位**：历史上的高级编程入门单元，面向基础较强学生，在两种相关语言中深化过程式编程。
- **主要知识点**：程序设计、内存模型、递归、编译、测试和调试；具体内容仅用于理解历史课程定位。
- **2026 S2 开课**：**不开设**；官网仍显示 2025 unit information，且 2026 无 availability。
- **整体难度**：中高（历史定位），节奏快于普通入门课。
- **考核说明**：没有可用于 26S2 的成绩组成，不建议依据旧 outline 制订 2026 选课计划。
- **建议学习路线**：如需 26S2 编程基础，应按培养方案核对 `INFO1110`、`INFO1112` 或 `INFO1113`，并确认先修与课程归属后再选。

### 算法 · 数据结构 · 理论

#### [`COMP2123`](https://www.sydney.edu.au/units/COMP2123) / [`COMP9123`](https://www.sydney.edu.au/units/COMP9123) Data Structures and Algorithms

- **课程定位**：本科 / 研究生对应的数据结构与算法核心课；内容主线相近，开课时段和考核结构可能不同。
- **主要知识点**：链表、栈、队列、优先队列、搜索树、哈希表、图、排序、树与图遍历、递归、Big-O，以及基础贪心和分治。
- **2026 S2 开课**：**两门均开设**；COMP2123 为 Normal day，COMP9123 为 Normal evening；S2 outline 尚未公开。
- **整体难度**：中高。需要同时完成复杂度推导、纸笔算法题和数据结构实现，知识点之间依赖强。
- **成绩组成**：26S2 以新 outline 为准。参考 2026 S1：[`COMP2123`](https://www.sydney.edu.au/units/COMP2123/2026-S1C-ND-CC) 为期末 60%（exam hurdle）、三次作业 30%、quiz 10%；[`COMP9123`](https://www.sydney.edu.au/units/COMP9123/2026-S1C-NE-CC) 为期末 50%（exam hurdle）、三次作业 40%、quiz 10%。
- **建议学习路线**：每种结构都完成“操作—不变量—复杂度—代码”四联表；算法题先写正确性思路，再分析最坏复杂度，最后限时手写。

#### [`COMP3027`](https://www.sydney.edu.au/units/COMP3027) / [`COMP3927`](https://www.sydney.edu.au/units/COMP3927) Algorithm Design

- **课程定位**：在基础数据结构之上学习通用算法设计范式；COMP3927 是 advanced 版本，先修成绩要求更高。
- **主要知识点**：贪心、分治、动态规划、网络流、复杂度分析、归约、NP-hardness，以及随机化和近似算法。
- **2026 S2 开课**：**不开设**；两门在 2026 Handbook 中均只列 Semester 1。
- **整体难度**：高。核心压力在建模、正确性证明、复杂度论证和 NP 问题归约，而不是套模板写代码。
- **考核说明**：S2 不开课，没有 26S2 成绩组成；advanced 版本还需特别核对 `COMP2123/COMP2823` 等先修及成绩门槛。
- **建议学习路线**：先掌握递归式、图与 DP 状态设计；每道题固定练“反例—算法—正确性—复杂度”四步，建立可迁移的证明模板。

#### [`COMP9007` Algorithms](https://www.sydney.edu.au/units/COMP9007)

- **课程定位**：旧版研究生算法单元，不能作为 2026 当前开课课程理解。
- **主要知识点**：历史描述涵盖图最短路与环检测、动态规划、分治、贪心、局部搜索 / 随机化和 NP-hardness。
- **2026 S2 开课**：**不开设**；官方页面仅保留 2020 unit information，2026 无 availability。
- **整体难度**：历史定位为高，但不应据此推断 2026 课程安排。
- **考核说明**：不存在 26S2 outline 或可用成绩组成。
- **建议学习路线**：若培养方案中出现该代码，先向 faculty 确认课程替代 / equivalence，不要直接套用旧课程资料。

### 计算机系统 · 体系结构

#### [`COMP2017`](https://www.sydney.edu.au/units/COMP2017) / [`COMP9017`](https://www.sydney.edu.au/units/COMP9017) Systems Programming

- **课程定位**：以 C 与 Unix 为主线的系统编程核心课，连接高级语言、操作系统接口与底层资源管理。
- **主要知识点**：指针和动态内存、链表 / 哈希表、线程与并发、Unix 文件 / 进程 / 系统调用 / shell、调试、版本控制、回归测试和安全漏洞。
- **2026 S2 开课**：**不开设**；两门均只列 Semester 1。
- **整体难度**：高。内存错误、并发问题和大作业调试成本高，需要稳定的 C 基础与命令行能力。
- **考核说明**：没有 26S2 成绩组成；不要把旧学期项目权重当成新学期规则。
- **建议学习路线**：提前练 C 指针、数组、结构体、函数指针和 `gdb` / sanitizers；项目优先保证内存安全和边界测试，再做性能优化。

#### [`COMP4348`](https://www.sydney.edu.au/units/COMP4348) / [`COMP5348`](https://www.sydney.edu.au/units/COMP5348) Enterprise Scale Software Architecture

- **课程定位**：本科 / 研究生企业级软件架构课，关注大型分布式系统的集成、伸缩性与可靠性。
- **主要知识点**：遗留代码 / 数据集成、分布式事务、远程对象、消息队列、发布订阅、集群、状态与并发、性能、可用性和可伸缩性分析。
- **2026 S2 开课**：**两门均开设**，Normal evening；S2 outline 尚未公开。
- **整体难度**：中高。概念跨度大，需把架构模式与故障、吞吐、延迟和一致性场景对应起来。
- **成绩组成**：26S2 官方比例待 outline，不预填往年权重。
- **建议学习路线**：用时序图和部署图解释消息流、状态和失败恢复；每学一种模式，都比较适用边界与一致性 / 可用性 / 性能代价。

### 数据库 · 信息系统

#### [`INFO4406`](https://www.sydney.edu.au/units/INFO4406) / [`INFO5306`](https://www.sydney.edu.au/units/INFO5306) Enterprise Healthcare Information Systems

- **课程定位**：历史上的医疗信息系统单元，结合信息系统架构与医疗场景。
- **主要知识点**：历史描述包含 HIS、PACS / 放射信息系统、EHR / PHR、医疗数据与事务、统计研究、决策支持、远程医疗、伦理与隐私。
- **2026 S2 开课**：**不开设**；官网仅显示 2024 unit information，2026 无 availability。
- **整体难度**：历史定位为中等，更强调领域理解、案例分析和信息系统设计。
- **考核说明**：没有 26S2 outline 或成绩组成。
- **建议学习路线**：如培养方案仍列该代码，应先确认替代单元；学习医疗数据时同步关注隐私、合规、互操作性和真实工作流。

#### [`COMP9110` System Analysis and Modelling](https://www.sydney.edu.au/units/COMP9110)

- **课程定位**：面向信息系统需求分析、建模与方案设计，连接业务问题和软件架构。
- **主要知识点**：功能 / 非功能需求、UML 结构与行为模型、风险、成本效益、计划、利益相关者、架构、安装与变更管理、测试、UI / Web 原型和生成式 AI 在分析设计中的使用。
- **2026 S2 开课**：**不开设**；2026 仅列 Semester 1。
- **整体难度**：中等。编码量通常不是核心，难点在需求边界、模型一致性、文档表达和团队协作。
- **考核说明**：S2 不开课，没有 26S2 成绩组成。
- **建议学习路线**：从用户目标和验收条件出发，再绘制 use case、domain model 与 sequence diagram；所有模型保持术语和业务规则一致。

#### [`COMP9120` Database Management Systems](https://www.sydney.edu.au/units/COMP9120)

- **课程定位**：研究生数据库基础与管理核心课，兼顾数据库设计、SQL 与系统内部机制。
- **主要知识点**：关系模型、SQL、概念建模、规范化、存储与索引、查询计划和优化、事务、OLTP / OLAP、数据仓库与数据库管理。
- **2026 S2 开课**：**开设**，Normal evening；S2 outline 尚未公开。
- **整体难度**：中高。SQL 入门不难，后半段的规范化、索引、查询代价和并发事务更需要推理。
- **成绩组成**：26S2 官方比例待 outline，不使用旧学期比例替代。
- **建议学习路线**：先把 ER 图稳定映射到关系模式；SQL 题用小数据手算结果，系统部分用 B+ 树、执行计划和事务调度图逐步推演。

### 人工智能 · 机器学习

#### [`COMP3308` Introduction to Artificial Intelligence](https://www.sydney.edu.au/units/COMP3308)

- **课程定位**：本科人工智能导论，覆盖经典搜索、博弈、机器学习与概率推理。
- **主要知识点**：启发式搜索、minimax 与 alpha-beta、博弈、机器学习、神经网络、概率推理和 AI 算法实现。
- **2026 S2 开课**：**不开设**；2026 仅列 Semester 1。
- **整体难度**：中高。知识面广，需要在算法直觉、数学表达和实现之间快速切换。
- **考核说明**：没有 26S2 成绩组成；S1 学生应以其正式 outline 为准。
- **建议学习路线**：搜索算法先画状态空间，概率与 ML 部分补齐条件概率、向量和基本优化；每个算法都能解释目标、假设与失败情形。

#### [`COMP4329`](https://www.sydney.edu.au/units/COMP4329) / [`COMP5329`](https://www.sydney.edu.au/units/COMP5329) Deep Learning

- **课程定位**：本科 / 研究生深度学习单元，兼顾模型原理、训练方法和计算机视觉应用。
- **主要知识点**：深层神经网络架构、优化与训练、理论分析，以及图像分类、目标检测、分割、人脸识别、原型实现和实验评估。
- **2026 S2 开课**：**不开设**；两门均只列 Semester 1。
- **整体难度**：高。数学、代码、算力和实验设计缺一不可，调参结果也需要严谨解释。
- **考核说明**：没有 26S2 成绩组成；本科与研究生版本不能默认考核完全相同。
- **建议学习路线**：先补线性代数、概率、微积分和反向传播；实验固定记录 baseline、变量、指标与随机种子，避免只追最终 accuracy。

#### [`COMP5318` Machine Learning and Data Mining](https://www.sydney.edu.au/units/COMP5318)

- **课程定位**：研究生机器学习与数据挖掘核心课，强调方法选择、实现与结果评估。
- **主要知识点**：分类、回归、聚类、强化学习基础、模式发现、特征提取、可视化，以及统计 / 机器学习方法的比较与评估。
- **2026 S2 开课**：**开设**，Normal evening；S2 outline 尚未公开。
- **整体难度**：高。官方 assumed knowledge 包括编程、数据结构、离散数学、概率、线性代数和微积分。
- **成绩组成**：26S2 官方比例待 outline，不预填未经核验的旧权重。
- **建议学习路线**：先补矩阵运算、概率分布、梯度和 train/validation/test；作业从简单 baseline 开始，再做特征、模型和误差分析。

#### [`COMP9208` Artificial Intelligence and Society](https://www.sydney.edu.au/units/COMP9208)

- **课程定位**：跨学科 AI 导论，从技术基础延伸到应用、影响和社会语境。
- **主要知识点**：智能体、搜索、规划、机器学习、AI 应用及其社会影响；编程和一年级数学有帮助但不是强制先修。
- **2026 S2 开课**：**不开设**；2026 仅列 Semester 1。
- **整体难度**：中等。数学深度低于纯技术 AI 课，但阅读、论证和跨领域分析要求较高。
- **考核说明**：没有 26S2 成绩组成。
- **建议学习路线**：技术概念与真实案例成对学习；分析 AI 系统时固定检查数据、目标、利益相关者、偏差、责任和治理边界。

### 数据科学 · 数据分析

#### [`DATA1001` Foundations of Data Science](https://www.sydney.edu.au/units/DATA1001)

- **课程定位**：数据科学基础课，以统计思维、数据表达和可复现分析为主，不是纯编程课。
- **主要知识点**：研究设计、base R / ggplot、图形与数值摘要、正态模型和测量误差、线性回归、概率与箱模型、中心极限定理、假设检验与 p-value、混杂与偏差。
- **2026 S2 开课**：**开设**，Normal day；S2 outline 尚未公开。
- **整体难度**：中等。代码门槛可控，真正难点是正确解释统计结论、识别偏差并把结果清楚写出来。
- **成绩组成**：26S2 以新 outline 为准；[2026 S1 官方 outline](https://www.sydney.edu.au/units/DATA1001/2026-S1C-ND-CC) 参考为期末 60%、项目合计 30%、quiz 5%、workshop contribution 5%。
- **建议学习路线**：每周用 R 从导入、清洗、可视化到解释完整走一遍；统计题先用自然语言写假设、变量与结论，再补公式和代码。

#### [`COMP4448`](https://www.sydney.edu.au/units/COMP4448) / [`COMP5048`](https://www.sydney.edu.au/units/COMP5048) Visual Analytics

- **课程定位**：可视分析课程，把信息可视化、交互设计和分析任务结合起来；2026 只有研究生代码 COMP5048 当前开设。
- **主要知识点**：视觉变量、空间与布局、信息组织、人机交互、可视化技术与算法、问题域选择、可视化评价和新方法研究。
- **2026 S2 开课**：`COMP5048` **开设**（Normal evening）；`COMP4448` 官网仍显示 2024 unit information，2026 无 offering。
- **整体难度**：中高。既要做实现，也要说明设计选择为何适合数据、任务和目标用户。
- **成绩组成**：[COMP5048 26S2 官方 outline](https://www.sydney.edu.au/units/COMP5048/2026-S2C-NE-CC) 为持续 lab / tutorial 评估 20%、Assignment 1 20%、Assignment 2 小组展示 10%、Assignment 2 小组报告 50%；后三项均标为 hurdle task。COMP4448 没有 26S2 成绩组成。
- **建议学习路线**：先定义用户问题和分析任务，再选择编码与交互；每张图检查可读性、误导风险、可访问性，并用用户测试验证。

#### [`COMP5310` Principles of Data Science](https://www.sydney.edu.au/units/COMP5310)

- **课程定位**：研究生数据科学基础课，以 Python 串联完整数据流程；官方要求具备关系数据库基础。
- **主要知识点**：数据采集、清洗、预处理、存储与数据库、探索性分析、无标签模式发现、监督学习、可视化和结果沟通。
- **2026 S2 开课**：**开设**，Normal evening；S2 outline 尚未公开。
- **整体难度**：中高。覆盖面广，作业往往要求把数据工程、建模、评价和解释连成可复现流程。
- **成绩组成**：26S2 以新 outline 为准；[2026 S1 官方 outline](https://www.sydney.edu.au/units/COMP5310/2026-S1C-NE-CC) 参考为期末 60%（exam hurdle）、作业一 15%、作业二 25%。
- **建议学习路线**：提前熟悉 Python、pandas、SQL 和 notebook；每次建模先划分数据和建立 baseline，再处理缺失值、特征与评价指标。

#### [`COMP5339` Data Engineering](https://www.sydney.edu.au/units/COMP5339)

- **课程定位**：面向可靠、自动化、可扩展数据管道的数据工程进阶课，先修为 `COMP5310`。
- **主要知识点**：从数据库、文件与 Web 服务摄取数据，清洗转换、自动化流水线、流式与分布式处理、Apache Spark，以及鲁棒性、安全与隐私。
- **2026 S2 开课**：**开设**，Normal evening；S2 outline 尚未公开。
- **整体难度**：高。默认具备 Python、SQL 和 Unix 能力，难点是规模化、故障处理和端到端工程质量。
- **成绩组成**：26S2 官方比例待 outline，不预填往年权重。
- **建议学习路线**：先把单机 ETL 写成可测试、可重跑、可观测流程，再迁移到 Spark；为 schema、失败重试、数据质量和权限建立明确规则。

## 官方来源与使用说明

- 每门详解标题均链接到 [USYD 官方 unit page](https://www.sydney.edu.au/units)，开课状态按 2026 availability 核验。
- “S2 outline 尚未公开”表示截至本页更新时间，官网尚无可核验的 2026 S2 成绩细则；学校后续更新时，以对应 teaching period 的 outline 为最终依据。
- 本科 / 研究生共享课程名称不代表先修、课堂安排与考核一定相同；选课前还需对照本人 course resolution 和 enrolment rules。

## CS 课程体系（按类型）

以下列表用于按代码和方向定位课程，**不等于 2026 S2 开课清单**；上述 19 组核心课程的开课状态与详解以上方核验结果为准。

**编程 · 软件工程 · 项目**

- `INFO1111` — Computing 1A Professionalism
- `INFO1113` — Object-Oriented Programming
- `INFO1910` — Introduction to Programming (Advanced)
- `INFO1911` — IT Special Project 1A
- `INFO1912` — IT Special Project 1B
- `INFO2911` — IT Special Project 2A
- `INFO2912` — IT Special Project 2B
- `INFO3600` — Major Development Project (Advanced)
- `COMP3888` — Computer Science Project
- `INFO3911` — IT Special Project 3A
- `INFO3912` — IT Special Project 3B
- `INFO4001` — Thesis A
- `INFO4002` — Thesis B
- `INFO4003` — Thesis B (extension)
- `COMP4103` — Computer Science Honours Project A
- `COMP4104` — Computer Science Honours Project B
- `COMP4105` — Computer Science Honours Project C
- `COMP4106` — Computer Science Honours Project D
- `COMP4347 / COMP5347` — Web Application Development
- `COMP4405 / COMP5405` — Digital Media Computing
- `COMP4425 / COMP5425` — Multimedia Retrieval
- `COMP4427 / COMP5427` — Usability Engineering
- `INFO4444` — Computing 4 Innovation
- `INFO4491 / INFO5991` — Services Science Management and Engineering
- `INFO4911` — CS Research Thesis A
- `INFO4912` — CS Research Thesis B
- `INFO4913` — CS Research Thesis C
- `INFO4990` — Computer Science Research Methods
- `INFO4991` — IT Research Thesis A
- `INFO4992` — IT Research Thesis B
- `INFO4994 / INFO5994` — Advanced Topics in Computer Science
- `INFO4999` — Computer Science Honours Result
- `INFO5010` — IT Advanced Topic A
- `INFO5011` — IT Advanced Topic B
- `COMP5206` — Information Technologies and Systems
- `COMP5615` — Software Engineering Project
- `COMP5702` — IT Research Project A
- `COMP5703` — Information Technology Capstone Project
- `COMP5704` — IT Research Project B
- `COMP5707` — Information Technology Capstone A
- `COMP5708` — Information Technology Capstone B
- `COMP5709` — IT Capstone Project - Individual
- `COMP5802` — Work Integrated Project
- `COMP9003` — Object-Oriented Programming
- `COMP9201` — Software Construction and Design 1
- `COMP9412` — Agile Software Development Practices
- `COMP9601` — Computer and Network Organisation

**算法 · 数据结构 · 理论**

- `COMP2022` — Models of Computation
- `COMP2123 / COMP9123` — Data Structures and Algorithms
- `COMP2823` — Data Structures and Algorithms (Adv)
- `COMP2922` — Models of Computation (Adv)
- `COMP3027 / COMP3927` — Algorithm Design
- `COMP3109` — Programming Languages and Paradigms
- `COMP3530 / COMP4530 / COMP5530` — Discrete Optimization
- `COMP4445 / COMP5045` — Computational Geometry
- `COMP9007` — Algorithms

**计算机系统 · 体系结构**

- `COMP2017 / COMP9017` — Systems Programming
- `COMP4348 / COMP5348` — Enterprise Scale Software Architecture
- `COMP4349 / COMP5349` — Cloud Computing
- `COMP4426 / COMP5426` — Parallel and Distributed Computing
- `COMP4447 / COMP5047` — Pervasive Computing

**计算机网络**

- `COMP4416 / COMP5416` — Advanced Network Technologies
- `COMP5416` — Advanced Network Technologies

**数据库 · 信息系统**

- `INFO4406 / INFO5306` — Enterprise Healthcare Information Systems
- `COMP9110` — System Analysis and Modelling
- `COMP9120` — Database Management Systems

**人工智能 · 机器学习**

- `COMP3308` — Introduction to Artificial Intelligence
- `COMP3608` — Introduction to Artificial Intelligence (Adv)
- `COMP4328` — COMP5328/COMP8328 - Advanced Machine Learning
- `COMP4329 / COMP5329` — Deep Learning
- `COMP4446 / COMP5046` — Natural Language Processing
- `COMP5318` — Machine Learning and Data Mining
- `COMP9208` — Artificial Intelligence and Society

**数据科学 · 数据分析**

- `DATA1001` — Foundations of Data Science
- `INFO2150` — Introduction to Health Data Science
- `COMP4448 / COMP5048` — Visual Analytics
- `INFO5060` — Data Analytics and Business Intelligence
- `COMP5310` — Principles of Data Science
- `COMP5339` — Data Engineering

**网络安全**

- `INFO2222` — Computing 2 Usability and Security
- `COMP4617 / COMP5617` — Empirical Security Analysis and Engineering
- `COMP4618 / COMP5618` — Applied Cybersecurity
- `COMP8617` — Empirical Security Analysis and Engineering
---

## 需要按这所学校定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
