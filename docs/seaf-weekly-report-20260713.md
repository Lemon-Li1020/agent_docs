# 🌐 Seaf 竞品周报 | 2026-07-13（第 12 期）

> 数据周期：2026-07-07 ~ 2026-07-13

---

## 【ToC 智能体助手】

📌 **豆包** — 字节跳动持续强化豆包 PC 端与飞书联动，推出"工作流模式"内测，支持多智能体串联执行复杂任务。

📌 **ChatGPT** — OpenAI 发布 ChatGPT Mac 版重大更新，新增文件对话、项目管理（Projects）功能和自定义指令强化，桌面端体验进一步向专业用户靠拢。

📌 **Claude** — Anthropic 持续优化 Claude Code 编程能力，本周新增对大型代码库的上下文感知重构支持，内联代码审查准确率提升。

📌 **DeepSeek** — DeepSeek-V3 API 更新上下文窗口上限至 200K，同时对 MMLU、Math 等 benchmark 进行了新一轮优化，开发者生态持续扩大。

📌 **Gemini** — Google 在 I/O 2026 后持续推进 Gemini 2.5 与 Google Workspace 的深度集成，Gemini in Docs/Sheets 功能全面上线。

📌 **Kimi** — 月之暗面本周发布 Kimi 视觉思考模式，支持在推理过程中主动调用摄像头和屏幕截图，适用于复杂任务拆解与可视化思考。

---

## 【ToB 智能体工厂】

📌 **Dify** — v1.16.0-rc1 发布（2026-07-09），重磅推出**Dify Agent（实验性）**：基于 Linux 沙箱的智能体运行环境，支持 UI 构建、Skill 打包与工作流集成；同时新增 difyctl CLI 工具和严格的环境变量规范。
  - GitHub: https://github.com/langgenius/dify/releases/tag/1.16.0-rc1

📌 **FastGPT** — v4.15.1 发布，重构多项核心能力：新增**技能（Skill）模块**、Agent V2 loop 逻辑重写提升多轮工具调用稳定性、插件系统架构全面重构（workspace monorepo）、新增循环节点替代旧批量执行、PDF 解析替换为 liteparse 提速 3 倍、引入 PRO_TOKEN 服务间鉴权机制。
  - GitHub: https://github.com/labring/FastGPT/releases/tag/v4.15.1

📌 **Coze（扣子）** — 字节跳动 Coze 国内版本周更新插件市场，上线"Coze Studio"低代码智能体编排模板，新增电商客服和内容审核场景模板。

📌 **LangChain** — LangChain Python v0.3 发布，稳定版 API 落地，支持结构化输出强化和多模态工具链简化。

---

## 【GitHub Trending AI 类项目】

> 本周（截至 2026-07-13）

💻 **system_prompts_leaks** ⭐ 56,724 | ⬆️ +7,155 ⭐ | 收集各 AI 平台 system prompt 泄漏数据，持续引发安全与隐私讨论

💻 **chrome-devtools-mcp** ⭐ 46,768 | ⬆️ +872 ⭐ | Chrome DevTools MCP 服务，为编程智能体提供浏览器控制能力

💻 **strix** ⭐ 40,853 | ⬆️ +4,143 ⭐ | 开源 AI 渗透测试工具，可自动化发现并修复应用安全漏洞

💻 **codex-plugin-cc** ⭐ 28,055 | ⬆️ +2,803 ⭐ | OpenAI Codex 插件让 Claude Code 直接调用 Codex 辅助代码审查与任务分发

💻 **page-agent** ⭐ 26,216 | ⬆️ +2,666 ⭐ | 阿里开源 JavaScript GUI 智能体，通过自然语言控制网页界面

💻 **claude-skills** ⭐ 22,375 | ⬆️ +1,993 ⭐ | 345 个 Claude Code / Codex / Cursor 等编码智能体的 Skills 集合

💻 **pentagi** ⭐ 20,160 | ⬆️ +1,989 ⭐ | 全自主渗透测试 AI Agents 系统，基于 Go 实现

💻 **DesktopCommanderMCP** ⭐ 7,983 | ⬆️ +1,678 ⭐ | MCP Server 让 Claude 控制终端、搜索文件和 diff 编辑

💻 **claude-video** ⭐ 7,828 | ⬆️ +4,353 ⭐ | 让 Claude 具备"观看"视频的能力，自动下载、截帧、转录后交由 LLM 分析

💻 **archify** ⭐ 3,907 | ⬆️ +1,180 ⭐ | 任意智能体的架构图生成 Skill，支持多主题切换与多格式导出

💻 **OmniRoute** ⭐ 16,211 | ⬆️ +4,506 ⭐ | 聚合 231+ AI 提供商的免费网关，支持 Claude Code / Codex / Cursor 多端接入

---

## 【arXiv 热点论文（本周 cs.AI）】

📄 **IdeaGene-Bench**（arXiv:2607.08758）— 提出科学思想遗传推理与 IdeaGenome 基准，为 AI 生成具有继承变异脉络的科研新思路提供评测框架

📄 **多智能体市场稳定性**（arXiv:2607.08652）— 基于 DeepSeek-V3 的 18 个自利智能体模拟市场交易，验证调停（Mediation）机制是抗对抗攻击最鲁棒的稳定性方案

📄 **Knowing-Using Gap**（arXiv:2607.08393）— 揭示大模型微调后"记住了知识却不会用"的机理，提出 self-patching 定位失配表征并可恢复 58-75% 泛化差距

📄 **PolyUQuest**（arXiv:2607.08269）— 异构图感知的结构化 Web RAG 框架，可验证答案溯源至 HTML 结构证据，性能优于传统平面文本 RAG

📄 **MentalHospital**（arXiv:2607.08257）— 虚拟精神科临床评估环境，用 1193 份 EHR 构建标准化患者，评测 LLM 在 S.O.A.P. 全流程中的表现与医生差距达 37.28%

---

## 【Seaf 机会点】

💡 **加速 MCP + Skill 双生态联动**：FastGPT v4.15.1 和 Dify v1.16.0-rc1 均在本周强化了 Skill/Agent 能力，Seaf 应快速上线 Skill 模板商店并与 MCP 能力打通，形成"技能即插即用"的差异化体验，抢占开发者心智。

💡 **跟进沙箱智能体赛道**：Dify Agent 的 Linux 沙箱智能体方向是 ToB 平台的明确趋势，Seaf 应评估自研沙箱或集成 CubeSandbox（腾讯本周Trending，⭐9.8K，Rust 实现）的能力，作为 Agent 执行层的核心技术储备。

💡 **知识库差异化：结构化 RAG + 可验证溯源**：PolyUQuest 等论文显示结构化 Web RAG（异构图+可验证引用）是下一代知识库方向，结合 FastGPT 本周 PDF 解析 3 倍提速，Seaf 知识库应快速落地"引用高亮可点击溯源"和"多模态文档解析加速"功能，形成技术护城河。

---

*数据来源：GitHub Releases / Trending / arXiv cs.AI / 公开报道 | 2026-07-13*
