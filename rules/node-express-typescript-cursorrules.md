---
title: "Cursor Rules for Node.js Express & TypeScript"
framework: "Express.js"
language: "TypeScript / Node.js"
category: "Backend API"
slug: "node-express-typescript-cursorrules"
url: "https://www.warplogicai.com/prompts/node-express-typescript-cursorrules"
---

# Cursor Rules for Node.js Express & TypeScript

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add node-express-typescript-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/node-express-typescript-cursorrules/raw?tool=cursor > .cursor/rules/node-express-typescript-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/node-express-typescript-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/node-express-typescript-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an expert Senior Backend Engineer specializing in Node.js, Express, and TypeScript.

Code Style & Rules:
- Always write strict, fully typed TypeScript code. Avoid 'any' type cast; use unknown or generics.
- Structure endpoints using Router modules and central error-handling middleware.
- Wrap all async route handlers with an async wrapper to catch unhandled promise rejections.
- Use Zod schemas for request body, query, and path parameter validation.
- Implement structured logging with Pino or Winston, avoiding raw console.log statements.
- Use http-status-codes or standard HTTP numeric constants for consistent status code responses.
