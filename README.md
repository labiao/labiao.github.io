# Daoyuan Zheng's Academic Homepage

Complete [al-folio v1.2](https://github.com/alshedivat/al-folio/releases/tag/v1.2) site using the official `al_folio_core` theme and upstream pinned plugins.

## Deployment

In **Settings → Pages → Build and deployment → Source**, select **GitHub Actions**. Push all migrated files to `main` or `master`. The **Build and deploy al-folio** workflow builds and publishes the full site at <https://labiao.github.io>.

The built-in GitHub Pages Jekyll build cannot load al-folio's custom plugins. Do not select **Deploy from a branch** for this source repository.

## Content

- `_config.yml`: identity, domain, appearance, feature flags.
- `_pages/about.md`: biography, portrait, news, selected publications.
- `_bibliography/papers.bib`: all 20 migrated papers; `selected = {true}` adds a paper to the homepage.
- `_news/`: announcements.
- `_projects/` and `_pages/projects.md`: research code and funded projects.
- `_data/socials.yml`: email, Google Scholar, GitHub, ORCID, CV links.
- `_data/cv.yml`: structured CV rendered by the official plugin.
- `assets/img/profile.jpg`: original portrait.
- `files/Daoyuan_Zheng_CV.pdf`: original downloadable CV.

Author lists that originally used “et al.” remain abbreviated. Full coauthors have not been guessed.

## Local build

Use Ruby 3.3 or later, Node.js, and ImageMagick:

```bash
bundle install
npm ci
bundle exec al-folio upgrade audit
bundle exec jekyll build
bundle exec jekyll serve
```

Open <http://localhost:4000/>. This personal site uses an empty `baseurl`. Official gems supply the theme layouts, styles, scripts, icons, and search; no custom runtime overrides are used.

Upstream license is retained in `LICENSE`.
