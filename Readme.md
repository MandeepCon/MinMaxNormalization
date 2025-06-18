#  Min-Max Normalization Workshop
 
## Overview
 
This project demonstrates how to apply **Min-Max Normalization** on a real-world housing dataset. The objective is to prepare the data for machine learning models by scaling all numeric features to a uniform range [0, 1], preventing any one feature from dominating due to its scale.
 
---
 
##  Dataset
 
**File:** `housing_data.csv`  
**Description:** Contains 2,000 rows and 7 columns including house price, area, number of rooms, lot size, and year built.
 
| Column Name     | Description                     |
|-----------------|---------------------------------|
| House_ID        | Unique identifier for each house|
| Price           | Sale price of the house         |
| Area_sqft       | Area in square feet             |
| Num_Bedrooms    | Number of bedrooms              |
| Num_Bathrooms   | Number of bathrooms             |
| Year_Built      | Year of construction            |
| Lot_Size        | Lot size in square feet         |
 
---
 
##  EDA (Exploratory Data Analysis)
 
###  Cleaning
- Checked for missing values → None found.
- Checked for duplicates → None found.
 
###  Boxplots
- Identified outliers in features like `Price` and `Lot_Size`.
 
###  Scatter Plots
- Visualized relationships between `Price` and other features like `Area_sqft`, `Lot_Size`.
 
###  Correlation Heatmap
- Revealed positive correlation between `Price` and `Area_sqft`/`Lot_Size`.
 
---
 
##  Normalization Process
 
###  Manual Min-Max Normalization
 
We normalized all numeric columns manually using the formula:
 
\[
x_{\text{norm}} = \frac{x - x_{\text{min}}}{x_{\text{max}} - x_{\text{min}}}
\]
 
This was implemented using pure Python and Pandas — no `sklearn` or `numpy` used.
 
### Outcome:
- All numeric features scaled to the range [0, 1].
- Dataset ready for use in algorithms like KNN, Linear Regression, or Neural Networks.
 
---
 
##  Technologies Used
 
- Python
- Pandas
- Matplotlib & Seaborn for visualization
- Jupyter Notebook
 
---
 
##  Team Information
 
- Course: *Foundations of Machine Learning Frameworks*
-  Team: 8
-  Members:
1. Hasyashri Bhatt
2. Mandeep Singh
3. Babandeep
 
---
 
## Status
 
- EDA Completed  
- Data Cleaned  
- Min-Max Normalization Applied  
- Visualizations Included
 
---
 
##  How to Run
 
1. Open the notebook `MinMax_Normalization_Workshop.ipynb`.
2. Run each cell in sequence:
   - EDA and Visualization
   - Manual Normalization
   - Normalized Output Preview