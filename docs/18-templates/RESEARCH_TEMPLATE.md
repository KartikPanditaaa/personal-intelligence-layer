---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Research Index](../02-research/README.md)
  - [Customer Interview Template](CUSTOMER_INTERVIEW_TEMPLATE.md)
  - [Assumptions to Validate](../02-research/26-assumptions-to-validate.md)
  - [Document Standards](DOCUMENT_STANDARDS.md)
Tags: templates, research, evidence
Source: New document. Supports the "research canon" recorded as Decided in the [Decisions Log](../16-decisions/decisions-log.md).
---

# Research Template

Copy to `docs/02-research/RES-NNNN-short-slug.md`.

The [Decisions Log](../16-decisions/decisions-log.md) records
"Build a research canon before architecture" as **Decided**. This template is
the unit of that canon.

The single rule: **evidence and interpretation never share a heading.**

---

```markdown
---
Status: Draft
Owner:
Last Updated: YYYY-MM-DD
Related Documents:
Tags: research
Source:
---

# RES-NNNN: <Question being researched>

**Claim status of conclusions:** Hypothesis | Requires Validation | Proposed
**Researcher:**
**Date range:**
**Time invested:**

## Research Question

One sentence, answerable, falsifiable.

## Why This Question Now

What decision is blocked on the answer. Link it.

## Method

- Sources searched, and how
- Inclusion and exclusion criteria
- What this method cannot tell us

## Sources

| # | Source | Type | Date | Quality |
|---|---|---|---|---|
| 1 | | Paper / Product / Post / Data | | Primary / Secondary / Anecdote |

Quality is not optional. A blog post and a longitudinal study are not the same evidence.

## Evidence

Findings only. No interpretation. Each line cites a source number.

| # | Finding | Source | Strength |
|---|---|---|---|
| 1 | | [1] | Strong / Moderate / Weak |

## Contradicting Evidence

Sources that disagree. If empty, state that you looked and found none.

## Interpretation

What you think the evidence means. Clearly separated from the evidence itself.

## Confidence

**Level:** High | Medium | Low
**Why:**
**What would raise it:**

## Implications

| Implication | Affects | Claim status |
|---|---|---|
| | Link to document | Hypothesis / Proposed |

## Open Questions Generated

Add these to [Open Questions](../01-problem-space/open-questions.md).
```
