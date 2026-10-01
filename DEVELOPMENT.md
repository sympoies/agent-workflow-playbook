# Development

Contributor guide for maintaining the Agent Workflow Playbook website. Read
[`AGENTS.md`](AGENTS.md) first.

## Setup and source ownership

Use Node.js 24 or newer. The site has no dependency-install step: its build and
validation scripts use Node.js directly.

- `src/index.html`, `src/main.js`, and `src/styles.css` own site content and
  behavior.
- `src/assets/` owns checked-in images and diagrams.
- `scripts/build.mjs` owns the deterministic `dist/` build.
- `scripts/validate.mjs` owns repository assertions.
- `.github/workflows/pages.yml` owns GitHub Pages build and publication.

Keep contributor procedure here, user-facing project identity in
[`README.md`](README.md), and detailed topic content in the site source.

## Change workflow

1. Update the smallest owning source or asset; do not edit generated `dist/`.
2. Keep public links, commands, diagrams, and screenshots aligned with the
   behavior they describe.
3. Run the finish-line checks:

   ```sh
   npm run build
   npm test
   ```

4. Preview locally when presentation or interaction changes:

   ```sh
   npm run serve
   ```

5. Deliver through the governed managed-worktree and PR flow. A merge to
   `main` triggers the Pages workflow.
