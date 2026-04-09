# Pelago Data Team — Monthly Updates

Public landing page for Data Team monthly impact updates.

**Live site:** https://danamabend.github.io/pelago-data-updates/

---

## Adding a new month

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

---

## File naming convention

```
index.html                        ← landing page (permanent link)
march-2026-data-impact.html
april-2026-data-impact.html
may-2026-data-impact.html
...
```
