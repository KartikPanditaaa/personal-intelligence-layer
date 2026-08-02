---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Decision Template](DECISION_TEMPLATE.md)"
  - "[RFC Template](RFC_TEMPLATE.md)"
  - "[Document Standards](DOCUMENT_STANDARDS.md)"
  - "[Architecture Index](../04-architecture/README.md)"
Tags: templates, adr, architecture, decisions
Source: New document.
---

# ADR Template

Copy to `docs/16-decisions/ADR-NNNN-short-slug.md`. Number sequentially. Never renumber.

Use an ADR for a decision that constrains the **system**: storage, boundaries,
protocols, runtime, data flow. For product or company decisions use the
[Decision Template](DECISION_TEMPLATE.md).

---

```markdown
---
Status: Draft
Owner:
Last Updated: YYYY-MM-DD
Related Documents:
Tags: adr, architecture
Source:
---

# ADR-NNNN: <Title in the imperative>

**Claim status:** Proposed | Decided | Rejected | Deferred | Superseded
**Date:**
**Deciders:**
**Supersedes:**
**Superseded by:**

## Context

What forces are at play? What is true today that makes this decision necessary
now? State constraints as facts, with links. Do not argue for an option here.

## Decision Drivers

- Driver, and why it matters
- Constraint that narrows the field

## Options Considered

### Option A — <name>

Description.

- **Pros:**
- **Cons:**
- **Cost / effort:**
- **Reversibility:** One-way | Reversible with effort | Cheap to reverse

### Option B — <name>

*(repeat)*

### Option C — Do nothing

Always include this. What happens if we defer?

## Decision

We chose **<option>**.

## Rationale

Why this option beat the others. Reference the drivers by name.

## Trade-offs Accepted

State plainly what gets worse. An ADR with no accepted downside is incomplete.

## Consequences

- **Immediate:**
- **Downstream:**
- **What this forecloses:**

## Validation

How we will know this was right or wrong, and by when.

## Traceability

- Discussion:
- Research:
- Customer evidence:
- Founder decision:
```
