---
title: "Guided Exercise: Recognize and Respond to Drift"
description: "Practise identifying intent, assessing evidence, establishing authority, and choosing a response to drift in a business or technical workflow."
content_type: "exercise"
maturity: "illustrative"
---

# Guided Exercise: Recognize and Respond to Drift

Allow about 15–20 minutes after either [reading path](reading-map.md). You will produce a short response plan that separates a drift signal from a conclusion and connects action to evidence and authority.

By the end, you should be able to identify the intended outcome, distinguish facts from assumptions, choose a proportionate intervention, and explain how you would verify the result. This is a hypothetical practice scenario, not an assessment or certification.

Write your answers before opening the suggested response. There can be more than one reasonable response; the aim is to make your reasoning inspectable.

## The Scenario

It is Wednesday morning. Your team supplies a customer with a weekly report. The report supports the customer’s Monday planning meeting.

You have four records:

- **Customer agreement:** deliver a reviewed report by Friday at 4 p.m. The account manager owns the commitment. Changing the delivery date requires the account manager and customer to agree.
- **Operating procedure:** the analyst prepares the report; the team lead reviews it before release. Only the team lead can approve an alternative review arrangement.
- **Tuesday’s planning update:** the analyst forecasts completion on Monday because source data is late. The team lead has not yet assessed a recovery option.
- **Status dashboard:** the item is green because the report-generation job ran successfully. There is no record of a completed report, review, or customer-approved date change.

You have been asked to assess the situation and recommend the next step. You have no authority to change the commitment or release an unreviewed report.

## 1. Establish the Intent

What outcome matters to the customer? What promise and review requirement define acceptable delivery? Separate the purpose from the process used to achieve it.

Complete: **“Success means …, subject to …”**

## 2. Identify the Drift Signal

Where do the records disagree? Which observations support a concern? What would be premature to conclude?

Write three short lists: **known facts**, **reasonable inferences**, and **unanswered questions**. Include the age and limits of the evidence: a Tuesday forecast may have changed by Wednesday.

## 3. Establish Authority

Who can verify the forecast, approve a review arrangement, and agree on a changed customer commitment? What can you recommend or investigate yourself, and what needs someone else’s decision?

Do not treat access to the dashboard as authority to change the promise.

## 4. Choose a Proportionate Response

What is the smallest useful next action? Decide what needs checking, what should be flagged, and what should wait for approval. Explain why your response fits the evidence and the time remaining before Friday.

Consider both possibilities: the team may recover the original plan, or an explicitly agreed change may better serve the customer. Neither possibility is established yet.

## 5. Define Follow-Through

Name an owner, a proposed next check, and the evidence needed to close the exception. How will you distinguish a completed job from an acceptable customer outcome? What happens if the check cannot be completed?

Use this response record:

```text
Intended outcome and operating bounds:
Observed change and source:
What is known / inferred / still unknown:
Decision owner and authority required:
Proposed immediate response:
Next check, owner, and proposed time:
Evidence required to close the exception:
Escalation if evidence or progress is missing:
```

## Compare Your Reasoning

??? note "Suggested response — open after writing your own"

    **Intent:** provide a reviewed report by Friday at 4 p.m. so the customer can prepare for Monday’s meeting. A successful generation job is only one step towards that outcome.

    **Signal:** Tuesday’s Monday completion forecast conflicts with Friday’s commitment. The green dashboard reflects job execution, not report completion, review, or delivery. The promise is at risk; a missed deadline has not yet occurred. Missing approval records do not prove that no conversation happened, so check before concluding.

    **Evidence to obtain:** ask the analyst for the current forecast and data availability; ask the team lead about review capacity and recovery options; ask the account manager whether the customer has agreed to any change. Record the source and time of each confirmation.

    **Authority:** the analyst supplies the forecast. The team lead decides review arrangements. The account manager and customer agree on any delivery-date change. Your role is to surface the discrepancy and recommend action, not silently revise the commitment or waive review.

    **Immediate response:** flag the delivery risk to the team lead and account manager, with the conflicting records. Recommend checking recovery options before promising a new date. Preserve the original commitment as the comparison point until an authorized change is recorded. Do not release an unreviewed report to make the dashboard appear healthy.

    **Follow-through:** propose that the team lead confirm a feasible preparation and review plan by Wednesday at noon, with the account manager coordinating any customer decision. That is a proposed checkpoint, not an already accepted assignment. If confirmation is missing, escalate the unresolved risk to those owners. An updated forecast alone does not close the exception: closure needs evidence of delivery and review against the agreed commitment, or a recorded authorized change with the remaining work tracked.

    **Doctrine connection:** awareness reveals the conflicting signals; alignment reconnects measures and decisions to the customer’s purpose; coordination brings the analyst, team lead, account manager, and customer into the decisions they own.

## Check Your Answer

- Did you describe the customer’s purpose as well as the deadline?
- Did you distinguish a warning from a confirmed failure?
- Did you identify which evidence is stale or missing?
- Did you name who can authorize each consequential change?
- Did you choose a response that fits the evidence, rather than either ignoring the signal or stopping everything?
- Did you specify an owner, a checkpoint, and observable closure evidence?

If an answer is missing, revise your response record. These questions support self-review; they are not a numerical score or proof of competence.

## Change One Assumption

Now suppose the account manager produces a written customer agreement moving delivery to Monday afternoon because the planning meeting has moved to Tuesday. The review requirement remains.

What changes in your assessment? What still needs verification? Should the old Friday target remain the measure of success?

??? note "Compare your revised response"

    The authorized agreement changes the delivery baseline. Continuing to judge delivery solely against Friday would misclassify an agreed adaptation as a failure. Record the revised commitment and its source while retaining the history of the change.

    The original scheduling discrepancy is resolved, but delivery and review are still unverified. Check whether the current preparation and review plan can meet Monday afternoon. The green job status remains insufficient evidence of an acceptable report.

## Apply It to Technical Work

If you followed the technical path, reuse the response record for a workflow that automatically publishes the report when its generation job succeeds.

Where should the workflow check review approval and the current authorized commitment? What should happen when either record is missing or stale? What evidence should it record, and who can authorize an exception?

Use [Governance](governance.md), [Observability](observability.md), and [Intervention](intervention.md) to explain the controls you would propose. Describe how you would test them before allowing automatic publication.

??? note "Technical comparison"

    Propose a publication checkpoint that verifies approval for the exact report version and reads the current authorized commitment from its source of record. A successful generation job cannot grant publication authority.

    If required evidence is missing, stale, or belongs to a different version, hold publication and route the exception to the appropriate owner. Record the report version, evidence checked, decision, time, and authority. Test missing approval, an approval for an older version, an authorized date change, and an unavailable source before enabling the workflow.

## Try a Situation of Your Own

Use a small, non-sensitive example: a recurring handoff, a changed assumption, or a dashboard that measures activity rather than the intended outcome. Apply the same response record. If practising with others, compare which facts you relied on and where your proposed interventions differ.

Return to the [reading map](reading-map.md), or compare the shorter [Business Commitment Example](examples/business-commitment-example.md).
