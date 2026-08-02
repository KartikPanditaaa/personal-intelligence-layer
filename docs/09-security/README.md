---
Status: Stub
Owner: Founder
Last Updated: 2026-08-02
Related Documents:
  - [Documentation Index](../README.md)
  - [Privacy](../10-privacy/README.md)
  - [Legal and Compliance Notes](../14-business/23-legal-and-compliance-notes.md)
  - [Integration Strategy](../04-architecture/13-integration-strategy.md)
  - [Risk Register](../00-company/25-risk-register.md)
Tags: security, index, stub
Source: New document. No security material exists in any source document.
---

# 09 — Security

Threat model, access control, and secure handling of user data.

> **No documents yet — and no source material either.**
>
> Unlike most stubs in this repository, this section does not summarise
> existing discussion, because there is none. Security was not discussed as a
> distinct topic in any migrated document. Privacy was discussed extensively;
> security was not.
>
> This is recorded as a gap rather than filled with assumptions.

## Adjacent material

| Topic | Location | Note |
|---|---|---|
| Privacy as a differentiator | [10-privacy](../10-privacy/README.md) | Related but distinct |
| Confidential information must not leak | [03-target-user-personas.md](../01-problem-space/03-target-user-personas.md) | Stated as a persona pain, not a security requirement |
| Compliance targets | [23-legal-and-compliance-notes.md](../14-business/23-legal-and-compliance-notes.md) | GDPR / SOC 2 / HIPAA listed as undecided |
| Security as a future role | [22-team-and-hiring-plan.md](../14-business/22-team-and-hiring-plan.md) | Reasoned |
| Integration authentication | [13-integration-strategy.md](../04-architecture/13-integration-strategy.md) | Requires founder decision |

## Why this gap matters

The product is intended to hold long-term memory of a user's work, and
[23-legal-and-compliance-notes.md](../14-business/23-legal-and-compliance-notes.md)
records that enterprise trust was discussed extensively. A system in that
position needs a threat model before it needs a stack.

## What belongs here when it exists

- Threat model and adversaries
- Authentication and authorization
- Encryption at rest and in transit
- Secrets handling
- Audit logging
- Incident response
- Third-party and integration security posture

## Recommended first document

An RFC establishing the threat model, using
[RFC_TEMPLATE.md](../18-templates/RFC_TEMPLATE.md), red-teamed with
[RED_TEAM_CHECKLIST.md § E](../18-templates/RED_TEAM_CHECKLIST.md).
