---
Status: In Review
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[RFC Index](README.md)"
  - "[RFC Template](../18-templates/RFC_TEMPLATE.md)"
  - "[Red Team Checklist](../18-templates/RED_TEAM_CHECKLIST.md)"
  - "[Decisions Log](../16-decisions/decisions-log.md)"
  - "[Product Brief](../03-product/product-brief.md)"
  - "[Product Scope v1](../03-product/05-product-scope-v1.md)"
  - "[Data Model](../04-architecture/12-data-model.md)"
  - "[Assumptions to Validate](../02-research/26-assumptions-to-validate.md)"
Tags: rfc, context-engine, memory, privacy, local-first, v1
Source: Founder review session 2026-08-02; decisions recorded in 16-decisions/decisions-log.md.
---

# RFC-0001: Personal Context Engine

**Claim status:** Proposed
**Author:** Founder (drafted with Claude)
**Created:** 2026-08-02
**Discussion window closes:** _TBD (founder to set)_
**Outcome:** Open
**Resulting record:** _pending — on acceptance, produces ADR-0001 (system shape) and promotes the Proposed items in the 2026-08-02 decisions-log section to Decided_

## Summary

Propose a **Personal Context Engine (PCE)**: a local-first, user-owned store
of a developer's context — projects, preferences, decisions, goals,
constraints — injected into one AI coding tool so the user stops re-explaining
themselves. v1 is deliberately four capabilities and one tool, built to test
whether developers will actually maintain such a layer.

## Motivation

Developers using AI coding tools repeatedly re-explain the same project
structure, constraints, decisions, and preferences because the AI forgets
between sessions and across tools — so the human becomes the memory. This is
the sharpest, best-evidenced pain in the
[Product Brief](../03-product/product-brief.md) and
[Problem Deep Dive](../01-problem-space/02-problem-deep-dive.md).

Honest evidence note: the pain is well-attested in discussion, but the specific
bet — that users will *maintain* a dedicated context layer — is **untested**.
See [Assumptions to Validate](../02-research/26-assumptions-to-validate.md).
This RFC's implementation exists primarily to test that.

The PCE is the platform tier: Personal Intelligence Layer (vision) → Personal
Context Engine (platform) → persistent context for AI coding (first product).
Memory is one part of context, not the product itself.

## Guide-Level Explanation

To a new teammate: today you re-tell Claude/Cursor your stack, conventions, and
past decisions every session. The PCE remembers those *for you*, on your
machine, and hands the relevant slice to your coding tool automatically.

Four things, nothing more, in v1:

1. **Persistent context** — it captures projects, preferences, decisions,
   goals, constraints.
2. **Context injection** — it feeds the relevant slice into one coding tool.
3. **Confirm-to-learn** — it never learns silently; it proposes ("Remember
   that you prefer X?") and you accept, edit, or reject.
4. **Inspect / edit / delete** — everything it knows is visible and removable
   in plain form.

Because the human-readable surface is Markdown, "inspect what it knows" is
close to free.

## Reference-Level Explanation

**Storage (prototype).** Local-first; human-readable Markdown as the surface,
SQLite as the index/relationship store. No cloud. No account. Embeddings
deferred until retrieval quality demands them.

**Data model.** Relationship-oriented: entities (User, Workspace, Project,
Preference, Decision, Goal, Constraint, Memory) and *typed edges* between them,
so it can grow into a knowledge graph without a rewrite. Not isolated per-item
files. Exact schema is out of scope here → Memory Model RFC.

**Capture & confirm-to-learn.** Candidate memories are proposed, never written
silently. Secret-detection runs on capture so credentials are never persisted.

**Injection.** A scoped, reviewable slice of context is provided to one tool
(proposed: Claude Code). Selection logic and prompt-budget handling are out of
scope here → Context Injection RFC.

**Privacy boundaries.**
- *Stored (Proposed):* project context, stated preferences, decisions, goals,
  style samples, corrections.
- *Never stored (Proposed):* secrets/credentials/keys; raw source unless
  explicitly opted in; nothing leaves the device without consent.
- Exact, testable rules → Privacy Model RFC.

**Trust properties.** Trust is delivered as a *property* (inspectability +
confirm-to-learn + local ownership), not a metric. Formal trust measurement is
Deferred.

## Drawbacks

- The whole thesis may be false: users may ignore the layer and keep
  re-explaining. If so, this is wasted build — though cheaply, and it is
  exactly what the prototype measures.
- A context layer that injects stale or wrong context makes the AI *worse*.
- Maintaining a separate store is user effort; effort that does not visibly pay
  back gets abandoned.
- Graph ambition could balloon scope if not held to Markdown + SQLite.

## Rationale and Alternatives

| Option | Why not / why |
|---|---|
| Do nothing; rely on the tool's own memory | Cheapest, but cedes the wedge to incumbents and never tests the thesis. **Rejected.** |
| Single Markdown context file (a richer `CLAUDE.md`) | Cheap, instantly inspectable, but no relationships and caps out fast. Good fallback, insufficient as the model. |
| **Relationship-oriented store, Markdown surface + SQLite** | Human-readable and inspectable, yet schema captures entities + edges so it can become a graph without a rewrite. **Recommended.** |
| Full graph DB + embeddings now | Most powerful, most over-built for a prototype whose job is to test whether anyone maintains this at all. **Deferred (YAGNI).** |

Impact of not doing this: we keep planning a broad platform with no buildable,
testable slice, and the beachhead stays theoretical.

## Prior Art

Cursor rules/memory, GitHub Copilot instructions, Claude Code `CLAUDE.md` /
memory, Continue.dev context. See
[Competitive Landscape](../02-research/competitive-landscape.md). What they get
wrong for our purposes: context is **tool-owned and tool-locked**, not
user-owned and portable. `CLAUDE.md`-style files prove developers *will*
maintain persistent, human-readable context when it pays off — evidence for
feasibility. The gap: no incumbent gives the user a tool-agnostic, local,
inspectable context store that follows them across tools. That is the wedge.

## Unresolved Questions

In scope for the child RFCs / the decision this triggers, not for this RFC:

- Exact entity/relationship schema → **Memory Model RFC**.
- Context selection & injection without leaking secrets or overflowing the
  prompt → **Context Injection RFC**.
- Precise never-store rules and secret detection → **Privacy Model RFC**.
- Confirm-to-learn mechanics for profile evolution → **User Profile RFC**.
- Which single tool is first (Proposed: Claude Code).

## Future Possibilities

**Not part of this proposal.** Cross-application context across many tools;
writing/planning/research surfaces; team/shared context; embeddings-based
retrieval; a true knowledge graph. All Deferred and gated on validating v1.

## Red Team

Not yet performed. Per
[17-rfcs process](README.md), an RFC accepted without a recorded red team has
not followed process. Run [RED_TEAM_CHECKLIST](../18-templates/RED_TEAM_CHECKLIST.md)
before setting an outcome. Known lead concern to stress-test: the maintenance/
abandonment risk (does anyone keep the layer current?).
