# Thought Crystallizer Quick Start

English | [简体中文](zh-CN/QUICK_START.md)

## Ordinary AI chat (recommended for most people)

Download and upload
[`Thought-Crystallizer-Chat-EN.md`](../portable/Thought-Crystallizer-Chat-EN.md),
then tell the AI:

```text
Load Thought Crystallizer. From now on, when I say "crystallize," follow its rules.
```

Not sure which route to use? Use this one.

## Native Agent Skill

Install the repository as a Skill, start a new task, and ask:

```text
Use $thought-crystallizer to crystallize the durable insight in this conversation.

<paste the conversation>
```

The runtime entry point is the English canonical [`SKILL.md`](../SKILL.md).

Use the Native Skill route only when the product explicitly supports Agent
Skills or `SKILL.md` packages.

## Read the result

- `Outcome: CRYSTALLIZE` means the material yielded one to three reusable,
  evidence-bounded cards.
- `Outcome: DO NOT CRYSTALLIZE` means the Skill ran but the material failed a
  gate.
- A summary-only or translation-only request should not activate the Skill at
  all.

Never paste private material into a public Issue or ask the Skill to turn it
into a public example. Public artifacts must be synthetic and created from
scratch.
