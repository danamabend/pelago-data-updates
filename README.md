# Pelago Data Team — Public Site

Public GitHub Pages site for the Pelago Data Team. Hosts two things:

1. **Monthly data impact updates** at the repo root
2. **Cube Knowledge Center** under `/cube/`

**Live site:** https://danamabend.github.io/pelago-data-updates/
**Cube Knowledge Center:** https://danamabend.github.io/pelago-data-updates/cube/

---

## Cube Knowledge Center

The home for everything related to using Pelago's Cube semantic layer. Lives in `/cube/`. Four interlinked pages:

| File | What it is |
| --- | --- |
| `cube/index.html` | Landing page. Start here for any user. |
| `cube/prompting-best-practices.html` | Full prompting guide for asking Cube questions. |
| `cube/domain-directory.html` | Directory of all 15 Cube data domains, in plain language. |
| `cube/guardrails.html` | Why to use the semantic layer instead of writing custom mart queries. |

### Updating the Knowledge Center

To edit an existing page, open the file in `/cube/`, make the change, commit. Pages rebuilds within ~60 seconds.

To add a new page:

1. Create the new HTML file inside `/cube/`
2. Add a link to the new page in the `<nav>` block of each existing page's top bar
3. Add a card to `cube/index.html` linking to the new page
4. Commit

---

## Monthly Impact Updates

Public landing page for Data Team monthly impact updates lives at the repo root (`index.html`).

### Adding a new month

1. Create the new HTML file and name it using the format `month-year-data-impact.html`
   e.g. `april-2026-data-impact.html`
2. Open `index.html` and find the comment `<!-- ADD NEW MONTHS ABOVE THIS LINE -->`
3. Copy the March card block and paste it above that comment. Update:
   - `href` — filename of the new HTML file
   - Month name and year in the date block
   - Card title, summary text, and tags
   - Add the `latest` class to the new card
   - Remove `latest` from the previous month's card
4. Update the "Coming soon" placeholder at the top to reflect the following month
5. Upload the new HTML file + updated `index.html` to the repo and commit

The site updates automatically within ~60 seconds of committing.

### File naming convention

```
index.html                        ← landing page (permanent link)
march-2026-data-impact.html
april-2026-data-impact.html
may-2026-data-impact.html
...
```

---

## Repo Notes

- GitHub Pages serves directly from `main`. No build step, no Jekyll config.
- `cube-announcement.html` lives at the repo root for backwards-compatibility with previously shared links. Don't move it. Anyone landing on it should be funneled into `/cube/` via in-page links.
- The `/cube/` folder is intentionally separate from the monthly updates so the two don't tangle.
