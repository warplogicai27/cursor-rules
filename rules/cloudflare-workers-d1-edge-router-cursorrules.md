---
title: "Cloudflare Workers & D1 Serverless SQL Edge Router Rules"
framework: "Cloudflare Workers"
language: "TypeScript"
category: "Cloud Infrastructure"
slug: "cloudflare-workers-d1-edge-router-cursorrules"
url: "https://www.warplogicai.com/prompts/cloudflare-workers-d1-edge-router-cursorrules"
---

# Cloudflare Workers & D1 Serverless SQL Edge Router Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add cloudflare-workers-d1-edge-router-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-workers-d1-edge-router-cursorrules/raw?tool=cursor > .cursor/rules/cloudflare-workers-d1-edge-router-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-workers-d1-edge-router-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/cloudflare-workers-d1-edge-router-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an Edge Computing Specialist specializing in Cloudflare Workers, Cloudflare Pages, and D1 Database.

Edge Architecture Rules:
- Export the standard ES module fetch handler: `export default { async fetch(request: Request, env: Env, ctx: ExecutionContext): Promise<Response> }`.
- Execute SQL queries against Cloudflare D1 with parameterized prepared statements: `await env.DB.prepare('SELECT * FROM users WHERE tenant_id = ?').bind(tenantId).all()`.
- Accelerate high-volume read endpoints using Cloudflare Cache API or KV storage with explicit `Cache-Control: public, max-age=3600, s-maxage=86400` headers.
- Offload background logging and telemetry using `ctx.waitUntil(logEvent(event))` so user HTTP responses return with zero latency overhead.
- Keep Edge Worker bundle size under 1MB by tree-shaking dependencies and avoiding heavy Node.js built-ins.
