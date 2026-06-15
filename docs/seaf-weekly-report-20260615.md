# 🌐 Seaf 竞品周报 | 2026-06-15（第 24 期）

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动）** — 持续强化多模态能力，豆包电脑版新增屏幕理解与自动化操作功能，支持复杂工作场景下的 Agent 交互；AI 搜索体验进一步优化。

📌 **通义千问（阿里）** — 通义万相 2.1 上线，支持更高分辨率图像生成；Qwen3 系列开源模型持续迭代，工具调用与 Agent 能力成为核心迭代方向。

📌 **Kimi（月之暗面）** — Kimi 推出浏览器插件版，支持网页内容摘要与问答；长上下文窗口仍是核心卖点，支持百万 token 无损上下文。

📌 **DeepSeek** — DeepSeek-V3.1 版本传闻即将发布，代码生成与推理能力持续提升；DeepSeek-Coder 系列继续保持开源竞争力。

📌 **ChatGPT（OpenAI）** — GPT-4o 语音模式全面开放，实时对话能力增强；OpenAI 宣布 GPT-5 训练进展顺利，多模态理解能力大幅提升。

📌 **Claude（Anthropic）** — Claude 3.7 Sonnet 正式发布，扩展上下文至 200K，Agent 模式（Computer Use）正式公测，支持自动化浏览器操作。

📌 **Gemini（Google）** — Gemini 2.0 Flash 实验版本上线，推理速度提升 2 倍；Google DeepMind 发布 Gemini 家族新成员，支持原生工具调用。

---

## 【ToB 智能体工厂】

📌 **Dify** — 发布 v1.14.2 安全补丁版本，强化租户隔离与工具凭证安全，修复工作流执行、HITL 恢复、RAG 管道等多项稳定性问题，重点提升企业级部署安全性。
  - GitHub: https://github.com/langgenius/dify/releases

📌 **FastGPT** — 发布 v4.15.0-beta4，重写插件系统架构（迁移至 pnpm workspace monorepo），重写 Chatbox UI，新增虚拟列表渲染优化性能，PDF 解析替换为 liteparse 提速 3 倍，系统工具迁移至 local-pool 进程池，大幅提升插件运行稳定性与安全性。
  - GitHub: https://github.com/labring/fastgpt/releases

📌 **Coze（扣子）** — 持续迭代 Bot Store 与工作流编排能力，MCP 插件支持进一步完善，海外版 Coze 拓展企业级市场。

📌 **LangFlow** — 开源 LangFlow 项目持续活跃，聚焦可视化 LangChain 工作流编排，版本迭代稳定。

---

## 【GitHub Trending AI 类】

💻 **[last30days-skill](https://github.com/mvanhorn/last30days-skill)** ⭐ 41,992 | ⬆️ +12,053 本周 | AI agent skill，可跨 Reddit/X/YouTube/HN/Polymarket/Web 搜索并综合总结任意话题

💻 **[headroom](https://github.com/chopratejas/headroom)** ⭐ 27,563 | ⬆️ +10,653 本周 | 压缩 LLM 输入 token（工具输出/日志/RAG chunks），节省 60-95% token 同时保持答案质量，支持 MCP server

💻 **[SkillSpector](https://github.com/NVIDIA/SkillSpector)** ⭐ 5,271 | ⬆️ +3,669 本周 | NVIDIA 出品的 AI agent skill 安全扫描工具，检测漏洞与恶意模式

💻 **[agent-skills](https://github.com/addyosmani/agent-skills)** ⭐ 59,464 | ⬆️ +10,445 本周 | Google 出品的 AI 编码 agent 工程化技能集，含 100+ 生产级 skill

💻 **[Agent-Reach](https://github.com/Panniantong/Agent-Reach)** ⭐ 28,733 | ⬆️ +5,468 本周 | 让 AI agent 能"看见"全网，支持 Twitter/Reddit/YouTube/GitHub/小红书等平台搜索，无 API 费用

💻 **[taste-skill](https://github.com/Leonxlnx/taste-skill)** ⭐ 43,685 | ⬆️ +7,591 本周 | 提升 AI 生成质量的 skill，避免无聊/通用/俗套输出

💻 **[goose](https://github.com/aaif-goose/goose)** ⭐ 49,374 | ⬆️ +2,165 本周 | 开源可扩展 AI agent（Rust），超越代码建议，支持安装/执行/编辑/测试任意 LLM

💻 **[graphify](https://github.com/safishamsi/graphify)** ⭐ 67,148 | ⬆️ +5,478 本周 | 将代码库/SQL/RAG/文档/视频等转化为可查询知识图谱，支持 Claude Code/Codex/Cursor 等

💻 **[open-notebook](https://github.com/lfnovo/open-notebook)** ⭐ 30,525 | ⬆️ +3,468 本周 | 开源 NotebookLM 实现，功能更灵活，支持播客/视频/文档总结

💻 **[Supervision](https://github.com/roboflow/supervision)** ⭐ 44,193 | ⬆️ +3,315 本周 | 计算机视觉工具库，AI agent 视觉理解场景必备

---

## 【Seaf 机会点】

💡 **Agent Skill 安全将成为刚需**：NVIDIA SkillSpector 的火爆（周增 3.6k⭐）说明 skill 安全审计是市场空白。Seaf 的 MCP/Skill 审核流程可强化安全扫描能力（如恶意代码检测、越权风险检测），将其作为差异化卖点向企业客户推广。

💡 **Token 压缩工具（headroom）值得集成**：LLM 输入压缩赛道快速崛起，Seaf 可考虑在工作流编排中引入 token 优化层（工具输出压缩/历史摘要），既能降低用户成本，也能提升调用效率，契合企业级需求。

💡 **AI Agent 原生知识管理**：open-notebook（NotebookLM 开源替代）和 graphify（知识图谱）等项目的热度反映用户对"让 AI 真正理解我的数据"的强烈需求。Seaf 可强化知识库模块的语义理解深度，支持多模态知识解析与知识图谱构建，形成与 Dify/FastGPT 的体验差异。

💡 **PDF/文档解析性能优化参照**：FastGPT 将 PDF 解析速度提升 3 倍（liteparse 替换 PDF.js），说明解析性能是企业用户的核心痛点。Seaf 应评估当前文档解析效率，考虑升级解析引擎或引入流式解析。

---

## 【arXiv cs.AI 本周热点】

本周 cs.AI 分类新增 222 篇论文（截至 6月12日），热门方向集中在：
- **Agent Planning & Reasoning**：多步骤任务规划、长程推理、安全约束下的 agent 决策
- **LLM Evaluation**：多模态 LLM 评估框架、Agent 性能评测标准
- **MCP & Tool Use**：模型上下文协议扩展、工具调用可靠性
- **RAG & Knowledge**：检索增强生成的最新进展、幻觉检测与缓解

---

*数据来源：GitHub Releases / Trending / 公开报道 | 2026-06-15*
