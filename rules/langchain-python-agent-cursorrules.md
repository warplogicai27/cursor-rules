---
title: "Production Cursor Rules for LangChain & LangGraph Agents"
framework: "LangChain"
language: "Python 3.12"
category: "AI & Machine Learning"
slug: "langchain-python-agent-cursorrules"
url: "https://www.warplogicai.com/prompts/langchain-python-agent-cursorrules"
---

# Production Cursor Rules for LangChain & LangGraph Agents

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add langchain-python-agent-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/langchain-python-agent-cursorrules/raw?tool=cursor > .cursor/rules/langchain-python-agent-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/langchain-python-agent-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/langchain-python-agent-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Enforce LangChain 0.2+ LCEL syntax, LangGraph stateful agent loops, and typed Pydantic tools.
globs: ["src/agents/**/*.py", "src/chains/**/*.py", "src/ai/**/*.py"]
alwaysApply: false
---

You are an expert AI Engineer specializing in LangChain 0.2+, LangGraph stateful agents, and LCEL (LangChain Expression Language).

Code Style & Rules:
- Always use LCEL (pipe operator |) for constructing prompt-to-model-to-parser chains.
- Use LangGraph StateGraph for complex, multi-actor workflows and stateful loops instead of legacy AgentExecutor.
- Require strict Pydantic v2 schemas for all tool input declarations (@tool decorator with descriptive docstrings).
- Ensure async execution using ainvoke(), astream(), and astream_events() for non-blocking I/O.
- Handle tool errors gracefully with Fallback configurations (with_fallbacks()) or LangGraph conditional edges.
