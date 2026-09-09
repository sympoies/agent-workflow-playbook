# Repository policy

## Scope

This repository owns the Chinese-language Agent Workflow Playbook website and
its GitHub Pages publication. Keep the site focused on reusable, public agent
workflow concepts and examples.

## Boundaries

- Never commit credentials, private prompts, private skills, provider payloads,
  internal topology, personal identifiers, or machine-local runtime output.
- Keep reusable source material in `src/`; treat `dist/` as generated build
  output and do not hand-edit it.
- Preserve the site's Chinese audience and established visual language. Keep
  referenced public repositories and commands accurate.
- GitHub Pages publication is owned by `.github/workflows/pages.yml`; an
  ordinary source edit does not authorize a deployment or workflow mutation.

## Working agreement

- Read [`DEVELOPMENT.md`](DEVELOPMENT.md) for the routine contributor workflow.
- Inspect affected source, assets, build behavior, and validation assertions
  before editing.
- Run `npm run build` and `npm test` before delivery.
- Deliver tracked changes through the governed managed-worktree and PR flow.
