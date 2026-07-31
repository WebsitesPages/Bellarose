# BELLAROSE HAIRSALON

Statische Website für den Friseursalon Bellarose, Kaulbachstraße 36, 80539 München.
Eine Datei, kein Build-Schritt, Auslieferung über GitHub Pages.

## Aufbau

```
index.html          gesamte Startseite (HTML, CSS und JS in einer Datei)
recht.css           Blatt für Impressum und Datenschutz
impressum/          Impressum — ENTWURF, siehe Markierungen auf der Seite
datenschutz/        Datenschutz — ENTWURF, siehe Markierungen auf der Seite
bilder/             Salonfotos (JPG)
fonts/              Bodoni Moda und Jost als WOFF2, lokal eingebunden
.nojekyll           schaltet die Jekyll-Verarbeitung von GitHub Pages ab
```

## Pflegen

**Preise** stehen im Array `PRICES` in `index.html`. Zahlen unter `p` sind
`[S, M, L]` nach Haarlänge, `fix` ist ein fester Preis, `from` ein Ab-Preis.

**Öffnungszeiten** stehen im Array `HOURS`. Bei Änderung auch das
`openingHoursSpecification` im JSON-LD im `<head>` nachziehen.

**Bilder** liegen in `bilder/`. Die Hausgradation (warme Angleichung an die
Champagner-Palette) passiert per CSS über die Klasse `.pic` — die Dateien
selbst sind unverändert.

## Vor dem Livegang noch offen

- [ ] Impressum vervollständigen — Rechtsform, Vertretungsberechtigter,
      Handwerkskammer, E-Mail. Ohne das ist die Seite abmahnfähig.
- [ ] Datenschutzerklärung prüfen lassen; AV-Vertrag mit GitHub abschließen
- [ ] Echte E-Mail-Adresse einrichten und die Platzhalter ersetzen
- [ ] Gründungsjahr im Abschnitt „Der Salon" prüfen (steht auf 2019)
- [ ] Preisstand aktualisieren (steht auf Juli 2026)
- [ ] Bildrechte klären, Einwilligung fürs Teamporträt dokumentieren
- [ ] Höher aufgelöste Fotos vom Fotografen — aktuell nur 720 px breit
- [ ] Echte Vorher/Nachher-Bilder von Farbergebnissen für „Im Salon"
- [ ] Optional: Frames nach `frames/` legen (`hair-001.webp` …), dann wird
      die Standbild-Bühne automatisch zur scrollgesteuerten Sequenz
