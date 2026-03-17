# Purchase Order App

Mobile-first Purchase Order app with Telegram-style supplier chat UI.

## Features
- Supplier list with profile images, online status, currency badge
- Per-supplier currency (USD, VND, CNY, EUR, etc.)
- Manual line item creation (Code, Name, Price, Qty, Image)
- Responsive: phone (full-screen) + tablet (sidebar + panel)
- Light theme

## Deploy to Vercel

### Option 1 — Vercel CLI (fastest)
```bash
npm i -g vercel
vercel
```
Follow the prompts. Your app will be live in ~30 seconds.

### Option 2 — Vercel Dashboard (no CLI)
1. Go to https://vercel.com/new
2. Click **"Import Git Repository"** — or drag & drop this folder
3. If drag & drop: zip this folder, then upload at https://vercel.com/new
4. Framework preset: **Other** (static)
5. Click **Deploy**

### Option 3 — GitHub + Vercel (auto-deploy on push)
1. Push this folder to a GitHub repo
2. Go to https://vercel.com/new → Import your repo
3. Framework: **Other**
4. Every `git push` will auto-deploy

## Local Development
Just open `index.html` in any browser — no build step needed.

## Customize Suppliers
Edit the `SUPPLIERS` array in `index.html`:
```js
{
  id: 1,
  name: "Your Supplier",
  code: "SUP-001",
  currency: "USD",        // USD, VND, CNY, EUR, GBP, JPY, ...
  photo: "https://...",   // URL to logo/photo (optional)
  status: "online",       // online | away | offline
  meta: "Category",
  ...
}
```
