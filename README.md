# OTT Platform Churn Analysis & Customer Intelligence
# Overview
This project delivers an end-to-end customer churn analytics pipeline for an Over-The-Top (OTT) streaming platform. By integrating relational subscriber data across demographics, subscription plans, and customer support escalations, this analysis quantifies MRR leakage and customer lifetime value (CLTV) loss, offering actionable strategies to drive subscriber retention.  
# Tech Stack & Tools
Database Management: SQLite (sqlite3)  
Data Processing & Manipulation: Python, Pandas, NumPy  
Data Visualization: Matplotlib, Seaborn  
Analysis & Analytics: Exploratory Data Analysis (EDA), Feature Engineering, SQL Queries  
# Project Architecture & Data Schema
The analysis extracts and connects data across three core relational tables within the customer_churn database:  
db_customer: Demographic details including customerid, name, country, state, gender, dob, interests, and pincode.  
db_subscription: Plan configurations including subscription_start_date, subscription_type, renewal_date, plan_type (Basic/Standard/Premium), contract_type, cancellation_date, cancellation_reason, monthly_charges, cltv, and churn_score.  
db_support: Escalation data including complaint_date, escalations, csat_score, and customer feedback.  
# Key Metrics & Formulas Implemented
 

# Key Insights & Analytics Findings
Overall Churn Profile: The platform exhibits an overall 28.6% Churn Rate (71.4% Retention Rate). 
Contract Length Disparity: Monthly contract subscribers churn at 55.6%, compared to only 8.3% for annual contract subscribers (a 6.7x difference). 
Financial Impact:
Total Revenue: $395 | Revenue Loss due to Churn: $74 (18% revenue loss). 
Total CLTV Lost: $2,047 across high-risk cohorts.  
Geographic & Temporal Trends: Churn spiked significantly in September 2024, with the highest concentration of churned users originating from Karnataka. 
Plan Tier Impact: The majority of churned users were concentrated in the Basic subscription plan.  
# Strategic Action Items
Contract Migration Strategy: Incentivise high-risk monthly subscribers to transition into annual plans to mitigate short-term attrition. 
Root-Cause Investigation: Investigate localized price increases, feature rollouts, or service outages in Karnataka corresponding to the September 2024 spike.  
Support-Driven Retention: Prioritise high-LTV customers exhibiting high/medium churn risk scores and unresolved escalation tickets via targeted outreach.
Competitor Benchmarking: Conduct competitive analysis on Basic tier pricing and content library offerings to address competitor switching drivers.  
# Workflow & Roadmap
Database Integration: Connect Python to SQLite database via sqlite3 and pandas.  
Data Cleaning & QC: Validate data types, handle missing values, and standardize schemas. 
Feature Engineering: Calculate customer tenure, aging metrics, and risk flags. 
Exploratory Data Analysis: Aggregate, pivot, and segment cohorts by contract, region, and tier.  
Visualization & Reporting: Build distribution plots, correlation maps, and executive summary slides. 
