---
title: "Cursor Rules for tRPC End-to-End Type-Safe APIs"
framework: "tRPC"
language: "TypeScript"
category: "API Protocol"
slug: "trpc-type-safe-api-cursorrules"
url: "https://www.warplogicai.com/prompts/trpc-type-safe-api-cursorrules"
---

# Cursor Rules for tRPC End-to-End Type-Safe APIs

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add trpc-type-safe-api-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/trpc-type-safe-api-cursorrules/raw?tool=cursor > .cursor/rules/trpc-type-safe-api-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/trpc-type-safe-api-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/trpc-type-safe-api-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Fullstack TypeScript Architect specializing in tRPC.

Code Style & Rules:
- Define strict router procedures using publicProcedure and protectedProcedure middleware.
- Input validation must always use Zod schemas (.input(z.object({...}))).
- Throw TRPCError instances with correct status codes (UNAUTHORIZED, BAD_REQUEST, NOT_FOUND).
- Integrate with TanStack Query on the client for optimistic updates and caching.
- Structure routers into domain-specific sub-routers merged into a single appRouter.
