# Personal Intelligence Layer

Canonical knowledge base for a personal intelligence layer spanning writing,
coding, planning, and knowledge work — a system intended to learn with the
user over time, prioritise trust, privacy, and human capability, and avoid
making users dependent on AI.

**Status: research and planning phase. No implementation exists.**

This repository contains no code and is not a software project. It is the
research canon, decision record, and product thinking behind one.

---

## Start here

| Goal | Go to |
|---|---|
| Understand the project in five minutes | [Executive Summary](docs/00-company/00-executive-summary.md) |
| Understand the direction | [VISION](docs/00-company/VISION.md) |
| See everything | [Documentation Index](docs/README.md) |
| See what is unresolved | [Open Questions](docs/01-problem-space/open-questions.md) |
| See what to write next | [Documentation Roadmap](docs/DOCUMENTATION_ROADMAP.md) |
| Contribute a document | [Document Standards](docs/18-templates/DOCUMENT_STANDARDS.md) |

## Structure

```text
docs/
├── 00-company/          Vision, constitution, design principles, anti-goals, glossary
├── 01-problem-space/    Problems, personas, open questions
├── 02-research/         Research canon, competitive analysis, assumptions
├── 03-product/          Brief, scope, journeys, roadmap, UX principles
├── 04-architecture/     Technical plan, system shape, data model  (conceptual only)
├── 05-ai/               Model strategy                            (empty)
├── 06-memory/           Long-term memory                          (empty)
├── 07-context/          Context engine                            (empty)
├── 08-trust/            Observable trust                          (empty)
├── 09-security/         Threat model                              (empty)
├── 10-privacy/          Data handling, local-first                (empty)
├── 11-learning/         Co-evolution, human growth                (empty)
├── 12-writing/          Writing surface                           (empty)
├── 13-coding/           Coding surface                            (empty)
├── 14-business/         Model, pricing, finance, team, metrics
├── 15-go-to-market/     Market, distribution, launch
├── 16-decisions/        Decision log, DEC and ADR records
├── 17-rfcs/             Proposals open for disagreement
├── 18-templates/        Standards and blank forms
└── 19-graveyard/        Superseded directions (index only, nothing deleted)
```

Empty sections are deliberate destinations. Each has a README pointing at where
that topic is currently discussed elsewhere.

## Conventions

Every document carries frontmatter — status, owner, last updated, related
documents, tags, and source — and is written to be read on its own.

Two status vocabularies are in use, and they mean different things:

- **Document status** — `Stub`, `Draft`, `In Review`, `Ratified`, `Superseded`, `Archived`
- **Claim status** — `Decided`, `Proposed`, `Hypothesis`, `Requires Validation`, `Rejected`, `Deferred`

Documents migrated from the earlier `blueprint/` and `context/` directories
retain their original `Decided` / `Reasoned` / `Requires founder decision`
labels. These were deliberately not rewritten: reclassifying a claim changes
its meaning, and that is a founder decision. The mapping is documented in
[Document Standards § 5](docs/18-templates/DOCUMENT_STANDARDS.md).

## Ground rules

1. Rationale is never deleted. Superseded material is marked and linked, not removed.
2. Every `Decided` claim traces to discussion, research, customer evidence, or an explicit founder decision.
3. Evidence and interpretation never share a heading.
4. No number without a citation.
5. Major proposals are red-teamed before acceptance.

## A caveat worth reading

[Problem Deep Dive](docs/01-problem-space/02-problem-deep-dive.md) records that
customer interviews and structured validation have not been completed, and
[Assumptions to Validate](docs/02-research/26-assumptions-to-validate.md) lists
five load-bearing assumptions, none of them tested.

This is an organised set of beliefs, not a validated plan. It is structured so
that the difference stays visible.
