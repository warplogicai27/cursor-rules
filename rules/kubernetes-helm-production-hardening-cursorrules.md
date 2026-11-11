---
title: "Kubernetes Helm Chart Security & Hardening .cursorrules"
framework: "Kubernetes"
language: "YAML / Go Templates"
category: "DevOps & Infrastructure"
slug: "kubernetes-helm-production-hardening-cursorrules"
url: "https://www.warplogicai.com/prompts/kubernetes-helm-production-hardening-cursorrules"
---

# Kubernetes Helm Chart Security & Hardening .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add kubernetes-helm-production-hardening-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm-production-hardening-cursorrules/raw?tool=cursor > .cursor/rules/kubernetes-helm-production-hardening-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm-production-hardening-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm-production-hardening-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Kubernetes Helm Hardening .cursorrules

## Security Standards
- Containers must run as non-root: `runAsNonRoot: true`, `runAsUser: 10001`.
- Enforce `readOnlyRootFilesystem: true` with ephemeral `emptyDir` mounts for `/tmp`.
- Drop all Linux capabilities by default: `capabilities: { drop: ['ALL'] }`.
- Explicitly define `resources.limits` and `resources.requests` for both CPU and memory to prevent noisy neighbor starvation.
- Configure `livenessProbe` and `readinessProbe` with appropriate `initialDelaySeconds` and `periodSeconds`.

