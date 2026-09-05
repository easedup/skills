# EduPlugins Skills

Skills are folders of instructions, scripts, and resources that an AI agent loads dynamically to
improve performance on a specialized task. This repository is EduPlugins' public collection of
[Agent Skills](https://agentskills.io) — it follows the conventions of
[anthropics/skills](https://github.com/anthropics/skills), the reference implementation for skills
built for Claude.

For background on the format itself:
- [What are skills?](https://support.claude.com/en/articles/12512176-what-are-skills)
- [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude)
- [How to create custom skills](https://support.claude.com/en/articles/12512198-creating-custom-skills)
- [Agent Skills spec](https://github.com/anthropics/skills/blob/main/spec/agent-skills-spec.md)

## About this repository

This repo is content, not code — each skill is self-contained in its own folder with a `SKILL.md`
file containing the instructions and metadata an agent reads. It's built to feed the
[home](https://github.com/eduplugins/home) site's skills catalog (`easedup.com/skills`) the same way
[eduplugins/plugins](https://github.com/eduplugins/plugins) already feeds it for the Education
industry — `home` pulls `skills/<category>/<name>/SKILL.md` straight out of this repo at build time.

## Repo structure

```
skills/<category>/<name>/SKILL.md   hand-authored — one folder per skill, grouped by category
skills/<category>/<name>/LICENSE.txt  per-skill license (Apache 2.0 by default — see below)
.claude-plugin/marketplace.json     the Claude Code plugin marketplace manifest
template/SKILL.md                   starting point for a new skill
CONTRIBUTING.md                     how to propose a skill
```

One deliberate difference from `anthropics/skills`: skills here sit under a category folder
(`skills/<category>/<name>/SKILL.md`, e.g. `skills/assessment/rubric-builder/`) rather than flat
(`skills/<name>/SKILL.md`). That's so this repo can be ingested by `home`'s catalog exactly the way
`eduplugins/plugins` already is, with no parser changes.

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

## Try in Claude Code

Once this repo has skills in it, register it as a Claude Code plugin marketplace:

```
/plugin marketplace add eduplugins/skills
```

then browse and install from it, the same way you would
[anthropics/skills](https://github.com/anthropics/skills#try-in-claude-code-claudeai-and-the-api).

## Disclaimer

Skills in this repository are provided for the tasks they describe. Always test a skill in your own
environment before relying on it for critical work.

## License

There's no single repo-wide license — each skill folder carries its own `LICENSE.txt`, same as
[anthropics/skills](https://github.com/anthropics/skills). Apache 2.0 is the default for skills
authored here; see the per-skill `LICENSE.txt` for the terms that actually apply.
