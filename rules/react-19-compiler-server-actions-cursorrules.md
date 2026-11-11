---
title: "React 19 & Next.js 15 Server Actions Production .cursorrules"
framework: "React 19"
language: "TypeScript"
category: "Frontend Frameworks"
slug: "react-19-compiler-server-actions-cursorrules"
url: "https://www.warplogicai.com/prompts/react-19-compiler-server-actions-cursorrules"
---

# React 19 & Next.js 15 Server Actions Production .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add react-19-compiler-server-actions-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/react-19-compiler-server-actions-cursorrules/raw?tool=cursor > .cursor/rules/react-19-compiler-server-actions-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/react-19-compiler-server-actions-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/react-19-compiler-server-actions-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# React 19 & Next.js 15 Server Actions .cursorrules

## Core Principles
- Always leverage the React 19 Compiler: avoid unnecessary `useMemo` and `useCallback` unless profiling proves referential stability issues.
- Use `useActionState` and `useOptimistic` for form actions instead of legacy `useEffect` state syncing.
- Define Server Actions in isolated `actions/` files marked with `'use server'`.
- Validate all inputs in Server Actions using Zod before performing database mutations.
- Return discriminated union results: `{ success: true, data: T } | { success: false, error: string }`.

## Code Patterns
```typescript
'use server';
import { z } from 'zod';

const UpdateProfileSchema = z.object({
  name: z.string().min(2),
  email: z.string().email(),
});

export async function updateProfile(prevState: any, formData: FormData) {
  const parsed = UpdateProfileSchema.safeParse(Object.fromEntries(formData));
  if (!parsed.success) {
    return { success: false, error: parsed.error.issues[0].message };
  }
  // Perform atomic mutation...
  return { success: true, data: parsed.data };
}
```

