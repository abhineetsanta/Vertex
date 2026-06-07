# 🏪 VERTEX — Local Inventory Management System

> **Your entire shop. One screen. No internet. No fees. Forever.**

A free, offline desktop application for small shop owners, retailers, and small businesses to manage inventory, billing, and sales — all from a single window on your computer.

---

## Why VERTEX?

Most inventory software either costs money every month, requires an internet connection, or is too complicated for a small shop. VERTEX is different — you run it once, it works forever, and your data never leaves your computer.

No cloud. No subscription. No nonsense.

---

## What Can You Do With It?

### 📦 Inventory Management
- Add products with name, category, cost price, and selling price
- Increase or decrease stock with one click
- Automatic **low stock alerts** when any item falls below 5 units
- Search and filter products by name or category instantly

### 🛒 Selling & Billing
- Select a product from the list, enter quantity, add to cart
- Supports customer name and phone number on each bill
- Live Grand Total updates as you add items
- Increase, decrease, or remove cart items before checkout
- On checkout, a **receipt file is automatically saved** to your folder

### 📊 Shop Analytics
At a glance, see:
- Total money invested in inventory (cost value)
- Total potential revenue if everything sells (retail value)
- Expected net profit
- Total items in stock
- How many products are running low

### 🧾 Invoices & History
- Every sale gets a unique invoice number (`INV-YYYYMMDDHHMMSS`)
- Full transaction history saved permanently
- View today's total sales and revenue in one click
- All activity is logged automatically

---

## Installation

**Requirements:** Python 3.8 or above (Tkinter comes included — no extra installs needed)

```bash
# Step 1 — Clone the repo
git clone https://github.com/ACEVINCIBLE/vertex-inventory.git
cd vertex-inventory

# Step 2 — Run it
python main.py
```

That's it. The databases are created automatically on first run. Nothing else to configure.

---

## Project Structure

```
vertex-inventory/
│
├── main.py                  ← Entry point — runs everything
├── database.py              ← Manages all three SQLite databases
├── inventory_dashboard.py   ← Inventory tab UI
├── selling_dashboard.py     ← Billing & selling tab UI
├── analysis_dashboard.py    ← Analytics tab UI
├── billing_popup.py         ← Invoice preview (in progress)
│
├── inventory.db             ← Product data (auto-created)
├── sales.db                 ← Sales history (auto-created)
├── system_logs.db           ← Activity log (auto-created)
│
└── receipt_INV-*.txt        ← Text receipts saved after each sale
```

---

## Tech Stack

| | |
|---|---|
| Language | Python 3 |
| GUI | Tkinter (ttk) |
| Database | SQLite — 3 separate local files |
| Dependencies | **None** — pure Python standard library |
| Internet Required | **No** |
| Platforms | Windows, macOS, Linux |

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Enter` in quantity field | Add item to cart |
| `Double-click` on product | Add item to cart |
| `Delete` in cart | Remove selected item |

---

## Roadmap

- [ ] Proper PDF invoice printing via BillingPopup
- [ ] Search bills by invoice number
- [ ] Date-range sales reports
- [ ] PDF receipt export
- [ ] Barcode scanner support
- [ ] Multi-user / staff login

---

## Good to Know

- All data is stored **locally on your machine** — no one else can see it
- The `.db` files are your database — back them up regularly
- Receipts are saved as `.txt` files in the same folder as `main.py`
- On Windows, receipts open automatically; on Linux/macOS, open them manually from the folder

---

## Developed By

**ACEVINCIBLE**

Built for small shops that just need something that works.

---

## License

MIT License — free to use, modify, and share. A credit is always appreciated.
