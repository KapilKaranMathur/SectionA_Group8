# Real Estate Market Analysis & Investment Strategy
<div align="center">
	<img src="image.png" alt="Real Estate Market Dashboard" width="600" />
</div>
<div align="center">
	<a href="https://docs.google.com/spreadsheets/d/1QU5AEmZaSJcBjNW9MoLuTMz_-Acxpx7rbuLUTRQnjZs/edit?gid=1004518743#gid=1004518743" target="_blank" rel="noopener noreferrer">
		<img src="https://img.shields.io/badge/Cleaned%20Dataset-Google%20Sheets-brightgreen?logo=google-sheets&logoColor=white" alt="Cleaned dataset" />
	</a>
	&nbsp;
	<a href="https://docs.google.com/spreadsheets/d/1QU5AEmZaSJcBjNW9MoLuTMz_-Acxpx7rbuLUTRQnjZs/edit?gid=1285832976#gid=1285832976" target="_blank" rel="noopener noreferrer">
		<img src="https://img.shields.io/badge/Dashboard-Google%20Sheets-blue?logo=google-sheets&logoColor=white" alt="Dashboard" />
	</a>
</div>

## Project Overview
This project provides a comprehensive market analysis of over **21,600 housing transactions**. By cleaning raw transactional data and applying advanced aggregation techniques, this analysis identifies the key drivers of property value—ranging from waterfront premiums to renovation ROI—to guide a real estate investment firm’s acquisition strategy.

### Primary Decision Question
> *"Which specific property attributes and neighborhood factors (waterfront views, house condition, or recent renovations) most significantly influence sale prices, and how should an investment firm prioritize portfolio acquisitions to maximize potential returns?"*

---

## Data & Methodology
The analysis was performed on a cleaned dataset featuring 21 columns of property data, including price, size, age, and geographical coordinates.

### Key Processing Steps:
##  Data Cleaning & Preprocessing

The raw housing dataset was cleaned and transformed to make it suitable for machine learning modeling. The following steps were performed:

---

### 1. Column Standardization

- Renamed all columns to lowercase.
- Replaced spaces and special characters with underscores.
- Improved consistency and readability of column names.

---

### 2. Removed Irrelevant Features

The following columns were removed:

- `ID`
- `No_of_Times_Visited`

**Reason:**  
These features do not contribute to house price prediction and may introduce unnecessary noise into the model.

---

### 3. Handling Missing Values

- Identified missing/null values in the dataset.
- Applied appropriate handling techniques to reduce missing data.
- Improved overall dataset quality and reliability.

---

### 4. Feature Engineering

- Created new meaningful features to improve model performance.
- Derived additional attributes from existing columns where necessary.
- Enhanced the predictive capability of the dataset.

---

### 5. Data Type Optimization

- Ensured numeric columns are in proper numeric format.
- Corrected inconsistent data types.
- Verified the dataset is fully ready for machine learning modeling.

---

## Final Dataset Status

- Cleaned and standardized dataset
- Reduced missing values
- Optimized for ML pipeline
- Ready for training predictive models

* **Calculated Metrics:** Created `Price per Sqft` and `House Age` to allow for "Apples-to-Apples" comparisons across different neighborhoods.
* **Pivot Table Aggregation:** Built 11 distinct pivot tables to isolate variables such as the **Waterfront Premium** ($958k vs $508k) and the **Renovation Effect** ($656k vs $505k).

---

## Dashboard Visualizations
The final dashboard consists of **11 interactive charts** designed for executive-level decision-making:

### 1. Market Snapshot
* **Overall Market Metrics:** Scorecards for Total Sales, Avg. Price, and Median Price.
* **Price Trend Over Time:** Area chart tracking market momentum.

### 2. Property Attribute Analysis
* **Waterfront Value Gap:** Bar chart showing the massive luxury premium for waterfront access.
* **Condition vs. Valuation:** Combo chart comparing sales volume against average price for different house conditions.
* **Size Impact:** Area chart visualizing price growth relative to living area square footage.

### 3. Investment Strategy 
* **Renovation ROI:** Donut chart illustrating the value-add of property modernization.
* **Bed/Bath Heatmap:** A visual grid identifying the most profitable house configurations.
* **Age Effect:** Line chart showing the correlation between property age and market demand.

### 4. Geographic Intelligence
* **Price by Zipcode Map:** Geo-chart pinpointing high-value and emerging neighborhoods.
* **Luxury Pockets:** Stacked bar chart showing waterfront premiums by specific zipcode.
* **Acquisition Targets:** A ranked analysis of neighborhoods with the lowest **Price per Sqft**.

---

## Strategic Recommendations
* **Focus on Renovation:** Data shows a **$151,000+** average premium for renovated homes, suggesting a high-ROI "Fix-and-Flip" strategy is viable.
* **Target "Fair" Condition Volume:** The "Fair" condition segment represents the highest liquidity (14,000+ sales), making it the safest tier for rapid portfolio scaling.
* **Value Efficiency:** Acquisition efforts should prioritize zipcodes with low cost-per-square-foot but high overall grades to capture maximum appreciation.

---

## Repository Structure
- `Calculation&Pivot_Table`: Pivot table exports and calculation workbooks.
- `CleanedDataset`: Contains `Cleaned.csv` and notes about data cleaning.
- `Dashboard`: Dashboard assets and `Raw Housing Prices Dashboard (1).csv`.
- `Documentation`: Project documentation and methodology notes.
- `Presentation`: Final presentation slides.
- `RawDataset`: Original raw `dataset.csv`.
- `image.png`: Cover image used at the top of this README.
- `Readme.md`: Project overview and links.

---
