Fahrradwetter Blueprint (Sensor & Dashboard)

Dieses Paket erstellt ein Wetter-Panel für Radfahrer in Home Assistant. Es nutzt OpenWeatherMap und zeigt Temperatur, Wind & Regen für heute, morgen früh und morgen nachmittag.

## Installation

1. Öffne die ZIP-Datei
2. Ersetze `{{ lat }}`, `{{ lon }}`, `{{ api_key }}` in `sensor.yaml`
3. Setze Uhrzeiten `{{ morning_time }}` (z. B. `06`) und `{{ afternoon_time }}` (z. B. `15`)
4. Datei einfügen in `configuration.yaml` oder `sensor.yaml`
5. Füge das Dashboard YAML über die Benutzeroberfläche ein (z. B. als Button Card)
6. Neustarten!

## Benötigt

- OpenWeatherMap API Key
- Standort-Koordinaten
