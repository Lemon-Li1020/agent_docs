# 🌐 Seaf 竞品周报 | 2026-07-20（第29期）

> 数据周期：2026-07-13 ~ 2026-07-20

---

## 【ToC 智能体助手】

📌 **豆包（字节）** — 豆包 macOS 版持续迭代，AI 搜索和深度思考能力进一步整合，上下文窗口扩大，支持更长对话记忆。

📌 **通义千问（阿里）** — Qwen3 系列全面开源（Qwen3-8B/32B/72B），支持 128K 上下文和 MCP 协议，Agent 能力显著增强，多语言任务执行效率提升。

📌 **Kimi（月之暗面）** — Kimi 推出 AI 助手 2.0 版本，强化多模态交互，支持同时处理文档、代码和图像；上下文缓存功能正式上线，降低长对话成本。

📌 **DeepSeek** — DeepSeek V3.0614 版本更新，上下文窗口扩展至 200K，支持更复杂的多轮推理；API 价格进一步下调 30%，强化价格战。

📌 **ChatGPT（OpenAI）** — GPT-5.6 正式发布，集成更强大的 Agent 模式，支持自主执行多步骤任务；OpenAI 发布 Responses API 全面替代 Chat Completions API。

📌 **Gemini（Google）** — Gemini 2.5 Flash 更新，上下文处理速度提升 40%，Agent 模式支持更丰富的工具调用，Deep Research 能力下沉至免费用户。

📌 **Claude（Anthropic）** — Claude 4 发布，支持 200K 超长上下文，Computer Use 能力正式上线，Agent 任务执行稳定性大幅提升。

---

## 【ToB 智能体工厂】

📌 **Dify** — v1.16.0 正式发布，重磅推出 **Dify Agent（Beta）**：基于 Linux 沙箱的 Agent 构建体验，支持 Skill 系统打包和分发，可通过 UI 创建 Agent 或在 Workflow 中引用；同步升级 MCP 协议至 2025-06-18 版本，支持动态 HTTP header 注入；修复多项 SQL 注入和 SSRF 安全漏洞；前端升级至 TypeScript 7 + Vite+ 工具链。[🔗 Release](https://github.com/langgenius/dify/releases/tag/1.16.0)

📌 **FastGPT** — v4.15.2 正式发布：工作流节点增加实时错误提示；自定义工具参数节点支持手动输入 JSONSchema 和必填选项；引入**企业认证/公司认证**能力；Agent V2 支持在门户页选择；OpenSandbox 镜像升级至 v0.2.1 修复中文文件名下载问题；**Agent Loop 执行内核完成统一重构**，ToolCall 与 Workflow Agent 共用执行链路，工具调度支持批量并行；安全方面移除 PPTX 解析高风险解压库。[🔗 Release](https://github.com/labring/FastGPT/releases/tag/v4.15.2)

---

## 【GitHub Trending AI 类】

💻 **[OpenAI / codex](https://github.com/openai/codex)** ⭐99,680 | ⬆️2,361 本周 | OpenAI 轻量级编码 Agent，直接在终端运行，支持多语言代码生成与执行。

💻 **[OpenCut-app / OpenCut](https://github.com/OpenCut-app/OpenCut)** ⭐75,860 | ⬆️12,743 本周 | 开源 CapCut 替代品，AI 驱动的视频剪辑工具。

💻 **[earendil-works / pi](https://github.com/earendil-works/pi)** ⭐72,762 | ⬆️8,987 本周 | AI Agent 工具包：统一 LLM API、Agent 循环、TUI 和编码 Agent CLI。

💻 **[OpenInterpreter / openinterpreter](https://github.com/openinterpreter/openinterpreter)** ⭐66,827 | ⬆️2,498 本周 | 开源模型的编码 Agent，支持 Kimi K3 等开放模型在本地执行任务。

💻 **[HKUDS / DeepTutor](https://github.com/HKUDS/DeepTutor)** ⭐27,920 | ⬆️2,375 本周 | 终身个性化 AI 导师系统，基于深度学习提供自适应学习路径。

💻 **[HKUDS / Vibe-Trading](https://github.com/HKUDS/Vibe-Trading)** ⭐25,281 | ⬆️5,228 本周 | 个人 AI 交易 Agent，集成多数据源进行市场分析和自动化交易。

💻 **[iOfficeAI / OfficeCLI](https://github.com/iOfficeAI/OfficeCLI)** ⭐19,646 | ⬆️4,269 本周 | 首个 AI Agent 办公自动化 CLI 工具，支持 Word/Excel/PowerPoint 的读写和自动化，无须安装 Office。

💻 **[tirth8205 / code-review-graph](https://github.com/tirth8205/code-review-graph)** ⭐21,164 | ⬆️1,103 本周 | 本地优先的代码智能图谱，支持 MCP/CLI，为 AI 编码工具提供精准的代码库上下文。

💻 **[Shubhamsaboo / awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps)** ⭐— | ⬆️— 本周 | 收录 100+ 可运行的 AI Agent 和 RAG 应用集合。

💻 **[kangarooking / cangjie-skill](https://github.com/kangarooking/cangjie-skill)** ⭐3,824 | ⬆️1,284 本周 | 将书籍、长视频、播客等内容蒸馏为可执行的 Agent Skills，与 Seaf Skill 概念高度相似。

---

## 【Seaf 机会点】

💡 **Skill 标准化赛道热度上升**：本周 `cangjie-skill`（将内容蒸馏为 Agent Skills）一周获 1.2K star，"Skill as 可执行知识单元"概念正在形成行业共识。Seaf 应加速 Skill 商店建设，制定 Skill 编写规范，抢占开发者心智。

💡 **B2B Agent 沙箱隔离成标配**：Dify Agent Beta 和 FastGPT OpenSandbox v0.2.1 均强调沙箱安全性，FastGPT 更引入企业认证能力。Seaf 若面向企业用户，Agent 沙箱隔离 + 企业身份认证是两个必须补齐的基础能力。

💡 **编码 Agent 赛道持续爆发**：OpenAI codex、OpenInterpreter、pi 等编码 Agent 合计周增 star 超 1.5 万，说明"AI 执行操作"替代"AI 给出建议"的范式已深入人心。Seaf 智能体工厂可考虑引入预置编码 Agent 模板（代码审查、数据处理、文件自动化），降低企业用户使用门槛。

---

*数据来源：GitHub Releases / Trending / 公开报道 | 2026-07-20*
