# Workspace modes

Read this reference only when the project needs persistent records, multiple projects, parallel tasks, or worktrees.

## Single-project mode

Use the host repository's existing conventions. Add only the records that improve review or reproducibility.

An optional compact structure is:

```text
project/
├── README.md
├── research.md
├── reflection.md
├── project.json
├── src/
└── assets/
```

The templates in the skill's `assets/` folder can seed these records. Do not overwrite existing project documentation or force this layout on a mature repository.

## Portfolio mode

Keep projects isolated under one predictable directory, for example:

```text
portfolio/
├── projects/
│   ├── 01-first-project/
│   └── 02-second-project/
├── WORKBOARD.md
└── projects.json
```

Assign one source of truth to each kind of data:

- repository files for reproducible artifacts;
- a private knowledge system for complete working notes, when used;
- a public index for intentionally published metadata only.

Do not make the public site depend on private records. Generate or update shared indexes from explicit public fields.

## Optional lifecycle

Use a lifecycle only when it improves coordination:

```text
idea → researching → replicated → problem-found → proposing
→ implementing → reflected → revising → completed → published
```

Treat these as evidence states, not progress theater. A project reaches `published` only when the public artifact exists and its links have been verified.

## Parallel tasks and worktrees

For concurrent implementation:

1. Keep the main checkout for integration, shared indexes, and release work.
2. Give each active project or non-overlapping change its own branch and worktree.
3. State the permitted project directory in the task handoff.
4. Avoid two tasks editing the same shared files.
5. Finish with evidence, tests, and a focused commit before integration.
6. Validate shared indexes and public metadata after merging.

Do not create a worktree before the repository has a baseline commit. Explain that uncommitted files are not inherited and obtain approval before creating a baseline commit.

## Public/private boundary

Before publishing a workspace-derived project, check for:

- absolute user paths and usernames;
- private knowledge-base URLs or identifiers;
- credentials and environment variables;
- unpublished user data or conversations;
- internal brand assets, copy, or source material;
- claims not supported by the public artifact.

Publish a sanitized snapshot rather than coupling the public artifact to private systems.
