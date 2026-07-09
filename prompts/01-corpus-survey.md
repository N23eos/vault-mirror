# 01 — Corpus Survey

## Goal

Produce a factual census of the vault and fix the methodology that all later
modules will reuse. No interpretation yet — only what is there.

## Method

- Walk the vault (respecting exclusions from `00-start.md`). Record: note
  count, total volume, date range, notes per year/period, folder map, size
  distribution (find the giants and the one-liners).
- Detect languages used and the dominant one.
- Identify content types: journals, project notes, drafts, lists, clippings,
  fleeting notes. Estimate proportions.
- Fix the sampling strategy for large vaults (see `00-start.md`) and write it
  down explicitly.

## Output contract — `Analysis/01-corpus-survey.md`

```
# Corpus Survey
## Numbers            (count, volume, date range)
## Timeline           (notes per year/period, table)
## Folder map         (what lives where, one line per area)
## Content types      (types + estimated share)
## Languages
## Methodology        (reading strategy for this vault; sampling rules if any)
## Anomalies          (gaps in the timeline, dead folders, oddities)
```

## Rules reminder

Apply the global rules from `prompts/00-start.md`.

## Quality bar

- Could another agent reproduce your numbers from the methodology section?
- Are timeline gaps flagged rather than smoothed over?
- Zero interpretation — save it for later modules.
