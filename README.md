# NovaCart — ZeroIntern E-Commerce Platform

A polished React + Vite, **frontend/local-first** e-commerce implementation designed around the ZeroIntern Project 1 brief.

## Why this version is GitHub Pages friendly
- Uses hash-based routing (`#/shop`, `#/product/p01`, etc.), so refreshing a deep link on GitHub Pages does not require server rewrites.
- Vite is configured with `base: './'` for relative asset paths.
- Images use lazy loading, async decoding and an automatic fallback image if an external image cannot be reached.
- Top-sales videos are loaded only when their cards approach the viewport instead of downloading all six immediately.
- Cart, wishlist, users, products, categories, videos and orders persist in browser `localStorage`.

## Run locally
```bash
npm install
npm run dev
```
Then open the Vite URL shown in the terminal.

## Production test
```bash
npm run build
npm run preview
```

## Demo accounts
**Customer**
- Email: `demo@novacart.local`
- Password: `Demo@123`

**Admin**
- Email: `admin@novacart.local`
- Password: `Admin@123`

## Included flows
- Home page, category section, top-sales video section and featured products
- 15 products across 6 categories
- Product details, search, category filtering and sorting
- Cart with quantity controls and stock limits
- Wishlist
- Registration + login
- Duplicate-email prevention
- Password validation: 8+ characters, uppercase, lowercase, number and special character
- Customer account dashboard and order history
- Checkout with COD, demo Card and demo PayPal options
- Automatic inventory reduction after an order
- Admin dashboard
- Product CRUD
- Category CRUD
- Top-sales video/poster CRUD
- Order status management
- Customer list
- Responsive desktop/tablet/mobile UI

## Important submission note
This is intentionally a **frontend/local-first** implementation because the requested deployment model does not use a separately hosted backend. PostgreSQL, Express and real Stripe processing therefore are not connected. Card/PayPal checkout is simulated and never charges a real payment method.

For a ZeroIntern submission that specifically requires a deployed REST API, PostgreSQL and real Stripe integration, a separate backend deployment would be required.
