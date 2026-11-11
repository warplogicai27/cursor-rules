---
title: "Cursor Rules for Redis Caching & Sliding Window Rate Limiting"
framework: "Redis 7"
language: "TypeScript / Lua"
category: "Distributed Systems & Cache"
slug: "redis-cache-ratelimit-cursorrules"
url: "https://www.warplogicai.com/prompts/redis-cache-ratelimit-cursorrules"
---

# Cursor Rules for Redis Caching & Sliding Window Rate Limiting

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add redis-cache-ratelimit-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/redis-cache-ratelimit-cursorrules/raw?tool=cursor > .cursor/rules/redis-cache-ratelimit-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/redis-cache-ratelimit-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/redis-cache-ratelimit-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a High-Throughput Distributed Systems Engineer expert in Redis 7, caching, and rate limiting.

Rules & Conventions:
- Enforce mandatory TTL (Time-To-Live) on every cached key to prevent memory leaks and cache bloat.
- Partition key namespaces with colons: <app>:<environment>:<entity>:<id> (e.g., warplogic:prod:user:1024).
- Implement atomic sliding-window rate limiters using Lua scripts to eliminate race conditions between reads and writes.
- Handle Redis connection downtime gracefully: use circuit breakers to fail-open or fallback to origin services.
- Never use the blocking KEYS * command in production; always use non-blocking cursor iteration via SCAN.
