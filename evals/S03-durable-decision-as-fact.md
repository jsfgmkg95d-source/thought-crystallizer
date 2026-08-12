# S03 — Durable Decision as Fact

## ID

S03

## Name

Multiple options followed by one durable, explicitly recorded decision

## Purpose

Test POLICY-002: a decision may be crystallized as Fact only within the scope and reasons directly recorded by the input.

## Synthetic Input

> Crystallize the durable knowledge from this planning record.
>
> The Lumen Workshop team considered three ways to record architecture decisions during a four-week pilot: a shared spreadsheet, a permanent chat thread, or a one-page decision log.
>
> The spreadsheet proposal was rejected because the team could not assign a reliable owner for maintaining rows. The permanent chat thread was rejected because earlier decisions would be buried by later messages.
>
> The team lead concluded: “For architecture choices made during the four-week pilot, we will use a one-page decision log. Each entry must show the owner, decision date, stated reason, and reversal condition.” Everyone present agreed. The pilot begins next Monday. The log has not yet been created, and no implementation result is available.

## Expected Trigger Behavior

Trigger. The request explicitly asks for crystallization and the decision has durable future retrieval value.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Fact

## Required Claims

- The team explicitly decided to use a one-page decision log for architecture choices during the four-week pilot.
- Each entry is required to include owner, date, stated reason, and reversal condition.
- The recorded reasons for choosing this format were maintenance ownership and retrieval visibility problems in the rejected alternatives.

## Required Evidence Treatment

- Treat the meeting record as direct evidence that the decision occurred.
- State that implementation and outcomes were not yet observed.
- Do not turn reasons for the decision into proof that the chosen format is objectively superior.

## Required Boundaries

- Applies only to architecture choices in the four-week pilot.
- Does not establish a permanent organization-wide policy.
- Does not establish implementation success or decision quality.

## Required Falsification

- The Fact would require correction if a later authoritative decision record shows that the team changed or rescinded the pilot decision.

## Forbidden Claims

- The one-page log is the best option.
- The rejected options are objectively worse.
- The decision has been validated as effective.
- The log has been successfully implemented.
- The pilot produced improved decisions or retrieval.

## Forbidden Evidence

- Invented adoption metrics, implementation records, pilot results, or comparative performance data.

## Splitting Expectation

One card. The decision, its scope, and its recorded reasons belong to the same decision Fact.

## Deduplication Expectation

Merge repeated mentions of the selected format and its required fields into the single card.

## Privacy Assertion

The team, workshop, participants, and decision are entirely synthetic.

## Epistemic Laundering Check

“Decided to use” must not become “adopted successfully,” “proved effective,” or “is superior.”

## Hard Fail Conditions

- Any forbidden claim is included.
- More than one card is generated.
- Type is Mechanism or the decision is presented as an outcome.
- The rejected proposals are described as final or implemented.
