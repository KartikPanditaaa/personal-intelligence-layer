---
Status: Draft
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Documentation Index](../README.md)"
  - "[Documentation Roadmap](../DOCUMENTATION_ROADMAP.md)"
  - "[Decision Template](DECISION_TEMPLATE.md)"
  - "[ADR Template](ADR_TEMPLATE.md)"
  - "[RFC Template](RFC_TEMPLATE.md)"
Tags: standards, meta, process
Source: New document. Codifies conventions already implicit in the migrated blueprint and context notes.
---

# Document Standards

How every document in this repository is written, labelled, and linked.
This document defines form only. It never defines product substance.

## 1. Every document is self-contained

A reader must be able to open any single file and understand:

- what the document covers
- how confident the project is in each claim
- where the claim came from
- what to read next

Do not rely on folder position to carry meaning. State it in the document.

## 2. Frontmatter is mandatory

Every markdown file begins with:

```yaml
---
Status: Draft
Owner: Founder
Last Updated: YYYY-MM-DD
Related Documents:
  - "[Label](relative/path.md)"
Tags: comma, separated, lowercase
Source: Where this document's content originated
---
```

| Field | Meaning |
|---|---|
| `Status` | **Document lifecycle** — see section 3. Not the confidence of the claims inside. |
| `Owner` | Who is accountable for the document being correct. |
| `Last Updated` | ISO 8601 (`YYYY-MM-DD`). |
| `Related Documents` | Relative markdown links, **each wrapped in double quotes**. At least two where any exist. |
| `Tags` | Lowercase, comma-separated. Used for search. |
| `Source` | Origin of the content: a prior file path, a discussion, a research artefact, or `New document`. |

### Why the quotes are mandatory

An unquoted `- [Label](path.md)` is not the string it looks like. YAML reads
`[Label]` as a *flow sequence* and then fails on the trailing `(path.md)`:

```text
did not find expected '-' indicator while parsing a block collection
```

GitHub renders frontmatter with a strict YAML parser and shows that error
banner at the top of the page instead of the document. Double quotes force the
value to be read as a plain string.

Any value beginning with `[`, `{`, `*`, `&`, `!`, `%`, `@`, or a backtick needs
the same treatment.

## 3. Document lifecycle status

Applies to the file as a whole, in frontmatter.

| Status | Meaning |
|---|---|
| `Stub` | Placeholder. Structure exists, content does not. |
| `Draft` | Written but not reviewed. |
| `In Review` | Under active review or red-team. |
| `Ratified` | Reviewed and accepted by the owner. |
| `Superseded` | Replaced. Must link to its replacement. |
| `Archived` | No longer active. Lives in `19-graveyard/`. |

## 4. Claim status vocabulary

Applies to **statements inside** a document, not the document itself.
Never mix these in one list. Give each its own heading or its own labelled line.

| Label | Meaning | Test |
|---|---|---|
| **Decided** | A commitment has been made. | Someone with authority chose this. Reversing it requires a new decision record. |
| **Proposed** | Put forward for consideration. Not yet chosen. | A reasonable person could still reject it without contradicting anything. |
| **Hypothesis** | A belief about the world we hold but have not tested. | It could be shown false by evidence. |
| **Requires Validation** | A hypothesis with a validation method attached and queued. | We know how we would test it. |
| **Rejected** | Considered and ruled out. Rationale retained. | Must state why. Must never be deleted. |
| **Deferred** | Deliberately postponed. | Must state what unblocks it. |

Preferred form:

```markdown
## Memory retention window

**Status: Hypothesis**

Users value memory that persists beyond a single session.

**Basis:** Discussion, see [Problem Deep Dive](../01-problem-space/02-problem-deep-dive.md).
**Validation:** Not yet designed. Tracked in [Assumptions to Validate](../02-research/26-assumptions-to-validate.md).
```

## 5. Legacy label mapping

Documents migrated from `blueprint/` and `context/` use an earlier three-label
vocabulary. **Those labels have been left exactly as written.** They were not
rewritten, because reclassifying a claim changes its meaning, and that is a
founder decision rather than a documentation decision.

| Legacy label | Closest current label | Notes |
|---|---|---|
| `Decided` | `Decided` | Direct equivalent. |
| `Reasoned` | `Proposed` — *provisionally* | Ambiguous in the source. Some `Reasoned` items read as `Proposed`, others as `Hypothesis`. Per-item reclassification is **open**. |
| `Requires founder decision` | `Deferred` — *provisionally* | Distinct in origin: it marks an unmade decision rather than a postponed one. Whether to fold it into `Deferred` or keep it as a seventh label is **open**. |

Resolving this mapping is tracked in the [Documentation Roadmap](../DOCUMENTATION_ROADMAP.md).
Until it is resolved, **do not** bulk-rewrite legacy labels.

New documents use the section 4 vocabulary only.

## 6. Traceability

Every `Decided` claim must be traceable to one of:

1. **Discussion** — cite the thread, date, or originating note.
2. **Research** — link a document in `02-research/`.
3. **Customer evidence** — link an interview record.
4. **Founder decision** — link a record in `16-decisions/`.

If a claim cannot be traced, it is not `Decided`. Label it `Proposed` and note the gap.

**Rationale is never removed.** When a decision is reversed, the original record
stays, is marked `Superseded`, and links forward to what replaced it.

## 7. Linking

- Links are relative and end in `.md`.
- Every document links to its section `README.md`.
- Every claim borrowed from another document links to that document rather than restating it.
- Broken links are a defect. Check them when moving files.

## 8. Writing rules

- One idea per heading.
- Prefer a list over a paragraph when enumerating.
- Prefer a table over a list when items share attributes.
- Do not editorialise inside a research document. Findings and interpretation get separate headings.
- Do not use a number unless its source is cited.
