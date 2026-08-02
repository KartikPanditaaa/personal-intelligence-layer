---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Assumptions to Validate](../02-research/26-assumptions-to-validate.md)"
  - "[Decisions Log](../16-decisions/decisions-log.md)"
  - "[Documentation Roadmap](../DOCUMENTATION_ROADMAP.md)"
  - "[Decision Template](../18-templates/DECISION_TEMPLATE.md)"
Tags: problem-space, open-questions, backlog
Source: Migrated verbatim from `context/open-questions.md`
---

# Open Questions

-   How should enterprise privacy be implemented?
-   What deployment model should enterprise use?
-   How should long-term memory work technically?
-   What should the first product actually be?
-   What is the first beachhead market?
-   What is the pricing model?
-   How should voice fit into v1?
-   What data should be stored?
-   What data should never be stored?
-   How should trust be measured?
-   How should growth be measured?
-   Which features belong in v1?
-   How should cross-application context work?
-   How should user-controlled profiles evolve?
-   Which assumptions require user research?

---

## Resolution status (2026-08-02)

The list above is preserved verbatim as migrated. This section maps each
question to its current status per the
[Decisions Log § 2026-08-02](../16-decisions/decisions-log.md) and
[RFC-0001](../17-rfcs/RFC-0001-personal-context-engine.md). Inline labels above
were intentionally not rewritten.

| Question | Status |
|---|---|
| What should the first product actually be? | **Decided** — Personal Context Engine; v1 = persistent context for AI coding |
| What is the first beachhead market? | **Decided** — solo developers/vibe coders using AI coding tools |
| Which features belong in v1? | **Decided** — the four-item scope |
| How should voice fit into v1? | **Decided** — it does not (Deferred beyond v1) |
| How should long-term memory work technically? | **Decided (prototype)** — local-first Markdown + SQLite, relationship-oriented; detail → Memory Model RFC |
| How should user-controlled profiles evolve? | **Decided in principle** — confirm-to-learn; mechanics → User Profile RFC |
| What data should be stored? | **Proposed** — see decisions log |
| What data should never be stored? | **Proposed** — exact rules → Privacy Model RFC |
| Which assumptions require user research? | **Hypothesis / Requires Validation** — riskiest: will users maintain a context layer |
| How should enterprise privacy be implemented? | **Deferred** |
| What deployment model should enterprise use? | **Deferred** |
| What is the pricing model? | **Deferred** |
| How should trust be measured? | **Deferred** — v1 uses inspectability as the mechanism, not a metric |
| How should growth be measured? | **Deferred** |
| How should cross-application context work? | **Deferred** — v1 is one tool only |
