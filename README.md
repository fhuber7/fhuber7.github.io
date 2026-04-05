# fhuber7.github.io

Personal academic homepage of Florian Huber, built with [Jekyll](https://jekyllrb.com/) and the default [Minima](https://github.com/jekyll/minima) theme — deployed via GitHub Pages.

## Structure

```
.
├── _config.yml        # site settings and nav
├── index.md           # home page (bio, awards, contact)
├── publications.md    # full publication list
├── research.md        # current research & funded projects
├── code.md            # replication code / R packages
├── cv.md              # short CV
├── teaching.md        # teaching history
├── assets/css/        # minimal SCSS overrides
├── Gemfile            # Ruby dependencies (for local preview)
└── README.md
```

## Deploying to GitHub Pages

1. Create a **public** repository named `YOURUSER.github.io` (e.g. `fhuber7.github.io`).
2. Copy all files in this folder into the repo (or push from this folder directly).
3. On GitHub: **Settings → Pages → Source → Deploy from a branch → `main` / `/ (root)` → Save**.
4. Within a minute or two the site will be live at `https://YOURUSER.github.io`.

### Pushing from the command line

```bash
cd fhuber-github-page
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOURUSER/YOURUSER.github.io.git
git push -u origin main
```

## Previewing locally (optional)

```bash
# Install Ruby + bundler first, then:
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```

## Editing content

All pages are plain **Markdown**. Just edit the `.md` files and commit — GitHub Pages will rebuild the site automatically.
