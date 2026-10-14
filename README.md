# Thala 7 — Sneaker Store (CSS Mini Project)

A multi-page sneaker e-commerce website built with **pure HTML and CSS** — no
Bootstrap, no CSS frameworks, no JavaScript.

## Contents

| File | Purpose |
|------|---------|
| `index.html` | Landing page |
| `product.html` | Product display page |
| `cart.html` | Shopping cart page |
| `payment.html` | Payment / checkout page (`checkout.html` alias) |
| `style.css` | Single stylesheet linked from every page |
| `images/` | Sneaker images (works offline) |
| `README.md` | This file |

## The Four Pages

1. **Landing (`index.html`)** — Navbar (logo left / menu center / search + cart + profile right, Flexbox), hero with two divs (description + "Shop Now" button / sneaker image), full-width service strip (2k+ Reviews, 30k+ Customers, High Quality, 4.5/5 Rating).
2. **Product Display (`product.html`)** — Breadcrumb, main image left / product details right (name, description, ₹1,334, Save 12%, quantity selector, Add to cart), horizontally scrolling image gallery using Flex.
3. **Shopping Cart (`cart.html`)** — "Shopping Cart" heading, table (Product / Quantity / Price / remove icon), coupon input + Apply Coupon, Sub Total / Taxes / Discount / Total, Pay Now button, Razorpay trust icons, Continue Shopping link.
4. **Payment (`payment.html`)** — "Checkout" label, Email ID input, payment method tabs (Card / Crypto / Bank / more), Card Number / Expiry / CVC / Country / ZIP inputs, Order Summary card, Pay Now button, Razorpay icons.

The pages are linked together through the navbar, "Shop Now", "Add to cart", "Pay Now",
and "Continue Shopping" actions.

## How to Run

```bash
# Option 1 — open directly
open index.html

# Option 2 — serve locally (recommended)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Design Notes

- **Colors:** orange `#e07b28` (primary), blue `#1a73e8` (accents), white/grey surfaces.
- **Typography:** Poppins (Google Fonts) with a system-sans fallback.
- **Flexbox:** navbar, hero, service strip, product grid, cart grid, checkout grid, gallery strip, coupon rows, payment tabs.
- **Horizontal scroll:** `.gallery-strip` uses `display: flex` + `overflow-x: auto`.
- **Responsive:** breakpoints at 1024px, 900px and 640px.

## Constraints Met

- ✅ No Bootstrap or any CSS framework
- ✅ Only HTML + CSS, no JavaScript
- ✅ Four separate HTML pages + one stylesheet
- ✅ CSS properly linked via `<link rel="stylesheet" href="style.css">`
- ✅ Navbar & layouts implemented with Flexbox as specified
- ✅ Horizontal scrolling gallery on the product section
- ✅ Coupon input + Apply Coupon, Pay Now and Razorpay trust icons on cart & payment
