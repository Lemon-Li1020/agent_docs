# Seaf 竞品周报 | 2026年8月31日（2026年第35周）

---

## 【ToC 智能体助手】

📌 **豆包** — 持续优化多模态理解与视频理解能力，豆包电脑版上线深度研究模式，支持联网搜索与长文生成。

📌 **ChatGPT** — OpenAI 发布 ChatGPT 新界面集成 codex CLI，桌面端支持原生 terminal 集成编程能力（本周 GitHub codex 项目开放）。

📌 **Claude** — Anthropic 发布 Claude Code 官方插件市场（claude-plugins-official），本周新增数千 star，社区插件生态快速扩张。

📌 **DeepSeek** — DeepSeek 发布 V3.5 系列更新，上下文窗口扩展至 256K，支持超长文档分析与代码库推理。

📌 **Kimi（月之暗面）** — Kimi 多模态模型发布新版本，视觉推理能力大幅提升，支持复杂图表解析与结构化输出。

📌 **通义千问（阿里）** — 阿里发布 Qwen3.5-2B/9B 开源小模型系列，ASIL 评测中表现优异（Qwen3.5-9B + RL 微调达 82.2 分）。

📌 **Gemini（Google）** — Google 发布 Gemini 多模态 Embedder（OmniUE），支持文本、视频、音频任意组合的跨模态检索。

---

## 【ToB 智能体工厂】

📌 **Dify** — 发布 Agent 大版本更新（2025年8月25日）：新增 E2B 云沙盒后端、Build-time Home Snapshots（构建时环境快照）、Workspace 级别 Skill 管理体系、Context-aware 历史压缩、Go to Anything（⌘K 全局搜索）、Cloudflare Turnstile 验证码支持、TiDB 向量混合检索等重量级功能。[[GitHub](https://github.com/langgenius/dify/releases)]

📌 **FastGPT** — 发布 v4.16.1：小版本修复与优化，重点包括 MCP/HTTP 工具 JSON Schema 统一为字符串存储（解决与 Mongo 规则冲突）、团队系统插件管理、第三方发布渠道支持多模态文件/音频转录、沙盒支持自定义 apt 源等。[[GitHub](https://github.com/labring/fastgpt/releases)]

📌 **Coze（扣子）** — 字节 Coze 持续优化多 Agent 协作与工作流编排能力，国内企业版推进 MCP 工具市场集成。

📌 **LangFlow** — 开源可视化 LangChain 工作流编辑器持续迭代，新增 RAG 组件与向量数据库深度集成。

---

## 【GitHub Trending AI 类】

💻 **freestylefly/awesome-gpt-image-2** ⭐25,640 | ⬆️13,413 本周 | GPT-Image2 工业级提示词引擎与模板库，530+ 案例逆向工程

💻 **anthropics/claude-plugins-community** ⭐2,877 | ⬆️2,162 本周 | Claude Cowork/Code 社区插件市场镜像

💻 **tt-a1i/archify** ⭐34,523 | ⬆️18,103 本周 | Agent 架构图表生成 Skill，支持工作流/序列/数据流图

💻 **apache/maka** ⭐4,187 | ⬆️1,973 本周 | Apache 本地优先 AI Agent 工作空间，append-only log 记录

💻 **MadsLorentzen/ai-job-search** ⭐38,521 | ⬆️5,348 本周 | Claude Code 求职应用框架，AI 简历/求职信/面试准备

💻 **K-Dense-AI/scientific-agent-skills** ⭐39,212 | ⬆️4,309 本周 | 科学 Agent Skills 库，165+ 验证技能，覆盖生物/化学/医学

💻 **Alishahryar1/free-claude-code** ⭐51,932 | ⬆️4,324 本周 | 免费使用 Claude Code/Codex/Pi 等（1.3B+ 免费 Token）

💻 **rohitg00/ai-engineering-from-scratch** ⭐51,270 | ⬆️3,720 本周 | AI 工程从零到一学习路线

💻 **tashfeenahmed/freellmapi** ⭐22,769 | ⬆️3,037 本周 | 34 家 LLM 提供商、635 免费端点，智能路由与自动故障转移

💻 **tinyhumansai/openhuman** ⭐39,014 | ⬆️2,526 本周 | 本地优先个人 AI 超脑，Agent 编排与记忆管理

---

## 【本周热门 arXiv 论文】

📄 **WikiSkill: Compiling Agent Experience into Persistent Knowledge for Skill Evolution** [arXiv:2608.27454]
- 将 Agent 执行经验持久化为可复用 Skill 的知识库框架，Skill 进化与模型规模互补

📄 **ASIL: Replacing Screenshot-and-Click with Structured State and Semantic Actions** [arXiv:2608.26991]
- 提出 Agent-原生软件交互层，在 15 应用 300 任务上达 80+ 准确率，超越截图方案 6 倍

📄 **Naive Prompt Optimization (NPO)** [arXiv:2608.27266]
- 简单线性 prompt 优化可媲美复杂搜索方法，揭示优化器端搜索复杂度的非必要性

📄 **OmniUE: Omni-Interactive Universal Embedder** [arXiv:2608.27044]
- 首个支持文本/视频/音频任意交互查询的统一多模态 Embedder，刷新多项 SOTA

📄 **BekchiAI: Measuring & Controlling LLM Agents** [arXiv:2608.26867]
- 提出 Agentic Skill 评测基准（13 类 ReAct Agent、2057 任务）及实时可观测平台

---

## 【Seaf 机会点】

💡 **Skill 体系加速构建**：Dify 本周重磅推出 Workspace 级 Skill 管理体系（draft→publish→version 生命周期），标志 Skill 化开发范式进入主流。Seaf 应加快 Skill 审核/发布流程的打磨，提前布局 Skill 市场，并参考 WikiSkill 的持久化知识积累思路，提升 Skill 可复用性与跨 Agent 迁移能力。

💡 **Agent 可观测性补齐**：BekchiAI 等论文揭示 Agent 执行过程的深度可观测性（token 级延迟、工具调用链路、URL 幻觉检测）正成为企业刚需。Dify 已上线统一 Tracing（支持 Phoenix/LangSmith），Seaf 应完善日志回放与 Langfuse 执行链的集成，提供比 Dify 更细粒度的调试体验。

💡 **MCP 生态与工具治理**：FastGPT v4.16.1 完成 MCP/HTTP 工具 Schema 标准化（Dify 同期也在深化工具链），MCP 工具生态正在快速收敛。Seaf 应完善 MCP 工具的发布→审核→上线全链路，突出工具的可发现性与版本管理优势，形成差异化。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-08-31*
