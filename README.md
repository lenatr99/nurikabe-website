# Nurikabe Islands Website

Static website for the Nurikabe Islands iOS and Android app.

## Files

- `index.html` - Landing page
- `privacy.html` - Privacy Policy (default, redirects to English)
- `privacy-{lang}.html` - Localized privacy pages (generated)
- `privacy_template.html` - Template with `{{placeholders}}` for localization
- `support.html` - Support page with FAQ
- `icon.png` - App icon
- `logo.png` - Sailboat logo (from Nurikabe/Resources/Logo)

## Privacy localization

Privacy content is driven by JSON files in `metadata/privacy_lang/`:

- `en.json` - English (source of truth)
- `de.json`, `fr.json`, etc. - Per-locale translations

To regenerate all privacy pages after editing the template or locale JSONs:

```bash
python3 scripts/generate_privacy.py
```

This produces `privacy-en.html`, `privacy-de.html`, etc., plus `privacy.html` (copy of English).