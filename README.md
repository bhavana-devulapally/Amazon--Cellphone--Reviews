
# Amazon Cell-Phone Reviews Analytics Project

## Overview

 The project demonstrates robust data preparation, enrichment, exploratory analysis, and interactive dashboarding to derive actionable insights on model popularity, pricing, and user ratings.

## Features

* **Data Ingestion & Cleaning**: Load raw CSV; remove null and zero-price records; coerce datatypes; deduplicate ASINs; normalize fields.
* **Feature Engineering**: Generate review URLs and convert USD prices to EUR for additional analytical dimensions.
* **Exploratory Analysis**: Compute descriptive statistics, detect outliers, and segment brands by review volume and average rating using Pandas and Matplotlib.
* **Interactive Visualization**: Build Tableau dashboards for brand-level KPIs, rating distributions, and price/rating heatmaps.

## Data Source

* Raw reviews CSV: `cellphone_reviews2023.csv` 

## Tech Stack

* Python 3.8+
* pandas
* matplotlib
* numpy
* Docker & Kubernetes (for containerized services, optional)
* Tableau Desktop (for dashboard visualization)

## Installation

```bash
# Clone the repository
git clone https://github.com/YourUsername/amazon-cellphone-analytics.git
cd amazon-cellphone-analytics

# Install Python dependencies
pip install pandas matplotlib numpy
```

## Usage

1. **Data Cleaning & Enrichment**

   ```bash
   python scripts/clean_data.py --input cellphone_reviews2023.csv --output cleaned_reviews.csv  
   ```
2. **Exploratory Analysis**

   ```bash
   python scripts/explore.py --data cleaned_reviews.csv --output figures/  
   ```
3. **Dashboarding**

   * Open `dashboards/Cellphone_Reviews_Dashboard.twbx` in Tableau Desktop to explore interactive charts.


## Results & Insights

* Samsung Brand leads in average reviews per model with high user ratings.
* Model pricing clusters reveal budget, mid-tier, and premium segments.
* Correlation between high review counts and above-average ratings indicates strong user satisfaction drivers.


