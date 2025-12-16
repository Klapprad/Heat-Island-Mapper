# Urban Heat
Scope: Urban Heat Islands in Städten sichtbar macht und quantifiziert.
Es kombiniert offene Datenquellen (OpenStreetMap, Wetter- und Klimadaten, Satellitenbilder) mit Geoanalyse und Machine Learning, um:

- **Hitzebelastung in verschiedenen Stadtteilen kartieren**
- **Einfluss von Flächennutzung (z. B. Parkplätze vs. Grünflächen) auf die Temperaturen zu analysieren**
- **Szenarien für Entsiegelung, Begrünung und Flächengerechtigkeit zu simulieren**

Idee: Die Ergebnisse in einem interaktiven Dashboard und Karten zu visualisierren. Im Hinblick auf Flächengerechtigkeit
- Visualisierung von Temperatur-Hotspots im Stadtgebiet
- Nutzung offener Quellen wie OSM, Wetterstationen, Satellitenbildern
- Analyse, wie städtischer Raum (Autos, Menschen, Grünfläche) verteilt ist und deren Einfluss auf die Bildung von Urban Heat Islands  
- Temperaturveränderungen bei Umwidmung von Flächen (z. B. Parkplatz zu Grünfläche)

## SRC
- [OpenStreetMap](https://www.openstreetmap.org/) -> Straßen, Gebäude, Parkflächen, Landnutzung  
- [DWD OpenData](https://opendata.dwd.de/) oder [Open-Meteo](https://open-meteo.com/) -> Wetter- und Klimadaten  
- [Copernicus / Sentinel-2](https://scihub.copernicus.eu/) -> Vegetation (NDVI), Landbedeckung  
- [Städtische OpenData-Portale] (Baumkataster, Parkzonen)  
- OpenWeather historical

## Stand und Aktueller Befund
Ähnliche Abkühlungsraten wischen den Locations (im Beriech von -4.5°C und -4.2°C) und nur geringe Temperaturunterschiede (~0.2°C Spanne zwischen 17.92°C und 18.11°C). 

Interpretation die Locations in Mannheim sind thermisch sehr homogen. Kein ausgeprägter Urban Heat Island Effekt zwischen den Stadtteilen, alle Standorte haben ähnliche nächtliche Bedingungen. Die gesehenen Unterschiede sind praktisch nicht relevant (< 0.2°C)

ANOVA Test: Nächtliche Temperaturen zwischen Locations
============================================================
F-Statistik: 0.226
p-Wert: 0.923691
→ Keine signifikanten Unterschiede (p ≥ 0.05)

Next: Oberflächentemperaturen höher auflösen im Bereich von wenigen Metern um Unterschiede besser zu sehen. Vielleicht Fokus auf zeitliche Muster (Hitzewellen, Tropennächte) um Daten/requests zu verschlanken.


