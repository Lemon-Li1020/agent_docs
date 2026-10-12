# 🌐 Seaf 竞品周报 | 2026-10-12（第41期）

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动）** — **Seedance 2.0 视频生成模型全面接入豆包**，登录即可免费使用；同步上线**"任务模式"**（从需求输入到结果交付的闭环），并向全场景 Agent 生态继续演进。

📌 **通义千问（阿里）** — 发布 **Qwen3.8-Max**（2.4 万亿参数），在编码、办公、研究与长周期任务上全面提升；配套 **Qwen-Image 3.0-Pro** 支持复杂版面一次生成、12 种语言 20+ 字体原生渲染，图像生成向生产力工具靠拢。

📌 **Kimi（月之暗面）** — **Kimi K3** 正式上线：2.8 万亿参数、基于 KDA 混合线性注意力（Kimi Delta Attention）与注意力残差技术、原生视觉理解、100 万 token 上下文；产品侧推出 **Swarm 智能体集群**与 **Goal 模式**并行执行任务，并支持 Kimi Work 桌面端浏览器 Agent。

📌 **DeepSeek** — 本周无新模型发布，延续 **DeepSeek-V4.1-Flash / V4-Pro**（V4-Pro-0813 已于 8 月 GA、MIT 权重开源）的 API 服务，保持长上下文（1M）与低价策略。

📌 **ChatGPT（OpenAI）** — 发布新版**桌面 App 体验路线图**（10-09），把聊天、Projects 与工具整合进统一工作区，并支持从应用/文件/浏览器/截图引入上下文；延续 GPT-6 系列型号迭代。

📌 **Claude（Anthropic）** — 本周公开渠道无新版本，最新仍为 **Claude Opus 5.5**（成本较上一代下降、多个任务接近前沿水平）。

📌 **Gemini（Google / DeepMind）** — 延续面向免费用户开放 **Gemini Skills**，持续在多模态实时交互与政企私有 AI 计算方向布局，本周无重大更新。

---

## 【ToB 智能体工厂】

📌 **Dify** — 最新版本仍为 **v1.17.1**（2026-09-10），本周无新 Release。
- **数据集级知识库 API Key**：Key 可绑定指定知识库，越权访问其他数据集（含 list-all）返回 403，解决"一个 key 通吃整个工作区"的权限隐患。
- **工作流键盘操作**：节点 / 多选 / 评论标记支持方向键移动（Shift 大步），松键合并为一条撤销记录。
- **市场创作者主页 + 首页改版**：作者公开主页 `/marketplace/creator/`，首页重构为 hero + 轮播 + 吸顶搜索 + 标签筛选。
- ⚠️ **升级警示**：自托管且使用内置 Weaviate 的部署需**分阶段手动升级**（1.27.0 → 1.39.2，跨 12 个 minor），跳版会静默且永久破坏向量检索。
- 🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT** — 发布 **v4.17.2**（2026-10-09）。
- **知识库数据提前落库 + 训练链路重构**：解析分块/图片导入内容解析完成后立即落库为可见数据行，全流程绑定唯一 `dataId`，训练完成后向量与索引写回同一条数据，杜绝长训练周期无数据、中断残留孤儿数据。
- **数据索引三态流转**（`parsed` → `indexing` → `indexed`）：待索引数据在检索层天然隔离、不被召回；训练失败数据支持直接编辑或删除。
- **目录子树搜索**：知识库/文件列表在指定目录下搜索时自动限定当前路径及全部子文件夹，根目录下保持全量检索（含成环与深度截断保护）。
- **前端 CSR + 浅路由迁移**：智能体、技能、MCP、模板市场、评测、账号中心、管理后台等全面迁移客户端渲染，消除页面切换白屏、提升响应速度。
- 🔗 https://github.com/labring/fastgpt/releases

---

## 【GitHub Trending AI 类】（本周）

💻 **thedotmack/claude-mem** ⭐99,738 | ⬆️ +3,803 | 跨会话持久上下文：捕获 agent 会话、AI 压缩后回注未来会话（兼容 Claude Code / OpenClaw / Codex / Gemini 等）

💻 **heygen-com/hyperframes** ⭐60,966 | ⬆️ +4,223 | 写 HTML 渲染视频，为 agent 打造的视频生成框架

💻 **earthtojake/text-to-cad** ⭐19,254 | ⬆️ +2,508 | 给 agent 装上 CAD 超能力（文本 → CAD 建模）

💻 **tester-army/e2e** ⭐9,040 | ⬆️ +6,440 | 面向 Web 与移动应用的新一代端到端测试框架

💻 **cursor/plugins** ⭐10,898 | ⬆️ +1,140 | Cursor 插件规范与官方插件

💻 **mvschwarz/openrig** ⭐6,973 | ⬆️ +2,028 | 用 Claude Code / Codex / Pi 组建 agent 网络：带角色、共享上下文与任务归属的持久团队

💻 **mattpocock/skills** ⭐快速增长 | — | "写给真实工程师的 Skills"，直接来自作者的 .agents 目录

💻 **ranxianglei/billion-context** ⭐903 | ⬆️ +337 | 面向小窗口的上下文压缩插件（100K 上下文即可、省 5 倍 token、支持数月级超长会话）

---

## 【arXiv cs.AI 近期精选】（Agent / LLM / MCP）

📄 **From Reactive Containment to Proactive Assurance: Lessons from OpenAI, Anthropic, and Google Agent Security Incidents** — 从三大厂商 Agent 安全事件提炼"主动保障"框架
📄 **OnTrack: Real-Time Monitoring and Intervention in LLM Agent Trajectories via Streaming Structure-Aware Optimal Transport** — Agent 轨迹实时监控与干预
📄 **Accurate but Not Humble: Evaluating Epistemic Humility in LLM Agents under Knowledge Conflict** — 知识冲突下 Agent 的"认知谦逊"评测
📄 **Ecology of AI Agents: Collaboration Creates a Population Threshold for Takeoff** — 多 Agent 协作的"起飞"人口阈值
📄 **Use and Disuse: Intent-Structured Experience Consolidation for Memory and Learning in LLM Agents** — Agent 记忆与学习的意图结构化经验固化
📄 **A Closer Look at Agentic BBO: Benchmarking LLM Agents for Black-Box Optimization** — Agent 黑盒优化能力基准
📄 **Recursive Self-Improvement through Multi-Agent Self-Supervision** — 多 Agent 自监督的递归自我改进

---

## 【Seaf 机会点】

💡 **1. 复用知识库"落库—索引"治理经验，主打可靠性与可观测性**
FastGPT v4.17.2 把"数据提前落库 + 索引三态（parsed/indexing/indexed）+ 检索层隔离"做成体系，Dify 也强化了知识库权限与抽取修复。Seaf 可在知识库/RAG 模块对标补上**数据行-向量一致性校验、训练失败可编辑可重试、检索等价性回归测试**，把"不静默出错"变成卖点。

💡 **2. 跟随 Agent 记忆与跨会话上下文这一高热度方向**
claude-mem（周 +3,803）、billion-context、以及 arXiv 上关于 Agent 记忆/经验固化的多篇论文，说明"持久记忆 + 上下文压缩"是当前最热需求。Seaf 可接入/自研**跨会话记忆层 + 上下文压缩插件**，并给出插件市场化的接入规范，抢占开发者心智。

💡 **3. 把 Agent 安全与 MCP 治理产品化**
arXiv 上"Agent 安全事件 → 主动保障""Agent 轨迹实时监控"等论文密集出现，Dify 也在收紧 Key/数据集作用域。Seaf 宜尽早补齐**细粒度权限（数据集/工具/MCP 作用域）、运行轨迹监控与干预、越权访问拦截**，作为 ToB 智能体工厂的合规与安全底座，形成与开源平台的差异化。

---

*数据来源：GitHub Releases / Trending / arXiv / 公开报道 | 2026-10-12*
