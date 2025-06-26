# Burned Area

# Burned Area and Fire Activity Analysis in Brazil

This notebook contains a detailed exploratory analysis of fire activity in Brazil using FRP (Fire Radiative Power) data from Bdqueimadas. The goal is to identify spatial and temporal patterns of fire events across states and municipalities.

## Key Outputs

1. **FRP Records by State and Municipality**  
   A comparative bar plot showing total FRP records:
   - In blue: aggregated by **state**
   - In orange: aggregated by **municipality**
   - Both are sorted in descending order for clear visual comparison.

2. **Monthly FRP Activity by State (Map)**  
   A map of Brazil showing the average **monthly FRP activity by state** for a specific year.

3. **Monthly FRP Activity by Municipality (Map)**  
   Same as result 2, but aggregated by **municipality**, providing a finer spatial resolution.

4. **Daily FRP Occurrence in Selected States**  
   A time series plot showing **daily fire activity** in selected states during a specific year.

5. **Total Annual Burned Area in Brazil**  
   A bar chart showing the total number of fire events per year, sorted from lowest to highest.

6. **Annual Burned Area in a Specific State**  
   Same as result 5, but filtered for a **single Brazilian state**.

7. **Monthly Averages by State (Sorted)**  
   A bar chart showing the **monthly average number of FRP occurrences per state**, sorted in descending order.

##  Data & Tools

- Python (Pandas, Matplotlib, Cartopy, Xarray)
- FRP data from bdqueimadas from INPE 
- Brazilian spatial boundaries (states and municipalities)

##  Author

This analysis was developed by **Paulo Antunes** as part of a broader project investigating the relationship between biomass burning and air quality impacts in Brazil.
