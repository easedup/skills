Thank you for your interest in EduPlugins Skills.

We are not currently accepting contributions.

For now:
1. Explore and learn from the skills as they're published
2. Fork the repo for your own experiments — check each skill's `LICENSE.txt` first
3. Share the link with others who might find it useful

Though we are not accepting contributions right now, we'd still love to hear from you! If you have
feedback or suggestions, please open an issue in this repository or contact us
[here](https://eduplugins.com/contact). We'll open up for community contributions once we're ready,
so stay tuned!

## Adding a skill (maintainer notes)

1. Create `skills/<category>/<name>/SKILL.md` — `name` and `description` frontmatter are required;
   see [template/SKILL.md](template/SKILL.md).
2. Add `skills/<category>/<name>/LICENSE.txt` (Apache 2.0 unless the skill needs different terms).
3. Add the skill to a plugin bundle in [.claude-plugin/marketplace.json](.claude-plugin/marketplace.json)
   if it should be installable as (or part of) a Claude Code plugin.
4. `home`'s `sync-content` step picks up any `skills/<category>/<name>/SKILL.md` in this repo
   automatically — no change needed there.
