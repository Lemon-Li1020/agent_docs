🌐 Seaf 竞品周报 | 2026-10-26（第43期）

> 覆盖周期：2026-10-20 ~ 2026-10-26　周期内 ToC / ToB 智能体平台与 AI 开源生态动态

---

## 【ToC 智能体助手】

📌 **OpenAI / ChatGPT** — 本周主线是「让 Agent 做更快的小决策」与企业分发：
- 10/22 **Decisions API 正式 GA**：基于 **GPT-6 Luna**，专攻「有界答案」的判定类调用（分类、路由、下一步动作），比走 Responses API **快至 10×**；单请求最多 **400 个问题**（翻倍），新增 GPT-Live 集成、prompt caching、美/欧推理驻留。
- 10/21 **OpenAI 模型上 Google Cloud**（多云分发）；**ChatGPT Ads 扩展至 26 个新国家**（商业化加速）。
- 10/22 **Uber 全员铺开 ChatGPT Work**，企业侧 Agent 落地再添大客户案例。
- 10/21 **Patch the Planet**：以 Agent 批量发现关键漏洞并做全球协同披露，安全场景的 Agent 规模化信号。
- 10/23 工程博客：支撑 **10 亿 ChatGPT 用户**的在线存储扩展（Part II）。

📌 **DeepSeek** — 模型静默换代 + Agent 工具链开放：
- API 文档更新：`deepseek-flash` 现由 **DeepSeek-V4.1-Flash-1017** 提供服务；旧名 `deepseek-v4-flash` / `deepseek-v4-flash-vision-exp` 仍可调用但对应模型已退役，按 Flash 价格计费。
- **DeepSeek Harness 开发者预览**开放（面向 agent harness 开发者），并明确 Claude Code / GitHub Copilot / OpenCode 可直接以 DeepSeek 为后端模型。

📌 **Kimi / Moonshot** — 编码 Agent 客户端一周连发三版：
- **kimi-code 2.3.0（10/21）→ 2.3.1（10/23）→ 2.3.2（10/25）**：插件技能统一为 `<pluginId>:<skillName>` 限定名（同名技能不再互相覆盖，裸名调用失效）；远程控制的大请求/响应改为流式传输，上限 **10 MiB → 100 MiB** 且并发受限以保护内存；会话中切换模型新增确认弹窗（新建会话/压缩后继续/直接继续/取消）。

📌 **通义 / Qwen** — 桌面端与托管会话能力补齐：
- **qwen-code v0.26.1 + Qwen Code Desktop v0.26.1（10/24）**：daemon token 持久化（`--save-token` 写入仅所有者可读文件）；Workspace 绑定的 Managed Session 支持**空闲时手动上下文压缩**（保留审计历史）；OpenTUI 的输入/草稿/statusline 行为对齐 Ink；Shell 工具会提醒模型记录命令写出的文件。
- 仓库活跃度维持高位（⭐28.7k，10/26 仍有提交）。

📌 **豆包 / 字节** — 本周**无可核验的产品版本公告**（豆包/火山引擎页面为 JS 渲染，抓取未取到有效内容）。可侧证的是字节 Seed 开源侧持续投入：VeOmni（训练/推理编排）10/24 有更新。**不臆测产品更新**。

---

## 【ToB 智能体工厂】

📌 **Dify — v1.18.0（2026-10-23）** 本周最重磅 ToB 发布，四个方向：
- **Agent 决定下一步**：新增 **Output Routes**，让 Agent 按条件选择工作流分支（直接答复 or 转交专家），并提供只读的 route 输出便于追踪；Plain Agent v2 节点开始**流式输出**文本。
- **可移植应用包 `.ifpkg`**：把应用连同内联 Agent、Skill 及其文件打成单包迁移，导入时在新工作区重建资源并**重映射引用**；文件/URL 导入同时支持包与 YAML。
- **嵌套工作流可观测**：从运行历史进入 Workflow Tool 子图，逐步查看子流程，支持协调式 pause/resume/stop 与文件输出，并有源应用详情的权限校验。
- **Agent Knowledge Base（Beta）**：独立知识空间，可看文档处理、元数据、检索 trace 与质量评估；新增 Knowledge Retrieval 节点，与经典知识库并存（需独立服务与数据库）。
- 开发者侧：**OpenAPI + 新 CLI `difyctl`**（应用创建、DSL 导入导出、发布、版本回滚、draft hash 防并发覆盖），可 `difyctl install skills`。
- ⚠️ 升级注意：Agent Backend/runtime/API/worker 需一起升级，`/runs` 只接受 composition v2，本地 Agent 沙箱必须设非空 token，源码安装需 Python 3.13，`PASSWORD_PEPPER` 必须保留。
- 🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT — 本周无新 Release**，最新仍为 **v4.17.2（2026-10-09）**（上期已详述）：知识库数据提前落库 + 索引三态流转（parsed → indexing → indexed）、QA 一对多拆分优化、训练进度看板、控制台 CSR 迁移与 i18n 优化、BullMQ 失败任务按数量保留、If/Else 非字符串条件修复。
- 🔗 https://github.com/labring/fastgpt/releases

---

## 【GitHub Trending AI 类】（本周）

💻 **cloudflare/security-audit-skill** ⭐46,865 | ⬆️+15,072 | 给编码 Agent 用的多阶段安全审计技能，产出可机器校验的结论
💻 **stablyai/orca** ⭐105,812 | ⬆️+9,622 | 用一个订阅驱动一支 Agent 舰队（Claude Code、Grok Bot 等），桌面/移动/远程运行时
💻 **anomalyco/opencode** ⭐221,515 | ⬆️+5,921 | 开源编码 Agent
💻 **heygen-com/hyperframes** ⭐72,152 | ⬆️+5,612 | 写 HTML 即渲染视频，为 Agent 而设计
💻 **akitaonrails/ai-memory** ⭐13,519 | ⬆️+3,254 | 编码 CLI 的长期记忆与跨厂商 Agent 交接（Rust）
💻 **ruvnet/ruflo** ⭐79,280 | ⬆️+2,987 | 多 Agent 蜂群编排框架：自适应记忆、自学习、联邦、向量 RAG
💻 **anthropics/knowledge-work-plugins** ⭐32,977 | ⬆️+2,790 | 面向知识工作者的 Claude Cowork 插件集
💻 **anthropics/claude-plugins-official** ⭐44,560 | ⬆️+2,245 | Anthropic 官方管理的 Claude Code 高质量插件目录
💻 **pingdotgg/t3code** ⭐30,125 | ⬆️+1,770 | 轻量编码 Agent 客户端（TypeScript）
💻 **vllm-project/vllm** ⭐95,490 | ⬆️+1,445 | 高吞吐 LLM 推理与服务引擎（持续霸榜基础设施位）

---

## 【arXiv 前沿】（cs.AI，10/22–10/23 批次）

📄 **EpiSEM-Bench**（2610.31650）— 证据缺失场景下 LLM Agent 的安全性与证据恢复能力评测基准
📄 **AgentPhishing**（2610.31404）— 自适应攻击下 LLM 邮件 Agent 的安全基准
📄 **Certified Execution Harness**（2610.31376）— 用 Petri 网监督控制卡在「推理」与「动作」之间，做最小侵入的安全执行壳
📄 **Adaptive Skill Granularity for Coding Agents**（2610.31461）— 运行时路由 + 宏/微恢复，动态调整技能粒度
📄 **Muffin**（2610.31355）— 面向异步多 Agent 的共享记忆缓冲区
📄 **Subgoal-aware Memory Graph**（2610.31307）— GUI Agent 的子目标感知记忆图
📄 **Training Small Language Models for Transferable Tool Selection**（2610.31483）— 小模型的可迁移工具选择能力
📄 **Post-Audit Mirage**（2610.31130）— 离线 Agent 校验的可识别性上限（审计≠可信）
📄 **RIDAR**（2610.31372）— 自主科研 Agent 的完整性检测与运行时干预

---

## 【Seaf 机会点】

💡 **1. 「可解释的决策路由」该进编排层了。** Dify 1.18 把「Agent 选下一个分支」做成一等公民（Output Routes + 只读 route 输出），OpenAI 同时用 Decisions API 把「小决策」单独产品化（10× 延迟优势）。Seaf 编排 Tab 建议补**条件路由节点 + 命中原因可回放**（直接复用已有调用日志/日志回放/Langfuse 执行链），让企业能回答「为什么走了这条分支」——这是测试验收和线上排障的刚需。

💡 **2. 应用「一键打包迁移」是私有化交付的胜负手。** `.ifpkg` 把应用 + 内联 Agent + Skill + 文件打成单包并在导入侧重映射引用，等于把「交付物」标准化。Seaf 三平台（开发/用户/管理）天然适合做**智能体交付包**：智能体 + Skill + MCP 依赖 + 知识库引用 + 权限声明，导入时按目标环境重绑定并触发审核流。对 ToB 私有化项目，这一条能直接省掉大量手工配置与联调。

💡 **3. 知识库要从「能检索」升级到「可解释 + 可评估」。** Dify Agent KB 把文档处理、元数据、检索 trace、质量评估放在一个视图；FastGPT 用三态索引解决长训练链路的一致性。Seaf 知识库建议补**索引状态可视化 + 检索 trace + 失败可重试**，并把「检索质量评估」做成可跑的分层用例——这既是产品能力，也是测试侧的验收抓手。

---

*数据来源：GitHub Releases（Dify / FastGPT / kimi-code / qwen-code）/ GitHub Trending（weekly）/ OpenAI News / DeepSeek API Docs / arXiv cs.AI | 2026-10-26*
