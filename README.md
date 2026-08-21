# karpathy-guidelines-openai

面向 OpenAI/Codex coding agents 的可复用 skill。它基于 [Karpathy-Inspired Claude Code Guidelines](https://github.com/multica-ai/andrej-karpathy-skills)，并按 OpenAI Skills 格式整理，帮助 agent 在软件开发任务中保持范围清晰、实现简单、修改克制，并以验证结果支撑结论。

## 核心原则

- 先明确目标、范围、约束和成功标准，再开始修改。
- 优先采用满足当前需求的最简单方案。
- 只做与请求直接相关的局部修改，保留无关代码和用户已有改动。
- 将任务转化为可观察的验证项，区分静态检查、测试、运行时和硬件验证。
- 对假设、证据和未验证部分保持透明，不虚构工具结果或完成状态。

## 安装

将整个目录复制到 Codex 的 skills 目录：

```text
<CODEX_HOME>/skills/karpathy-guidelines-openai/
```

如果未设置 `CODEX_HOME`，可使用默认目录：

```text
~/.codex/skills/karpathy-guidelines-openai/
```

目录至少包含：

```text
karpathy-guidelines-openai/
├── SKILL.md
└── agents/
    └── openai.yaml
```

## 使用

可显式调用：

```text
Use $karpathy-guidelines-openai to keep this coding task minimal, scoped, and verified.
```

该 skill 默认允许隐式调用；当任务涉及软件编写、评审、调试、重构或计划时，也可以根据 description 自动匹配。

## 适用边界

本项目只针对 OpenAI/Codex Skills 设计。skill 提供工作方法和验证约束，不覆盖项目自身的 `AGENTS.md`、用户请求或其他更高优先级指令。

## 来源与许可

- 来源：[andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills)
- 许可：MIT
