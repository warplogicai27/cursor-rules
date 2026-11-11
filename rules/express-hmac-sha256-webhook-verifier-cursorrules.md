---
title: "HMAC SHA-256 Cryptographic Webhook Verifier Middleware Rules"
framework: "Express.js / Node.js"
language: "TypeScript"
category: "API Security & Auth"
slug: "express-hmac-sha256-webhook-verifier-cursorrules"
url: "https://www.warplogicai.com/prompts/express-hmac-sha256-webhook-verifier-cursorrules"
---

# HMAC SHA-256 Cryptographic Webhook Verifier Middleware Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add express-hmac-sha256-webhook-verifier-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/express-hmac-sha256-webhook-verifier-cursorrules/raw?tool=cursor > .cursor/rules/express-hmac-sha256-webhook-verifier-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/express-hmac-sha256-webhook-verifier-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/express-hmac-sha256-webhook-verifier-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Senior Backend Engineer specializing in Webhook Architecture and Cryptographic Payload Verification.

Webhook Verifier Rules:
- Always compute and verify HMAC signatures using the RAW binary request body buffer before any JSON parsing takes place.
- Configure Express `body-parser` with a `verify` hook to capture `req.rawBody = buf`:
  `express.json({ verify: (req: any, _res, buf) => { req.rawBody = buf; } })`.
- Compute signature: `crypto.createHmac('sha256', secret).update(rawBody).digest('hex')`.
- Compare signatures using constant-time comparison `crypto.timingSafeEqual()` to completely eliminate timing side-channel attacks.
- Check incoming webhook timestamp headers (e.g., within 5 minutes) to prevent replay attacks.
