---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Documentation Index](../README.md)
  - [Decisions Log](decisions-log.md)
  - [Decision Template](../18-templates/DECISION_TEMPLATE.md)
  - [ADR Template](../18-templates/ADR_TEMPLATE.md)
  - [RFC Index](../17-rfcs/README.md)
Tags: decisions, index, governance
Source: New document. Replaces the empty top-level `decisions/` directory.
---

# 16 — Decisions

The decision record. [decisions-log.md](../16-decisions/decisions-log.md)
records "Maintain decision logs and research evidence" as **Decided**; this
section is where that obligation is met.

## Documents

| Document | Covers |
|---|---|
| [decisions-log.md](decisions-log.md) | The running log: concrete decisions, positioning discussions, pricing direction, stack, pivots and reversals |

No individual `DEC-` or `ADR-` records exist yet. The log is the only record.

## Record types

| Type | Filename | Template | For |
|---|---|---|---|
| Decision | `DEC-NNNN-slug.md` | [DECISION_TEMPLATE.md](../18-templates/DECISION_TEMPLATE.md) | Product, market, pricing, process |
| Architecture Decision | `ADR-NNNN-slug.md` | [ADR_TEMPLATE.md](../18-templates/ADR_TEMPLATE.md) | Decisions constraining the system |

Numbers are sequential per type and never reused. A superseded record is
retained, marked `Superseded`, and linked forward to its replacement.

## Traceability requirement

Every decision must trace to discussion, research, customer evidence, or an
explicit founder decision. See
[DOCUMENT_STANDARDS.md § 6](../18-templates/DOCUMENT_STANDARDS.md).

**Rationale is never deleted.** A reversed decision keeps its original
reasoning, because the reasoning is what tells a future reader whether the
reversal was correct.

## Reversals already on record

[decisions-log.md](decisions-log.md) documents five direction changes under
"Pivots and reversals". They are preserved as written and indexed in
[19-graveyard](../19-graveyard/README.md). No superseded direction has been
deleted from this repository.

## Relationship to RFCs

An [RFC](../17-rfcs/README.md) precedes a decision and invites disagreement.
When an RFC is accepted it produces a record here, and the RFC links to it.

## Backlog

[decisions-log.md](decisions-log.md) has no per-decision dates, deciders,
evidence, or trade-offs, because it was written as a summary rather than as a
set of records. Whether to retrofit the existing entries into individual `DEC-`
records is an open question tracked in the
[Documentation Roadmap](../DOCUMENTATION_ROADMAP.md).
