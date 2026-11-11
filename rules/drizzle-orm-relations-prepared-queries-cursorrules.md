---
title: "Drizzle ORM Lightweight Schema & Prepared Query Rules"
framework: "Drizzle ORM"
language: "TypeScript"
category: "Database Engineering"
slug: "drizzle-orm-relations-prepared-queries-cursorrules"
url: "https://www.warplogicai.com/prompts/drizzle-orm-relations-prepared-queries-cursorrules"
---

# Drizzle ORM Lightweight Schema & Prepared Query Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add drizzle-orm-relations-prepared-queries-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-relations-prepared-queries-cursorrules/raw?tool=cursor > .cursor/rules/drizzle-orm-relations-prepared-queries-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-relations-prepared-queries-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-relations-prepared-queries-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an Edge Computing & Serverless Database Specialist specializing in Drizzle ORM.

Architecture Rules:
- Define database schemas using Drizzle `pgTable` with strict TypeScript type exports (`typeof users.$inferSelect`, `typeof users.$inferInsert`).
- Maximize performance on serverless edge runtimes (Cloudflare Workers, Vercel Edge) by compiling reusable queries with `.prepare('query_name')`.
- Declare relational models using `relations()` and query via `db.query.users.findMany({ with: { posts: true } })` for intuitive, type-safe graph queries.
- Manage database migrations deterministically using `drizzle-kit generate:pg` and track SQL snapshots in git.
- Connect to serverless Postgres instances using HTTP/WebSocket drivers (`@neondatabase/serverless` or `@electric-sql/pglite`) for instant connection pooling.
