# OTT Subscription Churn & Customer Intelligence Analysis

##  Executive Summary
Analyzed subscriber behavior, revenue leakage, and service support data across **4,188 customers** to uncover churn drivers for a digital subscription platform. 

While baseline contract terms showed minimal difference in retention, customer support escalations proved to be the single strongest predictor of churn ($r \approx 0.43$).

---

##  Key Business Metrics
- **Overall Churn Rate:** 28.15% (Retention Rate: 71.85%)
- **Monthly Recurring Revenue (MRR):** ₹70,381.12
- **Direct Revenue Leakage:** ₹19,483.21/month (~27.7% of monthly revenue)
- **Cumulative CLTV Lost:** ₹730,645+ across churned cohorts
- **Average Customer Tenure:** 1,752 days (~4.8 years)
- **Average Revenue Per User (ARPU):** ₹16.81

---

##  Core Findings
1. **The Escalation Trap:** 
   - Customers with escalated support tickets exhibited a **~43% correlation with cancellation**. 
   - Service dissatisfaction—not pricing—is the primary driver of subscriber departure.
2. **Uniform Plan Churn:** 
   - Standard (32.3%), Basic (32.0%), and Premium (31.3%) have near-identical churn rates, indicating churn is tier-agnostic.
3. **Contract Duration Insensitivity:** 
   - Monthly churn (29.3%) and Annual churn (27.2%) show no major delta, disproving the assumption that annual lock-ins alone solve retention.
4. **Seasonal Volatility:** 
   - Cancellations peaked sharply in **December (~151 customers)** compared to the annual low in **February (~101 customers)**.
5. **Geographic Variance:** 
   - Highest churn observed in Nigeria (32.1%), South Africa (31.3%), and Mexico (31.0%); lowest in Canada (20.5%).

---

##  Strategic Recommendations
- **SLA Alert for Support Escalations:** Implement automated retention outreach (e.g., credit extensions, dedicated account executive) within 24 hours of an escalation flag (`Y`).
- **Q4 Churn Prevention Playbook:** Run proactive engagement, holiday discount offers, and content premieres ahead of the November–December cancellation window.
- **Service Audit for High-Churn Markets:** Investigate payment gateways and content localization in regions exceeding 30% churn (Nigeria, South Africa, Egypt, Mexico).

---

##  Tech Stack
- **Database Extraction:** MySQL, `mysql.connector`
- **Data Engineering & Manipulation:** Python, Pandas, NumPy
- **Exploratory Data Analysis & Visualization:** Matplotlib, Seaborn
