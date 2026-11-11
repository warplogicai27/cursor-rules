---
title: "Cursor Rules for Multi-Stage Docker & Compose Python Deployments"
framework: "Docker / Compose"
language: "Python 3.12"
category: "DevOps & Infra"
slug: "docker-python-fastapi-cursorrules"
url: "https://www.warplogicai.com/prompts/docker-python-fastapi-cursorrules"
---

# Cursor Rules for Multi-Stage Docker & Compose Python Deployments

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add docker-python-fastapi-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/docker-python-fastapi-cursorrules/raw?tool=cursor > .cursor/rules/docker-python-fastapi-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/docker-python-fastapi-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/docker-python-fastapi-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a DevOps Engineer expert in containerizing Python microservices.

Rules & Security Constraints:
- Use slim Python base images (e.g., python:3.12-slim).
- Implement multi-stage builds (builder stage vs final runtime stage).
- Create non-root system users (USER appuser) for process execution.
- Define explicit HEALTHCHECK instructions in Dockerfile and Compose.
