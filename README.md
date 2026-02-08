# Loan Approval Prediction System

A Machine Learning project developed to automate the loan eligibility process based on customer details provided in online application forms. The model predicts whether a loan will be approved or rejected based on features like Credit History, Income, and Education.

## 📌 Project Overview
The goal of this project is to build a classification model that helps financial institutions streamline their loan approval process. By analyzing historical data, we identify the key factors that influence loan eligibility.

## 🚀 Key Features
* **Data Cleaning:** Implemented Mode and Median imputation for missing values in `Credit_History`, `Self_Employed`, and `LoanAmount`.
* **Feature Engineering:** * Created a `Total_Income` feature by combining Applicant and Co-applicant incomes.
    * Applied **Log Transformations** to handle skewed data and outliers in income and loan amounts.
* **Exploratory Data Analysis (EDA):** Performed correlation analysis using Heatmaps and analyzed categorical relationships with Loan Status.
* **Model Training:** Built and compared **Logistic Regression** and **Random Forest Classifier**.
* **Model Evaluation:** Achieved a validation accuracy of **83%** and used **5-Fold Cross-Validation** for robust performance estimation.

![Correlation Heatmap](images/heatmap.png)

## 🛠️ Technologies Used
* **Python** (Core Logic)
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-learn** (Machine Learning & Evaluation)

## 📊 Results & Insights
* **Top Predictor:** `Credit_History` was found to be the most influential factor (0.54 correlation with Loan Status).
* **Income Influence:** Total household income significantly impacts the model's decision-making process.
* **Model Accuracy:** * Validation Accuracy: **~83%**
    * Mean CV Accuracy: **~78%**

## 📂 Project Structure
```text
├── data/
│   ├── train.csv           # Training dataset
│   └── test.csv            # Independent test dataset
├── notebooks/
│   └── loan_prediction.ipynb # Full Jupyter notebook with EDA and Modeling
├── models/
│   └── loan_model.pkl      # Saved Random Forest model
├── README.md               # Project documentation
└── submission.csv          # Final predictions for the test set
