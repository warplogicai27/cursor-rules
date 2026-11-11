---
title: "Anthropic Claude 3.5 Sonnet Prompt Architecture .cursorrules"
framework: "Anthropic SDK"
language: "TypeScript"
category: "AI & Machine Learning"
slug: "anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules"
url: "https://www.warplogicai.com/prompts/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules"
---

# Anthropic Claude 3.5 Sonnet Prompt Architecture .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules/raw?tool=cursor > .cursor/rules/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/anthropic-claude-3-5-sonnet-prompt-engineering-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Anthropic Claude 3.5 Sonnet System Prompt .cursorrules

## Prompt Engineering Principles
- Enclose instructions and dynamic context in structured XML tags (`<instructions>`, `<context>`, `<rules>`, `<schema>`).
- Instruct Claude to output structured JSON or strict code within dedicated blocks without conversational fluff.
- When defining tools, provide comprehensive descriptions for both the tool purpose and each schema parameter.
- Enforce chain-of-thought (CoT) inside `<thinking>` tags for complex mathematical, architectural, or logic transformations.

