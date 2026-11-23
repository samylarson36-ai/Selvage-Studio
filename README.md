# Selvage Studio — online store template (sewing patterns, courses, masterclasses)

Static front-end: HTML + CSS + vanilla JS. No build step.

## Host it
- Vercel: drag the unzipped folder onto vercel.com/new. Netlify: drag it onto app.netlify.com/drop.

## Connect a real backend
1. Products: replace the `P` array in `js/data.js` with a `fetch('/api/products')` call.
2. Payments: in `js/app.js`, inside `#f` `onsubmit`, call your server to create a Checkout Session / payment link
   (Stripe, PayPal, Flutterwave, Paddle or Lemon Squeezy), then redirect to the returned URL.
   Never put secret keys in the front-end.
3. Product images: swap the SVG `art()` for `<img loading="lazy" src="…" width height>` (use WebP/AVIF).

Demo discount code: SEW10
