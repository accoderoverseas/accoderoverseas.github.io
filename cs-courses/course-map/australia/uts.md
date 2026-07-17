---
title: 悉尼科技大学（University of Technology Sydney, UTS）
parent: 澳洲
grand_parent: 学校课程图谱
nav_order: 7
permalink: /cs-courses/course-map/australia/uts/
published_at: "2026-07-18 07:37:47"
---

<style>
/* 课程号-课程名统一紫色加粗（仅本页生效）：第一部分课程小标题 + 第二部分清单条目 */
.main-content h4 { color: #7253ed; }
.main-content h4 code { color: #7253ed; background: transparent; font-weight: 700; }
.main-content li:has(> code:first-child) { color: #7253ed; font-weight: 700; }
.main-content li:has(> code:first-child) > code:first-child { color: #7253ed; background: transparent; font-weight: 700; }
</style>

# 悉尼科技大学（University of Technology Sydney, UTS）

UTS CS 课程以六位数字编码。本页先整理指定的**核心 / 高频课程详解**，再保留原有的**完整「CS 课程体系（按类型）」清单**，便于按方向继续查课。

> **核验说明（2026-07-18）**：课程名称、课程简介、学习成果和开课信息均逐项对照 [UTS 2026 Course Handbook](https://coursehandbook.uts.edu.au/subject/2026/41039)。本文将官方标注为 **City campus · Spring Session · On campus - Weekly** 的 offering 视为 **2026 S2**，并且只为这类课程写入详解；不是“Spring”的课程不会混入。**整体难度和学习建议**是经验参考。UTS Handbook 提示须先在页面右上角选择 availability 才会显示对应 assessment information，当前公开页未统一给出可核实的固定权重，因此本页不以旧 outline 猜填比例；最终考核以当学期 Canvas subject outline 为准。

## 26S2 开课状态速查

| 专题 | 已确认 City campus Spring（纳入下方详解） | 不纳入 26S2 详解的指定课程 |
|:--|:--|:--|
| 编程 · 软件工程 · 项目 | `31268`、`31282`、`41026`、`41039`、`48024` | `41025`（仅 Autumn Session） |
| 算法 · 数据结构 · 理论 | `31251`、`41052`、`41080` | — |
| 计算机系统 · 体系结构 | `41001`、`41891`、`48033`、`48433` | — |
| 数据库 · 信息系统 | `31266`、`31271` | `31253`（2026 页面未列 availability）；`31257`（仅 Autumn Session） |
| 人工智能 · 机器学习 | `31005`、`31256`、`41040` | `41042`（2026 Handbook 页面为 404）；`41043`、`42028`（仅 Autumn Session） |
| 数据科学 · 数据分析 | `31250`、`32146` | — |

## 核心 / 高频课程详解

### 编程 · 软件工程 · 项目

#### [`31268` — Web Systems](https://coursehandbook.uts.edu.au/subject/2026/31268)
- **课程简介**：以 Web 为案例建立 IT 基础，不只做网页，还理解支撑网站的硬件、软件、网络与操作系统，并据此搭建可用网站。
- **主要知识点**：硬件 / 软件与进程、操作系统组件、网络安全基础、Linux 命令行与简单脚本、Internet 与 World Wide Web、分布式 Internet 应用、按规格设计和实现简单网站；大作业还会延展到网页美学与可访问性。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — Web 制作本身是入门级，但要同时消化 Linux、操作系统与网络的横向基础。
- **建议学习路线**：不要只把它当 HTML 课。先练熟命令行和文件操作，再用一个小站把“页面—服务器环境—网络访问”串起来；每周预习线上材料后再进 lab，效率更高。

#### [`31282` — Systems Testing and Quality Management](https://coursehandbook.uts.edu.au/subject/2026/31282)
- **课程简介**：聚焦如何度量和控制软件质量，学习软件质量保证、质量管理和系统 / 软件测试的实际做法。
- **主要知识点**：质量保证与质量管理原则、测试过程与阶段、测试类型和技术、测试计划、测试质量体系的协作规划、执行与文档化、用测试评估系统运行和功能。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 编码压力通常低于项目开发课，难点是把测试思路写成可执行、可追溯的方案。
- **建议学习路线**：课前完成 FLIP 视频与阅读，tutorial participation 会依赖这部分准备。对每个练习都问“测什么、为什么这样测、失败如何定位”，逐步建立测试用例而非只背术语。

#### [`41026` — Advanced Software Development](https://coursehandbook.uts.edu.au/subject/2026/41026)
- **课程简介**：在真实感较强的客户需求下，由高度自主的团队设计、开发和评估一个满足功能与非功能需求的复杂软件系统。
- **主要知识点**：需求获取与持续管理、功能 / 非功能需求、软件设计与实现、项目规划、团队角色与协作、进度汇报、面向利益相关者的项目沟通和交付评审。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 主要压力来自团队项目的工程量、协作和按节点交付，不是单纯写功能。
- **建议学习路线**：第一周就明确需求、分工、代码协作和 review 节奏；把每次向 tutor 的进度展示当作小型交付。开发时同时维护需求、设计、测试和决策记录，后期不会只剩“能跑但说不清”。

#### [`41039` — Programming 1](https://coursehandbook.uts.edu.au/subject/2026/41039)
- **课程简介**：面向编程起点的基础课，以项目式学习建立解决计算问题和清晰表达程序设计决策的能力。
- **主要知识点**：状态、分支、迭代、抽象建模、简单可运行程序的设计与实现、程序解释与文档、对不同设计方案的反思。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 语法不是唯一考点；持续练习、调试和把设计理由讲清楚更重要。
- **建议学习路线**：不要跳过每周的预习模块和分级练习。先自己写出最小可运行版本，再补测试、注释和改进方案；项目会把前面的知识连起来，遇到问题及时带到 weekly drop-in 解决。

#### [`48024` — Programming 2](https://coursehandbook.uts.edu.au/subject/2026/48024)
- **课程简介**：在 Java 或 Python 的实践中学习面向对象和 GUI 编程，目标是从规格出发设计、开发并评估具备可用性的业务系统。
- **主要知识点**：面向对象设计、类与对象、继承、列表、由规格构建 OO 方案、GUI 界面实现、代码调试与运行、从功能性和可用性评估软件质量。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 继承、对象协作和“由规格反推设计”会比基础语法更费脑。
- **建议学习路线**：每周先完成 Canvas study module 和前置 lab（未完成会锁定后续 lab 材料），再进两小时 lab 写代码。练习时先画类之间的职责和关系，避免一开始就把所有逻辑塞进一个类里。

### 算法 · 数据结构 · 理论

#### [`31251` — Data Structures and Algorithms](https://coursehandbook.uts.edu.au/subject/2026/31251)
- **课程简介**：用 C++ 学习数据结构与算法的设计、评价和实现，并将它们用于较复杂的问题与软件方案。
- **主要知识点**：C++ 与 IDE 中的程序设计、数据结构和算法的实现 / 比较 / 评价、将算法原则用于复杂与非结构化问题、功能性与可用性的权衡。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 抽象程度和 C++ 实现细节都会抬高门槛，不能只会调用现成容器。
- **建议学习路线**：按“概念 → 手写实现 → 复杂度 / 适用场景比较”推进。tutorial 是获得实现反馈的关键；每周写完后自己解释为什么选该结构、替代方案是什么。

#### [`41052` — Advanced Algorithms](https://coursehandbook.uts.edu.au/subject/2026/41052)
- **课程简介**：深入高级数据结构和算法技巧，重点处理图与优化类问题，并训练实现、测试和评价算法性能的完整能力。
- **主要知识点**：高级数据结构、算法范式、图问题、优化问题、计算复杂度、算法性能测试与评价、算法策略的协作式表达。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 难在从“会写”提升到“能设计并证明 / 评估为什么高效”。
- **建议学习路线**：开课前复习复杂度、基础图算法和递归。每道题至少留下三份记录：建模、复杂度、测试数据；测试驱动的探索式编程正好能暴露边界条件和性能误判。

#### [`41080` — Theory of Computing Science](https://coursehandbook.uts.edu.au/subject/2026/41080)
- **课程简介**：研究自动机、可判定性与计算复杂度，理解哪些问题能算、如何描述计算，以及理论如何落到解析、改写和算法效率判断。
- **主要知识点**：自动机与形式模型、图灵机、可判定 / 不可判定问题的证明、计算复杂度、算法效率分析与改进、为现实问题建立可计算模型。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐⭐ — 形式化定义、证明和抽象建模密集，是这组中最偏理论的一门。
- **建议学习路线**：每周 pre-work 后务必自己推一遍定义和证明，别只看懂例题。课程的个人作业、后续小组扩展任务和书面作业彼此衔接；从第一份作业开始就练习把“直觉”写成严格步骤。

### 计算机系统 · 体系结构

#### [`41001` — Cloud Computing and Software as a Service](https://coursehandbook.uts.edu.au/subject/2026/41001)
- **课程简介**：从云架构、虚拟化和多租户切入，结合研究报告与小组云应用，理解云服务如何支撑实际业务场景。
- **主要知识点**：云计算架构、IaaS / PaaS / SaaS、虚拟化、多租户、云服务在业务与公共服务中的应用、云平台原型、云应用开发与批判性分析。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 概念跨度大，但每周 lab 会把理论落到云端小应用；难点是兼顾技术实现和小组研究表达。
- **建议学习路线**：用同一个应用场景分别思考 IaaS、PaaS、SaaS 的边界；每周 lab 的 mini-application 及时完成，团队报告与应用开发都不要等到最后再整合。

#### [`41891` — Cloud Computing Infrastructure](https://coursehandbook.uts.edu.au/subject/2026/41891)
- **课程简介**：进一步研究云基础设施的搭建与运行：架构、虚拟化、存储、数据中心，以及安全和合规问题，并在 lab 使用行业相关工具。
- **主要知识点**：IaaS 平台、虚拟化、云存储与数据中心基础、云安全 / 合规、数据主权与司法辖区风险、动态扩缩容、SLA、面向小型企业的云基础设施设计。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 既要配置 / 实现，又要解释性能、成本、风险和业务约束之间的取舍。
- **建议学习路线**：从第一周开始完成每个 lab，并固定和 tutor 核对配置与未完成项。大作业发布后先谈好 learning contract，再逐步做设计和实现；不要把安全、数据主权和 SLA 留在报告收尾才补。

#### [`48033` — Internet of Things](https://coursehandbook.uts.edu.au/subject/2026/48033)
- **课程简介**：构建对 IoT 系统的端到端认识：感知与执行、通信 / 网络、信号和数据处理，以及 AI 如何服务于实际 IoT 应用。
- **主要知识点**：传感与执行技术、IoT 通信和网络、IoT 信号 / 数据处理、传感器网络与遥测、IoT 数据分析、使用 microcontroller 与 sensor kit 开发小型项目、ThingSpeak、Git 与云平台。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 硬件、网络、数据和项目实现同时出现，调试链路更长。
- **建议学习路线**：按“传感数据采集 → 传输 → 云端处理 → 展示 / 控制”拆解每次 lab；先让最小链路跑通，再扩展功能。书本与 lecture 预读能明显降低 lab 现场排错成本。

#### [`48433` — Software Architecture](https://coursehandbook.uts.edu.au/subject/2026/48433)
- **课程简介**：学习为真实行业问题设计、开发和评估软件架构，并用架构工具、方法和多视图表达作出有依据的决策。
- **主要知识点**：架构模式、利益相关者与架构需求、性能 / 安全 / 可维护性 / 可靠性 / 可用性等质量属性、架构方案比较、概念 / 执行 / 实现多视图、架构评审。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 不是背模式名，而是要能解释某种架构如何满足或牺牲特定质量属性。
- **建议学习路线**：按周完成线上 lecture 和 quiz，再带着一个贯穿案例进 tutorial。大作业期间要认真做团队互评：把“哪里可能失效、怎样验证”说清楚，比画一张漂亮图更重要。

### 数据库 · 信息系统

#### [`31266` — Introduction to Information Systems](https://coursehandbook.uts.edu.au/subject/2026/31266)
- **课程简介**：从社会、组织和业务语境理解信息系统如何被获取、实施、维护并帮助组织形成竞争优势，同时讨论伦理、隐私与安全。
- **主要知识点**：信息系统与业务环境、信息系统获取过程、电信与网络概念、数据管理与知识管理、组织竞争优势、信息系统伦理、隐私与安全、案例分析与协作讨论。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 代码门槛低，挑战在于把案例和概念连起来，清晰论证组织层面的选择。
- **建议学习路线**：每周 lecture 后先用一个企业案例回答“问题、系统、数据、风险、价值”五个问题，再做 tutorial。Bachelor of Computing Science 学生还要留意官方列出的 OPELA / Language Development Tutorials 要求，未完成可能影响通过。

#### [`31271` — Database Fundamentals](https://coursehandbook.uts.edu.au/subject/2026/31271)
- **课程简介**：从组织中的数据结构和管理出发，建立数据库设计基础，并用 SQL 完成数据检索和修改，配合实操与案例分析。
- **主要知识点**：数据库设计、概念数据模型、数据冗余、规范化与数据完整性、SQL 查询与数据修改、数据库在应用开发中的作用。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 入门路径清晰，但规范化和多条件 SQL 容易在细节上丢分。
- **建议学习路线**：先把实体、关系和键画成模型，再落到表和 SQL；每周独立改写 tutorial 查询，不要只看答案。提交前用能暴露冗余和约束问题的数据测试设计。

### 人工智能 · 机器学习

#### [`31005` — Machine Learning](https://coursehandbook.uts.edu.au/subject/2026/31005)
- **课程简介**：通过理论学习和编程实践，掌握将机器学习方法用于智能系统和专业领域问题的能力，覆盖基础与进阶算法的应用边界。
- **主要知识点**：机器学习问题建模、机器学习方法的使用或编程实现、算法理论与实现教程、方法的适用范围和局限、专业领域方案设计、项目实践。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 要同时理解算法原理、完成实现并判断何时不该用某种方法，数学和编程基础会直接影响体验。
- **建议学习路线**：预习材料看完后，自己重写一遍算法 tutorial 的关键步骤并替换数据验证。每周 in-class test 用来即时查漏，项目不要等到模型堆不动才开始补理论。

#### [`31256` — Image Processing and Pattern Recognition](https://coursehandbook.uts.edu.au/subject/2026/31256)
- **课程简介**：学习图像处理和模式识别原理，开发用于自动图像 / 视频分析的软件，并在团队项目中处理真实应用问题。
- **主要知识点**：图像与视频目标 / 活动检测、MATLAB 脚本、图像滤波、分割、局部特征、统计分类器及其他分类器、问题规格、实现与展示。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐⭐☆ — 数学直觉、MATLAB 实操和团队项目缺一不可，视觉结果“看起来对”不等于方法正确。
- **建议学习路线**：每次课前完成 Canvas 的短视频和引导问题，lab 中立即验证滤波、分割和特征的效果。团队项目先写清问题规格和评价标准，利用 week 4 的形成性 quiz 与项目中途反馈及时修正。

#### [`41040` — Introduction to Artificial Intelligence](https://coursehandbook.uts.edu.au/subject/2026/41040)
- **课程简介**：以讲授和实践 lab 建立 AI 的全景认知，学习为简单现实问题选择恰当模型与算法，并完成 AI 应用示例和小组项目。
- **主要知识点**：机器学习、自然语言处理、计算机视觉、搜索、知识表示、推理、AI 方法选择、简单 AI 应用设计与团队沟通。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 覆盖面广但以入门应用为目标；真正的挑战是不要把搜索、推理、学习等方法混成一团。
- **建议学习路线**：先用“问题表示—可用知识—搜索 / 推理 / 学习方法—评估”框架整理每种 AI 技术。前半学期 lab 的 demo 要亲手改动，后半学期 tutorial 的知识表示与推理例题要多画图；课程官方说明含 open-book exam、AI mini demos 和小组项目。

### 数据科学 · 数据分析

#### [`31250` — Introduction to Data Analytics](https://coursehandbook.uts.edu.au/subject/2026/31250)
- **课程简介**：从大型复杂数据中形成可行动洞察，学习数据预处理、探索、可视化和预测建模，并能把结果讲给业务利益相关者。
- **主要知识点**：数据预处理、探索性分析、可视化、预测趋势的数据分析技术、数据挖掘项目、不同方法的可能性与局限、业务语境中的洞察沟通。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 工具操作并非最难，难在选对方法、解释结果，以及把技术发现转成业务语言。
- **建议学习路线**：把每份数据作业固定成“问题—清洗—探索—方法—结果—限制—建议”的流程。课前准备 Canvas 材料，三小时 workshop / lab 用来真正跑工具；持续 quiz 很适合每周复盘薄弱概念。

#### [`32146` — Data Visualisation and Visual Analytics](https://coursehandbook.uts.edu.au/subject/2026/32146)
- **课程简介**：研究支撑视觉分析和决策的数据可视化、交互与界面设计，训练用高级软件将数据变成适合特定人群的数据故事。
- **主要知识点**：静态与交互式可视化、视觉数据分析流程、人机交互、数据故事、面向社会情境和特定用户的可视化设计、可视化界面评价、相关研究文献与软件实践。
- **2026 S2 开课**：City campus，On campus - Weekly。
- **整体难度**：⭐⭐⭐☆☆ — 编程未必是主障碍，难点在“图为什么适合这个用户和问题”的设计判断与迭代。
- **建议学习路线**：别只追求图表好看。每次作品先写清目标用户、要发现的模式和交互目的，再选择编码方式；week 2–12 的 self-paced workshop 要按周完成，主动拿 peer / staff feedback 改图。

## 官方来源与使用说明

- 每门详解的标题都链接至对应的 **UTS 2026 Course Handbook** 页面；该页的 *Offerings* 是本页判断 26S2 的唯一依据。
- UTS 把授课期写作 **Autumn Session / Spring Session**。本页的“26S2”仅指上表所列 **City campus Spring Session**，不以海外或其他 teaching period 替代。
- 选课前还应在课程页的 *Requisites* 区域打开官方 **access conditions**，确认自己满足先修、限修与学位规则；具体 assessment 与时间表以已选 availability 后的 Handbook、Canvas 和当学期 subject outline 为准。

## CS 课程体系（按类型）

**编程 · 软件工程 · 项目**

- `31097` — IT Operations Management
- `31242` — Advanced Internet Programming
- `31245` — Business Process and IT Strategy
- `31247` — Collaborative Business Processes
- `31255` — Finance and IT Professionals
- `31258` — Innovations for Global Relationship Management
- `31268` — Web Systems
- `31269` — Business Requirements Modelling
- `31272` — Project Management and the Professional
- `31280` — Strategic IT Project
- `31282` — Systems Testing and Quality Management
- `31482` — Honours Project
- `31748` — Programming on the Internet
- `31927` — Application Development with .NET
- `32144` — Technology Research Preparation
- `32931` — Technology Research Methods
- `41025` — Introduction to Software Development
- `41026` — Advanced Software Development
- `41039` — Programming 1
- `41078` — Computing Science Studio 1
- `41079` — Computing Science Studio 2
- `41113` — Software Development Studio 1
- `41114` — Software Development Studio 2
- `41889` — Application Development in the iOS Environment
- `42913` — Social and Information Network Analysis
- `48024` — Programming 2

**算法 · 数据结构 · 理论**

- `31251` — Data Structures and Algorithms
- `41052` — Advanced Algorithms
- `41080` — Theory of Computing Science

**计算机系统 · 体系结构**

- `41001` — Cloud Computing and Software as a Service
- `41891` — Cloud Computing Infrastructure
- `48033` — Internet of Things
- `48433` — Software Architecture

**计算机网络**

- `31276` — Networked Enterprise Architecture
- `41092` — Network Fundamentals

**数据库 · 信息系统**

- `31253` — Database Programming
- `31257` — Information System Development Methodologies
- `31266` — Introduction to Information Systems
- `31271` — Database Fundamentals

**人工智能 · 机器学习**

- `31005` — Machine Learning
- `31243` — AI/Analytics Capstone Project B
- `31256` — Image Processing and Pattern Recognition
- `41004` — AI/Analytics Capstone Project
- `41040` — Introduction to Artificial Intelligence
- `41041` — Emerging Topics in Artificial Intelligence
- `41042` — Introduction to Computational Intelligence
- `41043` — Natural Language Processing
- `41077` — Data Driven and Intelligent Robotics
- `42028` — Deep Learning and Convolutional Neural Network

**数据科学 · 数据分析**

- `31250` — Introduction to Data Analytics
- `32146` — Data Visualisation and Visual Analytics

**网络安全**

- `48730` — Cybersecurity
---

## 需要按这所学校定制辅导？
选课不确定值不值得选、已选课想搭知识体系、考前（含 hurdle 科目）没头绪——**[联系我](/contact/)** 做 1v1 辅导 / 陪练，按你的课程大纲定制方案，帮你把课程彻底弄懂吃透。
