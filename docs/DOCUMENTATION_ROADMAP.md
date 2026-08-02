---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Documentation Index](README.md)"
  - "[Document Standards](18-templates/DOCUMENT_STANDARDS.md)"
  - "[Open Questions](01-problem-space/open-questions.md)"
  - "[90-Day Execution Plan](00-company/27-90-day-execution-plan.md)"
Tags: meta, roadmap, navigation, backlog
Source: New document. Derived from gaps observed during the documentation migration. Contains no product decisions.
---

# Documentation Roadmap

Which documents should exist, which do not yet, and in what order to write
them.

> **Scope.** This is a roadmap for *documents*, not for the product. Nothing
> here decides what gets built. Where a document is blocked on a product
> decision, that is stated rather than resolved.

## Structural questions raised by the migration

These arose from reorganising, not from product thinking. Each needs a decision
recorded in [16-decisions](16-decisions/README.md).

| # | Question | Why it matters |
|---|---|---|
| S-1 | Should legacy `Reasoned` labels be reclassified as `Proposed` or `Hypothesis`, item by item? | The two mean different things. Bulk-renaming would assert confidence nobody has stated. |
| S-2 | Should `Requires founder decision` fold into `Deferred`, or stay a seventh label? | It marks an unmade decision, not a postponed one. |
| S-3 | Do [16-competitive-analysis.md](02-research/16-competitive-analysis.md) and [competitive-landscape.md](02-research/competitive-landscape.md) merge? | Same 16 competitors, two documents, no canonical version. |
| S-4 | Do [09-pricing-and-packaging.md](14-business/09-pricing-and-packaging.md) and [20-business-model.md](14-business/20-business-model.md) merge? | Both contain the Free / Pro / Team / Enterprise progression. |
| S-5 | Does [DECISION_TEMPLATE.md](18-templates/DECISION_TEMPLATE.md) supersede [28-decision-log-template.md](18-templates/28-decision-log-template.md)? | Two decision templates, one a superset of the other. |
| S-6 | Should the existing [decisions-log.md](16-decisions/decisions-log.md) entries be retrofitted into individual `DEC-` records? | The log has no dates, deciders, or evidence per entry. |
| S-7 | Do [25-risk-register.md](00-company/25-risk-register.md) and [27-90-day-execution-plan.md](00-company/27-90-day-execution-plan.md) belong in `00-company`? | Placed there because the hierarchy has no execution section. |
| S-8 | Should numeric filename prefixes inherited from `blueprint/` be renumbered per section? | They are non-contiguous now. Renumbering costs traceability. |

## Missing documents, by priority

### Tier 1 — blocking almost everything downstream

| Document | Destination | Blocked on |
|---|---|---|
| Memory model | [06-memory](06-memory/README.md) | Nothing. Memory is called foundational in six documents and defined in none. |
| Threat model | [09-security](09-security/README.md) | Nothing. No security material exists anywhere. |
| Data inventory: what is stored, what never is | [10-privacy](10-privacy/README.md) | Partly on the memory model |
| First customer interviews | [02-research](02-research/README.md) | Nothing. Recruiting is the only cost. |
| Beachhead decision | [16-decisions](16-decisions/README.md) | Founder decision |
| Ratify the constitution | [00-company](00-company/PRODUCT_CONSTITUTION.md) | Founder decision |

### Tier 2 — needed before architecture

| Document | Destination | Blocked on |
|---|---|---|
| Context engine, and its boundary with memory | [07-context](07-context/README.md) | Memory model |
| What observable trust means concretely | [08-trust](08-trust/README.md) | Nothing |
| How trust is measured | [08-trust](08-trust/README.md) / [14-business](14-business/README.md) | Trust definition |
| How growth is measured | [11-learning](11-learning/README.md) | Nothing |
| Model strategy and evaluation | [05-ai](05-ai/README.md) | Nothing |
| Research notes backing the five key assumptions | [02-research](02-research/README.md) | Nothing |
| Enterprise deployment and privacy model | [10-privacy](10-privacy/README.md) | Founder decision |

### Tier 3 — needed before building

| Document | Destination | Blocked on |
|---|---|---|
| MVP feature list | [03-product](03-product/README.md) | Beachhead decision |
| First-platform ADR | [16-decisions](16-decisions/README.md) | MVP scope |
| Stack ADRs | [16-decisions](16-decisions/README.md) | Research canon |
| Writing surface definition | [12-writing](12-writing/README.md) | MVP scope |
| Coding surface definition | [13-coding](13-coding/README.md) | MVP scope |
| Market sizing with cited sources | [15-go-to-market](15-go-to-market/README.md) | Beachhead decision |
| Founder narrative | [00-company](00-company/VISION.md) | Founder decision |

## Dependency shape

```text
Customer interviews ─┬─► Validated problem ──► Beachhead decision ──► MVP scope
                     │                                                   │
                     └─► Assumption tests                                ├─► Writing surface
                                                                         ├─► Coding surface
Memory model ─┬─► Context engine ──► System architecture ──► Stack ADRs  └─► First platform
              ├─► Data inventory ──► Enterprise privacy model
              └─► Trust definition ──► Trust measurement

Threat model ──► Security posture ──► Enterprise readiness
```

Two chains run in parallel and only meet at architecture. The interview chain
is currently unstarted; the memory chain is blocked on nothing at all.

## Standing hygiene

- Every new document uses [DOCUMENT_STANDARDS](18-templates/DOCUMENT_STANDARDS.md).
- Every new claim carries a status label and a source.
- Every new document is linked from its section README.
- Answered items in [Open Questions](01-problem-space/open-questions.md) move
  to a decision record; the question is struck through, not deleted.
- Check links after moving any file.
