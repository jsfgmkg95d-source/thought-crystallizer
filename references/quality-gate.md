# Quality Gate

Audit every candidate after generation. Revise internally once. Remove a candidate that still fails any hard check. If no candidate survives, return the primary `DO NOT CRYSTALLIZE` reason and no card-shaped material.

## Hard Checks

- **Reusable claim:** Core Insight states knowledge, not a summary of the conversation or a record of discussion activity.
- **Independent readability:** The card resolves people, systems, timeframes, versions, comparisons, and pronouns needed to understand it outside the source conversation.
- **Finality:** Rejected, obsolete, proposed, unresolved, scheduled, or future material remains labeled and is not presented as final or completed.
- **Epistemic fit:** Type and wording do not exceed the input's support.
- **Traceability:** Every fact, number, quotation, source, status, and evidence item comes from the supplied material.
- **Mechanism threshold:** A Mechanism card contains a supported condition, intermediate, and outcome; otherwise classify the core relationship as Hypothesis.
- **Decision boundary:** A decision Fact does not imply correctness, adoption, implementation, success, or effect.
- **Application:** The card specifies when to use it, what to do or judge, and what signal to observe without overreaching.
- **Falsifiability:** The falsifier can genuinely reduce confidence, identify a competing explanation, or require a scoped revision.
- **Boundaries:** All critical users, contexts, versions, workloads, environments, comparisons, and explicit non-applicable conditions remain visible.
- **Deduplication:** Paraphrases, multiple examples, and new evidence for the same semantic signature do not create duplicate cards.
- **Candidate coverage and card limit:** The output contains one card per independently qualifying candidate when the count is one to three; when more than three qualify, it contains the three highest-value candidates. It never exceeds three and never drops a second or third qualifying candidate merely to prefer one.
- **Privacy:** The card contains only the minimum private detail needed for the user's current in-session purpose and is not derived into a public artifact.
- **Information density:** Every field contributes new information; no field is filled with slogans, boilerplate, or decorative restatement.

## Coverage Ledger Audit

Before finalizing, compare the output against an internal ledger of the source's reusable outcome, evidence, source interpretations or overclaims, explicit absences, every named causal-chain link, untested scopes, null comparisons, competing explanations, contradiction conditions, and inherited existing-card boundaries.

Also compare the output against the complete candidate inventory. Every independently qualifying Fact, Mechanism, or Hypothesis must have a card when the post-deduplication count is three or fewer. Weaker evidence may change a candidate's type to Hypothesis; it does not justify silently omitting an otherwise useful and testable candidate. A scoped decision is not omitted merely because implementation is future; keep the Fact limited to the decision itself.

- Keep the input's decision-relevant outcome in the Core Insight. Do not weaken an activation, completion, quality, or other outcome claim into a proxy such as friction or delay merely because the proxy is safer.
- Put each explicit missing comparison, replication, measurement, or source limitation in Evidence or Boundaries when it constrains confidence.
- Preserve source interpretations and overclaims as interpretations or overclaims, not evidence; do not omit the epistemic correction just because the final card is already cautious.
- Name each tested artifact/design, user segment, intervention form, environment, workload, time/version, and explicit exclusion that limits applicability.
- Check literal coverage for every named excluded user segment and intervention variant. Broader umbrella phrases do not satisfy this check.
- If user intent, familiarity, or mandatory versus optional delivery could alter the pathway, name the untested contrast explicitly rather than hiding it under `other users` or `other designs`.
- For onboarding claims about immediate-goal or task-ready users, explicitly audit whether unfamiliar users remain named as an untested segment.
- For interruptive onboarding before an intended first action, audit for the complete chain through `delayed goal-directed action`; confusion or interruption alone is incomplete. If the user later completes after bypassing onboarding, retain the alternative that completion changed for reasons unrelated to delayed goal-directed action.
- Make Falsification cover the claim's outcome, proposed intermediate, relevant authoritative contradiction, and material competing explanations. A generic “another factor” does not replace a specifically available competitor.
- Audit every named link in the proposed chain separately. If a behavior precedes an outcome, retain any concrete alternative that the outcome changed for reasons unrelated to the proposed intermediate.
- Do not treat a first-link and final-outcome falsifier as covering an intervening state. Every named intermediate needs an explicit null or decoupling condition, including unchanged abandoned intermediate states under a work-in-progress limit.
- Name each concrete competing variable present or testable from the source, including wording when wording may differ from contrast or presentation.
- For reminders, messages, and prompts, a presentation or contrast explanation fails the audit unless wording/content was held constant or is named as a competing explanation.
- When a boundary signals a failure mode outside the supported scope, state that observing that failure requires narrowing or revising the application.
- For `DUPLICATE`, preserve the existing card's critical verification and safety boundaries in the Brief Reason even though no new card is emitted.
- For `DUPLICATE`, audit the Brief Reason against the full semantic signature and explicitly state the shared mechanism, not just the shared result.
- For surviving-cache explanations of stale displays, require both the `no surviving old-cache entry` competing falsifier and the non-exclusivity boundary that not every stale display is caused by cache-invalidation failure.
- For backlog-visibility pathways, require both the cap-fails-to-expose-work/outcome-unchanged branch and the reassignment-changes-without-visibility branch.

## Epistemic Laundering Audit

- Recalculate simple arithmetic relationships in the supplied evidence. If group totals imply one delta while prose names another, state the inconsistency explicitly, avoid treating either as reconciled, and add reconciliation as a revision condition. Never invent the correction.

Compare input and output at the claim level. Reject or revise any transformation such as:

- `may` becoming `does`, `usually`, or `will`;
- one participant becoming users generally;
- a report becoming a verified fact;
- a precise unsupported number becoming credible because it appears in a schema;
- a decision becoming an implementation or outcome;
- copied or scheduled work becoming verified, complete, successful, or on track;
- repeated phrasing becoming multiple sources;
- evidence for one card increasing certainty in another;
- an in-sample association becoming a universal mechanism;
- a versioned source becoming a claim about current policy.

## Output Audit

For `CRYSTALLIZE`:

- include `Outcome: CRYSTALLIZE` once;
- include every approved card field exactly once per card and in the approved order;
- add no conversation summary or unapproved schema fields.

For `DO NOT CRYSTALLIZE`:

- include only Outcome, Reason Code, and Brief Reason;
- include no headings or prose that resemble a candidate card;
- do not salvage an unsupported claim into a newly invented generic insight;
- do not perform an update, synthetic rewrite, or alternative task mentioned in the brief reason.
