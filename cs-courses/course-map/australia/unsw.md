---
title: 新南威尔士大学（UNSW Sydney）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 2
permalink: /cs-courses/course-map/australia/unsw/
published_at: "2026-07-05 17:18:05"
---

# 新南威尔士大学（UNSW Sydney）

UNSW CS 采用 **COMP** 课程编码、每年 3 个 term（T1/T2/T3）快节奏授课。下方先给出**核心 / 高频课程详解**，再附**完整课程清单**（均**按课程类型归类**，本科与研究生课程合并）。

> 说明：每门课的 **课程简介 · 主要知识点** 依据 UNSW **2026 官方 handbook / 课程 outline** 整理；**整体难度 · 建议学习路线** 为 **辅导视角**（主观参考，因人而异）。来源见页面底部。

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### `COMP1511` — Programming Fundamentals（编程入门）
- **课程简介**：面向零基础的编程入门课，用 **C 语言**教授程序设计基础，训练把现实问题转化为程序解法的能力，并初步理解计算机如何执行指令。
- **主要知识点**：C 语言语法与编程基础、问题分解与算法思维、数组与链表等基础数据结构、指针与内存、调试技巧、计算机体系结构入门。
- **整体难度**（辅导视角）：⭐⭐☆☆☆ — 概念不深，但节奏快、作业密集；**指针 / 链表**是第一个坎。
- **建议学习路线**（辅导视角）：跟紧每周 lab + 小作业，尽早养成"写小程序→调试"的手感；用画内存图的方式理解指针与链表。它是 COMP2521 的地基。

#### `COMP1531` — Software Engineering Fundamentals（软件工程基础）
- **课程简介**：软件工程入门，介绍需求、软件设计基础、版本管理（git）、团队协作与项目实践（常用 Python + 敏捷）。
- **主要知识点**：git 版本控制、软件设计基础、需求与规格、测试、团队协作 / 敏捷、REST/接口入门。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 内容不难，但**团队项目**占比高，协作与工程规范是难点。
- **建议学习路线**（辅导视角）：先练熟 git 工作流；把"需求→设计→测试"跑通一个小项目；它是 COMP2511 的先修。

#### `COMP2511` — Object-Oriented Design & Programming（面向对象设计与编程）
- **课程简介**：面向对象设计与编程的理论与实践，强调运用**软件设计原则与设计模式**构建灵活、可复用、可维护的系统；含 Java OOP、design by contract、UI 设计，并以结对 + 敏捷完成一个大型项目。
- **主要知识点**：OO 设计原则（SOLID）、常用设计模式、design by contract、Java 面向对象编程、UI 设计入门、敏捷实践。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — 概念不难，但"设计品味"需要练；**大项目**占比高。
- **建议学习路线**（辅导视角）：先打牢 SOLID，再逐个吃透常用模式（策略 / 工厂 / 观察者 / 组合 …）并在项目中落地；先修 COMP1531。

### 算法 · 数据结构 · 理论

#### `COMP2521` — Data Structures and Algorithms（数据结构与算法）
- **课程简介**：深化对数据结构与算法的理解及其在软件系统设计中的有效运用；覆盖递归、排序、图论等核心主题，用 **C** 实现，为进阶计算课程打基础。
- **主要知识点**：抽象数据类型（ADT）、递归、排序算法、树、**图与图算法**、复杂度分析、用 C 维护上千行代码的工程能力。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — UNSW CS 的核心分水岭课，概念 + 工程双重要求。
- **建议学习路线**（辅导视角）：吃透每种结构的"接口→实现→复杂度"；**图算法（BFS/DFS/最短路/MST）** 是重点与高频考点；坚持手写实现而非套模板。

### 数据库 · 信息系统

#### `COMP3311` — Database Systems（数据库系统）
- **课程简介**：深入数据库应用开发实践与关系型数据库（RDBMS）背后的理论，概览 DBMS 实现技术与数据库系统发展；实践使用 **PostgreSQL**。
- **主要知识点**：ER 建模、关系模型、**SQL**、数据库应用开发、RDBMS 内部原理与管理、范式与规范化。
- **整体难度**（辅导视角）：⭐⭐⭐☆☆ — SQL 上手快，但 **ER 设计 + 范式 + 应用开发**作业有量。
- **建议学习路线**（辅导视角）：SQL 多写多练（聚合 / 连接 / 子查询）；"ER→关系模式→范式"是设计主线；用 PostgreSQL 做小项目巩固。

### 计算机网络

#### `COMP3331` — Computer Networks and Applications（计算机网络与应用）
- **课程简介**：面向 CS / EE 背景的计算机网络入门，聚焦当代数据通信中常见的范式与协议，概览互联网架构并引入**网络编程**。
- **主要知识点**：互联网架构、介质访问 / 拥塞控制 / 流量控制 / 可靠传输、寻址与路由、**Ethernet / IP / TCP / UDP / HTTP**、网络安全威胁与防御、CDN / P2P / 无线专题；用 C / Java / Python 实现协议与应用并评估性能。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — 概念多、协议细节多，**socket 编程大作业**有挑战。
- **建议学习路线**（辅导视角）：以 TCP/IP 分层为骨架把协议挂上去；重点吃透 **TCP 可靠传输与拥塞控制**；尽早动手 socket 编程作业。

### 人工智能 · 机器学习

#### `COMP9417` — Machine Learning and Data Mining（机器学习与数据挖掘）
- **课程简介**：机器学习作为"从数据中学习"的算法方法，及数据挖掘（把 ML 工具用于从数据中获取洞见）的核心内容。
- **主要知识点**：监督 / 无监督学习、回归与分类、模型评估与泛化、常见 ML 算法、数据挖掘方法。
- **整体难度**（辅导视角）：⭐⭐⭐⭐☆ — **数学（线代 / 概率 / 优化）要求较高**，作业偏理论 + 实现。
- **建议学习路线**（辅导视角）：先补线代 / 概率 / 梯度基础；按"任务→模型→损失→优化→评估"框架串联算法；每个算法先手推再调库。

> 更多核心课（如 `COMP9024`、`COMP9444` 深度学习、`COMP9517` 计算机视觉、`COMP3141` …）将按同样标准补充。想优先哪几门？→ [联系我](/contact/)。

---

## 完整课程清单（按类型）

**编程 · 软件工程 · 项目**

- `COMP1010` — The Art of Computing
- `COMP1511 / COMP1911` — Programming Fundamentals
- `COMP1531` — Software Engineering Fundamentals
- `COMP2041 / COMP9044` — Software Construction
- `COMP2511` — The Art of Software Design (OO Design & Programming)
- `COMP3141` — Software System Design and Implementation
- `COMP6080` — Web Front-end Programming
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

- `COMP9334` — Capacity Planning of Computer Systems and Networks

**计算机网络**

- `COMP3331 / COMP9331` — Computer Networks and Applications

**数据库 · 信息系统**

- `COMP3311` — Database Systems
- `COMP6714` — Information Retrieval and Web Search
- `COMP9311` — Database Systems
- `COMP9315` — Database Systems Implementation
- `COMP9321` — Data Services Engineering

**人工智能 · 机器学习**

- `COMP3411 / COMP9814` — Artificial Intelligence
- `COMP3431 / COMP9434` — Robot Software Architectures
- `COMP4418` — Knowledge Representation and Reasoning
- `COMP6713` — Natural Language Processing
- `COMP9414` — Artificial Intelligence
- `COMP9417` — Machine Learning and Data Mining
- `COMP9418` — Advanced Topics in Statistical Machine Learning
- `COMP9444` — Neural Networks and Deep Learning
- `COMP9491` — Applied AI
- `COMP9517` — Computer Vision

**数据科学 · 数据分析**

- `INFS2608` — Database Management and Big Data Infrastructures
- `COMP9312` — Data Analytics for Graphs
- `COMP9313` — Big Data Management

**网络安全**

- `COMP6843` — Extended Web Application Security and Testing

---

## 资料来源（官方，2026）

- UNSW Handbook 2026：[COMP1511](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP1511)、[COMP2521](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP2521)、[COMP2511](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP2511)、[COMP3311](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP3311)、[COMP3331](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP3331)、[COMP9417](https://www.handbook.unsw.edu.au/undergraduate/courses/2026/COMP9417)
- UNSW CSE 课程 outline（webcms3 / cgi.cse.unsw.edu.au，按 term 更新）

> 「整体难度 / 建议学习路线」为辅导视角的主观参考；正式选课与评估请以对应 term 的官方 course outline 为准。

---

## 需要按 UNSW 定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
