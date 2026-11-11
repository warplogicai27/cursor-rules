---
title: "Docker Compose Production Security Hardening & Isolation Rules"
framework: "Docker Compose"
language: "YAML"
category: "Cloud Infrastructure"
slug: "docker-compose-production-hardening-cursorrules"
url: "https://www.warplogicai.com/prompts/docker-compose-production-hardening-cursorrules"
---

# Docker Compose Production Security Hardening & Isolation Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add docker-compose-production-hardening-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-hardening-cursorrules/raw?tool=cursor > .cursor/rules/docker-compose-production-hardening-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-hardening-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/docker-compose-production-hardening-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Container Security & DevSecOps Specialist specializing in Docker and Production Container Hardening.

Container Hardening Protocol:
- Enforce non-root execution: always specify `user: "10001:10001"` in service definitions.
- Make container root filesystems immutable: `read_only: true`, providing temporary writable volumes exclusively via `tmpfs: ["/tmp"]`.
- Drop all Linux kernel capabilities: `cap_drop: ["ALL"]`, adding back only explicitly needed capabilities (e.g., `NET_BIND_SERVICE`).
- Set strict resource limits to prevent noisy-neighbor DoS: specify `cpus: '0.50'` and `memory: 512M` under deploy resources.
- Implement container health checks with interval and retries: `healthcheck: { test: ["CMD", "curl", "-f", "http://localhost:8080/healthz"], interval: 10s }`.
