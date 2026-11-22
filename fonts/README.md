# Selbst gehostete Schriften (thymply.de)

Die Seite lädt ihre Schriften nur von hier (`/fonts/…`), nicht von Google (F-005, 2026-11-19). Eingebunden per `@font-face` im `<style>`-Block von `index.html`.

| Familie | Genutzte Schnitte | Dateien | Lizenz | Lizenzdatei | Urheber laut Lizenz |
|---|---|---|---|---|---|
| DM Sans | 300, 400, 500 (variable Datei) | `DMSans-latin.woff2`, `DMSans-latin-ext.woff2` | SIL Open Font License 1.1 | `OFL-DMSans.txt` | The DM Sans Project Authors (2014) |
| Sora | 600 | `Sora-latin.woff2`, `Sora-latin-ext.woff2` | SIL Open Font License 1.1 | `OFL-Sora.txt` | The Sora Project Authors (2019) |
| Syne | 700 | `Syne-latin.woff2`, `Syne-latin-ext.woff2` | SIL Open Font License 1.1 | `OFL-Syne.txt` | The Syne Project Authors (2017) |

Die OFL 1.1 erlaubt Nutzung, Einbettung und Weitergabe, auch gewerblich, wenn der Lizenztext beiliegt. Keine der drei Schriften hat einen Reserved Font Name (erste Zeile der Lizenzdateien). `METADATA.pb` im offiziellen Repo nennt für alle drei `license: "OFL"`.

## Quelle

- **Schriftdateien:** Google Fonts, CSS2-API mit aktuellem Browser-User-Agent, abgerufen am 2026-11-19:
  `https://fonts.googleapis.com/css2?family=Sora:wght@600&family=Syne:wght@700&family=DM+Sans:wght@300;400;500&display=swap`.
  Übernommen sind die Subsets `latin` (enthält ä, ö, ü, ß) und `latin-ext` mit der `unicode-range` aus der Antwort; `greek` von Syne nicht. Die Dateien von `fonts.gstatic.com` sind unverändert und nur umbenannt. Versionen laut URL: dmsans v17, sora v17, syne v24.
- **Lizenztexte:** github.com/google/fonts, Commit `7af0d90b4d532ffa4b041937b560c6df4e7b1e95`, Pfade `ofl/dmsans/OFL.txt`, `ofl/sora/OFL.txt`, `ofl/syne/OFL.txt`, unverändert.

## sha256

```
a5d38fe99f930275684999b462c7123faa063d9e44e73b4b241723d884aa0f49  DMSans-latin-ext.woff2
9fea608a947e67020c33cad9a6fe3d60c54119dfb8cff87768a8117a15ed7543  DMSans-latin.woff2
2c17a94fef4242d1c33ffcc9bb43c7eb93ad88db53409c1067ac23cc914523e2  Sora-latin-ext.woff2
fa9ab76f30510ad92153c6d6d72d0508884b85e9f0148abdfa963231b2a4845a  Sora-latin.woff2
f1c45224922ef9247ef025b780abff888af301b4b1bd251d11997bd0a3ab3178  Syne-latin-ext.woff2
0aad69416fc0ccf6f340647c46e759d5c6e4628d92576b279ec5ada0afbd9d35  Syne-latin.woff2
```
