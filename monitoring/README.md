<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Beobachtung: was gelesen wird und was daraus folgte

[English](README.en.md)

Wie global-law jedes Land beobachtet: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Diese Seite zeigt dasselbe nur für Obwalden: jedes Lesen einer amtlichen Quelle, wann, und was daraus folgte (Vorschriften hinzugefügt, geändert und entfernt). Maschinenlesbar in [data/checks/](../data/checks/) (JSON Lines, Schema `lexifina-check/1`), in `git log` als Commits mit `Kind: check` und Monat für Monat in [checks/](checks/).

**Letzte Prüfung:** 2026-11-27 06:39 UTC, Obwalden: Systematische Sammlung (gdb.ow.ch): 135 Adressen gelesen; 0 hinzugefügt, 0 geändert, 0 entfernt; keine Änderung; 108 nicht veröffentlicht, davon 0 ohne Grund.

## Quellen

| Quelle | Ordner | Wie oft | Letzte erfolgreiche Prüfung | Letztes Ergebnis | Stand |
| --- | --- | --- | --- | --- | --- |
| [Obwalden: Systematische Sammlung (gdb.ow.ch)](https://gdb.ow.ch/) | `<act>/` | täglich | 2026-11-27 06:39 UTC | keine Änderung | beobachtet |

## Die letzten 30 Tage

| Beginn (UTC) | Quelle | Gelesen | Hinzugefügt | Geändert | Entfernt | Nicht veröffentlicht (ohne Grund) | Ergebnis | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-27 06:36](checks/2026-11.md#ch-lexwork-obwalden-20261127t063641z) | lexwork-obwalden | 135 | 0 | 0 | 0 | 108 (0) | keine Änderung | — |
| [2026-11-26 06:35](checks/2026-11.md#ch-lexwork-obwalden-20261126t063505z) | lexwork-obwalden | 160 | 0 | 0 | 0 | 110 (0) | keine Änderung | — |
| [2026-11-25 07:23](checks/2026-11.md#ch-lexwork-obwalden-20261125t072346z) | lexwork-obwalden | 262 | 80 | 0 | 0 | 107 (0) | Änderungen gefunden | [107](https://github.com/lexifina/switzerland-obwalden-law/compare/2c22f4e77188...6d90aa17b21a) |
| [2026-11-24 12:13](checks/2026-11.md#ch-lexwork-obwalden-20261124t121334z) | lexwork-obwalden | 275 | 230 | 0 | 0 | 163 (0) | Änderungen gefunden | [160](https://github.com/lexifina/switzerland-obwalden-law/compare/45788458216b...e24b87ba08b5) |

## Selbst prüfen

```
python tools/checktrail.py                      # die letzte Prüfung jeder Quelle
python tools/checktrail.py --day 2026-11-23     # jede Prüfung eines Tages
python tools/checktrail.py --act <id>           # wann eine Vorschrift gesehen und veröffentlicht wurde
git log --grep='^Kind: check' --format='%ci %s'  # die Prüfungen in der Historie
```

Rechtskraft hat nur die amtliche Verkündung; die Texte hier sind Kopien zum Lesen und Suchen.
