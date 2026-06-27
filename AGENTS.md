# Agent Notes

This repository is the Projects hub for `https://dev-heps.github.io/projects/`.

## Purpose

- Keep a maintained public index of projects.
- Do not replace individual project repositories.
- Each project entry should link to source, demo, and write-up when available.

## Structure

- `docs/`: GitHub Pages source. Pages is configured to publish `main` branch `/docs`.
- `docs/index.html`: Projects index page.
- `docs/projects.js`: canonical public project metadata.
- `docs/guide/index.html`: maintenance guide.
- `docs/styles.css`: shared styling for public pages.
- `templates/project-page.md`: template for project write-ups in project repos.

## Editing Rules

- Update `docs/projects.js` when adding or changing project entries.
- Keep fields consistent: `title`, `summary`, `status`, `domain`, `year`, `source`, `demo`, `writeup`.
- Use directory URLs with trailing slashes for public pages.
- Every public page should include a path back to `Projects` and `Portfolio`.
- Do not add GitHub Actions workflows unless the token has `workflow` scope. This repo currently uses `/docs` Pages publishing.
- Keep the design aligned with the main portfolio: thin borders, compact cards, quiet typography.

## Checks

Before commit:

```bash
git diff --check
```

After pushing, verify:

- `https://dev-heps.github.io/projects/`
- `https://dev-heps.github.io/projects/guide/`

