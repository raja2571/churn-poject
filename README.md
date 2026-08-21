# 🚀 AI-Powered Customer Churn Prediction with Explainable AI (LLM)

## 📌 Project Overview

Customer churn is one of the biggest challenges faced by subscription-based businesses such as telecom companies, banks, insurance providers, and SaaS platforms. Acquiring a new customer is significantly more expensive than retaining an existing one. Therefore, identifying customers who are likely to leave the service is essential for improving customer retention and reducing revenue loss.

This project presents an end-to-end AI-powered Customer Churn Prediction System that combines Machine Learning, Explainable AI, Large Language Models (LLMs), and Business Intelligence to predict customer churn and generate human-readable explanations for each prediction.

Unlike traditional churn prediction models that only classify customers as "Churn" or "No Churn", this project uses a Large Language Model (Groq LLM) to explain *why* a customer is likely to churn and recommends personalized retention strategies.

---

# 🎯 Problem Statement

Telecom companies lose a significant number of customers every year due to competition, pricing, service quality, and customer dissatisfaction.

Traditional machine learning models only predict whether a customer will churn (0 or 1), but they do not answer important business questions such as:

- Why will this customer churn?
- Which customer attributes influenced the prediction?
- What actions should the company take to retain the customer?

This project solves these challenges by integrating Machine Learning with a Large Language Model (LLM) to generate business-friendly explanations and recommendations.

---

# 🎯 Objectives

- Predict whether a customer will churn.
- Identify important factors influencing churn.
- Generate AI-powered explanations for predictions.
- Recommend customer retention strategies.
- Visualize business insights using Power BI.
- Build an end-to-end business intelligence solution.

---

# 📊 Dataset

Dataset: Telecom Customer Churn Dataset

Features include:

- Customer ID
- Gender
- Senior Citizen
- Partner
- Dependents
- Tenure
- Phone Service
- Multiple Lines
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming TV
- Streaming Movies
- Contract
- Paperless Billing
- Payment Method
- Monthly Charges
- Total Charges
- Churn (Target Variable)

Target Variable:

- 0 → Customer Stays
- 1 → Customer Churns

---

# 🏗️ Project Architecture

```
                    Dataset
                       │
                       ▼
             Data Cleaning & Preprocessing
                       │
                       ▼
             Feature Engineering & Encoding
                       │
                       ▼
                Feature Scaling
            (StandardScaler)
                       │
                       ▼
          Machine Learning Models
      ┌─────────────────────────────────┐
      │ Logistic Regression             │
      │ Decision Tree                   │
      │ Random Forest                   │
      │ XGBoost                         │
      └─────────────────────────────────┘
                       │
                       ▼
           Best Model Selection
        (Logistic Regression)
                       │
                       ▼
          Hyperparameter Tuning
                       │
                       ▼
          Customer Churn Prediction
                       │
                       ▼
         Prediction Probability Score
                       │
                       ▼
          Groq LLM Integration
 (AI Explanation & Retention Strategy)
                       │
                       ▼
             Power BI Dashboard
```

---

# ⚙️ Workflow

### 1. Data Collection

- Load Telecom Customer Churn dataset into Google Colab.

---

### 2. Data Cleaning

- Handle missing values
- Convert TotalCharges to numeric
- Remove incorrect values
- Verify data types

---

### 3. Data Preprocessing

- Label Encoding
- One-Hot Encoding
- Feature Selection
- Train-Test Split
- StandardScaler

---

### 4. Model Training

The following models were trained:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

---

### 5. Model Evaluation

Evaluation Metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

### 6. Hyperparameter Tuning

GridSearchCV was applied to optimize Logistic Regression and improve prediction performance.

---

### 7. AI Explainability

Instead of showing:

```
Prediction = 1
```

The system generates:

```
Prediction:
Customer is likely to churn.

Reasons:

• High Monthly Charges
• Month-to-Month Contract
• Low Tenure
• No Tech Support
• No Online Security

Recommendation:

• Offer annual plan
• Provide discount
• Free technical support
```

---

# 🤖 LLM Integration

The project integrates Groq LLM (`openai/gpt-oss-120b`) to generate:

- Human-readable explanations
- Churn reasons
- Customer summaries
- Retention recommendations
- Business insights

Prompt Engineering is used to convert prediction outputs into meaningful business decisions.

---

# 📈 Power BI Dashboard

The project includes an interactive Power BI dashboard.

### Dashboard Pages

## 1. Summary Dashboard

- Total Customers
- Churn Customers
- Churn Rate
- Churn vs Non-Churn
- Contract Type Analysis

---

## 2. Demographic Analysis

- Gender Analysis
- Senior Citizen Analysis
- Partner Analysis
- Dependents Analysis

---

## 3. Account Analysis

- Contract Type
- Payment Method
- Monthly Charges
- Tenure

---

## 4. Service Usage

- Internet Service
- Tech Support
- Streaming TV
- Streaming Movies
- Online Security

---

## 5. AI Prediction Dashboard

Displays

- Customer Prediction
- Confidence Score
- AI Explanation
- Retention Recommendation

---

# 💻 Technologies Used

### Programming

- Python

### Notebook

- Google Colab

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Groq SDK

### Machine Learning

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

### Explainable AI

- Groq LLM
- Prompt Engineering

### Data Visualization

- Power BI

### Version Control

- Git
- GitHub

---

# 📂 Project Structure

```
Customer-Churn-Prediction/
│
├── Dataset/
│
├── Notebook/
│   ├── churn_prediction.ipynb
│
├── PowerBI/
│   ├── ChurnDashboard.pbix
│
├── Reports/
│   ├── Customer_Churn_AI_Report.csv
│
├── README.md
│
└── requirements.txt
```

---

# 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- Classification Report

---

# 🚀 Future Enhancements

- SHAP-based Explainable AI
- Streamlit Web Application
- Real-time Prediction API
- Customer Risk Score
- Multi-Language AI Explanations
- Email Generation for Customer Retention
- AI Chatbot for Business Users
- Deployment on Hugging Face Spaces
- Docker Containerization
- Cloud Deployment (AWS / Azure / GCP)

---

# 🎯 Key Features

✅ Customer Churn Prediction

✅ AI-Powered Business Explanations

✅ Customer Retention Recommendations

✅ Hyperparameter Tuning

✅ Explainable AI

✅ Interactive Power BI Dashboard

✅ Google Colab Implementation

✅ End-to-End Machine Learning Pipeline

---

# 📌 Results

- Logistic Regression achieved the best overall performance.
- AI explanations provide understandable reasons for predictions.
- Business recommendations help customer retention teams make informed decisions.
- Interactive dashboards support better decision-making.

---

# 👨‍💻 Author

**Raja Reddy**

MCA Student | AI & Machine Learning Enthusiast

Skills:
Python • SQL • Machine Learning • Power BI • Explainable AI • LLM Integration • Data Analytics
