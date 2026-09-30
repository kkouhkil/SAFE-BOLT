# SAFE-BOLT Website

Public Jekyll/GitHub Pages website for **SAFE-BOLT: Safety-Assured Force-aware Execution for Bimanual Operations on Lab Tools**.

## The files you normally edit

- `index.md` — homepage structure
- `_data/home.yml` — homepage wording and research pipeline
- `project.md`, `research.md`, `applications.md`, `demo.md`, `team.md`, `resources.md` — page content
- `_posts/` — project/news updates
- `assets/css/style.css` — layout, font sizes and visual design
- `assets/css/colors.css` — reusable color library
- `assets/img/` — approved images

## Header controls

In `assets/css/style.css`, search for:

- `.ut-logo` → UT Austin logo size
- `.project-brand` → SAFE-BOLT header text size
- `.nav` → Project / Research / Applications / etc. size and spacing

The required logo filename is:

`assets/img/branding/ut_austin_primary.png`

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000/SAFE-BOLT/`.

## GitHub Pages

The repository can remain named `SAFE-BOLT`. With `baseurl: /SAFE-BOLT`, the project site is designed for a URL such as `https://<username>.github.io/SAFE-BOLT/`.
