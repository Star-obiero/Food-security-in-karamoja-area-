# Food-security-in-karamoja-area-
It visualizes karamoja area of Uganda knowing it is the most food insecure area to give NGO insight on which areas are the most needy so that they don't miss there target



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

Karamoja is sorghum dependent if sorghum fails due to drought ,pest or some other reason the food security will be compromised
Even though sorghum production in kg is higher than that of maize there is growing concern about its yield per hectares this forcing community to allocate large lands for sorghum cultivation and neglecting other like maize which are doing well on small pieces of land

District like Aibim and morroto are underperforming  both having very low yield production and very low crop production yet at the same time they have low population

Areas with high cultivation area dose not necessarily suggest higher crop production this can be seen in districts like Napak and Kabong this because the corelation between crop area and crop yield are not strong

Low correlation between population and yield highlight the risk of hidden food insecurity hotspot ,some densely populated district (e.g Kabong)may be at high risk even if yield was average

# Recommendations for NGOs
Diversify Beyond Sorghum


* Promote alternative drought-tolerant crops such as maize, cassava, millet, and legumes to reduce dependency on sorghum.


* Support seed distribution programs for these alternatives.


Boost Productivity per Hectare


* Provide training on modern agronomic practices (fertilizer use, pest management, intercropping).


* Introduce improved sorghum varieties with higher yield per hectare and pest resistance.


Target Underperforming Districts (Aibim and Moroto)


* Prioritize interventions here by supplying inputs, irrigation tools, and extension services.


* Encourage kitchen gardens and small-scale irrigation to reduce reliance on rain-fed farming.


Address Misallocation of Land


* Sensitize communities on balancing sorghum cultivation with other crops (e.g., maize, which performs well on smaller plots).


* Support land-use planning and farmer cooperatives to optimize crop mix.


Link Production to Food Security Hotspots


* Establish food banks and grain storage in densely populated but food-insecure districts (like Kabong).


* Strengthen early-warning systems that connect yield monitoring with population data to detect hidden hotspots.


Invest in Climate Resilience


* Promote water harvesting, small-scale irrigation, and soil conservation to reduce drought risks.


* Introduce community-level crop insurance schemes against drought and pests.



Future improvements to the dashboard (adding new data, predictive analysis).

# Next Steps
Policy & Stakeholder Engagement


* Suggest partnerships between NGOs, local government, and community leaders for coordinated action.


* Advocate for integration of NGO programs into district food security plans.


Capacity Building


* Propose training of local farmers, extension workers, and youth groups to ensure sustainability.


* Recommend peer-to-peer farmer networks for knowledge sharing.


Pilot and Scale


* Start with pilot projects (e.g., improved seed trials, irrigation demos) in high-risk districts.


* Plan to scale successful interventions region-wide.


Monitoring & Evaluation


* Develop indicators (yield per hectare, nutrition levels, storage capacity, crop diversity).


* Use periodic surveys and satellite/field data to track progress.


Sustainability & Exit Plan


* Encourage community ownership (cooperatives, savings groups).


* Suggest that NGOs gradually shift from aid to resilience-building so communities are not aid-dependent.






## Tableau Dashboard

! Project Report

You can view our full project report here:  
[Google Doc Link](https://docs.google.com/document/d/1euVAsRmF__Y5HhQrDEgSGU4-59-kBV0gpekxJH1IojM/edit?usp=sharing)
Explore the interactive dashboard on (https://public.tableau.com/app/profile/lynn.rotich/viz/Group_9_Tableau_Workbook_17564945353750/RelationshipofCropGrowingAreaToTheTotalCropYield?publish=yes).

![Dashboard Preview](Tableauimage.png)

