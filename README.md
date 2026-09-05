# EasedUP Skills

Skills are folders of instructions, scripts, and resources that an AI agent loads dynamically to
improve performance on a specialized task. This repository is EasedUP' public collection of
[Agent Skills](https://agentskills.io).

## About this repository

This repo is content, not code — each skill is self-contained in its own folder with a `SKILL.md`
file containing the instructions and metadata an agent reads.

## Repo structure

```
skills/<category>/<name>/SKILL.md   hand-authored — one folder per skill, grouped by category
skills/<category>/<name>/LICENSE.txt  per-skill license (Apache 2.0 by default — see below)
.claude-plugin/marketplace.json     the Claude Code plugin marketplace manifest
template/SKILL.md                   starting point for a new skill
CONTRIBUTING.md                     how to propose a skill
```

## Creating a basic skill

Skills are simple to create — just a folder with a `SKILL.md` file containing YAML frontmatter and
instructions. Use [template/SKILL.md](template/SKILL.md) as a starting point:

```markdown
---
name: my-skill-name
description: A clear description of what this skill does and when to use it
license: Complete terms in LICENSE.txt
---

# My Skill Name

[Add your instructions here that the agent will follow when this skill is active]
```

The frontmatter requires two fields:
- `name` — a unique identifier for the skill (lowercase, hyphens for spaces)
- `description` — a complete description of what the skill does and when to use it

Place the folder at `skills/<category>/<name>/`, alongside a `LICENSE.txt` (Apache 2.0 unless the
skill states otherwise). See [CONTRIBUTING.md](CONTRIBUTING.md) before opening a PR.


## Disclaimer

Skills in this repository are provided for the tasks they describe. Always test a skill in your own
environment before relying on it for critical work.
