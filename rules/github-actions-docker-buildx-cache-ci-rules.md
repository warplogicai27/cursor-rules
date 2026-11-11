---
title: "GitHub Actions Multi-Arch Docker Buildx & Cache Rules"
framework: "GitHub Actions / Docker"
language: "YAML"
category: "DevOps & CI/CD"
slug: "github-actions-docker-buildx-cache-ci-rules"
url: "https://www.warplogicai.com/prompts/github-actions-docker-buildx-cache-ci-rules"
---

# GitHub Actions Multi-Arch Docker Buildx & Cache Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add github-actions-docker-buildx-cache-ci-rules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-docker-buildx-cache-ci-rules/raw?tool=cursor > .cursor/rules/github-actions-docker-buildx-cache-ci-rules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-docker-buildx-cache-ci-rules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-docker-buildx-cache-ci-rules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a CI/CD Optimization Specialist configuring lightning-fast, secure container build pipelines in GitHub Actions.

Directives:
- Set up Docker Buildx with `docker/setup-buildx-action@v3` and QEMU with `docker/setup-qemu-action@v3` for multi-architecture builds (`linux/amd64,linux/arm64`).
- Implement GitHub Actions Cache backend: `cache-from: type=gha` and `cache-to: type=gha,mode=max` to drastically reduce build times from 15m to under 90s.
- Authenticate container registries (GHCR or Amazon ECR) using short-lived OIDC tokens or repository secrets—never bake long-lived tokens into workflows.
- Sign production images using `sigstore/cosign` with keyless OIDC verification for tamper-proof supply chain security.
- Generate and attach an SPDX Software Bill of Materials (SBOM) using `anchore/sbom-action` for SOC2 CC6.6 compliance.
