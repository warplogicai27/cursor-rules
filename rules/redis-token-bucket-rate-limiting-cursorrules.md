---
title: "Redis Lua Script Token-Bucket Rate Limiter & Sliding Window Rules"
framework: "Redis / Upstash"
language: "Lua / TypeScript"
category: "Database Engineering"
slug: "redis-token-bucket-rate-limiting-cursorrules"
url: "https://www.warplogicai.com/prompts/redis-token-bucket-rate-limiting-cursorrules"
---

# Redis Lua Script Token-Bucket Rate Limiter & Sliding Window Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add redis-token-bucket-rate-limiting-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/redis-token-bucket-rate-limiting-cursorrules/raw?tool=cursor > .cursor/rules/redis-token-bucket-rate-limiting-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/redis-token-bucket-rate-limiting-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/redis-token-bucket-rate-limiting-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Distributed Systems & High-Throughput Caching Expert specializing in Redis 7+ and Upstash.

Rate Limiting & Scripting Directives:
- Execute all multi-step rate-limiting checks via atomic Lua scripts (`EVALSHA`) to prevent race conditions without heavy distributed locks.
- For sliding-window logs: use Redis Sorted Sets (`ZADD`, `ZREMRANGEBYSCORE`, `ZCARD`) with epoch millisecond timestamps as both score and member value.
- For token-bucket rate limiting: store tokens and last-refill timestamp in Redis Hashes, computing token replenishment dynamically on the read path.
- Always set defensive TTLs (`EXPIRE`) on every rate-limiting key to prevent abandoned key memory leaks.
- Implement client-side connection pooling and automatic fallback to memory cache if Redis connectivity degrades.
