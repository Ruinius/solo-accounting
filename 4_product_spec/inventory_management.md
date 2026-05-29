# 📦 Inventory & Cost of Goods Sold (COGS)

For makers, bakers, and retailers, physical product stock represents significant cash tied up in the business. **Solo Accounting** features a simplified, highly visual inventory tracking system designed specifically for solopreneurs to manage stock levels, calculate the true Cost of Goods Sold (COGS), and protect profit margins without requiring enterprise database setups.

---

## 💡 How Inventory & COGS Work (In Plain English)

Inventory refers to the physical items, raw ingredients, or products you have on hand ready to sell.
* When you buy materials or inventory, it is **not** an immediate expense. It is a business asset because it still holds cash value.
* It only becomes an expense—specifically, **Cost of Goods Sold (COGS)**—when you actually sell that product to a customer.
* Tracking this correctly is critical for taxes and understanding your actual profitability, but most software makes it incredibly difficult.

Solo Accounting makes this painless:
1. **Define Your Products:** Input your products, their starting stock, and how much they cost you to make or buy.
2. **Auto-Deduct Stock:** When you send an invoice for a product, Solo automatically decreases your stock level.
3. **Smart COGS Calculations:** The app automatically shifts the exact value of the sold inventory from your asset books to your expense books, so your tax returns are calculated flawlessly.

---

## 📊 Simplified Product Catalog & Stock Tracking

For makers (like our home bakery owner **Sarah Baker**), keeping tabs on ingredient stock and finished products prevents missing orders.

```
┌────────────────────────────────────────────────────────┐
│            📦 Product Inventory & Margins             │
├────────────────────────────────────────────────────────┤
│ • Product: Custom Sourdough Boule (Loaf)               │
│ • Stock Level: 45 units  [ Low Stock Alert < 10 ]      │
│ • Unit Cost: $2.50 USD   (Flour, yeast, energy)        │
│ • Retail Price: $8.00 USD                              │
│ • Margin: 68.75% ($5.50 profit per loaf)               │
│                                                        │
│ [ + Add Stock ]     [ 📝 Adjust Stock Count ]          │
└────────────────────────────────────────────────────────┘
```

* **Live Inventory Ledger:** Track stock counts in real time. Stock increases when you log material purchases, and decreases when invoices are finalized.
* **Low-Stock Alerts:** Set custom thresholds for each product. When stock drops below a safe level, the dashboard triggers a subtle warning to remind you to restock raw materials.
* **Non-Physical Products:** Easily designate items as "Services" (which bypass inventory counts) or "Physical Goods" (which track inventory).

---

## ⚖️ Automated double-entry COGS Calculations

To keep CPAs happy and tax audits non-existent, Solo Accounting handles the complex accounting behind the scenes:

> [!IMPORTANT]
> Solo Accounting uses the **Average Cost Method** for inventory valuation by default (ideal for solopreneurs due to its extreme simplicity). 
> When you buy 10 bags of flour at $2.00, and later 10 bags at $3.00, Solo calculates your average ingredient cost as $2.50, keeping valuation simple and tax-compliant.

* **The Asset-to-Expense Pipeline:**
  1. **Purchase:** You buy $500 worth of packaging boxes.
     * *Ledger:* Debit `Assets:Inventory` $500, Credit `Assets:Checking` $500.
  2. **Sale:** You invoice a client for a gift basket that uses $50 worth of inventory.
     * *Ledger:* Debit `Expenses:COGS` $50, Credit `Assets:Inventory` $50.
* **Shrinkage & Damage Adjustments:** Real life happens. If ingredients spoil or products are damaged, log a simple "Inventory Adjustment" to write off the lost value to `Expenses:InventoryShrinkage` instantly.
