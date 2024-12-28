# GlobalTemperatureAnalysis
Data Engineering Projekt zur Analyse globaler Temperaturdaten

## Projektübersicht
In diesem Projekt habe ich eine globale Temperaturdatensammlung analysiert und bereinigt. Die Daten wurden in eine SQL-Datenbank geladen und einer detaillierten Analyse unterzogen, um fehlende Werte zu identifizieren und mit verschiedenen Methoden zu behandeln. Ziel war es, die Daten zu bereinigen und nützliche Erkenntnisse über Temperaturtrends in verschiedenen Städten weltweit zu gewinnen.

## Datenquellen
Die Daten stammen von [Kaggle Global Temperature Data](https://www.kaggle.com), die historische Temperaturmessungen enthalten. Diese Daten wurden in eine SQL-Datenbank (Azure SQL) geladen und weiter verarbeitet.

## Datenstruktur
Die Tabelle `dbo.GlobalTempData` enthält folgende Spalten:

- `dt`: Datum der Temperaturmessung
- `AverageTemperature`: Durchschnittstemperatur
- `AverageTemperatureUncertainty`: Unsicherheit der Messung
- `City`: Stadt, in der die Messung durchgeführt wurde
- `Country`: Land der Stadt
- `Latitude`: Breitengrad
- `Longitude`: Längengrad

## Projektziele

1. **Datenbereinigung**: Entfernen von Duplikaten und Umgang mit fehlenden Werten.
2. **Datenanalyse**: Bereitstellung von Einblicken in Temperaturtrends und den Vergleich von Städten.
3. **Visualisierungen**: Erstellen von Graphen, die den Temperaturverlauf und Unterschiede zwischen den Städten zeigen.

## Struktur des Repositories

- `data/`: Enthält Rohdaten und bereinigte Daten
- `notebooks/`: Jupyter Notebooks mit Analysen und Visualisierungen
- `src/`: Python Skripte zur Datenpipeline
- `sql_queries/`: SQL-Skripte zur Datenbereinigung und Analyse
- `requirements.txt`: Python-Pakete, die benötigt werden

## Installation

1. Klone das Repository:
    ```bash
    git clone https://github.com/deinbenutzername/GlobalTemperatureAnalysis.git
    cd GlobalTemperatureAnalysis
    ```

2. Installiere die erforderlichen Python-Pakete:
    ```bash
    pip install -r requirements.txt
    ```

## Verwendung

- Die Daten können im Ordner `data/Processed_Data/` gefunden werden.
- Die SQL-Datenbank ist in `sql_queries/` beschrieben. Führe die SQL-Abfragen auf einer Azure SQL-Datenbank aus.
- Die Notebooks für die Datenbereinigung und Analyse befinden sich im `notebooks/`-Ordner.

## Lizenz
Dieses Projekt ist unter der MIT-Lizenz lizenziert.
