# MODIS AOD Analysis
This folder contains scripts for performing Empirical Orthogonal Function (EOF) analysis on MODIS (Moderate Resolution Imaging Spectroradiometer) Aerosol Optical Depth (AOD) data.

## Contents

### 1. `MODIS_AOD_EOF.ipynb`
This notebook performs a **global EOF analysis** on the AOD data from MODIS. It computes the dominant modes of variability across the entire globe, helping to identify large-scale patterns in aerosol distribution.

### 2. `MODIS_AOD_EOF_regional.ipynb`
This notebook performs a **regional EOF analysis** on MODIS AOD data. Although the script currently focuses on a specific region, it is designed to be **flexible and applicable to any region of the globe** by modifying the latitude and longitude boundaries accordingly.

## Purpose

The EOF technique is useful for identifying the principal spatial patterns and associated temporal variability in aerosol concentrations derived from satellite data. These analyses are essential for understanding atmospheric processes, air quality, and radiative forcing due to aerosols.

## Notes

- The regional analysis script is modular and easy to adapt for different spatial domains.
- The global script offers a comprehensive overview and is suitable for large-scale climate and environmental studies.

---
Developed as part of atmospheric data analysis with MODIS datasets.

## Author

This analysis was developed by **Paulo Antunes** as part of a aerosols analysis over the globe using remote sensing data and Python-based scientific tools.
