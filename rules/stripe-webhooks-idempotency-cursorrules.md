---
title: "Stripe Billing & Webhooks Idempotency .cursorrules"
framework: "Stripe SDK"
language: "TypeScript"
category: "API Security"
slug: "stripe-webhooks-idempotency-cursorrules"
url: "https://www.warplogicai.com/prompts/stripe-webhooks-idempotency-cursorrules"
---

# Stripe Billing & Webhooks Idempotency .cursorrules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add stripe-webhooks-idempotency-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/stripe-webhooks-idempotency-cursorrules/raw?tool=cursor > .cursor/rules/stripe-webhooks-idempotency-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/stripe-webhooks-idempotency-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/stripe-webhooks-idempotency-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

# Stripe Webhooks & Idempotency .cursorrules

## Payment Security Rules
- Validate raw request bytes using `stripe.webhooks.constructEvent(rawBody, sig, endpointSecret)` before parsing JSON.
- Store processed event IDs in Redis or database with 7-day TTL (`stripe_events:{id}`) to guarantee strict idempotency.
- Acknowledge webhooks with `HTTP 200` in under 3 seconds; delegate heavy background workflows to asynchronous queues.
- Handle subscription lifecycle events: `customer.subscription.created`, `customer.subscription.updated`, `customer.subscription.deleted`, `invoice.payment_succeeded`.

