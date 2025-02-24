

# Mall Statistics Project

This project aims to analyze and visualize shopping trends in a mall using the provided dataset. The dataset contains various features such as customer demographics, purchase behavior, and location information.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Data Preparation](#data-preparation)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Data Visualization](#data-visualization)
5. [Conclusion](#conclusion)

## Project Structure

The project structure is as follows:

```
Mall Statistics/
│   README.md
│   shopping_trends.csv
│
└───Notebooks/
    │   MainNotebook.ipynb
```

## Data Preparation

The dataset, `shopping_trends.csv`, was loaded into a pandas DataFrame for further analysis. The following steps were performed:

1. Checked for missing values using the `isnull().sum()` function.
2. Checked for duplicates using the `duplicated().sum()` function.
3. Calculated the correlation matrix for numerical columns using the `corr()` function.
4. Created a heatmap of the correlation matrix using seaborn's `heatmap()` function.
5. One-hot encoded the 'gender' column and made it binary (0 and 1) using pandas' `get_dummies()` function.
6. Label encoded string columns (excluding 'gender') using pandas' `astype('category').cat.codes` attribute.
7. Dropped the 'Customer ID' column from the DataFrame.

## Exploratory Data Analysis (EDA)

The following exploratory data analysis was performed:

1. Calculated the correlation matrix for all columns using the `corr()` function.
2. Created a heatmap of the correlation matrix using seaborn's `heatmap()` function.
3. Created histograms of the numerical columns to visualize their distributions.
4. Created a countplot of the 'product_category' column to visualize the distribution of product categories.
5. Created a countplot of the 'gender' column to visualize the distribution of genders.
6. Created a bar chart to visualize the top 5 product categories for each gender.
7. Created a bar chart to visualize the total purchase amount for each gender.
8. Created a bar chart to visualize the top 10 locations with the highest total purchase amount.
9. Created a horizontal bar chart to visualize the count of each payment method.

## Data Visualization

The following data visualizations were created:

1. Correlation matrix heatmap for all columns.
2. Side-by-side bar chart comparing the purchase amount by gender.
3. Bar chart comparing the purchase amount by the top 5 locations.
4. Horizontal bar chart comparing the purchase amount by the top 10 locations.
5. Bar chart showing the count of each payment method.

## Conclusion

The exploratory data analysis and data visualization provided valuable insights into the shopping trends in the mall. The correlation matrix highlighted the relationships between different features, and the data visualizations allowed for a better understanding of the distribution and patterns in the data. Further analysis and modeling can be performed based on these findings to improve the shopping experience and make informed decisions.
