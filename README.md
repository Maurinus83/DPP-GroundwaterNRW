# 🚀 Trend- und Zeitreihenanalyse von Grundwasserständen in Nordrhein-Westfalen 2010 – 2019

In diesem Projekt werden Grundwasserstandsdaten aus Nordrhein-Westfalen für den Zeitraum 2010 – 2019 mithilfe von Trend- und Zeitreihenanalysen ausgewertet. Ziel ist es, langfristige Entwicklungen der Grundwasserstände zu identifizieren und räumlich vergleichbar darzustellen.

## 📊 Projektübersicht

**Problemstellung:**  
In den vergangenen Jahrzehnten ist die Diskussion um die globale Erwärmung zunehmend in den öffentlichen Fokus gerückt. Auch in Deutschland lassen sich die Auswirkungen dieses Phänomens mittlerweile deutlich messen. Damit einhergehend werden in vielen Regionen rückläufige Niederschläge beobachtet, wobei insbesondere das extreme Dürrejahr 2018 hervorzuheben ist. Als Folge der geringeren Niederschlagsmengen ist in weiten Teilen Deutschlands eine Absenkung des Grundwasserspiegels festzustellen. Neben klimatischen Einflüssen trägt auch die zunehmende Nutzung des Grundwassers als Trink- und Brauchwasserressource zur Belastung der Grundwasservorkommen bei. Dank des gut ausgebauten Grundwassermessstellennetzes in Deutschland lässt sich diese Entwicklung zuverlässig erfassen.
<!-- Beschreibe das Problem, das du lösen möchtest -->

**Ziel:**  
Ziel dieses Projekts ist es, den übergeordneten Trend der Grundwasserstandsentwicklung in Nordrhein-Westfalen während der Wasserwirtschaftsjahre 2010 bis 2019 zu untersuchen. Im Fokus steht die Frage, ob sich infolge klimatischer Veränderungen sowie einer teilweise erhöhten Nutzung des Grundwassers messbare Änderungen der Grundwasserstände feststellen lassen und in welchem Ausmaß diese auftreten. Abschließend soll die räumliche Verteilung der Grundwasserstandsänderungen mithilfe eines Geoinformationssystems analysiert und visualisiert werden.
<!-- Was ist das Hauptziel deines Projekts? -->

**Methoden:** 
* Explorative Datenanalyse (EDA)
* Lineare Regression
* Zeitreihenanalyse
* räumliche Visualisierung in QGIS (Postprocessing)
<!-- Welche Techniken/Algorithmen verwendest du? -->

## 🪃 Datenquelle

Die Rohdaten stammen aus dem OpenHygrisC-Projekt des Bundeslandes Nordrhein-Westfalen. OpenHygrisC ist ein offener Datensatz mit Messwerten aus der Grundwasserüberwachung in Nordrhein-Westfalen. Er umfasst unter anderem Informationen zu Messstellen, Wasserständen sowie chemischen Messwerten über einen langen Zeitraum.

Die Daten werden im Rahmen der Open-Data-Initiativen des Landes über die offene Geodateninfrastruktur OpenGeodata.NRW veröffentlicht und von der Landesverwaltung Nordrhein-Westfalen betrieben und gepflegt. Sie stehen unter der Lizenz „Datenlizenz Deutschland – Zero (DL-DE-Zero)“ und können damit uneingeschränkt, auch für wissenschaftliche, kommerzielle und nicht kommerzielle Zwecke, genutzt werden.
  
https://www.opengeodata.nrw.de/produkte/umwelt_klima/wasser/grundwasser/hygrisc/  
    
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

Die Notebooks 06 und 07 werden ausschließlich zur Erläuterung und Präsentation der Ergebnisse verwendet und enthalten keinen ausführbaren Quellcode.  

* notebooks/06_spatial_representation_qgis.ipynb
* notebooks/07_powerpoint presentation.ipynb


