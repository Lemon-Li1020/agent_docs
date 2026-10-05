# 🌐 Seaf 竞品周报 | 2026-10-05（第40期）

---

## 【ToC 智能体助手】

📌 **ChatGPT（OpenAI）** — 本周（09-28～10-04）动作密集：**DevDay 2026**（09-29）发布 **GPT-6.1 Sol**（09-29，附安全 Addendum）与新产品 **dots**（09-29）；产品侧发布《**用 GPT-6 构建的实用指南**》（10-02）；安全侧披露一起**协同模型蒸馏（model-distillation）攻击**（09-30）并发布前沿 AI 训练安全案例框架（09-28）。生态侧牵手 **AWS** 布局托管 Agent（推 500 美元 Pro 顶配套餐）、与 **ModRetro** 推 Codex 复古 Game Boy 游戏插件；另有《纽约时报》报道指 GPT-6.1 Astra 因内部安全预警被搁置。

📌 **Claude（Anthropic）** — 本周公开渠道无新版本，最新为 **Claude Opus 5.5**（09-22，多数任务达到 Fable 5.1 水平、运行成本较 Opus 5 降 40%）。资本侧：招股书曝光**亏损超 80 亿元**、向 **SpaceX 豪掷 845 亿美元**锁定 AI 算力。

📌 **Gemini（Google / DeepMind）** — 面向**免费用户全面开放 Gemini Skills**，**Gems 功能将于 11 月完成整合**；延续多模态实时交互与面向政企的私有 AI 计算布局。

📌 **豆包（字节跳动）** — 个人助手独立 App 实锤，定名 **"小豆"**，剑指全场景智能生态；同步升级**一站式出行全流程**，进一步向生活服务入口延伸。

📌 **腾讯元宝（腾讯）** — 入局 **Personal Agent** 赛道，内部代号 **"Handy Bot"**，已在微信低调内测。

📌 **通义千问（阿里）** — 本周公开渠道未见重大新版本；国内侧延续 **Qwen3Guard** 安全护栏与 **Qwen-Image-Edit** 图像编辑能力。

📌 **Kimi（月之暗面）** — 最新旗舰仍为 **Kimi K3**（2.8 万亿参数、原生多模态、百万 token 上下文），本周无新版本。

📌 **DeepSeek** — 本周无新模型发布；延续 **DeepSeek-V4.1-Flash / deepseek-v4-pro** 的 API 服务，并向 Agent 生态推出 **DeepSeek Harness**（开发者预览，支持 Claude Code / Copilot / OpenCode 等后端直连）。

---

## 【ToB 智能体工厂】

📌 **Dify** — 最新版本仍为 **v1.17.1**（2026-09-10，本周无新 Release）
- **数据集级知识库 API Key**：Key 可绑定指定知识库，越权访问其他数据集（含 list-all）返回 403，解决"一个 key 通吃整个工作区"的权限问题。
- **工作流键盘操作**：节点 / 多选 / 评论标记支持方向键移动（Shift 大步），松键合并为一条撤销记录。
- **市场创作者主页 + 首页改版**：作者公开主页 `/marketplace/creator/`，首页重构为 hero + 轮播 + 吸顶搜索 + 标签筛选。
- ⚠️ **升级警示**：自托管内置 Weaviate 需从 1.27.0 **分阶段**升级到 1.39.2（跨 12 个 minor 版本），直接拉起重启可能永久损坏向量检索。
- 🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT** — 本周发布 **v4.17.1**（配套 fastgpt-plugin v1.1.4、AI Proxy v0.7.3），为本次周期内少见的**大版本级更新**：
- **管理员入口并入主应用**：商业版管理界面合并进 FastGPT 主应用，root 登录后从「管理员」进入系统配置（`/admin/settings/*`）、运营管理与 License 激活续期，旧路径不再保留；Pro 服务仍需保留，健康检查探测路径调整为 `/api/health`。
- **应用发布资源权限快照 + 运行时授权**：静态资源按发布时快照校验、动态资源按实际运行用户校验，解决协作开发下运行时权限分散问题。
- **知识库文件级权限（集合级权限）**：可按文件/文件夹单独配置协作者，支持继承与独立态、恢复继承、所有权转移；默认关闭，开启后列表/详情/检索召回逐条鉴权。
- **知识库标签管理与筛选**：支持类型化标签值、集合标签维护，并在工作流与 Agent V2 知识库搜索中使用标签条件（含 string 类型标签）。
- **系统模型健康探测与监控**：48 小时状态图可视化、告警 Webhook 与 Token，模型状态变动时通知。
- **安全修复**：修复 **MCP DNS rebinding 导致的 SSRF 风险**、收紧解析地址族校验；修复 **Markdown 渲染危险链接协议（javascript: 等）存储型点击 XSS**。
- 其他：应用 Token 统计看板、列表批量选择/移动/删除、支持 OFD 文件解析、SSO 密码策略、工作流新增 off 输入类型、OpenAPI 新增模型管理接口、`DISABLE_MARKETPLACE` 开关等。
- 🔗 https://github.com/labring/fastgpt/releases

---

## 【GitHub Trending AI 类】（本周）

💻 **debpalash/VoiceStudio** ⭐53.2k | ⬆️+14,689 | 完全本地的开源 ElevenLabs 替代（语音克隆/设计/配音/转录，646 种语言）
💻 **vectorize-io/hindsight** ⭐45.5k | ⬆️+10,623 | 会学习的 Agent 记忆系统（Agent Memory That Learns）
💻 **paperclipai/paperclip** ⭐97.2k | ⬆️+8,732 | 团队协作管理 Agent 的开源应用
💻 **NVIDIA/OpenShell** ⭐14.9k | ⬆️+5,996 | 面向自主 AI Agent 的安全、私有运行时（Rust）
💻 **rohitg00/ai-engineering-from-scratch** ⭐63.9k | ⬆️+4,904 | 从零学 AI 工程：Learn / Build / Ship
💻 **Panniantong/Agent-Reach** ⭐90.9k | ⬆️+4,789 | 给 Agent 装上"看整个互联网的眼睛"（Twitter/Reddit/YouTube/GitHub/B站/小红书，一个 CLI 零 API 费）
💻 **mvschwarz/openrig** ⭐5.0k | ⬆️+4,251 | 用 Claude Code / Codex / Pi 搭建自有 Agent 网络（持久团队、角色、共享上下文）
💻 **pbakaus/impeccable** ⭐76.3k | ⬆️+4,242 | 让 AI harness 更懂设计的"设计语言"
💻 **heygen-com/hyperframes** ⭐56.8k | ⬆️+3,096 | 写 HTML、渲染视频，为 Agent 而生
💻 **TencentCloud/Octop** ⭐6.7k | ⬆️+1,496 | 更聪明的自托管 AI 助手（多用户、多 Agent）
💻 **alirezarezvani/claude-skills** ⭐27.6k | ⬆️+1,024 | 380+ Claude Code / Agent Skills 与插件合集

> 趋势信号：本周 AI 榜继续由 **Agent 记忆 / Harness / 安全运行时 / 多 Agent 协作 / Skill 生态** 主导；"给 Agent 装能力（记忆、技能、安全、协作、网络访问）"与"Agent 团队编排"是最热方向，且多家（NVIDIA、腾讯）以**自托管 / 私有运行时**切入企业信任。

---

## 【arXiv cs.AI 亮点】（Agent / LLM / MCP 方向，10-01 批次）

🤖 **【工具调用】KaliBench** —— 面向 Kali Linux 的细粒度「自然语言→CLI」基准，覆盖 1,642 个工具、8,504 条 query-command 对；无提示下最强开源模型精确命令准确率**不足 42%**，并给出可无运行时验证的奖励用于训练（NeurIPS 2026）。
🤖 **【具身 Agent】Reconstruct, Practice, Go Real (RPG)** —— 不更新模型权重，通过离线数据重建练习任务 + 执行反馈诊断，自动演化可复用 Symbolic Skill 库，22 项操作任务成功率 **28.6%→95.0%**。
🤖 **【检索/科研 Agent】ScholarCatalyst** —— 以"作者标注哪些论文启发了本研究"构建检索基准；发现 **Agentic 搜索并不优于向量检索**（0.42 vs 0.48 R@20），指出模型缺乏专家式检索直觉，呼吁新训练配方。
🤖 **【实时 Avatar】GALA（Gaussian Blendshape Distillation）** —— 用线性 blendshape 蒸馏替代逐帧重神经解码，CPU 动画成本最高降三个数量级，移动端可达 60fps。

---

## 【Seaf 机会点】

💡 **1. 安全运行时的"企业级 Kubernetes"叙事升温，Seaf 可主打"可治理 Agent 运行时"。**
NVIDIA/OpenShell（自主 Agent 安全私有运行时，单周 +6k）与 OpenAI/红帽等推进的 **OCE 1.0（面向 AI 代理的企业级编排）** 共同表明：企业要的不只是"能编排 Agent"，而是**隔离、权限、审计、可私有化**的运行底座。Seaf 三个平台（开发/用户/管理）叠加 MCP/Skill 审核，天然贴近这一叙事，建议把**执行隔离 + 细粒度权限 + 审计**打包成"企业可托管 Agent 运行时"卖点。

💡 **2. 竞品在"知识库权限与安全"上正面加码，Seaf 需补齐知识库/资源的**逐条鉴权**能力。**
FastGPT v4.17.1 一次性补齐**知识库文件级权限（继承/独立/所有权转移）**、**应用发布资源权限快照**、并修复 **MCP SSRF** 与 **Markdown XSS**；Dify 则推**数据集级 API Key**。这已成 ToB 准入标配。Seaf 的知识库关联与 MCP/Skill 审核之外，建议补上**资源级 ACL（知识库/文件）+ 发布快照授权 + MCP 出网安全策略**，避免在企业安全评审中被拉开差距。

💡 **3. 记忆（Memory）与 Skill 生态仍是开源最热入口，Seaf 应把二者做成"可治理资产层"。**
**hindsight（会学习的 Agent 记忆）**单周 +10.6k、**claude-skills（380+ Skills）** 持续走热，配合 arXiv 检索/技能演化研究，说明"记忆 + 技能"正从 Demo 变成平台黏性资产。Seaf 可把**知识库 + 会话/长期记忆 + Skill 市场**统一为可审核、可溯源、可复用的"能力资产层"，用行业模板 + Skill 包加速企业冷启动。

💡 **4. 模型网关与内容安全持续抬高门槛，Seaf 需强化"统一模型治理 + 内容护栏"。**
DeepSeek 推 **Harness**、FastGPT 强制 AI Proxy 化、GPT-6.1 Astra 因安全预警被搁置——模型接入与安全治理正同步收紧。Seaf 建议在既有能力上补**统一模型网关（密钥/渠道/额度治理）+ 内容安全护栏 + 私有化数据面**，作为面向大型企业的准入级差异化。

---

*数据来源：GitHub Releases / GitHub Trending(weekly) / arXiv cs.AI / OpenAI News / Anthropic / Qwen Blog / DeepSeek API Docs / AIbase / 公开报道 | 2026-10-05*