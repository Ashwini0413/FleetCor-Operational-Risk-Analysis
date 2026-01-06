# FleetCor Cross-Sell Strategy Optimization

## Project Overview
This project focuses on optimizing FleetCor’s **cross-sell strategy** by identifying high-potential Fuel-Only cardholders who should be upgraded to **Universal Cards**, while minimizing credit risk and write-offs. The solution combines **predictive modeling, KPI analysis, and interactive dashboards** to drive data-backed business decisions.

The goal was to enhance profitability by improving eligibility rules, optimizing credit line utilization (CLI), and refining probability cutoffs.

---

## Business Objective
- Increase **net financial gain** from cross-selling Universal Cards  
- Reduce **credit risk and write-offs**
- Identify **profitable swap-in** and **low-performing swap-out** customers
- Provide decision-makers with **real-time insights** using dashboards

---

## Modeling Approach
- Primary Model: Random Forest  
- Baseline Model: Logistic Regression  
- Final Accuracy: 99.33% (Random Forest)

### Key Predictive Features
| Feature | Importance |
|------|------|
| DAYS_PAST_DUE | Highest |
| FUEL_SPEND_RATIO | High |
| CREDIT_LIMIT | Moderate |

Less impactful variables (e.g., `BAL_90_PLUS`) were removed to reduce noise and improve performance.

---

## Key Insights
- **CLI% > 50K** leads to a sharp increase in write-off risk  
- **Optimal profitability range:** CLI between **20K–40K**  
- Universal Cardholders:
  - Higher spend ($111K avg)
  - Slightly higher write-offs ($2.97K avg)
  - Strong net value contribution

---

## Strategy Optimization
- Lowered probability cutoff from **0.5 → 0.4**
- Resulted in:
  - **31.59K profitable swap-ins**
  - **$2M reduction** in risky CLI exposure
  - **$1.2M estimated net gain**

---

## KPIs Tracked
- Total Net Gain: **~$1.17B**
- Total Write-Offs: **$37.81M**
- CLI Utilization: **$1.14M**
- Customers Analyzed: **~180K**

---

## Power BI Dashboard
The interactive dashboard enables real-time monitoring and scenario analysis with views such as:
- Cross-Sell Eligibility Effectiveness  
- CLI% vs Bad Rate  
- Fuel vs Universal Card Performance  
- Model Prediction Results  
- Eligibility Policy Impact  

---

## Tools & Technologies
- **Languages:** R, Python  
- **Visualization:** Power BI  
- **Data Handling:** Excel  
- **Models:** Random Forest, Logistic Regression  

---

## Final Recommendations
- Target customers with **prediction probability > 0.7**
- Cap **CLI at 40K** for mid-risk profiles
- Integrate external variables (industry, company size, tenure)
- Retrain models **semi-annually**
- Implement automated **CLI risk alerts**

---

## Impact
This project demonstrates how **advanced analytics and machine learning** can directly influence **profitability, risk management, and policy decisions** in financial services.

---

## Author
**Venkat Sai Ashwini Molakaluri**  
Master’s in Business Analytics (Global Supply Chain)  
Skills: R | Python | SQL | Power BI | Predictive Modeling | Business Analytics

