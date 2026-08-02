---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Risk Register](../00-company/25-risk-register.md)
  - [Anti-Goals](../00-company/ANTI_GOALS.md)
  - [Assumptions to Validate](../02-research/26-assumptions-to-validate.md)
  - [RFC Template](RFC_TEMPLATE.md)
  - [Product Constitution](../00-company/PRODUCT_CONSTITUTION.md)
Tags: templates, red-team, review, risk
Source: New document. The [Decisions Log](../16-decisions/decisions-log.md) records "Use red-team reviews for major ideas" as Decided; this operationalises that without adding to it.
---

# Red Team Checklist

Run this against any RFC, ADR, or major decision before it is accepted.

The reviewer's job is to make the idea fail on paper. A red team that produces
no findings has not been run properly.

## How to run it

1. The reviewer must **not** be the author.
2. Work through every section. Write "no finding" explicitly rather than skipping.
3. File findings against the source document. Do not resolve them yourself.
4. The author responds to each finding in writing before acceptance.

---

## A. Problem integrity

- [ ] Is the stated problem the real problem, or a symptom of one further up?
- [ ] Who has this problem, specifically? Can we name three?
- [ ] What evidence exists that it is painful enough to pay for?
- [ ] What do people do today instead? Why is that not good enough for them?
- [ ] Would the target user recognise this description of their problem?

## B. Evidence integrity

- [ ] Which claims are asserted with no source?
- [ ] Which "Decided" claims are actually untested beliefs?
- [ ] Is any number presented without a citation?
- [ ] Was disconfirming evidence sought, or only supporting evidence?
- [ ] Is the sample size honest about what it can support?

## C. Assumption stack

- [ ] List every assumption the proposal rests on.
- [ ] Which single assumption, if false, collapses the whole thing?
- [ ] Is that assumption in [Assumptions to Validate](../02-research/26-assumptions-to-validate.md)?
- [ ] How cheaply could we test it before committing?

## D. Constitution and anti-goals

- [ ] Does this violate anything in [Product Constitution](../00-company/PRODUCT_CONSTITUTION.md)?
- [ ] Does it drift toward anything in [Anti-Goals](../00-company/ANTI_GOALS.md)?
- [ ] Does it increase user dependence rather than user capability?
- [ ] Would a user be surprised or unsettled by what the system now knows or does?

## E. Trust, privacy, and data

- [ ] What new data does this require? Is any of it data we said we would not hold?
- [ ] Can the user see, correct, export, and delete it?
- [ ] What is the worst outcome if this data leaked?
- [ ] Is the trust cost of this feature worth its utility?
- [ ] Does this hold up under an enterprise privacy review?

## F. Competitive and durability

- [ ] Which incumbent could ship this within a quarter?
- [ ] What stops them? Is that a real moat or a head start?
- [ ] Does a better foundation model make this feature redundant?
- [ ] Are we competing on model quality despite saying we would not?

## G. Scope and execution

- [ ] Is this the smallest version that tests the idea?
- [ ] What are we saying no to by saying yes to this?
- [ ] What breaks at 10x usage? At 100x?
- [ ] Is this reversible? If not, is it worth being irreversible?

## H. Failure modes

- [ ] What happens when the model is wrong here?
- [ ] What happens when memory is wrong, stale, or misattributed?
- [ ] How does a user notice and recover?
- [ ] What is the failure that loses a user permanently?

## I. The uncomfortable questions

- [ ] If this shipped and nobody used it, what would the most likely reason be?
- [ ] What are we avoiding thinking about?
- [ ] Are we building this because it is right, or because it is interesting?
- [ ] Who would tell us this is a bad idea, and have we asked them?

---

## Findings

| # | Section | Severity | Finding | Author response | Resolved |
|---|---|---|---|---|---|
| 1 | | Blocker / Major / Minor | | | |

## Reviewer verdict

**Recommendation:** Accept | Accept with changes | Revise and re-review | Reject
**Reviewer:**
**Date:**
**Rationale:**
