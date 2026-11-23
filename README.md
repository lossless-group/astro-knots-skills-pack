# Astro Knots skill pack

Skills for building Astro sites the way The Lossless Group does: the stack and
its prohibitions, themes and modes, markdown, splash pages, share images and
metadata, analytics, and brand marks.

| Skill | Use it when |
|---|---|
| [`astro-knots`](./skills/astro-knots/) | Starting or changing any Astro site: the tech hierarchy, approved frameworks, and what never to install |
| [`theme-system`](./skills/theme-system/) | Setting up tokens and the light, dark and vibrant modes |
| [`maintain-design-md`](./skills/maintain-design-md/) | Writing or updating a site's `DESIGN.md` |
| [`lossless-flavored-markdown`](./skills/lossless-flavored-markdown/) | Authoring or rendering content with LFM |
| [`maintain-splash-pages`](./skills/maintain-splash-pages/) | Building a repo's `splash/` site on GitHub Pages |
| [`generate-consistent-og-images`](./skills/generate-consistent-og-images/) | Making share images that look like one family |
| [`open-graph-share-seo-geo`](./skills/open-graph-share-seo-geo/) | Getting links to unfurl, plus sitemaps, robots and `llms.txt` |
| [`openpanel-analytics`](./skills/openpanel-analytics/) | Adding or debugging OpenPanel |
| [`trademark-packs-files`](./skills/trademark-packs-files/) | Making a site's favicon, appIcon, wordmark, trademark and `favicon.ico` |

## Layout

Each skill sits at `skills/<name>/SKILL.md`. This repo is mounted into
[`lossless-agent-skills`](https://github.com/lossless-group/lossless-agent-skills)
as the submodule `skill-packs/astro-knots/`, and that repo's
`sync-skills-symlinks.sh` links `~/.claude/skills/<name>` straight to each
skill's folder, so harnesses see every skill by its bare name.

To use the pack on its own, link each skill into your harness's skills
directory:

```bash
for d in skills/*/; do ln -s "$PWD/$d" ~/.claude/skills/; done
```

Why packs exist: `context-v/explorations/Organize-Our-Skills-into-Skill-Packs.md`
in `lossless-agent-skills`.

## Where else it appears

The [Astro Knots MCP](https://github.com/lossless-group/astro-knots-mcp)
copies most of these skills into its `skills/` folder with `pnpm sync-skills`,
so its Claude Code and Codex plugins ship them. Edit them here, never there.
