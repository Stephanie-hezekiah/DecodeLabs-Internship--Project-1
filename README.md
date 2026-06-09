# DecodeLabs-Internship
Data Analysis Excel Project

### PROJECT TITLE: Data Cleaning and Preparation using Excel

[Status](https://img.shields.io/badge/Status-Complete-success)

[Project Overview](#project-overview)

[Data Sources](#data-sources)

[Tools Used](#tools-used)

[Data Cleaning & Transformation](#data-Cleaning-and-transformation)

[Contact](#contact)


### Project Overview
---
The focus is on Uncovering the Story, interrogating raw data to isolate missing records, clean structural formatting errors, and map out statistical boundaries before any visualization or predictive modeling occurs. This foundational phase establishes clean pipelines that convert messy corporate records into absolute business clarity.

Key Objectives:

* Profile Descriptive Statistics: Calculate exact baselines for mean, median, and record counts to evaluate data distribution.
  
* Conduct Data Forensics: Audit structural integrity by identifying missing values, format errors, and misaligned records.
  
* Isolate Outliers & Trends: Distinguish non-valuable data entry noise from high-value business signals.
  
* Translate to Impact: Apply the "So What?" test to convert statistical patterns directly into quantifiable business insights for stakeholders.

### Data Sources
---
The data set was given by our tutors 


### Tools Used
---
Excel Office: Initial data exploration and cleaning.


### Data Cleaning & Transformation
---
To ensure data integrity and structural accuracy before exploratory data analysis, the raw dataset underwent a rigorous data cleaning and transformation pipeline. This process systematically tracked modifications across a dedicated project change log to preserve transparency and ensure high data completeness.

### 1. Structural Diagnostics & Data Quality Assessment
An initial audit of the data schema evaluated the health of individual columns, diagnosing missing fields, formatting failures, and tracking loops:
* **Completeness Validation:** Columns such as `ID`, `Timestamp`, and `Location` were verified for completeness. Blank or null entry loops were flagged to compute an absolute data completeness profile.
* **Temporal Consistency:** Raw date and time stamps were audited to eliminate format corruption (e.g., handling invalid datetime entries like `INVALID_DATE`) and normalized into a unified, ISO-compliant temporal format (`YYYY-MM-DDTHH:MM:SSZ`).
* **Value Consistency:** Data values and record streams were checked for alignment errors, ensuring numerical scales and categorical tags matched their correct data types.

### 2. Forensic Log Changes (Noise vs. Signal)
Using structural filtering, data anomalies were split into non-valuable errors ("Noise") to be cleaned, and critical business exceptions ("Signal") to be preserved:
* **Null Value Imputation:** Missing numerical values or corrupted fields were handled using targeted replacement rules or statistical defaults to prevent calculation skew in downstream metrics.
* **Error Scrubbing:** Explicit format breakdowns and corrupt strings (such as row entries processing with system errors) were structurally resolved, boosting overall valid data points across the operational table.
* **Categorical Standardization:** Text inconsistencies across categorical indices (such as locations or status fields like `Valid`, `Alert`, and `Error`) were mapped to a clean, standardized master schema to eliminate duplicate group variables.

### 3. Statistical Geometry & Transformations
To prepare the cleaned evidence for modeling and dashboard construction, core mathematical transformations were established:
* **Central Tendency Selection:** Univariate shape checks were applied to numerical columns. Symmetrical distributions utilize the arithmetic **Mean**, while right-skewed business records rely on the **Median** as a robust anchor against extreme anomalies.
* **Outlier Boundary Controls:** To separate structural typos from high-value business trends, formal Interquartile Range (IQR) limits were established to flag exceptions:
    $$\text{Lower Outlier} < Q_1 - 1.5 \times \text{IQR}$$
    $$\text{Upper Outlier} > Q_3 + 1.5 \times \text{IQR}$$
* **Relationship Mapping:** Clean bivariate columns were prepared for Pearson Correlation Coefficient ($r$) matrix processing to track linear strength and direction while isolating compounding variables.


### Contact
---
•	LinkedIn: https://www.linkedin.com/in/hezekiah-stephanie-11061422a/

•	Email: stephaniehezekiel@gmail.com

•	Portfolio: https://github.com/Stephanie-hezekiah


