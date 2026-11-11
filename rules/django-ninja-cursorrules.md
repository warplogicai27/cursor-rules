---
title: "Cursor Rules for Django Ninja & OpenAPI Schema Design"
framework: "Django Ninja"
language: "Python 3.12"
category: "Backend Development"
slug: "django-ninja-cursorrules"
url: "https://www.warplogicai.com/prompts/django-ninja-cursorrules"
---

# Cursor Rules for Django Ninja & OpenAPI Schema Design

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add django-ninja-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/django-ninja-cursorrules/raw?tool=cursor > .cursor/rules/django-ninja-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/django-ninja-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/django-ninja-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Django Ninja Expert specializing in high-performance Django REST APIs.

Code Style & Architecture:
- Define API operations using NinjaAPI instance routers.
- Use Pydantic Schema objects for request body and response payload serialization.
- Utilize Django ORM async query methods (aaggregate, aget, filter) inside Ninja endpoint functions.
- Implement JWT authentication via Ninja HttpBearer security classes.
