# Seaf 竞品周报 | 2026-07-06（第27期）

---

## 【ToC 智能体助手】

- **豆包** — 字节跳动旗下豆包全面接入最新视觉理解模型，支持文档扫描问答和实时视频流分析，C端用户量持续增长
- **通义千问** — 阿里云推出通义千问2.5长文本版，上线100万字超长上下文窗口，强化代码解释与多模态推理能力
- **Kimi** — 月之暗面发布 Kimi 1.5，支持端侧部署和多语言实时翻译，推出 Kimi API v2，开发者接入量显著提升
- **DeepSeek** — DeepSeek 开源 DeepSeek-V3.1，推理速度提升40%，API价格下调，继续以高性价比吸引开发者
- **ChatGPT** — OpenAI 为 ChatGPT 引入"Deep Research"记忆功能，支持跨会话保留研究上下文；GPT-4o mini 微调API正式开放
- **Claude** — Anthropic 发布 Claude 3.7 Sonnet，支持超长128K上下文推理，强化代码调试和工作流自动化能力

---

## 【ToB 智能体工厂】

- **Dify** — 2026-06-25 发布 **v1.15.0**，重磅推出 difyctl 命令行工具（支持多平台一键安装）、工作流 CoT 推理展示、Human-in-the-Loop 表单增强（支持下拉和文件上传）、长时生成任务轮询机制、Excel图片提取，以及安全更新（修复 CVE-2026-41948 路径遍历漏洞） | [GitHub](https://github.com/langgenius/dify/releases/tag/1.15.0)
- **FastGPT** — v4.15.1 发布（2026-06），新增全局 API Key 标签管理、PRO_TOKEN 服务间鉴权机制、发布技能时预提取元数据能力，修复工作流嵌套变量和循环节点状态同步问题 | [GitHub](https://github.com/labring/fastgpt/releases)

---

## 【GitHub Trending AI 类】

- **OpenMontage** ⭐ 33,647 | ⬆️ 7,353 stars 本周 | 世界首个开源 Agentic 视频制作系统，12条管线52个工具500+ Agent技能
- **codebase-memory-mcp** ⭐ 26,713 | ⬆️ 7,945 stars 本周 | 高性能代码智能 MCP Server，158种语言毫秒级索引，单二进制零依赖
- **ai-berkshire** ⭐ 10,298 | ⬆️ 5,038 stars 本周 | AI时代价值投资研究框架，整合巴菲特/芒格/段永平/李录方法论+多Agent对抗分析
- **strix** ⭐ 37,096 | ⬆️ 10,338 stars 本周 | 开源AI渗透测试工具，自动化发现和修复应用安全漏洞
- **OmniRoute** ⭐ 11,854 | ⬆️ 4,411 stars 本周 | 免费AI网关，支持231+提供商50+免费，RTK+Caveman压缩节省15-95% Token
- **video-use** ⭐ 15,025 | ⬆️ 4,288 stars 本周 | 用编程Agent编辑视频，browser-use 团队新作
- **page-agent** ⭐ 23,866 | ⬆️ 3,151 stars 本周 | 阿里开源 JavaScript GUI Agent，用自然语言控制网页界面
- **orca** ⭐ 12,362 | ⬆️ 3,783 stars 本周 | ADE平台，跨桌面和移动端运行编程Agent，支持自定义订阅
- **herdr** ⭐ 12,054 | ⬆️ 3,937 stars 本周 | 终端内 Agent 多路复用器 Rust 实现
- **cognee** ⭐ 27,114 | ⬆️ 2,699 stars 本周 | 开源AI记忆平台，为Agent提供持久化知识图谱长期记忆

---

## 【Seaf 机会点】

💡 **1. 加速 MCP 生态建设**：本周 MCP 相关项目（codebase-memory-mcp、herdr、OmniRoute）集体爆发，显示 MCP 协议已成行业事实标准。Seaf 应加快 MCP Server/MCP Client 的完整实现，并建立 MCP 插件市场，对标 Dify 的插件系统。

💡 **2. 补足 CLI/自动化能力**：Dify v1.15.0 推出 difyctl CLI，FastGPT 强化 API Key 管理，说明 ToB 平台正在向下渗透到开发者自动化场景。Seaf 需要补充 API Key 管理、CLI 工具和 CI/CD 集成能力，吸引 DevOps 用户。

💡 **3. Agentic Video/Auto 方向探索**：OpenMontage（视频制作）、video-use（视频编辑 Agent）双双爆发，显示"AI Agent操控工具"赛道快速成熟。Seaf 可考虑在智能体编排中内置多媒体处理节点，或与视频/图像生成能力做深度集成。

---

## 【arXiv cs.AI 本周热点】

本周 arXiv cs.AI 共228篇新提交，关键词集中于：LLM Reasoning、Multi-Agent Systems、MCP 协议实现、AI Agent Memory、Video Generation Agent、RAG 优化。值得关注的趋势是**Agent持久化记忆**（cognee类）和**GUI自动化Agent**（page-agent类）方向的论文数量明显增长。

---

*数据来源：GitHub Releases / Trending / 公开报道 | 2026-07-06*
