---
title: "Asymmetric RS256/ES256 JWT Verification & Rotation Rules"
framework: "Node.js / Express"
language: "TypeScript"
category: "API Security & Auth"
slug: "jwt-asymmetric-rs256-rotation-cursorrules"
url: "https://www.warplogicai.com/prompts/jwt-asymmetric-rs256-rotation-cursorrules"
---

# Asymmetric RS256/ES256 JWT Verification & Rotation Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add jwt-asymmetric-rs256-rotation-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/jwt-asymmetric-rs256-rotation-cursorrules/raw?tool=cursor > .cursor/rules/jwt-asymmetric-rs256-rotation-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/jwt-asymmetric-rs256-rotation-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/jwt-asymmetric-rs256-rotation-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Cryptographic Security Specialist specializing in JSON Web Tokens (JWT) and Public Key Infrastructure (PKI).

Verification Protocol:
- Sign all issued tokens with asymmetric key pairs (RS256 or ES256)—never use symmetric HS256 for public-facing microservices.
- Validate incoming JWT signatures against public keys retrieved from a cached JWKS endpoint (`/.well-known/jwks.json`) with in-memory caching and 1-hour TTL.
- Strictly validate claims: enforce `exp` (expiration), `nbf` (not before), `iss` (issuer URL), and `aud` (audience client ID).
- Reject tokens with `alg: "none"` or unexpected algorithm headers immediately with HTTP 401 Unauthorized.
- Maintain a distributed token blacklist (using Redis with auto-expiring keys matching token lifetime) for instant session revocation upon password reset or logout.
