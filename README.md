# TCL Model Alternatives picker

A static, single-page tool for L1 and warranty agents.

When a customer's TCL TV model is out of stock, type that model in and the
picker shows which model to send instead, in this order: same size, same
series, same generation first, then next generation, then a different OS as
a platform change needing customer agreement. It also shows 1st, 2nd, and
3rd step-up upgrades, with approval flags on the 2nd and 3rd, a Holiday
path for 2024 Holiday models, an Exclude list for models already known to
be unavailable, and a side-by-side comparison table with the 1st, 2nd,
and 3rd picks as columns, oldest to newest, with the 4th pick named in
a separate line directly under the table.

## Files

- `index.html` — the complete picker, self-contained. Open it in a browser
  to use it. No build step and no server code are needed.

## Notes

- Covers 754 TV models.
- The picker does not check live stock.
- This build is the 3-pick comparison build: a Feature column on the left
  and the 1st, 2nd, and 3rd pick columns side by side on the right, with
  only rows that differ between those picks shown. Each column header
  shows the pick tag and the model year.
- OS swap disclaimer: every different OS pick, including Holiday alternatives that change platform, carries a disclaimer on its card and in the copy list. Do not offer a platform change proactively. Offer only if the customer requested that platform, or if the Warranty Team approves it internally. Fire OS gets an extra sentence: Fire OS is not offered for an OS swap except as an approved exception. Fire picks stay visible, they are not removed.
- Quantity indicators: a blue QTY pill sits above the model number
  wherever a model with a known quantity is listed: comparison headers,
  the 4th pick line, the customer-model summary, main pick cards,
  step-up, size-up, downgrade, Holiday options, and left search chips.
  The quantity table is empty in this publish, per Daniel on Nov 4,
  2026: publish without the example quantities. No pill shows until
  a real quantity is added. Never a guessed quantity.
