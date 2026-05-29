# 👥 Multi-User Collaboration & Permissions

As a business grows, bookkeeping is no longer a solo journey. **Solo Accounting** includes a clean, simple, yet secure multi-user collaboration engine that allows you to invite team members, manage payroll tax coordination, and hand off access to your CPA without paying massive, bloated commercial seat licenses.

---

## 💡 How Collaboration Works (In Plain English)

You shouldn't have to share your primary password just to let a trusted helper run invoices or let your accountant download reports. 

Solo Accounting solves this by letting you issue secure invitations:
1. **Invite via Email:** Send an email invite to a contractor, apprentice, or CPA.
2. **Assign a Role:** Choose a pre-configured role that matches their duties.
3. **Control Access:** The system restricts what they can see and do, protecting your sensitive account balances.

---

## 🔑 Pre-Configured Collaboration Roles

We keep permissions simple and functional:

```
┌────────────────────────────────────────────────────────┐
│                       Owner                            │
│           (Full Control & Bank Sync Setup)             │
└───────────┬────────────────────────────┬───────────────┘
            │                            │
            ▼                            ▼
┌────────────────────────┐  ┌────────────────────────┐
│      Accountant        │  │     Billing Clerk      │
│  • Reads all ledgers   │  │  • Writes invoices     │
│  • Performs adjustments│  │  • Cannot see bank accounts
│  • Generates tax exports│ │  • Cannot see P&L totals│
└────────────────────────┘  └────────────────────────┘
```

| Role Name | Access Level | Best For |
| :--- | :--- | :--- |
| **Owner** | 🔑 Full read, write, sync, and payment setup. | You (the business owner). |
| **Accountant** | 📊 Full read-only ledger access, plus ability to write adjusting journal entries. | Your CPA or external bookkeeper. |
| **Billing Clerk** | ✍️ Can draft invoices and log customer payments; completely blocked from viewing bank accounts, P&L reports, or payroll. | Apprentices, field crew, or administrative helpers (like **Joe Plumber**'s crew). |

---

## 💸 Basic Payroll Tax Coordination

For micro-businesses expanding beyond solopreneurship (like our personas **Joe Plumber** with 3 employees and **Marcus Contractor** with 8 crew members), commercial payroll platforms charge massive monthly premiums.

Solo Accounting keeps it lean:
* **Timecard Integration:** Field employees can record hourly logs. The Billing Clerk reviews and logs approved hours.
* **Payroll Tax Calculator Helper:** Under the hood, Solo integrates standard tables to calculate federal and state employment tax withholdings, creating draft payroll transactions that map perfectly to double-entry ledger accounts (`Expenses:Payroll:Wages` and `Liabilities:PayrollTaxes`).
* **CPA Check-off:** When payroll is processed, your accountant can instantly verify the draft transactions via their secure role access before you execute the bank payments, preventing costly compliance errors.
