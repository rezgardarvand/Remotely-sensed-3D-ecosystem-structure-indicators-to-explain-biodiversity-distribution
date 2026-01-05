# Remotely-sensed-3D-ecosystem-structure-indicators-to-explain-biodiversity-distribution
# Code for reproducible SDM analyses 

This repository contains the R scripts used in the manuscript.

## Data availability
All data and codes used in this study are publicly available on Zenodo:
DOI: 10.5281/zenodo.18147310

GitHub repository:
https://github.com/rezgardarvand/Remotely-sensed-3D-ecosystem-structure-indicators-to-explain-biodiversity-distribution

## Folder structure
- `scripts/` : all R scripts
- `data/` : data are not stored in this repository (see Zenodo)
- `outputs/` : outputs will be created when scripts are run

## Required inputs (from Zenodo)
- Species table: `Cupressus.csv`
- Predictors:
  - GEDI rasters at 500 m
  - CHELSA rasters 

## How to run
Run scripts in this order:
1. `scripts/01_extract_gedi_level2.R` (optional: requires GEDI .h5 files)
2. `scripts/02_derive_products_from_metrics.R`
3. `scripts/03_idw_interpolation_metrics_excel_500m_FINAL.R`
4. `scripts/04_SDM_3scenarios_500m_FINAL.R`
