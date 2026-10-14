# 🎯 AI Agent 开源技能全景总结

[![收录技能](https://img.shields.io/badge/收录技能-33-blue?style=flat-square)](#分类目录)
[![覆盖领域](https://img.shields.io/badge/覆盖领域-4-green?style=flat-square)](#分类目录)
[![许可证](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)
[![语言](https://img.shields.io/badge/语言-中文-red?style=flat-square)](#)

收录**最全、可核验**的开源 AI Agent 能力模块总结，覆盖 **🧠 通用 Agent 框架、💻 编程 Agent、🔬 科研 Agent、🏢 企业自动化** 四大领域，涵盖 Claude / OpenAI / LangChain / CrewAI / AutoGen / Semantic Kernel / Dify / n8n 等不限框架的 Agent Skill、MCP Server、Tools / Plugin、工作流节点等**可被 AI Agent 调用、集成、复用的开源能力**。

---

## 📊 统计数据

- **收录条目**：33 个（详细核验）+ 8 个（附录候选）
- **覆盖领域**：4 大领域 + MCP 基础设施 + 文档处理

## 🌟 主要发现

1. **Agent Skills（`SKILL.md` 范式）是 2025–2026 增长最快的生态**：`anthropics/skills` 官方仓库 star 达 18 万+，社区涌现 `addyosmani/agent-skills`、`VoltAgent/awesome-agent-skills`、`K-Dense-AI/scientific-agent-skills` 等高 star 集合。
2. **MCP（Model Context Protocol）成为跨框架的「工具互联标准」**：官方参考服务器仓库 star 9.1 万+，`awesome-mcp-servers` 等超大精选列表持续增长。
3. **多 Agent 框架进入洗牌期**：Microsoft 将 AutoGen 与 Semantic Kernel 收敛到 **Microsoft Agent Framework (MAF)**；`microsoft/autogen` 已进入维护模式（LICENSE 变更为 CC-BY-4.0）。
4. **「开源」与「source-available」需严格区分**：`claude-code`（专有）、`n8n`（Sustainable Use License）、`Dify`（修改版 Apache-2.0）、`Flowise`/`LiteLLM`（核心开源 + enterprise 闭源）等，商用前须逐个确认。
5. **企业自动化工作流**：`n8n`（20.7 万 star）、`Dify`（15.8 万 star）是自我托管工作流/Agent 平台两大代表。

---

## 🗂️ 分类目录

| 分类                     | 数量 | 说明                                                             |
| ------------------------ | ---- | ---------------------------------------------------------------- |
| 🧠 通用 AI Agent 框架    | 12   | LangChain、LangGraph、OpenAI/Google SDK、多 Agent 框架、模型网关 |
| 💻 编程 Agent 与工程技能 | 8    | Claude Code、官方 Skills、MCP 工具、代码沙箱、文档注入           |
| 🔌 MCP 工具互联          | 3    | MCP 协议规范、参考服务器、框架适配器                             |
| 🔬 科研 Agent            | 1    | 科研专用 skills（文献检索/数据分析/论文写作）                    |
| 🏢 企业自动化与工作流    | 6    | Dify、n8n、Flowise、Composio、浏览器自动化                       |
| 📄 文档处理与精选列表    | 3    | MarkItDown、MCP/Agent Skills 精选索引                            |

---

## 📚 分类详表

### 🧠 通用 AI Agent 框架（12）

- **langchain-ai/langchain** ⭐⭐⭐⭐⭐ - 最主流的 Agent 工程平台，海量工具/模型/集成抽象
- **langchain-ai/langgraph** ⭐⭐⭐⭐⭐ - 有状态、可控的 Agent 图编排运行时
- **openai/openai-agents-python** ⭐⭐⭐⭐⭐ - OpenAI 官方多 Agent 框架（tools/handoffs/guardrails/tracing）
- **run-llama/llama_index** ⭐⭐⭐⭐ - RAG/数据 Agent 框架，丰富 data connectors 与 tools
- **crewAIInc/crewAI** ⭐⭐⭐⭐ - 基于角色的多 Agent 协作框架
- **google/adk-python** ⭐⭐⭐⭐ - Google Agent Development Kit，可组合 Agent+工具
- **microsoft/semantic-kernel** ⭐⭐⭐⭐ - 企业级 Agent SDK，Plugin/OpenAPI/MCP 插件体系
- **microsoft/agent-framework** ⭐⭐⭐⭐ - 微软新一代企业 Agent 框架（AutoGen/SK 收敛目标）
- **block/goose** ⭐⭐⭐⭐ - Block 开源本地 AI Agent，支持 MCP 扩展
- **vercel/ai** ⭐⭐⭐⭐ - TypeScript AI SDK，统一多 provider 的 tool/agent 调用
- **BerriAI/litellm** ⭐⭐⭐⭐ - 统一 100+ LLM 的 API 网关，含 tool calling
- **microsoft/autogen** ⭐⭐⭐ - 多 Agent 对话框架（⚠️ 已进入维护期，被 MAF 取代）

### 💻 编程 Agent 与工程技能（8）

- **anthropics/claude-code** ⭐⭐⭐⭐⭐ - Anthropic 官方终端编程 Agent CLI（⚠️ 专有 source-available）
- **anthropics/skills** ⭐⭐⭐⭐⭐ - 官方 Agent Skills 仓库，SKILL.md 范式与 19 个示例
- **github/github-mcp-server** ⭐⭐⭐⭐⭐ - GitHub 官方 MCP，读写 issues/PR/代码/Actions
- **addyosmani/agent-skills** ⭐⭐⭐⭐ - 生产级工程 skills（代码审查/重构/测试/架构）
- **upstash/context7** ⭐⭐⭐⭐ - 为 LLM/编辑器注入实时最新库文档
- **e2b-dev/code-interpreter** ⭐⭐⭐⭐ - 安全沙箱执行 AI 生成代码
- **ChromeDevTools/chrome-devtools-mcp** ⭐⭐⭐⭐ - 官方 MCP，自动化/调试浏览器
- **crewAIInc/crewAI-tools** ⭐⭐⭐ - CrewAI 官方工具库（⚠️ 更新放缓）

### 🔌 MCP 工具互联（3）

- **modelcontextprotocol/servers** ⭐⭐⭐⭐⭐ - MCP 官方参考服务器集合
- **modelcontextprotocol/modelcontextprotocol** ⭐⭐⭐⭐⭐ - MCP 协议规范与各语言 SDK
- **langchain-ai/langchain-mcp-adapters** ⭐⭐⭐⭐ - 将 MCP 工具转成 LangChain Tools

### 🔬 科研 Agent（1）

- **K-Dense-AI/scientific-agent-skills** ⭐⭐⭐ - 面向科研的 177+ 个 ready-to-use skills（文献检索/数据分析/论文写作/实验设计）

> 💡 科研场景推荐组合：`K-Dense-AI/scientific-agent-skills` + `e2b-dev/code-interpreter`（沙箱跑代码）+ `microsoft/markitdown`（文献转文本）+ `run-llama/llama_index`（RAG 建库）。附录另见 `yenanjing/awesome-ai-for-science`（485 个科研自动化仓库）。

### 🏢 企业自动化与工作流（6）

- **n8n-io/n8n** ⭐⭐⭐⭐⭐ - 400+ 集成的可视化工作流自动化（⚠️ fair-code 非 OSI）
- **langgenius/dify** ⭐⭐⭐⭐⭐ - 可视化 Agent 工作流与 RAG 平台（⚠️ 修改版 Apache-2.0）
- **browser-use/browser-use** ⭐⭐⭐⭐⭐ - 让 LLM 通过真实浏览器与网页交互
- **FlowiseAI/Flowise** ⭐⭐⭐⭐ - 拖拽式 LLM 应用/Agent 编排
- **ComposioHQ/composio** ⭐⭐⭐⭐ - 250+ SaaS 工具/API 集成
- **langgenius/dify-plugins** ⭐⭐⭐ - Dify 官方插件市场分发仓库

### 📄 文档处理与精选列表（3）

- **microsoft/markitdown** ⭐⭐⭐⭐⭐ - PDF/Office/图片/音频 → Markdown，供 LLM 读取
- **punkpeye/awesome-mcp-servers** ⭐⭐⭐⭐ - 数千个 MCP server 的分类精选列表
- **VoltAgent/awesome-agent-skills** ⭐⭐⭐⭐ - 1000+ 官方/社区 agent skills 精选索引

---

## 🚀 快速开始

```bash
# 1. 克隆仓库
git clone https://github.com/WangJingyao07/Awesome-Skill.git
cd agent-skill-store

# 2. 读取结构化数据（机器可读，含 stars/许可证/评级/安装方式）
cat data/skills.json

# 3. 用 jq 快速筛选，例如只看五星项目
jq '.skills[] | select(.rating == 5) | {name: .full_name, stars, license}' data/skills.json

# 4. 按领域筛选（general / coding / mcp / research / enterprise / docs）
jq '.skills[] | select(.category == "research")' data/skills.json
```

## 📊 数据格式

`data/skills.json` 由三部分组成：`metadata`（元信息）、`skills`（33 条核验条目）、`appendix`（8 条候选）+ `scenarios`（10 个场景推荐）。单条 skill 结构如下：

```json
{
  "full_name": "langchain-ai/langchain",
  "url": "https://github.com/langchain-ai/langchain",
  "category": "general",
  "one_line": "最主流的 Agent 工程平台，提供海量工具/模型/集成抽象",
  "frameworks": ["LangChain 生态"],
  "license": "MIT",
  "openness": "open",
  "license_note": null,
  "stars": 147816,
  "forks": 24792,
  "updated_at": "2026-10-13",
  "rating": 5,
  "source": "official",
  "maintainer": "LangChain（官方）",
  "install": "pip install langchain",
  "limitations": "抽象层较多，学习曲线陡；版本迭代快"
}
```

字段说明：

| 字段         | 含义             | 取值                                                                          |
| ------------ | ---------------- | ----------------------------------------------------------------------------- |
| `category` | 领域分类         | `general` / `coding` / `mcp` / `research` / `enterprise` / `docs` |
| `openness` | 开源度           | `open` / `source-available` / `fair-code` / `mixed` / `unverified`  |
| `source`   | 维护来源         | `official`（官方）/ `community`（社区）                                   |
| `rating`   | 推荐指数（主观） | `5` / `4` / `3`                                                         |

---

## 🎯 五星推荐（⭐ 12 个）

1. **anthropics/skills** - 官方 Agent Skills 范式的事实标准
2. **anthropics/claude-code** - 编程 Agent 生态核心宿主（⚠️ 专有）
3. **langchain-ai/langchain** - 生态最全的 Agent 工程平台
4. **langchain-ai/langgraph** - 复杂 Agent 控制流编排首选
5. **openai/openai-agents-python** - OpenAI 侧 Agent 工具权威实现
6. **modelcontextprotocol/servers** - MCP 生态地基
7. **modelcontextprotocol/modelcontextprotocol** - MCP 协议与 SDK
8. **github/github-mcp-server** - 编程 Agent 高频工具
9. **microsoft/markitdown** - 文档/知识库场景实用工具
10. **langgenius/dify** - 企业自动化低代码 Agent 代表
11. **n8n-io/n8n** - 集成最广的工作流自动化（⚠️ fair-code）
12. **browser-use/browser-use** - 网页浏览与自动化首选

---

## 🔗 按场景推荐

| 场景                       | 推荐组合                                                                                                            |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **网页搜索与浏览**   | `browser-use/browser-use` + `ChromeDevTools/chrome-devtools-mcp` + `github/github-mcp-server`                 |
| **文件与代码操作**   | `modelcontextprotocol/servers`（Filesystem/Git）+ `github/github-mcp-server` + `anthropics/claude-code`       |
| **数据库与知识库**   | `run-llama/llama_index` / `langchain-ai/langchain` + DB MCP + `microsoft/markitdown`                          |
| **API 与 SaaS 集成** | `ComposioHQ/composio` + `langchain-ai/langchain-mcp-adapters` + `microsoft/semantic-kernel`                   |
| **多模态处理**       | `microsoft/markitdown`（OCR/转录）                                                                                |
| **多 Agent 协作**    | `crewAIInc/crewAI` / `microsoft/agent-framework` / `openai/openai-agents-python` + `langchain-ai/langgraph` |
| **自动化工作流**     | `n8n-io/n8n` / `langgenius/dify` + `langgenius/dify-plugins`                                                  |
| **科研与数据分析**   | `K-Dense-AI/scientific-agent-skills` + `e2b-dev/code-interpreter` + `microsoft/markitdown`                    |
| **安全与合规**       | `e2b-dev/code-interpreter`（沙箱隔离）+ 最小权限 + 代理网关限流                                                   |
| **代码补全/文档**    | `upstash/context7` + `addyosmani/agent-skills` + `VoltAgent/awesome-agent-skills`                             |

---

## ⚠️ 风险与合规提示

1. **许可证风险（最重要）**：
   - `anthropics/claude-code`、`anthropics/claude-agent-sdk` 为 **Anthropic 商业条款（source-available，非开源）**。
   - `n8n` 为 **Sustainable Use License（fair-code）**：以「向第三方提供 SaaS」方式商用受限。
   - `dify` 为 **修改版 Apache-2.0**：多租户 SaaS 需商业许可。
   - `Flowise`、`litellm` 为 **核心开源 + enterprise 目录闭源** 的混合模式，二次分发需剔除 enterprise 部分。
   - `microsoft/autogen` 为 **CC-BY-4.0**，且已进入维护期。
   - `anthropics/skills` 无统一许可证，**文档类 skill 为 source-available**。
   - `modelcontextprotocol/*` 处于 **MIT → Apache-2.0 过渡**。
2. **API Key 管理**：环境变量注入、密钥管理器、按 scope 最小授权、定期轮换；避免硬编码进 `SKILL.md` 或代码。
3. **数据隐私**：`Composio`、`litellm` 代理、云托管 MCP 会经过第三方；涉及客户数据优先自托管。
4. **提示注入**：Agent 读取的外部内容可能携带恶意指令，需 sanitize + guardrails。
5. **供应链安全**：社区 skills 列表可能混入恶意脚本，安装前审查来源、优先官方/高 star 项目。
6. **信息时效**：本文 star/forks/release 为 2026-10-14 快照，决策前以仓库当前状态为准。

---

## 📝 更新日志

### v1.0 (2026-10-14)

- 🎉 初始版本发布
- 📊 收录 33 条核验条目 + 8 条附录候选
- 🗂️ 建立 6 大分类（4 领域 + MCP + 文档/列表）
- 🔍 全部条目经 GitHub API + LICENSE 直读 + releases 源交叉核验
- 📦 提供 `data/skills.json` 结构化数据 + 10 个场景推荐

---

## 📄 许可证

[MIT](./LICENSE)

## 🙏 致谢

- [anthropics/skills](https://github.com/anthropics/skills) - Agent Skills 范式来源
- [anbeime/skill](https://github.com/anbeime/skill) - 本仓库样式参考
- 所有被收录项目及其维护团队
