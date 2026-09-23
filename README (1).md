# Customer Segmentation & Churn Pattern Analytics in European Banking

## 📌 Project Overview

Customer churn is a major challenge in retail banking because losing existing customers can reduce customer lifetime value, increase acquisition costs, and create revenue instability.

This project analyzes customer churn patterns in European banking using customer demographics, geography, financial characteristics, product ownership, engagement, and tenure.

The analysis focuses on identifying customer segments with different levels of churn and understanding the characteristics associated with churn.

---

## 🎯 Objectives

### Primary Objectives

- Calculate the overall customer churn rate.
- Identify churn patterns across customer segments.
- Compare churn behavior across European countries.
- Analyze demographic and financial characteristics of churned customers.

### Secondary Objectives

- Analyze churn among high-value customers.
- Examine the relationship between customer engagement and churn.
- Evaluate tenure and product-ownership patterns.
- Identify customer segments requiring closer retention attention.
- Present findings through an interactive Streamlit dashboard.

---

## 📊 Dataset

The dataset contains customer-level banking information.

| Column | Description |
|---|---|
| CustomerId | Unique customer identifier |
| Surname | Customer surname |
| CreditScore | Customer creditworthiness score |
| Geography | Customer's country: France, Spain, or Germany |
| Gender | Customer gender |
| Age | Customer age |
| Tenure | Number of years with the bank |
| Balance | Customer account balance |
| NumOfProducts | Number of banking products |
| HasCrCard | Credit card ownership indicator |
| IsActiveMember | Customer activity indicator |
| EstimatedSalary | Estimated annual salary |
| Exited | Churn indicator |

`Exited = 1` represents a churned customer and `Exited = 0` represents a retained customer.

---

## 🔍 Analytical Methodology

### 1. Data Ingestion

- Load the dataset using Pandas.
- Inspect dataset dimensions and data types.
- Identify missing and duplicate records.
- Validate categorical and binary variables.

### 2. Data Cleaning

- Remove non-analytical fields such as `Surname`.
- Check missing values.
- Validate binary variables.
- Check numerical ranges and potential outliers.
- Verify churn labels.

### 3. Customer Segmentation

Customers are segmented using:

#### Geography

- France
- Spain
- Germany

#### Age

- Under 30
- 30–45
- 46–60
- 60+

#### Credit Score

- Low
- Medium
- High

#### Tenure

- New
- Mid-term
- Long-term

#### Balance

- Zero Balance
- Low Balance
- High Balance

---

## 📈 Key Analysis

The project analyzes:

- Overall churn rate
- Churn rate by geography
- Churn rate by age group
- Churn rate by gender
- Churn rate by credit score
- Churn rate by tenure
- Churn rate by balance segment
- Churn rate by number of products
- Churn rate by credit-card ownership
- Churn rate by active-member status

---

## 💰 High-Value Customer Analysis

A separate analysis is performed for customers with comparatively high account balances.

The analysis examines:

- High-balance customer churn
- High-balance churn by geography
- High-balance churn by age
- High-balance churn by activity status
- Salary versus balance patterns
- Number of products among high-value customers
- Potential financial exposure associated with churn

---

## 📊 Key Performance Indicators

The dashboard tracks:

- **Overall Churn Rate**
- **Segment Churn Rate**
- **Churned Customer Count**
- **High-Value Customer Churn Rate**
- **Geographic Churn Exposure**
- **Inactive Customer Churn Rate**

---

## 🖥️ Streamlit Dashboard

The project includes an interactive Streamlit dashboard.

### Dashboard Modules

#### 1. Overview

Provides:

- Total customers
- Churned customers
- Overall churn rate
- Average balance
- High-value churn metrics

#### 2. Geography Analysis

Visualizes churn across:

- France
- Spain
- Germany

#### 3. Demographic Analysis

Analyzes churn by:

- Age
- Gender
- Credit score

#### 4. Tenure & Engagement

Analyzes:

- Tenure groups
- Active vs inactive members
- Product ownership

#### 5. High-Value Customer Analysis

Explores churn among customers with high account balances.

#### 6. Customer Explorer

Allows users to apply filters and investigate specific customer segments.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Plotly**
- **Scikit-learn**
- **Streamlit**
- **Jupyter Notebook**
- **SQL**

---

## 📁 Project Structure

```text
customer-churn-european-banking/
│
├── data/
│   └── bank_churn.csv
│
├── notebooks/
│   └── customer_churn_eda.ipynb
│
├── sql/
│   └── churn_analysis.sql
│
├── app/
│   └── streamlit_app.py
│
├── reports/
│   ├── research_paper.pdf
│   └── executive_summary.pdf
│
├── images/
│   └── dashboard_screenshots/
│
├── requirements.txt
├── README.md
└── .gitignore
