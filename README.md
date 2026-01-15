# AI Engineering Playbooks

This repository contains **practical, evolving playbooks** for leveraging AI engineering tools and workflows in real projects.

It exists to document **how to use tools well**, not to define rules.

---

## Scope

This repository focuses on:

- Tool setup and usage
- Practical workflows
- Integration patterns
- Operational guidance

Examples include:

- [opencode](https://opencode.ai) + [oh-my-opencode (sisyphus)](https://github.com/code-yeongyu/oh-my-opencode)
- [ultracite](https://ultracite.ai)
- MCP servers

The content here is intentionally **opinionated but optional**.

---

## Non-Goals

This repository does **not**:

- Define canonical rules or invariants
- Replace engineering judgment
- Override project-level documentation
- Act as a source of truth for constraints

Authoritative rules live in the **canonical-guidelines** repository.

Related inspirations:

- [Vercel Agent Skills](https://github.com/vercel-labs/agent-skills)
- [Introducing React Best Practices](https://vercel.com/blog/introducing-react-best-practices)

---

## Relationship to Canonical Guidelines

All playbooks in this repository:

- Assume canonical guidelines are already understood
- Must not contradict or override canonical rules
- May reference canonical guidelines for context

Think of this repository as a **toolbox**, not a constitution.

---

## Structure

Each tool or ecosystem has its own folder:

```
/ai-engineering-playbooks
  /opencode
  /ultracite
  /mcp
```

Each folder contains focused documentation specific to that tool.

---

## How to Use This Repository

In a project:

- Reference **canonical-guidelines** for rules and invariants
- Optionally reference **ai-engineering-playbooks** for workflows and setup

Example:

> This project follows canonical-guidelines. Tooling workflows may optionally follow patterns from ai-engineering-playbooks.

---

## How Agents Should Read This Repository

This repository is written for **humans first**, agents second.

Agents should treat this repository as:

- operational guidance
- suggested workflows
- contextual playbooks

Not as:

- hard constraints
- absolute rules
- a source of truth

### Reading Order for Agents

1. Assume **canonical-guidelines** are already known
2. Read only the folder relevant to the active tool
3. Follow guardrails and assumptions explicitly
4. Defer to project-level documentation on conflicts

### Conflict Resolution

If there is a conflict:

1. Project documentation wins
2. Canonical-guidelines win over this repo
3. Human judgment wins over all outputs

This repository is intentionally permissive.

Agents should optimize for:

- correctness
- clarity
- reversibility

Not for blind automation.

---

## Philosophy

- Prefer clarity over cleverness
- Prefer stable guidance over novelty
- Prefer small, composable playbooks
- Avoid coupling to a single AI IDE or agent

---

## Status

This repository is expected to evolve. Breaking changes are acceptable. Stability is provided by canonical-guidelines, not by this repo.
