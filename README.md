# Medicare Bill Generator (Bill Of Supply)

Single-page browser app for creating and printing Indian pharmacy-style medical bills.

## Files

- `index.html` - Complete app (HTML, CSS, JS in one file)

## How to Use

1. Open `index.html` in any browser.
2. Fill patient details and medicine rows directly on the bill.
3. Use toolbar buttons:
   - `New Bill` - starts a fresh bill and increments Memo No.
   - `Add Row` - adds a new medicine row
   - `Clear Fields` - clears bill content without changing Memo No.
   - `Print / Download` - opens print dialog for printing or saving PDF
4. Data auto-saves to browser `localStorage` while typing.

## Features Included

- Live editable bill layout matching a traditional Indian pharmacy print format
- Auto calculations:
  - `Amount = Qty x M.R.P.`
  - `GROSS = Sum of Amount`
  - `NET = GROSS - LESS`
- Starts with 14 rows and supports adding/removing rows
- Print CSS for clean A4 output (hides toolbar and action controls)
- Draft autosave + restore from `localStorage`
- Memo number auto-increment across new bills (`localStorage` backed)

## Host on GitHub Pages

1. Push this folder to your GitHub repository (branch `main`).
2. Open repository `Settings`.
3. Go to `Pages`.
4. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main** and folder: **/ (root)**
5. Save.
6. Wait for deployment, then open the published URL shown in Pages settings.

No backend is required. The app runs fully in the browser.
