---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Research Template](RESEARCH_TEMPLATE.md)
  - [Assumptions to Validate](../02-research/26-assumptions-to-validate.md)
  - [Target User Personas](../01-problem-space/03-target-user-personas.md)
  - [Problem Deep Dive](../01-problem-space/02-problem-deep-dive.md)
Tags: templates, research, interviews, validation
Source: New document.
---

# Customer Interview Template

Copy to `docs/02-research/interviews/INT-NNNN-<persona>-<date>.md`.

[Problem Deep Dive](../01-problem-space/02-problem-deep-dive.md) records that
structured validation has not yet been completed. This template exists so that
when it starts, every interview is comparable to every other.

## Interviewing rules

- Ask about **past behaviour**, never about future intent. "When did you last…" not "Would you…".
- Never describe the product before the problem section is finished.
- Record what they *did*, and separately what they *said*. They differ.
- A compliment is not evidence. A workaround they already built is.

---

```markdown
---
Status: Draft
Owner:
Last Updated: YYYY-MM-DD
Related Documents:
Tags: interview, research
Source: Interview conducted YYYY-MM-DD
---

# INT-NNNN: <Persona> — <Date>

## Participant

| Field | Value |
|---|---|
| Segment / persona | |
| Role | |
| Org size | |
| Current AI tools used | |
| Recruited via | |
| Consent to record | Yes / No |
| Compensated | Yes / No |

## Assumptions Under Test

List the specific entries from
[Assumptions to Validate](../02-research/26-assumptions-to-validate.md)
this interview is meant to probe. If none, say why the interview is exploratory.

## Section 1 — Current workflow (no product mention)

- Walk me through the last time you used an AI tool for real work.
- What happened immediately before and after?
- What did you have to re-explain?

## Section 2 — Pain and workarounds

- What is the most annoying part of that?
- What have you built or hacked together to cope?
- How often does this happen? When did it last happen?
- What does it cost you when it does?

## Section 3 — Trust, privacy, memory

Probe only what they raise unprompted first. Then ask directly.

- What would you never paste into an AI tool? Why?
- Has a tool ever remembered something you wished it had not?
- How would you want to see what it knows about you?

## Section 4 — Alternatives

- What else have you tried? Why did you stop?
- If this problem vanished tomorrow, what would change for you?

## Section 5 — Reaction (only if applicable)

Describe the concept last. Record first reaction verbatim.

## Verbatim Quotes

> Quote, with timestamp.

## Observed Behaviours

Things they did or showed, distinct from things they said.

## Findings

| # | Finding | Supports / Contradicts | Assumption | Confidence |
|---|---|---|---|---|
| 1 | | Supports / Contradicts | | High / Med / Low |

## Disconfirming Evidence

What in this interview argues *against* the current direction.
Leaving this blank is a warning sign, not a good result.

## Follow-up Actions
```
