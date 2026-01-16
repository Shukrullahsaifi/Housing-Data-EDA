# Housing-Data-EDA

## Overview
This project presents a comprehensive Exploratory Data Analysis (EDA) of a 3,000‑row U.S. housing dataset. The goal is to transform raw, inconsistent real‑estate data into clear insights that support informed decision‑making for buyers, investors, analysts, and real‑estate professionals.
The analysis follows industry‑standard data‑cleaning practices, applies ethical visualization principles, and focuses on uncovering meaningful trends related to pricing, home characteristics, and market behavior.

## Project Motivation
The U.S. housing market is complex, competitive, and constantly evolving. Raw housing data is often messy, inconsistent, and difficult to interpret without proper cleaning and analysis.
This project was created to:
- Strengthen professional‑level data‑analysis skills
- Build a polished, portfolio‑ready demonstration of data wrangling & visualization
- Understand what drives changes in home prices and affordability
- Support real‑estate investment decisions with objective data
- Develop a clear, ethical, and presentation‑ready data story

## Business Value
A well‑structured housing dataset unlocks insights for:

### Real‑Estate Professionals
- Spot pricing patterns across property types
- Understand how square footage, bedrooms, and bathrooms impact value

### Investors
- Calculate actionable metrics like price per square foot
- Compare homes using quartile‑based price bands

### Data Teams
- Create a foundation for prediction models and dashboards
- Ensure clear, accurate, and ethical visual communication

## Dataset Description
The dataset contains ~3,000 U.S. residential property records with fields such as:
- Price
- Square Footage (area_sqft)
- Bedrooms & Bathrooms
- Lot Size
- Year Built
- Property Type
- City, State, Zipcode
- Days on Market

A full data dictionary is included in the notebook.

## Key Steps in the Analysis

### 1. Importing & Inspecting the Data
- Verified shape, structure, and schema
- Identified missing values, duplicates, and type issues

### 2. Data Cleaning & Wrangling
- Renamed columns into snake_case
- Removed symbols and characters from numeric fields
- Converted data types correctly
- Handled missing values using industry best practices
- Created engineered features:
  - `price_per_sqft`
  - `price_band` (quartiles)

### 3. Exploratory Data Analysis
- Summary statistics
- Grouped insights
- Distribution checks
- Relationship analysis

### 4. Ethical Visualization Practices
- Non‑misleading scales
- Clear labels & neutral color choices
- Accessibility adjustments
- Chart simplicity & integrity

## Visualizations Included
- **Correlation heatmap**
- **Scatter plot: area vs price**
- **Pair plot with KDE diagonals**
- **Histogram of price**
- **Bar chart by property type**

Each chart includes markdown explaining:
- What question it answers
- Why the chart type fits
- How ethical visualization principles were applied

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
venv\Scripts\activate    # Windows
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
- `Housing Dataset EDA.ipynb` — Main notebook
- `us_house_Sales_data.csv` — Dataset
- `requirements.txt` — Dependencies
- `README.md` — Documentation

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
