# Teaching Notes

## User profile
- Java 后端工程师，熟悉 Spring / MySQL / Redis 等技术栈
- Python 能用但不精通
- 大概知道 LLM 原理和基础 API 调用
- 面试导向，需要能讲清原理和 tradeoff

## Teaching preferences
- 用 Java/后端类比解释 AI 概念（如：tool call ≈ RPC，agent loop ≈ 事件循环）
- 每个概念配面试角度："面试官会怎么问？"
- 代码示例优先 Python（agent 生态主流），Java 版本作为参考
- 偏重应用开发 + 必要原理，不深入数学推导
- 课程配图一律用 `lesson-svg-diagram` skill 画内联 SVG，禁止 ASCII 字符画（┌─┐│└┘）。配色锁课程主题蓝系，模板见 skill REFERENCE.md

## Progress tracking
- 课程大纲：完成（reference/course-syllabus.html）
- Stage 0: ✅ 完成（L0001）
- Stage 1: ✅ 完成
  - L1.1 LLM API 基础调用：✅ 完成（L0002）
  - L1.2 Tool Schema 与结构化输出：✅ 完成（L0003）
  - L1.3 最小 Agent Loop：✅ 完成（L0004）
  - L1.4 健壮性处理：✅ 完成（L0005）
- Stage 2: ✅ 完成
  - L2.1 RAG Pipeline 全流程：✅ 完成（L0006）
  - L2.2 多样化工具接入：✅ 完成（L0007）
  - L2.3 记忆系统设计：✅ 完成（L0008）
  - L2.4 RAG Agent 常见问题：✅ 完成（L0009）
- Stage 3-8: 未开始

## References created
- reference/glossary.html — 术语速查
- reference/llm-api-quick-ref.html — LLM API 速查（OpenAI + Anthropic）
- reference/course-syllabus.html — 课程大纲

## Lessons
- L0001: Agent 概念辨析（Chatbot vs Workflow vs Agent vs Multi-Agent）
- L0002: LLM API 基础调用（curl + Python SDK + 参数调优）
- L0003: Tool Schema 与结构化输出（Tool Call 数据流 + OpenAI/Anthropic 差异）
- L0004: 手写最小 Agent Loop（calculator + search，messages 变化追踪）
- L0005: Agent 健壮性处理（MAX_STEPS + 超时 + 错误回传 + 安全执行）
- L0006: RAG Pipeline 全流程（加载→分块→向量化→检索→重排→生成）
- L0007: 多样化工具接入（搜索/SQL/文件/代码执行 + 四原则 + 安全）
- L0008: 记忆系统设计（短期/会话/长期三层架构 + 摘要压缩 + 持久化）
- L0009: RAG Agent 常见问题（幻觉引用/空结果/重复调用/防御策略）
