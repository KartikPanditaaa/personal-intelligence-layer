---
Status: Stub
Owner: Founder
Last Updated: 2026-08-11
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Constitution](../00-CONSTITUTION/README.md)"
  - "[Templates](../04-TEMPLATES/README.md)"
  - "[docs/16-decisions](../../docs/16-decisions/README.md)"
  - "[docs/17-rfcs](../../docs/17-rfcs/README.md)"
  - "[Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md)"
Tags: aios, governance, amendment, stub
Source: AIOS v0.1.0 Sprint 1, amended per the Sprint 1 governance resolution draft (proposed, founder approval pending). No governance process has been written.
---

# 05 - Governance

How AIOS itself is changed.

> **No documents yet.** No amendment process exists, which is why nothing
> elsewhere in AIOS is binding. Sprint 1 created the destination only.

## Purpose

Sections 00-04 describe how agents work. This one describes how those
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
- Version history for AIOS as a whole

What does not belong here:

- **AIOS decision records and RFCs, as a second artifact store.** AIOS does
  not maintain its own decision or RFC log. A decision or proposal about how
  agents work is recorded as a normal entry in
  [docs/16-decisions](../../docs/16-decisions/README.md) or
  [docs/17-rfcs](../../docs/17-rfcs/README.md), tagged as AIOS so it is
  distinguishable from a product decision. This section owns the amendment
  *process*; it does not own a duplicate log of the records that process
  produces.
- **A competing documentation standard.**
  [Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md) remains
  the single repository-wide standard, including for the records described
  above. AIOS governance does not define its own.
- The rules themselves - those are [00-CONSTITUTION](../00-CONSTITUTION/README.md)

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
| [docs/18-templates](../../docs/18-templates/README.md) | Existing ADR and RFC forms this section's amendments and AIOS-tagged records reuse, per [04-TEMPLATES](../04-TEMPLATES/README.md) |
| [docs/16-decisions](../../docs/16-decisions/README.md) | Canonical location for AIOS decision records, tagged as AIOS |
| [docs/17-rfcs](../../docs/17-rfcs/README.md) | Canonical location for AIOS RFCs, tagged as AIOS |

Every other AIOS section depends on this one for the meaning of "ratified".

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| Amendment process | Who proposes, who decides, what evidence is required? |
| Version history | What changed between AIOS versions, and why? |

AIOS decision records and RFCs are not future documents of this section: they
are entries in [docs/16-decisions](../../docs/16-decisions/README.md) and
[docs/17-rfcs](../../docs/17-rfcs/README.md), tagged as AIOS. This section
does not accumulate a parallel log; it links to the tagged entries as they
are created.
