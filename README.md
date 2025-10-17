# Sales Summary Single-Page App

This is a client-side HTML/JavaScript application that fetches CSV data embedded directly in the code, sums the sales values, and displays the total within a styled page. The page uses Bootstrap 5.3.3 loaded from jsDelivr CDN for styling and includes fallback CSS in case Bootstrap fails to load.

## Features

- Sets the document title to `Sales Summary {encodedSeed}`, where the seed encodes contextual info.
- Loads Bootstrap CSS for styling; provides basic fallback styling if Bootstrap fails.
- Parses embedded `data.csv` and computes the total sales.
- Displays the total sales dynamically inside the page.
- Introduces a currency select (`#currency-picker`) that converts the total sales using rates loaded from `rates.json`.
- Mirroring the active currency in `#total-currency`.
- Performs checks to ensure correct document title, CSS loaded, and verified total calculation within a small margin.

## Usage

Open the `index.html` file in a web browser to view the sales summary.

## Notes

- The code is entirely client-side and self-contained.
- The sales data is included inline for simplicity; in production, it might be fetched from an external source.
- The currency converter uses predefined rates (`rates.json`) embedded in the script.
- The app validates the presence of key elements via checks, fulfilling the specified verification. Output exactly in this format with no extra text or markdown code fences (```):