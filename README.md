# Hoorin Money

## GitHub Pages setup
1. Upload all files in this folder to the repository root.
2. Open Settings → Pages. Choose Deploy from a branch, `main`, and `/(root)`.
3. Save and open the published URL.

## Changes in this update
- Wallets now display remaining balance (opening balance + income − expenses/transfers + incoming transfers).
- Removed Wallet from Dashboard Quick add.
- Transfers count as expenses in totals and category budgets while still moving balance from source wallet to destination wallet.
- Transfers made from a wallet whose type is Card also create an outstanding item in Loans & Dues.
- Guarded an optional currencies element to prevent a render error if it is absent.

## Important
Before replacing your existing `index.html`, export a JSON backup. Existing data stays in the same browser storage as long as the site origin and localStorage key remain unchanged. Google Drive OAuth may need its GitHub Pages origin added to Authorized JavaScript origins.
