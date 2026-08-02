---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Decision Template](../18-templates/DECISION_TEMPLATE.md)"
  - "[Decision Log Template](../18-templates/28-decision-log-template.md)"
  - "[ADR Template](../18-templates/ADR_TEMPLATE.md)"
  - "[Graveyard](../19-graveyard/README.md)"
  - "[Open Questions](../01-problem-space/open-questions.md)"
  - "[RFC-0001: Personal Context Engine](../17-rfcs/RFC-0001-personal-context-engine.md)"
Tags: decisions, log, history, pivots, personal-context-engine
Source: Migrated verbatim from `context/decisions-log.md`
---

# Decisions Log

## Concrete decisions made

-   Product direction shifted from an AI coding IDE toward a broader
    Personal Intelligence Layer.
-   Human capability is a core design principle.
-   Privacy should be a product differentiator.
-   Trust should be observable and inspectable.
-   Memory should extend beyond conversations.
-   Product should co-evolve with the user.
-   Research phase should precede implementation.
-   Claude Code/Codex intended for implementation later.
-   ChatGPT role: product strategy, research, architecture planning,
    critical review.
-   Build a research canon before architecture.
-   Maintain decision logs and research evidence.
-   Use red-team reviews for major ideas.
-   Separate hidden platform from visible products.

## Positioning discussions

-   Not another autocomplete.
-   Not another AI IDE.
-   Build an intelligence layer.

## Pricing direction

Not yet defined.

## Technology stack

Not yet defined.

## Pivots and reversals

-   Initial focus: AI coding IDE.
-   Expanded to writing assistant.
-   Expanded again into a Personal Intelligence Layer.
-   Discussion moved from 'modes' toward contextual workspaces/dynamic
    expertise.
-   Moved from 'AI learns' toward 'AI and user co-evolve.'

---

## 2026-08-02 — Personal Context Engine direction (session decisions)

New decisions from the founder review session. Recorded in the current
claim-status vocabulary
([DOCUMENT_STANDARDS § 4](../18-templates/DOCUMENT_STANDARDS.md)). The
earlier sections above are preserved verbatim as migrated; nothing there
was rewritten. Items marked **Proposed** are **not** binding — they await
either founder approval or acceptance of
[RFC-0001](../17-rfcs/RFC-0001-personal-context-engine.md).

### Decided

- **Company vision is unchanged: the Personal Intelligence Layer.**
  Narrowing the first product does not narrow the vision.
- **Three-tier hierarchy.** Vision: Personal Intelligence Layer →
  Platform: Personal Context Engine → First product: persistent context
  for AI coding workflows (one tool). (Platform-tier naming settled;
  wording may be refined.)
- **The product is a Personal Context Engine, not a "memory layer."**
  Memory is an implementation detail. What the user buys is never having
  to repeatedly explain themselves, their projects, preferences, or
  decisions. Context = memory + constraints + decisions + goals +
  preferences + project state, and the relationships between them.
- **Beachhead: solo developers / vibe coders already using AI coding
  tools.** Single first market. Founder is the initial dogfood user.
- **Core product principles (permanent, beyond v1):** local-first;
  confirm-to-learn (system proposes, user approves — no silent learning);
  inspect/edit/delete everything the system knows; human growth (design
  to make the user more capable over time, retained even though v1 will
  not measure it); augment rather than replace.
- **v1 scope, exhaustive:** (1) persistent context, (2) context
  injection into one coding workflow, (3) confirm-to-learn, (4)
  inspect/edit/delete. Nothing beyond this until validated.
- **Validation gate.** Nothing is added beyond the four v1 items until it
  is validated that users actually want and maintain a personal context
  layer.
- **Prototype technical direction.** Local-first; human-readable Markdown
  + SQLite; no cloud; embeddings deferred. Conceptual data model is
  relationship-oriented (entities + edges), designed to evolve into a
  knowledge graph without a product rethink — not isolated memory files.
- **Process: RFC-before-implementation.** Every major capability starts
  with an RFC. This is consistent with the existing
  [17-rfcs](../17-rfcs/README.md) process.
- **Minimum-question prototyping.** Answer only the questions needed to
  build a meaningful prototype; defer the rest deliberately.
- **Voice is cut from v1.** (See Deferred for its future status.)

*Note: the founder-requested decision categories
(Decided / Proposed / Hypothesis / Deferred / Rejected) already exist in
this repo as the claim-status vocabulary, plus `Requires Validation`.
No new taxonomy was introduced.*

### Proposed (awaiting founder approval — not binding)

- **Data stored (v1):** project context, stated preferences, decisions,
  goals, style samples, corrections.
- **Data never stored (v1):** secrets/credentials/keys; raw source code
  unless explicitly opted in; nothing leaves the device without consent.
  (Exact, testable rules → Privacy Model RFC.)
- **First integration surface = Claude Code** (founder uses it daily),
  ahead of Cursor/Copilot.
- **Prototype value signal:** captured context measurably reduces
  repeated explanation / re-prompting over time.

### Hypothesis

- Users will actually maintain a personal context layer rather than
  ignore it and keep re-explaining. *(Riskiest assumption; the prototype
  exists mainly to test it.)*
- Persistent context meaningfully reduces repeated prompting.
- Confirm-to-learn builds more trust than silent learning.
- (Carried) Privacy-first/local is commercially valuable; personalization
  increases retention; users prefer one context layer over many tools —
  see [Assumptions to Validate](../02-research/26-assumptions-to-validate.md).

### Requires Validation

- The riskiest-assumption test above is the prototype's explicit
  validation method for the "users maintain a context layer" hypothesis.

### Deferred

- Enterprise privacy implementation; enterprise deployment; pricing
  model; formal trust *measurement* (v1 uses inspectability as the trust
  mechanism, not a metric); growth/"human capability" measurement;
  cross-application context (v1 = one tool); voice; expansion into
  writing/planning/research surfaces; multi-market expansion (knowledge
  workers, students, corporate).

### Rejected

- Positioning as "the memory layer for AI coding" — memory is an
  implementation detail, not the product.
- Silent / automatic learning — violates confirm-to-learn and user
  ownership.
- Cloud dependency in v1 — violates local-first.
- Isolated per-item memory files as the core model — not evolvable into a
  knowledge graph.
- (Carried) Autocomplete / AI-IDE / chat-wrapper positioning.
- Building the broad multi-domain product in v1.

### Affects existing documents

These migrated docs now conflict with the decisions above and need a
founder pass (mark `Superseded`/update — not done here, per the
no-bulk-rewrite rule):

- [15-market-sizing](../15-go-to-market/15-market-sizing.md) — lists five
  markets as "Decided"; superseded by the single beachhead above.
- [05-product-scope-v1](../03-product/05-product-scope-v1.md) — v1 scope
  is now the four-item list.
- [04-positioning](../00-company/04-positioning-and-differentiation.md) —
  add the "not a memory layer" rejection and the hierarchy.
- [12-data-model](../04-architecture/12-data-model.md) — relationship-
  oriented direction.
