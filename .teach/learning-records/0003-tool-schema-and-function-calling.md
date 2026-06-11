# Learning Record: 0003-tool-schema-and-function-calling

## Date
2026-06-11

## Lesson
[L0003 - Tool Schema 与结构化输出](../lessons/0003-tool-schema-and-function-calling.html)

## Key Insights

1. **Tool Call 本质是 RPC**：LLM 不执行函数，只输出调用意图（函数名 + 参数 JSON）。代码执行后把结果喂回去。
2. **Tool Schema ≈ OpenAPI Spec**：name = 接口路径，description = 接口描述，parameters/input_schema = 请求参数。
3. **三大坑**：
   - OpenAI `parameters` vs Anthropic `input_schema`（字段名不同）
   - OpenAI `arguments` 是字符串（需 json.loads）vs Anthropic `input` 是 dict
   - 回传结果 role 不同：OpenAI 用 `"tool"`，Anthropic 用 `"user"`
4. **完整数据流**：发 messages+tools → 收 tool_call → 执行 → 回传 tool_result → 再调 LLM 得最终答案

## Analogies That Clicked
- Tool Call ≈ RPC（LLM 是客户端，代码是服务端）
- Tool Schema ≈ Swagger/OpenAPI 接口契约
- Agent Loop = 反复做 Tool Call 流程

## Interview Ready
- 能画出 Tool Call 完整数据流（5 步）
- 能说清 OpenAI 和 Anthropic 的 3 个关键差异
- 能解释 "LLM 不执行函数，只表达意图"

## Next
L0004 - 手写最小 Agent Loop
