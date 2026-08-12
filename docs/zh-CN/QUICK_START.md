# Thought Crystallizer 快速开始

[English](../QUICK_START.md) | 简体中文

## 普通 AI 聊天（适合绝大多数用户）

下载并上传
[`Thought-Crystallizer-Chat-ZH.md`](../../portable/Thought-Crystallizer-Chat-ZH.md)，
然后告诉 AI：

```text
加载 Thought Crystallizer。以后我说“结晶”时，按照其中规则执行。
```

不知道选哪个？就用这个。

## 原生 Agent Skill

把仓库安装为 Skill，新建任务，然后输入：

```text
使用 $thought-crystallizer 结晶这段对话中值得长期复用的洞见。

<粘贴对话>
```

实际运行入口只有英文规范版 [`SKILL.md`](../../SKILL.md)。

只有产品明确支持 Agent Skills 或 `SKILL.md` 包时，才使用 Native Skill 路线。

## 如何理解结果

- `Outcome: CRYSTALLIZE`：材料通过门禁，产出一至三张有证据边界的结晶候选卡。
- `Outcome: DO NOT CRYSTALLIZE`：Skill 已运行，但材料未通过某个门禁。
- 仅要求总结或翻译时，不应触发 Thought Crystallizer，也不应输出上述结果。

不要把私人材料粘贴到公开 Issue，也不要要求 Skill 把私人材料改造成公开示例。公开产物必须完全从零合成。
