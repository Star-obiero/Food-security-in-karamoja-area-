# Food Security in Karamoja area

The visualization focuses on the Karamoja region of Uganda, the most food-insecure area in the country, providing NGOs with insights into the most vulnerable areas to ensure that interventions are accurately targeted and effective.


## Food Security Monitoring in Karamoja
# Overview

Karamoja is the most food-insecure region of Uganda. One of the key reasons is the low productivity of staple crops such as maize and sorghum, caused by recurrent droughts, pests, and diseases. NGOs working in the region provide technical support and farm inputs but lack visibility into the overall state of agricultural production.

This project analyzes sub-county level crop yield data (2017 season) for maize and sorghum in Karamoja and prepares the foundation for an interactive visualization tool that can support decision-making for food security interventions.

Business Problem

NGOs in Karamoja need better insight into crop yields across the region. Localized, fragmented data sources limit their ability to allocate resources effectively. The goal of this project is to:

Explore and analyze yield data for maize and sorghum.

Combine crop yield data with geospatial boundaries (districts and sub-counties).

Prepare data for visualization in a dashboard tool, enabling results to be viewed at both district and sub-county levels.

# Data Sources

Uganda Administrative Boundaries

District-level shapefile

Sub-county-level shapefile

Crop Yield Data (2017)

Maize field area (hectares)

Sorghum field area (hectares)

Linked with sub-county shapefile for spatial analysis.

# Methods

Data Cleaning and Preparation

Loaded shapefiles into GeoPandas.

Merged crop yield data with geospatial boundaries at sub-county and district levels.

Checked for missing values and filled NaN values with zero where needed.

Filtered the data to focus on Karamoja sub-region only.

Reduced dataset to 53 sub-counties relevant for Karamoja.

# Exploratory Data Analysis (EDA)

Inspected distributions of maize and sorghum areas.

Counted missing and zero entries.

Observed that most sub-counties had missing or zero values, with ~61 non-null maize entries and ~58 non-null sorghum entries out of 1382.

Geospatial Processing

Created GeoDataFrames for sub-counties and districts.

Verified geometries and alignment of boundaries.

Merged dataframes with yields for mapping purposes.

# Results

After filtering, the Karamoja dataset contained 53 sub-counties.

Only 61 maize records and 58 sorghum records had valid field area values, highlighting the sparsity of yield data.

Large portions of the dataset contained zeros or missing values, reflecting limited coverage of remote sensing yield estimates in 2017.

Despite sparsity, the prepared dataset is suitable for generating maps that visualize crop yields across sub-counties and districts.

# Conclusions

Crop yields in Karamoja (2017) were very sparsely captured, limiting the depth of statistical analysis.

The cleaned dataset can still provide valuable visual insights into where production exists or is absent.

District and sub-county geospatial joins are functional, making it possible to display results in a mapping tool.

# Next Steps

Build an interactive dashboard (e.g., in Tableau or Power BI) that displays yields at both district and sub-county levels.

Use the maps to highlight areas with zero or low yields for NGO decision-making.

If possible, acquire additional years of crop yield data to improve trend analysis and reduce sparsity.




## Tableau Dashboard
Explore the interactive dashboard on [Tableau Public](https://public.tableau.com/app/profile/prince.obiero/viz/FixingKaramojafoodinsecurityissues/Dashbordshowingareascultivatedandthereyield?publish=yes).

![Dashboard Preview](images/dashboard.png)

