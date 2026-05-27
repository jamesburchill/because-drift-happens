# Architecture Patterns

These pattern stubs are starting points for future expansion. Each pattern should eventually include intent, context, forces, implementation notes, risks, and example signals.

## Drift Detector

Identifies movement away from expected behaviour, policy, state, cost, quality, or outcome. A drift detector should distinguish normal adaptation from movement that weakens coherence.

## Governance Checkpoint

Evaluates policy, authority, risk, context, or constraints before execution continues. A checkpoint can approve, reject, hold, or escalate.

## Runtime Veto

Stops an action while the system is running. A runtime veto should record the triggering condition, relevant context, authority, and next available path.

## Coherence Boundary

Defines where coherence expectations apply and who is responsible for maintaining them. A boundary may surround an agent group, workflow, domain, organisation, or federation.

## Policy-Aware Delegation

Carries policy, authority, constraints, and context when work is delegated. The receiving actor should know not only what to do, but also what bounds apply.

## Federation Health Signal

Reports whether a federated set of agents or systems remains within acceptable operating bounds. Signals may include conflict rate, stale context, veto rate, escalation load, cost variance, and unresolved drift.

## Escalation Router

Routes ambiguous, risky, conflicting, or unauthorised situations to the right actor or control plane. Routing should be explicit, auditable, and connected to authority.

## Audit Trail Spine

Provides a consistent record across agents, tools, workflows, and control-plane decisions. The spine should connect intent, context, authority, action, policy checks, state changes, and outcome.
