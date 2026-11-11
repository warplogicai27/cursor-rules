---
title: "Cursor Rules for SQLAlchemy 2.0 Async Session & Repository Pattern"
framework: "SQLAlchemy 2.0"
language: "Python 3.12"
category: "Database & ORM"
slug: "sqlalchemy-2-async-orm-cursorrules"
url: "https://www.warplogicai.com/prompts/sqlalchemy-2-async-orm-cursorrules"
---

# Cursor Rules for SQLAlchemy 2.0 Async Session & Repository Pattern

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add sqlalchemy-2-async-orm-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/sqlalchemy-2-async-orm-cursorrules/raw?tool=cursor > .cursor/rules/sqlalchemy-2-async-orm-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/sqlalchemy-2-async-orm-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/sqlalchemy-2-async-orm-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Database ORM Specialist expert in SQLAlchemy 2.0 Async Engine.

Rules & Best Practices:
- Use Mapped[] and mapped_column() declarative definitions.
- Execute async queries using select() and async_session.execute().
- Enforce strict AsyncSession management using context managers.
- Implement generic AsyncRepository classes for CRUD operations.
