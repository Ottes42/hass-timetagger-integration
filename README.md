# TimeTagger – Home Assistant Integration

Dieses Custom Component integriert die TimeTagger-API in Home Assistant und stellt mehrere Sensoren bereit:

- Arbeitszeit heute
- Arbeitszeit diese Woche
- Arbeitszeit diesen Monat
- Restzeit diese Woche
- Monats-Saldo Arbeitszeit

Alle Entitäten erscheinen sauber unter einem Gerät "TimeTagger".

## Installation über HACS

1. HACS öffnen
2. „Custom Repositories“
3. Repo hinzufügen: 
    https://github.com/ottes/ottes-ha-timetagger 
    Kategorie: **Integration**
4. Danach unter „Integrationen → TimeTagger“ konfigurieren:
- API URL
- API Token
- Tags (z. B. `#work`)
- Tägliche Sollstunden

## Beispiel: TimeTagger Instanz

Der API-Endpoint sieht typischerweise so aus:
https://dein-host/timetagger/api/v2/records

Für Cloudinstanzen noch ungestestet!

## Features

- DataUpdateCoordinator für effiziente API-Abfragen
- Gerätestruktur für alle Sensoren
- UI-Konfiguration per Config Flow
- Aggregationen für heute, Woche, Monat

## ToDo / Roadmap

- Deepwork-Sensoren
- Homeoffice/Office-Erkennung
- Krankheit/Urlaub getrennt auswerten
- ApexCharts-Blueprints

## Support

Issues willkommen:  
https://github.com/ottes/ottes-ha-timetagger/issues