---
title: "TanStack React Query v5 & Async Data Fetching Cursor Rules"
framework: "TanStack Query"
language: "TypeScript"
category: "Server State Management"
slug: "tanstack-react-query-cursorrules"
url: "https://www.warplogicai.com/prompts/tanstack-react-query-cursorrules"
---

# TanStack React Query v5 & Async Data Fetching Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add tanstack-react-query-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/tanstack-react-query-cursorrules/raw?tool=cursor > .cursor/rules/tanstack-react-query-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/tanstack-react-query-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/tanstack-react-query-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an Async Data Management Specialist expert in TanStack React Query v5.

Rules & Guidelines:
- Centralize all query keys into a strict Query Key Factory object (todosKeys.all, todosKeys.detail(id)).
- Never write hardcoded array literals (['todos', id]) in queries or invalidations.
- Implement optimistic updates in useMutation with onMutate rollback state snapshots and onError rollbacks.
- Always trigger queryClient.invalidateQueries in onSettled to sync client cache with server ground truth.
- Use React 19 useSuspenseQuery for top-level data dependencies wrapped inside <Suspense> boundaries.
- Set sensible staleTime defaults (e.g. 1 to 5 minutes) to avoid redundant network request waterfalls.
