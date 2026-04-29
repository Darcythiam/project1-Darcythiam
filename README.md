# Minnesota Housing Price Prediction (Machine Learning Project)

## Project Overview

This project applies machine learning techniques to predict Minnesota housing prices using demographic and geographic data.

The work is structured in two stages:

- **Baseline Modeling** – data exploration, preprocessing, and initial model training  
- **Model Improvement & Regularization** – improving generalization using advanced techniques  

Together, these stages demonstrate a complete and iterative machine learning workflow.

---

## Notebooks

| Notebook | Purpose |
|---|---|
| `Project1_MN_Housing.ipynb` | Baseline model: EDA, preprocessing, and initial regression models |
| `Project3_Regularized_Regression_MN_Housing.ipynb` | Extended work: regularization, model tuning, and improved generalization |

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

## Workflow

### 1. Exploratory Data Analysis
- Histograms, scatter plots, correlation analysis  
- Identified median income as the strongest predictor  

---

### 2. Data Preparation
- Missing value handling  
- Feature scaling  
- Feature engineering  

Engineered features:
- Rooms per household  
- Bedrooms per room  
- Population per household  

---

### 3. Train/Test Split
- Stratified sampling based on income categories  
- Preserved data distribution  

---

### 4. Baseline Models (Project 1)
- Linear Regression (baseline)  
- Decision Tree (overfitting observed)  
- Random Forest (best initial performance)  

---

### 5. Model Improvement (Project 3)
- Regularization techniques to reduce overfitting  
- Improved generalization performance  
- Model tuning and refinement  

---

### 6. Evaluation
- Root Mean Squared Error (RMSE)  
- Cross-validation  

| Model | Result |
|------|--------|
| Linear Regression | Strong baseline |
| Decision Tree | Overfit |
| Random Forest | Best performance |

---

### 7. Feature Importance
Key predictors:
1. Median income  
2. Geographic location  
3. Engineered housing density features  

Median income was the dominant feature.

---

## Technologies

- Python  
- Pandas, NumPy  
- Matplotlib  
- Scikit-learn  

---

## Key Takeaways

- Feature engineering significantly improves performance  
- Decision Trees are prone to overfitting without control  
- Random Forest provides strong baseline performance  
- Regularization improves model generalization  

---

## Skills Demonstrated

- Regression modeling  
- Feature engineering  
- Model evaluation  
- Cross-validation  
- Regularization techniques  

---

## Running the Project

```bash
pip install pandas numpy matplotlib scikit-learn
jupyter notebook Project1_MN_Housing.ipynb