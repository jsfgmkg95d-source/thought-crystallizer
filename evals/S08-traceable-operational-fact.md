# S08 — Traceable Operational Fact

## ID

S08

## Name

Durable operational constraint stated in a supplied synthetic manual

## Purpose

Verify that a source-bounded, reusable fact can pass when its evidence and scope are explicit.

## Synthetic Input

> Extract any durable crystal from this synthetic manual excerpt.
>
> Source: “Oriole Workshop Runbook,” version 2.1, section 4.3, page 18.
>
> “During the first business day of each month, the archive index is read-only from 09:00 to 11:00 workshop time while integrity checks run. Import requests submitted during that window remain queued until the index returns to writable mode. This restriction applies only to the archive index; live drafting remains available.”

## Expected Trigger Behavior

Trigger. The user requests crystallization and provides a durable, traceable operating constraint.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Fact

## Required Claims

- The archive index is read-only from 09:00 to 11:00 workshop time on the first business day of each month.
- Import requests queue during that window.
- Live drafting remains available.

## Required Evidence Treatment

- Attribute every claim to the supplied runbook excerpt.
- Preserve the version, section, and page locator.
- Do not claim currentness beyond version 2.1.

## Required Boundaries

- Applies only to the archive index.
- Applies only during the stated monthly window.
- Does not imply that live drafting or all services are unavailable.

## Required Falsification

- A later authoritative runbook version or observed system behavior contradicting the stated window would require correction or retirement of the Fact.

## Forbidden Claims

- The entire workshop is offline.
- Imports fail or are deleted.
- Version 2.1 is the latest current policy.

## Forbidden Evidence

- Invented system logs, later versions, incident reports, or author names.

## Splitting Expectation

One card. The read-only window, queued imports, and unaffected drafting define one bounded operational constraint.

## Deduplication Expectation

Do not create separate cards for the window and the queue behavior.

## Privacy Assertion

The workshop, manual, schedule, and system are synthetic.

## Epistemic Laundering Check

The supplied source supports only the exact versioned rule; it does not support claims about present-day policy or actual uptime.

## Hard Fail Conditions

- Scope expands from archive index to the whole system.
- The source locator is altered or supplemented.
- More than one card is generated.
