# 🌐 Seaf 竞品周报 | 2026-06-29（第 16 期）

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动）** — 豆包大模型持续迭代，豆包1.5Pro/豆包1.5 Turbo 在多模态能力上强化，AI 助手 App 端新增语音克隆与情感对话功能，进一步提升 ToC 用户粘性。

📌 **通义千问（阿里云）** — 通义万相 2.0 视频生成能力向企业用户全量开放，通义 App 上线"超级助手"入口，支持多智能体协作编排个人日程与信息处理。

📌 **Kimi（月之暗面）** — Kimi 推出"多模态记忆"功能，支持跨会话记住用户偏好与知识图谱；Kimi API 平台新增 function calling 与流式输出优化，开发者体验持续改善。

📌 **DeepSeek（深度求索）** — DeepSeek-V3.5 开源权重发布，在推理效率与长上下文支持上有显著提升；DeepSeek Chat 新增深度搜索（Deep Search）模式，挑战 Perplexity 的问答体验。

📌 **ChatGPT（OpenAI）** — GPT-4o 新增"Memory across sessions"长期记忆能力，ChatGPT 可以记住用户的长期偏好与项目上下文；GPT-4o mini API 定价下调，ToC+ToB 双线竞争加剧。

📌 **Claude（Anthropic）** — Claude 3.7 Sonnet 持续强化 Agent 能力，新增 Computer Use 升级版，支持更稳定的浏览器操作自动化；Claude.ai 新增团队协作 Spaces 功能。

📌 **Gemini（Google）** — Gemini 2.5 Flash 成为 Google AI Studio 默认模型，Gemini API 新增语音输入/输出原生支持；Google Workspace 集成进一步深化，Gmail/Docs 内 AI 助手能力升级。

---

## 【ToB 智能体工厂】

📌 **Dify** — 发布 v1.15.0，带来全新 difyctl 命令行工具（跨平台 CLI，支持直接运行工作流）、工作流/Chatflow 原生 CoT 推理链展示、Human-in-the-Loop 表单增强（支持下拉与文件上传）、长耗时模型轮询机制及知识库 Excel 图片提取；修复路径遍历安全漏洞（CVE-2026-41948）。【[GitHub Release](https://github.com/langgenius/dify/releases/tag/v1.15.0)】

📌 **FastGPT** — 发布 v4.15.0-beta6，重构 Skill Edit 对话存储链路（统一标准 Chat 模型）、Agent Sandbox 新增 npm/PyPI 镜像源配置（提升私有网络依赖安装成功率）、LLM 请求追踪记录新增 teamId 字段实现团队隔离查询、对话标题生成模型迁移至页面系统默认模型配置；商业版支持本地直连调试插件。【[GitHub Release](https://github.com/labring/FastGPT/releases/tag/v4.15.0-beta6)】

📌 **Coze（字节）** — Coze 国内版持续完善 Bot Store 生态，海外版 Coze 推出 Agent SDK 支持企业级多 Agent 编排；Coze Bot 上线"多模态卡片"发布能力，支持在 IM 渠道内原生展示图文卡片。

📌 **LangFlow** — 社区版持续完善可视化 DAG 编排，v1.2.x 系列在组件丰富度与数据流可视化上有小幅迭代，主要聚焦稳定性与文档完善。

📌 **n8n** — n8n v1.90+ 发布，新增 AI Sub-nodes 增强包，支持在 n8n 工作流中更便捷地串联 LLM 节点与外部 API，AI Agent 节点支持多模型切换与 Token 预算控制。

---

## 【GitHub Trending AI 类项目】（本周）

💻 **[OpenMontage](https://github.com/calesthio/OpenMontage)** ⭐ 26,923 | ⬆️ 18,703 ⭐/周 | 世界首个开源 Agentic 视频制作系统，12 条管线、52 种工具、500+ Agent 技能，可将 AI 编码助手转变为完整视频工作室。

💻 **[codebase-memory-mcp](https://github.com/DeusData/codebase-memory-mcp)** ⭐ 19,622 | ⬆️ 8,926 ⭐/周 | 高性能代码智能 MCP 服务器，将代码库索引为持久知识图谱，支持 158 种语言、亚毫秒查询、99% 更少 Token，单二进制零依赖。

💻 **[design.md](https://github.com/google-labs-code/design.md)** ⭐ 22,834 | ⬆️ 6,728 ⭐/周 | Google Labs 出品，为 AI 编码助手提供视觉设计系统描述的格式规范，让 Agent 获得持久、结构化的设计语言理解能力。

💻 **[ai-website-cloner-template](https://github.com/JCodesMore/ai-website-cloner-template)** ⭐ 22,804 | ⬆️ 5,317 ⭐/周 | 一行命令克隆任意网站，专为 AI 编码 Agent 设计，支持 Claude/GPT/Claude 等主流 Agent 调用。

💻 **[daily_stock_analysis](https://github.com/ZhuLinsen/daily_stock_analysis)** ⭐ 51,109 | ⬆️ 7,045 ⭐/周 | LLM 驱动的多市场股票智能分析系统，支持多源行情、实时新闻、决策看板与零成本定时运行。

💻 **[Agent-Reach](https://github.com/Panniantong/Agent-Reach)** ⭐ 44,453 | ⬆️ 7,692 ⭐/周 | 让 AI Agent 具备"视力"读懂整个互联网，支持 Twitter/Reddit/YouTube/GitHub/B站/小红书，零 API 费用。

💻 **[voicebox](https://github.com/jamiepine/voicebox)** ⭐ 35,429 | ⬆️ 3,883 ⭐/周 | 开源 AI 语音工作室，支持克隆、听写、语音创建。

💻 **[orca](https://github.com/stablyai/orca)** ⭐ 8,607 | ⬆️ 2,769 ⭐/周 | 多并行 Agent 的 ADE（Agent Development Environment），支持用自己的订阅运行任意编码 Agent，跨桌面和移动端。

💻 **[Agent-Native](https://github.com/BuilderIO/agent-native)** ⭐ 2,884 | ⬆️ 1,540 ⭐/周 | Builder.io 出品，构建 Agent 原生应用的框架，聚焦 Agent 优先的应用架构范式。

💻 **[aws/agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws)** ⭐ 1,541 | ⬆️ 600 ⭐/周 | AWS 官方 MCP 服务器、Skills 和插件官方工具包，帮助 AI Agent 在 AWS 上构建应用。

---

## 【Seaf 机会点】

💡 **MCP 生态布局窗口期**：codebase-memory-mcp 一周 8,926 ⭐、aws/agent-toolkit-for-aws 持续增长，说明 MCP 工具生态正处于爆发期。Seaf 应加快 MCP 工具的接入与审核效率，建立 MCP 工具认证体系，形成差异化竞争力。

💡 **Agent Sandbox 镜像源支持**：FastGPT v4.15.0-beta6 在 Agent Sandbox 中新增 npm/PyPI 镜像配置，解决私有网络依赖安装痛点。Seaf 如有沙盒能力，应同步关注镜像源配置的灵活性，特别是面向企业内网部署场景。

💡 **工作流 CoT 可视化能力**：Dify v1.15.0 实现了工作流中的 CoT 推理链流式展示，将思考过程从最终回答中分离。这对 Seaf 的"日志回放+执行链"模块有直接参考价值，可考虑在调用日志中展示模型的推理过程（thinking），提升开发者调试体验。

💡 **CLI 工具降低使用门槛**：Dify difyctl 的发布说明 CLI 化是 ToB 平台的重要趋势。Seaf 可探索提供 openclaw CLI 或 seafctl 工具，支持开发者从终端直接管理智能体和工作流，拓展使用场景。

---

*数据来源：GitHub Releases / Trending / 公开报道 | 2026-06-29*
