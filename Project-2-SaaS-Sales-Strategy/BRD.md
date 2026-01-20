## 🏗️ Data Architecture Strategy

To solve the issue of scattered data, I have designed a centralized data pipeline:

### 📥 Data Ingestion
- **CRM Export:** Weekly CSV dumps of lead status.
- **Manual Logs:** Structured Excel templates to replace unstructured WhatsApp notes.
- **Financials:** Direct API integration with the bank to track real-time revenue.

### ⚙️ ETL & Transformation
- Use **Power Query** to merge disparate sources.
- Standardize all "Province" entries (e.g., changing "GP", "Gauteng", and "JHB" to a single "Gauteng" value).

### 📤 Data Destination
- All data will be staged in a **SQL Server** environment. This ensures that the Sales Manager and the CFO are looking at the exact same numbers.