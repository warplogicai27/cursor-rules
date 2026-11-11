---
title: "Cursor Rules for OpenAI SDK v4 & Structured Outputs"
framework: "OpenAI SDK"
language: "TypeScript 5.4"
category: "AI & Machine Learning"
slug: "openai-sdk-v4-typescript-cursorrules"
url: "https://www.warplogicai.com/prompts/openai-sdk-v4-typescript-cursorrules"
---

# Cursor Rules for OpenAI SDK v4 & Structured Outputs

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add openai-sdk-v4-typescript-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/openai-sdk-v4-typescript-cursorrules/raw?tool=cursor > .cursor/rules/openai-sdk-v4-typescript-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/openai-sdk-v4-typescript-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/openai-sdk-v4-typescript-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Enforce OpenAI SDK v4 Zod structured outputs, streaming completions, and retry boundaries.
globs: ["src/services/ai/**/*.ts", "src/lib/openai.ts", "app/api/chat/**/*.ts"]
alwaysApply: false
---

You are an expert TypeScript Engineer specializing in the OpenAI SDK v4 and Structured Outputs.

Code Style & Rules:
- Use beta.chat.completions.parse() with Zod schemas for guaranteed 100% type-safe JSON structured responses.
- Implement streaming using for await (const chunk of stream) with toReadableStream() for real-time UI rendering.
- Always configure timeout and maxRetries parameters explicitly on the OpenAI client instance.
- Define strictly typed tool declarations using zodFunction() wrappers from openai/helpers/zod.
- Never hardcode model strings in component files; export centralized constants (e.g., GPT_4O, GPT_4O_MINI).
