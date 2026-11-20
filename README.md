# R & E Kitchen website

A responsive, static restaurant ordering site built from the supplied R and E Kitchen opening flyer. No build step or package install is required.

## Run locally

From this directory, start a static server, for example:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Included

- Restaurant landing page with menu search and categories, opening hours, location details, and directions.
- Cart and checkout for pickup, dine-in, or delivery (delivery fee is set to ₦1,500 in this demo).
- Reservation requests with date, time, guest count, and contact details.
- Customer dashboard with order history, reservation history, and a loyalty wallet.
- Staff dashboard for order status, reservation status, and menu editing / availability.
- Browser `localStorage` persistence for menu, orders, reservations, cart, and customer accounts.

## Credits rule

Customers start with 20 credits. One credit is worth ₦10 in this demo; orders award one credit per ₦1,000 paid. Checkout limits redemption to credits above 20, validates it again when placing an order, and the wallet logic enforces the same floor. The credit policy is visible in the customer wallet and checkout.

## Staff demo

Use **Staff sign in** in the footer and PIN `2026`.

## Important before launch

This is a front-end prototype. Data is stored only in the current browser and is not shared across devices. The demo checkout does not process payments, and the staff PIN is visible in client-side code. Before taking real orders, connect a server/database, add secure customer/staff authentication and permissions, verify the restaurant's menu/prices/delivery zones, and integrate a payment provider and order notifications. The sample menu and delivery fee are editable demo content.
