# opencode Playbook

This playbook documents **practical usage patterns** for working with `opencode` in real-world projects.

It focuses on *how* to leverage opencode effectively, not on defining rules or constraints.

---

## What opencode Is Good At

Use opencode when you want to:
- Initialize or improve project documentation
- Analyze an existing codebase holistically
- Apply consistent structure across files
- Assist large refactors with context awareness

opencode excels when the task requires:
- scanning many files
- reasoning about project structure
- generating or aligning documentation artifacts

---

## What opencode Is NOT For

Do **not** rely on opencode to:
- define canonical rules or invariants
- replace architectural decisions
- enforce security policies
- make irreversible changes without review

opencode is a *co-pilot*, not an authority.

---

## Assumptions

This playbook assumes:
- canonical-guidelines are already applied or referenced
- the repository has a clear scope
- humans remain responsible for final decisions

If canonical rules exist, opencode should be guided to **respect and reference them**, not recreate them.

---

## Common Usage Patterns

### 1. Documentation Initialization

Use opencode to:
- scan the repository
- infer structure and responsibilities
- generate or enhance documentation files

This works best when combined with a clear prompt that:
- references canonical-guidelines
- states explicit expected outputs

### 2. Documentation Alignment

Use opencode to:
- align README, SPEC, CONTRIBUTING, and AGENTS files
- reduce drift between documents
- surface implicit assumptions

### 3. Exploratory Analysis

Use opencode to:
- understand unfamiliar codebases
- summarize modules and dependencies
- identify architectural boundaries

---

## Guardrails

When using opencode:
- Always review generated output
- Avoid blindly accepting large diffs
- Prefer incremental application
- Treat suggestions as drafts

---

## Relationship to Other Playbooks

- oh-my-opencode / sisyphus: advanced workflows built on top of opencode
- ultracite: complementary tooling for deeper analysis
- MCP servers: extend context, not authority

---

## Summary

Use opencode to **amplify understanding and consistency**, not to outsource responsibility.

When in doubt, defer to:
- canonical-guidelines for rules
- humans for judgment

