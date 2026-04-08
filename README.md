# Housing & Income Data Analysis

## Overview
This project presents a comprehensive data analysis of U.S. housing data combined with ZIP code–level income data. The goal is to transform raw, inconsistent datasets into meaningful insights about housing prices, affordability, and market behavior.

The analysis integrates two datasets using SQL and explores how property characteristics and local income levels interact to influence housing value. The final output is a professional, portfolio-ready project demonstrating data cleaning, exploratory analysis, database design, and data-driven storytelling.

---

## Project Motivation
The U.S. housing market is complex and influenced by both property features and economic conditions. Raw data alone is not sufficient to understand pricing patterns or affordability.

This project was developed to:

- Strengthen real-world data analysis and SQL skills  
- Build a complete, portfolio-ready analytics project  
- Understand how income impacts housing prices and affordability  
- Apply data cleaning, feature engineering, and visualization techniques  
- Create a clear and professional data narrative  

---

## Business Value
This analysis provides insights for multiple audiences:

### Real Estate Professionals
- Identify pricing trends across different regions  
- Understand how property characteristics affect value  

### Investors
- Evaluate affordability using price-to-income ratios  
- Identify potentially undervalued or overpriced areas  

### Data Teams
- Demonstrate a clean data pipeline (EDA → SQL → insights)  
- Provide a foundation for predictive modeling or dashboards  

---

## Dataset Description

### Housing Dataset (~3,000 records)
- Price  
- Square Footage (`area_sqft`)  
- Bedrooms & Bathrooms  
- Property Type  
- City, State, ZIP Code  
- Additional listing attributes  

### Income Dataset (ZIP-level)
- ZIP Code  
- State Code  
- Household Count  
- Total Adjusted Gross Income  
- Average Household Income  

---

## Project Structure

### Section 1 — Housing Data Analysis
- Data cleaning and preprocessing  
- Feature engineering (`price_per_sqft`, price bands)  
- Exploratory analysis of property characteristics  
- Visualization of pricing trends  

---

### Section 2 — Income Data Analysis
- Cleaning and standardization of income data  
- Aggregation at ZIP level  
- Distribution and variability analysis  
- Economic context for housing markets  

---

### Section 3 — Data Integration & Advanced Analysis
- Built a SQLite database  
- Stored datasets as relational tables  
- Performed SQL joins to combine housing and income data  
- Created a unified dataset (`master_df`)  

Key analyses:
- Price vs income relationship  
- Price per square foot across income levels  
- Affordability analysis using price-to-income ratio  
- Market segmentation (undervalued vs high-pressure areas)  

---

## Key Questions Answered

- Do higher-income ZIP codes have higher home prices?  
- How does price per square foot vary across income levels?  
- Are some areas overpriced relative to local income?  
- What features most strongly influence housing prices?  

---

## Key Insights

- Housing prices generally increase with income, but not perfectly  
- Price per square foot is higher in wealthier areas  
- Some ZIP codes show affordability pressure (high price-to-income ratios)  
- Property size is the strongest driver of price  
- Market dynamics are influenced by both property features and location economics  

---

## Database & SQL

The project uses SQLite to structure and integrate data.

### Tables:
- `property_listings`
- `neighborhood_income`
- `master_df`

### Key Concepts:
- LEFT JOIN on ZIP code  
- Aggregation and grouping  
- Data validation and consistency checks  

---

## ERD & Schema

An Entity Relationship Diagram (ERD) was created to represent the database structure.

Relationship:
- One ZIP code → Many housing listings  

This design ensures:
- minimal data duplication  
- scalable analysis  
- clear relational structure  

---

## Visualizations

The project includes multiple visualizations such as:

- Correlation heatmap  
- Price vs square footage scatter plots  
- Price distribution histograms  
- Price per square foot analysis  
- Affordability comparisons by ZIP code  
- Market segmentation plots  

Each visualization is accompanied by clear explanations and interpretation.

---

## How to Run

### 1. Clone the Repository
```
git clone https://github.com/Shukrullahsaifi/Housing-Data-EDA.git
cd Housing-Data-EDA
```

### 2. Create a Virtual Environment
```
python -m venv venv
source venv/bin/activate   # macOS
venv\Scripts\activate      # Windows
```

### 3. Install Requirements
```
pip install -r requirements.txt
```

### 4. Open the Notebook
```
code .
```

## Repository Contents
	- Housing Dataset EDA.ipynb — Full analysis notebook
	- us_house_Sales_data.csv — Housing dataset
	- housing_analysis.db — SQLite database
	- requirements.txt — Dependencies
	- README.md — Project documentation
## Limitations
	- Income data is aggregated at ZIP level, not individual household level
	- Not all housing records matched with income data
	- Listing prices may differ from actual sale prices
	- External factors (interest rates, supply constraints) are not included

## Insights & Conclusions
  - Price strongly correlates with area_sqft
  - Bedrooms/bathrooms influence price, but less than square footage
  - Price‑per‑sqft stabilizes comparisons across markets
  - Outliers highlight unique properties or errors

## Future Work
  - Build price prediction models
  - Add geographic mapping
  - Combine with income or interest‑rate data
  - Extend to full capstone analysis

## Author
**Shukrullah Saifi**  
Data Analyst | Real Estate Analytics Enthusiast  
Louisville, KY
