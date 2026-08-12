# Repository Guidelines

## Agent Working Agreements

- Prefer minimal, targeted changes; avoid unrelated refactoring or formatting.
- Inspect the existing implementation before modifying it.
- Do not commit, push, merge, delete branches, or otherwise modify Git history.
- Do not add or update dependencies unless the task explicitly requires it.
- Before finishing, run the applicable local checks and review the resulting diff.
- Report the files changed, commands run, and verification performed.
- If an important requirement is ambiguous, ask before making the change.

## Project Structure & Module Organization

This repository builds a Jekyll academic website. Site-wide settings live in `_config.yml`. Page content is organized in `_pages/`, while dated posts and collection entries live in `_posts/`, `_talks/`, `_teaching/`, `_portfolio/`, `_notebooks/`, and `_codes/`. Reusable Liquid markup belongs in `_includes/`; page shells belong in `_layouts/`. Store images in `images/` and JavaScript, fonts, and other theme resources in `assets/`.

Content-generation utilities are in `markdown_generator/`, with additional CV conversion scripts in `scripts/`. Avoid editing backup files ending in `~`; update the corresponding source file instead.

## Build, Test, and Development Commands

- `bundle install` installs Ruby and Jekyll dependencies.
- `bundle exec jekyll serve -l -H localhost` builds the site, watches for changes, and serves it at `http://localhost:4000`.
- `bundle exec jekyll build` performs a production-style build and catches Liquid, front-matter, and configuration errors.
- `docker compose up --build` runs the same development site in a container.
- `npm install` installs JavaScript build dependencies.
- `npm run build:js` regenerates `assets/js/main.min.js` from the source scripts.

## Coding Style & Naming Conventions

Use two-space indentation in YAML, HTML, Liquid, JavaScript, and JSON. Keep Markdown concise and include valid YAML front matter where Jekyll expects it. Follow existing collection naming: dated posts use `YYYY-MM-DD-slug.md`; other entries use descriptive lowercase or established course identifiers such as `_teaching/EC413.md`. Edit `assets/js/_main.js` or plugin sources, then rebuild the minified bundle rather than hand-editing it.

## Testing Guidelines

There is no dedicated automated test suite or coverage target. Before submitting changes, run `bundle exec jekyll build`, inspect the affected page locally, and check navigation, links, images, and responsive layout. For Python generator changes, run the modified script against its TSV input and review the generated Markdown diff.
- Bundler may be installed user-locally and absent from `PATH`. If `bundle`
  is unavailable, locate the user gem directory with `Gem.user_dir` rather
  than modifying shell configuration automatically.
  
## Commit & Pull Request Guidelines

Recent commits use short, imperative or topic-style subjects such as `CV`, `about`, and `codes`. Prefer a concise, specific subject (for example, `Update EC413 teaching page`) and keep each commit focused. Pull requests should explain the user-visible change, identify affected pages or collections, link relevant issues, and include screenshots for layout or styling changes. Confirm the local Jekyll build result in the description.
