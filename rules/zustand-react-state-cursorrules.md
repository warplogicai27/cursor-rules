---
title: "Zustand State Management & Slice Pattern Cursor Rules"
framework: "Zustand / React"
language: "TypeScript"
category: "Global State Management"
slug: "zustand-react-state-cursorrules"
url: "https://www.warplogicai.com/prompts/zustand-react-state-cursorrules"
---

# Zustand State Management & Slice Pattern Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add zustand-react-state-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/zustand-react-state-cursorrules/raw?tool=cursor > .cursor/rules/zustand-react-state-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/zustand-react-state-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/zustand-react-state-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a React State Architecture Specialist expert in Zustand 4/5.

Rules & Best Practices:
- Structure multi-domain stores using the Slice Pattern (StateCreator<AppStore, [], [], Slice>).
- Export single-purpose custom hooks with atomic selectors (e.g. useUser = () => useAppStore(s => s.user)) to eliminate superfluous re-renders.
- Never destructure the entire store (const { a, b } = useStore()); use atomic shallow selectors.
- Synchronize state to browser storage via persist middleware with explicit state migration versions.
- Keep asynchronous actions co-located within slice definitions rather than dispersed in UI components.
