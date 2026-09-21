# Toronto 311 Service Request Analysis

## Overview

The City of Toronto receives hundreds of thousands of 311 service requests each year. Understanding when and where these requests occur, and which services generate the most demand, can help identify patterns in how residents use municipal services.

This project analyzes Toronto's 2025 311 Service Request data using Python to explore service demand across request types, city divisions, time periods, and Toronto wards.

The analysis focuses on three questions:

1. **Which services generate the most requests?**
2. **When is demand highest?**
3. **Where is demand concentrated?**

## Dataset

The project uses the **2025 Toronto 311 Service Request dataset** from the City of Toronto Open Data Portal.

Each record represents an individual 311 service request and contains information such as:

* Service request type
* Responsible city division
* Request status
* Ward
* Creation date and time
* Section and subsection

The original dataset contained more than **500,000 service request records**.

**Source:** City of Toronto Open Data Portal

## Tools & Technologies

* **Python**
* **pandas** — data cleaning, transformation, and analysis
* **NumPy** — missing-value handling
* **Matplotlib** — data visualization
* **Seaborn** — visualization styling
* **Jupyter Notebook** — analysis environment

## Data Cleaning

Before performing the analysis, I reviewed the dataset for missing values, inconsistent formatting, duplicate records, and incorrect data types.

Key preparation steps included:

* Standardizing column names
* Converting creation dates to datetime format
* Standardizing categorical values
* Separating ward names and ward numbers
* Reviewing missing values in critical fields
* Identifying and removing duplicate records
* Creating month, weekday, and hour features for time-based analysis

## Analysis

The exploratory analysis examines service demand from several perspectives:

* Most common service request types
* Request volume by city division
* Monthly and seasonal patterns
* Day-of-week and hourly patterns
* Weekday versus weekend request patterns
* Ward-level service demand
* Road pothole and road damage trends

Additional analysis was performed to investigate unusual patterns, including the February increase in service requests and the March peak in pothole and road damage reports.

## Key Findings

* **Residential Bin Lid Damaged** was the most frequently reported individual service request type.
* **Solid Waste Management Services** handled the largest overall volume of requests.
* Service request volume was highest in **February**, with snow clearing and winter maintenance requests contributing substantially to the increase.
* Request activity was highest during the workweek and peaked around **10:00–11:00 AM**.
* **Road Pothole / Road Damage** requests showed a strong seasonal pattern, reaching their highest level in **March** before declining throughout the remainder of the year.
* **Toronto-Danforth** recorded the highest total 311 request volume, while **Etobicoke-Lakeshore** recorded the most pothole and road damage requests.

## Limitations

Several factors should be considered when interpreting the results:

* 311 requests measure **reported service demand**, not necessarily the total number of issues occurring across Toronto.
* Differences between wards may be influenced by population, density, infrastructure, land use, and residents' likelihood of using 311.
* The dataset does not contain enough information to determine the cause of every observed pattern.
* External factors such as weather could help explain seasonal patterns but were not included in this analysis.

Because of these limitations, the results should be interpreted as patterns in 311 reporting rather than direct measures of service quality.

## Repository Structure


## View the Full Analysis

The complete data cleaning process, exploratory analysis, visualizations, and detailed findings are available in:

**`Toronto_311_Service_Request_Analysis.ipynb`**

## Data Source

City of Toronto Open Data — 311 Service Requests
