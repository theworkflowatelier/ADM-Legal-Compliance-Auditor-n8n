# 🛡️ Automating CCPA/CPRA Legal Compliance Audits in n8n (Gemini 2.5 Flash)

An enterprise-grade headless automation architecture designed to ingest dense vendor contracts (100+ pages), evaluate complex legal syntax against Automated Decision-Making (ADM) privacy frameworks, and log verbatim deficient clauses directly into executive reporting dashboards.

[![Get Turnkey Production Bundle]([https://img.shields.io/badge/📦_Download_Full_Production_Bundle-$499-blue?style=for-the-badge])]

---

## ⚡ The Engineering Challenge & Solution
Manual legal audits of dense vendor contracts cost $300–$500/hr and standard LLM chat interfaces frequently fail due to memory timeouts, token limits, and hallucinated summaries. 

This n8n architecture solves three major production bottlenecks:
1. **Ingestion & Rate-Limit Throttling:** Routes documents through a `SplitInBatches` node with a configurable throttle to prevent Google Drive and Gemini API rate-limit crashes during bulk audits.
2. **Verbatim Clause Extraction:** Enforces strict JSON schema outputs, requiring the engine to extract the exact string (`Deficient_Clause_Quote`) and map a 1-2 sentence actionable remediation step without generic summaries.
3. **Failsafe Error Routing:** A dedicated error branch catches corrupted PDFs or API timeouts, logging failed payloads directly to an "Exceptions Queue" tab so the loop never breaks.

---

## 📊 Stress-Test Benchmark Results
We benchmarked this routing engine against **Meta’s public 100+ page Privacy Policy**. 
* **Execution Time:** ~14 seconds
* **Accuracy:** Successfully isolated non-compliant profiling clauses without hallucination
* **API Cost:** Sub-cent per execution run

📺 **[Watch the 120-Second Architecture Execution Demo Video](https://www.youtube.com/watch?v=brv3bNtOPuw)**

---

## 🚀 Free Tier vs. Production Turnkey Bundle

This repository provides the structural core routing JSON (`N8N_WORKFLOW_Sanitized.json`) for developers looking to build and test their own compliance pipelines from scratch. 

For automation agencies, legal ops teams, and DPOs requiring an instant, turnkey deployment without 35+ hours of prompt engineering and spreadsheet schema mapping, we offer the **Full Production Bundle**.

| Feature | Free GitHub Tier | Production Turnkey Bundle ($499) |
| :--- | :---: | :---: |
| **Core n8n Routing JSON** | ✅ Included (Sanitized) | ✅ Production-Ready |
| **Batch Throttling Logic** | ✅ Basic | ✅ Advanced Error-Catching |
| **Gemini 2.5 Flash System Prompt** | ❌ *Placeholder String* | ✅ **Stress-Tested Verbatim Prompt** |
| **Executive Spreadsheet Dashboard** | ❌ *Basic CSV Schema* | ✅ **Pre-Mapped Dashboard & Error Queue** |
| **Zero-Data-Retention Addendum** | ❌ | ✅ **Corporate Legal Security Addendum** |
| **Agency White-Label Guide & SOPs**| ❌ | ✅ **Step-by-Step Operator Setup Guide** |
| **Executive ROI Calculator** | ❌ | ✅ **Client Pitch & Payback Calculator** |

👉 **[Deploy the Full Production Turnkey Bundle to Your Server Today](https://theworkflowatelier.gumroad.com/l/admcap)**

---

## 🛠️ Quick Start (Free Tier Setup)
1. Download `N8N_WORKFLOW_Sanitized.json` from this repository.
2. In your self-hosted or cloud n8n workspace, click **Workflows** $\rightarrow$ **Import from File**.
3. Connect your Google Drive OAuth and Google Gemini API credentials.
4. *Note:* You will need to write and configure your own custom Gemini system prompt and map your own spreadsheet data columns before running production contracts.

---

## 📄 License & Use
The raw structural JSON in this repository is open-source under the MIT License. Turnkey production assets, legal guardrail addendums, and proprietary system prompts are licensed strictly via [Gumroad](INSERT_YOUR_GUMROAD_LINK_HERE).
