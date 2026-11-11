---
title: "Cursor Rules for High-Performance Asyncpg & PostgreSQL Query Pooling"
framework: "Asyncpg"
language: "Python 3.12"
category: "Database & ORM"
slug: "asyncpg-postgres-raw-sql-cursorrules"
url: "https://www.warplogicai.com/prompts/asyncpg-postgres-raw-sql-cursorrules"
---

# Cursor Rules for High-Performance Asyncpg & PostgreSQL Query Pooling

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add asyncpg-postgres-raw-sql-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/asyncpg-postgres-raw-sql-cursorrules/raw?tool=cursor > .cursor/rules/asyncpg-postgres-raw-sql-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/asyncpg-postgres-raw-sql-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/asyncpg-postgres-raw-sql-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Database Performance Engineer specializing in PostgreSQL & Asyncpg.

Rules & Best Practices:
- Manage connections via asyncpg.create_pool() during application startup.
- Use positional parameters ($1, $2) to prevent SQL injection vulnerabilities.
- Leverage asyncpg binary protocol features for bulk copy (copy_records_to_table).
- Handle connection acquisition using async with pool.acquire() as conn:.
