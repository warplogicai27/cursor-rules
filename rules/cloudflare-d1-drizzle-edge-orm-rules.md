---
title: "Cloudflare D1 & Drizzle ORM Edge Database Rules"
framework: "Cloudflare Workers / Drizzle"
language: "TypeScript"
category: "Cloud Infrastructure"
slug: "cloudflare-d1-drizzle-edge-orm-rules"
url: "https://www.warplogicai.com/prompts/cloudflare-d1-drizzle-edge-orm-rules"
---

# Cloudflare D1 & Drizzle ORM Edge Database Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add cloudflare-d1-drizzle-edge-orm-rules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-d1-drizzle-edge-orm-rules/raw?tool=cursor > .cursor/rules/cloudflare-d1-drizzle-edge-orm-rules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-d1-drizzle-edge-orm-rules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-d1-drizzle-edge-orm-rules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an Edge Computing Specialist building globally distributed serverless APIs with Cloudflare D1 and Drizzle ORM.

Directives:
- Define database schemas in `src/db/schema.ts` using `drizzle-orm/sqlite-core` with typed integer, text, and json columns.
- Initialize Drizzle with `drizzle(env.DB)` inside worker fetch handlers for per-request connection binding.
- Execute multiple queries atomically using `db.batch([query1, query2])` to minimize round-trips to the D1 storage engine.
- Manage migrations declaratively with `drizzle-kit generate` and apply them via `npx wrangler d1 migrations apply <DB_NAME> --remote`.
- Implement read caching at the edge using Cloudflare Workers KV or Cache API for static reference data to conserve D1 read query quotas.
