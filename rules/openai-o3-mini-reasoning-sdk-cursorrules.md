---
title: "OpenAI o3-mini & Reasoning Models .cursorrules"
framework: "OpenAI SDK"
language: "TypeScript"
category: "AI & Machine Learning"
slug: "openai-o3-mini-reasoning-sdk-cursorrules"
url: "https://www.warplogicai.com/prompts/openai-o3-mini-reasoning-sdk-cursorrules"
---

# OpenAI o3-mini & Reasoning Models .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add openai-o3-mini-reasoning-sdk-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/openai-o3-mini-reasoning-sdk-cursorrules/raw?tool=cursor > .cursor/rules/openai-o3-mini-reasoning-sdk-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/openai-o3-mini-reasoning-sdk-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/openai-o3-mini-reasoning-sdk-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# OpenAI o1 & o3-mini Reasoning .cursorrules

## Architecture
- Use `developer` role instead of `system` role when targeting OpenAI o-series reasoning models.
- Configure `reasoning_effort` ('low', 'medium', 'high') based on latency and complexity requirements.
- Do NOT pass `temperature`, `top_p`, or `presence_penalty` parameters as reasoning models handle exploration internally.
- Pair with Zod `zodResponseFormat` for zero-hallucination JSON schema guarantees.

