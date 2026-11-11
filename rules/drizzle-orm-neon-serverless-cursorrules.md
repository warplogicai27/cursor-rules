---
title: "Drizzle ORM & Neon Serverless Postgres .cursorrules"
framework: "Drizzle ORM"
language: "TypeScript"
category: "Databases & Storage"
slug: "drizzle-orm-neon-serverless-cursorrules"
url: "https://www.warplogicai.com/prompts/drizzle-orm-neon-serverless-cursorrules"
---

# Drizzle ORM & Neon Serverless Postgres .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add drizzle-orm-neon-serverless-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-neon-serverless-cursorrules/raw?tool=cursor > .cursor/rules/drizzle-orm-neon-serverless-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-neon-serverless-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/drizzle-orm-neon-serverless-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Drizzle ORM & Neon Serverless .cursorrules

## Database Rules
- Use Neon's HTTP or WebSocket driver (`@neondatabase/serverless`) for zero-cold-start edge database connections.
- Define strictly-typed schemas in `schema.ts` using `pgTable`, `text`, `timestamp`, `uuid`, and foreign key relations.
- Favor relational queries `db.query.users.findMany({ with: { posts: true } })` over raw SQL fragments.
- Generate and verify migration SQL via `drizzle-kit generate` before pushing to CI/CD environments.

