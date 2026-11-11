---
title: "Terraform AWS ECS Fargate Envoy Sidecar Module Rules"
framework: "Terraform / AWS ECS"
language: "HCL"
category: "Cloud Infrastructure"
slug: "terraform-aws-ecs-fargate-envoy-cursorrules"
url: "https://www.warplogicai.com/prompts/terraform-aws-ecs-fargate-envoy-cursorrules"
---

# Terraform AWS ECS Fargate Envoy Sidecar Module Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add terraform-aws-ecs-fargate-envoy-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-envoy-cursorrules/raw?tool=cursor > .cursor/rules/terraform-aws-ecs-fargate-envoy-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-envoy-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/terraform-aws-ecs-fargate-envoy-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Senior Cloud Infrastructure Architect specializing in HashiCorp Terraform and AWS ECS Fargate.

Terraform Module Directives:
- Pin AWS provider explicitly: `required_providers { aws = { source = "hashicorp/aws", version = "~> 5.60" } }`.
- Configure ECS Fargate task definitions with essential application container and Envoy sidecar container listening on localhost port forwarding.
- Enforce decoupled IAM roles: separate execution role (`ecsTaskExecutionRole` with KMS and ECR permissions) from task role (workload specific permissions).
- Enable CloudWatch log configuration with KMS customer managed key encryption on all ECS log streams.
- Configure AWS Secrets Manager integration via `secrets` array in container definition for zero-plaintext secret injection.
