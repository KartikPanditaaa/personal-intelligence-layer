---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [RFC Index](../17-rfcs/README.md)
  - [ADR Template](ADR_TEMPLATE.md)
  - [Red Team Checklist](RED_TEAM_CHECKLIST.md)
  - [Document Standards](DOCUMENT_STANDARDS.md)
Tags: templates, rfc, process
Source: New document.
---

# RFC Template

Copy to `docs/17-rfcs/RFC-NNNN-short-slug.md`.

An RFC proposes something substantial and invites disagreement **before** a
decision is made. An RFC is not a decision record. When an RFC is accepted, it
produces an ADR or a Decision record, and the RFC is marked accordingly.

---

```markdown
---
Status: Draft
Owner:
Last Updated: YYYY-MM-DD
Related Documents:
Tags: rfc
Source:
---

# RFC-NNNN: <Title>

**Claim status:** Proposed
**Author:**
**Created:**
**Discussion window closes:**
**Outcome:** Open | Accepted | Rejected | Withdrawn | Deferred
**Resulting record:** *(link to ADR or Decision once resolved)*

## Summary

Three sentences. What is being proposed, for whom, and why now.

## Motivation

The problem. Link to `01-problem-space/` and `02-research/`. If there is no
evidence, say so explicitly rather than implying there is.

## Guide-Level Explanation

Explain the proposal as if to a new team member. Use examples. Avoid internals.

## Reference-Level Explanation

The detail. Data shapes, boundaries, flows, failure behaviour.

## Drawbacks

Why we might not want to do this.

## Rationale and Alternatives

- Why this design over the others
- What alternatives were considered and set aside
- What is the impact of not doing this

## Prior Art

What comparable products or literature do here, and what they got wrong.
Link to `02-research/`.

## Unresolved Questions

Explicitly out of scope for this RFC but in scope for the decision it triggers.

## Future Possibilities

Things this makes possible later. Clearly marked as **not** part of the proposal.

## Red Team

Findings from the [Red Team Checklist](../18-templates/RED_TEAM_CHECKLIST.md).
```
