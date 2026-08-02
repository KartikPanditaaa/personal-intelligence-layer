---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Governance](../05-GOVERNANCE/README.md)"
  - "[Product Constitution](../../docs/00-company/PRODUCT_CONSTITUTION.md)"
  - "[Glossary](../../docs/00-company/29-glossary-and-definitions.md)"
Tags: aios, constitution, rules, vocabulary, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no constitutional content has been written.
---

# 00 — Constitution

The rules an agent may not break, and the words it must use consistently.

> **No documents yet.** This section is a destination. Sprint 1 created it
> empty on purpose: writing rules before the roles and workflows they govern
> exist would produce rules nobody has tested against real work.

## Purpose

Two things belong here, and they support each other:

- **Rules** — constraints that hold across every role, model, and workflow.
  A rule is binding, not aspirational. It can be violated, it outranks
  convenience, and amending it is a recorded decision rather than a quiet edit.
- **Vocabulary** — the terms AIOS uses, defined once. Where a term already has
  a product meaning in the
  [Glossary](../../docs/00-company/29-glossary-and-definitions.md), the AIOS
  definition cites it rather than competing with it.

This is *not* the Product Constitution. That document lives at
[docs/00-company/PRODUCT_CONSTITUTION.md](../../docs/00-company/PRODUCT_CONSTITUTION.md)
and constrains the product. This one constrains agents.

## Contents

Currently this README only.

What belongs here:

- Constraints that apply regardless of which agent is acting
- Terms whose meaning must not drift between documents or sessions
- The distinction between a binding rule and a default that may be overridden

What does not belong here:

- Anything true of only one role, model, or workflow — those have their own sections
- Product commitments of any kind
- Process for changing these rules — that is [05-GOVERNANCE](../05-GOVERNANCE/README.md)

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

This section is intended to outrank every other AIOS section. A workflow that
contradicts a rule here is expected to be wrong, not the rule.

That precedence takes effect only once rules exist and
[05-GOVERNANCE](../05-GOVERNANCE/README.md) defines ratification. Today the
section is empty, so it constrains nothing.

## Dependencies

| Depends on | Why |
|---|---|
| [Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md) | Form of every file written here |
| [Glossary](../../docs/00-company/29-glossary-and-definitions.md) | Existing product terms the vocabulary must not redefine |
| [05-GOVERNANCE](../05-GOVERNANCE/README.md) | Nothing here becomes binding without a ratification process |

Sections 01–04 depend on this one. It depends on none of them.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| `RULES.md` | What may an agent never do, and what must it always do? |
| `VOCABULARY.md` | What does each AIOS term mean, and where did it come from? |
| Mission | What is AIOS for, stated in one place? |
| Philosophy | What beliefs about agent work do the rules follow from? |

Whether mission and philosophy are separate files or headings inside `RULES.md`
is unresolved and belongs to Sprint 2.
