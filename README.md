Fahrradwetter Dashboard (Home Assistant)



Dieses Projekt zeigt eine schöne, einfache Dashboard-Karte in Home Assistant, um das Wetter fürs Fahrradfahren anzuzeigen.

Varianten

Es gibt zwei Varianten für die Nutzung:

1. Nur OpenWeatherMap-Daten verwenden

Für Benutzer ohne eigene Wetterstation.

Datei: sensor_openweathermap_only.yaml

2. OpenWeatherMap + lokale Wetterstation kombinieren

Für Benutzer mit einer eigenen Wetterstation (z. B. GW1100A).

Datei: sensor_both.yaml

Einrichtung

1. Sensor-Datei auswählen

Füge eine der YAML-Dateien in deine Home Assistant configuration.yaml ein oder verwende sie über die sensor:-Konfiguration.

Benenne sie ggf. um in sensor.yaml, falls du mehrere Dateien nutzt.

2. Koordinaten und API-Key eintragen

In der gewählten Datei musst du Folgendes ersetzen:

lat=YOUR_LATITUDE
lon=YOUR_LONGITUDE
appid=YOUR_API_KEY

YOUR_LATITUDE: z. B. 52.52 für Berlin

YOUR_LONGITUDE: z. B. 13.41 für Berlin

YOUR_API_KEY: deinen API-Key von https://openweathermap.org/api

3. Dashboard-Karte hinzufügen

Verwende den Code aus der Datei dashboard_button_card.yaml, um eine schöne Visualisierung im Dashboard zu erhalten.

Die Karte verwendet das Plugin button-card. Stelle sicher, dass du es über HACS oder manuell installiert hast: https://github.com/custom-cards/button-card

Beispielanzeige

Die Karte zeigt drei Zeitpunkte an:

Aktuelles Wetter (ggf. von deiner Wetterstation)

Morgen um 06:30 Uhr

Morgen um 16:00 Uhr

Für jeden Zeitpunkt siehst du:

Temperatur

Windgeschwindigkeit

Regenmenge

Eine simple Bewertung (✅ Gut / ❌ Schlecht)

Lizenz

MIT License

