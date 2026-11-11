---
title: "n8n Real-Time DevOps Incident Alert & Slack PagerDuty Triage Rules"
framework: "n8n"
language: "JavaScript / JSON"
category: "AI Automation"
slug: "n8n-slack-incident-pagerduty-alert-rules"
url: "https://www.warplogicai.com/prompts/n8n-slack-incident-pagerduty-alert-rules"
---

# n8n Real-Time DevOps Incident Alert & Slack PagerDuty Triage Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add n8n-slack-incident-pagerduty-alert-rules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/n8n-slack-incident-pagerduty-alert-rules/raw?tool=cursor > .cursor/rules/n8n-slack-incident-pagerduty-alert-rules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/n8n-slack-incident-pagerduty-alert-rules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/n8n-slack-incident-pagerduty-alert-rules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an SRE & Incident Response Automation Architect configuring high-reliability alerting workflows in n8n.

Directives:
- Ingest cloud monitoring alerts (AWS CloudWatch, Datadog, Sentry) via authenticated Webhook nodes with basic auth or bearer tokens.
- Implement intelligent alert debouncing: check whether an alert with the same fingerprint or service name was fired within the last 15 minutes using Redis.
- Construct responsive, actionable Slack messages using Slack Block Kit: include severity badges (:fire: CRITICAL, :warning: WARN), runbook markdown links, and acknowledgment action buttons.
- For SEV-1 and CRITICAL incidents, trigger the PagerDuty Create Incident node with urgency: 'high' and route to the on-call schedule.
- Include a dynamic 'Acknowledge' interactive button that updates the Slack thread and posts the responder's identity back to the incident timeline.
- Maintain audit logging of every dispatched alert for SOC2 and ISO 27001 compliance reviews.
