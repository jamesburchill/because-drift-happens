# Drift Signal Example

## Scenario

An autonomous workflow prepares weekly operational summaries. It uses recent tickets, deployment notes, and incident records.

## Expected Behaviour

The summary should reflect the current week, include material exceptions, and identify unresolved operational risk.

## Drift Signal

For three weeks, the workflow marks summaries as complete while omitting open incidents that were tagged after the initial retrieval step.

## Interpretation

The workflow has not fully failed. It still produces a document. The drift is in coverage and freshness. The system is treating an early context snapshot as if it remains complete.

## Coherence Risk

The organisation may believe unresolved risk has been reviewed when it has not. The output remains plausible, which makes the drift harder to detect.

## Possible Response

- Add a freshness check before final summary generation.
- Record the retrieval window in the audit trail.
- Flag unresolved incidents added after the first retrieval.
- Hold publication if unresolved high-priority incidents were not evaluated.
