# MERRA2 Aerosols

This folder contains Python scripts for performing **Empirical Orthogonal Function (EOF) analysis** on various aerosol variables from the **MERRA-2 reanalysis dataset**. The goal is to identify and visualize the dominant spatial-temporal patterns of atmospheric aerosols globally and regionally.

## Contents

- `EOF_Global_AOD.ipynb`  
  Performs EOF analysis of **Aerosol Optical Depth (AOD)** on a **global scale**. This notebook is designed for applications that require global atmospheric aerosol patterns.

- `EOF_Regional_AOD.ipynb`  
  EOF analysis of **AOD** over a selected region. Despite being named “regional,” the script is fully adaptable and can be used for **any subregion of the globe**, making it a versatile tool for localized studies.

- `EOF_Regional_Black_Carbon.ipynb`  
  Performs EOF analysis on **Black Carbon aerosol** concentrations over a specific region. Like the other regional scripts, it can be customized for different spatial extents.

- `EOF_Regional_Dust.ipynb`  
  Computes EOFs for **Dust aerosols** in a regional domain. Useful for exploring dominant dust transport mechanisms and seasonality.

- `EOF_Regional_Organic_Carbon.ipynb`  
  Analyzes the variability of **Organic Carbon aerosols** through EOF decomposition in a defined region. Allows users to investigate biogenic and combustion-related aerosol sources.

## Key Notes

- All notebooks use **MERRA-2 reanalysis data** from NASA's Global Modeling and Assimilation Office (GMAO).
- The regional scripts are highly flexible and allow you to define **any latitude and longitude bounds**, making them suitable for case studies on continents, countries, or specific atmospheric hotspots.
- Outputs include maps of the **leading EOF modes**, **principal components**, and **explained variance fractions**, with figures saved in high resolution.

## Requirements

- Python ≥ 3.7  
- `xarray`, `matplotlib`, `eofs`, `cartopy`, `netCDF4`, and other standard scientific libraries.
- 
## Author

This analysis was developed by **Paulo Antunes** as part of a aerosols analysis over the globe using reanalysis data and Python-based scientific tools.
