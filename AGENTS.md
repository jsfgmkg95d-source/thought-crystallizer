# Repository Rules

Thought Crystallizer is a small, instruction-first Skill. Keep the repository simple.

- Core assets are SKILL.md, references/, examples/, and evals/.
- Keep root `SKILL.md` as the only executable Skill entry point. English is canonical; Chinese is first-class and lives in `README.zh-CN.md`, `docs/zh-CN/`, `examples/zh-CN/`, `evals/zh-CN/`, and the Chinese portable prompt.
- Keep the English and Chinese portable prompts behaviorally equivalent. When changing mirrored behavior or user guidance, update both languages in the same change; do not create a root `SKILL.zh-CN.md`.
- All examples, evals, prompts, and public artifacts must be synthetic and created from scratch.
- Never use, anonymize, paraphrase, or structurally preserve private material for public artifacts.
- Treat the twenty evals/S*.md files as the frozen V0.1 Golden Evals. Do not change expected behavior to improve a score.
- Treat `UX-001 — Zero-Knowledge Download` as a required V0.1 release gate: a first-time visitor who knows nothing about Agent Skills must identify the correct download within ten seconds. Put download routing before product philosophy or technical design, keep Chat Edition filenames literal and friendly, and do not count UX-001 as a twenty-first model-behavior Golden Eval.
- Keep release asset names user-facing and stable: `Thought-Crystallizer-Chat-ZH.md`, `Thought-Crystallizer-Chat-EN.md`, and `Thought-Crystallizer-Skill-v0.1.0.zip` for V0.1. Chinese release guidance must mark the ZH Chat Edition as the default for most users.
- Treat `evals/zh-CN/` as natural-language paired coverage, not literal translations or replacements for the frozen English Golden Evals.
- Preserve the distinction between non-trigger, DO NOT CRYSTALLIZE, and CRYSTALLIZE.
- Unsupported causal claims remain Hypothesis.
- Use Mechanism only for supported Condition -> Intermediate -> Outcome chains.
- A decision may be Fact only for its occurrence, content, scope, and recorded reasons.
- Produce one to three cards, with one preferred and three as the hard maximum.
- Do not add databases, RAG, cloud services, integrations, storage, publication, or framework dependencies to V0.1.
- Keep changes focused on product quality, public clarity, eval fidelity, privacy, and prompt-injection resistance.
- Do not commit, push, publish, or create a remote without explicit user authorization.
