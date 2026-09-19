# 📊 Telecom Customer Churn Analysis & Machine Learning Prediction System

An end-to-end Telecom Customer Churn solution integrating **Interactive Power BI Dashboards** for business intelligence and a **Gradient Boosting Machine Learning Model** deployed via **FastAPI** for real-time churn risk scoring.

---

## 📌 Executive Summary

Customer churn is a critical metric in the telecommunications industry. This project aims to analyze historical customer behavior, identify key retention drivers, and deploy a predictive engine to flag high-risk customers before they churn.

- **Total Customers Analyzed:** ~7.03K
- **Overall Churn Rate:** 26.58%
- **Total Revenue Lost to Churn:** $2.86M ($139K Monthly)
- **High Risk Customers Identified:** 148 (~$11.91K monthly revenue at immediate risk)

---

## 🛠️ Tech Stack & Tools

- **Business Intelligence & Visualization:** Power BI, DAX, Data Modeling
- **Machine Learning & Analytics:** Python, Pandas, Scikit-Learn (Gradient Boosting)
- **Deployment & API:** FastAPI, Uvicorn, RESTful API
- **Version Control:** Git, GitHub

---

## 📉 Dashboard Key Insights & Structure

The Power BI report consists of **5 dedicated interactive pages**:

### 1. Executive Overview
- Highlights macro KPIs: Churn Rate (26.58%), Revenue Loss ($2.86M).
- **Key Finding:** Month-to-month contracts account for the highest churn rate (42.71%), while electronic check is the most vulnerable payment method ($84K lost revenue).

### 2. Customer Demographics
- Analyzes churn by gender, senior status, and tenure.
- **Key Finding:** Senior citizens living alone show a significantly higher churn rate (up to 50%). Customers with higher monthly charges ($70 - $100) are most likely to churn (39.87%).

### 3. Services Breakdown
- Evaluates service adoption vs. customer loss.
- **Key Finding:** Fiber Optic users exhibit a high churn rate (41.9%), and customers without Technical Support show an 83.4% churn proportion within their segment.

### 4. Retention & Predictive Risk
- Combines historical metrics with ML model prediction outputs.
- Displays a real-time risk leaderboard sorted by predicted churn probability (>70%) to enable proactive customer outreach.

### 5. Predictive Insights & ML Model Overview
- Explains the Machine Learning architecture, handling class imbalance, critical retention windows (first 3-6 months), and integration points with FastAPI.

---

## 🤖 Machine Learning Model & Deployment

- **Algorithm:** Gradient Boosting Classifier
- **Class Imbalance Handling:** Weighted loss functions/balanced class weights to adjust for the ~26% churn baseline.
- **Critical Retention Window:** Early tenure (0-6 months) identified as the primary intervention window.
- **API Deployment:** Integrated via **FastAPI** endpoints for real-time scoring.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.9+
- Power BI Desktop (for opening `.pbix` file)

### Installation & API Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Alikamer22/telecom-churn-prediction.git](https://github.com/Alikamer22/telecom-churn-prediction.git)
   cd telecom-churn-prediction
