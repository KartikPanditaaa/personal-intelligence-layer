---
Status: Stub
Owner: Founder
Last Updated: 2026-08-11
Related Documents:
  - "[Repository README](../README.md)"
  - "[Documentation Index](../docs/README.md)"
  - "[Document Standards](../docs/18-templates/DOCUMENT_STANDARDS.md)"
  - "[Documentation Roadmap](../docs/DOCUMENTATION_ROADMAP.md)"
Tags: aios, index, navigation, stub
Source: AIOS v0.1.0 Sprint 1, amended per the Sprint 1 governance resolution draft (proposed, founder approval pending). No AIOS content has been written.
---

# AIOS

The operating layer that governs how AI agents work: what they may assume,
what roles they take, which models they run on, which workflows they follow,
and who decides when any of that changes.

This repository is where AIOS is currently documented and instantiated.
Whether AIOS is scoped to this repository or to the company as a whole is an
open founder decision, not something this README settles by asserting either
scope.

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
| `aios/` | How is AI agent work governed? |

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
├── 02-MODELS/           Per-vendor model operating notes and adapters
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
| 03 | [Workflows](03-WORKFLOWS/README.md) | - |
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

- [Document Standards](../docs/18-templates/DOCUMENT_STANDARDS.md) - every file
  here follows it: mandatory frontmatter, the status vocabularies, relative
  links, no uncited numbers. AIOS does not define a competing standard.
- [Documentation Index](../docs/README.md) - the product canon AIOS operates on.
- No AIOS section depends on another section's *contents* yet, because no
  contents exist. The precedence order above is the only coupling.

## Future Documents

Named here so the shape is visible. **None of these exist, and Sprint 1 does
not create them.**

| Section | Expected documents |
|---|---|
| 00-CONSTITUTION | `RULES.md`, `VOCABULARY.md`, `AGENTS.md`, mission and philosophy statements |
| 01-ROLES | One document per role |
| 02-MODELS | One operating-notes file per vendor (`claude.md`, `codex.md`, `gemini.md`, `chatgpt.md`) |
| 03-WORKFLOWS | Workflow definitions, prompt files |
| 04-TEMPLATES | Blank forms for AIOS documents |
| 05-GOVERNANCE | Amendment process, version history |

Each section README states its own list in full.

## Version

AIOS v0.1.0. Sprint 1 delivered directory structure and navigation. No
behavioural content has been authored, reviewed, or ratified.

Proposed version identity: a git tag as the immutable release marker, plus a
human-readable `aios/VERSION` file for navigation. Neither exists yet. The
tag format is not decided, so this Sprint does not create `aios/VERSION` -
doing so before the format is approved would fix a decision that has not
been made.
