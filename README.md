# 🚀 Matimu Mkhacane | Data Analytics
*Bridging the gap between raw data and strategic business value.*

---

## 📂 Featured Projects

### 1. 🏦 Credit Risk & Loan Portfolio Analysis
**The Problem:** A retail bank was managing a portfolio of over 32,000 loans totaling R312.43M. Management lacked real-time visibility into default risks, specifically for high-risk loan grades (D through G), and struggled with data integrity issues like incorrect interest rate formatting.

**The Solution:**
- **Data Engineering:** Used Power Query to resolve locale-based formatting errors and standardized fields into a "Distinct Count" to accurately reflect 32,581 unique borrowers.
- **Analytics:** Developed DAX measures to calculate a 21.82% Portfolio Default Rate and isolated the Top 10 high-exposure accounts for targeted intervention.
- **Result:** A dynamic Power BI dashboard that allows executives to filter by loan intent and home ownership to monitor risk in real-time.

---

### 2. 📊 SaaS Data Strategy & Solution Design
**The Problem:**
A South African FinTech startup had critical sales data scattered across Excel, WhatsApp, and an old CRM. The lack of a "Single Source of Truth" made it impossible for the CFO to forecast revenue or for the Sales Manager to identify where leads were dropping off.

**The Solution:**
- **Strategy:** Authored a Business Requirements Document (BRD) defining key User Stories to align Sales and Finance teams.
- **Governance:** Established a **Metric Dictionary** to standardize KPIs like MRR (Monthly Recurring Revenue) and CAC (Customer Acquisition Cost), ensuring everyone uses the same math.
- **Design:** Created a high-fidelity **Dashboard Wireframe** featuring a Sales Funnel and Regional Heatmap to identify growth opportunities in provinces like Gauteng and Western Cape.
- **Result:** A comprehensive roadmap to centralize data into a SQL-based pipeline, reducing "data friction" and manual logging time.

---

## 🛠️ Technical Toolbox
- **Data Visualization:** Power BI Desktop
- **ETL & Data Modeling:** Power Query (M), Star Schema Design
- **Analytical Languages:** DAX, LaTeX (for financial formulas)
- **Documentation:** VS Code, Markdown

---
# 📊 Project 1: Credit Risk & Loan Portfolio Analysis

## 🎯 Executive Summary
This project delivers a comprehensive analysis of a retail banking loan portfolio. Using **Power BI**, I transformed a raw dataset of 32,000+ records into an interactive dashboard to monitor default rates, interest rate sensitivity, and high-exposure lending risks.

---

## 📈 Key Dashboard Features

### 1. KPI Scorecard
- **Total Principal Disbursed (R312.43M):** The total capital currently lent across the portfolio.
- **Portfolio Default Rate (21.82%):** The percentage of loans currently categorized as unpaid.
- **Weighted Avg. Interest Rate (11.01%):** The average cost of borrowing for the portfolio.

### 2. Risk Distribution Analysis
I implemented a **"Traffic Light" Risk Model** to categorize borrowers:
- **Low Risk:** High-grade loans with consistent payment history.
- **High Risk:** Loans showing signs of distress (Grades D-G).

### 3. High-Exposure Tracking
The dashboard includes a **Top 10 Exposure Table** which identifies the largest individual loans. This allows credit officers to prioritize intervention for high-value accounts at risk.

---

## 🏗️ Data Engineering Process
One of the primary challenges was **Data Cleaning**:
1. **Locale Conflicts:** Fixed interest rate decimal errors using English (US) locale settings in Power Query.
2. **Data Integrity:** Resolved "Sum of Accounts" errors by converting account fields to **Distinct Count** to accurately represent the 32,581 unique borrowers.
3. **Outlier Management:** Filtered and visualized interest rate spreads using Scatter Plots to identify predatory or high-risk outliers.

---

## 📊 Final Dashboard View

![Final Credit Risk Dashboard](Dashboard.png)
---

## 🚀 How to View the Project
1. Download the `credit_risk_dataset.pbix` file.
2. Open with **Power BI Desktop**.
3. Interact with the **Loan Intent** and **Home Ownership** slicers to see dynamic risk updates.
---   

# 📊 Project 2: SaaS Sales Pipeline Strategy & Solution Design

## 🏢 The Case Study: FinTech Startup Optimization
**Scenario:** A South African FinTech startup providing digital payment solutions to SMEs was struggling with "Data Silos." Sales data was scattered across Excel, WhatsApp logs, and an old CRM, making it impossible to forecast revenue or track lead conversion accurately.

**My Role:** As the Lead Data Analyst, I designed a centralized data reporting strategy to bridge the gap between messy manual logs and executive decision-making.

---

## 🏗️ Step 1 & 2: Data Strategy & Architecture
To solve the visibility gap, I proposed a transition from manual tracking to a structured data pipeline:

1. **Data Ingestion:** Streamlining inputs from CRM exports, structured Excel templates (replacing WhatsApp), and Bank APIs.
2. **ETL Layer:** Using Power Query to clean "Province" data (e.g., standardizing "JHB" to "Gauteng") and resolving duplicate lead entries.
3. **Central Database:** Staging cleaned data in a SQL environment to serve as the "Single Source of Truth" for both Sales and Finance.

---

## 📏 Step 3: Metric Standardization
I developed a **Metric Dictionary** (see `Metric-Dictionary.md`) to ensure all stakeholders agree on the math. Key KPIs include:
- **MRR (Monthly Recurring Revenue):** To track predictable growth.
- **Lead Conversion Rate:** To measure sales team efficiency.
- **CAC (Customer Acquisition Cost):** To monitor marketing ROI.

---

## 🖼️ Step 4: Dashboard Mockup (Wireframe)
Before technical implementation, I designed a wireframe to align with the CEO's requirements.

### Layout Strategy:
- **Top Row:** High-level KPI cards (MRR, Conversion %, Churn).
- **Center Left:** A **Sales Funnel** showing drop-offs from *Lead* to *Closed-Won*.
- **Center Right:** A **Geographic Heatmap** of South Africa to identify regional hotspots.
- **Bottom:** An **Actionable Table** listing "Idle Leads" (no contact in >48 hours).

![SaaS Dashboard Wireframe](mockup_wireframe.png)

---

## 🏁 Conclusion & Business Impact

### 💡 Strategic ROI (Return on Investment)
By implementing this centralized Data Strategy:
1. **Time Efficiency:** Sales reps save approximately 5 hours a week by moving away from manual WhatsApp/Excel logging into a structured CRM flow.
2. **Forecast Accuracy:** The CFO can now predict cash flow with 95% accuracy using the defined MRR and Churn metrics.
3. **Data Quality:** Standardizing geographic data allows for precise regional marketing spend and better resource allocation.

### 🔑 Key Learning
This project demonstrated that a successful BI solution is 20% visualization and 80% strategy. Establishing **Data Governance** and **Architecture** is what truly turns "messy data" into a business asset.   
**Author:** Matimu Mkhacane 

