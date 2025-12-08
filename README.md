# Eviction Risk Prediction in Philadelphia

## MUSA 5080 Final Project
This project aims to predict eviction filings in Philadelphia using open-source data and spatial analysis techniques. By analyzing historical eviction data alongside housing violations and demographic factors, we identify high-risk areas to support targeted policy interventions.

## Project Review
Eviction is a complex socio-economic issue affecting housing stability in Philadelphia. This analysis leverages machine learning models to understand the drivers of eviction and forecast future risks at the census tract level.

**Key Objectives**:
- **Exploratory Data Analysis (EDA)**: Visualize spatial and temporal patterns of eviction filings.
- **Feature Engineering**: Integrate diverse datasets including L&I violations and census data.
- **Predictive Modeling**: Build and evaluate models (Logistic Regression) to predict high-eviction risk tracts.
- **Policy Recommendations**: Provide actionable insights based on model results.

## Key Findings
- **High Concentration of Risk**: Eviction risk is not randomly distributed but highly concentrated. We forecast 71 census tracts (approx. 20% of the city) as high-risk for 2026. These tracts form continuous corridors primarily in North and West Philadelphia.
- **Top Risk Drivers**: The "Full Integrated Model" (Model 5) achieved the best performance (Accuracy: 94.3%, AUC: 0.97). The analysis reveals that eviction risk is dominated by historical inertia (past filing rates) and landlord hotspots, and is significantly amplified in renter-majority and Black-majority neighborhoods.
- **Emerging Hotspots**: While historical data is predictive, recent trends show some tracts experiencing 100-200% increases in filing rates compared to baselines, signaling new areas of distress that require immediate attention.

## Policy Recommendations
To address the looming 2026 housing cliff, we propose a **Tiered Intervention Strategy** to optimize the allocation of limited legal and financial resources:

1. High-Precision Targeting (Risk ≥ 80%)
- Target: A small set of extreme hotspot tracts.
- Action: Deploy resource-intensive interventions such as direct rent relief, full legal representation, and intensive case management.
- Goal: Prevent immediate displacement in the most vulnerable corridors.

2. Broad Outreach Ring (Risk ≥ 30%)
- Target: The wider "at-risk ring" surrounding the hotspots.
- Action: Implement low-cost preventive measures like SMS alerts, "Know Your Rights" workshops, and landlord engagement programs.
- Goal: Monitor for emerging hotspots and mitigate risk before it escalates.

3. Property-Level Verification
- Since predictions are at the census tract level, we recommend verifying specific property conditions with local partners before allocating expensive resources to avoid false positives.

## Data sources

### Primary dataset
Eviction Lab – Philadelphia Tracking
- City-level series
- Tract-level monthly data over multiple years
- Tract-level snapshot of Philadelphia eviction risk (since Nov 2024)
- Group-level disparities
- landlord hotspots

### Additional dataset
ACS (American Community Survey) 5-year 2022 data for Philadelphia census tracts

Historic code-violation (2012-2016) (From Licenses and Inspections Department of Philadelphia)

311 Service and Information Requests
- 311 housing-related complaint data: https://drive.google.com/file/d/1pLO9Z_d2I7L6PLXnn6sUD0hyzXRP-Rpf/view?usp=drive_link

## Author
Lingxuan Gao & Xiaoqing Chen

Master of Urban Spatial Analytics (MUSA), University of Pennsylvania
