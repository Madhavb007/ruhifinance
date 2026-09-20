# Finance Tracker V6

A free, browser-only personal finance tracker.

## Included

- Dashboard with net worth, income, spending, net cash flow and savings rate
- Separate Bank, M-PESA and Savings dashboards
- Multiple accounts of different types:
  - Bank
  - Savings
  - M-PESA
  - Cash
  - Credit card
  - Loan/debt
  - Other
- GBP, KES, USD and EUR
- Manual exchange rates
- Income, outgoing and own-account transfers
- Transfer-aware balances and KPIs
- Upcoming income, expenses and transfers
- Recurring transactions
- Spending categories including Gym
- Monthly budgets
- Spending analytics
- Net worth page
- Transaction search and account/type filters
- JSON backup and restore
- Basic CSV import
- Local browser storage
- Responsive/mobile layout
- Validation around invalid transfers and transactions

## Transfer rule

Transfers are represented by one record with:
From account -> To account -> Amount.

They change account balances but do not count as income or spending.

For safety, cross-currency transfers are blocked in this version. Currency conversion is a separate feature so the app does not silently apply a rate.

## M-PESA

M-PESA is modelled as its own wallet/account. There is no live Safaricom API connection in this free browser-only version.

Automatic M-PESA/bank connectivity should be added only with a secure backend. Never put API credentials in public JavaScript/GitHub Pages.

## Storage and privacy

Data is stored in browser localStorage. GitHub Pages hosts the app files but does not receive the user's transaction data.

Use Export Backup regularly. If browser storage is cleared, local data can be lost unless you have a backup.

## Run

Open `index.html`.

## GitHub Pages

Upload `index.html`, `style.css` and `app.js` to a GitHub repository and enable GitHub Pages.

This version deliberately has no paid service or database dependency.
