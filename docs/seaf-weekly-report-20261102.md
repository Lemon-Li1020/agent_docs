🌐 Seaf 竞品周报 | 2026-11-02（第 45 期）

> 本期聚焦：ToC 助手集体冲刺「实时语音 / 多模态 / 长上下文」，ToB 工厂加速「智能体路由 + 可移植应用 + 沙盒配额治理」。Agent Skills 生态在 GitHub Trending 全面霸榜。

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动 · 火山方舟）** — 多模态矩阵持续扩容：图像侧上线 Doubao Seedream 5.0 pro / flash 并支持交互式编辑，视频侧推进 Seedance 2.5（含提示词指南与 2.0 系列教程），同时补齐 3D 生成、GUI Agent 与 Managed Agents 能力；平台侧托管 DeepSeek-V4.1-Flash（1017 升级版），强化「一站式模型货架」定位。

📌 **通义千问（阿里 · 百炼 / Qwen）** — 10/27 发布实时双工语音模型 qwen-audio-3.1-realtime-flash（26 万上下文、支持工具调用/联网搜索/声音复刻）；10/22 接入 PixVerse V6 文生视频 / 图生视频；同期上架蚂蚁数科 Ling-3.1-flash（约 560B 总参数、25B 激活、1M 上下文）；3D 生成侧一次性引入 Tripo 全套（文生 3D、贴图、分割、网格补全、重拓扑）。

📌 **Kimi（月之暗面）** — 旗舰模型 Kimi K3.1 Pro 正式发布（普速版 + 高速版），主打 1M token 超长上下文与原生视觉理解，重点强化代码、3D 创作、金融研究与建模；同步在 API 开放平台完善思考模型、上下文缓存、动态加载工具与 MCP 调试，编程 Agent 场景（Kimi Code / Codex / Claude Code）适配持续加码。

📌 **DeepSeek（深度求索）** — 主推模型升级为 DeepSeek-V4.1-Flash-1017（旧版 deepseek-v4-flash / vision-exp 已退役，请求自动由新模型承接、按 Flash 价格计费）；官方文档新增 DeepSeek Harness 及 Claude Code / Codex / OpenClaw 等一批 Agent 集成教程，明显向「Agent 友好型 API」倾斜。

📌 **ChatGPT（OpenAI）** — 近一周以治理与生态为主：更新 Model Spec（10/29）、发布青少年安全社区报告与新保护措施（10/30）、上线网站表达 AI 训练偏好的工具（10/30）、披露前沿模型失准检测方法（10/29）；企业侧宣布与 ServiceNow 扩大合作、把 Oracle 应用接入 ChatGPT（10/27）。

---

## 【ToB 智能体工厂】

📌 **Dify — v1.18.0（2026-10-23）**
- **Agent Output Routes**：让 Agent 自主选择工作流下一分支（条件路由 + 只读 switch 输出），实现「直接解决 / 升级专家」式编排；Agent v2 节点支持流式输出。
- **Portable Apps（.ifpkg）**：工作流/对话流可打包内联 Agent、Skill 及其文件，导入时自动重建并重映射引用，迁移更省心。
- **更深的运行可见性**：嵌套工作流运行可视化增强；新增 OpenAPI 与 difyctl CLI，命令行建管应用。
- **Agent Knowledge Base（可选体验）**：Agent 可挂载知识库检索。
- 升级注意：API/worker/Agent Backend/Runtime 镜像需同升，源码部署需 Python 3.13，本地沙盒需非空鉴权 token。
- 🔗 https://github.com/langgenius/dify/releases/tag/1.18.0

📌 **FastGPT — v4.17.3（2026-11-01）**
- **知识库训练链路重构（延续 4.17.2）**：解析完成即落库为可见数据行，全流程绑定唯一 dataId，杜绝「长训练无数据 / 训练中断孤儿数据」；新增 parsed→indexing→indexed 三态流转，待索引数据检索层天然隔离。
- **Agent 沙盒配额治理**：AGENT_SANDBOX_MAX（默认 100，会话与技能编辑共用）+ 新增 AGENT_SANDBOX_MAX_PER_TEAM 单团队上限；OpenSandbox 新增 CPU/内存 overcommit 系数（K8s + Server≥v0.2.1 生效）。
- **运维/兼容**：应用市场默认地址迁移至 v3.marketplace.fastgpt.cn；移除 DEFAULT_ROOT_PSW（新 root 首登强改密）；多个回填迁移脚本（沙盒团队归属、目录祖先路径、模型价格百万单位）。
- 🔗 https://github.com/labring/FastGPT/releases/tag/v4.17.3

---

## 【GitHub Trending AI 类 · 本周】

💻 **obra/superpowers** ⭐310,633 | ⬆️ +5,896 | Agentic Skills 框架与软件开发方法论
💻 **affaan-m/ECC** ⭐294,802 | ⬆️ +6,299 | Agent harness 性能优化系统（技能/记忆/安全/研究）
💻 **multica-ai/andrej-karpathy-skills** ⭐227,990 | ⬆️ +4,459 | 一份 CLAUDE.md 改善 Claude Code 行为
💻 **anthropics/skills** ⭐186,362 | ⬆️ +2,600 | Anthropic 官方 Agent Skills 公共仓库
💻 **TauricResearch/TradingAgents** ⭐119,528 | ⬆️ +5,432 | 多智能体 LLM 金融交易框架
💻 **thedotmack/claude-mem** ⭐109,250 | ⬆️ +5,852 | 跨会话持久上下文记忆
💻 **Leonxlnx/taste-skill** ⭐107,776 | ⬆️ +5,336 | 给编码 Agent 注入「审美」的技能集
💻 **pbakaus/impeccable** ⭐99,315 | ⬆️ +12,017 | 面向编码 Agent 的设计词汇/审查技能
💻 **cloudflare/security-audit-skill** ⭐56,365 | ⬆️ +10,069 | 多阶段安全审计编码 Agent 技能
💻 **Nutlope/hallmark** ⭐44,863 | ⬆️ +11,566 | 反「AI 味」设计技能（Claude Code/Cursor/Codex）
💻 **AgriciDaniel/claude-seo** ⭐25,533 | ⬆️ +5,034 | 通用 SEO 技能（26 子技能 + 19 子 Agent）

> 观察：本周 Trending 前列几乎被「Agent Skills / Claude Code 生态」占据，且方向从「炫技」转向「设计审美、安全审计、记忆、SEO」等可落地专业场景。

---

## 【前沿论文速览 · arXiv cs.AI】

📄 Collaborative AI agents for autonomous experimental research（2610.40589）
📄 Retrieval as Traversal: Value-Indexed Memory for Stateful Long-Context Agents（2610.40545）
📄 Prefix Executability: Evaluating Tool-Using Agents Beyond Final Success（2610.40444）
📄 EpiAgent: Epistemic Self-Play for LLM Agents（2610.40227）
📄 Locating and Closing Information Gaps in Multi-Agent Systems（2610.40186）
📄 Long-Term Agent Memory through Complementary Curation and Consolidation（2610.39790）
📄 EnvOS: Auditing Computer-Use Agents When the World Moves On（2610.40246）
📄 DynaRev: Benchmarking Web Agents under Dynamic Goal Revision（2610.40133）

> 趋势：Agent 记忆（value-indexed / 长期记忆整理）、工具调用执行性评估、多智能体信息差修补、CUA 审计与动态目标基准是本周研究热点。

---

## 【Seaf 机会点】

💡 **1｜补齐「Agent 可移植与自主路由」能力对标 Dify**
Dify 1.18 的 .ifpkg 一键打包迁移 + Output Routes 自主分支，正击中企业「一次编排、多环境复用、复杂分流」的痛点。Seaf 三平台协同（开发/用户/管理）若能在导出导入时完整携带 Agent/Skill/知识库引用并自动重映射，将形成比 Dify 更完整的「企业交付闭环」，建议优先规划「应用包/资产包」能力。

💡 **2｜把握 Agent Skills 生态红利，做「技能市场 + 审核治理」差异化**
Trending 本周几乎全是 Skills 仓库，但开源形态普遍缺乏企业级治理。Seaf 已有 MCP/Skill 发布-审核-下架流程，建议顺势推出「企业技能/插件市场」：统一版本、权限、审计、复用度统计，把散落的开源技能沉淀为可治理资产，直击 Dify/FastGPT 尚未强化的治理短板。

💡 **3｜资源配额与运行可观测性是企业级刚需，可做成卖点**
FastGPT 4.17.3 花大力气做沙盒配额（单团队上限、overcommit）与训练链路治理，说明「多租户资源管控 + 数据一致性」是 ToB 客户真实痛点。Seaf 已有调用日志 + 回放 + Langfuse 执行链，建议叠加「按团队/智能体的沙盒与 Token 配额 + 成本看板」，把可观测性从「排障」升级为「成本与治理」双价值。

---
*数据来源：GitHub Releases（Dify / FastGPT）/ GitHub Trending（weekly）/ arXiv cs.AI / OpenAI News / 阿里云百炼 & 火山方舟 & Kimi 官方文档 | 2026-11-02*
