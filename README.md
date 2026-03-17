# PO System

Full Purchase Order system — single HTML file, no build step.

## Deploy to Vercel

### Option 1 — Vercel CLI
```bash
npm i -g vercel
vercel
```

### Option 2 — Drag & Drop
1. Zip this folder
2. Go to https://vercel.com/new
3. Drag the zip file → Deploy

### Option 3 — GitHub
1. Push to GitHub
2. Import at vercel.com/new → Framework: Other → Deploy

## Features
- Dashboard with stats, quick menu, recent POs, currency & supplier summary
- New Order: Telegram-style supplier chat with manual item entry
- Suppliers: Add/Edit/Delete with profile photo, currency, status
- Currencies: Full CRUD with symbol & decimal config
- Exchange Rates: CRUD + live currency converter widget
- All data persisted in localStorage
