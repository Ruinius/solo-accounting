# 🏦 Automated Bank Connection & Feeds

For modern small businesses, manual transaction entry is a relic of the past. **Solo Accounting** integrates a secure, automated bank connection engine that streams real-time transaction feeds directly into your bookkeeping ledger, keeping your books constantly up to date with zero effort.

---

## 💡 What is Bank Synchronization? (In Plain English)

Think of bank synchronization as a secure digital pipe between your bank account and your accounting software. 
* Instead of logging into your bank website, downloading messy spreadsheet files (CSVs), and uploading them, Solo Accounting connects securely behind the scenes.
* Every time you swipe your business debit card or receive a client payment, that transaction appears inside your accounting dashboard automatically.
* You do not have to write down details; they are imported instantly and ready to be sorted.

> [!IMPORTANT]
> **Privacy & Security First:** Solo Accounting *never* stores your bank username or password. We partner with secure, government-regulated financial aggregators (like Plaid or SimpleFIN) that have "read-only" access. We can see transactions, but we can never move or touch your money.

---

## 💰 The Lowest Pricing Tier: Covering the Integration Cost

We want Solo Accounting to be free or low-cost. However, high-quality bank sync networks charge software developers for every active bank connection. To ensure the software is highly sustainable, we structure our pricing as follows:

| Plan Tier | Monthly Cost | Bank Sync | Best For |
| :--- | :--- | :--- | :--- |
| **Local Offline** | **$0.00 / Free** | ❌ Manual Upload Only (CSV / QIF) | DIY Solopreneurs & Hobbyists |
| **Starter Cloud** | **$3.00 - $5.00** *(At Cost)* |  Secure Automated Feeds | Freelancers needing fast automated feeds |
| **Small Business** | **$9.00 - $12.00** |  Secure Automated Feeds + Team Access | Expanding firms needing payroll integration |

By charging a tiny, at-cost subscription for our lowest paid tier, we can offer robust bank synchronization without selling your data or cluttering your screen with ads.

---

## ⚙️ How Bank Feeds Flow into Your Ledger

Here is how transaction imports are processed, categorized, and balanced automatically:

```
┌────────────────────────┐
│   Chase/Amex/Plaid     │  ◄── Secure Read-Only API
└──────────┬─────────────┘
           │
           ▼
┌────────────────────────┐
│    Transaction Feed    │  (e.g., "$12.50 at Blue Bottle Coffee")
└──────────┬─────────────┘
           │
           ▼
┌────────────────────────┐
│  Smart Matching Rules  │  ◄── Matches past coffee shops to "Meals & Entertainment"
└──────────┬─────────────┘
           │
           ▼
┌────────────────────────┐
│   Double-Entry Entry   │  DR: Expenses:Meals
│        (Draft)         │  CR: Assets:BusinessChecking
└────────────────────────┘
```

---

## 🧠 Smart Matching & Auto-Categorization

When a bank transaction arrives, Solo Accounting doesn't just sit there. It looks at your past habits and uses simple, smart rules to propose a category:

1. **Exact Rule Matches:** If a payee contains `Chevron` or `Shell`, the system automatically maps it to your `Expenses:Travel:Fuel` account.
2. **AI Assistance:** If the vendor is new (e.g. `Joe's Bakery Supply`), our local-first AI assistant parses the name and matches it to `Expenses:Supplies:BakingSupplies`, displaying a small indicator: `95% Match Confidence`.
3. **One-Click Reconciliation:** Your dashboard shows a simple list of new transactions. You just scan the list, tap the Spacebar or click **"Reconcile All"**, and they are instantly added to your balanced ledger.
