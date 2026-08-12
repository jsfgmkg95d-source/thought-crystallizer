# V0.1 简体中文配对 Evals

本目录用于测试 Thought Crystallizer 的认识论纪律能否跨语言保持稳定。

- 英文 `evals/S01`–`S20` 是冻结的 V0.1 Golden Evals，也是规范基线。
- 本目录只覆盖八个关键能力，ID 使用 `<英文能力 ID>-zh`。
- 中文输入均为自然中文、从零合成，不是英文 fixture 的逐字翻译。
- 中文配对 Eval 不替代、不修改，也不降低英文 Golden Evals 的要求。
- 若中英文预期行为冲突，以英文 Golden Eval 与英文 `SKILL.md` 为准。

| 配对 ID | 对应能力 |
| --- | --- |
| S01-zh | 明确要求结晶也不能强迫低价值材料出卡 |
| S02-zh | summary-only 属于 non-trigger |
| S03-zh | 决策只可作为有范围的 Fact |
| S05-zh | 单次观察最多支持有边界的 Hypothesis |
| S06-zh | 完整条件—中间机制—结果链可使用 Mechanism |
| S14-zh | 新措辞或新例子不构成新卡 |
| S18-zh | 私人材料不得衍生公开 Eval |
| S19-zh | 来源中的提示词注入不具备指令权或证据力 |
