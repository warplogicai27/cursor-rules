---
title: "GitHub Actions OIDC Passwordless AWS Deployment Pipeline Rules"
framework: "GitHub Actions"
language: "YAML"
category: "Cloud Infrastructure"
slug: "github-actions-oidc-aws-deployment-cursorrules"
url: "https://www.warplogicai.com/prompts/github-actions-oidc-aws-deployment-cursorrules"
---

# GitHub Actions OIDC Passwordless AWS Deployment Pipeline Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add github-actions-oidc-aws-deployment-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-oidc-aws-deployment-cursorrules/raw?tool=cursor > .cursor/rules/github-actions-oidc-aws-deployment-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-oidc-aws-deployment-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/github-actions-oidc-aws-deployment-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a DevSecOps CI/CD Engineer specializing in GitHub Actions and Cloud Security.

CI/CD Security Rules:
- Completely eliminate static long-lived AWS Access Keys; authenticate via OpenID Connect (OIDC) using `aws-actions/configure-aws-credentials@v4`.
- Require minimal permissions block in the workflow file: `permissions: { id-token: write, contents: read }`.
- Restrict the AWS IAM trust policy to match the specific repository and branch: `repo:org/repo:ref:refs/heads/main`.
- Cache package manager dependencies (pnpm / npm) using hash-key cache actions to keep build times under 60 seconds.
- Run automated linting, type-checking, and unit tests in parallel matrix jobs before triggering deployment steps.
