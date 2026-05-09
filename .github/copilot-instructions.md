# Copilot Instructions

## Project Overview

**nexum.space** is a Jekyll site ("protocol for human evolution") deployed to GitHub Pages at `www.nexum.space`.

## Deployment

- Pushes to `master` automatically trigger the GitHub Actions workflow (`.github/workflows/jekyll-gh-pages.yml`), which builds and deploys the site via `actions/jekyll-build-pages`.
- No manual deploy step is needed.

## Local Development

Jekyll builds from the repository root (`source: ./`). To run locally:

```bash
bundle exec jekyll serve
```

Requires a `Gemfile` with `gem "jekyll"` (or `gem "github-pages"` for full parity with the GitHub Pages build environment).

## Repository Structure

This is an early-stage project. As it grows, standard Jekyll conventions apply:
- `_config.yml` — site configuration
- `_layouts/` — HTML templates
- `_includes/` — reusable partials
- `_posts/` — blog posts (if used)
- `assets/` — CSS, JS, images
- `CNAME` — custom domain (`www.nexum.space`), do not delete or rename
