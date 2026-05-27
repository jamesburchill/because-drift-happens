# Runtime Intervention Example

## Scenario

A multi-agent remediation workflow detects repeated job failures and begins restarting services.

## Observed Condition

The restart count exceeds the normal threshold. Error rates continue to rise. A second agent begins scaling related workers based on queue depth.

## Intervention Trigger

The control plane detects conflicting remediation actions and rising blast-radius risk.

## Intervention

The system places the remediation workflow on hold, blocks further restarts, allows read-only diagnostics, and escalates to the on-call operator.

## Recorded Evidence

- Agents involved.
- Actions already taken.
- Tool calls attempted.
- Restart count.
- Queue-depth signal.
- Policy checkpoint result.
- Reason for hold.
- Escalation target.

## Coherence Effect

The intervention prevents local remediation from creating wider instability while preserving enough context for a responsible operator to decide the next action.
