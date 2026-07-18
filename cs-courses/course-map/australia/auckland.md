---
title: 奥克兰大学（University of Auckland, UoA）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 1
permalink: /cs-courses/course-map/australia/auckland/
published_at: "2026-07-18 08:37:37"
---

<style>
/* 课程号-课程名统一紫色加粗（仅本页生效）：第一部分课程小标题 + 第二部分清单条目 */
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 奥克兰大学（University of Auckland, UoA）

本页以 UoA [Bachelor of Science major in Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/plan?p7_code=COMP-BSc) 的 Stage I → II → III 主修链为骨架，补入面向零基础、软件工程、研究和 capstone 的高频课。所有列出的课程均为 **15 points**，并且已在 **2026 官方 Catalogue** 的 *Availability* 表中确认有 **City · Semester Two** offering。

> **核验说明（2026-07-18）**：UoA 以 *Semester One / Semester Two* 标示学期；本页的“26S2”严格指官方列出的 **2026 Semester Two（City，20 Jul 2026 开始）**。因此，虽然 BSc 主修还包含其他重要课程，本轮不会把仅在 S1 开设的数据库、机器学习、计算理论等课混入。课程简介与知识点来自每门课的 2026 Catalogue 页面；**整体难度与学习建议**为经验参考。考核比例和具体任务仍以本学期 Canvas / course outline 为准。

## 26S2 核心课程速查

| 专题 | 已确认 2026 Semester Two（City）的课程 |
|:--|:--|
| 编程 · 软件工程 · 项目 | `COMPSCI 101`、`COMPSCI 130`、`COMPSCI 230`、`COMPSCI 235`、`COMPSCI 335`、`COMPSCI 380`、`COMPSCI 389`、`COMPSCI 399` |
| 算法 · 数据结构 · 理论 | `COMPSCI 120`、`COMPSCI 220`、`COMPSCI 225`、`COMPSCI 320` |
| 计算机系统 · 体系结构 | `COMPSCI 110`、`COMPSCI 210`、`COMPSCI 313`、`COMPSCI 340` |
| 计算机网络 | `COMPSCI 315` |
| 人工智能 · 机器学习 | `COMPSCI 367` |
| 网络安全 | `COMPSCI 316` |

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### [`COMPSCI 101` — Principles of Programming](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20101)

- **课程定位**：面向没有编程经验、准备继续读 Computer Science 或 Information Systems 的实践型 Python 入门课；它是进入 `COMPSCI 130` 前的衔接选择，不是 BSc CS 主修的三门 Stage I 必修之一。
- **主要知识点**：Python、变量与表达式、输入 / 输出、分支与循环、函数、列表和字典、标准模块、按细致需求读写结构清晰且正确的程序。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐☆☆☆ — 语法门槛友好，真正的挑战是把题意拆准并形成逐步调试的习惯。
- **建议学习路线**：每个练习都先写 2—3 个输入输出样例，再写函数；不要跳过 lab。完成后能独立解释变量如何变化、函数为何这样拆分，再进入 `COMPSCI 130` 会稳得多。

#### [`COMPSCI 130` — Introduction to Software Fundamentals](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20130)

- **课程定位**：有既往编程经验学生进入 CS 主修的 Stage I 核心课，从“能写程序”提升到按良好软件开发过程写出可靠代码。
- **主要知识点**：条件、迭代、递归、函数、测试与调试、代码阅读 / 文档、问题分解、排序与搜索、列表 / 栈 / 队列 / 字典 / 树等抽象数据类型的使用与实现。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐☆☆ — 递归、数据结构与程序质量要求会同时上来，节奏比零基础课明显更快。
- **建议学习路线**：每周把“需求 → 分解 → 实现 → 测试 → 调试”完整跑一遍；数据结构不要只会调用，至少亲手实现并解释其操作代价，为 `COMPSCI 220` 打底。

#### [`COMPSCI 230` — Object Oriented Software Development](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20230)

- **课程定位**：Stage II 的面向对象软件开发核心课，用 Java 训练设计、建模与实现中等复杂度的应用，是多门三年级软件 / 系统课的基础。
- **主要知识点**：类、对象与多态、封装 / 模块化 / 复用、UML 类图、面向测试和变化的设计、代码异味与重构、设计模式、GUI 应用与 Java 代码规范。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 难点是从“代码能跑”转向“对象职责是否合理、能否修改与测试”。
- **建议学习路线**：先画 UML 和对象职责，再写类；每次重构前补测试。课程官方设有受控（test + exam）与 coursework 两条通过要求，不能只押项目或只刷考试。

#### [`COMPSCI 235` — Software Development Methodologies](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20235)

- **课程定位**：软件开发的过程与工具课，系统认识开发流程、最佳实践、工具链与质量保证；官方建议在完成 `COMPSCI 230` 后学习。
- **主要知识点**：软件开发方法论、过程组织、设计方法、开发工具、最佳实践、质量保证与测试。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐☆☆ — 编程深度通常不如核心项目课，难在把抽象流程和质量标准落实到实际 artefact。
- **建议学习路线**：把课程里的每个方法都映射到一个小项目：需求如何留痕、分支如何管理、测试如何证明质量。它与 `COMPSCI 230` 同修时，正好可互相强化设计和工程习惯。

#### [`COMPSCI 335` — Web Programming and Distributed Services](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20335)

- **课程定位**：从前后端两个视角理解 Web 应用与分布式服务，目标是具备设计和构建较复杂现实 Web 应用的 full-stack 视角。
- **主要知识点**：客户端 / 服务端、动态 Web 应用、异构与异步数据整合、Web 与 cloud clients / services、声明式 / 函数式技术、安全与性能、真实 Web 应用设计。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 难在前后端协同、异步数据和安全 / 性能不再能分开处理。
- **建议学习路线**：先搭一个最小 client-server 闭环，再逐步加入数据源、鉴权和性能考虑；从第一个功能起就记录 API 合约和失败场景，不要等联调时才补设计。

#### [`COMPSCI 380` — Project in Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20380)

- **课程定位**：面向优秀 Stage III 学生的个人实践项目，不是常规授课项目。须先与 staff supervisor 确认主题，且官方明确仅允许有优秀学业记录的学生修读。
- **主要知识点**：独立项目选题、问题定义、在指导下完成理论或实践性 artefact、技术沟通与研究 / 项目过程管理。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 难点不只在技术，而在于自行界定范围、持续推进并把成果讲清楚。
- **建议学习路线**：先用一页 proposal 说清问题、可交付物、风险和 12 周节奏；找 supervisor 前准备已有基础和可执行的最小目标。不要把它当作“有空再做”的自由课。

#### [`COMPSCI 389` — Research Methods in Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20389)

- **课程定位**：为研究、honours 或需要严谨论证的项目建立方法论基础；会将形式化证明和定量 / 定性实证方法放在同一研究流程里理解。
- **主要知识点**：形式化证明、定量与定性实证方法、研究问题与方法匹配、协作研究项目、研究 proposal、学术讨论与论证。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐☆☆ — 技术编码负担未必最大，难在把“感兴趣”缩成可研究、可验证的问题。
- **建议学习路线**：从一个很小的可验证问题开始，提前建立文献、数据 / 证据和结论之间的对应表；写 proposal 时明确变量、评价方法和可能的威胁，而不只堆背景介绍。

#### [`COMPSCI 399` — Capstone: Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20399)

- **课程定位**：CS capstone 选择之一。小组围绕一个实质性问题完成分析、方案、artefact 与展示，用问题导向学习整合主修阶段的技术和沟通能力。
- **主要知识点**：问题分析、方案设计、团队开发、产出 artefact、技术展示、跨课程知识整合、反思与职业过渡。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 工作量和团队协同是核心压力；成败取决于需求边界、技术选型和持续交付，而非最后一周的 demo。
- **建议学习路线**：项目早期就锁定问题、用户 / 利益相关者、成功标准和责任边界；每周安排可演示的增量。把 `COMPSCI 220 / 230 / 235` 的算法、设计、测试实践真正带入项目。

### 算法 · 数据结构 · 理论

#### [`COMPSCI 120` — Mathematics for Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20120)

- **课程定位**：CS 主修 Stage I 的数学和证明地基，后续 `COMPSCI 220`、`COMPSCI 225`、算法 / ML / 理论课都会用到这里的抽象推理。
- **主要知识点**：整数与有理数、字符串与集合、证明与归纳法、算法与函数、图与树、计数与概率。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 对习惯“代公式”的同学，证明书写和抽象对象定义是最大转换。
- **建议学习路线**：把每周题目分成“定义、例子、证明模板”三栏；归纳法、反证法和集合 / 函数的语言一定要亲手写，不能只看答案觉得懂了。

#### [`COMPSCI 220` — Algorithms and Data Structures](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20220)

- **课程定位**：所有 CS majors 必修的 Stage II 核心算法课，研究如何高效存储、处理数据并评估程序随数据规模增长时的表现。
- **主要知识点**：抽象数据类型及实现、渐近复杂度、排序与搜索、深度 / 广度优先搜索及应用、图优化问题、算法分析。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 数据结构实现、Big-O 和图算法需并行掌握，后续 `COMPSCI 320` 的上限很大程度由它决定。
- **建议学习路线**：每种结构都做“操作—不变量—复杂度—代码”四联表；图题先画图、写遍历状态和复杂度，再开始实现。不要用刷题量替代对 ADT 选择理由的理解。

#### [`COMPSCI 225` — Discrete Structures in Mathematics and Computer Science](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20225)

- **课程定位**：以“数学证明”为中心的离散结构课，为逻辑、算法、自动机和计算理论补齐更系统的形式化工具。
- **主要知识点**：逻辑、计数原理、数学归纳法、递归、集合与函数、图、编码、有限自动机。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 内容广且证明密集，容易在符号精度和推理跳步上失分。
- **建议学习路线**：不要把它拆成零散知识点背诵；用“定义 → 小例子 → 反例 → 正式证明”处理每个概念。和 `COMPSCI 120` 同学期时，统一整理证明语言会轻松许多。

#### [`COMPSCI 320` — Applied Algorithmics](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20320)

- **课程定位**：三年级算法设计课，在 `COMPSCI 220` 之上学习怎样设计既正确又高效的算法，并理解 NP-completeness 等计算能力边界。
- **主要知识点**：高效问题求解的设计技术、正确性与效率、算法选择、计算能力极限、NP-completeness、正确性或性能无保证的方法。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐⭐ — 不只问“怎么实现”，更要求算法设计、正确性论证和复杂度分析同时成立。
- **建议学习路线**：复习 `COMPSCI 220` 的递归、图和复杂度；每道题固定写“模型—算法—正确性—复杂度—边界”，把证明作为解题的一部分而不是交卷前补写。

### 计算机系统 · 体系结构

#### [`COMPSCI 110` — Introduction to Computer Systems](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20110)

- **课程定位**：CS 主修 Stage I 的系统总览课，从二进制数据一路连到硬件、低层编程、操作系统、应用和通信。
- **主要知识点**：数据与指令编码、二进制表示、硬件层、低层编程、操作系统、应用层、网络 / Internet 和现代计算系统的分层关系。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐☆☆ — 纵向跨度很大，难点是把众多层次串成一条因果链，而不是记术语。
- **建议学习路线**：始终用“数据如何表示—指令怎样执行—系统怎样管理—机器怎样通信”作为主线；每学一层都画出它与上下层交换了什么信息，为 `COMPSCI 210` 做准备。

#### [`COMPSCI 210` — Computer Organisation](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20210)

- **课程定位**：Stage II 的核心系统课，研究程序员能看到的硬件 / 软件接口，是 Stage III 系统课程的重要先修。
- **主要知识点**：低层数据和算法表示、指令执行模型、ISA、汇编与反汇编、汇编编程、C 到机器层的映射、内存组织、支持安全多用户操作系统的硬件机制。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 汇编、内存和 C / ISA 映射需要耐心追踪执行过程，不能停留在概念层。
- **建议学习路线**：遇到程序就按“寄存器—指令—内存”三张表走一遍；手写并单步跟踪小段汇编，把 C 变量和内存地址对应起来，理解才会稳定。

#### [`COMPSCI 313` — Computer Architecture](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20313)

- **课程定位**：在组织层之上研究现代处理器和计算系统设计，适合希望理解性能瓶颈、硬件选型和并行处理的学生。
- **主要知识点**：现代处理器设计、流水线、内存层次与管理、I/O 与网络接口、编译器 / OS 支持、嵌入式处理器、性能评估、多处理器。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 缓存、流水线和性能之间的权衡很抽象，计算题与机制理解缺一不可。
- **建议学习路线**：按“单条指令 → 流水线 → cache / memory → 多处理器”由小到大建图；每次性能题都写清假设、瓶颈和指标，别只套公式。

#### [`COMPSCI 340` — Operating Systems](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20340)

- **课程定位**：系统软件核心课，理解操作系统怎样在资源、并发、安全和分布式需求之间做管理与取舍。
- **主要知识点**：多用户系统、虚拟化、调度、进程 / 线程 / 同步 / 死锁、内存分配与虚拟内存、文件 / 磁盘 / 外设、安全与保护、分布式透明性、实时需求。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 并发状态、死锁与虚拟内存既抽象又容易在边界条件上出错。
- **建议学习路线**：画状态图而非硬背定义：线程何时阻塞、锁由谁持有、页面何时换入换出。先用小例子验证正确性，再分析性能与可扩展性。

### 计算机网络

#### [`COMPSCI 315` — Data Communications Technologies](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20315)

- **课程定位**：以 Internet 为主线的网络基础课，覆盖从数据传输到应用协议的通信架构，也为分布式系统理解提供底座。
- **主要知识点**：分层协议模型、数据传输与编码、链路层和 LAN 协议、广域互联与路由、传输层和安全协议、应用协议、分布式计算基础。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 网络跨层、协议多，难点是理解每层的职责、封装和取舍，而不只是背缩写。
- **建议学习路线**：先搭一张“应用 → 传输 → 网络 → 链路”分层图，再把每个协议放入其中。分析一次访问网页或发送数据包的路径，协议关系会更直观。

### 人工智能 · 机器学习

#### [`COMPSCI 367` — Artificial Intelligence](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20367)

- **课程定位**：AI 的知识表示与搜索主干课，学习如何把现实问题表示成计算机能求解的形式，并思考 AI 的历史、未来与伦理。
- **主要知识点**：AI 算法与表示方案、启发式搜索、约束满足、最优与 satisficing 任务、对抗搜索与博弈、规划、自然语言处理、知识表示、AI 伦理。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 搜索策略、问题表示和不同任务目标之间的关系是主要门槛；它不是只靠调模型的 ML 课。
- **建议学习路线**：每类题先定义 state、actions、goal / utility 和约束，再选搜索或表示方法。把 BFS、DFS、启发式、CSP、对抗搜索分别放进同一张决策图，不易混淆。

### 网络安全

#### [`COMPSCI 316` — Cyber Security](https://study.auckland.ac.nz/ords/r/uoa/catalogue/course?p6_code=COMPSCI%20316)

- **课程定位**：横跨软件、系统和网络的安全基础课，兼顾攻击面分析与当代安全技术话题。
- **主要知识点**：隐私攻击与攻击面、恶意软件静态 / 动态分析、硬件安全、可信计算基、secure boot 与 attestation、网络安全、椭圆曲线、区块链和 Bitcoin。
- **2026 S2 开课**：City，Semester Two。
- **整体难度**：⭐⭐⭐⭐☆ — 范围广，既要能从攻击者视角推演，也要理解防御边界和系统依赖。
- **建议学习路线**：用“资产—攻击面—威胁—控制—残余风险”统一整理每个主题；不只记攻击名，要说清它利用了什么假设、有什么证据和防御代价。

## 官方来源与使用说明

- [UoA BSc Computer Science major](https://study.auckland.ac.nz/ords/r/uoa/catalogue/plan?p7_code=COMP-BSc) 用于核对 Stage I / II 必修与 Stage III 课程池；每门详解标题均链接至对应的 **2026 UoA Course Catalogue**。
- 本页以各课程页 *Availability* 表的 **2026 · Semester Two · City** 行判断能否写入，未把 S1-only 课程写入“核心 / 高频课程详解”或下方体系清单。
- UoA 课程页的 assessment 信息可能随具体 offering 或 Canvas 更新；选课前还须在官方页确认 prerequisites / restrictions，并以当学期 Canvas 和 course outline 为最终依据。

## CS 课程体系（按类型）

> 以下是本轮已确认 **2026 Semester Two（City）** 开设、且围绕 UoA CS 主修链或其常见衔接的课程；不以旧学期或仅 S1 的课程凑数量。

**编程 · 软件工程 · 项目**

- `COMPSCI 101` — Principles of Programming
- `COMPSCI 130` — Introduction to Software Fundamentals
- `COMPSCI 230` — Object Oriented Software Development
- `COMPSCI 235` — Software Development Methodologies
- `COMPSCI 335` — Web Programming and Distributed Services
- `COMPSCI 380` — Project in Computer Science
- `COMPSCI 389` — Research Methods in Computer Science
- `COMPSCI 399` — Capstone: Computer Science

**算法 · 数据结构 · 理论**

- `COMPSCI 120` — Mathematics for Computer Science
- `COMPSCI 220` — Algorithms and Data Structures
- `COMPSCI 225` — Discrete Structures in Mathematics and Computer Science
- `COMPSCI 320` — Applied Algorithmics

**计算机系统 · 体系结构**

- `COMPSCI 110` — Introduction to Computer Systems
- `COMPSCI 210` — Computer Organisation
- `COMPSCI 313` — Computer Architecture
- `COMPSCI 340` — Operating Systems

**计算机网络**

- `COMPSCI 315` — Data Communications Technologies

**数据库 · 信息系统**

- 本轮核心范围内没有已确认 2026 S2 开设的课程；不以仅 S1 开设的课替代。

**人工智能 · 机器学习**

- `COMPSCI 367` — Artificial Intelligence

**数据科学 · 数据分析**

- 本轮核心范围内没有已确认 2026 S2 开设的课程；不以仅 S1 开设的课替代。

**网络安全**

- `COMPSCI 316` — Cyber Security

---

## 需要按这所学校定制辅导？

选课不确定值不值得选、已选课想搭知识体系、项目无从拆解、考前（含 hurdle 课程）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲和基础定制方案，把课程真正弄懂吃透。
