# MCP Servers Playbook

This playbook documents how **MCP (Model Context Protocol) servers** are used to enrich AI-assisted engineering workflows with **external, authoritative context**.

MCP servers extend an agent’s capabilities by giving it structured access to tools, libraries, and live knowledge sources.

This playbook focuses on *when* and *why* to use MCP servers, not on setup mechanics.

---

## What MCP Servers Are Good At

Use MCP servers when you need:
- authoritative information from external tools or libraries
- up-to-date knowledge that does not live in the repository
- precise API, component, or framework references
- reduction of hallucination risk

MCP servers are most effective when:
- the source is trusted and well-scoped
- the question is concrete
- local code context alone is insufficient

---

## What MCP Servers Are NOT For

Do **not** rely on MCP servers to:
- replace reading the actual code
- make architectural decisions
- infer undocumented conventions
- compensate for unclear requirements

MCP servers provide context, not judgment.

---

## Assumptions

This playbook assumes:
- canonical-guidelines are known and respected
- MCP usage is intentional, not automatic
- outputs are validated against local context

External truth must still be integrated carefully.

---

## Common MCP Servers in Use

Below are MCP servers commonly used across projects. Availability may vary by environment or IDE.

### UI & Component Libraries

- **shadcn**: Component patterns and CLI-driven primitives
- **HeroUI (React / Native)**: Design system components for web and mobile
- **Chakra UI**: Accessible React component library
- **React Aria**: Accessibility-first component primitives

Use these when:
- referencing component APIs
- confirming usage patterns
- aligning with design system constraints

---

### Framework & Tooling

- **next-devtools**: Next.js-specific debugging and conventions
- **Playwright**: Browser automation and testing APIs

Use these when:
- validating framework-specific behavior
- generating or reviewing test logic

---

### Code & Knowledge Search

- **GitHub MCP**: Repository-level search and metadata
- **grep.app**: Cross-repository code search

Use these when:
- looking for real-world usage examples
- validating patterns across projects

---

### Analysis & Reasoning

- **ultracite MCP**: Remote deep-analysis and reasoning support

Use this when:
- validating assumptions
- performing second-pass analysis
- correctness matters more than speed

---

## Usage Patterns

### 1. Context Enrichment

Use MCP servers to:
- fetch authoritative definitions
- confirm APIs and interfaces
- ground reasoning in real references

This reduces hallucination and guesswork.

---

### 2. Cross-Validation

Use MCP servers to:
- verify conclusions drawn from local code
- compare patterns against external sources

Think of this as an external consistency check.

---

## Guardrails

When using MCP servers:
- prefer trusted and official sources
- avoid mixing conflicting external guidance
- always reconcile with local code
- stop if results introduce ambiguity

External context should clarify, not confuse.

---

## Failure Modes & Risks

Common risks include:
- blindly trusting external examples
- version mismatches
- importing patterns that do not fit the codebase

Mitigation strategies:
- check versions explicitly
- adapt patterns intentionally
- defer to project constraints

---

## Relationship to Other Playbooks

- opencode: discovers structure and generates drafts
- ultracite: performs focused deep analysis
- sisyphus: accelerates iterative refinement

MCP servers **augment** these tools with external truth.

---

## Relationship to Canonical Guidelines

MCP servers:
- do not define rules
- do not override invariants
- must operate within canonical-guidelines

If external guidance conflicts with canonical rules, canonical rules win.

---

## Summary

Use MCP servers when **local context is insufficient** and correctness depends on authoritative external knowledge.

They are most valuable when used deliberately and sparingly.

