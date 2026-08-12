# Classification and Crystal Schema

## Classification Rules

### Fact

Use `Fact` for a claim directly supported by the supplied record, checkable material, or valid source-bounded derivation.

- Preserve the source version, locator, scope, and currentness limit.
- Treat an explicit durable decision as Fact only for the decision's occurrence, content, explicit scope, and recorded reasons.
- Do not infer that a decision was correct, superior, implemented, successful, or effective.
- Do not represent progress, intent, scheduling, copying, or booking as verification, completion, success, or result.

### Mechanism

Use `Mechanism` only when the input supports the complete chain:

`Condition -> Intermediate Mechanism -> Outcome`

Qualifying support may include repeated observations with intermediate evidence, a controlled comparison, traceable system behavior, or multiple mutually supporting observations. Co-occurrence, one anecdote, a confident explanation, or detail without an intermediate does not qualify.

Preserve every tested condition and null comparison that limits the mechanism. Do not claim statistical significance, universality, optimality, production validity, or downstream effects unless supplied.

### Hypothesis

Use `Hypothesis` for a worthwhile, testable factual or causal claim that has a genuine supplied basis but insufficient support.

- State the limited observation, missing comparison, conflict, or alternative explanation.
- Use modal language such as `may` when the input only supports possibility.
- Do not generalize one observation to a population.
- If the core causal claim is unverified, prefer `Hypothesis` even when the proposed content describes a mechanism.
- Preserve the actual decision-relevant outcome proposed by the input as a bounded hypothesis. Do not replace it with an easier-to-support proxy outcome. A proxy may appear as the proposed intermediate, not as a substitute for the core claim.

### Mixed

Use `Mixed` only when a confirmed component and an unconfirmed explanatory component cannot be separated without destroying the insight's value. Mark the confirmed and unconfirmed parts explicitly.

Prefer separate cards when the components have independent claims, applications, falsifiers, and boundaries. Otherwise, when the reusable core is the unconfirmed relationship, use `Hypothesis`. Keep `Mixed` rare.

## V0.1 Crystal Candidate Schema

Use every field exactly once and in this order:

```markdown
# Title

## Core Insight

## Type
Fact / Mechanism / Hypothesis / Mixed

## Why It Matters

## Evidence

## Mechanism

## Application

## Falsification

## Boundaries

## Source
```

## Field Rules

### Title

Name the insight itself. Do not use process titles such as “Summary of the discussion.”

### Core Insight

State the complete reusable claim in one to three sentences. Resolve pronouns and context-dependent references. Preserve modality, quantities, status, and critical conditions.

### Type

Use exactly one of `Fact`, `Mechanism`, `Hypothesis`, or `Mixed` under the rules above.

### Why It Matters

State which future judgment, explanation, or action this insight can improve. Do not add an unsupported benefit.

### Evidence

List only supplied support. Distinguish direct records, traceable source statements, observations, opinions, reasoning, and missing evidence. Keep evidence attached to its own card; evidence strength must not leak across candidates.

When a teammate, narrator, or source says that an anecdote `proves`, `shows`, or establishes a broader causal or population claim, identify that statement as an interpretation or overclaim rather than additional evidence. Do not silently omit it, because that can hide the exact epistemic correction the card must preserve.

Repeated wording is not repeated evidence. Multiple examples supporting the same variable chain are evidence within one card, not separate crystals.

### Mechanism

For `Mechanism`, state the condition, variables, intermediate, and outcome. For `Hypothesis`, label the proposed chain as unconfirmed. For a purely descriptive Fact, write `Not applicable: this card records a descriptive fact.`

Preserve every materially named link in the proposed chain. If the source distinguishes interruption or confusion from delayed goal-directed action and then from activation or completion, do not collapse the middle outcome into a nearby proxy. State which links are observed, inferred, or unmeasured.

Do not fill this field with a paraphrase of the Core Insight.

### Application

Use this structure:

- `When:` the bounded situation in which to recall the card;
- `Do:` the action or judgment it supports;
- `Observe:` the signal to monitor.

Do not prescribe action beyond the evidence or boundaries.

### Falsification

Name an observable result, competing explanation, authoritative superseding record, or revision condition that would weaken, overturn, or narrow the claim. Do not merely negate the conclusion.

- For a source-bounded operational Fact, cover both an authoritative source change and contradictory observed behavior when either could invalidate the card.
- For a Mechanism or Hypothesis, test both the proposed intermediate and the stated outcome. If either changes without the other, require revision of the pathway.
- For a multi-link pathway, give every named intermediate its own null or decoupling test. If a limit is proposed to change pull behavior, abandoned intermediate states, and final handoffs, explicitly test the possibility that abandoned intermediate states do not decline despite the limit; testing only the first and final links is incomplete.
- Convert boundary-relevant failure risks into revision conditions. If applying the insight outside a separable category could create consistency, quality, safety, or coupling failures, state that such failures require narrowing the application.
- Preserve competing explanations supplied or exposed by the comparison design, including wording, participant differences, workload, environment, or another changed variable. Do not replace one required competitor with a generic catch-all.
- When the source identifies or leaves testable a concrete alternative feature, such as wording rather than presentation, name that feature verbatim in Falsification. `Another factor` or `other uncontrolled conditions` is insufficient.
- For reminder, message, or prompt variants whose outcome is attributed to contrast or another presentation feature, check whether wording and content were held constant. If the source does not explicitly establish that control, name **wording or content rather than contrast/presentation** as a competing explanation in Falsification.
- When a behavior such as skipping, dismissing, or bypassing precedes completion, test the source's named causal intermediate and explicitly retain the alternative that completion changed for reasons unrelated to that intermediate. Merely testing whether the behavior and final outcome correlate is insufficient.
- For visibility-and-reassignment mechanisms, test both required branches: whether a comparable cap leaves hidden work and the age/backlog outcome unchanged, and whether reassignment changes without queue visibility changing, which requires a competing mechanism.

### Boundaries

State the applicable objects or users, context, time or version, tested assumptions, unknowns, and explicit exclusions. Preserve null conditions and non-applicable segments. Do not guess unknown boundaries.

Name explicitly supplied exclusions rather than collapsing them into a broader phrase. Preserve the tested artifact or design variants, user familiarity or intent, optional versus required interventions, environment, workload, and version whenever the input distinguishes them.

Enumerate distinct excluded populations and intervention variants individually. Do not treat `other users` as preserving a named segment such as unfamiliar users, or `other designs` as preserving optional versus required behavior.

When a proposed effect depends on a person's immediate goal, prior familiarity, or an intervention being mandatory, explicitly separate:

- users with the immediate goal from unfamiliar users or users without that goal; and
- required interventions from optional or skippable variants.

Do not transfer a one-segment observation across these contrasts unless the input supplies evidence for them.

For onboarding interventions specifically, always distinguish task-ready or immediate-goal users from unfamiliar users who may need orientation. A result for the first group does not establish the effect for unfamiliar users. Name `unfamiliar users` explicitly in Boundaries when they were not tested.

For an interruptive onboarding sequence placed before a task-ready user's intended first action, name the candidate intermediate as **delayed goal-directed action** when the source shows the user trying to bypass the sequence to proceed. Confusion or interruption may precede that delay, but does not replace it. If completion occurs after skipping or bypassing, Falsification must also test whether completion changed for reasons unrelated to delayed goal-directed action.

For a stale-display mechanism attributed to a surviving old cache entry, include both safeguards: Falsification must require a competing explanation if the display remains stale when no old-cache entry survives, and Boundaries must state that the evidence does not establish that every stale display is caused by cache-invalidation failure.

### Source

Use only a locator supplied in the task, such as a document title, version, section, page, message label, or named synthetic test. If no stable locator exists, state that the source is the current user-supplied material and has not been independently verified.

Do not invent a URL, citation, author, date, study, dashboard, or current-version claim.

## Multi-Card Rules

- Prefer one card when the material forms one semantic unit. Do not use this preference to discard a second or third independently qualifying candidate.
- Split only when every candidate has an independent Core Insight, Application, Falsification, and Boundaries.
- Require that removing one card would not damage another card's completeness.
- Keep a fact, its evidence, its mechanism, and its examples together when they form one insight.
- When one to three candidates independently qualify, return each qualifying candidate. When more than three qualify, retain only the three with the highest long-term reuse value. Do not mention discarded slogans or low-value candidates as extra cards.
