# 🚀 OTT Subscriber Churn Intelligence & Revenue Impact Pipeline

An end-to-end data analytics and customer intelligence pipeline built for an OTT subscription platform to predict high-risk subscriber churn, quantify Monthly Recurring Revenue (MRR) leakage, and analyze support escalation drivers[cite: 9, 15, 16].

---

## 📌 Project Overview
In the hyper-competitive streaming and subscription landscape, retaining existing users is critical for sustained profitability[cite: 9]. This project integrates multi-table relational databases with Python to extract, clean, and analyze subscriber behavior, subscription tiers, and support escalations[cite: 9, 12, 15]. 

The goal is to transition from raw data tracking to actionable business intelligence—identifying why users leave, when they churn, and how to mitigate revenue loss[cite: 11, 15].

---

## 🛠️ Tech Stack & Libraries
* **Database Management:** SQLite / SQL Server (`sqlite3`)[cite: 10]
* **Data Manipulation & Cleaning:** Python, Pandas, NumPy[cite: 10]
* **Exploratory Data Analysis (EDA):** Aggregations, Group-Bys, Pivot Tables[cite: 10]
* **Data Visualization:** Matplotlib, Seaborn[cite: 10]
* **Environment:** Jupyter Notebook / Python Scripting

---

## 🗄️ Relational Database Schema (`customer_churn`)
The project utilizes a multi-table relational architecture joined via Python:
1. **`db_customer`**: Demographics data (Customer ID, Name, Country, State, Gender, DOB, Interests)[cite: 12].
2. **`db_subscription`**: Subscription lifecycle data (Plan Type, Contract Type, Start/Renewal/Cancellation Dates, Monthly Charges, CLTV, Churn Score)[cite: 12, 13].
3. **`db_support`**: Customer service interactions (Escalations, Complaint Dates, CSAT Scores, Comments)[cite: 12, 13].

---

## 📊 Key Performance Indicators (KPIs) & Metrics Tracked
* **Overall Churn Rate & Retention Rate** (28.6% Churn / 71.4% Retention)[cite: 13, 14]
* **Average Revenue Per User (ARPU)** & Customer Lifetime Value (CLTV)[cite: 13, 14]
* **Segmented Churn Analysis:** Monthly contract vs. Annual contract churn disparity[cite: 15, 16]
* **Revenue at Risk & MRR Leakage** due to high-risk churn scores ($>70$)[cite: 13, 14]
* **Support Intelligence:** Escalation rate, average complaints per customer, and correlation between support tickets and churn[cite: 13, 15].

---

## 🔍 Key Business Insights & Findings
* **Contract Disparity:** Monthly-contract subscribers exhibited a **55.6% churn rate**, which is **6.7 times higher** than the **8.3% churn rate** seen in annual-contract subscribers[cite: 14, 16].
* **Financial Impact:** Identified **$73.94/mo in MRR leakage** and **$2,047 in CLTV erosion** concentrated within high-risk cohorts[cite: 16].
* **Geographic & Temporal Trends:** High churn spikes were isolated during specific periods (e.g., September) with localized spikes observed in regions like Karnataka[cite: 14].
* **Support Correlation:** Support escalations and unresolved complaints were disproportionately concentrated among churned customers, pointing to immediate product and service bottlenecks[cite: 15].

---

## 💡 Strategic Action Items & Recommendations
1. **Contract Migration Strategy:** Push aggressive discount incentives or bundled perks to convert monthly subscribers onto annual billing plans[cite: 15, 16].
2. **Proactive Intervention:** Prioritize retention outreach (via targeted emails, SMS, or calls) for users flagged with 'High' or 'Medium' churn scores before cancellation requests occur[cite: 14, 15].
3. **Customer Support Audit:** Investigate support ticket bottlenecks in high-churn regions (e.g., Karnataka) to drastically reduce escalations and improve CSAT scores[cite: 14].

---

## 📁 Repository Structure
```text
📦 OTT-Subscriber-Churn-Intelligence-Pipeline
│
├── 📂 data                # Raw and processed CSV datasets / SQLite DB
├── 📂 notebooks           # Jupyter Notebooks (SQL integration, EDA, Viz)
├── 📂 visualisations      # Generated Matplotlib & Seaborn charts
├── 📄 requirements.txt    # Required Python libraries (pandas, numpy, etc.)
└── 📄 README.md           # Project documentation
