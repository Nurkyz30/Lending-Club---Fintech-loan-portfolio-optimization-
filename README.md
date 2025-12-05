# Lending club analysis
Comprehensive analysis of Lending Club's loan portfolio (2007-2018) to optimize profitability and risk management. This project demonstrates end-to-end data analytics capabilities from SQL data modeling to executive dashboard creation.

Identified $700M+ opportunity through portfolio rebalancing and strategic recommendations validated by rigorous statistical analysis.

### Data Architecture

**Normalized SQLite Database:**
- `dim_loan_products`: Loan characteristics (grade, term, amount, interest rate)
- `dim_borrowers`: Borrower profiles (FICO, DTI, employment)
- `fact_loan_performance`: Loan outcomes and performance metrics

**Dataset:**
- **Records:** 1,347,721 loans
- **Time Period:** 2007-2018
- **Source:** Lending Club fintech company (historical real world data) 
- **Size:** 1.35M records across 3 normalized tables
Recourses 
- **Data Source:** Lending Club (real world fintech 2007-2018 historical loan data)

### Primary Findings

| Finding | Current State | Opportunity | Value Impact |
|---------|--------------|-------------|--------------|
| **Term Mix Optimization** | 24% in 60-month loans | Increase to 40-45% | **$600M+** |
| **Grade B-C Expansion** | 34% of volume | Expand 60-month by 50% | **$465M** |
| **Grade A Repricing** | 14.2% ROI (below avg) | Shift to 60-month | **$240M** |
| **Grade G-36m Exit** | Negative ROI (-4.6%) | Discontinue product | **$7M + risk reduction** |
| **TOTAL VALUE CREATION** | - | 18-24 month horizon | **$1.3B+** |
### Portfolio Metrics

- **Total Loans Analyzed:** 1,347,721
- **Total Profit Generated:** $3,171.5M
- **Average ROI:** 16.3%
- **Average Default Rate:** 29.7%
  <img width="856" height="476" alt="image" src="https://github.com/user-attachments/assets/19aa0d00-0798-401b-b671-ef23411d2b56" />
## 🔍 Key Insights

### 1️⃣ Term Structure Premium (183% Profitability Gap)

**60-month loans dramatically outperform 36-month equivalents:**

- 60-month average profit: **$4,626** (22.0% ROI)
- 36-month average profit: **$1,632** (7.9% ROI)
- **Extended term compensates for higher default risk** through accumulated interest

**Strategic Implication:** Portfolio significantly underweighted in high-performing segment (24% vs optimal 40-45%)
### 2️⃣ Grade B-C Sweet Spot

**Moderate-risk segments deliver optimal risk-return balance:**

| Segment | Avg Profit | ROI | Volume | Strategic Rating |
|---------|-----------|-----|--------|-----------------|
| **B-60m** | $5,258 | 25.8% | 47,808 | ⭐⭐⭐ Star |
| **C-60m** | $4,925 | 24.9% | 105,553 | ⭐⭐⭐ Star |
| A-60m | $4,665 | 24.2% | 6,289 | ⭐⭐ Growth |
| A-36m | $1,950 | 14.2% | 228,864 | ⚠️ Review |

**Recommendation:** Aggressively scale Grade B-C 60-month products - best combination of volume, profitability, and risk management.

---

### 3️⃣ Risk Model Validation

**Composite risk score (4-13) demonstrates strong predictive power:**

- **Score 4 (Lowest Risk):** 4.8% default, 308K loans
- **Score 8 (Moderate Risk):** 20.2% default, 308K loans (largest segment)
- **Score 13 (Highest Risk):** 60.5% default, 1K loans
- **12.5x separation** between lowest and highest risk

**Portfolio Strategy:** 72% concentrated in moderate risk (scores 7-10), optimized for volume with acceptable loss rates (20-35%).

---

### 4️⃣ Economic Cycle Resilience

**2007-2008 Financial Crisis impact analysis:**

- **2007 vintages:** 26% average default rate (peak)
- **2009-2010 recovery:** Declined to 13-15%
- **Post-2015 stabilization:** 18-22% normalized rate
- **All grades affected proportionally**, maintaining risk differentiation throughout cycle
- **2-year recovery period** demonstrates portfolio resilience

**Risk Management Validation:** Model maintained predictive power across economic cycles.

Tools & Technologies

| Category | Tools | Purpose |
|----------|-------|---------|
| **Database** | SQLite | Data storage & normalization |
| **Analysis** | SQL (Window functions, CTEs, aggregations) | Complex analytical queries |
| **Data Processing** | Python (pandas) | Data export & transformation |
| **Visualization** | Power BI Desktop | Interactive dashboards |
