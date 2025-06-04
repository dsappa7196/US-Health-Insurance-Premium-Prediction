# US-Health-Insurance-Premium-Prediction
A data-driven analysis and machine learning model to predict U.S. health insurance charges based on demographic, lifestyle, and health factors. Built using Python, EDA, and Gradient Boosting with 90%+ accuracy.
# 🏥 Health Insurance Premium Prediction

📦 **Project Type**: Data Analysis + Machine Learning | Regression & Risk Modeling  
🎓 **Course**: ISYS 812 – Programming & Applications for Data Analytics  
👩‍💻 **Authors**: Padmasree Sappa, Saptami Biswas  
📁 Tools Used: Python, Pandas, Seaborn, Scikit-learn, Matplotlib, Linear & Ensemble Models

---

## 🧠 Project Overview

As healthcare costs continue to climb, understanding the financial drivers behind insurance pricing has become crucial for providers, policyholders, and regulators alike. This project takes a deep dive into the **U.S. Health Insurance Dataset** to explore how demographic, geographic, and lifestyle-related attributes impact insurance charges.

We used Python and its powerful data analysis stack to uncover patterns in insurance costs, develop new variables (like `Risk Score` and `BMI Category`), and build **machine learning models that predict premiums with over 90% accuracy**. Insights from this analysis can support smarter health policy decisions, fairer pricing strategies, and more personalized insurance plans.

---

## 🎯 Project Goals

1. Identify key attributes (e.g., smoking, BMI, age, region) that impact insurance charges
2. Perform rigorous data cleaning and feature engineering
3. Develop new insights through EDA and risk modeling
4. Build and compare predictive models for premium estimation
5. Deliver actionable recommendations for insurers and policy makers

---

## 📊 Dataset Summary

- 📁 Source: [Kaggle – US Health Insurance Dataset](https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset/data)  
- 👥 1,338 records  
- 💡 7 key features: `Age`, `Sex`, `BMI`, `Children`, `Smoker`, `Region`, `Charges`

### Feature Engineering:
- ➕ `Risk Score`: Combines Age, BMI, and Smoker status into a risk metric
- ➕ `BMI Category`: Underweight / Healthy / Overweight / Obese
- 📦 One-hot encoding for categorical variables

---

## 🔍 Exploratory Insights

- 🚬 **Smoking** is the most influential factor (average smoker pays $32K vs $8K for non-smokers)
- 🎂 **Age** is moderately correlated with charges (older = higher cost)
- 🧍 **BMI** is weakly but positively related to premium charges
- 👶 Number of **children** slightly increases cost but not significantly
- 🌍 **Southeast** region had the highest average charges

---

## 🤖 Predictive Modeling

We trained and evaluated three models:

| Model              | R² Score | MSE            |
|--------------------|----------|----------------|
| Linear Regression  | 0.7996   | 36.8 million   |
| Random Forest      | 0.8840   | 21.3 million   |
| Gradient Boosting  | **0.9007** | **18.2 million** |

✅ Gradient Boosting outperformed others — handling complex, non-linear interactions well

---

## 🛠 Technical Workflow

1. **Data Cleaning**: Removed duplicates, encoded categoricals, handled outliers
2. **EDA**: Used histograms, box plots, heatmaps, and correlation matrices
3. **Feature Engineering**: Derived risk scores, encoded BMI categories
4. **Model Training**: Used 80/20 split with GBM, RF, and Linear Regression
5. **Evaluation**: Compared models on MSE and R², visualized residuals & importance

---

## 📂 Files in This Repository

| File | Description |
|------|-------------|
| [insurance_analysis.ipynb](https://github.com/dsappa7196/seoul-bike-demand-prediction/blob/main/DataMining_SeoulBikeSharingDemand_Project.ipynb) |  Python notebook with full analysis, charts, models |
| [insurance_report.pdf](https://github.com/dsappa7196/seoul-bike-demand-prediction/blob/main/DS861_SeoulBikeSharingDemandPrediction_Sappa.pdf) | Final report covering problem, insights, modeling |
| `README.md`               | This file |

---

## 💼 Business Implications

- 📉 Targeted discounts for low-risk individuals (non-smokers, healthy BMI)
- 📍 Regional premium adjustment strategies
- 🧬 Risk-adjusted pricing models
- 🚭 Policy-driven wellness programs to curb smoking & obesity

---

## 🔮 Future Work

- Add income, employment, or chronic illness data
- Compare to datasets from other countries or states
- Build an interactive tool for premium forecasting
- Apply explainable AI (SHAP) for deeper insights

---

> _“From data to decisions — this project transforms insurance pricing from guesswork to predictive science.”_
