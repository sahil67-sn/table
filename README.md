# Electronics Items Table

A single-page HTML/CSS project that displays an inventory of electronics items in a styled table, with quantity, per-unit price, line amount, and a grand total.

## Files

| File | Description |
|------|-------------|
| `index.html` | The complete page (HTML and CSS in one file) |

## What It Shows

A table titled **Electronics Items** with these columns:

| Column | Description |
|--------|-------------|
| Sr. No. | Row number (1-10) |
| Product Name | Television, Laptop, Mobile, Tablet, PS5 Ultimate, AC, Sound System, Dyson, Fridge, Inverter |
| Quantity | Number of units |
| Per Unit Price | Price of one unit |
| Amount | Quantity x Per Unit Price |

The last row is a **Total** row that uses `colspan="4"` to span the first four columns, with the grand total in the final column.

## Styling

- `border-collapse: collapse` for a clean single-line grid
- Table centered with `margin: auto` and set to 75% width
- Blue header cells with white text
- Row highlight (dark grey) on hover using `tr:hover`
- Centered text in all cells

## Getting Started

No installation or build step is needed.

1. Save `index.html` to a folder.
2. Open it in any modern web browser.

## Known Issues

- **Data error:** The Television row shows an amount of `1460000`, but 48 x 30000 = `1440000`. The grand total of `9850000` is only correct if the Television amount is `1440000`, so the amount in that row should be corrected.
- The table height is set to `100vh`, which stretches the rows to fill the screen and may look oversized.
- The `border="1px"` attribute on `<table>` is outdated HTML; borders are better handled in CSS.
- The page title is the default "Document".
- Values have no currency symbol or thousands separators, which makes large numbers harder to read.
- Amounts and the total are typed in by hand, so they will not update if quantities or prices change.

## Possible Improvements

- Fix the Television amount to `1440000`
- Use `<thead>`, `<tbody>`, and `<tfoot>` for better structure and accessibility
- Format numbers with currency and separators (e.g., Rs 14,40,000)
- Calculate amounts and the total with JavaScript so they stay accurate
- Add zebra striping, and sorting or search for the table
- Make the table responsive for small screens
- Set a descriptive `<title>`
