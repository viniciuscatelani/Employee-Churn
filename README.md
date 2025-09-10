# 📉 Employee Attrition Analysis and Prediction

🚨 **What makes an employee leave a company? Can we predict it in advance?**

In this project, I performed a detailed analysis of an employee attrition dataset to identify the main factors associated with exits and build a predictive model to anticipate such cases.

---

## 📌 Objectives

- Analyze employee attrition behavior
- Identify key factors related to churn
- Build predictive models to estimate the likelihood of attrition
- Provide actionable insights to help reduce employee turnover

---

## 📊 Dataset

- Source: [Kaggle - Employee Attrition Dataset](https://www.kaggle.com/datasets/patelprashant/employee-attrition)
- Contains demographic and professional data from employees of a company
- Target variable: Attrition (indicates whether the employee left the company)

---

## 🧪 Techniques Used

- Exploratory Data Analysis (EDA)
- Statistical Testing
- Interactive Visualizations (Plotly, Seaborn)
- Modeling with LightGBM and CatBoost
- Evaluation based on Recall, Confusion Matrix, and Classification Report

---

## 🧠 Key Insights

- Features like **JobRole**, **OverTime**, and **StockOptionLevel** showed strong correlation with attrition.
- Frequent business travel and certain departments are more prone to churn.
- The final model performed well in identifying high-risk employee profiles.

---

## ⚙️ How to Run

Clone this repository:
```git clone https://github.com/your-username/employee-attrition.git```

Install requirements:
```pip install -r requirements.txt```

Run the notebook:
```jupyter notebook employee_attrition.ipynb```

---

## 📁 Project Structure

employee-attrition/
│
├── data/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── employee_attrition.ipynb
├── README.md
└── requirements.txt

## 🤝 Contribution

Contributions are welcome! Feel free to open issues or submit pull requests with improvements, bug fixes, or new ideas.

---

This project was developed for learning purposes and to enhance my Data Science portfolio.
