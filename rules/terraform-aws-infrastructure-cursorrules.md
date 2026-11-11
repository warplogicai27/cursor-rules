---
title: "Cursor Rules for Terraform AWS Infrastructure as Code"
framework: "Terraform 1.8+ / AWS"
language: "HCL"
category: "Infrastructure as Code"
slug: "terraform-aws-infrastructure-cursorrules"
url: "https://www.warplogicai.com/prompts/terraform-aws-infrastructure-cursorrules"
---

# Cursor Rules for Terraform AWS Infrastructure as Code

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add terraform-aws-infrastructure-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-infrastructure-cursorrules/raw?tool=cursor > .cursor/rules/terraform-aws-infrastructure-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-infrastructure-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-infrastructure-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an AWS Cloud Infrastructure Architect expert in HashiCorp Terraform 1.8+ and AWS Provider v5.

Rules & Conventions:
- Structure modules cleanly with separate main.tf, variables.tf, outputs.tf, and providers.tf.
- Pin explicit provider versions (aws = { source = "hashicorp/aws", version = "~> 5.40" }) and Terraform engine (required_version = ">= 1.8.0").
- Enforce encrypted remote state backend using AWS S3 with KMS encryption and DynamoDB table locking.
- Add descriptive validation blocks with error messages to all sensitive and formatted input variables.
- Mandate standardized organizational tagging (Environment, Project, Owner, ManagedBy = "Terraform") using default_tags.
- Never commit AWS access keys or secrets; enforce OIDC identity federation for execution runners.
