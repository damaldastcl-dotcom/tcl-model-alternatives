# TCL Model Alternatives picker

A static, single-page tool for L1 and warranty agents.

When a customer's TCL TV model is out of stock, type that model in and the
picker shows which model to send instead, in this order: same size, same
series, same generation first, then next generation, then a different OS as
a platform change needing customer agreement. It also shows 1st, 2nd, and
3rd step-up upgrades, with approval flags on the 2nd and 3rd, a Holiday
path for 2024 Holiday models, an Exclude list for models already known to
be unavailable, and a side-by-side comparison table for the customer's
model versus a selected alternative.

## Files

- `index.html` — the complete picker, self-contained. Open it in a browser
  to use it. No build step and no server code are needed.

## Notes

- Covers 754 TV models.
- The picker does not check live stock.
- This build is the Muse artifact build v18, the picture-match comparison
  build: a Feature column on the left and the two comparing model columns
  side by side on the right, with all 10 comparison rows shown.
