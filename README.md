# Ultra Marathon Data Analysis Project
# 🏃‍♂️🔍

### Overview
This ongoing project is a comprehensive exploration of ultra marathon running events, powered by Python, pandas, and seaborn data science libraries. Currently, it focuses on a subset of the original dataset, containing 7.5 million records.

### Key Steps
### 1. Importing and Exploring Data
The journey begins with importing libraries and examining the dataset. We showcase the first 10 rows, perform shape and data type checks, setting the foundation for further analysis.

### 2. Cleaning and Filtering
Our meticulous cleaning process targets USA races with 50km or 50 miles distances in 2020. Extracting valuable information from event names, calculating athlete ages, and eliminating unnecessary columns refine the dataset.

### 3. Quality Checks
Data integrity is paramount. We conduct checks for duplicate rows and ensure a clean dataset by resetting the index.

### 4. Data Type Conversion and Column Renaming
Maintaining accurate data types is crucial. We convert athlete age to integers and athlete average speed to floats. Column names are streamlined for clarity.

### 5. Plotting graphs with Seaborn 
We utilize Seaborn to visualize key insights. Histograms showcase race lengths, distributions of athlete average speeds, and violin plots provide a comparative view of athlete average speeds across different race lengths and genders. Additionally, a scatter plot explores the relationship between athlete age and average speed.

### 6. **Analyzing Seasonal Trends in Athlete Performance**
   Explore seasonal trends in athlete performance by categorizing races into seasons and analyzing average speeds.
   Additionally, focus on 50mi races and analyze average speeds by season.

```python
df3.query('race_length == "50mi"').groupby('race_season')['athlete_average_speed'].agg(['mean', 'count']).sort_values('mean', ascending=False)
```

## Status
While we've made significant progress, this project is not yet complete. The original dataset, boasting 7.5 million records, holds immense potential for deeper insights. Stay tuned for further developments!

### Note: Explore the code and dive into the cleaned dataset. The original dataset promises a broader perspective on ultra marathon events.
