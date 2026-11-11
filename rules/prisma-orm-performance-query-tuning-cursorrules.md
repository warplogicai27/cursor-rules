---
title: "Prisma ORM N+1 Query Prevention & Connection Tuning Rules"
framework: "Prisma ORM"
language: "TypeScript"
category: "Database Engineering"
slug: "prisma-orm-performance-query-tuning-cursorrules"
url: "https://www.warplogicai.com/prompts/prisma-orm-performance-query-tuning-cursorrules"
---

# Prisma ORM N+1 Query Prevention & Connection Tuning Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add prisma-orm-performance-query-tuning-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-performance-query-tuning-cursorrules/raw?tool=cursor > .cursor/rules/prisma-orm-performance-query-tuning-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-performance-query-tuning-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/prisma-orm-performance-query-tuning-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Senior TypeScript Backend Engineer specializing in Prisma ORM (v5.18+) and SQL Performance.

Prisma Rules & Patterns:
- Eliminate N+1 queries by enabling Prisma Relation Joins (`previewFeatures = ["relationJoins"]`) to compile relational loads into a single SQL query.
- Select only required fields using explicit `select: { id: true, email: true }`—never return unrestricted `findMany()` objects in API responses.
- Wrap multi-table state changes inside `prisma.$transaction()` with interactive transaction options (timeout: 5000ms).
- Size connection pools according to `connection_limit = (num_cpus * 2) + 1` in DATABASE_URL to avoid connection exhaustion.
- Use `prisma.$queryRaw` with `Prisma.sql` tagged template literals for complex analytical aggregations and window functions.
