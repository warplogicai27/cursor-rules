---
title: "SvelteKit 5 Runes & Tailwind v4 Production Cursor Rules"
framework: "SvelteKit"
language: "TypeScript"
category: "Frontend Frameworks"
slug: "sveltekit-5-runes-tailwind-v4-cursorrules"
url: "https://www.warplogicai.com/prompts/sveltekit-5-runes-tailwind-v4-cursorrules"
---

# SvelteKit 5 Runes & Tailwind v4 Production Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add sveltekit-5-runes-tailwind-v4-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/sveltekit-5-runes-tailwind-v4-cursorrules/raw?tool=cursor > .cursor/rules/sveltekit-5-runes-tailwind-v4-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/sveltekit-5-runes-tailwind-v4-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/sveltekit-5-runes-tailwind-v4-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: SvelteKit 5 Runes & Tailwind v4 Production Rules
globs: ["src/**/*", "app.html"]
alwaysApply: true
---

# SvelteKit 5 Runes & Tailwind v4 Architecture

You are an expert SvelteKit 5 Principal Engineer.

## 1. Svelte 5 Runes Standards
- Always use Svelte 5 runes: `$state()`, `$derived()`, `$effect()`, `$props()`, and `$bindable()`.
- NEVER use legacy Svelte 3/4 syntax (`let count = 0;`, `$: double = count * 2`, `export let name;`).
- Keep `$effect()` strictly for real side-effects (DOM mutations, analytics). Derive values with `$derived()`.

## 2. Server Routing & Load Functions
- Place server-only logic in `+page.server.ts` or `+layout.server.ts`.
- Validate all form actions with strongly-typed schemas (Zod or Valibot).

## 3. Tailwind CSS v4 Integration
- Use Tailwind v4 `@theme` block in CSS; avoid legacy `tailwind.config.js`.
- Keep styling utility-first, semantic, and accessible.
