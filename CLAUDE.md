@AGENTS.md

# CLAUDE.md — Social Science Collaboratory Website

## Project overview

This is the website for the **Social Science Collaboratory**, a research group at the **University of Florida**. The lab focuses on advancing open, collaborative, and quantitative methods in the social sciences, with three main research strands:

1. **Studying big team science** — tracking patterns and impact across millions of scientific teams
2. **Building big team science** — running large multi-lab collaborations (Many Smiles, Global Gratitude, EPiC)
3. **Supporting big team science** — publishing guides and advising other large initiatives (Psychological Science Accelerator, etc.)

The site is being migrated from Wix (current site: https://www.nicholas-a-coles.com/social-science-collaboratory) to GitHub Pages.

## Technical stack

- **Theme:** al-folio (https://github.com/alshedivat/al-folio), Jekyll-based
- **Hosting:** GitHub Pages, deployed via GitHub Actions (`.github/workflows/deploy.yml`)
- **Repo:** Social-Science-Collaboratory/LabWebsite on GitHub
- **Live site:** https://social-science-collaboratory.github.io/LabWebsite/
- **Local environment:** Windows 11, VS Code, GitHub Desktop, PowerShell

## Working preferences

- **Explain before doing.** For non-trivial changes, briefly say what you're about to do and why before doing it. For tiny edits (typo fixes, single config values), just do it.
- **Make small, focused commits.** One logical change per commit. Suggest clear commit messages.
- **Don't bulk-rewrite.** We prefer targeted line-level fixes over wholesale rewrites of files we've been working on. If a file already has structure, preserve it and edit minimally.
- **Flag al-folio-specific conventions.** When you do something that's particular to al-folio (e.g., editing `_pages/`, `_data/`, `_bibliography/`, the `enabled:` toggles in `_config.yml`), mention it so that we learn the theme structure.
- **Don't touch the LICENSE file.** al-folio is MIT-licensed; the LICENSE must stay.

## Current status (update as work progresses)

- ✅ Repo created from al-folio template
- ✅ GitHub Pages enabled, deploy workflow succeeding
- ✅ `_config.yml` URL/baseurl set correctly; live site loads
- ⏳ Local preview environment (Docker via al-folio's `.devcontainer/`, or native Ruby+Jekyll) — **next task**
- ⏳ Demo content cleanup — `about.md` updated with real PI bio and research links; `about_einstein.md` still present (needs removal); demo publications/projects still in place
- ⏳ Disable unused al-folio features (CV, teaching, books, etc.) in `_config.yml`
- ⏳ Port content from Wix site — PI bio drafted in `about.md`; three research-strand sections and People page still needed
- ⏳ Custom domain transfer from Wix (later)

## Decisions already made

- **Theme: al-folio**, chosen over Beautiful Jekyll because al-folio has built-in structure for lab sites (people, publications, projects, news as al-folio collections) that maps better to the Collaboratory's content.
- **Repo name: `LabWebsite`** (capital L, capital W). The site lives at `/LabWebsite/`. May rename to lowercase-hyphenated later; if so, update `baseurl` in `_config.yml`.
- **Deployment: GitHub Actions** (al-folio's default), source = "GitHub Actions" in Settings → Pages.
- **Workflows to disable/delete:** "Prettier code formatter" and "Render a CV" — both fail noisily and aren't needed for a lab site. Don't need to act on this immediately; tracking for cleanup pass.

## Useful file/folder map (al-folio)

- `_config.yml` — main settings, feature toggles, navigation
- `_pages/` — top-level pages (about, publications, people, etc.)
- `_data/` — YAML data files (team members, etc.)
- `_bibliography/papers.bib` — publications as BibTeX entries
- `_news/` — short news items (one Markdown file per item)
- `_projects/` — project cards (one per file)
- `assets/img/` — images
- `_includes/` and `_layouts/` — theme internals; touch with care
- `.github/workflows/` — GitHub Actions (deploy.yml is the important one)
