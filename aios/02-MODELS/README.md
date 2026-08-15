---
Status: Stub
Owner: Founder
Last Updated: 2026-08-11
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Roles](../01-ROLES/README.md)"
  - "[Workflows](../03-WORKFLOWS/README.md)"
  - "[Governance](../05-GOVERNANCE/README.md)"
  - "[docs/05-ai](../../docs/05-ai/README.md)"
Tags: aios, models, adapters, stub
Source: AIOS v0.1.0 Sprint 1, amended per the Sprint 1 governance resolution draft (proposed, founder approval pending). No model adapter has been written.
---

# 02 - Models

One operating-notes file per model vendor: its capabilities, its quirks, and
how it is invoked within AIOS.

> **No documents yet.** No model adapter has been written. Sprint 1 created
> the destination only.

## Purpose

This section holds per-vendor adapters, not a routing or assignment policy.
Each expected document (`claude.md`, `codex.md`, `gemini.md`, `chatgpt.md`)
is a fixed point about one model: what it is good at, what it gets wrong,
what context it needs, and how it is invoked. It answers "how do I work with
this model," not "which model should this role use."

Whether AIOS needs a separate routing, assignment, or fallback policy layer -
and if so, where it lives - is unresolved. It does not default to living
here. This section governs by convention until a decision is made through
[05-GOVERNANCE](../05-GOVERNANCE/README.md).

## Contents

Currently this README only.

What belongs here:

- One adapter document per model vendor
- Known capabilities, limitations, and invocation quirks for that model
- Nothing that assumes a specific role or workflow is using it

What does not belong here:

- **The product's** model strategy. That is
  [docs/05-ai](../../docs/05-ai/README.md), which covers which models the
  Personal Intelligence Layer ships to users. This section covers which models
  build it. The two may reach different answers and should not be merged.
- Role-to-model assignment, routing, or fallback policy. That question is
  unresolved and does not belong here by default - see Purpose above.
- Prompts. Those are [03-WORKFLOWS](../03-WORKFLOWS/README.md).

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

Adapters are subordinate to [00-CONSTITUTION](../00-CONSTITUTION/README.md):
an adapter may describe how a model behaves, not authorize it to break a
rule. [03-WORKFLOWS](../03-WORKFLOWS/README.md) may consume an adapter's
notes when a step names a model; this section does not decide which model a
step uses.

Per [Document Standards § 8](../../docs/18-templates/DOCUMENT_STANDARDS.md), any
benchmark, cost, or latency figure recorded here carries a citation. Model
claims age quickly and an uncited one cannot be re-checked.

## Dependencies

| Depends on | Why |
|---|---|
| [00-CONSTITUTION](../00-CONSTITUTION/README.md) | Rules constraining what any model may be asked to do |
| [docs/05-ai](../../docs/05-ai/README.md) | Adjacent, not authoritative - read before writing to avoid contradiction |

[03-WORKFLOWS](../03-WORKFLOWS/README.md) may reference this section; nothing
requires it to exist first.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| `claude.md` | What are Claude's capabilities, limitations, and invocation notes within AIOS? |
| `codex.md` | Same, for Codex. |
| `gemini.md` | Same, for Gemini. |
| `chatgpt.md` | Same, for ChatGPT. |

Whether "models" here should also cover embedding and retrieval models, or
only generation models, is unresolved. Whether a routing, assignment, or
fallback policy is needed at all - and where it would live if so - is also
unresolved; see Purpose above.
