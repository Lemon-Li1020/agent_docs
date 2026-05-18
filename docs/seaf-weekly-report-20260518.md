# 🌐 Seaf 竞品周报 | 2026-05-18（第21期）

---

## 【ToC 智能体助手】

- **ChatGPT** — OpenAI 发布 GPT-4o 更新，上下文理解能力进一步提升，多模态交互更流畅
- **Claude** — Anthropic 强化 Claude Code 能力，新增更长的执行上下文窗口，支持复杂项目级别的代码重构
- **Gemini** — Google 发布 Gemini 2.5 Flash，主打低成本高速推理，上下文窗口达 1M token
- **DeepSeek** — DeepSeek V3 微调版本上线，数学和代码能力小幅提升；终端工具 DeepSeek-TUI 登上 GitHub 周Trending 第4位，本周 7,444 stars
- **豆包*  — 孕节跳动豆包更新多agent协作能力，支持更复杂的工作流编排与跨应用调用
- **通义千问** — 阿里云通义更新视觉理解模块，图像理解准确率提升，上下文长度扩展至 128K
- **Kimi** — 月之暗面 Kimi 发布长文档处理优化，PDF/Word 解析速度提升 40%，支持更长的上下文
- **Perplexity** — Perplexity 推出 Pages 功能，AI 搜索结果可一键生成结构化报告并发布分享

---

## 【ToB 智能体工厂】

📌 **Dify** — v1.14.1 安全补丁版，重点修复 SECRET_KEY 硬编码漏洞、内部指标接口暴露、IDOR 权限问题，升级 LiteLLM 修复 CVE-2026-42208；工作流编辑器继续迁移至新 UI 组件库，Dify UI 组件覆盖范围进一步扩大
  - 🔗 https://github.com/langgenius/dify/releases/tag/v1.14.1

📌 **FastGPT** — v4.14.20 发布，正式引入**循环（Loop）节点**，替代旧的批量执行功能，支持 start/break 子节点；新增模型思考配置、S3 CDN 支持、钉钉知识库接入；加强 SSRF 防护和 codex-sandbox AST 安全检查；升级 Next.js 至最新版本，切换至 Turbopack 构建
  - 🔗 https://github.com/labring/FastGPT/releases/tag/v4.14.20

📌 **Coze** — 字节 Coze 国内版持续优化 Bot Store 生态，新增多个行业模板和工作流组件，MCP 插件市场热度上升

📌 **LangFlow** — 开源 LangFlow 推出新版可视化编排界面，拖拽式 DAG 编辑器体验改善，Python API 集成能力增强

---

## 【GitHub Trending AI 类】

💻 **[agentmemory](https://github.com/rohitg00/agentmemory)** ⭐ 11,279 | ⬆️ +7,103 本周 | 为 AI Coding Agent 提供持久化记忆，基于真实世界基准测试优化

💻 **[DeepSeek-TUI](https://github.com/Hmbown/DeepSeek-TUI)** ⭐ 31,235 | ⬆️ +7,444 本周 | 面向 DeepSeek 模型的终端 Coding Agent，Rust 实现

💻 **[academic-research-skills](https://github.com/Imbad0202/academic-research-skills)** ⭐ 9,312 | ⬆️ +3,624 本周 | 为 Claude Code 提供学术研究能力：研究→写作→审稿→修订全流程

💻 **[AI-Trader](https://github.com/HKUDS/AI-Trader)** ⭐ 17,872 | ⬆️ +2,499 本周 | "100% 全自动 Agent 原生交易系统"，港大团队出品

💻 **[UI-TARS-desktop](https://github.com/bytedance/UI-TARS-desktop)** ⭐ 34,411 | ⬆️ +2,563 本周 | 孕节开源多模态 AI Agent 平台，连接前沿 AI 模型与 Agent 基础设施

💻 **[react-doctor](https://github.com/millionco/react-doctor)** ⭐ 9,947 | ⬆️ +2,430 本周 | AI Agent 写出劣质 React 代码？自动检测并修复

💻 **[9router](https://github.com/decolua/9router)** ⭐ 11,599 | ⬆️ +4,458 本周 | 连接 Claude Code/Codex/Cursor 等接入 40+ 免费 AI 提供商，自动降级

---

## 【arXiv 热点论文】（cs.AI，5月11-15日）

📄 **OpenDeepThink** — 通过 Bradley-Terry 聚合实现并行推理，在 8 轮 LLM 调用内将 Gemini 3.1 Pro 的 Codeforces Elo 提升 405 分，发布 CF-73 高质量代码推理数据集

📄 **CAST（Case-Based Calibration）** — 基于历史执行轨迹的案例驱动框架，实现 LLM 工具调用的自适应推理，执行准确率提升 5.85pp，推理长度减少 26%

📄 **Learning Developmental Scaffoldings** — 借鉴生物发育机制，研究如何通过初始条件引导自组织过程，揭示 AI Agent 中记忆-计算权衡的新思路

---

## 【Seaf 机会点】

💡 **1. 跟进循环节点能力** — FastGPT v4.14.20 正式弃用旧批量执行、引入 Loop 节点，Seaf 应考虑在编排 Tab 中快速跟进类似能力（循环/条件分支/break），尤其对复杂业务流场景至关重要

💡 **2. MCP 插件安全审核** — Dify 和 FastGPT 本周均在 MCP 工具 URL 验证和 SSRF 防护上修了安全问题，Seaf 的 MCP 发布/下架/审核流程应内置 URL 白名单和 SSRF 检测机制

💡 **3. Coding Agent + 记忆层** — GitHub d�� agentmemory 类持久化记忆项目热度极高（7k+ stars/周），Seaf 可探索在日志回放/Langfuse 执行链基础上构建 Agent 记忆层，支持跨会话上下文复用

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-05-18*
