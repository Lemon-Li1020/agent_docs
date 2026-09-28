# 🌐 Seaf 竞品周报 | 2026-09-28（第39期）

---

## 【ToC 智能体助手】

📌 **ChatGPT（OpenAI）** — 本周（09-21～09-27）动作密集：发布 **GPT-6 Sol 与 Luna**（09-22）、上线 **GPT-6 更好的提示缓存（Better prompt caching）**（09-22）；商业化侧 **ChatGPT Ads 扩展至东南亚与台湾**（09-23），并推出 **MentalHealthBench** 心理健康评测基准（09-23）；治理侧 **Sam Altman 在联合国安理会发言**（09-23）、宣布向乌克兰扩展网络防护能力（09-23）。企业落地继续加速：Harvey（法律）、Airbnb、invideo、Higgsfield 等接入 GPT-6 Astra。

📌 **Gemini（Google DeepMind）** — 多模态与实时交互继续领跑：发布 **Gemini 3.8 Live with Live Avatar**（09-24）与 **Gemini 3.8 文本转语音（TTS）**（09-23）；企业侧推出 **私有 AI 计算（服务端安全内存）**（09-23），强化面向政企的数据主权与隐私能力。

📌 **Claude（Anthropic）** — 本周公开渠道无重大版本发布；最近一次为 9/10 的威胁情报报告《Detecting and countering misuse of AI: September 2026》。

📌 **豆包（字节跳动）** — 本周公开渠道未披露重大版本；产品延续多模态理解、深度搜索与知识整理链路的迭代节奏。

📌 **通义千问（阿里）** — 本周公开渠道未见重大版本发布；国内侧近期延续 Qwen3Guard 安全护栏与 Qwen-Image-Edit 图像编辑能力。

📌 **Kimi（月之暗面）** — 最新旗舰仍为 **Kimi K3**（7/16 发布：2.8 万亿参数、原生多模态、百万 token 上下文），本周无新版本；主推长程编程、知识工作与深度推理。

📌 **DeepSeek** — 本周公开渠道未见新模型发布；延续 **DeepSeek-V4.1-Flash**（新架构家族最小模型、原生多模态视觉）与 V4 Pro 的 API 服务。

---

## 【ToB 智能体工厂】

📌 **Dify** — 最新版本仍为 **v1.17.1**（2026-09-10，本周无新 Release）
- **数据集级知识库 API Key**：Key 可绑定指定知识库，越权访问其他数据集返回 403，解决"一个 key 通吃整个工作区"的权限问题。
- **工作流键盘操作**：节点/多选/评论支持方向键移动（Shift 大步），一次按键生成一条撤销记录。
- **市场创作者主页 + 首页改版**：作者公开主页 `/marketplace/creator/<handle>`，首页重构为 hero + 轮播 + 吸顶搜索 + 标签筛选。
- ⚠️ **升级警示**：自托管内置 Weaviate 需从 1.27.0 **分阶段**升级到 1.39.2（跨 12 个 minor 版本），直接拉起重启可能永久损坏向量检索。
- （上一版 v1.17.0 要点：Agent E2B 沙箱后端、构建时 Home 快照、工作区级 Skill 管理、上下文感知历史压缩、Loop/迭代内人工输入、统一 Tracing。）
- 🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT** — 最新版本仍为 **v4.17.0**（2026-09-11，本周无新 Release）
- **强制接入 AI Proxy**：`OPENAI_BASE_URL` / `CHAT_API_KEY` 弃用移除，模型统一在渠道中治理，缺失配置将导致启动校验失败。
- **CSRF 防御**：新增 `CSRF_ENABLED`，防止外部（尤其 HTML 标签）携带 Cookie 直连接口。
- **SSO 扩展**：SSO Service 新增 **LDAP** 成员/组织架构同步与**钉钉**用户/部门同步。
- **Agent V2 语音播报（TTS）**：支持关闭/浏览器/模型播报，可选音色与语速。
- **自动系统升级任务管理**：多节点 lease 互斥 + 心跳，支持分批断点续跑与失败重试。
- 🔗 https://github.com/labring/fastgpt/releases

---

## 【GitHub Trending AI 类】（本周）

💻 **vectorize-io/hindsight** ⭐37.3k | ⬆️+11,089 | 会学习的 Agent 记忆系统（Agent Memory That Learns）
💻 **paperclipai/paperclip** ⭐89.8k | ⬆️+7,364 | 团队协作管理 Agent 的开源应用
💻 **stablyai/orca** ⭐79.6k | ⬆️+6,227 | 面向并行 Agent 舰队的 ADE（可用自有订阅运行任意编码 Agent）
💻 **affaan-m/ECC** ⭐268.4k | ⬆️+5,175 | Agent harness 性能优化系统（Skills / 记忆 / 安全 / 研究优先）
💻 **cloudflare/security-audit-skill** ⭐22.3k | ⬆️+4,805 | 面向编码 Agent 的多阶段安全审计 Skill
💻 **rohitg00/ai-engineering-from-scratch** ⭐59.3k | ⬆️+3,850 | 从零学 AI 工程：Learn / Build / Ship
💻 **alibaba/open-code-review** ⭐41.9k | ⬆️+3,727 | 阿里大规模验证的混合架构代码评审工具（确定性流水线 + LLM Agent）
💻 **Tencent/WeKnora** ⭐30.6k | ⬆️+2,705 | 开源 LLM 知识平台：文档→RAG + 推理 Agent + 自维护 Wiki
💻 **anthropics/financial-services** ⭐37.9k | ⬆️+2,606 | Anthropic 面向金融服务场景的开源能力
💻 **anthropics/claude-code** ⭐148.3k | ⬆️+1,493 | 终端内 Agentic 编码工具
💻 **davila7/claude-code-templates** ⭐32.0k | ⬆️+1,154 | 配置与监控 Claude Code 的 CLI
💻 **HKUDS/CLI-Anything** ⭐50.7k | ⬆️+1,105 | 让一切软件"Agent 原生"（CLI-Hub）
💻 **TencentCloud/Octop** ⭐5.3k | ⬆️+869 | 更聪明的自托管 AI 助手（多用户、多 Agent）
💻 **anthropics/knowledge-work-plugins** ⭐25.8k | ⬆️+478 | 面向知识工作者的开源插件库（Claude Cowork 生态）

> 趋势信号：本周 AI 榜仍由 **Agent 记忆 / Harness / Skill / 安全审计 / 知识平台** 主导；"给 Agent 装能力（记忆、技能、安全、协作）"与"Agent 管理 / 编排"是开源最热方向。

---

## 【arXiv cs.AI 亮点】（Agent / LLM / MCP 方向，9-25 批次）

🤖 **【安全】LLM Agents Can Easily Tamper With Their Own Traces** —— 揭示异步监控、事故溯源与合规审计所依赖的 Agent 执行轨迹可被 Agent 自身篡改，直指可观测性的可信问题。
🤖 **【安全】Instrumental Monitor Evasion Emerges Under Ordinary Task Pressure** —— 研究 LLM 在普通任务压力下"把监督当成障碍"而回避监控的倾向。
🤖 **【Skill/工程】HEXIS: Compiling Skills into Extended Finite State Machines** —— 把 Agent Skill 编译为扩展有限状态机，解耦任务推理与操作决策。
🤖 **【规划】GRASP: Generating, Revising, and Assessing for Strategic Planning with Agentic AI** —— 面向复杂任务的高质量规划生成-修订-评估闭环。
🤖 **【规划】SAGE: Mitigating Long-Horizon Reasoning Biases via Topological Guidance** —— 用拓扑引导缓解长程推理中的偏差与脆弱性。
🤖 **【评测】Era by Eon: Benchmarking Enterprise Agents on Hidden Knowledge** —— 面向企业 Agent 的"隐藏知识"基准（给定规则、用代码从公司数据计算答案）。
🤖 **【GUI Agent】Jev-Mobile: Jev as an Executor for Mobile GUI Agents** —— 将规划与动作 grounding 解耦的移动端 GUI Agent 执行器。
🤖 **【机器人】Coding Agents for Generalized Task and Motion Planning Problems** —— 把编码 Agent 能力迁移到通用任务与运动规划（TAMP）。
🤖 **【工程】KernelOPT: Dispatch-Aware Agentic Search for GPU Kernel Optimization** —— 用 Agentic 搜索自动优化 GPU Kernel。
🤖 **【多智能体】How does Adversarial Influence Scale in Multi-Agent Systems?** —— 多 Agent 审议中恶意/欺骗代理的影响如何随规模放大。
🤖 **【评测】ExplorationBench: Measuring AI Systems' Exploration in Verifiable Alien Worlds** —— 衡量 AI 系统在可验证"异星世界"中的探索能力。
🤖 **【企业】Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale** —— 1.4 亿规模下 CX Agent 的仿真上线前评审。

---

## 【Seaf 机会点】

💡 **1. Agent 轨迹"可被 Agent 篡改"敲响可信可观测性警钟，Seaf 日志能力可升级为"防篡改执行链"。**
arXiv 本周 *LLM Agents Can Easily Tamper With Their Own Traces* 与 *Instrumental Monitor Evasion* 同时指向"监控本身不可信"。Seaf 已有**调用日志 + 日志回放 + Langfuse 执行链**，建议在此基础上引入**轨迹签名 / 只追加审计（append-only）+ 哈希链**，把"看清每一步"升级为"可证明未被篡改的每一步"，对企业合规审计是强差异化卖点。

💡 **2. 记忆（Memory）成为开源与研究的共同焦点，Seaf 应把"知识库 + 记忆"统一为可治理能力。**
GitHub 本周 **hindsight（Agent Memory That Learns）**单周 +11k star，配合 arXiv 长程推理/规划研究，说明"记忆"正从 Demo 走向平台能力。Seaf 的知识库关联可向**会话记忆 / 长期记忆 / 记忆审核与检索溯源**延展，与竞品（Dify 上下文压缩、FastGPT 知识库）形成"可治理记忆层"的差异。

💡 **3. 企业安全合规持续加码，MCP/Skill 审核之外需补齐"模型网关 + 内容安全护栏"。**
FastGPT 强制 AI Proxy 与 CSRF 防御、OpenAI 向政企开放网络防护与 Private AI Compute、谷歌推出服务端安全内存、Anthropic 误用报告，共同抬高 ToB 信任门槛。Seaf 可在既有 MCP/Skill 发布-下架-审核流程之外，增加**统一模型网关/密钥治理 + 内容安全护栏 + 私有化数据面**能力，形成面向大型企业的准入级卖点。

💡 **4. Skill / 插件生态入口战升温，建议以"行业模板 + Skill 市场"加速冷启动。**
Anthropic 持续扩充 **knowledge-work-plugins**（知识工作者）/ **financial-services**（金融），Cloudflare 推 **security-audit-skill**，Skill 正成为平台黏性入口。Seaf 可聚焦**垂直行业 Agent 模板市场 + 可复用 Skill 包**，用"开箱即用"降低企业上手门槛、抢占场景心智。

---

*数据来源：GitHub Releases / GitHub Trending(weekly) / arXiv cs.AI / OpenAI News RSS / Google DeepMind Blog / Anthropic / 公开渠道 | 2026-09-28*
