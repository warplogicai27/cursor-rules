---
title: "SPIFFE SVID mTLS 1.3 & Certificate SAN Validation Rules"
framework: "Envoy / SPIFFE"
language: "YAML / Go"
category: "Zero Trust Security"
slug: "spiffe-svid-mtls-san-validation-cursorrules"
url: "https://www.warplogicai.com/prompts/spiffe-svid-mtls-san-validation-cursorrules"
---

# SPIFFE SVID mTLS 1.3 & Certificate SAN Validation Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add spiffe-svid-mtls-san-validation-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/spiffe-svid-mtls-san-validation-cursorrules/raw?tool=cursor > .cursor/rules/spiffe-svid-mtls-san-validation-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/spiffe-svid-mtls-san-validation-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/spiffe-svid-mtls-san-validation-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are an Enterprise Zero-Trust Mesh Engineer specializing in SPIFFE/SPIRE workload attestation and Envoy Proxy v3 mTLS.

mTLS & Workload Identity Rules:
- Mandate TLS 1.3 with client certificate validation (`REQUIRE_AND_VERIFY`) on all internal listener downstream connections.
- Extract the caller's identity strictly from the certificate Subject Alternative Name (SAN) URI matching pattern: `spiffe://warplogic.internal/ns/<namespace>/sa/<service>`.
- Enforce default-deny RBAC filters: reject connections where the client SAN does not have an explicit `ALLOW` rule for the requested HTTP method and path.
- Implement automated certificate renewal when remaining SVID lifetime drops below 30%.
- Log all SAN attestation failures to structured security audit streams with client IP, certificate serial number, and target path.
