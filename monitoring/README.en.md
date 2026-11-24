<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Deutsch](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Obwalden only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-24 12:23 UTC, Obwalden: systematic collection (gdb.ow.ch): 275 addresses read; 230 added, 0 changed, 0 removed; changes found; 163 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Obwalden: systematic collection (gdb.ow.ch)](https://gdb.ow.ch/) | `<act>/` | daily | 2026-11-24 12:23 UTC | changes found | watched |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-24 12:13](checks/2026-11.md#ch-lexwork-obwalden-20261124t121334z) | lexwork-obwalden | 275 | 230 | 0 | 0 | 163 (0) | changes found | [160](https://github.com/lexifina/switzerland-obwalden-law/compare/45788458216b...e24b87ba08b5) |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
