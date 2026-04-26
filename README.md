# Financial Risk and Performance Analysis 

This repository contains the complete, end-to-end documentation for a 3-week Financial Risk and Performance Analysis project. By combining data visualization with GenAI automation, this project provides a comprehensive solution for identifying, monitoring, and acting upon high-risk loans within a financial portfolio.

---

## Repository Contents
- **`Comprehensive_Project_Report.pdf`** *(or .docx / .md)*: The primary master document containing the full 3-week progression of this project, including problem statements, methodology, Excel Insights, Power BI insights, and n8n workflow documentation.
- **`/Project_Assets`**: Document file containing supporting files such as the `.pbix` dashboard, exported JSON workflows, and execution screenshots.

---

## Project Progression (The 3-Week Lifecycle)

This project was developed in three distinct phases to simulate a real-world enterprise data lifecycle:

### **Week 1: Data Foundation & Exploratory Analysis**
- **Objective:** Understand the raw loan data, clean inconsistencies, and identify initial risk indicators.
- **Key Actions:** Data profiling, handling missing values, and structuring the data model to focus on Debt-to-Income (DTI) ratios, employment lengths, and loan grades.

### **Week 2: Power BI Dashboard & Risk Modeling**
- **Objective:** Transform the cleaned data into an interactive macro-level monitoring tool.
- **Key Actions:** Built a Star Schema data model, utilized DAX for advanced KPI calculations, and designed an executive-facing dashboard to visualize default trends and geographic risk exposure.

### **Week 3: n8n + GenAI Automation**
- **Objective:** Bridge the gap between static analytics and active business operations.
- **Key Actions:** - Designed **Workflow 1 (Executive Alerting):** Scheduled data extraction triggering an AI model (LLaMA 3.3 70B) to summarize portfolio risk and email the Chief Risk Officer.
  - Designed **Workflow 2 (Borrower Transparency):** A webhook-triggered AI explainer that translates complex "Bad Loan" classifications into human-readable, empathetic emails for customers.

---

## Core Business Insights
1. **DTI and Income Thresholds:** Borrowers with a DTI above 40% in the lower income brackets are the primary drivers of portfolio defaults. 
2. **Grade Discrepancies:** Grade E, F, and G loans account for a disproportionate amount of charge-offs, requiring tighter automated underwriting rules.
3. **Operational Efficiency:** Integrating n8n with LLaMA 3.3 successfully reduced the time required for risk reporting and customer-facing explanations from hours to seconds via automated REST API pipelines.

---

## Tech Stack Demonstrated
- **Business Intelligence:** Excel, Power BI, Power Query, DAX
- **Process Automation:** n8n (Webhooks, Schedule Triggers, HTTP Requests)
- **Generative AI:** LLaMA 3.3 70B (via Groq/OpenAI Node)
- **API Integration:** Google Cloud (Gmail OAuth2 API), REST APIs (`httpbin.org` testing)

---
**Developed by:** Allan Alex
**Program:** Master's in Data Science
**Final Submission Target:** April 2026
