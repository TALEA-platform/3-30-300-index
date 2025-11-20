# 3-30-300 Index
**Version in italiano qui → [Italian version](#versione-italiana)**

## English Version

## Introduction
This repository provides tools, data, and workflows to compute the **3-30-300 index**, an indicator designed to assess urban green accessibility through three core components:

- **3** → proximity to a minimum number of trees around residential buildings
- **30** → at least 30% tree canopy coverage within each statistical area
- **300** → access to parks or gardens within 300 meters from buildings

The model generates indicators at both building and statistical-area levels, supporting analyses on urban fragility, environmental quality, proximity to green spaces, and climate-adaptation strategies.

## Main Features
- Extraction of buildings and road networks from OpenStreetMap
- Calculation of distance between buildings and trees/parks
- Measurement of canopy coverage across areas
- Evaluation of the three 3-30-300 criteria
- Aggregation into final indicators at statistical-area scale
- Export of results for mapping, dashboards, and further analyses

## Repository Structure
```
3-30-300-index/
│
├── data/                # Input datasets
├── notebooks/
│   └── 3_30_300index_and_clusters.ipynb
├── src/                 # Modular scripts
├── outputs/             # Final results (CSV, GeoJSON, maps)
└── README.md
```

## Requirements
- Python 3.10+
- Key packages:
  - geopandas
  - osmnx
  - shapely
  - pandas / numpy
  - rasterio
  - scikit-learn (optional analyses)
  - matplotlib / seaborn

Install dependencies with:
```bash
pip install -r requirements.txt
```

## Getting Started
1. Clone the repository:
```bash
git clone https://github.com/TALEA-platform/3-30-300-index
cd 3-30-300-index
```
2. Open the main notebook:
```
notebooks/3_30_300index_and_clusters.ipynb
```
3. Configure data paths in the first notebook cells
4. Run all sections to generate indicators

## Outputs
- **3_30_300_stat_areas.csv** – 3-30-300 indicators for each statistical area

---

# Versione italiana

## Introduzione
Questo repository contiene strumenti, dati e workflow per calcolare l’indice **3-30-300**, un indicatore che misura l’accessibilità al verde urbano attraverso tre dimensioni principali:

- **3** → prossimità a un numero minimo di alberi intorno agli edifici residenziali
- **30** → copertura arborea (canopy) pari ad almeno il 30% dell’area considerata
- **300** → accesso a parchi o giardini entro 300 metri dagli edifici

Il modello produce indicatori sia a livello di edificio che a livello di area statistica, utili per analizzare fragilità urbana, qualità ambientale, prossimità agli spazi verdi e strategie di adattamento climatico.

## Funzionalità principali
- Estrazione di edifici e rete stradale da OpenStreetMap
- Calcolo della distanza tra edifici, alberi e parchi
- Misura della copertura arborea (canopy)
- Valutazione dei tre criteri del modello 3-30-300
- Aggregazione degli indicatori a livello di area statistica
- Esportazione dei risultati per mappe, dashboard o analisi successive

## Struttura del repository
```
3-30-300-index/
│
├── data/                # Dati di input
├── notebooks/
│   └── 3_30_300index_and_clusters.ipynb
├── src/                 # Script modulari
├── outputs/             # Risultati finali (CSV, GeoJSON, mappe)
└── README.md
```

## Requisiti
- Python 3.10+
- Pacchetti principali:
  - geopandas
  - osmnx
  - shapely
  - pandas / numpy
  - rasterio
  - scikit-learn
  - matplotlib / seaborn

Installazione:
```bash
pip install -r requirements.txt
```

## Come iniziare
1. Clonare il repository:
```bash
git clone https://github.com/talea-platform/3-30-300-index
cd 3-30-300-index
```
2. Aprire il notebook principale:
```
notebooks/3_30_300index_and_clusters.ipynb
```
3. Configurare i percorsi dei dati nelle prime celle
4. Eseguire tutte le sezioni per generare gli indicatori

## Output
- **3_30_300_stat_areas.csv** – indicatori 3-30-300 per area statistica
