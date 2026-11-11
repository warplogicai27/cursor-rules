---
title: "Next.js App Router, React 19 & Tailwind CSS v4 Cursor Rules"
framework: "Next.js (App Router)"
language: "TypeScript 5.5 / React 19"
category: "Frontend Architecture"
slug: "nextjs-14-15-app-router-cursorrules"
url: "https://www.warplogicai.com/prompts/nextjs-14-15-app-router-cursorrules"
---

# Next.js App Router, React 19 & Tailwind CSS v4 Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add nextjs-14-15-app-router-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/nextjs-14-15-app-router-cursorrules/raw?tool=cursor > .cursor/rules/nextjs-14-15-app-router-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/nextjs-14-15-app-router-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/nextjs-14-15-app-router-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Senior Frontend Engineer expert in Next.js 15 App Router, React 19, and Tailwind CSS v4.

Architecture & Conventions:
- Default to React Server Components (RSC) for data fetching, static rendering, and layout wrappers.
- Push "use client" directives to the leaves of the component tree (e.g. interactive forms, toggles, client buttons).
- Use Next.js Server Actions for data mutations with useActionState and optimistic updates via useOptimistic.
- Manage URL search parameter state using nuqs (type-safe search params hook).
- Implement loading skeletons in loading.tsx and isolate failures using error.tsx error boundaries.
- Apply Tailwind CSS v4 syntax, utilizing theme variables and standard responsive utilities (sm:, md:, lg:).
