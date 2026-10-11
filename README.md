# ManeMuse — Hair Atelier

Full responsive storefront source and original image assets for ManeMuse.

Live site: https://manemuse-hair-atelier.sylviemailletb107185.chatgpt.site/

## Run locally

No build step or dependencies are required. From the repository root:

```sh
python3 -m http.server 8080 --directory dist
```

Open http://localhost:8080. Serve `dist/` as the public directory on any static host.

## Included

- Mobile navigation and desktop storefront
- Product collection, texture finder and multi-angle galleries
- Automatic portrait carousel with reduced-motion support
- Saved styles and shopping bag
- Delivery checkout, shipping estimates, card/bank payment previews
- Original campaign photos, bundled fonts, icons and vendor licenses
- Design notes and checkout regression tests

## Verify

```sh
node --check dist/app.js
node --check dist/checkout.js
node tests/checkout.test.cjs
```

## Payments and orders

Payment screens are previews. No gateway is connected, no card information is collected and no real orders are submitted. Product prices, delivery rates and policies are illustrative. Connect a merchant payment gateway and server-side verification before accepting real payments.

The source matches published Site version 12, commit `04a07763924a15311feec1cb5089ba0ac8b2223b`.
