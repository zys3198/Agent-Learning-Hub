# AI Agent 学习资源

## Knowledge

### 基础概念（Stage 0-1）
- [Anthropic: Building effective agents](https://www.anthropic.com/engineering/building-effective-agents)
  Agent 设计入门必读。讲清 workflow vs agent 边界。面试第一题常考。
- [OpenAI: A practical guide to building agents](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/)
  面向产品和工程团队的 agent 落地指南。和 Anthropic 的文章对照读。
- [OpenAI Function Calling](https://platform.openai.com/docs/guides/function-calling)
  Tool call 机制官方文档。实现 agent loop 必读。
- [Claude Tool Use](https://docs.anthropic.com/en/docs/agents-and-tools/tool-use/overview)
  Claude 侧工具调用。和 OpenAI 的对比理解。
- [Gemini Function Calling](https://ai.google.dev/gemini-api/docs/function-calling)
  第三家 API 对比，面试加分。

### RAG + Tool Use + Memory（Stage 2）
- [Model Context Protocol](https://modelcontextprotocol.io/)
  Agent 连接工具/数据源的标准协议。面试必考。
- [LlamaIndex Agents](https://docs.llamaindex.ai/en/stable/use_cases/agents/)
  RAG + Agent 结合的参考实现。
- [mem0](https://github.com/mem0ai/mem0)
  记忆层组件。学长期 memory 怎么设计。

### Agent Harness 架构（Stage 3）
- [Claude Code Docs](https://code.claude.com/docs/en/overview)
  最值得研究的 coding agent 产品文档。
- [Claude Code Subagents](https://code.claude.com/docs/en/sub-agents)
  任务拆分、上下文隔离、子代理。
- [Claude Code Hooks](https://code.claude.com/docs/en/hooks)
  拦截、校验、扩展 agent 行为。
- [learn-claude-code](https://github.com/shareAI-lab/learn-claude-code)
  从 0 到 1 复刻 Claude Code-like harness。
- [claw0](https://github.com/shareAI-lab/claw0)
  从 agent loop 构建到 gateway、session、memory。

### 协议与 Skills（Stage 5）
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
  Skill 文件结构和触发机制。
- [Agent2Agent Protocol](https://a2a-protocol.org/latest/specification/)
  Agent 间发现、通信、协作。
- [Agent Client Protocol](https://agentclientprotocol.com/)
  Agent 与宿主应用间统一接口。

### 评测与安全（Stage 7）
- [SWE-bench](https://arxiv.org/abs/2310.06770)
  真实 GitHub issue 修复评测。理解 eval 怎么做。
- [AgentBench](https://arxiv.org/abs/2308.03688)
  Agent 能力评测 benchmark。

### 论文（面试加分）
- [ReAct](https://arxiv.org/abs/2210.03629) — Reasoning + acting 基础范式
- [Reflexion](https://arxiv.org/abs/2303.11366) — 语言反馈和自我改进
- [Dive into Claude Code](https://arxiv.org/abs/2604.14228) — Coding agent harness 分析
- [AI Harness Engineering](https://arxiv.org/abs/2605.13357) — Harness 作为 agent 能力来源

## Wisdom (Communities)

- [Datawhale](https://github.com/datawhalechina)
  中文 AI 学习社区，有 hello-agents 等教程项目。
- [GitHub Discussions: langchain-ai/langgraph](https://github.com/langchain-ai/langgraph/discussions)
  Agent 工程实践讨论。

## Gaps

- Java 生态的 agent 框架参考较少（Spring AI / LangChain4j），需补充
- 缺少面试真题库，需在学习过程中积累
