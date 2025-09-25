# Linear Regression - Housing Price Prediction

This repository demonstrating linear regression techniques for predicting housing prices based on various features from a housing dataset.

## Contents

- **3.Linear Regression.ipynb**  
  Step-by-step notebook covering:
  - Data exploration and preprocessing
  - Feature encoding and scaling
  - Correlation analysis
  - Simple linear regression with area as predictor
  - Data visualization

- **Housing.csv**  
  The dataset used for analysis. Contains information on house price, area, bedrooms, bathrooms, stories, and other features.

---

## About the Data

The dataset (`Housing.csv`) contains 545 records of houses with the following attributes:

- **price**: Sale price of the house (numeric)
- **area**: Area of the house in square feet (numeric)
- **bedrooms**: Number of bedrooms (numeric)
- **bathrooms**: Number of bathrooms (numeric)
- **stories**: Number of stories (numeric)
- **mainroad**: Whether the house is on the main road (yes/no)
- **guestroom**: Availability of guest room (yes/no)
- **basement**: Availability of basement (yes/no)
- **hotwaterheating**: Availability of hot water heating (yes/no)
- **airconditioning**: Availability of air conditioning (yes/no)
- **parking**: Number of parking spaces (numeric)
- **prefarea**: Located in a preferred area (yes/no)
- **furnishingstatus**: Furnishing status (furnished/semi-furnished/unfurnished)

There are no missing or duplicate values in the dataset. Categorical columns are encoded for analysis.

---

## About the Code

The notebook walks through:

1. **Data Loading & Inspection**  
   - Loads the CSV into a pandas DataFrame
   - Shows summary statistics and checks for missing/duplicate values

2. **Feature Processing**
   - Binary categorical columns (yes/no) converted to 1/0
   - Multi-category columns (`furnishingstatus`) one-hot encoded
   - Numerical columns scaled using MinMaxScaler

3. **Exploratory Data Analysis**
   - Displays correlation matrix and visualizes relationships (e.g., area vs price)
   - Scatter and heatmap plots for feature relationships

4. **Simple Linear Regression**
   - Predicts house price using area as the sole feature
   - Splits data into train/test sets
   - Trains and evaluates a linear regression model using scikit-learn

5. **Visualization**
   - Plots model results and feature relationships for interpretation

---
