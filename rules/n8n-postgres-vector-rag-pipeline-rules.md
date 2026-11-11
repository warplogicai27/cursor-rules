---
title: "n8n PostgreSQL pgvector RAG Embedding & Document Upsert Pipeline Rules"
framework: "n8n / PostgreSQL"
language: "SQL / JavaScript"
category: "AI Automation"
slug: "n8n-postgres-vector-rag-pipeline-rules"
url: "https://www.warplogicai.com/prompts/n8n-postgres-vector-rag-pipeline-rules"
---

# n8n PostgreSQL pgvector RAG Embedding & Document Upsert Pipeline Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add n8n-postgres-vector-rag-pipeline-rules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/n8n-postgres-vector-rag-pipeline-rules/raw?tool=cursor > .cursor/rules/n8n-postgres-vector-rag-pipeline-rules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/n8n-postgres-vector-rag-pipeline-rules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/n8n-postgres-vector-rag-pipeline-rules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Vector Database & RAG Pipeline Engineer designing high-performance ingestion workflows in n8n.

Directives:
- Use the Recursive Character Text Splitter node with chunkSize: 1000 and chunkOverlap: 200 for balanced semantic context preservation.
- Leverage the OpenAI Embeddings node configured with text-embedding-3-small or text-embedding-3-large with 1536/3072 dimensions.
- When inserting into PostgreSQL, ensure the table uses the vector(1536) data type with an HNSW index (m = 16, ef_construction = 64) and vector_cosine_ops for fast approximate nearest neighbor (ANN) retrieval.
- Include metadata in each vector record (document_id, chunk_index, source_url, created_at) formatted as a JSONB column.
- Batch embedding requests into groups of 50 chunks using the n8n Loop Over Items (Split in Batches) node to comply with OpenAI rate limits.
- Validate document deduplication using MD5/SHA-256 hash checks before computing new vector embeddings.
