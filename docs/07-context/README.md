---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[Documentation Index](../README.md)"
  - "[System Architecture](../04-architecture/10-system-architecture.md)"
  - "[Memory](../06-memory/README.md)"
  - "[Integration Strategy](../04-architecture/13-integration-strategy.md)"
Tags: context, index, stub
Source: New document. Distinct from the former top-level `context/` directory, whose contents were distributed by subject.
---

# 07 — Context

The context engine: gathering, scoping, and supplying the right information at
the right moment.

> **No documents yet.**

> **Naming caution.** This section is *not* the old top-level `context/`
> directory. That directory held general planning notes, and its five files
> were distributed by subject:
>
> | Original | Now at |
> |---|---|
> | `context/product-brief.md` | [03-product/product-brief.md](../03-product/product-brief.md) |
> | `context/technical-plan.md` | [04-architecture/technical-plan.md](../04-architecture/technical-plan.md) |
> | `context/decisions-log.md` | [16-decisions/decisions-log.md](../16-decisions/decisions-log.md) |
> | `context/competitive-landscape.md` | [02-research/competitive-landscape.md](../02-research/competitive-landscape.md) |
> | `context/open-questions.md` | [01-problem-space/open-questions.md](../01-problem-space/open-questions.md) |
>
> This section means *context* in the product sense: what the system knows
> about the user's current situation.

## Where context is currently discussed

| Statement | Location | Status |
|---|---|---|
| Context Engine in the component flow | [10-system-architecture.md](../04-architecture/10-system-architecture.md) | Reasoned |
| Universal context engine | [technical-plan.md](../04-architecture/technical-plan.md) | Speculative |
| Preserve context | [01-vision-and-thesis.md](../00-company/01-vision-and-thesis.md) | Decided |
| Context loss as a core pain point | [02-problem-deep-dive.md](../01-problem-space/02-problem-deep-dive.md) | Decided |
| Context as a differentiator | [04-positioning-and-differentiation.md](../00-company/04-positioning-and-differentiation.md) | Decided |
| Context explosion as a risk | [14-scalability-and-risk.md](../04-architecture/14-scalability-and-risk.md) | Discussed |
| Contextual workspaces / dynamic expertise | [decisions-log.md](../16-decisions/decisions-log.md) | Direction shift recorded |

## Context versus memory

The sources do not draw this boundary, and it will need drawing. A working
distinction to argue with rather than adopt: memory is what persists, context
is what is relevant right now. Where that line falls is undecided — see
[06-memory](../06-memory/README.md).

## What belongs here when it exists

- Context sources and how they are gathered
- Scoping and relevance selection
- Handling context explosion at scale
- Cross-application context propagation
- What the user can see and suppress
