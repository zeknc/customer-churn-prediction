# 🎯 Customer Churn Prediction System

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3.0-orange.svg)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28-red.svg)](https://streamlit.io/)

An end-to-end data science project designed to predict customer churn in E-commerce and Telecom sectors using machine learning algorithms.

---

## 📋 Project Overview

This project utilizes a telecom company's dataset containing 7,000+ customer records to predict which customers are highly likely to leave the company (churn) with an accuracy of **80.5%**.

### 🎯 Project Objectives
- Early detection of high-risk customer churn.
- Identifying key drivers influencing customer attrition.
- Serving predictions via an interactive web dashboard.
- Proposing data-driven customer retention strategies.

---

## 🚀 Key Features

✅ **Comprehensive Exploratory Data Analysis (EDA)**
- In-depth analysis of 21 unique customer attributes.
- Statistical hypothesis testing (Chi-Square Test, T-Test).
- 15+ rich data visualizations.

✅ **Machine Learning Modeling Pipeline**
- Logistic Regression
- Random Forest
- XGBoost (Champion Model: 80.5% accuracy)

✅ **Advanced Feature Engineering**
- Customer tenure grouping.
- Average monthly spend indicators.
- Charge-to-tenure ratio metrics.

✅ **Interactive Web Dashboard**
- Developed using Streamlit framework.
- Real-time churn probability estimation.
- Risk scoring and categorization system.
- Executive visual reporting.

---

## 📊 Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | AUC |
|-------|----------|-----------|--------|----------|-----|
| Logistic Regression | 78.0% | 0.65 | 0.52 | 0.55 | 0.84 |
| Random Forest | 79.0% | 0.66 | 0.55 | 0.58 | 0.85 |
| **XGBoost** | **80.5%** | **0.67** | **0.54** | **0.60** | **0.86** |

🏆 **XGBoost** emerged as the champion model across key classification metrics.

---

## 🔍 Key Insights & Findings

### Top Churn Risk Drivers:
1. **Contract Type:** Customers with Month-to-Month contracts have a 42% churn rate (compared to only 3% for 2-year contracts).
2. **Tenure:** Churn risk spikes above 50% within the first 12 months of customer acquisition.
3. **Internet Service Type:** Fiber optic subscribers experience a high churn rate of 41%.
4. **Payment Method:** Electronic check users show a 45% churn rate.
5. **Monthly Charges:** Customers paying $70+ represent a significantly higher risk tier.

### 💡 Business Recommendations:
- Implement specialized onboarding and support programs during the critical first 12 months.
- Incentivize month-to-month subscribers to transition into long-term annual contracts.
- Audit and optimize service quality for fiber optic infrastructure to reduce attrition.
- Promote automated billing cycles to decrease dependency on manual electronic checks.

---

## 🛠️ Tech Stack

### Data Processing & Analytics
- **Python 3.10**
- **Pandas** - Data manipulation and profiling
- **NumPy** - Vectorized numerical computations
- **Matplotlib & Seaborn** - Statistical visualizations

### Machine Learning & Modeling
- **Scikit-learn** - Preprocessing, pipeline optimization, and baseline modeling
- **XGBoost** - Advanced gradient boosting implementation
- **Imbalanced-learn** - Handling class imbalance challenges

### Frontend & Deployment UI
- **Streamlit** - Interactive dashboard deployment
- **Plotly** - Dynamic, interactive data charting

### Ecosystem Tools
- **Jupyter Notebook** - Prototyping and sandbox EDA
- **Git & GitHub** - Version control and collaboration
- **Kaggle** - Primary data repository source

---

## 📁 Repository Structure
customer-churn-prediction/
│
├── data/
│   ├── raw/                           # Raw source files (CSV)
│   └── processed/                     # Serialization outputs (PKL)
│
├── notebooks/
│   ├── 01_eda.ipynb                   # Exploratory Data Analysis
│   └── 02_preprocessing_modeling.ipynb # Feature processing & ML development
│
├── models/
│   ├── random_forest_model.pkl       # Serialized Random Forest model
│   ├── xgboost_model.pkl             # Serialized Champion XGBoost model
│   └── scaler.pkl                     # Standardized feature scaler
│
├── app/
│   └── dashboard.py                   # Streamlit analytics dashboard
│
├── requirements.txt                   # Dependency environment manifest
└── README.md

## 🚀 Installation & Deployment Guide

### 1. Clone the Repository
```bash
git clone [https://github.com/zeknc/customer-churn-prediction.git](https://github.com/zeknc/customer-churn-prediction.git)
cd customer-churn-prediction

Install Project Dependencies
pip install -r requirements.txt

Retrieve the Dataset
Download the source data from Kaggle - Telco Customer Churn

Save the WA_Fn-UseC_-Telco-Customer-Churn.csv file into the data/raw/ directory.

Execute the Modeling Pipeline
jupyter notebook
# Open and execute 01_eda.ipynb and 02_preprocessing_modeling.ipynb sequentially.

Launch the Web Interface
cd app
streamlit run dashboard.py

The app will instantly serve locally at: http://localhost:8501

📊 Dashboard Architecture
📈 Data Exploration Tab
High-level demographic breakdown metrics.

Historical churn volume distributions.

Granular cross-tabulations on contract variables.

🤖 Predictive Inference Tab
Input customizable customer attributes (gender, contract type, pricing tier, etc.).

Trigger the "Predict" algorithm.

Review the real-time churn probability percentage and tactical retention suggestions.

📊 Model Diagnostics Tab
Comparative performance tracking charts.

Detailed classification confusion matrices.

Algorithmic evaluation scorecards.

📈 Executive Impact & Milestones
Business Value
Discovered an baseline 27% churn rate in legacy operations.

Established an infrastructure capable of predicting risk vectors with 80.5% accuracy.

Highlighted the first 12 months as the high-attrition danger zone.

Extracted and defined the 4 primary operational risk drivers.

Technical Achievements
Built an end-to-end production-ready machine learning lifecycle pipeline.

Benchmarked and tuned multiple algorithms simultaneously.

Enhanced classification metrics via targeted predictive feature engineering.

Delivered an executive-facing interactive software prototype.

🎓 Core Competencies Developed
Through this project implementation:

✅ Real-world dataset cleaning and outlier management.

✅ Statistical hypothesis verification frameworks.

✅ Automated data transformation and alignment pipelines.

✅ Supervised classification architecture development.

✅ Rigorous model evaluation, selection, and diagnostics.

✅ Deployment of analytic web web frameworks.

✅ Modern Git/GitHub version control workflows.

🔮 Roadmap & Future Enhancements
[ ] Evaluate alternative gradient boosting architectures (CatBoost, LightGBM).

[ ] Implement hyperparameter optimization frameworks (GridSearchCV, Optuna).

[ ] Inject model interpretability metrics via SHAP / LIME values.

[ ] Expose real-time prediction interfaces via a lightweight REST API.

[ ] Containerize the full environment stack using Docker.

[ ] Configure CI/CD automated deployment pathways to cloud infrastructure (AWS/Azure).

[ ] Integrate an automated dynamic A/B testing simulation module.

👨‍💻 Developer Profile
Name: Zehra Ekinci

LinkedIn: linkedin.com/in/zehra-ekinci-264496253

Email: zhrekncr7@gmail.com

GitHub: @zeknc

📝 License
This project is open-source and licensed under the terms of the MIT License.

🙏 Acknowledgments
Data Attribution: Kaggle - Telco Customer Churn Dataset

Inspiration: Solving high-impact, real-world corporate business problems through algorithmic intelligence.

📞 Contact & Support
For queries, bug reports, or deep-dives:

Feel free to open a GitHub Issue in this repository.

Connect via professional message on LinkedIn.

⭐ If you find this project valuable, please consider leaving a star!
