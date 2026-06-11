# Learning Record: 0002-llm-api-first-call

## Date
2026-06-11

## Lesson
[L0002 - LLM API 基础调用](../lessons/0002-llm-api-basics.html)

## Key Insights

1. **LLM API 本质是 HTTP 请求**：SDK 只是封装，底层是 POST JSON → 拿回 JSON。类比 RestTemplate。
2. **messages 数组是无状态的**：每次请求要传完整历史，不传就"失忆"。context window 限制了历史长度。
3. **OpenAI vs Anthropic 三大坑**：
   - system 消息位置不同（messages 内 vs 独立参数）
   - Anthropic max_tokens 必填
   - 响应结构不同（choices[0].message.content vs content[0].text）
4. **temperature=0 不保证完全确定性**：只是选概率最高的 token，理论上相同输入同输出，但不同模型版本可能有差异。

## Analogies That Clicked
- 调 LLM API ≈ 调 REST 接口（SDK ≈ RestTemplate）
- messages ≈ Session 聊天历史（但无状态，每次全传）
- temperature ≈ 数据库隔离级别（0=SERIALIZABLE, 1=READ COMMITTED）

## Interview Ready
- 能说清 OpenAI 和 Anthropic API 的 5 个关键差异
- 能解释 temperature/max_tokens 的实际效果和选择依据
- 能解释为什么 messages 是无状态的

## Next
L0003 - Tool Schema 与结构化输出
