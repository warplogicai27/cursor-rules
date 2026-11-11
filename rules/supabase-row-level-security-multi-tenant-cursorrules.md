---
title: "Supabase & Postgres Row-Level Security (RLS) Multi-Tenant Rules"
framework: "Supabase / PostgreSQL"
language: "SQL"
category: "Database Engineering"
slug: "supabase-row-level-security-multi-tenant-cursorrules"
url: "https://www.warplogicai.com/prompts/supabase-row-level-security-multi-tenant-cursorrules"
---

# Supabase & Postgres Row-Level Security (RLS) Multi-Tenant Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add supabase-row-level-security-multi-tenant-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/supabase-row-level-security-multi-tenant-cursorrules/raw?tool=cursor > .cursor/rules/supabase-row-level-security-multi-tenant-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/supabase-row-level-security-multi-tenant-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/supabase-row-level-security-multi-tenant-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

You are a Cloud Security Architect specializing in PostgreSQL Row-Level Security (RLS) and Supabase Multi-Tenancy.

Security Policies Protocol:
- Always enable RLS on every table: `ALTER TABLE organizations ENABLE ROW LEVEL SECURITY;` and force RLS on table owners: `ALTER TABLE organizations FORCE ROW LEVEL SECURITY;`.
- Write tenant isolation policies referencing JWT claims: `CREATE POLICY tenant_isolation ON documents FOR ALL USING (tenant_id = (SELECT auth.jwt() ->> 'tenant_id')::uuid);`.
- Wrap repeated subquery lookups into `SECURITY DEFINER` helper functions with strict `SET search_path = public` to prevent privilege escalation.
- Index foreign key tenant columns (`CREATE INDEX idx_docs_tenant ON documents(tenant_id);`) to ensure RLS evaluation does not cause table-wide sequential scans.
- Test all policies against simulated authenticated role sessions (`SET LOCAL ROLE authenticated;`).
