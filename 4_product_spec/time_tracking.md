# ⏱️ Time Tracking & Hourly Billing

For remote consultants, creative freelancers, and service contractors, time is the inventory they sell. **Solo Accounting** features a highly optimized, intuitive time-tracking system that lets you log hours, manage multiple projects, split billable and non-billable tasks, and seamlessly convert timesheets into professional invoices with a single click.

---

## 💡 How Time Tracking Works (In Plain English)

When you bill by the hour, you need to show your client exactly what you did and how long it took.
* Doing this manually on paper or in a spreadsheet makes it easy to forget half of your work, leaving money on the table.
* Using complex enterprise software is overkill and adds unnecessary subscription costs.

Solo Accounting makes time tracking effortless:
1. **Click to Start:** Tap a simple stopwatch button in the app when you start a task.
2. **Assign to Client:** Select which client or project you are working on.
3. **Log Notes:** Quickly jot down what you worked on (e.g. "Drafted homepage layout").
4. **Auto-Bill:** When it's time to invoice, Solo automatically pulls all your unbilled hours for that client and builds a gorgeous, itemized bill.

---

## ⏱️ Interactive Stopwatch & Offline-Resilient Timers

For busy contractors and remote consultants (like our persona **Elena Designer**), work happens anywhere. 

```
┌────────────────────────────────────────────────────────┐
28: │              ⏱️ ACTIVE TIMER: Elena Designer          │
29: ├────────────────────────────────────────────────────────┤
30: │ • Client: Elena's Design Co -> Brand Strategy          │
31: │ • Elapsed: 02:45:12                                    │
32: │ • Current Session Rate: $100 / hr                      │
33: │ • Accrued: $275.33                                     │
34: │                                                        │
35: │ [ ■ Stop & Log ]     [ ⏸ Pause ]     [ ❌ Cancel ]     │
36: └────────────────────────────────────────────────────────┘
```

* **PWA Ambient Timer:** Because Solo Accounting is a Progressive Web App (PWA), the timer runs in a lightweight service worker. Even if you close your browser tab, lose internet access, or restart your device, the timer keeps running locally.
* **Smart Local Storage:** Sessions are automatically saved to your browser's secure local database. If you drop offline during a session, the log is securely queued and synced as soon as a connection is restored.
* **Manual Time Logs:** Forgot to start the timer? Easily add a manual time entry with start/end times or total duration.

---

## 📊 Billable vs. Non-Billable Rules & Projects

To build a profitable micro-business, you must understand your true utilization rate (how much of your work time actually generates revenue vs. admin overhead).

> [!TIP]
> Solo Accounting distinguishes between **Billable Hours** (directly charged to a client) and **Non-Billable Hours** (like administrative work, marketing, or research).
> Non-billable hours are tracked so you can analyze your business efficiency, but they are excluded from client invoices automatically.

* **Project-Based Rate Cards:** Define default hourly rates by client, project, or task category (e.g., $100/hr for design, $50/hr for research).
* **Multi-User Logging:** If you operate a small team (like **Marcus Contractor** with a few helpers), employees can log hours under their restricted "Helper" profiles, which the owner can review and approve before invoicing.

---

## 🔗 Ledger & Invoice Integration

Solo Accounting bridges the gap between raw hours and double-entry accounting:

* **Instant Invoice Generation:** When you open a client's detail page, Solo highlights "Unbilled Hours." Clicking **"Generate Invoice"** aggregates all entries, applies local sales tax or VAT, and automatically converts them to accounts receivable (`Assets:AccountsReceivable`).
* **Time-to-Revenue Matching:** The second the invoice is paid by the client, the double-entry engine debits your cash account (`Assets:Checking`) and credits service revenue (`Revenue:Services`).
