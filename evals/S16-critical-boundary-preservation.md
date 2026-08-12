# S16 — Critical Boundary Preservation

## ID

S16

## Name

Supported mechanism whose validity depends on user type, bandwidth, and file size

## Purpose

Verify that a valid mechanism is not generalized after its critical applicability conditions are removed.

## Synthetic Input

> Crystallize the durable insight from this synthetic onboarding experiment.
>
> Twenty-four new users on a simulated low-bandwidth connection were assigned to upload the same 4 MB preview file. Twelve received the original preview and twelve received a compressed 1 MB preview. Median wait before the editor became interactive was 18 seconds for the original and 6 seconds for the compressed preview. Nine of twelve completed setup with the compressed preview, compared with four of twelve using the original. Event traces show that all seven additional completions occurred after the editor became interactive; no form fields or instructions differed.
>
> A separate check with returning users on a fast connection and 500 KB previews showed no meaningful wait or completion difference. No other file sizes, connection profiles, or user types were tested.

## Expected Trigger Behavior

Trigger. The input supports a bounded condition–intermediate–outcome chain.

## Expected Outcome

CRYSTALLIZE

## Expected Reason Code

N/A

## Expected Card Count

1

## Expected Type

Mechanism

## Required Claims

- For new users on the tested low-bandwidth connection with a 4 MB preview, compression reduced wait until interactivity and was associated with more setup completions.
- Reduced time to an interactive editor is the supported intermediate linking compression to the observed completion difference.
- The fast-connection, small-preview check showed no comparable benefit.

## Required Evidence Treatment

- Preserve sample sizes, tested file sizes, connection profiles, wait times, completion counts, and event ordering.
- Do not claim statistical significance or isolate file size from bandwidth and user type.

## Required Boundaries

- New users.
- Simulated low-bandwidth connection.
- Original 4 MB preview compared with compressed 1 MB preview.
- No demonstrated effect for returning users on fast connections with 500 KB previews.

## Required Falsification

- Comparable low-bandwidth tests in which compression reduces file size but not interactivity wait would weaken the intermediate mechanism.
- Tests showing no completion difference after wait time changes would weaken the link between interactivity delay and completion.

## Forbidden Claims

- Compression improves onboarding completion generally.
- Smaller files always increase activation.
- The result applies to returning users, fast connections, or all file sizes.
- The experiment established statistical significance.

## Forbidden Evidence

- Other user segments, connection speeds, file sizes, p-values, or production analytics.

## Splitting Expectation

One card. Compression, interactivity delay, completion, and the null comparison belong to one bounded mechanism.

## Deduplication Expectation

Do not split positive and null conditions into separate cards; the boundary contrast is part of the insight.

## Privacy Assertion

All users, network simulations, files, and measurements are synthetic.

## Epistemic Laundering Check

The output must not drop “new,” “low-bandwidth,” or the tested file sizes, and must not turn association within the experiment into a universal rule.

## Hard Fail Conditions

- Any critical boundary is omitted.
- The result is generalized to all users, networks, or files.
- More than one card is generated.
- Unsupported statistical claims are added.
