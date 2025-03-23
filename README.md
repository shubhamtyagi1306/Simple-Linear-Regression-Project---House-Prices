# Simple-Linear-Regression-Project---House-Prices
This project builds a Simple Linear Regression model to predict house prices based on area.

## **1. Steps Followed in the Project**

### **Step 1: Load Dataset**
- Read the dataset containing house prices and area.
- Display the first few rows to understand its structure.

### **Step 2: Exploratory Data Analysis (EDA)**
- Check dataset information (`df.info()`) and statistics (`df.describe()`).
- Identify missing values and clean the data if there is any missing value.
- Visualize the dataset using a pair plot.

### **Step 3: Data Preprocessing**
- Handle missing values by dropping them if there is any missing value in the dataset.
- Select **area** as the independent variable (X) and **price** as the dependent variable (y).

### **Step 4: Train-Test Split**
- Split the dataset into **80% training data** and **20% testing data**.

### **Step 5: Train the Model**
- Use **Simple Linear Regression** from `sklearn.linear_model` to train the model.

### **Step 6: Model Evaluation**
- Predict house prices for the test set.
- Evaluate the model using:
  - **Mean Squared Error (MSE)** → Measures error in price predictions.
  - **R-squared (R²)** → Measures how well the model explains price variation.

### **Step 7: Visualization**
- Plot actual vs. predicted prices.
- Visualize the regression line on test data.
- Check for linearity using a regression plot.

---

## **2. Model Performance Analysis**
### **Key Findings**
- **High MSE** and **Low R² (~0.30)** indicate poor model performance.
- **area alone does not explain house price variations well.**

### **Why is R² Low?**
1. **Missing Important Features**: bedrooms, bathrooms, age, etc., are missing.
2. **Data Scaling Issues**: Large numeric differences between features might affect regression.

---

## **3. How to Improve the Model?**
From our project, we observed a low R-squared value (~0.30), meaning our Simple Linear Regression model does not explain most of the variability in house prices. The key reason is missing important features: Prices depend on many factors (e.g., location, number of bedrooms, age, amenities), but we only used area as the predictor as we are building the project in Simple Linear Regression algorithm.
The current model is too simplistic and does not capture all the factors influencing house prices. By adding more features and trying advanced models like Multiple Linear regression or Decision Tree or Random Forest, we can significantly improve accuracy and business impact.
---
