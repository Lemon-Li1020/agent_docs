# Seaf 竞品周报 | 2026-06-22（第 6 期）

---

## 【ToC 智能体助手】

**📌 豆包** — 豆包 1.2 版本持续迭代，AI 生图与视频能力进一步融入抖音内容生态，语音交互延迟大幅降低，APP 日活保持国内第一。

**📌 Kimi（月之暗面）** — 推出 Kimi 视觉版，支持图片输入分析与多图对比，长上下文分析能力向 200K 窗口扩展，学术场景口碑持续上升。

**📌 DeepSeek** — DeepSeek-V3 开源版继续保持高热，API 调用价格维持行业最低档，吸引大量中小企业和独立开发者迁移。

**📌 通义千问** — 阿里云发布 Qwen3-32B 开源版本，新增 Agent Mode，工具调用和代码执行能力大幅提升，开始渗透开发者市场。

**📌 ChatGPT** — OpenAI 为 ChatGPT 桌面版上线高级语音深度搜索功能，GPT-4o 多模态 API 新增视频理解参数，生态继续扩张。

**📌 Claude** — Anthropic 发布 Claude 3.7 Sonnet，优化长任务多步推理与工具调用稳定性，Claude Code 正式版开放企业授权。

**📌 Gemini** — Google Gemini 2.5 Flash 全面上线 Deep Research，Gemini in Gmail/Docs 集成度再升级，Google Workspace AI 覆盖率超 50%。

**📌 Copilot** — Microsoft Copilot 更新支持 Teams 会议实时摘要与 PPT 自动生成，Windows 11 系统级 AI 入口持续深化。

---

## 【ToB 智能体工厂】

**📌 Dify** — 发布 v1.14.2 安全补丁版，强化多租户隔离、工作流可观测性与 RAG 管道稳定性，修复 30+ 个 issue，Langfuse v3 追踪集成完善。

🔗 https://github.com/langgenius/dify/releases/tag/1.14.2

**📌 FastGPT** — 发布 v4.15.0-beta4，全面重写插件系统架构（pnpm workspace monorepo），新增系统工具进程池、PDF 解析速度提升 3 倍（liteparser），重绘 ChatUI。

🔗 https://github.com/labring/fastgpt/releases/tag/v4.15.0-beta.4

**📌 Coze（扣子）** — Coze 国内版持续完善多 Agent 协作编排能力，快直播/短视频卡片组件更新，企业知识库挂载体验优化。

**📌 LangFlow** — LangChain 发布 v0.3.x 更新，集成更多 MCP 协议支持，可视化流程编辑稳定性提升。

---

## 【GitHub Trending AI 类】

本周 GitHub 周榜涌现多个 Agent/MCP 相关明星项目：

| 仓库 | ⭐ 总星 | 📈 本周增长 | 简介 |
|------|--------|------------|------|
| `chopratejas/headroom` | 44.3k | +16.1k ⬆️ | LLM Token 压缩工具，可减少 60-95% 的工具输出 Token，支持 MCP Server |
| `Panniantong/Agent-Reach` | 36.8k | +8.2k ⬆️ | 为 AI Agent 赋予多平台浏览器能力（Twitter/Reddit/GitHub等），零 API 费用 |
| `DeusData/codebase-memory-mcp` | 10.3k | +6.4k ⬆️ | 高性能代码知识图谱 MCP Server，158 语言支持，毫秒级查询 |
| `addyosmani/agent-skills` | 64.8k | +5.6k ⬆️ | 面向 AI 编码 Agent 的工程化 Skill 合集，涵盖代码审查/测试等 |
| `calesthio/OpenMontage` | 8.7k | +2.9k ⬆️ | 首个开源 Agentic 视频制作系统，12 条 Pipeline、52 工具、500+ Agent 技能 |
| `NVIDIA/SkillSpector` | 9.0k | +4.1k ⬆️ | AI Agent Skill 安全扫描工具，检测漏洞与恶意模式 |
| `LMCache/LMCache` | 9.5k | +0.5k ⬆️ | KV Cache 加速层，为 LLM 推理提速 |
| `withastro/flue` | 6.3k | +1.3k ⬆️ | 沙盒化 Agent 框架，由 Astro 团队开源 |

---

## 【Seaf 机会点】

💡 **强化 MCP 生态集成**：竞品 Dify/FastGPT 持续完善 MCP 支持，本周 `codebase-memory-mcp`（+6.4k star）等高质量 MCP Server 涌现，Seaf 应加快 MCP 工具的导入/发布/审核流程优化，并建立 MCP 工具市场。

💡 **关注 Token 压缩与工具优化**：`headroom`（+16.1k ⬆️）和 `LMCache` 等项目热度极高，说明 Agent 推理成本控制是行业痛点。Seaf 应考虑在日志模块中集成 Token 消耗统计与优化建议，帮助用户降低调用成本。

💡 **Agent 安全与 Skill 评测**：NVIDIA 开源 `SkillSpector`（+4.1k）专门做 Skill 安全扫描，OpenMontage 等 Agentic 系统对 Skill 质量提出更高要求。Seaf 应建立 Skill/MCP 上架前的安全审核与质量评分体系，提升平台可信度。

---

## 【本周 arXiv 热点论文】（cs.AI / Agent / LLM 相关）

- **Beyond Static Endpoints: Tool Programs as an Interface for Flexible Agentic Web Services** — 探索 Agent 时代工具接口的新范式（Submitted 18 Jun 2026）
- **ProvenanceGuard: Source-Aware Factuality Verification for MCP-Based LLM Agents** — 针对 MCP Agent 的事实性校验研究（Submitted 16 Jun 2026）
- **Compositional Skill Routing for LLM Agents** — LLM Agent 的组合式 Skill 路由，提升技能复用（Submitted 16 Jun 2026）
- **PrologMCP: A Standardized Prolog Tool Interface for LLM Agents** — 标准化 Prolog 工具接口融入 MCP 协议（Submitted 12 Jun 2026）

---
*数据来源：GitHub Releases / Trending / arXiv / 公开报道 | 2026-06-22*
