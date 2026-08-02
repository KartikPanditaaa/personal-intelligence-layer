---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Roles](../01-ROLES/README.md)"
  - "[Workflows](../03-WORKFLOWS/README.md)"
  - "[docs/05-ai](../../docs/05-ai/README.md)"
Tags: aios, models, routing, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no model policy has been written.
---

# 02 — Models

Which model backs which role, on what basis, and what happens when it is the
wrong one.

> **No documents yet.** No model has been selected, compared, or assigned.
> Sprint 1 created the destination only.

## Purpose

Roles describe accountability; this section describes the machinery a role runs
on. Keeping the two apart means a model can be swapped without renegotiating
what anyone is responsible for.

Three questions belong here:

- **Assignment** — which model backs which role, and why that one
- **Routing** — how a task is matched to a capability tier
- **Failure** — what happens when a model is unavailable, refuses, or is wrong

The third is the one most often skipped. A model policy that only covers the
happy path is not a policy.

## Contents

Currently this README only.

What belongs here:

- Selection criteria and the evidence behind each choice
- Role-to-model assignments, with a stated basis per assignment
- Fallback and escalation behaviour
- How assignments get re-evaluated as models change

What does not belong here:

- **The product's** model strategy. That is
  [docs/05-ai](../../docs/05-ai/README.md), which covers which models the
  Personal Intelligence Layer ships to users. This section covers which models
  build it. The two may reach different answers and should not be merged.
- Prompts. Those are [03-WORKFLOWS](../03-WORKFLOWS/README.md).

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

Model assignments are subordinate to [01-ROLES](../01-ROLES/README.md): choosing
a model may not alter a role's mandate or widen its scope. Assignments bind
[03-WORKFLOWS](../03-WORKFLOWS/README.md), which consume them rather than
setting them.

Per [Document Standards § 8](../../docs/18-templates/DOCUMENT_STANDARDS.md), any
benchmark, cost, or latency figure recorded here carries a citation. Model
claims age quickly and an uncited one cannot be re-checked.

## Dependencies

| Depends on | Why |
|---|---|
| [01-ROLES](../01-ROLES/README.md) | There is nothing to assign a model to until roles exist |
| [00-CONSTITUTION](../00-CONSTITUTION/README.md) | Rules constraining what any model may be asked to do |
| [docs/05-ai](../../docs/05-ai/README.md) | Adjacent, not authoritative — read before writing to avoid contradiction |

[03-WORKFLOWS](../03-WORKFLOWS/README.md) depends on this section.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| Selection criteria | On what basis is a model chosen for a role? |
| Role-to-model assignments | Which model backs which role today, and why? |
| Routing and fallback policy | What happens when the assigned model is unavailable or wrong? |
| Re-evaluation cadence | When are assignments revisited, and what triggers it? |

Whether "models" here should also cover embedding and retrieval models, or only
generation models, is unresolved.
