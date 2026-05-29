# 🤖 AI-Friendly Financial Engine & API

Solo Accounting is designed from the ground up for a new era where business owners utilize AI assistants to handle tedious administrative tasks. Instead of manual data entry, your accounting software works natively with AI agents to automate categorization, verify tax deductions, and reconcile accounts—all under your absolute control.

---

## 💡 What is an AI-Friendly Accounting System? (In Plain English)

Traditional accounting programs are built only for humans clicking buttons on a screen. If you want an AI helper to enter data, it has to pretend to be a human, clicking around a laggy interface.

**Solo Accounting is different.** We built a high-speed, highly structured API (an "Application Programming Interface" or digital highway) alongside our interface. 
* It is like building a house with both a front door for humans (a beautiful web app) and a special, secure service entrance for your AI assistant.
* The AI can instantly read transaction files, matching them up in milliseconds, and draft your books for you.
* **You are always in the driver's seat.** The AI only proposes actions—you click "Approve" before anything becomes official.

---

## 🔐 The Security Sandbox: Protecting Your Financial Privacy

We know your financial data is highly sensitive. Solo Accounting implements strict safety guidelines to ensure AI integration is incredibly secure:

```
┌────────────────────────────────────────────────────────┐
│                   Owner Dashboard                      │
│     [ Approve ] ◄─── AI Proposes Category & Deductions │
└──────────────────────────┬─────────────────────────────┘
                           │
                 🔐 Security Sandbox
┌──────────────────────────▼─────────────────────────────┐
│                 AI Financial Agent                     │
│  • Reads receipts  • Parses Bank CSVs  • Runs matches  │
└────────────────────────────────────────────────────────┘
```

> [!IMPORTANT]
> **Core Safety Tenets:**
> 1. **Zero Auto-Write Permissions:** The AI agent can *never* directly finalize a change in your official ledger without explicit owner confirmation. It acts as a highly capable draft clerk.
> 2. **Local & Cloud Encryption:** When the AI accesses data, it runs in a sandboxed runtime. Your underlying bank credentials are never visible to the AI engine.
> 3. **Audit Trail:** Every edit proposed by the AI is marked with a special tag: `created_by: "AI_Agent" (Draft)`. You can revert or edit any suggestion with a single click.

---

## 📊 The Universal AI Transaction Language (JSON Schema)

To make it incredibly easy for any AI agent (like ChatGPT, Claude, or local open-source models) to assist you, Solo Accounting uses a simple, readable data format (JSON) for its double-entry transactions.

Here is an example of how the AI agent reads and structures a transaction for Sarah's bakery:

```json
{
  "transaction_id": "tx_902183981",
  "date": "2026-05-29",
  "payee": "Central Flour Mills",
  "description": "Bulk organic pastry flour and yeast supply",
  "status": "draft_proposed_by_ai",
  "metadata": {
    "receipt_matched": "rec_8821.jpg",
    "confidence_score": 0.98,
    "tax_deductible": true,
    "tax_category": "Schedule_C_Supplies"
  },
  "ledger_entries": [
    {
      "account": "Expenses:Supplies:BakingSupplies",
      "type": "debit",
      "amount": 100.00
    },
    {
      "account": "Assets:Checking:BusinessChecking",
      "type": "credit",
      "amount": 100.00
    }
  ]
}
```

---

## 💬 Natural Language Conversational Commands

Because the system is AI-friendly, you can simply type or speak to Solo Accounting to run complex tasks:

* 🗣️ *"AI, check if I uploaded the receipt for the $45 hardware store charge on Tuesday."*
* 🗣️ *"Categorize all my rideshare gas charges from last month as business travel expenses."*
* 🗣️ *"Draft an invoice for Elena's new branding package client for $2,500 USD, converted to Euros."*

The AI performs the research in the background and presents a neat interactive card showing exactly what it wants to do, waiting for your green light.
