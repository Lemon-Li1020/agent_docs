# 🌐 Seaf 竞品周报 | 2026-05-11（第20期）

---

## 【ToC 智能体助手】

- **豆包（ByteDance）** — 豆包持续深化多模态能力，5月初在办公场景推出AI PPT生成与协作功能，与飞书/WPS深度集成，进一步蚕食微软Copilot在中文办公市场。
- **通义千问（阿里）** — 阿里云通义发布Qwen3.5系列小模型（1.8B/4B），在端侧部署性能大幅提升，同时推出"通义听见"企业版，支持会议实时多语言字幕与摘要。
- **Kimi（月之暗面）** — Kimi发力长上下文处理，推出200K上下文窗口企业API定价下调30%，并新增文档问答、知识库管理多模态插件生态。
- **DeepSeek** — DeepSeek-V3上周开源后引发全球热潮，代码能力逼近GPT-4，HuggingFace单周下载量超500万次；同时DeepSeek API新增MCP工具调用支持。
- **ChatGPT（OpenAI）** — OpenAI为ChatGPT推出"深度研究"Agent模式，可自主浏览网页、编写并执行Python代码完成复杂分析任务；GPT-5进展持续受到关注。

---

## 【ToB 智能体工厂】

- **Dify** — 发布 v1.14.0（4月29日），核心亮点：**协作模式（Workflow Collaboration）** 支持多人实时编辑同一工作流，含在线状态与图谱同步；新增HITL（Human-in-the-loop）Service API；MCP工具元数据刷新机制完善；引入@langgenius/dify-ui共享组件库；Langfuse可观测新增TTFT指标；安全性方面修复邮箱变更token处理漏洞（GHSA-4q3w-q5mc-45rq）。

  🔗 https://github.com/langgenius/dify/releases/tag/v1.14.0

- **FastGPT** — 发布 v4.15.0-beta1（5月9日），核心亮点：**循环节点（Loop Run）** 正式替代旧批量执行；全局变量支持object类型；工具调用模式支持文件注入虚拟机；新增S3 CDN配置与模型思考配置；安全方面加强SSRF防护与AST沙箱检查；工程化升级Next.js + Turbopack + Node.js 24。

  🔗 https://github.com/labring/FastGPT/releases/tag/v4.15.0-beta1

---

## 【GitHub Trending AI 类】

| 仓库 | ⭐总星 | 📈本周增长 | 简介 |
|------|--------|-----------|------|
| `mattpocock/skills` | 69,048 | +12,722 | AI编码Agent工程技能集，Claude/MCP最佳实践 |
| `TauricResearch/TradingAgents` | 73,200 | +8,872 | 多Agent LLM金融交易框架，LlamaIndex集成 |
| `ruvnet/ruflo` | 48,477 | +10,779 | Claude Agent编排平台，支持多Agent swarm编排 |
| `addyosmani/agent-skills` | 38,393 | +10,738 | 生产级AI编码Agent技能工程化指南 |
| `Hmbown/DeepSeek-TUI` | 24,017 | +22,034 | 终端DeepSeek Coding Agent，Rust实现 |
| `anthropics/financial-services` | 18,781 | +10,272 | Anthropic金融领域AI Agent参考架构 |
| `VectifyAI/PageIndex` | 30,443 | +4,328 | 向量-less推理RAG，革新文档检索范式 |
| `dexter/virattt` | 25,156 | +2,741 | 自主金融深度研究Agent，TypeScript |
| `bytedance/UI-TARS-desktop` | 32,093 | +2,191 | 多模态AI Agent技术栈，UI自动化 |
| `local-deep-research/LearningCircuit` | 7,073 | +2,483 | 本地化深度研究，3090即可运行Qwen3.6-27B |
| `cocoindex-io/cocoindex` | 9,481 | +1,831 | 长时域Agent增量计算引擎 |
| `InsForge/InsForge` | 9,335 | +1,377 | 全栈Agent编码后端平台，含数据库/Auth/存储 |
| `browserbase/skills` | 3,087 | +1,403 | Browserbase官方Web访问Agent技能集 |
| `openai/symphony` | 23,155 | +2,204 | OpenAI开源Agent工作流管理框架（Elixir） |
| `withastro/flue` | 3,072 | +1,014 | Astro沙箱Agent框架 |

---

## 【arXiv 热点论文（本周 cs.AI）】

- **DADL**（5月4日）— LLM Agent企业工具库的声明式描述语言，兼容MCP协议。
- **AgentTrust**（5月6日）— AI Agent运行时安全评估与拦截框架，覆盖文件/Shell/HTTP等危险操作。
- **TSCG**（5月4日）— Agentic LLM部署的确定性工具Schema编译方法。
- **When Agents Handle Secrets**（5月7日）— Agentic AI机密计算综述，涵盖TEE/安全飞地等前沿方向。
- **ARIS**（5月4日）— 对抗性多Agent协作的自主研究框架。
- **Feedback-Normalized Dev Memory**（5月2日）— RL编码Agent的安全门控MCP架构。

---

## 【Seaf 机会点】

1. **Agent安全能力补齐**：FastGPT和Dify本周均在安全方向（SSRF防护、沙箱AST检查、IDOR加固）密集发力。Seaf应优先构建统一的**Agent运行时安全扫描**能力，包括MCP工具URL校验、Shell命令白名单、文件操作风险提示，这是企业客户的核心刚需。

2. **Workflow协作与多Agent编排**：Dify v1.14.0推出实时协作工作流，FastGPT推出循环节点（Loop Run）。Seaf应加速**多人协作编辑**和**多Agent协同编排**功能，参考ruflo的多Agent swarm思路，形成差异化竞争优势。

3. **垂直领域Agent加速落地**：本周GitHub热榜中金融领域（TradingAgents、financial-services、dexter）占比极高，DeepResearch类需求爆发（local-deep-research 2500+⭐/周）。Seaf可考虑在智能体工厂中内置**金融/法律/医疗垂直Agent模板**，快速抢占ToB市场。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-05-11*
