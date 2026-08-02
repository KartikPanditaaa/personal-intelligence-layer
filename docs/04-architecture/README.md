---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Documentation Index](../README.md)
  - [ADR Template](../18-templates/ADR_TEMPLATE.md)
  - [Glossary](../00-company/29-glossary-and-definitions.md)
  - [Product](../03-product/README.md)
Tags: architecture, index
Source: New document.
---

# 04 — Architecture

System shape. Currently conceptual: [10-system-architecture.md](10-system-architecture.md)
states "Research and planning only", and
[11-tech-stack-rationale.md](11-tech-stack-rationale.md) states that no
implementation stack has been selected.

## Documents

| Document | Covers |
|---|---|
| [technical-plan.md](technical-plan.md) | Decided / Speculative / Not yet defined, cleanly separated |
| [10-system-architecture.md](10-system-architecture.md) | Conceptual component flow |
| [11-tech-stack-rationale.md](11-tech-stack-rationale.md) | No stack chosen; tooling roles |
| [12-data-model.md](12-data-model.md) | Nine candidate entities |
| [13-integration-strategy.md](13-integration-strategy.md) | Potential integration surfaces |
| [14-scalability-and-risk.md](14-scalability-and-risk.md) | Technical risks |

## Start here

[technical-plan.md](technical-plan.md) is the best entry point. It is the only
document in the repository that already separates Decided, Speculative, and
Not-yet-defined into three explicit lists — the pattern
[DOCUMENT_STANDARDS.md](../18-templates/DOCUMENT_STANDARDS.md) generalises.

## Capability sections

The speculative capabilities in [technical-plan.md](technical-plan.md) have
dedicated sections, currently empty:

| Capability | Section |
|---|---|
| Multi-layer memory architecture | [06-memory](../06-memory/README.md) |
| Universal context engine | [07-context](../07-context/README.md) |
| Trust dashboard | [08-trust](../08-trust/README.md) |
| Local-first / hybrid processing | [10-privacy](../10-privacy/README.md) |
| Personal Intelligence Model, Evolution Engine | [05-ai](../05-ai/README.md), [11-learning](../11-learning/README.md) |

## Before any stack decision

Record it as an ADR using [ADR_TEMPLATE.md](../18-templates/ADR_TEMPLATE.md).
[11-tech-stack-rationale.md](11-tech-stack-rationale.md) explicitly rejects
"premature implementation before research", so an ADR that cites no research
should not be accepted.
