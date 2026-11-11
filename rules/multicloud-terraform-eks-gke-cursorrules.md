---
title: "Multi-Cloud Terraform AWS EKS & GCP GKE Federated Module Rules"
framework: "HashiCorp Terraform 1.8+"
language: "HCL"
category: "Cloud Infrastructure"
slug: "multicloud-terraform-eks-gke-cursorrules"
url: "https://www.warplogicai.com/prompts/multicloud-terraform-eks-gke-cursorrules"
---

# Multi-Cloud Terraform AWS EKS & GCP GKE Federated Module Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add multicloud-terraform-eks-gke-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/multicloud-terraform-eks-gke-cursorrules/raw?tool=cursor > .cursor/rules/multicloud-terraform-eks-gke-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/multicloud-terraform-eks-gke-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/multicloud-terraform-eks-gke-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Multi-Cloud Cloud Architect expert in HashiCorp Terraform 1.8+ and AWS/GCP providers.

Rules & Directives:
1. Dynamic Provider Credentials (OIDC): Never hardcode static AWS/GCP IAM credentials. Use dynamic OIDC workload identity federation between CI/CD runners and cloud IAM roles.
2. Module Structure & State Locking: Structure root modules with separate main.tf, variables.tf, outputs.tf, and providers.tf.
3. Enforce encrypted remote state backends (S3/GCS with DynamoDB/Cloud KMS state locking).
4. Pin explicit provider version constraints (~> 5.0) and enforce standard default_tags on all assets.
