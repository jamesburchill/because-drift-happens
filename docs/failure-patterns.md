# Failure Patterns

Failure patterns describe recurring ways autonomous systems can lose coherence. They are not exhaustive. They are early labels for problems that should become easier to detect and discuss.

## Local Optimisation Drift

An agent, workflow, service, or team improves its local objective while weakening the larger system. The local action may be rational in isolation and harmful in aggregate.

## Context Collapse

The system acts as if it has enough context when key context is missing, stale, contradictory, or outside the current execution window.

## Policy Bypass

Execution avoids, ignores, misinterprets, or routes around a required policy checkpoint. This may happen through bad design, unclear authority, tool misuse, or accumulated exceptions.

## Recursive Delegation Drift

An agent delegates to another agent, which delegates again, causing intent, authority, and constraints to degrade with each handoff.

## Silent Workflow Degradation

A workflow continues to run while its quality, coverage, timeliness, or alignment declines. Basic success signals remain green while the real outcome weakens.

## Runaway Automation

An automated process repeats, expands, retries, spends, or modifies state beyond intended bounds because stop conditions are weak or missing.

## Conflicting Agents

Multiple agents take actions that are each locally valid but mutually incompatible. Conflict may appear only after shared state, cost, or external systems are affected.

## Stale Memory

The system treats outdated stored context as current truth. Stale memory can preserve old policies, old assumptions, obsolete facts, or previous exceptions.

## Authority Confusion

The system cannot determine who or what has permission to decide, approve, override, escalate, or act. Confusion can lead to delay, overreach, or unauthorised execution.

## Missing Escalation Path

The system encounters ambiguity, conflict, or risk but has no defined route to a responsible actor or control plane. Execution either stalls or continues without adequate authority.
