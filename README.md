# ThonRetire — sealed editions

Machine-readable mirror of the ThonRetire retirement destination dataset, one folder per
sealed edition. Licensed CC-BY-4.0: use it anywhere, including commercially, including
in a competing ranking. The only condition is that you credit ThonRetire and link back.

**Site:** https://thonretire.com · **Method:** https://thonretire.com/method · **Live data:** https://thonretire.com/data

## Editions

| Edition | Released | Destinations | Version | DOI |
| --- | --- | --- | --- | --- |
| [2026](editions/2026/) | 2026-08-01 | 17 | v1.3 | — |

## Why "sealed"

The site keeps moving — a figure re-checked today changes the live ranking today. That is
right for someone choosing where to live and wrong for someone citing us: a number quoted
in an article should still mean what it meant the day it was quoted.

So each edition is frozen to disk and carries a sha256 computed over its
own contents. Anyone can prove the numbers they cited are the numbers that were published.
Nothing in this repository is recomputed at read time.

## Verifying an edition

```sh
cd editions/2026 && sha256sum -c MANIFEST.sha256
```

## Citing

```
Nguyễn Thành Dân (2026). ThonRetire Retirement Index 2026. Frozen 2026-08. https://thonretire.com/edition/2026 — CC-BY-4.0
```

BibTeX keys are `thonretire-index-<year>` and never change, so a later edition arrives in
your reference manager as a new entry instead of overwriting the one you already filed.

## Corrections

Numbers here are assembled by hand from the page each government publishes. If one is
wrong, say so at https://thonretire.com/data — corrections land in the changelog carried inside every
edition file, with the date.
