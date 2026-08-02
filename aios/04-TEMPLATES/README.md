---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Workflows](../03-WORKFLOWS/README.md)"
  - "[Governance](../05-GOVERNANCE/README.md)"
  - "[docs/18-templates](../../docs/18-templates/README.md)"
Tags: aios, templates, forms, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no template has been written.
---

# 04 — Templates

The blank forms AIOS work is written into.

> **No documents yet.** No template has been written. Sprint 1 created the
> destination only.

## Purpose

A template fixes the shape of a document so that the person writing it decides
substance and nothing else. Following the precedent set by
[Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md), which
states that it "defines form only, it never defines product substance", a
template here defines form only and never defines agent behaviour.

The practical value is comparability: two role documents written a year apart
should answer the same questions in the same order, or they cannot be reviewed
against each other.

## Contents

Currently this README only.

What belongs here:

- Blank forms for the recurring AIOS document types
- Nothing filled in, and no worked examples that could be mistaken for policy

What does not belong here:

- **Product templates.** Those already exist at
  [docs/18-templates](../../docs/18-templates/README.md) — ADR, RFC, decision,
  research, and interview forms, plus the red-team checklist. This section holds
  forms for AIOS documents only, and reuses the product templates where they
  already fit rather than forking them.
- Prompts. A prompt instructs an agent; a template shapes a document. They are
  different things and prompts live in
  [03-WORKFLOWS](../03-WORKFLOWS/README.md).

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

Templates constrain form and carry no authority over substance. A template may
require that a role document state its boundary; it may not state what that
boundary is.

Every template inherits the mandatory frontmatter block and the two status
vocabularies from
[Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md). Where the
two disagree, Document Standards wins.

## Dependencies

| Depends on | Why |
|---|---|
| [Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md) | Frontmatter, status vocabularies, and linking rules every template inherits |
| [docs/18-templates](../../docs/18-templates/README.md) | Existing forms to reuse before writing new ones |
| [01-ROLES](../01-ROLES/README.md), [03-WORKFLOWS](../03-WORKFLOWS/README.md) | A template cannot be shaped before the document type it serves is understood |

Nothing depends on this section being populated. Templates make documents
consistent; their absence does not block writing one.

## Future Documents

**Not created by Sprint 1.**

| Document | Shapes |
|---|---|
| Role template | A single role document |
| Workflow template | A single workflow document |
| Prompt template | A prompt file and its provenance |
| Model assignment template | One role-to-model assignment and its basis |

Whether AIOS needs its own ADR and RFC forms, or reuses
[ADR_TEMPLATE](../../docs/18-templates/ADR_TEMPLATE.md) and
[RFC_TEMPLATE](../../docs/18-templates/RFC_TEMPLATE.md), is unresolved and is a
question for [05-GOVERNANCE](../05-GOVERNANCE/README.md).
