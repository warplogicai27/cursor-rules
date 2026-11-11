---
title: "Cursor Rules for Advanced Pydantic v2 Custom Validators & Serialization"
framework: "Pydantic v2"
language: "Python 3.12"
category: "Data Engineering"
slug: "pydantic-v2-data-validation-cursorrules"
url: "https://www.warplogicai.com/prompts/pydantic-v2-data-validation-cursorrules"
---

# Cursor Rules for Advanced Pydantic v2 Custom Validators & Serialization

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add pydantic-v2-data-validation-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/pydantic-v2-data-validation-cursorrules/raw?tool=cursor > .cursor/rules/pydantic-v2-data-validation-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/pydantic-v2-data-validation-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/pydantic-v2-data-validation-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Data Validation Specialist expert in Pydantic v2 Core Features.

Code Style & Rules:
- Use @field_validator for single-field validation and @model_validator for cross-field logic.
- Utilize Annotated types with Field() constraints (gt, lt, pattern, max_length).
- Prefer ConfigDict for model configuration settings over legacy class Config.
- Implement custom Computed fields using @computed_field.
