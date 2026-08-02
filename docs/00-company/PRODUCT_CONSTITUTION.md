---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [VISION](VISION.md)
  - [Design Principles](DESIGN_PRINCIPLES.md)
  - [Anti-Goals](ANTI_GOALS.md)
  - [UX Principles](../03-product/08-ux-principles.md)
  - [Red Team Checklist](../18-templates/RED_TEAM_CHECKLIST.md)
Tags: company, constitution, principles, canonical
Source: Scaffold. Candidate articles are drawn verbatim from statements already marked Decided in migrated documents. Ratification is not yet done.
---

# Product Constitution

> **Not yet ratified.**
>
> [Glossary](29-glossary-and-definitions.md) defines a Product Constitution as
> a "set of non-negotiable principles", and the
> [Decisions Log](../16-decisions/decisions-log.md) records
> "Define product constitution before implementation" as **Decided**.
> That definition exists; the ratified document does not.
>
> What follows is a **scaffold**. Every candidate article below is quoted from
> a statement already marked `Decided` elsewhere in this repository and is
> cited. No article here was invented, and none has been ratified as
> non-negotiable. Promoting a candidate to a binding article is a founder
> decision and must be recorded in [16-decisions](../16-decisions/README.md).

## What a constitutional article is

An article is binding, not aspirational. It has three properties:

1. **It can be violated.** If no realistic feature could breach it, it is not an article.
2. **It outranks the roadmap.** A feature that violates it does not ship, regardless of demand.
3. **Amending it is a recorded decision**, never a quiet edit.

A principle that fails these tests belongs in
[Design Principles](DESIGN_PRINCIPLES.md) instead.

## Candidate articles

Each is sourced. **Status: Proposed** for all of them, pending ratification.

### C-1 — Augmentation over replacement

AI should augment rather than replace humans. Automation should remove
repetitive work while strengthening long-term capability.

*Source: [Vision and Thesis § Product Philosophy](01-vision-and-thesis.md) — Decided*

### C-2 — Human capability is a design constraint

Human capability is a core design principle.

*Source: [Decisions Log § Concrete decisions made](../16-decisions/decisions-log.md) — Decided*

### C-3 — Co-evolution

The product co-evolves with the user. The framing is not "AI learns" but
"AI and user co-evolve".

*Source: [Vision and Thesis § Guiding Principle](01-vision-and-thesis.md) and
[Decisions Log § Pivots and reversals](../16-decisions/decisions-log.md) — Decided*

### C-4 — Privacy is a differentiator, not a setting

Privacy should be a product differentiator. Privacy must become a differentiator.

*Source: [Decisions Log](../16-decisions/decisions-log.md) and
[Scalability and Risk § Decided](../04-architecture/14-scalability-and-risk.md) — Decided*

### C-5 — Trust is observable

Trust should be observable and inspectable.

*Source: [Decisions Log § Concrete decisions made](../16-decisions/decisions-log.md) — Decided*

### C-6 — Memory is inspectable and user-controlled

Memory should extend beyond conversations. UX principles record inspectable
memory and user control as Decided; the risk register lists user-controlled
memory as a mitigation.

*Source: [Decisions Log](../16-decisions/decisions-log.md),
[UX Principles § Decided](../03-product/08-ux-principles.md),
[Risk Register § Mitigations Discussed](25-risk-register.md) — Decided*

### C-7 — Transparency and explainability

Transparency. Explainability. Trust over novelty.

*Source: [UX Principles § Decided](../03-product/08-ux-principles.md) — Decided*

### C-8 — Evidence before architecture

Research phase precedes implementation. Build a research canon before
architecture. Maintain decision logs and research evidence.

*Source: [Decisions Log § Concrete decisions made](../16-decisions/decisions-log.md) — Decided*

### C-9 — Adversarial review of major ideas

Use red-team reviews for major ideas.

*Source: [Decisions Log § Concrete decisions made](../16-decisions/decisions-log.md) — Decided;
operationalised by [Red Team Checklist](../18-templates/RED_TEAM_CHECKLIST.md)*

### C-10 — Compete around the model, not on the model

Compete on the experience surrounding foundation models rather than on
foundation models themselves.

*Source: [Positioning § Competitive Philosophy](04-positioning-and-differentiation.md) — Decided*

## Corresponding prohibitions

The negative form of the constitution lives in [Anti-Goals](ANTI_GOALS.md).

## Ratification

**Status: Deferred** — awaiting founder decision.

Open before this document can be ratified:

| Question | Why it blocks ratification |
|---|---|
| Which candidates are genuinely non-negotiable, and which are merely strong preferences? | An article that will be traded away under pressure is not an article. |
| What is the amendment process? | A constitution with no amendment process either freezes or erodes silently. |
| Who ratifies, and who can invoke an article to block work? | Unenforced articles are decoration. |
| How does an article get tested during review? | See [Red Team Checklist § D](../18-templates/RED_TEAM_CHECKLIST.md). |
| Do C-4, C-5, C-6 survive contact with an enterprise deployment model? | [Open Questions](../01-problem-space/open-questions.md) flags enterprise privacy and deployment as undecided. |

Record the outcome using the [Decision Template](../18-templates/DECISION_TEMPLATE.md).
