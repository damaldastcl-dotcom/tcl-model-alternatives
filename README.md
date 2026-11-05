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
  Quantities are real ASP data, never guessed. Current source: ASP
  Inventory Report, November 5, 2026. USA QTY is A stock from ITI FG
  Inventory, TV category only, 89 models. A model in that tab with
  A stock 0 shows QTY 0. A model not in that tab shows no QTY pill.
- Inventory section: Section 3 on the picker page. Type a model number
  to see USA A stock, and Canada A stock and B stock separately from
  Canada FG, TV category only, 28 models. A model not in the file
  shows 0 in this section. The top notice states the inventory date
  and publish time.
  Daily check: weekdays at 9:30am Pacific, silent on days with no new
  ASP file. New files replace the prior day data and are published
  to GitHub as soon as ready.
