# Problem Statement

The goal is to implement the Nature Risk Profile methodology—a joint venture by S&P Global and UNEP-WCMC. This methodology seeks to evaluate materiality, relevance, reliance, resilience, and dependency scores associated with ground and surface water ecosystem services for three notable mining companies: BHP Group, Freeport McMoran, and Glencore.

These companies maintain a vast array of assets globally, encompassing activities from sugar refining and biofuel production to oil extraction, power generation, and steel manufacturing. Given this diverse range, the reliance on ecosystem services significantly fluctuates based on the asset's nature and its geographical positioning.

## Key Questions:

1.Calculate the Water Materiality score of each asset and/or company.
2.Calculate the Water Relevance score of each asset and/or company.
3.Calculate the Water Reliance score of each asset and/or company.
4.Calculate the Water Resilience score of each asset and/or company.
5.Calculate the Water Dependency score of each asset and/or company.
6.Please compare each company and provide insights relevant to an investment portfolio manager who may be invested in them, or may look to invest in one or more of them.


## Several datasets are available to facilitate this assessment:

1. **Asset Dataset**: Provides details on assets held by the specified companies, including their geographical locations and attributes like Ultimate Parent ISIN, Asset_id_type, Asset_id, Facility_category, and Activity description for the fiscal year 2021.
2. **Universe Dataset**: Covers water usage and revenue data at the company level from 2018 to 2022, offering granular details about the GICS sector/subindustry and industry group name. This dataset is yet to be integrated.
3. **ENCORE Dataset**: Highlights the materiality of risks tied to various processes, assisting in aligning these with asset categories. Each process gets a materiality quality score, convertible into a numerical "materiality score" between 0 and 1.
4. **World Resource Institute Aqueduct Dataset**: Presents Water Risk insights at Basin and Country Levels. It's primed to provide a resilience measure for ground and surface water ecosystem services. Risk levels are rated between 1 and 5, which, per the given methodology, are convertible to a scale of 0 to 1.

## Work Structure

The project comprises five main notebooks, a Python utility file, and a summary document:

- 1.EDA_asset_universe: Conducts exploratory data analysis (EDA) on the asset and universe datasets.
- 2.EDA_Encore: Focuses on the ENCORE dataset through detailed EDA.
- 3.EDA_asset_water: Examines the relationship between assets and water risk as provided by the World Resource Institute (WRI).
- 4.Water_Risk_Methodology: Implements the Nature Risk Profile methodology, applying it at the asset, asset group, and company levels.
- 5.EDA_water_risk_methodology_results: Examines key findings coming from 4.Water_Risk_Methodology
- support_function.py: Hosts a collection of functions utilized across the notebooks.
- findings_portfolio_manager.docx: Consolidates the findings, offering insights tailored for investment portfolio managers.

