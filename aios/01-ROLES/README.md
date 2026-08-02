---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Constitution](../00-CONSTITUTION/README.md)"
  - "[Models](../02-MODELS/README.md)"
  - "[Workflows](../03-WORKFLOWS/README.md)"
Tags: aios, roles, agents, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no role has been defined.
---

# 01 — Roles

Who the agents are, what each is accountable for, and where each one's
authority stops.

> **No documents yet.** No role has been defined, named, or scoped. Sprint 1
> created the destination only.

## Purpose

A role is a bounded job: a mandate, a scope, and an explicit edge. Defining
roles before workflows exists to prevent the common failure where one
undifferentiated agent is asked to research, decide, implement, and review the
same change — and reviews its own work.

Each role document is expected to state four things:

1. **Mandate** — what this role is accountable for producing
2. **Scope** — what it may read and write
3. **Boundary** — what it must hand off rather than do itself
4. **Handoff** — which role receives the work next

## Contents

Currently this README only.

What belongs here:

- One document per role
- A single index naming every role and its mandate in one line

What does not belong here:

- Which model backs a role — that is [02-MODELS](../02-MODELS/README.md)
- The order roles act in — that is [03-WORKFLOWS](../03-WORKFLOWS/README.md)
- Constraints every role shares — those are [00-CONSTITUTION](../00-CONSTITUTION/README.md)

The split matters: a role should survive a change of model, and a workflow
should be describable as a sequence of roles rather than a sequence of prompts.

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

Roles are subordinate to [00-CONSTITUTION](../00-CONSTITUTION/README.md) and
binding on [02-MODELS](../02-MODELS/README.md) and
[03-WORKFLOWS](../03-WORKFLOWS/README.md): a workflow may sequence roles but may
not widen one's scope, and a model assignment may not change what a role is
accountable for.

No role exists, so this section currently grants and constrains nothing.

## Dependencies

| Depends on | Why |
|---|---|
| [00-CONSTITUTION](../00-CONSTITUTION/README.md) | Rules and vocabulary every role inherits |
| [Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md) | Form of every role document |

Sections 02 and 03 depend on this one. Writing a workflow before roles exist
would embed role definitions inside workflow steps, where they cannot be reused
or reviewed.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| `AGENTS.md` | Which roles exist, and what is each accountable for? |
| One file per role | What is this role's mandate, scope, boundary, and handoff? |

Which roles exist at all is an open question. Sprint 1 deliberately does not
propose a roster, because a role list asserted before any workflow is written
would be a guess presented as a design.
