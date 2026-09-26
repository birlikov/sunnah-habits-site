# Sunnah Habits — support and privacy site

Three static pages, no build step, no external assets: everything (CSS included) is
inline, and both themes come from `prefers-color-scheme`.

| File           | Served at  |
| -------------- | ---------- |
| `index.html`   | `/`        |
| `privacy.html` | `/privacy` |
| `support.html` | `/support` |

GitHub Pages resolves an extensionless request to the matching `.html` file, which is
why the App Store URLs have no `.html` on them and why the links between these pages
are written without it.

## Deployment

Deployed with **GitHub Pages from the `main` branch, repository root** — not from
`/docs`, and with no Actions workflow or Jekyll build. Copy the three HTML files to
the root of the [`sunnah-habits-site`](https://github.com/birlikov/sunnah-habits-site)
repository, push to `main`, and in **Settings → Pages** set the source to
_Deploy from a branch_ → `main` → `/ (root)`.

Live at:

- https://birlikov.github.io/sunnah-habits-site/
- https://birlikov.github.io/sunnah-habits-site/privacy
- https://birlikov.github.io/sunnah-habits-site/support

The last two are the Privacy Policy URL and the Support URL given in App Store
Connect, and in `store/metadata/*.json`.

## Editing

Keep the three pages consistent: same palette, same `max-width`, same footer. If the
privacy policy changes in substance, update the effective date on `privacy.html`.
