# 🚀 Zeitreihen- und Trendanalyse von Grundwasserständen in Nordrhein-Westfalen (2010–2019)

In diesem Projekt werden Grundwasserstandsdaten aus Nordrhein-Westfalen für den Zeitraum 2010–2019 mithilfe von Zeitreihen- und Trendanalysen ausgewertet. Ziel ist es, langfristige Entwicklungen des Grundwasserspiegels zu identifizieren und räumlich vergleichbar darzustellen.

## 📊 Projektübersicht

**Problemstellung:**  
In den vergangenen Jahrzehnten ist die Diskussion um die globale Erwärmung zunehmend in den öffentlichen Fokus gerückt. Auch in Deutschland lassen sich die Auswirkungen dieses Phänomens mittlerweile deutlich messen. Damit einhergehend werden in vielen Regionen rückläufige Niederschläge beobachtet, wobei insbesondere das extreme Dürrejahr 2018 hervorzuheben ist. Als Folge der geringeren Niederschlagsmengen ist in weiten Teilen Deutschlands eine Absenkung des Grundwasserspiegels festzustellen. Neben klimatischen Einflüssen trägt auch die zunehmende Nutzung des Grundwassers als Trink- und Brauchwasserressource zur Belastung der Grundwasservorkommen bei. Dank des gut ausgebauten Grundwassermessstellennetzes in Deutschland lässt sich diese Entwicklung zuverlässig erfassen.
<!-- Beschreibe das Problem, das du lösen möchtest -->

**Ziel:**  
Ziel dieses Projekts ist es, den übergeordneten Trend der Grundwasserstandsentwicklung in Nordrhein-Westfalen während der Wasserwirtschaftsjahre 2010 bis 2019 zu untersuchen. Im Fokus steht die Frage, ob sich infolge klimatischer Veränderungen sowie einer teilweise erhöhten Nutzung des Grundwassers messbare Änderungen der Grundwasserstände feststellen lassen und in welchem Ausmaß diese auftreten. Abschließend soll die räumliche Verteilung der Grundwasserstandsänderungen mithilfe eines Geoinformationssystems analysiert und visualisiert werden.
<!-- Was ist das Hauptziel deines Projekts? -->

**Methoden:** 
* Explorative Datenanalyse (EDA)
* Zeitreihenanalyse
* Lineare Regression
* räumliche Analyse in QGIS (Postprocessing)
<!-- Welche Techniken/Algorithmen verwendest du? -->

## 🪃 Datenquelle

Die Rohdaten stammen aus dem OpenHygrisC-Projekt des Bundeslandes Nordrhein-Westfalen. OpenHygrisC bezeichnet ein offenes Datenset mit Grundwasserdaten, das im Rahmen der Open-Data-Initiativen des Landes zur frei verfügbaren Nutzung bereitgestellt wird – und wird u. a. für Bildung, Forschung und Umweltanalysen genutzt.  
  
https://www.opengeodata.nrw.de/produkte/umwelt_klima/wasser/grundwasser/hygrisc/  
  
OpenHygrisC ist ein offener Datensatz mit Messwerten aus der Grundwasser-Überwachung von Nordrhein-Westfalen. Diese Daten umfassen chemische Messwerte, Wasserstände und Informationen zu Messstellen über viele Jahre. Die Daten werden auf dem Portal OpenGeodata.NRW veröffentlicht, unter der Lizenz „Datenlizenz Deutschland – Zero (DL-DE-Zero)“, was bedeutet, dass sie ohne Einschränkungen frei verwendet werden können (auch für kommerzielle und wissenschaftliche Zwecke).  
Nähere Informationen finden Sie [hier](docs/data_source.md).

## ⚙ Setup

Klone das Repository
```bash
# Repository klonen
git clone [DEIN-REPO-LINK]
cd [REPO-NAME]
```

Installiere [uv](https://uv.dev) (falls noch nicht installiert) und synchronisiere die Abhängigkeiten
```bash
# Dependencies installieren
uv sync
```

### Ausführung

Notebooks in dieser Reihenfolge ausführen:
1. notebooks/01_reading_cleaning.ipynb
2. notebooks/02_analysis_slope_per_year.ipynb
3. notebooks/03_analysis_total_trend.ipynb
4. notebooks/04_visualization_slope_per_year.ipynb
5. notebooks/05_visualization_total_trend.ipynb
<!--
2. notebooks/02_preprocessing.ipynb
3. notebooks/03_modeling.ipynb
4. notebooks/04_results.ipynb
-->


