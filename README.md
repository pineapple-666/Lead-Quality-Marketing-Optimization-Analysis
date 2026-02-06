# Lead-Quality-Marketing-Optimization-Analysis
# Lead Quality & Marketing Optimization Analysis

This repository contains a data-driven evaluation of marketing lead performance, focusing on identifying the drivers of "lead quality" and opportunities for financial optimization. The project specifically analyzes whether a 20% improvement in lead quality is achievable to justify a proposed increase in Cost Per Lead (CPL).

## Project Overview

The analysis processes 3,012 valid lead records collected from one publisher to one advertiser between April and October 2009. By examining various segments—including ad creative, consumer demographics, and traffic sources—this project identifies strategies to maximize lead conversion rates and marketing ROI.

## Key Business Questions

* **Trend Analysis:** Are there statistically significant lead quality trends (improving or declining) over time? 


* **Driver Identification:** What segments—such as ad type, debt level, or design—most influence lead quality? 


* **Financial Opportunity:** Can we increase lead quality by 20% (from 8.0% to 9.6%) to secure a 20% increase in CPL? 



## Core Findings

* **Temporal Patterns:** No statistically significant linear trend in lead quality was detected over time (), indicating that timing alone does not explain quality changes.


* **Primary Drivers:** The **AdGroup** (type of ad seen) and consumer **DebtLevel** were identified as the strongest predictors of lead quality ( and , respectively).


* **Optimization Potential:** Simulation results demonstrated that deprioritizing low-performing segments could raise lead quality by **47–51%**, easily exceeding the 20% improvement threshold required for a CPL increase.



## Technical Implementation

### Data Processing & Cleaning

* **Validation:** Cleaned the original 3,021-record dataset to retain 3,012 valid records, removing duplicates and missing entries.


* **Feature Engineering:** Extracted ad features from internal `WidgetName` fields, including size, design, and layout.


* **Outcome Mapping:** Categorized leads into "Good" (converted or engaged), "Bad" (non-convertible), and "Neutral" (neither).



### Statistical Methodologies

* **Regression Modeling:** Utilized OLS regression to assess the relationship between `GoodLeadPercentage` and time (weeks).


* **Categorical Testing:** Applied **Chi-square tests** to determine the significance of relationships between lead quality and variables like `MarketingCampaign`, `Partner`, and `Design`.


* **Simulation:** Conducted "what-if" analyses to measure the impact of filtering underperforming `AdGroups` and `DebtLevels` on overall lead volume and quality.



## Tools Used

* **Language:** Python 


* **Key Libraries:** Pandas, Scikit-learn, Statsmodels, Matplotlib, Seaborn 


* **Other Platforms:** Tableau (for leadership reporting), SQL (for data extraction) 



---

**Author:** Siming Chen

**Date:** January, 2026
