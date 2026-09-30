# fhuber7.github.io

Personal academic homepage of Florian Huber, live at https://fhuber7.github.io. Built with [Jekyll](https://jekyllrb.com/) and the [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) theme (loaded via `remote_theme`, pinned to a release in `_config.yml`). GitHub Pages builds and deploys the site directly from the `main` branch. This README is excluded from the built site.

## Structure

```
.
├── _config.yml                 # site settings, theme, author sidebar links
├── _data/navigation.yml        # top navigation
├── _includes/head/custom.html  # sidebar styling and link behaviour
├── index.md                    # home page
├── publications.md             # journal articles, other publications, book chapters
├── working-papers.md           # papers under revision and work in progress
├── research.md                 # third-party funding
├── awards.md                   # awards and rankings
├── code.md                     # R packages and replication code
├── cv.md                       # CV (repeats awards, rankings, funding and top papers)
├── assets/images/profile.jpg   # sidebar photo
└── Gemfile                     # Ruby dependencies (local preview only)
```

## Editing content

All pages are plain Markdown. Commit to `main` and GitHub Pages rebuilds the site within a minute or two.

- `cv.md` repeats information from `awards.md`, `publications.md` and `research.md`. Update it whenever those change.
- Check a deploy with `gh api repos/fhuber7/fhuber7.github.io/pages/builds/latest` or on the live page. Do not use `raw.githubusercontent.com`, which can serve stale copies.
- To update the theme, change the release tag in `remote_theme` deliberately and check the live site afterwards.

## Previewing locally (optional)

```bash
bundle install
bundle exec jekyll serve   # then open http://localhost:4000
```
