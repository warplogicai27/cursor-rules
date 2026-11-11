---
title: "Docker Compose Production Security & Multi-Stage .cursorrules"
framework: "Docker"
language: "Dockerfile / YAML"
category: "DevOps & Infrastructure"
slug: "docker-compose-production-security-cursorrules"
url: "https://www.warplogicai.com/prompts/docker-compose-production-security-cursorrules"
---

# Docker Compose Production Security & Multi-Stage .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add docker-compose-production-security-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-security-cursorrules/raw?tool=cursor > .cursor/rules/docker-compose-production-security-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-security-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-security-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Docker Production Hardening .cursorrules

## Dockerfile Best Practices
- Employ multi-stage builds (`AS builder` -> `AS runner`) to exclude compilation toolchains from the final image.
- Use minimal production base images (`node:22-alpine` or `gcr.io/distroless/nodejs22-debian12`).
- Create and switch to an unprivileged system user (`USER node` or `USER 10001:10001`).
- Never embed credentials in image layers; inject runtime configuration via Docker Compose `secrets`.

