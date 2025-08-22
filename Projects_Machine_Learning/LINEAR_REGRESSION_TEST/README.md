# Car Price Prediction using Linear Regression

This repository contains a Jupyter Notebook that walks through the process of building and evaluating different regression models to predict car selling prices.  

## 📌 Project Overview
The goal of this project is to use machine learning regression techniques to predict the selling price of cars based on their features (year, mileage, fuel type, transmission, etc.).  
We experimented with **Linear Regression, Lasso, Ridge, and Polynomial Regression**, and compared their performances.

---

## 🔑 Steps in the Notebook

### 1. Data Cleaning & Preprocessing
- Understood the meaning of each dataset column (brand, model, year, selling_price, km_driven, fuel type, seller type, transmission).
- Handled **missing values**:
  - Explained why missing target values cannot be used.
  - Discussed trade-offs between dropping vs. filling missing values.
  - Used median imputation for skewed data.

### 2. Exploratory Data Analysis (EDA)
- Visualized data distributions.
- Checked for skewness and correlations.
- Identified features influencing selling price the most.

### 3. Feature Engineering
- Converted categorical features (e.g., fuel, seller_type, transmission) into numerical form.
- Scaled numeric values for better model performance.

### 4. Model Training
- **Linear Regression**: Baseline model.
- **Lasso Regression**: Tested feature selection by shrinking coefficients.
- **Ridge Regression**: Handled multicollinearity with regularization (GridSearchCV used to find best alpha).
- **Polynomial Regression**: Tried higher-order terms to capture non-linear relationships.

### 5. Model Evaluation
- Compared models using performance metrics (e.g., R², MAE, RMSE).
- Discussed scenarios where polynomial regression might be useful.

### 6. Findings & Insights
- Summarized which model performed best overall and why.
- Highlighted trade-offs between underfitting and overfitting.
- Suggested possible improvements (feature engineering, hyperparameter tuning, or advanced models).

---

## 📊 Results Summary
- **Linear Regression**: Simple, interpretable, but limited in capturing complex patterns.  
- **Lasso Regression**: Useful for feature selection but may underfit.  
- **Ridge Regression**: Balanced trade-off, performed better with regularization.  
- **Polynomial Regression**: Captured non-linear trends but risked overfitting.  

**Best Model:** Ridge Regression (based on evaluation metrics and generalization).  

---

## 🚀 Next Steps
- Tune hyperparameters further.
- Try ensemble methods (Random Forest, Gradient Boosting).
- Deploy as a web app for car price prediction.

---

## 📂 Files in this Repository
- `Linear_Regression_Test_Loryne.ipynb` – Main notebook with full workflow.
- `README.md` – This documentation.

---

## 🛠️ Tech Stack
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)
- Jupyter Notebook
