# Nurikabe Islands website

The site for [Nurikabe Islands](https://nurikabeislands.com), a logic puzzle game for iOS and Android. It's a small Jekyll site, and GitHub Pages builds and deploys it on every push to `main`.

## Layout

```
_config.yml          site name, URL, contact email, store links
_layouts/            default (shell) → page (header + white panel) / privacy
_includes/           head, nav, footer, page header, panel, background numbers, icons/
_data/
  i18n.yml           nav and footer labels per language
  rules.yml          How to Play (home)
  features.yml       feature cards (home)
  faq.yml            FAQ (support), answers in Markdown
  privacy/en.yml     privacy policy, one file per language
assets/css/          base.css (shared) + home / support / privacy
assets/images/       icon and logo
index.html, support.html, privacy*.html    pages (front matter + markup)
```

`CNAME`, `app-ads.txt`, `robots.txt` and `sitemap.xml` stay at the root, where crawlers and ad networks expect them.

## Editing

- **Copy:** usually a YAML file in `_data/`.
- **Privacy policy:** edit `_data/privacy/<lang>.yml` and update `updated`. `privacy.html` and `privacy-en.html` (the App Store link) both show the English text.
- **New privacy language:** add `_data/privacy/<lang>.yml`, its labels in `_data/i18n.yml`, a `privacy-<lang>.html` stub, and an entry under `translations` in `_layouts/privacy.html`.

## Preview

```bash
gem install jekyll
jekyll serve        # http://localhost:4000
```
