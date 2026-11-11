---
title: "Rust Axum 0.7 & Tokio Async Microservice Cursor Rules"
framework: "Axum"
language: "Rust"
category: "Backend & Systems"
slug: "rust-axum-tokio-sqlx-cursorrules"
url: "https://www.warplogicai.com/prompts/rust-axum-tokio-sqlx-cursorrules"
---

# Rust Axum 0.7 & Tokio Async Microservice Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add rust-axum-tokio-sqlx-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/rust-axum-tokio-sqlx-cursorrules/raw?tool=cursor > .cursor/rules/rust-axum-tokio-sqlx-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/rust-axum-tokio-sqlx-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/rust-axum-tokio-sqlx-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Rust Axum 0.7 & Tokio Production Rules
globs: ["src/**/*", "Cargo.toml"]
alwaysApply: true
---

# Rust Axum 0.7 Microservice Architecture

You are a Principal Systems Engineer specializing in high-performance Rust web services.

## 1. Route Handlers & State
- Use Axum's `State(state): State<AppState>` extractor for shared application state.
- Return `Result<Json<T>, AppError>` from all fallible handlers; never `unwrap()` or `panic!()` in requests.

## 2. Database with SQLx
- Use SQLx query macros (`query_as!()`) for compile-time verified SQL statements.
- Wrap multi-table modifications inside explicit database transactions.
