---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[UX Principles](../03-product/08-ux-principles.md)"
  - "[Product Constitution](PRODUCT_CONSTITUTION.md)"
  - "[Anti-Goals](ANTI_GOALS.md)"
  - "[User Journeys](../03-product/06-user-journeys.md)"
  - "[Trust](../08-trust/README.md)"
Tags: company, design, principles, ux
Source: Assembled from `08-ux-principles.md` (Decided list) plus related Decided statements. No new principles introduced.
---

# Design Principles

> **Assembly notice.** Every principle below is quoted from an existing
> `Decided` statement and cited. Nothing here is new.
> [UX Principles](../03-product/08-ux-principles.md) remains the source of record.

## Constitution versus design principles

| | [Product Constitution](PRODUCT_CONSTITUTION.md) | This document |
|---|---|---|
| Binding? | Non-negotiable once ratified | Strong default |
| Violating it | Blocks the work | Requires a stated reason |
| Changing it | Recorded amendment | Ordinary decision |

If a principle here is one we would never trade away, it should be promoted to
a constitutional article instead.

## Principles

**Status: Decided** — all of the following, per
[UX Principles § Decided](../03-product/08-ux-principles.md).

### P-1 — AI augments rather than replaces

The interface should make the user the actor and the system the assistant.

### P-2 — Trust over novelty

Where a novel interaction and a trustworthy one conflict, choose trustworthy.

### P-3 — Transparency

The user can see what the system is doing.

### P-4 — User control

The user can change or override what the system does.

### P-5 — Minimal cognitive interruption

Assistance should not fragment the user's attention.

### P-6 — Personalization

The experience adapts to the individual user.

### P-7 — Human growth

The design should leave the user more capable over time, not less.

### P-8 — Inspectable memory

What the system remembers is visible to the user.

### P-9 — Explainability

The system can account for why it did what it did.

## Supporting principles from adjacent sources

**Status: Decided**

- **Preserve context.** — [Vision and Thesis](01-vision-and-thesis.md)
- **Avoid creating dependence.** — [Vision and Thesis](01-vision-and-thesis.md)
- **Co-evolve with the user.** — [Vision and Thesis](01-vision-and-thesis.md)

**Status: Proposed** *(recorded as "Reasoned" in the source)*

- Measure human capability, not only AI usage. — [Metrics and KPIs](../14-business/24-metrics-and-kpis.md)

## Tensions between principles

These conflicts are **latent in the sources**; naming them is not resolving
them. Each needs a founder decision, and none has one.

| Tension | Principles in conflict | Where it will surface |
|---|---|---|
| Helpful proactivity vs. minimal interruption | P-5 vs. P-6 | Any suggestion or ambient feature |
| Inspectable memory vs. minimal interruption | P-8 vs. P-5 | Memory confirmation flows — see [User Journeys](../03-product/06-user-journeys.md) |
| Personalization vs. privacy | P-6 vs. C-4 in [Product Constitution](PRODUCT_CONSTITUTION.md) | What gets stored — see [Open Questions](../01-problem-space/open-questions.md) |
| Human growth vs. task efficiency | P-7 vs. the user's immediate goal | Any automation that would be faster done for them |
| Explainability vs. simplicity | P-9 vs. P-5 | Surfacing model reasoning |

## Not yet defined

**Status: Requires founder decision** — per
[UX Principles § Requires founder decision](../03-product/08-ux-principles.md).

- Visual language
- Design system
- Navigation
- Accessibility targets
