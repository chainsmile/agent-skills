# Agent Skills

一组可单独安装的 Agent Skills，适用于 Codex 和 Claude Code。

| Skill | 用途 |
| --- | --- |
| [deepen-task](skills/deepen-task/SKILL.md) | 深化现有任务提示词，在原范围内补足专业判断、原始证据、具体方法和可独立核验的验收条件。 |

## 个人级安装

先克隆仓库，再复制需要的 Skill 目录。已有同名 Skill 时，请先检查本地内容。

```sh
git clone https://github.com/chainsmile/agent-skills.git
cd agent-skills
```

**Codex**

```sh
mkdir -p ~/.agents/skills
cp -Ri skills/deepen-task ~/.agents/skills/
```

**Claude Code**

```sh
mkdir -p ~/.claude/skills
cp -Ri skills/deepen-task ~/.claude/skills/
```

## 使用

在 Codex 输入 `$deepen-task`，或在 Claude Code 输入 `/deepen-task`，然后附上原任务。

> 把这条任务改得更深入，交付物仍是一份一页的诊断报告：调查为什么结账成功率下降，并说明最可能的原因。

Skill 会先给出四项分析，再输出可复制的改写稿。这个例子适合把「调查下降」具体化为检查原始结账事件、对齐分母和时间窗口、区分失败阶段，并用独立的支付记录核对结论。

## 库结构

每个 Skill 放在 `skills/<skill-name>/` 下，以 `SKILL.md` 为入口。新增 Skill 时，在本页目录登记名称和用途。
