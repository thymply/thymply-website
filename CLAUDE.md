# CLAUDE.md — thymply.de (Firmenseite)

Firmenseite von Thymply, eine einzige Datei `index.html` (Deutsch, ohne Build, ohne i18n-System). Projekt: Firmenebene, Sitzung `cc-firma`. Befunde und offene Punkte: `~/vault/00-Firma/Backlog.md` (F-004 bis F-010), Herkunft `~/vault/00-Firma/thymply-de-Quelle-2026-11-19.md`.

## Veröffentlichung
- Live-Seite: Cloudflare-Pages-Projekt `thymply` (`thymply.pages.dev`), Domain thymply.de.
- Entscheidung Tim F-20261119-10 = A: Das Pages-Projekt `thymply` ist seit 2026-11-19 mit diesem Repo verbunden. Jeder Push auf `main` geht live. Beleg: GitHub-Check „Cloudflare Pages" (App `cloudflare-workers-and-pages`) auf `aa6bb9b` mit `success`; thymply.de und `thymply.pages.dev` liefern danach genau `index.html` aus dem Repo.
- Ein Push auf `main` ist damit ein Prod-Deploy der Firmenseite: Änderungen an Texten, Impressum oder Datenschutzerklärung nur nach Tims Ja (`~/vault/00-Firma/Regeln/ja-grenze.md`). Reine Technik ohne sichtbare Änderung gilt wie Code ändern.
- Cloudflare schreibt auf thymply.de die Mailadressen um (`/cdn-cgi/…email-decode`). Das steht nicht in der Quelle; Vergleiche mit der Live-Seite gegen `thymply.pages.dev` machen.

## Regeln
- Echte Umlaute (ä, ö, ü, ß), im Code gerade Anführungszeichen.
- Git: explizite Pfade, direkt auf `main` (`~/vault/00-Firma/Regeln/git.md`).
- Impressum und Datenschutzerklärung sind Rechtstexte: nie ohne Tims Ja ändern.
