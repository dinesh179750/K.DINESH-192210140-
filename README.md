Car Price Analysis Notebook
This notebook performs an exploratory data analysis (EDA) on a car dataset to understand various factors influencing car prices.

Table of Contents
Introduction,
Data Loading and Initial Inspection,
Data Cleaning and Preprocessing,
Exploratory Data Analysis (EDA),
Descriptive Statistics,
Feature Normalization,
Data Binning,
Visualizations,
Libraries Used.
1. Introduction
This project aims to analyze a dataset of car features to identify key relationships and patterns that affect car prices. The notebook covers data loading, cleaning, transformation, and various visualizations to gain insights into the data.

2. Data Loading and Initial Inspection
The dataset data.csv is loaded into a pandas DataFrame.
Initial inspection includes viewing the head of the DataFrame and assigning appropriate headers to columns.
3. Data Cleaning and Preprocessing
Missing values represented by '?' are handled, specifically by removing rows where 'price' is missing.
Data types are converted for relevant columns (e.g., 'price' to integer).
Feature normalization is applied to 'length', 'width', and 'height' to scale values between 0 and 1.
'city-mpg' is converted to 'city-L / 100km' for better interpretation.
Price data is binned into 'Low', 'Medium', and 'High' categories.
4. Exploratory Data Analysis (EDA)
Descriptive Statistics: data.describe() provides a statistical summary of the numerical features.
Visualizations:
Histograms of binned price to understand price distribution.
Box plots of 'price' against 'drive-wheels' to compare price distributions across different drive types.
Scatter plot of 'engine-size' vs 'price' to visualize their relationship.
Pivot tables and heatmaps (plt.pcolor) to show the average price based on 'drive-wheels' and 'body-style'.
5. Libraries Used
pandas: For data manipulation and analysis.
numpy: For numerical operations.
matplotlib.pyplot: For creating static, interactive, and animated visualizations.
seaborn: For drawing attractive and informative statistical graphics.
scipy: For scientific computing (though its direct use for the currently visible cells is minimal, it was imported).
