# 🌐 Seaf 竞品周报 | 2026-05-25（第 8 期）

---

## 【ToC 智能体助手】

📌 **豆包（字节）** — 豆包 PC 端持续优化多 Agent 协作与插件生态，上线新版知识库问答体验；C 端用户量保持国内领先，豆包模型持续迭代上下文与推理能力。

📌 **通义千问（阿里）** — 通义继续深化企业端渗透，Qwen3 系列开源模型社区热度高，配套工具链（ModelScope、PAI）持续完善，多模态能力向 Agent 场景扩展。

📌 **Kimi（月之暗面）** — Kimi 继续保持长上下文窗口优势，发布新版浏览器插件与 API 更新，Kimi+ 智能体市场持续扩充模板与工具。

📌 **DeepSeek** — DeepSeek-V3 模型性能逼近 GPT-4o，R1 推理模型引发全球关注；开源社区活跃，企业级 API 价格优势明显，越来越多 Agent 平台开始接入 DeepSeek。

📌 **ChatGPT（OpenAI）** — OpenAI 发布 GPT-4o 更新与 Agent SDK 增强版，Operator 功能向 Plus 用户全面开放，Canvas 协作编辑正式上线，Code Interpreter 能力显著提升。

📌 **Claude（Anthropic）** — Claude 4 发布预期升温，Artifex 模型专注长任务与工具调用；MCP 协议生态持续扩张，已有多家平台原生集成。

📌 **Gemini（Google）** — Gemini 2.5 Pro 在多模态推理评测中持续领先，Deep Research 功能升级，Agent 工具集（Agent Development Kit）向开发者全面开放。

---

## 【ToB 智能体工厂】

📌 **Dify** — 发布 v1.14.2 安全补丁（多租户隔离加固、工具凭证权限收紧），v1.14.1 引入 Docker Compose 环境变量重构与可配置 Explore 分类；v1.14.0 正式上线**协作编辑（Collaboration）**功能，支持工作流多人实时协同编辑，HITL 新增服务 API，MCP 元数据刷新机制优化，@langgenius/dify-ui 设计系统持续完善。
  - 🔗 https://github.com/langgenius/dify/releases/tag/v1.14.2

📌 **FastGPT** — 发布 v4.15.0-beta2，重写 AgentV2 loop 逻辑为线性 messages loop，**新增 Skill 编辑与使用支持**（仅静态 Skill），知识库搜索支持原生多模态 embedding 与图搜图，异常中断会话通过 Redis stream 心跳检测实现 2 分钟快速恢复；v4.14.22 修复工作流默认模型回传问题；整体向 Skill 生态与沙箱稳定性方向快速迭代。
  - 🔗 https://github.com/labring/fastgpt/releases/tag/v4.15.0-beta2

📌 **Coze（扣子）** — Coze 国内版持续完善 Bot Store 与工作流编排，扣子星尘插件市场活跃；Coze Enterprise 向企业级 MCP 管理与知识库集成方向深化。

📌 **LangFlow** — 本周社区更新围绕可视化 DAG 编排与 LangChain/LangGraph 集成优化，版本迭代节奏稳定。

---

## 【GitHub Trending AI 类】

💻 **openhuman** ⭐27.1k | ⬆️+15.2k | 私人 AI 超级智能体，Rust 实现，主打本地隐私与高性能

💻 **codegraph** ⭐21.9k | ⬆️+18.1k | 为 Claude Code/Cursor 等 Coding Agent 预索引代码知识图谱，减少 token 消耗与工具调用

💻 **Understand-Anything** ⭐25.7k | ⬆️+9.1k | 将任意代码转为交互式知识图谱，支持 Claude Code/Copilot 等多 Agent

💻 **academic-research-skills** ⭐20.6k | ⬆️+11.4k | 面向 Claude Code 的学术研究工作流（研究→写作→评审→修订）

💻 **agentmemory** ⭐17.3k | ⬆️+6.4k | AI Coding Agent 持久化记忆框架，基于真实评测排名第一

💻 **scientific-agent-skills** ⭐25.6k | ⬆️+2.0k | 科研/金融/工程领域即用型 Agent Skill 合集

💻 **RuView** ⭐65.4k | ⬆️+6.5k | WiFi 信号转空间智能与生命体征监测，无需摄像头

💻 **CLI-Anything** ⭐40.1k | ⬆️+4.8k | 让所有软件具备 CLI Agent 原生能力

💻 **ai-engineering-from-scratch** ⭐15.9k | ⬆️+6.9k | 从零学习 AI 工程实战课程

💻 **easy-vibe** ⭐14.5k | ⬆️+2.4k | Datawhale 出品的 Vibe Coding 2026 入门课程

💻 **ai-to-earn** ⭐16.3k | ⬆️+1.8k | AI 变现项目集合

💻 **CloakBrowser** ⭐20.3k | ⬆️+6.9k | 反机器人检测的 Stealth Chromium，替代 Playwright

💻 **oh-my-pi** ⭐7.0k | ⬆️+2.4k | 终端 AI Coding Agent，支持 hash 锚定编辑、LSP、Python、浏览器等

💻 **supertonIC** ⭐10.2k | ⬆️+2.7k | 闪电级端侧多语言 TTS，ONNX 原生运行

💻 **orca** ⭐3.2k | ⬆️+554 | 多 Agent 并行 ADE 平台，支持桌面与移动端

---

## 【arXiv 热点论文（cs.AI）】

📄 **MOSS** — 自主 Agent 源码级自演化系统，通过生产失败证据自动重写 Agent 底层代码，评测分数提升 144%（0.25→0.61），为 Agent 自适应能力开辟新路径。

📄 **TerminalWorld** — 1530 个真实终端任务评测基准，8 个前沿模型最高通过率仅 62.5%，揭示当前 Agent 在真实命令行场景的能力差距。

📄 **HarnessAPI** — Python Skill 优先框架，同一 handler 自动派生 HTTP 端点 + SSE 流 + MCP 工具，减少样板代码 74%，与 Seaf Skill 体系高度相关。

📄 **AtelierEval（ICML 2026）** — 首个 Agent T2I Prompt 能力评测基准，揭示模仿优于规划，建议未来 Prompt 器走图像增强路线。

📄 **LLM-Metrics** — 利用 LLM 参数记忆评估论文学术影响力，为研究影响力评估提供实时、跨学科新范式。

📄 **能力即负债** — 发现更强大 LLM 在尾部风险预测中反而更差，对金融/医疗 Agent 应用有重要警示意义。

---

## 【Seaf 机会点】

💡 **加速 Skill 生态建设**：FastGPT v4.15 beta 已支持 Skill 编辑与 AgentV2 集成，HarnessAPI 论文证明 Skill-First 架构趋势明确。Seaf 应尽快完善 Skill 的定义、发布、版本管理与反向调用机制，打造差异化竞争力。

💡 **Agent 协作能力补齐**：Dify v1.14.0 协作编辑功能上线，Orca 等新锐 ADE 平台押注多 Agent 并行编排。Seaf 三平台协同架构天然适合协作场景，建议加速"多人协同编排"与"Agent 间通信协议"功能落地。

💡 **企业级安全与可观测性**：Dify 本周密集发布安全补丁（v1.14.1/1.14.2），FastGPT 通过 Redis stream 提升异常检测速度。企业客户对安全隔离、日志追溯、MCP 工具 URL 校验需求强烈，Seaf 应持续强化这些工程能力并形成文档化优势。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-05-25*
