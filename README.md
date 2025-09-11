# 📉 Employee Attrition Analysis: Prediction and Causation

🚨 **What makes an employee leave a company? Can we predict it, and can we understand the root causes?**

This project performs a comprehensive analysis of employee attrition in two stages. First, it identifies key factors and builds a machine learning model to **predict** which employees are at high risk of leaving. Second, it moves beyond prediction to conduct a **causal inference** analysis, aiming to understand the true drivers that *cause* employees to resign.

---

##  📊Notebooks

This project is divided into two main parts, each in its own Jupyter Notebook:

* **1. 📊 [Predictive Modeling: `[employee_attrition.ipynb](https://github.com/viniciuscatelani/Employee-Churn/blob/main/employee_attrition.ipynb)`](#)**
    * This notebook covers the full exploratory data analysis (EDA), feature engineering, and the development of a LightGBM model to predict employee churn.

* **2. 🔎 [Causal Inference: `[employee_attrition_causal_inference.ipynb](https://github.com/viniciuscatelani/Employee-Churn/blob/main/employee_attrition_causal_inference.ipynb)`](#)**
    * This notebook goes a step further to answer "why." It uses the `DoWhy` library and Directed Acyclic Graphs (DAGs) to estimate the causal impact of specific factors like overtime, work-life balance, and business travel on attrition.

---

## 📌 Objectives

-   Analyze employee attrition behavior through detailed EDA.
-   Build a high-performing predictive model to estimate the likelihood of attrition.
-   Move beyond correlation to identify the **causal drivers** of attrition using causal inference techniques.
-   Provide nuanced, actionable insights to help reduce employee turnover.

---

## 📊 Dataset

-   **Source:** [Kaggle - Employee Attrition Dataset](https://www.kaggle.com/datasets/patelprashant/employee-attrition)
-   **Contains:** Demographic and professional data from employees of a company.
-   **Target Variable:** `Attrition` (indicates whether the employee left the company).

---

## 🧪 Techniques Used

#### Predictive Modeling
-   Exploratory Data Analysis (EDA)
-   Interactive Visualizations (Plotly, Seaborn)
-   Modeling with LightGBM and CatBoost
-   Model Evaluation (Recall, Confusion Matrix, Classification Report)

#### Causal Inference
-   Causal Reasoning and Model Specification
-   Directed Acyclic Graphs (DAGs)
-   Causal Effect Estimation with the `DoWhy` Library
-   Backdoor Criterion and Confounder Adjustment
-   Propensity Score Matching and Linear Regression Estimators

---

## 🧠 Key Insights

This project highlights the crucial difference between prediction and causation.

#### Predictive Insights (Correlations)
-   Features like **OverTime**, **JobRole**, and **StockOptionLevel** showed the strongest correlation with attrition and were the most important features in the predictive model.

#### Causal Insights (Causes)
-   **The Overtime Illusion:** While `OverTime` was the top predictor, its direct causal effect on attrition was found to be very small **(~1%)** after controlling for a comprehensive set of confounders. This suggests overtime is more of a symptom of other underlying issues than a primary cause itself.
-   **Direct Causal Drivers:** Low **Environment Satisfaction** (+11%) and **Frequent Business Travel** (+9.9%) were identified as significant, direct causal drivers of an employee's decision to leave.
-   **Complex Factors:** The causal link between **Work-Life Balance** and attrition was found to be statistically insignificant, suggesting a more complex relationship heavily influenced by unobservable factors like employee resilience.

---

## ⚙️ How to Run

Clone this repository:
```bash
git clone [https://github.com/your-username/employee-attrition.git](https://github.com/your-username/employee-attrition.git)
```
Install requirements:
```pip install -r requirements.txt```

Run the notebook:
```
jupyter notebook employee_attrition.ipynb
jupyter notebook employee_attrition_causal_inference.ipynb
```

---

## 📁 Project Structure

employee-attrition/
│
├── data/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── employee_attrition.ipynb
├── employee_attrition_causal_inference.ipynb
├── README.md
└── requirements.txt

## 🤝 Contribution

Contributions are welcome! Feel free to open issues or submit pull requests with improvements, bug fixes, or new ideas.

---

This project was developed for learning purposes and to enhance my Data Science portfolio.
