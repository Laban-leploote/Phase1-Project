# Aircraft Risk Assessment For New Aviation Division

## Overview

This project was developed to support the company’s plan to diversify into the aviation industry by identifying the safest aircraft for potential purchase. The primary goal was to transform over sixty years of historical aviation accident data into actionable insights that can guide decision-making. Using data cleaning, analysis, and visualization techniques in Python, the project identifies aircraft models with the lowest accident risk and provides business recommendations for safe and sustainable investments.

## Business Problem 

The company is expanding into new industries, particularly in aviation, to operate both commercial and private aircraft. However, there is limited knowledge about the relative risks associated with different aircraft models. The challenge is to assess and determine which aircraft are safest to operate. This analysis provides a data-driven approach that helps the aviation division leadership understand risk levels across aircraft types and make informed purchase decisions.

## Objectives

1. To evaluate aircraft safety using NTSB data to understand historical accident and fatality patterns.
2. To develop a quantitative risk score to compare aircraft models and identify the safest options.
3. To provide clear, data-driven recommendations that guide safe and sustainable aircraft acquisitions as the company enters the aviation business.


## Data 

The dataset used in this analysis comes from the National Transportation Safety Board (NTSB) and contains civil aviation accident data from 1962 to 2023. It includes over 90,000 records and 31 variables such as the event date, aircraft make and model, number of engines, injury severity, and total fatalities. The dataset provides both U.S. and international accident data. Significant preprocessing was necessary due to missing values, inconsistent formatting, and duplicate entries.

## Data Cleaning and Preparation

The data cleaning process involved several key steps. Duplicates were removed to ensure data accuracy. Missing values were handled appropriately — categorical features like aircraft make and model were filled with “Unknown” or dropped where irrelevant, and numerical injury counts were filled with zeros. Column names were standardized, and invalid or incomplete date records were dropped. A new column was created by combining the Make and Model columns to form a unified “Aircraft” identifier. Additionally, an “Accident Year” column was extracted from the event date to allow for temporal analysis.

## Data Analysis and Methodology

The analytical process began by aggregating accident records by aircraft make and model. Key metrics were calculated, including total accidents, total fatalities, fatal accident counts, and a risk score that combines accident frequency and fatality rate. The risk score was designed so that lower values represent safer aircraft. Only aircraft with at least five recorded accidents were included in the final ranking to avoid bias from small samples.

This allowed the identification of aircraft models that consistently demonstrate low fatality rates relative to their accident counts. Models with high total fatalities or fatality rates were categorized as high-risk, while models with minimal fatal records were considered safe investment options for the company’s aviation expansion.

## Visualizations and Key Insights

Several visualizations were developed to make the analysis clear to non-technical stakeholders. A bar chart was used to show the top 15 aircraft by number of accidents, providing insight into which models are most frequently involved in accidents. A line graph highlighted the ten aircraft with the lowest risk scores, showing clear differences in safety among them. These visuals make it easy for executives to interpret the data and support evidence-based decision-making.
We also added and interactive dashboard to help with the visualization here is the link attached:
https://public.tableau.com/views/Projectdashboard_17595816573930/AircraftSafetyRiskAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Findings and Insights

The analysis revealed that aircraft models such as the Airbus A300-600 and McDonnell Douglas DC-9 have historically low fatality rates and represent safer investments. On the other hand, several aircraft types, including certain Boeing and Douglas models, exhibited higher fatality counts despite having fewer accidents. This pattern indicates that while some aircraft experience fewer crashes, those crashes tend to be more severe.

These insights provide a balanced view for decision-makers — highlighting which aircraft are statistically safer and which ones carry elevated risk levels.

## Business Recommendations

Based on the findings, three main recommendations were made to the aviation division:

1. Prioritize the safest aircraft models — Aircraft with the lowest risk scores and minimal fatalities should be prioritized for acquisition as they provide the highest operational safety.

2. Avoid high-fatality models — Aircraft with historically high fatality counts should not be considered in the early stages of expansion to avoid financial and reputational damage.

3. Adopt a balanced selection strategy — Combine accident data with operational factors such as maintenance cost, availability, and flight purpose to achieve sustainable and safe investments.

## Conclusion

This project successfully transformed decades of aviation accident data into meaningful insights. Through data cleaning, aggregation, and visualization, it identified the safest and riskiest aircraft models for potential purchase. The findings provide a clear, evidence-based foundation for the company’s entry into the aviation industry. By focusing on low-risk aircraft, the company can minimize operational hazards and position itself as a trusted and safety-conscious aviation operator.