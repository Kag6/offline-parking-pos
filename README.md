# Offline Parking POS (Single-File HTML)

A fully offline parking lot POS & ticketing system built as a **single HTML file**.

## What it does
- Vehicle entry → creates **ticket** (slip) and prints it
- Vehicle exit → finds ticket by **ticket number or plate**
- Fee calculation based on:
  - vehicle type pricing rules
  - duration (minutes → hours)
  - grace period
  - rounding policy
  - optional daily max
- Payment processing → marks ticket as **PAID**
- Daily reports:
  - revenue
  - paid count
  - open tickets
- Backup & restore:
  - **JSON export/import**

## Offline storage
Data is stored in the browser using **IndexedDB**.
- Works without internet
- Persists across browser restarts
- **Important:** clearing browser site data will delete records.
  - Use **JSON export** as daily/weekly backup.

## Getting started
1. Download or clone the repo
2. Open `index.html` in Chrome/Edge
3. Login with a **Company ID** and **Operator name**
4. Configure pricing in **Settings**
5. Start issuing tickets

## Printing
The app includes print-friendly layouts for:
- Entry ticket
- Payment receipt

Use your printer or “Microsoft Print to PDF”.

## Tech
- HTML
- CSS
- Vanilla JavaScript
- IndexedDB

## License
MIT
