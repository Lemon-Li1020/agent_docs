🌐 Seaf 竞品周报 | 2026-11-09（第 46 期）

> 本期聚焦：ToC 侧「托管式 Agent」发力（Kimi Hosted Agents、Perplexity Teammate），ToB 工厂进入「可观测性 + 打包可移植」竞争期（Dify 1.19 递归链路追踪），GitHub Trending 上 Agent Skills / 上下文记忆 / Agent 专用浏览器继续霸榜。

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动 · 火山方舟）** — 11 月模型清单显示 doubao-seed-evolving 深度思考模型完成版本更新，升级集中在 Agent 复杂任务执行与抗幻觉：多步骤任务的任务规划与结果验收更完整，工具调用与事实一致性明显改善，多数场景响应时延与单次成本同步下降，统一 Model ID 调用即自动生效。

📌 **通义千问（阿里 · 百炼 / Qwen）** — 本周公开渠道未捕获重大模型或平台版本发布（百炼「产品动态」页本期无可解析更新），维持上期能力组合（qwen-audio-3.1-realtime-flash 实时双工语音、PixVerse V6 视频、Ling-3.1-flash、Tripo 3D 全家桶）；建议下周继续跟踪其「模型货架扩充」节奏。

📌 **Kimi（月之暗面）** — 「Kimi Hosted Agents」正式发布，把 Agent 从「本地跑脚本」推进到平台托管运行（会话持续、任务在后台推进），是本周 ToC 侧最明确的「Agent 产品化」信号，直接对标 ChatGPT Agent / Claude 的托管代理形态。

📌 **DeepSeek（深度求索）** — 主线仍是 DeepSeek-V4.1-Flash-1017（旧 deepseek-v4-flash / vision-exp 已退役，请求自动承接、按 Flash 价计费）；API 文档明确「Agent 友好」路线：DeepSeek Harness 已进入开发者预览，并给出 Claude Code / GitHub Copilot / OpenCode 等 Agent 后端接入指南。

📌 **ChatGPT（OpenAI）** — 宣布收购 Pierre，用以扩充 Codex 开发者工具生态，编程 Agent 的「工具链纵深」继续加厚；同期 Google 侧 Gemini Omni 1.2 Flash 将视频生成时长拉到 15 秒、API 价格下调 30%，海外多模态价格战延续。

📌 **其他值得注意** — Perplexity 上线「Teammate」功能（以 AI 代理程式管理持续性专案）；Meta Muse 支持视频对话（给 AI「安上脸和嗓子」）；iOS 27.3 曝光 HomeView 将接入 ChatGPT 与 Claude，系统级入口之争升温。

---

## 【ToB 智能体工厂】

📌 **Dify — v1.19.0（2026-11-04）｜Trace Your Workflows, Layer by Layer**
- **嵌套工作流追踪（Nested workflow tracing）**：外部观测（如 Langfuse）现在能看到 Workflow Tool 内部被持久化的执行步骤，子步骤挂在调用它的 Tool span 之下，保留嵌套与重复调用的层级；同时带出格式化 prompt / response、token 用量、项目-trace-observation 链接。历史 trace 不回填，滚动升级需按文档调整 tracing 队列。
- **Workflow Tools 随应用打包**：`.ifpkg` 应用包现在会把 Workflow Tool 背后的工作流按「绑定版本」一并打包，含传递依赖；导入时复用目标空间已有工具并重建缺失部分。
- **Skill Hub 自动化**：Skill Hub 增加自动化能力；Agent 文件的上传与预览体验优化。
- **插件守护进程**升级至 0.6.14-local。
- 🔗 https://github.com/langgenius/dify/releases/tag/1.19.0

📌 **FastGPT — v4.17.4（2026-11-05）｜以稳定性收尾**
- **体验优化**：列表滚动分页监听优化，减少滚动中组件重渲染。
- **对话体验修复**：免登录分享对话中「全局变量 / 交互表单使用模型选择器」未携带分享鉴权导致模型列表加载失败；顶部变量面板不再向分享用户暴露外部变量；修复分享对话删除消息、重试、编辑后发送失败。
- **关键修复**：部分工作流工具「编辑器配置正常但运行时被错误过滤、无法调用」；工具参数 JSON Schema 格式不规范导致模型请求失败 —— 均为 Agent 落地链路上的高频坑。
- **其他**：列表在内容缩短后无法继续滚动加载 / 分页失败后重复请求；账号与团队侧中文输入法回车误提交。
- 🔗 https://github.com/labring/FastGPT/releases/tag/v4.17.4

> 观察：Dify 已把竞争重心从「功能有没有」转到「运行时可观测 + 资产可搬运」；FastGPT 本周则是纯稳定性迭代，说明其 Agent/知识库主链路进入收敛期。

---

## 【GitHub Trending AI 类 · 本周】

💻 **NVIDIA/auto-ontology** ⭐10,380 | ⬆️ +9,327 | 在数据之上构建语义图谱推理层的 Python 框架，面向 LLM/Agent 工作流做确定性查询生成与更可解释的上下文检索（本周增速第一）
💻 **thedotmack/claude-mem** ⭐114,901 | ⬆️ +6,443 | 跨会话持久上下文：捕获 Agent 会话、AI 压缩、再把相关上下文注入未来会话
💻 **pingdotgg/t3code** ⭐52,487 | ⬆️ +15,379 | 本周绝对增量冠军（TS 生态编码工具链）
💻 **Donchitos/Claude-Code-Game-Studios** ⭐37,003 | ⬆️ +5,235 | 把 Claude Code 变成「游戏工作室」：49 个 Agent + 72 个 workflow skill + 层级协作体系
💻 **Nutlope/hallmark** ⭐50,960 | ⬆️ +6,356 | 反「AI 味」设计技能（Claude Code / Cursor / Codex）
💻 **blader/humanizer** ⭐66,501 | ⬆️ +3,118 | 去除 AI 生成痕迹的写作技能
💻 **D4Vinci/Scrapling** ⭐99,876 | ⬆️ +8,342 | 从单请求到全站爬取的 Web Scraping 框架
💻 **vercel-labs/agent-browser** ⭐47,588 | ⬆️ +2,190 | 面向 AI Agent 的浏览器自动化 CLI（Rust）
💻 **max-sixty/worktrunk** ⭐12,119 | ⬆️ +2,313 | Git worktree 管理 CLI，专为并行 Agent 工作流设计
💻 **anthropics/skills** | Agent Skills 官方公共仓库（持续在榜）
💻 **github/spec-kit** | SDD（规格驱动开发）工具包，Agent 工程化的另一条路线

> 观察：本周结构很清晰 —— ①「Agent 上下文/记忆」成为独立赛道（claude-mem、auto-ontology）；②Skills 从「炫技」转向「祛 AI 味、审美、写作」等拟人化质量；③Agent 专用基础设施（浏览器、worktree、PR Review）开始成规模。

---

## 【前沿论文速览 · arXiv cs.AI】

📄 SwarmEvolve: Latent Agent Swarms for Evolutionary Discovery and Optimization（2611.08483）
📄 Enhancing Local and Global Structure in Compressed AI Agent Memory（2611.08341）
📄 MCPHallu: Benchmarking Reasoning, Execution, and Memory Hallucinations in MCP Agents（2611.07689）
📄 Don't Prompt Your Agents. Equip Them: Skillware as a Modular Standard for Auditable, Deterministic Capability Execution（2611.07652）
📄 SMART: State-based Multi Agent Reasoning Traces for Verification-oriented Problem-Solving（2611.08196）
📄 Benchmarks as Software: Terminal-Bench and the Case for Continuous Benchmarks（2611.08417）
📄 Persistent Retrieval for Conversational Agents: A Study of Retrieval Efficiency（2611.07899）
📄 PCBRouteAgent: How Close Are LLM Agents to Becoming PCB Routing Engineers?（2611.08175）
📄 StepBack: Step-Level Error-Localized Resampling for Efficient Test-Time Reasoning（2611.08403）
📄 Beneath the Surface: What We Overlook When We Talk About Agent Evolution（2611.07624）

> 趋势：①Agent 记忆压缩后「局部+全局结构」保真；②MCP Agent 的幻觉评测（推理/执行/记忆三类）首次成体系；③「别 prompt，装备它们」—— 技能化能力封装标准；④连续化基准（Benchmark as Software）在挑战一次性榜单。

---

## 【Seaf 机会点】

💡 **1｜把「嵌套链路追踪」做成平台级默认能力，而不是可选项**
Dify 1.19 已能把多层 Workflow Tool 的内部步骤连同 LLM 上下文完整下钻到 Langfuse；这正在变成企业采购的硬指标。Seaf 若在「智能体调试/运行详情」里默认提供「调用树 + 每层输入输出 + token 成本」，并支持导出到主流观测后端，可同时服务测试同学（定位失败层）与客户（成本归因），形成比 Dify「需自建 Langfuse」更开箱即用的差异点。

💡 **2｜MCP/Skill 的「幻觉与安全」评测是空白位，可抢先建立标准**
本周 arXiv 出现 MCPHallu（系统性评测 MCP Agent 的推理/执行/记忆幻觉）、Skillware（可审计、确定性的技能封装标准），而 Trending 上 Skills 仓库仍以「好玩」为主。Seaf 已有 MCP/Skill 发布-审核流程，建议补一套「技能准入评测集」：参数 Schema 合法性、越权调用、执行失败重试、幻觉率，用评测报告作为上架门槛 —— 这是竞品都没有的治理护城河，也能直接复用你们已有的评测框架沉淀。

💡 **3｜企业资产「可搬运」应补齐到 Skill / 知识库 / 环境变量层级**
Dify 1.19 把 Workflow Tool 的底层工作流按绑定版本打进 .ifpkg（含传递依赖），FastGPT 则在本周修「工具运行时被过滤 / Schema 不规范」这类迁移后的运行期坑。说明客户真实痛点在「跨环境迁移后还能跑」。建议 Seaf 把「应用包」升级为「资产包」：Agent + Skill + MCP 连接 + 知识库 + 模型/环境变量 + 版本锁，导入时做依赖解析与冲突预检，导出即交付 —— 直接吃下 ToB 交付场景。

---

*数据来源：GitHub Releases（Dify / FastGPT）/ GitHub Trending（weekly）/ arXiv cs.AI recent / 火山方舟模型发布公告 / AIbase 公开报道 | 2026-11-09*
