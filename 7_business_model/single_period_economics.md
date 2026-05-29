# 💵 Single Period Economics (Annual P&L)

This document provides a detailed, pro-forma Profit & Loss (P&L) statement for **Solo Accounting** over a single 12-month period, assuming a benchmark scale of **1,000 active customers** and operating as a **California LLC**.

---

## 📋 Core Assumptions

* **Active Customer Base:** 1,000 steady-state users.
* **Subscription Split:**
  * **70% Annual Plan:** 700 customers paying $70.00 / year.
  * **30% Monthly Plan:** 300 customers paying $7.00 / month.
* **Corporate Entity:** California Single-Member LLC.
  * California imposes a flat **$800 annual franchise tax** on all LLCs.
  * An additional fee is applied *only* if gross receipts exceed $250,000. Since our gross revenue is $74,200, the additional state fee is **$0.00**.

---

## 📊 Pro-Forma Annual P&L Statement (1,000 Users)

| P&L Category | Annual Projection | % of Revenue | Notes |
| :--- | :---: | :---: | :--- |
| **Operating Revenue** | | | |
| &nbsp;&nbsp;&nbsp;&nbsp;Annual Subscriptions (700 x $70.00) | $49,000.00 | 66.0% | Paid upfront |
| &nbsp;&nbsp;&nbsp;&nbsp;Monthly Subscriptions (300 x $7.00 x 12) | $25,200.00 | 34.0% | Recurring monthly inflow |
| **Gross Operating Revenue** | **$74,200.00** | **100.0%** | **Blended ARPU of ~$74.20/yr** |
| | | | |
| **Cost of Goods Sold (COGS)** | | | |
| &nbsp;&nbsp;&nbsp;&nbsp;Payment Processing Fees (Stripe) | $3,431.00 | 4.6% | Detailed processing breakdown below |
| &nbsp;&nbsp;&nbsp;&nbsp;Bank Sync Integrations ($1.00/user/mo) | $12,000.00 | 16.2% | Automated transaction aggregation |
| &nbsp;&nbsp;&nbsp;&nbsp;AI API Token Usage ($0.50/user/mo) | $6,000.00 | 8.1% | Categorization, prompt caches, OCR |
| &nbsp;&nbsp;&nbsp;&nbsp;Infrastructure & Hosting ($0.30/user/mo) | $3,600.00 | 4.9% | Cloudflare Workers, serverless DB |
| **Total Cost of Goods Sold** | **$25,031.00** | **33.7%** | **Blended COGS of $25.03/user/year** |
| | | | |
| **Gross Profit** | **$49,169.00** | **66.3%** | **Healthy service margin** |
| | | | |
| **Operating Expenses (OPEX)** | | | |
| &nbsp;&nbsp;&nbsp;&nbsp;California LLC Franchise Tax | $800.00 | 1.1% | Flat mandatory state fee |
| &nbsp;&nbsp;&nbsp;&nbsp;Domains, SSL, and Email Hosting | $200.00 | 0.3% | Custom domains and transactional email |
| &nbsp;&nbsp;&nbsp;&nbsp;Community & Organic Marketing | $1,000.00 | 1.3% | Value-first content and forum sponsorships |
| &nbsp;&nbsp;&nbsp;&nbsp;Accounting & Tax Software Tools | $500.00 | 0.7% | Operational tools for managing the LLC |
| &nbsp;&nbsp;&nbsp;&nbsp;Legal & CPA Consulting | $1,500.00 | 2.0% | Year-end tax filing and corporate compliance |
| **Total Operating Expenses** | **$4,000.00** | **5.4%** | **Extremely lean fixed cost structure** |
| | | | |
| **Net Income (EBITDA)** | **$45,169.00** | **60.9%** | **Pre-tax net cash flow** |

---

## 🔍 Detailed Analysis & Explanatory Notes

### 1. Stripe Processing Fee Breakdown
* **Monthly Cohort Processing:** 300 monthly users generate 12 payments per year = 3,600 total transactions. At standard Stripe rates (2.9% + $0.30), the fee is $0.50 per transaction.
  $$\text{Monthly Processing Costs} = 3,600 \text{ trans.} \times \$0.50 = \$1,800.00$$
* **Annual Cohort Processing:** 700 annual users generate 1 payment per year = 700 total transactions. At standard Stripe rates, the fee on a $70.00 transaction is 2.9% * $70 + $0.30 = $2.33.
  $$\text{Annual Processing Costs} = 700 \text{ trans.} \times \$2.33 = \$1,631.00$$
* **Total Transaction Drag:** $1,800 + $1,631 = $3,431. Note that standard monthly subscription processing eats **7.1%** of revenue, whereas annual processing only consumes **3.3%**.

### 2. High Pre-Tax Profit Margins (60.9%)
Because Solo Accounting is a **privacy-first, edge-optimized, serverless cloud SaaS**, the server-side compute footprint is exceptionally small. Most heavy analytical queries are cached at the edge, and PostgreSQL Row-Level Security keeps database operations lightweight and perfectly partitioned, reducing hosting costs to negligible levels.

### 3. Solopreneur Owner Compensation
For a single developer or solopreneur, a net income of **$45,169.00** on 1,000 users represents a highly successful side project or a sustainable bootstrap model. This cash surplus can be:
* Paid out as owner draws (profits flow through to the personal tax return in a single-member LLC).
* Reinvested to scale the product (e.g., adding localized marketing or hiring part-time support).
