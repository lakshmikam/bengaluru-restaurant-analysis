# Bengaluru Restaurant Data Analysis

## Project Overview

This project presents an end-to-end data cleaning, feature engineering, and exploratory data analysis of restaurant listings in Bengaluru. The dataset was preprocessed to remove inconsistencies, handle missing values, eliminate duplicates, and create structured features for meaningful business analysis.

The objective of this analysis was to evaluate how pricing, popularity, location, and operational factors influence restaurant ratings and engagement.

---

## Dataset Information

- Total valid entries after cleaning: 844
- Location: Bengaluru
- Data includes restaurant-level attributes such as:
  - Rating
  - Votes
  - Cost for two
  - Service type
  - Cuisine type
  - Online ordering availability
  - Table booking availability

---

## Data Cleaning Steps

- Removed redundant columns (address, phone, reviews_list)
- Standardized column names
- Converted rating from string format (e.g., "3.8/5") to float
- Removed invalid entries ("NEW", "-")
- Cleaned and converted cost column to numeric format
- Dropped duplicate records (40 duplicates removed)
- Handled missing values
- Standardized categorical values (location, service type)

---

## Feature Engineering

The following derived features were created:

- `high_rated` → 1 if rating ≥ 4.0, else 0  
- `price_category` → budget / mid_range / premium  
- `vote_category` → low / medium / high engagement  
- `multi_cuisine` → 1 if restaurant serves 3+ cuisines  

---

## Key Analytical Questions & Findings

### 1. Pricing Sweet Spot
- Correlation between cost and rating: **-0.01**
- Conclusion: Higher pricing does not guarantee better ratings.

### 2. Popularity vs Rating (Hype Factor)
- Correlation between votes and rating: **0.01**
- Conclusion: Higher engagement does not necessarily reflect higher quality.

### 3. Geographical Trends
- Indiranagar has the highest concentration of high-rated restaurants.
- Certain areas function as stronger dining hubs.

### 4. Operational Insights
- Table booking availability does not significantly increase engagement.
- Rating variation across top chains shows moderate consistency.

### 5. Price Category Insights
- Mid-range restaurants show slightly stronger median ratings.

---

## Tools & Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## Project Structure
