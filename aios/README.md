---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Repository README](../README.md)"
  - "[Documentation Index](../docs/README.md)"
  - "[Document Standards](../docs/18-templates/DOCUMENT_STANDARDS.md)"
  - "[Documentation Roadmap](../docs/DOCUMENTATION_ROADMAP.md)"
Tags: aios, index, navigation, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no AIOS content has been written.
---

# AIOS

The operating layer that governs how AI agents work inside this repository:
what they may assume, what roles they take, which models they run on, which
workflows they follow, and who decides when any of that changes.

> **This directory contains no AIOS documents.** Sprint 1 created the
> structure and nothing else. Every section below is a destination with a
> README and no contents. Nothing here has been ratified, and no claim in this
> directory outranks anything in [`docs/`](../docs/README.md) yet.

## Purpose

`docs/` records what the product is and why. AIOS records how work on it gets
done when an agent is doing that work. The two answer different questions and
are kept apart deliberately:

| Directory | Question it answers |
|---|---|
| [`docs/`](../docs/README.md) | What are we building, and on what evidence? |
| `aios/` | How does an agent operate on this repository? |

Separating them keeps operating rules from being mistaken for product
decisions. An agent instruction that leaks into `docs/` reads as a commitment
about the product; a product commitment that leaks into `aios/` becomes an
unreviewed constraint on every future session.

## Contents

```text
aios/
├── README.md            This file
├── 00-CONSTITUTION/     Non-negotiable rules and shared vocabulary
├── 01-ROLES/            Who the agents are and what each is accountable for
├── 02-MODELS/           Which models back which roles, and on what basis
├── 03-WORKFLOWS/        The sequences agents follow, and the prompts they use
├── 04-TEMPLATES/        Blank forms AIOS work is written into
└── 05-GOVERNANCE/       How AIOS itself is changed
```

Numbering is a precedence order, not a reading order. Lower numbers constrain
higher ones.

| # | Section | Constrains |
|---|---|---|
| 00 | [Constitution](00-CONSTITUTION/README.md) | Everything below it |
| 01 | [Roles](01-ROLES/README.md) | 02, 03 |
| 02 | [Models](02-MODELS/README.md) | 03 |
| 03 | [Workflows](03-WORKFLOWS/README.md) | — |
| 04 | [Templates](04-TEMPLATES/README.md) | Form only, never substance |
| 05 | [Governance](05-GOVERNANCE/README.md) | Changes to 00–04 |

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

1. AIOS governs agent behaviour. It does not govern the product.
2. Where AIOS and `docs/` appear to conflict about the product, `docs/` wins,
   and the conflict is a defect in AIOS.
3. Nothing in `aios/` is binding until [00-CONSTITUTION](00-CONSTITUTION/README.md)
   exists and [05-GOVERNANCE](05-GOVERNANCE/README.md) defines what ratifying it
   means.
4. Until then this directory is descriptive: it says where things will go, not
   what anyone must do.

## Dependencies

- [Document Standards](../docs/18-templates/DOCUMENT_STANDARDS.md) — every file
  here follows it: mandatory frontmatter, the status vocabularies, relative
  links, no uncited numbers.
- [Documentation Index](../docs/README.md) — the product canon AIOS operates on.
- No AIOS section depends on another section's *contents* yet, because no
  contents exist. The precedence order above is the only coupling.

## Future Documents

Named here so the shape is visible. **None of these exist, and Sprint 1 does
not create them.**

| Section | Expected documents |
|---|---|
| 00-CONSTITUTION | `RULES.md`, `VOCABULARY.md`, mission and philosophy statements |
| 01-ROLES | `AGENTS.md`, one document per role |
| 02-MODELS | Model selection criteria, routing and fallback policy |
| 03-WORKFLOWS | Workflow definitions, prompt files |
| 04-TEMPLATES | Blank forms for AIOS documents |
| 05-GOVERNANCE | Amendment process, AIOS RFCs and ADRs, version history |

Each section README states its own list in full.

## Version

AIOS v0.1.0. Sprint 1 delivered directory structure and navigation. No
behavioural content has been authored, reviewed, or ratified.
