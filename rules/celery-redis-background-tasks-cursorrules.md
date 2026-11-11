---
title: "Cursor Rules for Celery & Redis Asynchronous Task Queues"
framework: "Celery / Redis"
language: "Python 3.12"
category: "Distributed Systems"
slug: "celery-redis-background-tasks-cursorrules"
url: "https://www.warplogicai.com/prompts/celery-redis-background-tasks-cursorrules"
---

# Cursor Rules for Celery & Redis Asynchronous Task Queues

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add celery-redis-background-tasks-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/celery-redis-background-tasks-cursorrules/raw?tool=cursor > .cursor/rules/celery-redis-background-tasks-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/celery-redis-background-tasks-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/celery-redis-background-tasks-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Distributed Systems Engineer expert in Celery task execution.

Code Style & Rules:
- Annotate tasks with @shared_task or @celery_app.task.
- Enforce automatic retries with exponential backoff using autoretry_for and retry_backoff.
- Make task parameters JSON-serializable (strings, numbers, dicts).
- Configure Celery beat schedule dynamically inside config module.
