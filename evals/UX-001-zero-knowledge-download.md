# UX-001 — Zero-Knowledge Download

## Status

Required V0.1 release UX gate.

This gate supplements the twenty frozen `evals/S*.md` model-behavior Golden
Evals. It does not modify, replace, renumber, or expand that frozen suite.

## Product Principle

A first-time repository visitor who does not know what Agent Skills, Codex, Git,
or `SKILL.md` are must identify the correct download within ten seconds.

Thought Crystallizer is a knowledge-crystallization method for AI conversations.
Native Agent Skill packaging is one distribution format, not the product's
definition.

## Synthetic Test Persona

Lin uses Doubao in an ordinary chat window. Lin has never used Git, Codex,
plugins, Agent Skills, or a command line. Lin opens the Chinese README for the
first time.

This persona is synthetic and created from scratch.

## Test Procedure

1. Open the rendered Chinese README at the top of the page.
2. Do not scroll past the first download-routing section.
3. Allow the tester no more than ten seconds to scan the page.
4. Ask: “You normally chat in Doubao. Which file should you download?”
5. Repeat with the English README and an English-speaking ordinary-chat user.
6. Confirm that a user whose tool explicitly supports Agent Skills can also
   identify the Native Skill package without confusing it with Chat Edition.

## Required Result

- The Chinese ordinary-chat answer is exactly
  `Thought-Crystallizer-Chat-ZH.md`.
- The English ordinary-chat answer is exactly
  `Thought-Crystallizer-Chat-EN.md`.
- The Agent Skills answer is exactly
  `Thought-Crystallizer-Skill-v0.1.0.zip` for V0.1.
- The ordinary-chat route is visibly described as the default for most users.
- The user can identify the route before reading project philosophy,
  architecture, installation internals, or Agent Skills explanations.
- The first screen states that Chat Edition requires no Codex, Git,
  programming, or plugin installation.

## Release Asset Contract

V0.1 release assets use only these public filenames:

```text
Thought-Crystallizer-Chat-ZH.md
Thought-Crystallizer-Chat-EN.md
Thought-Crystallizer-Skill-v0.1.0.zip
```

The Chinese release page must visibly state:

> ⭐ 90%的用户请下载：Thought-Crystallizer-Chat-ZH.md

Do not replace these names with internal or build-oriented names such as
`core.zip`, `portable-runtime.md`, `agent-package.zip`, or `dist-final-v2.zip`.

## Hard Fails

- The tester must scroll past philosophy, architecture, or technical setup to
  find the download choice.
- The tester must understand Agent Skills, Codex, Git, or repository structure
  before choosing.
- Two or more files appear equally recommended to an ordinary-chat user.
- The visible filename differs from the actual release asset filename.
- The ordinary-chat path requires uploading multiple repository files.
- The README leads an ordinary-chat user to the Native Skill package.
- The Chinese release page omits the explicit 90% recommendation.
- A release uses an internal, ambiguous, or version-suffix filename for either
  Chat Edition file.

## Maintainer Check

Before every V0.1 release, verify rendered README placement, link targets,
literal filenames, and release assets. Record pass or fail independently from
the model-behavior Golden Eval score.
