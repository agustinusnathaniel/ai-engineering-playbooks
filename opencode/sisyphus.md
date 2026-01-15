# oh-my-opencode (sisyphus)

This document describes how to leverage **oh-my-opencode (sisyphus)** as an advanced workflow layer on top of `opencode`.

It is intentionally framed as a **power tool**: useful, sharp, and capable of causing damage if misused.

---

## What Sisyphus Adds on Top of opencode

Sisyphus extends opencode by:
- providing preconfigured prompt workflows
- encouraging iterative, loop-based refinement
- reducing friction when running repeated analysis or generation tasks

It optimizes for **velocity and repetition**, not for correctness or authority.

---

## When to Use Sisyphus

Use sisyphus when:
- you already understand the codebase
- the task is exploratory or iterative
- you want to refine output over multiple passes
- you are comfortable reviewing and correcting outputs

Typical scenarios:
- refining documentation drafts
- iterating on prompts
- exploring alternative structures

---

## When NOT to Use Sisyphus

Avoid sisyphus when:
- defining canonical rules or invariants
- making architectural decisions
- performing sensitive refactors
- working in high-risk or regulated code paths

If correctness and stability matter more than speed, prefer manual control.

---

## Typical Workflows

### Iterative Documentation Refinement

A common pattern:
1. Run an initial opencode pass to generate documentation
2. Use sisyphus to iteratively refine clarity, structure, and tone
3. Manually review and consolidate the final output

Sisyphus shines in the *middle* of the loop, not at the beginning or end.

---

## Failure Modes & Risks

Common risks include:
- reinforcing incorrect assumptions
- amplifying early mistakes through iteration
- producing overly confident but wrong output

These risks increase when:
- prompts are vague
- constraints are not explicit
- canonical guidelines are not referenced

---

## Guardrails

When using sisyphus:
- Always anchor prompts to existing context
- Keep iteration scope small
- Reset and restart when output quality degrades
- Never treat generated output as final without review

Human judgment remains mandatory.

---

## Relationship to Canonical Guidelines

Sisyphus:
- does not define rules
- does not override constraints
- must operate within canonical-guidelines

If a sisyphus workflow conflicts with canonical rules, the workflow is wrong.

---

## Summary

Use oh-my-opencode (sisyphus) to **accelerate iteration**, not to delegate responsibility.

Speed is its strength. Discipline is its requirement.

