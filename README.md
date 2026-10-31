# CardWise Deals

A single-page tool for Indian online shoppers. Pick a store (Amazon or Flipkart), your credit card bank, a category and your delivery pincode, and see products ranked by how much your bank's card offers save you, with a link to each listing.

## Run it

No build step. Open `index.html` in a browser, or publish it with GitHub Pages (Settings → Pages → Deploy from branch → `main` / root).

## Data

All products and offers live in the `<script>` block of `index.html`:

- `BANKS`, `CATS`: dropdown options.
- `OFFERS`: bank-wide offer rules (store, categories, % off, cap, minimum order, card-variant limits). Used for products without checked offers.
- `PRODUCTS`: product list. Amazon smartphones carry real ASIN links, prices and per-bank offers checked on 20 Oct 2026, 11:00 IST (logged out, no pincode). Everything else is example data and is labelled that way on the page.

Bank offers change daily, so prices and offers need refreshing before the page is used for real purchases. Pincode delivery is approximated by pincode prefix and is not checked against the stores.
