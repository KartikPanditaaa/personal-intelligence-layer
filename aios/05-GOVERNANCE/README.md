---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Constitution](../00-CONSTITUTION/README.md)"
  - "[docs/16-decisions](../../docs/16-decisions/README.md)"
  - "[docs/17-rfcs](../../docs/17-rfcs/README.md)"
Tags: aios, governance, amendment, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no governance process has been written.
---

# 05 — Governance

How AIOS itself is changed.

> **No documents yet.** No amendment process exists, which is why nothing
> elsewhere in AIOS is binding. Sprint 1 created the destination only.

## Purpose

Sections 00–04 describe how agents work. This one describes how those
descriptions change: who may propose an amendment, what evidence is required,
who decides, and where the reasoning is kept afterwards.

It carries the load-bearing definition of what ratification means. Until that
is written, [00-CONSTITUTION](../00-CONSTITUTION/README.md) can hold rules but
cannot make them binding, because there is no defined act that turns a proposed
rule into a settled one.

The repository's existing ground rule applies here without modification:
rationale is never deleted. A superseded rule is marked and linked forward, not
removed.

## Contents

Currently this README only.

What belongs here:

- The amendment process, from proposal to ratification
- AIOS decision records and RFCs
- Version history for AIOS as a whole

What does not belong here:

- **Product decisions and RFCs.** Those live in
  [docs/16-decisions](../../docs/16-decisions/README.md) and
  [docs/17-rfcs](../../docs/17-rfcs/README.md). A decision about how agents work
  is not a decision about what gets built, and the two records are kept
  separate so neither is read as the other.
- The rules themselves — those are [00-CONSTITUTION](../00-CONSTITUTION/README.md)

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

This section governs changes to all of AIOS, including
[00-CONSTITUTION](../00-CONSTITUTION/README.md) and including itself. That is a
deliberate circularity: the first version of the amendment process cannot be
ratified by a process that does not yet exist, so it is adopted by founder
decision and amendable thereafter by its own terms.

Governance has no authority over product substance. An AIOS amendment cannot
change anything in [`docs/`](../../docs/README.md).

## Dependencies

| Depends on | Why |
|---|---|
| [00-CONSTITUTION](../00-CONSTITUTION/README.md) | An amendment process needs something to amend |
| [docs/18-templates](../../docs/18-templates/README.md) | Existing ADR and RFC forms to reuse or deliberately fork |
| [docs/16-decisions](../../docs/16-decisions/README.md) | Precedent for how decisions are recorded here |

Every other AIOS section depends on this one for the meaning of "ratified".

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| Amendment process | Who proposes, who decides, what evidence is required? |
| AIOS decision records | What was decided about AIOS, when, by whom, on what basis? |
| AIOS RFCs | What substantial changes are open for disagreement? |
| Version history | What changed between AIOS versions, and why? |

Whether AIOS records live here or as a tagged subset of
[docs/16-decisions](../../docs/16-decisions/README.md) is unresolved. Separate
records keep operating decisions out of the product log; a shared log keeps one
place to look.
