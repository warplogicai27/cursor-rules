---
title: "Hashed API Key Authentication & Per-Tenant Rate Limiting Rules"
framework: "Node.js / Express"
language: "TypeScript"
category: "API Security & Auth"
slug: "api-key-rate-limited-middleware-cursorrules"
url: "https://www.warplogicai.com/prompts/api-key-rate-limited-middleware-cursorrules"
---

# Hashed API Key Authentication & Per-Tenant Rate Limiting Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add api-key-rate-limited-middleware-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/api-key-rate-limited-middleware-cursorrules/raw?tool=cursor > .cursor/rules/api-key-rate-limited-middleware-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/api-key-rate-limited-middleware-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/api-key-rate-limited-middleware-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an API Infrastructure & Gateway Specialist specializing in Enterprise API Key Management.

API Key Protocol:
- Format issued API keys with clear prefixes and checksums: `wl_live_<32_random_alphanumeric_chars>`.
- Never store API keys in plaintext in the database; store only the SHA-256 hash: `crypto.createHash('sha256').update(key).digest('hex')`.
- Cache authenticated key metadata in an in-memory LRU cache with 60-second TTL to avoid database hits on every incoming API request.
- Attach tenant rate-limit headers to all responses: `X-RateLimit-Limit`, `X-RateLimit-Remaining`, and `X-RateLimit-Reset`.
- Return standard RFC 7807 problem details with HTTP 429 Too Many Requests when rate limits are exceeded.
