# ultracite Playbook

This playbook documents how to use **ultracite** as a complementary analysis tool in AI-assisted engineering workflows.

It focuses on _depth of analysis_ and _signal extraction_, not speed or automation.

---

## What ultracite Is Good At

Use ultracite when you need:

- deeper reasoning over complex code paths
- focused analysis of a specific module or concern
- careful inspection of non-obvious behavior
- validation of assumptions surfaced by other tools

ultracite is most effective when:

- the scope is narrow
- questions are explicit
- correctness matters more than velocity

---

## What ultracite Is NOT For

Do **not** rely on ultracite to:

- bootstrap large repositories
- generate bulk documentation
- replace architectural ownership
- make decisions without context

It is not a discovery tool. It is a refinement tool.

---

## Assumptions

This playbook assumes:

- the codebase structure is already understood at a high level
- canonical-guidelines are known and respected
- outputs will be reviewed by a human

ultracite works best after initial exploration is complete.

---

## Common Usage Patterns

### 1. Focused Code Analysis

Use ultracite to:

- analyze a single module
- understand subtle logic or side effects
- reason about edge cases

This is especially useful for:

- legacy code
- performance-sensitive paths
- correctness-critical logic

---

### 2. Assumption Validation

Use ultracite to:

- verify assumptions made during earlier analysis
- cross-check conclusions from faster tools
- surface hidden constraints

Think of this as a second-pass sanity check.

---

## Guardrails

When using ultracite:

- keep input scope intentionally small
- ask one question at a time
- avoid chaining speculative conclusions
- stop when uncertainty increases

Depth without discipline leads to false confidence.

---

## Failure Modes & Risks

Common risks include:

- overfitting conclusions to a narrow context
- missing system-level interactions
- mistaking detailed output for correctness

Mitigation strategies:

- cross-reference with broader context
- validate against actual code behavior
- involve human review

---

## Relationship to Other Playbooks

- opencode: broad exploration and documentation
- sisyphus (oh-my-opencode): iterative refinement and velocity
- MCP servers: external context enrichment

ultracite complements these tools by providing **focused depth**.

---

## Relationship to Canonical Guidelines

ultracite:

- does not define rules
- does not override invariants
- must operate within canonical-guidelines

If ultracite-derived conclusions conflict with canonical rules, the conclusions are wrong.

---

## Summary

Use ultracite when **precision matters more than speed**.

It is most valuable as a deliberate, second-pass tool.
