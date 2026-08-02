---
Status: Stub
Owner: Founder
Last Updated: 2026-08-11
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Roles](../01-ROLES/README.md)"
  - "[Governance](../05-GOVERNANCE/README.md)"
  - "[docs/00-company](../../docs/00-company/README.md)"
  - "[Product Constitution](../../docs/00-company/PRODUCT_CONSTITUTION.md)"
  - "[Design Principles](../../docs/00-company/DESIGN_PRINCIPLES.md)"
  - "[Anti-Goals](../../docs/00-company/ANTI_GOALS.md)"
  - "[Glossary](../../docs/00-company/29-glossary-and-definitions.md)"
Tags: aios, constitution, rules, vocabulary, agents, stub
Source: AIOS v0.1.0 Sprint 1, amended per the Sprint 1 governance resolution draft (proposed, founder approval pending). No constitutional content has been written.
---

# 00 - Constitution

The rules an agent may not break, and the words it must use consistently.

> **No documents yet.** This section is a destination. Sprint 1 created it
> empty on purpose: writing rules before the roles and workflows they govern
> exist would produce rules nobody has tested against real work.

## Purpose

Three things belong here, and they support each other:

- **Rules** - constraints that hold across every role, model, and workflow.
  A rule is binding, not aspirational. It can be violated, it outranks
  convenience, and amending it is a recorded decision rather than a quiet edit.
- **Vocabulary** - the terms AIOS uses, defined once. Where a term already has
  a product meaning in the
  [Glossary](../../docs/00-company/29-glossary-and-definitions.md), the AIOS
  definition cites it rather than competing with it.
- **`AGENTS.md`** - the roster of agent roles and the authority model that
  governs them. It lives here, not in [01-ROLES](../01-ROLES/README.md),
  because it is constitutional: it establishes who may act and on what
  basis, not what any one role does day to day. 01-ROLES holds the
  individual role documents that `AGENTS.md` indexes.

This is *not* the Product Constitution, and it is not a Company Constitution.
[docs/00-company/PRODUCT_CONSTITUTION.md](../../docs/00-company/PRODUCT_CONSTITUTION.md)
constrains the product. A company-wide constitution, if and when one is
ratified, is expected at `docs/00-company/COMPANY_CONSTITUTION.md` and would
outrank both the Product Constitution and this section - it does not exist
yet. This section constrains agent behaviour only, and does not compete with
either.

This section also does not duplicate
[Design Principles](../../docs/00-company/DESIGN_PRINCIPLES.md) or
[Anti-Goals](../../docs/00-company/ANTI_GOALS.md). Those are canonical under
[docs/00-company](../../docs/00-company/README.md) and are referenced from
here, not forked. If AIOS ever needs a principle specific to agent conduct
rather than the product, it gets a distinct name so it is never mistaken for
the product-level document.

## Contents

Currently this README only.

What belongs here:

- Constraints that apply regardless of which agent is acting
- Terms whose meaning must not drift between documents or sessions
- The distinction between a binding rule and a default that may be overridden

What does not belong here:

- Anything true of only one role, model, or workflow - those have their own sections
- Product commitments of any kind
- Process for changing these rules - that is [05-GOVERNANCE](../05-GOVERNANCE/README.md)
- Duplicated copies of [Design Principles](../../docs/00-company/DESIGN_PRINCIPLES.md)
  or [Anti-Goals](../../docs/00-company/ANTI_GOALS.md) - reference them, don't fork them

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

This section is intended to outrank every other AIOS section. A workflow that
contradicts a rule here is expected to be wrong, not the rule.

That precedence takes effect only once rules exist and
[05-GOVERNANCE](../05-GOVERNANCE/README.md) defines ratification. Today the
section is empty, so it constrains nothing.

This section is subordinate to a ratified Company Constitution, should one
come to exist at `docs/00-company/COMPANY_CONSTITUTION.md`. Neither document
exists yet, so the ordering is stated and not yet in effect.

## Dependencies

| Depends on | Why |
|---|---|
| [Document Standards](../../docs/18-templates/DOCUMENT_STANDARDS.md) | Form of every file written here |
| [Glossary](../../docs/00-company/29-glossary-and-definitions.md) | Existing product terms the vocabulary must not redefine |
| [Design Principles](../../docs/00-company/DESIGN_PRINCIPLES.md), [Anti-Goals](../../docs/00-company/ANTI_GOALS.md) | Canonical product principles this section references rather than forks |
| [05-GOVERNANCE](../05-GOVERNANCE/README.md) | Nothing here becomes binding without a ratification process |

Sections 01-04 depend on this one. It depends on none of them.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| `RULES.md` | What may an agent never do, and what must it always do? |
| `VOCABULARY.md` | What does each AIOS term mean, and where did it come from? |
| `AGENTS.md` | Which agent roles exist, and on what authority does each act? |
| Mission | What is AIOS for, stated in one place? |
| Philosophy | What beliefs about agent work do the rules follow from? |

Whether mission and philosophy are separate files or headings inside `RULES.md`
is unresolved and belongs to Sprint 2.
