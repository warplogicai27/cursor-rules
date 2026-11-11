---
title: "Tailwind CSS v4 & Shadcn UI Modern .cursorrules"
framework: "Tailwind v4"
language: "TypeScript"
category: "Frontend Frameworks"
slug: "tailwind-v4-vite-shadcn-cursorrules"
url: "https://www.warplogicai.com/prompts/tailwind-v4-vite-shadcn-cursorrules"
---

# Tailwind CSS v4 & Shadcn UI Modern .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add tailwind-v4-vite-shadcn-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/tailwind-v4-vite-shadcn-cursorrules/raw?tool=cursor > .cursor/rules/tailwind-v4-vite-shadcn-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/tailwind-v4-vite-shadcn-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/tailwind-v4-vite-shadcn-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Tailwind CSS v4 & Shadcn UI .cursorrules

## Styling Guidelines
- Tailwind v4 uses CSS-first configuration: define design tokens in `@theme` blocks inside `app.css` rather than `tailwind.config.js`.
- Utilize `cn()` helper (`clsx` + `tailwind-merge`) for dynamic and conditional class application.
- Enforce dark-mode first design tokens with clean CSS variables.
- Adhere to accessible Radix UI primitives (`aria-*` compliance, focus visible rings, keyboard navigability).

```css
@import 'tailwindcss';

@theme {
  --color-brand-primary: #06b6d4;
  --color-brand-surface: #0a0f1d;
  --font-mono: 'JetBrains Mono', monospace;
}
```

