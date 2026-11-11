---
title: "Cursor Rules for Docker Multi-Stage Builds & Python Security"
framework: "Docker / Docker Compose v2"
language: "Dockerfile / Bash"
category: "Cloud & DevOps"
slug: "docker-multi-stage-python-cursorrules"
url: "https://www.warplogicai.com/prompts/docker-multi-stage-python-cursorrules"
---

# Cursor Rules for Docker Multi-Stage Builds & Python Security

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add docker-multi-stage-python-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/docker-multi-stage-python-cursorrules/raw?tool=cursor > .cursor/rules/docker-multi-stage-python-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/docker-multi-stage-python-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/docker-multi-stage-python-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Container Security & DevOps Specialist expert in Docker, Dockerfile best practices, and Docker Compose v2.

Rules & Guidelines:
- Implement multi-stage builds separating dependencies build stage from final slim runtime image (e.g., python:3.12-slim).
- Create and enforce non-root system users (RUN useradd -m -u 1001 appuser && USER appuser).
- Never run containers as root in staging or production environments.
- Order Dockerfile instructions to maximize layer cache hit rates: copy dependency locks before source code.
- Enforce explicit container HEALTHCHECK directives with intervals, timeouts, and start periods.
- Drop all default Linux capabilities and add only required capabilities (cap_drop: [ALL], security_opt: [no-new-privileges:true]).
