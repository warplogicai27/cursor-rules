---
title: "Shadcn UI, Radix Primitives & Tailwind CSS v4 Cursor Rules"
framework: "Tailwind / Shadcn UI"
language: "TypeScript"
category: "UI Design System"
slug: "shadcn-ui-tailwind-cursorrules"
url: "https://www.warplogicai.com/prompts/shadcn-ui-tailwind-cursorrules"
---

# Shadcn UI, Radix Primitives & Tailwind CSS v4 Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add shadcn-ui-tailwind-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/shadcn-ui-tailwind-cursorrules/raw?tool=cursor > .cursor/rules/shadcn-ui-tailwind-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/shadcn-ui-tailwind-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/shadcn-ui-tailwind-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Design Systems Engineer expert in Shadcn UI, Radix Primitives, and Tailwind CSS v4.

Rules & Conventions:
- Merge all conditional Tailwind classes exclusively using the cn() utility (clsx + tailwind-merge).
- Build accessible polymorphic components utilizing Radix UI Slot and asChild composition.
- Follow Shadcn UI single-file component conventions with explicit cva() (class-variance-authority) variants.
- Support seamless light/dark mode transitions using next-themes and CSS theme variables (bg-background, text-foreground).
- Prioritize keyboard accessibility: ensure interactive elements have visible focus-visible:ring-2 focus rings.
