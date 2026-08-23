# Projects Emergence

[简体中文](README.zh-CN.md)

Projects Emergence is a research-driven Agent Skill that turns rough ideas into reproducible, reflective, and publishable projects.

It helps Codex and other Agent Skills-compatible tools decide when to research, when to replicate an existing solution, when to implement, and when to pause for evidence or approval.

## Why

Project workflows often jump from an exciting idea straight to implementation. The result may run without answering whether it solves the right problem, whether a mature reference already exists, or whether its public claims are supported.

Projects Emergence introduces a proportionate loop:

```text
clarify → research → replicate or adapt → implement → reflect → research → revise
```

The workflow does not require novelty. Replication, adaptation, focused improvement, and redesign are all valid paths when supported by evidence.

## What the beta includes

- Proportionate research routing for new ideas, design choices, bugs, and publication risks.
- An explicit evidence gate before substantial implementation.
- Replicate / adapt / improve / redesign decision paths.
- Minimal implementation and verification guidance.
- Project-specific reflection prompts and a research re-entry loop.
- Optional templates for research, reflection, and public-safe project metadata.
- Optional portfolio, multi-project, and Git worktree coordination.
- A skills-only Codex plugin manifest.

## Install

Ask Codex to install the skill from this repository:

```text
$skill-installer Install projects-emergence from https://github.com/xlth10/projects-emergence/tree/main/skills/projects-emergence
```

For a manual Codex installation, clone the repository and link or copy the skill folder into `~/.agents/skills/`:

```bash
git clone https://github.com/xlth10/projects-emergence.git
mkdir -p ~/.agents/skills
ln -s "$(pwd)/projects-emergence/skills/projects-emergence" ~/.agents/skills/projects-emergence
```

Restart Codex if the skill does not appear immediately.

## Use

Invoke it explicitly:

```text
$projects-emergence I have an idea for a local-first reading tool.
```

Or describe a matching task naturally. Implicit invocation is enabled by default.

## Design boundaries

The beta intentionally does not include:

- Notion or another knowledge-base dependency;
- machine-specific paths or portfolio IDs;
- automatic commits, pushes, deployments, purchases, or messages;
- a requirement to create process documents for every small task;
- claims that a runnable implementation is automatically a completed project.

## Repository layout

```text
.codex-plugin/plugin.json                  Skills-only plugin manifest
skills/projects-emergence/SKILL.md         Skill entry point
skills/projects-emergence/references/      Conditional workflow guidance
skills/projects-emergence/assets/          Optional project templates
examples/emergence-lab/                    Origin and dogfooding case study
evals/cases.md                             Behavioral evaluation cases
```

## Status

`v0.1.0-beta` is based on repeated use in the Emergence Lab portfolio. The next milestone is external validation across different repositories, project types, and agent hosts.

## License

Apache License 2.0. See [LICENSE](LICENSE).
