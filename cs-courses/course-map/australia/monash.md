---
title: 莫纳什大学（Monash University）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 4
permalink: /cs-courses/course-map/australia/monash/
published_at: "2026-07-05 17:18:05"
---

# 莫纳什大学（Monash University）

Monash CS 采用 **FIT** 课程编码（数学类为 **MAT**），本科（FIT1xxx–FIT4xxx）与研究生（FIT5xxx / FIT9xxx）课程合并整理。下方先给出**核心 / 高频课程详解**，再附**完整课程清单**（均**按课程类型归类**）。

> 说明：每门课的 **课程简介 · 主要知识点 · 成绩组成** 依据 Monash **2026 官方 handbook / unit guide** 整理；**整体难度 · 建议学习路线** 为 **辅导视角**（主观参考，因人而异）。部分课程 2026 年处于考核改版过渡期，成绩组成最终一律以当学期 unit guide 为准。来源见页面底部。

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### `FIT1045` — Introduction to Programming（编程入门）
- **课程简介**：Monash 计算机专业的第一门编程课，使用 **Python** 从零教起。它不只是教语法，而是训练你"像程序员一样思考"——把一个现实问题拆解成算法，再用代码实现，并评估算法的效率与局限。是整个 CS 学位的基石课。
- **主要知识点**：Python 基础语法、控制结构（分支 / 循环）、数据类型、函数与模块化、递归、算法设计与问题分解、计算成本与算法复杂度评估、算法的局限性。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 语法本身不难，真正的坎在"算法思维"和递归：很多零基础同学卡在如何把问题抽象成可编程的步骤。
- **成绩组成**：Workshops 12% + Tutorial Preparation 8% + In-semester Tests 8% + Assignment 22% + 期末考试（2h10m）50%（即平时 50% + 期末 50%；通常设有 hurdle 门槛，考试与平时分各需约 45%，以当学期 unit guide 为准）。
- **建议学习路线**（辅导视角）：从第一周起坚持每天写代码，把 tutorial preparation 当作硬任务完成，切勿积压。重点攻克递归和循环不变式。学完可顺利衔接 FIT1008 / FIT2004（数据结构与算法）；有基础的同学可考虑进阶版 FIT1053。

#### `FIT1050` — Web Fundamentals（Web 基础）
- **课程简介**：面向 Web 开发的入门课，带你俯瞰整个 Web 技术生态。它强调"广度优先"——让你理解一个真实 Web 系统从前端到后端会涉及哪些技术、每种技术的取舍，以及开发者需要解决的关键问题，并通过团队项目动手做出一个网站。
- **主要知识点**：Web 与 Web 应用核心技术、前端页面构建、Web 技术的优劣势与适用场景对比、Web 应用开发基本任务、团队协作开发流程。
- **整体难度**（辅导视角）：⭐⭐☆☆☆ — 概念多但深度浅，压力主要来自多个连续的实践作业和团队协作，而非技术难度本身。
- **成绩组成**：期末考试（2h10m）40% + Assignment 1 个人展示 10% + Assignment 2 网站重设计 15% + Assignment 3 网站开发 25% + 参与里程碑 10%（平时 60% + 期末 40%）。
- **建议学习路线**（辅导视角）：把三个作业当成一条递进的项目线来经营，动手实践 HTML / CSS / JS 越早越好，团队作业要尽早分工。这门课是通往 FIT2095（全栈开发）的良好铺垫。

#### `FIT1051 / FIT9131` — Programming Fundamentals in Java / Programming Foundations in Java（Java 编程基础）
- **课程简介**：这是一对"孪生课"——**FIT1051 面向本科生**、**FIT9131 面向研究生**，都用 **Java** 教授编程基础，核心都是把问题规格翻译成程序设计再实现为代码。FIT1051 更贴近工业级软件开发语境（SDLC、API 库、多类应用）；FIT9131 则更侧重面向零基础研究生的软件工程原则（可维护性、可读性、模块化，使用 BlueJ 环境）。
- **主要知识点**：Java 语法、变量与数据类型、控制结构、方法与模块化、值类型与引用类型、自定义类与对象、继承与接口、多类应用开发、测试与调试、面向对象基础概念、代码规范与职业伦理。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — Java 的强类型和面向对象概念（类 / 对象 / 继承）是主要门槛，尤其对零基础的研究生（FIT9131）而言，OO 思维的建立需要时间。
- **成绩组成**：
  - FIT1051：Pre-reading Quizzes 10% + Workshop / Short Quizzes 10% + Laboratory Assessments 20% + 期末考试（3h10m）60%。
  - FIT9131：Pre-tutorial tasks 5% + Assignment 1 10% + Assignment 2 25% + 期末考试（2h10m）60%（以当学期 unit guide 为准）。
- **建议学习路线**（辅导视角）：先吃透"类与对象"这一核心，多用 BlueJ / IDE 动手建对象观察运行，每周 lab 不要拖。这门课是 FIT2099（面向对象设计）和后续 Java 项目课的直接前置。

#### `FIT2001` — Systems Development（系统开发）
- **课程简介**：从"写代码"转向"设计系统"的关键课。它教你在某种方法论框架下，把系统分析与设计当作解决问题的过程——如何采集需求、建模需求、做原型和界面设计，同时培养系统开发所需的职业软技能，贴近当代行业实践。
- **主要知识点**：系统开发方法论、系统分析与设计流程、需求采集与需求建模、不同抽象层次的问题求解、原型设计与界面设计、职业实践技能。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 编程量不大，难在"从技术思维切换到分析设计思维"，需求建模（如用例 / 流程图）需要严谨和规范。
- **成绩组成**：期末考试（2h10m）50% + 平时 50%（每周 workshop 测验与参与 8% + Assignment 1 需求采集 5% + Assignment 2 需求建模 25% + Assignment 3 原型与界面设计 12%）。
- **建议学习路线**（辅导视角）：把三个作业看作一个完整项目的三个阶段，前后衔接理解，重点练习需求建模的规范表达。可与 FIT2101 / FIT2107（软件工程过程 / 质量测试）互为补充。

#### `FIT2095` — Full Stack Development（全栈开发）
- **课程简介**：Monash 最受欢迎的实战课之一，教你用 JavaScript 全栈技术栈（Node.js + Express + Angular / React + MongoDB 这一类现代栈）从零构建 Web 与移动应用。覆盖前端到后端到数据库的完整链路，强调工业级技术与职业化的编程规范。（注：该课程 2026 handbook 标题已由旧称 "e-Business software technologies" 更新为 "Full stack development"。）
- **主要知识点**：HTML5 / CSS3、现代 JavaScript（ES2015+ / 面向对象）、Ajax / JSON / XML、MVC 架构、Node.js、Angular / React、TypeScript、MongoDB、核心 API 使用、应用调试、良好编程实践与职业伦理。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 技术栈广而杂，异步编程、前后端联调和 MongoDB 数据建模是主要难点，作业节奏快、工程量大。
- **成绩组成**：Laboratory Assessments（11 次）20% + Workshop Quizzes（11 次）10% + Pre-reading Quizzes 10% + 期末考试（2h10m）60%（因课程改版占比可能调整，以当学期 unit guide 为准）。
- **建议学习路线**（辅导视角）：先把 JavaScript 异步（Promise / async-await）和 Node 基础打牢，再逐层往上叠框架，每周 lab 紧跟不掉队。建议先修 FIT1050（Web 基础），学完可承接 FIT5032 / 大型 Web 项目课。

#### `FIT2099` — Object Oriented Design and Implementation（面向对象设计与实现）
- **课程简介**：把 Java 编程能力升华为"设计能力"的核心课。它教你用面向对象设计原则去构建高质量软件——先用 UML 迭代地设计中小型系统，评估设计质量，再用 Java 实现，并借助 UML 工具和版本控制系统化地开发和调试。
- **主要知识点**：面向对象设计原则、UML 建模（类图等）、迭代式设计、设计质量评估、Java 实现、系统化调试、软件工程工具（UML 编辑器、版本控制 Git）。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 难在"好设计"没有唯一答案，设计原则（职责分配、可扩展性）的权衡需要经验；把 UML 设计准确落地为代码也考验功力。
- **成绩组成**：Java Bootcamp 10% + Assignment 1 15% + Assignment 2 15% + Assignment 3 20% + 期末考试（2h10m）40%（平时 60% + 期末 40%）。
- **建议学习路线**（辅导视角）：先修 FIT1051 / FIT9131 打好 Java 与 OO 基础。学习时不要只求"能跑"，要反复推敲设计是否符合原则、是否易扩展；三个作业通常层层递进，务必吃透前一个再做下一个。

#### `FIT9136` — Introduction to Python Programming（Python 编程入门）
- **课程简介**：面向研究生的 Python 入门课（2026 handbook 标题为 "Introduction to Python programming"，旧称 "Algorithms and programming foundations in Python"）。它同时教 Python 编程与基础数据结构和算法——从设计、分析到实现，涵盖列表、栈、队列、树、递归以及排序 / 查找算法，是许多 IT / 数据科学硕士的第一门编程课。
- **主要知识点**：Python 语法与程序设计、基本数据类型与数据结构（列表 / 栈 / 队列 / 树）、递归、排序与查找算法、算法复杂度分析、程序测试与文档。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 语法友好，但对零基础研究生而言，把编程与"数据结构 + 算法复杂度"打包一起学，后半程（树、递归、复杂度）会明显加速。
- **成绩组成**：Assignment 1 15% + In-semester Test（45 分钟）15% + Assignment 2 20% + 期末考试（2h10m）50%（以当学期 unit guide 为准）。
- **建议学习路线**（辅导视角）：前四周把 Python 基础和函数练熟，中期重点攻数据结构与递归，最后系统复习算法复杂度。是研究生转向 FIT5xxx 编程 / 数据类课程的敲门砖。

### 算法 · 数据结构 · 理论

#### `FIT1008` — Fundamentals of Algorithms（算法基础）
- **课程简介**：Monash CS 学生真正的"算法与数据结构入门课"（2026 起由旧称 *Introduction to Computer Science* 更名重构）。你将学会把一个问题陈述转化为结构良好的计算解决方案：选对数据结构、设计高效算法，并权衡正确性、性能与可维护性。
- **主要知识点**：递归、入门复杂度分析、栈与队列、树、堆、哈希表、算法的理论与实验性能评估、时间 / 空间权衡、程序设计与测试。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 对大一学生而言节奏快、抽象度陡增，递归与复杂度分析是第一道大坎。
- **成绩组成**：2026 年处于改版过渡期，存在两种考核形式——新版（Sem 2, 2026 起）为 **Portfolio 100%**（持续性作品集考核）；旧版（Sem 1, 2026）为 **在学期测验 30% + 项目 / 期末 40% + 其余测验**。以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：这是后续 FIT2004、FIT3155 的直接先修，务必把递归和 Big-O 打扎实。建议同步修读 MAT1830（离散数学）支撑复杂度证明，平时多手写数据结构而非只靠库函数。

#### `FIT2004` — Algorithms and Data Structures（算法与数据结构）
- **课程简介**：Monash CS 的核心"硬课"之一，系统训练算法设计与分析的科学方法。从问题规格化到算法设计、复杂度分析再到实现，是通往高级算法与技术面试的必经之路。
- **主要知识点**：最好 / 平均 / 最坏情况的时间与空间复杂度分析、递归、高级数据结构（堆、B 树）、哈希、排序算法、搜索算法、图算法、数值计算。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 内容密度大、证明与实现并重，图算法与复杂度分析是主要拉分点。
- **成绩组成**：2026 handbook 显示为 **Portfolio（作品集 / 持续性考核）100%**（含 Quiz / Test 组件，设有阈值 hurdle 门槛）。具体各次作业占比以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：先修 FIT1008 / FIT1054。开课前复习递归与 Big-O；学期中按周跟进图算法（最短路、MST、网络流）并动手实现，避免期末堆积。是 FIT3155 的直接先修。

#### `FIT2014` — Theory of Computation（计算理论）
- **课程简介**：一门"烧脑但优雅"的理论课，回答"计算机到底能算什么、不能算什么"。带你走进形式语言、自动机与计算复杂度的世界，并系统训练严格的数学证明能力。
- **主要知识点**：有限状态自动机、正则表达式、文法、下推自动机、可计算函数、图灵机、多项式时间归约、复杂度类 P 与 NP、NP 完全性、形式化证明写作。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 抽象、偏数学，写形式证明对很多同学是最大挑战。
- **成绩组成**：Written 20% + Project 15% + 期末考试（Examination）50% + 其余组件（约 5% + 10%，视 offering 而定）；设有阈值 hurdle 门槛。以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：数学证明基础是关键，建议先巩固 MAT1830（离散数学）。把每周的自动机 / 归约例题独立重做，NP 完全性部分要理解归约构造而非死记，考前重点练证明表达。

#### `FIT2085` — Fundamentals of Algorithms for Engineers（工程师算法基础）
- **课程简介**：这是 FIT1008 面向工程学院学生的等价变体版本，内容与 FIT1008 高度一致，但结合工程语境教学。学习目标与数据结构 / 算法核心内容相同，供工程专业学生修读。
- **主要知识点**：递归、入门复杂度分析、栈与队列、树、堆、哈希表、算法性能的理论与实验评估、程序设计、实现与测试。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 与 FIT1008 难度相当，对非 CS 背景的工程学生抽象门槛偏高。
- **成绩组成**：同处 2026 改版过渡期——新版为 **Portfolio 100%**；旧版含 **Portfolio 30% + 项目 40% + 测验 30%** 等组件。以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：与 FIT1008 学习策略一致，重在多写代码、吃透递归与复杂度。工程学生尤其要补齐编程手感，可把课堂数据结构逐一自己实现一遍。

#### `FIT2102` — Programming Paradigms（编程范式）
- **课程简介**：一门拓宽编程视野的课——就像学习不同语法的自然语言，不同"范式"的编程语言在表达力与效率上迥异。你将深入函数式与声明式编程，理解语言设计原理，学会用更优雅、正确、可维护的方式解决问题。
- **主要知识点**：函数式编程、声明式编程、编程语言设计原理与演化、低级到高级范式对比、语言表达力与效率、范式间的比较与权衡（常用 Haskell / TypeScript 等）。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 思维方式转变（从命令式到函数式）是最大障碍，上手陡但回报高。
- **成绩组成**：Assignment 1（Project）+ Assignment 2（Project）+ Quiz + 课堂练习（Exercise），各组件约 20–30%（合计 100%）；设有两处 45% 门槛（两次作业合计、worksheet 与 quiz 合计）。以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：先修 FIT1008 / FIT2004。提前熟悉函数式语言（高阶函数、递归、纯函数、类型系统），每周跟做 worksheet 保持手感，两个大作业尽早动手。

#### `FIT3155` — Advanced Data Structures and Algorithms（高级数据结构与算法）
- **课程简介**：FIT2004 的进阶延续，聚焦解决真实世界编程难题所需的高级算法范式。深入研究空间高效的数据结构与时间高效的求解策略，是算法竞赛与高强度技术面试的"利器课"。
- **主要知识点**：摊还分析（amortized analysis）、高级排序与搜索算法、新型树 / 字符串 / 图数据结构与算法、数论算法等。
- **整体难度**（辅导视角）：⭐⭐⭐⭐⭐ — Monash 算法方向难度天花板，字符串算法与摊还分析对多数学生极具挑战。
- **成绩组成**：Artefact 1（作业）20% + Artefact 2（作业）20% + 期末考试（Examination）60%；设有阈值门槛（期末 ≥45%、平时 ≥45%、总分 ≥50%）。以当学期 unit guide 为准。
- **建议学习路线**（辅导视角）：务必先扎实完成 FIT2004。开课前复习图算法与复杂度分析；学期中紧跟字符串算法（后缀树 / 数组、Z-algorithm 等）逐一实现，期末占比高须持续复习。

> 其余课程类型（计算机系统 · 体系结构、计算机网络、数据库 · 信息系统、人工智能 · 机器学习、数据科学 · 数据分析）的核心课详解，正按同样标准补充中。想优先哪几门？→ [联系我](/contact/)。

---

## 完整课程清单（按类型）

**编程 · 软件工程 · 项目**

- `FIT1045` — Introduction to Programming
- `FIT1050` — Web Fundamentals
- `FIT1051` — Programming Fundamentals in Java
- `FIT1053` — Introduction to Programming (Advanced)
- `FIT1055` — IT Professional Practice and Ethics
- `FIT1056` — Introduction to Software Engineering
- `FIT1058` — Foundations of Computing
- `FIT2001` — Systems Development
- `FIT2002` — IT Project Management
- `FIT2032` — Industry-Based Learning
- `FIT2082` — Computer Science Research Project
- `FIT2083` — Innovation and Research in Computer Science
- `FIT2095` — Full Stack Development
- `FIT2099` — Object Oriented Design and Implementation
- `FIT2101` — Software Engineering Process and Management
- `FIT2107` — Software Quality and Testing
- `FIT2108` — Industry Based Learning Seminar
- `FIT2175` — Usability
- `FIT3045` — Industry-Based Learning
- `FIT3144` — Advanced Computer Science Research Project
- `FIT3158` — Business Decision Modelling
- `FIT3161` — Computer Science Project 1
- `FIT3162` — Computer Science Project 2
- `FIT3170` — Software Engineering Practice
- `FIT4701` — Final Year Software Engineering Project A
- `FIT4702` — Final Year Software Engineering Project B
- `FIT5032` — Internet Applications Development
- `FIT5057` — Project Management
- `FIT5094` — IT for Management Decision Making
- `FIT5102` — IT Strategy and Governance
- `FIT5107` — Recordkeeping Informatics
- `FIT5136` — Software Engineering
- `FIT5152` — User Interface Design and Usability
- `FIT5160` — Business Process Modelling, Design and Simulation
- `FIT5190` — Introduction to IT Research Methods
- `FIT5206` — Digital Continuity
- `FIT5231` — Indigenous Data Sovereignty
- `FIT5238` — Information Technology Systems Capstone Project
- `FIT9131` — Programming Foundations in Java
- `FIT9136` — Introduction to Python Programming

**算法 · 数据结构 · 理论**

- `FIT1008` — Fundamentals of Algorithms
- `FIT1054` — Fundamentals of Algorithms (Advanced)
- `MAT1830` — Discrete Mathematics for Computer Science
- `MAT1841` — Continuous Mathematics for Computer Science
- `FIT2004` — Algorithms and Data Structures
- `FIT2014` — Theory of Computation
- `FIT2085` — Fundamentals of Algorithms for Engineers
- `FIT2102` — Programming Paradigms
- `FIT3139` — Computational Modelling and Simulation
- `FIT3155` — Advanced Data Structures and Algorithms
- `FIT5216` — Modelling Discrete Optimisation Problems

**计算机系统 · 体系结构**

- `FIT1060` — Pervasive Computing
- `FIT2100` — Operating Systems
- `FIT3077` — Software Engineering: Architecture and Design
- `FIT3143` — Parallel Computing
- `FIT3159` — Computer Architecture
- `FIT5046` — Mobile and Distributed Computing Systems
- `FIT5171` — System Validation and Verification, Quality and Standards
- `FIT5236` — Enterprise Applications and Architecture
- `FIT9137` — Introduction to Computer Architecture and Networks

**计算机网络**

- `FIT2165` — Computer Networks
- `FIT3165` — Computer Networks
- `FIT4165` — Computer Networks

**数据库 · 信息系统**

- `FIT1006` — Business Information Analysis
- `FIT2090` — Business Information Systems and Processes
- `FIT2094` — Databases
- `FIT2104` — Web Database Interface
- `FIT3171` — Databases
- `FIT3176` — Advanced Database Design
- `FIT5137` — Advanced Database Technology
- `FIT5234` — Advanced Business Information Systems Analysis and Design
- `FIT9123` — Fundamentals of Business Information Systems
- `FIT9132` — Introduction to Databases
- `FIT9138` — Information Systems Analysis, Design and Systems Thinking

**人工智能 · 机器学习**

- `FIT1059` — AI for Everyone
- `FIT1061` — Introduction to Artificial Intelligence
- `FIT2110` — Human-Centred Artificial Intelligence
- `FIT3080` — Artificial Intelligence
- `FIT3181` — Deep Learning
- `FIT5047` — Fundamentals of Artificial Intelligence
- `FIT5201` — Machine Learning
- `FIT5215` — Deep Learning
- `FIT5217` — Natural Language Processing
- `FIT5226` — Multi-Agent Systems and Collective Behaviour
- `FIT5230` — Malicious AI

**数据科学 · 数据分析**

- `FIT1043` — Introduction to Data Science
- `FIT2086` — Modelling for Data Analysis
- `FIT2179` — Data Visualisation
- `FIT3003` — Business Intelligence and Data Warehousing
- `FIT3152` — Data Analytics
- `FIT3154` — Advanced Data Analysis
- `FIT3163` — Data Science Project 1
- `FIT3164` — Data Science Project 2
- `FIT3179` — Data Visualisation
- `FIT3182` — Big Data Management and Processing
- `FIT5145` — Foundations of Data Science
- `FIT5147` — Data Exploration and Visualisation
- `FIT5149` — Applied Data Analysis
- `FIT5196` — Data Wrangling
- `FIT5197` — Statistical Data Modelling
- `FIT5202` — Data Processing for Big Data
- `FIT5212` — Data Analysis for Semi-structured Data
- `FIT5235` — Business Intelligence and Analytics

**网络安全**

- `FIT1057` — Introduction to Cybersecurity
- `FIT1093` — Cybersecurity Tools and Techniques
- `FIT2093` — Cybersecurity Tools and Techniques
- `FIT2173` — Software Security
- `FIT3031` — Network Security
- `FIT3168` — IT Forensics
- `FIT3183` — Malicious AI and Dark Side Security
- `FIT3188` — Cybersecurity Project 1
- `FIT5003` — Software Security
- `FIT5037` — Network Security
- `FIT5129` — Cyber Operations
- `FIT5163` — Introduction to Cryptography for Cybersecurity
- `FIT5225` — Cloud Computing and Security

---

## 资料来源（官方，2026）

- Monash Handbook 2026：[FIT1045](https://handbook.monash.edu/2026/units/FIT1045)、[FIT2004](https://handbook.monash.edu/2026/units/FIT2004)、[FIT2099](https://handbook.monash.edu/2026/units/FIT2099)、[FIT2095](https://handbook.monash.edu/2026/units/FIT2095)、[FIT2014](https://handbook.monash.edu/2026/units/FIT2014)、[FIT3155](https://handbook.monash.edu/2026/units/FIT3155)（其余单元同址，将 URL 末段替换为对应课程号即可）
- 各单元每学期 unit guide / Moodle（成绩组成以当学期 unit guide 为准）

> 「整体难度 / 建议学习路线」为辅导视角的主观参考；部分课程 2026 年处于考核改版过渡期，正式选课与评估请以对应学期的官方 unit guide 为准。

---

## 需要按这所学校定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
