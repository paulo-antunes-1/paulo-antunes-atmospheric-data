**# Aerosol Transport — Atmospheric Aerosol Transport Analysis**

🇧🇷 [Versão em Português](README_PT.md)

**## Overview**

A Python-based data pipeline for the integration, processing, and analysis of atmospheric aerosols, meteorological variables, and biomass-burning observations over South America.

The project explores the spatial and vertical evolution of atmospheric aerosols by combining three-dimensional atmospheric data with fire observations, providing a framework for aerosol transport analysis and predictive modeling.

**## Problem**

Biomass-burning emissions can be transported over long distances and reach different atmospheric levels depending on meteorological conditions.

Understanding this evolution requires the integration of multiple sources of atmospheric information, including aerosol concentrations, meteorological variables, pressure levels, and fire observations.

This project addresses the challenge of processing and integrating these multidimensional datasets into a consistent spatial-temporal framework for aerosol transport analysis.

**## Solution**

A Python workflow was developed to integrate atmospheric and fire datasets and analyze the horizontal and vertical evolution of aerosols.

The workflow includes:

* processing of multidimensional atmospheric datasets;
* integration of aerosol and meteorological variables;
* integration of biomass-burning observations;
* analysis across multiple atmospheric pressure levels;
* generation of vertical aerosol profiles;
* spatial and temporal analysis of aerosol concentrations;
* construction of structured datasets for predictive modeling;
* visualization of horizontal and vertical aerosol transport.

**## Data**

**### MERRA-2**

Atmospheric reanalysis data used to obtain aerosol and meteorological variables at multiple vertical levels.

Variables analyzed include aerosol species such as:

* Organic Carbon (OC);
* Black Carbon (BC);
* aerosol optical properties;
* meteorological variables associated with atmospheric transport.

**### FIRMS**

Satellite-based fire observations used to characterize the spatial and temporal occurrence of biomass burning.

Raw datasets are not included in this repository due to their size.

**## 🔬 Methodology**

The general processing workflow follows:

**Atmospheric Data → Preprocessing → Fire Data Integration → Vertical-Level Analysis → Spatial-Temporal Dataset → Transport Analysis → Predictive Modeling**

The processing pipeline organizes atmospheric variables in space, time, and vertical levels, allowing relationships between meteorological conditions, fire occurrence, and aerosol evolution to be investigated.

**## Predictive Modeling**

The project provides a framework for investigating whether the current atmospheric state can be used to estimate subsequent aerosol behavior.

The modeling dataset combines aerosol concentrations, meteorological conditions, fire information, and vertical atmospheric structure to support machine-learning experiments focused on aerosol evolution.

This component is under development.

**## Outputs**

The workflow can generate:

* aerosol concentration maps;
* vertical aerosol profiles;
* time series;
* atmospheric-level comparisons;
* spatial-temporal aerosol datasets;
* visualizations of horizontal and vertical aerosol evolution.

**## Technologies**

* Python
* Xarray
* NumPy
* Pandas
* SciPy
* Matplotlib
* Cartopy
* NetCDF
* MERRA-2
* FIRMS
* Machine Learning

**## Project Structure**

```text
Aerosol_Transport/
│
├── README.md
├── README_PT.md
├── requirements.txt
│
├── src/
│   ├── data_processing.py
│   ├── fire_processing.py
│   ├── vertical_analysis.py
│   ├── transport_analysis.py
│   ├── feature_engineering.py
│   └── visualization.py
│
└── figures/
```

**## Project Status**

Active development.

Current work focuses on atmospheric data integration, vertical aerosol analysis, and the development of datasets for predictive modeling.

**## Author**

**Paulo Antunes**

Meteorologist | Atmospheric Data Scientist | Data Products & AI
