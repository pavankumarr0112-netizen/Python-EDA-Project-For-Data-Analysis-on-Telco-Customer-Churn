# 📊 Customer Churn Analysis – Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of a Customer Churn dataset. The main goal is to understand customer behavior and identify the key factors that influence whether a customer churns (leaves the service) or not.

The dataset contains **7043 rows and 21 columns**, including customer demographics, services subscribed, contract details, payment methods, and churn status .

---

## 📂 Dataset Information

The dataset includes:

* Customer details (gender, SeniorCitizen, Partner, Dependents)
* Account information (tenure, Contract, PaymentMethod, MonthlyCharges, TotalCharges)
* Services used (InternetService, OnlineSecurity, TechSupport, StreamingTV, etc.)
* Target variable: **Churn (Yes/No)**

From the dataset summary shown in the project:

* Total records: **7043**
* No missing values after cleaning
* `TotalCharges` was converted from object to float by replacing blank values with 0 .

---

## 🛠️ Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 🧹 Data Cleaning Steps

1. Loaded dataset using Pandas.
2. Checked dataset shape and column details.
3. Replaced blank values in `TotalCharges` with 0 and converted to float .
4. Verified missing values (no null values found).
5. Checked duplicate records (no duplicates found).
6. Converted `SeniorCitizen` values from 0/1 to Yes/No format .

---

## 📊 Key Analysis Performed

### 1️⃣ Overall Churn Analysis

* Around **26.54% of customers have churned**, while 73.46% stayed .
* Visualized using count plots and pie charts.

---

### 2️⃣ Churn by Gender

* Churn rate is almost similar between male and female customers .

---

### 3️⃣ Churn by Senior Citizens

* A higher percentage of **Senior Citizens** have churned compared to non-senior customers .

---

### 4️⃣ Churn by Tenure

* Customers who stayed longer (higher tenure) are less likely to churn.
* Customers with 1–2 months tenure have higher churn probability .

---

### 5️⃣ Churn by Contract Type

* Customers with **Month-to-month contracts** are more likely to churn.
* Customers with **One-year or Two-year contracts** are more stable .

---

### 6️⃣ Churn by Services Used

Customers who do not churn generally have:

* PhoneService
* DSL Internet
* OnlineSecurity enabled

Higher churn observed when:

* OnlineBackup not used
* TechSupport not used
* Streaming services unavailable .

---

### 7️⃣ Churn by Payment Method

* Customers using **Electronic Check** are more likely to churn compared to other payment methods .

---

## 📈 Key Insights

* Short tenure customers are high risk.
* Month-to-month contracts increase churn probability.
* Lack of additional services like TechSupport and OnlineSecurity increases churn.
* Electronic check users show higher churn behavior.
* Senior citizens show comparatively higher churn percentage.

---

## 🎯 Conclusion

This project helps identify the major factors contributing to customer churn. The insights gained from EDA can be used to:

* Improve customer retention strategies
* Offer better contract plans
* Promote additional services
* Target high-risk customers early

This analysis forms a strong foundation for building a **machine learning churn prediction model** in future work.

---

## 🚀 Future Improvements

* Perform feature engineering
* Apply machine learning models
* Build churn prediction dashboard
* Deploy model for real-time prediction

---

