# CBB Hackathon — Site

Single-page Jekyll site for the Computational Biology & Bioinformatics
Hackathon. Deployed via GitHub Pages. All main content lives on the
homepage as anchor sections; the navbar jumps between them.

## Editing content

All page content lives in markdown — edit the file, commit, GitHub Pages rebuilds.

| What you want to change                | Where to edit                          |
| -------------------------------------- | -------------------------------------- |
| Site title, dates, URLs                | `_config.yml` (top of file)            |
| Any homepage section's content         | `_sections/<weight>-<name>.md`         |
| Add a new homepage section             | New file in `_sections/` with `weight` |
| Top navbar order/labels                | `_data/navigation.yml`                 |
| Organizing committee                   | `_data/organizers.yml`                 |
| Sponsors / partners                    | `_data/partners.yml` + logo files      |
| Per-project detail pages               | `_projects/*.md`                       |
| Colors / typography                    | `_sass/_variables.scss`                |
| Logos and images                       | `assets/images/`                       |

### How sections work

Each file in `_sections/` becomes one anchor block on the homepage.
Front matter controls the section:

```yaml
---
title: "Build with biology, in three days."   # H2 heading
eyebrow: About                                  # tiny uppercase label above
section_id: about                               # the #anchor id (must match _data/navigation.yml)
weight: 10                                      # ordering on the page (low → top)
section_class: "section--alt"                   # optional: alt background
---
```

Add a new section by dropping a markdown file in `_sections/`, picking a
`weight` between existing ones, and adding a matching nav entry to
`_data/navigation.yml` with `url: "#your-section-id"`.

### Per-project pages

The Projects section on the homepage shows project cards that link to
detail pages. Add a project by dropping a markdown file in `_projects/` —
it appears in the cards automatically. Use one of the existing files as a
template.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Deploy

Push to GitHub. In repository **Settings → Pages**, set source to
**GitHub Actions** (recommended) or the `gh-pages` branch. The
`github-pages` gem handles the build.

If hosting under `https://<user>.github.io/<repo>/`, set
`baseurl: "/<repo>"` in `_config.yml`.
