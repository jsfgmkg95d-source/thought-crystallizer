# S14 — Semantic Duplicate of an Existing Card

## ID

S14

## Name

New wording and evidence for an already represented semantic signature

## Purpose

Verify that semantic duplication results in no new card even when the new discussion sounds polished and includes a fresh example.

## Synthetic Input

> Review the new discussion against the existing crystal and create a new crystal only if the insight is independently new.
>
> Existing crystal:
>
> **Core Insight:** A work handoff is less likely to produce duplicate effort when it names the current state, the last verified action, and the next owner.
>
> **Mechanism:** These three fields reduce ambiguity about what is complete and who acts next.
>
> **Application:** Use the three-field handoff when work changes owners.
>
> **Boundary:** This does not guarantee the handoff is correct; the stated current state must still be verified.
>
> New discussion:
>
> In a synthetic catalog exercise, two editors repeated the same correction after a handoff message said only “please continue.” In a replay, the message listed the current state, the last checked item, and the next editor. No correction was repeated. The group concluded that explicit state, last action, and next owner reduce duplicate handoff work.

## Expected Trigger Behavior

Trigger. The user explicitly asks for crystallization review with an existing comparison card.

## Expected Outcome

DO NOT CRYSTALLIZE

## Expected Reason Code

DUPLICATE

## Expected Card Count

0

## Expected Type

N/A

## Required Claims

- The new discussion has the same core variables, direction, application, and mechanism as the existing crystal.
- The new exercise is additional evidence, not an independently new insight.

## Required Evidence Treatment

- Recognize the synthetic catalog exercise as possible update evidence for the existing card.
- Do not create a new card merely because the example or wording is new.

## Required Boundaries

None for a new card. The existing card’s verification boundary must not be erased in the brief reason.

## Required Falsification

None for a new card.

## Forbidden Claims

- The new discussion introduces a distinct handoff mechanism.
- The replay proves the handoff format always prevents duplicate work.

## Forbidden Evidence

- Additional handoffs, measured rates, or claims that the existing card has been globally validated.

## Splitting Expectation

Zero new cards.

## Deduplication Expectation

Exact semantic duplicate: suggest updating the existing card rather than creating another, but output only the allowed DO NOT CRYSTALLIZE fields.

## Privacy Assertion

The existing crystal, catalog exercise, editors, and results are synthetic.

## Epistemic Laundering Check

A fresh example must not make an old bounded mechanism universal or justify a duplicate crystal.

## Hard Fail Conditions

- Any new, partial, or “for reference” card is produced.
- More than zero cards are produced.
- The duplicate is treated as independently new.
- The existing boundary is silently removed.
