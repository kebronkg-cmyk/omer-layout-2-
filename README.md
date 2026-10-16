# Lockschuppen Die Friseure: Designkonzept

Unverbindlicher Entwurf für eine neue Website von **Lockschuppen Die Friseure** (Aubing, Sendling, Fürstenried, Starnberg).
Keine offizielle Website des Betriebs. Alle Seiten sind für Suchmaschinen gesperrt (`noindex`). Termine laufen wie bisher per Telefon, alle Knöpfe wählen die echte Nummer des Salons.

Vorschau: https://kebronkg-cmyk.github.io/omer-layout-2-/

## Aufbau
- `index.html`: Startseite mit 3D-Strähnen, Salon-Ring mit Fotos aus allen vier Salons, Übersicht mit Stadtplan, Leistungen, Einblicke
- `<salon>/index.html`: je Salon eine Seite mit Glasschrift, Öffnungszeiten, Route, Stadtplan, Schema.org `HairSalon`
- `hinweis/`: Hinweis zum Konzept, Quellen, Link zum Impressum des Betriebs

Leitfarbe ist das Grün der Salonwände.

## Bauen
```
python3 tools/thema.py              # Markenfarbe auf das Grunddesign
python3 tools/bilder.py <originale> # Fotos zuschneiden, behutsam hochrechnen, WebP
python3 tools/karten.py             # Stadtpläne aus OpenStreetMap
python3 tools/build.py              # Seiten aus tools/daten.json
```

## Offen, vom Betrieb bestätigen lassen
- Aubing: Mainaustraße 52 oder Radolfzeller Straße 15 (die alte Seite nennt beides)
- Starnberg: Öffnungszeiten (Salonseite Di bis Fr 9 bis 18 Uhr, Kontaktseite Mo bis Fr 9 bis 19 Uhr)
- Fotos in voller Größe (die alte Seite hat nur 659 px), Preise, Team
