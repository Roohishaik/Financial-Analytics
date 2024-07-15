# Financial-Analytics

## Problem Statement
Without analyzing the competition, it is difficult for a business to survive. You are
tasked to analyze the competition for the management to provide better results. This
dataset contains information on the market capitalization of the top 500 companies in
India.
Serial Number, Name, Name of Company, Mar Cap – Crore (Market Capitalization in
Crores), Sales Qtr – Crore (Quarterly Sale in crores) are the columns in the dataset. Find
key metrics and factors and show the meaningful relationships between attributes.
Do your own research and come up with your findings.
## Introduction
1. In the ever-evolving landscape of business, the ability to navigate and thrive in a competitive environment is paramount for sustained success. Without a profound understanding of the competition, businesses face the risk of stagnation or even
failure. Recognizing this imperative, our analysis aims to delve into the dynamics of competition within the Indian corporate landscape, focusing on the market capitalization of the top 500 companies. 

2. The dataset under scrutiny encapsulates
critical information such as Serial Number, Company Name, Market Capitalization, and Quarterly Sales. By leveraging analytical methodologies, we aspire to unearth key
metrics, discern influential factors, and unravel meaningful relationships between attributes. 

3. This investigation is driven by the overarching goal of equipping management with insights that pave the way for informed decision-making, strategic planning, and ultimately, superior business outcomes.

## Code Demonstration
### Libraries

The following python libraries were used to perform the various actions on the dataset from loading to preprocessing to visualizing and predicting the results.
 ```
import numpy as np 
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```
## Analysis Approach
1. Data Loading and Overview
The analysis begins by loading the dataset from the 'Financial Analytics data.csv' file. The initial exploration provides an overview of the dataset,allowing us to understand its structure and content.
# Load data
 ```
file_path = 'Financial Analytics data.csv'
old_df = load_data(file_path)
 ```
# Display basic information about the original dataset
 ```
print("Original DataFrame:")
print(old_df.head())
 ```
2. Handling Missing Values
To ensure the quality of the analysis, missing values are handled by dropping
rows with any missing data. This step ensures that the subsequent analysis is
conducted on a clean dataset.
# Handle missing values and continue with the cleaned DataFrame
 ```
df = handle_missing_values(old_df)
 ```
3. Mean Metrics Calculation
Key metrics, such as the mean market capitalization and mean quarterly sales,
are calculated to provide a central tendency measure for the dataset.
# Calculate mean metrics
 ```
calculate_mean_metrics(df)
 ```
4. Scatter Plot: Market Cap vs. Quarterly Sales
A scatter plot is created to visualize the relationship between market
capitalization and quarterly sales. This plot helps identify trends and patterns
in the data.
# Create scatter plot
 ```
create_scatter_plot(df)
 ```
5. Correlation Matrix
A correlation matrix plot is generated to showcase the relationships between
different attributes, particularly focusing on the correlation between market
capitalization and quarterly sales.
# Create correlation matrix plot
 ```
create_correlation_matrix(df)
 ```
6. Top Companies by Market Capitalization
The analysis includes the identification and display of the top N companies based on market capitalization. This information is valuable for understanding
the market leaders.
# Display top companies based on market capitalization
 ```
top_market_cap_companies(df)
 ```
7. Correlation Analysis
The correlation between market capitalization and quarterly sales is quantified and presented, providing insights into the strength and direction of this
relationship.
# Display correlation between market capitalization and quarterly
 ```
sales
calculate_correlation(df)
 ```
## Conclusion
This competition analysis offers valuable insights into the top 500 companies in India,focusing on market capitalization and quarterly sales. The calculated metrics,visualizations, and correlation analysis provide a comprehensive understanding of thedataset. Further exploration and in-depth analyses can be conducted based on these initial findings to support management decisions and enhance business results.
