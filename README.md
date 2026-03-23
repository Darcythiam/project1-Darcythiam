# Minnesota Housing Price Prediction (Machine Learning Project)

## Project Overview

This project applies machine learning techniques to predict Minnesota housing prices using demographic and geographic data. The project follows a complete data science workflow including exploratory data analysis, preprocessing, model training, hyperparameter tuning, and performance evaluation.

This project demonstrates practical skills in:

- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Machine learning modeling
- Model evaluation and optimization
- Data visualization

---

## Dataset

The dataset contains housing information including:

- Median income
- Total rooms
- Total bedrooms
- Population
- Households
- Latitude
- Longitude
- Median house value (target variable)

The goal is to predict **median house value** using these features.

---

## Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Scikit-learn

### Machine Learning Methods

- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- GridSearchCV
- Cross Validation
- Feature Importance Analysis

---

## Project Workflow

### 1. Exploratory Data Analysis

Explored distributions and relationships between variables using:

- Histograms
- Scatter plots
- Correlation matrices

Key finding:

Median income showed the strongest correlation with housing prices.

---

### 2. Data Preparation

Data preparation included:

- Handling missing values
- Feature scaling
- Feature engineering
- Data transformation

Engineered features included:

- Rooms per household
- Bedrooms per room
- Population per household

These features improved model performance.

---

### 3. Train/Test Split

Used **stratified sampling** based on income categories to maintain representative distributions across training and testing datasets.

---

### 4. Model Training

Models trained:

### Linear Regression

Used as baseline model for comparison.

### Decision Tree

Achieved very low training error but showed overfitting.

### Random Forest

Provided the best performance due to reduced variance and improved generalization.

---

### 5. Hyperparameter Tuning

Used **GridSearchCV** to optimize:

- Number of estimators
- Maximum features
- Tree depth

This improved predictive accuracy.

---

### 6. Model Evaluation

Models evaluated using:

- Root Mean Squared Error (RMSE)
- Cross Validation

| Model | Result |
|------|--------|
| Linear Regression | Strong baseline |
| Decision Tree | Overfit |
| Random Forest | Best performance |

Random Forest produced the most reliable results.

---

### 7. Feature Importance

Most important predictors identified:

1. Median income
2. Geographic location
3. Engineered housing density features

Median income was the dominant predictor.

---

## Installation

Install dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn

Run notebook:

jupyter notebook Project1_MN_Housing.ipynb

