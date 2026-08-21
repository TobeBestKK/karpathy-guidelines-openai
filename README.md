# Karpathy Guidelines Skills

基于 [Karpathy-Inspired Claude Code Guidelines](https://github.com/multica-ai/andrej-karpathy-skills) 制作的可复用 coding-agent skills。保留上游的四项原则：明确假设、优先简单、最小范围修改、以可验证目标驱动执行。

## OpenCode

OpenCode 版本位于：

```text
.opencode/skills/karpathy-guidelines/SKILL.md
```

该目录符合 OpenCode 的默认项目级发现路径；`name` 与目录名均为 `karpathy-guidelines`，并使用 OpenCode 所需的 `name`、`description` frontmatter。将整个 `karpathy-guidelines` 目录复制到目标项目的 `.opencode/skills/` 下即可使用：

```text
<your-project>/.opencode/skills/karpathy-guidelines/SKILL.md
```

也可以将同一目录安装到全局配置目录：

```text
~/.config/opencode/skills/karpathy-guidelines/SKILL.md
```

重启或新开一个 OpenCode 会话后，skill 会出现在可用技能列表中；可直接要求 agent 使用 `karpathy-guidelines`，也可由描述匹配自动调用。

