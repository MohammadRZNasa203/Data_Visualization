#California Housing Data Analysis

Project Overview:

-This Jupyter Notebook performs exploratory data analysis and visualization on the California Housing dataset. The project demonstrates data loading, preprocessing, exploratory analysis, and visualization techniques using various Python libraries.

Dataset Information:

-Note: While the notebook initially downloads the "coffee-sales" dataset from Kaggle, the actual analysis is performed on the California Housing dataset (california_housing_train.csv).

Dataset Statistics:

-Total Rows: 17,000

-Total Columns: 9

-No Missing Values: All columns have complete data

-No Duplicate Rows: Clean dataset

Project Structure:

1. Installation and Setup:

-Installs Kaggle API client for dataset downloading

-Imports necessary libraries:

-pandas: Data manipulation and analysis

-matplotlib.pyplot: Basic plotting

-seaborn: Statistical data visualization

-plotly.express: Interactive visualizations

-bokeh: Interactive web visualizations

-altair: Declarative statistical visualization

2. Data Loading:

-Loads California Housing dataset from /content/sample_data/california_housing_train.csv

-Note: Despite downloading the coffee-sales dataset, the actual analysis uses California housing data

3. Exploratory Data Analysis:

Basic Exploration:

-Dataset Shape: (17000, 9)

-First 5 Rows Preview: Shows initial data structure

-Data Information: Column names, data types, and non-null counts

-Descriptive Statistics: Count, mean, std, min, percentiles, max for all columns

-Unique Values: Count of unique values per column

Data Quality Checks:

-Missing Values: No missing values detected

-Duplicate Rows: No duplicate rows found

4. Data Preprocessing:
   
-Outlier Removal: Filters out houses with median_house_value >= $500,000

-Feature Engineering: Creates income quartile categories (income_q) based on median_income

5. Data Visualization:
   
Creates a scatter plot using Seaborn showing the relationship between:

-X-axis: median_income

-Y-axis: median_house_value

Visualization Details:

-Uses a sample of 2000 points for better visualization clarity

-Applies transparency (alpha=0.6) for density viewing

-Sets Seaborn theme for improved aesthetics

-Includes descriptive title

#Key Insights from Initial Analysis:

Data Distribution:

-Geographic Coverage: Longitude ranges from -124.35 to -114.31, Latitude from 32.54 to 41.95

-Housing Age: Median housing age ranges from 1 to 52 years

-Room Statistics: Total rooms range from 2 to 37,937 per block

-Income Range: Median income varies from $4,999 to $150,001 (scaled)

-House Values: Median house values range from $14,999 to $500,001

Relationships Observed:

The scatter plot reveals a positive correlation between median income and median house value, suggesting that higher-income areas tend to have more expensive housing.

Dependencies:

-Python 3.12+

Required packages:

-kaggle (1.7.4.5)

-pandas

-matplotlib

-seaborn

-plotly

-bokeh

-altair

Usage Notes :

-The notebook is designed to run in Google Colab environment

-The path to the dataset is hardcoded for Colab's sample data directory

-Visualization libraries are imported but only Seaborn is used in the current analysis

-Additional visualizations using Plotly, Bokeh, and Altair can be implemented as needed
