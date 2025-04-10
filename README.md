# Enrollment Trend Analysis and Forecasting for Public Schools

## Overview
This project simulates an analysis of student enrollment trends across U.S. states to forecast future growth and inform resource allocation decisions for educational institutions. The focus is on identifying regions with projected enrollment changes and providing actionable recommendations for school planning. The analysis includes data cleaning, imputation of missing values, predictive modeling, and interactive geographical visualizations.

## Objectives
- Forecast enrollment trends for U.S. states from 2023–2032.
- Identify states/counties requiring resource adjustments (e.g., staffing, facilities).
- Provide actionable insights for expanding school networks in high-growth regions.

## Data Sources
- **National Center for Education Statistics (NCES):** Enrollment data by state (simulated dataset).
- **Texas Open Data Portal:** County-level child population data (2022).
- **U.S. Census Bureau (via `tidycensus`):** Geographical boundaries for mapping.

## Methodology
1. **Data Preparation**  
   - Converted "Year" from string to numeric format.
   - Handled missing values using MICE imputation (CART and Lasso methods).
   - Compared imputed vs. original data distributions.

2. **Modeling**  
   - Built linear regression models to predict enrollment trends for Texas.
   - Tested models using original and imputed datasets (70/30 train-test split).
   - Forecasted enrollment for 2023–2032.

3. **Visualization**  
   - Created interactive maps using `leaflet` to display projected enrollment changes by state.
   - Analyzed Texas county-level child population data to pinpoint growth hotspots.

## Key Findings
- **Texas Enrollment Trends:** Predicted steady enrollment growth from 2023–2032.
- **High-Growth Counties:** Starr County identified as a priority for expansion due to its high child population and proximity to existing schools.
- **Resource Recommendations:** Houston, Dallas, Austin, and San Antonio may require scaling programs to accommodate growth.
