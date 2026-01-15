# MCP Playbook

This playbook explains how to reason about and leverage **MCP (Model Context Protocol)** servers in AI-assisted development workflows.

It focuses on *conceptual correctness* and *safe usage patterns*, not on implementation details.

---

## What MCP Is

MCP is a protocol that allows AI agents and IDEs to:
- access external context
- query structured data or services
- extend their understanding beyond the local repository

An MCP server provides **additional context**, not instructions or authority.

---

## What MCP Is Good At

Use MCP servers to:
- expose reference documentation
- surface structured domain knowledge
- provide read-only access to external systems
- enrich agent understanding with controlled context

MCP works best when:
- context is stable
- interfaces are explicit
- permissions are constrained

---

## What MCP Is NOT For

Do **not** use MCP servers to:
- encode canonical rules
- bypass code review or human approval
- execute destructive actions by default
- inject mutable or unbounded context

MCP should extend *visibility*, not *power*.

---

## Common Usage Patterns

### 1. Reference Context

Expose:
- canonical documentation
- internal handbooks
- API references

This allows agents to reason with shared knowledge without duplicating it.

### 2. Structured Queries

Provide:
- bounded query interfaces
- deterministic outputs
- clear schemas

Avoid free-form or side-effectful endpoints.

---

## Guardrails

When working with MCP servers:
- prefer read-only access
- keep scopes narrow
- document exposed capabilities
- assume agents may misunderstand intent

Every exposed capability should be treated as a public API.

---

## Failure Modes & Risks

Common risks include:
- leaking sensitive context
- introducing stale or misleading data
- overloading agents with irrelevant information

Mitigation strategies:
- explicit scoping
- documentation-first design
- conservative defaults

---

## Relationship to Canonical Guidelines

MCP servers:
- may expose canonical documentation
- must not redefine canonical rules
- must defer to canonical-guidelines for authority

If MCP-provided context conflicts with canonical rules, the MCP context is wrong.

---

## Summary

Use MCP to **expand context safely**.

The value of MCP comes from discipline, not from reach.