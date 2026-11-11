---
title: "AWS CDK v2 Serverless & Lambda Powertools .cursorrules"
framework: "AWS CDK"
language: "TypeScript"
category: "Cloud Infrastructure"
slug: "aws-cdk-v2-serverless-typescript-cursorrules"
url: "https://www.warplogicai.com/prompts/aws-cdk-v2-serverless-typescript-cursorrules"
---

# AWS CDK v2 Serverless & Lambda Powertools .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add aws-cdk-v2-serverless-typescript-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/aws-cdk-v2-serverless-typescript-cursorrules/raw?tool=cursor > .cursor/rules/aws-cdk-v2-serverless-typescript-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/aws-cdk-v2-serverless-typescript-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/aws-cdk-v2-serverless-typescript-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# AWS CDK v2 Serverless .cursorrules

## Construct Standards
- Target ARM64 Graviton architecture (`Architecture.ARM_64`) for 20-30% cost and compute savings.
- Use `NodejsFunction` with esbuild bundling, source maps enabled, and minify enabled for production.
- Implement Least-Privilege IAM: grant granular table or bucket access (`table.grantReadWriteData(fn)`) rather than wildcards.
- Enable AWS Lambda Powertools for structured JSON logging, distributed tracing (X-Ray), and CloudWatch embedded metrics.

