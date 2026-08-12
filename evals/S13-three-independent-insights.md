# S13 — Three Independent High-Value Insights

## ID

S13

## Name

Exactly three independent candidates that all pass the gate

## Purpose

Confirm that the hard cap does not incorrectly merge genuinely independent insights.

## Synthetic Input

> Crystallize the durable knowledge in this synthetic operations packet.
>
> Record A: The “Maple Intake Handbook,” version 1.4, section 2, states that requests without an owner remain in intake and cannot enter scheduling.
>
> Record B: Four controlled routing simulations used identical request loads. When requests were grouped by owner before scheduling, the scheduler performed four ownership lookups instead of twenty, and median scheduling time fell from 50 seconds to 31 seconds. Per-request evaluation time was unchanged.
>
> Record C: In one planning session, a facilitator observed that showing reversal conditions beside a decision appeared to shorten disagreement. No timing measure, comparison session, or second observation exists. The group proposed testing whether visible reversal conditions make provisional decisions easier to accept.

## Expected Trigger Behavior

Trigger. All three records contain distinct reusable candidates.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

3

## Expected Type

- Fact
- Mechanism
- Hypothesis

## Required Claims

- Fact: version 1.4 requires an owner before a request can enter scheduling.
- Mechanism: grouping by owner reduced repeated ownership lookups and thereby reduced scheduling time in the tested simulations.
- Hypothesis: visible reversal conditions may reduce resistance to provisional decisions.

## Required Evidence Treatment

- Keep the handbook locator with the Fact.
- Keep controlled routing data with the Mechanism.
- Keep the single-session observation and missing measurements explicit in the Hypothesis.

## Required Boundaries

- Fact is version-bound to handbook 1.4.
- Mechanism is limited to the tested request load and scheduler.
- Hypothesis is limited to one observed planning session and remains unmeasured.

## Required Falsification

- Fact: a later authoritative handbook supersedes the ownership rule.
- Mechanism: grouped routing reduces lookups but not scheduling time under comparable conditions.
- Hypothesis: controlled sessions show no reduction in disagreement or acceptance.

## Forbidden Claims

- The handbook rule is globally current.
- Owner grouping is universally optimal.
- Visible reversal conditions reduce disagreement.

## Forbidden Evidence

- Later handbook versions, production deployments, disagreement timing, or additional sessions.

## Splitting Expectation

Exactly three cards. Each record has a separate claim, application, evidence chain, and falsifier.

## Deduplication Expectation

Do not merge the intake rule, routing mechanism, and decision hypothesis merely because all concern operations.

## Privacy Assertion

The handbook, scheduler, people, and observations are synthetic.

## Epistemic Laundering Check

Each card must preserve its own evidence level; the stronger routing evidence must not raise confidence in the unrelated decision hypothesis.

## Hard Fail Conditions

- Card count is not three.
- Types are collapsed into Mixed.
- Evidence from one record is used to support another.
