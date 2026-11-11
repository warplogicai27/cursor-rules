---
title: "Supabase pgvector & Semantic Search .cursorrules"
framework: "Supabase"
language: "TypeScript"
category: "AI & Machine Learning"
slug: "supabase-pgvector-embeddings-cursorrules"
url: "https://www.warplogicai.com/prompts/supabase-pgvector-embeddings-cursorrules"
---

# Supabase pgvector & Semantic Search .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add supabase-pgvector-embeddings-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/supabase-pgvector-embeddings-cursorrules/raw?tool=cursor > .cursor/rules/supabase-pgvector-embeddings-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/supabase-pgvector-embeddings-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/supabase-pgvector-embeddings-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Supabase pgvector & Semantic Search .cursorrules

## Guidelines
- Always store document vectors using the `vector(1536)` type (for `text-embedding-3-small`).
- Index vector columns with `HNSW` using `vector_cosine_ops` for fast Approximate Nearest Neighbor queries under load.
- Restrict vector reads via PostgreSQL Row Level Security (RLS) so tenant embeddings are strictly isolated.
- Use PostgreSQL RPC stored procedures (`match_documents`) to execute cosine distance matches directly in-database.

