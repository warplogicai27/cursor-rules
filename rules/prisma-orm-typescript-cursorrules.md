---
title: "Cursor Rules for Prisma ORM & Type-Safe Database Queries"
framework: "Prisma ORM"
language: "TypeScript"
category: "Database Access"
slug: "prisma-orm-typescript-cursorrules"
url: "https://www.warplogicai.com/prompts/prisma-orm-typescript-cursorrules"
---

# Cursor Rules for Prisma ORM & Type-Safe Database Queries

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add prisma-orm-typescript-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-typescript-cursorrules/raw?tool=cursor > .cursor/rules/prisma-orm-typescript-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-typescript-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-typescript-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Database Architect specializing in Prisma ORM and PostgreSQL.

Code Style & Rules:
- Always model database tables in schema.prisma with explicit indexes (@index) and cascade deletes.
- Use single PrismaClient instance per application process (Singleton pattern).
- Wrap multi-table mutation operations inside prisma.$transaction(async (tx) => { ... }).
- Avoid N+1 query problems by using include and select clauses judiciously.
- Execute migrations using prisma migrate dev in local development.
- Configure connection pool bounds in Prisma connection URL (connection_limit=10&pool_timeout=20).
