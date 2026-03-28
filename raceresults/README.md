# Race Results

Race results are organized by year. Each year has its own folder containing one Markdown file per event.

## Folder structure

```
raceresults/
  YYYY/
    index.md                          ← auto-generated year landing page (lists all events)
    SERIES-E#-MonDD-Venue-Name.md     ← one file per race event
```

## Adding a new race result

1. Create a new `.md` file inside the correct year folder (e.g. `raceresults/2026/`).
2. Name it using the convention: `SERIES-E#-MonDD-Venue-Name.md`
   - `SERIES` — series identifier (e.g. `KCRX`, `KSRX`)
   - `E#` — event number within the series for that year (e.g. `E1`, `E10`)
   - `MonDD` — month abbreviation + zero-padded day (e.g. `Mar22`, `Nov08`)
   - `Venue-Name` — venue with spaces replaced by hyphens
3. Use this front matter template at the top of the file:

```yaml
---
layout: default
title: "SERIES E# - Mon DD - Venue Name"
series: SERIES
event: #
date: YYYY-MM-DD
venue: Venue Name
format: Format Name   # optional (e.g. Endurocross, Barrel Racing, Plinko, BDR)
---
```

4. Below the front matter, add the event heading and results table:

```markdown
**SERIES E# - Mon DD - Venue Name**

| Driver | Class | Car | Finish | Total Time | Notes |
|--------|-------|-----|--------|------------|-------|
| Driver Name | Class | Car | Finish | Time | Notes |
```

## Creating a new year folder

1. Create a new folder named with the 4-digit year: `raceresults/YYYY/`
2. Copy `raceresults/2025/index.md` into the new folder, updating the title to the new year
   and adjusting the Liquid filter `p.dir == '/raceresults/YYYY/'` to match.
