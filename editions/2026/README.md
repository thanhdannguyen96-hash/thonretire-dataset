# ThonRetire Retirement Index 2026

A sealed edition of the ThonRetire retirement destination dataset.

**DOI:** https://doi.org/10.5281/zenodo.21817351

**Landing page:** https://thonretire.com/edition/2026
**Licence:** Creative Commons Attribution 4.0 International (CC-BY-4.0) — https://creativecommons.org/licenses/by/4.0/
**Released:** 2026-08-01 · **Data verified:** July 2026 · **Version:** 1.3

## What this is

17 retirement destinations scored on 39 criteria across
6 ranking axes. It is assembled by hand from the page each government
publishes, and **every figure carries the month that page was last opened**.

Two things follow from that, and both are unusual:

1. A figure past twice its refresh interval is **withheld**, not shown stale. The
   `status` column says so out loud rather than leaving a silent blank.
2. `thonretire-2026-facts.csv` is one row per fact, each with its own verification date,
   confidence, volatility class and a link to the primary source. That is the dataset;
   the wide table is a convenience.

## Files

| File | Rows | What it is |
| --- | --- | --- |
| `thonretire-2026-countries.csv` | 17 | One row per destination, wide. Convenience view — no per-field provenance. |
| `thonretire-2026-facts.csv` | 391 | One row per public fact, with its own verification date, freshness status, confidence and primary source link. |
| `thonretire-2026-cities.csv` | 62 | One row per city, including the gap between city cost and the country-level headline figure. |
| `thonretire-2026.json` | — | Everything above in one file, with the field dictionary and this licence embedded. |
| `edition-2026.json` | — | The sealed edition itself: rankings, facets, changelog, method and integrity hash. |
| `MANIFEST.sha256` | — | Checksums for everything above. |

## Verifying it

The edition file carries a sha256 over its own contents (excluding the
`integrity` field itself):

```
45f2266f7801ff60ec5760b90369d5c8010e0a2687cb6c34a34e449622f68f13
```

Check the package contents against `MANIFEST.sha256`:

```sh
sha256sum -c MANIFEST.sha256
```

## Citing it

```
Nguyễn Thành Dân (2026). ThonRetire Retirement Index 2026. Frozen 2026-08. https://thonretire.com/edition/2026 — CC-BY-4.0
```

BibTeX key: `thonretire-index-2026`. It will not change. A later edition arrives as a
separate entry rather than overwriting this one.

## What it is not

Not legal, tax or immigration advice. I am not an immigration lawyer, a tax adviser or a financial adviser, and nothing here is advice. What I can promise is narrower and checkable: where each number came from, and when.

Known gaps are stated rather than hidden: Some immigration backlogs, bank KYC timelines and insurance quotes move faster than this page. Open gaps are marked in criteria. Always confirm against the official source before acting.
