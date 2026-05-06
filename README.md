# 🛒 Customer Churn Prediction — Olist E-commerce Dataset
 
## 📌 Project Overview
This project predicts whether an e-commerce customer will churn (stop purchasing) using real-world data from the **Olist Brazilian E-commerce Dataset**. The goal is to help businesses identify at-risk customers and take proactive retention actions.
 
---
 
## 🎯 Problem Statement
**Can we predict which customers are likely to churn based on their purchase behaviour, payment patterns, and review scores?**
 
- **Churn Definition:** A customer who has not made a purchase in the last 180 days is considered churned.
---
 
## 📂 Dataset
- **Source:** [Olist Brazilian E-commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- **Size:** 99,441 orders | 96,096 unique customers
- **Tables Used:**
  - olist_customers_dataset.csv
  - olist_orders_dataset.csv
  - olist_order_items_dataset.csv
  - olist_order_payments_dataset.csv
  - olist_order_reviews_dataset.csv
---
 
## 🔧 Tools & Technologies
| Tool | Purpose |
|------|---------|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Computing |
| Matplotlib & Seaborn | Data Visualization |
| Scikit-learn | Machine Learning |
| Jupyter Notebook | Development Environment |
 
---
 
## 📊 Project Workflow
 
```
Step 1 → Import Libraries
Step 2 → Load Datasets
Step 3 → Merge Datasets
Step 4 → Define Churn
Step 5 → Feature Engineering
Step 6 → Data Cleaning
Step 7 → Exploratory Data Analysis (EDA)
Step 8 → Model Building
Step 9 → Model Evaluation (ROC Curve & Feature Importance)
```
 
---
 
## 🧠 Features Used
| Feature | Description |
|---------|-------------|
| total_orders | Total number of orders placed |
| total_spend | Total amount spent |
| avg_spend | Average spend per order |
| avg_review_score | Average review score given |
| avg_installments | Average payment installments |
 
---
 
## 📈 EDA Insights
- **70.88% churn rate** — majority of customers churned
- Churned customers tend to have **lower total orders**
- **Total spend and avg spend** are the strongest predictors of churn
- Review score alone is **not a reliable predictor** of churn
---
 
## 🤖 Models Built
| Model | Accuracy | AUC Score |
|-------|----------|-----------|
| Logistic Regression | 54.14% | 0.56 |
| Random Forest | 60.10% | 0.65 |
 
✅ **Random Forest** outperformed Logistic Regression with higher accuracy and AUC score!
 
---
 
## 📉 Challenges & Solutions
| Challenge | Solution |
|-----------|---------|
| Class Imbalance (70% churned) | Applied undersampling to balance classes |
| Data Leakage | Removed `days_since_last_purchase` from features |
| Missing Values | Filled with median/default values |
 
---
 
## 📊 Visualizations
### EDA Charts
![EDA Charts](images/eda_charts.png)
 
### Model Evaluation
![Model Evaluation](images/model_evaluation.png)
 
---
 
## 💡 Business Insights
1. Customers who purchase **only once** are most likely to churn
2. **High spenders** are less likely to churn — focus retention on low spenders
3. **Review score alone** cannot predict churn — need behavioural data
4. Businesses should target customers with **low avg spend and few orders** with special offers
---
 
## 🚀 How to Run
1. Clone this repository
2. Install required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
3. Open `notebooks/churn_prediction.ipynb` in Jupyter Notebook
4. Run all cells in order
---
 
## 👩‍💻 Author
**Keerthana Gurunathan**
- 📧 keerthanagurunathan.98@gmail.com
- 🐙 [GitHub](https://github.com/Keetna-github)
---
 
⭐ If you found this project helpful, please give it a star!
