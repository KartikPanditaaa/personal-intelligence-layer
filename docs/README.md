---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Repository README](../README.md)
  - [Document Standards](18-templates/DOCUMENT_STANDARDS.md)
  - [Documentation Roadmap](DOCUMENTATION_ROADMAP.md)
  - [VISION](00-company/VISION.md)
Tags: index, navigation, meta
Source: New document.
---

# Documentation Index

The knowledge base for the Personal Intelligence Layer. Research and planning
only — no implementation exists.

## Start here

| If you are… | Read |
|---|---|
| New to the project | [Executive Summary](00-company/00-executive-summary.md), then [VISION](00-company/VISION.md) |
| Looking for what is settled | [VISION](00-company/VISION.md), [ANTI_GOALS](00-company/ANTI_GOALS.md), [Decisions Log](16-decisions/decisions-log.md) |
| Looking for what is open | [Open Questions](01-problem-space/open-questions.md), [Assumptions to Validate](02-research/26-assumptions-to-validate.md) |
| About to write a document | [DOCUMENT_STANDARDS](18-templates/DOCUMENT_STANDARDS.md) |
| About to make a decision | [DECISION_TEMPLATE](18-templates/DECISION_TEMPLATE.md) or [ADR_TEMPLATE](18-templates/ADR_TEMPLATE.md) |
| About to propose something big | [RFC_TEMPLATE](18-templates/RFC_TEMPLATE.md), then [RED_TEAM_CHECKLIST](18-templates/RED_TEAM_CHECKLIST.md) |
| Wondering what to write next | [DOCUMENTATION_ROADMAP](DOCUMENTATION_ROADMAP.md) |

## Sections

| # | Section | Docs | State |
|---|---|---|---|
| 00 | [Company](00-company/README.md) | 10 | Populated |
| 01 | [Problem Space](01-problem-space/README.md) | 3 | Populated |
| 02 | [Research](02-research/README.md) | 3 | Thin — no research notes or interviews yet |
| 03 | [Product](03-product/README.md) | 5 | Populated |
| 04 | [Architecture](04-architecture/README.md) | 6 | Populated, conceptual only |
| 05 | [AI](05-ai/README.md) | 0 | Empty |
| 06 | [Memory](06-memory/README.md) | 0 | Empty — largest gap |
| 07 | [Context](07-context/README.md) | 0 | Empty |
| 08 | [Trust](08-trust/README.md) | 0 | Empty |
| 09 | [Security](09-security/README.md) | 0 | Empty — no source material at all |
| 10 | [Privacy](10-privacy/README.md) | 0 | Empty |
| 11 | [Learning](11-learning/README.md) | 0 | Empty |
| 12 | [Writing](12-writing/README.md) | 0 | Empty |
| 13 | [Coding](13-coding/README.md) | 0 | Empty |
| 14 | [Business](14-business/README.md) | 6 | Populated, mostly undecided |
| 15 | [Go-To-Market](15-go-to-market/README.md) | 4 | Populated, blocked on beachhead |
| 16 | [Decisions](16-decisions/README.md) | 1 | Log only, no individual records |
| 17 | [RFCs](17-rfcs/README.md) | 0 | Empty |
| 18 | [Templates](18-templates/README.md) | 8 | Complete |
| 19 | [Graveyard](19-graveyard/README.md) | Index | Index only, nothing moved |

Sections 05–13 are topic destinations with no documents. Each README points at
where that topic is currently discussed elsewhere, so nothing is lost by the
section being empty.

## Canonical documents

| Document | Question it answers |
|---|---|
| [VISION](00-company/VISION.md) | Where is this going? |
| [PRODUCT_CONSTITUTION](00-company/PRODUCT_CONSTITUTION.md) | What will we never trade away? *(not ratified)* |
| [DESIGN_PRINCIPLES](00-company/DESIGN_PRINCIPLES.md) | How do we decide product questions? |
| [ANTI_GOALS](00-company/ANTI_GOALS.md) | What have we said no to? |
| [DOCUMENT_STANDARDS](18-templates/DOCUMENT_STANDARDS.md) | How do we write things down? |

The first four are **assemblies**: they restate sourced statements with
citations and introduce no new commitments.

## How to read a status label

Two vocabularies are in use, deliberately.

- **Frontmatter `Status`** describes the document: `Stub`, `Draft`, `In Review`, `Ratified`, `Superseded`, `Archived`.
- **Inline labels** describe a claim: `Decided`, `Proposed`, `Hypothesis`, `Requires Validation`, `Rejected`, `Deferred`.

Documents migrated from `blueprint/` and `context/` still use the older
`Decided` / `Reasoned` / `Requires founder decision` labels. Those were left
exactly as written, because reclassifying a claim changes its meaning. The
mapping is in [DOCUMENT_STANDARDS § 5](18-templates/DOCUMENT_STANDARDS.md).

## The honest summary

Almost nothing here is validated. [Problem Deep Dive](01-problem-space/02-problem-deep-dive.md)
states that customer interviews and structured validation have not been
completed, and [Assumptions to Validate](02-research/26-assumptions-to-validate.md)
lists five load-bearing assumptions, none tested.

This repository is a well-organised set of beliefs. Read it as such.
