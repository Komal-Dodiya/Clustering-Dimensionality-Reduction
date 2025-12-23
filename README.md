# Online Retail Customer Behavior Analysis using Python

## Overview
This project analyzes an online retail dataset to understand customer purchasing behavior and sales patterns using data analysis and data mining techniques. The goal is to extract actionable business insights through exploratory data analysis and customer segmentation.

## Dataset Description
The dataset contains transactional data from an online retail store, including invoice details, product quantities, prices, customer information, and purchase timestamps. The data is primarily UK-centric, with the majority of transactions originating from the United Kingdom.

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Data Cleaning & Preprocessing
- Removed invalid records such as negative quantities (product returns).
- Filtered transactions with zero or negative unit prices.
- Converted `InvoiceDate` to datetime format.
- Cast `CustomerID` to integer type for consistency.
- Created a new feature `TotalAmount` by multiplying Quantity and UnitPrice to represent transaction value.

## Outlier Treatment
- Applied the Interquartile Range (IQR) method to remove outliers from Quantity and UnitPrice.
- Improved data quality and reduced the impact of extreme values on analysis.

## Exploratory Data Analysis (EDA)
- Analyzed data distributions, trends, and purchasing patterns.
- Conducted country-wise transaction analysis, identifying the UK as the primary market.
- Performed product-level analysis showing that a small percentage of products contribute to a large share of total sales (Pareto principle).
- Examined temporal trends and identified seasonal sales peaks during holiday periods.
- Conducted correlation analysis, showing a strong positive relationship between Quantity and TotalAmount.

## Customer Segmentation
- Performed RFM (Recency, Frequency, Monetary) analysis to model customer purchasing behavior.
- Applied K-Means clustering on standardized RFM features to segment customers.
- Used the Elbow Method to determine the optimal number of clusters.
- Evaluated clustering performance using the Silhouette Score to assess cluster quality.

## Key Insights
- Sales are highly concentrated among a small group of products and customers.
- Seasonal trends significantly impact monthly sales performance.
- Customer segmentation revealed distinct purchasing behaviors that can support targeted marketing strategies.

## Conclusion
This analysis demonstrates how data cleaning, exploratory analysis, and unsupervised machine learning techniques can be used to derive meaningful insights from transactional retail data. The findings can help businesses improve customer retention, marketing strategies, and sales performance.

## Author
Komal Dodiya  
Master’s Student in Data Science (STEM OPT Eligible)
