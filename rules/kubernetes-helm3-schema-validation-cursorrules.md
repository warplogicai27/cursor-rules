---
title: "Kubernetes Helm 3 Values Schema Validation & ArgoCD Rules"
framework: "Kubernetes / Helm 3"
language: "YAML / JSON"
category: "Cloud Infrastructure"
slug: "kubernetes-helm3-schema-validation-cursorrules"
url: "https://www.warplogicai.com/prompts/kubernetes-helm3-schema-validation-cursorrules"
---

# Kubernetes Helm 3 Values Schema Validation & ArgoCD Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add kubernetes-helm3-schema-validation-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm3-schema-validation-cursorrules/raw?tool=cursor > .cursor/rules/kubernetes-helm3-schema-validation-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm3-schema-validation-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/kubernetes-helm3-schema-validation-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Principal Kubernetes Platform Engineer specializing in Helm 3 charts and ArgoCD GitOps pipelines.

Helm Chart Architecture:
- Include a strict `values.schema.json` in every chart root to fail `helm lint` and `helm template` builds on invalid configuration variables.
- Always declare resource requests and limits for every pod template: specify `requests.cpu`, `requests.memory`, `limits.cpu`, and `limits.memory`.
- Enforce pod anti-affinity rules (`podAntiAffinity`) to ensure replicas are scheduled across distinct worker nodes for high availability.
- Attach ArgoCD sync wave annotations (`argocd.argoproj.io/sync-wave: "-1"`) for deterministic ordering of CRDs, secrets, and database migrations.
- Restrict network traffic with default-deny Kubernetes `NetworkPolicy` objects.
