---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Documentation Index](../README.md)"
  - "[RFC Template](../18-templates/RFC_TEMPLATE.md)"
  - "[Red Team Checklist](../18-templates/RED_TEAM_CHECKLIST.md)"
  - "[Decisions Index](../16-decisions/README.md)"
Tags: rfcs, index, process
Source: New document. Absorbs the empty top-level `reviews/` directory.
---

# 17 — RFCs

Proposals open for disagreement, before anything is decided.

## Current RFCs

One RFC open for comment.

| ID | Title | Status | Outcome |
|---|---|---|---|
| [RFC-0001](RFC-0001-personal-context-engine.md) | Personal Context Engine | In Review | Open |

## What an RFC is for

An RFC exists to be argued with. It is written when a proposal is substantial
enough that being wrong about it would be expensive, and when the author wants
objections before commitment rather than after.

An RFC is **not** a decision record. When one is accepted it produces a record
in [16-decisions](../16-decisions/README.md), and the RFC is marked with the
outcome and linked to that record.

## Lifecycle

```text
Draft ──► Open for comment ──► Red team ──► Outcome
                                              ├── Accepted  ──► DEC- or ADR- record
                                              ├── Rejected  ──► retained, rationale kept
                                              ├── Withdrawn ──► retained
                                              └── Deferred  ──► retained, unblocking condition stated
```

Rejected and withdrawn RFCs stay in this directory. They are part of the
record: the argument that was made and lost is often more useful later than
the one that won.

## Conventions

- Filename: `RFC-NNNN-short-slug.md`
- Numbers sequential, never reused
- Template: [RFC_TEMPLATE.md](../18-templates/RFC_TEMPLATE.md)
- Every RFC is red-teamed with [RED_TEAM_CHECKLIST.md](../18-templates/RED_TEAM_CHECKLIST.md) before its outcome is set

## Review obligation

[decisions-log.md](../16-decisions/decisions-log.md) records "Use red-team
reviews for major ideas" as **Decided**. An RFC accepted without a recorded red
team has not followed process.

## Note on the former `reviews/` directory

The empty top-level `reviews/` directory has been absorbed into this section,
since review output attaches to the RFC or decision being reviewed rather than
living separately.
