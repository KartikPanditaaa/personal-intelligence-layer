---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Documentation Index](../README.md)
  - [Decisions Log](../16-decisions/decisions-log.md)
  - [Anti-Goals](../00-company/ANTI_GOALS.md)
  - [Positioning and Differentiation](../00-company/04-positioning-and-differentiation.md)
Tags: graveyard, superseded, rejected, index
Source: New document. Indexes superseded directions already recorded in `decisions-log.md` and `04-positioning-and-differentiation.md`. Nothing has been moved here or deleted.
---

# 19 — Graveyard

Directions that were considered and set aside.

> **Nothing has been deleted, and no document has been moved into this
> directory.** This is an index. Every superseded direction below is still
> recorded, in full, in its original document. This section exists so that a
> reader can find what was abandoned and why, without that history being
> mistaken for current direction.

## Why this section exists

A superseded idea is evidence. It tells a future reader which paths were
already walked, and stops the same ground being re-covered as though it were
new. It also guards against silent reversal: if a proposal starts drifting back
toward something on this list, that should be a deliberate, argued reversal
rather than an accident.

## Superseded product directions

Recorded under "Pivots and reversals" in
[decisions-log.md](../16-decisions/decisions-log.md).

| Direction | Superseded by | Source |
|---|---|---|
| AI coding IDE (initial focus) | Writing assistant, then Personal Intelligence Layer | [decisions-log.md](../16-decisions/decisions-log.md) |
| Writing assistant | Personal Intelligence Layer | [decisions-log.md](../16-decisions/decisions-log.md) |
| "Modes" | Contextual workspaces / dynamic expertise | [decisions-log.md](../16-decisions/decisions-log.md) |
| "AI learns" framing | "AI and user co-evolve" | [decisions-log.md](../16-decisions/decisions-log.md) |

The category progression is also recorded as an explicit sequence in
[04-positioning-and-differentiation.md](../00-company/04-positioning-and-differentiation.md):
AI Coding IDE → AI Writing Assistant → Personal Intelligence Layer.

## Rejected positioning

Recorded under "Explicitly Rejected Positioning" in
[04-positioning-and-differentiation.md](../00-company/04-positioning-and-differentiation.md)
and carried into [Anti-Goals](../00-company/ANTI_GOALS.md).

| Rejected | Status |
|---|---|
| Another autocomplete | Rejected |
| Another AI IDE | Rejected |
| Another chat wrapper | Rejected |

## Rejected process

Recorded in
[11-tech-stack-rationale.md](../04-architecture/11-tech-stack-rationale.md).

| Rejected | Status |
|---|---|
| Premature implementation before research | Rejected |

## Missing rationale

The sources record **what** changed but not, in most cases, **why**, when it
happened, or what evidence prompted it. That rationale is not recoverable from
the documents alone.

Reconstructing it is worth doing while it is still remembered, and is tracked
in the [Documentation Roadmap](../DOCUMENTATION_ROADMAP.md). Per
[DOCUMENT_STANDARDS.md § 6](../18-templates/DOCUMENT_STANDARDS.md), rationale
is never removed — but rationale that was never written down cannot be
preserved, only reconstructed.

## Adding to this section

When a direction is abandoned:

1. Mark the original document `Superseded` in frontmatter and link forward to
   its replacement. **Do not delete it.**
2. Record the reversal in [16-decisions](../16-decisions/README.md) with the
   reasoning that prompted it.
3. Add a row to this index.
4. If it should never be revisited, add it to
   [Anti-Goals](../00-company/ANTI_GOALS.md) as well.
