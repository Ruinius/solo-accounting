# 🛠️ Product Specification Summary - Solo Accounting

This specification outlines the functional and non-functional requirements for the **Solo Accounting MVP**, detailing the features required for a successful launch and the long-term product roadmap.

---

## 💎 Core MVP Features

```text
┌─────────────────────────────────────────────────────────────────┐
│                     SOLO ACCOUNTING MVP CORE                    │
├─────────────────┬─────────────────┬──────────────┬──────────────┤
│  Double-Entry   │    Custom PDF   │   Smart CSV  │  Schedule C  │
│  Engine (Quiet) │ Invoice Builder │  Importer    │  Tax Reports │
└─────────────────┴─────────────────┴──────────────┴──────────────┘
```

### 1. Quiet Double-Entry Bookkeeping Engine
* **The Concept:** A robust double-entry general ledger runs silently in the background. The user interacts with clean, intuitive screens (e.g., "Add Expense", "Receive Payment") while the software automatically registers the debits and credits.
* **Chart of Accounts:** Pre-configured default categories tailored for freelancers (Assets, Liabilities, Equity, Revenue, Expenses).
* **Manual Journal Entries:** An optional "Expert Mode" for manual adjustments, depreciation entry, or tax corrections.

### 2. Custom Invoicing Suite
* **Template Engine:** Modern, highly aesthetic invoice templates with dynamic CSS layouts, custom typography, and logo uploads.
* **Drafting & PDF Export:** Auto-saves drafts, handles tax calculations (VAT/Sales Tax), and exports clean vector PDFs locally.
* **Client Directory:** Simple contact records with default terms, address, and outstanding balance summaries.

### 3. Smart CSV Transaction Importer
* **Interface:** Drag-and-drop file upload for standard bank CSV exports.
* **Column Mapping:** Intelligent mapper that remembers header associations for major banks.
* **Auto-Categorization Rules:** A learning engine that suggests account categories based on descriptions (e.g., "Slack" -> "Software Expense").

### 4. Interactive Reporting Dashboard
* **Profit & Loss (P&L):** Dynamic date-range selectors, collapsible expense categories, and beautiful HSL-colored trend line charts.
* **Balance Sheet:** Live snapshot of Assets, Liabilities, and Equity.
* **Tax Helper (Schedule C):** Specifically highlights categories matching IRS Schedule C lines (or local equivalent) for rapid tax filing.

---

## ⚙️ Non-Functional Requirements

1. **Local-First Architecture:** All data is saved on the user's hard drive in a standard, open **SQLite** file. The app requires zero internet access to function fully.
2. **Speed & Snappiness:** Transitions must be instant, with no loading spinners for local actions.
3. **Visual WOW Factor:** Sleek dark-mode by default, interactive graphs, hover feedback, and fluid transitions between dashboards.
4. **Data Portability:** Single-click full backup to a standard `.db` or `.json` file, and single-click full export of all transactions to Excel/CSV.

---

## 🗺️ Product Roadmap

### Phase 1: The Local Core (MVP)
* Desktop application (Windows, macOS, Linux via Tauri/Electron).
* Local SQLite storage.
* CSV bank statement importing, manual ledger tagging, and client management.
* Beautiful PDF invoice generation.

### Phase 2: Secure Sync & Collaboration
* End-to-End Encrypted (E2EE) database synchronization between multiple devices (e.g., Laptop and Mobile).
* Paid cloud sync utility ($3 - $5/month) using decentralized servers.
* Lightweight mobile companion app for receipt capturing and invoice viewing.

### Phase 3: The Integrations & Extensions Hub
* Developer SDK to build plugins (e.g., automated sales tax calculations, Shopify imports).
* Direct bank API sync (Plaid/Yodlee) for cloud tier.
* Integrated digital credit card/ACH invoice payment processing.
