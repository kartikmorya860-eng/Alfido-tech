# Zomato Dataset Analysis

## Project Overview
This project performs comprehensive exploratory data analysis (EDA) on the Zomato dataset. It examines restaurant characteristics, ratings, costs, and various other factors to derive meaningful insights about dining establishments and their performance metrics.

## Dataset
- **File**: `zomato.csv`
- **Description**: Contains restaurant data from Zomato including restaurant types, cuisines, locations, ratings, costs, and online order availability.

## Project Structure
```
zomzto data/
├── Zomato_dataset_analysis.ipynb    (Main analysis notebook)
├── zomato.csv                        (Raw dataset)
└── README.md                         (This file)
```

## Notebook Contents

### 1. Data Loading
- Loads the Zomato dataset using pandas
- Handles bad lines during import

### 2. Data Cleaning
- **Duplicate Removal**: Eliminates duplicate records
- **Rate Column Cleaning**: 
  - Removes '/5' suffix
  - Replaces invalid values (NEW, -, empty strings) with NaN
  - Fills missing values with mean rating
- **Cost Column Cleaning**:
  - Removes comma formatting
  - Handles missing and invalid values
  - Fills NaN values with median

### 3. Exploratory Data Analysis (EDA)
Comprehensive analysis including:
- **Data Overview**: Shape, info, missing values, and descriptive statistics
- **Restaurant Types**: Top 10 restaurant types visualization
- **Cuisines**: Top 10 cuisines distribution
- **Locations**: Top 10 restaurant locations
- **Cost Analysis**: Distribution of approximate costs for two people
- **Rating Analysis**: Distribution of restaurant ratings

### 4. Statistical Analysis
- **Two-Sample T-Test**: Compares mean ratings between restaurants offering online delivery vs. those that don't
- **Descriptive Statistics**: Breakdown of ratings by online order availability

## Key Findings

1. **Restaurant Types**: Casual Dining and Quick Bites are the most common restaurant types
2. **Online Delivery Impact**: Restaurants offering online delivery generally have slightly higher ratings
3. **Popular Cuisines**: North Indian, Chinese, and Fast Food are the top cuisines
4. **Top Locations**: BTM Layout, Indiranagar, and Koramangala have the highest number of restaurants
5. **Cost Range**: Most customers spend between ₹200 – ₹600 for two people
6. **Rating Distribution**: Majority of restaurants have ratings between 3.5 and 4.5
7. **Engagement**: Higher-rated restaurants generally have more votes/reviews

## Dependencies
```python
- pandas
- numpy
- matplotlib
- seaborn
- scipy (for statistical tests)
```

## How to Run

1. Ensure you have the required libraries installed:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy
   ```

2. Open the notebook in Jupyter:
   ```bash
   jupyter notebook Zomato_dataset_analysis.ipynb
   ```

3. Execute cells sequentially from top to bottom to:
   - Load the raw data
   - Clean and preprocess the data
   - Generate visualizations
   - Perform statistical analysis

## Data Columns
The dataset includes the following key columns:
- `rate`: Restaurant rating (cleaned from string format)
- `rest_type`: Type of restaurant
- `cuisines`: Cuisines offered
- `location`: Restaurant location
- `approx_cost(for two people)`: Approximate cost for two people
- `online_order`: Whether online orders are available (Yes/No)
- Additional columns with restaurant metadata

## Visualizations Included
- Bar plots for top restaurants, cuisines, and locations
- Histograms for cost and rating distributions
- Statistical comparisons between online and offline restaurants

## Statistical Methods
- **Two-Sample Independent T-Test**: Tests the significance of the difference in mean ratings between restaurants with and without online delivery options
- **Descriptive Statistics**: Mean, median, standard deviation, min, and max values

## Future Enhancements
- Sentiment analysis of reviews
- Predictive modeling for restaurant ratings
- Correlation analysis between different variables
- Time-series analysis if temporal data is available
- Location-based clustering analysis

## Notes
- Missing values in the 'rate' column are filled with the mean rating
- Missing values in the 'approx_cost(for two people)' column are filled with the median cost
- All visualizations include appropriate titles and axis labels
- Results are presented with 2 decimal places for clarity

## Author
Zomato Dataset Analysis - Alfido Tech

## Last Updated
2026-07-11
