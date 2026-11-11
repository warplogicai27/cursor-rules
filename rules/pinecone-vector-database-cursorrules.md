---
title: "Cursor Rules for Pinecone Vector DB & Hybrid Search"
framework: "Pinecone"
language: "Python 3.12"
category: "AI & Machine Learning"
slug: "pinecone-vector-database-cursorrules"
url: "https://www.warplogicai.com/prompts/pinecone-vector-database-cursorrules"
---

# Cursor Rules for Pinecone Vector DB & Hybrid Search

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add pinecone-vector-database-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/pinecone-vector-database-cursorrules/raw?tool=cursor > .cursor/rules/pinecone-vector-database-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/pinecone-vector-database-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/pinecone-vector-database-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Enforce Pinecone v3 serverless index management, chunked upserts, and metadata filtering.
globs: ["src/vectorstore/**/*.py", "src/db/pinecone.py", "services/vector/**/*.py"]
alwaysApply: false
---

You are an expert Database & AI Engineer specializing in Pinecone Vector Database v3.

Code Style & Rules:
- Initialize Pinecone client using Pinecone(api_key=...) and target serverless AWS/GCP index deployments.
- Perform batch vector upserts in chunks of 100 vectors using async batching or thread pools.
- Include structured metadata attributes (tenant_id, document_type, created_at) with indexed fields pre-configured.
- Apply strict metadata filtering dictionaries ($eq, $in, $gte) on query and hybrid search operations.
- Isolate environments and multi-tenant tenants using explicit namespace partition parameters.
