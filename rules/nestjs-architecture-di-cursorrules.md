---
title: "Cursor Rules for NestJS Enterprise Architecture & DI"
framework: "NestJS"
language: "TypeScript / Node.js"
category: "Backend API"
slug: "nestjs-architecture-di-cursorrules"
url: "https://www.warplogicai.com/prompts/nestjs-architecture-di-cursorrules"
---

# Cursor Rules for NestJS Enterprise Architecture & DI

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add nestjs-architecture-di-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/nestjs-architecture-di-cursorrules/raw?tool=cursor > .cursor/rules/nestjs-architecture-di-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/nestjs-architecture-di-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/nestjs-architecture-di-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an expert NestJS Architect enforcing modular, clean architecture.

Code Style & Rules:
- Organize application feature domain modules into separate directories (Controller, Service, Module, DTO).
- Always define class-validator and class-transformer DTOs for request payloads.
- Use Custom Exceptions extending HttpException for predictable HTTP error responses.
- Implement Auth Guards and Role-based decorators for endpoint protection.
- Write unit tests for services using Jest and @nestjs/testing module mocks.
- Enable global validation pipe in main.ts with whitelist: true and forbidNonWhitelisted: true.
