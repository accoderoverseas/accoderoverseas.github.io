---
title: 莫纳什大学（Monash University）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 4
permalink: /cs-courses/course-map/australia/monash/
published_at: "2026-07-05 17:18:05"
---

<style>
/* 课程号-课程名统一紫色加粗（仅本页生效）：第一部分课程小标题 + 第二部分清单条目 */
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 莫纳什大学（Monash University）

Monash CS 采用 **FIT** 课程编码（数学类为 **MAT**），本科（FIT1xxx–FIT4xxx）与研究生（FIT5xxx / FIT9xxx）课程合并整理。下方先给出**核心 / 高频课程详解**，再附**完整课程清单**（均**按课程类型归类**）。

> 说明：每门课的 **课程简介 · 主要知识点 · 成绩组成** 依据 Monash **2026 官方 handbook / unit guide** 整理；**整体难度 · 建议学习路线** 为 **主观经验参考**（因人而异）。部分课程 2026 年处于考核改版过渡期，成绩组成最终一律以当学期 unit guide 为准。来源见页面底部。

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### `FIT1045` — Introduction to Programming（编程入门）
- **课程简介**：Monash 计算机专业的第一门编程课，使用 **Python** 从零教起。它不只是教语法，而是训练你"像程序员一样思考"——把一个现实问题拆解成算法，再用代码实现，并评估算法的效率与局限。是整个 CS 学位的基石课。
- **主要知识点**：Python 基础语法、控制结构（分支 / 循环）、数据类型、函数与模块化、递归、算法设计与问题分解、计算成本与算法复杂度评估、算法的局限性。
- **整体难度**：⭐⭐⭐☆☆ — 语法本身不难，真正的坎在"算法思维"和递归：很多零基础同学卡在如何把问题抽象成可编程的步骤。
- **成绩组成**：Workshops 12% + Tutorial Preparation 8% + In-semester Tests 8% + Assignment 22% + 期末考试（2h10m）50%（即平时 50% + 期末 50%；通常设有 hurdle 门槛，考试与平时分各需约 45%，以当学期 unit guide 为准）。
- **建议学习路线**：零基础也完全能选，关键是从第一周就每天动手写一点，别把 tutorial preparation 攒着——它其实是帮你不掉队的缓冲。递归和循环不变式是最容易卡住你的地方，卡住很正常，多画几遍执行过程就通了。学完你就能顺畅接上 FIT1008 / FIT2004；本来就有底子的话可以直接挑战进阶版 FIT1053。

#### `FIT1050` — Web Fundamentals（Web 基础）
- **课程简介**：面向 Web 开发的入门课，带你俯瞰整个 Web 技术生态。它强调"广度优先"——让你理解一个真实 Web 系统从前端到后端会涉及哪些技术、每种技术的取舍，以及开发者需要解决的关键问题，并通过团队项目动手做出一个网站。
- **主要知识点**：Web 与 Web 应用核心技术、前端页面构建、Web 技术的优劣势与适用场景对比、Web 应用开发基本任务、团队协作开发流程。
- **整体难度**：⭐⭐☆☆☆ — 概念多但深度浅，压力主要来自多个连续的实践作业和团队协作，而非技术难度本身。
- **成绩组成**：期末考试（2h10m）40% + Assignment 1 个人展示 10% + Assignment 2 网站重设计 15% + Assignment 3 网站开发 25% + 参与里程碑 10%（平时 60% + 期末 40%）。
- **建议学习路线**：如果你想入门 Web 又怕难，这门课很适合——技术难度不高，选了会学得比较轻松。真正需要留意的是三个作业连着来、还有团队协作，所以别拖：把三个作业当成一条递进的项目线，HTML / CSS / JS 越早上手越好，团队作业一拿到就分工。学完它，你去修 FIT2095（全栈开发）会顺很多。

#### `FIT1051 / FIT9131` — Programming Fundamentals in Java / Programming Foundations in Java（Java 编程基础）
- **课程简介**：这是一对"孪生课"——**FIT1051 面向本科生**、**FIT9131 面向研究生**，都用 **Java** 教授编程基础，核心都是把问题规格翻译成程序设计再实现为代码。FIT1051 更贴近工业级软件开发语境（SDLC、API 库、多类应用）；FIT9131 则更侧重面向零基础研究生的软件工程原则（可维护性、可读性、模块化，使用 BlueJ 环境）。
- **主要知识点**：Java 语法、变量与数据类型、控制结构、方法与模块化、值类型与引用类型、自定义类与对象、继承与接口、多类应用开发、测试与调试、面向对象基础概念、代码规范与职业伦理。
- **整体难度**：⭐⭐⭐☆☆ — Java 的强类型和面向对象概念（类 / 对象 / 继承）是主要门槛，尤其对零基础的研究生（FIT9131）而言，OO 思维的建立需要时间。
- **成绩组成**：
  - FIT1051：Pre-reading Quizzes 10% + Workshop / Short Quizzes 10% + Laboratory Assessments 20% + 期末考试（3h10m）60%。
  - FIT9131：Pre-tutorial tasks 5% + Assignment 1 10% + Assignment 2 25% + 期末考试（2h10m）60%（以当学期 unit guide 为准）。
- **建议学习路线**：Java 的强类型和"类 / 对象 / 继承"听起来吓人，但你只要抓住"类与对象"这一个核心慢慢建立直觉就不难了，尤其零基础的研究生别急，OO 思维本来就需要一点时间。学的时候多用 BlueJ / IDE 亲手建对象、看它怎么跑，每周 lab 跟上别攒。打好这门，你后面修 FIT2099（面向对象设计）和各种 Java 项目课都会踏实很多。

#### `FIT2001` — Systems Development（系统开发）
- **课程简介**：从"写代码"转向"设计系统"的关键课。它教你在某种方法论框架下，把系统分析与设计当作解决问题的过程——如何采集需求、建模需求、做原型和界面设计，同时培养系统开发所需的职业软技能，贴近当代行业实践。
- **主要知识点**：系统开发方法论、系统分析与设计流程、需求采集与需求建模、不同抽象层次的问题求解、原型设计与界面设计、职业实践技能。
- **整体难度**：⭐⭐⭐☆☆ — 编程量不大，难在"从技术思维切换到分析设计思维"，需求建模（如用例 / 流程图）需要严谨和规范。
- **成绩组成**：期末考试（2h10m）50% + 平时 50%（每周 workshop 测验与参与 8% + Assignment 1 需求采集 5% + Assignment 2 需求建模 25% + Assignment 3 原型与界面设计 12%）。
- **建议学习路线**：这门课编程量不大，别以为轻松——它的挑战在于让你从"写代码"切到"分析设计"的思维，需求建模（用例、流程图）讲究规范，一开始不适应很正常。学的时候把三个作业当成同一个项目的三个阶段前后串起来理解，重点把需求建模的规范表达练顺。想更完整地搭软工体系，可以搭配 FIT2101 / FIT2107（软件工程过程 / 质量测试）一起看。

#### `FIT2095` — Full Stack Development（全栈开发）
- **课程简介**：Monash 最受欢迎的实战课之一，教你用 JavaScript 全栈技术栈（Node.js + Express + Angular / React + MongoDB 这一类现代栈）从零构建 Web 与移动应用。覆盖前端到后端到数据库的完整链路，强调工业级技术与职业化的编程规范。（注：该课程 2026 handbook 标题已由旧称 "e-Business software technologies" 更新为 "Full stack development"。）
- **主要知识点**：HTML5 / CSS3、现代 JavaScript（ES2015+ / 面向对象）、Ajax / JSON / XML、MVC 架构、Node.js、Angular / React、TypeScript、MongoDB、核心 API 使用、应用调试、良好编程实践与职业伦理。
- **整体难度**：⭐⭐⭐⭐☆ — 技术栈广而杂，异步编程、前后端联调和 MongoDB 数据建模是主要难点，作业节奏快、工程量大。
- **成绩组成**：Laboratory Assessments（11 次）20% + Workshop Quizzes（11 次）10% + Pre-reading Quizzes 10% + 期末考试（2h10m）60%（因课程改版占比可能调整，以当学期 unit guide 为准）。
- **建议学习路线**：这门很值得选，但技术栈又广又杂、作业节奏快，别裸奔进来——最好先修过 FIT1050（Web 基础）再选会舒服很多。学的时候先把 JavaScript 异步（Promise / async-await）和 Node 基础打牢，再一层层往上叠框架，千万别一开始就贪全套；每周 lab 紧跟别掉队，掉一次很容易滚雪球。撑过这门，你去做 FIT5032 或大型 Web 项目课就有底气了。

#### `FIT2099` — Object Oriented Design and Implementation（面向对象设计与实现）
- **课程简介**：把 Java 编程能力升华为"设计能力"的核心课。它教你用面向对象设计原则去构建高质量软件——先用 UML 迭代地设计中小型系统，评估设计质量，再用 Java 实现，并借助 UML 工具和版本控制系统化地开发和调试。
- **主要知识点**：面向对象设计原则、UML 建模（类图等）、迭代式设计、设计质量评估、Java 实现、系统化调试、软件工程工具（UML 编辑器、版本控制 Git）。
- **整体难度**：⭐⭐⭐⭐☆ — 难在"好设计"没有唯一答案，设计原则（职责分配、可扩展性）的权衡需要经验；把 UML 设计准确落地为代码也考验功力。
- **成绩组成**：Java Bootcamp 10% + Assignment 1 15% + Assignment 2 15% + Assignment 3 20% + 期末考试（2h10m）40%（平时 60% + 期末 40%）。
- **建议学习路线**：选它之前最好先修过 FIT1051 / FIT9131，把 Java 和 OO 基础打牢，不然会挺吃力。它最"磨人"的地方是好设计没有标准答案，别慌——你要练的就是不满足于"能跑"，而是多问一句"这样设计合不合原则、好不好扩展"。三个作业通常层层递进，吃透前一个再做下一个，别急着往前赶。

#### `FIT9136` — Introduction to Python Programming（Python 编程入门）
- **课程简介**：面向研究生的 Python 入门课（2026 handbook 标题为 "Introduction to Python programming"，旧称 "Algorithms and programming foundations in Python"）。它同时教 Python 编程与基础数据结构和算法——从设计、分析到实现，涵盖列表、栈、队列、树、递归以及排序 / 查找算法，是许多 IT / 数据科学硕士的第一门编程课。
- **主要知识点**：Python 语法与程序设计、基本数据类型与数据结构（列表 / 栈 / 队列 / 树）、递归、排序与查找算法、算法复杂度分析、程序测试与文档。
- **整体难度**：⭐⭐⭐☆☆ — 语法友好，但对零基础研究生而言，把编程与"数据结构 + 算法复杂度"打包一起学，后半程（树、递归、复杂度）会明显加速。
- **成绩组成**：Assignment 1 15% + In-semester Test（45 分钟）15% + Assignment 2 20% + 期末考试（2h10m）50%（以当学期 unit guide 为准）。
- **建议学习路线**：作为研究生第一门编程课，Python 语法很友好，零基础也不用怕，只是它把"编程 + 数据结构 + 复杂度"打包一起教，后半程（树、递归、复杂度）会明显提速，你要有心理准备。建议前四周先把 Python 基础和函数练熟打好节奏，中期集中攻数据结构与递归，最后系统过一遍算法复杂度。稳稳修完，你再去碰 FIT5xxx 的编程 / 数据类课就有底了。

### 算法 · 数据结构 · 理论

#### `FIT1008` — Fundamentals of Algorithms（算法基础）
- **课程简介**：Monash CS 学生真正的"算法与数据结构入门课"（2026 起由旧称 *Introduction to Computer Science* 更名重构）。你将学会把一个问题陈述转化为结构良好的计算解决方案：选对数据结构、设计高效算法，并权衡正确性、性能与可维护性。
- **主要知识点**：递归、入门复杂度分析、栈与队列、树、堆、哈希表、算法的理论与实验性能评估、时间 / 空间权衡、程序设计与测试。
- **整体难度**：⭐⭐⭐⭐☆ — 对大一学生而言节奏快、抽象度陡增，递归与复杂度分析是第一道大坎。
- **成绩组成**：2026 年处于改版过渡期，存在两种考核形式——新版（Sem 2, 2026 起）为 **Portfolio 100%**（持续性作品集考核）；旧版（Sem 1, 2026）为 **在学期测验 30% + 项目 / 期末 40% + 其余测验**。以当学期 unit guide 为准。
- **建议学习路线**：这是 FIT2004、FIT3155 的直接先修，也就是说你现在偷的懒后面都要还，所以递归和 Big-O 一定要打扎实。大一节奏突然变快、抽象度陡增很正常，别被它劝退——递归和复杂度是第一道坎，跟上就好了。建议同步修 MAT1830（离散数学）来撑复杂度证明，平时多亲手写数据结构、别只调库函数，这样理解才扎实。

#### `FIT2004` — Algorithms and Data Structures（算法与数据结构）
- **课程简介**：Monash CS 的核心"硬课"之一，系统训练算法设计与分析的科学方法。从问题规格化到算法设计、复杂度分析再到实现，是通往高级算法与技术面试的必经之路。
- **主要知识点**：最好 / 平均 / 最坏情况的时间与空间复杂度分析、递归、高级数据结构（堆、B 树）、哈希、排序算法、搜索算法、图算法、数值计算。
- **整体难度**：⭐⭐⭐⭐☆ — 内容密度大、证明与实现并重，图算法与复杂度分析是主要拉分点。
- **成绩组成**：2026 handbook 显示为 **Portfolio（作品集 / 持续性考核）100%**（含 Quiz / Test 组件，设有阈值 hurdle 门槛）。具体各次作业占比以当学期 unit guide 为准。
- **建议学习路线**：这是公认的硬课，但也是通往高级算法和技术面试的必经之路，值得认真拿下。选之前先修好 FIT1008 / FIT1054，开课前把递归和 Big-O 再过一遍，你会轻松不少。学期里最容易翻车的是图算法（最短路、MST、网络流），务必按周跟进、动手实现，别攒到期末——一堆积就崩。学好它，你就能直接接 FIT3155。

#### `FIT2014` — Theory of Computation（计算理论）
- **课程简介**：一门"烧脑但优雅"的理论课，回答"计算机到底能算什么、不能算什么"。带你走进形式语言、自动机与计算复杂度的世界，并系统训练严格的数学证明能力。
- **主要知识点**：有限状态自动机、正则表达式、文法、下推自动机、可计算函数、图灵机、多项式时间归约、复杂度类 P 与 NP、NP 完全性、形式化证明写作。
- **整体难度**：⭐⭐⭐⭐☆ — 抽象、偏数学，写形式证明对很多同学是最大挑战。
- **成绩组成**：Written 20% + Project 15% + 期末考试（Examination）50% + 其余组件（约 5% + 10%，视 offering 而定）；设有阈值 hurdle 门槛。以当学期 unit guide 为准。
- **建议学习路线**：这门课偏数学、要写形式证明，如果你怕证明，先把 MAT1830（离散数学）巩固好再选会踏实很多。它其实没那么可怕——诀窍是把每周的自动机 / 归约例题自己独立重做一遍，手感就出来了。NP 完全性那块别死记，重点是理解归约怎么构造；考前多练"把证明写清楚"这件事，因为这才是最拉分的地方。

#### `FIT2085` — Fundamentals of Algorithms for Engineers（工程师算法基础）
- **课程简介**：这是 FIT1008 面向工程学院学生的等价变体版本，内容与 FIT1008 高度一致，但结合工程语境教学。学习目标与数据结构 / 算法核心内容相同，供工程专业学生修读。
- **主要知识点**：递归、入门复杂度分析、栈与队列、树、堆、哈希表、算法性能的理论与实验评估、程序设计、实现与测试。
- **整体难度**：⭐⭐⭐⭐☆ — 与 FIT1008 难度相当，对非 CS 背景的工程学生抽象门槛偏高。
- **成绩组成**：同处 2026 改版过渡期——新版为 **Portfolio 100%**；旧版含 **Portfolio 30% + 项目 40% + 测验 30%** 等组件。以当学期 unit guide 为准。
- **建议学习路线**：这门就是工程学院版的 FIT1008，难度差不多，非 CS 背景的你可能觉得抽象门槛偏高，别担心，办法很简单——多写代码、把递归和复杂度真正吃透。最有效的做法是把课堂上讲的每个数据结构都自己从头实现一遍，编程手感一上来，这门课就没那么唬人了。

#### `FIT2102` — Programming Paradigms（编程范式）
- **课程简介**：一门拓宽编程视野的课——就像学习不同语法的自然语言，不同"范式"的编程语言在表达力与效率上迥异。你将深入函数式与声明式编程，理解语言设计原理，学会用更优雅、正确、可维护的方式解决问题。
- **主要知识点**：函数式编程、声明式编程、编程语言设计原理与演化、低级到高级范式对比、语言表达力与效率、范式间的比较与权衡（常用 Haskell / TypeScript 等）。
- **整体难度**：⭐⭐⭐⭐☆ — 思维方式转变（从命令式到函数式）是最大障碍，上手陡但回报高。
- **成绩组成**：Assignment 1（Project）+ Assignment 2（Project）+ Quiz + 课堂练习（Exercise），各组件约 20–30%（合计 100%）；设有两处 45% 门槛（两次作业合计、worksheet 与 quiz 合计）。以当学期 unit guide 为准。
- **建议学习路线**：函数式编程会颠覆你习惯的命令式思维，上手是有点陡，但回报很高，学完你看代码的眼光会不一样，很值得选。选之前先修好 FIT1008 / FIT2004，开课前提前摸一摸函数式语言（高阶函数、递归、纯函数、类型系统），转起来会顺很多。每周的 worksheet 跟着做保持手感，两个大作业尽早动手，别等灵感——早开工就不慌。

#### `FIT3155` — Advanced Data Structures and Algorithms（高级数据结构与算法）
- **课程简介**：FIT2004 的进阶延续，聚焦解决真实世界编程难题所需的高级算法范式。深入研究空间高效的数据结构与时间高效的求解策略，是算法竞赛与高强度技术面试的"利器课"。
- **主要知识点**：摊还分析（amortized analysis）、高级排序与搜索算法、新型树 / 字符串 / 图数据结构与算法、数论算法等。
- **整体难度**：⭐⭐⭐⭐⭐ — Monash 算法方向难度天花板，字符串算法与摊还分析对多数学生极具挑战。
- **成绩组成**：Artefact 1（作业）20% + Artefact 2（作业）20% + 期末考试（Examination）60%；设有阈值门槛（期末 ≥45%、平时 ≥45%、总分 ≥50%）。以当学期 unit guide 为准。
- **建议学习路线**：这是 Monash 算法方向的难度天花板，选它之前一定要先把 FIT2004 学扎实，否则会很痛苦。字符串算法和摊还分析确实劝退不少人，但它们是可以一块块啃下来的——开课前先复习图算法与复杂度，学期中紧跟字符串算法（后缀树 / 数组、Z-algorithm 等）逐个动手实现。期末占比高，别指望考前突击，从头到尾持续复习才稳。

### 计算机系统 · 体系结构

#### `FIT2100` — Operating Systems（操作系统）
- **课程简介**：这门课带你揭开操作系统这层"看不见的管家"的面纱——它如何在硬件之上调度进程、分配内存、协调 I/O 设备，让多个程序看似同时流畅运行。课程强调 hands-on，实验以部分完成的编程练习为基础，需要你读懂系统调用并动手扩展。
- **主要知识点**：进程与线程、处理器调度策略、内存管理、虚拟内存、I/O 设备管理、进程同步（synchronization）、系统调用（system calls）、多道程序设计性能优化。
- **整体难度**：⭐⭐⭐☆☆ — 概念不难但 C 语言系统编程和同步机制（锁 / 信号量）的实验容易踩坑。
- **成绩组成**：期末考试（2h10m）50% + In-semester assessment 50%（含必做的实验 / lab 编程作业；具体细分以当学期 unit guide 为准）。
- **建议学习路线**：操作系统的概念其实不算难，真正让人踩坑的是 C 语言系统编程和同步机制的实验，所以选之前先把 C 指针、内存模型和多线程基础补一补，你会省不少力。实验一拿到就动手跑通再改，别放着；同步那部分（死锁、竞态）容易绕晕，用小例子画时序图就清楚了。考试爱考"各种调度 / 内存策略谁优谁劣"这类对比，复习时自己列一张横向对比表最省事又提分。

#### `FIT3143` — Parallel Computing（并行计算）
- **课程简介**：现代计算机在硬件和软件层面都充满并行性，这门课教你如何"榨干"多核、集群和分布式超算的算力。你会同时接触共享内存与消息传递两大范式，写出真正跑在多处理器上的并行算法，并学会评估它们的性能与加速比。
- **主要知识点**：并行计算体系结构、共享内存与消息传递范式、并发 / 多线程 / 同步性、并行算法设计、性能分析与评估、集群与分布式超算模型、并行编程语言与工具（如 MPI / OpenMP 类）。
- **整体难度**：⭐⭐⭐⭐☆ — 并行 bug（竞态、死锁）难复现难调试，性能分析与算法设计对功底要求高。
- **成绩组成**：期末考试（2h10m）50% + In-semester assessment 50%（具体细分以当学期 unit guide 为准）。
- **建议学习路线**：这门课和 FIT2100（操作系统）衔接很紧，选它之前把并发 / 线程基础补齐，你会顺很多。并行 bug（竞态、死锁）难复现又难调，别硬刚——先用小规模数据把正确性验证好，再上真正的并行。性能分析要抓住 Amdahl 定律这类核心方法，把"设计—实现—测性能"当成一条完整流水线来练；另外报告写作也计分，表达别马虎。

#### `FIT3159` — Computer Architecture（计算机体系结构）
- **课程简介**：这门课深入计算机"内部齿轮"，从布尔逻辑门一路讲到流水线与超标量处理器，让你真正理解一条指令是如何被硬件执行的。内容技术性强，特别适合软件工程和网络安全方向、想打通"软硬件之间那层"的同学。
- **主要知识点**：组合与时序逻辑、布尔代数、计数器 / 加法器、内存与寻址、总线与 DMA、数据表示与机器运算、微程序设计、缓存与缓存架构、虚拟内存与 TLB、中断（向量 / 轮询）、流水线与超标量架构、数据相关与冒险、CISC / RISC / VLIW。
- **整体难度**：⭐⭐⭐⭐☆ — 知识点密集且底层，缓存 / 流水线 / 冒险等概念抽象，实验偏硬件仿真。
- **成绩组成**：期末考试（2h10m）60% + In-semester assessment 40%（含 Laboratory Exercises 约 30%，每次约 5%；具体细分以当学期 unit guide 为准）。
- **建议学习路线**：如果你想打通"软硬件之间那层"，尤其做软工或网安方向，这门课很值得选。知识点底层又密集，别想着一口吃下——跟着"逻辑门 → 运算 → 存储层次 → 流水线"的自底向上主线走，每个概念都动手画图或做仿真，理解会牢很多。缓存命中 / 缺失、流水线冒险与相关是考试重灾区，多做数值计算题就不怕；实验占比高又是每周累积，千万别拖到堆在一起。

#### `FIT9137` — Introduction to Computer Architecture and Networks（计算机体系结构与网络导论）
- **课程简介**：这是面向研究生的基础衔接课（foundation unit），一门课同时覆盖计算机体系结构与计算机网络两大基础板块，由早期的 FIT9134 与 FIT9135 合并而来。它帮助非科班背景的研究生快速补齐"硬件 + 网络"的共同底座，为后续 IT 硕士课程铺路。
- **主要知识点**：计算机硬件与操作系统基础、数据表示、无线网络（物理层与数据链路层）、网络分层模型、局域网 / 骨干网 / 广域网的结构与功能、网络与传输层、网络架构与应用、网络安全基础。
- **整体难度**：⭐⭐⭐☆☆ — 作为导论课概念铺得广但不深，难在"架构 + 网络"两条线内容量大、跨度广。
- **成绩组成**：Lab Assessment Tasks 10%（三次实验经 Moodle quiz 提交）+ Assignment 1 20%（无线网络物理 / 数据链路层 + 案例研究报告）+ Assignment 2 12%（网络与传输层、LAN / 骨干 / WAN、网络安全）+ 期末评估约 58%（以当学期 unit guide 为准）。
- **建议学习路线**：这门是给非科班研究生补底子的导论课，概念铺得广但不深，别被"架构 + 网络"两大块的信息量吓到——把它拆成"体系结构"和"网络"两条线分别推进就清晰多了。网络那条紧扣 OSI / TCP-IP 分层模型，把知识点挂上去串起来最好记。实验和两次 assignment 集中在学期前中段，跟着节奏按周消化就能拿下；报告类作业占比不小，注意技术写作规范。

### 计算机网络

#### `FIT2165` — Computer Networks（计算机网络）
- **课程简介**：这门课带你从零搭建对计算机网络的整体认知——数据是如何从你的一台设备"跳"到地球另一端的另一台设备的。课程以软件与系统为核心视角，覆盖数据通信、网络协议与相关软件接口，并引入网络设计、配置、管理与安全的基本原理。学完后你能看懂 ISO/OSI 与 Internet 分层模型，并动手用 socket 编程实现一个联网的小程序。
- **主要知识点**：网络体系结构标准、ISO 参考模型与 Internet 模型、网络互联（internetworking）与 IP 编址、进程间通信与 socket 接口编程、物理层（有线 / 无线）技术、数据链路层技术、网络层基础（分组交换、排队）、LAN / WAN 设计（ALOHA、CSMA/CD）、网络配置 / 管理与安全基础。
- **整体难度**：⭐⭐⭐☆☆ — 概念分层清晰但面广，难点在于既要记下大量协议 / 标准，又要真正上手写 socket 网络程序把抽象模型落地。
- **成绩组成**：期末考试（2h）60% + 平时（in-semester，含小测 / quiz / assignment）40%（2026 handbook 页面为动态渲染，各项拆分未能逐条核实，**以当学期 unit guide 为准**；历史同名单元通常为 期末 60% + 期中测 10% + Quiz 10% + Assignment 20%）。
- **建议学习路线**：这门课分层清晰但面广，别急着死背零散协议——先用 OSI / Internet 分层模型搭一个"自上而下"的骨架，把每层的职责和代表协议串成一张图，后面填知识点就轻松了。socket 编程别拖，尽早动手写 TCP / UDP 的客户端-服务器小练习，把网络层和传输层真正跑通你才有实感。IP 编址和子网划分靠多刷计算题练到形成肌肉记忆，考试就不慌了。

### 数据库 · 信息系统

#### `FIT1006` — Business Information Analysis（商业信息分析）
- **课程简介**：这门课其实是一门"商科统计入门"，把统计与定量方法放进商业与经济的语境里讲。你会学会怎么用图表呈现商业数据、读懂数据背后的规律，并用概率、抽样、假设检验、回归和预测等工具为商业决策提供依据。它是后续更高阶统计与数据分析课程的地基。
- **主要知识点**：描述性统计（集中趋势与离散程度）、频数分布、概率原理、概率分布、抽样理论、区间估计、假设检验、回归分析、指数（index numbers）、预测方法。
- **整体难度**：⭐⭐⭐☆☆ — 概念不深但计算细节多，公式套用与统计解读容易失分。
- **成绩组成**：期末考试（Final Examination）50% + Assignment 1 18% + Assignment 2 30% + Online quiz 2%。
- **建议学习路线**：这本质上是门商科统计入门，概念不深，就是计算细节多、容易在套公式和解读上丢分。诀窍是先把描述统计和概率分布的基本公式吃透，做题时养成"先判断该用哪种分布 / 检验"的习惯，思路对了就不容易错。两个 assignment 合起来占 48%，务必对着 rubric 逐条打钩，而且别只写数字——把统计结果翻译成商业含义才是拿分关键。

#### `FIT2094 / FIT9132` — Databases / Introduction to Databases（数据库）
- **课程简介**：这是 Monash 数据库入门的"孪生课"——**FIT2094 面向本科生**、**FIT9132 面向研究生**（Introduction to Databases），内容主线一致：从关系模型理论出发，教你做数据建模、设计并用 SQL 在企业级数据库上实现。FIT2094 明确以 Oracle 企业级系统实操为主，涵盖建表、填充、查询、更新与完整性约束；FIT9132 更侧重把关系模型的理论基础、分析设计与 SQL 实现完整走一遍。两者难度相近，选课由学位层次决定。
- **主要知识点**：关系模型理论、ER / 概念建模、逻辑设计与规范化、SQL（DDL / DML）、数据完整性约束、数据填充与查询 / 更新、（FIT2094）Oracle 企业级实现与数据管理。
- **整体难度**：⭐⭐⭐☆☆ — 概念清晰但规范化与复杂 SQL 联表查询是主要坎，实操细节容易翻车。
- **成绩组成**：
  - FIT2094：Assignment 1 35% + Assignment 2 35% + In-Class test 1 15% + In-Class test 2 15%。
  - FIT9132：Assignment 1（Database Design）35% + Assignment 2（Creating, Populating and Manipulating Databases）35% + Class test 1 15% + Class test 2 15%。
- **建议学习路线**：数据库概念清晰、好上手，真正会卡你的是规范化和复杂 SQL 联表查询，实操细节一疏忽就翻车。别慌，练法很明确：先把 ER 图和规范化（到 3NF / BCNF）练到能徒手推，再大量刷 SQL，直到多表连接、子查询、聚合都成肌肉记忆。两个 assignment 合起来占 70%，从设计到实现要保持模型一致，提交前一定用真实数据把所有约束跑通再交。

#### `FIT3176` — Advanced Database Design（高级数据库设计）
- **课程简介**：当关系型数据库不够用时，这门课带你进入 NoSQL 与非关系型世界。你会动手玩 MongoDB（文档型）、Cassandra（列式）和 Neo4j（图数据库），学习它们的设计思路、查询方式，以及和传统关系型模型的取舍对比。是面向大数据 / 现代应用后端的进阶课。
- **主要知识点**：文档型 / 列式 / 图数据库设计、NoSQL 概念、MongoDB、Apache Cassandra、Neo4j 与图查询、非关系型事务处理、关系型与非关系型模型对比。
- **整体难度**：⭐⭐⭐⭐☆ — 需同时掌握三套异构系统的模型与查询语法，实操工具链多、上手成本高。
- **成绩组成**：Assignment - MongoDB 30% + Assignment - Neo4j and Cassandra 30% + Mid-semester Test 20% + Final Test 20%。
- **建议学习路线**：想做大数据 / 现代后端方向的话这门很值得选，只是它一次要你上手三套异构系统，工具链多、上手成本高，选之前先修好 FIT2094 / FIT3171 会稳很多。学的时候先建立"按数据形态选数据库"的判断力（文档 / 列 / 图各自适合什么场景），再逐个把 MongoDB、Cassandra、Neo4j 的建模和查询语法练熟。两个实操 assignment 占 60%，一定尽早把本地环境搭好，别临期才发现装不上而踩坑。

#### `FIT9123` — Fundamentals of Business Information Systems（商业信息系统基础）
- **课程简介**：这是一门研究生信息系统的"通识入门"，帮你建立对信息技术及其运行、创建与管理语境的整体认识——技术为何存在、由谁管理、服务于什么商业目标。偏概念与思辨，写作与反思占比很重。
- **主要知识点**：信息系统与信息技术基础、技术运行与管理语境、IT 在组织中的目的与目标、技术的创建与治理、商业情境下的批判性反思。
- **整体难度**：⭐⭐☆☆☆ — 无编程门槛，难在写作质量与批判性反思深度，而非技术。
- **成绩组成**：Assignment 2（Group：presentation + report + individual reflection）60% + Assignment 1（Individual：prompts and reflections）30% + Applied-class assessed activity 10%。
- **建议学习路线**：这门没有编程门槛，偏概念和思辨，但别以为轻松——难点全在写作质量和反思深度上。把重心放在把观点结构化地写清楚，多拿真实企业案例来支撑会更有说服力。占 60% 的小组作业要尽早分工、统一一条叙事逻辑；个人反思那部分自己单独打磨好，别被小组的进度拖累。

#### `FIT9138` — Information Systems Analysis, Design and Systems Thinking（信息系统分析、设计与系统思维）
- **课程简介**：这门课教你像设计师一样思考信息系统——以人为本的设计（human-centred design）、设计思维流程，以及"系统思维"这套理解各部分如何相互关联、系统如何随时间演化的方法论。课程强调动手实践，你会真正设计一套信息系统。
- **主要知识点**：以人为本的信息系统设计、设计思维流程、系统思维、需求分析、系统建模与设计、系统随时间的动态演化。
- **整体难度**：⭐⭐⭐☆☆ — 概念框架多、偏方法论，难在把抽象的设计 / 系统思维落到具体产物上。
- **成绩组成**：Group Report with walkthrough 40% + In-Class Quizzes 20% + Group Presentation 20% + Individual Assignment 20%。
- **建议学习路线**：这门偏方法论、概念框架多，最容易卡你的是"怎么把抽象的设计 / 系统思维落到具体产物上"。别硬记概念——先抓住设计思维和系统思维两条主线，用一个贯穿始终的案例把分析 → 设计 → 建模完整走一遍，你就有实感了。小组报告加演示合计 60%，一定让团队对同一个系统的理解保持一致；随堂 quiz 覆盖概念，每周跟着读材料就不至于临时抱佛脚。

### 人工智能 · 机器学习

#### `FIT1059` — AI for Everyone（人人都懂人工智能）
- **课程简介**：这是一门面向全校各专业的入门通识课，无需任何编程或技术背景。它用生活化的方式讲清"AI 到底是什么、能做什么、不能做什么"，帮助你看懂正在重塑世界的这项技术，并思考它带来的伦理与社会影响。适合想入门但又怕数学 / 代码的同学。
- **主要知识点**：AI 基本概念与发展史、机器学习直觉理解、生成式 AI（如大语言模型）、AI 的实际应用场景、AI 伦理与社会影响、负责任地使用 AI。
- **整体难度**：⭐☆☆☆☆ — 概念性通识课，几乎无数学与编程门槛，难点仅在于把抽象概念说清楚、写好反思性作业。
- **成绩组成**：2026 handbook 未公开精确百分比；作为入门通识 / Enrich 型 unit，通常以平时作业、测验与反思报告为主、无重型考试（**以当学期 unit guide 为准**）。
- **建议学习路线**：怕数学、怕代码但又想入门 AI 的话，这门通识课就是为你准备的，几乎零门槛，选了不用担心。它唯一需要你花心思的是"用自己的话把概念讲清楚"和写好反思作业。平时多结合新闻里真实的 AI 事件来写反思，再跟上每周小测保持节奏，轻松就能过。

#### `FIT3080` — Artificial Intelligence（人工智能）
- **课程简介**：本科阶段的经典 AI 主干课，系统讲授"符号主义 AI"的核心方法。你会从智能体（agent）出发，学会用搜索、逻辑推理、概率推理和机器学习让机器"做出理性决策"，覆盖从棋类博弈到贝叶斯网络的经典技术。
- **主要知识点**：AI 发展史与智能体、问题求解与搜索（启发式搜索、迭代改进、博弈搜索）、知识表示与推理（命题 / 一阶逻辑、规划、语义网络）、不确定性推理（信念 / 贝叶斯网络）、机器学习（决策树、朴素贝叶斯、神经网络、遗传算法）、语言技术。
- **整体难度**：⭐⭐⭐⭐☆ — 内容面广，搜索算法与逻辑推理需要较强的算法与数学基础，3h10m 大考占比高，需大量刷题。
- **成绩组成**：期末考试（3h10m）60% + 平时 40%（Assignment 1 搜索求解 14% + Assignment 2 智能体决策 24% + Quizzes 2%）。
- **建议学习路线**：这是本科经典 AI 主干课，内容面广、需要一定算法和数学底子，3h10m 的大考还占 60%，选之前有点心理准备。别被吓住——高频考点其实很集中，先把搜索（A*、minimax、alpha-beta）和贝叶斯网络这两块吃透，你就稳了一大半。两个 assignment 是拉分关键，一定动手把算法实现出来，别只背概念；期末按 lecture 主题系统整理笔记，配上历年题多刷就行。

#### `FIT5047` — Fundamentals of Artificial Intelligence（人工智能基础）
- **课程简介**：研究生版 AI 基础课（Master of AI 核心），内容与 FIT3080 思路相近但面向硕士生，节奏更快、深度更高。它带你搭建对"智能软件系统"的完整认知：搜索、知识表示、规划、不确定性推理、机器学习与进化算法一网打尽。
- **主要知识点**：自动搜索方法、知识表示与推理、规划、不确定性推理（贝叶斯推断）、监督与无监督机器学习、遗传 / 进化算法，以及自然语言处理、用户建模、软件智能体、推荐系统等应用。
- **整体难度**：⭐⭐⭐⭐☆ — 覆盖面广且默认硕士生能快速上手数学（概率、逻辑），考试占比大，短时间内消化众多范式是主要挑战。
- **成绩组成**：期末考试（2h10m）60% + 平时 40%（Task 1 = 10 次 quiz + 2 次作业共 20%；Task 2 = 贝叶斯网络与机器学习作业各 10%，共 20%）。
- **建议学习路线**：这是研究生版 AI 基础课，默认你能快速上手概率和逻辑，节奏比本科快、考试占比也大，选之前掂量一下自己的数学底子。覆盖面广听着唬人，但拆开看就好办了：贝叶斯网络和机器学习的实验是评分核心，一定配合 Python 工具亲手做；每周 quiz 就用来逼自己跟上进度。考前按"搜索 / 逻辑 / 概率 / 学习"四大板块分模块复习，一块块过就不乱。

#### `FIT5201` — Machine Learning（机器学习）
- **课程简介**：Master of AI / Data Science 的机器学习主力课，重理论与统计学习基础。它不满足于"调包"，而是带你理解模型背后的数学：为什么会过拟合、如何做模型选择、生成式与判别式模型的区别，让你成为真正理解 ML 的人。
- **主要知识点**：统计学习理论（偏差-方差、模型选择、模型复杂度）、回归与分类的线性模型（线性基函数、逻辑回归、贝叶斯分类器、广义线性模型）、判别式与生成式模型、K-means 与隐变量模型（GMM、EM）、神经网络与深度学习入门、大数据下的算法扩展。
- **整体难度**：⭐⭐⭐⭐⭐ — 全课最吃数学：线性代数、概率统计、微积分缺一不可，公式推导密集，是 AI / ML 方向公认的硬课。
- **成绩组成**（On-Campus）：期末考试（2h10m）50% + Assignment 1 25% + Assignment 2 16% + Quiz 9%（Monash Online 模式为 100% 平时、无考试——**以当学期 unit guide 为准**）。
- **建议学习路线**：这是 AI / ML 方向公认最吃数学的硬课，线代、概率、微积分缺一不可，公式推导密集，选之前一定要对自己的数学底子有数——底子弱的话强烈建议开学前先补齐概率和线性代数，会救你一命。别指望躲开推导：边学边亲手推关键公式（偏差-方差、EM、逻辑回归梯度）才是真懂。两个 assignment 既写代码又写数学推导，尽早启动、留足调试时间，别拖到最后。

#### `FIT5215` — Deep Learning（深度学习）
- **课程简介**：面向研究生的深度学习实战课，教你从零设计并训练现代神经网络。从全连接网到 CNN、RNN，再到表示学习与嵌入方法，最终能落地到图像识别、文本聚类等真实任务。理论 + 编程并重。
- **主要知识点**：机器学习系统设计、深度神经网络、卷积神经网络（CNN）、循环神经网络（RNN）、各类优化训练策略、无监督特征学习与表示学习、嵌入（embedding）方法、时序数据建模。
- **整体难度**：⭐⭐⭐⭐☆ — 数学（梯度、反向传播、优化）与深度学习框架编程双重要求，作业训练模型耗时耗算力，是硬核实战课。
- **成绩组成**（学期制）：期末考试（2h）40% + Assignment 1 20% + Assignment 2 20% + In-semester test 1 10% + In-semester test 2 10%（Term 3 集中授课模式权重略有不同，**以当学期 unit guide 为准**）。
- **建议学习路线**：这是门硬核实战课，既要数学（梯度、反向传播、优化）又要会写深度学习框架，作业还得真训练模型、挺耗时耗算力，选之前先把 Python + PyTorch / TensorFlow 和 numpy 向量化练熟会轻松很多。作业要训练 CNN / RNN，务必提前把环境跑通、留足调参时间，别等 deadline 才发现环境报错。两次期中测验紧扣理论，随堂就把反向传播和优化器原理巩固好，考试就不慌。

#### `FIT5217` — Natural Language Processing（自然语言处理）
- **课程简介**：研究生 NLP 入门课，带你理解"如何让机器读懂人类语言"。从词、句、篇章的分析技术，到信息抽取、问答系统等实际应用，是进入 NLP / 大模型领域的重要基础课。
- **主要知识点**：NLP 核心问题与应用体系、词 / 句 / 篇章多层次文本分析、信息抽取、问答系统、NLP 系统设计与评估、各类 NLP 方法的比较分析。
- **整体难度**：⭐⭐⭐⭐☆ — 需要概率、机器学习 / 深度学习基础，考试占比高（60%），编程作业与理论并重，对 ML 底子弱的同学有挑战。
- **成绩组成**：期末考试（2h）60% + Assignment 1 20% + Quizzes 20%。
- **建议学习路线**：想进 NLP / 大模型领域的话这门是重要基础，很值得选，但它需要概率和 ML / 深度学习底子，ML 底子弱的同学会有点吃力——最好先修或并修 ML / 深度学习课，把词向量、序列模型这些补上再进来。作业偏编程实现，动手复现几个经典模型你就通了。期末占 60%，平时就把每个 NLP 任务的方法和评估指标系统整理成表，考前会省很多力。

#### `FIT5226` — Multi-Agent Systems and Collective Behaviour（多智能体系统与群体行为）
- **课程简介**：Master of AI 的进阶核心课，聚焦"多个自主智能体如何交互与协作"。前段深入强化学习与 Deep Q-Learning，后段转向博弈论、群体动力学与集体行为，从蚁群、鱼群到蜂群机器人，兼具趣味与硬核。
- **主要知识点**：强化学习与 Deep Q-Learning、多智能体系统建模与设计、博弈论（种群博弈、重复博弈、联盟博弈）、社会选择与群体动力学、集体行为分析、群体机器人与信息物理系统、科学建模应用。
- **整体难度**：⭐⭐⭐⭐☆ — 强化学习本身概念抽象，学期项目需从单智能体表格 Q-learning 一路搭到多智能体 Deep Q-learning 并结合博弈论分析，最后阶段综合性极强。
- **成绩组成**：期末考试（2h10m）40% + 平时（in-semester，含贯穿整学期的仿真项目）60%。
- **建议学习路线**：这门课题材很有意思（蚁群、鱼群、蜂群机器人），但强化学习本身抽象、后段综合性又强，别小看它。诀窍是先把强化学习基础（MDP、Q-learning、DQN）和 Python 仿真能力打牢，你上手就不慌。贯穿整学期的核心项目是分阶段推进的，每个阶段务必按时完成，千万别把最后的综合任务攒到一起。博弈论那块从 week 5 之后开始，跟着 lecture 一块块吃透就好。

### 数据科学 · 数据分析

#### `FIT1043` — Introduction to Data Science（数据科学导论）
- **课程简介**：这是数据科学专业的入门第一课。它不急着教你写复杂算法，而是带你俯瞰整个数据科学的"生态版图"——数据从哪来、如何存储清洗、有哪些分析方法、数据科学家在团队里扮演什么角色。用大量真实案例让你先看懂"数据能干什么"，再谈怎么干。
- **主要知识点**：数据采集与准备、数据清洗与流处理、数据存储与管理、数据科学项目角色分工、常见分析与统计方法概览、可用工具与资源、数据的政策 / 法律 / 伦理问题。
- **整体难度**：⭐⭐☆☆☆ — 概念广但不深，难点在于第一次接触命令行 / 脚本工具（如 Python、Bash、SQL）时的上手门槛。
- **成绩组成**：Assignment 1 10% + Assignment 2 20% + Assignment 3 20% + 期末考试（2h10m）50%（以当学期 unit guide 为准）。
- **建议学习路线**：作为数据科学第一课，它概念广但不深，很适合入门，唯一的门槛是第一次接触命令行 / 脚本工具（Python、Bash、SQL）时会有点手生，别怕，多敲几次就熟了。把三次 assignment 当作主线练手，每次都亲手跑一遍完整的"取数—清洗—分析—可视化"小流程，实感就有了。概念多而杂，边学边整理一份术语表，能帮你为后面的 FIT2086、FIT3152 打好底。

#### `FIT2086` — Modelling for Data Analysis（数据分析建模）
- **课程简介**：这是整个专业里"统计味"最重的一门，用 R 系统讲清数据分析背后的数学地基。从概率分布、假设检验，到回归、贝叶斯分类、最大似然估计与交叉验证，帮你从"会调库"升级到"懂原理"。
- **主要知识点**：数据采集与抽样、数据质量、统计假设检验、探索性与验证性分析、概率分布（多元高斯 / 泊松 / 狄利克雷）、随机数生成与模拟、Bootstrap、线性与逻辑回归、贝叶斯分类、参数与函数估计、最大似然 / 最小成本估计、蒙特卡洛估计、偏差-方差权衡、交叉验证、模型性能评估。
- **整体难度**：⭐⭐⭐⭐☆ — 数学与统计推导密集，对概率论和线性代数基础要求较高，是本专业公认的硬骨头。
- **成绩组成**：Assignment 1 10% + Assignment 2 20% + Assignment 3 20% + 期末考试（2h10m）50%（以当学期 unit guide 为准）。
- **建议学习路线**：这是本专业公认"统计味最重"的硬骨头，对概率论和线性代数要求较高，选之前先掂量下自己的数学底子——底子一般的话先把概率分布和回归的基本功补齐，会救你不少。别只想着"会调库"：逐周用 R 把课件里的每个模型亲手复现一遍，你才真正懂原理。考试占比高又偏推导，平时就系统整理好公式和假设条件，多做历年 assignment 类型题，考前会踏实很多。

#### `FIT2179` — Data Visualisation（数据可视化）
- **课程简介**：本科阶段的数据可视化专门课（数据科学方向 Year 2 Sem 1 核心单元）。它教你如何用视觉手段"讲好数据的故事"，从图形语法原理到亲手做出有说服力的静态与交互式可视化作品。
- **主要知识点**：可视化设计原则、视觉编码与图形语法、定性 / 定量 / 时间 / 空间数据的可视化、交互式可视化、可视化的批判性评估、（本科方向常用 Python / Altair 等声明式可视化工具）。
- **整体难度**：⭐⭐⭐☆☆ — 概念上手不难，但要做出"既准确又美观"的作品需要审美与打磨，作业投入时间偏多。
- **成绩组成**：未能核实精确百分比（2026 handbook 该单元 Assessment 明细未公开）；此类可视化单元通常为平时作业 / 项目 + 期末，**以当学期 unit guide 为准**。
- **建议学习路线**：概念上手不难，但想做出"既准确又美观"的作品需要审美和反复打磨，作业投入的时间会比你预期多一些，选之前留够时间。学的时候把每个可视化项目都当作作品集来经营，动手前先想清"我要回答什么问题"再选图表类型，就不会做偏。多研究优秀的 D3 / Altair 案例并模仿重做，设计评审环节的反馈别忽略——那是让你作品变好看的捷径。

#### `FIT3152` — Data Analytics（数据分析）
- **课程简介**：本科高阶数据分析实战课，聚焦"大数据时代如何把现实问题变成可解的分析问题"。用 R 覆盖从数据清洗、统计与图形分析到机器学习 / 数据挖掘的完整链路，案例涵盖健康信息、网络流量、欺诈检测等。
- **主要知识点**：数据探索与可视化、统计分析、机器学习与数据挖掘、数据清洗与准备、大数据管理、欺诈检测与模式识别、风险评估与客户行为分析、结果验证与沟通。
- **整体难度**：⭐⭐⭐⭐☆ — 内容广且期末考占比高（60%），需同时具备编程、统计和机器学习综合能力。
- **成绩组成**：Assignment 1 20% + Assignment 2 20% + 期末考试（2h10m）60%（以当学期 unit guide 为准）。
- **建议学习路线**：这是本科高阶实战课，内容广、期末又占 60%，需要你同时具备编程、统计和机器学习能力，选之前最好这几块都有点底子。别被"综合"两个字唬住——把 R 当主力，逐个把决策树、聚类、关联规则等经典模型跑通就上手了。期末权重大，平时就要把每个算法的适用场景、参数含义和结果解读真正吃透，别只停留在会调包，这样考试才顶得住。

#### `FIT5145` — Foundations of Data Science（数据科学基础）
- **课程简介**：研究生版的"数据科学导论"，是 FIT1043 在硕士层面的对应课。以流程、案例和轻量工具带你理解数据科学在组织与商业中的全貌，并用 Python / Jupyter 做实操练习。
- **主要知识点**：数据在组织中的角色、数据管护与生命周期管理、探索性数据分析与可视化、大数据管理与处理、预测建模概览、数据存储与处理需求评估、商业案例分析、Python + Jupyter 实操。
- **整体难度**：⭐⭐⭐☆☆ — 概念广度大、编程要求中等，对无编程背景的转专业硕士生是主要挑战。
- **成绩组成**（On-Campus）：Data Science Exercises I 5% + Business Case Study Plan 5% + Data Science Exercises II 20% + Business Case Study Report & Presentation 10% + 期末考试 60%（Monash Online 版权重不同；以当学期 unit guide 为准）。
- **建议学习路线**：这是研究生版的"数据科学导论"，概念铺得广、编程要求中等，转专业、没编程背景的你会觉得这是最大的坎，别担心——尽早把 Python 和 Jupyter 基础补齐，把每次练习题当成编程热身，慢慢就跟上了。商业案例那部分重点是"用数据讲好一个商业故事"，多练报告写作和口头 / 视频展示，这门课就拿得稳。

#### `FIT5147` — Data Exploration and Visualisation（数据探索与可视化）
- **课程简介**：研究生数据可视化核心课，把"探索性数据分析"和"可视化叙事"结合起来。教你用统计与可视化手段探索数据、评估可视化优劣，并用 R、Python、Tableau、D3 做出交互式作品。
- **主要知识点**：探索性数据分析、可视化在数据科学中的作用与局限、定性 / 定量 / 时间 / 空间数据可视化、有效可视化设计、交互式可视化、可视化的批判性评估、多工具实操（R / Python / Tableau / D3）。
- **整体难度**：⭐⭐⭐☆☆ — 无期末考、全平时，难在两个大项目工作量大且要求工具面广。
- **成绩组成**（On-Campus，全平时）：Programming Exercise 1 (Tableau Public) 5% + Programming Exercise 2 (R) 5% + Programming Exercise 3 (D3) 5% + Data Exploration Project 35% + Visualisation Project 40% + Online Quiz 10%（以当学期 unit guide 为准）。
- **建议学习路线**：这门没有期末考、全靠平时，听着轻松，其实压力在两个工作量很大、工具面又广的大项目上，选之前要有心理准备。三个小编程练习是你熟悉 Tableau / R / D3 的踏板，务必按时做完。两个大项目合计 75%，尽早选一个有数据支撑的选题，把探索项目和可视化项目连贯地规划成一条线；D3 交互那部分最耗时，一定提前预留充足时间，别拖到最后赶。

#### `FIT5149` — Applied Data Analysis（应用数据分析）
- **课程简介**：面向数据科学家 / 业务分析师角色的应用型建模课。系统训练回归、分类、聚类等机器学习方法，重点不在推导而在"如何理解问题、选对模型、正确解读结果"。以 R 为主、Python 为辅。
- **主要知识点**：回归分析、分类算法、聚类方法、统计分析、机器学习基础、模型选择、结果解读与评估、结果沟通。
- **整体难度**：⭐⭐⭐⭐☆ — 需要扎实统计 / 机器学习基础（通常以 FIT5197 为前置），Data Analysis Challenge 项目挑战性强。
- **成绩组成**（On-Campus）：Mining Knowledge from Data（个人）15% + Data Analysis Challenge（小组）35% + 期末考试（2h10m）50%（Monash Online 版为 100% 平时；以当学期 unit guide 为准）。
- **建议学习路线**：这门偏应用，需要扎实的统计 / 机器学习基础，通常以 FIT5197 为前置，选之前先把它修了会顺很多。重点不在推导，而在"理解问题、选对模型、把结果讲清楚"，所以先把回归 / 分类 / 聚类各自的适用条件和评估指标彻底搞清。占 35% 的小组 Data Analysis Challenge 有点像 Kaggle 竞赛、挑战性强，尽早分工、搭好一条完整的建模流水线，别小看特征工程和结果解释——分差往往就在这里。

#### `FIT5196` — Data Wrangling（数据整理）
- **课程简介**：专攻"脏数据变可用数据"的实战课。针对真实数据中的缺失、错误、格式混乱等问题，系统训练解析、清洗、集成与预处理技能，全程用 Python 3 + Pandas + Jupyter。
- **主要知识点**：多格式数据解析、数据质量评估与修复、缺失 / 异常值处理、数据集成与丰富化、特征选择、文本挖掘、网络数据分析、整理过程文档化。
- **整体难度**：⭐⭐⭐☆☆ — 概念不深但对 Python / Pandas 熟练度和细致程度要求高，作业容易在细节（编码、格式、边界情况）上丢分。
- **成绩组成**：Assessment 1（解析原始数据与文本预处理：Part 1 20% + Part 2 15%）35% + Assessment 2（数据清洗与集成）35% + End-of-Term Quiz 30%（以当学期 unit guide 为准）。
- **建议学习路线**：这门概念不深，但对 Python / Pandas 的熟练度和细致程度要求很高，作业特别容易在细节（编码、格式、边界情况）上悄悄丢分，你要有耐心。先把 Pandas 的索引、分组、正则和文本处理练熟，上手就轻松。两个 assignment 都要求可复现、文档清晰，养成写清注释和处理逻辑的习惯，并对边界与异常数据做稳健处理，你的分数就稳了。

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

> 「整体难度 / 建议学习路线」为主观经验参考；部分课程 2026 年处于考核改版过渡期，正式选课与评估请以对应学期的官方 unit guide 为准。

---

## 需要按这所学校定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
