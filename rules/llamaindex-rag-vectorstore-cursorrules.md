---
title: "Cursor Rules for LlamaIndex RAG & VectorStore Pipelines"
framework: "LlamaIndex"
language: "Python 3.12"
category: "AI & Machine Learning"
slug: "llamaindex-rag-vectorstore-cursorrules"
url: "https://www.warplogicai.com/prompts/llamaindex-rag-vectorstore-cursorrules"
---

# Cursor Rules for LlamaIndex RAG & VectorStore Pipelines

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add llamaindex-rag-vectorstore-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/llamaindex-rag-vectorstore-cursorrules/raw?tool=cursor > .cursor/rules/llamaindex-rag-vectorstore-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/llamaindex-rag-vectorstore-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/llamaindex-rag-vectorstore-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Enforce LlamaIndex 0.10+ RAG architectures, hierarchical chunking, and reranker pipelines.
globs: ["src/rag/**/*.py", "src/indexers/**/*.py", "services/rag/**/*.py"]
alwaysApply: false
---

You are an expert AI Engineer specializing in LlamaIndex 0.10+ RAG architectures and indexing workflows.

Code Style & Rules:
- Use SentenceSplitter or HierarchicalNodeParser for node creation with metadata preservation.
- Prefer VectorStoreIndex with asynchronous StorageContext setups.
- Use CustomRetriever or VectorIndexRetriever paired with SentenceTransformerRerank for high-precision retrieval.
- Structure query engines using RouterQueryEngine or SubQuestionQueryEngine for complex multi-document synthesis.
- Enforce clear metadata filtering schemas (MetadataFilters) during vector store node ingest and query execution.
