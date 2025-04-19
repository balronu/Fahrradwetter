
# Fahrradwetter für Home Assistant

Dieses Paket enthält eine Wetteranzeige für Fahrradfahrer auf dem Home Assistant Dashboard. Es nutzt Daten von OpenWeatherMap und optional von einer lokalen Wetterstation (z. B. GW1100A).

## Inhalt

- `sensor_openweathermap_only.yaml`: Nur OpenWeatherMap-Daten
- `sensor_both.yaml`: Kombination aus lokaler Wetterstation und OpenWeatherMap
- `dashboard_card.yaml`: Button-Card für die Anzeige im Dashboard
- `screenshot.png`: Beispielansicht der Dashboard-Karte

## Einrichtung

1. **API-Key anpassen:**
   Ersetze `YOUR_OPENWEATHERMAP_API_KEY` in den YAML-Dateien durch deinen persönlichen API-Key von https://openweathermap.org/api.

2. **Sensoren einfügen:**
   Wähle entweder:
   - Nur `sensor_openweathermap_only.yaml`, wenn du keine lokale Wetterstation hast.
   - Oder `sensor_both.yaml`, wenn du z. B. eine Ecowitt/GW1100A Wetterstation betreibst.

   Die YAML-Dateien kannst du z. B. in deine `configuration.yaml` einbinden:
   ```yaml
   sensor: !include sensors/sensor_openweathermap_only.yaml
   ```

3. **Dashboard-Karte hinzufügen:**
   Füge den Inhalt aus `dashboard_card.yaml` als benutzerdefinierte Karte in dein Dashboard ein.
   Die `button-card` Custom Card muss installiert sein (z. B. über HACS).

## Beispielansicht

Siehe `screenshot.png` für eine visuelle Vorschau der fertigen Dashboard-Karte.
