# El Niño exposure of Honduras's Dry Corridor food system

Data and code for the Food Trade & Migration Analysis Project (CLMT G5047, Columbia University, Fall 2026).
**Team:** Fabricio Correa Lara and Siddhi Vora.

**Research question:** How exposed are subsistence maize and bean farmers in Honduras's Dry Corridor to the 2026 El Niño, and does a failed primera harvest lead people to move?

## Repository structure

| Folder | Contents |
|---|---|
| `data/` | Datasets (ENSO, rainfall, prices, migration, displacement, production, trade, remittances, food security) |
| `notebooks/` | Google Colab notebooks used to download, clean, analyse and plot the data |
| `figures/` | Final figures used in the report |

## Datasets (accessed October–November 2026)

| Topic | Source | File(s) | Coverage |
|---|---|---|---|
| ENSO | NOAA CPC, Oceanic Niño Index (ONI) and Relative ONI (RONI) | `data/displacement/enso_jja_classes.csv` | 1981–2026 (JJA season) |
| Rainfall | Climate Hazards Center, CHIRPS v3 pentad, via Google Earth Engine (`UCSB-CHC/CHIRPS/V3/PENTAD`); boundaries FAO GAUL 2025 | `data/displacement/hnd_rain_*.csv`, `hnd_chirps_v3_pentad_raw.csv`, `hnd_departments.geojson` | Jan 1981 – Sep 2026, 18 departments + national + Dry Corridor |
| Prices (Honduras) | FAO GIEWS FPMA Tool, wholesale white maize and red beans, national average | `data/prices/FPMA_Honduras_Tue_Oct_27_2026.csv` | Jan 2000 – Aug 2026, monthly (2000–2004 excluded from analysis) |
| Prices (world) | World Bank Commodity Price Data (Pink Sheet), maize | `data/prices/CMO-Historical-Data-Monthly.xlsx` | Monthly |
| Migration (cross-border) | U.S. CBP,
