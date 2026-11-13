# Dungeon 67 – Website

Statische, deutschsprachige Website für Cloudflare Pages mit bearbeitbaren Inhalten in `content/site.json`.

## GitHub

Repository `dungeon67-website` öffnen → **Add file → Upload files**. ZIP lokal entpacken und **alle Inhalte des Ordners** (einschliesslich `.pages.yml`) ins Repository-Stammverzeichnis hochladen. GitHub-Webupload kann versteckte Dateien übersehen; `.pages.yml` gegebenenfalls über **Add file → Create new file** separat anlegen und Inhalt einfügen.

## Cloudflare Pages

Workers & Pages → Create → Pages → Connect to Git → GitHub-Repository auswählen.
- Framework preset: None
- Build command: leer lassen
- Build output directory: `/` (oder `.` wenn die Oberfläche dies verlangt)
- Root directory: Repository-Stammverzeichnis

Die Seite läuft zunächst auf einer `*.pages.dev`-Adresse. Domain/DNS erst später verbinden.

## Pages CMS

Auf https://pagescms.org/ mit GitHub anmelden und das Repository auswählen. Die Datei `.pages.yml` im Repository-Stammverzeichnis beschreibt die bearbeitbaren Felder. Änderungen im CMS werden als Git-Commits gespeichert und lösen bei Cloudflare einen neuen Deploy aus. CMS-Integration nach erstem Deploy testen; Feldschema ggf. an die aktuelle Pages-CMS-Version anpassen.

## Inhalte ändern

- `content/site.json`: Club, Angebote, Events, Links, FAQ und Kontakt.
- `assets/style.css`: Design.
- `index.html`: Grundgerüst.

**Vor Veröffentlichung ergänzen:** Kontakt-E-Mail, echte Social-/Buchungslinks, endgültige Preise, Logo, eigene Fotos, Datenschutzhinweise und gegebenenfalls Impressum. Es sind absichtlich keine erfundenen Links oder Kontaktdaten enthalten.

**Hinweis:** Das öffentliche GitHub-Repository enthält nur öffentliche Website-Inhalte. Keine Passwörter, internen Telefonnummern oder vertraulichen Daten hochladen.
