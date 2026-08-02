---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Documentation Index](../README.md)
  - [Document Standards](DOCUMENT_STANDARDS.md)
  - [Decisions Index](../16-decisions/README.md)
  - [RFC Index](../17-rfcs/README.md)
Tags: templates, index, process
Source: New document.
---

# 18 — Templates

Blank forms and the standards that govern them. Nothing here contains product
substance; copy a template out before filling it in.

## Standards

| Document | Purpose |
|---|---|
| [DOCUMENT_STANDARDS.md](DOCUMENT_STANDARDS.md) | Frontmatter, status vocabularies, traceability, linking, writing rules. **Read this first.** |

## Templates

| Template | Use it for | Output location |
|---|---|---|
| [ADR_TEMPLATE.md](ADR_TEMPLATE.md) | Decisions that constrain the system | `16-decisions/ADR-NNNN-*.md` |
| [DECISION_TEMPLATE.md](DECISION_TEMPLATE.md) | Product, market, pricing, process decisions | `16-decisions/DEC-NNNN-*.md` |
| [RFC_TEMPLATE.md](RFC_TEMPLATE.md) | Proposals open for disagreement before deciding | `17-rfcs/RFC-NNNN-*.md` |
| [RESEARCH_TEMPLATE.md](RESEARCH_TEMPLATE.md) | A unit of the research canon | `02-research/RES-NNNN-*.md` |
| [CUSTOMER_INTERVIEW_TEMPLATE.md](CUSTOMER_INTERVIEW_TEMPLATE.md) | A single customer interview | `02-research/interviews/INT-NNNN-*.md` |
| [RED_TEAM_CHECKLIST.md](RED_TEAM_CHECKLIST.md) | Adversarial review of any major idea | Attached to the reviewed document |

## Retained originals

| Document | Note |
|---|---|
| [28-decision-log-template.md](28-decision-log-template.md) | The original decision log template from `blueprint/06-risk-execution/`. Preserved unchanged. [DECISION_TEMPLATE.md](DECISION_TEMPLATE.md) is a superset of it. Which becomes canonical is an open question. |

## Which template do I want?

```text
Is it already decided?
├── No, and I want disagreement first ──────────► RFC_TEMPLATE
├── No, I am gathering evidence ────────────────► RESEARCH_TEMPLATE
│                                                 CUSTOMER_INTERVIEW_TEMPLATE
└── Yes
    ├── It constrains the system's shape ───────► ADR_TEMPLATE
    └── It constrains product / market / process ► DECISION_TEMPLATE

Before accepting any of the above ───────────────► RED_TEAM_CHECKLIST
```
