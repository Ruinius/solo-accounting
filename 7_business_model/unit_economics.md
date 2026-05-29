# 📊 Unit Economics Model

To keep **Solo Accounting** viable as a free-to-low-cost utility, our primary financial objective is **breakeven sustainability** rather than hyper-profitability. This document outlines the unit economics of our two pricing structures ($7.00/month and $70.00/year) and details our Cost of Goods Sold (COGS) model.

---

## 💵 Price Point Comparison

We offer two straightforward plans designed to cover standard transaction, infrastructure, and third-party integration costs:

1. **Monthly Subscription:** $7.00 / month
2. **Annual Subscription:** $70.00 / year (equivalent to $5.83 / month)

Assuming a typical SaaS tier distribution of **70% Annual** and **30% Monthly** subscribers, our blended average metrics are modeled below.

### Blended Average Monthly Metrics (Per User)

| Metric | Monthly Plan ($7.00/mo) | Annual Plan ($70.00/yr) | Blended Average (~70% Ann / 30% Mo) |
| :--- | :---: | :---: | :---: |
| **Gross Monthly Revenue** | **$7.00** | **$5.83** | **$6.18** |
| Stripe Payment Fee (2.9% + $0.30) | $0.50 | $0.19 | $0.29 |
| **Net Revenue (After Gateway)** | **$6.50** | **$5.64** | **$5.89** |
| *COGS: Bank Sync (Teller/Plaid)* | $1.00 | $1.00 | $1.00 |
| *COGS: AI Model Tokens* | $0.50 | $0.50 | $0.50 |
| *COGS: Infrastructure & Hosting* | $0.30 | $0.30 | $0.30 |
| **Total Monthly COGS** | **$1.80** | **$1.80** | **$1.80** |
| **Contribution Margin ($)** | **$4.70** | **$3.84** | **$4.09** |
| **Contribution Margin (%)** | **67.1%** | **65.9%** | **66.2%** |

---

## 🔍 Cost of Goods Sold (COGS) Breakdown

Our variable costs are highly optimized through architectural decisions designed for privacy-respecting and serverless cloud operations:

### 1. Payment Processing (Stripe)
* **Monthly Billing:** Standard Stripe fee of 2.9% + $0.30 equals **$0.50** per transaction.
* **Annual Billing:** Standard Stripe fee on a $70.00 transaction is 2.9% + $0.30 = $2.33, which amortizes to **$0.19 / month** over 12 months.
* **Optimization:** Actively encouraging annual billing yields a **62% transaction fee savings** per user per month.

### 2. Automated Bank Sync (Plaid / Teller / GoCardless)
* **Allocation:** **$1.00 / user / month**
* **Details:** Direct bank data synchronization via APIs. In the US, aggregators typically charge per active connection, while in Europe (under PSD2), open banking options are even more cost-effective.
* **Optimization:** Users can manually import standard OFX/CSV files for free, which incurs **$0.00 COGS** for users who choose to opt-out of automated sync.

### 3. Secure AI Integrations (Tokens)
* **Allocation:** **$0.50 / user / month**
* **Details:** Transaction categorization, OCR processing for receipts, and conversational financial assistance.
* **Optimization:** 
  - **Centralized Semantic Caching:** Utilizing Redis semantic caches to intercept and resolve standard classification and lookup queries without touching expensive foundation model APIs.
  - **Prompt Caching:** Implementing Redis-based semantic prompt caching on the server side to intercept and reuse common requests.
  - **Efficient Models:** Using ultra-fast, low-cost API endpoints (e.g., Gemini 3.5 Flash or DeepSeek V3) rather than bloated flagship models.

### 4. Infrastructure & Hosting
* **Allocation:** **$0.30 / user / month**
* **Details:** Database hosting (PostgreSQL serverless with Neon/Supabase), edge compute functions (Cloudflare Workers), and Redis caching.
* **Optimization:** Centralized PostgreSQL partitions and Cloudflare workers process and cache ledger queries at the edge, keeping heavy database query costs to an absolute minimum.

---

> [!TIP]
> **Key Takeaway:** With a robust blended contribution margin of **66.2% ($4.09 per user per month)**, Solo Accounting possesses highly resilient unit economics. This allows the business to safely absorb sudden spikes in API costs or variable hosting demands while remaining exceptionally affordable for solopreneurs.
