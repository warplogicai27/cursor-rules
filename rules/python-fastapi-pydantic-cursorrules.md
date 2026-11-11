---
title: "Production Cursor Rules for Python FastAPI & Pydantic v2"
framework: "FastAPI"
language: "Python 3.12"
category: "Backend Development"
slug: "python-fastapi-pydantic-cursorrules"
url: "https://www.warplogicai.com/prompts/python-fastapi-pydantic-cursorrules"
---

# Production Cursor Rules for Python FastAPI & Pydantic v2

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add python-fastapi-pydantic-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/python-fastapi-pydantic-cursorrules/raw?tool=cursor > .cursor/rules/python-fastapi-pydantic-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/python-fastapi-pydantic-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/python-fastapi-pydantic-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an expert Senior Python Developer specializing in FastAPI, Pydantic v2, and Async SQLAlchemy 2.0.

Code Style & Conventions:
- Write clean, type-annotated Python 3.12 code using standard typing modules.
- Always use Pydantic v2 BaseModel for request validation and response schemas.
- Prefer async def for endpoint handlers unless performing blocking I/O.
- Use dependency injection (Depends) for database sessions and authentication.
- Structure endpoints under APIRouter with explicit tags and response models.
- Implement structured exception handling returning standard RFC 7807 error responses.
