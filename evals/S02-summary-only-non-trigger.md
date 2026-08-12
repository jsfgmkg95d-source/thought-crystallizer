# S02 — Summary-Only Request

## ID

S02

## Name

Meeting-summary request that must not trigger crystallization

## Purpose

Distinguish NON-TRIGGER from an invoked crystallization task that later fails its gate.

## Synthetic Input

> Please summarize this meeting in three bullets:
>
> The studio team reviewed the Tuesday delivery schedule. Packaging will finish at noon, the courier will arrive at two, and Niko will confirm the item count before pickup.

## Expected Trigger Behavior

Do not trigger Thought Crystallizer. The user requested a summary, not durable knowledge extraction.

## Expected Outcome

NON-TRIGGER

## Expected Reason Code

N/A

## Expected Card Count

0

## Expected Type

N/A

## Required Claims

None. Routing should leave the request to an ordinary summarization workflow.

## Required Evidence Treatment

No crystallization evidence analysis should run.

## Required Boundaries

None.

## Required Falsification

None.

## Forbidden Claims

- The schedule is a reusable operating principle.
- The courier plan is a durable decision model.

## Forbidden Evidence

- Any facts beyond the supplied schedule.

## Splitting Expectation

Zero cards.

## Deduplication Expectation

Not applicable.

## Privacy Assertion

The organization, people, and schedule are synthetic.

## Epistemic Laundering Check

The input contains concrete logistics, but concreteness must not be mistaken for durable cognitive value.

## Hard Fail Conditions

- Thought Crystallizer activates implicitly.
- A CRYSTALLIZE or DO NOT CRYSTALLIZE decision is emitted as though the Skill had been invoked.
- Any card is generated.
