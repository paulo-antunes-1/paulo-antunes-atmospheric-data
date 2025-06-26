This is a simple code to download and generate results from ERA_5 for any variable. In this case I used the 2-meter air temperature variable as an example.


# ERA5_Climatology – Temperature Analysis Over Brazil Using ERA5 Data

This code will be used for downloading, processing, and visualizing near-surface temperature (2m temperature) from the **ERA5 reanalysis dataset** provided by the **Copernicus Climate Data Store (CDS)**. The focus is on Brazil for the year 2022.

---

#Description of the Analysis

The code performs the following steps:

1. **Data Download**:
   - Downloads daily data of 2-meter air temperature (`t2m`) from ERA5 using the CDS API.
   - Region limited to Brazil (lat: -35 to 5, lon: -75 to -35).
   - Format: NetCDF (`.nc`).

2. **Preprocessing**:
   - Converts temperature from Kelvin to Celsius.
   - Aggregates data into:
     - **Monthly means** (for each of the 12 months).
     - **Annual mean** (average of the entire year).

3. **Visualization**:
   - Generates a panel with 12 subplots (one for each month) showing spatial patterns of mean temperature.
   - Adds:
     - State borders of Brazil.
     - Latitude/longitude grid lines (only on outer edges for readability).
     - Unified color scale across all maps.

---

## Example Outputs

- **Monthly mean temperature maps** for each month of 2022.
- **Annual mean temperature map** (optional addition).
- All maps include political boundaries and use an intuitive `coolwarm_r` colormap.

---

## Dependencies

This project uses:

- `xarray`
- `matplotlib`
- `cartopy`
- `geopandas`
- `cdsapi`
- `netCDF4`

Make sure to install them before running the scripts.

---

## How to Run

If using Google Colab:

1. Mount your Google Drive
2. Configure your `.cdsapirc` file with CDS API credentials
3. Run the script provided in the notebook

---

## CDS Access

To download ERA5 data, you must:

1. Create an account at: [https://cds.climate.copernicus.eu](https://cds.climate.copernicus.eu)
2. Accept the dataset license terms
3. Generate your API key and save it in a `.cdsapirc` file

---

## Author

This analysis was developed by **Paulo Antunes** as part of a climatological exploration over Brazil using reanalysis data and Python-based scientific tools.
