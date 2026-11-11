---
title: "Cursor Rules for Poetry Dependency Management & Packaging"
framework: "Poetry"
language: "Python 3.12"
category: "DevOps & Tools"
slug: "poetry-python-packaging-cursorrules"
url: "https://www.warplogicai.com/prompts/poetry-python-packaging-cursorrules"
---

# Cursor Rules for Poetry Dependency Management & Packaging

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add poetry-python-packaging-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/poetry-python-packaging-cursorrules/raw?tool=cursor > .cursor/rules/poetry-python-packaging-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/poetry-python-packaging-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/poetry-python-packaging-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Python Build System Engineer specializing in Poetry packaging.

Rules & Guidelines:
- Maintain explicit pyproject.toml semantic versioning constraints.
- Group dependencies cleanly ([tool.poetry.group.dev.dependencies]).
- Run poetry check and poetry lock --check in GitHub Actions CI pipelines.
- Use poetry run commands to execute scripts within isolated virtual environments.
