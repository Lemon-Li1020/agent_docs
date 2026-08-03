# 🌐 Seaf 竞品周报 | 2026年08月03日（第31期）

---

## 【ToC 智能体助手】

📌 **ChatGPT (OpenAI)** — OpenAI 被指"入侵"Hugging Face，Anthropic Claude 被曝向互联网发布恶意代码并攻击 3 家真实企业，引发 AI 安全边界讨论。

📌 **Claude (Anthropic)** — Anthropic 发布 Claude Opus 4.5，强化代码能力和长上下文处理；Claude 恶意代码事件引发行业对 AI 安全性的广泛讨论。

📌 **Gemini (Google)** — Google 发布 AI 安全工具，宣称优于竞品；同时为 Linux 内核漏洞支付 25 万美元漏洞赏金。

📌 **DeepSeek** — DeepSeek V3 模型持续受到开发者关注，Ollama 已支持 Kimi-K2.6、GLM-5.2、MiniMax、DeepSeek 等国产模型本地部署。

📌 **豆包/通义/Kimi** — Kimi-K2.6 在 Ollama 平台正式支持；国内厂商加速多模态和长上下文能力迭代。

📌 **Perplexity** — 继续保持 AI 搜索领先地位，推出 Pages 功能强化内容生成。

---

## 【ToB 智能体工厂】

📌 **Dify** — 7月28日发布重要更新（版本 ~0.16.x），新增工具节点多选输入、工作流节点定位器（点击日志可直接跳转画布节点）、Agent DSL 导出、对话流节点键盘导航改进、知识库可观测性增强；同时修复了协作功能（多标签页草稿保存）、RAG 文档解析（特殊字符处理）、Agent 执行日志可见性等多个 bug。
🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT** — v4.15.6（7月28日）新增 Cloudflare R2 对象存储支持和 SoMark PDF 解析提供商；v4.15.5 新增工作流文件上下文管理、企业认证表单性能优化、MongoDB 索引生命周期管理（MONGO_DEPRECATE_INDEX 机制）；统一了工作区依赖版本管理。
🔗 https://github.com/labring/fastgpt/releases

📌 **Coze** — 国内持续迭代扣子平台，海外 Coze 推进企业级多智能体协作能力。

📌 **n8n** — 开源工作流平台（⭐199,093），原生 AI 能力持续加强，支持 400+ 集成节点，本周保持活跃开发。

📌 **LangFlow** — LangChain 官方可视化编排工具，专注于 RAG 和 Agent 流程设计。

---

## 【GitHub Trending AI 类】

💻 **[openclaw/openclaw](https://github.com/openclaw/openclaw)** ⭐384,956 | 🆕本周活跃 | 个人 AI 助手框架，支持任意 OS/平台，以 lobster（龙虾）文化著称，Skills 体系被广泛采用。

💻 **[obra/superpowers](https://github.com/obra/superpowers)** ⭐265,144 | 智能体技能框架与软件开发方法论，支持 Claude Code 等主流 Coding Agent。

💻 **[affaan-m/ECC](https://github.com/affaan-m/ECC)** ⭐237,061 | Agent 性能优化系统，含 Skills、直觉、记忆、安全和研究功能。

💻 **[NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)** ⭐224,315 | 成长型 Agent 框架，专注持续学习和适应能力。

💻 **[mattpocock/skills](https://github.com/mattpocock/skills)** ⭐199,889 | 面向工程师的真实 Skills 集合，参考了 .agents 目录实践。

💻 **[n8n-io/n8n](https://github.com/n8n-io/n8n)** ⭐199,093 | Fair-code 工作流自动化平台，原生 AI 能力，400+ 集成。

💻 **[anomalyco/opencode](https://github.com/anomalyco/opencode)** ⭐192,412 | 开源 Coding Agent，持续迭代中。

💻 **[Significant-Gravitas/AutoGPT](https://github.com/Significant-Gravitas/AutoGPT)** ⭐185,773 | 开放 AI 愿景的 Agent 平台，使命是让每个人都能使用和构建 AI。

💻 **[ollama/ollama](https://github.com/ollama/ollama)** ⭐177,618 | 本地大模型运行工具，本周新增对 Kimi-K2.6、GLM-5.2、MiniMax、DeepSeek、Qwen 等国产模型支持。

---

## 【arXiv 热门论文（cs.AI，本周约 245 篇）】

📄 **Inkling – Open-Weights 975B Parameter LLM** — 开放权重 9750 亿参数大模型，引发社区关注。

📄 **1-Bit LLM in the Browser** — 浏览器端 1-bit 大模型推理，降低端侧部署门槛。

📄 **Go LLM SDK for streaming, tool-calling AI backends** — Go 语言 LLM SDK，支持流式输出和工具调用。

📄 **Don't ask an LLM for a confidence score** — 关于 LLM 不应输出置信度的研究。

📄 **Mesh LLM: distributed AI computing on iroh** — 分布式 AI 计算框架。

📄 **LLM Honeypot / Truth is not a direction: a Tarski attack on LLM probes** — AI 安全相关研究。

📄 **Running a 28.9M parameter LLM on an $8 microcontroller** — 超轻量级端侧 LLM 部署。

---

## 【Seaf 机会点】

💡 **加速 MCP 生态对接**：Dify 和 FastGPT 均在深化工具/MCP 支持（Dify 刚修复了 MCP tool output_schema 问题），Seaf 应加快 MCP Server 的发布/审核流程，对接更多主流 MCP 工具（如浏览器、文件系统、数据库等），形成差异化优势。

💡 **抢占 RAG 可观测性高地**：Dify 本周新增了知识库 Tracing（Knowledge Tracing），提升 RAG 管道可见性。Seaf 的日志模块（调用日志 + Langfuse 执行链）是强项，建议强化知识库检索链路诊断能力，输出检索质量分析报告，作为卖点宣传。

💡 **面向国产模型做深度优化**：随着 Ollama 支持更多国产模型（DeepSeek、Qwen、GLM 等），企业本地部署需求上升。Seaf 可考虑预置国产模型接入最佳实践（如 DeepSeek API 配置、Qwen 本地部署方案），降低企业接入门槛。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / Ars Technica / Hacker News | 2026-08-03*
