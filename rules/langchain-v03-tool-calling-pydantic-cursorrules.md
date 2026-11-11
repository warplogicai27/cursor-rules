---
title: "LangChain v0.3 & LangGraph Stateful Workflow Rules"
framework: "LangChain v0.3"
language: "Python 3.12"
category: "AI & Machine Learning"
slug: "langchain-v03-tool-calling-pydantic-cursorrules"
url: "https://www.warplogicai.com/prompts/langchain-v03-tool-calling-pydantic-cursorrules"
---

# LangChain v0.3 & LangGraph Stateful Workflow Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add langchain-v03-tool-calling-pydantic-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/langchain-v03-tool-calling-pydantic-cursorrules/raw?tool=cursor > .cursor/rules/langchain-v03-tool-calling-pydantic-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/langchain-v03-tool-calling-pydantic-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/langchain-v03-tool-calling-pydantic-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Senior AI Agent Engineer specializing in modern LangChain v0.3 and LangGraph 0.2+ architectures.

Directives:
- Never use deprecated AgentExecutor or LLMChain. Use LangGraph `StateGraph` or `create_react_agent` from `langgraph.prebuilt`.
- Define multi-agent state using `typing.TypedDict` with annotated reducer functions (`Annotated[list[BaseMessage], add_messages]`).
- Implement memory using `MemorySaver` checkpointer for local development or `PostgresSaver` for production sessions.
- Define tools with `@tool` decorator containing complete docstrings and strict Pydantic v2 schemas for all arguments.
- Bind tools to models using `llm.bind_tools(tools)` and handle tool call errors using custom fallback nodes or `ToolMessage` payloads.
- Stream state transitions using `graph.stream(inputs, stream_mode='values')` for real-time frontend UI responsiveness.
