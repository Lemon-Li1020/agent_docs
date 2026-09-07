# 🌐 Seaf 竞品周报 | 2026-09-07（第3期）

---

## 【ToC 智能体助手】

📌 **豆包（ByteDance）** — 豆包电脑版持续迭代多模态能力，新增 AI 写作辅助与代码解释功能，在中文理解任务上持续对标 GPT-4o。

📌 **通义千问（阿里云）** — Qwen2.5 系列持续开源更新，Qwen2.5-Coder 在代码 Agent 领域热度不减，社区涌现大量基于 Qwen 的垂直 Agent 项目。

📌 **Kimi（月之暗面）** — Kimi 开放平台新增长文档解析 API，支持百万字级上下文窗口，深度集成知识库检索增强能力。

📌 **DeepSeek** — DeepSeek-V3 及 DeepSeek-Coder 系列持续霸榜开源模型榜单，API 价格优势明显，正快速渗透 Agent 开发市场。

📌 **ChatGPT（OpenAI）** — OpenAI 发布 o1-preview 稳定版并开放 Agents SDK，引入内置工具调用与循环控制能力，正式入局 AI Agent 开发框架赛道。

---

## 【ToB 智能体工厂】

📌 **Dify** — 发布 v1.17.0（[GitHub](https://github.com/langgenius/dify/releases/tag/1.17.0)），重磅推出：
- 🤖 **Agent 技能系统（Skill Management）**：工作区级技能管理，支持 draft→publish→version 生命周期管理，附 Web UI 与文件编辑器
- 🔒 **E2B 云沙箱后端**：Agent 代码执行支持 E2B 云端沙箱，与本地沙箱可切换（DIFY_AGENT_RUNTIME_BACKEND）
- 📸 **Home Snapshots**：Agent 构建时自动捕获完整文件系统状态（含依赖包与工作文件），发布后 Agent 从快照恢复，保证每次运行状态一致
- 🧠 **上下文压缩**：长对话自动 tiered compaction（先清理旧工具结果→再摘要历史），确保不超过模型 context window
- 🔗 **可复用 LLM 环境变量**：工作流中定义共享的 provider/model/parameters，一次修改全局生效
- 👤 **Human-in-the-Loop**：Loop/Iteration 节点内支持人工审批/表单介入

📌 **FastGPT** — 发布 v4.16.2（[GitHub](https://github.com/labring/fastgpt/releases/tag/v4.16.2)），重点更新：
- ⚙️ **Worker 并发自动检测**：移除手动 PARSE_FILE_WORKERS 等配置，改为根据 CPU 核心数自动设置
- 🇰🇷 **新增韩语支持**
- 📄 **Milvus BM25 全文检索**：使用 Milvus 时自动启用 BM25 全文搜索（需 Milvus ≥ 2.5.16）
- 📎 **文档解析大扩展**：新增 DOC/WPS/PPT/XLS/DOCM/PPTM/EPUB 等 16 种格式，内嵌图片自动提取
- 🔧 **全节点工具调用**：所有节点均支持工具调用，优化工具配置 UI 与版本选择体验

---

## 【GitHub Trending AI 类】

> 本周（2026-09-01 ~ 2026-09-07）GitHub 周榜 AI 相关热门项目

💻 **[affaan-m/ECC](https://github.com/affaan-m/ECC)** ⭐251.3k | ⬆️+6,394/wk | Agent 性能优化系统，含 Skill/Memory/Security，为 Claude Code/Codex/Cursor 等提供增强框架

💻 **[DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail)** ⭐129.3k | ⬆️+12,186/wk | "让 AI Agent 像最懒的高级工程师一样思考"——代码精简哲学，12k stars 本周爆发

💻 **[jingyaogong/minimind](https://github.com/jingyaogong/minimind)** ⭐59.1k | ⬆️+3,816/wk | 从零训练 64M 参数 LLM 仅需 2 小时，教育向 LLM 训练框架

💻 **[ChromeDevTools/chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp)** ⭐51.2k | ⬆️+965/wk | Chrome DevTools for Coding Agents，为 AI 编程 Agent 提供浏览器自动化能力

💻 **[tt-a1i/archify](https://github.com/tt-a1i/archify)** ⭐50.8k | ⬆️+17,190/wk | Agent 技能：生成架构图/工作流图/序列图/数据流图，自包含 HTML+动画导出

💻 **[K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)** ⭐43.3k | ⬆️+4,718/wk | AI Scientist 技能库，190k+ 科学家使用，含 165+ 验证技能 + 100+ 科学数据库

💻 **[Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)** ⭐46.6k | ⬆️+2,334/wk | 学术研究 Agent 技能：研究→写作→评审→修订→定稿全流程

💻 **[magnitudedev/magnitude](https://github.com/magnitudedev/magnitude)** ⭐3.7k | ⬆️+1,961/wk | 开源本地推理服务器，为 OpenClaw/Codex/Claude Code 等提供本地模型支持

💻 **[THU-MAIC/OpenMAIC](https://github.com/THU-MAIC/OpenMAIC)** ⭐32.4k | ⬆️+9,193/wk | 清华多智能体互动课堂，一键沉浸式多 Agent 学习体验

💻 **[Gitlawb/openclaude](https://github.com/Gitlawb/openclaude)** ⭐32.8k | ⬆️+1,944/wk | 任意环境运行、使用任意模型的开源 OpenClaude 分支

💻 **[every-app/open-seo](https://github.com/every-app/open-seo)** ⭐17.5k | ⬆️+2,503/wk | 开源 Semrush/Ahrefs 替代品，SEO 分析 Agent

💻 **[debpalash/VoiceStudio](https://github.com/debpalash/VoiceStudio)** ⭐19.8k | ⬆️+7,513/wk | 开源 ElevenLabs 替代方案，支持 646 种语言语音克隆/视频配音/听写

---

## 【arXiv 热门论文】（cs.AI 本周）

- 📄 **ACLE-MCP**（arXiv:2609.04177）：Attested Capability Leases for Execution-Time Trust in Remote LLM Tool Use——远程 MCP 服务的可信执行时信任协议，9月2日提交
- 📄 **Interface-Induced Trajectory Censoring**（arXiv:2609.03966）：揭示 BFCL v4 测试中服务器解析器静默丢弃 Agent 工具调用轨迹的现象，0.00 vs 0.96 仅因 adapter 差异；发布 98 行 preflight check 开源工具
- 📄 **Harness Engineering**（arXiv:2609.03973）：解剖 11 个 Coding Agent 的 Harness（运行时框架）架构，源码级研究
- 📄 **Clean Engineering, Unstable Measurement**（arXiv:2609.04198）：LLM 评测的可靠性危机——52,988 次评测证明共享端点上"同一模型名"不是稳定测量仪器，发布 8 条设计规则

---

## 【Seaf 机会点】

💡 **1. 加速 Skill/MCP 生态建设**：Dify v1.17.0 已推出正式 Skill 管理系统，FastGPT v4.16.2 全节点工具调用完成。Seaf 应加快 MCP Server 接入与 Skill 商店能力，差异化可聚焦垂直场景（如专利、代码、科学研究），参考 scientific-agent-skills 的 165 技能打法。

💡 **2. 重视 Agent 可观测性**：arXiv 论文反复证明"同一模型名在不同接口上表现差异巨大"（工具调用率 0% vs 96%），Seaf 应在内置 tracing、可视化日志、工具调用审计上发力，做成产品卖点而非运维负担。

💡 **3. 关注"懒人哲学"的产品化**：ponytail（"让 AI 像最懒的高级工程师"）本周 12k stars 爆发式增长，archify 生成架构图 17k stars。Seaf Agent 可考虑内置"最小化输出/代码优先拒绝"类策略，或提供"简洁模式"开关，迎合开发者社区对 Agent"不废话"的需求。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI | 2026-09-07*
