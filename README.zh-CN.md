# Projects Emergence

[English](README.md)

Projects Emergence 是一个研究驱动的 Agent Skill，用于把早期灵感发展为可调研、可复现、可反思、可修正和可公开展示的项目。

它帮助 Codex 以及兼容 Agent Skills 标准的工具判断：什么时候需要调研，什么时候应直接复现成熟方案，什么时候进入实现，以及什么时候应该因为证据或授权不足而暂停。

## 为什么需要它

很多项目会从“这个想法不错”直接跳到写代码。最终结果可能可以运行，却没有回答：问题是否真实、是否已有成熟方案、改动是否必要、公开结论是否有证据。

Projects Emergence 使用一个按需循环：

```text
澄清 → 调研 → 复现或适配 → 实现 → 反思 → 调研 → 修正
```

这个工作流不强制创新。只要有证据支持，直接复现、场景适配、局部改进和重新设计都是合理结果。

## Beta 内容

- 针对新想法、设计选择、Bug 和发布风险选择合适的调研深度。
- 在大规模实现前设置证据与用户确认闸门。
- 明确区分直接复现、场景适配、局部改进和重新设计。
- 先实现能够验证假设的最小切片，再扩大范围。
- 根据产品、工具、研究、创意或数据项目选择反思问题。
- 提供可选的调研、反思和公开项目元数据模板。
- 提供可选的作品集、多项目和 Git worktree 协作模式。
- 包含 skills-only Codex plugin manifest。

## 安装

可以让 Codex 直接从 GitHub 安装：

```text
$skill-installer 从 https://github.com/xlth10/projects-emergence/tree/main/skills/projects-emergence 安装 projects-emergence
```

也可以手动克隆并把 Skill 复制或链接到 `~/.agents/skills/`：

```bash
git clone https://github.com/xlth10/projects-emergence.git
mkdir -p ~/.agents/skills
ln -s "$(pwd)/projects-emergence/skills/projects-emergence" ~/.agents/skills/projects-emergence
```

如果没有立即出现，请重启 Codex。

## 使用

显式调用：

```text
$projects-emergence 我有一个灵感：做一个本地优先的阅读工具。
```

也可以直接描述符合范围的任务。Skill 默认允许自动匹配。

## 边界

Beta 版本不会：

- 强制依赖 Notion 或其他知识库；
- 包含用户本地路径、私人项目编号或内部记录；
- 未经授权自动提交、推送、部署、购买或发送消息；
- 要求每个小任务都创建流程文档；
- 因为代码能够运行就自动宣称项目已经完成。

## 当前状态

`v0.1.0-beta` 已在 Emergence Lab 的多个真实项目中持续使用。下一阶段将验证它在不同仓库、项目类型和 Agent 宿主中的表现。

## 许可证

Apache License 2.0，详见 [LICENSE](LICENSE)。
