# OIO Racing

This repository is the central data store and knowledge base for **OIO Racing**, a grassroots motorsport team competing in rally cross events in the Kansas City area.

## What's Here

| Path | Contents |
|------|----------|
| `raceresults/` | Per-season race results in Markdown tables |
| `index.html` | GitHub Pages entry point listing all result years |
| `.github/copilot-instructions.md` | Instructions that tell GitHub Copilot how to act as an OIO Racing collaborator |

## Series
- **KCRX** — Kansas City Rally Cross
- **KSRX** — Kansas Shifter Rally Cross (also runs specialty formats: Endurocross, Barrel Racing, Plinko, BDR)

## Drivers (as of 2025)
| Driver | Primary Class | Car(s) |
|--------|--------------|--------|
| Ryan Redenbaugh | MF / MR | 2007 Honda Fit, 1973 MGB GTS |
| Ian Jennings | MR / O4 | 1985/1987 Toyota MR2, 2009 Honda Fit, 1994 Toyota Celica |
| Miles Smith | MR | 1985 Toyota MR2, 1991 Mazda Miata |
| Hudson Smith | Novice / MF | 2009 Honda Fit |
| Richard Thompson | SR / O4 | 2001 Mazda MX-5, 1994 Toyota Celica |

## Venues
- Thunder Valley Sand Drags
- Holsworth Farm
- McCain's Offroad Park
- Ray Rocks Offroad Resort
- I-35 Speedway

## Adding Results
Race results go in `raceresults/<year>.md`, following the table format already in use:

```markdown
**<Series> <Event#> - <Date> - <Venue>**

| Driver | Class | Car | Finish | Total Time | Notes |
|--------|-------|-----|--------|------------|-------|
| Name   | Class | Car | Xth of Y | 000.000 | Any notes |
```
