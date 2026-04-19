# pcsea-dummy-feeds

Fabricated RSS feeds and CSV seed data for the Protein Challenge Southeast Asia (PCSEA) sensing-layer demo.

## Purpose

This repo exists to give an n8n workflow a reliable, rich stream of demo news items to classify during an interview walkthrough of Forum for the Future's PCSEA sensing layer. Real Southeast Asian sustainability RSS feeds are too sparse and unpredictable for a controlled demo, so this repo publishes four fake-but-realistic feeds via GitHub Pages.

**All content is fabricated.** All article URLs resolve to `example.com` placeholders. Organisation names are real (ADB, FAIRR, Aquaspark, DBS, UOB, Temasek, Olam, Wilmar, Nestle SEA, Unilever SEA, GFI APAC, AVPN, etc.), but no quoted individual or event is real. Do not redistribute as journalism.

## Feed URLs

Once GitHub Pages is enabled, the four feeds are available at:

- `https://<username>.github.io/pcsea-dummy-feeds/sea-food-agri.xml` — general food and agriculture news (18 items)
- `https://<username>.github.io/pcsea-dummy-feeds/sea-policy-capital.xml` — policy and capital flows (15 items)
- `https://<username>.github.io/pcsea-dummy-feeds/sea-cooperative-adoption.xml` — cooperative and adoption signals (15 items)
- `https://<username>.github.io/pcsea-dummy-feeds/sea-shocks-context.xml` — climate shocks and context (12 items)

Total: 60 items. Publication dates are spread across the last 14 days, with roughly half inside the last 48 hours.

## Seed data CSVs

Under `seed-data/`:

- `frame-tracker.csv` — 30 rows across 6 weeks, with a visible upward adoption trend
- `practice-watch.csv` — 10 rows against real SEA-active entities
- `pulse-notes.csv` — 3 Visionary-conversation synthesis rows

Import these directly into Airtable via the view-dropdown "Import data" flow.

## Updating content

Edit the XML files (or CSVs), commit, and push. GitHub Pages republishes automatically within a minute or two.

```
git add .
git commit -m "Refresh demo content"
git push
```

To change the weighting of signal types across the feeds, edit the individual `<item>` blocks. The channel metadata at the top of each file rarely needs changing.

## Licence

Treat as internal demo material. Do not redistribute.
