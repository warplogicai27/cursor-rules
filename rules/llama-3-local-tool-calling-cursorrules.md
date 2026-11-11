---
title: "Llama 3.3 Local Tool Calling & Function Execution Rules"
framework: "Llama 3 / Ollama"
language: "Python / JSON"
category: "LLM System Prompts"
slug: "llama-3-local-tool-calling-cursorrules"
url: "https://www.warplogicai.com/prompts/llama-3-local-tool-calling-cursorrules"
---

# Llama 3.3 Local Tool Calling & Function Execution Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add llama-3-local-tool-calling-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/llama-3-local-tool-calling-cursorrules/raw?tool=cursor > .cursor/rules/llama-3-local-tool-calling-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/llama-3-local-tool-calling-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/llama-3-local-tool-calling-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an expert in Local LLM Deployment and Function Calling for Meta Llama 3.3 (Instruct) via Ollama, vLLM, and llama.cpp.

Formatting Directives:
- Enforce the official Llama 3 prompt template format: `<|begin_of_text|><|start_header_id|>system<|end_header_id|>...<|eot_id|>...`.
- Supply tool definitions in the system prompt inside `<tools>...</tools>` tags formatted as JSON arrays of OpenAI-compatible function specs.
- When the model decides to invoke a tool, parse `<tool_call>{"name": "...", "arguments": {...}}</tool_call>` output with strict JSON parsing and schema validation.
- Implement local context truncation and sliding window kv-cache retention to prevent out-of-memory errors on GPU inference nodes.
- Keep token costs at $0 by caching common embedding vectors in local ChromaDB / pgvector instances.
