# El Niño exposure of Honduras's food system

Data and code for the Food Trade & Migration Analysis Project (CLMT G5047, Columbia University, Fall 2026).
**Team:** Fabricio Correa Lara and Siddhi Vora.

**Focus (draft):** How exposed are subsistence maize and bean farmers in Honduras's Dry Corridor to the 2026 El Niño, and does a failed primera harvest lead people to move?

## Repository structure

| Folder | Contents |
|---|---|
| `data/` | Processed datasets (ENSO, rainfall, prices, migration, displacement) |
| `notebooks/` | Google Colab notebooks used to download, clean and explore the data |
| `figures/` | Draft figures |

## Datasets (accessed 26–27 Oct 2026)

| Topic | Source | File(s) | Coverage |
|---|---|---|---|
| ENSO | NOAA CPC, Oceanic Niño Index (ONI) and Relative ONI (RONI) | `data/enso_jja_classes.csv` | 1981–2026 (JJA season) |
| Rainfall | Climate Hazards Center, CHIRPS v3 pentad, via Google Earth Engine (`UCSB-CHC/CHIRPS/V3/PENTAD`); boundaries FAO GAUL 2025 | `data/hnd_rain_*.csv`, `data/hnd_departments.geojson` | Jan 1981 – Sep 2026, 18 departments + national |
| Prices | FAO GIEWS FPMA Tool, wholesale white maize and red beans, national average | `data/prices/` | Jan 2000 – Aug 2026, monthly |
| Migration (cross-border) | U.S. CBP, Southwest Land Border Encounters | `data/migration/` | Oct 2018 – Aug 2026, monthly |
| Displacement (internal) | IDMC, Global Internal Displacement Database (GIDD) | `data/displacement/` | 2008–2025, annual |

## Notebooks and AI use

| Notebook | Purpose | Code written by |
|---|---|---|
| `Honduras_CHIRPS_GEE.ipynb` | Extracts CHIRPS rainfall by department, builds seasonal anomalies and draft figures | Claude (Anthropic) |
| `ENSO_index.ipynb` | Compares ONI and RONI, classifies El Niño years | Gemini (Google) |
| `Prices.ipynb` | Loads and explores FPMA price series | Gemini (Google) |
| `Migration.ipynb` | Combines CBP files, monthly Honduran encounters | Gemini (Google) |

All code was run, reviewed and checked by the team.

## Status

Milestone 1 (data summary): datasets downloaded and explored. Analysis in progress.
