# Development log

A time-ordered narrative of notable work on the Agent Workflow Playbook: what
changed, why it mattered, the evidence, and links worth keeping for future
maintenance. It complements, rather than duplicates, the repository's other
records:

- Commit messages say what changed. The devlog preserves the non-obvious
  context, validation results, and external references that a diff cannot.
- `README.md`, `DEVELOPMENT.md`, and `src/` describe the current site. The
  devlog is an append-only historical narrative; update the canonical current
  source first when content or guidance changes.
- GitHub Pages retains publication history. The devlog summarizes the content
  and maintenance milestones that remain useful after deployment.

## When to add an entry

Add one after non-trivial development work produces a durable outcome worth
future lookup: a substantial teaching module, a site or publishing contract,
a validation milestone, or an incident-relevant finding. Skip copy edits,
transient work, and same-turn fixes with no future decision value.

## Conventions

- One file per month: `docs/devlog/YYYY-MM.md`, with the newest entry on top.
- Write durable maintenance entries in English; keep the playbook's audience
  and site content in Chinese.
- Keep current docs and `src/` current. The devlog records history; it does not
  own the site's current guidance, build, validation, or publishing contract.
- This is a public repository. Never record secrets, private skill contents,
  personal identifiers, internal hostnames, private deployment topology,
  machine-local paths, or credentials. Use public references and neutral
  descriptions.
- Search past entries with `devlog search <term> [--month YYYY-MM]`. The
  `devlog` binary ships with `nils-cli`; without it, search the month files
  directly.
- When an entry is committed separately, use
  `docs(devlog): <YYYY-MM> - <subject>`.

### Entry template

```md
## YYYY-MM-DD - <short title>

### Result

- What shipped or changed.

### Why / context

- The non-obvious reasoning or maintenance context.

### Evidence

- Commands run and concrete observations.

### Links

- Commits, issues, pull requests, external references, and relevant docs.

### Follow-ups

- Optional.
```

`Result`, `Why / context`, and `Evidence` are required. `Links` and
`Follow-ups` are optional: omit the whole section rather than leaving a
placeholder in it.

## Months

- [2026-09](2026-09.md)
- [2026-06](2026-06.md)
