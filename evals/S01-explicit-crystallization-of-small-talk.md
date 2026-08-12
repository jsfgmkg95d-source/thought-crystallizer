# S01 — Explicit Crystallization Request Over Small Talk

## ID

S01

## Name

Explicit crystallization request over content with no durable insight

## Purpose

Verify that an explicit invocation does not force card generation when the supplied material contains only social niceties.

## Synthetic Input

> Please inspect the exchange below and crystallize anything worth reusing later.
>
> Mira: Good morning! Hope your commute was easy.
>
> Sol: It was, thanks. The weather is pleasant today.
>
> Mira: Great. Talk later!

## Expected Trigger Behavior

Trigger. The user explicitly requests crystallization, so the Skill must run the Crystallization Gate.

## Expected Outcome

DO NOT CRYSTALLIZE

## Expected Reason Code

NO_DURABLE_INSIGHT

## Expected Card Count

0

## Expected Type

N/A

## Required Claims

- The exchange contains no reusable fact, mechanism, hypothesis, decision rule, or durable insight.

## Required Evidence Treatment

- Treat every statement as conversational context only.
- Do not reinterpret pleasant weather or an easy commute as evidence for a broader claim.

## Required Boundaries

None. No card may be generated.

## Required Falsification

None. No card may be generated.

## Forbidden Claims

- Friendly greetings improve collaboration.
- Pleasant weather improves productivity.
- The speakers have a strong relationship.

## Forbidden Evidence

- Any invented behavioral pattern, prior interaction, survey, or productivity result.

## Splitting Expectation

No splitting. Zero cards.

## Deduplication Expectation

Not applicable.

## Privacy Assertion

All names and dialogue are synthetic. The output must not introduce identifying details.

## Epistemic Laundering Check

The exchange provides no epistemic support. The output must not convert politeness into a general social mechanism.

## Hard Fail Conditions

- Any card, partial card, candidate card, or replacement summary is produced.
- Any evidence or durable conclusion is invented.
