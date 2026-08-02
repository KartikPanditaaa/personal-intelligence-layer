---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - "[AIOS Index](../README.md)"
  - "[Roles](../01-ROLES/README.md)"
  - "[Models](../02-MODELS/README.md)"
  - "[Templates](../04-TEMPLATES/README.md)"
Tags: aios, workflows, prompts, stub
Source: AIOS v0.1.0 Sprint 1. Structure only — no workflow has been written.
---

# 03 — Workflows

The sequences agents follow, and the prompts that drive them.

> **No documents yet.** No workflow has been written and no prompt has been
> authored. Sprint 1 created the destination only.

## Purpose

A workflow composes roles into an ordered piece of work: what happens first,
what each step must produce before the next begins, and what stops the sequence.

Each workflow is expected to state:

1. **Trigger** — what starts it
2. **Steps** — which role acts at each step, in order
3. **Gate** — what each step must produce before the next may begin
4. **Exit** — what "done" means, and what aborts it

Prompts live here rather than in [01-ROLES](../01-ROLES/README.md) because a
prompt is an instance of how a role is invoked at a step, not the definition of
the role. The same role may be prompted differently in different workflows.

## Contents

Currently this README only.

What belongs here:

- One document per workflow
- Prompt files, each traceable to the workflow step it serves

What does not belong here:

- Role definitions restated inline — link to [01-ROLES](../01-ROLES/README.md)
- Model choices — those are [02-MODELS](../02-MODELS/README.md)
- Blank forms a workflow's output is written into — those are
  [04-TEMPLATES](../04-TEMPLATES/README.md)

A workflow that cannot be described as an ordered list of existing roles is a
sign that a role is missing, not that the workflow needs its own definitions.

## Authority

**Status: Proposed.** Sourced to the AIOS v0.1.0 Sprint 1 brief. Not ratified.

Workflows are the most subordinate operational section. They may sequence roles
and consume model assignments; they may not redefine either, and they may not
override [00-CONSTITUTION](../00-CONSTITUTION/README.md). Where a workflow
appears to require breaking a rule, the workflow is wrong.

Workflows bind nothing below them.

## Dependencies

| Depends on | Why |
|---|---|
| [01-ROLES](../01-ROLES/README.md) | Steps are role invocations; without roles there is nothing to sequence |
| [02-MODELS](../02-MODELS/README.md) | Each step runs on an assigned model |
| [00-CONSTITUTION](../00-CONSTITUTION/README.md) | Rules constraining every step |
| [04-TEMPLATES](../04-TEMPLATES/README.md) | Where step output is written |

This is the most dependent section in AIOS and should be written last.

## Future Documents

**Not created by Sprint 1.**

| Document | Answers |
|---|---|
| One file per workflow | What is the trigger, step order, gate, and exit? |
| Prompt files | How is a given role invoked at a given step? |
| Workflow index | Which workflows exist, and when is each used? |

Whether prompts are stored as separate files or embedded in the workflow
document that uses them is unresolved. Separate files are reusable across
workflows; embedded prompts stay readable in context.
