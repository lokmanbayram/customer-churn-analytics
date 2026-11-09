# Telco Customer Churn & Revenue Exposure Analytics

An end-to-end analytics project evaluating subscription retention drivers, customer lifetime risk, and recurring revenue exposure across 7,043 customer accounts. Built with a cloud-native data stack leveraging **Neon (PostgreSQL)** for staging/analytical modeling and **Python** for automated ingestion and exploratory data analysis.

---

## Business Problem & Objectives

Customer attrition poses a direct threat to Monthly Recurring Revenue (MRR) in subscription-based services. This project quantifies customer lifecycle friction and segments high-risk cohorts to support targeted retention strategies.

**Core Objectives:**
* Quantify baseline churn rate and aggregate MRR exposure.
* Identify high-risk segments across contract models, onboarding lifecycles, and payment workflows.
* Provide data-driven strategic interventions to mitigate revenue leakage.

---

## Technical Stack & Architecture

* **Database Engine:** PostgreSQL (Serverless instance deployed on Neon)
* **Analysis & Transformation:** Python 3.10+ (`pandas`, `numpy`, `SQLAlchemy`, `psycopg2`)
* **Data Visualization:** `matplotlib`, `seaborn`
* **Development Environment:** VS Code, Google Colab

```text
customer-churn-analytics/
├── data/
│   └── churn_analysis_dashboard.png     # Exported high-resolution dashboard
├── notebooks/
│   └── exploratory_data_analysis.ipynb  # End-to-end data pipeline & visual EDA
├── sql/
│   ├── 01_schema_setup.sql              # Raw staging DDL
│   └── 02_analytical_queries.sql        # Business marts, aggregations, & cohorts
├── .gitignore
├── README.md
└── requirements.txt