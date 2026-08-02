---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[ADR Template](ADR_TEMPLATE.md)"
  - "[Legacy Decision Log Template](28-decision-log-template.md)"
  - "[Decisions Index](../16-decisions/README.md)"
  - "[Document Standards](DOCUMENT_STANDARDS.md)"
Tags: templates, decisions, governance
Source: New document. Extends the fields already present in the legacy `28-decision-log-template.md`, which is retained unchanged.
---

# Decision Template

Copy to `docs/16-decisions/DEC-NNNN-short-slug.md` for product, positioning,
market, pricing, or process decisions. For system-shape decisions use the
[ADR Template](ADR_TEMPLATE.md).

This template is a superset of the original
[legacy decision log template](28-decision-log-template.md), which is preserved
as written.

---

```markdown
---
Status: Draft
Owner:
Last Updated: YYYY-MM-DD
Related Documents:
Tags: decision
Source:
---

# DEC-NNNN: <Decision in one line>

**Decision ID:**
**Date:**
**Topic:**
**Claim status:** Decided | Proposed | Rejected | Deferred | Superseded
**Decider:**
**Review date:**

## Context

What prompted this. What was unresolved before.

## Options Considered

| Option | Summary | Why not chosen |
|---|---|---|
| A | | |
| B | | |
| Do nothing | | |

## Decision

## Evidence

Cite each. Mark anything asserted without evidence as an assumption.

| Type | Reference | Strength |
|---|---|---|
| Discussion | | |
| Research | | |
| Customer evidence | | |
| Founder judgement | | |

## Trade-offs

What we knowingly gave up.

## Assumptions This Rests On

Link each to [Assumptions to Validate](../02-research/26-assumptions-to-validate.md).

## Reversal Conditions

What evidence would make us revisit this.

## Future Review Date
```
