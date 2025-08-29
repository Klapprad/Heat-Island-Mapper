# Heat-Island-Mapper
Mapping and analyzing urban heat islands using open data, geospatial analysis, and scenario simulations for greener, fairer cities.

Heat Island Mapper ist ein datengetriebenes Tool, das Urban Heat Islands in Städten sichtbar macht und quantifiziert.
Es kombiniert offene Datenquellen (OpenStreetMap, Wetter- und Klimadaten, Satellitenbilder) mit Geoanalyse und Machine Learning, um:

    Hitzebelastung in verschiedenen Stadtteilen zu kartieren,
    den Einfluss von Flächennutzung (z. B. Parkplätze vs. Grünflächen) auf die Temperaturen zu analysieren,
    Szenarien für Entsiegelung, Begrünung und Flächengerechtigkeit zu simulieren.

Die Ergebnisse werden in einem interaktiven Dashboard und Karten visualisiert und bieten so sowohl Bürger:innen als auch Stadtplaner:innen ein Werkzeug, um nachhaltigere Entscheidungen zu treffen.



###################################

## Geplante Features
- **Urban Heat Mapping**: Visualisierung von Temperatur-Hotspots im Stadtgebiet.  
- **Geo-Datenintegration**: Nutzung offener Quellen wie OSM, Wetterstationen, Satellitenbildern.  
- **Flächengerechtigkeit**: Analyse, wie städtischer Raum (Autos, Menschen, Grünfläche) verteilt ist und deren Einfluss auf die Bildung von Urban Heat Islands.  
- **Szenario-Simulationen**: Temperaturveränderungen bei Umwidmung von Flächen (z. B. Parkplatz zu Grünfläche).  
- **Interaktive Visualisierung**: Karten, Dashboards und Diagramme mit *Streamlit* oder *Dash*.  

## Datenquellen & API Key
- [OpenStreetMap](https://www.openstreetmap.org/) – Straßen, Gebäude, Parkflächen, Landnutzung  
- [DWD OpenData](https://opendata.dwd.de/) oder [Open-Meteo](https://open-meteo.com/) – Wetter- und Klimadaten  
- [Copernicus / Sentinel-2](https://scihub.copernicus.eu/) – Vegetation (NDVI), Landbedeckung  
- [Städtische OpenData-Portale] (falls vorhanden, z. B. Baumkataster, Parkzonen)  
- OpenWeather historical 


## Installation

- Python 3.10+  
- PostgreSQL mit [PostGIS](https://postgis.net/) (für Geodaten)  

```bash
git clone https://github.com/USERNAME/heat-island-mapper.git
cd heat-island-mapper

# Python-Env
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
