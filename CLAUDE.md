# CLAUDE.md — thymply.de (Firmenseite)

Firmenseite von Thymply, eine einzige Datei `index.html` (Deutsch, ohne Build, ohne i18n-System). Projekt: Firmenebene, Sitzung `cc-firma`. Befunde und offene Punkte: `~/vault/00-Firma/Backlog.md` (F-004 bis F-010), Herkunft `~/vault/00-Firma/thymply-de-Quelle-2026-11-19.md`.

## Veröffentlichung
- Live-Seite: Domain thymply.de (und www), Cloudflare-Projekt `thymply-website`.
- Entscheidung Tim F-20261119-10 = A: thymply.de kommt seit 2026-11-19 aus dem Cloudflare-Projekt `thymply-website` (Workers Builds, mit diesem Repo verbunden). Jeder Push auf `main` geht live. Beleg: GitHub-Check „Workers Builds: thymply-website" auf `634527a` und `45a618f` mit `success`, thymply.de liefert danach den jeweiligen Stand.
- Das alte Pages-Projekt `thymply` (`thymply.pages.dev`) hängt nicht mehr an der Domain und bleibt auf dem Stand `aa6bb9b`. Löschen entscheidet Tim.
- `.assetsignore` schließt Dateien von der Auslieferung aus (z. B. `CLAUDE.md`). Neue Dateien, die nicht öffentlich sein sollen, dort eintragen und nach dem Deploy mit `curl -o /dev/null -w "%{http_code}"` auf 404 prüfen.
- Ein Push auf `main` ist damit ein Prod-Deploy der Firmenseite: Änderungen an Texten, Impressum oder Datenschutzerklärung nur nach Tims Ja (`~/vault/00-Firma/Regeln/ja-grenze.md`). Reine Technik ohne sichtbare Änderung gilt wie Code ändern.
- Cloudflare fügt am Ende jeder Antwort ein eigenes Skript ein. Vergleiche mit der Live-Seite ohne die letzte Zeile machen. Die Mail-Verschleierung (`/cdn-cgi/…email-decode`) war beim alten Pages-Projekt aktiv, über `thymply-website` am 2026-11-19 nicht mehr.

## Regeln
- Echte Umlaute (ä, ö, ü, ß), im Code gerade Anführungszeichen.
- Git: explizite Pfade, direkt auf `main` (`~/vault/00-Firma/Regeln/git.md`).
- Impressum und Datenschutzerklärung sind Rechtstexte: nie ohne Tims Ja ändern.
