---
title: "Elixir Phoenix LiveView 1.0 Production Cursor Rules"
framework: "Phoenix LiveView"
language: "Elixir"
category: "Fullstack & Real-Time"
slug: "elixir-phoenix-liveview-cursorrules"
url: "https://www.warplogicai.com/prompts/elixir-phoenix-liveview-cursorrules"
---

# Elixir Phoenix LiveView 1.0 Production Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add elixir-phoenix-liveview-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/elixir-phoenix-liveview-cursorrules/raw?tool=cursor > .cursor/rules/elixir-phoenix-liveview-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/elixir-phoenix-liveview-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/elixir-phoenix-liveview-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Elixir Phoenix LiveView 1.0 Production Rules
globs: ["lib/**/*"]
alwaysApply: true
---

# Elixir Phoenix LiveView 1.0 Architecture

You are a Principal BEAM / Elixir Architect.

## 1. LiveView 1.0 Idioms
- Use `stream/3` and `stream_insert/4` for large or dynamic collections to avoid heavy client DOM memory.
- Delegate complex business processes to dedicated GenServer workers or Task.async calls.

## 2. State & PubSub
- Use Phoenix.PubSub for real-time broadcasts across distributed nodes.
