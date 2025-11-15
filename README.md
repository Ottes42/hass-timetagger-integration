# TimeTagger – Home Assistant Integration

Dieses Custom Component integriert die [TimeTagger](https://timetagger.app)-API in Home Assistant
und stellt mehrere Sensoren bereit:

- `sensor.arbeitszeit_heute`
- `sensor.arbeitszeit_diese_woche`
- `sensor.arbeitszeit_diesen_monat`
- `sensor.restzeit_diese_woche`
- `sensor.monats_saldo_arbeitszeit`

Alle Entitäten erscheinen unter einem Gerät **„TimeTagger“**.

## Installation über HACS

1. HACS öffnen
2. „Custom Repositories“ öffnen
3. Dieses Repository hinzufügen, z. B.:

   ```text
   https://github.com/Ottes42/hass-timetagger-integration
Kategorie: Integration

Danach unter Einstellungen → Geräte & Dienste → Integration hinzufügen
nach TimeTagger suchen und konfigurieren:

API URL (z. B. https://dein-host/timetagger/)

API Token

Work-Tags (z. B. #work)

Tägliche Sollstunden (Standard: 8)

Verwendung
Nach der Einrichtung stehen im TimeTagger-Gerät u. a. folgende Sensoren zur Verfügung:

Arbeitszeit heute – Summe aller TimeTagger-Records heute (in Stunden)

Arbeitszeit diese Woche – Summe aller Records seit Wochenbeginn (Montag)

Arbeitszeit diesen Monat – Summe aller Records seit Monatsbeginn

Restzeit diese Woche – (Sollstunden bis heute) minus (gearbeitete Stunden)

Monats-Saldo Arbeitszeit – Über-/Minusstunden diesen Monat

Diese Sensoren eignen sich ideal für:

ApexCharts (Wochenbalken + kumulierte Überstundenlinie)

Automationen („Feierabend, wenn Restzeit diese Woche <= 0“)

Dashboards für Arbeitszeit-/Überstundenkontrolle

Roadmap
Weitere Sensoren (Deep Work, Homeoffice/Office per Tagging)

Unterstützung für mehrere Profile / Tag-Sets

Blueprint-Beispiele für ApexCharts

Support
Issues und Feature Requests gern über GitHub-Issues.

sql
Code kopieren
