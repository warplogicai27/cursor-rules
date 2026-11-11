---
title: "Upstash Redis Sliding-Window Rate Limiting .cursorrules"
framework: "Upstash"
language: "TypeScript"
category: "API Security"
slug: "redis-upstash-rate-limiting-cursorrules"
url: "https://www.warplogicai.com/prompts/redis-upstash-rate-limiting-cursorrules"
---

# Upstash Redis Sliding-Window Rate Limiting .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add redis-upstash-rate-limiting-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/redis-upstash-rate-limiting-cursorrules/raw?tool=cursor > .cursor/rules/redis-upstash-rate-limiting-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/redis-upstash-rate-limiting-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/redis-upstash-rate-limiting-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Upstash Redis Rate Limiting .cursorrules

## Implementation
- Use `@upstash/ratelimit` with `Ratelimit.slidingWindow(limit, window)` for smooth rate enforcement.
- Key rate limits on authenticated identity (SPIFFE ID, API Key, User ID) with fallback to hashed IP address.
- Return standard RFC 6585 headers: `X-RateLimit-Limit`, `X-RateLimit-Remaining`, `X-RateLimit-Reset`.
- On limit exceeded, immediately return `HTTP 429 Too Many Requests` with `Retry-After` header.

