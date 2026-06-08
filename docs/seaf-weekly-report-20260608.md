# 🌐 Seaf 竞品周报 | 2026-06-08（第 24 期）

> 统计周期：2026-06-01 ~ 2026-06-07 | 生成时间：2026-06-08 08:30

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动）** — 多模态模型持续迭代，豆包网页版与移动端强化了视频理解与实时搜索能力，端到端响应速度进一步优化。

📌 **通义千问（阿里云）** — Qwen3 系列开源后生态快速扩张，Qwen-Agent 框架新增 MCP 协议支持与批量任务编排能力，配套文档与示例完善。

📌 **Kimi（月之暗面）** — Kimi 开放平台新增长文本摘要 API，支持 100 万字无损上下文，企业级用例（法律文档分析、研报处理）场景进一步拓展。

📌 **DeepSeek** — DeepSeek-Coder-V2 开源代码能力逼近 GPT-4-Turbo，DeepSeek-V2.5 在数学推理与中文理解榜单上持续领先，API 价格优势保持。

📌 **ChatGPT（OpenAI）** — GPT-4o 语音交互全面开放，移动端支持实时屏幕共享与视觉推理，ChatGPT Mac 版集成桌面应用生态。

📌 **文心一言（百度）** — 文心 4.0 Turbo 正式商用，ERNIE Agent 平台支持多工具编排与知识库 RAG，企业定制化能力增强。

📌 **智谱 GLM（清华智谱）** — GLM-4V 发布视觉语言模型，CodeGeex 代码助手新增多语言实时翻译与项目级代码理解能力。

---

## 【ToB 智能体工厂】

📌 **Dify** — v1.14.2（2026-05-19）补丁版本发布，聚焦安全加固（多租户隔离、工具凭证权限管控）、工作流执行可靠性、RAG 文档处理优化及 UI 组件迁移至 @langgenius/dify-ui。
🔗 https://github.com/langgenius/dify/releases/tag/v1.14.2

📌 **FastGPT** — v4.15.0-beta3（2026-05-28）Beta 版发布，支持多模态模型音视频输入、新增 Skill 编辑与 AgentV2 Skill 调用、重写 Agent V2 线性 messages loop、Code Sandbox 新增多项安全环境变量与 queueId 并发排队机制。
🔗 https://github.com/labring/FastGPT/releases/tag/v4.15.0-beta3

📌 **Coze / 扣子（字节）** — Bot Store 插件生态持续扩张，支持更多第三方工具接入，工作流节点类型进一步丰富。

📌 **Dify 社区趋势** — GitHub Star 突破 75k，近一月增长约 3k，贡献者活跃度高，插件市场（MCP Server 集成）成为新亮点。

---

## 【GitHub Trending AI 类】🔥 本周（2026-06-01 ~ 2026-06-07）

| 仓库 | ⭐ 总星 | 📈 本周新增 | 简介 |
|------|--------|-----------|------|
| NousResearch/hermes-agent | 185.9k | +11.4k | 通用 Agent 框架，支持自我进化与工具调用 |
| affaan-m/ECC | 209.8k | +10.2k | Agent 性能优化系统，含 Skill/Memory/Security 模块 |
| microsoft/markitdown | 147.3k | +13.4k | 文档转 Markdown 工具，支持 Office 全格式 |
| chopratejas/headroom | 16.9k | +14.3k | LLM 输出压缩工具，减少 60-95% Token 消耗 |
| harry0703/MoneyPrinterTurbo | 81.2k | +8.0k | AI 一键生成高清短视频 |
| open-notebook (lfnovo) | 27.2k | +3.0k | 开源 NotebookLM，支持多语言与自定义功能 |
| Panniantong/Agent-Reach | 23.1k | +2.3k | 让 Agent 操控全网：Twitter/Reddit/YouTube/GitHub 等 |
| last30days-skill (mvanhorn) | 30.9k | +2.7k | Reddit/X/YouTube/HN/Polymarket 研究型 Skill |
| taste-skill (Leonxlnx) | 36.6k | +6.4k | 提升 AI 输出「品味」，避免千篇一律的废话 |
| pbakaus/impeccable | 35.5k | +3.6k | AI 设计语言框架，提升 Agent UI 能力 |
| open-llm-vtuber | 10.3k | +2.4k | 开源 LLM 虚拟主播，支持语音打断与 Live2D |
| revfactory/harness | 6.4k | +2.0k | 专业领域 Agent 团队设计元 Skill |
| nesquena/hermes-webui | 13.8k | +4.3k | Hermes Agent 的 Web 界面 |
| oh-my-pi (can1357) | 11.1k | +2.1k | 终端 AI Coding Agent，含 hash 锚定编辑 |

**本周趋势观察：**
- **Agent 能力层**（ECC、Harness、taste-skill）大热，说明社区对 Agent 框架与 Skill 标准化极度关注
- **输出压缩**（headroom）新晋即爆，减少 Token 成本成为刚需
- **多模态 Agent**（Agent-Reach、Open-LLM-VTuber）显示 Agent 向多模态交互演进的明确方向

---

## 【arXiv 热点论文 · cs.AI】📄 本周精选

| 论文 | 领域 | 摘要 |
|------|------|------|
| **MLEvolve** (`2606.06473`) | Agent / MLE | LLM 驱动的自演化多 Agent 框架，用于自动机器学习算法发现，采用图结构跨分支信息流 |
| **TRACE** (`2606.06285`) | 多模态 / 时序 | 条件估计范式，处理多模态时序模型中的缺失模态与时间对齐问题 |
| **Appropriate Reliance** (`2606.06081`) | HCI / AI | 首个评估人类对集合值 AI 建议的信赖框架，覆盖分类与回归任务 |
| **ProSarc** (`2606.06168`) | 多模态 / 语音 | 仅用音频检测讽刺语气（Interspeech 2026），无需文本信息 |
| **MResOpt** (`2606.06300`) | 优化 / 神经网络 | 多残差网络用于约束优化，支持物理启发的约束优先级排序 |

---

## 【Seaf 机会点】💡

**1. 加速 MCP 协议深度集成**
本周 GitHub Trending 中 Agent 类项目大量涉及 MCP 协议（headroom、ECC 均支持），Dify v1.14 也明确加强了 MCP Server 集成能力。Seaf 应快速推进 MCP 工具生态，优先支持主流工具（如 Filesystem、Git、Browser），形成差异化 Skill 市场。

**2. 借鉴 taste-skill 思路，提升 Agent 输出「人味」**
taste-skill 专门解决 LLM 输出「废话/通用感」问题，当前 Star 36.6k、周增 6.4k，说明用户对 Agent 个性化与输出质量有强烈需求。建议 Seaf 在 Agent 配置中加入「风格/语气」选项，并内置 prompt 优化建议功能。

**3. 布局多模态 Agent 与 RAG 融合**
FastGPT v4.15 支持多模态 embedding + 图搜图，Dify 强化 RAG 管道，TRACE 论文处理多模态缺失问题——三者方向一致：多模态 RAG 是下一个技术高地。Seaf 应在知识库模块优先支持图像/音视频检索，形成技术护城河。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-06-08*
