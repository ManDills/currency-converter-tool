# Currency Converter

A single-file EUR → USD currency converter, built to embed in a Notion page.

- No build step, no dependencies, no network calls at runtime.
- Defaults to euros → dollars; ten other currencies available, plus a swap button.
- Light and dark themes follow the viewer's system setting.
- Rates are ECB reference rates, stored in the page. "Edit rate" lets a reader
  override the rate for the current pair with a live or bank-specific quote.

## Hosting

Served by GitHub Pages from the repository root: `index.html`.

## Embedding in Notion

Type `/embed` in a Notion page, paste the Pages URL, and drag the block's
bottom edge to size it.

## Updating rates

Edit the `RATES` object near the top of the `<script>` block in `index.html`,
then update the date in the header and the footnote. Source: European Central
Bank euro reference rates —
<https://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html>
