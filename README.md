<h1 align="center">🎓 计算机与人工智能方向复试展示档案</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=0969DA&center=true&vCenter=true&width=600&height=50&lines=你好，我是黄信博+👋;专注于+大模型微调+与+AI+应用架构落地;具备从0到1的数据管线与RAG系统开发经验;欢迎来到我的复试作品集仓库！" alt="Typing SVG" />
</p>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=storyeer&show_icons=true&theme=tokyonight&hide_border=true&ring_color=0969DA" alt="GitHub stats" />
  <br><br>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Neo4j-018bff?style=for-the-badge&logo=neo4j&logoColor=white" />
</div>

<br>

> 本仓库收录了我在本科（南京审计大学 数据科学与大数据技术，2022-至今）及实习期间主导或参与的核心项目，旨在全面展示我的**学术研究能力**、**AI 工程落地经验**以及**高并发复杂系统架构设计能力**。

- 📧 **联系方式**: 222090532@stu.nau.edu.cn | 133-3816-7290

---

## 🚀 核心研发经历与产出

### 1. 🏅 审计大模型课题组：基于微调的财务异常与工程合规模型增强
*大模型微调 (Fine-tuning) · 领域专用模型 (Domain-specific LLM) · 提示词工程 (Prompt Engineering)*
>**项目时间**: 2024.03 - 2025.03

* **清洗与去重管线**：设计基于 TF-IDF 提取稀疏向量并结合余弦相似度的轻量去重算法，将百万级异构审计语料重复率由 15% 降至 5%，交付 **1万+** 纯净指令微调集。
* **模型微调实战**：基于 Qwen (2/2.5/3) 系列基座，设计并执行 48 组 `QLoRA` 正交实验，探索最优学习率退火路径与吞吐批次。
* **业务落地成效**：使得审计风险有效识别率**从 50% 显著提升至 82%**，报告逻辑完整度达 70%。

<details>
<summary>💡 <b>展开查看：工程亮点与算力优化机制 (点击展开)</b></summary>
<br>
<blockquote>
突破性引入了 <b>“失效快跑（Fail-Fast）前置校验漏斗”</b> 机制。在昂贵的张量推理前，通过句间余弦相似度极速评估文本连贯性，精准拦截乱码与无关段落。经测算，该早停机制有效保护了数据集纯净度，并<b>节约了多达 45% 的无效算力开销</b>。
</blockquote>
</details>

<br>

### 2. 🧩 基于 LLM 的智能语义分块与增强检索 RAG 框架
*检索增强生成 (RAG) · 混合大模型推理架构 · 智能文档解析切割*
>**项目时间**: 2025.03 - 2025.08

* **击破截断瓶颈**：独立研发突破传统 Token 暴力定长截断的新型 RAG 框架，实现基于上下文的“按语义边界智能分块”。
* **双模态异构调度**：采用 **DeepSeek (结构化解析分块) + Qwen3 (下游检索生成)** 的解耦架构协作，提升资源伸缩性。

<details>
<summary>💡 <b>展开查看：核心技术难点破局 (点击展开)</b></summary>
<br>
<blockquote>
在高度复杂的表格与嵌套列表中，成功保留了核心上下文元数据 (Metadata)，从根本上缓解了超长文本处理时易发的 <b>幻觉 (Hallucination) 与注意力漂移</b> 问题。
</blockquote>
</details>

<br>

### 3. ⚡ 面向速率受限 API 的高性能动态异步调用框架
*高并发工程 · 分布式限流 · 闭环反馈系统*
>**项目时间**: 2025.01 - 2025.05

* **核心贡献**: 独立架构了一套闭环反馈控制引擎，攻克了微服务集群因粗暴触碰 API Rate Limit 导致的雪崩与性能倒挂。
* **技术创新**: 采用基于下游 API 响应状态的**动态调度自适应机制**（而非暴力硬等待）；全链路埋点监控，内置自动化断路器与退火重试逻辑。**本项目已梳理为发明专利申请中**。

---

## 💼 业务级海量数据处理经验：如皋市审计局实习

> 聚焦建筑工程招标舞弊风险，独立主导搭建 Python 自动化数据审计清洗分析链。

* **实体精准嗅探**：设计数十组沉浸式正则表达式，从数百万异构混排文件中精准剥离 “投标保证金账户”、“项目经理社保” 等 12 类高敏特征。
* **🚀 引擎提速重构**：直面 Python GIL 全局解释器锁瓶颈。果断重构代码架构，落地 **多进程 (Multiprocessing) 并行调度网络**，将 10 万条单批次数据洗牌耗时 **自 8 小时硬核斩断至 5 小时**。
* **实战战果**：协助查实违规案件 12 起（**涉案逾人民币 2000 万元**），脚本受编入市局官方反舞弊工具库。

---

## 🛠 专业技能雷达 (Tech Stack Radar)

| 体系架构层级 | 核心技术栈 |
| :--- | :--- |
| **🧠 算法与大模型域** | `大语言模型微调 (QLoRA)` • `RAG / 向量检索` • `提示词工程 (CoT解构)` • `Neo4j (知识图谱)` |
| **🔨 工程基建与数仓** | `Python (熟练)` • `C 语言` • `Pandas (海量数据清洗)` • `SQL` |
| **⚙️ 高级编程与性能** | `多进程/协程高并发设计` • `API 动态抗压限流` • `正则表达式与文本解析` |

---

## 🏆 学术竞赛与社会荣誉 (Honors & Awards)

* 🥇 **2024.05** - 第十四届 MathorCup 数学应用挑战赛 **[ 🏆 国家一等奖 ]**
* 🥈 **2024.03** - 美国大学生数学建模竞赛 (MCM/ICM) **[ 🏅 Honorable Mention (H 奖) ]** 
    * *(独立负责核心系统仿真与模型寻优求解)*
* 🏅 **2024.05** - 大学生创新创业训练计划 **[ 🚀 省级立项 (一作/负责人) ]**
* 🥉 **2023.08** - 第十六届中国大学生计算机设计大赛 **[ 🥈 省级三等奖 (团队负责人) ]**
    * *(领衔研发“审计智能问答大模型”前身矩阵)*
* ⭐ **2023.10** - 大学生社会实践“千校千项” **国家级优秀项目 (队长)**

---
<p align="center">
<i><b>"Talk is cheap. Show me the code (and the AI capabilities)."</b> - A passionate learner driven by engineering and fundamental truths.</i>
</p>
