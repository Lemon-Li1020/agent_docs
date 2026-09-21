# 🌐 Seaf 竞品周报 | 2026-09-21（第38期）

---

## 【ToC 智能体助手】

📌 **豆包（字节跳动）** — 本周公开渠道未披露重大版本；产品侧延续多模态理解、深度搜索与知识整理链路的迭代节奏（字节 Seed 官方博客本周无新模型发布）。

📌 **通义千问（阿里）** — Qwen 团队发布家族首个安全护栏模型 **Qwen3Guard**（支持 prompt/响应风险分级与分类，覆盖中英及多语种），并推出 **Qwen-Image-Edit**，把 Qwen-Image 的文本渲染与精确编辑能力延伸到图像编辑场景。

📌 **Kimi（月之暗面）** — 最新旗舰仍为 **Kimi K3**（2026-07-16 发布：2.8 万亿参数、原生多模态、百万 token 上下文），官方博客本周无新版本；产品主推长程编程、知识工作与深度推理。

📌 **DeepSeek** — **9 月 10 日发布 DeepSeek-V4.1-Flash**（新架构家族中的最小模型，原生多模态视觉理解），API 价格随之下调；官方确认 V4 Pro 的 API 服务在 9 月 14 日后继续提供、计费方式不变。同时提供 DeepSeek Harness 开发者预览。

📌 **ChatGPT（OpenAI）** — 9 月密集落地行业化与企业能力：**ChatGPT for Financial Services**（09-10）、企业数据打通用能力（*Now everyone can put data to work*，09-10）、**Astra for Law**（09-17）、广告业务 AI 重构（09-16）；工程侧披露存储系统已服务 **超 10 亿 ChatGPT 用户**（09-11）。

📌 **Gemini（Google DeepMind）** — 9 月发布 **Gemini 3.8 Flash / 3.8 Flash Cyber**、**Gemini 3.8 Live 及 Live Extended Thinking**，并上线 **Gemini 的 agentic 视频理解**能力，同时推进面向政企的主动式网络防御。

📌 **Claude（Anthropic）** — **9 月 10 日发布威胁情报报告《Detecting and countering misuse of AI: September 2026》**；8 月底公布对齐与安全改进进展，并将就此前 Claude 越权访问事件与 METR 合作开展独立审查。

---

## 【ToB 智能体工厂】

📌 **Dify** — 最新 **v1.17.1**（2026-09-10）
- **数据集级知识库 API Key**：API Key 可绑定到指定知识库，越权访问其他数据集返回 403，解决"一个 key 通吃整个工作区"的权限问题。
- **工作流键盘操作**：节点/多选/评论可用方向键移动（Shift 大步），一次按键生成一条撤销记录。
- **市场创作者主页 + 首页改版**：作者公开主页 `/marketplace/creator/<handle>`，首页重构为 hero + 轮播 + 吸顶搜索 + 标签筛选。
- ⚠️ **升级警示**：自托管内置 Weaviate 需从 1.27.0 **分阶段**升级到 1.39.2，跨 12 个 minor 版本，直接拉起重启可能永久损坏向量检索。
- v1.17.0（08-25）要点：Agent **E2B 沙箱后端**、**构建时 Home 快照**、**工作区级 Skill 管理**（草稿→发布→版本）、**上下文感知历史压缩**、工作流**可复用 LLM 环境变量**、Loop/迭代内**人工输入**、**统一 Tracing（Phoenix / LangSmith）**。
- 🔗 https://github.com/langgenius/dify/releases

📌 **FastGPT** — 最新 **v4.17.0**
- **强制接入 AI Proxy**：`OPENAI_BASE_URL` / `CHAT_API_KEY` 弃用移除，模型统一在渠道中治理，缺失配置将导致启动校验失败。
- **CSRF 防御**：新增 `CSRF_ENABLED`，防止外部（尤其 HTML 标签）携带 Cookie 直连接口。
- **SSO 扩展**：SSO Service 新增 **LDAP** 成员/组织架构同步与**钉钉**用户/部门同步。
- **Agent V2 语音播报（TTS）**：支持关闭/浏览器/模型播报，可选音色与语速。
- **自动系统升级任务管理**：多节点 lease 互斥 + 心跳，支持分批断点续跑与失败重试。
- 🔗 https://github.com/labring/fastgpt/releases

---

## 【GitHub Trending AI 类】（本周）

💻 **alibaba/open-code-review** ⭐38.4k | ⬆️+15,504 | 阿里大规模验证的混合架构代码评审工具（确定性流水线 + LLM Agent）
💻 **bilawalsidhu/gods-eye-view** ⭐39.6k | ⬆️+8,111 | 浏览器内基于真实数据的卫星空间情报模拟器
💻 **affaan-m/ECC** ⭐263.7k | ⬆️+6,453 | Agent harness 性能优化系统（Skills / 记忆 / 安全 / 研究优先）
💻 **stablyai/orca** ⭐73.6k | ⬆️+5,841 | 面向并行 Agent 舰队的 ADE（可用自有订阅运行任意编码 Agent）
💻 **ayghri/i-have-adhd** ⭐49.2k | ⬆️+5,249 | 让编码 Agent 不再"埋没答案"的 skill
💻 **Tencent/WeKnora** ⭐28.0k | ⬆️+5,242 | 开源 LLM 知识平台：文档→RAG + 推理 Agent + 自维护知识库
💻 **addyosmani/agent-skills** ⭐97.7k | ⬆️+3,986 | 生产级 Agent 工程技能集
💻 **Panniantong/Agent-Reach** ⭐83.8k | ⬆️+3,690 | 给 Agent 装上"全网眼睛"（Twitter/Reddit/YouTube/GitHub/B站/小红书）
💻 **blader/humanizer** ⭐50.6k | ⬆️+3,045 | 去除 AI 生成痕迹的写作 Agent skill
💻 **heygen-com/hyperframes** ⭐52.0k | ⬆️+2,546 | 写 HTML 渲染视频，为 Agent 而生的视频生成
💻 **microsoft/markitdown** ⭐185.9k | ⬆️+2,521 | 文件/办公文档转 Markdown 的 Python 工具
💻 **anthropics/claude-code** ⭐147.1k | ⬆️+2,342 | 终端内 Agentic 编码工具
💻 **danny-avila/LibreChat** ⭐44.5k | ⬆️+1,600 | 增强版 ChatGPT 克隆，支持 Agents / MCP / Skills / 多模型
💻 **mksglu/context-mode** ⭐23.8k | ⬆️+1,242 | 编码 Agent 上下文窗口优化（工具输出沙箱化，降约 98%）

> 趋势信号：本周 AI 榜几乎被 **Agent 工具链 / Skill / Harness / 上下文与记忆优化** 占据，"给 Agent 装能力（Skill / 眼睛 / 记忆 / 沙箱）"成为开源主流方向。

---

## 【arXiv cs.AI 亮点】（Agent / LLM 方向，9-17 批次）

🤖 **Agent Harness 正在成为研究热点**：*An Empirical Study of Harness Design for Coding Agents*、*How Do Agent Harnesses Create Value? Planning Information and Release Control*、*SoL-Pi: Recursively Scaling Auto-Research Loops for Efficient Agent Harness* —— 编排/脚手架工程被系统化研究。
🤖 **Chronicle: Cut-Point Replay for Regression Testing of LLM Agents** —— 面向 Agent 的回归测试与可复现回放。
🤖 **A Scalable Trust Discovery Architecture for the Internet of Agents** —— 多 Agent 互联的信任发现架构。
🤖 **Rethinking Multi-Agent Collaboration: When More Is Less** —— 反思"多 Agent 协作"，更多未必更好。
🤖 **RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents** —— 有状态 RAG 故障排查 Agent。
🤖 **UnifiedPlayers: Enhance Tool-Integrated Reasoning in Agentic RL** —— 工具调用与 Agentic RL 的融合训练。

---

## 【Seaf 机会点】

💡 **1. "Harness / 编排工程"正成为分水岭，Seaf 应主打工程化叙事。**
Dify 补上工作区级 Skill 管理与 E2B 沙箱、FastGPT 统一 AI Proxy 模型网关，arXiv 又集中出现 Harness 设计研究。Seaf 的「编排 Tab + Skill/MCP 发布-下架-审核流程」正好对标这一趋势，建议对外强化"可治理的 Agent 编排底座"叙事，并补齐沙箱执行、上下文压缩等运行底座能力。

💡 **2. Agent 可观测与回归测试是明显空白，Seaf 的日志能力可直接产品化。**
Chronicle（Agent 回归测试）、Dify 统一 Tracing 说明"看清 Agent 每一步"已成刚需。Seaf 已有**调用日志 + 日志回放 + Langfuse 执行链**，建议包装成差异化卖点——「Agent 执行链回放 + 回归对比」，这是多数竞品尚未覆盖的能力。

💡 **3. 企业安全合规需求上升，MCP/Skill 审核之外需要"内容安全 + 密钥治理"。**
FastGPT 强制 AI Proxy 与 CSRF 防御、Qwen3Guard 安全护栏、Anthropic 误用报告共同指向 ToB 的安全门槛。Seaf 可在既有的 MCP/Skill 审核流程之外，增加**模型网关/密钥治理 + 内容安全护栏**能力，形成对企业的信任卖点。

💡 **4. 生态入口竞争加剧，建议以"行业模板市场"加速冷启动。**
Anthropic 推出面向知识工作者的插件库（Claude Cowork）、OpenAI 密集行业化（法律 Astra for Law、金融 ChatGPT for Financial Services）。Seaf 可聚焦**垂直行业 Agent 模板市场**，用可复用模板降低企业上手门槛，抢占场景心智。

---

*数据来源：GitHub Releases / GitHub Trending(weekly) / arXiv cs.AI / OpenAI / Anthropic / Google DeepMind / Qwen / Moonshot / DeepSeek 官方渠道 | 2026-09-21*
