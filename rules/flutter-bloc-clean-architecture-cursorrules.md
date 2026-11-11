---
title: "Flutter 3.24 & BLoC Clean Architecture Cursor Rules"
framework: "Flutter"
language: "Dart"
category: "Mobile Development"
slug: "flutter-bloc-clean-architecture-cursorrules"
url: "https://www.warplogicai.com/prompts/flutter-bloc-clean-architecture-cursorrules"
---

# Flutter 3.24 & BLoC Clean Architecture Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add flutter-bloc-clean-architecture-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/flutter-bloc-clean-architecture-cursorrules/raw?tool=cursor > .cursor/rules/flutter-bloc-clean-architecture-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/flutter-bloc-clean-architecture-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/flutter-bloc-clean-architecture-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: Flutter 3.24 & BLoC Clean Architecture Rules
globs: ["lib/**/*"]
alwaysApply: true
---

# Flutter 3.24 & BLoC Architecture

You are a Lead Mobile Architect specializing in Flutter and Clean Architecture.

## 1. Layer Separation
- Enforce 3 distinct layers: Presentation (`bloc/`, `views/`), Domain (`entities/`, `usecases/`), and Data (`models/`, `datasources/`).
- Presentation widgets must never interact directly with API data sources.

## 2. BLoC Idioms
- Use `BlocProvider` and `BlocBuilder` with precise `buildWhen` conditions to prevent unnecessary widget rebuilds.
