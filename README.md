# ClearSpend

A mobile/web friendly purchase request and budget tracking app for businesses with multiple locations. Manage approvals, track spending, and see available budgets in one place.

## Preview locally

1. Download or clone this repository.
2. Open a terminal in its folder and run:

```sh
python3 -m http.server 4173 --directory dist
```

3. Open http://localhost:4173 in your browser.

No installation or build step is required. The website uses HTML, CSS, and JavaScript.

## Features

- Employee and manager demo views
- Purchase requests, approvals, ordering, completion, cancellation, and record removal/restoration
- Location budgets with actual spending, approved commitments, and available funds
- Monthly, quarterly, and yearly spending charts with detailed purchase history
- External funds and spending adjustments

Approval reserves funds; completion moves that amount to spending without counting it twice. Cancellation releases commitments.

## Tests

With Node.js installed:

```sh
node tests/accounting.test.cjs
```

## Files

- `dist/index.html`: page structure
- `dist/style.css`: styling and responsive layout
- `dist/app.js`: application behavior and fictional data
- `tests/accounting.test.cjs`: accounting checks

## Demo limitations

All data is fictional and saved in your browser's local storage. The view switcher is for demonstration, not secure authentication. There is no backend, shared database, or real money transfer. Clearing browser storage resets the demo data.
