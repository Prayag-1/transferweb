# Surgical Mart Nepal

Medical and surgical ecommerce platform for hospitals, clinics, laboratories, and home care providers in Nepal. Built on MERN with Redux Toolkit, admin workflows, and COD checkout.

## Features

- Category- and brand-driven catalog with filters
- Product detail pages with reviews/ratings
- Cart, shipping, and COD-only checkout
- User profiles with order history
- Admin management for products, users, orders, categories, and brands
- Image upload, pagination, and search

## Getting Started

1) Install dependencies

```
npm install
cd frontend && npm install
```

2) Environment

Copy `.env.example` to `.env` and set your values (MongoDB, JWT secret, etc.).

3) Run (dev)

```
npm run dev
```

Frontend uses the proxy in `frontend/package.json` to reach the API on `:5000`.

4) Seed data

```
npm run data:import
```

This loads admin/user accounts, medical categories/brands, and starter products.

## Build

```
cd frontend
npm run build
```

## Notes

- Payments are COD-only; PayPal SDK is removed.
- Keep `PAGINATION_LIMIT` set in `.env` to control listing sizes.
- For production, serve `frontend/build` from `backend/server.js` as configured.
