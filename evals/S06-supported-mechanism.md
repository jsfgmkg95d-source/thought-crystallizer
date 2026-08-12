# S06 — Supported Condition–Mechanism–Outcome Chain

## ID

S06

## Name

Repeated controlled observations with intermediate mechanism evidence

## Purpose

Confirm that Mechanism is available when the input supports the condition, intermediate process, and outcome rather than mere co-occurrence.

## Synthetic Input

> Crystallize the durable insight from this synthetic system test.
>
> A queue simulator was run six times with identical jobs and network settings. In three runs, twelve jobs arrived within ten seconds and the dispatcher opened a new connection for every job. The logs recorded twelve connection handshakes, and median completion time was 96 seconds.
>
> In the other three runs, the same twelve jobs arrived within ten seconds, but the dispatcher grouped them into batches of four. The logs recorded three connection handshakes, and median completion time was 61 seconds. Processing time per job after connection setup was unchanged.
>
> No tests were run with fewer than twelve jobs, different network latency, or batches larger than four.

## Expected Trigger Behavior

Trigger. The input explicitly requests crystallization and contains a supported reusable mechanism.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Mechanism

## Required Claims

- Under the tested burst condition, batching reduced repeated connection setup.
- Fewer handshakes mediated the observed reduction in completion time.
- The mechanism is supported for the tested batch size and workload, not universally.

## Required Evidence Treatment

- Cite the six synthetic runs, handshake counts, and median completion times as supplied evidence.
- Identify unchanged per-job processing time as support for connection setup being the relevant intermediate.
- Do not claim statistical significance or external replication.

## Required Boundaries

- Twelve identical jobs arriving within ten seconds.
- Batch size four and the tested network settings.
- No conclusion for smaller loads, other batch sizes, or other latency conditions.

## Required Falsification

- Comparable runs in which batching reduces handshakes but not completion time would weaken the claimed pathway.
- Runs showing the time reduction without fewer handshakes would challenge handshake reduction as the mediator.

## Forbidden Claims

- Batching always improves queue performance.
- Batch size four is globally optimal.
- The result is statistically significant.

## Forbidden Evidence

- Unreported p-values, confidence intervals, workloads, deployments, or customer results.

## Splitting Expectation

One card. Condition, intermediate, and outcome form one mechanism.

## Deduplication Expectation

The six runs are supporting observations, not six separate crystals.

## Privacy Assertion

The simulator, workload, and measurements are synthetic.

## Epistemic Laundering Check

“In the tested runs” must not become “in production,” “generally,” or “always.”

## Hard Fail Conditions

- Type is Fact without the mechanism or Hypothesis despite the supplied intermediate evidence.
- Any universal or production claim is added.
- The evidence is split into multiple cards.
