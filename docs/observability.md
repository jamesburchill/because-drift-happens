# Observability

Observability for autonomous systems must include more than logs, traces, and metrics. Those remain necessary, but they are not sufficient when systems interpret intent, use tools, delegate work, and change state.

The system must be observable at the level where governance decisions are made.

## What Must Be Observed

Autonomous systems should make the following visible where practical:

- **Intent:** What the system or agent is trying to accomplish.
- **Context:** What information the action was based on.
- **Action:** What was done or proposed.
- **Delegation:** What work was delegated, to whom, and under what constraints.
- **Tool use:** Which tools were invoked, with what authority, and with what result.
- **Policy checks:** Which policies were evaluated and what they returned.
- **State changes:** What changed in the system of record.
- **Exceptions:** What failed, timed out, conflicted, or required alternate handling.
- **Cost:** What resources, money, tokens, time, or operational capacity were consumed.
- **Outcome:** What result occurred and whether it matched intent.

## Observability And Intervention

Observability without intervention becomes theatre. Seeing a problem is not enough if the system cannot pause, redirect, contain, or escalate.

Instrumentation should therefore connect to control surfaces. A useful signal should help a person, agent, or control plane decide what to do next.

## Interpretable Records

Audit records should be understandable after the fact. A useful record explains the action, context, authority, policy checks, state change, and outcome in terms that support accountability.
