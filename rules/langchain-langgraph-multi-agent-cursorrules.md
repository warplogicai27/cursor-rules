---
title: "LangGraph Multi-Agent Architecture .cursorrules"
framework: "LangGraph"
language: "TypeScript"
category: "AI & Machine Learning"
slug: "langchain-langgraph-multi-agent-cursorrules"
url: "https://www.warplogicai.com/prompts/langchain-langgraph-multi-agent-cursorrules"
---

# LangGraph Multi-Agent Architecture .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add langchain-langgraph-multi-agent-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/langchain-langgraph-multi-agent-cursorrules/raw?tool=cursor > .cursor/rules/langchain-langgraph-multi-agent-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/langchain-langgraph-multi-agent-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/langchain-langgraph-multi-agent-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# LangGraph Multi-Agent Workflows .cursorrules

## StateGraph Standards
- Explicitly annotate state interfaces: `const StateAnnotation = Annotation.Root({ messages: Annotation<BaseMessage[]>({ reducer: ... }) })`.
- Keep node functions pure: nodes take state, execute specialized agent LLM or tool logic, and return state updates.
- Route state dynamically via `addConditionalEdges(source, routerFunction, pathMap)`.
- Implement persistent memory checkpointers (`MemorySaver` or Postgres checkpointer) for multi-turn thread persistence.

