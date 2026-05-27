# Governance Checkpoint Example

## Scenario

An agent proposes to update a customer-facing operational message after detecting a service degradation.

## Proposed Action

Publish a revised message to the public status page.

## Checkpoint Inputs

- Current incident status.
- Source of the proposed message.
- Authority of the proposing agent.
- Policy for customer-facing updates.
- Whether legal, support, or operations review is required.
- Difference between the proposed message and the approved incident language.

## Checkpoint Decision

The checkpoint allows low-impact internal updates automatically, but public status messages require approval from the incident commander or designated communications owner.

## Result

The action is held. The proposed message, context, policy result, and required approver are recorded. The incident commander receives an escalation with the proposed text and evidence.

## Coherence Effect

The system preserves speed while keeping external communication under explicit authority.
