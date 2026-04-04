# Bodega Tracker 💰

A personal finance tracker built as a single HTML file. No backend, no database, no login — everything stays on your device.

## Features

- **Overview** — Net savings ring, income vs expenses, monthly bar chart, spending by category
- **Bills** — Four sub-tabs: Manual (checklist), Auto-deducted, Loans/Installments, Subscriptions. All bills automatically count toward total expenses on the dashboard.
- **Add Entry** — Log income or expenses with two-level category → subcategory selection
- **Plan** — Budget tab (variable expense cap, monthly savings target, per-category limits) and Savings Goals tab (goal tracker with progress bars and deadlines)
- **AI Analysis** — Builds a prompt from your data and copies it to clipboard for pasting into Claude
- **History** — Filterable transaction log including bills
- **Settings** — Add subcategories and create new parent categories with custom emoji and color

## Category Structure

| Category | Subcategories |
|---|---|
| 💰 Income | Salary, Freelance, Consulting, Investment, Business, Other Income |
| 🍽️ Food | Dine-In, Delivery, To-Go, Drinks |
| 🏠 Household | Grocery, Laundry, Home |
| 🚗 Transportation | Commute, Grab, InDrive |
| 💅 Personal Care | Grooming, Make-up, Skincare, Bag & Clothes, Shoes |
| 🎉 Lifestyle | Entertainment, Hotel, Travel, Sports, Membership |
| ❤️ People | Gift, Parents, Family, Tithes |
| 🏥 Health | Health, Medicine |
| ⚠️ Debt | Interest Charges |

## How to Use

### On Desktop
1. Download `index.html`
2. Open it in any browser

### On iPhone (via GitHub Pages)
1. Open the GitHub Pages URL in Safari
2. Tap Share → **Add to Home Screen**
3. It will appear as an app icon on your home screen

### Data & Privacy
- All data is stored in your browser's `localStorage` — it never leaves your device
- The AI tab copies a prompt to your clipboard (totals and category names only, no notes) — you paste it into Claude yourself, nothing is sent automatically
- Clearing your browser data will erase your entries — use the CSV export regularly as a backup

### CSV Export / Import
- Tap **↓** in the header to export all transactions as a CSV
- Tap **↑** to import a CSV back (compatible with the export format)
- Import into Google Sheets for further analysis

## Setup for GitHub Pages

1. Fork or upload this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)` folder
4. Save — your app will be live at `https://yourusername.github.io/fintrack`

## Tech Stack

- Vanilla HTML, CSS, JavaScript — zero dependencies
- Google Fonts (Plus Jakarta Sans + Playfair Display) — loaded via `@import`
- Data persistence via `localStorage`
- No build step, no framework, no server required

## Currency

Amounts are displayed in **Philippine Peso (₱)**. To change the currency symbol, search for `₱` in `index.html` and replace with your preferred symbol.
