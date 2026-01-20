# 📖 Metric Dictionary & Data Governance

## 🎯 Strategic Alignment
To solve the problem of scattered data across Excel, WhatsApp, and CRM systems, I have defined a "Single Source of Truth." This dictionary ensures that the Sales, Finance, and Management teams are all using the same definitions for business success.

---

## 📊 Core Business Metrics (KPIs)

| KPI Name | Technical Logic / Formula | Business Value |
| :--- | :--- | :--- |
| **MRR** (Monthly Recurring Revenue) | $\sum(\text{Active Monthly Subscriptions})$ | Measures the "heartbeat" of the SaaS business and predictable cash flow. |
| **Lead Conversion Rate** | $(\frac{\text{Closed-Won Deals}}{\text{Total Leads}}) \times 100$ | Measures the efficiency of the sales pipeline and team performance. |
| **CAC** (Customer Acquisition Cost) | $\frac{\text{Total Sales \& Marketing Spend}}{\text{New Customers Acquired}}$ | Determines the ROI of marketing efforts and business sustainability. |
| **Churn Rate** | $(\frac{\text{Lost Customers}}{\text{Total Customers at Start of Month}}) \times 100$ | Identifies if the product is failing to retain SME clients. |
| **Average Deal Value** | $\frac{\text{Total Revenue}}{\text{Number of Closed-Won Deals}}$ | Helps in forecasting future revenue based on current lead volume. |

---

## 🛠️ Data Standardization & Quality Rules

To eliminate the "messy data" problem identified in the case study, the following rules must be enforced during the ETL (Extract, Transform, Load) process:

### 1. Geographic Mapping (Province)
All manual entries must be standardized to the 9 official South African provinces. 
- *Rule:* Convert "JHB", "Pretoria", or "GP" $\rightarrow$ **Gauteng**.
- *Rule:* Convert "CT", "Cape Town", or "WC" $\rightarrow$ **Western Cape**.

### 2. Lead Status Categories
To prevent confusion in the CRM, only five statuses are permitted:
1. **New:** Initial lead entry.
2. **Contacted:** Initial outreach completed.
3. **Qualified:** Interest confirmed and solution proposed.
4. **Closed-Won:** Contract signed and payment verified.
5. **Closed-Lost:** Deal did not move forward.

### 3. Financial Consistency
- **Currency:** All values must be recorded in South African Rand (ZAR).
- **Date Format:** Must follow the ISO standard `YYYY-MM-DD` for database compatibility.

---

## 💡 Note
By establishing this dictionary, we reduce "data friction." When the CFO and Sales Manager look at the dashboard, they no longer argue about the numbers; they focus on making decisions based on the data.