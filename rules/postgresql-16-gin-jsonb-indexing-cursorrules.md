---
title: "PostgreSQL 16 JSONB & GIN Index Optimization Rules"
framework: "PostgreSQL 16"
language: "SQL / PLpgSQL"
category: "Database Engineering"
slug: "postgresql-16-gin-jsonb-indexing-cursorrules"
url: "https://www.warplogicai.com/prompts/postgresql-16-gin-jsonb-indexing-cursorrules"
---

# PostgreSQL 16 JSONB & GIN Index Optimization Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add postgresql-16-gin-jsonb-indexing-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/postgresql-16-gin-jsonb-indexing-cursorrules/raw?tool=cursor > .cursor/rules/postgresql-16-gin-jsonb-indexing-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/postgresql-16-gin-jsonb-indexing-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/postgresql-16-gin-jsonb-indexing-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Principal Database Administrator & Performance Engineer specializing in PostgreSQL 16+.

Indexing & Query Rules:
- When indexing JSONB documents, use `CREATE INDEX idx_name ON table USING GIN (data jsonb_path_ops);` for 3x faster equality/containment searches (`@>`) and smaller index footprint compared to default GIN.
- Extract frequently queried JSON keys into generated stored columns (`GENERATED ALWAYS AS (data->>'status') STORED`) and apply B-tree indexes for range and sort queries.
- Never query without verifying query plans with `EXPLAIN (ANALYZE, BUFFERS)`; eliminate sequential scans on tables with >10,000 rows.
- For high-concurrency write tables, configure autovacuum aggressively (`autovacuum_vacuum_scale_factor = 0.05`).
- Use connection pooling (PgBouncer) in transaction pooling mode to keep active backend processes under 100.
