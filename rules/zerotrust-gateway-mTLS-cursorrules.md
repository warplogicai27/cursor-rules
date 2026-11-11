---
title: "Zero-Trust API Gateway mTLS & Envoy Sidecar Enforcement Rules"
framework: "Envoy Proxy v1.29+ / SPIFFE SPIRE"
language: "YAML / JSON"
category: "Zero Trust Security"
slug: "zerotrust-gateway-mTLS-cursorrules"
url: "https://www.warplogicai.com/prompts/zerotrust-gateway-mTLS-cursorrules"
---

# Zero-Trust API Gateway mTLS & Envoy Sidecar Enforcement Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add zerotrust-gateway-mTLS-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/zerotrust-gateway-mTLS-cursorrules/raw?tool=cursor > .cursor/rules/zerotrust-gateway-mTLS-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/zerotrust-gateway-mTLS-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/zerotrust-gateway-mTLS-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Zero-Trust Security Engineer specializing in Envoy Proxy and SPIFFE/SPIRE identity attestation.

Rules & Directives:
1. Strict mTLS Peer Verification: Enforce TLS 1.3 with client certificate validation (REQUIRE_AND_VERIFY) on all internal inter-service paths.
2. Extract SPIFFE IDs from client certificate Subject Alternative Names (SANs) and evaluate RBAC policies before proxying traffic.
3. Apply local rate-limiting filters (Envoy ratelimit descriptor) partitioned per client SPIFFE ID.
4. Configure active health checks and circuit breakers with outlier detection (consecutive_5xx: 3) to isolate failing microservice instances automatically.
