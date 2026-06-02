# AGENTS.md

Guidelines for AI agents working in this repository.

## Repository Overview

This repository publishes a portable writing skill for AI agents. The installable skill lives under `skills/` and follows the Agent Skills directory shape:

```text
skills/
└── clear-writing/
    ├── SKILL.md
    └── references/
```

The `.claude/skills/` directory is kept for Claude Code project-local use. Keep the skill content synchronized when changing the published skill.

## Published Skills

- `clear-writing`: Rules and worked examples for writing clear, accurate prose that does not read like AI-generated text. Tone-neutral; intended for business communication.

## Skill Format

Each skill requires a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: skill-name
description: What this skill does and when to use it.
---
```

Optional supporting material belongs beside the skill:

```text
skills/skill-name/
├── SKILL.md
├── references/
├── scripts/
└── assets/
```

## Manual Checks

- `name` must match the parent directory name.
- `description` should state what the skill does and when to use it.
- Keep large reference material in `references/` so agents can load it on demand.
- Do not weaken the writing rules while changing the package format.
