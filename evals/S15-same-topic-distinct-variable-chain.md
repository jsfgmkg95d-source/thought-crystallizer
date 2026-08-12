# S15 — Same Topic, Distinct Variable Chain

## ID

S15

## Name

Coordination insight that is not a semantic duplicate of the supplied card

## Purpose

Ensure deduplication compares variable chains and applications rather than rejecting every insight with the same broad topic.

## Synthetic Input

> Compare the new evidence with the existing crystal and crystallize only an independently new insight.
>
> Existing crystal:
>
> **Core Insight:** Explicit receipt confirmation reduces duplicate handling when a message may not have been seen.
>
> **Mechanism:** A receipt closes uncertainty about whether the next owner received the handoff.
>
> New evidence:
>
> A synthetic service desk ran four matched queue simulations. In the first two, each handler could hold any number of active tickets. The visible queue showed only unassigned tickets, while handlers accumulated eleven and thirteen active tickets; new tickets appeared scarce even though work-in-progress was high. In the matched simulations, each handler could hold at most three active tickets. Excess tickets remained visible in the shared queue, making backlog size visible and prompting reassignment. Median oldest-ticket age fell from 42 minutes to 25 minutes. Receipt confirmations were identical in all four simulations.

## Expected Trigger Behavior

Trigger. The new claim concerns workload visibility and a work-in-progress cap, not receipt uncertainty.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Mechanism

## Required Claims

- In the tested desk, unlimited private work-in-progress hid backlog inside handlers’ active lists.
- A three-ticket cap kept excess demand visible in the shared queue, enabling reassignment and reducing oldest-ticket age.
- This variable chain is distinct from confirmation of handoff receipt.

## Required Evidence Treatment

- Use the matched simulations, active-ticket counts, queue visibility, and oldest-ticket age.
- Note that receipt confirmations were held constant.
- Do not infer service quality or customer outcomes.

## Required Boundaries

- Synthetic service desk, tested loads, and a cap of three active tickets.
- Does not establish that three is optimal or that caps help every workflow.

## Required Falsification

- If a comparable cap leaves hidden work and oldest-ticket age unchanged, the proposed visibility pathway is weakened.
- If reassignment changes without queue visibility changing, a competing mechanism is required.

## Forbidden Claims

- The existing receipt-confirmation crystal explains the result.
- Three tickets is the optimal universal limit.
- Lower ticket age improved service quality.

## Forbidden Evidence

- Customer satisfaction, production data, additional simulations, or optimization studies.

## Splitting Expectation

One new card for the distinct workload-visibility mechanism.

## Deduplication Expectation

Do not reject it as a duplicate merely because both cards concern coordination; the variables, mediator, and intervention differ.

## Privacy Assertion

The service desk, simulations, workloads, and measurements are synthetic.

## Epistemic Laundering Check

Matched simulations support the tested mechanism only; they do not establish a universal WIP limit or downstream quality gain.

## Hard Fail Conditions

- Outcome is DUPLICATE.
- The new mechanism is merged into receipt confirmation.
- The cap is generalized or called optimal.
