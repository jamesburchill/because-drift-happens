---
title: "RFC 0001: Framework Scope"
description: "The accepted scope of the broad Drift Doctrine and its technical framework, including non-goals and implementation-neutral boundaries."
content_type: "scope-decision"
maturity: "accepted"
---

# RFC 0001: Framework Scope

## Status

Accepted as initial repository scope.

## Summary

This RFC defines the initial scope, non-goals, terminology policy, and relationship between Because Drift Happens and future implementation repositories.

## Scope

Because Drift Happens is a public doctrine about drift across businesses, teams, processes, and technology. The six-line [Drift Doctrine](../doctrine.md) is the stable reference; AI is one application, not its boundary.

The technical framework applies that doctrine to intelligent and autonomous systems as they adapt, delegate, and drift. It focuses on:

- Drift in dynamic, autonomous, and multi-agent systems.
- Operational coherence under change.
- Governance as runtime regulation.
- Control planes above agents, workflows, tools, and federations.
- Observability that includes intent, context, policy, authority, action, state change, cost, and outcome.
- Intervention mechanisms such as vetoes, holds, escalations, rollback triggers, and containment.
- Failure patterns and architecture patterns for drift-aware system design.

## Non-Goals

This repository does not aim to:

- Define a complete software product.
- Promote a vendor or implementation.
- Provide legal, compliance, or regulatory advice.
- Make universal claims about all autonomous systems.
- Replace domain-specific safety, security, or risk practices.
- Publish private, client, commercial, or confidential material.

## Terminology Policy

Terms should be added or changed carefully. A term belongs in the framework when it helps people reason more clearly about operational drift, coherence, governance, federation, intervention, or control planes.

Terminology should:

- Use plain language.
- Avoid unnecessary novelty.
- Be defined in the glossary when used as a framework term.
- Be connected to operational meaning.
- Avoid hype, fear-based framing, and vague thought-leadership language.
- Be reviewed for consistency across existing documents.

## Relationship To Implementation Repositories

This repository defines doctrine and vocabulary. Future implementation repositories may demonstrate or apply these ideas, but they should not redefine the core terms casually.

Implementation repositories may include code, tools, agents, control-plane services, governance engines, observability components, or example systems. Their licences, maturity, and architecture may differ.

The doctrine repository should remain implementation-neutral. It may reference related implementation repositories once they are public and appropriately scoped.

## Open Questions

- Which diagrams should become canonical first?
- Which failure patterns need evidence-backed examples?
- Which governance concepts require stricter definitions before implementation work references them?

Page maturity is now identified using the [content maturity labels](../reading-map.md#content-maturity). Those labels distinguish the stable core from working interpretations, illustrative examples, and planned work; they do not settle the remaining evidence questions above.
