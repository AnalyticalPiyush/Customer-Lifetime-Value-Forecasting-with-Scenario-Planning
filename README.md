# Customer Lifetime Value Forecasting with Scenario Planning

## Project Overview
This project develops **Customer Lifetime Value (CLV) models** using real e-commerce data (Online Retail II, UCI/Kaggle).  
The aim is to show how not all customers are equally valuable and how businesses can forecast long-term value, segment customers, and test strategic what-if scenarios.  

The project combines:
- **Data Cleaning & Enrichment** (channels, CAC, loyalty, seasonality)
- **Exploratory Analysis** (cohort retention, RFM segmentation, Pareto rule)
- **CLV Modelling** (heuristic + probabilistic BG/NBD + Gamma-Gamma)
- **Scenario Planning** (retention uplift, loyalty programs, pricing strategy, channel mix)

---

## Methodology

### 1. Data Preparation
- Removed cancellations and non-positive transactions.  
- Calculated revenue per order.  
- Added synthetic business features:  
- Acquisition channel (Paid Search, Organic, Social, Referral, Email)  
- CAC (channel-specific acquisition cost)  
- Loyalty flag (~25% customers as members)  
- Seasonality index (holiday uplift, January dip)  

### 2. Exploratory Analysis
- Cohort Analysis:** measured retention across acquisition months.  
- RFM Segmentation:** grouped customers into Champions, Loyal, Potential Loyalists, At Risk, and Lost.  
- Pareto Analysis:** confirmed the top 20% of customers generated ~77% of revenue.  

### 3. CLV Modelling
- Heuristic CLV: Orders × Average Order Value × Survival × Discounting.  
- Advanced CLV:  
  - BG/NBD (purchase frequency)  
  - Gamma-Gamma (average spend per order)  
  - Combined into 12-month CLV forecasts.  

### 4. Scenario Planning
Tested what-if strategies:
- Retention uplift (reduce churn by 10%)  
- Loyalty effect (increase frequency by 15% for members)  
- Pricing strategy (increase AOV by 5%)  
- Acquisition mix (shift spend towards Organic)  


##  Key Insights
- Top 20% of customers contributed ~77% of portfolio revenue.**  
- Loyalty members generated 76% of CLV despite being only 24% of customers.**  
- Holiday cohorts retained better and had higher CLV than Jan–May cohorts.**  
- Retention improvement (+10%) delivered the biggest uplift in CLV, more than pricing or frequency changes.**


##  Deliverables
- Power BI Dashboard**: Segmentation, retention curves, Pareto chart, and interactive scenario sliders.  
- Slide Deck**: Problem, methodology, insights, and recommendations.  
- GitHub Repo**: Full Python notebooks, cleaned datasets, and scenario planner functions.
<img width="1242" height="701" alt="Screenshot 2025-09-02 at 19 50 47" src="https://github.com/user-attachments/assets/040f0449-52af-49e9-a9ea-509be7702ecc" />


- **GitHub Repository:**  
  - Python notebooks for cleaning, analysis, CLV modelling, and scenario planning  
  - Exported CSVs for Power BI  
  - README with business + technical explanation  

##  Tech Stack
- Python:** pandas, numpy, matplotlib, seaborn, lifetimes  
- BI Tools:** Power BI / Tableau    
- Data:** Online Retail II dataset (UCI/Kaggle), enriched with synthetic features  

 ## Recommendations
- Prioritize retention for Elite and High-value customers.
- Reinforce loyalty programs for Potential Loyalists.
- Rebalance acquisition spend towards Organic and Paid Search.
- Use CLV forecasts for smarter budgeting and targeting.
