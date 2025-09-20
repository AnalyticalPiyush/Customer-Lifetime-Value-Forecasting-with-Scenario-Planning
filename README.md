# Customer Lifetime Value Forecasting with Scenario Planning

## 1. Business Problem
Companies spend heavily on acquiring new customers, but not all customers generate equal value. Many churn after one purchase, while a smaller group remains loyal and drives the majority of long-term revenue. Without forecasting and segmentation, businesses risk misallocating marketing budgets and underinvesting in high-value segments.

---

## 2. Objective
- Forecast Customer Lifetime Value (CLV) at the customer and segment level.  
- Enrich data with business attributes such as acquisition channel, CAC, loyalty membership, and seasonality.  
- Test strategic scenarios (retention uplift, loyalty effects, pricing changes, acquisition mix) to identify the most impactful levers for growth.  
- Deliver actionable insights via dashboards and a business-ready report.

---

## 3. Requirements

### Business Requirements
- Identify which customers and channels drive the most long-term value.  
- Quantify ROI of retention and loyalty initiatives.  
- Simulate strategies before making marketing or pricing investments.  

### Technical Requirements
- Data cleaning (remove cancellations, invalid IDs, non-positive transactions).  
- Feature engineering (revenue, acquisition channel, CAC, loyalty flags, seasonality).  
- Exploratory analysis: Cohort retention, RFM segmentation, Pareto 80/20.  
- CLV modelling: heuristic formula and advanced BG/NBD + Gamma-Gamma (Lifetimes).  
- Scenario planning: parameterised simulations for retention, frequency, AOV, and channel mix.  
- Delivery through Power BI dashboard and GitHub repository.

---

## 4. Process
1. **Data Preparation**: Cleaned Online Retail II dataset; created enriched features.  
2. **Exploratory Analysis**: Cohort heatmaps, RFM segmentation, and Pareto distribution to highlight high-value customers.  
3. **CLV Modelling**:  
   - Heuristic: Orders × AOV × Survival × Discounting.  
   - Probabilistic: BG/NBD for purchase frequency + Gamma-Gamma for spend.  
4. **Scenario Planning**: Simulated what-if scenarios for churn reduction, loyalty frequency uplift, price changes, and acquisition mix.  
5. **Deliverables**: Python notebooks, enriched datasets, Power BI dashboard, and slide deck.

---

## 5. Outcome
- Clear segmentation of customers into Low, Mid, High, and Elite CLV groups.  
- Insights on retention patterns across cohorts, with stronger performance from holiday acquisitions.  
- Robust 12-month CLV forecasts per customer, channel, and loyalty segment.  
- Scenario planner demonstrating financial impact of strategic levers.

---

## 6. Results / Insights
- **Top 20% of customers generated ~77% of revenue.**  
- **Loyalty members (24% of customers) contributed 76% of CLV.**  
- **Holiday cohorts delivered up to £120 higher CLV than Jan cohorts.**  
- **Retention uplift (+10%) created the largest CLV increase, more than pricing or frequency changes.**
<img width="1224" height="689" alt="Screenshot 2025-09-11 at 13 33 23" src="https://github.com/user-attachments/assets/db74fda3-d08f-4a61-8f7f-3f69b311b9b1" />
---

## 7. Business Value / Recommendations
- Focus retention efforts on Elite and High-value customers where marginal gains drive disproportionate returns.  
- Expand loyalty programs to convert Potential Loyalists into Loyal/Champions.  
- Prioritize acquisition through Organic and Paid Search channels, which deliver the strongest CLV relative to CAC.  
- Use CLV forecasting to guide marketing budget allocation, ensuring spend aligns with long-term customer profitability.

---

## 8. Summary
This project applies real e-commerce data to forecast Customer Lifetime Value using both heuristic and probabilistic models. By combining exploratory analysis, advanced CLV modelling, and scenario planning, it demonstrates how businesses can quantify customer value, test strategic initiatives, and allocate resources intelligently. Results showed that loyalty and retention are the strongest levers for long-term growth, highlighting the importance of customer-centric strategies in retail and e-commerce.

---

## 📊 Tech Stack
- **Python:** Pandas, NumPy, Matplotlib, Seaborn, Lifetimes, Scikit-learn  
- **Visualization:** Power BI 
- **Data Handling:** OpenPyXL (Excel/CSV I/O)  
- **Version Control:** Git, GitHub  





