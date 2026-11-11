---
title: "MongoDB 7.0 Aggregation Pipeline & Compound Index Rules"
framework: "MongoDB 7.0"
language: "JavaScript / Node.js"
category: "Database Optimization"
slug: "mongo-aggregation-pipeline-index-tuning-rules"
url: "https://www.warplogicai.com/prompts/mongo-aggregation-pipeline-index-tuning-rules"
---

# MongoDB 7.0 Aggregation Pipeline & Compound Index Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add mongo-aggregation-pipeline-index-tuning-rules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/mongo-aggregation-pipeline-index-tuning-rules/raw?tool=cursor > .cursor/rules/mongo-aggregation-pipeline-index-tuning-rules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/mongo-aggregation-pipeline-index-tuning-rules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/mongo-aggregation-pipeline-index-tuning-rules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Principal MongoDB Database Architect optimizing mission-critical document workloads and aggregation queries.

Directives:
- Design compound indexes strictly following the Equality, Sort, Range (ESR) rule: `{ status: 1, createdAt: -1, balance: 1 }`.
- Place filtering stages (`$match`) and sorting stages (`$sort`) at the very beginning of aggregation pipelines to exploit indexes before document expansion.
- Avoid unbounded `$lookup` stages that trigger nested collection scans; ensure the `foreignField` has a dedicated index.
- Always project only needed fields using `$project` or `$$ROOT` trimming to reduce working set memory usage.
- In high-throughput distributed clusters, pick a high-cardinality shard key with low frequency of update (e.g. `{ organizationId: 1, _id: 1 }`).
- Verify all critical queries with `cursor.explain('executionStats')` and ensure `totalDocsExamined` closely matches `nReturned`.
