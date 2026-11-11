---
title: "Terraform AWS ECS Fargate Module Rules"
framework: "Terraform 1.8+ / AWS"
language: "HCL"
category: "Cloud Infrastructure"
slug: "terraform-aws-ecs-fargate-module-cursorrules"
url: "https://www.warplogicai.com/prompts/terraform-aws-ecs-fargate-module-cursorrules"
---

# Terraform AWS ECS Fargate Module Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add terraform-aws-ecs-fargate-module-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-module-cursorrules/raw?tool=cursor > .cursor/rules/terraform-aws-ecs-fargate-module-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-module-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-module-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an AWS Cloud Infrastructure Architect expert in HashiCorp Terraform and ECS Fargate.

Rules & Directives:
1. Provider & Version Constraints: Require explicit required_providers with AWS provider version ~> 5.0. Pin exact Terraform version in required_version = ">= 1.7.0".
2. ECS Task Execution & Security: Enforce separate IAM roles for execution_role_arn (image pulling, CloudWatch) and task_role_arn (runtime app permissions).
3. Enable AWS KMS customer-managed encryption for CloudWatch log groups and ECS task storage volumes.
4. Networking & Load Balancing: Deploy ECS tasks into private subnets only; route public traffic exclusively via Application Load Balancers.
