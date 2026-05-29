# 📄 Invoicing, Multi-Currency, & Billing

For freelancers and local service businesses, invoicing is the lifeblood of their cash flow. **Solo Accounting** includes a modern, beautifully designed invoicing system that helps you create professional estimates, bill clients, capture rapid payments in the field, and manage international currencies without getting bogged down by hidden fees.

---

## 💡 How Invoicing and Billing Works (In Plain English)

An invoice is simply a professional bill you send to a client detailing the services or products you provided and how much they owe you. 

Solo Accounting elevates this standard process by making it fully digital and interactive:
1. **Create in Seconds:** Fill out a simple web form detailing items, prices, and taxes.
2. **Send a Magic Link:** Send your client a secure web link (e.g. `solo.acct/yourbusiness/inv-092`).
3. **Client Portal Payment:** Your client opens the link, reviews the beautiful, mobile-friendly invoice, and clicks "Pay with Credit Card" or "Bank Transfer."
4. **Auto-Update Ledger:** The second they pay, the money is tracked, the invoice is marked as Paid, and the double-entry ledger is updated automatically. No manual recording required.

---

## 🌎 Multi-Currency Billing (The Remote Contractor Advantage)

For remote consultants (like our persona **Elena Designer**), working with clients in different countries can be a financial nightmare due to shifting exchange rates and high bank conversion fees.

```
┌────────────────────────┐
│   Invoice: $1,000 USD  │  ◄── Drafted by Elena
└──────────┬─────────────┘
           │  Real-time exchange conversion API
           ▼
┌────────────────────────┐
│    Client Pays in EUR  │  ◄── Client sees €920.00
└──────────┬─────────────┘
           │  Matches exact local bank deposit
           ▼
┌────────────────────────┐
│  Ledger Record Draft   │  Debit: Assets:Checking (in EUR & USD base)
│                        │  Gain/Loss Account (tracks FX fluctuations)
└────────────────────────┘
```

> [!TIP]
> Solo Accounting integrates a real-time exchange rate engine. If you issue an invoice in USD but the client pays in Euros, the system tracks the precise exchange value at the exact second the payment is cleared, automatically calculation any exchange gains or losses for your tax records.

---

## 📱 In-Field Payments (The Tradesperson Advantage)

For service businesses operating on-site (like our persona **Joe Plumber**), waiting days for clients to mail a check leads to cash flow bottlenecks.

Solo Accounting solves this by enabling **In-Field Mobile Payments**:
* **QR Code Payment:** Once a job is finished, display a secure QR code on your phone screen. The client scans it with their camera and pays immediately using Apple Pay, Google Pay, or a credit card.
* **Low-Cost Processing Fees:** We integrate directly with Stripe, ensuring you pay only the standard, rock-bottom credit card processing rates with zero extra markup fees.
* **Auto-Reconciliation:** Because the invoice is tied to your Stripe integration, the processing fees are split out and categorized under `Expenses:BankFees` automatically, preserving your ledger balance.
