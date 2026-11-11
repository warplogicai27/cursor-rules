---
title: "Cursor Rules for Anthropic Claude SDK & Prompt Caching"
framework: "Anthropic SDK"
language: "Python 3.12 / TS"
category: "AI & Machine Learning"
slug: "anthropic-claude-sdk-cursorrules"
url: "https://www.warplogicai.com/prompts/anthropic-claude-sdk-cursorrules"
---

# Cursor Rules for Anthropic Claude SDK & Prompt Caching

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add anthropic-claude-sdk-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-sdk-cursorrules/raw?tool=cursor > .cursor/rules/anthropic-claude-sdk-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-sdk-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-sdk-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Enforce Anthropic Claude 3.5 Sonnet prompt caching, XML structure, and tool-use loops.
globs: ["src/ai/claude/**/*.py", "src/lib/claude.ts", "services/llm/claude*.py"]
alwaysApply: false
---

You are an expert AI Engineer specializing in Anthropic Claude 3.5 Sonnet API integration and Prompt Caching.

Code Style & Rules:
- Structure prompts with explicit XML tags (<context>, <instructions>, <examples>) for optimal Claude adherence.
- Enable Prompt Caching (cache_control: {"type": "ephemeral"}) on large system prompts (>1,024 tokens) to reduce latency by 80% and cost by 90%.
- Use anthropic.types.MessageParam and TextBlock type definitions for complete type safety.
- Handle tool_use stop_reasons explicitly in conversational agent loops.
- Implement exponential backoff retries for RateLimitError (429) and OverloadedError (529).
