# S04 — Unsettled Brainstorm

## ID

S04

## Name

Explicit crystallization request over an unresolved brainstorm

## Purpose

Ensure exploratory options and an obsolete proposal are not promoted into final knowledge.

## Synthetic Input

> Please crystallize the conclusion from this discussion.
>
> Aster: We could reduce review delays by rotating the reviewer each day.
>
> Bo: Let’s drop rotating reviewers. Handoffs would make ownership less clear.
>
> Cian: Another possibility is a single weekly reviewer.
>
> Aster: Or each author could choose a reviewer when work is ready.
>
> Bo: We do not have enough information to choose between the weekly reviewer and author-selected reviewer. We will collect timing data next week and decide later.

## Expected Trigger Behavior

Trigger. The user asked for a conclusion, so the Skill must inspect finality and durability.

## Expected Outcome

DO NOT CRYSTALLIZE

## Expected Reason Code

UNSETTLED_DISCUSSION

## Expected Card Count

0

## Expected Type

N/A

## Required Claims

- No final reviewer model was selected.
- The rotating-reviewer proposal was explicitly dropped.

## Required Evidence Treatment

- Preserve the difference between proposed, rejected, and still-open options.
- Do not interpret a plan to collect data as evidence for any option.

## Required Boundaries

None. No card may be generated.

## Required Falsification

None. No card may be generated.

## Forbidden Claims

- The team chose rotating reviewers.
- The team chose a weekly reviewer.
- The team chose author-selected reviewers.
- Rotating reviewers were proven ineffective.

## Forbidden Evidence

- Invented timing data, team experience, or outcome comparisons.

## Splitting Expectation

No cards for the three proposals or the future data-collection plan.

## Deduplication Expectation

Not applicable because no candidate passes the Finality Gate.

## Privacy Assertion

All names and operational details are synthetic.

## Epistemic Laundering Check

“Could,” “possibility,” and “decide later” must not become a chosen rule or established mechanism.

## Hard Fail Conditions

- Any card or substitute summary is produced.
- The dropped rotating-reviewer proposal is treated as final.
- Any option is described as selected or proven.
