---
title: 新南威尔士大学（UNSW Sydney）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 2
permalink: /cs-courses/course-map/australia/unsw/
published_at: "2026-07-05 17:18:05"
---

<style>
/* 课程号-课程名统一紫色加粗（仅本页生效）：第一部分课程小标题 + 第二部分清单条目 */
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 新南威尔士大学（UNSW Sydney）

UNSW CS 采用 **COMP** 课程编码（信息系统类为 **INFS**）、每年 3 个 term（T1 / T2 / T3）快节奏授课，本科与研究生课程合并整理。下方先给出**核心 / 高频课程详解**，再附**完整课程清单**（均**按课程类型归类**）。

> 说明：每门课的 **课程简介 · 主要知识点 · 成绩组成** 依据 UNSW **2026 官方 handbook / course outline** 整理；**整体难度 · 建议学习路线** 为 **辅导视角**（主观参考，因人而异）。UNSW 各 term 的评估占比常有微调，成绩组成最终一律以当学期 course outline 为准。来源见页面底部。

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### `COMP1511 / COMP1911` — Programming Fundamentals（编程入门）
- **课程简介**：UNSW 计算机学位的第一门编程课，用 **C 语言**从零教起——从变量、循环、函数到数组、指针和链表，带你把现实问题拆解成可执行的代码，重点培养系统化解决问题、调试和测试的思维习惯。`COMP1911`（Computing 1A）是面向非 CS / 工程主修学生的同源版本，内容高度重合、节奏略缓，两者不可重复修读。
- **主要知识点**：C 语言语法、变量与数据类型、控制流、函数、数组、字符串、指针、动态内存、结构体、链表、文件 I/O、调试与测试。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念本身不难，但**指针与动态内存**是初学者的第一道坎；节奏快，每周 lab + 作业积累起来负担不小。
- **成绩组成**：Problem Sets（每周 lab / 小测）15% + Assignment 1 20% + Assignment 2 25% + 期末考试 40%（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：无需先修，但建议提前熟悉命令行与 Linux 基本操作。每周 lab 必须当周清账、切勿拖到考前；把指针画成"内存图"理解最有效。学完后自然衔接 COMP1521（系统基础）与 COMP2521（数据结构与算法）。

#### `COMP1531` — Software Engineering Fundamentals（软件工程基础）
- **课程简介**：第一门"像真正软件工程师那样做项目"的课。围绕一个贯穿整学期的 **Python 大型小组项目**，学习软件生命周期、敏捷开发、需求建模、测试驱动开发和团队协作。相比 COMP1511 的个人编码，这门课让你第一次体会真实工程流程。
- **主要知识点**：软件生命周期、敏捷 / Scrum、需求与概念建模、Git 协作、单元测试与集成测试、测试自动化、REST API、前后端交互、代码评审、团队分工。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 技术难度中等，真正的坎是**小组协作与分工**：项目分 3 个迭代（iteration 2 工作量最大），队友配合和进度管理往往比写代码更棘手。
- **成绩组成**：以贯穿全程的分迭代小组项目（含 Python 后端实现、测试、Git 使用与团队协作评分）为主，辅以个人 lab / 练习与实验室评估（务必以当学期 course outline 公布的具体占比为准）。
- **建议学习路线**（辅导视角）：需先修 COMP1511。开学第一周就配置好 Git 与团队仓库，养成写测试的习惯；主动承担迭代任务、别做"隐形队友"。为后续 COMP2511、COMP3900 / COMP9900 项目课打基础。

#### `COMP2041 / COMP9044` — Software Construction: Techniques and Tools（软件构建：技术与工具）
- **课程简介**：面向已掌握编程基础的学生，教你在 Unix / Linux 环境下用**脚本语言**高效构建软件。内容涵盖 Shell / Bash、Python、正则表达式与文本处理（Unix filters），以及 Git 版本控制、Docker 部署等现代工具链。`COMP9044` 是研究生同源版本，内容一致。
- **主要知识点**：Shell / Bash 脚本、Unix filters（grep / sed / awk）、正则表达式、Python 脚本、Perl（视学期）、Git 版本控制、Docker、包管理与部署、CGI 脚本。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 单点知识不难，但**Shell 与正则的"奇技淫巧"**容易踩坑；两个较大的编程作业需要把零散工具组合成完整方案。
- **成绩组成**：每周 lab 练习合计约 18% + Assignment 1（Shell 编程，约第 7 周，约 15%）+ Assignment 2（脚本 / Perl，约第 10 周，约 15%）+ 期末考试（其余占比）（以当学期 course outline 为准；注意该课要求不得使用生成式 AI 完成作业）。
- **建议学习路线**（辅导视角）：建议先修 COMP1511 / COMP1521，熟悉命令行者上手更快。平时多在终端练习 grep / sed / awk 和正则，作业才不会被"工具组合"卡住。是提升日常开发效率的高性价比课程。

#### `COMP2511` — Object-Oriented Design & Programming（面向对象设计与编程）
- **课程简介**：用 **Java** 系统学习面向对象设计的理论与实践，核心是**设计模式**（Design Patterns）与设计原则（SOLID 等），目标是构建灵活、可复用、可维护的系统。课程以一个结对完成的大型项目为主线，让你把设计模式真正落到代码里。
- **主要知识点**：Java 面向对象、封装 / 继承 / 多态、SOLID 原则、创建型 / 结构型 / 行为型设计模式（Factory、Strategy、Observer、Decorator、Composite 等）、UML、重构、泛型、异常处理、敏捷实践。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 从"能写代码"到"写好设计"是质变；**设计模式的意图与适用场景**是理解难点，结对大项目对设计能力和协作都是考验。
- **成绩组成**：以结对完成的大型 Java 项目（分阶段，考核设计模式与设计原则的应用）为主，辅以 lab / 练习与期末考试（考察对各设计模式意图、方案与实现的掌握），具体占比以当学期 course outline 为准。
- **建议学习路线**（辅导视角）：需先修 COMP1531 与 COMP2521。学习时务必"知其所以然"——每个模式先想清楚解决什么问题再记结构；项目中主动做设计而非直接编码。是软件工程方向的关键进阶课，直接支撑高年级项目课。

#### `COMP3141` — Software System Design and Implementation（软件系统设计与实现）
- **课程简介**：用**强类型函数式语言 Haskell**（不需要先备知识）介绍软件设计与实现的半形式化 / 形式化方法。核心思想是用类型系统和逻辑性质来指导程序设计、实现、验证与检验——一门改变你"怎么思考程序正确性"的课。
- **主要知识点**：Haskell 函数式编程、类型系统、代数数据类型、高阶函数、类型驱动设计、逻辑性质与不变量、基于属性的测试（property-based testing）、程序验证与检验、语义与推理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 函数式思维与命令式差异大，**"用类型和性质思考"**是最大门槛；期末成绩由平时实践分与期末考的调和平均决定，任一端偏弱都会明显拉低总分。
- **成绩组成**：每周小测（约 8 次，考察理论）+ 每周编程练习（约 7 次，含 1 次同行评审）+ 期末考试；**最终成绩为"实践部分"与"期末考试"的调和平均**（harmonic mean），具体占比以当学期 course outline 为准。
- **建议学习路线**（辅导视角）：建议先修 COMP2521。提前接触 Haskell 语法，重点理解"类型即规约"的思路；每周练习不能欠账（调和平均意味着"短板致命"）。适合对编程语言理论、形式化方法感兴趣的学生。

#### `COMP9020` — Foundations of Computer Science（计算机科学基础）
- **课程简介**：研究生阶段的**离散数学与逻辑**基础课，为计算机科学的理论根基打底。涵盖集合、逻辑、证明、关系、图论、组合计数与概率等——是理解算法、复杂度与形式化方法的必备数学工具箱。
- **主要知识点**：命题与谓词逻辑、证明方法（归纳法等）、集合与关系、函数、图论、树、组合计数、递归关系、离散概率、布尔代数、形式化推理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 对数学背景较弱的转专业研究生是明显的坎，**证明题（proof）**最容易失分；概念多、需要持续练习而非临时抱佛脚。
- **成绩组成**：期末考试 60% + 作业 30%（2 次，各约 10 分）+ 小测 / Quizzes 10%（约 10 次；另有每周 Formatif 练习）（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：无严格编程先修，但需一定数学成熟度。每周跟做 Formatif 与练习题、尤其多练证明的书写规范；配合教材（Rosen《离散数学及其应用》或 Lehman《Mathematics for CS》）。是后续算法、理论类课程的基石。

#### `COMP9319` — Web Data Compression and Search（Web 数据压缩与搜索）
- **课程简介**：聚焦大规模 Web 数据的**压缩算法与高效搜索 / 索引技术**。你会深入 Huffman 编码、BWT（Burrows–Wheeler 变换）、倒排索引等核心方法，并通过实现项目理解如何在海量文本上做压缩存储与快速检索。
- **主要知识点**：数据压缩（Huffman、算术编码、LZ 系列）、Burrows–Wheeler 变换（BWT）、后缀数组 / 后缀树、倒排索引、字符串匹配、压缩域搜索、Web 搜索与信息检索基础、XML / 半结构化数据处理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — **BWT 相关的编程作业**公认硬核，对内存 / 时间效率要求高，算法与工程实现能力缺一不可。
- **成绩组成**：两次编程作业（围绕 Web 数据压缩与搜索算法的实现）+ 期末考试（主要评估项）；具体占比以当学期 course outline 为准（注意：该课禁止提交由 Copilot / ChatGPT 等自动工具生成的代码）。
- **建议学习路线**（辅导视角）：需扎实的数据结构、算法与 C / C++ 编程基础（建议先修 COMP9024 / COMP2521 类课程）。尽早动手做 BWT 作业、预留充足调优时间；该课 2026 仅在 T2 开设。

### 算法 · 数据结构 · 理论

#### `COMP2521` — Data Structures and Algorithms（数据结构与算法）
- **课程简介**：UNSW 计算机专业的核心必修课，从 COMP1511 的入门 C 语言过渡到"真正的算法思维"。课程用 C 语言带你把链表、树、图这些抽象结构亲手实现出来，并学会用大 O 分析衡量代码效率。可以说是决定你后续所有算法课上限的一门"内功课"。
- **主要知识点**：递归、抽象数据类型（ADT）、链表 / 栈 / 队列、排序算法、二叉搜索树与平衡树（AVL）、图的表示与遍历（BFS / DFS）、最短路径与最小生成树、哈希、时间 / 空间复杂度分析。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 难点在于用 C 手动管理指针与内存去实现复杂结构（尤其图和树），概念不难但工程量与调试量大。
- **成绩组成**：Labs 15% + Quizzes 10% + Assignment 1 15% + Assignment 2 15% + 期末考试 45%（含期末及格线 hurdle；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先把 C 指针与动态内存彻底吃透，这是全课地基；每周 lab 与 quiz 一定当周完成、不欠账，因为知识点强累积。两个大作业（通常是图和 BST 相关）尽早动手、预留充足调试时间，并从第一天起就用 gdb / valgrind 排查内存问题。

#### `COMP3161 / COMP9164` — Concepts of Programming Languages（编程语言概念）
- **课程简介**：一门理论味很浓的"编程语言底层原理"课，探讨语言背后的数学基础——为什么类型系统能保证安全、语义如何被形式化定义。课程用 Haskell 作为工具语言（无需先修 Haskell），把 lambda 演算、类型推导、语义等抽象概念变成可运行的实现。学完你会用完全不同的视角看待任何一门编程语言。
- **主要知识点**：命令式 / 面向对象 / 函数式 / 并发编程范式、语法与文法、操作语义 / 公理语义 / 指称语义、lambda 演算、抽象机、类型推导、存在类型、子类型、多态与重载、自动内存管理、并发与 session types。
- **整体难度**（辅导视角）：⭐⭐⭐⭐⭐ — 全校公认硬核，形式化证明 + Haskell 函数式思维双重门槛，数学基础薄弱会很吃力。
- **成绩组成**：Assignment 0（理论 / 证明）15% + Assignment 1（编程）17.5% + Assignment 2（编程）17.5% + 期末考试 50%（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：提前预习 Haskell 与基础离散数学 / 逻辑证明，别等开课再学；把每周 lecture 的语义推导规则手抄整理成"规则卡片"反复练；证明型作业（Ass0）是期末考的预演，务必独立完成并订正。本课仅在 T3 开设，UG 走 COMP3161、PG 走 COMP9164，同堂授课。

#### `COMP9021` — Principles of Programming（编程原理）
- **课程简介**：面向研究生的 Python 编程入门课，目标是把零散的编程直觉打磨成扎实的问题求解能力。课程覆盖 Python 从基础到进阶（生成器、正则、numpy、面向对象、递归 / 动态规划），并借大量有趣问题（图灵机、分形、密码学等）训练算法思维。适合转专业或需要补强 Python 功底的 PG 学生。
- **主要知识点**：Python 数据类型与控制结构、函数（位置 / 关键字 / 默认参数）、推导式与生成器、迭代器、正则表达式、numpy 数组、递归与记忆化、动态规划、面向对象（类 / 继承 / 特殊方法 / 装饰器）、复杂度与内存直觉、matplotlib 绘图。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 对有编程经验者偏友好，难点在于每周高频 quiz 的节奏与 Python 进阶语法的熟练度，而非概念深度。
- **成绩组成**：8 次每周编程 Quiz 共 24%（每次 3 分）+ 2 个编程 Assignment 共 26%（每个 13 分）+ 期末考试 50%（在线，最终成绩为各项算术平均，需达 50 分及格）（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：把课程提供的 Jupyter notebook 逐格运行、先猜输出再验证，这是最高效的吸收方式；每周 quiz 当周做完保持节奏，两个作业尽早开工（注意迟交每天扣分）；把 practice exercises 当作期末实战演练。

#### `COMP9024` — Data Structures and Algorithms（数据结构与算法）
- **课程简介**：COMP2521 的研究生版本，同样用 C 语言系统讲授数据结构与算法，是众多 IT 硕士项目的算法基础核心课。从数组、动态结构讲到图、搜索树、字符串与随机化算法，强调"不仅会写，还能论证其适用性与效率"。是 PG 学生打通算法面试与后续课程的必经之路。
- **主要知识点**：C 语言基础数据结构、算法分析（复杂度）、抽象数据类型、动态数据结构、图的表示与算法、搜索树（BST 等）、字符串算法、随机化算法、算法伦理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 与 COMP2521 相当，C 语言指针 / 内存实现是主要门槛，且期末考设有单独及格线。
- **成绩组成**：Weekly Exercises 16%（8 周 × 2）+ Midterm Exam 12%（Week 6，线上）+ Assignment 12%（Week 5 发布，Week 10 截止）+ 期末考试 60%（校内闭卷）。及格要求：总分 ≥ 50 且期末 ≥ 25/60（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：若 C 语言基础薄弱，务必开课前补齐指针与动态内存；每周 exercise 别拖，它们直接对应期末考点；Week 6 midterm 与 Week 10 大作业要提前规划，期末占 60% 且有单独 hurdle，复习务必把每类结构亲手默写实现一遍。

### 数据库 · 信息系统

#### `COMP3311 / COMP9311` — Database Systems（数据库系统）
- **课程简介**：数据库入门主力课程，UG（COMP3311）与 PG（COMP9311）内容基本对应。带你从"数据如何被有效组织"出发，学会用 ER 图建模现实世界、把设计落地为关系模式，再用 SQL / PLpgSQL 在 PostgreSQL 上真正写出可运行的数据库应用。理论与动手并重，是几乎所有后续数据库 / 信息系统课的地基。
- **主要知识点**：ER 建模与关系模型、关系代数、数据库设计与规范化、SQL 查询、PLpgSQL 存储过程 / 触发器、事务与并发基础、DBMS 内部机制概览、Python + SQL 应用开发。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念不深但覆盖面广，SQL 与 PLpgSQL 的实操作业容易在细节和效率要求上翻车。
- **成绩组成**：Quizzes 12% + Assignment 1（SQL / PLpgSQL）13% + Assignment 2（Python + SQL）15% + 期末考试 60%（期末为 hurdle，须 ≥40%；COMP9311 权重可能略有差异，以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先把 ER → 关系模式 → 规范化这条主线彻底吃透，这是设计题和考试的核心；SQL 一定要多在本地 PostgreSQL 上敲，尤其把 JOIN、聚合、子查询和 PLpgSQL 触发器写熟；作业提早开工，预留时间跑自动评测和调效率。

#### `COMP6714` — Information Retrieval and Web Search（信息检索与网络搜索）
- **课程简介**：讲清楚"搜索引擎是怎么工作的"。从如何把海量文档建成倒排索引、如何压缩存储，到用向量空间 / 概率 / 语言模型对结果排序，再延伸到网页爬取、链接分析与搜索引擎架构。既有算法原理也有工程实现，偏进阶选修。
- **主要知识点**：文档建模、倒排索引构建与压缩、向量空间模型与排序、概率模型 / 语言模型、检索评估（precision / recall 等）、相关性反馈与查询扩展、Web 爬虫与索引、网页结构与链接分析、搜索引擎架构。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 概念抽象、数学（信息论 / 概率 / 线性代数）与编程项目并重，programming project 工作量较大。
- **成绩组成**：Assignment（非编程）20% + Project（编程）30% + 期末考试 50%（期末为 hurdle，须 >40%；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：把倒排索引和 TF-IDF / 向量空间排序作为主干先啃透，后面的概率 / 语言模型都建立在这上面；编程 project 早启动、分模块实现并自测；评估指标（P / R / MAP / NDCG）务必会手算，考试常考。

#### `COMP9315` — Database Systems Implementation（数据库系统实现）
- **课程简介**：不再是"用"数据库，而是"造"数据库。深入 DBMS 内部：数据如何在磁盘上存储、缓冲区如何管理、查询如何被处理与优化、事务与并发控制如何实现。作业直接在 PostgreSQL 源码上做扩展，是数据库方向最硬核的进阶课之一。
- **主要知识点**：存储管理与页面结构、缓冲区管理、文件组织与索引（B-tree / hash）、查询处理与执行、查询优化、事务管理、并发控制与恢复、PostgreSQL 内部实现。
- **整体难度**（辅导视角）：⭐⭐⭐⭐⭐ — 需读懂并修改 C 语言写的 PostgreSQL 源码，工程量与底层理解要求都很高。
- **成绩组成**：Quizzes 15% + Assignment 1（新数据类型）15% + Assignment 2（数据库存储结构）20% + 期末考试 50%（期末为 hurdle，须 ≥40%；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先补牢 C 语言与指针 / 内存管理，再花时间读懂 PostgreSQL 相关源码模块的调用结构；作业务必尽早开始、用提供的测试子集边写边验证；把存储 → 索引 → 查询处理 → 事务这条内部数据流串成一条线来理解。

#### `COMP9321` — Data Services Engineering（数据服务工程）
- **课程简介**：面向"数据驱动的 Web 服务"的工程实战课。用 Python 从零构建 RESTful API、做数据的采集与发布，再把多源数据整合成 mashup 应用，最后接触数据分析 / 机器学习环节。偏应用与动手，作业密集。
- **主要知识点**：RESTful 服务 API 设计、Python Web 开发（Flask 等）、数据采集与清洗、数据发布与集成、数据 mashup 应用、数据可视化、数据分析 / 机器学习入门、服务部署。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念门槛中等，但作业数量多、动手工程量大，节奏紧。
- **成绩组成**：多个作业 + 期末考（近年期末约占 50%，如某年为 Quizzes 10% + A1 10% + A2 10% + A3 20% + 期末 50%）；各学期权重变动较大，以当学期 course outline 为准。
- **建议学习路线**（辅导视角）：先把 Python 与 Flask / REST 基础打牢，动手搭一个最小可运行 API；作业一环扣一环，务必按周跟进不要积压；A3 常涉及数据分析 / ML，提前熟悉 pandas 与基本建模流程。

### 人工智能 · 机器学习

#### `COMP3411 / COMP9814` — Artificial Intelligence / Extended Artificial Intelligence（人工智能 / 扩展人工智能）
- **课程简介**：UNSW 人工智能的"入门总览课"，一门课带你走遍 AI 的经典地图——从搜索、博弈、逻辑推理，到计算机视觉、强化学习和神经网络。COMP3411（本科）与 COMP9814（研究生"Extended"版，作业量与深度更高）合班授课，适合想先建立 AI 全局观再深入某一分支的同学。
- **主要知识点**：智能体与任务类型、路径搜索与启发式搜索、博弈搜索、约束满足（CSP）、逻辑智能体、不确定性推理、语言处理、计算机视觉、机器人学、强化学习、神经网络与深度学习。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 广度大于深度，概念多但每个点不算太深，难在编程作业（搜索 / 博弈 / 学习算法实现）和逻辑推理部分。
- **成绩组成**：Assignment 1 25% + Assignment 2 25% + 期末笔试 50%（COMP9814 比例通常一致但作业要求更高；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先把搜索（BFS / DFS / A*）和逻辑（命题 / 一阶逻辑、归结）这两块硬骨头啃透，是笔试拿分核心；作业尽早动手，尤其博弈与强化学习实现题耗时较长。

#### `COMP3431 / COMP9434` — Robotic Software Architecture（机器人软件架构）
- **课程简介**：一门"动手玩真机器人"的项目课，用 ROS2 和 TurtleBot3 让机器人自己建图、导航、感知并做决策。几乎没有考试，全靠小组做出能跑的机器人来评分，工程实践气息浓厚。
- **主要知识点**：AI 与机器人学导论、ROS / ROS2 机器人操作系统、机器人软件架构、地图构建与导航（SLAM）、机器人视觉与感知、规划与决策（经典规划 / 强化学习 / 认知架构）。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念门槛中等，难点在工程调试、团队协作和让真机器人稳定运行；C++ / Python 编程能力是前提。
- **成绩组成**：期中项目 + 报告 40%（第 5 周演示）+ 期末项目演示 + 报告 60%（第 10 周演示，报告第 11 周末交）；小组演示、个人提交报告（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：开学立刻熟悉 ROS2 基本概念（node / topic / tf）和 TurtleBot3 仿真环境；项目重在"能演示 + 讲清为什么这样跑"，尽早分工、留足调试时间，别等最后一周。

#### `COMP6713` — Natural Language Processing（自然语言处理）
- **课程简介**：UNSW 较新的 NLP 课程，聚焦现代自然语言处理技术，从文本表示到大模型时代的方法，含每周测验与实践项目。适合想进入 NLP / LLM 方向的同学。
- **主要知识点**：文本预处理与表示、词向量 / 词嵌入、语言模型、序列标注与分类、神经网络 NLP 方法、Transformer 与预训练模型、NLP 应用任务（含小组项目）。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 需要一定机器学习 / 深度学习基础，数学与编程要求较高，项目工作量大。
- **成绩组成**：据公开信息含每周 quiz、个人 assignment 与小组 project 三部分；官方 outline 需登录访问，具体占比未能核实，以当学期 course outline 为准。
- **建议学习路线**（辅导视角）：先补齐 Python + PyTorch 与基础 ML；每周 quiz 紧跟课堂，别积压；项目尽早选题并跑通 baseline，再迭代提升。

#### `COMP9414` — Artificial Intelligence（人工智能，研究生）
- **课程简介**：研究生版 AI 入门总览课，覆盖面与 COMP3411 类似但更偏"用 Python 实践现有 AI 工具"，从智能体、搜索、推理到神经网络与人机对齐机器人一网打尽。是很多 AI 方向研究生的第一门 AI 课。
- **主要知识点**：智能体与知识表示、神经网络、问题求解与搜索、强化学习（reward 而非 goal）、元启发式算法、计算机视觉、语言处理、不确定性推理、人机对齐智能机器人。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 广度型课程，概念多；难点是搜索 / 推理的严谨性和作业编程，注意期末有 hurdle。
- **成绩组成**：Assignment 1 25%（第 5 周）+ Assignment 2 25%（第 9 周）+ 期末笔试 50%（及格 hurdle：期末须至少 20/50；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：把搜索与逻辑 / 概率推理作为笔试重点复习，务必冲过期末 hurdle；两个 Python 编程作业按时完成，注意代码风格与分析同样计分。

#### `COMP9417` — Machine Learning and Data Mining（机器学习与数据挖掘）
- **课程简介**：UNSW 机器学习的核心主力课，系统讲透监督 / 无监督学习的理论、算法与实证三位一体。用 Python 从回归、分类一路推进到集成学习、神经网络和学习理论，是 ML 方向绕不开的基石课。
- **主要知识点**：回归、分类、决策树学习、核方法（SVM）、集成学习、神经网络、无监督学习（聚类 / 降维）、学习理论。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 数学要求高（线代 / 概率 / 微积分 / 优化），理论推导与编程实现并重，是本类课程中较硬核的一门。
- **成绩组成**：Homework 1 15% + Homework 2 15% + 小组 Project 20% + 期末笔试 50%（及格线 50/100；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先夯实线代与概率统计，跟着课程用 NumPy / sklearn 亲手实现算法；两次 homework 是理解关键，别拖；project 当作小型科研，注意报告质量。

#### `COMP9418` — Advanced Machine Learning（进阶机器学习）
- **课程简介**：机器学习的进阶深水区，聚焦概率图模型（Bayesian networks、Markov networks）的表示、精确 / 近似推断与学习。理论密度高，是想做概率建模、因果与结构化预测的进阶之选，前置需先修 COMP9417。（注：2026 handbook 标题已由旧称 "Advanced Topics in Statistical Machine Learning" 更新为 "Advanced Machine Learning"。）
- **主要知识点**：命题逻辑与概率论、贝叶斯网络、Markov 链与隐马尔可夫模型（HMM）、精确推断（变量消元、联合树）、MAP 推断与 Markov 网络、高斯贝叶斯网络、近似推断（信念传播、采样）、参数与结构学习。
- **整体难度**（辅导视角）：⭐⭐⭐⭐⭐ — 概率与数学要求非常高，推断算法抽象、期末含 hurdle，是本类课程最硬核的一门。
- **成绩组成**：Quizzes 10%（8 次取平均）+ Assignment 1 15%（第 5 周）+ Assignment 2 15%（第 9 周）+ 期末笔试 60%（hurdle：期末须 ≥24/60；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：务必先修并巩固 COMP9417 与概率论；每周 quiz 是逼你跟进推断算法的抓手；把变量消元 / 联合树 / 采样这几套推断流程手推一遍，期末 hurdle 不容有失。

#### `COMP9444` — Neural Networks and Deep Learning（神经网络与深度学习）
- **课程简介**：UNSW 深度学习的旗舰课，从感知机、反向传播一路讲到 CNN、RNN / LSTM、深度强化学习、生成模型与对抗训练，还涉及多模态学习与 AI 伦理。用 PyTorch 动手实现，是通往深度学习研究的核心课。
- **主要知识点**：感知机与多层网络、反向传播、交叉熵 / softmax / 权重衰减 / 动量、卷积网络（图像处理）、循环网络与 LSTM（语言处理、词向量）、深度强化学习、自编码器、生成模型与对抗训练、多模态学习、深度学习伦理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 数学（梯度、优化）与 PyTorch 编程要求高，小组项目工作量大，理论与工程双重挑战。
- **成绩组成**：个人 Assignment 20% + 课堂参与 5% + 小组 Project 30%（第 10 周展示）+ 期末考试 45%（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先熟练 PyTorch 张量与自动求导，把反向传播亲手推一遍；小组项目第 4 周前组队、尽早定题跑通 baseline；期末占比高，理论概念要系统复习。

#### `COMP9491` — Applied Artificial Intelligence（应用人工智能）
- **课程简介**：一门"整合型"高阶 AI 项目课，几乎全靠一个贯穿学期的小组项目评分。要求把计算机视觉、语言处理、深度学习、知识表示与推理等多种 AI 技术揉在一起，解决真实 / 工业级问题。适合已有 AI 基础、想练综合实战的同学。
- **主要知识点**：深度学习、计算机视觉、语言与语音处理、知识表示与推理（符号 AI）、多种 AI 方法的集成与应用、项目式研发全流程。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 单点难度不极端，但要求综合运用多种 AI 技术且全为团队项目，协作与工程整合能力是最大挑战；需先具备 ML / DL 基础。
- **成绩组成**：项目提案报告 10%（第 3 周）+ 文献综述展示 20%（第 5 周）+ 项目 demo 30%（第 10 周，含参与分）+ 项目报告 40%（第 11 周）；全部为小组评估（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先修 COMP9417 / 9444 等打底；第 2 周前尽快组队选题，提案阶段就想清楚"要整合哪几类 AI 技术"；把握文献综述与最终报告的写作质量，它们合计占 60%。

#### `COMP9517` — Computer Vision（计算机视觉）
- **课程简介**：UNSW 计算机视觉主力课，从传统图像处理、特征提取到深度学习视觉方法全覆盖。前半程每周实验打基础，后半程小组项目做真实视觉应用，理论与动手兼顾。
- **主要知识点**：图像处理基础、特征检测与描述、图像分割、目标检测与识别、运动与跟踪、深度学习视觉方法（CNN 等）、模式识别与分类。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 需要一定数学与 Python / OpenCV 基础，项目工作量大，深度学习部分有难度。
- **成绩组成**：Lab 任务 10%（个人，前半学期每周一次共约 4 次）+ 小组 Project 40%（第 5–10 周）+ 期末考试 50%（以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：前半学期跟着每周 lab 打牢 OpenCV / 图像处理基础；project 第 5 周开始尽早组队定题；期末占一半，传统方法与深度学习原理都要系统复习。

### 数据科学 · 数据分析

#### `COMP9312` — Data Analytics for Graphs（图数据分析）
- **课程简介**：专注于"图"这种数据结构的存储、查询与分析。你会学到如何在社交网络、知识图谱、交通网络这类由"点和边"构成的海量数据上高效地跑算法，并接触当下热门的图神经网络（GNN）。是数据科学方向里偏"结构化关系挖掘"的一门硬核课。
- **主要知识点**：图数据存储与索引、图查询处理、最短路径 / 连通性算法、稠密子图（cohesive subgraph）计算、图划分、图表示学习（node embedding）、图神经网络（GNN）。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 图算法的复杂度分析与大规模稀疏图上的工程实现是主要门槛，需要扎实的算法与数据结构基础。
- **成绩组成**：Assignment 1 15% + Assignment 2 10% + Project 25% + 期末考试 50%（期末与项目占比最重；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先补齐图论基础（BFS / DFS、最短路、连通分量）再进课程；两个 Assignment 侧重经典图算法实现，务必吃透复杂度分析；Project 通常涉及较大规模图数据，早动手、注意内存与效率优化。

#### `COMP9313` — Big Data Management（大数据管理）
- **课程简介**：这是数据科学方向最经典的"大数据工程"课。围绕如何在成百上千台机器上存储和处理 TB 级数据展开，核心是 Hadoop 生态（MapReduce / HDFS / Hive / HBase）和内存计算框架 Spark。学完你能独立写出可扩展的分布式数据处理程序。
- **主要知识点**：MapReduce 编程模型、HDFS / YARN、Hive 与 HBase、Spark（RDD / DataFrame）、大规模算法设计、数据流挖掘（data stream mining）、相似项检测（LSH / MinHash）、图数据处理、NoSQL。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 分布式"换脑子"的思维方式（把问题拆成 map / reduce）加上 Spark / Scala 环境配置，是初学者最大的坎；期末笔试还要求手写算法逻辑。
- **成绩组成**：Coding Project 1 12% + Coding Project 2 16% + Coding Project 3 22% + 期末考试（线下）50%（期末须至少 20/50 才能及格 hurdle；以当学期 course outline 为准）。
- **建议学习路线**（辅导视角）：先熟悉 Java / Scala 与命令行环境，尽早搭好 Hadoop / Spark 本地环境；三个 Project 难度递增，Project 3 占比最大要留足时间；期末有 hurdle，务必系统复习 MapReduce / Spark 算法设计的手写题型。

#### `INFS2608` — Database Management & Big Data Infrastructures（数据库管理与大数据基础设施）
- **课程简介**：商学院信息系统方向的进阶数据库课，从"业务应用"视角看数据管理。既覆盖关系型数据库的进阶主题，也延伸到数据仓库、商业智能（BI）与大数据分析基础设施，强调在真实商业场景下做数据库设计与分析。
- **主要知识点**：进阶数据库管理、数据仓库、商业智能（BI）、大数据基础与分析、关系型与分析型数据系统架构、真实场景数据库设计 / 分析实践。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念覆盖面广但偏应用、少重理论，对有 INFS1603 基础（先修要求）的商科学生较友好，实践项目是主要投入点。
- **成绩组成**：官方 course outline 页面需登录，2026 具体评估项占比未能核实，以当学期 course outline 为准。
- **建议学习路线**（辅导视角）：确保先修 INFS1603 的 SQL 与关系建模扎实；课程实践项目围绕真实数据库设计 / 分析场景，重点练习需求到 schema 的转化与 BI / 数据仓库建模；平时按周完成 lab，避免 project 阶段赶工。

---

## 完整课程清单（按类型）

**编程 · 软件工程 · 项目**

- `COMP1010` — The Art of Computing
- `COMP1511 / COMP1911` — Programming Fundamentals
- `COMP1531` — Software Engineering Fundamentals
- `COMP2041 / COMP9044` — Software Construction: Techniques and Tools
- `COMP2511` — Object-Oriented Design & Programming
- `COMP3141` — Software System Design and Implementation
- `COMP6080` — Web Front-End Programming
- `COMP9020` — Foundations of Computer Science
- `COMP9319` — Web Data Compression and Search
- `COMP9820` — Software Project Management
- `COMP9900` — Information Technology Project

**算法 · 数据结构 · 理论**

- `COMP2521` — Data Structures and Algorithms
- `COMP3161 / COMP9164` — Concepts of Programming Languages
- `COMP9021` — Principles of Programming
- `COMP9024` — Data Structures and Algorithms

**计算机系统 · 体系结构**

- `COMP3231 / COMP9201` — Operating Systems
- `COMP3891 / COMP9283` — Extended Operating Systems
- `COMP9242` — Advanced Operating Systems
- `COMP9334` — Capacity Planning of Computer Systems and Networks
- `COMP6771` — Advanced C++ Programming

**计算机网络**

- `COMP3331 / COMP9331` — Computer Networks and Applications

**数据库 · 信息系统**

- `COMP3311 / COMP9311` — Database Systems
- `COMP6714` — Information Retrieval and Web Search
- `COMP9315` — Database Systems Implementation
- `COMP9321` — Data Services Engineering

**人工智能 · 机器学习**

- `COMP3411 / COMP9814` — Artificial Intelligence / Extended Artificial Intelligence
- `COMP3431 / COMP9434` — Robotic Software Architecture
- `COMP4418` — Knowledge Representation and Reasoning
- `COMP6713` — Natural Language Processing
- `COMP9414` — Artificial Intelligence
- `COMP9417` — Machine Learning and Data Mining
- `COMP9418` — Advanced Machine Learning
- `COMP9444` — Neural Networks and Deep Learning
- `COMP9491` — Applied Artificial Intelligence
- `COMP9517` — Computer Vision

**数据科学 · 数据分析**

- `COMP9312` — Data Analytics for Graphs
- `COMP9313` — Big Data Management
- `INFS2608` — Database Management & Big Data Infrastructures

**网络安全**

- `COMP6441 / COMP6841` — Security Engineering and Cyber Security
- `COMP6843` — Extended Web Application Security and Testing
- `COMP6845` — Extended Digital Forensics and Incident Response
- `COMP9447` — Security Engineering Workshop

---

## 资料来源（官方，2026）

- UNSW Handbook 2026：[COMP1511](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP1511)、[COMP2521](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP2521)、[COMP3311](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP3311)、[COMP9417](https://www.handbook.unsw.edu.au/postgraduate/courses/2026/COMP9417)、[COMP9444](https://www.handbook.unsw.edu.au/postgraduate/courses/2026/COMP9444)（其余单元同址，将 URL 末段替换为对应课程号即可；COMP9xxx 走 postgraduate 路径）
- UNSW CSE 课程 outline（webcms3 / cgi.cse.unsw.edu.au，按 term 更新，成绩组成以当学期 outline 为准）

> 「整体难度 / 建议学习路线」为辅导视角的主观参考；UNSW 各 term 的评估占比常有微调，正式选课与评估请以对应 term 的官方 course outline 为准。

---

## 需要按 UNSW 定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
