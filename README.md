# 🏨 Hotel Booking Analysis — End-to-End Data Analytics Project

## 📌 Project Overview

This project is a **full-scale, end-to-end data analytics project** that analyzes hotel booking data to uncover:

- What drives **cancellations**
- How **pricing, lead time, and seasonality** affect bookings
- Which **market segments generate the most revenue**
- Where the business is **losing money due to cancellations**

The project follows a **real-world analytics workflow**:

> Raw Data → Excel Audit → Data Cleaning → Python Processing → EDA → Feature Engineering → Dashboard → Business Insights

---

## 🎯 Business Problem

The hotel business faces:

- A **high cancellation rate (~27%)**
- Uncertainty in **revenue forecasting**
- High dependency on **travel agents & specific channels**
- Strong **seasonality effects**

### Business Questions Answered

- Why do customers cancel?
- Which bookings are most risky?
- Which segments bring the most revenue but also the most cancellations?
- How does booking behavior change over time?

---

## 🛠️ Tools & Technologies

- **Python** (Pandas, NumPy)
- **Matplotlib, Seaborn** (Visualization)
- **Excel** (Initial audit & cleaning)
- **Jupyter Notebooks**
- **Git & GitHub** (Project tracking & version control)
- **VS Code**

---

## 📂 Project Structure

hotel-booking-analysis/
│
├── data/
│ ├── excel_cleaned/
│ ├── python_cleaned/
│
├── notebooks/
│ ├── 01_data_understanding.ipynb
│ ├── 04_feature_engineering.ipynb
│ ├── 05_univariate_eda.ipynb
│ ├── 06_bivariate_eda.ipynb
│ ├── 07_multivariate_eda.ipynb
│ ├── 08_time_series_analysis.ipynb
│ ├── 09_dashboard.ipynb
│
├── outputs/
├── requirements.txt
└── README.md


---

## 🔄 Data Pipeline

### 1️⃣ Excel Audit & Cleaning
- Checked missing values, duplicates, invalid rows
- Removed:
  - Invalid ADR bookings
  - Zero-night stays
  - Invalid adult counts
  - Exact duplicates (~31,900 rows)
- Saved clean CSV for Python

### 2️⃣ Python Cleaning & Validation
- Filled missing values (children, agent, company, country)
- Fixed data types
- Removed duplicates again for safety
- Final dataset size: **87,486 rows**

### 3️⃣ Feature Engineering
Created new features:
- `total_guests`
- `total_nights`
- `arrival_date`
- `arrival_month`, `arrival_year`
- `is_family`
- `revenue`

---

## 📊 Exploratory Data Analysis

### Univariate Analysis
- ~27.46% bookings are cancelled
- City Hotels dominate booking volume
- ADR is right-skewed
- Most bookings are for **2 guests**

### Bivariate Analysis
- **Lead time strongly affects cancellation**
- Hotel type affects cancellation behavior
- Price alone is **not** the main driver of cancellation
- Families and non-families show different cancellation patterns

### Multivariate Analysis
- **Lead time is the strongest predictor of cancellations**
- Cancellations show **clear seasonality**, especially for City Hotels
- **Revenue is concentrated in travel agent segments**
- High-revenue channels also have **high cancellation risk**

### Time Series Analysis
- Strong seasonal trends in bookings and revenue
- Cancellation spikes during certain periods
- Clear peaks and troughs across months

---

## 📈 Final Dashboard

The dashboard summarizes:

- Total bookings
- Cancellation rate
- Revenue trends
- Lead time vs cancellation behavior
- Market segment performance
- Hotel-wise cancellation patterns

---

## 🧠 Key Business Insights

- **~27% of all bookings are cancelled** → major revenue risk
- **Lead time is the strongest driver of cancellations**
- **City Hotels are more volatile** than Resort Hotels
- **Travel agent channels generate the most revenue AND the most cancellations**
- Cancellations follow **strong seasonal patterns**

---

## 💡 Business Recommendations

- Introduce **stricter cancellation policies** for high lead-time bookings
- Use **dynamic pricing or partial prepayment** for risky segments
- Focus retention strategies on **high-revenue, high-cancellation channels**
- Use **seasonal forecasting models** for staffing and inventory planning

---

## 🧪 How to Run This Project

```bash
pip install -r requirements.txt



Open notebooks in this order:

01_data_understanding.ipynb

04_feature_engineering.ipynb

05_univariate_eda.ipynb

06_bivariate_eda.ipynb

07_multivariate_eda.ipynb

08_time_series_analysis.ipynb

09_dashboard.ipynb




👤 About Me

I am a Data Analyst / Python Developer with experience in:

  Data cleaning & preprocessing

  Exploratory data analysis

  Business analytics

  Dashboarding

  SQL, Python, Pandas, Tableau

This project demonstrates my ability to handle real-world messy data, build end-to-end pipelines, and extract business insights.

⭐ Why This Project Stands Out

✅ End-to-end workflow (not just charts)

✅ Real data problems (duplicates, missing values, invalid rows)

✅ Business-driven insights

✅ Clean GitHub structure

✅ Reproducible pipeline

✅ Dashboard + Executive Summary