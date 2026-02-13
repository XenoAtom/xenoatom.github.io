# xenoatom.github.io - Codex Agent Instructions

This repository hosts the XenoAtom landing website published at `https://xenoatom.github.io/`.

Paths and commands below are relative to this repository root.

## Website Scope

- This site is a **landing page** that redirects visitors to project websites and repositories.
- It intentionally has **no docs section** and **no docs sidebar menu**.
- Keep all website source files under `site/`.

## Structure

- `site/readme.md` -> home page (`/`)
- `site/menu.yml` -> top navigation
- `site/config.scriban` -> Lunet project configuration
- `site/img/**` -> logo/images used by the landing page
- `.github/workflows/site.yml` -> GitHub Pages deployment workflow

## Build

Install lunet (once):

`dotnet tool install -g lunet`

Build locally:

`cd site`

`lunet build`

## Contribution Notes

- Keep link cards grouped by category (terminal/CLI, logging, systems foundations, graphics/tooling).
- Prefer linking to:
  - `https://xenoatom.github.io/<project>/` when project docs exist
  - `https://github.com/XenoAtom/<repo>` for repository links
- If new projects are added to the organization, update `site/readme.md`.
