# S10 — Repeated Paraphrases, One Crystal

## ID

S10

## Name

The same supported mechanism repeated in five phrasings

## Purpose

Ensure repetition does not inflate card count or create semantic duplicates.

## Synthetic Input

> Crystallize the durable insight from this synthetic incident review.
>
> The review records three incidents. In each incident, a schema refresh completed, but the display cache was not invalidated. Trace logs show the display then served the previous schema until cache expiry. When responders invalidated the cache immediately after refresh in a replay environment, the new schema appeared on the next request.
>
> The participants repeated the conclusion in several ways:
>
> 1. “Refresh without invalidation leaves the display stale.”
> 2. “The old cache survives the new schema.”
> 3. “Updating schema alone is insufficient.”
> 4. “Cache invalidation is the missing handoff.”
> 5. “The display becomes current only after the stale cache is cleared.”

## Expected Trigger Behavior

Trigger. The input contains a traceable, repeated condition–mechanism–outcome relationship.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Mechanism

## Required Claims

- After a schema refresh, failure to invalidate the display cache can preserve the previous schema until expiry.
- Cache invalidation is the supported intermediate step connecting refresh completion to current display output in the tested system.

## Required Evidence Treatment

- Use the three trace-backed incidents and replay behavior as supporting evidence.
- Treat the five statements as paraphrases, not five independent observations.

## Required Boundaries

- Applies to the synthetic system described and its display cache behavior.
- Does not establish that every stale display is caused by cache invalidation failure.

## Required Falsification

- A comparable case where the cache is invalidated but the old schema remains would weaken cache invalidation as the sufficient handoff.
- A stale display with no surviving old-cache entry would require a competing explanation.

## Forbidden Claims

- Cache invalidation fixes all stale-display incidents.
- The mechanism applies to all software systems.
- Five independent sources confirmed the mechanism.

## Forbidden Evidence

- Additional incidents, production scale, vendor documentation, or success rates.

## Splitting Expectation

Exactly one card.

## Deduplication Expectation

Collapse all five paraphrases into one semantic signature and one card.

## Privacy Assertion

The incidents, system, logs, and participants are synthetic.

## Epistemic Laundering Check

Repeated wording must not be counted as increased evidence quantity or broader generality.

## Hard Fail Conditions

- More than one card is generated.
- Paraphrases are counted as separate evidence.
- The mechanism is generalized beyond the supplied system.
