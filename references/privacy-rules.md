# Privacy Rules

## In-Session Private Input

Process private material only when the user supplies it for their own current in-session crystallization task and the requested output remains private to that task.

- Use only the minimum detail needed to express the insight.
- Avoid copying long passages, identity details, medical details, financial details, relationship details, unpublished creative text, or other sensitive context into a card.
- Do not access private knowledge bases, diaries, chat archives, other repositories, or unrelated folders.
- Do not save, index, synchronize, publish, or ingest the result.
- Do not imply that the Skill controls the host application's retention, storage, or data policy.

## Public Artifacts

Require public examples, fixtures, evals, prompts, screenshots, documentation cases, and repository content to be synthetic and created from scratch.

Do not use real private material through:

- anonymization;
- redaction;
- abstraction;
- paraphrase;
- fictionalized names;
- preservation of its emotional, event, relationship, medical, financial, identity, or narrative structure.

When a user requests public reuse of asserted private material:

1. Do not open or inspect the private attachment or source.
2. Do not quote, summarize, classify, diagnose, or infer an insight from it.
3. Return `DO NOT CRYSTALLIZE` with `PRIVACY_RISK`.
4. State briefly that a separately created, from-scratch synthetic scenario is the safe route, without generating a substitute card or fixture in the same output.

## Public Synthetic Construction

When separately authorized to create a synthetic public artifact:

- invent the scenario from scratch;
- use fictional people, organizations, measurements, sources, and events;
- do not preserve the distinctive structure of private source material;
- label the artifact synthetic;
- never later present it as a real case study.

## Source Minimization

In private in-session cards, use the smallest truthful locator needed, such as `current user-supplied conversation` or a supplied document label. Do not reproduce sensitive passages merely to make the source field look complete.

In public artifacts, cite only the synthetic fixture or public source actually supplied. Never fabricate a public citation to replace a private source.
