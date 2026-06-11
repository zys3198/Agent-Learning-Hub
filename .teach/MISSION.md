# Mission: AI Agent 应用开发工程师面试准备

## Why
Java 后端工程师转型 AI Agent 方向，目标是通过 AI Agent 相关技术面试，成为资深 Java+AI 开发工程师。不是转行做算法研究，而是在工程层面掌握 agent 构建能力——能设计、实现、调试、评测一个真实 agent 系统。

## Success looks like
- 能手写一个最小 agent loop（含 tool call、错误处理、最大步数限制）
- 能解释 Claude Code / Codex 类 coding agent 的 harness 架构：工具协议、权限、上下文压缩、subagents
- 能说清 MCP / A2A / ACP / Skills 各解决什么问题，怎么协作
- 能设计一个带 eval、trace、权限边界的 agent 系统，并在面试白板上画出架构
- 能对比单 agent vs 多 agent 的取舍，说清什么时候该用哪个
- 能用 Java 或 Python 实现一个 RAG pipeline（chunk → embed → retrieve → answer with citations）

## Constraints
- 每天 4-5 小时，每周 7 天，约 30-35h/周
- Java 后端背景，Python 能用但不精通
- 面试导向——需要能说清楚原理和 tradeoff，不只是跑通 demo
- 偏重应用开发 + 必要的 AI 原理，不深入算法/训练/数学推导

## Out of scope
- LLM 训练与微调（fine-tuning 的高阶细节）
- 纯学术研究方向（RL 理论、transformer 数学推导）
- 非 Java/Python 生态的框架（Go agent 框架等）
- 浏览器自动化 agent（Stage 6，优先级低，面试不太考）

## Roadmap alignment
基于 README.md 的 9 阶段路线图，按面试价值重新排序：
1. **Stage 0-1**：基础概念 + 最小 agent loop（必须扎实）
2. **Stage 2**：RAG + Tool Use + Memory（面试高频）
3. **Stage 3**：现代 Agent Harness（Claude Code / OpenClaw 架构理解）
4. **Stage 5**：Skills / MCP / A2A / ACP 协议（架构设计题）
5. **Stage 4**：Multi-Agent 协调（高级话题）
6. **Stage 7**：评测、可观测性、安全（工程化加分项）
7. **Stage 8**：交付一个真实 agent 项目（作品集）
